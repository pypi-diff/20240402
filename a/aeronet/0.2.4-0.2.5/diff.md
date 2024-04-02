# Comparing `tmp/aeronet-0.2.4.tar.gz` & `tmp/aeronet-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aeronet-0.2.4.tar", last modified: Thu Mar 28 14:59:49 2024, max compression
+gzip compressed data, was "aeronet-0.2.5.tar", last modified: Tue Apr  2 15:39:57 2024, max compression
```

## Comparing `aeronet-0.2.4.tar` & `aeronet-0.2.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 vasiliy   (1000) vasiliy   (1000)        0 2024-03-28 14:59:49.666563 aeronet-0.2.4/
--rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)     1077 2024-03-28 14:57:48.000000 aeronet-0.2.4/LICENSE
--rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)       18 2024-03-28 14:57:48.000000 aeronet-0.2.4/MANIFEST.in
--rw-r--r--   0 vasiliy   (1000) vasiliy   (1000)     1056 2024-03-28 14:59:49.666563 aeronet-0.2.4/PKG-INFO
--rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)     4729 2024-03-28 14:57:48.000000 aeronet-0.2.4/README.rst
-drwxrwxr-x   0 vasiliy   (1000) vasiliy   (1000)        0 2024-03-28 14:59:49.666563 aeronet-0.2.4/aeronet/
--rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)        0 2024-03-28 14:57:48.000000 aeronet-0.2.4/aeronet/__init__.py
--rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)       63 2024-03-28 14:57:48.000000 aeronet-0.2.4/aeronet/__version__.py
-drwxrwxr-x   0 vasiliy   (1000) vasiliy   (1000)        0 2024-03-28 14:59:49.666563 aeronet-0.2.4/aeronet/converters/
--rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)        0 2024-03-28 14:57:48.000000 aeronet-0.2.4/aeronet/converters/__init__.py
--rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)      225 2024-03-28 14:57:48.000000 aeronet-0.2.4/aeronet/converters/split.py
-drwxrwxr-x   0 vasiliy   (1000) vasiliy   (1000)        0 2024-03-28 14:59:49.666563 aeronet-0.2.4/aeronet/dataset/
--rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)      905 2024-03-28 14:57:48.000000 aeronet-0.2.4/aeronet/dataset/__init__.py
--rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)      263 2024-03-28 14:57:48.000000 aeronet-0.2.4/aeronet/dataset/coords.py
-drwxrwxr-x   0 vasiliy   (1000) vasiliy   (1000)        0 2024-03-28 14:59:49.666563 aeronet-0.2.4/aeronet/dataset/io/
--rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)      415 2024-03-28 14:57:48.000000 aeronet-0.2.4/aeronet/dataset/io/__init__.py
--rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)      230 2024-03-28 14:57:48.000000 aeronet-0.2.4/aeronet/dataset/utils.py
-drwxrwxr-x   0 vasiliy   (1000) vasiliy   (1000)        0 2024-03-28 14:59:49.666563 aeronet-0.2.4/aeronet.egg-info/
--rw-r--r--   0 vasiliy   (1000) vasiliy   (1000)     1056 2024-03-28 14:59:49.000000 aeronet-0.2.4/aeronet.egg-info/PKG-INFO
--rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)      405 2024-03-28 14:59:49.000000 aeronet-0.2.4/aeronet.egg-info/SOURCES.txt
--rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)        1 2024-03-28 14:59:49.000000 aeronet-0.2.4/aeronet.egg-info/dependency_links.txt
--rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)      172 2024-03-28 14:59:49.000000 aeronet-0.2.4/aeronet.egg-info/requires.txt
--rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)       62 2024-03-28 14:59:49.000000 aeronet-0.2.4/aeronet.egg-info/top_level.txt
--rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)       38 2024-03-28 14:59:49.666563 aeronet-0.2.4/setup.cfg
--rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)     4157 2024-03-28 14:57:48.000000 aeronet-0.2.4/setup.py
+drwxrwxr-x   0 vasiliy   (1000) vasiliy   (1000)        0 2024-04-02 15:39:57.210288 aeronet-0.2.5/
+-rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)     1077 2024-03-28 14:57:48.000000 aeronet-0.2.5/LICENSE
+-rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)       18 2024-03-28 14:57:48.000000 aeronet-0.2.5/MANIFEST.in
+-rw-r--r--   0 vasiliy   (1000) vasiliy   (1000)     1056 2024-04-02 15:39:57.210288 aeronet-0.2.5/PKG-INFO
+-rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)     4729 2024-03-28 14:57:48.000000 aeronet-0.2.5/README.rst
+drwxrwxr-x   0 vasiliy   (1000) vasiliy   (1000)        0 2024-04-02 15:39:57.210288 aeronet-0.2.5/aeronet/
+-rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)        0 2024-03-28 14:57:48.000000 aeronet-0.2.5/aeronet/__init__.py
+-rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)       63 2024-04-02 15:25:28.000000 aeronet-0.2.5/aeronet/__version__.py
+drwxrwxr-x   0 vasiliy   (1000) vasiliy   (1000)        0 2024-04-02 15:39:57.210288 aeronet-0.2.5/aeronet/converters/
+-rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)        0 2024-03-28 14:57:48.000000 aeronet-0.2.5/aeronet/converters/__init__.py
+-rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)      225 2024-03-28 14:57:48.000000 aeronet-0.2.5/aeronet/converters/split.py
+drwxrwxr-x   0 vasiliy   (1000) vasiliy   (1000)        0 2024-04-02 15:39:57.210288 aeronet-0.2.5/aeronet/dataset/
+-rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)      905 2024-03-28 14:57:48.000000 aeronet-0.2.5/aeronet/dataset/__init__.py
+-rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)      263 2024-03-28 14:57:48.000000 aeronet-0.2.5/aeronet/dataset/coords.py
+drwxrwxr-x   0 vasiliy   (1000) vasiliy   (1000)        0 2024-04-02 15:39:57.210288 aeronet-0.2.5/aeronet/dataset/io/
+-rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)      415 2024-03-28 14:57:48.000000 aeronet-0.2.5/aeronet/dataset/io/__init__.py
+-rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)      230 2024-03-28 14:57:48.000000 aeronet-0.2.5/aeronet/dataset/utils.py
+drwxrwxr-x   0 vasiliy   (1000) vasiliy   (1000)        0 2024-04-02 15:39:57.210288 aeronet-0.2.5/aeronet.egg-info/
+-rw-r--r--   0 vasiliy   (1000) vasiliy   (1000)     1056 2024-04-02 15:39:57.000000 aeronet-0.2.5/aeronet.egg-info/PKG-INFO
+-rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)      405 2024-04-02 15:39:57.000000 aeronet-0.2.5/aeronet.egg-info/SOURCES.txt
+-rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)        1 2024-04-02 15:39:57.000000 aeronet-0.2.5/aeronet.egg-info/dependency_links.txt
+-rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)      172 2024-04-02 15:39:57.000000 aeronet-0.2.5/aeronet.egg-info/requires.txt
+-rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)       62 2024-04-02 15:39:57.000000 aeronet-0.2.5/aeronet.egg-info/top_level.txt
+-rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)       38 2024-04-02 15:39:57.210288 aeronet-0.2.5/setup.cfg
+-rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)     4157 2024-03-28 14:57:48.000000 aeronet-0.2.5/setup.py
```

### Comparing `aeronet-0.2.4/LICENSE` & `aeronet-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aeronet-0.2.4/PKG-INFO` & `aeronet-0.2.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aeronet
-Version: 0.2.4
+Version: 0.2.5
 Summary: Deep learning with remote sensing data.
 Home-page: 
 Author: Geoalert
 Author-email: hello@geoalert.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -12,18 +12,18 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: raster
-Requires-Dist: aeronet-raster==0.2.4; extra == "raster"
+Requires-Dist: aeronet-raster==0.2.5; extra == "raster"
 Provides-Extra: vector
-Requires-Dist: aeronet-vector==0.2.4; extra == "vector"
+Requires-Dist: aeronet-vector==0.2.5; extra == "vector"
 Provides-Extra: convert
-Requires-Dist: aeronet-convert==0.2.4; extra == "convert"
+Requires-Dist: aeronet-convert==0.2.5; extra == "convert"
 Provides-Extra: all
-Requires-Dist: aeronet-vector==0.2.4; extra == "all"
-Requires-Dist: aeronet-raster==0.2.4; extra == "all"
-Requires-Dist: aeronet-convert==0.2.4; extra == "all"
+Requires-Dist: aeronet-vector==0.2.5; extra == "all"
+Requires-Dist: aeronet-raster==0.2.5; extra == "all"
+Requires-Dist: aeronet-convert==0.2.5; extra == "all"
 
 Deep learning with remote sensing data.
```

### Comparing `aeronet-0.2.4/README.rst` & `aeronet-0.2.5/README.rst`

 * *Files identical despite different names*

### Comparing `aeronet-0.2.4/aeronet/dataset/__init__.py` & `aeronet-0.2.5/aeronet/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `aeronet-0.2.4/aeronet.egg-info/PKG-INFO` & `aeronet-0.2.5/aeronet.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aeronet
-Version: 0.2.4
+Version: 0.2.5
 Summary: Deep learning with remote sensing data.
 Home-page: 
 Author: Geoalert
 Author-email: hello@geoalert.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -12,18 +12,18 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: raster
-Requires-Dist: aeronet-raster==0.2.4; extra == "raster"
+Requires-Dist: aeronet-raster==0.2.5; extra == "raster"
 Provides-Extra: vector
-Requires-Dist: aeronet-vector==0.2.4; extra == "vector"
+Requires-Dist: aeronet-vector==0.2.5; extra == "vector"
 Provides-Extra: convert
-Requires-Dist: aeronet-convert==0.2.4; extra == "convert"
+Requires-Dist: aeronet-convert==0.2.5; extra == "convert"
 Provides-Extra: all
-Requires-Dist: aeronet-vector==0.2.4; extra == "all"
-Requires-Dist: aeronet-raster==0.2.4; extra == "all"
-Requires-Dist: aeronet-convert==0.2.4; extra == "all"
+Requires-Dist: aeronet-vector==0.2.5; extra == "all"
+Requires-Dist: aeronet-raster==0.2.5; extra == "all"
+Requires-Dist: aeronet-convert==0.2.5; extra == "all"
 
 Deep learning with remote sensing data.
```

### Comparing `aeronet-0.2.4/setup.py` & `aeronet-0.2.5/setup.py`

 * *Files identical despite different names*

