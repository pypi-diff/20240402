# Comparing `tmp/aepp-0.3.4.tar.gz` & `tmp/aepp-0.3.4.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aepp-0.3.4.tar", last modified: Mon Mar 18 13:52:32 2024, max compression
+gzip compressed data, was "aepp-0.3.4.post1.tar", last modified: Tue Apr  2 10:50:42 2024, max compression
```

## Comparing `aepp-0.3.4.tar` & `aepp-0.3.4.post1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2024-03-18 13:52:32.855309 aepp-0.3.4/
--rw-rw-rw-   0        0        0    10337 2023-05-10 18:38:24.000000 aepp-0.3.4/LICENSE
--rw-rw-rw-   0        0        0       16 2023-05-10 18:38:24.000000 aepp-0.3.4/MANIFEST.in
--rw-rw-rw-   0        0        0     4268 2024-03-18 13:52:32.855309 aepp-0.3.4/PKG-INFO
--rw-rw-rw-   0        0        0     3457 2024-03-18 13:44:44.000000 aepp-0.3.4/README.md
-drwxrwxrwx   0        0        0        0 2024-03-18 13:52:32.778849 aepp-0.3.4/aepp/
--rw-rw-rw-   0        0        0     5224 2023-05-10 18:04:54.000000 aepp-0.3.4/aepp/__init__.py
--rw-rw-rw-   0        0        0       23 2024-03-18 13:51:23.000000 aepp-0.3.4/aepp/__version__.py
--rw-rw-rw-   0        0        0    17426 2024-02-21 09:35:17.000000 aepp-0.3.4/aepp/accesscontrol.py
--rw-rw-rw-   0        0        0    58818 2024-03-18 13:33:11.000000 aepp-0.3.4/aepp/catalog.py
--rw-rw-rw-   0        0        0     2579 2024-03-18 11:49:30.000000 aepp-0.3.4/aepp/config.py
--rw-rw-rw-   0        0        0    17655 2024-02-21 09:35:17.000000 aepp-0.3.4/aepp/configs.py
--rw-rw-rw-   0        0        0    30254 2024-02-21 09:35:17.000000 aepp-0.3.4/aepp/connector.py
--rw-rw-rw-   0        0        0    42510 2024-02-21 09:35:17.000000 aepp-0.3.4/aepp/customerprofile.py
--rw-rw-rw-   0        0        0    14252 2023-11-02 07:50:23.000000 aepp-0.3.4/aepp/dataaccess.py
--rw-rw-rw-   0        0        0    27357 2023-11-02 07:50:23.000000 aepp-0.3.4/aepp/dataprep.py
--rw-rw-rw-   0        0        0     8778 2023-11-02 07:50:23.000000 aepp-0.3.4/aepp/datasets.py
--rw-rw-rw-   0        0        0    24348 2023-11-02 07:50:23.000000 aepp-0.3.4/aepp/destination.py
--rw-rw-rw-   0        0        0     5378 2023-11-02 07:50:23.000000 aepp-0.3.4/aepp/destinationinstanceservice.py
--rw-rw-rw-   0        0        0    18629 2023-09-28 14:47:02.000000 aepp-0.3.4/aepp/exportDatasetToDataLandingZone.py
--rw-rw-rw-   0        0        0    76765 2023-12-04 09:42:32.000000 aepp-0.3.4/aepp/flowservice.py
--rw-rw-rw-   0        0        0    13075 2024-03-18 13:42:09.000000 aepp-0.3.4/aepp/hygiene.py
--rw-rw-rw-   0        0        0    20080 2024-02-21 09:35:17.000000 aepp-0.3.4/aepp/identity.py
--rw-rw-rw-   0        0        0    21460 2023-11-02 07:50:23.000000 aepp-0.3.4/aepp/ingestion.py
--rw-rw-rw-   0        0        0     9951 2023-11-02 07:50:23.000000 aepp-0.3.4/aepp/observability.py
--rw-rw-rw-   0        0        0    24930 2023-11-02 07:50:23.000000 aepp-0.3.4/aepp/policy.py
--rw-rw-rw-   0        0        0     8794 2023-11-02 07:50:23.000000 aepp-0.3.4/aepp/privacyservice.py
--rw-rw-rw-   0        0        0    52507 2023-11-02 07:50:24.000000 aepp-0.3.4/aepp/queryservice.py
--rw-rw-rw-   0        0        0    21063 2023-11-02 07:50:24.000000 aepp-0.3.4/aepp/sandboxes.py
--rw-rw-rw-   0        0        0   215461 2024-03-01 18:04:45.000000 aepp-0.3.4/aepp/schema.py
--rw-rw-rw-   0        0        0    38660 2024-02-21 09:35:17.000000 aepp-0.3.4/aepp/segmentation.py
--rw-rw-rw-   0        0        0     7761 2023-10-23 08:56:18.000000 aepp-0.3.4/aepp/sensei.py
--rw-rw-rw-   0        0        0     1200 2023-10-23 08:56:14.000000 aepp-0.3.4/aepp/utils.py
-drwxrwxrwx   0        0        0        0 2024-03-18 13:52:32.836228 aepp-0.3.4/aepp.egg-info/
--rw-rw-rw-   0        0        0     4268 2024-03-18 13:52:32.000000 aepp-0.3.4/aepp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      928 2024-03-18 13:52:32.000000 aepp-0.3.4/aepp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-18 13:52:32.000000 aepp-0.3.4/aepp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-03-18 13:52:32.000000 aepp-0.3.4/aepp.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-03-18 13:52:32.000000 aepp-0.3.4/aepp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-18 13:52:32.855309 aepp-0.3.4/setup.cfg
--rw-rw-rw-   0        0        0     2206 2023-11-23 12:55:39.000000 aepp-0.3.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-18 13:52:32.836228 aepp-0.3.4/tests/
--rw-rw-rw-   0        0        0      623 2023-05-10 18:04:54.000000 aepp-0.3.4/tests/__init__.py
--rw-rw-rw-   0        0        0     2246 2023-05-10 18:04:54.000000 aepp-0.3.4/tests/catalog_test.py
--rw-rw-rw-   0        0        0     1238 2023-05-10 18:04:54.000000 aepp-0.3.4/tests/dataaccess_test.py
--rw-rw-rw-   0        0        0     1093 2023-05-10 18:04:54.000000 aepp-0.3.4/tests/datasets_test.py
--rw-rw-rw-   0        0        0     2105 2023-05-23 14:25:29.000000 aepp-0.3.4/tests/destinationinstanceservice_test.py
--rw-rw-rw-   0        0        0     7684 2023-09-28 14:47:02.000000 aepp-0.3.4/tests/exportDatasetToDatalandingZone_test.py
--rw-rw-rw-   0        0        0     4208 2023-05-10 18:04:54.000000 aepp-0.3.4/tests/flowservice_test.py
--rw-rw-rw-   0        0        0     2774 2023-05-10 18:04:54.000000 aepp-0.3.4/tests/schema_test.py
+drwxrwxrwx   0        0        0        0 2024-04-02 10:50:42.118875 aepp-0.3.4.post1/
+-rw-rw-rw-   0        0        0    10337 2023-05-10 18:38:24.000000 aepp-0.3.4.post1/LICENSE
+-rw-rw-rw-   0        0        0       16 2023-05-10 18:38:24.000000 aepp-0.3.4.post1/MANIFEST.in
+-rw-rw-rw-   0        0        0     4274 2024-04-02 10:50:42.118875 aepp-0.3.4.post1/PKG-INFO
+-rw-rw-rw-   0        0        0     3457 2024-03-18 13:57:44.000000 aepp-0.3.4.post1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 10:50:42.053016 aepp-0.3.4.post1/aepp/
+-rw-rw-rw-   0        0        0     5224 2023-05-10 18:04:54.000000 aepp-0.3.4.post1/aepp/__init__.py
+-rw-rw-rw-   0        0        0       25 2024-03-25 07:12:28.000000 aepp-0.3.4.post1/aepp/__version__.py
+-rw-rw-rw-   0        0        0    17426 2024-02-21 09:35:17.000000 aepp-0.3.4.post1/aepp/accesscontrol.py
+-rw-rw-rw-   0        0        0    58818 2024-03-18 13:57:44.000000 aepp-0.3.4.post1/aepp/catalog.py
+-rw-rw-rw-   0        0        0     2579 2024-03-18 13:57:44.000000 aepp-0.3.4.post1/aepp/config.py
+-rw-rw-rw-   0        0        0    17655 2024-02-21 09:35:17.000000 aepp-0.3.4.post1/aepp/configs.py
+-rw-rw-rw-   0        0        0    30251 2024-03-20 09:24:20.000000 aepp-0.3.4.post1/aepp/connector.py
+-rw-rw-rw-   0        0        0    42510 2024-02-21 09:35:17.000000 aepp-0.3.4.post1/aepp/customerprofile.py
+-rw-rw-rw-   0        0        0    14252 2023-11-02 07:50:23.000000 aepp-0.3.4.post1/aepp/dataaccess.py
+-rw-rw-rw-   0        0        0    27357 2023-11-02 07:50:23.000000 aepp-0.3.4.post1/aepp/dataprep.py
+-rw-rw-rw-   0        0        0     8778 2023-11-02 07:50:23.000000 aepp-0.3.4.post1/aepp/datasets.py
+-rw-rw-rw-   0        0        0    24348 2023-11-02 07:50:23.000000 aepp-0.3.4.post1/aepp/destination.py
+-rw-rw-rw-   0        0        0     5378 2023-11-02 07:50:23.000000 aepp-0.3.4.post1/aepp/destinationinstanceservice.py
+-rw-rw-rw-   0        0        0    18629 2023-09-28 14:47:02.000000 aepp-0.3.4.post1/aepp/exportDatasetToDataLandingZone.py
+-rw-rw-rw-   0        0        0    76765 2023-12-04 09:42:32.000000 aepp-0.3.4.post1/aepp/flowservice.py
+-rw-rw-rw-   0        0        0    13075 2024-03-18 13:57:44.000000 aepp-0.3.4.post1/aepp/hygiene.py
+-rw-rw-rw-   0        0        0    20080 2024-02-21 09:35:17.000000 aepp-0.3.4.post1/aepp/identity.py
+-rw-rw-rw-   0        0        0    21460 2024-03-25 07:12:28.000000 aepp-0.3.4.post1/aepp/ingestion.py
+-rw-rw-rw-   0        0        0     9951 2023-11-02 07:50:23.000000 aepp-0.3.4.post1/aepp/observability.py
+-rw-rw-rw-   0        0        0    24930 2023-11-02 07:50:23.000000 aepp-0.3.4.post1/aepp/policy.py
+-rw-rw-rw-   0        0        0     8794 2023-11-02 07:50:23.000000 aepp-0.3.4.post1/aepp/privacyservice.py
+-rw-rw-rw-   0        0        0    52507 2023-11-02 07:50:24.000000 aepp-0.3.4.post1/aepp/queryservice.py
+-rw-rw-rw-   0        0        0    21063 2023-11-02 07:50:24.000000 aepp-0.3.4.post1/aepp/sandboxes.py
+-rw-rw-rw-   0        0        0   215461 2024-03-01 18:04:45.000000 aepp-0.3.4.post1/aepp/schema.py
+-rw-rw-rw-   0        0        0    42269 2024-03-25 07:12:28.000000 aepp-0.3.4.post1/aepp/segmentation.py
+-rw-rw-rw-   0        0        0     7761 2023-10-23 08:56:18.000000 aepp-0.3.4.post1/aepp/sensei.py
+-rw-rw-rw-   0        0        0     1200 2023-10-23 08:56:14.000000 aepp-0.3.4.post1/aepp/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-02 10:50:42.118875 aepp-0.3.4.post1/aepp.egg-info/
+-rw-rw-rw-   0        0        0     4274 2024-04-02 10:50:41.000000 aepp-0.3.4.post1/aepp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      928 2024-04-02 10:50:41.000000 aepp-0.3.4.post1/aepp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 10:50:41.000000 aepp-0.3.4.post1/aepp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-04-02 10:50:41.000000 aepp-0.3.4.post1/aepp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-02 10:50:41.000000 aepp-0.3.4.post1/aepp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-02 10:50:42.118875 aepp-0.3.4.post1/setup.cfg
+-rw-rw-rw-   0        0        0     2206 2023-11-23 12:55:39.000000 aepp-0.3.4.post1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 10:50:42.113944 aepp-0.3.4.post1/tests/
+-rw-rw-rw-   0        0        0      623 2023-05-10 18:04:54.000000 aepp-0.3.4.post1/tests/__init__.py
+-rw-rw-rw-   0        0        0     2246 2023-05-10 18:04:54.000000 aepp-0.3.4.post1/tests/catalog_test.py
+-rw-rw-rw-   0        0        0     1238 2023-05-10 18:04:54.000000 aepp-0.3.4.post1/tests/dataaccess_test.py
+-rw-rw-rw-   0        0        0     1093 2023-05-10 18:04:54.000000 aepp-0.3.4.post1/tests/datasets_test.py
+-rw-rw-rw-   0        0        0     2105 2023-05-23 14:25:29.000000 aepp-0.3.4.post1/tests/destinationinstanceservice_test.py
+-rw-rw-rw-   0        0        0     7684 2023-09-28 14:47:02.000000 aepp-0.3.4.post1/tests/exportDatasetToDatalandingZone_test.py
+-rw-rw-rw-   0        0        0     4208 2023-05-10 18:04:54.000000 aepp-0.3.4.post1/tests/flowservice_test.py
+-rw-rw-rw-   0        0        0     2774 2023-05-10 18:04:54.000000 aepp-0.3.4.post1/tests/schema_test.py
```

### Comparing `aepp-0.3.4/LICENSE` & `aepp-0.3.4.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4/PKG-INFO` & `aepp-0.3.4.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aepp
-Version: 0.3.4
+Version: 0.3.4.post1
 Summary: Package to manage AEP API endpoint and some helper functions
 Home-page: https://github.com/adobe/aepp
 Author: Julien Piccini
 Author-email: piccini.julien@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `aepp-0.3.4/README.md` & `aepp-0.3.4.post1/README.md`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4/aepp/__init__.py` & `aepp-0.3.4.post1/aepp/__init__.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4/aepp/accesscontrol.py` & `aepp-0.3.4.post1/aepp/accesscontrol.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4/aepp/catalog.py` & `aepp-0.3.4.post1/aepp/catalog.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4/aepp/config.py` & `aepp-0.3.4.post1/aepp/config.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4/aepp/configs.py` & `aepp-0.3.4.post1/aepp/configs.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4/aepp/connector.py` & `aepp-0.3.4.post1/aepp/connector.py`

 * *Files 0% similar despite different names*

```diff
@@ -286,15 +286,15 @@
         if now > self.config["date_limit"]:
             if self.loggingEnabled:
                 self.logger.warning("token expired. Trying to retrieve a new token")
             if self.connectionType == 'jwt':
                 token_with_expiry = self.get_jwt_token_and_expiry_for_config(config=self.config)
             elif self.connectionType == 'oauthV1' or self.connectionType == 'oauthV2':
                 token_with_expiry = self.get_oauth_token_and_expiry_for_config(config=self.config)
-            self.token = token_with_expiry["token"]
+            self.token = token_with_expiry.token
             self.config["token"] = self.token
             if self.loggingEnabled:
                 self.logger.info("new token retrieved : {self.token}")
             self.header.update({"Authorization": f"Bearer {self.token}"})
             if self.connectionType == 'jwt':
                 timeScale = 1000 ## jwt returns milliseconds expiry
             elif self.connectionType == 'oauthV1' or self.connectionType == 'oauthV2':
```

### Comparing `aepp-0.3.4/aepp/customerprofile.py` & `aepp-0.3.4.post1/aepp/customerprofile.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4/aepp/dataaccess.py` & `aepp-0.3.4.post1/aepp/dataaccess.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4/aepp/dataprep.py` & `aepp-0.3.4.post1/aepp/dataprep.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4/aepp/datasets.py` & `aepp-0.3.4.post1/aepp/datasets.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4/aepp/destination.py` & `aepp-0.3.4.post1/aepp/destination.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4/aepp/destinationinstanceservice.py` & `aepp-0.3.4.post1/aepp/destinationinstanceservice.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4/aepp/exportDatasetToDataLandingZone.py` & `aepp-0.3.4.post1/aepp/exportDatasetToDataLandingZone.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4/aepp/flowservice.py` & `aepp-0.3.4.post1/aepp/flowservice.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4/aepp/hygiene.py` & `aepp-0.3.4.post1/aepp/hygiene.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4/aepp/identity.py` & `aepp-0.3.4.post1/aepp/identity.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4/aepp/ingestion.py` & `aepp-0.3.4.post1/aepp/ingestion.py`

 * *Files 0% similar despite different names*

```diff
@@ -237,15 +237,15 @@
         if self.loggingEnabled:
             self.logger.debug(f"uploadSmallFile as format: ({type(data)})")
         privateHeader = deepcopy(self.header)
         privateHeader["Content-Type"] = "application/octet-stream"
         path = f"/batches/{batchId}/datasets/{datasetId}/files/{filePath}"
         if type(data) == str:
             if '.json' in data:
-                with open(Path(path),'r') as f:
+                with open(Path(data),'r') as f:
                     data = json.load(f)
         res = self.connector.putData(
             self.endpoint + path, data=data, headers=privateHeader
         )
         return res
 
     def uploadSmallFileFinish(
```

### Comparing `aepp-0.3.4/aepp/observability.py` & `aepp-0.3.4.post1/aepp/observability.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4/aepp/policy.py` & `aepp-0.3.4.post1/aepp/policy.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4/aepp/privacyservice.py` & `aepp-0.3.4.post1/aepp/privacyservice.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4/aepp/queryservice.py` & `aepp-0.3.4.post1/aepp/queryservice.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4/aepp/sandboxes.py` & `aepp-0.3.4.post1/aepp/sandboxes.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4/aepp/schema.py` & `aepp-0.3.4.post1/aepp/schema.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4/aepp/segmentation.py` & `aepp-0.3.4.post1/aepp/segmentation.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from aepp import connector
 import time
 from concurrent import futures
 import logging
 from typing import Union
 from copy import deepcopy
 from .configs import ConnectObject
-import json
+import json, re
 
 class Segmentation:
     """
     A class containing methods to use on segmentation.
     A complete documentation can be found here:
     https://www.adobe.io/apis/experienceplatform/home/api-reference.html#!acpdr/swagger-specs/segmentation.yaml
     """
@@ -894,9 +894,76 @@
             raise ValueError("Require a new definition")
         if self.loggingEnabled:
             self.logger.debug(f"Starting putAudience for audienceId: {audienceId}")
         path = f"/audiences/{audienceId}"
         res = self.connector.putData(self.endpoint + path,data=audienceObj)
         return res
     
+    def __pqlJSONSegmentReader__(self,segmentValue:Union[str,dict],listFields=None,tmp_str=None)->list:
+        """
+        read the dictionary of the segment.expression.value
+        use listFields and tmp_str to pass data in recursive mode
+        return a list of paths
+        """
+        if type(segmentValue) == str:
+            json_data = json.loads(segmentValue)
+        else:
+            json_data = segmentValue
+        if listFields is None:
+            listFields = list()
+        for key in json_data:
+            if type(json_data[key]) == dict and key != 'object': ## if needs to be recursively checked, needs to pass the list already found
+                tmp_str = self.__pqlJSONSegmentReader__(json_data[key],listFields=listFields)
+            elif type(json_data[key]) == list: ## if needs to be looped through
+                for var in json_data[key]:
+                    if type(var) == dict: ## if element is a dict, it can be recursively checked, need to pass the list already found
+                        tmp_str = self.__pqlJSONSegmentReader__(var,listFields=listFields)
+            elif json_data[key] == 'fieldLookup': ## if the key is fieldLookup the path is built
+                if tmp_str is None: # if first element of the path
+                    tmp_str = json_data['fieldName']
+                else:
+                    tmp_str = f"{json_data['fieldName']}.{tmp_str}"
+                if 'object' in json_data.keys() and 'fieldName' in json_data.get('object',{}).keys(): ## if there is a lower/higher node to be added, passing the incomplete node and the list already found
+                    tmp_str = self.__pqlJSONSegmentReader__(json_data['object'],tmp_str=tmp_str,listFields=listFields)
+                else: ## if end of the nodes, just adding the path to the list of path found
+                    listFields.append(tmp_str)
+                    return tmp_str
+        return list(set(listFields))
+    
 
+    def extractPaths(self,audience:Union[dict,str]=None,recursive:bool=False)->list:
+        """
+        BETA
+        Extract the schema paths present in the segment or audience definition.
+        Argument:
+            audience : REQUIRED : Audience or segment definition.
+        """
+        if audience is None:
+            raise ValueError("require an audience or segment definition")
+        if type(audience) == str:
+            audience = self.getAudience(audience)
+        formatt = audience.get('expression',{}).get('format')
+        if formatt == 'pql/text':
+            paths = re.findall('WHAT\((.+?)\.[^\.]+\(',audience.get('expression',{}).get('value'))
+            return paths
+        if formatt == 'pql/json':
+            paths = self.__pqlJSONSegmentReader__(audience.get('expression',{}).get('value'))
+            if recursive:
+                dependencies = self.extractAudiences(audience)
+                if len(dependencies) > 0:
+                    for dependency in dependencies:
+                        paths += self.extractPaths(dependency, recursive=True)
+            return paths
+
+    def extractAudiences(self,audience:dict=None)->list:
+        """
+        BETA
+        Extract the audience Id used in the audience definition.
+        In case you have build audience of audience.
+        Argument: 
+            audience : REQUIRED : Audience or Segment definition
+        """
+        if audience is None:
+            raise ValueError("require an audience or segment definition")
+        dependencies = audience.get('dependencies',[])
+        return dependencies
```

### Comparing `aepp-0.3.4/aepp/sensei.py` & `aepp-0.3.4.post1/aepp/sensei.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4/aepp/utils.py` & `aepp-0.3.4.post1/aepp/utils.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4/aepp.egg-info/PKG-INFO` & `aepp-0.3.4.post1/aepp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aepp
-Version: 0.3.4
+Version: 0.3.4.post1
 Summary: Package to manage AEP API endpoint and some helper functions
 Home-page: https://github.com/adobe/aepp
 Author: Julien Piccini
 Author-email: piccini.julien@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `aepp-0.3.4/aepp.egg-info/SOURCES.txt` & `aepp-0.3.4.post1/aepp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4/setup.py` & `aepp-0.3.4.post1/setup.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4/tests/__init__.py` & `aepp-0.3.4.post1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4/tests/catalog_test.py` & `aepp-0.3.4.post1/tests/catalog_test.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4/tests/dataaccess_test.py` & `aepp-0.3.4.post1/tests/dataaccess_test.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4/tests/datasets_test.py` & `aepp-0.3.4.post1/tests/datasets_test.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4/tests/destinationinstanceservice_test.py` & `aepp-0.3.4.post1/tests/destinationinstanceservice_test.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4/tests/exportDatasetToDatalandingZone_test.py` & `aepp-0.3.4.post1/tests/exportDatasetToDatalandingZone_test.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4/tests/flowservice_test.py` & `aepp-0.3.4.post1/tests/flowservice_test.py`

 * *Files identical despite different names*

### Comparing `aepp-0.3.4/tests/schema_test.py` & `aepp-0.3.4.post1/tests/schema_test.py`

 * *Files identical despite different names*

