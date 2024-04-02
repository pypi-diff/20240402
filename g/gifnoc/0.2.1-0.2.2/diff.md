# Comparing `tmp/gifnoc-0.2.1.tar.gz` & `tmp/gifnoc-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gifnoc-0.2.1.tar", max compression
+gzip compressed data, was "gifnoc-0.2.2.tar", max compression
```

## Comparing `gifnoc-0.2.1.tar` & `gifnoc-0.2.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     2268 2024-03-13 17:48:39.575307 gifnoc-0.2.1/README.md
--rw-r--r--   0        0        0      467 2024-03-20 01:16:51.384569 gifnoc-0.2.1/gifnoc/__init__.py
--rw-r--r--   0        0        0     3289 2024-03-22 19:29:13.603238 gifnoc-0.2.1/gifnoc/__main__.py
--rw-r--r--   0        0        0     2988 2024-03-20 22:11:14.339440 gifnoc-0.2.1/gifnoc/acquire.py
--rw-r--r--   0        0        0     6292 2024-03-22 19:30:42.121327 gifnoc-0.2.1/gifnoc/arg.py
--rw-r--r--   0        0        0     1293 2024-03-20 17:29:30.398729 gifnoc-0.2.1/gifnoc/config.py
--rw-r--r--   0        0        0     9878 2024-03-22 19:29:35.957640 gifnoc-0.2.1/gifnoc/core.py
--rw-r--r--   0        0        0      584 2024-03-11 19:31:05.660822 gifnoc-0.2.1/gifnoc/define.py
--rw-r--r--   0        0        0     4420 2024-03-14 18:27:32.891465 gifnoc-0.2.1/gifnoc/docstrings.py
--rw-r--r--   0        0        0     1348 2024-03-04 20:00:45.907307 gifnoc-0.2.1/gifnoc/merge.py
--rw-r--r--   0        0        0     3787 2024-03-20 22:24:36.979399 gifnoc-0.2.1/gifnoc/parse.py
--rw-r--r--   0        0        0     3175 2024-03-20 20:39:19.046342 gifnoc-0.2.1/gifnoc/registry.py
--rw-r--r--   0        0        0     1585 2024-03-08 22:41:21.116456 gifnoc-0.2.1/gifnoc/schema.py
--rw-r--r--   0        0        0      247 2024-03-08 22:39:08.607547 gifnoc-0.2.1/gifnoc/std/__init__.py
--rw-r--r--   0        0        0      819 2024-03-11 19:06:40.540661 gifnoc-0.2.1/gifnoc/std/_time.py
--rw-r--r--   0        0        0     3316 2024-03-21 18:13:13.453188 gifnoc-0.2.1/gifnoc/type_wrappers.py
--rw-r--r--   0        0        0     4273 2024-03-20 22:11:06.107781 gifnoc-0.2.1/gifnoc/utils.py
--rw-r--r--   0        0        0       18 2024-03-22 19:31:23.950839 gifnoc-0.2.1/gifnoc/version.py
--rw-r--r--   0        0        0      544 2024-03-22 19:31:23.928513 gifnoc-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2895 1970-01-01 00:00:00.000000 gifnoc-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     2268 2024-03-13 17:48:39.575307 gifnoc-0.2.2/README.md
+-rw-r--r--   0        0        0      467 2024-03-20 01:16:51.384569 gifnoc-0.2.2/gifnoc/__init__.py
+-rw-r--r--   0        0        0     3289 2024-03-22 19:29:13.603238 gifnoc-0.2.2/gifnoc/__main__.py
+-rw-r--r--   0        0        0     2988 2024-03-20 22:11:14.339440 gifnoc-0.2.2/gifnoc/acquire.py
+-rw-r--r--   0        0        0     6306 2024-04-02 18:13:35.610877 gifnoc-0.2.2/gifnoc/arg.py
+-rw-r--r--   0        0        0     1390 2024-04-02 18:17:30.844733 gifnoc-0.2.2/gifnoc/config.py
+-rw-r--r--   0        0        0     9878 2024-03-22 19:29:35.957640 gifnoc-0.2.2/gifnoc/core.py
+-rw-r--r--   0        0        0      584 2024-03-11 19:31:05.660822 gifnoc-0.2.2/gifnoc/define.py
+-rw-r--r--   0        0        0     4420 2024-03-14 18:27:32.891465 gifnoc-0.2.2/gifnoc/docstrings.py
+-rw-r--r--   0        0        0     1348 2024-03-04 20:00:45.907307 gifnoc-0.2.2/gifnoc/merge.py
+-rw-r--r--   0        0        0     3782 2024-04-02 18:12:58.922625 gifnoc-0.2.2/gifnoc/parse.py
+-rw-r--r--   0        0        0     3175 2024-03-20 20:39:19.046342 gifnoc-0.2.2/gifnoc/registry.py
+-rw-r--r--   0        0        0     1585 2024-03-08 22:41:21.116456 gifnoc-0.2.2/gifnoc/schema.py
+-rw-r--r--   0        0        0      247 2024-03-08 22:39:08.607547 gifnoc-0.2.2/gifnoc/std/__init__.py
+-rw-r--r--   0        0        0      819 2024-03-11 19:06:40.540661 gifnoc-0.2.2/gifnoc/std/_time.py
+-rw-r--r--   0        0        0     3316 2024-03-21 18:13:13.453188 gifnoc-0.2.2/gifnoc/type_wrappers.py
+-rw-r--r--   0        0        0     4273 2024-03-20 22:11:06.107781 gifnoc-0.2.2/gifnoc/utils.py
+-rw-r--r--   0        0        0       18 2024-04-02 18:25:49.929057 gifnoc-0.2.2/gifnoc/version.py
+-rw-r--r--   0        0        0      544 2024-04-02 18:25:49.907352 gifnoc-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2895 1970-01-01 00:00:00.000000 gifnoc-0.2.2/PKG-INFO
```

### Comparing `gifnoc-0.2.1/README.md` & `gifnoc-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `gifnoc-0.2.1/gifnoc/__main__.py` & `gifnoc-0.2.2/gifnoc/__main__.py`

 * *Files identical despite different names*

### Comparing `gifnoc-0.2.1/gifnoc/acquire.py` & `gifnoc-0.2.2/gifnoc/acquire.py`

 * *Files identical despite different names*

### Comparing `gifnoc-0.2.1/gifnoc/arg.py` & `gifnoc-0.2.2/gifnoc/arg.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 def compile_option(model: bool, path: str, option: Option):
     if option.action is None:
         option.action = argparse.BooleanOptionalAction
     return option
 
 
 @ovld
-def compile_option(model: (int, float), path: str, option: Option):
+def compile_option(model: (int, float), path: str, option: Option):  # noqa: F811
     if option.type is None:
         option.type = model
     return option
 
 
 @ovld
 def compile_option(model: object, path: str, option: Option):  # noqa: F811
```

### Comparing `gifnoc-0.2.1/gifnoc/config.py` & `gifnoc-0.2.2/gifnoc/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,14 +33,16 @@
     def __str__(self):
         return f"Proxy for {self._obj()}"
 
     def __repr__(self):
         return f"_Proxy({self._obj()!r})"
 
     def __getattr__(self, attr):
+        if attr.startswith("__") and attr.endswith("__"):
+            raise AttributeError(attr)
         return getattr(self._obj(), attr)
 
 
 def __getattr__(key):
     return _Proxy(key)
```

### Comparing `gifnoc-0.2.1/gifnoc/core.py` & `gifnoc-0.2.2/gifnoc/core.py`

 * *Files identical despite different names*

### Comparing `gifnoc-0.2.1/gifnoc/define.py` & `gifnoc-0.2.2/gifnoc/define.py`

 * *Files identical despite different names*

### Comparing `gifnoc-0.2.1/gifnoc/docstrings.py` & `gifnoc-0.2.2/gifnoc/docstrings.py`

 * *Files identical despite different names*

### Comparing `gifnoc-0.2.1/gifnoc/merge.py` & `gifnoc-0.2.2/gifnoc/merge.py`

 * *Files identical despite different names*

### Comparing `gifnoc-0.2.1/gifnoc/parse.py` & `gifnoc-0.2.2/gifnoc/parse.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import json
 from argparse import Namespace
 from dataclasses import dataclass
 from os import environ
 from pathlib import Path
-from types import NoneType
 
 from ovld import ovld
 
 from .utils import DELETE, MissingProxy
 
+NoneType = type(None)
 EnvironType = type(environ)
 
 
 class NoParserError(Exception):
     """Exception to raise when no parser is found."""
```

### Comparing `gifnoc-0.2.1/gifnoc/registry.py` & `gifnoc-0.2.2/gifnoc/registry.py`

 * *Files identical despite different names*

### Comparing `gifnoc-0.2.1/gifnoc/schema.py` & `gifnoc-0.2.2/gifnoc/schema.py`

 * *Files identical despite different names*

### Comparing `gifnoc-0.2.1/gifnoc/std/_time.py` & `gifnoc-0.2.2/gifnoc/std/_time.py`

 * *Files identical despite different names*

### Comparing `gifnoc-0.2.1/gifnoc/type_wrappers.py` & `gifnoc-0.2.2/gifnoc/type_wrappers.py`

 * *Files identical despite different names*

### Comparing `gifnoc-0.2.1/gifnoc/utils.py` & `gifnoc-0.2.2/gifnoc/utils.py`

 * *Files identical despite different names*

### Comparing `gifnoc-0.2.1/pyproject.toml` & `gifnoc-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gifnoc"
-version = "0.2.1"
+version = "0.2.2"
 description = "Handle configuration for multiple libraries"
 authors = ["Olivier Breuleux <breuleux@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `gifnoc-0.2.1/PKG-INFO` & `gifnoc-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gifnoc
-Version: 0.2.1
+Version: 0.2.2
 Summary: Handle configuration for multiple libraries
 License: MIT
 Author: Olivier Breuleux
 Author-email: breuleux@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

