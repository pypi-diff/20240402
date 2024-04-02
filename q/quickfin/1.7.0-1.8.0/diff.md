# Comparing `tmp/quickfin-1.7.0.tar.gz` & `tmp/quickfin-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickfin-1.7.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "quickfin-1.8.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `quickfin-1.7.0.tar` & `quickfin-1.8.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0       66 2024-04-01 12:12:25.158711 quickfin-1.7.0/README.md
--rw-r--r--   0        0        0      730 2024-04-02 09:40:45.743229 quickfin-1.7.0/pyproject.toml
--rw-r--r--   0        0        0    26853 2024-04-02 09:40:19.685593 quickfin-1.7.0/quickfin.py
--rw-r--r--   0        0        0      666 1970-01-01 00:00:00.000000 quickfin-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0       66 2024-04-01 12:12:25.158711 quickfin-1.8.0/README.md
+-rw-r--r--   0        0        0      730 2024-04-02 09:50:53.413362 quickfin-1.8.0/pyproject.toml
+-rw-r--r--   0        0        0    26853 2024-04-02 09:51:06.546151 quickfin-1.8.0/quickfin.py
+-rw-r--r--   0        0        0      666 1970-01-01 00:00:00.000000 quickfin-1.8.0/PKG-INFO
```

### Comparing `quickfin-1.7.0/pyproject.toml` & `quickfin-1.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "quickfin"
-version = "1.7.0"
+version = "1.8.0"
 authors = [{name = "Derek Evans"}]
 description = "A Python module providing instant access to live and historical stock market price data, automated Plotly data visualization generators and a metadata catalog for referencing equities, stock symbols, sectors, and industry information."
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `quickfin-1.7.0/quickfin.py` & `quickfin-1.8.0/quickfin.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 A Python module providing instant access to live
 and historical stock market price data, automated
 Plotly data visualization generators and a metadata
 catalog for referencing equities, stock symbols, sectors,
 and industry information.
 """
 
-__version__ = "1.7.0"
+__version__ = "1.8.0"
 __author__ = "Derek Evans <https://github.com/REPNOT>"
 __date__ = "28 March 2024"
 
 import json
 from pprint import pprint
 import requests
 import datetime
```

### Comparing `quickfin-1.7.0/PKG-INFO` & `quickfin-1.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickfin
-Version: 1.7.0
+Version: 1.8.0
 Summary: A Python module providing instant access to live and historical stock market price data, automated Plotly data visualization generators and a metadata catalog for referencing equities, stock symbols, sectors, and industry information.
 Author: Derek Evans
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

