# Comparing `tmp/logs_ingestion-0.2.0.tar.gz` & `tmp/logs_ingestion-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logs_ingestion-0.2.0.tar", max compression
+gzip compressed data, was "logs_ingestion-0.2.1.tar", max compression
```

## Comparing `logs_ingestion-0.2.0.tar` & `logs_ingestion-0.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2299 2024-03-31 16:23:50.662520 logs_ingestion-0.2.0/README.md
--rw-r--r--   0        0        0        0 2024-03-29 21:50:48.811293 logs_ingestion-0.2.0/logs_ingestion/__init__.py
--rw-r--r--   0        0        0     1902 2024-03-31 15:34:00.474787 logs_ingestion-0.2.0/logs_ingestion/logs_adapter.py
--rw-r--r--   0        0        0     1340 2024-03-31 14:50:26.629587 logs_ingestion-0.2.0/logs_ingestion/logs_decorator.py
--rw-r--r--   0        0        0     2262 2024-03-31 16:30:04.954894 logs_ingestion-0.2.0/logs_ingestion/logs_ingestion.py
--rw-r--r--   0        0        0     1524 2024-03-31 15:22:02.349670 logs_ingestion-0.2.0/logs_ingestion/logs_record.py
--rw-r--r--   0        0        0      570 2024-03-31 16:30:33.264070 logs_ingestion-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3027 1970-01-01 00:00:00.000000 logs_ingestion-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     2299 2024-03-31 16:33:10.041001 logs_ingestion-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2024-03-31 16:33:10.041216 logs_ingestion-0.2.1/logs_ingestion/__init__.py
+-rw-r--r--   0        0        0     1902 2024-03-31 16:33:10.041651 logs_ingestion-0.2.1/logs_ingestion/logs_adapter.py
+-rw-r--r--   0        0        0     1340 2024-03-31 16:33:10.041874 logs_ingestion-0.2.1/logs_ingestion/logs_decorator.py
+-rw-r--r--   0        0        0     2262 2024-03-31 16:33:10.041995 logs_ingestion-0.2.1/logs_ingestion/logs_ingestion.py
+-rw-r--r--   0        0        0     1524 2024-03-31 16:33:10.042245 logs_ingestion-0.2.1/logs_ingestion/logs_record.py
+-rw-r--r--   0        0        0      570 2024-03-31 18:35:00.993238 logs_ingestion-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3027 1970-01-01 00:00:00.000000 logs_ingestion-0.2.1/PKG-INFO
```

### Comparing `logs_ingestion-0.2.0/README.md` & `logs_ingestion-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `logs_ingestion-0.2.0/logs_ingestion/logs_adapter.py` & `logs_ingestion-0.2.1/logs_ingestion/logs_adapter.py`

 * *Files identical despite different names*

### Comparing `logs_ingestion-0.2.0/logs_ingestion/logs_decorator.py` & `logs_ingestion-0.2.1/logs_ingestion/logs_decorator.py`

 * *Files identical despite different names*

### Comparing `logs_ingestion-0.2.0/logs_ingestion/logs_ingestion.py` & `logs_ingestion-0.2.1/logs_ingestion/logs_ingestion.py`

 * *Files identical despite different names*

### Comparing `logs_ingestion-0.2.0/logs_ingestion/logs_record.py` & `logs_ingestion-0.2.1/logs_ingestion/logs_record.py`

 * *Files identical despite different names*

### Comparing `logs_ingestion-0.2.0/pyproject.toml` & `logs_ingestion-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "logs-ingestion"
-version = "0.2.0"
+version = "0.2.1"
 description = "Package for logging to Azure Logs Ingestion API using decorators and regular logging statements."
 authors = ["Richard Kooijman <kooijman.richard@gmail.com>"]
 license = "Apache"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `logs_ingestion-0.2.0/PKG-INFO` & `logs_ingestion-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logs-ingestion
-Version: 0.2.0
+Version: 0.2.1
 Summary: Package for logging to Azure Logs Ingestion API using decorators and regular logging statements.
 License: Apache
 Author: Richard Kooijman
 Author-email: kooijman.richard@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

