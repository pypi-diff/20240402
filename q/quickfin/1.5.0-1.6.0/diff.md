# Comparing `tmp/quickfin-1.5.0.tar.gz` & `tmp/quickfin-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickfin-1.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "quickfin-1.6.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `quickfin-1.5.0.tar` & `quickfin-1.6.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0       66 2024-04-01 12:12:25.158711 quickfin-1.5.0/README.md
--rw-r--r--   0        0        0      770 2024-04-01 12:34:56.676433 quickfin-1.5.0/pyproject.toml
--rw-r--r--   0        0        0    28708 2024-04-01 12:34:50.989524 quickfin-1.5.0/quickfin.py
--rw-r--r--   0        0        0      703 1970-01-01 00:00:00.000000 quickfin-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0       66 2024-04-01 12:12:25.158711 quickfin-1.6.0/README.md
+-rw-r--r--   0        0        0      729 2024-04-01 14:20:04.529503 quickfin-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0    28708 2024-04-01 14:19:53.389110 quickfin-1.6.0/quickfin.py
+-rw-r--r--   0        0        0      665 1970-01-01 00:00:00.000000 quickfin-1.6.0/PKG-INFO
```

### Comparing `quickfin-1.5.0/pyproject.toml` & `quickfin-1.6.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "quickfin"
-version = "1.5.0"
-authors = [{name = "Derek Evans", email = "derek.evans@deinfoservice.com"}]
+version = "1.6.0"
+authors = [{name = "Derek Evans"}]
 description = "A Python module providing instant access to live and historical stock market price data, automated Plotly data visualization generators and a metadata catalog for referencing equities, stock symbols, sectors, and industry information."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `quickfin-1.5.0/quickfin.py` & `quickfin-1.6.0/quickfin.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 A Python module providing instant access to live
 and historical stock market price data, automated
 Plotly data visualization generators and a metadata
 catalog for referencing equities, stock symbols, sectors,
 and industry information.
 """
 
-__version__ = "1.5.0"
+__version__ = "1.6.0"
 __author__ = "Derek Evans <https://github.com/REPNOT>"
 __date__ = "28 March 2024"
 
 import json
 from pprint import pprint
 import requests
 import datetime
```

### Comparing `quickfin-1.5.0/PKG-INFO` & `quickfin-1.6.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: quickfin
-Version: 1.5.0
+Version: 1.6.0
 Summary: A Python module providing instant access to live and historical stock market price data, automated Plotly data visualization generators and a metadata catalog for referencing equities, stock symbols, sectors, and industry information.
-Author-email: Derek Evans <derek.evans@deinfoservice.com>
+Author: Derek Evans
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Dist: plotly
 Project-URL: Home, https://quickfin.techbyderek.com/
```

