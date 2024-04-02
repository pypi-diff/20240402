# Comparing `tmp/feliz_db-0.0.4.tar.gz` & `tmp/feliz_db-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feliz_db-0.0.4.tar", last modified: Tue Feb 20 08:35:12 2024, max compression
+gzip compressed data, was "feliz_db-0.0.5.tar", last modified: Tue Apr  2 04:05:45 2024, max compression
```

## Comparing `feliz_db-0.0.4.tar` & `feliz_db-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 zenith3092   (501) staff       (20)        0 2024-02-20 08:35:12.283519 feliz_db-0.0.4/
--rw-r--r--   0 zenith3092   (501) staff       (20)     1071 2024-02-20 04:51:52.000000 feliz_db-0.0.4/LICENSE
--rw-r--r--   0 zenith3092   (501) staff       (20)      607 2024-02-20 08:35:12.283402 feliz_db-0.0.4/PKG-INFO
--rw-r--r--   0 zenith3092   (501) staff       (20)       88 2024-02-20 04:51:52.000000 feliz_db-0.0.4/README.md
-drwxr-xr-x   0 zenith3092   (501) staff       (20)        0 2024-02-20 08:35:12.282269 feliz_db-0.0.4/feliz_db/
--rw-r--r--   0 zenith3092   (501) staff       (20)        0 2024-02-20 04:51:52.000000 feliz_db-0.0.4/feliz_db/__init__.py
--rw-r--r--   0 zenith3092   (501) staff       (20)    26197 2024-02-20 08:34:18.000000 feliz_db-0.0.4/feliz_db/mongo_tools.py
--rw-r--r--   0 zenith3092   (501) staff       (20)    39841 2024-02-20 04:51:52.000000 feliz_db-0.0.4/feliz_db/postgres_tools.py
-drwxr-xr-x   0 zenith3092   (501) staff       (20)        0 2024-02-20 08:35:12.283251 feliz_db-0.0.4/feliz_db.egg-info/
--rw-r--r--   0 zenith3092   (501) staff       (20)      607 2024-02-20 08:35:12.000000 feliz_db-0.0.4/feliz_db.egg-info/PKG-INFO
--rw-r--r--   0 zenith3092   (501) staff       (20)      257 2024-02-20 08:35:12.000000 feliz_db-0.0.4/feliz_db.egg-info/SOURCES.txt
--rw-r--r--   0 zenith3092   (501) staff       (20)        1 2024-02-20 08:35:12.000000 feliz_db-0.0.4/feliz_db.egg-info/dependency_links.txt
--rw-r--r--   0 zenith3092   (501) staff       (20)       36 2024-02-20 08:35:12.000000 feliz_db-0.0.4/feliz_db.egg-info/requires.txt
--rw-r--r--   0 zenith3092   (501) staff       (20)        9 2024-02-20 08:35:12.000000 feliz_db-0.0.4/feliz_db.egg-info/top_level.txt
--rw-r--r--   0 zenith3092   (501) staff       (20)       38 2024-02-20 08:35:12.283557 feliz_db-0.0.4/setup.cfg
--rw-r--r--   0 zenith3092   (501) staff       (20)      908 2024-02-20 08:34:18.000000 feliz_db-0.0.4/setup.py
+drwxr-xr-x   0 zenith3092   (501) staff       (20)        0 2024-04-02 04:05:45.177667 feliz_db-0.0.5/
+-rw-r--r--   0 zenith3092   (501) staff       (20)     1071 2024-02-20 04:51:52.000000 feliz_db-0.0.5/LICENSE
+-rw-r--r--   0 zenith3092   (501) staff       (20)      607 2024-04-02 04:05:45.177419 feliz_db-0.0.5/PKG-INFO
+-rw-r--r--   0 zenith3092   (501) staff       (20)       88 2024-02-20 04:51:52.000000 feliz_db-0.0.5/README.md
+drwxr-xr-x   0 zenith3092   (501) staff       (20)        0 2024-04-02 04:05:45.175955 feliz_db-0.0.5/feliz_db/
+-rw-r--r--   0 zenith3092   (501) staff       (20)        0 2024-02-20 04:51:52.000000 feliz_db-0.0.5/feliz_db/__init__.py
+-rw-r--r--   0 zenith3092   (501) staff       (20)    25339 2024-04-02 04:02:34.000000 feliz_db-0.0.5/feliz_db/mongo_tools.py
+-rw-r--r--   0 zenith3092   (501) staff       (20)    39839 2024-04-02 03:54:05.000000 feliz_db-0.0.5/feliz_db/postgres_tools.py
+drwxr-xr-x   0 zenith3092   (501) staff       (20)        0 2024-04-02 04:05:45.177208 feliz_db-0.0.5/feliz_db.egg-info/
+-rw-r--r--   0 zenith3092   (501) staff       (20)      607 2024-04-02 04:05:45.000000 feliz_db-0.0.5/feliz_db.egg-info/PKG-INFO
+-rw-r--r--   0 zenith3092   (501) staff       (20)      257 2024-04-02 04:05:45.000000 feliz_db-0.0.5/feliz_db.egg-info/SOURCES.txt
+-rw-r--r--   0 zenith3092   (501) staff       (20)        1 2024-04-02 04:05:45.000000 feliz_db-0.0.5/feliz_db.egg-info/dependency_links.txt
+-rw-r--r--   0 zenith3092   (501) staff       (20)       36 2024-04-02 04:05:45.000000 feliz_db-0.0.5/feliz_db.egg-info/requires.txt
+-rw-r--r--   0 zenith3092   (501) staff       (20)        9 2024-04-02 04:05:45.000000 feliz_db-0.0.5/feliz_db.egg-info/top_level.txt
+-rw-r--r--   0 zenith3092   (501) staff       (20)       38 2024-04-02 04:05:45.177745 feliz_db-0.0.5/setup.cfg
+-rw-r--r--   0 zenith3092   (501) staff       (20)      908 2024-04-02 03:57:00.000000 feliz_db-0.0.5/setup.py
```

### Comparing `feliz_db-0.0.4/LICENSE` & `feliz_db-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `feliz_db-0.0.4/PKG-INFO` & `feliz_db-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feliz_db
-Version: 0.0.4
+Version: 0.0.5
 Summary: A framework designed to assist in using databases and compatible with feliz framework
 Home-page: https://github.com/zenith3092/feliz_db
 Author: Vincent Wu, Linga Chen, Brian Yin
 Author-email: zenith3092@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `feliz_db-0.0.4/feliz_db/mongo_tools.py` & `feliz_db-0.0.5/feliz_db/mongo_tools.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,69 +1,150 @@
 import mongoengine as mongo
 from pymongo.errors import ServerSelectionTimeoutError
 from pymongo import MongoClient
 import logging
 import datetime
 from bson import ObjectId
 
+class DocumentHandler(mongo.Document):
+    meta = { "abstract": True}
+
+    @classmethod
+    def format_data(cls, mongo_obj):
+        sub_item = mongo_obj.to_mongo().to_dict()
+        return sub_item
+
+    @classmethod
+    def format_data_list(cls, mongo_obj_list):
+        ret = []
+        for item in mongo_obj_list:
+            sub_item = item.to_mongo().to_dict()
+            ret.append(sub_item)
+        return ret
+    
+    @classmethod
+    def format_and_validate_document(cls, data):
+        ret = []
+        for item in data:
+            add_item = cls(**item)
+            add_item.validate()
+            ret.append(add_item)
+        return ret
+
+    @classmethod
+    def handle_modified_time(cls, data: list) -> list:
+        for item in data:
+            item["modified_time"] = datetime.datetime.now().strftime("%Y%m%d%H%M%S%f")[:-3]
+        return data
+
+    @classmethod
+    def get_headers(cls):
+        return list(cls._fields_ordered)
+
+    @classmethod
+    def add_data(cls, data):
+        add_data = cls.format_and_validate_document(data)
+        ret = cls.objects.insert(add_data)
+        return cls.format_data_list(ret)
+
+    @classmethod
+    def get_data(cls, conditions, order_by_list=[]):
+        if conditions:
+            if "_id" in conditions:
+                conditions["_id"] = ObjectId(conditions["_id"])
+            raw_data = cls.objects(__raw__=conditions)
+        else:
+            raw_data = cls.objects
+        return cls.format_data_list(raw_data.order_by(*order_by_list))
+    
+    @classmethod
+    def update_data(cls, conditions, update_data):
+        if conditions:
+            if "_id" in conditions:
+                conditions["_id"] = ObjectId(conditions["_id"])
+            raw_data = cls.objects(__raw__=conditions)
+        else:
+            raw_data = cls.objects
+        return cls.format_data(raw_data.modify(__raw__={"$set": update_data}, new=True))
+    
+    @classmethod
+    def delete_data(cls, conditions):
+        if conditions:
+            if "_id" in conditions:
+                conditions["_id"] = ObjectId(conditions["_id"])
+            raw_data = cls.objects(__raw__=conditions)
+        else:
+            raw_data = cls.objects
+        
+        return raw_data.delete()
+
 class MongoHandler:
     """
     MongoDB Handler
 
     Args:
         alias (str): alias of MongoDB
         host (str): host of MongoDB
         port (int): port of MongoDB
         database (str): database of MongoDB
         username (str): username of MongoDB
         password (str): password of MongoDB
-        schemas (dict): {
-            "schema_name": schema
+        schemas (dict[str, DocumentHandler]): {
+            schema_name: schema
         }
     """
-    def __init__(self, alias: str, host: str, port: int, database: str, username: str, password: str, schemas: str):
+    def __init__(self, alias: str, host: str, port: int, database: str, username: str, password: str, schemas: dict[str, DocumentHandler], **kwargs):
         self.db_type = "mongo"
         self.alias = alias
         self.host = host
         self.port = port
         self.database = database
         self.username = username
         self.password = password
-        self.timeout = 5000 # ms
+        self.timeout = kwargs.get("timeout") if kwargs.get("timeout") else 5000
 
         if not logging.getLogger().hasHandlers():
             logging.basicConfig(level=logging.INFO)
         
-        self.create_schemas(schemas)
+        self._create_schemas(schemas)
         self.connect(first_time=True)
 
     def connect(self, first_time=False) -> None:
+        """
+        This function is used to connect to MongoDB
+
+        Args:
+            first_time (bool, optional): connect to MongoDB for the first time. Defaults to False.
+        """
         try:
             if first_time:
                 client = MongoClient(host=self.host, port=self.port, username=self.username, password=self.password, serverSelectionTimeoutMS=self.timeout)
                 client.server_info()
                 logging.info(" [MongoHandler] Connect to MongoDB successfully ")
                 client.close()
             else:
                 mongo.connect(alias=self.alias, db=self.database, host=self.host, port=self.port, username=self.username, password=self.password, serverSelectionTimeoutMS=self.timeout)
         except ServerSelectionTimeoutError as e:
             logging.warning(" [MongoHandler] Connect to MongoDB failed: \n{} ".format(e))
         except Exception as e:
             logging.warning(" [MongoHandler] Connect to MongoDB failed: \n{} ".format(e))
 
     def disconnect(self) -> None:
+        """
+        This function is used to disconnect from MongoDB
+        """
         mongo.disconnect(alias=self.alias)
     
-    def create_schemas(self, schemas: dict) -> None:
+    def _create_schemas(self, schemas: dict[str, DocumentHandler]) -> None:
         """
         Create schemas
 
         Args:
             schemas (dict): {
-                "schema_name": schema
+                schema_name: schema
             }
         """
         for schema_name, schema in schemas.items():
             self.__dict__[schema_name] = schema
     
     def get_headers(self, schema_name: str) -> dict:
         """
@@ -72,45 +153,44 @@
         Args:
             schema_name (str): name of schema
         
         Returns:
             dict: {
                 "indicator": bool,
                 "message": str,
-                "data": list
+                "formatted_data": list[dict]
             }
         """
         self.connect()
         try:
             data = self.__dict__[schema_name].get_headers()
             indicator = True
             message = "Get headers from MongoDB successfully"
         except Exception as e:
             data = []
             indicator = False
             message = "[MongoHandler] Get headers from MongoDB failed: \n{}".format(e)
             logging.warning(message)
         self.disconnect()
-        return {"indicator": indicator, "message": message, "data": data}
+        return {"indicator": indicator, "message": message, "formatted_data": data}
 
-    def get_data(self, schema_name: str, conditions={}, order_by_list=[], ret_type="jsonable") -> dict:
+    def get_data(self, schema_name: str, conditions={}, order_by_list=[]) -> dict:
         """
         Get data from MongoDB
         
         Args:
             schema_name (str): name of schema (collection name in MongoDB)
             conditions (dict): conditions of query (follow MongoDB query syntax)
-            order_by (list, optional): order by. + for ascending and - for descending. e.g. ["-modified_time"]. Defaults to [].
-            ret_type (str, optional): return type. Defaults to "jsonable". Should be one of ["jsonable", "original"].
+            order_by_list (list, optional): order by. + for ascending and - for descending. e.g. ["-modified_time"]. Defaults to [].
             
         Returns:
             dict: {
                 "indicator": bool,
                 "message": str,
-                "formatted_data": list
+                "formatted_data": list[dict]
             }
         
         Operators(use "$" to represent the operator in conditions):
             - comparison operators:
                 $eq: match values that are equal to a specified value (e.g. {"name": {"$eq": "John"}})
                 $gt: match values that are greater than a specified value (e.g. {"age": {"$gt": 18}})
                 $gte: match values that are greater than or equal to a specified value (e.g. {"age": {"$gte": 18}})
@@ -145,82 +225,92 @@
         TIPS:
             $or can be replaced by $in, e.g. {"$or": [{"name": "John"}, {"name": "Peter"}]} can be replaced by {"name": {"$in": ["John", "Peter"]}}
             $and can be replaced by $all, e.g. {"$and": [{"name": "John"}, {"age": 18}]} can be replaced by {"$all": [{"name": "John"}, {"age": 18}]}
             $not can be replaced by $ne, e.g. {"name": {"$not": {"$eq": "John"}}} can be replaced by {"name": {"$ne": "John"}}
             $nor can be replaced by $nin, e.g. {"$nor": [{"name": "John"}, {"name": "Peter"}]} can be replaced by {"name": {"$nin": ["John", "Peter"]}}
         """
         self.connect()
+
         try:
+            schema: DocumentHandler = self.__dict__[schema_name]
+
             indicator = True
             message = "Get data from MongoDB successfully"
-            data = self.__dict__[schema_name].get_data(conditions, order_by_list, ret_type)
+            data = schema.get_data(conditions, order_by_list)
         except Exception as e:
             indicator = False
             message = "[MongoHandler] Get data from MongoDB failed: {}".format(e)
             data = []
             logging.warning(message)
+        
         self.disconnect()
         return {"indicator": indicator, "message": message, "formatted_data": data}
     
-    def add_data(self, schema_name: str, input_data: list, ret_type="jsonable") -> dict:
+    def add_data(self, schema_name: str, input_data: list[dict]) -> dict:
         """
         Add data to MongoDB and return the data added
         
         Args:
             schema_name (str): name of schema
-            input_data (list of dict): data to add
-            ret_type (str, optional): return type. Defaults to "jsonable". Should be one of ["jsonable", "original"].
+            input_data (list[dict]): data to add
 
         Returns:
             dict: {
                 "indicator": bool,
                 "message": str,
-                "formatted_data": list
+                "formatted_data": list[dict]
             }
         """
         self.connect()
+
         try:
+            schema: DocumentHandler = self.__dict__[schema_name]
+
             indicator = True
             message = "Add data to MongoDB successfully"
-            data = self.__dict__[schema_name].add_data(input_data, ret_type)
+            data = schema.add_data(input_data)
         except Exception as e:
             indicator = False
             message = "[MongoHandler] Add data to MongoDB failed: {}".format(e)
             data = []
             logging.warning(message)
+        
         self.disconnect()
         return {"indicator": indicator, "message": message, "formatted_data": data}
     
-    def update_data(self, schema_name: str, conditions: dict, update_data: dict, ret_type="jsonable") -> dict:
+    def update_data(self, schema_name: str, conditions: dict, update_data: dict) -> dict:
         """
         Update data in MongoDB and return the data updated
         
         Args:
             schema_name (str): name of schema
             conditions (dict): conditions of query (follow MongoDB query syntax)
             update_data (dict): data to update
-            ret_type (str, optional): return type. Defaults to "jsonable". Should be one of ["jsonable", "original"].
         
         Returns:
             dict: {
                 "indicator": bool,
                 "message": str,
                 "formatted_data": list
             }
         """
         self.connect()
+
         try:
+            schema: DocumentHandler = self.__dict__[schema_name]
+
             indicator = True
             message = "Update data in MongoDB successfully"
-            data = self.__dict__[schema_name].update_data(conditions, update_data, ret_type)
+            data = schema.update_data(conditions, update_data)
         except Exception as e:
             indicator = False
             message = "[MongoHandler] Update data in MongoDB failed: {}".format(e)
             data = []
             logging.warning(message)
+
         self.disconnect()
         return {"indicator": indicator, "message": message, "formatted_data": data}
     
     def delete_data(self, schema_name: str, conditions: dict) -> dict:
         """
         Delete data from MongoDB
         
@@ -232,119 +322,31 @@
             dict: {
                 "indicator": bool,
                 "message": str,
                 "formatted_data": list
             }
         """
         self.connect()
+        
         try:
+            schema: DocumentHandler = self.__dict__[schema_name]
+
             indicator = True
             message = "Delete data from MongoDB successfully"
-            delete_count = self.__dict__[schema_name].delete_data(conditions)
-            if "_id" in conditions:
-                conditions["_id"] = str(conditions["_id"])
+            delete_count = schema.delete_data(conditions)
+
             data = [{"deleted_count": delete_count, "conditions": conditions}]
         except Exception as e:
             indicator = False
             message = "[MongoHandler] Delete data from MongoDB failed: {}".format(e)
             data = []
             logging.warning(message)
+        
         self.disconnect()
         return {"indicator": indicator, "message": message, "formatted_data": data}
-    
-class DocumentHandler(mongo.Document):
-    meta = { "abstract": True}
-    _valid_ret_type_list = ["jsonable", "original"]
-
-    @classmethod
-    def format_data(cls, mongo_obj, ret_type="jsonable"):
-        sub_item = mongo_obj.to_mongo().to_dict()
-        if ret_type not in cls._valid_ret_type_list:
-            raise ValueError("Invalid ret_type: {}".format(ret_type))
-        
-        if ret_type == "jsonable":
-            for key, value in sub_item.items():
-                if isinstance(value, ObjectId):
-                    sub_item[key] = str(value)
-                elif isinstance(value, datetime.datetime):
-                    sub_item[key] = value.timestamp()
-        return sub_item
-
-    @classmethod
-    def format_data_list(cls, mongo_obj_list, ret_type="jsonable"):
-        ret = []
-        if ret_type not in cls._valid_ret_type_list:
-            raise ValueError("Invalid ret_type: {}".format(ret_type))
-        
-        for item in mongo_obj_list:
-            sub_item = item.to_mongo().to_dict()
-            if ret_type == "jsonable":
-                for key, value in sub_item.items():
-                    if isinstance(value, ObjectId):
-                        sub_item[key] = str(value)
-                    elif isinstance(value, datetime.datetime):
-                        sub_item[key] = value.timestamp()
-            ret.append(sub_item)
-        return ret
-    
-    @classmethod
-    def format_and_validate_document(cls, data):
-        ret = []
-        for item in data:
-            add_item = cls(**item)
-            add_item.validate()
-            ret.append(add_item)
-        return ret
-
-    @classmethod
-    def handle_modified_time(cls, data: list) -> list:
-        for item in data:
-            item["modified_time"] = datetime.datetime.now().strftime("%Y%m%d%H%M%S%f")[:-3]
-        return data
-
-    @classmethod
-    def get_headers(cls):
-        return list(cls._fields_ordered)
-
-    @classmethod
-    def add_data(cls, data, ret_type="jsonable"):
-        add_data = cls.format_and_validate_document(data)
-        ret = cls.objects.insert(add_data)
-        return cls.format_data_list(ret, ret_type)
-
-    @classmethod
-    def get_data(cls, conditions, order_by_list=[], ret_type="jsonable"):
-        if conditions:
-            if "_id" in conditions:
-                conditions["_id"] = ObjectId(conditions["_id"])
-            raw_data = cls.objects(__raw__=conditions)
-        else:
-            raw_data = cls.objects
-        return cls.format_data_list(raw_data.order_by(*order_by_list), ret_type)
-    
-    @classmethod
-    def update_data(cls, conditions, update_data, ret_type="jsonable"):
-        if conditions:
-            if "_id" in conditions:
-                conditions["_id"] = ObjectId(conditions["_id"])
-            raw_data = cls.objects(__raw__=conditions)
-        else:
-            raw_data = cls.objects
-        return cls.format_data(raw_data.modify(__raw__={"$set": update_data}, new=True), ret_type)
-    
-    @classmethod
-    def delete_data(cls, conditions):
-        if conditions:
-            if "_id" in conditions:
-                conditions["_id"] = ObjectId(conditions["_id"])
-            raw_data = cls.objects(__raw__=conditions)
-        else:
-            raw_data = cls.objects
-        
-        return raw_data.delete()
 
 class MongoWidget:
     """
     MongoDB Widget, this class is used to connect to MongoDB and get data from MongoDB.
     If you want to add data to MongoDB, please use MongoHandler class for strict data validation.
 
     Args:
@@ -415,15 +417,15 @@
                                            e.g. [("modified_time", -1)]
             ret_type (str, optional): return type. Defaults to "jsonable". Should be one of ["jsonable", "original"].
 
         Returns:
             dict: {
                 "indicator": bool,
                 "message": str,
-                "data": list
+                "data": list[dict]
             }
         """
         self.connect()
         try:
             indicator = True
             message = "Get data from MongoDB successfully"
             if ret_type not in self.__class__._valid_ret_type_list:
@@ -443,30 +445,31 @@
             indicator = False
             message = "[MongoWidget] Get data from MongoDB failed: {}".format(e)
             data = []
             logging.warning(message)
         self.disconnect()
         return {"indicator": indicator, "message": message, "data": data}
     
-    def _add_data(self, collection: str, data: list, ret_type="jsonable") -> dict:
+    def _add_data(self, collection: str, data: list[dict], ret_type="jsonable") -> dict:
         """
         Add data to MongoDB
         
         Args:
             collection (str): name of collection
-            data (list of dict): data to add
+            data (list[dict]): data to add
 
         Returns:
             dict: {
                 "indicator": bool,
                 "message": str,
-                "data": list
+                "data": list[dict]
             }
         """
         self.connect()
+
         try:
             indicator = True
             message = "Add data to MongoDB successfully"
             if ret_type not in self.__class__._valid_ret_type_list:
                 raise ValueError("Invalid ret_type: {}".format(ret_type))
             
             ret = self.client[self.database][collection].insert_many(data)
@@ -480,14 +483,15 @@
                     for item in ret:
                         item = self.form_jsonable_data(item)
         except Exception as e:
             indicator = False
             message = "[MongoWidget] Add data to MongoDB failed: {}".format(e)
             ret = []
             logging.warning(message)
+        
         self.disconnect()
         return {"indicator": indicator, "message": message, "data": ret}
 
     def _update_data(self, collection: str, conditions: dict, update_data: dict, ret_type="jsonable") -> dict:
         """
         Update data in MongoDB
         
@@ -500,14 +504,15 @@
             dict: {
                 "indicator": bool,
                 "message": str,
                 "data": list
             }
         """
         self.connect()
+
         try:
             indicator = True
             message = "Update data in MongoDB successfully"
             if ret_type not in self.__class__._valid_ret_type_list:
                 raise ValueError("Invalid ret_type: {}".format(ret_type))
             
             ret = self.client[self.database][collection].update_many(conditions, {"$set": update_data})
@@ -519,14 +524,15 @@
                     for item in ret:
                         item = self.form_jsonable_data(item)
         except Exception as e:
             indicator = False
             message = "[MongoWidget] Update data in MongoDB failed: {}".format(e)
             ret = []
             logging.warning(message)
+        
         self.disconnect()
         return {"indicator": indicator, "message": message, "data": ret}
 
     def _delete_data(self, collection: str, conditions: dict):
         """
         Delete data from MongoDB
         
@@ -538,23 +544,25 @@
             dict: {
                 "indicator": bool,
                 "message": str,
                 "data": list
             }
         """
         self.connect()
+
         try:
             indicator = True
             message = "Delete data from MongoDB successfully"
             ret = [{"deleted_count": self.client[self.database][collection].delete_many(conditions).deleted_count, "conditions": conditions}]
         except Exception as e:
             indicator = False
             message = "[MongoWidget] Delete data from MongoDB failed: {}".format(e)
             ret = []
             logging.warning(message)
+        
         self.disconnect()
         return {"indicator": indicator, "message": message, "data": ret}
 
 # if __name__ == '__main__':
 #     # ========== MongoWidget Example ==========
 
 #     configs = {
@@ -585,29 +593,29 @@
     #     meta = {"db_alias": "trigger"}
 
     # # Construct MongoHandler:
 
     # configs = {
     #             "alias": "trigger",
     #             "host": "localhost",
-    #             "port": 48763,
+    #             "port": 5445,
     #             "database": "trigger",
     #             "username": "test",
-    #             "password": "mongodb",
+    #             "password": "test",
     #             "schemas": {"user": User}
     #           }
     # mh = MongoHandler(**configs)
 
     # # Get Data
 
     # conditions = {"update_state": False, "favorite": {"$elemMatch": {"title": "react"}}}
-    # order_by_list = [("-modified_time")]
+    # order_by_list = ["-modified_time"]
     # res = mh.get_data("user", conditions, order_by_list)
     # if res["indicator"]:
-    #     print(res["data"])
+    #     print(res["formatted_data"])
     # else:
     #     print(res["message"])
     
 #     # Add Data
 
 #     data = [{
 #             'account_id': 'charlie_sysadmin',
@@ -617,29 +625,29 @@
 #             'permission': 'a',
 #             'favorite': [{'title': 'linux', 'author': 'open_source_guru'}],
 #             "modified_time": datetime.datetime.now().strftime("%Y%m%d%H%M%S%f")[:-3],
 #             'comments': 'System administrator specializing in Linux.'
 #             }]
 #     res = mh.add_data("user", data)
 #     if res["indicator"]:
-#         print(res["data"])
+#         print(res["formatted_data"])
 #     else:
 #         print(res["message"])
     
 #     # Update Data
 
 #     update_query = {"account_id": "charlie_sysadmin"}
 #     update_data =  {"update_state": True}
 #     res = mh.update_data("user", update_query, update_data)
 #     if res["indicator"]:
-#         print(res["data"])
+#         print(res["formatted_data"])
 #     else:
 #         print(res["message"])
     
 #     # Delete Data
 
 #     delete_query = {"account_id": "charlie_sysadmin"}
 #     res = mh.delete_data("user", delete_query)
 #     if res["indicator"]:
-#         print(res["data"])
+#         print(res["formatted_data"])
 #     else:
 #         print(res["message"])
```

### Comparing `feliz_db-0.0.4/feliz_db/postgres_tools.py` & `feliz_db-0.0.5/feliz_db/postgres_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -377,15 +377,15 @@
             del result["data"]
             return result
         except Exception as e:
             msg = "[PostgresHandler] delete_data ERROR: "+str(e)
             logging.error(msg)
             return {"indicator": False, "message":msg}
 
-class PostgresModelHandler():
+class PostgresModelHandler:
     """
     This is the class to define the postgres model.
 
     Required Class Attributes:
         meta (dict): The meta data of this class.
             \- initialize (boolean): If this class will be initialized when server starts.
             \- conditional_init (boolean): If this class will be initialized conditionally.
```

### Comparing `feliz_db-0.0.4/feliz_db.egg-info/PKG-INFO` & `feliz_db-0.0.5/feliz_db.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feliz-db
-Version: 0.0.4
+Version: 0.0.5
 Summary: A framework designed to assist in using databases and compatible with feliz framework
 Home-page: https://github.com/zenith3092/feliz_db
 Author: Vincent Wu, Linga Chen, Brian Yin
 Author-email: zenith3092@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `feliz_db-0.0.4/setup.py` & `feliz_db-0.0.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = fh.read()
 
 with open(os.path.join(os.path.dirname(__file__), "requirements.txt"), "r") as f:
     requirements = f.read().split("\n")
 
 setuptools.setup(
     name="feliz_db",
-    version="0.0.4",
+    version="0.0.5",
     author="Vincent Wu, Linga Chen, Brian Yin",
     author_email="zenith3092@gmail.com",
     description="A framework designed to assist in using databases and compatible with feliz framework",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/zenith3092/feliz_db",
     license="MIT",
```

