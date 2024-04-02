# Comparing `tmp/projen-0.80.8.tar.gz` & `tmp/projen-0.80.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "projen-0.80.8.tar", last modified: Wed Mar  6 12:26:18 2024, max compression
+gzip compressed data, was "projen-0.80.9.tar", last modified: Thu Mar  7 10:04:58 2024, max compression
```

## Comparing `projen-0.80.8.tar` & `projen-0.80.9.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 12:26:18.948807 projen-0.80.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-03-06 12:26:08.000000 projen-0.80.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-06 12:26:08.000000 projen-0.80.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    76741 2024-03-06 12:26:18.948807 projen-0.80.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    75912 2024-03-06 12:26:08.000000 projen-0.80.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-06 12:26:08.000000 projen-0.80.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-06 12:26:18.948807 projen-0.80.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-03-06 12:26:08.000000 projen-0.80.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 12:26:18.932807 projen-0.80.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 12:26:18.932807 projen-0.80.8/src/projen/
--rw-r--r--   0 runner    (1001) docker     (127)   649146 2024-03-06 12:26:08.000000 projen-0.80.8/src/projen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 12:26:18.936807 projen-0.80.8/src/projen/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-03-06 12:26:08.000000 projen-0.80.8/src/projen/_jsii/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 12:26:18.936807 projen-0.80.8/src/projen/_jsii/bin/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-03-06 12:26:08.000000 projen-0.80.8/src/projen/_jsii/bin/projen
--rw-r--r--   0 runner    (1001) docker     (127)  2650926 2024-03-06 12:26:08.000000 projen-0.80.8/src/projen/_jsii/projen@0.80.8.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 12:26:18.940807 projen-0.80.8/src/projen/awscdk/
--rw-r--r--   0 runner    (1001) docker     (127)  1074174 2024-03-06 12:26:08.000000 projen-0.80.8/src/projen/awscdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 12:26:18.940807 projen-0.80.8/src/projen/build/
--rw-r--r--   0 runner    (1001) docker     (127)    46549 2024-03-06 12:26:08.000000 projen-0.80.8/src/projen/build/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 12:26:18.940807 projen-0.80.8/src/projen/cdk/
--rw-r--r--   0 runner    (1001) docker     (127)   505357 2024-03-06 12:26:08.000000 projen-0.80.8/src/projen/cdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 12:26:18.940807 projen-0.80.8/src/projen/cdk8s/
--rw-r--r--   0 runner    (1001) docker     (127)   593908 2024-03-06 12:26:08.000000 projen-0.80.8/src/projen/cdk8s/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 12:26:18.940807 projen-0.80.8/src/projen/cdktf/
--rw-r--r--   0 runner    (1001) docker     (127)   222660 2024-03-06 12:26:08.000000 projen-0.80.8/src/projen/cdktf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 12:26:18.940807 projen-0.80.8/src/projen/circleci/
--rw-r--r--   0 runner    (1001) docker     (127)    75837 2024-03-06 12:26:08.000000 projen-0.80.8/src/projen/circleci/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 12:26:18.940807 projen-0.80.8/src/projen/github/
--rw-r--r--   0 runner    (1001) docker     (127)   407540 2024-03-06 12:26:08.000000 projen-0.80.8/src/projen/github/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 12:26:18.944807 projen-0.80.8/src/projen/github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)   250661 2024-03-06 12:26:08.000000 projen-0.80.8/src/projen/github/workflows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 12:26:18.944807 projen-0.80.8/src/projen/gitlab/
--rw-r--r--   0 runner    (1001) docker     (127)   202734 2024-03-06 12:26:08.000000 projen-0.80.8/src/projen/gitlab/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 12:26:18.944807 projen-0.80.8/src/projen/java/
--rw-r--r--   0 runner    (1001) docker     (127)   183633 2024-03-06 12:26:08.000000 projen-0.80.8/src/projen/java/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 12:26:18.944807 projen-0.80.8/src/projen/javascript/
--rw-r--r--   0 runner    (1001) docker     (127)   835713 2024-03-06 12:26:08.000000 projen-0.80.8/src/projen/javascript/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 12:26:08.000000 projen-0.80.8/src/projen/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 12:26:18.944807 projen-0.80.8/src/projen/python/
--rw-r--r--   0 runner    (1001) docker     (127)   213082 2024-03-06 12:26:08.000000 projen-0.80.8/src/projen/python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 12:26:18.944807 projen-0.80.8/src/projen/release/
--rw-r--r--   0 runner    (1001) docker     (127)   280230 2024-03-06 12:26:08.000000 projen-0.80.8/src/projen/release/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 12:26:18.944807 projen-0.80.8/src/projen/typescript/
--rw-r--r--   0 runner    (1001) docker     (127)   470703 2024-03-06 12:26:08.000000 projen-0.80.8/src/projen/typescript/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 12:26:18.948807 projen-0.80.8/src/projen/vscode/
--rw-r--r--   0 runner    (1001) docker     (127)    68964 2024-03-06 12:26:08.000000 projen-0.80.8/src/projen/vscode/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 12:26:18.948807 projen-0.80.8/src/projen/web/
--rw-r--r--   0 runner    (1001) docker     (127)   790628 2024-03-06 12:26:08.000000 projen-0.80.8/src/projen/web/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 12:26:18.936807 projen-0.80.8/src/projen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    76741 2024-03-06 12:26:18.000000 projen-0.80.8/src/projen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-03-06 12:26:18.000000 projen-0.80.8/src/projen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 12:26:18.000000 projen-0.80.8/src/projen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-03-06 12:26:18.000000 projen-0.80.8/src/projen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-06 12:26:18.000000 projen-0.80.8/src/projen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 10:04:58.020989 projen-0.80.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-03-07 10:04:47.000000 projen-0.80.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-07 10:04:47.000000 projen-0.80.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    76741 2024-03-07 10:04:58.020989 projen-0.80.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    75912 2024-03-07 10:04:47.000000 projen-0.80.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-07 10:04:47.000000 projen-0.80.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-07 10:04:58.020989 projen-0.80.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-03-07 10:04:47.000000 projen-0.80.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 10:04:58.004989 projen-0.80.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 10:04:58.004989 projen-0.80.9/src/projen/
+-rw-r--r--   0 runner    (1001) docker     (127)   649146 2024-03-07 10:04:47.000000 projen-0.80.9/src/projen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 10:04:58.008989 projen-0.80.9/src/projen/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-03-07 10:04:47.000000 projen-0.80.9/src/projen/_jsii/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 10:04:58.008989 projen-0.80.9/src/projen/_jsii/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-03-07 10:04:47.000000 projen-0.80.9/src/projen/_jsii/bin/projen
+-rw-r--r--   0 runner    (1001) docker     (127)  2637531 2024-03-07 10:04:47.000000 projen-0.80.9/src/projen/_jsii/projen@0.80.9.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 10:04:58.012989 projen-0.80.9/src/projen/awscdk/
+-rw-r--r--   0 runner    (1001) docker     (127)  1074174 2024-03-07 10:04:47.000000 projen-0.80.9/src/projen/awscdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 10:04:58.012989 projen-0.80.9/src/projen/build/
+-rw-r--r--   0 runner    (1001) docker     (127)    46549 2024-03-07 10:04:47.000000 projen-0.80.9/src/projen/build/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 10:04:58.012989 projen-0.80.9/src/projen/cdk/
+-rw-r--r--   0 runner    (1001) docker     (127)   505357 2024-03-07 10:04:47.000000 projen-0.80.9/src/projen/cdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 10:04:58.012989 projen-0.80.9/src/projen/cdk8s/
+-rw-r--r--   0 runner    (1001) docker     (127)   593908 2024-03-07 10:04:47.000000 projen-0.80.9/src/projen/cdk8s/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 10:04:58.012989 projen-0.80.9/src/projen/cdktf/
+-rw-r--r--   0 runner    (1001) docker     (127)   222660 2024-03-07 10:04:47.000000 projen-0.80.9/src/projen/cdktf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 10:04:58.012989 projen-0.80.9/src/projen/circleci/
+-rw-r--r--   0 runner    (1001) docker     (127)    75837 2024-03-07 10:04:47.000000 projen-0.80.9/src/projen/circleci/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 10:04:58.012989 projen-0.80.9/src/projen/github/
+-rw-r--r--   0 runner    (1001) docker     (127)   407540 2024-03-07 10:04:47.000000 projen-0.80.9/src/projen/github/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 10:04:58.016989 projen-0.80.9/src/projen/github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)   250661 2024-03-07 10:04:47.000000 projen-0.80.9/src/projen/github/workflows/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 10:04:58.016989 projen-0.80.9/src/projen/gitlab/
+-rw-r--r--   0 runner    (1001) docker     (127)   202734 2024-03-07 10:04:47.000000 projen-0.80.9/src/projen/gitlab/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 10:04:58.016989 projen-0.80.9/src/projen/java/
+-rw-r--r--   0 runner    (1001) docker     (127)   183633 2024-03-07 10:04:47.000000 projen-0.80.9/src/projen/java/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 10:04:58.016989 projen-0.80.9/src/projen/javascript/
+-rw-r--r--   0 runner    (1001) docker     (127)   835713 2024-03-07 10:04:47.000000 projen-0.80.9/src/projen/javascript/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 10:04:47.000000 projen-0.80.9/src/projen/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 10:04:58.016989 projen-0.80.9/src/projen/python/
+-rw-r--r--   0 runner    (1001) docker     (127)   213082 2024-03-07 10:04:47.000000 projen-0.80.9/src/projen/python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 10:04:58.016989 projen-0.80.9/src/projen/release/
+-rw-r--r--   0 runner    (1001) docker     (127)   280230 2024-03-07 10:04:47.000000 projen-0.80.9/src/projen/release/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 10:04:58.016989 projen-0.80.9/src/projen/typescript/
+-rw-r--r--   0 runner    (1001) docker     (127)   470703 2024-03-07 10:04:47.000000 projen-0.80.9/src/projen/typescript/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 10:04:58.020989 projen-0.80.9/src/projen/vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)    68964 2024-03-07 10:04:47.000000 projen-0.80.9/src/projen/vscode/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 10:04:58.020989 projen-0.80.9/src/projen/web/
+-rw-r--r--   0 runner    (1001) docker     (127)   790628 2024-03-07 10:04:47.000000 projen-0.80.9/src/projen/web/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 10:04:58.008989 projen-0.80.9/src/projen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    76741 2024-03-07 10:04:57.000000 projen-0.80.9/src/projen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-03-07 10:04:57.000000 projen-0.80.9/src/projen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 10:04:57.000000 projen-0.80.9/src/projen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-03-07 10:04:57.000000 projen-0.80.9/src/projen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-07 10:04:57.000000 projen-0.80.9/src/projen.egg-info/top_level.txt
```

### Comparing `projen-0.80.8/LICENSE` & `projen-0.80.9/LICENSE`

 * *Files identical despite different names*

### Comparing `projen-0.80.8/PKG-INFO` & `projen-0.80.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: projen
-Version: 0.80.8
+Version: 0.80.9
 Summary: CDK for software projects
 Home-page: https://github.com/projen/projen.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/projen/projen.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `projen-0.80.8/README.md` & `projen-0.80.9/README.md`

 * *Files identical despite different names*

### Comparing `projen-0.80.8/setup.py` & `projen-0.80.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "projen",
-    "version": "0.80.8",
+    "version": "0.80.9",
     "description": "CDK for software projects",
     "license": "Apache-2.0",
     "url": "https://github.com/projen/projen.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -38,15 +38,15 @@
         "projen.release",
         "projen.typescript",
         "projen.vscode",
         "projen.web"
     ],
     "package_data": {
         "projen._jsii": [
-            "projen@0.80.8.jsii.tgz"
+            "projen@0.80.9.jsii.tgz"
         ],
         "projen": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `projen-0.80.8/src/projen/__init__.py` & `projen-0.80.9/src/projen/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.80.8/src/projen/awscdk/__init__.py` & `projen-0.80.9/src/projen/awscdk/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.80.8/src/projen/build/__init__.py` & `projen-0.80.9/src/projen/build/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.80.8/src/projen/cdk/__init__.py` & `projen-0.80.9/src/projen/cdk/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.80.8/src/projen/cdk8s/__init__.py` & `projen-0.80.9/src/projen/cdk8s/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.80.8/src/projen/cdktf/__init__.py` & `projen-0.80.9/src/projen/cdktf/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.80.8/src/projen/circleci/__init__.py` & `projen-0.80.9/src/projen/circleci/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.80.8/src/projen/github/__init__.py` & `projen-0.80.9/src/projen/github/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.80.8/src/projen/github/workflows/__init__.py` & `projen-0.80.9/src/projen/github/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.80.8/src/projen/gitlab/__init__.py` & `projen-0.80.9/src/projen/gitlab/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.80.8/src/projen/java/__init__.py` & `projen-0.80.9/src/projen/java/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.80.8/src/projen/javascript/__init__.py` & `projen-0.80.9/src/projen/javascript/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.80.8/src/projen/python/__init__.py` & `projen-0.80.9/src/projen/python/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.80.8/src/projen/release/__init__.py` & `projen-0.80.9/src/projen/release/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.80.8/src/projen/typescript/__init__.py` & `projen-0.80.9/src/projen/typescript/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.80.8/src/projen/vscode/__init__.py` & `projen-0.80.9/src/projen/vscode/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.80.8/src/projen/web/__init__.py` & `projen-0.80.9/src/projen/web/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.80.8/src/projen.egg-info/PKG-INFO` & `projen-0.80.9/src/projen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: projen
-Version: 0.80.8
+Version: 0.80.9
 Summary: CDK for software projects
 Home-page: https://github.com/projen/projen.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/projen/projen.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `projen-0.80.8/src/projen.egg-info/SOURCES.txt` & `projen-0.80.9/src/projen.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 src/projen/py.typed
 src/projen.egg-info/PKG-INFO
 src/projen.egg-info/SOURCES.txt
 src/projen.egg-info/dependency_links.txt
 src/projen.egg-info/requires.txt
 src/projen.egg-info/top_level.txt
 src/projen/_jsii/__init__.py
-src/projen/_jsii/projen@0.80.8.jsii.tgz
+src/projen/_jsii/projen@0.80.9.jsii.tgz
 src/projen/_jsii/bin/projen
 src/projen/awscdk/__init__.py
 src/projen/build/__init__.py
 src/projen/cdk/__init__.py
 src/projen/cdk8s/__init__.py
 src/projen/cdktf/__init__.py
 src/projen/circleci/__init__.py
```

