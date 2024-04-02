# Comparing `tmp/fastapi-di-extension-0.0.2.tar.gz` & `tmp/fastapi-di-extension-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-di-extension-0.0.2.tar", last modified: Fri Mar 29 12:35:23 2024, max compression
+gzip compressed data, was "fastapi-di-extension-0.0.3.tar", last modified: Tue Apr  2 03:03:40 2024, max compression
```

## Comparing `fastapi-di-extension-0.0.2.tar` & `fastapi-di-extension-0.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 alim      (1000) alim      (1000)        0 2024-03-29 12:35:23.138420 fastapi-di-extension-0.0.2/
--rw-rw-r--   0 alim      (1000) alim      (1000)     1074 2024-03-28 03:34:37.000000 fastapi-di-extension-0.0.2/LICENSE
--rw-r--r--   0 alim      (1000) alim      (1000)     1357 2024-03-29 12:35:23.138420 fastapi-di-extension-0.0.2/PKG-INFO
--rw-rw-r--   0 alim      (1000) alim      (1000)      132 2024-03-29 12:24:14.000000 fastapi-di-extension-0.0.2/README.md
--rw-rw-r--   0 alim      (1000) alim      (1000)     1320 2024-03-29 12:24:26.000000 fastapi-di-extension-0.0.2/pyproject.toml
--rw-rw-r--   0 alim      (1000) alim      (1000)       38 2024-03-29 12:35:23.138420 fastapi-di-extension-0.0.2/setup.cfg
-drwxrwxr-x   0 alim      (1000) alim      (1000)        0 2024-03-29 12:35:23.134420 fastapi-di-extension-0.0.2/src/
-drwxrwxr-x   0 alim      (1000) alim      (1000)        0 2024-03-29 12:35:23.134420 fastapi-di-extension-0.0.2/src/fast_di/
--rw-rw-r--   0 alim      (1000) alim      (1000)      350 2024-03-29 12:35:18.000000 fastapi-di-extension-0.0.2/src/fast_di/__init__.py
-drwxrwxr-x   0 alim      (1000) alim      (1000)        0 2024-03-29 12:35:23.134420 fastapi-di-extension-0.0.2/src/fast_di/collector/
--rw-rw-r--   0 alim      (1000) alim      (1000)        0 2024-03-28 00:10:02.000000 fastapi-di-extension-0.0.2/src/fast_di/collector/__init__.py
--rw-rw-r--   0 alim      (1000) alim      (1000)     1354 2024-03-28 00:21:33.000000 fastapi-di-extension-0.0.2/src/fast_di/collector/base.py
--rw-rw-r--   0 alim      (1000) alim      (1000)      686 2024-03-28 04:44:43.000000 fastapi-di-extension-0.0.2/src/fast_di/collector/collector.py
-drwxrwxr-x   0 alim      (1000) alim      (1000)        0 2024-03-29 12:35:23.134420 fastapi-di-extension-0.0.2/src/fast_di/depends/
--rw-rw-r--   0 alim      (1000) alim      (1000)        0 2024-03-28 00:10:21.000000 fastapi-di-extension-0.0.2/src/fast_di/depends/__init__.py
--rw-rw-r--   0 alim      (1000) alim      (1000)      246 2024-03-28 00:32:14.000000 fastapi-di-extension-0.0.2/src/fast_di/depends/depends.py
--rw-rw-r--   0 alim      (1000) alim      (1000)     1040 2024-03-28 04:43:17.000000 fastapi-di-extension-0.0.2/src/fast_di/depends/depends_stub.py
--rw-rw-r--   0 alim      (1000) alim      (1000)      396 2024-03-28 04:44:22.000000 fastapi-di-extension-0.0.2/src/fast_di/init_dependencies.py
-drwxrwxr-x   0 alim      (1000) alim      (1000)        0 2024-03-29 12:35:23.134420 fastapi-di-extension-0.0.2/src/fastapi_di_extension.egg-info/
--rw-r--r--   0 alim      (1000) alim      (1000)     1357 2024-03-29 12:35:23.000000 fastapi-di-extension-0.0.2/src/fastapi_di_extension.egg-info/PKG-INFO
--rw-rw-r--   0 alim      (1000) alim      (1000)      526 2024-03-29 12:35:23.000000 fastapi-di-extension-0.0.2/src/fastapi_di_extension.egg-info/SOURCES.txt
--rw-rw-r--   0 alim      (1000) alim      (1000)        1 2024-03-29 12:35:23.000000 fastapi-di-extension-0.0.2/src/fastapi_di_extension.egg-info/dependency_links.txt
--rw-rw-r--   0 alim      (1000) alim      (1000)      182 2024-03-29 12:35:23.000000 fastapi-di-extension-0.0.2/src/fastapi_di_extension.egg-info/requires.txt
--rw-rw-r--   0 alim      (1000) alim      (1000)        8 2024-03-29 12:35:23.000000 fastapi-di-extension-0.0.2/src/fastapi_di_extension.egg-info/top_level.txt
+drwxrwxr-x   0 alim      (1000) alim      (1000)        0 2024-04-02 03:03:40.472175 fastapi-di-extension-0.0.3/
+-rw-rw-r--   0 alim      (1000) alim      (1000)     1074 2024-03-28 03:34:37.000000 fastapi-di-extension-0.0.3/LICENSE
+-rw-r--r--   0 alim      (1000) alim      (1000)     1357 2024-04-02 03:03:40.468175 fastapi-di-extension-0.0.3/PKG-INFO
+-rw-rw-r--   0 alim      (1000) alim      (1000)      132 2024-03-29 12:24:14.000000 fastapi-di-extension-0.0.3/README.md
+-rw-rw-r--   0 alim      (1000) alim      (1000)     1320 2024-04-02 03:03:12.000000 fastapi-di-extension-0.0.3/pyproject.toml
+-rw-rw-r--   0 alim      (1000) alim      (1000)       38 2024-04-02 03:03:40.472175 fastapi-di-extension-0.0.3/setup.cfg
+drwxrwxr-x   0 alim      (1000) alim      (1000)        0 2024-04-02 03:03:40.464175 fastapi-di-extension-0.0.3/src/
+drwxrwxr-x   0 alim      (1000) alim      (1000)        0 2024-04-02 03:03:40.468175 fastapi-di-extension-0.0.3/src/fast_di/
+-rw-rw-r--   0 alim      (1000) alim      (1000)      350 2024-04-02 03:03:04.000000 fastapi-di-extension-0.0.3/src/fast_di/__init__.py
+drwxrwxr-x   0 alim      (1000) alim      (1000)        0 2024-04-02 03:03:40.468175 fastapi-di-extension-0.0.3/src/fast_di/collector/
+-rw-rw-r--   0 alim      (1000) alim      (1000)        0 2024-03-28 00:10:02.000000 fastapi-di-extension-0.0.3/src/fast_di/collector/__init__.py
+-rw-rw-r--   0 alim      (1000) alim      (1000)     1354 2024-03-28 00:21:33.000000 fastapi-di-extension-0.0.3/src/fast_di/collector/base.py
+-rw-rw-r--   0 alim      (1000) alim      (1000)      626 2024-03-29 16:28:32.000000 fastapi-di-extension-0.0.3/src/fast_di/collector/collector.py
+drwxrwxr-x   0 alim      (1000) alim      (1000)        0 2024-04-02 03:03:40.468175 fastapi-di-extension-0.0.3/src/fast_di/depends/
+-rw-rw-r--   0 alim      (1000) alim      (1000)        0 2024-03-28 00:10:21.000000 fastapi-di-extension-0.0.3/src/fast_di/depends/__init__.py
+-rw-rw-r--   0 alim      (1000) alim      (1000)      246 2024-03-28 00:32:14.000000 fastapi-di-extension-0.0.3/src/fast_di/depends/depends.py
+-rw-rw-r--   0 alim      (1000) alim      (1000)     1040 2024-04-02 03:02:22.000000 fastapi-di-extension-0.0.3/src/fast_di/depends/depends_stub.py
+-rw-rw-r--   0 alim      (1000) alim      (1000)      452 2024-04-02 03:02:53.000000 fastapi-di-extension-0.0.3/src/fast_di/init_dependencies.py
+drwxrwxr-x   0 alim      (1000) alim      (1000)        0 2024-04-02 03:03:40.468175 fastapi-di-extension-0.0.3/src/fastapi_di_extension.egg-info/
+-rw-r--r--   0 alim      (1000) alim      (1000)     1357 2024-04-02 03:03:40.000000 fastapi-di-extension-0.0.3/src/fastapi_di_extension.egg-info/PKG-INFO
+-rw-rw-r--   0 alim      (1000) alim      (1000)      526 2024-04-02 03:03:40.000000 fastapi-di-extension-0.0.3/src/fastapi_di_extension.egg-info/SOURCES.txt
+-rw-rw-r--   0 alim      (1000) alim      (1000)        1 2024-04-02 03:03:40.000000 fastapi-di-extension-0.0.3/src/fastapi_di_extension.egg-info/dependency_links.txt
+-rw-rw-r--   0 alim      (1000) alim      (1000)      182 2024-04-02 03:03:40.000000 fastapi-di-extension-0.0.3/src/fastapi_di_extension.egg-info/requires.txt
+-rw-rw-r--   0 alim      (1000) alim      (1000)        8 2024-04-02 03:03:40.000000 fastapi-di-extension-0.0.3/src/fastapi_di_extension.egg-info/top_level.txt
```

### Comparing `fastapi-di-extension-0.0.2/LICENSE` & `fastapi-di-extension-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi-di-extension-0.0.2/PKG-INFO` & `fastapi-di-extension-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-di-extension
-Version: 0.0.2
+Version: 0.0.3
 Summary: Minimal DI library for fastapi
 Author-email: Alim Abrekov <Abrekovalim38702@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/dark04072006/fastapi-di-extension
 Project-URL: Homepage, https://github.com/dark04072006/fastapi-di-extension
 Project-URL: Bug Tracker, https://github.com/dark04072006/fastapi-di-extension/issues
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `fastapi-di-extension-0.0.2/pyproject.toml` & `fastapi-di-extension-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 include-package-data = true
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [project]
 name = "fastapi-di-extension"
-version = "0.0.2"
+version = "0.0.3"
 readme = "README.md"
 authors = [
     { name = "Alim Abrekov", email = "Abrekovalim38702@gmail.com" },
 ]
 license = { text = "Apache-2.0" }
 description = "Minimal DI library for fastapi"
 requires-python = ">=3.10"
```

### Comparing `fastapi-di-extension-0.0.2/src/fast_di/collector/base.py` & `fastapi-di-extension-0.0.3/src/fast_di/collector/base.py`

 * *Files identical despite different names*

### Comparing `fastapi-di-extension-0.0.2/src/fast_di/collector/collector.py` & `fastapi-di-extension-0.0.3/src/fast_di/collector/collector.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 from typing import Callable
 
 from fast_di.collector.base import BaseDependencyCollector, DependencyT, FactoryT
 
 
 class DependencyCollector(BaseDependencyCollector):
-    def __init__(self) -> None:
-        super().__init__()
-
     def factory(self, dependency: DependencyT) -> Callable[[FactoryT], None]:
         def decorator(factory: FactoryT) -> None:
             self.add_factory(dependency, factory)
 
         return decorator
 
     def singleton(
```

### Comparing `fastapi-di-extension-0.0.2/src/fast_di/depends/depends_stub.py` & `fastapi-di-extension-0.0.3/src/fast_di/depends/depends_stub.py`

 * *Files identical despite different names*

### Comparing `fastapi-di-extension-0.0.2/src/fastapi_di_extension.egg-info/PKG-INFO` & `fastapi-di-extension-0.0.3/src/fastapi_di_extension.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-di-extension
-Version: 0.0.2
+Version: 0.0.3
 Summary: Minimal DI library for fastapi
 Author-email: Alim Abrekov <Abrekovalim38702@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/dark04072006/fastapi-di-extension
 Project-URL: Homepage, https://github.com/dark04072006/fastapi-di-extension
 Project-URL: Bug Tracker, https://github.com/dark04072006/fastapi-di-extension/issues
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `fastapi-di-extension-0.0.2/src/fastapi_di_extension.egg-info/SOURCES.txt` & `fastapi-di-extension-0.0.3/src/fastapi_di_extension.egg-info/SOURCES.txt`

 * *Files identical despite different names*

