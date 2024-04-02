# Comparing `tmp/cvat-cli-2.9.1.tar.gz` & `tmp/cvat-cli-2.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvat-cli-2.9.1.tar", last modified: Mon Nov 27 13:51:32 2023, max compression
+gzip compressed data, was "cvat-cli-2.9.2.tar", last modified: Mon Dec 11 18:26:42 2023, max compression
```

## Comparing `cvat-cli-2.9.1.tar` & `cvat-cli-2.9.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 13:51:32.179599 cvat-cli-2.9.1/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2023-11-27 13:51:00.000000 cvat-cli-2.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2420 2023-11-27 13:51:32.179599 cvat-cli-2.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2023-11-27 13:51:00.000000 cvat-cli-2.9.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      383 2023-11-27 13:51:00.000000 cvat-cli-2.9.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 13:51:32.175599 cvat-cli-2.9.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2023-11-27 13:51:00.000000 cvat-cli-2.9.1/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-27 13:51:32.179599 cvat-cli-2.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2023-11-27 13:51:00.000000 cvat-cli-2.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 13:51:32.175599 cvat-cli-2.9.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 13:51:32.175599 cvat-cli-2.9.1/src/cvat_cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 13:51:00.000000 cvat-cli-2.9.1/src/cvat_cli/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2279 2023-11-27 13:51:00.000000 cvat-cli-2.9.1/src/cvat_cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6052 2023-11-27 13:51:00.000000 cvat-cli-2.9.1/src/cvat_cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    15540 2023-11-27 13:51:00.000000 cvat-cli-2.9.1/src/cvat_cli/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-11-27 13:51:00.000000 cvat-cli-2.9.1/src/cvat_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 13:51:32.179599 cvat-cli-2.9.1/src/cvat_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2420 2023-11-27 13:51:32.000000 cvat-cli-2.9.1/src/cvat_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      402 2023-11-27 13:51:32.000000 cvat-cli-2.9.1/src/cvat_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-27 13:51:32.000000 cvat-cli-2.9.1/src/cvat_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2023-11-27 13:51:32.000000 cvat-cli-2.9.1/src/cvat_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2023-11-27 13:51:32.000000 cvat-cli-2.9.1/src/cvat_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-11-27 13:51:32.000000 cvat-cli-2.9.1/src/cvat_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 18:26:42.135757 cvat-cli-2.9.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2023-12-11 18:26:10.000000 cvat-cli-2.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2420 2023-12-11 18:26:42.135757 cvat-cli-2.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2023-12-11 18:26:10.000000 cvat-cli-2.9.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2023-12-11 18:26:10.000000 cvat-cli-2.9.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 18:26:42.131756 cvat-cli-2.9.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2023-12-11 18:26:10.000000 cvat-cli-2.9.2/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-11 18:26:42.135757 cvat-cli-2.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2023-12-11 18:26:10.000000 cvat-cli-2.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 18:26:42.131756 cvat-cli-2.9.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 18:26:42.131756 cvat-cli-2.9.2/src/cvat_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-11 18:26:10.000000 cvat-cli-2.9.2/src/cvat_cli/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2279 2023-12-11 18:26:10.000000 cvat-cli-2.9.2/src/cvat_cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6052 2023-12-11 18:26:10.000000 cvat-cli-2.9.2/src/cvat_cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15540 2023-12-11 18:26:10.000000 cvat-cli-2.9.2/src/cvat_cli/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2023-12-11 18:26:10.000000 cvat-cli-2.9.2/src/cvat_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 18:26:42.131756 cvat-cli-2.9.2/src/cvat_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2420 2023-12-11 18:26:42.000000 cvat-cli-2.9.2/src/cvat_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2023-12-11 18:26:42.000000 cvat-cli-2.9.2/src/cvat_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-11 18:26:42.000000 cvat-cli-2.9.2/src/cvat_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2023-12-11 18:26:42.000000 cvat-cli-2.9.2/src/cvat_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2023-12-11 18:26:42.000000 cvat-cli-2.9.2/src/cvat_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-11 18:26:42.000000 cvat-cli-2.9.2/src/cvat_cli.egg-info/top_level.txt
```

### Comparing `cvat-cli-2.9.1/PKG-INFO` & `cvat-cli-2.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: cvat-cli
-Version: 2.9.1
+Version: 2.9.2
 Summary: Command-line client for CVAT
 Home-page: https://github.com/cvat-ai/cvat/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: cvat-sdk~=2.9.1
+Requires-Dist: cvat-sdk~=2.9.2
 Requires-Dist: Pillow>=10.0.1
 Requires-Dist: setuptools>=65.5.1
 
 # Command-line client for CVAT
 
 A simple command line interface for working with CVAT tasks. At the moment it
 implements a basic feature set but may serve as the starting point for a more
```

### Comparing `cvat-cli-2.9.1/README.md` & `cvat-cli-2.9.2/README.md`

 * *Files identical despite different names*

### Comparing `cvat-cli-2.9.1/setup.py` & `cvat-cli-2.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `cvat-cli-2.9.1/src/cvat_cli/__main__.py` & `cvat-cli-2.9.2/src/cvat_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `cvat-cli-2.9.1/src/cvat_cli/cli.py` & `cvat-cli-2.9.2/src/cvat_cli/cli.py`

 * *Files identical despite different names*

### Comparing `cvat-cli-2.9.1/src/cvat_cli/parser.py` & `cvat-cli-2.9.2/src/cvat_cli/parser.py`

 * *Files identical despite different names*

### Comparing `cvat-cli-2.9.1/src/cvat_cli.egg-info/PKG-INFO` & `cvat-cli-2.9.2/src/cvat_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: cvat-cli
-Version: 2.9.1
+Version: 2.9.2
 Summary: Command-line client for CVAT
 Home-page: https://github.com/cvat-ai/cvat/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: cvat-sdk~=2.9.1
+Requires-Dist: cvat-sdk~=2.9.2
 Requires-Dist: Pillow>=10.0.1
 Requires-Dist: setuptools>=65.5.1
 
 # Command-line client for CVAT
 
 A simple command line interface for working with CVAT tasks. At the moment it
 implements a basic feature set but may serve as the starting point for a more
```

