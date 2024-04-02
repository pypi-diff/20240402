# Comparing `tmp/napari_cellseg3d-0.1.1rc1.tar.gz` & `tmp/napari_cellseg3d-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari_cellseg3d-0.1.1rc1.tar", last modified: Thu Dec 14 17:37:16 2023, max compression
+gzip compressed data, was "napari_cellseg3d-0.1.2.tar", last modified: Tue Apr  2 08:55:46 2024, max compression
```

## Comparing `napari_cellseg3d-0.1.1rc1.tar` & `napari_cellseg3d-0.1.2.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 17:37:16.429882 napari_cellseg3d-0.1.1rc1/
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      206 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9748 2023-12-14 17:37:16.429882 napari_cellseg3d-0.1.1rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7078 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 17:37:16.413882 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 17:37:16.417882 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/_tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/_tests/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 17:37:16.417882 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/_tests/res/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/_tests/res/test.png
--rw-r--r--   0 runner    (1001) docker     (127)      577 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/_tests/test_base_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/_tests/test_dock_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/_tests/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3426 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/_tests/test_inference.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/_tests/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/_tests/test_labels_correction.py
--rw-r--r--   0 runner    (1001) docker     (127)     3630 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/_tests/test_model_framework.py
--rw-r--r--   0 runner    (1001) docker     (127)     3953 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/_tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3276 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/_tests/test_plugin_inference.py
--rw-r--r--   0 runner    (1001) docker     (127)     4125 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/_tests/test_plugin_training.py
--rw-r--r--   0 runner    (1001) docker     (127)     2362 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/_tests/test_plugin_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      627 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/_tests/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/_tests/test_review.py
--rw-r--r--   0 runner    (1001) docker     (127)     4291 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/_tests/test_training.py
--rw-r--r--   0 runner    (1001) docker     (127)     7335 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/_tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/_tests/test_weight_download.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/_tests/test_wnet_training.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 17:37:16.417882 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_models/
--rw-r--r--   0 runner    (1001) docker     (127)      659 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9598 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_models/crf.py
--rw-r--r--   0 runner    (1001) docker     (127)    30959 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_models/instance_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)    13712 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_models/model_framework.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 17:37:16.421882 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_models/models/
--rw-r--r--   0 runner    (1001) docker     (127)      981 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_models/models/TEMPLATE_model.py
--rw-r--r--   0 runner    (1001) docker     (127)       67 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_models/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_models/models/model_SegResNet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1868 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_models/models/model_SwinUNetR.py
--rw-r--r--   0 runner    (1001) docker     (127)     3853 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_models/models/model_TRAILMAP.py
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_models/models/model_TRAILMAP_MS.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_models/models/model_VNet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_models/models/model_WNet.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_models/models/model_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 17:37:16.421882 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_models/models/pretrained/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_models/models/pretrained/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_models/models/pretrained/pretrained_model_urls.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 17:37:16.421882 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_models/models/unet/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_models/models/unet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19683 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_models/models/unet/buildingblocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6032 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_models/models/unet/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 17:37:16.421882 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_models/models/wnet/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_models/models/wnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9105 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_models/models/wnet/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5065 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_models/models/wnet/soft_Ncuts.py
--rw-r--r--   0 runner    (1001) docker     (127)    37497 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_models/worker_inference.py
--rw-r--r--   0 runner    (1001) docker     (127)    67942 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_models/worker_training.py
--rw-r--r--   0 runner    (1001) docker     (127)    11149 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_models/workers_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 17:37:16.425882 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_plugins/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18865 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_plugins/plugin_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    26739 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_plugins/plugin_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)    10316 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_plugins/plugin_crf.py
--rw-r--r--   0 runner    (1001) docker     (127)    23870 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_plugins/plugin_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_plugins/plugin_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    10859 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_plugins/plugin_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    36264 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_plugins/plugin_model_inference.py
--rw-r--r--   0 runner    (1001) docker     (127)    61979 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_plugins/plugin_model_training.py
--rw-r--r--   0 runner    (1001) docker     (127)    16713 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_plugins/plugin_review.py
--rw-r--r--   0 runner    (1001) docker     (127)    10102 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_plugins/plugin_review_dock.py
--rw-r--r--   0 runner    (1001) docker     (127)     7700 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_plugins/plugin_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    12482 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 17:37:16.425882 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/dev_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/dev_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14359 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/dev_scripts/artefact_labeling.py
--rw-r--r--   0 runner    (1001) docker     (127)    29035 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/dev_scripts/colab_training.py
--rw-r--r--   0 runner    (1001) docker     (127)    12203 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/dev_scripts/correct_labels.py
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/dev_scripts/crop_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    11993 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/dev_scripts/evaluate_labels.py
--rw-r--r--   0 runner    (1001) docker     (127)     4025 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/dev_scripts/remote_training.py
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/dev_scripts/sliding_window_voronoi.py
--rw-r--r--   0 runner    (1001) docker     (127)     4611 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/dev_scripts/thread_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/dev_scripts/whole_brain_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    50627 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)      988 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/napari.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      749 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 17:37:16.425882 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/res/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/res/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   495510 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/res/logo_alpha.png
--rw-r--r--   0 runner    (1001) docker     (127)       91 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    21526 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 17:37:16.429882 napari_cellseg3d-0.1.1rc1/napari_cellseg3d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9748 2023-12-14 17:37:16.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3915 2023-12-14 17:37:16.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-14 17:37:16.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2023-12-14 17:37:16.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      418 2023-12-14 17:37:16.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2023-12-14 17:37:16.000000 napari_cellseg3d-0.1.1rc1/napari_cellseg3d.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3535 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      315 2023-12-14 17:36:59.000000 napari_cellseg3d-0.1.1rc1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      736 2023-12-14 17:37:16.429882 napari_cellseg3d-0.1.1rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:55:46.183704 napari_cellseg3d-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9462 2024-04-02 08:55:46.183704 napari_cellseg3d-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6795 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:55:46.167704 napari_cellseg3d-0.1.2/napari_cellseg3d/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:55:46.171704 napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:55:46.171704 napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/res/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/res/test.png
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/test_base_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/test_dock_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/test_inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/test_labels_correction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/test_model_framework.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/test_plugin_inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/test_plugin_training.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/test_plugin_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/test_review.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4316 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/test_training.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7335 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/test_weight_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/test_wnet_training.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:55:46.175704 napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9598 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/crf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30959 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/instance_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13712 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/model_framework.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:55:46.175704 napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/models/TEMPLATE_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/models/model_SegResNet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/models/model_SwinUNetR.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/models/model_TRAILMAP.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/models/model_TRAILMAP_MS.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/models/model_VNet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/models/model_WNet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/models/model_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:55:46.175704 napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/models/pretrained/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/models/pretrained/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/models/pretrained/pretrained_model_urls.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:55:46.175704 napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/models/unet/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/models/unet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19683 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/models/unet/buildingblocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6032 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/models/unet/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:55:46.175704 napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/models/wnet/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/models/wnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9105 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/models/wnet/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5065 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/models/wnet/soft_Ncuts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37497 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/worker_inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68486 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/worker_training.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11149 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/workers_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:55:46.179704 napari_cellseg3d-0.1.2/napari_cellseg3d/code_plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18865 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_plugins/plugin_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27266 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_plugins/plugin_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10606 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_plugins/plugin_crf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23870 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_plugins/plugin_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_plugins/plugin_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10859 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_plugins/plugin_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36530 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_plugins/plugin_model_inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61986 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_plugins/plugin_model_training.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16713 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_plugins/plugin_review.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10102 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_plugins/plugin_review_dock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7700 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/code_plugins/plugin_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12482 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:55:46.179704 napari_cellseg3d-0.1.2/napari_cellseg3d/dev_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/dev_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14359 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/dev_scripts/artefact_labeling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29173 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/dev_scripts/colab_training.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12203 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/dev_scripts/correct_labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/dev_scripts/crop_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11993 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/dev_scripts/evaluate_labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/dev_scripts/remote_training.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/dev_scripts/sliding_window_voronoi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/dev_scripts/thread_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/dev_scripts/whole_brain_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53880 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/napari.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:55:46.179704 napari_cellseg3d-0.1.2/napari_cellseg3d/res/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/res/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   495510 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/res/logo_alpha.png
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21552 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/napari_cellseg3d/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:55:46.183704 napari_cellseg3d-0.1.2/napari_cellseg3d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9462 2024-04-02 08:55:46.000000 napari_cellseg3d-0.1.2/napari_cellseg3d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-04-02 08:55:46.000000 napari_cellseg3d-0.1.2/napari_cellseg3d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 08:55:46.000000 napari_cellseg3d-0.1.2/napari_cellseg3d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-02 08:55:46.000000 napari_cellseg3d-0.1.2/napari_cellseg3d.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-02 08:55:46.000000 napari_cellseg3d-0.1.2/napari_cellseg3d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-02 08:55:46.000000 napari_cellseg3d-0.1.2/napari_cellseg3d.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-02 08:55:33.000000 napari_cellseg3d-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-02 08:55:46.183704 napari_cellseg3d-0.1.2/setup.cfg
```

### Comparing `napari_cellseg3d-0.1.1rc1/LICENSE` & `napari_cellseg3d-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.1rc1/PKG-INFO` & `napari_cellseg3d-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari_cellseg3d
-Version: 0.1.1rc1
+Version: 0.1.2
 Summary: Plugin for cell segmentation in 3D
 Author-email: Cyril Achard <cyril.achard@epfl.ch>, Maxime Vidal <maxime.vidal@epfl.ch>, Mackenzie Mathis <mackenzie@post.harvard.edu>
 License: MIT
 Project-URL: Homepage, https://github.com/AdaptiveMotorControlLab/CellSeg3d
 Project-URL: Documentation, https://adaptivemotorcontrollab.github.io/cellseg3d-docs/res/welcome.html
 Project-URL: Issues, https://github.com/AdaptiveMotorControlLab/CellSeg3d/issues
 Classifier: Development Status :: 4 - Beta
@@ -80,17 +80,19 @@
 
 **Help us make the code better by reporting issues and adding your feature requests!**
 
 ----------------------------------
 
 ## News
 
-**New version : v0.1.1rc1**
+**New version : v0.1.2**
 
-Added :
+- Fixed manifest issue for PyPi
+
+Previous additions :
 
 - Improved training interface
 - Unsupervised model : WNet
   - Generate labels directly from raw data !
   - Can be trained in napari directly or in Colab
   - Pretrained weights for mesoSPIM whole-brain cell segmentation
 - WandB support (install wandb and login to use automatically when training)
@@ -102,31 +104,15 @@
 
 ## Demo
 
 ![demo](https://images.squarespace-cdn.com/content/v1/57f6d51c9f74566f55ecf271/0d16a71b-3ff2-477a-9d83-18d96cb1ce28/full_demo.gif?format=500w)
 
 ## Installation
 
-**Note** : we recommend using conda to create a new environment for the plugin.
-**M1 Mac users, please see the [M1 install section](#m1-mac-users)**
-
-    conda create --name napari-cellseg3d python=3.8
-    conda activate napari-cellseg3d
-
-You can install `napari-cellseg3d` via [pip]:
-
-    pip install napari-cellseg3d[all]
-
-OR directly via [napari-hub]:
-
-- Install napari from pip with `pip install "napari[all]"`,
-then from the “Plugins” menu within the napari application, select “Install/Uninstall Package(s)...”
-- Copy `napari-cellseg3d` and paste it where it says “Install by name/url…”
-- Click “Install”
-- Restart napari
+See the [Installation page] in the documentation for detailed instructions.
 
 ### M1 Mac users
 
 To avoid issues when installing on the ARM64 architecture, please follow these steps.
 
 1) Create a new conda env using the provided conda/napari_cellseg3d_m1.yml file :
 
@@ -177,14 +163,18 @@
 
 ## Issues
 
 If you encounter any problems, please [file an issue] along with a detailed description.
 
 ## Testing
 
+Before testing, install all requirements using ``pip install napari-cellseg3d[test]``.
+
+``pydensecrf`` is also required for testing.
+
 To run tests locally:
 
 - Locally : run ``pytest`` in the plugin folder
 - Locally with coverage : In the plugin folder, run ``coverage run --source=napari_cellseg3d -m pytest`` then ``coverage xml`` to generate a .xml coverage file.
 - With tox : run ``tox`` in the plugin folder (will simulate tests with several python and OS configs, requires substantial storage space)
 
 ## Contributing
@@ -212,15 +202,15 @@
 [Cookiecutter]: https://github.com/audreyr/cookiecutter
 [@napari]: https://github.com/napari
 [MIT]: http://opensource.org/licenses/MIT
 [cookiecutter-napari-plugin]: https://github.com/napari/cookiecutter-napari-plugin
 [tox]: https://tox.readthedocs.io/en/latest/
 [pip]: https://pypi.org/project/pip/
 [PyPI]: https://pypi.org/
-
+[Installation page]: https://adaptivemotorcontrollab.github.io/CellSeg3d/source/guides/installation_guide.html
 [the PyTorch website for installation instructions]: https://pytorch.org/get-started/locally/
 [PyTorch]: https://pytorch.org/get-started/locally/
 [MONAI's optional dependencies]: https://docs.monai.io/en/stable/installation.html#installing-the-recommended-dependencies
 [MONAI]: https://docs.monai.io/en/stable/installation.html#installing-the-recommended-dependencies
 
 ## Acknowledgements
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: napari_cellseg3d Version: 0.1.1rc1 Summary: Plugin
-for cell segmentation in 3D Author-email: Cyril Achard
+Metadata-Version: 2.1 Name: napari_cellseg3d Version: 0.1.2 Summary: Plugin for
+cell segmentation in 3D Author-email: Cyril Achard
 epfl.ch>, Maxime Vidal
 epfl.ch>, Mackenzie Mathis
 post.harvard.edu> License: MIT Project-URL: Homepage, https://github.com/
 AdaptiveMotorControlLab/CellSeg3d Project-URL: Documentation, https://
 adaptivemotorcontrollab.github.io/cellseg3d-docs/res/welcome.html Project-URL:
 Issues, https://github.com/AdaptiveMotorControlLab/CellSeg3d/issues Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Science/
@@ -46,39 +46,32 @@
 AdaptiveMotorControlLab/CellSeg3d) [![napari hub](https://img.shields.io/
 endpoint?url=https://api.napari-hub.org/shields/napari-cellseg3d)](https://
 www.napari-hub.org/plugins/napari-cellseg3d) A napari plugin for 3D cell
 segmentation: training, inference, and data review. In particular, this project
 was developed for analysis of mesoSPIM-acquired (cleared tissue + lightsheet)
 datasets. **Help us make the code better by reporting issues and adding your
 feature requests!** ---------------------------------- ## News **New version :
-v0.1.1rc1** Added : - Improved training interface - Unsupervised model : WNet -
-Generate labels directly from raw data ! - Can be trained in napari directly or
-in Colab - Pretrained weights for mesoSPIM whole-brain cell segmentation -
-WandB support (install wandb and login to use automatically when training) -
-Remade and improved documentation - Moved to Jupyter Book - Dedicated
-installation page, and working ARM64 install for macOS Silicon users - New
-utilities - Many small improvements and many bug fixes ## Demo ![demo](https://
-images.squarespace-cdn.com/content/v1/57f6d51c9f74566f55ecf271/0d16a71b-3ff2-
-477a-9d83-18d96cb1ce28/full_demo.gif?format=500w) ## Installation **Note** : we
-recommend using conda to create a new environment for the plugin. **M1 Mac
-users, please see the [M1 install section](#m1-mac-users)** conda create --name
-napari-cellseg3d python=3.8 conda activate napari-cellseg3d You can install
-`napari-cellseg3d` via [pip]: pip install napari-cellseg3d[all] OR directly via
-[napari-hub]: - Install napari from pip with `pip install "napari[all]"`, then
-from the âPluginsâ menu within the napari application, select âInstall/
-Uninstall Package(s)...â - Copy `napari-cellseg3d` and paste it where it says
-âInstall by name/urlâ¦â - Click âInstallâ - Restart napari ### M1 Mac
-users To avoid issues when installing on the ARM64 architecture, please follow
-these steps. 1) Create a new conda env using the provided conda/
-napari_cellseg3d_m1.yml file : git clone https://github.com/
-AdaptiveMotorControlLab/CellSeg3d.git cd CellSeg3d conda env create -f conda/
-napari_cellseg3d_m1.yml conda activate napari_cellseg3d_m1 2) Install the
-plugin. From repository root folder, run : pip install -e . OR directly via
-PyPi : pip install napari-cellseg3d OR directly via [napari-hub] (see
-Installation section above) ## Documentation Available at https://
+v0.1.2** - Fixed manifest issue for PyPi Previous additions : - Improved
+training interface - Unsupervised model : WNet - Generate labels directly from
+raw data ! - Can be trained in napari directly or in Colab - Pretrained weights
+for mesoSPIM whole-brain cell segmentation - WandB support (install wandb and
+login to use automatically when training) - Remade and improved documentation -
+Moved to Jupyter Book - Dedicated installation page, and working ARM64 install
+for macOS Silicon users - New utilities - Many small improvements and many bug
+fixes ## Demo ![demo](https://images.squarespace-cdn.com/content/v1/
+57f6d51c9f74566f55ecf271/0d16a71b-3ff2-477a-9d83-18d96cb1ce28/
+full_demo.gif?format=500w) ## Installation See the [Installation page] in the
+documentation for detailed instructions. ### M1 Mac users To avoid issues when
+installing on the ARM64 architecture, please follow these steps. 1) Create a
+new conda env using the provided conda/napari_cellseg3d_m1.yml file : git clone
+https://github.com/AdaptiveMotorControlLab/CellSeg3d.git cd CellSeg3d conda env
+create -f conda/napari_cellseg3d_m1.yml conda activate napari_cellseg3d_m1 2)
+Install the plugin. From repository root folder, run : pip install -e . OR
+directly via PyPi : pip install napari-cellseg3d OR directly via [napari-hub]
+(see Installation section above) ## Documentation Available at https://
 AdaptiveMotorControlLab.github.io/CellSeg3d You can also generate docs by
 running ``make html`` in the docs/ folder. ## Usage To use the plugin, please
 run: ``` napari ``` Then go into Plugins > napari-cellseg3d, and choose which
 tool to use. - **Review**: This module allows you to review your labels, from
 predictions or manual labeling, and correct them if needed. It then saves the
 status of each file in a csv, for easier monitoring. - **Inference**: This
 module allows you to use pre-trained segmentation algorithms on volumes to
@@ -91,35 +84,38 @@
 opposite. ## Requirements **Python 3.8 or 3.9 required.** Requires **
 [napari]**, **[PyTorch]** and **[MONAI]**. For PyTorch, please see [the PyTorch
 website for installation instructions]. A CUDA-capable GPU is not needed but
 very strongly recommended, especially for training. If you get errors from
 MONAI regarding missing readers, please see [MONAI's optional dependencies]
 page for instructions on getting the readers required by your images. ## Issues
 If you encounter any problems, please [file an issue] along with a detailed
-description. ## Testing To run tests locally: - Locally : run ``pytest`` in the
-plugin folder - Locally with coverage : In the plugin folder, run ``coverage
-run --source=napari_cellseg3d -m pytest`` then ``coverage xml`` to generate a
-.xml coverage file. - With tox : run ``tox`` in the plugin folder (will
-simulate tests with several python and OS configs, requires substantial storage
-space) ## Contributing Contributions are very welcome. Please ensure the
-coverage at least stays the same before you submit a pull request. For local
-installation from Github cloning, please run: ``` pip install -e . ``` ##
-License Distributed under the terms of the [MIT] license. "napari-cellseg3d" is
-free and open source software. [napari-hub]: https://www.napari-hub.org/
-plugins/napari-cellseg3d [file an issue]: https://github.com/
-AdaptiveMotorControlLab/CellSeg3d/issues [napari]: https://github.com/napari/
-napari [Cookiecutter]: https://github.com/audreyr/cookiecutter [@napari]:
-https://github.com/napari [MIT]: http://opensource.org/licenses/MIT
-[cookiecutter-napari-plugin]: https://github.com/napari/cookiecutter-napari-
-plugin [tox]: https://tox.readthedocs.io/en/latest/ [pip]: https://pypi.org/
-project/pip/ [PyPI]: https://pypi.org/ [the PyTorch website for installation
-instructions]: https://pytorch.org/get-started/locally/ [PyTorch]: https://
-pytorch.org/get-started/locally/ [MONAI's optional dependencies]: https://
-docs.monai.io/en/stable/installation.html#installing-the-recommended-
-dependencies [MONAI]: https://docs.monai.io/en/stable/
-installation.html#installing-the-recommended-dependencies ## Acknowledgements
-This plugin was developed by Cyril Achard, Maxime Vidal, Mackenzie Mathis. This
-work was funded, in part, from the Wyss Center to the [Mathis Laboratory of
-Adaptive Motor Control](https://www.mackenziemathislab.org/). Please refer to
-the documentation for full acknowledgements. ## Plugin base This [napari]
-plugin was generated with [Cookiecutter] using [@napari]'s [cookiecutter-
-napari-plugin] template.
+description. ## Testing Before testing, install all requirements using ``pip
+install napari-cellseg3d[test]``. ``pydensecrf`` is also required for testing.
+To run tests locally: - Locally : run ``pytest`` in the plugin folder - Locally
+with coverage : In the plugin folder, run ``coverage run --
+source=napari_cellseg3d -m pytest`` then ``coverage xml`` to generate a .xml
+coverage file. - With tox : run ``tox`` in the plugin folder (will simulate
+tests with several python and OS configs, requires substantial storage space)
+## Contributing Contributions are very welcome. Please ensure the coverage at
+least stays the same before you submit a pull request. For local installation
+from Github cloning, please run: ``` pip install -e . ``` ## License
+Distributed under the terms of the [MIT] license. "napari-cellseg3d" is free
+and open source software. [napari-hub]: https://www.napari-hub.org/plugins/
+napari-cellseg3d [file an issue]: https://github.com/AdaptiveMotorControlLab/
+CellSeg3d/issues [napari]: https://github.com/napari/napari [Cookiecutter]:
+https://github.com/audreyr/cookiecutter [@napari]: https://github.com/napari
+[MIT]: http://opensource.org/licenses/MIT [cookiecutter-napari-plugin]: https:/
+/github.com/napari/cookiecutter-napari-plugin [tox]: https://
+tox.readthedocs.io/en/latest/ [pip]: https://pypi.org/project/pip/ [PyPI]:
+https://pypi.org/ [Installation page]: https://
+adaptivemotorcontrollab.github.io/CellSeg3d/source/guides/
+installation_guide.html [the PyTorch website for installation instructions]:
+https://pytorch.org/get-started/locally/ [PyTorch]: https://pytorch.org/get-
+started/locally/ [MONAI's optional dependencies]: https://docs.monai.io/en/
+stable/installation.html#installing-the-recommended-dependencies [MONAI]:
+https://docs.monai.io/en/stable/installation.html#installing-the-recommended-
+dependencies ## Acknowledgements This plugin was developed by Cyril Achard,
+Maxime Vidal, Mackenzie Mathis. This work was funded, in part, from the Wyss
+Center to the [Mathis Laboratory of Adaptive Motor Control](https://
+www.mackenziemathislab.org/). Please refer to the documentation for full
+acknowledgements. ## Plugin base This [napari] plugin was generated with
+[Cookiecutter] using [@napari]'s [cookiecutter-napari-plugin] template.
```

### Comparing `napari_cellseg3d-0.1.1rc1/README.md` & `napari_cellseg3d-0.1.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -13,17 +13,19 @@
 
 **Help us make the code better by reporting issues and adding your feature requests!**
 
 ----------------------------------
 
 ## News
 
-**New version : v0.1.1rc1**
+**New version : v0.1.2**
 
-Added :
+- Fixed manifest issue for PyPi
+
+Previous additions :
 
 - Improved training interface
 - Unsupervised model : WNet
   - Generate labels directly from raw data !
   - Can be trained in napari directly or in Colab
   - Pretrained weights for mesoSPIM whole-brain cell segmentation
 - WandB support (install wandb and login to use automatically when training)
@@ -35,31 +37,15 @@
 
 ## Demo
 
 ![demo](https://images.squarespace-cdn.com/content/v1/57f6d51c9f74566f55ecf271/0d16a71b-3ff2-477a-9d83-18d96cb1ce28/full_demo.gif?format=500w)
 
 ## Installation
 
-**Note** : we recommend using conda to create a new environment for the plugin.
-**M1 Mac users, please see the [M1 install section](#m1-mac-users)**
-
-    conda create --name napari-cellseg3d python=3.8
-    conda activate napari-cellseg3d
-
-You can install `napari-cellseg3d` via [pip]:
-
-    pip install napari-cellseg3d[all]
-
-OR directly via [napari-hub]:
-
-- Install napari from pip with `pip install "napari[all]"`,
-then from the “Plugins” menu within the napari application, select “Install/Uninstall Package(s)...”
-- Copy `napari-cellseg3d` and paste it where it says “Install by name/url…”
-- Click “Install”
-- Restart napari
+See the [Installation page] in the documentation for detailed instructions.
 
 ### M1 Mac users
 
 To avoid issues when installing on the ARM64 architecture, please follow these steps.
 
 1) Create a new conda env using the provided conda/napari_cellseg3d_m1.yml file :
 
@@ -110,14 +96,18 @@
 
 ## Issues
 
 If you encounter any problems, please [file an issue] along with a detailed description.
 
 ## Testing
 
+Before testing, install all requirements using ``pip install napari-cellseg3d[test]``.
+
+``pydensecrf`` is also required for testing.
+
 To run tests locally:
 
 - Locally : run ``pytest`` in the plugin folder
 - Locally with coverage : In the plugin folder, run ``coverage run --source=napari_cellseg3d -m pytest`` then ``coverage xml`` to generate a .xml coverage file.
 - With tox : run ``tox`` in the plugin folder (will simulate tests with several python and OS configs, requires substantial storage space)
 
 ## Contributing
@@ -145,15 +135,15 @@
 [Cookiecutter]: https://github.com/audreyr/cookiecutter
 [@napari]: https://github.com/napari
 [MIT]: http://opensource.org/licenses/MIT
 [cookiecutter-napari-plugin]: https://github.com/napari/cookiecutter-napari-plugin
 [tox]: https://tox.readthedocs.io/en/latest/
 [pip]: https://pypi.org/project/pip/
 [PyPI]: https://pypi.org/
-
+[Installation page]: https://adaptivemotorcontrollab.github.io/CellSeg3d/source/guides/installation_guide.html
 [the PyTorch website for installation instructions]: https://pytorch.org/get-started/locally/
 [PyTorch]: https://pytorch.org/get-started/locally/
 [MONAI's optional dependencies]: https://docs.monai.io/en/stable/installation.html#installing-the-recommended-dependencies
 [MONAI]: https://docs.monai.io/en/stable/installation.html#installing-the-recommended-dependencies
 
 ## Acknowledgements
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -10,39 +10,32 @@
 AdaptiveMotorControlLab/CellSeg3d) [![napari hub](https://img.shields.io/
 endpoint?url=https://api.napari-hub.org/shields/napari-cellseg3d)](https://
 www.napari-hub.org/plugins/napari-cellseg3d) A napari plugin for 3D cell
 segmentation: training, inference, and data review. In particular, this project
 was developed for analysis of mesoSPIM-acquired (cleared tissue + lightsheet)
 datasets. **Help us make the code better by reporting issues and adding your
 feature requests!** ---------------------------------- ## News **New version :
-v0.1.1rc1** Added : - Improved training interface - Unsupervised model : WNet -
-Generate labels directly from raw data ! - Can be trained in napari directly or
-in Colab - Pretrained weights for mesoSPIM whole-brain cell segmentation -
-WandB support (install wandb and login to use automatically when training) -
-Remade and improved documentation - Moved to Jupyter Book - Dedicated
-installation page, and working ARM64 install for macOS Silicon users - New
-utilities - Many small improvements and many bug fixes ## Demo ![demo](https://
-images.squarespace-cdn.com/content/v1/57f6d51c9f74566f55ecf271/0d16a71b-3ff2-
-477a-9d83-18d96cb1ce28/full_demo.gif?format=500w) ## Installation **Note** : we
-recommend using conda to create a new environment for the plugin. **M1 Mac
-users, please see the [M1 install section](#m1-mac-users)** conda create --name
-napari-cellseg3d python=3.8 conda activate napari-cellseg3d You can install
-`napari-cellseg3d` via [pip]: pip install napari-cellseg3d[all] OR directly via
-[napari-hub]: - Install napari from pip with `pip install "napari[all]"`, then
-from the âPluginsâ menu within the napari application, select âInstall/
-Uninstall Package(s)...â - Copy `napari-cellseg3d` and paste it where it says
-âInstall by name/urlâ¦â - Click âInstallâ - Restart napari ### M1 Mac
-users To avoid issues when installing on the ARM64 architecture, please follow
-these steps. 1) Create a new conda env using the provided conda/
-napari_cellseg3d_m1.yml file : git clone https://github.com/
-AdaptiveMotorControlLab/CellSeg3d.git cd CellSeg3d conda env create -f conda/
-napari_cellseg3d_m1.yml conda activate napari_cellseg3d_m1 2) Install the
-plugin. From repository root folder, run : pip install -e . OR directly via
-PyPi : pip install napari-cellseg3d OR directly via [napari-hub] (see
-Installation section above) ## Documentation Available at https://
+v0.1.2** - Fixed manifest issue for PyPi Previous additions : - Improved
+training interface - Unsupervised model : WNet - Generate labels directly from
+raw data ! - Can be trained in napari directly or in Colab - Pretrained weights
+for mesoSPIM whole-brain cell segmentation - WandB support (install wandb and
+login to use automatically when training) - Remade and improved documentation -
+Moved to Jupyter Book - Dedicated installation page, and working ARM64 install
+for macOS Silicon users - New utilities - Many small improvements and many bug
+fixes ## Demo ![demo](https://images.squarespace-cdn.com/content/v1/
+57f6d51c9f74566f55ecf271/0d16a71b-3ff2-477a-9d83-18d96cb1ce28/
+full_demo.gif?format=500w) ## Installation See the [Installation page] in the
+documentation for detailed instructions. ### M1 Mac users To avoid issues when
+installing on the ARM64 architecture, please follow these steps. 1) Create a
+new conda env using the provided conda/napari_cellseg3d_m1.yml file : git clone
+https://github.com/AdaptiveMotorControlLab/CellSeg3d.git cd CellSeg3d conda env
+create -f conda/napari_cellseg3d_m1.yml conda activate napari_cellseg3d_m1 2)
+Install the plugin. From repository root folder, run : pip install -e . OR
+directly via PyPi : pip install napari-cellseg3d OR directly via [napari-hub]
+(see Installation section above) ## Documentation Available at https://
 AdaptiveMotorControlLab.github.io/CellSeg3d You can also generate docs by
 running ``make html`` in the docs/ folder. ## Usage To use the plugin, please
 run: ``` napari ``` Then go into Plugins > napari-cellseg3d, and choose which
 tool to use. - **Review**: This module allows you to review your labels, from
 predictions or manual labeling, and correct them if needed. It then saves the
 status of each file in a csv, for easier monitoring. - **Inference**: This
 module allows you to use pre-trained segmentation algorithms on volumes to
@@ -55,35 +48,38 @@
 opposite. ## Requirements **Python 3.8 or 3.9 required.** Requires **
 [napari]**, **[PyTorch]** and **[MONAI]**. For PyTorch, please see [the PyTorch
 website for installation instructions]. A CUDA-capable GPU is not needed but
 very strongly recommended, especially for training. If you get errors from
 MONAI regarding missing readers, please see [MONAI's optional dependencies]
 page for instructions on getting the readers required by your images. ## Issues
 If you encounter any problems, please [file an issue] along with a detailed
-description. ## Testing To run tests locally: - Locally : run ``pytest`` in the
-plugin folder - Locally with coverage : In the plugin folder, run ``coverage
-run --source=napari_cellseg3d -m pytest`` then ``coverage xml`` to generate a
-.xml coverage file. - With tox : run ``tox`` in the plugin folder (will
-simulate tests with several python and OS configs, requires substantial storage
-space) ## Contributing Contributions are very welcome. Please ensure the
-coverage at least stays the same before you submit a pull request. For local
-installation from Github cloning, please run: ``` pip install -e . ``` ##
-License Distributed under the terms of the [MIT] license. "napari-cellseg3d" is
-free and open source software. [napari-hub]: https://www.napari-hub.org/
-plugins/napari-cellseg3d [file an issue]: https://github.com/
-AdaptiveMotorControlLab/CellSeg3d/issues [napari]: https://github.com/napari/
-napari [Cookiecutter]: https://github.com/audreyr/cookiecutter [@napari]:
-https://github.com/napari [MIT]: http://opensource.org/licenses/MIT
-[cookiecutter-napari-plugin]: https://github.com/napari/cookiecutter-napari-
-plugin [tox]: https://tox.readthedocs.io/en/latest/ [pip]: https://pypi.org/
-project/pip/ [PyPI]: https://pypi.org/ [the PyTorch website for installation
-instructions]: https://pytorch.org/get-started/locally/ [PyTorch]: https://
-pytorch.org/get-started/locally/ [MONAI's optional dependencies]: https://
-docs.monai.io/en/stable/installation.html#installing-the-recommended-
-dependencies [MONAI]: https://docs.monai.io/en/stable/
-installation.html#installing-the-recommended-dependencies ## Acknowledgements
-This plugin was developed by Cyril Achard, Maxime Vidal, Mackenzie Mathis. This
-work was funded, in part, from the Wyss Center to the [Mathis Laboratory of
-Adaptive Motor Control](https://www.mackenziemathislab.org/). Please refer to
-the documentation for full acknowledgements. ## Plugin base This [napari]
-plugin was generated with [Cookiecutter] using [@napari]'s [cookiecutter-
-napari-plugin] template.
+description. ## Testing Before testing, install all requirements using ``pip
+install napari-cellseg3d[test]``. ``pydensecrf`` is also required for testing.
+To run tests locally: - Locally : run ``pytest`` in the plugin folder - Locally
+with coverage : In the plugin folder, run ``coverage run --
+source=napari_cellseg3d -m pytest`` then ``coverage xml`` to generate a .xml
+coverage file. - With tox : run ``tox`` in the plugin folder (will simulate
+tests with several python and OS configs, requires substantial storage space)
+## Contributing Contributions are very welcome. Please ensure the coverage at
+least stays the same before you submit a pull request. For local installation
+from Github cloning, please run: ``` pip install -e . ``` ## License
+Distributed under the terms of the [MIT] license. "napari-cellseg3d" is free
+and open source software. [napari-hub]: https://www.napari-hub.org/plugins/
+napari-cellseg3d [file an issue]: https://github.com/AdaptiveMotorControlLab/
+CellSeg3d/issues [napari]: https://github.com/napari/napari [Cookiecutter]:
+https://github.com/audreyr/cookiecutter [@napari]: https://github.com/napari
+[MIT]: http://opensource.org/licenses/MIT [cookiecutter-napari-plugin]: https:/
+/github.com/napari/cookiecutter-napari-plugin [tox]: https://
+tox.readthedocs.io/en/latest/ [pip]: https://pypi.org/project/pip/ [PyPI]:
+https://pypi.org/ [Installation page]: https://
+adaptivemotorcontrollab.github.io/CellSeg3d/source/guides/
+installation_guide.html [the PyTorch website for installation instructions]:
+https://pytorch.org/get-started/locally/ [PyTorch]: https://pytorch.org/get-
+started/locally/ [MONAI's optional dependencies]: https://docs.monai.io/en/
+stable/installation.html#installing-the-recommended-dependencies [MONAI]:
+https://docs.monai.io/en/stable/installation.html#installing-the-recommended-
+dependencies ## Acknowledgements This plugin was developed by Cyril Achard,
+Maxime Vidal, Mackenzie Mathis. This work was funded, in part, from the Wyss
+Center to the [Mathis Laboratory of Adaptive Motor Control](https://
+www.mackenziemathislab.org/). Please refer to the documentation for full
+acknowledgements. ## Plugin base This [napari] plugin was generated with
+[Cookiecutter] using [@napari]'s [cookiecutter-napari-plugin] template.
```

### Comparing `napari_cellseg3d-0.1.1rc1/napari_cellseg3d/_tests/fixtures.py` & `napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.1rc1/napari_cellseg3d/_tests/test_base_plugin.py` & `napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/test_base_plugin.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.1rc1/napari_cellseg3d/_tests/test_dock_widget.py` & `napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/test_dock_widget.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.1rc1/napari_cellseg3d/_tests/test_inference.py` & `napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/test_inference.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.1rc1/napari_cellseg3d/_tests/test_labels_correction.py` & `napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/test_labels_correction.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.1rc1/napari_cellseg3d/_tests/test_model_framework.py` & `napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/test_model_framework.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.1rc1/napari_cellseg3d/_tests/test_models.py` & `napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/test_models.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.1rc1/napari_cellseg3d/_tests/test_plugin_inference.py` & `napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/test_plugin_inference.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.1rc1/napari_cellseg3d/_tests/test_plugin_training.py` & `napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/test_plugin_training.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.1rc1/napari_cellseg3d/_tests/test_plugin_utils.py` & `napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/test_plugin_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from napari_cellseg3d.utils import rand_gen
 
 
 def test_utils_plugin(make_napari_viewer_proxy):
     view = make_napari_viewer_proxy()
     widget = Utilities(view)
 
-    image = rand_gen.random((10, 10, 10)).astype(np.uint8)
+    image = rand_gen.random((10, 10, 10))  # .astype(np.uint8)
     image_layer = view.add_image(image, name="image")
     label_layer = view.add_labels(image.astype(np.uint8), name="labels")
 
     view.window.add_dock_widget(widget)
     view.dims.ndisplay = 3
     for i, utils_name in enumerate(UTILITIES_WIDGETS.keys()):
         widget.utils_choice.setCurrentIndex(i)
```

### Comparing `napari_cellseg3d-0.1.1rc1/napari_cellseg3d/_tests/test_plugins.py` & `napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/test_plugins.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.1rc1/napari_cellseg3d/_tests/test_review.py` & `napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/test_review.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.1rc1/napari_cellseg3d/_tests/test_training.py` & `napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/test_training.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 from napari_cellseg3d.code_models.models.model_test import TestModel
 from napari_cellseg3d.code_models.workers_utils import TrainingReport
 from napari_cellseg3d.code_plugins.plugin_model_training import (
     Trainer,
 )
 from napari_cellseg3d.config import MODEL_LIST
 
+WANDB_MODE = "disabled"
+
 im_path = Path(__file__).resolve().parent / "res/test.tif"
 im_path_str = str(im_path)
 lab_path = Path(__file__).resolve().parent / "res/test_labels.tif"
 lab_path_str = str(lab_path)
 
 
 def test_supervised_training(make_napari_viewer_proxy):
```

### Comparing `napari_cellseg3d-0.1.1rc1/napari_cellseg3d/_tests/test_utils.py` & `napari_cellseg3d-0.1.2/napari_cellseg3d/_tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_models/__init__.py` & `napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/__init__.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_models/crf.py` & `napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/crf.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_models/instance_segmentation.py` & `napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/instance_segmentation.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_models/model_framework.py` & `napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/model_framework.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_models/models/TEMPLATE_model.py` & `napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/models/TEMPLATE_model.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_models/models/model_SegResNet.py` & `napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/models/model_SegResNet.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_models/models/model_SwinUNetR.py` & `napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/models/model_SwinUNetR.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_models/models/model_TRAILMAP.py` & `napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/models/model_TRAILMAP.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_models/models/model_TRAILMAP_MS.py` & `napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/models/model_TRAILMAP_MS.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_models/models/model_VNet.py` & `napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/models/model_VNet.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_models/models/model_WNet.py` & `napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/models/model_WNet.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_models/models/model_test.py` & `napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/models/model_test.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_models/models/pretrained/pretrained_model_urls.json` & `napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/models/pretrained/pretrained_model_urls.json`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_models/models/unet/buildingblocks.py` & `napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/models/unet/buildingblocks.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_models/models/unet/model.py` & `napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/models/unet/model.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_models/models/wnet/model.py` & `napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/models/wnet/model.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_models/models/wnet/soft_Ncuts.py` & `napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/models/wnet/soft_Ncuts.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_models/worker_inference.py` & `napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/worker_inference.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_models/worker_training.py` & `napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/worker_training.py`

 * *Files 2% similar despite different names*

```diff
@@ -421,16 +421,18 @@
             set_track_meta(False)
             ##############
             if WANDB_INSTALLED:
                 config_dict = self.config.__dict__
                 logger.debug(f"wandb config : {config_dict}")
                 wandb.init(
                     config=config_dict,
-                    project="CellSeg3D",
+                    project="CellSeg3D - WNet",
+                    name=f"WNet_training - {utils.get_date_time()}",
                     mode=self.wandb_config.mode,
+                    tags=["WNet", "training"],
                 )
 
             set_determinism(seed=self.config.deterministic_config.seed)
             torch.use_deterministic_algorithms(True, warn_only=True)
 
             device = self.config.device
 
@@ -781,15 +783,19 @@
             optimizer = None
             del optimizer
             criterionE = None
             del criterionE
             criterionW = None
             del criterionW
             torch.cuda.empty_cache()
+            if WANDB_INSTALLED:
+                wandb.finish()
         except Exception as e:
+            if WANDB_INSTALLED:
+                wandb.finish()
             msg = f"Training failed with exception: {e}"
             self.log(msg)
             self.raise_error(e, msg)
             self.quit()
             raise e
 
     def eval(self, model, epoch) -> TrainingReport:
@@ -1113,14 +1119,16 @@
             if WANDB_INSTALLED:
                 config_dict = self.config.__dict__
                 logger.debug(f"wandb config : {config_dict}")
                 try:
                     wandb.init(
                         config=config_dict,
                         project="CellSeg3D",
+                        name=f"{model_config.name}_supervised_training - {utils.get_date_time()}",
+                        tags=[f"{model_config.name}", "supervised"],
                         mode=self.wandb_config.mode,
                     )
                 except AttributeError:
                     logger.warning(
                         "Could not initialize wandb."
                         "This might be due to running napari in a folder where there is a directory named 'wandb'."
                         "Aborting, please run napari in a different folder or install wandb. Sorry for the inconvenience."
@@ -1718,14 +1726,17 @@
             self.log("Saving last model")
             torch.save(
                 model.state_dict(),
                 Path(self.config.results_path_folder) / Path(weights_filename),
             )
             self.log("Saving complete, exiting")
             model.to("cpu")
+
+            if WANDB_INSTALLED:
+                wandb.finish()
             # clear (V)RAM
             model = None
             del model
             train_loader = None
             del train_loader
             validation_loader = None
             del validation_loader
@@ -1733,11 +1744,13 @@
             del optimizer
             scheduler = None
             del scheduler
             if device.type == "cuda":
                 torch.cuda.empty_cache()
 
         except Exception as e:
+            if WANDB_INSTALLED:
+                wandb.finish()
             self.raise_error(e, "Error in training")
             self.quit()
         finally:
             self.quit()
```

### Comparing `napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_models/workers_utils.py` & `napari_cellseg3d-0.1.2/napari_cellseg3d/code_models/workers_utils.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_plugins/plugin_base.py` & `napari_cellseg3d-0.1.2/napari_cellseg3d/code_plugins/plugin_base.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_plugins/plugin_convert.py` & `napari_cellseg3d-0.1.2/napari_cellseg3d/code_plugins/plugin_convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -359,14 +359,20 @@
         self.results_path = str(self.save_path)
         self.results_filewidget.text_field.setText(self.results_path)
         self.results_filewidget.check_ready()
 
         self.container = self._build()
 
         self.function = clear_small_objects
+        self._set_tooltips()
+
+    def _set_tooltips(self):
+        self.size_for_removal_counter.setToolTip(
+            "Size of the objects to remove, in pixels."
+        )
 
     def _build(self):
         container = ui.ContainerWidget()
 
         ui.add_widgets(
             self.data_panel.layout,
             [
@@ -643,14 +649,23 @@
         self.results_path = str(self.save_path)
         self.results_filewidget.text_field.setText(self.results_path)
         self.results_filewidget.check_ready()
 
         self.container = self._build()
         self.function = threshold
 
+        self._set_tooltips()
+
+    def _set_tooltips(self):
+        self.binarize_counter.setToolTip(
+            "Value to use as threshold for binarization."
+            "For labels, use the highest ID you want to keep. All lower IDs will be removed."
+            "For images, use the intensity value (pixel value) to threshold the image."
+        )
+
     def _build(self):
         container = ui.ContainerWidget()
 
         ui.add_widgets(
             self.data_panel.layout,
             [
                 self.binarize_counter.label,
```

### Comparing `napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_plugins/plugin_crf.py` & `napari_cellseg3d-0.1.2/napari_cellseg3d/code_plugins/plugin_crf.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,14 +47,21 @@
         )
         #######
         self._build()
         self._set_tooltips()
 
     def _build(self):
         if not CRF_INSTALLED:
+            self.sa_choice.setVisible(False)
+            self.sb_choice.setVisible(False)
+            self.sg_choice.setVisible(False)
+            self.w1_choice.setVisible(False)
+            self.w2_choice.setVisible(False)
+            self.n_iter_choice.setVisible(False)
+            ###
             ui.add_widgets(
                 self.layout,
                 [
                     ui.make_label(
                         "ERROR: CRF not installed.\nPlease refer to the documentation to install it."
                     ),
                 ],
```

### Comparing `napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_plugins/plugin_crop.py` & `napari_cellseg3d-0.1.2/napari_cellseg3d/code_plugins/plugin_crop.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_plugins/plugin_helper.py` & `napari_cellseg3d-0.1.2/napari_cellseg3d/code_plugins/plugin_helper.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         self.logo_label.setIconSize(QSize(200, 200))
         self.logo_label.setStyleSheet(
             "QPushButton { background-color: transparent }"
         )
         self.logo_label.setToolTip("Open Github page")
 
         self.info_label = ui.make_label(
-            f"You are using napari-cellseg3d v.{'0.1.1rc1'}\n\n"
+            f"You are using napari-cellseg3d v.{'0.1.2'}\n\n"
             f"Plugin for cell segmentation developed\n"
             f"by the Mathis Lab of Adaptive Motor Control\n\n"
             f"Code by :\nCyril Achard\nMaxime Vidal\nJessy Lauer\nMackenzie Mathis\n"
             f"\nReleased under the MIT license",
             self,
         )
```

### Comparing `napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_plugins/plugin_metrics.py` & `napari_cellseg3d-0.1.2/napari_cellseg3d/code_plugins/plugin_metrics.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_plugins/plugin_model_inference.py` & `napari_cellseg3d-0.1.2/napari_cellseg3d/code_plugins/plugin_model_inference.py`

 * *Files 2% similar despite different names*

```diff
@@ -277,14 +277,15 @@
         )
         self.model_input_size.setToolTip(
             "Image size on which the model has been trained (default : 128)\n"
             "DO NOT CHANGE if you are using the provided pre-trained weights"
         )
 
         thresh_desc = (
+            "NOT RECOMMENDED ON FIRST RUN - check results without first!\n"
             "Thresholding : all values in the image below the chosen probability"
             " threshold will be set to 0, and all others to 1."
         )
 
         self.thresholding_checkbox.setToolTip(thresh_desc)
         self.thresholding_slider.tooltips = thresh_desc
         self.use_window_choice.setToolTip(
@@ -297,14 +298,15 @@
         )
         self.window_overlap_slider.tooltips = "Percentage of overlap between windows to use when using sliding window"
 
         self.keep_data_on_cpu_box.setToolTip(
             "If enabled, data will be kept on the RAM rather than the VRAM.\nCan avoid out of memory issues with CUDA"
         )
         self.use_instance_choice.setToolTip(
+            "NOT RECOMMENDED ON FIRST RUN - check results without first!\n"
             "Instance segmentation will convert instance (0/1) labels to labels"
             " that attempt to assign an unique ID to each cell."
         )
 
         self.save_stats_to_csv_box.setToolTip(
             "Will save several statistics for each object to a csv in the results folder. Stats include : "
             "volume, centroid coordinates, sphericity"
@@ -649,14 +651,16 @@
                 result.semantic_segmentation, 0.5
             )
             index_channel_sorted = np.argsort(fractions_per_channel)
             for channel in index_channel_sorted:
                 if result.semantic_segmentation[channel].sum() > 0:
                     index_channel_least_labelled = channel
                     break
+                # if no channel has any label, use the first one
+                index_channel_least_labelled = 0
             viewer.dims.set_point(
                 0, index_channel_least_labelled
             )  # TODO(cyril: check if this is always the right axis
 
         if result.crf_results is not None and not isinstance(
             result.crf_results, Exception
         ):
```

### Comparing `napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_plugins/plugin_model_training.py` & `napari_cellseg3d-0.1.2/napari_cellseg3d/code_plugins/plugin_model_training.py`

 * *Files 1% similar despite different names*

```diff
@@ -1243,15 +1243,15 @@
         self.log.print_and_log("Saving log")
         self.save_log_to_path(self.worker_config.results_path_folder)
 
         self.log.print_and_log("Done")
         self.log.print_and_log("*" * 10)
         try:
             self._make_csv()
-        except ValueError as e:
+        except (ValueError, KeyError) as e:
             logger.warning(f"Error while saving CSV report: {e}")
 
         self.start_btn.setText("Start")
         [btn.setVisible(True) for btn in self.close_buttons]
 
         if self.config.save_as_zip:
             shutil.make_archive(
@@ -1371,19 +1371,19 @@
         if len(self.loss_1_values) == 0 or self.loss_1_values is None:
             logger.warning("No loss values to add to csv !")
             return
 
         try:
             self.loss_1_values["Loss"]
             supervised = True
-        except KeyError("Loss"):
+        except KeyError:
             try:
                 self.loss_1_values["SoftNCuts"]
                 supervised = False
-            except KeyError("SoftNCuts") as e:
+            except KeyError as e:
                 raise KeyError(
                     "Error when making csv. Check loss dict keys ?"
                 ) from e
 
         if supervised:
             val = utils.fill_list_in_between(
                 self.loss_2_values,
@@ -1394,16 +1394,16 @@
             self.df = pd.DataFrame(
                 {
                     "epoch": size_column,
                     "loss": self.loss_1_values["Loss"],
                     "validation": val,
                 }
             )
-            if len(val) != len(self.loss_1_values):
-                err = f"Validation and loss values don't have the same length ! Got {len(val)} and {len(self.loss_1_values)}"
+            if len(val) != len(self.loss_1_values["Loss"]):
+                err = f"Validation and loss values don't have the same length ! Got {len(val)} and {len(self.loss_1_values['Loss'])}"
                 logger.error(err)
                 raise ValueError(err)
         else:
             ncuts_loss = self.loss_1_values["SoftNCuts"]
             try:
                 dice_metric = self.loss_1_values["Dice metric"]
                 self.df = pd.DataFrame(
```

### Comparing `napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_plugins/plugin_review.py` & `napari_cellseg3d-0.1.2/napari_cellseg3d/code_plugins/plugin_review.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_plugins/plugin_review_dock.py` & `napari_cellseg3d-0.1.2/napari_cellseg3d/code_plugins/plugin_review_dock.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.1rc1/napari_cellseg3d/code_plugins/plugin_utilities.py` & `napari_cellseg3d-0.1.2/napari_cellseg3d/code_plugins/plugin_utilities.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.1rc1/napari_cellseg3d/config.py` & `napari_cellseg3d-0.1.2/napari_cellseg3d/config.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.1rc1/napari_cellseg3d/dev_scripts/artefact_labeling.py` & `napari_cellseg3d-0.1.2/napari_cellseg3d/dev_scripts/artefact_labeling.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.1rc1/napari_cellseg3d/dev_scripts/colab_training.py` & `napari_cellseg3d-0.1.2/napari_cellseg3d/dev_scripts/colab_training.py`

 * *Files 1% similar despite different names*

```diff
@@ -326,15 +326,17 @@
             ##############
             if WANDB_INSTALLED:
                 config_dict = self.config.__dict__
                 logger.debug(f"wandb config : {config_dict}")
                 wandb.init(
                     config=config_dict,
                     project="CellSeg3D (Colab)",
+                    name=f"{self.config.model_info.name} training - {utils.get_date_time()}",
                     mode=self.wandb_config.mode,
+                    tags=["WNet", "Colab"],
                 )
 
             set_determinism(seed=self.config.deterministic_config.seed)
             torch.use_deterministic_algorithms(True, warn_only=True)
 
             device = self.config.device
```

### Comparing `napari_cellseg3d-0.1.1rc1/napari_cellseg3d/dev_scripts/correct_labels.py` & `napari_cellseg3d-0.1.2/napari_cellseg3d/dev_scripts/correct_labels.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.1rc1/napari_cellseg3d/dev_scripts/crop_data.py` & `napari_cellseg3d-0.1.2/napari_cellseg3d/dev_scripts/crop_data.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.1rc1/napari_cellseg3d/dev_scripts/evaluate_labels.py` & `napari_cellseg3d-0.1.2/napari_cellseg3d/dev_scripts/evaluate_labels.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.1rc1/napari_cellseg3d/dev_scripts/remote_training.py` & `napari_cellseg3d-0.1.2/napari_cellseg3d/dev_scripts/remote_training.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.1rc1/napari_cellseg3d/dev_scripts/sliding_window_voronoi.py` & `napari_cellseg3d-0.1.2/napari_cellseg3d/dev_scripts/sliding_window_voronoi.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.1rc1/napari_cellseg3d/dev_scripts/thread_test.py` & `napari_cellseg3d-0.1.2/napari_cellseg3d/dev_scripts/thread_test.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.1rc1/napari_cellseg3d/dev_scripts/whole_brain_utils.py` & `napari_cellseg3d-0.1.2/napari_cellseg3d/dev_scripts/whole_brain_utils.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.1rc1/napari_cellseg3d/interface.py` & `napari_cellseg3d-0.1.2/napari_cellseg3d/interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """User interface functions and aliases."""
+import contextlib
 import threading
 from functools import partial
 from typing import List, Optional
+from warnings import warn
 
 import napari
 
 # Qt
 # from qtpy.QtCore import QtWarningMsg
 from qtpy import QtCore
 from qtpy.QtCore import QObject, Qt, QUrl
@@ -800,51 +802,122 @@
         self.layer_list = DropdownMenu(
             parent=self, text_label=name, fixed=False
         )
         self.layer_description = make_label("Shape:", parent=self)
         self.layer_description.setVisible(False)
         # self.layer_list.setSizeAdjustPolicy(QComboBox.AdjustToContents) # use tooltip instead ?
 
+        # connect to LayerList events
         self._viewer.layers.events.inserted.connect(partial(self._add_layer))
         self._viewer.layers.events.removed.connect(partial(self._remove_layer))
+        self._viewer.layers.events.changed.connect(self._check_for_layers)
 
+        # update self.layer_list when layers are added or removed
         self.layer_list.currentIndexChanged.connect(self._update_tooltip)
         self.layer_list.currentTextChanged.connect(self._update_description)
 
         add_widgets(
             self.layout,
             [self.layer_list.label, self.layer_list, self.layer_description],
         )
         self._check_for_layers()
 
+    def _get_all_layers(self):
+        return [
+            self.layer_list.itemText(i) for i in range(self.layer_list.count())
+        ]
+
     def _check_for_layers(self):
+        """Check for layers of the correct type and update the dropdown menu.
+
+        Also removes layers that have been removed from the viewer.
+        """
         for layer in self._viewer.layers:
-            if isinstance(layer, self.layer_type):
+            layer.events.name.connect(self._rename_layer)
+
+            if (
+                isinstance(layer, self.layer_type)
+                and layer.name not in self._get_all_layers()
+            ):
+                logger.debug(
+                    f"Layer {layer.name} - List : {self._get_all_layers()}"
+                )
+                # add new layers of correct type
                 self.layer_list.addItem(layer.name)
+                logger.debug(f"Layer {layer.name} has been added to the menu")
+                # break
+                # once added, check again for previously renamed layers
+                self._check_for_removed_layer(layer)
+
+            if layer.name in self._get_all_layers() and not isinstance(
+                layer, self.layer_type
+            ):
+                # remove layers of incorrect type
+                index = self.layer_list.findText(layer.name)
+                self.layer_list.removeItem(index)
+                logger.debug(
+                    f"Layer {layer.name} has been removed from the menu"
+                )
+
+        self._check_for_removed_layers()
+        self._update_tooltip()
+        self._update_description()
+
+    def _check_for_removed_layer(self, layer):
+        """Check if a specific layer has been removed from the viewer and must be removed from the menu."""
+        if isinstance(layer, str):
+            name = layer
+        elif isinstance(layer, self.layer_type):
+            name = layer.name
+        else:
+            logger.warning("Layer is not a string or a valid napari layer")
+            return
+
+        if name in self._get_all_layers() and name not in [
+            l.name for l in self._viewer.layers
+        ]:
+            index = self.layer_list.findText(name)
+            self.layer_list.removeItem(index)
+            logger.debug(f"Layer {name} has been removed from the menu")
+
+    def _check_for_removed_layers(self):
+        """Check for layers that have been removed from the viewer and must be removed from the menu."""
+        for layer in self._get_all_layers():
+            self._check_for_removed_layer(layer)
 
     def _update_tooltip(self):
         self.layer_list.setToolTip(self.layer_list.currentText())
 
     def _update_description(self):
         try:
             if self.layer_list.currentText() != "":
-                self.layer_description.setVisible(True)
-                shape_desc = f"Shape : {self.layer_data().shape}"
-                self.layer_description.setText(shape_desc)
+                try:
+                    shape_desc = f"Shape : {self.layer_data().shape}"
+                    self.layer_description.setText(shape_desc)
+                    self.layer_description.setVisible(True)
+                except AttributeError:
+                    self.layer_description.setVisible(False)
             else:
                 self.layer_description.setVisible(False)
         except KeyError:
             self.layer_description.setVisible(False)
 
     def _add_layer(self, event):
         inserted_layer = event.value
 
         if isinstance(inserted_layer, self.layer_type):
             self.layer_list.addItem(inserted_layer.name)
 
+        # check for renaming
+        inserted_layer.events.name.connect(self._rename_layer)
+
+    def _rename_layer(self, _):
+        # on layer rename, check for removed/new layers
+        self._check_for_layers()
+
     def _remove_layer(self, event):
         removed_layer = event.value
 
         if isinstance(
             removed_layer, self.layer_type
         ) and removed_layer.name in [
             self.layer_list.itemText(i) for i in range(self.layer_list.count())
@@ -863,23 +936,32 @@
         try:
             return self._viewer.layers[self.layer_name()]
         except ValueError:
             return None
 
     def layer_name(self):
         """Returns the name of the layer selected in the dropdown menu."""
-        return self.layer_list.currentText()
+        try:
+            return self.layer_list.currentText()
+        except (KeyError, ValueError):
+            logger.warning("Layer list is empty")
+            return None
 
     def layer_data(self):
         """Returns the data of the layer selected in the dropdown menu."""
         if self.layer_list.count() < 1:
             logger.debug("Layer list is empty")
             return None
-
-        return self.layer().data
+        try:
+            return self.layer().data
+        except (KeyError, ValueError):
+            msg = f"Layer {self.layer_name()} has no data. Layer might have been renamed or removed."
+            logger.warning(msg)
+            warn(msg, stacklevel=1)
+            return None
 
 
 class FilePathWidget(QWidget):  # TODO include load as folder
     """Widget to handle the choice of file paths for data throughout the plugin.
 
     Provides the following elements :
         An "Open" button to show a file dialog (defined externally)
```

### Comparing `napari_cellseg3d-0.1.1rc1/napari_cellseg3d/napari.yaml` & `napari_cellseg3d-0.1.2/napari_cellseg3d/napari.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-name: napari-cellseg3d
+name: napari_cellseg3d
 display_name: CellSeg3D
 schema_version: 0.0.4
 
 contributions:
   commands:
-  - id: napari-cellseg3d.load
+  - id: napari_cellseg3d.load
     title: Create reviewer
     python_name: napari_cellseg3d.plugins:Reviewer
 
-  - id: napari-cellseg3d.help
+  - id: napari_cellseg3d.help
     title: Create Help
     python_name: napari_cellseg3d.plugins:Helper
 
-  - id: napari-cellseg3d.utils
+  - id: napari_cellseg3d.utils
     title:  Create utilities
     python_name: napari_cellseg3d.plugins:Utilities
 
-  - id: napari-cellseg3d.infer
+  - id: napari_cellseg3d.infer
     title: Create Inference widget
     python_name: napari_cellseg3d.plugins:Inferer
 
-  - id: napari-cellseg3d.train
+  - id: napari_cellseg3d.train
     title: Create Trainer widget
     python_name: napari_cellseg3d.plugins:Trainer
 
 
   widgets:
-  - command: napari-cellseg3d.load
+  - command: napari_cellseg3d.load
     display_name: Review
 
-  - command: napari-cellseg3d.infer
+  - command: napari_cellseg3d.infer
     display_name: Inference
 
-  - command: napari-cellseg3d.train
+  - command: napari_cellseg3d.train
     display_name: Training
 
-  - command: napari-cellseg3d.utils
+  - command: napari_cellseg3d.utils
     display_name: Utilities
 
-  - command: napari-cellseg3d.help
+  - command: napari_cellseg3d.help
     display_name: Help/About...
```

### Comparing `napari_cellseg3d-0.1.1rc1/napari_cellseg3d/plugins.py` & `napari_cellseg3d-0.1.2/napari_cellseg3d/plugins.py`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.1rc1/napari_cellseg3d/res/logo_alpha.png` & `napari_cellseg3d-0.1.2/napari_cellseg3d/res/logo_alpha.png`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.1rc1/napari_cellseg3d/utils.py` & `napari_cellseg3d-0.1.2/napari_cellseg3d/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from monai.transforms import Zoom
 from numpy.random import PCG64, Generator
 from tifffile import imread, imwrite
 
 LOGGER = logging.getLogger(__name__)
 ###############
 # Global logging level setting
+# SET TO INFO FOR RELEASE
 # LOGGER.setLevel(logging.DEBUG)
 LOGGER.setLevel(logging.INFO)
 ###############
 """
 utils.py
 ====================================
 Definitions of utility functions, classes, and variables
```

### Comparing `napari_cellseg3d-0.1.1rc1/napari_cellseg3d.egg-info/PKG-INFO` & `napari_cellseg3d-0.1.2/napari_cellseg3d.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: napari-cellseg3d
-Version: 0.1.1rc1
+Name: napari_cellseg3d
+Version: 0.1.2
 Summary: Plugin for cell segmentation in 3D
 Author-email: Cyril Achard <cyril.achard@epfl.ch>, Maxime Vidal <maxime.vidal@epfl.ch>, Mackenzie Mathis <mackenzie@post.harvard.edu>
 License: MIT
 Project-URL: Homepage, https://github.com/AdaptiveMotorControlLab/CellSeg3d
 Project-URL: Documentation, https://adaptivemotorcontrollab.github.io/cellseg3d-docs/res/welcome.html
 Project-URL: Issues, https://github.com/AdaptiveMotorControlLab/CellSeg3d/issues
 Classifier: Development Status :: 4 - Beta
@@ -80,17 +80,19 @@
 
 **Help us make the code better by reporting issues and adding your feature requests!**
 
 ----------------------------------
 
 ## News
 
-**New version : v0.1.1rc1**
+**New version : v0.1.2**
 
-Added :
+- Fixed manifest issue for PyPi
+
+Previous additions :
 
 - Improved training interface
 - Unsupervised model : WNet
   - Generate labels directly from raw data !
   - Can be trained in napari directly or in Colab
   - Pretrained weights for mesoSPIM whole-brain cell segmentation
 - WandB support (install wandb and login to use automatically when training)
@@ -102,31 +104,15 @@
 
 ## Demo
 
 ![demo](https://images.squarespace-cdn.com/content/v1/57f6d51c9f74566f55ecf271/0d16a71b-3ff2-477a-9d83-18d96cb1ce28/full_demo.gif?format=500w)
 
 ## Installation
 
-**Note** : we recommend using conda to create a new environment for the plugin.
-**M1 Mac users, please see the [M1 install section](#m1-mac-users)**
-
-    conda create --name napari-cellseg3d python=3.8
-    conda activate napari-cellseg3d
-
-You can install `napari-cellseg3d` via [pip]:
-
-    pip install napari-cellseg3d[all]
-
-OR directly via [napari-hub]:
-
-- Install napari from pip with `pip install "napari[all]"`,
-then from the “Plugins” menu within the napari application, select “Install/Uninstall Package(s)...”
-- Copy `napari-cellseg3d` and paste it where it says “Install by name/url…”
-- Click “Install”
-- Restart napari
+See the [Installation page] in the documentation for detailed instructions.
 
 ### M1 Mac users
 
 To avoid issues when installing on the ARM64 architecture, please follow these steps.
 
 1) Create a new conda env using the provided conda/napari_cellseg3d_m1.yml file :
 
@@ -177,14 +163,18 @@
 
 ## Issues
 
 If you encounter any problems, please [file an issue] along with a detailed description.
 
 ## Testing
 
+Before testing, install all requirements using ``pip install napari-cellseg3d[test]``.
+
+``pydensecrf`` is also required for testing.
+
 To run tests locally:
 
 - Locally : run ``pytest`` in the plugin folder
 - Locally with coverage : In the plugin folder, run ``coverage run --source=napari_cellseg3d -m pytest`` then ``coverage xml`` to generate a .xml coverage file.
 - With tox : run ``tox`` in the plugin folder (will simulate tests with several python and OS configs, requires substantial storage space)
 
 ## Contributing
@@ -212,15 +202,15 @@
 [Cookiecutter]: https://github.com/audreyr/cookiecutter
 [@napari]: https://github.com/napari
 [MIT]: http://opensource.org/licenses/MIT
 [cookiecutter-napari-plugin]: https://github.com/napari/cookiecutter-napari-plugin
 [tox]: https://tox.readthedocs.io/en/latest/
 [pip]: https://pypi.org/project/pip/
 [PyPI]: https://pypi.org/
-
+[Installation page]: https://adaptivemotorcontrollab.github.io/CellSeg3d/source/guides/installation_guide.html
 [the PyTorch website for installation instructions]: https://pytorch.org/get-started/locally/
 [PyTorch]: https://pytorch.org/get-started/locally/
 [MONAI's optional dependencies]: https://docs.monai.io/en/stable/installation.html#installing-the-recommended-dependencies
 [MONAI]: https://docs.monai.io/en/stable/installation.html#installing-the-recommended-dependencies
 
 ## Acknowledgements
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: napari-cellseg3d Version: 0.1.1rc1 Summary: Plugin
-for cell segmentation in 3D Author-email: Cyril Achard
+Metadata-Version: 2.1 Name: napari_cellseg3d Version: 0.1.2 Summary: Plugin for
+cell segmentation in 3D Author-email: Cyril Achard
 epfl.ch>, Maxime Vidal
 epfl.ch>, Mackenzie Mathis
 post.harvard.edu> License: MIT Project-URL: Homepage, https://github.com/
 AdaptiveMotorControlLab/CellSeg3d Project-URL: Documentation, https://
 adaptivemotorcontrollab.github.io/cellseg3d-docs/res/welcome.html Project-URL:
 Issues, https://github.com/AdaptiveMotorControlLab/CellSeg3d/issues Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Science/
@@ -46,39 +46,32 @@
 AdaptiveMotorControlLab/CellSeg3d) [![napari hub](https://img.shields.io/
 endpoint?url=https://api.napari-hub.org/shields/napari-cellseg3d)](https://
 www.napari-hub.org/plugins/napari-cellseg3d) A napari plugin for 3D cell
 segmentation: training, inference, and data review. In particular, this project
 was developed for analysis of mesoSPIM-acquired (cleared tissue + lightsheet)
 datasets. **Help us make the code better by reporting issues and adding your
 feature requests!** ---------------------------------- ## News **New version :
-v0.1.1rc1** Added : - Improved training interface - Unsupervised model : WNet -
-Generate labels directly from raw data ! - Can be trained in napari directly or
-in Colab - Pretrained weights for mesoSPIM whole-brain cell segmentation -
-WandB support (install wandb and login to use automatically when training) -
-Remade and improved documentation - Moved to Jupyter Book - Dedicated
-installation page, and working ARM64 install for macOS Silicon users - New
-utilities - Many small improvements and many bug fixes ## Demo ![demo](https://
-images.squarespace-cdn.com/content/v1/57f6d51c9f74566f55ecf271/0d16a71b-3ff2-
-477a-9d83-18d96cb1ce28/full_demo.gif?format=500w) ## Installation **Note** : we
-recommend using conda to create a new environment for the plugin. **M1 Mac
-users, please see the [M1 install section](#m1-mac-users)** conda create --name
-napari-cellseg3d python=3.8 conda activate napari-cellseg3d You can install
-`napari-cellseg3d` via [pip]: pip install napari-cellseg3d[all] OR directly via
-[napari-hub]: - Install napari from pip with `pip install "napari[all]"`, then
-from the âPluginsâ menu within the napari application, select âInstall/
-Uninstall Package(s)...â - Copy `napari-cellseg3d` and paste it where it says
-âInstall by name/urlâ¦â - Click âInstallâ - Restart napari ### M1 Mac
-users To avoid issues when installing on the ARM64 architecture, please follow
-these steps. 1) Create a new conda env using the provided conda/
-napari_cellseg3d_m1.yml file : git clone https://github.com/
-AdaptiveMotorControlLab/CellSeg3d.git cd CellSeg3d conda env create -f conda/
-napari_cellseg3d_m1.yml conda activate napari_cellseg3d_m1 2) Install the
-plugin. From repository root folder, run : pip install -e . OR directly via
-PyPi : pip install napari-cellseg3d OR directly via [napari-hub] (see
-Installation section above) ## Documentation Available at https://
+v0.1.2** - Fixed manifest issue for PyPi Previous additions : - Improved
+training interface - Unsupervised model : WNet - Generate labels directly from
+raw data ! - Can be trained in napari directly or in Colab - Pretrained weights
+for mesoSPIM whole-brain cell segmentation - WandB support (install wandb and
+login to use automatically when training) - Remade and improved documentation -
+Moved to Jupyter Book - Dedicated installation page, and working ARM64 install
+for macOS Silicon users - New utilities - Many small improvements and many bug
+fixes ## Demo ![demo](https://images.squarespace-cdn.com/content/v1/
+57f6d51c9f74566f55ecf271/0d16a71b-3ff2-477a-9d83-18d96cb1ce28/
+full_demo.gif?format=500w) ## Installation See the [Installation page] in the
+documentation for detailed instructions. ### M1 Mac users To avoid issues when
+installing on the ARM64 architecture, please follow these steps. 1) Create a
+new conda env using the provided conda/napari_cellseg3d_m1.yml file : git clone
+https://github.com/AdaptiveMotorControlLab/CellSeg3d.git cd CellSeg3d conda env
+create -f conda/napari_cellseg3d_m1.yml conda activate napari_cellseg3d_m1 2)
+Install the plugin. From repository root folder, run : pip install -e . OR
+directly via PyPi : pip install napari-cellseg3d OR directly via [napari-hub]
+(see Installation section above) ## Documentation Available at https://
 AdaptiveMotorControlLab.github.io/CellSeg3d You can also generate docs by
 running ``make html`` in the docs/ folder. ## Usage To use the plugin, please
 run: ``` napari ``` Then go into Plugins > napari-cellseg3d, and choose which
 tool to use. - **Review**: This module allows you to review your labels, from
 predictions or manual labeling, and correct them if needed. It then saves the
 status of each file in a csv, for easier monitoring. - **Inference**: This
 module allows you to use pre-trained segmentation algorithms on volumes to
@@ -91,35 +84,38 @@
 opposite. ## Requirements **Python 3.8 or 3.9 required.** Requires **
 [napari]**, **[PyTorch]** and **[MONAI]**. For PyTorch, please see [the PyTorch
 website for installation instructions]. A CUDA-capable GPU is not needed but
 very strongly recommended, especially for training. If you get errors from
 MONAI regarding missing readers, please see [MONAI's optional dependencies]
 page for instructions on getting the readers required by your images. ## Issues
 If you encounter any problems, please [file an issue] along with a detailed
-description. ## Testing To run tests locally: - Locally : run ``pytest`` in the
-plugin folder - Locally with coverage : In the plugin folder, run ``coverage
-run --source=napari_cellseg3d -m pytest`` then ``coverage xml`` to generate a
-.xml coverage file. - With tox : run ``tox`` in the plugin folder (will
-simulate tests with several python and OS configs, requires substantial storage
-space) ## Contributing Contributions are very welcome. Please ensure the
-coverage at least stays the same before you submit a pull request. For local
-installation from Github cloning, please run: ``` pip install -e . ``` ##
-License Distributed under the terms of the [MIT] license. "napari-cellseg3d" is
-free and open source software. [napari-hub]: https://www.napari-hub.org/
-plugins/napari-cellseg3d [file an issue]: https://github.com/
-AdaptiveMotorControlLab/CellSeg3d/issues [napari]: https://github.com/napari/
-napari [Cookiecutter]: https://github.com/audreyr/cookiecutter [@napari]:
-https://github.com/napari [MIT]: http://opensource.org/licenses/MIT
-[cookiecutter-napari-plugin]: https://github.com/napari/cookiecutter-napari-
-plugin [tox]: https://tox.readthedocs.io/en/latest/ [pip]: https://pypi.org/
-project/pip/ [PyPI]: https://pypi.org/ [the PyTorch website for installation
-instructions]: https://pytorch.org/get-started/locally/ [PyTorch]: https://
-pytorch.org/get-started/locally/ [MONAI's optional dependencies]: https://
-docs.monai.io/en/stable/installation.html#installing-the-recommended-
-dependencies [MONAI]: https://docs.monai.io/en/stable/
-installation.html#installing-the-recommended-dependencies ## Acknowledgements
-This plugin was developed by Cyril Achard, Maxime Vidal, Mackenzie Mathis. This
-work was funded, in part, from the Wyss Center to the [Mathis Laboratory of
-Adaptive Motor Control](https://www.mackenziemathislab.org/). Please refer to
-the documentation for full acknowledgements. ## Plugin base This [napari]
-plugin was generated with [Cookiecutter] using [@napari]'s [cookiecutter-
-napari-plugin] template.
+description. ## Testing Before testing, install all requirements using ``pip
+install napari-cellseg3d[test]``. ``pydensecrf`` is also required for testing.
+To run tests locally: - Locally : run ``pytest`` in the plugin folder - Locally
+with coverage : In the plugin folder, run ``coverage run --
+source=napari_cellseg3d -m pytest`` then ``coverage xml`` to generate a .xml
+coverage file. - With tox : run ``tox`` in the plugin folder (will simulate
+tests with several python and OS configs, requires substantial storage space)
+## Contributing Contributions are very welcome. Please ensure the coverage at
+least stays the same before you submit a pull request. For local installation
+from Github cloning, please run: ``` pip install -e . ``` ## License
+Distributed under the terms of the [MIT] license. "napari-cellseg3d" is free
+and open source software. [napari-hub]: https://www.napari-hub.org/plugins/
+napari-cellseg3d [file an issue]: https://github.com/AdaptiveMotorControlLab/
+CellSeg3d/issues [napari]: https://github.com/napari/napari [Cookiecutter]:
+https://github.com/audreyr/cookiecutter [@napari]: https://github.com/napari
+[MIT]: http://opensource.org/licenses/MIT [cookiecutter-napari-plugin]: https:/
+/github.com/napari/cookiecutter-napari-plugin [tox]: https://
+tox.readthedocs.io/en/latest/ [pip]: https://pypi.org/project/pip/ [PyPI]:
+https://pypi.org/ [Installation page]: https://
+adaptivemotorcontrollab.github.io/CellSeg3d/source/guides/
+installation_guide.html [the PyTorch website for installation instructions]:
+https://pytorch.org/get-started/locally/ [PyTorch]: https://pytorch.org/get-
+started/locally/ [MONAI's optional dependencies]: https://docs.monai.io/en/
+stable/installation.html#installing-the-recommended-dependencies [MONAI]:
+https://docs.monai.io/en/stable/installation.html#installing-the-recommended-
+dependencies ## Acknowledgements This plugin was developed by Cyril Achard,
+Maxime Vidal, Mackenzie Mathis. This work was funded, in part, from the Wyss
+Center to the [Mathis Laboratory of Adaptive Motor Control](https://
+www.mackenziemathislab.org/). Please refer to the documentation for full
+acknowledgements. ## Plugin base This [napari] plugin was generated with
+[Cookiecutter] using [@napari]'s [cookiecutter-napari-plugin] template.
```

### Comparing `napari_cellseg3d-0.1.1rc1/napari_cellseg3d.egg-info/SOURCES.txt` & `napari_cellseg3d-0.1.2/napari_cellseg3d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.1rc1/pyproject.toml` & `napari_cellseg3d-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `napari_cellseg3d-0.1.1rc1/setup.cfg` & `napari_cellseg3d-0.1.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = napari_cellseg3d
-version = 0.1.1rc1
+version = 0.1.2
 
 [options]
 packages = find:
 include_package_data = True
 python_requires = >=3.8
 package_dir = 
 	=.
```

