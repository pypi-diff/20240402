# Comparing `tmp/keble_db-0.0.8.tar.gz` & `tmp/keble_db-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keble_db-0.0.8.tar", max compression
+gzip compressed data, was "keble_db-0.0.9.tar", max compression
```

## Comparing `keble_db-0.0.8.tar` & `keble_db-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1067 2024-03-06 02:48:07.551279 keble_db-0.0.8/LICENSE
--rw-r--r--   0        0        0        0 2024-03-05 10:59:07.033132 keble_db-0.0.8/README.md
--rw-r--r--   0        0        0      273 2024-03-05 12:18:33.687391 keble_db-0.0.8/keble_db/__init__.py
--rw-r--r--   0        0        0       61 2024-03-05 12:04:13.118041 keble_db-0.0.8/keble_db/crud/__init__.py
--rw-r--r--   0        0        0        0 2024-03-05 11:57:35.638146 keble_db-0.0.8/keble_db/crud/base.py
--rw-r--r--   0        0        0     3666 2024-03-05 12:04:13.112549 keble_db-0.0.8/keble_db/crud/mongo.py
--rw-r--r--   0        0        0     2510 2024-03-05 11:59:16.291357 keble_db-0.0.8/keble_db/crud/mongo_util.py
--rw-r--r--   0        0        0     4475 2024-03-19 03:49:27.459302 keble_db-0.0.8/keble_db/crud/sql.py
--rw-r--r--   0        0        0     1682 2024-03-05 12:02:49.151552 keble_db-0.0.8/keble_db/crud/sql_util.py
--rw-r--r--   0        0        0       26 2024-03-05 12:18:33.696464 keble_db-0.0.8/keble_db/deps/__init__.py
--rw-r--r--   0        0        0      963 2024-03-05 12:18:33.693304 keble_db-0.0.8/keble_db/deps/api.py
--rw-r--r--   0        0        0     2944 2024-03-05 11:00:41.549075 keble_db-0.0.8/keble_db/mongo.py
--rw-r--r--   0        0        0     4599 2024-03-06 06:41:18.476617 keble_db-0.0.8/keble_db/schemas.py
--rw-r--r--   0        0        0     3954 2024-03-06 08:13:23.744108 keble_db-0.0.8/keble_db/session.py
--rw-r--r--   0        0        0      434 2024-03-19 03:49:38.696169 keble_db-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      642 1970-01-01 00:00:00.000000 keble_db-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-03-06 02:48:07.551279 keble_db-0.0.9/LICENSE
+-rw-r--r--   0        0        0        0 2024-03-05 10:59:07.033132 keble_db-0.0.9/README.md
+-rw-r--r--   0        0        0      273 2024-03-05 12:18:33.687391 keble_db-0.0.9/keble_db/__init__.py
+-rw-r--r--   0        0        0       61 2024-03-05 12:04:13.118041 keble_db-0.0.9/keble_db/crud/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-05 11:57:35.638146 keble_db-0.0.9/keble_db/crud/base.py
+-rw-r--r--   0        0        0     3666 2024-03-05 12:04:13.112549 keble_db-0.0.9/keble_db/crud/mongo.py
+-rw-r--r--   0        0        0     2510 2024-03-05 11:59:16.291357 keble_db-0.0.9/keble_db/crud/mongo_util.py
+-rw-r--r--   0        0        0     4475 2024-03-19 03:49:27.459302 keble_db-0.0.9/keble_db/crud/sql.py
+-rw-r--r--   0        0        0     1682 2024-03-05 12:02:49.151552 keble_db-0.0.9/keble_db/crud/sql_util.py
+-rw-r--r--   0        0        0       26 2024-03-05 12:18:33.696464 keble_db-0.0.9/keble_db/deps/__init__.py
+-rw-r--r--   0        0        0      963 2024-03-05 12:18:33.693304 keble_db-0.0.9/keble_db/deps/api.py
+-rw-r--r--   0        0        0     2944 2024-03-05 11:00:41.549075 keble_db-0.0.9/keble_db/mongo.py
+-rw-r--r--   0        0        0     4794 2024-03-20 16:03:31.425677 keble_db-0.0.9/keble_db/schemas.py
+-rw-r--r--   0        0        0     3954 2024-03-06 08:13:23.744108 keble_db-0.0.9/keble_db/session.py
+-rw-r--r--   0        0        0      434 2024-03-20 16:04:32.020634 keble_db-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      642 1970-01-01 00:00:00.000000 keble_db-0.0.9/PKG-INFO
```

### Comparing `keble_db-0.0.8/LICENSE` & `keble_db-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `keble_db-0.0.8/keble_db/crud/mongo.py` & `keble_db-0.0.9/keble_db/crud/mongo.py`

 * *Files identical despite different names*

### Comparing `keble_db-0.0.8/keble_db/crud/mongo_util.py` & `keble_db-0.0.9/keble_db/crud/mongo_util.py`

 * *Files identical despite different names*

### Comparing `keble_db-0.0.8/keble_db/crud/sql.py` & `keble_db-0.0.9/keble_db/crud/sql.py`

 * *Files identical despite different names*

### Comparing `keble_db-0.0.8/keble_db/crud/sql_util.py` & `keble_db-0.0.9/keble_db/crud/sql_util.py`

 * *Files identical despite different names*

### Comparing `keble_db-0.0.8/keble_db/deps/api.py` & `keble_db-0.0.9/keble_db/deps/api.py`

 * *Files identical despite different names*

### Comparing `keble_db-0.0.8/keble_db/mongo.py` & `keble_db-0.0.9/keble_db/mongo.py`

 * *Files identical despite different names*

### Comparing `keble_db-0.0.8/keble_db/schemas.py` & `keble_db-0.0.9/keble_db/schemas.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from uuid import UUID as _UUID
 
 from bson import Binary
 from bson import ObjectId as _ObjectId
 from pydantic import GetCoreSchemaHandler, BaseModel
 from pydantic.json_schema import JsonSchemaValue
 from pydantic_core import core_schema
+from pydantic.functional_serializers import PlainSerializer
 
 
 def is_optional(field):
     return get_origin(field) is Union and \
            type(None) in get_args(field)
 
 
@@ -64,14 +65,18 @@
             cls.validate_uuid,
             core_schema.uuid_schema(),
             serialization=core_schema.plain_serializer_function_ser_schema(
                 function=cls.from_uuid
             ),
         )
 
+# add json plain serializer to Uuid
+Uuid = Annotated[
+    Uuid, PlainSerializer(lambda x: str(x), return_type=str, when_used='json')
+]
 
 MaybeUuid = Union[Uuid, _UUID, Binary]
 
 
 def to_binary_uuid(uuid_: Union[MaybeUuid, List[MaybeUuid]]):
     if isinstance(uuid_, list): return [to_binary_uuid(u) for u in uuid_]
     if isinstance(uuid_, Binary): return uuid_
```

### Comparing `keble_db-0.0.8/keble_db/session.py` & `keble_db-0.0.9/keble_db/session.py`

 * *Files identical despite different names*

### Comparing `keble_db-0.0.8/PKG-INFO` & `keble_db-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keble-db
-Version: 0.0.8
+Version: 0.0.9
 Summary: Keble db
 Author: zhenhao-ma
 Author-email: bob0103779@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

