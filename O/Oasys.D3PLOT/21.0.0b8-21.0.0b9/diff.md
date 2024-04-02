# Comparing `tmp/Oasys.D3PLOT-21.0.0b8.tar.gz` & `tmp/Oasys.D3PLOT-21.0.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Oasys.D3PLOT-21.0.0b8.tar", last modified: Thu Feb 22 15:57:59 2024, max compression
+gzip compressed data, was "Oasys.D3PLOT-21.0.0b9.tar", last modified: Tue Feb 27 16:51:44 2024, max compression
```

## Comparing `Oasys.D3PLOT-21.0.0b8.tar` & `Oasys.D3PLOT-21.0.0b9.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2024-02-22 15:57:59.430462 Oasys.D3PLOT-21.0.0b8/
--rw-rw-rw-   0        0        0     1086 2024-01-20 12:37:59.000000 Oasys.D3PLOT-21.0.0b8/LICENSE
--rw-rw-rw-   0        0        0     5682 2024-02-22 15:57:59.426473 Oasys.D3PLOT-21.0.0b8/PKG-INFO
--rw-rw-rw-   0        0        0     3792 2024-01-09 11:46:29.000000 Oasys.D3PLOT-21.0.0b8/README.rst
--rw-rw-rw-   0        0        0      778 2024-02-22 15:57:29.000000 Oasys.D3PLOT-21.0.0b8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-22 15:57:59.430462 Oasys.D3PLOT-21.0.0b8/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-02-22 15:57:59.266027 Oasys.D3PLOT-21.0.0b8/src/
-drwxrwxrwx   0        0        0        0 2024-02-22 15:57:59.266027 Oasys.D3PLOT-21.0.0b8/src/Oasys/
-drwxrwxrwx   0        0        0        0 2024-02-22 15:57:59.419491 Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/
--rw-rw-rw-   0        0        0     1778 2024-01-17 15:45:08.000000 Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/__init__.py
--rw-rw-rw-   0        0        0    15476 2024-02-20 17:17:10.000000 Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/beam.py
--rw-rw-rw-   0        0        0     1928 2024-01-17 15:45:07.000000 Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/colour.py
--rw-rw-rw-   0        0        0     8919 2024-01-31 14:55:03.000000 Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/component.py
--rw-rw-rw-   0        0        0     1331 2024-01-31 14:55:03.000000 Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/constant.py
--rw-rw-rw-   0        0        0    15145 2024-02-20 17:17:10.000000 Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/contact.py
--rw-rw-rw-   0        0        0     4280 2024-01-17 15:45:08.000000 Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/core.py
--rw-rw-rw-   0        0        0    10248 2024-01-17 15:45:08.000000 Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/funcs.py
--rw-rw-rw-   0        0        0     6659 2024-01-17 15:45:08.000000 Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/graphicswindow.py
--rw-rw-rw-   0        0        0     5034 2024-01-17 15:45:08.000000 Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/group.py
--rw-rw-rw-   0        0        0     2394 2024-01-20 12:37:59.000000 Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/image.py
--rw-rw-rw-   0        0        0     3733 2024-01-17 15:45:08.000000 Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/include.py
--rw-rw-rw-   0        0        0      623 2024-01-09 11:46:30.000000 Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/itemobject.py
--rw-rw-rw-   0        0        0     7361 2024-02-20 17:17:10.000000 Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/material.py
--rw-rw-rw-   0        0        0     4094 2024-02-20 17:17:10.000000 Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/measure.py
--rw-rw-rw-   0        0        0     6924 2024-02-20 17:17:10.000000 Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/model.py
--rw-rw-rw-   0        0        0    15396 2024-02-20 17:17:10.000000 Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/node.py
--rw-rw-rw-   0        0        0      786 2024-01-17 15:45:08.000000 Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/options.py
--rw-rw-rw-   0        0        0     3362 2024-01-17 15:45:08.000000 Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/page.py
--rw-rw-rw-   0        0        0    13727 2024-02-20 17:17:10.000000 Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/part.py
--rw-rw-rw-   0        0        0    14386 2024-02-20 17:17:10.000000 Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/segment.py
--rw-rw-rw-   0        0        0     8101 2024-02-20 17:17:10.000000 Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/setbeam.py
--rw-rw-rw-   0        0        0     8101 2024-02-20 17:17:10.000000 Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/setnode.py
--rw-rw-rw-   0        0        0     8101 2024-02-20 17:17:10.000000 Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/setpart.py
--rw-rw-rw-   0        0        0     8166 2024-02-20 17:17:10.000000 Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/setshell.py
--rw-rw-rw-   0        0        0     8166 2024-02-20 17:17:10.000000 Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/setsolid.py
--rw-rw-rw-   0        0        0     8426 2024-02-20 17:17:10.000000 Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/settshell.py
--rw-rw-rw-   0        0        0    17259 2024-02-20 17:17:10.000000 Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/shell.py
--rw-rw-rw-   0        0        0    17211 2024-02-20 17:17:10.000000 Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/solid.py
--rw-rw-rw-   0        0        0    17389 2024-02-20 17:17:10.000000 Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/tshell.py
--rw-rw-rw-   0        0        0     1144 2024-01-31 14:55:03.000000 Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/type.py
--rw-rw-rw-   0        0        0     5384 2024-01-17 15:45:08.000000 Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/utils.py
--rw-rw-rw-   0        0        0     3164 2024-01-17 15:45:08.000000 Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/view.py
--rw-rw-rw-   0        0        0    11675 2024-01-17 15:45:08.000000 Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/window.py
--rw-rw-rw-   0        0        0    10619 2024-01-31 14:55:03.000000 Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/workflow.py
-drwxrwxrwx   0        0        0        0 2024-02-22 15:57:59.423481 Oasys.D3PLOT-21.0.0b8/src/Oasys.D3PLOT.egg-info/
--rw-rw-rw-   0        0        0     5682 2024-02-22 15:57:59.000000 Oasys.D3PLOT-21.0.0b8/src/Oasys.D3PLOT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1194 2024-02-22 15:57:59.000000 Oasys.D3PLOT-21.0.0b8/src/Oasys.D3PLOT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-22 15:57:59.000000 Oasys.D3PLOT-21.0.0b8/src/Oasys.D3PLOT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2024-02-22 15:57:59.000000 Oasys.D3PLOT-21.0.0b8/src/Oasys.D3PLOT.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-02-22 15:57:59.000000 Oasys.D3PLOT-21.0.0b8/src/Oasys.D3PLOT.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-02-27 16:51:44.456212 Oasys.D3PLOT-21.0.0b9/
+-rw-rw-rw-   0        0        0     1086 2024-01-20 12:37:59.000000 Oasys.D3PLOT-21.0.0b9/LICENSE
+-rw-rw-rw-   0        0        0     5682 2024-02-27 16:51:44.453218 Oasys.D3PLOT-21.0.0b9/PKG-INFO
+-rw-rw-rw-   0        0        0     3792 2024-01-09 11:46:29.000000 Oasys.D3PLOT-21.0.0b9/README.rst
+-rw-rw-rw-   0        0        0      778 2024-02-27 16:51:18.000000 Oasys.D3PLOT-21.0.0b9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-02-27 16:51:44.457207 Oasys.D3PLOT-21.0.0b9/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-02-27 16:51:44.314123 Oasys.D3PLOT-21.0.0b9/src/
+drwxrwxrwx   0        0        0        0 2024-02-27 16:51:44.314123 Oasys.D3PLOT-21.0.0b9/src/Oasys/
+drwxrwxrwx   0        0        0        0 2024-02-27 16:51:44.446236 Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/
+-rw-rw-rw-   0        0        0     1778 2024-02-27 16:37:35.000000 Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/__init__.py
+-rw-rw-rw-   0        0        0    15476 2024-02-27 16:37:34.000000 Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/beam.py
+-rw-rw-rw-   0        0        0     1928 2024-02-27 16:37:34.000000 Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/colour.py
+-rw-rw-rw-   0        0        0     8923 2024-02-27 16:37:34.000000 Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/component.py
+-rw-rw-rw-   0        0        0     1331 2024-02-27 16:37:34.000000 Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/constant.py
+-rw-rw-rw-   0        0        0    15145 2024-02-27 16:37:34.000000 Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/contact.py
+-rw-rw-rw-   0        0        0     4280 2024-02-27 16:37:35.000000 Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/core.py
+-rw-rw-rw-   0        0        0    10248 2024-02-27 16:37:35.000000 Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/funcs.py
+-rw-rw-rw-   0        0        0     6659 2024-02-27 16:37:34.000000 Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/graphicswindow.py
+-rw-rw-rw-   0        0        0     5034 2024-02-27 16:37:34.000000 Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/group.py
+-rw-rw-rw-   0        0        0     2394 2024-02-27 16:37:34.000000 Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/image.py
+-rw-rw-rw-   0        0        0     3733 2024-02-27 16:37:35.000000 Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/include.py
+-rw-rw-rw-   0        0        0      623 2024-01-09 11:46:30.000000 Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/itemobject.py
+-rw-rw-rw-   0        0        0     7361 2024-02-27 16:37:35.000000 Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/material.py
+-rw-rw-rw-   0        0        0     4094 2024-02-27 16:37:35.000000 Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/measure.py
+-rw-rw-rw-   0        0        0     6924 2024-02-27 16:37:35.000000 Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/model.py
+-rw-rw-rw-   0        0        0    15396 2024-02-27 16:37:35.000000 Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/node.py
+-rw-rw-rw-   0        0        0      786 2024-02-27 16:37:35.000000 Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/options.py
+-rw-rw-rw-   0        0        0     3362 2024-02-27 16:37:35.000000 Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/page.py
+-rw-rw-rw-   0        0        0    13727 2024-02-27 16:37:35.000000 Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/part.py
+-rw-rw-rw-   0        0        0    14386 2024-02-27 16:37:35.000000 Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/segment.py
+-rw-rw-rw-   0        0        0     8101 2024-02-27 16:37:35.000000 Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/setbeam.py
+-rw-rw-rw-   0        0        0     8101 2024-02-27 16:37:35.000000 Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/setnode.py
+-rw-rw-rw-   0        0        0     8101 2024-02-27 16:37:35.000000 Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/setpart.py
+-rw-rw-rw-   0        0        0     8166 2024-02-27 16:37:35.000000 Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/setshell.py
+-rw-rw-rw-   0        0        0     8166 2024-02-27 16:37:35.000000 Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/setsolid.py
+-rw-rw-rw-   0        0        0     8426 2024-02-27 16:37:35.000000 Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/settshell.py
+-rw-rw-rw-   0        0        0    17259 2024-02-27 16:37:35.000000 Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/shell.py
+-rw-rw-rw-   0        0        0    17211 2024-02-27 16:37:35.000000 Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/solid.py
+-rw-rw-rw-   0        0        0    17389 2024-02-27 16:37:35.000000 Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/tshell.py
+-rw-rw-rw-   0        0        0     1144 2024-02-27 16:37:35.000000 Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/type.py
+-rw-rw-rw-   0        0        0     5616 2024-02-27 16:37:35.000000 Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/utils.py
+-rw-rw-rw-   0        0        0     3164 2024-02-27 16:37:35.000000 Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/view.py
+-rw-rw-rw-   0        0        0    11675 2024-02-27 16:37:35.000000 Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/window.py
+-rw-rw-rw-   0        0        0    10619 2024-02-27 16:37:35.000000 Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/workflow.py
+drwxrwxrwx   0        0        0        0 2024-02-27 16:51:44.450225 Oasys.D3PLOT-21.0.0b9/src/Oasys.D3PLOT.egg-info/
+-rw-rw-rw-   0        0        0     5682 2024-02-27 16:51:44.000000 Oasys.D3PLOT-21.0.0b9/src/Oasys.D3PLOT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1194 2024-02-27 16:51:44.000000 Oasys.D3PLOT-21.0.0b9/src/Oasys.D3PLOT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-02-27 16:51:44.000000 Oasys.D3PLOT-21.0.0b9/src/Oasys.D3PLOT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2024-02-27 16:51:44.000000 Oasys.D3PLOT-21.0.0b9/src/Oasys.D3PLOT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-02-27 16:51:44.000000 Oasys.D3PLOT-21.0.0b9/src/Oasys.D3PLOT.egg-info/top_level.txt
```

### Comparing `Oasys.D3PLOT-21.0.0b8/LICENSE` & `Oasys.D3PLOT-21.0.0b9/LICENSE`

 * *Files identical despite different names*

### Comparing `Oasys.D3PLOT-21.0.0b8/PKG-INFO` & `Oasys.D3PLOT-21.0.0b9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Oasys.D3PLOT
-Version: 21.0.0b8
+Version: 21.0.0b9
 Summary: Python API for Oasys D3PLOT
 Author: Miles Thornton
 Maintainer-email: DYNA support <dyna.support@arup.com>
 License: MIT License
         
         Copyright (c) 2024 Oasys Ltd
         
@@ -30,15 +30,15 @@
 Project-URL: Homepage, https://www.oasys-software.com/dyna/software/d3plot/
 Project-URL: Linkedin, https://www.linkedin.com/company/oasys-ltd-software/
 Project-URL: YouTube, https://www.youtube.com/c/OasysLtd
 Keywords: Oasys,D3PLOT
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: Oasys.gRPC>=21.0.0b5
+Requires-Dist: Oasys.gRPC>=21.0.0b6
 
 The Oasys.D3PLOT package allows Python scripts to control the Oasys LS-DYNA Environment
 software `D3PLOT <https://www.oasys-software.com/dyna/software/d3plot/>`_.
 
 Basic Information
 -----------------
```

### Comparing `Oasys.D3PLOT-21.0.0b8/README.rst` & `Oasys.D3PLOT-21.0.0b9/README.rst`

 * *Files identical despite different names*

### Comparing `Oasys.D3PLOT-21.0.0b8/pyproject.toml` & `Oasys.D3PLOT-21.0.0b9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "Oasys.D3PLOT"
-version = "21.0.0b8"
+version = "21.0.0b9"
 license = {file = "LICENSE"}
 requires-python = ">=3.7"
 keywords = ["Oasys", "D3PLOT"]
 dependencies = [
-  "Oasys.gRPC >= 21.0.0b5"
+  "Oasys.gRPC >= 21.0.0b6"
 ]
 description = "Python API for Oasys D3PLOT"
 readme = "README.rst"
 authors = [
   {name = "Miles Thornton"},
 ]
 maintainers = [
```

### Comparing `Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/__init__.py` & `Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/__init__.py`

 * *Files identical despite different names*

### Comparing `Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/beam.py` & `Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/beam.py`

 * *Files identical despite different names*

### Comparing `Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/colour.py` & `Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/colour.py`

 * *Files identical despite different names*

### Comparing `Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/component.py` & `Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/component.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         if name in ComponentType._consts:
             return Oasys.D3PLOT._connection.classGetter(cls.__name__, name)
 
         raise AttributeError
 
 
 class Component(Oasys.gRPC.OasysItem, metaclass=ComponentType):
-    _props = {'component', 'dataType', 'dispose', 'location', 'name'}
+    _props = {'componentType', 'dataType', 'dispose', 'location', 'name'}
 
 
     def __del__(self):
         if not Oasys.D3PLOT._connection:
             return
 
         Oasys.D3PLOT._connection.destructor(self.__class__.__name__, self._handle)
```

### Comparing `Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/constant.py` & `Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/constant.py`

 * *Files identical despite different names*

### Comparing `Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/contact.py` & `Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/contact.py`

 * *Files identical despite different names*

### Comparing `Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/core.py` & `Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/core.py`

 * *Files identical despite different names*

### Comparing `Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/funcs.py` & `Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/funcs.py`

 * *Files identical despite different names*

### Comparing `Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/graphicswindow.py` & `Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/graphicswindow.py`

 * *Files identical despite different names*

### Comparing `Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/group.py` & `Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/group.py`

 * *Files identical despite different names*

### Comparing `Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/image.py` & `Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/image.py`

 * *Files identical despite different names*

### Comparing `Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/include.py` & `Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/include.py`

 * *Files identical despite different names*

### Comparing `Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/itemobject.py` & `Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/itemobject.py`

 * *Files identical despite different names*

### Comparing `Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/material.py` & `Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/material.py`

 * *Files identical despite different names*

### Comparing `Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/measure.py` & `Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/measure.py`

 * *Files identical despite different names*

### Comparing `Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/model.py` & `Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/model.py`

 * *Files identical despite different names*

### Comparing `Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/node.py` & `Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/node.py`

 * *Files identical despite different names*

### Comparing `Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/options.py` & `Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/options.py`

 * *Files identical despite different names*

### Comparing `Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/page.py` & `Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/page.py`

 * *Files identical despite different names*

### Comparing `Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/part.py` & `Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/part.py`

 * *Files identical despite different names*

### Comparing `Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/segment.py` & `Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/segment.py`

 * *Files identical despite different names*

### Comparing `Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/setbeam.py` & `Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/setbeam.py`

 * *Files identical despite different names*

### Comparing `Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/setnode.py` & `Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/setnode.py`

 * *Files identical despite different names*

### Comparing `Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/setpart.py` & `Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/setpart.py`

 * *Files identical despite different names*

### Comparing `Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/setshell.py` & `Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/setshell.py`

 * *Files identical despite different names*

### Comparing `Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/setsolid.py` & `Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/setsolid.py`

 * *Files identical despite different names*

### Comparing `Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/settshell.py` & `Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/settshell.py`

 * *Files identical despite different names*

### Comparing `Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/shell.py` & `Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/shell.py`

 * *Files identical despite different names*

### Comparing `Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/solid.py` & `Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/solid.py`

 * *Files identical despite different names*

### Comparing `Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/tshell.py` & `Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/tshell.py`

 * *Files identical despite different names*

### Comparing `Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/type.py` & `Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/type.py`

 * *Files identical despite different names*

### Comparing `Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/utils.py` & `Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,25 @@
         Returns
         -------
         str
             string
         """
         return Oasys.D3PLOT._connection.classMethod(__class__.__name__, "Ascii85Encode", data, length)
 
+    def Build():
+        """
+        Returns the build number
+
+        Returns
+        -------
+        int
+            integer
+        """
+        return Oasys.D3PLOT._connection.classMethod(__class__.__name__, "Build")
+
     def CallPromiseHandlers():
         """
         Manually call any promise handlers/callbacks in the job queue
 
         Returns
         -------
         None
```

### Comparing `Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/view.py` & `Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/view.py`

 * *Files identical despite different names*

### Comparing `Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/window.py` & `Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/window.py`

 * *Files identical despite different names*

### Comparing `Oasys.D3PLOT-21.0.0b8/src/Oasys/D3PLOT/workflow.py` & `Oasys.D3PLOT-21.0.0b9/src/Oasys/D3PLOT/workflow.py`

 * *Files identical despite different names*

### Comparing `Oasys.D3PLOT-21.0.0b8/src/Oasys.D3PLOT.egg-info/PKG-INFO` & `Oasys.D3PLOT-21.0.0b9/src/Oasys.D3PLOT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Oasys.D3PLOT
-Version: 21.0.0b8
+Version: 21.0.0b9
 Summary: Python API for Oasys D3PLOT
 Author: Miles Thornton
 Maintainer-email: DYNA support <dyna.support@arup.com>
 License: MIT License
         
         Copyright (c) 2024 Oasys Ltd
         
@@ -30,15 +30,15 @@
 Project-URL: Homepage, https://www.oasys-software.com/dyna/software/d3plot/
 Project-URL: Linkedin, https://www.linkedin.com/company/oasys-ltd-software/
 Project-URL: YouTube, https://www.youtube.com/c/OasysLtd
 Keywords: Oasys,D3PLOT
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: Oasys.gRPC>=21.0.0b5
+Requires-Dist: Oasys.gRPC>=21.0.0b6
 
 The Oasys.D3PLOT package allows Python scripts to control the Oasys LS-DYNA Environment
 software `D3PLOT <https://www.oasys-software.com/dyna/software/d3plot/>`_.
 
 Basic Information
 -----------------
```

### Comparing `Oasys.D3PLOT-21.0.0b8/src/Oasys.D3PLOT.egg-info/SOURCES.txt` & `Oasys.D3PLOT-21.0.0b9/src/Oasys.D3PLOT.egg-info/SOURCES.txt`

 * *Files identical despite different names*

