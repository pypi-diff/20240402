# Comparing `tmp/backpack_exchange_sdk-0.2.5.tar.gz` & `tmp/backpack_exchange_sdk-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backpack_exchange_sdk-0.2.5.tar", last modified: Tue Apr  2 16:04:12 2024, max compression
+gzip compressed data, was "backpack_exchange_sdk-0.2.6.tar", last modified: Tue Apr  2 16:08:07 2024, max compression
```

## Comparing `backpack_exchange_sdk-0.2.5.tar` & `backpack_exchange_sdk-0.2.6.tar`

### file list

```diff
@@ -1,18 +1,22 @@
-drwxr-xr-x   0 solomeowl   (501) staff       (20)        0 2024-04-02 16:04:12.726956 backpack_exchange_sdk-0.2.5/
--rw-r--r--   0 solomeowl   (501) staff       (20)     1066 2024-03-08 15:43:17.000000 backpack_exchange_sdk-0.2.5/LICENSE
--rw-r--r--   0 solomeowl   (501) staff       (20)     2477 2024-04-02 16:04:12.726695 backpack_exchange_sdk-0.2.5/PKG-INFO
--rw-r--r--   0 solomeowl   (501) staff       (20)     2119 2024-04-02 15:44:43.000000 backpack_exchange_sdk-0.2.5/README.md
-drwxr-xr-x   0 solomeowl   (501) staff       (20)        0 2024-04-02 16:04:12.723180 backpack_exchange_sdk-0.2.5/backpack_exchange_sdk/
--rw-r--r--   0 solomeowl   (501) staff       (20)        0 2024-03-09 08:21:03.000000 backpack_exchange_sdk-0.2.5/backpack_exchange_sdk/__init__.py
--rw-r--r--   0 solomeowl   (501) staff       (20)     9416 2024-04-02 16:03:57.000000 backpack_exchange_sdk-0.2.5/backpack_exchange_sdk/authenticated.py
--rw-r--r--   0 solomeowl   (501) staff       (20)     3754 2024-03-24 15:57:21.000000 backpack_exchange_sdk-0.2.5/backpack_exchange_sdk/public.py
-drwxr-xr-x   0 solomeowl   (501) staff       (20)        0 2024-04-02 16:04:12.726390 backpack_exchange_sdk-0.2.5/backpack_exchange_sdk.egg-info/
--rw-r--r--   0 solomeowl   (501) staff       (20)     2477 2024-04-02 16:04:12.000000 backpack_exchange_sdk-0.2.5/backpack_exchange_sdk.egg-info/PKG-INFO
--rw-r--r--   0 solomeowl   (501) staff       (20)      360 2024-04-02 16:04:12.000000 backpack_exchange_sdk-0.2.5/backpack_exchange_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 solomeowl   (501) staff       (20)        1 2024-04-02 16:04:12.000000 backpack_exchange_sdk-0.2.5/backpack_exchange_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 solomeowl   (501) staff       (20)       22 2024-04-02 16:04:12.000000 backpack_exchange_sdk-0.2.5/backpack_exchange_sdk.egg-info/top_level.txt
--rw-r--r--   0 solomeowl   (501) staff       (20)       38 2024-04-02 16:04:12.727011 backpack_exchange_sdk-0.2.5/setup.cfg
--rw-r--r--   0 solomeowl   (501) staff       (20)      533 2024-04-02 16:04:04.000000 backpack_exchange_sdk-0.2.5/setup.py
-drwxr-xr-x   0 solomeowl   (501) staff       (20)        0 2024-04-02 16:04:12.726185 backpack_exchange_sdk-0.2.5/tests/
--rw-r--r--   0 solomeowl   (501) staff       (20)        0 2024-03-09 08:00:27.000000 backpack_exchange_sdk-0.2.5/tests/test_authenticated.py
--rw-r--r--   0 solomeowl   (501) staff       (20)        0 2024-03-09 08:00:27.000000 backpack_exchange_sdk-0.2.5/tests/test_public.py
+drwxr-xr-x   0 solomeowl   (501) staff       (20)        0 2024-04-02 16:08:07.649361 backpack_exchange_sdk-0.2.6/
+-rw-r--r--   0 solomeowl   (501) staff       (20)     1066 2024-03-08 15:43:17.000000 backpack_exchange_sdk-0.2.6/LICENSE
+-rw-r--r--   0 solomeowl   (501) staff       (20)     2477 2024-04-02 16:08:07.649050 backpack_exchange_sdk-0.2.6/PKG-INFO
+-rw-r--r--   0 solomeowl   (501) staff       (20)     2119 2024-04-02 15:44:43.000000 backpack_exchange_sdk-0.2.6/README.md
+drwxr-xr-x   0 solomeowl   (501) staff       (20)        0 2024-04-02 16:08:07.644331 backpack_exchange_sdk-0.2.6/backpack_exchange_sdk/
+-rw-r--r--   0 solomeowl   (501) staff       (20)        0 2024-04-02 16:07:47.000000 backpack_exchange_sdk-0.2.6/backpack_exchange_sdk/__init__.py
+-rw-r--r--   0 solomeowl   (501) staff       (20)     9416 2024-04-02 16:03:57.000000 backpack_exchange_sdk-0.2.6/backpack_exchange_sdk/authenticated.py
+-rw-r--r--   0 solomeowl   (501) staff       (20)     3754 2024-03-24 15:57:21.000000 backpack_exchange_sdk-0.2.6/backpack_exchange_sdk/public.py
+drwxr-xr-x   0 solomeowl   (501) staff       (20)        0 2024-04-02 16:08:07.648826 backpack_exchange_sdk-0.2.6/backpack_exchange_sdk.egg-info/
+-rw-r--r--   0 solomeowl   (501) staff       (20)     2477 2024-04-02 16:08:07.000000 backpack_exchange_sdk-0.2.6/backpack_exchange_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 solomeowl   (501) staff       (20)      423 2024-04-02 16:08:07.000000 backpack_exchange_sdk-0.2.6/backpack_exchange_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 solomeowl   (501) staff       (20)        1 2024-04-02 16:08:07.000000 backpack_exchange_sdk-0.2.6/backpack_exchange_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 solomeowl   (501) staff       (20)       28 2024-04-02 16:08:07.000000 backpack_exchange_sdk-0.2.6/backpack_exchange_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 solomeowl   (501) staff       (20)        0 2024-04-02 16:08:07.648418 backpack_exchange_sdk-0.2.6/enums/
+-rw-r--r--   0 solomeowl   (501) staff       (20)      368 2024-03-24 15:57:21.000000 backpack_exchange_sdk-0.2.6/enums/RequestEnums.py
+-rw-r--r--   0 solomeowl   (501) staff       (20)      248 2024-03-24 15:57:21.000000 backpack_exchange_sdk-0.2.6/enums/ResponseEnums.py
+-rw-r--r--   0 solomeowl   (501) staff       (20)        0 2024-04-02 16:07:48.000000 backpack_exchange_sdk-0.2.6/enums/__init__.py
+-rw-r--r--   0 solomeowl   (501) staff       (20)       38 2024-04-02 16:08:07.649412 backpack_exchange_sdk-0.2.6/setup.cfg
+-rw-r--r--   0 solomeowl   (501) staff       (20)      533 2024-04-02 16:07:59.000000 backpack_exchange_sdk-0.2.6/setup.py
+drwxr-xr-x   0 solomeowl   (501) staff       (20)        0 2024-04-02 16:08:07.648657 backpack_exchange_sdk-0.2.6/tests/
+-rw-r--r--   0 solomeowl   (501) staff       (20)        0 2024-03-09 08:00:27.000000 backpack_exchange_sdk-0.2.6/tests/test_authenticated.py
+-rw-r--r--   0 solomeowl   (501) staff       (20)        0 2024-03-09 08:00:27.000000 backpack_exchange_sdk-0.2.6/tests/test_public.py
```

### Comparing `backpack_exchange_sdk-0.2.5/LICENSE` & `backpack_exchange_sdk-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `backpack_exchange_sdk-0.2.5/PKG-INFO` & `backpack_exchange_sdk-0.2.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backpack_exchange_sdk
-Version: 0.2.5
+Version: 0.2.6
 Summary: A simple SDK for backpack exchange
 Home-page: https://github.com/solomeowl/backpack_exchange_sdk
 Author: solomeowl
 Author-email: j19940430@gmail.com
 Project-URL: Source, https://github.com/solomeowl/backpack_exchange_sdk
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `backpack_exchange_sdk-0.2.5/README.md` & `backpack_exchange_sdk-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `backpack_exchange_sdk-0.2.5/backpack_exchange_sdk/authenticated.py` & `backpack_exchange_sdk-0.2.6/backpack_exchange_sdk/authenticated.py`

 * *Files identical despite different names*

### Comparing `backpack_exchange_sdk-0.2.5/backpack_exchange_sdk/public.py` & `backpack_exchange_sdk-0.2.6/backpack_exchange_sdk/public.py`

 * *Files identical despite different names*

### Comparing `backpack_exchange_sdk-0.2.5/backpack_exchange_sdk.egg-info/PKG-INFO` & `backpack_exchange_sdk-0.2.6/backpack_exchange_sdk.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backpack_exchange_sdk
-Version: 0.2.5
+Version: 0.2.6
 Summary: A simple SDK for backpack exchange
 Home-page: https://github.com/solomeowl/backpack_exchange_sdk
 Author: solomeowl
 Author-email: j19940430@gmail.com
 Project-URL: Source, https://github.com/solomeowl/backpack_exchange_sdk
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `backpack_exchange_sdk-0.2.5/setup.py` & `backpack_exchange_sdk-0.2.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="backpack_exchange_sdk",
-    version="0.2.5",
+    version="0.2.6",
     author="solomeowl",
     author_email="j19940430@gmail.com",
     description="A simple SDK for backpack exchange",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/solomeowl/backpack_exchange_sdk",
     project_urls={
```

