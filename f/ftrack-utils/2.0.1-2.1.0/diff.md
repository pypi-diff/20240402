# Comparing `tmp/ftrack_utils-2.0.1.tar.gz` & `tmp/ftrack_utils-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ftrack_utils-2.0.1.tar", max compression
+gzip compressed data, was "ftrack_utils-2.1.0.tar", max compression
```

## Comparing `ftrack_utils-2.0.1.tar` & `ftrack_utils-2.1.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
--rw-r--r--   0        0        0    10176 2024-03-08 10:45:49.114759 ftrack_utils-2.0.1/LICENSE.txt
--rw-r--r--   0        0        0       56 2024-03-08 10:45:49.114759 ftrack_utils-2.0.1/README.md
--rw-r--r--   0        0        0      783 2024-03-08 10:45:49.114759 ftrack_utils-2.0.1/pyproject.toml
--rw-r--r--   0        0        0      353 2024-03-08 10:45:49.114759 ftrack_utils-2.0.1/source/ftrack_utils/__init__.py
--rw-r--r--   0        0        0      251 2024-03-08 10:45:49.114759 ftrack_utils-2.0.1/source/ftrack_utils/decorators/__init__.py
--rw-r--r--   0        0        0      992 2024-03-08 10:45:49.114759 ftrack_utils-2.0.1/source/ftrack_utils/decorators/asynchronous.py
--rw-r--r--   0        0        0     1133 2024-03-08 10:45:49.114759 ftrack_utils-2.0.1/source/ftrack_utils/decorators/session.py
--rw-r--r--   0        0        0     5642 2024-03-08 10:45:49.114759 ftrack_utils-2.0.1/source/ftrack_utils/decorators/track_usage.py
--rw-r--r--   0        0        0       57 2024-03-08 10:45:49.114759 ftrack_utils-2.0.1/source/ftrack_utils/directories/__init__.py
--rw-r--r--   0        0        0      514 2024-03-08 10:45:49.114759 ftrack_utils-2.0.1/source/ftrack_utils/directories/scan_dir.py
--rw-r--r--   0        0        0       57 2024-03-08 10:45:49.114759 ftrack_utils-2.0.1/source/ftrack_utils/extensions/__init__.py
--rw-r--r--   0        0        0      339 2024-03-08 10:45:49.114759 ftrack_utils-2.0.1/source/ftrack_utils/extensions/environment.py
--rw-r--r--   0        0        0     4703 2024-03-08 10:45:49.114759 ftrack_utils-2.0.1/source/ftrack_utils/extensions/registry.py
--rw-r--r--   0        0        0       57 2024-03-08 10:45:49.114759 ftrack_utils-2.0.1/source/ftrack_utils/framework/__init__.py
--rw-r--r--   0        0        0       57 2024-03-08 10:45:49.114759 ftrack_utils-2.0.1/source/ftrack_utils/framework/config/__init__.py
--rw-r--r--   0        0        0     4843 2024-03-08 10:45:49.114759 ftrack_utils-2.0.1/source/ftrack_utils/framework/config/tool.py
--rw-r--r--   0        0        0      270 2024-03-08 10:45:49.114759 ftrack_utils-2.0.1/source/ftrack_utils/framework/remote.py
--rw-r--r--   0        0        0      980 2024-03-08 10:45:49.114759 ftrack_utils-2.0.1/source/ftrack_utils/json/__init__.py
--rw-r--r--   0        0        0       57 2024-03-08 10:45:49.114759 ftrack_utils-2.0.1/source/ftrack_utils/modules/__init__.py
--rw-r--r--   0        0        0      698 2024-03-08 10:45:49.114759 ftrack_utils-2.0.1/source/ftrack_utils/modules/scan_modules.py
--rw-r--r--   0        0        0     1624 2024-03-08 10:45:49.114759 ftrack_utils-2.0.1/source/ftrack_utils/paths/__init__.py
--rw-r--r--   0        0        0      191 2024-03-08 10:45:49.114759 ftrack_utils-2.0.1/source/ftrack_utils/server/__init__.py
--rw-r--r--   0        0        0      996 2024-03-08 10:45:49.114759 ftrack_utils-2.0.1/source/ftrack_utils/server/send_event.py
--rw-r--r--   0        0        0      631 2024-03-08 10:45:49.114759 ftrack_utils-2.0.1/source/ftrack_utils/server/track_usage.py
--rw-r--r--   0        0        0     1863 2024-03-08 10:45:49.114759 ftrack_utils-2.0.1/source/ftrack_utils/string/__init__.py
--rw-r--r--   0        0        0      661 2024-03-08 10:45:49.114759 ftrack_utils-2.0.1/source/ftrack_utils/threading/__init__.py
--rw-r--r--   0        0        0      111 2024-03-08 10:45:49.114759 ftrack_utils-2.0.1/source/ftrack_utils/usage/__init__.py
--rw-r--r--   0        0        0     2238 2024-03-08 10:45:49.114759 ftrack_utils-2.0.1/source/ftrack_utils/usage/track_usage.py
--rw-r--r--   0        0        0      940 2024-03-08 10:45:49.114759 ftrack_utils-2.0.1/source/ftrack_utils/version/__init__.py
--rw-r--r--   0        0        0      885 1970-01-01 00:00:00.000000 ftrack_utils-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0    10176 2024-04-02 08:39:14.288332 ftrack_utils-2.1.0/LICENSE.txt
+-rw-r--r--   0        0        0      154 2024-04-02 08:39:14.288332 ftrack_utils-2.1.0/README.md
+-rw-r--r--   0        0        0      783 2024-04-02 08:39:14.288332 ftrack_utils-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0      353 2024-04-02 08:39:14.288332 ftrack_utils-2.1.0/source/ftrack_utils/__init__.py
+-rw-r--r--   0        0        0      251 2024-04-02 08:39:14.288332 ftrack_utils-2.1.0/source/ftrack_utils/decorators/__init__.py
+-rw-r--r--   0        0        0      992 2024-04-02 08:39:14.288332 ftrack_utils-2.1.0/source/ftrack_utils/decorators/asynchronous.py
+-rw-r--r--   0        0        0     1133 2024-04-02 08:39:14.288332 ftrack_utils-2.1.0/source/ftrack_utils/decorators/session.py
+-rw-r--r--   0        0        0     5652 2024-04-02 08:39:14.288332 ftrack_utils-2.1.0/source/ftrack_utils/decorators/track_usage.py
+-rw-r--r--   0        0        0       57 2024-04-02 08:39:14.288332 ftrack_utils-2.1.0/source/ftrack_utils/directories/__init__.py
+-rw-r--r--   0        0        0      514 2024-04-02 08:39:14.288332 ftrack_utils-2.1.0/source/ftrack_utils/directories/scan_dir.py
+-rw-r--r--   0        0        0       57 2024-04-02 08:39:14.288332 ftrack_utils-2.1.0/source/ftrack_utils/extensions/__init__.py
+-rw-r--r--   0        0        0      349 2024-04-02 08:39:14.288332 ftrack_utils-2.1.0/source/ftrack_utils/extensions/environment.py
+-rw-r--r--   0        0        0     1708 2024-04-02 08:39:14.288332 ftrack_utils-2.1.0/source/ftrack_utils/extensions/overrides.py
+-rw-r--r--   0        0        0     5712 2024-04-02 08:39:14.288332 ftrack_utils-2.1.0/source/ftrack_utils/extensions/registry.py
+-rw-r--r--   0        0        0       57 2024-04-02 08:39:14.288332 ftrack_utils-2.1.0/source/ftrack_utils/framework/__init__.py
+-rw-r--r--   0        0        0       57 2024-04-02 08:39:14.288332 ftrack_utils-2.1.0/source/ftrack_utils/framework/config/__init__.py
+-rw-r--r--   0        0        0     4843 2024-04-02 08:39:14.288332 ftrack_utils-2.1.0/source/ftrack_utils/framework/config/tool.py
+-rw-r--r--   0        0        0      270 2024-04-02 08:39:14.288332 ftrack_utils-2.1.0/source/ftrack_utils/framework/remote.py
+-rw-r--r--   0        0        0      980 2024-04-02 08:39:14.288332 ftrack_utils-2.1.0/source/ftrack_utils/json/__init__.py
+-rw-r--r--   0        0        0       57 2024-04-02 08:39:14.288332 ftrack_utils-2.1.0/source/ftrack_utils/modules/__init__.py
+-rw-r--r--   0        0        0      698 2024-04-02 08:39:14.288332 ftrack_utils-2.1.0/source/ftrack_utils/modules/scan_modules.py
+-rw-r--r--   0        0        0     1624 2024-04-02 08:39:14.288332 ftrack_utils-2.1.0/source/ftrack_utils/paths/__init__.py
+-rw-r--r--   0        0        0      191 2024-04-02 08:39:14.288332 ftrack_utils-2.1.0/source/ftrack_utils/server/__init__.py
+-rw-r--r--   0        0        0      996 2024-04-02 08:39:14.288332 ftrack_utils-2.1.0/source/ftrack_utils/server/send_event.py
+-rw-r--r--   0        0        0      633 2024-04-02 08:39:14.288332 ftrack_utils-2.1.0/source/ftrack_utils/server/track_usage.py
+-rw-r--r--   0        0        0     1863 2024-04-02 08:39:14.288332 ftrack_utils-2.1.0/source/ftrack_utils/string/__init__.py
+-rw-r--r--   0        0        0      661 2024-04-02 08:39:14.288332 ftrack_utils-2.1.0/source/ftrack_utils/threading/__init__.py
+-rw-r--r--   0        0        0      111 2024-04-02 08:39:14.288332 ftrack_utils-2.1.0/source/ftrack_utils/usage/__init__.py
+-rw-r--r--   0        0        0     2239 2024-04-02 08:39:14.288332 ftrack_utils-2.1.0/source/ftrack_utils/usage/track_usage.py
+-rw-r--r--   0        0        0     1639 2024-04-02 08:39:14.288332 ftrack_utils-2.1.0/source/ftrack_utils/version/__init__.py
+-rw-r--r--   0        0        0      983 1970-01-01 00:00:00.000000 ftrack_utils-2.1.0/PKG-INFO
```

### Comparing `ftrack_utils-2.0.1/LICENSE.txt` & `ftrack_utils-2.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ftrack_utils-2.0.1/pyproject.toml` & `ftrack_utils-2.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ftrack-utils"
-version = "2.0.1"
+version = "2.1.0"
 description='ftrack utils library'
 authors = ["ftrack Integrations Team <integrations@backlight.co>"]
 readme = "README.md"
 packages = [{include = "ftrack_utils", from = "source"}]
 license = "Apache-2.0"
 homepage = "https://ftrack.com"
 repository = "https://github.com/ftrackhq/integrations/tree/main/libs/utils"
```

### Comparing `ftrack_utils-2.0.1/source/ftrack_utils/decorators/asynchronous.py` & `ftrack_utils-2.1.0/source/ftrack_utils/decorators/asynchronous.py`

 * *Files identical despite different names*

### Comparing `ftrack_utils-2.0.1/source/ftrack_utils/decorators/session.py` & `ftrack_utils-2.1.0/source/ftrack_utils/decorators/session.py`

 * *Files identical despite different names*

### Comparing `ftrack_utils-2.0.1/source/ftrack_utils/decorators/track_usage.py` & `ftrack_utils-2.1.0/source/ftrack_utils/decorators/track_usage.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import sys
 import logging
 import inspect
 
 logger = logging.getLogger('ftrack_utils:usage')
 
 
-def track_framework_usage(event_name, metadata, tracked_args=[]):
+def track_framework_usage(event_name, metadata, tracked_args=None):
     """
     Decorator to track usage of framework functions.
 
     This decorator wraps a function to track its usage along with specified metadata and arguments. It ensures that a
     UsageTracker instance is set and available. If not, it attempts to initialize a default one using the session
     attribute of the first argument of the wrapped function, which is expected to be an instance of a class with a
     session attribute.
@@ -39,14 +39,17 @@
 
     This will track the usage of `some_function`, including the values of `arg1` and `arg2` in the metadata.
 
     Returns:
     The original function wrapped with usage tracking functionality.
     """
 
+    if not tracked_args:
+        tracked_args = []
+
     def decorator(func):
         @functools.wraps(func)
         def wrapper(*args, **kwargs):
             from ftrack_utils.usage import (
                 get_usage_tracker,
                 set_usage_tracker,
                 UsageTracker,
@@ -106,21 +109,21 @@
 
                 except Exception as e:
                     logger.error(e)
 
                 finally:
                     usage_tracker = get_usage_tracker()
 
-            # Get the function's argument names and values
-            func_args = inspect.signature(func).parameters
-            arg_names = list(func_args.keys())
-
-            # Build a dictionary of argument names and values
-            arg_values = args + tuple(kwargs.values())
-            args_metadata = dict(zip(arg_names, arg_values))
+            # Get the function's signature
+            sig = inspect.signature(func)
+            bound_args = sig.bind(*args, **kwargs)
+            bound_args.apply_defaults()
+
+            # Build a dictionary of argument names and their bound values
+            args_metadata = bound_args.arguments
 
             # Update metadata with function arguments if specified in kwarg_mapping_list
             for key in tracked_args:
                 if key in args_metadata:
                     metadata[key] = args_metadata[key]
                 else:
                     logger.warning(
```

### Comparing `ftrack_utils-2.0.1/source/ftrack_utils/directories/scan_dir.py` & `ftrack_utils-2.1.0/source/ftrack_utils/directories/scan_dir.py`

 * *Files identical despite different names*

### Comparing `ftrack_utils-2.0.1/source/ftrack_utils/framework/config/tool.py` & `ftrack_utils-2.1.0/source/ftrack_utils/framework/config/tool.py`

 * *Files identical despite different names*

### Comparing `ftrack_utils-2.0.1/source/ftrack_utils/json/__init__.py` & `ftrack_utils-2.1.0/source/ftrack_utils/json/__init__.py`

 * *Files identical despite different names*

### Comparing `ftrack_utils-2.0.1/source/ftrack_utils/modules/scan_modules.py` & `ftrack_utils-2.1.0/source/ftrack_utils/modules/scan_modules.py`

 * *Files identical despite different names*

### Comparing `ftrack_utils-2.0.1/source/ftrack_utils/paths/__init__.py` & `ftrack_utils-2.1.0/source/ftrack_utils/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `ftrack_utils-2.0.1/source/ftrack_utils/server/send_event.py` & `ftrack_utils-2.1.0/source/ftrack_utils/server/send_event.py`

 * *Files identical despite different names*

### Comparing `ftrack_utils-2.0.1/source/ftrack_utils/server/track_usage.py` & `ftrack_utils-2.1.0/source/ftrack_utils/server/track_usage.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 from ftrack_utils.decorators import asynchronous
 from ftrack_utils.server.send_event import send_async_event, send_event
 
 
 logger = logging.getLogger('ftrack_utils:usage')
 
 
-def send_usage_event(session, event_name, metadata=None, asynchronous=True):
+def send_usage_event(session, event_name, metadata=None, _asynchronous=True):
     '''Send usage event with *event_name* and *metadata*.
 
     If asynchronous is True, the event will be sent in a new thread.
     '''
 
-    if asynchronous:
+    if _asynchronous:
         send_async_event(session, '_track_usage', event_name, metadata)
     else:
         send_event(session, '_track_usage', event_name, metadata)
```

### Comparing `ftrack_utils-2.0.1/source/ftrack_utils/string/__init__.py` & `ftrack_utils-2.1.0/source/ftrack_utils/string/__init__.py`

 * *Files identical despite different names*

### Comparing `ftrack_utils-2.0.1/source/ftrack_utils/threading/__init__.py` & `ftrack_utils-2.1.0/source/ftrack_utils/threading/__init__.py`

 * *Files identical despite different names*

### Comparing `ftrack_utils-2.0.1/source/ftrack_utils/usage/track_usage.py` & `ftrack_utils-2.1.0/source/ftrack_utils/usage/track_usage.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,12 +64,12 @@
         # To not modify the default metadata dictionary instance, we do a deep copy of it.
         default_metadata = copy.deepcopy(self._default_data)
         default_metadata.update(metadata)
         send_usage_event(
             self._session,
             event_name,
             default_metadata,
-            asynchronous=True,
+            _asynchronous=True,
         )
         logger.debug(
             f"Tracking: event_name: {event_name}, metadata: {metadata}"
         )
```

### Comparing `ftrack_utils-2.0.1/PKG-INFO` & `ftrack_utils-2.1.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ftrack-utils
-Version: 2.0.1
+Version: 2.1.0
 Summary: ftrack utils library
 Home-page: https://ftrack.com
 License: Apache-2.0
 Author: ftrack Integrations Team
 Author-email: integrations@backlight.co
 Requires-Python: >=3.7,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
@@ -19,8 +19,9 @@
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Project-URL: Repository, https://github.com/ftrackhq/integrations/tree/main/libs/utils
 Description-Content-Type: text/markdown
 
 # Utils
 
 This is the ftrack integrations utils library.
+This library contains a bunch of utility functions used around all ftrack integrations products.
```

