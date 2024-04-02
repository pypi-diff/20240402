# Comparing `tmp/jhammer-3.1.1.tar.gz` & `tmp/jhammer-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jhammer-3.1.1.tar", last modified: Sat Mar 30 04:38:46 2024, max compression
+gzip compressed data, was "jhammer-3.1.2.tar", last modified: Tue Apr  2 02:39:57 2024, max compression
```

## Comparing `jhammer-3.1.1.tar` & `jhammer-3.1.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 daijian    (501) staff       (20)        0 2024-03-30 04:38:46.861738 jhammer-3.1.1/
--rw-r--r--   0 daijian    (501) staff       (20)    35149 2022-01-18 06:32:18.000000 jhammer-3.1.1/LICENSE
--rw-r--r--   0 daijian    (501) staff       (20)      686 2024-03-30 04:38:46.860462 jhammer-3.1.1/PKG-INFO
--rw-r--r--   0 daijian    (501) staff       (20)        8 2022-01-18 06:32:18.000000 jhammer-3.1.1/README.md
-drwxr-xr-x   0 daijian    (501) staff       (20)        0 2024-03-30 04:38:46.821781 jhammer-3.1.1/jhammer/
--rw-r--r--   0 daijian    (501) staff       (20)        0 2022-08-11 06:59:33.000000 jhammer-3.1.1/jhammer/__init__.py
--rw-r--r--   0 daijian    (501) staff       (20)     1726 2024-03-20 01:43:38.000000 jhammer-3.1.1/jhammer/checkpoint.py
--rw-r--r--   0 daijian    (501) staff       (20)     2706 2024-03-20 13:41:12.000000 jhammer-3.1.1/jhammer/config.py
--rw-r--r--   0 daijian    (501) staff       (20)     1557 2024-01-19 07:52:39.000000 jhammer-3.1.1/jhammer/cumulative_metric.py
--rw-r--r--   0 daijian    (501) staff       (20)     1269 2024-01-31 06:14:16.000000 jhammer-3.1.1/jhammer/distance_maps.py
-drwxr-xr-x   0 daijian    (501) staff       (20)        0 2024-03-30 04:38:46.830170 jhammer-3.1.1/jhammer/image/
--rw-r--r--   0 daijian    (501) staff       (20)       68 2024-01-30 14:00:33.000000 jhammer-3.1.1/jhammer/image/__init__.py
--rw-r--r--   0 daijian    (501) staff       (20)      479 2022-09-11 02:51:46.000000 jhammer-3.1.1/jhammer/image/colors.py
--rw-r--r--   0 daijian    (501) staff       (20)      382 2023-11-05 03:47:11.000000 jhammer-3.1.1/jhammer/image/contrast.py
--rw-r--r--   0 daijian    (501) staff       (20)      735 2023-10-20 08:46:51.000000 jhammer-3.1.1/jhammer/image/overlay.py
--rw-r--r--   0 daijian    (501) staff       (20)     6389 2024-01-31 06:16:04.000000 jhammer-3.1.1/jhammer/io.py
--rw-r--r--   0 daijian    (501) staff       (20)      327 2023-09-26 14:30:53.000000 jhammer-3.1.1/jhammer/log.py
-drwxr-xr-x   0 daijian    (501) staff       (20)        0 2024-03-30 04:38:46.834736 jhammer-3.1.1/jhammer/losses/
--rw-r--r--   0 daijian    (501) staff       (20)       32 2023-11-10 06:19:42.000000 jhammer-3.1.1/jhammer/losses/__init__.py
--rw-r--r--   0 daijian    (501) staff       (20)     2389 2024-01-30 15:22:05.000000 jhammer-3.1.1/jhammer/losses/dice_loss.py
--rw-r--r--   0 daijian    (501) staff       (20)     1028 2024-02-04 14:25:20.000000 jhammer-3.1.1/jhammer/lr_schedulers.py
--rw-r--r--   0 daijian    (501) staff       (20)      300 2024-01-29 12:01:59.000000 jhammer-3.1.1/jhammer/lr_utils.py
--rw-r--r--   0 daijian    (501) staff       (20)      760 2024-01-31 06:09:08.000000 jhammer-3.1.1/jhammer/medical_image_converters.py
--rw-r--r--   0 daijian    (501) staff       (20)      762 2024-03-20 13:41:12.000000 jhammer-3.1.1/jhammer/metrics.py
-drwxr-xr-x   0 daijian    (501) staff       (20)        0 2024-03-30 04:38:46.842054 jhammer-3.1.1/jhammer/models/
--rw-r--r--   0 daijian    (501) staff       (20)       64 2023-10-25 11:57:54.000000 jhammer-3.1.1/jhammer/models/__init__.py
--rw-r--r--   0 daijian    (501) staff       (20)     3892 2024-03-18 01:17:18.000000 jhammer-3.1.1/jhammer/models/unet.py
--rw-r--r--   0 daijian    (501) staff       (20)     3375 2024-03-18 01:17:18.000000 jhammer-3.1.1/jhammer/models/unet_plus_plus.py
--rw-r--r--   0 daijian    (501) staff       (20)      146 2024-01-30 15:00:06.000000 jhammer-3.1.1/jhammer/reductions.py
-drwxr-xr-x   0 daijian    (501) staff       (20)        0 2024-03-30 04:38:46.851792 jhammer-3.1.1/jhammer/samplers/
--rw-r--r--   0 daijian    (501) staff       (20)      141 2023-11-05 04:04:18.000000 jhammer-3.1.1/jhammer/samplers/__init__.py
--rw-r--r--   0 daijian    (501) staff       (20)     5396 2024-01-31 06:14:16.000000 jhammer-3.1.1/jhammer/samplers/coordinate_generator.py
--rw-r--r--   0 daijian    (501) staff       (20)     4876 2024-01-31 06:14:16.000000 jhammer-3.1.1/jhammer/samplers/grid_sampler.py
--rw-r--r--   0 daijian    (501) staff       (20)     2068 2024-01-31 06:14:16.000000 jhammer-3.1.1/jhammer/samplers/patch_picker.py
--rw-r--r--   0 daijian    (501) staff       (20)     1899 2023-11-05 04:04:18.000000 jhammer-3.1.1/jhammer/samplers/preloaded_data_loader.py
--rw-r--r--   0 daijian    (501) staff       (20)     3478 2024-01-31 00:27:50.000000 jhammer-3.1.1/jhammer/samplers/preloaded_dataset.py
--rw-r--r--   0 daijian    (501) staff       (20)     2618 2024-01-31 06:14:16.000000 jhammer-3.1.1/jhammer/samplers/utils.py
--rw-r--r--   0 daijian    (501) staff       (20)     1234 2024-01-31 00:27:50.000000 jhammer-3.1.1/jhammer/statistics.py
-drwxr-xr-x   0 daijian    (501) staff       (20)        0 2024-03-30 04:38:46.858613 jhammer-3.1.1/jhammer/transforms/
--rw-r--r--   0 daijian    (501) staff       (20)       98 2024-01-30 09:19:33.000000 jhammer-3.1.1/jhammer/transforms/__init__.py
--rw-r--r--   0 daijian    (501) staff       (20)     4247 2024-03-07 13:32:51.000000 jhammer-3.1.1/jhammer/transforms/data_transforms.py
--rw-r--r--   0 daijian    (501) staff       (20)      698 2024-03-07 13:26:40.000000 jhammer-3.1.1/jhammer/transforms/distance_transforms.py
--rw-r--r--   0 daijian    (501) staff       (20)     4458 2024-03-08 04:50:36.000000 jhammer-3.1.1/jhammer/transforms/image_transforms.py
--rw-r--r--   0 daijian    (501) staff       (20)      328 2024-03-07 13:26:40.000000 jhammer-3.1.1/jhammer/transforms/transforms.py
--rw-r--r--   0 daijian    (501) staff       (20)     2744 2024-01-31 06:14:16.000000 jhammer-3.1.1/jhammer/type_converters.py
-drwxr-xr-x   0 daijian    (501) staff       (20)        0 2024-03-30 04:38:46.826811 jhammer-3.1.1/jhammer.egg-info/
--rw-r--r--   0 daijian    (501) staff       (20)      686 2024-03-30 04:38:46.000000 jhammer-3.1.1/jhammer.egg-info/PKG-INFO
--rw-r--r--   0 daijian    (501) staff       (20)     1158 2024-03-30 04:38:46.000000 jhammer-3.1.1/jhammer.egg-info/SOURCES.txt
--rw-r--r--   0 daijian    (501) staff       (20)        1 2024-03-30 04:38:46.000000 jhammer-3.1.1/jhammer.egg-info/dependency_links.txt
--rw-r--r--   0 daijian    (501) staff       (20)      119 2024-03-30 04:38:46.000000 jhammer-3.1.1/jhammer.egg-info/requires.txt
--rw-r--r--   0 daijian    (501) staff       (20)        8 2024-03-30 04:38:46.000000 jhammer-3.1.1/jhammer.egg-info/top_level.txt
--rw-r--r--   0 daijian    (501) staff       (20)       38 2024-03-30 04:38:46.862341 jhammer-3.1.1/setup.cfg
--rw-r--r--   0 daijian    (501) staff       (20)      903 2024-03-20 11:33:18.000000 jhammer-3.1.1/setup.py
+drwxr-xr-x   0 daijian    (501) staff       (20)        0 2024-04-02 02:39:57.316423 jhammer-3.1.2/
+-rw-r--r--   0 daijian    (501) staff       (20)    35149 2022-01-18 06:32:18.000000 jhammer-3.1.2/LICENSE
+-rw-r--r--   0 daijian    (501) staff       (20)      686 2024-04-02 02:39:57.315747 jhammer-3.1.2/PKG-INFO
+-rw-r--r--   0 daijian    (501) staff       (20)        8 2022-01-18 06:32:18.000000 jhammer-3.1.2/README.md
+drwxr-xr-x   0 daijian    (501) staff       (20)        0 2024-04-02 02:39:57.280317 jhammer-3.1.2/jhammer/
+-rw-r--r--   0 daijian    (501) staff       (20)        0 2022-08-11 06:59:33.000000 jhammer-3.1.2/jhammer/__init__.py
+-rw-r--r--   0 daijian    (501) staff       (20)     1726 2024-03-20 01:43:38.000000 jhammer-3.1.2/jhammer/checkpoint.py
+-rw-r--r--   0 daijian    (501) staff       (20)     2706 2024-03-20 13:41:12.000000 jhammer-3.1.2/jhammer/config.py
+-rw-r--r--   0 daijian    (501) staff       (20)     1557 2024-01-19 07:52:39.000000 jhammer-3.1.2/jhammer/cumulative_metric.py
+-rw-r--r--   0 daijian    (501) staff       (20)     1269 2024-01-31 06:14:16.000000 jhammer-3.1.2/jhammer/distance_maps.py
+drwxr-xr-x   0 daijian    (501) staff       (20)        0 2024-04-02 02:39:57.289098 jhammer-3.1.2/jhammer/image/
+-rw-r--r--   0 daijian    (501) staff       (20)       68 2024-01-30 14:00:33.000000 jhammer-3.1.2/jhammer/image/__init__.py
+-rw-r--r--   0 daijian    (501) staff       (20)      479 2022-09-11 02:51:46.000000 jhammer-3.1.2/jhammer/image/colors.py
+-rw-r--r--   0 daijian    (501) staff       (20)      382 2023-11-05 03:47:11.000000 jhammer-3.1.2/jhammer/image/contrast.py
+-rw-r--r--   0 daijian    (501) staff       (20)      735 2023-10-20 08:46:51.000000 jhammer-3.1.2/jhammer/image/overlay.py
+-rw-r--r--   0 daijian    (501) staff       (20)     7314 2024-04-01 13:53:12.000000 jhammer-3.1.2/jhammer/io.py
+-rw-r--r--   0 daijian    (501) staff       (20)      327 2023-09-26 14:30:53.000000 jhammer-3.1.2/jhammer/log.py
+drwxr-xr-x   0 daijian    (501) staff       (20)        0 2024-04-02 02:39:57.291588 jhammer-3.1.2/jhammer/losses/
+-rw-r--r--   0 daijian    (501) staff       (20)       32 2023-11-10 06:19:42.000000 jhammer-3.1.2/jhammer/losses/__init__.py
+-rw-r--r--   0 daijian    (501) staff       (20)     2389 2024-01-30 15:22:05.000000 jhammer-3.1.2/jhammer/losses/dice_loss.py
+-rw-r--r--   0 daijian    (501) staff       (20)     1028 2024-02-04 14:25:20.000000 jhammer-3.1.2/jhammer/lr_schedulers.py
+-rw-r--r--   0 daijian    (501) staff       (20)      300 2024-01-29 12:01:59.000000 jhammer-3.1.2/jhammer/lr_utils.py
+-rw-r--r--   0 daijian    (501) staff       (20)      760 2024-01-31 06:09:08.000000 jhammer-3.1.2/jhammer/medical_image_converters.py
+-rw-r--r--   0 daijian    (501) staff       (20)      762 2024-03-20 13:41:12.000000 jhammer-3.1.2/jhammer/metrics.py
+drwxr-xr-x   0 daijian    (501) staff       (20)        0 2024-04-02 02:39:57.294604 jhammer-3.1.2/jhammer/models/
+-rw-r--r--   0 daijian    (501) staff       (20)       64 2023-10-25 11:57:54.000000 jhammer-3.1.2/jhammer/models/__init__.py
+-rw-r--r--   0 daijian    (501) staff       (20)     3892 2024-03-18 01:17:18.000000 jhammer-3.1.2/jhammer/models/unet.py
+-rw-r--r--   0 daijian    (501) staff       (20)     3375 2024-03-18 01:17:18.000000 jhammer-3.1.2/jhammer/models/unet_plus_plus.py
+-rw-r--r--   0 daijian    (501) staff       (20)      146 2024-01-30 15:00:06.000000 jhammer-3.1.2/jhammer/reductions.py
+drwxr-xr-x   0 daijian    (501) staff       (20)        0 2024-04-02 02:39:57.305307 jhammer-3.1.2/jhammer/samplers/
+-rw-r--r--   0 daijian    (501) staff       (20)      141 2023-11-05 04:04:18.000000 jhammer-3.1.2/jhammer/samplers/__init__.py
+-rw-r--r--   0 daijian    (501) staff       (20)     5396 2024-01-31 06:14:16.000000 jhammer-3.1.2/jhammer/samplers/coordinate_generator.py
+-rw-r--r--   0 daijian    (501) staff       (20)     4876 2024-01-31 06:14:16.000000 jhammer-3.1.2/jhammer/samplers/grid_sampler.py
+-rw-r--r--   0 daijian    (501) staff       (20)     2068 2024-01-31 06:14:16.000000 jhammer-3.1.2/jhammer/samplers/patch_picker.py
+-rw-r--r--   0 daijian    (501) staff       (20)     1899 2023-11-05 04:04:18.000000 jhammer-3.1.2/jhammer/samplers/preloaded_data_loader.py
+-rw-r--r--   0 daijian    (501) staff       (20)     3478 2024-01-31 00:27:50.000000 jhammer-3.1.2/jhammer/samplers/preloaded_dataset.py
+-rw-r--r--   0 daijian    (501) staff       (20)     2618 2024-01-31 06:14:16.000000 jhammer-3.1.2/jhammer/samplers/utils.py
+-rw-r--r--   0 daijian    (501) staff       (20)     1234 2024-01-31 00:27:50.000000 jhammer-3.1.2/jhammer/statistics.py
+drwxr-xr-x   0 daijian    (501) staff       (20)        0 2024-04-02 02:39:57.313736 jhammer-3.1.2/jhammer/transforms/
+-rw-r--r--   0 daijian    (501) staff       (20)       98 2024-01-30 09:19:33.000000 jhammer-3.1.2/jhammer/transforms/__init__.py
+-rw-r--r--   0 daijian    (501) staff       (20)     4247 2024-03-07 13:32:51.000000 jhammer-3.1.2/jhammer/transforms/data_transforms.py
+-rw-r--r--   0 daijian    (501) staff       (20)      698 2024-03-07 13:26:40.000000 jhammer-3.1.2/jhammer/transforms/distance_transforms.py
+-rw-r--r--   0 daijian    (501) staff       (20)     4458 2024-03-08 04:50:36.000000 jhammer-3.1.2/jhammer/transforms/image_transforms.py
+-rw-r--r--   0 daijian    (501) staff       (20)      328 2024-03-07 13:26:40.000000 jhammer-3.1.2/jhammer/transforms/transforms.py
+-rw-r--r--   0 daijian    (501) staff       (20)     2744 2024-01-31 06:14:16.000000 jhammer-3.1.2/jhammer/type_converters.py
+drwxr-xr-x   0 daijian    (501) staff       (20)        0 2024-04-02 02:39:57.284979 jhammer-3.1.2/jhammer.egg-info/
+-rw-r--r--   0 daijian    (501) staff       (20)      686 2024-04-02 02:39:57.000000 jhammer-3.1.2/jhammer.egg-info/PKG-INFO
+-rw-r--r--   0 daijian    (501) staff       (20)     1158 2024-04-02 02:39:57.000000 jhammer-3.1.2/jhammer.egg-info/SOURCES.txt
+-rw-r--r--   0 daijian    (501) staff       (20)        1 2024-04-02 02:39:57.000000 jhammer-3.1.2/jhammer.egg-info/dependency_links.txt
+-rw-r--r--   0 daijian    (501) staff       (20)      119 2024-04-02 02:39:57.000000 jhammer-3.1.2/jhammer.egg-info/requires.txt
+-rw-r--r--   0 daijian    (501) staff       (20)        8 2024-04-02 02:39:57.000000 jhammer-3.1.2/jhammer.egg-info/top_level.txt
+-rw-r--r--   0 daijian    (501) staff       (20)       38 2024-04-02 02:39:57.316631 jhammer-3.1.2/setup.cfg
+-rw-r--r--   0 daijian    (501) staff       (20)      903 2024-04-01 13:53:12.000000 jhammer-3.1.2/setup.py
```

### Comparing `jhammer-3.1.1/LICENSE` & `jhammer-3.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jhammer-3.1.1/PKG-INFO` & `jhammer-3.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jhammer
-Version: 3.1.1
+Version: 3.1.2
 Summary: My hammer for medical image processing and deap learning.
 Author: Dai Jian
 Author-email: daijian@stumail.ysu.edu.cn
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: ~=3.11
```

### Comparing `jhammer-3.1.1/jhammer/checkpoint.py` & `jhammer-3.1.2/jhammer/checkpoint.py`

 * *Files identical despite different names*

### Comparing `jhammer-3.1.1/jhammer/config.py` & `jhammer-3.1.2/jhammer/config.py`

 * *Files identical despite different names*

### Comparing `jhammer-3.1.1/jhammer/cumulative_metric.py` & `jhammer-3.1.2/jhammer/cumulative_metric.py`

 * *Files identical despite different names*

### Comparing `jhammer-3.1.1/jhammer/distance_maps.py` & `jhammer-3.1.2/jhammer/distance_maps.py`

 * *Files identical despite different names*

### Comparing `jhammer-3.1.1/jhammer/image/overlay.py` & `jhammer-3.1.2/jhammer/image/overlay.py`

 * *Files identical despite different names*

### Comparing `jhammer-3.1.1/jhammer/io.py` & `jhammer-3.1.2/jhammer/io.py`

 * *Files 8% similar despite different names*

```diff
@@ -205,7 +205,39 @@
         json.dump(obj, file, cls=NumpyJSONEncoder, **{"primitive": primitive, "base64": base64})
 
 
 def ensure_dir(input_file):
     input_dir = os.path.split(input_file)[0]
     if not os.path.exists(input_dir):
         os.makedirs(input_dir, exist_ok=True)
+
+
+def scp(dst_user, dst_host, dst_path, local_path, dst_port=None, recursive=False, send=False, receive=False):
+    """
+    Transmit file(s) through scp.
+
+    Args:
+        dst_user (str):
+        dst_host (str):
+        dst_path (str or Path):
+        local_path (str or Path):
+        dst_port (str or int or None, optional, default=None): if None, usually refer to port 22.
+        recursive (bool, default=False): transmit directories recursively.
+        send (bool, default=False): send file(s) from local to destination.
+        receive (bool, default=False): receive file(s) sent from destination.
+
+    Returns:
+
+    """
+    assert send ^ receive
+
+    cmd = "scp"
+    dst = f"{dst_user}@{dst_host}:{dst_path}"
+    if recursive:
+        cmd += " -r"
+    if dst_port:
+        cmd += f" -P {dst_port}"
+    if send:
+        cmd += f" {local_path} {dst}"
+    else:
+        cmd += f" {dst} {local_path}"
+    os.system(cmd)
```

### Comparing `jhammer-3.1.1/jhammer/losses/dice_loss.py` & `jhammer-3.1.2/jhammer/losses/dice_loss.py`

 * *Files identical despite different names*

### Comparing `jhammer-3.1.1/jhammer/lr_schedulers.py` & `jhammer-3.1.2/jhammer/lr_schedulers.py`

 * *Files identical despite different names*

### Comparing `jhammer-3.1.1/jhammer/medical_image_converters.py` & `jhammer-3.1.2/jhammer/medical_image_converters.py`

 * *Files identical despite different names*

### Comparing `jhammer-3.1.1/jhammer/metrics.py` & `jhammer-3.1.2/jhammer/metrics.py`

 * *Files identical despite different names*

### Comparing `jhammer-3.1.1/jhammer/models/unet.py` & `jhammer-3.1.2/jhammer/models/unet.py`

 * *Files identical despite different names*

### Comparing `jhammer-3.1.1/jhammer/models/unet_plus_plus.py` & `jhammer-3.1.2/jhammer/models/unet_plus_plus.py`

 * *Files identical despite different names*

### Comparing `jhammer-3.1.1/jhammer/samplers/coordinate_generator.py` & `jhammer-3.1.2/jhammer/samplers/coordinate_generator.py`

 * *Files identical despite different names*

### Comparing `jhammer-3.1.1/jhammer/samplers/grid_sampler.py` & `jhammer-3.1.2/jhammer/samplers/grid_sampler.py`

 * *Files identical despite different names*

### Comparing `jhammer-3.1.1/jhammer/samplers/patch_picker.py` & `jhammer-3.1.2/jhammer/samplers/patch_picker.py`

 * *Files identical despite different names*

### Comparing `jhammer-3.1.1/jhammer/samplers/preloaded_data_loader.py` & `jhammer-3.1.2/jhammer/samplers/preloaded_data_loader.py`

 * *Files identical despite different names*

### Comparing `jhammer-3.1.1/jhammer/samplers/preloaded_dataset.py` & `jhammer-3.1.2/jhammer/samplers/preloaded_dataset.py`

 * *Files identical despite different names*

### Comparing `jhammer-3.1.1/jhammer/samplers/utils.py` & `jhammer-3.1.2/jhammer/samplers/utils.py`

 * *Files identical despite different names*

### Comparing `jhammer-3.1.1/jhammer/statistics.py` & `jhammer-3.1.2/jhammer/statistics.py`

 * *Files identical despite different names*

### Comparing `jhammer-3.1.1/jhammer/transforms/data_transforms.py` & `jhammer-3.1.2/jhammer/transforms/data_transforms.py`

 * *Files identical despite different names*

### Comparing `jhammer-3.1.1/jhammer/transforms/distance_transforms.py` & `jhammer-3.1.2/jhammer/transforms/distance_transforms.py`

 * *Files identical despite different names*

### Comparing `jhammer-3.1.1/jhammer/transforms/image_transforms.py` & `jhammer-3.1.2/jhammer/transforms/image_transforms.py`

 * *Files identical despite different names*

### Comparing `jhammer-3.1.1/jhammer/type_converters.py` & `jhammer-3.1.2/jhammer/type_converters.py`

 * *Files identical despite different names*

### Comparing `jhammer-3.1.1/jhammer.egg-info/PKG-INFO` & `jhammer-3.1.2/jhammer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jhammer
-Version: 3.1.1
+Version: 3.1.2
 Summary: My hammer for medical image processing and deap learning.
 Author: Dai Jian
 Author-email: daijian@stumail.ysu.edu.cn
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: ~=3.11
```

### Comparing `jhammer-3.1.1/jhammer.egg-info/SOURCES.txt` & `jhammer-3.1.2/jhammer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jhammer-3.1.1/setup.py` & `jhammer-3.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="jhammer",
-    version="3.1.1",
+    version="3.1.2",
     author="Dai Jian",
     author_email="daijian@stumail.ysu.edu.cn",
     description="My hammer for medical image processing and deap learning.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

