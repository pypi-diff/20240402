# Comparing `tmp/prusek_spheroid-3.1.tar.gz` & `tmp/prusek_spheroid-3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prusek_spheroid-3.1.tar", last modified: Sat Mar 30 15:27:19 2024, max compression
+gzip compressed data, was "prusek_spheroid-3.2.tar", last modified: Tue Apr  2 12:01:24 2024, max compression
```

## Comparing `prusek_spheroid-3.1.tar` & `prusek_spheroid-3.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-03-30 15:27:19.327958 prusek_spheroid-3.1/
--rw-r--r--   0 michalprusek   (501) staff       (20)     9069 2024-03-30 15:27:19.327710 prusek_spheroid-3.1/PKG-INFO
--rw-r--r--   0 michalprusek   (501) staff       (20)     8544 2024-03-27 11:29:11.000000 prusek_spheroid-3.1/README.md
-drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-03-30 15:27:19.326649 prusek_spheroid-3.1/prusek_spheroid/
--rw-r--r--   0 michalprusek   (501) staff       (20)    16442 2024-03-29 08:04:06.000000 prusek_spheroid-3.1/prusek_spheroid/ContoursClassGUI.py
--rw-r--r--   0 michalprusek   (501) staff       (20)    35463 2024-03-30 15:25:43.000000 prusek_spheroid-3.1/prusek_spheroid/GUI.py
--rw-r--r--   0 michalprusek   (501) staff       (20)    12427 2024-03-22 06:33:48.000000 prusek_spheroid-3.1/prusek_spheroid/GradientDescentGUI.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     2370 2024-03-25 13:56:52.000000 prusek_spheroid-3.1/prusek_spheroid/calculate_iou.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     4491 2024-01-27 10:12:42.000000 prusek_spheroid-3.1/prusek_spheroid/characteristic_functions.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     6703 2024-03-30 14:40:26.000000 prusek_spheroid-3.1/prusek_spheroid/file_management.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     3467 2024-03-25 13:54:08.000000 prusek_spheroid-3.1/prusek_spheroid/image_processing.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     3686 2024-03-27 08:39:08.000000 prusek_spheroid-3.1/prusek_spheroid/methods.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     4632 2024-03-27 08:31:17.000000 prusek_spheroid-3.1/prusek_spheroid/selection_dialog.py
-drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-03-30 15:27:19.327494 prusek_spheroid-3.1/prusek_spheroid.egg-info/
--rw-r--r--   0 michalprusek   (501) staff       (20)     9069 2024-03-30 15:27:19.000000 prusek_spheroid-3.1/prusek_spheroid.egg-info/PKG-INFO
--rw-r--r--   0 michalprusek   (501) staff       (20)      520 2024-03-30 15:27:19.000000 prusek_spheroid-3.1/prusek_spheroid.egg-info/SOURCES.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)        1 2024-03-30 15:27:19.000000 prusek_spheroid-3.1/prusek_spheroid.egg-info/dependency_links.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)      110 2024-03-30 15:27:19.000000 prusek_spheroid-3.1/prusek_spheroid.egg-info/requires.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)       16 2024-03-30 15:27:19.000000 prusek_spheroid-3.1/prusek_spheroid.egg-info/top_level.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)       38 2024-03-30 15:27:19.328002 prusek_spheroid-3.1/setup.cfg
--rw-r--r--   0 michalprusek   (501) staff       (20)      729 2024-03-30 15:27:10.000000 prusek_spheroid-3.1/setup.py
+drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-02 12:01:24.787548 prusek_spheroid-3.2/
+-rw-r--r--   0 michalprusek   (501) staff       (20)     9069 2024-04-02 12:01:24.787350 prusek_spheroid-3.2/PKG-INFO
+-rw-r--r--   0 michalprusek   (501) staff       (20)     8544 2024-03-27 11:29:11.000000 prusek_spheroid-3.2/README.md
+drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-02 12:01:24.786146 prusek_spheroid-3.2/prusek_spheroid/
+-rw-r--r--   0 michalprusek   (501) staff       (20)    16442 2024-03-29 08:04:06.000000 prusek_spheroid-3.2/prusek_spheroid/ContoursClassGUI.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)    35159 2024-04-02 11:58:27.000000 prusek_spheroid-3.2/prusek_spheroid/GUI.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)    12427 2024-03-22 06:33:48.000000 prusek_spheroid-3.2/prusek_spheroid/GradientDescentGUI.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     2370 2024-03-25 13:56:52.000000 prusek_spheroid-3.2/prusek_spheroid/calculate_iou.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     4491 2024-01-27 10:12:42.000000 prusek_spheroid-3.2/prusek_spheroid/characteristic_functions.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     7059 2024-04-02 11:58:27.000000 prusek_spheroid-3.2/prusek_spheroid/file_management.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     3466 2024-04-02 09:37:18.000000 prusek_spheroid-3.2/prusek_spheroid/image_processing.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     3705 2024-04-02 09:37:18.000000 prusek_spheroid-3.2/prusek_spheroid/methods.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     4632 2024-03-27 08:31:17.000000 prusek_spheroid-3.2/prusek_spheroid/selection_dialog.py
+drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-02 12:01:24.787142 prusek_spheroid-3.2/prusek_spheroid.egg-info/
+-rw-r--r--   0 michalprusek   (501) staff       (20)     9069 2024-04-02 12:01:24.000000 prusek_spheroid-3.2/prusek_spheroid.egg-info/PKG-INFO
+-rw-r--r--   0 michalprusek   (501) staff       (20)      520 2024-04-02 12:01:24.000000 prusek_spheroid-3.2/prusek_spheroid.egg-info/SOURCES.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)        1 2024-04-02 12:01:24.000000 prusek_spheroid-3.2/prusek_spheroid.egg-info/dependency_links.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)      110 2024-04-02 12:01:24.000000 prusek_spheroid-3.2/prusek_spheroid.egg-info/requires.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)       16 2024-04-02 12:01:24.000000 prusek_spheroid-3.2/prusek_spheroid.egg-info/top_level.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)       38 2024-04-02 12:01:24.787596 prusek_spheroid-3.2/setup.cfg
+-rw-r--r--   0 michalprusek   (501) staff       (20)      729 2024-04-02 12:01:03.000000 prusek_spheroid-3.2/setup.py
```

### Comparing `prusek_spheroid-3.1/PKG-INFO` & `prusek_spheroid-3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prusek_spheroid
-Version: 3.1
+Version: 3.2
 Summary: Spheroid segmentation package
 Home-page: https://github.com/michalprusek/prusek-spheroid
 Author: Michal Prusek
 Author-email: prusemic@cvut.cz
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: opencv-python
```

### Comparing `prusek_spheroid-3.1/README.md` & `prusek_spheroid-3.2/README.md`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-3.1/prusek_spheroid/ContoursClassGUI.py` & `prusek_spheroid-3.2/prusek_spheroid/ContoursClassGUI.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-3.1/prusek_spheroid/GUI.py` & `prusek_spheroid-3.2/prusek_spheroid/GUI.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,32 +44,21 @@
 
 
 def open_quantification_gui(dialog, root):
     dialog.destroy()
     root.deiconify()
     app = SpheroidQuantificationGUI(root)
 
-
 def update_addresses(annotationsAddress):
     annotation_address = os.path.join(annotationsAddress, "annotations")
     images_address = os.path.join(annotationsAddress, "images")
 
     return annotation_address, images_address
 
 
-def unzip(zip_file_path, extract_path):
-    with zipfile.ZipFile(zip_file_path, 'r') as zip_ref:
-        zip_ref.extractall(extract_path)
-
-    # Assuming the content is directly in the extracted folder
-    extracted_folder = extract_path
-
-    return extracted_folder
-
-
 class ProcessingProgressWindow(tk.Toplevel):
     def __init__(self, master):
         tk.Toplevel.__init__(self, master)
         self.title("Processing Progress")
 
         self.geometry("500x250")
         self.resizable(width=False, height=False)
@@ -692,15 +681,15 @@
         if self.loaded_parameters is None and not any(var.get() == 1 for _, var in self.methods_checkboxes):
             messagebox.showerror("Error", "At least one of the four segmentation methods must be selected.")
             return
 
         if self.loaded_parameters is None:
             if current_tab == self.coco_tab:
                 annotation_address = self.coco_annotation_path.get()
-                annotation_address = unzip(annotation_address, os.path.dirname(annotation_address))
+                annotation_address = fm.unzip(annotation_address)
                 annotations_address, images_address = update_addresses(annotation_address)
                 annotation_data = fm.load_annotations(
                     os.path.join(annotations_address, 'instances_default.json'), images_address)
                 print(f"Loaded {len(annotation_data)} annotated images")
             elif current_tab == self.mask_tab:
                 mask_adress = self.masks_annotation_path.get()
                 images_address = self.image_dataset_path.get()
```

### Comparing `prusek_spheroid-3.1/prusek_spheroid/GradientDescentGUI.py` & `prusek_spheroid-3.2/prusek_spheroid/GradientDescentGUI.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-3.1/prusek_spheroid/calculate_iou.py` & `prusek_spheroid-3.2/prusek_spheroid/calculate_iou.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-3.1/prusek_spheroid/characteristic_functions.py` & `prusek_spheroid-3.2/prusek_spheroid/characteristic_functions.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-3.1/prusek_spheroid/file_management.py` & `prusek_spheroid-3.2/prusek_spheroid/file_management.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,30 @@
 import zipfile
 import cv2 as cv
 import numpy as np
 import json as js
 from tkinter import messagebox
 
 
+import zipfile
+import os
+
+def unzip(zip_file_path):
+    # Získá cestu ke složce, kde se nachází zip soubor
+    extract_path = os.path.dirname(zip_file_path)
+
+    with zipfile.ZipFile(zip_file_path, 'r') as zip_ref:
+        zip_ref.extractall(extract_path)
+
+    annotation_address, _ = os.path.splitext(zip_file_path)
+
+    return annotation_address
+
+
+
 def create_directory(directory_path, delete=False):
     if delete and os.path.exists(directory_path):
         # Remove all files and subdirectories in the specified directory
         for filename in os.listdir(directory_path):
             file_path = os.path.join(directory_path, filename)
             try:
                 if os.path.isfile(file_path) or os.path.islink(file_path):
```

### Comparing `prusek_spheroid-3.1/prusek_spheroid/image_processing.py` & `prusek_spheroid-3.2/prusek_spheroid/image_processing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import numpy as np
 import cv2 as cv
 from skimage import img_as_ubyte
 from skimage import feature
 
-
 def find_intersection(img_binary, filtered_contours, contours, hierarchy, edges, inner_contours):
     result_mask = np.zeros_like(img_binary, dtype=np.uint8)
 
     for contour in filtered_contours:
         filled_contour = cv.fillPoly(np.zeros_like(img_binary), [contour], 1)
 
         intersection = filled_contour & edges
```

### Comparing `prusek_spheroid-3.1/prusek_spheroid/methods.py` & `prusek_spheroid-3.2/prusek_spheroid/methods.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import sys
 from prusek_spheroid import image_processing as ip
 from skimage.filters import threshold_sauvola, threshold_niblack
 import cv2 as cv
+import numpy as np
 
 
 class BaseImageProcessing:
     def apply_segmentation_algorithm(self, algorithm, parameters, img, inner_contours,
                                      detect_corrupted):
         if algorithm == "Sauvola":
             return self.sauvola(parameters, img, inner_contours, detect_corrupted)
```

### Comparing `prusek_spheroid-3.1/prusek_spheroid/selection_dialog.py` & `prusek_spheroid-3.2/prusek_spheroid/selection_dialog.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-3.1/prusek_spheroid.egg-info/PKG-INFO` & `prusek_spheroid-3.2/prusek_spheroid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prusek_spheroid
-Version: 3.1
+Version: 3.2
 Summary: Spheroid segmentation package
 Home-page: https://github.com/michalprusek/prusek-spheroid
 Author: Michal Prusek
 Author-email: prusemic@cvut.cz
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: opencv-python
```

### Comparing `prusek_spheroid-3.1/prusek_spheroid.egg-info/SOURCES.txt` & `prusek_spheroid-3.2/prusek_spheroid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-3.1/setup.py` & `prusek_spheroid-3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="prusek_spheroid",
-    version="3.1",
+    version="3.2",
     description="Spheroid segmentation package",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Michal Prusek",
     author_email="prusemic@cvut.cz",
     url="https://github.com/michalprusek/prusek-spheroid",
     packages=["prusek_spheroid"],
```

