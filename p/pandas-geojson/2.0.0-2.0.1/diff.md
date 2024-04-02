# Comparing `tmp/pandas_geojson-2.0.0.tar.gz` & `tmp/pandas_geojson-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandas_geojson-2.0.0.tar", last modified: Mon Mar 18 21:57:22 2024, max compression
+gzip compressed data, was "pandas_geojson-2.0.1.tar", last modified: Tue Apr  2 03:02:39 2024, max compression
```

## Comparing `pandas_geojson-2.0.0.tar` & `pandas_geojson-2.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-03-18 21:57:22.083388 pandas_geojson-2.0.0/
--rw-rw-rw-   0        0        0     1097 2024-03-18 19:56:01.000000 pandas_geojson-2.0.0/LICENSE
--rw-rw-rw-   0        0        0    53082 2024-03-18 21:57:22.082390 pandas_geojson-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0    52649 2024-03-18 19:56:01.000000 pandas_geojson-2.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-03-18 21:57:22.059382 pandas_geojson-2.0.0/pandas_geojson/
--rw-rw-rw-   0        0        0      280 2024-03-18 19:56:01.000000 pandas_geojson-2.0.0/pandas_geojson/__init__.py
--rw-rw-rw-   0        0        0     3146 2024-03-18 19:56:01.000000 pandas_geojson-2.0.0/pandas_geojson/core.py
--rw-rw-rw-   0        0        0      645 2024-03-18 19:56:01.000000 pandas_geojson-2.0.0/pandas_geojson/io.py
-drwxrwxrwx   0        0        0        0 2024-03-18 21:57:22.080389 pandas_geojson-2.0.0/pandas_geojson.egg-info/
--rw-rw-rw-   0        0        0    53082 2024-03-18 21:57:22.000000 pandas_geojson-2.0.0/pandas_geojson.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      286 2024-03-18 21:57:22.000000 pandas_geojson-2.0.0/pandas_geojson.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-18 21:57:22.000000 pandas_geojson-2.0.0/pandas_geojson.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-03-18 21:57:22.000000 pandas_geojson-2.0.0/pandas_geojson.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-03-18 21:57:22.000000 pandas_geojson-2.0.0/pandas_geojson.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-18 21:57:22.084389 pandas_geojson-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0      823 2024-03-18 21:57:05.000000 pandas_geojson-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 03:02:39.262102 pandas_geojson-2.0.1/
+-rw-rw-rw-   0        0        0     1097 2024-03-18 19:56:01.000000 pandas_geojson-2.0.1/LICENSE
+-rw-rw-rw-   0        0        0    53377 2024-04-02 03:02:39.261104 pandas_geojson-2.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0    52944 2024-03-27 02:11:25.000000 pandas_geojson-2.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 03:02:39.227433 pandas_geojson-2.0.1/pandas_geojson/
+-rw-rw-rw-   0        0        0      280 2024-04-02 03:02:09.000000 pandas_geojson-2.0.1/pandas_geojson/__init__.py
+-rw-rw-rw-   0        0        0     3347 2024-04-02 02:59:27.000000 pandas_geojson-2.0.1/pandas_geojson/core.py
+-rw-rw-rw-   0        0        0      645 2024-03-18 19:56:01.000000 pandas_geojson-2.0.1/pandas_geojson/io.py
+drwxrwxrwx   0        0        0        0 2024-04-02 03:02:39.259104 pandas_geojson-2.0.1/pandas_geojson.egg-info/
+-rw-rw-rw-   0        0        0    53377 2024-04-02 03:02:39.000000 pandas_geojson-2.0.1/pandas_geojson.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      286 2024-04-02 03:02:39.000000 pandas_geojson-2.0.1/pandas_geojson.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 03:02:39.000000 pandas_geojson-2.0.1/pandas_geojson.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-02 03:02:39.000000 pandas_geojson-2.0.1/pandas_geojson.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-02 03:02:39.000000 pandas_geojson-2.0.1/pandas_geojson.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-02 03:02:39.262102 pandas_geojson-2.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      823 2024-04-02 03:01:31.000000 pandas_geojson-2.0.1/setup.py
```

### Comparing `pandas_geojson-2.0.0/LICENSE` & `pandas_geojson-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pandas_geojson-2.0.0/PKG-INFO` & `pandas_geojson-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 Metadata-Version: 2.1
 Name: pandas_geojson
-Version: 2.0.0
+Version: 2.0.1
 Summary: Convert Pandas Dataframe to GeoJSON
 Home-page: https://github.com/jrasband-dev/pandas-geojson
 Author: Jayden Rasband
 Author-email: jayden.rasband@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas
 
 ![](https://raw.githubusercontent.com/jrasband-dev/pandas-geojson/master/static/pandasgeojson.png)
 
 ---
+![PyPI - Version](https://img.shields.io/pypi/v/pandas-geojson)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/pandas-geojson)
+![PyPI - License](https://img.shields.io/pypi/l/pandas-geojson)
+![Libraries.io SourceRank](https://img.shields.io/librariesio/sourcerank/pypi/pandas-geojson)
+
 
 # Getting Started
 Install the latest version of pandas-geojson using pip.
 ```
 pip install pandas-geojson
 ```
```

#### html2text {}

```diff
@@ -1,14 +1,18 @@
-Metadata-Version: 2.1 Name: pandas_geojson Version: 2.0.0 Summary: Convert
+Metadata-Version: 2.1 Name: pandas_geojson Version: 2.0.1 Summary: Convert
 Pandas Dataframe to GeoJSON Home-page: https://github.com/jrasband-dev/pandas-
 geojson Author: Jayden Rasband Author-email: jayden.rasband@gmail.com License:
 MIT Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: pandas ![](https://raw.githubusercontent.com/jrasband-
-dev/pandas-geojson/master/static/pandasgeojson.png) --- # Getting Started
+dev/pandas-geojson/master/static/pandasgeojson.png) --- ![PyPI - Version]
+(https://img.shields.io/pypi/v/pandas-geojson) ![PyPI - Downloads](https://
+img.shields.io/pypi/dm/pandas-geojson) ![PyPI - License](https://
+img.shields.io/pypi/l/pandas-geojson) ![Libraries.io SourceRank](https://
+img.shields.io/librariesio/sourcerank/pypi/pandas-geojson) # Getting Started
 Install the latest version of pandas-geojson using pip. ``` pip install pandas-
 geojson ``` ## Open GeoJSON Files Using the `read_geojson` function, you can
 easily read in GeoJSON data int the GeoJSON object. ```python import
 pandas_geojson as pdg geojson = pdg.read_geojson('datasets/
 National_Obesity_By_State.geojson') type(geojson) ```
 pandas_geojson.core.GeoJSON ## List Properties Pandas-GeoJSON utilizes
 properties to filter large geojson files. This functionallity helps you
```

### Comparing `pandas_geojson-2.0.0/README.md` & `pandas_geojson-2.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 ![](https://raw.githubusercontent.com/jrasband-dev/pandas-geojson/master/static/pandasgeojson.png)
 
 ---
+![PyPI - Version](https://img.shields.io/pypi/v/pandas-geojson)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/pandas-geojson)
+![PyPI - License](https://img.shields.io/pypi/l/pandas-geojson)
+![Libraries.io SourceRank](https://img.shields.io/librariesio/sourcerank/pypi/pandas-geojson)
+
 
 # Getting Started
 Install the latest version of pandas-geojson using pip.
 ```
 pip install pandas-geojson
 ```
```

#### html2text {}

```diff
@@ -1,14 +1,18 @@
 ![](https://raw.githubusercontent.com/jrasband-dev/pandas-geojson/master/
-static/pandasgeojson.png) --- # Getting Started Install the latest version of
-pandas-geojson using pip. ``` pip install pandas-geojson ``` ## Open GeoJSON
-Files Using the `read_geojson` function, you can easily read in GeoJSON data
-int the GeoJSON object. ```python import pandas_geojson as pdg geojson =
-pdg.read_geojson('datasets/National_Obesity_By_State.geojson') type(geojson)
-``` pandas_geojson.core.GeoJSON ## List Properties Pandas-GeoJSON utilizes
+static/pandasgeojson.png) --- ![PyPI - Version](https://img.shields.io/pypi/v/
+pandas-geojson) ![PyPI - Downloads](https://img.shields.io/pypi/dm/pandas-
+geojson) ![PyPI - License](https://img.shields.io/pypi/l/pandas-geojson) !
+[Libraries.io SourceRank](https://img.shields.io/librariesio/sourcerank/pypi/
+pandas-geojson) # Getting Started Install the latest version of pandas-geojson
+using pip. ``` pip install pandas-geojson ``` ## Open GeoJSON Files Using the
+`read_geojson` function, you can easily read in GeoJSON data int the GeoJSON
+object. ```python import pandas_geojson as pdg geojson = pdg.read_geojson
+('datasets/National_Obesity_By_State.geojson') type(geojson) ```
+pandas_geojson.core.GeoJSON ## List Properties Pandas-GeoJSON utilizes
 properties to filter large geojson files. This functionallity helps you
 identify all of the properties in the geojson file so that you can choose a
 filter criteria. For more on filtering see [filter_geojson](#filter-geojson)
 ```python geojson.get_properties() ``` ['FID', 'NAME', 'Obesity',
 'SHAPE_Length', 'SHAPE_Area'] ## DataFrame to GeoJSON Pandas-GeoJSON makes it
 easy to convert a dataframe with coordinates into a GeoJSON object. Your
 DataFrame **must** contain at least two columns with the following information:
```

### Comparing `pandas_geojson-2.0.0/pandas_geojson/core.py` & `pandas_geojson-2.0.1/pandas_geojson/core.py`

 * *Files 13% similar despite different names*

```diff
@@ -44,15 +44,19 @@
         '''
         filtered_features = [feature for feature in self.features if feature.properties.get(property_key) in property_values]
         return GeoJSON(type='FeatureCollection', features=filtered_features)
     
 
     @classmethod
     def from_dict(cls, data):
-        features = [GeoJSONFeature(**feature) for feature in data['features']]
+        features = []
+        for feature_data in data['features']:
+            properties = feature_data.get('properties', {})
+            feature = GeoJSONFeature(type='Feature', geometry=feature_data['geometry'], properties=properties)
+            features.append(feature)
         return cls(type=data['type'], features=features)
     
     @classmethod
     def from_dataframe(cls
                        ,df
                        ,geometry_type_col: str = 'geometry.type'
                        ,coordinate_col: str = 'geometry.coordinates'
```

### Comparing `pandas_geojson-2.0.0/pandas_geojson/io.py` & `pandas_geojson-2.0.1/pandas_geojson/io.py`

 * *Files identical despite different names*

### Comparing `pandas_geojson-2.0.0/pandas_geojson.egg-info/PKG-INFO` & `pandas_geojson-2.0.1/pandas_geojson.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 Metadata-Version: 2.1
 Name: pandas_geojson
-Version: 2.0.0
+Version: 2.0.1
 Summary: Convert Pandas Dataframe to GeoJSON
 Home-page: https://github.com/jrasband-dev/pandas-geojson
 Author: Jayden Rasband
 Author-email: jayden.rasband@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas
 
 ![](https://raw.githubusercontent.com/jrasband-dev/pandas-geojson/master/static/pandasgeojson.png)
 
 ---
+![PyPI - Version](https://img.shields.io/pypi/v/pandas-geojson)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/pandas-geojson)
+![PyPI - License](https://img.shields.io/pypi/l/pandas-geojson)
+![Libraries.io SourceRank](https://img.shields.io/librariesio/sourcerank/pypi/pandas-geojson)
+
 
 # Getting Started
 Install the latest version of pandas-geojson using pip.
 ```
 pip install pandas-geojson
 ```
```

#### html2text {}

```diff
@@ -1,14 +1,18 @@
-Metadata-Version: 2.1 Name: pandas_geojson Version: 2.0.0 Summary: Convert
+Metadata-Version: 2.1 Name: pandas_geojson Version: 2.0.1 Summary: Convert
 Pandas Dataframe to GeoJSON Home-page: https://github.com/jrasband-dev/pandas-
 geojson Author: Jayden Rasband Author-email: jayden.rasband@gmail.com License:
 MIT Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: pandas ![](https://raw.githubusercontent.com/jrasband-
-dev/pandas-geojson/master/static/pandasgeojson.png) --- # Getting Started
+dev/pandas-geojson/master/static/pandasgeojson.png) --- ![PyPI - Version]
+(https://img.shields.io/pypi/v/pandas-geojson) ![PyPI - Downloads](https://
+img.shields.io/pypi/dm/pandas-geojson) ![PyPI - License](https://
+img.shields.io/pypi/l/pandas-geojson) ![Libraries.io SourceRank](https://
+img.shields.io/librariesio/sourcerank/pypi/pandas-geojson) # Getting Started
 Install the latest version of pandas-geojson using pip. ``` pip install pandas-
 geojson ``` ## Open GeoJSON Files Using the `read_geojson` function, you can
 easily read in GeoJSON data int the GeoJSON object. ```python import
 pandas_geojson as pdg geojson = pdg.read_geojson('datasets/
 National_Obesity_By_State.geojson') type(geojson) ```
 pandas_geojson.core.GeoJSON ## List Properties Pandas-GeoJSON utilizes
 properties to filter large geojson files. This functionallity helps you
```

### Comparing `pandas_geojson-2.0.0/setup.py` & `pandas_geojson-2.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="pandas_geojson",
-    version="2.0.0",
+    version="2.0.1",
     description="Convert Pandas Dataframe to GeoJSON",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/jrasband-dev/pandas-geojson",
     author="Jayden Rasband",
     author_email="jayden.rasband@gmail.com",
     license="MIT",
```

