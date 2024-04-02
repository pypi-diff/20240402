# Comparing `tmp/napari-segment-everything-0.1.0.tar.gz` & `tmp/napari-segment-everything-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-segment-everything-0.1.0.tar", last modified: Mon Apr  1 12:02:00 2024, max compression
+gzip compressed data, was "napari-segment-everything-0.1.1.tar", last modified: Tue Apr  2 13:51:52 2024, max compression
```

## Comparing `napari-segment-everything-0.1.0.tar` & `napari-segment-everything-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 bnorthan  (1000) bnorthan  (1000)        0 2024-04-01 12:02:00.772370 napari-segment-everything-0.1.0/
--rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)     1488 2024-04-01 09:06:08.000000 napari-segment-everything-0.1.0/LICENSE
--rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)       96 2024-04-01 09:06:08.000000 napari-segment-everything-0.1.0/MANIFEST.in
--rw-r--r--   0 bnorthan  (1000) bnorthan  (1000)     4244 2024-04-01 12:02:00.772370 napari-segment-everything-0.1.0/PKG-INFO
--rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)     2776 2024-04-01 09:06:08.000000 napari-segment-everything-0.1.0/README.md
--rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)     1185 2024-04-01 09:06:08.000000 napari-segment-everything-0.1.0/pyproject.toml
--rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)     1549 2024-04-01 12:02:00.772370 napari-segment-everything-0.1.0/setup.cfg
-drwxrwxr-x   0 bnorthan  (1000) bnorthan  (1000)        0 2024-04-01 12:02:00.772370 napari-segment-everything-0.1.0/src/
-drwxrwxr-x   0 bnorthan  (1000) bnorthan  (1000)        0 2024-04-01 12:02:00.772370 napari-segment-everything-0.1.0/src/napari_segment_everything/
--rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)        0 2024-04-01 09:06:08.000000 napari-segment-everything-0.1.0/src/napari_segment_everything/__init__.py
-drwxrwxr-x   0 bnorthan  (1000) bnorthan  (1000)        0 2024-04-01 12:02:00.772370 napari-segment-everything-0.1.0/src/napari_segment_everything/_tests/
--rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)        0 2024-04-01 09:06:08.000000 napari-segment-everything-0.1.0/src/napari_segment_everything/_tests/__init__.py
--rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)       67 2024-04-01 09:06:08.000000 napari-segment-everything-0.1.0/src/napari_segment_everything/_tests/test_widget.py
--rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)      214 2024-04-01 09:06:08.000000 napari-segment-everything-0.1.0/src/napari_segment_everything/interactive_launch.py
--rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)      411 2024-04-01 09:06:08.000000 napari-segment-everything-0.1.0/src/napari_segment_everything/napari.yaml
--rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)     6850 2024-04-01 10:18:06.000000 napari-segment-everything-0.1.0/src/napari_segment_everything/sam_helper.py
--rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)    16066 2024-04-01 10:25:18.000000 napari-segment-everything-0.1.0/src/napari_segment_everything/segment_everything.py
--rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)     7539 2024-04-01 09:06:08.000000 napari-segment-everything-0.1.0/src/napari_segment_everything/widgets.py
-drwxrwxr-x   0 bnorthan  (1000) bnorthan  (1000)        0 2024-04-01 12:02:00.772370 napari-segment-everything-0.1.0/src/napari_segment_everything.egg-info/
--rw-r--r--   0 bnorthan  (1000) bnorthan  (1000)     4244 2024-04-01 12:02:00.000000 napari-segment-everything-0.1.0/src/napari_segment_everything.egg-info/PKG-INFO
--rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)      748 2024-04-01 12:02:00.000000 napari-segment-everything-0.1.0/src/napari_segment_everything.egg-info/SOURCES.txt
--rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)        1 2024-04-01 12:02:00.000000 napari-segment-everything-0.1.0/src/napari_segment_everything.egg-info/dependency_links.txt
--rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)       84 2024-04-01 12:02:00.000000 napari-segment-everything-0.1.0/src/napari_segment_everything.egg-info/entry_points.txt
--rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)      131 2024-04-01 12:02:00.000000 napari-segment-everything-0.1.0/src/napari_segment_everything.egg-info/requires.txt
--rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)       26 2024-04-01 12:02:00.000000 napari-segment-everything-0.1.0/src/napari_segment_everything.egg-info/top_level.txt
+drwxrwxr-x   0 bnorthan  (1000) bnorthan  (1000)        0 2024-04-02 13:51:52.050761 napari-segment-everything-0.1.1/
+-rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)     1488 2024-04-01 09:06:08.000000 napari-segment-everything-0.1.1/LICENSE
+-rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)       96 2024-04-01 09:06:08.000000 napari-segment-everything-0.1.1/MANIFEST.in
+-rw-r--r--   0 bnorthan  (1000) bnorthan  (1000)     4244 2024-04-02 13:51:52.046761 napari-segment-everything-0.1.1/PKG-INFO
+-rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)     2776 2024-04-01 09:06:08.000000 napari-segment-everything-0.1.1/README.md
+-rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)     1185 2024-04-01 09:06:08.000000 napari-segment-everything-0.1.1/pyproject.toml
+-rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)     1549 2024-04-02 13:51:52.050761 napari-segment-everything-0.1.1/setup.cfg
+drwxrwxr-x   0 bnorthan  (1000) bnorthan  (1000)        0 2024-04-02 13:51:52.046761 napari-segment-everything-0.1.1/src/
+drwxrwxr-x   0 bnorthan  (1000) bnorthan  (1000)        0 2024-04-02 13:51:52.046761 napari-segment-everything-0.1.1/src/napari_segment_everything/
+-rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)        0 2024-04-01 09:06:08.000000 napari-segment-everything-0.1.1/src/napari_segment_everything/__init__.py
+drwxrwxr-x   0 bnorthan  (1000) bnorthan  (1000)        0 2024-04-02 13:51:52.046761 napari-segment-everything-0.1.1/src/napari_segment_everything/_tests/
+-rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)        0 2024-04-01 09:06:08.000000 napari-segment-everything-0.1.1/src/napari_segment_everything/_tests/__init__.py
+-rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)       67 2024-04-01 09:06:08.000000 napari-segment-everything-0.1.1/src/napari_segment_everything/_tests/test_widget.py
+-rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)      214 2024-04-01 09:06:08.000000 napari-segment-everything-0.1.1/src/napari_segment_everything/interactive_launch.py
+-rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)      411 2024-04-01 09:06:08.000000 napari-segment-everything-0.1.1/src/napari_segment_everything/napari.yaml
+-rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)     6570 2024-04-02 12:43:49.000000 napari-segment-everything-0.1.1/src/napari_segment_everything/sam_helper.py
+-rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)    16181 2024-04-02 13:38:14.000000 napari-segment-everything-0.1.1/src/napari_segment_everything/segment_everything.py
+-rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)     7539 2024-04-01 09:06:08.000000 napari-segment-everything-0.1.1/src/napari_segment_everything/widgets.py
+drwxrwxr-x   0 bnorthan  (1000) bnorthan  (1000)        0 2024-04-02 13:51:52.046761 napari-segment-everything-0.1.1/src/napari_segment_everything.egg-info/
+-rw-r--r--   0 bnorthan  (1000) bnorthan  (1000)     4244 2024-04-02 13:51:52.000000 napari-segment-everything-0.1.1/src/napari_segment_everything.egg-info/PKG-INFO
+-rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)      748 2024-04-02 13:51:52.000000 napari-segment-everything-0.1.1/src/napari_segment_everything.egg-info/SOURCES.txt
+-rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)        1 2024-04-02 13:51:52.000000 napari-segment-everything-0.1.1/src/napari_segment_everything.egg-info/dependency_links.txt
+-rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)       84 2024-04-02 13:51:52.000000 napari-segment-everything-0.1.1/src/napari_segment_everything.egg-info/entry_points.txt
+-rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)      131 2024-04-02 13:51:52.000000 napari-segment-everything-0.1.1/src/napari_segment_everything.egg-info/requires.txt
+-rw-rw-r--   0 bnorthan  (1000) bnorthan  (1000)       26 2024-04-02 13:51:52.000000 napari-segment-everything-0.1.1/src/napari_segment_everything.egg-info/top_level.txt
```

### Comparing `napari-segment-everything-0.1.0/LICENSE` & `napari-segment-everything-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-segment-everything-0.1.0/PKG-INFO` & `napari-segment-everything-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-segment-everything
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Napari SAM plugin to segment everything in your image (not just some things)
 Home-page: https://github.com/True-North-Intelligent-Algorithms/napari-segment-everything
 Author: Brian Northan
 Author-email: bnorthan@gmail.com
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: napari
```

### Comparing `napari-segment-everything-0.1.0/README.md` & `napari-segment-everything-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `napari-segment-everything-0.1.0/pyproject.toml` & `napari-segment-everything-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `napari-segment-everything-0.1.0/setup.cfg` & `napari-segment-everything-0.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = napari-segment-everything
-version = 0.1.0
+version = 0.1.1
 description = A Napari SAM plugin to segment everything in your image (not just some things)
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/True-North-Intelligent-Algorithms/napari-segment-everything
 author = Brian Northan
 author_email = bnorthan@gmail.com
 license = BSD-3-Clause
```

### Comparing `napari-segment-everything-0.1.0/src/napari_segment_everything/sam_helper.py` & `napari-segment-everything-0.1.1/src/napari_segment_everything/sam_helper.py`

 * *Files 9% similar despite different names*

```diff
@@ -84,43 +84,41 @@
 def get_sam_predictor(model_type: str):
     sam = sam_model_registry[model_type](get_weights_path(model_type))
     #sam.to(self._device)
     return SamPredictor(sam)
 
 def get_sam_automatic_mask_generator(model_type: str, points_per_side=32, pred_iou_thresh=0.1, stability_score_thresh=0.1, box_nms_thresh=0.5):
     sam = sam_model_registry[model_type](get_weights_path(model_type))
-
     sam_anything_predictor = SamAutomaticMaskGenerator(sam,
         points_per_side=int(points_per_side),
-        #points_per_batch=int(self.le_points_per_batch.text()),
+        #points_per_batch=64,
         pred_iou_thresh=pred_iou_thresh,
         stability_score_thresh=stability_score_thresh,
-        #stability_score_offset=float(self.le_stability_score_offset.text()),
+        #stability_score_offset=1.0
         box_nms_thresh=box_nms_thresh,
-        #crop_n_layers=int(self.le_crop_n_layers.text()),
-        #crop_nms_thresh=float(self.le_crop_nms_thresh.text()),
-        #crop_overlap_ratio=float(self.le_crop_overlap_ratio.text()),
-        #crop_n_points_downscale_factor=int(self.le_crop_n_points_downscale_factor.text()),
-        #min_mask_region_area=int(self.le_min_mask_region_area.text()),
+        #crop_n_layers=1,
+        #crop_nms_thresh=0.7,
+        #crop_overlap_ratio: float = 512 / 1500,
+        #crop_n_points_downscale_factor=1,
+        #in_mask_region_area=0,
+        #point_grids: Optional[List[np.ndarray]] = None,
         )
     #sam.to(self._device)
     return sam_anything_predictor
 
 import numpy as np
 
 def make_label_image_3d(masks):
     '''
     Creates a label image by adding one mask at a time onto an empty image
     '''
     num_masks = len(masks)
     label_image = np.zeros( (num_masks, masks[0]['segmentation'].shape[0], masks[0]['segmentation'].shape[1]), dtype='uint16')
 
-    sorted_masks = sorted(masks, key=lambda x: x['area'], reverse=True)
-    
-    for enum, mask in enumerate(sorted_masks):
+    for enum, mask in enumerate(masks):
         mnarray = mask['segmentation']
         label_image[enum,:,:] = mnarray.astype('uint16') * (enum+1)
 
     return label_image
 
 def filter_labels_3d_multi(label_image, sorted_results, stats, mins, maxes, napari_label=None): 
     for enum, result in enumerate(sorted_results):
```

### Comparing `napari-segment-everything-0.1.0/src/napari_segment_everything/segment_everything.py` & `napari-segment-everything-0.1.1/src/napari_segment_everything/segment_everything.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,15 +143,15 @@
         self.make_2d_labels_layout = QVBoxLayout()
         self.make_2d_labels_groups.setLayout(self.make_2d_labels_layout)
         
         # add 2d labels options
         self.labels_options_layout = QHBoxLayout()
         self.labels_options_label = QLabel("2D Labels Options")
         self.labels_options_combo = QComboBox()
-        self.labels_options_combo.addItems(["Big in front", "Small in front"])
+        self.labels_options_combo.addItems(["Small in front", "Big in front"])
         self.labels_options_layout.addWidget(self.labels_options_label)
         self.labels_options_layout.addWidget(self.labels_options_combo)
         
         # add make 2d labels button
         self.make_2d_labels_button = QPushButton("Make 2D Labels")
         self.make_2d_labels_button.clicked.connect(self.make_2d_labels)
 
@@ -201,15 +201,15 @@
         pred_iou_thresh = self.pred_iou_thresh_spinner.spinner.value()
         stability_score_thresh = self.stability_score_thresh_spinner.spinner.value()
         box_nms_thresh = self.box_nms_thresh_spinner.spinner.value()
         
         self._predictor = get_sam_automatic_mask_generator("vit_b", points_per_side=points_per_side, pred_iou_thresh=pred_iou_thresh, stability_score_thresh=stability_score_thresh, box_nms_thresh=box_nms_thresh)
         
         self.results = self._predictor.generate(self.image)
-        self.results = sorted(self.results, key=lambda x: x['area'], reverse=True)
+        self.results = sorted(self.results, key=lambda x: x['area'], reverse=False)
 
         print(len(self.results), 'objects found')
         label_num=1
         for result in self.results:
             result['keep'] = True
             result['label_num'] = label_num
             label_num += 1
@@ -223,27 +223,32 @@
         self._3D_labels_layer.data = label_image
         
         self.block_stats = True
         self.min_max_label_num_slider.max_spinbox.setRange(0, label_num)
         self.min_max_label_num_slider.max_slider.setRange(0, label_num)
         self.block_stats = False
 
+        self.viewer.dims.ndisplay = 3
+
     def update_slider_min_max(self):
 
         stats = ['area', 'label_num', 'solidity', 'circularity', 'mean_intensity', '10th_percentile_intensity', 'mean_hue', 'mean_saturation', 'predicted_iou', 'stability_score']
         for stat in stats:
             min_ = min([result[stat] for result in self.results])
             max_ = max([result[stat] for result in self.results])
 
             print(stat, min_, max_)
         
     def change_stat(self, stat, min_value, max_value):
         if (self.block_stats == True):
             return
         
+        if (self.viewer.dims.ndisplay != 3):
+            return
+        
         if (self.results is None):
             return
         
         # max of predicted_iou stat
         min_iou = min([result['predicted_iou'] for result in self.results])
         max_iou = max([result['predicted_iou'] for result in self.results])
 
@@ -293,15 +298,15 @@
             p10_intensity_max = max(p10_intensity_max, result['10th_percentile_intensity'])
 
     def make_2d_labels(self):
         min_max = self.labels_options_combo.currentText()
         
         label_image = self._3D_labels_layer.data
         
-        if min_max == "Big in front":
+        if min_max == "Small in front":
              # Create a masked array where zeros are masked
             masked_label_image = np.ma.masked_equal(label_image, 0)
             # Perform the min projection on the masked array
             labels = np.ma.min(masked_label_image, axis=0).filled(0)
         else:
             labels = np.max(label_image, axis=0)
         self.viewer.add_labels(labels, name="2D labels")
```

### Comparing `napari-segment-everything-0.1.0/src/napari_segment_everything/widgets.py` & `napari-segment-everything-0.1.1/src/napari_segment_everything/widgets.py`

 * *Files identical despite different names*

### Comparing `napari-segment-everything-0.1.0/src/napari_segment_everything.egg-info/PKG-INFO` & `napari-segment-everything-0.1.1/src/napari_segment_everything.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-segment-everything
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Napari SAM plugin to segment everything in your image (not just some things)
 Home-page: https://github.com/True-North-Intelligent-Algorithms/napari-segment-everything
 Author: Brian Northan
 Author-email: bnorthan@gmail.com
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: napari
```

### Comparing `napari-segment-everything-0.1.0/src/napari_segment_everything.egg-info/SOURCES.txt` & `napari-segment-everything-0.1.1/src/napari_segment_everything.egg-info/SOURCES.txt`

 * *Files identical despite different names*

