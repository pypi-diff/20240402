# Comparing `tmp/turbopuffer-0.1.8.tar.gz` & `tmp/turbopuffer-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turbopuffer-0.1.8.tar", max compression
+gzip compressed data, was "turbopuffer-0.1.9.tar", max compression
```

## Comparing `turbopuffer-0.1.8.tar` & `turbopuffer-0.1.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1073 2023-12-15 23:16:10.914169 turbopuffer-0.1.8/LICENSE
--rw-r--r--   0        0        0     2413 2024-03-14 13:20:57.357530 turbopuffer-0.1.8/README.md
--rw-r--r--   0        0        0     1710 2024-03-14 13:22:19.900317 turbopuffer-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1243 2024-03-14 12:37:39.142334 turbopuffer-0.1.8/turbopuffer/__init__.py
--rw-r--r--   0        0        0     6454 2024-03-14 12:37:39.142750 turbopuffer-0.1.8/turbopuffer/backend.py
--rw-r--r--   0        0        0      363 2024-03-14 12:37:39.143087 turbopuffer-0.1.8/turbopuffer/error.py
--rw-r--r--   0        0        0    18852 2024-03-14 13:20:57.358283 turbopuffer-0.1.8/turbopuffer/namespace.py
--rw-r--r--   0        0        0     2693 2024-03-14 12:37:39.144023 turbopuffer-0.1.8/turbopuffer/query.py
--rw-r--r--   0        0        0    14172 2024-03-14 12:37:39.144652 turbopuffer-0.1.8/turbopuffer/vectors.py
--rw-r--r--   0        0        0       18 2024-03-14 13:22:25.179134 turbopuffer-0.1.8/turbopuffer/version.py
--rw-r--r--   0        0        0     4108 1970-01-01 00:00:00.000000 turbopuffer-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-03-28 21:43:34.286657 turbopuffer-0.1.9/LICENSE
+-rw-r--r--   0        0        0     2449 2024-04-02 19:50:02.831182 turbopuffer-0.1.9/README.md
+-rw-r--r--   0        0        0     1680 2024-04-02 19:54:43.868093 turbopuffer-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1239 2024-04-02 19:26:27.466553 turbopuffer-0.1.9/turbopuffer/__init__.py
+-rw-r--r--   0        0        0     6454 2024-03-28 21:43:34.287759 turbopuffer-0.1.9/turbopuffer/backend.py
+-rw-r--r--   0        0        0      363 2024-03-28 21:43:34.287840 turbopuffer-0.1.9/turbopuffer/error.py
+-rw-r--r--   0        0        0    18827 2024-04-02 19:25:42.356517 turbopuffer-0.1.9/turbopuffer/namespace.py
+-rw-r--r--   0        0        0     2132 2024-04-02 19:42:11.598894 turbopuffer-0.1.9/turbopuffer/query.py
+-rw-r--r--   0        0        0    14172 2024-03-28 21:43:34.288143 turbopuffer-0.1.9/turbopuffer/vectors.py
+-rw-r--r--   0        0        0       18 2024-04-02 19:53:32.375717 turbopuffer-0.1.9/turbopuffer/version.py
+-rw-r--r--   0        0        0     4120 1970-01-01 00:00:00.000000 turbopuffer-0.1.9/PKG-INFO
```

### Comparing `turbopuffer-0.1.8/LICENSE` & `turbopuffer-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `turbopuffer-0.1.8/README.md` & `turbopuffer-0.1.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -46,15 +46,18 @@
 )
 
 # Query your dataset
 vectors = ns.query(
     vector=[0.15, 0.22],
     distance_metric='cosine_distance',
     top_k=10,
-    filters={ 'name': [['Glob', 'foo*'], ['NotEq', 'food']] },
+    filters=['And', [
+        ['name', 'Glob', 'foo*'],
+        ['name', 'NotEq', 'food'],
+    ]],
     include_attributes=['name'],
     include_vectors=True
 )
 print(vectors)
 # [
 #   VectorRow(id=2, vector=[0.30000001192092896, 0.4000000059604645], attributes={'name': 'foos'}, dist=0.001016080379486084),
 #   VectorRow(id=1, vector=[0.10000000149011612, 0.20000000298023224], attributes={'name': 'foo'}, dist=0.009067952632904053)
```

### Comparing `turbopuffer-0.1.8/pyproject.toml` & `turbopuffer-0.1.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 [tool.poetry]
 name = "turbopuffer"
-version = "0.1.8"
+version = "0.1.9"
 description = "Python Client for accessing the turbopuffer API"
 authors = ["turbopuffer Inc. <info@turbopuffer.com>"]
-maintainers = ["Jacob Wirth"]
 homepage = "https://turbopuffer.com"
 documentation = "https://turbopuffer.com/docs"
 repository  = "https://github.com/turbopuffer/turbopuffer-python"
 license = "MIT"
 readme = "README.md"
 keywords = ["turbopuffer", "vector", "database", "cloud"]
 classifiers = [
```

### Comparing `turbopuffer-0.1.8/turbopuffer/__init__.py` & `turbopuffer-0.1.9/turbopuffer/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,9 +23,9 @@
             return json.JSONEncoder.default(self, obj)
 
     def dump_json_bytes(obj): return json.dumps(obj, cls=NumpyEncoder).encode()
 
 from turbopuffer.version import VERSION
 from turbopuffer.namespace import Namespace, namespaces
 from turbopuffer.vectors import VectorColumns, VectorRow, VectorResult
-from turbopuffer.query import VectorQuery, FilterTuple
+from turbopuffer.query import VectorQuery, Filters
 from turbopuffer.error import TurbopufferError, AuthenticationError, APIError
```

### Comparing `turbopuffer-0.1.8/turbopuffer/backend.py` & `turbopuffer-0.1.9/turbopuffer/backend.py`

 * *Files identical despite different names*

### Comparing `turbopuffer-0.1.8/turbopuffer/namespace.py` & `turbopuffer-0.1.9/turbopuffer/namespace.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
 import iso8601
 from turbopuffer.error import APIError
 from turbopuffer.vectors import Cursor, VectorResult, VectorColumns, VectorRow, batch_iter
 from turbopuffer.backend import Backend
-from turbopuffer.query import VectorQuery, FilterTuple
+from turbopuffer.query import VectorQuery, Filters
 from typing import Dict, List, Optional, Iterable, Union, overload
 import turbopuffer as tpuf
 
 
 class Namespace:
     """
     The Namespace type represents a set of vectors stored in turbopuffer.
@@ -237,15 +237,15 @@
     @overload
     def query(self,
               vector: Optional[List[float]] = None,
               distance_metric: Optional[str] = None,
               top_k: int = 10,
               include_vectors: bool = False,
               include_attributes: Optional[Union[List[str], bool]] = None,
-              filters: Optional[Dict[str, List[FilterTuple]]] = None) -> VectorResult:
+              filters: Optional[Filters] = None) -> VectorResult:
         ...
 
     @overload
     def query(self, query_data: VectorQuery) -> VectorResult:
         ...
 
     @overload
```

### Comparing `turbopuffer-0.1.8/turbopuffer/vectors.py` & `turbopuffer-0.1.9/turbopuffer/vectors.py`

 * *Files identical despite different names*

### Comparing `turbopuffer-0.1.8/PKG-INFO` & `turbopuffer-0.1.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: turbopuffer
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python Client for accessing the turbopuffer API
 Home-page: https://turbopuffer.com
 License: MIT
 Keywords: turbopuffer,vector,database,cloud
 Author: turbopuffer Inc.
 Author-email: info@turbopuffer.com
-Maintainer: Jacob Wirth
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: System Administrators
@@ -87,15 +86,18 @@
 )
 
 # Query your dataset
 vectors = ns.query(
     vector=[0.15, 0.22],
     distance_metric='cosine_distance',
     top_k=10,
-    filters={ 'name': [['Glob', 'foo*'], ['NotEq', 'food']] },
+    filters=['And', [
+        ['name', 'Glob', 'foo*'],
+        ['name', 'NotEq', 'food'],
+    ]],
     include_attributes=['name'],
     include_vectors=True
 )
 print(vectors)
 # [
 #   VectorRow(id=2, vector=[0.30000001192092896, 0.4000000059604645], attributes={'name': 'foos'}, dist=0.001016080379486084),
 #   VectorRow(id=1, vector=[0.10000000149011612, 0.20000000298023224], attributes={'name': 'foo'}, dist=0.009067952632904053)
```

