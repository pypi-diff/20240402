# Comparing `tmp/rrcgeoviz-0.1.1.tar.gz` & `tmp/rrcgeoviz-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rrcgeoviz-0.1.1.tar", last modified: Thu Mar 21 06:06:31 2024, max compression
+gzip compressed data, was "rrcgeoviz-0.1.2.tar", last modified: Tue Apr  2 04:49:37 2024, max compression
```

## Comparing `rrcgeoviz-0.1.1.tar` & `rrcgeoviz-0.1.2.tar`

### file list

```diff
@@ -1,47 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 06:06:31.685761 rrcgeoviz-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     4718 2024-03-21 06:06:31.685761 rrcgeoviz-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-03-21 06:06:18.000000 rrcgeoviz-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-03-21 06:06:18.000000 rrcgeoviz-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-03-21 06:06:18.000000 rrcgeoviz-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-21 06:06:31.685761 rrcgeoviz-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 06:06:31.681760 rrcgeoviz-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 06:06:31.681760 rrcgeoviz-0.1.1/src/rrcgeoviz/
--rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-03-21 06:06:18.000000 rrcgeoviz-0.1.1/src/rrcgeoviz/GeneratedData.py
--rw-r--r--   0 runner    (1001) docker     (127)     7833 2024-03-21 06:06:18.000000 rrcgeoviz-0.1.1/src/rrcgeoviz/GeoVizPanelDashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     4945 2024-03-21 06:06:18.000000 rrcgeoviz-0.1.1/src/rrcgeoviz/JavaCreator.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 06:06:18.000000 rrcgeoviz-0.1.1/src/rrcgeoviz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-03-21 06:06:18.000000 rrcgeoviz-0.1.1/src/rrcgeoviz/arguments.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 06:06:31.681760 rrcgeoviz-0.1.1/src/rrcgeoviz/datagenerators/
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-03-21 06:06:18.000000 rrcgeoviz-0.1.1/src/rrcgeoviz/datagenerators/GeneratorBertopic.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-03-21 06:06:18.000000 rrcgeoviz-0.1.1/src/rrcgeoviz/datagenerators/GeneratorExample.py
--rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-03-21 06:06:18.000000 rrcgeoviz-0.1.1/src/rrcgeoviz/datagenerators/GeneratorPOI.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-03-21 06:06:18.000000 rrcgeoviz-0.1.1/src/rrcgeoviz/datagenerators/ParentDataGenerator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 06:06:31.681760 rrcgeoviz-0.1.1/src/rrcgeoviz/datagenerators/data/
--rw-r--r--   0 runner    (1001) docker     (127)    44894 2024-03-21 06:06:18.000000 rrcgeoviz-0.1.1/src/rrcgeoviz/datagenerators/data/ports.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 06:06:31.685761 rrcgeoviz-0.1.1/src/rrcgeoviz/features/
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-03-21 06:06:18.000000 rrcgeoviz-0.1.1/src/rrcgeoviz/features/Downloadables.py
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-03-21 06:06:18.000000 rrcgeoviz-0.1.1/src/rrcgeoviz/features/FeartureDataFrameEditor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-03-21 06:06:18.000000 rrcgeoviz-0.1.1/src/rrcgeoviz/features/FeatureAllMonths.py
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-03-21 06:06:18.000000 rrcgeoviz-0.1.1/src/rrcgeoviz/features/FeatureBertopic.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-03-21 06:06:18.000000 rrcgeoviz-0.1.1/src/rrcgeoviz/features/FeatureHeatmap.py
--rw-r--r--   0 runner    (1001) docker     (127)     4166 2024-03-21 06:06:18.000000 rrcgeoviz-0.1.1/src/rrcgeoviz/features/FeatureOneYear.py
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-03-21 06:06:18.000000 rrcgeoviz-0.1.1/src/rrcgeoviz/features/FeatureOneYearMonths.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-03-21 06:06:18.000000 rrcgeoviz-0.1.1/src/rrcgeoviz/features/FeaturePOI.py
--rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-03-21 06:06:18.000000 rrcgeoviz-0.1.1/src/rrcgeoviz/features/FeatureSearch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-03-21 06:06:18.000000 rrcgeoviz-0.1.1/src/rrcgeoviz/features/FeatureThreeD.py
--rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-03-21 06:06:18.000000 rrcgeoviz-0.1.1/src/rrcgeoviz/features/FeatureYearlyRange.py
--rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-03-21 06:06:18.000000 rrcgeoviz-0.1.1/src/rrcgeoviz/features/ParentGeovizFeature.py
--rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-03-21 06:06:18.000000 rrcgeoviz-0.1.1/src/rrcgeoviz/features/VisualizeBert.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-03-21 06:06:18.000000 rrcgeoviz-0.1.1/src/rrcgeoviz/geoviz_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 06:06:31.685761 rrcgeoviz-0.1.1/src/rrcgeoviz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4718 2024-03-21 06:06:31.000000 rrcgeoviz-0.1.1/src/rrcgeoviz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-03-21 06:06:31.000000 rrcgeoviz-0.1.1/src/rrcgeoviz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 06:06:31.000000 rrcgeoviz-0.1.1/src/rrcgeoviz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-21 06:06:31.000000 rrcgeoviz-0.1.1/src/rrcgeoviz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-03-21 06:06:31.000000 rrcgeoviz-0.1.1/src/rrcgeoviz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-21 06:06:31.000000 rrcgeoviz-0.1.1/src/rrcgeoviz.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 06:06:31.685761 rrcgeoviz-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-03-21 06:06:18.000000 rrcgeoviz-0.1.1/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     9094 2024-03-21 06:06:18.000000 rrcgeoviz-0.1.1/tests/test_caching.py
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-03-21 06:06:18.000000 rrcgeoviz-0.1.1/tests/test_weird_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-03-21 06:06:18.000000 rrcgeoviz-0.1.1/tests/test_weird_options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:49:37.483479 rrcgeoviz-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     4718 2024-04-02 04:49:37.483479 rrcgeoviz-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 04:49:37.483479 rrcgeoviz-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:49:37.471479 rrcgeoviz-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:49:37.475479 rrcgeoviz-0.1.2/src/rrcgeoviz/
+-rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/GeneratedData.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7833 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/GeoVizPanelDashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/JsonCreator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:49:37.471479 rrcgeoviz-0.1.2/src/rrcgeoviz/JsonCreatorClasses/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:49:37.475479 rrcgeoviz-0.1.2/src/rrcgeoviz/JsonCreatorClasses/Blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/JsonCreatorClasses/Blocks/ArrayTextBox.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/JsonCreatorClasses/Blocks/BaseBlock.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/JsonCreatorClasses/Blocks/DownloadButton.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/JsonCreatorClasses/Blocks/ImageCheckbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/JsonCreatorClasses/Blocks/TextBox.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/JsonCreatorClasses/Blocks/Toggle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:49:37.479479 rrcgeoviz-0.1.2/src/rrcgeoviz/JsonCreatorClasses/Sections/
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/JsonCreatorClasses/Sections/BaseSection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/JsonCreatorClasses/Sections/CacheSetter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/JsonCreatorClasses/Sections/ColumnSetter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/JsonCreatorClasses/Sections/DownloadSection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/JsonCreatorClasses/Sections/FeatureCustomizationsSetter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/JsonCreatorClasses/Sections/FeatureSetter.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/arguments.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:49:37.479479 rrcgeoviz-0.1.2/src/rrcgeoviz/datagenerators/
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/datagenerators/GeneratorBertopic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/datagenerators/GeneratorExample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/datagenerators/GeneratorPOI.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/datagenerators/ParentDataGenerator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:49:37.479479 rrcgeoviz-0.1.2/src/rrcgeoviz/datagenerators/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    44894 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/datagenerators/data/ports.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:49:37.483479 rrcgeoviz-0.1.2/src/rrcgeoviz/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/features/Downloadables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/features/FeartureDataFrameEditor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/features/FeatureAllMonths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/features/FeatureBertopic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/features/FeatureHeatmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4166 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/features/FeatureOneYear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/features/FeatureOneYearMonths.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/features/FeaturePOI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/features/FeatureSearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/features/FeatureThreeD.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/features/FeatureYearlyRange.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/features/ParentGeovizFeature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/features/VisualizeBert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/src/rrcgeoviz/geoviz_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:49:37.483479 rrcgeoviz-0.1.2/src/rrcgeoviz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4718 2024-04-02 04:49:37.000000 rrcgeoviz-0.1.2/src/rrcgeoviz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-04-02 04:49:37.000000 rrcgeoviz-0.1.2/src/rrcgeoviz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 04:49:37.000000 rrcgeoviz-0.1.2/src/rrcgeoviz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-02 04:49:37.000000 rrcgeoviz-0.1.2/src/rrcgeoviz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-02 04:49:37.000000 rrcgeoviz-0.1.2/src/rrcgeoviz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-02 04:49:37.000000 rrcgeoviz-0.1.2/src/rrcgeoviz.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 04:49:37.483479 rrcgeoviz-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-04-02 04:49:31.000000 rrcgeoviz-0.1.2/tests/test_arguments.py
```

### Comparing `rrcgeoviz-0.1.1/PKG-INFO` & `rrcgeoviz-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rrcgeoviz
-Version: 0.1.1
+Version: 0.1.2
 Summary: EDA tool for spatio-temporal data
 Author-email: Jonas Nielsen <bobthebuilder.chfi@gmail.com>, Daniel Millward <dfmillward02@gmail.com>, Stephen Tveten  <stveten@student.byu.edu>
 Project-URL: Documentation, https://rincon-geoviz.readthedocs.io/en/latest/index.html
 Project-URL: Homepage, https://github.com/rrc-byu/ds-capstone-2023-2024
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: ydata-profiling==4.6.2
```

### Comparing `rrcgeoviz-0.1.1/README.md` & `rrcgeoviz-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.1/pyproject.toml` & `rrcgeoviz-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.1/src/rrcgeoviz/GeneratedData.py` & `rrcgeoviz-0.1.2/src/rrcgeoviz/GeneratedData.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         return self.data_dict
 
     # arguments.generated_data.data_dict["generator_bertopic"]
     def _setLocation(self):
         if "cache_location" in self.arguments.getCaching():
             return self.arguments.getCaching()["cache_location"]
         else:
-            return "./.geovizcache"
+            return os.path.join(os.path.curdir, ".geovizcache")
 
     def _setShouldCache(self):
         if (
             "cache_results" in self.arguments.getCaching()
             and self.arguments.getCaching()["cache_results"] == True
         ):
             Path(self.location).mkdir(parents=True, exist_ok=True)
```

### Comparing `rrcgeoviz-0.1.1/src/rrcgeoviz/GeoVizPanelDashboard.py` & `rrcgeoviz-0.1.2/src/rrcgeoviz/GeoVizPanelDashboard.py`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.1/src/rrcgeoviz/datagenerators/GeneratorBertopic.py` & `rrcgeoviz-0.1.2/src/rrcgeoviz/datagenerators/GeneratorBertopic.py`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.1/src/rrcgeoviz/datagenerators/GeneratorPOI.py` & `rrcgeoviz-0.1.2/src/rrcgeoviz/datagenerators/GeneratorPOI.py`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.1/src/rrcgeoviz/datagenerators/ParentDataGenerator.py` & `rrcgeoviz-0.1.2/src/rrcgeoviz/datagenerators/ParentDataGenerator.py`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.1/src/rrcgeoviz/datagenerators/data/ports.csv` & `rrcgeoviz-0.1.2/src/rrcgeoviz/datagenerators/data/ports.csv`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.1/src/rrcgeoviz/features/Downloadables.py` & `rrcgeoviz-0.1.2/src/rrcgeoviz/features/Downloadables.py`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.1/src/rrcgeoviz/features/FeatureAllMonths.py` & `rrcgeoviz-0.1.2/src/rrcgeoviz/features/FeatureAllMonths.py`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.1/src/rrcgeoviz/features/FeatureBertopic.py` & `rrcgeoviz-0.1.2/src/rrcgeoviz/features/FeatureBertopic.py`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.1/src/rrcgeoviz/features/FeatureHeatmap.py` & `rrcgeoviz-0.1.2/src/rrcgeoviz/features/FeatureHeatmap.py`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.1/src/rrcgeoviz/features/FeatureOneYear.py` & `rrcgeoviz-0.1.2/src/rrcgeoviz/features/FeatureOneYear.py`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.1/src/rrcgeoviz/features/FeatureOneYearMonths.py` & `rrcgeoviz-0.1.2/src/rrcgeoviz/features/FeatureOneYearMonths.py`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.1/src/rrcgeoviz/features/FeaturePOI.py` & `rrcgeoviz-0.1.2/src/rrcgeoviz/features/FeaturePOI.py`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.1/src/rrcgeoviz/features/FeatureSearch.py` & `rrcgeoviz-0.1.2/src/rrcgeoviz/features/FeatureSearch.py`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.1/src/rrcgeoviz/features/FeatureThreeD.py` & `rrcgeoviz-0.1.2/src/rrcgeoviz/features/FeatureThreeD.py`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.1/src/rrcgeoviz/features/FeatureYearlyRange.py` & `rrcgeoviz-0.1.2/src/rrcgeoviz/features/FeatureYearlyRange.py`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.1/src/rrcgeoviz/features/ParentGeovizFeature.py` & `rrcgeoviz-0.1.2/src/rrcgeoviz/features/ParentGeovizFeature.py`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.1/src/rrcgeoviz/features/VisualizeBert.py` & `rrcgeoviz-0.1.2/src/rrcgeoviz/features/VisualizeBert.py`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.1/src/rrcgeoviz/geoviz_cli.py` & `rrcgeoviz-0.1.2/src/rrcgeoviz/geoviz_cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import json
 import subprocess
 import argparse
 import sys
 import pandas as pd
 from pandas.errors import EmptyDataError
-from rrcgeoviz.GeoVizPanelDashboard import GeoVizPanelDashboard
 
 from rrcgeoviz.arguments import Arguments
 
-from rrcgeoviz.GeneratedData import GeneratedData
+from rrcgeoviz.JsonCreator import main_javacreator
+
 
 # https://docs.python.org/3/library/argparse.html#action
 
 PARSER_ARGUMENTS = [
     {
         "name": "data",
         "metavar": "csvfilepath",
@@ -50,26 +50,34 @@
                 help=argument["help"],
                 action=argument["action"],
             )
     return parser
 
 
 def main(argv=None):
+    if (argv is not None and "--init" in argv) or "--init" in sys.argv:
+        main_javacreator()
+        sys.exit()
+
     """argv is an array of strings, simulating command line arguments"""
     parser = argparse.ArgumentParser(
         description="Command-Line Interface for GeoViz Project"
     )
     parser = addParserArguments(parser)
     args = parser.parse_args(argv)
     arguments = Arguments(args.data, args.options)
 
     if args.test:
         print("Testing mode enabled")
 
+    from rrcgeoviz.GeneratedData import GeneratedData
+
     arguments.generated_data = GeneratedData(arguments)
+    from rrcgeoviz.GeoVizPanelDashboard import GeoVizPanelDashboard
+
     dashboard = GeoVizPanelDashboard(args=arguments, test=args.test)
 
     if not args.test:
         dashboard.render()
 
 
 if __name__ == "__main__":
```

### Comparing `rrcgeoviz-0.1.1/src/rrcgeoviz.egg-info/PKG-INFO` & `rrcgeoviz-0.1.2/src/rrcgeoviz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rrcgeoviz
-Version: 0.1.1
+Version: 0.1.2
 Summary: EDA tool for spatio-temporal data
 Author-email: Jonas Nielsen <bobthebuilder.chfi@gmail.com>, Daniel Millward <dfmillward02@gmail.com>, Stephen Tveten  <stveten@student.byu.edu>
 Project-URL: Documentation, https://rincon-geoviz.readthedocs.io/en/latest/index.html
 Project-URL: Homepage, https://github.com/rrc-byu/ds-capstone-2023-2024
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: ydata-profiling==4.6.2
```

### Comparing `rrcgeoviz-0.1.1/src/rrcgeoviz.egg-info/SOURCES.txt` & `rrcgeoviz-0.1.2/src/rrcgeoviz.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,34 @@
 README.md
 pyproject.toml
 requirements.txt
 src/rrcgeoviz/GeneratedData.py
 src/rrcgeoviz/GeoVizPanelDashboard.py
-src/rrcgeoviz/JavaCreator.py
+src/rrcgeoviz/JsonCreator.py
 src/rrcgeoviz/__init__.py
 src/rrcgeoviz/arguments.py
 src/rrcgeoviz/geoviz_cli.py
 src/rrcgeoviz.egg-info/PKG-INFO
 src/rrcgeoviz.egg-info/SOURCES.txt
 src/rrcgeoviz.egg-info/dependency_links.txt
 src/rrcgeoviz.egg-info/entry_points.txt
 src/rrcgeoviz.egg-info/requires.txt
 src/rrcgeoviz.egg-info/top_level.txt
+src/rrcgeoviz/JsonCreatorClasses/Blocks/ArrayTextBox.py
+src/rrcgeoviz/JsonCreatorClasses/Blocks/BaseBlock.py
+src/rrcgeoviz/JsonCreatorClasses/Blocks/DownloadButton.py
+src/rrcgeoviz/JsonCreatorClasses/Blocks/ImageCheckbox.py
+src/rrcgeoviz/JsonCreatorClasses/Blocks/TextBox.py
+src/rrcgeoviz/JsonCreatorClasses/Blocks/Toggle.py
+src/rrcgeoviz/JsonCreatorClasses/Sections/BaseSection.py
+src/rrcgeoviz/JsonCreatorClasses/Sections/CacheSetter.py
+src/rrcgeoviz/JsonCreatorClasses/Sections/ColumnSetter.py
+src/rrcgeoviz/JsonCreatorClasses/Sections/DownloadSection.py
+src/rrcgeoviz/JsonCreatorClasses/Sections/FeatureCustomizationsSetter.py
+src/rrcgeoviz/JsonCreatorClasses/Sections/FeatureSetter.py
 src/rrcgeoviz/datagenerators/GeneratorBertopic.py
 src/rrcgeoviz/datagenerators/GeneratorExample.py
 src/rrcgeoviz/datagenerators/GeneratorPOI.py
 src/rrcgeoviz/datagenerators/ParentDataGenerator.py
 src/rrcgeoviz/datagenerators/data/ports.csv
 src/rrcgeoviz/features/Downloadables.py
 src/rrcgeoviz/features/FeartureDataFrameEditor.py
@@ -27,11 +39,8 @@
 src/rrcgeoviz/features/FeatureOneYearMonths.py
 src/rrcgeoviz/features/FeaturePOI.py
 src/rrcgeoviz/features/FeatureSearch.py
 src/rrcgeoviz/features/FeatureThreeD.py
 src/rrcgeoviz/features/FeatureYearlyRange.py
 src/rrcgeoviz/features/ParentGeovizFeature.py
 src/rrcgeoviz/features/VisualizeBert.py
-tests/test_basic.py
-tests/test_caching.py
-tests/test_weird_data.py
-tests/test_weird_options.py
+tests/test_arguments.py
```

