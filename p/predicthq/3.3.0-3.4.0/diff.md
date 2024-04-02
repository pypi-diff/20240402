# Comparing `tmp/predicthq-3.3.0.tar.gz` & `tmp/predicthq-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "predicthq-3.3.0.tar", last modified: Tue Apr  2 02:44:39 2024, max compression
+gzip compressed data, was "predicthq-3.4.0.tar", last modified: Tue Apr  2 20:17:24 2024, max compression
```

## Comparing `predicthq-3.3.0.tar` & `predicthq-3.4.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:44:39.444814 predicthq-3.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-02 02:44:33.000000 predicthq-3.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-02 02:44:33.000000 predicthq-3.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9215 2024-04-02 02:44:39.444814 predicthq-3.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7961 2024-04-02 02:44:33.000000 predicthq-3.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:44:39.440814 predicthq-3.3.0/predicthq/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-02 02:44:33.000000 predicthq-3.3.0/predicthq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-04-02 02:44:33.000000 predicthq-3.3.0/predicthq/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-02 02:44:33.000000 predicthq-3.3.0/predicthq/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:44:39.440814 predicthq-3.3.0/predicthq/endpoints/
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-02 02:44:33.000000 predicthq-3.3.0/predicthq/endpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-02 02:44:33.000000 predicthq-3.3.0/predicthq/endpoints/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-04-02 02:44:33.000000 predicthq-3.3.0/predicthq/endpoints/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:44:39.440814 predicthq-3.3.0/predicthq/endpoints/oauth2/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-02 02:44:33.000000 predicthq-3.3.0/predicthq/endpoints/oauth2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-02 02:44:33.000000 predicthq-3.3.0/predicthq/endpoints/oauth2/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-02 02:44:33.000000 predicthq-3.3.0/predicthq/endpoints/oauth2/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-02 02:44:33.000000 predicthq-3.3.0/predicthq/endpoints/oauth2/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-02 02:44:33.000000 predicthq-3.3.0/predicthq/endpoints/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:44:39.440814 predicthq-3.3.0/predicthq/endpoints/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 02:44:33.000000 predicthq-3.3.0/predicthq/endpoints/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:44:39.440814 predicthq-3.3.0/predicthq/endpoints/v1/accounts/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-02 02:44:33.000000 predicthq-3.3.0/predicthq/endpoints/v1/accounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-02 02:44:33.000000 predicthq-3.3.0/predicthq/endpoints/v1/accounts/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-02 02:44:33.000000 predicthq-3.3.0/predicthq/endpoints/v1/accounts/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:44:39.440814 predicthq-3.3.0/predicthq/endpoints/v1/broadcasts/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-02 02:44:33.000000 predicthq-3.3.0/predicthq/endpoints/v1/broadcasts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-02 02:44:33.000000 predicthq-3.3.0/predicthq/endpoints/v1/broadcasts/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-04-02 02:44:33.000000 predicthq-3.3.0/predicthq/endpoints/v1/broadcasts/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:44:39.440814 predicthq-3.3.0/predicthq/endpoints/v1/events/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-02 02:44:33.000000 predicthq-3.3.0/predicthq/endpoints/v1/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-02 02:44:33.000000 predicthq-3.3.0/predicthq/endpoints/v1/events/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-04-02 02:44:33.000000 predicthq-3.3.0/predicthq/endpoints/v1/events/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:44:39.444814 predicthq-3.3.0/predicthq/endpoints/v1/features/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-02 02:44:33.000000 predicthq-3.3.0/predicthq/endpoints/v1/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-02 02:44:33.000000 predicthq-3.3.0/predicthq/endpoints/v1/features/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     9100 2024-04-02 02:44:33.000000 predicthq-3.3.0/predicthq/endpoints/v1/features/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:44:39.444814 predicthq-3.3.0/predicthq/endpoints/v1/places/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-02 02:44:33.000000 predicthq-3.3.0/predicthq/endpoints/v1/places/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-02 02:44:33.000000 predicthq-3.3.0/predicthq/endpoints/v1/places/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-02 02:44:33.000000 predicthq-3.3.0/predicthq/endpoints/v1/places/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:44:39.444814 predicthq-3.3.0/predicthq/endpoints/v1/radius/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-02 02:44:33.000000 predicthq-3.3.0/predicthq/endpoints/v1/radius/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-02 02:44:33.000000 predicthq-3.3.0/predicthq/endpoints/v1/radius/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-02 02:44:33.000000 predicthq-3.3.0/predicthq/endpoints/v1/radius/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-02 02:44:33.000000 predicthq-3.3.0/predicthq/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-02 02:44:33.000000 predicthq-3.3.0/predicthq/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:44:39.444814 predicthq-3.3.0/predicthq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9215 2024-04-02 02:44:39.000000 predicthq-3.3.0/predicthq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-02 02:44:39.000000 predicthq-3.3.0/predicthq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 02:44:39.000000 predicthq-3.3.0/predicthq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-02 02:44:39.000000 predicthq-3.3.0/predicthq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-02 02:44:39.000000 predicthq-3.3.0/predicthq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-02 02:44:39.444814 predicthq-3.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-02 02:44:33.000000 predicthq-3.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:44:39.444814 predicthq-3.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4667 2024-04-02 02:44:33.000000 predicthq-3.3.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-02 02:44:33.000000 predicthq-3.3.0/tests/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:17:24.632434 predicthq-3.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-02 20:17:15.000000 predicthq-3.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-02 20:17:15.000000 predicthq-3.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9215 2024-04-02 20:17:24.632434 predicthq-3.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7961 2024-04-02 20:17:15.000000 predicthq-3.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:17:24.628434 predicthq-3.4.0/predicthq/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-02 20:17:15.000000 predicthq-3.4.0/predicthq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-04-02 20:17:15.000000 predicthq-3.4.0/predicthq/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-02 20:17:15.000000 predicthq-3.4.0/predicthq/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:17:24.628434 predicthq-3.4.0/predicthq/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-02 20:17:15.000000 predicthq-3.4.0/predicthq/endpoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-02 20:17:15.000000 predicthq-3.4.0/predicthq/endpoints/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-04-02 20:17:15.000000 predicthq-3.4.0/predicthq/endpoints/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:17:24.628434 predicthq-3.4.0/predicthq/endpoints/oauth2/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-02 20:17:15.000000 predicthq-3.4.0/predicthq/endpoints/oauth2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-02 20:17:15.000000 predicthq-3.4.0/predicthq/endpoints/oauth2/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-02 20:17:15.000000 predicthq-3.4.0/predicthq/endpoints/oauth2/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-02 20:17:15.000000 predicthq-3.4.0/predicthq/endpoints/oauth2/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-02 20:17:15.000000 predicthq-3.4.0/predicthq/endpoints/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:17:24.628434 predicthq-3.4.0/predicthq/endpoints/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 20:17:15.000000 predicthq-3.4.0/predicthq/endpoints/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:17:24.628434 predicthq-3.4.0/predicthq/endpoints/v1/accounts/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-02 20:17:15.000000 predicthq-3.4.0/predicthq/endpoints/v1/accounts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-02 20:17:15.000000 predicthq-3.4.0/predicthq/endpoints/v1/accounts/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-02 20:17:15.000000 predicthq-3.4.0/predicthq/endpoints/v1/accounts/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:17:24.628434 predicthq-3.4.0/predicthq/endpoints/v1/broadcasts/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-02 20:17:15.000000 predicthq-3.4.0/predicthq/endpoints/v1/broadcasts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-02 20:17:15.000000 predicthq-3.4.0/predicthq/endpoints/v1/broadcasts/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-04-02 20:17:15.000000 predicthq-3.4.0/predicthq/endpoints/v1/broadcasts/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:17:24.632434 predicthq-3.4.0/predicthq/endpoints/v1/events/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-02 20:17:15.000000 predicthq-3.4.0/predicthq/endpoints/v1/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-02 20:17:15.000000 predicthq-3.4.0/predicthq/endpoints/v1/events/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3326 2024-04-02 20:17:15.000000 predicthq-3.4.0/predicthq/endpoints/v1/events/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:17:24.632434 predicthq-3.4.0/predicthq/endpoints/v1/features/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-02 20:17:15.000000 predicthq-3.4.0/predicthq/endpoints/v1/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-02 20:17:15.000000 predicthq-3.4.0/predicthq/endpoints/v1/features/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9100 2024-04-02 20:17:15.000000 predicthq-3.4.0/predicthq/endpoints/v1/features/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:17:24.632434 predicthq-3.4.0/predicthq/endpoints/v1/places/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-02 20:17:15.000000 predicthq-3.4.0/predicthq/endpoints/v1/places/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-02 20:17:15.000000 predicthq-3.4.0/predicthq/endpoints/v1/places/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-02 20:17:15.000000 predicthq-3.4.0/predicthq/endpoints/v1/places/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:17:24.632434 predicthq-3.4.0/predicthq/endpoints/v1/radius/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-02 20:17:15.000000 predicthq-3.4.0/predicthq/endpoints/v1/radius/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-02 20:17:15.000000 predicthq-3.4.0/predicthq/endpoints/v1/radius/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-02 20:17:15.000000 predicthq-3.4.0/predicthq/endpoints/v1/radius/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-02 20:17:15.000000 predicthq-3.4.0/predicthq/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-02 20:17:15.000000 predicthq-3.4.0/predicthq/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:17:24.632434 predicthq-3.4.0/predicthq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9215 2024-04-02 20:17:24.000000 predicthq-3.4.0/predicthq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-02 20:17:24.000000 predicthq-3.4.0/predicthq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 20:17:24.000000 predicthq-3.4.0/predicthq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-02 20:17:24.000000 predicthq-3.4.0/predicthq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-02 20:17:24.000000 predicthq-3.4.0/predicthq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-02 20:17:24.632434 predicthq-3.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-02 20:17:15.000000 predicthq-3.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:17:24.632434 predicthq-3.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4667 2024-04-02 20:17:15.000000 predicthq-3.4.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-02 20:17:15.000000 predicthq-3.4.0/tests/test_config.py
```

### Comparing `predicthq-3.3.0/LICENSE` & `predicthq-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `predicthq-3.3.0/PKG-INFO` & `predicthq-3.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: predicthq
-Version: 3.3.0
+Version: 3.4.0
 Summary: PredictHQ Event Intelligence
 Home-page: https://github.com/predicthq/sdk-py
 Author: PredictHQ
 Author-email: developers@predicthq.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `predicthq-3.3.0/README.md` & `predicthq-3.4.0/README.md`

 * *Files identical despite different names*

### Comparing `predicthq-3.3.0/predicthq/client.py` & `predicthq-3.4.0/predicthq/client.py`

 * *Files identical despite different names*

### Comparing `predicthq-3.3.0/predicthq/config.py` & `predicthq-3.4.0/predicthq/config.py`

 * *Files identical despite different names*

### Comparing `predicthq-3.3.0/predicthq/endpoints/base.py` & `predicthq-3.4.0/predicthq/endpoints/base.py`

 * *Files identical despite different names*

### Comparing `predicthq-3.3.0/predicthq/endpoints/decorators.py` & `predicthq-3.4.0/predicthq/endpoints/decorators.py`

 * *Files identical despite different names*

### Comparing `predicthq-3.3.0/predicthq/endpoints/oauth2/decorators.py` & `predicthq-3.4.0/predicthq/endpoints/oauth2/decorators.py`

 * *Files identical despite different names*

### Comparing `predicthq-3.3.0/predicthq/endpoints/oauth2/endpoint.py` & `predicthq-3.4.0/predicthq/endpoints/oauth2/endpoint.py`

 * *Files identical despite different names*

### Comparing `predicthq-3.3.0/predicthq/endpoints/oauth2/schemas.py` & `predicthq-3.4.0/predicthq/endpoints/oauth2/schemas.py`

 * *Files identical despite different names*

### Comparing `predicthq-3.3.0/predicthq/endpoints/schemas.py` & `predicthq-3.4.0/predicthq/endpoints/schemas.py`

 * *Files identical despite different names*

### Comparing `predicthq-3.3.0/predicthq/endpoints/v1/broadcasts/schemas.py` & `predicthq-3.4.0/predicthq/endpoints/v1/broadcasts/schemas.py`

 * *Files identical despite different names*

### Comparing `predicthq-3.3.0/predicthq/endpoints/v1/events/endpoint.py` & `predicthq-3.4.0/predicthq/endpoints/v1/events/endpoint.py`

 * *Files identical despite different names*

### Comparing `predicthq-3.3.0/predicthq/endpoints/v1/events/schemas.py` & `predicthq-3.4.0/predicthq/endpoints/v1/events/schemas.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,15 +108,15 @@
 class EventResultSet(ResultSet):
     overflow: Optional[bool] = False
     results: List[Optional[Event]]
 
 
 class CountResultSet(BaseModel):
     count: int
-    top_rank: float
+    top_rank: Optional[float]
     rank_levels: dict
     categories: dict
     labels: dict
 
 
 class CalendarDay(BaseModel):
     date: date
```

### Comparing `predicthq-3.3.0/predicthq/endpoints/v1/features/endpoint.py` & `predicthq-3.4.0/predicthq/endpoints/v1/features/endpoint.py`

 * *Files identical despite different names*

### Comparing `predicthq-3.3.0/predicthq/endpoints/v1/features/schemas.py` & `predicthq-3.4.0/predicthq/endpoints/v1/features/schemas.py`

 * *Files identical despite different names*

### Comparing `predicthq-3.3.0/predicthq.egg-info/PKG-INFO` & `predicthq-3.4.0/predicthq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: predicthq
-Version: 3.3.0
+Version: 3.4.0
 Summary: PredictHQ Event Intelligence
 Home-page: https://github.com/predicthq/sdk-py
 Author: PredictHQ
 Author-email: developers@predicthq.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `predicthq-3.3.0/predicthq.egg-info/SOURCES.txt` & `predicthq-3.4.0/predicthq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `predicthq-3.3.0/setup.py` & `predicthq-3.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `predicthq-3.3.0/tests/test_client.py` & `predicthq-3.4.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `predicthq-3.3.0/tests/test_config.py` & `predicthq-3.4.0/tests/test_config.py`

 * *Files identical despite different names*

