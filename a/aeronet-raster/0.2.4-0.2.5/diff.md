# Comparing `tmp/aeronet_raster-0.2.4.tar.gz` & `tmp/aeronet_raster-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aeronet_raster-0.2.4.tar", last modified: Thu Mar 28 14:59:49 2024, max compression
+gzip compressed data, was "aeronet_raster-0.2.5.tar", last modified: Tue Apr  2 15:39:56 2024, max compression
```

## Comparing `aeronet_raster-0.2.4.tar` & `aeronet_raster-0.2.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 vasiliy   (1000) vasiliy   (1000)        0 2024-03-28 14:59:49.290567 aeronet_raster-0.2.4/
--rw-r--r--   0 vasiliy   (1000) vasiliy   (1000)      796 2024-03-28 14:59:49.290567 aeronet_raster-0.2.4/PKG-INFO
--rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)     4784 2024-03-28 14:57:48.000000 aeronet_raster-0.2.4/README.rst
-drwxrwxr-x   0 vasiliy   (1000) vasiliy   (1000)        0 2024-03-28 14:59:49.290567 aeronet_raster-0.2.4/aeronet_raster/
--rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)      392 2024-03-28 14:57:48.000000 aeronet_raster-0.2.4/aeronet_raster/__init__.py
--rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)       63 2024-03-28 14:57:48.000000 aeronet_raster-0.2.4/aeronet_raster/__version__.py
-drwxrwxr-x   0 vasiliy   (1000) vasiliy   (1000)        0 2024-03-28 14:59:49.290567 aeronet_raster-0.2.4/aeronet_raster/band/
--rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)       58 2024-03-28 14:57:48.000000 aeronet_raster-0.2.4/aeronet_raster/band/__init__.py
--rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)    16937 2024-03-28 14:57:48.000000 aeronet_raster-0.2.4/aeronet_raster/band/band.py
--rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)    12101 2024-03-28 14:57:48.000000 aeronet_raster-0.2.4/aeronet_raster/band/bandsample.py
-drwxrwxr-x   0 vasiliy   (1000) vasiliy   (1000)        0 2024-03-28 14:59:49.290567 aeronet_raster-0.2.4/aeronet_raster/bandcollection/
--rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)       98 2024-03-28 14:57:48.000000 aeronet_raster-0.2.4/aeronet_raster/bandcollection/__init__.py
--rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)     7392 2024-03-28 14:57:48.000000 aeronet_raster-0.2.4/aeronet_raster/bandcollection/bandcollection.py
--rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)     5982 2024-03-28 14:57:48.000000 aeronet_raster-0.2.4/aeronet_raster/bandcollection/bandcollectionsample.py
--rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)    22143 2024-03-28 14:57:48.000000 aeronet_raster-0.2.4/aeronet_raster/collectionprocessor.py
-drwxrwxr-x   0 vasiliy   (1000) vasiliy   (1000)        0 2024-03-28 14:59:49.290567 aeronet_raster-0.2.4/aeronet_raster/geoobject/
--rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)       32 2024-03-28 14:57:48.000000 aeronet_raster-0.2.4/aeronet_raster/geoobject/__init__.py
--rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)     2642 2024-03-28 14:57:48.000000 aeronet_raster-0.2.4/aeronet_raster/geoobject/geoobject.py
--rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)     1997 2024-03-28 14:57:48.000000 aeronet_raster-0.2.4/aeronet_raster/merge.py
--rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)     5729 2024-03-28 14:57:48.000000 aeronet_raster-0.2.4/aeronet_raster/split.py
-drwxrwxr-x   0 vasiliy   (1000) vasiliy   (1000)        0 2024-03-28 14:59:49.290567 aeronet_raster-0.2.4/aeronet_raster/utils/
--rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)        0 2024-03-28 14:57:48.000000 aeronet_raster-0.2.4/aeronet_raster/utils/__init__.py
--rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)     6530 2024-03-28 14:57:48.000000 aeronet_raster-0.2.4/aeronet_raster/utils/calc_window_weight_mtrx.py
--rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)     1267 2024-03-28 14:57:48.000000 aeronet_raster-0.2.4/aeronet_raster/utils/coords.py
--rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)     1269 2024-03-28 14:57:48.000000 aeronet_raster-0.2.4/aeronet_raster/utils/utils.py
-drwxrwxr-x   0 vasiliy   (1000) vasiliy   (1000)        0 2024-03-28 14:59:49.290567 aeronet_raster-0.2.4/aeronet_raster.egg-info/
--rw-r--r--   0 vasiliy   (1000) vasiliy   (1000)      796 2024-03-28 14:59:49.000000 aeronet_raster-0.2.4/aeronet_raster.egg-info/PKG-INFO
--rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)      806 2024-03-28 14:59:49.000000 aeronet_raster-0.2.4/aeronet_raster.egg-info/SOURCES.txt
--rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)        1 2024-03-28 14:59:49.000000 aeronet_raster-0.2.4/aeronet_raster.egg-info/dependency_links.txt
--rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)       49 2024-03-28 14:59:49.000000 aeronet_raster-0.2.4/aeronet_raster.egg-info/requires.txt
--rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)       15 2024-03-28 14:59:49.000000 aeronet_raster-0.2.4/aeronet_raster.egg-info/top_level.txt
--rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)       38 2024-03-28 14:59:49.290567 aeronet_raster-0.2.4/setup.cfg
--rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)     3757 2024-03-28 14:57:48.000000 aeronet_raster-0.2.4/setup.py
+drwxrwxr-x   0 vasiliy   (1000) vasiliy   (1000)        0 2024-04-02 15:39:56.838285 aeronet_raster-0.2.5/
+-rw-r--r--   0 vasiliy   (1000) vasiliy   (1000)      796 2024-04-02 15:39:56.838285 aeronet_raster-0.2.5/PKG-INFO
+-rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)     4784 2024-03-28 14:57:48.000000 aeronet_raster-0.2.5/README.rst
+drwxrwxr-x   0 vasiliy   (1000) vasiliy   (1000)        0 2024-04-02 15:39:56.838285 aeronet_raster-0.2.5/aeronet_raster/
+-rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)      392 2024-03-28 14:57:48.000000 aeronet_raster-0.2.5/aeronet_raster/__init__.py
+-rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)       63 2024-04-02 15:25:28.000000 aeronet_raster-0.2.5/aeronet_raster/__version__.py
+drwxrwxr-x   0 vasiliy   (1000) vasiliy   (1000)        0 2024-04-02 15:39:56.838285 aeronet_raster-0.2.5/aeronet_raster/band/
+-rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)       58 2024-03-28 14:57:48.000000 aeronet_raster-0.2.5/aeronet_raster/band/__init__.py
+-rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)    16937 2024-03-28 14:57:48.000000 aeronet_raster-0.2.5/aeronet_raster/band/band.py
+-rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)    12101 2024-03-28 14:57:48.000000 aeronet_raster-0.2.5/aeronet_raster/band/bandsample.py
+drwxrwxr-x   0 vasiliy   (1000) vasiliy   (1000)        0 2024-04-02 15:39:56.838285 aeronet_raster-0.2.5/aeronet_raster/bandcollection/
+-rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)       98 2024-03-28 14:57:48.000000 aeronet_raster-0.2.5/aeronet_raster/bandcollection/__init__.py
+-rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)     7392 2024-03-28 14:57:48.000000 aeronet_raster-0.2.5/aeronet_raster/bandcollection/bandcollection.py
+-rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)     5982 2024-03-28 14:57:48.000000 aeronet_raster-0.2.5/aeronet_raster/bandcollection/bandcollectionsample.py
+-rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)    22143 2024-03-28 14:57:48.000000 aeronet_raster-0.2.5/aeronet_raster/collectionprocessor.py
+drwxrwxr-x   0 vasiliy   (1000) vasiliy   (1000)        0 2024-04-02 15:39:56.838285 aeronet_raster-0.2.5/aeronet_raster/geoobject/
+-rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)       32 2024-03-28 14:57:48.000000 aeronet_raster-0.2.5/aeronet_raster/geoobject/__init__.py
+-rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)     2642 2024-03-28 14:57:48.000000 aeronet_raster-0.2.5/aeronet_raster/geoobject/geoobject.py
+-rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)     1997 2024-03-28 14:57:48.000000 aeronet_raster-0.2.5/aeronet_raster/merge.py
+-rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)     5729 2024-03-28 14:57:48.000000 aeronet_raster-0.2.5/aeronet_raster/split.py
+drwxrwxr-x   0 vasiliy   (1000) vasiliy   (1000)        0 2024-04-02 15:39:56.838285 aeronet_raster-0.2.5/aeronet_raster/utils/
+-rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)        0 2024-03-28 14:57:48.000000 aeronet_raster-0.2.5/aeronet_raster/utils/__init__.py
+-rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)     6530 2024-03-28 14:57:48.000000 aeronet_raster-0.2.5/aeronet_raster/utils/calc_window_weight_mtrx.py
+-rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)     1267 2024-03-28 14:57:48.000000 aeronet_raster-0.2.5/aeronet_raster/utils/coords.py
+-rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)     1269 2024-03-28 14:57:48.000000 aeronet_raster-0.2.5/aeronet_raster/utils/utils.py
+drwxrwxr-x   0 vasiliy   (1000) vasiliy   (1000)        0 2024-04-02 15:39:56.838285 aeronet_raster-0.2.5/aeronet_raster.egg-info/
+-rw-r--r--   0 vasiliy   (1000) vasiliy   (1000)      796 2024-04-02 15:39:56.000000 aeronet_raster-0.2.5/aeronet_raster.egg-info/PKG-INFO
+-rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)      806 2024-04-02 15:39:56.000000 aeronet_raster-0.2.5/aeronet_raster.egg-info/SOURCES.txt
+-rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)        1 2024-04-02 15:39:56.000000 aeronet_raster-0.2.5/aeronet_raster.egg-info/dependency_links.txt
+-rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)       49 2024-04-02 15:39:56.000000 aeronet_raster-0.2.5/aeronet_raster.egg-info/requires.txt
+-rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)       15 2024-04-02 15:39:56.000000 aeronet_raster-0.2.5/aeronet_raster.egg-info/top_level.txt
+-rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)       38 2024-04-02 15:39:56.838285 aeronet_raster-0.2.5/setup.cfg
+-rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)     3757 2024-03-28 14:57:48.000000 aeronet_raster-0.2.5/setup.py
```

### Comparing `aeronet_raster-0.2.4/PKG-INFO` & `aeronet_raster-0.2.5/aeronet_raster.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: aeronet_raster
-Version: 0.2.4
+Name: aeronet-raster
+Version: 0.2.5
 Summary: Raster operations for deep learning with remote sensing data. Based on Rasterio.
 Home-page: 
 Author: Geoalert
 Author-email: hello@geoalert.io
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `aeronet_raster-0.2.4/README.rst` & `aeronet_raster-0.2.5/README.rst`

 * *Files identical despite different names*

### Comparing `aeronet_raster-0.2.4/aeronet_raster/band/band.py` & `aeronet_raster-0.2.5/aeronet_raster/band/band.py`

 * *Files identical despite different names*

### Comparing `aeronet_raster-0.2.4/aeronet_raster/band/bandsample.py` & `aeronet_raster-0.2.5/aeronet_raster/band/bandsample.py`

 * *Files identical despite different names*

### Comparing `aeronet_raster-0.2.4/aeronet_raster/bandcollection/bandcollection.py` & `aeronet_raster-0.2.5/aeronet_raster/bandcollection/bandcollection.py`

 * *Files identical despite different names*

### Comparing `aeronet_raster-0.2.4/aeronet_raster/bandcollection/bandcollectionsample.py` & `aeronet_raster-0.2.5/aeronet_raster/bandcollection/bandcollectionsample.py`

 * *Files identical despite different names*

### Comparing `aeronet_raster-0.2.4/aeronet_raster/collectionprocessor.py` & `aeronet_raster-0.2.5/aeronet_raster/collectionprocessor.py`

 * *Files identical despite different names*

### Comparing `aeronet_raster-0.2.4/aeronet_raster/geoobject/geoobject.py` & `aeronet_raster-0.2.5/aeronet_raster/geoobject/geoobject.py`

 * *Files identical despite different names*

### Comparing `aeronet_raster-0.2.4/aeronet_raster/merge.py` & `aeronet_raster-0.2.5/aeronet_raster/merge.py`

 * *Files identical despite different names*

### Comparing `aeronet_raster-0.2.4/aeronet_raster/split.py` & `aeronet_raster-0.2.5/aeronet_raster/split.py`

 * *Files identical despite different names*

### Comparing `aeronet_raster-0.2.4/aeronet_raster/utils/calc_window_weight_mtrx.py` & `aeronet_raster-0.2.5/aeronet_raster/utils/calc_window_weight_mtrx.py`

 * *Files identical despite different names*

### Comparing `aeronet_raster-0.2.4/aeronet_raster/utils/coords.py` & `aeronet_raster-0.2.5/aeronet_raster/utils/coords.py`

 * *Files identical despite different names*

### Comparing `aeronet_raster-0.2.4/aeronet_raster/utils/utils.py` & `aeronet_raster-0.2.5/aeronet_raster/utils/utils.py`

 * *Files identical despite different names*

### Comparing `aeronet_raster-0.2.4/aeronet_raster.egg-info/PKG-INFO` & `aeronet_raster-0.2.5/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: aeronet-raster
-Version: 0.2.4
+Name: aeronet_raster
+Version: 0.2.5
 Summary: Raster operations for deep learning with remote sensing data. Based on Rasterio.
 Home-page: 
 Author: Geoalert
 Author-email: hello@geoalert.io
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `aeronet_raster-0.2.4/aeronet_raster.egg-info/SOURCES.txt` & `aeronet_raster-0.2.5/aeronet_raster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aeronet_raster-0.2.4/setup.py` & `aeronet_raster-0.2.5/setup.py`

 * *Files identical despite different names*

