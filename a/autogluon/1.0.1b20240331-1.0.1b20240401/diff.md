# Comparing `tmp/autogluon-1.0.1b20240331.tar.gz` & `tmp/autogluon-1.0.1b20240401.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon-1.0.1b20240331.tar", last modified: Sun Mar 31 09:05:38 2024, max compression
+gzip compressed data, was "autogluon-1.0.1b20240401.tar", last modified: Mon Apr  1 09:05:28 2024, max compression
```

## Comparing `autogluon-1.0.1b20240331.tar` & `autogluon-1.0.1b20240401.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 09:05:38.150693 autogluon-1.0.1b20240331/
--rw-r--r--   0 runner    (1001) docker     (127)    11743 2024-03-31 09:05:38.150693 autogluon-1.0.1b20240331/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 09:05:38.150693 autogluon-1.0.1b20240331/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-03-31 09:04:04.000000 autogluon-1.0.1b20240331/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 09:05:38.150693 autogluon-1.0.1b20240331/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 09:05:38.150693 autogluon-1.0.1b20240331/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 09:05:38.150693 autogluon-1.0.1b20240331/src/autogluon/_internal_/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 09:04:04.000000 autogluon-1.0.1b20240331/src/autogluon/_internal_/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 09:05:38.150693 autogluon-1.0.1b20240331/src/autogluon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11743 2024-03-31 09:05:38.000000 autogluon-1.0.1b20240331/src/autogluon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-03-31 09:05:38.000000 autogluon-1.0.1b20240331/src/autogluon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 09:05:38.000000 autogluon-1.0.1b20240331/src/autogluon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-31 09:05:38.000000 autogluon-1.0.1b20240331/src/autogluon.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-03-31 09:05:38.000000 autogluon-1.0.1b20240331/src/autogluon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-31 09:05:38.000000 autogluon-1.0.1b20240331/src/autogluon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 09:05:38.000000 autogluon-1.0.1b20240331/src/autogluon.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:05:27.996476 autogluon-1.0.1b20240401/
+-rw-r--r--   0 runner    (1001) docker     (127)    11743 2024-04-01 09:05:27.996476 autogluon-1.0.1b20240401/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 09:05:27.996476 autogluon-1.0.1b20240401/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-01 09:03:49.000000 autogluon-1.0.1b20240401/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:05:27.996476 autogluon-1.0.1b20240401/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:05:27.996476 autogluon-1.0.1b20240401/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:05:27.996476 autogluon-1.0.1b20240401/src/autogluon/_internal_/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 09:03:49.000000 autogluon-1.0.1b20240401/src/autogluon/_internal_/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 09:05:27.996476 autogluon-1.0.1b20240401/src/autogluon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11743 2024-04-01 09:05:27.000000 autogluon-1.0.1b20240401/src/autogluon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-01 09:05:27.000000 autogluon-1.0.1b20240401/src/autogluon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 09:05:27.000000 autogluon-1.0.1b20240401/src/autogluon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-01 09:05:27.000000 autogluon-1.0.1b20240401/src/autogluon.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-01 09:05:27.000000 autogluon-1.0.1b20240401/src/autogluon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-01 09:05:27.000000 autogluon-1.0.1b20240401/src/autogluon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 09:05:27.000000 autogluon-1.0.1b20240401/src/autogluon.egg-info/zip-safe
```

### Comparing `autogluon-1.0.1b20240331/PKG-INFO` & `autogluon-1.0.1b20240401/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon
-Version: 1.0.1b20240331
+Version: 1.0.1b20240401
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon-1.0.1b20240331/setup.py` & `autogluon-1.0.1b20240401/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon-1.0.1b20240331/src/autogluon.egg-info/PKG-INFO` & `autogluon-1.0.1b20240401/src/autogluon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon
-Version: 1.0.1b20240331
+Version: 1.0.1b20240401
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

