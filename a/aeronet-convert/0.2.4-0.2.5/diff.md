# Comparing `tmp/aeronet_convert-0.2.4.tar.gz` & `tmp/aeronet_convert-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aeronet_convert-0.2.4.tar", last modified: Thu Mar 28 14:59:49 2024, max compression
+gzip compressed data, was "aeronet_convert-0.2.5.tar", last modified: Tue Apr  2 15:39:57 2024, max compression
```

## Comparing `aeronet_convert-0.2.4.tar` & `aeronet_convert-0.2.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 vasiliy   (1000) vasiliy   (1000)        0 2024-03-28 14:59:49.546564 aeronet_convert-0.2.4/
--rw-r--r--   0 vasiliy   (1000) vasiliy   (1000)      861 2024-03-28 14:59:49.546564 aeronet_convert-0.2.4/PKG-INFO
--rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)     2053 2024-03-28 14:57:48.000000 aeronet_convert-0.2.4/README.rst
-drwxrwxr-x   0 vasiliy   (1000) vasiliy   (1000)        0 2024-03-28 14:59:49.546564 aeronet_convert-0.2.4/aeronet_convert/
--rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)       67 2024-03-28 14:57:48.000000 aeronet_convert-0.2.4/aeronet_convert/__init__.py
--rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)       63 2024-03-28 14:57:48.000000 aeronet_convert-0.2.4/aeronet_convert/__version__.py
--rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)     1250 2024-03-28 14:57:48.000000 aeronet_convert-0.2.4/aeronet_convert/rasterize.py
--rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)     5428 2024-03-28 14:57:48.000000 aeronet_convert-0.2.4/aeronet_convert/vectorize.py
-drwxrwxr-x   0 vasiliy   (1000) vasiliy   (1000)        0 2024-03-28 14:59:49.546564 aeronet_convert-0.2.4/aeronet_convert.egg-info/
--rw-r--r--   0 vasiliy   (1000) vasiliy   (1000)      861 2024-03-28 14:59:49.000000 aeronet_convert-0.2.4/aeronet_convert.egg-info/PKG-INFO
--rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)      330 2024-03-28 14:59:49.000000 aeronet_convert-0.2.4/aeronet_convert.egg-info/SOURCES.txt
--rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)        1 2024-03-28 14:59:49.000000 aeronet_convert-0.2.4/aeronet_convert.egg-info/dependency_links.txt
--rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)       65 2024-03-28 14:59:49.000000 aeronet_convert-0.2.4/aeronet_convert.egg-info/requires.txt
--rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)       16 2024-03-28 14:59:49.000000 aeronet_convert-0.2.4/aeronet_convert.egg-info/top_level.txt
--rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)       38 2024-03-28 14:59:49.546564 aeronet_convert-0.2.4/setup.cfg
--rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)     4373 2024-03-28 14:57:48.000000 aeronet_convert-0.2.4/setup.py
+drwxrwxr-x   0 vasiliy   (1000) vasiliy   (1000)        0 2024-04-02 15:39:57.086287 aeronet_convert-0.2.5/
+-rw-r--r--   0 vasiliy   (1000) vasiliy   (1000)      861 2024-04-02 15:39:57.086287 aeronet_convert-0.2.5/PKG-INFO
+-rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)     2053 2024-03-28 14:57:48.000000 aeronet_convert-0.2.5/README.rst
+drwxrwxr-x   0 vasiliy   (1000) vasiliy   (1000)        0 2024-04-02 15:39:57.086287 aeronet_convert-0.2.5/aeronet_convert/
+-rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)       67 2024-03-28 14:57:48.000000 aeronet_convert-0.2.5/aeronet_convert/__init__.py
+-rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)       63 2024-04-02 15:25:28.000000 aeronet_convert-0.2.5/aeronet_convert/__version__.py
+-rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)     1250 2024-03-28 14:57:48.000000 aeronet_convert-0.2.5/aeronet_convert/rasterize.py
+-rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)     5428 2024-03-28 14:57:48.000000 aeronet_convert-0.2.5/aeronet_convert/vectorize.py
+drwxrwxr-x   0 vasiliy   (1000) vasiliy   (1000)        0 2024-04-02 15:39:57.086287 aeronet_convert-0.2.5/aeronet_convert.egg-info/
+-rw-r--r--   0 vasiliy   (1000) vasiliy   (1000)      861 2024-04-02 15:39:57.000000 aeronet_convert-0.2.5/aeronet_convert.egg-info/PKG-INFO
+-rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)      330 2024-04-02 15:39:57.000000 aeronet_convert-0.2.5/aeronet_convert.egg-info/SOURCES.txt
+-rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)        1 2024-04-02 15:39:57.000000 aeronet_convert-0.2.5/aeronet_convert.egg-info/dependency_links.txt
+-rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)       65 2024-04-02 15:39:57.000000 aeronet_convert-0.2.5/aeronet_convert.egg-info/requires.txt
+-rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)       16 2024-04-02 15:39:57.000000 aeronet_convert-0.2.5/aeronet_convert.egg-info/top_level.txt
+-rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)       38 2024-04-02 15:39:57.086287 aeronet_convert-0.2.5/setup.cfg
+-rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)     4373 2024-03-28 14:57:48.000000 aeronet_convert-0.2.5/setup.py
```

### Comparing `aeronet_convert-0.2.4/PKG-INFO` & `aeronet_convert-0.2.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: aeronet_convert
-Version: 0.2.4
+Version: 0.2.5
 Summary: Raster-vector conversion for deep learning with remote sensing data. Based on opencv, rasterio, shapely.
 Home-page: 
 Author: Geoalert
 Author-email: hello@geoalert.io
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 Requires-Dist: opencv-python>=4.0.0
-Requires-Dist: aeronet-raster==0.2.4
-Requires-Dist: aeronet-vector==0.2.4
+Requires-Dist: aeronet-raster==0.2.5
+Requires-Dist: aeronet-vector==0.2.5
 
 Raster-vector conversion for deep learning with remote sensing data. Based on opencv, rasterio, shapely.
```

### Comparing `aeronet_convert-0.2.4/README.rst` & `aeronet_convert-0.2.5/README.rst`

 * *Files identical despite different names*

### Comparing `aeronet_convert-0.2.4/aeronet_convert/rasterize.py` & `aeronet_convert-0.2.5/aeronet_convert/rasterize.py`

 * *Files identical despite different names*

### Comparing `aeronet_convert-0.2.4/aeronet_convert/vectorize.py` & `aeronet_convert-0.2.5/aeronet_convert/vectorize.py`

 * *Files identical despite different names*

### Comparing `aeronet_convert-0.2.4/aeronet_convert.egg-info/PKG-INFO` & `aeronet_convert-0.2.5/aeronet_convert.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: aeronet-convert
-Version: 0.2.4
+Version: 0.2.5
 Summary: Raster-vector conversion for deep learning with remote sensing data. Based on opencv, rasterio, shapely.
 Home-page: 
 Author: Geoalert
 Author-email: hello@geoalert.io
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 Requires-Dist: opencv-python>=4.0.0
-Requires-Dist: aeronet-raster==0.2.4
-Requires-Dist: aeronet-vector==0.2.4
+Requires-Dist: aeronet-raster==0.2.5
+Requires-Dist: aeronet-vector==0.2.5
 
 Raster-vector conversion for deep learning with remote sensing data. Based on opencv, rasterio, shapely.
```

### Comparing `aeronet_convert-0.2.4/setup.py` & `aeronet_convert-0.2.5/setup.py`

 * *Files identical despite different names*

