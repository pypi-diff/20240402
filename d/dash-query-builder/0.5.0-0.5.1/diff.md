# Comparing `tmp/dash_query_builder-0.5.0.tar.gz` & `tmp/dash_query_builder-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash_query_builder-0.5.0.tar", max compression
+gzip compressed data, was "dash_query_builder-0.5.1.tar", max compression
```

## Comparing `dash_query_builder-0.5.0.tar` & `dash_query_builder-0.5.1.tar`

### file list

```diff
@@ -1,10 +1,26 @@
--rw-r--r--   0        0        0     1053 2024-04-01 16:21:49.619114 dash_query_builder-0.5.0/LICENSE
--rw-r--r--   0        0        0     2687 2024-04-01 16:21:49.883113 dash_query_builder-0.5.0/dash_query_builder/__init__.py
--rw-r--r--   0        0        0       84 2024-04-01 16:21:49.879113 dash_query_builder-0.5.0/dash_query_builder/_imports_.py
--rw-r--r--   0        0        0     1880 2024-04-01 16:21:50.611109 dash_query_builder-0.5.0/dash_query_builder/where_parser/__init__.py
--rw-r--r--   0        0        0    16126 2024-04-01 16:21:50.623109 dash_query_builder-0.5.0/dash_query_builder/where_parser/actions.py
--rw-r--r--   0        0        0     6389 2024-04-01 16:21:50.659109 dash_query_builder-0.5.0/dash_query_builder/where_parser/constants.py
--rw-r--r--   0        0        0     1659 2024-04-01 16:21:50.671109 dash_query_builder-0.5.0/dash_query_builder/where_parser/operators.py
--rw-r--r--   0        0        0     3141 2024-04-01 16:21:50.703109 dash_query_builder-0.5.0/dash_query_builder/where_parser/parser_.py
--rw-r--r--   0        0        0     1150 2024-04-01 16:21:49.619114 dash_query_builder-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      954 1970-01-01 00:00:00.000000 dash_query_builder-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1053 2024-04-02 15:19:11.124567 dash_query_builder-0.5.1/LICENSE
+-rw-r--r--   0        0        0     4415 2024-04-02 15:19:12.184556 dash_query_builder-0.5.1/dash_query_builder/DashQueryBuilder.py
+-rw-r--r--   0        0        0     2687 2024-04-02 15:19:11.596562 dash_query_builder-0.5.1/dash_query_builder/__init__.py
+-rw-r--r--   0        0        0       84 2024-04-02 15:19:11.580562 dash_query_builder-0.5.1/dash_query_builder/_imports_.py
+-rw-r--r--   0        0        0   762844 2024-04-02 15:19:11.732560 dash_query_builder-0.5.1/dash_query_builder/async-antd.min.js
+-rw-r--r--   0        0        0      149 2024-04-02 15:19:11.640561 dash_query_builder-0.5.1/dash_query_builder/async-antd.min.js.LICENSE.txt
+-rw-r--r--   0        0        0  3129007 2024-04-02 15:19:11.724561 dash_query_builder-0.5.1/dash_query_builder/async-antd.min.js.map
+-rw-r--r--   0        0        0     3806 2024-04-02 15:19:11.772560 dash_query_builder-0.5.1/dash_query_builder/async-basic.min.js
+-rw-r--r--   0        0        0     1647 2024-04-02 15:19:11.776560 dash_query_builder-0.5.1/dash_query_builder/async-basic.min.js.map
+-rw-r--r--   0        0        0  1096429 2024-04-02 15:19:11.876559 dash_query_builder-0.5.1/dash_query_builder/async-bootstrap.min.js
+-rw-r--r--   0        0        0  2585885 2024-04-02 15:19:11.904559 dash_query_builder-0.5.1/dash_query_builder/async-bootstrap.min.js.map
+-rw-r--r--   0        0        0   429867 2024-04-02 15:19:11.996558 dash_query_builder-0.5.1/dash_query_builder/async-mui.min.js
+-rw-r--r--   0        0        0      731 2024-04-02 15:19:11.920559 dash_query_builder-0.5.1/dash_query_builder/async-mui.min.js.LICENSE.txt
+-rw-r--r--   0        0        0  2169836 2024-04-02 15:19:12.024557 dash_query_builder-0.5.1/dash_query_builder/async-mui.min.js.map
+-rw-r--r--   0        0        0   772581 2024-04-02 15:19:12.124556 dash_query_builder-0.5.1/dash_query_builder/dash_query_builder.min.js
+-rw-r--r--   0        0        0      815 2024-04-02 15:19:12.064557 dash_query_builder-0.5.1/dash_query_builder/dash_query_builder.min.js.LICENSE.txt
+-rw-r--r--   0        0        0  3020693 2024-04-02 15:19:12.136556 dash_query_builder-0.5.1/dash_query_builder/dash_query_builder.min.js.map
+-rw-r--r--   0        0        0     5459 2024-04-02 15:19:12.192556 dash_query_builder-0.5.1/dash_query_builder/metadata.json
+-rw-r--r--   0        0        0     2599 2024-04-02 15:19:12.232555 dash_query_builder-0.5.1/dash_query_builder/package.json
+-rw-r--r--   0        0        0     1880 2024-04-02 15:19:12.328554 dash_query_builder-0.5.1/dash_query_builder/where_parser/__init__.py
+-rw-r--r--   0        0        0    16126 2024-04-02 15:19:12.352554 dash_query_builder-0.5.1/dash_query_builder/where_parser/actions.py
+-rw-r--r--   0        0        0     6389 2024-04-02 15:19:12.376554 dash_query_builder-0.5.1/dash_query_builder/where_parser/constants.py
+-rw-r--r--   0        0        0     1659 2024-04-02 15:19:12.404554 dash_query_builder-0.5.1/dash_query_builder/where_parser/operators.py
+-rw-r--r--   0        0        0     3141 2024-04-02 15:19:12.428553 dash_query_builder-0.5.1/dash_query_builder/where_parser/parser_.py
+-rw-r--r--   0        0        0     1150 2024-04-02 15:19:11.312565 dash_query_builder-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0      954 1970-01-01 00:00:00.000000 dash_query_builder-0.5.1/PKG-INFO
```

### Comparing `dash_query_builder-0.5.0/LICENSE` & `dash_query_builder-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dash_query_builder-0.5.0/dash_query_builder/__init__.py` & `dash_query_builder-0.5.1/dash_query_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `dash_query_builder-0.5.0/dash_query_builder/where_parser/__init__.py` & `dash_query_builder-0.5.1/dash_query_builder/where_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `dash_query_builder-0.5.0/dash_query_builder/where_parser/actions.py` & `dash_query_builder-0.5.1/dash_query_builder/where_parser/actions.py`

 * *Files identical despite different names*

### Comparing `dash_query_builder-0.5.0/dash_query_builder/where_parser/constants.py` & `dash_query_builder-0.5.1/dash_query_builder/where_parser/constants.py`

 * *Files identical despite different names*

### Comparing `dash_query_builder-0.5.0/dash_query_builder/where_parser/operators.py` & `dash_query_builder-0.5.1/dash_query_builder/where_parser/operators.py`

 * *Files identical despite different names*

### Comparing `dash_query_builder-0.5.0/dash_query_builder/where_parser/parser_.py` & `dash_query_builder-0.5.1/dash_query_builder/where_parser/parser_.py`

 * *Files identical despite different names*

### Comparing `dash_query_builder-0.5.0/pyproject.toml` & `dash_query_builder-0.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dash-query-builder"
-version = "0.5.0"
+version = "0.5.1"
 description = "Dash Component based on react-awesome-query-builder"
 authors = ["Tyler Baur <baur.tyler@protonmail.com>"]
 license = "MIT"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Framework :: Dash",
     "Programming Language :: Python :: 3.8",
```

### Comparing `dash_query_builder-0.5.0/PKG-INFO` & `dash_query_builder-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash-query-builder
-Version: 0.5.0
+Version: 0.5.1
 Summary: Dash Component based on react-awesome-query-builder
 License: MIT
 Author: Tyler Baur
 Author-email: baur.tyler@protonmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Dash
```

