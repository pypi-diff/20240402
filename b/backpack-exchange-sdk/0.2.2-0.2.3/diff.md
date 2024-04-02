# Comparing `tmp/backpack_exchange_sdk-0.2.2.tar.gz` & `tmp/backpack_exchange_sdk-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backpack_exchange_sdk-0.2.2.tar", last modified: Tue Apr  2 15:49:18 2024, max compression
+gzip compressed data, was "backpack_exchange_sdk-0.2.3.tar", last modified: Tue Apr  2 15:54:41 2024, max compression
```

## Comparing `backpack_exchange_sdk-0.2.2.tar` & `backpack_exchange_sdk-0.2.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 solomeowl   (501) staff       (20)        0 2024-04-02 15:49:18.297391 backpack_exchange_sdk-0.2.2/
--rw-r--r--   0 solomeowl   (501) staff       (20)     1066 2024-03-08 15:43:17.000000 backpack_exchange_sdk-0.2.2/LICENSE
--rw-r--r--   0 solomeowl   (501) staff       (20)     2477 2024-04-02 15:49:18.297084 backpack_exchange_sdk-0.2.2/PKG-INFO
--rw-r--r--   0 solomeowl   (501) staff       (20)     2119 2024-04-02 15:44:43.000000 backpack_exchange_sdk-0.2.2/README.md
-drwxr-xr-x   0 solomeowl   (501) staff       (20)        0 2024-04-02 15:49:18.295604 backpack_exchange_sdk-0.2.2/backpack_exchange_sdk/
--rw-r--r--   0 solomeowl   (501) staff       (20)        0 2024-03-09 08:21:03.000000 backpack_exchange_sdk-0.2.2/backpack_exchange_sdk/__init__.py
--rw-r--r--   0 solomeowl   (501) staff       (20)     9295 2024-03-24 16:07:16.000000 backpack_exchange_sdk-0.2.2/backpack_exchange_sdk/authenticated.py
--rw-r--r--   0 solomeowl   (501) staff       (20)     3754 2024-03-24 15:57:21.000000 backpack_exchange_sdk-0.2.2/backpack_exchange_sdk/public.py
-drwxr-xr-x   0 solomeowl   (501) staff       (20)        0 2024-04-02 15:49:18.296789 backpack_exchange_sdk-0.2.2/backpack_exchange_sdk.egg-info/
--rw-r--r--   0 solomeowl   (501) staff       (20)     2477 2024-04-02 15:49:18.000000 backpack_exchange_sdk-0.2.2/backpack_exchange_sdk.egg-info/PKG-INFO
--rw-r--r--   0 solomeowl   (501) staff       (20)      360 2024-04-02 15:49:18.000000 backpack_exchange_sdk-0.2.2/backpack_exchange_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 solomeowl   (501) staff       (20)        1 2024-04-02 15:49:18.000000 backpack_exchange_sdk-0.2.2/backpack_exchange_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 solomeowl   (501) staff       (20)       22 2024-04-02 15:49:18.000000 backpack_exchange_sdk-0.2.2/backpack_exchange_sdk.egg-info/top_level.txt
--rw-r--r--   0 solomeowl   (501) staff       (20)       38 2024-04-02 15:49:18.297459 backpack_exchange_sdk-0.2.2/setup.cfg
--rw-r--r--   0 solomeowl   (501) staff       (20)      533 2024-04-02 15:49:05.000000 backpack_exchange_sdk-0.2.2/setup.py
-drwxr-xr-x   0 solomeowl   (501) staff       (20)        0 2024-04-02 15:49:18.296589 backpack_exchange_sdk-0.2.2/tests/
--rw-r--r--   0 solomeowl   (501) staff       (20)        0 2024-03-09 08:00:27.000000 backpack_exchange_sdk-0.2.2/tests/test_authenticated.py
--rw-r--r--   0 solomeowl   (501) staff       (20)        0 2024-03-09 08:00:27.000000 backpack_exchange_sdk-0.2.2/tests/test_public.py
+drwxr-xr-x   0 solomeowl   (501) staff       (20)        0 2024-04-02 15:54:41.218866 backpack_exchange_sdk-0.2.3/
+-rw-r--r--   0 solomeowl   (501) staff       (20)     1066 2024-03-08 15:43:17.000000 backpack_exchange_sdk-0.2.3/LICENSE
+-rw-r--r--   0 solomeowl   (501) staff       (20)     2477 2024-04-02 15:54:41.218608 backpack_exchange_sdk-0.2.3/PKG-INFO
+-rw-r--r--   0 solomeowl   (501) staff       (20)     2119 2024-04-02 15:44:43.000000 backpack_exchange_sdk-0.2.3/README.md
+drwxr-xr-x   0 solomeowl   (501) staff       (20)        0 2024-04-02 15:54:41.216731 backpack_exchange_sdk-0.2.3/backpack_exchange_sdk/
+-rw-r--r--   0 solomeowl   (501) staff       (20)        0 2024-03-09 08:21:03.000000 backpack_exchange_sdk-0.2.3/backpack_exchange_sdk/__init__.py
+-rw-r--r--   0 solomeowl   (501) staff       (20)     9297 2024-04-02 15:54:09.000000 backpack_exchange_sdk-0.2.3/backpack_exchange_sdk/authenticated.py
+-rw-r--r--   0 solomeowl   (501) staff       (20)     3754 2024-03-24 15:57:21.000000 backpack_exchange_sdk-0.2.3/backpack_exchange_sdk/public.py
+drwxr-xr-x   0 solomeowl   (501) staff       (20)        0 2024-04-02 15:54:41.218317 backpack_exchange_sdk-0.2.3/backpack_exchange_sdk.egg-info/
+-rw-r--r--   0 solomeowl   (501) staff       (20)     2477 2024-04-02 15:54:41.000000 backpack_exchange_sdk-0.2.3/backpack_exchange_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 solomeowl   (501) staff       (20)      360 2024-04-02 15:54:41.000000 backpack_exchange_sdk-0.2.3/backpack_exchange_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 solomeowl   (501) staff       (20)        1 2024-04-02 15:54:41.000000 backpack_exchange_sdk-0.2.3/backpack_exchange_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 solomeowl   (501) staff       (20)       22 2024-04-02 15:54:41.000000 backpack_exchange_sdk-0.2.3/backpack_exchange_sdk.egg-info/top_level.txt
+-rw-r--r--   0 solomeowl   (501) staff       (20)       38 2024-04-02 15:54:41.218934 backpack_exchange_sdk-0.2.3/setup.cfg
+-rw-r--r--   0 solomeowl   (501) staff       (20)      533 2024-04-02 15:54:36.000000 backpack_exchange_sdk-0.2.3/setup.py
+drwxr-xr-x   0 solomeowl   (501) staff       (20)        0 2024-04-02 15:54:41.218106 backpack_exchange_sdk-0.2.3/tests/
+-rw-r--r--   0 solomeowl   (501) staff       (20)        0 2024-03-09 08:00:27.000000 backpack_exchange_sdk-0.2.3/tests/test_authenticated.py
+-rw-r--r--   0 solomeowl   (501) staff       (20)        0 2024-03-09 08:00:27.000000 backpack_exchange_sdk-0.2.3/tests/test_public.py
```

### Comparing `backpack_exchange_sdk-0.2.2/LICENSE` & `backpack_exchange_sdk-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `backpack_exchange_sdk-0.2.2/PKG-INFO` & `backpack_exchange_sdk-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backpack_exchange_sdk
-Version: 0.2.2
+Version: 0.2.3
 Summary: A simple SDK for backpack exchange
 Home-page: https://github.com/solomeowl/backpack_exchange_sdk
 Author: solomeowl
 Author-email: j19940430@gmail.com
 Project-URL: Source, https://github.com/solomeowl/backpack_exchange_sdk
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `backpack_exchange_sdk-0.2.2/README.md` & `backpack_exchange_sdk-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `backpack_exchange_sdk-0.2.2/backpack_exchange_sdk/authenticated.py` & `backpack_exchange_sdk-0.2.3/backpack_exchange_sdk/authenticated.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     # Capital - Capital management.
     # ================================================================
     def get_balances(self):
         """
         Retrieves account balances and the state of the balances (locked or available).
         Locked assets are those that are currently in an open order.
         """
-        return self._send_request('GET', 'api/v1/capital', 'balanceQuery', {})
+        return self._send_request('GET', 'api/v1/capital', 'balanceQuery', None)
 
     def get_deposits(self, limit: int = 100, offset: int = 0):
         """
         Retrieves deposit history.
         """
         params = {'limit': limit, 'offset': offset}
         return self._send_request('GET', 'wapi/v1/capital/deposits', 'depositQueryAll', params)
```

### Comparing `backpack_exchange_sdk-0.2.2/backpack_exchange_sdk/public.py` & `backpack_exchange_sdk-0.2.3/backpack_exchange_sdk/public.py`

 * *Files identical despite different names*

### Comparing `backpack_exchange_sdk-0.2.2/backpack_exchange_sdk.egg-info/PKG-INFO` & `backpack_exchange_sdk-0.2.3/backpack_exchange_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backpack_exchange_sdk
-Version: 0.2.2
+Version: 0.2.3
 Summary: A simple SDK for backpack exchange
 Home-page: https://github.com/solomeowl/backpack_exchange_sdk
 Author: solomeowl
 Author-email: j19940430@gmail.com
 Project-URL: Source, https://github.com/solomeowl/backpack_exchange_sdk
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `backpack_exchange_sdk-0.2.2/setup.py` & `backpack_exchange_sdk-0.2.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="backpack_exchange_sdk",
-    version="0.2.2",
+    version="0.2.3",
     author="solomeowl",
     author_email="j19940430@gmail.com",
     description="A simple SDK for backpack exchange",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/solomeowl/backpack_exchange_sdk",
     project_urls={
```

