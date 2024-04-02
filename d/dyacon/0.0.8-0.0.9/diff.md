# Comparing `tmp/dyacon-0.0.8.tar.gz` & `tmp/dyacon-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dyacon-0.0.8.tar", last modified: Sun Nov  5 15:55:27 2023, max compression
+gzip compressed data, was "dyacon-0.0.9.tar", last modified: Thu Nov  9 10:47:45 2023, max compression
```

## Comparing `dyacon-0.0.8.tar` & `dyacon-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-05 15:55:27.528172 dyacon-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2023-11-05 15:54:57.000000 dyacon-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7763 2023-11-05 15:55:27.528172 dyacon-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7082 2023-11-05 15:54:57.000000 dyacon-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      722 2023-11-05 15:54:57.000000 dyacon-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-05 15:55:27.528172 dyacon-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-05 15:55:27.524172 dyacon-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-05 15:55:27.524172 dyacon-0.0.8/src/dyacon/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2023-11-05 15:54:57.000000 dyacon-0.0.8/src/dyacon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-05 15:55:27.524172 dyacon-0.0.8/src/dyacon/loaders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-05 15:54:57.000000 dyacon-0.0.8/src/dyacon/loaders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-05 15:55:27.524172 dyacon-0.0.8/src/dyacon/loaders/external/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2023-11-05 15:54:57.000000 dyacon-0.0.8/src/dyacon/loaders/external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2964 2023-11-05 15:54:57.000000 dyacon-0.0.8/src/dyacon/loaders/external/google.py
--rw-r--r--   0 runner    (1001) docker     (127)     3622 2023-11-05 15:54:57.000000 dyacon-0.0.8/src/dyacon/loaders/loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2023-11-05 15:54:57.000000 dyacon-0.0.8/src/dyacon/read.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-05 15:55:27.524172 dyacon-0.0.8/src/dyacon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7763 2023-11-05 15:55:27.000000 dyacon-0.0.8/src/dyacon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      423 2023-11-05 15:55:27.000000 dyacon-0.0.8/src/dyacon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-05 15:55:27.000000 dyacon-0.0.8/src/dyacon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       88 2023-11-05 15:55:27.000000 dyacon-0.0.8/src/dyacon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-11-05 15:55:27.000000 dyacon-0.0.8/src/dyacon.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-05 15:55:27.528172 dyacon-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3313 2023-11-05 15:54:57.000000 dyacon-0.0.8/tests/test_loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)     2656 2023-11-05 15:54:57.000000 dyacon-0.0.8/tests/test_read.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 10:47:45.593863 dyacon-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2023-11-09 10:47:24.000000 dyacon-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7763 2023-11-09 10:47:45.593863 dyacon-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7082 2023-11-09 10:47:24.000000 dyacon-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2023-11-09 10:47:24.000000 dyacon-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-09 10:47:45.593863 dyacon-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 10:47:45.589863 dyacon-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 10:47:45.589863 dyacon-0.0.9/src/dyacon/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2023-11-09 10:47:24.000000 dyacon-0.0.9/src/dyacon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 10:47:45.593863 dyacon-0.0.9/src/dyacon/loaders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 10:47:24.000000 dyacon-0.0.9/src/dyacon/loaders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 10:47:45.593863 dyacon-0.0.9/src/dyacon/loaders/external/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2023-11-09 10:47:24.000000 dyacon-0.0.9/src/dyacon/loaders/external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2964 2023-11-09 10:47:24.000000 dyacon-0.0.9/src/dyacon/loaders/external/google.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3622 2023-11-09 10:47:24.000000 dyacon-0.0.9/src/dyacon/loaders/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2023-11-09 10:47:24.000000 dyacon-0.0.9/src/dyacon/read.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 10:47:45.589863 dyacon-0.0.9/src/dyacon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7763 2023-11-09 10:47:45.000000 dyacon-0.0.9/src/dyacon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2023-11-09 10:47:45.000000 dyacon-0.0.9/src/dyacon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-09 10:47:45.000000 dyacon-0.0.9/src/dyacon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2023-11-09 10:47:45.000000 dyacon-0.0.9/src/dyacon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2023-11-09 10:47:45.000000 dyacon-0.0.9/src/dyacon.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 10:47:45.593863 dyacon-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3313 2023-11-09 10:47:24.000000 dyacon-0.0.9/tests/test_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2023-11-09 10:47:24.000000 dyacon-0.0.9/tests/test_read.py
```

### Comparing `dyacon-0.0.8/LICENSE` & `dyacon-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dyacon-0.0.8/PKG-INFO` & `dyacon-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyacon
-Version: 0.0.8
+Version: 0.0.9
 Summary: Yaml config package
 Author-email: Aleksei Morozov <morozov6420@gmail.com>
 Project-URL: Homepage, https://github.com/morozov6420/dyacon
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `dyacon-0.0.8/README.md` & `dyacon-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `dyacon-0.0.8/pyproject.toml` & `dyacon-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dyacon"
-version = "0.0.8"
+version = "0.0.9"
 authors = [{ name = "Aleksei Morozov", email = "morozov6420@gmail.com" }]
 description = "Yaml config package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `dyacon-0.0.8/src/dyacon/loaders/external/google.py` & `dyacon-0.0.9/src/dyacon/loaders/external/google.py`

 * *Files identical despite different names*

### Comparing `dyacon-0.0.8/src/dyacon/loaders/loaders.py` & `dyacon-0.0.9/src/dyacon/loaders/loaders.py`

 * *Files identical despite different names*

### Comparing `dyacon-0.0.8/src/dyacon/read.py` & `dyacon-0.0.9/src/dyacon/read.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,30 +13,30 @@
     dataclass_instance = dataclass_from_dict(klass, config_dict)
     return dataclass_instance
 
 
 def read_yaml_to_dict(path: str = 'config/config.yaml') -> Dict:
     # TODO: add exception or warning for non-dict structures?
     config_abs_path = find_dotenv(path)
-    if not config_abs_path:
-        raise ValueError('Config yaml file not found')
+    if not config_abs_path and not os.path.isfile(path):
+        raise ValueError(f'Config yaml file not found on path: {path}')
 
     class Loader(yaml.SafeLoader):
         def __init__(self, stream):
             self._root = os.path.split(stream.name)[0]
             super().__init__(stream)
 
         def include(self, node):
             filename = os.path.join(self._root, self.construct_scalar(node))
             with open(filename, 'r') as file:
                 return yaml.load(file, Loader)
 
     Loader.add_constructor('!include', Loader.include)
 
-    with open(config_abs_path, 'r') as f:
+    with open(config_abs_path or path, 'r') as f:
         config_dict: Dict = yaml.load(f, Loader=Loader)
     return config_dict
 
 
 def dataclass_from_dict(klass: Type[T], d: Dict) -> T:
     # TODO: add exceptions or warnings for container types&
     #  they work, but descriptor loaders.loaders.Load() is not working for
```

### Comparing `dyacon-0.0.8/src/dyacon.egg-info/PKG-INFO` & `dyacon-0.0.9/src/dyacon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyacon
-Version: 0.0.8
+Version: 0.0.9
 Summary: Yaml config package
 Author-email: Aleksei Morozov <morozov6420@gmail.com>
 Project-URL: Homepage, https://github.com/morozov6420/dyacon
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `dyacon-0.0.8/tests/test_loaders.py` & `dyacon-0.0.9/tests/test_loaders.py`

 * *Files identical despite different names*

### Comparing `dyacon-0.0.8/tests/test_read.py` & `dyacon-0.0.9/tests/test_read.py`

 * *Files identical despite different names*

