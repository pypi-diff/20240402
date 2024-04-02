# Comparing `tmp/catnekaise.ghrawel-0.0.7.tar.gz` & `tmp/catnekaise.ghrawel-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catnekaise.ghrawel-0.0.7.tar", last modified: Tue Mar 26 08:12:26 2024, max compression
+gzip compressed data, was "catnekaise.ghrawel-0.0.8.tar", last modified: Tue Apr  2 06:51:31 2024, max compression
```

## Comparing `catnekaise.ghrawel-0.0.7.tar` & `catnekaise.ghrawel-0.0.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:12:26.089177 catnekaise.ghrawel-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-03-26 08:12:12.000000 catnekaise.ghrawel-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-26 08:12:12.000000 catnekaise.ghrawel-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    18327 2024-03-26 08:12:26.089177 catnekaise.ghrawel-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17320 2024-03-26 08:12:12.000000 catnekaise.ghrawel-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-26 08:12:12.000000 catnekaise.ghrawel-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 08:12:26.089177 catnekaise.ghrawel-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-03-26 08:12:12.000000 catnekaise.ghrawel-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:12:26.085177 catnekaise.ghrawel-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:12:26.089177 catnekaise.ghrawel-0.0.7/src/catnekaise.ghrawel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18327 2024-03-26 08:12:26.000000 catnekaise.ghrawel-0.0.7/src/catnekaise.ghrawel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-03-26 08:12:26.000000 catnekaise.ghrawel-0.0.7/src/catnekaise.ghrawel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 08:12:26.000000 catnekaise.ghrawel-0.0.7/src/catnekaise.ghrawel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-03-26 08:12:26.000000 catnekaise.ghrawel-0.0.7/src/catnekaise.ghrawel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-26 08:12:26.000000 catnekaise.ghrawel-0.0.7/src/catnekaise.ghrawel.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:12:26.089177 catnekaise.ghrawel-0.0.7/src/catnekaise_ghrawel/
--rw-r--r--   0 runner    (1001) docker     (127)   169741 2024-03-26 08:12:12.000000 catnekaise.ghrawel-0.0.7/src/catnekaise_ghrawel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:12:26.089177 catnekaise.ghrawel-0.0.7/src/catnekaise_ghrawel/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-03-26 08:12:12.000000 catnekaise.ghrawel-0.0.7/src/catnekaise_ghrawel/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   213782 2024-03-26 08:12:12.000000 catnekaise.ghrawel-0.0.7/src/catnekaise_ghrawel/_jsii/ghrawel@0.0.7.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 08:12:12.000000 catnekaise.ghrawel-0.0.7/src/catnekaise_ghrawel/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:51:31.792390 catnekaise.ghrawel-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-02 06:51:21.000000 catnekaise.ghrawel-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-02 06:51:21.000000 catnekaise.ghrawel-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    18327 2024-04-02 06:51:31.792390 catnekaise.ghrawel-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17320 2024-04-02 06:51:21.000000 catnekaise.ghrawel-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-02 06:51:21.000000 catnekaise.ghrawel-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 06:51:31.792390 catnekaise.ghrawel-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-02 06:51:21.000000 catnekaise.ghrawel-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:51:31.792390 catnekaise.ghrawel-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:51:31.792390 catnekaise.ghrawel-0.0.8/src/catnekaise.ghrawel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18327 2024-04-02 06:51:31.000000 catnekaise.ghrawel-0.0.8/src/catnekaise.ghrawel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-02 06:51:31.000000 catnekaise.ghrawel-0.0.8/src/catnekaise.ghrawel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 06:51:31.000000 catnekaise.ghrawel-0.0.8/src/catnekaise.ghrawel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-02 06:51:31.000000 catnekaise.ghrawel-0.0.8/src/catnekaise.ghrawel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-02 06:51:31.000000 catnekaise.ghrawel-0.0.8/src/catnekaise.ghrawel.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:51:31.792390 catnekaise.ghrawel-0.0.8/src/catnekaise_ghrawel/
+-rw-r--r--   0 runner    (1001) docker     (127)   169741 2024-04-02 06:51:21.000000 catnekaise.ghrawel-0.0.8/src/catnekaise_ghrawel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:51:31.792390 catnekaise.ghrawel-0.0.8/src/catnekaise_ghrawel/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-02 06:51:21.000000 catnekaise.ghrawel-0.0.8/src/catnekaise_ghrawel/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   213785 2024-04-02 06:51:21.000000 catnekaise.ghrawel-0.0.8/src/catnekaise_ghrawel/_jsii/ghrawel@0.0.8.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 06:51:21.000000 catnekaise.ghrawel-0.0.8/src/catnekaise_ghrawel/py.typed
```

### Comparing `catnekaise.ghrawel-0.0.7/LICENSE` & `catnekaise.ghrawel-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `catnekaise.ghrawel-0.0.7/PKG-INFO` & `catnekaise.ghrawel-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catnekaise.ghrawel
-Version: 0.0.7
+Version: 0.0.8
 Summary: Use ghrawel to deploy an AWS API Gateway RestAPI capable of returning GitHub App installation access tokens and use AWS IAM to control access to this API.
 Home-page: https://github.com/catnekaise/ghrawel.git
 Author: Daniel Jonsén<djonser1@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/catnekaise/ghrawel.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `catnekaise.ghrawel-0.0.7/README.md` & `catnekaise.ghrawel-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `catnekaise.ghrawel-0.0.7/setup.py` & `catnekaise.ghrawel-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "catnekaise.ghrawel",
-    "version": "0.0.7",
+    "version": "0.0.8",
     "description": "Use ghrawel to deploy an AWS API Gateway RestAPI capable of returning GitHub App installation access tokens and use AWS IAM to control access to this API.",
     "license": "Apache-2.0",
     "url": "https://github.com/catnekaise/ghrawel.git",
     "long_description_content_type": "text/markdown",
     "author": "Daniel Jonsén<djonser1@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "catnekaise_ghrawel",
         "catnekaise_ghrawel._jsii"
     ],
     "package_data": {
         "catnekaise_ghrawel._jsii": [
-            "ghrawel@0.0.7.jsii.tgz"
+            "ghrawel@0.0.8.jsii.tgz"
         ],
         "catnekaise_ghrawel": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `catnekaise.ghrawel-0.0.7/src/catnekaise.ghrawel.egg-info/PKG-INFO` & `catnekaise.ghrawel-0.0.8/src/catnekaise.ghrawel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catnekaise.ghrawel
-Version: 0.0.7
+Version: 0.0.8
 Summary: Use ghrawel to deploy an AWS API Gateway RestAPI capable of returning GitHub App installation access tokens and use AWS IAM to control access to this API.
 Home-page: https://github.com/catnekaise/ghrawel.git
 Author: Daniel Jonsén<djonser1@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/catnekaise/ghrawel.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `catnekaise.ghrawel-0.0.7/src/catnekaise_ghrawel/__init__.py` & `catnekaise.ghrawel-0.0.8/src/catnekaise_ghrawel/__init__.py`

 * *Files identical despite different names*

