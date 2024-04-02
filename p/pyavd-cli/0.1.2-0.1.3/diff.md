# Comparing `tmp/pyavd_cli-0.1.2.tar.gz` & `tmp/pyavd_cli-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyavd_cli-0.1.2.tar", max compression
+gzip compressed data, was "pyavd_cli-0.1.3.tar", max compression
```

## Comparing `pyavd_cli-0.1.2.tar` & `pyavd_cli-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0      255 2024-03-04 17:00:10.970570 pyavd_cli-0.1.2/CHANGELOG.md
--rw-r--r--   0        0        0       18 2024-03-04 17:00:10.970570 pyavd_cli-0.1.2/README.md
--rw-r--r--   0        0        0       26 2024-03-04 17:00:10.970570 pyavd_cli-0.1.2/pyavd_cli/__init__.py
--rwxr-xr-x   0        0        0     8166 2024-03-04 17:00:10.970570 pyavd_cli-0.1.2/pyavd_cli/build.py
--rw-r--r--   0        0        0      887 2024-03-04 17:00:17.506623 pyavd_cli-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      539 1970-01-01 00:00:00.000000 pyavd_cli-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      376 2024-04-02 14:48:39.841060 pyavd_cli-0.1.3/CHANGELOG.md
+-rw-r--r--   0        0        0    11344 2024-04-02 14:48:39.841060 pyavd_cli-0.1.3/LICENSE
+-rw-r--r--   0        0        0       18 2024-04-02 14:48:39.841060 pyavd_cli-0.1.3/README.md
+-rw-r--r--   0        0        0      148 2024-04-02 14:48:39.841060 pyavd_cli-0.1.3/pyavd_cli/__init__.py
+-rwxr-xr-x   0        0        0     8758 2024-04-02 14:48:39.841060 pyavd_cli-0.1.3/pyavd_cli/build.py
+-rw-r--r--   0        0        0      898 2024-04-02 14:48:43.889116 pyavd_cli-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      539 1970-01-01 00:00:00.000000 pyavd_cli-0.1.3/PKG-INFO
```

### Comparing `pyavd_cli-0.1.2/pyavd_cli/build.py` & `pyavd_cli-0.1.3/pyavd_cli/build.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,60 @@
-# pylint: disable=missing-module-docstring,missing-function-docstring
+# Copyright (c) 2024 Arista Networks, Inc.
+# Use of this source code is governed by the Apache License 2.0
+# that can be found in the LICENSE file.
 
 import argparse
 import logging
 import os
 import time
 from concurrent.futures import Executor, ProcessPoolExecutor, as_completed
+from functools import wraps
 from pathlib import Path
+from typing import Callable, Optional
 
 import yaml
 from ansible.inventory.manager import InventoryManager  # type: ignore
 from ansible.parsing.dataloader import DataLoader  # type: ignore
 from ansible.parsing.yaml.dumper import AnsibleDumper  # type: ignore
 from ansible.plugins.loader import init_plugin_loader  # type: ignore
 from ansible.template import Templar  # type: ignore
 from ansible.vars.manager import VariableManager  # type: ignore
-from pyavd import (  # type: ignore
+from pyavd import __version__ as pyavd_version  # type: ignore
+from pyavd import (
     get_avd_facts,
     get_device_config,
     get_device_structured_config,
     validate_inputs,
     validate_structured_config,
 )
 
 os.environ["PYAVD"] = "1"
 
 logger = logging.getLogger()
 
 
+def log_execution_time(logger_fn: Callable = logger.debug, log_prefix: Optional[str] = None) -> Callable:
+    def decorator_log_execution_time(func: Callable) -> Callable:
+        @wraps(func)
+        def wrapper(*args, **kwargs):
+            start = time.perf_counter()
+            value = func(*args, **kwargs)
+            logger_fn("%s: %fs", log_prefix or func.__name__, (time.perf_counter() - start))
+            return value
+
+        return wrapper
+
+    return decorator_log_execution_time
+
+
 def validate_hostvars(hostname: str, hostvars: dict, strict: bool):
     results = validate_inputs(hostvars)
     if results.failed:
         for result in results.validation_errors:
-            logger.error(result)
+            logger.error("%s: %s", hostname, result)
         if strict:
             raise RuntimeError(f"{hostname} validate_inputs failed")
 
     return hostname, hostvars
 
 
 def build_structured_config(hostname: str, inputs: dict, avd_facts: dict):
@@ -47,82 +66,33 @@
     return hostname, structured_config
 
 
 def build_device_config(hostname: str, structured_config: dict, strict: bool):
     results = validate_structured_config(structured_config)
     if results.failed:
         for result in results.validation_errors:
-            logger.error(result)
+            logger.error("%s: %s", hostname, result)
         if strict:
             raise RuntimeError(f"{hostname} validate_structured_config failed")
 
     return hostname, get_device_config(structured_config)
 
 
-def build(  # pylint: disable=too-many-arguments,too-many-locals
-    inventory_path: Path,
-    fabric_name: str,
-    limit: str,
-    intended_configs_path: Path,
-    structured_configs_path: Path,
-    max_workers: int = 10,
-    strict: bool = False,
-):
-    init_plugin_loader()
-
-    loader = DataLoader()
-    inventory = InventoryManager(loader=loader, sources=[inventory_path.as_posix()])
-    variable_manager = VariableManager(loader=loader, inventory=inventory)
-
-    templar = Templar(loader=loader)
-
-    all_hostvars = {}
-    for host in inventory.get_hosts(pattern=fabric_name):
-        hostvars = variable_manager.get_vars(host=inventory.get_host(host.name))
-        templar.available_variables = hostvars
-        template_hostvars = templar.template(hostvars, fail_on_undefined=False)
-        all_hostvars[host.name] = template_hostvars
-
-    limit_hostnames = [host.name for host in inventory.get_hosts(pattern=limit)]
-
-    with ProcessPoolExecutor(max_workers=max_workers) as executor:
-        # Validate inputs
-        start = time.time()
-        all_hostvars = validate_all_inputs(all_hostvars, strict, executor)
-        logger.debug("Validate inputs time: %ds", (time.time() - start))
-
-        # Generate facts
-        start = time.time()
-        avd_facts = get_avd_facts(all_hostvars)
-        logger.debug("Generate facts time: %ds", (time.time() - start))
-
-        limit_hostvars = {hostname: hostvars for hostname, hostvars in all_hostvars.items() if hostname in limit_hostnames}
-
-        # Build structured config
-        start = time.time()
-        structured_configs = build_and_write_all_structured_configs(
-            limit_hostvars, avd_facts, structured_configs_path, templar, executor
-        )
-        logger.debug("Build structured config time: %ds", (time.time() - start))
-
-        start = time.time()
-        build_and_write_all_device_configs(intended_configs_path, structured_configs, strict, executor)
-        logger.debug("Build designed config time: %ds", (time.time() - start))
-
-
+@log_execution_time(log_prefix="Validate inputs time")
 def validate_all_inputs(all_hostvars: dict, strict: bool, executor: Executor) -> dict:
     validated_inputs = {}
     futures = [executor.submit(validate_hostvars, hostname, hostvars, strict) for hostname, hostvars in all_hostvars.items()]
     for future in as_completed(futures):
         hostname, hostvars = future.result()
         validated_inputs[hostname] = hostvars
 
     return validated_inputs
 
 
+@log_execution_time(log_prefix="Build structured config time")
 def build_and_write_all_structured_configs(
     all_hostvars: dict,
     avd_facts: dict,
     structured_configs_path: Path,
     templar: Templar,
     executor: Executor,
 ) -> dict:
@@ -147,14 +117,15 @@
                 indent=2,
                 sort_keys=False,
                 width=130,
             )
     return structured_configs
 
 
+@log_execution_time(log_prefix="Build device config time")
 def build_and_write_all_device_configs(
     intended_configs_path: Path,
     structured_configs: dict,
     strict: bool,
     executor: Executor,
 ):
     # Build device config
@@ -167,14 +138,59 @@
     for future in as_completed(futures):
         hostname, device_config = future.result()
 
         with open(intended_configs_path / f"{hostname}.cfg", mode="w", encoding="utf8") as fd:
             fd.write(device_config)
 
 
+@log_execution_time(log_prefix="Total build time")
+def build(  # pylint: disable=too-many-arguments,too-many-locals
+    inventory_path: Path,
+    fabric_name: str,
+    limit: str,
+    intended_configs_path: Path,
+    structured_configs_path: Path,
+    max_workers: int = 10,
+    strict: bool = False,
+):
+    init_plugin_loader()
+
+    loader = DataLoader()
+    inventory = InventoryManager(loader=loader, sources=[inventory_path.as_posix()])
+    variable_manager = VariableManager(loader=loader, inventory=inventory)
+
+    templar = Templar(loader=loader)
+
+    all_hostvars = {}
+    for host in inventory.get_hosts(pattern=fabric_name):
+        hostvars = variable_manager.get_vars(host=inventory.get_host(host.name))
+        templar.available_variables = hostvars
+        template_hostvars = templar.template(hostvars, fail_on_undefined=False)
+        all_hostvars[host.name] = template_hostvars
+
+    limit_hostnames = [host.name for host in inventory.get_hosts(pattern=limit)]
+
+    with ProcessPoolExecutor(max_workers=max_workers) as executor:
+        # Validate inputs
+        all_hostvars = validate_all_inputs(all_hostvars, strict, executor)
+
+        # Generate facts
+        avd_facts = log_execution_time(log_prefix="Generate facts time")(get_avd_facts)(all_hostvars)
+
+        limit_hostvars = {hostname: hostvars for hostname, hostvars in all_hostvars.items() if hostname in limit_hostnames}
+
+        # Build structured config
+        structured_configs = build_and_write_all_structured_configs(
+            limit_hostvars, avd_facts, structured_configs_path, templar, executor
+        )
+
+        # Generate device config
+        build_and_write_all_device_configs(intended_configs_path, structured_configs, strict, executor)
+
+
 def main():
     parser = argparse.ArgumentParser(description="Build AVD fabric.")
     parser.add_argument("-i", "--inventory-path", required=True, type=Path)
     parser.add_argument("-o", "--config-output-path", default=Path("intended"), type=Path)
     parser.add_argument("-f", "--fabric-group-name", required=True, type=str)
     parser.add_argument("-l", "--limit", default="all,!cvp", type=str)
     parser.add_argument("-m", "--max-workers", default=os.cpu_count(), type=int)
@@ -194,30 +210,29 @@
     intended_configs_path = config_output_path / "configs"
     structured_configs_path = config_output_path / "structured_configs"
     max_workers = args.max_workers
     strict = args.strict
     fabric_group_name = args.fabric_group_name
     limit = args.limit
 
+    logger.debug("pyavd version: %s", pyavd_version)
     logger.debug("inventory_path: %s", inventory_path)
     logger.debug("intended_configs_path: %s", intended_configs_path)
     logger.debug("structured_configs_path: %s", structured_configs_path)
     logger.debug("max_workers: %s", max_workers)
     logger.debug("strict: %s", strict)
     logger.debug("fabric_group_name: %s", fabric_group_name)
     logger.debug("limit: %s", limit)
 
-    start = time.time()
     build(
         inventory_path=inventory_path,
         fabric_name=fabric_group_name,
         limit=limit,
         intended_configs_path=intended_configs_path,
         structured_configs_path=structured_configs_path,
         max_workers=max_workers,
         strict=strict,
     )
-    logger.info("Total build time: %ds", (time.time() - start))
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `pyavd_cli-0.1.2/pyproject.toml` & `pyavd_cli-0.1.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 name = "pyavd-cli"
-version = "0.1.2"
+version = "0.1.3"
 description = "A collection of cli scripts to use pyavd"
 authors = ["Arista Networks <eosplus-dev@arista.com>"]
 readme = "README.md"
-include = ["CHANGELOG.md"]
+include = ["CHANGELOG.md", "LICENSE"]
 
 [tool.poetry-dynamic-versioning]
 enable = false
 metadata = false
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `pyavd_cli-0.1.2/PKG-INFO` & `pyavd_cli-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyavd-cli
-Version: 0.1.2
+Version: 0.1.3
 Summary: A collection of cli scripts to use pyavd
 Author: Arista Networks
 Author-email: eosplus-dev@arista.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

