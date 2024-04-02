# Comparing `tmp/pathopatch-1.0.0b0.tar.gz` & `tmp/pathopatch-1.0.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pathopatch-1.0.0b0.tar", last modified: Wed Mar 27 14:28:16 2024, max compression
+gzip compressed data, was "pathopatch-1.0.1b0.tar", last modified: Tue Apr  2 13:03:03 2024, max compression
```

## Comparing `pathopatch-1.0.0b0.tar` & `pathopatch-1.0.1b0.tar`

### file list

```diff
@@ -1,63 +1,67 @@
-drwxr-xr-x   0 fhoerst    (501) staff       (20)        0 2024-03-27 14:28:16.786553 pathopatch-1.0.0b0/
--rw-r--r--   0 fhoerst    (501) staff       (20)     1184 2024-03-26 16:01:10.000000 pathopatch-1.0.0b0/LICENSE.md
--rw-r--r--   0 fhoerst    (501) staff       (20)    17500 2024-03-27 14:28:16.786319 pathopatch-1.0.0b0/PKG-INFO
--rw-r--r--   0 fhoerst    (501) staff       (20)    21699 2024-03-27 12:42:32.000000 pathopatch-1.0.0b0/README.md
-drwxr-xr-x   0 fhoerst    (501) staff       (20)        0 2024-03-27 14:28:16.774145 pathopatch-1.0.0b0/pathopatch/
--rw-r--r--   0 fhoerst    (501) staff       (20)       96 2024-01-12 12:43:51.000000 pathopatch-1.0.0b0/pathopatch/__init__.py
--rw-r--r--   0 fhoerst    (501) staff       (20)     5013 2024-01-12 12:43:51.000000 pathopatch-1.0.0b0/pathopatch/annotation_conversion.py
-drwxr-xr-x   0 fhoerst    (501) staff       (20)        0 2024-03-27 14:28:16.775807 pathopatch-1.0.0b0/pathopatch/base_ml/
--rw-r--r--   0 fhoerst    (501) staff       (20)        0 2024-01-12 12:43:51.000000 pathopatch-1.0.0b0/pathopatch/base_ml/__init__.py
--rw-r--r--   0 fhoerst    (501) staff       (20)     4541 2024-01-12 12:43:51.000000 pathopatch-1.0.0b0/pathopatch/base_ml/base_cli.py
--rw-r--r--   0 fhoerst    (501) staff       (20)    39164 2024-01-23 11:58:35.000000 pathopatch-1.0.0b0/pathopatch/cli.py
-drwxr-xr-x   0 fhoerst    (501) staff       (20)        0 2024-03-27 14:28:16.776377 pathopatch-1.0.0b0/pathopatch/config/
--rw-r--r--   0 fhoerst    (501) staff       (20)       96 2024-01-12 12:43:51.000000 pathopatch-1.0.0b0/pathopatch/config/__init__.py
--rw-r--r--   0 fhoerst    (501) staff       (20)     1452 2024-01-23 10:37:28.000000 pathopatch-1.0.0b0/pathopatch/config/config.py
-drwxr-xr-x   0 fhoerst    (501) staff       (20)        0 2024-03-27 14:28:16.777109 pathopatch-1.0.0b0/pathopatch/data/
--rw-r--r--   0 fhoerst    (501) staff       (20)       96 2024-01-12 12:43:51.000000 pathopatch-1.0.0b0/pathopatch/data/__init__.py
--rw-r--r--   0 fhoerst    (501) staff       (20)     1165 2024-01-12 12:43:52.000000 pathopatch-1.0.0b0/pathopatch/macenko_vector_generation.py
-drwxr-xr-x   0 fhoerst    (501) staff       (20)        0 2024-03-27 14:28:16.779031 pathopatch-1.0.0b0/pathopatch/patch_extraction/
--rw-r--r--   0 fhoerst    (501) staff       (20)       96 2024-01-12 12:43:52.000000 pathopatch-1.0.0b0/pathopatch/patch_extraction/__init__.py
--rw-r--r--   0 fhoerst    (501) staff       (20)     3088 2024-01-12 12:43:52.000000 pathopatch-1.0.0b0/pathopatch/patch_extraction/cucim_deepzoom.py
--rw-r--r--   0 fhoerst    (501) staff       (20)    32615 2024-03-27 14:27:28.000000 pathopatch-1.0.0b0/pathopatch/patch_extraction/dataset.py
--rw-r--r--   0 fhoerst    (501) staff       (20)    61495 2024-03-27 11:56:23.000000 pathopatch-1.0.0b0/pathopatch/patch_extraction/patch_extraction.py
--rw-r--r--   0 fhoerst    (501) staff       (20)     9601 2024-01-12 12:43:52.000000 pathopatch-1.0.0b0/pathopatch/patch_extraction/process_batch.py
--rw-r--r--   0 fhoerst    (501) staff       (20)    12265 2024-01-12 12:43:52.000000 pathopatch-1.0.0b0/pathopatch/patch_extraction/storage.py
-drwxr-xr-x   0 fhoerst    (501) staff       (20)        0 2024-03-27 14:28:16.782346 pathopatch-1.0.0b0/pathopatch/utils/
--rw-r--r--   0 fhoerst    (501) staff       (20)        0 2024-01-12 12:43:52.000000 pathopatch-1.0.0b0/pathopatch/utils/__init__.py
--rw-r--r--   0 fhoerst    (501) staff       (20)      608 2024-01-12 12:43:52.000000 pathopatch-1.0.0b0/pathopatch/utils/exceptions.py
--rw-r--r--   0 fhoerst    (501) staff       (20)      626 2024-01-12 12:43:52.000000 pathopatch-1.0.0b0/pathopatch/utils/file_handling.py
--rw-r--r--   0 fhoerst    (501) staff       (20)    13833 2024-03-26 16:01:13.000000 pathopatch-1.0.0b0/pathopatch/utils/filters.py
--rw-r--r--   0 fhoerst    (501) staff       (20)     6334 2024-03-27 14:05:13.000000 pathopatch-1.0.0b0/pathopatch/utils/logger.py
--rw-r--r--   0 fhoerst    (501) staff       (20)    10801 2024-01-19 13:20:20.000000 pathopatch-1.0.0b0/pathopatch/utils/masking.py
--rw-r--r--   0 fhoerst    (501) staff       (20)     3216 2024-01-12 12:43:52.000000 pathopatch-1.0.0b0/pathopatch/utils/patch_dataset.py
--rw-r--r--   0 fhoerst    (501) staff       (20)    46353 2024-03-26 15:00:36.000000 pathopatch-1.0.0b0/pathopatch/utils/patch_util.py
--rw-r--r--   0 fhoerst    (501) staff       (20)    10592 2024-01-12 12:43:52.000000 pathopatch-1.0.0b0/pathopatch/utils/plotting.py
--rw-r--r--   0 fhoerst    (501) staff       (20)     7204 2024-01-12 12:43:52.000000 pathopatch-1.0.0b0/pathopatch/utils/tools.py
--rw-r--r--   0 fhoerst    (501) staff       (20)     1066 2024-03-26 13:08:00.000000 pathopatch-1.0.0b0/pathopatch/wsi_extraction.py
-drwxr-xr-x   0 fhoerst    (501) staff       (20)        0 2024-03-27 14:28:16.775179 pathopatch-1.0.0b0/pathopatch.egg-info/
--rw-r--r--   0 fhoerst    (501) staff       (20)    17500 2024-03-27 14:28:16.000000 pathopatch-1.0.0b0/pathopatch.egg-info/PKG-INFO
--rw-r--r--   0 fhoerst    (501) staff       (20)     1681 2024-03-27 14:28:16.000000 pathopatch-1.0.0b0/pathopatch.egg-info/SOURCES.txt
--rw-r--r--   0 fhoerst    (501) staff       (20)        1 2024-03-27 14:28:16.000000 pathopatch-1.0.0b0/pathopatch.egg-info/dependency_links.txt
--rw-r--r--   0 fhoerst    (501) staff       (20)      198 2024-03-27 14:28:16.000000 pathopatch-1.0.0b0/pathopatch.egg-info/entry_points.txt
--rw-r--r--   0 fhoerst    (501) staff       (20)      259 2024-03-27 14:28:16.000000 pathopatch-1.0.0b0/pathopatch.egg-info/requires.txt
--rw-r--r--   0 fhoerst    (501) staff       (20)       11 2024-03-27 14:28:16.000000 pathopatch-1.0.0b0/pathopatch.egg-info/top_level.txt
--rw-r--r--   0 fhoerst    (501) staff       (20)       38 2024-03-27 14:28:16.786594 pathopatch-1.0.0b0/setup.cfg
--rw-r--r--   0 fhoerst    (501) staff       (20)     2107 2024-03-27 14:27:15.000000 pathopatch-1.0.0b0/setup.py
-drwxr-xr-x   0 fhoerst    (501) staff       (20)        0 2024-03-27 14:28:16.782680 pathopatch-1.0.0b0/tests/
--rw-r--r--   0 fhoerst    (501) staff       (20)        0 2024-01-12 10:03:42.000000 pathopatch-1.0.0b0/tests/__init__.py
-drwxr-xr-x   0 fhoerst    (501) staff       (20)        0 2024-03-27 14:28:16.785097 pathopatch-1.0.0b0/tests/test_core_modules/
--rw-r--r--   0 fhoerst    (501) staff       (20)        0 2024-01-12 10:03:42.000000 pathopatch-1.0.0b0/tests/test_core_modules/__init__.py
--rw-r--r--   0 fhoerst    (501) staff       (20)     5478 2024-03-25 15:46:06.000000 pathopatch-1.0.0b0/tests/test_core_modules/test_annotations_filtering.py
--rw-r--r--   0 fhoerst    (501) staff       (20)     5956 2024-03-26 07:05:02.000000 pathopatch-1.0.0b0/tests/test_core_modules/test_baseline.py
--rw-r--r--   0 fhoerst    (501) staff       (20)     5198 2024-03-25 15:46:15.000000 pathopatch-1.0.0b0/tests/test_core_modules/test_complex_setup.py
--rw-r--r--   0 fhoerst    (501) staff       (20)     4700 2024-03-25 15:46:19.000000 pathopatch-1.0.0b0/tests/test_core_modules/test_downsample.py
--rw-r--r--   0 fhoerst    (501) staff       (20)     5457 2024-03-25 15:46:28.000000 pathopatch-1.0.0b0/tests/test_core_modules/test_roi.py
--rw-r--r--   0 fhoerst    (501) staff       (20)     5759 2024-03-25 15:46:24.000000 pathopatch-1.0.0b0/tests/test_core_modules/test_roi_context.py
--rw-r--r--   0 fhoerst    (501) staff       (20)     3064 2024-03-25 15:46:32.000000 pathopatch-1.0.0b0/tests/test_core_modules/test_target_magnification.py
--rw-r--r--   0 fhoerst    (501) staff       (20)     3021 2024-03-25 15:46:42.000000 pathopatch-1.0.0b0/tests/test_core_modules/test_target_mpp.py
--rw-r--r--   0 fhoerst    (501) staff       (20)     3705 2024-03-26 15:00:25.000000 pathopatch-1.0.0b0/tests/test_core_modules/test_target_mpp_macenko.py
-drwxr-xr-x   0 fhoerst    (501) staff       (20)        0 2024-03-27 14:28:16.785995 pathopatch-1.0.0b0/tests/test_utils/
--rw-r--r--   0 fhoerst    (501) staff       (20)        0 2024-01-12 10:03:42.000000 pathopatch-1.0.0b0/tests/test_utils/__init__.py
--rw-r--r--   0 fhoerst    (501) staff       (20)     1657 2024-01-12 12:43:52.000000 pathopatch-1.0.0b0/tests/test_utils/test_csv_loading.py
--rw-r--r--   0 fhoerst    (501) staff       (20)     5002 2024-03-26 16:01:13.000000 pathopatch-1.0.0b0/tests/test_utils/test_filters.py
--rw-r--r--   0 fhoerst    (501) staff       (20)     1254 2024-01-12 12:43:52.000000 pathopatch-1.0.0b0/tests/test_utils/test_mask_rgb.py
+drwxr-xr-x   0 fhoerst    (501) staff       (20)        0 2024-04-02 13:03:03.892184 pathopatch-1.0.1b0/
+-rw-r--r--   0 fhoerst    (501) staff       (20)     1184 2024-03-26 16:01:10.000000 pathopatch-1.0.1b0/LICENSE.md
+-rw-r--r--   0 fhoerst    (501) staff       (20)    18127 2024-04-02 13:03:03.891783 pathopatch-1.0.1b0/PKG-INFO
+-rw-r--r--   0 fhoerst    (501) staff       (20)    23383 2024-04-02 13:00:08.000000 pathopatch-1.0.1b0/README.md
+drwxr-xr-x   0 fhoerst    (501) staff       (20)        0 2024-04-02 13:03:03.879218 pathopatch-1.0.1b0/pathopatch/
+-rw-r--r--   0 fhoerst    (501) staff       (20)       96 2024-01-12 12:43:51.000000 pathopatch-1.0.1b0/pathopatch/__init__.py
+-rw-r--r--   0 fhoerst    (501) staff       (20)     5013 2024-01-12 12:43:51.000000 pathopatch-1.0.1b0/pathopatch/annotation_conversion.py
+drwxr-xr-x   0 fhoerst    (501) staff       (20)        0 2024-04-02 13:03:03.880583 pathopatch-1.0.1b0/pathopatch/base_ml/
+-rw-r--r--   0 fhoerst    (501) staff       (20)        0 2024-01-12 12:43:51.000000 pathopatch-1.0.1b0/pathopatch/base_ml/__init__.py
+-rw-r--r--   0 fhoerst    (501) staff       (20)     4541 2024-01-12 12:43:51.000000 pathopatch-1.0.1b0/pathopatch/base_ml/base_cli.py
+-rw-r--r--   0 fhoerst    (501) staff       (20)    39568 2024-04-02 12:25:57.000000 pathopatch-1.0.1b0/pathopatch/cli.py
+drwxr-xr-x   0 fhoerst    (501) staff       (20)        0 2024-04-02 13:03:03.881350 pathopatch-1.0.1b0/pathopatch/config/
+-rw-r--r--   0 fhoerst    (501) staff       (20)       96 2024-01-12 12:43:51.000000 pathopatch-1.0.1b0/pathopatch/config/__init__.py
+-rw-r--r--   0 fhoerst    (501) staff       (20)     1428 2024-04-02 12:25:57.000000 pathopatch-1.0.1b0/pathopatch/config/config.py
+drwxr-xr-x   0 fhoerst    (501) staff       (20)        0 2024-04-02 13:03:03.881678 pathopatch-1.0.1b0/pathopatch/data/
+-rw-r--r--   0 fhoerst    (501) staff       (20)       96 2024-01-12 12:43:51.000000 pathopatch-1.0.1b0/pathopatch/data/__init__.py
+-rw-r--r--   0 fhoerst    (501) staff       (20)     1165 2024-01-12 12:43:52.000000 pathopatch-1.0.1b0/pathopatch/macenko_vector_generation.py
+drwxr-xr-x   0 fhoerst    (501) staff       (20)        0 2024-04-02 13:03:03.883254 pathopatch-1.0.1b0/pathopatch/patch_extraction/
+-rw-r--r--   0 fhoerst    (501) staff       (20)       96 2024-01-12 12:43:52.000000 pathopatch-1.0.1b0/pathopatch/patch_extraction/__init__.py
+-rw-r--r--   0 fhoerst    (501) staff       (20)    32674 2024-04-02 06:34:36.000000 pathopatch-1.0.1b0/pathopatch/patch_extraction/dataset.py
+-rw-r--r--   0 fhoerst    (501) staff       (20)    63509 2024-04-02 12:25:59.000000 pathopatch-1.0.1b0/pathopatch/patch_extraction/patch_extraction.py
+-rw-r--r--   0 fhoerst    (501) staff       (20)     9676 2024-04-02 12:25:58.000000 pathopatch-1.0.1b0/pathopatch/patch_extraction/process_batch.py
+-rw-r--r--   0 fhoerst    (501) staff       (20)    12265 2024-01-12 12:43:52.000000 pathopatch-1.0.1b0/pathopatch/patch_extraction/storage.py
+drwxr-xr-x   0 fhoerst    (501) staff       (20)        0 2024-04-02 13:03:03.886088 pathopatch-1.0.1b0/pathopatch/utils/
+-rw-r--r--   0 fhoerst    (501) staff       (20)        0 2024-01-12 12:43:52.000000 pathopatch-1.0.1b0/pathopatch/utils/__init__.py
+-rw-r--r--   0 fhoerst    (501) staff       (20)      608 2024-01-12 12:43:52.000000 pathopatch-1.0.1b0/pathopatch/utils/exceptions.py
+-rw-r--r--   0 fhoerst    (501) staff       (20)      626 2024-01-12 12:43:52.000000 pathopatch-1.0.1b0/pathopatch/utils/file_handling.py
+-rw-r--r--   0 fhoerst    (501) staff       (20)    13833 2024-03-26 16:01:13.000000 pathopatch-1.0.1b0/pathopatch/utils/filters.py
+-rw-r--r--   0 fhoerst    (501) staff       (20)     6334 2024-03-27 14:05:13.000000 pathopatch-1.0.1b0/pathopatch/utils/logger.py
+-rw-r--r--   0 fhoerst    (501) staff       (20)    10801 2024-01-19 13:20:20.000000 pathopatch-1.0.1b0/pathopatch/utils/masking.py
+-rw-r--r--   0 fhoerst    (501) staff       (20)     3216 2024-01-12 12:43:52.000000 pathopatch-1.0.1b0/pathopatch/utils/patch_dataset.py
+-rw-r--r--   0 fhoerst    (501) staff       (20)    46150 2024-04-02 12:25:58.000000 pathopatch-1.0.1b0/pathopatch/utils/patch_util.py
+-rw-r--r--   0 fhoerst    (501) staff       (20)    10592 2024-01-12 12:43:52.000000 pathopatch-1.0.1b0/pathopatch/utils/plotting.py
+-rw-r--r--   0 fhoerst    (501) staff       (20)     7204 2024-01-12 12:43:52.000000 pathopatch-1.0.1b0/pathopatch/utils/tools.py
+-rw-r--r--   0 fhoerst    (501) staff       (20)     1066 2024-04-02 07:26:35.000000 pathopatch-1.0.1b0/pathopatch/wsi_extraction.py
+drwxr-xr-x   0 fhoerst    (501) staff       (20)        0 2024-04-02 13:03:03.887253 pathopatch-1.0.1b0/pathopatch/wsi_interfaces/
+-rw-r--r--   0 fhoerst    (501) staff       (20)      387 2024-03-29 14:01:43.000000 pathopatch-1.0.1b0/pathopatch/wsi_interfaces/__init__.py
+-rw-r--r--   0 fhoerst    (501) staff       (20)     3115 2024-04-02 06:35:01.000000 pathopatch-1.0.1b0/pathopatch/wsi_interfaces/cucim_deepzoom.py
+-rw-r--r--   0 fhoerst    (501) staff       (20)     1318 2024-04-02 12:25:58.000000 pathopatch-1.0.1b0/pathopatch/wsi_interfaces/openslide_deepzoom.py
+-rw-r--r--   0 fhoerst    (501) staff       (20)    10081 2024-04-02 12:25:58.000000 pathopatch-1.0.1b0/pathopatch/wsi_interfaces/wsidicomizer_openslide.py
+drwxr-xr-x   0 fhoerst    (501) staff       (20)        0 2024-04-02 13:03:03.891276 pathopatch-1.0.1b0/pathopatch.egg-info/
+-rw-r--r--   0 fhoerst    (501) staff       (20)    18127 2024-04-02 13:03:03.000000 pathopatch-1.0.1b0/pathopatch.egg-info/PKG-INFO
+-rw-r--r--   0 fhoerst    (501) staff       (20)     1817 2024-04-02 13:03:03.000000 pathopatch-1.0.1b0/pathopatch.egg-info/SOURCES.txt
+-rw-r--r--   0 fhoerst    (501) staff       (20)        1 2024-04-02 13:03:03.000000 pathopatch-1.0.1b0/pathopatch.egg-info/dependency_links.txt
+-rw-r--r--   0 fhoerst    (501) staff       (20)      198 2024-04-02 13:03:03.000000 pathopatch-1.0.1b0/pathopatch.egg-info/entry_points.txt
+-rw-r--r--   0 fhoerst    (501) staff       (20)      297 2024-04-02 13:03:03.000000 pathopatch-1.0.1b0/pathopatch.egg-info/requires.txt
+-rw-r--r--   0 fhoerst    (501) staff       (20)       11 2024-04-02 13:03:03.000000 pathopatch-1.0.1b0/pathopatch.egg-info/top_level.txt
+-rw-r--r--   0 fhoerst    (501) staff       (20)       38 2024-04-02 13:03:03.892238 pathopatch-1.0.1b0/setup.cfg
+-rw-r--r--   0 fhoerst    (501) staff       (20)     2167 2024-04-02 13:03:00.000000 pathopatch-1.0.1b0/setup.py
+drwxr-xr-x   0 fhoerst    (501) staff       (20)        0 2024-04-02 13:03:03.887740 pathopatch-1.0.1b0/tests/
+-rw-r--r--   0 fhoerst    (501) staff       (20)        0 2024-01-12 10:03:42.000000 pathopatch-1.0.1b0/tests/__init__.py
+drwxr-xr-x   0 fhoerst    (501) staff       (20)        0 2024-04-02 13:03:03.890027 pathopatch-1.0.1b0/tests/test_core_modules/
+-rw-r--r--   0 fhoerst    (501) staff       (20)        0 2024-01-12 10:03:42.000000 pathopatch-1.0.1b0/tests/test_core_modules/__init__.py
+-rw-r--r--   0 fhoerst    (501) staff       (20)     5478 2024-03-25 15:46:06.000000 pathopatch-1.0.1b0/tests/test_core_modules/test_annotations_filtering.py
+-rw-r--r--   0 fhoerst    (501) staff       (20)     5956 2024-03-26 07:05:02.000000 pathopatch-1.0.1b0/tests/test_core_modules/test_baseline.py
+-rw-r--r--   0 fhoerst    (501) staff       (20)     5198 2024-03-25 15:46:15.000000 pathopatch-1.0.1b0/tests/test_core_modules/test_complex_setup.py
+-rw-r--r--   0 fhoerst    (501) staff       (20)     4700 2024-03-25 15:46:19.000000 pathopatch-1.0.1b0/tests/test_core_modules/test_downsample.py
+-rw-r--r--   0 fhoerst    (501) staff       (20)     5457 2024-03-25 15:46:28.000000 pathopatch-1.0.1b0/tests/test_core_modules/test_roi.py
+-rw-r--r--   0 fhoerst    (501) staff       (20)     5759 2024-03-25 15:46:24.000000 pathopatch-1.0.1b0/tests/test_core_modules/test_roi_context.py
+-rw-r--r--   0 fhoerst    (501) staff       (20)     3064 2024-03-25 15:46:32.000000 pathopatch-1.0.1b0/tests/test_core_modules/test_target_magnification.py
+-rw-r--r--   0 fhoerst    (501) staff       (20)     3021 2024-03-25 15:46:42.000000 pathopatch-1.0.1b0/tests/test_core_modules/test_target_mpp.py
+-rw-r--r--   0 fhoerst    (501) staff       (20)     3705 2024-03-26 15:00:25.000000 pathopatch-1.0.1b0/tests/test_core_modules/test_target_mpp_macenko.py
+drwxr-xr-x   0 fhoerst    (501) staff       (20)        0 2024-04-02 13:03:03.890980 pathopatch-1.0.1b0/tests/test_utils/
+-rw-r--r--   0 fhoerst    (501) staff       (20)        0 2024-01-12 10:03:42.000000 pathopatch-1.0.1b0/tests/test_utils/__init__.py
+-rw-r--r--   0 fhoerst    (501) staff       (20)     1657 2024-01-12 12:43:52.000000 pathopatch-1.0.1b0/tests/test_utils/test_csv_loading.py
+-rw-r--r--   0 fhoerst    (501) staff       (20)     5002 2024-03-26 16:01:13.000000 pathopatch-1.0.1b0/tests/test_utils/test_filters.py
+-rw-r--r--   0 fhoerst    (501) staff       (20)     1254 2024-01-12 12:43:52.000000 pathopatch-1.0.1b0/tests/test_utils/test_mask_rgb.py
```

### Comparing `pathopatch-1.0.0b0/LICENSE.md` & `pathopatch-1.0.1b0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pathopatch-1.0.0b0/PKG-INFO` & `pathopatch-1.0.1b0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pathopatch
-Version: 1.0.0b0
+Version: 1.0.1b0
 Summary: PathoPatch - Accelerating Artificial Intelligence Based Whole Slide Image Analysis with an Optimized Preprocessing Pipeline
 Home-page: https://github.com/TIO-IKIM/PathoPatcher
 Author: Fabian Hörst
 Author-email: fabian.hoerst@uk-essen.de
 Keywords: python,pathopatch
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
@@ -12,14 +12,36 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Other
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
+Requires-Dist: Pillow>=9.5.0
+Requires-Dist: PyYAML
+Requires-Dist: Shapely==1.8.5.post1
+Requires-Dist: colorama
+Requires-Dist: future
+Requires-Dist: geojson>=3.0.0
+Requires-Dist: matplotlib
+Requires-Dist: natsort
+Requires-Dist: numpy<1.24,>1.22
+Requires-Dist: opencv_python_headless
+Requires-Dist: openslide_python
+Requires-Dist: pandas
+Requires-Dist: pydantic==1.10.4
+Requires-Dist: rasterio==1.3.5.post1
+Requires-Dist: requests
+Requires-Dist: scikit-image
+Requires-Dist: setuptools<=65.6.3
+Requires-Dist: tqdm
+Requires-Dist: torchvision
+Requires-Dist: torch
+Requires-Dist: wsidicom==0.20.4
+Requires-Dist: wsidicomizer==0.13.2
 
 [![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-360/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 ![Test-Results](https://github.com/TIO-IKIM/PathoPatcher/actions/workflows/test_build.yml/badge.svg)
 <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=Pytorch&logoColor=white"/></a>
 
 ___
```

### Comparing `pathopatch-1.0.0b0/README.md` & `pathopatch-1.0.1b0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -50,14 +50,16 @@
 This activates pre-commit hooks, files are edited when commited and need to added again as they might change
 
 ## Usage
 We provide different use cases - Offline-Dataset (Store on Disk :floppy_disk:) and Inference-Dataset for :zap: PyTorch :zap:
 
 In our Pre-Processing pipeline, we are able to extract quadratic patches from detected tissue areas, load annotation files (`.json`) and apply color normlizations. We make use of the popular [OpenSlide](https://openslide.org/) library, but extended it with the [RAPIDS cuCIM](https://github.com/rapidsai/cucim) framework for a speedup in patch-extraction.
 
+> We support all OpenSlide file formats + .dcm-File format (DICOM), by utilizing [`wsidicom`](https://github.com/imi-bigpicture/wsidicom) and [`wsidicomizer`](https://github.com/imi-bigpicture/wsidicomizer).
+
 **Explanations for use cases :floppy_disk: vs :zap:**
 <details>
   <summary>Offline-Dataset</summary>
 
 
   In general, our framework has the following commands registered in your shell:
   > **wsi_extraction**: Extract patches with specific configuration and store them on the disk
@@ -365,18 +367,31 @@
   ```
 </details>
 
 ## Examples
 An example notebook is given [here](PathoPatch.ipynb):
 <a href="https://colab.research.google.com/github/TIO-IKIM/PathoPatcher/blob/main/PathoPatch.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
 
-## Roadmap
-- :construction: In-memory inference loader - This feature is currently under development. Once completed, it will allow a dataset to be loaded into memory for inference, eliminating the need to store it on disk. Useful for inference
+### Example config files
+Example config files for various use-cases can be found in the [test database](tests/static_test_files/preprocessing) (tests/static_test_files/preprocessing)
+
+### DICOM-conversion
+To convert WSI-Files into DICOM-Format, please follow [this documentation](docs/DICOM.md)
+
+### Filelist with metadata
+See here: [examples/filelist.csv](examples/filelist.csv)
+
+```csv
+path,slide_mpp,magnification
+./test_database/input/WSI/CMU-1.svs,0.500,20
+```
+Only the path is enforced, other two cols are optional.
 
-- :soon: Dicom support - We plan to add another backend for handling DICOM files with a different structure
+## Roadmap
+- :construction: In-memory inference loader - This feature is currently under development -  an unstable version is already online. Once completed, it will allow a dataset to be loaded into memory for inference, eliminating the need to store it on disk. Useful for inference
 
 - :soon: More test cases
 
 - :soon: More examples
 
 ## License
 <p xmlns:cc="http://creativecommons.org/ns#" xmlns:dct="http://purl.org/dc/terms/"><a property="dct:title" rel="cc:attributionURL" href="https://github.com/TIO-IKIM/PathoPatcher">PathoPatcher</a> by <a rel="cc:attributionURL dct:creator" property="cc:attributionName" href="https://github.com/FabianHoerst">Fabian Hörst, University Hospital Essen,</a> is licensed under <a href="http://creativecommons.org/licenses/by-nc-sa/4.0/?ref=chooser-v1" target="_blank" rel="license noopener noreferrer" style="display:inline-block;">CC BY-NC-SA 4.0
@@ -402,10 +417,17 @@
     booktitle="Bildverarbeitung f{\"u}r die Medizin 2024",
     year="2024",
     publisher="Springer Fachmedien Wiesbaden",
     address="Wiesbaden",
     pages="356--361",,
     isbn="978-3-658-44037-4"
 }
+```
 
+### Acknowledgement
+For processing DICOM-files, this work relies on the IMI-Bigpicture [`wsidicom`](https://github.com/imi-bigpicture/wsidicom) and [`wsidicomizer`](https://github.com/imi-bigpicture/wsidicomizer) libraries, with the following acknowledgements:
 
-```
+>wsidicom: Copyright 2021 Sectra AB, licensed under Apache 2.0.
+This project is part of a project that has received funding from the Innovative Medicines Initiative 2 Joint Undertaking under grant agreement No 945358. This Joint Undertaking receives support from the European Union’s Horizon 2020 research and innovation programme and EFPIA. IMI website: <www.imi.europa.eu>
+
+>wsidicomizer: Copyright 2021 Sectra AB, licensed under Apache 2.0.
+This project is part of a project that has received funding from the Innovative Medicines Initiative 2 Joint Undertaking under grant agreement No 945358. This Joint Undertaking receives support from the European Union’s Horizon 2020 research and innovation programme and EFPIA. IMI website: <www.imi.europa.eu>
```

### Comparing `pathopatch-1.0.0b0/pathopatch/annotation_conversion.py` & `pathopatch-1.0.1b0/pathopatch/annotation_conversion.py`

 * *Files identical despite different names*

### Comparing `pathopatch-1.0.0b0/pathopatch/base_ml/base_cli.py` & `pathopatch-1.0.1b0/pathopatch/base_ml/base_cli.py`

 * *Files identical despite different names*

### Comparing `pathopatch-1.0.0b0/pathopatch/cli.py` & `pathopatch-1.0.1b0/pathopatch/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,17 +81,19 @@
     """Storing the preprocessing configuration
 
     All string that describe paths are converted to pathlib.Path objects.
 
     Args:
         wsi_paths (str): Path to the folder where all WSI are stored or path to a single WSI-file.
         output_path (str): Path to the folder where the resulting dataset should be stored.
-        wsi_extension (str, optional): The extension of the WSI-files. Defaults to "svs.
+        wsi_extension (str, optional): The extension of the WSI-files. Defaults to "svs".
         wsi_filelist (str, optional): Path to a csv-filelist with WSI files (separator: `,`), if provided just these files are used. Must include full paths to WSIs, including suffixes.
-            Can be used as an replacement for the wsi_paths option. If both are provided, yields an error. Defaults to None.
+            Can be used as an replacement for the wsi_paths option. If both are provided, yields an error.
+            The path to the files should be written in a column named "path". Metadata for slide magnification and mpp can be provided in columns named 'slide_mpp' and 'magnification'.
+            Defaults to None.
         patch_size (int, optional): The size of the patches in pixel that will be retrieved from the WSI, e.g. 256 for 256px. Defaults to 256.
         patch_overlap (float, optional): The percentage amount pixels that should overlap between two different patches.
             Please Provide as integer between 0 and 100, indicating overlap in percentage.
             Defaults to 0.
         target_mpp (float, optional): If this parameter is provided, the output level of the WSI
             corresponds to the level that is at the target microns per pixel of the WSI.
             Alternative to target_mag, downsaple and level. Highest priority, overwrites all other setups for magnifcation, downsample, or level.
@@ -335,17 +337,19 @@
             "--wsi_paths",
             type=str,
             help="Path to the folder where all WSI are stored or path to a single WSI-file.",
         )
         parser.add_argument(
             "--wsi_filelist",
             type=str,
-            help="Path to a csv-filelist with WSI files (separator: `,`), if provided just these files are used."
-            "Must include full paths to WSIs, including suffixes."
-            "Can be used as an replacement for the wsi_paths option."
+            help="Path to a csv-filelist with WSI files (separator: `,`), if provided just these files are used. "
+            "Must include full paths to WSIs, including suffixes. "
+            "Can be used as an replacement for the wsi_paths option. "
+            "The path to the files should be written in a column named `path`. "
+            "Metadata for slide magnification and mpp can be provided in columns named `slide_mpp` and `magnification`. "
             "If both are provided, yields an error.",
         )
         parser.add_argument(
             "--output_path",
             type=str,
             help="Path to the folder where the resulting dataset should be stored.",
         )
```

### Comparing `pathopatch-1.0.0b0/pathopatch/config/config.py` & `pathopatch-1.0.1b0/pathopatch/config/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "tif",
     "bif",
     "scn",
     "ndpi",
     "vms",
     "vmu",
     "dcm",
-]  # mirax not tested yet
+]
 ANNOTATION_EXT: List[str] = ["json"]
 LOGGING_EXT: List[str] = ["critical", "error", "warning", "info", "debug"]
 
 # Currently: 30 Colors
 COLOR_DEFINITIONS: dict[int, tuple[int]] = {
     0: (239, 71, 111),
     1: (255, 209, 102),
```

### Comparing `pathopatch-1.0.0b0/pathopatch/macenko_vector_generation.py` & `pathopatch-1.0.1b0/pathopatch/macenko_vector_generation.py`

 * *Files identical despite different names*

### Comparing `pathopatch-1.0.0b0/pathopatch/patch_extraction/cucim_deepzoom.py` & `pathopatch-1.0.1b0/pathopatch/wsi_interfaces/cucim_deepzoom.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 
 
 class DeepZoomGeneratorCucim(DeepZoomGenerator):
     """Create a DeepZoomGenerator, but instead of utilizing OpenSlide,
     use cucim to read regions.
 
     Args:
-        osr (OpenSlide): OpenSlide Image. Needed for OS compatibility and for retrieving metadata.
-        cucim_slide (CuImage): CuImage slide. Used for retrieving image data.
+        meta_loader (OpenSlide): OpenSlide Image. Needed for OS compatibility and for retrieving metadata.
+        image_loader (CuImage): CuImage slide. Used for retrieving image data.
         tile_size (int, optional): the width and height of a single tile.  For best viewer
                       performance, tile_size + 2 * overlap should be a power
                       of two.. Defaults to 254.
         overlap (int, optional): the number of extra pixels to add to each interior edge
                       of a tile. Defaults to 1.
         limit_bounds (bool, optional): True to render only the non-empty slide region. Defaults to False.
 
@@ -37,23 +37,23 @@
 
     Methods:
         get_tile(level: int, address: tuple[int]) -> Image: Returns an RGB PIL.Image for a tile.
     """
 
     def __init__(
         self,
-        osr: OpenSlide,
-        cucim_slide: CuImage,
+        meta_loader: OpenSlide,
+        image_loader: CuImage,
         tile_size: int = 254,
         overlap: int = 1,
         limit_bounds=False,
     ):
-        super().__init__(osr, tile_size, overlap, limit_bounds)
+        super().__init__(meta_loader, tile_size, overlap, limit_bounds)
 
-        self._cucim_slide = cucim_slide
+        self._cucim_slide = image_loader
         self.memory_capacity = preferred_memory_capacity(
             self._cucim_slide, patch_size=(tile_size, tile_size)
         )
         self.cache = CuImage.cache(
             "per_process", memory_capacity=self.memory_capacity, record_stat=True
         )
```

### Comparing `pathopatch-1.0.0b0/pathopatch/patch_extraction/dataset.py` & `pathopatch-1.0.1b0/pathopatch/patch_extraction/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 from pydantic import BaseModel, validator
 from shapely.affinity import scale
 from shapely.geometry import Polygon
 from torch.utils.data import Dataset
 from torchvision.transforms.v2 import ToTensor
 from PIL import Image
 from pathopatch.utils.exceptions import WrongParameterException
+from pathopatch.wsi_interfaces.openslide_deepzoom import DeepZoomGeneratorOS
 from pathopatch.utils.patch_util import (
-    DeepZoomGeneratorOS,
     calculate_background_ratio,
     compute_interesting_patches,
     get_intersected_labels,
     get_regions_json,
     macenko_normalization,
     pad_tile,
     patch_to_tile_size,
@@ -280,15 +280,15 @@
 
     def _set_hardware(self) -> None:
         """Either load CuCIM (GPU-accelerated) or OpenSlide"""
         if module_exists("cucim", error="ignore"):
             self.logger.debug("Using CuCIM")
             from cucim import CuImage
 
-            from pathopatch.patch_extraction.cucim_deepzoom import (
+            from pathopatch.wsi_interfaces.cucim_deepzoom import (
                 DeepZoomGeneratorCucim,
             )
 
             self.deepzoomgenerator = DeepZoomGeneratorCucim
             self.image_loader = CuImage
         else:
             self.logger.debug("Using OpenSlide")
@@ -447,16 +447,16 @@
             resulting_mpp = slide_properties["mpp"] * self.config.downsample
 
         self.res_tile_size, self.res_overlap = patch_to_tile_size(
             self.config.patch_size, self.config.patch_overlap, self.rescaling_factor
         )
 
         self.tile_extractor = self.deepzoomgenerator(
-            osr=self.slide_openslide,
-            cucim_slide=self.slide,
+            meta_loader=self.slide_openslide,
+            image_loader=self.slide,
             tile_size=self.res_tile_size,
             overlap=self.res_overlap,
             limit_bounds=True,
         )
 
         if self.config.downsample is not None:
             # Each level is downsampled by a factor of 2
```

### Comparing `pathopatch-1.0.0b0/pathopatch/patch_extraction/patch_extraction.py` & `pathopatch-1.0.1b0/pathopatch/patch_extraction/patch_extraction.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,45 +2,45 @@
 # Main Patch Extraction Class for a WSI/Dataset
 #
 # @ Fabian Hörst, fabian.hoerst@uk-essen.de
 # Institute for Artifical Intelligence in Medicine,
 # University Medicine Essen
 
 
-import csv
 import json
 import multiprocessing
 import os
 import random
 import re
 from pathlib import Path
 from shutil import rmtree
 from typing import Any, Callable, List, Tuple, Union
+
 import matplotlib
 import torch
 
 matplotlib.use("Agg")  # Agg is a non-interactive backend
 
 import warnings
 
 import numpy as np
+import pandas as pd
 from natsort import natsorted
 from openslide import OpenSlide
 from PIL import Image
 from shapely.affinity import scale
 from shapely.geometry import Polygon
 from tqdm import tqdm
 
 from pathopatch import logger
 from pathopatch.cli import PreProcessingConfig
 from pathopatch.patch_extraction.storage import Storage
 from pathopatch.utils.exceptions import UnalignedDataException, WrongParameterException
 from pathopatch.utils.patch_dataset import load_tissue_detection_dl
 from pathopatch.utils.patch_util import (
-    DeepZoomGeneratorOS,
     calculate_background_ratio,
     compute_interesting_patches,
     generate_thumbnails,
     get_files_from_dir,
     get_intersected_labels,
     get_regions_json,
     get_regions_xml,
@@ -48,14 +48,19 @@
     macenko_normalization,
     pad_tile,
     patch_to_tile_size,
     target_mag_to_downsample,
     target_mpp_to_downsample,
 )
 from pathopatch.utils.tools import end_timer, module_exists, start_timer
+from pathopatch.wsi_interfaces.openslide_deepzoom import DeepZoomGeneratorOS
+from pathopatch.wsi_interfaces.wsidicomizer_openslide import (
+    DicomSlide,
+    DeepZoomGeneratorDicom,
+)
 
 warnings.filterwarnings("ignore", category=DeprecationWarning)
 warnings.filterwarnings("ignore", category=UserWarning)
 
 
 def queue_worker(
     q: multiprocessing.Queue,
@@ -191,14 +196,15 @@
         deepzoomgenerator (Union[DeepZoomGeneratorOS, DeepZoomGeneratorCucim]): DeepZoomGenerator object
         image_loader (Union[OpenSlide, CuImage]): Image loader object
         detector_device (str): Device for tissue detection
         detector_model (nn.Module): Tissue detection model
         detector_transforms (Compose): Tissue detection transforms
         curr_wsi_level (int): Current WSI level
         save_context (bool): Save context flag
+        # TODO: improve and check with new dcm coce and new filelist loading
 
     Methods:
         setup_output_path(output_path: Union[str, Path]) -> None:
             Create output path
         _set_wsi_paths(wsi_paths: Union[str, Path, List], wsi_extension: str) -> None:
             Set the path(s) to the WSI files. Find all wsi files with given extension
         _load_wsi_filelist(wsi_filelist: Union[str, Path]) -> None:
@@ -266,14 +272,15 @@
         self.detector_model: torch.nn.Module
         self.detector_transforms: Callable
         self.curr_wsi_level: int
         self.save_context: bool
 
         self.config = slide_processor_config
         self.files, self.annotation_files = [], []
+        self.global_properties = {}
         self.num_files = 0
         self.rescaling_factor = 1
 
         # paths
         self.setup_output_path(self.config.output_path)
         if self.config.wsi_paths is not None:
             self._set_wsi_paths(self.config.wsi_paths, self.config.wsi_extension)
@@ -338,30 +345,42 @@
     def _load_wsi_filelist(self, wsi_filelist: Union[str, Path]) -> None:
         """Load wsi from csv filelist
 
         Args:
             wsi_filelist (Union[str, Path]):  Path to the CSV file containing the WSI file list.
 
         CSV File Example:
-            The CSV file should contain a single column with the paths to the WSI files.
+            The CSV file should contain the path column, with path to the WSI. slide_mpp and magnification are optional.
             Example content of "wsi_filelist.csv":
             ```
-            /path/to/wsi1.svs
-            /path/to/wsi2.svs
-            /path/to/wsi3.svs
+            path,slide_mpp,magnification
+            test_database/input/WSI/CMU-1.svs,0.499,20
             ```
         """
         self.files = []
-        with open(wsi_filelist, "r") as csv_file:
-            csv_reader = csv.reader(csv_file)
-            for row in csv_reader:
-                self.files.append(Path(row[0]))
-        self.files = natsorted(self.files, key=lambda x: x.name)
+        csv_file = pd.read_csv(wsi_filelist, sep=",")
+
+        self.files = natsorted(csv_file["path"].to_list(), key=lambda x: Path(x).name)
+        self.files = [Path(f) for f in self.files]
         self.num_files = len(self.files)
 
+        for row in csv_file.iterrows():
+            file = row[1]["path"]
+            try:
+                slide_mpp = row[1]["slide_mpp"]
+            except KeyError:
+                slide_mpp = None
+            try:
+                magnification = row[1]["magnification"]
+            except KeyError:
+                magnification = None
+            prop_dict = {"slide_mpp": slide_mpp, "magnification": magnification}
+            prop_dict = {k: v for k, v in prop_dict.items() if v is not None}
+            self.global_properties[Path(file).name] = prop_dict
+
     def _set_annotations_paths(
         self,
         annotation_paths: Union[Path, str],
         annotation_extension: str,
         incomplete_annotations: bool = True,
     ) -> None:
         """Set the path to the annotation files. Find all annotations
@@ -399,31 +418,36 @@
         """Either load CuCIM (GPU-accelerated) or OpenSlide
 
 
         Args:
             hardware_selection (str, optional): Specify hardware. Just for experiments. Must be either "openslide", or "cucim".
                 Defaults to cucim.
         """
-        if (
-            module_exists("cucim", error="ignore")
-            and hardware_selection.lower() == "cucim"
-        ):
-            logger.info("Using CuCIM")
-            from cucim import CuImage
+        if self.config.wsi_extension == "dcm":
+            logger.info("Using WsiDicom as WSIReader")
+            self.deepzoomgenerator = DeepZoomGeneratorDicom
+            self.image_loader = DicomSlide
+        else:
+            if (
+                module_exists("cucim", error="ignore")
+                and hardware_selection.lower() == "cucim"
+            ):
+                logger.info("Using CuCIM as WSIReader")
+                from cucim import CuImage
 
-            from pathopatch.patch_extraction.cucim_deepzoom import (
-                DeepZoomGeneratorCucim,
-            )
+                from pathopatch.wsi_interfaces.cucim_deepzoom import (
+                    DeepZoomGeneratorCucim,
+                )
 
-            self.deepzoomgenerator = DeepZoomGeneratorCucim
-            self.image_loader = CuImage
-        else:
-            logger.info("Using OpenSlide")
-            self.deepzoomgenerator = DeepZoomGeneratorOS
-            self.image_loader = OpenSlide
+                self.deepzoomgenerator = DeepZoomGeneratorCucim
+                self.image_loader = CuImage
+            else:
+                logger.info("Using OpenSlide as WSIReader")
+                self.deepzoomgenerator = DeepZoomGeneratorOS
+                self.image_loader = OpenSlide
 
     def _set_tissue_detector(self) -> None:
         """Set up the tissue detection model and transformations.
 
         Raises:
             ImportError: If torch or torchvision cannot be imported.
 
@@ -770,55 +794,68 @@
         Todo:
             * TODO: Check if this works out for non-GPU devices
             * TODO: Class documentation link
         """
         logger.info(f"Computing patches for {wsi_file.name}")
 
         # load slide (OS and CuImage/OS)
-        slide = OpenSlide(str(wsi_file))
+        if self.config.wsi_extension == "dcm":
+            slide = DicomSlide(wsi_file)
+        else:
+            slide = OpenSlide(str(wsi_file))
         slide_cu = self.image_loader(str(wsi_file))
-        if "openslide.mpp-x" in slide.properties:
-            slide_mpp = float(slide.properties.get("openslide.mpp-x"))
-        elif (
-            self.config.wsi_properties is not None
-            and "slide_mpp" in self.config.wsi_properties
-        ):
-            slide_mpp = self.config.wsi_properties["slide_mpp"]
-        else:  # last option is to use regex
-            try:
-                pattern = re.compile(r"MPP(?: =)? (\d+\.\d+)")
-                # Use the pattern to find the match in the string
-                match = pattern.search(slide.properties["openslide.comment"])
-                # Extract the float value
-                if match:
-                    slide_mpp = float(match.group(1))
-                    logger.warning(
-                        f"MPP {slide_mpp:.4f} was extracted from the comment of the WSI (Tiff-Metadata comment string) - Please check for correctness!"
-                    )
-                else:
+
+        slide_mpp = None
+        slide_mag = None
+        if str(wsi_file.name) in self.global_properties:
+            slide_properties = self.global_properties[str(wsi_file.name)]
+            if "slide_mpp" in slide_properties:
+                slide_mpp = slide_properties["slide_mpp"]
+            if "magnification" in slide_properties:
+                slide_mag = slide_properties["magnification"]
+        if slide_mpp is None:
+            if "openslide.mpp-x" in slide.properties:
+                slide_mpp = float(slide.properties.get("openslide.mpp-x"))
+            elif (
+                self.config.wsi_properties is not None
+                and "slide_mpp" in self.config.wsi_properties
+            ):
+                slide_mpp = self.config.wsi_properties["slide_mpp"]
+            else:  # last option is to use regex
+                try:
+                    pattern = re.compile(r"MPP(?: =)? (\d+\.\d+)")
+                    # Use the pattern to find the match in the string
+                    match = pattern.search(slide.properties["openslide.comment"])
+                    # Extract the float value
+                    if match:
+                        slide_mpp = float(match.group(1))
+                        logger.warning(
+                            f"MPP {slide_mpp:.4f} was extracted from the comment of the WSI (Tiff-Metadata comment string) - Please check for correctness!"
+                        )
+                    else:
+                        raise NotImplementedError(
+                            "MPP must be defined either by metadata or by config file!"
+                        )
+                except:
                     raise NotImplementedError(
                         "MPP must be defined either by metadata or by config file!"
                     )
-            except:
+        if slide_mag is None:
+            if "openslide.objective-power" in slide.properties:
+                slide_mag = float(slide.properties.get("openslide.objective-power"))
+            elif (
+                self.config.wsi_properties is not None
+                and "magnification" in self.config.wsi_properties
+            ):
+                slide_mag = self.config.wsi_properties["magnification"]
+            else:
                 raise NotImplementedError(
-                    "MPP must be defined either by metadata or by config file!"
+                    "Magnification must be defined either by metadata or by config file!"
                 )
 
-        if "openslide.objective-power" in slide.properties:
-            slide_mag = float(slide.properties.get("openslide.objective-power"))
-        elif (
-            self.config.wsi_properties is not None
-            and "magnification" in self.config.wsi_properties
-        ):
-            slide_mag = self.config.wsi_properties["magnification"]
-        else:
-            raise NotImplementedError(
-                "MPP must be defined either by metadata or by config file!"
-            )
-
         slide_properties = {"mpp": slide_mpp, "magnification": slide_mag}
         # Generate thumbnails
         logger.info("Generate thumbnails")
         thumbnails = generate_thumbnails(
             slide, slide_properties["mpp"], sample_factors=[32, 64, 128]
         )  # todo
 
@@ -856,16 +893,16 @@
         # - Pixel coordinates within slide level 0 (l0_)
         # Tile size is the amount of pixels that are taken from the image (without overlaps)
         tile_size, overlap = patch_to_tile_size(
             self.config.patch_size, self.config.patch_overlap, self.rescaling_factor
         )
 
         tiles = self.deepzoomgenerator(
-            osr=slide,
-            cucim_slide=slide_cu,
+            meta_loader=slide,
+            image_loader=slide_cu,
             tile_size=tile_size,
             overlap=overlap,
             limit_bounds=True,
         )
 
         if self.config.downsample is not None:
             # Each level is downsampled by a factor of 2
@@ -999,35 +1036,38 @@
         """
         logger.debug(f"Started process {multiprocessing.current_process().name}")
 
         # store context_tiles
         context_tiles = {}
 
         # reload image
-        slide = OpenSlide(str(wsi_file))
+        if self.config.wsi_extension == "dcm":
+            slide = DicomSlide(wsi_file)
+        else:
+            slide = OpenSlide(str(wsi_file))
         slide_cu = self.image_loader(str(wsi_file))
 
         tile_size, overlap = patch_to_tile_size(
             self.config.patch_size, self.config.patch_overlap, self.rescaling_factor
         )
 
         tiles = self.deepzoomgenerator(
-            osr=slide,
-            cucim_slide=slide_cu,
+            meta_loader=slide,
+            image_loader=slide_cu,
             tile_size=tile_size,
             overlap=overlap,
             limit_bounds=True,
         )
 
         if self.config.context_scales is not None:
             for c_scale in self.config.context_scales:
                 overlap_context = int((c_scale - 1) * tile_size / 2) + overlap
                 context_tiles[c_scale] = self.deepzoomgenerator(
-                    osr=slide,
-                    cucim_slide=slide_cu,
+                    meta_loader=slide,
+                    image_loader=slide_cu,
                     tile_size=tile_size,  # tile_size,
                     overlap=overlap_context,  # (1-c_scale) * tile_size / 2,
                     limit_bounds=True,
                 )
         # queue setup
         queue = multiprocessing.Queue()
         processes = []
@@ -1220,16 +1260,16 @@
         slide = OpenSlide(str(wsi_file))
         slide_cu = self.image_loader(str(wsi_file))
 
         tile_size, overlap = patch_to_tile_size(
             self.config.patch_size, self.config.patch_overlap, self.rescaling_factor
         )
         tiles = self.deepzoomgenerator(
-            osr=slide,
-            cucim_slide=slide_cu,
+            meta_loader=slide,
+            image_loader=slide_cu,
             tile_size=tile_size,
             overlap=overlap,
             limit_bounds=True,
         )
 
         (
             interesting_coords,
@@ -1348,16 +1388,16 @@
         tile_size, overlap = patch_to_tile_size(
             self.config.patch_size, self.config.patch_overlap
         )
 
         # extract all patches
         patches = []
         tiles = self.deepzoomgenerator(
-            osr=slide,
-            cucim_slide=slide_cu,
+            meta_loader=slide,
+            image_loader=slide_cu,
             tile_size=tile_size,
             overlap=overlap,
             limit_bounds=True,
         )
 
         for row, col, _ in interesting_coords_wsi:
             new_tile = np.array(
```

### Comparing `pathopatch-1.0.0b0/pathopatch/patch_extraction/process_batch.py` & `pathopatch-1.0.1b0/pathopatch/patch_extraction/process_batch.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,26 +11,25 @@
 from typing import Dict, List, Tuple, Union
 
 import numpy as np
 from openslide import OpenSlide
 from PIL import Image
 from shapely.geometry import Polygon
 
+from pathopatch import logger
 from pathopatch.utils.patch_util import (
-    DeepZoomGeneratorOS,
     calculate_background_ratio,
     get_intersected_labels,
     macenko_normalization,
     pad_tile,
     patch_to_tile_size,
     standardize_brightness,
 )
 from pathopatch.utils.tools import module_exists
-
-from pathopatch import logger
+from pathopatch.wsi_interfaces.openslide_deepzoom import DeepZoomGeneratorOS
 
 
 def process_batch(
     batch: List[Tuple[int, int, float]],
     *,
     wsi_file: Union[Path, str],
     wsi_metadata: dict,
@@ -103,40 +102,40 @@
     else:
         context_patches = {}
 
     # reopen slide
     if module_exists("cucim", error="ignore"):
         from cucim import CuImage
 
-        from pathopatch.deepzoom.cucim_deepzoom import DeepZoomGeneratorCucim
+        from pathopatch.wsi_interfaces.cucim_deepzoom import DeepZoomGeneratorCucim
 
         generator_module = DeepZoomGeneratorCucim
         image_loader = CuImage
     else:
         generator_module = DeepZoomGeneratorOS
         image_loader = OpenSlide
 
     slide = OpenSlide(str(wsi_file))
     slide_cu = image_loader(str(wsi_file))
     tile_size = patch_to_tile_size(patch_size, patch_overlap)
 
     tiles = generator_module(
-        osr=slide,
-        cucim_slide=slide_cu,
+        meta_loader=slide,
+        image_loader=slide_cu,
         tile_size=tile_size,
         overlap=patch_overlap,
         limit_bounds=True,
     )
 
     if context_scales is not None:
         for scale in context_scales:
             overlap_context = int((scale - 1) * patch_size / 2) + patch_overlap
             context_tiles[scale] = generator_module(
-                osr=slide,
-                cucim_slide=slide_cu,
+                meta_loader=slide,
+                image_loader=slide_cu,
                 tile_size=tile_size,  # tile_size,
                 overlap=overlap_context,  # (1-scale) * tile_size / 2,
                 limit_bounds=True,
             )
     # patches_count = 0
 
     for row, col, _ in batch:
```

### Comparing `pathopatch-1.0.0b0/pathopatch/patch_extraction/storage.py` & `pathopatch-1.0.1b0/pathopatch/patch_extraction/storage.py`

 * *Files identical despite different names*

### Comparing `pathopatch-1.0.0b0/pathopatch/utils/exceptions.py` & `pathopatch-1.0.1b0/pathopatch/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `pathopatch-1.0.0b0/pathopatch/utils/file_handling.py` & `pathopatch-1.0.1b0/pathopatch/utils/file_handling.py`

 * *Files identical despite different names*

### Comparing `pathopatch-1.0.0b0/pathopatch/utils/filters.py` & `pathopatch-1.0.1b0/pathopatch/utils/filters.py`

 * *Files identical despite different names*

### Comparing `pathopatch-1.0.0b0/pathopatch/utils/logger.py` & `pathopatch-1.0.1b0/pathopatch/utils/logger.py`

 * *Files identical despite different names*

### Comparing `pathopatch-1.0.0b0/pathopatch/utils/masking.py` & `pathopatch-1.0.1b0/pathopatch/utils/masking.py`

 * *Files identical despite different names*

### Comparing `pathopatch-1.0.0b0/pathopatch/utils/patch_dataset.py` & `pathopatch-1.0.1b0/pathopatch/utils/patch_dataset.py`

 * *Files identical despite different names*

### Comparing `pathopatch-1.0.0b0/pathopatch/utils/patch_util.py` & `pathopatch-1.0.1b0/pathopatch/utils/patch_util.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,33 +43,48 @@
         file_type (str, optional): The desired file extension. Defaults to "svs".
 
     Returns:
         List[Path]: A list of valid paths with the given file extension
     """
     if not isinstance(file_path, list):
         file_path = [file_path]
-    all_files = []
-    for curr_path in file_path:
-        # Could be that the path itself is a WSI
-        curr_path = Path(curr_path)
-        if curr_path.suffix[1:] == file_type and curr_path.is_file():
-            all_files += [curr_path]
-        else:
-            all_files += [
-                curr_file
-                for curr_file in curr_path.glob("*." + file_type)
-                if curr_file.is_file()
-            ]
-            # Could also be (class) folder in folder
-            if len(all_files) == 0:
+    if file_type == "dcm":
+        # dicom files: files of one WSI need to be stored inside a folder
+        all_files = []
+        for curr_path in file_path:
+            # check if path contains dcm files
+            subfiles = [f for f in curr_path.glob("*.dcm") if f.is_file()]
+            if len(subfiles) != 0:
+                all_files.append(curr_path)  # -> dicom folder needs to be loaded
+            # check if path contains subfolders with dicom files
+            subfolders = [f for f in curr_path.glob("*") if f.is_dir()]
+            for subfolder in subfolders:
+                subfiles = [f for f in subfolder.glob("*.dcm") if f.is_file()]
+                if len(subfiles) != 0:
+                    all_files.append(subfolder)
+    else:
+        all_files = []
+        for curr_path in file_path:
+            # Could be that the path itself is a WSI
+            curr_path = Path(curr_path)
+            if curr_path.suffix[1:] == file_type and curr_path.is_file():
+                all_files += [curr_path]
+            else:
                 all_files += [
                     curr_file
-                    for curr_file in curr_path.glob("**/*" + file_type)
+                    for curr_file in curr_path.glob("*." + file_type)
                     if curr_file.is_file()
                 ]
+                # Could also be (class) folder in folder
+                if len(all_files) == 0:
+                    all_files += [
+                        curr_file
+                        for curr_file in curr_path.glob("**/*" + file_type)
+                        if curr_file.is_file()
+                    ]
 
     return all_files
 
 
 def is_power_of_two(n: int) -> bool:
     """Checks if input integer is power of two
 
@@ -1076,27 +1091,7 @@
             label_mask = np.zeros((mask_size, mask_size, num_labels), dtype=np.uint8)
             for poly, label in poly_label_pair:
                 label_submask = np.zeros((patch_size, patch_size), dtype=np.uint8)
                 rasterize((poly, 1), out=label_mask, all_touched=True)
                 label_mask[:, :, label] = label_submask
 
     return label_mask
-
-
-# ignore kwargs for OpenSlide DeepZoomGenerator
-class DeepZoomGeneratorOS(DeepZoomGenerator):
-    def __init__(self, osr, tile_size=254, overlap=1, limit_bounds=False, **kwargs):
-        """Overwrite DeepZoomGenerator of OpenSlide
-
-            DeepZoomGenerator gets overwritten to provide matching API with CuCim
-            No Change in functionality
-
-        Args:
-            osr (OpenSlide): OpenSlide Image. Needed for OS compatibility and for retrieving metadata.
-            tile_size (int, optional): the width and height of a single tile.  For best viewer
-                          performance, tile_size + 2 * overlap should be a power
-                          of two.. Defaults to 254.
-            overlap (int, optional): the number of extra pixels to add to each interior edge
-                          of a tile. Defaults to 1.
-            limit_bounds (bool, optional): True to render only the non-empty slide region. Defaults to False.
-        """
-        super().__init__(osr, tile_size, overlap, limit_bounds)
```

### Comparing `pathopatch-1.0.0b0/pathopatch/utils/plotting.py` & `pathopatch-1.0.1b0/pathopatch/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `pathopatch-1.0.0b0/pathopatch/utils/tools.py` & `pathopatch-1.0.1b0/pathopatch/utils/tools.py`

 * *Files identical despite different names*

### Comparing `pathopatch-1.0.0b0/pathopatch/wsi_extraction.py` & `pathopatch-1.0.1b0/pathopatch/wsi_extraction.py`

 * *Files identical despite different names*

### Comparing `pathopatch-1.0.0b0/pathopatch.egg-info/PKG-INFO` & `pathopatch-1.0.1b0/pathopatch.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pathopatch
-Version: 1.0.0b0
+Version: 1.0.1b0
 Summary: PathoPatch - Accelerating Artificial Intelligence Based Whole Slide Image Analysis with an Optimized Preprocessing Pipeline
 Home-page: https://github.com/TIO-IKIM/PathoPatcher
 Author: Fabian Hörst
 Author-email: fabian.hoerst@uk-essen.de
 Keywords: python,pathopatch
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
@@ -12,14 +12,36 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Other
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
+Requires-Dist: Pillow>=9.5.0
+Requires-Dist: PyYAML
+Requires-Dist: Shapely==1.8.5.post1
+Requires-Dist: colorama
+Requires-Dist: future
+Requires-Dist: geojson>=3.0.0
+Requires-Dist: matplotlib
+Requires-Dist: natsort
+Requires-Dist: numpy<1.24,>1.22
+Requires-Dist: opencv_python_headless
+Requires-Dist: openslide_python
+Requires-Dist: pandas
+Requires-Dist: pydantic==1.10.4
+Requires-Dist: rasterio==1.3.5.post1
+Requires-Dist: requests
+Requires-Dist: scikit-image
+Requires-Dist: setuptools<=65.6.3
+Requires-Dist: tqdm
+Requires-Dist: torchvision
+Requires-Dist: torch
+Requires-Dist: wsidicom==0.20.4
+Requires-Dist: wsidicomizer==0.13.2
 
 [![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-360/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 ![Test-Results](https://github.com/TIO-IKIM/PathoPatcher/actions/workflows/test_build.yml/badge.svg)
 <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=Pytorch&logoColor=white"/></a>
 
 ___
```

### Comparing `pathopatch-1.0.0b0/pathopatch.egg-info/SOURCES.txt` & `pathopatch-1.0.1b0/pathopatch.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -14,29 +14,32 @@
 pathopatch.egg-info/top_level.txt
 pathopatch/base_ml/__init__.py
 pathopatch/base_ml/base_cli.py
 pathopatch/config/__init__.py
 pathopatch/config/config.py
 pathopatch/data/__init__.py
 pathopatch/patch_extraction/__init__.py
-pathopatch/patch_extraction/cucim_deepzoom.py
 pathopatch/patch_extraction/dataset.py
 pathopatch/patch_extraction/patch_extraction.py
 pathopatch/patch_extraction/process_batch.py
 pathopatch/patch_extraction/storage.py
 pathopatch/utils/__init__.py
 pathopatch/utils/exceptions.py
 pathopatch/utils/file_handling.py
 pathopatch/utils/filters.py
 pathopatch/utils/logger.py
 pathopatch/utils/masking.py
 pathopatch/utils/patch_dataset.py
 pathopatch/utils/patch_util.py
 pathopatch/utils/plotting.py
 pathopatch/utils/tools.py
+pathopatch/wsi_interfaces/__init__.py
+pathopatch/wsi_interfaces/cucim_deepzoom.py
+pathopatch/wsi_interfaces/openslide_deepzoom.py
+pathopatch/wsi_interfaces/wsidicomizer_openslide.py
 tests/__init__.py
 tests/test_core_modules/__init__.py
 tests/test_core_modules/test_annotations_filtering.py
 tests/test_core_modules/test_baseline.py
 tests/test_core_modules/test_complex_setup.py
 tests/test_core_modules/test_downsample.py
 tests/test_core_modules/test_roi.py
```

### Comparing `pathopatch-1.0.0b0/setup.py` & `pathopatch-1.0.1b0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-VERSION = "1.0.0b"
+VERSION = "1.0.1b"
 DESCRIPTION = "PathoPatch - Accelerating Artificial Intelligence Based Whole Slide Image Analysis with an Optimized Preprocessing Pipeline"
 with open("docs/README_pypi.md", "r") as fh:
     LONG_DESCRIPTION = fh.read()
 
 # Setting up
 setup(
     # the name must match the folder name 'verysimplemodule'
@@ -35,14 +35,16 @@
         "rasterio==1.3.5.post1",
         "requests",
         "scikit-image",
         "setuptools<=65.6.3",
         "tqdm",
         "torchvision",
         "torch",
+        "wsidicom==0.20.4",
+        "wsidicomizer==0.13.2",
     ],
     scripts=[
         "pathopatch/wsi_extraction.py",
         "pathopatch/annotation_conversion.py",
         "pathopatch/macenko_vector_generation.py",
     ],
     entry_points={
```

### Comparing `pathopatch-1.0.0b0/tests/test_core_modules/test_annotations_filtering.py` & `pathopatch-1.0.1b0/tests/test_core_modules/test_annotations_filtering.py`

 * *Files identical despite different names*

### Comparing `pathopatch-1.0.0b0/tests/test_core_modules/test_baseline.py` & `pathopatch-1.0.1b0/tests/test_core_modules/test_baseline.py`

 * *Files identical despite different names*

### Comparing `pathopatch-1.0.0b0/tests/test_core_modules/test_complex_setup.py` & `pathopatch-1.0.1b0/tests/test_core_modules/test_complex_setup.py`

 * *Files identical despite different names*

### Comparing `pathopatch-1.0.0b0/tests/test_core_modules/test_downsample.py` & `pathopatch-1.0.1b0/tests/test_core_modules/test_downsample.py`

 * *Files identical despite different names*

### Comparing `pathopatch-1.0.0b0/tests/test_core_modules/test_roi.py` & `pathopatch-1.0.1b0/tests/test_core_modules/test_roi.py`

 * *Files identical despite different names*

### Comparing `pathopatch-1.0.0b0/tests/test_core_modules/test_roi_context.py` & `pathopatch-1.0.1b0/tests/test_core_modules/test_roi_context.py`

 * *Files identical despite different names*

### Comparing `pathopatch-1.0.0b0/tests/test_core_modules/test_target_magnification.py` & `pathopatch-1.0.1b0/tests/test_core_modules/test_target_magnification.py`

 * *Files identical despite different names*

### Comparing `pathopatch-1.0.0b0/tests/test_core_modules/test_target_mpp.py` & `pathopatch-1.0.1b0/tests/test_core_modules/test_target_mpp.py`

 * *Files identical despite different names*

### Comparing `pathopatch-1.0.0b0/tests/test_core_modules/test_target_mpp_macenko.py` & `pathopatch-1.0.1b0/tests/test_core_modules/test_target_mpp_macenko.py`

 * *Files identical despite different names*

### Comparing `pathopatch-1.0.0b0/tests/test_utils/test_csv_loading.py` & `pathopatch-1.0.1b0/tests/test_utils/test_csv_loading.py`

 * *Files identical despite different names*

### Comparing `pathopatch-1.0.0b0/tests/test_utils/test_filters.py` & `pathopatch-1.0.1b0/tests/test_utils/test_filters.py`

 * *Files identical despite different names*

### Comparing `pathopatch-1.0.0b0/tests/test_utils/test_mask_rgb.py` & `pathopatch-1.0.1b0/tests/test_utils/test_mask_rgb.py`

 * *Files identical despite different names*

