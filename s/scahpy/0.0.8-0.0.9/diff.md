# Comparing `tmp/scahpy-0.0.8.tar.gz` & `tmp/scahpy-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scahpy-0.0.8.tar", last modified: Fri Feb 23 17:04:20 2024, max compression
+gzip compressed data, was "scahpy-0.0.9.tar", last modified: Mon Feb 26 20:38:47 2024, max compression
```

## Comparing `scahpy-0.0.8.tar` & `scahpy-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxrwxrwx   0 usuario   (1000) usuario   (1000)        0 2024-02-23 17:04:20.471735 scahpy-0.0.8/
--rwxrwxrwx   0 usuario   (1000) usuario   (1000)    35128 2024-02-23 15:21:08.000000 scahpy-0.0.8/LICENSE
--rwxrwxrwx   0 usuario   (1000) usuario   (1000)      174 2024-02-23 16:55:13.000000 scahpy-0.0.8/MANIFEST.in
--rwxrwxrwx   0 usuario   (1000) usuario   (1000)    43728 2024-02-23 17:04:20.471277 scahpy-0.0.8/PKG-INFO
--rwxrwxrwx   0 usuario   (1000) usuario   (1000)     2477 2024-02-23 15:21:08.000000 scahpy-0.0.8/README.md
--rwxrwxrwx   0 usuario   (1000) usuario   (1000)      859 2024-02-23 17:00:48.000000 scahpy-0.0.8/pyproject.toml
-drwxrwxrwx   0 usuario   (1000) usuario   (1000)        0 2024-02-23 17:04:20.467441 scahpy-0.0.8/scahpy/
--rwxrwxrwx   0 usuario   (1000) usuario   (1000)      168 2024-02-23 17:00:37.000000 scahpy-0.0.8/scahpy/__init__.py
--rwxrwxrwx   0 usuario   (1000) usuario   (1000)     1152 2024-02-23 15:21:08.000000 scahpy-0.0.8/scahpy/colors_scales.py
--rwxrwxrwx   0 usuario   (1000) usuario   (1000)     8402 2024-02-23 15:21:08.000000 scahpy-0.0.8/scahpy/in_out.py
--rwxrwxrwx   0 usuario   (1000) usuario   (1000)     3594 2024-02-23 15:21:08.000000 scahpy-0.0.8/scahpy/map_plots.py
--rwxrwxrwx   0 usuario   (1000) usuario   (1000)     2905 2024-02-23 15:21:08.000000 scahpy-0.0.8/scahpy/met_diag.py
--rwxrwxrwx   0 usuario   (1000) usuario   (1000)     1502 2024-02-23 15:21:08.000000 scahpy-0.0.8/scahpy/spatial_scales.py
--rwxrwxrwx   0 usuario   (1000) usuario   (1000)     3398 2024-02-23 15:21:08.000000 scahpy-0.0.8/scahpy/temp_scales.py
-drwxrwxrwx   0 usuario   (1000) usuario   (1000)        0 2024-02-23 17:04:20.470527 scahpy-0.0.8/scahpy.egg-info/
--rwxrwxrwx   0 usuario   (1000) usuario   (1000)    43728 2024-02-23 17:04:20.000000 scahpy-0.0.8/scahpy.egg-info/PKG-INFO
--rwxrwxrwx   0 usuario   (1000) usuario   (1000)      339 2024-02-23 17:04:20.000000 scahpy-0.0.8/scahpy.egg-info/SOURCES.txt
--rwxrwxrwx   0 usuario   (1000) usuario   (1000)        1 2024-02-23 17:04:20.000000 scahpy-0.0.8/scahpy.egg-info/dependency_links.txt
--rwxrwxrwx   0 usuario   (1000) usuario   (1000)       76 2024-02-23 17:04:20.000000 scahpy-0.0.8/scahpy.egg-info/requires.txt
--rwxrwxrwx   0 usuario   (1000) usuario   (1000)        7 2024-02-23 17:04:20.000000 scahpy-0.0.8/scahpy.egg-info/top_level.txt
--rwxrwxrwx   0 usuario   (1000) usuario   (1000)       38 2024-02-23 17:04:20.471814 scahpy-0.0.8/setup.cfg
+drwxrwxrwx   0 usuario   (1000) usuario   (1000)        0 2024-02-26 20:38:47.432346 scahpy-0.0.9/
+-rwxrwxrwx   0 usuario   (1000) usuario   (1000)    35128 2024-02-23 15:21:08.000000 scahpy-0.0.9/LICENSE
+-rwxrwxrwx   0 usuario   (1000) usuario   (1000)      174 2024-02-23 16:55:13.000000 scahpy-0.0.9/MANIFEST.in
+-rwxrwxrwx   0 usuario   (1000) usuario   (1000)    43728 2024-02-26 20:38:47.431844 scahpy-0.0.9/PKG-INFO
+-rwxrwxrwx   0 usuario   (1000) usuario   (1000)     2477 2024-02-23 15:21:08.000000 scahpy-0.0.9/README.md
+-rwxrwxrwx   0 usuario   (1000) usuario   (1000)      859 2024-02-26 20:34:53.000000 scahpy-0.0.9/pyproject.toml
+drwxrwxrwx   0 usuario   (1000) usuario   (1000)        0 2024-02-26 20:38:47.425890 scahpy-0.0.9/scahpy/
+-rwxrwxrwx   0 usuario   (1000) usuario   (1000)      168 2024-02-26 20:35:09.000000 scahpy-0.0.9/scahpy/__init__.py
+-rwxrwxrwx   0 usuario   (1000) usuario   (1000)     1152 2024-02-23 15:21:08.000000 scahpy-0.0.9/scahpy/colors_scales.py
+drwxrwxrwx   0 usuario   (1000) usuario   (1000)        0 2024-02-26 20:38:47.430416 scahpy-0.0.9/scahpy/data/
+-rwxrwxrwx   0 usuario   (1000) usuario   (1000)        0 2024-02-23 22:23:44.000000 scahpy-0.0.9/scahpy/data/__init__.py
+-rwxrwxrwx   0 usuario   (1000) usuario   (1000)     8402 2024-02-23 15:21:08.000000 scahpy-0.0.9/scahpy/in_out.py
+-rwxrwxrwx   0 usuario   (1000) usuario   (1000)     3594 2024-02-23 15:21:08.000000 scahpy-0.0.9/scahpy/map_plots.py
+-rwxrwxrwx   0 usuario   (1000) usuario   (1000)     2905 2024-02-23 15:21:08.000000 scahpy-0.0.9/scahpy/met_diag.py
+-rwxrwxrwx   0 usuario   (1000) usuario   (1000)     1502 2024-02-23 15:21:08.000000 scahpy-0.0.9/scahpy/spatial_scales.py
+-rwxrwxrwx   0 usuario   (1000) usuario   (1000)     3398 2024-02-23 15:21:08.000000 scahpy-0.0.9/scahpy/temp_scales.py
+drwxrwxrwx   0 usuario   (1000) usuario   (1000)        0 2024-02-26 20:38:47.431025 scahpy-0.0.9/scahpy.egg-info/
+-rwxrwxrwx   0 usuario   (1000) usuario   (1000)    43728 2024-02-26 20:38:47.000000 scahpy-0.0.9/scahpy.egg-info/PKG-INFO
+-rwxrwxrwx   0 usuario   (1000) usuario   (1000)      363 2024-02-26 20:38:47.000000 scahpy-0.0.9/scahpy.egg-info/SOURCES.txt
+-rwxrwxrwx   0 usuario   (1000) usuario   (1000)        1 2024-02-26 20:38:47.000000 scahpy-0.0.9/scahpy.egg-info/dependency_links.txt
+-rwxrwxrwx   0 usuario   (1000) usuario   (1000)       76 2024-02-26 20:38:47.000000 scahpy-0.0.9/scahpy.egg-info/requires.txt
+-rwxrwxrwx   0 usuario   (1000) usuario   (1000)        7 2024-02-26 20:38:47.000000 scahpy-0.0.9/scahpy.egg-info/top_level.txt
+-rwxrwxrwx   0 usuario   (1000) usuario   (1000)       38 2024-02-26 20:38:47.432420 scahpy-0.0.9/setup.cfg
```

### Comparing `scahpy-0.0.8/LICENSE` & `scahpy-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `scahpy-0.0.8/PKG-INFO` & `scahpy-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scahpy
-Version: 0.0.8
+Version: 0.0.9
 Summary: Package to process and analyze outputs from IGP-RESM-COW model
 Author-email: Fiorela Castillón <fv.castillon@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `scahpy-0.0.8/README.md` & `scahpy-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `scahpy-0.0.8/pyproject.toml` & `scahpy-0.0.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "scahpy"
-version = "0.0.8"
+version = "0.0.9"
 description = "Package to process and analyze outputs from IGP-RESM-COW model"
 readme = "README.md"
 authors = [{ name = "Fiorela Castillón", email = "fv.castillon@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python",
```

### Comparing `scahpy-0.0.8/scahpy/colors_scales.py` & `scahpy-0.0.9/scahpy/colors_scales.py`

 * *Files identical despite different names*

### Comparing `scahpy-0.0.8/scahpy/in_out.py` & `scahpy-0.0.9/scahpy/in_out.py`

 * *Files identical despite different names*

### Comparing `scahpy-0.0.8/scahpy/map_plots.py` & `scahpy-0.0.9/scahpy/map_plots.py`

 * *Files identical despite different names*

### Comparing `scahpy-0.0.8/scahpy/met_diag.py` & `scahpy-0.0.9/scahpy/met_diag.py`

 * *Files identical despite different names*

### Comparing `scahpy-0.0.8/scahpy/spatial_scales.py` & `scahpy-0.0.9/scahpy/spatial_scales.py`

 * *Files identical despite different names*

### Comparing `scahpy-0.0.8/scahpy/temp_scales.py` & `scahpy-0.0.9/scahpy/temp_scales.py`

 * *Files identical despite different names*

### Comparing `scahpy-0.0.8/scahpy.egg-info/PKG-INFO` & `scahpy-0.0.9/scahpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scahpy
-Version: 0.0.8
+Version: 0.0.9
 Summary: Package to process and analyze outputs from IGP-RESM-COW model
 Author-email: Fiorela Castillón <fv.castillon@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

