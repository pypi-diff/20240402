# Comparing `tmp/ovp_docker_utils-1.0.3.tar.gz` & `tmp/ovp_docker_utils-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovp_docker_utils-1.0.3.tar", last modified: Thu Mar 28 14:09:39 2024, max compression
+gzip compressed data, was "ovp_docker_utils-1.0.4.tar", last modified: Tue Apr  2 03:28:56 2024, max compression
```

## Comparing `ovp_docker_utils-1.0.3.tar` & `ovp_docker_utils-1.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-03-28 14:09:39.078479 ovp_docker_utils-1.0.3/
--rw-rw-rw-   0        0        0    11527 2024-02-19 17:41:17.000000 ovp_docker_utils-1.0.3/LICENSE
--rw-rw-rw-   0        0        0      380 2024-03-28 14:09:39.077482 ovp_docker_utils-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1431 2024-03-23 02:29:42.000000 ovp_docker_utils-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-03-28 14:09:39.041883 ovp_docker_utils-1.0.3/ovp_docker_utils/
--rw-rw-rw-   0        0        0      361 2024-03-22 19:21:30.000000 ovp_docker_utils-1.0.3/ovp_docker_utils/__init__.py
--rw-rw-rw-   0        0        0       21 2024-03-28 14:06:58.000000 ovp_docker_utils-1.0.3/ovp_docker_utils/__version__.py
--rw-rw-rw-   0        0        0       27 2024-03-22 19:21:25.000000 ovp_docker_utils-1.0.3/ovp_docker_utils/defaults.py
--rw-rw-rw-   0        0        0     2502 2024-03-22 19:21:15.000000 ovp_docker_utils-1.0.3/ovp_docker_utils/docker_compose_instance.py
--rw-rw-rw-   0        0        0     5214 2024-03-22 19:21:11.000000 ovp_docker_utils-1.0.3/ovp_docker_utils/oem_logging.py
--rw-rw-rw-   0        0        0    33465 2024-03-28 14:00:49.000000 ovp_docker_utils-1.0.3/ovp_docker_utils/ovp_docker_utils.py
--rw-rw-rw-   0        0        0     6779 2024-03-22 19:21:01.000000 ovp_docker_utils-1.0.3/ovp_docker_utils/ssh_file_utils.py
--rw-rw-rw-   0        0        0     4077 2024-03-28 14:01:00.000000 ovp_docker_utils-1.0.3/ovp_docker_utils/ssh_key_gen.py
-drwxrwxrwx   0        0        0        0 2024-03-28 14:09:39.076477 ovp_docker_utils-1.0.3/ovp_docker_utils.egg-info/
--rw-rw-rw-   0        0        0      380 2024-03-28 14:09:38.000000 ovp_docker_utils-1.0.3/ovp_docker_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      553 2024-03-28 14:09:38.000000 ovp_docker_utils-1.0.3/ovp_docker_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-28 14:09:38.000000 ovp_docker_utils-1.0.3/ovp_docker_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       75 2024-03-28 14:09:38.000000 ovp_docker_utils-1.0.3/ovp_docker_utils.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       35 2024-03-28 14:09:38.000000 ovp_docker_utils-1.0.3/ovp_docker_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-03-28 14:09:38.000000 ovp_docker_utils-1.0.3/ovp_docker_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       88 2024-02-19 17:41:17.000000 ovp_docker_utils-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-28 14:09:39.078479 ovp_docker_utils-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      910 2024-03-22 13:34:44.000000 ovp_docker_utils-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 03:28:56.261077 ovp_docker_utils-1.0.4/
+-rw-rw-rw-   0        0        0    11527 2024-02-19 17:41:17.000000 ovp_docker_utils-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0      380 2024-04-02 03:28:56.260078 ovp_docker_utils-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1409 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 03:28:56.219748 ovp_docker_utils-1.0.4/ovp_docker_utils/
+-rw-rw-rw-   0        0        0      354 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.4/ovp_docker_utils/__init__.py
+-rw-rw-rw-   0        0        0       21 2024-04-02 03:16:28.000000 ovp_docker_utils-1.0.4/ovp_docker_utils/__version__.py
+-rw-rw-rw-   0        0        0       27 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.4/ovp_docker_utils/defaults.py
+-rw-rw-rw-   0        0        0     2441 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.4/ovp_docker_utils/docker_compose_instance.py
+-rw-rw-rw-   0        0        0     5084 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.4/ovp_docker_utils/oem_logging.py
+-rw-rw-rw-   0        0        0    33420 2024-04-02 03:28:03.000000 ovp_docker_utils-1.0.4/ovp_docker_utils/ovp_docker_utils.py
+-rw-rw-rw-   0        0        0     6556 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.4/ovp_docker_utils/ssh_file_utils.py
+-rw-rw-rw-   0        0        0     3948 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.4/ovp_docker_utils/ssh_key_gen.py
+drwxrwxrwx   0        0        0        0 2024-04-02 03:28:56.259077 ovp_docker_utils-1.0.4/ovp_docker_utils.egg-info/
+-rw-rw-rw-   0        0        0      380 2024-04-02 03:28:56.000000 ovp_docker_utils-1.0.4/ovp_docker_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      553 2024-04-02 03:28:56.000000 ovp_docker_utils-1.0.4/ovp_docker_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 03:28:56.000000 ovp_docker_utils-1.0.4/ovp_docker_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       75 2024-04-02 03:28:56.000000 ovp_docker_utils-1.0.4/ovp_docker_utils.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       35 2024-04-02 03:28:56.000000 ovp_docker_utils-1.0.4/ovp_docker_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-02 03:28:56.000000 ovp_docker_utils-1.0.4/ovp_docker_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       88 2024-02-19 17:41:17.000000 ovp_docker_utils-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-02 03:28:56.262080 ovp_docker_utils-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      878 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.4/setup.py
```

### Comparing `ovp_docker_utils-1.0.3/LICENSE` & `ovp_docker_utils-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ovp_docker_utils-1.0.3/README.md` & `ovp_docker_utils-1.0.4/README.md`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-# O3R docker manager
-
-## Why this library exists
-
-The o3r camera system is setup to facilitate the usage of docker containers to deploy applications to the VPU (OVPxxx).
-
-The ifm3d c++/python api allows a developer to write applications using the o3r on their local machine and then recompile those applications to run directly on the VPU with minimal overhead. This library incorporates lesson from the ifm3d.com documentation on docker implementations. For each robust production ready solution a few common tools and practices are standard. An opinionated set of these tools are provided by this o3r deployment library to facilitate convenient and reliable deployment of 3rd party applications to the o3r platform.
-
-- System for setting up and sharing a common directory between the running application and the rest of the VPU (see docker volumes documentation)
-- Reccommended log cache file structure and logging tools for python (and soon c++)
-- System for collating application logs in a consistent way whenever the developer connects to the vpu to perform updates/troubleshooting
-- "One-click" solution deployment scripting
-
-The following architecture is prescribed to minimize feedback loops during the development process:
-
-![](schematic.drawio.svg)
-
-
-## Quick start (from source)
-
-`pip install -e ./ovp_docker_utils`
-
+# O3R docker manager
+
+## Why this library exists
+
+The o3r camera system is setup to facilitate the usage of docker containers to deploy applications to the VPU (OVPxxx).
+
+The ifm3d c++/python api allows a developer to write applications using the o3r on their local machine and then recompile those applications to run directly on the VPU with minimal overhead. This library incorporates lesson from the ifm3d.com documentation on docker implementations. For each robust production ready solution a few common tools and practices are standard. An opinionated set of these tools are provided by this o3r deployment library to facilitate convenient and reliable deployment of 3rd party applications to the o3r platform.
+
+- System for setting up and sharing a common directory between the running application and the rest of the VPU (see docker volumes documentation)
+- Reccommended log cache file structure and logging tools for python (and soon c++)
+- System for collating application logs in a consistent way whenever the developer connects to the vpu to perform updates/troubleshooting
+- "One-click" solution deployment scripting
+
+The following architecture is prescribed to minimize feedback loops during the development process:
+
+![](schematic.drawio.svg)
+
+
+## Quick start (from source)
+
+`pip install -e ./ovp_docker_utils`
+
 Check out the ovp8xx deployment examples on https://github.com/ifm/ifm3d-examples
```

### Comparing `ovp_docker_utils-1.0.3/ovp_docker_utils/docker_compose_instance.py` & `ovp_docker_utils-1.0.4/ovp_docker_utils/docker_compose_instance.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,61 +1,61 @@
-
-from typing import List, Tuple
-
-import yaml
-from pydantic import BaseModel, model_validator
-
-
-class DockerComposeServiceInstance(BaseModel):
-    """
-    A class to hold the information needed to deploy a docker-compose service instance to the VPU
-
-    For simplicity, use one docker-compose file for each service instance.
-
-    Multiple containers can be deployed from a single docker-compose file using different service names but the autostart daemon will only launch the file using `docker-compose -f <file> up -d` once.
-    """
-    docker_compose_src_on_pc: str
-    docker_compose_dst_on_vpu: str
-    additional_project_files_to_transfer: List[Tuple[str, str]] = []
-    volumes_to_setup: List[Tuple[str, str]] = []
-
-    # The following are optional and can be used to specify the docker image to load onto the VPU
-    # prefer to pull from registry if possible
-    tag_to_pull_from_registry: str = None
-    # otherwise, load from a tar file on the host machine
-    docker_image_src_on_pc: str = None
-    docker_image_dst_on_vpu: str = None
-
-    docker_compose: dict = {}
-
-    @model_validator(mode='after')
-    def validate_constraints(self) -> 'DockerComposeServiceInstance':
-        if not (self.docker_compose_src_on_pc.endswith(".yml") or self.docker_compose_src_on_pc.endswith(".yaml")):
-            raise ValueError(
-                "docker_compose_src_on_pc must be a path to a yaml file")
-        if not self.docker_compose:
-            with open(self.docker_compose_src_on_pc, "r") as f:
-                self.docker_compose = yaml.load(f, yaml.BaseLoader)
-        else:
-            with open(self.docker_compose_src_on_pc, "w") as f:
-                yaml.dump(self.docker_compose, f)
-        return self
-
-    @property
-    def service_name(self):
-        return list(self.docker_compose["services"].keys())[0]
-
-    @property
-    def docker_repository_name(self):
-        return self.docker_compose["services"][self.service_name]["image"].split(":")[0]
-
-    @property
-    def container_name(self):
-        return self.docker_compose["services"][self.service_name]["container_name"]
-
-    @property
-    def log_driver(self):
-        if "logging" not in self.docker_compose["services"][self.service_name]:
-            return None
-        if "driver" not in self.docker_compose["services"][self.service_name]["logging"]:
-            return None
-        return self.docker_compose["services"][self.service_name]["logging"]["driver"]
+
+from typing import List, Tuple
+
+import yaml
+from pydantic import BaseModel, model_validator
+
+
+class DockerComposeServiceInstance(BaseModel):
+    """
+    A class to hold the information needed to deploy a docker-compose service instance to the VPU
+
+    For simplicity, use one docker-compose file for each service instance.
+
+    Multiple containers can be deployed from a single docker-compose file using different service names but the autostart daemon will only launch the file using `docker-compose -f <file> up -d` once.
+    """
+    docker_compose_src_on_pc: str
+    docker_compose_dst_on_vpu: str
+    additional_project_files_to_transfer: List[Tuple[str, str]] = []
+    volumes_to_setup: List[Tuple[str, str]] = []
+
+    # The following are optional and can be used to specify the docker image to load onto the VPU
+    # prefer to pull from registry if possible
+    tag_to_pull_from_registry: str = None
+    # otherwise, load from a tar file on the host machine
+    docker_image_src_on_pc: str = None
+    docker_image_dst_on_vpu: str = None
+
+    docker_compose: dict = {}
+
+    @model_validator(mode='after')
+    def validate_constraints(self) -> 'DockerComposeServiceInstance':
+        if not (self.docker_compose_src_on_pc.endswith(".yml") or self.docker_compose_src_on_pc.endswith(".yaml")):
+            raise ValueError(
+                "docker_compose_src_on_pc must be a path to a yaml file")
+        if not self.docker_compose:
+            with open(self.docker_compose_src_on_pc, "r") as f:
+                self.docker_compose = yaml.load(f, yaml.BaseLoader)
+        else:
+            with open(self.docker_compose_src_on_pc, "w") as f:
+                yaml.dump(self.docker_compose, f)
+        return self
+
+    @property
+    def service_name(self):
+        return list(self.docker_compose["services"].keys())[0]
+
+    @property
+    def docker_repository_name(self):
+        return self.docker_compose["services"][self.service_name]["image"].split(":")[0]
+
+    @property
+    def container_name(self):
+        return self.docker_compose["services"][self.service_name]["container_name"]
+
+    @property
+    def log_driver(self):
+        if "logging" not in self.docker_compose["services"][self.service_name]:
+            return None
+        if "driver" not in self.docker_compose["services"][self.service_name]["logging"]:
+            return None
+        return self.docker_compose["services"][self.service_name]["logging"]["driver"]
```

### Comparing `ovp_docker_utils-1.0.3/ovp_docker_utils/oem_logging.py` & `ovp_docker_utils-1.0.4/ovp_docker_utils/oem_logging.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,130 +1,130 @@
-#############################################
-# Copyright 2021-present ifm electronic, gmbh
-# SPDX-License-Identifier: Apache-2.0
-#############################################
-
-import logging
-import os
-import sys
-from logging.handlers import RotatingFileHandler
-from pathlib import Path
-
-LOG_FORMAT = "%(asctime)s:%(filename)-10s:%(levelname)-8s:%(message)s"
-logging.basicConfig(
-    format=LOG_FORMAT,
-    datefmt="%y-%m-%d %H:%M:%S",
-    stream=sys.stdout,
-    level=logging.INFO,
-)
-logger = logging.getLogger("oem")
-
-
-def setup_log_handler(
-    logger: logging.Logger = logger,
-    total_cached_log_size: int = -1,
-    log_dir: str = "~/ovp8xx_logs",
-    log_series_name: str = "Demos",
-    t_initialized=None,
-    format=LOG_FORMAT,
-    level=logging.INFO,
-) -> str:
-    """
-    Sets up a rotating log handler for the specified logger. NOTE to prevent data loss, be careful when using this tool for local development. If the total_cached_log_size is exceeded, the oldest files in the specified log_dir_name/log_series_name directory will be deleted first. The log files will be stored in the specified log_dir_name/log_series_name directory. The log file name will be the next highest integer in the log_series_name directory, unless t_initialized is specified, in which case the log file name will be the specified t_initialized timestamp.
-
-    Parameters
-    ----------
-    logger : logging.Logger
-        The logger to which the rotating log handler will be added
-    total_cached_log_size : int, optional
-        Number of bytes to limit the specified log directory to. 0 is no log file and no pruning will occur, -1 is unlimited and no pruning will occur, by default 1e8
-    log_dir_name : str, optional
-        Where to find/manage logs can be absolute or relative, by default "logs"
-    log_series_name : str, optional
-        A title for the application or test series, by default "demo"
-    t_initialized : str, optional
-        Timestamp of the test run, by default None
-
-    Returns
-    -------
-    str
-        the path to the log file
-    """
-
-    log_path = None
-    if total_cached_log_size != 0:
-        # Set up logging to file
-        if log_dir[:2] == "..":
-            log_dir = Path(os.getcwd()).parent / log_dir[3:]
-        if log_dir[:1] == "~":
-            log_dir = Path.home() / log_dir[2:]
-        elif Path(log_dir).is_absolute():
-            log_dir = Path(log_dir)
-        else:
-            log_dir = Path(os.getcwd()) / log_dir
-
-        # Setup log directory
-        if not log_dir.exists():
-            os.mkdir(log_dir)
-
-        # Setup log-series directory
-        # Run identifier could be the next int in a series or the specified t_initialized
-        log_series_dir = log_dir / log_series_name
-        if not log_series_dir.exists():
-            os.mkdir(log_series_dir)
-            most_recent_log = 0
-        else:
-            log_entries = os.listdir(log_series_dir)
-            if t_initialized is None:
-                most_recent_log = 0
-                for log_entry in log_entries:
-                    if log_entry[-4:] == ".log":
-                        run_identification = log_entry.replace(".log", "")
-                        if run_identification.isnumeric():
-                            i = int(run_identification)
-                            if i > most_recent_log:
-                                most_recent_log = i
-
-            if total_cached_log_size > 0:
-                # Check for oldest log files to delete them first if necessary
-                log_files = []
-                for root, dirs, files in os.walk(log_series_dir):
-                    for file in files:
-                        path = os.path.join(root, file)
-                        log_files.append(
-                            {
-                                "path": path,
-                                "fname": file,
-                                "size": os.path.getsize(path),
-                                "last_modified": os.path.getmtime(path),
-                            }
-                        )
-                log_files = sorted(log_files, key=lambda k: k["fname"])
-                total_size = 0
-                for log_file in log_files:
-                    total_size += log_file["size"]
-                    if total_size > total_cached_log_size:
-                        os.remove(log_file["path"])
-
-        if t_initialized is None:
-            this_run_identifier = str(most_recent_log + 1)
-        else:
-            this_run_identifier = str(t_initialized)
-
-        log_fname = this_run_identifier + ".log"
-        log_path = log_series_dir / log_fname
-
-        if total_cached_log_size < 0:
-            total_cached_log_size = 0
-        rotating_handler = RotatingFileHandler(
-            log_path,
-            mode="a",
-            maxBytes=total_cached_log_size,
-            backupCount=0,
-            encoding=None,
-            delay=0,
-        )
-        rotating_handler.setFormatter(logging.Formatter(format))
-        rotating_handler.setLevel(level)
-        logger.addHandler(rotating_handler)
-
-    return str(log_path)
+#############################################
+# Copyright 2021-present ifm electronic, gmbh
+# SPDX-License-Identifier: Apache-2.0
+#############################################
+
+import logging
+import os
+import sys
+from logging.handlers import RotatingFileHandler
+from pathlib import Path
+
+LOG_FORMAT = "%(asctime)s:%(filename)-10s:%(levelname)-8s:%(message)s"
+logging.basicConfig(
+    format=LOG_FORMAT,
+    datefmt="%y-%m-%d %H:%M:%S",
+    stream=sys.stdout,
+    level=logging.INFO,
+)
+logger = logging.getLogger("oem")
+
+
+def setup_log_handler(
+    logger: logging.Logger = logger,
+    total_cached_log_size: int = -1,
+    log_dir: str = "~/ovp8xx_logs",
+    log_series_name: str = "Demos",
+    t_initialized=None,
+    format=LOG_FORMAT,
+    level=logging.INFO,
+) -> str:
+    """
+    Sets up a rotating log handler for the specified logger. NOTE to prevent data loss, be careful when using this tool for local development. If the total_cached_log_size is exceeded, the oldest files in the specified log_dir_name/log_series_name directory will be deleted first. The log files will be stored in the specified log_dir_name/log_series_name directory. The log file name will be the next highest integer in the log_series_name directory, unless t_initialized is specified, in which case the log file name will be the specified t_initialized timestamp.
+
+    Parameters
+    ----------
+    logger : logging.Logger
+        The logger to which the rotating log handler will be added
+    total_cached_log_size : int, optional
+        Number of bytes to limit the specified log directory to. 0 is no log file and no pruning will occur, -1 is unlimited and no pruning will occur, by default 1e8
+    log_dir_name : str, optional
+        Where to find/manage logs can be absolute or relative, by default "logs"
+    log_series_name : str, optional
+        A title for the application or test series, by default "demo"
+    t_initialized : str, optional
+        Timestamp of the test run, by default None
+
+    Returns
+    -------
+    str
+        the path to the log file
+    """
+
+    log_path = None
+    if total_cached_log_size != 0:
+        # Set up logging to file
+        if log_dir[:2] == "..":
+            log_dir = Path(os.getcwd()).parent / log_dir[3:]
+        if log_dir[:1] == "~":
+            log_dir = Path.home() / log_dir[2:]
+        elif Path(log_dir).is_absolute():
+            log_dir = Path(log_dir)
+        else:
+            log_dir = Path(os.getcwd()) / log_dir
+
+        # Setup log directory
+        if not log_dir.exists():
+            os.mkdir(log_dir)
+
+        # Setup log-series directory
+        # Run identifier could be the next int in a series or the specified t_initialized
+        log_series_dir = log_dir / log_series_name
+        if not log_series_dir.exists():
+            os.mkdir(log_series_dir)
+            most_recent_log = 0
+        else:
+            log_entries = os.listdir(log_series_dir)
+            if t_initialized is None:
+                most_recent_log = 0
+                for log_entry in log_entries:
+                    if log_entry[-4:] == ".log":
+                        run_identification = log_entry.replace(".log", "")
+                        if run_identification.isnumeric():
+                            i = int(run_identification)
+                            if i > most_recent_log:
+                                most_recent_log = i
+
+            if total_cached_log_size > 0:
+                # Check for oldest log files to delete them first if necessary
+                log_files = []
+                for root, dirs, files in os.walk(log_series_dir):
+                    for file in files:
+                        path = os.path.join(root, file)
+                        log_files.append(
+                            {
+                                "path": path,
+                                "fname": file,
+                                "size": os.path.getsize(path),
+                                "last_modified": os.path.getmtime(path),
+                            }
+                        )
+                log_files = sorted(log_files, key=lambda k: k["fname"])
+                total_size = 0
+                for log_file in log_files:
+                    total_size += log_file["size"]
+                    if total_size > total_cached_log_size:
+                        os.remove(log_file["path"])
+
+        if t_initialized is None:
+            this_run_identifier = str(most_recent_log + 1)
+        else:
+            this_run_identifier = str(t_initialized)
+
+        log_fname = this_run_identifier + ".log"
+        log_path = log_series_dir / log_fname
+
+        if total_cached_log_size < 0:
+            total_cached_log_size = 0
+        rotating_handler = RotatingFileHandler(
+            log_path,
+            mode="a",
+            maxBytes=total_cached_log_size,
+            backupCount=0,
+            encoding=None,
+            delay=0,
+        )
+        rotating_handler.setFormatter(logging.Formatter(format))
+        rotating_handler.setLevel(level)
+        logger.addHandler(rotating_handler)
+
+    return str(log_path)
```

### Comparing `ovp_docker_utils-1.0.3/ovp_docker_utils/ovp_docker_utils.py` & `ovp_docker_utils-1.0.4/ovp_docker_utils/ovp_docker_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,773 +1,788 @@
-#############################################
-# Copyright 2021-present ifm electronic, gmbh
-# SPDX-License-Identifier: Apache-2.0
-#############################################
-
-import os
-import re
-from pathlib import Path
-import sys
-import logging
-import time
-from datetime import datetime
-import subprocess
-import select
-import threading
-from typing import Union, List, Tuple, Dict
-
-from pydantic import BaseModel, model_validator
-from paramiko.client import SSHClient
-from scp import SCPClient
-import semver
-
-try:
-    import ifm3dpy
-    USING_IFM3DPY = True
-except ImportError:
-    USING_IFM3DPY = False
-
-from .oem_logging import setup_log_handler
-from .defaults import DEFAULT_IP
-from .ssh_file_utils import SSH_collect_VPU_handles, SSH_listdir, SSH_path_exists, SSH_isdir, SSH_makedirs, SCP_transfer_item
-from .docker_compose_instance import DockerComposeServiceInstance
-from .ssh_key_gen import assign_key
-
-USING_IPYTHON = "ipykernel" in sys.modules
-if USING_IPYTHON:
-    logger = logging.getLogger("notebook")
-else:
-    logger = logging.getLogger("deploy")
-
-TESTED_COMPATIBLE_FIRMWARE_RANGES = [
-    ["1.0.14", "1.4.30"],
-]
-
-
-def configure_manager_logging(logger: logging.Logger, log_level: str = "", log_dir: str = "~/ovp_logs") -> str:
-    """
-    Configures logging to console and file
-
-    If log level is not specified, only console logging is configured and defaults to INFO level
-
-    Parameters
-    ----------
-    logger : logging.Logger
-        logger to configure
-    log_level : str, optional
-        string level representation one of {"","DEBUG","INFO","CRITICAL","EXCEPTION",...}, by default ""
-    log_dir : str, optional
-        path to log directory, by default "~/ovp_logs"
-    """
-    # Setup console logging
-    log_format = "%(asctime)s:%(filename)-8s:%(levelname)-8s:%(message)s"
-    datefmt = "%y.%m.%d_%H.%M.%S"
-    if not log_level:
-        console_log_level = logging.INFO
-    else:
-        console_log_level = logging.getLevelName(log_level)
-    logging.basicConfig(format=log_format,
-                        level=console_log_level, datefmt=datefmt)
-
-    ts_format = "%y.%m.%d_%H.%M.%S%z"
-    now = datetime.now().astimezone()
-    now_local_ts = now.strftime(ts_format)
-    # Add log file handler
-    if log_dir:
-        log_file = setup_log_handler(
-            logger=logger,
-            total_cached_log_size=-1,  # no pruning of logs, not rollover of log file
-            log_dir=log_dir,
-            log_series_name="Deployments",
-            t_initialized=now_local_ts,
-        )
-    else:
-        log_file = ""
-    return log_file
-
-
-def device_present(IP: str = os.environ.get("IFM3D_IP", DEFAULT_IP), USING_IFM3DPY: bool = ("ipykernel" in sys.modules)) -> bool:
-    if USING_IFM3DPY:
-        logger.info(f"Using ifm3dpy=={ifm3dpy.__version__}")
-    else:
-        logger.info("ifm3dpy unavailable")
-
-    logger.info(f"Checking for device at {IP}")
-    if USING_IFM3DPY:
-        o3r = ifm3dpy.O3R(IP)
-        config = o3r.get()
-        logger.info(f"VPU is connected at {IP}")
-        device_found = True
-    else:
-        logger.info("Trying to connect to VPU without ifm3d")
-        with subprocess.Popen(['ping', IP], stdout=subprocess.PIPE) as process:
-            # Get rid of the first line output from the ping cmd
-            output = process.stdout.readline().decode()
-            device_found = False
-            while True:
-                output = process.stdout.readline().decode()
-                if "unreachable".lower() in output.lower():
-                    break
-                if "bytes" and IP in output:
-                    device_found = True
-                    break
-        logger.info(
-            f"Device is { {False: 'not ',True:''}[device_found]}connected at {IP}")
-
-    return device_found
-
-
-def get_logs(vpu_log_dir: str, local_log_cache: str, vpu_sn: str, ssh: SSHClient, scp: SCPClient, vpu_name: str = "") -> None:
-    """
-    This function caches logs from the vpu to the local machine
-
-    Parameters
-    ----------
-    vpu_log_dir : str
-        path to logs on vpu
-    local_log_cache : str
-        path to cache logs to on local machine
-    IP : str
-        IP address of vpu
-    ssh : SSHClient
-        ssh library native handle
-    scp : SCPClient
-        scp library native handle
-    """
-    if SSH_path_exists(ssh, vpu_log_dir):
-        sn = vpu_sn
-        vpu_specific_log_cache_dir_name = f"sn{sn}"
-        if vpu_name:
-            vpu_specific_log_cache_dir_name += "_"+vpu_name
-
-        local_log_cache = Path(local_log_cache).expanduser().absolute()
-        vpu_specific_local_cache_path = local_log_cache/vpu_specific_log_cache_dir_name
-
-        logger.info(
-            f"Merging {vpu_log_dir} into {vpu_specific_local_cache_path}")
-        # There is some arbitrary behavior around how directories get merged when using scp get but the following works around it
-        if not vpu_specific_local_cache_path.parent.exists():
-            os.makedirs(vpu_specific_local_cache_path.parent)
-        elif vpu_specific_local_cache_path.exists():
-            for item in SSH_listdir(ssh, vpu_log_dir):
-                scp.get(vpu_log_dir+"/"+item,
-                        vpu_specific_local_cache_path, recursive=True)
-        else:
-            scp.get(vpu_log_dir, vpu_specific_local_cache_path, recursive=True)
-    else:
-        logger.info(
-            f"No logs collected from {vpu_log_dir}, directory does not yet exist"
-        )
-
-
-def expand_pc_path(pc_path: str) -> str:
-    pc_path = str(pc_path).replace("~", str(Path().home()))
-    pc_path = pc_path.replace(
-        "./", str(Path(os.getcwd()))+"/").replace("\\", "/")
-    return pc_path
-
-
-def expand_vpu_path(vpu_path: str) -> str:
-    vpu_path = str(vpu_path).replace("~", "/home/oem")
-    return vpu_path
-
-
-def structure_docker_table_output(docker_table: List[str]) -> List[dict]:
-    """
-    This function structures the output of a docker table into a list of dictionaries    
-    """
-    params = [param.strip() for param in docker_table[0].split("  ")if param]
-    param_starting_positions = []
-    param_end_positions = []
-    cursor = 0
-    for param in params:
-        for i in range(cursor, len(docker_table[0])):
-            if docker_table[0][i:].startswith(param):
-                param_starting_positions.append(i)
-                cursor = i + len(param)
-                break
-    param_end_positions = param_starting_positions[1:] + [len(docker_table[0])]
-    entry_dicts = []
-    for running_container in docker_table[1:]:
-        container_dict = {}
-        for param, param_starting_position, param_end_position in zip(params, param_starting_positions, param_end_positions):
-            container_dict[param] = running_container[param_starting_position:param_end_position].strip(
-            )
-        entry_dicts.append(container_dict)
-    return entry_dicts
-
-
-def run_read_print_ssh_loop(ip: str, cmd: str, stop_loop, private_key_path: str, password: str = "oem",  timeout: int = 0, output_buffer: str = "") -> str:
-    """
-    This function runs a command on the remote device and prints the output to the console
-
-    Parameters
-    ----------
-    ip : str
-        IP address of the device
-    cmd : str
-        command to run on the device
-    stop_loop : bool
-        thread safe callable flag to stop the loop
-    private_key_path : str
-        path to private key
-    password : str
-        password for the device
-    timeout : int
-        time to run the loop for
-    output_buffer : str
-        buffer to store output
-
-    Returns
-    -------
-    str
-        output of the command
-    """
-    ssh, scp = SSH_collect_VPU_handles(
-        IP=ip, password=password, private_key_path=private_key_path)
-    ssh: SSHClient = ssh
-    transport = ssh.get_transport()
-    channel = transport.open_session()
-    channel.exec_command(cmd)
-
-    start = time.perf_counter()
-    try:
-        while not channel.exit_status_ready() and (not timeout or time.perf_counter() < start+timeout) and not stop_loop():
-            rl, wl, xl = select.select([channel], [], [], 0.0)
-            if len(rl) > 0:
-                # Must be stdout
-                output = channel.recv(1024).decode()
-                if output:
-                    print(output, end="")
-                    output_buffer += [output]
-    except:
-        pass
-    return output_buffer
-
-
-class ManagerConfig(BaseModel):
-    IP: str = os.environ.get("IFM3D_IP", DEFAULT_IP)
-    possible_initial_ip_addresses_to_try: List[str] = []
-    log_level: str = "INFO"
-    log_dir: str = "~/ovp_logs"
-    ssh_key_dir: str = "~/.ssh/"
-    oem_user_password: str = "oem"
-    ssh_key_file_name: str = "id_rsa_ovp8xx"
-
-
-class Manager:
-    def __init__(
-        self,
-        config: ManagerConfig = ManagerConfig(),
-    ):
-        """
-        This class handles the deployment of docker containers to the OVP8XX. It is a thin wrapper around the ifm3dpy library, the paramiko and scp libraries for SSH and SCP respectively, and the docker command line interface on the VPU.
-
-        The objective here is to minimize magic and maximize transparency. The user should be able to see exactly what is happening on the VPU and be able to interact with the VPU directly if desired. Manager.o3r is the native ifm3dpy handle to the VPU. Manager.ssh and Manager.scp are the native paramiko and scp handles to the VPU respectively.
-
-        Each cli command run on the VPU (outside of simple filesystem operations from ovp_docker_utils.ssh_file_utils) is logged so that issues can be debugged if they arise.
-        """
-
-        self.config: ManagerConfig = config
-
-        self._log_file_path = configure_manager_logging(
-            logger,
-            self.config.log_level,
-            self.config.log_dir
-        )
-
-        self._connected = False
-        self._o3r = None
-        self._ssh = None
-        self._scp = None
-        self._fw_version = None
-        self.private_key_path = None
-
-        self.connect()
-
-    @property
-    def log_file_path(self):
-        return self._log_file_path
-
-    @property
-    def connected(self):
-        return self._connected
-
-    @property
-    def o3r(self):
-        return self._o3r
-
-    @property
-    def ssh(self):
-        return self._ssh
-
-    @property
-    def scp(self):
-        return self._scp
-
-    @property
-    def vpu_config(self):
-        if not self._o3r:
-            raise Exception("Not connected to device")
-        return self._o3r.get()
-
-    @property
-    def fw_version(self):
-        if not self._o3r:
-            raise Exception("Not connected to device")
-        return self._fw_version
-
-    @property
-    def vpu_sn(self):
-        return self.vpu_config["device"]["info"]["serialNumber"]
-
-    @property
-    def vpu_name(self):
-        return self.vpu_config["device"]["info"]["name"]
-
-    def connect(self,) -> bool:
-
-        if not USING_IFM3DPY:
-            logger.info("ifm3dpy unavailable")
-        if USING_IFM3DPY and self.config.possible_initial_ip_addresses_to_try:
-            possible_initial_ip_addresses = list(
-                set([self.config.IP] + self.config.possible_initial_ip_addresses_to_try))
-            if len(possible_initial_ip_addresses) > 1:
-                logger.info(
-                    f"Trying to connect to VPU at any of the following addresses: {possible_initial_ip_addresses}")
-
-                for temp_IP in possible_initial_ip_addresses:
-                    try:
-                        VPU_config = ifm3dpy.O3R(temp_IP).get()
-                        logger.info(f"Connected to {temp_IP}")
-                        self._connected = True
-                        break
-                    except Exception as e:
-                        if "XMLRPC Timeout" in str(e):
-                            continue
-                        raise e
-                if not self._connected:
-                    logger.info(
-                        f"VPU could not be found at any of the following addresses: {possible_initial_ip_addresses}")
-                elif temp_IP != self.config.IP:
-                    logger.info(
-                        f"Updating IP address from {temp_IP} to {self.config.IP}")
-                    gateway = ".".join(
-                        self.config.IP.split(".")[:-1] + ["255"])
-                    mask = 24
-                    ifm3dpy.O3R(temp_IP).set({"device": {"network": {"interfaces": {"eth0": {
-                        "ipv4": {
-                            "address": self.config.IP,
-                            "gateway": gateway,
-                            "mask": mask
-                        }}}}}})  # in c
-                    ifm3dpy.O3R(temp_IP).reboot()
-                    wait_period = 80
-                    logger.info(f"Waiting 80s for VPU to reboot.")
-                    heartbeat_rate = 2
-                    for x in range(int(wait_period/heartbeat_rate)):
-                        print(".", end="")
-                        time.sleep(heartbeat_rate)
-        if USING_IFM3DPY and self._connected:
-            self._o3r = ifm3dpy.O3R(self.config.IP)
-            self._fw_version = ".".join(self.vpu_config["device"]["swVersion"]["firmware"].split(
-                "-")[0].split(".")[:3])  # get the first 3 parts of the version number
-
-            logger.info(f"Device firmware version: {self._fw_version}")
-
-            # Check for firmware compatibility
-            if not any(
-                    [semver.compare(self._fw_version, range[0])*semver.compare(range[1], self._fw_version) == 1 for range in TESTED_COMPATIBLE_FIRMWARE_RANGES]):
-                raise Exception(
-                    f"Device firmware version {self._fw_version} is not compatible with version of the deployment manager (tested with the following ranges: {TESTED_COMPATIBLE_FIRMWARE_RANGES})")
-
-            self.private_key_path = assign_key(
-                ip=self.config.IP, target_dir=self.config.ssh_key_dir, key_title=self.config.ssh_key_file_name)
-
-            logger.info(f"private_key_path = {self.private_key_path}")
-
-            try:
-                self._ssh, self._scp = SSH_collect_VPU_handles(
-                    IP=self.config.IP, password=self.config.oem_user_password, private_key_path=self.private_key_path)
-            except Exception as e:
-                logger.info(
-                    f"Device is present but failed to connect via ssh: {e}")
-                self._connected = False
-                raise e
-
-            logger.info(
-                f"Device accessible using ifm3dpy=={ifm3dpy.__version__} and ssh connected")
-        return self._connected
-
-    def mkdir(self, dir_path: str) -> None:
-        if not SSH_path_exists(self._ssh, dir_path):
-            cmd = f"mkdir {dir_path}"
-            logger.info(cmd)
-            _stdin, _stdout, _stderr = self._ssh.exec_command(cmd)
-            logger.info(
-                f">>> {_stderr.read().decode().strip()} {_stdout.read().decode().strip()}")
-
-    def append_deployment_timestamp(self, deployment_timestamp_path: str = "~/share/Deployments") -> None:
-        cmd = f'echo "{Path(self._log_file_path).name[:-4]}" >> {deployment_timestamp_path}'
-        logger.info(cmd)
-        _stdin, _stdout, _stderr = self._ssh.exec_command(cmd)
-        logger.info(
-            f">>> {_stderr.read().decode().strip()} {_stdout.read().decode().strip()}")
-
-    def append_docker_registry(self, docker_registry_host: str = "", docker_registry_port: int = 5000) -> None:
-        insecure_registries = self.vpu_config["device"]["docker"]["insecure-registries"]
-        if docker_registry_host and docker_registry_port:
-            if f"{docker_registry_host}:{docker_registry_port}" not in insecure_registries:
-                logger.info(
-                    f"Adding {docker_registry_host}:{docker_registry_port} to insecure registries in VPU config")
-                if len(insecure_registries) > 2:
-                    logger.warning(
-                        f"VPU already has {len(insecure_registries)} insecure registries, adding more is not permitted, the last one will be replaced")
-                    insecure_registries.pop()
-                insecure_registries.append(
-                    f"{docker_registry_host}:{docker_registry_port}")
-                self._o3r.set(
-                    {"device": {"docker": {"insecure-registries": insecure_registries}}})
-                logger.info(
-                    f"Success! {docker_registry_host}:{docker_registry_port} added to insecure registries in VPU config, restarting the vpu to apply changes")
-                self._o3r.reboot()
-                timeout = 100
-                logger.info(
-                    f"VPU rebooting, waiting {timeout}s for it to come back online")
-                heartbeat_rate = 2
-                for x in range(timeout//heartbeat_rate):
-                    print(".", end="")
-                    time.sleep(heartbeat_rate)
-                self.connect()
-
-            else:
-                logger.info(
-                    f"{docker_registry_host}:{docker_registry_port} already in insecure registries in VPU config")
-
-    def transfer_to_vpu(self, src: str, dst: str) -> None:
-        src = expand_pc_path(src)
-        dst = expand_vpu_path(dst)
-        if Path(src).exists():
-            logger.info(
-                f"transferring {src} to {dst}")
-            SCP_transfer_item(
-                self._ssh, self._scp, src, dst, True)
-        else:
-            logger.info(f"file not found '{src}'")
-
-    def transfer_from_vpu(self, src: str, dst: str) -> None:
-        src = expand_vpu_path(src)
-        dst = expand_pc_path(dst)
-        if SSH_path_exists(self._ssh, src):
-            logger.info(
-                f"Transferring {src} to {dst}")
-            SCP_transfer_item(
-                self._ssh, self._scp, src, dst, False)
-        else:
-            logger.info(f"file not found '{src}'")
-
-    def get_running_docker_containers(self) -> List[str]:
-        cmd = "docker ps -a"
-        _stdin, _stdout, _stderr = self._ssh.exec_command(cmd)
-        running_containers_list = _stdout.read().decode().strip().split("\n")
-        return structure_docker_table_output(running_containers_list)
-
-    def remove_running_docker_containers(self, running_containers_to_remove: list = []) -> None:
-        for running_container in running_containers_to_remove:
-            cmd = f"docker rm -f {running_container['CONTAINER ID']}"
-            logger.info(cmd)
-            _stdin, _stdout, _stderr = self._ssh.exec_command(cmd)
-            logger.info(f">>>{_stdout.read().decode().strip()}")
-
-    def get_cached_docker_images(self) -> List[str]:
-        cmd = "docker image ls"
-        _stdin, _stdout, _stderr = self._ssh.exec_command(cmd)
-        cached_images_list = _stdout.read().decode().strip().split("\n")
-        return structure_docker_table_output(cached_images_list)
-
-    def remove_cached_docker_images(self, cached_images_to_remove: list = []) -> None:
-        for cached_container in cached_images_to_remove:
-            cmd = f"docker image rm {cached_container['IMAGE ID']}"
-            logger.info(cmd)
-            _stdin, _stdout, _stderr = self._ssh.exec_command(cmd)
-            logger.info(f">>>{_stdout.read().decode().strip()}")
-
-    def get_registered_docker_volumes(self) -> List[str]:
-        cmd = "docker volume ls"
-        _stdin, _stdout, _stderr = self._ssh.exec_command(cmd)
-        cached_images_list = _stdout.read().decode().strip().split("\n")
-        return structure_docker_table_output(cached_images_list)
-
-    def remove_registered_docker_volumes(self, registered_volumes_to_remove: list = []) -> None:
-        for volume in registered_volumes_to_remove:
-            cmd = f"docker volume rm {volume['VOLUME NAME']}"
-            logger.info(cmd)
-            _stdin, _stdout, _stderr = self._ssh.exec_command(cmd)
-            logger.info(f">>>{_stdout.read().decode().strip()}")
-
-    def get_logs(self, vpu_log_dir: str = "/home/oem/share/logs", local_log_cache: str = "~/ovp_logs/From_VPUs") -> None:
-        get_logs(
-            vpu_log_dir=vpu_log_dir,
-            local_log_cache=local_log_cache,
-            vpu_sn=self.vpu_sn,
-            scp=self._scp,
-            ssh=self._ssh,
-        )
-
-    def set_vpu_name(self, set_vpu_name: str) -> None:
-        logger.info(f"Setting device name to {set_vpu_name}")
-        self._o3r.set({"device": {"info": {"name": set_vpu_name}}})
-
-    def mount_usb(self) -> list:
-        cmd = f"mount"
-        logger.info(cmd)
-        _stdin, _stdout, _stderr = self.ssh.exec_command(cmd)
-        output = _stdout.read().decode().strip()
-        logger.info(">>>" + output.split("\n")
-                    [0] + " ..." + _stderr.read().decode().strip())
-        mounted_disks_dirs = [disk_desc.split(
-            " ")[2] for disk_desc in output.split("\n") if ("autofs" in disk_desc)]
-        return mounted_disks_dirs
-
-    def disk_is_available(self, known_disk_name: str) -> bool:
-        self.mount_usb()
-        disk_dir = "/run/media/system/" + known_disk_name
-        logger.info(f"Checking if disk is available at {disk_dir}")
-        disk_is_available = SSH_path_exists(self._ssh, disk_dir)
-        return disk_is_available
-
-    def setup_docker_volume(self, path_for_volume_to_mount: str, volume_name: str) -> None:
-        # setup volume as specified
-        cmd = f'docker volume create --driver local -o o=bind -o type=none -o device="{path_for_volume_to_mount}" {volume_name}'
-        _stdin, _stdout, _stderr = self._ssh.exec_command(cmd)
-        logger.info(cmd)
-        if _stdout.read().decode().strip() == volume_name:
-            logger.info("Success!")
-        else:
-            logger.info("Issue encountered while setting up shared volume")
-            raise Exception(_stderr.read().decode().strip())
-
-    def import_docker_image(self, image_to_import: str) -> None:
-        # load image
-        docker_image_fname = Path(image_to_import).name
-        logger.info("importing image into vpu docker storage")
-        cmd = f"cat {image_to_import}| docker import - {docker_image_fname[:-4]}"
-        logger.info(cmd)
-        _stdin, _stdout, _stderr = self._ssh.exec_command(cmd)
-        logger.info(">>>"+_stdout.read().decode().strip() +
-                    _stderr.read().decode().strip())
-
-    def load_docker_image(self, image_to_load: str, update_tag_on_VPU_to: str = "") -> None:
-        # load image
-        docker_image_fname = Path(image_to_load).name
-        logger.info("loading image into vpu docker storage")
-        cmd = f"docker load -i {image_to_load}"
-        logger.info(cmd)
-        _stdin, _stdout, _stderr = self._ssh.exec_command(cmd)
-        stdout = _stdout.read().decode().strip()
-        logger.info(">>>"+stdout +
-                    _stderr.read().decode().strip())
-        if "Loaded image" not in stdout:
-            logger.warning("Issue encountered while loading image")
-        elif update_tag_on_VPU_to:
-            tag_of_loaded_image = stdout.strip().split(" ")[-1]
-            cmd = f"docker tag {tag_of_loaded_image} {update_tag_on_VPU_to}"
-            logger.info(cmd)
-            _stdin, _stdout, _stderr = self._ssh.exec_command(cmd)
-            logger.info(">>>"+_stdout.read().decode().strip() +
-                        _stderr.read().decode().strip())
-
-    def pull_docker_image_from_registry(self, docker_registry_host: str, docker_registry_port: int, docker_repository_name: str, docker_image_tag: str = "latest", update_tag_on_VPU_to: str = "") -> None:
-        # pull image
-        logger.info("pulling image from local registry (this may take a while)")
-        cmd = f"docker pull {docker_registry_host}:{docker_registry_port}/{docker_repository_name}:{docker_image_tag}"
-        logger.info(cmd)
-        _stdin, _stdout, _stderr = self._ssh.exec_command(cmd)
-        logger.info(">>>"+_stdout.read().decode().strip() +
-                    _stderr.read().decode().strip())
-
-        if update_tag_on_VPU_to:
-            cmd = f"docker tag {docker_registry_host}:{docker_registry_port}/{docker_repository_name}:{docker_image_tag} {update_tag_on_VPU_to}"
-            logger.info(cmd)
-            _stdin, _stdout, _stderr = self._ssh.exec_command(cmd)
-            logger.info(">>>"+_stdout.read().decode().strip() +
-                        _stderr.read().decode().strip())
-
-    def rm_item(self, item_to_rm: str) -> None:
-        if SSH_path_exists(self._ssh, item_to_rm):
-            logger.info(f"Removing {item_to_rm}")
-            if SSH_isdir(self._ssh, item_to_rm):
-                cmd = f"rm -r {item_to_rm}"
-                logger.info(cmd)
-                _stdin, _stdout, _stderr = self._ssh.exec_command(cmd)
-                logger.info(_stdout.read().decode().strip() +
-                            _stderr.read().decode().strip())
-            else:
-                cmd = f"rm {item_to_rm}"
-                logger.info(cmd)
-                _stdin, _stdout, _stderr = self._ssh.exec_command(cmd)
-                logger.info(">>>"+_stdout.read().decode().strip() +
-                            _stderr.read().decode().strip())
-
-    def enable_autostart(self, docker_compose_fname: str, service_name: str) -> None:
-        # check if symlink already exists
-        docker_compose_dir = f"/usr/share/oem/docker/compose/{service_name}"
-
-        docker_compose_vpu_path = docker_compose_dir+"/docker-compose.yml"
-
-        if not SSH_path_exists(self._ssh, docker_compose_vpu_path):
-            logger.info(
-                "no docker-compose symlink for auto-start found, setting it up now")
-            SSH_makedirs(self._ssh, docker_compose_dir)
-            cmd = f"ln -s {docker_compose_fname} {docker_compose_vpu_path}"
-            logger.info(cmd)
-            _stdin, _stdout, _stderr = self._ssh.exec_command(cmd)
-            logger.info(
-                f">>> {_stderr.read().decode().strip()} {_stdout.read().decode().strip()}")
-
-        logger.info("Enabling autostart...")
-        cmd = f'systemctl --user enable oem-dc@{service_name}'
-        logger.info(cmd)
-        _stdin, _stdout, _stderr = self._ssh.exec_command(cmd)
-        output = _stdout.read().decode().strip()
-
-    def autostart_enabled(self, service_name: str) -> bool:
-        cmd = f"systemctl --user status oem-dc@{service_name}"
-        logger.info(cmd)
-        _stdin, _stdout, _stderr = self._ssh.exec_command(cmd)
-        # logger.info(
-        #     f">>> {_stderr.read().decode().strip()} {_stdout.read().decode().strip()}")
-        output = _stdout.read().decode().strip()
-        return "enabled;" in output
-
-    def get_all_autostart_instances(self) -> List[str]:
-        cmd = f"ls /home/oem/.config/systemd/user/default.target.wants/"
-        logger.info(cmd)
-        _stdin, _stdout, _stderr = self._ssh.exec_command(cmd)
-        output = _stdout.read().decode().strip()
-        # Regular expression pattern
-        pattern = r'oem-dc@(.*?).service'
-        # Find matches
-        matches = re.findall(pattern, output)
-        logger.info(">>>" + output)
-        return matches
-
-    def disable_autostart(self, service_name: str) -> None:
-        logger.info("disabling autostart...")
-        cmd = f'systemctl --user disable oem-dc@{service_name}'
-        logger.info(cmd)
-        _stdin, _stdout, _stderr = self._ssh.exec_command(cmd)
-        logger.info(
-            f">>> {_stderr.read().decode().strip()} {_stdout.read().decode().strip()}")
-
-    def stop_container(self, service_name: str):
-        cmd = f"docker rm -f {service_name}"
-        logger.info(f"Stopping container with: {cmd}")
-        _stdin, _stdout, _stderr = self._ssh.exec_command(cmd)
-        logger.info(">>>" + _stdout.read().decode().strip() +
-                    _stderr.read().decode().strip())
-
-    def initialize_container(self, service: DockerComposeServiceInstance, pipe_duration: float = 0, stop_upon_exit: bool = False, trigger_to_close_container: str = "") -> None:
-        initialized = False
-
-        non_standard_docker_logger_used = service.log_driver is not None
-
-        if non_standard_docker_logger_used or not pipe_duration:
-            # detach from the container immediately
-            cmd = f"docker-compose -f {service.docker_compose_dst_on_vpu} up --d --remove-orphan {service.service_name} "
-            _stdin, _stdout, _stderr = self._ssh.exec_command(cmd)
-            logger.info(cmd)
-            output_lines_from_container = _stdout.read().decode().strip().split("\n")
-            logger.info(
-                f">>> {_stderr.read().decode().strip()} {' '.join(output_lines_from_container)}")
-            logger.info(
-                f"{service.service_name} initialized from {service.docker_compose_dst_on_vpu}")
-
-            initialized = True
-
-        else:
-            output_lines_from_container = []
-
-        if pipe_duration:
-            if initialized:
-                cmd = f"docker attach {service.container_name}"
-                logger.info(
-                    f"Now Attempting to show output from {service.container_name}: {cmd}")
-            else:
-                cmd = f"docker-compose -f {service.docker_compose_dst_on_vpu} up {service.service_name}"
-                logger.info(
-                    f"Initializing service and showing output of container as it appears to be using the standard logger... {cmd}")
-
-            output_lines_from_container += self.attach_to_container(
-                cmd=cmd,
-                container_name=service.container_name,
-                pipe_duration=pipe_duration,
-                stop_upon_exit=stop_upon_exit,
-                trigger_to_close_container=trigger_to_close_container,
-            )
-
-        # check if any non-ssd safe logging drivers are allowed in the docker-compose file
-        ssd_safe_docker_logging_drivers = ["none", "local"]
-        if service.log_driver not in ssd_safe_docker_logging_drivers:
-            logger.critical(
-                f"Write-intensive Docker logging driver used for service '{service.service_name}'. Try using: \nlogging:\n   driver: \"none\" ")
-
-        return output_lines_from_container
-
-    def attach_to_container(self, cmd: str = "", container_name: str = "", pipe_duration: float = 20, stop_upon_exit: bool = False, trigger_to_close_container: str = "") -> List[str]:
-
-        if not cmd:
-            cmd = f"docker attach {container_name}"
-        output_lines_from_container = []
-
-        stop_loop = False
-        print_loop_thread = threading.Thread(
-            target=run_read_print_ssh_loop,
-            args=(self.config.IP, cmd, lambda: stop_loop, self.private_key_path,
-                  self.config.oem_user_password, pipe_duration, output_lines_from_container),
-            daemon=True
-        )
-        n_output_lines = len(output_lines_from_container)
-        print_loop_thread.start()
-        start_t = time.perf_counter()
-        while not stop_loop:
-            try:
-                time.sleep(0.2)
-                if pipe_duration > 0 and time.perf_counter() > start_t+pipe_duration:
-                    logger.info(
-                        f"run_duration of {pipe_duration} seconds has been reached, detaching from container...")
-                    stop_loop = True
-                else:
-                    # check if new output lines have been added
-                    if len(output_lines_from_container) > n_output_lines:
-                        latest_lines = output_lines_from_container[n_output_lines:]
-                        n_output_lines = len(output_lines_from_container)
-                        if any([" exited with code 0\n\x1b[0m" in line for line in latest_lines]):
-                            logger.info("Container exited with code 0")
-                            stop_loop = True
-                        if trigger_to_close_container and any([trigger_to_close_container in line for line in latest_lines]):
-                            logger.info(
-                                f"Container exited with trigger: {trigger_to_close_container}")
-                            stop_loop = True
-            except KeyboardInterrupt:
-                logger.info(
-                    "KeyboardInterrupt detected, Detaching from container...")
-                stop_loop = True
-
-        if stop_upon_exit:
-            logger.info("Stopping container...")
-            self.stop_container(service_name=container_name)
-            time.sleep(0.5)
-        time.sleep(0.5)
-        if not print_loop_thread.is_alive():
-            print_loop_thread.join()
-        else:
-            logger.info(
-                "Failed to stop container monitor thread... it will exit with the program exit")
-
-        output_lines_from_container = output_lines_from_container.copy()
-        del (print_loop_thread)
-        time.sleep(2)
-
-        logger.info("Container monitor thread stopped")
-
-        return output_lines_from_container
+#############################################
+# Copyright 2021-present ifm electronic, gmbh
+# SPDX-License-Identifier: Apache-2.0
+#############################################
+
+import os
+import re
+from pathlib import Path
+import sys
+import logging
+import time
+from datetime import datetime
+import subprocess
+import select
+import threading
+from typing import Union, List, Tuple, Dict
+
+from pydantic import BaseModel, model_validator
+from paramiko.client import SSHClient
+from scp import SCPClient
+import semver
+
+try:
+    import ifm3dpy
+    USING_IFM3DPY = True
+except ImportError:
+    USING_IFM3DPY = False
+
+from .oem_logging import setup_log_handler
+from .defaults import DEFAULT_IP
+from .ssh_file_utils import SSH_collect_VPU_handles, SSH_listdir, SSH_path_exists, SSH_isdir, SSH_makedirs, SCP_transfer_item
+from .docker_compose_instance import DockerComposeServiceInstance
+from .ssh_key_gen import assign_key
+
+USING_IPYTHON = "ipykernel" in sys.modules
+if USING_IPYTHON:
+    logger = logging.getLogger("notebook")
+else:
+    logger = logging.getLogger("deploy")
+
+TESTED_COMPATIBLE_FIRMWARE_RANGES = [
+    ["1.0.14", "1.4.30"],
+]
+
+
+def configure_manager_logging(logger: logging.Logger, log_level: str = "", log_dir: str = "~/ovp_logs") -> str:
+    """
+    Configures logging to console and file
+
+    If log level is not specified, only console logging is configured and defaults to INFO level
+
+    Parameters
+    ----------
+    logger : logging.Logger
+        logger to configure
+    log_level : str, optional
+        string level representation one of {"","DEBUG","INFO","CRITICAL","EXCEPTION",...}, by default ""
+    log_dir : str, optional
+        path to log directory, by default "~/ovp_logs"
+    """
+    # Setup console logging
+    log_format = "%(asctime)s:%(filename)-8s:%(levelname)-8s:%(message)s"
+    datefmt = "%y.%m.%d_%H.%M.%S"
+    if not log_level:
+        console_log_level = logging.INFO
+    else:
+        console_log_level = logging.getLevelName(log_level)
+    logging.basicConfig(format=log_format,
+                        level=console_log_level, datefmt=datefmt)
+
+    ts_format = "%y.%m.%d_%H.%M.%S%z"
+    now = datetime.now().astimezone()
+    now_local_ts = now.strftime(ts_format)
+    # Add log file handler
+    if log_dir:
+        log_file = setup_log_handler(
+            logger=logger,
+            total_cached_log_size=-1,  # no pruning of logs, not rollover of log file
+            log_dir=log_dir,
+            log_series_name="Deployments",
+            t_initialized=now_local_ts,
+        )
+    else:
+        log_file = ""
+    return log_file
+
+
+def device_present(IP: str = os.environ.get("IFM3D_IP", DEFAULT_IP), USING_IFM3DPY: bool = ("ipykernel" in sys.modules)) -> bool:
+    if USING_IFM3DPY:
+        logger.info(f"Using ifm3dpy=={ifm3dpy.__version__}")
+    else:
+        logger.info("ifm3dpy unavailable")
+
+    logger.info(f"Checking for device at {IP}")
+    if USING_IFM3DPY:
+        o3r = ifm3dpy.O3R(IP)
+        config = o3r.get()
+        logger.info(f"VPU is connected at {IP}")
+        device_found = True
+    else:
+        logger.info("Trying to connect to VPU without ifm3d")
+        with subprocess.Popen(['ping', IP], stdout=subprocess.PIPE) as process:
+            # Get rid of the first line output from the ping cmd
+            output = process.stdout.readline().decode()
+            device_found = False
+            while True:
+                output = process.stdout.readline().decode()
+                if "unreachable".lower() in output.lower():
+                    break
+                if "bytes" and IP in output:
+                    device_found = True
+                    break
+        logger.info(
+            f"Device is { {False: 'not ',True:''}[device_found]}connected at {IP}")
+
+    return device_found
+
+
+def get_logs(vpu_log_dir: str, local_log_cache: str, vpu_sn: str, ssh: SSHClient, scp: SCPClient, vpu_name: str = "") -> None:
+    """
+    This function caches logs from the vpu to the local machine
+
+    Parameters
+    ----------
+    vpu_log_dir : str
+        path to logs on vpu
+    local_log_cache : str
+        path to cache logs to on local machine
+    IP : str
+        IP address of vpu
+    ssh : SSHClient
+        ssh library native handle
+    scp : SCPClient
+        scp library native handle
+    """
+    if SSH_path_exists(ssh, vpu_log_dir):
+        sn = vpu_sn
+        vpu_specific_log_cache_dir_name = f"sn{sn}"
+        if vpu_name:
+            vpu_specific_log_cache_dir_name += "_"+vpu_name
+
+        local_log_cache = Path(local_log_cache).expanduser().absolute()
+        vpu_specific_local_cache_path = local_log_cache/vpu_specific_log_cache_dir_name
+
+        logger.info(
+            f"Merging {vpu_log_dir} into {vpu_specific_local_cache_path}")
+        # There is some arbitrary behavior around how directories get merged when using scp get but the following works around it
+        if not vpu_specific_local_cache_path.parent.exists():
+            os.makedirs(vpu_specific_local_cache_path.parent)
+        elif vpu_specific_local_cache_path.exists():
+            for item in SSH_listdir(ssh, vpu_log_dir):
+                scp.get(vpu_log_dir+"/"+item,
+                        vpu_specific_local_cache_path, recursive=True)
+        else:
+            scp.get(vpu_log_dir, vpu_specific_local_cache_path, recursive=True)
+    else:
+        logger.info(
+            f"No logs collected from {vpu_log_dir}, directory does not yet exist"
+        )
+
+
+def expand_pc_path(pc_path: str) -> str:
+    pc_path = str(pc_path).replace("~", str(Path().home()))
+    pc_path = pc_path.replace(
+        "./", str(Path(os.getcwd()))+"/").replace("\\", "/")
+    return pc_path
+
+
+def expand_vpu_path(vpu_path: str) -> str:
+    vpu_path = str(vpu_path).replace("~", "/home/oem")
+    return vpu_path
+
+
+def structure_docker_table_output(docker_table: List[str]) -> List[dict]:
+    """
+    This function structures the output of a docker table into a list of dictionaries    
+    """
+    params = [param.strip() for param in docker_table[0].split("  ")if param]
+    param_starting_positions = []
+    param_end_positions = []
+    cursor = 0
+    for param in params:
+        for i in range(cursor, len(docker_table[0])):
+            if docker_table[0][i:].startswith(param):
+                param_starting_positions.append(i)
+                cursor = i + len(param)
+                break
+    param_end_positions = param_starting_positions[1:] + [len(docker_table[0])]
+    entry_dicts = []
+    for running_container in docker_table[1:]:
+        container_dict = {}
+        for param, param_starting_position, param_end_position in zip(params, param_starting_positions, param_end_positions):
+            container_dict[param] = running_container[param_starting_position:param_end_position].strip(
+            )
+        entry_dicts.append(container_dict)
+    return entry_dicts
+
+
+def run_read_print_ssh_loop(ip: str, cmd: str, stop_loop, private_key_path: str, password: str = "oem",  timeout: int = 0, output_buffer: str = "") -> str:
+    """
+    This function runs a command on the remote device and prints the output to the console
+
+    Parameters
+    ----------
+    ip : str
+        IP address of the device
+    cmd : str
+        command to run on the device
+    stop_loop : bool
+        thread safe callable flag to stop the loop
+    private_key_path : str
+        path to private key
+    password : str
+        password for the device
+    timeout : int
+        time to run the loop for
+    output_buffer : str
+        buffer to store output
+
+    Returns
+    -------
+    str
+        output of the command
+    """
+    ssh, scp = SSH_collect_VPU_handles(
+        IP=ip, password=password, private_key_path=private_key_path)
+    ssh: SSHClient = ssh
+    transport = ssh.get_transport()
+    channel = transport.open_session()
+    channel.exec_command(cmd)
+
+    start = time.perf_counter()
+    try:
+        while not channel.exit_status_ready() and (not timeout or time.perf_counter() < start+timeout) and not stop_loop():
+            rl, wl, xl = select.select([channel], [], [], 0.0)
+            if len(rl) > 0:
+                # Must be stdout
+                output = channel.recv(1024).decode()
+                if output:
+                    print(output, end="")
+                    output_buffer += [output]
+    except:
+        pass
+    return output_buffer
+
+
+class ManagerConfig(BaseModel):
+    IP: str = os.environ.get("IFM3D_IP", DEFAULT_IP)
+    possible_initial_ip_addresses_to_try: List[str] = []
+    log_level: str = "INFO"
+    log_dir: str = "~/ovp_logs"
+    ssh_key_dir: str = "~/.ssh/"
+    oem_user_password: str = "oem"
+    ssh_key_file_name: str = "id_rsa_ovp8xx"
+
+
+class Manager:
+    def __init__(
+        self,
+        config: ManagerConfig = ManagerConfig(),
+    ):
+        """
+        This class handles the deployment of docker containers to the OVP8XX. It is a thin wrapper around the ifm3dpy library, the paramiko and scp libraries for SSH and SCP respectively, and the docker command line interface on the VPU.
+
+        The objective here is to minimize magic and maximize transparency. The user should be able to see exactly what is happening on the VPU and be able to interact with the VPU directly if desired. Manager.o3r is the native ifm3dpy handle to the VPU. Manager.ssh and Manager.scp are the native paramiko and scp handles to the VPU respectively.
+
+        Each cli command run on the VPU (outside of simple filesystem operations from ovp_docker_utils.ssh_file_utils) is logged so that issues can be debugged if they arise.
+        """
+
+        self.config: ManagerConfig = config
+
+        self._log_file_path = configure_manager_logging(
+            logger,
+            self.config.log_level,
+            self.config.log_dir
+        )
+
+        self._connected = False
+        self._o3r = None
+        self._ssh = None
+        self._scp = None
+        self._fw_version = None
+        self.private_key_path = None
+
+        self.connect()
+
+    @property
+    def log_file_path(self):
+        return self._log_file_path
+
+    @property
+    def connected(self):
+        return self._connected
+
+    @property
+    def o3r(self):
+        return self._o3r
+
+    @property
+    def ssh(self):
+        return self._ssh
+
+    @property
+    def scp(self):
+        return self._scp
+
+    @property
+    def vpu_config(self):
+        if not self._o3r:
+            raise Exception("Not connected to device")
+        return self._o3r.get()
+
+    @property
+    def fw_version(self):
+        if not self._o3r:
+            raise Exception("Not connected to device")
+        return self._fw_version
+
+    @property
+    def vpu_sn(self):
+        return self.vpu_config["device"]["info"]["serialNumber"]
+
+    @property
+    def vpu_name(self):
+        return self.vpu_config["device"]["info"]["name"]
+
+    def connect(self,) -> bool:
+
+        if not USING_IFM3DPY:
+            logger.info("ifm3dpy unavailable")
+        if USING_IFM3DPY and self.config.possible_initial_ip_addresses_to_try:
+            possible_initial_ip_addresses = list(
+                set([self.config.IP] + self.config.possible_initial_ip_addresses_to_try))
+            if len(possible_initial_ip_addresses) > 1:
+                logger.info(
+                    f"Trying to connect to VPU at any of the following addresses: {possible_initial_ip_addresses}")
+
+                for temp_IP in possible_initial_ip_addresses:
+                    try:
+                        VPU_config = ifm3dpy.O3R(temp_IP).get()
+                        logger.info(f"Connected to {temp_IP}")
+                        self._connected = True
+                        break
+                    except Exception as e:
+                        if "XMLRPC Timeout" in str(e):
+                            continue
+                        raise e
+                if not self._connected:
+                    logger.info(
+                        f"VPU could not be found at any of the following addresses: {possible_initial_ip_addresses}")
+                elif temp_IP != self.config.IP:
+                    logger.info(
+                        f"Updating IP address from {temp_IP} to {self.config.IP}")
+                    gateway = ".".join(
+                        self.config.IP.split(".")[:-1] + ["255"])
+                    mask = 24
+                    ifm3dpy.O3R(temp_IP).set({"device": {"network": {"interfaces": {"eth0": {
+                        "ipv4": {
+                            "address": self.config.IP,
+                            "gateway": gateway,
+                            "mask": mask
+                        }}}}}})  # in c
+                    ifm3dpy.O3R(temp_IP).reboot()
+                    wait_period = 80
+                    logger.info(f"Waiting 80s for VPU to reboot.")
+                    heartbeat_rate = 2
+                    for x in range(int(wait_period/heartbeat_rate)):
+                        print(".", end="")
+                        time.sleep(heartbeat_rate)
+        if USING_IFM3DPY and self._connected:
+            self._o3r = ifm3dpy.O3R(self.config.IP)
+            self._fw_version = ".".join(self.vpu_config["device"]["swVersion"]["firmware"].split(
+                "-")[0].split(".")[:3])  # get the first 3 parts of the version number
+
+            logger.info(f"Device firmware version: {self._fw_version}")
+
+            # Check for firmware compatibility
+            if not any(
+                    [semver.compare(self._fw_version, range[0])*semver.compare(range[1], self._fw_version) == 1 for range in TESTED_COMPATIBLE_FIRMWARE_RANGES]):
+                raise Exception(
+                    f"Device firmware version {self._fw_version} is not compatible with version of the deployment manager (tested with the following ranges: {TESTED_COMPATIBLE_FIRMWARE_RANGES})")
+
+            self.private_key_path = assign_key(
+                ip=self.config.IP, target_dir=self.config.ssh_key_dir, key_title=self.config.ssh_key_file_name)
+
+            logger.info(f"private_key_path = {self.private_key_path}")
+
+            try:
+                self._ssh, self._scp = SSH_collect_VPU_handles(
+                    IP=self.config.IP, password=self.config.oem_user_password, private_key_path=self.private_key_path)
+            except Exception as e:
+                logger.info(
+                    f"Device is present but failed to connect via ssh: {e}")
+                self._connected = False
+                raise e
+
+            logger.info(
+                f"Device accessible using ifm3dpy=={ifm3dpy.__version__} and ssh connected")
+        return self._connected
+
+    def mkdir(self, dir_path: str) -> None:
+        if not SSH_path_exists(self._ssh, dir_path):
+            cmd = f"mkdir {dir_path}"
+            logger.info(cmd)
+            _stdin, _stdout, _stderr = self._ssh.exec_command(cmd)
+            logger.info(
+                f">>> {_stderr.read().decode().strip()} {_stdout.read().decode().strip()}")
+
+    def append_deployment_timestamp(self, deployment_timestamp_path: str = "~/share/Deployments") -> None:
+        cmd = f'echo "{Path(self._log_file_path).name[:-4]}" >> {deployment_timestamp_path}'
+        logger.info(cmd)
+        _stdin, _stdout, _stderr = self._ssh.exec_command(cmd)
+        logger.info(
+            f">>> {_stderr.read().decode().strip()} {_stdout.read().decode().strip()}")
+
+    def append_docker_registry(self, docker_registry_host: str = "", docker_registry_port: int = 5000) -> None:
+        insecure_registries = self.vpu_config["device"]["docker"]["insecure-registries"]
+        if docker_registry_host and docker_registry_port:
+            if f"{docker_registry_host}:{docker_registry_port}" not in insecure_registries:
+                logger.info(
+                    f"Adding {docker_registry_host}:{docker_registry_port} to insecure registries in VPU config")
+                if len(insecure_registries) > 2:
+                    logger.warning(
+                        f"VPU already has {len(insecure_registries)} insecure registries, adding more is not permitted, the last one will be replaced")
+                    insecure_registries.pop()
+                insecure_registries.append(
+                    f"{docker_registry_host}:{docker_registry_port}")
+                self._o3r.set(
+                    {"device": {"docker": {"insecure-registries": insecure_registries}}})
+                logger.info(
+                    f"Success! {docker_registry_host}:{docker_registry_port} added to insecure registries in VPU config, restarting the vpu to apply changes")
+                self._o3r.reboot()
+                timeout = 100
+                logger.info(
+                    f"VPU rebooting, waiting {timeout}s for it to come back online")
+                heartbeat_rate = 2
+                for x in range(timeout//heartbeat_rate):
+                    print(".", end="")
+                    time.sleep(heartbeat_rate)
+                self.connect()
+
+            else:
+                logger.info(
+                    f"{docker_registry_host}:{docker_registry_port} already in insecure registries in VPU config")
+
+    def transfer_to_vpu(self, src: str, dst: str) -> None:
+        src = expand_pc_path(src)
+        dst = expand_vpu_path(dst)
+        if Path(src).exists():
+            logger.info(
+                f"transferring {src} to {dst}")
+            SCP_transfer_item(
+                self._ssh, self._scp, src, dst, True)
+        else:
+            logger.info(f"file not found '{src}'")
+
+    def transfer_from_vpu(self, src: str, dst: str) -> None:
+        src = expand_vpu_path(src)
+        dst = expand_pc_path(dst)
+        if SSH_path_exists(self._ssh, src):
+            logger.info(
+                f"Transferring {src} to {dst}")
+            SCP_transfer_item(
+                self._ssh, self._scp, src, dst, False)
+        else:
+            logger.info(f"file not found '{src}'")
+
+    def get_running_docker_containers(self) -> List[str]:
+        cmd = "docker ps -a"
+        _stdin, _stdout, _stderr = self._ssh.exec_command(cmd)
+        running_containers_list = _stdout.read().decode().strip().split("\n")
+        return structure_docker_table_output(running_containers_list)
+
+    def remove_running_docker_containers(self, running_containers_to_remove: list = []) -> None:
+        for running_container in running_containers_to_remove:
+            cmd = f"docker rm -f {running_container['CONTAINER ID']}"
+            logger.info(cmd)
+            _stdin, _stdout, _stderr = self._ssh.exec_command(cmd)
+            logger.info(f">>>{_stdout.read().decode().strip()}")
+
+    def get_cached_docker_images(self) -> List[str]:
+        cmd = "docker image ls"
+        _stdin, _stdout, _stderr = self._ssh.exec_command(cmd)
+        cached_images_list = _stdout.read().decode().strip().split("\n")
+        return structure_docker_table_output(cached_images_list)
+
+    def remove_cached_docker_images(self, cached_images_to_remove: list = []) -> None:
+        for cached_container in cached_images_to_remove:
+            cmd = f"docker image rm {cached_container['IMAGE ID']}"
+            logger.info(cmd)
+            _stdin, _stdout, _stderr = self._ssh.exec_command(cmd)
+            logger.info(f">>>{_stdout.read().decode().strip()}")
+
+    def get_registered_docker_volumes(self) -> List[str]:
+        cmd = "docker volume ls"
+        _stdin, _stdout, _stderr = self._ssh.exec_command(cmd)
+        cached_images_list = _stdout.read().decode().strip().split("\n")
+        return structure_docker_table_output(cached_images_list)
+
+    def remove_registered_docker_volumes(self, registered_volumes_to_remove: list = []) -> None:
+        for volume in registered_volumes_to_remove:
+            cmd = f"docker volume rm {volume['VOLUME NAME']}"
+            logger.info(cmd)
+            _stdin, _stdout, _stderr = self._ssh.exec_command(cmd)
+            logger.info(f">>>{_stdout.read().decode().strip()}")
+
+    def get_logs(self, vpu_log_dir: str = "/home/oem/share/logs", local_log_cache: str = "~/ovp_logs/From_VPUs") -> None:
+        get_logs(
+            vpu_log_dir=vpu_log_dir,
+            local_log_cache=local_log_cache,
+            vpu_sn=self.vpu_sn,
+            scp=self._scp,
+            ssh=self._ssh,
+        )
+
+    def set_vpu_name(self, set_vpu_name: str) -> None:
+        logger.info(f"Setting device name to {set_vpu_name}")
+        self._o3r.set({"device": {"info": {"name": set_vpu_name}}})
+
+    def mount_usb(self) -> list:
+        cmd = f"mount"
+        logger.info(cmd)
+        _stdin, _stdout, _stderr = self.ssh.exec_command(cmd)
+        output = _stdout.read().decode().strip()
+        logger.info(">>>" + output.split("\n")
+                    [0] + " ..." + _stderr.read().decode().strip())
+        mounted_disks_dirs = [disk_desc.split(
+            " ")[2] for disk_desc in output.split("\n") if ("autofs" in disk_desc)]
+        return mounted_disks_dirs
+
+    def disk_is_available(self, known_disk_name: str) -> bool:
+        self.mount_usb()
+        disk_dir = "/run/media/system/" + known_disk_name
+        logger.info(f"Checking if disk is available at {disk_dir}")
+        disk_is_available = SSH_path_exists(self._ssh, disk_dir)
+        return disk_is_available
+
+    def setup_docker_volume(self, path_for_volume_to_mount: str, volume_name: str) -> None:
+        # setup volume as specified
+        cmd = f'docker volume create --driver local -o o=bind -o type=none -o device="{path_for_volume_to_mount}" {volume_name}'
+        _stdin, _stdout, _stderr = self._ssh.exec_command(cmd)
+        logger.info(cmd)
+        if _stdout.read().decode().strip() == volume_name:
+            logger.info("Success!")
+        else:
+            logger.info("Issue encountered while setting up shared volume")
+            raise Exception(_stderr.read().decode().strip())
+
+    def import_docker_image(self, image_to_import: str) -> None:
+        # load image
+        docker_image_fname = Path(image_to_import).name
+        logger.info("importing image into vpu docker storage")
+        cmd = f"cat {image_to_import}| docker import - {docker_image_fname[:-4]}"
+        logger.info(cmd)
+        _stdin, _stdout, _stderr = self._ssh.exec_command(cmd)
+        logger.info(">>>"+_stdout.read().decode().strip() +
+                    _stderr.read().decode().strip())
+
+    def load_docker_image(self, image_to_load: str, update_tag_on_VPU_to: str = "") -> None:
+        # load image
+        docker_image_fname = Path(image_to_load).name
+        logger.info("loading image into vpu docker storage")
+        cmd = f"docker load -i {image_to_load}"
+        logger.info(cmd)
+        _stdin, _stdout, _stderr = self._ssh.exec_command(cmd)
+        stdout = _stdout.read().decode().strip()
+        logger.info(">>>"+stdout +
+                    _stderr.read().decode().strip())
+        if "Loaded image" not in stdout:
+            logger.warning("Issue encountered while loading image")
+        elif update_tag_on_VPU_to:
+            tag_of_loaded_image = stdout.strip().split(" ")[-1]
+            cmd = f"docker tag {tag_of_loaded_image} {update_tag_on_VPU_to}"
+            logger.info(cmd)
+            _stdin, _stdout, _stderr = self._ssh.exec_command(cmd)
+            logger.info(">>>"+_stdout.read().decode().strip() +
+                        _stderr.read().decode().strip())
+
+    def pull_docker_image_from_registry(self, docker_registry_host: str, docker_registry_port: int, docker_repository_name: str, docker_image_tag: str = "latest", update_tag_on_VPU_to: str = "") -> None:
+        # pull image
+        logger.info("pulling image from local registry (this may take a while)")
+        cmd = f"docker pull {docker_registry_host}:{docker_registry_port}/{docker_repository_name}:{docker_image_tag}"
+        logger.info(cmd)
+        _stdin, _stdout, _stderr = self._ssh.exec_command(cmd)
+        logger.info(">>>"+_stdout.read().decode().strip() +
+                    _stderr.read().decode().strip())
+
+        if update_tag_on_VPU_to:
+            cmd = f"docker tag {docker_registry_host}:{docker_registry_port}/{docker_repository_name}:{docker_image_tag} {update_tag_on_VPU_to}"
+            logger.info(cmd)
+            _stdin, _stdout, _stderr = self._ssh.exec_command(cmd)
+            logger.info(">>>"+_stdout.read().decode().strip() +
+                        _stderr.read().decode().strip())
+
+    def rm_item(self, item_to_rm: str) -> None:
+        if SSH_path_exists(self._ssh, item_to_rm):
+            logger.info(f"Removing {item_to_rm}")
+            if SSH_isdir(self._ssh, item_to_rm):
+                cmd = f"rm -r {item_to_rm}"
+                logger.info(cmd)
+                _stdin, _stdout, _stderr = self._ssh.exec_command(cmd)
+                logger.info(_stdout.read().decode().strip() +
+                            _stderr.read().decode().strip())
+            else:
+                cmd = f"rm {item_to_rm}"
+                logger.info(cmd)
+                _stdin, _stdout, _stderr = self._ssh.exec_command(cmd)
+                logger.info(">>>"+_stdout.read().decode().strip() +
+                            _stderr.read().decode().strip())
+
+    def enable_autostart(self, docker_compose_fname: str, service_name: str) -> None:
+        # check if symlink already exists
+        docker_compose_dir = f"/usr/share/oem/docker/compose/{service_name}"
+
+        docker_compose_vpu_path = docker_compose_dir+"/docker-compose.yml"
+
+        if not SSH_path_exists(self._ssh, docker_compose_vpu_path):
+            logger.info(
+                "no docker-compose symlink for auto-start found, setting it up now")
+            SSH_makedirs(self._ssh, docker_compose_dir)
+            cmd = f"ln -s {docker_compose_fname} {docker_compose_vpu_path}"
+            logger.info(cmd)
+            _stdin, _stdout, _stderr = self._ssh.exec_command(cmd)
+            logger.info(
+                f">>> {_stderr.read().decode().strip()} {_stdout.read().decode().strip()}")
+
+        logger.info("Enabling autostart...")
+        cmd = f'systemctl --user enable oem-dc@{service_name}'
+        logger.info(cmd)
+        _stdin, _stdout, _stderr = self._ssh.exec_command(cmd)
+        output = _stdout.read().decode().strip()
+
+    def autostart_enabled(self, service_name: str) -> bool:
+        cmd = f"systemctl --user status oem-dc@{service_name}"
+        logger.info(cmd)
+        _stdin, _stdout, _stderr = self._ssh.exec_command(cmd)
+        # logger.info(
+        #     f">>> {_stderr.read().decode().strip()} {_stdout.read().decode().strip()}")
+        output = _stdout.read().decode().strip()
+        return "enabled;" in output
+
+    def get_all_autostart_instances(self) -> List[str]:
+        cmd = f"ls /home/oem/.config/systemd/user/default.target.wants/"
+        logger.info(cmd)
+        _stdin, _stdout, _stderr = self._ssh.exec_command(cmd)
+        output = _stdout.read().decode().strip()
+        # Regular expression pattern
+        pattern = r'oem-dc@(.*?).service'
+        # Find matches
+        matches = re.findall(pattern, output)
+        logger.info(">>>" + output)
+        return matches
+
+    def disable_autostart(self, service_name: str) -> None:
+        logger.info("disabling autostart...")
+        cmd = f'systemctl --user disable oem-dc@{service_name}'
+        logger.info(cmd)
+        _stdin, _stdout, _stderr = self._ssh.exec_command(cmd)
+        logger.info(
+            f">>> {_stderr.read().decode().strip()} {_stdout.read().decode().strip()}")
+
+    def stop_container(self, service_name: str):
+        cmd = f"docker rm -f {service_name}"
+        logger.info(f"Stopping container with: {cmd}")
+        _stdin, _stdout, _stderr = self._ssh.exec_command(cmd)
+        logger.info(">>>" + _stdout.read().decode().strip() +
+                    _stderr.read().decode().strip())
+        
+    def pull_journalctl_logs(self, dst_dir: Union[Path, str], dst_name = "") -> List[str]:
+        if not dst_name:
+            ts = datetime.now().strftime("%Y%m%d_%H%M%S")
+            dst_name = f"journalctl_{ts}.gzip"
+        fname = "journalctl.gzip"
+        logger.info(f"journalctl | gzip > {fname}")
+        _stdin, _stdout, _stderr = self._ssh.exec_command(
+            f"journalctl | gzip > {fname}")
+        logger.info(
+            f">>> {_stderr.read().decode().strip()} {_stdout.read().decode().strip()}")
+        if type(dst_dir) == str:
+            dst_dir = Path(dst_dir).expanduser().absolute()
+        logger.info(dst_dir/dst_name)
+        self.transfer_from_vpu("/home/oem/"+fname, dst_dir/dst_name)
+
+    def initialize_container(self, service: DockerComposeServiceInstance, pipe_duration: float = 0, stop_upon_exit: bool = False, trigger_to_close_container: str = "") -> None:
+        initialized = False
+
+        non_standard_docker_logger_used = service.log_driver is not None
+
+        if non_standard_docker_logger_used or not pipe_duration:
+            # detach from the container immediately
+            cmd = f"docker-compose -f {service.docker_compose_dst_on_vpu} up --d --remove-orphan {service.service_name} "
+            _stdin, _stdout, _stderr = self._ssh.exec_command(cmd)
+            logger.info(cmd)
+            output_lines_from_container = _stdout.read().decode().strip().split("\n")
+            logger.info(
+                f">>> {_stderr.read().decode().strip()} {' '.join(output_lines_from_container)}")
+            logger.info(
+                f"{service.service_name} initialized from {service.docker_compose_dst_on_vpu}")
+
+            initialized = True
+
+        else:
+            output_lines_from_container = []
+
+        if pipe_duration:
+            if initialized:
+                cmd = f"docker attach {service.container_name}"
+                logger.info(
+                    f"Now Attempting to show output from {service.container_name}: {cmd}")
+            else:
+                cmd = f"docker-compose -f {service.docker_compose_dst_on_vpu} up {service.service_name}"
+                logger.info(
+                    f"Initializing service and showing output of container as it appears to be using the standard logger... {cmd}")
+
+            output_lines_from_container += self.attach_to_container(
+                cmd=cmd,
+                container_name=service.container_name,
+                pipe_duration=pipe_duration,
+                stop_upon_exit=stop_upon_exit,
+                trigger_to_close_container=trigger_to_close_container,
+            )
+
+        # check if any non-ssd safe logging drivers are allowed in the docker-compose file
+        ssd_safe_docker_logging_drivers = ["none", "local"]
+        if service.log_driver not in ssd_safe_docker_logging_drivers:
+            logger.critical(
+                f"Write-intensive Docker logging driver used for service '{service.service_name}'. Try using: \nlogging:\n   driver: \"none\" ")
+
+        return output_lines_from_container
+
+    def attach_to_container(self, cmd: str = "", container_name: str = "", pipe_duration: float = 20, stop_upon_exit: bool = False, trigger_to_close_container: str = "") -> List[str]:
+
+        if not cmd:
+            cmd = f"docker attach {container_name}"
+        output_lines_from_container = []
+
+        stop_loop = False
+        print_loop_thread = threading.Thread(
+            target=run_read_print_ssh_loop,
+            args=(self.config.IP, cmd, lambda: stop_loop, self.private_key_path,
+                  self.config.oem_user_password, pipe_duration, output_lines_from_container),
+            daemon=True
+        )
+        n_output_lines = len(output_lines_from_container)
+        print_loop_thread.start()
+        start_t = time.perf_counter()
+        while not stop_loop:
+            try:
+                time.sleep(0.2)
+                if pipe_duration > 0 and time.perf_counter() > start_t+pipe_duration:
+                    logger.info(
+                        f"run_duration of {pipe_duration} seconds has been reached, detaching from container...")
+                    stop_loop = True
+                else:
+                    # check if new output lines have been added
+                    if len(output_lines_from_container) > n_output_lines:
+                        latest_lines = output_lines_from_container[n_output_lines:]
+                        n_output_lines = len(output_lines_from_container)
+                        if any([" exited with code 0\n\x1b[0m" in line for line in latest_lines]):
+                            logger.info("Container exited with code 0")
+                            stop_loop = True
+                        if trigger_to_close_container and any([trigger_to_close_container in line for line in latest_lines]):
+                            logger.info(
+                                f"Container exited with trigger: {trigger_to_close_container}")
+                            stop_loop = True
+            except KeyboardInterrupt:
+                logger.info(
+                    "KeyboardInterrupt detected, Detaching from container...")
+                stop_loop = True
+
+        if stop_upon_exit:
+            logger.info("Stopping container...")
+            self.stop_container(service_name=container_name)
+            time.sleep(0.5)
+        time.sleep(0.5)
+        if not print_loop_thread.is_alive():
+            print_loop_thread.join()
+        else:
+            logger.info(
+                "Failed to stop container monitor thread... it will exit with the program exit")
+
+        output_lines_from_container = output_lines_from_container.copy()
+        del (print_loop_thread)
+        time.sleep(2)
+
+        logger.info("Container monitor thread stopped")
+
+        return output_lines_from_container
```

### Comparing `ovp_docker_utils-1.0.3/ovp_docker_utils/ssh_file_utils.py` & `ovp_docker_utils-1.0.4/ovp_docker_utils/ssh_file_utils.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,223 +1,223 @@
-#############################################
-# Copyright 2021-present ifm electronic, gmbh
-# SPDX-License-Identifier: Apache-2.0
-#############################################
-
-import logging
-import sys
-from pathlib import Path
-from typing import Tuple, List
-
-from paramiko import AutoAddPolicy
-from paramiko.client import SSHClient
-from scp import SCPClient
-
-
-from .defaults import DEFAULT_IP
-
-USING_IPYTHON = "ipykernel" in sys.modules
-if USING_IPYTHON:
-    logger = logging.getLogger("notebook")
-else:
-    logger = logging.getLogger("deploy")
-
-
-def SSH_collect_VPU_handles(oem_username: str = "oem", password: str = "oem", private_key_path: str = None, IP: str = DEFAULT_IP, port: int = 22, remove_known_host: bool = True) -> Tuple[SSHClient, SCPClient]:
-    """
-    This function collects the ssh and scp handles for the vpu
-
-    Parameters
-    ----------
-    oem_username : str, optional
-        By default "oem"
-    password : str, optional
-        By default "oem"
-    IP : str, optional
-        By default "192.168.0.69"
-    port : int, optional
-        By default 22
-    remove_known_hosts : bool, optionally remove the entry for this IP from the known_hosts file after connecting (useful when simultaneously sshing into system via cli),
-        By default True
-
-    Returns
-    -------
-    tuple[SSHClient, SCPClient]
-        ssh and scp handles for the vpu
-
-    Raises
-    ------
-    Exception
-        If the vpu cannot be connected to
-    """
-
-    logging.getLogger("paramiko").setLevel(logging.INFO)
-    logging.getLogger("scp").setLevel(logging.INFO)
-
-    ssh: SSHClient = SSHClient()
-    ssh.set_missing_host_key_policy(AutoAddPolicy())
-
-    try:
-        ssh.connect(hostname=IP, username=oem_username,
-                    password=password, key_filename=private_key_path, timeout=1, port=port)
-    except Exception as FailureToConnectError:
-        if "timed out" in str(FailureToConnectError):
-            logger.info(
-                f"Attempt to connect to {oem_username}@{IP}:{port} timed out.")
-        raise FailureToConnectError
-
-    scp = SCPClient(ssh.get_transport())
-
-    known_hosts_path = Path("~/.ssh/known_hosts").expanduser()
-    if remove_known_host and known_hosts_path.exists():
-        with open(known_hosts_path, "r") as f:
-            lines = f.readlines()
-        with open(known_hosts_path, "w") as f:
-            f.write(
-                "\n".join([line for line in lines if not (line.split(" ")[0] == IP)]))
-
-    return ssh, scp
-
-
-def SSH_listdir(ssh: SSHClient, path: str = "~") -> List[str]:
-    """
-    This function lists the contents of a directory via SSH
-
-    Parameters
-    ----------
-    ssh : SSHClient
-        ssh library native handle
-    path : str, optional
-        path to check, by default "~"
-
-    Returns
-    -------
-    bool
-        list of contents of the directory
-    """
-    cmd = f"ls {path}"
-    _stdin, _stdout, _stderr = ssh.exec_command(cmd)
-    return _stdout.read().decode().strip().split("\n")
-
-
-def SSH_path_exists(ssh: SSHClient, path: str = "~") -> bool:
-    """
-    This function checks whether a path exists
-
-    Parameters
-    ----------
-    ssh : SSHClient
-        ssh library native handle
-    path : str, optional
-        path to check, by default "~"
-
-    Returns
-    -------
-    bool
-        Whether the path exists
-    """
-    cmd = f"cd {path}"
-    _stdin, _stdout, _stderr = ssh.exec_command(cmd)
-    if _stderr.read():
-        tokenized_path = path.split("/")
-        if len(tokenized_path) > 1:
-            contents_of_parent = SSH_listdir(
-                ssh, "/".join(tokenized_path[:-1]))
-            path_exists = tokenized_path[-1] in contents_of_parent
-        else:
-            path_exists = False
-    else:
-        path_exists = True
-    return path_exists
-
-
-def SSH_isdir(ssh: SSHClient, path: str = "~") -> bool:
-    """
-    This function checks whether a path exists and is a directory
-
-    Parameters
-    ----------
-    ssh : SSHClient
-        ssh library native handle
-    path : str, optional
-        path to check, by default "~"
-
-    Returns
-    -------
-    bool
-        Whether the path exists and is a directory
-    """
-    cmd = f"cd {path}"
-    _stdin, _stdout, _stderr = ssh.exec_command(cmd)
-    return not bool(_stderr.read().decode())
-
-
-def SSH_makedirs(ssh: SSHClient, path: str = "") -> None:
-    """
-    This function makes directories via SSH
-
-    Parameters
-    ----------
-    ssh : SSHClient
-        ssh library native handle
-    path : str, optional
-        path to check, by default ""
-
-    Raises
-    ------
-    Exception
-        If the path or one of its parents exists but is not a directory
-    """
-    sub_path_to_check = []
-    if path[-1] != "/":
-        path += "/"
-    for dir in path.split("/"):
-        if sub_path_to_check:
-            sub_path = "/".join(sub_path_to_check)
-            if not SSH_isdir(ssh, sub_path):
-                if SSH_path_exists(ssh, sub_path):
-                    logger.exception(
-                        f"Error making directories, {path}, via SSH. {sub_path} is not a directory")
-                    raise Exception(
-                        f"Error making directories, {path}, via SSH. {sub_path} is not a directory")
-                else:
-                    _stdin, _stdout, _stderr = ssh.exec_command(
-                        f"mkdir {sub_path}")
-        sub_path_to_check += [dir]
-
-
-def SCP_transfer_item(ssh: SSHClient, scp: SCPClient, src: str, dst: str, src_is_local: bool = True) -> None:
-    """
-    This function transfers a file or directory between the local machine and the vpu
-
-    Parameters
-    ----------
-    ssh : SSHClient
-        ssh library native handle
-    scp : SCPClient
-        scp library native handle
-    src : str
-        path to source file or directory
-    dst : str
-        path to destination file or directory
-    src_is_local : bool, optional
-        Whether the source is local or remote, by default True
-    """
-    if src_is_local:
-        if Path(src).exists():
-            if Path(src).is_dir():
-                dst = "/".join(dst.split("/")[:-1])
-                if not SSH_path_exists(ssh, dst):
-                    SSH_makedirs(ssh, dst)
-                scp.put(
-                    files=[src],
-                    remote_path=dst, recursive=True)
-            else:
-                scp.put(
-                    files=[src],
-                    remote_path=dst)
-    else:
-        if SSH_path_exists(ssh, src):
-            if SSH_isdir(ssh, src):
-                scp.get(src, dst, recursive=True)
-            else:
-                scp.get(src, dst)
+#############################################
+# Copyright 2021-present ifm electronic, gmbh
+# SPDX-License-Identifier: Apache-2.0
+#############################################
+
+import logging
+import sys
+from pathlib import Path
+from typing import Tuple, List
+
+from paramiko import AutoAddPolicy
+from paramiko.client import SSHClient
+from scp import SCPClient
+
+
+from .defaults import DEFAULT_IP
+
+USING_IPYTHON = "ipykernel" in sys.modules
+if USING_IPYTHON:
+    logger = logging.getLogger("notebook")
+else:
+    logger = logging.getLogger("deploy")
+
+
+def SSH_collect_VPU_handles(oem_username: str = "oem", password: str = "oem", private_key_path: str = None, IP: str = DEFAULT_IP, port: int = 22, remove_known_host: bool = True) -> Tuple[SSHClient, SCPClient]:
+    """
+    This function collects the ssh and scp handles for the vpu
+
+    Parameters
+    ----------
+    oem_username : str, optional
+        By default "oem"
+    password : str, optional
+        By default "oem"
+    IP : str, optional
+        By default "192.168.0.69"
+    port : int, optional
+        By default 22
+    remove_known_hosts : bool, optionally remove the entry for this IP from the known_hosts file after connecting (useful when simultaneously sshing into system via cli),
+        By default True
+
+    Returns
+    -------
+    tuple[SSHClient, SCPClient]
+        ssh and scp handles for the vpu
+
+    Raises
+    ------
+    Exception
+        If the vpu cannot be connected to
+    """
+
+    logging.getLogger("paramiko").setLevel(logging.INFO)
+    logging.getLogger("scp").setLevel(logging.INFO)
+
+    ssh: SSHClient = SSHClient()
+    ssh.set_missing_host_key_policy(AutoAddPolicy())
+
+    try:
+        ssh.connect(hostname=IP, username=oem_username,
+                    password=password, key_filename=private_key_path, timeout=1, port=port)
+    except Exception as FailureToConnectError:
+        if "timed out" in str(FailureToConnectError):
+            logger.info(
+                f"Attempt to connect to {oem_username}@{IP}:{port} timed out.")
+        raise FailureToConnectError
+
+    scp = SCPClient(ssh.get_transport())
+
+    known_hosts_path = Path("~/.ssh/known_hosts").expanduser()
+    if remove_known_host and known_hosts_path.exists():
+        with open(known_hosts_path, "r") as f:
+            lines = f.readlines()
+        with open(known_hosts_path, "w") as f:
+            f.write(
+                "\n".join([line for line in lines if not (line.split(" ")[0] == IP)]))
+
+    return ssh, scp
+
+
+def SSH_listdir(ssh: SSHClient, path: str = "~") -> List[str]:
+    """
+    This function lists the contents of a directory via SSH
+
+    Parameters
+    ----------
+    ssh : SSHClient
+        ssh library native handle
+    path : str, optional
+        path to check, by default "~"
+
+    Returns
+    -------
+    bool
+        list of contents of the directory
+    """
+    cmd = f"ls {path}"
+    _stdin, _stdout, _stderr = ssh.exec_command(cmd)
+    return _stdout.read().decode().strip().split("\n")
+
+
+def SSH_path_exists(ssh: SSHClient, path: str = "~") -> bool:
+    """
+    This function checks whether a path exists
+
+    Parameters
+    ----------
+    ssh : SSHClient
+        ssh library native handle
+    path : str, optional
+        path to check, by default "~"
+
+    Returns
+    -------
+    bool
+        Whether the path exists
+    """
+    cmd = f"cd {path}"
+    _stdin, _stdout, _stderr = ssh.exec_command(cmd)
+    if _stderr.read():
+        tokenized_path = path.split("/")
+        if len(tokenized_path) > 1:
+            contents_of_parent = SSH_listdir(
+                ssh, "/".join(tokenized_path[:-1]))
+            path_exists = tokenized_path[-1] in contents_of_parent
+        else:
+            path_exists = False
+    else:
+        path_exists = True
+    return path_exists
+
+
+def SSH_isdir(ssh: SSHClient, path: str = "~") -> bool:
+    """
+    This function checks whether a path exists and is a directory
+
+    Parameters
+    ----------
+    ssh : SSHClient
+        ssh library native handle
+    path : str, optional
+        path to check, by default "~"
+
+    Returns
+    -------
+    bool
+        Whether the path exists and is a directory
+    """
+    cmd = f"cd {path}"
+    _stdin, _stdout, _stderr = ssh.exec_command(cmd)
+    return not bool(_stderr.read().decode())
+
+
+def SSH_makedirs(ssh: SSHClient, path: str = "") -> None:
+    """
+    This function makes directories via SSH
+
+    Parameters
+    ----------
+    ssh : SSHClient
+        ssh library native handle
+    path : str, optional
+        path to check, by default ""
+
+    Raises
+    ------
+    Exception
+        If the path or one of its parents exists but is not a directory
+    """
+    sub_path_to_check = []
+    if path[-1] != "/":
+        path += "/"
+    for dir in path.split("/"):
+        if sub_path_to_check:
+            sub_path = "/".join(sub_path_to_check)
+            if not SSH_isdir(ssh, sub_path):
+                if SSH_path_exists(ssh, sub_path):
+                    logger.exception(
+                        f"Error making directories, {path}, via SSH. {sub_path} is not a directory")
+                    raise Exception(
+                        f"Error making directories, {path}, via SSH. {sub_path} is not a directory")
+                else:
+                    _stdin, _stdout, _stderr = ssh.exec_command(
+                        f"mkdir {sub_path}")
+        sub_path_to_check += [dir]
+
+
+def SCP_transfer_item(ssh: SSHClient, scp: SCPClient, src: str, dst: str, src_is_local: bool = True) -> None:
+    """
+    This function transfers a file or directory between the local machine and the vpu
+
+    Parameters
+    ----------
+    ssh : SSHClient
+        ssh library native handle
+    scp : SCPClient
+        scp library native handle
+    src : str
+        path to source file or directory
+    dst : str
+        path to destination file or directory
+    src_is_local : bool, optional
+        Whether the source is local or remote, by default True
+    """
+    if src_is_local:
+        if Path(src).exists():
+            if Path(src).is_dir():
+                dst = "/".join(dst.split("/")[:-1])
+                if not SSH_path_exists(ssh, dst):
+                    SSH_makedirs(ssh, dst)
+                scp.put(
+                    files=[src],
+                    remote_path=dst, recursive=True)
+            else:
+                scp.put(
+                    files=[src],
+                    remote_path=dst)
+    else:
+        if SSH_path_exists(ssh, src):
+            if SSH_isdir(ssh, src):
+                scp.get(src, dst, recursive=True)
+            else:
+                scp.get(src, dst)
```

### Comparing `ovp_docker_utils-1.0.3/ovp_docker_utils.egg-info/SOURCES.txt` & `ovp_docker_utils-1.0.4/ovp_docker_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovp_docker_utils-1.0.3/setup.py` & `ovp_docker_utils-1.0.4/setup.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-from setuptools import setup, find_packages
-
-import sys
-from pathlib import Path
-sys.path.append(str(Path(__file__).parent/'ovp_docker_utils'))
-from __version__ import __version__
-
-
-NAME = 'ovp_docker_utils'
-VERSION = __version__
-DESCRIPTION = 'O3R docker deployment utilities'
-LONG_DESCRIPTION = 'A package for deployment and testing of code for the O3R camera system via docker container on the OVP8XX platform.'
-
-setup(
-    name= NAME,
-    version=VERSION,
-    description=DESCRIPTION,
-    long_description=LONG_DESCRIPTION,
-    author="ifm gmbh",
-    # author_email="",
-    packages=find_packages(include=['ovp_docker_utils']),
-    install_requires=[
-        'pyyaml',
-        'scp',
-        'ifm3dpy',
-        'pydantic',
-        'semver',
-    ],
-    entry_points = {
-        'console_scripts':[
-            'ovp_docker_utils=ovp_docker_utils.ovp_docker_utils:app']
-    }
+from setuptools import setup, find_packages
+
+import sys
+from pathlib import Path
+sys.path.append(str(Path(__file__).parent/'ovp_docker_utils'))
+from __version__ import __version__
+
+
+NAME = 'ovp_docker_utils'
+VERSION = __version__
+DESCRIPTION = 'O3R docker deployment utilities'
+LONG_DESCRIPTION = 'A package for deployment and testing of code for the O3R camera system via docker container on the OVP8XX platform.'
+
+setup(
+    name= NAME,
+    version=VERSION,
+    description=DESCRIPTION,
+    long_description=LONG_DESCRIPTION,
+    author="ifm gmbh",
+    # author_email="",
+    packages=find_packages(include=['ovp_docker_utils']),
+    install_requires=[
+        'pyyaml',
+        'scp',
+        'ifm3dpy',
+        'pydantic',
+        'semver',
+    ],
+    entry_points = {
+        'console_scripts':[
+            'ovp_docker_utils=ovp_docker_utils.ovp_docker_utils:app']
+    }
 )
```

