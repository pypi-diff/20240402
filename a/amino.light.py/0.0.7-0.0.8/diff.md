# Comparing `tmp/amino.light.py-0.0.7.tar.gz` & `tmp/amino.light.py-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amino.light.py-0.0.7.tar", last modified: Fri Mar 29 01:42:46 2024, max compression
+gzip compressed data, was "amino.light.py-0.0.8.tar", last modified: Tue Apr  2 15:12:27 2024, max compression
```

## Comparing `amino.light.py-0.0.7.tar` & `amino.light.py-0.0.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-03-29 01:42:46.370000 amino.light.py-0.0.7/
-drwxrwxrwx   0        0        0        0 2024-03-29 01:42:46.344991 amino.light.py-0.0.7/AminoLightPy/
--rw-rw-rw-   0        0        0      262 2024-03-29 01:37:10.000000 amino.light.py-0.0.7/AminoLightPy/__init__.py
--rw-rw-rw-   0        0        0     9363 2024-03-29 00:27:12.000000 amino.light.py-0.0.7/AminoLightPy/acm.py
--rw-rw-rw-   0        0        0    70188 2024-03-29 01:02:11.000000 amino.light.py-0.0.7/AminoLightPy/client.py
--rw-rw-rw-   0        0        0     1762 2024-03-29 01:02:12.000000 amino.light.py-0.0.7/AminoLightPy/constants.py
-drwxrwxrwx   0        0        0        0 2024-03-29 01:42:46.345991 amino.light.py-0.0.7/AminoLightPy/lib/
--rw-rw-rw-   0        0        0        0 2023-02-13 07:38:45.000000 amino.light.py-0.0.7/AminoLightPy/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-29 01:42:46.349990 amino.light.py-0.0.7/AminoLightPy/lib/util/
--rw-rw-rw-   0        0        0       73 2024-03-27 16:01:15.000000 amino.light.py-0.0.7/AminoLightPy/lib/util/__init__.py
--rw-rw-rw-   0        0        0    31621 2024-03-29 00:26:02.000000 amino.light.py-0.0.7/AminoLightPy/lib/util/exceptions.py
--rw-rw-rw-   0        0        0     1238 2024-03-29 00:27:48.000000 amino.light.py-0.0.7/AminoLightPy/lib/util/helpers.py
--rw-rw-rw-   0        0        0   163863 2024-03-29 00:27:06.000000 amino.light.py-0.0.7/AminoLightPy/lib/util/objects.py
--rw-rw-rw-   0        0        0    11163 2024-03-29 01:00:51.000000 amino.light.py-0.0.7/AminoLightPy/socket.py
--rw-rw-rw-   0        0        0    73275 2024-03-29 00:23:56.000000 amino.light.py-0.0.7/AminoLightPy/sub_client.py
--rw-rw-rw-   0        0        0     1384 2024-03-29 01:42:46.369000 amino.light.py-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      878 2024-03-29 01:32:56.000000 amino.light.py-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-03-29 01:42:46.366989 amino.light.py-0.0.7/amino.light.py.egg-info/
--rw-rw-rw-   0        0        0     1384 2024-03-29 01:42:46.000000 amino.light.py-0.0.7/amino.light.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      526 2024-03-29 01:42:46.000000 amino.light.py-0.0.7/amino.light.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-29 01:42:46.000000 amino.light.py-0.0.7/amino.light.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-03-29 01:42:46.000000 amino.light.py-0.0.7/amino.light.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-03-29 01:42:46.000000 amino.light.py-0.0.7/amino.light.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-29 01:42:46.371994 amino.light.py-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      869 2024-03-29 01:42:30.000000 amino.light.py-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 15:12:27.161224 amino.light.py-0.0.8/
+drwxrwxrwx   0        0        0        0 2024-04-02 15:12:27.129531 amino.light.py-0.0.8/AminoLightPy/
+-rw-rw-rw-   0        0        0      287 2024-03-31 23:25:44.000000 amino.light.py-0.0.8/AminoLightPy/__init__.py
+-rw-rw-rw-   0        0        0     9363 2024-03-29 00:27:12.000000 amino.light.py-0.0.8/AminoLightPy/acm.py
+-rw-rw-rw-   0        0        0    70320 2024-03-30 19:18:45.000000 amino.light.py-0.0.8/AminoLightPy/client.py
+-rw-rw-rw-   0        0        0     1513 2024-03-30 16:04:39.000000 amino.light.py-0.0.8/AminoLightPy/constants.py
+drwxrwxrwx   0        0        0        0 2024-04-02 15:12:27.130530 amino.light.py-0.0.8/AminoLightPy/lib/
+-rw-rw-rw-   0        0        0        0 2023-02-13 07:38:45.000000 amino.light.py-0.0.8/AminoLightPy/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 15:12:27.136534 amino.light.py-0.0.8/AminoLightPy/lib/util/
+-rw-rw-rw-   0        0        0       73 2024-03-27 16:01:15.000000 amino.light.py-0.0.8/AminoLightPy/lib/util/__init__.py
+-rw-rw-rw-   0        0        0    31621 2024-03-29 00:26:02.000000 amino.light.py-0.0.8/AminoLightPy/lib/util/exceptions.py
+-rw-rw-rw-   0        0        0     1238 2024-03-30 22:17:35.000000 amino.light.py-0.0.8/AminoLightPy/lib/util/helpers.py
+-rw-rw-rw-   0        0        0   100212 2024-04-02 15:03:13.000000 amino.light.py-0.0.8/AminoLightPy/lib/util/objects.py
+-rw-rw-rw-   0        0        0    11163 2024-03-29 01:00:51.000000 amino.light.py-0.0.8/AminoLightPy/socket.py
+-rw-rw-rw-   0        0        0    73627 2024-03-30 19:42:47.000000 amino.light.py-0.0.8/AminoLightPy/sub_client.py
+-rw-rw-rw-   0        0        0     1417 2024-04-02 15:12:27.161224 amino.light.py-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      878 2024-03-29 01:32:56.000000 amino.light.py-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 15:12:27.160222 amino.light.py-0.0.8/amino.light.py.egg-info/
+-rw-rw-rw-   0        0        0     1417 2024-04-02 15:12:26.000000 amino.light.py-0.0.8/amino.light.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      526 2024-04-02 15:12:27.000000 amino.light.py-0.0.8/amino.light.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 15:12:26.000000 amino.light.py-0.0.8/amino.light.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-04-02 15:12:26.000000 amino.light.py-0.0.8/amino.light.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-02 15:12:26.000000 amino.light.py-0.0.8/amino.light.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-02 15:12:27.163224 amino.light.py-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      889 2024-04-02 15:12:23.000000 amino.light.py-0.0.8/setup.py
```

### Comparing `amino.light.py-0.0.7/AminoLightPy/acm.py` & `amino.light.py-0.0.8/AminoLightPy/acm.py`

 * *Files identical despite different names*

### Comparing `amino.light.py-0.0.7/AminoLightPy/client.py` & `amino.light.py-0.0.8/AminoLightPy/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,15 +162,16 @@
         **Parameters**
             - **SID** : SID of the account
         """
         userId = helpers.sid_to_uid(SID)
         self.authenticated = True
         self.sid = SID
 
-        self.profile: objects.UserProfile = self.get_user_info(userId)
+        self.profile: objects.UserProfile = objects.UserProfile({"uid": userId}).UserProfile
+        # self.profile: objects.UserProfile = self.get_user_info(userId)
     
         self.session.headers.update({
             "NDCAUTH": f"sid={self.sid}",
             "AUID": self.profile.userId
             })
 
         self.profile.session = self.session
@@ -191,15 +192,16 @@
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
 
         data = {
             "email": email,
             "secret": f"0 {password}",
-            "clientType": 300
+            "clientType": 100,
+            "deviceID": device_id
         }
 
         response = self.session.post(f"{api}/g/s/auth/login", json=data)
         self.authenticated = True
         json = response.json()
         self.sid = json["sid"]
         self.profile: objects.UserProfile = objects.UserProfile(json["userProfile"]).UserProfile
```

### Comparing `amino.light.py-0.0.7/AminoLightPy/constants.py` & `amino.light.py-0.0.8/AminoLightPy/constants.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,41 @@
 from time import time
 from json import dumps
-from random import randint
 from requests import Session
 from .lib.util import signature, gen_deviceId
 from .lib.util.exceptions import CheckException
 
 # add by August Light
 
 api = "http://service.aminoapps.com:80/api/v1"
 device_id = gen_deviceId()
 
 class CustomSession(Session):
+    def __init__(self) -> None:
+        super().__init__()
+        self.headers.update({
+            "NDCDEVICEID": device_id,
+            "User-Agent": "Apple iPhone13,1 iOS v16.5 Main/3.19.0"
+        })
+
     def request(self, method, url, *args, **kwargs):
 
         headers = kwargs.setdefault("headers", {})
 
         if method.lower() == "post":
-            if "data" in kwargs or "json" in kwargs:
-                data = kwargs.get('data') or kwargs.get("json")
+            if "json" in kwargs:
+                data = kwargs.get("json")
                 
                 data["timestamp"] = int(time() * 1000)
-
-                if not isinstance(data, str):
-                    try:
-                        data = dumps(data)
-                    except (TypeError, ValueError):
-                        print("Error: data must be structure JSON")
-                        return None
-
+                data  = dumps(data)
                 headers["Content-Type"] = "application/json"
                 headers["NDC-MSG-SIG"] = signature(data)
 
             else:
                 headers["Content-Type"] = "application/x-www-form-urlencoded"
-            
-        headers["NDCDEVICEID"] = device_id
-        headers["User-Agent"] = f"Apple iPhone{randint(0,99999)},1 iOS v16.5 Main/3.19.0"
 
         response = super().request(method, url, *args, **kwargs)
 
         if response.status_code != 200:
             CheckException(response.text)
 
         return response
```

### Comparing `amino.light.py-0.0.7/AminoLightPy/lib/util/exceptions.py` & `amino.light.py-0.0.8/AminoLightPy/lib/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `amino.light.py-0.0.7/AminoLightPy/lib/util/helpers.py` & `amino.light.py-0.0.8/AminoLightPy/lib/util/helpers.py`

 * *Files identical despite different names*

### Comparing `amino.light.py-0.0.7/AminoLightPy/socket.py` & `amino.light.py-0.0.8/AminoLightPy/socket.py`

 * *Files identical despite different names*

### Comparing `amino.light.py-0.0.7/AminoLightPy/sub_client.py` & `amino.light.py-0.0.8/AminoLightPy/sub_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -565,14 +565,17 @@
         if asGuest: flg = "g-flag"
         else: flg = "flag"
 
         
         response = self.session.post(f"{api}/x{self.comId}/s/{flg}", json=data)
         return response.status_code
 
+    def check_values(self, *args):
+        return any(arg is None for arg in args)
+
     def send_message(self, chatId: str, message: str = None, messageType: int = 0, file: BinaryIO = None, fileType: str = None, replyTo: str = None, mentionUserIds: list = None, stickerId: str = None, embedId: str = None, embedType: int = None, embedLink: str = None, embedTitle: str = None, embedContent: str = None, embedImage: BinaryIO = None):
         """
         Send a Message to a Chat.
 
         **Parameters**
             - **message** : Message to be sent
             - **chatId** : ID of the Chat.
@@ -590,70 +593,81 @@
             - **embedId** : ID of the Embed.
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-
-        if message is not None and file is None:
-            message = message.replace("<$", "‎‏").replace("$>", "‬‭")
-
-        mentions = []
-        if mentionUserIds:
-            for mention_uid in mentionUserIds:
-                mentions.append({"uid": mention_uid})
-
-        if embedImage:
-            embedImage = [[100, self.upload_media(embedImage, "image"), None]]
+        
 
         data = {
             "type": messageType,
-            "content": message,
-            "clientRefId": int(timestamp() / 10 % 1000000000),
-            "attachedObject": {
-                "objectId": embedId,
-                "objectType": embedType,
-                "link": embedLink,
-                "title": embedTitle,
-                "content": embedContent,
-                "mediaList": embedImage
-            },
-            "extensions": { "mentionedArray": mentions }
+            "content": message
         }
+        
+        # if self.check_values(embedId, embedType, embedLink, embedTitle, embedContent, embedImage):
+        #     attachedObject = dict()
 
-        if replyTo: data["replyMessageId"] = replyTo
-
-        if stickerId:
-            data["content"] = None
-            data["stickerId"] = stickerId
-            data["type"] = 3
+        #     if embedId:
+        #         attachedObject["objectId"] = embedId
 
-        if file:
-            data["content"] = None
-            if fileType == "audio":
-                data["type"] = 2
-                data["mediaType"] = 110
+        #     if embedType:
+        #         attachedObject["objectType"] = embedType
 
-            elif fileType == "image":
-                data["mediaType"] = 100
-                data["mediaUploadValueContentType"] = "image/jpg"
-                data["mediaUhqEnabled"] = True
+        #     if embedLink:
+        #         attachedObject["link"] = embedLink
 
-            elif fileType == "gif":
-                data["mediaType"] = 100
-                data["mediaUploadValueContentType"] = "image/gif"
-                data["mediaUhqEnabled"] = True
+        #     if embedTitle:
+        #         attachedObject["title"] = embedTitle
 
-            else: raise exceptions.SpecifyType(fileType)
+        #     if embedContent:
+        #         attachedObject["content"] = embedContent
 
-            data["mediaUploadValue"] = b64encode(file.read()).decode()
+        #     if embedImage:
+        #         attachedObject["mediaList"] = [[100, self.upload_media(embedImage, "image"), None]]
 
+        #     data["attachedObject"] = attachedObject
+        
+        # if mentionUserIds:
+        #     mentions = [{"uid": mention_uid} for mention_uid in mentionUserIds]
+        #     data["extensions"] = {"mentionedArray": mentions}
+
+        # if replyTo: data["replyMessageId"] = replyTo
+
+        # if stickerId:
+        #     data["content"] = None
+        #     data["stickerId"] = stickerId
+        #     data["type"] = 3
+
+        # if file:
+        #     data["content"] = None
+        #     if fileType == "audio":
+        #         data["type"] = 2
+        #         data["mediaType"] = 110
+
+        #     elif fileType == "image":
+        #         data["mediaType"] = 100
+        #         data["mediaUploadValueContentType"] = "image/jpg"
+        #         data["mediaUhqEnabled"] = True
+
+        #     elif fileType == "gif":
+        #         data["mediaType"] = 100
+        #         data["mediaUploadValueContentType"] = "image/gif"
+        #         data["mediaUhqEnabled"] = True
+
+        #     else: raise exceptions.SpecifyType(fileType)
+
+        #     data["mediaUploadValue"] = b64encode(file.read()).decode()
+
+
+        response = self.session.post(
+            url=f"{api}/x{self.comId}/s/chat/thread/{chatId}/message",
+            json=data
+        )
 
-        response = self.session.post(f"{api}/x{self.comId}/s/chat/thread/{chatId}/message", json=data)
         return response.status_code
 
     def full_embed(self, link: str, image: BinaryIO, message: str, chatId: str):
         data = {
             "type": 0,
             "content": message,
             "extensions": {
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `amino.light.py-0.0.7/PKG-INFO` & `amino.light.py-0.0.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: amino.light.py
-Version: 0.0.7
+Version: 0.0.8
 Summary: Best Amino.py alternative
 Author: AugustLight
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 Requires-Dist: requests
+Requires-Dist: websocket-client
 
 # AminoLightPy
 ## _The best Amino.py alternative!_
 
 Why should you choose this library?
 
 ## Features
```

### Comparing `amino.light.py-0.0.7/README.md` & `amino.light.py-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `amino.light.py-0.0.7/amino.light.py.egg-info/PKG-INFO` & `amino.light.py-0.0.8/amino.light.py.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: amino.light.py
-Version: 0.0.7
+Version: 0.0.8
 Summary: Best Amino.py alternative
 Author: AugustLight
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 Requires-Dist: requests
+Requires-Dist: websocket-client
 
 # AminoLightPy
 ## _The best Amino.py alternative!_
 
 Why should you choose this library?
 
 ## Features
```

### Comparing `amino.light.py-0.0.7/amino.light.py.egg-info/SOURCES.txt` & `amino.light.py-0.0.8/amino.light.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amino.light.py-0.0.7/setup.py` & `amino.light.py-0.0.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="amino.light.py",
-    version="0.0.7",
+    version="0.0.8",
     license="MIT",
     description="Best Amino.py alternative",
     author="AugustLight",
     packages=find_packages(),
-    install_requires=["requests"],
+    install_requires=["requests", "websocket-client"],
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
```

