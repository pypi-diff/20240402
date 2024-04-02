# Comparing `tmp/nornir_nautobot-3.1.2.tar.gz` & `tmp/nornir_nautobot-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nornir_nautobot-3.1.2.tar", max compression
+gzip compressed data, was "nornir_nautobot-3.2.0.tar", max compression
```

## Comparing `nornir_nautobot-3.1.2.tar` & `nornir_nautobot-3.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1743 2024-03-15 01:09:50.847231 nornir_nautobot-3.1.2/README.md
--rw-r--r--   0        0        0       33 2024-03-15 01:09:50.847231 nornir_nautobot-3.1.2/nornir_nautobot/__init__.py
--rw-r--r--   0        0        0      126 2024-03-15 01:09:50.847231 nornir_nautobot-3.1.2/nornir_nautobot/exceptions.py
--rw-r--r--   0        0        0       33 2024-03-15 01:09:50.847231 nornir_nautobot-3.1.2/nornir_nautobot/plugins/__init__.py
--rw-r--r--   0        0        0       33 2024-03-15 01:09:50.851230 nornir_nautobot-3.1.2/nornir_nautobot/plugins/inventory/__init__.py
--rw-r--r--   0        0        0     6153 2024-03-15 01:09:50.851230 nornir_nautobot-3.1.2/nornir_nautobot/plugins/inventory/nautobot.py
--rw-r--r--   0        0        0     2668 2024-03-15 01:09:50.851230 nornir_nautobot-3.1.2/nornir_nautobot/plugins/processors/__init__.py
--rw-r--r--   0        0        0     5355 2024-03-15 01:09:50.851230 nornir_nautobot-3.1.2/nornir_nautobot/plugins/processors/get_config.py
--rw-r--r--   0        0        0     2478 2024-03-15 01:09:50.851230 nornir_nautobot-3.1.2/nornir_nautobot/plugins/tasks/dispatcher/__init__.py
--rw-r--r--   0        0        0      400 2024-03-15 01:09:50.851230 nornir_nautobot-3.1.2/nornir_nautobot/plugins/tasks/dispatcher/arista_eos.py
--rw-r--r--   0        0        0      395 2024-03-15 01:09:50.851230 nornir_nautobot-3.1.2/nornir_nautobot/plugins/tasks/dispatcher/cisco_asa.py
--rw-r--r--   0        0        0      395 2024-03-15 01:09:50.851230 nornir_nautobot-3.1.2/nornir_nautobot/plugins/tasks/dispatcher/cisco_ios.py
--rw-r--r--   0        0        0      400 2024-03-15 01:09:50.851230 nornir_nautobot-3.1.2/nornir_nautobot/plugins/tasks/dispatcher/cisco_nxos.py
--rw-r--r--   0        0        0      390 2024-03-15 01:09:50.851230 nornir_nautobot-3.1.2/nornir_nautobot/plugins/tasks/dispatcher/cisco_xr.py
--rw-r--r--   0        0        0    20703 2024-03-15 01:09:50.851230 nornir_nautobot-3.1.2/nornir_nautobot/plugins/tasks/dispatcher/default.py
--rw-r--r--   0        0        0      439 2024-03-15 01:09:50.851230 nornir_nautobot-3.1.2/nornir_nautobot/plugins/tasks/dispatcher/juniper_junos.py
--rw-r--r--   0        0        0     9881 2024-03-15 01:09:50.851230 nornir_nautobot-3.1.2/nornir_nautobot/plugins/tasks/dispatcher/mikrotik_routeros.py
--rw-r--r--   0        0        0     3150 2024-03-15 01:09:50.851230 nornir_nautobot-3.1.2/nornir_nautobot/plugins/tasks/dispatcher/ruckus_fastiron.py
--rw-r--r--   0        0        0     7468 2024-03-15 01:09:50.851230 nornir_nautobot-3.1.2/nornir_nautobot/plugins/tasks/dispatcher/ruckus_smartzone.py
--rw-r--r--   0        0        0      921 2024-03-15 01:09:50.851230 nornir_nautobot-3.1.2/nornir_nautobot/utils/helpers.py
--rw-r--r--   0        0        0      913 2024-03-15 01:09:50.851230 nornir_nautobot-3.1.2/nornir_nautobot/utils/mock.py
--rw-r--r--   0        0        0     3010 2024-03-15 01:10:01.927250 nornir_nautobot-3.1.2/pyproject.toml
--rw-r--r--   0        0        0     3292 1970-01-01 00:00:00.000000 nornir_nautobot-3.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1743 2024-04-02 19:00:11.762138 nornir_nautobot-3.2.0/README.md
+-rw-r--r--   0        0        0       33 2024-04-02 19:00:11.766138 nornir_nautobot-3.2.0/nornir_nautobot/__init__.py
+-rw-r--r--   0        0        0      126 2024-04-02 19:00:11.766138 nornir_nautobot-3.2.0/nornir_nautobot/exceptions.py
+-rw-r--r--   0        0        0       33 2024-04-02 19:00:11.766138 nornir_nautobot-3.2.0/nornir_nautobot/plugins/__init__.py
+-rw-r--r--   0        0        0       33 2024-04-02 19:00:11.766138 nornir_nautobot-3.2.0/nornir_nautobot/plugins/inventory/__init__.py
+-rw-r--r--   0        0        0     6153 2024-04-02 19:00:11.766138 nornir_nautobot-3.2.0/nornir_nautobot/plugins/inventory/nautobot.py
+-rw-r--r--   0        0        0     2668 2024-04-02 19:00:11.766138 nornir_nautobot-3.2.0/nornir_nautobot/plugins/processors/__init__.py
+-rw-r--r--   0        0        0     5355 2024-04-02 19:00:11.766138 nornir_nautobot-3.2.0/nornir_nautobot/plugins/processors/get_config.py
+-rw-r--r--   0        0        0     2478 2024-04-02 19:00:11.766138 nornir_nautobot-3.2.0/nornir_nautobot/plugins/tasks/dispatcher/__init__.py
+-rw-r--r--   0        0        0      400 2024-04-02 19:00:11.766138 nornir_nautobot-3.2.0/nornir_nautobot/plugins/tasks/dispatcher/arista_eos.py
+-rw-r--r--   0        0        0      395 2024-04-02 19:00:11.766138 nornir_nautobot-3.2.0/nornir_nautobot/plugins/tasks/dispatcher/cisco_asa.py
+-rw-r--r--   0        0        0      395 2024-04-02 19:00:11.766138 nornir_nautobot-3.2.0/nornir_nautobot/plugins/tasks/dispatcher/cisco_ios.py
+-rw-r--r--   0        0        0      400 2024-04-02 19:00:11.766138 nornir_nautobot-3.2.0/nornir_nautobot/plugins/tasks/dispatcher/cisco_nxos.py
+-rw-r--r--   0        0        0      390 2024-04-02 19:00:11.766138 nornir_nautobot-3.2.0/nornir_nautobot/plugins/tasks/dispatcher/cisco_xr.py
+-rw-r--r--   0        0        0    20382 2024-04-02 19:00:11.766138 nornir_nautobot-3.2.0/nornir_nautobot/plugins/tasks/dispatcher/default.py
+-rw-r--r--   0        0        0      439 2024-04-02 19:00:11.766138 nornir_nautobot-3.2.0/nornir_nautobot/plugins/tasks/dispatcher/juniper_junos.py
+-rw-r--r--   0        0        0     9881 2024-04-02 19:00:11.766138 nornir_nautobot-3.2.0/nornir_nautobot/plugins/tasks/dispatcher/mikrotik_routeros.py
+-rw-r--r--   0        0        0     3150 2024-04-02 19:00:11.766138 nornir_nautobot-3.2.0/nornir_nautobot/plugins/tasks/dispatcher/ruckus_fastiron.py
+-rw-r--r--   0        0        0     7468 2024-04-02 19:00:11.766138 nornir_nautobot-3.2.0/nornir_nautobot/plugins/tasks/dispatcher/ruckus_smartzone.py
+-rw-r--r--   0        0        0     1736 2024-04-02 19:00:11.766138 nornir_nautobot-3.2.0/nornir_nautobot/utils/helpers.py
+-rw-r--r--   0        0        0      913 2024-04-02 19:00:11.766138 nornir_nautobot-3.2.0/nornir_nautobot/utils/mock.py
+-rw-r--r--   0        0        0     3010 2024-04-02 19:00:25.946086 nornir_nautobot-3.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3292 1970-01-01 00:00:00.000000 nornir_nautobot-3.2.0/PKG-INFO
```

### Comparing `nornir_nautobot-3.1.2/README.md` & `nornir_nautobot-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `nornir_nautobot-3.1.2/nornir_nautobot/plugins/inventory/nautobot.py` & `nornir_nautobot-3.2.0/nornir_nautobot/plugins/inventory/nautobot.py`

 * *Files identical despite different names*

### Comparing `nornir_nautobot-3.1.2/nornir_nautobot/plugins/processors/__init__.py` & `nornir_nautobot-3.2.0/nornir_nautobot/plugins/processors/__init__.py`

 * *Files identical despite different names*

### Comparing `nornir_nautobot-3.1.2/nornir_nautobot/plugins/processors/get_config.py` & `nornir_nautobot-3.2.0/nornir_nautobot/plugins/processors/get_config.py`

 * *Files identical despite different names*

### Comparing `nornir_nautobot-3.1.2/nornir_nautobot/plugins/tasks/dispatcher/__init__.py` & `nornir_nautobot-3.2.0/nornir_nautobot/plugins/tasks/dispatcher/__init__.py`

 * *Files identical despite different names*

### Comparing `nornir_nautobot-3.1.2/nornir_nautobot/plugins/tasks/dispatcher/default.py` & `nornir_nautobot-3.2.0/nornir_nautobot/plugins/tasks/dispatcher/default.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,17 +19,17 @@
 
 from nornir.core.exceptions import NornirSubTaskError
 from nornir.core.task import Result, Task
 
 from nornir_jinja2.plugins.tasks import template_file
 from nornir_napalm.plugins.tasks import napalm_configure, napalm_get
 from nornir_netmiko.tasks import netmiko_send_command
-
 from nornir_nautobot.exceptions import NornirNautobotException
-from nornir_nautobot.utils.helpers import make_folder
+from nornir_nautobot.utils.helpers import make_folder, get_stack_trace, is_truthy
+
 
 _logger = logging.getLogger(__name__)
 
 
 class DispatcherMixin:
     """Mixin for non-network driver related tasks."""
 
@@ -145,14 +145,15 @@
         obj,
         jinja_template: str,
         jinja_root_path: str,
         output_file_location: str,
         jinja_filters: Optional[dict] = None,
         jinja_env: Optional[jinja2.Environment] = None,
     ) -> Result:
+        # pylint: disable=too-many-locals
         """A small wrapper around template_file Nornir task.
 
         Args:
             task (Task): Nornir Task.
             logger (logging.Logger): Logger that may be a Nautobot Jobs or Python logger.
             obj (Device): A Nautobot Device Django ORM object instance.
             jinja_template (str): The file location of the actual Jinja template.
@@ -170,37 +171,30 @@
                 task=template_file,
                 template=jinja_template,
                 path=jinja_root_path,
                 jinja_filters=jinja_filters,
                 jinja_env=jinja_env,
             )[0].result
         except NornirSubTaskError as exc:
-            if isinstance(exc.result.exception, jinja2.exceptions.UndefinedError):  # pylint: disable=no-else-raise
-                error_msg = (
-                    f"`E1010:` There was a jinja2.exceptions.UndefinedError error: ``{str(exc.result.exception)}``"
-                )
-                logger.error(error_msg, extra={"object": obj})
-                raise NornirNautobotException(error_msg)
+            stack_trace = get_stack_trace(exc.result.exception)
 
-            elif isinstance(exc.result.exception, jinja2.TemplateSyntaxError):
-                error_msg = (f"`E1011:` There was a jinja2.TemplateSyntaxError error: ``{str(exc.result.exception)}``",)
-                logger.error(error_msg, extra={"object": obj})
-                raise NornirNautobotException(error_msg)
+            error_mapping = {
+                jinja2.exceptions.UndefinedError: ("E1010", "Undefined variable in Jinja2 template"),
+                jinja2.TemplateSyntaxError: ("E1011", "Syntax error in Jinja2 template"),
+                jinja2.TemplateNotFound: ("E1012", "Jinja2 template not found"),
+                jinja2.TemplateError: ("E1013", "General Jinja2 template error"),
+            }
+
+            for error, (code, message) in error_mapping.items():
+                if isinstance(exc.result.exception, error):
+                    error_msg = f"`{code}:` {message} - ``{str(exc.result.exception)}``\n```\n{stack_trace}\n```"
+                    logger.error(error_msg, extra={"object": obj})
+                    raise NornirNautobotException(error_msg)
 
-            elif isinstance(exc.result.exception, jinja2.TemplateNotFound):
-                error_msg = f"`E1012:` There was an issue finding the template and a jinja2.TemplateNotFound error was raised: ``{str(exc.result.exception)}``"
-                logger.error(error_msg, extra={"object": obj})
-                raise NornirNautobotException(error_msg)
-
-            elif isinstance(exc.result.exception, jinja2.TemplateError):
-                error_msg = f"`E1013:` There was an issue general Jinja error: ``{str(exc.result.exception)}``"
-                logger.error(error_msg, extra={"object": obj})
-                raise NornirNautobotException(error_msg)
-
-            error_msg = f"`E1014:` Failed with an unknown issue. `{exc.result.exception}`"
+            error_msg = f"`E1014:` Unknown error - `{exc.result.exception}`\n```\n{stack_trace}\n```"
             logger.error(error_msg, extra={"object": obj})
             raise NornirNautobotException(error_msg)
 
         make_folder(os.path.dirname(output_file_location))
         with open(output_file_location, "w", encoding="utf8") as filehandler:
             filehandler.write(filled_template)
         return Result(host=task.host, result={"config": filled_template})
@@ -455,15 +449,19 @@
             Result: Nornir Result object with a dict as a result containing the running configuration
                 { "config: <running configuration> }
         """
         logger.debug(f"Executing get_config for {task.host.name} on {task.host.platform}")
         command = cls.config_command
 
         try:
-            result = task.run(task=netmiko_send_command, command_string=command)
+            result = task.run(
+                task=netmiko_send_command,
+                command_string=command,
+                enable=is_truthy(os.getenv("NORNIR_NAUTOBOT_NETMIKO_ENABLE_DEFAULT", default="True")),
+            )
         except NornirSubTaskError as exc:
             if isinstance(exc.result.exception, NetmikoAuthenticationException):
                 error_msg = f"`E1017:` Failed with an authentication issue: `{exc.result.exception}`"
                 logger.error(error_msg, extra={"object": obj})
                 raise NornirNautobotException(error_msg)
 
             if isinstance(exc.result.exception, NetmikoTimeoutException):
```

### Comparing `nornir_nautobot-3.1.2/nornir_nautobot/plugins/tasks/dispatcher/mikrotik_routeros.py` & `nornir_nautobot-3.2.0/nornir_nautobot/plugins/tasks/dispatcher/mikrotik_routeros.py`

 * *Files identical despite different names*

### Comparing `nornir_nautobot-3.1.2/nornir_nautobot/plugins/tasks/dispatcher/ruckus_fastiron.py` & `nornir_nautobot-3.2.0/nornir_nautobot/plugins/tasks/dispatcher/ruckus_fastiron.py`

 * *Files identical despite different names*

### Comparing `nornir_nautobot-3.1.2/nornir_nautobot/plugins/tasks/dispatcher/ruckus_smartzone.py` & `nornir_nautobot-3.2.0/nornir_nautobot/plugins/tasks/dispatcher/ruckus_smartzone.py`

 * *Files identical despite different names*

### Comparing `nornir_nautobot-3.1.2/nornir_nautobot/utils/helpers.py` & `nornir_nautobot-3.2.0/nornir_nautobot/utils/helpers.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """A set of helper utilities."""
 
 import errno
 import os
 import logging
 import importlib
+import traceback
 
 LOGGER = logging.getLogger(__name__)
 
 
 def make_folder(folder):
     """Helper method to sanely create folders."""
     if not os.path.exists(folder):
@@ -27,7 +28,35 @@
 def import_string(dotted_path):
     """Import the python object by dotted_path string ."""
     module_name, class_name = dotted_path.rsplit(".", 1)
     try:
         return getattr(importlib.import_module(module_name), class_name)
     except (ModuleNotFoundError, AttributeError):
         return None
+
+
+def get_stack_trace(exc: Exception) -> str:
+    """Converts the provided exception's stack trace into a string."""
+    stack_trace_lines = traceback.format_exception(type(exc), exc, exc.__traceback__)
+    return "".join(stack_trace_lines)
+
+
+def is_truthy(arg):
+    """Convert "truthy" strings into Booleans.
+
+    Args:
+        arg (str): Truthy string (True values are y, yes, t, true, on and 1; false values are n, no,
+        f, false, off and 0. Raises ValueError if val is anything else.
+
+    Examples:
+        >>> is_truthy('yes')
+        True
+    """
+    if isinstance(arg, bool):
+        return arg
+
+    val = str(arg).lower()
+    if val in ("y", "yes", "t", "true", "on", "1"):
+        return True
+    if val in ("n", "no", "f", "false", "off", "0"):
+        return False
+    return True
```

### Comparing `nornir_nautobot-3.1.2/nornir_nautobot/utils/mock.py` & `nornir_nautobot-3.2.0/nornir_nautobot/utils/mock.py`

 * *Files identical despite different names*

### Comparing `nornir_nautobot-3.1.2/pyproject.toml` & `nornir_nautobot-3.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nornir-nautobot"
-version = "v3.1.2"
+version = "v3.2.0"
 description = "Nornir Nautobot"
 authors = ["Network to Code, LLC <opensource@networktocode.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 keywords = ["Nautobot"]
 classifiers = [
   "Intended Audience :: Developers",
```

### Comparing `nornir_nautobot-3.1.2/PKG-INFO` & `nornir_nautobot-3.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nornir-nautobot
-Version: 3.1.2
+Version: 3.2.0
 Summary: Nornir Nautobot
 Home-page: https://nautobot.com
 License: Apache-2.0
 Keywords: Nautobot
 Author: Network to Code, LLC
 Author-email: opensource@networktocode.com
 Requires-Python: >=3.8,<4.0
```

