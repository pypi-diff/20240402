# Comparing `tmp/cut-detector-0.0.8.tar.gz` & `tmp/cut-detector-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cut-detector-0.0.8.tar", last modified: Fri Dec  1 15:07:49 2023, max compression
+gzip compressed data, was "cut-detector-0.0.9.tar", last modified: Tue Apr  2 15:15:07 2024, max compression
```

## Comparing `cut-detector-0.0.8.tar` & `cut-detector-0.0.9.tar`

### file list

```diff
@@ -1,85 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 15:07:49.257459 cut-detector-0.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 15:07:49.245459 cut-detector-0.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 15:07:49.249459 cut-detector-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2875 2023-12-01 15:07:33.000000 cut-detector-0.0.8/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2023-12-01 15:07:33.000000 cut-detector-0.0.8/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 15:07:49.249459 cut-detector-0.0.8/.napari-hub/
--rw-r--r--   0 runner    (1001) docker     (127)      463 2023-12-01 15:07:33.000000 cut-detector-0.0.8/.napari-hub/DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (127)      542 2023-12-01 15:07:33.000000 cut-detector-0.0.8/.napari-hub/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      815 2023-12-01 15:07:33.000000 cut-detector-0.0.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2023-12-01 15:07:33.000000 cut-detector-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       96 2023-12-01 15:07:33.000000 cut-detector-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6381 2023-12-01 15:07:49.257459 cut-detector-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4586 2023-12-01 15:07:33.000000 cut-detector-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 15:07:49.249459 cut-detector-0.0.8/playground/
--rw-r--r--   0 runner    (1001) docker     (127)      742 2023-12-01 15:07:33.000000 cut-detector-0.0.8/playground/napari_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2023-12-01 15:07:33.000000 cut-detector-0.0.8/playground/segmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2023-12-01 15:07:33.000000 cut-detector-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2023-12-01 15:07:49.257459 cut-detector-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 15:07:49.245459 cut-detector-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 15:07:49.249459 cut-detector-0.0.8/src/cut_detector/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2023-12-01 15:07:33.000000 cut-detector-0.0.8/src/cut_detector/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 15:07:49.253459 cut-detector-0.0.8/src/cut_detector/_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 15:07:33.000000 cut-detector-0.0.8/src/cut_detector/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2023-12-01 15:07:33.000000 cut-detector-0.0.8/src/cut_detector/_tests/test_micro_tubules_cut_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2023-12-01 15:07:33.000000 cut-detector-0.0.8/src/cut_detector/_tests/test_mid_body_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2023-12-01 15:07:33.000000 cut-detector-0.0.8/src/cut_detector/_tests/test_results_saving.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2023-12-01 15:07:33.000000 cut-detector-0.0.8/src/cut_detector/_tests/test_segmentation_tracking.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2023-12-01 15:07:33.000000 cut-detector-0.0.8/src/cut_detector/_tests/test_track_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)      141 2023-12-01 15:07:33.000000 cut-detector-0.0.8/src/cut_detector/_tests/test_whole_process.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-12-01 15:07:49.000000 cut-detector-0.0.8/src/cut_detector/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     8586 2023-12-01 15:07:33.000000 cut-detector-0.0.8/src/cut_detector/_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 15:07:49.253459 cut-detector-0.0.8/src/cut_detector/constants/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 15:07:33.000000 cut-detector-0.0.8/src/cut_detector/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2023-12-01 15:07:33.000000 cut-detector-0.0.8/src/cut_detector/constants/annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2023-12-01 15:07:33.000000 cut-detector-0.0.8/src/cut_detector/constants/bridges.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2023-12-01 15:07:33.000000 cut-detector-0.0.8/src/cut_detector/constants/tracking.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 15:07:49.253459 cut-detector-0.0.8/src/cut_detector/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 15:07:33.000000 cut-detector-0.0.8/src/cut_detector/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2023-12-01 15:07:33.000000 cut-detector-0.0.8/src/cut_detector/data/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 15:07:49.253459 cut-detector-0.0.8/src/cut_detector/factories/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 15:07:33.000000 cut-detector-0.0.8/src/cut_detector/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17669 2023-12-01 15:07:33.000000 cut-detector-0.0.8/src/cut_detector/factories/mid_body_detection_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    29512 2023-12-01 15:07:33.000000 cut-detector-0.0.8/src/cut_detector/factories/mt_cut_detection_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    12535 2023-12-01 15:07:33.000000 cut-detector-0.0.8/src/cut_detector/factories/tracks_merging_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 15:07:49.253459 cut-detector-0.0.8/src/cut_detector/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 15:07:33.000000 cut-detector-0.0.8/src/cut_detector/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2023-12-01 15:07:33.000000 cut-detector-0.0.8/src/cut_detector/models/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2023-12-01 15:07:33.000000 cut-detector-0.0.8/src/cut_detector/napari.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 15:07:49.253459 cut-detector-0.0.8/src/cut_detector/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 15:07:33.000000 cut-detector-0.0.8/src/cut_detector/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2023-12-01 15:07:33.000000 cut-detector-0.0.8/src/cut_detector/utils/box_dimensions.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2023-12-01 15:07:33.000000 cut-detector-0.0.8/src/cut_detector/utils/box_dimensions_dln.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 15:07:49.257459 cut-detector-0.0.8/src/cut_detector/utils/bridges_classification/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-01 15:07:33.000000 cut-detector-0.0.8/src/cut_detector/utils/bridges_classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      377 2023-12-01 15:07:33.000000 cut-detector-0.0.8/src/cut_detector/utils/bridges_classification/impossible_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)      477 2023-12-01 15:07:33.000000 cut-detector-0.0.8/src/cut_detector/utils/bridges_classification/template_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 15:07:49.257459 cut-detector-0.0.8/src/cut_detector/utils/cell_division_detection/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 15:07:33.000000 cut-detector-0.0.8/src/cut_detector/utils/cell_division_detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      728 2023-12-01 15:07:33.000000 cut-detector-0.0.8/src/cut_detector/utils/cell_division_detection/metaphase_cnn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2023-12-01 15:07:33.000000 cut-detector-0.0.8/src/cut_detector/utils/cell_division_detection/metaphase_cnn_data_set.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2023-12-01 15:07:33.000000 cut-detector-0.0.8/src/cut_detector/utils/cell_division_detection/metaphase_cnn_model_params.py
--rw-r--r--   0 runner    (1001) docker     (127)    12513 2023-12-01 15:07:33.000000 cut-detector-0.0.8/src/cut_detector/utils/hidden_markov_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     6453 2023-12-01 15:07:33.000000 cut-detector-0.0.8/src/cut_detector/utils/image_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2023-12-01 15:07:33.000000 cut-detector-0.0.8/src/cut_detector/utils/mid_body_spot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2023-12-01 15:07:33.000000 cut-detector-0.0.8/src/cut_detector/utils/mid_body_track.py
--rw-r--r--   0 runner    (1001) docker     (127)    24807 2023-12-01 15:07:33.000000 cut-detector-0.0.8/src/cut_detector/utils/mitosis_track.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2023-12-01 15:07:33.000000 cut-detector-0.0.8/src/cut_detector/utils/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2023-12-01 15:07:33.000000 cut-detector-0.0.8/src/cut_detector/utils/trackmate_frame_spots.py
--rw-r--r--   0 runner    (1001) docker     (127)     2608 2023-12-01 15:07:33.000000 cut-detector-0.0.8/src/cut_detector/utils/trackmate_spot.py
--rw-r--r--   0 runner    (1001) docker     (127)    10424 2023-12-01 15:07:33.000000 cut-detector-0.0.8/src/cut_detector/utils/trackmate_track.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 15:07:49.257459 cut-detector-0.0.8/src/cut_detector/widget_functions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 15:07:33.000000 cut-detector-0.0.8/src/cut_detector/widget_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3033 2023-12-01 15:07:33.000000 cut-detector-0.0.8/src/cut_detector/widget_functions/mid_body_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     7077 2023-12-01 15:07:33.000000 cut-detector-0.0.8/src/cut_detector/widget_functions/mitosis_track_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2023-12-01 15:07:33.000000 cut-detector-0.0.8/src/cut_detector/widget_functions/mt_cut_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)    11116 2023-12-01 15:07:33.000000 cut-detector-0.0.8/src/cut_detector/widget_functions/save_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     6685 2023-12-01 15:07:33.000000 cut-detector-0.0.8/src/cut_detector/widget_functions/tracking.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 15:07:49.257459 cut-detector-0.0.8/src/cut_detector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6381 2023-12-01 15:07:49.000000 cut-detector-0.0.8/src/cut_detector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2703 2023-12-01 15:07:49.000000 cut-detector-0.0.8/src/cut_detector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-01 15:07:49.000000 cut-detector-0.0.8/src/cut_detector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2023-12-01 15:07:49.000000 cut-detector-0.0.8/src/cut_detector.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      238 2023-12-01 15:07:49.000000 cut-detector-0.0.8/src/cut_detector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-12-01 15:07:49.000000 cut-detector-0.0.8/src/cut_detector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      594 2023-12-01 15:07:33.000000 cut-detector-0.0.8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:15:07.961104 cut-detector-0.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:15:07.949104 cut-detector-0.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:15:07.949104 cut-detector-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-04-02 15:14:56.000000 cut-detector-0.0.9/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-04-02 15:14:56.000000 cut-detector-0.0.9/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:15:07.953104 cut-detector-0.0.9/.napari-hub/
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-02 15:14:56.000000 cut-detector-0.0.9/.napari-hub/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-02 15:14:56.000000 cut-detector-0.0.9/.napari-hub/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-02 15:14:56.000000 cut-detector-0.0.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-02 15:14:56.000000 cut-detector-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-02 15:14:56.000000 cut-detector-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6537 2024-04-02 15:15:07.961104 cut-detector-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-04-02 15:14:56.000000 cut-detector-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:15:07.953104 cut-detector-0.0.9/playground/
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-02 15:14:56.000000 cut-detector-0.0.9/playground/mid_body_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-04-02 15:14:56.000000 cut-detector-0.0.9/playground/mid_body_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-02 15:14:56.000000 cut-detector-0.0.9/playground/mid_body_execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-04-02 15:14:56.000000 cut-detector-0.0.9/playground/mt_cut_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-04-02 15:14:56.000000 cut-detector-0.0.9/playground/napari_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-04-02 15:14:56.000000 cut-detector-0.0.9/playground/segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-04-02 15:14:56.000000 cut-detector-0.0.9/playground/tracking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-02 15:14:56.000000 cut-detector-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-02 15:15:07.965104 cut-detector-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:15:07.949104 cut-detector-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:15:07.953104 cut-detector-0.0.9/src/cut_detector/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-02 15:14:56.000000 cut-detector-0.0.9/src/cut_detector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:15:07.957104 cut-detector-0.0.9/src/cut_detector/_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 15:14:56.000000 cut-detector-0.0.9/src/cut_detector/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-02 15:14:56.000000 cut-detector-0.0.9/src/cut_detector/_tests/test_annotations_upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-02 15:14:56.000000 cut-detector-0.0.9/src/cut_detector/_tests/test_micro_tubules_cut_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-02 15:14:56.000000 cut-detector-0.0.9/src/cut_detector/_tests/test_mid_body_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-02 15:14:56.000000 cut-detector-0.0.9/src/cut_detector/_tests/test_results_saving.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-02 15:14:56.000000 cut-detector-0.0.9/src/cut_detector/_tests/test_segmentation_tracking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-02 15:14:56.000000 cut-detector-0.0.9/src/cut_detector/_tests/test_track_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-02 15:14:56.000000 cut-detector-0.0.9/src/cut_detector/_tests/test_whole_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-02 15:15:07.000000 cut-detector-0.0.9/src/cut_detector/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8374 2024-04-02 15:14:56.000000 cut-detector-0.0.9/src/cut_detector/_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:15:07.957104 cut-detector-0.0.9/src/cut_detector/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 15:14:56.000000 cut-detector-0.0.9/src/cut_detector/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-04-02 15:14:56.000000 cut-detector-0.0.9/src/cut_detector/constants/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-02 15:14:56.000000 cut-detector-0.0.9/src/cut_detector/constants/tracking.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:15:07.957104 cut-detector-0.0.9/src/cut_detector/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 15:14:56.000000 cut-detector-0.0.9/src/cut_detector/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-04-02 15:14:56.000000 cut-detector-0.0.9/src/cut_detector/data/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:15:07.957104 cut-detector-0.0.9/src/cut_detector/factories/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 15:14:56.000000 cut-detector-0.0.9/src/cut_detector/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19322 2024-04-02 15:14:56.000000 cut-detector-0.0.9/src/cut_detector/factories/mid_body_detection_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12309 2024-04-02 15:14:56.000000 cut-detector-0.0.9/src/cut_detector/factories/mt_cut_detection_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11926 2024-04-02 15:14:56.000000 cut-detector-0.0.9/src/cut_detector/factories/results_saving_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8231 2024-04-02 15:14:56.000000 cut-detector-0.0.9/src/cut_detector/factories/segmentation_tracking_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10933 2024-04-02 15:14:56.000000 cut-detector-0.0.9/src/cut_detector/factories/tracks_merging_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:15:07.957104 cut-detector-0.0.9/src/cut_detector/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 15:14:56.000000 cut-detector-0.0.9/src/cut_detector/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-02 15:14:56.000000 cut-detector-0.0.9/src/cut_detector/models/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-02 15:14:56.000000 cut-detector-0.0.9/src/cut_detector/napari.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:15:07.961104 cut-detector-0.0.9/src/cut_detector/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 15:14:56.000000 cut-detector-0.0.9/src/cut_detector/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-02 15:14:56.000000 cut-detector-0.0.9/src/cut_detector/utils/box_dimensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-02 15:14:56.000000 cut-detector-0.0.9/src/cut_detector/utils/box_dimensions_dln.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:15:07.961104 cut-detector-0.0.9/src/cut_detector/utils/bridges_classification/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 15:14:56.000000 cut-detector-0.0.9/src/cut_detector/utils/bridges_classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-02 15:14:56.000000 cut-detector-0.0.9/src/cut_detector/utils/bridges_classification/bridges_mt_cnn_model_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7118 2024-04-02 15:14:56.000000 cut-detector-0.0.9/src/cut_detector/utils/bridges_classification/bridges_mt_model_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-02 15:14:56.000000 cut-detector-0.0.9/src/cut_detector/utils/bridges_classification/impossible_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6210 2024-04-02 15:14:56.000000 cut-detector-0.0.9/src/cut_detector/utils/bridges_classification/micro_tubules_augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-02 15:14:56.000000 cut-detector-0.0.9/src/cut_detector/utils/bridges_classification/template_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:15:07.961104 cut-detector-0.0.9/src/cut_detector/utils/cell_division_detection/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 15:14:56.000000 cut-detector-0.0.9/src/cut_detector/utils/cell_division_detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-02 15:14:56.000000 cut-detector-0.0.9/src/cut_detector/utils/cell_division_detection/metaphase_cnn_model_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-02 15:14:56.000000 cut-detector-0.0.9/src/cut_detector/utils/cell_spot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11091 2024-04-02 15:14:56.000000 cut-detector-0.0.9/src/cut_detector/utils/cell_track.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-02 15:14:56.000000 cut-detector-0.0.9/src/cut_detector/utils/cnn_data_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-04-02 15:14:56.000000 cut-detector-0.0.9/src/cut_detector/utils/hidden_markov_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6645 2024-04-02 15:14:56.000000 cut-detector-0.0.9/src/cut_detector/utils/image_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-02 15:14:56.000000 cut-detector-0.0.9/src/cut_detector/utils/mid_body_spot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-02 15:14:56.000000 cut-detector-0.0.9/src/cut_detector/utils/mid_body_track.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27304 2024-04-02 15:14:56.000000 cut-detector-0.0.9/src/cut_detector/utils/mitosis_track.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-02 15:14:56.000000 cut-detector-0.0.9/src/cut_detector/utils/spot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17022 2024-04-02 15:14:56.000000 cut-detector-0.0.9/src/cut_detector/utils/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-02 15:14:56.000000 cut-detector-0.0.9/src/cut_detector/utils/track.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-02 15:14:56.000000 cut-detector-0.0.9/src/cut_detector/utils/trackmate_frame_spots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-02 15:14:56.000000 cut-detector-0.0.9/src/cut_detector/utils/trackmate_spot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-02 15:14:56.000000 cut-detector-0.0.9/src/cut_detector/utils/trackmate_track.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:15:07.961104 cut-detector-0.0.9/src/cut_detector/widget_functions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 15:14:56.000000 cut-detector-0.0.9/src/cut_detector/widget_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-04-02 15:14:56.000000 cut-detector-0.0.9/src/cut_detector/widget_functions/mid_body_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7382 2024-04-02 15:14:56.000000 cut-detector-0.0.9/src/cut_detector/widget_functions/mitosis_track_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-04-02 15:14:56.000000 cut-detector-0.0.9/src/cut_detector/widget_functions/mt_cut_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-02 15:14:56.000000 cut-detector-0.0.9/src/cut_detector/widget_functions/save_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-02 15:14:56.000000 cut-detector-0.0.9/src/cut_detector/widget_functions/tracking.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:15:07.961104 cut-detector-0.0.9/src/cut_detector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6537 2024-04-02 15:15:07.000000 cut-detector-0.0.9/src/cut_detector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-04-02 15:15:07.000000 cut-detector-0.0.9/src/cut_detector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 15:15:07.000000 cut-detector-0.0.9/src/cut_detector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-02 15:15:07.000000 cut-detector-0.0.9/src/cut_detector.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-02 15:15:07.000000 cut-detector-0.0.9/src/cut_detector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-02 15:15:07.000000 cut-detector-0.0.9/src/cut_detector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-02 15:14:56.000000 cut-detector-0.0.9/tox.ini
```

### Comparing `cut-detector-0.0.8/.github/workflows/test_and_deploy.yml` & `cut-detector-0.0.9/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `cut-detector-0.0.8/.gitignore` & `cut-detector-0.0.9/.gitignore`

 * *Files 16% similar despite different names*

```diff
@@ -83,16 +83,26 @@
 # written by setuptools_scm
 **/_version.py
 
 # downloaded models
 src/cut_detector/models/segmentation_model
 src/cut_detector/models/hmm_bridges_parameters.npz
 src/cut_detector/models/hmm_metaphase_parameters.npz
-src/cut_detector/models/metaphase_cnn/
-src/cut_detector/models/svc_bridges/
+
+src/cut_detector/models/metaphase_cnn*
+src/cut_detector/models/svc_bridges*
+src/cut_detector/models/hmm*
+src/cut_detector/models/segmentation*
+src/cut_detector/models/bridges_mt_cnn*
+
 
 # downloaded data
 src/cut_detector/data/mitoses/
 src/cut_detector/data/models/
 src/cut_detector/data/tracks/
 src/cut_detector/data/videos/
 src/cut_detector/data/results/
+src/cut_detector/data/mitosis_movies/
+src/cut_detector/data/mid_bodies/
+src/cut_detector/data/segmentation_results/
+src/cut_detector/data/spots/
+src/cut_detector/data/annotations/
```

### Comparing `cut-detector-0.0.8/.napari-hub/config.yml` & `cut-detector-0.0.9/.napari-hub/config.yml`

 * *Files identical despite different names*

### Comparing `cut-detector-0.0.8/.pre-commit-config.yaml` & `cut-detector-0.0.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cut-detector-0.0.8/LICENSE` & `cut-detector-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cut-detector-0.0.8/PKG-INFO` & `cut-detector-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cut-detector
-Version: 0.0.8
+Version: 0.0.9
 Summary: Automatic Cut Detector
 Home-page: https://github.com/15bonte/cut-detector
 Author: Thomas Bonte
 Author-email: thomas.bonte@mines-paristech.fr
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/15bonte/cut-detector/issues
 Project-URL: Documentation, https://github.com/15bonte/cut-detector#README.md
@@ -24,15 +24,15 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cellpose>=2.2.3
 Requires-Dist: pyimagej
 Requires-Dist: scyjava
 Requires-Dist: numpy<=1.24
-Requires-Dist: cnn_framework==0.0.11
+Requires-Dist: cnn_framework==0.0.15
 Requires-Dist: magicgui
 Requires-Dist: pydantic==1.10.12
 Requires-Dist: xmltodict
 Requires-Dist: shapely
 Requires-Dist: aicsimageio
 Requires-Dist: scikit-learn==1.2.2
 Requires-Dist: charset-normalizer==3.3.0
@@ -72,34 +72,47 @@
 
 ### Conda environment
 
 It is highly recommended to create a dedicated conda environment, by following these few steps:
 
 1. Install an [Anaconda] distribution of Python. Note you might need to use an anaconda prompt if you did not add anaconda to the path.
 
-2. Open an Anaconda prompt as admin to create a new environment using [conda]. We advice to use python 3.10 and conda 23.10.0, to get conda-libmamba-solver as default solver. Note than openjdk is necessary to call Fiji from python, which is needed as you will see below.
+2. Open an Anaconda prompt as admin to create a new environment using [conda]. We advice to use python 3.10 and conda 23.10.0, to get conda-libmamba-solver as default solver.
 
 ```
 conda create --name cut_detector python=3.10 conda=23.10.0
 conda activate cut_detector
-conda install -c conda-forge openjdk=8
 ```
 
 ### Package installation
 
 Once in a dedicated environment, our package can be installed via [pip]:
 
 ```
 pip install cut_detector
 ```
 
+Alternatively, you can clone the github repo to access to playground scripts.
+
+```
+git clone https://github.com/15bonte/cut-detector.git
+cd cut-detector
+pip install -e .
+```
+
 ### Fiji
 
 This package relies on [Trackmate] to perform cell tracking. Trackmate is called through [Fiji], which has to be installed independently. Please follow the steps [here](https://imagej.net/software/fiji/downloads) to install it.
 
+Next, install openjdk which is necessary to call Fiji from python.
+
+```
+conda install -c conda-forge openjdk=8
+```
+
 ### GPU
 
 We highly recommend to use GPU to speed up segmentation. To use your NVIDIA GPU, the first step is to download the dedicated driver from [NVIDIA].
 
 Next we need to remove the CPU version of torch:
 
 ```
```

### Comparing `cut-detector-0.0.8/README.md` & `cut-detector-0.0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -25,34 +25,47 @@
 
 ### Conda environment
 
 It is highly recommended to create a dedicated conda environment, by following these few steps:
 
 1. Install an [Anaconda] distribution of Python. Note you might need to use an anaconda prompt if you did not add anaconda to the path.
 
-2. Open an Anaconda prompt as admin to create a new environment using [conda]. We advice to use python 3.10 and conda 23.10.0, to get conda-libmamba-solver as default solver. Note than openjdk is necessary to call Fiji from python, which is needed as you will see below.
+2. Open an Anaconda prompt as admin to create a new environment using [conda]. We advice to use python 3.10 and conda 23.10.0, to get conda-libmamba-solver as default solver.
 
 ```
 conda create --name cut_detector python=3.10 conda=23.10.0
 conda activate cut_detector
-conda install -c conda-forge openjdk=8
 ```
 
 ### Package installation
 
 Once in a dedicated environment, our package can be installed via [pip]:
 
 ```
 pip install cut_detector
 ```
 
+Alternatively, you can clone the github repo to access to playground scripts.
+
+```
+git clone https://github.com/15bonte/cut-detector.git
+cd cut-detector
+pip install -e .
+```
+
 ### Fiji
 
 This package relies on [Trackmate] to perform cell tracking. Trackmate is called through [Fiji], which has to be installed independently. Please follow the steps [here](https://imagej.net/software/fiji/downloads) to install it.
 
+Next, install openjdk which is necessary to call Fiji from python.
+
+```
+conda install -c conda-forge openjdk=8
+```
+
 ### GPU
 
 We highly recommend to use GPU to speed up segmentation. To use your NVIDIA GPU, the first step is to download the dedicated driver from [NVIDIA].
 
 Next we need to remove the CPU version of torch:
 
 ```
```

### Comparing `cut-detector-0.0.8/playground/segmentation.py` & `cut-detector-0.0.9/playground/segmentation.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,56 +4,55 @@
 import matplotlib.pyplot as plt
 from cellpose import models
 
 from cnn_framework.utils.readers.tiff_reader import TiffReader
 
 from cut_detector.data.tools import get_data_path
 from cut_detector.models.tools import get_model_path
-from cut_detector.constants.tracking import (
-    AUGMENT,
-    CELLPROB_THRESHOLD,
-    FLOW_THRESHOLD,
+from cut_detector.factories.segmentation_tracking_factory import (
+    SegmentationTrackingFactory,
 )
 
 
 def main(
     image_path: Optional[str] = get_data_path("videos"),
-    model_path: Optional[str] = get_model_path("segmentation_model"),
+    model_path: Optional[str] = os.path.join(
+        get_model_path("segmentation"), "segmentation_model"
+    ),
     diameter=0,  # 0 means using segmentation model saved value
     channel_to_segment=3,  # index starts at 1
     nucleus_channel=0,  # 0 means no nucleus channel
-    cellprob_threshold=CELLPROB_THRESHOLD,
-    flow_treshold=FLOW_THRESHOLD,
-    augment=AUGMENT,
 ):
     """
     Script to run simple cellpose segmentation.
     """
     # If image_path or model_path are directories, take their first file
     if os.path.isdir(image_path):
         image_path = os.path.join(image_path, os.listdir(image_path)[0])
     if os.path.isdir(model_path):
         model_path = os.path.join(model_path, os.listdir(model_path)[0])
 
     # Read image and preprocess if needed
     image = TiffReader(image_path).image  # TCZYX
 
-    device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
+    # Initialize factory to get constants
+    factory = SegmentationTrackingFactory(model_path)
 
+    device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
     model = models.CellposeModel(pretrained_model=[model_path], device=device)
 
     for frame in range(image.shape[0]):
         frame_image = image[frame, ...].squeeze()
         results, flows, _ = model.eval(
             [frame_image],
             channels=[channel_to_segment, nucleus_channel],
             diameter=diameter,
-            flow_threshold=flow_treshold,
-            cellprob_threshold=cellprob_threshold,
-            augment=augment,
+            flow_threshold=factory.flow_threshold,
+            cellprob_threshold=factory.cellprob_threshold,
+            augment=factory.augment,
         )
 
         # Plot image_to_segment and segmented_image
         _, ax = plt.subplots(2, 2)
         ax[0, 0].set_title("Raw image")
         ax[0, 0].imshow(frame_image[channel_to_segment - 1], cmap="gray")
         ax[0, 1].set_title("Cellpose")
```

### Comparing `cut-detector-0.0.8/pyproject.toml` & `cut-detector-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cut-detector-0.0.8/setup.cfg` & `cut-detector-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 [options]
 packages = find:
 install_requires = 
 	cellpose>=2.2.3  # to get augment in command line
 	pyimagej
 	scyjava
 	numpy<=1.24
-	cnn_framework==0.0.11
+	cnn_framework==0.0.15
 	magicgui
 	pydantic==1.10.12
 	xmltodict
 	shapely
 	aicsimageio
 	scikit-learn==1.2.2
 	charset-normalizer==3.3.0
```

### Comparing `cut-detector-0.0.8/src/cut_detector/_tests/test_mid_body_detection.py` & `cut-detector-0.0.9/src/cut_detector/_tests/test_micro_tubules_cut_detection.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 import os
 from skimage import io
 
-from cut_detector._widget import mid_body_detection
+from cut_detector._widget import micro_tubules_cut_detection
 from cut_detector.data.tools import get_data_path
+from cut_detector.widget_functions.mt_cut_detection import (
+    perform_mt_cut_detection,
+)
 
 
-def test_open_mid_body_detection_widget():
+def test_open_micro_tubules_cut_detection_widget():
     # Just try to open the widget
-    mid_body_detection()
+    micro_tubules_cut_detection()
 
 
-def test_mid_body_detection_widget(make_napari_viewer_proxy):
-    viewer = make_napari_viewer_proxy()
+def test_micro_tubules_cut_detection():
 
     # Add video
-    video = io.imread(os.path.join(get_data_path("videos"), "example_video.tif"))
-    viewer.add_image(video, name="example_video")
-
-    # Open the widget
-    widget = mid_body_detection()
-
-    # Run process
-    widget(viewer.layers[0], get_data_path("mitoses"), get_data_path("tracks"), False, "")
+    video = io.imread(
+        os.path.join(get_data_path("videos"), "example_video.tif")  # TYXC
+    )
+
+    perform_mt_cut_detection(
+        video,
+        "example_video",
+        get_data_path("mitoses"),
+        update_mitoses=False,
+    )
```

### Comparing `cut-detector-0.0.8/src/cut_detector/_widget.py` & `cut-detector-0.0.9/src/cut_detector/_widget.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,10 @@
-"""
-This module is an example of a barebones QWidget plugin for napari
-
-It implements the Widget specification.
-see: https://napari.org/stable/plugins/guides.html?#widgets
-
-Replace code below according to your needs.
-"""
 import os
 from pathlib import Path
-from typing import TYPE_CHECKING
+from typing import Optional
 
 from magicgui import magic_factory
 import tempfile
 
 
 from .utils.tools import re_organize_channels
 
@@ -20,17 +12,14 @@
 from .widget_functions.mid_body_detection import perform_mid_body_detection
 from .widget_functions.mitosis_track_generation import (
     perform_mitosis_track_generation,
 )
 from .widget_functions.mt_cut_detection import perform_mt_cut_detection
 from .widget_functions.save_results import perform_results_saving
 
-if TYPE_CHECKING:
-    import napari
-
 
 @magic_factory(
     call_button="Run Whole Process",
     layout="vertical",
     fiji_dir=dict(
         widget_type="FileEdit",
         label="Fiji path (likely named Fiji.app): ",
@@ -204,16 +193,16 @@
         label="Directory to save .bin tracks: ",
         mode="d",
     ),
 )
 def mitosis_track_generation(
     img_layer: "napari.layers.Image",
     xml_model_dir: str,
-    mitoses_save_dir: str,
-    tracks_save_dir: str,
+    mitoses_save_dir: Optional[str],
+    tracks_save_dir: Optional[str],
 ):
     raw_video = re_organize_channels(img_layer.data)  # TXYC
     perform_mitosis_track_generation(
         raw_video,
         img_layer.name,
         xml_model_dir,
         mitoses_save_dir,
@@ -271,15 +260,19 @@
         mode="d",
     ),
 )
 def micro_tubules_cut_detection(
     img_layer: "napari.layers.Image", exported_mitoses_dir: str
 ):
     raw_video = re_organize_channels(img_layer.data)  # TXYC
-    perform_mt_cut_detection(raw_video, img_layer.name, exported_mitoses_dir)
+    perform_mt_cut_detection(
+        raw_video,
+        img_layer.name,
+        exported_mitoses_dir,
+    )
     print("\nMicro-tubules cut detection finished with success!")
 
 
 @magic_factory(
     call_button="Save results",
     layout="vertical",
     exported_mitoses_dir=dict(
```

### Comparing `cut-detector-0.0.8/src/cut_detector/constants/annotations.py` & `cut-detector-0.0.9/src/cut_detector/constants/annotations.py`

 * *Files identical despite different names*

### Comparing `cut-detector-0.0.8/src/cut_detector/data/tools.py` & `cut-detector-0.0.9/src/cut_detector/data/tools.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,31 +12,39 @@
     if data_name == "mitoses":
         files = ["example_video_mitosis_0_4_to_0.bin"]
     elif data_name == "models":
         files = ["example_video_model.xml"]
     elif data_name == "tracks":
         sub_folder_to_create = f"{data_name}/example_video"
         files = [
-            "example_video/track_0.bin",
-            "example_video/track_1.bin",
-            "example_video/track_2.bin",
-            "example_video/track_3.bin",
-            "example_video/track_4.bin",
+            f"example_video/track_{track_id}.bin" for track_id in range(5)
         ]
     elif data_name == "results":
         files = []  # no files to download here
     elif data_name == "videos":
         files = ["example_video.tif"]
+    elif data_name == "mitosis_movies":
+        files = ["example_video_mitosis_0_0_to_4.tiff"]
+    elif data_name == "mid_bodies":
+        files = []  # no files to download here
+    elif data_name == "segmentation_results":
+        files = ["example_video.bin"]
+    elif data_name == "spots":
+        sub_folder_to_create = f"{data_name}/example_video"
+        files = [f"example_video/spot_{spot_id}.bin" for spot_id in range(237)]
+    elif data_name == "annotations":
+        sub_folder_to_create = f"{data_name}/example_video"
+        files = [
+            "example_video/CellCounter_example_video_mitosis_0_0_to_4.xml"
+        ]
     else:
         raise ValueError(f"Unknown data name: {data_name}")
 
     local_path = os.path.join(CURRENT_DIR, data_name)
-
-    if sub_folder_to_create is not None:
-        os.makedirs(os.path.join(CURRENT_DIR, sub_folder_to_create), exist_ok=True)
+    os.makedirs(os.path.join(CURRENT_DIR, sub_folder_to_create), exist_ok=True)
 
     for file in files:
         file_local_path = os.path.join(local_path, file)
         if not os.path.exists(file_local_path):
             print(f"Downloading data {data_name}...")
             urllib.request.urlretrieve(
                 f"https://raw.githubusercontent.com//15bonte/cut-detector-models/main/data/{data_name}/{file}",
```

### Comparing `cut-detector-0.0.8/src/cut_detector/factories/mid_body_detection_factory.py` & `cut-detector-0.0.9/src/cut_detector/factories/mid_body_detection_factory.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 import os
+from random import shuffle
 from typing import Optional
 import numpy as np
-from bigfish import stack, detection, plot
+from bigfish import stack, detection
 from skimage.morphology import extrema, opening
 from scipy import ndimage
 from scipy.optimize import linear_sum_assignment
+import matplotlib as mpl
 
 from cnn_framework.utils.display_tools import display_progress
 
 from ..constants.tracking import CYTOKINESIS_DURATION
 from ..utils.mid_body_track import MidBodyTrack
 from ..utils.image_tools import smart_cropping
 from ..utils.mid_body_spot import MidBodySpot
 from ..utils.mitosis_track import MitosisTrack
 from ..utils.trackmate_track import TrackMateTrack
+from ..utils.tools import plot_detection
 
 
 class MidBodyDetectionFactory:
     """
     Class to perform mid-body detection, tracking and filtering.
 
     Args:
@@ -57,54 +60,54 @@
 
     def update_mid_body_spots(
         self,
         mitosis_track: MitosisTrack,
         mitosis_movie: np.array,
         mask_movie: np.array,
         tracks: list[TrackMateTrack],
-        path_output: Optional[str] = None,
     ) -> None:
         """
         Get spots of best mitosis track.
 
         Parameters
         ----------
-        mitosis_movie: (T, H, W, C)
-        mask_movie: (T, H, W)
+        mitosis_movie: TYXC
+        mask_movie: TYX
 
         """
 
-        spots_candidates = self._detect_mid_body_spots(
-            mitosis_movie, mask_movie=mask_movie, path_output=path_output
+        spots_candidates = self.detect_mid_body_spots(
+            mitosis_movie, mask_movie=mask_movie
+        )
+        mid_body_tracks = self.generate_tracks_from_spots(spots_candidates)
+        kept_track = self._select_best_track(
+            mitosis_track, mid_body_tracks, tracks, mitosis_movie
         )
-        mid_body_tracks = self._generate_tracks_from_spots(spots_candidates)
-        kept_track = self._select_best_track(mitosis_track, mid_body_tracks, tracks, mitosis_movie)
 
         if kept_track is None:
             return
 
         # Keep only spots of best mitosis track
         for rel_frame, spot in kept_track.spots.items():
             frame = rel_frame + mitosis_track.min_frame
             mitosis_track.mid_body_spots[frame] = spot
 
-    def _detect_mid_body_spots(
+    def detect_mid_body_spots(
         self,
         mitosis_movie: np.array,
         mask_movie: Optional[np.array] = None,
         mid_body_channel=1,
         sir_channel=0,
-        path_output: Optional[str] = None,
         mode="h_maxima",
     ) -> dict[int, list[MidBodySpot]]:
         """
         Parameters
         ----------
-        mitosis_movie: (T, H, W, C)
-        mask_movie: (T, H, W)
+        mitosis_movie: TYXC
+        mask_movie: TYX
 
         Returns
         ----------
         spots_dictionary: dict[int, list[MidBodySpot]]
         """
 
         # Default mask is all ones
@@ -118,39 +121,37 @@
             display_progress(
                 "Detect mid-body spots...",
                 frame + 1,
                 nb_frames,
                 additional_message=f"Frame {frame + 1}/{nb_frames}",
             )
 
-            mitosis_frame = mitosis_movie[frame, :, :, :].squeeze()  # H, W, C
-            mask_frame = mask_movie[frame, :, :].squeeze()  # H, W
-            spots = self.spot_detection(
+            mitosis_frame = mitosis_movie[frame, :, :, :].squeeze()  # YXC
+            mask_frame = mask_movie[frame, :, :].squeeze()  # YX
+            spots = self._spot_detection(
                 mitosis_frame,
                 mask_frame,
                 mid_body_channel,
                 sir_channel,
-                path_output=path_output,
                 mode=mode,
                 frame=frame,
             )
 
             # Update dictionary
             spots_dictionary[frame] = spots
 
         return spots_dictionary
 
-    def spot_detection(
+    def _spot_detection(
         self,
         image: np.array,
         mask: np.array,
         mid_body_channel: int,
         sir_channel: int,
-        path_output: Optional[str] = None,
-        mode="bigfish",
+        mode: str,
         frame=-1,
     ) -> list[MidBodySpot]:
         """
         Mode 'bigfish'
             threshold_1: sigma for log filter
             threshold_2: threshold for spots detection
 
@@ -162,30 +163,35 @@
 
         image_sir = image[:, :, sir_channel]
         image_mklp = image[:, :, mid_body_channel]  #
 
         if mode == "bigfish":
             # Spots detection with bigfish functions
             filtered_image = stack.log_filter(image_mklp, sigma=self.sigma)
-            filtered_image = image_mklp
             # Filter out spots which are not maximal or outside convex hull
             spots_mask = (filtered_image > 0) * mask
             # If mask is empty, skip frame
             if np.sum(spots_mask) == 0:
-                spots = np.array([], dtype=np.int64).reshape((0, filtered_image.ndim))
+                spots = np.array([], dtype=np.int64).reshape(
+                    (0, filtered_image.ndim)
+                )
             else:
                 spots, _ = detection.spots_thresholding(
-                    filtered_image, spots_mask.astype(np.bool), threshold=self.threshold
+                    filtered_image,
+                    spots_mask.astype(bool),
+                    threshold=self.threshold,
                 )
 
         elif mode == "h_maxima":
             # Perform opening followed by closing to remove small spots
             filtered_image = opening(image_mklp, footprint=np.ones((3, 3)))
             # Get local maxima using h_maxima
-            local_maxima = extrema.h_maxima(filtered_image, self.h_maxima_threshold)
+            local_maxima = extrema.h_maxima(
+                filtered_image, self.h_maxima_threshold
+            )
             # Label spot regions
             labeled_local_maxima, nb_labels = ndimage.label(
                 local_maxima, structure=np.ones((3, 3))
             )
             # Remove inconsistent labels
             # Threshold is computed as 99th percentile of image
             filtering_threshold = np.quantile(image_mklp.flatten(), 0.99)
@@ -205,62 +211,58 @@
                 local_maxima, labeled_local_maxima, range(1, nb_labels + 1)
             )
             spots = np.asarray(spots, dtype=np.int64)
 
             # Here, do something to retrieve mid_body area and/or circularity...
 
             if len(spots) == 0:
-                spots = np.array([], dtype=np.int64).reshape((0, filtered_image.ndim))
+                spots = np.array([], dtype=np.int64).reshape(
+                    (0, filtered_image.ndim)
+                )
 
         else:
             raise ValueError(f"Unknown mode: {mode}")
 
-        if path_output is not None:
-            # Check if directory exists
-            if not os.path.exists(path_output):
-                os.makedirs(path_output)
-            # Count number of files in directory
-            nb_files = len(os.listdir(path_output))
-            plot.plot_detection(
-                filtered_image,
-                spots,
-                contrast=True,
-                path_output=os.path.join(path_output, f"spot_detection_{nb_files+1}.png"),
-                show=False,
-            )
-
         # Convert spots to MidBodySpot objects (switch (y, x) to (x, y))
         mid_body_spots = [
             MidBodySpot(
                 frame,
-                (position[1], position[0]),
+                x=position[1],
+                y=position[0],
                 intensity=self._get_average_intensity(position, image_mklp),
                 sir_intensity=self._get_average_intensity(position, image_sir),
             )
             for position in spots
         ]
 
         return mid_body_spots
 
     @staticmethod
-    def _get_average_intensity(position: tuple[int], image: np.array, margin=1) -> int:
+    def _get_average_intensity(
+        position: tuple[int], image: np.array, margin=1
+    ) -> int:
         """
         Parameters
         ----------
         position: (y, x)
-        image: (H, W)
+        image: YX
         margin: int
 
         Returns
         ----------
         average_intensity: int
         """
         # Get associated crop
         crop = smart_cropping(
-            image, margin, position[1], position[0], position[1] + 1, position[0] + 1
+            image,
+            margin,
+            position[1],
+            position[0],
+            position[1] + 1,
+            position[0] + 1,
         )
 
         # Return average intensity
         return int(np.mean(crop))
 
     def _update_spots_hereditary(
         self, spots1: list[MidBodySpot], spots2: list[MidBodySpot]
@@ -270,15 +272,17 @@
         """
         # Ignore empty spots list
         if len(spots1) == 0 or len(spots2) == 0:
             return
 
         # Create cost matrix
         # https://imagej.net/plugins/trackmate/algorithms
-        cost_matrix = np.zeros((len(spots1) + len(spots2), len(spots1) + len(spots2)))
+        cost_matrix = np.zeros(
+            (len(spots1) + len(spots2), len(spots1) + len(spots2))
+        )
         max_cost = 0
         for i, spot1 in enumerate(spots1):
             for j, spot2 in enumerate(spots2):
                 intensity_penalty = (
                     3
                     * self.weight_mklp_intensity_factor
                     * np.abs(spot1.intensity - spot2.intensity)
@@ -287,38 +291,46 @@
                 sir_intensity_penalty = (
                     3
                     * self.weight_sir_intensity_factor
                     * np.abs(spot1.sir_intensity - spot2.sir_intensity)
                     / (spot1.sir_intensity + spot2.sir_intensity)
                 )
                 penalty = 1 + intensity_penalty + sir_intensity_penalty
-                distance = np.linalg.norm(np.array(spot1.position) - np.array(spot2.position))
+                distance = spot1.distance_to(spot2)
                 if distance > self.mid_body_linking_max_distance:
                     cost_matrix[i, j] = np.inf
                 else:
                     # Compared to original TrackMate algorithm, remove square to penalize no attribution to the closest spot
                     cost_matrix[i, j] = (penalty * distance) ** 1
                     max_cost = max(max_cost, cost_matrix[i, j])
 
-        min_cost = 0 if np.max(cost_matrix) == 0 else np.min(cost_matrix[np.nonzero(cost_matrix)])
+        min_cost = (
+            0
+            if np.max(cost_matrix) == 0
+            else np.min(cost_matrix[np.nonzero(cost_matrix)])
+        )
 
-        cost_matrix[len(spots1) :, : len(spots2)] = max_cost * 1.05  # bottom left
-        cost_matrix[: len(spots1), len(spots2) :] = max_cost * 1.05  # top right
+        cost_matrix[len(spots1) :, : len(spots2)] = (
+            max_cost * 1.05
+        )  # bottom left
+        cost_matrix[: len(spots1), len(spots2) :] = (
+            max_cost * 1.05
+        )  # top right
         cost_matrix[len(spots1) :, len(spots2) :] = min_cost  # bottom right
 
         # Hungarian algorithm
         row_ind, col_ind = linear_sum_assignment(cost_matrix)
 
         # Update parent and child spots
         for i, j in zip(row_ind, col_ind):
             if i < len(spots1) and j < len(spots2):
                 spots1[i].child_spot = spots2[j]
                 spots2[j].parent_spot = spots1[i]
 
-    def _generate_tracks_from_spots(
+    def generate_tracks_from_spots(
         self, spots_candidates: dict[int, list[MidBodySpot]]
     ) -> list[MidBodyTrack]:
         """
         Use spots linked together to generate tracks.
 
         Parameters
         ----------
@@ -331,97 +343,130 @@
         """
 
         # Update parent and child spots
         for frame in spots_candidates.keys():
             # Ignore if no spot detected in next frame
             if not frame + 1 in spots_candidates:
                 continue
-            self._update_spots_hereditary(spots_candidates[frame], spots_candidates[frame + 1])
+            self._update_spots_hereditary(
+                spots_candidates[frame], spots_candidates[frame + 1]
+            )
 
         tracks = []
         for spots in spots_candidates.values():
             for spot in spots:
                 if spot.track_id is None:
                     # Create new track
                     track_id = len(tracks)
                     new_track = MidBodyTrack(track_id)
                     new_track.add_spot(spot)
                     tracks.append(new_track)
+
         return tracks
 
     def _select_best_track(
         self,
         mitosis_track: MitosisTrack,
         mid_body_tracks: list[MidBodyTrack],
         trackmate_tracks: list[TrackMateTrack],
         mitosis_movie: np.array,
         sir_channel=0,
     ) -> MidBodyTrack:
         """
         Select best track from mid-body tracks.
+
+        Parameters
+        ----------
+        mitosis_movie: TYXC
         """
-        mother_track, daughter_tracks = mitosis_track.get_mother_daughters_tracks(trackmate_tracks)
+        (
+            mother_track,
+            daughter_tracks,
+        ) = mitosis_track.get_mother_daughters_tracks(trackmate_tracks)
         # NB: only first daughter is considered
         daughter_track = daughter_tracks[0]
 
         expected_positions = {}
-        for frame in range(daughter_track.start, daughter_track.start + self.cytokinesis_duration):
+        for frame in range(
+            daughter_track.start,
+            daughter_track.start + self.cytokinesis_duration,
+        ):
             # If one cell does not exist anymore, stop
-            if frame not in daughter_track.track_spots or frame not in mother_track.track_spots:
+            if (
+                frame not in daughter_track.spots
+                or frame not in mother_track.spots
+            ):
                 continue
             # Compute mid-body expected relative position at current frame
             closest_points = []
             min_distance = np.inf
-            for mother_point in mother_track.track_spots[frame].spot_points:
+            for mother_point in mother_track.spots[frame].spot_points:
                 position_mother = [
                     int(mother_point[0]) - mitosis_track.position.min_x,
                     int(mother_point[1]) - mitosis_track.position.min_y,
                 ]
-                for daughter_point in daughter_track.track_spots[frame].spot_points:
+                for daughter_point in daughter_track.spots[frame].spot_points:
                     position_daughter = [
                         int(daughter_point[0]) - mitosis_track.position.min_x,
                         int(daughter_point[1]) - mitosis_track.position.min_y,
                     ]
                     distance = np.linalg.norm(
-                        [a - b for a, b in zip(position_mother, position_daughter)]
+                        [
+                            a - b
+                            for a, b in zip(position_mother, position_daughter)
+                        ]
                     )
                     if distance < min_distance:
                         min_distance = distance
                         closest_points = [(position_mother, position_daughter)]
                     if distance == min_distance:
-                        closest_points.append((position_mother, position_daughter))
+                        closest_points.append(
+                            (position_mother, position_daughter)
+                        )
 
             mid_body_position = np.mean(closest_points, axis=0)
             mid_body_position = np.mean(mid_body_position, axis=0)
-            expected_positions[frame - mitosis_track.min_frame] = mid_body_position
+            expected_positions[frame - mitosis_track.min_frame] = (
+                mid_body_position
+            )
 
         # Remove wrong tracks by keeping only tracks with at least minimum_track_length points
         mid_body_tracks = [
-            track for track in mid_body_tracks if track.length > self.minimum_mid_body_track_length
+            track
+            for track in mid_body_tracks
+            if track.length > self.minimum_mid_body_track_length
         ]
 
         # Compute mean intensity on sir-tubulin channel for each track
-        image_sir = mitosis_movie[:, :, :, sir_channel]
+        image_sir = mitosis_movie[..., sir_channel]  # TYX
         sir_intensity_track = [0 for _ in mid_body_tracks]
         for idx, track in enumerate(mid_body_tracks):
             abs_track_frames = [
-                frame + mitosis_track.min_frame for frame in list(track.spots.keys())
+                frame + mitosis_track.min_frame
+                for frame in list(track.spots.keys())
             ]
-            abs_min_frame = mitosis_track.key_events_frame["cytokinesis"]  # Cytokinesis start
+            abs_min_frame = mitosis_track.key_events_frame[
+                "cytokinesis"
+            ]  # Cytokinesis start
             abs_max_frame = abs_min_frame + int(self.cytokinesis_duration / 2)
-            if abs_min_frame > abs_track_frames[-1] or abs_max_frame < abs_track_frames[0]:
+            if (
+                abs_min_frame > abs_track_frames[-1]
+                or abs_max_frame < abs_track_frames[0]
+            ):
                 sir_intensity_track[idx] = -np.inf
             frame_count = 0
             for frame in range(abs_min_frame, abs_max_frame + 1):
                 if frame not in abs_track_frames:
                     continue
                 frame_count += 1
-                track_position = track.spots[frame - mitosis_track.min_frame].position
+                track_spot = track.spots[frame - mitosis_track.min_frame]
                 sir_intensity_track[idx] += image_sir[
-                    frame - mitosis_track.min_frame, track_position[1], track_position[0]
+                    frame - mitosis_track.min_frame,
+                    track_spot.y,
+                    track_spot.x,
                 ]
 
             if frame_count < (abs_max_frame - abs_min_frame + 1) / 2:
                 sir_intensity_track[idx] = -np.inf
             else:
                 sir_intensity_track[idx] /= frame_count
 
@@ -450,7 +495,57 @@
             fun_values.append(func_sir_intensity(track))
             if func_sir_intensity(track) != np.inf:
                 final_tracks.append(track)
 
         # Sort tracks by func value
         sorted_tracks = sorted(final_tracks, key=func_sir_intensity)
         return sorted_tracks[0] if len(sorted_tracks) > 0 else None
+
+    def save_mid_body_tracking(
+        self,
+        spots_candidates,
+        mitosis_movie: np.ndarray,
+        path_output: str,
+        mid_body_channel=1,
+    ):
+        """
+        Plot spots detection & tracking.
+        """
+        # Check if directory exists
+        if not os.path.exists(path_output):
+            os.makedirs(path_output)
+
+        matplotlib_colors = [
+            mpl.colormaps["hsv"](i)[:3] for i in np.linspace(0, 0.9, 100)
+        ]
+        shuffle(matplotlib_colors)
+
+        # Detect spots in each frame
+        nb_frames = mitosis_movie.shape[0]
+        for frame in range(nb_frames):
+            image = mitosis_movie[frame, :, :, mid_body_channel].squeeze()
+
+            # Bigfish spots
+            frame_spots = [
+                [spot.y, spot.x] for spot in spots_candidates[frame]
+            ]
+            colors = [
+                (
+                    matplotlib_colors[spot.track_id % len(matplotlib_colors)]
+                    if spot.track_id is not None
+                    else (0, 0, 0)
+                )
+                for spot in spots_candidates[frame]
+            ]
+
+            plot_detection(
+                image,
+                frame_spots,
+                color=colors,
+                contrast=True,
+                path_output=os.path.join(
+                    path_output, f"spot_detection_{frame}.png"
+                ),
+                show=False,
+                title=f"Python frame {frame} - Fiji frame {frame + 1}",
+                fill=True,
+            )
```

### Comparing `cut-detector-0.0.8/src/cut_detector/factories/tracks_merging_factory.py` & `cut-detector-0.0.9/src/cut_detector/factories/tracks_merging_factory.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,29 @@
 import json
 import os
 import numpy as np
 import xmltodict
-import torch
-from torch.utils.data import DataLoader
 
-from cnn_framework.utils.model_managers.cnn_model_manager import (
-    CnnModelManager,
-)
-from cnn_framework.utils.data_managers.default_data_manager import (
-    DefaultDataManager,
-)
-from cnn_framework.utils.metrics.classification_accuracy import (
-    ClassificationAccuracy,
-)
-from cnn_framework.utils.data_loader_generators.data_loader_generator import (
-    collate_dataset_output,
-)
-from cnn_framework.utils.enum import PredictMode
-
-from ..utils.mitosis_track import MitosisTrack
+from ..utils.cell_track import CellTrack
 from ..utils.trackmate_spot import TrackMateSpot
+from ..utils.tools import perform_cnn_inference
+from ..utils.mitosis_track import MitosisTrack
+from ..utils.cell_spot import CellSpot
 from ..utils.trackmate_track import TrackMateTrack
 from ..utils.trackmate_frame_spots import TrackMateFrameSpots
 from ..utils.hidden_markov_models import HiddenMarkovModel
-from ..utils.cell_division_detection.metaphase_cnn_data_set import (
-    MetaphaseCnnDataSet,
-)
-from ..utils.cell_division_detection.metaphase_cnn import MetaphaseCnn
 from ..utils.cell_division_detection.metaphase_cnn_model_params import (
     MetaphaseCnnModelParams,
 )
 
 
-def get_track_from_id(
-    tracks: list[TrackMateTrack], track_id: int
-) -> TrackMateTrack:
+def get_track_from_id(tracks: list[CellTrack], track_id: int) -> CellTrack:
+    """
+    Used to get track from its id.
+    """
     for track in tracks:
         if track.track_id == track_id:
             return track
     raise ValueError(f"Track {track_id} not found")
 
 
 class TracksMergingFactory:
@@ -60,15 +44,15 @@
     ) -> None:
         self.min_track_spots = min_track_spots
         self.minimum_metaphase_interval = minimum_metaphase_interval
         self.max_spot_distance_for_split = max_spot_distance_for_split
 
     def read_trackmate_xml(
         self, xml_model_path: str, raw_video_shape: np.ndarray
-    ) -> None:
+    ) -> tuple[list[TrackMateTrack], list[TrackMateSpot]]:
         """
         Read useful information from xml file.
         """
         if not os.path.exists(xml_model_path):
             print("No xml file found for this video.")
             return None, None
         with open(xml_model_path) as fd:
@@ -83,48 +67,54 @@
                     TrackMateTrack(track)
                     for track in doc["TrackMate"]["Model"]["AllTracks"][
                         "Track"
                     ]
                 ],
             )
         )
-        raw_spots = [
+        raw_frames_spots = [
             TrackMateFrameSpots(spots, raw_video_shape)
             for spots in doc["TrackMate"]["Model"]["AllSpots"]["SpotsInFrame"]
         ]
+        # Merge all frames - to get rid of TrackMateFrameSpots
+        spots = [
+            spot
+            for raw_frame_spots in raw_frames_spots
+            for spot in raw_frame_spots.spots
+        ]
 
-        return trackmate_tracks, raw_spots
+        return trackmate_tracks, spots
 
     def get_tracks_to_merge(
-        self, raw_tracks: list[TrackMateTrack]
+        self, raw_tracks: list[CellTrack]
     ) -> list[MitosisTrack]:
         """
         Plug tracks occurring at frame>0 to closest metaphase.
         """
-        ordered_tracks = sorted(raw_tracks, key=lambda x: x.track_start)
+        ordered_tracks = sorted(raw_tracks, key=lambda x: x.start)
         mitosis_tracks: list[MitosisTrack] = []
 
         # Loop through all tracks beginning at frame > 0 and try to plug them to the previous metaphase
         for track in reversed(ordered_tracks):
             # Break when reaching tracking starting at first frame, as they are ordered
-            track_first_frame = min(track.track_spots.keys())
+            track_first_frame = min(track.spots.keys())
             if track_first_frame == 0:
                 break
 
             # Get all spots at same frame
             contemporary_spots = [
-                raw_track.track_spots[track_first_frame]
+                raw_track.spots[track_first_frame]
                 for raw_track in raw_tracks
-                if track_first_frame in raw_track.track_spots
+                if track_first_frame in raw_track.spots
                 and raw_track.track_id != track.track_id
             ]
 
             # Keep only stuck spots
-            first_spot = track.track_spots[track_first_frame]
-            stuck_spots: list[TrackMateSpot] = list(
+            first_spot = track.spots[track_first_frame]
+            stuck_spots: list[CellSpot] = list(
                 filter(
                     lambda x: x.is_stuck_to(
                         first_spot, self.max_spot_distance_for_split
                     ),
                     contemporary_spots,
                 )
             )
@@ -205,16 +195,16 @@
                 corrected_sequence[
                     list(range(metaphase_index[idx - 1], metaphase_index[idx]))
                 ] = 1
         return corrected_sequence
 
     def pre_process_spots(
         self,
-        trackmate_tracks: list[TrackMateTrack],
-        raw_spots: list[TrackMateFrameSpots],
+        trackmate_tracks: list[CellTrack],
+        raw_spots: list[CellSpot],
         raw_video: np.array,
         metaphase_model_path: str,
         hmm_metaphase_parameters_file: str,
         predictions_file: str,
         video_name: str,
         only_predictions_update: bool,
     ) -> None:
@@ -267,83 +257,44 @@
         )
 
     @staticmethod
     def _predict_metaphase_spots(
         metaphase_model_path: str, nuclei_crops: list[np.array]
     ) -> list[int]:
         """
-        Run CNN model to predict metaphase spots
+        Run CNN model to predict metaphase spots.
 
         Parameters
         ----------
-        metaphase_model: CNN model path
-        nuclei_crops: [C, H, W]
+        metaphase_model : str
+            CNN model path
+        nuclei_crops :  list[np.array]
+            list[CYX]
 
         Returns
         -------
-        predictions: [class predicted]
+        predictions : list[int]
+            predicted classes
         """
 
-        # Metaphase model parameters
-        model_parameters = MetaphaseCnnModelParams()
-        # Modify parameters for training
-        model_parameters.train_ratio = 0
-        model_parameters.val_ratio = 0
-        model_parameters.test_ratio = 1
-
-        # Model definition
-        # Load pretrained model
-        model = MetaphaseCnn(nb_classes=model_parameters.nb_classes)
-
-        map_location = None
-        if not torch.cuda.is_available():
-            map_location = torch.device("cpu")
-            print("No GPU found, using CPU.")
-        model.load_state_dict(
-            torch.load(
-                metaphase_model_path,
-                map_location=map_location,
-            )
-        )
-
-        # Test (no sampler to keep order)
-        dataset_test = MetaphaseCnnDataSet(
-            nuclei_crops,
-            is_train=False,
-            names=[f"{idx}.ext" for idx in range(len(nuclei_crops))],
-            data_manager=DefaultDataManager(""),
-            params=model_parameters,
+        predictions = perform_cnn_inference(
+            model_path=metaphase_model_path,
+            images=nuclei_crops,
+            cnn_model_params=MetaphaseCnnModelParams,
         )
-        test_dl = DataLoader(
-            dataset_test,
-            batch_size=128,
-            collate_fn=collate_dataset_output,
-        )
-
-        manager = CnnModelManager(
-            model, model_parameters, ClassificationAccuracy
-        )
-
-        predictions = manager.predict(
-            test_dl,
-            predict_mode=PredictMode.GetPrediction,
-            nb_images_to_save=0,
-        )  # careful, this is scores and not probabilities
-        predictions = [int(np.argmax(p)) for p in predictions]
-
         return predictions
 
     @staticmethod
     def update_predictions_file(
-        tracks: list[TrackMateTrack], predictions_file: str, video_name: str
+        tracks: list[CellTrack], predictions_file: str, video_name: str
     ) -> None:
         """
         Parameters
         ----------
-        tracks: [TrackMateTrack]
+        tracks: [CellTrack]
         predictions_file: str
         video_name: str
         """
         if predictions_file is None:
             return
 
         # Read data from json prediction if exists
@@ -352,16 +303,15 @@
                 predictions_data = json.load(json_file)
         else:
             predictions_data = {}
 
         # Retrieve predictions
         predictions = {
             int(track.track_id): [
-                int(spot.predicted_phase)
-                for spot in track.track_spots.values()
+                int(spot.predicted_phase) for spot in track.spots.values()
             ]
             for track in tracks
         }
         predictions_data[video_name] = predictions
         # Save predictions data
         with open(predictions_file, "w") as json_file:
             json.dump(predictions_data, json_file)
```

### Comparing `cut-detector-0.0.8/src/cut_detector/napari.yaml` & `cut-detector-0.0.9/src/cut_detector/napari.yaml`

 * *Files identical despite different names*

### Comparing `cut-detector-0.0.8/src/cut_detector/utils/box_dimensions.py` & `cut-detector-0.0.9/src/cut_detector/utils/box_dimensions.py`

 * *Files identical despite different names*

### Comparing `cut-detector-0.0.8/src/cut_detector/utils/cell_division_detection/metaphase_cnn_data_set.py` & `cut-detector-0.0.9/src/cut_detector/utils/cnn_data_set.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,50 @@
 import numpy as np
 import albumentations as A
 
 from cnn_framework.utils.data_sets.abstract_data_set import AbstractDataSet
 from cnn_framework.utils.data_sets.dataset_output import DatasetOutput
-from cnn_framework.utils.preprocessing import normalize_array
+from cnn_framework.utils.tools import handle_image_type
 
 
-class MetaphaseCnnDataSet(AbstractDataSet):
+class CnnDataSet(AbstractDataSet):
     """
     Custom class to avoid loading images from folder.
     """
 
     def __init__(self, data, *args, **kwargs):
-        # Not pythonic, but needed as super init calls generate_raw_images
-        self.data = data
         super().__init__(*args, **kwargs)
+        self.data = data
 
     def set_transforms(self):
         height, width = self.params.input_dimensions.to_tuple(False)
         self.transforms = A.Compose(
             [
+                A.Normalize(
+                    self.mean_std["mean"],
+                    std=self.mean_std["std"],
+                    max_pixel_value=1,
+                ),
                 A.PadIfNeeded(
                     min_height=height,
                     min_width=width,
                     border_mode=0,
                     value=0,
                     p=1,
                 ),
                 A.CenterCrop(height=height, width=width, p=1),
             ]
         )
 
-    def generate_raw_images(self, filename):
+    def generate_images(self, filename):
         idx = int(filename.split(".")[0])
-        nucleus_image = normalize_array(self.data[idx], None)  # C, H, W
-        nucleus_image = np.moveaxis(nucleus_image, 0, -1)  # H, W, C
+        # Get image and adapt it to torch
+        nucleus_image = np.moveaxis(self.data[idx], 0, -1)  # YXC
+        nucleus_image = handle_image_type(nucleus_image)  # to [0, 1]
+        # Define any target value
+        target_array = np.zeros(self.params.nb_classes)
+        target_array[0] = 1
+        # Construct output
         return DatasetOutput(
-            input=nucleus_image, target_array=np.asarray([0, 1, 0])
+            input=nucleus_image,
+            target_array=target_array,
         )
```

### Comparing `cut-detector-0.0.8/src/cut_detector/utils/cell_division_detection/metaphase_cnn_model_params.py` & `cut-detector-0.0.9/src/cut_detector/utils/cell_division_detection/metaphase_cnn_model_params.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,15 +8,16 @@
     """
 
     def __init__(self):
         super().__init__("metaphase_cnn")
 
         self.input_dimensions = Dimensions(height=256, width=256)
 
-        self.num_epochs = 50
-        self.learning_rate = 0.1
-
         self.nb_classes = 3
         self.class_names = ["Interphase", "Metaphase", "Death"]
 
         self.c_indexes = [0, 1, 2]
         self.z_indexes = [0]
+
+        self.batch_size = 128
+
+        self.encoder_name = "resnet18"
```

### Comparing `cut-detector-0.0.8/src/cut_detector/utils/image_tools.py` & `cut-detector-0.0.9/src/cut_detector/utils/image_tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,20 @@
     # Define margins for both sides
     pad_margin_w_left = abs(desired_width - width) // 2
     pad_margin_w_right = abs(desired_width - width) - pad_margin_w_left
 
     pad_margin_h_top = abs(desired_height - height) // 2
     pad_margin_h_bottom = abs(desired_height - height) - pad_margin_h_top
 
-    return pad_margin_w_left, pad_margin_h_top, pad_margin_w_right, pad_margin_h_bottom
+    return (
+        pad_margin_w_left,
+        pad_margin_h_top,
+        pad_margin_w_right,
+        pad_margin_h_bottom,
+    )
 
 
 def resize_padding(image, output_shape, mode, pad_margin_w, pad_margin_h):
     """
     mode: "min" or "zero"
     """
     channels_to_stack = []
@@ -39,15 +44,17 @@
     if height > desired_height:
         image = crop_center(image, (depth, desired_height, width))
         height = desired_height
     if width > desired_width:
         image = crop_center(image, (depth, height, desired_width))
         width = desired_width
 
-    raw_padding = get_padding(image.shape, output_shape)  # left, top, right and bottom
+    raw_padding = get_padding(
+        image.shape, output_shape
+    )  # left, top, right and bottom
 
     # Define margins for both sides
     if pad_margin_w is None:
         pad_margin_w_left = raw_padding[0]
         pad_margin_w_right = raw_padding[2]
     else:
         pad_margin_w_left, pad_margin_w_right = pad_margin_w
@@ -88,16 +95,16 @@
     image,
     output_shape=None,
     method="zero",
     pad_margin_w=None,
     pad_margin_h=None,
 ):
     """
-    Expect image to be a 3D numpy array (C, H, W).
-    Output_shape is a tuple (C, H, W).
+    Expect image to be a 3D numpy array CYX.
+    Output_shape is a tuple CYX.
     """
 
     if method == "min" or method == "zero":
         # Compute output_shape
         if output_shape is None:
             if pad_margin_h is None or pad_margin_w is None:
                 raise ValueError(
@@ -111,15 +118,17 @@
                 )
         # Protect against output_shape and margins inconsistency
         if output_shape is not None and pad_margin_h is not None:
             assert sum(pad_margin_h) == output_shape[1] - image.shape[1]
         if output_shape is not None and pad_margin_w is not None:
             assert sum(pad_margin_w) == output_shape[2] - image.shape[2]
         # Pad to required_dimensions
-        return resize_padding(image, output_shape, method, pad_margin_w, pad_margin_h)
+        return resize_padding(
+            image, output_shape, method, pad_margin_w, pad_margin_h
+        )
 
     raise ValueError(f"Unknown resize method: {method}")
 
 
 def smart_cropping(
     microscopy_image,
     margin,
@@ -128,15 +137,15 @@
     max_x=None,
     max_y=None,
     fade_margin=False,
     pad=False,
 ):
     """
     Crop microscopy image with smart margin.
-    microscopy_image: ..., H, W
+    microscopy_image: ..., YX
     """
 
     # Get image shape
     height, width = microscopy_image.shape[-2:]
 
     # Define empty rectangle if single point is given
     if max_x is None:
@@ -148,15 +157,17 @@
     clipped_min_y = max(min_y - margin, 0)
     clipped_max_y = min(max_y + margin, height)
     clipped_min_x = max(min_x - margin, 0)
     clipped_max_x = min(max_x + margin, width)
 
     # Crop image
     clipped_image = np.copy(
-        microscopy_image[..., clipped_min_y:clipped_max_y, clipped_min_x:clipped_max_x]
+        microscopy_image[
+            ..., clipped_min_y:clipped_max_y, clipped_min_x:clipped_max_x
+        ]
     )
 
     # Fade margin
     if fade_margin:
         margin_positions = (
             [
                 [y, x]
@@ -186,15 +197,24 @@
             )
 
     # Pad if necessary
     if pad and clipped_image.shape[-1] * clipped_image.shape[-2] != (
         max_x - min_x + 2 * margin
     ) * (max_y - min_y + 2 * margin):
         # Compute padding
-        pad_margin_h = (clipped_min_y - (min_y - margin), max_y + margin - clipped_max_y)
-        pad_margin_w = (clipped_min_x - (min_x - margin), max_x + margin - clipped_max_x)
+        pad_margin_h = (
+            clipped_min_y - (min_y - margin),
+            max_y + margin - clipped_max_y,
+        )
+        pad_margin_w = (
+            clipped_min_x - (min_x - margin),
+            max_x + margin - clipped_max_x,
+        )
         # Pad
         clipped_image = resize_image(
-            clipped_image, pad_margin_h=pad_margin_h, pad_margin_w=pad_margin_w, method="zero"
+            clipped_image,
+            pad_margin_h=pad_margin_h,
+            pad_margin_w=pad_margin_w,
+            method="zero",
         )
 
     return clipped_image
```

### Comparing `cut-detector-0.0.8/src/cut_detector/utils/mid_body_track.py` & `cut-detector-0.0.9/src/cut_detector/utils/mid_body_track.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,26 @@
+from __future__ import annotations
+from typing import Callable, Optional
 import numpy as np
 
+from .track import Track
 from .mid_body_spot import MidBodySpot
 
 
-class MidBodyTrack:
+class MidBodyTrack(Track[MidBodySpot]):
     """
     Mid-body candidate track
     """
 
-    def __init__(self, track_id: int):
-        self.track_id = track_id
-        self.spots: dict[int, MidBodySpot] = {}
-        self.length = 0
+    max_frame_gap = 2
 
     def add_spot(self, spot: MidBodySpot) -> None:
+        """
+        Add spot to track.
+        """
         self.spots[spot.frame] = spot
         spot.track_id = self.track_id
         self.length += 1
         # Add children recursively
         if spot.child_spot is not None:
             self.add_spot(spot.child_spot)
 
@@ -28,17 +31,31 @@
         Compute the average distance between mid-body expected positions and current
         track positions.
         """
         distances = []
         for frame, position in expected_positions.items():
             if frame not in self.spots:
                 continue
+            spot = self.spots[frame]
             distances.append(
-                np.linalg.norm(np.array(self.spots[frame].position) - np.array(position))
+                np.linalg.norm(spot.get_position() - np.array(position))
             )
         # If there are no frames in common, for sure track is not the right one
         if len(distances) == 0:
             return np.inf
         mean_distance = np.mean(distances)
         if mean_distance > max_distance:
             return np.inf
         return mean_distance
+
+    @staticmethod
+    def generate_tracks_from_spots(
+        spots: dict[int, list[MidBodySpot]],
+        linking_max_distance: int,
+        gap_closing_max_distance: int = None,
+        track_dist_metric: str | Callable = "sqeuclidean",
+    ) -> list[MidBodyTrack]:
+        """
+        Generate tracks from spots.
+        """
+        max_frame_gap = MidBodyTrack.max_frame_gap
+        raise NotImplementedError
```

### Comparing `cut-detector-0.0.8/src/cut_detector/utils/mitosis_track.py` & `cut-detector-0.0.9/src/cut_detector/utils/mitosis_track.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,14 +45,15 @@
         self.mother_track_id = mother_track_id
         self.daughter_track_ids = [daughter_track_id]
         self.id: Optional[int] = None
 
         self.metaphase_frame = metaphase_frame
 
         # Key events: metaphase/cytokinesis/first_mt_cut/second_mt_cut/first_membrane_cut
+        # Absolute frame
         self.key_events_frame: dict[str, Union[int, ImpossibleDetection]] = {}
         self.gt_key_events_frame: Optional[dict[str, int]] = None
 
         # Time
         self.min_frame: Optional[int] = None
         self.max_frame: Optional[int] = None
 
@@ -138,32 +139,34 @@
         self.min_frame = min_frame
         self.max_frame = max_frame
 
     def update_is_near_border(self, raw_video: np.array) -> None:
         """
         Parameters
         ----------
-        raw_video: np.array  # (T, H, W, C)
-        ----------
+        raw_video: np.array
+            TYXC
+
         """
 
         max_height, max_width = raw_video.shape[1], raw_video.shape[2]
 
         cyto_frame = self.key_events_frame["cytokinesis"]
         last_frame = cyto_frame + CYTOKINESIS_DURATION
 
         # get mitosis coordinates between cyto_frame and last_frame
         min_dist_to_border = np.inf
         for frame in range(cyto_frame, last_frame + 1):
             if frame not in self.mid_body_spots:
                 continue
 
             # get mid-body coordinates
-            x_rel = self.mid_body_spots[frame].position[0]
-            y_rel = self.mid_body_spots[frame].position[1]
+            mid_body_frame = self.mid_body_spots[frame]
+            x_rel = mid_body_frame.x
+            y_rel = mid_body_frame.y
 
             x_abs = x_rel + self.position.min_x
             y_abs = y_rel + self.position.min_y
             mid_body_coordinates = (x_abs, y_abs)
 
             # get distance to border
             min_x = min(
@@ -184,20 +187,17 @@
         mother_track, daughter_tracks = self.get_mother_daughters_tracks(
             trackmate_tracks
         )
 
         # Store first metaphase frame
         for frame in range(self.metaphase_frame, mother_track.start, -1):
             # Some frames may be missing since gap closing is allowed
-            if frame not in mother_track.track_spots:
+            if frame not in mother_track.spots:
                 continue
-            if (
-                mother_track.track_spots[frame].predicted_phase
-                != METAPHASE_INDEX
-            ):
+            if mother_track.spots[frame].predicted_phase != METAPHASE_INDEX:
                 self.key_events_frame["metaphase"] = frame + 1
                 break
 
         # If no metaphase frame found, consider it is the first frame of the mother track
         if "metaphase" not in self.key_events_frame:
             self.key_events_frame["metaphase"] = mother_track.start
 
@@ -232,22 +232,24 @@
 
     def generate_video_movie(
         self, raw_video: np.array
     ) -> Tuple[np.array, np.array]:
         """
         Parameters
         ----------
-        raw_video: initial video (T, H, W, C)
-        ----------
+        raw_video : np.array
+            initial video, TYXC
 
         Returns
         ----------
-        mitosis_movie: mitosis movie (T, H, W, C)
-        mask_movie: mask movie (T, H, W, C) (all channels are actually the same)
-        ----------
+        mitosis_movie : np.array
+            mitosis movie, TYXC
+        mask_movie : np.array
+            mask movie, TYX
+
         """
 
         mitosis_movie, mask_movie = [], []
         for frame in range(self.min_frame, self.max_frame + 1):
             # Get useful data for current frame
             min_x = self.dln_positions[frame].min_x
             max_x = self.dln_positions[frame].max_x
@@ -257,50 +259,55 @@
 
             # Extract frame image, big enough to keep all spots for current track
             frame_image = raw_video[
                 frame,
                 self.position.min_y : self.position.max_y,
                 self.position.min_x : self.position.max_x,
                 :,
-            ]  # H, W, C
+            ]  # YXC
 
             # Generate mask with Delaunay triangulation
             current_frame_shape = (
                 max_y - min_y,
                 max_x - min_x,
             )  # current spot
             indices = np.stack(np.indices(current_frame_shape), axis=-1)
             out_idx = np.nonzero(dln.find_simplex(indices) + 1)
             single_channel_mask = np.zeros(current_frame_shape)
             single_channel_mask[out_idx] = 1
 
             # Construct mask image
             mask_image = np.stack(
                 [single_channel_mask] * raw_video.shape[-1], axis=0
-            )  # C, H, W
+            )  # CYX
             mask_image = resize_image(
                 mask_image,
                 method="zero",
                 pad_margin_h=[
                     min_y - self.position.min_y,
                     self.position.max_y - max_y,
                 ],
                 pad_margin_w=[
                     min_x - self.position.min_x,
                     self.position.max_x - max_x,
                 ],
             )[
                 0, ...
-            ]  # H, W
+            ]  # YX
 
             mitosis_movie.append(frame_image)
             mask_movie.append(mask_image)
 
-        mitosis_movie = np.array(mitosis_movie)  # T, H, W, C
-        mask_movie = np.array(mask_movie)  # T, H, W
+        mitosis_movie = np.array(mitosis_movie)  # TYXC
+        mask_movie = np.array(mask_movie)  # TYX
+
+        # If mid-bodies are already computed, add them to the mitosis movie
+        if self.mid_body_spots:
+            mitosis_movie = self.add_mid_body_movie(mitosis_movie, mask_movie)
+            return mitosis_movie[..., :-1], mitosis_movie[..., -1].squeeze()
 
         return mitosis_movie, mask_movie
 
     def generate_mitosis_summary(
         self, raw_tracks: list[TrackMateTrack], save_path: str
     ) -> None:
         """
@@ -312,25 +319,22 @@
         mother_track, daughter_tracks = self.get_mother_daughters_tracks(
             raw_tracks
         )
         daughters_first_frame = min([track.start for track in daughter_tracks])
 
         for idx, frame in enumerate(range(self.min_frame, self.max_frame + 1)):
             # Extreme case where mother track is not present at beginning of mitosis movie
-            if frame not in mother_track.track_spots:
+            if frame not in mother_track.spots:
                 mitosis_summary[idx + 1] = "interphase"
                 continue
             # Telophase defined as first frame after metaphase or daughters first frame
             if frame >= self.metaphase_frame or frame >= daughters_first_frame:
                 mitosis_summary[idx + 1] = "telophase"
             # Metaphase according to CNN + HMM prediction
-            elif (
-                mother_track.track_spots[frame].predicted_phase
-                == METAPHASE_INDEX
-            ):
+            elif mother_track.spots[frame].predicted_phase == METAPHASE_INDEX:
                 mitosis_summary[idx + 1] = "metaphase"
             # In other cases, interphase
             else:
                 mitosis_summary[idx + 1] = "interphase"
 
         # Save mitosis summary
         with open(save_path, "w") as f:
@@ -352,51 +356,47 @@
 
     def add_mid_body_movie(
         self, mitosis_movie: np.array, mask_movie: np.array
     ) -> np.array:
         """
         Parameters
         ----------
-        mitosis_movie: (T, H, W, C)
-        mask_movie: (T, H, W)
+        mitosis_movie: TYXC
+        mask_movie: TYX
 
         Returns
         ----------
-        spots_video: (T, H, W, 1)
+        spots_video: TYX C=1
         """
 
         video_shape = mitosis_movie.shape[:3]
-        spots_video = np.zeros(video_shape)  # T, H, W
+        spots_video = np.zeros(video_shape)  # TYX
 
         for absolute_frame, spot in self.mid_body_spots.items():
             # Create 1 circle around spot position
             square_size = 2
             spots_video[
                 absolute_frame - self.min_frame,
-                spot.position[1]
-                - square_size : spot.position[1]
-                + square_size,
-                spot.position[0]
-                - square_size : spot.position[0]
-                + square_size,
+                spot.y - square_size : spot.y + square_size,
+                spot.x - square_size : spot.x + square_size,
             ] = 1
 
         # Add empty dimension at end
-        mid_body_movie = np.expand_dims(spots_video, axis=-1)  # (T, H, W, 1)
+        mid_body_movie = np.expand_dims(spots_video, axis=-1)  # TYX C=1
 
         # Mix mid-body and mask movie
-        mask_movie = np.expand_dims(mask_movie, axis=-1)  # (T, H, W, 1)
-        mid_body_mask_movie = mask_movie + mid_body_movie  # (T, H, W, 1)
+        mask_movie = np.expand_dims(mask_movie, axis=-1)  # TYX C=1
+        mid_body_mask_movie = mask_movie + mid_body_movie  # TYX C=1
 
         # Cast mid_body_mask_movie to mitosis_movie dtype
         mid_body_mask_movie = mid_body_mask_movie.astype(mitosis_movie.dtype)
 
         mitosis_movie = np.concatenate(
             [mitosis_movie, mid_body_mask_movie], axis=-1
-        )  # (T, H, W, C+1)
+        )  # TYX C=C+1
 
         return mitosis_movie
 
     def update_mid_body_ground_truth(
         self, annotation_file: str, nb_channels: int
     ) -> None:
         """
@@ -436,15 +436,15 @@
                     int(marker.MarkerY),
                     cell_counter_frame_to_video_frame(
                         int(marker.MarkerZ), nb_channels
                     ),
                 )
                 # Create associated spot
                 self.gt_mid_body_spots[frame + self.min_frame] = MidBodySpot(
-                    frame, (x_pos, y_pos)
+                    frame, x=x_pos, y=y_pos
                 )
 
             # If Name is missing of wrong, assume it is i
             if (
                 "Name" not in type_data
                 or type_data.Name not in NAMES_DICTIONARY
             ):
@@ -463,43 +463,43 @@
                 "first_mt_cut" not in self.gt_key_events_frame
                 and class_index in get_class_ids_after_first_mt_cut()
             ):
                 assert (
                     class_abs_first_frame
                     >= self.gt_key_events_frame["cytokinesis"]
                 )  # after metaphase
-                self.gt_key_events_frame[
-                    "first_mt_cut"
-                ] = class_abs_first_frame
+                self.gt_key_events_frame["first_mt_cut"] = (
+                    class_abs_first_frame
+                )
 
             # Second MT cut
             if (
                 "second_mt_cut" not in self.gt_key_events_frame
                 and class_index in get_class_ids_after_second_mt_cut()
             ):
                 assert (
                     class_abs_first_frame
                     >= self.gt_key_events_frame["first_mt_cut"]
                 )  # after first MT cut
-                self.gt_key_events_frame[
-                    "second_mt_cut"
-                ] = class_abs_first_frame
+                self.gt_key_events_frame["second_mt_cut"] = (
+                    class_abs_first_frame
+                )
 
             # First membrane cut
             if (
                 "first_membrane_cut" not in self.gt_key_events_frame
                 and class_index in get_class_ids_after_first_membrane_cut()
             ):
                 assert (
                     class_abs_first_frame
                     >= self.gt_key_events_frame["first_mt_cut"]
                 )  # after first MT cut
-                self.gt_key_events_frame[
-                    "first_membrane_cut"
-                ] = class_abs_first_frame
+                self.gt_key_events_frame["first_membrane_cut"] = (
+                    class_abs_first_frame
+                )
 
     def evaluate_mid_body_detection(
         self, tolerance=10, percent_seen=0.9
     ) -> bool:
         """
         Mid_body is considered as detected if during at least percent_seen % of frames
         between cytokinesis and second MT cut it is at most tolerance pixels away
@@ -523,17 +523,16 @@
         for frame in range(self.gt_key_events_frame["cytokinesis"], max_frame):
             if frame not in self.gt_mid_body_spots:
                 continue
             if frame not in self.mid_body_spots:
                 position_difference.append(1e3)  # random huge value
                 continue
             position_difference.append(
-                np.linalg.norm(
-                    np.array(self.gt_mid_body_spots[frame].position)
-                    - np.array(self.mid_body_spots[frame].position)
+                self.gt_mid_body_spots[frame].distance_to(
+                    self.mid_body_spots[frame]
                 )
             )
 
         # Get percent_seen th percentile of position difference
         position_difference = np.array(position_difference)
         max_position_difference = np.quantile(
             position_difference, percent_seen
@@ -602,23 +601,24 @@
             frame = first_cut_frame + i
 
             # Make sure mid-body exists at frame
             if not self.mid_body_spots or frame not in self.mid_body_spots:
                 continue
 
             # Get mid-body coordinates
-            x_pos, y_pos = self.mid_body_spots[frame].position
+            mid_body_frame = self.mid_body_spots[frame]
+            x_pos, y_pos = mid_body_frame.x, mid_body_frame.y
 
             # Extract image and crop on the midbody
-            img = np.transpose(video[frame, ...], (2, 0, 1))  # C, H, W
+            img = np.transpose(video[frame, ...], (2, 0, 1))  # CYX
             crop = smart_cropping(
                 img, crop_size_light_spot, x_pos, y_pos, pad=True
             )[
                 0, ...
-            ]  # H, W
+            ]  # YX
 
             # Perform opening to remove small spots and apply h_maxima to get potential spots
             filtered_image = opening(crop, footprint=np.ones((3, 3)))
             local_maxima = extrema.h_maxima(
                 filtered_image, h_maxima_light_spot
             )
 
@@ -675,7 +675,79 @@
             print("frame_counted: ", frame_counted)
             print("spot_detected: ", spot_detected)
             print(
                 f"Track: {self.id}_{self.mother_track_id}_to_{','.join(str(daughter) for daughter in self.daughter_track_ids)}"
             )
 
         return spot_detected
+
+    def get_bridge_images(
+        self, video: np.array, margin: int
+    ) -> list[np.array]:
+        """
+        Generate list of crops around the mid-body.
+        First frame is the maximum of cytokinesis frame and mid-body first frame.
+        Last frame is the last mid-body frame.
+
+        Parameters
+        ----------
+        video: np.array
+            TYXC
+        margin: int
+            number of pixels to keep around the mid-body, in all directions
+
+        Returns
+        ----------
+        bridge_images: list[np.array]
+            list of crops around the mid-body, TCYX
+        """
+
+        ordered_mb_frames = sorted(self.mid_body_spots.keys())
+        first_mb_frame = ordered_mb_frames[0]
+        last_mb_frame = ordered_mb_frames[-1]
+        first_frame = max(
+            first_mb_frame, self.key_events_frame["cytokinesis"] - 2
+        )  # -2?
+
+        bridge_images = []
+        for frame in range(first_frame, last_mb_frame + 1):
+            min_x = self.position.min_x
+            min_y = self.position.min_y
+
+            # Get midbody coordinates
+            frame_mid_body = self.mid_body_spots[frame]
+            x_pos, y_pos = min_x + frame_mid_body.x, min_y + frame_mid_body.y
+
+            # Extract frame image and crop around the midbody Sir-tubulin
+            frame_image = (
+                video[frame, :, :, :].squeeze().transpose(2, 0, 1)
+            )  # CYX
+            crop = smart_cropping(
+                frame_image, margin, x_pos, y_pos, pad=True
+            )  # CYX
+            bridge_images.append(crop)
+
+        return bridge_images
+
+    def adapt_deprecated_attributes(self) -> None:
+        """
+        Used to adapt deprecated attributes to new ones.
+        In particular, x and y instead of position for mid_body_spots.
+        """
+        # Predicted
+        for mid_body_spot in self.mid_body_spots.values():
+            if (
+                hasattr(mid_body_spot, "position")
+                and mid_body_spot.position is not None
+            ):
+                mid_body_spot.x = mid_body_spot.position[0]
+                mid_body_spot.y = mid_body_spot.position[1]
+        # Ground truth
+        if self.gt_mid_body_spots is None:
+            return
+        for mid_body_spot in self.gt_mid_body_spots.values():
+            if (
+                hasattr(mid_body_spot, "position")
+                and mid_body_spot.position is not None
+            ):
+                mid_body_spot.x = mid_body_spot.position[0]
+                mid_body_spot.y = mid_body_spot.position[1]
```

### Comparing `cut-detector-0.0.8/src/cut_detector/utils/trackmate_track.py` & `cut-detector-0.0.9/src/cut_detector/utils/cell_track.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,143 +1,160 @@
 from __future__ import annotations
+
 from typing import Optional, Tuple
 from scipy.spatial import ConvexHull, Delaunay
 import numpy as np
 
+
 from ..constants.tracking import (
     FRAMES_AROUND_METAPHASE,
     INTERPHASE_INDEX,
     METAPHASE_INDEX,
-    MAX_FRAME_GAP,
 )
-from .box_dimensions import BoxDimensions
+from .track import Track
 from .box_dimensions_dln import BoxDimensionsDln
-from .trackmate_spot import TrackMateSpot
-from .trackmate_frame_spots import TrackMateFrameSpots
+from .box_dimensions import BoxDimensions
+from .cell_spot import CellSpot
 
 
 def get_whole_box_dimensions_dln(
-    tracks: list[TrackMateTrack], frame: int
+    tracks: list[CellTrack], frame: int
 ) -> Tuple[BoxDimensionsDln, list[list[int]]]:
+    """
+    Merge different tracks.
+
+    Parameters
+    ----------
+    predictions : list[int]
+        list of predictions for each frame of the track.
+
+    Returns
+    -------
+    BoxDimensionsDln : Box dimension of merged tracks.
+    list[list[int]] : List of box dimension coordinates for all tracks.
+
+    """
     box_dimensions_dln = BoxDimensionsDln()
     track_frame_points = []
 
     # For all tracks: mother and daughter(s)
     for track in tracks:
-        if frame in track.track_spots:
-            current_spot = track.track_spots[frame]
+        if frame in track.spots:
+            current_spot = track.spots[frame]
             track_frame_points = track_frame_points + current_spot.spot_points
             box_dimensions_dln.update(
                 current_spot.abs_min_x,
                 current_spot.abs_max_x,
                 current_spot.abs_min_y,
                 current_spot.abs_max_y,
             )
     return box_dimensions_dln, track_frame_points
 
 
-class TrackMateTrack:
+class CellTrack(Track[CellSpot]):
     """
-    Parse TrackMate track from xml file.
+    Cell track.
     """
 
-    def __init__(self, trackmate_track):
-        self.track_start = int(float(trackmate_track["@TRACK_START"]))
-        self.track_id = int(trackmate_track["@TRACK_ID"])
-
-        self.track_spots_ids: set[int] = set()
-
-        if isinstance(trackmate_track["Edge"], dict):  # only one edge
-            self.track_spots_ids.add(
-                int(trackmate_track["Edge"]["@SPOT_SOURCE_ID"])
-            )
-            self.track_spots_ids.add(
-                int(trackmate_track["Edge"]["@SPOT_TARGET_ID"])
-            )
-        else:
-            for edge in trackmate_track["Edge"]:
-                self.track_spots_ids.add(int(edge["@SPOT_SOURCE_ID"]))
-                self.track_spots_ids.add(int(edge["@SPOT_TARGET_ID"]))
-
-        self.start = int(float(trackmate_track["@TRACK_START"]))
-        self.stop = int(float(trackmate_track["@TRACK_STOP"]))
-
-        self.track_spots: dict[
-            int, TrackMateSpot
-        ] = {}  # {frame: TrackMateSpot}
-        self.metaphase_spots: list[TrackMateSpot] = []
+    max_frame_gap = 3
 
-        # Can be different from len(self.track_spots) if we have a gap in the track
-        self.number_spots = 0
+    def __init__(
+        self, track_id: int, track_spots_ids: set[int], start: int, stop: int
+    ) -> None:
+        super().__init__(track_id)
+        self.track_spots_ids = track_spots_ids
+        self.start = start
+        self.stop = stop
+
+        self.metaphase_spots: list[CellSpot] = []
 
     def update_metaphase_spots(self, predictions: list[int]) -> None:
         """
         Populate metaphase_spots with candidates.
 
         Parameters
         ----------
         predictions : list[int]
             list of predictions for each frame of the track.
 
+        Returns
+        -------
+        None.
+
         """
-        for idx, frame in enumerate(sorted(self.track_spots.keys())):
-            self.track_spots[frame].predicted_phase = predictions[idx]
+        for idx, frame in enumerate(sorted(self.spots.keys())):
+            self.spots[frame].predicted_phase = predictions[idx]
 
         # Store last metaphase spot of each group
         metaphase_finished = False
         for frame in range(self.start, self.stop + 1):
             # Ignore first spots of cell as they are metaphase only if end of previous metaphase
             if predictions[frame - self.start] == INTERPHASE_INDEX:
                 metaphase_finished = True
             if not metaphase_finished:
                 continue
 
             # From this point, get metaphase spots
             if (
-                frame in self.track_spots  # current frame contains a spot
+                frame in self.spots  # current frame contains a spot
                 and predictions[frame - self.start]
                 == METAPHASE_INDEX  # current spot is in metaphase
                 and frame != self.stop  # current spot is not last spot
                 and (
                     predictions[frame - self.start + 1] != METAPHASE_INDEX
-                    and frame in self.track_spots
+                    and frame in self.spots
                 )  # next frame is not a spot in metaphase
             ):
-                self.metaphase_spots.append(self.track_spots[frame])
+                self.metaphase_spots.append(self.spots[frame])
 
-    def has_close_metaphase(
-        self, spot: TrackMateSpot, target_frame: int
-    ) -> bool:
+    def has_close_metaphase(self, spot: CellSpot, target_frame: int) -> bool:
         """
-        Returns True if corresponding track contains one metaphase spot close to target frame.
+        Parameters
+        ----------
+        spot : CellSpot
+            Only used to update corresponding metaphase spot.
+
+        Returns
+        -------
+        bool : True if corresponding track contains one metaphase spot close to target frame.
+
         """
         # Look for metaphase spot
         for metaphase_spot in self.metaphase_spots:
             if (
                 abs(metaphase_spot.frame - target_frame)
                 < FRAMES_AROUND_METAPHASE
             ):
                 # Mother track found!
                 spot.corresponding_metaphase_spot = metaphase_spot
                 return True
         return False
 
-    def compute_metaphase_iou(self, daughter_track: TrackMateTrack) -> float:
+    def compute_metaphase_iou(self, daughter_track: CellTrack) -> float:
         """
         Get intersection between daughter area at first frame and self area at previous frame.
-        Get self area at previous frame.
-        Returns the quotient.
+        Get self area at previous frame. Returns the quotient.
 
         Ideally, it should be close to 0.5 as a daughter cell should occupy 50% of the area
         of the mother cell.
 
         May be improved by checking overlap of areas instead of convex hulls.
+
+        Parameters
+        ----------
+        daughter_track : CellTrack
+            Potential daughter track.
+
+        Returns
+        -------
+        float : Intersection Over Union.
+
         """
 
-        daughter_track_first_frame = min(daughter_track.track_spots.keys())
+        daughter_track_first_frame = min(daughter_track.spots.keys())
 
         # If current track starts at first frame, ignore as it cannot be a mother track
         if self.start == daughter_track_first_frame:
             return -1
 
         # Compute two regions
         self_previous_region = self.compute_dln_from_tracks(
@@ -177,17 +194,37 @@
 
         return overlap / previous_area
 
     def compute_dln_from_tracks(
         self,
         frame: int,
         previous_box_dimensions_dln: Optional[BoxDimensionsDln] = None,
-        additional_tracks: Optional[list[TrackMateTrack]] = None,
+        additional_tracks: Optional[list[CellTrack]] = None,
         relative: bool = True,
     ) -> BoxDimensionsDln:
+        """
+        Compute Delaunay triangulation at given frame.
+
+        Parameters
+        ----------
+        frame : int
+            Frame at which Delaunay triangulation is computed.
+        previous_box_dimensions_dln : Optional[BoxDimensionsDln] = None
+            If specified and current track has no spot at frame, no computation is done
+            and previous_box_dimensions_dln is returned.
+        additional_tracks : Optional[list[CellTrack]] = None
+            If specified, perform computation on both current track and these additional tracks.
+        relative : bool = True
+            If True, indexes are relative to current track position.
+
+        Returns
+        -------
+        BoxDimensionsDln : Track(s) Delaunay triangulation.
+
+        """
         tracks = [self]
         if additional_tracks is not None:
             tracks = tracks + additional_tracks
 
         box_dimensions_dln, track_frame_points = get_whole_box_dimensions_dln(
             tracks, frame
         )
@@ -195,27 +232,27 @@
         # If missing spot at this frame...
         if box_dimensions_dln.is_empty():
             # ... use previous frame data if provided
             if previous_box_dimensions_dln:
                 return previous_box_dimensions_dln
 
             # ... or try with previous frame if not
-            for _ in range(MAX_FRAME_GAP):
+            for _ in range(CellTrack.max_frame_gap):
                 frame = frame - 1
                 (
                     box_dimensions_dln,
                     track_frame_points,
                 ) = get_whole_box_dimensions_dln(tracks, frame)
                 if not box_dimensions_dln.is_empty():
                     break
 
         # Should not be empty after this loop
         if box_dimensions_dln.is_empty():
             raise ValueError(
-                f"No previous dln & Tracks with no spots in {MAX_FRAME_GAP} frames in a row"
+                f"No previous dln & Tracks with no spots in {CellTrack.max_frame_gap} frames in a row"
             )
 
         # Else, compute convex hull and Delaunay triangulation
         # Switch dimensions
         if relative:
             track_frame_points = [
                 [y - box_dimensions_dln.min_y, x - box_dimensions_dln.min_x]
@@ -228,62 +265,73 @@
         box_dimensions_dln.dln = Delaunay(
             np.array(track_frame_points)[hull.vertices]
         )
 
         return box_dimensions_dln
 
     def get_spots_data(
-        self, raw_spots: list[TrackMateFrameSpots], raw_video: np.array
+        self, raw_spots: list[CellSpot], raw_video: np.array
     ) -> list[np.array]:
         """
-        Parse xml data to assign spots at corresponding track.
-        Returns list of nucleus crops for each frame.
+        Generate crops around cells for metaphase CNN inference.
 
         Parameters
         ----------
-        track: TrackMateTrack
-        raw_spots: [TrackMateFrameSpots]
-        raw_video: T, H, W, C
+        raw_spots : list[CellSpot]
+            All video spots.
+        raw_video : np.array
+            TYXC
 
         Returns
         -------
-        nucleus_crops: [C, H, W]
+        list[np.array]: Cell crops (CYX)
+
         """
 
         spot_abs_positions = {}  # {frame: BoxDimensions}
-        nucleus_crops = []  # [C, H, W]
+        cell_crops = []  # CYX
 
-        for frame_spots in raw_spots:
+        for spot in raw_spots:
             # Ignore spots before or after current track
-            if frame_spots.frame < self.start or frame_spots.frame > self.stop:
+            if spot.frame < self.start or spot.frame > self.stop:
                 continue
-            for spot in frame_spots.spots:
-                # Ignore spots not in current track
-                if spot.id not in self.track_spots_ids:
-                    continue
-
-                # Store positions
-                spot_abs_positions[spot.frame] = BoxDimensions(
-                    spot.abs_min_x,
-                    spot.abs_max_x,
-                    spot.abs_min_y,
-                    spot.abs_max_y,
-                )
-                # Store all spots
-                spot.track_id = self.track_id  # add track information
-                self.track_spots[spot.frame] = spot
+            # Ignore spots not in current track
+            if spot.id not in self.track_spots_ids:
+                continue
+            # Store positions
+            spot_abs_positions[spot.frame] = BoxDimensions(
+                spot.abs_min_x,
+                spot.abs_max_x,
+                spot.abs_min_y,
+                spot.abs_max_y,
+            )
+            # Store all spots
+            spot.track_id = self.track_id  # add track information
+            self.spots[spot.frame] = spot
 
         # If no spot in track for current frame, use previous frame position
         for frame in range(self.start, self.stop + 1):
             if frame in spot_abs_positions:
                 min_y, max_y, min_x, max_x = (
                     spot_abs_positions[frame].min_y,
                     spot_abs_positions[frame].max_y,
                     spot_abs_positions[frame].min_x,
                     spot_abs_positions[frame].max_x,
                 )
-            nucleus = raw_video[frame, min_y:max_y, min_x:max_x, :]  # H, W, C
-            nucleus = np.moveaxis(nucleus, -1, 0)  # C, H, W
-            nucleus_crops.append(nucleus)
-
-        self.number_spots = len(nucleus_crops)
-        return nucleus_crops
+            nucleus = raw_video[frame, min_y:max_y, min_x:max_x, :]  # YXC
+            nucleus = np.moveaxis(nucleus, -1, 0)  # CYX
+            cell_crops.append(nucleus)
+
+        self.number_spots = len(cell_crops)
+        return cell_crops
+
+    @staticmethod
+    def generate_tracks_from_spots(
+        spots: dict[int, list[CellSpot]],
+        linking_max_distance: int,
+        gap_closing_max_distance: int,
+    ) -> list[CellTrack]:
+        """
+        Generate tracks from spots.
+        """
+        max_frame_gap = CellTrack.max_frame_gap
+        raise NotImplementedError
```

### Comparing `cut-detector-0.0.8/src/cut_detector/widget_functions/mid_body_detection.py` & `cut-detector-0.0.9/src/cut_detector/widget_functions/mid_body_detection.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,78 +3,89 @@
 from typing import Optional
 import numpy as np
 from aicsimageio.writers import OmeTiffWriter
 
 from ..factories.mid_body_detection_factory import MidBodyDetectionFactory
 
 from ..utils.mitosis_track import MitosisTrack
+from ..utils.trackmate_track import TrackMateTrack
 
 
 def perform_mid_body_detection(
     raw_video: np.ndarray,
     video_name: str,
     exported_mitoses_dir: str,
     exported_tracks_dir: str,
     save_dir: Optional[str] = None,
+    update_mitoses: bool = True,
 ):
     mitosis_tracks: list[MitosisTrack] = []
     # Iterate over "bin" files in exported_mitoses_dir
     for state_path in os.listdir(exported_mitoses_dir):
         # Ignore if not for current video
         if video_name not in state_path:
             continue
         # Load mitosis track
         with open(os.path.join(exported_mitoses_dir, state_path), "rb") as f:
-            mitosis_track = pickle.load(f)
+            mitosis_track: MitosisTrack = pickle.load(f)
+            mitosis_track.adapt_deprecated_attributes()
 
         # Add mitosis track to list
         mitosis_tracks.append(mitosis_track)
 
     # Load trackmate tracks
-    trackmate_tracks = []
+    trackmate_tracks: list[TrackMateTrack] = []
     # Iterate over "bin" files in exported_tracks_dir
     video_exported_tracks_dir = os.path.join(exported_tracks_dir, video_name)
     for state_path in os.listdir(video_exported_tracks_dir):
         # Load mitosis track
-        with open(os.path.join(video_exported_tracks_dir, state_path), "rb") as f:
-            trackmate_track = pickle.load(f)
-
-        # Add trackmate track to list
-        trackmate_tracks.append(trackmate_track)
+        with open(
+            os.path.join(video_exported_tracks_dir, state_path), "rb"
+        ) as f:
+            trackmate_track: TrackMateTrack = pickle.load(f)
+            trackmate_track.adapt_deprecated_attributes()
+            trackmate_tracks.append(trackmate_track)
 
     # Generate movie for each mitosis and save
     mid_body_detector = MidBodyDetectionFactory()
     for i, mitosis_track in enumerate(mitosis_tracks):
         print(f"\nGenerate mitosis movies ({i+1}/{len(mitosis_tracks)})...")
 
         # Generate mitosis movie
         mitosis_movie, mask_movie = mitosis_track.generate_video_movie(
             raw_video
-        )  # (T, H, W, C), (T, H, W)
+        )  # TYXC, TYX
 
         # Search for mid-body in mitosis movie
         mid_body_detector.update_mid_body_spots(
             mitosis_track, mitosis_movie, mask_movie, trackmate_tracks
         )
 
         # Save updated mitosis track
-        daughter_track_ids = ",".join([str(d) for d in mitosis_track.daughter_track_ids])
-        state_path = f"{video_name}_mitosis_{mitosis_track.id}_{mitosis_track.mother_track_id}_to_{daughter_track_ids}.bin"
-        save_path = os.path.join(
-            exported_mitoses_dir,
-            state_path,
-        )
-        with open(save_path, "wb") as f:
-            pickle.dump(mitosis_track, f)
+        if update_mitoses:
+            daughter_track_ids = ",".join(
+                [str(d) for d in mitosis_track.daughter_track_ids]
+            )
+            state_path = f"{video_name}_mitosis_{mitosis_track.id}_{mitosis_track.mother_track_id}_to_{daughter_track_ids}.bin"
+            save_path = os.path.join(
+                exported_mitoses_dir,
+                state_path,
+            )
+            with open(save_path, "wb") as f:
+                pickle.dump(mitosis_track, f)
 
         if save_dir:
             # Save mitosis movie
             final_mitosis_movie = mitosis_track.add_mid_body_movie(
                 mitosis_movie, mask_movie
-            )  # (T, H, W, C+1)
+            )  # TYX C=C+1
             image_save_path = os.path.join(
                 save_dir,
                 f"{video_name}_mitosis_{mitosis_track.id}_{mitosis_track.mother_track_id}_to_{daughter_track_ids}.tiff",
             )
-            # Transpose to match  T, C, H, W
-            final_mitosis_movie = np.transpose(final_mitosis_movie, (0, 3, 1, 2))
-            OmeTiffWriter.save(final_mitosis_movie, image_save_path, dim_order="TCYX")
+            # Transpose to match TCYX
+            final_mitosis_movie = np.transpose(
+                final_mitosis_movie, (0, 3, 1, 2)
+            )
+            OmeTiffWriter.save(
+                final_mitosis_movie, image_save_path, dim_order="TCYX"
+            )
```

### Comparing `cut-detector-0.0.8/src/cut_detector/widget_functions/mitosis_track_generation.py` & `cut-detector-0.0.9/src/cut_detector/widget_functions/mitosis_track_generation.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,31 +2,32 @@
 from typing import Optional, Union
 import pickle
 import numpy as np
 from matplotlib import pyplot as plt
 
 from cnn_framework.utils.display_tools import display_progress
 
-
-from ..utils.trackmate_frame_spots import TrackMateFrameSpots
+from ..utils.cell_spot import CellSpot
 from ..utils.trackmate_track import TrackMateTrack
 from ..factories.tracks_merging_factory import TracksMergingFactory
 from ..models.tools import get_model_path
 from ..utils.mitosis_track import MitosisTrack
 
 
 def plot_predictions_evolution(
-    raw_spots: list[TrackMateFrameSpots],
+    raw_spots: list[CellSpot],
     raw_tracks: list[TrackMateTrack],
     mitosis_tracks: list[MitosisTrack],
 ) -> None:
     # Spots detected by Cellpose
-    detected_spots = {
-        raw_spot.frame: len(raw_spot.spots) for raw_spot in raw_spots
-    }
+    detected_spots = {}
+    for raw_spot in raw_spots:
+        if raw_spot.frame not in detected_spots:
+            detected_spots[raw_spot.frame] = 0
+        detected_spots[raw_spot.frame] += 1
 
     # Mitoses identified by current method, minus ending tracks
     detected_mitoses = {frame: detected_spots[0] for frame in detected_spots}
     max_frame = max(detected_spots.keys())
     for mitosis_track in mitosis_tracks:
         for frame in range(mitosis_track.metaphase_frame, max_frame + 1):
             detected_mitoses[frame] += len(mitosis_track.daughter_track_ids)
@@ -108,53 +109,56 @@
     plt.show()
 
 
 def perform_mitosis_track_generation(
     raw_video: np.ndarray,
     video_name: str,
     xml_model_dir: str,
-    mitoses_save_dir: str,
-    tracks_save_dir: str,
-    metaphase_model_path: Optional[str] = get_model_path("metaphase_model"),
-    hmm_metaphase_parameters_file: Optional[str] = get_model_path(
-        "hmm_metaphase_parameters"
+    mitoses_save_dir: Optional[str] = None,
+    tracks_save_dir: Optional[str] = None,
+    metaphase_model_path: Optional[str] = get_model_path("metaphase_cnn"),
+    hmm_metaphase_parameters_file: Optional[str] = os.path.join(
+        get_model_path("hmm"), "hmm_metaphase_parameters.npz"
     ),
     predictions_file: Optional[str] = None,
     only_predictions_update: bool = False,
     plot_evolution: bool = False,
 ) -> Union[list[MitosisTrack], None]:
     """
     Perform mitosis track generation.
     """
     # Create save_dir if not exists
-    if not os.path.exists(mitoses_save_dir):
+    if mitoses_save_dir is not None and not os.path.exists(mitoses_save_dir):
         os.makedirs(mitoses_save_dir)
 
     # Create video tracks save dir if not exists
-    video_tracks_save_dir = os.path.join(tracks_save_dir, video_name)
-    if not os.path.exists(video_tracks_save_dir):
-        os.makedirs(video_tracks_save_dir)
+    if tracks_save_dir is not None:
+        video_tracks_save_dir = os.path.join(tracks_save_dir, video_name)
+        if not os.path.exists(video_tracks_save_dir):
+            os.makedirs(video_tracks_save_dir)
+    else:
+        video_tracks_save_dir = None
 
     # Create factory instance, where useful functions are defined
     tracks_merging_factory = TracksMergingFactory()
 
     # Read useful information from xml file
     xml_model_path = os.path.join(xml_model_dir, f"{video_name}_model.xml")
-    trackmate_tracks, raw_spots = tracks_merging_factory.read_trackmate_xml(
+    cell_tracks, cell_spots = tracks_merging_factory.read_trackmate_xml(
         xml_model_path, raw_video.shape
     )
 
     # Missing xml file case
-    if trackmate_tracks is None:
+    if cell_tracks is None:
         return None
 
     # Get dictionary of TrackMate spots (from xml file) for each track and detect metaphase spots
     tracks_merging_factory.pre_process_spots(
-        trackmate_tracks,
-        raw_spots,
+        cell_tracks,
+        cell_spots,
         raw_video,
         metaphase_model_path,
         hmm_metaphase_parameters_file,
         predictions_file,
         video_name,
         only_predictions_update,
     )
@@ -162,55 +166,53 @@
     # If the goal is only to update predictions file, stop here
     if only_predictions_update:
         return None
 
     print("\nGet tracks to merge...")
 
     # Plug tracks occurring at frame>0 to closest metaphase
-    mitosis_tracks = tracks_merging_factory.get_tracks_to_merge(
-        trackmate_tracks
-    )
+    mitosis_tracks = tracks_merging_factory.get_tracks_to_merge(cell_tracks)
 
     # Plot predictions evolution
     if plot_evolution:
-        plot_predictions_evolution(raw_spots, trackmate_tracks, mitosis_tracks)
+        plot_predictions_evolution(cell_spots, cell_tracks, mitosis_tracks)
 
     # Update useful attributes for each track
     for i, mitosis_track in enumerate(mitosis_tracks):
         mitosis_track.id = i
-        mitosis_track.update_mitosis_start_end(
-            trackmate_tracks, mitosis_tracks
-        )
-        mitosis_track.update_key_events_frame(trackmate_tracks)
-        mitosis_track.update_mitosis_position_dln(trackmate_tracks)
+        mitosis_track.update_mitosis_start_end(cell_tracks, mitosis_tracks)
+        mitosis_track.update_key_events_frame(cell_tracks)
+        mitosis_track.update_mitosis_position_dln(cell_tracks)
         mitosis_track.update_is_near_border(raw_video)
 
         # Save mitosis track
-        daughter_track_ids = ",".join(
-            [str(d) for d in mitosis_track.daughter_track_ids]
-        )
-        state_path = f"{video_name}_mitosis_{i}_{mitosis_track.mother_track_id}_to_{daughter_track_ids}.bin"
-        save_path = os.path.join(
-            mitoses_save_dir,
-            state_path,
-        )
-        with open(save_path, "wb") as f:
-            pickle.dump(mitosis_track, f)
+        if mitoses_save_dir is not None:
+            daughter_track_ids = ",".join(
+                [str(d) for d in mitosis_track.daughter_track_ids]
+            )
+            state_path = f"{video_name}_mitosis_{i}_{mitosis_track.mother_track_id}_to_{daughter_track_ids}.bin"
+            save_path = os.path.join(
+                mitoses_save_dir,
+                state_path,
+            )
+            with open(save_path, "wb") as f:
+                pickle.dump(mitosis_track, f)
 
         display_progress(
             "Mitosis tracks generation:",
             i + 1,
             len(mitosis_tracks),
-            additional_message=f"Frame {i + 1}/{len(mitosis_tracks)}",
+            additional_message=f"Mitosis {i + 1}/{len(mitosis_tracks)}",
         )
 
-    # Save updated trackmate tracks
-    for trackmate_track in trackmate_tracks:
-        state_path = f"track_{trackmate_track.track_id}.bin"
-        save_path = os.path.join(
-            video_tracks_save_dir,
-            state_path,
-        )
-        with open(save_path, "wb") as f:
-            pickle.dump(trackmate_track, f)
+    # Save updated cell tracks
+    if video_tracks_save_dir is not None:
+        for cell_track in cell_tracks:
+            state_path = f"track_{cell_track.track_id}.bin"
+            save_path = os.path.join(
+                video_tracks_save_dir,
+                state_path,
+            )
+            with open(save_path, "wb") as f:
+                pickle.dump(cell_track, f)
 
     return mitosis_tracks
```

### Comparing `cut-detector-0.0.8/src/cut_detector/widget_functions/mt_cut_detection.py` & `cut-detector-0.0.9/src/cut_detector/widget_functions/mt_cut_detection.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,43 +8,59 @@
 from ..utils.mitosis_track import MitosisTrack
 
 
 def perform_mt_cut_detection(
     raw_video: np.ndarray,
     video_name: str,
     exported_mitoses_dir: str,
-    scaler_path: Optional[str] = get_model_path("svc_scaler"),
-    model_path: Optional[str] = get_model_path("svc_model"),
-    hmm_bridges_parameters_file: Optional[str] = get_model_path("hmm_bridges_parameters"),
+    hmm_bridges_parameters_file: Optional[str] = os.path.join(
+        get_model_path("hmm"), "hmm_bridges_parameters.npz"
+    ),
+    bridges_mt_cnn_model_path: Optional[str] = get_model_path(
+        "bridges_mt_cnn"
+    ),
+    update_mitoses: Optional[bool] = True,
 ):
+    """
+
+    Parameters
+    ----------
+    raw_video: np.ndarray
+        TYXC
+
+    """
     mitosis_tracks: list[MitosisTrack] = []
     # Iterate over "bin" files in exported_mitoses_dir
     for state_path in os.listdir(exported_mitoses_dir):
         # Ignore if not for current video
         if video_name not in state_path:
             continue
         # Load mitosis track
         with open(os.path.join(exported_mitoses_dir, state_path), "rb") as f:
-            mitosis_track = pickle.load(f)
+            mitosis_track: MitosisTrack = pickle.load(f)
+            mitosis_track.adapt_deprecated_attributes()
 
         # Add mitosis track to list
         mitosis_tracks.append(mitosis_track)
 
-    # Generate a list of the first MT cut time for each mitosis track
+    # Perform cut detection
     mt_cut_detector = MtCutDetectionFactory()
-    for i, mitosis_track in enumerate(mitosis_tracks):
-        print(f"Detect MT cut ({i+1}/{len(mitosis_tracks)})...")
-
-        # Perform cut detection
-        mt_cut_detector.update_mt_cut_detection(
-            mitosis_track, raw_video, scaler_path, model_path, hmm_bridges_parameters_file
-        )
+    mt_cut_detector.update_mt_cut_detection(
+        mitosis_tracks,
+        raw_video,
+        hmm_bridges_parameters_file,
+        bridges_mt_cnn_model_path,
+    )
 
+    for mitosis_track in mitosis_tracks:
         # Save updated mitosis track
-        daughter_track_ids = ",".join([str(d) for d in mitosis_track.daughter_track_ids])
-        state_path = f"{video_name}_mitosis_{mitosis_track.id}_{mitosis_track.mother_track_id}_to_{daughter_track_ids}.bin"
-        save_path = os.path.join(
-            exported_mitoses_dir,
-            state_path,
-        )
-        with open(save_path, "wb") as f:
-            pickle.dump(mitosis_track, f)
+        if update_mitoses:
+            daughter_track_ids = ",".join(
+                [str(d) for d in mitosis_track.daughter_track_ids]
+            )
+            state_path = f"{video_name}_mitosis_{mitosis_track.id}_{mitosis_track.mother_track_id}_to_{daughter_track_ids}.bin"
+            save_path = os.path.join(
+                exported_mitoses_dir,
+                state_path,
+            )
+            with open(save_path, "wb") as f:
+                pickle.dump(mitosis_track, f)
```

### Comparing `cut-detector-0.0.8/src/cut_detector/widget_functions/save_results.py` & `cut-detector-0.0.9/src/cut_detector/factories/results_saving_factory.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,326 +1,342 @@
 import os
-import pickle
 from typing import Optional
+from scipy.stats import ttest_1samp
 import numpy as np
 import matplotlib.pyplot as plt
-from scipy.stats import ttest_1samp
 
 from ..utils.mitosis_track import MitosisTrack
-from ..constants.bridges import TIME_RESOLUTION
 from ..utils.bridges_classification.impossible_detection import (
     ImpossibleDetection,
 )
 
-ALPHA = 0.05
-MAX_FRAME = np.inf  # 48*6 <-> 48h * 6 frames/hour
-
 
-def box_plot_cut_differences(
-    cut_differences: list[int], show: bool, save_dir: Optional[str]
-) -> None:
-    """
-    Plot box plot of cut differences
-    """
-    if len(cut_differences) == 0:
-        return
-
-    plt.figure()
-    plt.boxplot(cut_differences)
-    plt.title("Box plot of cut differences")
-    plt.ylabel("Cut difference (min)")
-
-    if show:
-        plt.show()
-
-    if save_dir is not None:
-        plt.savefig(os.path.join(save_dir, "first_mt_cut_differences.png"))
-
-
-def plot_cut_distributions(
-    first_cut_times: list[int],
-    first_cut_times_gt: list[int],
-    p_value: Optional[float],
-    show: bool,
-    save_dir: Optional[str],
-) -> None:
-    """
-    Plot distribution of cut differences
-    """
+class ResultsSavingFactory:
+    """Factory to save results."""
 
-    plt.figure()
-
-    for cut_times, name in zip(
-        [first_cut_times, first_cut_times_gt], ["Predicted", "Ground truth"]
+    def __init__(
+        self,
+        time_resolution: Optional[int] = 10,
+        max_frame: Optional[int] = np.inf,
     ):
-        if len(cut_times) == 0:  # ignore empty gt list
-            continue
-        curve_values = []
-        nb_values = len(cut_times)
-        number_of_cut = 0
-        for i in range(max(cut_times) + 1):
-            count = cut_times.count(i)
-            number_of_cut += count
-            curve_values.append(number_of_cut / nb_values)
-        plt.plot(curve_values, label=name)
-
-    # Quartiles and median
-    predicted_median = np.median(first_cut_times)
-    gt_median = np.median(first_cut_times_gt) if len(first_cut_times_gt) else None
-    predicted_q1 = np.percentile(first_cut_times, 25)
-    predicted_q3 = np.percentile(first_cut_times, 75)
-    plt.axvline(
-        x=predicted_q1,
-        color="r",
-        linestyle="--",
-        linewidth=0.5,
-        label=f"Detected Q1: {predicted_q1}",
-    )
-    plt.axvline(
-        x=predicted_median,
-        color="r",
-        linestyle="-",
-        linewidth=0.5,
-        label=f"Detected median: {predicted_median}"
-        + (f"vs {gt_median} Ground truth median" if gt_median else ""),
-    )
-    plt.axvline(
-        x=predicted_q3,
-        color="r",
-        linestyle="--",
-        linewidth=0.5,
-        label=f"Detected Q3: {predicted_q3}",
-    )
-
-    # add t test result to legend
-    if p_value is not None:
-        plt.legend(loc="lower right", title=f"t test p-value: {p_value:.2f}")
-    else:
-        plt.legend(loc="lower right")
-
-    plt.title(
-        f"Proportion of MT cuts over time - {len(first_cut_times)} predicted mitoses"
-        + (f"- {len(first_cut_times_gt)} ground truth mitoses" if len(first_cut_times_gt) else "")
-    )
-    plt.xlabel("Time (min)")
-    plt.ylabel("Proportion of first cut")
-
-    if show:
-        plt.show()
-
-    if save_dir is not None:
-        plt.savefig(os.path.join(save_dir, "first_mt_cut_distributions.png"))
-
-
-def perform_t_test(cut_differences: list[int]) -> float:
-    """
-    Compute t-test of the differences, which is supposed to be 0.
-    """
-    if len(cut_differences) == 0:
-        return None
-
-    t_result = ttest_1samp(cut_differences, 0)
-    p_value = t_result.pvalue
-
-    # Output the results
-    print(f"P-value: {p_value}")
-
-    # Check if the result is statistically significant (e.g., using a significance level of 0.05)
-    if p_value < ALPHA:
-        print("Reject the null hypothesis: There is a statistically significant difference.")
-    else:
-        print(
-            "Fail to reject the null hypothesis: There is no statistically significant difference."
+        self.time_resolution = time_resolution
+        self.max_frame = max_frame  # for debug, 48*6 <-> 48h * 6 frames/hour
+
+        self.first_cut_times: list[int] = []  # time in absolute time
+        self.first_cut_times_gt: list[int] = []  # time in absolute time
+        self.cut_differences: list[int] = []
+
+        self.mitosis_results_summary: dict[int, int] = {}
+        self.gt_mitosis_results_summary: dict[int, int] = {}
+
+        self.p_value = None
+
+    def _print_weird_mitoses(
+        self, selected_tracks: list[MitosisTrack], min_acceptable_frame: int
+    ) -> None:
+        """
+        Print useful information about weird mitoses.
+        """
+        ordered_tracks = [
+            track
+            for track in selected_tracks
+            if track.key_events_frame["first_mt_cut"]
+            - track.key_events_frame["cytokinesis"]
+            <= min_acceptable_frame
+        ]
+        ordered_tracks.sort(
+            key=lambda x: x.key_events_frame["first_mt_cut"]
+            - x.key_events_frame["cytokinesis"]
         )
 
-    return p_value
+        print("Weird mitoses (early cut):")
+        for mitosis_track in ordered_tracks:
+            print("")
+            print(
+                f"Track: {mitosis_track.id}_{mitosis_track.mother_track_id}_to_{','.join(str(daughter) for daughter in mitosis_track.daughter_track_ids)}"
+            )
+            print(f"Key events frame: {mitosis_track.key_events_frame}")
+            print(
+                "video frame cut",
+                mitosis_track.key_events_frame["first_mt_cut"]
+                - mitosis_track.min_frame
+                + 1,
+            )
+            if mitosis_track.gt_key_events_frame is not None:
+                print(
+                    f"GT key events frame: {mitosis_track.gt_key_events_frame}"
+                )
+                print(
+                    "video frame cut",
+                    mitosis_track.gt_key_events_frame["first_mt_cut"]
+                    - mitosis_track.min_frame
+                    + 1,
+                )
+
+    def update_cut_times(
+        self,
+        mitosis_tracks: list[MitosisTrack],
+        verbose: bool,
+        min_acceptable_frame=13,
+    ) -> None:
+        """Update cut times and summary."""
+
+        selected_tracks: list[MitosisTrack] = []  # kept tracks
+
+        for mitosis_track in mitosis_tracks:
+            # Get first cut frame and start of cytokinesis frame
+            cyto_frame = mitosis_track.key_events_frame["cytokinesis"]
+            cut_frame = mitosis_track.key_events_frame["first_mt_cut"]
+
+            if cut_frame < 0 or cut_frame > self.max_frame:
+                # No cut detected, for some reason
+                cut_time = None
+            else:
+                # At least one cut was actually detected
+                assert cut_frame >= cyto_frame  # should not be possible
+                # Add the difference time to the list
+                cut_time = (cut_frame - cyto_frame) * self.time_resolution
+                self.first_cut_times.append(cut_time)
+                selected_tracks.append(mitosis_track)
+
+            # Update summary
+            cut_id = min(cut_frame, 0)  # 0 if normal, negative otherwise
+
+            if cut_id not in self.mitosis_results_summary:
+                self.mitosis_results_summary[cut_id] = 0
+            self.mitosis_results_summary[cut_id] += 1
+
+            # Ignore if information is not there
+            if (
+                mitosis_track.gt_key_events_frame is None
+                or "first_mt_cut" not in mitosis_track.gt_key_events_frame
+            ):
+                continue
+
+            if (
+                mitosis_track.gt_key_events_frame["first_mt_cut"]
+                > self.max_frame
+            ):
+                # Ignore mitoses that are too late
+                continue
+
+            cut_time_gt = (
+                mitosis_track.gt_key_events_frame["first_mt_cut"]
+                - mitosis_track.gt_key_events_frame["cytokinesis"]
+            ) * self.time_resolution
+            self.first_cut_times_gt.append(cut_time_gt)
+
+            if cut_time is not None:
+                self.cut_differences.append(cut_time - cut_time_gt)
+
+            # Update ground truth summary
+            if cut_id not in self.gt_mitosis_results_summary:
+                self.gt_mitosis_results_summary[cut_id] = 0
+            self.gt_mitosis_results_summary[cut_id] += 1
+
+        # Display few details on mitoses with very early cut
+        if verbose:
+            self._print_weird_mitoses(selected_tracks, min_acceptable_frame)
+
+    def perform_t_test(self, alpha=0.05) -> None:
+        """
+        Compute t-test of the differences, which is supposed to be 0.
+        """
+        if len(self.cut_differences) == 0:
+            return None
+
+        t_result = ttest_1samp(self.cut_differences, 0)
+        self.p_value = t_result.pvalue
 
+        # Output the results
+        print(f"P-value: {self.p_value}")
+
+        # Check if the result is statistically significant (e.g., using a significance level of 0.05)
+        if self.p_value < alpha:
+            print(
+                "Reject the null hypothesis: There is a statistically significant difference."
+            )
+        else:
+            print(
+                "Fail to reject the null hypothesis: There is no statistically significant difference."
+            )
 
-def print_weird_mitoses(selected_tracks: list[MitosisTrack], min_acceptable_frame=13) -> None:
-    """
-    Print useful information about weird mitoses.
-    """
-    ordered_tracks = [
-        track
-        for track in selected_tracks
-        if track.key_events_frame["first_mt_cut"] - track.key_events_frame["cytokinesis"]
-        <= min_acceptable_frame
-    ]
-    ordered_tracks.sort(
-        key=lambda x: x.key_events_frame["first_mt_cut"] - x.key_events_frame["cytokinesis"]
-    )
-
-    print("Weird mitoses (early cut):")
-    for mitosis_track in ordered_tracks:
-        print("")
+    def print_analysis_summary(self, mitosis_tracks) -> None:
+        """Print analysis summary."""
         print(
-            f"Track: {mitosis_track.id}_{mitosis_track.mother_track_id}_to_{','.join(str(daughter) for daughter in mitosis_track.daughter_track_ids)}"
+            f"\n Among the {len(mitosis_tracks)} mitoses detected, there are:"
         )
-        print(f"Key events frame: {mitosis_track.key_events_frame}")
+        for cut_id, count in self.mitosis_results_summary.items():
+            print(
+                f"    - {count} mitoses in category {ImpossibleDetection(cut_id).name}"
+            )
+
+        if len(self.first_cut_times_gt) == 0:
+            return
         print(
-            "video frame cut",
-            mitosis_track.key_events_frame["first_mt_cut"] - mitosis_track.min_frame + 1,
+            f"\n Among the {len(self.first_cut_times_gt)} mitoses annotated, there are:"
         )
-        if mitosis_track.gt_key_events_frame is not None:
-            print(f"GT key events frame: {mitosis_track.gt_key_events_frame}")
+        for cut_id, count in self.gt_mitosis_results_summary.items():
             print(
-                "video frame cut",
-                mitosis_track.gt_key_events_frame["first_mt_cut"] - mitosis_track.min_frame + 1,
+                f"    - {count} mitoses in category {ImpossibleDetection(cut_id).name}"
             )
 
+    def box_plot_cut_differences(
+        self, show: bool, save_dir: Optional[str]
+    ) -> None:
+        """
+        Plot box plot of cut differences
+        """
+        if len(self.cut_differences) == 0:
+            return
+
+        plt.figure()
+        plt.boxplot(self.cut_differences)
+        plt.title("Box plot of cut differences")
+        plt.ylabel("Cut difference (min)")
+
+        if show:
+            plt.show()
+
+        if save_dir is not None:
+            plt.savefig(os.path.join(save_dir, "first_mt_cut_differences.png"))
+
+    def plot_cut_distributions(
+        self,
+        show: bool,
+        save_dir: Optional[str],
+    ) -> None:
+        """
+        Plot distribution of cut differences
+        """
+
+        plt.figure()
+
+        for cut_times, name in zip(
+            [self.first_cut_times, self.first_cut_times_gt],
+            ["Predicted", "Ground truth"],
+        ):
+            if len(cut_times) == 0:  # ignore empty gt list
+                continue
+            curve_values = []
+            nb_values = len(cut_times)
+            number_of_cut = 0
+            for i in range(max(cut_times) + 1):
+                count = cut_times.count(i)
+                number_of_cut += count
+                curve_values.append(number_of_cut / nb_values)
+            plt.plot(curve_values, label=name)
+
+        # Quartiles and median
+        predicted_median = np.median(self.first_cut_times)
+        gt_median = (
+            np.median(self.first_cut_times_gt)
+            if len(self.first_cut_times_gt)
+            else None
+        )
+        predicted_q1 = np.percentile(self.first_cut_times, 25)
+        predicted_q3 = np.percentile(self.first_cut_times, 75)
+        plt.axvline(
+            x=predicted_q1,
+            color="r",
+            linestyle="--",
+            linewidth=0.5,
+            label=f"Detected Q1: {predicted_q1}",
+        )
+        plt.axvline(
+            x=predicted_median,
+            color="r",
+            linestyle="-",
+            linewidth=0.5,
+            label=f"Detected median: {predicted_median}"
+            + (f"vs {gt_median} Ground truth median" if gt_median else ""),
+        )
+        plt.axvline(
+            x=predicted_q3,
+            color="r",
+            linestyle="--",
+            linewidth=0.5,
+            label=f"Detected Q3: {predicted_q3}",
+        )
 
-def print_analysis_summary(
-    mitosis_tracks: list[MitosisTrack],
-    mitosis_results_summary: dict[int, int],
-    first_cut_times_gt: list[int],
-    gt_mitosis_results_summary: dict[int, int],
-) -> None:
-    print(f"\n Among the {len(mitosis_tracks)} mitoses detected, there are:")
-    for cut_id, count in mitosis_results_summary.items():
-        print(f"    - {count} mitoses in category {ImpossibleDetection(cut_id).name}")
-
-    if len(first_cut_times_gt) == 0:
-        return
-    print(f"\n Among the {len(first_cut_times_gt)} mitoses annotated, there are:")
-    for cut_id, count in gt_mitosis_results_summary.items():
-        print(f"    - {count} mitoses in category {ImpossibleDetection(cut_id).name}")
-
-
-def save_csv_results(mitosis_tracks: list[MitosisTrack], save_dir: Optional[str] = None) -> None:
-    if save_dir is None:
-        return
-
-    csv_path = os.path.join(save_dir, "results.csv")
-    # Create CSV results file if it does not exist
-    if not os.path.exists(csv_path):
-        with open(csv_path, "w") as f:
-            f.write(
-                "id;mother track;daughter track(s);metaphase frame;cytokinesis frame;first MT cut frame;second MT cut frame;first MT cut time;second MT cut time\n"
+        # add t test result to legend
+        if self.p_value is not None:
+            plt.legend(
+                loc="lower right", title=f"t test p-value: {self.p_value:.2f}"
             )
-        f.close()
+        else:
+            plt.legend(loc="lower right")
 
-    # Store useful results in global results file
-    with open(csv_path, "a") as f:
-        for mitosis_track in mitosis_tracks:
-            f.write(f"{mitosis_track.id};")
-            f.write(f"{mitosis_track.mother_track_id};")
-            daughter_ids = ",".join([str(d) for d in mitosis_track.daughter_track_ids])
-            f.write(f"{daughter_ids};")
-            f.write(f"{mitosis_track.key_events_frame['metaphase']};")
-            cytokinesis_frame = mitosis_track.key_events_frame["cytokinesis"]
-            f.write(f"{cytokinesis_frame};")
-            first_cut_frame = mitosis_track.key_events_frame["first_mt_cut"]
-            f.write(f"{first_cut_frame};")
-            second_cut_frame = mitosis_track.key_events_frame["second_mt_cut"]
-            f.write(f"{second_cut_frame};")
-            first_cut_time = (
-                (first_cut_frame - cytokinesis_frame) * TIME_RESOLUTION
-                if first_cut_frame >= 0
-                else ""
-            )
-            f.write(f"{first_cut_time};")
-            second_cut_time = (
-                (second_cut_frame - cytokinesis_frame) * TIME_RESOLUTION
-                if second_cut_frame >= 0
+        plt.title(
+            f"Proportion of MT cuts over time - {len(self.first_cut_times)} predicted mitoses"
+            + (
+                f"- {len(self.first_cut_times_gt)} ground truth mitoses"
+                if len(self.first_cut_times_gt)
                 else ""
             )
-            f.write(f"{second_cut_time};\n")
-    f.close()
+        )
+        plt.xlabel("Time (min)")
+        plt.ylabel("Proportion of first cut")
 
+        if show:
+            plt.show()
 
-def perform_results_saving(
-    exported_mitoses_dir: str,
-    show: bool = False,
-    save_dir: Optional[str] = None,
-    verbose: bool = False,
-) -> None:
-    # Create save_dir if specified and it does not exist
-    if save_dir is not None and not os.path.exists(save_dir):
-        os.makedirs(save_dir)
-
-    mitosis_tracks: list[MitosisTrack] = []
-    # Iterate over "bin" files in exported_mitoses_dir
-    for state_path in os.listdir(exported_mitoses_dir):
-        # Load mitosis track
-        with open(os.path.join(exported_mitoses_dir, state_path), "rb") as f:
-            mitosis_track = pickle.load(f)
-
-        # Add mitosis track to list
-        mitosis_tracks.append(mitosis_track)
-
-    # Define lists and dictionaries to store results
-    first_cut_times: list[int] = []  # time in absolute time
-    first_cut_times_gt: list[int] = []  # time in absolute time
-    selected_tracks: list[MitosisTrack] = []  # kept tracks
-    cut_differences: list[int] = []
-    mitosis_results_summary: dict[int, int] = {}
-    gt_mitosis_results_summary: dict[int, int] = {}
-    # Get first MT cut time
-    for mitosis_track in mitosis_tracks:
-        # Get first cut frame and start of cytokinesis frame
-        cyto_frame = mitosis_track.key_events_frame["cytokinesis"]
-        cut_frame = mitosis_track.key_events_frame["first_mt_cut"]
-
-        if cut_frame < 0 or cut_frame > MAX_FRAME:
-            # No cut detected, for some reason
-            cut_time = None
-        else:
-            # At least one cut was actually detected
-            assert cut_frame >= cyto_frame  # should not be possible
-            # Add the difference time to the list
-            cut_time = (cut_frame - cyto_frame) * TIME_RESOLUTION
-            first_cut_times.append(cut_time)
-            selected_tracks.append(mitosis_track)
-
-        # Update summary
-        cut_id = min(cut_frame, 0)  # 0 if normal, negative otherwise
-
-        if cut_id not in mitosis_results_summary:
-            mitosis_results_summary[cut_id] = 0
-        mitosis_results_summary[cut_id] += 1
-
-        # Ignore if information is not there
-        if (
-            mitosis_track.gt_key_events_frame is None
-            or "first_mt_cut" not in mitosis_track.gt_key_events_frame
-        ):
-            continue
+        if save_dir is not None:
+            plt.savefig(
+                os.path.join(save_dir, "first_mt_cut_distributions.png")
+            )
 
-        if mitosis_track.gt_key_events_frame["first_mt_cut"] > MAX_FRAME:
-            # Ignore mitoses that are too late
-            continue
-
-        cut_time_gt = (
-            mitosis_track.gt_key_events_frame["first_mt_cut"]
-            - mitosis_track.gt_key_events_frame["cytokinesis"]
-        ) * TIME_RESOLUTION
-        first_cut_times_gt.append(cut_time_gt)
-
-        if cut_time is not None:
-            cut_differences.append(cut_time - cut_time_gt)
-
-        # Update ground truth summary
-        if cut_id not in gt_mitosis_results_summary:
-            gt_mitosis_results_summary[cut_id] = 0
-        gt_mitosis_results_summary[cut_id] += 1
-
-    # Display few details on mitoses with very early cut
-    if verbose:
-        print_weird_mitoses(selected_tracks)
-
-    # Statistical test
-    p_value = perform_t_test(cut_differences)
-
-    # Print summaries
-    print_analysis_summary(
-        mitosis_tracks,
-        mitosis_results_summary,
-        first_cut_times_gt,
-        gt_mitosis_results_summary,
-    )
-
-    # Save results in as csv file
-    save_csv_results(mitosis_tracks, save_dir)
-
-    # Plot results
-    box_plot_cut_differences(cut_differences, show, save_dir)
-    plot_cut_distributions(first_cut_times, first_cut_times_gt, p_value, show, save_dir)
+    def save_csv_results(
+        self,
+        mitosis_tracks: list[MitosisTrack],
+        save_dir: Optional[str] = None,
+    ) -> None:
+        """Save results in CSV file."""
+        if save_dir is None:
+            return
+
+        csv_path = os.path.join(save_dir, "results.csv")
+        # Create CSV results file if it does not exist
+        if not os.path.exists(csv_path):
+            with open(csv_path, "w") as f:
+                f.write(
+                    "id;mother track;daughter track(s);metaphase frame;cytokinesis frame;first MT cut frame;second MT cut frame;first MT cut time;second MT cut time\n"
+                )
+            f.close()
+
+        # Store useful results in global results file
+        with open(csv_path, "a") as f:
+            for mitosis_track in mitosis_tracks:
+                f.write(f"{mitosis_track.id};")
+                f.write(f"{mitosis_track.mother_track_id};")
+                daughter_ids = ",".join(
+                    [str(d) for d in mitosis_track.daughter_track_ids]
+                )
+                f.write(f"{daughter_ids};")
+                f.write(f"{mitosis_track.key_events_frame['metaphase']};")
+                cytokinesis_frame = mitosis_track.key_events_frame[
+                    "cytokinesis"
+                ]
+                f.write(f"{cytokinesis_frame};")
+                first_cut_frame = mitosis_track.key_events_frame[
+                    "first_mt_cut"
+                ]
+                f.write(f"{first_cut_frame};")
+                second_cut_frame = mitosis_track.key_events_frame[
+                    "second_mt_cut"
+                ]
+                f.write(f"{second_cut_frame};")
+                first_cut_time = (
+                    (first_cut_frame - cytokinesis_frame)
+                    * self.time_resolution
+                    if first_cut_frame >= 0
+                    else ""
+                )
+                f.write(f"{first_cut_time};")
+                second_cut_time = (
+                    (second_cut_frame - cytokinesis_frame)
+                    * self.time_resolution
+                    if second_cut_frame >= 0
+                    else ""
+                )
+                f.write(f"{second_cut_time};\n")
+        f.close()
```

### Comparing `cut-detector-0.0.8/src/cut_detector/widget_functions/tracking.py` & `cut-detector-0.0.9/src/cut_detector/factories/segmentation_tracking_factory.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,180 +1,222 @@
 import os
 import sys
-from typing import Optional
 import torch
 import imagej
 import scyjava as sj
 from cellpose import models
 
-from ..models.tools import get_model_path
-from ..constants.tracking import (
-    AUGMENT,
-    CELLPROB_THRESHOLD,
-    FLOW_THRESHOLD,
-    GAP_CLOSING_MAX_DISTANCE_RATIO,
-    LINKING_MAX_DISTANCE_RATIO,
-    MAX_FRAME_GAP,
-)
-
-
-def perform_tracking(
-    video_path: str,
-    fiji_path: str,
-    save_folder: str,
-    model_path: Optional[str],
-    fast_mode: bool,
-) -> None:
-    # Load default model if necessary
-    if model_path is None:
-        model_path = get_model_path("segmentation_model")
-
-    # Create save directory if it doesn't exist
-    if not os.path.exists(save_folder):
-        os.makedirs(save_folder)
-
-    ij_instance = imagej.init(fiji_path, mode="interactive")
-
-    bf_plugin = sj.jimport("loci.plugins.BF")
-    importer_options = sj.jimport("loci.plugins.in.ImporterOptions")
-
-    # Import TrackMate via scyjava
-    track_mate_model = sj.jimport(
-        "fiji.plugin.trackmate.Model"
-    )  # class in charge of storing the data
-    track_mate_settings = sj.jimport(
-        "fiji.plugin.trackmate.Settings"
-    )  # class storing the fields that will configure TrackMate and pilot how the data is created
-    track_mate = sj.jimport("fiji.plugin.trackmate.TrackMate")
-    logger = sj.jimport("fiji.plugin.trackmate.Logger")
-    lap_utils = sj.jimport("fiji.plugin.trackmate.tracking.jaqaman.LAPUtils")
-    sparse_lap_tracker_factory = sj.jimport(
-        "fiji.plugin.trackmate.tracking.jaqaman.SparseLAPTrackerFactory"
-    )
-    file = sj.jimport("java.io.File")
-    tm_xml_writer = sj.jimport("fiji.plugin.trackmate.io.TmXmlWriter")
-    tracker_keys = sj.jimport("fiji.plugin.trackmate.tracking.TrackerKeys")
-    track_mate_track_analyzer_provider = sj.jimport(
-        "fiji.plugin.trackmate.providers.TrackAnalyzerProvider"
-    )
-    track_mate_edge_analyzer_provider = sj.jimport(
-        "fiji.plugin.trackmate.providers.EdgeAnalyzerProvider"
-    )
+from ..utils.cell_track import CellTrack
 
-    if fast_mode:
-        try:
+
+class SegmentationTrackingFactory:
+    """
+    Class to perform cell segmentation and tracking.
+
+    Args:
+        model_path (str): path to the cellpose model
+        augment (bool)
+        cellprob_threshold (float)
+        flow_threshold (float)
+        gap_closing_max_distance_ratio (float): ratio of average spot size
+        linking_max_distance_ratio  (float): ratio of average spot size
+        max_frame_gap (int)
+    """
+
+    def __init__(
+        self,
+        model_path: str,
+        augment=True,
+        cellprob_threshold=0.0,
+        flow_threshold=0.0,
+        gap_closing_max_distance_ratio=0.5,
+        linking_max_distance_ratio=1,
+        max_frame_gap=CellTrack.max_frame_gap,
+    ) -> None:
+        self.model_path = model_path
+        self.augment = augment
+        self.cellprob_threshold = cellprob_threshold
+        self.flow_threshold = flow_threshold
+        self.gap_closing_max_distance_ratio = gap_closing_max_distance_ratio
+        self.linking_max_distance_ratio = linking_max_distance_ratio
+        self.max_frame_gap = max_frame_gap
+
+    def perform_trackmate_tracking(
+        self,
+        video_path: str,
+        fiji_path: str,
+        save_folder: str,
+        fast_mode: bool,
+    ):
+        """
+        Use Trackmate to run both segmentation and tracking.
+        """
+        ij_instance = imagej.init(fiji_path, mode="interactive")
+
+        bf_plugin = sj.jimport("loci.plugins.BF")
+        importer_options = sj.jimport("loci.plugins.in.ImporterOptions")
+
+        # Import TrackMate via scyjava
+        track_mate_model = sj.jimport(
+            "fiji.plugin.trackmate.Model"
+        )  # class in charge of storing the data
+        track_mate_settings = sj.jimport(
+            "fiji.plugin.trackmate.Settings"
+        )  # class storing the fields that will configure TrackMate and pilot how the data is created
+        track_mate = sj.jimport("fiji.plugin.trackmate.TrackMate")
+        logger = sj.jimport("fiji.plugin.trackmate.Logger")
+        lap_utils = sj.jimport(
+            "fiji.plugin.trackmate.tracking.jaqaman.LAPUtils"
+        )
+        sparse_lap_tracker_factory = sj.jimport(
+            "fiji.plugin.trackmate.tracking.jaqaman.SparseLAPTrackerFactory"
+        )
+        file = sj.jimport("java.io.File")
+        tm_xml_writer = sj.jimport("fiji.plugin.trackmate.io.TmXmlWriter")
+        tracker_keys = sj.jimport("fiji.plugin.trackmate.tracking.TrackerKeys")
+        track_mate_track_analyzer_provider = sj.jimport(
+            "fiji.plugin.trackmate.providers.TrackAnalyzerProvider"
+        )
+        track_mate_edge_analyzer_provider = sj.jimport(
+            "fiji.plugin.trackmate.providers.EdgeAnalyzerProvider"
+        )
+
+        if fast_mode:
+            try:
+                cellpose_detector_factory = sj.jimport(
+                    "fiji.plugin.trackmate.cellpose.tbonte.CellposeDetectorFactory"
+                )
+                pretrained_model = sj.jimport(
+                    "fiji.plugin.trackmate.cellpose.tbonte.CellposeSettings.PretrainedModel"
+                )
+            except TypeError:
+                print(
+                    "No Trackmate plugin found for fast mode. Using usual segmentation instead."
+                )
+                fast_mode = False
+
+        if not fast_mode:
             cellpose_detector_factory = sj.jimport(
-                "fiji.plugin.trackmate.cellpose.tbonte.CellposeDetectorFactory"
+                "fiji.plugin.trackmate.cellpose.CellposeDetectorFactory"
             )
             pretrained_model = sj.jimport(
-                "fiji.plugin.trackmate.cellpose.tbonte.CellposeSettings.PretrainedModel"
+                "fiji.plugin.trackmate.cellpose.CellposeSettings.PretrainedModel"
+            )
+
+        # Skip if file already exists
+        video_file_name = os.path.basename(video_path).split(".")[0]
+        out_file = os.path.join(save_folder, f"{video_file_name}_model.xml")
+        if os.path.exists(out_file):
+            print(f"File {out_file} already exists. Skipping.")
+            return
+
+        # Get currently selected image
+        options = importer_options()
+        options.setColorMode(importer_options.COLOR_MODE_GRAYSCALE)
+        options.setId(video_path)
+        imps = bf_plugin.openImagePlus(options)
+        imp = imps[0]
+
+        # Swap Z and T dimensions if necessary
+        dims = imp.getDimensions()
+        if imp.dims[-1] == "Z":
+            imp.setDimensions(
+                sj.to_java(dims[2]), sj.to_java(dims[4]), sj.to_java(dims[3])
+            )
+            print("Swapping Z and T dimensions")
+
+        # Get the average spot size to define max linking distances
+        average_spot_size = models.CellposeModel(
+            pretrained_model=[self.model_path]
+        ).diam_labels
+
+        # Create model object
+        model = track_mate_model()
+
+        # Send all messages to ImageJ log window.
+        model.setLogger(logger.IJ_LOGGER)
+
+        # Prepare settings object
+        settings = track_mate_settings(imp)
+
+        # Configure detector - We use the Strings for the keys
+        settings.detectorFactory = cellpose_detector_factory()
+        settings.detectorSettings["TARGET_CHANNEL"] = sj.to_java(3)
+        settings.detectorSettings["OPTIONAL_CHANNEL_2"] = sj.to_java(0)
+        settings.detectorSettings["CELLPOSE_PYTHON_FILEPATH"] = sys.executable
+        settings.detectorSettings["CELLPOSE_MODEL_FILEPATH"] = self.model_path
+        settings.detectorSettings["CELLPOSE_MODEL"] = pretrained_model.CUSTOM
+        settings.detectorSettings["CELL_DIAMETER"] = sj.to_java(
+            0.0, type="double"
+        )
+        settings.detectorSettings["USE_GPU"] = (
+            True if torch.cuda.is_available() else False
+        )
+        settings.detectorSettings["SIMPLIFY_CONTOURS"] = True
+
+        if fast_mode:
+            settings.detectorSettings["FLOW_THRESHOLD"] = self.flow_threshold
+            settings.detectorSettings["CELLPROB_THRESHOLD"] = (
+                self.cellprob_threshold
             )
-        except TypeError:
-            print("No Trackmate plugin found for fast mode. Using usual segmentation instead.")
-            fast_mode = False
-
-    if not fast_mode:
-        cellpose_detector_factory = sj.jimport(
-            "fiji.plugin.trackmate.cellpose.CellposeDetectorFactory"
-        )
-        pretrained_model = sj.jimport(
-            "fiji.plugin.trackmate.cellpose.CellposeSettings.PretrainedModel"
-        )
-
-    # Skip if file already exists
-    video_file_name = os.path.basename(video_path).split(".")[0]
-    out_file = os.path.join(save_folder, f"{video_file_name}_model.xml")
-    if os.path.exists(out_file):
-        print(f"File {out_file} already exists. Skipping.")
-        return
-
-    # Get currently selected image
-    options = importer_options()
-    options.setColorMode(importer_options.COLOR_MODE_GRAYSCALE)
-    options.setId(video_path)
-    imps = bf_plugin.openImagePlus(options)
-    imp = imps[0]
-
-    # Swap Z and T dimensions if necessary
-    dims = imp.getDimensions()
-    if imp.dims[-1] == "Z":
-        imp.setDimensions(sj.to_java(dims[2]), sj.to_java(dims[4]), sj.to_java(dims[3]))
-        print("Swapping Z and T dimensions")
-
-    # Get the average spot size to define max linking distances
-    average_spot_size = models.CellposeModel(pretrained_model=[model_path]).diam_labels
-
-    # Create model object
-    model = track_mate_model()
-
-    # Send all messages to ImageJ log window.
-    model.setLogger(logger.IJ_LOGGER)
-
-    # Prepare settings object
-    settings = track_mate_settings(imp)
-
-    # Configure detector - We use the Strings for the keys
-    settings.detectorFactory = cellpose_detector_factory()
-    settings.detectorSettings["TARGET_CHANNEL"] = sj.to_java(3)
-    settings.detectorSettings["OPTIONAL_CHANNEL_2"] = sj.to_java(0)
-    settings.detectorSettings["CELLPOSE_PYTHON_FILEPATH"] = sys.executable
-    settings.detectorSettings["CELLPOSE_MODEL_FILEPATH"] = model_path
-    settings.detectorSettings["CELLPOSE_MODEL"] = pretrained_model.CUSTOM
-    settings.detectorSettings["CELL_DIAMETER"] = sj.to_java(0.0, type="double")
-    settings.detectorSettings["USE_GPU"] = True if torch.cuda.is_available() else False
-    settings.detectorSettings["SIMPLIFY_CONTOURS"] = True
-
-    if fast_mode:
-        settings.detectorSettings["FLOW_THRESHOLD"] = FLOW_THRESHOLD
-        settings.detectorSettings["CELLPROB_THRESHOLD"] = CELLPROB_THRESHOLD
-        settings.detectorSettings["AUGMENT"] = AUGMENT
-
-    # Configure tracker
-    settings.trackerFactory = sparse_lap_tracker_factory()
-    settings.trackerSettings = lap_utils.getDefaultSegmentSettingsMap()  # almost good enough
-    settings.trackerSettings["LINKING_MAX_DISTANCE"] = (
-        LINKING_MAX_DISTANCE_RATIO * average_spot_size
-    )
-    settings.trackerSettings["ALLOW_GAP_CLOSING"] = True
-    settings.trackerSettings["GAP_CLOSING_MAX_DISTANCE"] = (
-        GAP_CLOSING_MAX_DISTANCE_RATIO * average_spot_size
-    )
-    settings.trackerSettings["MAX_FRAME_GAP"] = sj.to_java(MAX_FRAME_GAP)
-    settings.trackerSettings["ALLOW_TRACK_MERGING"] = False
-    settings.trackerSettings["ALLOW_TRACK_SPLITTING"] = False
-    settings.trackerSettings[
-        "LINKING_FEATURE_PENALTIES"
-    ] = tracker_keys.DEFAULT_LINKING_FEATURE_PENALTIES
-
-    settings.initialSpotFilterValue = -1.0
-
-    # Add useful track analyzers
-    track_analyzer_provider = track_mate_track_analyzer_provider()
-    settings.addTrackAnalyzer(track_analyzer_provider.getFactory("Track duration"))
-    settings.addTrackAnalyzer(track_analyzer_provider.getFactory("Track index"))
-
-    edge_analyzer_provider = track_mate_edge_analyzer_provider()
-    settings.addEdgeAnalyzer(edge_analyzer_provider.getFactory("Edge target"))
-
-    # Instantiate plugin
-    trackmate = track_mate(model, settings)
-
-    # Process
-    process_ok = trackmate.checkInput()
-    if not process_ok:
-        sys.exit(str(trackmate.getErrorMessage()))
-
-    process_ok = trackmate.process()
-    if not process_ok:
-        sys.exit(str(trackmate.getErrorMessage()))
-
-    # Echo results with the logger we set at start:
-    model.getLogger().log(str(model))
-
-    out_file_model = file(save_folder, f"{video_file_name}_model.xml")
-    writer = tm_xml_writer(out_file_model)
-    writer.appendModel(model)
-    writer.appendSettings(settings)
-    writer.writeToFile()
+            settings.detectorSettings["AUGMENT"] = self.augment
+
+        # Configure tracker
+        settings.trackerFactory = sparse_lap_tracker_factory()
+        settings.trackerSettings = (
+            lap_utils.getDefaultSegmentSettingsMap()
+        )  # almost good enough
+        settings.trackerSettings["LINKING_MAX_DISTANCE"] = (
+            self.linking_max_distance_ratio * average_spot_size
+        )
+        settings.trackerSettings["ALLOW_GAP_CLOSING"] = True
+        settings.trackerSettings["GAP_CLOSING_MAX_DISTANCE"] = (
+            self.gap_closing_max_distance_ratio * average_spot_size
+        )
+        settings.trackerSettings["MAX_FRAME_GAP"] = sj.to_java(
+            self.max_frame_gap
+        )
+        settings.trackerSettings["ALLOW_TRACK_MERGING"] = False
+        settings.trackerSettings["ALLOW_TRACK_SPLITTING"] = False
+        settings.trackerSettings["LINKING_FEATURE_PENALTIES"] = (
+            tracker_keys.DEFAULT_LINKING_FEATURE_PENALTIES
+        )
+
+        settings.initialSpotFilterValue = -1.0
+
+        # Add useful track analyzers
+        track_analyzer_provider = track_mate_track_analyzer_provider()
+        settings.addTrackAnalyzer(
+            track_analyzer_provider.getFactory("Track duration")
+        )
+        settings.addTrackAnalyzer(
+            track_analyzer_provider.getFactory("Track index")
+        )
+
+        edge_analyzer_provider = track_mate_edge_analyzer_provider()
+        settings.addEdgeAnalyzer(
+            edge_analyzer_provider.getFactory("Edge target")
+        )
+
+        # Instantiate plugin
+        trackmate = track_mate(model, settings)
+
+        # Process
+        process_ok = trackmate.checkInput()
+        if not process_ok:
+            sys.exit(str(trackmate.getErrorMessage()))
+
+        process_ok = trackmate.process()
+        if not process_ok:
+            sys.exit(str(trackmate.getErrorMessage()))
+
+        # Echo results with the logger we set at start:
+        model.getLogger().log(str(model))
+
+        out_file_model = file(save_folder, f"{video_file_name}_model.xml")
+        writer = tm_xml_writer(out_file_model)
+        writer.appendModel(model)
+        writer.appendSettings(settings)
+        writer.writeToFile()
 
-    # Force exit
-    ij_instance.dispose()
+        # Force exit
+        ij_instance.dispose()
```

### Comparing `cut-detector-0.0.8/src/cut_detector.egg-info/PKG-INFO` & `cut-detector-0.0.9/src/cut_detector.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cut-detector
-Version: 0.0.8
+Version: 0.0.9
 Summary: Automatic Cut Detector
 Home-page: https://github.com/15bonte/cut-detector
 Author: Thomas Bonte
 Author-email: thomas.bonte@mines-paristech.fr
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/15bonte/cut-detector/issues
 Project-URL: Documentation, https://github.com/15bonte/cut-detector#README.md
@@ -24,15 +24,15 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cellpose>=2.2.3
 Requires-Dist: pyimagej
 Requires-Dist: scyjava
 Requires-Dist: numpy<=1.24
-Requires-Dist: cnn_framework==0.0.11
+Requires-Dist: cnn_framework==0.0.15
 Requires-Dist: magicgui
 Requires-Dist: pydantic==1.10.12
 Requires-Dist: xmltodict
 Requires-Dist: shapely
 Requires-Dist: aicsimageio
 Requires-Dist: scikit-learn==1.2.2
 Requires-Dist: charset-normalizer==3.3.0
@@ -72,34 +72,47 @@
 
 ### Conda environment
 
 It is highly recommended to create a dedicated conda environment, by following these few steps:
 
 1. Install an [Anaconda] distribution of Python. Note you might need to use an anaconda prompt if you did not add anaconda to the path.
 
-2. Open an Anaconda prompt as admin to create a new environment using [conda]. We advice to use python 3.10 and conda 23.10.0, to get conda-libmamba-solver as default solver. Note than openjdk is necessary to call Fiji from python, which is needed as you will see below.
+2. Open an Anaconda prompt as admin to create a new environment using [conda]. We advice to use python 3.10 and conda 23.10.0, to get conda-libmamba-solver as default solver.
 
 ```
 conda create --name cut_detector python=3.10 conda=23.10.0
 conda activate cut_detector
-conda install -c conda-forge openjdk=8
 ```
 
 ### Package installation
 
 Once in a dedicated environment, our package can be installed via [pip]:
 
 ```
 pip install cut_detector
 ```
 
+Alternatively, you can clone the github repo to access to playground scripts.
+
+```
+git clone https://github.com/15bonte/cut-detector.git
+cd cut-detector
+pip install -e .
+```
+
 ### Fiji
 
 This package relies on [Trackmate] to perform cell tracking. Trackmate is called through [Fiji], which has to be installed independently. Please follow the steps [here](https://imagej.net/software/fiji/downloads) to install it.
 
+Next, install openjdk which is necessary to call Fiji from python.
+
+```
+conda install -c conda-forge openjdk=8
+```
+
 ### GPU
 
 We highly recommend to use GPU to speed up segmentation. To use your NVIDIA GPU, the first step is to download the dedicated driver from [NVIDIA].
 
 Next we need to remove the CPU version of torch:
 
 ```
```

### Comparing `cut-detector-0.0.8/src/cut_detector.egg-info/SOURCES.txt` & `cut-detector-0.0.9/src/cut_detector.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -5,63 +5,76 @@
 README.md
 pyproject.toml
 setup.cfg
 tox.ini
 .github/workflows/test_and_deploy.yml
 .napari-hub/DESCRIPTION.md
 .napari-hub/config.yml
+playground/mid_body_detection.py
+playground/mid_body_evaluation.py
+playground/mid_body_execution.py
+playground/mt_cut_detection.py
 playground/napari_layer.py
 playground/segmentation.py
+playground/tracking.py
 src/cut_detector/__init__.py
 src/cut_detector/_version.py
 src/cut_detector/_widget.py
 src/cut_detector/napari.yaml
 src/cut_detector.egg-info/PKG-INFO
 src/cut_detector.egg-info/SOURCES.txt
 src/cut_detector.egg-info/dependency_links.txt
 src/cut_detector.egg-info/entry_points.txt
 src/cut_detector.egg-info/requires.txt
 src/cut_detector.egg-info/top_level.txt
 src/cut_detector/_tests/__init__.py
+src/cut_detector/_tests/test_annotations_upload.py
 src/cut_detector/_tests/test_micro_tubules_cut_detection.py
 src/cut_detector/_tests/test_mid_body_detection.py
 src/cut_detector/_tests/test_results_saving.py
 src/cut_detector/_tests/test_segmentation_tracking.py
 src/cut_detector/_tests/test_track_generation.py
 src/cut_detector/_tests/test_whole_process.py
 src/cut_detector/constants/__init__.py
 src/cut_detector/constants/annotations.py
-src/cut_detector/constants/bridges.py
 src/cut_detector/constants/tracking.py
 src/cut_detector/data/__init__.py
 src/cut_detector/data/tools.py
 src/cut_detector/factories/__init__.py
 src/cut_detector/factories/mid_body_detection_factory.py
 src/cut_detector/factories/mt_cut_detection_factory.py
+src/cut_detector/factories/results_saving_factory.py
+src/cut_detector/factories/segmentation_tracking_factory.py
 src/cut_detector/factories/tracks_merging_factory.py
 src/cut_detector/models/__init__.py
 src/cut_detector/models/tools.py
 src/cut_detector/utils/__init__.py
 src/cut_detector/utils/box_dimensions.py
 src/cut_detector/utils/box_dimensions_dln.py
+src/cut_detector/utils/cell_spot.py
+src/cut_detector/utils/cell_track.py
+src/cut_detector/utils/cnn_data_set.py
 src/cut_detector/utils/hidden_markov_models.py
 src/cut_detector/utils/image_tools.py
 src/cut_detector/utils/mid_body_spot.py
 src/cut_detector/utils/mid_body_track.py
 src/cut_detector/utils/mitosis_track.py
+src/cut_detector/utils/spot.py
 src/cut_detector/utils/tools.py
+src/cut_detector/utils/track.py
 src/cut_detector/utils/trackmate_frame_spots.py
 src/cut_detector/utils/trackmate_spot.py
 src/cut_detector/utils/trackmate_track.py
 src/cut_detector/utils/bridges_classification/__init__.py
+src/cut_detector/utils/bridges_classification/bridges_mt_cnn_model_params.py
+src/cut_detector/utils/bridges_classification/bridges_mt_model_manager.py
 src/cut_detector/utils/bridges_classification/impossible_detection.py
+src/cut_detector/utils/bridges_classification/micro_tubules_augmentation.py
 src/cut_detector/utils/bridges_classification/template_type.py
 src/cut_detector/utils/cell_division_detection/__init__.py
-src/cut_detector/utils/cell_division_detection/metaphase_cnn.py
-src/cut_detector/utils/cell_division_detection/metaphase_cnn_data_set.py
 src/cut_detector/utils/cell_division_detection/metaphase_cnn_model_params.py
 src/cut_detector/widget_functions/__init__.py
 src/cut_detector/widget_functions/mid_body_detection.py
 src/cut_detector/widget_functions/mitosis_track_generation.py
 src/cut_detector/widget_functions/mt_cut_detection.py
 src/cut_detector/widget_functions/save_results.py
 src/cut_detector/widget_functions/tracking.py
```

### Comparing `cut-detector-0.0.8/tox.ini` & `cut-detector-0.0.9/tox.ini`

 * *Files identical despite different names*

