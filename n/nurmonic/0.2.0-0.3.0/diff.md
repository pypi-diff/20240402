# Comparing `tmp/nurmonic-0.2.0.tar.gz` & `tmp/nurmonic-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nurmonic-0.2.0.tar", last modified: Thu Mar 21 14:32:13 2024, max compression
+gzip compressed data, was "nurmonic-0.3.0.tar", last modified: Tue Apr  2 03:18:46 2024, max compression
```

## Comparing `nurmonic-0.2.0.tar` & `nurmonic-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-21 14:32:13.330695 nurmonic-0.2.0/
--rw-r--r--   0 runner    (1000) runner    (1000)     1772 2024-03-21 14:32:13.330695 nurmonic-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)     1519 2024-03-21 13:41:27.000000 nurmonic-0.2.0/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-21 14:32:13.326695 nurmonic-0.2.0/nurmonic/
--rw-r--r--   0 runner    (1000) runner    (1000)       53 2024-03-21 13:41:52.000000 nurmonic-0.2.0/nurmonic/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      856 2024-03-21 14:31:27.000000 nurmonic-0.2.0/nurmonic/nurmonic.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-03-21 14:32:13.330695 nurmonic-0.2.0/nurmonic.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     1772 2024-03-21 14:32:13.000000 nurmonic-0.2.0/nurmonic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      234 2024-03-21 14:32:13.000000 nurmonic-0.2.0/nurmonic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-03-21 14:32:13.000000 nurmonic-0.2.0/nurmonic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       17 2024-03-21 14:32:13.000000 nurmonic-0.2.0/nurmonic.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        9 2024-03-21 14:32:13.000000 nurmonic-0.2.0/nurmonic.egg-info/top_level.txt
--rw-------   0 runner    (1000) runner    (1000)      544 2024-02-27 23:10:40.000000 nurmonic-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-03-21 14:32:13.330695 nurmonic-0.2.0/setup.cfg
--rw-------   0 runner    (1000) runner    (1000)      430 2024-03-21 14:31:45.000000 nurmonic-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-02 03:18:46.102122 nurmonic-0.3.0/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1772 2024-04-02 03:18:46.102122 nurmonic-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     1519 2024-03-21 13:41:27.000000 nurmonic-0.3.0/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-02 03:18:46.098122 nurmonic-0.3.0/nurmonic/
+-rw-r--r--   0 runner    (1000) runner    (1000)       53 2024-03-21 13:41:52.000000 nurmonic-0.3.0/nurmonic/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1114 2024-04-02 03:17:11.000000 nurmonic-0.3.0/nurmonic/nurmonic.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-02 03:18:46.102122 nurmonic-0.3.0/nurmonic.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1772 2024-04-02 03:18:45.000000 nurmonic-0.3.0/nurmonic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      234 2024-04-02 03:18:45.000000 nurmonic-0.3.0/nurmonic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-04-02 03:18:45.000000 nurmonic-0.3.0/nurmonic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       17 2024-04-02 03:18:45.000000 nurmonic-0.3.0/nurmonic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        9 2024-04-02 03:18:45.000000 nurmonic-0.3.0/nurmonic.egg-info/top_level.txt
+-rw-------   0 runner    (1000) runner    (1000)      544 2024-02-27 23:10:40.000000 nurmonic-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-04-02 03:18:46.102122 nurmonic-0.3.0/setup.cfg
+-rw-------   0 runner    (1000) runner    (1000)      430 2024-04-02 03:18:38.000000 nurmonic-0.3.0/setup.py
```

### Comparing `nurmonic-0.2.0/PKG-INFO` & `nurmonic-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nurmonic
-Version: 0.2.0
+Version: 0.3.0
 Summary: A Python client for the Nurmonic API.
 Home-page: https://nurmonic.xyz
 Author: Reksely
 Author-email: reksely@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: requests>=2.25.1
```

### Comparing `nurmonic-0.2.0/README.md` & `nurmonic-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `nurmonic-0.2.0/nurmonic/nurmonic.py` & `nurmonic-0.3.0/nurmonic/nurmonic.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,33 @@
-# nurmonic.py
-
 import os
 import requests
 
 class Nurmonic:
     def __init__(self, api_key=None):
         self.api_key = api_key if api_key is not None else os.environ.get('NURMONIC_KEY')
         self.base_url = 'https://nurmonic.xyz/chat/completions'
 
-    def create_completion(self, messages, model):
+    def create_completion(self, messages, model, character=None):
         headers = {'Authorization': self.api_key}
-        response = requests.post(self.base_url, json={'model': model, 'messages': messages}, headers=headers)
+
+        if model == 'nurmo-2' and character is None:
+            raise ValueError("When using model 'nurmo-2', a character must be provided.")
+
+        data = {'model': model, 'messages': messages}
+
+        if model == 'nurmo-2':
+            data['character'] = character
+
+        response = requests.post(self.base_url, json=data, headers=headers)
         response_text = response.text
+
         try:
-          response_data = response.json()
-          if 'error' in response_data:
-              if response_data['error'] == "Unknown model":
-                  raise Exception(f"Unknown model named {model}")
-              else:
-                  raise Exception(response_data['error'])
+            response_data = response.json()
+            if 'error' in response_data:
+                if response_data['error'] == "Unknown model":
+                    raise Exception(f"Unknown model named {model}")
+                else:
+                    raise Exception(response_data['error'])
         except:
-          pass
-        return response_text
+            pass
+
+        return response_text
```

### Comparing `nurmonic-0.2.0/nurmonic.egg-info/PKG-INFO` & `nurmonic-0.3.0/nurmonic.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nurmonic
-Version: 0.2.0
+Version: 0.3.0
 Summary: A Python client for the Nurmonic API.
 Home-page: https://nurmonic.xyz
 Author: Reksely
 Author-email: reksely@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: requests>=2.25.1
```

### Comparing `nurmonic-0.2.0/pyproject.toml` & `nurmonic-0.3.0/pyproject.toml`

 * *Files identical despite different names*

