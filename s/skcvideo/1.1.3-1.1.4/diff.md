# Comparing `tmp/skcvideo-1.1.3.tar.gz` & `tmp/skcvideo-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skcvideo-1.1.3.tar", max compression
+gzip compressed data, was "skcvideo-1.1.4.tar", max compression
```

## Comparing `skcvideo-1.1.3.tar` & `skcvideo-1.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1069 2023-10-06 07:07:06.607681 skcvideo-1.1.3/LICENSE
--rw-r--r--   0        0        0      419 2023-10-06 07:07:06.611681 skcvideo-1.1.3/README.md
--rw-r--r--   0        0        0      965 2023-12-13 16:25:12.700394 skcvideo-1.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-10-06 07:07:06.611681 skcvideo-1.1.3/skcvideo/__init__.py
--rw-r--r--   0        0        0     1261 2023-11-09 14:04:57.354195 skcvideo-1.1.3/skcvideo/button_widget.py
--rw-r--r--   0        0        0      362 2023-10-06 07:07:06.611681 skcvideo-1.1.3/skcvideo/colors.py
--rw-r--r--   0        0        0     5747 2023-11-09 14:05:24.642014 skcvideo-1.1.3/skcvideo/controlled_fps_video_capture.py
--rw-r--r--   0        0        0     7472 2023-11-09 14:04:57.354195 skcvideo-1.1.3/skcvideo/core.py
--rw-r--r--   0        0        0     3697 2023-11-09 14:04:57.354195 skcvideo-1.1.3/skcvideo/field_model.py
--rw-r--r--   0        0        0     3274 2023-11-09 14:04:57.354195 skcvideo-1.1.3/skcvideo/images_list_incrustation.py
--rw-r--r--   0        0        0     2425 2023-11-09 14:04:57.354195 skcvideo-1.1.3/skcvideo/list.py
--rw-r--r--   0        0        0     3765 2023-11-09 14:04:57.354195 skcvideo-1.1.3/skcvideo/minimap.py
--rw-r--r--   0        0        0     6703 2023-11-09 14:04:57.354195 skcvideo-1.1.3/skcvideo/reader.py
--rw-r--r--   0        0        0     3058 2023-11-09 14:04:57.354195 skcvideo-1.1.3/skcvideo/table.py
--rw-r--r--   0        0        0     9046 2023-11-09 14:04:57.354195 skcvideo-1.1.3/skcvideo/timeline.py
--rw-r--r--   0        0        0      896 2023-11-09 14:04:57.354195 skcvideo-1.1.3/skcvideo/utils.py
--rw-r--r--   0        0        0     5708 2023-11-09 14:04:57.354195 skcvideo-1.1.3/skcvideo/video_capture.py
--rw-r--r--   0        0        0     1422 2023-11-09 14:04:57.354195 skcvideo-1.1.3/skcvideo/video_incrustation.py
--rw-r--r--   0        0        0     1120 1970-01-01 00:00:00.000000 skcvideo-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-10-06 07:07:06.607681 skcvideo-1.1.4/LICENSE
+-rw-r--r--   0        0        0      419 2023-10-06 07:07:06.611681 skcvideo-1.1.4/README.md
+-rw-r--r--   0        0        0      965 2024-03-05 11:17:29.066092 skcvideo-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-10-06 07:07:06.611681 skcvideo-1.1.4/skcvideo/__init__.py
+-rw-r--r--   0        0        0     1261 2024-03-05 11:11:13.391051 skcvideo-1.1.4/skcvideo/button_widget.py
+-rw-r--r--   0        0        0      362 2023-10-06 07:07:06.611681 skcvideo-1.1.4/skcvideo/colors.py
+-rw-r--r--   0        0        0     5747 2024-03-05 11:10:33.151157 skcvideo-1.1.4/skcvideo/controlled_fps_video_capture.py
+-rw-r--r--   0        0        0     7472 2024-03-05 11:11:13.391051 skcvideo-1.1.4/skcvideo/core.py
+-rw-r--r--   0        0        0     3697 2024-03-05 11:11:13.391051 skcvideo-1.1.4/skcvideo/field_model.py
+-rw-r--r--   0        0        0     3274 2024-03-05 11:11:13.391051 skcvideo-1.1.4/skcvideo/images_list_incrustation.py
+-rw-r--r--   0        0        0     2425 2024-03-05 11:11:13.391051 skcvideo-1.1.4/skcvideo/list.py
+-rw-r--r--   0        0        0     3765 2024-03-05 11:11:13.391051 skcvideo-1.1.4/skcvideo/minimap.py
+-rw-r--r--   0        0        0     6703 2024-03-05 11:11:13.391051 skcvideo-1.1.4/skcvideo/reader.py
+-rw-r--r--   0        0        0     3058 2024-03-05 11:11:13.391051 skcvideo-1.1.4/skcvideo/table.py
+-rw-r--r--   0        0        0     9046 2024-03-05 11:11:13.391051 skcvideo-1.1.4/skcvideo/timeline.py
+-rw-r--r--   0        0        0      896 2024-03-05 11:11:13.395051 skcvideo-1.1.4/skcvideo/utils.py
+-rw-r--r--   0        0        0     5729 2024-03-05 11:19:04.317855 skcvideo-1.1.4/skcvideo/video_capture.py
+-rw-r--r--   0        0        0     1422 2024-03-05 11:11:13.395051 skcvideo-1.1.4/skcvideo/video_incrustation.py
+-rw-r--r--   0        0        0     1120 1970-01-01 00:00:00.000000 skcvideo-1.1.4/PKG-INFO
```

### Comparing `skcvideo-1.1.3/LICENSE` & `skcvideo-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `skcvideo-1.1.3/pyproject.toml` & `skcvideo-1.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "skcvideo"
-version = "1.1.3"
+version = "1.1.4"
 description = "video utils"
 authors = ["timothe.collet"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.7,<3.11"
```

### Comparing `skcvideo-1.1.3/skcvideo/button_widget.py` & `skcvideo-1.1.4/skcvideo/button_widget.py`

 * *Files identical despite different names*

### Comparing `skcvideo-1.1.3/skcvideo/controlled_fps_video_capture.py` & `skcvideo-1.1.4/skcvideo/controlled_fps_video_capture.py`

 * *Files identical despite different names*

### Comparing `skcvideo-1.1.3/skcvideo/core.py` & `skcvideo-1.1.4/skcvideo/core.py`

 * *Files identical despite different names*

### Comparing `skcvideo-1.1.3/skcvideo/field_model.py` & `skcvideo-1.1.4/skcvideo/field_model.py`

 * *Files identical despite different names*

### Comparing `skcvideo-1.1.3/skcvideo/images_list_incrustation.py` & `skcvideo-1.1.4/skcvideo/images_list_incrustation.py`

 * *Files identical despite different names*

### Comparing `skcvideo-1.1.3/skcvideo/list.py` & `skcvideo-1.1.4/skcvideo/list.py`

 * *Files identical despite different names*

### Comparing `skcvideo-1.1.3/skcvideo/minimap.py` & `skcvideo-1.1.4/skcvideo/minimap.py`

 * *Files identical despite different names*

### Comparing `skcvideo-1.1.3/skcvideo/reader.py` & `skcvideo-1.1.4/skcvideo/reader.py`

 * *Files identical despite different names*

### Comparing `skcvideo-1.1.3/skcvideo/table.py` & `skcvideo-1.1.4/skcvideo/table.py`

 * *Files identical despite different names*

### Comparing `skcvideo-1.1.3/skcvideo/timeline.py` & `skcvideo-1.1.4/skcvideo/timeline.py`

 * *Files identical despite different names*

### Comparing `skcvideo-1.1.3/skcvideo/utils.py` & `skcvideo-1.1.4/skcvideo/utils.py`

 * *Files identical despite different names*

### Comparing `skcvideo-1.1.3/skcvideo/video_capture.py` & `skcvideo-1.1.4/skcvideo/video_capture.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 DEFAULT_HEIGHT = 720
 
 SET_READ_TRADEOFF = 20
 MAX_STORED = 100
 AMONG_FRAMES = 20
 
 
-class TransformedImageVideoCapture(ControlledFPSVideoCapture):
+class TransformedImageVideoCapture:
     """
     This VideoCapture overlay aims to add operations on the images before
     providing them.
 
     For instance, the operations are:
         - change channel order to switch from BGR to RGB
         - resize to desired shape
@@ -36,31 +36,31 @@
 
         if self.min_frame < 0:
             self.min_frame = 0
 
         if self.colormap not in ['rgb', 'bgr']:
             raise NotImplementedError
 
-        super(TransformedImageVideoCapture, self).__init__(*args, **kwargs)
+        self.frame_reader = ControlledFPSVideoCapture(*args, **kwargs)
 
         if self.resize is not None:
             resize_log = 'Resize to {}x{}'.format(self.resize[0], self.resize[1])
         else:
             resize_log = 'No resize'
         colormap_log = 'Colormap: {}'.format(self.colormap)
         print('{}, {}'.format(resize_log, colormap_log))
 
         if self.min_frame > 0:
-            self.set(cv2.CAP_PROP_POS_FRAMES, self.min_frame)
+            self.frame_reader.set(cv2.CAP_PROP_POS_FRAMES, self.min_frame)
 
         # According to our use-case we prefer to have the first frame already read.
         self.read()
 
     def read(self):
-        ret, self.image = super(TransformedImageVideoCapture, self).read()
+        ret, self.image = self.frame_reader.read()
 
         if self.interlaced:
             h, w = self.image.shape[:2]
             self.image = cv2.resize(self.image[::2], (w, h))
 
         self.image_before_resize = self.image
         if self.resize is not None:
@@ -89,19 +89,19 @@
         This method aims to manage the tradoff between directly setting the
         VideoCapture to the desired frame and reading the successive frames
         up to the desired in order to get the frame in the fastest manner.
 
         /!\\ Default value was chosen empirically and may not be optimal
         depending on your architecture.
         """
-        if not (self.output_frame <= frame < self.output_frame + SET_READ_TRADEOFF):
-            self.set(cv2.CAP_PROP_POS_FRAMES, frame)
+        if not (self.frame_reader.output_frame <= frame < self.frame_reader.output_frame + SET_READ_TRADEOFF):
+            self.frame_reader.set(cv2.CAP_PROP_POS_FRAMES, frame)
             self.read()
 
-        while self.output_frame < frame:
+        while self.frame_reader.output_frame < frame:
             self.read()
         return self.image
 
 
 class StoredImagesVideoCapture(TransformedImageVideoCapture):
     """
     This VideoCapture overlay stores previously read frames for faster access.
@@ -120,33 +120,33 @@
     """
 
     def __init__(self, *args, **kwargs):
         self.stored_images = {}
         super(StoredImagesVideoCapture, self).__init__(*args, **kwargs)
 
     def get_max_frame(self):
-        return self.get(cv2.CAP_PROP_FRAME_COUNT)
+        return self.frame_reader.get(cv2.CAP_PROP_FRAME_COUNT)
 
     def read(self):
         """
         Overrides read() method to store the output
         """
         super(StoredImagesVideoCapture, self).read()
-        if self.output_frame - MAX_STORED in self.stored_images:
-            del self.stored_images[self.output_frame - MAX_STORED]
-        self.stored_images[self.output_frame] = self.image
+        if self.frame_reader.output_frame - MAX_STORED in self.stored_images:
+            del self.stored_images[self.frame_reader.output_frame - MAX_STORED]
+        self.stored_images[self.frame_reader.output_frame] = self.image
 
     def set(self, prop_id, value):
         """
         Overrides set() method to erase all the stored values
         """
         if prop_id == cv2.CAP_PROP_POS_FRAMES:
             self.stored_images = {}
-            super(StoredImagesVideoCapture, self).set(prop_id, value - AMONG_FRAMES)
+            self.frame_reader.set(prop_id, value - AMONG_FRAMES)
         else:
-            super(StoredImagesVideoCapture, self).set(prop_id, value)
+            self.frame_reader.set(prop_id, value)
 
     def seek(self, frame):
         if frame not in self.stored_images:
             super(StoredImagesVideoCapture, self).seek(frame)
         self.frame = frame
         return self.stored_images[frame]
```

### Comparing `skcvideo-1.1.3/skcvideo/video_incrustation.py` & `skcvideo-1.1.4/skcvideo/video_incrustation.py`

 * *Files identical despite different names*

### Comparing `skcvideo-1.1.3/PKG-INFO` & `skcvideo-1.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skcvideo
-Version: 1.1.3
+Version: 1.1.4
 Summary: video utils
 License: MIT
 Author: timothe.collet
 Requires-Python: >=3.7,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

