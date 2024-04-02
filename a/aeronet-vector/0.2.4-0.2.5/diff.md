# Comparing `tmp/aeronet_vector-0.2.4.tar.gz` & `tmp/aeronet_vector-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aeronet_vector-0.2.4.tar", last modified: Thu Mar 28 14:59:49 2024, max compression
+gzip compressed data, was "aeronet_vector-0.2.5.tar", last modified: Tue Apr  2 15:39:56 2024, max compression
```

## Comparing `aeronet_vector-0.2.4.tar` & `aeronet_vector-0.2.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 vasiliy   (1000) vasiliy   (1000)        0 2024-03-28 14:59:49.430566 aeronet_vector-0.2.4/
--rw-r--r--   0 vasiliy   (1000) vasiliy   (1000)      801 2024-03-28 14:59:49.430566 aeronet_vector-0.2.4/PKG-INFO
--rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)     2371 2024-03-28 14:57:48.000000 aeronet_vector-0.2.4/README.rst
-drwxrwxr-x   0 vasiliy   (1000) vasiliy   (1000)        0 2024-03-28 14:59:49.426566 aeronet_vector-0.2.4/aeronet_vector/
--rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)       78 2024-03-28 14:57:48.000000 aeronet_vector-0.2.4/aeronet_vector/__init__.py
--rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)       63 2024-03-28 14:57:48.000000 aeronet_vector-0.2.4/aeronet_vector/__version__.py
--rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)     6538 2024-03-28 14:57:48.000000 aeronet_vector-0.2.4/aeronet_vector/feature.py
--rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)    12347 2024-03-28 14:57:48.000000 aeronet_vector-0.2.4/aeronet_vector/featurecollection.py
--rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)     1009 2024-03-28 14:57:48.000000 aeronet_vector-0.2.4/aeronet_vector/merge.py
--rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)     1030 2024-03-28 14:57:48.000000 aeronet_vector-0.2.4/aeronet_vector/utils.py
-drwxrwxr-x   0 vasiliy   (1000) vasiliy   (1000)        0 2024-03-28 14:59:49.426566 aeronet_vector-0.2.4/aeronet_vector.egg-info/
--rw-r--r--   0 vasiliy   (1000) vasiliy   (1000)      801 2024-03-28 14:59:49.000000 aeronet_vector-0.2.4/aeronet_vector.egg-info/PKG-INFO
--rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)      375 2024-03-28 14:59:49.000000 aeronet_vector-0.2.4/aeronet_vector.egg-info/SOURCES.txt
--rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)        1 2024-03-28 14:59:49.000000 aeronet_vector-0.2.4/aeronet_vector.egg-info/dependency_links.txt
--rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)       63 2024-03-28 14:59:49.000000 aeronet_vector-0.2.4/aeronet_vector.egg-info/requires.txt
--rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)       15 2024-03-28 14:59:49.000000 aeronet_vector-0.2.4/aeronet_vector.egg-info/top_level.txt
--rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)       38 2024-03-28 14:59:49.430566 aeronet_vector-0.2.4/setup.cfg
--rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)     3780 2024-03-28 14:57:48.000000 aeronet_vector-0.2.4/setup.py
+drwxrwxr-x   0 vasiliy   (1000) vasiliy   (1000)        0 2024-04-02 15:39:56.966286 aeronet_vector-0.2.5/
+-rw-r--r--   0 vasiliy   (1000) vasiliy   (1000)      801 2024-04-02 15:39:56.966286 aeronet_vector-0.2.5/PKG-INFO
+-rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)     2371 2024-03-28 14:57:48.000000 aeronet_vector-0.2.5/README.rst
+drwxrwxr-x   0 vasiliy   (1000) vasiliy   (1000)        0 2024-04-02 15:39:56.966286 aeronet_vector-0.2.5/aeronet_vector/
+-rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)       78 2024-03-28 14:57:48.000000 aeronet_vector-0.2.5/aeronet_vector/__init__.py
+-rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)       63 2024-04-02 15:25:28.000000 aeronet_vector-0.2.5/aeronet_vector/__version__.py
+-rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)     6540 2024-04-02 15:25:28.000000 aeronet_vector-0.2.5/aeronet_vector/feature.py
+-rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)    12351 2024-04-02 15:25:28.000000 aeronet_vector-0.2.5/aeronet_vector/featurecollection.py
+-rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)     1009 2024-03-28 14:57:48.000000 aeronet_vector-0.2.5/aeronet_vector/merge.py
+-rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)     1030 2024-03-28 14:57:48.000000 aeronet_vector-0.2.5/aeronet_vector/utils.py
+drwxrwxr-x   0 vasiliy   (1000) vasiliy   (1000)        0 2024-04-02 15:39:56.966286 aeronet_vector-0.2.5/aeronet_vector.egg-info/
+-rw-r--r--   0 vasiliy   (1000) vasiliy   (1000)      801 2024-04-02 15:39:56.000000 aeronet_vector-0.2.5/aeronet_vector.egg-info/PKG-INFO
+-rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)      375 2024-04-02 15:39:56.000000 aeronet_vector-0.2.5/aeronet_vector.egg-info/SOURCES.txt
+-rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)        1 2024-04-02 15:39:56.000000 aeronet_vector-0.2.5/aeronet_vector.egg-info/dependency_links.txt
+-rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)       63 2024-04-02 15:39:56.000000 aeronet_vector-0.2.5/aeronet_vector.egg-info/requires.txt
+-rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)       15 2024-04-02 15:39:56.000000 aeronet_vector-0.2.5/aeronet_vector.egg-info/top_level.txt
+-rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)       38 2024-04-02 15:39:56.966286 aeronet_vector-0.2.5/setup.cfg
+-rw-rw-r--   0 vasiliy   (1000) vasiliy   (1000)     3780 2024-03-28 14:57:48.000000 aeronet_vector-0.2.5/setup.py
```

### Comparing `aeronet_vector-0.2.4/PKG-INFO` & `aeronet_vector-0.2.5/aeronet_vector.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: aeronet_vector
-Version: 0.2.4
+Name: aeronet-vector
+Version: 0.2.5
 Summary: Vector operations for aeronetlib. Based on shapely + r-tree indexing
 Home-page: 
 Author: Geoalert
 Author-email: hello@geoalert.io
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `aeronet_vector-0.2.4/README.rst` & `aeronet_vector-0.2.5/README.rst`

 * *Files identical despite different names*

### Comparing `aeronet_vector-0.2.4/aeronet_vector/feature.py` & `aeronet_vector-0.2.5/aeronet_vector/feature.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,27 +145,27 @@
         dst_crs = utm_zone((lat1 + lat2)/2, (lon1 + lon2)/2)
         return self.reproject(dst_crs)
 
     def copy(self):
         """Returns a copy of feature"""
         return Feature(shape(self.geometry), {k: v for k, v in self.properties.items()}, self.crs)
 
-    def simplify(self, tolerance: float, inplace: bool = True):
+    def simplify(self, tolerance: float, inplace: bool = False):
         """Simplifies geometry with Douglas-Pecker
         Args:
             tolerance (float): simplification tolerance
             inplace (bool): if True modifies Feature inplace, else returns new Feature
         Returns:
             new Feature if inplace, else None"""
         if inplace:
             self._geometry = self._geometry.simplify(tolerance)
         else:
             return self.copy().simplify(tolerance, inplace=True)
 
-    def cast_property_to(self, key: str, new_type: type, inplace: bool = True):
+    def cast_property_to(self, key: str, new_type: type, inplace: bool = False):
         """Casts property to new type (e.g. str to int)
         Args:
             key (str): key of modified property
             new_type (bool): type to cast to
             inplace (bool): if True modifies Feature inplace, else returns new Feature
         Returns:
             new Feature if inplace, else None"""
```

### Comparing `aeronet_vector-0.2.4/aeronet_vector/featurecollection.py` & `aeronet_vector-0.2.5/aeronet_vector/featurecollection.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,29 +44,29 @@
             if not f.geometry.get('coordinates'):  # remove possible empty shapes
                 warnings.warn('Empty geometry detected. This geometry has been removed from collection.',
                               RuntimeWarning)
             else:
                 valid_features.append(f)
         return valid_features
 
-    def apply(self,  func: Callable, inplace: bool = True):
+    def apply(self,  func: Callable, inplace: bool = False):
         """Applies function to collection geometries
         Args:
             func (Callable): function to apply
             inplace (bool): if True modifies collection inplace, else returns new collection
         Returns:
             new FeatureCollection if inplace, else None
         """
         if inplace:
             for f in self.features:
                 f.apply(func, True)
         else:
             return FeatureCollection([f.apply(func) for f in self.features], crs=self.crs)
 
-    def filter(self, func: Callable, inplace: bool = True):
+    def filter(self, func: Callable, inplace: bool = False):
         """Filters collection according to func
         Args:
             func (Callable): filtering function
             inplace (bool): if True modifies collection inplace, else returns new collection
         Returns:
             new FeatureCollection if inplace, else None
         """
@@ -276,28 +276,28 @@
         """
         return self.reproject(dst_crs='utm')
 
     def copy(self):
         """Returns a copy of collection"""
         return FeatureCollection((f.copy() for f in self.features), crs=self.crs)
 
-    def simplify(self, tolerance: float, inplace: bool = True):
+    def simplify(self, tolerance: float, inplace: bool = False):
         """Simplifies geometries with Douglas-Pecker
         Args:
             tolerance (float): simplification tolerance
             inplace (bool): if True modifies Feature inplace, else returns new Feature
         Returns:
             FeatureCollection if inplace, else None"""
         if inplace:
             for f in self.features:
                 f.simplify(tolerance, inplace=True)
         else:
             return self.copy().simplify(tolerance, inplace=True)
 
-    def cast_property_to(self, key: str, new_type: type, inplace: bool = True):
+    def cast_property_to(self, key: str, new_type: type, inplace: bool = False):
         """Casts property to new type (e.g. str to int)
         Args:
             key (str): key of modified property
             new_type (bool): type to cast to
             inplace (bool): if True modifies Feature inplace, else returns new Feature
         Returns:
             FeatureCollection if inplace, else None"""
```

### Comparing `aeronet_vector-0.2.4/aeronet_vector/merge.py` & `aeronet_vector-0.2.5/aeronet_vector/merge.py`

 * *Files identical despite different names*

### Comparing `aeronet_vector-0.2.4/aeronet_vector/utils.py` & `aeronet_vector-0.2.5/aeronet_vector/utils.py`

 * *Files identical despite different names*

### Comparing `aeronet_vector-0.2.4/aeronet_vector.egg-info/PKG-INFO` & `aeronet_vector-0.2.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: aeronet-vector
-Version: 0.2.4
+Name: aeronet_vector
+Version: 0.2.5
 Summary: Vector operations for aeronetlib. Based on shapely + r-tree indexing
 Home-page: 
 Author: Geoalert
 Author-email: hello@geoalert.io
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `aeronet_vector-0.2.4/setup.py` & `aeronet_vector-0.2.5/setup.py`

 * *Files identical despite different names*

