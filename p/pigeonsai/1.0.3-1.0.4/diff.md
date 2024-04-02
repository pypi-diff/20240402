# Comparing `tmp/pigeonsai-1.0.3.tar.gz` & `tmp/pigeonsai-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pigeonsai-1.0.3.tar", last modified: Wed Mar 27 17:04:39 2024, max compression
+gzip compressed data, was "pigeonsai-1.0.4.tar", last modified: Tue Apr  2 15:06:50 2024, max compression
```

## Comparing `pigeonsai-1.0.3.tar` & `pigeonsai-1.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 bs        (1000) bs        (1000)        0 2024-03-27 17:04:39.928776 pigeonsai-1.0.3/
--rw-r--r--   0 bs        (1000) bs        (1000)     2046 2024-03-27 17:04:39.928776 pigeonsai-1.0.3/PKG-INFO
--rw-r--r--   0 bs        (1000) bs        (1000)      560 2024-03-25 05:17:42.000000 pigeonsai-1.0.3/README.md
--rw-r--r--   0 bs        (1000) bs        (1000)       38 2024-03-27 17:04:39.928776 pigeonsai-1.0.3/setup.cfg
--rw-r--r--   0 bs        (1000) bs        (1000)     2075 2024-03-27 17:04:03.000000 pigeonsai-1.0.3/setup.py
-drwxr-xr-x   0 bs        (1000) bs        (1000)        0 2024-03-27 17:04:39.918776 pigeonsai-1.0.3/src/
-drwxr-xr-x   0 bs        (1000) bs        (1000)        0 2024-03-27 17:04:39.918776 pigeonsai-1.0.3/src/pigeonsai/
--rw-r--r--   0 bs        (1000) bs        (1000)      479 2024-03-15 16:34:17.000000 pigeonsai-1.0.3/src/pigeonsai/__init__.py
--rw-r--r--   0 bs        (1000) bs        (1000)     3913 2024-03-22 23:15:49.000000 pigeonsai-1.0.3/src/pigeonsai/_client.py
--rw-r--r--   0 bs        (1000) bs        (1000)       49 2024-03-26 06:03:43.000000 pigeonsai-1.0.3/src/pigeonsai/_constants.py
--rw-r--r--   0 bs        (1000) bs        (1000)     3288 2024-03-16 02:35:35.000000 pigeonsai-1.0.3/src/pigeonsai/_exceptions.py
-drwxr-xr-x   0 bs        (1000) bs        (1000)        0 2024-03-27 17:04:39.918776 pigeonsai-1.0.3/src/pigeonsai/_utils/
--rw-r--r--   0 bs        (1000) bs        (1000)       39 2024-03-15 17:28:27.000000 pigeonsai-1.0.3/src/pigeonsai/_utils/__init__.py
--rw-r--r--   0 bs        (1000) bs        (1000)      136 2024-03-15 16:23:51.000000 pigeonsai-1.0.3/src/pigeonsai/_utils/_utils.py
-drwxr-xr-x   0 bs        (1000) bs        (1000)        0 2024-03-27 17:04:39.918776 pigeonsai-1.0.3/src/pigeonsai/resources/
--rw-r--r--   0 bs        (1000) bs        (1000)      148 2024-03-19 16:08:19.000000 pigeonsai-1.0.3/src/pigeonsai/resources/__init__.py
--rw-r--r--   0 bs        (1000) bs        (1000)      181 2024-03-19 16:42:03.000000 pigeonsai-1.0.3/src/pigeonsai/resources/anomaly_detector.py
--rw-r--r--   0 bs        (1000) bs        (1000)     9322 2024-03-26 03:32:55.000000 pigeonsai-1.0.3/src/pigeonsai/resources/data_connector.py
--rw-r--r--   0 bs        (1000) bs        (1000)     8058 2024-03-27 01:36:15.000000 pigeonsai-1.0.3/src/pigeonsai/resources/recommender.py
-drwxr-xr-x   0 bs        (1000) bs        (1000)        0 2024-03-27 17:04:39.928776 pigeonsai-1.0.3/src/pigeonsai.egg-info/
--rw-r--r--   0 bs        (1000) bs        (1000)     2046 2024-03-27 17:04:39.000000 pigeonsai-1.0.3/src/pigeonsai.egg-info/PKG-INFO
--rw-r--r--   0 bs        (1000) bs        (1000)      535 2024-03-27 17:04:39.000000 pigeonsai-1.0.3/src/pigeonsai.egg-info/SOURCES.txt
--rw-r--r--   0 bs        (1000) bs        (1000)        1 2024-03-27 17:04:39.000000 pigeonsai-1.0.3/src/pigeonsai.egg-info/dependency_links.txt
--rw-r--r--   0 bs        (1000) bs        (1000)       31 2024-03-27 17:04:39.000000 pigeonsai-1.0.3/src/pigeonsai.egg-info/requires.txt
--rw-r--r--   0 bs        (1000) bs        (1000)       10 2024-03-27 17:04:39.000000 pigeonsai-1.0.3/src/pigeonsai.egg-info/top_level.txt
+drwxr-xr-x   0 bs        (1000) bs        (1000)        0 2024-04-02 15:06:50.148120 pigeonsai-1.0.4/
+-rw-r--r--   0 bs        (1000) bs        (1000)     2046 2024-04-02 15:06:50.148120 pigeonsai-1.0.4/PKG-INFO
+-rw-r--r--   0 bs        (1000) bs        (1000)      560 2024-03-25 05:17:42.000000 pigeonsai-1.0.4/README.md
+-rw-r--r--   0 bs        (1000) bs        (1000)       38 2024-04-02 15:06:50.148120 pigeonsai-1.0.4/setup.cfg
+-rw-r--r--   0 bs        (1000) bs        (1000)     2075 2024-03-28 04:38:26.000000 pigeonsai-1.0.4/setup.py
+drwxr-xr-x   0 bs        (1000) bs        (1000)        0 2024-04-02 15:06:50.138120 pigeonsai-1.0.4/src/
+drwxr-xr-x   0 bs        (1000) bs        (1000)        0 2024-04-02 15:06:50.138120 pigeonsai-1.0.4/src/pigeonsai/
+-rw-r--r--   0 bs        (1000) bs        (1000)      479 2024-03-15 16:34:17.000000 pigeonsai-1.0.4/src/pigeonsai/__init__.py
+-rw-r--r--   0 bs        (1000) bs        (1000)     3913 2024-03-22 23:15:49.000000 pigeonsai-1.0.4/src/pigeonsai/_client.py
+-rw-r--r--   0 bs        (1000) bs        (1000)       48 2024-04-02 15:06:23.000000 pigeonsai-1.0.4/src/pigeonsai/_constants.py
+-rw-r--r--   0 bs        (1000) bs        (1000)     3288 2024-03-16 02:35:35.000000 pigeonsai-1.0.4/src/pigeonsai/_exceptions.py
+drwxr-xr-x   0 bs        (1000) bs        (1000)        0 2024-04-02 15:06:50.138120 pigeonsai-1.0.4/src/pigeonsai/_utils/
+-rw-r--r--   0 bs        (1000) bs        (1000)       39 2024-03-15 17:28:27.000000 pigeonsai-1.0.4/src/pigeonsai/_utils/__init__.py
+-rw-r--r--   0 bs        (1000) bs        (1000)      136 2024-03-15 16:23:51.000000 pigeonsai-1.0.4/src/pigeonsai/_utils/_utils.py
+drwxr-xr-x   0 bs        (1000) bs        (1000)        0 2024-04-02 15:06:50.148120 pigeonsai-1.0.4/src/pigeonsai/resources/
+-rw-r--r--   0 bs        (1000) bs        (1000)      148 2024-03-19 16:08:19.000000 pigeonsai-1.0.4/src/pigeonsai/resources/__init__.py
+-rw-r--r--   0 bs        (1000) bs        (1000)      181 2024-03-19 16:42:03.000000 pigeonsai-1.0.4/src/pigeonsai/resources/anomaly_detector.py
+-rw-r--r--   0 bs        (1000) bs        (1000)     9645 2024-03-28 04:03:04.000000 pigeonsai-1.0.4/src/pigeonsai/resources/data_connector.py
+-rw-r--r--   0 bs        (1000) bs        (1000)     8314 2024-03-30 06:05:17.000000 pigeonsai-1.0.4/src/pigeonsai/resources/recommender.py
+drwxr-xr-x   0 bs        (1000) bs        (1000)        0 2024-04-02 15:06:50.148120 pigeonsai-1.0.4/src/pigeonsai.egg-info/
+-rw-r--r--   0 bs        (1000) bs        (1000)     2046 2024-04-02 15:06:50.000000 pigeonsai-1.0.4/src/pigeonsai.egg-info/PKG-INFO
+-rw-r--r--   0 bs        (1000) bs        (1000)      535 2024-04-02 15:06:50.000000 pigeonsai-1.0.4/src/pigeonsai.egg-info/SOURCES.txt
+-rw-r--r--   0 bs        (1000) bs        (1000)        1 2024-04-02 15:06:50.000000 pigeonsai-1.0.4/src/pigeonsai.egg-info/dependency_links.txt
+-rw-r--r--   0 bs        (1000) bs        (1000)       31 2024-04-02 15:06:50.000000 pigeonsai-1.0.4/src/pigeonsai.egg-info/requires.txt
+-rw-r--r--   0 bs        (1000) bs        (1000)       10 2024-04-02 15:06:50.000000 pigeonsai-1.0.4/src/pigeonsai.egg-info/top_level.txt
```

### Comparing `pigeonsai-1.0.3/PKG-INFO` & `pigeonsai-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pigeonsai
-Version: 1.0.3
+Version: 1.0.4
 Summary: PigeonAI client and SDK
 Home-page: https://www.pigeonsai.com/
 Author: PigeonsAI Inc.
 Author-email: info@pigeonsai.com
 License: Proprietary License
 Project-URL: Homepage, https://www.pigeonsai.com
 Project-URL: Documentation, https://docs.pigeonsai.com/
```

### Comparing `pigeonsai-1.0.3/README.md` & `pigeonsai-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pigeonsai-1.0.3/setup.py` & `pigeonsai-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 long_desc = """
 PigeonsAI is an ecosystem to build production ready machine learning applications.
 """
 
 setup(
     name="pigeonsai",
-    version="1.0.3",
+    version="1.0.4",
     description="PigeonAI client and SDK",
     license="Proprietary License",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     url="https://www.pigeonsai.com/",
     project_urls={
         "Homepage": "https://www.pigeonsai.com",
```

### Comparing `pigeonsai-1.0.3/src/pigeonsai/_client.py` & `pigeonsai-1.0.4/src/pigeonsai/_client.py`

 * *Files identical despite different names*

### Comparing `pigeonsai-1.0.3/src/pigeonsai/_exceptions.py` & `pigeonsai-1.0.4/src/pigeonsai/_exceptions.py`

 * *Files identical despite different names*

### Comparing `pigeonsai-1.0.3/src/pigeonsai/resources/data_connector.py` & `pigeonsai-1.0.4/src/pigeonsai/resources/data_connector.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # resources/data_connector.py
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
+from typing import Literal
 from .._constants import (BASE_URL_V2)
 
 import httpx
 import os
 import json
 
 if TYPE_CHECKING:
@@ -18,31 +19,34 @@
 
     def __init__(self, client: PigeonsAI):
         self.client = client
 
     def create_connector(
         self,
         connection_name: str,
-        connection_type: str,
+        connection_type: Literal['postgres', 'mysql'],
         db_host: str,
         db_name: str,
         db_username: str,
         db_password: str,
         db_port: int
     ):
+        if connection_type not in ['postgres', 'mysql']:
+            raise ValueError("Invalid connection type. Please choose 'postgres' or 'mysql'.")
+    
         url = f"{BASE_URL_V2}/create-data-connector"
         headers = self.client.auth_headers
         data = {
-            "conn_id": connection_name,
-            "conn_type": connection_type,
-            "host": db_host,
-            "login": db_username,
-            "password": db_password,
-            "port": db_port,
-            "schema_param": db_name
+            "data_connection_custom_name": connection_name,
+            "data_connection_type": connection_type,
+            "data_connection_host": db_host,
+            "data_connection_port": db_port,
+            "data_connection_database_name": db_name,
+            "data_connection_username": db_username,
+            "data_connection_password": db_password
         }
 
         response = self.client._request("POST", url, headers=headers, data=data)
         response_json = response.json()
 
         _data = response_json['data']
```

### Comparing `pigeonsai-1.0.3/src/pigeonsai/resources/recommender.py` & `pigeonsai-1.0.4/src/pigeonsai/resources/recommender.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,35 +63,37 @@
 
         return response
 
     def _inference(
         self,
         user_history_ids: Optional[str] = None,
         user_id: Optional[int] = None,
+        exclude_seen: Optional[bool] = None,
         k: int = 10,
-        model_uri: str = None,
+        model_endpoint: str = None,
         model_name: str = None
     ):
         if user_history_ids is None and user_id is None:
             raise ValueError("Either user_id or user_history_ids must be provided.")
 
-        if model_name and model_uri:
-            raise ValueError("Both model_name and model_uri are provided. Either one of them will be used.")
+        if model_name and model_endpoint:
+            raise ValueError("Both model_name and model_endpoint are provided. Either one of them will be used.")
 
-        model_uri = _construct_model_url(model_uri=model_uri, model_name=model_name)
+        model_endpoint = _construct_model_url(model_endpoint=model_endpoint, model_name=model_name)
 
         headers = self.client.auth_headers
         data = {
             "k": k,
             "user_id": user_id,
+            "exclude_seen": exclude_seen,
             "history_ids": user_history_ids,
         }
 
         try:
-            response = self.client._http_client.post(model_uri, headers=headers, json=data, timeout=300.0)
+            response = self.client._http_client.post(model_endpoint, headers=headers, json=data, timeout=300.0)
             response.raise_for_status()
             return response.json()
         except httpx.HTTPStatusError as e:
             error_message = f"Status code: {e.response.status_code}, Error: {e.response.text}"
             print(error_message)
         except Exception as e:
             raise e
@@ -146,22 +148,22 @@
         return self._train(custom_model_name, train_set_uri, **{k: v for k, v in kwargs.items() if v is not None})
 
     def inference(
         self,
         user_history_ids: Optional[str] = None,
         user_id: Optional[int] = None,
         k: int = 10,
-        model_uri: str = None,
+        model_endpoint: str = None,
         model_name: str = None
     ):
         return self._inference(
             user_history_ids=user_history_ids,
             user_id=user_id,
             k=k,
-            model_uri=model_uri,
+            model_endpoint=model_endpoint,
             model_name=model_name
         )
         
     def retrain(
         self,
         unique_identifier: str,
         pull_latest_data: bool,
@@ -213,37 +215,39 @@
         }
         return self._train(custom_model_name, train_set_uri, **{k: v for k, v in kwargs.items() if v is not None})
         
     def inference(
         self,
         user_history_ids: Optional[str] = None,
         user_id: Optional[int] = None,
+        exclude_seen: Optional[bool] = None,
         k: int = 10,
-        model_uri: str = None,
+        model_endpoint: str = None,
         model_name: str = None
     ):
         return self._inference(
             user_history_ids=user_history_ids,
             user_id=user_id,
+            exclude_seen=exclude_seen,
             k=k,
-            model_uri=model_uri,
+            model_endpoint=model_endpoint,
             model_name=model_name
         )
         
     def retrain(
         self,
         unique_identifier: str,
         pull_latest_data: bool,
     ):
         return self._retrain(
             unique_identifier=unique_identifier,
             pull_latest_data=pull_latest_data,
         )
 
 
-def _construct_model_url(model_name: Optional[str] = None, model_uri: Optional[str] = None) -> str:
+def _construct_model_url(model_name: Optional[str] = None, model_endpoint: Optional[str] = None) -> str:
     if model_name:
         return f"https://{model_name}.apps.api1.pigeonsai.cloud/recommend"
-    elif model_uri:
-        return f"{model_uri.rstrip('/')}/recommend"
+    elif model_endpoint:
+        return f"{model_endpoint.rstrip('/')}/recommend"
     else:
-        raise ValueError("Either model_name or model_uri must be provided")
+        raise ValueError("Either model_name or model_endpoint must be provided")
```

### Comparing `pigeonsai-1.0.3/src/pigeonsai.egg-info/PKG-INFO` & `pigeonsai-1.0.4/src/pigeonsai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pigeonsai
-Version: 1.0.3
+Version: 1.0.4
 Summary: PigeonAI client and SDK
 Home-page: https://www.pigeonsai.com/
 Author: PigeonsAI Inc.
 Author-email: info@pigeonsai.com
 License: Proprietary License
 Project-URL: Homepage, https://www.pigeonsai.com
 Project-URL: Documentation, https://docs.pigeonsai.com/
```

### Comparing `pigeonsai-1.0.3/src/pigeonsai.egg-info/SOURCES.txt` & `pigeonsai-1.0.4/src/pigeonsai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

