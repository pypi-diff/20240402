# Comparing `tmp/predicthq-3.2.0.tar.gz` & `tmp/predicthq-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "predicthq-3.2.0.tar", last modified: Tue Mar 19 01:06:59 2024, max compression
+gzip compressed data, was "predicthq-3.3.0.tar", last modified: Tue Apr  2 02:44:39 2024, max compression
```

## Comparing `predicthq-3.2.0.tar` & `predicthq-3.3.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 01:06:59.137119 predicthq-3.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-03-19 01:06:52.000000 predicthq-3.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-03-19 01:06:52.000000 predicthq-3.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9215 2024-03-19 01:06:59.137119 predicthq-3.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7961 2024-03-19 01:06:52.000000 predicthq-3.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 01:06:59.129119 predicthq-3.2.0/predicthq/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-19 01:06:52.000000 predicthq-3.2.0/predicthq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-03-19 01:06:52.000000 predicthq-3.2.0/predicthq/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-03-19 01:06:52.000000 predicthq-3.2.0/predicthq/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 01:06:59.133119 predicthq-3.2.0/predicthq/endpoints/
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-03-19 01:06:52.000000 predicthq-3.2.0/predicthq/endpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-03-19 01:06:52.000000 predicthq-3.2.0/predicthq/endpoints/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-03-19 01:06:52.000000 predicthq-3.2.0/predicthq/endpoints/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 01:06:59.133119 predicthq-3.2.0/predicthq/endpoints/oauth2/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-19 01:06:52.000000 predicthq-3.2.0/predicthq/endpoints/oauth2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-03-19 01:06:52.000000 predicthq-3.2.0/predicthq/endpoints/oauth2/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-03-19 01:06:52.000000 predicthq-3.2.0/predicthq/endpoints/oauth2/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-03-19 01:06:52.000000 predicthq-3.2.0/predicthq/endpoints/oauth2/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-03-19 01:06:52.000000 predicthq-3.2.0/predicthq/endpoints/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 01:06:59.133119 predicthq-3.2.0/predicthq/endpoints/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 01:06:52.000000 predicthq-3.2.0/predicthq/endpoints/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 01:06:59.133119 predicthq-3.2.0/predicthq/endpoints/v1/accounts/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-19 01:06:52.000000 predicthq-3.2.0/predicthq/endpoints/v1/accounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-03-19 01:06:52.000000 predicthq-3.2.0/predicthq/endpoints/v1/accounts/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-03-19 01:06:52.000000 predicthq-3.2.0/predicthq/endpoints/v1/accounts/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 01:06:59.133119 predicthq-3.2.0/predicthq/endpoints/v1/broadcasts/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-19 01:06:52.000000 predicthq-3.2.0/predicthq/endpoints/v1/broadcasts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-03-19 01:06:52.000000 predicthq-3.2.0/predicthq/endpoints/v1/broadcasts/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-03-19 01:06:52.000000 predicthq-3.2.0/predicthq/endpoints/v1/broadcasts/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 01:06:59.133119 predicthq-3.2.0/predicthq/endpoints/v1/events/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-19 01:06:52.000000 predicthq-3.2.0/predicthq/endpoints/v1/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-03-19 01:06:52.000000 predicthq-3.2.0/predicthq/endpoints/v1/events/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-03-19 01:06:52.000000 predicthq-3.2.0/predicthq/endpoints/v1/events/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 01:06:59.133119 predicthq-3.2.0/predicthq/endpoints/v1/features/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-19 01:06:52.000000 predicthq-3.2.0/predicthq/endpoints/v1/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-19 01:06:52.000000 predicthq-3.2.0/predicthq/endpoints/v1/features/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     9100 2024-03-19 01:06:52.000000 predicthq-3.2.0/predicthq/endpoints/v1/features/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 01:06:59.137119 predicthq-3.2.0/predicthq/endpoints/v1/places/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-19 01:06:52.000000 predicthq-3.2.0/predicthq/endpoints/v1/places/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-03-19 01:06:52.000000 predicthq-3.2.0/predicthq/endpoints/v1/places/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-03-19 01:06:52.000000 predicthq-3.2.0/predicthq/endpoints/v1/places/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 01:06:59.137119 predicthq-3.2.0/predicthq/endpoints/v1/radius/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-19 01:06:52.000000 predicthq-3.2.0/predicthq/endpoints/v1/radius/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-03-19 01:06:52.000000 predicthq-3.2.0/predicthq/endpoints/v1/radius/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-03-19 01:06:52.000000 predicthq-3.2.0/predicthq/endpoints/v1/radius/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-03-19 01:06:52.000000 predicthq-3.2.0/predicthq/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-19 01:06:52.000000 predicthq-3.2.0/predicthq/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 01:06:59.137119 predicthq-3.2.0/predicthq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9215 2024-03-19 01:06:59.000000 predicthq-3.2.0/predicthq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-03-19 01:06:59.000000 predicthq-3.2.0/predicthq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 01:06:59.000000 predicthq-3.2.0/predicthq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-19 01:06:59.000000 predicthq-3.2.0/predicthq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-19 01:06:59.000000 predicthq-3.2.0/predicthq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-19 01:06:59.137119 predicthq-3.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-03-19 01:06:52.000000 predicthq-3.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 01:06:59.137119 predicthq-3.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4667 2024-03-19 01:06:52.000000 predicthq-3.2.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-03-19 01:06:52.000000 predicthq-3.2.0/tests/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:44:39.444814 predicthq-3.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-02 02:44:33.000000 predicthq-3.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-02 02:44:33.000000 predicthq-3.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9215 2024-04-02 02:44:39.444814 predicthq-3.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7961 2024-04-02 02:44:33.000000 predicthq-3.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:44:39.440814 predicthq-3.3.0/predicthq/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-02 02:44:33.000000 predicthq-3.3.0/predicthq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-04-02 02:44:33.000000 predicthq-3.3.0/predicthq/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-02 02:44:33.000000 predicthq-3.3.0/predicthq/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:44:39.440814 predicthq-3.3.0/predicthq/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-02 02:44:33.000000 predicthq-3.3.0/predicthq/endpoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-02 02:44:33.000000 predicthq-3.3.0/predicthq/endpoints/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-04-02 02:44:33.000000 predicthq-3.3.0/predicthq/endpoints/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:44:39.440814 predicthq-3.3.0/predicthq/endpoints/oauth2/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-02 02:44:33.000000 predicthq-3.3.0/predicthq/endpoints/oauth2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-02 02:44:33.000000 predicthq-3.3.0/predicthq/endpoints/oauth2/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-02 02:44:33.000000 predicthq-3.3.0/predicthq/endpoints/oauth2/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-02 02:44:33.000000 predicthq-3.3.0/predicthq/endpoints/oauth2/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-02 02:44:33.000000 predicthq-3.3.0/predicthq/endpoints/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:44:39.440814 predicthq-3.3.0/predicthq/endpoints/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 02:44:33.000000 predicthq-3.3.0/predicthq/endpoints/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:44:39.440814 predicthq-3.3.0/predicthq/endpoints/v1/accounts/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-02 02:44:33.000000 predicthq-3.3.0/predicthq/endpoints/v1/accounts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-02 02:44:33.000000 predicthq-3.3.0/predicthq/endpoints/v1/accounts/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-02 02:44:33.000000 predicthq-3.3.0/predicthq/endpoints/v1/accounts/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:44:39.440814 predicthq-3.3.0/predicthq/endpoints/v1/broadcasts/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-02 02:44:33.000000 predicthq-3.3.0/predicthq/endpoints/v1/broadcasts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-02 02:44:33.000000 predicthq-3.3.0/predicthq/endpoints/v1/broadcasts/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-04-02 02:44:33.000000 predicthq-3.3.0/predicthq/endpoints/v1/broadcasts/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:44:39.440814 predicthq-3.3.0/predicthq/endpoints/v1/events/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-02 02:44:33.000000 predicthq-3.3.0/predicthq/endpoints/v1/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-02 02:44:33.000000 predicthq-3.3.0/predicthq/endpoints/v1/events/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-04-02 02:44:33.000000 predicthq-3.3.0/predicthq/endpoints/v1/events/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:44:39.444814 predicthq-3.3.0/predicthq/endpoints/v1/features/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-02 02:44:33.000000 predicthq-3.3.0/predicthq/endpoints/v1/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-02 02:44:33.000000 predicthq-3.3.0/predicthq/endpoints/v1/features/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9100 2024-04-02 02:44:33.000000 predicthq-3.3.0/predicthq/endpoints/v1/features/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:44:39.444814 predicthq-3.3.0/predicthq/endpoints/v1/places/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-02 02:44:33.000000 predicthq-3.3.0/predicthq/endpoints/v1/places/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-02 02:44:33.000000 predicthq-3.3.0/predicthq/endpoints/v1/places/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-02 02:44:33.000000 predicthq-3.3.0/predicthq/endpoints/v1/places/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:44:39.444814 predicthq-3.3.0/predicthq/endpoints/v1/radius/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-02 02:44:33.000000 predicthq-3.3.0/predicthq/endpoints/v1/radius/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-02 02:44:33.000000 predicthq-3.3.0/predicthq/endpoints/v1/radius/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-02 02:44:33.000000 predicthq-3.3.0/predicthq/endpoints/v1/radius/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-02 02:44:33.000000 predicthq-3.3.0/predicthq/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-02 02:44:33.000000 predicthq-3.3.0/predicthq/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:44:39.444814 predicthq-3.3.0/predicthq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9215 2024-04-02 02:44:39.000000 predicthq-3.3.0/predicthq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-02 02:44:39.000000 predicthq-3.3.0/predicthq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 02:44:39.000000 predicthq-3.3.0/predicthq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-02 02:44:39.000000 predicthq-3.3.0/predicthq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-02 02:44:39.000000 predicthq-3.3.0/predicthq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-02 02:44:39.444814 predicthq-3.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-02 02:44:33.000000 predicthq-3.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:44:39.444814 predicthq-3.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4667 2024-04-02 02:44:33.000000 predicthq-3.3.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-02 02:44:33.000000 predicthq-3.3.0/tests/test_config.py
```

### Comparing `predicthq-3.2.0/LICENSE` & `predicthq-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `predicthq-3.2.0/PKG-INFO` & `predicthq-3.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: predicthq
-Version: 3.2.0
+Version: 3.3.0
 Summary: PredictHQ Event Intelligence
 Home-page: https://github.com/predicthq/sdk-py
 Author: PredictHQ
 Author-email: developers@predicthq.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `predicthq-3.2.0/README.md` & `predicthq-3.3.0/README.md`

 * *Files identical despite different names*

### Comparing `predicthq-3.2.0/predicthq/client.py` & `predicthq-3.3.0/predicthq/client.py`

 * *Files identical despite different names*

### Comparing `predicthq-3.2.0/predicthq/config.py` & `predicthq-3.3.0/predicthq/config.py`

 * *Files identical despite different names*

### Comparing `predicthq-3.2.0/predicthq/endpoints/base.py` & `predicthq-3.3.0/predicthq/endpoints/base.py`

 * *Files identical despite different names*

### Comparing `predicthq-3.2.0/predicthq/endpoints/decorators.py` & `predicthq-3.3.0/predicthq/endpoints/decorators.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,77 +1,77 @@
 import functools
-from collections import defaultdict
 
 from pydantic import ValidationError as PydanticValidationError
 
-from predicthq.endpoints.schemas import ResultSet
 from predicthq.exceptions import ValidationError
 
 
-def _to_url_params(data, glue=".", separator=","):
+def _kwargs_to_key_list_mapping(kwargs, separator="__"):
     """
-    Converts data dictionary to url parameters
+    Converts kwargs to a nested dictionary mapping keys to lists of values
     """
-    params = {}
-    for key, value in data.items():
-        if isinstance(value, bool):
-            params[key] = 1 if value else 0
-        elif isinstance(value, list):
-            params[key] = separator.join(map(str, value))
-        elif isinstance(value, dict):
-            params.update(_flatten_dict(value, glue, separator, parent_key=key))
-        else:
-            params[key] = value
-    return params
+    data = {}
+    for key, value in kwargs.items():
+        keys = key.split(separator, 1)
+        if len(keys) > 1:
+            value = {keys[1]: value}
+        if isinstance(value, dict):
+            value = _kwargs_to_key_list_mapping(value)
 
+        data[keys[0]] = [] if not data.get(keys[0]) else data[keys[0]]
+        data[keys[0]].append(value)
+    return data
 
-def _flatten_dict(d, glue, separator, parent_key=""):
-    flat_dict = {}
-    for k, v in d.items():
-        if isinstance(v, dict):
-            flat_dict.update(_flatten_dict(v, glue, separator, f"{parent_key}{glue}{k}" if parent_key else k))
-            continue
-        if isinstance(v, list):
-            flat_dict.update({f"{parent_key}{glue}{k}" if parent_key else k: separator.join(map(str, v))})
-            continue
-        flat_dict.update({f"{parent_key}{glue}{k}" if parent_key else k: v})
-    return flat_dict
-
-
-def _assign_nested_key(parent_dict, keys, value):
-    current_key = keys[0]
-    if len(keys) > 1:
-        if current_key not in parent_dict:
-            parent_dict[current_key] = dict()
-        _assign_nested_key(parent_dict[current_key], keys[1:], value)
-    else:
-        parent_dict[current_key] = value        
 
+def _to_url_params(key_list_mapping, glue=".", separator=",", parent_key=""):
+    """
+    Converts key_list_mapping to url parameters
+    """
+    params = {}
+    for key, value in key_list_mapping.items():
+        current_key = f"{parent_key}{glue}{key}" if parent_key else key
+        for v in value:
+            if isinstance(v, dict):
+                params.update(_to_url_params(v, glue, separator, current_key))
+            elif isinstance(v, list):
+                params.update({current_key: separator.join(map(str, v))})
+            elif isinstance(v, bool):
+                params.update({current_key: 1 if v else 0})
+            else:
+                params.update({current_key: v})
+    return params
 
-def _process_kwargs(kwargs, separator="__"):
-    data = dict()
-    for key, value in kwargs.items():
-        if separator in key:
-            _assign_nested_key(data, key.split(separator), value)
-        else:
-            data[key] = value
-    return data
 
+def _to_json(key_list_mapping):
+    """
+    Converts key_list_mapping to json
+    """
+    json = {}
+    for key, value in key_list_mapping.items():
+        for v in value:
+            json[key] = dict() if not json.get(key) else json[key]
+            if isinstance(v, dict):
+                json[key].update(_to_json(v))
+            else:
+                json[key] = v
+    return json
 
 
 def accepts(query_string=True, role=None):
     def decorator(f):
         @functools.wraps(f)
         def wrapper(endpoint, *args, **kwargs):
-            data = _process_kwargs(kwargs)
+            key_list_mapping = _kwargs_to_key_list_mapping(kwargs)
             if hasattr(endpoint, "mutate_bool_to_default_for_type"):
-                endpoint.mutate_bool_to_default_for_type(data)
+                endpoint.mutate_bool_to_default_for_type(key_list_mapping)
 
             if query_string:
-                data = _to_url_params(data=data)
+                data = _to_url_params(key_list_mapping)
+            else:
+                data = _to_json(key_list_mapping)
 
             return f(endpoint, *args, **data)
 
         return wrapper
 
     return decorator
```

### Comparing `predicthq-3.2.0/predicthq/endpoints/oauth2/decorators.py` & `predicthq-3.3.0/predicthq/endpoints/oauth2/decorators.py`

 * *Files identical despite different names*

### Comparing `predicthq-3.2.0/predicthq/endpoints/oauth2/endpoint.py` & `predicthq-3.3.0/predicthq/endpoints/oauth2/endpoint.py`

 * *Files identical despite different names*

### Comparing `predicthq-3.2.0/predicthq/endpoints/oauth2/schemas.py` & `predicthq-3.3.0/predicthq/endpoints/oauth2/schemas.py`

 * *Files identical despite different names*

### Comparing `predicthq-3.2.0/predicthq/endpoints/schemas.py` & `predicthq-3.3.0/predicthq/endpoints/schemas.py`

 * *Files identical despite different names*

### Comparing `predicthq-3.2.0/predicthq/endpoints/v1/broadcasts/schemas.py` & `predicthq-3.3.0/predicthq/endpoints/v1/broadcasts/schemas.py`

 * *Files identical despite different names*

### Comparing `predicthq-3.2.0/predicthq/endpoints/v1/events/endpoint.py` & `predicthq-3.3.0/predicthq/endpoints/v1/events/endpoint.py`

 * *Files identical despite different names*

### Comparing `predicthq-3.2.0/predicthq/endpoints/v1/events/schemas.py` & `predicthq-3.3.0/predicthq/endpoints/v1/events/schemas.py`

 * *Files identical despite different names*

### Comparing `predicthq-3.2.0/predicthq/endpoints/v1/features/endpoint.py` & `predicthq-3.3.0/predicthq/endpoints/v1/features/endpoint.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 from predicthq.endpoints.base import UserBaseEndpoint
 from predicthq.endpoints.decorators import accepts, returns
 from .schemas import FeatureResultSet
 
 
 class FeaturesEndpoint(UserBaseEndpoint):
 
-    BASE_FEATURE_CRITERIA = {"stats": ["sum", "count"], "phq_rank": None}
+    BASE_FEATURE_CRITERIA = {"stats": [["sum", "count"]], "phq_rank": [None]}
     FIELDS_TO_MUTATE = frozenset([
         "phq_attendance_",
         "phq_viewership_sports",
         "phq_impact_severe_weather_",
         "phq_spend_"
     ])
 
     @classmethod
     def mutate_bool_to_default_for_type(cls, user_request_spec):
         for key, val in user_request_spec.items():
-            if any(key.startswith(x) for x in cls.FIELDS_TO_MUTATE) and isinstance(val, bool):
-                user_request_spec[key] = cls.BASE_FEATURE_CRITERIA
+            if any(key.startswith(x) for x in cls.FIELDS_TO_MUTATE):
+                user_request_spec[key] = [cls.BASE_FEATURE_CRITERIA if isinstance(v, bool) else v for v in val]
 
     @accepts(query_string=False)
     @returns(FeatureResultSet)
     def obtain_features(self, **request):
         verify_ssl = request.pop("config", {}).get("verify_ssl", True)
         return self.client.post(
             self.build_url("v1", "features"),
```

### Comparing `predicthq-3.2.0/predicthq/endpoints/v1/features/schemas.py` & `predicthq-3.3.0/predicthq/endpoints/v1/features/schemas.py`

 * *Files identical despite different names*

### Comparing `predicthq-3.2.0/predicthq.egg-info/PKG-INFO` & `predicthq-3.3.0/predicthq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: predicthq
-Version: 3.2.0
+Version: 3.3.0
 Summary: PredictHQ Event Intelligence
 Home-page: https://github.com/predicthq/sdk-py
 Author: PredictHQ
 Author-email: developers@predicthq.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `predicthq-3.2.0/predicthq.egg-info/SOURCES.txt` & `predicthq-3.3.0/predicthq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `predicthq-3.2.0/setup.py` & `predicthq-3.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `predicthq-3.2.0/tests/test_client.py` & `predicthq-3.3.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `predicthq-3.2.0/tests/test_config.py` & `predicthq-3.3.0/tests/test_config.py`

 * *Files identical despite different names*

