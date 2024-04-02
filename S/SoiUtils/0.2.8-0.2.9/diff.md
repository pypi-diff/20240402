# Comparing `tmp/SoiUtils-0.2.8.tar.gz` & `tmp/SoiUtils-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SoiUtils-0.2.8.tar", last modified: Mon Mar 25 14:48:00 2024, max compression
+gzip compressed data, was "SoiUtils-0.2.9.tar", last modified: Tue Apr  2 06:53:48 2024, max compression
```

## Comparing `SoiUtils-0.2.8.tar` & `SoiUtils-0.2.9.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 xd_skomisarov_gcp_idf_il (343331064) xd_skomisarov_gcp_idf_il (343331064)        0 2024-03-25 14:48:00.838219 SoiUtils-0.2.8/
--rw-r--r--   0 xd_skomisarov_gcp_idf_il (343331064) xd_skomisarov_gcp_idf_il (343331064)    11357 2023-10-24 11:51:10.000000 SoiUtils-0.2.8/LICENSE
--rw-r--r--   0 xd_skomisarov_gcp_idf_il (343331064) xd_skomisarov_gcp_idf_il (343331064)      487 2024-03-25 14:48:00.838219 SoiUtils-0.2.8/PKG-INFO
--rw-r--r--   0 xd_skomisarov_gcp_idf_il (343331064) xd_skomisarov_gcp_idf_il (343331064)      103 2023-10-24 11:51:10.000000 SoiUtils-0.2.8/README.md
-drwxr-xr-x   0 xd_skomisarov_gcp_idf_il (343331064) xd_skomisarov_gcp_idf_il (343331064)        0 2024-03-25 14:48:00.834219 SoiUtils-0.2.8/SoiUtils/
--rw-r--r--   0 xd_skomisarov_gcp_idf_il (343331064) xd_skomisarov_gcp_idf_il (343331064)        0 2023-10-24 13:00:50.000000 SoiUtils-0.2.8/SoiUtils/__init__.py
-drwxr-xr-x   0 xd_skomisarov_gcp_idf_il (343331064) xd_skomisarov_gcp_idf_il (343331064)        0 2024-03-25 14:48:00.834219 SoiUtils-0.2.8/SoiUtils/cloud/
--rw-r--r--   0 xd_skomisarov_gcp_idf_il (343331064) xd_skomisarov_gcp_idf_il (343331064)        0 2023-11-28 08:49:14.000000 SoiUtils-0.2.8/SoiUtils/cloud/__init__.py
--rw-r--r--   0 xd_skomisarov_gcp_idf_il (343331064) xd_skomisarov_gcp_idf_il (343331064)     1355 2024-01-09 19:34:45.000000 SoiUtils-0.2.8/SoiUtils/cloud/storage.py
-drwxr-xr-x   0 xd_skomisarov_gcp_idf_il (343331064) xd_skomisarov_gcp_idf_il (343331064)        0 2024-03-25 14:48:00.838219 SoiUtils-0.2.8/SoiUtils/datasets/
--rw-r--r--   0 xd_skomisarov_gcp_idf_il (343331064) xd_skomisarov_gcp_idf_il (343331064)        0 2023-11-28 08:49:14.000000 SoiUtils-0.2.8/SoiUtils/datasets/__init__.py
--rw-r--r--   0 xd_skomisarov_gcp_idf_il (343331064) xd_skomisarov_gcp_idf_il (343331064)      939 2023-11-28 08:49:14.000000 SoiUtils-0.2.8/SoiUtils/datasets/base.py
--rw-r--r--   0 xd_skomisarov_gcp_idf_il (343331064) xd_skomisarov_gcp_idf_il (343331064)     8659 2024-03-25 14:44:53.000000 SoiUtils-0.2.8/SoiUtils/datasets/datasets.py
--rw-r--r--   0 xd_skomisarov_gcp_idf_il (343331064) xd_skomisarov_gcp_idf_il (343331064)      147 2024-01-24 16:01:58.000000 SoiUtils-0.2.8/SoiUtils/general.py
--rw-r--r--   0 xd_skomisarov_gcp_idf_il (343331064) xd_skomisarov_gcp_idf_il (343331064)     2501 2023-12-26 12:33:29.000000 SoiUtils-0.2.8/SoiUtils/interfaces.py
--rw-r--r--   0 xd_skomisarov_gcp_idf_il (343331064) xd_skomisarov_gcp_idf_il (343331064)      411 2023-10-25 07:39:26.000000 SoiUtils-0.2.8/SoiUtils/load.py
--rw-r--r--   0 xd_skomisarov_gcp_idf_il (343331064) xd_skomisarov_gcp_idf_il (343331064)     1042 2024-01-25 09:13:25.000000 SoiUtils-0.2.8/SoiUtils/output_recorder.py
--rw-r--r--   0 xd_skomisarov_gcp_idf_il (343331064) xd_skomisarov_gcp_idf_il (343331064)     1200 2023-10-31 13:06:42.000000 SoiUtils-0.2.8/SoiUtils/parallelization.py
--rw-r--r--   0 xd_skomisarov_gcp_idf_il (343331064) xd_skomisarov_gcp_idf_il (343331064)     3272 2024-01-08 09:16:42.000000 SoiUtils-0.2.8/SoiUtils/ronen_api.py
--rw-r--r--   0 xd_skomisarov_gcp_idf_il (343331064) xd_skomisarov_gcp_idf_il (343331064)      275 2024-02-28 12:34:48.000000 SoiUtils-0.2.8/SoiUtils/test.py
--rw-r--r--   0 xd_skomisarov_gcp_idf_il (343331064) xd_skomisarov_gcp_idf_il (343331064)     2747 2023-11-02 14:35:45.000000 SoiUtils-0.2.8/SoiUtils/video_manipulations.py
-drwxr-xr-x   0 xd_skomisarov_gcp_idf_il (343331064) xd_skomisarov_gcp_idf_il (343331064)        0 2024-03-25 14:48:00.834219 SoiUtils-0.2.8/SoiUtils.egg-info/
--rw-r--r--   0 xd_skomisarov_gcp_idf_il (343331064) xd_skomisarov_gcp_idf_il (343331064)      487 2024-03-25 14:48:00.000000 SoiUtils-0.2.8/SoiUtils.egg-info/PKG-INFO
--rw-r--r--   0 xd_skomisarov_gcp_idf_il (343331064) xd_skomisarov_gcp_idf_il (343331064)      532 2024-03-25 14:48:00.000000 SoiUtils-0.2.8/SoiUtils.egg-info/SOURCES.txt
--rw-r--r--   0 xd_skomisarov_gcp_idf_il (343331064) xd_skomisarov_gcp_idf_il (343331064)        1 2024-03-25 14:48:00.000000 SoiUtils-0.2.8/SoiUtils.egg-info/dependency_links.txt
--rw-r--r--   0 xd_skomisarov_gcp_idf_il (343331064) xd_skomisarov_gcp_idf_il (343331064)       44 2024-03-25 14:48:00.000000 SoiUtils-0.2.8/SoiUtils.egg-info/requires.txt
--rw-r--r--   0 xd_skomisarov_gcp_idf_il (343331064) xd_skomisarov_gcp_idf_il (343331064)        9 2024-03-25 14:48:00.000000 SoiUtils-0.2.8/SoiUtils.egg-info/top_level.txt
--rw-r--r--   0 xd_skomisarov_gcp_idf_il (343331064) xd_skomisarov_gcp_idf_il (343331064)       38 2024-03-25 14:48:00.838219 SoiUtils-0.2.8/setup.cfg
--rw-r--r--   0 xd_skomisarov_gcp_idf_il (343331064) xd_skomisarov_gcp_idf_il (343331064)      966 2024-03-25 14:45:58.000000 SoiUtils-0.2.8/setup.py
+drwxr-xr-x   0 xd_skomisarov_gcp_idf_il (343331064) xd_skomisarov_gcp_idf_il (343331064)        0 2024-04-02 06:53:48.673187 SoiUtils-0.2.9/
+-rw-r--r--   0 xd_skomisarov_gcp_idf_il (343331064) xd_skomisarov_gcp_idf_il (343331064)    11357 2023-10-24 11:51:10.000000 SoiUtils-0.2.9/LICENSE
+-rw-r--r--   0 xd_skomisarov_gcp_idf_il (343331064) xd_skomisarov_gcp_idf_il (343331064)      487 2024-04-02 06:53:48.673187 SoiUtils-0.2.9/PKG-INFO
+-rw-r--r--   0 xd_skomisarov_gcp_idf_il (343331064) xd_skomisarov_gcp_idf_il (343331064)      103 2023-10-24 11:51:10.000000 SoiUtils-0.2.9/README.md
+drwxr-xr-x   0 xd_skomisarov_gcp_idf_il (343331064) xd_skomisarov_gcp_idf_il (343331064)        0 2024-04-02 06:53:48.669186 SoiUtils-0.2.9/SoiUtils/
+-rw-r--r--   0 xd_skomisarov_gcp_idf_il (343331064) xd_skomisarov_gcp_idf_il (343331064)        0 2023-10-24 13:00:50.000000 SoiUtils-0.2.9/SoiUtils/__init__.py
+drwxr-xr-x   0 xd_skomisarov_gcp_idf_il (343331064) xd_skomisarov_gcp_idf_il (343331064)        0 2024-04-02 06:53:48.669186 SoiUtils-0.2.9/SoiUtils/cloud/
+-rw-r--r--   0 xd_skomisarov_gcp_idf_il (343331064) xd_skomisarov_gcp_idf_il (343331064)        0 2023-11-28 08:49:14.000000 SoiUtils-0.2.9/SoiUtils/cloud/__init__.py
+-rw-r--r--   0 xd_skomisarov_gcp_idf_il (343331064) xd_skomisarov_gcp_idf_il (343331064)     1355 2024-01-09 19:34:45.000000 SoiUtils-0.2.9/SoiUtils/cloud/storage.py
+drwxr-xr-x   0 xd_skomisarov_gcp_idf_il (343331064) xd_skomisarov_gcp_idf_il (343331064)        0 2024-04-02 06:53:48.673187 SoiUtils-0.2.9/SoiUtils/datasets/
+-rw-r--r--   0 xd_skomisarov_gcp_idf_il (343331064) xd_skomisarov_gcp_idf_il (343331064)        0 2023-11-28 08:49:14.000000 SoiUtils-0.2.9/SoiUtils/datasets/__init__.py
+-rw-r--r--   0 xd_skomisarov_gcp_idf_il (343331064) xd_skomisarov_gcp_idf_il (343331064)      939 2023-11-28 08:49:14.000000 SoiUtils-0.2.9/SoiUtils/datasets/base.py
+-rw-r--r--   0 xd_skomisarov_gcp_idf_il (343331064) xd_skomisarov_gcp_idf_il (343331064)     8866 2024-04-02 06:50:55.000000 SoiUtils-0.2.9/SoiUtils/datasets/datasets.py
+-rw-r--r--   0 xd_skomisarov_gcp_idf_il (343331064) xd_skomisarov_gcp_idf_il (343331064)      147 2024-01-24 16:01:58.000000 SoiUtils-0.2.9/SoiUtils/general.py
+-rw-r--r--   0 xd_skomisarov_gcp_idf_il (343331064) xd_skomisarov_gcp_idf_il (343331064)     2501 2023-12-26 12:33:29.000000 SoiUtils-0.2.9/SoiUtils/interfaces.py
+-rw-r--r--   0 xd_skomisarov_gcp_idf_il (343331064) xd_skomisarov_gcp_idf_il (343331064)      411 2023-10-25 07:39:26.000000 SoiUtils-0.2.9/SoiUtils/load.py
+-rw-r--r--   0 xd_skomisarov_gcp_idf_il (343331064) xd_skomisarov_gcp_idf_il (343331064)     1042 2024-01-25 09:13:25.000000 SoiUtils-0.2.9/SoiUtils/output_recorder.py
+-rw-r--r--   0 xd_skomisarov_gcp_idf_il (343331064) xd_skomisarov_gcp_idf_il (343331064)     1200 2023-10-31 13:06:42.000000 SoiUtils-0.2.9/SoiUtils/parallelization.py
+-rw-r--r--   0 xd_skomisarov_gcp_idf_il (343331064) xd_skomisarov_gcp_idf_il (343331064)     3272 2024-01-08 09:16:42.000000 SoiUtils-0.2.9/SoiUtils/ronen_api.py
+-rw-r--r--   0 xd_skomisarov_gcp_idf_il (343331064) xd_skomisarov_gcp_idf_il (343331064)      275 2024-02-28 12:34:48.000000 SoiUtils-0.2.9/SoiUtils/test.py
+-rw-r--r--   0 xd_skomisarov_gcp_idf_il (343331064) xd_skomisarov_gcp_idf_il (343331064)      975 2024-04-02 06:50:55.000000 SoiUtils-0.2.9/SoiUtils/test_script.py
+-rw-r--r--   0 xd_skomisarov_gcp_idf_il (343331064) xd_skomisarov_gcp_idf_il (343331064)     2747 2023-11-02 14:35:45.000000 SoiUtils-0.2.9/SoiUtils/video_manipulations.py
+drwxr-xr-x   0 xd_skomisarov_gcp_idf_il (343331064) xd_skomisarov_gcp_idf_il (343331064)        0 2024-04-02 06:53:48.669186 SoiUtils-0.2.9/SoiUtils.egg-info/
+-rw-r--r--   0 xd_skomisarov_gcp_idf_il (343331064) xd_skomisarov_gcp_idf_il (343331064)      487 2024-04-02 06:53:48.000000 SoiUtils-0.2.9/SoiUtils.egg-info/PKG-INFO
+-rw-r--r--   0 xd_skomisarov_gcp_idf_il (343331064) xd_skomisarov_gcp_idf_il (343331064)      556 2024-04-02 06:53:48.000000 SoiUtils-0.2.9/SoiUtils.egg-info/SOURCES.txt
+-rw-r--r--   0 xd_skomisarov_gcp_idf_il (343331064) xd_skomisarov_gcp_idf_il (343331064)        1 2024-04-02 06:53:48.000000 SoiUtils-0.2.9/SoiUtils.egg-info/dependency_links.txt
+-rw-r--r--   0 xd_skomisarov_gcp_idf_il (343331064) xd_skomisarov_gcp_idf_il (343331064)       44 2024-04-02 06:53:48.000000 SoiUtils-0.2.9/SoiUtils.egg-info/requires.txt
+-rw-r--r--   0 xd_skomisarov_gcp_idf_il (343331064) xd_skomisarov_gcp_idf_il (343331064)        9 2024-04-02 06:53:48.000000 SoiUtils-0.2.9/SoiUtils.egg-info/top_level.txt
+-rw-r--r--   0 xd_skomisarov_gcp_idf_il (343331064) xd_skomisarov_gcp_idf_il (343331064)       38 2024-04-02 06:53:48.673187 SoiUtils-0.2.9/setup.cfg
+-rw-r--r--   0 xd_skomisarov_gcp_idf_il (343331064) xd_skomisarov_gcp_idf_il (343331064)      966 2024-04-02 06:52:16.000000 SoiUtils-0.2.9/setup.py
```

### Comparing `SoiUtils-0.2.8/LICENSE` & `SoiUtils-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `SoiUtils-0.2.8/SoiUtils/cloud/storage.py` & `SoiUtils-0.2.9/SoiUtils/cloud/storage.py`

 * *Files identical despite different names*

### Comparing `SoiUtils-0.2.8/SoiUtils/datasets/base.py` & `SoiUtils-0.2.9/SoiUtils/datasets/base.py`

 * *Files identical despite different names*

### Comparing `SoiUtils-0.2.8/SoiUtils/datasets/datasets.py` & `SoiUtils-0.2.9/SoiUtils/datasets/datasets.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from SoiUtils.datasets.base import ImageDetectionSample,Detection
 from PIL import Image
 import numpy as np
 # import fiftyone as fo
 import warnings
 from typing import Union, List
 import yaml
+import json
 
 
 def collate_fn(batch):
     return tuple(zip(*batch))
 
 #TODO: consider writing a prper fiftyone exporter
 def export_dataset(collection_datasets, export_dir_path, dataset_name, copy_images=False, move_images=False, tags=None):
@@ -96,17 +97,19 @@
                 export_media=export_mode
             )    
 
 class ImageDetectionDataset(Dataset):
     def __init__(self,
                  dataset_root_dir: str, 
                  annotation_file_path: str,
+                 telemetry_file_path: str,
                  origin_bbox_format: str = 'coco',
                  target_bbox_format: str = 'coco',
                  selected_classes: Union[str, List[str]] = 'all',
+                 video_color: str = 'thermal',
                  transforms = None):
         """
         dataset class for our tagged data in the gcp.
 
         Args:
             dataset_root_dir (str): path to the data directory.
             annotation_file_path (str): path to the annotation .json file .
@@ -120,14 +123,15 @@
         super().__init__()
 
         self.origin_bbox_format = origin_bbox_format
         self.target_bbox_format = target_bbox_format
 
         self.dataset_root_dir = Path(dataset_root_dir)
         all_dataset_info = COCO(annotation_file_path)
+        self.frame2telemetry = json.load(open(telemetry_file_path))[video_color]["data"]
         self.images = all_dataset_info.imgs
         self.frames_dir_name = all_dataset_info.dataset['info']['img_dir']
         self.classes = all_dataset_info.cats
         self.imgToAnns = all_dataset_info.imgToAnns
 
         self.selected_classes = selected_classes
         self.class_mapper = self.create_class_mapper()
@@ -154,27 +158,28 @@
 
     
     def get_image_file_path(self, index: int):
         image_id = self.images[index]['id']
         return str(self.dataset_root_dir/self.frames_dir_name/self.images[image_id]['file_name'])
 
     def __getitem__(self, index: int) -> ImageDetectionSample:
+        index = index + 1 # In COCO format the first frame has ID of 1 not 0
         image_file_path = self.get_image_file_path(index)
         image = np.asarray(Image.open(image_file_path).convert('RGB'))
         detections = [Detection.load_generic_mode(bbox=detection_annotation['bbox'], 
                                                   cl=self.class_mapper[detection_annotation['category_id']], 
                                                   from_type=self.origin_bbox_format, 
                                                   to_type=self.target_bbox_format, 
                                                   image_size=image.shape[:2][::-1])
                        
                        for detection_annotation in self.imgToAnns[index]]
 
         image_detection_sample = ImageDetectionSample(image=image, detections=detections)
 
-        telemetry = self.imgToAnns[index][0]['attributes'] if 'attributes' in self.imgToAnns[index][0] else None
+        telemetry = self.frame2telemetry[index - 1]
         
         if self.transforms is not None:
             item = self.transforms(image_detection_sample)
         else:
             item = image_detection_sample
         
         return item.image, [det.__dict__ for det in item.detections], telemetry
```

### Comparing `SoiUtils-0.2.8/SoiUtils/interfaces.py` & `SoiUtils-0.2.9/SoiUtils/interfaces.py`

 * *Files identical despite different names*

### Comparing `SoiUtils-0.2.8/SoiUtils/output_recorder.py` & `SoiUtils-0.2.9/SoiUtils/output_recorder.py`

 * *Files identical despite different names*

### Comparing `SoiUtils-0.2.8/SoiUtils/parallelization.py` & `SoiUtils-0.2.9/SoiUtils/parallelization.py`

 * *Files identical despite different names*

### Comparing `SoiUtils-0.2.8/SoiUtils/ronen_api.py` & `SoiUtils-0.2.9/SoiUtils/ronen_api.py`

 * *Files identical despite different names*

### Comparing `SoiUtils-0.2.8/SoiUtils/video_manipulations.py` & `SoiUtils-0.2.9/SoiUtils/video_manipulations.py`

 * *Files identical despite different names*

### Comparing `SoiUtils-0.2.8/SoiUtils.egg-info/SOURCES.txt` & `SoiUtils-0.2.9/SoiUtils.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 SoiUtils/general.py
 SoiUtils/interfaces.py
 SoiUtils/load.py
 SoiUtils/output_recorder.py
 SoiUtils/parallelization.py
 SoiUtils/ronen_api.py
 SoiUtils/test.py
+SoiUtils/test_script.py
 SoiUtils/video_manipulations.py
 SoiUtils.egg-info/PKG-INFO
 SoiUtils.egg-info/SOURCES.txt
 SoiUtils.egg-info/dependency_links.txt
 SoiUtils.egg-info/requires.txt
 SoiUtils.egg-info/top_level.txt
 SoiUtils/cloud/__init__.py
```

### Comparing `SoiUtils-0.2.8/setup.py` & `SoiUtils-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.2.8' 
+VERSION = '0.2.9' 
 DESCRIPTION = 'A Package that includes utility functions'
 LONG_DESCRIPTION = 'utils package that includes multiple utility functions that are used in different projects'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="SoiUtils",
```

