# Comparing `tmp/harreveltools-0.0.3.tar.gz` & `tmp/harreveltools-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "harreveltools-0.0.3.tar", last modified: Fri Sep 29 13:11:13 2023, max compression
+gzip compressed data, was "harreveltools-0.0.4.tar", last modified: Tue Apr  2 10:45:55 2024, max compression
```

## Comparing `harreveltools-0.0.3.tar` & `harreveltools-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxr-x   0 bugger    (1000) bugger    (1000)        0 2023-09-29 13:11:13.877413 harreveltools-0.0.3/
--rw-rw-r--   0 bugger    (1000) bugger    (1000)     1068 2023-02-20 13:33:03.000000 harreveltools-0.0.3/LICENSE
--rw-r--r--   0 bugger    (1000) bugger    (1000)      496 2023-09-29 13:11:13.877413 harreveltools-0.0.3/PKG-INFO
--rw-rw-r--   0 bugger    (1000) bugger    (1000)        8 2023-02-20 13:33:03.000000 harreveltools-0.0.3/README.md
--rw-rw-r--   0 bugger    (1000) bugger    (1000)      562 2023-09-29 13:11:06.000000 harreveltools-0.0.3/pyproject.toml
--rw-rw-r--   0 bugger    (1000) bugger    (1000)       38 2023-09-29 13:11:13.877413 harreveltools-0.0.3/setup.cfg
-drwxrwxr-x   0 bugger    (1000) bugger    (1000)        0 2023-09-29 13:11:13.873413 harreveltools-0.0.3/src/
--rw-rw-r--   0 bugger    (1000) bugger    (1000)        0 2023-02-20 13:33:03.000000 harreveltools-0.0.3/src/__init__.py
-drwxrwxr-x   0 bugger    (1000) bugger    (1000)        0 2023-09-29 13:11:13.873413 harreveltools-0.0.3/src/harreveltools/
--rw-rw-r--   0 bugger    (1000) bugger    (1000)        0 2023-02-20 13:33:03.000000 harreveltools-0.0.3/src/harreveltools/__init__.py
--rw-rw-r--   0 bugger    (1000) bugger    (1000)       42 2023-02-20 13:33:03.000000 harreveltools-0.0.3/src/harreveltools/example.py
-drwxrwxr-x   0 bugger    (1000) bugger    (1000)        0 2023-09-29 13:11:13.877413 harreveltools-0.0.3/src/harreveltools/helper/
--rw-rw-r--   0 bugger    (1000) bugger    (1000)        0 2023-02-20 13:33:03.000000 harreveltools-0.0.3/src/harreveltools/helper/__init__.py
--rw-rw-r--   0 bugger    (1000) bugger    (1000)    52909 2023-09-29 13:09:47.000000 harreveltools-0.0.3/src/harreveltools/helper/data_transform.py
--rw-rw-r--   0 bugger    (1000) bugger    (1000)    14302 2023-09-29 13:08:35.000000 harreveltools-0.0.3/src/harreveltools/helper/plot.py
-drwxrwxr-x   0 bugger    (1000) bugger    (1000)        0 2023-09-29 13:11:13.873413 harreveltools-0.0.3/src/harreveltools.egg-info/
--rw-r--r--   0 bugger    (1000) bugger    (1000)      496 2023-09-29 13:11:13.000000 harreveltools-0.0.3/src/harreveltools.egg-info/PKG-INFO
--rw-rw-r--   0 bugger    (1000) bugger    (1000)      410 2023-09-29 13:11:13.000000 harreveltools-0.0.3/src/harreveltools.egg-info/SOURCES.txt
--rw-rw-r--   0 bugger    (1000) bugger    (1000)        1 2023-09-29 13:11:13.000000 harreveltools-0.0.3/src/harreveltools.egg-info/dependency_links.txt
--rw-rw-r--   0 bugger    (1000) bugger    (1000)       23 2023-09-29 13:11:13.000000 harreveltools-0.0.3/src/harreveltools.egg-info/top_level.txt
-drwxrwxr-x   0 bugger    (1000) bugger    (1000)        0 2023-09-29 13:11:13.877413 harreveltools-0.0.3/tests/
--rw-rw-r--   0 bugger    (1000) bugger    (1000)       96 2023-02-20 13:33:03.000000 harreveltools-0.0.3/tests/test_helper_plot.py
+drwxrwxr-x   0 bugger    (1000) bugger    (1000)        0 2024-04-02 10:45:55.859957 harreveltools-0.0.4/
+-rw-rw-r--   0 bugger    (1000) bugger    (1000)     1068 2023-02-20 13:33:03.000000 harreveltools-0.0.4/LICENSE
+-rw-r--r--   0 bugger    (1000) bugger    (1000)      585 2024-04-02 10:45:55.859957 harreveltools-0.0.4/PKG-INFO
+-rw-rw-r--   0 bugger    (1000) bugger    (1000)       96 2024-04-02 10:45:50.000000 harreveltools-0.0.4/README.md
+-rw-rw-r--   0 bugger    (1000) bugger    (1000)      562 2024-04-02 10:43:14.000000 harreveltools-0.0.4/pyproject.toml
+-rw-rw-r--   0 bugger    (1000) bugger    (1000)       38 2024-04-02 10:45:55.859957 harreveltools-0.0.4/setup.cfg
+drwxrwxr-x   0 bugger    (1000) bugger    (1000)        0 2024-04-02 10:45:55.855957 harreveltools-0.0.4/src/
+-rw-rw-r--   0 bugger    (1000) bugger    (1000)        0 2023-02-20 13:33:03.000000 harreveltools-0.0.4/src/__init__.py
+drwxrwxr-x   0 bugger    (1000) bugger    (1000)        0 2024-04-02 10:45:55.855957 harreveltools-0.0.4/src/harreveltools/
+-rw-rw-r--   0 bugger    (1000) bugger    (1000)        0 2023-02-20 13:33:03.000000 harreveltools-0.0.4/src/harreveltools/__init__.py
+-rw-rw-r--   0 bugger    (1000) bugger    (1000)       42 2023-02-20 13:33:03.000000 harreveltools-0.0.4/src/harreveltools/example.py
+drwxrwxr-x   0 bugger    (1000) bugger    (1000)        0 2024-04-02 10:45:55.859957 harreveltools-0.0.4/src/harreveltools/helper/
+-rw-rw-r--   0 bugger    (1000) bugger    (1000)        0 2023-02-20 13:33:03.000000 harreveltools-0.0.4/src/harreveltools/helper/__init__.py
+-rw-rw-r--   0 bugger    (1000) bugger    (1000)    52909 2023-09-29 13:09:47.000000 harreveltools-0.0.4/src/harreveltools/helper/data_transform.py
+-rw-rw-r--   0 bugger    (1000) bugger    (1000)     2377 2024-04-02 10:41:47.000000 harreveltools-0.0.4/src/harreveltools/helper/file_handeling.py
+-rw-rw-r--   0 bugger    (1000) bugger    (1000)    14302 2023-09-29 13:08:35.000000 harreveltools-0.0.4/src/harreveltools/helper/plot.py
+drwxrwxr-x   0 bugger    (1000) bugger    (1000)        0 2024-04-02 10:45:55.859957 harreveltools-0.0.4/src/harreveltools.egg-info/
+-rw-r--r--   0 bugger    (1000) bugger    (1000)      585 2024-04-02 10:45:55.000000 harreveltools-0.0.4/src/harreveltools.egg-info/PKG-INFO
+-rw-rw-r--   0 bugger    (1000) bugger    (1000)      453 2024-04-02 10:45:55.000000 harreveltools-0.0.4/src/harreveltools.egg-info/SOURCES.txt
+-rw-rw-r--   0 bugger    (1000) bugger    (1000)        1 2024-04-02 10:45:55.000000 harreveltools-0.0.4/src/harreveltools.egg-info/dependency_links.txt
+-rw-rw-r--   0 bugger    (1000) bugger    (1000)       23 2024-04-02 10:45:55.000000 harreveltools-0.0.4/src/harreveltools.egg-info/top_level.txt
+drwxrwxr-x   0 bugger    (1000) bugger    (1000)        0 2024-04-02 10:45:55.859957 harreveltools-0.0.4/tests/
+-rw-rw-r--   0 bugger    (1000) bugger    (1000)       96 2023-02-20 13:33:03.000000 harreveltools-0.0.4/tests/test_helper_plot.py
```

### Comparing `harreveltools-0.0.3/LICENSE` & `harreveltools-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `harreveltools-0.0.3/pyproject.toml` & `harreveltools-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "harreveltools"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="S Harrevelt", email="author@example.com" },
 ]
 description = "This package is the result of sweat and tears"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `harreveltools-0.0.3/src/harreveltools/helper/data_transform.py` & `harreveltools-0.0.4/src/harreveltools/helper/data_transform.py`

 * *Files identical despite different names*

### Comparing `harreveltools-0.0.3/src/harreveltools/helper/plot.py` & `harreveltools-0.0.4/src/harreveltools/helper/plot.py`

 * *Files identical despite different names*

