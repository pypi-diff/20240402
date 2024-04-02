# Comparing `tmp/codec_sdk-0.2.2.tar.gz` & `tmp/codec_sdk-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codec_sdk-0.2.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "codec_sdk-0.2.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `codec_sdk-0.2.2.tar` & `codec_sdk-0.2.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     2757 2024-03-25 13:32:56.805766 codec_sdk-0.2.2/.gitignore
--rw-r--r--   0        0        0      148 2024-03-27 16:29:36.840236 codec_sdk-0.2.2/.pypirc
--rw-r--r--   0        0        0      376 2024-03-31 16:13:59.307377 codec_sdk-0.2.2/CHANGELOG.md
--rw-r--r--   0        0        0     1072 2024-03-25 11:46:44.142211 codec_sdk-0.2.2/LICENSE
--rw-r--r--   0        0        0      211 2024-03-25 20:13:09.134215 codec_sdk-0.2.2/Pipfile
--rw-r--r--   0        0        0     1405 2024-03-31 16:16:48.725034 codec_sdk-0.2.2/README.md
--rw-r--r--   0        0        0       95 2024-03-31 16:18:17.533206 codec_sdk-0.2.2/codec/__init__.py
--rw-r--r--   0        0        0      389 2024-03-25 15:11:00.385160 codec_sdk-0.2.2/codec/auth.py
--rw-r--r--   0        0        0     1054 2024-03-31 14:50:48.455279 codec_sdk-0.2.2/codec/client.py
--rw-r--r--   0        0        0     1289 2024-03-29 12:39:46.742731 codec_sdk-0.2.2/codec/constants.py
--rw-r--r--   0        0        0     1154 2024-03-28 20:45:03.626126 codec_sdk-0.2.2/codec/exceptions.py
--rw-r--r--   0        0        0      153 2024-03-31 14:51:02.287124 codec_sdk-0.2.2/codec/resources/__init__.py
--rw-r--r--   0        0        0        0 2024-03-31 14:49:40.788907 codec_sdk-0.2.2/codec/resources/collections/__init__.py
--rw-r--r--   0        0        0     1003 2024-03-31 16:15:40.706200 codec_sdk-0.2.2/codec/resources/collections/collections.py
--rw-r--r--   0        0        0      476 2024-03-31 15:55:20.630364 codec_sdk-0.2.2/codec/resources/collections/format.py
--rw-r--r--   0        0        0      246 2024-03-31 16:04:43.219098 codec_sdk-0.2.2/codec/resources/collections/types.py
--rw-r--r--   0        0        0       98 2024-03-26 14:18:08.353442 codec_sdk-0.2.2/codec/resources/logger.py
--rw-r--r--   0        0        0     2819 2024-03-31 14:50:06.360715 codec_sdk-0.2.2/codec/resources/request.py
--rw-r--r--   0        0        0        0 2024-03-31 14:50:01.919681 codec_sdk-0.2.2/codec/resources/search/__init__.py
--rw-r--r--   0        0        0      604 2024-03-31 15:45:58.898697 codec_sdk-0.2.2/codec/resources/search/search.py
--rw-r--r--   0        0        0      273 2024-03-31 14:57:46.178512 codec_sdk-0.2.2/codec/resources/search/types.py
--rw-r--r--   0        0        0       45 2024-03-27 14:23:27.578193 codec_sdk-0.2.2/codec/resources/utils/__init__.py
--rw-r--r--   0        0        0      409 2024-03-31 14:51:05.257604 codec_sdk-0.2.2/codec/resources/utils/utils.py
--rw-r--r--   0        0        0      597 2024-03-27 15:12:10.116736 codec_sdk-0.2.2/codec/resources/utils/webhook.py
--rw-r--r--   0        0        0        0 2024-03-31 14:49:13.206374 codec_sdk-0.2.2/codec/resources/videos/__init__.py
--rw-r--r--   0        0        0      371 2024-03-31 15:54:29.778454 codec_sdk-0.2.2/codec/resources/videos/format.py
--rw-r--r--   0        0        0      486 2024-03-31 16:04:41.602700 codec_sdk-0.2.2/codec/resources/videos/types.py
--rw-r--r--   0        0        0     2770 2024-03-31 16:07:41.627900 codec_sdk-0.2.2/codec/resources/videos/videos.py
--rw-r--r--   0        0        0        0 2024-03-25 20:03:51.340117 codec_sdk-0.2.2/codec/utils/__init__.py
--rw-r--r--   0        0        0      633 2024-03-26 12:38:41.420078 codec_sdk-0.2.2/codec/utils/file_utils.py
--rw-r--r--   0        0        0      114 2024-03-31 15:35:42.827701 codec_sdk-0.2.2/codec/utils/type_utils.py
--rw-r--r--   0        0        0      606 2024-03-31 16:16:51.826816 codec_sdk-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1903 1970-01-01 00:00:00.000000 codec_sdk-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     2757 2024-03-25 13:32:56.805766 codec_sdk-0.2.3/.gitignore
+-rw-r--r--   0        0        0      148 2024-03-27 16:29:36.840236 codec_sdk-0.2.3/.pypirc
+-rw-r--r--   0        0        0      376 2024-04-02 10:46:49.198011 codec_sdk-0.2.3/CHANGELOG.md
+-rw-r--r--   0        0        0     1072 2024-03-25 11:46:44.142211 codec_sdk-0.2.3/LICENSE
+-rw-r--r--   0        0        0      211 2024-03-25 20:13:09.134215 codec_sdk-0.2.3/Pipfile
+-rw-r--r--   0        0        0     1405 2024-03-31 16:16:48.725034 codec_sdk-0.2.3/README.md
+-rw-r--r--   0        0        0       95 2024-04-02 10:47:00.564022 codec_sdk-0.2.3/codec/__init__.py
+-rw-r--r--   0        0        0      389 2024-03-25 15:11:00.385160 codec_sdk-0.2.3/codec/auth.py
+-rw-r--r--   0        0        0     1054 2024-03-31 16:40:58.242942 codec_sdk-0.2.3/codec/client.py
+-rw-r--r--   0        0        0     1318 2024-04-02 10:46:02.079632 codec_sdk-0.2.3/codec/constants.py
+-rw-r--r--   0        0        0     1154 2024-03-31 16:38:04.420397 codec_sdk-0.2.3/codec/exceptions.py
+-rw-r--r--   0        0        0      153 2024-03-31 14:51:02.287124 codec_sdk-0.2.3/codec/resources/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-31 14:49:40.788907 codec_sdk-0.2.3/codec/resources/collections/__init__.py
+-rw-r--r--   0        0        0     1076 2024-04-02 09:17:33.564675 codec_sdk-0.2.3/codec/resources/collections/collections.py
+-rw-r--r--   0        0        0      476 2024-03-31 15:55:20.630364 codec_sdk-0.2.3/codec/resources/collections/format.py
+-rw-r--r--   0        0        0      246 2024-03-31 16:21:39.938800 codec_sdk-0.2.3/codec/resources/collections/types.py
+-rw-r--r--   0        0        0       98 2024-03-31 16:53:09.176751 codec_sdk-0.2.3/codec/resources/logger.py
+-rw-r--r--   0        0        0     2819 2024-03-31 14:50:06.360715 codec_sdk-0.2.3/codec/resources/request.py
+-rw-r--r--   0        0        0        0 2024-03-31 14:50:01.919681 codec_sdk-0.2.3/codec/resources/search/__init__.py
+-rw-r--r--   0        0        0      604 2024-03-31 16:40:39.439653 codec_sdk-0.2.3/codec/resources/search/search.py
+-rw-r--r--   0        0        0      273 2024-03-31 16:52:38.800607 codec_sdk-0.2.3/codec/resources/search/types.py
+-rw-r--r--   0        0        0       45 2024-03-27 14:23:27.578193 codec_sdk-0.2.3/codec/resources/utils/__init__.py
+-rw-r--r--   0        0        0      409 2024-03-31 14:51:05.257604 codec_sdk-0.2.3/codec/resources/utils/utils.py
+-rw-r--r--   0        0        0      597 2024-03-27 15:12:10.116736 codec_sdk-0.2.3/codec/resources/utils/webhook.py
+-rw-r--r--   0        0        0        0 2024-03-31 14:49:13.206374 codec_sdk-0.2.3/codec/resources/videos/__init__.py
+-rw-r--r--   0        0        0      371 2024-03-31 15:54:29.778454 codec_sdk-0.2.3/codec/resources/videos/format.py
+-rw-r--r--   0        0        0      486 2024-03-31 16:04:41.602700 codec_sdk-0.2.3/codec/resources/videos/types.py
+-rw-r--r--   0        0        0     2882 2024-03-31 16:39:01.854587 codec_sdk-0.2.3/codec/resources/videos/videos.py
+-rw-r--r--   0        0        0        0 2024-03-25 20:03:51.340117 codec_sdk-0.2.3/codec/utils/__init__.py
+-rw-r--r--   0        0        0      633 2024-03-26 12:38:41.420078 codec_sdk-0.2.3/codec/utils/file_utils.py
+-rw-r--r--   0        0        0      114 2024-03-31 15:35:42.827701 codec_sdk-0.2.3/codec/utils/type_utils.py
+-rw-r--r--   0        0        0      606 2024-03-31 16:16:51.826816 codec_sdk-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1903 1970-01-01 00:00:00.000000 codec_sdk-0.2.3/PKG-INFO
```

### Comparing `codec_sdk-0.2.2/.gitignore` & `codec_sdk-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `codec_sdk-0.2.2/LICENSE` & `codec_sdk-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `codec_sdk-0.2.2/README.md` & `codec_sdk-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `codec_sdk-0.2.2/codec/client.py` & `codec_sdk-0.2.3/codec/client.py`

 * *Files identical despite different names*

### Comparing `codec_sdk-0.2.2/codec/constants.py` & `codec_sdk-0.2.3/codec/constants.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 TIMEOUT_MESSAGE = "Your request cannot be processed at this time due to a timeout from the upstream server. Please try again later. If the issue persists, check our status page https://status.codec.io or contact support@codec.io for assistance."
 API_ERROR_CODES = [
     "unknown_error",
     "gateway_timeout",
     "too_many_requests",
     "auth.not_found",
     "auth.not_team_owner",
-    "expand.invalid_keys"
+    "expand.invalid_keys",
+    "auth.payment_required"
 ]
 COLLECTION_ERROR_CODES = [
     "collections.invalid_name",
     "collections.not_found"
 ]
 INDEXING_ERROR_CODES = [
     "indexer.video_not_found"
```

### Comparing `codec_sdk-0.2.2/codec/exceptions.py` & `codec_sdk-0.2.3/codec/exceptions.py`

 * *Files identical despite different names*

### Comparing `codec_sdk-0.2.2/codec/resources/collections/collections.py` & `codec_sdk-0.2.3/codec/resources/collections/collections.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,22 +2,29 @@
 from codec.resources.request import Request
 
 
 class Collections:
     def __init__(self, auth):
         self.auth = auth
 
-    def create(self, name: str):
+    def create(
+        self,
+        name: str
+    ):
         endpoint = "/collection"
-        response = Request(self.auth).post(endpoint)
+        response = Request(self.auth).post(endpoint, body={"name": name})
         response = format_collection_object(response)
         
         return response
     
-    def get(self, uid: str = None, expand: list = None):
+    def get(
+        self,
+        uid: str = None,
+        expand: list = None
+    ):
         if uid:
             endpoint = f"/collection/{uid}"
         else:
             endpoint = "/collection"
         
         expand_parameter = None if expand is None else {"expand": ",".join(expand)}
         response = Request(self.auth).get(endpoint, params=expand_parameter)
```

### Comparing `codec_sdk-0.2.2/codec/resources/request.py` & `codec_sdk-0.2.3/codec/resources/request.py`

 * *Files identical despite different names*

### Comparing `codec_sdk-0.2.2/codec/resources/search/search.py` & `codec_sdk-0.2.3/codec/resources/search/search.py`

 * *Files identical despite different names*

### Comparing `codec_sdk-0.2.2/codec/resources/utils/webhook.py` & `codec_sdk-0.2.3/codec/resources/utils/webhook.py`

 * *Files identical despite different names*

### Comparing `codec_sdk-0.2.2/codec/resources/videos/videos.py` & `codec_sdk-0.2.3/codec/resources/videos/videos.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,32 +66,47 @@
     return response
 
 
 class Videos:
     def __init__(self, auth):
         self.auth = auth
 
-    def get(self, uid: str, expand: list = None):
+    def get(
+        self,
+        uid: str,
+        expand: list = None
+    ):
         endpoint = f"/video/{uid}"
 
         expand_parameter = None if expand is None else {"expand": ",".join(expand)}
         response = Request(self.auth).get(endpoint, params=expand_parameter)
         response = format_video_object(response)
 
         return response
 
-    def delete(self, uid: str):
+    def delete(
+        self,
+        uid: str
+    ):
         endpoint = f"/video/{uid}"
         response = Request(self.auth).delete(endpoint)
         response = VideoStatusObject(**response)
 
         return response
     
-    def upload(self, path: str, collection: str):
+    def upload(
+        self,
+        path: str,
+        collection: str
+    ):
         response = _upload_video(path=path, auth=self.auth, collection=collection)
 
         return response
 
-    def index(self, uid: str, wait: bool = False):
+    def index(
+        self,
+        uid: str,
+        wait: bool = False
+    ):
         response = _index_video(uid=uid, auth=self.auth, wait=wait)
 
         return response
```

### Comparing `codec_sdk-0.2.2/codec/utils/file_utils.py` & `codec_sdk-0.2.3/codec/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `codec_sdk-0.2.2/pyproject.toml` & `codec_sdk-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `codec_sdk-0.2.2/PKG-INFO` & `codec_sdk-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codec-sdk
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python Library for the Codec API
 Author-email: Armada Labs Inc <contact@codec.io>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: requests >=2.31.0
 Requires-Dist: supabase >=1.0.3
```

