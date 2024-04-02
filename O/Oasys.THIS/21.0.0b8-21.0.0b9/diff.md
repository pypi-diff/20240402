# Comparing `tmp/Oasys.THIS-21.0.0b8.tar.gz` & `tmp/Oasys.THIS-21.0.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Oasys.THIS-21.0.0b8.tar", last modified: Tue Feb 27 16:53:08 2024, max compression
+gzip compressed data, was "Oasys.THIS-21.0.0b9.tar", last modified: Thu Feb 29 17:37:02 2024, max compression
```

## Comparing `Oasys.THIS-21.0.0b8.tar` & `Oasys.THIS-21.0.0b9.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2024-02-27 16:53:08.184470 Oasys.THIS-21.0.0b8/
--rw-rw-rw-   0        0        0     1086 2024-01-20 12:37:59.000000 Oasys.THIS-21.0.0b8/LICENSE
--rw-rw-rw-   0        0        0     6608 2024-02-27 16:53:08.182476 Oasys.THIS-21.0.0b8/PKG-INFO
--rw-rw-rw-   0        0        0     4719 2024-01-09 11:46:34.000000 Oasys.THIS-21.0.0b8/README.rst
--rw-rw-rw-   0        0        0      780 2024-02-27 16:52:41.000000 Oasys.THIS-21.0.0b8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-27 16:53:08.185470 Oasys.THIS-21.0.0b8/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-02-27 16:53:08.074541 Oasys.THIS-21.0.0b8/src/
-drwxrwxrwx   0        0        0        0 2024-02-27 16:53:08.075566 Oasys.THIS-21.0.0b8/src/Oasys/
-drwxrwxrwx   0        0        0        0 2024-02-27 16:53:08.174498 Oasys.THIS-21.0.0b8/src/Oasys/THIS/
--rw-rw-rw-   0        0        0     1251 2024-02-27 16:37:40.000000 Oasys.THIS-21.0.0b8/src/Oasys/THIS/__init__.py
--rw-rw-rw-   0        0        0     2171 2024-02-27 16:37:40.000000 Oasys.THIS-21.0.0b8/src/Oasys/THIS/colour.py
--rw-rw-rw-   0        0        0     5223 2024-02-27 16:37:40.000000 Oasys.THIS-21.0.0b8/src/Oasys/THIS/component.py
--rw-rw-rw-   0        0        0     3397 2024-02-27 16:37:40.000000 Oasys.THIS-21.0.0b8/src/Oasys/THIS/core.py
--rw-rw-rw-   0        0        0    17485 2024-02-27 16:37:40.000000 Oasys.THIS-21.0.0b8/src/Oasys/THIS/curve.py
--rw-rw-rw-   0        0        0     6733 2024-02-27 16:37:40.000000 Oasys.THIS-21.0.0b8/src/Oasys/THIS/datum.py
--rw-rw-rw-   0        0        0     2264 2024-02-27 16:37:40.000000 Oasys.THIS-21.0.0b8/src/Oasys/THIS/entity.py
--rw-rw-rw-   0        0        0    13490 2024-02-27 16:37:40.000000 Oasys.THIS-21.0.0b8/src/Oasys/THIS/funcs.py
--rw-rw-rw-   0        0        0     8871 2024-02-27 16:37:40.000000 Oasys.THIS-21.0.0b8/src/Oasys/THIS/graph.py
--rw-rw-rw-   0        0        0     8228 2024-02-27 16:37:40.000000 Oasys.THIS-21.0.0b8/src/Oasys/THIS/group.py
--rw-rw-rw-   0        0        0      741 2024-02-27 16:37:40.000000 Oasys.THIS-21.0.0b8/src/Oasys/THIS/include.py
--rw-rw-rw-   0        0        0      614 2023-08-29 08:26:20.000000 Oasys.THIS-21.0.0b8/src/Oasys/THIS/itemobject.py
--rw-rw-rw-   0        0        0      790 2024-02-27 16:37:40.000000 Oasys.THIS-21.0.0b8/src/Oasys/THIS/linestyle.py
--rw-rw-rw-   0        0        0      816 2024-02-27 16:37:40.000000 Oasys.THIS-21.0.0b8/src/Oasys/THIS/linewidth.py
--rw-rw-rw-   0        0        0    16280 2024-02-27 16:37:40.000000 Oasys.THIS-21.0.0b8/src/Oasys/THIS/model.py
--rw-rw-rw-   0        0        0    61932 2024-02-27 16:37:40.000000 Oasys.THIS-21.0.0b8/src/Oasys/THIS/operate.py
--rw-rw-rw-   0        0        0      780 2024-02-27 16:37:40.000000 Oasys.THIS-21.0.0b8/src/Oasys/THIS/options.py
--rw-rw-rw-   0        0        0     5622 2024-02-27 16:37:40.000000 Oasys.THIS-21.0.0b8/src/Oasys/THIS/page.py
--rw-rw-rw-   0        0        0     5439 2024-02-27 16:37:40.000000 Oasys.THIS-21.0.0b8/src/Oasys/THIS/read.py
--rw-rw-rw-   0        0        0      796 2024-02-27 16:37:40.000000 Oasys.THIS-21.0.0b8/src/Oasys/THIS/symbol.py
--rw-rw-rw-   0        0        0     2045 2024-02-27 16:37:40.000000 Oasys.THIS-21.0.0b8/src/Oasys/THIS/units.py
--rw-rw-rw-   0        0        0      760 2024-02-27 16:37:40.000000 Oasys.THIS-21.0.0b8/src/Oasys/THIS/unitsystem.py
--rw-rw-rw-   0        0        0     5586 2024-02-27 16:37:40.000000 Oasys.THIS-21.0.0b8/src/Oasys/THIS/utils.py
--rw-rw-rw-   0        0        0    11643 2024-02-27 16:37:40.000000 Oasys.THIS-21.0.0b8/src/Oasys/THIS/window.py
--rw-rw-rw-   0        0        0    10593 2024-02-27 16:37:40.000000 Oasys.THIS-21.0.0b8/src/Oasys/THIS/workflow.py
-drwxrwxrwx   0        0        0        0 2024-02-27 16:53:08.179484 Oasys.THIS-21.0.0b8/src/Oasys.THIS.egg-info/
--rw-rw-rw-   0        0        0     6608 2024-02-27 16:53:08.000000 Oasys.THIS-21.0.0b8/src/Oasys.THIS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      857 2024-02-27 16:53:08.000000 Oasys.THIS-21.0.0b8/src/Oasys.THIS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-27 16:53:08.000000 Oasys.THIS-21.0.0b8/src/Oasys.THIS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2024-02-27 16:53:08.000000 Oasys.THIS-21.0.0b8/src/Oasys.THIS.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-02-27 16:53:08.000000 Oasys.THIS-21.0.0b8/src/Oasys.THIS.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-02-29 17:37:02.923227 Oasys.THIS-21.0.0b9/
+-rw-rw-rw-   0        0        0     1086 2024-01-18 09:18:00.000000 Oasys.THIS-21.0.0b9/LICENSE
+-rw-rw-rw-   0        0        0     6608 2024-02-29 17:37:02.922271 Oasys.THIS-21.0.0b9/PKG-INFO
+-rw-rw-rw-   0        0        0     4719 2024-01-04 08:22:01.000000 Oasys.THIS-21.0.0b9/README.rst
+-rw-rw-rw-   0        0        0      780 2024-02-29 17:33:26.000000 Oasys.THIS-21.0.0b9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-02-29 17:37:02.923227 Oasys.THIS-21.0.0b9/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-02-29 17:37:02.632522 Oasys.THIS-21.0.0b9/src/
+drwxrwxrwx   0        0        0        0 2024-02-29 17:37:02.632522 Oasys.THIS-21.0.0b9/src/Oasys/
+drwxrwxrwx   0        0        0        0 2024-02-29 17:37:02.919228 Oasys.THIS-21.0.0b9/src/Oasys/THIS/
+-rw-rw-rw-   0        0        0     1251 2024-02-29 17:28:11.000000 Oasys.THIS-21.0.0b9/src/Oasys/THIS/__init__.py
+-rw-rw-rw-   0        0        0     2171 2024-02-29 17:28:11.000000 Oasys.THIS-21.0.0b9/src/Oasys/THIS/colour.py
+-rw-rw-rw-   0        0        0     5223 2024-02-29 17:28:11.000000 Oasys.THIS-21.0.0b9/src/Oasys/THIS/component.py
+-rw-rw-rw-   0        0        0     3397 2024-02-29 17:28:11.000000 Oasys.THIS-21.0.0b9/src/Oasys/THIS/core.py
+-rw-rw-rw-   0        0        0    17485 2024-02-29 17:28:11.000000 Oasys.THIS-21.0.0b9/src/Oasys/THIS/curve.py
+-rw-rw-rw-   0        0        0     6733 2024-02-29 17:28:11.000000 Oasys.THIS-21.0.0b9/src/Oasys/THIS/datum.py
+-rw-rw-rw-   0        0        0     2264 2024-02-29 17:28:11.000000 Oasys.THIS-21.0.0b9/src/Oasys/THIS/entity.py
+-rw-rw-rw-   0        0        0    13490 2024-02-29 17:28:11.000000 Oasys.THIS-21.0.0b9/src/Oasys/THIS/funcs.py
+-rw-rw-rw-   0        0        0     8871 2024-02-29 17:28:11.000000 Oasys.THIS-21.0.0b9/src/Oasys/THIS/graph.py
+-rw-rw-rw-   0        0        0     8228 2024-02-29 17:28:11.000000 Oasys.THIS-21.0.0b9/src/Oasys/THIS/group.py
+-rw-rw-rw-   0        0        0      741 2024-02-29 17:28:11.000000 Oasys.THIS-21.0.0b9/src/Oasys/THIS/include.py
+-rw-rw-rw-   0        0        0      614 2023-08-10 13:12:58.000000 Oasys.THIS-21.0.0b9/src/Oasys/THIS/itemobject.py
+-rw-rw-rw-   0        0        0      790 2024-02-29 17:28:11.000000 Oasys.THIS-21.0.0b9/src/Oasys/THIS/linestyle.py
+-rw-rw-rw-   0        0        0      816 2024-02-29 17:28:11.000000 Oasys.THIS-21.0.0b9/src/Oasys/THIS/linewidth.py
+-rw-rw-rw-   0        0        0    16280 2024-02-29 17:28:11.000000 Oasys.THIS-21.0.0b9/src/Oasys/THIS/model.py
+-rw-rw-rw-   0        0        0    61932 2024-02-29 17:28:11.000000 Oasys.THIS-21.0.0b9/src/Oasys/THIS/operate.py
+-rw-rw-rw-   0        0        0      780 2024-02-29 17:28:11.000000 Oasys.THIS-21.0.0b9/src/Oasys/THIS/options.py
+-rw-rw-rw-   0        0        0     5622 2024-02-29 17:28:11.000000 Oasys.THIS-21.0.0b9/src/Oasys/THIS/page.py
+-rw-rw-rw-   0        0        0     5439 2024-02-29 17:28:11.000000 Oasys.THIS-21.0.0b9/src/Oasys/THIS/read.py
+-rw-rw-rw-   0        0        0      796 2024-02-29 17:28:11.000000 Oasys.THIS-21.0.0b9/src/Oasys/THIS/symbol.py
+-rw-rw-rw-   0        0        0     2045 2024-02-29 17:28:11.000000 Oasys.THIS-21.0.0b9/src/Oasys/THIS/units.py
+-rw-rw-rw-   0        0        0      760 2024-02-29 17:28:11.000000 Oasys.THIS-21.0.0b9/src/Oasys/THIS/unitsystem.py
+-rw-rw-rw-   0        0        0     5586 2024-02-29 17:28:11.000000 Oasys.THIS-21.0.0b9/src/Oasys/THIS/utils.py
+-rw-rw-rw-   0        0        0    11643 2024-02-29 17:28:11.000000 Oasys.THIS-21.0.0b9/src/Oasys/THIS/window.py
+-rw-rw-rw-   0        0        0    10593 2024-02-29 17:28:11.000000 Oasys.THIS-21.0.0b9/src/Oasys/THIS/workflow.py
+drwxrwxrwx   0        0        0        0 2024-02-29 17:37:02.921302 Oasys.THIS-21.0.0b9/src/Oasys.THIS.egg-info/
+-rw-rw-rw-   0        0        0     6608 2024-02-29 17:37:02.000000 Oasys.THIS-21.0.0b9/src/Oasys.THIS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      857 2024-02-29 17:37:02.000000 Oasys.THIS-21.0.0b9/src/Oasys.THIS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-02-29 17:37:02.000000 Oasys.THIS-21.0.0b9/src/Oasys.THIS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2024-02-29 17:37:02.000000 Oasys.THIS-21.0.0b9/src/Oasys.THIS.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-02-29 17:37:02.000000 Oasys.THIS-21.0.0b9/src/Oasys.THIS.egg-info/top_level.txt
```

### Comparing `Oasys.THIS-21.0.0b8/LICENSE` & `Oasys.THIS-21.0.0b9/LICENSE`

 * *Files identical despite different names*

### Comparing `Oasys.THIS-21.0.0b8/PKG-INFO` & `Oasys.THIS-21.0.0b9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Oasys.THIS
-Version: 21.0.0b8
+Version: 21.0.0b9
 Summary: Python API for Oasys T/HIS
 Author: Miles Thornton
 Maintainer-email: DYNA support <dyna.support@arup.com>
 License: MIT License
         
         Copyright (c) 2024 Oasys Ltd
         
@@ -30,15 +30,15 @@
 Project-URL: Homepage, https://www.oasys-software.com/dyna/software/t-his/
 Project-URL: Linkedin, https://www.linkedin.com/company/oasys-ltd-software/
 Project-URL: YouTube, https://www.youtube.com/c/OasysLtd
 Keywords: Oasys,THIS,T/HIS
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: Oasys.gRPC>=21.0.0b6
+Requires-Dist: Oasys.gRPC>=21.0.0b7
 
 The Oasys.THIS package allows Python scripts to control the Oasys LS-DYNA Environment
 software `T/HIS <https://www.oasys-software.com/dyna/software/t-his/>`_.
 
 Basic Information
 -----------------
```

### Comparing `Oasys.THIS-21.0.0b8/README.rst` & `Oasys.THIS-21.0.0b9/README.rst`

 * *Files identical despite different names*

### Comparing `Oasys.THIS-21.0.0b8/pyproject.toml` & `Oasys.THIS-21.0.0b9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "Oasys.THIS"
-version = "21.0.0b8"
+version = "21.0.0b9"
 license = {file = "LICENSE"}
 requires-python = ">=3.7"
 keywords = ["Oasys", "THIS", "T/HIS"]
 dependencies = [
-  "Oasys.gRPC >= 21.0.0b6"
+  "Oasys.gRPC >= 21.0.0b7"
 ]
 description = "Python API for Oasys T/HIS"
 readme = "README.rst"
 authors = [
   {name = "Miles Thornton"},
 ]
 maintainers = [
```

### Comparing `Oasys.THIS-21.0.0b8/src/Oasys/THIS/__init__.py` & `Oasys.THIS-21.0.0b9/src/Oasys/THIS/__init__.py`

 * *Files identical despite different names*

### Comparing `Oasys.THIS-21.0.0b8/src/Oasys/THIS/colour.py` & `Oasys.THIS-21.0.0b9/src/Oasys/THIS/colour.py`

 * *Files identical despite different names*

### Comparing `Oasys.THIS-21.0.0b8/src/Oasys/THIS/component.py` & `Oasys.THIS-21.0.0b9/src/Oasys/THIS/component.py`

 * *Files identical despite different names*

### Comparing `Oasys.THIS-21.0.0b8/src/Oasys/THIS/core.py` & `Oasys.THIS-21.0.0b9/src/Oasys/THIS/core.py`

 * *Files identical despite different names*

### Comparing `Oasys.THIS-21.0.0b8/src/Oasys/THIS/curve.py` & `Oasys.THIS-21.0.0b9/src/Oasys/THIS/curve.py`

 * *Files identical despite different names*

### Comparing `Oasys.THIS-21.0.0b8/src/Oasys/THIS/datum.py` & `Oasys.THIS-21.0.0b9/src/Oasys/THIS/datum.py`

 * *Files identical despite different names*

### Comparing `Oasys.THIS-21.0.0b8/src/Oasys/THIS/entity.py` & `Oasys.THIS-21.0.0b9/src/Oasys/THIS/entity.py`

 * *Files identical despite different names*

### Comparing `Oasys.THIS-21.0.0b8/src/Oasys/THIS/funcs.py` & `Oasys.THIS-21.0.0b9/src/Oasys/THIS/funcs.py`

 * *Files identical despite different names*

### Comparing `Oasys.THIS-21.0.0b8/src/Oasys/THIS/graph.py` & `Oasys.THIS-21.0.0b9/src/Oasys/THIS/graph.py`

 * *Files identical despite different names*

### Comparing `Oasys.THIS-21.0.0b8/src/Oasys/THIS/group.py` & `Oasys.THIS-21.0.0b9/src/Oasys/THIS/group.py`

 * *Files identical despite different names*

### Comparing `Oasys.THIS-21.0.0b8/src/Oasys/THIS/include.py` & `Oasys.THIS-21.0.0b9/src/Oasys/THIS/include.py`

 * *Files identical despite different names*

### Comparing `Oasys.THIS-21.0.0b8/src/Oasys/THIS/itemobject.py` & `Oasys.THIS-21.0.0b9/src/Oasys/THIS/itemobject.py`

 * *Files identical despite different names*

### Comparing `Oasys.THIS-21.0.0b8/src/Oasys/THIS/linestyle.py` & `Oasys.THIS-21.0.0b9/src/Oasys/THIS/linestyle.py`

 * *Files identical despite different names*

### Comparing `Oasys.THIS-21.0.0b8/src/Oasys/THIS/linewidth.py` & `Oasys.THIS-21.0.0b9/src/Oasys/THIS/linewidth.py`

 * *Files identical despite different names*

### Comparing `Oasys.THIS-21.0.0b8/src/Oasys/THIS/model.py` & `Oasys.THIS-21.0.0b9/src/Oasys/THIS/model.py`

 * *Files identical despite different names*

### Comparing `Oasys.THIS-21.0.0b8/src/Oasys/THIS/operate.py` & `Oasys.THIS-21.0.0b9/src/Oasys/THIS/operate.py`

 * *Files identical despite different names*

### Comparing `Oasys.THIS-21.0.0b8/src/Oasys/THIS/options.py` & `Oasys.THIS-21.0.0b9/src/Oasys/THIS/options.py`

 * *Files identical despite different names*

### Comparing `Oasys.THIS-21.0.0b8/src/Oasys/THIS/page.py` & `Oasys.THIS-21.0.0b9/src/Oasys/THIS/page.py`

 * *Files identical despite different names*

### Comparing `Oasys.THIS-21.0.0b8/src/Oasys/THIS/read.py` & `Oasys.THIS-21.0.0b9/src/Oasys/THIS/read.py`

 * *Files identical despite different names*

### Comparing `Oasys.THIS-21.0.0b8/src/Oasys/THIS/symbol.py` & `Oasys.THIS-21.0.0b9/src/Oasys/THIS/symbol.py`

 * *Files identical despite different names*

### Comparing `Oasys.THIS-21.0.0b8/src/Oasys/THIS/units.py` & `Oasys.THIS-21.0.0b9/src/Oasys/THIS/units.py`

 * *Files identical despite different names*

### Comparing `Oasys.THIS-21.0.0b8/src/Oasys/THIS/unitsystem.py` & `Oasys.THIS-21.0.0b9/src/Oasys/THIS/unitsystem.py`

 * *Files identical despite different names*

### Comparing `Oasys.THIS-21.0.0b8/src/Oasys/THIS/utils.py` & `Oasys.THIS-21.0.0b9/src/Oasys/THIS/utils.py`

 * *Files identical despite different names*

### Comparing `Oasys.THIS-21.0.0b8/src/Oasys/THIS/window.py` & `Oasys.THIS-21.0.0b9/src/Oasys/THIS/window.py`

 * *Files identical despite different names*

### Comparing `Oasys.THIS-21.0.0b8/src/Oasys/THIS/workflow.py` & `Oasys.THIS-21.0.0b9/src/Oasys/THIS/workflow.py`

 * *Files identical despite different names*

### Comparing `Oasys.THIS-21.0.0b8/src/Oasys.THIS.egg-info/PKG-INFO` & `Oasys.THIS-21.0.0b9/src/Oasys.THIS.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Oasys.THIS
-Version: 21.0.0b8
+Version: 21.0.0b9
 Summary: Python API for Oasys T/HIS
 Author: Miles Thornton
 Maintainer-email: DYNA support <dyna.support@arup.com>
 License: MIT License
         
         Copyright (c) 2024 Oasys Ltd
         
@@ -30,15 +30,15 @@
 Project-URL: Homepage, https://www.oasys-software.com/dyna/software/t-his/
 Project-URL: Linkedin, https://www.linkedin.com/company/oasys-ltd-software/
 Project-URL: YouTube, https://www.youtube.com/c/OasysLtd
 Keywords: Oasys,THIS,T/HIS
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: Oasys.gRPC>=21.0.0b6
+Requires-Dist: Oasys.gRPC>=21.0.0b7
 
 The Oasys.THIS package allows Python scripts to control the Oasys LS-DYNA Environment
 software `T/HIS <https://www.oasys-software.com/dyna/software/t-his/>`_.
 
 Basic Information
 -----------------
```

### Comparing `Oasys.THIS-21.0.0b8/src/Oasys.THIS.egg-info/SOURCES.txt` & `Oasys.THIS-21.0.0b9/src/Oasys.THIS.egg-info/SOURCES.txt`

 * *Files identical despite different names*

