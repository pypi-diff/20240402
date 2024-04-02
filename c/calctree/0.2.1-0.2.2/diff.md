# Comparing `tmp/calctree-0.2.1.tar.gz` & `tmp/calctree-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calctree-0.2.1.tar", max compression
+gzip compressed data, was "calctree-0.2.2.tar", max compression
```

## Comparing `calctree-0.2.1.tar` & `calctree-0.2.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1065 2024-01-25 06:17:32.518074 calctree-0.2.1/LICENSE
--rw-r--r--   0        0        0     1373 2024-03-28 05:21:21.983559 calctree-0.2.1/README.md
--rw-r--r--   0        0        0      376 2024-03-28 05:14:01.768883 calctree-0.2.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-08 04:34:01.046790 calctree-0.2.1/src/calctree/__init__.py
--rw-r--r--   0        0        0     1724 2024-03-28 05:14:01.769466 calctree-0.2.1/src/calctree/calculation_result.py
--rw-r--r--   0        0        0     2545 2024-03-28 05:14:01.770148 calctree-0.2.1/src/calctree/client.py
--rw-r--r--   0        0        0       54 2024-03-28 05:14:01.772124 calctree-0.2.1/src/calctree/exceptions.py
--rw-r--r--   0        0        0     1773 1970-01-01 00:00:00.000000 calctree-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-01-25 06:17:32.518074 calctree-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1373 2024-03-28 05:21:21.983559 calctree-0.2.2/README.md
+-rw-r--r--   0        0        0      376 2024-04-02 00:38:30.000938 calctree-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      181 2024-04-02 00:24:30.436727 calctree-0.2.2/src/calctree/__init__.py
+-rw-r--r--   0        0        0     1711 2024-04-02 00:36:33.402029 calctree-0.2.2/src/calctree/calculation_result.py
+-rw-r--r--   0        0        0     2532 2024-04-02 00:09:20.269193 calctree-0.2.2/src/calctree/client.py
+-rw-r--r--   0        0        0       54 2024-03-28 05:14:01.772124 calctree-0.2.2/src/calctree/exceptions.py
+-rw-r--r--   0        0        0     1773 1970-01-01 00:00:00.000000 calctree-0.2.2/PKG-INFO
```

### Comparing `calctree-0.2.1/LICENSE` & `calctree-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `calctree-0.2.1/README.md` & `calctree-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `calctree-0.2.1/src/calctree/calculation_result.py` & `calctree-0.2.2/src/calctree/calculation_result.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 from typing import List
 
-from src.calctree.exceptions import ParameterNotFoundException
+from exceptions import ParameterNotFoundException
 
 
 class CalculationResult:
     """
     Represents the result of a calculation performed by the CalcTree API.
     """
```

### Comparing `calctree-0.2.1/src/calctree/client.py` & `calctree-0.2.2/src/calctree/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 from urllib import request
 
-from src.calctree.calculation_result import CalculationResult
+from calculation_result import CalculationResult
 
 
 class CalcTreeClient:
     """Client for interacting with the CalcTree API.
 
     This client allows you to perform calculations using the CalcTree API.
```

### Comparing `calctree-0.2.1/PKG-INFO` & `calctree-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calctree
-Version: 0.2.1
+Version: 0.2.2
 Summary: 
 Author: CalcTree
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

