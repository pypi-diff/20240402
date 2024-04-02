# Comparing `tmp/shipyard_file_manipulation-0.2.0.tar.gz` & `tmp/shipyard_file_manipulation-0.2.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_file_manipulation-0.2.0.tar", max compression
+gzip compressed data, was "shipyard_file_manipulation-0.2.0a0.tar", max compression
```

## Comparing `shipyard_file_manipulation-0.2.0.tar` & `shipyard_file_manipulation-0.2.0a0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2024-01-04 01:57:22.676418 shipyard_file_manipulation-0.2.0/README.md
--rw-r--r--   0        0        0      630 2024-04-02 01:23:00.860623 shipyard_file_manipulation-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       74 2024-04-02 01:11:25.049115 shipyard_file_manipulation-0.2.0/shipyard_file_manipulation/__init__.py
--rw-r--r--   0        0        0     2860 2024-04-02 01:11:25.049485 shipyard_file_manipulation-0.2.0/shipyard_file_manipulation/cli/compare.py
--rw-r--r--   0        0        0     3522 2024-04-02 01:11:25.049660 shipyard_file_manipulation-0.2.0/shipyard_file_manipulation/cli/compress.py
--rw-r--r--   0        0        0     5139 2024-04-02 01:11:25.049888 shipyard_file_manipulation-0.2.0/shipyard_file_manipulation/cli/convert.py
--rw-r--r--   0        0        0     2840 2024-04-02 01:11:25.050043 shipyard_file_manipulation-0.2.0/shipyard_file_manipulation/cli/decompress.py
--rw-r--r--   0        0        0     3980 2024-04-02 01:11:25.050406 shipyard_file_manipulation-0.2.0/shipyard_file_manipulation/core.py
--rw-r--r--   0        0        0      979 2024-04-02 01:11:25.050581 shipyard_file_manipulation-0.2.0/shipyard_file_manipulation/errors.py
--rw-r--r--   0        0        0      678 1970-01-01 00:00:00.000000 shipyard_file_manipulation-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-01-04 01:57:22.676418 shipyard_file_manipulation-0.2.0a0/README.md
+-rw-r--r--   0        0        0      524 2024-03-27 22:10:03.809124 shipyard_file_manipulation-0.2.0a0/pyproject.toml
+-rw-r--r--   0        0        0       74 2024-03-27 20:24:20.948612 shipyard_file_manipulation-0.2.0a0/shipyard_file_manipulation/__init__.py
+-rw-r--r--   0        0        0     2860 2024-03-27 22:16:52.780650 shipyard_file_manipulation-0.2.0a0/shipyard_file_manipulation/cli/compare.py
+-rw-r--r--   0        0        0     3522 2024-03-27 22:06:49.237062 shipyard_file_manipulation-0.2.0a0/shipyard_file_manipulation/cli/compress.py
+-rw-r--r--   0        0        0     5139 2024-03-27 22:06:49.244042 shipyard_file_manipulation-0.2.0a0/shipyard_file_manipulation/cli/convert.py
+-rw-r--r--   0        0        0     2840 2024-03-27 22:06:49.235391 shipyard_file_manipulation-0.2.0a0/shipyard_file_manipulation/cli/decompress.py
+-rw-r--r--   0        0        0     3980 2024-03-27 22:16:44.413719 shipyard_file_manipulation-0.2.0a0/shipyard_file_manipulation/core.py
+-rw-r--r--   0        0        0      979 2024-03-27 22:06:49.241843 shipyard_file_manipulation-0.2.0a0/shipyard_file_manipulation/errors.py
+-rw-r--r--   0        0        0      572 1970-01-01 00:00:00.000000 shipyard_file_manipulation-0.2.0a0/PKG-INFO
```

### Comparing `shipyard_file_manipulation-0.2.0/pyproject.toml` & `shipyard_file_manipulation-0.2.0a0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "shipyard-file-manipulation"
-version = "0.2.0"
-description = "A set of utility functions for maniuplating datasets. This is primarily used within the Shipyard Application"
+version = "0.2.0a0"
+description = ""
 authors = ["wrp801 <wespoulsen@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pandas = "^2.0"
 pyarrow = "^15.0.2"
```

### Comparing `shipyard_file_manipulation-0.2.0/shipyard_file_manipulation/cli/compare.py` & `shipyard_file_manipulation-0.2.0a0/shipyard_file_manipulation/cli/compare.py`

 * *Files identical despite different names*

### Comparing `shipyard_file_manipulation-0.2.0/shipyard_file_manipulation/cli/compress.py` & `shipyard_file_manipulation-0.2.0a0/shipyard_file_manipulation/cli/compress.py`

 * *Files identical despite different names*

### Comparing `shipyard_file_manipulation-0.2.0/shipyard_file_manipulation/cli/convert.py` & `shipyard_file_manipulation-0.2.0a0/shipyard_file_manipulation/cli/convert.py`

 * *Files identical despite different names*

### Comparing `shipyard_file_manipulation-0.2.0/shipyard_file_manipulation/cli/decompress.py` & `shipyard_file_manipulation-0.2.0a0/shipyard_file_manipulation/cli/decompress.py`

 * *Files identical despite different names*

### Comparing `shipyard_file_manipulation-0.2.0/shipyard_file_manipulation/core.py` & `shipyard_file_manipulation-0.2.0a0/shipyard_file_manipulation/core.py`

 * *Files identical despite different names*

### Comparing `shipyard_file_manipulation-0.2.0/shipyard_file_manipulation/errors.py` & `shipyard_file_manipulation-0.2.0a0/shipyard_file_manipulation/errors.py`

 * *Files identical despite different names*

### Comparing `shipyard_file_manipulation-0.2.0/PKG-INFO` & `shipyard_file_manipulation-0.2.0a0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: shipyard-file-manipulation
-Version: 0.2.0
-Summary: A set of utility functions for maniuplating datasets. This is primarily used within the Shipyard Application
+Version: 0.2.0a0
+Summary: 
 Author: wrp801
 Author-email: wespoulsen@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

