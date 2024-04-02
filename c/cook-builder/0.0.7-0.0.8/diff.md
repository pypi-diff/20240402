# Comparing `tmp/cook_builder-0.0.7.tar.gz` & `tmp/cook_builder-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cook_builder-0.0.7.tar", last modified: Thu Mar 14 17:56:50 2024, max compression
+gzip compressed data, was "cook_builder-0.0.8.tar", last modified: Tue Apr  2 18:51:15 2024, max compression
```

## Comparing `cook_builder-0.0.7.tar` & `cook_builder-0.0.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 seweryn   (1000) seweryn   (1000)        0 2024-03-14 17:56:50.745086 cook_builder-0.0.7/
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1072 2024-02-10 12:14:36.000000 cook_builder-0.0.7/LICENSE
--rw-r--r--   0 seweryn   (1000) seweryn   (1000)     2664 2024-03-14 17:56:50.745086 cook_builder-0.0.7/PKG-INFO
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      534 2024-03-10 11:58:42.000000 cook_builder-0.0.7/README.md
-drwxrwxr-x   0 seweryn   (1000) seweryn   (1000)        0 2024-03-14 17:56:50.745086 cook_builder-0.0.7/cook/
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)        0 2024-02-10 12:15:45.000000 cook_builder-0.0.7/cook/__init__.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      672 2024-03-13 18:33:30.000000 cook_builder-0.0.7/cook/cli.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     5574 2024-03-12 20:40:38.000000 cook_builder-0.0.7/cook/configuration.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     3498 2024-03-13 19:03:20.000000 cook_builder-0.0.7/cook/cook.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      369 2024-03-13 19:09:39.000000 cook_builder-0.0.7/cook/logger.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1205 2024-03-13 18:44:51.000000 cook_builder-0.0.7/cook/receipe.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      936 2024-03-09 09:22:10.000000 cook_builder-0.0.7/cook/rsync.py
-drwxrwxr-x   0 seweryn   (1000) seweryn   (1000)        0 2024-03-14 17:56:50.745086 cook_builder-0.0.7/cook_builder.egg-info/
--rw-r--r--   0 seweryn   (1000) seweryn   (1000)     2664 2024-03-14 17:56:50.000000 cook_builder-0.0.7/cook_builder.egg-info/PKG-INFO
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      359 2024-03-14 17:56:50.000000 cook_builder-0.0.7/cook_builder.egg-info/SOURCES.txt
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)        1 2024-03-14 17:56:50.000000 cook_builder-0.0.7/cook_builder.egg-info/dependency_links.txt
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)       39 2024-03-14 17:56:50.000000 cook_builder-0.0.7/cook_builder.egg-info/entry_points.txt
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)       27 2024-03-14 17:56:50.000000 cook_builder-0.0.7/cook_builder.egg-info/requires.txt
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)        5 2024-03-14 17:56:50.000000 cook_builder-0.0.7/cook_builder.egg-info/top_level.txt
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      983 2024-03-14 17:54:01.000000 cook_builder-0.0.7/pyproject.toml
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)       38 2024-03-14 17:56:50.745086 cook_builder-0.0.7/setup.cfg
+drwxrwxr-x   0 seweryn   (1000) seweryn   (1000)        0 2024-04-02 18:51:15.142826 cook_builder-0.0.8/
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1072 2024-02-10 12:14:36.000000 cook_builder-0.0.8/LICENSE
+-rw-r--r--   0 seweryn   (1000) seweryn   (1000)     2662 2024-04-02 18:51:15.142826 cook_builder-0.0.8/PKG-INFO
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      532 2024-04-02 18:20:44.000000 cook_builder-0.0.8/README.md
+drwxrwxr-x   0 seweryn   (1000) seweryn   (1000)        0 2024-04-02 18:51:15.142826 cook_builder-0.0.8/cook/
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)        0 2024-02-10 12:15:45.000000 cook_builder-0.0.8/cook/__init__.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1211 2024-04-02 18:37:31.000000 cook_builder-0.0.8/cook/cli.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     5742 2024-04-02 18:20:44.000000 cook_builder-0.0.8/cook/configuration.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     3491 2024-04-02 18:20:52.000000 cook_builder-0.0.8/cook/cook.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      369 2024-03-13 19:09:39.000000 cook_builder-0.0.8/cook/logger.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1342 2024-04-02 18:46:13.000000 cook_builder-0.0.8/cook/recipe.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      936 2024-03-09 09:22:10.000000 cook_builder-0.0.8/cook/rsync.py
+drwxrwxr-x   0 seweryn   (1000) seweryn   (1000)        0 2024-04-02 18:51:15.142826 cook_builder-0.0.8/cook_builder.egg-info/
+-rw-r--r--   0 seweryn   (1000) seweryn   (1000)     2662 2024-04-02 18:51:15.000000 cook_builder-0.0.8/cook_builder.egg-info/PKG-INFO
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      358 2024-04-02 18:51:15.000000 cook_builder-0.0.8/cook_builder.egg-info/SOURCES.txt
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)        1 2024-04-02 18:51:15.000000 cook_builder-0.0.8/cook_builder.egg-info/dependency_links.txt
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)       39 2024-04-02 18:51:15.000000 cook_builder-0.0.8/cook_builder.egg-info/entry_points.txt
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)       27 2024-04-02 18:51:15.000000 cook_builder-0.0.8/cook_builder.egg-info/requires.txt
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)        5 2024-04-02 18:51:15.000000 cook_builder-0.0.8/cook_builder.egg-info/top_level.txt
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      983 2024-04-02 18:50:59.000000 cook_builder-0.0.8/pyproject.toml
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)       38 2024-04-02 18:51:15.142826 cook_builder-0.0.8/setup.cfg
```

### Comparing `cook_builder-0.0.7/LICENSE` & `cook_builder-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cook_builder-0.0.7/PKG-INFO` & `cook_builder-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cook_builder
-Version: 0.0.7
+Version: 0.0.8
 Summary: Build script aggregator and remote executor
 Author: Seweryn Rusecki
 License: MIT License
         
         Copyright (c) 2024 Seweryn Rusecki
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -61,14 +61,14 @@
 git clone https://github.com/serweryn617/cook.git
 cd cook
 pip install .
 ```
 
 ### Setup
 
-Create `receipe.py` file which describes how to build Your project and lists the available remote build servers.
+Create `recipe.py` file which describes how to build Your project and lists the available remote build servers.
 
 See the [example project](example).
 
 ### Run
 
-Run `cook` command in the directory where the `receipe.py` file is located and see how the project is being built!
+Run `cook` command in the directory where the `recipe.py` file is located and see how the project is being built!
```

### Comparing `cook_builder-0.0.7/README.md` & `cook_builder-0.0.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,14 @@
 git clone https://github.com/serweryn617/cook.git
 cd cook
 pip install .
 ```
 
 ### Setup
 
-Create `receipe.py` file which describes how to build Your project and lists the available remote build servers.
+Create `recipe.py` file which describes how to build Your project and lists the available remote build servers.
 
 See the [example project](example).
 
 ### Run
 
-Run `cook` command in the directory where the `receipe.py` file is located and see how the project is being built!
+Run `cook` command in the directory where the `recipe.py` file is located and see how the project is being built!
```

### Comparing `cook_builder-0.0.7/cook/configuration.py` & `cook_builder-0.0.8/cook/configuration.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 class BuildType(Enum):
     LOCAL = auto()
     REMOTE = auto()
     COMPOSITE = auto()
 
 
 class Configuration:
-    def __init__(self, receipe):
-        self.projects = receipe.projects
+    def __init__(self, recipe):
+        self.projects = recipe.projects
 
-        self.default_project = receipe.default_project
-        self.default_build_server = receipe.default_build_server
+        self.default_project = recipe.default_project
+        self.default_build_server = recipe.default_build_server
 
-        self.base_path = receipe.base_path
+        self.base_path = recipe.base_path
         self.skip = False
 
     def setup(self, project, server):
         if project is None:
             project = self.default_project
         self._set_project(project)
         self._update_local_path()
@@ -83,19 +83,26 @@
                 self.local_path = self.base_path / local_path
 
     def _get_build_server_override(self):
         build_servers = self._get_nested_item(self.projects, self.project, 'build_servers')
         if build_servers is None:
             return None
 
+        overrides = []
         for server_name, config in build_servers.items():
             override = self._get_nested_item(config, 'override')
             if override == True:
-                # TODO: Detect multiple overrides
-                return server_name
+                overrides.append(server_name)
+
+        if len(overrides) > 1:
+            logger.error(f"Multiple server overrides defined for {self.project}")
+            exit(1)
+
+        if overrides:
+            return overrides[0]
 
     def _is_composite(self):
         is_composite = 'components' in self.projects[self.project]
         return is_composite
 
     def _is_local(self):
         is_local = self.build_server == 'local'
```

### Comparing `cook_builder-0.0.7/cook/cook.py` & `cook_builder-0.0.8/cook/cook.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import fabric
 import subprocess
 
 from .rsync import Rsync
-from .receipe import Receipe
+from .recipe import Recipe
 from .configuration import Configuration, BuildType
 from cook import logger
 
 
 class Cook:
-    def __init__(self, receipe, configuration):
-        self.receipe = receipe
+    def __init__(self, recipe, configuration):
+        self.recipe = recipe
         self.configuration = configuration
 
     def cook(self):
         build_type = self.configuration.get_build_type()
 
         if build_type == BuildType.LOCAL:
             self._local_build()
@@ -89,14 +89,14 @@
             return
 
         logger.local('Executing Components')
 
         for component in components:
             logger.local(f'Component: {component}')
 
-            sub_configuration = Configuration(self.receipe)
+            sub_configuration = Configuration(self.recipe)
 
             build_server = self.configuration.get_build_server()
             sub_configuration.setup(component, build_server)
 
-            sub_cook = Cook(self.receipe, sub_configuration)
+            sub_cook = Cook(self.recipe, sub_configuration)
             sub_cook.cook()
```

### Comparing `cook_builder-0.0.7/cook/receipe.py` & `cook_builder-0.0.8/cook/recipe.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 import importlib.util
 import sys
 from pathlib import Path
 from cook import logger
 
 
-class Receipe:
-    def __init__(self, base_path: Path):
+class Recipe:
+    def __init__(self, base_path: Path, user_args: dict):
         self.base_path = base_path
+        self.user_args = user_args
 
         self.projects = None
 
         self.default_project = None
         self.default_build_server = 'local'
 
     def load(self):
-        receipes = list(self.base_path.glob('receipe.py'))
+        recipes = list(self.base_path.glob('recipe.py'))
 
-        if len(receipes) == 0:
-            logger.error(f'Receipe file not found in {self.base_path}')
+        if len(recipes) == 0:
+            logger.error(f'Recipe file not found in {self.base_path}')
             exit(1)
 
-        receipe_file_path = str(receipes[0])
-        module_name = 'receipe'
+        recipe_file_path = str(recipes[0])
+        module_name = 'recipe'
 
-        spec = importlib.util.spec_from_file_location(module_name, receipe_file_path)
-        receipe = importlib.util.module_from_spec(spec)
-        sys.modules[module_name] = receipe
-        spec.loader.exec_module(receipe)
+        spec = importlib.util.spec_from_file_location(module_name, recipe_file_path)
+        recipe = importlib.util.module_from_spec(spec)
+        sys.modules[module_name] = recipe
+        recipe.user_args = self.user_args  # Inject user_args to receipe.py before executing the module
+        spec.loader.exec_module(recipe)
 
-        if hasattr(receipe, 'projects'):
-            self.projects = receipe.projects
+        if hasattr(recipe, 'projects'):
+            self.projects = recipe.projects
         else:
-            logger.error('No projects found in receipe.')
+            logger.error('No projects found in recipe.')
             exit(1)
 
-        if hasattr(receipe, 'default_project'):
-            self.default_project = receipe.default_project
+        if hasattr(recipe, 'default_project'):
+            self.default_project = recipe.default_project
 
-        if hasattr(receipe, 'default_build_server'):
-            self.default_build_server = receipe.default_build_server
+        if hasattr(recipe, 'default_build_server'):
+            self.default_build_server = recipe.default_build_server
```

### Comparing `cook_builder-0.0.7/cook/rsync.py` & `cook_builder-0.0.8/cook/rsync.py`

 * *Files identical despite different names*

### Comparing `cook_builder-0.0.7/cook_builder.egg-info/PKG-INFO` & `cook_builder-0.0.8/cook_builder.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cook_builder
-Version: 0.0.7
+Version: 0.0.8
 Summary: Build script aggregator and remote executor
 Author: Seweryn Rusecki
 License: MIT License
         
         Copyright (c) 2024 Seweryn Rusecki
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -61,14 +61,14 @@
 git clone https://github.com/serweryn617/cook.git
 cd cook
 pip install .
 ```
 
 ### Setup
 
-Create `receipe.py` file which describes how to build Your project and lists the available remote build servers.
+Create `recipe.py` file which describes how to build Your project and lists the available remote build servers.
 
 See the [example project](example).
 
 ### Run
 
-Run `cook` command in the directory where the `receipe.py` file is located and see how the project is being built!
+Run `cook` command in the directory where the `recipe.py` file is located and see how the project is being built!
```

### Comparing `cook_builder-0.0.7/pyproject.toml` & `cook_builder-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cook_builder"
-version = "0.0.7"
+version = "0.0.8"
 dependencies = [
   "fabric==3.2.2",
   "rich==13.7.1",
 ]
 requires-python = ">=3.10"
 authors = [
   { name="Seweryn Rusecki" },
```

