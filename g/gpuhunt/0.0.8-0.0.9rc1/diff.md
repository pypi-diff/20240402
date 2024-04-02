# Comparing `tmp/gpuhunt-0.0.8.tar.gz` & `tmp/gpuhunt-0.0.9rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpuhunt-0.0.8.tar", last modified: Fri Mar 15 13:59:48 2024, max compression
+gzip compressed data, was "gpuhunt-0.0.9rc1.tar", last modified: Tue Apr  2 12:11:40 2024, max compression
```

## Comparing `gpuhunt-0.0.8.tar` & `gpuhunt-0.0.9rc1.tar`

### file list

```diff
@@ -1,58 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 13:59:48.274278 gpuhunt-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)    15976 2024-03-15 13:59:37.000000 gpuhunt-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3484 2024-03-15 13:59:48.274278 gpuhunt-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-03-15 13:59:37.000000 gpuhunt-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-03-15 13:59:37.000000 gpuhunt-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-15 13:59:48.274278 gpuhunt-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 13:59:48.266278 gpuhunt-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 13:59:48.266278 gpuhunt-0.0.8/src/gpuhunt/
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-03-15 13:59:37.000000 gpuhunt-0.0.8/src/gpuhunt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-03-15 13:59:37.000000 gpuhunt-0.0.8/src/gpuhunt/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 13:59:48.270278 gpuhunt-0.0.8/src/gpuhunt/_internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 13:59:37.000000 gpuhunt-0.0.8/src/gpuhunt/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9214 2024-03-15 13:59:37.000000 gpuhunt-0.0.8/src/gpuhunt/_internal/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-03-15 13:59:37.000000 gpuhunt-0.0.8/src/gpuhunt/_internal/constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-03-15 13:59:37.000000 gpuhunt-0.0.8/src/gpuhunt/_internal/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-03-15 13:59:37.000000 gpuhunt-0.0.8/src/gpuhunt/_internal/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-03-15 13:59:37.000000 gpuhunt-0.0.8/src/gpuhunt/_internal/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-03-15 13:59:37.000000 gpuhunt-0.0.8/src/gpuhunt/_internal/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 13:59:48.270278 gpuhunt-0.0.8/src/gpuhunt/providers/
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-03-15 13:59:37.000000 gpuhunt-0.0.8/src/gpuhunt/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8194 2024-03-15 13:59:37.000000 gpuhunt-0.0.8/src/gpuhunt/providers/aws.py
--rw-r--r--   0 runner    (1001) docker     (127)    10015 2024-03-15 13:59:37.000000 gpuhunt-0.0.8/src/gpuhunt/providers/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)    13592 2024-03-15 13:59:37.000000 gpuhunt-0.0.8/src/gpuhunt/providers/cudo.py
--rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-03-15 13:59:37.000000 gpuhunt-0.0.8/src/gpuhunt/providers/datacrunch.py
--rw-r--r--   0 runner    (1001) docker     (127)     9430 2024-03-15 13:59:37.000000 gpuhunt-0.0.8/src/gpuhunt/providers/gcp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-03-15 13:59:37.000000 gpuhunt-0.0.8/src/gpuhunt/providers/lambdalabs.py
--rw-r--r--   0 runner    (1001) docker     (127)    11796 2024-03-15 13:59:37.000000 gpuhunt-0.0.8/src/gpuhunt/providers/nebius.py
--rw-r--r--   0 runner    (1001) docker     (127)     9566 2024-03-15 13:59:37.000000 gpuhunt-0.0.8/src/gpuhunt/providers/tensordock.py
--rw-r--r--   0 runner    (1001) docker     (127)     6169 2024-03-15 13:59:37.000000 gpuhunt-0.0.8/src/gpuhunt/providers/vastai.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-15 13:59:46.000000 gpuhunt-0.0.8/src/gpuhunt/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 13:59:48.274278 gpuhunt-0.0.8/src/gpuhunt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3484 2024-03-15 13:59:48.000000 gpuhunt-0.0.8/src/gpuhunt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-03-15 13:59:48.000000 gpuhunt-0.0.8/src/gpuhunt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 13:59:48.000000 gpuhunt-0.0.8/src/gpuhunt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-03-15 13:59:48.000000 gpuhunt-0.0.8/src/gpuhunt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-15 13:59:48.000000 gpuhunt-0.0.8/src/gpuhunt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 13:59:48.270278 gpuhunt-0.0.8/src/integrity_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 13:59:37.000000 gpuhunt-0.0.8/src/integrity_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-15 13:59:37.000000 gpuhunt-0.0.8/src/integrity_tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-03-15 13:59:37.000000 gpuhunt-0.0.8/src/integrity_tests/test_all.py
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-03-15 13:59:37.000000 gpuhunt-0.0.8/src/integrity_tests/test_aws.py
--rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-03-15 13:59:37.000000 gpuhunt-0.0.8/src/integrity_tests/test_azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-03-15 13:59:37.000000 gpuhunt-0.0.8/src/integrity_tests/test_datacrunch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-03-15 13:59:37.000000 gpuhunt-0.0.8/src/integrity_tests/test_gcp.py
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-03-15 13:59:37.000000 gpuhunt-0.0.8/src/integrity_tests/test_nebius.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 13:59:48.270278 gpuhunt-0.0.8/src/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 13:59:37.000000 gpuhunt-0.0.8/src/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 13:59:48.274278 gpuhunt-0.0.8/src/tests/_internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 13:59:37.000000 gpuhunt-0.0.8/src/tests/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-03-15 13:59:37.000000 gpuhunt-0.0.8/src/tests/_internal/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-03-15 13:59:37.000000 gpuhunt-0.0.8/src/tests/_internal/test_constraints.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 13:59:48.274278 gpuhunt-0.0.8/src/tests/providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 13:59:37.000000 gpuhunt-0.0.8/src/tests/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7243 2024-03-15 13:59:37.000000 gpuhunt-0.0.8/src/tests/providers/test_cudo.py
--rw-r--r--   0 runner    (1001) docker     (127)    11443 2024-03-15 13:59:37.000000 gpuhunt-0.0.8/src/tests/providers/test_datacrunch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-03-15 13:59:37.000000 gpuhunt-0.0.8/src/tests/providers/test_providers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-03-15 13:59:37.000000 gpuhunt-0.0.8/src/tests/providers/test_tensordock.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-03-15 13:59:37.000000 gpuhunt-0.0.8/src/tests/providers/test_vastai.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:11:40.413836 gpuhunt-0.0.9rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)    15976 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-02 12:11:40.413836 gpuhunt-0.0.9rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 12:11:40.413836 gpuhunt-0.0.9rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:11:40.401836 gpuhunt-0.0.9rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:11:40.401836 gpuhunt-0.0.9rc1/src/gpuhunt/
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/gpuhunt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/gpuhunt/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:11:40.405836 gpuhunt-0.0.9rc1/src/gpuhunt/_internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/gpuhunt/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9224 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/gpuhunt/_internal/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/gpuhunt/_internal/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/gpuhunt/_internal/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/gpuhunt/_internal/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/gpuhunt/_internal/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/gpuhunt/_internal/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:11:40.405836 gpuhunt-0.0.9rc1/src/gpuhunt/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/gpuhunt/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8194 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/gpuhunt/providers/aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10015 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/gpuhunt/providers/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13592 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/gpuhunt/providers/cudo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/gpuhunt/providers/datacrunch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9430 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/gpuhunt/providers/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/gpuhunt/providers/lambdalabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11796 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/gpuhunt/providers/nebius.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8306 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/gpuhunt/providers/runpod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9566 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/gpuhunt/providers/tensordock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6169 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/gpuhunt/providers/vastai.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-02 12:11:37.000000 gpuhunt-0.0.9rc1/src/gpuhunt/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:11:40.409836 gpuhunt-0.0.9rc1/src/gpuhunt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-02 12:11:40.000000 gpuhunt-0.0.9rc1/src/gpuhunt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-02 12:11:40.000000 gpuhunt-0.0.9rc1/src/gpuhunt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 12:11:40.000000 gpuhunt-0.0.9rc1/src/gpuhunt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-02 12:11:40.000000 gpuhunt-0.0.9rc1/src/gpuhunt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-02 12:11:40.000000 gpuhunt-0.0.9rc1/src/gpuhunt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:11:40.409836 gpuhunt-0.0.9rc1/src/integrity_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/integrity_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/integrity_tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/integrity_tests/test_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/integrity_tests/test_aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/integrity_tests/test_azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/integrity_tests/test_datacrunch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/integrity_tests/test_gcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/integrity_tests/test_nebius.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/integrity_tests/test_runpod.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:11:40.409836 gpuhunt-0.0.9rc1/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:11:40.409836 gpuhunt-0.0.9rc1/src/tests/_internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/tests/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/tests/_internal/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/tests/_internal/test_constraints.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:11:40.409836 gpuhunt-0.0.9rc1/src/tests/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/tests/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7243 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/tests/providers/test_cudo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11443 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/tests/providers/test_datacrunch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/tests/providers/test_providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/tests/providers/test_tensordock.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-02 12:11:15.000000 gpuhunt-0.0.9rc1/src/tests/providers/test_vastai.py
```

### Comparing `gpuhunt-0.0.8/LICENSE` & `gpuhunt-0.0.9rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.8/PKG-INFO` & `gpuhunt-0.0.9rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpuhunt
-Version: 0.0.8
+Version: 0.0.9rc1
 Summary: A catalog of GPU pricing for different cloud providers
 Author: dstack GmbH
 Project-URL: GitHub, https://github.com/dstackai/gpuhunt
 Project-URL: Issues, https://github.com/dstackai/gpuhunt/issues
 Keywords: gpu,cloud,pricing
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
@@ -81,15 +81,15 @@
 
 ## Advanced usage
 
 ```python
 from gpuhunt import Catalog
 
 catalog = Catalog()
-catalog.load(version="20240310")
+catalog.load(version="20240402")
 items = catalog.query()
 
 print(*items, sep="\n")
 ```
 
 ## Supported providers
```

### Comparing `gpuhunt-0.0.8/README.md` & `gpuhunt-0.0.9rc1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 ## Advanced usage
 
 ```python
 from gpuhunt import Catalog
 
 catalog = Catalog()
-catalog.load(version="20240310")
+catalog.load(version="20240402")
 items = catalog.query()
 
 print(*items, sep="\n")
 ```
 
 ## Supported providers
```

### Comparing `gpuhunt-0.0.8/pyproject.toml` & `gpuhunt-0.0.9rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.8/src/gpuhunt/__main__.py` & `gpuhunt-0.0.9rc1/src/gpuhunt/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
             "aws",
             "azure",
             "cudo",
             "datacrunch",
             "gcp",
             "lambdalabs",
             "nebius",
+            "runpod",
             "tensordock",
             "vastai",
         ],
     )
     parser.add_argument("--output", required=True)
     parser.add_argument("--no-filter", action="store_true")
     args = parser.parse_args()
@@ -54,14 +55,18 @@
         from gpuhunt.providers.lambdalabs import LambdaLabsProvider
 
         provider = LambdaLabsProvider(os.getenv("LAMBDALABS_TOKEN"))
     elif args.provider == "nebius":
         from gpuhunt.providers.nebius import NebiusProvider
 
         provider = NebiusProvider(json.loads(os.getenv("NEBIUS_SERVICE_ACCOUNT")))
+    elif args.provider == "runpod":
+        from gpuhunt.providers.runpod import RunpodProvider
+
+        provider = RunpodProvider()
     elif args.provider == "tensordock":
         from gpuhunt.providers.tensordock import TensorDockProvider
 
         provider = TensorDockProvider()
     elif args.provider == "vastai":
         from gpuhunt.providers.vastai import VastAIProvider
```

### Comparing `gpuhunt-0.0.8/src/gpuhunt/_internal/catalog.py` & `gpuhunt-0.0.9rc1/src/gpuhunt/_internal/catalog.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from gpuhunt._internal.models import CatalogItem, QueryFilter
 from gpuhunt._internal.utils import parse_compute_capability
 from gpuhunt.providers import AbstractProvider
 
 logger = logging.getLogger(__name__)
 version_url = "https://dstack-gpu-pricing.s3.eu-west-1.amazonaws.com/v1/version"
 catalog_url = "https://dstack-gpu-pricing.s3.eu-west-1.amazonaws.com/v1/{version}/catalog.zip"
-OFFLINE_PROVIDERS = ["aws", "azure", "datacrunch", "gcp", "lambdalabs", "nebius"]
+OFFLINE_PROVIDERS = ["aws", "azure", "datacrunch", "gcp", "lambdalabs", "nebius", "runpod"]
 ONLINE_PROVIDERS = ["cudo", "tensordock", "vastai"]
 RELOAD_INTERVAL = 4 * 60 * 60  # 4 hours
 
 
 class Catalog:
     def __init__(self, balance_resources: bool = True, auto_reload: bool = True):
         """
```

### Comparing `gpuhunt-0.0.8/src/gpuhunt/_internal/constraints.py` & `gpuhunt-0.0.9rc1/src/gpuhunt/_internal/constraints.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.8/src/gpuhunt/_internal/default.py` & `gpuhunt-0.0.9rc1/src/gpuhunt/_internal/default.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.8/src/gpuhunt/_internal/models.py` & `gpuhunt-0.0.9rc1/src/gpuhunt/_internal/models.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.8/src/gpuhunt/_internal/storage.py` & `gpuhunt-0.0.9rc1/src/gpuhunt/_internal/storage.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.8/src/gpuhunt/providers/aws.py` & `gpuhunt-0.0.9rc1/src/gpuhunt/providers/aws.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.8/src/gpuhunt/providers/azure.py` & `gpuhunt-0.0.9rc1/src/gpuhunt/providers/azure.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.8/src/gpuhunt/providers/cudo.py` & `gpuhunt-0.0.9rc1/src/gpuhunt/providers/cudo.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.8/src/gpuhunt/providers/datacrunch.py` & `gpuhunt-0.0.9rc1/src/gpuhunt/providers/datacrunch.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.8/src/gpuhunt/providers/gcp.py` & `gpuhunt-0.0.9rc1/src/gpuhunt/providers/gcp.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.8/src/gpuhunt/providers/lambdalabs.py` & `gpuhunt-0.0.9rc1/src/gpuhunt/providers/lambdalabs.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.8/src/gpuhunt/providers/nebius.py` & `gpuhunt-0.0.9rc1/src/gpuhunt/providers/nebius.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.8/src/gpuhunt/providers/tensordock.py` & `gpuhunt-0.0.9rc1/src/gpuhunt/providers/tensordock.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.8/src/gpuhunt/providers/vastai.py` & `gpuhunt-0.0.9rc1/src/gpuhunt/providers/vastai.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.8/src/gpuhunt.egg-info/PKG-INFO` & `gpuhunt-0.0.9rc1/src/gpuhunt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpuhunt
-Version: 0.0.8
+Version: 0.0.9rc1
 Summary: A catalog of GPU pricing for different cloud providers
 Author: dstack GmbH
 Project-URL: GitHub, https://github.com/dstackai/gpuhunt
 Project-URL: Issues, https://github.com/dstackai/gpuhunt/issues
 Keywords: gpu,cloud,pricing
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
@@ -81,15 +81,15 @@
 
 ## Advanced usage
 
 ```python
 from gpuhunt import Catalog
 
 catalog = Catalog()
-catalog.load(version="20240310")
+catalog.load(version="20240402")
 items = catalog.query()
 
 print(*items, sep="\n")
 ```
 
 ## Supported providers
```

### Comparing `gpuhunt-0.0.8/src/gpuhunt.egg-info/SOURCES.txt` & `gpuhunt-0.0.9rc1/src/gpuhunt.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -20,24 +20,26 @@
 src/gpuhunt/providers/aws.py
 src/gpuhunt/providers/azure.py
 src/gpuhunt/providers/cudo.py
 src/gpuhunt/providers/datacrunch.py
 src/gpuhunt/providers/gcp.py
 src/gpuhunt/providers/lambdalabs.py
 src/gpuhunt/providers/nebius.py
+src/gpuhunt/providers/runpod.py
 src/gpuhunt/providers/tensordock.py
 src/gpuhunt/providers/vastai.py
 src/integrity_tests/__init__.py
 src/integrity_tests/conftest.py
 src/integrity_tests/test_all.py
 src/integrity_tests/test_aws.py
 src/integrity_tests/test_azure.py
 src/integrity_tests/test_datacrunch.py
 src/integrity_tests/test_gcp.py
 src/integrity_tests/test_nebius.py
+src/integrity_tests/test_runpod.py
 src/tests/__init__.py
 src/tests/_internal/__init__.py
 src/tests/_internal/test_catalog.py
 src/tests/_internal/test_constraints.py
 src/tests/providers/__init__.py
 src/tests/providers/test_cudo.py
 src/tests/providers/test_datacrunch.py
```

### Comparing `gpuhunt-0.0.8/src/integrity_tests/test_aws.py` & `gpuhunt-0.0.9rc1/src/integrity_tests/test_aws.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.8/src/integrity_tests/test_azure.py` & `gpuhunt-0.0.9rc1/src/integrity_tests/test_azure.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.8/src/integrity_tests/test_datacrunch.py` & `gpuhunt-0.0.9rc1/src/integrity_tests/test_datacrunch.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.8/src/integrity_tests/test_gcp.py` & `gpuhunt-0.0.9rc1/src/integrity_tests/test_gcp.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.8/src/integrity_tests/test_nebius.py` & `gpuhunt-0.0.9rc1/src/integrity_tests/test_nebius.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.8/src/tests/_internal/test_catalog.py` & `gpuhunt-0.0.9rc1/src/tests/_internal/test_catalog.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.8/src/tests/_internal/test_constraints.py` & `gpuhunt-0.0.9rc1/src/tests/_internal/test_constraints.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.8/src/tests/providers/test_cudo.py` & `gpuhunt-0.0.9rc1/src/tests/providers/test_cudo.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.8/src/tests/providers/test_datacrunch.py` & `gpuhunt-0.0.9rc1/src/tests/providers/test_datacrunch.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.8/src/tests/providers/test_providers.py` & `gpuhunt-0.0.9rc1/src/tests/providers/test_providers.py`

 * *Files identical despite different names*

### Comparing `gpuhunt-0.0.8/src/tests/providers/test_tensordock.py` & `gpuhunt-0.0.9rc1/src/tests/providers/test_tensordock.py`

 * *Files identical despite different names*

