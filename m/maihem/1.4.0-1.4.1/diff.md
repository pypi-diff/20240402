# Comparing `tmp/maihem-1.4.0.tar.gz` & `tmp/maihem-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maihem-1.4.0.tar", last modified: Thu Mar  7 01:33:34 2024, max compression
+gzip compressed data, was "maihem-1.4.1.tar", last modified: Tue Apr  2 17:09:30 2024, max compression
```

## Comparing `maihem-1.4.0.tar` & `maihem-1.4.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 eduardocandela   (501) staff       (20)        0 2024-03-07 01:33:34.608538 maihem-1.4.0/
--rw-r--r--   0 eduardocandela   (501) staff       (20)     1063 2023-12-12 19:12:18.000000 maihem-1.4.0/LICENSE
--rw-r--r--   0 eduardocandela   (501) staff       (20)        0 2023-12-14 20:19:47.000000 maihem-1.4.0/MANIFEST.in
--rw-r--r--   0 eduardocandela   (501) staff       (20)     3530 2024-03-07 01:33:34.608458 maihem-1.4.0/PKG-INFO
--rw-r--r--   0 eduardocandela   (501) staff       (20)     1754 2024-03-07 01:27:56.000000 maihem-1.4.0/README.md
--rw-r--r--   0 eduardocandela   (501) staff       (20)      685 2024-03-05 01:55:36.000000 maihem-1.4.0/pyproject.toml
--rw-r--r--   0 eduardocandela   (501) staff       (20)       38 2024-03-07 01:33:34.608751 maihem-1.4.0/setup.cfg
-drwxr-xr-x   0 eduardocandela   (501) staff       (20)        0 2024-03-07 01:33:34.606403 maihem-1.4.0/src/
-drwxr-xr-x   0 eduardocandela   (501) staff       (20)        0 2024-03-07 01:33:34.607149 maihem-1.4.0/src/maihem/
--rw-r--r--   0 eduardocandela   (501) staff       (20)       82 2024-03-06 21:21:19.000000 maihem-1.4.0/src/maihem/__init__.py
--rw-r--r--   0 eduardocandela   (501) staff       (20)     8201 2024-03-07 00:52:03.000000 maihem-1.4.0/src/maihem/functions.py
-drwxr-xr-x   0 eduardocandela   (501) staff       (20)        0 2024-03-07 01:33:34.608234 maihem-1.4.0/src/maihem.egg-info/
--rw-r--r--   0 eduardocandela   (501) staff       (20)     3530 2024-03-07 01:33:34.000000 maihem-1.4.0/src/maihem.egg-info/PKG-INFO
--rw-r--r--   0 eduardocandela   (501) staff       (20)      270 2024-03-07 01:33:34.000000 maihem-1.4.0/src/maihem.egg-info/SOURCES.txt
--rw-r--r--   0 eduardocandela   (501) staff       (20)        1 2024-03-07 01:33:34.000000 maihem-1.4.0/src/maihem.egg-info/dependency_links.txt
--rw-r--r--   0 eduardocandela   (501) staff       (20)       16 2024-03-07 01:33:34.000000 maihem-1.4.0/src/maihem.egg-info/requires.txt
--rw-r--r--   0 eduardocandela   (501) staff       (20)        7 2024-03-07 01:33:34.000000 maihem-1.4.0/src/maihem.egg-info/top_level.txt
+drwxr-xr-x   0 eduardocandela   (501) staff       (20)        0 2024-04-02 17:09:30.194836 maihem-1.4.1/
+-rw-r--r--   0 eduardocandela   (501) staff       (20)     1063 2023-12-12 19:12:18.000000 maihem-1.4.1/LICENSE
+-rw-r--r--   0 eduardocandela   (501) staff       (20)        0 2023-12-14 20:19:47.000000 maihem-1.4.1/MANIFEST.in
+-rw-r--r--   0 eduardocandela   (501) staff       (20)     3530 2024-04-02 17:09:30.194755 maihem-1.4.1/PKG-INFO
+-rw-r--r--   0 eduardocandela   (501) staff       (20)     1754 2024-03-07 01:27:56.000000 maihem-1.4.1/README.md
+-rw-r--r--   0 eduardocandela   (501) staff       (20)      685 2024-04-02 17:07:07.000000 maihem-1.4.1/pyproject.toml
+-rw-r--r--   0 eduardocandela   (501) staff       (20)       38 2024-04-02 17:09:30.195041 maihem-1.4.1/setup.cfg
+drwxr-xr-x   0 eduardocandela   (501) staff       (20)        0 2024-04-02 17:09:30.192082 maihem-1.4.1/src/
+drwxr-xr-x   0 eduardocandela   (501) staff       (20)        0 2024-04-02 17:09:30.193182 maihem-1.4.1/src/maihem/
+-rw-r--r--   0 eduardocandela   (501) staff       (20)       82 2024-03-06 21:21:19.000000 maihem-1.4.1/src/maihem/__init__.py
+-rw-r--r--   0 eduardocandela   (501) staff       (20)     8747 2024-04-02 17:04:57.000000 maihem-1.4.1/src/maihem/functions.py
+drwxr-xr-x   0 eduardocandela   (501) staff       (20)        0 2024-04-02 17:09:30.194498 maihem-1.4.1/src/maihem.egg-info/
+-rw-r--r--   0 eduardocandela   (501) staff       (20)     3530 2024-04-02 17:09:30.000000 maihem-1.4.1/src/maihem.egg-info/PKG-INFO
+-rw-r--r--   0 eduardocandela   (501) staff       (20)      270 2024-04-02 17:09:30.000000 maihem-1.4.1/src/maihem.egg-info/SOURCES.txt
+-rw-r--r--   0 eduardocandela   (501) staff       (20)        1 2024-04-02 17:09:30.000000 maihem-1.4.1/src/maihem.egg-info/dependency_links.txt
+-rw-r--r--   0 eduardocandela   (501) staff       (20)       16 2024-04-02 17:09:30.000000 maihem-1.4.1/src/maihem.egg-info/requires.txt
+-rw-r--r--   0 eduardocandela   (501) staff       (20)        7 2024-04-02 17:09:30.000000 maihem-1.4.1/src/maihem.egg-info/top_level.txt
```

### Comparing `maihem-1.4.0/LICENSE` & `maihem-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `maihem-1.4.0/PKG-INFO` & `maihem-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maihem
-Version: 1.4.0
+Version: 1.4.1
 Summary: LLM evaluations and synthetic data generation with the MAIHEM models
 Author: MAIHEM
 License: MIT License
         
         Copyright (c) 2023 MAIHEM
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `maihem-1.4.0/README.md` & `maihem-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `maihem-1.4.0/pyproject.toml` & `maihem-1.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "maihem"
-version = "1.4.0"
+version = "1.4.1"
 description = "LLM evaluations and synthetic data generation with the MAIHEM models"
 readme = "README.md"
 authors = [{ name = "MAIHEM"}]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `maihem-1.4.0/src/maihem/functions.py` & `maihem-1.4.1/src/maihem/functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 import os
 import pandas as pd
 import requests
-import warnings
-import sys
-import threading
-import time
 from typing import List
 
 
 class APIKeyWarning(UserWarning):
     pass
 
 
@@ -45,20 +41,32 @@
         try:
             response = requests.post(self.URL_API + endpoint, headers=self.headers, json=payload)
         except requests.exceptions.HTTPError as err:
             raise SystemExit(err)
         
         if response.status_code == 401:
             raise ExceptionAPI("Invalid or missing API key")
-
-        if "info" in response.json():
-            print(response.json()['info'])
-            return response.json()
+        
+        try:
+            json_response = response.json()
+        except ValueError: # If no response received, try one more time
+            try:
+                response = requests.post(self.URL_API + endpoint, headers=self.headers, json=payload)
+            except requests.exceptions.HTTPError as err:
+                raise SystemExit(err)
+            try:
+                json_response = response.json()
+            except ValueError:
+                raise NoResponseData("No response was received")
+
+        if "info" in json_response:
+            print(json_response['info'])    
+            return json_response
         else:
-            raise ExceptionAPI(response.json()['detail'])
+            raise ExceptionAPI(json_response['detail'])
 
 
 def create_test(test_name: str, chatbot_role: str, industry: str, n: int, topic: str=None, language: str=None):
     """
     Create a test with a set of AI personas
 
     No return value
@@ -78,16 +86,17 @@
     language : str, optional
         Language of the chatbot, default is English
 
     Returns
     -------
     None
 
-    """
-    print("Creating test and AI personas...")
+    """    
+    print("Creating test and AI personas... It might take a few minutes")
+
     # Create API object
     api = CallAPI()
 
     payload = {
         "test_name": test_name,
         "chatbot_role": chatbot_role,
         "industry": industry,
@@ -95,15 +104,15 @@
         "topic": topic,
         "language": language
     }
     response = api._call_api(payload, "/create_test_simulated")
     print(response['response']) 
     
 
-def chat_with_persona(test_name: str, test_run_name: str, persona_id: int, message: str) -> str:
+def chat_with_persona(test_name: str, test_run_name: str, persona_id: int, message: str, num_turns_max=None) -> str:
     """
     Chat in a conversation with a single AI persona
 
     Returns the message from the AI persona
 
     Parameters
     ----------
@@ -123,15 +132,16 @@
     # Create API object
     api = CallAPI()
 
     payload = {
         "test_name": test_name,
         "test_run_name": test_run_name,
         "persona_id": persona_id,
-        "message": message
+        "message": message,
+        "num_turns_max": num_turns_max
     }
 
     response = api._call_api(payload, "/chat_with_persona")
     print(response['response'])
     return response['response']
```

### Comparing `maihem-1.4.0/src/maihem.egg-info/PKG-INFO` & `maihem-1.4.1/src/maihem.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maihem
-Version: 1.4.0
+Version: 1.4.1
 Summary: LLM evaluations and synthetic data generation with the MAIHEM models
 Author: MAIHEM
 License: MIT License
         
         Copyright (c) 2023 MAIHEM
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

