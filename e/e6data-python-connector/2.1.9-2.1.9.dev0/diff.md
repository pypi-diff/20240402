# Comparing `tmp/e6data-python-connector-2.1.9.tar.gz` & `tmp/e6data-python-connector-2.1.9.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e6data-python-connector-2.1.9.tar", last modified: Thu Feb  1 07:48:01 2024, max compression
+gzip compressed data, was "e6data-python-connector-2.1.9.dev0.tar", last modified: Wed Mar 13 09:04:23 2024, max compression
```

## Comparing `e6data-python-connector-2.1.9.tar` & `e6data-python-connector-2.1.9.dev0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 vishalanand   (501) staff       (20)        0 2024-02-01 07:48:01.689676 e6data-python-connector-2.1.9/
--rw-r--r--   0 vishalanand   (501) staff       (20)    11357 2023-09-18 08:03:34.000000 e6data-python-connector-2.1.9/LICENSE
--rw-r--r--   0 vishalanand   (501) staff       (20)       55 2023-09-18 08:03:34.000000 e6data-python-connector-2.1.9/MANIFEST.in
--rw-r--r--   0 vishalanand   (501) staff       (20)     6941 2024-02-01 07:48:01.689312 e6data-python-connector-2.1.9/PKG-INFO
--rw-r--r--   0 vishalanand   (501) staff       (20)     6030 2024-02-01 07:45:58.000000 e6data-python-connector-2.1.9/README.md
-drwxr-xr-x   0 vishalanand   (501) staff       (20)        0 2024-02-01 07:48:01.613266 e6data-python-connector-2.1.9/e6data_python_connector/
--rw-r--r--   0 vishalanand   (501) staff       (20)      103 2023-09-18 08:03:34.000000 e6data-python-connector-2.1.9/e6data_python_connector/__init__.py
--rw-r--r--   0 vishalanand   (501) staff       (20)     9976 2023-12-11 15:43:06.000000 e6data-python-connector-2.1.9/e6data_python_connector/common.py
--rw-r--r--   0 vishalanand   (501) staff       (20)      682 2023-09-18 08:03:34.000000 e6data-python-connector-2.1.9/e6data_python_connector/constants.py
--rw-r--r--   0 vishalanand   (501) staff       (20)    11498 2024-02-01 07:45:32.000000 e6data-python-connector-2.1.9/e6data_python_connector/datainputstream.py
--rw-r--r--   0 vishalanand   (501) staff       (20)    13623 2023-09-18 08:03:34.000000 e6data-python-connector-2.1.9/e6data_python_connector/date_time_utils.py
--rw-r--r--   0 vishalanand   (501) staff       (20)    11209 2024-01-30 03:52:48.000000 e6data-python-connector-2.1.9/e6data_python_connector/dialect.py
--rw-r--r--   0 vishalanand   (501) staff       (20)    24167 2024-01-30 04:38:45.000000 e6data-python-connector-2.1.9/e6data_python_connector/e6data_grpc.py
-drwxr-xr-x   0 vishalanand   (501) staff       (20)        0 2024-02-01 07:48:01.647762 e6data-python-connector-2.1.9/e6data_python_connector/e6x_vector/
--rw-r--r--   0 vishalanand   (501) staff       (20)       34 2023-12-07 17:22:03.000000 e6data-python-connector-2.1.9/e6data_python_connector/e6x_vector/__init__.py
--rw-r--r--   0 vishalanand   (501) staff       (20)      366 2023-12-07 17:22:03.000000 e6data-python-connector-2.1.9/e6data_python_connector/e6x_vector/constants.py
--rw-r--r--   0 vishalanand   (501) staff       (20)    54197 2023-12-07 17:22:03.000000 e6data-python-connector-2.1.9/e6data_python_connector/e6x_vector/ttypes.py
--rw-r--r--   0 vishalanand   (501) staff       (20)      382 2023-09-18 08:03:34.000000 e6data-python-connector-2.1.9/e6data_python_connector/exceptions.py
-drwxr-xr-x   0 vishalanand   (501) staff       (20)        0 2024-02-01 07:48:01.687351 e6data-python-connector-2.1.9/e6data_python_connector/server/
--rw-r--r--   0 vishalanand   (501) staff       (20)   198503 2023-12-07 17:22:03.000000 e6data-python-connector-2.1.9/e6data_python_connector/server/QueryEngineService.py
--rw-r--r--   0 vishalanand   (501) staff       (20)       56 2023-10-19 09:48:55.000000 e6data-python-connector-2.1.9/e6data_python_connector/server/__init__.py
--rw-r--r--   0 vishalanand   (501) staff       (20)      366 2023-12-07 17:22:03.000000 e6data-python-connector-2.1.9/e6data_python_connector/server/constants.py
--rw-r--r--   0 vishalanand   (501) staff       (20)    16340 2024-01-08 12:08:22.000000 e6data-python-connector-2.1.9/e6data_python_connector/server/e6x_engine_pb2.py
--rw-r--r--   0 vishalanand   (501) staff       (20)    18693 2024-01-08 12:08:22.000000 e6data-python-connector-2.1.9/e6data_python_connector/server/e6x_engine_pb2.pyi
--rw-r--r--   0 vishalanand   (501) staff       (20)    46671 2024-01-08 12:08:22.000000 e6data-python-connector-2.1.9/e6data_python_connector/server/e6x_engine_pb2_grpc.py
--rw-r--r--   0 vishalanand   (501) staff       (20)    21227 2023-12-07 17:22:03.000000 e6data-python-connector-2.1.9/e6data_python_connector/server/ttypes.py
--rw-r--r--   0 vishalanand   (501) staff       (20)     1777 2023-09-18 08:03:34.000000 e6data-python-connector-2.1.9/e6data_python_connector/typeId.py
-drwxr-xr-x   0 vishalanand   (501) staff       (20)        0 2024-02-01 07:48:01.688482 e6data-python-connector-2.1.9/e6data_python_connector.egg-info/
--rw-r--r--   0 vishalanand   (501) staff       (20)     6941 2024-02-01 07:48:01.000000 e6data-python-connector-2.1.9/e6data_python_connector.egg-info/PKG-INFO
--rw-r--r--   0 vishalanand   (501) staff       (20)     1160 2024-02-01 07:48:01.000000 e6data-python-connector-2.1.9/e6data_python_connector.egg-info/SOURCES.txt
--rw-r--r--   0 vishalanand   (501) staff       (20)        1 2024-02-01 07:48:01.000000 e6data-python-connector-2.1.9/e6data_python_connector.egg-info/dependency_links.txt
--rw-r--r--   0 vishalanand   (501) staff       (20)       77 2024-02-01 07:48:01.000000 e6data-python-connector-2.1.9/e6data_python_connector.egg-info/entry_points.txt
--rw-r--r--   0 vishalanand   (501) staff       (20)       97 2024-02-01 07:48:01.000000 e6data-python-connector-2.1.9/e6data_python_connector.egg-info/requires.txt
--rw-r--r--   0 vishalanand   (501) staff       (20)       24 2024-02-01 07:48:01.000000 e6data-python-connector-2.1.9/e6data_python_connector.egg-info/top_level.txt
--rw-r--r--   0 vishalanand   (501) staff       (20)       64 2023-09-18 08:03:34.000000 e6data-python-connector-2.1.9/pyproject.toml
--rw-r--r--   0 vishalanand   (501) staff       (20)       73 2024-02-01 07:48:01.692294 e6data-python-connector-2.1.9/setup.cfg
--rw-r--r--   0 vishalanand   (501) staff       (20)     1936 2024-02-01 07:45:58.000000 e6data-python-connector-2.1.9/setup.py
+drwxr-xr-x   0 vishalanand   (501) staff       (20)        0 2024-03-13 09:04:23.846603 e6data-python-connector-2.1.9.dev0/
+-rw-r--r--   0 vishalanand   (501) staff       (20)    11357 2023-09-18 08:03:34.000000 e6data-python-connector-2.1.9.dev0/LICENSE
+-rw-r--r--   0 vishalanand   (501) staff       (20)       55 2023-09-18 08:03:34.000000 e6data-python-connector-2.1.9.dev0/MANIFEST.in
+-rw-r--r--   0 vishalanand   (501) staff       (20)     6947 2024-03-13 09:04:23.846221 e6data-python-connector-2.1.9.dev0/PKG-INFO
+-rw-r--r--   0 vishalanand   (501) staff       (20)     6031 2024-02-02 09:28:37.000000 e6data-python-connector-2.1.9.dev0/README.md
+drwxr-xr-x   0 vishalanand   (501) staff       (20)        0 2024-03-13 09:04:23.760761 e6data-python-connector-2.1.9.dev0/e6data_python_connector/
+-rw-r--r--   0 vishalanand   (501) staff       (20)      103 2023-09-18 08:03:34.000000 e6data-python-connector-2.1.9.dev0/e6data_python_connector/__init__.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)     9976 2023-12-11 15:43:06.000000 e6data-python-connector-2.1.9.dev0/e6data_python_connector/common.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)      682 2023-09-18 08:03:34.000000 e6data-python-connector-2.1.9.dev0/e6data_python_connector/constants.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)    11746 2024-03-13 09:02:41.000000 e6data-python-connector-2.1.9.dev0/e6data_python_connector/datainputstream.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)    13623 2023-09-18 08:03:34.000000 e6data-python-connector-2.1.9.dev0/e6data_python_connector/date_time_utils.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)    11177 2024-02-02 09:28:17.000000 e6data-python-connector-2.1.9.dev0/e6data_python_connector/dialect.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)    25679 2024-03-13 09:02:41.000000 e6data-python-connector-2.1.9.dev0/e6data_python_connector/e6data_grpc.py
+drwxr-xr-x   0 vishalanand   (501) staff       (20)        0 2024-03-13 09:04:23.798315 e6data-python-connector-2.1.9.dev0/e6data_python_connector/e6x_vector/
+-rw-r--r--   0 vishalanand   (501) staff       (20)       34 2023-12-07 17:22:03.000000 e6data-python-connector-2.1.9.dev0/e6data_python_connector/e6x_vector/__init__.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)      366 2023-12-07 17:22:03.000000 e6data-python-connector-2.1.9.dev0/e6data_python_connector/e6x_vector/constants.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)    54197 2023-12-07 17:22:03.000000 e6data-python-connector-2.1.9.dev0/e6data_python_connector/e6x_vector/ttypes.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)      382 2023-09-18 08:03:34.000000 e6data-python-connector-2.1.9.dev0/e6data_python_connector/exceptions.py
+drwxr-xr-x   0 vishalanand   (501) staff       (20)        0 2024-03-13 09:04:23.842648 e6data-python-connector-2.1.9.dev0/e6data_python_connector/server/
+-rw-r--r--   0 vishalanand   (501) staff       (20)   198503 2023-12-07 17:22:03.000000 e6data-python-connector-2.1.9.dev0/e6data_python_connector/server/QueryEngineService.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)       56 2023-10-19 09:48:55.000000 e6data-python-connector-2.1.9.dev0/e6data_python_connector/server/__init__.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)      366 2023-12-07 17:22:03.000000 e6data-python-connector-2.1.9.dev0/e6data_python_connector/server/constants.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)    16340 2024-01-08 12:08:22.000000 e6data-python-connector-2.1.9.dev0/e6data_python_connector/server/e6x_engine_pb2.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)    18693 2024-01-08 12:08:22.000000 e6data-python-connector-2.1.9.dev0/e6data_python_connector/server/e6x_engine_pb2.pyi
+-rw-r--r--   0 vishalanand   (501) staff       (20)    46671 2024-01-08 12:08:22.000000 e6data-python-connector-2.1.9.dev0/e6data_python_connector/server/e6x_engine_pb2_grpc.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)    21227 2023-12-07 17:22:03.000000 e6data-python-connector-2.1.9.dev0/e6data_python_connector/server/ttypes.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)     1777 2023-09-18 08:03:34.000000 e6data-python-connector-2.1.9.dev0/e6data_python_connector/typeId.py
+drwxr-xr-x   0 vishalanand   (501) staff       (20)        0 2024-03-13 09:04:23.845075 e6data-python-connector-2.1.9.dev0/e6data_python_connector.egg-info/
+-rw-r--r--   0 vishalanand   (501) staff       (20)     6947 2024-03-13 09:04:23.000000 e6data-python-connector-2.1.9.dev0/e6data_python_connector.egg-info/PKG-INFO
+-rw-r--r--   0 vishalanand   (501) staff       (20)     1160 2024-03-13 09:04:23.000000 e6data-python-connector-2.1.9.dev0/e6data_python_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 vishalanand   (501) staff       (20)        1 2024-03-13 09:04:23.000000 e6data-python-connector-2.1.9.dev0/e6data_python_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 vishalanand   (501) staff       (20)       77 2024-03-13 09:04:23.000000 e6data-python-connector-2.1.9.dev0/e6data_python_connector.egg-info/entry_points.txt
+-rw-r--r--   0 vishalanand   (501) staff       (20)       97 2024-03-13 09:04:23.000000 e6data-python-connector-2.1.9.dev0/e6data_python_connector.egg-info/requires.txt
+-rw-r--r--   0 vishalanand   (501) staff       (20)       24 2024-03-13 09:04:23.000000 e6data-python-connector-2.1.9.dev0/e6data_python_connector.egg-info/top_level.txt
+-rw-r--r--   0 vishalanand   (501) staff       (20)       64 2023-09-18 08:03:34.000000 e6data-python-connector-2.1.9.dev0/pyproject.toml
+-rw-r--r--   0 vishalanand   (501) staff       (20)       73 2024-03-13 09:04:23.851199 e6data-python-connector-2.1.9.dev0/setup.cfg
+-rw-r--r--   0 vishalanand   (501) staff       (20)     1943 2024-03-13 09:03:22.000000 e6data-python-connector-2.1.9.dev0/setup.py
```

### Comparing `e6data-python-connector-2.1.9/LICENSE` & `e6data-python-connector-2.1.9.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `e6data-python-connector-2.1.9/PKG-INFO` & `e6data-python-connector-2.1.9.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e6data-python-connector
-Version: 2.1.9
+Version: 2.1.9.dev0
 Summary: Client for the e6data distributed SQL Engine.
 Home-page: https://github.com/e6x-labs/e6data-python-connector
 Author: Uniphi, Inc.
 Author-email: info@e6data.com
 License: Apache 2.0
 Classifier: Operating System :: POSIX :: Linux
 Classifier: License :: OSI Approved :: Apache Software License
@@ -23,15 +23,15 @@
 Requires-Dist: thrift
 Requires-Dist: grpcio
 Requires-Dist: grpcio-tools
 Requires-Dist: sqlalchemy
 
 # e6data Python Connector
 
-![version](https://img.shields.io/badge/version-2.1.9-blue.svg)
+![version](https://img.shields.io/badge/version-2.1.10-blue.svg)
 
 ## Introduction
 
 The e6data Connector for Python provides an interface for writing Python applications that can connect to e6data and perform operations.
 
 ### Dependencies
 Make sure to install below dependencies and wheel before install e6data-python-connector.
```

### Comparing `e6data-python-connector-2.1.9/README.md` & `e6data-python-connector-2.1.9.dev0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # e6data Python Connector
 
-![version](https://img.shields.io/badge/version-2.1.9-blue.svg)
+![version](https://img.shields.io/badge/version-2.1.10-blue.svg)
 
 ## Introduction
 
 The e6data Connector for Python provides an interface for writing Python applications that can connect to e6data and perform operations.
 
 ### Dependencies
 Make sure to install below dependencies and wheel before install e6data-python-connector.
```

### Comparing `e6data-python-connector-2.1.9/e6data_python_connector/common.py` & `e6data-python-connector-2.1.9.dev0/e6data_python_connector/common.py`

 * *Files identical despite different names*

### Comparing `e6data-python-connector-2.1.9/e6data_python_connector/constants.py` & `e6data-python-connector-2.1.9.dev0/e6data_python_connector/constants.py`

 * *Files identical despite different names*

### Comparing `e6data-python-connector-2.1.9/e6data_python_connector/datainputstream.py` & `e6data-python-connector-2.1.9.dev0/e6data_python_connector/datainputstream.py`

 * *Files 8% similar despite different names*

```diff
@@ -170,24 +170,32 @@
         except Exception as e:
             _logger.error(e)
             value_array.append('Failed to parse.')
 
     return value_array
 
 
-def read_rows_from_chunk(query_columns_description: list, buffer):
+def reconstruct_chunk(buffer):
     # Create a transport and protocol instance for deserialization
     transport = TTransport.TMemoryBuffer(buffer)
     protocol = TBinaryProtocol.TBinaryProtocolAccelerated(transport)
 
     # Create an instance of the Thrift struct and read from the protocol
     chunk = Chunk()
     chunk.read(protocol)
+    return chunk
+
+
+def read_rows_from_chunk(query_columns_description: list, buffer):
+    chunk = reconstruct_chunk(buffer)
+    return deserialize_chunk_to_rows(query_columns_description, chunk)
+
 
-    if chunk.size <= 0:
+def deserialize_chunk_to_rows(query_columns_description: list, chunk):
+    if chunk is None or chunk.size <= 0:
         return None
 
     rows = list()
     columns = list()
 
     for col, colName in enumerate(query_columns_description):
         columns.append(get_column_from_chunk(chunk.vectors[col]))
```

### Comparing `e6data-python-connector-2.1.9/e6data_python_connector/date_time_utils.py` & `e6data-python-connector-2.1.9.dev0/e6data_python_connector/date_time_utils.py`

 * *Files identical despite different names*

### Comparing `e6data-python-connector-2.1.9/e6data_python_connector/dialect.py` & `e6data-python-connector-2.1.9.dev0/e6data_python_connector/dialect.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,43 +210,43 @@
     supports_multivalues_insert = True
     type_compiler = E6dataTypeCompiler
     supports_sane_rowcount = False
     driver = 'e6data'
     scheme = 'e6data'
     catalog_name = None
     cluster_uuid = None
-    secure_channel = False
+    secure = False
 
     def _dialect_specific_select_one(self):
         return "NOOP"
 
     @classmethod
     def dbapi(cls):
         return e6data_grpc
 
     def create_connect_args(self, url):
         database = None
         if url.query.get("schema"):
             database = url.query.get("schema")
         self.catalog_name = url.query.get("catalog")
         self.cluster_uuid = url.query.get("cluster-uuid")
-        self.secure_channel = url.query.get("secure") == 'true'
+        self.secure = url.query.get("secure") == 'true'
         if not self.catalog_name:
             raise Exception('Please specify catalog in query parameter.')
 
         kwargs = {
             "host": url.host,
             "port": url.port,
             "scheme": self.scheme,
             "username": url.username or None,
             "password": url.password or None,
             "database": database,
             "catalog": self.catalog_name,
             "cluster_uuid": self.cluster_uuid,
-            'secure_channel': self.secure_channel
+            'secure': self.secure
         }
         return [], kwargs
 
     def get_schema_names(self, connection, **kw):
         # Equivalent to SHOW DATABASES
         # Rerouting to view names
         if isinstance(connection, Engine):
```

### Comparing `e6data-python-connector-2.1.9/e6data_python_connector/e6data_grpc.py` & `e6data-python-connector-2.1.9.dev0/e6data_python_connector/e6data_grpc.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 from io import BytesIO
 from ssl import CERT_NONE, CERT_OPTIONAL, CERT_REQUIRED
 
 import grpc
 
 from e6data_python_connector.common import DBAPITypeObject, ParamEscaper, DBAPICursor
 from e6data_python_connector.constants import *
-from e6data_python_connector.datainputstream import get_query_columns_info, read_rows_from_chunk
+from e6data_python_connector.datainputstream import get_query_columns_info, read_rows_from_chunk, reconstruct_chunk, \
+    deserialize_chunk_to_rows
 from e6data_python_connector.server import e6x_engine_pb2_grpc, e6x_engine_pb2
 from e6data_python_connector.typeId import *
 
 apilevel = '2.0'
 threadsafety = 2  # Threads may share the e6xdb and connections.
 paramstyle = 'pyformat'  # Python extended format codes, e.g. ...WHERE name=%(name)s
 
@@ -68,19 +69,19 @@
         # Newer SQLAlchemy checks dialect.supports_unicode_binds before encoding Unicode strings
         # as byte strings. The old version always encodes Unicode as byte strings, which breaks
         # string formatting here.
         if isinstance(item, bytes):
             item = item.decode('utf-8')
         return "'{}'".format(
             item
-            .replace('\\', '\\\\')
-            .replace("'", "\\'")
-            .replace('\r', '\\r')
-            .replace('\n', '\\n')
-            .replace('\t', '\\t')
+                .replace('\\', '\\\\')
+                .replace("'", "\\'")
+                .replace('\r', '\\r')
+                .replace('\n', '\\n')
+                .replace('\t', '\\t')
         )
 
 
 _escaper = HiveParamEscaper()
 
 
 def _get_grpc_header(engine_ip=None, cluster=None):
@@ -515,23 +516,22 @@
                 sessionId=self.connection.get_session_id,
                 queryId=self._query_id
             )
             client.executeStatementV2(
                 execute_statement_request,
                 metadata=self.metadata
             )
-        self.update_mete_data()
+        self.update_meta_data()
         return self._query_id
 
     @property
     def rowcount(self):
-        self.update_mete_data()
         return self._rowcount
 
-    def update_mete_data(self):
+    def update_meta_data(self):
         result_meta_data_request = e6x_engine_pb2.GetResultMetadataRequest(
             engineIP=self._engine_ip,
             sessionId=self.connection.get_session_id,
             queryId=self._query_id
         )
         get_result_metadata_response = self.connection.client.getResultMetadata(
             result_meta_data_request,
@@ -567,38 +567,53 @@
             self._query_id = query_id
         while True:
             rows = self.fetch_batch()
             if not rows:
                 return
             yield rows
 
-    def fetch_batch(self):
+    def get_next_batch(self):
         client = self.connection.client
         get_next_result_batch_request = e6x_engine_pb2.GetNextResultBatchRequest(
             engineIP=self._engine_ip,
             sessionId=self.connection.get_session_id,
             queryId=self._query_id
         )
         get_next_result_batch_response = client.getNextResultBatch(
             get_next_result_batch_request,
             metadata=self.metadata
         )
         buffer = get_next_result_batch_response.resultBatch
         if not self._is_metadata_updated:
-            self.update_mete_data()
+            self.update_meta_data()
         if not buffer or len(buffer) == 0:
             return None
+        return buffer
+
+    def fetch_batch(self):
+        buffer = self.get_next_batch()
         # one batch retrieves the predefined set of rows
         return read_rows_from_chunk(self._query_columns_description, buffer)
 
+    def fetch_all_columnar(self):
+        list_chunk = list()
+        while True:
+            buffer = self.get_next_batch()
+            if buffer is None:
+                break
+            chunk = reconstruct_chunk(buffer)
+            list_chunk.append(chunk)
+        result = ColumnarResult(list_chunk, self._query_columns_description)
+        return result
+
     def fetchall(self):
         return self._fetch_all()
 
     def fetchmany(self, size: int = None):
-        # _logger.info("fetching all from overriden method")
+        # _logger.info("fetching all from overridden method")
         if size is None:
             size = self.arraysize
         if self._data is None:
             self._data = list()
         while len(self._data) < size:
             rows = self.fetch_batch()
             if rows is None:
@@ -670,14 +685,43 @@
     pass
 
 
 class Error(Exception):
     pass
 
 
+class ColumnarResult:
+    def __init__(self, list_chunk, list_column_description):
+        self.rows = None
+        self._list_chunk = list_chunk
+        self._cur_chunk = None
+        self._list_column_description = list_column_description
+        self._cur_chunk_index = 0
+        self._cur_chunk_row_idx = 0
+
+    def get_next_row(self):
+        if self._cur_chunk is None or self._cur_chunk_row_idx >= self._cur_chunk.size:
+            self.move_to_next_chunk()
+            self.rows = deserialize_chunk_to_rows(self._list_column_description, self._cur_chunk)
+            _cur_chunk_row_idx = 0
+        if self._cur_chunk is None:
+            return None
+        row = self.rows[self._cur_chunk_row_idx]
+        self._cur_chunk_row_idx += 1
+        return row
+
+    def move_to_next_chunk(self):
+        if self._cur_chunk_index >= len(self._list_chunk):
+            self._cur_chunk = None
+
+        else:
+            self._cur_chunk = self._list_chunk[self._cur_chunk_index]
+            self._cur_chunk_index += 1
+
+
 #
 # Type Objects and Constructors
 #
 
 for type_id in PRIMITIVE_TYPES:
     name = TypeId._VALUES_TO_NAMES[type_id]
     setattr(sys.modules[__name__], name, DBAPITypeObject([name]))
```

### Comparing `e6data-python-connector-2.1.9/e6data_python_connector/e6x_vector/ttypes.py` & `e6data-python-connector-2.1.9.dev0/e6data_python_connector/e6x_vector/ttypes.py`

 * *Files identical despite different names*

### Comparing `e6data-python-connector-2.1.9/e6data_python_connector/server/QueryEngineService.py` & `e6data-python-connector-2.1.9.dev0/e6data_python_connector/server/QueryEngineService.py`

 * *Files identical despite different names*

### Comparing `e6data-python-connector-2.1.9/e6data_python_connector/server/e6x_engine_pb2.py` & `e6data-python-connector-2.1.9.dev0/e6data_python_connector/server/e6x_engine_pb2.py`

 * *Files identical despite different names*

### Comparing `e6data-python-connector-2.1.9/e6data_python_connector/server/e6x_engine_pb2.pyi` & `e6data-python-connector-2.1.9.dev0/e6data_python_connector/server/e6x_engine_pb2.pyi`

 * *Files identical despite different names*

### Comparing `e6data-python-connector-2.1.9/e6data_python_connector/server/e6x_engine_pb2_grpc.py` & `e6data-python-connector-2.1.9.dev0/e6data_python_connector/server/e6x_engine_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `e6data-python-connector-2.1.9/e6data_python_connector/server/ttypes.py` & `e6data-python-connector-2.1.9.dev0/e6data_python_connector/server/ttypes.py`

 * *Files identical despite different names*

### Comparing `e6data-python-connector-2.1.9/e6data_python_connector/typeId.py` & `e6data-python-connector-2.1.9.dev0/e6data_python_connector/typeId.py`

 * *Files identical despite different names*

### Comparing `e6data-python-connector-2.1.9/e6data_python_connector.egg-info/PKG-INFO` & `e6data-python-connector-2.1.9.dev0/e6data_python_connector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e6data-python-connector
-Version: 2.1.9
+Version: 2.1.9.dev0
 Summary: Client for the e6data distributed SQL Engine.
 Home-page: https://github.com/e6x-labs/e6data-python-connector
 Author: Uniphi, Inc.
 Author-email: info@e6data.com
 License: Apache 2.0
 Classifier: Operating System :: POSIX :: Linux
 Classifier: License :: OSI Approved :: Apache Software License
@@ -23,15 +23,15 @@
 Requires-Dist: thrift
 Requires-Dist: grpcio
 Requires-Dist: grpcio-tools
 Requires-Dist: sqlalchemy
 
 # e6data Python Connector
 
-![version](https://img.shields.io/badge/version-2.1.9-blue.svg)
+![version](https://img.shields.io/badge/version-2.1.10-blue.svg)
 
 ## Introduction
 
 The e6data Connector for Python provides an interface for writing Python applications that can connect to e6data and perform operations.
 
 ### Dependencies
 Make sure to install below dependencies and wheel before install e6data-python-connector.
```

### Comparing `e6data-python-connector-2.1.9/e6data_python_connector.egg-info/SOURCES.txt` & `e6data-python-connector-2.1.9.dev0/e6data_python_connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `e6data-python-connector-2.1.9/setup.py` & `e6data-python-connector-2.1.9.dev0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import setuptools
 
-VERSION = [2, 1, 9]
+VERSION = [2, 1, 9, 'dev']
 
 
 def get_long_desc():
     with open("README.md", "r") as fh:
         long_description = fh.read()
     return long_description
```

