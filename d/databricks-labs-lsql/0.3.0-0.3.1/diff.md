# Comparing `tmp/databricks_labs_lsql-0.3.0.tar.gz` & `tmp/databricks_labs_lsql-0.3.1.tar.gz`

## Comparing `databricks_labs_lsql-0.3.0.tar` & `databricks_labs_lsql-0.3.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.3.0/databricks/__init__.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.3.0/databricks/labs/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.3.0/databricks/labs/lsql/__about__.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.3.0/databricks/labs/lsql/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.3.0/databricks/labs/lsql/__main__.py
--rw-r--r--   0        0        0    13018 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.3.0/databricks/labs/lsql/backends.py
--rw-r--r--   0        0        0    23637 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.3.0/databricks/labs/lsql/core.py
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.3.0/databricks/labs/lsql/deployment.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.3.0/databricks/labs/lsql/py.typed
--rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.3.0/.gitignore
--rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.3.0/LICENSE
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.3.0/NOTICE
--rw-r--r--   0        0        0     7650 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.3.0/README.md
--rw-r--r--   0        0        0    26430 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     8715 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.3.1/databricks/__init__.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.3.1/databricks/labs/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.3.1/databricks/labs/lsql/__about__.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.3.1/databricks/labs/lsql/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.3.1/databricks/labs/lsql/__main__.py
+-rw-r--r--   0        0        0    13017 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.3.1/databricks/labs/lsql/backends.py
+-rw-r--r--   0        0        0    23637 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.3.1/databricks/labs/lsql/core.py
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.3.1/databricks/labs/lsql/deployment.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.3.1/databricks/labs/lsql/py.typed
+-rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.3.1/.gitignore
+-rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.3.1/LICENSE
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.3.1/NOTICE
+-rw-r--r--   0        0        0     7650 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.3.1/README.md
+-rw-r--r--   0        0        0    26430 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     8715 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.3.1/PKG-INFO
```

### Comparing `databricks_labs_lsql-0.3.0/databricks/labs/lsql/backends.py` & `databricks_labs_lsql-0.3.1/databricks/labs/lsql/backends.py`

 * *Files 1% similar despite different names*

```diff
@@ -235,15 +235,15 @@
     def __init__(self, ws: WorkspaceClient):
         try:
             # pylint: disable-next=import-outside-toplevel
             from databricks.connect import (  # type: ignore[import-untyped]
                 DatabricksSession,
             )
 
-            spark = DatabricksSession.builder.sdk_config(ws.config).getOrCreate()
+            spark = DatabricksSession.builder.sdkConfig(ws.config).getOrCreate()
             super().__init__(spark, ws.config.debug_truncate_bytes)
         except ImportError as e:
             raise RuntimeError("Please run `pip install databricks-connect`") from e
 
 
 class MockBackend(SqlBackend):
     def __init__(
```

### Comparing `databricks_labs_lsql-0.3.0/databricks/labs/lsql/core.py` & `databricks_labs_lsql-0.3.1/databricks/labs/lsql/core.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_lsql-0.3.0/databricks/labs/lsql/deployment.py` & `databricks_labs_lsql-0.3.1/databricks/labs/lsql/deployment.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_lsql-0.3.0/.gitignore` & `databricks_labs_lsql-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `databricks_labs_lsql-0.3.0/LICENSE` & `databricks_labs_lsql-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `databricks_labs_lsql-0.3.0/NOTICE` & `databricks_labs_lsql-0.3.1/NOTICE`

 * *Files identical despite different names*

### Comparing `databricks_labs_lsql-0.3.0/README.md` & `databricks_labs_lsql-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `databricks_labs_lsql-0.3.0/pyproject.toml` & `databricks_labs_lsql-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `databricks_labs_lsql-0.3.0/PKG-INFO` & `databricks_labs_lsql-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: databricks-labs-lsql
-Version: 0.3.0
+Version: 0.3.1
 Summary: Lightweight stateless SQL execution for Databricks with minimal dependencies
 Project-URL: Documentation, https://github.com/databrickslabs/lsql#readme
 Project-URL: Issues, https://github.com/databrickslabs/lsql/issues
 Project-URL: Source, https://github.com/databrickslabs/lsql
 Author-email: Serge Smertin <serge.smertin@databricks.com>
 License-File: LICENSE
 License-File: NOTICE
```

