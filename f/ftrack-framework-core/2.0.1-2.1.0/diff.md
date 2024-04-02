# Comparing `tmp/ftrack_framework_core-2.0.1.tar.gz` & `tmp/ftrack_framework_core-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ftrack_framework_core-2.0.1.tar", max compression
+gzip compressed data, was "ftrack_framework_core-2.1.0.tar", max compression
```

## Comparing `ftrack_framework_core-2.0.1.tar` & `ftrack_framework_core-2.1.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    10176 2024-03-08 11:11:34.750665 ftrack_framework_core-2.0.1/LICENSE.txt
--rw-r--r--   0        0        0       74 2024-03-08 11:11:34.750665 ftrack_framework_core-2.0.1/README.md
--rw-r--r--   0        0        0     1196 2024-03-08 11:11:34.754665 ftrack_framework_core-2.0.1/pyproject.toml
--rw-r--r--   0        0        0      566 2024-03-08 11:11:34.754665 ftrack_framework_core-2.0.1/source/ftrack_framework_core/__init__.py
--rw-r--r--   0        0        0     6749 2024-03-08 11:11:34.754665 ftrack_framework_core-2.0.1/source/ftrack_framework_core/asset/__init__.py
--rw-r--r--   0        0        0     7568 2024-03-08 11:11:34.754665 ftrack_framework_core-2.0.1/source/ftrack_framework_core/asset/asset_info.py
--rw-r--r--   0        0        0     4130 2024-03-08 11:11:34.754665 ftrack_framework_core-2.0.1/source/ftrack_framework_core/asset/dcc_object.py
--rw-r--r--   0        0        0    17682 2024-03-08 11:11:34.754665 ftrack_framework_core-2.0.1/source/ftrack_framework_core/client/__init__.py
--rw-r--r--   0        0        0     8631 2024-03-08 11:11:34.754665 ftrack_framework_core-2.0.1/source/ftrack_framework_core/client/host_connection.py
--rw-r--r--   0        0        0     4603 2024-03-08 11:11:34.754665 ftrack_framework_core-2.0.1/source/ftrack_framework_core/configure_logging.py
--rw-r--r--   0        0        0     9330 2024-03-08 11:11:34.754665 ftrack_framework_core-2.0.1/source/ftrack_framework_core/engine/__init__.py
--rw-r--r--   0        0        0    17206 2024-03-08 11:11:34.754665 ftrack_framework_core-2.0.1/source/ftrack_framework_core/event/__init__.py
--rw-r--r--   0        0        0      162 2024-03-08 11:11:34.754665 ftrack_framework_core-2.0.1/source/ftrack_framework_core/exceptions/__init__.py
--rw-r--r--   0        0        0      277 2024-03-08 11:11:34.754665 ftrack_framework_core-2.0.1/source/ftrack_framework_core/exceptions/engine.py
--rw-r--r--   0        0        0     1501 2024-03-08 11:11:34.754665 ftrack_framework_core-2.0.1/source/ftrack_framework_core/exceptions/plugin.py
--rw-r--r--   0        0        0    12705 2024-03-08 11:11:34.754665 ftrack_framework_core-2.0.1/source/ftrack_framework_core/host/__init__.py
--rw-r--r--   0        0        0     8625 2024-03-08 11:11:34.754665 ftrack_framework_core-2.0.1/source/ftrack_framework_core/log/__init__.py
--rw-r--r--   0        0        0     1184 2024-03-08 11:11:34.754665 ftrack_framework_core-2.0.1/source/ftrack_framework_core/log/log_item.py
--rw-r--r--   0        0        0     1831 2024-03-08 11:11:34.754665 ftrack_framework_core-2.0.1/source/ftrack_framework_core/plugin/__init__.py
--rw-r--r--   0        0        0     1975 2024-03-08 11:11:34.754665 ftrack_framework_core-2.0.1/source/ftrack_framework_core/plugin/plugin_info.py
--rw-r--r--   0        0        0     7456 2024-03-08 11:11:34.754665 ftrack_framework_core-2.0.1/source/ftrack_framework_core/registry/__init__.py
--rw-r--r--   0        0        0     3437 2024-03-08 11:11:34.754665 ftrack_framework_core-2.0.1/source/ftrack_framework_core/widget/__init__.py
--rw-r--r--   0        0        0    17207 2024-03-08 11:11:34.754665 ftrack_framework_core-2.0.1/source/ftrack_framework_core/widget/dialog.py
--rw-r--r--   0        0        0     4475 2024-03-08 11:11:34.754665 ftrack_framework_core-2.0.1/source/ftrack_framework_core/widget/widget.py
--rw-r--r--   0        0        0     1165 1970-01-01 00:00:00.000000 ftrack_framework_core-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0    10176 2024-04-02 08:36:55.882153 ftrack_framework_core-2.1.0/LICENSE.txt
+-rw-r--r--   0        0        0      177 2024-04-02 08:36:55.882153 ftrack_framework_core-2.1.0/README.md
+-rw-r--r--   0        0        0     1196 2024-04-02 08:36:55.882153 ftrack_framework_core-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0      566 2024-04-02 08:36:55.882153 ftrack_framework_core-2.1.0/source/ftrack_framework_core/__init__.py
+-rw-r--r--   0        0        0     6749 2024-04-02 08:36:55.882153 ftrack_framework_core-2.1.0/source/ftrack_framework_core/asset/__init__.py
+-rw-r--r--   0        0        0     7568 2024-04-02 08:36:55.886153 ftrack_framework_core-2.1.0/source/ftrack_framework_core/asset/asset_info.py
+-rw-r--r--   0        0        0     4130 2024-04-02 08:36:55.886153 ftrack_framework_core-2.1.0/source/ftrack_framework_core/asset/dcc_object.py
+-rw-r--r--   0        0        0    17702 2024-04-02 08:36:55.886153 ftrack_framework_core-2.1.0/source/ftrack_framework_core/client/__init__.py
+-rw-r--r--   0        0        0     8631 2024-04-02 08:36:55.886153 ftrack_framework_core-2.1.0/source/ftrack_framework_core/client/host_connection.py
+-rw-r--r--   0        0        0     4603 2024-04-02 08:36:55.886153 ftrack_framework_core-2.1.0/source/ftrack_framework_core/configure_logging.py
+-rw-r--r--   0        0        0     9330 2024-04-02 08:36:55.886153 ftrack_framework_core-2.1.0/source/ftrack_framework_core/engine/__init__.py
+-rw-r--r--   0        0        0    17206 2024-04-02 08:36:55.886153 ftrack_framework_core-2.1.0/source/ftrack_framework_core/event/__init__.py
+-rw-r--r--   0        0        0      162 2024-04-02 08:36:55.886153 ftrack_framework_core-2.1.0/source/ftrack_framework_core/exceptions/__init__.py
+-rw-r--r--   0        0        0      277 2024-04-02 08:36:55.886153 ftrack_framework_core-2.1.0/source/ftrack_framework_core/exceptions/engine.py
+-rw-r--r--   0        0        0     1501 2024-04-02 08:36:55.886153 ftrack_framework_core-2.1.0/source/ftrack_framework_core/exceptions/plugin.py
+-rw-r--r--   0        0        0    12705 2024-04-02 08:36:55.886153 ftrack_framework_core-2.1.0/source/ftrack_framework_core/host/__init__.py
+-rw-r--r--   0        0        0     8625 2024-04-02 08:36:55.886153 ftrack_framework_core-2.1.0/source/ftrack_framework_core/log/__init__.py
+-rw-r--r--   0        0        0     1184 2024-04-02 08:36:55.886153 ftrack_framework_core-2.1.0/source/ftrack_framework_core/log/log_item.py
+-rw-r--r--   0        0        0     1831 2024-04-02 08:36:55.886153 ftrack_framework_core-2.1.0/source/ftrack_framework_core/plugin/__init__.py
+-rw-r--r--   0        0        0     1975 2024-04-02 08:36:55.886153 ftrack_framework_core-2.1.0/source/ftrack_framework_core/plugin/plugin_info.py
+-rw-r--r--   0        0        0     7987 2024-04-02 08:36:55.886153 ftrack_framework_core-2.1.0/source/ftrack_framework_core/registry/__init__.py
+-rw-r--r--   0        0        0     3437 2024-04-02 08:36:55.886153 ftrack_framework_core-2.1.0/source/ftrack_framework_core/widget/__init__.py
+-rw-r--r--   0        0        0    17207 2024-04-02 08:36:55.886153 ftrack_framework_core-2.1.0/source/ftrack_framework_core/widget/dialog.py
+-rw-r--r--   0        0        0     4475 2024-04-02 08:36:55.886153 ftrack_framework_core-2.1.0/source/ftrack_framework_core/widget/widget.py
+-rw-r--r--   0        0        0     1268 1970-01-01 00:00:00.000000 ftrack_framework_core-2.1.0/PKG-INFO
```

### Comparing `ftrack_framework_core-2.0.1/LICENSE.txt` & `ftrack_framework_core-2.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ftrack_framework_core-2.0.1/pyproject.toml` & `ftrack_framework_core-2.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ftrack-framework-core"
-version = "2.0.1"
+version = "2.1.0"
 description='ftrack Framework Core library'
 authors = ["ftrack Integrations Team <integrations@backlight.co>"]
 readme = "README.md"
 packages = [{include = "ftrack_framework_core", from = "source"}]
 license = "Apache-2.0"
 homepage = "https://ftrack.com"
 repository = "https://github.com/ftrackhq/integrations/tree/main/libs/framework-core"
```

### Comparing `ftrack_framework_core-2.0.1/source/ftrack_framework_core/__init__.py` & `ftrack_framework_core-2.1.0/source/ftrack_framework_core/__init__.py`

 * *Files identical despite different names*

### Comparing `ftrack_framework_core-2.0.1/source/ftrack_framework_core/asset/__init__.py` & `ftrack_framework_core-2.1.0/source/ftrack_framework_core/asset/__init__.py`

 * *Files identical despite different names*

### Comparing `ftrack_framework_core-2.0.1/source/ftrack_framework_core/asset/asset_info.py` & `ftrack_framework_core-2.1.0/source/ftrack_framework_core/asset/asset_info.py`

 * *Files identical despite different names*

### Comparing `ftrack_framework_core-2.0.1/source/ftrack_framework_core/asset/dcc_object.py` & `ftrack_framework_core-2.1.0/source/ftrack_framework_core/asset/dcc_object.py`

 * *Files identical despite different names*

### Comparing `ftrack_framework_core-2.0.1/source/ftrack_framework_core/client/__init__.py` & `ftrack_framework_core-2.1.0/source/ftrack_framework_core/client/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -337,15 +337,15 @@
         '''
         self.host_connection.reset_all_tool_configs()
 
     # UI
     @track_framework_usage(
         'FRAMEWORK_RUN_DIALOG',
         {'module': 'client'},
-        ['dialog_name', 'dialog_options', 'dock_func'],
+        ['dialog_name', 'dialog_options'],
     )
     def run_dialog(
         self,
         dialog_name,
         dialog_class=None,
         dialog_options=None,
         dock_func=None,
@@ -410,15 +410,15 @@
             connect_getter_property_callback=self._connect_getter_property_callback,
             dialog_options=dialog_options,
         )
         # Append dialog to dialogs
         self._register_dialog(dialog)
         self.dialog = dialog
         # If a docking function is provided, use it
-        if dock_func:
+        if dialog_options.get('docked') and dock_func:
             dock_func(self.dialog)
         else:
             self.dialog.show_ui()
             self.dialog.setFocus()
 
     def _register_dialog(self, dialog):
         '''Register the given initialized *dialog* to the dialogs registry'''
```

### Comparing `ftrack_framework_core-2.0.1/source/ftrack_framework_core/client/host_connection.py` & `ftrack_framework_core-2.1.0/source/ftrack_framework_core/client/host_connection.py`

 * *Files identical despite different names*

### Comparing `ftrack_framework_core-2.0.1/source/ftrack_framework_core/configure_logging.py` & `ftrack_framework_core-2.1.0/source/ftrack_framework_core/configure_logging.py`

 * *Files identical despite different names*

### Comparing `ftrack_framework_core-2.0.1/source/ftrack_framework_core/engine/__init__.py` & `ftrack_framework_core-2.1.0/source/ftrack_framework_core/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `ftrack_framework_core-2.0.1/source/ftrack_framework_core/event/__init__.py` & `ftrack_framework_core-2.1.0/source/ftrack_framework_core/event/__init__.py`

 * *Files identical despite different names*

### Comparing `ftrack_framework_core-2.0.1/source/ftrack_framework_core/exceptions/plugin.py` & `ftrack_framework_core-2.1.0/source/ftrack_framework_core/exceptions/plugin.py`

 * *Files identical despite different names*

### Comparing `ftrack_framework_core-2.0.1/source/ftrack_framework_core/host/__init__.py` & `ftrack_framework_core-2.1.0/source/ftrack_framework_core/host/__init__.py`

 * *Files identical despite different names*

### Comparing `ftrack_framework_core-2.0.1/source/ftrack_framework_core/log/__init__.py` & `ftrack_framework_core-2.1.0/source/ftrack_framework_core/log/__init__.py`

 * *Files identical despite different names*

### Comparing `ftrack_framework_core-2.0.1/source/ftrack_framework_core/log/log_item.py` & `ftrack_framework_core-2.1.0/source/ftrack_framework_core/log/log_item.py`

 * *Files identical despite different names*

### Comparing `ftrack_framework_core-2.0.1/source/ftrack_framework_core/plugin/__init__.py` & `ftrack_framework_core-2.1.0/source/ftrack_framework_core/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `ftrack_framework_core-2.0.1/source/ftrack_framework_core/plugin/plugin_info.py` & `ftrack_framework_core-2.1.0/source/ftrack_framework_core/plugin/plugin_info.py`

 * *Files identical despite different names*

### Comparing `ftrack_framework_core-2.0.1/source/ftrack_framework_core/registry/__init__.py` & `ftrack_framework_core-2.1.0/source/ftrack_framework_core/registry/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 # :coding: utf-8
 # :copyright: Copyright (c) 2024 ftrack
+import os.path
 import uuid
+import pkgutil
+import inspect
 
 import logging
 from collections import defaultdict
 
-from ftrack_utils.extensions import registry
+from ftrack_utils.extensions import registry, overrides
 
 logger = logging.getLogger(__name__)
 
 
 class Registry(object):
     @property
     def schemas(self):
@@ -50,19 +53,19 @@
     def dialogs(self):
         '''
         Returns the registered engines`
         '''
         return self.__registry.get('dialog')
 
     @property
-    def launchers(self):
+    def launch_configs(self):
         '''
         Returns the registered launcher configs`
         '''
-        return self.__registry.get('launcher')
+        return self.__registry.get('launch_config')
 
     @property
     def dcc_configs(self):
         '''
         Returns the registered dcc configs`
         '''
         return self.__registry.get('dcc_config')
@@ -87,24 +90,33 @@
 
         self.logger.debug('Initializing Registry {}'.format(self))
 
         # Reset all registries
         self.__registry = defaultdict(list)
 
     # Register
-    def scan_extensions(self, paths):
+    def scan_extensions(self, paths, extension_types=None):
         '''
-        Scan framework extension modules from the given *paths*
+        Scan framework extension modules from the given *paths*. If *extension_types*
+        is given, only consider the given extension types.
         '''
 
         discovered_extensions = []
-        for path in paths:
-            discovered_extensions.extend(
-                registry.get_extensions_from_directory(path)
+        for path in reversed(paths):
+            logging.debug(
+                f'Scanning {path} for {f"{extension_types} " if extension_types else ""}extensions'
             )
+            dir_extensions = registry.get_extensions_from_directory(
+                path, extension_types=extension_types
+            )
+            # Merge/override
+            unique_extensions = overrides.set_overrides(
+                discovered_extensions, dir_extensions
+            )
+
         for extension in discovered_extensions:
             self.add(**extension)
 
     def add(self, extension_type, name, extension, path):
         '''
         Add the given *extension_type* with *name*, *extension* and *path to
         the registry
@@ -184,15 +196,16 @@
 
     def augment_tool_config(self, tool_config):
         '''
         Augment the given *tool_config* to add a reference id to it
         and each plugin and group
         '''
         tool_config['reference'] = uuid.uuid4().hex
-        self._recursive_create_reference(tool_config.get('engine'))
+        if 'engine' in tool_config:
+            self._recursive_create_reference(tool_config['engine'])
         return tool_config
 
     def _recursive_create_reference(self, tool_config_engine_portion):
         '''
         Recursive method to add reference number to each plugin and group of the
         given engine portion of a tool_config.
         '''
```

### Comparing `ftrack_framework_core-2.0.1/source/ftrack_framework_core/widget/__init__.py` & `ftrack_framework_core-2.1.0/source/ftrack_framework_core/widget/__init__.py`

 * *Files identical despite different names*

### Comparing `ftrack_framework_core-2.0.1/source/ftrack_framework_core/widget/dialog.py` & `ftrack_framework_core-2.1.0/source/ftrack_framework_core/widget/dialog.py`

 * *Files identical despite different names*

### Comparing `ftrack_framework_core-2.0.1/source/ftrack_framework_core/widget/widget.py` & `ftrack_framework_core-2.1.0/source/ftrack_framework_core/widget/widget.py`

 * *Files identical despite different names*

### Comparing `ftrack_framework_core-2.0.1/PKG-INFO` & `ftrack_framework_core-2.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ftrack-framework-core
-Version: 2.0.1
+Version: 2.1.0
 Summary: ftrack Framework Core library
 Home-page: https://ftrack.com
 License: Apache-2.0
 Author: ftrack Integrations Team
 Author-email: integrations@backlight.co
 Requires-Python: >=3.7,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
@@ -23,8 +23,9 @@
 Requires-Dist: six (>=1,<2)
 Project-URL: Repository, https://github.com/ftrackhq/integrations/tree/main/libs/framework-core
 Description-Content-Type: text/markdown
 
 # Framework Core
 
 This is the ftrack integrations framework-core library.
+Client, Host, Registry, extensions bases and all the base code for the framework should be found here.
```

