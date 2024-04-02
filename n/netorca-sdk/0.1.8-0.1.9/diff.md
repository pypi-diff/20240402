# Comparing `tmp/netorca-sdk-0.1.8.tar.gz` & `tmp/netorca-sdk-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netorca-sdk-0.1.8.tar", last modified: Wed Sep 13 14:29:17 2023, max compression
+gzip compressed data, was "netorca-sdk-0.1.9.tar", last modified: Wed Sep 13 14:39:50 2023, max compression
```

## Comparing `netorca-sdk-0.1.8.tar` & `netorca-sdk-0.1.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-13 14:29:17.083665 netorca-sdk-0.1.8/
--rw-rw-rw-   0 root         (0) root         (0)     1068 2023-09-13 14:29:00.000000 netorca-sdk-0.1.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)      733 2023-09-13 14:29:17.083665 netorca-sdk-0.1.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      290 2023-09-13 14:29:00.000000 netorca-sdk-0.1.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-13 14:29:17.082665 netorca-sdk-0.1.8/netorca_sdk/
--rw-rw-rw-   0 root         (0) root         (0)       95 2023-09-13 14:29:00.000000 netorca-sdk-0.1.8/netorca_sdk/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6316 2023-09-13 14:29:00.000000 netorca-sdk-0.1.8/netorca_sdk/auth.py
--rw-rw-rw-   0 root         (0) root         (0)     1343 2023-09-13 14:29:00.000000 netorca-sdk-0.1.8/netorca_sdk/config.py
--rw-rw-rw-   0 root         (0) root         (0)    12279 2023-09-13 14:29:00.000000 netorca-sdk-0.1.8/netorca_sdk/consumer.py
--rw-rw-rw-   0 root         (0) root         (0)       43 2023-09-13 14:29:00.000000 netorca-sdk-0.1.8/netorca_sdk/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     9142 2023-09-13 14:29:00.000000 netorca-sdk-0.1.8/netorca_sdk/netorca.py
--rw-rw-rw-   0 root         (0) root         (0)    10434 2023-09-13 14:29:00.000000 netorca-sdk-0.1.8/netorca_sdk/serviceowner.py
--rw-rw-rw-   0 root         (0) root         (0)      156 2023-09-13 14:29:00.000000 netorca-sdk-0.1.8/netorca_sdk/validations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-13 14:29:17.083665 netorca-sdk-0.1.8/netorca_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)      733 2023-09-13 14:29:17.000000 netorca-sdk-0.1.8/netorca_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      500 2023-09-13 14:29:17.000000 netorca-sdk-0.1.8/netorca_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-09-13 14:29:17.000000 netorca-sdk-0.1.8/netorca_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-09-13 14:29:17.000000 netorca-sdk-0.1.8/netorca_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-09-13 14:29:17.000000 netorca-sdk-0.1.8/netorca_sdk.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      144 2023-09-13 14:29:00.000000 netorca-sdk-0.1.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-09-13 14:29:17.083665 netorca-sdk-0.1.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      852 2023-09-13 14:29:00.000000 netorca-sdk-0.1.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-13 14:29:17.083665 netorca-sdk-0.1.8/tests/
--rw-rw-rw-   0 root         (0) root         (0)     3858 2023-09-13 14:29:00.000000 netorca-sdk-0.1.8/tests/test_auth.py
--rw-rw-rw-   0 root         (0) root         (0)    12250 2023-09-13 14:29:00.000000 netorca-sdk-0.1.8/tests/test_consumer.py
--rw-rw-rw-   0 root         (0) root         (0)    11806 2023-09-13 14:29:00.000000 netorca-sdk-0.1.8/tests/test_netorca.py
--rw-rw-rw-   0 root         (0) root         (0)     7998 2023-09-13 14:29:00.000000 netorca-sdk-0.1.8/tests/test_serviceowner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-13 14:39:50.320729 netorca-sdk-0.1.9/
+-rw-rw-rw-   0 root         (0) root         (0)     1068 2023-09-13 14:39:33.000000 netorca-sdk-0.1.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      758 2023-09-13 14:39:50.320729 netorca-sdk-0.1.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      290 2023-09-13 14:39:33.000000 netorca-sdk-0.1.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-13 14:39:50.319729 netorca-sdk-0.1.9/netorca_sdk/
+-rw-rw-rw-   0 root         (0) root         (0)       95 2023-09-13 14:39:33.000000 netorca-sdk-0.1.9/netorca_sdk/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6316 2023-09-13 14:39:33.000000 netorca-sdk-0.1.9/netorca_sdk/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)     1343 2023-09-13 14:39:33.000000 netorca-sdk-0.1.9/netorca_sdk/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    12279 2023-09-13 14:39:33.000000 netorca-sdk-0.1.9/netorca_sdk/consumer.py
+-rw-rw-rw-   0 root         (0) root         (0)       43 2023-09-13 14:39:33.000000 netorca-sdk-0.1.9/netorca_sdk/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     9142 2023-09-13 14:39:33.000000 netorca-sdk-0.1.9/netorca_sdk/netorca.py
+-rw-rw-rw-   0 root         (0) root         (0)    10434 2023-09-13 14:39:33.000000 netorca-sdk-0.1.9/netorca_sdk/serviceowner.py
+-rw-rw-rw-   0 root         (0) root         (0)      156 2023-09-13 14:39:33.000000 netorca-sdk-0.1.9/netorca_sdk/validations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-13 14:39:50.320729 netorca-sdk-0.1.9/netorca_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      758 2023-09-13 14:39:50.000000 netorca-sdk-0.1.9/netorca_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      500 2023-09-13 14:39:50.000000 netorca-sdk-0.1.9/netorca_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-09-13 14:39:50.000000 netorca-sdk-0.1.9/netorca_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       41 2023-09-13 14:39:50.000000 netorca-sdk-0.1.9/netorca_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-09-13 14:39:50.000000 netorca-sdk-0.1.9/netorca_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      144 2023-09-13 14:39:33.000000 netorca-sdk-0.1.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-09-13 14:39:50.320729 netorca-sdk-0.1.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      873 2023-09-13 14:39:33.000000 netorca-sdk-0.1.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-13 14:39:50.320729 netorca-sdk-0.1.9/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     3858 2023-09-13 14:39:33.000000 netorca-sdk-0.1.9/tests/test_auth.py
+-rw-rw-rw-   0 root         (0) root         (0)    12250 2023-09-13 14:39:33.000000 netorca-sdk-0.1.9/tests/test_consumer.py
+-rw-rw-rw-   0 root         (0) root         (0)    11806 2023-09-13 14:39:33.000000 netorca-sdk-0.1.9/tests/test_netorca.py
+-rw-rw-rw-   0 root         (0) root         (0)     7998 2023-09-13 14:39:33.000000 netorca-sdk-0.1.9/tests/test_serviceowner.py
```

### Comparing `netorca-sdk-0.1.8/LICENSE` & `netorca-sdk-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `netorca-sdk-0.1.8/PKG-INFO` & `netorca-sdk-0.1.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netorca-sdk
-Version: 0.1.8
+Version: 0.1.9
 Summary: A package for interacting with the NetOrca API
 Home-page: https://gitlab.com/netorca_public/netorca_sdk/
 Author: Scott Rowlandson
 Author-email: scott@netautomate.org
 License: MIT
 Keywords: netorca,orchestration,netautomate
 Classifier: Development Status :: 3 - Alpha
@@ -14,7 +14,8 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE
 Requires-Dist: beautifultable
 Requires-Dist: pyyaml
 Requires-Dist: requests
+Requires-Dist: gitpython
```

### Comparing `netorca-sdk-0.1.8/netorca_sdk/auth.py` & `netorca-sdk-0.1.9/netorca_sdk/auth.py`

 * *Files identical despite different names*

### Comparing `netorca-sdk-0.1.8/netorca_sdk/config.py` & `netorca-sdk-0.1.9/netorca_sdk/config.py`

 * *Files identical despite different names*

### Comparing `netorca-sdk-0.1.8/netorca_sdk/consumer.py` & `netorca-sdk-0.1.9/netorca_sdk/consumer.py`

 * *Files identical despite different names*

### Comparing `netorca-sdk-0.1.8/netorca_sdk/netorca.py` & `netorca-sdk-0.1.9/netorca_sdk/netorca.py`

 * *Files identical despite different names*

### Comparing `netorca-sdk-0.1.8/netorca_sdk/serviceowner.py` & `netorca-sdk-0.1.9/netorca_sdk/serviceowner.py`

 * *Files identical despite different names*

### Comparing `netorca-sdk-0.1.8/netorca_sdk.egg-info/PKG-INFO` & `netorca-sdk-0.1.9/netorca_sdk.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netorca-sdk
-Version: 0.1.8
+Version: 0.1.9
 Summary: A package for interacting with the NetOrca API
 Home-page: https://gitlab.com/netorca_public/netorca_sdk/
 Author: Scott Rowlandson
 Author-email: scott@netautomate.org
 License: MIT
 Keywords: netorca,orchestration,netautomate
 Classifier: Development Status :: 3 - Alpha
@@ -14,7 +14,8 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE
 Requires-Dist: beautifultable
 Requires-Dist: pyyaml
 Requires-Dist: requests
+Requires-Dist: gitpython
```

### Comparing `netorca-sdk-0.1.8/setup.py` & `netorca-sdk-0.1.9/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from distutils.core import setup
 
 setup(
     name="netorca-sdk",
     packages=["netorca_sdk"],
-    version="0.1.8",
+    version="0.1.9",
     license="MIT",
     description="A package for interacting with the NetOrca API",
     author="Scott Rowlandson",
     author_email="scott@netautomate.org",
     url="https://gitlab.com/netorca_public/netorca_sdk/",
     keywords=["netorca", "orchestration", "netautomate"],
     install_requires=[
         "beautifultable",
         "pyyaml",
         "requests",
+        "gitpython",
     ],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Build Tools",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.9",
```

### Comparing `netorca-sdk-0.1.8/tests/test_auth.py` & `netorca-sdk-0.1.9/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `netorca-sdk-0.1.8/tests/test_consumer.py` & `netorca-sdk-0.1.9/tests/test_consumer.py`

 * *Files identical despite different names*

### Comparing `netorca-sdk-0.1.8/tests/test_netorca.py` & `netorca-sdk-0.1.9/tests/test_netorca.py`

 * *Files identical despite different names*

### Comparing `netorca-sdk-0.1.8/tests/test_serviceowner.py` & `netorca-sdk-0.1.9/tests/test_serviceowner.py`

 * *Files identical despite different names*

