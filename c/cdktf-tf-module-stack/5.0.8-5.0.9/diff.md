# Comparing `tmp/cdktf-tf-module-stack-5.0.8.tar.gz` & `tmp/cdktf-tf-module-stack-5.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-tf-module-stack-5.0.8.tar", last modified: Mon Mar  4 00:14:37 2024, max compression
+gzip compressed data, was "cdktf-tf-module-stack-5.0.9.tar", last modified: Wed Mar 13 13:21:50 2024, max compression
```

## Comparing `cdktf-tf-module-stack-5.0.8.tar` & `cdktf-tf-module-stack-5.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 00:14:37.244776 cdktf-tf-module-stack-5.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)    16012 2024-03-04 00:14:24.000000 cdktf-tf-module-stack-5.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-04 00:14:24.000000 cdktf-tf-module-stack-5.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6487 2024-03-04 00:14:37.244776 cdktf-tf-module-stack-5.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-03-04 00:14:24.000000 cdktf-tf-module-stack-5.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-04 00:14:24.000000 cdktf-tf-module-stack-5.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-04 00:14:37.244776 cdktf-tf-module-stack-5.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-03-04 00:14:24.000000 cdktf-tf-module-stack-5.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 00:14:37.244776 cdktf-tf-module-stack-5.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 00:14:37.244776 cdktf-tf-module-stack-5.0.8/src/cdktf_tf_module_stack/
--rw-r--r--   0 runner    (1001) docker     (127)    16854 2024-03-04 00:14:24.000000 cdktf-tf-module-stack-5.0.8/src/cdktf_tf_module_stack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 00:14:37.244776 cdktf-tf-module-stack-5.0.8/src/cdktf_tf_module_stack/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-03-04 00:14:24.000000 cdktf-tf-module-stack-5.0.8/src/cdktf_tf_module_stack/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38789 2024-03-04 00:14:24.000000 cdktf-tf-module-stack-5.0.8/src/cdktf_tf_module_stack/_jsii/tf-module-stack@5.0.8.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 00:14:24.000000 cdktf-tf-module-stack-5.0.8/src/cdktf_tf_module_stack/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 00:14:37.244776 cdktf-tf-module-stack-5.0.8/src/cdktf_tf_module_stack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6487 2024-03-04 00:14:37.000000 cdktf-tf-module-stack-5.0.8/src/cdktf_tf_module_stack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-03-04 00:14:37.000000 cdktf-tf-module-stack-5.0.8/src/cdktf_tf_module_stack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 00:14:37.000000 cdktf-tf-module-stack-5.0.8/src/cdktf_tf_module_stack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-04 00:14:37.000000 cdktf-tf-module-stack-5.0.8/src/cdktf_tf_module_stack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-04 00:14:37.000000 cdktf-tf-module-stack-5.0.8/src/cdktf_tf_module_stack.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 13:21:50.219776 cdktf-tf-module-stack-5.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    16012 2024-03-13 13:21:34.000000 cdktf-tf-module-stack-5.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-13 13:21:34.000000 cdktf-tf-module-stack-5.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6487 2024-03-13 13:21:50.215777 cdktf-tf-module-stack-5.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-03-13 13:21:34.000000 cdktf-tf-module-stack-5.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-13 13:21:34.000000 cdktf-tf-module-stack-5.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-13 13:21:50.219776 cdktf-tf-module-stack-5.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-03-13 13:21:34.000000 cdktf-tf-module-stack-5.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 13:21:50.215777 cdktf-tf-module-stack-5.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 13:21:50.215777 cdktf-tf-module-stack-5.0.9/src/cdktf_tf_module_stack/
+-rw-r--r--   0 runner    (1001) docker     (127)    16854 2024-03-13 13:21:34.000000 cdktf-tf-module-stack-5.0.9/src/cdktf_tf_module_stack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 13:21:50.215777 cdktf-tf-module-stack-5.0.9/src/cdktf_tf_module_stack/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-03-13 13:21:34.000000 cdktf-tf-module-stack-5.0.9/src/cdktf_tf_module_stack/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38789 2024-03-13 13:21:34.000000 cdktf-tf-module-stack-5.0.9/src/cdktf_tf_module_stack/_jsii/tf-module-stack@5.0.9.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 13:21:34.000000 cdktf-tf-module-stack-5.0.9/src/cdktf_tf_module_stack/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 13:21:50.215777 cdktf-tf-module-stack-5.0.9/src/cdktf_tf_module_stack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6487 2024-03-13 13:21:50.000000 cdktf-tf-module-stack-5.0.9/src/cdktf_tf_module_stack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-03-13 13:21:50.000000 cdktf-tf-module-stack-5.0.9/src/cdktf_tf_module_stack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 13:21:50.000000 cdktf-tf-module-stack-5.0.9/src/cdktf_tf_module_stack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-13 13:21:50.000000 cdktf-tf-module-stack-5.0.9/src/cdktf_tf_module_stack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-13 13:21:50.000000 cdktf-tf-module-stack-5.0.9/src/cdktf_tf_module_stack.egg-info/top_level.txt
```

### Comparing `cdktf-tf-module-stack-5.0.8/LICENSE` & `cdktf-tf-module-stack-5.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-tf-module-stack-5.0.8/PKG-INFO` & `cdktf-tf-module-stack-5.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-tf-module-stack
-Version: 5.0.8
+Version: 5.0.9
 Summary: A drop-in replacement for cdktf.TerraformStack that lets you define Terraform modules as constructs
 Home-page: https://github.com/cdktf/cdktf-tf-module-stack.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-tf-module-stack.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-tf-module-stack-5.0.8/README.md` & `cdktf-tf-module-stack-5.0.9/README.md`

 * *Files identical despite different names*

### Comparing `cdktf-tf-module-stack-5.0.8/setup.py` & `cdktf-tf-module-stack-5.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-tf-module-stack",
-    "version": "5.0.8",
+    "version": "5.0.9",
     "description": "A drop-in replacement for cdktf.TerraformStack that lets you define Terraform modules as constructs",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-tf-module-stack.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdktf_tf_module_stack",
         "cdktf_tf_module_stack._jsii"
     ],
     "package_data": {
         "cdktf_tf_module_stack._jsii": [
-            "tf-module-stack@5.0.8.jsii.tgz"
+            "tf-module-stack@5.0.9.jsii.tgz"
         ],
         "cdktf_tf_module_stack": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `cdktf-tf-module-stack-5.0.8/src/cdktf_tf_module_stack/__init__.py` & `cdktf-tf-module-stack-5.0.9/src/cdktf_tf_module_stack/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-tf-module-stack-5.0.8/src/cdktf_tf_module_stack.egg-info/PKG-INFO` & `cdktf-tf-module-stack-5.0.9/src/cdktf_tf_module_stack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-tf-module-stack
-Version: 5.0.8
+Version: 5.0.9
 Summary: A drop-in replacement for cdktf.TerraformStack that lets you define Terraform modules as constructs
 Home-page: https://github.com/cdktf/cdktf-tf-module-stack.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-tf-module-stack.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

