# Comparing `tmp/Oasys.REPORTER-21.0.0b8.tar.gz` & `tmp/Oasys.REPORTER-21.0.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Oasys.REPORTER-21.0.0b8.tar", last modified: Thu Feb 29 17:36:32 2024, max compression
+gzip compressed data, was "Oasys.REPORTER-21.0.0b9.tar", last modified: Fri Mar  8 14:49:40 2024, max compression
```

## Comparing `Oasys.REPORTER-21.0.0b8.tar` & `Oasys.REPORTER-21.0.0b9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-02-29 17:36:32.435202 Oasys.REPORTER-21.0.0b8/
--rw-rw-rw-   0        0        0     1086 2024-01-18 09:17:47.000000 Oasys.REPORTER-21.0.0b8/LICENSE
--rw-rw-rw-   0        0        0     6285 2024-02-29 17:36:32.434207 Oasys.REPORTER-21.0.0b8/PKG-INFO
--rw-rw-rw-   0        0        0     4385 2023-10-04 15:20:46.000000 Oasys.REPORTER-21.0.0b8/README.rst
--rw-rw-rw-   0        0        0      788 2024-02-29 17:33:06.000000 Oasys.REPORTER-21.0.0b8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-29 17:36:32.435202 Oasys.REPORTER-21.0.0b8/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-02-29 17:36:32.254418 Oasys.REPORTER-21.0.0b8/src/
-drwxrwxrwx   0        0        0        0 2024-02-29 17:36:32.255419 Oasys.REPORTER-21.0.0b8/src/Oasys/
-drwxrwxrwx   0        0        0        0 2024-02-29 17:36:32.431201 Oasys.REPORTER-21.0.0b8/src/Oasys/REPORTER/
--rw-rw-rw-   0        0        0      726 2024-02-29 17:27:47.000000 Oasys.REPORTER-21.0.0b8/src/Oasys/REPORTER/__init__.py
--rw-rw-rw-   0        0        0     5875 2024-02-29 17:27:47.000000 Oasys.REPORTER-21.0.0b8/src/Oasys/REPORTER/colour.py
--rw-rw-rw-   0        0        0     2560 2024-02-29 17:27:47.000000 Oasys.REPORTER-21.0.0b8/src/Oasys/REPORTER/core.py
--rw-rw-rw-   0        0        0     3776 2024-02-29 17:27:47.000000 Oasys.REPORTER-21.0.0b8/src/Oasys/REPORTER/funcs.py
--rw-rw-rw-   0        0        0     9181 2024-02-29 17:27:47.000000 Oasys.REPORTER-21.0.0b8/src/Oasys/REPORTER/image.py
--rw-rw-rw-   0        0        0      753 2024-02-29 17:27:47.000000 Oasys.REPORTER-21.0.0b8/src/Oasys/REPORTER/include.py
--rw-rw-rw-   0        0        0    20110 2024-02-29 17:27:47.000000 Oasys.REPORTER-21.0.0b8/src/Oasys/REPORTER/item.py
--rw-rw-rw-   0        0        0      629 2023-08-10 13:13:39.000000 Oasys.REPORTER-21.0.0b8/src/Oasys/REPORTER/itemobject.py
--rw-rw-rw-   0        0        0      996 2024-02-29 17:27:47.000000 Oasys.REPORTER-21.0.0b8/src/Oasys/REPORTER/options.py
--rw-rw-rw-   0        0        0     4491 2024-02-29 17:27:47.000000 Oasys.REPORTER-21.0.0b8/src/Oasys/REPORTER/page.py
--rw-rw-rw-   0        0        0     1447 2024-02-29 17:27:47.000000 Oasys.REPORTER-21.0.0b8/src/Oasys/REPORTER/reporter.py
--rw-rw-rw-   0        0        0    11499 2024-02-29 17:27:47.000000 Oasys.REPORTER-21.0.0b8/src/Oasys/REPORTER/template.py
--rw-rw-rw-   0        0        0     4491 2024-02-29 17:27:47.000000 Oasys.REPORTER-21.0.0b8/src/Oasys/REPORTER/utils.py
--rw-rw-rw-   0        0        0     4407 2024-02-29 17:27:47.000000 Oasys.REPORTER-21.0.0b8/src/Oasys/REPORTER/variable.py
--rw-rw-rw-   0        0        0     8450 2024-02-29 17:27:47.000000 Oasys.REPORTER-21.0.0b8/src/Oasys/REPORTER/window.py
-drwxrwxrwx   0        0        0        0 2024-02-29 17:36:32.432202 Oasys.REPORTER-21.0.0b8/src/Oasys.REPORTER.egg-info/
--rw-rw-rw-   0        0        0     6285 2024-02-29 17:36:32.000000 Oasys.REPORTER-21.0.0b8/src/Oasys.REPORTER.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      682 2024-02-29 17:36:32.000000 Oasys.REPORTER-21.0.0b8/src/Oasys.REPORTER.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-29 17:36:32.000000 Oasys.REPORTER-21.0.0b8/src/Oasys.REPORTER.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2024-02-29 17:36:32.000000 Oasys.REPORTER-21.0.0b8/src/Oasys.REPORTER.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-02-29 17:36:32.000000 Oasys.REPORTER-21.0.0b8/src/Oasys.REPORTER.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-03-08 14:49:40.356643 Oasys.REPORTER-21.0.0b9/
+-rw-rw-rw-   0        0        0     1086 2024-01-18 09:17:47.000000 Oasys.REPORTER-21.0.0b9/LICENSE
+-rw-rw-rw-   0        0        0     6285 2024-03-08 14:49:40.355643 Oasys.REPORTER-21.0.0b9/PKG-INFO
+-rw-rw-rw-   0        0        0     4385 2023-10-04 15:20:46.000000 Oasys.REPORTER-21.0.0b9/README.rst
+-rw-rw-rw-   0        0        0      788 2024-03-07 13:43:06.000000 Oasys.REPORTER-21.0.0b9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-03-08 14:49:40.356643 Oasys.REPORTER-21.0.0b9/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-03-08 14:49:40.309643 Oasys.REPORTER-21.0.0b9/src/
+drwxrwxrwx   0        0        0        0 2024-03-08 14:49:40.309643 Oasys.REPORTER-21.0.0b9/src/Oasys/
+drwxrwxrwx   0        0        0        0 2024-03-08 14:49:40.352642 Oasys.REPORTER-21.0.0b9/src/Oasys/REPORTER/
+-rw-rw-rw-   0        0        0      726 2024-03-08 14:42:52.000000 Oasys.REPORTER-21.0.0b9/src/Oasys/REPORTER/__init__.py
+-rw-rw-rw-   0        0        0     6353 2024-03-08 14:42:52.000000 Oasys.REPORTER-21.0.0b9/src/Oasys/REPORTER/colour.py
+-rw-rw-rw-   0        0        0     3219 2024-03-08 14:42:52.000000 Oasys.REPORTER-21.0.0b9/src/Oasys/REPORTER/core.py
+-rw-rw-rw-   0        0        0     3776 2024-03-08 14:42:52.000000 Oasys.REPORTER-21.0.0b9/src/Oasys/REPORTER/funcs.py
+-rw-rw-rw-   0        0        0     9873 2024-03-08 14:42:52.000000 Oasys.REPORTER-21.0.0b9/src/Oasys/REPORTER/image.py
+-rw-rw-rw-   0        0        0     1453 2024-03-08 14:42:52.000000 Oasys.REPORTER-21.0.0b9/src/Oasys/REPORTER/include.py
+-rw-rw-rw-   0        0        0    20864 2024-03-08 14:42:52.000000 Oasys.REPORTER-21.0.0b9/src/Oasys/REPORTER/item.py
+-rw-rw-rw-   0        0        0      629 2023-08-10 13:13:39.000000 Oasys.REPORTER-21.0.0b9/src/Oasys/REPORTER/itemobject.py
+-rw-rw-rw-   0        0        0     1887 2024-03-08 14:42:52.000000 Oasys.REPORTER-21.0.0b9/src/Oasys/REPORTER/options.py
+-rw-rw-rw-   0        0        0     4963 2024-03-08 14:42:52.000000 Oasys.REPORTER-21.0.0b9/src/Oasys/REPORTER/page.py
+-rw-rw-rw-   0        0        0     2151 2024-03-08 14:42:52.000000 Oasys.REPORTER-21.0.0b9/src/Oasys/REPORTER/reporter.py
+-rw-rw-rw-   0        0        0    11983 2024-03-08 14:42:52.000000 Oasys.REPORTER-21.0.0b9/src/Oasys/REPORTER/template.py
+-rw-rw-rw-   0        0        0     4899 2024-03-08 14:42:52.000000 Oasys.REPORTER-21.0.0b9/src/Oasys/REPORTER/utils.py
+-rw-rw-rw-   0        0        0     5111 2024-03-08 14:42:52.000000 Oasys.REPORTER-21.0.0b9/src/Oasys/REPORTER/variable.py
+-rw-rw-rw-   0        0        0     9146 2024-03-08 14:42:52.000000 Oasys.REPORTER-21.0.0b9/src/Oasys/REPORTER/window.py
+drwxrwxrwx   0        0        0        0 2024-03-08 14:49:40.354642 Oasys.REPORTER-21.0.0b9/src/Oasys.REPORTER.egg-info/
+-rw-rw-rw-   0        0        0     6285 2024-03-08 14:49:40.000000 Oasys.REPORTER-21.0.0b9/src/Oasys.REPORTER.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      682 2024-03-08 14:49:40.000000 Oasys.REPORTER-21.0.0b9/src/Oasys.REPORTER.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-08 14:49:40.000000 Oasys.REPORTER-21.0.0b9/src/Oasys.REPORTER.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2024-03-08 14:49:40.000000 Oasys.REPORTER-21.0.0b9/src/Oasys.REPORTER.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-03-08 14:49:40.000000 Oasys.REPORTER-21.0.0b9/src/Oasys.REPORTER.egg-info/top_level.txt
```

### Comparing `Oasys.REPORTER-21.0.0b8/LICENSE` & `Oasys.REPORTER-21.0.0b9/LICENSE`

 * *Files identical despite different names*

### Comparing `Oasys.REPORTER-21.0.0b8/PKG-INFO` & `Oasys.REPORTER-21.0.0b9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Oasys.REPORTER
-Version: 21.0.0b8
+Version: 21.0.0b9
 Summary: Python API for Oasys REPORTER
 Author: Miles Thornton
 Maintainer-email: DYNA support <dyna.support@arup.com>
 License: MIT License
         
         Copyright (c) 2024 Oasys Ltd
         
@@ -27,18 +27,18 @@
         SOFTWARE
         
 Project-URL: Documentation, https://www.oasys-software.com/dyna/sphinx/21.0/REPORTER/
 Project-URL: Homepage, https://www.oasys-software.com/dyna/software/reporter/
 Project-URL: Linkedin, https://www.linkedin.com/company/oasys-ltd-software/
 Project-URL: YouTube, https://www.youtube.com/c/OasysLtd
 Keywords: Oasys,REPORTER
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: Oasys.gRPC>=21.0.0b7
+Requires-Dist: Oasys.gRPC>=21.0.0b8
 
 The Oasys.REPORTER package allows Python scripts to control the Oasys LS-DYNA Environment
 software `REPORTER <https://www.oasys-software.com/dyna/software/reporter/>`_.
 
 Basic Information
 -----------------
```

### Comparing `Oasys.REPORTER-21.0.0b8/README.rst` & `Oasys.REPORTER-21.0.0b9/README.rst`

 * *Files identical despite different names*

### Comparing `Oasys.REPORTER-21.0.0b8/pyproject.toml` & `Oasys.REPORTER-21.0.0b9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "Oasys.REPORTER"
-version = "21.0.0b8"
+version = "21.0.0b9"
 license = {file = "LICENSE"}
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 keywords = ["Oasys", "REPORTER"]
 dependencies = [
-  "Oasys.gRPC >= 21.0.0b7"
+  "Oasys.gRPC >= 21.0.0b8"
 ]
 description = "Python API for Oasys REPORTER"
 readme = "README.rst"
 authors = [
   {name = "Miles Thornton"},
 ]
 maintainers = [
```

### Comparing `Oasys.REPORTER-21.0.0b8/src/Oasys/REPORTER/__init__.py` & `Oasys.REPORTER-21.0.0b9/src/Oasys/REPORTER/__init__.py`

 * *Files identical despite different names*

### Comparing `Oasys.REPORTER-21.0.0b8/src/Oasys/REPORTER/colour.py` & `Oasys.REPORTER-21.0.0b9/src/Oasys/REPORTER/colour.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,40 +2,48 @@
 
 
 # Metaclass for static properties and constants
 class ColourType(type):
 
     def __getattr__(cls, name):
 
-        raise AttributeError
+        raise AttributeError("Colour class attribute '{}' does not exist".format(name))
 
 
 class Colour(Oasys.gRPC.OasysItem, metaclass=ColourType):
     _rprops = {'blue', 'green', 'name', 'red'}
 
 
     def __del__(self):
         if not Oasys.REPORTER._connection:
             return
 
+        if self._handle is None:
+            return
+
         Oasys.REPORTER._connection.destructor(self.__class__.__name__, self._handle)
 
 
     def __getattr__(self, name):
+# If constructor for an item fails in program, then _handle will not be set and when
+# __del__ is called to return the object we will call this to get the (undefined) value
+        if name == "_handle":
+            return None
+
 # If one of the read only properties we define then get it
         if name in Colour._rprops:
             return Oasys.REPORTER._connection.instanceGetter(self.__class__.__name__, self._handle, name)
 
-        raise AttributeError
+        raise AttributeError("Colour instance attribute '{}' does not exist".format(name))
 
 
     def __setattr__(self, name, value):
 # If one of the read only properties we define then error
         if name in Colour._rprops:
-            raise AttributeError
+            raise AttributeError("Cannot set read-only Colour instance attribute '{}'".format(name))
 
 # Set the property locally
         self.__dict__[name] = value
 
 
 # Static methods
     def Black():
```

### Comparing `Oasys.REPORTER-21.0.0b8/src/Oasys/REPORTER/core.py` & `Oasys.REPORTER-21.0.0b9/src/Oasys/REPORTER/core.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import subprocess
 import time
+import importlib.metadata
 import Oasys.gRPC
 
 
 _connection = None
 _debug      = False
 
 
@@ -26,14 +27,27 @@
 
 def connect(port=50053, memory=25, hostname='localhost', debug=False):
     if debug:
         print("Called connect with port {} and memory {}".format(port, memory))
 
     Oasys.REPORTER._debug      = debug
     Oasys.REPORTER._connection = Oasys.gRPC.Connection("REPORTER", port, memory, hostname, debug)
+
+# Check version
+    version  = importlib.metadata.version('Oasys.REPORTER')
+    modMajor = int(version.split('.')[0]);
+    exeMajor = int(Oasys.REPORTER._connection.version);
+
+    if debug:
+        print("Oasys.REPORTER module version {} ({})".format(modMajor, version))
+        print("REPORTER executable version {} ({})".format(exeMajor, Oasys.REPORTER._connection.version))
+
+    if exeMajor < modMajor:
+        raise ValueError("Major version ({}) of REPORTER executable {} < major version ({}) of Oasys.REPORTER module {}. Cannot continue".format(exeMajor, Oasys.REPORTER._connection.version, modMajor, version))
+
     return Oasys.REPORTER._connection
 
 
 def disconnect(connection):
     if Oasys.REPORTER._debug:
         print("Called disconnect")
```

### Comparing `Oasys.REPORTER-21.0.0b8/src/Oasys/REPORTER/funcs.py` & `Oasys.REPORTER-21.0.0b9/src/Oasys/REPORTER/funcs.py`

 * *Files identical despite different names*

### Comparing `Oasys.REPORTER-21.0.0b8/src/Oasys/REPORTER/image.py` & `Oasys.REPORTER-21.0.0b9/src/Oasys/REPORTER/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,34 +5,51 @@
 class ImageType(type):
     _consts = {'BMP', 'JPG', 'PNG'}
 
     def __getattr__(cls, name):
         if name in ImageType._consts:
             return Oasys.REPORTER._connection.classGetter(cls.__name__, name)
 
-        raise AttributeError
+        raise AttributeError("Image class attribute '{}' does not exist".format(name))
+
+
+    def __setattr__(cls, name, value):
+# If one of the constants we define then error
+        if name in ImageType._consts:
+            raise AttributeError("Cannot set Image class constant '{}'".format(name))
+
+# Set the property locally
+        cls.__dict__[name] = value
 
 
 class Image(Oasys.gRPC.OasysItem, metaclass=ImageType):
     _props = {'antialiasing', 'fillColour', 'font', 'fontAngle', 'fontColour', 'fontJustify', 'fontSize', 'fontStyle', 'height', 'lineCapStyle', 'lineColour', 'lineJoinStyle', 'lineStyle', 'lineWidth', 'width'}
 
 
     def __del__(self):
         if not Oasys.REPORTER._connection:
             return
 
+        if self._handle is None:
+            return
+
         Oasys.REPORTER._connection.destructor(self.__class__.__name__, self._handle)
 
 
     def __getattr__(self, name):
+# If constructor for an item fails in program, then _handle will not be set and when
+# __del__ is called to return the object we will call this to get the (undefined) value
+        if name == "_handle":
+            return None
+
 # If one of the properties we define then get it
         if name in Image._props:
             return Oasys.REPORTER._connection.instanceGetter(self.__class__.__name__, self._handle, name)
 
-        raise AttributeError
+        raise AttributeError("Image instance attribute '{}' does not exist".format(name))
 
 
     def __setattr__(self, name, value):
 # If one of the properties we define then set it
         if name in Image._props:
             Oasys.REPORTER._connection.instanceSetter(self.__class__.__name__, self._handle, name, value)
             return
```

### Comparing `Oasys.REPORTER-21.0.0b8/src/Oasys/REPORTER/item.py` & `Oasys.REPORTER-21.0.0b9/src/Oasys/REPORTER/item.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,50 +5,67 @@
 class ItemType(type):
     _consts = {'ARROW', 'AUTO_TABLE', 'D3PLOT', 'ELLIPSE', 'IMAGE', 'IMAGE_FILE', 'LIBRARY_IMAGE', 'LIBRARY_PROGRAM', 'LINE', 'NOTE', 'PLACEHOLDER', 'PRIMER', 'PROGRAM', 'RECTANGLE', 'SCRIPT', 'SCRIPT_FILE', 'TABLE', 'TEXT', 'TEXTBOX', 'TEXT_FILE', 'THIS'}
 
     def __getattr__(cls, name):
         if name in ItemType._consts:
             return Oasys.REPORTER._connection.classGetter(cls.__name__, name)
 
-        raise AttributeError
+        raise AttributeError("Item class attribute '{}' does not exist".format(name))
+
+
+    def __setattr__(cls, name, value):
+# If one of the constants we define then error
+        if name in ItemType._consts:
+            raise AttributeError("Cannot set Item class constant '{}'".format(name))
+
+# Set the property locally
+        cls.__dict__[name] = value
 
 
 class Item(Oasys.gRPC.OasysItem, metaclass=ItemType):
     _props = {'active', 'autotableType', 'bottomCrop', 'bottomMargin', 'columns', 'conditions', 'embed', 'file', 'fillColour', 'fontName', 'fontSize', 'fontStyle', 'generatedRowHeight', 'headerHeight', 'height', 'job', 'justify', 'leftCrop', 'leftMargin', 'lineColour', 'lineStyle', 'lineWidth', 'name', 'resolution', 'rightCrop', 'rightMargin', 'rows', 'saveCSV', 'saveCSVFilename', 'saveXlsx', 'saveXlsxFilename', 'script', 'text', 'textColour', 'topCrop', 'topMargin', 'width', 'x', 'x2', 'y', 'y2'}
     _rprops = {'filetype', 'type'}
 
 
     def __del__(self):
         if not Oasys.REPORTER._connection:
             return
 
+        if self._handle is None:
+            return
+
         Oasys.REPORTER._connection.destructor(self.__class__.__name__, self._handle)
 
 
     def __getattr__(self, name):
+# If constructor for an item fails in program, then _handle will not be set and when
+# __del__ is called to return the object we will call this to get the (undefined) value
+        if name == "_handle":
+            return None
+
 # If one of the properties we define then get it
         if name in Item._props:
             return Oasys.REPORTER._connection.instanceGetter(self.__class__.__name__, self._handle, name)
 
 # If one of the read only properties we define then get it
         if name in Item._rprops:
             return Oasys.REPORTER._connection.instanceGetter(self.__class__.__name__, self._handle, name)
 
-        raise AttributeError
+        raise AttributeError("Item instance attribute '{}' does not exist".format(name))
 
 
     def __setattr__(self, name, value):
 # If one of the properties we define then set it
         if name in Item._props:
             Oasys.REPORTER._connection.instanceSetter(self.__class__.__name__, self._handle, name, value)
             return
 
 # If one of the read only properties we define then error
         if name in Item._rprops:
-            raise AttributeError
+            raise AttributeError("Cannot set read-only Item instance attribute '{}'".format(name))
 
 # Set the property locally
         self.__dict__[name] = value
 
 
 # Constructor
     def __init__(self, page, type, name=Oasys.gRPC.defaultArg, x=Oasys.gRPC.defaultArg, x2=Oasys.gRPC.defaultArg, y=Oasys.gRPC.defaultArg, y2=Oasys.gRPC.defaultArg):
```

### Comparing `Oasys.REPORTER-21.0.0b8/src/Oasys/REPORTER/itemobject.py` & `Oasys.REPORTER-21.0.0b9/src/Oasys/REPORTER/itemobject.py`

 * *Files identical despite different names*

### Comparing `Oasys.REPORTER-21.0.0b8/src/Oasys/REPORTER/page.py` & `Oasys.REPORTER-21.0.0b9/src/Oasys/REPORTER/page.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,50 +2,58 @@
 
 
 # Metaclass for static properties and constants
 class PageType(type):
 
     def __getattr__(cls, name):
 
-        raise AttributeError
+        raise AttributeError("Page class attribute '{}' does not exist".format(name))
 
 
 class Page(Oasys.gRPC.OasysItem, metaclass=PageType):
     _props = {'name'}
     _rprops = {'items', 'master'}
 
 
     def __del__(self):
         if not Oasys.REPORTER._connection:
             return
 
+        if self._handle is None:
+            return
+
         Oasys.REPORTER._connection.destructor(self.__class__.__name__, self._handle)
 
 
     def __getattr__(self, name):
+# If constructor for an item fails in program, then _handle will not be set and when
+# __del__ is called to return the object we will call this to get the (undefined) value
+        if name == "_handle":
+            return None
+
 # If one of the properties we define then get it
         if name in Page._props:
             return Oasys.REPORTER._connection.instanceGetter(self.__class__.__name__, self._handle, name)
 
 # If one of the read only properties we define then get it
         if name in Page._rprops:
             return Oasys.REPORTER._connection.instanceGetter(self.__class__.__name__, self._handle, name)
 
-        raise AttributeError
+        raise AttributeError("Page instance attribute '{}' does not exist".format(name))
 
 
     def __setattr__(self, name, value):
 # If one of the properties we define then set it
         if name in Page._props:
             Oasys.REPORTER._connection.instanceSetter(self.__class__.__name__, self._handle, name, value)
             return
 
 # If one of the read only properties we define then error
         if name in Page._rprops:
-            raise AttributeError
+            raise AttributeError("Cannot set read-only Page instance attribute '{}'".format(name))
 
 # Set the property locally
         self.__dict__[name] = value
 
 
 # Constructor
     def __init__(self, template, options=Oasys.gRPC.defaultArg):
```

### Comparing `Oasys.REPORTER-21.0.0b8/src/Oasys/REPORTER/reporter.py` & `Oasys.REPORTER-21.0.0b9/src/Oasys/REPORTER/reporter.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,27 +5,44 @@
 class ReporterType(type):
     _consts = {'AUTO_TABLE_DIRECTORY', 'AUTO_TABLE_FILE', 'AUTO_TABLE_HEADER', 'AUTO_TABLE_ROWS', 'CAP_FLAT', 'CAP_ROUND', 'CAP_SQUARE', 'CONDITION_BETWEEN', 'CONDITION_CONTAINS_STRING', 'CONDITION_DOESNT_CONTAIN_STRING', 'CONDITION_DOESNT_MATCH_REGEX', 'CONDITION_EQUAL_TO', 'CONDITION_GREATER_THAN', 'CONDITION_LESS_THAN', 'CONDITION_MATCHES_REGEX', 'CONDITION_NOT_BETWEEN', 'CONDITION_NOT_EQUAL_TO', 'JOIN_BEVEL', 'JOIN_MITRE', 'JOIN_ROUND', 'JUSTIFY_BOTTOM', 'JUSTIFY_CENTRE', 'JUSTIFY_LEFT', 'JUSTIFY_MIDDLE', 'JUSTIFY_RIGHT', 'JUSTIFY_TOP', 'LINE_DASH', 'LINE_DASH_DOT', 'LINE_DASH_DOT_DOT', 'LINE_DOT', 'LINE_NONE', 'LINE_SOLID', 'TEXT_BOLD', 'TEXT_ITALIC', 'TEXT_NORMAL', 'TEXT_UNDERLINE', 'VIEW_DESIGN', 'VIEW_PRESENTATION'}
 
     def __getattr__(cls, name):
         if name in ReporterType._consts:
             return Oasys.REPORTER._connection.classGetter(cls.__name__, name)
 
-        raise AttributeError
+        raise AttributeError("Reporter class attribute '{}' does not exist".format(name))
+
+
+    def __setattr__(cls, name, value):
+# If one of the constants we define then error
+        if name in ReporterType._consts:
+            raise AttributeError("Cannot set Reporter class constant '{}'".format(name))
+
+# Set the property locally
+        cls.__dict__[name] = value
 
 
 class Reporter(Oasys.gRPC.OasysItem, metaclass=ReporterType):
 
 
     def __del__(self):
         if not Oasys.REPORTER._connection:
             return
 
+        if self._handle is None:
+            return
+
         Oasys.REPORTER._connection.destructor(self.__class__.__name__, self._handle)
 
 
     def __getattr__(self, name):
-        raise AttributeError
+# If constructor for an item fails in program, then _handle will not be set and when
+# __del__ is called to return the object we will call this to get the (undefined) value
+        if name == "_handle":
+            return None
+
+        raise AttributeError("Reporter instance attribute '{}' does not exist".format(name))
 
 
     def __setattr__(self, name, value):
 # Set the property locally
         self.__dict__[name] = value
```

### Comparing `Oasys.REPORTER-21.0.0b8/src/Oasys/REPORTER/template.py` & `Oasys.REPORTER-21.0.0b9/src/Oasys/REPORTER/template.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,50 +2,58 @@
 
 
 # Metaclass for static properties and constants
 class TemplateType(type):
 
     def __getattr__(cls, name):
 
-        raise AttributeError
+        raise AttributeError("Template class attribute '{}' does not exist".format(name))
 
 
 class Template(Oasys.gRPC.OasysItem, metaclass=TemplateType):
     _props = {'view'}
     _rprops = {'filename', 'pages', 'path'}
 
 
     def __del__(self):
         if not Oasys.REPORTER._connection:
             return
 
+        if self._handle is None:
+            return
+
         Oasys.REPORTER._connection.destructor(self.__class__.__name__, self._handle)
 
 
     def __getattr__(self, name):
+# If constructor for an item fails in program, then _handle will not be set and when
+# __del__ is called to return the object we will call this to get the (undefined) value
+        if name == "_handle":
+            return None
+
 # If one of the properties we define then get it
         if name in Template._props:
             return Oasys.REPORTER._connection.instanceGetter(self.__class__.__name__, self._handle, name)
 
 # If one of the read only properties we define then get it
         if name in Template._rprops:
             return Oasys.REPORTER._connection.instanceGetter(self.__class__.__name__, self._handle, name)
 
-        raise AttributeError
+        raise AttributeError("Template instance attribute '{}' does not exist".format(name))
 
 
     def __setattr__(self, name, value):
 # If one of the properties we define then set it
         if name in Template._props:
             Oasys.REPORTER._connection.instanceSetter(self.__class__.__name__, self._handle, name, value)
             return
 
 # If one of the read only properties we define then error
         if name in Template._rprops:
-            raise AttributeError
+            raise AttributeError("Cannot set read-only Template instance attribute '{}'".format(name))
 
 # Set the property locally
         self.__dict__[name] = value
 
 
 # Constructor
     def __init__(self, filename=Oasys.gRPC.defaultArg):
```

### Comparing `Oasys.REPORTER-21.0.0b8/src/Oasys/REPORTER/utils.py` & `Oasys.REPORTER-21.0.0b9/src/Oasys/REPORTER/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,29 +2,37 @@
 
 
 # Metaclass for static properties and constants
 class UtilsType(type):
 
     def __getattr__(cls, name):
 
-        raise AttributeError
+        raise AttributeError("Utils class attribute '{}' does not exist".format(name))
 
 
 class Utils(Oasys.gRPC.OasysItem, metaclass=UtilsType):
 
 
     def __del__(self):
         if not Oasys.REPORTER._connection:
             return
 
+        if self._handle is None:
+            return
+
         Oasys.REPORTER._connection.destructor(self.__class__.__name__, self._handle)
 
 
     def __getattr__(self, name):
-        raise AttributeError
+# If constructor for an item fails in program, then _handle will not be set and when
+# __del__ is called to return the object we will call this to get the (undefined) value
+        if name == "_handle":
+            return None
+
+        raise AttributeError("Utils instance attribute '{}' does not exist".format(name))
 
 
     def __setattr__(self, name, value):
 # Set the property locally
         self.__dict__[name] = value
```

### Comparing `Oasys.REPORTER-21.0.0b8/src/Oasys/REPORTER/variable.py` & `Oasys.REPORTER-21.0.0b9/src/Oasys/REPORTER/variable.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,34 +5,51 @@
 class VariableType(type):
     _consts = {'DESCRIPTION', 'FORMAT', 'FORMAT_FLOAT', 'FORMAT_GENERAL', 'FORMAT_INTEGER', 'FORMAT_LOWERCASE', 'FORMAT_NONE', 'FORMAT_SCIENTIFIC', 'FORMAT_UPPERCASE', 'NAME', 'PRECISION', 'READONLY', 'TEMPORARY', 'TYPE', 'VALUE'}
 
     def __getattr__(cls, name):
         if name in VariableType._consts:
             return Oasys.REPORTER._connection.classGetter(cls.__name__, name)
 
-        raise AttributeError
+        raise AttributeError("Variable class attribute '{}' does not exist".format(name))
+
+
+    def __setattr__(cls, name, value):
+# If one of the constants we define then error
+        if name in VariableType._consts:
+            raise AttributeError("Cannot set Variable class constant '{}'".format(name))
+
+# Set the property locally
+        cls.__dict__[name] = value
 
 
 class Variable(Oasys.gRPC.OasysItem, metaclass=VariableType):
     _props = {'description', 'format', 'name', 'precision', 'readonly', 'temporary', 'type', 'value'}
 
 
     def __del__(self):
         if not Oasys.REPORTER._connection:
             return
 
+        if self._handle is None:
+            return
+
         Oasys.REPORTER._connection.destructor(self.__class__.__name__, self._handle)
 
 
     def __getattr__(self, name):
+# If constructor for an item fails in program, then _handle will not be set and when
+# __del__ is called to return the object we will call this to get the (undefined) value
+        if name == "_handle":
+            return None
+
 # If one of the properties we define then get it
         if name in Variable._props:
             return Oasys.REPORTER._connection.instanceGetter(self.__class__.__name__, self._handle, name)
 
-        raise AttributeError
+        raise AttributeError("Variable instance attribute '{}' does not exist".format(name))
 
 
     def __setattr__(self, name, value):
 # If one of the properties we define then set it
         if name in Variable._props:
             Oasys.REPORTER._connection.instanceSetter(self.__class__.__name__, self._handle, name, value)
             return
```

### Comparing `Oasys.REPORTER-21.0.0b8/src/Oasys/REPORTER/window.py` & `Oasys.REPORTER-21.0.0b9/src/Oasys/REPORTER/window.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,46 @@
 class WindowType(type):
     _consts = {'CANCEL', 'NO', 'OK', 'YES'}
 
     def __getattr__(cls, name):
         if name in WindowType._consts:
             return Oasys.REPORTER._connection.classGetter(cls.__name__, name)
 
-        raise AttributeError
+        raise AttributeError("Window class attribute '{}' does not exist".format(name))
+
+
+    def __setattr__(cls, name, value):
+# If one of the constants we define then error
+        if name in WindowType._consts:
+            raise AttributeError("Cannot set Window class constant '{}'".format(name))
+
+# Set the property locally
+        cls.__dict__[name] = value
 
 
 class Window(Oasys.gRPC.OasysItem, metaclass=WindowType):
 
 
     def __del__(self):
         if not Oasys.REPORTER._connection:
             return
 
+        if self._handle is None:
+            return
+
         Oasys.REPORTER._connection.destructor(self.__class__.__name__, self._handle)
 
 
     def __getattr__(self, name):
-        raise AttributeError
+# If constructor for an item fails in program, then _handle will not be set and when
+# __del__ is called to return the object we will call this to get the (undefined) value
+        if name == "_handle":
+            return None
+
+        raise AttributeError("Window instance attribute '{}' does not exist".format(name))
 
 
     def __setattr__(self, name, value):
 # Set the property locally
         self.__dict__[name] = value
```

### Comparing `Oasys.REPORTER-21.0.0b8/src/Oasys.REPORTER.egg-info/PKG-INFO` & `Oasys.REPORTER-21.0.0b9/src/Oasys.REPORTER.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Oasys.REPORTER
-Version: 21.0.0b8
+Version: 21.0.0b9
 Summary: Python API for Oasys REPORTER
 Author: Miles Thornton
 Maintainer-email: DYNA support <dyna.support@arup.com>
 License: MIT License
         
         Copyright (c) 2024 Oasys Ltd
         
@@ -27,18 +27,18 @@
         SOFTWARE
         
 Project-URL: Documentation, https://www.oasys-software.com/dyna/sphinx/21.0/REPORTER/
 Project-URL: Homepage, https://www.oasys-software.com/dyna/software/reporter/
 Project-URL: Linkedin, https://www.linkedin.com/company/oasys-ltd-software/
 Project-URL: YouTube, https://www.youtube.com/c/OasysLtd
 Keywords: Oasys,REPORTER
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: Oasys.gRPC>=21.0.0b7
+Requires-Dist: Oasys.gRPC>=21.0.0b8
 
 The Oasys.REPORTER package allows Python scripts to control the Oasys LS-DYNA Environment
 software `REPORTER <https://www.oasys-software.com/dyna/software/reporter/>`_.
 
 Basic Information
 -----------------
```

### Comparing `Oasys.REPORTER-21.0.0b8/src/Oasys.REPORTER.egg-info/SOURCES.txt` & `Oasys.REPORTER-21.0.0b9/src/Oasys.REPORTER.egg-info/SOURCES.txt`

 * *Files identical despite different names*

