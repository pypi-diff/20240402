# Comparing `tmp/scisuit-1.2.3.tar.gz` & `tmp/scisuit-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scisuit-1.2.3.tar", last modified: Mon Mar 25 13:11:15 2024, max compression
+gzip compressed data, was "scisuit-1.2.4.tar", last modified: Tue Apr  2 11:58:23 2024, max compression
```

## Comparing `scisuit-1.2.3.tar` & `scisuit-1.2.4.tar`

### file list

```diff
@@ -1,61 +1,62 @@
-drwxrwxrwx   0        0        0        0 2024-03-25 13:11:15.407781 scisuit-1.2.3/
--rw-rw-rw-   0        0        0       36 2024-02-26 09:50:28.000000 scisuit-1.2.3/MANIFEST.in
--rw-rw-rw-   0        0        0     3762 2024-03-25 13:11:15.403154 scisuit-1.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     3249 2024-03-07 14:57:26.000000 scisuit-1.2.3/README.md
--rw-rw-rw-   0        0        0    60302 2024-02-26 10:10:56.000000 scisuit-1.2.3/chart_multiple.png
--rw-rw-rw-   0        0        0    41412 2024-02-26 10:21:41.000000 scisuit-1.2.3/chart_scatter_trendline.png
--rw-rw-rw-   0        0        0      618 2024-03-25 11:52:15.000000 scisuit-1.2.3/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-03-25 13:11:14.388106 scisuit-1.2.3/scisuit/
--rw-rw-rw-   0        0        0       20 2023-09-05 12:11:22.000000 scisuit-1.2.3/scisuit/__init__.py
--rw-rw-rw-   0        0        0    14400 2024-03-21 13:14:10.000000 scisuit-1.2.3/scisuit/_ctypeslib.py
--rw-rw-rw-   0        0        0     1245 2024-02-09 13:09:45.000000 scisuit-1.2.3/scisuit/app.py
--rw-rw-rw-   0        0        0   174080 2022-12-08 15:59:38.000000 scisuit-1.2.3/scisuit/boost_math_tr1-vc143-mt-x64-1_81.dll
--rw-rw-rw-   0        0        0      124 2023-10-03 10:58:39.000000 scisuit-1.2.3/scisuit/decorators.py
--rw-rw-rw-   0        0        0       57 2023-10-07 09:47:36.000000 scisuit-1.2.3/scisuit/defs.py
--rw-rw-rw-   0        0        0     1600 2024-01-21 09:38:45.000000 scisuit-1.2.3/scisuit/derivative.py
-drwxrwxrwx   0        0        0        0 2024-03-25 13:11:14.824003 scisuit-1.2.3/scisuit/eng/
--rw-rw-rw-   0        0        0      144 2023-09-28 18:02:39.000000 scisuit-1.2.3/scisuit/eng/__init__.py
--rw-rw-rw-   0        0        0      326 2023-10-26 12:28:32.000000 scisuit-1.2.3/scisuit/eng/defs.py
--rw-rw-rw-   0        0        0     1702 2023-08-30 07:30:54.000000 scisuit-1.2.3/scisuit/eng/dryair.py
-drwxrwxrwx   0        0        0        0 2024-03-25 13:11:14.944647 scisuit-1.2.3/scisuit/eng/fpe/
--rw-rw-rw-   0        0        0      305 2023-10-03 10:06:50.000000 scisuit-1.2.3/scisuit/eng/fpe/__init__.py
--rw-rw-rw-   0        0        0    29633 2024-01-24 09:50:38.000000 scisuit-1.2.3/scisuit/eng/fpe/foodmaterial.py
--rw-rw-rw-   0        0        0     4948 2023-10-20 08:27:23.000000 scisuit-1.2.3/scisuit/eng/fpe/foodproperty.py
--rw-rw-rw-   0        0        0     2926 2023-10-14 09:51:05.000000 scisuit-1.2.3/scisuit/eng/humidair.py
--rw-rw-rw-   0        0        0    25131 2023-07-22 16:44:17.000000 scisuit-1.2.3/scisuit/eng/refrigerants.py
--rw-rw-rw-   0        0        0     1723 2024-01-25 09:58:13.000000 scisuit-1.2.3/scisuit/eng/water.py
--rw-rw-rw-   0        0        0     4395 2024-03-14 13:29:38.000000 scisuit-1.2.3/scisuit/fitting.py
--rw-rw-rw-   0        0        0     2496 2023-12-29 09:22:24.000000 scisuit-1.2.3/scisuit/integ.py
-drwxrwxrwx   0        0        0        0 2024-03-25 13:11:15.222820 scisuit-1.2.3/scisuit/plot/
--rw-rw-rw-   0        0        0      410 2024-03-21 13:18:40.000000 scisuit-1.2.3/scisuit/plot/__init__.py
--rw-rw-rw-   0        0        0     3995 2024-03-21 11:05:10.000000 scisuit-1.2.3/scisuit/plot/barcharts.py
--rw-rw-rw-   0        0        0     2668 2024-03-20 15:04:36.000000 scisuit-1.2.3/scisuit/plot/bubblechart.py
--rw-rw-rw-   0        0        0      687 2024-03-11 10:20:52.000000 scisuit-1.2.3/scisuit/plot/chartelems.py
--rw-rw-rw-   0        0        0    10507 2024-03-21 13:17:49.000000 scisuit-1.2.3/scisuit/plot/charts.py
--rw-rw-rw-   0        0        0     9159 2024-03-20 16:52:43.000000 scisuit-1.2.3/scisuit/plot/gdi.py
--rw-rw-rw-   0        0        0     3948 2024-03-20 15:04:36.000000 scisuit-1.2.3/scisuit/plot/gdiobj.py
--rw-rw-rw-   0        0        0     2412 2024-03-14 13:40:55.000000 scisuit-1.2.3/scisuit/plot/qqcharts.py
--rw-rw-rw-   0        0        0     2610 2024-03-20 15:04:36.000000 scisuit-1.2.3/scisuit/plot/quiverchart.py
--rw-rw-rw-   0        0        0     6976 2024-01-21 09:38:45.000000 scisuit-1.2.3/scisuit/roots.py
--rw-rw-rw-   0        0        0  1033728 2024-03-25 09:35:56.000000 scisuit-1.2.3/scisuit/scisuit_core.dll
--rw-rw-rw-   0        0        0  1094656 2024-03-25 09:37:01.000000 scisuit-1.2.3/scisuit/scisuit_plotter.dll
--rw-rw-rw-   0        0        0   160768 2024-03-25 11:47:46.000000 scisuit-1.2.3/scisuit/scisuit_pybind310.dll
--rw-rw-rw-   0        0        0   160768 2024-03-25 11:48:36.000000 scisuit-1.2.3/scisuit/scisuit_pybind311.dll
--rw-rw-rw-   0        0        0   160768 2024-03-25 11:49:22.000000 scisuit-1.2.3/scisuit/scisuit_pybind312.dll
-drwxrwxrwx   0        0        0        0 2024-03-25 13:11:15.389260 scisuit-1.2.3/scisuit/stats/
--rw-rw-rw-   0        0        0     1025 2024-03-12 13:20:29.000000 scisuit-1.2.3/scisuit/stats/__init__.py
--rw-rw-rw-   0        0        0    40449 2023-08-23 07:18:05.000000 scisuit-1.2.3/scisuit/stats/aov.py
--rw-rw-rw-   0        0        0     3867 2023-10-12 13:54:40.000000 scisuit-1.2.3/scisuit/stats/core.py
--rw-rw-rw-   0        0        0    18176 2023-10-12 13:55:10.000000 scisuit-1.2.3/scisuit/stats/distributions.py
--rw-rw-rw-   0        0        0    11530 2023-08-22 09:29:31.000000 scisuit-1.2.3/scisuit/stats/linregress.py
--rw-rw-rw-   0        0        0    16328 2023-12-29 11:21:02.000000 scisuit-1.2.3/scisuit/stats/test_basic.py
--rw-rw-rw-   0        0        0     1617 2024-03-20 15:04:36.000000 scisuit-1.2.3/scisuit/util.py
--rw-rw-rw-   0        0        0    93184 2023-10-12 08:59:10.000000 scisuit-1.2.3/scisuit/wxmsw32u_gl_vc_custom.dll
--rw-rw-rw-   0        0        0 17864704 2023-10-12 08:59:02.000000 scisuit-1.2.3/scisuit/wxmsw32u_vc_custom.dll
-drwxrwxrwx   0        0        0        0 2024-03-25 13:11:15.400155 scisuit-1.2.3/scisuit.egg-info/
--rw-rw-rw-   0        0        0     3762 2024-03-25 13:11:10.000000 scisuit-1.2.3/scisuit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1288 2024-03-25 13:11:10.000000 scisuit-1.2.3/scisuit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-25 13:11:10.000000 scisuit-1.2.3/scisuit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-03-25 13:11:10.000000 scisuit-1.2.3/scisuit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-03-25 13:11:10.000000 scisuit-1.2.3/scisuit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-25 13:11:15.408304 scisuit-1.2.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-02 11:58:23.256700 scisuit-1.2.4/
+-rw-rw-rw-   0        0        0     1202 2024-01-16 09:45:52.000000 scisuit-1.2.4/LICENSE
+-rw-rw-rw-   0        0        0       36 2024-02-26 09:50:28.000000 scisuit-1.2.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     3785 2024-04-02 11:58:23.256700 scisuit-1.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3249 2024-03-07 14:57:26.000000 scisuit-1.2.4/README.md
+-rw-rw-rw-   0        0        0    60302 2024-02-26 10:10:56.000000 scisuit-1.2.4/chart_multiple.png
+-rw-rw-rw-   0        0        0    41412 2024-02-26 10:21:41.000000 scisuit-1.2.4/chart_scatter_trendline.png
+-rw-rw-rw-   0        0        0      618 2024-04-02 11:54:58.000000 scisuit-1.2.4/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-02 11:58:22.864611 scisuit-1.2.4/scisuit/
+-rw-rw-rw-   0        0        0       20 2023-09-05 12:11:22.000000 scisuit-1.2.4/scisuit/__init__.py
+-rw-rw-rw-   0        0        0    14400 2024-03-21 13:14:10.000000 scisuit-1.2.4/scisuit/_ctypeslib.py
+-rw-rw-rw-   0        0        0     1245 2024-02-09 13:09:45.000000 scisuit-1.2.4/scisuit/app.py
+-rw-rw-rw-   0        0        0   174080 2022-12-08 15:59:38.000000 scisuit-1.2.4/scisuit/boost_math_tr1-vc143-mt-x64-1_81.dll
+-rw-rw-rw-   0        0        0      124 2023-10-03 10:58:39.000000 scisuit-1.2.4/scisuit/decorators.py
+-rw-rw-rw-   0        0        0       57 2023-10-07 09:47:36.000000 scisuit-1.2.4/scisuit/defs.py
+-rw-rw-rw-   0        0        0     1600 2024-01-21 09:38:45.000000 scisuit-1.2.4/scisuit/derivative.py
+drwxrwxrwx   0        0        0        0 2024-04-02 11:58:23.005632 scisuit-1.2.4/scisuit/eng/
+-rw-rw-rw-   0        0        0      144 2023-09-28 18:02:39.000000 scisuit-1.2.4/scisuit/eng/__init__.py
+-rw-rw-rw-   0        0        0      326 2023-10-26 12:28:32.000000 scisuit-1.2.4/scisuit/eng/defs.py
+-rw-rw-rw-   0        0        0     1702 2023-08-30 07:30:54.000000 scisuit-1.2.4/scisuit/eng/dryair.py
+drwxrwxrwx   0        0        0        0 2024-04-02 11:58:23.036943 scisuit-1.2.4/scisuit/eng/fpe/
+-rw-rw-rw-   0        0        0      305 2023-10-03 10:06:50.000000 scisuit-1.2.4/scisuit/eng/fpe/__init__.py
+-rw-rw-rw-   0        0        0    29633 2024-01-24 09:50:38.000000 scisuit-1.2.4/scisuit/eng/fpe/foodmaterial.py
+-rw-rw-rw-   0        0        0     4948 2023-10-20 08:27:23.000000 scisuit-1.2.4/scisuit/eng/fpe/foodproperty.py
+-rw-rw-rw-   0        0        0     2926 2023-10-14 09:51:05.000000 scisuit-1.2.4/scisuit/eng/humidair.py
+-rw-rw-rw-   0        0        0    25120 2024-03-29 12:27:53.000000 scisuit-1.2.4/scisuit/eng/refrigerants.py
+-rw-rw-rw-   0        0        0     1770 2024-03-29 12:16:58.000000 scisuit-1.2.4/scisuit/eng/water.py
+-rw-rw-rw-   0        0        0     4244 2024-03-29 14:13:30.000000 scisuit-1.2.4/scisuit/fitting.py
+-rw-rw-rw-   0        0        0     2496 2023-12-29 09:22:24.000000 scisuit-1.2.4/scisuit/integ.py
+drwxrwxrwx   0        0        0        0 2024-04-02 11:58:23.162505 scisuit-1.2.4/scisuit/plot/
+-rw-rw-rw-   0        0        0      410 2024-03-21 13:18:40.000000 scisuit-1.2.4/scisuit/plot/__init__.py
+-rw-rw-rw-   0        0        0     4043 2024-03-31 14:08:08.000000 scisuit-1.2.4/scisuit/plot/barcharts.py
+-rw-rw-rw-   0        0        0     2668 2024-03-20 15:04:36.000000 scisuit-1.2.4/scisuit/plot/bubblechart.py
+-rw-rw-rw-   0        0        0      687 2024-03-11 10:20:52.000000 scisuit-1.2.4/scisuit/plot/chartelems.py
+-rw-rw-rw-   0        0        0    10512 2024-03-31 14:08:05.000000 scisuit-1.2.4/scisuit/plot/charts.py
+-rw-rw-rw-   0        0        0     9159 2024-03-20 16:52:43.000000 scisuit-1.2.4/scisuit/plot/gdi.py
+-rw-rw-rw-   0        0        0     3948 2024-03-20 15:04:36.000000 scisuit-1.2.4/scisuit/plot/gdiobj.py
+-rw-rw-rw-   0        0        0     2413 2024-04-01 14:10:03.000000 scisuit-1.2.4/scisuit/plot/qqcharts.py
+-rw-rw-rw-   0        0        0     2610 2024-03-20 15:04:36.000000 scisuit-1.2.4/scisuit/plot/quiverchart.py
+-rw-rw-rw-   0        0        0     6942 2024-03-29 15:11:07.000000 scisuit-1.2.4/scisuit/roots.py
+-rw-rw-rw-   0        0        0  1033728 2024-04-02 11:31:30.000000 scisuit-1.2.4/scisuit/scisuit_core.dll
+-rw-rw-rw-   0        0        0  1094656 2024-04-02 11:32:33.000000 scisuit-1.2.4/scisuit/scisuit_plotter.dll
+-rw-rw-rw-   0        0        0   160768 2024-04-02 11:53:45.000000 scisuit-1.2.4/scisuit/scisuit_pybind310.dll
+-rw-rw-rw-   0        0        0   160768 2024-04-02 11:52:27.000000 scisuit-1.2.4/scisuit/scisuit_pybind311.dll
+-rw-rw-rw-   0        0        0   160768 2024-04-02 11:54:26.000000 scisuit-1.2.4/scisuit/scisuit_pybind312.dll
+drwxrwxrwx   0        0        0        0 2024-04-02 11:58:23.256700 scisuit-1.2.4/scisuit/stats/
+-rw-rw-rw-   0        0        0     1025 2024-03-12 13:20:29.000000 scisuit-1.2.4/scisuit/stats/__init__.py
+-rw-rw-rw-   0        0        0    40578 2024-03-30 13:37:40.000000 scisuit-1.2.4/scisuit/stats/aov.py
+-rw-rw-rw-   0        0        0     3867 2023-10-12 13:54:40.000000 scisuit-1.2.4/scisuit/stats/core.py
+-rw-rw-rw-   0        0        0    18976 2024-03-31 12:41:47.000000 scisuit-1.2.4/scisuit/stats/distributions.py
+-rw-rw-rw-   0        0        0    11530 2023-08-22 09:29:31.000000 scisuit-1.2.4/scisuit/stats/linregress.py
+-rw-rw-rw-   0        0        0    16795 2024-03-31 09:01:03.000000 scisuit-1.2.4/scisuit/stats/test_basic.py
+-rw-rw-rw-   0        0        0     1617 2024-03-20 15:04:36.000000 scisuit-1.2.4/scisuit/util.py
+-rw-rw-rw-   0        0        0    93184 2023-10-12 08:59:10.000000 scisuit-1.2.4/scisuit/wxmsw32u_gl_vc_custom.dll
+-rw-rw-rw-   0        0        0 17864704 2023-10-12 08:59:02.000000 scisuit-1.2.4/scisuit/wxmsw32u_vc_custom.dll
+drwxrwxrwx   0        0        0        0 2024-04-02 11:58:23.256700 scisuit-1.2.4/scisuit.egg-info/
+-rw-rw-rw-   0        0        0     3785 2024-04-02 11:58:20.000000 scisuit-1.2.4/scisuit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1296 2024-04-02 11:58:20.000000 scisuit-1.2.4/scisuit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 11:58:20.000000 scisuit-1.2.4/scisuit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-02 11:58:20.000000 scisuit-1.2.4/scisuit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-02 11:58:20.000000 scisuit-1.2.4/scisuit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-02 11:58:23.256700 scisuit-1.2.4/setup.cfg
```

### Comparing `scisuit-1.2.3/PKG-INFO` & `scisuit-1.2.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: scisuit
-Version: 1.2.3
+Version: 1.2.4
 Summary: Scientific Computing Package
 Author-email: "Gokhan Bingol, PhD" <gbingol@pebytes.com>
 Project-URL: Homepage, https://www.pebytes.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: C++
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: numpy
 
 ## scisuit
 
 A computing and plotting library designed with engineers
 in mind..
```

### Comparing `scisuit-1.2.3/README.md` & `scisuit-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `scisuit-1.2.3/chart_multiple.png` & `scisuit-1.2.4/chart_multiple.png`

 * *Files identical despite different names*

### Comparing `scisuit-1.2.3/chart_scatter_trendline.png` & `scisuit-1.2.4/chart_scatter_trendline.png`

 * *Files identical despite different names*

### Comparing `scisuit-1.2.3/pyproject.toml` & `scisuit-1.2.4/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "scisuit"
-version = "1.2.3"
+version = "1.2.4"
 authors = [{ name="Gokhan Bingol, PhD", email="gbingol@pebytes.com" },]
 description = "Scientific Computing Package"
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = ["numpy", ]
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `scisuit-1.2.3/scisuit/_ctypeslib.py` & `scisuit-1.2.4/scisuit/_ctypeslib.py`

 * *Files identical despite different names*

### Comparing `scisuit-1.2.3/scisuit/app.py` & `scisuit-1.2.4/scisuit/app.py`

 * *Files identical despite different names*

### Comparing `scisuit-1.2.3/scisuit/boost_math_tr1-vc143-mt-x64-1_81.dll` & `scisuit-1.2.4/scisuit/boost_math_tr1-vc143-mt-x64-1_81.dll`

 * *Files identical despite different names*

### Comparing `scisuit-1.2.3/scisuit/derivative.py` & `scisuit-1.2.4/scisuit/derivative.py`

 * *Files identical despite different names*

### Comparing `scisuit-1.2.3/scisuit/eng/dryair.py` & `scisuit-1.2.4/scisuit/eng/dryair.py`

 * *Files identical despite different names*

### Comparing `scisuit-1.2.3/scisuit/eng/fpe/foodmaterial.py` & `scisuit-1.2.4/scisuit/eng/fpe/foodmaterial.py`

 * *Files identical despite different names*

### Comparing `scisuit-1.2.3/scisuit/eng/fpe/foodproperty.py` & `scisuit-1.2.4/scisuit/eng/fpe/foodproperty.py`

 * *Files identical despite different names*

### Comparing `scisuit-1.2.3/scisuit/eng/humidair.py` & `scisuit-1.2.4/scisuit/eng/humidair.py`

 * *Files identical despite different names*

### Comparing `scisuit-1.2.3/scisuit/eng/refrigerants.py` & `scisuit-1.2.4/scisuit/eng/refrigerants.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import dataclasses as _dc
 import numpy as _np
 
 @_dc.dataclass
 class Refrigerant:
 	"""
-	Properties of refrigerants \n
-	S: Saturated \n
-	\n
-	T: Saturation temperature (K) \n
-	P: Saturation pressure (kPa) \n
-	vf, vg: specific volume (m3/kg) \n
-	hf, hg: enthalpy (kJ/kg) \n
-	sf, sg: entropy (kJ/kgK)
+	Properties of refrigerants
+	`S:` Saturated
+	`T:` Saturation temperature (K)
+	`P:` Saturation pressure (kPa)
+	`vf, vg:` specific volume (m3/kg)
+	`hf, hg:` enthalpy (kJ/kg)
+	`sf, sg:` entropy (kJ/kgK)
 	"""
 	@_dc.dataclass
 	class SR12:
 		"""Dichlorodifluoromethane"""
 		T = _np.array([183.15, 188.15, 193.15, 198.15, 203.15, 208.15, 213.15, 218.15,
 		223.15, 228.15, 233.15, 238.15, 243.15, 248.15, 253.15, 258.15,
 		263.15, 268.15, 273.15, 278.15, 283.15, 288.15, 293.15, 298.15,
```

### Comparing `scisuit-1.2.3/scisuit/eng/water.py` & `scisuit-1.2.4/scisuit/eng/water.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 		"""T in Celcius"""
 		assert T>0 and T<100, "T must be in range (0, 100)"
 		self.__T = T
 	
 	
 	def cp(self)->float:
 		"""
+		Computes specific heat capacity, kJ/kgK
+		
 		Thermo-physical properties are valid in the range of -40<=T(C) <=150
 		2006, ASHRAE Handbook Chapter 9, Table 1 (source: Choi and Okos (1986))
 		"""
 		T = self.__T
 		return 4.1289 + T*(-9.0864e-05 + 5.4731e-06*T)
```

### Comparing `scisuit-1.2.3/scisuit/fitting.py` & `scisuit-1.2.4/scisuit/fitting.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,25 +54,24 @@
 
 	return m * xval + n
 
 
 
 
 
-def lagrange(x:Iterable, y:Iterable, val:float)->float:
+def lagrange(
+		x:Iterable, 
+		y:Iterable, 
+		value:float)->float:
 	"""
 	Constructs lagrange polynomial from x,y to compute the given value.
-
-	## Inputs:
-	x, y: x and y-values \n
-	val: value in the range of x whose corresponding y value is wish to be known.
 	"""
-	assert issubclass(val, _numbers.Real)
+	assert issubclass(value, _numbers.Real)
 
-	return _pydll.c_fit_lagrange(x, y, _ct.c_double(val))
+	return _pydll.c_fit_lagrange(x, y, _ct.c_double(value))
 
 
 ########################################################################################
 
 
 @_dc.dataclass
 class SplineResult:
@@ -93,23 +92,22 @@
 	
 	return  [SplineResult(_Polynomial.Polynomial(l[0]), l[1], l[2]) for l in lst]
 
 
 ########################################################################################
 
 
-def expfit(x, y, intercept=None)->list:
+def expfit(
+		x:Iterable, 
+		y:Iterable, 
+		intercept:None|float=None)->list:
 	"""
 	Fits x,y to the equation y = a*exp(b*x) \n
 	Returns [a, b]
 
-	## Inputs:
-	x, y: list/ndarray \n
-	intercept: None or float
-
 	## Note:
 	If intercept is not provided both a, b are computed. \n
 	If intercept is given then a=intercept and b is computed accordingly.
 	"""
 	if(intercept!=None):
 		assert issubclass(intercept, _numbers.Real)
 
@@ -135,22 +133,18 @@
 	"""
 	if(limit!=None):
 		assert issubclass(limit, _numbers.Real)
 
 	return _pydll.c_fit_logistfit(x, y, limit)
 
 
-def polyfit(x, y, deg)->tuple:
+def polyfit(x:Iterable, y:Iterable, deg)->tuple:
 	"""
-	Uses numpy.polynomial.polynomial.polyfit \n
-	Returns (coefficients, residuals)
-
-	## Inputs:
-	x, y: list/ndarray
-
+	Uses numpy.polynomial.polynomial.polyfit
+	returns (coefficients, residuals)
 	"""
 	coeffs, stats = _Polynomial.polyfit(x=x, y=y, deg=deg)
 	return coeffs, stats[0]
 
 
 def powfit(x:Iterable, y:Iterable)->list[float]:
 	"""
```

### Comparing `scisuit-1.2.3/scisuit/integ.py` & `scisuit-1.2.4/scisuit/integ.py`

 * *Files identical despite different names*

### Comparing `scisuit-1.2.3/scisuit/plot/barcharts.py` & `scisuit-1.2.4/scisuit/plot/barcharts.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,21 @@
 from .charts import canvas, xlim, ylim, set_xticks, set_yticks
 from ..util import NiceNumbers, minmax
 
 
 
 
 
-def bar(x, height, width=0.8, bottom=0.0, color = None, **kwargs):
+def bar(
+		x, 
+		height, 
+		width=0.8, 
+		bottom=0.0, 
+		color = None, 
+		**kwargs):
 	"""
 	`x:` The x coordinates of the bars or category
 	`height:` The height of the bars.
 	`width:` The width of the bars.
 	`bottom:` The y coordinate of the bottom side of the bars.
 	"""
 	assert isinstance(bottom, numbers.Real|_Iterable)
@@ -67,15 +73,21 @@
 	if X_HasStr:
 		set_xticks(pos, x)
 
 
 
 
 
-def barh(y, width, height=0.8, left=0.0, color = None, **kwargs):
+def barh(
+		y, 
+		width, 
+		height=0.8, 
+		left=0.0, 
+		color = None, 
+		**kwargs):
 	"""
 	`y:` The y coordinates of the bars or category
 	`height:` The height of the bars.
 	`width:` The width of the bars.
 	`bottom:` The y coordinate of the bottom side of the bars.
 	"""
 	assert isinstance(left, numbers.Real|_Iterable)
```

### Comparing `scisuit-1.2.3/scisuit/plot/bubblechart.py` & `scisuit-1.2.4/scisuit/plot/bubblechart.py`

 * *Files identical despite different names*

### Comparing `scisuit-1.2.3/scisuit/plot/chartelems.py` & `scisuit-1.2.4/scisuit/plot/chartelems.py`

 * *Files identical despite different names*

### Comparing `scisuit-1.2.3/scisuit/plot/charts.py` & `scisuit-1.2.4/scisuit/plot/charts.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 
 
 #-----------------------------------------------------------------------------------
 
 def boxplot(
 	data:_Iterable, 
-	label:str = None, 
+	label:str|None = None, 
 	**kwargs):
 	"""
 	Plots box-whisker chart.
 
 	## Input
 	data : Data to be plotted \n
 	label: Name of the series
```

### Comparing `scisuit-1.2.3/scisuit/plot/gdi.py` & `scisuit-1.2.4/scisuit/plot/gdi.py`

 * *Files identical despite different names*

### Comparing `scisuit-1.2.3/scisuit/plot/gdiobj.py` & `scisuit-1.2.4/scisuit/plot/gdiobj.py`

 * *Files identical despite different names*

### Comparing `scisuit-1.2.3/scisuit/plot/qqcharts.py` & `scisuit-1.2.4/scisuit/plot/qqcharts.py`

 * *Files 9% similar despite different names*

```diff
@@ -56,23 +56,26 @@
 		MinQ, MaxQ = minmax(Quantiles)
 
 		#Extend the line by 10% in both directions
 		MinQ = MinQ*1.1
 		MaxQ = MaxQ*1.1
 
 		lwidth = (kwargs.get("lw") or kwargs.get("linewidth")) or 2
-		scatter(x=(MinQ, MaxQ), y=(MinQ, MaxQ), marker=None, lw=lwidth, **kwargs)
+		scatter(x=(MinQ, MaxQ), y=(MinQ, MaxQ), marker=None, **kwargs)
 
 	scatter(x=Quantiles, y=_np.sort(data), label=label, marker=marker)
 
 
 
 
 
-def qqplot(x:_Iterable, y:_Iterable, **kwargs):
+def qqplot(
+		x:_Iterable, 
+		y:_Iterable, 
+		**kwargs):
 	"""
 	Plots quantile-quantile chart using two data-sets (x,y)
 
 	## Input
 	x, y: Data
 	"""
 	assert isinstance(x, _Iterable), "'x' must be iterable"
```

### Comparing `scisuit-1.2.3/scisuit/plot/quiverchart.py` & `scisuit-1.2.4/scisuit/plot/quiverchart.py`

 * *Files identical despite different names*

### Comparing `scisuit-1.2.3/scisuit/roots.py` & `scisuit-1.2.4/scisuit/roots.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,20 +33,20 @@
 	maxiter=100, 
 	method="bf", 
 	modified=False)->tuple[float, Info]:
 	"""
 	Finds the root using bisection method, returns (root, Info)
 
 	## Inputs:
-	f: A unary function \n
-	a, b:	The interval where the root lies in \n
-	tol:	tolerance for error \n
-	maxiter: Maximum number of iterations \n
-	method: "bf" for brute-force (halving)  \n
-	"rf" for regula falsi (false position)  \n
+	f: A unary function
+	a, b: The interval where the root lies in
+	tol: tolerance for error
+	maxiter: Maximum number of iterations
+	method: "bf" for brute-force (halving) 
+	"rf" for regula falsi (false position) 
 	modified: True for modified regula falsi method.
 	"""
 	assert callable(f), "f must be function"
 	assert isinstance(a, _numbers.Real), "a must be real number"
 	assert isinstance(b, _numbers.Real), "b must be real number"
 
 	root, lst =_pydll.c_root_bisect(f, _ct.c_double(a), _ct.c_double(b), 
@@ -71,15 +71,14 @@
 	using inverse quadratic interpolation, returns (root, Info)
 
 	## Inputs:
 	f: A unary function whose root is sought after \n
 	a, b: The interval where root lies in \n
 	tol: tolerance for error \n
 	maxiter: Maximum number of iterations during the search for the root
-
 	"""
 	assert callable(f), "f must be function"
 	assert isinstance(a, _numbers.Real), "a must be real number"
 	assert isinstance(b, _numbers.Real), "b must be real number"
 
 	root, lst = _pydll.c_root_brentq(f, _ct.c_double(a), _ct.c_double(b), _ct.c_double(tol), _ct.c_int(maxiter))
 
@@ -124,18 +123,18 @@
 	"""
 	If fprime is provided then uses Newton-Raphson method  \n
 	If fprime is not provided, then x1 must be provided uses Secant method.
 
 	returns (root, Info)
 
 	## Inputs:
-	f: A unary function \n
-	fprime: derivative of f \n
-	x0, x1: Initial guesses \n
-	tol: tolerance for error \n
+	f: A unary function 
+	fprime: derivative of f 
+	x0, x1: Initial guesses 
+	tol: tolerance for error 
 	maxiter: Max number of iterations
 	"""
 	assert callable(f), "f must be function"
 	assert isinstance(x0, _numbers.Real)
 	if(fprime == None):
 		assert isinstance(x1, _numbers.Real), "If fprime not provided, x1 must be a real number"
 	else:
@@ -154,17 +153,17 @@
 	b:float, 
 	tol=1E-5, 
 	maxiter=100)->tuple[float, Info]:
 	"""
 	Uses Ridder's method.
 
 	## Inputs:
-	f: A unary function \n
-	a, b:	The interval where the root lies in \n
-	tol: tolerance for error \n
+	f: A unary function 
+	a, b: The interval where the root lies in 
+	tol: tolerance for error 
 	maxiter: Maximum number of iterations
 	"""
 	assert callable(f), "f must be function"
 	assert isinstance(a, _numbers.Real), "a must be real number"
 	assert isinstance(b, _numbers.Real), "b must be real number"
 	
 	root, lst = _pydll.c_root_ridder(f, _ct.c_double(a), _ct.c_double(b), _ct.c_double(tol), _ct.c_int(maxiter))
```

### Comparing `scisuit-1.2.3/scisuit/scisuit_core.dll` & `scisuit-1.2.4/scisuit/scisuit_core.dll`

 * *Files 0% similar despite different names*

#### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800b2690
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Mon Mar 25 09:35:56 2024
+Time/Date		Tue Apr  2 11:31:30 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	39
 SizeOfCode		00000000000b5000
 SizeOfInitializedData	0000000000047800
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000b2690
@@ -21773,15 +21773,15 @@
 	reloc   16 offset  530 [f7530] DIR64
 	reloc   17 offset    0 [f7000] ABSOLUTE
 
 There is a debug directory in .rdata at 0x1800de8a0
 
 Type                Size     Rva      Offset
   2        CodeView 0000006c 000e0320 000df720
-(format RSDS signature 9357c4151b174b13a02bcbeac799e128 age 1 pdb C:\Users\gbing\Documents\Visual Studio 2022\Projects\sci_libs\libs\scisuit_core.pdb)
+(format RSDS signature e7ae524271754b669a903003d3f0ce7f age 1 pdb C:\Users\gbing\Documents\Visual Studio 2022\Projects\sci_libs\libs\scisuit_core.pdb)
  12         Feature 00000014 000e038c 000df78c
  13         CoffGrp 00000364 000e03a0 000df7a0
  14           ILTCG 00000000 00000000 00000000
 
 The .rsrc Resource Directory section:
 000  Type Table: Char: 0, Time: 00000000, Ver: 0/0, Num Names: 0, IDs: 2
 010   Entry: ID: 0x000010, Value: 0x80000020
@@ -259157,41 +259157,43 @@
    1800de890:	cmp    %ah,0xb(%rbp)
    1800de893:	addb   $0x0,(%rcx)
    1800de896:	add    %al,(%rax)
    1800de898:	rex
    1800de899:	or     %gs:0x1(%rax),%eax
    1800de8a0:	add    %al,(%rax)
    1800de8a2:	add    %al,(%rax)
-   1800de8a4:	jl     0x1800de8eb
-   1800de8a6:	add    %esp,0x0(%rsi)
+   1800de8a4:	xchg   %eax,%edx
+   1800de8a5:	in     (%dx),%al
+   1800de8a6:	or     0x0(%rsi),%esp
    1800de8a9:	add    %al,(%rax)
    1800de8ab:	add    %al,(%rdx)
    1800de8ad:	add    %al,(%rax)
    1800de8af:	add    %ch,0x0(%rax,%rax,1)
    1800de8b3:	add    %ah,(%rax)
    1800de8b5:	add    (%rsi),%ecx
    1800de8b7:	add    %ah,(%rax)
-   1800de8b9:	testl  $0x1457c00,0x0(%rip)        # 0x1800de8c3
+   1800de8b9:	testl  $0xbec9200,0x0(%rip)        # 0x1800de8c3
    1800de8c3:	data16 add %al,(%rax)
    1800de8c6:	add    %al,(%rax)
    1800de8c8:	or     $0x0,%al
    1800de8ca:	add    %al,(%rax)
    1800de8cc:	adc    $0x0,%al
    1800de8ce:	add    %al,(%rax)
    1800de8d0:	mov    %es,(%rbx)
    1800de8d2:	(bad)
    1800de8d3:	add    %cl,0xd(%rdi,%rsi,8)
    1800de8da:	add    %al,(%rax)
-   1800de8dc:	jl     0x1800de923
-   1800de8de:	add    %esp,0x0(%rsi)
+   1800de8dc:	xchg   %eax,%edx
+   1800de8dd:	in     (%dx),%al
+   1800de8de:	or     0x0(%rsi),%esp
    1800de8e1:	add    %al,(%rax)
    1800de8e3:	add    %cl,0x64000000(%rip)        # 0x1e40de8e9
    1800de8e9:	add    (%rax),%eax
    1800de8eb:	add    %ah,-0x5ffff1fd(%rax)
-   1800de8f1:	testl  $0x1457c00,0x0(%rip)        # 0x1800de8fb
+   1800de8f1:	testl  $0xbec9200,0x0(%rip)        # 0x1800de8fb
    1800de8fb:	data16 add %al,(%rax)
    1800de8fe:	add    %al,(%rax)
    1800de900:	(bad)
 	...
    1800de97d:	add    %al,(%rax)
    1800de97f:	add    %ch,(%rax)
    1800de981:	(bad)
@@ -260973,17 +260975,24 @@
    1800e0318:	cmp    $0x5e,%al
    1800e031a:	or     (%rax),%eax
    1800e031c:	jnp    0x1800e031f
    1800e031e:	add    %al,(%rax)
    1800e0320:	push   %rdx
    1800e0321:	push   %rbx
    1800e0322:	rex.R push %rbx
-   1800e0324:	adc    $0x179357c4,%eax
-   1800e0329:	sbb    (%rbx),%edx
-   1800e032b:	rex.WXB movabs 0x128e199c7eacb2b,%al
+   1800e0324:	rex.X push %rdx
+   1800e0326:	scas   %es:(%rdi),%al
+   1800e0327:	out    %eax,$0x75
+   1800e0329:	jno    0x1800e0391
+   1800e032b:	rex.WXB (bad)
+   1800e032d:	nop
+   1800e032e:	xor    %al,(%rbx)
+   1800e0330:	shl    %cl,%eax
+   1800e0332:	(bad)
+   1800e0333:	jg     0x1800e0336
    1800e0335:	add    %al,(%rax)
    1800e0337:	add    %al,0x3a(%rbx)
    1800e033a:	pop    %rsp
    1800e033b:	push   %rbp
    1800e033c:	jae    0x1800e03a3
    1800e033e:	jb     0x1800e03b3
    1800e0340:	pop    %rsp
```

### Comparing `scisuit-1.2.3/scisuit/scisuit_plotter.dll` & `scisuit-1.2.4/scisuit/scisuit_plotter.dll`

 * *Files 1% similar despite different names*

#### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180069930
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Mon Mar 25 09:37:01 2024
+Time/Date		Tue Apr  2 11:32:33 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	39
 SizeOfCode		0000000000075a00
 SizeOfInitializedData	0000000000095c00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000069930
@@ -41116,15 +41116,15 @@
 	reloc    0 offset   40 [ff040] DIR64
 	reloc    1 offset    0 [ff000] ABSOLUTE
 
 There is a debug directory in .rdata at 0x1800b9460
 
 Type                Size     Rva      Offset
   2        CodeView 0000006f 000c85e8 000c73e8
-(format RSDS signature 5830f45d9b3542b3af3c37e055f26fe2 age 1 pdb C:\Users\gbing\Documents\Visual Studio 2022\Projects\sci_libs\libs\scisuit_plotter.pdb)
+(format RSDS signature 4627226cc83845a2b5b5d0a56c8be043 age 1 pdb C:\Users\gbing\Documents\Visual Studio 2022\Projects\sci_libs\libs\scisuit_plotter.pdb)
  12         Feature 00000014 000c8658 000c7458
  13         CoffGrp 000002f4 000c866c 000c746c
  14           ILTCG 00000000 00000000 00000000
 
 The .rsrc Resource Directory section:
 000  Type Table: Char: 0, Time: 00000000, Ver: 0/0, Num Names: 0, IDs: 1
 010   Entry: ID: 0x000018, Value: 0x80000018
@@ -84160,17 +84160,17 @@
    180025b46:	cvtdq2pd %xmm1,%xmm1
    180025b4a:	mulsd  %xmm7,%xmm1
    180025b4e:	divsd  %xmm9,%xmm1
    180025b53:	addsd  %xmm0,%xmm1
    180025b57:	cvttsd2si %xmm1,%eax
    180025b5b:	mov    %eax,0x24(%rsp)
    180025b5f:	test   %ecx,%ecx
-   180025b61:	jle    0x180025b71
+   180025b61:	js     0x180025b71
    180025b63:	test   %eax,%eax
-   180025b65:	jle    0x180025b71
+   180025b65:	js     0x180025b71
    180025b67:	mov    0x20(%rsp),%rcx
    180025b6c:	mov    %rcx,(%rbx)
    180025b6f:	jmp    0x180025b76
    180025b71:	xor    %eax,%eax
    180025b73:	mov    %rax,(%rbx)
    180025b76:	movaps 0x60(%rsp),%xmm6
    180025b7b:	mov    %rbx,%rax
@@ -272670,45 +272670,52 @@
    1800b944e:	add    %al,(%rax)
    1800b9450:	rcrb   $1,0x18007(%rdi)
    1800b9456:	add    %al,(%rax)
    1800b9458:	fcomps 0x18007(%rdi)
    1800b945e:	add    %al,(%rax)
    1800b9460:	add    %al,(%rax)
    1800b9462:	add    %al,(%rax)
-   1800b9464:	mov    $0x660145,%ebp
+   1800b9464:	shr    $1,%esp
+   1800b9466:	or     0x0(%rsi),%esp
    1800b9469:	add    %al,(%rax)
    1800b946b:	add    %al,(%rdx)
    1800b946d:	add    %al,(%rax)
    1800b946f:	add    %ch,0x0(%rdi)
    1800b9472:	add    %al,(%rax)
    1800b9474:	call   0x1680ba0fe
    1800b9479:	jae    0x1800b9487
    1800b947b:	add    %al,(%rax)
    1800b947d:	add    %al,(%rax)
-   1800b947f:	add    %bh,0x660145(%rbp)
+   1800b947f:	add    %dl,%cl
+   1800b9481:	in     (%dx),%al
+   1800b9482:	or     0x0(%rsi),%esp
    1800b9485:	add    %al,(%rax)
    1800b9487:	add    %cl,(%rax,%rax,1)
    1800b948a:	add    %al,(%rax)
    1800b948c:	adc    $0x0,%al
    1800b948e:	add    %al,(%rax)
    1800b9490:	pop    %rax
    1800b9491:	xchg   %cl,(%rax,%rax,1)
    1800b9494:	pop    %rax
    1800b9495:	je     0x1800b94a3
    1800b9497:	add    %al,(%rax)
    1800b9499:	add    %al,(%rax)
-   1800b949b:	add    %bh,0x660145(%rbp)
+   1800b949b:	add    %dl,%cl
+   1800b949d:	in     (%dx),%al
+   1800b949e:	or     0x0(%rsi),%esp
    1800b94a1:	add    %al,(%rax)
    1800b94a3:	add    %cl,-0xc000000(%rip)        # 0x1740b94a9
    1800b94a9:	add    (%rax),%al
    1800b94ab:	add    %ch,0xc(%rsi,%rax,4)
    1800b94af:	add    %ch,0xc(%rsp,%rsi,2)
    1800b94b3:	add    %al,(%rax)
    1800b94b5:	add    %al,(%rax)
-   1800b94b7:	add    %bh,0x660145(%rbp)
+   1800b94b7:	add    %dl,%cl
+   1800b94b9:	in     (%dx),%al
+   1800b94ba:	or     0x0(%rsi),%esp
    1800b94bd:	add    %al,(%rax)
    1800b94bf:	add    %cl,(%rsi)
 	...
    1800b94fd:	add    %al,(%rax)
    1800b94ff:	add    %al,(%rcx)
 	...
    1800b9509:	add    %al,(%rax)
@@ -288820,30 +288827,22 @@
    1800c85dd:	add    %eax,(%rax)
    1800c85df:	add    %bh,0x7(%rax,%rbp,2)
    1800c85e3:	add    %bl,0x0(%rbx)
    1800c85e6:	add    %al,(%rax)
    1800c85e8:	push   %rdx
    1800c85e9:	push   %rbx
    1800c85ea:	rex.R push %rbx
-   1800c85ec:	pop    %rbp
-   1800c85ed:	hlt
-   1800c85ee:	xor    %bl,0x35(%rax)
-   1800c85f1:	fwait
-   1800c85f2:	mov    $0x42,%bl
-   1800c85f4:	scas   %es:(%rdi),%eax
-   1800c85f5:	cmp    $0x37,%al
-   1800c85f7:	loopne 0x1800c864e
-   1800c85f9:	repnz outsl %ds:(%rsi),(%dx)
-   1800c85fb:	loop   0x1800c85fe
-   1800c85fd:	add    %al,(%rax)
-   1800c85ff:	add    %al,0x3a(%rbx)
-   1800c8602:	pop    %rsp
-   1800c8603:	push   %rbp
-   1800c8604:	jae    0x1800c866b
-   1800c8606:	jb     0x1800c867b
+   1800c85ec:	insb   (%dx),%es:(%rdi)
+   1800c85ed:	and    (%rdi),%ah
+   1800c85ef:	rex.RX cmp %r9b,%al
+   1800c85f2:	movabs %al,0xe08b6ca5d0b5b545
+   1800c85fb:	rex.XB add %eax,(%r8)
+   1800c85fe:	add    %al,(%rax)
+   1800c8600:	cmp    0x73(%r13,%r10,2),%bl
+   1800c8605:	gs jb  0x1800c867b
    1800c8608:	pop    %rsp
    1800c8609:	(bad)
    1800c860f:	rex.R outsl %ds:(%rsi),(%dx)
    1800c8611:	movsxd 0x6d(%rbp),%esi
    1800c8614:	outsb  %gs:(%rsi),(%dx)
    1800c8616:	je     0x1800c868b
    1800c8618:	pop    %rsp
```

### Comparing `scisuit-1.2.3/scisuit/scisuit_pybind310.dll` & `scisuit-1.2.4/scisuit/scisuit_pybind310.dll`

 * *Files 0% similar despite different names*

#### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800153c8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Mon Mar 25 11:47:45 2024
+Time/Date		Tue Apr  2 11:53:45 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	39
 SizeOfCode		0000000000016200
 SizeOfInitializedData	0000000000011400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000153c8
@@ -33337,16 +33337,17 @@
    180019c2d:	add    %al,(%rax)
    180019c2f:	add    %dh,-0x74(%rax)
    180019c32:	add    %eax,0x1(%rax)
    180019c38:	js     0x180019bc6
    180019c3a:	add    %eax,0x1(%rax)
    180019c40:	add    %al,(%rax)
    180019c42:	add    %al,(%rax)
-   180019c44:	(bad)
-   180019c45:	add    %esp,%fs:0x0(%rsi)
+   180019c44:	leave
+   180019c45:	int1
+   180019c46:	or     0x0(%rsi),%esp
    180019c49:	add    %al,(%rax)
    180019c4b:	add    %cl,-0x20000000(%rip)        # 0x160019c51
    180019c51:	add    (%rax),%al
    180019c53:	add    %al,(%rsp,%rbp,4)
    180019c56:	add    %eax,(%rax)
    180019c58:	add    $0x92,%al
    180019c5a:	add    %eax,(%rax)
```

### Comparing `scisuit-1.2.3/scisuit/scisuit_pybind311.dll` & `scisuit-1.2.4/scisuit/scisuit_pybind311.dll`

 * *Files 0% similar despite different names*

#### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800153c8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Mon Mar 25 11:48:36 2024
+Time/Date		Tue Apr  2 11:51:54 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	39
 SizeOfCode		0000000000016200
 SizeOfInitializedData	0000000000011400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000153c8
@@ -33338,16 +33338,17 @@
    180019c2d:	add    %al,(%rax)
    180019c2f:	add    %dh,-0x74(%rax)
    180019c32:	add    %eax,0x1(%rax)
    180019c38:	js     0x180019bc6
    180019c3a:	add    %eax,0x1(%rax)
    180019c40:	add    %al,(%rax)
    180019c42:	add    %al,(%rax)
-   180019c44:	xchg   %eax,%esp
-   180019c45:	add    %esp,%fs:0x0(%rsi)
+   180019c44:	pop    %rdx
+   180019c45:	int1
+   180019c46:	or     0x0(%rsi),%esp
    180019c49:	add    %al,(%rax)
    180019c4b:	add    %cl,-0x20000000(%rip)        # 0x160019c51
    180019c51:	add    (%rax),%al
    180019c53:	add    %al,(%rsp,%rbp,4)
    180019c56:	add    %eax,(%rax)
    180019c58:	add    $0x92,%al
    180019c5a:	add    %eax,(%rax)
```

### Comparing `scisuit-1.2.3/scisuit/scisuit_pybind312.dll` & `scisuit-1.2.4/scisuit/scisuit_pybind312.dll`

 * *Files 1% similar despite different names*

#### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180015408
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Mon Mar 25 11:49:22 2024
+Time/Date		Tue Apr  2 11:54:26 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	39
 SizeOfCode		0000000000016200
 SizeOfInitializedData	0000000000011400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000015408
@@ -33366,18 +33366,18 @@
    180019c2d:	add    %al,(%rax)
    180019c2f:	add    %dh,-0x74(%rax)
    180019c32:	add    %eax,0x1(%rax)
    180019c38:	js     0x180019bc6
    180019c3a:	add    %eax,0x1(%rax)
    180019c40:	add    %al,(%rax)
    180019c42:	add    %al,(%rax)
-   180019c44:	ret    $0x164
-   180019c47:	data16 add %al,(%rax)
-   180019c4a:	add    %al,(%rax)
-   180019c4c:	or     $0xe0000000,%eax
+   180019c44:	repnz int1
+   180019c46:	or     0x0(%rsi),%esp
+   180019c49:	add    %al,(%rax)
+   180019c4b:	add    %cl,-0x20000000(%rip)        # 0x160019c51
    180019c51:	add    (%rax),%al
    180019c53:	add    %al,(%rsp,%rbp,4)
    180019c56:	add    %eax,(%rax)
    180019c58:	add    $0x92,%al
    180019c5a:	add    %eax,(%rax)
 	...
    180019c80:	add    %eax,(%rax)
```

### Comparing `scisuit-1.2.3/scisuit/stats/__init__.py` & `scisuit-1.2.4/scisuit/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `scisuit-1.2.3/scisuit/stats/aov.py` & `scisuit-1.2.4/scisuit/stats/aov.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import math
 import numbers
 import numpy as np
 from dataclasses import dataclass
+from typing import Iterable
 
 from .distributions import pf
 from ..fitting import linearinterp
 
 
 __all__ = ['aov', 'aov2_results', 'aov']
 
@@ -58,14 +59,27 @@
 		v = arr.mean(axis = 0)
 		MatAverage.append(v.tolist())
 	return MatAverage
 
 
 
 
+@dataclass
+class aov_results:
+	Treat_DF:int
+	Treat_SS:float
+	Treat_MS:float
+	Error_DF:int
+	Error_SS:float
+	Error_MS:float
+	Total_DF:int
+	Total_SS:float
+	Total_MS:float
+	Fvalue:float
+
 
 
 class aov: 
 
 	class TukeyComparison:
 		def __init__(self) -> None:
 			self.m_a=None
@@ -82,100 +96,103 @@
 				str(round(self.m_CILow, 2)) + \
 				"," \
 				+ str(round(self.m_CIHigh, 2))
 			return retStr
 
 
 	def __init__(self, *args) -> None:
-		self.m_args = args
-		self.m_Averages = []
-		self.m_SampleSizes = []
+		self._args = args
+		self._Averages = []
+		self._SampleSizes = []
 
 		self.m_MSError=None
 		self.m_DFTreatment=None
 		self.m_DFError=None
 		self.m_TukeyTable=[]
 		self.m_pvalue = None
 
 
 
-	def compute(self):
+	def compute(self)->tuple[float, aov_results]:
 		SS_Treatment, SS_Error, SS_Total=0, 0, 0
 		NEntries = 0
 
 		#C is a variable defined to speed up computations (see Larsen Marx Chapter 12 on ANOVA)
-		C = 0
+		_c = 0.0
 
-		for elem in self.m_args:
+		for elem in self._args:
 			TypeOK=isinstance(elem, list) or isinstance(elem, np.ndarray)
 			if(TypeOK == False):
 				raise TypeError("list/ndarray expected")
 
 			ElemSize = len(elem)
-			LocalSum=0
+			LocalSum = 0.0
 			
 			for entry in elem:
 				LocalSum += entry
 				SS_Total += entry**2
 			
 			#Required for Tukey test
-			self.m_Averages.append(LocalSum/ElemSize)
-			self.m_SampleSizes.append(ElemSize) 
+			self._Averages.append(LocalSum/ElemSize)
+			self._SampleSizes.append(ElemSize) 
 
-			C += LocalSum
+			_c += LocalSum
 			NEntries += ElemSize
 			SS_Treatment += LocalSum**2/ElemSize
 
             
-		C = C**2 / NEntries
+		_c = _c**2 / NEntries
 		
-		SS_Total = SS_Total - C
-		SS_Treatment = SS_Treatment - C
+		SS_Total = SS_Total - _c
+		SS_Treatment = SS_Treatment - _c
 		SS_Error = SS_Total - SS_Treatment
 
-		self.m_DFError, self.m_DFTreatment = NEntries-len(self.m_args), len(self.m_args)-1 
+		self.m_DFError, self.m_DFTreatment = NEntries-len(self._args), len(self._args)-1 
 		DF_Total = self.m_DFError + self.m_DFTreatment
 
 		MS_Treatment, self.m_MSError = SS_Treatment/self.m_DFTreatment , SS_Error/self.m_DFError
 
 		Fvalue = MS_Treatment/self.m_MSError
 
-		self.m_pvalue = 1 - pf(q = Fvalue, df1 = self.m_DFTreatment, df2 = self.m_DFError)
-
-		Dict = dict()
-		Dict["Treatment"] = {'DF':self.m_DFTreatment, 'SS':SS_Treatment, 'MS':MS_Treatment}
-		Dict["Error"] = {'DF':self.m_DFError, 'SS':SS_Error, 'MS':self.m_MSError}
-		Dict["Total"] = {'DF':DF_Total, 'SS':SS_Total, 'MS': SS_Total/DF_Total}
-		Dict["Fvalue"] = Fvalue
+		self.m_pvalue = 1 - pf(q = float(Fvalue), df1 = self.m_DFTreatment, df2 = self.m_DFError)
 
+		ResultCls = aov_results(
+			Treat_DF=self.m_DFTreatment,
+			Treat_MS=MS_Treatment,
+			Treat_SS=SS_Treatment,
+			Error_DF=self.m_DFError,
+			Error_SS=SS_Error,
+			Error_MS=self.m_MSError,
+			Total_DF=DF_Total,
+			Total_SS=SS_Total,
+			Total_MS=SS_Total/DF_Total,
+			Fvalue=Fvalue)
 
-		return self.m_pvalue, Dict
+		return self.m_pvalue, ResultCls
 
 
 
-	def tukey(self, Alpha)->list:
+	def tukey(self, alpha)->list:
 		"""
-		perform tukey test \n
-
-		tukey(Alpha)-> list
+		perform tukey test
 		"""
 		
-		if(len(self.m_Averages) == 0):
+		if(len(self._Averages) == 0):
 			raise RuntimeError("first compute must be called")
 		
-		if(isinstance(Alpha, numbers.Number) == False):
+		if(isinstance(alpha, numbers.Number) == False):
 			raise TypeError("Alpha must be of type number")
 
-		D = qdist(1-Alpha, self.m_DFTreatment-1, self.m_DFError-1) / math.sqrt(self.m_SampleSizes[0])
+		D = qdist(1-alpha, self.m_DFTreatment-1, self.m_DFError-1) / math.sqrt(self._SampleSizes[0])
 		ConfIntervalLength = D*math.sqrt(self.m_MSError)
 
 		self.m_TukeyTable=[]
-		for i in range(len(self.m_Averages)):
-			for j in range(i+1, len(self.m_Averages)):
-				MeanValueDiff = self.m_Averages[i]-self.m_Averages[j]
+		for i in range(len(self._Averages)):
+			for j in range(i+1, len(self._Averages)):
+				MeanValueDiff = self._Averages[i]-self._Averages[j]
 				ConfInterval1 = MeanValueDiff-ConfIntervalLength
 				ConfInterval2 = MeanValueDiff+ConfIntervalLength
 
 				com = self.TukeyComparison()
 
 				com.m_a=i
 				com.m_b=j
@@ -184,29 +201,20 @@
 				com.m_CIHigh = max(ConfInterval1,ConfInterval2)
 
 				self.m_TukeyTable.append(com)
 
 		return self.m_TukeyTable
 
 
-	def __str__(self) -> str:
-		if(isinstance(self.m_pvalue, numbers.Number) == False):
-				raise RuntimeError("compute method has not been called")
-		
-		retStr= "p-value = " + str(self.m_pvalue) + "\n"
 
-		retStr += "Pairs \t \t Diff  \t \t Tukey Interval"
-		retStr +="\n"
-		
-		for Entry in self.m_TukeyTable:
-				retStr += str(Entry)
-				retStr += "\n"
-		
-		return retStr
-	
+
+"""
+-------------------------------------------------------------------------------------------
+-------------------------------------------------------------------------------------------
+"""
 
 
 
 @dataclass
 class aov2_results():
 	DFError:int; DFFact1:int; DFFact2:int; DFinteract:int
 	FvalFact1:float; FvalFact2:float; Fvalinteract:float
@@ -214,20 +222,22 @@
 	pvalFact1:float; pvalFact2:float; pvalinteract:float
 	SSError:float; SSFact1:float; SSFact2:float; SSinteract:float
 
 	Residuals:list
 	Fits:list
 
 
-def aov2(y, x1, x2):
+def aov2(
+		y:Iterable, 
+		x1:Iterable, 
+		x2:Iterable)->aov2_results:
 	"""
 	Performs 2-way ANOVA
 
-	## Input
-	y: Responses \n
+	y: Responses
 	x1, x2: factors
 	"""
 	X1 = x1
 	if isinstance(x1, list):
 		X1 = np.asfarray(x1)
 	
 	X2 = x2
@@ -273,26 +283,26 @@
 
 	meanj = MatAverage.mean(axis = 0)
 	meani = MatAverage.transpose().mean(axis = 0)
 
 	DFFact1, DFFact2 = len(v1) - 1, len(v2) - 1
 	SSFact1 = np.sum((meanj - GrandMean)**2) * Nreplicate * len(v2)
 	SSFact2 = np.sum((meani - GrandMean)**2) * Nreplicate * len(v1)
-	MSFact1, MSFact2 = SSFact1 / DFFact1, SSFact2 / DFFact2
+	MSFact1, MSFact2 = float(SSFact1) / DFFact1, float(SSFact2) / DFFact2
 
 	SSinteract = 0
 	for i in range(len(v2)):
 		for j in range(len(v1)):
 			SSinteract += (MatAverage[i, j] - meanj[j] - meani[i] + GrandMean)**2
 
 	SSinteract *= Nreplicate
 	DFinteract = DFFact1 * DFFact2
 	MSinteract = SSinteract / DFinteract
 
-	FvalFact1, FvalFact2, Fvalinteract = MSFact1 / MSerror, MSFact2 / MSerror, MSinteract / MSerror
+	FvalFact1, FvalFact2, Fvalinteract = float(MSFact1 / MSerror), float(MSFact2 / MSerror), float(MSinteract / MSerror)
 	pvalFact1 = 1.0 - pf(FvalFact1, DFFact1, DFerror)
 	pvalFact2 = 1.0 - pf(FvalFact2, DFFact2, DFerror)
 	pvalinteract = 1.0 - pf(Fvalinteract, DFinteract, DFerror)
 
 	return aov2_results(
 		DFError=DFerror, DFFact1=DFFact1, DFFact2=DFFact2,DFinteract=DFinteract,
 		FvalFact1=FvalFact1, FvalFact2 =FvalFact2, Fvalinteract = Fvalinteract,
```

### Comparing `scisuit-1.2.3/scisuit/stats/core.py` & `scisuit-1.2.4/scisuit/stats/core.py`

 * *Files identical despite different names*

### Comparing `scisuit-1.2.3/scisuit/stats/distributions.py` & `scisuit-1.2.4/scisuit/stats/distributions.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,35 +10,35 @@
 
 def dbeta(x:Iterable|Real, shape1:float, shape2:float)->list|Real:
 	"""
 	shape1, shape2: similar to alpha and beta
 	"""
 	assert shape1>0, "shape1>0 expected"
 	assert shape2>0, "shape2>0 expected"
-	return _pydll.c_stat_dbeta(x, _ct.c_double(shape1), _ct.c_double(shape2))
+	return _pydll.c_stat_dbeta(_ct.py_object(x), _ct.c_double(shape1), _ct.c_double(shape2))
 
 
 def pbeta(q:Iterable|Real, shape1:float, shape2:float)->list|Real:
 	"""
 	shape1, shape2: similar to alpha and beta
 	"""
 	assert shape1>0, "shape1>0 expected"
 	assert shape2>0, "shape2>0 expected"
 
-	return _pydll.c_stat_pbeta(q, _ct.c_double(shape1), _ct.c_double(shape2))
+	return _pydll.c_stat_pbeta(_ct.py_object(q), _ct.c_double(shape1), _ct.c_double(shape2))
 
 
 def qbeta(p:Iterable|Real, shape1:float, shape2:float)->list|Real:
 	"""
 	shape1, shape2: similar to alpha and beta
 	"""
 	assert shape1>0, "shape1>0 expected"
 	assert shape2>0, "shape2>0 expected"
 
-	return _pydll.c_stat_qbeta(p, _ct.c_double(shape1), _ct.c_double(shape2))
+	return _pydll.c_stat_qbeta(_ct.py_object(p), _ct.c_double(shape1), _ct.c_double(shape2))
 	
 
 def rbeta(n:int, shape1:float, shape2:float)->list:
 	"""
 	shape1, shape2: similar to alpha and beta
 	"""
 	assert n>0 ,"n>0 expected"
@@ -52,37 +52,37 @@
 # ----- Binomial Distribution  -------
 
 def dbinom(x:Iterable|Real, size:int, prob:float)->list|Real:
 	"""
 	size: number of trials
 	prob: probability of success in each trial
 	"""
-	return _pydll.c_stat_dbinom(x, _ct.c_int(size), _ct.c_double(prob))
+	return _pydll.c_stat_dbinom(_ct.py_object(x), _ct.c_int(size), _ct.c_double(prob))
 
 
 def pbinom(q:Iterable|Real, size:int, prob:float)->list|Real:
 	"""
 	size: number of trials
 	prob: probability of success in each trial
 	"""
 	assert size>0, "size>0 expected"
 	assert prob>=0 and prob<=1, "prob in [0, 1] expected"
 
-	return _pydll.c_stat_pbinom(q, _ct.c_int(size), _ct.c_double(prob))
+	return _pydll.c_stat_pbinom(_ct.py_object(q), _ct.c_int(size), _ct.c_double(prob))
 
 
 def qbinom(p:Iterable|Real, size:int, prob:float)->list|Real:
 	"""
 	size: number of trials
 	prob: probability of success in each trial
 	"""
 	assert size>0, "size>0 expected"
 	assert prob>=0 and prob<=1, "prob in [0, 1] expected"
 
-	return _pydll.c_stat_qbinom(p, _ct.c_int(size), _ct.c_double(prob))
+	return _pydll.c_stat_qbinom(_ct.py_object(p), _ct.c_int(size), _ct.c_double(prob))
 	
 
 def rbinom(n:int, size:int, prob:float)->list:
 	"""
 	size: number of trials
 	prob: probability of success in each trial
 	"""
@@ -102,38 +102,38 @@
 	x: quantiles representing number of failures
 	size: target for number of successful trials
 	prob: probability of success in each trial
 	"""
 	assert size>0, "size>0 expected"
 	assert prob>=0 and prob<=1, "prob in [0, 1] expected"
 
-	return _pydll.c_stat_dnbinom(x, _ct.c_int(size), _ct.c_double(prob))
+	return _pydll.c_stat_dnbinom(_ct.py_object(x), _ct.c_int(size), _ct.c_double(prob))
 
 
 def pnbinom(q:Iterable|Real, size:int, prob:float)->list|Real:
 	"""
 	q: quantiles representing number of failures
 	size: target for number of successful trials
 	prob: probability of success in each trial
 	"""
 	assert size>0, "size>0 expected"
 	assert prob>=0 and prob<=1, "prob in [0, 1] expected"
 
-	return _pydll.c_stat_pnbinom(q, _ct.c_int(size), _ct.c_double(prob))
+	return _pydll.c_stat_pnbinom(_ct.py_object(q), _ct.c_int(size), _ct.c_double(prob))
 
 def qnbinom(p:Iterable|Real, size:int, prob:float)->list|Real:
 	"""
 	p: probabilities
 	size: target for number of successful trials
 	prob: probability of success in each trial
 	"""
 	assert size>0, "size>0 expected"
 	assert prob>=0 and prob<=1, "prob in [0, 1] expected"
 
-	return _pydll.c_stat_qnbinom(p, _ct.c_int(size), _ct.c_double(prob))
+	return _pydll.c_stat_qnbinom(_ct.py_object(p), _ct.c_int(size), _ct.c_double(prob))
 
 
 def rnbinom(n:int, size, prob)->list:
 	"""
 	size: target for number of successful trials
 	prob: probability of success in each trial
 	"""
@@ -156,15 +156,15 @@
 	## Note:
 	Internally sum of probabilities is normalized to 1.0
 	"""
 
 	assert sum(x) == size, "sum(x) == size expected."
 	assert size>0, "size>0 expected"
 
-	return _pydll.c_stat_dmultinom(x, _ct.c_int(size), prob)
+	return _pydll.c_stat_dmultinom(_ct.py_object(x), _ct.c_int(size), prob)
 
 
 def rmultinom(n:int, size:int, prob:Iterable)->list:
 	"""
 	size: number of trials
 	prob: probabilities of success in each trial
 
@@ -187,32 +187,31 @@
 # ----- Chi-Square Distribution  -------
 
 def dchisq(x:Iterable|Real, df:int)->list|Real:
 	"""
 	df: degrees of freedom
 	"""
 	assert df>0, "df>0 expected"
+	return _pydll.c_stat_dchisq(_ct.py_object(x), _ct.c_int(df))
 
-	return _pydll.c_stat_dchisq(x, _ct.c_int(df))
 
 def pchisq(q:Iterable|Real, df:int)->list|Real:
 	"""
 	df: degrees of freedom
 	"""
-	assert df>0, "df>0 expected"
-	
-	return _pydll.c_stat_pchisq(q, _ct.c_int(df))
+	assert df>0, "df>0 expected"	
+	return _pydll.c_stat_pchisq(_ct.py_object(q), _ct.c_int(df))
+
 
 def qchisq(p:Iterable|Real, df:int)->list|Real:
 	"""
 	df: degrees of freedom
 	"""
 	assert df>0, "df>0 expected"
-	
-	return _pydll.c_stat_qchisq(p, _ct.c_int(df))
+	return _pydll.c_stat_qchisq(_ct.py_object(p), _ct.c_int(df))
 
 
 def rchisq(n:int, df)->list:
 	"""
 	df: degrees of freedom
 	"""
 	assert n>0 ,"n>0 expected"
@@ -225,31 +224,31 @@
 # ----- Exponential Distribution  -------
 
 def dexp(x:Iterable|Real, rate = 1.0)->list|Real:
 	"""
 	x: quantiles
 	rate: 1/mean, where mean is the waiting time for the next event recurrence
 	"""
-	return _pydll.c_stat_dexp(x, _ct.c_double(rate))
+	return _pydll.c_stat_dexp(_ct.py_object(x), _ct.c_double(rate))
 
 
 def pexp(q:Iterable|Real, rate = 1.0)->list|Real:
 	"""
 	q: quantiles
 	rate: 1/mean, where mean is the waiting time for the next event recurrence
 	"""
-	return _pydll.c_stat_pexp(q,  _ct.c_double(rate))
+	return _pydll.c_stat_pexp(_ct.py_object(q),  _ct.c_double(rate))
 
 
 def qexp(p:Iterable|Real, rate = 1.0)->list|Real:
 	"""
 	p: probabilities
 	rate: 1/mean, where mean is the waiting time for the next event recurrence
 	"""
-	return _pydll.c_stat_qexp(p,  _ct.c_double(rate))
+	return _pydll.c_stat_qexp(_ct.py_object(p), _ct.c_double(rate))
 
 
 def rexp(n:int, rate=1.0)->list:
 	"""
 	rate: 1/mean, where mean is the waiting time for the next event recurrence
 	"""
 	assert n>0 ,"n>0 expected"
@@ -265,36 +264,36 @@
 	"""
 	df1: degrees of freedom, numerator
 	df2: degrees of freedom, denominator
 	"""
 	assert df1>0, "df1>0 expected"
 	assert df2>0, "df2>0 expected"
 
-	return _pydll.c_stat_df(x, _ct.c_int(df1), _ct.c_int(df2))
+	return _pydll.c_stat_df(_ct.py_object(x), _ct.c_int(df1), _ct.c_int(df2))
 
 
 def pf(q:Iterable|Real, df1:int, df2:int)->list|Real:
 	"""
 	df1: degrees of freedom, numerator
 	df2: degrees of freedom, denominator
 	"""
 	assert df1>0, "df1>0 expected"
 	assert df2>0, "df2>0 expected"
 
-	return _pydll.c_stat_pf(q, _ct.c_int(df1), _ct.c_int(df2))
+	return _pydll.c_stat_pf(_ct.py_object(q), _ct.c_int(df1), _ct.c_int(df2))
 
 def qf(p:Iterable|Real, df1:int, df2:int)->list|Real:
 	"""
 	df1: degrees of freedom, numerator
 	df2: degrees of freedom, denominator
 	"""
 	assert df1>0, "df1>0 expected"
 	assert df2>0, "df2>0 expected"
 
-	return _pydll.c_stat_qf(p, _ct.c_int(df1), _ct.c_int(df2))
+	return _pydll.c_stat_qf(_ct.py_object(p), _ct.c_int(df1), _ct.c_int(df2))
 
 
 def rf(n:int, df1, df2)->list:
 	"""
 	df1: degrees of freedom, numerator
 	df2: degrees of freedom, denominator
 	"""
@@ -305,42 +304,42 @@
 	return _np.random.f(size=n, dfnum=df1, dfden=df2).tolist()
 
 
 
 
 # ----- Gamma Distribution  -------
 
-def dgamma(x:Iterable|Real, shape:float, scale = 1.0)->list|Real:
+def dgamma(x:Iterable|Real, shape:Real, scale = 1.0)->list|Real:
 	"""
 	x: quantile	
 	shape: waiting time for the rth event to occur
 	scale: average waiting time for the next event recurrence
 	"""
-	return _pydll.c_stat_dgamma(x, _ct.c_double(shape), _ct.c_double(scale))
+	return _pydll.c_stat_dgamma(_ct.py_object(x), _ct.c_double(shape), _ct.c_double(scale))
 
 
 def pgamma(q:Iterable|Real, shape:float, scale = 1.0)->list|Real:
 	"""
 	q: quantile
 	shape: waiting time for the rth event to occur
 	scale: average waiting time for the next event recurrence
 	"""
-	return _pydll.c_stat_pgamma(q, _ct.c_double(shape), _ct.c_double(scale))
+	return _pydll.c_stat_pgamma(_ct.py_object(q), _ct.c_double(shape), _ct.c_double(scale))
 
 
-def qgamma(p:Iterable|Real, shape:float, scale = 1.0)->list|Real:
+def qgamma(p:Iterable|Real, shape:Real, scale = 1.0)->list|Real:
 	"""
 	p: probabilities
 	shape: waiting time for the rth event to occur
 	scale: average waiting time for the next event recurrence
 	"""
-	return _pydll.c_stat_qgamma(p, _ct.c_double(shape), _ct.c_double(scale))
+	return _pydll.c_stat_qgamma(_ct.py_object(p), _ct.c_double(shape), _ct.c_double(scale))
 
 
-def rgamma(n:int, shape:float, scale=1.0)->list:
+def rgamma(n:int, shape:Real, scale=1.0)->list:
 	"""
 	Draw samples from gamma distribution
 	"""
 	assert n>0 ,"n>0 expected"
 	assert shape>0, "shape>0 expected"
 	assert scale>0, "scale>0 expected"
 
@@ -352,33 +351,34 @@
 # ----- Geometric Distribution  -------
 
 def dgeom(x:Iterable|Real, prob:float)->list|Real:
 	"""
 	x: Number of failures before success occurs.
 	prob: probability of success in each trial.
 	"""
-	return _pydll.c_stat_dgeom(x, _ct.c_double(prob))
+	return _pydll.c_stat_dgeom(_ct.py_object(x), _ct.c_double(prob))
 
 
-def pgeom(q:Iterable|Real, prob:float)->list|Real:
+def pgeom(q:Iterable|Real, prob:Real)->list|Real:
 	"""
 	q: Number of failures before success occurs.
 	prob: probability of success in each trial.
 	"""
-	return _pydll.c_stat_pgeom(q, _ct.c_double(prob))
+	return _pydll.c_stat_pgeom(_ct.py_object(q), _ct.c_double(prob))
 
-def qgeom(p:Iterable|Real, prob:float)->list|Real:
+
+def qgeom(p:Iterable|Real, prob:Real)->list|Real:
 	"""
 	p: probabilities
 	prob: probability of success in each trial.
 	"""
-	return _pydll.c_stat_qgeom(p, _ct.c_double(prob))
+	return _pydll.c_stat_qgeom(_ct.py_object(p), _ct.c_double(prob))
 
 
-def rgeom(n:int, prob)->list:
+def rgeom(n:int, prob:Real)->list:
 	"""
 	Draw samples from geometric distribution
 	"""
 	assert n>0 ,"n>0 expected"
 	assert prob>=0 and prob<=1, "prob in [0, 1] expected"
 
 	return _np.random.geometric(size=n, p=prob).tolist()
@@ -390,33 +390,33 @@
 
 def dhyper(x:Iterable|Real, m:int, n:int, k:int)->list|Real:
 	"""
 	m: number of good samples in the urn
 	n: number of bad samples in the urn
 	k: samples drawn from the urn
 	"""
-	return _pydll.c_stat_dhyper(x, _ct.c_int(m), _ct.c_int(n), _ct.c_int(k))
+	return _pydll.c_stat_dhyper(_ct.py_object(x), _ct.c_int(m), _ct.c_int(n), _ct.c_int(k))
 
 
 def phyper(q:Iterable|Real, m:int, n:int, k:int)->list|Real:
 	"""
 	m: number of good samples in the urn
 	n: number of bad samples in the urn
 	k: samples drawn from the urn
 	"""
-	return _pydll.c_stat_phyper(q, _ct.c_int(m), _ct.c_int(n), _ct.c_int(k))
+	return _pydll.c_stat_phyper(_ct.py_object(q), _ct.c_int(m), _ct.c_int(n), _ct.c_int(k))
 
 
 def qhyper(p:Iterable|Real, m:int, n:int, k:int)->list|Real:
 	"""
 	m: number of good samples in the urn
 	n: number of bad samples in the urn
 	k: samples drawn from the urn
 	"""
-	return _pydll.c_stat_qhyper(p, _ct.c_int(m), _ct.c_int(n), _ct.c_int(k))
+	return _pydll.c_stat_qhyper(_ct.py_object(p), _ct.c_int(m), _ct.c_int(n), _ct.c_int(k))
 
 
 def rhyper(nn:int, m:int, n:int, k:int)->list:
 	"""
 	m: number of good samples in the urn
 	n: number of bad samples in the urn
 	k: samples drawn from the urn
@@ -434,31 +434,31 @@
 # ----- Normal Distribution  -------
 
 def dnorm(x:Iterable|Real, mean=0.0, sd=1.0)->list|Real:
 	"""
 	mean: mean value of the distribution
 	sd: standard deviation of the distribution
 	"""
-	return _pydll.c_stat_dnorm(x, _ct.c_double(mean), _ct.c_double(sd))
+	return _pydll.c_stat_dnorm(_ct.py_object(x), _ct.c_double(mean), _ct.c_double(sd))
 
 
 def pnorm(q:Iterable|Real, mean=0.0, sd=1.0)->list|Real:
 	"""
 	mean: mean value of the distribution
 	sd: standard deviation of the distribution
 	"""
-	return _pydll.c_stat_pnorm(q, _ct.c_double(mean), _ct.c_double(sd))
+	return _pydll.c_stat_pnorm(_ct.py_object(q), _ct.c_double(mean), _ct.c_double(sd))
 
 
 def qnorm(p:Iterable|Real, mean=0.0, sd=1.0)->list|Real:
 	"""
 	mean: mean value of the distribution
 	sd: standard deviation of the distribution
 	"""
-	return _pydll.c_stat_qnorm(p, _ct.c_double(mean), _ct.c_double(sd))
+	return _pydll.c_stat_qnorm(_ct.py_object(p), _ct.c_double(mean), _ct.c_double(sd))
 
 
 def rnorm(n:int, mean=0.0, sd=1.0)->list:
 	"""
 	mean: mean value of the distribution
 	sd: standard deviation of the distribution
 	"""
@@ -473,31 +473,31 @@
 # ----- Log Normal Distribution  -------
 
 def dlnorm(x:Iterable|Real, meanlog=0.0, sdlog=1.0)->list|Real:
 	"""
 	meanlog: mean value of the distribution
 	sdlog: standard deviation of the distribution
 	"""
-	return _pydll.c_stat_dlnorm(x, _ct.c_double(meanlog), _ct.c_double(sdlog))
+	return _pydll.c_stat_dlnorm(_ct.py_object(x), _ct.c_double(meanlog), _ct.c_double(sdlog))
 
 
 def plnorm(q:Iterable|Real, meanlog=0.0, sdlog=1.0)->list|Real:
 	"""
 	mean: mean value of the distribution
 	sd: standard deviation of the distribution
 	"""
-	return _pydll.c_stat_plnorm(q, _ct.c_double(meanlog), _ct.c_double(sdlog))
+	return _pydll.c_stat_plnorm(_ct.py_object(q), _ct.c_double(meanlog), _ct.c_double(sdlog))
 
 
 def qlnorm(p:Iterable|Real, meanlog=0.0, sdlog=1.0)->list|Real:
 	"""
 	mean: mean value of the distribution
 	sd: standard deviation of the distribution
 	"""
-	return _pydll.c_stat_qlnorm(p, _ct.c_double(meanlog), _ct.c_double(sdlog))
+	return _pydll.c_stat_qlnorm(_ct.py_object(p), _ct.c_double(meanlog), _ct.c_double(sdlog))
 
 
 def rlnorm(n:int, meanlog=0.0, sdlog=1.0)->list:
 	"""
 	mean: mean value of the distribution
 	sd: standard deviation of the distribution
 	"""
@@ -507,42 +507,42 @@
 	return _np.random.lognormal(size=n, mean=meanlog, sigma=sdlog).tolist()
 
 
 
 
 # ----- Pareto Distribution  -------
 
-def dpareto(x:Iterable|Real, location, shape=1.0)->list|Real:
+def dpareto(x:Iterable|Real, location:Real, shape=1.0)->list|Real:
 	"""
 	location: location parameter
 	shape: shape parameter
 	"""
 	assert location>0 and shape>0, "'location' and 'shape' must be positive"
-	return _pydll.c_stat_dpareto(x, _ct.c_double(location), _ct.c_double(shape))
+	return _pydll.c_stat_dpareto(_ct.py_object(x), _ct.c_double(location), _ct.c_double(shape))
 
 
-def ppareto(q:Iterable|Real, location, shape=1.0)->list|Real:
+def ppareto(q:Iterable|Real, location:Real, shape=1.0)->list|Real:
 	"""
 	location: location parameter
 	shape: shape parameter
 	"""
 	assert location>0 and shape>0, "'location' and 'shape' must be positive"
-	return _pydll.c_stat_ppareto(q, _ct.c_double(location), _ct.c_double(shape))
+	return _pydll.c_stat_ppareto(_ct.py_object(q), _ct.c_double(location), _ct.c_double(shape))
 
 
-def qpareto(p:Iterable|Real, location, shape=1.0)->list|Real:
+def qpareto(p:Iterable|Real, location:Real, shape=1.0)->list|Real:
 	"""
 	location: location parameter
 	shape: shape parameter
 	"""
 	assert location>0 and shape>0, "'location' and 'shape' must be positive"
-	return _pydll.c_stat_qpareto(p, _ct.c_double(location), _ct.c_double(shape))
+	return _pydll.c_stat_qpareto(_ct.py_object(p), _ct.c_double(location), _ct.c_double(shape))
 
 
-def rpareto(n:int, location, shape=1.0)->list:
+def rpareto(n:int, location:Real, shape=1.0)->list:
 	"""
 	location: location parameter
 	shape: shape parameter
 	"""
 	assert location>0 and shape>0, "'location' and 'shape' must be positive"
 	assert n>0 ,"n>0 expected"
 	
@@ -550,23 +550,23 @@
 
 
 
 
 # ----- Poisson Distribution  -------
 
 def dpois(x:Iterable|Real, mu:float)->list|Real:
-	return _pydll.c_stat_dpois(x, _ct.c_double(mu))
+	return _pydll.c_stat_dpois(_ct.py_object(x), _ct.c_double(mu))
 
 
 def ppois(q:Iterable|Real, mu:float)->list|Real:
-	return _pydll.c_stat_ppois(q, _ct.c_double(mu))
+	return _pydll.c_stat_ppois(_ct.py_object(q), _ct.c_double(mu))
 
 
 def qpois(p:Iterable|Real, mu:float)->list|Real:
-	return _pydll.c_stat_qpois(p, _ct.c_double(mu))
+	return _pydll.c_stat_qpois(_ct.py_object(p), _ct.c_double(mu))
 
 
 def rpois(n:int, mu = 1)->list:
 	"""
 	Draw samples from Poisson distribution
 	"""
 	assert n>0 ,"n>0 expected"
@@ -581,92 +581,77 @@
 
 def dt(x:Iterable|Real, df:int)->list|Real:
 	"""
 	df: degrees of freedom
 	"""
 	assert df>0, "df>0 expected"
 
-	return _pydll.c_stat_dt(x, _ct.c_int(df))
+	return _pydll.c_stat_dt(_ct.py_object(x), _ct.c_int(df))
 
 
 def pt(q:Iterable|Real, df:int)->list|Real:
 	"""
 	df: degrees of freedom
 	"""
 	assert df>0, "df>0 expected"
 
-	return _pydll.c_stat_pt(q, _ct.c_int(df))
+	return _pydll.c_stat_pt(_ct.py_object(q), _ct.c_int(df))
 
 
 def qt(p:Iterable|Real, df:int)->list|Real:
 	"""
 	df: degrees of freedom
 	"""
 	assert df>0, "df>0 expected"
 
-	return _pydll.c_stat_qt(p, _ct.c_int(df))
+	return _pydll.c_stat_qt(_ct.py_object(p), _ct.c_int(df))
 
 
 def rt(n:int, df)->list:
 	"""
 	df: degrees of freedom
 	"""
 	assert n>0 ,"n>0 expected"
 	assert df>0, "df1>0 expected"
 
 	return _np.random.standard_t(size=n, df=df).tolist()
 
 
 
 
-# ----- Wilcoxon Sign Rank Distribution  -------
-
-def dsignrank(x:Iterable|Real, n:int)->list|Real:
-	return _pydll.c_stat_dsignrank(x, _ct.c_int(n))
-
-
-def psignrank(q:Iterable|Real, n:int)->list|Real:
-	return _pydll.c_stat_psignrank(q, _ct.c_int(n))
-
-
-def qsignrank(p:Iterable|Real, n:int)->list|Real:
-	return _pydll.c_stat_qsignrank(p, _ct.c_int(n))
-
-
-
 # ----- Uniform Distribution  -------
 
 def dunif(x:Iterable|Real, min=0.0, max=1.0)->list|Real:
 	"""
 	min: minimum bound
 	max: maximum bound
 	"""
 	assert max>min, "max>min expected"
 
-	return _pydll.c_stat_dunif(x, _ct.c_double(min), _ct.c_double(max))
+	return _pydll.c_stat_dunif(_ct.py_object(x), _ct.c_double(min), _ct.c_double(max))
 
 
 def punif(q:Iterable|Real, min=0.0, max=1.0)->list|Real:
 	"""
 	min: minimum bound
 	max: maximum bound
 	"""
 	assert max>min, "max>min expected"
 
-	return _pydll.c_stat_punif(q, _ct.c_double(min), _ct.c_double(max))
+	return _pydll.c_stat_punif(_ct.py_object(q), _ct.c_double(min), _ct.c_double(max))
 
 
 def qunif(p:Iterable|Real, min=0.0, max=1.0)->list|Real:
 	"""
 	min: minimum bound
 	max: maximum bound
 	"""
 	assert max>min, "max>min expected"
 
-	return _pydll.c_stat_qunif(p, _ct.c_double(min), _ct.c_double(max))
+	return _pydll.c_stat_qunif(_ct.py_object(p), _ct.c_double(min), _ct.c_double(max))
 
 
 def runif(n:int, min=0.0, max=1.0)->list:
 	"""
 	min: minimum bound
 	max: maximum bound
 	"""
@@ -684,43 +669,58 @@
 	x: quantile	
 	shape: known as Weibull-slope
 	scale: characteristic life
 	"""
 	assert shape>0, "shape>0 expected"
 	assert scale>0, "scale>0 expected"
 
-	return _pydll.c_stat_dweibull(x, _ct.c_double(shape), _ct.c_double(scale))
+	return _pydll.c_stat_dweibull(_ct.py_object(x), _ct.c_double(shape), _ct.c_double(scale))
 
 
 def pweibull(q:Iterable|Real, shape:float, scale = 1.0)->list|Real:
 	"""
 	q: quantile
 	shape: known as Weibull-slope
 	scale: characteristic life
 	"""
 	assert shape>0, "shape>0 expected"
 	assert scale>0, "scale>0 expected"
 
-	return _pydll.c_stat_pweibull(q, _ct.c_double(shape), _ct.c_double(scale))
+	return _pydll.c_stat_pweibull(_ct.py_object(q), _ct.c_double(shape), _ct.c_double(scale))
 
 
 def qweibull(p:Iterable|Real, shape:float, scale = 1.0)->list|Real:
 	"""
 	p: probabilities
 	shape: known as Weibull-slope
 	scale: characteristic life
 	"""
 	assert shape>0, "shape>0 expected"
 	assert scale>0, "scale>0 expected"
 	
-	return _pydll.c_stat_qweibull(p, _ct.c_double(shape), _ct.c_double(scale))
+	return _pydll.c_stat_qweibull(_ct.py_object(p), _ct.c_double(shape), _ct.c_double(scale))
 
 
 def rweibull(n:int, shape:float, scale=1.0)->list:
 	"""
 	Draw samples from weibull distribution
 	"""
 	assert n>0 ,"n>0 expected"
 	assert shape>0, "shape>0 expected"
 	assert scale>0, "scale>0 expected"
 
-	return (scale*_np.random.weibull(size=n, a=shape, )).tolist()
+	return (scale*_np.random.weibull(size=n, a=shape, )).tolist()
+
+
+# ----- Wilcoxon Sign Rank Distribution  -------
+
+def dsignrank(x:Iterable|Real, n:int)->list|Real:
+	return _pydll.c_stat_dsignrank(_ct.py_object(x), _ct.c_int(n))
+
+
+def psignrank(q:Iterable|Real, n:int)->list|Real:
+	return _pydll.c_stat_psignrank(_ct.py_object(q), _ct.c_int(n))
+
+
+def qsignrank(p:Iterable|Real, n:int)->list|Real:
+	return _pydll.c_stat_qsignrank(_ct.py_object(p), _ct.c_int(n))
+
```

### Comparing `scisuit-1.2.3/scisuit/stats/linregress.py` & `scisuit-1.2.4/scisuit/stats/linregress.py`

 * *Files identical despite different names*

### Comparing `scisuit-1.2.3/scisuit/stats/test_basic.py` & `scisuit-1.2.4/scisuit/stats/test_basic.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 * Sign-Test
 * t-tests (1-sample, 2-sample, paired)
 * Z-test
 """
 
 
 import math
+import numbers
+from typing import Iterable
 import numpy as _np
 from .._ctypeslib import pydll as _pydll
 
 from dataclasses import dataclass
 from .distributions import pbinom, pf, qf, pt, qt, pnorm, qnorm
 
 
@@ -33,15 +35,17 @@
 """ *********** Anderson-Darling Test ******************* """
 
 @dataclass
 class TestNormRes:
 	pval:float
 	A2:float
 
-def test_norm_ad(x):
+def test_norm_ad(x:Iterable)->TestNormRes:
+	assert isinstance(x, Iterable), "x must be an Iterable object"
+	
 	pval, A2 = _pydll.c_stat_test_norm_ad(x)
 	return TestNormRes(pval, A2)
 
 
 
 
 
@@ -56,25 +60,30 @@
 	Fcritical:float
 	df1:int; df2:int
 	var1:float; var2:float
 	CI_lower:float; CI_upper:float
 
 
 
-def test_f(x, y, ratio:float = 1.0, alternative:str = "two.sided", conflevel:float = 0.95)->tuple:
+def test_f(
+		x:Iterable, 
+		y:Iterable, 
+		ratio:float = 1.0, 
+		alternative:str = "two.sided", 
+		conflevel:float = 0.95)->tuple[float, test_f_Result]:
 	"""
 	Performs F test
 
 	## Return
-	p-value and test_f_Result class. \n
+	p-value and test_f_Result class.
 
 	## Input
-	x/y: First/second sample, ndarray/list \n
-	alternative: "two.sided", "less", "greater" \n
-	ratio: Assumed ratio of variances of the samples \n
+	x/y: First/second sample
+	alternative: "two.sided", "less", "greater"
+	ratio: Assumed ratio of variances of the samples
 	conflevel: Confidence level, [0,1] 
 	"""
 	assert conflevel>=0.0 or conflevel <= 1.0, "conflevel must be in range (0, 1)"
 	assert isinstance(x, list) or type(x)==_np.ndarray, "x must be list/ndarray"
 	assert isinstance(y, list) or type(y)==_np.ndarray, "y must be list/ndarray"
 
 	XX, YY = x, y
@@ -87,20 +96,19 @@
 	assert _np.issubdtype(XX.dtype, _np.number), "x must contain only numbers"
 	assert _np.issubdtype(YY.dtype, _np.number), "y must contain only numbers"
 
 	alpha = 1 - conflevel
 	df1, df2 = len(XX) - 1, len(YY) -1 #degrees of freedoms
 	
 	var1, var2 = _np.var(XX, ddof = 1), _np.var(YY, ddof = 1)
-	varRatio = var1 / var2
+	varRatio = float(var1) / float(var2)
 
 	Fcritical = varRatio / ratio
 
 	pvalue = 0.0
-
 	if alternative == "two.sided" or alternative == "notequal":
 		#F distribution is non - symmetric
 		a = pf(Fcritical, df1, df2)
 		b = 1 - pf(Fcritical, df1, df2)
 
 		c = pf(1 / Fcritical, df1, df2)
 		d = 1 - pf(1 / Fcritical, df1, df2)
@@ -225,53 +233,51 @@
 
 	return lowerRes, upperRes
 
 
 
 
 
-def test_sign(x, md, y=None, alternative="two.sided", conflevel=0.95):
+def test_sign(
+		x:Iterable, 
+		md:numbers.Real, 
+		y=None, 
+		alternative="two.sided", 
+		conflevel=0.95)->tuple[float, test_sign_Result]:
 	"""
-	
-	## Return
-	p-value and a test_sign_Result class. \n
+	returns p-value and a test_sign_Result class. \n
 
-	## Input
-	x: Sample \n
-	y: Second sample \n
-	md: Median of the population tested by the null hypothesis \n
-	alternative: "two.sided", "less", "greater" \n
+	x: Sample
+	y: Second sample
+	md: Median of the population tested by the null hypothesis
+	alternative: "two.sided", "less", "greater" 
 	conflevel:	Confidence level, [0,1]
 	"""
 
 	NORMALAPPROX = 12
 
-	assert conflevel>=0.0 or conflevel <= 1.0, "conflevel must be in range (0, 1)"
-	assert isinstance(x, list) or type(x)==_np.ndarray, "x must be list/ndarray"
+	assert conflevel>0.0 or conflevel<1.0, "conflevel must be in range (0, 1)"
+	assert isinstance(x, Iterable), "x must be Iterable"
 
-	XX, YY = x, y
-	if isinstance(x, list):
-		XX = _np.asfarray(x)
+	XX = _np.asfarray(x)
 	
 	assert _np.issubdtype(XX.dtype, _np.number), "x must contain only numbers"
 	
 	xvec = XX
 
 	if y != None:
-		assert isinstance(y, list) or type(y)==_np.ndarray, "y must be list/ndarray"
-		if isinstance(y, list):
-			YY = _np.asfarray(y)
+		assert isinstance(y, Iterable), "y must be Iterable"
+		YY = _np.asfarray(y)
 
 		assert _np.issubdtype(YY.dtype, _np.number), "y must contain only numbers"
 		xvec = XX - YY
 	
 	NGreater = len(_np.argwhere(xvec>md))
 
 	EqIndex = _np.where(xvec == md)
-	NEqual = len(EqIndex)
 	xvec = _np.delete(xvec, EqIndex)
 
 	pvalue = 0.0
 
 	NSample = len(xvec)
 
 	if NSample < NORMALAPPROX:
@@ -305,35 +311,35 @@
 
 		elif alternative == "less":
 			#area on the left
 			pvalue = pnorm(zvalue, 0.0, 1.0)
 
 	Lower, Upper = _FindCI(xvec, alternative, conflevel)
 
-	interpolated = CI_Result(pos=-1, prob=conflevel, CILow=0.0, CIHigh=0.0)
+	interped = CI_Result(pos=-1, prob=conflevel, CILow=0.0, CIHigh=0.0)
 	if alternative == "two.sided" or alternative == "notequal":
 		x1, x2 = Lower.prob, Upper.prob
 
-		interpolated.CILow = _np.interp(conflevel, [x1, x2], [Lower.CILow, Upper.CILow] )
-		interpolated.CIHigh = _np.interp(conflevel, [x1, x2], [Lower.CIHigh, Upper.CIHigh])
+		interped.CILow = _np.interp(conflevel, [x1, x2], [Lower.CILow, Upper.CILow] )
+		interped.CIHigh = _np.interp(conflevel, [x1, x2], [Lower.CIHigh, Upper.CIHigh])
 	
 	elif alternative == "greater":
-		interpolated.CILow = _np.interp(conflevel, [Lower.prob, Upper.prob], [Lower.CILow, Upper.CILow])
-		interpolated.CIHigh = math.inf
+		interped.CILow = _np.interp(conflevel, [Lower.prob, Upper.prob], [Lower.CILow, Upper.CILow])
+		interped.CIHigh = math.inf
 	
 	elif alternative == "less":
-		interpolated.CILow = -math.inf
-		interpolated.CIHigh = _np.interp(conflevel, [Lower.prob, Upper.prob], [Lower.CIHigh, Upper.CIHigh])
+		interped.CILow = -math.inf
+		interped.CIHigh = _np.interp(conflevel, [Lower.prob, Upper.prob], [Lower.CIHigh, Upper.CIHigh])
 	
 	else:
 		raise ValueError("Values for 'alternative': \"two.sided\" or \"notequal\", \"greater\", \"less\"")
 
 	result = test_sign_Result(
 		lower= Lower,
-		interpolated=interpolated,
+		interpolated=interped,
 		upper = Upper)
 	
 	return pvalue, result
 
 
 
 
@@ -371,33 +377,35 @@
 	xaver:float; yaver:float
 	s1:float; s2:float; SE:float
 	N:int
 	mean:float #mean of difference
 	stdev:float #stdev of difference
 
 
-def _test_t1(x, mu, alternative="two.sided", conflevel=0.95):
+def _test_t1(
+		x:Iterable, 
+		mu:numbers.Real, 
+		alternative="two.sided", 
+		conflevel=0.95)->tuple[float, test_t1_result]:
 	assert conflevel>=0.0 or conflevel <= 1.0, "conflevel must be in range (0, 1)"
-	assert isinstance(x, list) or type(x)==_np.ndarray, "x must be list/ndarray"
+	assert isinstance(x, Iterable), "x must be Iterable"
 
-	XX = x
-	if isinstance(x, list):
-		XX = _np.asfarray(x)
+	XX = _np.asfarray(x)
 
 	assert len(XX)>= 3, "container must have at least 3 elements"
 	assert _np.issubdtype(XX.dtype, _np.number), "x must contain only numbers"
 
 	N = len(XX)
 	df = N -1
 	
 	stdev = _np.std(XX, ddof =1) #sample's standard deviation
 	SE = stdev / math.sqrt(N) #Standard Error of Mean
 	
 	xaver = _np.mean(XX)
-	tcritical = (xaver - mu) / SE
+	tcritical = float((xaver - mu) / SE)
 
 	pvalue = 0.0
 	if alternative == "two.sided" or alternative == "notequal":
 		if (tcritical <= 0.0):
 			#area on the left of tcrit + area on the right of positive
 			pvalue = pt(tcritical, df) + (1.0 - pt(abs(tcritical), df))
 		else:
@@ -428,55 +436,56 @@
 		mean = xaver,
 		tcritical = tcritical)
 	
 	return pvalue, Result
 
 
 
-def _test_t2(x, y, mu, varequal = True, alternative="two.sided", conflevel=0.95):
+def _test_t2(
+		x:Iterable, 
+		y:Iterable, 
+		mu:numbers.Real, 
+		varequal = True, 
+		alternative="two.sided", 
+		conflevel=0.95)->tuple[float, test_t2_result]:
 	assert conflevel>=0.0 or conflevel <= 1.0, "conflevel must be in range (0, 1)"
-	assert isinstance(x, list) or type(x)==_np.ndarray, "x must be list/ndarray"
+	assert isinstance(x, Iterable), "x must be Iterable"
 
-	XX = x
-	if isinstance(x, list):
-		XX = _np.asfarray(x)
-	
-	YY = y
-	if isinstance(y, list):
-		YY = _np.asfarray(y)
+	XX = _np.asfarray(x)
+	YY = _np.asfarray(y)
 
 	assert len(XX)>= 3, "x must have at least 3 elements"
 	assert len(YY)>= 3, "y must have at least 3 elements"
 	assert _np.issubdtype(XX.dtype, _np.number), "x must contain only numbers"
 	assert _np.issubdtype(YY.dtype, _np.number), "y must contain only numbers"
 
 	n1, n2 = len(XX), len(YY)
-	xaver, yaver = _np.mean(XX), _np.mean(YY)
-	s1, s2 = _np.std(XX, ddof = 1), _np.std(YY, ddof = 1)
+	xaver, yaver = float(_np.mean(XX)), float(_np.mean(YY))
+	s1, s2 = float(_np.std(XX, ddof = 1)), float(_np.std(YY, ddof = 1))
 	var1, var2 = s1**2, s2**2
 	alpha = 1 - conflevel
 
 	tcritical, SE = None, None
 	sp = -1 #pooled
 
 	if varequal == False:
 		df_num = (var1 / n1 + var2 / n2)**2
 		df_denom = 1 / (n1 - 1) * (var1 / n1)**2 + 1 / (n2 - 1) * (var2 / n2)**2
 		df = math.floor(df_num / df_denom)
 
-		tcritical = ((xaver - yaver) - mu) / math.sqrt(var1 / n1 + var2 / n2)
+		tcritical = float((xaver - yaver) - mu) / math.sqrt(var1 / n1 + var2 / n2)
 		SE = math.sqrt(var1 / n1 + var2 / n2)
 	
 	else:
 		df = n1 + n2 - 2
 
 		sp_num = (n1 - 1) * var1 + (n2 - 1) * var2
 		sp = math.sqrt(sp_num / df)
 
-		tcritical = ((xaver - yaver) - mu) / (sp * math.sqrt(1 / n1 + 1 / n2))
+		tcritical = float((xaver - yaver) - mu) / (sp * math.sqrt(1 / n1 + 1 / n2))
 		SE = sp * math.sqrt(1 / n1 + 1 / n2)
 	
 	pvalue = 0
 	if alternative == "two.sided" or alternative == "notequal":
 		if tcritical <= 0:
 			#area on the left of tcrit + area on the right of positive
 			pvalue = pt(tcritical, df) + (1 - pt(abs(tcritical), df))
@@ -510,17 +519,17 @@
 		df=df,
 		s1 = s1, s2=s2, sp=sp,
 		xaver = xaver, yaver = yaver)
 	
 	return pvalue, Result
 
 
-def _test_t_paired(x, y, mu, alternative="two.sided", conflevel=0.95):
+def _test_t_paired(x, y, mu, alternative="two.sided", conflevel=0.95)->tuple[float, test_tpaired_result]:
 	assert conflevel>=0.0 or conflevel <= 1.0, "conflevel must be in range (0, 1)"
-	assert isinstance(x, list) or type(x)==_np.ndarray, "x must be list/ndarray"
+	assert isinstance(x, Iterable), "x must be Iterable"
 
 	XX = x
 	if isinstance(x, list):
 		XX = _np.asfarray(x)
 	
 	YY = y
 	if isinstance(y, list):
@@ -550,17 +559,31 @@
 		N = Res1.N,
 		stdev=Res1.stdev)
 	
 	return pvalue, Result
 
 
 
-def test_t (x, y = None, varequal=True, alternative="two.sided", mu=0, conflevel=0.95, paired=False ):
+def test_t (
+		x:Iterable, 
+		y:Iterable|None = None, 
+		varequal=True, 
+		alternative="two.sided", 
+		mu:numbers.Real=0.0, 
+		conflevel:numbers.Real=0.95, 
+		paired=False ):
 	"""
 	Performs paired, 1-sample and 2-sample t-test
+
+	x, y: First and second samples
+	varequal: assuming equal variances
+	alternative: 'two.sided', 'less' or 'greater'
+	mu: Assumed difference between samples or assumed mean
+	conflevel: Confidence level, [0,1]
+	paired: For paired t-test
 	"""
 	if y == None:
 		return _test_t1(x=x, mu=mu, alternative=alternative, conflevel=conflevel )	
 	else:
 		if paired==False:
 			return _test_t2(x=x, y=y, mu=mu, varequal=varequal, alternative=alternative, conflevel=conflevel)
 		else:
@@ -581,45 +604,50 @@
 	SE:float ; stdev:float 
 	mean: float 
 	zcritical:float 
 	CI_upper: float ; CI_lower: float
 	N:int
 
 
-def test_z(x, sd, mu, alternative="two.sided", conflevel=0.95):
+def test_z(
+		x:Iterable, 
+		sd:numbers.Real, 
+		mu:numbers.Real, 
+		alternative="two.sided", 
+		conflevel=0.95)->tuple[float, test_z_Result]:
 	"""
 	
 	## Return
-	p-value and test_z_Result class. \n
+	p-value and test_z_Result class.
 
 	## Input
-	x: sample,  ndarray/list \n
-	sd: Standard deviation of population \n
-	mu: Assumed mean of population \n
-	alternative: "two.sided", "less", "greater" \n
+	x: sample,  ndarray/list 
+	sd: Standard deviation of population
+	mu: Assumed mean of population
+	alternative: "two.sided", "less", "greater"
 	conflevel: Confidence level, (0,1)
 	"""
-	assert conflevel>=0.0 or conflevel <= 1.0, "conflevel must be in range (0, 1)"
+	assert conflevel>0.0 or conflevel<1.0, "conflevel must be in range (0, 1)"
 	assert sd >= 0, "sd must be >0"
-	assert isinstance(x, list) or type(x)==_np.ndarray, "x must be list/ndarray"
+	assert isinstance(x, Iterable), "x must be Iterable"
 
 	XX = x
 	if isinstance(x, list):
 		XX = _np.asfarray(x)
 
 	assert len(XX)>= 3, "container must have at least 3 elements"
 	assert _np.issubdtype(XX.dtype, _np.number), "x must contain only numbers"
 
 	dim = len(XX)
 	xaver = _np.mean(XX)
 	SE = sd / math.sqrt(dim)
 	stdeviation = _np.std(XX, ddof =1); #sample's standard deviation
 
 	alpha = 1 - conflevel
-	zcritical = (xaver - mu) / SE
+	zcritical = float((xaver - mu) / SE)
 
 	pvalue = 0.0
 
 	if alternative == "two.sided" or alternative == "notequal":
 		if zcritical <= 0:
 			#area on the left of zcrit + area on the right of positive
 			pvalue = pnorm(zcritical, 0.0, 1.0) + (1.0 - pnorm(abs(zcritical), 0.0, 1.0))
```

### Comparing `scisuit-1.2.3/scisuit/util.py` & `scisuit-1.2.4/scisuit/util.py`

 * *Files identical despite different names*

### Comparing `scisuit-1.2.3/scisuit/wxmsw32u_gl_vc_custom.dll` & `scisuit-1.2.4/scisuit/wxmsw32u_gl_vc_custom.dll`

 * *Files identical despite different names*

### Comparing `scisuit-1.2.3/scisuit/wxmsw32u_vc_custom.dll` & `scisuit-1.2.4/scisuit/wxmsw32u_vc_custom.dll`

 * *Files identical despite different names*

### Comparing `scisuit-1.2.3/scisuit.egg-info/PKG-INFO` & `scisuit-1.2.4/scisuit.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: scisuit
-Version: 1.2.3
+Version: 1.2.4
 Summary: Scientific Computing Package
 Author-email: "Gokhan Bingol, PhD" <gbingol@pebytes.com>
 Project-URL: Homepage, https://www.pebytes.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: C++
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: numpy
 
 ## scisuit
 
 A computing and plotting library designed with engineers
 in mind..
```

### Comparing `scisuit-1.2.3/scisuit.egg-info/SOURCES.txt` & `scisuit-1.2.4/scisuit.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 MANIFEST.in
 README.md
 chart_multiple.png
 chart_scatter_trendline.png
 pyproject.toml
 scisuit/__init__.py
 scisuit/_ctypeslib.py
```

