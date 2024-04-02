# Comparing `tmp/tablestore-5.4.3.tar.gz` & `tmp/tablestore-5.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Tue Feb 27 08:56:51 2024, from Unix
+gzip compressed data, last modified: Tue Apr  2 07:58:25 2024, from Unix
```

## Comparing `tablestore-5.4.3.tar` & `tablestore-5.4.4.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 simply     (502) staff       (20)        0 2024-02-27 08:55:02.000000 tablestore-5.4.3/
--rw-r--r--   0 simply     (502) staff       (20)     6828 2024-02-27 08:55:02.000000 tablestore-5.4.3/PKG-INFO
-drwxr-xr-x   0 simply     (502) staff       (20)        0 2024-02-27 08:55:01.000000 tablestore-5.4.3/tablestore.egg-info/
--rwxr-xr-x   0 simply     (502) staff       (20)     1949 2024-02-27 08:00:50.000000 tablestore-5.4.3/setup.py
-drwxr-xr-x   0 simply     (502) staff       (20)        0 2024-02-27 08:55:01.000000 tablestore-5.4.3/tablestore/
--rw-r--r--   0 simply     (502) staff       (20)       38 2024-02-27 08:55:02.000000 tablestore-5.4.3/setup.cfg
--rw-r--r--   0 simply     (502) staff       (20)     4939 2023-09-01 08:26:14.000000 tablestore-5.4.3/README.rst
--rw-r--r--   0 simply     (502) staff       (20)    36560 2024-02-27 07:52:14.000000 tablestore-5.4.3/tablestore/decoder.py
-drwxr-xr-x   0 simply     (502) staff       (20)        0 2024-02-27 08:55:01.000000 tablestore-5.4.3/tablestore/plainbuffer/
--rw-r--r--   0 simply     (502) staff       (20)     3820 2024-02-27 07:52:14.000000 tablestore-5.4.3/tablestore/aggregation.py
--rw-r--r--   0 simply     (502) staff       (20)    30179 2024-02-27 07:52:14.000000 tablestore-5.4.3/tablestore/metadata.py
--rw-r--r--   0 simply     (502) staff       (20)     1056 2024-02-27 07:52:14.000000 tablestore-5.4.3/tablestore/error.py
--rw-r--r--   0 simply     (502) staff       (20)    11380 2024-02-27 07:52:14.000000 tablestore-5.4.3/tablestore/protocol.py
--rw-r--r--   0 simply     (502) staff       (20)    37223 2024-02-27 07:52:14.000000 tablestore-5.4.3/tablestore/client.py
--rw-r--r--   0 simply     (502) staff       (20)    11575 2024-02-27 07:52:14.000000 tablestore-5.4.3/tablestore/group_by.py
--rw-r--r--   0 simply     (502) staff       (20)     2865 2024-02-27 07:52:14.000000 tablestore-5.4.3/tablestore/__init__.py
--rw-r--r--   0 simply     (502) staff       (20)      827 2024-02-27 07:52:14.000000 tablestore-5.4.3/tablestore/types.py
--rw-r--r--   0 simply     (502) staff       (20)    56288 2024-02-27 07:52:14.000000 tablestore-5.4.3/tablestore/encoder.py
--rw-r--r--   0 simply     (502) staff       (20)     5072 2024-02-27 07:52:14.000000 tablestore-5.4.3/tablestore/retry.py
--rw-r--r--   0 simply     (502) staff       (20)     1836 2024-02-27 07:52:14.000000 tablestore-5.4.3/tablestore/connection.py
-drwxr-xr-x   0 simply     (502) staff       (20)        0 2024-02-27 08:55:01.000000 tablestore-5.4.3/tablestore/flatbuffer/
-drwxr-xr-x   0 simply     (502) staff       (20)        0 2024-02-27 08:55:22.000000 tablestore-5.4.3/tablestore/protobuf/
--rw-r--r--   0 simply     (502) staff       (20)      372 2024-02-27 07:52:14.000000 tablestore-5.4.3/tablestore/const.py
-drwxr-xr-x   0 simply     (502) staff       (20)        0 2024-02-27 08:55:22.000000 tablestore-5.4.3/tablestore/protobuf/py3/
-drwxr-xr-x   0 simply     (502) staff       (20)        0 2024-02-27 08:55:02.000000 tablestore-5.4.3/tablestore/protobuf/py2/
--rw-r--r--   0 simply     (502) staff       (20)    11503 2024-02-27 07:52:14.000000 tablestore-5.4.3/tablestore/protobuf/py2/table_store_filter_pb2.py
--rw-r--r--   0 simply     (502) staff       (20)        0 2024-02-27 07:52:14.000000 tablestore-5.4.3/tablestore/protobuf/py2/__init__.py
--rw-r--r--   0 simply     (502) staff       (20)   164399 2024-02-27 07:52:14.000000 tablestore-5.4.3/tablestore/protobuf/py2/table_store_pb2.py
--rw-r--r--   0 simply     (502) staff       (20)   209501 2024-02-27 07:52:14.000000 tablestore-5.4.3/tablestore/protobuf/py2/search_pb2.py
--rw-r--r--   0 simply     (502) staff       (20)     6840 2024-02-27 08:55:22.000000 tablestore-5.4.3/tablestore/protobuf/py3/._table_store_filter_pb2.py
--rw-r--r--   0 simply     (502) staff       (20)    13500 2024-02-27 08:55:22.376147 tablestore-5.4.3/tablestore/protobuf/py3/table_store_filter_pb2.py
--rw-r--r--   0 simply     (502) staff       (20)        0 2024-02-27 08:55:22.000000 tablestore-5.4.3/tablestore/protobuf/py3/__init__.py
--rw-r--r--   0 simply     (502) staff       (20)   184768 2024-02-27 08:55:22.000000 tablestore-5.4.3/tablestore/protobuf/py3/table_store_pb2.py
--rw-r--r--   0 simply     (502) staff       (20)   234437 2024-02-27 08:55:22.000000 tablestore-5.4.3/tablestore/protobuf/py3/search_pb2.py
--rw-r--r--   0 simply     (502) staff       (20)     2951 2024-02-27 07:52:14.000000 tablestore-5.4.3/tablestore/flatbuffer/flat_buffer_decoder.py
--rw-r--r--   0 simply     (502) staff       (20)        0 2024-02-27 07:52:14.000000 tablestore-5.4.3/tablestore/flatbuffer/__init__.py
-drwxr-xr-x   0 simply     (502) staff       (20)        0 2024-02-27 08:55:01.000000 tablestore-5.4.3/tablestore/flatbuffer/dataprotocol/
--rw-r--r--   0 simply     (502) staff       (20)        0 2024-02-27 07:52:14.000000 tablestore-5.4.3/tablestore/flatbuffer/dataprotocol/__init__.py
--rw-r--r--   0 simply     (502) staff       (20)     5013 2024-02-27 07:52:14.000000 tablestore-5.4.3/tablestore/flatbuffer/dataprotocol/SQLResponseColumns.py
--rw-r--r--   0 simply     (502) staff       (20)     3932 2024-02-27 07:52:14.000000 tablestore-5.4.3/tablestore/flatbuffer/dataprotocol/BytesValue.py
--rw-r--r--   0 simply     (502) staff       (20)     4532 2024-02-27 07:52:14.000000 tablestore-5.4.3/tablestore/flatbuffer/dataprotocol/SQLResponseColumn.py
--rw-r--r--   0 simply     (502) staff       (20)      227 2024-02-27 07:52:14.000000 tablestore-5.4.3/tablestore/flatbuffer/dataprotocol/DataType.py
--rw-r--r--   0 simply     (502) staff       (20)    17063 2024-02-27 07:52:14.000000 tablestore-5.4.3/tablestore/flatbuffer/dataprotocol/ColumnValues.py
--rw-r--r--   0 simply     (502) staff       (20)     6177 2024-02-27 07:52:14.000000 tablestore-5.4.3/tablestore/flatbuffer/dataprotocol/RLEStringValues.py
--rw-r--r--   0 simply     (502) staff       (20)    24014 2024-02-27 07:52:14.000000 tablestore-5.4.3/tablestore/plainbuffer/plain_buffer_coded_stream.py
--rw-r--r--   0 simply     (502) staff       (20)        0 2024-02-27 07:52:14.000000 tablestore-5.4.3/tablestore/plainbuffer/__init__.py
--rw-r--r--   0 simply     (502) staff       (20)     9774 2024-02-27 07:52:14.000000 tablestore-5.4.3/tablestore/plainbuffer/plain_buffer_builder.py
--rw-r--r--   0 simply     (502) staff       (20)     3197 2024-02-27 07:52:14.000000 tablestore-5.4.3/tablestore/plainbuffer/plain_buffer_crc8.py
--rw-r--r--   0 simply     (502) staff       (20)     1186 2024-02-27 07:52:14.000000 tablestore-5.4.3/tablestore/plainbuffer/plain_buffer_consts.py
--rw-r--r--   0 simply     (502) staff       (20)     3416 2024-02-27 07:52:14.000000 tablestore-5.4.3/tablestore/plainbuffer/plain_buffer_stream.py
--rw-r--r--   0 simply     (502) staff       (20)     6828 2024-02-27 08:55:01.000000 tablestore-5.4.3/tablestore.egg-info/PKG-INFO
--rw-r--r--   0 simply     (502) staff       (20)     4977 2024-02-27 08:55:01.000000 tablestore-5.4.3/tablestore.egg-info/._SOURCES.txt
--rw-r--r--   0 simply     (502) staff       (20)     1353 2024-02-27 08:55:01.000000 tablestore-5.4.3/tablestore.egg-info/SOURCES.txt
--rw-r--r--   0 simply     (502) staff       (20)     4523 2024-02-27 08:55:01.000000 tablestore-5.4.3/tablestore.egg-info/._requires.txt
--rw-r--r--   0 simply     (502) staff       (20)      126 2024-02-27 08:55:01.000000 tablestore-5.4.3/tablestore.egg-info/requires.txt
--rw-r--r--   0 simply     (502) staff       (20)     4603 2024-02-27 08:55:01.000000 tablestore-5.4.3/tablestore.egg-info/._top_level.txt
--rw-r--r--   0 simply     (502) staff       (20)       24 2024-02-27 08:55:01.000000 tablestore-5.4.3/tablestore.egg-info/top_level.txt
--rw-r--r--   0 simply     (502) staff       (20)     4559 2024-02-27 08:55:01.000000 tablestore-5.4.3/tablestore.egg-info/._dependency_links.txt
--rw-r--r--   0 simply     (502) staff       (20)        1 2024-02-27 08:55:01.000000 tablestore-5.4.3/tablestore.egg-info/dependency_links.txt
+drwxr-xr-x   0 jeffcheung   (502) staff       (20)        0 2024-04-02 07:56:55.000000 tablestore-5.4.4/
+-rw-r--r--   0 jeffcheung   (502) staff       (20)     6828 2024-04-02 07:56:55.000000 tablestore-5.4.4/PKG-INFO
+drwxr-xr-x   0 jeffcheung   (502) staff       (20)        0 2024-04-02 07:56:55.000000 tablestore-5.4.4/tablestore.egg-info/
+-rwxr-xr-x   0 jeffcheung   (502) staff       (20)     1949 2024-04-02 07:21:42.000000 tablestore-5.4.4/setup.py
+drwxr-xr-x   0 jeffcheung   (502) staff       (20)        0 2024-04-02 07:56:55.000000 tablestore-5.4.4/tablestore/
+-rw-r--r--   0 jeffcheung   (502) staff       (20)       38 2024-04-02 07:56:55.000000 tablestore-5.4.4/setup.cfg
+-rw-r--r--   0 jeffcheung   (502) staff       (20)     4939 2024-04-02 07:21:42.000000 tablestore-5.4.4/README.rst
+-rw-r--r--   0 jeffcheung   (502) staff       (20)    36560 2024-04-02 07:21:42.000000 tablestore-5.4.4/tablestore/decoder.py
+drwxr-xr-x   0 jeffcheung   (502) staff       (20)        0 2024-04-02 07:56:55.000000 tablestore-5.4.4/tablestore/plainbuffer/
+-rw-r--r--   0 jeffcheung   (502) staff       (20)     3820 2024-04-02 07:21:42.000000 tablestore-5.4.4/tablestore/aggregation.py
+-rw-r--r--   0 jeffcheung   (502) staff       (20)    30536 2024-04-02 07:21:42.000000 tablestore-5.4.4/tablestore/metadata.py
+-rw-r--r--   0 jeffcheung   (502) staff       (20)     1056 2024-04-02 07:21:42.000000 tablestore-5.4.4/tablestore/error.py
+-rw-r--r--   0 jeffcheung   (502) staff       (20)    11380 2024-04-02 07:21:42.000000 tablestore-5.4.4/tablestore/protocol.py
+-rw-r--r--   0 jeffcheung   (502) staff       (20)    37215 2024-04-02 07:21:42.000000 tablestore-5.4.4/tablestore/client.py
+-rw-r--r--   0 jeffcheung   (502) staff       (20)    11575 2024-04-02 07:21:42.000000 tablestore-5.4.4/tablestore/group_by.py
+-rw-r--r--   0 jeffcheung   (502) staff       (20)     2865 2024-04-02 07:40:11.000000 tablestore-5.4.4/tablestore/__init__.py
+-rw-r--r--   0 jeffcheung   (502) staff       (20)      903 2024-04-02 07:21:42.000000 tablestore-5.4.4/tablestore/types.py
+-rw-r--r--   0 jeffcheung   (502) staff       (20)    56359 2024-04-02 07:21:42.000000 tablestore-5.4.4/tablestore/encoder.py
+-rw-r--r--   0 jeffcheung   (502) staff       (20)     5072 2024-04-02 07:21:42.000000 tablestore-5.4.4/tablestore/retry.py
+-rw-r--r--   0 jeffcheung   (502) staff       (20)     1836 2024-04-02 07:21:42.000000 tablestore-5.4.4/tablestore/connection.py
+-rw-r--r--   0 jeffcheung   (502) staff       (20)      627 2024-04-02 07:21:42.000000 tablestore-5.4.4/tablestore/utils.py
+drwxr-xr-x   0 jeffcheung   (502) staff       (20)        0 2024-04-02 07:56:55.000000 tablestore-5.4.4/tablestore/flatbuffer/
+drwxr-xr-x   0 jeffcheung   (502) staff       (20)        0 2024-04-02 07:57:55.000000 tablestore-5.4.4/tablestore/protobuf/
+-rw-r--r--   0 jeffcheung   (502) staff       (20)      372 2024-04-02 07:21:42.000000 tablestore-5.4.4/tablestore/const.py
+drwxr-xr-x   0 jeffcheung   (502) staff       (20)        0 2024-04-02 07:57:55.000000 tablestore-5.4.4/tablestore/protobuf/py3/
+drwxr-xr-x   0 jeffcheung   (502) staff       (20)        0 2024-04-02 07:56:55.000000 tablestore-5.4.4/tablestore/protobuf/py2/
+-rw-r--r--   0 jeffcheung   (502) staff       (20)    11503 2024-04-02 07:21:42.000000 tablestore-5.4.4/tablestore/protobuf/py2/table_store_filter_pb2.py
+-rw-r--r--   0 jeffcheung   (502) staff       (20)        0 2024-04-02 07:21:42.000000 tablestore-5.4.4/tablestore/protobuf/py2/__init__.py
+-rw-r--r--   0 jeffcheung   (502) staff       (20)   164399 2024-04-02 07:21:42.000000 tablestore-5.4.4/tablestore/protobuf/py2/table_store_pb2.py
+-rw-r--r--   0 jeffcheung   (502) staff       (20)   209501 2024-04-02 07:21:42.000000 tablestore-5.4.4/tablestore/protobuf/py2/search_pb2.py
+-rw-r--r--   0 jeffcheung   (502) staff       (20)    13500 2024-04-02 07:57:55.000000 tablestore-5.4.4/tablestore/protobuf/py3/table_store_filter_pb2.py
+-rw-r--r--   0 jeffcheung   (502) staff       (20)        0 2024-04-02 07:57:55.000000 tablestore-5.4.4/tablestore/protobuf/py3/__init__.py
+-rw-r--r--   0 jeffcheung   (502) staff       (20)   184768 2024-04-02 07:57:55.000000 tablestore-5.4.4/tablestore/protobuf/py3/table_store_pb2.py
+-rw-r--r--   0 jeffcheung   (502) staff       (20)   234437 2024-04-02 07:57:55.000000 tablestore-5.4.4/tablestore/protobuf/py3/search_pb2.py
+-rw-r--r--   0 jeffcheung   (502) staff       (20)     2951 2024-04-02 07:21:42.000000 tablestore-5.4.4/tablestore/flatbuffer/flat_buffer_decoder.py
+-rw-r--r--   0 jeffcheung   (502) staff       (20)        0 2024-04-02 07:21:42.000000 tablestore-5.4.4/tablestore/flatbuffer/__init__.py
+drwxr-xr-x   0 jeffcheung   (502) staff       (20)        0 2024-04-02 07:56:55.000000 tablestore-5.4.4/tablestore/flatbuffer/dataprotocol/
+-rw-r--r--   0 jeffcheung   (502) staff       (20)        0 2024-04-02 07:21:42.000000 tablestore-5.4.4/tablestore/flatbuffer/dataprotocol/__init__.py
+-rw-r--r--   0 jeffcheung   (502) staff       (20)     5013 2024-04-02 07:21:42.000000 tablestore-5.4.4/tablestore/flatbuffer/dataprotocol/SQLResponseColumns.py
+-rw-r--r--   0 jeffcheung   (502) staff       (20)     3932 2024-04-02 07:21:42.000000 tablestore-5.4.4/tablestore/flatbuffer/dataprotocol/BytesValue.py
+-rw-r--r--   0 jeffcheung   (502) staff       (20)     4532 2024-04-02 07:21:42.000000 tablestore-5.4.4/tablestore/flatbuffer/dataprotocol/SQLResponseColumn.py
+-rw-r--r--   0 jeffcheung   (502) staff       (20)      227 2024-04-02 07:21:42.000000 tablestore-5.4.4/tablestore/flatbuffer/dataprotocol/DataType.py
+-rw-r--r--   0 jeffcheung   (502) staff       (20)    17063 2024-04-02 07:21:42.000000 tablestore-5.4.4/tablestore/flatbuffer/dataprotocol/ColumnValues.py
+-rw-r--r--   0 jeffcheung   (502) staff       (20)     6177 2024-04-02 07:21:42.000000 tablestore-5.4.4/tablestore/flatbuffer/dataprotocol/RLEStringValues.py
+-rw-r--r--   0 jeffcheung   (502) staff       (20)    24014 2024-04-02 07:21:42.000000 tablestore-5.4.4/tablestore/plainbuffer/plain_buffer_coded_stream.py
+-rw-r--r--   0 jeffcheung   (502) staff       (20)        0 2024-04-02 07:21:42.000000 tablestore-5.4.4/tablestore/plainbuffer/__init__.py
+-rw-r--r--   0 jeffcheung   (502) staff       (20)     9774 2024-04-02 07:21:42.000000 tablestore-5.4.4/tablestore/plainbuffer/plain_buffer_builder.py
+-rw-r--r--   0 jeffcheung   (502) staff       (20)     3197 2024-04-02 07:21:42.000000 tablestore-5.4.4/tablestore/plainbuffer/plain_buffer_crc8.py
+-rw-r--r--   0 jeffcheung   (502) staff       (20)     1186 2024-04-02 07:21:42.000000 tablestore-5.4.4/tablestore/plainbuffer/plain_buffer_consts.py
+-rw-r--r--   0 jeffcheung   (502) staff       (20)     3416 2024-04-02 07:21:42.000000 tablestore-5.4.4/tablestore/plainbuffer/plain_buffer_stream.py
+-rw-r--r--   0 jeffcheung   (502) staff       (20)     6828 2024-04-02 07:56:55.000000 tablestore-5.4.4/tablestore.egg-info/PKG-INFO
+-rw-r--r--   0 jeffcheung   (502) staff       (20)     4991 2024-04-02 07:56:55.000000 tablestore-5.4.4/tablestore.egg-info/._SOURCES.txt
+-rw-r--r--   0 jeffcheung   (502) staff       (20)     1373 2024-04-02 07:56:55.000000 tablestore-5.4.4/tablestore.egg-info/SOURCES.txt
+-rw-r--r--   0 jeffcheung   (502) staff       (20)     4539 2024-04-02 07:56:55.000000 tablestore-5.4.4/tablestore.egg-info/._requires.txt
+-rw-r--r--   0 jeffcheung   (502) staff       (20)      126 2024-04-02 07:56:55.000000 tablestore-5.4.4/tablestore.egg-info/requires.txt
+-rw-r--r--   0 jeffcheung   (502) staff       (20)     4605 2024-04-02 07:56:55.000000 tablestore-5.4.4/tablestore.egg-info/._top_level.txt
+-rw-r--r--   0 jeffcheung   (502) staff       (20)       24 2024-04-02 07:56:55.000000 tablestore-5.4.4/tablestore.egg-info/top_level.txt
+-rw-r--r--   0 jeffcheung   (502) staff       (20)     4545 2024-04-02 07:56:55.000000 tablestore-5.4.4/tablestore.egg-info/._dependency_links.txt
+-rw-r--r--   0 jeffcheung   (502) staff       (20)        1 2024-04-02 07:56:55.000000 tablestore-5.4.4/tablestore.egg-info/dependency_links.txt
```

### Comparing `tablestore-5.4.3/PKG-INFO` & `tablestore-5.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tablestore
-Version: 5.4.3
+Version: 5.4.4
 Summary: Aliyun TableStore(OTS) SDK
 Home-page: https://cn.aliyun.com/product/ots
 Author: UNKNOWN
 Author-email: UNKNOWN
 License: UNKNOWN
 Description: Aliyun Tablestore SDK for Python
         ==================================
```

### Comparing `tablestore-5.4.3/setup.py` & `tablestore-5.4.4/setup.py`

 * *Files identical despite different names*

### Comparing `tablestore-5.4.3/README.rst` & `tablestore-5.4.4/README.rst`

 * *Files identical despite different names*

### Comparing `tablestore-5.4.3/tablestore/decoder.py` & `tablestore-5.4.4/tablestore/decoder.py`

 * *Files identical despite different names*

### Comparing `tablestore-5.4.3/tablestore/aggregation.py` & `tablestore-5.4.4/tablestore/aggregation.py`

 * *Files identical despite different names*

### Comparing `tablestore-5.4.3/tablestore/metadata.py` & `tablestore-5.4.4/tablestore/metadata.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 # -*- coding: utf8 -*-
 
 import six
-from tablestore.error import *
 from enum import Enum
-import tablestore.protobuf.search_pb2 as search_pb2
+from tablestore.error import *
+from tablestore.utils import DefaultJsonObject
+from tablestore.protobuf import search_pb2
 
-class TableMeta(object):
+class TableMeta(DefaultJsonObject):
 
     def __init__(self, table_name, schema_of_primary_key, defined_columns=[]):
         # schema_of_primary_key: [('PK0', 'STRING'), ('PK1', 'INTEGER'), ...]
         self.table_name = table_name
         self.schema_of_primary_key = schema_of_primary_key
         self.defined_columns = defined_columns
 
-class TableOptions(object):
-    def __init__(self, time_to_live = -1, max_version = 1, max_time_deviation = 86400, allow_update = None):
+class TableOptions(DefaultJsonObject):
+    def __init__(self, time_to_live=-1, max_version=1, max_time_deviation=86400, allow_update=None):
         self.time_to_live = time_to_live
         self.max_version = max_version
         self.max_time_deviation = max_time_deviation
         self.allow_update = allow_update
 
-class CapacityUnit(object):
+class CapacityUnit(DefaultJsonObject):
 
     def __init__(self, read=0, write=0):
         self.read = read
         self.write = write
 
 
-class ReservedThroughput(object):
+class ReservedThroughput(DefaultJsonObject):
 
     def __init__(self, capacity_unit):
         self.capacity_unit = capacity_unit
 
 
-class ReservedThroughputDetails(object):
+class ReservedThroughputDetails(DefaultJsonObject):
 
     def __init__(self, capacity_unit, last_increase_time, last_decrease_time):
         self.capacity_unit = capacity_unit
         self.last_increase_time = last_increase_time
         self.last_decrease_time = last_decrease_time
 
 
@@ -55,25 +56,25 @@
 class AnalyzerType(object):
     SINGLEWORD = "single_word"
     MAXWORD = "max_word"
     MINWORD = "min_word"
     FUZZY = "fuzzy"
     SPLIT = "split"
 
-class SingleWordAnalyzerParameter(object):
-    def __init__(self, case_sensitive = False, delimit_word = False):
+class SingleWordAnalyzerParameter(DefaultJsonObject):
+    def __init__(self, case_sensitive=False, delimit_word=False):
         self.case_sensitive = case_sensitive
         self.delimit_word = delimit_word
 
-class SplitAnalyzerParameter(object):
-    def __init__(self, delimiter = ' '):
+class SplitAnalyzerParameter(DefaultJsonObject):
+    def __init__(self, delimiter=' '):
         self.delimiter = delimiter
 
-class FuzzyAnalyzerParameter(object):
-    def __init__(self, min_chars = 1, max_chars = 7):
+class FuzzyAnalyzerParameter(DefaultJsonObject):
+    def __init__(self, min_chars=1, max_chars=7):
         self.min_chars = min_chars
         self.max_chars = max_chars
 
 class ScoreMode(Enum):
     NONE = search_pb2.SCORE_MODE_NONE
     AVG = search_pb2.SCORE_MODE_AVG
     MAX = search_pb2.SCORE_MODE_MAX
@@ -89,15 +90,15 @@
     ASC = search_pb2.SORT_ORDER_ASC
     DESC = search_pb2.SORT_ORDER_DESC
 
 class GeoDistanceType(Enum):
     ARC = search_pb2.GEO_DISTANCE_ARC
     PLANE = search_pb2.GEO_DISTANCE_PLANE
 
-class Sorter(object):
+class Sorter(DefaultJsonObject):
     def __init__(self):
         pass
 
 class FieldSort(Sorter):
 
     def __init__(self, field_name, sort_order=None, sort_mode=None, nested_filter=None):
         self.field_name = field_name
@@ -121,20 +122,20 @@
         self.sort_order = sort_order
 
 class PrimaryKeySort(Sorter):
 
     def __init__(self, sort_order=SortOrder.ASC):
         self.sort_order = sort_order
 
-class Sort(object):
+class Sort(DefaultJsonObject):
 
     def __init__(self, sorters):
         self.sorters = sorters
 
-class IndexSetting(object):
+class IndexSetting(DefaultJsonObject):
 
     def __init__(self, routing_fields=[]):
         self.routing_fields = routing_fields
 
 
 class VectorDataType(Enum):
     VD_FLOAT_32 = search_pb2.VD_FLOAT_32
@@ -142,23 +143,23 @@
 
 class VectorMetricType(Enum):
     VM_EUCLIDEAN = search_pb2.VM_EUCLIDEAN
     VM_COSINE = search_pb2.VM_COSINE
     VM_DOT_PRODUCT = search_pb2.VM_DOT_PRODUCT
 
 
-class VectorOptions(object):
+class VectorOptions(DefaultJsonObject):
 
     def __init__(self, data_type, metric_type, dimension):
         self.data_type = data_type
         self.metric_type = metric_type
         self.dimension = dimension
 
 
-class FieldSchema(object):
+class FieldSchema(DefaultJsonObject):
 
     def __init__(self, field_name, field_type, index=None,
                  store=None, is_array=None, enable_sort_and_agg=None,
                  analyzer=None, sub_field_schemas=[], analyzer_parameter=None,
                  date_formats=[], is_virtual_field=False, source_fields=[], vector_options=None):
 
         self.field_name = field_name
@@ -176,39 +177,39 @@
         self.vector_options = vector_options
 
 
 class SyncPhase(Enum):
     FULL = 0
     INCR = 1
 
-class SyncStat(object):
+class SyncStat(DefaultJsonObject):
 
     def __init__(self, sync_phase, current_sync_timestamp):
         self.sync_phase = sync_phase
         self.current_sync_timestamp = current_sync_timestamp
 
-class SearchIndexMeta(object):
+class SearchIndexMeta(DefaultJsonObject):
 
     def __init__(self, fields, index_setting=None, index_sort=None, time_to_live=-1):
         self.fields = fields
         self.index_setting = index_setting
         self.index_sort = index_sort
         self.time_to_live = time_to_live
 
-class DefinedColumnSchema(object):
+class DefinedColumnSchema(DefaultJsonObject):
 
     def __init__(self, name, column_type):
         self.name = name
         self.column_type = column_type
 
 class SecondaryIndexType(Enum):
     GLOBAL_INDEX = 0
     LOCAL_INDEX = 1
 
-class SecondaryIndexMeta(object):
+class SecondaryIndexMeta(DefaultJsonObject):
 
     def __init__(self, index_name, primary_key_names, defined_column_names, index_type=SecondaryIndexType.GLOBAL_INDEX):
         self.index_name = index_name
         self.primary_key_names = primary_key_names
         self.defined_column_names = defined_column_names
         self.index_type = index_type
 
@@ -221,15 +222,15 @@
     INF_MIN = "INF_MIN"
     INF_MAX = "INF_MAX"
 
 class ReturnType(object):
     RT_NONE = "RT_NONE"
     RT_PK = "RT_PK"
 
-class Column(object):
+class Column(DefaultJsonObject):
     def __init__(self, name, value = None, timestamp = None):
         self.name = name
         self.value = value
         self.timestamp = timestamp
 
     def set_timestamp(self, timestamp):
         self.timestamp = timestamp
@@ -249,15 +250,15 @@
 
 class UpdateType(object):
     PUT = "PUT"
     DELETE = "DELETE"
     DELETE_ALL = "DELETE_ALL"
     INCREMENT = "INCREMENT"
 
-class CommonResponse(object):
+class CommonResponse(DefaultJsonObject):
     def __init__(self):
         self.request_id = ''
 
     def set_request_id(self, request_id):
         self.request_id = request_id
 
 class UpdateTableResponse(CommonResponse):
@@ -272,15 +273,15 @@
     def __init__(self, table_meta, table_options, reserved_throughput_details, secondary_indexes=[]):
         self.table_meta = table_meta
         self.table_options = table_options
         self.reserved_throughput_details = reserved_throughput_details
         self.secondary_indexes = secondary_indexes
 
 
-class RowDataItem(object):
+class RowDataItem(DefaultJsonObject):
 
     def __init__(self, is_ok, error_code, error_message, table_name, consumed, primary_key_columns, attribute_columns):
         # is_ok can be True or False
         # when is_ok is False,
         #     error_code & error_message are available
         # when is_ok is True,
         #     consumed & primary_key_columns & attribute_columns are available
@@ -337,33 +338,30 @@
     ]
 
 
 class ColumnConditionType(object):
     COMPOSITE_COLUMN_CONDITION = 0
     SINGLE_COLUMN_CONDITION = 1
 
-class ColumnCondition(object):
+class ColumnCondition(DefaultJsonObject):
     pass
 
 class CompositeColumnCondition(ColumnCondition):
 
     def __init__(self, combinator):
         self.sub_conditions = []
-        self.set_combinator(combinator)
-
-    def get_type(self):
-        return ColumnConditionType.COMPOSITE_COLUMN_CONDITION
-
-    def set_combinator(self, combinator):
         if combinator not in LogicalOperator.__values__:
             raise OTSClientError(
-                "Expect input combinator should be one of %s, but '%s'"%(str(LogicalOperator.__members__), combinator)
+                "Expect input combinator should be one of %s, but '%s'" % (str(LogicalOperator.__members__), combinator)
             )
         self.combinator = combinator
 
+    def get_type(self):
+        return ColumnConditionType.COMPOSITE_COLUMN_CONDITION
+
     def get_combinator(self):
         return self.combinator
 
     def add_sub_condition(self, condition):
         if not isinstance(condition, ColumnCondition):
             raise OTSClientError(
                 "The input condition should be an instance of ColumnCondition, not %s"%
@@ -469,15 +467,15 @@
 
     __members__ = [
         "RowExistenceExpectation.IGNORE",
         "RowExistenceExpectation.EXPECT_EXIST",
         "RowExistenceExpectation.EXPECT_NOT_EXIST",
     ]
 
-class Condition(object):
+class Condition(DefaultJsonObject):
 
     def __init__(self, row_existence_expectation, column_condition = None):
         self.row_existence_expectation = None
         self.column_condition = None
 
         self.set_row_existence_expectation(row_existence_expectation)
         if column_condition != None:
@@ -501,20 +499,20 @@
                 column_condition.__class__.__name__
             )
         self.column_condition = column_condition
 
     def get_column_condition(self):
         self.column_condition
 
-class Row(object):
+class Row(DefaultJsonObject):
     def __init__(self, primary_key, attribute_columns = None):
         self.primary_key = primary_key
         self.attribute_columns = attribute_columns
 
-class RowItem(object):
+class RowItem(DefaultJsonObject):
 
     def __init__(self, row_type, row, condition, return_type = None):
         self.type = row_type
         self.condition = condition
         self.row = row
         self.return_type = return_type
 
@@ -530,15 +528,15 @@
 
 class DeleteRowItem(RowItem):
 
     def __init__(self, row, condition, return_type = None):
         super(DeleteRowItem, self).__init__(BatchWriteRowType.DELETE, row, condition, return_type)
 
 
-class TableInBatchGetRowItem(object):
+class TableInBatchGetRowItem(DefaultJsonObject):
 
     def __init__(self, table_name, primary_keys, columns_to_get=None,
                  column_filter=None, max_version=None, time_range=None,
                  start_column=None, end_column=None, token=None):
         self.table_name = table_name
         self.primary_keys = primary_keys
         self.columns_to_get = columns_to_get
@@ -546,15 +544,15 @@
         self.max_version = max_version
         self.time_range = time_range
         self.start_column = start_column
         self.end_column = end_column
         self.token = token
 
 
-class BatchGetRowRequest(object):
+class BatchGetRowRequest(DefaultJsonObject):
 
     def __init__(self):
         self.items = {}
 
     def add(self, table_item):
         """
         说明：添加tablestore.metadata.TableInBatchGetRowItem对象
@@ -565,15 +563,15 @@
             raise OTSClientError(
                 "The input table_item should be an instance of TableInBatchGetRowItem, not %s"%
                 table_item.__class__.__name__
             )
 
         self.items[table_item.table_name] = table_item
 
-class BatchGetRowResponse(object):
+class BatchGetRowResponse(DefaultJsonObject):
 
     def __init__(self, table_rows):
         self.items = table_rows
 
     def get_failed_rows(self):
         return [row for rows in self.items.values() for row in rows if not row.is_ok]
 
@@ -594,22 +592,22 @@
 
 class BatchWriteRowType(object):
     PUT = "put"
     UPDATE = "update"
     DELETE = "delete"
 
 
-class TableInBatchWriteRowItem(object):
+class TableInBatchWriteRowItem(DefaultJsonObject):
 
     def __init__(self, table_name, row_items):
         self.table_name = table_name
         self.row_items = row_items
 
 
-class BatchWriteRowRequest(object):
+class BatchWriteRowRequest(DefaultJsonObject):
 
     def __init__(self):
         self.items = {}
         self.transaction_id = None
 
     def add(self, table_item):
         """
@@ -625,15 +623,15 @@
 
         self.items[table_item.table_name] = table_item
 
     def set_transaction_id(self, transcation_id):
         self.transaction_id = transcation_id
 
 
-class BatchWriteRowResponse(object):
+class BatchWriteRowResponse(DefaultJsonObject):
 
     def __init__(self, request, response):
         self.table_of_put = {}
         self.table_of_update = {}
         self.table_of_delete = {}
 
         for table_name in list(response.keys()):
@@ -731,15 +729,15 @@
         succ, fail = self.get_delete()
         fail = None
         return succ
 
     def is_all_succeed(self):
         return self.get_failed_of_put() == [] and self.get_failed_of_update() == [] and self.get_failed_of_delete() == []
 
-class BatchWriteRowResponseItem(object):
+class BatchWriteRowResponseItem(DefaultJsonObject):
 
     def __init__(self, is_ok, error_code, error_message, consumed, primary_key):
         self.is_ok = is_ok
         self.error_code = error_code
         self.error_message = error_message
         self.consumed = consumed
         self.row = Row(primary_key)
@@ -777,15 +775,15 @@
     TERMS_QUERY = search_pb2.TERMS_QUERY
     KNN_VECTOR_QUERY = search_pb2.KNN_VECTOR_QUERY
 
 class QueryOperator(Enum):
     OR = search_pb2.OR
     AND = search_pb2.AND
 
-class Query(object):
+class Query(DefaultJsonObject):
 
     def __init__(self):
         pass
 
 class MatchQuery(Query):
 
     def __init__(self, field_name, text, minimum_should_match=None, operator=None):
@@ -871,26 +869,26 @@
 
 class GeoPolygonQuery(Query):
 
     def __init__(self, field_name, points):
         self.field_name = field_name
         self.points = points
 
-class Collapse(object):
+class Collapse(DefaultJsonObject):
 
     def __init__(self, field_name):
         self.field_name = field_name
 
-class NestedFilter(object):
+class NestedFilter(DefaultJsonObject):
 
     def __init__(self, path, query_filter):
         self.path = path
         self.query_filter = query_filter
 
-class FieldValueFactor(object):
+class FieldValueFactor(DefaultJsonObject):
 
     def __init__(self, field_name):
         self.field_name = field_name
 
 class FunctionScoreQuery(Query):
 
     def __init__(self, query, field_value_factor):
@@ -906,15 +904,15 @@
 
     def __init__(self, field_name, top_k=None, float32_query_vector=None, filter=None):
         self.field_name = field_name
         self.top_k = top_k
         self.float32_query_vector = float32_query_vector
         self.filter = filter
 
-class SearchQuery(object):
+class SearchQuery(DefaultJsonObject):
 
     def __init__(self, query, sort=None, get_total_count=False,
                  next_token=None, offset=None, limit=None,
                  aggs = None, group_bys = None, collapse_field = None):
 
         self.query = query
         self.sort = sort
@@ -922,15 +920,15 @@
         self.next_token = next_token
         self.offset = offset
         self.limit = limit
         self.aggs = aggs
         self.group_bys = group_bys
         self.collapse = collapse_field
 
-class ScanQuery(object):
+class ScanQuery(DefaultJsonObject):
 
     def __init__(self, query, limit, next_token, current_parallel_id, max_parallel, alive_time = 60):
         self.query = query
         self.limit = limit
         self.next_token = next_token
         self.current_parallel_id = current_parallel_id
         self.max_parallel = max_parallel
@@ -939,15 +937,15 @@
 class ColumnReturnType(Enum):
 
     ALL = search_pb2.RETURN_ALL
     SPECIFIED = search_pb2.RETURN_SPECIFIED
     NONE = search_pb2.RETURN_NONE
     ALL_FROM_INDEX = search_pb2.RETURN_ALL_FROM_INDEX
 
-class ColumnsToGet(object):
+class ColumnsToGet(DefaultJsonObject):
 
     def __init__(self, column_names=[], return_type=ColumnReturnType.NONE):
         self.column_names = column_names
         self.return_type = return_type
 
 class IterableResponse(CommonResponse):
     def __init__(self):
```

### Comparing `tablestore-5.4.3/tablestore/error.py` & `tablestore-5.4.4/tablestore/error.py`

 * *Files identical despite different names*

### Comparing `tablestore-5.4.3/tablestore/protocol.py` & `tablestore-5.4.4/tablestore/protocol.py`

 * *Files identical despite different names*

### Comparing `tablestore-5.4.3/tablestore/client.py` & `tablestore-5.4.4/tablestore/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 import sys
 import six
 import time
 import _strptime
 
 import logging
+
 try:  # Python 2.7+
     from logging import NullHandler
 except ImportError:
     class NullHandler(logging.Handler):
         def emit(self, record):
             pass
 
@@ -33,15 +34,14 @@
     ``OTSClient``实现了OTS服务的所有接口。用户可以通过创建``OTSClient``的实例，并调用它的
     方法来访问OTS服务的所有功能。用户可以在初始化方法``__init__()``中设置各种权限、连接等参数。
 
     除非另外说明，``OTSClient``的所有接口都以抛异常的方式处理错误(请参考模块``tablestore.error``
     )，即如果某个函数有返回值，则会在描述中说明；否则返回None。
     """
 
-
     DEFAULT_ENCODING = 'utf8'
     DEFAULT_SOCKET_TIMEOUT = 50
     DEFAULT_MAX_CONNECTION = 50
     DEFAULT_LOGGER_NAME = 'tablestore-client'
 
     protocol_class = OTSProtocol
     connection_pool_class = ConnectionPool
@@ -219,15 +219,15 @@
         示例：
 
             table_list = client.list_table()
         """
 
         return self._request_helper('ListTable')
 
-    def update_table(self, table_name, table_options = None, reserved_throughput = None):
+    def update_table(self, table_name, table_options=None, reserved_throughput=None):
         """
         说明：更新表属性，目前只支持修改预留读写吞吐量。
 
         ``table_name``是对应的表名。
         ``table_options``是``tablestore.metadata.TableOptions``类的示例，它包含time_to_live，max_version和max_time_deviation三个参数。
         ``reserved_throughput``是``tablestore.metadata.ReservedThroughput``类的实例，表示预留读写吞吐量。
 
@@ -239,15 +239,15 @@
 
             reserved_throughput = ReservedThroughput(CapacityUnit(0, 0))
             table_options = TableOptions();
             update_response = client.update_table('myTable', table_options, reserved_throughput)
         """
 
         return self._request_helper(
-                    'UpdateTable', table_name, table_options, reserved_throughput
+            'UpdateTable', table_name, table_options, reserved_throughput
         )
 
     def describe_table(self, table_name):
         """
         说明：获取表的描述信息。
 
         ``table_name``是对应的表名。
@@ -287,20 +287,20 @@
 
             primary_key = [('gid',1), ('uid',101)]
             columns_to_get = ['name', 'address', 'age']
             consumed, return_row, next_token = client.get_row('myTable', primary_key, columns_to_get)
         """
 
         return self._request_helper(
-                    'GetRow', table_name, primary_key, columns_to_get,
-                    column_filter, max_version, time_range,
-                    start_column, end_column, token, transaction_id
+            'GetRow', table_name, primary_key, columns_to_get,
+            column_filter, max_version, time_range,
+            start_column, end_column, token, transaction_id
         )
 
-    def put_row(self, table_name, row, condition = None, return_type = None, transaction_id = None):
+    def put_row(self, table_name, row, condition=None, return_type=None, transaction_id=None):
         """
         说明：写入一行数据。返回本次操作消耗的CapacityUnit。
 
         ``table_name``是对应的表名。
         ``row``是行数据，包括主键和属性列。
         ``condition``表示执行操作前做条件检查，满足条件才执行，是tablestore.metadata.Condition类的实例。
         目前支持两种条件检测，一是对行的存在性进行检查，检查条件包括：'IGNORE'，'EXPECT_EXIST'和'EXPECT_NOT_EXIST';二是对属性列值的条件检测。
@@ -317,18 +317,18 @@
             attribute_columns = [('name','张三'), ('mobile',111111111), ('address','中国A地'), ('age',20)]
             row = Row(primary_key, attribute_columns)
             condition = Condition('EXPECT_NOT_EXIST')
             consumed, return_row = client.put_row('myTable', row, condition)
         """
 
         return self._request_helper(
-                    'PutRow', table_name, row, condition, return_type, transaction_id
+            'PutRow', table_name, row, condition, return_type, transaction_id
         )
 
-    def update_row(self, table_name, row, condition, return_type = None, transaction_id = None):
+    def update_row(self, table_name, row, condition, return_type=None, transaction_id=None):
         """
         说明：更新一行数据。
 
         ``table_name``是对应的表名。
         ``row``表示更新的行数据，包括主键列和属性列，主键列是list；属性列是dict。
         ``condition``表示执行操作前做条件检查，满足条件才执行，是tablestore.metadata.Condition类的实例。
         目前支持两种条件检测，一是对行的存在性进行检查，检查条件包括：'IGNORE'，'EXPECT_EXIST'和'EXPECT_NOT_EXIST';二是对属性列值的条件检测。
@@ -350,18 +350,18 @@
             }
             row = Row(primary_key, update_of_attribute_columns)
             condition = Condition('EXPECT_EXIST')
             consumed = client.update_row('myTable', row, condition)
         """
 
         return self._request_helper(
-                    'UpdateRow', table_name, row, condition, return_type, transaction_id
+            'UpdateRow', table_name, row, condition, return_type, transaction_id
         )
 
-    def delete_row(self, table_name, row, condition, return_type = None, transaction_id = None):
+    def delete_row(self, table_name, row, condition, return_type=None, transaction_id=None):
         """
         说明：删除一行数据。
 
         ``table_name``是对应的表名。
         ``row``表示行数据，在delete_row仅包含主键。
         ``condition``表示执行操作前做条件检查，满足条件才执行，是tablestore.metadata.Condition类的实例。
         目前支持两种条件检测，一是对行的存在性进行检查，检查条件包括：'IGNORE'，'EXPECT_EXIST'和'EXPECT_NOT_EXIST';二是对属性列值的条件检测。
@@ -376,35 +376,35 @@
             primary_key = [('gid',1), ('uid',101)]
             row = Row(primary_key)
             condition = Condition('IGNORE')
             consumed, return_row = client.delete_row('myTable', row, condition)
         """
 
         return self._request_helper(
-                    'DeleteRow', table_name, row, condition, return_type, transaction_id
+            'DeleteRow', table_name, row, condition, return_type, transaction_id
         )
-    
-    def exe_sql_query(self,query):
+
+    def exe_sql_query(self, query):
         """
         说明：执行sql query
 
         ``query``query是需要执行的query。
-        
+
         (rows,table_capacity_units,search_capacity_units)
 
         返回：
         ``table_capacity_units``  本次操作消耗的每张table对应的CapacityUnit
         ``search_capacity_units`` 本次操作消耗的每个search的CapacityUnit
         ``rows``                  返回的数据
-        
+
         示例：
         row_list,table_comsume_list,search_comsume_list = client.exe_sql_query(query)
         """
         return self._request_helper(
-                    'SQLQuery', query
+            'SQLQuery', query
         )
 
     def batch_get_row(self, request):
         """
         说明：批量获取多行数据。
         request = BatchGetRowRequest()
 
@@ -485,26 +485,25 @@
 
         """
 
         response = self._request_helper('BatchWriteRow', request)
 
         return BatchWriteRowResponse(request, response)
 
-
     def get_range(self, table_name, direction,
                   inclusive_start_primary_key,
                   exclusive_end_primary_key,
                   columns_to_get=None,
                   limit=None,
                   column_filter=None,
                   max_version=1,
                   time_range=None,
                   start_column=None,
                   end_column=None,
-                  token = None,
+                  token=None,
                   transaction_id=None):
         """
         说明：根据范围条件获取多行数据。
 
         ``table_name``是对应的表名。
         ``direction``表示范围的方向，字符串格式，取值包括'FORWARD'和'BACKWARD'。
         ``inclusive_start_primary_key``表示范围的起始主键（在范围内）。
@@ -534,35 +533,35 @@
                         'myTable', 'FORWARD',
                         inclusive_start_primary_key, exclusive_end_primary_key,
                         columns_to_get, 100
             )
         """
 
         return self._request_helper(
-                    'GetRange', table_name, direction,
-                    inclusive_start_primary_key, exclusive_end_primary_key,
-                    columns_to_get, limit,
-                    column_filter, max_version,
-                    time_range, start_column,
-                    end_column, token,
-                    transaction_id
+            'GetRange', table_name, direction,
+            inclusive_start_primary_key, exclusive_end_primary_key,
+            columns_to_get, limit,
+            column_filter, max_version,
+            time_range, start_column,
+            end_column, token,
+            transaction_id
         )
 
     def xget_range(self, table_name, direction,
                    inclusive_start_primary_key,
                    exclusive_end_primary_key,
                    consumed_counter,
                    columns_to_get=None,
                    count=None,
                    column_filter=None,
                    max_version=1,
                    time_range=None,
                    start_column=None,
                    end_column=None,
-                   token = None):
+                   token=None):
         """
         说明：根据范围条件获取多行数据，iterator版本。
 
         ``table_name``是对应的表名。
         ``direction``表示范围的方向，取值为Direction的FORWARD和BACKWARD。
         ``inclusive_start_primary_key``表示范围的起始主键（在范围内）。
         ``exclusive_end_primary_key``表示范围的结束主键（不在范围内）。
@@ -623,15 +622,14 @@
             for row in row_list:
                 yield row
                 if left_count is not None:
                     left_count -= 1
                     if left_count <= 0:
                         return
 
-
     def _validate_parameter(self, endpoint, access_key_id, access_key_secret, instance_name):
         if endpoint is None or endpoint == '':
             raise OTSClientError('endpoint is None or empty.')
 
         if access_key_id is None or access_key_id == '':
             raise OTSClientError('access_key_id is None or empty.')
 
@@ -711,15 +709,14 @@
         Example usage:
            index_meta = SearchIndexMeta(fields=None, index_setting=None, index_sort=None, time_to_live = 94608000)
            client.update_search_index('table_1', 'index_1', index_meta)
         """
 
         self._request_helper('UpdateSearchIndex', table_name, index_name, index_meta)
 
-
     def describe_search_index(self, table_name, index_name):
         """
         Describe search index.
 
         :type table_name: str
         :param table_name: The name of table.
 
@@ -780,15 +777,15 @@
 
         ``compute_splits_response``表示并发度计算的结果，是 tablestore.metadata.ComputeSplitsResponse 类的实例。
 
         Example usage:
             compute_splits_response = client.compute_splits(table_name, index_name)
             )
         """
-        
+
         return self._request_helper('ComputeSplits', table_name, index_name)
 
     def parallel_scan(self, table_name, index_name, scan_query, session_id, columns_to_get=None):
         """
         Perform parallel scan on search index.
 
         :type table_name: str
@@ -816,33 +813,36 @@
             parallel_scan_response = client.parallel_scan(
                 table_name, index_name,
                 ScanQuery(query, token = token_str, current_parallel_id = 0, max_parallel = 3, limit=100),
                 ColumnsToGet(return_type=ColumnReturnType.RETURN_ALL_FROM_INDEX)
             )
         """
 
-        return self._request_helper('ParallelScan', table_name, index_name, scan_query, 
+        return self._request_helper('ParallelScan', table_name, index_name, scan_query,
                                     session_id, columns_to_get)
 
-    def create_secondary_index(self, table_name, index_meta):
+    def create_secondary_index(self, table_name, index_meta, include_base_data):
         """
         Create a new secondary index.
 
         :type table_name: str
         :param table_name: The name of table.
 
         :type index_meta: tablestore.metadata.SecondaryIndexMeta
         :param index_meta: The definition of index.
 
+        :type include_base_data: bool
+        :param include_base_data: Whether to include the data in the main table or not.
+
         Example usage:
             index_meta = SecondaryIndexMeta('index1', ['i', 's'], ['gid', 'uid', 'bool', 'b', 'd'])
             client.create_secondary_index(table_name, index_meta)
         """
 
-        return self._request_helper('CreateIndex', table_name, index_meta)
+        return self._request_helper('CreateIndex', table_name, index_meta, include_base_data)
 
     def delete_secondary_index(self, table_name, index_name):
         """
         Delete the secondary index.
 
         :type table_name: str
         :param table_name: The name of table.
```

### Comparing `tablestore-5.4.3/tablestore/group_by.py` & `tablestore-5.4.4/tablestore/group_by.py`

 * *Files identical despite different names*

### Comparing `tablestore-5.4.3/tablestore/__init__.py` & `tablestore-5.4.4/tablestore/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf8 -*-
 
-__version__ = '5.4.3'
+__version__ = '5.4.4'
 __all__ = [
     'OTSClient',
 
     # Data Types
     'INF_MIN',
     'INF_MAX',
     'PK_AUTO_INCR',
```

### Comparing `tablestore-5.4.3/tablestore/encoder.py` & `tablestore-5.4.4/tablestore/encoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1313,18 +1313,19 @@
             proto.max_parallel = max_parallel
         else:
             raise OTSClientError('max_parallel must be integer')
 
         return proto.SerializeToString()
 
 
-    def _encode_create_index(self, table_name, index_meta):
+    def _encode_create_index(self, table_name, index_meta, include_base_data):
         proto = pb2.CreateIndexRequest()
 
         proto.main_table_name = table_name
+        proto.include_base_data = include_base_data
         self._make_secondary_index(proto.index_meta, index_meta)
 
         return proto
 
     def _encode_delete_index(self, table_name, index_name):
         proto = pb2.DropIndexRequest()
         proto.main_table_name = table_name
```

### Comparing `tablestore-5.4.3/tablestore/retry.py` & `tablestore-5.4.4/tablestore/retry.py`

 * *Files identical despite different names*

### Comparing `tablestore-5.4.3/tablestore/connection.py` & `tablestore-5.4.4/tablestore/connection.py`

 * *Files identical despite different names*

### Comparing `tablestore-5.4.3/tablestore/protobuf/py2/table_store_filter_pb2.py` & `tablestore-5.4.4/tablestore/protobuf/py2/table_store_filter_pb2.py`

 * *Files identical despite different names*

### Comparing `tablestore-5.4.3/tablestore/protobuf/py2/table_store_pb2.py` & `tablestore-5.4.4/tablestore/protobuf/py2/table_store_pb2.py`

 * *Files identical despite different names*

### Comparing `tablestore-5.4.3/tablestore/protobuf/py2/search_pb2.py` & `tablestore-5.4.4/tablestore/protobuf/py2/search_pb2.py`

 * *Files identical despite different names*

### Comparing `tablestore-5.4.3/tablestore/protobuf/py3/table_store_filter_pb2.py` & `tablestore-5.4.4/tablestore/protobuf/py3/table_store_filter_pb2.py`

 * *Files identical despite different names*

### Comparing `tablestore-5.4.3/tablestore/protobuf/py3/table_store_pb2.py` & `tablestore-5.4.4/tablestore/protobuf/py3/table_store_pb2.py`

 * *Files identical despite different names*

### Comparing `tablestore-5.4.3/tablestore/protobuf/py3/search_pb2.py` & `tablestore-5.4.4/tablestore/protobuf/py3/search_pb2.py`

 * *Files identical despite different names*

### Comparing `tablestore-5.4.3/tablestore/flatbuffer/flat_buffer_decoder.py` & `tablestore-5.4.4/tablestore/flatbuffer/flat_buffer_decoder.py`

 * *Files identical despite different names*

### Comparing `tablestore-5.4.3/tablestore/flatbuffer/dataprotocol/SQLResponseColumns.py` & `tablestore-5.4.4/tablestore/flatbuffer/dataprotocol/SQLResponseColumns.py`

 * *Files identical despite different names*

### Comparing `tablestore-5.4.3/tablestore/flatbuffer/dataprotocol/BytesValue.py` & `tablestore-5.4.4/tablestore/flatbuffer/dataprotocol/BytesValue.py`

 * *Files identical despite different names*

### Comparing `tablestore-5.4.3/tablestore/flatbuffer/dataprotocol/SQLResponseColumn.py` & `tablestore-5.4.4/tablestore/flatbuffer/dataprotocol/SQLResponseColumn.py`

 * *Files identical despite different names*

### Comparing `tablestore-5.4.3/tablestore/flatbuffer/dataprotocol/ColumnValues.py` & `tablestore-5.4.4/tablestore/flatbuffer/dataprotocol/ColumnValues.py`

 * *Files identical despite different names*

### Comparing `tablestore-5.4.3/tablestore/flatbuffer/dataprotocol/RLEStringValues.py` & `tablestore-5.4.4/tablestore/flatbuffer/dataprotocol/RLEStringValues.py`

 * *Files identical despite different names*

### Comparing `tablestore-5.4.3/tablestore/plainbuffer/plain_buffer_coded_stream.py` & `tablestore-5.4.4/tablestore/plainbuffer/plain_buffer_coded_stream.py`

 * *Files identical despite different names*

### Comparing `tablestore-5.4.3/tablestore/plainbuffer/plain_buffer_builder.py` & `tablestore-5.4.4/tablestore/plainbuffer/plain_buffer_builder.py`

 * *Files identical despite different names*

### Comparing `tablestore-5.4.3/tablestore/plainbuffer/plain_buffer_crc8.py` & `tablestore-5.4.4/tablestore/plainbuffer/plain_buffer_crc8.py`

 * *Files identical despite different names*

### Comparing `tablestore-5.4.3/tablestore/plainbuffer/plain_buffer_consts.py` & `tablestore-5.4.4/tablestore/plainbuffer/plain_buffer_consts.py`

 * *Files identical despite different names*

### Comparing `tablestore-5.4.3/tablestore/plainbuffer/plain_buffer_stream.py` & `tablestore-5.4.4/tablestore/plainbuffer/plain_buffer_stream.py`

 * *Files identical despite different names*

### Comparing `tablestore-5.4.3/tablestore.egg-info/PKG-INFO` & `tablestore-5.4.4/tablestore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tablestore
-Version: 5.4.3
+Version: 5.4.4
 Summary: Aliyun TableStore(OTS) SDK
 Home-page: https://cn.aliyun.com/product/ots
 Author: UNKNOWN
 Author-email: UNKNOWN
 License: UNKNOWN
 Description: Aliyun Tablestore SDK for Python
         ==================================
```

### Comparing `tablestore-5.4.3/tablestore.egg-info/SOURCES.txt` & `tablestore-5.4.4/tablestore.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 tablestore/encoder.py
 tablestore/error.py
 tablestore/group_by.py
 tablestore/metadata.py
 tablestore/protocol.py
 tablestore/retry.py
 tablestore/types.py
+tablestore/utils.py
 tablestore.egg-info/PKG-INFO
 tablestore.egg-info/SOURCES.txt
 tablestore.egg-info/dependency_links.txt
 tablestore.egg-info/requires.txt
 tablestore.egg-info/top_level.txt
 tablestore/flatbuffer/__init__.py
 tablestore/flatbuffer/flat_buffer_decoder.py
```

