# Comparing `tmp/prusek_spheroid-3.2.tar.gz` & `tmp/prusek_spheroid-3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prusek_spheroid-3.2.tar", last modified: Tue Apr  2 12:01:24 2024, max compression
+gzip compressed data, was "prusek_spheroid-3.3.tar", last modified: Tue Apr  2 12:13:42 2024, max compression
```

## Comparing `prusek_spheroid-3.2.tar` & `prusek_spheroid-3.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-02 12:01:24.787548 prusek_spheroid-3.2/
--rw-r--r--   0 michalprusek   (501) staff       (20)     9069 2024-04-02 12:01:24.787350 prusek_spheroid-3.2/PKG-INFO
--rw-r--r--   0 michalprusek   (501) staff       (20)     8544 2024-03-27 11:29:11.000000 prusek_spheroid-3.2/README.md
-drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-02 12:01:24.786146 prusek_spheroid-3.2/prusek_spheroid/
--rw-r--r--   0 michalprusek   (501) staff       (20)    16442 2024-03-29 08:04:06.000000 prusek_spheroid-3.2/prusek_spheroid/ContoursClassGUI.py
--rw-r--r--   0 michalprusek   (501) staff       (20)    35159 2024-04-02 11:58:27.000000 prusek_spheroid-3.2/prusek_spheroid/GUI.py
--rw-r--r--   0 michalprusek   (501) staff       (20)    12427 2024-03-22 06:33:48.000000 prusek_spheroid-3.2/prusek_spheroid/GradientDescentGUI.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     2370 2024-03-25 13:56:52.000000 prusek_spheroid-3.2/prusek_spheroid/calculate_iou.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     4491 2024-01-27 10:12:42.000000 prusek_spheroid-3.2/prusek_spheroid/characteristic_functions.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     7059 2024-04-02 11:58:27.000000 prusek_spheroid-3.2/prusek_spheroid/file_management.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     3466 2024-04-02 09:37:18.000000 prusek_spheroid-3.2/prusek_spheroid/image_processing.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     3705 2024-04-02 09:37:18.000000 prusek_spheroid-3.2/prusek_spheroid/methods.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     4632 2024-03-27 08:31:17.000000 prusek_spheroid-3.2/prusek_spheroid/selection_dialog.py
-drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-02 12:01:24.787142 prusek_spheroid-3.2/prusek_spheroid.egg-info/
--rw-r--r--   0 michalprusek   (501) staff       (20)     9069 2024-04-02 12:01:24.000000 prusek_spheroid-3.2/prusek_spheroid.egg-info/PKG-INFO
--rw-r--r--   0 michalprusek   (501) staff       (20)      520 2024-04-02 12:01:24.000000 prusek_spheroid-3.2/prusek_spheroid.egg-info/SOURCES.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)        1 2024-04-02 12:01:24.000000 prusek_spheroid-3.2/prusek_spheroid.egg-info/dependency_links.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)      110 2024-04-02 12:01:24.000000 prusek_spheroid-3.2/prusek_spheroid.egg-info/requires.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)       16 2024-04-02 12:01:24.000000 prusek_spheroid-3.2/prusek_spheroid.egg-info/top_level.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)       38 2024-04-02 12:01:24.787596 prusek_spheroid-3.2/setup.cfg
--rw-r--r--   0 michalprusek   (501) staff       (20)      729 2024-04-02 12:01:03.000000 prusek_spheroid-3.2/setup.py
+drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-02 12:13:42.377776 prusek_spheroid-3.3/
+-rw-r--r--   0 michalprusek   (501) staff       (20)     9069 2024-04-02 12:13:42.377497 prusek_spheroid-3.3/PKG-INFO
+-rw-r--r--   0 michalprusek   (501) staff       (20)     8544 2024-03-27 11:29:11.000000 prusek_spheroid-3.3/README.md
+drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-02 12:13:42.376134 prusek_spheroid-3.3/prusek_spheroid/
+-rw-r--r--   0 michalprusek   (501) staff       (20)    16442 2024-03-29 08:04:06.000000 prusek_spheroid-3.3/prusek_spheroid/ContoursClassGUI.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)    35159 2024-04-02 11:58:27.000000 prusek_spheroid-3.3/prusek_spheroid/GUI.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)    12427 2024-03-22 06:33:48.000000 prusek_spheroid-3.3/prusek_spheroid/GradientDescentGUI.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     2370 2024-03-25 13:56:52.000000 prusek_spheroid-3.3/prusek_spheroid/calculate_iou.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     4491 2024-01-27 10:12:42.000000 prusek_spheroid-3.3/prusek_spheroid/characteristic_functions.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     7200 2024-04-02 12:11:35.000000 prusek_spheroid-3.3/prusek_spheroid/file_management.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     3466 2024-04-02 09:37:18.000000 prusek_spheroid-3.3/prusek_spheroid/image_processing.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     3705 2024-04-02 09:37:18.000000 prusek_spheroid-3.3/prusek_spheroid/methods.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     4632 2024-03-27 08:31:17.000000 prusek_spheroid-3.3/prusek_spheroid/selection_dialog.py
+drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-02 12:13:42.377221 prusek_spheroid-3.3/prusek_spheroid.egg-info/
+-rw-r--r--   0 michalprusek   (501) staff       (20)     9069 2024-04-02 12:13:42.000000 prusek_spheroid-3.3/prusek_spheroid.egg-info/PKG-INFO
+-rw-r--r--   0 michalprusek   (501) staff       (20)      520 2024-04-02 12:13:42.000000 prusek_spheroid-3.3/prusek_spheroid.egg-info/SOURCES.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)        1 2024-04-02 12:13:42.000000 prusek_spheroid-3.3/prusek_spheroid.egg-info/dependency_links.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)      110 2024-04-02 12:13:42.000000 prusek_spheroid-3.3/prusek_spheroid.egg-info/requires.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)       16 2024-04-02 12:13:42.000000 prusek_spheroid-3.3/prusek_spheroid.egg-info/top_level.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)       38 2024-04-02 12:13:42.377824 prusek_spheroid-3.3/setup.cfg
+-rw-r--r--   0 michalprusek   (501) staff       (20)      729 2024-04-02 12:13:11.000000 prusek_spheroid-3.3/setup.py
```

### Comparing `prusek_spheroid-3.2/PKG-INFO` & `prusek_spheroid-3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prusek_spheroid
-Version: 3.2
+Version: 3.3
 Summary: Spheroid segmentation package
 Home-page: https://github.com/michalprusek/prusek-spheroid
 Author: Michal Prusek
 Author-email: prusemic@cvut.cz
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: opencv-python
```

### Comparing `prusek_spheroid-3.2/README.md` & `prusek_spheroid-3.3/README.md`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-3.2/prusek_spheroid/ContoursClassGUI.py` & `prusek_spheroid-3.3/prusek_spheroid/ContoursClassGUI.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-3.2/prusek_spheroid/GUI.py` & `prusek_spheroid-3.3/prusek_spheroid/GUI.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-3.2/prusek_spheroid/GradientDescentGUI.py` & `prusek_spheroid-3.3/prusek_spheroid/GradientDescentGUI.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-3.2/prusek_spheroid/calculate_iou.py` & `prusek_spheroid-3.3/prusek_spheroid/calculate_iou.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-3.2/prusek_spheroid/characteristic_functions.py` & `prusek_spheroid-3.3/prusek_spheroid/characteristic_functions.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-3.2/prusek_spheroid/file_management.py` & `prusek_spheroid-3.3/prusek_spheroid/file_management.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,24 +6,28 @@
 import json as js
 from tkinter import messagebox
 
 
 import zipfile
 import os
 
+
 def unzip(zip_file_path):
-    # Získá cestu ke složce, kde se nachází zip soubor
-    extract_path = os.path.dirname(zip_file_path)
+    # Odstranění přípony '.zip' a vytvoření cesty pro cílovou složku
+    base_path = os.path.splitext(zip_file_path)[0]
 
-    with zipfile.ZipFile(zip_file_path, 'r') as zip_ref:
-        zip_ref.extractall(extract_path)
+    # Kontrola, zda cílová složka již existuje. Pokud ne, vytvoří ji.
+    if not os.path.exists(base_path):
+        os.makedirs(base_path)
 
-    annotation_address, _ = os.path.splitext(zip_file_path)
+    # Extrahování souborů do cílové složky
+    with zipfile.ZipFile(zip_file_path, 'r') as zip_ref:
+        zip_ref.extractall(base_path)
 
-    return annotation_address
+    return base_path
 
 
 
 def create_directory(directory_path, delete=False):
     if delete and os.path.exists(directory_path):
         # Remove all files and subdirectories in the specified directory
         for filename in os.listdir(directory_path):
```

### Comparing `prusek_spheroid-3.2/prusek_spheroid/image_processing.py` & `prusek_spheroid-3.3/prusek_spheroid/image_processing.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-3.2/prusek_spheroid/methods.py` & `prusek_spheroid-3.3/prusek_spheroid/methods.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-3.2/prusek_spheroid/selection_dialog.py` & `prusek_spheroid-3.3/prusek_spheroid/selection_dialog.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-3.2/prusek_spheroid.egg-info/PKG-INFO` & `prusek_spheroid-3.3/prusek_spheroid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prusek_spheroid
-Version: 3.2
+Version: 3.3
 Summary: Spheroid segmentation package
 Home-page: https://github.com/michalprusek/prusek-spheroid
 Author: Michal Prusek
 Author-email: prusemic@cvut.cz
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: opencv-python
```

### Comparing `prusek_spheroid-3.2/prusek_spheroid.egg-info/SOURCES.txt` & `prusek_spheroid-3.3/prusek_spheroid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-3.2/setup.py` & `prusek_spheroid-3.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="prusek_spheroid",
-    version="3.2",
+    version="3.3",
     description="Spheroid segmentation package",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Michal Prusek",
     author_email="prusemic@cvut.cz",
     url="https://github.com/michalprusek/prusek-spheroid",
     packages=["prusek_spheroid"],
```

