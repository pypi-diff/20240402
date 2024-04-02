# Comparing `tmp/prusek_spheroid-3.3.tar.gz` & `tmp/prusek_spheroid-3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prusek_spheroid-3.3.tar", last modified: Tue Apr  2 12:13:42 2024, max compression
+gzip compressed data, was "prusek_spheroid-3.4.tar", last modified: Tue Apr  2 12:27:31 2024, max compression
```

## Comparing `prusek_spheroid-3.3.tar` & `prusek_spheroid-3.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-02 12:13:42.377776 prusek_spheroid-3.3/
--rw-r--r--   0 michalprusek   (501) staff       (20)     9069 2024-04-02 12:13:42.377497 prusek_spheroid-3.3/PKG-INFO
--rw-r--r--   0 michalprusek   (501) staff       (20)     8544 2024-03-27 11:29:11.000000 prusek_spheroid-3.3/README.md
-drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-02 12:13:42.376134 prusek_spheroid-3.3/prusek_spheroid/
--rw-r--r--   0 michalprusek   (501) staff       (20)    16442 2024-03-29 08:04:06.000000 prusek_spheroid-3.3/prusek_spheroid/ContoursClassGUI.py
--rw-r--r--   0 michalprusek   (501) staff       (20)    35159 2024-04-02 11:58:27.000000 prusek_spheroid-3.3/prusek_spheroid/GUI.py
--rw-r--r--   0 michalprusek   (501) staff       (20)    12427 2024-03-22 06:33:48.000000 prusek_spheroid-3.3/prusek_spheroid/GradientDescentGUI.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     2370 2024-03-25 13:56:52.000000 prusek_spheroid-3.3/prusek_spheroid/calculate_iou.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     4491 2024-01-27 10:12:42.000000 prusek_spheroid-3.3/prusek_spheroid/characteristic_functions.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     7200 2024-04-02 12:11:35.000000 prusek_spheroid-3.3/prusek_spheroid/file_management.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     3466 2024-04-02 09:37:18.000000 prusek_spheroid-3.3/prusek_spheroid/image_processing.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     3705 2024-04-02 09:37:18.000000 prusek_spheroid-3.3/prusek_spheroid/methods.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     4632 2024-03-27 08:31:17.000000 prusek_spheroid-3.3/prusek_spheroid/selection_dialog.py
-drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-02 12:13:42.377221 prusek_spheroid-3.3/prusek_spheroid.egg-info/
--rw-r--r--   0 michalprusek   (501) staff       (20)     9069 2024-04-02 12:13:42.000000 prusek_spheroid-3.3/prusek_spheroid.egg-info/PKG-INFO
--rw-r--r--   0 michalprusek   (501) staff       (20)      520 2024-04-02 12:13:42.000000 prusek_spheroid-3.3/prusek_spheroid.egg-info/SOURCES.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)        1 2024-04-02 12:13:42.000000 prusek_spheroid-3.3/prusek_spheroid.egg-info/dependency_links.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)      110 2024-04-02 12:13:42.000000 prusek_spheroid-3.3/prusek_spheroid.egg-info/requires.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)       16 2024-04-02 12:13:42.000000 prusek_spheroid-3.3/prusek_spheroid.egg-info/top_level.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)       38 2024-04-02 12:13:42.377824 prusek_spheroid-3.3/setup.cfg
--rw-r--r--   0 michalprusek   (501) staff       (20)      729 2024-04-02 12:13:11.000000 prusek_spheroid-3.3/setup.py
+drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-02 12:27:31.934502 prusek_spheroid-3.4/
+-rw-r--r--   0 michalprusek   (501) staff       (20)     9069 2024-04-02 12:27:31.934225 prusek_spheroid-3.4/PKG-INFO
+-rw-r--r--   0 michalprusek   (501) staff       (20)     8544 2024-03-27 11:29:11.000000 prusek_spheroid-3.4/README.md
+drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-02 12:27:31.932931 prusek_spheroid-3.4/prusek_spheroid/
+-rw-r--r--   0 michalprusek   (501) staff       (20)    16651 2024-04-02 12:25:09.000000 prusek_spheroid-3.4/prusek_spheroid/ContoursClassGUI.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)    35159 2024-04-02 11:58:27.000000 prusek_spheroid-3.4/prusek_spheroid/GUI.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)    12427 2024-03-22 06:33:48.000000 prusek_spheroid-3.4/prusek_spheroid/GradientDescentGUI.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     2370 2024-03-25 13:56:52.000000 prusek_spheroid-3.4/prusek_spheroid/calculate_iou.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     4491 2024-01-27 10:12:42.000000 prusek_spheroid-3.4/prusek_spheroid/characteristic_functions.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     7200 2024-04-02 12:11:35.000000 prusek_spheroid-3.4/prusek_spheroid/file_management.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     3466 2024-04-02 09:37:18.000000 prusek_spheroid-3.4/prusek_spheroid/image_processing.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     3705 2024-04-02 09:37:18.000000 prusek_spheroid-3.4/prusek_spheroid/methods.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     4632 2024-03-27 08:31:17.000000 prusek_spheroid-3.4/prusek_spheroid/selection_dialog.py
+drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-02 12:27:31.933949 prusek_spheroid-3.4/prusek_spheroid.egg-info/
+-rw-r--r--   0 michalprusek   (501) staff       (20)     9069 2024-04-02 12:27:31.000000 prusek_spheroid-3.4/prusek_spheroid.egg-info/PKG-INFO
+-rw-r--r--   0 michalprusek   (501) staff       (20)      520 2024-04-02 12:27:31.000000 prusek_spheroid-3.4/prusek_spheroid.egg-info/SOURCES.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)        1 2024-04-02 12:27:31.000000 prusek_spheroid-3.4/prusek_spheroid.egg-info/dependency_links.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)      110 2024-04-02 12:27:31.000000 prusek_spheroid-3.4/prusek_spheroid.egg-info/requires.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)       16 2024-04-02 12:27:31.000000 prusek_spheroid-3.4/prusek_spheroid.egg-info/top_level.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)       38 2024-04-02 12:27:31.934583 prusek_spheroid-3.4/setup.cfg
+-rw-r--r--   0 michalprusek   (501) staff       (20)      729 2024-04-02 12:27:21.000000 prusek_spheroid-3.4/setup.py
```

### Comparing `prusek_spheroid-3.3/PKG-INFO` & `prusek_spheroid-3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prusek_spheroid
-Version: 3.3
+Version: 3.4
 Summary: Spheroid segmentation package
 Home-page: https://github.com/michalprusek/prusek-spheroid
 Author: Michal Prusek
 Author-email: prusemic@cvut.cz
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: opencv-python
```

### Comparing `prusek_spheroid-3.3/README.md` & `prusek_spheroid-3.4/README.md`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-3.3/prusek_spheroid/ContoursClassGUI.py` & `prusek_spheroid-3.4/prusek_spheroid/ContoursClassGUI.py`

 * *Files 2% similar despite different names*

```diff
@@ -213,43 +213,50 @@
 
         self.plot_lock = Lock()
 
         # for mask, name in zip(self.masks, self.img_names):
         #    cv.imwrite(f"img_print/{name}",mask)
 
     def process_and_compute_iou(self, ref_mask, img, img_name, parameters, save, lock):
-        # Převod tensoru masky a obrázku na numpy pole
+        # Convert the mask tensor and image tensor to numpy arrays
         ref_mask = ref_mask.numpy()
         img = img.numpy()
 
-        # Zpracování obrazu (předpokládá se, že img je ve formátu BGR)
+        # Convert image to grayscale (assuming img is in BGR format)
         img_gray = cv.cvtColor(img, cv.COLOR_BGR2GRAY)
 
-        # Aplikace algoritmu segmentace
+        # Apply the segmentation algorithm
         img_binary, inner_contours_mask = self.apply_segmentation_algorithm(
-            self.algorithm, parameters, img_gray, inner_contours=self.contours_state,
-            detect_corrupted=self.detect_corrupted)
+            self.algorithm, parameters, img_gray, self.contours_state,
+            self.detect_corrupted)
 
-        # Další zpracování a výpočet IoU, TPR, PPV
+        # Further processing and IoU, TPR, PPV computation
         if self.contours_state == "all" or self.contours_state == "select":
             intersection = inner_contours_mask & img_binary
             img_binary = img_binary - intersection
 
         contours, hierarchy = cv.findContours(img_binary, cv.RETR_EXTERNAL, cv.CHAIN_APPROX_NONE)
 
         mask = np.zeros_like(img_binary, dtype=np.uint8)
         if not contours:
+            # If no contours are found, draw a default contour
             contour = np.array([[0, 0]], dtype=np.int32)
             cv.drawContours(mask, [contour], 0, color=255, thickness=-1)
         else:
+            # Draw contours on the mask
             for contour in contours:
                 cv.drawContours(mask, [contour], 0, color=255, thickness=-1)
 
-        iou, tpr, ppv = metric.IoU(self.project, self.algorithm, ref_mask, mask, img_name, save=save,
-                                   lock=lock, address=self.adresa_plots)
+        # Thread-safe operations start here
+        lock.acquire()
+        try:
+            iou, tpr, ppv = metric.IoU(self.project, self.algorithm, ref_mask, mask, img_name, save=save,
+                                       lock=lock, address=self.adresa_plots)
+        finally:
+            lock.release()
 
         return iou, tpr, ppv
 
     def run(self, batch, parameters, save_txt):
         IoUbuffer = []
         ratesBuffer = []
```

### Comparing `prusek_spheroid-3.3/prusek_spheroid/GUI.py` & `prusek_spheroid-3.4/prusek_spheroid/GUI.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-3.3/prusek_spheroid/GradientDescentGUI.py` & `prusek_spheroid-3.4/prusek_spheroid/GradientDescentGUI.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-3.3/prusek_spheroid/calculate_iou.py` & `prusek_spheroid-3.4/prusek_spheroid/calculate_iou.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-3.3/prusek_spheroid/characteristic_functions.py` & `prusek_spheroid-3.4/prusek_spheroid/characteristic_functions.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-3.3/prusek_spheroid/file_management.py` & `prusek_spheroid-3.4/prusek_spheroid/file_management.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-3.3/prusek_spheroid/image_processing.py` & `prusek_spheroid-3.4/prusek_spheroid/image_processing.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-3.3/prusek_spheroid/methods.py` & `prusek_spheroid-3.4/prusek_spheroid/methods.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-3.3/prusek_spheroid/selection_dialog.py` & `prusek_spheroid-3.4/prusek_spheroid/selection_dialog.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-3.3/prusek_spheroid.egg-info/PKG-INFO` & `prusek_spheroid-3.4/prusek_spheroid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prusek_spheroid
-Version: 3.3
+Version: 3.4
 Summary: Spheroid segmentation package
 Home-page: https://github.com/michalprusek/prusek-spheroid
 Author: Michal Prusek
 Author-email: prusemic@cvut.cz
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: opencv-python
```

### Comparing `prusek_spheroid-3.3/prusek_spheroid.egg-info/SOURCES.txt` & `prusek_spheroid-3.4/prusek_spheroid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-3.3/setup.py` & `prusek_spheroid-3.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="prusek_spheroid",
-    version="3.3",
+    version="3.4",
     description="Spheroid segmentation package",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Michal Prusek",
     author_email="prusemic@cvut.cz",
     url="https://github.com/michalprusek/prusek-spheroid",
     packages=["prusek_spheroid"],
```

