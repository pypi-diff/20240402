# Comparing `tmp/cdktf-cdk8s-0.9.8.tar.gz` & `tmp/cdktf-cdk8s-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdk8s-0.9.8.tar", last modified: Mon Jan  8 00:25:48 2024, max compression
+gzip compressed data, was "cdktf-cdk8s-0.9.9.tar", last modified: Thu Jan 11 04:37:25 2024, max compression
```

## Comparing `cdktf-cdk8s-0.9.8.tar` & `cdktf-cdk8s-0.9.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 00:25:48.967049 cdktf-cdk8s-0.9.8/
--rw-r--r--   0 runner    (1001) docker     (127)    16012 2024-01-08 00:25:35.000000 cdktf-cdk8s-0.9.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-01-08 00:25:35.000000 cdktf-cdk8s-0.9.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4255 2024-01-08 00:25:48.967049 cdktf-cdk8s-0.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3382 2024-01-08 00:25:35.000000 cdktf-cdk8s-0.9.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-01-08 00:25:35.000000 cdktf-cdk8s-0.9.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-08 00:25:48.967049 cdktf-cdk8s-0.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-01-08 00:25:35.000000 cdktf-cdk8s-0.9.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 00:25:48.963048 cdktf-cdk8s-0.9.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 00:25:48.967049 cdktf-cdk8s-0.9.8/src/cdktf_cdk8s/
--rw-r--r--   0 runner    (1001) docker     (127)    38396 2024-01-08 00:25:35.000000 cdktf-cdk8s-0.9.8/src/cdktf_cdk8s/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 00:25:48.967049 cdktf-cdk8s-0.9.8/src/cdktf_cdk8s/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-01-08 00:25:35.000000 cdktf-cdk8s-0.9.8/src/cdktf_cdk8s/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   123287 2024-01-08 00:25:35.000000 cdktf-cdk8s-0.9.8/src/cdktf_cdk8s/_jsii/cdktf-cdk8s@0.9.8.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-08 00:25:35.000000 cdktf-cdk8s-0.9.8/src/cdktf_cdk8s/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 00:25:48.967049 cdktf-cdk8s-0.9.8/src/cdktf_cdk8s.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4255 2024-01-08 00:25:48.000000 cdktf-cdk8s-0.9.8/src/cdktf_cdk8s.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-01-08 00:25:48.000000 cdktf-cdk8s-0.9.8/src/cdktf_cdk8s.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-08 00:25:48.000000 cdktf-cdk8s-0.9.8/src/cdktf_cdk8s.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-01-08 00:25:48.000000 cdktf-cdk8s-0.9.8/src/cdktf_cdk8s.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-01-08 00:25:48.000000 cdktf-cdk8s-0.9.8/src/cdktf_cdk8s.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 04:37:25.590644 cdktf-cdk8s-0.9.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    16012 2024-01-11 04:37:14.000000 cdktf-cdk8s-0.9.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-01-11 04:37:14.000000 cdktf-cdk8s-0.9.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4255 2024-01-11 04:37:25.590644 cdktf-cdk8s-0.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3382 2024-01-11 04:37:14.000000 cdktf-cdk8s-0.9.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-01-11 04:37:14.000000 cdktf-cdk8s-0.9.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-11 04:37:25.590644 cdktf-cdk8s-0.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-01-11 04:37:14.000000 cdktf-cdk8s-0.9.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 04:37:25.586644 cdktf-cdk8s-0.9.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 04:37:25.586644 cdktf-cdk8s-0.9.9/src/cdktf_cdk8s/
+-rw-r--r--   0 runner    (1001) docker     (127)    38396 2024-01-11 04:37:14.000000 cdktf-cdk8s-0.9.9/src/cdktf_cdk8s/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 04:37:25.590644 cdktf-cdk8s-0.9.9/src/cdktf_cdk8s/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-01-11 04:37:14.000000 cdktf-cdk8s-0.9.9/src/cdktf_cdk8s/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   123284 2024-01-11 04:37:14.000000 cdktf-cdk8s-0.9.9/src/cdktf_cdk8s/_jsii/cdktf-cdk8s@0.9.9.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-11 04:37:14.000000 cdktf-cdk8s-0.9.9/src/cdktf_cdk8s/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 04:37:25.586644 cdktf-cdk8s-0.9.9/src/cdktf_cdk8s.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4255 2024-01-11 04:37:25.000000 cdktf-cdk8s-0.9.9/src/cdktf_cdk8s.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-01-11 04:37:25.000000 cdktf-cdk8s-0.9.9/src/cdktf_cdk8s.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-11 04:37:25.000000 cdktf-cdk8s-0.9.9/src/cdktf_cdk8s.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-01-11 04:37:25.000000 cdktf-cdk8s-0.9.9/src/cdktf_cdk8s.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-01-11 04:37:25.000000 cdktf-cdk8s-0.9.9/src/cdktf_cdk8s.egg-info/top_level.txt
```

### Comparing `cdktf-cdk8s-0.9.8/LICENSE` & `cdktf-cdk8s-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdk8s-0.9.8/PKG-INFO` & `cdktf-cdk8s-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdk8s
-Version: 0.9.8
+Version: 0.9.9
 Summary: A compatibility layer for using cdk8s constructs within Terraform CDK.
 Home-page: https://github.com/cdktf/cdktf-cdk8s.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-cdk8s.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdk8s-0.9.8/README.md` & `cdktf-cdk8s-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `cdktf-cdk8s-0.9.8/setup.py` & `cdktf-cdk8s-0.9.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdk8s",
-    "version": "0.9.8",
+    "version": "0.9.9",
     "description": "A compatibility layer for using cdk8s constructs within Terraform CDK.",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-cdk8s.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdktf_cdk8s",
         "cdktf_cdk8s._jsii"
     ],
     "package_data": {
         "cdktf_cdk8s._jsii": [
-            "cdktf-cdk8s@0.9.8.jsii.tgz"
+            "cdktf-cdk8s@0.9.9.jsii.tgz"
         ],
         "cdktf_cdk8s": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `cdktf-cdk8s-0.9.8/src/cdktf_cdk8s/__init__.py` & `cdktf-cdk8s-0.9.9/src/cdktf_cdk8s/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdk8s-0.9.8/src/cdktf_cdk8s.egg-info/PKG-INFO` & `cdktf-cdk8s-0.9.9/src/cdktf_cdk8s.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdk8s
-Version: 0.9.8
+Version: 0.9.9
 Summary: A compatibility layer for using cdk8s constructs within Terraform CDK.
 Home-page: https://github.com/cdktf/cdktf-cdk8s.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-cdk8s.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

