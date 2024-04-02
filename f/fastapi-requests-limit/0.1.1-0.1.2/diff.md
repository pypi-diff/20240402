# Comparing `tmp/fastapi-requests-limit-0.1.1.tar.gz` & `tmp/fastapi-requests-limit-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-requests-limit-0.1.1.tar", last modified: Tue Apr  2 21:08:12 2024, max compression
+gzip compressed data, was "fastapi-requests-limit-0.1.2.tar", last modified: Tue Apr  2 21:20:04 2024, max compression
```

## Comparing `fastapi-requests-limit-0.1.1.tar` & `fastapi-requests-limit-0.1.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 21:08:12.128140 fastapi-requests-limit-0.1.1/
--rw-rw-rw-   0        0        0     1106 2024-03-21 23:13:37.000000 fastapi-requests-limit-0.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0     3922 2024-04-02 21:08:12.128140 fastapi-requests-limit-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2928 2024-04-02 21:08:00.000000 fastapi-requests-limit-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-02 21:08:12.076216 fastapi-requests-limit-0.1.1/fastapi_requests_limit/
--rw-rw-rw-   0        0        0        0 2023-10-17 00:43:53.000000 fastapi-requests-limit-0.1.1/fastapi_requests_limit/__init__.py
--rw-rw-rw-   0        0        0      864 2024-04-02 20:00:53.000000 fastapi-requests-limit-0.1.1/fastapi_requests_limit/configuration.py
--rw-rw-rw-   0        0        0      538 2024-04-02 20:00:53.000000 fastapi-requests-limit-0.1.1/fastapi_requests_limit/handle_errors.py
--rw-rw-rw-   0        0        0     2162 2024-04-02 20:00:54.000000 fastapi-requests-limit-0.1.1/fastapi_requests_limit/limiter_rest.py
--rw-rw-rw-   0        0        0      270 2024-04-02 21:06:26.000000 fastapi-requests-limit-0.1.1/fastapi_requests_limit/storage_engines.py
-drwxrwxrwx   0        0        0        0 2024-04-02 21:08:12.122873 fastapi-requests-limit-0.1.1/fastapi_requests_limit/storages/
--rw-rw-rw-   0        0        0        0 2023-10-19 02:31:00.000000 fastapi-requests-limit-0.1.1/fastapi_requests_limit/storages/__init__.py
--rw-rw-rw-   0        0        0      771 2024-04-02 20:00:54.000000 fastapi-requests-limit-0.1.1/fastapi_requests_limit/storages/memory.py
--rw-rw-rw-   0        0        0        0 2023-10-19 02:31:30.000000 fastapi-requests-limit-0.1.1/fastapi_requests_limit/storages/mondodb.py
--rw-rw-rw-   0        0        0      897 2024-04-02 20:00:53.000000 fastapi-requests-limit-0.1.1/fastapi_requests_limit/storages/redis.py
--rw-rw-rw-   0        0        0      589 2024-04-02 20:03:20.000000 fastapi-requests-limit-0.1.1/fastapi_requests_limit/storages/storage.py
-drwxrwxrwx   0        0        0        0 2024-04-02 21:08:12.127071 fastapi-requests-limit-0.1.1/fastapi_requests_limit/test/
--rw-rw-rw-   0        0        0        0 2023-11-09 21:24:25.000000 fastapi-requests-limit-0.1.1/fastapi_requests_limit/test/__init__.py
--rw-rw-rw-   0        0        0      282 2023-11-17 23:12:25.000000 fastapi-requests-limit-0.1.1/fastapi_requests_limit/test/mock.py
--rw-rw-rw-   0        0        0      420 2024-04-02 20:03:32.000000 fastapi-requests-limit-0.1.1/fastapi_requests_limit/test/test.py
--rw-rw-rw-   0        0        0       33 2023-11-17 16:42:06.000000 fastapi-requests-limit-0.1.1/fastapi_requests_limit/test/test_constans.py
--rw-rw-rw-   0        0        0     1517 2024-04-02 21:06:26.000000 fastapi-requests-limit-0.1.1/fastapi_requests_limit/test/test_limiter_memory.py
-drwxrwxrwx   0        0        0        0 2024-04-02 21:08:12.119329 fastapi-requests-limit-0.1.1/fastapi_requests_limit.egg-info/
--rw-rw-rw-   0        0        0     3922 2024-04-02 21:08:12.000000 fastapi-requests-limit-0.1.1/fastapi_requests_limit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      876 2024-04-02 21:08:12.000000 fastapi-requests-limit-0.1.1/fastapi_requests_limit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 21:08:12.000000 fastapi-requests-limit-0.1.1/fastapi_requests_limit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-02 21:08:12.000000 fastapi-requests-limit-0.1.1/fastapi_requests_limit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2024-04-02 21:08:12.000000 fastapi-requests-limit-0.1.1/fastapi_requests_limit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-02 21:08:12.129162 fastapi-requests-limit-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1359 2024-04-02 21:06:26.000000 fastapi-requests-limit-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 21:20:04.008581 fastapi-requests-limit-0.1.2/
+-rw-rw-rw-   0        0        0     1106 2024-03-21 23:13:37.000000 fastapi-requests-limit-0.1.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     3922 2024-04-02 21:20:04.008581 fastapi-requests-limit-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2928 2024-04-02 21:08:00.000000 fastapi-requests-limit-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 21:20:03.983886 fastapi-requests-limit-0.1.2/fastapi_requests_limit/
+-rw-rw-rw-   0        0        0        0 2023-10-17 00:43:53.000000 fastapi-requests-limit-0.1.2/fastapi_requests_limit/__init__.py
+-rw-rw-rw-   0        0        0      864 2024-04-02 20:00:53.000000 fastapi-requests-limit-0.1.2/fastapi_requests_limit/configuration.py
+-rw-rw-rw-   0        0        0      538 2024-04-02 20:00:53.000000 fastapi-requests-limit-0.1.2/fastapi_requests_limit/handle_errors.py
+-rw-rw-rw-   0        0        0     2162 2024-04-02 20:00:54.000000 fastapi-requests-limit-0.1.2/fastapi_requests_limit/limiter_rest.py
+-rw-rw-rw-   0        0        0      270 2024-04-02 21:06:26.000000 fastapi-requests-limit-0.1.2/fastapi_requests_limit/storage_engines.py
+drwxrwxrwx   0        0        0        0 2024-04-02 21:20:04.004385 fastapi-requests-limit-0.1.2/fastapi_requests_limit/storages/
+-rw-rw-rw-   0        0        0        0 2023-10-19 02:31:00.000000 fastapi-requests-limit-0.1.2/fastapi_requests_limit/storages/__init__.py
+-rw-rw-rw-   0        0        0      771 2024-04-02 20:00:54.000000 fastapi-requests-limit-0.1.2/fastapi_requests_limit/storages/memory.py
+-rw-rw-rw-   0        0        0        0 2023-10-19 02:31:30.000000 fastapi-requests-limit-0.1.2/fastapi_requests_limit/storages/mondodb.py
+-rw-rw-rw-   0        0        0      897 2024-04-02 20:00:53.000000 fastapi-requests-limit-0.1.2/fastapi_requests_limit/storages/redis.py
+-rw-rw-rw-   0        0        0      589 2024-04-02 20:03:20.000000 fastapi-requests-limit-0.1.2/fastapi_requests_limit/storages/storage.py
+drwxrwxrwx   0        0        0        0 2024-04-02 21:20:04.007452 fastapi-requests-limit-0.1.2/fastapi_requests_limit/test/
+-rw-rw-rw-   0        0        0        0 2023-11-09 21:24:25.000000 fastapi-requests-limit-0.1.2/fastapi_requests_limit/test/__init__.py
+-rw-rw-rw-   0        0        0      282 2023-11-17 23:12:25.000000 fastapi-requests-limit-0.1.2/fastapi_requests_limit/test/mock.py
+-rw-rw-rw-   0        0        0      420 2024-04-02 20:03:32.000000 fastapi-requests-limit-0.1.2/fastapi_requests_limit/test/test.py
+-rw-rw-rw-   0        0        0       33 2023-11-17 16:42:06.000000 fastapi-requests-limit-0.1.2/fastapi_requests_limit/test/test_constans.py
+-rw-rw-rw-   0        0        0     1517 2024-04-02 21:06:26.000000 fastapi-requests-limit-0.1.2/fastapi_requests_limit/test/test_limiter_memory.py
+drwxrwxrwx   0        0        0        0 2024-04-02 21:20:04.001219 fastapi-requests-limit-0.1.2/fastapi_requests_limit.egg-info/
+-rw-rw-rw-   0        0        0     3922 2024-04-02 21:20:03.000000 fastapi-requests-limit-0.1.2/fastapi_requests_limit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      876 2024-04-02 21:20:03.000000 fastapi-requests-limit-0.1.2/fastapi_requests_limit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 21:20:03.000000 fastapi-requests-limit-0.1.2/fastapi_requests_limit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-02 21:20:03.000000 fastapi-requests-limit-0.1.2/fastapi_requests_limit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2024-04-02 21:20:03.000000 fastapi-requests-limit-0.1.2/fastapi_requests_limit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-02 21:20:04.008581 fastapi-requests-limit-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1302 2024-04-02 21:19:15.000000 fastapi-requests-limit-0.1.2/setup.py
```

### Comparing `fastapi-requests-limit-0.1.1/LICENSE.txt` & `fastapi-requests-limit-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fastapi-requests-limit-0.1.1/PKG-INFO` & `fastapi-requests-limit-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-requests-limit
-Version: 0.1.1
+Version: 0.1.2
 Summary: Control and limit request rates to FastAPI applications with Redis and local memory support.
 Home-page: https://github.com/oscarPyth/fastapi-limit-requests
 Author: Oscar Arias
 Author-email: ariasp26@gmail.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/oscarPyth/fastapi-limit-requests/issues
 Project-URL: Source, https://github.com/oscarPyth/fastapi-limit-requests
```

### Comparing `fastapi-requests-limit-0.1.1/README.md` & `fastapi-requests-limit-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `fastapi-requests-limit-0.1.1/fastapi_requests_limit/configuration.py` & `fastapi-requests-limit-0.1.2/fastapi_requests_limit/configuration.py`

 * *Files identical despite different names*

### Comparing `fastapi-requests-limit-0.1.1/fastapi_requests_limit/handle_errors.py` & `fastapi-requests-limit-0.1.2/fastapi_requests_limit/handle_errors.py`

 * *Files identical despite different names*

### Comparing `fastapi-requests-limit-0.1.1/fastapi_requests_limit/limiter_rest.py` & `fastapi-requests-limit-0.1.2/fastapi_requests_limit/limiter_rest.py`

 * *Files identical despite different names*

### Comparing `fastapi-requests-limit-0.1.1/fastapi_requests_limit/storages/memory.py` & `fastapi-requests-limit-0.1.2/fastapi_requests_limit/storages/memory.py`

 * *Files identical despite different names*

### Comparing `fastapi-requests-limit-0.1.1/fastapi_requests_limit/storages/redis.py` & `fastapi-requests-limit-0.1.2/fastapi_requests_limit/storages/redis.py`

 * *Files identical despite different names*

### Comparing `fastapi-requests-limit-0.1.1/fastapi_requests_limit/storages/storage.py` & `fastapi-requests-limit-0.1.2/fastapi_requests_limit/storages/storage.py`

 * *Files identical despite different names*

### Comparing `fastapi-requests-limit-0.1.1/fastapi_requests_limit/test/test_limiter_memory.py` & `fastapi-requests-limit-0.1.2/fastapi_requests_limit/test/test_limiter_memory.py`

 * *Files identical despite different names*

### Comparing `fastapi-requests-limit-0.1.1/fastapi_requests_limit.egg-info/PKG-INFO` & `fastapi-requests-limit-0.1.2/fastapi_requests_limit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-requests-limit
-Version: 0.1.1
+Version: 0.1.2
 Summary: Control and limit request rates to FastAPI applications with Redis and local memory support.
 Home-page: https://github.com/oscarPyth/fastapi-limit-requests
 Author: Oscar Arias
 Author-email: ariasp26@gmail.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/oscarPyth/fastapi-limit-requests/issues
 Project-URL: Source, https://github.com/oscarPyth/fastapi-limit-requests
```

### Comparing `fastapi-requests-limit-0.1.1/fastapi_requests_limit.egg-info/SOURCES.txt` & `fastapi-requests-limit-0.1.2/fastapi_requests_limit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastapi-requests-limit-0.1.1/setup.py` & `fastapi-requests-limit-0.1.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from setuptools import find_packages, setup
 
-with open("requirements.txt") as f:
-    requirements = f.read().splitlines()
-
 setup(
     name="fastapi-requests-limit",
-    version="0.1.1",
+    version="0.1.2",
     author="Oscar Arias",
     author_email="ariasp26@gmail.com",
     description="Control and limit request rates to FastAPI applications with Redis and local memory support.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/oscarPyth/fastapi-limit-requests",
     packages=find_packages(),
-    install_requires=requirements,
+    install_requires=[
+        "fastapi>=0.103.2"
+    ],
     license="MIT",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
```

