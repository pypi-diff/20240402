# Comparing `tmp/drf-sse-1.0.0.tar.gz` & `tmp/drf-sse-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf-sse-1.0.0.tar", last modified: Tue Apr  2 03:11:09 2024, max compression
+gzip compressed data, was "drf-sse-1.0.1.tar", last modified: Tue Apr  2 03:12:38 2024, max compression
```

## Comparing `drf-sse-1.0.0.tar` & `drf-sse-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 suqingdong  (1000) disease   (8039)        0 2024-04-02 03:11:09.275185 drf-sse-1.0.0/
--rw-r--r--   0 suqingdong  (1000) disease   (8039)       54 2024-04-02 02:48:45.000000 drf-sse-1.0.0/MANIFEST.in
--rw-r--r--   0 suqingdong  (1000) disease   (8039)     4359 2024-04-02 03:11:09.267794 drf-sse-1.0.0/PKG-INFO
--rw-r--r--   0 suqingdong  (1000) disease   (8039)     2588 2024-04-02 03:08:52.000000 drf-sse-1.0.0/README.md
-drwxr-xr-x   0 suqingdong  (1000) disease   (8039)        0 2024-04-02 03:11:09.047885 drf-sse-1.0.0/drf_sse/
--rw-r--r--   0 suqingdong  (1000) disease   (8039)      288 2024-04-02 02:12:40.000000 drf-sse-1.0.0/drf_sse/__init__.py
--rw-r--r--   0 suqingdong  (1000) disease   (8039)      241 2024-04-02 02:12:23.000000 drf-sse-1.0.0/drf_sse/mixins.py
--rw-r--r--   0 suqingdong  (1000) disease   (8039)      294 2024-04-01 08:39:39.000000 drf-sse-1.0.0/drf_sse/renderers.py
--rw-r--r--   0 suqingdong  (1000) disease   (8039)      294 2024-04-01 08:39:39.000000 drf-sse-1.0.0/drf_sse/renders.py
--rw-r--r--   0 suqingdong  (1000) disease   (8039)     1141 2024-04-01 10:23:44.000000 drf-sse-1.0.0/drf_sse/responses.py
--rw-r--r--   0 suqingdong  (1000) disease   (8039)      247 2024-04-02 02:49:22.000000 drf-sse-1.0.0/drf_sse/version.json
-drwxr-xr-x   0 suqingdong  (1000) disease   (8039)        0 2024-04-02 03:11:09.233816 drf-sse-1.0.0/drf_sse.egg-info/
--rw-r--r--   0 suqingdong  (1000) disease   (8039)     4359 2024-04-02 03:11:08.000000 drf-sse-1.0.0/drf_sse.egg-info/PKG-INFO
--rw-r--r--   0 suqingdong  (1000) disease   (8039)      321 2024-04-02 03:11:08.000000 drf-sse-1.0.0/drf_sse.egg-info/SOURCES.txt
--rw-r--r--   0 suqingdong  (1000) disease   (8039)        1 2024-04-02 03:11:08.000000 drf-sse-1.0.0/drf_sse.egg-info/dependency_links.txt
--rw-r--r--   0 suqingdong  (1000) disease   (8039)       20 2024-04-02 03:11:08.000000 drf-sse-1.0.0/drf_sse.egg-info/requires.txt
--rw-r--r--   0 suqingdong  (1000) disease   (8039)        8 2024-04-02 03:11:08.000000 drf-sse-1.0.0/drf_sse.egg-info/top_level.txt
--rw-r--r--   0 suqingdong  (1000) disease   (8039)       20 2024-04-02 02:56:59.000000 drf-sse-1.0.0/requirements.txt
--rw-r--r--   0 suqingdong  (1000) disease   (8039)       38 2024-04-02 03:11:09.281336 drf-sse-1.0.0/setup.cfg
--rw-r--r--   0 suqingdong  (1000) disease   (8039)     1310 2024-04-02 02:49:10.000000 drf-sse-1.0.0/setup.py
+drwxr-xr-x   0 suqingdong  (1000) disease   (8039)        0 2024-04-02 03:12:38.111961 drf-sse-1.0.1/
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)       54 2024-04-02 02:48:45.000000 drf-sse-1.0.1/MANIFEST.in
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)     4353 2024-04-02 03:12:38.105282 drf-sse-1.0.1/PKG-INFO
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)     2588 2024-04-02 03:08:52.000000 drf-sse-1.0.1/README.md
+drwxr-xr-x   0 suqingdong  (1000) disease   (8039)        0 2024-04-02 03:12:37.935681 drf-sse-1.0.1/drf_sse/
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)      288 2024-04-02 02:12:40.000000 drf-sse-1.0.1/drf_sse/__init__.py
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)      241 2024-04-02 02:12:23.000000 drf-sse-1.0.1/drf_sse/mixins.py
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)      294 2024-04-01 08:39:39.000000 drf-sse-1.0.1/drf_sse/renderers.py
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)      294 2024-04-01 08:39:39.000000 drf-sse-1.0.1/drf_sse/renders.py
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)     1141 2024-04-01 10:23:44.000000 drf-sse-1.0.1/drf_sse/responses.py
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)      241 2024-04-02 03:12:23.000000 drf-sse-1.0.1/drf_sse/version.json
+drwxr-xr-x   0 suqingdong  (1000) disease   (8039)        0 2024-04-02 03:12:38.077619 drf-sse-1.0.1/drf_sse.egg-info/
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)     4353 2024-04-02 03:12:37.000000 drf-sse-1.0.1/drf_sse.egg-info/PKG-INFO
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)      321 2024-04-02 03:12:37.000000 drf-sse-1.0.1/drf_sse.egg-info/SOURCES.txt
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)        1 2024-04-02 03:12:37.000000 drf-sse-1.0.1/drf_sse.egg-info/dependency_links.txt
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)       20 2024-04-02 03:12:37.000000 drf-sse-1.0.1/drf_sse.egg-info/requires.txt
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)        8 2024-04-02 03:12:37.000000 drf-sse-1.0.1/drf_sse.egg-info/top_level.txt
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)       20 2024-04-02 02:56:59.000000 drf-sse-1.0.1/requirements.txt
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)       38 2024-04-02 03:12:38.116448 drf-sse-1.0.1/setup.cfg
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)     1310 2024-04-02 02:49:10.000000 drf-sse-1.0.1/setup.py
```

### Comparing `drf-sse-1.0.0/PKG-INFO` & `drf-sse-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: drf-sse
-Version: 1.0.0
+Version: 1.0.1
 Summary: SSE(Server-Sent Events) for DjangoRestFramework
-Home-page: https://github.com/suqingdong/drf_sse_mixin
+Home-page: https://github.com/suqingdong/drf_sse
 Author: suqingdong
 Author-email: suqingdong1114@gmail.com
 License: MIT License
 Description: # SSE(Server-Sent Events) for DjangoRestFramework
         
         ## Installation
```

### Comparing `drf-sse-1.0.0/README.md` & `drf-sse-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `drf-sse-1.0.0/drf_sse/responses.py` & `drf-sse-1.0.1/drf_sse/responses.py`

 * *Files identical despite different names*

### Comparing `drf-sse-1.0.0/drf_sse.egg-info/PKG-INFO` & `drf-sse-1.0.1/drf_sse.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: drf-sse
-Version: 1.0.0
+Version: 1.0.1
 Summary: SSE(Server-Sent Events) for DjangoRestFramework
-Home-page: https://github.com/suqingdong/drf_sse_mixin
+Home-page: https://github.com/suqingdong/drf_sse
 Author: suqingdong
 Author-email: suqingdong1114@gmail.com
 License: MIT License
 Description: # SSE(Server-Sent Events) for DjangoRestFramework
         
         ## Installation
```

### Comparing `drf-sse-1.0.0/setup.py` & `drf-sse-1.0.1/setup.py`

 * *Files identical despite different names*

