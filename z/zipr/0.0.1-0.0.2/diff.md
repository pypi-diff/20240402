# Comparing `tmp/zipr-0.0.1.tar.gz` & `tmp/zipr-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zipr-0.0.1.tar", last modified: Thu Mar 28 16:49:14 2024, max compression
+gzip compressed data, was "zipr-0.0.2.tar", last modified: Tue Apr  2 17:37:37 2024, max compression
```

## Comparing `zipr-0.0.1.tar` & `zipr-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-03-28 16:49:14.193765 zipr-0.0.1/
--rw-r--r--   0 solst      (501) staff       (20)    11337 2024-03-28 11:48:35.000000 zipr-0.0.1/LICENSE
--rw-r--r--   0 solst      (501) staff       (20)      111 2024-03-28 11:48:35.000000 zipr-0.0.1/MANIFEST.in
--rw-r--r--   0 solst      (501) staff       (20)     2319 2024-03-28 16:49:14.193628 zipr-0.0.1/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)     1683 2024-03-28 16:48:56.000000 zipr-0.0.1/README.md
--rw-r--r--   0 solst      (501) staff       (20)      813 2024-03-28 11:48:50.000000 zipr-0.0.1/settings.ini
--rw-r--r--   0 solst      (501) staff       (20)       38 2024-03-28 16:49:14.193810 zipr-0.0.1/setup.cfg
--rw-r--r--   0 solst      (501) staff       (20)     2580 2024-03-28 11:48:35.000000 zipr-0.0.1/setup.py
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-03-28 16:49:14.192480 zipr-0.0.1/zipr/
--rw-r--r--   0 solst      (501) staff       (20)      322 2024-03-28 16:48:15.000000 zipr-0.0.1/zipr/__init__.py
--rw-r--r--   0 solst      (501) staff       (20)     6761 2024-03-28 16:48:15.000000 zipr-0.0.1/zipr/_modidx.py
--rw-r--r--   0 solst      (501) staff       (20)      421 2024-03-28 16:48:15.000000 zipr-0.0.1/zipr/_tmp.py
--rw-r--r--   0 solst      (501) staff       (20)    13572 2024-03-28 16:48:15.000000 zipr-0.0.1/zipr/core.py
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-03-28 16:49:14.193427 zipr-0.0.1/zipr.egg-info/
--rw-r--r--   0 solst      (501) staff       (20)     2319 2024-03-28 16:49:14.000000 zipr-0.0.1/zipr.egg-info/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)      307 2024-03-28 16:49:14.000000 zipr-0.0.1/zipr.egg-info/SOURCES.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2024-03-28 16:49:14.000000 zipr-0.0.1/zipr.egg-info/dependency_links.txt
--rw-r--r--   0 solst      (501) staff       (20)       30 2024-03-28 16:49:14.000000 zipr-0.0.1/zipr.egg-info/entry_points.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2024-03-28 16:46:14.000000 zipr-0.0.1/zipr.egg-info/not-zip-safe
--rw-r--r--   0 solst      (501) staff       (20)        7 2024-03-28 16:49:14.000000 zipr-0.0.1/zipr.egg-info/requires.txt
--rw-r--r--   0 solst      (501) staff       (20)        5 2024-03-28 16:49:14.000000 zipr-0.0.1/zipr.egg-info/top_level.txt
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-02 17:37:37.338498 zipr-0.0.2/
+-rw-r--r--   0 solst      (501) staff       (20)    11337 2024-03-28 11:48:35.000000 zipr-0.0.2/LICENSE
+-rw-r--r--   0 solst      (501) staff       (20)      111 2024-03-28 11:48:35.000000 zipr-0.0.2/MANIFEST.in
+-rw-r--r--   0 solst      (501) staff       (20)     2319 2024-04-02 17:37:37.338329 zipr-0.0.2/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)     1683 2024-03-28 16:48:56.000000 zipr-0.0.2/README.md
+-rw-r--r--   0 solst      (501) staff       (20)      813 2024-03-28 16:50:26.000000 zipr-0.0.2/settings.ini
+-rw-r--r--   0 solst      (501) staff       (20)       38 2024-04-02 17:37:37.338556 zipr-0.0.2/setup.cfg
+-rw-r--r--   0 solst      (501) staff       (20)     2580 2024-03-28 11:48:35.000000 zipr-0.0.2/setup.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-02 17:37:37.336758 zipr-0.0.2/zipr/
+-rw-r--r--   0 solst      (501) staff       (20)      322 2024-04-02 17:37:31.000000 zipr-0.0.2/zipr/__init__.py
+-rw-r--r--   0 solst      (501) staff       (20)    21556 2024-04-02 17:37:31.000000 zipr-0.0.2/zipr/_modidx.py
+-rw-r--r--   0 solst      (501) staff       (20)      421 2024-04-02 17:37:31.000000 zipr-0.0.2/zipr/_tmp.py
+-rw-r--r--   0 solst      (501) staff       (20)    58968 2024-04-02 17:37:31.000000 zipr-0.0.2/zipr/core.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-02 17:37:37.338093 zipr-0.0.2/zipr.egg-info/
+-rw-r--r--   0 solst      (501) staff       (20)     2319 2024-04-02 17:37:37.000000 zipr-0.0.2/zipr.egg-info/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)      307 2024-04-02 17:37:37.000000 zipr-0.0.2/zipr.egg-info/SOURCES.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2024-04-02 17:37:37.000000 zipr-0.0.2/zipr.egg-info/dependency_links.txt
+-rw-r--r--   0 solst      (501) staff       (20)       30 2024-04-02 17:37:37.000000 zipr-0.0.2/zipr.egg-info/entry_points.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2024-03-28 16:46:14.000000 zipr-0.0.2/zipr.egg-info/not-zip-safe
+-rw-r--r--   0 solst      (501) staff       (20)        7 2024-04-02 17:37:37.000000 zipr-0.0.2/zipr.egg-info/requires.txt
+-rw-r--r--   0 solst      (501) staff       (20)        5 2024-04-02 17:37:37.000000 zipr-0.0.2/zipr.egg-info/top_level.txt
```

### Comparing `zipr-0.0.1/LICENSE` & `zipr-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `zipr-0.0.1/PKG-INFO` & `zipr-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zipr
-Version: 0.0.1
+Version: 0.0.2
 Summary: zipr
 Home-page: https://github.com/dsm-72/zipr
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: zipr mount load package library mounter loader inspect import importlib pkg module
 Classifier: Development Status :: 4 - Beta
```

### Comparing `zipr-0.0.1/README.md` & `zipr-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `zipr-0.0.1/settings.ini` & `zipr-0.0.2/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = zipr
 lib_name = zipr
-version = 0.0.1
+version = 0.0.2
 min_python = 3.11
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = zipr
 nbs_path = nbs
 recursive = True
```

### Comparing `zipr-0.0.1/setup.py` & `zipr-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `zipr-0.0.1/zipr.egg-info/PKG-INFO` & `zipr-0.0.2/zipr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zipr
-Version: 0.0.1
+Version: 0.0.2
 Summary: zipr
 Home-page: https://github.com/dsm-72/zipr
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: zipr mount load package library mounter loader inspect import importlib pkg module
 Classifier: Development Status :: 4 - Beta
```

