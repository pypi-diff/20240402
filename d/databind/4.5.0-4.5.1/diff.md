# Comparing `tmp/databind-4.5.0.tar.gz` & `tmp/databind-4.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databind-4.5.0.tar", max compression
+gzip compressed data, was "databind-4.5.1.tar", max compression
```

## Comparing `databind-4.5.0.tar` & `databind-4.5.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     3048 2024-03-19 19:49:02.841940 databind-4.5.0/README.md
--rw-r--r--   0        0        0     1884 2024-03-19 19:49:06.792262 databind-4.5.0/pyproject.toml
--rw-r--r--   0        0        0     1601 2024-03-19 19:49:06.792427 databind-4.5.0/src/databind/core/__init__.py
--rw-r--r--   0        0        0     5481 2024-03-19 19:42:46.047393 databind-4.5.0/src/databind/core/context.py
--rw-r--r--   0        0        0     6703 2024-03-19 19:42:46.047542 databind-4.5.0/src/databind/core/converter.py
--rw-r--r--   0        0        0     4099 2024-03-19 19:42:46.047685 databind-4.5.0/src/databind/core/dataclasses.py
--rw-r--r--   0        0        0     7120 2024-03-19 19:42:46.047815 databind-4.5.0/src/databind/core/dataclasses.pyi
--rw-r--r--   0        0        0     3943 2024-03-19 19:42:46.047941 databind-4.5.0/src/databind/core/mapper.py
--rw-r--r--   0        0        0        0 2024-03-19 19:42:46.048001 databind-4.5.0/src/databind/core/py.typed
--rw-r--r--   0        0        0    15523 2024-03-19 19:42:46.048210 databind-4.5.0/src/databind/core/schema.py
--rw-r--r--   0        0        0    27807 2024-03-19 19:49:02.843315 databind-4.5.0/src/databind/core/settings.py
--rw-r--r--   0        0        0     1044 2024-03-19 19:42:46.048591 databind-4.5.0/src/databind/core/tests/context_test.py
--rw-r--r--   0        0        0     1275 2024-03-19 19:42:46.048704 databind-4.5.0/src/databind/core/tests/schema_docspec_example_test.py
--rw-r--r--   0        0        0    11105 2024-03-19 19:42:46.048839 databind-4.5.0/src/databind/core/tests/schema_test.py
--rw-r--r--   0        0        0      733 2024-03-19 19:42:46.048951 databind-4.5.0/src/databind/core/tests/schema_with_nested_dataclasses_test.py
--rw-r--r--   0        0        0     8933 2024-03-19 19:42:46.049093 databind-4.5.0/src/databind/core/union.py
--rw-r--r--   0        0        0     2955 2024-03-19 19:42:46.049212 databind-4.5.0/src/databind/core/utils.py
--rw-r--r--   0        0        0     2410 2024-03-19 19:49:06.792566 databind-4.5.0/src/databind/json/__init__.py
--rw-r--r--   0        0        0    35450 2024-03-19 19:42:46.049587 databind-4.5.0/src/databind/json/converters.py
--rw-r--r--   0        0        0     2951 2024-03-19 19:42:46.049715 databind-4.5.0/src/databind/json/module.py
--rw-r--r--   0        0        0        0 2024-03-19 19:42:46.049780 databind-4.5.0/src/databind/json/py.typed
--rw-r--r--   0        0        0     1934 2024-03-19 19:42:46.049914 databind-4.5.0/src/databind/json/settings.py
--rw-r--r--   0        0        0    27496 2024-03-19 19:42:46.050128 databind-4.5.0/src/databind/json/tests/converters_test.py
--rw-r--r--   0        0        0     4086 1970-01-01 00:00:00.000000 databind-4.5.0/PKG-INFO
+-rw-r--r--   0        0        0     3048 2024-04-02 09:25:49.053087 databind-4.5.1/README.md
+-rw-r--r--   0        0        0     2118 2024-04-02 10:02:28.522788 databind-4.5.1/pyproject.toml
+-rw-r--r--   0        0        0     1601 2024-04-02 10:02:28.522953 databind-4.5.1/src/databind/core/__init__.py
+-rw-r--r--   0        0        0     5481 2024-04-02 09:22:26.323647 databind-4.5.1/src/databind/core/context.py
+-rw-r--r--   0        0        0     6703 2024-04-02 09:22:26.323889 databind-4.5.1/src/databind/core/converter.py
+-rw-r--r--   0        0        0     4099 2024-04-02 09:22:26.324326 databind-4.5.1/src/databind/core/dataclasses.py
+-rw-r--r--   0        0        0     7120 2024-04-02 09:22:26.324930 databind-4.5.1/src/databind/core/dataclasses.pyi
+-rw-r--r--   0        0        0     3943 2024-04-02 09:22:26.325111 databind-4.5.1/src/databind/core/mapper.py
+-rw-r--r--   0        0        0        0 2024-04-02 09:22:26.325215 databind-4.5.1/src/databind/core/py.typed
+-rw-r--r--   0        0        0    15523 2024-04-02 09:22:26.325612 databind-4.5.1/src/databind/core/schema.py
+-rw-r--r--   0        0        0    27807 2024-04-02 09:22:26.325870 databind-4.5.1/src/databind/core/settings.py
+-rw-r--r--   0        0        0     1044 2024-04-02 09:22:26.326210 databind-4.5.1/src/databind/core/tests/context_test.py
+-rw-r--r--   0        0        0     1275 2024-04-02 09:22:26.331892 databind-4.5.1/src/databind/core/tests/schema_docspec_example_test.py
+-rw-r--r--   0        0        0    11105 2024-04-02 09:22:26.333093 databind-4.5.1/src/databind/core/tests/schema_test.py
+-rw-r--r--   0        0        0      733 2024-04-02 09:22:26.333360 databind-4.5.1/src/databind/core/tests/schema_with_nested_dataclasses_test.py
+-rw-r--r--   0        0        0     8933 2024-04-02 09:22:26.334093 databind-4.5.1/src/databind/core/union.py
+-rw-r--r--   0        0        0     2955 2024-04-02 09:22:26.334297 databind-4.5.1/src/databind/core/utils.py
+-rw-r--r--   0        0        0     2410 2024-04-02 10:02:28.523077 databind-4.5.1/src/databind/json/__init__.py
+-rw-r--r--   0        0        0    35450 2024-04-02 09:22:26.334878 databind-4.5.1/src/databind/json/converters.py
+-rw-r--r--   0        0        0     2951 2024-04-02 09:22:26.335050 databind-4.5.1/src/databind/json/module.py
+-rw-r--r--   0        0        0        0 2024-04-02 09:22:26.335120 databind-4.5.1/src/databind/json/py.typed
+-rw-r--r--   0        0        0     1934 2024-04-02 09:22:26.335313 databind-4.5.1/src/databind/json/settings.py
+-rw-r--r--   0        0        0    27496 2024-04-02 09:22:26.335657 databind-4.5.1/src/databind/json/tests/converters_test.py
+-rw-r--r--   0        0        0     4328 1970-01-01 00:00:00.000000 databind-4.5.1/PKG-INFO
```

### Comparing `databind-4.5.0/README.md` & `databind-4.5.1/README.md`

 * *Files identical despite different names*

### Comparing `databind-4.5.0/pyproject.toml` & `databind-4.5.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 [tool.poetry]
 name = "databind"
-version = "4.5.0"
+version = "4.5.1"
 description = "Databind is a library inspired by jackson-databind to de-/serialize Python dataclasses. The `databind` package will install the full suite of databind packages. Compatible with Python 3.8 and newer."
 authors = ["Niklas Rosenstein <rosensteinniklas@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "databind/core", from = "src"}, {include = "databind/json", from = "src"}]
 
+[tool.poetry.urls]
+"Bug Tracker" = "https://github.com/NiklasRosenstein/python-databind/issues"
+Documentation = "https://niklasrosenstein.github.io/python-databind/"
+Repository = "https://github.com/NiklasRosenstein/python-databind"
+
 [tool.poetry.dependencies]
 python = "^3.8.0"
 Deprecated = "^1.2.12"
 nr-date = "^2.0.0"
 nr-stream = "^1.0.0"
 setuptools = { version = ">=40.8.0", markers = "python_version < '3.10'" }
 typeapi = ">=2.0.1,<3"
```

### Comparing `databind-4.5.0/src/databind/core/__init__.py` & `databind-4.5.1/src/databind/core/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "4.5.0"
+__version__ = "4.5.1"
 
 from .context import Context, Direction, Location, format_context_trace
 from .converter import ConversionError, Converter, DelegateToClassmethodConverter, Module, NoMatchingConverter
 from .mapper import ObjectMapper
 from .schema import (
     Field,
     Schema,
```

### Comparing `databind-4.5.0/src/databind/core/context.py` & `databind-4.5.1/src/databind/core/context.py`

 * *Files identical despite different names*

### Comparing `databind-4.5.0/src/databind/core/converter.py` & `databind-4.5.1/src/databind/core/converter.py`

 * *Files identical despite different names*

### Comparing `databind-4.5.0/src/databind/core/dataclasses.py` & `databind-4.5.1/src/databind/core/dataclasses.py`

 * *Files identical despite different names*

### Comparing `databind-4.5.0/src/databind/core/dataclasses.pyi` & `databind-4.5.1/src/databind/core/dataclasses.pyi`

 * *Files identical despite different names*

### Comparing `databind-4.5.0/src/databind/core/mapper.py` & `databind-4.5.1/src/databind/core/mapper.py`

 * *Files identical despite different names*

### Comparing `databind-4.5.0/src/databind/core/schema.py` & `databind-4.5.1/src/databind/core/schema.py`

 * *Files identical despite different names*

### Comparing `databind-4.5.0/src/databind/core/settings.py` & `databind-4.5.1/src/databind/core/settings.py`

 * *Files identical despite different names*

### Comparing `databind-4.5.0/src/databind/core/tests/context_test.py` & `databind-4.5.1/src/databind/core/tests/context_test.py`

 * *Files identical despite different names*

### Comparing `databind-4.5.0/src/databind/core/tests/schema_docspec_example_test.py` & `databind-4.5.1/src/databind/core/tests/schema_docspec_example_test.py`

 * *Files identical despite different names*

### Comparing `databind-4.5.0/src/databind/core/tests/schema_test.py` & `databind-4.5.1/src/databind/core/tests/schema_test.py`

 * *Files identical despite different names*

### Comparing `databind-4.5.0/src/databind/core/tests/schema_with_nested_dataclasses_test.py` & `databind-4.5.1/src/databind/core/tests/schema_with_nested_dataclasses_test.py`

 * *Files identical despite different names*

### Comparing `databind-4.5.0/src/databind/core/union.py` & `databind-4.5.1/src/databind/core/union.py`

 * *Files identical despite different names*

### Comparing `databind-4.5.0/src/databind/core/utils.py` & `databind-4.5.1/src/databind/core/utils.py`

 * *Files identical despite different names*

### Comparing `databind-4.5.0/src/databind/json/__init__.py` & `databind-4.5.1/src/databind/json/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import json
 import typing as t
 
 from databind.core import ObjectMapper, Setting, Settings
 from databind.json.module import JsonModule
 from databind.json.settings import JsonConverter
 
-__version__ = "4.5.0"
+__version__ = "4.5.1"
 __all__ = [
     "dump",
     "dumps",
     "get_object_mapper",
     "JsonConverter",
     "JsonModule",
     "JsonType",
```

### Comparing `databind-4.5.0/src/databind/json/converters.py` & `databind-4.5.1/src/databind/json/converters.py`

 * *Files identical despite different names*

### Comparing `databind-4.5.0/src/databind/json/module.py` & `databind-4.5.1/src/databind/json/module.py`

 * *Files identical despite different names*

### Comparing `databind-4.5.0/src/databind/json/settings.py` & `databind-4.5.1/src/databind/json/settings.py`

 * *Files identical despite different names*

### Comparing `databind-4.5.0/src/databind/json/tests/converters_test.py` & `databind-4.5.1/src/databind/json/tests/converters_test.py`

 * *Files identical despite different names*

### Comparing `databind-4.5.0/PKG-INFO` & `databind-4.5.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databind
-Version: 4.5.0
+Version: 4.5.1
 Summary: Databind is a library inspired by jackson-databind to de-/serialize Python dataclasses. The `databind` package will install the full suite of databind packages. Compatible with Python 3.8 and newer.
 License: MIT
 Author: Niklas Rosenstein
 Author-email: rosensteinniklas@gmail.com
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -15,14 +15,17 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: Deprecated (>=1.2.12,<2.0.0)
 Requires-Dist: nr-date (>=2.0.0,<3.0.0)
 Requires-Dist: nr-stream (>=1.0.0,<2.0.0)
 Requires-Dist: setuptools (>=40.8.0) ; python_version < "3.10"
 Requires-Dist: typeapi (>=2.0.1,<3)
 Requires-Dist: typing-extensions (>=3.10.0,<5)
+Project-URL: Bug Tracker, https://github.com/NiklasRosenstein/python-databind/issues
+Project-URL: Documentation, https://niklasrosenstein.github.io/python-databind/
+Project-URL: Repository, https://github.com/NiklasRosenstein/python-databind
 Description-Content-Type: text/markdown
 
 <p align="center"><img src="https://i.imgur.com/KkWFne2.png" width="256px"></p>
 
 <h1 align="center">databind</h1>
 
 <p align="center">
```

