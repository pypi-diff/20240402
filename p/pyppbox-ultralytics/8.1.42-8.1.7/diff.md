# Comparing `tmp/pyppbox-ultralytics-8.1.42.tar.gz` & `tmp/pyppbox-ultralytics-8.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyppbox-ultralytics-8.1.42.tar", last modified: Tue Apr  2 18:15:28 2024, max compression
+gzip compressed data, was "pyppbox-ultralytics-8.1.7.tar", last modified: Mon Jan 29 11:25:20 2024, max compression
```

## Comparing `pyppbox-ultralytics-8.1.42.tar` & `pyppbox-ultralytics-8.1.7.tar`

### file list

```diff
@@ -1,258 +1,243 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:28.855491 pyppbox-ultralytics-8.1.42/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-04-02 18:15:28.855491 pyppbox-ultralytics-8.1.42/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:28.855491 pyppbox-ultralytics-8.1.42/pyppbox_ultralytics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-04-02 18:15:28.000000 pyppbox-ultralytics-8.1.42/pyppbox_ultralytics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7714 2024-04-02 18:15:28.000000 pyppbox-ultralytics-8.1.42/pyppbox_ultralytics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 18:15:28.000000 pyppbox-ultralytics-8.1.42/pyppbox_ultralytics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-02 18:15:28.000000 pyppbox-ultralytics-8.1.42/pyppbox_ultralytics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-02 18:15:28.000000 pyppbox-ultralytics-8.1.42/pyppbox_ultralytics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-02 18:15:28.000000 pyppbox-ultralytics-8.1.42/pyppbox_ultralytics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-02 18:15:28.855491 pyppbox-ultralytics-8.1.42/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:28.819491 pyppbox-ultralytics-8.1.42/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4711 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/tests/test_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)    23055 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/tests/test_python.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:28.819491 pyppbox-ultralytics-8.1.42/ultralytics/
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:28.819491 pyppbox-ultralytics-8.1.42/ultralytics/assets/
--rw-r--r--   0 runner    (1001) docker     (127)   137419 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/assets/bus.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    50427 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/assets/zidane.jpg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:28.819491 pyppbox-ultralytics-8.1.42/ultralytics/cfg/
--rw-r--r--   0 runner    (1001) docker     (127)    21316 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/cfg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:28.823491 pyppbox-ultralytics-8.1.42/ultralytics/cfg/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/cfg/datasets/Argoverse.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/cfg/datasets/DOTAv1.5.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/cfg/datasets/DOTAv1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/cfg/datasets/GlobalWheat2020.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    42507 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/cfg/datasets/ImageNet.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     9324 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/cfg/datasets/Objects365.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/cfg/datasets/SKU-110K.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/cfg/datasets/VOC.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/cfg/datasets/VisDrone.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/cfg/datasets/african-wildlife.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/cfg/datasets/brain-tumor.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/cfg/datasets/carparts-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/cfg/datasets/coco-pose.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/cfg/datasets/coco.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/cfg/datasets/coco128-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/cfg/datasets/coco128.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/cfg/datasets/coco8-pose.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/cfg/datasets/coco8-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/cfg/datasets/coco8.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/cfg/datasets/crack-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/cfg/datasets/dota8.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    29705 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/cfg/datasets/lvis.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    12493 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/cfg/datasets/open-images-v7.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/cfg/datasets/package-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/cfg/datasets/tiger-pose.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/cfg/datasets/xView.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8213 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/cfg/default.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:28.815491 pyppbox-ultralytics-8.1.42/ultralytics/cfg/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:28.823491 pyppbox-ultralytics-8.1.42/ultralytics/cfg/models/rt-detr/
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/cfg/models/rt-detr/rtdetr-l.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/cfg/models/rt-detr/rtdetr-resnet101.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/cfg/models/rt-detr/rtdetr-resnet50.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/cfg/models/rt-detr/rtdetr-x.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:28.827491 pyppbox-ultralytics-8.1.42/ultralytics/cfg/models/v3/
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/cfg/models/v3/yolov3-spp.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/cfg/models/v3/yolov3-tiny.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/cfg/models/v3/yolov3.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:28.827491 pyppbox-ultralytics-8.1.42/ultralytics/cfg/models/v5/
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/cfg/models/v5/yolov5-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/cfg/models/v5/yolov5.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:28.827491 pyppbox-ultralytics-8.1.42/ultralytics/cfg/models/v6/
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/cfg/models/v6/yolov6.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:28.827491 pyppbox-ultralytics-8.1.42/ultralytics/cfg/models/v8/
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/cfg/models/v8/yolov8-cls-resnet101.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/cfg/models/v8/yolov8-cls-resnet50.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/cfg/models/v8/yolov8-cls.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/cfg/models/v8/yolov8-ghost-p2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/cfg/models/v8/yolov8-ghost-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/cfg/models/v8/yolov8-ghost.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/cfg/models/v8/yolov8-obb.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/cfg/models/v8/yolov8-p2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/cfg/models/v8/yolov8-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/cfg/models/v8/yolov8-pose-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/cfg/models/v8/yolov8-pose.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/cfg/models/v8/yolov8-rtdetr.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/cfg/models/v8/yolov8-seg-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/cfg/models/v8/yolov8-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/cfg/models/v8/yolov8-world.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/cfg/models/v8/yolov8-worldv2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/cfg/models/v8/yolov8.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:28.827491 pyppbox-ultralytics-8.1.42/ultralytics/cfg/models/v9/
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/cfg/models/v9/yolov9c-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/cfg/models/v9/yolov9c.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/cfg/models/v9/yolov9e-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/cfg/models/v9/yolov9e.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:28.831491 pyppbox-ultralytics-8.1.42/ultralytics/cfg/trackers/
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/cfg/trackers/botsort.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/cfg/trackers/bytetrack.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:28.831491 pyppbox-ultralytics-8.1.42/ultralytics/data/
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/data/annotator.py
--rw-r--r--   0 runner    (1001) docker     (127)    57388 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/data/augment.py
--rw-r--r--   0 runner    (1001) docker     (127)    13470 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/data/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7265 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/data/build.py
--rw-r--r--   0 runner    (1001) docker     (127)    17527 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/data/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    22011 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/data/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:28.831491 pyppbox-ultralytics-8.1.42/ultralytics/data/explorer/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/data/explorer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18782 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/data/explorer/explorer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:28.831491 pyppbox-ultralytics-8.1.42/ultralytics/data/explorer/gui/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/data/explorer/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10044 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/data/explorer/gui/dash.py
--rw-r--r--   0 runner    (1001) docker     (127)     7041 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/data/explorer/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    23146 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/data/loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)    10010 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/data/split_dota.py
--rw-r--r--   0 runner    (1001) docker     (127)    30869 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:28.835492 pyppbox-ultralytics-8.1.42/ultralytics/engine/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    53790 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/engine/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)    39829 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/engine/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    17022 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/engine/predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)    30667 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/engine/results.py
--rw-r--r--   0 runner    (1001) docker     (127)    34919 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/engine/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11829 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/engine/tuner.py
--rw-r--r--   0 runner    (1001) docker     (127)    14645 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/engine/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:28.835492 pyppbox-ultralytics-8.1.42/ultralytics/hub/
--rw-r--r--   0 runner    (1001) docker     (127)     5068 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/hub/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    14649 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/hub/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     9729 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/hub/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:28.835492 pyppbox-ultralytics-8.1.42/ultralytics/models/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:28.835492 pyppbox-ultralytics-8.1.42/ultralytics/models/fastsam/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/models/fastsam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/models/fastsam/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/models/fastsam/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)    16132 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/models/fastsam/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/models/fastsam/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/models/fastsam/val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:28.835492 pyppbox-ultralytics-8.1.42/ultralytics/models/nas/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/models/nas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/models/nas/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/models/nas/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/models/nas/val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:28.835492 pyppbox-ultralytics-8.1.42/ultralytics/models/rtdetr/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/models/rtdetr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/models/rtdetr/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/models/rtdetr/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/models/rtdetr/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     5555 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/models/rtdetr/val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:28.839491 pyppbox-ultralytics-8.1.42/ultralytics/models/sam/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/models/sam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/models/sam/amg.py
--rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/models/sam/build.py
--rw-r--r--   0 runner    (1001) docker     (127)     4706 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/models/sam/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:28.839491 pyppbox-ultralytics-8.1.42/ultralytics/models/sam/modules/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/models/sam/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7816 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/models/sam/modules/decoders.py
--rw-r--r--   0 runner    (1001) docker     (127)    24746 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/models/sam/modules/encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/models/sam/modules/sam.py
--rw-r--r--   0 runner    (1001) docker     (127)    29135 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/models/sam/modules/tiny_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    11170 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/models/sam/modules/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    23632 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/models/sam/predict.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:28.839491 pyppbox-ultralytics-8.1.42/ultralytics/models/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/models/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15134 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/models/utils/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    13244 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/models/utils/ops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:28.839491 pyppbox-ultralytics-8.1.42/ultralytics/models/yolo/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/models/yolo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:28.839491 pyppbox-ultralytics-8.1.42/ultralytics/models/yolo/classify/
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/models/yolo/classify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/models/yolo/classify/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     6838 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/models/yolo/classify/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     4861 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/models/yolo/classify/val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:28.839491 pyppbox-ultralytics-8.1.42/ultralytics/models/yolo/detect/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/models/yolo/detect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/models/yolo/detect/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     6353 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/models/yolo/detect/train.py
--rw-r--r--   0 runner    (1001) docker     (127)    14416 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/models/yolo/detect/val.py
--rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/models/yolo/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:28.839491 pyppbox-ultralytics-8.1.42/ultralytics/models/yolo/obb/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/models/yolo/obb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/models/yolo/obb/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/models/yolo/obb/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/models/yolo/obb/val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:28.843491 pyppbox-ultralytics-8.1.42/ultralytics/models/yolo/pose/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/models/yolo/pose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/models/yolo/pose/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/models/yolo/pose/train.py
--rw-r--r--   0 runner    (1001) docker     (127)    10607 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/models/yolo/pose/val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:28.843491 pyppbox-ultralytics-8.1.42/ultralytics/models/yolo/segment/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/models/yolo/segment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/models/yolo/segment/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/models/yolo/segment/train.py
--rw-r--r--   0 runner    (1001) docker     (127)    11745 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/models/yolo/segment/val.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:28.843491 pyppbox-ultralytics-8.1.42/ultralytics/models/yolo/world/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/models/yolo/world/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/models/yolo/world/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/models/yolo/world/train_world.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:28.843491 pyppbox-ultralytics-8.1.42/ultralytics/nn/
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28718 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/nn/autobackend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:28.843491 pyppbox-ultralytics-8.1.42/ultralytics/nn/modules/
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/nn/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25251 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/nn/modules/block.py
--rw-r--r--   0 runner    (1001) docker     (127)    12722 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/nn/modules/conv.py
--rw-r--r--   0 runner    (1001) docker     (127)    22337 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/nn/modules/head.py
--rw-r--r--   0 runner    (1001) docker     (127)    17909 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/nn/modules/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/nn/modules/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    43623 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/nn/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:28.847492 pyppbox-ultralytics-8.1.42/ultralytics/solutions/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/solutions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/solutions/ai_gym.py
--rw-r--r--   0 runner    (1001) docker     (127)     6334 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/solutions/distance_calculation.py
--rw-r--r--   0 runner    (1001) docker     (127)    12902 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/solutions/heatmap.py
--rw-r--r--   0 runner    (1001) docker     (127)    12058 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/solutions/object_counter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/solutions/queue_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/solutions/speed_estimation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:28.847492 pyppbox-ultralytics-8.1.42/ultralytics/trackers/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/trackers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/trackers/basetrack.py
--rw-r--r--   0 runner    (1001) docker     (127)     8601 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/trackers/bot_sort.py
--rw-r--r--   0 runner    (1001) docker     (127)    18871 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/trackers/byte_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/trackers/track.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:28.847492 pyppbox-ultralytics-8.1.42/ultralytics/trackers/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/trackers/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13688 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/trackers/utils/gmc.py
--rw-r--r--   0 runner    (1001) docker     (127)    15168 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/trackers/utils/kalman_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/trackers/utils/matching.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:28.851492 pyppbox-ultralytics-8.1.42/ultralytics/utils/
--rw-r--r--   0 runner    (1001) docker     (127)    37845 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/utils/autobatch.py
--rw-r--r--   0 runner    (1001) docker     (127)    18285 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/utils/benchmarks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:28.855491 pyppbox-ultralytics-8.1.42/ultralytics/utils/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/utils/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5777 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/utils/callbacks/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/utils/callbacks/clearml.py
--rw-r--r--   0 runner    (1001) docker     (127)    13744 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/utils/callbacks/comet.py
--rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/utils/callbacks/dvc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/utils/callbacks/hub.py
--rw-r--r--   0 runner    (1001) docker     (127)     5333 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/utils/callbacks/mlflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/utils/callbacks/neptune.py
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/utils/callbacks/raytune.py
--rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/utils/callbacks/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     6635 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/utils/callbacks/wb.py
--rw-r--r--   0 runner    (1001) docker     (127)    28329 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/utils/dist.py
--rw-r--r--   0 runner    (1001) docker     (127)    21496 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/utils/downloads.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     6761 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (127)    15575 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/utils/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)    32716 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/utils/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    53473 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    33264 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/utils/ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/utils/patches.py
--rw-r--r--   0 runner    (1001) docker     (127)    46391 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/utils/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)    16017 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/utils/tal.py
--rw-r--r--   0 runner    (1001) docker     (127)    25825 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/utils/torch_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/utils/triton.py
--rw-r--r--   0 runner    (1001) docker     (127)     6171 2024-04-02 18:15:19.000000 pyppbox-ultralytics-8.1.42/ultralytics/utils/tuner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 11:25:20.734565 pyppbox-ultralytics-8.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-01-29 11:25:20.734565 pyppbox-ultralytics-8.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 11:25:20.734565 pyppbox-ultralytics-8.1.7/pyppbox_ultralytics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-01-29 11:25:20.000000 pyppbox-ultralytics-8.1.7/pyppbox_ultralytics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7168 2024-01-29 11:25:20.000000 pyppbox-ultralytics-8.1.7/pyppbox_ultralytics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-29 11:25:20.000000 pyppbox-ultralytics-8.1.7/pyppbox_ultralytics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-01-29 11:25:20.000000 pyppbox-ultralytics-8.1.7/pyppbox_ultralytics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-01-29 11:25:20.000000 pyppbox-ultralytics-8.1.7/pyppbox_ultralytics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-01-29 11:25:20.000000 pyppbox-ultralytics-8.1.7/pyppbox_ultralytics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-01-29 11:25:20.734565 pyppbox-ultralytics-8.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 11:25:20.698565 pyppbox-ultralytics-8.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5102 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/tests/test_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20266 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/tests/test_python.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 11:25:20.698565 pyppbox-ultralytics-8.1.7/ultralytics/
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 11:25:20.698565 pyppbox-ultralytics-8.1.7/ultralytics/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)   137419 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/assets/bus.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    50427 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/assets/zidane.jpg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 11:25:20.698565 pyppbox-ultralytics-8.1.7/ultralytics/cfg/
+-rw-r--r--   0 runner    (1001) docker     (127)    20768 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/cfg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 11:25:20.702565 pyppbox-ultralytics-8.1.7/ultralytics/cfg/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/cfg/datasets/Argoverse.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/cfg/datasets/DOTAv1.5.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/cfg/datasets/DOTAv1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/cfg/datasets/GlobalWheat2020.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    42507 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/cfg/datasets/ImageNet.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9324 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/cfg/datasets/Objects365.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/cfg/datasets/SKU-110K.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/cfg/datasets/VOC.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/cfg/datasets/VisDrone.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/cfg/datasets/carparts-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/cfg/datasets/coco-pose.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/cfg/datasets/coco.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/cfg/datasets/coco128-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/cfg/datasets/coco128.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/cfg/datasets/coco8-pose.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/cfg/datasets/coco8-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/cfg/datasets/coco8.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/cfg/datasets/crack-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/cfg/datasets/dota8.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    12493 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/cfg/datasets/open-images-v7.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/cfg/datasets/package-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/cfg/datasets/tiger-pose.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/cfg/datasets/xView.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8091 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/cfg/default.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 11:25:20.694564 pyppbox-ultralytics-8.1.7/ultralytics/cfg/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 11:25:20.706565 pyppbox-ultralytics-8.1.7/ultralytics/cfg/models/rt-detr/
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/cfg/models/rt-detr/rtdetr-l.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/cfg/models/rt-detr/rtdetr-resnet101.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/cfg/models/rt-detr/rtdetr-resnet50.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/cfg/models/rt-detr/rtdetr-x.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 11:25:20.706565 pyppbox-ultralytics-8.1.7/ultralytics/cfg/models/v3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/cfg/models/v3/yolov3-spp.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/cfg/models/v3/yolov3-tiny.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/cfg/models/v3/yolov3.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 11:25:20.706565 pyppbox-ultralytics-8.1.7/ultralytics/cfg/models/v5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/cfg/models/v5/yolov5-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/cfg/models/v5/yolov5.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 11:25:20.706565 pyppbox-ultralytics-8.1.7/ultralytics/cfg/models/v6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/cfg/models/v6/yolov6.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 11:25:20.710565 pyppbox-ultralytics-8.1.7/ultralytics/cfg/models/v8/
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/cfg/models/v8/yolov8-cls-resnet101.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/cfg/models/v8/yolov8-cls-resnet50.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/cfg/models/v8/yolov8-cls.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/cfg/models/v8/yolov8-ghost-p2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/cfg/models/v8/yolov8-ghost-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/cfg/models/v8/yolov8-ghost.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/cfg/models/v8/yolov8-obb.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/cfg/models/v8/yolov8-p2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/cfg/models/v8/yolov8-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/cfg/models/v8/yolov8-pose-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/cfg/models/v8/yolov8-pose.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/cfg/models/v8/yolov8-rtdetr.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/cfg/models/v8/yolov8-seg-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/cfg/models/v8/yolov8-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/cfg/models/v8/yolov8.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 11:25:20.710565 pyppbox-ultralytics-8.1.7/ultralytics/cfg/trackers/
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/cfg/trackers/botsort.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/cfg/trackers/bytetrack.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 11:25:20.710565 pyppbox-ultralytics-8.1.7/ultralytics/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/data/annotator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52000 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/data/augment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13216 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/data/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/data/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16496 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/data/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16526 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/data/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 11:25:20.710565 pyppbox-ultralytics-8.1.7/ultralytics/data/explorer/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/data/explorer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18688 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/data/explorer/explorer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 11:25:20.710565 pyppbox-ultralytics-8.1.7/ultralytics/data/explorer/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/data/explorer/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10042 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/data/explorer/gui/dash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7041 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/data/explorer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21910 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/data/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9961 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/data/split_dota.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29509 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 11:25:20.714565 pyppbox-ultralytics-8.1.7/ultralytics/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52004 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/engine/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21505 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/engine/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17832 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/engine/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27622 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/engine/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34307 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/engine/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11758 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/engine/tuner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14576 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/engine/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 11:25:20.714565 pyppbox-ultralytics-8.1.7/ultralytics/hub/
+-rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5370 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/hub/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14226 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/hub/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9736 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/hub/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 11:25:20.714565 pyppbox-ultralytics-8.1.7/ultralytics/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 11:25:20.714565 pyppbox-ultralytics-8.1.7/ultralytics/models/fastsam/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/models/fastsam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/models/fastsam/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/models/fastsam/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16190 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/models/fastsam/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/models/fastsam/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/models/fastsam/val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 11:25:20.718565 pyppbox-ultralytics-8.1.7/ultralytics/models/nas/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/models/nas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/models/nas/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/models/nas/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/models/nas/val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 11:25:20.718565 pyppbox-ultralytics-8.1.7/ultralytics/models/rtdetr/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/models/rtdetr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/models/rtdetr/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/models/rtdetr/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/models/rtdetr/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5401 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/models/rtdetr/val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 11:25:20.718565 pyppbox-ultralytics-8.1.7/ultralytics/models/sam/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/models/sam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/models/sam/amg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/models/sam/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4706 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/models/sam/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 11:25:20.718565 pyppbox-ultralytics-8.1.7/ultralytics/models/sam/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/models/sam/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7815 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/models/sam/modules/decoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24746 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/models/sam/modules/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/models/sam/modules/sam.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29136 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/models/sam/modules/tiny_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11170 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/models/sam/modules/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23632 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/models/sam/predict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 11:25:20.718565 pyppbox-ultralytics-8.1.7/ultralytics/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/models/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15134 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/models/utils/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13244 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/models/utils/ops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 11:25:20.722565 pyppbox-ultralytics-8.1.7/ultralytics/models/yolo/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/models/yolo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 11:25:20.722565 pyppbox-ultralytics-8.1.7/ultralytics/models/yolo/classify/
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/models/yolo/classify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/models/yolo/classify/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6832 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/models/yolo/classify/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4861 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/models/yolo/classify/val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 11:25:20.722565 pyppbox-ultralytics-8.1.7/ultralytics/models/yolo/detect/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/models/yolo/detect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/models/yolo/detect/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6306 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/models/yolo/detect/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13591 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/models/yolo/detect/val.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/models/yolo/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 11:25:20.722565 pyppbox-ultralytics-8.1.7/ultralytics/models/yolo/obb/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/models/yolo/obb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/models/yolo/obb/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/models/yolo/obb/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8409 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/models/yolo/obb/val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 11:25:20.722565 pyppbox-ultralytics-8.1.7/ultralytics/models/yolo/pose/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/models/yolo/pose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/models/yolo/pose/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/models/yolo/pose/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10607 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/models/yolo/pose/val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 11:25:20.722565 pyppbox-ultralytics-8.1.7/ultralytics/models/yolo/segment/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/models/yolo/segment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/models/yolo/segment/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/models/yolo/segment/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11745 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/models/yolo/segment/val.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 11:25:20.726565 pyppbox-ultralytics-8.1.7/ultralytics/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27071 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/nn/autobackend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 11:25:20.726565 pyppbox-ultralytics-8.1.7/ultralytics/nn/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/nn/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14488 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/nn/modules/block.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12722 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/nn/modules/conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19534 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/nn/modules/head.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17910 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/nn/modules/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/nn/modules/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38370 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/nn/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 11:25:20.726565 pyppbox-ultralytics-8.1.7/ultralytics/solutions/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/solutions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6006 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/solutions/ai_gym.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/solutions/distance_calculation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10838 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/solutions/heatmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10470 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/solutions/object_counter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6610 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/solutions/speed_estimation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 11:25:20.726565 pyppbox-ultralytics-8.1.7/ultralytics/trackers/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/trackers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/trackers/basetrack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8601 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/trackers/bot_sort.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18871 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/trackers/byte_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/trackers/track.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 11:25:20.730565 pyppbox-ultralytics-8.1.7/ultralytics/trackers/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/trackers/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13949 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/trackers/utils/gmc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15168 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/trackers/utils/kalman_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/trackers/utils/matching.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 11:25:20.730565 pyppbox-ultralytics-8.1.7/ultralytics/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)    36884 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/utils/autobatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17556 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/utils/benchmarks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 11:25:20.734565 pyppbox-ultralytics-8.1.7/ultralytics/utils/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/utils/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5777 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/utils/callbacks/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/utils/callbacks/clearml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13744 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/utils/callbacks/comet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/utils/callbacks/dvc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/utils/callbacks/hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4848 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/utils/callbacks/mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/utils/callbacks/neptune.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/utils/callbacks/raytune.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/utils/callbacks/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6650 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/utils/callbacks/wb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27964 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/utils/dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21189 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/utils/downloads.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15575 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/utils/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32581 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/utils/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53361 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32936 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/utils/ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/utils/patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44447 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/utils/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16015 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/utils/tal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25141 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/utils/torch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/utils/triton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-01-29 11:25:09.000000 pyppbox-ultralytics-8.1.7/ultralytics/utils/tuner.py
```

### Comparing `pyppbox-ultralytics-8.1.42/LICENSE` & `pyppbox-ultralytics-8.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/PKG-INFO` & `pyppbox-ultralytics-8.1.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyppbox-ultralytics
-Version: 8.1.42
+Version: 8.1.7
 Summary: Ultralytics YOLOv8 for SOTA object detection, multi-object tracking, instance segmentation, pose estimation and image classification.
 Home-page: https://github.com/rathaumons/ultralytics-for-pyppbox
 License: AGPL-3.0
 Project-URL: Bug Reports, https://github.com/rathaumons/ultralytics-for-pyppbox/issues
 Project-URL: Funding, https://ultralytics.com
 Project-URL: Source, https://github.com/rathaumons/ultralytics-for-pyppbox
 Keywords: machine-learning,deep-learning,vision,ML,DL,AI,YOLO,YOLOv3,YOLOv5,YOLOv8,HUB,Ultralytics
@@ -14,55 +14,60 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib>=3.3.0
-Requires-Dist: numpy>=1.22.2
 Requires-Dist: Pillow>=7.1.2
 Requires-Dist: PyYAML>=5.3.1
 Requires-Dist: requests>=2.23.0
 Requires-Dist: scipy>=1.4.1
 Requires-Dist: tqdm>=4.64.0
-Requires-Dist: hub-sdk>=0.0.5
+Requires-Dist: hub-sdk>=0.0.2
 Requires-Dist: pandas>=1.1.4
 Requires-Dist: seaborn>=0.11.0
 Requires-Dist: psutil
 Requires-Dist: py-cpuinfo
 Requires-Dist: thop>=0.1.1
+Provides-Extra: dev
+Requires-Dist: ipython; extra == "dev"
+Requires-Dist: check-manifest; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: coverage; extra == "dev"
+Requires-Dist: mkdocs-material; extra == "dev"
+Requires-Dist: mkdocstrings[python]; extra == "dev"
+Requires-Dist: mkdocs-redirects; extra == "dev"
+Requires-Dist: mkdocs-ultralytics-plugin>=0.0.42; extra == "dev"
 Provides-Extra: export
-Requires-Dist: onnx>=1.12.0; extra == "export"
 Requires-Dist: coremltools>=7.0; extra == "export"
-Requires-Dist: openvino>=2024.0.0; extra == "export"
-Provides-Extra: explorer
-Requires-Dist: lancedb; extra == "explorer"
-Requires-Dist: duckdb<=0.9.2; extra == "explorer"
-Requires-Dist: streamlit; extra == "explorer"
+Requires-Dist: openvino-dev>=2023.0; extra == "export"
+Requires-Dist: tensorflowjs; extra == "export"
 
-[![Test Build](https://github.com/rathaumons/ultralytics-for-pyppbox/actions/workflows/test_build.yaml/badge.svg)](https://github.com/rathaumons/ultralytics-for-pyppbox/actions/workflows/test_build.yaml) [![Build PyPI](https://github.com/rathaumons/ultralytics-for-pyppbox/actions/workflows/autobuild.yaml/badge.svg)](https://github.com/rathaumons/ultralytics-for-pyppbox/actions/workflows/autobuild.yaml)
+[![Build PyPI](https://github.com/rathaumons/ultralytics-for-pyppbox/actions/workflows/autobuild.yaml/badge.svg)](https://github.com/rathaumons/ultralytics-for-pyppbox/actions/workflows/autobuild.yaml)
 
-# Customized Ultralytics for pyppbox
+# Customized Ultralytics for [`pyppbox`](https://github.com/rathaumons/pyppbox)
 
-* Updated: **April 2, 2024**
-* Synced with: v8.1.42 -> [[3208eb7]](https://github.com/ultralytics/ultralytics/commit/3208eb72ef277b0b825306a84df6c460a8406647)
+* Updated: **January 29, 2024**
+* Synced with: v8.1.7 -> [[18d7ab0]](https://github.com/ultralytics/ultralytics/commit/18d7ab06ddcacdbde48900f5740d65223eafbf49)
 * All credit and info -> [[Original Ultralytics repo]](https://github.com/ultralytics/ultralytics)
-* Customized for [`pyppbox`](https://github.com/rathaumons/pyppbox):
+* What customized:
     - Enable OpenCV multithreading
     - Remove restrictions on customized OpenCV
     - Disable dependency auto-install
     - Disable auto update
 
 ## Installation
 
@@ -71,21 +76,17 @@
     pip install pyppbox-ultralytics
     ``` 
 * Or install from GitHub directly:
     ```
     pip install git+https://github.com/rathaumons/ultralytics-for-pyppbox.git
     ```
 * Or build from source:
-
-    <details><summary><ins>Click here to expand!</ins></summary>
-    
     ```
     git clone https://github.com/rathaumons/ultralytics-for-pyppbox.git
     cd ultralytics-for-pyppbox
     python -m pip install --upgrade pip
     pip install "setuptools>=67.2.0"
+    pip install -r requirements.txt
     pip install wheel build
     python -m build --wheel --skip-dependency-check --no-isolatio
     cd dist
     ```
-    
-    </details>
```

### Comparing `pyppbox-ultralytics-8.1.42/README.md` & `pyppbox-ultralytics-8.1.7/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-[![Test Build](https://github.com/rathaumons/ultralytics-for-pyppbox/actions/workflows/test_build.yaml/badge.svg)](https://github.com/rathaumons/ultralytics-for-pyppbox/actions/workflows/test_build.yaml) [![Build PyPI](https://github.com/rathaumons/ultralytics-for-pyppbox/actions/workflows/autobuild.yaml/badge.svg)](https://github.com/rathaumons/ultralytics-for-pyppbox/actions/workflows/autobuild.yaml)
+[![Build PyPI](https://github.com/rathaumons/ultralytics-for-pyppbox/actions/workflows/autobuild.yaml/badge.svg)](https://github.com/rathaumons/ultralytics-for-pyppbox/actions/workflows/autobuild.yaml)
 
-# Customized Ultralytics for pyppbox
+# Customized Ultralytics for [`pyppbox`](https://github.com/rathaumons/pyppbox)
 
-* Updated: **April 2, 2024**
-* Synced with: v8.1.42 -> [[3208eb7]](https://github.com/ultralytics/ultralytics/commit/3208eb72ef277b0b825306a84df6c460a8406647)
+* Updated: **January 29, 2024**
+* Synced with: v8.1.7 -> [[18d7ab0]](https://github.com/ultralytics/ultralytics/commit/18d7ab06ddcacdbde48900f5740d65223eafbf49)
 * All credit and info -> [[Original Ultralytics repo]](https://github.com/ultralytics/ultralytics)
-* Customized for [`pyppbox`](https://github.com/rathaumons/pyppbox):
+* What customized:
     - Enable OpenCV multithreading
     - Remove restrictions on customized OpenCV
     - Disable dependency auto-install
     - Disable auto update
 
 ## Installation
 
@@ -18,21 +18,17 @@
     pip install pyppbox-ultralytics
     ``` 
 * Or install from GitHub directly:
     ```
     pip install git+https://github.com/rathaumons/ultralytics-for-pyppbox.git
     ```
 * Or build from source:
-
-    <details><summary><ins>Click here to expand!</ins></summary>
-    
     ```
     git clone https://github.com/rathaumons/ultralytics-for-pyppbox.git
     cd ultralytics-for-pyppbox
     python -m pip install --upgrade pip
     pip install "setuptools>=67.2.0"
+    pip install -r requirements.txt
     pip install wheel build
     python -m build --wheel --skip-dependency-check --no-isolatio
     cd dist
     ```
-    
-    </details>
```

### Comparing `pyppbox-ultralytics-8.1.42/pyppbox_ultralytics.egg-info/PKG-INFO` & `pyppbox-ultralytics-8.1.7/pyppbox_ultralytics.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyppbox-ultralytics
-Version: 8.1.42
+Version: 8.1.7
 Summary: Ultralytics YOLOv8 for SOTA object detection, multi-object tracking, instance segmentation, pose estimation and image classification.
 Home-page: https://github.com/rathaumons/ultralytics-for-pyppbox
 License: AGPL-3.0
 Project-URL: Bug Reports, https://github.com/rathaumons/ultralytics-for-pyppbox/issues
 Project-URL: Funding, https://ultralytics.com
 Project-URL: Source, https://github.com/rathaumons/ultralytics-for-pyppbox
 Keywords: machine-learning,deep-learning,vision,ML,DL,AI,YOLO,YOLOv3,YOLOv5,YOLOv8,HUB,Ultralytics
@@ -14,55 +14,60 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib>=3.3.0
-Requires-Dist: numpy>=1.22.2
 Requires-Dist: Pillow>=7.1.2
 Requires-Dist: PyYAML>=5.3.1
 Requires-Dist: requests>=2.23.0
 Requires-Dist: scipy>=1.4.1
 Requires-Dist: tqdm>=4.64.0
-Requires-Dist: hub-sdk>=0.0.5
+Requires-Dist: hub-sdk>=0.0.2
 Requires-Dist: pandas>=1.1.4
 Requires-Dist: seaborn>=0.11.0
 Requires-Dist: psutil
 Requires-Dist: py-cpuinfo
 Requires-Dist: thop>=0.1.1
+Provides-Extra: dev
+Requires-Dist: ipython; extra == "dev"
+Requires-Dist: check-manifest; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: coverage; extra == "dev"
+Requires-Dist: mkdocs-material; extra == "dev"
+Requires-Dist: mkdocstrings[python]; extra == "dev"
+Requires-Dist: mkdocs-redirects; extra == "dev"
+Requires-Dist: mkdocs-ultralytics-plugin>=0.0.42; extra == "dev"
 Provides-Extra: export
-Requires-Dist: onnx>=1.12.0; extra == "export"
 Requires-Dist: coremltools>=7.0; extra == "export"
-Requires-Dist: openvino>=2024.0.0; extra == "export"
-Provides-Extra: explorer
-Requires-Dist: lancedb; extra == "explorer"
-Requires-Dist: duckdb<=0.9.2; extra == "explorer"
-Requires-Dist: streamlit; extra == "explorer"
+Requires-Dist: openvino-dev>=2023.0; extra == "export"
+Requires-Dist: tensorflowjs; extra == "export"
 
-[![Test Build](https://github.com/rathaumons/ultralytics-for-pyppbox/actions/workflows/test_build.yaml/badge.svg)](https://github.com/rathaumons/ultralytics-for-pyppbox/actions/workflows/test_build.yaml) [![Build PyPI](https://github.com/rathaumons/ultralytics-for-pyppbox/actions/workflows/autobuild.yaml/badge.svg)](https://github.com/rathaumons/ultralytics-for-pyppbox/actions/workflows/autobuild.yaml)
+[![Build PyPI](https://github.com/rathaumons/ultralytics-for-pyppbox/actions/workflows/autobuild.yaml/badge.svg)](https://github.com/rathaumons/ultralytics-for-pyppbox/actions/workflows/autobuild.yaml)
 
-# Customized Ultralytics for pyppbox
+# Customized Ultralytics for [`pyppbox`](https://github.com/rathaumons/pyppbox)
 
-* Updated: **April 2, 2024**
-* Synced with: v8.1.42 -> [[3208eb7]](https://github.com/ultralytics/ultralytics/commit/3208eb72ef277b0b825306a84df6c460a8406647)
+* Updated: **January 29, 2024**
+* Synced with: v8.1.7 -> [[18d7ab0]](https://github.com/ultralytics/ultralytics/commit/18d7ab06ddcacdbde48900f5740d65223eafbf49)
 * All credit and info -> [[Original Ultralytics repo]](https://github.com/ultralytics/ultralytics)
-* Customized for [`pyppbox`](https://github.com/rathaumons/pyppbox):
+* What customized:
     - Enable OpenCV multithreading
     - Remove restrictions on customized OpenCV
     - Disable dependency auto-install
     - Disable auto update
 
 ## Installation
 
@@ -71,21 +76,17 @@
     pip install pyppbox-ultralytics
     ``` 
 * Or install from GitHub directly:
     ```
     pip install git+https://github.com/rathaumons/ultralytics-for-pyppbox.git
     ```
 * Or build from source:
-
-    <details><summary><ins>Click here to expand!</ins></summary>
-    
     ```
     git clone https://github.com/rathaumons/ultralytics-for-pyppbox.git
     cd ultralytics-for-pyppbox
     python -m pip install --upgrade pip
     pip install "setuptools>=67.2.0"
+    pip install -r requirements.txt
     pip install wheel build
     python -m build --wheel --skip-dependency-check --no-isolatio
     cd dist
     ```
-    
-    </details>
```

### Comparing `pyppbox-ultralytics-8.1.42/pyppbox_ultralytics.egg-info/SOURCES.txt` & `pyppbox-ultralytics-8.1.7/pyppbox_ultralytics.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -24,27 +24,24 @@
 ultralytics/cfg/datasets/DOTAv1.yaml
 ultralytics/cfg/datasets/GlobalWheat2020.yaml
 ultralytics/cfg/datasets/ImageNet.yaml
 ultralytics/cfg/datasets/Objects365.yaml
 ultralytics/cfg/datasets/SKU-110K.yaml
 ultralytics/cfg/datasets/VOC.yaml
 ultralytics/cfg/datasets/VisDrone.yaml
-ultralytics/cfg/datasets/african-wildlife.yaml
-ultralytics/cfg/datasets/brain-tumor.yaml
 ultralytics/cfg/datasets/carparts-seg.yaml
 ultralytics/cfg/datasets/coco-pose.yaml
 ultralytics/cfg/datasets/coco.yaml
 ultralytics/cfg/datasets/coco128-seg.yaml
 ultralytics/cfg/datasets/coco128.yaml
 ultralytics/cfg/datasets/coco8-pose.yaml
 ultralytics/cfg/datasets/coco8-seg.yaml
 ultralytics/cfg/datasets/coco8.yaml
 ultralytics/cfg/datasets/crack-seg.yaml
 ultralytics/cfg/datasets/dota8.yaml
-ultralytics/cfg/datasets/lvis.yaml
 ultralytics/cfg/datasets/open-images-v7.yaml
 ultralytics/cfg/datasets/package-seg.yaml
 ultralytics/cfg/datasets/tiger-pose.yaml
 ultralytics/cfg/datasets/xView.yaml
 ultralytics/cfg/models/rt-detr/rtdetr-l.yaml
 ultralytics/cfg/models/rt-detr/rtdetr-resnet101.yaml
 ultralytics/cfg/models/rt-detr/rtdetr-resnet50.yaml
@@ -65,21 +62,15 @@
 ultralytics/cfg/models/v8/yolov8-p2.yaml
 ultralytics/cfg/models/v8/yolov8-p6.yaml
 ultralytics/cfg/models/v8/yolov8-pose-p6.yaml
 ultralytics/cfg/models/v8/yolov8-pose.yaml
 ultralytics/cfg/models/v8/yolov8-rtdetr.yaml
 ultralytics/cfg/models/v8/yolov8-seg-p6.yaml
 ultralytics/cfg/models/v8/yolov8-seg.yaml
-ultralytics/cfg/models/v8/yolov8-world.yaml
-ultralytics/cfg/models/v8/yolov8-worldv2.yaml
 ultralytics/cfg/models/v8/yolov8.yaml
-ultralytics/cfg/models/v9/yolov9c-seg.yaml
-ultralytics/cfg/models/v9/yolov9c.yaml
-ultralytics/cfg/models/v9/yolov9e-seg.yaml
-ultralytics/cfg/models/v9/yolov9e.yaml
 ultralytics/cfg/trackers/botsort.yaml
 ultralytics/cfg/trackers/bytetrack.yaml
 ultralytics/data/__init__.py
 ultralytics/data/annotator.py
 ultralytics/data/augment.py
 ultralytics/data/base.py
 ultralytics/data/build.py
@@ -153,32 +144,28 @@
 ultralytics/models/yolo/pose/predict.py
 ultralytics/models/yolo/pose/train.py
 ultralytics/models/yolo/pose/val.py
 ultralytics/models/yolo/segment/__init__.py
 ultralytics/models/yolo/segment/predict.py
 ultralytics/models/yolo/segment/train.py
 ultralytics/models/yolo/segment/val.py
-ultralytics/models/yolo/world/__init__.py
-ultralytics/models/yolo/world/train.py
-ultralytics/models/yolo/world/train_world.py
 ultralytics/nn/__init__.py
 ultralytics/nn/autobackend.py
 ultralytics/nn/tasks.py
 ultralytics/nn/modules/__init__.py
 ultralytics/nn/modules/block.py
 ultralytics/nn/modules/conv.py
 ultralytics/nn/modules/head.py
 ultralytics/nn/modules/transformer.py
 ultralytics/nn/modules/utils.py
 ultralytics/solutions/__init__.py
 ultralytics/solutions/ai_gym.py
 ultralytics/solutions/distance_calculation.py
 ultralytics/solutions/heatmap.py
 ultralytics/solutions/object_counter.py
-ultralytics/solutions/queue_management.py
 ultralytics/solutions/speed_estimation.py
 ultralytics/trackers/__init__.py
 ultralytics/trackers/basetrack.py
 ultralytics/trackers/bot_sort.py
 ultralytics/trackers/byte_tracker.py
 ultralytics/trackers/track.py
 ultralytics/trackers/utils/__init__.py
```

### Comparing `pyppbox-ultralytics-8.1.42/pyppbox_ultralytics.egg-info/top_level.txt` & `pyppbox-ultralytics-8.1.7/pyppbox_ultralytics.egg-info/top_level.txt`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 ultralytics/cfg/datasets
 ultralytics/cfg/models
 ultralytics/cfg/models/rt-detr
 ultralytics/cfg/models/v3
 ultralytics/cfg/models/v5
 ultralytics/cfg/models/v6
 ultralytics/cfg/models/v8
-ultralytics/cfg/models/v9
 ultralytics/cfg/trackers
 ultralytics/data
 ultralytics/data/explorer
 ultralytics/data/explorer/gui
 ultralytics/data/scripts
 ultralytics/engine
 ultralytics/hub
@@ -25,15 +24,14 @@
 ultralytics/models/utils
 ultralytics/models/yolo
 ultralytics/models/yolo/classify
 ultralytics/models/yolo/detect
 ultralytics/models/yolo/obb
 ultralytics/models/yolo/pose
 ultralytics/models/yolo/segment
-ultralytics/models/yolo/world
 ultralytics/nn
 ultralytics/nn/modules
 ultralytics/solutions
 ultralytics/trackers
 ultralytics/trackers/utils
 ultralytics/utils
 ultralytics/utils/callbacks
```

### Comparing `pyppbox-ultralytics-8.1.42/setup.cfg` & `pyppbox-ultralytics-8.1.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/setup.py` & `pyppbox-ultralytics-8.1.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 
     Args:
         file_path (str | Path): Path to the requirements.txt file.
 
     Returns:
         (List[str]): List of parsed requirements.
     """
+
     requirements = []
     for line in Path(file_path).read_text().splitlines():
         line = line.strip()
         if line and not line.startswith('#'):
             requirements.append(line.split('#')[0].strip())  # ignore inline comments
 
     return requirements
@@ -58,37 +59,43 @@
     packages=['ultralytics'] + [str(x) for x in Path('ultralytics').rglob('*/') if x.is_dir() and '__' not in str(x)],
     package_data={
         '': ['*.yaml'],
         'ultralytics.assets': ['*.jpg']},
     include_package_data=True,
     install_requires=parse_requirements(PARENT / 'requirements.txt'),
     extras_require={
+        'dev': [
+            'ipython',
+            'check-manifest',
+            'pre-commit',
+            'pytest',
+            'pytest-cov',
+            'coverage',
+            'mkdocs-material',
+            'mkdocstrings[python]',
+            'mkdocs-redirects',  # for 301 redirects
+            'mkdocs-ultralytics-plugin>=0.0.42',  # for meta descriptions and images, dates and authors
+        ],
         'export': [
-            'onnx>=1.12.0', # ONNX export
             'coremltools>=7.0',
-            'openvino>=2024.0.0', # OpenVINO export
-        ],
-        'explorer': [
-            'lancedb', # vector search
-            'duckdb<=0.9.2', # SQL queries, duckdb==0.10.0 bug https://github.com/ultralytics/ultralytics/pull/8181
-            'streamlit', # visualizing with GUI
-        ]
+            'openvino-dev>=2023.0',
+            'tensorflowjs',  # automatically installs tensorflow
+        ], 
     },
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'Intended Audience :: Education',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
-        'Programming Language :: Python :: 3.12',
         'Topic :: Software Development',
         'Topic :: Scientific/Engineering',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
         'Topic :: Scientific/Engineering :: Image Recognition',
         'Operating System :: POSIX :: Linux',
         'Operating System :: MacOS',
         'Operating System :: Microsoft :: Windows', ],
```

### Comparing `pyppbox-ultralytics-8.1.42/tests/conftest.py` & `pyppbox-ultralytics-8.1.7/tests/conftest.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,48 @@
 # Ultralytics YOLO 🚀, AGPL-3.0 license
 
 import shutil
 from pathlib import Path
 
+import pytest
+
 TMP = Path(__file__).resolve().parent / "tmp"  # temp directory for test files
 
 
 def pytest_addoption(parser):
     """
     Add custom command-line options to pytest.
 
     Args:
         parser (pytest.config.Parser): The pytest parser object.
     """
     parser.addoption("--slow", action="store_true", default=False, help="Run slow tests")
 
 
+def pytest_configure(config):
+    """
+    Register custom markers to avoid pytest warnings.
+
+    Args:
+        config (pytest.config.Config): The pytest config object.
+    """
+    config.addinivalue_line("markers", "slow: mark test as slow to run")
+
+
+def pytest_runtest_setup(item):
+    """
+    Setup hook to skip tests marked as slow if the --slow option is not provided.
+
+    Args:
+        item (pytest.Item): The test item object.
+    """
+    if "slow" in item.keywords and not item.config.getoption("--slow"):
+        pytest.skip("skip slow tests unless --slow is set")
+
+
 def pytest_collection_modifyitems(config, items):
     """
     Modify the list of test items to remove tests marked as slow if the --slow option is not provided.
 
     Args:
         config (pytest.config.Config): The pytest config object.
         items (list): List of test items to be executed.
```

### Comparing `pyppbox-ultralytics-8.1.42/tests/test_cli.py` & `pyppbox-ultralytics-8.1.7/tests/test_cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # Ultralytics YOLO 🚀, AGPL-3.0 license
 
 import subprocess
 
 import pytest
 
-from ultralytics.utils import ASSETS, WEIGHTS_DIR, checks
+from ultralytics.utils import ASSETS, WEIGHTS_DIR
+from ultralytics.utils.checks import cuda_device_count, cuda_is_available
 
-CUDA_IS_AVAILABLE = checks.cuda_is_available()
-CUDA_DEVICE_COUNT = checks.cuda_device_count()
+CUDA_IS_AVAILABLE = cuda_is_available()
+CUDA_DEVICE_COUNT = cuda_device_count()
 TASK_ARGS = [
     ("detect", "yolov8n", "coco8.yaml"),
     ("segment", "yolov8n-seg", "coco8-seg.yaml"),
     ("classify", "yolov8n-cls", "imagenet10"),
     ("pose", "yolov8n-pose", "coco8-pose.yaml"),
     ("obb", "yolov8n-obb", "dota8.yaml"),
 ]  # (task, model, data)
@@ -61,19 +62,18 @@
     """Test exporting a YOLO model to different formats."""
     run(f"yolo export model={WEIGHTS_DIR / model}.pt format={format} imgsz=32")
 
 
 def test_rtdetr(task="detect", model="yolov8n-rtdetr.yaml", data="coco8.yaml"):
     """Test the RTDETR functionality with the Ultralytics framework."""
     # Warning: MUST use imgsz=640
-    run(f"yolo train {task} model={model} data={data} --imgsz= 160 epochs =1, cache = disk")  # add coma, spaces to args
-    run(f"yolo predict {task} model={model} source={ASSETS / 'bus.jpg'} imgsz=160 save save_crop save_txt")
+    run(f"yolo train {task} model={model} data={data} --imgsz= 640 epochs =1, cache = disk")  # add coma, spaces to args
+    run(f"yolo predict {task} model={model} source={ASSETS / 'bus.jpg'} imgsz=640 save save_crop save_txt")
 
 
-@pytest.mark.skipif(checks.IS_PYTHON_3_12, reason="MobileSAM with CLIP is not supported in Python 3.12")
 def test_fastsam(task="segment", model=WEIGHTS_DIR / "FastSAM-s.pt", data="coco8-seg.yaml"):
     """Test FastSAM segmentation functionality within Ultralytics."""
     source = ASSETS / "bus.jpg"
 
     run(f"yolo segment val {task} model={model} data={data} imgsz=32")
     run(f"yolo segment predict model={model} source={source} imgsz=32 save save_crop save_txt")
```

### Comparing `pyppbox-ultralytics-8.1.42/tests/test_engine.py` & `pyppbox-ultralytics-8.1.7/tests/test_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 # Ultralytics YOLO 🚀, AGPL-3.0 license
 
-import sys
-from unittest import mock
 from ultralytics import YOLO
 from ultralytics.cfg import get_cfg
 from ultralytics.engine.exporter import Exporter
 from ultralytics.models.yolo import classify, detect, segment
 from ultralytics.utils import ASSETS, DEFAULT_CFG, WEIGHTS_DIR
 
 CFG_DET = "yolov8n.yaml"
@@ -47,18 +45,16 @@
     assert test_func in val.callbacks["on_val_start"], "callback test failed"
     val(model=trainer.best)  # validate best.pt
 
     # Predictor
     pred = detect.DetectionPredictor(overrides={"imgsz": [64, 64]})
     pred.add_callback("on_predict_start", test_func)
     assert test_func in pred.callbacks["on_predict_start"], "callback test failed"
-    # Confirm there is no issue with sys.argv being empty.
-    with mock.patch.object(sys, 'argv', []):
-        result = pred(source=ASSETS, model=f"{MODEL}.pt")
-        assert len(result), "predictor test failed"
+    result = pred(source=ASSETS, model=f"{MODEL}.pt")
+    assert len(result), "predictor test failed"
 
     overrides["resume"] = trainer.last
     trainer = detect.DetectionTrainer(overrides=overrides)
     try:
         trainer.train()
     except Exception as e:
         print(f"Expected exception caught: {e}")
```

### Comparing `pyppbox-ultralytics-8.1.42/tests/test_python.py` & `pyppbox-ultralytics-8.1.7/tests/test_python.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from copy import copy
 from pathlib import Path
 
 import cv2
 import numpy as np
 import pytest
 import torch
-import yaml
 from PIL import Image
 from torchvision.transforms import ToTensor
 
 from ultralytics import RTDETR, YOLO
 from ultralytics.cfg import TASK2DATA
 from ultralytics.data.build import load_inference_source
 from ultralytics.utils import (
@@ -26,15 +25,15 @@
     WEIGHTS_DIR,
     WINDOWS,
     Retry,
     checks,
     is_dir_writeable,
 )
 from ultralytics.utils.downloads import download
-from ultralytics.utils.torch_utils import TORCH_1_9, TORCH_1_13
+from ultralytics.utils.torch_utils import TORCH_1_9
 
 MODEL = WEIGHTS_DIR / "path with spaces" / "yolov8n.pt"  # test spaces in path
 CFG = "yolov8n.yaml"
 SOURCE = ASSETS / "bus.jpg"
 TMP = (ROOT / "../tests/tmp").resolve()  # temp directory for test files
 IS_TMP_WRITEABLE = is_dir_writeable(TMP)
 
@@ -166,14 +165,16 @@
 @pytest.mark.skipif(not IS_TMP_WRITEABLE, reason="directory is not writeable")
 def test_track_stream():
     """
     Test streaming tracking (short 10 frame video) with non-default ByteTrack tracker.
 
     Note imgsz=160 required for tracking for higher confidence and better matches
     """
+    import yaml
+
     video_url = "https://ultralytics.com/assets/decelera_portrait_min.mov"
     model = YOLO(MODEL)
     model.track(video_url, imgsz=160, tracker="bytetrack.yaml")
     model.track(video_url, imgsz=160, tracker="botsort.yaml", save_frames=True)  # test frame saving also
 
     # Test Global Motion Compensation (GMC) methods
     for gmc in "orb", "sift", "ecc":
@@ -213,23 +214,20 @@
 
 def test_export_onnx():
     """Test exporting the YOLO model to ONNX format."""
     f = YOLO(MODEL).export(format="onnx", dynamic=True)
     YOLO(f)(SOURCE)  # exported model inference
 
 
-@pytest.mark.skipif(checks.IS_PYTHON_3_12, reason="OpenVINO not supported in Python 3.12")
-@pytest.mark.skipif(not TORCH_1_13, reason="OpenVINO requires torch>=1.13")
 def test_export_openvino():
     """Test exporting the YOLO model to OpenVINO format."""
     f = YOLO(MODEL).export(format="openvino")
     YOLO(f)(SOURCE)  # exported model inference
 
 
-@pytest.mark.skipif(checks.IS_PYTHON_3_12, reason="CoreML not supported in Python 3.12")
 def test_export_coreml():
     """Test exporting the YOLO model to CoreML format."""
     if not WINDOWS:  # RuntimeError: BlobWriter not loaded with coremltools 7.0 on windows
         if MACOS:
             f = YOLO(MODEL).export(format="coreml")
             YOLO(f)(SOURCE)  # model prediction only supported on macOS for nms=False models
         else:
@@ -297,15 +295,15 @@
 
 
 def test_predict_callback_and_setup():
     """Test callback functionality during YOLO prediction."""
 
     def on_predict_batch_end(predictor):
         """Callback function that handles operations at the end of a prediction batch."""
-        path, im0s, _ = predictor.batch
+        path, im0s, _, _ = predictor.batch
         im0s = im0s if isinstance(im0s, list) else [im0s]
         bs = [predictor.dataset.bs for _ in range(len(path))]
         predictor.results = zip(predictor.results, im0s, bs)  # results is List[batch_size]
 
     model = YOLO(MODEL)
     model.add_callback("on_predict_batch_end", on_predict_batch_end)
 
@@ -330,36 +328,14 @@
             r.save_crop(save_dir=TMP / "runs/tests/crops/")
             r.tojson(normalize=True)
             r.plot(pil=True)
             r.plot(conf=True, boxes=True)
             print(r, len(r), r.path)
 
 
-def test_labels_and_crops():
-    """Test output from prediction args for saving detection labels and crops."""
-    imgs = [SOURCE, ASSETS / "zidane.jpg"]
-    results = YOLO(WEIGHTS_DIR / "yolov8n.pt")(imgs, imgsz=160, save_txt=True, save_crop=True)
-    save_path = Path(results[0].save_dir)
-    for r in results:
-        im_name = Path(r.path).stem
-        cls_idxs = r.boxes.cls.int().tolist()
-        # Check label path
-        labels = save_path / f"labels/{im_name}.txt"
-        assert labels.exists()
-        # Check detections match label count
-        assert len(r.boxes.data) == len([l for l in labels.read_text().splitlines() if l])
-        # Check crops path and files
-        crop_dirs = [p for p in (save_path / "crops").iterdir()]
-        crop_files = [f for p in crop_dirs for f in p.glob("*")]
-        # Crop directories match detections
-        assert all([r.names.get(c) in {d.name for d in crop_dirs} for c in cls_idxs])
-        # Same number of crops as detections
-        assert len([f for f in crop_files if im_name in f.name]) == len(r.boxes.data)
-
-
 @pytest.mark.skipif(not ONLINE, reason="environment is offline")
 def test_data_utils():
     """Test utility functions in ultralytics/data/utils.py."""
     from ultralytics.data.utils import HUBDatasetStats, autosplit
     from ultralytics.utils.downloads import zip_directory
 
     # from ultralytics.utils.files import WorkingDirectory
@@ -459,15 +435,14 @@
     m = Conv(64, 64, k=1, s=2)
 
     profile(x, [m], n=3)
     get_flops_with_torch_profiler(m)
     time_sync()
 
 
-@pytest.mark.slow
 @pytest.mark.skipif(not ONLINE, reason="environment is offline")
 def test_utils_downloads():
     """Test file download utilities."""
     from ultralytics.utils.downloads import get_google_drive_file_info
 
     get_google_drive_file_info("https://drive.google.com/file/d/1cqT-cJgANNrhIHCrEufUYhQ4RqiWG_lJ/view?usp=drive_link")
 
@@ -573,29 +548,27 @@
     export_fmts_hub()
     logout()
     smart_request("GET", "https://github.com", progress=True)
 
 
 @pytest.fixture
 def image():
-    """Loads an image from a predefined source using OpenCV."""
     return cv2.imread(str(SOURCE))
 
 
 @pytest.mark.parametrize(
     "auto_augment, erasing, force_color_jitter",
     [
         (None, 0.0, False),
         ("randaugment", 0.5, True),
         ("augmix", 0.2, False),
         ("autoaugment", 0.0, True),
     ],
 )
 def test_classify_transforms_train(image, auto_augment, erasing, force_color_jitter):
-    """Tests classification transforms during training with various augmentation settings."""
     import torchvision.transforms as T
 
     from ultralytics.data.augment import classify_augmentations
 
     transform = classify_augmentations(
         size=224,
         mean=(0.5, 0.5, 0.5),
@@ -632,40 +605,7 @@
     """Test YOLO model embeddings."""
     model_detect = YOLO(MODEL)
     model_segment = YOLO(WEIGHTS_DIR / "yolov8n-seg.pt")
 
     for batch in [SOURCE], [SOURCE, SOURCE]:  # test batch size 1 and 2
         assert len(model_detect.embed(source=batch, imgsz=32)) == len(batch)
         assert len(model_segment.embed(source=batch, imgsz=32)) == len(batch)
-
-
-@pytest.mark.skipif(checks.IS_PYTHON_3_12, reason="YOLOWorld with CLIP is not supported in Python 3.12")
-def test_yolo_world():
-    model = YOLO("yolov8s-world.pt")  # no YOLOv8n-world model yet
-    model.set_classes(["tree", "window"])
-    model(ASSETS / "bus.jpg", conf=0.01)
-
-    # Training from yaml
-    model = YOLO("yolov8s-worldv2.yaml")  # no YOLOv8n-world model yet
-    model.train(data="coco8.yaml", epochs=2, imgsz=32, cache="disk", batch=-1, close_mosaic=1, name="yolo-world")
-
-    model = YOLO("yolov8s-worldv2.pt")  # no YOLOv8n-world model yet
-    # val
-    model.val(data="coco8.yaml", imgsz=32, save_txt=True, save_json=True)
-    # Training from pretrain
-    model.train(data="coco8.yaml", epochs=2, imgsz=32, cache="disk", batch=-1, close_mosaic=1, name="yolo-world")
-
-    # test WorWorldTrainerFromScratch
-    from ultralytics.models.yolo.world.train_world import WorldTrainerFromScratch
-
-    model = YOLO("yolov8s-worldv2.yaml")  # no YOLOv8n-world model yet
-    data = dict(train=dict(yolo_data=["coco8.yaml"]), val=dict(yolo_data=["coco8.yaml"]))
-    model.train(
-        data=data,
-        epochs=2,
-        imgsz=32,
-        cache="disk",
-        batch=-1,
-        close_mosaic=1,
-        name="yolo-world",
-        trainer=WorldTrainerFromScratch,
-    )
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/__init__.py` & `pyppbox-ultralytics-8.1.7/ultralytics/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 # Ultralytics YOLO 🚀, AGPL-3.0 license
 
-__version__ = "8.1.42"
+__version__ = "8.1.7"
 
 from ultralytics.data.explorer.explorer import Explorer
-from ultralytics.models import RTDETR, SAM, YOLO, YOLOWorld
+from ultralytics.models import RTDETR, SAM, YOLO
 from ultralytics.models.fastsam import FastSAM
 from ultralytics.models.nas import NAS
 from ultralytics.utils import ASSETS, SETTINGS as settings
 from ultralytics.utils.checks import check_yolo as checks
 from ultralytics.utils.downloads import download
 
 __all__ = (
     "__version__",
     "ASSETS",
     "YOLO",
-    "YOLOWorld",
     "NAS",
     "SAM",
     "FastSAM",
     "RTDETR",
     "checks",
     "download",
     "settings",
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/assets/bus.jpg` & `pyppbox-ultralytics-8.1.7/ultralytics/assets/bus.jpg`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/assets/zidane.jpg` & `pyppbox-ultralytics-8.1.7/ultralytics/assets/zidane.jpg`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/cfg/__init__.py` & `pyppbox-ultralytics-8.1.7/ultralytics/cfg/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,16 +26,16 @@
     colorstr,
     deprecation_warn,
     yaml_load,
     yaml_print,
 )
 
 # Define valid tasks and modes
-MODES = {"train", "val", "predict", "export", "track", "benchmark"}
-TASKS = {"detect", "segment", "classify", "pose", "obb"}
+MODES = "train", "val", "predict", "export", "track", "benchmark"
+TASKS = "detect", "segment", "classify", "pose", "obb"
 TASK2DATA = {
     "detect": "coco8.yaml",
     "segment": "coco8-seg.yaml",
     "classify": "imagenet10",
     "pose": "coco8-pose.yaml",
     "obb": "dota8.yaml",
 }
@@ -50,17 +50,16 @@
     "detect": "metrics/mAP50-95(B)",
     "segment": "metrics/mAP50-95(M)",
     "classify": "metrics/accuracy_top1",
     "pose": "metrics/mAP50-95(P)",
     "obb": "metrics/mAP50-95(B)",
 }
 
-ARGV = sys.argv or ["", ""]  # sometimes sys.argv = []
 CLI_HELP_MSG = f"""
-    Arguments received: {str(['yolo'] + ARGV[1:])}. Ultralytics 'yolo' commands use the following syntax:
+    Arguments received: {str(['yolo'] + sys.argv[1:])}. Ultralytics 'yolo' commands use the following syntax:
 
         yolo TASK MODE ARGS
 
         Where   TASK (optional) is one of {TASKS}
                 MODE (required) is one of {MODES}
                 ARGS (optional) are any number of custom 'arg=value' pairs like 'imgsz=320' that override defaults.
                     See all ARGS at https://docs.ultralytics.com/usage/cfg or with 'yolo cfg'
@@ -90,16 +89,16 @@
 
     Docs: https://docs.ultralytics.com
     Community: https://community.ultralytics.com
     GitHub: https://github.com/ultralytics/ultralytics
     """
 
 # Define keys for arg type checks
-CFG_FLOAT_KEYS = {"warmup_epochs", "box", "cls", "dfl", "degrees", "shear", "time", "workspace"}
-CFG_FRACTION_KEYS = {
+CFG_FLOAT_KEYS = "warmup_epochs", "box", "cls", "dfl", "degrees", "shear", "time"
+CFG_FRACTION_KEYS = (
     "dropout",
     "iou",
     "lr0",
     "lrf",
     "momentum",
     "weight_decay",
     "warmup_momentum",
@@ -109,37 +108,37 @@
     "hsv_s",
     "hsv_v",
     "translate",
     "scale",
     "perspective",
     "flipud",
     "fliplr",
-    "bgr",
     "mosaic",
     "mixup",
     "copy_paste",
     "conf",
     "iou",
     "fraction",
-}  # fraction floats 0.0 - 1.0
-CFG_INT_KEYS = {
+)  # fraction floats 0.0 - 1.0
+CFG_INT_KEYS = (
     "epochs",
     "patience",
     "batch",
     "workers",
     "seed",
     "close_mosaic",
     "mask_ratio",
     "max_det",
     "vid_stride",
     "line_width",
+    "workspace",
     "nbs",
     "save_period",
-}
-CFG_BOOL_KEYS = {
+)
+CFG_BOOL_KEYS = (
     "save",
     "exist_ok",
     "verbose",
     "deterministic",
     "single_cls",
     "rect",
     "cos_lr",
@@ -166,15 +165,15 @@
     "optimize",
     "int8",
     "dynamic",
     "simplify",
     "nms",
     "profile",
     "multi_scale",
-}
+)
 
 
 def cfg2dict(cfg):
     """
     Convert a configuration object to a dictionary, whether it is a file path, a string, or a SimpleNamespace object.
 
     Args:
@@ -216,67 +215,54 @@
         if k in cfg and isinstance(cfg[k], (int, float)):
             cfg[k] = str(cfg[k])
     if cfg.get("name") == "model":  # assign model to 'name' arg
         cfg["name"] = cfg.get("model", "").split(".")[0]
         LOGGER.warning(f"WARNING ⚠️ 'name=model' automatically updated to 'name={cfg['name']}'.")
 
     # Type and Value checks
-    check_cfg(cfg)
-
-    # Return instance
-    return IterableSimpleNamespace(**cfg)
-
-
-def check_cfg(cfg, hard=True):
-    """Check Ultralytics configuration argument types and values."""
     for k, v in cfg.items():
         if v is not None:  # None values may be from optional args
             if k in CFG_FLOAT_KEYS and not isinstance(v, (int, float)):
-                if hard:
+                raise TypeError(
+                    f"'{k}={v}' is of invalid type {type(v).__name__}. "
+                    f"Valid '{k}' types are int (i.e. '{k}=0') or float (i.e. '{k}=0.5')"
+                )
+            elif k in CFG_FRACTION_KEYS:
+                if not isinstance(v, (int, float)):
                     raise TypeError(
                         f"'{k}={v}' is of invalid type {type(v).__name__}. "
                         f"Valid '{k}' types are int (i.e. '{k}=0') or float (i.e. '{k}=0.5')"
                     )
-                cfg[k] = float(v)
-            elif k in CFG_FRACTION_KEYS:
-                if not isinstance(v, (int, float)):
-                    if hard:
-                        raise TypeError(
-                            f"'{k}={v}' is of invalid type {type(v).__name__}. "
-                            f"Valid '{k}' types are int (i.e. '{k}=0') or float (i.e. '{k}=0.5')"
-                        )
-                    cfg[k] = v = float(v)
                 if not (0.0 <= v <= 1.0):
                     raise ValueError(f"'{k}={v}' is an invalid value. " f"Valid '{k}' values are between 0.0 and 1.0.")
             elif k in CFG_INT_KEYS and not isinstance(v, int):
-                if hard:
-                    raise TypeError(
-                        f"'{k}={v}' is of invalid type {type(v).__name__}. " f"'{k}' must be an int (i.e. '{k}=8')"
-                    )
-                cfg[k] = int(v)
+                raise TypeError(
+                    f"'{k}={v}' is of invalid type {type(v).__name__}. " f"'{k}' must be an int (i.e. '{k}=8')"
+                )
             elif k in CFG_BOOL_KEYS and not isinstance(v, bool):
-                if hard:
-                    raise TypeError(
-                        f"'{k}={v}' is of invalid type {type(v).__name__}. "
-                        f"'{k}' must be a bool (i.e. '{k}=True' or '{k}=False')"
-                    )
-                cfg[k] = bool(v)
+                raise TypeError(
+                    f"'{k}={v}' is of invalid type {type(v).__name__}. "
+                    f"'{k}' must be a bool (i.e. '{k}=True' or '{k}=False')"
+                )
+
+    # Return instance
+    return IterableSimpleNamespace(**cfg)
 
 
 def get_save_dir(args, name=None):
     """Return save_dir as created from train/val/predict arguments."""
 
     if getattr(args, "save_dir", None):
         save_dir = args.save_dir
     else:
         from ultralytics.utils.files import increment_path
 
         project = args.project or (ROOT.parent / "tests/tmp/runs" if TESTS_RUNNING else RUNS_DIR) / args.task
         name = name or args.name or f"{args.mode}"
-        save_dir = increment_path(Path(project) / name, exist_ok=args.exist_ok if RANK in {-1, 0} else True)
+        save_dir = increment_path(Path(project) / name, exist_ok=args.exist_ok if RANK in (-1, 0) else True)
 
     return Path(save_dir)
 
 
 def _handle_deprecation(custom):
     """Hardcoded function to handle deprecated config keys."""
 
@@ -406,15 +392,15 @@
     except Exception as e:
         LOGGER.warning(f"WARNING ⚠️ settings error: '{e}'. Please see {url} for help.")
 
 
 def handle_explorer():
     """Open the Ultralytics Explorer GUI."""
     checks.check_requirements("streamlit")
-    LOGGER.info("💡 Loading Explorer dashboard...")
+    LOGGER.info(f"💡 Loading Explorer dashboard...")
     subprocess.run(["streamlit", "run", ROOT / "data/explorer/gui/dash.py", "--server.maxMessageSize", "2048"])
 
 
 def parse_key_value_pair(pair):
     """Parse one 'key=value' pair and return key and value."""
     k, v = pair.split("=", 1)  # split on first '=' sign
     k, v = k.strip(), v.strip()  # remove spaces
@@ -448,15 +434,15 @@
     - specifying the mode, either 'train', 'val', 'test', or 'predict'
     - running special modes like 'checks'
     - passing overrides to the package's configuration
 
     It uses the package's default cfg and initializes it using the passed overrides.
     Then it calls the CLI function with the composed cfg
     """
-    args = (debug.split(" ") if debug else ARGV)[1:]
+    args = (debug.split(" ") if debug else sys.argv)[1:]
     if not args:  # no arguments passed
         LOGGER.info(CLI_HELP_MSG)
         return
 
     special = {
         "help": lambda: LOGGER.info(CLI_HELP_MSG),
         "checks": checks.collect_system_info,
@@ -474,18 +460,18 @@
     special.update({k[0]: v for k, v in special.items()})  # singular
     special.update({k[:-1]: v for k, v in special.items() if len(k) > 1 and k.endswith("s")})  # singular
     special = {**special, **{f"-{k}": v for k, v in special.items()}, **{f"--{k}": v for k, v in special.items()}}
 
     overrides = {}  # basic overrides, i.e. imgsz=320
     for a in merge_equals_args(args):  # merge spaces around '=' sign
         if a.startswith("--"):
-            LOGGER.warning(f"WARNING ⚠️ argument '{a}' does not require leading dashes '--', updating to '{a[2:]}'.")
+            LOGGER.warning(f"WARNING ⚠️ '{a}' does not require leading dashes '--', updating to '{a[2:]}'.")
             a = a[2:]
         if a.endswith(","):
-            LOGGER.warning(f"WARNING ⚠️ argument '{a}' does not require trailing comma ',', updating to '{a[:-1]}'.")
+            LOGGER.warning(f"WARNING ⚠️ '{a}' does not require trailing comma ',', updating to '{a[:-1]}'.")
             a = a[:-1]
         if "=" in a:
             try:
                 k, v = parse_key_value_pair(a)
                 if k == "cfg" and v is not None:  # custom.yaml passed
                     LOGGER.info(f"Overriding {DEFAULT_CFG_PATH} with {v}")
                     overrides = {k: val for k, val in yaml_load(checks.check_yaml(v)).items() if k != "cfg"}
@@ -514,15 +500,15 @@
     # Check keys
     check_dict_alignment(full_args_dict, overrides)
 
     # Mode
     mode = overrides.get("mode")
     if mode is None:
         mode = DEFAULT_CFG.mode or "predict"
-        LOGGER.warning(f"WARNING ⚠️ 'mode' argument is missing. Valid modes are {MODES}. Using default 'mode={mode}'.")
+        LOGGER.warning(f"WARNING ⚠️ 'mode' is missing. Valid modes are {MODES}. Using default 'mode={mode}'.")
     elif mode not in MODES:
         raise ValueError(f"Invalid 'mode={mode}'. Valid modes are {MODES}.\n{CLI_HELP_MSG}")
 
     # Task
     task = overrides.pop("task", None)
     if task:
         if task not in TASKS:
@@ -530,15 +516,15 @@
         if "model" not in overrides:
             overrides["model"] = TASK2MODEL[task]
 
     # Model
     model = overrides.pop("model", DEFAULT_CFG.model)
     if model is None:
         model = "yolov8n.pt"
-        LOGGER.warning(f"WARNING ⚠️ 'model' argument is missing. Using default 'model={model}'.")
+        LOGGER.warning(f"WARNING ⚠️ 'model' is missing. Using default 'model={model}'.")
     overrides["model"] = model
     stem = Path(model).stem.lower()
     if "rtdetr" in stem:  # guess architecture
         from ultralytics import RTDETR
 
         model = RTDETR(model)  # no task argument
     elif "fastsam" in stem:
@@ -562,25 +548,25 @@
             LOGGER.warning(
                 f"WARNING ⚠️ conflicting 'task={task}' passed with 'task={model.task}' model. "
                 f"Ignoring 'task={task}' and updating to 'task={model.task}' to match model."
             )
         task = model.task
 
     # Mode
-    if mode in {"predict", "track"} and "source" not in overrides:
+    if mode in ("predict", "track") and "source" not in overrides:
         overrides["source"] = DEFAULT_CFG.source or ASSETS
-        LOGGER.warning(f"WARNING ⚠️ 'source' argument is missing. Using default 'source={overrides['source']}'.")
-    elif mode in {"train", "val"}:
+        LOGGER.warning(f"WARNING ⚠️ 'source' is missing. Using default 'source={overrides['source']}'.")
+    elif mode in ("train", "val"):
         if "data" not in overrides and "resume" not in overrides:
             overrides["data"] = DEFAULT_CFG.data or TASK2DATA.get(task or DEFAULT_CFG.task, DEFAULT_CFG.data)
-            LOGGER.warning(f"WARNING ⚠️ 'data' argument is missing. Using default 'data={overrides['data']}'.")
+            LOGGER.warning(f"WARNING ⚠️ 'data' is missing. Using default 'data={overrides['data']}'.")
     elif mode == "export":
         if "format" not in overrides:
             overrides["format"] = DEFAULT_CFG.format or "torchscript"
-            LOGGER.warning(f"WARNING ⚠️ 'format' argument is missing. Using default 'format={overrides['format']}'.")
+            LOGGER.warning(f"WARNING ⚠️ 'format' is missing. Using default 'format={overrides['format']}'.")
 
     # Run command in python
     getattr(model, mode)(**overrides)  # default args from model
 
     # Show help
     LOGGER.info(f"💡 Learn more at https://docs.ultralytics.com/modes/{mode}")
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/cfg/datasets/Argoverse.yaml` & `pyppbox-ultralytics-8.1.7/ultralytics/cfg/datasets/Argoverse.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/cfg/datasets/DOTAv1.5.yaml` & `pyppbox-ultralytics-8.1.7/ultralytics/cfg/datasets/DOTAv1.5.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/cfg/datasets/DOTAv1.yaml` & `pyppbox-ultralytics-8.1.7/ultralytics/cfg/datasets/DOTAv1.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/cfg/datasets/GlobalWheat2020.yaml` & `pyppbox-ultralytics-8.1.7/ultralytics/cfg/datasets/GlobalWheat2020.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/cfg/datasets/ImageNet.yaml` & `pyppbox-ultralytics-8.1.7/ultralytics/cfg/datasets/ImageNet.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/cfg/datasets/Objects365.yaml` & `pyppbox-ultralytics-8.1.7/ultralytics/cfg/datasets/Objects365.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/cfg/datasets/SKU-110K.yaml` & `pyppbox-ultralytics-8.1.7/ultralytics/cfg/datasets/SKU-110K.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/cfg/datasets/VOC.yaml` & `pyppbox-ultralytics-8.1.7/ultralytics/cfg/datasets/VOC.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/cfg/datasets/VisDrone.yaml` & `pyppbox-ultralytics-8.1.7/ultralytics/cfg/datasets/VisDrone.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/cfg/datasets/carparts-seg.yaml` & `pyppbox-ultralytics-8.1.7/ultralytics/cfg/datasets/carparts-seg.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/cfg/datasets/coco-pose.yaml` & `pyppbox-ultralytics-8.1.7/ultralytics/cfg/datasets/coco-pose.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/cfg/datasets/coco.yaml` & `pyppbox-ultralytics-8.1.7/ultralytics/cfg/datasets/coco.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/cfg/datasets/coco128-seg.yaml` & `pyppbox-ultralytics-8.1.7/ultralytics/cfg/datasets/coco128-seg.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/cfg/datasets/coco128.yaml` & `pyppbox-ultralytics-8.1.7/ultralytics/cfg/datasets/coco128.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/cfg/datasets/coco8-pose.yaml` & `pyppbox-ultralytics-8.1.7/ultralytics/cfg/datasets/coco8-pose.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/cfg/datasets/coco8-seg.yaml` & `pyppbox-ultralytics-8.1.7/ultralytics/cfg/datasets/coco8-seg.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/cfg/datasets/coco8.yaml` & `pyppbox-ultralytics-8.1.7/ultralytics/cfg/datasets/coco8.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/cfg/datasets/crack-seg.yaml` & `pyppbox-ultralytics-8.1.7/ultralytics/cfg/datasets/crack-seg.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/cfg/datasets/dota8.yaml` & `pyppbox-ultralytics-8.1.7/ultralytics/cfg/datasets/dota8.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/cfg/datasets/open-images-v7.yaml` & `pyppbox-ultralytics-8.1.7/ultralytics/cfg/datasets/open-images-v7.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/cfg/datasets/package-seg.yaml` & `pyppbox-ultralytics-8.1.7/ultralytics/cfg/datasets/package-seg.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/cfg/datasets/tiger-pose.yaml` & `pyppbox-ultralytics-8.1.7/ultralytics/cfg/datasets/tiger-pose.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/cfg/datasets/xView.yaml` & `pyppbox-ultralytics-8.1.7/ultralytics/cfg/datasets/xView.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/cfg/default.yaml` & `pyppbox-ultralytics-8.1.7/ultralytics/cfg/default.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 mode: train # (str) YOLO mode, i.e. train, val, predict, export, track, benchmark
 
 # Train settings -------------------------------------------------------------------------------------------------------
 model: # (str, optional) path to model file, i.e. yolov8n.pt, yolov8n.yaml
 data: # (str, optional) path to data file, i.e. coco128.yaml
 epochs: 100 # (int) number of epochs to train for
 time: # (float, optional) number of hours to train for, overrides epochs if supplied
-patience: 100 # (int) epochs to wait for no observable improvement for early stopping of training
+patience: 50 # (int) epochs to wait for no observable improvement for early stopping of training
 batch: 16 # (int) number of images per batch (-1 for AutoBatch)
 imgsz: 640 # (int | list) input images size as int for train and val modes, or list[w,h] for predict and export modes
 save: True # (bool) save train checkpoints and predict results
 save_period: -1 # (int) Save checkpoint every x epochs (disabled if < 1)
 cache: False # (bool) True/ram, disk or False. Use cache for data loading
 device: # (int | str | list, optional) device to run on, i.e. cuda device=0 or device=0,1,2,3 or device=cpu
 workers: 8 # (int) number of worker threads for data loading (per RANK if DDP)
@@ -30,15 +30,15 @@
 cos_lr: False # (bool) use cosine learning rate scheduler
 close_mosaic: 10 # (int) disable mosaic augmentation for final epochs (0 to disable)
 resume: False # (bool) resume training from last checkpoint
 amp: True # (bool) Automatic Mixed Precision (AMP) training, choices=[True, False], True runs AMP check
 fraction: 1.0 # (float) dataset fraction to train on (default is 1.0, all images in train set)
 profile: False # (bool) profile ONNX and TensorRT speeds during training for loggers
 freeze: None # (int | list, optional) freeze first n layers, or freeze list of layer indices during training
-multi_scale: False # (bool) Whether to use multiscale during training
+multi_scale: False # (bool) Whether to use multi-scale during training
 # Segmentation
 overlap_mask: True # (bool) masks should overlap during training (segment train only)
 mask_ratio: 4 # (int) mask downsample ratio (segment train only)
 # Classification
 dropout: 0.0 # (float) use dropout regularization (classify train only)
 
 # Val/Test settings ----------------------------------------------------------------------------------------------------
@@ -107,20 +107,19 @@
 degrees: 0.0 # (float) image rotation (+/- deg)
 translate: 0.1 # (float) image translation (+/- fraction)
 scale: 0.5 # (float) image scale (+/- gain)
 shear: 0.0 # (float) image shear (+/- deg)
 perspective: 0.0 # (float) image perspective (+/- fraction), range 0-0.001
 flipud: 0.0 # (float) image flip up-down (probability)
 fliplr: 0.5 # (float) image flip left-right (probability)
-bgr: 0.0 # (float) image channel BGR (probability)
 mosaic: 1.0 # (float) image mosaic (probability)
 mixup: 0.0 # (float) image mixup (probability)
 copy_paste: 0.0 # (float) segment copy-paste (probability)
 auto_augment: randaugment # (str) auto augmentation policy for classification (randaugment, autoaugment, augmix)
-erasing: 0.4 # (float) probability of random erasing during classification training (0-0.9), 0 means no erasing, must be less than 1.0.
-crop_fraction: 1.0 # (float) image crop fraction for classification (0.1-1), 1.0 means no crop, must be greater than 0.
+erasing: 0.4 # (float) probability of random erasing during classification training (0-1)
+crop_fraction: 1.0 # (float) image crop fraction for classification evaluation/inference (0-1)
 
 # Custom config.yaml ---------------------------------------------------------------------------------------------------
 cfg: # (str, optional) for overriding defaults.yaml
 
 # Tracker settings ------------------------------------------------------------------------------------------------------
 tracker: botsort.yaml # (str) tracker type, choices=[botsort.yaml, bytetrack.yaml]
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/cfg/models/rt-detr/rtdetr-l.yaml` & `pyppbox-ultralytics-8.1.7/ultralytics/cfg/models/rt-detr/rtdetr-l.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/cfg/models/rt-detr/rtdetr-resnet101.yaml` & `pyppbox-ultralytics-8.1.7/ultralytics/cfg/models/rt-detr/rtdetr-resnet101.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/cfg/models/rt-detr/rtdetr-resnet50.yaml` & `pyppbox-ultralytics-8.1.7/ultralytics/cfg/models/rt-detr/rtdetr-resnet50.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/cfg/models/rt-detr/rtdetr-x.yaml` & `pyppbox-ultralytics-8.1.7/ultralytics/cfg/models/rt-detr/rtdetr-x.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/cfg/models/v3/yolov3-spp.yaml` & `pyppbox-ultralytics-8.1.7/ultralytics/cfg/models/v3/yolov3-spp.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/cfg/models/v3/yolov3-tiny.yaml` & `pyppbox-ultralytics-8.1.7/ultralytics/cfg/models/v3/yolov3-tiny.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/cfg/models/v3/yolov3.yaml` & `pyppbox-ultralytics-8.1.7/ultralytics/cfg/models/v3/yolov3.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/cfg/models/v5/yolov5-p6.yaml` & `pyppbox-ultralytics-8.1.7/ultralytics/cfg/models/v5/yolov5-p6.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/cfg/models/v5/yolov5.yaml` & `pyppbox-ultralytics-8.1.7/ultralytics/cfg/models/v5/yolov5.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/cfg/models/v6/yolov6.yaml` & `pyppbox-ultralytics-8.1.7/ultralytics/cfg/models/v6/yolov6.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/cfg/models/v8/yolov8-cls-resnet101.yaml` & `pyppbox-ultralytics-8.1.7/ultralytics/cfg/models/v8/yolov8-cls-resnet101.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/cfg/models/v8/yolov8-cls-resnet50.yaml` & `pyppbox-ultralytics-8.1.7/ultralytics/cfg/models/v8/yolov8-cls-resnet50.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/cfg/models/v8/yolov8-cls.yaml` & `pyppbox-ultralytics-8.1.7/ultralytics/cfg/models/v8/yolov8-cls.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/cfg/models/v8/yolov8-ghost-p2.yaml` & `pyppbox-ultralytics-8.1.7/ultralytics/cfg/models/v8/yolov8-ghost-p2.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/cfg/models/v8/yolov8-ghost-p6.yaml` & `pyppbox-ultralytics-8.1.7/ultralytics/cfg/models/v8/yolov8-ghost-p6.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/cfg/models/v8/yolov8-ghost.yaml` & `pyppbox-ultralytics-8.1.7/ultralytics/cfg/models/v8/yolov8-ghost.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/cfg/models/v8/yolov8-obb.yaml` & `pyppbox-ultralytics-8.1.7/ultralytics/cfg/models/v8/yolov8-obb.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/cfg/models/v8/yolov8-p2.yaml` & `pyppbox-ultralytics-8.1.7/ultralytics/cfg/models/v8/yolov8-p2.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/cfg/models/v8/yolov8-p6.yaml` & `pyppbox-ultralytics-8.1.7/ultralytics/cfg/models/v8/yolov8-p6.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/cfg/models/v8/yolov8-pose-p6.yaml` & `pyppbox-ultralytics-8.1.7/ultralytics/cfg/models/v8/yolov8-pose-p6.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/cfg/models/v8/yolov8-pose.yaml` & `pyppbox-ultralytics-8.1.7/ultralytics/cfg/models/v8/yolov8-pose.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/cfg/models/v8/yolov8-rtdetr.yaml` & `pyppbox-ultralytics-8.1.7/ultralytics/cfg/models/v8/yolov8-rtdetr.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/cfg/models/v8/yolov8-seg-p6.yaml` & `pyppbox-ultralytics-8.1.7/ultralytics/cfg/models/v8/yolov8-seg-p6.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/cfg/models/v8/yolov8-seg.yaml` & `pyppbox-ultralytics-8.1.7/ultralytics/cfg/models/v8/yolov8-seg.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/cfg/models/v8/yolov8-world.yaml` & `pyppbox-ultralytics-8.1.7/ultralytics/cfg/models/v8/yolov8.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Ultralytics YOLO 🚀, AGPL-3.0 license
-# YOLOv8-World object detection model with P3-P5 outputs. For details see https://docs.ultralytics.com/tasks/detect
+# YOLOv8 object detection model with P3-P5 outputs. For Usage examples see https://docs.ultralytics.com/tasks/detect
 
 # Parameters
 nc: 80 # number of classes
 scales: # model compound scaling constants, i.e. 'model=yolov8n.yaml' will call yolov8.yaml with scale 'n'
   # [depth, width, max_channels]
   n: [0.33, 0.25, 1024] # YOLOv8n summary: 225 layers,  3157200 parameters,  3157184 gradients,   8.9 GFLOPs
   s: [0.33, 0.50, 1024] # YOLOv8s summary: 225 layers, 11166560 parameters, 11166544 gradients,  28.8 GFLOPs
@@ -25,24 +25,22 @@
   - [-1, 3, C2f, [1024, True]]
   - [-1, 1, SPPF, [1024, 5]] # 9
 
 # YOLOv8.0n head
 head:
   - [-1, 1, nn.Upsample, [None, 2, "nearest"]]
   - [[-1, 6], 1, Concat, [1]] # cat backbone P4
-  - [-1, 3, C2fAttn, [512, 256, 8]] # 12
+  - [-1, 3, C2f, [512]] # 12
 
   - [-1, 1, nn.Upsample, [None, 2, "nearest"]]
   - [[-1, 4], 1, Concat, [1]] # cat backbone P3
-  - [-1, 3, C2fAttn, [256, 128, 4]] # 15 (P3/8-small)
+  - [-1, 3, C2f, [256]] # 15 (P3/8-small)
 
-  - [[15, 12, 9], 1, ImagePoolingAttn, [256]] # 16 (P3/8-small)
-
-  - [15, 1, Conv, [256, 3, 2]]
+  - [-1, 1, Conv, [256, 3, 2]]
   - [[-1, 12], 1, Concat, [1]] # cat head P4
-  - [-1, 3, C2fAttn, [512, 256, 8]] # 19 (P4/16-medium)
+  - [-1, 3, C2f, [512]] # 18 (P4/16-medium)
 
   - [-1, 1, Conv, [512, 3, 2]]
   - [[-1, 9], 1, Concat, [1]] # cat head P5
-  - [-1, 3, C2fAttn, [1024, 512, 16]] # 22 (P5/32-large)
+  - [-1, 3, C2f, [1024]] # 21 (P5/32-large)
 
-  - [[15, 19, 22], 1, WorldDetect, [nc, 512, False]] # Detect(P3, P4, P5)
+  - [[15, 18, 21], 1, Detect, [nc]] # Detect(P3, P4, P5)
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/cfg/trackers/botsort.yaml` & `pyppbox-ultralytics-8.1.7/ultralytics/cfg/trackers/botsort.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/cfg/trackers/bytetrack.yaml` & `pyppbox-ultralytics-8.1.7/ultralytics/cfg/trackers/bytetrack.yaml`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/data/annotator.py` & `pyppbox-ultralytics-8.1.7/ultralytics/data/annotator.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/data/augment.py` & `pyppbox-ultralytics-8.1.7/ultralytics/data/augment.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # Ultralytics YOLO 🚀, AGPL-3.0 license
 
 import math
 import random
 from copy import deepcopy
-from typing import Tuple, Union
 
 import cv2
 import numpy as np
 import torch
 import torchvision.transforms as T
 
 from ultralytics.utils import LOGGER, colorstr
@@ -63,49 +62,26 @@
 
 
 class Compose:
     """Class for composing multiple image transformations."""
 
     def __init__(self, transforms):
         """Initializes the Compose object with a list of transforms."""
-        self.transforms = transforms if isinstance(transforms, list) else [transforms]
+        self.transforms = transforms
 
     def __call__(self, data):
         """Applies a series of transformations to input data."""
         for t in self.transforms:
             data = t(data)
         return data
 
     def append(self, transform):
         """Appends a new transform to the existing list of transforms."""
         self.transforms.append(transform)
 
-    def insert(self, index, transform):
-        """Inserts a new transform to the existing list of transforms."""
-        self.transforms.insert(index, transform)
-
-    def __getitem__(self, index: Union[list, int]) -> "Compose":
-        """Retrieve a specific transform or a set of transforms using indexing."""
-        assert isinstance(index, (int, list)), f"The indices should be either list or int type but got {type(index)}"
-        index = [index] if isinstance(index, int) else index
-        return Compose([self.transforms[i] for i in index])
-
-    def __setitem__(self, index: Union[list, int], value: Union[list, int]) -> None:
-        """Retrieve a specific transform or a set of transforms using indexing."""
-        assert isinstance(index, (int, list)), f"The indices should be either list or int type but got {type(index)}"
-        if isinstance(index, list):
-            assert isinstance(
-                value, list
-            ), f"The indices should be the same type as values, but got {type(index)} and {type(value)}"
-        if isinstance(index, int):
-            index, value = [index], [value]
-        for i, v in zip(index, value):
-            assert i < len(self.transforms), f"list index {i} out of range {len(self.transforms)}."
-            self.transforms[i] = v
-
     def tolist(self):
         """Converts the list of transforms to a standard Python list."""
         return self.transforms
 
     def __repr__(self):
         """Returns a string representation of the object."""
         return f"{self.__class__.__name__}({', '.join([f'{t}' for t in self.transforms])})"
@@ -138,45 +114,27 @@
         mix_labels = [self.dataset.get_image_and_label(i) for i in indexes]
 
         if self.pre_transform is not None:
             for i, data in enumerate(mix_labels):
                 mix_labels[i] = self.pre_transform(data)
         labels["mix_labels"] = mix_labels
 
-        # Update cls and texts
-        labels = self._update_label_text(labels)
         # Mosaic or MixUp
         labels = self._mix_transform(labels)
         labels.pop("mix_labels", None)
         return labels
 
     def _mix_transform(self, labels):
         """Applies MixUp or Mosaic augmentation to the label dictionary."""
         raise NotImplementedError
 
     def get_indexes(self):
         """Gets a list of shuffled indexes for mosaic augmentation."""
         raise NotImplementedError
 
-    def _update_label_text(self, labels):
-        """Update label text."""
-        if "texts" not in labels:
-            return labels
-
-        mix_texts = sum([labels["texts"]] + [x["texts"] for x in labels["mix_labels"]], [])
-        mix_texts = list({tuple(x) for x in mix_texts})
-        text2id = {text: i for i, text in enumerate(mix_texts)}
-
-        for label in [labels] + labels["mix_labels"]:
-            for i, l in enumerate(label["cls"].squeeze(-1).tolist()):
-                text = label["texts"][int(l)]
-                label["cls"][i] = text2id[tuple(text)]
-            label["texts"] = mix_texts
-        return labels
-
 
 class Mosaic(BaseMixTransform):
     """
     Mosaic augmentation.
 
     This class performs mosaic augmentation by combining multiple (4 or 9) images into a single mosaic image.
     The augmentation is applied to a dataset with a given probability.
@@ -187,15 +145,15 @@
         p (float, optional): Probability of applying the mosaic augmentation. Must be in the range 0-1. Default to 1.0.
         n (int, optional): The grid size, either 4 (for 2x2) or 9 (for 3x3).
     """
 
     def __init__(self, dataset, imgsz=640, p=1.0, n=4):
         """Initializes the object with a dataset, image size, probability, and border."""
         assert 0 <= p <= 1.0, f"The probability should be in range [0, 1], but got {p}."
-        assert n in {4, 9}, "grid must be equal to 4 or 9."
+        assert n in (4, 9), "grid must be equal to 4 or 9."
         super().__init__(dataset=dataset, p=p)
         self.dataset = dataset
         self.imgsz = imgsz
         self.border = (-imgsz // 2, -imgsz // 2)  # width, height
         self.n = n
 
     def get_indexes(self, buffer=True):
@@ -358,16 +316,14 @@
             "cls": np.concatenate(cls, 0),
             "instances": Instances.concatenate(instances, axis=0),
             "mosaic_border": self.border,
         }
         final_labels["instances"].clip(imgsz, imgsz)
         good = final_labels["instances"].remove_zero_area_boxes()
         final_labels["cls"] = final_labels["cls"][good]
-        if "texts" in mosaic_labels[0]:
-            final_labels["texts"] = mosaic_labels[0]["texts"]
         return final_labels
 
 
 class MixUp(BaseMixTransform):
     """Class for applying MixUp augmentation to the dataset."""
 
     def __init__(self, dataset, pre_transform=None, p=0.0) -> None:
@@ -681,15 +637,15 @@
 
         Args:
             p (float, optional): The probability of applying the flip. Must be between 0 and 1. Default is 0.5.
             direction (str, optional): The direction to apply the flip. Must be 'horizontal' or 'vertical'.
                 Default is 'horizontal'.
             flip_idx (array-like, optional): Index mapping for flipping keypoints, if any.
         """
-        assert direction in {"horizontal", "vertical"}, f"Support direction `horizontal` or `vertical`, got {direction}"
+        assert direction in ["horizontal", "vertical"], f"Support direction `horizontal` or `vertical`, got {direction}"
         assert 0 <= p <= 1.0
 
         self.p = p
         self.direction = direction
         self.flip_idx = flip_idx
 
     def __call__(self, labels):
@@ -926,39 +882,36 @@
         bbox_format (str): Format for bounding boxes. Default is 'xywh'.
         normalize (bool): Whether to normalize bounding boxes. Default is True.
         return_mask (bool): Return instance masks for segmentation. Default is False.
         return_keypoint (bool): Return keypoints for pose estimation. Default is False.
         mask_ratio (int): Downsample ratio for masks. Default is 4.
         mask_overlap (bool): Whether to overlap masks. Default is True.
         batch_idx (bool): Keep batch indexes. Default is True.
-        bgr (float): The probability to return BGR images. Default is 0.0.
     """
 
     def __init__(
         self,
         bbox_format="xywh",
         normalize=True,
         return_mask=False,
         return_keypoint=False,
         return_obb=False,
         mask_ratio=4,
         mask_overlap=True,
         batch_idx=True,
-        bgr=0.0,
     ):
         """Initializes the Format class with given parameters."""
         self.bbox_format = bbox_format
         self.normalize = normalize
         self.return_mask = return_mask  # set False when training detection only
         self.return_keypoint = return_keypoint
         self.return_obb = return_obb
         self.mask_ratio = mask_ratio
         self.mask_overlap = mask_overlap
         self.batch_idx = batch_idx  # keep the batch indexes
-        self.bgr = bgr
 
     def __call__(self, labels):
         """Return formatted image, classes, bounding boxes & keypoints to be used by 'collate_fn'."""
         img = labels.pop("img")
         h, w = img.shape[:2]
         cls = labels.pop("cls")
         instances = labels.pop("instances")
@@ -991,16 +944,15 @@
             labels["batch_idx"] = torch.zeros(nl)
         return labels
 
     def _format_img(self, img):
         """Format the image for YOLO from Numpy array to PyTorch tensor."""
         if len(img.shape) < 3:
             img = np.expand_dims(img, -1)
-        img = img.transpose(2, 0, 1)
-        img = np.ascontiguousarray(img[::-1] if random.uniform(0, 1) > self.bgr else img)
+        img = np.ascontiguousarray(img.transpose(2, 0, 1)[::-1])
         img = torch.from_numpy(img)
         return img
 
     def _format_segments(self, instances, cls, w, h):
         """Convert polygon points to bitmap."""
         segments = instances.segments
         if self.mask_overlap:
@@ -1010,91 +962,14 @@
             cls = cls[sorted_idx]
         else:
             masks = polygons2masks((h, w), segments, color=1, downsample_ratio=self.mask_ratio)
 
         return masks, instances, cls
 
 
-class RandomLoadText:
-    """
-    Randomly sample positive texts and negative texts and update the class indices accordingly to the number of samples.
-
-    Attributes:
-        prompt_format (str): Format for prompt. Default is '{}'.
-        neg_samples (tuple[int]): A ranger to randomly sample negative texts, Default is (80, 80).
-        max_samples (int): The max number of different text samples in one image, Default is 80.
-        padding (bool): Whether to pad texts to max_samples. Default is False.
-        padding_value (str): The padding text. Default is "".
-    """
-
-    def __init__(
-        self,
-        prompt_format: str = "{}",
-        neg_samples: Tuple[int, int] = (80, 80),
-        max_samples: int = 80,
-        padding: bool = False,
-        padding_value: str = "",
-    ) -> None:
-        """Initializes the RandomLoadText class with given parameters."""
-        self.prompt_format = prompt_format
-        self.neg_samples = neg_samples
-        self.max_samples = max_samples
-        self.padding = padding
-        self.padding_value = padding_value
-
-    def __call__(self, labels: dict) -> dict:
-        """Return updated classes and texts."""
-        assert "texts" in labels, "No texts found in labels."
-        class_texts = labels["texts"]
-        num_classes = len(class_texts)
-        cls = np.asarray(labels.pop("cls"), dtype=int)
-        pos_labels = np.unique(cls).tolist()
-
-        if len(pos_labels) > self.max_samples:
-            pos_labels = set(random.sample(pos_labels, k=self.max_samples))
-
-        neg_samples = min(min(num_classes, self.max_samples) - len(pos_labels), random.randint(*self.neg_samples))
-        neg_labels = []
-        for i in range(num_classes):
-            if i not in pos_labels:
-                neg_labels.append(i)
-        neg_labels = random.sample(neg_labels, k=neg_samples)
-
-        sampled_labels = pos_labels + neg_labels
-        random.shuffle(sampled_labels)
-
-        label2ids = {label: i for i, label in enumerate(sampled_labels)}
-        valid_idx = np.zeros(len(labels["instances"]), dtype=bool)
-        new_cls = []
-        for i, label in enumerate(cls.squeeze(-1).tolist()):
-            if label not in label2ids:
-                continue
-            valid_idx[i] = True
-            new_cls.append([label2ids[label]])
-        labels["instances"] = labels["instances"][valid_idx]
-        labels["cls"] = np.array(new_cls)
-
-        # Randomly select one prompt when there's more than one prompts
-        texts = []
-        for label in sampled_labels:
-            prompts = class_texts[label]
-            assert len(prompts) > 0
-            prompt = self.prompt_format.format(prompts[random.randrange(len(prompts))])
-            texts.append(prompt)
-
-        if self.padding:
-            valid_labels = len(pos_labels) + len(neg_labels)
-            num_padding = self.max_samples - valid_labels
-            if num_padding > 0:
-                texts += [self.padding_value] * num_padding
-
-        labels["texts"] = texts
-        return labels
-
-
 def v8_transforms(dataset, imgsz, hyp, stretch=False):
     """Convert images to a size suitable for YOLOv8 training."""
     pre_transform = Compose(
         [
             Mosaic(dataset, imgsz=imgsz, p=hyp.mosaic),
             CopyPaste(p=hyp.copy_paste),
             RandomPerspective(
@@ -1173,15 +1048,15 @@
             std=torch.tensor(std),
         ),
     ]
 
     return T.Compose(tfl)
 
 
-# Classification training augmentations --------------------------------------------------------------------------------
+# Classification augmentations train ---------------------------------------------------------------------------------------
 def classify_augmentations(
     size=224,
     mean=DEFAULT_MEAN,
     std=DEFAULT_STD,
     scale=None,
     ratio=None,
     hflip=0.5,
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/data/base.py` & `pyppbox-ultralytics-8.1.7/ultralytics/data/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 import cv2
 import numpy as np
 import psutil
 from torch.utils.data import Dataset
 
 from ultralytics.utils import DEFAULT_CFG, LOCAL_RANK, LOGGER, NUM_THREADS, TQDM
-from .utils import HELP_URL, FORMATS_HELP_MSG, IMG_FORMATS
+from .utils import HELP_URL, IMG_FORMATS
 
 
 class BaseDataset(Dataset):
     """
     Base dataset class for loading and processing image data.
 
     Args:
@@ -77,16 +77,14 @@
         self.rect = rect
         self.batch_size = batch_size
         self.stride = stride
         self.pad = pad
         if self.rect:
             assert self.batch_size is not None
             self.set_rectangle()
-        if isinstance(cache, str):
-            cache = cache.lower()
 
         # Buffer thread for mosaic images
         self.buffer = []  # buffer size = batch size
         self.max_buffer_length = min((self.ni, self.batch_size * 8, 1000)) if self.augment else 0
 
         # Cache images
         if cache == "ram" and not self.check_cache_ram():
@@ -114,21 +112,19 @@
                         parent = str(p.parent) + os.sep
                         f += [x.replace("./", parent) if x.startswith("./") else x for x in t]  # local to global path
                         # F += [p.parent / x.lstrip(os.sep) for x in t]  # local to global path (pathlib)
                 else:
                     raise FileNotFoundError(f"{self.prefix}{p} does not exist")
             im_files = sorted(x.replace("/", os.sep) for x in f if x.split(".")[-1].lower() in IMG_FORMATS)
             # self.img_files = sorted([x for x in f if x.suffix[1:].lower() in IMG_FORMATS])  # pathlib
-            assert im_files, f"{self.prefix}No images found in {img_path}. {FORMATS_HELP_MSG}"
+            assert im_files, f"{self.prefix}No images found in {img_path}"
         except Exception as e:
             raise FileNotFoundError(f"{self.prefix}Error loading data from {img_path}\n{HELP_URL}") from e
         if self.fraction < 1:
-            # im_files = im_files[: round(len(im_files) * self.fraction)]
-            num_elements_to_select = round(len(im_files) * self.fraction)
-            im_files = random.sample(im_files, num_elements_to_select)
+            im_files = im_files[: round(len(im_files) * self.fraction)]
         return im_files
 
     def update_labels(self, include_class: Optional[list]):
         """Update labels to include only these classes (optional)."""
         include_class_array = np.array(include_class).reshape(1, -1)
         for i in range(len(self.labels)):
             if include_class is not None:
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/data/build.py` & `pyppbox-ultralytics-8.1.7/ultralytics/data/build.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,26 +7,26 @@
 import numpy as np
 import torch
 from PIL import Image
 from torch.utils.data import dataloader, distributed
 
 from ultralytics.data.loaders import (
     LOADERS,
-    LoadImagesAndVideos,
+    LoadImages,
     LoadPilAndNumpy,
     LoadScreenshots,
     LoadStreams,
     LoadTensor,
     SourceTypes,
     autocast_list,
 )
 from ultralytics.data.utils import IMG_FORMATS, VID_FORMATS
 from ultralytics.utils import RANK, colorstr
 from ultralytics.utils.checks import check_file
-from .dataset import YOLODataset, YOLOMultiModalDataset, GroundingDataset
+from .dataset import YOLODataset
 from .utils import PIN_MEMORY
 
 
 class InfiniteDataLoader(dataloader.DataLoader):
     """
     Dataloader that reuses workers.
 
@@ -78,18 +78,17 @@
 def seed_worker(worker_id):  # noqa
     """Set dataloader worker seed https://pytorch.org/docs/stable/notes/randomness.html#dataloader."""
     worker_seed = torch.initial_seed() % 2**32
     np.random.seed(worker_seed)
     random.seed(worker_seed)
 
 
-def build_yolo_dataset(cfg, img_path, batch, data, mode="train", rect=False, stride=32, multi_modal=False):
+def build_yolo_dataset(cfg, img_path, batch, data, mode="train", rect=False, stride=32):
     """Build YOLO Dataset."""
-    dataset = YOLOMultiModalDataset if multi_modal else YOLODataset
-    return dataset(
+    return YOLODataset(
         img_path=img_path,
         imgsz=cfg.imgsz,
         batch_size=batch,
         augment=mode == "train",  # augmentation
         hyp=cfg,  # TODO: probably add a get_hyps_from_cfg function
         rect=cfg.rect or rect,  # rectangular batches
         cache=cfg.cache or None,
@@ -100,35 +99,14 @@
         task=cfg.task,
         classes=cfg.classes,
         data=data,
         fraction=cfg.fraction if mode == "train" else 1.0,
     )
 
 
-def build_grounding(cfg, img_path, json_file, batch, mode="train", rect=False, stride=32):
-    """Build YOLO Dataset."""
-    return GroundingDataset(
-        img_path=img_path,
-        json_file=json_file,
-        imgsz=cfg.imgsz,
-        batch_size=batch,
-        augment=mode == "train",  # augmentation
-        hyp=cfg,  # TODO: probably add a get_hyps_from_cfg function
-        rect=cfg.rect or rect,  # rectangular batches
-        cache=cfg.cache or None,
-        single_cls=cfg.single_cls or False,
-        stride=int(stride),
-        pad=0.0 if mode == "train" else 0.5,
-        prefix=colorstr(f"{mode}: "),
-        task=cfg.task,
-        classes=cfg.classes,
-        fraction=cfg.fraction if mode == "train" else 1.0,
-    )
-
-
 def build_dataloader(dataset, batch, workers, shuffle=True, rank=-1):
     """Return an InfiniteDataLoader or DataLoader for training or validation set."""
     batch = min(batch, len(dataset))
     nd = torch.cuda.device_count()  # number of CUDA devices
     nw = min([os.cpu_count() // max(nd, 1), workers])  # number of workers
     sampler = None if rank == -1 else distributed.DistributedSampler(dataset, shuffle=shuffle)
     generator = torch.Generator()
@@ -147,15 +125,15 @@
 
 
 def check_source(source):
     """Check source type and return corresponding flag values."""
     webcam, screenshot, from_img, in_memory, tensor = False, False, False, False, False
     if isinstance(source, (str, int, Path)):  # int for local usb camera
         source = str(source)
-        is_file = Path(source).suffix[1:] in (IMG_FORMATS | VID_FORMATS)
+        is_file = Path(source).suffix[1:] in (IMG_FORMATS + VID_FORMATS)
         is_url = source.lower().startswith(("https://", "http://", "rtsp://", "rtmp://", "tcp://"))
         webcam = source.isnumeric() or source.endswith(".streams") or (is_url and not is_file)
         screenshot = source.lower() == "screen"
         if is_url and is_file:
             source = check_file(source)  # download
     elif isinstance(source, LOADERS):
         in_memory = True
@@ -168,41 +146,40 @@
         tensor = True
     else:
         raise TypeError("Unsupported image type. For supported types see https://docs.ultralytics.com/modes/predict")
 
     return source, webcam, screenshot, from_img, in_memory, tensor
 
 
-def load_inference_source(source=None, batch=1, vid_stride=1, buffer=False):
+def load_inference_source(source=None, vid_stride=1, buffer=False):
     """
     Loads an inference source for object detection and applies necessary transformations.
 
     Args:
         source (str, Path, Tensor, PIL.Image, np.ndarray): The input source for inference.
-        batch (int, optional): Batch size for dataloaders. Default is 1.
         vid_stride (int, optional): The frame interval for video sources. Default is 1.
         buffer (bool, optional): Determined whether stream frames will be buffered. Default is False.
 
     Returns:
         dataset (Dataset): A dataset object for the specified input source.
     """
-    source, stream, screenshot, from_img, in_memory, tensor = check_source(source)
-    source_type = source.source_type if in_memory else SourceTypes(stream, screenshot, from_img, tensor)
+    source, webcam, screenshot, from_img, in_memory, tensor = check_source(source)
+    source_type = source.source_type if in_memory else SourceTypes(webcam, screenshot, from_img, tensor)
 
     # Dataloader
     if tensor:
         dataset = LoadTensor(source)
     elif in_memory:
         dataset = source
-    elif stream:
+    elif webcam:
         dataset = LoadStreams(source, vid_stride=vid_stride, buffer=buffer)
     elif screenshot:
         dataset = LoadScreenshots(source)
     elif from_img:
         dataset = LoadPilAndNumpy(source)
     else:
-        dataset = LoadImagesAndVideos(source, batch=batch, vid_stride=vid_stride)
+        dataset = LoadImages(source, vid_stride=vid_stride)
 
     # Attach source types to the dataset
     setattr(dataset, "source_type", source_type)
 
     return dataset
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/data/converter.py` & `pyppbox-ultralytics-8.1.7/ultralytics/data/converter.py`

 * *Files 3% similar despite different names*

```diff
@@ -215,33 +215,30 @@
 
 def convert_coco(
     labels_dir="../coco/annotations/",
     save_dir="coco_converted/",
     use_segments=False,
     use_keypoints=False,
     cls91to80=True,
-    lvis=False,
 ):
     """
     Converts COCO dataset annotations to a YOLO annotation format  suitable for training YOLO models.
 
     Args:
         labels_dir (str, optional): Path to directory containing COCO dataset annotation files.
         save_dir (str, optional): Path to directory to save results to.
         use_segments (bool, optional): Whether to include segmentation masks in the output.
         use_keypoints (bool, optional): Whether to include keypoint annotations in the output.
         cls91to80 (bool, optional): Whether to map 91 COCO class IDs to the corresponding 80 COCO class IDs.
-        lvis (bool, optional): Whether to convert data in lvis dataset way.
 
     Example:
         ```python
         from ultralytics.data.converter import convert_coco
 
         convert_coco('../datasets/coco/annotations/', use_segments=True, use_keypoints=False, cls91to80=True)
-        convert_coco('../datasets/lvis/annotations/', use_segments=True, use_keypoints=False, cls91to80=False, lvis=True)
         ```
 
     Output:
         Generates output files in the specified output directory.
     """
 
     # Create dataset directory
@@ -250,46 +247,36 @@
         p.mkdir(parents=True, exist_ok=True)  # make dir
 
     # Convert classes
     coco80 = coco91_to_coco80_class()
 
     # Import json
     for json_file in sorted(Path(labels_dir).resolve().glob("*.json")):
-        lname = "" if lvis else json_file.stem.replace("instances_", "")
-        fn = Path(save_dir) / "labels" / lname  # folder name
+        fn = Path(save_dir) / "labels" / json_file.stem.replace("instances_", "")  # folder name
         fn.mkdir(parents=True, exist_ok=True)
-        if lvis:
-            # NOTE: create folders for both train and val in advance,
-            # since LVIS val set contains images from COCO 2017 train in addition to the COCO 2017 val split.
-            (fn / "train2017").mkdir(parents=True, exist_ok=True)
-            (fn / "val2017").mkdir(parents=True, exist_ok=True)
         with open(json_file) as f:
             data = json.load(f)
 
         # Create image dict
         images = {f'{x["id"]:d}': x for x in data["images"]}
         # Create image-annotations dict
         imgToAnns = defaultdict(list)
         for ann in data["annotations"]:
             imgToAnns[ann["image_id"]].append(ann)
 
-        image_txt = []
         # Write labels file
         for img_id, anns in TQDM(imgToAnns.items(), desc=f"Annotations {json_file}"):
             img = images[f"{img_id:d}"]
-            h, w = img["height"], img["width"]
-            f = str(Path(img["coco_url"]).relative_to("http://images.cocodataset.org")) if lvis else img["file_name"]
-            if lvis:
-                image_txt.append(str(Path("./images") / f))
+            h, w, f = img["height"], img["width"], img["file_name"]
 
             bboxes = []
             segments = []
             keypoints = []
             for ann in anns:
-                if ann.get("iscrowd", False):
+                if ann["iscrowd"]:
                     continue
                 # The COCO box format is [top left x, top left y, width, height]
                 box = np.array(ann["bbox"], dtype=np.float64)
                 box[:2] += box[2:] / 2  # xy top-left corner to center
                 box[[0, 2]] /= w  # normalize x
                 box[[1, 3]] /= h  # normalize y
                 if box[2] <= 0 or box[3] <= 0:  # if w <= 0 and h <= 0
@@ -323,20 +310,15 @@
                         line = (*(keypoints[i]),)  # cls, box, keypoints
                     else:
                         line = (
                             *(segments[i] if use_segments and len(segments[i]) > 0 else bboxes[i]),
                         )  # cls, box or segments
                     file.write(("%g " * len(line)).rstrip() % line + "\n")
 
-        if lvis:
-            with open((Path(save_dir) / json_file.name.replace("lvis_v1_", "").replace(".json", ".txt")), "a") as f:
-                for l in image_txt:
-                    f.write(f"{l}\n")
-
-    LOGGER.info(f"{'LVIS' if lvis else 'COCO'} data converted successfully.\nResults saved to {save_dir.resolve()}")
+    LOGGER.info(f"COCO data converted successfully.\nResults saved to {save_dir.resolve()}")
 
 
 def convert_dota_to_yolo_obb(dota_root_path: str):
     """
     Converts DOTA dataset annotations to YOLO OBB (Oriented Bounding Box) format.
 
     The function processes images in the 'train' and 'val' folders of the DOTA dataset. For each image, it reads the
@@ -350,25 +332,23 @@
         from ultralytics.data.converter import convert_dota_to_yolo_obb
 
         convert_dota_to_yolo_obb('path/to/DOTA')
         ```
 
     Notes:
         The directory structure assumed for the DOTA dataset:
-
             - DOTA
                 ├─ images
                 │   ├─ train
                 │   └─ val
                 └─ labels
                     ├─ train_original
                     └─ val_original
 
         After execution, the function will organize the labels into:
-
             - DOTA
                 └─ labels
                     ├─ train
                     └─ val
     """
     dota_root_path = Path(dota_root_path)
 
@@ -432,16 +412,16 @@
 
 
 def min_index(arr1, arr2):
     """
     Find a pair of indexes with the shortest distance between two arrays of 2D points.
 
     Args:
-        arr1 (np.ndarray): A NumPy array of shape (N, 2) representing N 2D points.
-        arr2 (np.ndarray): A NumPy array of shape (M, 2) representing M 2D points.
+        arr1 (np.array): A NumPy array of shape (N, 2) representing N 2D points.
+        arr2 (np.array): A NumPy array of shape (M, 2) representing M 2D points.
 
     Returns:
         (tuple): A tuple containing the indexes of the points with the shortest distance in arr1 and arr2 respectively.
     """
     dis = ((arr1[:, None, :] - arr2[None, :, :]) ** 2).sum(-1)
     return np.unravel_index(np.argmin(dis, axis=None), dis.shape)
 
@@ -477,23 +457,23 @@
                 if len(idx) == 2 and idx[0] > idx[1]:
                     idx = idx[::-1]
                     segments[i] = segments[i][::-1, :]
 
                 segments[i] = np.roll(segments[i], -idx[0], axis=0)
                 segments[i] = np.concatenate([segments[i], segments[i][:1]])
                 # Deal with the first segment and the last one
-                if i in {0, len(idx_list) - 1}:
+                if i in [0, len(idx_list) - 1]:
                     s.append(segments[i])
                 else:
                     idx = [0, idx[1] - idx[0]]
                     s.append(segments[i][idx[0] : idx[1] + 1])
 
         else:
             for i in range(len(idx_list) - 1, -1, -1):
-                if i not in {0, len(idx_list) - 1}:
+                if i not in [0, len(idx_list) - 1]:
                     idx = idx_list[i]
                     nidx = abs(idx[1] - idx[0])
                     s.append(segments[i][nidx:])
     return s
 
 
 def yolo_bbox2segment(im_dir, save_dir=None, sam_model="sam_b.pt"):
@@ -505,23 +485,22 @@
         im_dir (str | Path): Path to image directory to convert.
         save_dir (str | Path): Path to save the generated labels, labels will be saved
             into `labels-segment` in the same directory level of `im_dir` if save_dir is None. Default: None.
         sam_model (str): Segmentation model to use for intermediate segmentation data; optional.
 
     Notes:
         The input directory structure assumed for dataset:
-
             - im_dir
                 ├─ 001.jpg
                 ├─ ..
-                └─ NNN.jpg
+                ├─ NNN.jpg
             - labels
                 ├─ 001.txt
                 ├─ ..
-                └─ NNN.txt
+                ├─ NNN.txt
     """
     from ultralytics.data import YOLODataset
     from ultralytics.utils.ops import xywh2xyxy
     from ultralytics.utils import LOGGER
     from ultralytics import SAM
     from tqdm import tqdm
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/data/dataset.py` & `pyppbox-ultralytics-8.1.7/ultralytics/data/dataset.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,45 +1,24 @@
 # Ultralytics YOLO 🚀, AGPL-3.0 license
 import contextlib
 from itertools import repeat
-from collections import defaultdict
 from multiprocessing.pool import ThreadPool
 from pathlib import Path
 
 import cv2
-import json
 import numpy as np
 import torch
 import torchvision
 from PIL import Image
 
-from torch.utils.data import ConcatDataset
-from ultralytics.utils import LOCAL_RANK, NUM_THREADS, TQDM, colorstr
+from ultralytics.utils import LOCAL_RANK, NUM_THREADS, TQDM, colorstr, is_dir_writeable
 from ultralytics.utils.ops import resample_segments
-from .augment import (
-    Compose,
-    Format,
-    Instances,
-    LetterBox,
-    RandomLoadText,
-    classify_augmentations,
-    classify_transforms,
-    v8_transforms,
-)
+from .augment import Compose, Format, Instances, LetterBox, classify_augmentations, classify_transforms, v8_transforms
 from .base import BaseDataset
-from .utils import (
-    HELP_URL,
-    LOGGER,
-    get_hash,
-    img2label_paths,
-    verify_image,
-    verify_image_label,
-    load_dataset_cache_file,
-    save_dataset_cache_file,
-)
+from .utils import HELP_URL, LOGGER, get_hash, img2label_paths, verify_image, verify_image_label
 
 # Ultralytics dataset *.cache version, >= 1.0.0 for YOLOv8
 DATASET_CACHE_VERSION = "1.0.3"
 
 
 class YOLODataset(BaseDataset):
     """
@@ -73,15 +52,15 @@
             (dict): labels.
         """
         x = {"labels": []}
         nm, nf, ne, nc, msgs = 0, 0, 0, 0, []  # number missing, found, empty, corrupt, messages
         desc = f"{self.prefix}Scanning {path.parent / path.stem}..."
         total = len(self.im_files)
         nkpt, ndim = self.data.get("kpt_shape", (0, 0))
-        if self.use_keypoints and (nkpt <= 0 or ndim not in {2, 3}):
+        if self.use_keypoints and (nkpt <= 0 or ndim not in (2, 3)):
             raise ValueError(
                 "'kpt_shape' in data.yaml missing or incorrect. Should be a list with [number of "
                 "keypoints, number of dims (2 for x,y or 3 for x,y,visible)], i.e. 'kpt_shape: [17, 3]'"
             )
         with ThreadPool(NUM_THREADS) as pool:
             results = pool.imap(
                 func=verify_image_label,
@@ -122,15 +101,15 @@
         if msgs:
             LOGGER.info("\n".join(msgs))
         if nf == 0:
             LOGGER.warning(f"{self.prefix}WARNING ⚠️ No labels found in {path}. {HELP_URL}")
         x["hash"] = get_hash(self.label_files + self.im_files)
         x["results"] = nf, nm, ne, nc, len(self.im_files)
         x["msgs"] = msgs  # warnings
-        save_dataset_cache_file(self.prefix, path, x, DATASET_CACHE_VERSION)
+        save_dataset_cache_file(self.prefix, path, x)
         return x
 
     def get_labels(self):
         """Returns dictionary of labels for YOLO training."""
         self.label_files = img2label_paths(self.im_files)
         cache_path = Path(self.label_files[0]).parent.with_suffix(".cache")
         try:
@@ -138,15 +117,15 @@
             assert cache["version"] == DATASET_CACHE_VERSION  # matches current version
             assert cache["hash"] == get_hash(self.label_files + self.im_files)  # identical hash
         except (FileNotFoundError, AssertionError, AttributeError):
             cache, exists = self.cache_labels(cache_path), False  # run cache ops
 
         # Display cache
         nf, nm, ne, nc, n = cache.pop("results")  # found, missing, empty, corrupt, total
-        if exists and LOCAL_RANK in {-1, 0}:
+        if exists and LOCAL_RANK in (-1, 0):
             d = f"Scanning {cache_path}... {nf} images, {nm + ne} backgrounds, {nc} corrupt"
             TQDM(None, desc=self.prefix + d, total=n, initial=n)  # display results
             if cache["msgs"]:
                 LOGGER.info("\n".join(cache["msgs"]))  # display warnings
 
         # Read cache
         [cache.pop(k) for k in ("hash", "version", "msgs")]  # remove items
@@ -184,15 +163,14 @@
                 normalize=True,
                 return_mask=self.use_segments,
                 return_keypoint=self.use_keypoints,
                 return_obb=self.use_obb,
                 batch_idx=True,
                 mask_ratio=hyp.mask_ratio,
                 mask_overlap=hyp.overlap_mask,
-                bgr=hyp.bgr if self.augment else 0.0,  # only affect training.
             )
         )
         return transforms
 
     def close_mosaic(self, hyp):
         """Sets mosaic, copy_paste and mixup options to 0.0 and builds transformations."""
         hyp.mosaic = 0.0  # set mosaic ratio=0.0
@@ -231,63 +209,56 @@
         new_batch = {}
         keys = batch[0].keys()
         values = list(zip(*[list(b.values()) for b in batch]))
         for i, k in enumerate(keys):
             value = values[i]
             if k == "img":
                 value = torch.stack(value, 0)
-            if k in {"masks", "keypoints", "bboxes", "cls", "segments", "obb"}:
+            if k in ["masks", "keypoints", "bboxes", "cls", "segments", "obb"]:
                 value = torch.cat(value, 0)
             new_batch[k] = value
         new_batch["batch_idx"] = list(new_batch["batch_idx"])
         for i in range(len(new_batch["batch_idx"])):
             new_batch["batch_idx"][i] += i  # add target image index for build_targets()
         new_batch["batch_idx"] = torch.cat(new_batch["batch_idx"], 0)
         return new_batch
 
 
 # Classification dataloaders -------------------------------------------------------------------------------------------
 class ClassificationDataset(torchvision.datasets.ImageFolder):
     """
-    Extends torchvision ImageFolder to support YOLO classification tasks, offering functionalities like image
-    augmentation, caching, and verification. It's designed to efficiently handle large datasets for training deep
-    learning models, with optional image transformations and caching mechanisms to speed up training.
-
-    This class allows for augmentations using both torchvision and Albumentations libraries, and supports caching images
-    in RAM or on disk to reduce IO overhead during training. Additionally, it implements a robust verification process
-    to ensure data integrity and consistency.
+    YOLO Classification Dataset.
+
+    Args:
+        root (str): Dataset path.
 
     Attributes:
-        cache_ram (bool): Indicates if caching in RAM is enabled.
-        cache_disk (bool): Indicates if caching on disk is enabled.
-        samples (list): A list of tuples, each containing the path to an image, its class index, path to its .npy cache
-                        file (if caching on disk), and optionally the loaded image array (if caching in RAM).
-        torch_transforms (callable): PyTorch transforms to be applied to the images.
+        cache_ram (bool): True if images should be cached in RAM, False otherwise.
+        cache_disk (bool): True if images should be cached on disk, False otherwise.
+        samples (list): List of samples containing file, index, npy, and im.
+        torch_transforms (callable): torchvision transforms applied to the dataset.
+        album_transforms (callable, optional): Albumentations transforms applied to the dataset if augment is True.
     """
 
-    def __init__(self, root, args, augment=False, prefix=""):
+    def __init__(self, root, args, augment=False, cache=False, prefix=""):
         """
         Initialize YOLO object with root, image size, augmentations, and cache settings.
 
         Args:
-            root (str): Path to the dataset directory where images are stored in a class-specific folder structure.
-            args (Namespace): Configuration containing dataset-related settings such as image size, augmentation
-                parameters, and cache settings. It includes attributes like `imgsz` (image size), `fraction` (fraction
-                of data to use), `scale`, `fliplr`, `flipud`, `cache` (disk or RAM caching for faster training),
-                `auto_augment`, `hsv_h`, `hsv_s`, `hsv_v`, and `crop_fraction`.
-            augment (bool, optional): Whether to apply augmentations to the dataset. Default is False.
-            prefix (str, optional): Prefix for logging and cache filenames, aiding in dataset identification and
-                debugging. Default is an empty string.
+            root (str): Dataset path.
+            args (Namespace): Argument parser containing dataset related settings.
+            augment (bool, optional): True if dataset should be augmented, False otherwise. Defaults to False.
+            cache (bool | str | optional): Cache setting, can be True, False, 'ram' or 'disk'. Defaults to False.
         """
         super().__init__(root=root)
         if augment and args.fraction < 1.0:  # reduce training fraction
             self.samples = self.samples[: round(len(self.samples) * args.fraction)]
         self.prefix = colorstr(f"{prefix}: ") if prefix else ""
-        self.cache_ram = args.cache is True or str(args.cache).lower() == "ram"  # cache images into RAM
-        self.cache_disk = str(args.cache).lower() == "disk"  # cache images on hard drive as uncompressed *.npy files
+        self.cache_ram = cache is True or cache == "ram"
+        self.cache_disk = cache == "disk"
         self.samples = self.verify_images()  # filter out bad images
         self.samples = [list(x) + [Path(x[0]).with_suffix(".npy"), None] for x in self.samples]  # file, index, npy, im
         scale = (1.0 - args.scale, 1.0)  # (0.08, 1.0)
         self.torch_transforms = (
             classify_augmentations(
                 size=args.imgsz,
                 scale=scale,
@@ -302,17 +273,16 @@
             if augment
             else classify_transforms(size=args.imgsz, crop_fraction=args.crop_fraction)
         )
 
     def __getitem__(self, i):
         """Returns subset of data and targets corresponding to given indices."""
         f, j, fn, im = self.samples[i]  # filename, index, filename.with_suffix('.npy'), image
-        if self.cache_ram:
-            if im is None:  # Warning: two separate if statements required here, do not combine this with previous line
-                im = self.samples[i][3] = cv2.imread(f)
+        if self.cache_ram and im is None:
+            im = self.samples[i][3] = cv2.imread(f)
         elif self.cache_disk:
             if not fn.exists():  # load npy
                 np.save(fn.as_posix(), cv2.imread(f), allow_pickle=False)
             im = np.load(fn)
         else:  # read image
             im = cv2.imread(f)  # BGR
         # Convert NumPy array to PIL image
@@ -330,15 +300,15 @@
         path = Path(self.root).with_suffix(".cache")  # *.cache file path
 
         with contextlib.suppress(FileNotFoundError, AssertionError, AttributeError):
             cache = load_dataset_cache_file(path)  # attempt to load a *.cache file
             assert cache["version"] == DATASET_CACHE_VERSION  # matches current version
             assert cache["hash"] == get_hash([x[0] for x in self.samples])  # identical hash
             nf, nc, n, samples = cache.pop("results")  # found, missing, empty, corrupt, total
-            if LOCAL_RANK in {-1, 0}:
+            if LOCAL_RANK in (-1, 0):
                 d = f"{desc} {nf} images, {nc} corrupt"
                 TQDM(None, desc=d, total=n, initial=n)
                 if cache["msgs"]:
                     LOGGER.info("\n".join(cache["msgs"]))  # display warnings
             return samples
 
         # Run scan if *.cache retrieval failed
@@ -356,133 +326,39 @@
                 pbar.desc = f"{desc} {nf} images, {nc} corrupt"
             pbar.close()
         if msgs:
             LOGGER.info("\n".join(msgs))
         x["hash"] = get_hash([x[0] for x in self.samples])
         x["results"] = nf, nc, len(samples), samples
         x["msgs"] = msgs  # warnings
-        save_dataset_cache_file(self.prefix, path, x, DATASET_CACHE_VERSION)
+        save_dataset_cache_file(self.prefix, path, x)
         return samples
 
 
-class YOLOMultiModalDataset(YOLODataset):
-    """
-    Dataset class for loading object detection and/or segmentation labels in YOLO format.
-
-    Args:
-        data (dict, optional): A dataset YAML dictionary. Defaults to None.
-        task (str): An explicit arg to point current task, Defaults to 'detect'.
-
-    Returns:
-        (torch.utils.data.Dataset): A PyTorch dataset object that can be used for training an object detection model.
-    """
-
-    def __init__(self, *args, data=None, task="detect", **kwargs):
-        """Initializes a dataset object for object detection tasks with optional specifications."""
-        super().__init__(*args, data=data, task=task, **kwargs)
-
-    def update_labels_info(self, label):
-        """Add texts information for multi modal model training."""
-        labels = super().update_labels_info(label)
-        # NOTE: some categories are concatenated with its synonyms by `/`.
-        labels["texts"] = [v.split("/") for _, v in self.data["names"].items()]
-        return labels
-
-    def build_transforms(self, hyp=None):
-        """Enhances data transformations with optional text augmentation for multi-modal training."""
-        transforms = super().build_transforms(hyp)
-        if self.augment:
-            # NOTE: hard-coded the args for now.
-            transforms.insert(-1, RandomLoadText(max_samples=min(self.data["nc"], 80), padding=True))
-        return transforms
-
-
-class GroundingDataset(YOLODataset):
-    def __init__(self, *args, task="detect", json_file, **kwargs):
-        """Initializes a GroundingDataset for object detection, loading annotations from a specified JSON file."""
-        assert task == "detect", "`GroundingDataset` only support `detect` task for now!"
-        self.json_file = json_file
-        super().__init__(*args, task=task, data={}, **kwargs)
-
-    def get_img_files(self, img_path):
-        """The image files would be read in `get_labels` function, return empty list here."""
-        return []
-
-    def get_labels(self):
-        """Loads annotations from a JSON file, filters, and normalizes bounding boxes for each image."""
-        labels = []
-        LOGGER.info("Loading annotation file...")
-        with open(self.json_file, "r") as f:
-            annotations = json.load(f)
-        images = {f'{x["id"]:d}': x for x in annotations["images"]}
-        imgToAnns = defaultdict(list)
-        for ann in annotations["annotations"]:
-            imgToAnns[ann["image_id"]].append(ann)
-        for img_id, anns in TQDM(imgToAnns.items(), desc=f"Reading annotations {self.json_file}"):
-            img = images[f"{img_id:d}"]
-            h, w, f = img["height"], img["width"], img["file_name"]
-            im_file = Path(self.img_path) / f
-            if not im_file.exists():
-                continue
-            self.im_files.append(str(im_file))
-            bboxes = []
-            cat2id = {}
-            texts = []
-            for ann in anns:
-                if ann["iscrowd"]:
-                    continue
-                box = np.array(ann["bbox"], dtype=np.float32)
-                box[:2] += box[2:] / 2
-                box[[0, 2]] /= float(w)
-                box[[1, 3]] /= float(h)
-                if box[2] <= 0 or box[3] <= 0:
-                    continue
-
-                cat_name = " ".join([img["caption"][t[0] : t[1]] for t in ann["tokens_positive"]])
-                if cat_name not in cat2id:
-                    cat2id[cat_name] = len(cat2id)
-                    texts.append([cat_name])
-                cls = cat2id[cat_name]  # class
-                box = [cls] + box.tolist()
-                if box not in bboxes:
-                    bboxes.append(box)
-            lb = np.array(bboxes, dtype=np.float32) if len(bboxes) else np.zeros((0, 5), dtype=np.float32)
-            labels.append(
-                dict(
-                    im_file=im_file,
-                    shape=(h, w),
-                    cls=lb[:, 0:1],  # n, 1
-                    bboxes=lb[:, 1:],  # n, 4
-                    normalized=True,
-                    bbox_format="xywh",
-                    texts=texts,
-                )
-            )
-        return labels
-
-    def build_transforms(self, hyp=None):
-        """Configures augmentations for training with optional text loading; `hyp` adjusts augmentation intensity."""
-        transforms = super().build_transforms(hyp)
-        if self.augment:
-            # NOTE: hard-coded the args for now.
-            transforms.insert(-1, RandomLoadText(max_samples=80, padding=True))
-        return transforms
-
-
-class YOLOConcatDataset(ConcatDataset):
-    """
-    Dataset as a concatenation of multiple datasets.
-
-    This class is useful to assemble different existing datasets.
-    """
-
-    @staticmethod
-    def collate_fn(batch):
-        """Collates data samples into batches."""
-        return YOLODataset.collate_fn(batch)
+def load_dataset_cache_file(path):
+    """Load an Ultralytics *.cache dictionary from path."""
+    import gc
+
+    gc.disable()  # reduce pickle load time https://github.com/ultralytics/ultralytics/pull/1585
+    cache = np.load(str(path), allow_pickle=True).item()  # load dict
+    gc.enable()
+    return cache
+
+
+def save_dataset_cache_file(prefix, path, x):
+    """Save an Ultralytics dataset *.cache dictionary x to path."""
+    x["version"] = DATASET_CACHE_VERSION  # add cache version
+    if is_dir_writeable(path.parent):
+        if path.exists():
+            path.unlink()  # remove *.cache file if exists
+        np.save(str(path), x)  # save cache for next time
+        path.with_suffix(".cache.npy").rename(path)  # remove .npy suffix
+        LOGGER.info(f"{prefix}New cache created: {path}")
+    else:
+        LOGGER.warning(f"{prefix}WARNING ⚠️ Cache directory {path.parent} is not writeable, cache not saved.")
 
 
 # TODO: support semantic segmentation
 class SemanticDataset(BaseDataset):
     """
     Semantic Segmentation Dataset.
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/data/explorer/explorer.py` & `pyppbox-ultralytics-8.1.7/ultralytics/data/explorer/explorer.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,16 +55,15 @@
 class Explorer:
     def __init__(
         self,
         data: Union[str, Path] = "coco128.yaml",
         model: str = "yolov8n.pt",
         uri: str = USER_CONFIG_DIR / "explorer",
     ) -> None:
-        # Note duckdb==0.10.0 bug https://github.com/ultralytics/ultralytics/pull/8181
-        checks.check_requirements(["lancedb>=0.4.3", "duckdb<=0.9.2"])
+        checks.check_requirements(["lancedb>=0.4.3", "duckdb"])
         import lancedb
 
         self.connection = lancedb.connect(uri)
         self.table_name = Path(data).name.lower() + "_" + model.lower()
         self.sim_idx_base_name = (
             f"{self.table_name}_sim_idx".lower()
         )  # Use this name and append thres and top_k to reuse the table
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/data/explorer/gui/dash.py` & `pyppbox-ultralytics-8.1.7/ultralytics/data/explorer/gui/dash.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,17 +140,17 @@
         st.session_state["imgs"] = res.to_pydict()["im_file"]
         st.session_state["res"] = res
 
 
 def run_ai_query():
     """Execute SQL query and update session state with query results."""
     if not SETTINGS["openai_api_key"]:
-        st.session_state["error"] = (
-            'OpenAI API key not found in settings. Please run yolo settings openai_api_key="..."'
-        )
+        st.session_state[
+            "error"
+        ] = 'OpenAI API key not found in settings. Please run yolo settings openai_api_key="..."'
         return
     st.session_state["error"] = None
     query = st.session_state.get("ai_query")
     if query.rstrip().lstrip():
         exp = st.session_state["explorer"]
         res = exp.ask_ai(query)
         if not isinstance(res, pd.DataFrame) or res.empty:
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/data/explorer/utils.py` & `pyppbox-ultralytics-8.1.7/ultralytics/data/explorer/utils.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/data/loaders.py` & `pyppbox-ultralytics-8.1.7/ultralytics/data/loaders.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,32 +11,34 @@
 
 import cv2
 import numpy as np
 import requests
 import torch
 from PIL import Image
 
-from ultralytics.data.utils import IMG_FORMATS, VID_FORMATS, FORMATS_HELP_MSG
+from ultralytics.data.utils import IMG_FORMATS, VID_FORMATS
 from ultralytics.utils import LOGGER, is_colab, is_kaggle, ops
 from ultralytics.utils.checks import check_requirements
 
 
 @dataclass
 class SourceTypes:
     """Class to represent various types of input sources for predictions."""
 
-    stream: bool = False
+    webcam: bool = False
     screenshot: bool = False
     from_img: bool = False
     tensor: bool = False
 
 
 class LoadStreams:
     """
-    Stream Loader for various types of video streams, Supports RTSP, RTMP, HTTP, and TCP streams.
+    Stream Loader for various types of video streams.
+
+    Suitable for use with `yolo predict source='rtsp://example.com/media.mp4'`, supports RTSP, RTMP, HTTP, and TCP streams.
 
     Attributes:
         sources (str): The source input paths or URLs for the video streams.
         vid_stride (int): Video frame-rate stride, defaults to 1.
         buffer (bool): Whether to buffer input streams, defaults to False.
         running (bool): Flag to indicate if the streaming thread is running.
         mode (str): Set to 'stream' indicating real-time capture.
@@ -51,43 +53,37 @@
     Methods:
         __init__: Initialize the stream loader.
         update: Read stream frames in daemon thread.
         close: Close stream loader and release resources.
         __iter__: Returns an iterator object for the class.
         __next__: Returns source paths, transformed, and original images for processing.
         __len__: Return the length of the sources object.
-
-    Example:
-         ```bash
-         yolo predict source='rtsp://example.com/media.mp4'
-         ```
     """
 
     def __init__(self, sources="file.streams", vid_stride=1, buffer=False):
         """Initialize instance variables and check for consistent input stream shapes."""
         torch.backends.cudnn.benchmark = True  # faster for fixed-size inference
         self.buffer = buffer  # buffer input streams
         self.running = True  # running flag for Thread
         self.mode = "stream"
         self.vid_stride = vid_stride  # video frame-rate stride
 
         sources = Path(sources).read_text().rsplit() if os.path.isfile(sources) else [sources]
         n = len(sources)
-        self.bs = n
         self.fps = [0] * n  # frames per second
         self.frames = [0] * n
         self.threads = [None] * n
         self.caps = [None] * n  # video capture objects
         self.imgs = [[] for _ in range(n)]  # images
         self.shape = [[] for _ in range(n)]  # image shapes
         self.sources = [ops.clean_str(x) for x in sources]  # clean source names for later
         for i, s in enumerate(sources):  # index, source
             # Start thread to read frames from video stream
             st = f"{i + 1}/{n}: {s}... "
-            if urlparse(s).hostname in {"www.youtube.com", "youtube.com", "youtu.be"}:  # if source is YouTube video
+            if urlparse(s).hostname in ("www.youtube.com", "youtube.com", "youtu.be"):  # if source is YouTube video
                 # YouTube format i.e. 'https://www.youtube.com/watch?v=Zgi9g1ksQHc' or 'https://youtu.be/LNwODJXcvt4'
                 s = get_best_youtube_url(s)
             s = eval(s) if s.isnumeric() else s  # i.e. s = '0' local webcam
             if s == 0 and (is_colab() or is_kaggle()):
                 raise NotImplementedError(
                     "'source=0' webcam not supported in Colab and Kaggle notebooks. "
                     "Try running 'source=0' in a local environment."
@@ -109,14 +105,17 @@
             self.imgs[i].append(im)
             self.shape[i] = im.shape
             self.threads[i] = Thread(target=self.update, args=([i, self.caps[i], s]), daemon=True)
             LOGGER.info(f"{st}Success ✅ ({self.frames[i]} frames of shape {w}x{h} at {self.fps[i]:.2f} FPS)")
             self.threads[i].start()
         LOGGER.info("")  # newline
 
+        # Check for common shapes
+        self.bs = self.__len__()
+
     def update(self, i, cap, stream):
         """Read stream `i` frames in daemon thread."""
         n, f = 0, self.frames[i]  # frame number, frame array
         while self.running and cap.isOpened() and n < (f - 1):
             if len(self.imgs[i]) < 30:  # keep a <=30-image buffer
                 n += 1
                 cap.grab()  # .read() = .grab() followed by .retrieve()
@@ -172,19 +171,19 @@
                 images.append(x.pop(0))
 
             # Get the last frame, and clear the rest from the imgs buffer
             else:
                 images.append(x.pop(-1) if x else np.zeros(self.shape[i], dtype=np.uint8))
                 x.clear()
 
-        return self.sources, images, [""] * self.bs
+        return self.sources, images, None, ""
 
     def __len__(self):
         """Return the length of the sources object."""
-        return self.bs  # 1E12 frames = 32 streams at 30 FPS for 30 years
+        return len(self.sources)  # 1E12 frames = 32 streams at 30 FPS for 30 years
 
 
 class LoadScreenshots:
     """
     YOLOv8 screenshot dataloader.
 
     This class manages the loading of screenshot images for processing with YOLOv8.
@@ -221,15 +220,14 @@
             left, top, width, height = (int(x) for x in params)
         elif len(params) == 5:
             self.screen, left, top, width, height = (int(x) for x in params)
         self.mode = "stream"
         self.frame = 0
         self.sct = mss.mss()
         self.bs = 1
-        self.fps = 30
 
         # Parse monitor shape
         monitor = self.sct.monitors[self.screen]
         self.top = monitor["top"] if top is None else (monitor["top"] + top)
         self.left = monitor["left"] if left is None else (monitor["left"] + left)
         self.width = width or monitor["width"]
         self.height = height or monitor["height"]
@@ -241,18 +239,18 @@
 
     def __next__(self):
         """mss screen capture: get raw pixels from the screen as np array."""
         im0 = np.asarray(self.sct.grab(self.monitor))[:, :, :3]  # BGRA to BGR
         s = f"screen {self.screen} (LTWH): {self.left},{self.top},{self.width},{self.height}: "
 
         self.frame += 1
-        return [str(self.screen)], [im0], [s]  # screen, img, string
+        return [str(self.screen)], [im0], None, s  # screen, img, vid_cap, string
 
 
-class LoadImagesAndVideos:
+class LoadImages:
     """
     YOLOv8 image/video dataloader.
 
     This class manages the loading and pre-processing of image and video data for YOLOv8. It supports loading from
     various formats, including single image files, video files, and lists of image and video paths.
 
     Attributes:
@@ -267,15 +265,15 @@
         frames (int): Total number of frames in the video.
         count (int): Counter for iteration, initialized at 0 during `__iter__()`.
 
     Methods:
         _new_video(path): Create a new cv2.VideoCapture object for a given video path.
     """
 
-    def __init__(self, path, batch=1, vid_stride=1):
+    def __init__(self, path, vid_stride=1):
         """Initialize the Dataloader and raise FileNotFoundError if file not found."""
         parent = None
         if isinstance(path, str) and Path(path).suffix == ".txt":  # *.txt file with img/vid/dir on each line
             parent = Path(path).parent
             path = Path(path).read_text().splitlines()  # list of sources
         files = []
         for p in sorted(path) if isinstance(path, (list, tuple)) else [path]:
@@ -287,107 +285,83 @@
             elif os.path.isfile(a):
                 files.append(a)  # files (absolute or relative to CWD)
             elif parent and (parent / p).is_file():
                 files.append(str((parent / p).absolute()))  # files (relative to *.txt file parent)
             else:
                 raise FileNotFoundError(f"{p} does not exist")
 
-        # Define files as images or videos
-        images, videos = [], []
-        for f in files:
-            suffix = f.split(".")[-1].lower()  # Get file extension without the dot and lowercase
-            if suffix in IMG_FORMATS:
-                images.append(f)
-            elif suffix in VID_FORMATS:
-                videos.append(f)
+        images = [x for x in files if x.split(".")[-1].lower() in IMG_FORMATS]
+        videos = [x for x in files if x.split(".")[-1].lower() in VID_FORMATS]
         ni, nv = len(images), len(videos)
 
         self.files = images + videos
         self.nf = ni + nv  # number of files
-        self.ni = ni  # number of images
         self.video_flag = [False] * ni + [True] * nv
         self.mode = "image"
         self.vid_stride = vid_stride  # video frame-rate stride
-        self.bs = batch
+        self.bs = 1
         if any(videos):
             self._new_video(videos[0])  # new video
         else:
             self.cap = None
         if self.nf == 0:
-            raise FileNotFoundError(f"No images or videos found in {p}. {FORMATS_HELP_MSG}")
+            raise FileNotFoundError(
+                f"No images or videos found in {p}. "
+                f"Supported formats are:\nimages: {IMG_FORMATS}\nvideos: {VID_FORMATS}"
+            )
 
     def __iter__(self):
         """Returns an iterator object for VideoStream or ImageFolder."""
         self.count = 0
         return self
 
     def __next__(self):
-        """Returns the next batch of images or video frames along with their paths and metadata."""
-        paths, imgs, info = [], [], []
-        while len(imgs) < self.bs:
-            if self.count >= self.nf:  # end of file list
-                if len(imgs) > 0:
-                    return paths, imgs, info  # return last partial batch
-                else:
-                    raise StopIteration
-
-            path = self.files[self.count]
-            if self.video_flag[self.count]:
-                self.mode = "video"
-                if not self.cap or not self.cap.isOpened():
-                    self._new_video(path)
+        """Return next image, path and metadata from dataset."""
+        if self.count == self.nf:
+            raise StopIteration
+        path = self.files[self.count]
 
-                for _ in range(self.vid_stride):
-                    success = self.cap.grab()
-                    if not success:
-                        break  # end of video or failure
+        if self.video_flag[self.count]:
+            # Read video
+            self.mode = "video"
+            for _ in range(self.vid_stride):
+                self.cap.grab()
+            success, im0 = self.cap.retrieve()
+            while not success:
+                self.count += 1
+                self.cap.release()
+                if self.count == self.nf:  # last video
+                    raise StopIteration
+                path = self.files[self.count]
+                self._new_video(path)
+                success, im0 = self.cap.read()
+
+            self.frame += 1
+            # im0 = self._cv2_rotate(im0)  # for use if cv2 autorotation is False
+            s = f"video {self.count + 1}/{self.nf} ({self.frame}/{self.frames}) {path}: "
 
-                if success:
-                    success, im0 = self.cap.retrieve()
-                    if success:
-                        self.frame += 1
-                        paths.append(path)
-                        imgs.append(im0)
-                        info.append(f"video {self.count + 1}/{self.nf} (frame {self.frame}/{self.frames}) {path}: ")
-                        if self.frame == self.frames:  # end of video
-                            self.count += 1
-                            self.cap.release()
-                else:
-                    # Move to the next file if the current video ended or failed to open
-                    self.count += 1
-                    if self.cap:
-                        self.cap.release()
-                    if self.count < self.nf:
-                        self._new_video(self.files[self.count])
-            else:
-                self.mode = "image"
-                im0 = cv2.imread(path)  # BGR
-                if im0 is None:
-                    raise FileNotFoundError(f"Image Not Found {path}")
-                paths.append(path)
-                imgs.append(im0)
-                info.append(f"image {self.count + 1}/{self.nf} {path}: ")
-                self.count += 1  # move to the next file
-                if self.count >= self.ni:  # end of image list
-                    break
+        else:
+            # Read image
+            self.count += 1
+            im0 = cv2.imread(path)  # BGR
+            if im0 is None:
+                raise FileNotFoundError(f"Image Not Found {path}")
+            s = f"image {self.count}/{self.nf} {path}: "
 
-        return paths, imgs, info
+        return [path], [im0], self.cap, s
 
     def _new_video(self, path):
-        """Creates a new video capture object for the given path."""
+        """Create a new video capture object."""
         self.frame = 0
         self.cap = cv2.VideoCapture(path)
-        self.fps = int(self.cap.get(cv2.CAP_PROP_FPS))
-        if not self.cap.isOpened():
-            raise FileNotFoundError(f"Failed to open video {path}")
         self.frames = int(self.cap.get(cv2.CAP_PROP_FRAME_COUNT) / self.vid_stride)
 
     def __len__(self):
-        """Returns the number of batches in the object."""
-        return math.ceil(self.nf / self.bs)  # number of files
+        """Returns the number of files in the object."""
+        return self.nf  # number of files
 
 
 class LoadPilAndNumpy:
     """
     Load images from PIL and Numpy arrays for batch processing.
 
     This class is designed to manage loading and pre-processing of image data from both PIL and Numpy formats.
@@ -395,26 +369,28 @@
     downstream processing.
 
     Attributes:
         paths (list): List of image paths or autogenerated filenames.
         im0 (list): List of images stored as Numpy arrays.
         mode (str): Type of data being processed, defaults to 'image'.
         bs (int): Batch size, equivalent to the length of `im0`.
+        count (int): Counter for iteration, initialized at 0 during `__iter__()`.
 
     Methods:
         _single_check(im): Validate and format a single image to a Numpy array.
     """
 
     def __init__(self, im0):
         """Initialize PIL and Numpy Dataloader."""
         if not isinstance(im0, list):
             im0 = [im0]
         self.paths = [getattr(im, "filename", f"image{i}.jpg") for i, im in enumerate(im0)]
         self.im0 = [self._single_check(im) for im in im0]
         self.mode = "image"
+        # Generate fake paths
         self.bs = len(self.im0)
 
     @staticmethod
     def _single_check(im):
         """Validate and format an image to numpy array."""
         assert isinstance(im, (Image.Image, np.ndarray)), f"Expected PIL/np.ndarray image type, but got {type(im)}"
         if isinstance(im, Image.Image):
@@ -429,15 +405,15 @@
         return len(self.im0)
 
     def __next__(self):
         """Returns batch paths, images, processed images, None, ''."""
         if self.count == 1:  # loop only once as it's batch inference
             raise StopIteration
         self.count += 1
-        return self.paths, self.im0, [""] * self.bs
+        return self.paths, self.im0, None, ""
 
     def __iter__(self):
         """Enables iteration for class LoadPilAndNumpy."""
         self.count = 0
         return self
 
 
@@ -494,15 +470,15 @@
         return self
 
     def __next__(self):
         """Return next item in the iterator."""
         if self.count == 1:
             raise StopIteration
         self.count += 1
-        return self.paths, self.im0, [""] * self.bs
+        return self.paths, self.im0, None, ""
 
     def __len__(self):
         """Returns the batch size."""
         return self.bs
 
 
 def autocast_list(source):
@@ -518,14 +494,17 @@
                 f"type {type(im).__name__} is not a supported Ultralytics prediction source type. \n"
                 f"See https://docs.ultralytics.com/modes/predict for supported source types."
             )
 
     return files
 
 
+LOADERS = LoadStreams, LoadPilAndNumpy, LoadImages, LoadScreenshots  # tuple
+
+
 def get_best_youtube_url(url, use_pafy=True):
     """
     Retrieves the URL of the best quality MP4 video stream from a given YouTube video.
 
     This function uses the pafy or yt_dlp library to extract the video info from YouTube. It then finds the highest
     quality MP4 format that has video codec but no audio codec, and returns the URL of this video stream.
 
@@ -548,11 +527,7 @@
         with yt_dlp.YoutubeDL({"quiet": True}) as ydl:
             info_dict = ydl.extract_info(url, download=False)  # extract info
         for f in reversed(info_dict.get("formats", [])):  # reversed because best is usually last
             # Find a format with video codec, no audio, *.mp4 extension at least 1920x1080 size
             good_size = (f.get("width") or 0) >= 1920 or (f.get("height") or 0) >= 1080
             if good_size and f["vcodec"] != "none" and f["acodec"] == "none" and f["ext"] == "mp4":
                 return f.get("url")
-
-
-# Define constants
-LOADERS = (LoadStreams, LoadPilAndNumpy, LoadImagesAndVideos, LoadScreenshots)
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/data/split_dota.py` & `pyppbox-ultralytics-8.1.7/ultralytics/data/split_dota.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,15 +67,15 @@
                 - images
                     - train
                     - val
                 - labels
                     - train
                     - val
     """
-    assert split in {"train", "val"}, f"Split must be 'train' or 'val', not {split}."
+    assert split in ["train", "val"]
     im_dir = Path(data_root) / "images" / split
     assert im_dir.exists(), f"Can't find {im_dir}, please check your data root."
     im_files = glob(str(Path(data_root) / "images" / split / "*"))
     lb_files = img2label_paths(im_files)
     annos = []
     for im_file, lb_file in zip(im_files, lb_files):
         w, h = exif_size(Image.open(im_file))
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/data/utils.py` & `pyppbox-ultralytics-8.1.7/ultralytics/data/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,25 +25,23 @@
     SETTINGS_YAML,
     TQDM,
     clean_url,
     colorstr,
     emojis,
     yaml_load,
     yaml_save,
-    is_dir_writeable,
 )
 from ultralytics.utils.checks import check_file, check_font, is_ascii
 from ultralytics.utils.downloads import download, safe_download, unzip_file
 from ultralytics.utils.ops import segments2boxes
 
 HELP_URL = "See https://docs.ultralytics.com/datasets/detect for dataset formatting guidance."
-IMG_FORMATS = {"bmp", "dng", "jpeg", "jpg", "mpo", "png", "tif", "tiff", "webp", "pfm"}  # image suffixes
-VID_FORMATS = {"asf", "avi", "gif", "m4v", "mkv", "mov", "mp4", "mpeg", "mpg", "ts", "wmv", "webm"}  # video suffixes
+IMG_FORMATS = "bmp", "dng", "jpeg", "jpg", "mpo", "png", "tif", "tiff", "webp", "pfm"  # image suffixes
+VID_FORMATS = "asf", "avi", "gif", "m4v", "mkv", "mov", "mp4", "mpeg", "mpg", "ts", "wmv", "webm"  # video suffixes
 PIN_MEMORY = str(os.getenv("PIN_MEMORY", True)).lower() == "true"  # global pin_memory for dataloaders
-FORMATS_HELP_MSG = f"Supported formats are:\nimages: {IMG_FORMATS}\nvideos: {VID_FORMATS}"
 
 
 def img2label_paths(img_paths):
     """Define label paths as a function of image paths."""
     sa, sb = f"{os.sep}images{os.sep}", f"{os.sep}labels{os.sep}"  # /images/, /labels/ substrings
     return [sb.join(x.rsplit(sa, 1)).rsplit(".", 1)[0] + ".txt" for x in img_paths]
 
@@ -60,15 +58,15 @@
     """Returns exif-corrected PIL size."""
     s = img.size  # (width, height)
     if img.format == "JPEG":  # only support JPEG images
         with contextlib.suppress(Exception):
             exif = img.getexif()
             if exif:
                 rotation = exif.get(274, None)  # the EXIF key for the orientation tag is 274
-                if rotation in {6, 8}:  # rotation 270 or 90
+                if rotation in [6, 8]:  # rotation 270 or 90
                     s = s[1], s[0]
     return s
 
 
 def verify_image(args):
     """Verify one image."""
     (im_file, cls), prefix = args
@@ -76,16 +74,16 @@
     nf, nc, msg = 0, 0, ""
     try:
         im = Image.open(im_file)
         im.verify()  # PIL verify
         shape = exif_size(im)  # image size
         shape = (shape[1], shape[0])  # hw
         assert (shape[0] > 9) & (shape[1] > 9), f"image size {shape} <10 pixels"
-        assert im.format.lower() in IMG_FORMATS, f"Invalid image format {im.format}. {FORMATS_HELP_MSG}"
-        if im.format.lower() in {"jpg", "jpeg"}:
+        assert im.format.lower() in IMG_FORMATS, f"invalid image format {im.format}"
+        if im.format.lower() in ("jpg", "jpeg"):
             with open(im_file, "rb") as f:
                 f.seek(-2, 2)
                 if f.read() != b"\xff\xd9":  # corrupt JPEG
                     ImageOps.exif_transpose(Image.open(im_file)).save(im_file, "JPEG", subsampling=0, quality=100)
                     msg = f"{prefix}WARNING ⚠️ {im_file}: corrupt JPEG restored and saved"
         nf = 1
     except Exception as e:
@@ -102,16 +100,16 @@
     try:
         # Verify images
         im = Image.open(im_file)
         im.verify()  # PIL verify
         shape = exif_size(im)  # image size
         shape = (shape[1], shape[0])  # hw
         assert (shape[0] > 9) & (shape[1] > 9), f"image size {shape} <10 pixels"
-        assert im.format.lower() in IMG_FORMATS, f"invalid image format {im.format}. {FORMATS_HELP_MSG}"
-        if im.format.lower() in {"jpg", "jpeg"}:
+        assert im.format.lower() in IMG_FORMATS, f"invalid image format {im.format}"
+        if im.format.lower() in ("jpg", "jpeg"):
             with open(im_file, "rb") as f:
                 f.seek(-2, 2)
                 if f.read() != b"\xff\xd9":  # corrupt JPEG
                     ImageOps.exif_transpose(Image.open(im_file)).save(im_file, "JPEG", subsampling=0, quality=100)
                     msg = f"{prefix}WARNING ⚠️ {im_file}: corrupt JPEG restored and saved"
 
         # Verify labels
@@ -301,15 +299,15 @@
     # Resolve paths
     path = Path(extract_dir or data.get("path") or Path(data.get("yaml_file", "")).parent)  # dataset root
     if not path.is_absolute():
         path = (DATASETS_DIR / path).resolve()
 
     # Set paths
     data["path"] = path  # download scripts
-    for k in "train", "val", "test", "minival":
+    for k in "train", "val", "test":
         if data.get(k):  # prepend path
             if isinstance(data[k], str):
                 x = (path / data[k]).resolve()
                 if not x.exists() and data[k].startswith("../"):
                     x = (path / data[k][3:]).resolve()
                 data[k] = str(x)
             else:
@@ -333,15 +331,15 @@
                 safe_download(url=s, dir=DATASETS_DIR, delete=True)
             elif s.startswith("bash "):  # bash script
                 LOGGER.info(f"Running {s} ...")
                 r = os.system(s)
             else:  # python script
                 exec(s, {"yaml": data})
             dt = f"({round(time.time() - t, 1)}s)"
-            s = f"success ✅ {dt}, saved to {colorstr('bold', DATASETS_DIR)}" if r in {0, None} else f"failure {dt} ❌"
+            s = f"success ✅ {dt}, saved to {colorstr('bold', DATASETS_DIR)}" if r in (0, None) else f"failure {dt} ❌"
             LOGGER.info(f"Dataset download {s}\n")
     check_font("Arial.ttf" if is_ascii(data["names"]) else "Arial.Unicode.ttf")  # download fonts
 
     return data  # dictionary
 
 
 def check_cls_dataset(dataset, split=""):
@@ -363,17 +361,14 @@
             - 'nc' (int): The number of classes in the dataset.
             - 'names' (dict): A dictionary of class names in the dataset.
     """
 
     # Download (optional if dataset=https://file.zip is passed directly)
     if str(dataset).startswith(("http:/", "https:/")):
         dataset = safe_download(dataset, dir=DATASETS_DIR, unzip=True, delete=False)
-    elif Path(dataset).suffix in {".zip", ".tar", ".gz"}:
-        file = check_file(dataset)
-        dataset = safe_download(file, dir=DATASETS_DIR, unzip=True, delete=False)
 
     dataset = Path(dataset)
     data_dir = (dataset if dataset.is_dir() else (DATASETS_DIR / dataset)).resolve()
     if not data_dir.is_dir():
         LOGGER.warning(f"\nDataset not found ⚠️, missing path {data_dir}, attempting download...")
         t = time.time()
         if str(dataset) == "imagenet":
@@ -468,14 +463,15 @@
                 data = check_det_dataset(yaml_path, autodownload)  # dict
                 data["path"] = data_dir  # YAML path should be set to '' (relative) or parent (absolute)
             except Exception as e:
                 raise Exception("error/HUB/dataset_stats/init") from e
 
         self.hub_dir = Path(f'{data["path"]}-hub')
         self.im_dir = self.hub_dir / "images"
+        self.im_dir.mkdir(parents=True, exist_ok=True)  # makes /images
         self.stats = {"nc": len(data["names"]), "names": list(data["names"].values())}  # statistics dictionary
         self.data = data
 
     @staticmethod
     def _unzip(path):
         """Unzip data.zip."""
         if not str(path).endswith(".zip"):  # path is data.yaml
@@ -551,28 +547,26 @@
                         "per_class": (x > 0).sum(0).tolist(),
                     },
                     "labels": [{Path(k).name: _round(v)} for k, v in zip(dataset.im_files, dataset.labels)],
                 }
 
         # Save, print and return
         if save:
-            self.hub_dir.mkdir(parents=True, exist_ok=True)  # makes dataset-hub/
             stats_path = self.hub_dir / "stats.json"
             LOGGER.info(f"Saving {stats_path.resolve()}...")
             with open(stats_path, "w") as f:
                 json.dump(self.stats, f)  # save stats.json
         if verbose:
             LOGGER.info(json.dumps(self.stats, indent=2, sort_keys=False))
         return self.stats
 
     def process_images(self):
         """Compress images for Ultralytics HUB."""
         from ultralytics.data import YOLODataset  # ClassificationDataset
 
-        self.im_dir.mkdir(parents=True, exist_ok=True)  # makes dataset-hub/images/
         for split in "train", "val", "test":
             if self.data.get(split) is None:
                 continue
             dataset = YOLODataset(img_path=self.data[split], data=self.data)
             with ThreadPool(NUM_THREADS) as pool:
                 for _ in TQDM(pool.imap(self._hub_ops, dataset.im_files), total=len(dataset), desc=f"{split} images"):
                     pass
@@ -647,30 +641,7 @@
             (path.parent / x).unlink()  # remove existing
 
     LOGGER.info(f"Autosplitting images from {path}" + ", using *.txt labeled images only" * annotated_only)
     for i, img in TQDM(zip(indices, files), total=n):
         if not annotated_only or Path(img2label_paths([str(img)])[0]).exists():  # check label
             with open(path.parent / txt[i], "a") as f:
                 f.write(f"./{img.relative_to(path.parent).as_posix()}" + "\n")  # add image to txt file
-
-
-def load_dataset_cache_file(path):
-    """Load an Ultralytics *.cache dictionary from path."""
-    import gc
-
-    gc.disable()  # reduce pickle load time https://github.com/ultralytics/ultralytics/pull/1585
-    cache = np.load(str(path), allow_pickle=True).item()  # load dict
-    gc.enable()
-    return cache
-
-
-def save_dataset_cache_file(prefix, path, x, version):
-    """Save an Ultralytics dataset *.cache dictionary x to path."""
-    x["version"] = version  # add cache version
-    if is_dir_writeable(path.parent):
-        if path.exists():
-            path.unlink()  # remove *.cache file if exists
-        np.save(str(path), x)  # save cache for next time
-        path.with_suffix(".cache.npy").rename(path)  # remove .npy suffix
-        LOGGER.info(f"{prefix}New cache created: {path}")
-    else:
-        LOGGER.warning(f"{prefix}WARNING ⚠️ Cache directory {path.parent} is not writeable, cache not saved.")
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/engine/exporter.py` & `pyppbox-ultralytics-8.1.7/ultralytics/engine/exporter.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 CoreML                  | `coreml`                  | yolov8n.mlpackage
 TensorFlow SavedModel   | `saved_model`             | yolov8n_saved_model/
 TensorFlow GraphDef     | `pb`                      | yolov8n.pb
 TensorFlow Lite         | `tflite`                  | yolov8n.tflite
 TensorFlow Edge TPU     | `edgetpu`                 | yolov8n_edgetpu.tflite
 TensorFlow.js           | `tfjs`                    | yolov8n_web_model/
 PaddlePaddle            | `paddle`                  | yolov8n_paddle_model/
-NCNN                    | `ncnn`                    | yolov8n_ncnn_model/
+ncnn                    | `ncnn`                    | yolov8n_ncnn_model/
 
 Requirements:
     $ pip install "ultralytics[export]"
 
 Python:
     from ultralytics import YOLO
     model = YOLO('yolov8n.pt')
@@ -37,23 +37,21 @@
                          yolov8n.engine             # TensorRT
                          yolov8n.mlpackage          # CoreML (macOS-only)
                          yolov8n_saved_model        # TensorFlow SavedModel
                          yolov8n.pb                 # TensorFlow GraphDef
                          yolov8n.tflite             # TensorFlow Lite
                          yolov8n_edgetpu.tflite     # TensorFlow Edge TPU
                          yolov8n_paddle_model       # PaddlePaddle
-                         yolov8n_ncnn_model         # NCNN
 
 TensorFlow.js:
     $ cd .. && git clone https://github.com/zldrobit/tfjs-yolov5-example.git && cd tfjs-yolov5-example
     $ npm install
     $ ln -s ../../yolov5/yolov8n_web_model public/yolov8n_web_model
     $ npm start
 """
-
 import json
 import os
 import shutil
 import subprocess
 import time
 import warnings
 from copy import deepcopy
@@ -64,34 +62,34 @@
 import torch
 
 from ultralytics.cfg import get_cfg
 from ultralytics.data.dataset import YOLODataset
 from ultralytics.data.utils import check_det_dataset
 from ultralytics.nn.autobackend import check_class_names, default_class_names
 from ultralytics.nn.modules import C2f, Detect, RTDETRDecoder
-from ultralytics.nn.tasks import DetectionModel, SegmentationModel, WorldModel
+from ultralytics.nn.tasks import DetectionModel, SegmentationModel
 from ultralytics.utils import (
     ARM64,
     DEFAULT_CFG,
     LINUX,
     LOGGER,
     MACOS,
     ROOT,
     WINDOWS,
     __version__,
     callbacks,
     colorstr,
     get_default_args,
     yaml_save,
 )
-from ultralytics.utils.checks import PYTHON_VERSION, check_imgsz, check_is_path_safe, check_requirements, check_version
+from ultralytics.utils.checks import check_imgsz, check_is_path_safe, check_requirements, check_version
 from ultralytics.utils.downloads import attempt_download_asset, get_github_assets
 from ultralytics.utils.files import file_size, spaces_in_path
 from ultralytics.utils.ops import Profile
-from ultralytics.utils.torch_utils import TORCH_1_13, get_latest_opset, select_device, smart_inference_mode
+from ultralytics.utils.torch_utils import get_latest_opset, select_device, smart_inference_mode
 
 
 def export_formats():
     """YOLOv8 export formats."""
     import pandas
 
     x = [
@@ -103,15 +101,15 @@
         ["CoreML", "coreml", ".mlpackage", True, False],
         ["TensorFlow SavedModel", "saved_model", "_saved_model", True, True],
         ["TensorFlow GraphDef", "pb", ".pb", True, True],
         ["TensorFlow Lite", "tflite", ".tflite", True, False],
         ["TensorFlow Edge TPU", "edgetpu", "_edgetpu.tflite", True, False],
         ["TensorFlow.js", "tfjs", "_web_model", True, False],
         ["PaddlePaddle", "paddle", "_paddle_model", True, True],
-        ["NCNN", "ncnn", "_ncnn_model", True, True],
+        ["ncnn", "ncnn", "_ncnn_model", True, True],
     ]
     return pandas.DataFrame(x, columns=["Format", "Argument", "Suffix", "CPU", "GPU"])
 
 
 def gd_outputs(gd):
     """TensorFlow GraphDef model output node names."""
     name_list, input_list = [], []
@@ -155,29 +153,29 @@
 
         Args:
             cfg (str, optional): Path to a configuration file. Defaults to DEFAULT_CFG.
             overrides (dict, optional): Configuration overrides. Defaults to None.
             _callbacks (dict, optional): Dictionary of callback functions. Defaults to None.
         """
         self.args = get_cfg(cfg, overrides)
-        if self.args.format.lower() in {"coreml", "mlmodel"}:  # fix attempt for protobuf<3.20.x errors
+        if self.args.format.lower() in ("coreml", "mlmodel"):  # fix attempt for protobuf<3.20.x errors
             os.environ["PROTOCOL_BUFFERS_PYTHON_IMPLEMENTATION"] = "python"  # must run before TensorBoard callback
 
         self.callbacks = _callbacks or callbacks.get_default_callbacks()
         callbacks.add_integration_callbacks(self)
 
     @smart_inference_mode()
     def __call__(self, model=None):
         """Returns list of exported files/dirs after running callbacks."""
         self.run_callbacks("on_export_start")
         t = time.time()
         fmt = self.args.format.lower()  # to lowercase
-        if fmt in {"tensorrt", "trt"}:  # 'engine' aliases
+        if fmt in ("tensorrt", "trt"):  # 'engine' aliases
             fmt = "engine"
-        if fmt in {"mlmodel", "mlpackage", "mlprogram", "apple", "ios", "coreml"}:  # 'coreml' aliases
+        if fmt in ("mlmodel", "mlpackage", "mlprogram", "apple", "ios", "coreml"):  # 'coreml' aliases
             fmt = "coreml"
         fmts = tuple(export_formats()["Argument"][1:])  # available export formats
         flags = [x == fmt for x in fmts]
         if sum(flags) != 1:
             raise ValueError(f"Invalid export format='{fmt}'. Valid formats are {fmts}")
         jit, onnx, xml, engine, coreml, saved_model, pb, tflite, edgetpu, tfjs, paddle, ncnn = flags  # export booleans
 
@@ -197,21 +195,14 @@
             assert not self.args.dynamic, "half=True not compatible with dynamic=True, i.e. use only one."
         self.imgsz = check_imgsz(self.args.imgsz, stride=model.stride, min_dim=2)  # check image size
         if self.args.optimize:
             assert not ncnn, "optimize=True not compatible with format='ncnn', i.e. use optimize=False"
             assert self.device.type == "cpu", "optimize=True not compatible with cuda devices, i.e. use device='cpu'"
         if edgetpu and not LINUX:
             raise SystemError("Edge TPU export only supported on Linux. See https://coral.ai/docs/edgetpu/compiler/")
-        if isinstance(model, WorldModel):
-            LOGGER.warning(
-                "WARNING ⚠️ YOLOWorld (original version) export is not supported to any format.\n"
-                "WARNING ⚠️ YOLOWorldv2 models (i.e. 'yolov8s-worldv2.pt') only support export to "
-                "(torchscript, onnx, openvino, engine, coreml) formats. "
-                "See https://docs.ultralytics.com/models/yolo-world for details."
-            )
 
         # Input
         im = torch.zeros(self.args.batch, 3, *self.imgsz).to(self.device)
         file = Path(
             getattr(model, "pt_path", None) or getattr(model, "yaml_file", None) or model.yaml.get("yaml_file", "")
         )
         if file.suffix in {".yaml", ".yml"}:
@@ -221,26 +212,26 @@
         model = deepcopy(model).to(self.device)
         for p in model.parameters():
             p.requires_grad = False
         model.eval()
         model.float()
         model = model.fuse()
         for m in model.modules():
-            if isinstance(m, (Detect, RTDETRDecoder)):  # includes all Detect subclasses like Segment, Pose, OBB
+            if isinstance(m, (Detect, RTDETRDecoder)):  # Segment and Pose use Detect base class
                 m.dynamic = self.args.dynamic
                 m.export = True
                 m.format = self.args.format
             elif isinstance(m, C2f) and not any((saved_model, pb, tflite, edgetpu, tfjs)):
                 # EdgeTPU does not support FlexSplitV while split provides cleaner ONNX graph
                 m.forward = m.forward_split
 
         y = None
         for _ in range(2):
             y = model(im)  # dry runs
-        if self.args.half and onnx and self.device.type != "cpu":
+        if self.args.half and (engine or onnx) and self.device.type != "cpu":
             im, model = im.half(), model.half()  # to FP16
 
         # Filter warnings
         warnings.filterwarnings("ignore", category=torch.jit.TracerWarning)  # suppress TracerWarning
         warnings.filterwarnings("ignore", category=UserWarning)  # suppress shape prim::Constant missing ONNX warning
         warnings.filterwarnings("ignore", category=DeprecationWarning)  # suppress CoreML np.bool deprecation warning
 
@@ -255,18 +246,17 @@
         )
         self.pretty_name = Path(self.model.yaml.get("yaml_file", self.file)).stem.replace("yolo", "YOLO")
         data = model.args["data"] if hasattr(model, "args") and isinstance(model.args, dict) else ""
         description = f'Ultralytics {self.pretty_name} model {f"trained on {data}" if data else ""}'
         self.metadata = {
             "description": description,
             "author": "Ultralytics",
+            "license": "AGPL-3.0 https://ultralytics.com/license",
             "date": datetime.now().isoformat(),
             "version": __version__,
-            "license": "AGPL-3.0 License (https://ultralytics.com/license)",
-            "docs": "https://docs.ultralytics.com",
             "stride": int(max(model.stride)),
             "task": model.task,
             "batch": self.args.batch,
             "imgsz": self.imgsz,
             "names": model.names,
         }  # model metadata
         if model.task == "pose":
@@ -279,15 +269,15 @@
 
         # Exports
         f = [""] * len(fmts)  # exported filenames
         if jit or ncnn:  # TorchScript
             f[0], _ = self.export_torchscript()
         if engine:  # TensorRT required before ONNX
             f[1], _ = self.export_engine()
-        if onnx:  # ONNX
+        if onnx or xml:  # OpenVINO requires ONNX
             f[2], _ = self.export_onnx()
         if xml:  # OpenVINO
             f[3], _ = self.export_openvino()
         if coreml:  # CoreML
             f[4], _ = self.export_coreml()
         if any((saved_model, pb, tflite, edgetpu, tfjs)):  # TensorFlow formats
             self.args.int8 |= edgetpu
@@ -298,15 +288,15 @@
                 f[7], _ = self.export_tflite(keras_model=keras_model, nms=False, agnostic_nms=self.args.agnostic_nms)
             if edgetpu:
                 f[8], _ = self.export_edgetpu(tflite_model=Path(f[5]) / f"{self.file.stem}_full_integer_quant.tflite")
             if tfjs:
                 f[9], _ = self.export_tfjs()
         if paddle:  # PaddlePaddle
             f[10], _ = self.export_paddle()
-        if ncnn:  # NCNN
+        if ncnn:  # ncnn
             f[11], _ = self.export_ncnn()
 
         # Finish
         f = [str(x) for x in f if x]  # filter out '' and None
         if any(f):
             f = str(Path(f[-1]))
             square = self.imgsz[0] == self.imgsz[1]
@@ -349,16 +339,14 @@
 
     @try_export
     def export_onnx(self, prefix=colorstr("ONNX:")):
         """YOLOv8 ONNX export."""
         requirements = ["onnx>=1.12.0"]
         if self.args.simplify:
             requirements += ["onnxsim>=0.4.33", "onnxruntime-gpu" if torch.cuda.is_available() else "onnxruntime"]
-            if ARM64:
-                check_requirements("cmake")  # 'cmake' is needed to build onnxsim on aarch64
         check_requirements(requirements)
         import onnx  # noqa
 
         opset_version = self.args.opset or get_latest_opset()
         LOGGER.info(f"\n{prefix} starting export with onnx {onnx.__version__} opset {opset_version}...")
         f = str(self.file.with_suffix(".onnx"))
 
@@ -407,93 +395,76 @@
 
         onnx.save(model_onnx, f)
         return f, model_onnx
 
     @try_export
     def export_openvino(self, prefix=colorstr("OpenVINO:")):
         """YOLOv8 OpenVINO export."""
-        check_requirements("openvino>=2024.0.0")  # requires openvino: https://pypi.org/project/openvino/
-        import openvino as ov
+        check_requirements("openvino-dev>=2023.0")  # requires openvino-dev: https://pypi.org/project/openvino-dev/
+        import openvino.runtime as ov  # noqa
+        from openvino.tools import mo  # noqa
 
         LOGGER.info(f"\n{prefix} starting export with openvino {ov.__version__}...")
-        assert TORCH_1_13, f"OpenVINO export requires torch>=1.13.0 but torch=={torch.__version__} is installed"
-        ov_model = ov.convert_model(
-            self.model.cpu(),
-            input=None if self.args.dynamic else [self.im.shape],
-            example_input=self.im,
-        )
+        f = str(self.file).replace(self.file.suffix, f"_openvino_model{os.sep}")
+        fq = str(self.file).replace(self.file.suffix, f"_int8_openvino_model{os.sep}")
+        f_onnx = self.file.with_suffix(".onnx")
+        f_ov = str(Path(f) / self.file.with_suffix(".xml").name)
+        fq_ov = str(Path(fq) / self.file.with_suffix(".xml").name)
 
         def serialize(ov_model, file):
             """Set RT info, serialize and save metadata YAML."""
             ov_model.set_rt_info("YOLOv8", ["model_info", "model_type"])
             ov_model.set_rt_info(True, ["model_info", "reverse_input_channels"])
             ov_model.set_rt_info(114, ["model_info", "pad_value"])
             ov_model.set_rt_info([255.0], ["model_info", "scale_values"])
             ov_model.set_rt_info(self.args.iou, ["model_info", "iou_threshold"])
             ov_model.set_rt_info([v.replace(" ", "_") for v in self.model.names.values()], ["model_info", "labels"])
             if self.model.task != "classify":
                 ov_model.set_rt_info("fit_to_window_letterbox", ["model_info", "resize_type"])
 
-            ov.runtime.save_model(ov_model, file, compress_to_fp16=self.args.half)
+            ov.serialize(ov_model, file)  # save
             yaml_save(Path(file).parent / "metadata.yaml", self.metadata)  # add metadata.yaml
 
+        ov_model = mo.convert_model(
+            f_onnx, model_name=self.pretty_name, framework="onnx", compress_to_fp16=self.args.half
+        )  # export
+
         if self.args.int8:
-            fq = str(self.file).replace(self.file.suffix, f"_int8_openvino_model{os.sep}")
-            fq_ov = str(Path(fq) / self.file.with_suffix(".xml").name)
             if not self.args.data:
                 self.args.data = DEFAULT_CFG.data or "coco128.yaml"
                 LOGGER.warning(
                     f"{prefix} WARNING ⚠️ INT8 export requires a missing 'data' arg for calibration. "
                     f"Using default 'data={self.args.data}'."
                 )
-            check_requirements("nncf>=2.8.0")
+            check_requirements("nncf>=2.5.0")
             import nncf
 
             def transform_fn(data_item):
                 """Quantization transform function."""
                 assert (
                     data_item["img"].dtype == torch.uint8
                 ), "Input image must be uint8 for the quantization preprocessing"
                 im = data_item["img"].numpy().astype(np.float32) / 255.0  # uint8 to fp16/32 and 0 - 255 to 0.0 - 1.0
                 return np.expand_dims(im, 0) if im.ndim == 3 else im
 
             # Generate calibration data for integer quantization
             LOGGER.info(f"{prefix} collecting INT8 calibration images from 'data={self.args.data}'")
             data = check_det_dataset(self.args.data)
-            dataset = YOLODataset(data["val"], data=data, task=self.model.task, imgsz=self.imgsz[0], augment=False)
+            dataset = YOLODataset(data["val"], data=data, imgsz=self.imgsz[0], augment=False)
             n = len(dataset)
             if n < 300:
                 LOGGER.warning(f"{prefix} WARNING ⚠️ >300 images recommended for INT8 calibration, found {n} images.")
             quantization_dataset = nncf.Dataset(dataset, transform_fn)
-
-            ignored_scope = None
-            if isinstance(self.model.model[-1], Detect):
-                # Includes all Detect subclasses like Segment, Pose, OBB, WorldDetect
-                head_module_name = ".".join(list(self.model.named_modules())[-1][0].split(".")[:2])
-
-                ignored_scope = nncf.IgnoredScope(  # ignore operations
-                    patterns=[
-                        f".*{head_module_name}/.*/Add",
-                        f".*{head_module_name}/.*/Sub*",
-                        f".*{head_module_name}/.*/Mul*",
-                        f".*{head_module_name}/.*/Div*",
-                        f".*{head_module_name}\\.dfl.*",
-                    ],
-                    types=["Sigmoid"],
-                )
-
+            ignored_scope = nncf.IgnoredScope(types=["Multiply", "Subtract", "Sigmoid"])  # ignore operation
             quantized_ov_model = nncf.quantize(
                 ov_model, quantization_dataset, preset=nncf.QuantizationPreset.MIXED, ignored_scope=ignored_scope
             )
             serialize(quantized_ov_model, fq_ov)
             return fq, None
 
-        f = str(self.file).replace(self.file.suffix, f"_openvino_model{os.sep}")
-        f_ov = str(Path(f) / self.file.with_suffix(".xml").name)
-
         serialize(ov_model, f_ov)
         return f, None
 
     @try_export
     def export_paddle(self, prefix=colorstr("PaddlePaddle:")):
         """YOLOv8 Paddle export."""
         check_requirements(("paddlepaddle", "x2paddle"))
@@ -504,40 +475,40 @@
         f = str(self.file).replace(self.file.suffix, f"_paddle_model{os.sep}")
 
         pytorch2paddle(module=self.model, save_dir=f, jit_type="trace", input_examples=[self.im])  # export
         yaml_save(Path(f) / "metadata.yaml", self.metadata)  # add metadata.yaml
         return f, None
 
     @try_export
-    def export_ncnn(self, prefix=colorstr("NCNN:")):
+    def export_ncnn(self, prefix=colorstr("ncnn:")):
         """
-        YOLOv8 NCNN export using PNNX https://github.com/pnnx/pnnx.
+        YOLOv8 ncnn export using PNNX https://github.com/pnnx/pnnx.
         """
-        check_requirements("ncnn")
+        check_requirements("git+https://github.com/Tencent/ncnn.git" if ARM64 else "ncnn")  # requires ncnn
         import ncnn  # noqa
 
-        LOGGER.info(f"\n{prefix} starting export with NCNN {ncnn.__version__}...")
+        LOGGER.info(f"\n{prefix} starting export with ncnn {ncnn.__version__}...")
         f = Path(str(self.file).replace(self.file.suffix, f"_ncnn_model{os.sep}"))
         f_ts = self.file.with_suffix(".torchscript")
 
         name = Path("pnnx.exe" if WINDOWS else "pnnx")  # PNNX filename
         pnnx = name if name.is_file() else ROOT / name
         if not pnnx.is_file():
             LOGGER.warning(
                 f"{prefix} WARNING ⚠️ PNNX not found. Attempting to download binary file from "
                 "https://github.com/pnnx/pnnx/.\nNote PNNX Binary file must be placed in current working directory "
                 f"or in {ROOT}. See PNNX repo for full installation instructions."
             )
-            system = "macos" if MACOS else "windows" if WINDOWS else "linux-aarch64" if ARM64 else "linux"
-            _, assets = get_github_assets(repo="pnnx/pnnx", retry=True)
-            if assets:
-                url = [x for x in assets if f"{system}.zip" in x][0]
-            else:
-                url = f"https://github.com/pnnx/pnnx/releases/download/20240226/pnnx-20240226-{system}.zip"
-                LOGGER.warning(f"{prefix} WARNING ⚠️ PNNX GitHub assets not found, using default {url}")
+            system = ["macos"] if MACOS else ["windows"] if WINDOWS else ["ubuntu", "linux"]  # operating system
+            try:
+                _, assets = get_github_assets(repo="pnnx/pnnx", retry=True)
+                url = [x for x in assets if any(s in x for s in system)][0]
+            except Exception as e:
+                url = f"https://github.com/pnnx/pnnx/releases/download/20231127/pnnx-20231127-{system[0]}.zip"
+                LOGGER.warning(f"{prefix} WARNING ⚠️ PNNX GitHub assets not found: {e}, using default {url}")
             asset = attempt_download_asset(url, repo="pnnx/pnnx", release="latest")
             if check_is_path_safe(Path.cwd(), asset):  # avoid path traversal security vulnerability
                 unzip_dir = Path(asset).with_suffix("")
                 (unzip_dir / name).rename(pnnx)  # move binary to ROOT
                 shutil.rmtree(unzip_dir)  # delete unzip dir
                 Path(asset).unlink()  # delete zip
                 pnnx.chmod(0o777)  # set read, write, and execute permissions for everyone
@@ -620,16 +591,18 @@
                 import coremltools.optimize.coreml as cto
 
                 op_config = cto.OpPalettizerConfig(mode="kmeans", nbits=bits, weight_threshold=512)
                 config = cto.OptimizationConfig(global_config=op_config)
                 ct_model = cto.palettize_weights(ct_model, config=config)
         if self.args.nms and self.model.task == "detect":
             if mlmodel:
+                import platform
+
                 # coremltools<=6.2 NMS export requires Python<3.11
-                check_version(PYTHON_VERSION, "<3.11", name="Python ", hard=True)
+                check_version(platform.python_version(), "<3.11", name="Python ", hard=True)
                 weights_dir = None
             else:
                 ct_model.save(str(f))  # save otherwise weights_dir does not exist
                 weights_dir = str(f / "Data/com.apple.CoreML/weights")
             ct_model = self._pipeline_coreml(ct_model, weights_dir=weights_dir)
 
         m = self.metadata  # metadata dict
@@ -671,15 +644,17 @@
         f = self.file.with_suffix(".engine")  # TensorRT engine file
         logger = trt.Logger(trt.Logger.INFO)
         if self.args.verbose:
             logger.min_severity = trt.Logger.Severity.VERBOSE
 
         builder = trt.Builder(logger)
         config = builder.create_builder_config()
-        config.max_workspace_size = int(self.args.workspace * (1 << 30))
+        config.max_workspace_size = self.args.workspace * 1 << 30
+        # config.set_memory_pool_limit(trt.MemoryPoolType.WORKSPACE, workspace << 30)  # fix TRT 8.4 deprecation notice
+
         flag = 1 << int(trt.NetworkDefinitionCreationFlag.EXPLICIT_BATCH)
         network = builder.create_network(flag)
         parser = trt.OnnxParser(network, logger)
         if not parser.parse_from_file(f_onnx):
             raise RuntimeError(f"failed to load ONNX file: {f_onnx}")
 
         inputs = [network.get_input(i) for i in range(network.num_inputs)]
@@ -721,62 +696,56 @@
     @try_export
     def export_saved_model(self, prefix=colorstr("TensorFlow SavedModel:")):
         """YOLOv8 TensorFlow SavedModel export."""
         cuda = torch.cuda.is_available()
         try:
             import tensorflow as tf  # noqa
         except ImportError:
-            suffix = "-macos" if MACOS else "-aarch64" if ARM64 else "" if cuda else "-cpu"
-            version = "" if ARM64 else "<=2.13.1"
-            check_requirements(f"tensorflow{suffix}{version}")
+            check_requirements(f"tensorflow{'-macos' if MACOS else '-aarch64' if ARM64 else '' if cuda else '-cpu'}")
             import tensorflow as tf  # noqa
-        if ARM64:
-            check_requirements("cmake")  # 'cmake' is needed to build onnxsim on aarch64
         check_requirements(
             (
-                "onnx>=1.12.0",
+                "onnx",
                 "onnx2tf>=1.15.4,<=1.17.5",
                 "sng4onnx>=1.0.1",
                 "onnxsim>=0.4.33",
                 "onnx_graphsurgeon>=0.3.26",
                 "tflite_support",
-                "flatbuffers>=23.5.26,<100",  # update old 'flatbuffers' included inside tensorflow package
                 "onnxruntime-gpu" if cuda else "onnxruntime",
             ),
             cmds="--extra-index-url https://pypi.ngc.nvidia.com",
         )  # onnx_graphsurgeon only on NVIDIA
 
         LOGGER.info(f"\n{prefix} starting export with tensorflow {tf.__version__}...")
         check_version(
             tf.__version__,
             "<=2.13.1",
             name="tensorflow",
             verbose=True,
             msg="https://github.com/ultralytics/ultralytics/issues/5161",
         )
-        import onnx2tf
-
         f = Path(str(self.file).replace(self.file.suffix, "_saved_model"))
         if f.is_dir():
+            import shutil
+
             shutil.rmtree(f)  # delete output folder
 
         # Pre-download calibration file to fix https://github.com/PINTO0309/onnx2tf/issues/545
         onnx2tf_file = Path("calibration_image_sample_data_20x128x128x3_float32.npy")
         if not onnx2tf_file.exists():
             attempt_download_asset(f"{onnx2tf_file}.zip", unzip=True, delete=True)
 
         # Export to ONNX
         self.args.simplify = True
         f_onnx, _ = self.export_onnx()
 
         # Export to TF
         tmp_file = f / "tmp_tflite_int8_calibration_images.npy"  # int8 calibration images file
-        np_data = None
         if self.args.int8:
-            verbosity = "info"
+            verbosity = "--verbosity info"
             if self.args.data:
                 # Generate calibration data for integer quantization
                 LOGGER.info(f"{prefix} collecting INT8 calibration images from 'data={self.args.data}'")
                 data = check_det_dataset(self.args.data)
                 dataset = YOLODataset(data["val"], data=data, imgsz=self.imgsz[0], augment=False)
                 images = []
                 for i, batch in enumerate(dataset):
@@ -785,28 +754,24 @@
                     im = batch["img"].permute(1, 2, 0)[None]  # list to nparray, CHW to BHWC
                     images.append(im)
                 f.mkdir()
                 images = torch.cat(images, 0).float()
                 # mean = images.view(-1, 3).mean(0)  # imagenet mean [123.675, 116.28, 103.53]
                 # std = images.view(-1, 3).std(0)  # imagenet std [58.395, 57.12, 57.375]
                 np.save(str(tmp_file), images.numpy())  # BHWC
-                np_data = [["images", tmp_file, [[[[0, 0, 0]]]], [[[[255, 255, 255]]]]]]
+                int8 = f'-oiqt -qt per-tensor -cind images "{tmp_file}" "[[[[0, 0, 0]]]]" "[[[[255, 255, 255]]]]"'
+            else:
+                int8 = "-oiqt -qt per-tensor"
         else:
-            verbosity = "error"
+            verbosity = "--non_verbose"
+            int8 = ""
 
-        LOGGER.info(f"{prefix} starting TFLite export with onnx2tf {onnx2tf.__version__}...")
-        onnx2tf.convert(
-            input_onnx_file_path=f_onnx,
-            output_folder_path=str(f),
-            not_use_onnxsim=True,
-            verbosity=verbosity,
-            output_integer_quantized_tflite=self.args.int8,
-            quant_type="per-tensor",  # "per-tensor" (faster) or "per-channel" (slower but more accurate)
-            custom_input_op_name_np_data_path=np_data,
-        )
+        cmd = f'onnx2tf -i "{f_onnx}" -o "{f}" -nuo {verbosity} {int8}'.strip()
+        LOGGER.info(f"{prefix} running '{cmd}'")
+        subprocess.run(cmd, shell=True)
         yaml_save(f / "metadata.yaml", self.metadata)  # add metadata.yaml
 
         # Remove/rename TFLite models
         if self.args.int8:
             tmp_file.unlink(missing_ok=True)
             for file in f.rglob("*_dynamic_range_quant.tflite"):
                 file.rename(file.with_name(file.stem.replace("_dynamic_range_quant", "_int8") + file.suffix))
@@ -879,18 +844,16 @@
         subprocess.run(cmd, shell=True)
         self._add_tflite_metadata(f)
         return f, None
 
     @try_export
     def export_tfjs(self, prefix=colorstr("TensorFlow.js:")):
         """YOLOv8 TensorFlow.js export."""
-        check_requirements("tensorflowjs")
-        if ARM64:
-            # Fix error: `np.object` was a deprecated alias for the builtin `object` when exporting to TF.js on ARM64
-            check_requirements("numpy==1.23.5")
+        # JAX bug requiring install constraints in https://github.com/google/jax/issues/18978
+        check_requirements(["jax<=0.4.21", "jaxlib<=0.4.21", "tensorflowjs"])
         import tensorflow as tf
         import tensorflowjs as tfjs  # noqa
 
         LOGGER.info(f"\n{prefix} starting export with tensorflowjs {tfjs.__version__}...")
         f = str(self.file).replace(self.file.suffix, "_web_model")  # js dir
         f_pb = str(self.file.with_suffix(".pb"))  # *.pb path
 
@@ -898,18 +861,15 @@
         with open(f_pb, "rb") as file:
             gd.ParseFromString(file.read())
         outputs = ",".join(gd_outputs(gd))
         LOGGER.info(f"\n{prefix} output node names: {outputs}")
 
         quantization = "--quantize_float16" if self.args.half else "--quantize_uint8" if self.args.int8 else ""
         with spaces_in_path(f_pb) as fpb_, spaces_in_path(f) as f_:  # exporter can not handle spaces in path
-            cmd = (
-                "tensorflowjs_converter "
-                f'--input_format=tf_frozen_model {quantization} --output_node_names={outputs} "{fpb_}" "{f_}"'
-            )
+            cmd = f'tensorflowjs_converter --input_format=tf_frozen_model {quantization} --output_node_names={outputs} "{fpb_}" "{f_}"'
             LOGGER.info(f"{prefix} running '{cmd}'")
             subprocess.run(cmd, shell=True)
 
         if " " in f:
             LOGGER.warning(f"{prefix} WARNING ⚠️ your model may not work correctly with spaces in path '{f}'.")
 
         # f_json = Path(f) / 'model.json'  # *.json path
@@ -1096,18 +1056,18 @@
         pipeline.spec.description.metadata.userDefined.update(
             {"IoU threshold": str(nms.iouThreshold), "Confidence threshold": str(nms.confidenceThreshold)}
         )
 
         # Save the model
         model = ct.models.MLModel(pipeline.spec, weights_dir=weights_dir)
         model.input_description["image"] = "Input image"
-        model.input_description["iouThreshold"] = f"(optional) IoU threshold override (default: {nms.iouThreshold})"
-        model.input_description["confidenceThreshold"] = (
-            f"(optional) Confidence threshold override (default: {nms.confidenceThreshold})"
-        )
+        model.input_description["iouThreshold"] = f"(optional) IOU threshold override (default: {nms.iouThreshold})"
+        model.input_description[
+            "confidenceThreshold"
+        ] = f"(optional) Confidence threshold override (default: {nms.confidenceThreshold})"
         model.output_description["confidence"] = 'Boxes × Class confidence (see user-defined metadata "classes")'
         model.output_description["coordinates"] = "Boxes × [x, y, width, height] (relative to image size)"
         LOGGER.info(f"{prefix} pipeline success")
         return model
 
     def add_callback(self, event: str, callback):
         """Appends the given callback."""
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/engine/predictor.py` & `pyppbox-ultralytics-8.1.7/ultralytics/engine/predictor.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,19 +22,16 @@
                               yolov8n.engine             # TensorRT
                               yolov8n.mlpackage          # CoreML (macOS-only)
                               yolov8n_saved_model        # TensorFlow SavedModel
                               yolov8n.pb                 # TensorFlow GraphDef
                               yolov8n.tflite             # TensorFlow Lite
                               yolov8n_edgetpu.tflite     # TensorFlow Edge TPU
                               yolov8n_paddle_model       # PaddlePaddle
-                              yolov8n_ncnn_model         # NCNN
 """
-
 import platform
-import re
 import threading
 from pathlib import Path
 
 import cv2
 import numpy as np
 import torch
 
@@ -70,15 +67,17 @@
         args (SimpleNamespace): Configuration for the predictor.
         save_dir (Path): Directory to save results.
         done_warmup (bool): Whether the predictor has finished setup.
         model (nn.Module): Model used for prediction.
         data (dict): Data configuration.
         device (torch.device): Device used for prediction.
         dataset (Dataset): Dataset used for prediction.
-        vid_writer (dict): Dictionary of {save_path: video_writer, ...} writer for saving video output.
+        vid_path (str): Path to video file.
+        vid_writer (cv2.VideoWriter): Video writer for saving video output.
+        data_path (str): Path to data.
     """
 
     def __init__(self, cfg=DEFAULT_CFG, overrides=None, _callbacks=None):
         """
         Initializes the BasePredictor class.
 
         Args:
@@ -95,19 +94,18 @@
 
         # Usable if setup is done
         self.model = None
         self.data = self.args.data  # data_dict
         self.imgsz = None
         self.device = None
         self.dataset = None
-        self.vid_writer = {}  # dict of {save_path: video_writer, ...}
+        self.vid_path, self.vid_writer, self.vid_frame = None, None, None
         self.plotted_img = None
+        self.data_path = None
         self.source_type = None
-        self.seen = 0
-        self.windows = []
         self.batch = None
         self.results = None
         self.transforms = None
         self.callbacks = _callbacks or callbacks.get_default_callbacks()
         self.txt_path = None
         self._lock = threading.Lock()  # for automatic thread-safe inference
         callbacks.add_integration_callbacks(self)
@@ -147,18 +145,56 @@
 
         Args:
             im (List(np.ndarray)): (N, 3, h, w) for tensor, [(h, w, 3) x N] for list.
 
         Returns:
             (list): A list of transformed images.
         """
-        same_shapes = len({x.shape for x in im}) == 1
+        same_shapes = all(x.shape == im[0].shape for x in im)
         letterbox = LetterBox(self.imgsz, auto=same_shapes and self.model.pt, stride=self.model.stride)
         return [letterbox(image=x) for x in im]
 
+    def write_results(self, idx, results, batch):
+        """Write inference results to a file or directory."""
+        p, im, _ = batch
+        log_string = ""
+        if len(im.shape) == 3:
+            im = im[None]  # expand for batch dim
+        if self.source_type.webcam or self.source_type.from_img or self.source_type.tensor:  # batch_size >= 1
+            log_string += f"{idx}: "
+            frame = self.dataset.count
+        else:
+            frame = getattr(self.dataset, "frame", 0)
+        self.data_path = p
+        self.txt_path = str(self.save_dir / "labels" / p.stem) + ("" if self.dataset.mode == "image" else f"_{frame}")
+        log_string += "%gx%g " % im.shape[2:]  # print string
+        result = results[idx]
+        log_string += result.verbose()
+
+        if self.args.save or self.args.show:  # Add bbox to image
+            plot_args = {
+                "line_width": self.args.line_width,
+                "boxes": self.args.show_boxes,
+                "conf": self.args.show_conf,
+                "labels": self.args.show_labels,
+            }
+            if not self.args.retina_masks:
+                plot_args["im_gpu"] = im[idx]
+            self.plotted_img = result.plot(**plot_args)
+        # Write
+        if self.args.save_txt:
+            result.save_txt(f"{self.txt_path}.txt", save_conf=self.args.save_conf)
+        if self.args.save_crop:
+            result.save_crop(
+                save_dir=self.save_dir / "crops",
+                file_name=self.data_path.stem + ("" if self.dataset.mode == "image" else f"_{frame}"),
+            )
+
+        return log_string
+
     def postprocess(self, preds, img, orig_imgs):
         """Post-processes predictions for an image and returns them."""
         return preds
 
     def __call__(self, source=None, model=None, stream=False, *args, **kwargs):
         """Performs inference on an image or stream."""
         self.stream = stream
@@ -186,28 +222,26 @@
                 "transforms",
                 classify_transforms(self.imgsz[0], crop_fraction=self.args.crop_fraction),
             )
             if self.args.task == "classify"
             else None
         )
         self.dataset = load_inference_source(
-            source=source,
-            batch=self.args.batch,
-            vid_stride=self.args.vid_stride,
-            buffer=self.args.stream_buffer,
+            source=source, vid_stride=self.args.vid_stride, buffer=self.args.stream_buffer
         )
         self.source_type = self.dataset.source_type
         if not getattr(self, "stream", True) and (
-            self.source_type.stream
-            or self.source_type.screenshot
-            or len(self.dataset) > 1000  # many images
+            self.dataset.mode == "stream"  # streams
+            or len(self.dataset) > 1000  # images
             or any(getattr(self.dataset, "video_flag", [False]))
         ):  # videos
             LOGGER.warning(STREAM_WARNING)
-        self.vid_writer = {}
+        self.vid_path = [None] * self.dataset.bs
+        self.vid_writer = [None] * self.dataset.bs
+        self.vid_frame = [None] * self.dataset.bs
 
     @smart_inference_mode()
     def stream_inference(self, source=None, model=None, *args, **kwargs):
         """Streams real-time inference on camera feed and saves results to file."""
         if self.args.verbose:
             LOGGER.info("")
 
@@ -231,17 +265,18 @@
             self.seen, self.windows, self.batch = 0, [], None
             profilers = (
                 ops.Profile(device=self.device),
                 ops.Profile(device=self.device),
                 ops.Profile(device=self.device),
             )
             self.run_callbacks("on_predict_start")
-            for self.batch in self.dataset:
+            for batch in self.dataset:
                 self.run_callbacks("on_predict_batch_start")
-                paths, im0s, s = self.batch
+                self.batch = batch
+                path, im0s, vid_cap, s = batch
 
                 # Preprocess
                 with profilers[0]:
                     im = self.preprocess(im0s)
 
                 # Inference
                 with profilers[1]:
@@ -249,147 +284,120 @@
                     if self.args.embed:
                         yield from [preds] if isinstance(preds, torch.Tensor) else preds  # yield embedding tensors
                         continue
 
                 # Postprocess
                 with profilers[2]:
                     self.results = self.postprocess(preds, im, im0s)
-                self.run_callbacks("on_predict_postprocess_end")
 
+                self.run_callbacks("on_predict_postprocess_end")
                 # Visualize, save, write results
                 n = len(im0s)
                 for i in range(n):
                     self.seen += 1
                     self.results[i].speed = {
                         "preprocess": profilers[0].dt * 1e3 / n,
                         "inference": profilers[1].dt * 1e3 / n,
                         "postprocess": profilers[2].dt * 1e3 / n,
                     }
-                    if self.args.verbose or self.args.save or self.args.save_txt or self.args.show:
-                        s[i] += self.write_results(i, Path(paths[i]), im, s)
+                    p, im0 = path[i], None if self.source_type.tensor else im0s[i].copy()
+                    p = Path(p)
 
-                # Print batch results
-                if self.args.verbose:
-                    LOGGER.info("\n".join(s))
+                    if self.args.verbose or self.args.save or self.args.save_txt or self.args.show:
+                        s += self.write_results(i, self.results, (p, im, im0))
+                    if self.args.save or self.args.save_txt:
+                        self.results[i].save_dir = self.save_dir.__str__()
+                    if self.args.show and self.plotted_img is not None:
+                        self.show(p)
+                    if self.args.save and self.plotted_img is not None:
+                        self.save_preds(vid_cap, i, str(self.save_dir / p.name))
 
                 self.run_callbacks("on_predict_batch_end")
                 yield from self.results
 
+                # Print time (inference-only)
+                if self.args.verbose:
+                    LOGGER.info(f"{s}{profilers[1].dt * 1E3:.1f}ms")
+
         # Release assets
-        for v in self.vid_writer.values():
-            if isinstance(v, cv2.VideoWriter):
-                v.release()
+        if isinstance(self.vid_writer[-1], cv2.VideoWriter):
+            self.vid_writer[-1].release()  # release final video writer
 
-        # Print final results
+        # Print results
         if self.args.verbose and self.seen:
             t = tuple(x.t / self.seen * 1e3 for x in profilers)  # speeds per image
             LOGGER.info(
                 f"Speed: %.1fms preprocess, %.1fms inference, %.1fms postprocess per image at shape "
-                f"{(min(self.args.batch, self.seen), 3, *im.shape[2:])}" % t
+                f"{(1, 3, *im.shape[2:])}" % t
             )
         if self.args.save or self.args.save_txt or self.args.save_crop:
             nl = len(list(self.save_dir.glob("labels/*.txt")))  # number of labels
             s = f"\n{nl} label{'s' * (nl > 1)} saved to {self.save_dir / 'labels'}" if self.args.save_txt else ""
             LOGGER.info(f"Results saved to {colorstr('bold', self.save_dir)}{s}")
+
         self.run_callbacks("on_predict_end")
 
     def setup_model(self, model, verbose=True):
         """Initialize YOLO model with given parameters and set it to evaluation mode."""
         self.model = AutoBackend(
-            weights=model or self.args.model,
+            model or self.args.model,
             device=select_device(self.args.device, verbose=verbose),
             dnn=self.args.dnn,
             data=self.args.data,
             fp16=self.args.half,
-            batch=self.args.batch,
             fuse=True,
             verbose=verbose,
         )
 
         self.device = self.model.device  # update device
         self.args.half = self.model.fp16  # update half
         self.model.eval()
 
-    def write_results(self, i, p, im, s):
-        """Write inference results to a file or directory."""
-        string = ""  # print string
-        if len(im.shape) == 3:
-            im = im[None]  # expand for batch dim
-        if self.source_type.stream or self.source_type.from_img or self.source_type.tensor:  # batch_size >= 1
-            string += f"{i}: "
-            frame = self.dataset.count
-        else:
-            match = re.search(r"frame (\d+)/", s[i])
-            frame = int(match.group(1)) if match else None  # 0 if frame undetermined
-
-        self.txt_path = self.save_dir / "labels" / (p.stem + ("" if self.dataset.mode == "image" else f"_{frame}"))
-        string += "%gx%g " % im.shape[2:]
-        result = self.results[i]
-        result.save_dir = self.save_dir.__str__()  # used in other locations
-        string += result.verbose() + f"{result.speed['inference']:.1f}ms"
-
-        # Add predictions to image
-        if self.args.save or self.args.show:
-            self.plotted_img = result.plot(
-                line_width=self.args.line_width,
-                boxes=self.args.show_boxes,
-                conf=self.args.show_conf,
-                labels=self.args.show_labels,
-                im_gpu=None if self.args.retina_masks else im[i],
-            )
-
-        # Save results
-        if self.args.save_txt:
-            result.save_txt(f"{self.txt_path}.txt", save_conf=self.args.save_conf)
-        if self.args.save_crop:
-            result.save_crop(save_dir=self.save_dir / "crops", file_name=self.txt_path.stem)
-        if self.args.show:
-            self.show(str(p))
-        if self.args.save:
-            self.save_predicted_images(str(self.save_dir / p.name), frame)
-
-        return string
+    def show(self, p):
+        """Display an image in a window using OpenCV imshow()."""
+        im0 = self.plotted_img
+        if platform.system() == "Linux" and p not in self.windows:
+            self.windows.append(p)
+            cv2.namedWindow(str(p), cv2.WINDOW_NORMAL | cv2.WINDOW_KEEPRATIO)  # allow window resize (Linux)
+            cv2.resizeWindow(str(p), im0.shape[1], im0.shape[0])
+        cv2.imshow(str(p), im0)
+        cv2.waitKey(500 if self.batch[3].startswith("image") else 1)  # 1 millisecond
 
-    def save_predicted_images(self, save_path="", frame=0):
+    def save_preds(self, vid_cap, idx, save_path):
         """Save video predictions as mp4 at specified path."""
-        im = self.plotted_img
-
-        # Save videos and streams
-        if self.dataset.mode in {"stream", "video"}:
-            fps = self.dataset.fps if self.dataset.mode == "video" else 30
+        im0 = self.plotted_img
+        # Save imgs
+        if self.dataset.mode == "image":
+            cv2.imwrite(save_path, im0)
+        else:  # 'video' or 'stream'
             frames_path = f'{save_path.split(".", 1)[0]}_frames/'
-            if save_path not in self.vid_writer:  # new video
+            if self.vid_path[idx] != save_path:  # new video
+                self.vid_path[idx] = save_path
                 if self.args.save_frames:
                     Path(frames_path).mkdir(parents=True, exist_ok=True)
+                    self.vid_frame[idx] = 0
+                if isinstance(self.vid_writer[idx], cv2.VideoWriter):
+                    self.vid_writer[idx].release()  # release previous video writer
+                if vid_cap:  # video
+                    fps = int(vid_cap.get(cv2.CAP_PROP_FPS))  # integer required, floats produce error in MP4 codec
+                    w = int(vid_cap.get(cv2.CAP_PROP_FRAME_WIDTH))
+                    h = int(vid_cap.get(cv2.CAP_PROP_FRAME_HEIGHT))
+                else:  # stream
+                    fps, w, h = 30, im0.shape[1], im0.shape[0]
                 suffix, fourcc = (".mp4", "avc1") if MACOS else (".avi", "WMV2") if WINDOWS else (".avi", "MJPG")
-                self.vid_writer[save_path] = cv2.VideoWriter(
-                    filename=str(Path(save_path).with_suffix(suffix)),
-                    fourcc=cv2.VideoWriter_fourcc(*fourcc),
-                    fps=fps,  # integer required, floats produce error in MP4 codec
-                    frameSize=(im.shape[1], im.shape[0]),  # (width, height)
+                self.vid_writer[idx] = cv2.VideoWriter(
+                    str(Path(save_path).with_suffix(suffix)), cv2.VideoWriter_fourcc(*fourcc), fps, (w, h)
                 )
+            # Write video
+            self.vid_writer[idx].write(im0)
 
-            # Save video
-            self.vid_writer[save_path].write(im)
+            # Write frame
             if self.args.save_frames:
-                cv2.imwrite(f"{frames_path}{frame}.jpg", im)
-
-        # Save images
-        else:
-            cv2.imwrite(save_path, im)
-
-    def show(self, p=""):
-        """Display an image in a window using OpenCV imshow()."""
-        im = self.plotted_img
-        if platform.system() == "Linux" and p not in self.windows:
-            self.windows.append(p)
-            cv2.namedWindow(p, cv2.WINDOW_NORMAL | cv2.WINDOW_KEEPRATIO)  # allow window resize (Linux)
-            cv2.resizeWindow(p, im.shape[1], im.shape[0])  # (width, height)
-        cv2.imshow(p, im)
-        cv2.waitKey(300 if self.dataset.mode == "image" else 1)  # 1 millisecond
+                cv2.imwrite(f"{frames_path}{self.vid_frame[idx]}.jpg", im0)
+                self.vid_frame[idx] += 1
 
     def run_callbacks(self, event: str):
         """Runs all registered callbacks for a specific event."""
         for callback in self.callbacks.get(event, []):
             callback(self)
 
     def add_callback(self, event: str, func):
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/engine/results.py` & `pyppbox-ultralytics-8.1.7/ultralytics/engine/results.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,55 +63,38 @@
         return self.__class__(self.data[idx], self.orig_shape)
 
 
 class Results(SimpleClass):
     """
     A class for storing and manipulating inference results.
 
-    Attributes:
-        orig_img (numpy.ndarray): Original image as a numpy array.
-        orig_shape (tuple): Original image shape in (height, width) format.
-        boxes (Boxes, optional): Object containing detection bounding boxes.
-        masks (Masks, optional): Object containing detection masks.
-        probs (Probs, optional): Object containing class probabilities for classification tasks.
-        keypoints (Keypoints, optional): Object containing detected keypoints for each object.
-        speed (dict): Dictionary of preprocess, inference, and postprocess speeds (ms/image).
-        names (dict): Dictionary of class names.
-        path (str): Path to the image file.
+    Args:
+        orig_img (numpy.ndarray): The original image as a numpy array.
+        path (str): The path to the image file.
+        names (dict): A dictionary of class names.
+        boxes (torch.tensor, optional): A 2D tensor of bounding box coordinates for each detection.
+        masks (torch.tensor, optional): A 3D tensor of detection masks, where each mask is a binary image.
+        probs (torch.tensor, optional): A 1D tensor of probabilities of each class for classification task.
+        keypoints (List[List[float]], optional): A list of detected keypoints for each object.
 
-    Methods:
-        update(boxes=None, masks=None, probs=None, obb=None): Updates object attributes with new detection results.
-        cpu(): Returns a copy of the Results object with all tensors on CPU memory.
-        numpy(): Returns a copy of the Results object with all tensors as numpy arrays.
-        cuda(): Returns a copy of the Results object with all tensors on GPU memory.
-        to(*args, **kwargs): Returns a copy of the Results object with tensors on a specified device and dtype.
-        new(): Returns a new Results object with the same image, path, and names.
-        plot(...): Plots detection results on an input image, returning an annotated image.
-        show(): Show annotated results to screen.
-        save(filename): Save annotated results to file.
-        verbose(): Returns a log string for each task, detailing detections and classifications.
-        save_txt(txt_file, save_conf=False): Saves detection results to a text file.
-        save_crop(save_dir, file_name=Path("im.jpg")): Saves cropped detection images.
-        tojson(normalize=False): Converts detection results to JSON format.
+    Attributes:
+        orig_img (numpy.ndarray): The original image as a numpy array.
+        orig_shape (tuple): The original image shape in (height, width) format.
+        boxes (Boxes, optional): A Boxes object containing the detection bounding boxes.
+        masks (Masks, optional): A Masks object containing the detection masks.
+        probs (Probs, optional): A Probs object containing probabilities of each class for classification task.
+        keypoints (Keypoints, optional): A Keypoints object containing detected keypoints for each object.
+        speed (dict): A dictionary of preprocess, inference, and postprocess speeds in milliseconds per image.
+        names (dict): A dictionary of class names.
+        path (str): The path to the image file.
+        _keys (tuple): A tuple of attribute names for non-empty attributes.
     """
 
     def __init__(self, orig_img, path, names, boxes=None, masks=None, probs=None, keypoints=None, obb=None) -> None:
-        """
-        Initialize the Results class.
-
-        Args:
-            orig_img (numpy.ndarray): The original image as a numpy array.
-            path (str): The path to the image file.
-            names (dict): A dictionary of class names.
-            boxes (torch.tensor, optional): A 2D tensor of bounding box coordinates for each detection.
-            masks (torch.tensor, optional): A 3D tensor of detection masks, where each mask is a binary image.
-            probs (torch.tensor, optional): A 1D tensor of probabilities of each class for classification task.
-            keypoints (torch.tensor, optional): A 2D tensor of keypoint coordinates for each detection.
-            obb (torch.tensor, optional): A 2D tensor of oriented bounding box coordinates for each detection.
-        """
+        """Initialize the Results class."""
         self.orig_img = orig_img
         self.orig_shape = orig_img.shape[:2]
         self.boxes = Boxes(boxes, self.orig_shape) if boxes is not None else None  # native size boxes
         self.masks = Masks(masks, self.orig_shape) if masks is not None else None  # native size or imgsz masks
         self.probs = Probs(probs) if probs is not None else None
         self.keypoints = Keypoints(keypoints, self.orig_shape) if keypoints is not None else None
         self.obb = OBB(obb, self.orig_shape) if obb is not None else None
@@ -194,17 +177,14 @@
         im_gpu=None,
         kpt_radius=5,
         kpt_line=True,
         labels=True,
         boxes=True,
         masks=True,
         probs=True,
-        show=False,
-        save=False,
-        filename=None,
     ):
         """
         Plots the detection results on an input RGB image. Accepts a numpy array (cv2) or a PIL Image.
 
         Args:
             conf (bool): Whether to plot the detection confidence score.
             line_width (float, optional): The line width of the bounding boxes. If None, it is scaled to the image size.
@@ -215,17 +195,14 @@
             im_gpu (torch.Tensor): Normalized image in gpu with shape (1, 3, 640, 640), for faster mask plotting.
             kpt_radius (int, optional): Radius of the drawn keypoints. Default is 5.
             kpt_line (bool): Whether to draw lines connecting keypoints.
             labels (bool): Whether to plot the label of bounding boxes.
             boxes (bool): Whether to plot the bounding boxes.
             masks (bool): Whether to plot the masks.
             probs (bool): Whether to plot classification probability
-            show (bool): Whether to display the annotated image directly.
-            save (bool): Whether to save the annotated image to `filename`.
-            filename (str): Filename to save image to if save is True.
 
         Returns:
             (numpy.ndarray): A numpy array of the annotated image.
 
         Example:
             ```python
             from PIL import Image
@@ -287,35 +264,16 @@
             annotator.text([x, x], text, txt_color=(255, 255, 255))  # TODO: allow setting colors
 
         # Plot Pose results
         if self.keypoints is not None:
             for k in reversed(self.keypoints.data):
                 annotator.kpts(k, self.orig_shape, radius=kpt_radius, kpt_line=kpt_line)
 
-        # Show results
-        if show:
-            annotator.show(self.path)
-
-        # Save results
-        if save:
-            annotator.save(filename)
-
         return annotator.result()
 
-    def show(self, *args, **kwargs):
-        """Show annotated results image."""
-        self.plot(show=True, *args, **kwargs)
-
-    def save(self, filename=None, *args, **kwargs):
-        """Save annotated results image."""
-        if not filename:
-            filename = f"results_{Path(self.path).name}"
-        self.plot(save=True, filename=filename, *args, **kwargs)
-        return filename
-
     def verbose(self):
         """Return log string for each task."""
         log_string = ""
         probs = self.probs
         boxes = self.boxes
         if len(self) == 0:
             return log_string if probs is not None else f"{log_string}(no detections), "
@@ -381,100 +339,79 @@
             save_one_box(
                 d.xyxy,
                 self.orig_img.copy(),
                 file=Path(save_dir) / self.names[int(d.cls)] / f"{Path(file_name)}.jpg",
                 BGR=True,
             )
 
-    def summary(self, normalize=False, decimals=5):
-        """Convert the results to a summarized format."""
+    def tojson(self, normalize=False):
+        """Convert the object to JSON format."""
         if self.probs is not None:
-            LOGGER.warning("Warning: Classify results do not support the `summary()` method yet.")
+            LOGGER.warning("Warning: Classify task do not support `tojson` yet.")
             return
 
+        import json
+
         # Create list of detection dictionaries
         results = []
         data = self.boxes.data.cpu().tolist()
         h, w = self.orig_shape if normalize else (1, 1)
         for i, row in enumerate(data):  # xyxy, track_id if tracking, conf, class_id
-            box = {
-                "x1": round(row[0] / w, decimals),
-                "y1": round(row[1] / h, decimals),
-                "x2": round(row[2] / w, decimals),
-                "y2": round(row[3] / h, decimals),
-            }
-            conf = round(row[-2], decimals)
+            box = {"x1": row[0] / w, "y1": row[1] / h, "x2": row[2] / w, "y2": row[3] / h}
+            conf = row[-2]
             class_id = int(row[-1])
-            result = {"name": self.names[class_id], "class": class_id, "confidence": conf, "box": box}
+            name = self.names[class_id]
+            result = {"name": name, "class": class_id, "confidence": conf, "box": box}
             if self.boxes.is_track:
                 result["track_id"] = int(row[-3])  # track ID
             if self.masks:
-                result["segments"] = {
-                    "x": (self.masks.xy[i][:, 0] / w).round(decimals).tolist(),
-                    "y": (self.masks.xy[i][:, 1] / h).round(decimals).tolist(),
-                }
+                x, y = self.masks.xy[i][:, 0], self.masks.xy[i][:, 1]  # numpy array
+                result["segments"] = {"x": (x / w).tolist(), "y": (y / h).tolist()}
             if self.keypoints is not None:
                 x, y, visible = self.keypoints[i].data[0].cpu().unbind(dim=1)  # torch Tensor
-                result["keypoints"] = {
-                    "x": (x / w).numpy().round(decimals).tolist(),  # decimals named argument required
-                    "y": (y / h).numpy().round(decimals).tolist(),
-                    "visible": visible.numpy().round(decimals).tolist(),
-                }
+                result["keypoints"] = {"x": (x / w).tolist(), "y": (y / h).tolist(), "visible": visible.tolist()}
             results.append(result)
 
-        return results
-
-    def tojson(self, normalize=False, decimals=5):
-        """Convert the results to JSON format."""
-        import json
-
-        return json.dumps(self.summary(normalize=normalize, decimals=decimals), indent=2)
+        # Convert detections to JSON
+        return json.dumps(results, indent=2)
 
 
 class Boxes(BaseTensor):
     """
-    Manages detection boxes, providing easy access and manipulation of box coordinates, confidence scores, class
-    identifiers, and optional tracking IDs. Supports multiple formats for box coordinates, including both absolute and
-    normalized forms.
+    A class for storing and manipulating detection boxes.
+
+    Args:
+        boxes (torch.Tensor | numpy.ndarray): A tensor or numpy array containing the detection boxes,
+            with shape (num_boxes, 6) or (num_boxes, 7). The last two columns contain confidence and class values.
+            If present, the third last column contains track IDs.
+        orig_shape (tuple): Original image size, in the format (height, width).
 
     Attributes:
-        data (torch.Tensor): The raw tensor containing detection boxes and their associated data.
-        orig_shape (tuple): The original image size as a tuple (height, width), used for normalization.
-        is_track (bool): Indicates whether tracking IDs are included in the box data.
-
-    Properties:
-        xyxy (torch.Tensor | numpy.ndarray): Boxes in [x1, y1, x2, y2] format.
-        conf (torch.Tensor | numpy.ndarray): Confidence scores for each box.
-        cls (torch.Tensor | numpy.ndarray): Class labels for each box.
-        id (torch.Tensor | numpy.ndarray, optional): Tracking IDs for each box, if available.
-        xywh (torch.Tensor | numpy.ndarray): Boxes in [x, y, width, height] format, calculated on demand.
-        xyxyn (torch.Tensor | numpy.ndarray): Normalized [x1, y1, x2, y2] boxes, relative to `orig_shape`.
-        xywhn (torch.Tensor | numpy.ndarray): Normalized [x, y, width, height] boxes, relative to `orig_shape`.
+        xyxy (torch.Tensor | numpy.ndarray): The boxes in xyxy format.
+        conf (torch.Tensor | numpy.ndarray): The confidence values of the boxes.
+        cls (torch.Tensor | numpy.ndarray): The class values of the boxes.
+        id (torch.Tensor | numpy.ndarray): The track IDs of the boxes (if available).
+        xywh (torch.Tensor | numpy.ndarray): The boxes in xywh format.
+        xyxyn (torch.Tensor | numpy.ndarray): The boxes in xyxy format normalized by original image size.
+        xywhn (torch.Tensor | numpy.ndarray): The boxes in xywh format normalized by original image size.
+        data (torch.Tensor): The raw bboxes tensor (alias for `boxes`).
 
     Methods:
-        cpu(): Moves the boxes to CPU memory.
-        numpy(): Converts the boxes to a numpy array format.
-        cuda(): Moves the boxes to CUDA (GPU) memory.
-        to(device, dtype=None): Moves the boxes to the specified device.
+        cpu(): Move the object to CPU memory.
+        numpy(): Convert the object to a numpy array.
+        cuda(): Move the object to CUDA memory.
+        to(*args, **kwargs): Move the object to the specified device.
     """
 
     def __init__(self, boxes, orig_shape) -> None:
-        """
-        Initialize the Boxes class.
-
-        Args:
-            boxes (torch.Tensor | numpy.ndarray): A tensor or numpy array containing the detection boxes, with
-                shape (num_boxes, 6) or (num_boxes, 7). The last two columns contain confidence and class values.
-                If present, the third last column contains track IDs.
-            orig_shape (tuple): Original image size, in the format (height, width).
-        """
+        """Initialize the Boxes class."""
         if boxes.ndim == 1:
             boxes = boxes[None, :]
         n = boxes.shape[-1]
-        assert n in {6, 7}, f"expected 6 or 7 values but got {n}"  # xyxy, track_id, conf, cls
+        assert n in (6, 7), f"expected 6 or 7 values but got {n}"  # xyxy, track_id, conf, cls
         super().__init__(boxes, orig_shape)
         self.is_track = n == 7
         self.orig_shape = orig_shape
 
     @property
     def xyxy(self):
         """Return the boxes in xyxy format."""
@@ -666,15 +603,15 @@
         orig_shape (tuple): Original image size, in the format (height, width).
 
     Attributes:
         xywhr (torch.Tensor | numpy.ndarray): The boxes in [x_center, y_center, width, height, rotation] format.
         conf (torch.Tensor | numpy.ndarray): The confidence values of the boxes.
         cls (torch.Tensor | numpy.ndarray): The class values of the boxes.
         id (torch.Tensor | numpy.ndarray): The track IDs of the boxes (if available).
-        xyxyxyxyn (torch.Tensor | numpy.ndarray): The rotated boxes in xyxyxyxy format normalized by orig image size.
+        xyxyxyxyn (torch.Tensor | numpy.ndarray): The rotated boxes in xyxyxyxy format normalized by original image size.
         xyxyxyxy (torch.Tensor | numpy.ndarray): The rotated boxes in xyxyxyxy format.
         xyxy (torch.Tensor | numpy.ndarray): The horizontal boxes in xyxyxyxy format.
         data (torch.Tensor): The raw OBB tensor (alias for `boxes`).
 
     Methods:
         cpu(): Move the object to CPU memory.
         numpy(): Convert the object to a numpy array.
@@ -683,15 +620,15 @@
     """
 
     def __init__(self, boxes, orig_shape) -> None:
         """Initialize the Boxes class."""
         if boxes.ndim == 1:
             boxes = boxes[None, :]
         n = boxes.shape[-1]
-        assert n in {7, 8}, f"expected 7 or 8 values but got {n}"  # xywh, rotation, track_id, conf, cls
+        assert n in (7, 8), f"expected 7 or 8 values but got {n}"  # xywh, rotation, track_id, conf, cls
         super().__init__(boxes, orig_shape)
         self.is_track = n == 8
         self.orig_shape = orig_shape
 
     @property
     def xywhr(self):
         """Return the rotated boxes in xywhr format."""
@@ -720,15 +657,15 @@
 
     @property
     @lru_cache(maxsize=2)
     def xyxyxyxyn(self):
         """Return the boxes in xyxyxyxy format, (N, 4, 2)."""
         xyxyxyxyn = self.xyxyxyxy.clone() if isinstance(self.xyxyxyxy, torch.Tensor) else np.copy(self.xyxyxyxy)
         xyxyxyxyn[..., 0] /= self.orig_shape[1]
-        xyxyxyxyn[..., 1] /= self.orig_shape[0]
+        xyxyxyxyn[..., 1] /= self.orig_shape[1]
         return xyxyxyxyn
 
     @property
     @lru_cache(maxsize=2)
     def xyxy(self):
         """
         Return the horizontal boxes in xyxy format, (N, 4).
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/engine/trainer.py` & `pyppbox-ultralytics-8.1.7/ultralytics/engine/trainer.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 from ultralytics.utils.autobatch import check_train_batch_size
 from ultralytics.utils.checks import check_amp, check_file, check_imgsz, check_model_file_from_stem, print_args
 from ultralytics.utils.dist import ddp_cleanup, generate_ddp_command
 from ultralytics.utils.files import get_latest_run
 from ultralytics.utils.torch_utils import (
     EarlyStopping,
     ModelEMA,
-    convert_optimizer_state_dict_to_fp16,
+    de_parallel,
     init_seeds,
     one_cycle,
     select_device,
     strip_optimizer,
 )
 
 
@@ -103,34 +103,44 @@
         self.plots = {}
         init_seeds(self.args.seed + 1 + RANK, deterministic=self.args.deterministic)
 
         # Dirs
         self.save_dir = get_save_dir(self.args)
         self.args.name = self.save_dir.name  # update name for loggers
         self.wdir = self.save_dir / "weights"  # weights dir
-        if RANK in {-1, 0}:
+        if RANK in (-1, 0):
             self.wdir.mkdir(parents=True, exist_ok=True)  # make dir
             self.args.save_dir = str(self.save_dir)
             yaml_save(self.save_dir / "args.yaml", vars(self.args))  # save run args
         self.last, self.best = self.wdir / "last.pt", self.wdir / "best.pt"  # checkpoint paths
         self.save_period = self.args.save_period
 
         self.batch_size = self.args.batch
         self.epochs = self.args.epochs
         self.start_epoch = 0
         if RANK == -1:
             print_args(vars(self.args))
 
         # Device
-        if self.device.type in {"cpu", "mps"}:
+        if self.device.type in ("cpu", "mps"):
             self.args.workers = 0  # faster CPU training as time dominated by inference, not dataloading
 
         # Model and Dataset
         self.model = check_model_file_from_stem(self.args.model)  # add suffix, i.e. yolov8n -> yolov8n.pt
-        self.trainset, self.testset = self.get_dataset()
+        try:
+            if self.args.task == "classify":
+                self.data = check_cls_dataset(self.args.data)
+            elif self.args.data.split(".")[-1] in ("yaml", "yml") or self.args.task in ("detect", "segment", "pose"):
+                self.data = check_det_dataset(self.args.data)
+                if "yaml_file" in self.data:
+                    self.args.data = self.data["yaml_file"]  # for validating 'yolo train data=url.zip' usage
+        except Exception as e:
+            raise RuntimeError(emojis(f"Dataset '{clean_url(self.args.data)}' error ❌ {e}")) from e
+
+        self.trainset, self.testset = self.get_dataset(self.data)
         self.ema = None
 
         # Optimization utils init
         self.lf = None
         self.scheduler = None
 
         # Epoch level metrics
@@ -140,15 +150,15 @@
         self.tloss = None
         self.loss_names = ["Loss"]
         self.csv = self.save_dir / "results.csv"
         self.plot_idx = [0, 1, 2]
 
         # Callbacks
         self.callbacks = _callbacks or callbacks.get_default_callbacks()
-        if RANK in {-1, 0}:
+        if RANK in (-1, 0):
             callbacks.add_integration_callbacks(self)
 
     def add_callback(self, event: str, callback):
         """Appends the given callback."""
         self.callbacks[event].append(callback)
 
     def set_callback(self, event: str, callback):
@@ -206,17 +216,17 @@
         self.scheduler = optim.lr_scheduler.LambdaLR(self.optimizer, lr_lambda=self.lf)
 
     def _setup_ddp(self, world_size):
         """Initializes and sets the DistributedDataParallel parameters for training."""
         torch.cuda.set_device(RANK)
         self.device = torch.device("cuda", RANK)
         # LOGGER.info(f'DDP info: RANK {RANK}, WORLD_SIZE {world_size}, DEVICE {self.device}')
-        os.environ["TORCH_NCCL_BLOCKING_WAIT"] = "1"  # set to enforce timeout
+        os.environ["NCCL_BLOCKING_WAIT"] = "1"  # set to enforce timeout
         dist.init_process_group(
-            backend="nccl" if dist.is_nccl_available() else "gloo",
+            "nccl" if dist.is_nccl_available() else "gloo",
             timeout=timedelta(seconds=10800),  # 3 hours
             rank=RANK,
             world_size=world_size,
         )
 
     def _setup_train(self, world_size):
         """Builds dataloaders and optimizer on correct rank process."""
@@ -238,48 +248,48 @@
         always_freeze_names = [".dfl"]  # always freeze these layers
         freeze_layer_names = [f"model.{x}." for x in freeze_list] + always_freeze_names
         for k, v in self.model.named_parameters():
             # v.register_hook(lambda x: torch.nan_to_num(x))  # NaN to 0 (commented for erratic training results)
             if any(x in k for x in freeze_layer_names):
                 LOGGER.info(f"Freezing layer '{k}'")
                 v.requires_grad = False
-            elif not v.requires_grad and v.dtype.is_floating_point:  # only floating point Tensor can require gradients
+            elif not v.requires_grad:
                 LOGGER.info(
                     f"WARNING ⚠️ setting 'requires_grad=True' for frozen layer '{k}'. "
                     "See ultralytics.engine.trainer for customization of frozen layers."
                 )
                 v.requires_grad = True
 
         # Check AMP
         self.amp = torch.tensor(self.args.amp).to(self.device)  # True or False
-        if self.amp and RANK in {-1, 0}:  # Single-GPU and DDP
+        if self.amp and RANK in (-1, 0):  # Single-GPU and DDP
             callbacks_backup = callbacks.default_callbacks.copy()  # backup callbacks as check_amp() resets them
             self.amp = torch.tensor(check_amp(self.model), device=self.device)
             callbacks.default_callbacks = callbacks_backup  # restore callbacks
         if RANK > -1 and world_size > 1:  # DDP
             dist.broadcast(self.amp, src=0)  # broadcast the tensor from rank 0 to all other ranks (returns None)
         self.amp = bool(self.amp)  # as boolean
         self.scaler = torch.cuda.amp.GradScaler(enabled=self.amp)
         if world_size > 1:
             self.model = nn.parallel.DistributedDataParallel(self.model, device_ids=[RANK])
 
         # Check imgsz
         gs = max(int(self.model.stride.max() if hasattr(self.model, "stride") else 32), 32)  # grid size (max stride)
         self.args.imgsz = check_imgsz(self.args.imgsz, stride=gs, floor=gs, max_dim=1)
-        self.stride = gs  # for multiscale training
+        self.stride = gs  # for multi-scale training
 
         # Batch size
         if self.batch_size == -1 and RANK == -1:  # single-GPU only, estimate best batch size
             self.args.batch = self.batch_size = check_train_batch_size(self.model, self.args.imgsz, self.amp)
 
         # Dataloaders
         batch_size = self.batch_size // max(world_size, 1)
         self.train_loader = self.get_dataloader(self.trainset, batch_size=batch_size, rank=RANK, mode="train")
-        if RANK in {-1, 0}:
-            # Note: When training DOTA dataset, double batch size could get OOM on images with >2000 objects.
+        if RANK in (-1, 0):
+            # NOTE: When training DOTA dataset, double batch size could get OOM cause some images got more than 2000 objects.
             self.test_loader = self.get_dataloader(
                 self.testset, batch_size=batch_size if self.args.task == "obb" else batch_size * 2, rank=-1, mode="val"
             )
             self.validator = self.get_validator()
             metric_keys = self.validator.metrics.keys + self.label_loss_items(prefix="val")
             self.metrics = dict(zip(metric_keys, [0] * len(metric_keys)))
             self.ema = ModelEMA(self.model)
@@ -323,32 +333,28 @@
             f'Using {self.train_loader.num_workers * (world_size or 1)} dataloader workers\n'
             f"Logging results to {colorstr('bold', self.save_dir)}\n"
             f'Starting training for ' + (f"{self.args.time} hours..." if self.args.time else f"{self.epochs} epochs...")
         )
         if self.args.close_mosaic:
             base_idx = (self.epochs - self.args.close_mosaic) * nb
             self.plot_idx.extend([base_idx, base_idx + 1, base_idx + 2])
-        epoch = self.start_epoch
-        while True:
+        epoch = self.epochs  # predefine for resume fully trained model edge cases
+        for epoch in range(self.start_epoch, self.epochs):
             self.epoch = epoch
             self.run_callbacks("on_train_epoch_start")
-            with warnings.catch_warnings():
-                warnings.simplefilter("ignore")  # suppress 'Detected lr_scheduler.step() before optimizer.step()'
-                self.scheduler.step()
-
             self.model.train()
             if RANK != -1:
                 self.train_loader.sampler.set_epoch(epoch)
             pbar = enumerate(self.train_loader)
             # Update dataloader attributes (optional)
             if epoch == (self.epochs - self.args.close_mosaic):
                 self._close_dataloader_mosaic()
                 self.train_loader.reset()
 
-            if RANK in {-1, 0}:
+            if RANK in (-1, 0):
                 LOGGER.info(self.progress_string())
                 pbar = TQDM(enumerate(self.train_loader), total=nb)
             self.tloss = None
             self.optimizer.zero_grad()
             for i, batch in pbar:
                 self.run_callbacks("on_train_batch_start")
                 # Warmup
@@ -390,148 +396,129 @@
                             dist.broadcast_object_list(broadcast_list, 0)  # broadcast 'stop' to all ranks
                             self.stop = broadcast_list[0]
                         if self.stop:  # training time exceeded
                             break
 
                 # Log
                 mem = f"{torch.cuda.memory_reserved() / 1E9 if torch.cuda.is_available() else 0:.3g}G"  # (GB)
-                loss_len = self.tloss.shape[0] if len(self.tloss.shape) else 1
+                loss_len = self.tloss.shape[0] if len(self.tloss.size()) else 1
                 losses = self.tloss if loss_len > 1 else torch.unsqueeze(self.tloss, 0)
-                if RANK in {-1, 0}:
+                if RANK in (-1, 0):
                     pbar.set_description(
                         ("%11s" * 2 + "%11.4g" * (2 + loss_len))
                         % (f"{epoch + 1}/{self.epochs}", mem, *losses, batch["cls"].shape[0], batch["img"].shape[-1])
                     )
                     self.run_callbacks("on_batch_end")
                     if self.args.plots and ni in self.plot_idx:
                         self.plot_training_samples(batch, ni)
 
                 self.run_callbacks("on_train_batch_end")
 
             self.lr = {f"lr/pg{ir}": x["lr"] for ir, x in enumerate(self.optimizer.param_groups)}  # for loggers
             self.run_callbacks("on_train_epoch_end")
-            if RANK in {-1, 0}:
-                final_epoch = epoch + 1 >= self.epochs
+            if RANK in (-1, 0):
+                final_epoch = epoch + 1 == self.epochs
                 self.ema.update_attr(self.model, include=["yaml", "nc", "args", "names", "stride", "class_weights"])
 
                 # Validation
                 if self.args.val or final_epoch or self.stopper.possible_stop or self.stop:
                     self.metrics, self.fitness = self.validate()
                 self.save_metrics(metrics={**self.label_loss_items(self.tloss), **self.metrics, **self.lr})
-                self.stop |= self.stopper(epoch + 1, self.fitness) or final_epoch
+                self.stop |= self.stopper(epoch + 1, self.fitness)
                 if self.args.time:
                     self.stop |= (time.time() - self.train_time_start) > (self.args.time * 3600)
 
                 # Save model
                 if self.args.save or final_epoch:
                     self.save_model()
                     self.run_callbacks("on_model_save")
 
             # Scheduler
             t = time.time()
             self.epoch_time = t - self.epoch_time_start
             self.epoch_time_start = t
-            if self.args.time:
-                mean_epoch_time = (t - self.train_time_start) / (epoch - self.start_epoch + 1)
-                self.epochs = self.args.epochs = math.ceil(self.args.time * 3600 / mean_epoch_time)
-                self._setup_scheduler()
-                self.scheduler.last_epoch = self.epoch  # do not move
-                self.stop |= epoch >= self.epochs  # stop if exceeded epochs
+            with warnings.catch_warnings():
+                warnings.simplefilter("ignore")  # suppress 'Detected lr_scheduler.step() before optimizer.step()'
+                if self.args.time:
+                    mean_epoch_time = (t - self.train_time_start) / (epoch - self.start_epoch + 1)
+                    self.epochs = self.args.epochs = math.ceil(self.args.time * 3600 / mean_epoch_time)
+                    self._setup_scheduler()
+                    self.scheduler.last_epoch = self.epoch  # do not move
+                    self.stop |= epoch >= self.epochs  # stop if exceeded epochs
+                self.scheduler.step()
             self.run_callbacks("on_fit_epoch_end")
             torch.cuda.empty_cache()  # clear GPU memory at end of epoch, may help reduce CUDA out of memory errors
 
             # Early Stopping
             if RANK != -1:  # if DDP training
                 broadcast_list = [self.stop if RANK == 0 else None]
                 dist.broadcast_object_list(broadcast_list, 0)  # broadcast 'stop' to all ranks
                 self.stop = broadcast_list[0]
             if self.stop:
                 break  # must break all DDP ranks
-            epoch += 1
 
-        if RANK in {-1, 0}:
+        if RANK in (-1, 0):
             # Do final val with best.pt
             LOGGER.info(
                 f"\n{epoch - self.start_epoch + 1} epochs completed in "
                 f"{(time.time() - self.train_time_start) / 3600:.3f} hours."
             )
             self.final_eval()
             if self.args.plots:
                 self.plot_metrics()
             self.run_callbacks("on_train_end")
         torch.cuda.empty_cache()
         self.run_callbacks("teardown")
 
     def save_model(self):
         """Save model training checkpoints with additional metadata."""
-        import io
         import pandas as pd  # scope for faster startup
 
-        # Serialize ckpt to a byte buffer once (faster than repeated torch.save() calls)
-        buffer = io.BytesIO()
-        torch.save(
-            {
-                "epoch": self.epoch,
-                "best_fitness": self.best_fitness,
-                "model": None,  # resume and final checkpoints derive from EMA
-                "ema": deepcopy(self.ema.ema).half(),
-                "updates": self.ema.updates,
-                "optimizer": convert_optimizer_state_dict_to_fp16(deepcopy(self.optimizer.state_dict())),
-                "train_args": vars(self.args),  # save as dict
-                "train_metrics": {**self.metrics, **{"fitness": self.fitness}},
-                "train_results": {k.strip(): v for k, v in pd.read_csv(self.csv).to_dict(orient="list").items()},
-                "date": datetime.now().isoformat(),
-                "version": __version__,
-                "license": "AGPL-3.0 (https://ultralytics.com/license)",
-                "docs": "https://docs.ultralytics.com",
-            },
-            buffer,
-        )
-        serialized_ckpt = buffer.getvalue()  # get the serialized content to save
+        metrics = {**self.metrics, **{"fitness": self.fitness}}
+        results = {k.strip(): v for k, v in pd.read_csv(self.csv).to_dict(orient="list").items()}
+        ckpt = {
+            "epoch": self.epoch,
+            "best_fitness": self.best_fitness,
+            "model": deepcopy(de_parallel(self.model)).half(),
+            "ema": deepcopy(self.ema.ema).half(),
+            "updates": self.ema.updates,
+            "optimizer": self.optimizer.state_dict(),
+            "train_args": vars(self.args),  # save as dict
+            "train_metrics": metrics,
+            "train_results": results,
+            "date": datetime.now().isoformat(),
+            "version": __version__,
+        }
 
-        # Save checkpoints
-        self.last.write_bytes(serialized_ckpt)  # save last.pt
+        # Save last and best
+        torch.save(ckpt, self.last)
         if self.best_fitness == self.fitness:
-            self.best.write_bytes(serialized_ckpt)  # save best.pt
+            torch.save(ckpt, self.best)
         if (self.save_period > 0) and (self.epoch > 0) and (self.epoch % self.save_period == 0):
-            (self.wdir / f"epoch{self.epoch}.pt").write_bytes(serialized_ckpt)  # save epoch, i.e. 'epoch3.pt'
+            torch.save(ckpt, self.wdir / f"epoch{self.epoch}.pt")
 
-    def get_dataset(self):
+    @staticmethod
+    def get_dataset(data):
         """
         Get train, val path from data dict if it exists.
 
         Returns None if data format is not recognized.
         """
-        try:
-            if self.args.task == "classify":
-                data = check_cls_dataset(self.args.data)
-            elif self.args.data.split(".")[-1] in {"yaml", "yml"} or self.args.task in {
-                "detect",
-                "segment",
-                "pose",
-                "obb",
-            }:
-                data = check_det_dataset(self.args.data)
-                if "yaml_file" in data:
-                    self.args.data = data["yaml_file"]  # for validating 'yolo train data=url.zip' usage
-        except Exception as e:
-            raise RuntimeError(emojis(f"Dataset '{clean_url(self.args.data)}' error ❌ {e}")) from e
-        self.data = data
         return data["train"], data.get("val") or data.get("test")
 
     def setup_model(self):
         """Load/create/download model for any task."""
         if isinstance(self.model, torch.nn.Module):  # if model is loaded beforehand. No setup needed
             return
 
         model, weights = self.model, None
         ckpt = None
         if str(model).endswith(".pt"):
             weights, ckpt = attempt_load_one_weight(model)
-            cfg = weights.yaml
+            cfg = ckpt["model"].yaml
         else:
             cfg = model
         self.model = self.get_model(cfg=cfg, weights=weights, verbose=RANK == -1)  # calls Model(cfg, weights)
         return ckpt
 
     def optimizer_step(self):
         """Perform a single step of the training optimizer with gradient clipping and EMA update."""
@@ -645,43 +632,46 @@
                 # Check that resume data YAML exists, otherwise strip to force re-download of dataset
                 ckpt_args = attempt_load_weights(last).args
                 if not Path(ckpt_args["data"]).exists():
                     ckpt_args["data"] = self.args.data
 
                 resume = True
                 self.args = get_cfg(ckpt_args)
-                self.args.model = self.args.resume = str(last)  # reinstate model
-                for k in "imgsz", "batch", "device":  # allow arg updates to reduce memory or update device on resume
+                self.args.model = str(last)  # reinstate model
+                for k in "imgsz", "batch":  # allow arg updates to reduce memory on resume if crashed due to CUDA OOM
                     if k in overrides:
                         setattr(self.args, k, overrides[k])
 
             except Exception as e:
                 raise FileNotFoundError(
                     "Resume checkpoint not found. Please pass a valid checkpoint to resume from, "
                     "i.e. 'yolo train resume model=path/to/last.pt'"
                 ) from e
         self.resume = resume
 
     def resume_training(self, ckpt):
         """Resume YOLO training from given epoch and best fitness."""
-        if ckpt is None or not self.resume:
+        if ckpt is None:
             return
         best_fitness = 0.0
-        start_epoch = ckpt.get("epoch", -1) + 1
-        if ckpt.get("optimizer", None) is not None:
+        start_epoch = ckpt["epoch"] + 1
+        if ckpt["optimizer"] is not None:
             self.optimizer.load_state_dict(ckpt["optimizer"])  # optimizer
             best_fitness = ckpt["best_fitness"]
         if self.ema and ckpt.get("ema"):
             self.ema.ema.load_state_dict(ckpt["ema"].float().state_dict())  # EMA
             self.ema.updates = ckpt["updates"]
-        assert start_epoch > 0, (
-            f"{self.args.model} training to {self.epochs} epochs is finished, nothing to resume.\n"
-            f"Start a new training without resuming, i.e. 'yolo train model={self.args.model}'"
-        )
-        LOGGER.info(f"Resuming training {self.args.model} from epoch {start_epoch + 1} to {self.epochs} total epochs")
+        if self.resume:
+            assert start_epoch > 0, (
+                f"{self.args.model} training to {self.epochs} epochs is finished, nothing to resume.\n"
+                f"Start a new training without resuming, i.e. 'yolo train model={self.args.model}'"
+            )
+            LOGGER.info(
+                f"Resuming training from {self.args.model} from epoch {start_epoch + 1} to {self.epochs} total epochs"
+            )
         if self.epochs < start_epoch:
             LOGGER.info(
                 f"{self.model} has been trained for {ckpt['epoch']} epochs. Fine-tuning for {self.epochs} more epochs."
             )
             self.epochs += ckpt["epoch"]  # finetune additional epochs
         self.best_fitness = best_fitness
         self.start_epoch = start_epoch
@@ -734,15 +724,15 @@
                 if "bias" in fullname:  # bias (no decay)
                     g[2].append(param)
                 elif isinstance(module, bn):  # weight (no decay)
                     g[1].append(param)
                 else:  # weight (with decay)
                     g[0].append(param)
 
-        if name in {"Adam", "Adamax", "AdamW", "NAdam", "RAdam"}:
+        if name in ("Adam", "Adamax", "AdamW", "NAdam", "RAdam"):
             optimizer = getattr(optim, name, optim.Adam)(g[2], lr=lr, betas=(momentum, 0.999), weight_decay=0.0)
         elif name == "RMSProp":
             optimizer = optim.RMSprop(g[2], lr=lr, momentum=momentum)
         elif name == "SGD":
             optimizer = optim.SGD(g[2], lr=lr, momentum=momentum, nesterov=True)
         else:
             raise NotImplementedError(
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/engine/tuner.py` & `pyppbox-ultralytics-8.1.7/ultralytics/engine/tuner.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
     ```python
     from ultralytics import YOLO
 
     model = YOLO('yolov8n.pt')
     model.tune(data='coco8.yaml', epochs=10, iterations=300, optimizer='AdamW', plots=False, save=False, val=False)
     ```
 """
-
 import random
 import shutil
 import subprocess
 import time
 
 import numpy as np
 import torch
@@ -91,15 +90,14 @@
             "degrees": (0.0, 45.0),  # image rotation (+/- deg)
             "translate": (0.0, 0.9),  # image translation (+/- fraction)
             "scale": (0.0, 0.95),  # image scale (+/- gain)
             "shear": (0.0, 10.0),  # image shear (+/- deg)
             "perspective": (0.0, 0.001),  # image perspective (+/- fraction), range 0-0.001
             "flipud": (0.0, 1.0),  # image flip up-down (probability)
             "fliplr": (0.0, 1.0),  # image flip left-right (probability)
-            "bgr": (0.0, 1.0),  # image channel bgr (probability)
             "mosaic": (0.0, 1.0),  # image mixup (probability)
             "mixup": (0.0, 1.0),  # image mixup (probability)
             "copy_paste": (0.0, 1.0),  # segment copy-paste (probability)
         }
         self.args = get_cfg(overrides=args)
         self.tune_dir = get_save_dir(self.args, name="tune")
         self.tune_csv = self.tune_dir / "tune_results.csv"
@@ -185,19 +183,19 @@
             mutated_hyp = self._mutate()
             LOGGER.info(f"{self.prefix}Starting iteration {i + 1}/{iterations} with hyperparameters: {mutated_hyp}")
 
             metrics = {}
             train_args = {**vars(self.args), **mutated_hyp}
             save_dir = get_save_dir(get_cfg(train_args))
             weights_dir = save_dir / "weights"
+            ckpt_file = weights_dir / ("best.pt" if (weights_dir / "best.pt").exists() else "last.pt")
             try:
                 # Train YOLO model with mutated hyperparameters (run in subprocess to avoid dataloader hang)
                 cmd = ["yolo", "train", *(f"{k}={v}" for k, v in train_args.items())]
                 return_code = subprocess.run(cmd, check=True).returncode
-                ckpt_file = weights_dir / ("best.pt" if (weights_dir / "best.pt").exists() else "last.pt")
                 metrics = torch.load(ckpt_file)["train_metrics"]
                 assert return_code == 0, "training failed"
 
             except Exception as e:
                 LOGGER.warning(f"WARNING ❌️ training failure for hyperparameter tuning iteration {i + 1}\n{e}")
 
             # Save results and mutated_hyp to CSV
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/engine/validator.py` & `pyppbox-ultralytics-8.1.7/ultralytics/engine/validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,17 +13,15 @@
                           yolov8n.engine             # TensorRT
                           yolov8n.mlpackage          # CoreML (macOS-only)
                           yolov8n_saved_model        # TensorFlow SavedModel
                           yolov8n.pb                 # TensorFlow GraphDef
                           yolov8n.tflite             # TensorFlow Lite
                           yolov8n_edgetpu.tflite     # TensorFlow Edge TPU
                           yolov8n_paddle_model       # PaddlePaddle
-                          yolov8n_ncnn_model         # NCNN
 """
-
 import json
 import time
 from pathlib import Path
 
 import numpy as np
 import torch
 
@@ -118,15 +116,15 @@
             # self.model = model
             self.loss = torch.zeros_like(trainer.loss_items, device=trainer.device)
             self.args.plots &= trainer.stopper.possible_stop or (trainer.epoch == trainer.epochs - 1)
             model.eval()
         else:
             callbacks.add_integration_callbacks(self)
             model = AutoBackend(
-                weights=model or self.args.model,
+                model or self.args.model,
                 device=select_device(self.args.device, self.args.batch),
                 dnn=self.args.dnn,
                 data=self.args.data,
                 fp16=self.args.half,
             )
             # self.model = model
             self.device = model.device  # update device
@@ -135,22 +133,22 @@
             imgsz = check_imgsz(self.args.imgsz, stride=stride)
             if engine:
                 self.args.batch = model.batch_size
             elif not pt and not jit:
                 self.args.batch = 1  # export.py models default to batch-size 1
                 LOGGER.info(f"Forcing batch=1 square inference (1,3,{imgsz},{imgsz}) for non-PyTorch models")
 
-            if str(self.args.data).split(".")[-1] in {"yaml", "yml"}:
+            if str(self.args.data).split(".")[-1] in ("yaml", "yml"):
                 self.data = check_det_dataset(self.args.data)
             elif self.args.task == "classify":
                 self.data = check_cls_dataset(self.args.data, split=self.args.split)
             else:
                 raise FileNotFoundError(emojis(f"Dataset '{self.args.data}' for task={self.args.task} not found ❌"))
 
-            if self.device.type in {"cpu", "mps"}:
+            if self.device.type in ("cpu", "mps"):
                 self.args.workers = 0  # faster CPU val as time dominated by inference, not dataloading
             if not pt:
                 self.args.rect = False
             self.stride = model.stride  # used in get_dataloader() for padding
             self.dataloader = self.dataloader or self.get_dataloader(self.data.get(self.args.split), self.args.batch)
 
             model.eval()
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/hub/__init__.py` & `pyppbox-ultralytics-8.1.7/ultralytics/hub/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         api_key (str, optional): API key to use for authentication.
             If not provided, it will be retrieved from SETTINGS or HUB_API_KEY environment variable.
         save (bool, optional): Whether to save the API key to SETTINGS if authentication is successful.
 
     Returns:
         (bool): True if authentication is successful, False otherwise.
     """
-    checks.check_requirements("hub-sdk>=0.0.6")
+    checks.check_requirements("hub-sdk>=0.0.2")
     from hub_sdk import HUBClient
 
     api_key_url = f"{HUB_WEB_ROOT}/settings?tab=api+keys"  # set the redirect URL
     saved_key = SETTINGS.get("api_key")
     active_key = api_key or saved_key
     credentials = {"api_key": active_key} if active_key and active_key != "" else None  # set credentials
 
@@ -44,15 +44,15 @@
             "New authentication successful ✅" if client.api_key == api_key or not credentials else "Authenticated ✅"
         )
         LOGGER.info(f"{PREFIX}{log_message}")
 
         return True
     else:
         # Failed to authenticate with HUB
-        LOGGER.info(f"{PREFIX}Get API key from {api_key_url} and then run 'yolo hub login API_KEY'")
+        LOGGER.info(f"{PREFIX}Retrieve API key from {api_key_url}")
         return False
 
 
 def logout():
     """
     Log out of Ultralytics HUB by removing the API key from the settings file. To log in again, use 'yolo hub login'.
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/hub/auth.py` & `pyppbox-ultralytics-8.1.7/ultralytics/hub/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         # Update SETTINGS with the new API key after successful authentication
         if success:
             SETTINGS.update({"api_key": self.api_key})
             # Log that the new login was successful
             if verbose:
                 LOGGER.info(f"{PREFIX}New authentication successful ✅")
         elif verbose:
-            LOGGER.info(f"{PREFIX}Get API key from {API_KEY_URL} and then run 'yolo hub login API_KEY'")
+            LOGGER.info(f"{PREFIX}Retrieve API key from {API_KEY_URL}")
 
     def request_api_key(self, max_attempts=3):
         """
         Prompt the user to input their API key.
 
         Returns the model ID.
         """
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/hub/session.py` & `pyppbox-ultralytics-8.1.7/ultralytics/hub/session.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,14 @@
 
         self.rate_limits = {
             "metrics": 3.0,
             "ckpt": 900.0,
             "heartbeat": 300.0,
         }  # rate limits (seconds)
         self.metrics_queue = {}  # holds metrics for each epoch until upload
-        self.metrics_upload_failed_queue = {}  # holds metrics for each epoch if upload failed
         self.timers = {}  # holds timers in ultralytics/utils/callbacks/hub.py
 
         # Parse input
         api_key, model_id, self.filename = self._parse_identifier(identifier)
 
         # Get credentials
         active_key = api_key or SETTINGS.get("api_key")
@@ -166,45 +165,46 @@
                 raise HUBModelError(
                     f"model='{identifier}' could not be parsed. Check format is correct. "
                     f"Supported formats are Ultralytics HUB URL, apiKey_modelId, modelId, local pt or yaml file."
                 )
 
         return api_key, model_id, filename
 
-    def _set_train_args(self):
-        """
-        Initializes training arguments and creates a model entry on the Ultralytics HUB.
-
-        This method sets up training arguments based on the model's state and updates them with any additional
-        arguments provided. It handles different states of the model, such as whether it's resumable, pretrained,
-        or requires specific file setup.
-
-        Raises:
-            ValueError: If the model is already trained, if required dataset information is missing, or if there are
-                issues with the provided training arguments.
-        """
+    def _set_train_args(self, **kwargs):
+        """Initializes training arguments and creates a model entry on the Ultralytics HUB."""
         if self.model.is_trained():
+            # Model is already trained
             raise ValueError(emojis(f"Model is already trained and uploaded to {self.model_url} 🚀"))
 
         if self.model.is_resumable():
             # Model has saved weights
             self.train_args = {"data": self.model.get_dataset_url(), "resume": True}
             self.model_file = self.model.get_weights_url("last")
         else:
             # Model has no saved weights
-            self.train_args = self.model.data.get("train_args")  # new response
+            def get_train_args(config):
+                """Parses an identifier to extract API key, model ID, and filename if applicable."""
+                return {
+                    "batch": config["batchSize"],
+                    "epochs": config["epochs"],
+                    "imgsz": config["imageSize"],
+                    "patience": config["patience"],
+                    "device": config["device"],
+                    "cache": config["cache"],
+                    "data": self.model.get_dataset_url(),
+                }
 
+            self.train_args = get_train_args(self.model.data.get("config"))
             # Set the model file as either a *.pt or *.yaml file
             self.model_file = (
                 self.model.get_weights_url("parent") if self.model.is_pretrained() else self.model.get_architecture()
             )
 
-        if "data" not in self.train_args:
-            # RF bug - datasets are sometimes not exported
-            raise ValueError("Dataset may still be processing. Please wait a minute and try again.")
+        if not self.train_args.get("data"):
+            raise ValueError("Dataset may still be processing. Please wait a minute and try again.")  # RF fix
 
         self.model_file = checks.check_yolov5u_filename(self.model_file, verbose=False)  # YOLOv5->YOLOv5u
         self.model_id = self.model.id
 
     def request_queue(
         self,
         request_func,
@@ -230,17 +230,14 @@
                     time.sleep(2**i)  # Exponential backoff before retrying
                     continue  # Skip further processing and retry
 
                 if progress_total:
                     self._show_upload_progress(progress_total, response)
 
                 if HTTPStatus.OK <= response.status_code < HTTPStatus.MULTIPLE_CHOICES:
-                    # if request related to metrics upload
-                    if kwargs.get("metrics"):
-                        self.metrics_upload_failed_queue = {}
                     return response  # Success, no need to retry
 
                 if i == 0:
                     # Initial attempt, check status code and provide messages
                     message = self._get_failure_message(response, retry, timeout)
 
                     if verbose:
@@ -248,18 +245,14 @@
 
                 if not self._should_retry(response.status_code):
                     LOGGER.warning(f"{PREFIX}Request failed. {HELP_MSG} ({response.status_code}")
                     break  # Not an error that should be retried, exit loop
 
                 time.sleep(2**i)  # Exponential backoff for retries
 
-            # if request related to metrics upload and exceed retries
-            if response is None and kwargs.get("metrics"):
-                self.metrics_upload_failed_queue.update(kwargs.get("metrics", None))
-
             return response
 
         if thread:
             # Start a new thread to run the retry_request function
             threading.Thread(target=retry_request, daemon=True).start()
         else:
             # If running in the main thread, call retry_request directly
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/hub/utils.py` & `pyppbox-ultralytics-8.1.7/ultralytics/hub/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # Ultralytics YOLO 🚀, AGPL-3.0 license
 
 import os
 import platform
 import random
+import sys
 import threading
 import time
 from pathlib import Path
 
 import requests
 
 from ultralytics.utils import (
-    ARGV,
     ENVIRONMENT,
     LOGGER,
     ONLINE,
     RANK,
     SETTINGS,
     TESTS_RUNNING,
     TQDM,
@@ -80,15 +80,15 @@
 def requests_with_progress(method, url, **kwargs):
     """
     Make an HTTP request using the specified method and URL, with an optional progress bar.
 
     Args:
         method (str): The HTTP method to use (e.g. 'GET', 'POST').
         url (str): The URL to send the request to.
-        **kwargs (any): Additional keyword arguments to pass to the underlying `requests.request` function.
+        **kwargs (dict): Additional keyword arguments to pass to the underlying `requests.request` function.
 
     Returns:
         (requests.Response): The response object from the HTTP request.
 
     Note:
         - If 'progress' is set to True, the progress bar will display the download progress for responses with a known
         content length.
@@ -118,15 +118,15 @@
         url (str): The URL to make the request to.
         retry (int, optional): Number of retries to attempt before giving up. Default is 3.
         timeout (int, optional): Timeout in seconds after which the function will give up retrying. Default is 30.
         thread (bool, optional): Whether to execute the request in a separate daemon thread. Default is True.
         code (int, optional): An identifier for the request, used for logging purposes. Default is -1.
         verbose (bool, optional): A flag to determine whether to print out to console or not. Default is True.
         progress (bool, optional): Whether to show a progress bar during the request. Default is False.
-        **kwargs (any): Keyword arguments to be passed to the requests function specified in method.
+        **kwargs (dict): Keyword arguments to be passed to the requests function specified in method.
 
     Returns:
         (requests.Response): The HTTP response object. If the request is executed in a separate thread, returns None.
     """
     retry_codes = (408, 500)  # retry only these codes
 
     @TryExcept(verbose=verbose)
@@ -184,25 +184,25 @@
 
     def __init__(self):
         """Initializes the Events object with default values for events, rate_limit, and metadata."""
         self.events = []  # events list
         self.rate_limit = 60.0  # rate limit (seconds)
         self.t = 0.0  # rate limit timer (seconds)
         self.metadata = {
-            "cli": Path(ARGV[0]).name == "yolo",
+            "cli": Path(sys.argv[0]).name == "yolo",
             "install": "git" if is_git_dir() else "pip" if is_pip_package() else "other",
             "python": ".".join(platform.python_version_tuple()[:2]),  # i.e. 3.10
             "version": __version__,
             "env": ENVIRONMENT,
             "session_id": round(random.random() * 1e15),
             "engagement_time_msec": 1000,
         }
         self.enabled = (
             SETTINGS["sync"]
-            and RANK in {-1, 0}
+            and RANK in (-1, 0)
             and not TESTS_RUNNING
             and ONLINE
             and (is_pip_package() or get_git_origin_url() == "https://github.com/ultralytics/ultralytics.git")
         )
 
     def __call__(self, cfg):
         """
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/models/fastsam/model.py` & `pyppbox-ultralytics-8.1.7/ultralytics/models/fastsam/model.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,14 +20,14 @@
         ```
     """
 
     def __init__(self, model="FastSAM-x.pt"):
         """Call the __init__ method of the parent class (YOLO) with the updated default model."""
         if str(model) == "FastSAM.pt":
             model = "FastSAM-x.pt"
-        assert Path(model).suffix not in {".yaml", ".yml"}, "FastSAM models only support pre-trained models."
+        assert Path(model).suffix not in (".yaml", ".yml"), "FastSAM models only support pre-trained models."
         super().__init__(model=model, task="segment")
 
     @property
     def task_map(self):
         """Returns a dictionary mapping segment task to corresponding predictor and validator classes."""
         return {"segment": {"predictor": FastSAMPredictor, "validator": FastSAMValidator}}
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/models/fastsam/predict.py` & `pyppbox-ultralytics-8.1.7/ultralytics/models/fastsam/predict.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/models/fastsam/prompt.py` & `pyppbox-ultralytics-8.1.7/ultralytics/models/fastsam/prompt.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import cv2
 import matplotlib.pyplot as plt
 import numpy as np
 import torch
 from PIL import Image
 
-from ultralytics.utils import TQDM, checks
+from ultralytics.utils import TQDM
 
 
 class FastSAMPrompt:
     """
     Fast Segment Anything Model class for image annotation and visualization.
 
     Attributes:
@@ -27,17 +27,19 @@
         """Initializes FastSAMPrompt with given source, results and device, and assigns clip for linear assignment."""
         self.device = device
         self.results = results
         self.source = source
 
         # Import and assign clip
         try:
-            import clip
+            import clip  # for linear_assignment
         except ImportError:
-            checks.check_requirements("git+https://github.com/ultralytics/CLIP.git")
+            from ultralytics.utils.checks import check_requirements
+
+            check_requirements("git+https://github.com/openai/CLIP.git")
             import clip
         self.clip = clip
 
     @staticmethod
     def _segment_image(image, bbox):
         """Segments the given image according to the provided bounding box coordinates."""
         image_array = np.array(image)
@@ -109,16 +111,15 @@
         Args:
             annotations (list): Annotations to be plotted.
             output (str or Path): Output directory for saving the plots.
             bbox (list, optional): Bounding box coordinates [x1, y1, x2, y2]. Defaults to None.
             points (list, optional): Points to be plotted. Defaults to None.
             point_label (list, optional): Labels for the points. Defaults to None.
             mask_random_color (bool, optional): Whether to use random color for masks. Defaults to True.
-            better_quality (bool, optional): Whether to apply morphological transformations for better mask quality.
-                Defaults to True.
+            better_quality (bool, optional): Whether to apply morphological transformations for better mask quality. Defaults to True.
             retina (bool, optional): Whether to use retina mask. Defaults to False.
             with_contours (bool, optional): Whether to plot contours. Defaults to True.
         """
         pbar = TQDM(annotations, total=len(annotations))
         for ann in pbar:
             result_name = os.path.basename(ann.path)
             image = ann.orig_img[..., ::-1]  # BGR to RGB
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/models/fastsam/utils.py` & `pyppbox-ultralytics-8.1.7/ultralytics/models/fastsam/utils.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/models/fastsam/val.py` & `pyppbox-ultralytics-8.1.7/ultralytics/models/fastsam/val.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/models/nas/model.py` & `pyppbox-ultralytics-8.1.7/ultralytics/models/nas/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
     Note:
         YOLO-NAS models only support pre-trained models. Do not provide YAML configuration files.
     """
 
     def __init__(self, model="yolo_nas_s.pt") -> None:
         """Initializes the NAS model with the provided or default 'yolo_nas_s.pt' model."""
-        assert Path(model).suffix not in {".yaml", ".yml"}, "YOLO-NAS models only support pre-trained models."
+        assert Path(model).suffix not in (".yaml", ".yml"), "YOLO-NAS models only support pre-trained models."
         super().__init__(model, task="detect")
 
     @smart_inference_mode()
     def _load(self, weights: str, task: str):
         """Loads an existing NAS model weights or creates a new NAS model with pretrained weights if not provided."""
         import super_gradients
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/models/nas/predict.py` & `pyppbox-ultralytics-8.1.7/ultralytics/models/nas/predict.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/models/nas/val.py` & `pyppbox-ultralytics-8.1.7/ultralytics/models/nas/val.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/models/rtdetr/model.py` & `pyppbox-ultralytics-8.1.7/ultralytics/models/rtdetr/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,16 @@
 
         Args:
             model (str): Path to the pre-trained model. Defaults to 'rtdetr-l.pt'.
 
         Raises:
             NotImplementedError: If the model file extension is not 'pt', 'yaml', or 'yml'.
         """
+        if model and model.split(".")[-1] not in ("pt", "yaml", "yml"):
+            raise NotImplementedError("RT-DETR only supports creating from *.pt, *.yaml, or *.yml files.")
         super().__init__(model=model, task="detect")
 
     @property
     def task_map(self) -> dict:
         """
         Returns a task map for RT-DETR, associating tasks with corresponding Ultralytics classes.
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/models/rtdetr/predict.py` & `pyppbox-ultralytics-8.1.7/ultralytics/models/rtdetr/predict.py`

 * *Files 13% similar despite different names*

```diff
@@ -34,25 +34,22 @@
     def postprocess(self, preds, img, orig_imgs):
         """
         Postprocess the raw predictions from the model to generate bounding boxes and confidence scores.
 
         The method filters detections based on confidence and class if specified in `self.args`.
 
         Args:
-            preds (list): List of [predictions, extra] from the model.
+            preds (torch.Tensor): Raw predictions from the model.
             img (torch.Tensor): Processed input images.
             orig_imgs (list or torch.Tensor): Original, unprocessed images.
 
         Returns:
             (list[Results]): A list of Results objects containing the post-processed bounding boxes, confidence scores,
                 and class labels.
         """
-        if not isinstance(preds, (list, tuple)):  # list for PyTorch inference but list[0] Tensor for export inference
-            preds = [preds, None]
-
         nd = preds[0].shape[-1]
         bboxes, scores = preds[0].split((4, nd - 4), dim=-1)
 
         if not isinstance(orig_imgs, list):  # input images are a torch.Tensor, not a list
             orig_imgs = ops.convert_torch2numpy_batch(orig_imgs)
 
         results = []
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/models/rtdetr/train.py` & `pyppbox-ultralytics-8.1.7/ultralytics/models/rtdetr/train.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/models/rtdetr/val.py` & `pyppbox-ultralytics-8.1.7/ultralytics/models/rtdetr/val.py`

 * *Files 3% similar despite different names*

```diff
@@ -90,17 +90,14 @@
             cache=self.args.cache or None,
             prefix=colorstr(f"{mode}: "),
             data=self.data,
         )
 
     def postprocess(self, preds):
         """Apply Non-maximum suppression to prediction outputs."""
-        if not isinstance(preds, (list, tuple)):  # list for PyTorch inference but list[0] Tensor for export inference
-            preds = [preds, None]
-
         bs, _, nd = preds[0].shape
         bboxes, scores = preds[0].split((4, nd - 4), dim=-1)
         bboxes *= self.args.imgsz
         outputs = [torch.zeros((0, 6), device=bboxes.device)] * bs
         for i, bbox in enumerate(bboxes):  # (300, 4)
             bbox = ops.xywh2xyxy(bbox)
             score, cls = scores[i].max(-1)  # (300, )
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/models/sam/amg.py` & `pyppbox-ultralytics-8.1.7/ultralytics/models/sam/amg.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/models/sam/build.py` & `pyppbox-ultralytics-8.1.7/ultralytics/models/sam/build.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/models/sam/model.py` & `pyppbox-ultralytics-8.1.7/ultralytics/models/sam/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
         Args:
             model (str): Path to the pre-trained SAM model file. File should have a .pt or .pth extension.
 
         Raises:
             NotImplementedError: If the model file extension is not .pt or .pth.
         """
-        if model and Path(model).suffix not in {".pt", ".pth"}:
+        if model and Path(model).suffix not in (".pt", ".pth"):
             raise NotImplementedError("SAM prediction requires pre-trained *.pt or *.pth model.")
         super().__init__(model=model, task="segment")
 
     def _load(self, weights: str, task=None):
         """
         Loads the specified weights into the SAM model.
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/models/sam/modules/decoders.py` & `pyppbox-ultralytics-8.1.7/ultralytics/models/sam/modules/decoders.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,15 +117,15 @@
         """
         Predicts masks.
 
         See 'forward' for more details.
         """
         # Concatenate output tokens
         output_tokens = torch.cat([self.iou_token.weight, self.mask_tokens.weight], dim=0)
-        output_tokens = output_tokens.unsqueeze(0).expand(sparse_prompt_embeddings.shape[0], -1, -1)
+        output_tokens = output_tokens.unsqueeze(0).expand(sparse_prompt_embeddings.size(0), -1, -1)
         tokens = torch.cat((output_tokens, sparse_prompt_embeddings), dim=1)
 
         # Expand per-image data in batch direction to be per-mask
         src = torch.repeat_interleave(image_embeddings, tokens.shape[0], dim=0)
         src = src + dense_prompt_embeddings
         pos_src = torch.repeat_interleave(image_pe, tokens.shape[0], dim=0)
         b, c, h, w = src.shape
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/models/sam/modules/encoders.py` & `pyppbox-ultralytics-8.1.7/ultralytics/models/sam/modules/encoders.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/models/sam/modules/sam.py` & `pyppbox-ultralytics-8.1.7/ultralytics/models/sam/modules/sam.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/models/sam/modules/tiny_encoder.py` & `pyppbox-ultralytics-8.1.7/ultralytics/models/sam/modules/tiny_encoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
         super().__init__()
 
         self.input_resolution = input_resolution
         self.dim = dim
         self.out_dim = out_dim
         self.act = activation()
         self.conv1 = Conv2d_BN(dim, out_dim, 1, 1, 0)
-        stride_c = 1 if out_dim in {320, 448, 576} else 2
+        stride_c = 1 if out_dim in [320, 448, 576] else 2
         self.conv2 = Conv2d_BN(out_dim, out_dim, 3, stride_c, 1, groups=out_dim)
         self.conv3 = Conv2d_BN(out_dim, out_dim, 1, 1, 0)
 
     def forward(self, x):
         """Applies forward pass on the input utilizing convolution and activation layers, and returns the result."""
         if x.ndim == 3:
             H, W = self.input_resolution
@@ -728,15 +728,15 @@
 
         x = self.layers[0](x)
         start_i = 1
 
         for i in range(start_i, len(self.layers)):
             layer = self.layers[i]
             x = layer(x)
-        B, _, C = x.shape
+        B, _, C = x.size()
         x = x.view(B, 64, 64, C)
         x = x.permute(0, 3, 1, 2)
         return self.neck(x)
 
     def forward(self, x):
         """Executes a forward pass on the input tensor through the constructed model layers."""
         return self.forward_features(x)
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/models/sam/modules/transformer.py` & `pyppbox-ultralytics-8.1.7/ultralytics/models/sam/modules/transformer.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/models/sam/predict.py` & `pyppbox-ultralytics-8.1.7/ultralytics/models/sam/predict.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/models/utils/loss.py` & `pyppbox-ultralytics-8.1.7/ultralytics/models/utils/loss.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/models/utils/ops.py` & `pyppbox-ultralytics-8.1.7/ultralytics/models/utils/ops.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/models/yolo/classify/predict.py` & `pyppbox-ultralytics-8.1.7/ultralytics/models/yolo/classify/predict.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/models/yolo/classify/train.py` & `pyppbox-ultralytics-8.1.7/ultralytics/models/yolo/classify/train.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,20 +64,20 @@
 
         model, ckpt = str(self.model), None
         # Load a YOLO model locally, from torchvision, or from Ultralytics assets
         if model.endswith(".pt"):
             self.model, ckpt = attempt_load_one_weight(model, device="cpu")
             for p in self.model.parameters():
                 p.requires_grad = True  # for training
-        elif model.split(".")[-1] in {"yaml", "yml"}:
+        elif model.split(".")[-1] in ("yaml", "yml"):
             self.model = self.get_model(cfg=model)
         elif model in torchvision.models.__dict__:
             self.model = torchvision.models.__dict__[model](weights="IMAGENET1K_V1" if self.args.pretrained else None)
         else:
-            raise FileNotFoundError(f"ERROR: model={model} not found locally or online. Please check model name.")
+            FileNotFoundError(f"ERROR: model={model} not found locally or online. Please check model name.")
         ClassificationModel.reshape_outputs(self.model, self.data["nc"])
 
         return ckpt
 
     def build_dataset(self, img_path, mode="train", batch=None):
         """Creates a ClassificationDataset instance given an image path, and mode (train/test etc.)."""
         return ClassificationDataset(root=img_path, args=self.args, augment=mode == "train", prefix=mode)
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/models/yolo/classify/val.py` & `pyppbox-ultralytics-8.1.7/ultralytics/models/yolo/classify/val.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/models/yolo/detect/predict.py` & `pyppbox-ultralytics-8.1.7/ultralytics/models/yolo/detect/predict.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/models/yolo/detect/train.py` & `pyppbox-ultralytics-8.1.7/ultralytics/models/yolo/detect/train.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
             batch (int, optional): Size of batches, this is for `rect`. Defaults to None.
         """
         gs = max(int(de_parallel(self.model).stride.max() if self.model else 0), 32)
         return build_yolo_dataset(self.args, img_path, batch, self.data, mode=mode, rect=mode == "val", stride=gs)
 
     def get_dataloader(self, dataset_path, batch_size=16, rank=0, mode="train"):
         """Construct and return dataloader."""
-        assert mode in {"train", "val"}, f"Mode must be 'train' or 'val', not {mode}."
+        assert mode in ["train", "val"]
         with torch_distributed_zero_first(rank):  # init dataset *.cache only once if DDP
             dataset = self.build_dataset(dataset_path, mode, batch_size)
         shuffle = mode == "train"
         if getattr(dataset, "rect", False) and shuffle:
             LOGGER.warning("WARNING ⚠️ 'rect=True' is incompatible with DataLoader shuffle, setting shuffle=False")
             shuffle = False
         workers = self.args.workers if mode == "train" else self.args.workers * 2
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/models/yolo/detect/val.py` & `pyppbox-ultralytics-8.1.7/ultralytics/models/yolo/detect/val.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,19 +29,18 @@
     """
 
     def __init__(self, dataloader=None, save_dir=None, pbar=None, args=None, _callbacks=None):
         """Initialize detection model with necessary variables and settings."""
         super().__init__(dataloader, save_dir, pbar, args, _callbacks)
         self.nt_per_class = None
         self.is_coco = False
-        self.is_lvis = False
         self.class_map = None
         self.args.task = "detect"
         self.metrics = DetMetrics(save_dir=self.save_dir, on_plot=self.on_plot)
-        self.iouv = torch.linspace(0.5, 0.95, 10)  # IoU vector for mAP@0.5:0.95
+        self.iouv = torch.linspace(0.5, 0.95, 10)  # iou vector for mAP@0.5:0.95
         self.niou = self.iouv.numel()
         self.lb = []  # for autolabelling
 
     def preprocess(self, batch):
         """Preprocesses batch of images for YOLO training."""
         batch["img"] = batch["img"].to(self.device, non_blocking=True)
         batch["img"] = (batch["img"].half() if self.args.half else batch["img"].float()) / 255
@@ -63,17 +62,16 @@
 
         return batch
 
     def init_metrics(self, model):
         """Initialize evaluation metrics for YOLO."""
         val = self.data.get(self.args.split, "")  # validation path
         self.is_coco = isinstance(val, str) and "coco" in val and val.endswith(f"{os.sep}val2017.txt")  # is COCO
-        self.is_lvis = isinstance(val, str) and "lvis" in val and not self.is_coco  # is LVIS
-        self.class_map = converter.coco80_to_coco91_class() if self.is_coco else list(range(len(model.names)))
-        self.args.save_json |= (self.is_coco or self.is_lvis) and not self.training  # run on final val if training COCO
+        self.class_map = converter.coco80_to_coco91_class() if self.is_coco else list(range(1000))
+        self.args.save_json |= self.is_coco and not self.training  # run on final val if training COCO
         self.names = model.names
         self.nc = len(model.names)
         self.metrics.names = self.names
         self.metrics.plot = self.args.plots
         self.confusion_matrix = ConfusionMatrix(nc=self.nc, conf=self.args.conf)
         self.seen = 0
         self.jdict = []
@@ -130,29 +128,31 @@
             cls, bbox = pbatch.pop("cls"), pbatch.pop("bbox")
             nl = len(cls)
             stat["target_cls"] = cls
             if npr == 0:
                 if nl:
                     for k in self.stats.keys():
                         self.stats[k].append(stat[k])
-                    if self.args.plots:
+                    # TODO: obb has not supported confusion_matrix yet.
+                    if self.args.plots and self.args.task != "obb":
                         self.confusion_matrix.process_batch(detections=None, gt_bboxes=bbox, gt_cls=cls)
                 continue
 
             # Predictions
             if self.args.single_cls:
                 pred[:, 5] = 0
             predn = self._prepare_pred(pred, pbatch)
             stat["conf"] = predn[:, 4]
             stat["pred_cls"] = predn[:, 5]
 
             # Evaluate
             if nl:
                 stat["tp"] = self._process_batch(predn, bbox, cls)
-                if self.args.plots:
+                # TODO: obb has not supported confusion_matrix yet.
+                if self.args.plots and self.args.task != "obb":
                     self.confusion_matrix.process_batch(predn, bbox, cls)
             for k in self.stats.keys():
                 self.stats[k].append(stat[k])
 
             # Save
             if self.args.save_json:
                 self.pred_to_json(predn, batch["im_file"][si])
@@ -264,55 +264,38 @@
         image_id = int(stem) if stem.isnumeric() else stem
         box = ops.xyxy2xywh(predn[:, :4])  # xywh
         box[:, :2] -= box[:, 2:] / 2  # xy center to top-left corner
         for p, b in zip(predn.tolist(), box.tolist()):
             self.jdict.append(
                 {
                     "image_id": image_id,
-                    "category_id": self.class_map[int(p[5])]
-                    + (1 if self.is_lvis else 0),  # index starts from 1 if it's lvis
+                    "category_id": self.class_map[int(p[5])],
                     "bbox": [round(x, 3) for x in b],
                     "score": round(p[4], 5),
                 }
             )
 
     def eval_json(self, stats):
         """Evaluates YOLO output in JSON format and returns performance statistics."""
-        if self.args.save_json and (self.is_coco or self.is_lvis) and len(self.jdict):
+        if self.args.save_json and self.is_coco and len(self.jdict):
+            anno_json = self.data["path"] / "annotations/instances_val2017.json"  # annotations
             pred_json = self.save_dir / "predictions.json"  # predictions
-            anno_json = (
-                self.data["path"]
-                / "annotations"
-                / ("instances_val2017.json" if self.is_coco else f"lvis_v1_{self.args.split}.json")
-            )  # annotations
-            pkg = "pycocotools" if self.is_coco else "lvis"
-            LOGGER.info(f"\nEvaluating {pkg} mAP using {pred_json} and {anno_json}...")
+            LOGGER.info(f"\nEvaluating pycocotools mAP using {pred_json} and {anno_json}...")
             try:  # https://github.com/cocodataset/cocoapi/blob/master/PythonAPI/pycocoEvalDemo.ipynb
-                for x in pred_json, anno_json:
+                check_requirements("pycocotools>=2.0.6")
+                from pycocotools.coco import COCO  # noqa
+                from pycocotools.cocoeval import COCOeval  # noqa
+
+                for x in anno_json, pred_json:
                     assert x.is_file(), f"{x} file not found"
-                check_requirements("pycocotools>=2.0.6" if self.is_coco else "lvis>=0.5.3")
+                anno = COCO(str(anno_json))  # init annotations api
+                pred = anno.loadRes(str(pred_json))  # init predictions api (must pass string, not Path)
+                eval = COCOeval(anno, pred, "bbox")
                 if self.is_coco:
-                    from pycocotools.coco import COCO  # noqa
-                    from pycocotools.cocoeval import COCOeval  # noqa
-
-                    anno = COCO(str(anno_json))  # init annotations api
-                    pred = anno.loadRes(str(pred_json))  # init predictions api (must pass string, not Path)
-                    eval = COCOeval(anno, pred, "bbox")
-                else:
-                    from lvis import LVIS, LVISEval
-
-                    anno = LVIS(str(anno_json))  # init annotations api
-                    pred = anno._load_json(str(pred_json))  # init predictions api (must pass string, not Path)
-                    eval = LVISEval(anno, pred, "bbox")
-                eval.params.imgIds = [int(Path(x).stem) for x in self.dataloader.dataset.im_files]  # images to eval
+                    eval.params.imgIds = [int(Path(x).stem) for x in self.dataloader.dataset.im_files]  # images to eval
                 eval.evaluate()
                 eval.accumulate()
                 eval.summarize()
-                if self.is_lvis:
-                    eval.print_results()  # explicitly call print_results
-                # update mAP50-95 and mAP50
-                stats[self.metrics.keys[-1]], stats[self.metrics.keys[-2]] = (
-                    eval.stats[:2] if self.is_coco else [eval.results["AP50"], eval.results["AP"]]
-                )
+                stats[self.metrics.keys[-1]], stats[self.metrics.keys[-2]] = eval.stats[:2]  # update mAP50-95 and mAP50
             except Exception as e:
-                LOGGER.warning(f"{pkg} unable to run: {e}")
+                LOGGER.warning(f"pycocotools unable to run: {e}")
         return stats
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/models/yolo/obb/predict.py` & `pyppbox-ultralytics-8.1.7/ultralytics/models/yolo/obb/predict.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/models/yolo/obb/train.py` & `pyppbox-ultralytics-8.1.7/ultralytics/models/yolo/obb/train.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     """
     A class extending the DetectionTrainer class for training based on an Oriented Bounding Box (OBB) model.
 
     Example:
         ```python
         from ultralytics.models.yolo.obb import OBBTrainer
 
-        args = dict(model='yolov8n-obb.pt', data='dota8.yaml', epochs=3)
+        args = dict(model='yolov8n-seg.pt', data='coco8-seg.yaml', epochs=3)
         trainer = OBBTrainer(overrides=args)
         trainer.train()
         ```
     """
 
     def __init__(self, cfg=DEFAULT_CFG, overrides=None, _callbacks=None):
         """Initialize a OBBTrainer object with given arguments."""
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/models/yolo/obb/val.py` & `pyppbox-ultralytics-8.1.7/ultralytics/models/yolo/obb/val.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,19 +51,18 @@
         )
 
     def _process_batch(self, detections, gt_bboxes, gt_cls):
         """
         Return correct prediction matrix.
 
         Args:
-            detections (torch.Tensor): Tensor of shape [N, 7] representing detections.
-                Each detection is of the format: x1, y1, x2, y2, conf, class, angle.
-            gt_bboxes (torch.Tensor): Tensor of shape [M, 5] representing rotated boxes.
-                Each box is of the format: x1, y1, x2, y2, angle.
-            labels (torch.Tensor): Tensor of shape [M] representing labels.
+            detections (torch.Tensor): Tensor of shape [N, 6] representing detections.
+                Each detection is of the format: x1, y1, x2, y2, conf, class.
+            labels (torch.Tensor): Tensor of shape [M, 5] representing labels.
+                Each label is of the format: class, x1, y1, x2, y2.
 
         Returns:
             (torch.Tensor): Correct prediction matrix of shape [N, 10] for 10 IoU levels.
         """
         iou = batch_probiou(gt_bboxes, torch.cat([detections[:, :4], detections[:, -1:]], dim=-1))
         return self.match_predictions(detections[:, 5], gt_cls, iou)
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/models/yolo/pose/predict.py` & `pyppbox-ultralytics-8.1.7/ultralytics/models/yolo/pose/predict.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/models/yolo/pose/train.py` & `pyppbox-ultralytics-8.1.7/ultralytics/models/yolo/pose/train.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/models/yolo/pose/val.py` & `pyppbox-ultralytics-8.1.7/ultralytics/models/yolo/pose/val.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/models/yolo/segment/predict.py` & `pyppbox-ultralytics-8.1.7/ultralytics/models/yolo/segment/predict.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,15 +37,15 @@
             classes=self.args.classes,
         )
 
         if not isinstance(orig_imgs, list):  # input images are a torch.Tensor, not a list
             orig_imgs = ops.convert_torch2numpy_batch(orig_imgs)
 
         results = []
-        proto = preds[1][-1] if isinstance(preds[1], tuple) else preds[1]  # tuple if PyTorch model or array if exported
+        proto = preds[1][-1] if len(preds[1]) == 3 else preds[1]  # second output is len 3 if pt, but only 1 if exported
         for i, pred in enumerate(p):
             orig_img = orig_imgs[i]
             img_path = self.batch[0][i]
             if not len(pred):  # save empty boxes
                 masks = None
             elif self.args.retina_masks:
                 pred[:, :4] = ops.scale_boxes(img.shape[2:], pred[:, :4], orig_img.shape)
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/models/yolo/segment/train.py` & `pyppbox-ultralytics-8.1.7/ultralytics/models/yolo/segment/train.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/models/yolo/segment/val.py` & `pyppbox-ultralytics-8.1.7/ultralytics/models/yolo/segment/val.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/nn/__init__.py` & `pyppbox-ultralytics-8.1.7/ultralytics/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/nn/autobackend.py` & `pyppbox-ultralytics-8.1.7/ultralytics/nn/autobackend.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,42 +68,40 @@
             | CoreML                | *.mlpackage      |
             | TensorRT              | *.engine         |
             | TensorFlow SavedModel | *_saved_model    |
             | TensorFlow GraphDef   | *.pb             |
             | TensorFlow Lite       | *.tflite         |
             | TensorFlow Edge TPU   | *_edgetpu.tflite |
             | PaddlePaddle          | *_paddle_model   |
-            | NCNN                  | *_ncnn_model     |
+            | ncnn                  | *_ncnn_model     |
 
     This class offers dynamic backend switching capabilities based on the input model format, making it easier to deploy
     models across various platforms.
     """
 
     @torch.no_grad()
     def __init__(
         self,
         weights="yolov8n.pt",
         device=torch.device("cpu"),
         dnn=False,
         data=None,
         fp16=False,
-        batch=1,
         fuse=True,
         verbose=True,
     ):
         """
         Initialize the AutoBackend for inference.
 
         Args:
             weights (str): Path to the model weights file. Defaults to 'yolov8n.pt'.
             device (torch.device): Device to run the model on. Defaults to CPU.
             dnn (bool): Use OpenCV DNN module for ONNX inference. Defaults to False.
             data (str | Path | optional): Path to the additional data.yaml file containing class names. Optional.
             fp16 (bool): Enable half-precision inference. Supported only on specific backends. Defaults to False.
-            batch (int): Batch-size to assume for inference.
             fuse (bool): Fuse Conv2D + BatchNorm layers for optimization. Defaults to True.
             verbose (bool): Enable verbose logging. Defaults to True.
         """
         super().__init__()
         w = str(weights[0] if isinstance(weights, list) else weights)
         nn_module = isinstance(weights, torch.nn.Module)
         (
@@ -133,94 +131,75 @@
             device = torch.device("cpu")
             cuda = False
 
         # Download if not local
         if not (pt or triton or nn_module):
             w = attempt_download_asset(w)
 
-        # In-memory PyTorch model
-        if nn_module:
+        # Load model
+        if nn_module:  # in-memory PyTorch model
             model = weights.to(device)
-            if fuse:
-                model = model.fuse(verbose=verbose)
+            model = model.fuse(verbose=verbose) if fuse else model
             if hasattr(model, "kpt_shape"):
                 kpt_shape = model.kpt_shape  # pose-only
             stride = max(int(model.stride.max()), 32)  # model stride
             names = model.module.names if hasattr(model, "module") else model.names  # get class names
             model.half() if fp16 else model.float()
             self.model = model  # explicitly assign for to(), cpu(), cuda(), half()
             pt = True
-
-        # PyTorch
-        elif pt:
+        elif pt:  # PyTorch
             from ultralytics.nn.tasks import attempt_load_weights
 
             model = attempt_load_weights(
                 weights if isinstance(weights, list) else w, device=device, inplace=True, fuse=fuse
             )
             if hasattr(model, "kpt_shape"):
                 kpt_shape = model.kpt_shape  # pose-only
             stride = max(int(model.stride.max()), 32)  # model stride
             names = model.module.names if hasattr(model, "module") else model.names  # get class names
             model.half() if fp16 else model.float()
             self.model = model  # explicitly assign for to(), cpu(), cuda(), half()
-
-        # TorchScript
-        elif jit:
+        elif jit:  # TorchScript
             LOGGER.info(f"Loading {w} for TorchScript inference...")
             extra_files = {"config.txt": ""}  # model metadata
             model = torch.jit.load(w, _extra_files=extra_files, map_location=device)
             model.half() if fp16 else model.float()
             if extra_files["config.txt"]:  # load metadata dict
                 metadata = json.loads(extra_files["config.txt"], object_hook=lambda x: dict(x.items()))
-
-        # ONNX OpenCV DNN
-        elif dnn:
+        elif dnn:  # ONNX OpenCV DNN
             LOGGER.info(f"Loading {w} for ONNX OpenCV DNN inference...")
             # check_requirements("opencv-python>=4.5.4")
             net = cv2.dnn.readNetFromONNX(w)
-
-        # ONNX Runtime
-        elif onnx:
+        elif onnx:  # ONNX Runtime
             LOGGER.info(f"Loading {w} for ONNX Runtime inference...")
             check_requirements(("onnx", "onnxruntime-gpu" if cuda else "onnxruntime"))
             import onnxruntime
 
             providers = ["CUDAExecutionProvider", "CPUExecutionProvider"] if cuda else ["CPUExecutionProvider"]
             session = onnxruntime.InferenceSession(w, providers=providers)
             output_names = [x.name for x in session.get_outputs()]
-            metadata = session.get_modelmeta().custom_metadata_map
-
-        # OpenVINO
-        elif xml:
+            metadata = session.get_modelmeta().custom_metadata_map  # metadata
+        elif xml:  # OpenVINO
             LOGGER.info(f"Loading {w} for OpenVINO inference...")
-            check_requirements("openvino>=2024.0.0")
-            import openvino as ov
+            check_requirements("openvino>=2023.0")  # requires openvino-dev: https://pypi.org/project/openvino-dev/
+            from openvino.runtime import Core, Layout, get_batch  # noqa
 
-            core = ov.Core()
+            core = Core()
             w = Path(w)
             if not w.is_file():  # if not *.xml
                 w = next(w.glob("*.xml"))  # get *.xml file from *_openvino_model dir
             ov_model = core.read_model(model=str(w), weights=w.with_suffix(".bin"))
             if ov_model.get_parameters()[0].get_layout().empty:
-                ov_model.get_parameters()[0].set_layout(ov.Layout("NCHW"))
-
-            # OpenVINO inference modes are 'LATENCY', 'THROUGHPUT' (not recommended), or 'CUMULATIVE_THROUGHPUT'
-            inference_mode = "CUMULATIVE_THROUGHPUT" if batch > 1 else "LATENCY"
-            LOGGER.info(f"Using OpenVINO {inference_mode} mode for batch={batch} inference...")
-            ov_compiled_model = core.compile_model(
-                ov_model,
-                device_name="AUTO",  # AUTO selects best available device, do not modify
-                config={"PERFORMANCE_HINT": inference_mode},
-            )
-            input_name = ov_compiled_model.input().get_any_name()
+                ov_model.get_parameters()[0].set_layout(Layout("NCHW"))
+            batch_dim = get_batch(ov_model)
+            if batch_dim.is_static:
+                batch_size = batch_dim.get_length()
+            ov_compiled_model = core.compile_model(ov_model, device_name="AUTO")  # AUTO selects best available device
             metadata = w.parent / "metadata.yaml"
-
-        # TensorRT
-        elif engine:
+        elif engine:  # TensorRT
             LOGGER.info(f"Loading {w} for TensorRT inference...")
             try:
                 import tensorrt as trt  # noqa https://developer.nvidia.com/nvidia-tensorrt-download
             except ImportError:
                 if LINUX:
                     check_requirements("nvidia-tensorrt", cmds="-U --index-url https://pypi.ngc.nvidia.com")
                 import tensorrt as trt  # noqa
@@ -251,34 +230,28 @@
                 else:  # output
                     output_names.append(name)
                 shape = tuple(context.get_binding_shape(i))
                 im = torch.from_numpy(np.empty(shape, dtype=dtype)).to(device)
                 bindings[name] = Binding(name, dtype, shape, im, int(im.data_ptr()))
             binding_addrs = OrderedDict((n, d.ptr) for n, d in bindings.items())
             batch_size = bindings["images"].shape[0]  # if dynamic, this is instead max batch size
-
-        # CoreML
-        elif coreml:
+        elif coreml:  # CoreML
             LOGGER.info(f"Loading {w} for CoreML inference...")
             import coremltools as ct
 
             model = ct.models.MLModel(w)
             metadata = dict(model.user_defined_metadata)
-
-        # TF SavedModel
-        elif saved_model:
+        elif saved_model:  # TF SavedModel
             LOGGER.info(f"Loading {w} for TensorFlow SavedModel inference...")
             import tensorflow as tf
 
             keras = False  # assume TF1 saved_model
             model = tf.keras.models.load_model(w) if keras else tf.saved_model.load(w)
             metadata = Path(w) / "metadata.yaml"
-
-        # TF GraphDef
-        elif pb:  # https://www.tensorflow.org/guide/migrate#a_graphpb_or_graphpbtxt
+        elif pb:  # GraphDef https://www.tensorflow.org/guide/migrate#a_graphpb_or_graphpbtxt
             LOGGER.info(f"Loading {w} for TensorFlow GraphDef inference...")
             import tensorflow as tf
 
             from ultralytics.engine.exporter import gd_outputs
 
             def wrap_frozen_graph(gd, inputs, outputs):
                 """Wrap frozen graphs for deployment."""
@@ -286,16 +259,14 @@
                 ge = x.graph.as_graph_element
                 return x.prune(tf.nest.map_structure(ge, inputs), tf.nest.map_structure(ge, outputs))
 
             gd = tf.Graph().as_graph_def()  # TF GraphDef
             with open(w, "rb") as f:
                 gd.ParseFromString(f.read())
             frozen_func = wrap_frozen_graph(gd, inputs="x:0", outputs=gd_outputs(gd))
-
-        # TFLite or TFLite Edge TPU
         elif tflite or edgetpu:  # https://www.tensorflow.org/lite/guide/python#install_tensorflow_lite_for_python
             try:  # https://coral.ai/docs/edgetpu/tflite-python/#update-existing-tf-lite-code-for-the-edge-tpu
                 from tflite_runtime.interpreter import Interpreter, load_delegate
             except ImportError:
                 import tensorflow as tf
 
                 Interpreter, load_delegate = tf.lite.Interpreter, tf.lite.experimental.load_delegate
@@ -312,75 +283,66 @@
             input_details = interpreter.get_input_details()  # inputs
             output_details = interpreter.get_output_details()  # outputs
             # Load metadata
             with contextlib.suppress(zipfile.BadZipFile):
                 with zipfile.ZipFile(w, "r") as model:
                     meta_file = model.namelist()[0]
                     metadata = ast.literal_eval(model.read(meta_file).decode("utf-8"))
-
-        # TF.js
-        elif tfjs:
+        elif tfjs:  # TF.js
             raise NotImplementedError("YOLOv8 TF.js inference is not currently supported.")
-
-        # PaddlePaddle
-        elif paddle:
+        elif paddle:  # PaddlePaddle
             LOGGER.info(f"Loading {w} for PaddlePaddle inference...")
             check_requirements("paddlepaddle-gpu" if cuda else "paddlepaddle")
             import paddle.inference as pdi  # noqa
 
             w = Path(w)
             if not w.is_file():  # if not *.pdmodel
                 w = next(w.rglob("*.pdmodel"))  # get *.pdmodel file from *_paddle_model dir
             config = pdi.Config(str(w), str(w.with_suffix(".pdiparams")))
             if cuda:
                 config.enable_use_gpu(memory_pool_init_size_mb=2048, device_id=0)
             predictor = pdi.create_predictor(config)
             input_handle = predictor.get_input_handle(predictor.get_input_names()[0])
             output_names = predictor.get_output_names()
             metadata = w.parents[1] / "metadata.yaml"
-
-        # NCNN
-        elif ncnn:
-            LOGGER.info(f"Loading {w} for NCNN inference...")
-            check_requirements("git+https://github.com/Tencent/ncnn.git" if ARM64 else "ncnn")  # requires NCNN
+        elif ncnn:  # ncnn
+            LOGGER.info(f"Loading {w} for ncnn inference...")
+            check_requirements("git+https://github.com/Tencent/ncnn.git" if ARM64 else "ncnn")  # requires ncnn
             import ncnn as pyncnn
 
             net = pyncnn.Net()
             net.opt.use_vulkan_compute = cuda
             w = Path(w)
             if not w.is_file():  # if not *.param
                 w = next(w.glob("*.param"))  # get *.param file from *_ncnn_model dir
             net.load_param(str(w))
             net.load_model(str(w.with_suffix(".bin")))
             metadata = w.parent / "metadata.yaml"
-
-        # NVIDIA Triton Inference Server
-        elif triton:
+        elif triton:  # NVIDIA Triton Inference Server
             check_requirements("tritonclient[all]")
             from ultralytics.utils.triton import TritonRemoteModel
 
             model = TritonRemoteModel(w)
-
-        # Any other format (unsupported)
         else:
             from ultralytics.engine.exporter import export_formats
 
             raise TypeError(
                 f"model='{w}' is not a supported model format. "
-                f"See https://docs.ultralytics.com/modes/predict for help.\n\n{export_formats()}"
+                "See https://docs.ultralytics.com/modes/predict for help."
+                f"\n\n{export_formats()}"
             )
 
         # Load external metadata YAML
         if isinstance(metadata, (str, Path)) and Path(metadata).exists():
             metadata = yaml_load(metadata)
         if metadata:
             for k, v in metadata.items():
-                if k in {"stride", "batch"}:
+                if k in ("stride", "batch"):
                     metadata[k] = int(v)
-                elif k in {"imgsz", "names", "kpt_shape"} and isinstance(v, str):
+                elif k in ("imgsz", "names", "kpt_shape") and isinstance(v, str):
                     metadata[k] = eval(v)
             stride = metadata["stride"]
             task = metadata["task"]
             batch = metadata["batch"]
             imgsz = metadata["imgsz"]
             names = metadata["names"]
             kpt_shape = metadata.get("kpt_shape")
@@ -414,74 +376,42 @@
         """
         b, ch, h, w = im.shape  # batch, channel, height, width
         if self.fp16 and im.dtype != torch.float16:
             im = im.half()  # to FP16
         if self.nhwc:
             im = im.permute(0, 2, 3, 1)  # torch BCHW to numpy BHWC shape(1,320,192,3)
 
-        # PyTorch
-        if self.pt or self.nn_module:
+        if self.pt or self.nn_module:  # PyTorch
             y = self.model(im, augment=augment, visualize=visualize, embed=embed)
-
-        # TorchScript
-        elif self.jit:
+        elif self.jit:  # TorchScript
             y = self.model(im)
-
-        # ONNX OpenCV DNN
-        elif self.dnn:
+        elif self.dnn:  # ONNX OpenCV DNN
             im = im.cpu().numpy()  # torch to numpy
             self.net.setInput(im)
             y = self.net.forward()
-
-        # ONNX Runtime
-        elif self.onnx:
+        elif self.onnx:  # ONNX Runtime
             im = im.cpu().numpy()  # torch to numpy
             y = self.session.run(self.output_names, {self.session.get_inputs()[0].name: im})
-
-        # OpenVINO
-        elif self.xml:
+        elif self.xml:  # OpenVINO
             im = im.cpu().numpy()  # FP32
-
-            if self.inference_mode in {"THROUGHPUT", "CUMULATIVE_THROUGHPUT"}:  # optimized for larger batch-sizes
-                n = im.shape[0]  # number of images in batch
-                results = [None] * n  # preallocate list with None to match the number of images
-
-                def callback(request, userdata):
-                    """Places result in preallocated list using userdata index."""
-                    results[userdata] = request.results
-
-                # Create AsyncInferQueue, set the callback and start asynchronous inference for each input image
-                async_queue = self.ov.runtime.AsyncInferQueue(self.ov_compiled_model)
-                async_queue.set_callback(callback)
-                for i in range(n):
-                    # Start async inference with userdata=i to specify the position in results list
-                    async_queue.start_async(inputs={self.input_name: im[i : i + 1]}, userdata=i)  # keep image as BCHW
-                async_queue.wait_all()  # wait for all inference requests to complete
-                y = np.concatenate([list(r.values())[0] for r in results])
-
-            else:  # inference_mode = "LATENCY", optimized for fastest first result at batch-size 1
-                y = list(self.ov_compiled_model(im).values())
-
-        # TensorRT
-        elif self.engine:
+            y = list(self.ov_compiled_model(im).values())
+        elif self.engine:  # TensorRT
             if self.dynamic and im.shape != self.bindings["images"].shape:
                 i = self.model.get_binding_index("images")
                 self.context.set_binding_shape(i, im.shape)  # reshape if dynamic
                 self.bindings["images"] = self.bindings["images"]._replace(shape=im.shape)
                 for name in self.output_names:
                     i = self.model.get_binding_index(name)
                     self.bindings[name].data.resize_(tuple(self.context.get_binding_shape(i)))
             s = self.bindings["images"].shape
             assert im.shape == s, f"input size {im.shape} {'>' if self.dynamic else 'not equal to'} max model size {s}"
             self.binding_addrs["images"] = int(im.data_ptr())
             self.context.execute_v2(list(self.binding_addrs.values()))
             y = [self.bindings[x].data for x in sorted(self.output_names)]
-
-        # CoreML
-        elif self.coreml:
+        elif self.coreml:  # CoreML
             im = im[0].cpu().numpy()
             im_pil = Image.fromarray((im * 255).astype("uint8"))
             # im = im.resize((192, 320), Image.BILINEAR)
             y = self.model.predict({"image": im_pil})  # coordinates are xywh normalized
             if "confidence" in y:
                 raise TypeError(
                     "Ultralytics only supports inference of non-pipelined CoreML models exported with "
@@ -492,62 +422,59 @@
                 # box = xywh2xyxy(y['coordinates'] * [[w, h, w, h]])  # xyxy pixels
                 # conf, cls = y['confidence'].max(1), y['confidence'].argmax(1).astype(np.float32)
                 # y = np.concatenate((box, conf.reshape(-1, 1), cls.reshape(-1, 1)), 1)
             elif len(y) == 1:  # classification model
                 y = list(y.values())
             elif len(y) == 2:  # segmentation model
                 y = list(reversed(y.values()))  # reversed for segmentation models (pred, proto)
-
-        # PaddlePaddle
-        elif self.paddle:
+        elif self.paddle:  # PaddlePaddle
             im = im.cpu().numpy().astype(np.float32)
             self.input_handle.copy_from_cpu(im)
             self.predictor.run()
             y = [self.predictor.get_output_handle(x).copy_to_cpu() for x in self.output_names]
-
-        # NCNN
-        elif self.ncnn:
+        elif self.ncnn:  # ncnn
             mat_in = self.pyncnn.Mat(im[0].cpu().numpy())
-            with self.net.create_extractor() as ex:
-                ex.input(self.net.input_names()[0], mat_in)
-                y = [np.array(ex.extract(x)[1])[None] for x in self.net.output_names()]
-
-        # NVIDIA Triton Inference Server
-        elif self.triton:
+            ex = self.net.create_extractor()
+            input_names, output_names = self.net.input_names(), self.net.output_names()
+            ex.input(input_names[0], mat_in)
+            y = []
+            for output_name in output_names:
+                mat_out = self.pyncnn.Mat()
+                ex.extract(output_name, mat_out)
+                y.append(np.array(mat_out)[None])
+        elif self.triton:  # NVIDIA Triton Inference Server
             im = im.cpu().numpy()  # torch to numpy
             y = self.model(im)
-
-        # TensorFlow (SavedModel, GraphDef, Lite, Edge TPU)
-        else:
+        else:  # TensorFlow (SavedModel, GraphDef, Lite, Edge TPU)
             im = im.cpu().numpy()
             if self.saved_model:  # SavedModel
                 y = self.model(im, training=False) if self.keras else self.model(im)
                 if not isinstance(y, list):
                     y = [y]
             elif self.pb:  # GraphDef
                 y = self.frozen_func(x=self.tf.constant(im))
                 if len(y) == 2 and len(self.names) == 999:  # segments and names not defined
                     ip, ib = (0, 1) if len(y[0].shape) == 4 else (1, 0)  # index of protos, boxes
                     nc = y[ib].shape[1] - y[ip].shape[3] - 4  # y = (1, 160, 160, 32), (1, 116, 8400)
                     self.names = {i: f"class{i}" for i in range(nc)}
             else:  # Lite or Edge TPU
                 details = self.input_details[0]
-                is_int = details["dtype"] in {np.int8, np.int16}  # is TFLite quantized int8 or int16 model
-                if is_int:
+                integer = details["dtype"] in (np.int8, np.int16)  # is TFLite quantized int8 or int16 model
+                if integer:
                     scale, zero_point = details["quantization"]
                     im = (im / scale + zero_point).astype(details["dtype"])  # de-scale
                 self.interpreter.set_tensor(details["index"], im)
                 self.interpreter.invoke()
                 y = []
                 for output in self.output_details:
                     x = self.interpreter.get_tensor(output["index"])
-                    if is_int:
+                    if integer:
                         scale, zero_point = output["quantization"]
                         x = (x.astype(np.float32) - zero_point) * scale  # re-scale
-                    if x.ndim == 3:  # if task is not classification, excluding masks (ndim=4) as well
+                    if x.ndim > 2:  # if task is not classification
                         # Denormalize xywh by image size. See https://github.com/ultralytics/ultralytics/pull/1695
                         # xywh are normalized in TFLite/EdgeTPU to mitigate quantization error of integer models
                         x[:, [0, 2]] *= w
                         x[:, [1, 3]] *= h
                     y.append(x)
             # TF segment fixes: export is reversed vs ONNX export and protos are transposed
             if len(y) == 2:  # segment with (det, proto) output order reversed
@@ -600,22 +527,22 @@
         Examples:
             >>> model = AutoBackend(weights="path/to/model.onnx")
             >>> model_type = model._model_type()  # returns "onnx"
         """
         from ultralytics.engine.exporter import export_formats
 
         sf = list(export_formats().Suffix)  # export suffixes
-        if not is_url(p) and not isinstance(p, str):
+        if not is_url(p, check=False) and not isinstance(p, str):
             check_suffix(p, sf)  # checks
         name = Path(p).name
         types = [s in name for s in sf]
         types[5] |= name.endswith(".mlmodel")  # retain support for older Apple CoreML *.mlmodel formats
         types[8] &= not types[9]  # tflite &= not edgetpu
         if any(types):
             triton = False
         else:
             from urllib.parse import urlsplit
 
             url = urlsplit(p)
-            triton = bool(url.netloc) and bool(url.path) and url.scheme in {"http", "grpc"}
+            triton = url.netloc and url.path and url.scheme in {"http", "grpc"}
 
         return types + [triton]
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/nn/modules/__init__.py` & `pyppbox-ultralytics-8.1.7/ultralytics/nn/modules/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,32 +24,22 @@
     C3TR,
     DFL,
     SPP,
     SPPF,
     Bottleneck,
     BottleneckCSP,
     C2f,
-    C2fAttn,
-    ImagePoolingAttn,
     C3Ghost,
     C3x,
     GhostBottleneck,
     HGBlock,
     HGStem,
     Proto,
     RepC3,
     ResNetLayer,
-    ContrastiveHead,
-    BNContrastiveHead,
-    RepNCSPELAN4,
-    ADown,
-    SPPELAN,
-    CBFuse,
-    CBLinear,
-    Silence,
 )
 from .conv import (
     CBAM,
     ChannelAttention,
     Concat,
     Conv,
     Conv2,
@@ -58,15 +48,15 @@
     DWConvTranspose2d,
     Focus,
     GhostConv,
     LightConv,
     RepConv,
     SpatialAttention,
 )
-from .head import OBB, Classify, Detect, Pose, RTDETRDecoder, Segment, WorldDetect
+from .head import OBB, Classify, Detect, Pose, RTDETRDecoder, Segment
 from .transformer import (
     AIFI,
     MLP,
     DeformableTransformerDecoder,
     DeformableTransformerDecoderLayer,
     LayerNorm2d,
     MLPBlock,
@@ -99,15 +89,14 @@
     "HGStem",
     "SPP",
     "SPPF",
     "C1",
     "C2",
     "C3",
     "C2f",
-    "C2fAttn",
     "C3x",
     "C3TR",
     "C3Ghost",
     "GhostBottleneck",
     "Bottleneck",
     "BottleneckCSP",
     "Proto",
@@ -121,18 +110,8 @@
     "AIFI",
     "DeformableTransformerDecoder",
     "DeformableTransformerDecoderLayer",
     "MSDeformAttn",
     "MLP",
     "ResNetLayer",
     "OBB",
-    "WorldDetect",
-    "ImagePoolingAttn",
-    "ContrastiveHead",
-    "BNContrastiveHead",
-    "RepNCSPELAN4",
-    "ADown",
-    "SPPELAN",
-    "CBFuse",
-    "CBLinear",
-    "Silence",
 )
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/nn/modules/conv.py` & `pyppbox-ultralytics-8.1.7/ultralytics/nn/modules/conv.py`

 * *Files 1% similar despite different names*

```diff
@@ -292,15 +292,15 @@
 
 class SpatialAttention(nn.Module):
     """Spatial-attention module."""
 
     def __init__(self, kernel_size=7):
         """Initialize Spatial-attention module with kernel size argument."""
         super().__init__()
-        assert kernel_size in {3, 7}, "kernel size must be 3 or 7"
+        assert kernel_size in (3, 7), "kernel size must be 3 or 7"
         padding = 3 if kernel_size == 7 else 1
         self.cv1 = nn.Conv2d(2, 1, kernel_size, padding=padding, bias=False)
         self.act = nn.Sigmoid()
 
     def forward(self, x):
         """Apply channel and spatial attention on input for feature recalibration."""
         return x * self.act(self.cv1(torch.cat([torch.mean(x, 1, keepdim=True), torch.max(x, 1, keepdim=True)[0]], 1)))
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/nn/modules/head.py` & `pyppbox-ultralytics-8.1.7/ultralytics/nn/modules/head.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import math
 
 import torch
 import torch.nn as nn
 from torch.nn.init import constant_, xavier_uniform_
 
 from ultralytics.utils.tal import TORCH_1_10, dist2bbox, dist2rbox, make_anchors
-from .block import DFL, Proto, ContrastiveHead, BNContrastiveHead
+from .block import DFL, Proto
 from .conv import Conv
 from .transformer import MLP, DeformableTransformerDecoder, DeformableTransformerDecoderLayer
 from .utils import bias_init_with_prob, linear_init
 
 __all__ = "Detect", "Segment", "Pose", "Classify", "OBB", "RTDETRDecoder"
 
 
@@ -50,46 +50,45 @@
         # Inference path
         shape = x[0].shape  # BCHW
         x_cat = torch.cat([xi.view(shape[0], self.no, -1) for xi in x], 2)
         if self.dynamic or self.shape != shape:
             self.anchors, self.strides = (x.transpose(0, 1) for x in make_anchors(x, self.stride, 0.5))
             self.shape = shape
 
-        if self.export and self.format in {"saved_model", "pb", "tflite", "edgetpu", "tfjs"}:  # avoid TF FlexSplitV ops
+        if self.export and self.format in ("saved_model", "pb", "tflite", "edgetpu", "tfjs"):  # avoid TF FlexSplitV ops
             box = x_cat[:, : self.reg_max * 4]
             cls = x_cat[:, self.reg_max * 4 :]
         else:
             box, cls = x_cat.split((self.reg_max * 4, self.nc), 1)
+        dbox = self.decode_bboxes(box)
 
-        if self.export and self.format in {"tflite", "edgetpu"}:
+        if self.export and self.format in ("tflite", "edgetpu"):
             # Precompute normalization factor to increase numerical stability
             # See https://github.com/ultralytics/ultralytics/issues/7371
-            grid_h = shape[2]
-            grid_w = shape[3]
-            grid_size = torch.tensor([grid_w, grid_h, grid_w, grid_h], device=box.device).reshape(1, 4, 1)
-            norm = self.strides / (self.stride[0] * grid_size)
-            dbox = self.decode_bboxes(self.dfl(box) * norm, self.anchors.unsqueeze(0) * norm[:, :2])
-        else:
-            dbox = self.decode_bboxes(self.dfl(box), self.anchors.unsqueeze(0)) * self.strides
+            img_h = shape[2]
+            img_w = shape[3]
+            img_size = torch.tensor([img_w, img_h, img_w, img_h], device=box.device).reshape(1, 4, 1)
+            norm = self.strides / (self.stride[0] * img_size)
+            dbox = dist2bbox(self.dfl(box) * norm, self.anchors.unsqueeze(0) * norm[:, :2], xywh=True, dim=1)
 
         y = torch.cat((dbox, cls.sigmoid()), 1)
         return y if self.export else (y, x)
 
     def bias_init(self):
         """Initialize Detect() biases, WARNING: requires stride availability."""
         m = self  # self.model[-1]  # Detect() module
         # cf = torch.bincount(torch.tensor(np.concatenate(dataset.labels, 0)[:, 0]).long(), minlength=nc) + 1
         # ncf = math.log(0.6 / (m.nc - 0.999999)) if cf is None else torch.log(cf / cf.sum())  # nominal class frequency
         for a, b, s in zip(m.cv2, m.cv3, m.stride):  # from
             a[-1].bias.data[:] = 1.0  # box
             b[-1].bias.data[: m.nc] = math.log(5 / m.nc / (640 / s) ** 2)  # cls (.01 objects, 80 classes, 640 img)
 
-    def decode_bboxes(self, bboxes, anchors):
+    def decode_bboxes(self, bboxes):
         """Decode bounding boxes."""
-        return dist2bbox(bboxes, anchors, xywh=True, dim=1)
+        return dist2bbox(self.dfl(bboxes), self.anchors.unsqueeze(0), xywh=True, dim=1) * self.strides
 
 
 class Segment(Detect):
     """YOLOv8 Segment head for segmentation models."""
 
     def __init__(self, nc=80, nm=32, npr=256, ch=()):
         """Initialize the YOLO model attributes such as the number of masks, prototypes, and the convolution layers."""
@@ -136,17 +135,17 @@
         if not self.training:
             self.angle = angle
         x = self.detect(self, x)
         if self.training:
             return x, angle
         return torch.cat([x, angle], 1) if self.export else (torch.cat([x[0], angle], 1), (x[1], angle))
 
-    def decode_bboxes(self, bboxes, anchors):
+    def decode_bboxes(self, bboxes):
         """Decode rotated bounding boxes."""
-        return dist2rbox(bboxes, self.angle, anchors, dim=1)
+        return dist2rbox(self.dfl(bboxes), self.angle, self.anchors.unsqueeze(0), dim=1) * self.strides
 
 
 class Pose(Detect):
     """YOLOv8 Pose head for keypoints models."""
 
     def __init__(self, nc=80, kpt_shape=(17, 3), ch=()):
         """Initialize YOLO network with default parameters and Convolutional Layers."""
@@ -204,66 +203,14 @@
         """Performs a forward pass of the YOLO model on input image data."""
         if isinstance(x, list):
             x = torch.cat(x, 1)
         x = self.linear(self.drop(self.pool(self.conv(x)).flatten(1)))
         return x if self.training else x.softmax(1)
 
 
-class WorldDetect(Detect):
-    def __init__(self, nc=80, embed=512, with_bn=False, ch=()):
-        """Initialize YOLOv8 detection layer with nc classes and layer channels ch."""
-        super().__init__(nc, ch)
-        c3 = max(ch[0], min(self.nc, 100))
-        self.cv3 = nn.ModuleList(nn.Sequential(Conv(x, c3, 3), Conv(c3, c3, 3), nn.Conv2d(c3, embed, 1)) for x in ch)
-        self.cv4 = nn.ModuleList(BNContrastiveHead(embed) if with_bn else ContrastiveHead() for _ in ch)
-
-    def forward(self, x, text):
-        """Concatenates and returns predicted bounding boxes and class probabilities."""
-        for i in range(self.nl):
-            x[i] = torch.cat((self.cv2[i](x[i]), self.cv4[i](self.cv3[i](x[i]), text)), 1)
-        if self.training:
-            return x
-
-        # Inference path
-        shape = x[0].shape  # BCHW
-        x_cat = torch.cat([xi.view(shape[0], self.nc + self.reg_max * 4, -1) for xi in x], 2)
-        if self.dynamic or self.shape != shape:
-            self.anchors, self.strides = (x.transpose(0, 1) for x in make_anchors(x, self.stride, 0.5))
-            self.shape = shape
-
-        if self.export and self.format in {"saved_model", "pb", "tflite", "edgetpu", "tfjs"}:  # avoid TF FlexSplitV ops
-            box = x_cat[:, : self.reg_max * 4]
-            cls = x_cat[:, self.reg_max * 4 :]
-        else:
-            box, cls = x_cat.split((self.reg_max * 4, self.nc), 1)
-
-        if self.export and self.format in {"tflite", "edgetpu"}:
-            # Precompute normalization factor to increase numerical stability
-            # See https://github.com/ultralytics/ultralytics/issues/7371
-            grid_h = shape[2]
-            grid_w = shape[3]
-            grid_size = torch.tensor([grid_w, grid_h, grid_w, grid_h], device=box.device).reshape(1, 4, 1)
-            norm = self.strides / (self.stride[0] * grid_size)
-            dbox = self.decode_bboxes(self.dfl(box) * norm, self.anchors.unsqueeze(0) * norm[:, :2])
-        else:
-            dbox = self.decode_bboxes(self.dfl(box), self.anchors.unsqueeze(0)) * self.strides
-
-        y = torch.cat((dbox, cls.sigmoid()), 1)
-        return y if self.export else (y, x)
-
-    def bias_init(self):
-        """Initialize Detect() biases, WARNING: requires stride availability."""
-        m = self  # self.model[-1]  # Detect() module
-        # cf = torch.bincount(torch.tensor(np.concatenate(dataset.labels, 0)[:, 0]).long(), minlength=nc) + 1
-        # ncf = math.log(0.6 / (m.nc - 0.999999)) if cf is None else torch.log(cf / cf.sum())  # nominal class frequency
-        for a, b, s in zip(m.cv2, m.cv3, m.stride):  # from
-            a[-1].bias.data[:] = 1.0  # box
-            # b[-1].bias.data[:] = math.log(5 / m.nc / (640 / s) ** 2)  # cls (.01 objects, 80 classes, 640 img)
-
-
 class RTDETRDecoder(nn.Module):
     """
     Real-Time Deformable Transformer Decoder (RTDETRDecoder) module for object detection.
 
     This decoder module utilizes Transformer architecture along with deformable convolutions to predict bounding boxes
     and class labels for objects in an image. It integrates features from multiple layers and runs through a series of
     Transformer decoder layers to output the final predictions.
@@ -400,15 +347,15 @@
 
             valid_WH = torch.tensor([w, h], dtype=dtype, device=device)
             grid_xy = (grid_xy.unsqueeze(0) + 0.5) / valid_WH  # (1, h, w, 2)
             wh = torch.ones_like(grid_xy, dtype=dtype, device=device) * grid_size * (2.0**i)
             anchors.append(torch.cat([grid_xy, wh], -1).view(-1, h * w, 4))  # (1, h*w, 4)
 
         anchors = torch.cat(anchors, 1)  # (1, h*w*nl, 4)
-        valid_mask = ((anchors > eps) & (anchors < 1 - eps)).all(-1, keepdim=True)  # 1, h*w*nl, 1
+        valid_mask = ((anchors > eps) * (anchors < 1 - eps)).all(-1, keepdim=True)  # 1, h*w*nl, 1
         anchors = torch.log(anchors / (1 - anchors))
         anchors = anchors.masked_fill(~valid_mask, float("inf"))
         return anchors, valid_mask
 
     def _get_encoder_input(self, x):
         """Processes and returns encoder inputs by getting projection features from input and concatenating them."""
         # Get projection features
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/nn/modules/transformer.py` & `pyppbox-ultralytics-8.1.7/ultralytics/nn/modules/transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,15 +211,15 @@
         s = (x - u).pow(2).mean(1, keepdim=True)
         x = (x - u) / torch.sqrt(s + self.eps)
         return self.weight[:, None, None] * x + self.bias[:, None, None]
 
 
 class MSDeformAttn(nn.Module):
     """
-    Multiscale Deformable Attention Module based on Deformable-DETR and PaddleDetection implementations.
+    Multi-Scale Deformable Attention Module based on Deformable-DETR and PaddleDetection implementations.
 
     https://github.com/fundamentalvision/Deformable-DETR/blob/main/models/ops/modules/ms_deform_attn.py
     """
 
     def __init__(self, d_model=256, n_levels=4, n_heads=8, n_points=4):
         """Initialize MSDeformAttn with the given parameters."""
         super().__init__()
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/nn/modules/utils.py` & `pyppbox-ultralytics-8.1.7/ultralytics/nn/modules/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 def multi_scale_deformable_attn_pytorch(
     value: torch.Tensor,
     value_spatial_shapes: torch.Tensor,
     sampling_locations: torch.Tensor,
     attention_weights: torch.Tensor,
 ) -> torch.Tensor:
     """
-    Multiscale deformable attention.
+    Multi-scale deformable attention.
 
     https://github.com/IDEA-Research/detrex/blob/main/detrex/layers/multi_scale_deform_attn.py
     """
 
     bs, _, num_heads, embed_dims = value.shape
     _, num_queries, num_heads, num_levels, num_points, _ = sampling_locations.shape
     value_list = value.split([H_ * W_ for H_, W_ in value_spatial_shapes], dim=1)
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/nn/tasks.py` & `pyppbox-ultralytics-8.1.7/ultralytics/nn/tasks.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,16 +15,14 @@
     C3TR,
     OBB,
     SPP,
     SPPF,
     Bottleneck,
     BottleneckCSP,
     C2f,
-    C2fAttn,
-    ImagePoolingAttn,
     C3Ghost,
     C3x,
     Classify,
     Concat,
     Conv,
     Conv2,
     ConvTranspose,
@@ -38,21 +36,14 @@
     HGStem,
     Pose,
     RepC3,
     RepConv,
     ResNetLayer,
     RTDETRDecoder,
     Segment,
-    WorldDetect,
-    RepNCSPELAN4,
-    ADown,
-    SPPELAN,
-    CBFuse,
-    CBLinear,
-    Silence,
 )
 from ultralytics.utils import DEFAULT_CFG_DICT, DEFAULT_CFG_KEYS, LOGGER, colorstr, emojis, yaml_load
 from ultralytics.utils.checks import check_requirements, check_suffix, check_yaml
 from ultralytics.utils.loss import v8ClassificationLoss, v8DetectionLoss, v8OBBLoss, v8PoseLoss, v8SegmentationLoss
 from ultralytics.utils.plotting import feature_visualization
 from ultralytics.utils.torch_utils import (
     fuse_conv_and_bn,
@@ -227,15 +218,15 @@
             fn (function): the function to apply to the model
 
         Returns:
             (BaseModel): An updated BaseModel object.
         """
         self = super()._apply(fn)
         m = self.model[-1]  # Detect()
-        if isinstance(m, Detect):  # includes all Detect subclasses like Segment, Pose, OBB, WorldDetect
+        if isinstance(m, (Detect, Segment)):
             m.stride = fn(m.stride)
             m.anchors = fn(m.anchors)
             m.strides = fn(m.strides)
         return self
 
     def load(self, weights, verbose=True):
         """
@@ -286,15 +277,15 @@
             self.yaml["nc"] = nc  # override YAML value
         self.model, self.save = parse_model(deepcopy(self.yaml), ch=ch, verbose=verbose)  # model, savelist
         self.names = {i: f"{i}" for i in range(self.yaml["nc"])}  # default names dict
         self.inplace = self.yaml.get("inplace", True)
 
         # Build strides
         m = self.model[-1]  # Detect()
-        if isinstance(m, Detect):  # includes all Detect subclasses like Segment, Pose, OBB, WorldDetect
+        if isinstance(m, (Detect, Segment, Pose, OBB)):
             s = 256  # 2x min stride
             m.inplace = self.inplace
             forward = lambda x: self.forward(x)[0] if isinstance(m, (Segment, Pose, OBB)) else self.forward(x)
             m.stride = torch.tensor([s / x.shape[-2] for x in forward(torch.zeros(1, ch, s, s))])  # forward
             self.stride = m.stride
             m.bias_init()  # only run once
         else:
@@ -551,103 +542,14 @@
                 if m.i == max(embed):
                     return torch.unbind(torch.cat(embeddings, 1), dim=0)
         head = self.model[-1]
         x = head([y[j] for j in head.f], batch)  # head inference
         return x
 
 
-class WorldModel(DetectionModel):
-    """YOLOv8 World Model."""
-
-    def __init__(self, cfg="yolov8s-world.yaml", ch=3, nc=None, verbose=True):
-        """Initialize YOLOv8 world model with given config and parameters."""
-        self.txt_feats = torch.randn(1, nc or 80, 512)  # features placeholder
-        self.clip_model = None  # CLIP model placeholder
-        super().__init__(cfg=cfg, ch=ch, nc=nc, verbose=verbose)
-
-    def set_classes(self, text, batch=80, cache_clip_model=True):
-        """Set classes in advance so that model could do offline-inference without clip model."""
-        try:
-            import clip
-        except ImportError:
-            check_requirements("git+https://github.com/ultralytics/CLIP.git")
-            import clip
-
-        if (
-            not getattr(self, "clip_model", None) and cache_clip_model
-        ):  # for backwards compatibility of models lacking clip_model attribute
-            self.clip_model = clip.load("ViT-B/32")[0]
-        model = self.clip_model if cache_clip_model else clip.load("ViT-B/32")[0]
-        device = next(model.parameters()).device
-        text_token = clip.tokenize(text).to(device)
-        txt_feats = [model.encode_text(token).detach() for token in text_token.split(batch)]
-        txt_feats = txt_feats[0] if len(txt_feats) == 1 else torch.cat(txt_feats, dim=0)
-        txt_feats = txt_feats / txt_feats.norm(p=2, dim=-1, keepdim=True)
-        self.txt_feats = txt_feats.reshape(-1, len(text), txt_feats.shape[-1])
-        self.model[-1].nc = len(text)
-
-    def predict(self, x, profile=False, visualize=False, txt_feats=None, augment=False, embed=None):
-        """
-        Perform a forward pass through the model.
-
-        Args:
-            x (torch.Tensor): The input tensor.
-            profile (bool, optional): If True, profile the computation time for each layer. Defaults to False.
-            visualize (bool, optional): If True, save feature maps for visualization. Defaults to False.
-            txt_feats (torch.Tensor): The text features, use it if it's given. Defaults to None.
-            augment (bool, optional): If True, perform data augmentation during inference. Defaults to False.
-            embed (list, optional): A list of feature vectors/embeddings to return.
-
-        Returns:
-            (torch.Tensor): Model's output tensor.
-        """
-        txt_feats = (self.txt_feats if txt_feats is None else txt_feats).to(device=x.device, dtype=x.dtype)
-        if len(txt_feats) != len(x):
-            txt_feats = txt_feats.repeat(len(x), 1, 1)
-        ori_txt_feats = txt_feats.clone()
-        y, dt, embeddings = [], [], []  # outputs
-        for m in self.model:  # except the head part
-            if m.f != -1:  # if not from previous layer
-                x = y[m.f] if isinstance(m.f, int) else [x if j == -1 else y[j] for j in m.f]  # from earlier layers
-            if profile:
-                self._profile_one_layer(m, x, dt)
-            if isinstance(m, C2fAttn):
-                x = m(x, txt_feats)
-            elif isinstance(m, WorldDetect):
-                x = m(x, ori_txt_feats)
-            elif isinstance(m, ImagePoolingAttn):
-                txt_feats = m(x, txt_feats)
-            else:
-                x = m(x)  # run
-
-            y.append(x if m.i in self.save else None)  # save output
-            if visualize:
-                feature_visualization(x, m.type, m.i, save_dir=visualize)
-            if embed and m.i in embed:
-                embeddings.append(nn.functional.adaptive_avg_pool2d(x, (1, 1)).squeeze(-1).squeeze(-1))  # flatten
-                if m.i == max(embed):
-                    return torch.unbind(torch.cat(embeddings, 1), dim=0)
-        return x
-
-    def loss(self, batch, preds=None):
-        """
-        Compute loss.
-
-        Args:
-            batch (dict): Batch to compute loss on.
-            preds (torch.Tensor | List[torch.Tensor]): Predictions.
-        """
-        if not hasattr(self, "criterion"):
-            self.criterion = self.init_criterion()
-
-        if preds is None:
-            preds = self.forward(batch["img"], txt_feats=batch["txt_feats"])
-        return self.criterion(preds, batch)
-
-
 class Ensemble(nn.ModuleList):
     """Ensemble of models."""
 
     def __init__(self):
         """Initialize an ensemble of models."""
         super().__init__()
 
@@ -725,15 +627,15 @@
         with temporary_modules(
             {
                 "ultralytics.yolo.utils": "ultralytics.utils",
                 "ultralytics.yolo.v8": "ultralytics.models.yolo",
                 "ultralytics.yolo.data": "ultralytics.data",
             }
         ):  # for legacy 8.0 Classify and Pose models
-            ckpt = torch.load(file, map_location="cpu")
+            return torch.load(file, map_location="cpu"), file  # load
 
     except ModuleNotFoundError as e:  # e.name is missing module name
         if e.name == "models":
             raise TypeError(
                 emojis(
                     f"ERROR ❌️ {weight} appears to be an Ultralytics YOLOv5 model originally trained "
                     f"with https://github.com/ultralytics/yolov5.\nThis model is NOT forwards compatible with "
@@ -745,25 +647,16 @@
         LOGGER.warning(
             f"WARNING ⚠️ {weight} appears to require '{e.name}', which is not in ultralytics requirements."
             f"\nAutoInstall will run now for '{e.name}' but this feature will be removed in the future."
             f"\nRecommend fixes are to train a new model using the latest 'ultralytics' package or to "
             f"run a command with an official YOLOv8 model, i.e. 'yolo predict model=yolov8n.pt'"
         )
         check_requirements(e.name)  # install missing module
-        ckpt = torch.load(file, map_location="cpu")
 
-    if not isinstance(ckpt, dict):
-        # File is likely a YOLO instance saved with i.e. torch.save(model, "saved_model.pt")
-        LOGGER.warning(
-            f"WARNING ⚠️ The file '{weight}' appears to be improperly saved or formatted. "
-            f"For optimal results, use model.save('filename.pt') to correctly save YOLO models."
-        )
-        ckpt = {"model": ckpt.model}
-
-    return ckpt, file  # load
+        return torch.load(file, map_location="cpu"), file  # load
 
 
 def attempt_load_weights(weights, device=None, inplace=True, fuse=False):
     """Loads an ensemble of models weights=[a,b,c] or a single model weights=[a] or weights=a."""
 
     ensemble = Ensemble()
     for w in weights if isinstance(weights, list) else [weights]:
@@ -779,28 +672,29 @@
             model.stride = torch.tensor([32.0])
 
         # Append
         ensemble.append(model.fuse().eval() if fuse and hasattr(model, "fuse") else model.eval())  # model in eval mode
 
     # Module updates
     for m in ensemble.modules():
-        if hasattr(m, "inplace"):
+        t = type(m)
+        if t in (nn.Hardswish, nn.LeakyReLU, nn.ReLU, nn.ReLU6, nn.SiLU, Detect, Segment, Pose, OBB):
             m.inplace = inplace
-        elif isinstance(m, nn.Upsample) and not hasattr(m, "recompute_scale_factor"):
+        elif t is nn.Upsample and not hasattr(m, "recompute_scale_factor"):
             m.recompute_scale_factor = None  # torch 1.11.0 compatibility
 
     # Return model
     if len(ensemble) == 1:
         return ensemble[-1]
 
     # Return ensemble
     LOGGER.info(f"Ensemble created with {weights}\n")
     for k in "names", "nc", "yaml":
         setattr(ensemble, k, getattr(ensemble[0], k))
-    ensemble.stride = ensemble[int(torch.argmax(torch.tensor([m.stride.max() for m in ensemble])))].stride
+    ensemble.stride = ensemble[torch.argmax(torch.tensor([m.stride.max() for m in ensemble])).int()].stride
     assert all(ensemble[0].nc == m.nc for m in ensemble), f"Models differ in class counts {[m.nc for m in ensemble]}"
     return ensemble
 
 
 def attempt_load_one_weight(weight, device=None, inplace=True, fuse=False):
     """Loads a single model weights."""
     ckpt, weight = torch_safe_load(weight)  # load ckpt
@@ -814,17 +708,18 @@
     if not hasattr(model, "stride"):
         model.stride = torch.tensor([32.0])
 
     model = model.fuse().eval() if fuse and hasattr(model, "fuse") else model.eval()  # model in eval mode
 
     # Module updates
     for m in model.modules():
-        if hasattr(m, "inplace"):
+        t = type(m)
+        if t in (nn.Hardswish, nn.LeakyReLU, nn.ReLU, nn.ReLU6, nn.SiLU, Detect, Segment, Pose, OBB):
             m.inplace = inplace
-        elif isinstance(m, nn.Upsample) and not hasattr(m, "recompute_scale_factor"):
+        elif t is nn.Upsample and not hasattr(m, "recompute_scale_factor"):
             m.recompute_scale_factor = None  # torch 1.11.0 compatibility
 
     # Return model and ckpt
     return model, ckpt
 
 
 def parse_model(d, ch, verbose=True):  # model_dict, input_channels(3)
@@ -855,80 +750,65 @@
         m = getattr(torch.nn, m[3:]) if "nn." in m else globals()[m]  # get module
         for j, a in enumerate(args):
             if isinstance(a, str):
                 with contextlib.suppress(ValueError):
                     args[j] = locals()[a] if a in locals() else ast.literal_eval(a)
 
         n = n_ = max(round(n * depth), 1) if n > 1 else n  # depth gain
-        if m in {
+        if m in (
             Classify,
             Conv,
             ConvTranspose,
             GhostConv,
             Bottleneck,
             GhostBottleneck,
             SPP,
             SPPF,
             DWConv,
             Focus,
             BottleneckCSP,
             C1,
             C2,
             C2f,
-            RepNCSPELAN4,
-            ADown,
-            SPPELAN,
-            C2fAttn,
             C3,
             C3TR,
             C3Ghost,
             nn.ConvTranspose2d,
             DWConvTranspose2d,
             C3x,
             RepC3,
-        }:
+        ):
             c1, c2 = ch[f], args[0]
             if c2 != nc:  # if c2 not equal to number of classes (i.e. for Classify() output)
                 c2 = make_divisible(min(c2, max_channels) * width, 8)
-            if m is C2fAttn:
-                args[1] = make_divisible(min(args[1], max_channels // 2) * width, 8)  # embed channels
-                args[2] = int(
-                    max(round(min(args[2], max_channels // 2 // 32)) * width, 1) if args[2] > 1 else args[2]
-                )  # num heads
 
             args = [c1, c2, *args[1:]]
-            if m in {BottleneckCSP, C1, C2, C2f, C2fAttn, C3, C3TR, C3Ghost, C3x, RepC3}:
+            if m in (BottleneckCSP, C1, C2, C2f, C3, C3TR, C3Ghost, C3x, RepC3):
                 args.insert(2, n)  # number of repeats
                 n = 1
         elif m is AIFI:
             args = [ch[f], *args]
-        elif m in {HGStem, HGBlock}:
+        elif m in (HGStem, HGBlock):
             c1, cm, c2 = ch[f], args[0], args[1]
             args = [c1, cm, c2, *args[2:]]
             if m is HGBlock:
                 args.insert(4, n)  # number of repeats
                 n = 1
         elif m is ResNetLayer:
             c2 = args[1] if args[3] else args[1] * 4
         elif m is nn.BatchNorm2d:
             args = [ch[f]]
         elif m is Concat:
             c2 = sum(ch[x] for x in f)
-        elif m in {Detect, WorldDetect, Segment, Pose, OBB, ImagePoolingAttn}:
+        elif m in (Detect, Segment, Pose, OBB):
             args.append([ch[x] for x in f])
             if m is Segment:
                 args[2] = make_divisible(min(args[2], max_channels) * width, 8)
         elif m is RTDETRDecoder:  # special case, channels arg must be passed in index 1
             args.insert(1, [ch[x] for x in f])
-        elif m is CBLinear:
-            c2 = args[0]
-            c1 = ch[f]
-            args = [c1, c2, *args[1:]]
-        elif m is CBFuse:
-            c2 = ch[f[-1]]
         else:
             c2 = ch[f]
 
         m_ = nn.Sequential(*(m(*args) for _ in range(n))) if n > 1 else m(*args)  # module
         t = str(m)[8:-2].replace("__main__.", "")  # module type
         m.np = sum(x.numel() for x in m_.parameters())  # number params
         m_.i, m_.f, m_.type = i, f, t  # attach index, 'from' index, type
@@ -992,15 +872,15 @@
     Raises:
         SyntaxError: If the task of the model could not be determined.
     """
 
     def cfg2task(cfg):
         """Guess from YAML dictionary."""
         m = cfg["head"][-1][-2].lower()  # output module name
-        if m in {"classify", "classifier", "cls", "fc"}:
+        if m in ("classify", "classifier", "cls", "fc"):
             return "classify"
         if m == "detect":
             return "detect"
         if m == "segment":
             return "segment"
         if m == "pose":
             return "pose"
@@ -1018,24 +898,24 @@
             with contextlib.suppress(Exception):
                 return eval(x)["task"]
         for x in "model.yaml", "model.model.yaml", "model.model.model.yaml":
             with contextlib.suppress(Exception):
                 return cfg2task(eval(x))
 
         for m in model.modules():
-            if isinstance(m, Segment):
+            if isinstance(m, Detect):
+                return "detect"
+            elif isinstance(m, Segment):
                 return "segment"
             elif isinstance(m, Classify):
                 return "classify"
             elif isinstance(m, Pose):
                 return "pose"
             elif isinstance(m, OBB):
                 return "obb"
-            elif isinstance(m, (Detect, WorldDetect)):
-                return "detect"
 
     # Guess from model filename
     if isinstance(model, (str, Path)):
         model = Path(model)
         if "-seg" in model.stem or "segment" in model.parts:
             return "segment"
         elif "-cls" in model.stem or "classify" in model.parts:
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/solutions/ai_gym.py` & `pyppbox-ultralytics-8.1.7/ultralytics/solutions/ai_gym.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,50 +42,56 @@
         line_thickness=2,
         view_img=False,
         pose_up_angle=145.0,
         pose_down_angle=90.0,
         pose_type="pullup",
     ):
         """
-        Configures the AIGym line_thickness, save image and view image parameters.
-
+        Configures the AIGym line_thickness, save image and view image parameters
         Args:
             kpts_to_check (list): 3 keypoints for counting
             line_thickness (int): Line thickness for bounding boxes.
             view_img (bool): display the im0
             pose_up_angle (float): Angle to set pose position up
             pose_down_angle (float): Angle to set pose position down
-            pose_type (str): "pushup", "pullup" or "abworkout"
+            pose_type: "pushup", "pullup" or "abworkout"
         """
         self.kpts_to_check = kpts_to_check
         self.tf = line_thickness
         self.view_img = view_img
         self.poseup_angle = pose_up_angle
         self.posedown_angle = pose_down_angle
         self.pose_type = pose_type
 
     def start_counting(self, im0, results, frame_count):
         """
-        Function used to count the gym steps.
-
+        Function used to count the gym steps
         Args:
             im0 (ndarray): Current frame from the video stream.
-            results (list): Pose estimation data
-            frame_count (int): store current frame count
+            results: Pose estimation data
+            frame_count: store current frame count
         """
         self.im0 = im0
         if frame_count == 1:
             self.count = [0] * len(results[0])
             self.angle = [0] * len(results[0])
             self.stage = ["-" for _ in results[0]]
         self.keypoints = results[0].keypoints.data
         self.annotator = Annotator(im0, line_width=2)
 
+        num_keypoints = len(results[0])
+
+        # Resize self.angle, self.count, and self.stage if the number of keypoints has changed
+        if len(self.angle) != num_keypoints:
+            self.angle = [0] * num_keypoints
+            self.count = [0] * num_keypoints
+            self.stage = ["-" for _ in range(num_keypoints)]
+
         for ind, k in enumerate(reversed(self.keypoints)):
-            if self.pose_type in {"pushup", "pullup"}:
+            if self.pose_type in ["pushup", "pullup"]:
                 self.angle[ind] = self.annotator.estimate_pose_angle(
                     k[int(self.kpts_to_check[0])].cpu(),
                     k[int(self.kpts_to_check[1])].cpu(),
                     k[int(self.kpts_to_check[2])].cpu(),
                 )
                 self.im0 = self.annotator.draw_specific_points(k, self.kpts_to_check, shape=(640, 640), radius=10)
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/solutions/distance_calculation.py` & `pyppbox-ultralytics-8.1.7/ultralytics/solutions/distance_calculation.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,36 +103,33 @@
         """
         self.boxes = tracks[0].boxes.xyxy.cpu()
         self.clss = tracks[0].boxes.cls.cpu().tolist()
         self.trk_ids = tracks[0].boxes.id.int().cpu().tolist()
 
     def calculate_centroid(self, box):
         """
-        Calculate the centroid of bounding box.
-
+        Calculate the centroid of bounding box
         Args:
             box (list): Bounding box data
         """
         return int((box[0] + box[2]) // 2), int((box[1] + box[3]) // 2)
 
     def calculate_distance(self, centroid1, centroid2):
         """
-        Calculate distance between two centroids.
-
+        Calculate distance between two centroids
         Args:
             centroid1 (point): First bounding box data
             centroid2 (point): Second bounding box data
         """
         pixel_distance = math.sqrt((centroid1[0] - centroid2[0]) ** 2 + (centroid1[1] - centroid2[1]) ** 2)
         return pixel_distance / self.pixel_per_meter, (pixel_distance / self.pixel_per_meter) * 1000
 
     def start_process(self, im0, tracks):
         """
-        Calculate distance between two bounding boxes based on tracking data.
-
+        Calculate distance between two bounding boxes based on tracking data
         Args:
             im0 (nd array): Image
             tracks (list): List of tracks obtained from the object tracking process.
         """
         self.im0 = im0
         if tracks[0].boxes.id is None:
             if self.view_img:
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/solutions/heatmap.py` & `pyppbox-ultralytics-8.1.7/ultralytics/solutions/heatmap.py`

 * *Files 26% similar despite different names*

```diff
@@ -20,16 +20,14 @@
         """Initializes the heatmap class with default values for Visual, Image, track, count and heatmap parameters."""
 
         # Visual information
         self.annotator = None
         self.view_img = False
         self.shape = "circle"
 
-        self.names = None  # Classes names
-
         # Image information
         self.imw = None
         self.imh = None
         self.im0 = None
         self.view_in_counts = True
         self.view_out_counts = True
 
@@ -50,114 +48,104 @@
         self.line_dist_thresh = 15
         self.region_thickness = 5
         self.region_color = (255, 0, 255)
 
         # Object Counting Information
         self.in_counts = 0
         self.out_counts = 0
-        self.count_ids = []
-        self.class_wise_count = {}
+        self.counting_list = []
         self.count_txt_thickness = 0
-        self.count_txt_color = (255, 255, 255)
-        self.line_color = (255, 255, 255)
-        self.cls_txtdisplay_gap = 50
-        self.fontsize = 0.6
+        self.count_txt_color = (0, 0, 0)
+        self.count_color = (255, 255, 255)
 
         # Decay factor
         self.decay_factor = 0.99
 
         # Check if environment support imshow
         self.env_check = check_imshow(warn=True)
 
     def set_args(
         self,
         imw,
         imh,
-        classes_names=None,
         colormap=cv2.COLORMAP_JET,
         heatmap_alpha=0.5,
         view_img=False,
         view_in_counts=True,
         view_out_counts=True,
         count_reg_pts=None,
         count_txt_thickness=2,
-        count_txt_color=(255, 255, 255),
-        fontsize=0.8,
-        line_color=(255, 255, 255),
+        count_txt_color=(0, 0, 0),
+        count_color=(255, 255, 255),
         count_reg_color=(255, 0, 255),
         region_thickness=5,
         line_dist_thresh=15,
         decay_factor=0.99,
         shape="circle",
-        cls_txtdisplay_gap=50,
     ):
         """
         Configures the heatmap colormap, width, height and display parameters.
 
         Args:
             colormap (cv2.COLORMAP): The colormap to be set.
             imw (int): The width of the frame.
             imh (int): The height of the frame.
-            classes_names (dict): Classes names
             heatmap_alpha (float): alpha value for heatmap display
             view_img (bool): Flag indicating frame display
             view_in_counts (bool): Flag to control whether to display the incounts on video stream.
             view_out_counts (bool): Flag to control whether to display the outcounts on video stream.
             count_reg_pts (list): Object counting region points
             count_txt_thickness (int): Text thickness for object counting display
             count_txt_color (RGB color): count text color value
-            fontsize (float): Text display font size
-            line_color (RGB color): count highlighter line color
+            count_color (RGB color): count text background color value
             count_reg_color (RGB color): Color of object counting region
             region_thickness (int): Object counting Region thickness
             line_dist_thresh (int): Euclidean Distance threshold for line counter
             decay_factor (float): value for removing heatmap area after object passed
             shape (str): Heatmap shape, rect or circle shape supported
-            cls_txtdisplay_gap (int): Display gap between each class count
         """
-        self.names = classes_names
         self.imw = imw
         self.imh = imh
         self.heatmap_alpha = heatmap_alpha
         self.view_img = view_img
         self.view_in_counts = view_in_counts
         self.view_out_counts = view_out_counts
         self.colormap = colormap
 
         # Region and line selection
         if count_reg_pts is not None:
             if len(count_reg_pts) == 2:
                 print("Line Counter Initiated.")
                 self.count_reg_pts = count_reg_pts
-                self.counting_region = LineString(self.count_reg_pts)
-            elif len(count_reg_pts) >= 3:
-                print("Polygon Counter Initiated.")
+                self.counting_region = LineString(count_reg_pts)
+
+            elif len(count_reg_pts) == 4:
+                print("Region Counter Initiated.")
                 self.count_reg_pts = count_reg_pts
                 self.counting_region = Polygon(self.count_reg_pts)
+
             else:
-                print("Invalid Region points provided, region_points must be 2 for lines or >= 3 for polygons.")
+                print("Region or line points Invalid, 2 or 4 points supported")
                 print("Using Line Counter Now")
-                self.counting_region = LineString(self.count_reg_pts)
+                self.counting_region = Polygon([(20, 400), (1260, 400)])  # dummy points
 
         # Heatmap new frame
         self.heatmap = np.zeros((int(self.imh), int(self.imw)), dtype=np.float32)
 
         self.count_txt_thickness = count_txt_thickness
         self.count_txt_color = count_txt_color
-        self.fontsize = fontsize
-        self.line_color = line_color
+        self.count_color = count_color
         self.region_color = count_reg_color
         self.region_thickness = region_thickness
         self.decay_factor = decay_factor
         self.line_dist_thresh = line_dist_thresh
         self.shape = shape
-        self.cls_txtdisplay_gap = cls_txtdisplay_gap
 
         # shape of heatmap, if not selected
-        if self.shape not in {"circle", "rect"}:
+        if self.shape not in ["circle", "rect"]:
             print("Unknown shape value provided, 'circle' & 'rect' supported")
             print("Using Circular shape now")
             self.shape = "circle"
 
     def extract_results(self, tracks):
         """
         Extracts results from the provided data.
@@ -175,36 +163,29 @@
 
         Args:
             im0 (nd array): Image
             tracks (list): List of tracks obtained from the object tracking process.
         """
         self.im0 = im0
         if tracks[0].boxes.id is None:
-            self.heatmap = np.zeros((int(self.imh), int(self.imw)), dtype=np.float32)
             if self.view_img and self.env_check:
                 self.display_frames()
-            return im0
+            return
         self.heatmap *= self.decay_factor  # decay factor
         self.extract_results(tracks)
         self.annotator = Annotator(self.im0, self.count_txt_thickness, None)
 
         if self.count_reg_pts is not None:
             # Draw counting region
             if self.view_in_counts or self.view_out_counts:
                 self.annotator.draw_region(
                     reg_pts=self.count_reg_pts, color=self.region_color, thickness=self.region_thickness
                 )
 
             for box, cls, track_id in zip(self.boxes, self.clss, self.track_ids):
-                # Store class info
-                if self.names[cls] not in self.class_wise_count:
-                    if len(self.names[cls]) > 5:
-                        self.names[cls] = self.names[cls][:5]
-                    self.class_wise_count[self.names[cls]] = {"in": 0, "out": 0}
-
                 if self.shape == "circle":
                     center = (int((box[0] + box[2]) // 2), int((box[1] + box[3]) // 2))
                     radius = min(int(box[2]) - int(box[0]), int(box[3]) - int(box[1])) // 2
 
                     y, x = np.ogrid[0 : self.heatmap.shape[0], 0 : self.heatmap.shape[1]]
                     mask = (x - center[0]) ** 2 + (y - center[1]) ** 2 <= radius**2
 
@@ -217,47 +198,31 @@
 
                 # Store tracking hist
                 track_line = self.track_history[track_id]
                 track_line.append((float((box[0] + box[2]) / 2), float((box[1] + box[3]) / 2)))
                 if len(track_line) > 30:
                     track_line.pop(0)
 
-                prev_position = self.track_history[track_id][-2] if len(self.track_history[track_id]) > 1 else None
-
-                # Count objects in any polygon
-                if len(self.count_reg_pts) >= 3:
-                    is_inside = self.counting_region.contains(Point(track_line[-1]))
-
-                    if prev_position is not None and is_inside and track_id not in self.count_ids:
-                        self.count_ids.append(track_id)
-
-                        if (box[0] - prev_position[0]) * (self.counting_region.centroid.x - prev_position[0]) > 0:
-                            self.in_counts += 1
-                            self.class_wise_count[self.names[cls]]["in"] += 1
-                        else:
+                # Count objects
+                if len(self.count_reg_pts) == 4:
+                    if self.counting_region.contains(Point(track_line[-1])) and track_id not in self.counting_list:
+                        self.counting_list.append(track_id)
+                        if box[0] < self.counting_region.centroid.x:
                             self.out_counts += 1
-                            self.class_wise_count[self.names[cls]]["out"] += 1
+                        else:
+                            self.in_counts += 1
 
-                # Count objects using line
                 elif len(self.count_reg_pts) == 2:
-                    is_inside = (box[0] - prev_position[0]) * (self.counting_region.centroid.x - prev_position[0]) > 0
-
-                    if prev_position is not None and is_inside and track_id not in self.count_ids:
-                        distance = Point(track_line[-1]).distance(self.counting_region)
-
-                        if distance < self.line_dist_thresh and track_id not in self.count_ids:
-                            self.count_ids.append(track_id)
-
-                            if (box[0] - prev_position[0]) * (self.counting_region.centroid.x - prev_position[0]) > 0:
-                                self.in_counts += 1
-                                self.class_wise_count[self.names[cls]]["in"] += 1
-                            else:
-                                self.out_counts += 1
-                                self.class_wise_count[self.names[cls]]["out"] += 1
-
+                    distance = Point(track_line[-1]).distance(self.counting_region)
+                    if distance < self.line_dist_thresh and track_id not in self.counting_list:
+                        self.counting_list.append(track_id)
+                        if box[0] < self.counting_region.centroid.x:
+                            self.out_counts += 1
+                        else:
+                            self.in_counts += 1
         else:
             for box, cls in zip(self.boxes, self.clss):
                 if self.shape == "circle":
                     center = (int((box[0] + box[2]) // 2), int((box[1] + box[3]) // 2))
                     radius = min(int(box[2]) - int(box[0]), int(box[3]) - int(box[1])) // 2
 
                     y, x = np.ogrid[0 : self.heatmap.shape[0], 0 : self.heatmap.shape[1]]
@@ -270,38 +235,34 @@
                 else:
                     self.heatmap[int(box[1]) : int(box[3]), int(box[0]) : int(box[2])] += 2
 
         # Normalize, apply colormap to heatmap and combine with original image
         heatmap_normalized = cv2.normalize(self.heatmap, None, 0, 255, cv2.NORM_MINMAX)
         heatmap_colored = cv2.applyColorMap(heatmap_normalized.astype(np.uint8), self.colormap)
 
-        label = "Ultralytics Analytics \t"
+        incount_label = f"In Count : {self.in_counts}"
+        outcount_label = f"OutCount : {self.out_counts}"
 
-        for key, value in self.class_wise_count.items():
-            if value["in"] != 0 or value["out"] != 0:
-                if not self.view_in_counts and not self.view_out_counts:
-                    label = None
-                elif not self.view_in_counts:
-                    label += f"{str.capitalize(key)}: IN {value['in']} \t"
-                elif not self.view_out_counts:
-                    label += f"{str.capitalize(key)}: OUT {value['out']} \t"
-                else:
-                    label += f"{str.capitalize(key)}: IN {value['in']} OUT {value['out']} \t"
-
-        label = label.rstrip()
-        label = label.split("\t")
+        # Display counts based on user choice
+        counts_label = None
+        if not self.view_in_counts and not self.view_out_counts:
+            counts_label = None
+        elif not self.view_in_counts:
+            counts_label = outcount_label
+        elif not self.view_out_counts:
+            counts_label = incount_label
+        else:
+            counts_label = f"{incount_label} {outcount_label}"
 
-        if self.count_reg_pts is not None and label is not None:
-            self.annotator.display_counts(
-                counts=label,
-                tf=self.count_txt_thickness,
-                fontScale=self.fontsize,
+        if self.count_reg_pts is not None and counts_label is not None:
+            self.annotator.count_labels(
+                counts=counts_label,
+                count_txt_size=self.count_txt_thickness,
                 txt_color=self.count_txt_color,
-                line_color=self.line_color,
-                classwise_txtgap=self.cls_txtdisplay_gap,
+                color=self.count_color,
             )
 
         self.im0 = cv2.addWeighted(self.im0, 1 - self.heatmap_alpha, heatmap_colored, self.heatmap_alpha, 0)
 
         if self.env_check and self.view_img:
             self.display_frames()
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/solutions/object_counter.py` & `pyppbox-ultralytics-8.1.7/ultralytics/solutions/object_counter.py`

 * *Files 26% similar despite different names*

```diff
@@ -34,32 +34,28 @@
         self.tf = None
         self.view_img = False
         self.view_in_counts = True
         self.view_out_counts = True
 
         self.names = None  # Classes names
         self.annotator = None  # Annotator
-        self.window_name = "Ultralytics YOLOv8 Object Counter"
 
         # Object counting Information
         self.in_counts = 0
         self.out_counts = 0
-        self.count_ids = []
-        self.class_wise_count = {}
+        self.counting_list = []
         self.count_txt_thickness = 0
-        self.count_txt_color = (255, 255, 255)
-        self.line_color = (255, 255, 255)
-        self.cls_txtdisplay_gap = 50
-        self.fontsize = 0.6
+        self.count_txt_color = (0, 0, 0)
+        self.count_color = (255, 255, 255)
 
         # Tracks info
         self.track_history = defaultdict(list)
         self.track_thickness = 2
         self.draw_tracks = False
-        self.track_color = None
+        self.track_color = (0, 255, 0)
 
         # Check if environment support imshow
         self.env_check = check_imshow(warn=True)
 
     def set_args(
         self,
         classes_names,
@@ -67,22 +63,20 @@
         count_reg_color=(255, 0, 255),
         line_thickness=2,
         track_thickness=2,
         view_img=False,
         view_in_counts=True,
         view_out_counts=True,
         draw_tracks=False,
-        count_txt_thickness=3,
-        count_txt_color=(255, 255, 255),
-        fontsize=0.8,
-        line_color=(255, 255, 255),
-        track_color=None,
+        count_txt_thickness=2,
+        count_txt_color=(0, 0, 0),
+        count_color=(255, 255, 255),
+        track_color=(0, 255, 0),
         region_thickness=5,
         line_dist_thresh=15,
-        cls_txtdisplay_gap=50,
     ):
         """
         Configures the Counter's image, bounding box line thickness, and counting region points.
 
         Args:
             line_thickness (int): Line thickness for bounding boxes.
             view_img (bool): Flag to control whether to display the video stream.
@@ -90,53 +84,49 @@
             view_out_counts (bool): Flag to control whether to display the outcounts on video stream.
             reg_pts (list): Initial list of points defining the counting region.
             classes_names (dict): Classes names
             track_thickness (int): Track thickness
             draw_tracks (Bool): draw tracks
             count_txt_thickness (int): Text thickness for object counting display
             count_txt_color (RGB color): count text color value
-            fontsize (float): Text display font size
-            line_color (RGB color): count highlighter line color
+            count_color (RGB color): count text background color value
             count_reg_color (RGB color): Color of object counting region
             track_color (RGB color): color for tracks
             region_thickness (int): Object counting Region thickness
             line_dist_thresh (int): Euclidean Distance threshold for line counter
-            cls_txtdisplay_gap (int): Display gap between each class count
         """
         self.tf = line_thickness
         self.view_img = view_img
         self.view_in_counts = view_in_counts
         self.view_out_counts = view_out_counts
         self.track_thickness = track_thickness
         self.draw_tracks = draw_tracks
 
         # Region and line selection
         if len(reg_pts) == 2:
             print("Line Counter Initiated.")
             self.reg_pts = reg_pts
             self.counting_region = LineString(self.reg_pts)
-        elif len(reg_pts) >= 3:
-            print("Polygon Counter Initiated.")
+        elif len(reg_pts) == 4:
+            print("Region Counter Initiated.")
             self.reg_pts = reg_pts
             self.counting_region = Polygon(self.reg_pts)
         else:
-            print("Invalid Region points provided, region_points must be 2 for lines or >= 3 for polygons.")
+            print("Invalid Region points provided, region_points can be 2 or 4")
             print("Using Line Counter Now")
             self.counting_region = LineString(self.reg_pts)
 
         self.names = classes_names
         self.track_color = track_color
         self.count_txt_thickness = count_txt_thickness
         self.count_txt_color = count_txt_color
-        self.fontsize = fontsize
-        self.line_color = line_color
+        self.count_color = count_color
         self.region_color = count_reg_color
         self.region_thickness = region_thickness
         self.line_dist_thresh = line_dist_thresh
-        self.cls_txtdisplay_gap = cls_txtdisplay_gap
 
     def mouse_event_for_region(self, event, x, y, flags, params):
         """
         This function is designed to move region with mouse events in a real-time video stream.
 
         Args:
             event (int): The type of mouse event (e.g., cv2.EVENT_MOUSEMOVE, cv2.EVENT_LBUTTONDOWN, etc.).
@@ -164,129 +154,114 @@
 
         elif event == cv2.EVENT_LBUTTONUP:
             self.is_drawing = False
             self.selected_point = None
 
     def extract_and_process_tracks(self, tracks):
         """Extracts and processes tracks for object counting in a video stream."""
+        boxes = tracks[0].boxes.xyxy.cpu()
+        clss = tracks[0].boxes.cls.cpu().tolist()
+        track_ids = tracks[0].boxes.id.int().cpu().tolist()
 
         # Annotator Init and region drawing
         self.annotator = Annotator(self.im0, self.tf, self.names)
+        self.annotator.draw_region(reg_pts=self.reg_pts, color=self.region_color, thickness=self.region_thickness)
 
-        if tracks[0].boxes.id is not None:
-            boxes = tracks[0].boxes.xyxy.cpu()
-            clss = tracks[0].boxes.cls.cpu().tolist()
-            track_ids = tracks[0].boxes.id.int().cpu().tolist()
-
-            # Extract tracks
-            for box, track_id, cls in zip(boxes, track_ids, clss):
-                # Draw bounding box
-                self.annotator.box_label(box, label=f"{self.names[cls]}#{track_id}", color=colors(int(track_id), True))
-
-                # Store class info
-                if self.names[cls] not in self.class_wise_count:
-                    if len(self.names[cls]) > 5:
-                        self.names[cls] = self.names[cls][:5]
-                    self.class_wise_count[self.names[cls]] = {"in": 0, "out": 0}
-
-                # Draw Tracks
-                track_line = self.track_history[track_id]
-                track_line.append((float((box[0] + box[2]) / 2), float((box[1] + box[3]) / 2)))
-                if len(track_line) > 30:
-                    track_line.pop(0)
-
-                # Draw track trails
-                if self.draw_tracks:
-                    self.annotator.draw_centroid_and_tracks(
-                        track_line,
-                        color=self.track_color if self.track_color else colors(int(track_id), True),
-                        track_thickness=self.track_thickness,
-                    )
-
-                prev_position = self.track_history[track_id][-2] if len(self.track_history[track_id]) > 1 else None
-
-                # Count objects in any polygon
-                if len(self.reg_pts) >= 3:
-                    is_inside = self.counting_region.contains(Point(track_line[-1]))
+        # Extract tracks
+        for box, track_id, cls in zip(boxes, track_ids, clss):
+            # Draw bounding box
+            self.annotator.box_label(box, label=f"{track_id}:{self.names[cls]}", color=colors(int(cls), True))
+
+            # Draw Tracks
+            track_line = self.track_history[track_id]
+            track_line.append((float((box[0] + box[2]) / 2), float((box[1] + box[3]) / 2)))
+            if len(track_line) > 30:
+                track_line.pop(0)
+
+            # Draw track trails
+            if self.draw_tracks:
+                self.annotator.draw_centroid_and_tracks(
+                    track_line, color=self.track_color, track_thickness=self.track_thickness
+                )
 
-                    if prev_position is not None and is_inside and track_id not in self.count_ids:
-                        self.count_ids.append(track_id)
+            prev_position = self.track_history[track_id][-2] if len(self.track_history[track_id]) > 1 else None
 
+            # Count objects
+            if len(self.reg_pts) == 4:
+                if (
+                    prev_position is not None
+                    and self.counting_region.contains(Point(track_line[-1]))
+                    and track_id not in self.counting_list
+                ):
+                    self.counting_list.append(track_id)
+                    if (box[0] - prev_position[0]) * (self.counting_region.centroid.x - prev_position[0]) > 0:
+                        self.in_counts += 1
+                    else:
+                        self.out_counts += 1
+
+            elif len(self.reg_pts) == 2:
+                if prev_position is not None:
+                    distance = Point(track_line[-1]).distance(self.counting_region)
+                    if distance < self.line_dist_thresh and track_id not in self.counting_list:
+                        self.counting_list.append(track_id)
                         if (box[0] - prev_position[0]) * (self.counting_region.centroid.x - prev_position[0]) > 0:
                             self.in_counts += 1
-                            self.class_wise_count[self.names[cls]]["in"] += 1
                         else:
                             self.out_counts += 1
-                            self.class_wise_count[self.names[cls]]["out"] += 1
 
-                # Count objects using line
-                elif len(self.reg_pts) == 2:
-                    is_inside = (box[0] - prev_position[0]) * (self.counting_region.centroid.x - prev_position[0]) > 0
-
-                    if prev_position is not None and is_inside and track_id not in self.count_ids:
-                        distance = Point(track_line[-1]).distance(self.counting_region)
-
-                        if distance < self.line_dist_thresh and track_id not in self.count_ids:
-                            self.count_ids.append(track_id)
-
-                            if (box[0] - prev_position[0]) * (self.counting_region.centroid.x - prev_position[0]) > 0:
-                                self.in_counts += 1
-                                self.class_wise_count[self.names[cls]]["in"] += 1
-                            else:
-                                self.out_counts += 1
-                                self.class_wise_count[self.names[cls]]["out"] += 1
-
-        label = "Ultralytics Analytics \t"
-
-        for key, value in self.class_wise_count.items():
-            if value["in"] != 0 or value["out"] != 0:
-                if not self.view_in_counts and not self.view_out_counts:
-                    label = None
-                elif not self.view_in_counts:
-                    label += f"{str.capitalize(key)}: IN {value['in']} \t"
-                elif not self.view_out_counts:
-                    label += f"{str.capitalize(key)}: OUT {value['out']} \t"
-                else:
-                    label += f"{str.capitalize(key)}: IN {value['in']} OUT {value['out']} \t"
-
-        label = label.rstrip()
-        label = label.split("\t")
-
-        if label is not None:
-            self.annotator.display_counts(
-                counts=label,
-                tf=self.count_txt_thickness,
-                fontScale=self.fontsize,
+        incount_label = f"In Count : {self.in_counts}"
+        outcount_label = f"OutCount : {self.out_counts}"
+
+        # Display counts based on user choice
+        counts_label = None
+        if not self.view_in_counts and not self.view_out_counts:
+            counts_label = None
+        elif not self.view_in_counts:
+            counts_label = outcount_label
+        elif not self.view_out_counts:
+            counts_label = incount_label
+        else:
+            counts_label = f"{incount_label} {outcount_label}"
+
+        if counts_label is not None:
+            self.annotator.count_labels(
+                counts=counts_label,
+                count_txt_size=self.count_txt_thickness,
                 txt_color=self.count_txt_color,
-                line_color=self.line_color,
-                classwise_txtgap=self.cls_txtdisplay_gap,
+                color=self.count_color,
             )
 
     def display_frames(self):
         """Display frame."""
         if self.env_check:
-            self.annotator.draw_region(reg_pts=self.reg_pts, color=self.region_color, thickness=self.region_thickness)
-            cv2.namedWindow(self.window_name)
+            cv2.namedWindow("Ultralytics YOLOv8 Object Counter")
             if len(self.reg_pts) == 4:  # only add mouse event If user drawn region
-                cv2.setMouseCallback(self.window_name, self.mouse_event_for_region, {"region_points": self.reg_pts})
-            cv2.imshow(self.window_name, self.im0)
+                cv2.setMouseCallback(
+                    "Ultralytics YOLOv8 Object Counter", self.mouse_event_for_region, {"region_points": self.reg_pts}
+                )
+            cv2.imshow("Ultralytics YOLOv8 Object Counter", self.im0)
             # Break Window
             if cv2.waitKey(1) & 0xFF == ord("q"):
                 return
 
     def start_counting(self, im0, tracks):
         """
         Main function to start the object counting process.
 
         Args:
             im0 (ndarray): Current frame from the video stream.
             tracks (list): List of tracks obtained from the object tracking process.
         """
         self.im0 = im0  # store image
-        self.extract_and_process_tracks(tracks)  # draw region even if no objects
+
+        if tracks[0].boxes.id is None:
+            if self.view_img:
+                self.display_frames()
+            return
+        self.extract_and_process_tracks(tracks)
 
         if self.view_img:
             self.display_frames()
         return self.im0
 
 
 if __name__ == "__main__":
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/solutions/speed_estimation.py` & `pyppbox-ultralytics-8.1.7/ultralytics/solutions/speed_estimation.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,16 +120,15 @@
         self.annotator.box_label(box, speed_label, bbox_color)
 
         cv2.polylines(self.im0, [self.trk_pts], isClosed=False, color=(0, 255, 0), thickness=1)
         cv2.circle(self.im0, (int(track[-1][0]), int(track[-1][1])), 5, bbox_color, -1)
 
     def calculate_speed(self, trk_id, track):
         """
-        Calculation of object speed.
-
+        Calculation of object speed
         Args:
             trk_id (int): object track id.
             track (list): tracking history for tracks path drawing
         """
 
         if not self.reg_pts[0][0] < track[-1][0] < self.reg_pts[1][0]:
             return
@@ -150,32 +149,30 @@
                 dist_difference = np.abs(track[-1][1] - self.trk_previous_points[trk_id][1])
                 speed = dist_difference / time_difference
                 self.dist_data[trk_id] = speed
 
         self.trk_previous_times[trk_id] = time()
         self.trk_previous_points[trk_id] = track[-1]
 
-    def estimate_speed(self, im0, tracks, region_color=(255, 0, 0)):
+    def estimate_speed(self, im0, tracks):
         """
-        Calculate object based on tracking data.
-
+        Calculate object based on tracking data
         Args:
             im0 (nd array): Image
             tracks (list): List of tracks obtained from the object tracking process.
-            region_color (tuple): Color to use when drawing regions.
         """
         self.im0 = im0
         if tracks[0].boxes.id is None:
             if self.view_img and self.env_check:
                 self.display_frames()
-            return im0
+            return
         self.extract_tracks(tracks)
 
         self.annotator = Annotator(self.im0, line_width=2)
-        self.annotator.draw_region(reg_pts=self.reg_pts, color=region_color, thickness=self.region_thickness)
+        self.annotator.draw_region(reg_pts=self.reg_pts, color=(255, 0, 0), thickness=self.region_thickness)
 
         for box, trk_id, cls in zip(self.boxes, self.trk_ids, self.clss):
             track = self.store_track_info(trk_id, box)
 
             if trk_id not in self.trk_previous_times:
                 self.trk_previous_times[trk_id] = 0
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/trackers/basetrack.py` & `pyppbox-ultralytics-8.1.7/ultralytics/trackers/basetrack.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/trackers/bot_sort.py` & `pyppbox-ultralytics-8.1.7/ultralytics/trackers/bot_sort.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/trackers/byte_tracker.py` & `pyppbox-ultralytics-8.1.7/ultralytics/trackers/byte_tracker.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
     shared_kalman = KalmanFilterXYAH()
 
     def __init__(self, xywh, score, cls):
         """Initialize new STrack instance."""
         super().__init__()
         # xywh+idx or xywha+idx
-        assert len(xywh) in {5, 6}, f"expected 5 or 6 values but got {len(xywh)}"
+        assert len(xywh) in [5, 6], f"expected 5 or 6 values but got {len(xywh)}"
         self._tlwh = np.asarray(xywh2ltwh(xywh[:4]), dtype=np.float32)
         self.kalman_filter = None
         self.mean, self.covariance = None, None
         self.is_activated = False
 
         self.score = score
         self.tracklet_len = 0
@@ -231,15 +231,15 @@
         get_kalmanfilter(): Returns a Kalman filter object for tracking bounding boxes.
         init_track(dets, scores, cls, img=None): Initialize object tracking with detections.
         get_dists(tracks, detections): Calculates the distance between tracks and detections.
         multi_predict(tracks): Predicts the location of tracks.
         reset_id(): Resets the ID counter of STrack.
         joint_stracks(tlista, tlistb): Combines two lists of stracks.
         sub_stracks(tlista, tlistb): Filters out the stracks present in the second list from the first list.
-        remove_duplicate_stracks(stracksa, stracksb): Removes duplicate stracks based on IoU.
+        remove_duplicate_stracks(stracksa, stracksb): Removes duplicate stracks based on IOU.
     """
 
     def __init__(self, args, frame_rate=30):
         """Initialize a YOLOv8 object to track objects with given arguments and frame rate."""
         self.tracked_stracks = []  # type: list[STrack]
         self.lost_stracks = []  # type: list[STrack]
         self.removed_stracks = []  # type: list[STrack]
@@ -369,15 +369,15 @@
         return KalmanFilterXYAH()
 
     def init_track(self, dets, scores, cls, img=None):
         """Initialize object tracking with detections and scores using STrack algorithm."""
         return [STrack(xyxy, s, c) for (xyxy, s, c) in zip(dets, scores, cls)] if len(dets) else []  # detections
 
     def get_dists(self, tracks, detections):
-        """Calculates the distance between tracks and detections using IoU and fuses scores."""
+        """Calculates the distance between tracks and detections using IOU and fuses scores."""
         dists = matching.iou_distance(tracks, detections)
         # TODO: mot20
         # if not self.args.mot20:
         dists = matching.fuse_score(dists, detections)
         return dists
 
     def multi_predict(self, tracks):
@@ -424,15 +424,15 @@
         return list(stracks.values())
         """
         track_ids_b = {t.track_id for t in tlistb}
         return [t for t in tlista if t.track_id not in track_ids_b]
 
     @staticmethod
     def remove_duplicate_stracks(stracksa, stracksb):
-        """Remove duplicate stracks with non-maximum IoU distance."""
+        """Remove duplicate stracks with non-maximum IOU distance."""
         pdist = matching.iou_distance(stracksa, stracksb)
         pairs = np.where(pdist < 0.15)
         dupa, dupb = [], []
         for p, q in zip(*pairs):
             timep = stracksa[p].frame_id - stracksa[p].start_frame
             timeq = stracksb[q].frame_id - stracksb[q].start_frame
             if timep > timeq:
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/trackers/track.py` & `pyppbox-ultralytics-8.1.7/ultralytics/trackers/track.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,50 +27,44 @@
     """
     if hasattr(predictor, "trackers") and persist:
         return
 
     tracker = check_yaml(predictor.args.tracker)
     cfg = IterableSimpleNamespace(**yaml_load(tracker))
 
-    if cfg.tracker_type not in {"bytetrack", "botsort"}:
+    if cfg.tracker_type not in ["bytetrack", "botsort"]:
         raise AssertionError(f"Only 'bytetrack' and 'botsort' are supported for now, but got '{cfg.tracker_type}'")
 
     trackers = []
     for _ in range(predictor.dataset.bs):
         tracker = TRACKER_MAP[cfg.tracker_type](args=cfg, frame_rate=30)
         trackers.append(tracker)
-        if predictor.dataset.mode != "stream":  # only need one tracker for other modes.
-            break
     predictor.trackers = trackers
-    predictor.vid_path = [None] * predictor.dataset.bs  # for determining when to reset tracker on new video
 
 
 def on_predict_postprocess_end(predictor: object, persist: bool = False) -> None:
     """
     Postprocess detected boxes and update with object tracking.
 
     Args:
         predictor (object): The predictor object containing the predictions.
         persist (bool, optional): Whether to persist the trackers if they already exist. Defaults to False.
     """
+    bs = predictor.dataset.bs
     path, im0s = predictor.batch[:2]
 
     is_obb = predictor.args.task == "obb"
-    is_stream = predictor.dataset.mode == "stream"
-    for i in range(len(im0s)):
-        tracker = predictor.trackers[i if is_stream else 0]
-        vid_path = predictor.save_dir / Path(path[i]).name
-        if not persist and predictor.vid_path[i if is_stream else 0] != vid_path:
-            tracker.reset()
-            predictor.vid_path[i if is_stream else 0] = vid_path
+    for i in range(bs):
+        if not persist and predictor.vid_path[i] != str(predictor.save_dir / Path(path[i]).name):  # new video
+            predictor.trackers[i].reset()
 
         det = (predictor.results[i].obb if is_obb else predictor.results[i].boxes).cpu().numpy()
         if len(det) == 0:
             continue
-        tracks = tracker.update(det, im0s[i])
+        tracks = predictor.trackers[i].update(det, im0s[i])
         if len(tracks) == 0:
             continue
         idx = tracks[:, -1].astype(int)
         predictor.results[i] = predictor.results[i][idx]
 
         update_args = dict()
         update_args["obb" if is_obb else "boxes"] = torch.as_tensor(tracks[:, :-1])
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/trackers/utils/gmc.py` & `pyppbox-ultralytics-8.1.7/ultralytics/trackers/utils/gmc.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 
     This class provides methods for tracking and detecting objects based on several tracking algorithms including ORB,
     SIFT, ECC, and Sparse Optical Flow. It also supports downscaling of frames for computational efficiency.
 
     Attributes:
         method (str): The method used for tracking. Options include 'orb', 'sift', 'ecc', 'sparseOptFlow', 'none'.
         downscale (int): Factor by which to downscale the frames for processing.
-        prevFrame (np.ndarray): Stores the previous frame for tracking.
+        prevFrame (np.array): Stores the previous frame for tracking.
         prevKeyPoints (list): Stores the keypoints from the previous frame.
-        prevDescriptors (np.ndarray): Stores the descriptors from the previous frame.
+        prevDescriptors (np.array): Stores the descriptors from the previous frame.
         initializedFirstFrame (bool): Flag to indicate if the first frame has been processed.
 
     Methods:
         __init__(self, method='sparseOptFlow', downscale=2): Initializes a GMC object with the specified method
                                                               and downscale factor.
         apply(self, raw_frame, detections=None): Applies the chosen method to a raw frame and optionally uses
                                                  provided detections.
@@ -78,44 +78,45 @@
         self.initializedFirstFrame = False
 
     def apply(self, raw_frame: np.array, detections: list = None) -> np.array:
         """
         Apply object detection on a raw frame using specified method.
 
         Args:
-            raw_frame (np.ndarray): The raw frame to be processed.
+            raw_frame (np.array): The raw frame to be processed.
             detections (list): List of detections to be used in the processing.
 
         Returns:
-            (np.ndarray): Processed frame.
+            (np.array): Processed frame.
 
         Examples:
             >>> gmc = GMC()
             >>> gmc.apply(np.array([[1, 2, 3], [4, 5, 6]]))
             array([[1, 2, 3],
                    [4, 5, 6]])
         """
-        if self.method in {"orb", "sift"}:
+        if self.method in ["orb", "sift"]:
             return self.applyFeatures(raw_frame, detections)
         elif self.method == "ecc":
-            return self.applyEcc(raw_frame)
+            return self.applyEcc(raw_frame, detections)
         elif self.method == "sparseOptFlow":
-            return self.applySparseOptFlow(raw_frame)
+            return self.applySparseOptFlow(raw_frame, detections)
         else:
             return np.eye(2, 3)
 
-    def applyEcc(self, raw_frame: np.array) -> np.array:
+    def applyEcc(self, raw_frame: np.array, detections: list = None) -> np.array:
         """
         Apply ECC algorithm to a raw frame.
 
         Args:
-            raw_frame (np.ndarray): The raw frame to be processed.
+            raw_frame (np.array): The raw frame to be processed.
+            detections (list): List of detections to be used in the processing.
 
         Returns:
-            (np.ndarray): Processed frame.
+            (np.array): Processed frame.
 
         Examples:
             >>> gmc = GMC()
             >>> gmc.applyEcc(np.array([[1, 2, 3], [4, 5, 6]]))
             array([[1, 2, 3],
                    [4, 5, 6]])
         """
@@ -139,30 +140,30 @@
             self.initializedFirstFrame = True
 
             return H
 
         # Run the ECC algorithm. The results are stored in warp_matrix.
         # (cc, H) = cv2.findTransformECC(self.prevFrame, frame, H, self.warp_mode, self.criteria)
         try:
-            (_, H) = cv2.findTransformECC(self.prevFrame, frame, H, self.warp_mode, self.criteria, None, 1)
+            (cc, H) = cv2.findTransformECC(self.prevFrame, frame, H, self.warp_mode, self.criteria, None, 1)
         except Exception as e:
             LOGGER.warning(f"WARNING: find transform failed. Set warp as identity {e}")
 
         return H
 
     def applyFeatures(self, raw_frame: np.array, detections: list = None) -> np.array:
         """
         Apply feature-based methods like ORB or SIFT to a raw frame.
 
         Args:
-            raw_frame (np.ndarray): The raw frame to be processed.
+            raw_frame (np.array): The raw frame to be processed.
             detections (list): List of detections to be used in the processing.
 
         Returns:
-            (np.ndarray): Processed frame.
+            (np.array): Processed frame.
 
         Examples:
             >>> gmc = GMC()
             >>> gmc.applyFeatures(np.array([[1, 2, 3], [4, 5, 6]]))
             array([[1, 2, 3],
                    [4, 5, 6]])
         """
@@ -253,15 +254,15 @@
         currPoints = np.array(currPoints)
 
         # Draw the keypoint matches on the output image
         # if False:
         #     import matplotlib.pyplot as plt
         #     matches_img = np.hstack((self.prevFrame, frame))
         #     matches_img = cv2.cvtColor(matches_img, cv2.COLOR_GRAY2BGR)
-        #     W = self.prevFrame.shape[1]
+        #     W = np.size(self.prevFrame, 1)
         #     for m in goodMatches:
         #         prev_pt = np.array(self.prevKeyPoints[m.queryIdx].pt, dtype=np.int_)
         #         curr_pt = np.array(keypoints[m.trainIdx].pt, dtype=np.int_)
         #         curr_pt[0] += W
         #         color = np.random.randint(0, 255, 3)
         #         color = (int(color[0]), int(color[1]), int(color[2]))
         #
@@ -270,15 +271,15 @@
         #         matches_img = cv2.circle(matches_img, curr_pt, 2, tuple(color), -1)
         #
         #     plt.figure()
         #     plt.imshow(matches_img)
         #     plt.show()
 
         # Find rigid matrix
-        if prevPoints.shape[0] > 4:
+        if (np.size(prevPoints, 0) > 4) and (np.size(prevPoints, 0) == np.size(prevPoints, 0)):
             H, inliers = cv2.estimateAffinePartial2D(prevPoints, currPoints, cv2.RANSAC)
 
             # Handle downscale
             if self.downscale > 1.0:
                 H[0, 2] *= self.downscale
                 H[1, 2] *= self.downscale
         else:
@@ -287,23 +288,24 @@
         # Store to next iteration
         self.prevFrame = frame.copy()
         self.prevKeyPoints = copy.copy(keypoints)
         self.prevDescriptors = copy.copy(descriptors)
 
         return H
 
-    def applySparseOptFlow(self, raw_frame: np.array) -> np.array:
+    def applySparseOptFlow(self, raw_frame: np.array, detections: list = None) -> np.array:
         """
         Apply Sparse Optical Flow method to a raw frame.
 
         Args:
-            raw_frame (np.ndarray): The raw frame to be processed.
+            raw_frame (np.array): The raw frame to be processed.
+            detections (list): List of detections to be used in the processing.
 
         Returns:
-            (np.ndarray): Processed frame.
+            (np.array): Processed frame.
 
         Examples:
             >>> gmc = GMC()
             >>> gmc.applySparseOptFlow(np.array([[1, 2, 3], [4, 5, 6]]))
             array([[1, 2, 3],
                    [4, 5, 6]])
         """
@@ -315,38 +317,38 @@
         if self.downscale > 1.0:
             frame = cv2.resize(frame, (width // self.downscale, height // self.downscale))
 
         # Find the keypoints
         keypoints = cv2.goodFeaturesToTrack(frame, mask=None, **self.feature_params)
 
         # Handle first frame
-        if not self.initializedFirstFrame or self.prevKeyPoints is None:
+        if not self.initializedFirstFrame:
             self.prevFrame = frame.copy()
             self.prevKeyPoints = copy.copy(keypoints)
             self.initializedFirstFrame = True
             return H
 
         # Find correspondences
-        matchedKeypoints, status, _ = cv2.calcOpticalFlowPyrLK(self.prevFrame, frame, self.prevKeyPoints, None)
+        matchedKeypoints, status, err = cv2.calcOpticalFlowPyrLK(self.prevFrame, frame, self.prevKeyPoints, None)
 
         # Leave good correspondences only
         prevPoints = []
         currPoints = []
 
         for i in range(len(status)):
             if status[i]:
                 prevPoints.append(self.prevKeyPoints[i])
                 currPoints.append(matchedKeypoints[i])
 
         prevPoints = np.array(prevPoints)
         currPoints = np.array(currPoints)
 
         # Find rigid matrix
-        if (prevPoints.shape[0] > 4) and (prevPoints.shape[0] == prevPoints.shape[0]):
-            H, _ = cv2.estimateAffinePartial2D(prevPoints, currPoints, cv2.RANSAC)
+        if np.size(prevPoints, 0) > 4 and np.size(prevPoints, 0) == np.size(prevPoints, 0):
+            H, inliers = cv2.estimateAffinePartial2D(prevPoints, currPoints, cv2.RANSAC)
 
             if self.downscale > 1.0:
                 H[0, 2] *= self.downscale
                 H[1, 2] *= self.downscale
         else:
             LOGGER.warning("WARNING: not enough matching points")
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/trackers/utils/kalman_filter.py` & `pyppbox-ultralytics-8.1.7/ultralytics/trackers/utils/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/trackers/utils/matching.py` & `pyppbox-ultralytics-8.1.7/ultralytics/trackers/utils/matching.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 try:
     import lap  # for linear_assignment
 
     assert lap.__version__  # verify package is not directory
 except (ImportError, AssertionError, AttributeError):
     from ultralytics.utils.checks import check_requirements
 
-    check_requirements("lapx>=0.5.7")  # update to lap package from https://github.com/rathaROG/lapx
+    check_requirements("lapx>=0.5.2")  # update to lap package from https://github.com/rathaROG/lapx
     import lap
 
 
 def linear_assignment(cost_matrix: np.ndarray, thresh: float, use_lap: bool = True) -> tuple:
     """
     Perform linear assignment using scipy or lap.lapjv.
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/utils/__init__.py` & `pyppbox-ultralytics-8.1.7/ultralytics/utils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,26 +26,25 @@
 from ultralytics import __version__
 
 # PyTorch Multi-GPU DDP Constants
 RANK = int(os.getenv("RANK", -1))
 LOCAL_RANK = int(os.getenv("LOCAL_RANK", -1))  # https://pytorch.org/docs/stable/elastic/run.html
 
 # Other Constants
-ARGV = sys.argv or ["", ""]  # sometimes sys.argv = []
 FILE = Path(__file__).resolve()
 ROOT = FILE.parents[1]  # YOLO
 ASSETS = ROOT / "assets"  # default images
 DEFAULT_CFG_PATH = ROOT / "cfg/default.yaml"
 NUM_THREADS = min(8, max(1, os.cpu_count() - 1))  # number of YOLOv5 multiprocessing threads
 AUTOINSTALL = str(os.getenv("YOLO_AUTOINSTALL", True)).lower() == "true"  # global auto-install mode
 VERBOSE = str(os.getenv("YOLO_VERBOSE", True)).lower() == "true"  # global verbose mode
 TQDM_BAR_FORMAT = "{l_bar}{bar:10}{r_bar}" if VERBOSE else None  # tqdm bar format
 LOGGING_NAME = "ultralytics"
 MACOS, LINUX, WINDOWS = (platform.system() == x for x in ["Darwin", "Linux", "Windows"])  # environment booleans
-ARM64 = platform.machine() in {"arm64", "aarch64"}  # ARM64 booleans
+ARM64 = platform.machine() in ("arm64", "aarch64")  # ARM64 booleans
 HELP_MSG = """
     Usage examples for running YOLOv8:
 
     1. Install the ultralytics package:
 
         pip install ultralytics
 
@@ -110,15 +109,15 @@
 
 class TQDM(tqdm_original):
     """
     Custom Ultralytics tqdm class with different default arguments.
 
     Args:
         *args (list): Positional arguments passed to original tqdm.
-        **kwargs (any): Keyword arguments, with custom defaults applied.
+        **kwargs (dict): Keyword arguments, with custom defaults applied.
     """
 
     def __init__(self, *args, **kwargs):
         """
         Initialize custom Ultralytics tqdm class with different default arguments.
 
         Note these can still be overridden when calling TQDM.
@@ -209,15 +208,15 @@
 
     def decorator(func):
         """Decorator to apply temporary rc parameters and backend to a function."""
 
         def wrapper(*args, **kwargs):
             """Sets rc parameters and backend, calls the original function, and restores the settings."""
             original_backend = plt.get_backend()
-            if backend.lower() != original_backend.lower():
+            if backend != original_backend:
                 plt.close("all")  # auto-close()ing of figures upon backend switching is deprecated since 3.8
                 plt.switch_backend(backend)
 
             with plt.rc_context(rcparams):
                 result = func(*args, **kwargs)
 
             if backend != original_backend:
@@ -226,50 +225,45 @@
             return result
 
         return wrapper
 
     return decorator
 
 
-def set_logging(name="LOGGING_NAME", verbose=True):
-    """Sets up logging for the given name with UTF-8 encoding support, ensuring compatibility across different
-    environments.
-    """
+def set_logging(name=LOGGING_NAME, verbose=True):
+    """Sets up logging for the given name with UTF-8 encoding support."""
     level = logging.INFO if verbose and RANK in {-1, 0} else logging.ERROR  # rank in world for Multi-GPU trainings
 
-    # Configure the console (stdout) encoding to UTF-8, with checks for compatibility
+    # Configure the console (stdout) encoding to UTF-8
     formatter = logging.Formatter("%(message)s")  # Default formatter
-    if WINDOWS and hasattr(sys.stdout, "encoding") and sys.stdout.encoding != "utf-8":
-
-        class CustomFormatter(logging.Formatter):
-            def format(self, record):
-                """Sets up logging with UTF-8 encoding and configurable verbosity."""
-                return emojis(super().format(record))
-
+    if WINDOWS and sys.stdout.encoding != "utf-8":
         try:
-            # Attempt to reconfigure stdout to use UTF-8 encoding if possible
             if hasattr(sys.stdout, "reconfigure"):
                 sys.stdout.reconfigure(encoding="utf-8")
-            # For environments where reconfigure is not available, wrap stdout in a TextIOWrapper
             elif hasattr(sys.stdout, "buffer"):
                 import io
 
                 sys.stdout = io.TextIOWrapper(sys.stdout.buffer, encoding="utf-8")
             else:
-                formatter = CustomFormatter("%(message)s")
+                sys.stdout.encoding = "utf-8"
         except Exception as e:
             print(f"Creating custom formatter for non UTF-8 environments due to {e}")
-            formatter = CustomFormatter("%(message)s")
 
-    # Create and configure the StreamHandler with the appropriate formatter and level
+            class CustomFormatter(logging.Formatter):
+                def format(self, record):
+                    """Sets up logging with UTF-8 encoding and configurable verbosity."""
+                    return emojis(super().format(record))
+
+            formatter = CustomFormatter("%(message)s")  # Use CustomFormatter to eliminate UTF-8 output as last recourse
+
+    # Create and configure the StreamHandler
     stream_handler = logging.StreamHandler(sys.stdout)
     stream_handler.setFormatter(formatter)
     stream_handler.setLevel(level)
 
-    # Set up the logger
     logger = logging.getLogger(name)
     logger.setLevel(level)
     logger.addHandler(stream_handler)
     logger.propagate = False
     return logger
 
 
@@ -360,15 +354,15 @@
     Args:
         file (str, optional): File name. Default is 'data.yaml'.
         append_filename (bool): Add the YAML filename to the YAML dictionary. Default is False.
 
     Returns:
         (dict): YAML data and file name.
     """
-    assert Path(file).suffix in {".yaml", ".yml"}, f"Attempting to load non-YAML file {file} with yaml_load()"
+    assert Path(file).suffix in (".yaml", ".yml"), f"Attempting to load non-YAML file {file} with yaml_load()"
     with open(file, errors="ignore", encoding="utf-8") as f:
         s = f.read()  # string
 
         # Remove special characters
         if not s.isprintable():
             s = re.sub(r"[^\x09\x0A\x0D\x20-\x7E\x85\xA0-\uD7FF\uE000-\uFFFD\U00010000-\U0010ffff]+", "", s)
 
@@ -524,15 +518,15 @@
 def is_pytest_running():
     """
     Determines whether pytest is currently running or not.
 
     Returns:
         (bool): True if pytest is running, False otherwise.
     """
-    return ("PYTEST_CURRENT_TEST" in os.environ) or ("pytest" in sys.modules) or ("pytest" in Path(ARGV[0]).stem)
+    return ("PYTEST_CURRENT_TEST" in os.environ) or ("pytest" in sys.modules) or ("pytest" in Path(sys.argv[0]).stem)
 
 
 def is_github_action_running() -> bool:
     """
     Determine if the current environment is a GitHub Actions runner.
 
     Returns:
@@ -785,15 +779,14 @@
         self.delay = delay
         self._attempts = 0
 
     def __call__(self, func):
         """Decorator implementation for Retry with exponential backoff."""
 
         def wrapped_func(*args, **kwargs):
-            """Applies retries to the decorated function or method."""
             self._attempts = 0
             while self._attempts < self.times:
                 try:
                     return func(*args, **kwargs)
                 except Exception as e:
                     self._attempts += 1
                     print(f"Retry {self._attempts}/{self.times} failed: {e}")
@@ -867,29 +860,29 @@
             hint (dict): A dictionary containing additional information about the error.
 
         Returns:
             dict: The modified event or None if the event should not be sent to Sentry.
         """
         if "exc_info" in hint:
             exc_type, exc_value, tb = hint["exc_info"]
-            if exc_type in {KeyboardInterrupt, FileNotFoundError} or "out of memory" in str(exc_value):
+            if exc_type in (KeyboardInterrupt, FileNotFoundError) or "out of memory" in str(exc_value):
                 return None  # do not send event
 
         event["tags"] = {
-            "sys_argv": ARGV[0],
-            "sys_argv_name": Path(ARGV[0]).name,
+            "sys_argv": sys.argv[0],
+            "sys_argv_name": Path(sys.argv[0]).name,
             "install": "git" if is_git_dir() else "pip" if is_pip_package() else "other",
             "os": ENVIRONMENT,
         }
         return event
 
     if (
         SETTINGS["sync"]
-        and RANK in {-1, 0}
-        and Path(ARGV[0]).name == "yolo"
+        and RANK in (-1, 0)
+        and Path(sys.argv[0]).name == "yolo"
         and not TESTS_RUNNING
         and ONLINE
         and is_pip_package()
         and not is_git_dir()
     ):
         # If sentry_sdk package is not installed then return and do not use Sentry
         try:
@@ -960,33 +953,23 @@
             if not self.file.exists():
                 self.save()
 
             self.load()
             correct_keys = self.keys() == self.defaults.keys()
             correct_types = all(type(a) is type(b) for a, b in zip(self.values(), self.defaults.values()))
             correct_version = check_version(self["settings_version"], self.version)
-            help_msg = (
-                f"\nView settings with 'yolo settings' or at '{self.file}'"
-                "\nUpdate settings with 'yolo settings key=value', i.e. 'yolo settings runs_dir=path/to/dir'. "
-                "For help see https://docs.ultralytics.com/quickstart/#ultralytics-settings."
-            )
             if not (correct_keys and correct_types and correct_version):
                 LOGGER.warning(
                     "WARNING ⚠️ Ultralytics settings reset to default values. This may be due to a possible problem "
-                    f"with your settings or a recent ultralytics package update. {help_msg}"
+                    "with your settings or a recent ultralytics package update. "
+                    f"\nView settings with 'yolo settings' or at '{self.file}'"
+                    "\nUpdate settings with 'yolo settings key=value', i.e. 'yolo settings runs_dir=path/to/dir'."
                 )
                 self.reset()
 
-            if self.get("datasets_dir") == self.get("runs_dir"):
-                LOGGER.warning(
-                    f"WARNING ⚠️ Ultralytics setting 'datasets_dir: {self.get('datasets_dir')}' "
-                    f"must be different than 'runs_dir: {self.get('runs_dir')}'. "
-                    f"Please change one to avoid possible issues during training. {help_msg}"
-                )
-
     def load(self):
         """Loads settings from the YAML file."""
         super().update(yaml_load(self.file))
 
     def save(self):
         """Saves the current settings to the YAML file."""
         yaml_save(self.file, dict(self))
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/utils/autobatch.py` & `pyppbox-ultralytics-8.1.7/ultralytics/utils/autobatch.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/utils/benchmarks.py` & `pyppbox-ultralytics-8.1.7/ultralytics/utils/benchmarks.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,30 +17,30 @@
 CoreML                  | `coreml`                  | yolov8n.mlpackage
 TensorFlow SavedModel   | `saved_model`             | yolov8n_saved_model/
 TensorFlow GraphDef     | `pb`                      | yolov8n.pb
 TensorFlow Lite         | `tflite`                  | yolov8n.tflite
 TensorFlow Edge TPU     | `edgetpu`                 | yolov8n_edgetpu.tflite
 TensorFlow.js           | `tfjs`                    | yolov8n_web_model/
 PaddlePaddle            | `paddle`                  | yolov8n_paddle_model/
-NCNN                    | `ncnn`                    | yolov8n_ncnn_model/
+ncnn                    | `ncnn`                    | yolov8n_ncnn_model/
 """
 
 import glob
 import platform
 import time
 from pathlib import Path
 
 import numpy as np
 import torch.cuda
 
-from ultralytics import YOLO, YOLOWorld
+from ultralytics import YOLO
 from ultralytics.cfg import TASK2DATA, TASK2METRIC
 from ultralytics.engine.exporter import export_formats
 from ultralytics.utils import ASSETS, LINUX, LOGGER, MACOS, TQDM, WEIGHTS_DIR
-from ultralytics.utils.checks import IS_PYTHON_3_12, check_requirements, check_yolo
+from ultralytics.utils.checks import check_requirements, check_yolo
 from ultralytics.utils.files import file_size
 from ultralytics.utils.torch_utils import select_device
 
 
 def benchmark(
     model=WEIGHTS_DIR / "yolov8n.pt", data=None, imgsz=160, half=False, int8=False, device="cpu", verbose=False
 ):
@@ -80,28 +80,20 @@
 
     y = []
     t0 = time.time()
     for i, (name, format, suffix, cpu, gpu) in export_formats().iterrows():  # index, (name, format, suffix, CPU, GPU)
         emoji, filename = "❌", None  # export defaults
         try:
             # Checks
-            if i == 9:  # Edge TPU
+            if i == 9:
                 assert LINUX, "Edge TPU export only supported on Linux"
-            elif i == 7:  # TF GraphDef
+            elif i == 7:
                 assert model.task != "obb", "TensorFlow GraphDef not supported for OBB task"
             elif i in {5, 10}:  # CoreML and TF.js
                 assert MACOS or LINUX, "export only supported on macOS and Linux"
-            if i in {3, 5}:  # CoreML and OpenVINO
-                assert not IS_PYTHON_3_12, "CoreML and OpenVINO not supported on Python 3.12"
-            if i in {6, 7, 8, 9, 10}:  # All TF formats
-                assert not isinstance(model, YOLOWorld), "YOLOWorldv2 TensorFlow exports not supported by onnx2tf yet"
-            if i in {11}:  # Paddle
-                assert not isinstance(model, YOLOWorld), "YOLOWorldv2 Paddle exports not supported yet"
-            if i in {12}:  # NCNN
-                assert not isinstance(model, YOLOWorld), "YOLOWorldv2 NCNN exports not supported yet"
             if "cpu" in device.type:
                 assert cpu, "inference not supported on CPU"
             if "cuda" in device.type:
                 assert gpu, "inference not supported on GPU"
 
             # Export
             if format == "-":
@@ -111,15 +103,15 @@
                 filename = model.export(imgsz=imgsz, format=format, half=half, int8=int8, device=device, verbose=False)
                 exported_model = YOLO(filename, task=model.task)
                 assert suffix in str(filename), "export failed"
             emoji = "❎"  # indicates export succeeded
 
             # Predict
             assert model.task != "pose" or i != 7, "GraphDef Pose inference is not supported"
-            assert i not in {9, 10}, "inference not supported"  # Edge TPU and TF.js are unsupported
+            assert i not in (9, 10), "inference not supported"  # Edge TPU and TF.js are unsupported
             assert i != 5 or platform.system() == "Darwin", "inference only supported on macOS>=10.13"  # CoreML
             exported_model.predict(ASSETS / "bus.jpg", imgsz=imgsz, device=device, half=half)
 
             # Validate
             data = data or TASK2DATA[model.task]  # task to dataset, i.e. coco8.yaml for task=detect
             key = TASK2METRIC[model.task]  # task to metric, i.e. metrics/mAP50-95(B) for task=detect
             results = exported_model.val(
@@ -151,15 +143,16 @@
     return df
 
 
 class ProfileModels:
     """
     ProfileModels class for profiling different models on ONNX and TensorRT.
 
-    This class profiles the performance of different models, returning results such as model speed and FLOPs.
+    This class profiles the performance of different models, provided their paths. The profiling includes parameters such as
+    model speed and FLOPs.
 
     Attributes:
         paths (list): Paths of the models to profile.
         num_timed_runs (int): Number of timed runs for the profiling. Default is 100.
         num_warmup_runs (int): Number of warmup runs before profiling. Default is 10.
         min_time (float): Minimum number of seconds to profile for. Default is 60.
         imgsz (int): Image size used in the models. Default is 640.
@@ -191,17 +184,17 @@
 
         Args:
             paths (list): List of paths of the models to be profiled.
             num_timed_runs (int, optional): Number of timed runs for the profiling. Default is 100.
             num_warmup_runs (int, optional): Number of warmup runs before the actual profiling starts. Default is 10.
             min_time (float, optional): Minimum time in seconds for profiling a model. Default is 60.
             imgsz (int, optional): Size of the image used during profiling. Default is 640.
-            half (bool, optional): Flag to indicate whether to use half-precision floating point for profiling.
+            half (bool, optional): Flag to indicate whether to use half-precision floating point for profiling. Default is True.
             trt (bool, optional): Flag to indicate whether to profile using TensorRT. Default is True.
-            device (torch.device, optional): Device used for profiling. If None, it is determined automatically.
+            device (torch.device, optional): Device used for profiling. If None, it is determined automatically. Default is None.
         """
         self.paths = paths
         self.num_timed_runs = num_timed_runs
         self.num_warmup_runs = num_warmup_runs
         self.min_time = min_time
         self.imgsz = imgsz
         self.half = half
@@ -216,15 +209,15 @@
             print("No matching *.pt or *.onnx files found.")
             return
 
         table_rows = []
         output = []
         for file in files:
             engine_file = file.with_suffix(".engine")
-            if file.suffix in {".pt", ".yaml", ".yml"}:
+            if file.suffix in (".pt", ".yaml", ".yml"):
                 model = YOLO(str(file))
                 model.fuse()  # to report correct params and GFLOPs in model.info()
                 model_info = model.info()
                 if self.trt and self.device.type != "cpu" and not engine_file.is_file():
                     engine_file = model.export(
                         format="engine", half=self.half, imgsz=self.imgsz, device=self.device, verbose=False
                     )
@@ -263,16 +256,15 @@
 
     def get_onnx_model_info(self, onnx_file: str):
         """Retrieves the information including number of layers, parameters, gradients and FLOPs for an ONNX model
         file.
         """
         return 0.0, 0.0, 0.0, 0.0  # return (num_layers, num_params, num_gradients, num_flops)
 
-    @staticmethod
-    def iterative_sigma_clipping(data, sigma=2, max_iters=3):
+    def iterative_sigma_clipping(self, data, sigma=2, max_iters=3):
         """Applies an iterative sigma clipping algorithm to the given data times number of iterations."""
         data = np.array(data)
         for _ in range(max_iters):
             mean, std = np.mean(data), np.std(data)
             clipped_data = data[(data > mean - sigma * std) & (data < mean + sigma * std)]
             if len(clipped_data) == len(data):
                 break
@@ -362,41 +354,30 @@
 
         run_times = self.iterative_sigma_clipping(np.array(run_times), sigma=2, max_iters=5)  # sigma clipping
         return np.mean(run_times), np.std(run_times)
 
     def generate_table_row(self, model_name, t_onnx, t_engine, model_info):
         """Generates a formatted string for a table row that includes model performance and metric details."""
         layers, params, gradients, flops = model_info
-        return (
-            f"| {model_name:18s} | {self.imgsz} | - | {t_onnx[0]:.2f} ± {t_onnx[1]:.2f} ms | {t_engine[0]:.2f} ± "
-            f"{t_engine[1]:.2f} ms | {params / 1e6:.1f} | {flops:.1f} |"
-        )
+        return f"| {model_name:18s} | {self.imgsz} | - | {t_onnx[0]:.2f} ± {t_onnx[1]:.2f} ms | {t_engine[0]:.2f} ± {t_engine[1]:.2f} ms | {params / 1e6:.1f} | {flops:.1f} |"
 
-    @staticmethod
-    def generate_results_dict(model_name, t_onnx, t_engine, model_info):
+    def generate_results_dict(self, model_name, t_onnx, t_engine, model_info):
         """Generates a dictionary of model details including name, parameters, GFLOPS and speed metrics."""
         layers, params, gradients, flops = model_info
         return {
             "model/name": model_name,
             "model/parameters": params,
             "model/GFLOPs": round(flops, 3),
             "model/speed_ONNX(ms)": round(t_onnx[0], 3),
             "model/speed_TensorRT(ms)": round(t_engine[0], 3),
         }
 
-    @staticmethod
-    def print_table(table_rows):
+    def print_table(self, table_rows):
         """Formats and prints a comparison table for different models with given statistics and performance data."""
         gpu = torch.cuda.get_device_name(0) if torch.cuda.is_available() else "GPU"
-        header = (
-            f"| Model | size<br><sup>(pixels) | mAP<sup>val<br>50-95 | Speed<br><sup>CPU ONNX<br>(ms) | "
-            f"Speed<br><sup>{gpu} TensorRT<br>(ms) | params<br><sup>(M) | FLOPs<br><sup>(B) |"
-        )
-        separator = (
-            "|-------------|---------------------|--------------------|------------------------------|"
-            "-----------------------------------|------------------|-----------------|"
-        )
+        header = f"| Model | size<br><sup>(pixels) | mAP<sup>val<br>50-95 | Speed<br><sup>CPU ONNX<br>(ms) | Speed<br><sup>{gpu} TensorRT<br>(ms) | params<br><sup>(M) | FLOPs<br><sup>(B) |"
+        separator = "|-------------|---------------------|--------------------|------------------------------|-----------------------------------|------------------|-----------------|"
 
         print(f"\n\n{header}")
         print(separator)
         for row in table_rows:
             print(row)
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/utils/callbacks/base.py` & `pyppbox-ultralytics-8.1.7/ultralytics/utils/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/utils/callbacks/clearml.py` & `pyppbox-ultralytics-8.1.7/ultralytics/utils/callbacks/clearml.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/utils/callbacks/comet.py` & `pyppbox-ultralytics-8.1.7/ultralytics/utils/callbacks/comet.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         return comet_ml.OfflineExperiment(project_name=project_name)
 
     return comet_ml.Experiment(project_name=project_name)
 
 
 def _create_experiment(args):
     """Ensures that the experiment object is only created in a single process during distributed training."""
-    if RANK not in {-1, 0}:
+    if RANK not in (-1, 0):
         return
     try:
         comet_mode = _get_comet_mode()
         _project_name = os.getenv("COMET_PROJECT_NAME", args.project)
         experiment = _get_experiment_type(comet_mode, _project_name)
         experiment.log_parameters(vars(args))
         experiment.log_others(
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/utils/callbacks/dvc.py` & `pyppbox-ultralytics-8.1.7/ultralytics/utils/callbacks/dvc.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/utils/callbacks/hub.py` & `pyppbox-ultralytics-8.1.7/ultralytics/utils/callbacks/hub.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,33 +29,28 @@
         }
         if trainer.epoch == 0:
             from ultralytics.utils.torch_utils import model_info_for_loggers
 
             all_plots = {**all_plots, **model_info_for_loggers(trainer)}
 
         session.metrics_queue[trainer.epoch] = json.dumps(all_plots)
-
-        # If any metrics fail to upload, add them to the queue to attempt uploading again.
-        if session.metrics_upload_failed_queue:
-            session.metrics_queue.update(session.metrics_upload_failed_queue)
-
         if time() - session.timers["metrics"] > session.rate_limits["metrics"]:
             session.upload_metrics()
             session.timers["metrics"] = time()  # reset timer
             session.metrics_queue = {}  # reset queue
 
 
 def on_model_save(trainer):
     """Saves checkpoints to Ultralytics HUB with rate limiting."""
     session = getattr(trainer, "hub_session", None)
     if session:
         # Upload checkpoints with rate limiting
         is_best = trainer.best_fitness == trainer.fitness
         if time() - session.timers["ckpt"] > session.rate_limits["ckpt"]:
-            LOGGER.info(f"{PREFIX}Uploading checkpoint {HUB_WEB_ROOT}/models/{session.model.id}")
+            LOGGER.info(f"{PREFIX}Uploading checkpoint {HUB_WEB_ROOT}/models/{session.model_id}")
             session.upload_model(trainer.epoch, trainer.last, is_best)
             session.timers["ckpt"] = time()  # reset timer
 
 
 def on_train_end(trainer):
     """Upload final model and metrics to Ultralytics HUB at the end of training."""
     session = getattr(trainer, "hub_session", None)
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/utils/callbacks/mlflow.py` & `pyppbox-ultralytics-8.1.7/ultralytics/utils/callbacks/mlflow.py`

 * *Files 10% similar despite different names*

```diff
@@ -54,15 +54,14 @@
     Global:
         mlflow: The imported mlflow module to use for logging.
 
     Environment Variables:
         MLFLOW_TRACKING_URI: The URI for MLflow tracking. If not set, defaults to 'runs/mlflow'.
         MLFLOW_EXPERIMENT_NAME: The name of the MLflow experiment. If not set, defaults to trainer.args.project.
         MLFLOW_RUN: The name of the MLflow run. If not set, defaults to trainer.args.name.
-        MLFLOW_KEEP_RUN_ACTIVE: Boolean indicating whether to keep the MLflow run active after the end of the training phase.
     """
     global mlflow
 
     uri = os.environ.get("MLFLOW_TRACKING_URI") or str(RUNS_DIR / "mlflow")
     LOGGER.debug(f"{PREFIX} tracking uri: {uri}")
     mlflow.set_tracking_uri(uri)
 
@@ -83,20 +82,17 @@
         LOGGER.warning(f"{PREFIX}WARNING ⚠️ Failed to initialize: {e}\n" f"{PREFIX}WARNING ⚠️ Not tracking this run")
 
 
 def on_train_epoch_end(trainer):
     """Log training metrics at the end of each train epoch to MLflow."""
     if mlflow:
         mlflow.log_metrics(
-            metrics={
-                **SANITIZE(trainer.lr),
-                **SANITIZE(trainer.label_loss_items(trainer.tloss, prefix="train")),
-            },
-            step=trainer.epoch,
+            metrics=SANITIZE(trainer.label_loss_items(trainer.tloss, prefix="train")), step=trainer.epoch
         )
+        mlflow.log_metrics(metrics=SANITIZE(trainer.lr), step=trainer.epoch)
 
 
 def on_fit_epoch_end(trainer):
     """Log training metrics at the end of each fit epoch to MLflow."""
     if mlflow:
         mlflow.log_metrics(metrics=SANITIZE(trainer.metrics), step=trainer.epoch)
 
@@ -104,30 +100,24 @@
 def on_train_end(trainer):
     """Log model artifacts at the end of the training."""
     if mlflow:
         mlflow.log_artifact(str(trainer.best.parent))  # log save_dir/weights directory with best.pt and last.pt
         for f in trainer.save_dir.glob("*"):  # log all other files in save_dir
             if f.suffix in {".png", ".jpg", ".csv", ".pt", ".yaml"}:
                 mlflow.log_artifact(str(f))
-        keep_run_active = os.environ.get("MLFLOW_KEEP_RUN_ACTIVE", "False").lower() == "true"
-        if keep_run_active:
-            LOGGER.info(f"{PREFIX}mlflow run still alive, remember to close it using mlflow.end_run()")
-        else:
-            mlflow.end_run()
-            LOGGER.debug(f"{PREFIX}mlflow run ended")
 
+        mlflow.end_run()
         LOGGER.info(
             f"{PREFIX}results logged to {mlflow.get_tracking_uri()}\n"
             f"{PREFIX}disable with 'yolo settings mlflow=False'"
         )
 
 
 callbacks = (
     {
         "on_pretrain_routine_end": on_pretrain_routine_end,
-        "on_train_epoch_end": on_train_epoch_end,
         "on_fit_epoch_end": on_fit_epoch_end,
         "on_train_end": on_train_end,
     }
     if mlflow
     else {}
 )
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/utils/callbacks/neptune.py` & `pyppbox-ultralytics-8.1.7/ultralytics/utils/callbacks/neptune.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/utils/callbacks/raytune.py` & `pyppbox-ultralytics-8.1.7/ultralytics/utils/callbacks/raytune.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 except (ImportError, AssertionError):
     tune = None
 
 
 def on_fit_epoch_end(trainer):
     """Sends training metrics to Ray Tune at end of each epoch."""
-    if ray.train._internal.session._get_session():  # replacement for deprecated ray.tune.is_session_enabled()
+    if ray.tune.is_session_enabled():
         metrics = trainer.metrics
         metrics["epoch"] = trainer.epoch
         session.report(metrics)
 
 
 callbacks = (
     {
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/utils/callbacks/tensorboard.py` & `pyppbox-ultralytics-8.1.7/ultralytics/utils/callbacks/tensorboard.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,15 +41,14 @@
 
     with warnings.catch_warnings():
         warnings.simplefilter("ignore", category=UserWarning)  # suppress jit trace warning
         warnings.simplefilter("ignore", category=torch.jit.TracerWarning)  # suppress jit trace warning
 
         # Try simple method first (YOLO)
         with contextlib.suppress(Exception):
-            trainer.model.eval()  # place in .eval() mode to avoid BatchNorm statistics changes
             WRITER.add_graph(torch.jit.trace(de_parallel(trainer.model), im, strict=False), [])
             LOGGER.info(f"{PREFIX}model graph visualization added ✅")
             return
 
         # Fallback to TorchScript export steps (RTDETR)
         try:
             model = deepcopy(de_parallel(trainer.model))
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/utils/callbacks/wb.py` & `pyppbox-ultralytics-8.1.7/ultralytics/utils/callbacks/wb.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,17 +19,16 @@
     wb = None
 
 
 def _custom_table(x, y, classes, title="Precision Recall Curve", x_title="Recall", y_title="Precision"):
     """
     Create and log a custom metric visualization to wandb.plot.pr_curve.
 
-    This function crafts a custom metric visualization that mimics the behavior of wandb's default precision-recall
-    curve while allowing for enhanced customization. The visual metric is useful for monitoring model performance across
-    different classes.
+    This function crafts a custom metric visualization that mimics the behavior of wandb's default precision-recall curve
+    while allowing for enhanced customization. The visual metric is useful for monitoring model performance across different classes.
 
     Args:
         x (List): Values for the x-axis; expected to have length N.
         y (List): Corresponding values for the y-axis; also expected to have length N.
         classes (List): Labels identifying the class of each point; length N.
         title (str, optional): Title for the plot; defaults to 'Precision Recall Curve'.
         x_title (str, optional): Label for the x-axis; defaults to 'Recall'.
@@ -61,16 +60,16 @@
     Log a metric curve visualization.
 
     This function generates a metric curve based on input data and logs the visualization to wandb.
     The curve can represent aggregated data (mean) or individual class data, depending on the 'only_mean' flag.
 
     Args:
         x (np.ndarray): Data points for the x-axis with length N.
-        y (np.ndarray): Corresponding data points for the y-axis with shape CxN, where C is the number of classes.
-        names (list, optional): Names of the classes corresponding to the y-axis data; length C. Defaults to [].
+        y (np.ndarray): Corresponding data points for the y-axis with shape CxN, where C represents the number of classes.
+        names (list, optional): Names of the classes corresponding to the y-axis data; length C. Defaults to an empty list.
         id (str, optional): Unique identifier for the logged data in wandb. Defaults to 'precision-recall'.
         title (str, optional): Title for the visualization plot. Defaults to 'Precision Recall Curve'.
         x_title (str, optional): Label for the x-axis. Defaults to 'Recall'.
         y_title (str, optional): Label for the y-axis. Defaults to 'Precision'.
         num_x (int, optional): Number of interpolated data points for visualization. Defaults to 100.
         only_mean (bool, optional): Flag to indicate if only the mean curve should be plotted. Defaults to True.
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/utils/checks.py` & `pyppbox-ultralytics-8.1.7/ultralytics/utils/checks.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import inspect
 import math
 import os
 import platform
 import re
 import shutil
 import subprocess
+import sys
 import time
 from importlib import metadata
 from pathlib import Path
 from typing import Optional
 
 import cv2
 import numpy as np
@@ -24,15 +25,14 @@
     ASSETS,
     AUTOINSTALL,
     LINUX,
     LOGGER,
     ONLINE,
     ROOT,
     USER_CONFIG_DIR,
-    Retry,
     SimpleNamespace,
     ThreadingLocked,
     TryExcept,
     clean_url,
     colorstr,
     downloads,
     emojis,
@@ -42,16 +42,14 @@
     is_jupyter,
     is_kaggle,
     is_online,
     is_pip_package,
     url2file,
 )
 
-PYTHON_VERSION = platform.python_version()
-
 
 def parse_requirements(file_path=ROOT.parent / "requirements.txt", package=""):
     """
     Parse a requirements.txt file, ignoring lines that start with '#' and any text after '#'.
 
     Args:
         file_path (Path): Path to the requirements.txt file.
@@ -139,16 +137,14 @@
     stride = int(stride.max() if isinstance(stride, torch.Tensor) else stride)
 
     # Convert image size to list if it is an integer
     if isinstance(imgsz, int):
         imgsz = [imgsz]
     elif isinstance(imgsz, (list, tuple)):
         imgsz = list(imgsz)
-    elif isinstance(imgsz, str):  # i.e. '640' or '[640,640]'
-        imgsz = [int(imgsz)] if imgsz.isnumeric() else eval(imgsz)
     else:
         raise TypeError(
             f"'imgsz={imgsz}' is of invalid type {type(imgsz).__name__}. "
             f"Valid imgsz types are int i.e. 'imgsz=640' or list i.e. 'imgsz=[640,640]'"
         )
 
     # Apply max_dim
@@ -234,15 +230,15 @@
     for r in required.strip(",").split(","):
         op, version = re.match(r"([^0-9]*)([\d.]+)", r).groups()  # split '>=22.04' -> ('>=', '22.04')
         v = parse_version(version)  # '1.2.3' -> (1, 2, 3)
         if op == "==" and c != v:
             result = False
         elif op == "!=" and c == v:
             result = False
-        elif op in {">=", ""} and not (c >= v):  # if no constraint passed assume '>=required'
+        elif op in (">=", "") and not (c >= v):  # if no constraint passed assume '>=required'
             result = False
         elif op == "<=" and not (c <= v):
             result = False
         elif op == ">" and not (c > v):
             result = False
         elif op == "<" and not (c < v):
             result = False
@@ -320,30 +316,30 @@
     # Check system fonts
     matches = [s for s in font_manager.findSystemFonts() if font in s]
     if any(matches):
         return matches[0]
 
     # Download to USER_CONFIG_DIR if missing
     url = f"https://ultralytics.com/assets/{name}"
-    if downloads.is_url(url, check=True):
+    if downloads.is_url(url):
         downloads.safe_download(url=url, file=file)
         return file
 
 
 def check_python(minimum: str = "3.8.0") -> bool:
     """
     Check current python version against the required minimum version.
 
     Args:
         minimum (str): Required minimum version of python.
 
     Returns:
         (bool): Whether the installed Python version meets the minimum constraints.
     """
-    return check_version(PYTHON_VERSION, minimum, name="Python ", hard=True)
+    return check_version(platform.python_version(), minimum, name="Python ", hard=True)
 
 
 @TryExcept()
 def check_requirements(requirements=ROOT.parent / "requirements.txt", exclude=(), install=True, cmds=""):
     """
     Check if installed dependencies meet YOLOv8 requirements and attempt to auto-update if needed.
 
@@ -393,16 +389,15 @@
     if s:
         if install and AUTOINSTALL:  # check environment variable
             n = len(pkgs)  # number of packages updates
             LOGGER.info(f"{prefix} Ultralytics requirement{'s' * (n > 1)} {pkgs} not found, attempting AutoUpdate...")
             try:
                 t = time.time()
                 assert is_online(), "AutoUpdate skipped (offline)"
-                with Retry(times=2, delay=1):  # run up to 2 times with 1-second retry delay
-                    LOGGER.info(subprocess.check_output(f"pip install --no-cache {s} {cmds}", shell=True).decode())
+                LOGGER.info(subprocess.check_output(f"pip install --no-cache {s} {cmds}", shell=True).decode())
                 dt = time.time() - t
                 LOGGER.info(
                     f"{prefix} AutoUpdate success ✅ {dt:.1f}s, installed {n} package{'s' * (n > 1)}: {pkgs}\n"
                     f"{prefix} ⚠️ {colorstr('bold', 'Restart runtime or rerun command for updates to take effect')}\n"
                 )
             except Exception as e:
                 LOGGER.warning(f"{prefix} ❌ {e}")
@@ -499,15 +494,15 @@
         file = url2file(file)  # '%2F' to '/', split https://url.com/file.txt?auth
         if Path(file).exists():
             LOGGER.info(f"Found {clean_url(url)} locally at {file}")  # file already exists
         else:
             downloads.safe_download(url=url, file=file, unzip=False)
         return file
     else:  # search
-        files = glob.glob(str(ROOT / "**" / file), recursive=True) or glob.glob(str(ROOT.parent / file))  # find file
+        files = glob.glob(str(ROOT / "cfg" / "**" / file), recursive=True)  # find file
         if not files and hard:
             raise FileNotFoundError(f"'{file}' does not exist")
         elif len(files) > 1 and hard:
             raise FileNotFoundError(f"Multiple files match '{file}', specify exact path: {files}")
         return files[0] if len(files) else []  # return file
 
 
@@ -587,15 +582,15 @@
     from ultralytics.utils.torch_utils import get_cpu_info
 
     ram_info = psutil.virtual_memory().total / (1024**3)  # Convert bytes to GB
     check_yolo()
     LOGGER.info(
         f"\n{'OS':<20}{platform.platform()}\n"
         f"{'Environment':<20}{ENVIRONMENT}\n"
-        f"{'Python':<20}{PYTHON_VERSION}\n"
+        f"{'Python':<20}{sys.version.split()[0]}\n"
         f"{'Install':<20}{'git' if is_git_dir() else 'pip' if is_pip_package() else 'other'}\n"
         f"{'RAM':<20}{ram_info:.2f} GB\n"
         f"{'CPU':<20}{get_cpu_info()}\n"
         f"{'CUDA':<20}{torch.version.cuda if torch and torch.cuda.is_available() else None}\n"
     )
 
     for r in parse_requirements(package="ultralytics"):
@@ -636,15 +631,15 @@
         check_amp(model)
         ```
 
     Returns:
         (bool): Returns True if the AMP functionality works correctly with YOLOv8 model, else False.
     """
     device = next(model.parameters()).device  # get model device
-    if device.type in {"cpu", "mps"}:
+    if device.type in ("cpu", "mps"):
         return False  # AMP only used on CUDA devices
 
     def amp_allclose(m, im):
         """All close FP32 vs AMP results."""
         a = m(im, device=device, verbose=False)[0].boxes.data  # FP32 inference
         with torch.cuda.amp.autocast(True):
             b = m(im, device=device, verbose=False)[0].boxes.data  # AMP inference
@@ -729,11 +724,7 @@
     """
     Check if CUDA is available in the environment.
 
     Returns:
         (bool): True if one or more NVIDIA GPUs are available, False otherwise.
     """
     return cuda_device_count() > 0
-
-
-# Define constants
-IS_PYTHON_3_12 = PYTHON_VERSION.startswith("3.12")
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/utils/dist.py` & `pyppbox-ultralytics-8.1.7/ultralytics/utils/dist.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/utils/downloads.py` & `pyppbox-ultralytics-8.1.7/ultralytics/utils/downloads.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,38 +16,34 @@
 
 # Define Ultralytics GitHub assets maintained at https://github.com/ultralytics/assets
 GITHUB_ASSETS_REPO = "ultralytics/assets"
 GITHUB_ASSETS_NAMES = (
     [f"yolov8{k}{suffix}.pt" for k in "nsmlx" for suffix in ("", "-cls", "-seg", "-pose", "-obb")]
     + [f"yolov5{k}{resolution}u.pt" for k in "nsmlx" for resolution in ("", "6")]
     + [f"yolov3{k}u.pt" for k in ("", "-spp", "-tiny")]
-    + [f"yolov8{k}-world.pt" for k in "smlx"]
-    + [f"yolov8{k}-worldv2.pt" for k in "smlx"]
-    + [f"yolov9{k}.pt" for k in "ce"]
     + [f"yolo_nas_{k}.pt" for k in "sml"]
     + [f"sam_{k}.pt" for k in "bl"]
     + [f"FastSAM-{k}.pt" for k in "sx"]
     + [f"rtdetr-{k}.pt" for k in "lx"]
     + ["mobile_sam.pt"]
-    + ["calibration_image_sample_data_20x128x128x3_float32.npy.zip"]
 )
 GITHUB_ASSETS_STEMS = [Path(k).stem for k in GITHUB_ASSETS_NAMES]
 
 
-def is_url(url, check=False):
+def is_url(url, check=True):
     """
     Validates if the given string is a URL and optionally checks if the URL exists online.
 
     Args:
         url (str): The string to be validated as a URL.
         check (bool, optional): If True, performs an additional check to see if the URL exists online.
             Defaults to True.
 
     Returns:
-        (bool): Returns True for a valid URL. If 'check' is True, also returns True if the URL exists online.
+        (bool): Returns True if the string is a valid URL. If 'check' is True, also returns True if the URL exists online.
             Returns False otherwise.
 
     Example:
         ```python
         valid = is_url("https://www.example.com")
         ```
     """
@@ -187,21 +183,20 @@
                 LOGGER.warning(f"Potentially insecure file path: {f}, skipping extraction.")
                 continue
             zipObj.extract(f, extract_path)
 
     return path  # return unzip dir
 
 
-def check_disk_space(url="https://ultralytics.com/assets/coco128.zip", path=Path.cwd(), sf=1.5, hard=True):
+def check_disk_space(url="https://ultralytics.com/assets/coco128.zip", sf=1.5, hard=True):
     """
     Check if there is sufficient disk space to download and store a file.
 
     Args:
         url (str, optional): The URL to the file. Defaults to 'https://ultralytics.com/assets/coco128.zip'.
-        path (str | Path, optional): The path or drive to check the available free space on.
         sf (float, optional): Safety factor, the multiplier for the required free space. Defaults to 2.0.
         hard (bool, optional): Whether to throw an error or not on insufficient disk space. Defaults to True.
 
     Returns:
         (bool): True if there is sufficient disk space, False otherwise.
     """
     try:
@@ -209,15 +204,15 @@
         assert r.status_code < 400, f"URL error for {url}: {r.status_code} {r.reason}"  # check response
     except Exception:
         return True  # requests issue, default to True
 
     # Check file size
     gib = 1 << 30  # bytes per GiB
     data = int(r.headers.get("Content-Length", 0)) / gib  # file size (GB)
-    total, used, free = (x / gib for x in shutil.disk_usage(path))  # bytes
+    total, used, free = (x / gib for x in shutil.disk_usage(Path.cwd()))  # bytes
 
     if data * sf < free:
         return True  # sufficient space
 
     # Insufficient space
     text = (
         f"WARNING ⚠️ Insufficient free disk space {free:.1f} GB < {data * sf:.3f} GB required, "
@@ -316,15 +311,15 @@
     f = Path(dir or ".") / (file or url2file(url))  # URL converted to filename
     if "://" not in str(url) and Path(url).is_file():  # URL exists ('://' check required in Windows Python<3.10)
         f = Path(url)  # filename
     elif not f.is_file():  # URL and file do not exist
         desc = f"Downloading {url if gdrive else clean_url(url)} to '{f}'"
         LOGGER.info(f"{desc}...")
         f.parent.mkdir(parents=True, exist_ok=True)  # make directory if missing
-        check_disk_space(url, path=f.parent)
+        check_disk_space(url)
         for i in range(retry + 1):
             try:
                 if curl or i > 0:  # curl download with retry, continue
                     s = "sS" * (not progress)  # silent
                     r = subprocess.run(["curl", "-#", f"-{s}L", url, "-o", f, "--retry", "3", "-C", "-"]).returncode
                     assert r == 0, f"Curl return value {r}"
                 else:  # urllib download
@@ -352,21 +347,21 @@
             except Exception as e:
                 if i == 0 and not is_online():
                     raise ConnectionError(emojis(f"❌  Download failure for {url}. Environment is not online.")) from e
                 elif i >= retry:
                     raise ConnectionError(emojis(f"❌  Download failure for {url}. Retry limit reached.")) from e
                 LOGGER.warning(f"⚠️ Download failure, retrying {i + 1}/{retry} {url}...")
 
-    if unzip and f.exists() and f.suffix in {"", ".zip", ".tar", ".gz"}:
+    if unzip and f.exists() and f.suffix in ("", ".zip", ".tar", ".gz"):
         from zipfile import is_zipfile
 
         unzip_dir = (dir or f.parent).resolve()  # unzip to dir if provided else unzip in place
         if is_zipfile(f):
             unzip_dir = unzip_file(file=f, path=unzip_dir, exist_ok=exist_ok, progress=progress)  # unzip
-        elif f.suffix in {".tar", ".gz"}:
+        elif f.suffix in (".tar", ".gz"):
             LOGGER.info(f"Unzipping {f} to {unzip_dir}...")
             subprocess.run(["tar", "xf" if f.suffix == ".tar" else "xfz", f, "--directory", unzip_dir], check=True)
         if delete:
             f.unlink()  # remove zip
         return unzip_dir
 
 
@@ -407,15 +402,15 @@
     Attempt to download a file from GitHub release assets if it is not found locally. The function checks for the file
     locally first, then tries to download it from the specified GitHub repository release.
 
     Args:
         file (str | Path): The filename or file path to be downloaded.
         repo (str, optional): The GitHub repository in the format 'owner/repo'. Defaults to 'ultralytics/assets'.
         release (str, optional): The specific release version to be downloaded. Defaults to 'v8.1.0'.
-        **kwargs (any): Additional keyword arguments for the download process.
+        **kwargs (dict): Additional keyword arguments for the download process.
 
     Returns:
         (str): The path to the downloaded file.
 
     Example:
         ```python
         file_path = attempt_download_asset('yolov5s.pt', repo='ultralytics/assets', release='latest')
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/utils/errors.py` & `pyppbox-ultralytics-8.1.7/ultralytics/utils/errors.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/utils/files.py` & `pyppbox-ultralytics-8.1.7/ultralytics/utils/files.py`

 * *Files 15% similar despite different names*

```diff
@@ -141,48 +141,7 @@
     return 0.0
 
 
 def get_latest_run(search_dir="."):
     """Return path to most recent 'last.pt' in /runs (i.e. to --resume from)."""
     last_list = glob.glob(f"{search_dir}/**/last*.pt", recursive=True)
     return max(last_list, key=os.path.getctime) if last_list else ""
-
-
-def update_models(model_names=("yolov8n.pt",), source_dir=Path("."), update_names=False):
-    """
-    Updates and re-saves specified YOLO models in an 'updated_models' subdirectory.
-
-    Args:
-        model_names (tuple, optional): Model filenames to update, defaults to ("yolov8n.pt").
-        source_dir (Path, optional): Directory containing models and target subdirectory, defaults to current directory.
-        update_names (bool, optional): Update model names from a data YAML.
-
-    Example:
-        ```python
-        from ultralytics.utils.files import update_models
-
-        model_names = (f"rtdetr-{size}.pt" for size in "lx")
-        update_models(model_names)
-        ```
-    """
-    from ultralytics import YOLO
-    from ultralytics.nn.autobackend import default_class_names
-
-    target_dir = source_dir / "updated_models"
-    target_dir.mkdir(parents=True, exist_ok=True)  # Ensure target directory exists
-
-    for model_name in model_names:
-        model_path = source_dir / model_name
-        print(f"Loading model from {model_path}")
-
-        # Load model
-        model = YOLO(model_path)
-        model.half()
-        if update_names:  # update model names from a dataset YAML
-            model.model.names = default_class_names("coco8.yaml")
-
-        # Define new save path
-        save_path = target_dir / model_name
-
-        # Save model using model.save()
-        print(f"Re-saving {model_name} model to {save_path}")
-        model.save(save_path, use_dill=False)
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/utils/instance.py` & `pyppbox-ultralytics-8.1.7/ultralytics/utils/instance.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/utils/loss.py` & `pyppbox-ultralytics-8.1.7/ultralytics/utils/loss.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,18 +133,18 @@
     def __init__(self, sigmas) -> None:
         """Initialize the KeypointLoss class."""
         super().__init__()
         self.sigmas = sigmas
 
     def forward(self, pred_kpts, gt_kpts, kpt_mask, area):
         """Calculates keypoint loss factor and Euclidean distance loss for predicted and actual keypoints."""
-        d = (pred_kpts[..., 0] - gt_kpts[..., 0]).pow(2) + (pred_kpts[..., 1] - gt_kpts[..., 1]).pow(2)
+        d = (pred_kpts[..., 0] - gt_kpts[..., 0]) ** 2 + (pred_kpts[..., 1] - gt_kpts[..., 1]) ** 2
         kpt_loss_factor = kpt_mask.shape[1] / (torch.sum(kpt_mask != 0, dim=1) + 1e-9)
         # e = d / (2 * (area * self.sigmas) ** 2 + 1e-9)  # from formula
-        e = d / ((2 * self.sigmas).pow(2) * (area + 1e-9) * 2)  # from cocoeval
+        e = d / (2 * self.sigmas) ** 2 / (area + 1e-9) / 2  # from cocoeval
         return (kpt_loss_factor.view(-1, 1) * ((1 - torch.exp(-e)) * kpt_mask)).mean()
 
 
 class v8DetectionLoss:
     """Criterion class for computing training losses."""
 
     def __init__(self, model):  # model must be de-paralleled
@@ -153,15 +153,15 @@
         h = model.args  # hyperparameters
 
         m = model.model[-1]  # Detect() module
         self.bce = nn.BCEWithLogitsLoss(reduction="none")
         self.hyp = h
         self.stride = m.stride  # model strides
         self.nc = m.nc  # number of classes
-        self.no = m.nc + m.reg_max * 4
+        self.no = m.no
         self.reg_max = m.reg_max
         self.device = device
 
         self.use_dfl = m.reg_max > 1
 
         self.assigner = TaskAlignedAssigner(topk=10, num_classes=self.nc, alpha=0.5, beta=6.0)
         self.bbox_loss = BboxLoss(m.reg_max - 1, use_dfl=self.use_dfl).to(device)
@@ -593,20 +593,15 @@
         """Compute the classification loss between predictions and true labels."""
         loss = torch.nn.functional.cross_entropy(preds, batch["cls"], reduction="mean")
         loss_items = loss.detach()
         return loss, loss_items
 
 
 class v8OBBLoss(v8DetectionLoss):
-    def __init__(self, model):
-        """
-        Initializes v8OBBLoss with model, assigner, and rotated bbox loss.
-
-        Note model must be de-paralleled.
-        """
+    def __init__(self, model):  # model must be de-paralleled
         super().__init__(model)
         self.assigner = RotatedTaskAlignedAssigner(topk=10, num_classes=self.nc, alpha=0.5, beta=6.0)
         self.bbox_loss = RotatedBboxLoss(self.reg_max - 1, use_dfl=self.use_dfl).to(self.device)
 
     def preprocess(self, targets, batch_size, scale_tensor):
         """Preprocesses the target counts and matches with the input batch size to output a tensor."""
         if targets.shape[0] == 0:
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/utils/metrics.py` & `pyppbox-ultralytics-8.1.7/ultralytics/utils/metrics.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,21 +18,21 @@
 
 
 def bbox_ioa(box1, box2, iou=False, eps=1e-7):
     """
     Calculate the intersection over box2 area given box1 and box2. Boxes are in x1y1x2y2 format.
 
     Args:
-        box1 (np.ndarray): A numpy array of shape (n, 4) representing n bounding boxes.
-        box2 (np.ndarray): A numpy array of shape (m, 4) representing m bounding boxes.
-        iou (bool): Calculate the standard IoU if True else return inter_area/box2_area.
+        box1 (np.array): A numpy array of shape (n, 4) representing n bounding boxes.
+        box2 (np.array): A numpy array of shape (m, 4) representing m bounding boxes.
+        iou (bool): Calculate the standard iou if True else return inter_area/box2_area.
         eps (float, optional): A small value to avoid division by zero. Defaults to 1e-7.
 
     Returns:
-        (np.ndarray): A numpy array of shape (n, m) representing the intersection over box2 area.
+        (np.array): A numpy array of shape (n, m) representing the intersection over box2 area.
     """
 
     # Get the coordinates of bounding boxes
     b1_x1, b1_y1, b1_x2, b1_y2 = box1.T
     b2_x1, b2_y1, b2_x2, b2_y2 = box2.T
 
     # Intersection area
@@ -112,20 +112,18 @@
 
     # IoU
     iou = inter / union
     if CIoU or DIoU or GIoU:
         cw = b1_x2.maximum(b2_x2) - b1_x1.minimum(b2_x1)  # convex (smallest enclosing box) width
         ch = b1_y2.maximum(b2_y2) - b1_y1.minimum(b2_y1)  # convex height
         if CIoU or DIoU:  # Distance or Complete IoU https://arxiv.org/abs/1911.08287v1
-            c2 = cw.pow(2) + ch.pow(2) + eps  # convex diagonal squared
-            rho2 = (
-                (b2_x1 + b2_x2 - b1_x1 - b1_x2).pow(2) + (b2_y1 + b2_y2 - b1_y1 - b1_y2).pow(2)
-            ) / 4  # center dist**2
+            c2 = cw**2 + ch**2 + eps  # convex diagonal squared
+            rho2 = ((b2_x1 + b2_x2 - b1_x1 - b1_x2) ** 2 + (b2_y1 + b2_y2 - b1_y1 - b1_y2) ** 2) / 4  # center dist ** 2
             if CIoU:  # https://github.com/Zzh-tju/DIoU-SSD-pytorch/blob/master/utils/box/box_utils.py#L47
-                v = (4 / math.pi**2) * ((w2 / h2).atan() - (w1 / h1).atan()).pow(2)
+                v = (4 / math.pi**2) * (torch.atan(w2 / h2) - torch.atan(w1 / h1)).pow(2)
                 with torch.no_grad():
                     alpha = v / (v - iou + (1 + eps))
                 return iou - (rho2 / c2 + v * alpha)  # CIoU
             return iou - rho2 / c2  # DIoU
         c_area = cw * ch + eps  # convex area
         return iou - (c_area - union) / c_area  # GIoU https://arxiv.org/pdf/1902.09630.pdf
     return iou  # IoU
@@ -160,45 +158,45 @@
         area (torch.Tensor): A tensor of shape (N,) representing areas from ground truth.
         sigma (list): A list containing 17 values representing keypoint scales.
         eps (float, optional): A small value to avoid division by zero. Defaults to 1e-7.
 
     Returns:
         (torch.Tensor): A tensor of shape (N, M) representing keypoint similarities.
     """
-    d = (kpt1[:, None, :, 0] - kpt2[..., 0]).pow(2) + (kpt1[:, None, :, 1] - kpt2[..., 1]).pow(2)  # (N, M, 17)
+    d = (kpt1[:, None, :, 0] - kpt2[..., 0]) ** 2 + (kpt1[:, None, :, 1] - kpt2[..., 1]) ** 2  # (N, M, 17)
     sigma = torch.tensor(sigma, device=kpt1.device, dtype=kpt1.dtype)  # (17, )
     kpt_mask = kpt1[..., 2] != 0  # (N, 17)
-    e = d / ((2 * sigma).pow(2) * (area[:, None, None] + eps) * 2)  # from cocoeval
+    e = d / (2 * sigma) ** 2 / (area[:, None, None] + eps) / 2  # from cocoeval
     # e = d / ((area[None, :, None] + eps) * sigma) ** 2 / 2  # from formula
-    return ((-e).exp() * kpt_mask[:, None]).sum(-1) / (kpt_mask.sum(-1)[:, None] + eps)
+    return (torch.exp(-e) * kpt_mask[:, None]).sum(-1) / (kpt_mask.sum(-1)[:, None] + eps)
 
 
 def _get_covariance_matrix(boxes):
     """
     Generating covariance matrix from obbs.
 
     Args:
         boxes (torch.Tensor): A tensor of shape (N, 5) representing rotated bounding boxes, with xywhr format.
 
     Returns:
         (torch.Tensor): Covariance metrixs corresponding to original rotated bounding boxes.
     """
     # Gaussian bounding boxes, ignore the center points (the first two columns) because they are not needed here.
-    gbbs = torch.cat((boxes[:, 2:4].pow(2) / 12, boxes[:, 4:]), dim=-1)
+    gbbs = torch.cat((torch.pow(boxes[:, 2:4], 2) / 12, boxes[:, 4:]), dim=-1)
     a, b, c = gbbs.split(1, dim=-1)
-    cos = c.cos()
-    sin = c.sin()
-    cos2 = cos.pow(2)
-    sin2 = sin.pow(2)
-    return a * cos2 + b * sin2, a * sin2 + b * cos2, (a - b) * cos * sin
+    return (
+        a * torch.cos(c) ** 2 + b * torch.sin(c) ** 2,
+        a * torch.sin(c) ** 2 + b * torch.cos(c) ** 2,
+        a * torch.cos(c) * torch.sin(c) - b * torch.sin(c) * torch.cos(c),
+    )
 
 
 def probiou(obb1, obb2, CIoU=False, eps=1e-7):
     """
-    Calculate the prob IoU between oriented bounding boxes, https://arxiv.org/pdf/2106.06072v1.pdf.
+    Calculate the prob iou between oriented bounding boxes, https://arxiv.org/pdf/2106.06072v1.pdf.
 
     Args:
         obb1 (torch.Tensor): A tensor of shape (N, 5) representing ground truth obbs, with xywhr format.
         obb2 (torch.Tensor): A tensor of shape (N, 5) representing predicted obbs, with xywhr format.
         eps (float, optional): A small value to avoid division by zero. Defaults to 1e-7.
 
     Returns:
@@ -206,38 +204,43 @@
     """
     x1, y1 = obb1[..., :2].split(1, dim=-1)
     x2, y2 = obb2[..., :2].split(1, dim=-1)
     a1, b1, c1 = _get_covariance_matrix(obb1)
     a2, b2, c2 = _get_covariance_matrix(obb2)
 
     t1 = (
-        ((a1 + a2) * (y1 - y2).pow(2) + (b1 + b2) * (x1 - x2).pow(2)) / ((a1 + a2) * (b1 + b2) - (c1 + c2).pow(2) + eps)
+        ((a1 + a2) * (torch.pow(y1 - y2, 2)) + (b1 + b2) * (torch.pow(x1 - x2, 2)))
+        / ((a1 + a2) * (b1 + b2) - (torch.pow(c1 + c2, 2)) + eps)
     ) * 0.25
-    t2 = (((c1 + c2) * (x2 - x1) * (y1 - y2)) / ((a1 + a2) * (b1 + b2) - (c1 + c2).pow(2) + eps)) * 0.5
+    t2 = (((c1 + c2) * (x2 - x1) * (y1 - y2)) / ((a1 + a2) * (b1 + b2) - (torch.pow(c1 + c2, 2)) + eps)) * 0.5
     t3 = (
-        ((a1 + a2) * (b1 + b2) - (c1 + c2).pow(2))
-        / (4 * ((a1 * b1 - c1.pow(2)).clamp_(0) * (a2 * b2 - c2.pow(2)).clamp_(0)).sqrt() + eps)
-        + eps
-    ).log() * 0.5
-    bd = (t1 + t2 + t3).clamp(eps, 100.0)
-    hd = (1.0 - (-bd).exp() + eps).sqrt()
+        torch.log(
+            ((a1 + a2) * (b1 + b2) - (torch.pow(c1 + c2, 2)))
+            / (4 * torch.sqrt((a1 * b1 - torch.pow(c1, 2)).clamp_(0) * (a2 * b2 - torch.pow(c2, 2)).clamp_(0)) + eps)
+            + eps
+        )
+        * 0.5
+    )
+    bd = t1 + t2 + t3
+    bd = torch.clamp(bd, eps, 100.0)
+    hd = torch.sqrt(1.0 - torch.exp(-bd) + eps)
     iou = 1 - hd
     if CIoU:  # only include the wh aspect ratio part
         w1, h1 = obb1[..., 2:4].split(1, dim=-1)
         w2, h2 = obb2[..., 2:4].split(1, dim=-1)
-        v = (4 / math.pi**2) * ((w2 / h2).atan() - (w1 / h1).atan()).pow(2)
+        v = (4 / math.pi**2) * (torch.atan(w2 / h2) - torch.atan(w1 / h1)).pow(2)
         with torch.no_grad():
             alpha = v / (v - iou + (1 + eps))
         return iou - v * alpha  # CIoU
     return iou
 
 
 def batch_probiou(obb1, obb2, eps=1e-7):
     """
-    Calculate the prob IoU between oriented bounding boxes, https://arxiv.org/pdf/2106.06072v1.pdf.
+    Calculate the prob iou between oriented bounding boxes, https://arxiv.org/pdf/2106.06072v1.pdf.
 
     Args:
         obb1 (torch.Tensor | np.ndarray): A tensor of shape (N, 5) representing ground truth obbs, with xywhr format.
         obb2 (torch.Tensor | np.ndarray): A tensor of shape (M, 5) representing predicted obbs, with xywhr format.
         eps (float, optional): A small value to avoid division by zero. Defaults to 1e-7.
 
     Returns:
@@ -248,24 +251,29 @@
 
     x1, y1 = obb1[..., :2].split(1, dim=-1)
     x2, y2 = (x.squeeze(-1)[None] for x in obb2[..., :2].split(1, dim=-1))
     a1, b1, c1 = _get_covariance_matrix(obb1)
     a2, b2, c2 = (x.squeeze(-1)[None] for x in _get_covariance_matrix(obb2))
 
     t1 = (
-        ((a1 + a2) * (y1 - y2).pow(2) + (b1 + b2) * (x1 - x2).pow(2)) / ((a1 + a2) * (b1 + b2) - (c1 + c2).pow(2) + eps)
+        ((a1 + a2) * (torch.pow(y1 - y2, 2)) + (b1 + b2) * (torch.pow(x1 - x2, 2)))
+        / ((a1 + a2) * (b1 + b2) - (torch.pow(c1 + c2, 2)) + eps)
     ) * 0.25
-    t2 = (((c1 + c2) * (x2 - x1) * (y1 - y2)) / ((a1 + a2) * (b1 + b2) - (c1 + c2).pow(2) + eps)) * 0.5
+    t2 = (((c1 + c2) * (x2 - x1) * (y1 - y2)) / ((a1 + a2) * (b1 + b2) - (torch.pow(c1 + c2, 2)) + eps)) * 0.5
     t3 = (
-        ((a1 + a2) * (b1 + b2) - (c1 + c2).pow(2))
-        / (4 * ((a1 * b1 - c1.pow(2)).clamp_(0) * (a2 * b2 - c2.pow(2)).clamp_(0)).sqrt() + eps)
-        + eps
-    ).log() * 0.5
-    bd = (t1 + t2 + t3).clamp(eps, 100.0)
-    hd = (1.0 - (-bd).exp() + eps).sqrt()
+        torch.log(
+            ((a1 + a2) * (b1 + b2) - (torch.pow(c1 + c2, 2)))
+            / (4 * torch.sqrt((a1 * b1 - torch.pow(c1, 2)).clamp_(0) * (a2 * b2 - torch.pow(c2, 2)).clamp_(0)) + eps)
+            + eps
+        )
+        * 0.5
+    )
+    bd = t1 + t2 + t3
+    bd = torch.clamp(bd, eps, 100.0)
+    hd = torch.sqrt(1.0 - torch.exp(-bd) + eps)
     return 1 - hd
 
 
 def smooth_BCE(eps=0.1):
     """
     Computes smoothed positive and negative Binary Cross-Entropy targets.
 
@@ -283,26 +291,26 @@
 
 class ConfusionMatrix:
     """
     A class for calculating and updating a confusion matrix for object detection and classification tasks.
 
     Attributes:
         task (str): The type of task, either 'detect' or 'classify'.
-        matrix (np.ndarray): The confusion matrix, with dimensions depending on the task.
+        matrix (np.array): The confusion matrix, with dimensions depending on the task.
         nc (int): The number of classes.
         conf (float): The confidence threshold for detections.
         iou_thres (float): The Intersection over Union threshold.
     """
 
     def __init__(self, nc, conf=0.25, iou_thres=0.45, task="detect"):
         """Initialize attributes for the YOLO model."""
         self.task = task
         self.matrix = np.zeros((nc + 1, nc + 1)) if self.task == "detect" else np.zeros((nc, nc))
         self.nc = nc  # number of classes
-        self.conf = 0.25 if conf in {None, 0.001} else conf  # apply 0.25 if default val conf is passed
+        self.conf = 0.25 if conf in (None, 0.001) else conf  # apply 0.25 if default val conf is passed
         self.iou_thres = iou_thres
 
     def process_cls_preds(self, preds, targets):
         """
         Update confusion matrix for classification task.
 
         Args:
@@ -314,21 +322,20 @@
             self.matrix[p][t] += 1
 
     def process_batch(self, detections, gt_bboxes, gt_cls):
         """
         Update confusion matrix for object detection task.
 
         Args:
-            detections (Array[N, 6] | Array[N, 7]): Detected bounding boxes and their associated information.
-                                      Each row should contain (x1, y1, x2, y2, conf, class)
-                                      or with an additional element `angle` when it's obb.
-            gt_bboxes (Array[M, 4]| Array[N, 5]): Ground truth bounding boxes with xyxy/xyxyr format.
+            detections (Array[N, 6]): Detected bounding boxes and their associated information.
+                                      Each row should contain (x1, y1, x2, y2, conf, class).
+            gt_bboxes (Array[M, 4]): Ground truth bounding boxes with xyxy format.
             gt_cls (Array[M]): The class labels.
         """
-        if gt_cls.shape[0] == 0:  # Check if labels is empty
+        if gt_cls.size(0) == 0:  # Check if labels is empty
             if detections is not None:
                 detections = detections[detections[:, 4] > self.conf]
                 detection_classes = detections[:, 5].int()
                 for dc in detection_classes:
                     self.matrix[dc, self.nc] += 1  # false positives
             return
         if detections is None:
@@ -336,20 +343,15 @@
             for gc in gt_classes:
                 self.matrix[self.nc, gc] += 1  # background FN
             return
 
         detections = detections[detections[:, 4] > self.conf]
         gt_classes = gt_cls.int()
         detection_classes = detections[:, 5].int()
-        is_obb = detections.shape[1] == 7 and gt_bboxes.shape[1] == 5  # with additional `angle` dimension
-        iou = (
-            batch_probiou(gt_bboxes, torch.cat([detections[:, :4], detections[:, -1:]], dim=-1))
-            if is_obb
-            else box_iou(gt_bboxes, detections[:, :4])
-        )
+        iou = box_iou(gt_bboxes, detections[:, :4])
 
         x = torch.where(iou > self.iou_thres)
         if x[0].shape[0]:
             matches = torch.cat((torch.stack(x, 1), iou[x[0], x[1]][:, None]), 1).cpu().numpy()
             if x[0].shape[0] > 1:
                 matches = matches[matches[:, 2].argsort()[::-1]]
                 matches = matches[np.unique(matches[:, 1], return_index=True)[1]]
@@ -398,15 +400,15 @@
         import seaborn as sn
 
         array = self.matrix / ((self.matrix.sum(0).reshape(1, -1) + 1e-9) if normalize else 1)  # normalize columns
         array[array < 0.005] = np.nan  # don't annotate (would appear as 0.00)
 
         fig, ax = plt.subplots(1, 1, figsize=(12, 9), tight_layout=True)
         nc, nn = self.nc, len(names)  # number of classes, names
-        sn.set_theme(font_scale=1.0 if nc < 50 else 0.8)  # for label size
+        sn.set(font_scale=1.0 if nc < 50 else 0.8)  # for label size
         labels = (0 < nn < 99) and (nn == nc)  # apply names to ticklabels
         ticklabels = (list(names) + ["background"]) if labels else "auto"
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")  # suppress empty matrix RuntimeWarning: All-NaN slice encountered
             sn.heatmap(
                 array,
                 ax=ax,
@@ -695,25 +697,25 @@
 
     @property
     def map50(self):
         """
         Returns the mean Average Precision (mAP) at an IoU threshold of 0.5.
 
         Returns:
-            (float): The mAP at an IoU threshold of 0.5.
+            (float): The mAP50 at an IoU threshold of 0.5.
         """
         return self.all_ap[:, 0].mean() if len(self.all_ap) else 0.0
 
     @property
     def map75(self):
         """
         Returns the mean Average Precision (mAP) at an IoU threshold of 0.75.
 
         Returns:
-            (float): The mAP at an IoU threshold of 0.75.
+            (float): The mAP50 at an IoU threshold of 0.75.
         """
         return self.all_ap[:, 5].mean() if len(self.all_ap) else 0.0
 
     @property
     def map(self):
         """
         Returns the mean Average Precision (mAP) over IoU thresholds of 0.5 - 0.95 in steps of 0.05.
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/utils/ops.py` & `pyppbox-ultralytics-8.1.7/ultralytics/utils/ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,15 +143,15 @@
 def nms_rotated(boxes, scores, threshold=0.45):
     """
     NMS for obbs, powered by probiou and fast-nms.
 
     Args:
         boxes (torch.Tensor): (N, 5), xywhr.
         scores (torch.Tensor): (N, ).
-        threshold (float): IoU threshold.
+        threshold (float): Iou threshold.
 
     Returns:
     """
     if len(boxes) == 0:
         return np.empty((0,), dtype=np.int8)
     sorted_idx = torch.argsort(scores, descending=True)
     boxes = boxes[sorted_idx]
@@ -169,15 +169,14 @@
     multi_label=False,
     labels=(),
     max_det=300,
     nc=0,  # number of classes (optional)
     max_time_img=0.05,
     max_nms=30000,
     max_wh=7680,
-    in_place=True,
     rotated=False,
 ):
     """
     Perform non-maximum suppression (NMS) on a set of boxes, with support for masks and multiple labels per box.
 
     Args:
         prediction (torch.Tensor): A tensor of shape (batch_size, num_classes + 4 + num_masks, num_boxes)
@@ -194,16 +193,15 @@
         labels (List[List[Union[int, float, torch.Tensor]]]): A list of lists, where each inner
             list contains the apriori labels for a given image. The list should be in the format
             output by a dataloader, with each label being a tuple of (class_index, x1, y1, x2, y2).
         max_det (int): The maximum number of boxes to keep after NMS.
         nc (int, optional): The number of classes output by the model. Any indices after this will be considered masks.
         max_time_img (float): The maximum time (seconds) for processing one image.
         max_nms (int): The maximum number of boxes into torchvision.ops.nms().
-        max_wh (int): The maximum box width and height in pixels.
-        in_place (bool): If True, the input prediction tensor will be modified in place.
+        max_wh (int): The maximum box width and height in pixels
 
     Returns:
         (List[torch.Tensor]): A list of length batch_size, where each element is a tensor of
             shape (num_boxes, 6 + num_masks) containing the kept boxes, with columns
             (x1, y1, x2, y2, confidence, class, mask1, mask2, ...).
     """
 
@@ -222,18 +220,15 @@
     # Settings
     # min_wh = 2  # (pixels) minimum box width and height
     time_limit = 2.0 + max_time_img * bs  # seconds to quit after
     multi_label &= nc > 1  # multiple labels per box (adds 0.5ms/img)
 
     prediction = prediction.transpose(-1, -2)  # shape(1,84,6300) to shape(1,6300,84)
     if not rotated:
-        if in_place:
-            prediction[..., :4] = xywh2xyxy(prediction[..., :4])  # xywh to xyxy
-        else:
-            prediction = torch.cat((xywh2xyxy(prediction[..., :4]), prediction[..., 4:]), dim=-1)  # xywh to xyxy
+        prediction[..., :4] = xywh2xyxy(prediction[..., :4])  # xywh to xyxy
 
     t = time.time()
     output = [torch.zeros((0, 6 + nm), device=prediction.device)] * bs
     for xi, x in enumerate(prediction):  # image index, image inference
         # Apply constraints
         # x[((x[:, 2:4] < min_wh) | (x[:, 2:4] > max_wh)).any(1), 4] = 0  # width-height
         x = x[xc[xi]]  # confidence
@@ -283,15 +278,15 @@
         i = i[:max_det]  # limit detections
 
         # # Experimental
         # merge = False  # use merge-NMS
         # if merge and (1 < n < 3E3):  # Merge NMS (boxes merged using weighted mean)
         #     # Update boxes as boxes(i,4) = weights(i,n) * boxes(n,4)
         #     from .metrics import box_iou
-        #     iou = box_iou(boxes[i], boxes) > iou_thres  # IoU matrix
+        #     iou = box_iou(boxes[i], boxes) > iou_thres  # iou matrix
         #     weights = iou * scores[None]  # box weights
         #     x[i, :4] = torch.mm(weights, x[:, :4]).float() / weights.sum(1, keepdim=True)  # merged boxes
         #     redundant = True  # require redundant detections
         #     if redundant:
         #         i = i[iou.sum(1) > 1]  # require redundancy
 
         output[xi] = x[i]
@@ -547,15 +542,15 @@
 
 def xywhr2xyxyxyxy(rboxes):
     """
     Convert batched Oriented Bounding Boxes (OBB) from [xywh, rotation] to [xy1, xy2, xy3, xy4]. Rotation values should
     be in degrees from 0 to 90.
 
     Args:
-        rboxes (numpy.ndarray | torch.Tensor): Boxes in [cx, cy, w, h, rotation] format of shape (n, 5) or (b, n, 5).
+        rboxes (numpy.ndarray | torch.Tensor): Input data in [cx, cy, w, h, rotation] format of shape (n, 5) or (b, n, 5).
 
     Returns:
         (numpy.ndarray | torch.Tensor): Converted corner points of shape (n, 4, 2) or (b, n, 4, 2).
     """
     is_numpy = isinstance(rboxes, np.ndarray)
     cos, sin = (np.cos, np.sin) if is_numpy else (torch.cos, torch.sin)
 
@@ -634,15 +629,15 @@
     Args:
         masks (torch.Tensor): [n, h, w] tensor of masks
         boxes (torch.Tensor): [n, 4] tensor of bbox coordinates in relative point form
 
     Returns:
         (torch.Tensor): The masks are being cropped to the bounding box.
     """
-    _, h, w = masks.shape
+    n, h, w = masks.shape
     x1, y1, x2, y2 = torch.chunk(boxes[:, :, None], 4, 1)  # x1 shape(n,1,1)
     r = torch.arange(w, device=masks.device, dtype=x1.dtype)[None, None, :]  # rows shape(1,1,w)
     c = torch.arange(h, device=masks.device, dtype=x1.dtype)[None, :, None]  # cols shape(1,h,1)
 
     return masks * ((r >= x1) * (r < x2) * (c >= y1) * (c < y2))
 
 
@@ -682,22 +677,20 @@
         (torch.Tensor): A binary mask tensor of shape [n, h, w], where n is the number of masks after NMS, and h and w
             are the height and width of the input image. The mask is applied to the bounding boxes.
     """
 
     c, mh, mw = protos.shape  # CHW
     ih, iw = shape
     masks = (masks_in @ protos.float().view(c, -1)).sigmoid().view(-1, mh, mw)  # CHW
-    width_ratio = mw / iw
-    height_ratio = mh / ih
 
     downsampled_bboxes = bboxes.clone()
-    downsampled_bboxes[:, 0] *= width_ratio
-    downsampled_bboxes[:, 2] *= width_ratio
-    downsampled_bboxes[:, 3] *= height_ratio
-    downsampled_bboxes[:, 1] *= height_ratio
+    downsampled_bboxes[:, 0] *= mw / iw
+    downsampled_bboxes[:, 2] *= mw / iw
+    downsampled_bboxes[:, 3] *= mh / ih
+    downsampled_bboxes[:, 1] *= mh / ih
 
     masks = crop_mask(masks, downsampled_bboxes)  # CHW
     if upsample:
         masks = F.interpolate(masks[None], shape, mode="bilinear", align_corners=False)[0]  # CHW
     return masks.gt_(0.5)
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/utils/patches.py` & `pyppbox-ultralytics-8.1.7/ultralytics/utils/patches.py`

 * *Files 16% similar despite different names*

```diff
@@ -56,33 +56,31 @@
     _imshow(winname.encode("unicode_escape").decode(), mat)
 
 
 # PyTorch functions ----------------------------------------------------------------------------------------------------
 _torch_save = torch.save  # copy to avoid recursion errors
 
 
-def torch_save(*args, use_dill=True, **kwargs):
+def torch_save(*args, **kwargs):
     """
-    Optionally use dill to serialize lambda functions where pickle does not, adding robustness with 3 retries and
-    exponential standoff in case of save failure.
+    Use dill (if exists) to serialize the lambda functions where pickle does not do this. Also adds 3 retries with
+    exponential standoff in case of save failure to improve robustness to transient issues.
 
     Args:
         *args (tuple): Positional arguments to pass to torch.save.
-        use_dill (bool): Whether to try using dill for serialization if available. Defaults to True.
-        **kwargs (any): Keyword arguments to pass to torch.save.
+        **kwargs (dict): Keyword arguments to pass to torch.save.
     """
     try:
-        assert use_dill
-        import dill as pickle
-    except (AssertionError, ImportError):
+        import dill as pickle  # noqa
+    except ImportError:
         import pickle
 
     if "pickle_module" not in kwargs:
-        kwargs["pickle_module"] = pickle
+        kwargs["pickle_module"] = pickle  # noqa
 
     for i in range(4):  # 3 retries
         try:
             return _torch_save(*args, **kwargs)
-        except RuntimeError as e:  # unable to save, possibly waiting for device to flush or antivirus scan
+        except RuntimeError:  # unable to save, possibly waiting for device to flush or anti-virus to finish scanning
             if i == 3:
-                raise e
-            time.sleep((2**i) / 2)  # exponential standoff: 0.5s, 1.0s, 2.0s
+                raise
+            time.sleep((2**i) / 2)  # exponential standoff 0.5s, 1.0s, 2.0s
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/utils/plotting.py` & `pyppbox-ultralytics-8.1.7/ultralytics/utils/plotting.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
     This class provides methods to work with the Ultralytics color palette, including converting hex color codes to
     RGB values.
 
     Attributes:
         palette (list of tuple): List of RGB color values.
         n (int): The number of colors in the palette.
-        pose_palette (np.ndarray): A specific color palette array with dtype np.uint8.
+        pose_palette (np.array): A specific color palette array with dtype np.uint8.
     """
 
     def __init__(self):
         """Initialize colors as hex = matplotlib.colors.TABLEAU_COLORS.values()."""
         hexs = (
             "FF3838",
             "FF9D97",
@@ -108,32 +108,31 @@
         skeleton (List[List[int]]): Skeleton structure for keypoints.
         limb_color (List[int]): Color palette for limbs.
         kpt_color (List[int]): Color palette for keypoints.
     """
 
     def __init__(self, im, line_width=None, font_size=None, font="Arial.ttf", pil=False, example="abc"):
         """Initialize the Annotator class with image and line width along with color palette for keypoints and limbs."""
+        assert im.data.contiguous, "Image not contiguous. Apply np.ascontiguousarray(im) to Annotator() input images."
         non_ascii = not is_ascii(example)  # non-latin labels, i.e. asian, arabic, cyrillic
-        input_is_pil = isinstance(im, Image.Image)
-        self.pil = pil or non_ascii or input_is_pil
-        self.lw = line_width or max(round(sum(im.size if input_is_pil else im.shape) / 2 * 0.003), 2)
+        self.pil = pil or non_ascii
+        self.lw = line_width or max(round(sum(im.shape) / 2 * 0.003), 2)  # line width
         if self.pil:  # use PIL
-            self.im = im if input_is_pil else Image.fromarray(im)
+            self.im = im if isinstance(im, Image.Image) else Image.fromarray(im)
             self.draw = ImageDraw.Draw(self.im)
             try:
                 font = check_font("Arial.Unicode.ttf" if non_ascii else font)
                 size = font_size or max(round(sum(self.im.size) / 2 * 0.035), 12)
                 self.font = ImageFont.truetype(str(font), size)
             except Exception:
                 self.font = ImageFont.load_default()
             # Deprecation fix for w, h = getsize(string) -> _, _, w, h = getbox(string)
             if check_version(pil_version, "9.2.0"):
                 self.font.getsize = lambda x: self.font.getbbox(x)[2:4]  # text width, height
         else:  # use cv2
-            assert im.data.contiguous, "Image not contiguous. Apply np.ascontiguousarray(im) to Annotator input images."
             self.im = im if im.flags.writeable else im.copy()
             self.tf = max(self.lw - 1, 1)  # font thickness
             self.sf = self.lw / 3  # font scale
         # Pose
         self.skeleton = [
             [16, 14],
             [14, 12],
@@ -247,16 +246,15 @@
         Args:
             kpts (tensor): Predicted keypoints with shape [17, 3]. Each keypoint has (x, y, confidence).
             shape (tuple): Image shape as a tuple (h, w), where h is the height and w is the width.
             radius (int, optional): Radius of the drawn keypoints. Default is 5.
             kpt_line (bool, optional): If True, the function will draw lines connecting keypoints
                                        for human pose. Default is True.
 
-        Note:
-            `kpt_line=True` currently only supports human pose plotting.
+        Note: `kpt_line=True` currently only supports human pose plotting.
         """
         if self.pil:
             # Convert to numpy first
             self.im = np.asarray(self.im).copy()
         nkpt, ndim = kpts.shape
         is_pose = nkpt == 17 and ndim in {2, 3}
         kpt_line &= is_pose  # `kpt_line=True` for now only supports human pose plotting
@@ -327,127 +325,69 @@
         self.im = im if isinstance(im, Image.Image) else Image.fromarray(im)
         self.draw = ImageDraw.Draw(self.im)
 
     def result(self):
         """Return annotated image as array."""
         return np.asarray(self.im)
 
-    def show(self, title=None):
-        """Show the annotated image."""
-        Image.fromarray(np.asarray(self.im)[..., ::-1]).show(title)
-
-    def save(self, filename="image.jpg"):
-        """Save the annotated image to 'filename'."""
-        cv2.imwrite(filename, np.asarray(self.im))
-
+    # Object Counting Annotator
     def draw_region(self, reg_pts=None, color=(0, 255, 0), thickness=5):
         """
-        Draw region line.
-
+        Draw region line
         Args:
             reg_pts (list): Region Points (for line 2 points, for region 4 points)
             color (tuple): Region Color value
             thickness (int): Region area thickness value
         """
         cv2.polylines(self.im, [np.array(reg_pts, dtype=np.int32)], isClosed=True, color=color, thickness=thickness)
 
     def draw_centroid_and_tracks(self, track, color=(255, 0, 255), track_thickness=2):
         """
-        Draw centroid point and track trails.
-
+        Draw centroid point and track trails
         Args:
             track (list): object tracking points for trails display
             color (tuple): tracks line color
             track_thickness (int): track line thickness value
         """
         points = np.hstack(track).astype(np.int32).reshape((-1, 1, 2))
         cv2.polylines(self.im, [points], isClosed=False, color=color, thickness=track_thickness)
         cv2.circle(self.im, (int(track[-1][0]), int(track[-1][1])), track_thickness * 2, color, -1)
 
-    def queue_counts_display(self, label, points=None, region_color=(255, 255, 255), txt_color=(0, 0, 0), fontsize=0.7):
-        """Displays queue counts on an image centered at the points with customizable font size and colors."""
-        x_values = [point[0] for point in points]
-        y_values = [point[1] for point in points]
-        center_x = sum(x_values) // len(points)
-        center_y = sum(y_values) // len(points)
-
-        text_size = cv2.getTextSize(label, cv2.FONT_HERSHEY_SIMPLEX, fontScale=fontsize, thickness=self.tf)[0]
-        text_width = text_size[0]
-        text_height = text_size[1]
-
-        rect_width = text_width + 20
-        rect_height = text_height + 20
-        rect_top_left = (center_x - rect_width // 2, center_y - rect_height // 2)
-        rect_bottom_right = (center_x + rect_width // 2, center_y + rect_height // 2)
-        cv2.rectangle(self.im, rect_top_left, rect_bottom_right, region_color, -1)
-
-        text_x = center_x - text_width // 2
-        text_y = center_y + text_height // 2
-
-        # Draw text
-        cv2.putText(
-            self.im,
-            label,
-            (text_x, text_y),
-            cv2.FONT_HERSHEY_SIMPLEX,
-            fontScale=fontsize,
-            color=txt_color,
-            thickness=self.tf,
-            lineType=cv2.LINE_AA,
-        )
-
-    def display_counts(
-        self, counts=None, tf=2, fontScale=0.6, line_color=(0, 0, 0), txt_color=(255, 255, 255), classwise_txtgap=55
-    ):
+    def count_labels(self, counts=0, count_txt_size=2, color=(255, 255, 255), txt_color=(0, 0, 0)):
         """
-        Display counts on im0.
-
+        Plot counts for object counter
         Args:
-            counts (str): objects count data
-            tf (int): text thickness for display
-            fontScale (float): text fontsize for display
-            line_color (RGB Color): counts highlighter color
-            txt_color (RGB Color): counts display color
-            classwise_txtgap (int): Gap between each class count data
+            counts (int): objects counts value
+            count_txt_size (int): text size for counts display
+            color (tuple): background color of counts display
+            txt_color (tuple): text color of counts display
         """
-
-        tl = tf or round(0.002 * (self.im.shape[0] + self.im.shape[1]) / 2) + 1
+        self.tf = count_txt_size
+        tl = self.tf or round(0.002 * (self.im.shape[0] + self.im.shape[1]) / 2) + 1
         tf = max(tl - 1, 1)
 
-        t_sizes = [cv2.getTextSize(str(count), 0, fontScale=0.8, thickness=tf)[0] for count in counts]
-
-        max_text_width = max([size[0] for size in t_sizes])
-        max_text_height = max([size[1] for size in t_sizes])
+        # Get text size for in_count and out_count
+        t_size_in = cv2.getTextSize(str(counts), 0, fontScale=tl / 2, thickness=tf)[0]
 
-        text_x = self.im.shape[1] - max_text_width - 20
-        text_y = classwise_txtgap
+        # Calculate positions for counts label
+        text_width = t_size_in[0]
+        text_x = (self.im.shape[1] - text_width) // 2  # Center x-coordinate
+        text_y = t_size_in[1]
 
-        for i, count in enumerate(counts):
-            text_x_pos = text_x
-            text_y_pos = text_y + i * classwise_txtgap
-
-            cv2.putText(
-                self.im,
-                str(count),
-                (text_x_pos, text_y_pos),
-                cv2.FONT_HERSHEY_SIMPLEX,
-                fontScale=fontScale,
-                color=txt_color,
-                thickness=tf,
-                lineType=cv2.LINE_AA,
-            )
-
-            line_y_pos = text_y_pos + max_text_height + 5
-            cv2.line(self.im, (text_x_pos, line_y_pos), (text_x_pos + max_text_width, line_y_pos), line_color, tf)
+        # Create a rounded rectangle for in_count
+        cv2.rectangle(
+            self.im, (text_x - 5, text_y - 5), (text_x + text_width + 7, text_y + t_size_in[1] + 7), color, -1
+        )
+        cv2.putText(
+            self.im, str(counts), (text_x, text_y + t_size_in[1]), 0, tl / 2, txt_color, self.tf, lineType=cv2.LINE_AA
+        )
 
     @staticmethod
     def estimate_pose_angle(a, b, c):
-        """
-        Calculate the pose angle for object.
-
+        """Calculate the pose angle for object
         Args:
             a (float) : The value of pose point a
             b (float): The value of pose point b
             c (float): The value o pose point c
 
         Returns:
             angle (degree): Degree value of angle between three points
@@ -465,14 +405,16 @@
 
         Args:
             keypoints (list): list of keypoints data to be plotted
             indices (list): keypoints ids list to be plotted
             shape (tuple): imgsz for model inference
             radius (int): Keypoint radius value
         """
+        nkpts, ndim = keypoints.shape
+        nkpts == 17 and ndim == 3
         for i, k in enumerate(keypoints):
             if i in indices:
                 x_coord, y_coord = k[0], k[1]
                 if x_coord % shape[1] != 0 and y_coord % shape[0] != 0:
                     if len(k) == 3:
                         conf = k[2]
                         if conf < 0.5:
@@ -755,15 +697,14 @@
     kpts=np.zeros((0, 51), dtype=np.float32),
     paths=None,
     fname="images.jpg",
     names=None,
     on_plot=None,
     max_subplots=16,
     save=True,
-    conf_thres=0.25,
 ):
     """Plot image grid with labels."""
     if isinstance(images, torch.Tensor):
         images = images.cpu().float().numpy()
     if isinstance(cls, torch.Tensor):
         cls = cls.cpu().numpy()
     if isinstance(bboxes, torch.Tensor):
@@ -821,15 +762,15 @@
                         boxes[..., :4] *= scale
                 boxes[..., 0::2] += x
                 boxes[..., 1::2] += y
                 for j, box in enumerate(boxes.astype(np.int64).tolist()):
                     c = classes[j]
                     color = colors(c)
                     c = names.get(c, c) if names else c
-                    if labels or conf[j] > conf_thres:
+                    if labels or conf[j] > 0.25:  # 0.25 conf thresh
                         label = f"{c}" if labels else f"{c} {conf[j]:.1f}"
                         annotator.box_label(box, label, color=color, rotated=is_obb)
 
             elif len(classes):
                 for c in classes:
                     color = colors(c)
                     c = names.get(c, c) if names else c
@@ -843,15 +784,15 @@
                         kpts_[..., 0] *= w  # scale to pixels
                         kpts_[..., 1] *= h
                     elif scale < 1:  # absolute coords need scale if image scales
                         kpts_ *= scale
                 kpts_[..., 0] += x
                 kpts_[..., 1] += y
                 for j in range(len(kpts_)):
-                    if labels or conf[j] > conf_thres:
+                    if labels or conf[j] > 0.25:  # 0.25 conf thresh
                         annotator.kpts(kpts_[j])
 
             # Plot masks
             if len(masks):
                 if idx.shape[0] == masks.shape[0]:  # overlap_masks=False
                     image_masks = masks[idx]
                 else:  # overlap_masks=True
@@ -859,15 +800,15 @@
                     nl = idx.sum()
                     index = np.arange(nl).reshape((nl, 1, 1)) + 1
                     image_masks = np.repeat(image_masks, nl, axis=0)
                     image_masks = np.where(image_masks == index, 1.0, 0.0)
 
                 im = np.asarray(annotator.im).copy()
                 for j in range(len(image_masks)):
-                    if labels or conf[j] > conf_thres:
+                    if labels or conf[j] > 0.25:  # 0.25 conf thresh
                         color = colors(classes[j])
                         mh, mw = image_masks[j].shape
                         if mh != h or mw != w:
                             mask = image_masks[j].astype(np.uint8)
                             mask = cv2.resize(mask, (w, h))
                             mask = mask.astype(bool)
                         else:
@@ -932,15 +873,15 @@
             x = data.values[:, 0]
             for i, j in enumerate(index):
                 y = data.values[:, j].astype("float")
                 # y[y == 0] = np.nan  # don't show zero values
                 ax[i].plot(x, y, marker=".", label=f.stem, linewidth=2, markersize=8)  # actual results
                 ax[i].plot(x, gaussian_filter1d(y, sigma=3), ":", label="smooth", linewidth=2)  # smoothing line
                 ax[i].set_title(s[j], fontsize=12)
-                # if j in {8, 9, 10}:  # share train and val loss y axes
+                # if j in [8, 9, 10]:  # share train and val loss y axes
                 #     ax[i].get_shared_y_axes().join(ax[i], ax[i - 5])
         except Exception as e:
             LOGGER.warning(f"WARNING: Plotting error for {f}: {e}")
     ax[1].legend()
     fname = save_dir / "results.png"
     fig.savefig(fname, dpi=200)
     plt.close()
@@ -1070,21 +1011,21 @@
         stage (int): Module stage within the model.
         n (int, optional): Maximum number of feature maps to plot. Defaults to 32.
         save_dir (Path, optional): Directory to save results. Defaults to Path('runs/detect/exp').
     """
     for m in ["Detect", "Pose", "Segment"]:
         if m in module_type:
             return
-    _, channels, height, width = x.shape  # batch, channels, height, width
+    batch, channels, height, width = x.shape  # batch, channels, height, width
     if height > 1 and width > 1:
         f = save_dir / f"stage{stage}_{module_type.split('.')[-1]}_features.png"  # filename
 
         blocks = torch.chunk(x[0].cpu(), channels, dim=0)  # select batch index 0, block by channels
         n = min(n, channels)  # number of plots
-        _, ax = plt.subplots(math.ceil(n / 8), 8, tight_layout=True)  # 8 rows x n/8 cols
+        fig, ax = plt.subplots(math.ceil(n / 8), 8, tight_layout=True)  # 8 rows x n/8 cols
         ax = ax.ravel()
         plt.subplots_adjust(wspace=0.05, hspace=0.05)
         for i in range(n):
             ax[i].imshow(blocks[i].squeeze())  # cmap='gray'
             ax[i].axis("off")
 
         LOGGER.info(f"Saving {f}... ({n}/{channels})")
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/utils/tal.py` & `pyppbox-ultralytics-8.1.7/ultralytics/utils/tal.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,16 +52,16 @@
         Returns:
             target_labels (Tensor): shape(bs, num_total_anchors)
             target_bboxes (Tensor): shape(bs, num_total_anchors, 4)
             target_scores (Tensor): shape(bs, num_total_anchors, num_classes)
             fg_mask (Tensor): shape(bs, num_total_anchors)
             target_gt_idx (Tensor): shape(bs, num_total_anchors)
         """
-        self.bs = pd_scores.shape[0]
-        self.n_max_boxes = gt_bboxes.shape[1]
+        self.bs = pd_scores.size(0)
+        self.n_max_boxes = gt_bboxes.size(1)
 
         if self.n_max_boxes == 0:
             device = gt_bboxes.device
             return (
                 torch.full_like(pd_scores[..., 0], self.bg_idx).to(device),
                 torch.zeros_like(pd_bboxes).to(device),
                 torch.zeros_like(pd_scores).to(device),
@@ -117,15 +117,15 @@
         gt_boxes = gt_bboxes.unsqueeze(2).expand(-1, -1, na, -1)[mask_gt]
         overlaps[mask_gt] = self.iou_calculation(gt_boxes, pd_boxes)
 
         align_metric = bbox_scores.pow(self.alpha) * overlaps.pow(self.beta)
         return align_metric, overlaps
 
     def iou_calculation(self, gt_bboxes, pd_bboxes):
-        """IoU calculation for horizontal bounding boxes."""
+        """Iou calculation for horizontal bounding boxes."""
         return bbox_iou(gt_bboxes, pd_bboxes, xywh=False, CIoU=True).squeeze(-1).clamp_(0)
 
     def select_topk_candidates(self, metrics, largest=True, topk_mask=None):
         """
         Select the top-k candidates based on the given metrics.
 
         Args:
@@ -227,15 +227,15 @@
         bbox_deltas = torch.cat((xy_centers[None] - lt, rb - xy_centers[None]), dim=2).view(bs, n_boxes, n_anchors, -1)
         # return (bbox_deltas.min(3)[0] > eps).to(gt_bboxes.dtype)
         return bbox_deltas.amin(3).gt_(eps)
 
     @staticmethod
     def select_highest_overlaps(mask_pos, overlaps, n_max_boxes):
         """
-        If an anchor box is assigned to multiple gts, the one with the highest IoU will be selected.
+        If an anchor box is assigned to multiple gts, the one with the highest IoI will be selected.
 
         Args:
             mask_pos (Tensor): shape(b, n_max_boxes, h*w)
             overlaps (Tensor): shape(b, n_max_boxes, h*w)
 
         Returns:
             target_gt_idx (Tensor): shape(b, h*w)
@@ -256,15 +256,15 @@
         # Find each grid serve which gt(index)
         target_gt_idx = mask_pos.argmax(-2)  # (b, h*w)
         return target_gt_idx, fg_mask, mask_pos
 
 
 class RotatedTaskAlignedAssigner(TaskAlignedAssigner):
     def iou_calculation(self, gt_bboxes, pd_bboxes):
-        """IoU calculation for rotated bounding boxes."""
+        """Iou calculation for rotated bounding boxes."""
         return probiou(gt_bboxes, pd_bboxes).squeeze(-1).clamp_(0)
 
     @staticmethod
     def select_candidates_in_gts(xy_centers, gt_bboxes):
         """
         Select the positive anchor center in gt for rotated bounding boxes.
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/utils/torch_utils.py` & `pyppbox-ultralytics-8.1.7/ultralytics/utils/torch_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,47 +1,46 @@
 # Ultralytics YOLO 🚀, AGPL-3.0 license
 
 import math
 import os
+import platform
 import random
 import time
 from contextlib import contextmanager
 from copy import deepcopy
 from pathlib import Path
 from typing import Union
 
 import numpy as np
 import torch
 import torch.distributed as dist
 import torch.nn as nn
 import torch.nn.functional as F
 import torchvision
 
-from ultralytics.utils import DEFAULT_CFG_DICT, DEFAULT_CFG_KEYS, LOGGER, colorstr, __version__
-from ultralytics.utils.checks import PYTHON_VERSION, check_version
+from ultralytics.utils import DEFAULT_CFG_DICT, DEFAULT_CFG_KEYS, LOGGER, __version__
+from ultralytics.utils.checks import check_version
 
 try:
     import thop
 except ImportError:
     thop = None
 
-# Version checks (all default to version>=min_version)
 TORCH_1_9 = check_version(torch.__version__, "1.9.0")
-TORCH_1_13 = check_version(torch.__version__, "1.13.0")
 TORCH_2_0 = check_version(torch.__version__, "2.0.0")
 TORCHVISION_0_10 = check_version(torchvision.__version__, "0.10.0")
 TORCHVISION_0_11 = check_version(torchvision.__version__, "0.11.0")
 TORCHVISION_0_13 = check_version(torchvision.__version__, "0.13.0")
 
 
 @contextmanager
 def torch_distributed_zero_first(local_rank: int):
     """Decorator to make all processes in distributed training wait for each local_master to do something."""
     initialized = torch.distributed.is_available() and torch.distributed.is_initialized()
-    if initialized and local_rank not in {-1, 0}:
+    if initialized and local_rank not in (-1, 0):
         dist.barrier(device_ids=[local_rank])
     yield
     if initialized and local_rank == 0:
         dist.barrier(device_ids=[0])
 
 
 def smart_inference_mode():
@@ -100,28 +99,28 @@
     Note:
         Sets the 'CUDA_VISIBLE_DEVICES' environment variable for specifying which GPUs to use.
     """
 
     if isinstance(device, torch.device):
         return device
 
-    s = f"Ultralytics YOLOv{__version__} 🚀 Python-{PYTHON_VERSION} torch-{torch.__version__} "
+    s = f"Ultralytics YOLOv{__version__} 🚀 Python-{platform.python_version()} torch-{torch.__version__} "
     device = str(device).lower()
     for remove in "cuda:", "none", "(", ")", "[", "]", "'", " ":
         device = device.replace(remove, "")  # to string, 'cuda:0' -> '0' and '(0, 1)' -> '0,1'
     cpu = device == "cpu"
-    mps = device in {"mps", "mps:0"}  # Apple Metal Performance Shaders (MPS)
+    mps = device in ("mps", "mps:0")  # Apple Metal Performance Shaders (MPS)
     if cpu or mps:
         os.environ["CUDA_VISIBLE_DEVICES"] = "-1"  # force torch.cuda.is_available() = False
     elif device:  # non-cpu device requested
         if device == "cuda":
             device = "0"
         visible = os.environ.get("CUDA_VISIBLE_DEVICES", None)
         os.environ["CUDA_VISIBLE_DEVICES"] = device  # set environment variable - must be before assert is_available()
-        if not (torch.cuda.is_available() and torch.cuda.device_count() >= len(device.split(","))):
+        if not (torch.cuda.is_available() and torch.cuda.device_count() >= len(device.replace(",", ""))):
             LOGGER.info(s)
             install = (
                 "See https://pytorch.org/get-started/locally/ for up-to-date torch install instructions if no "
                 "CUDA devices are seen by torch.\n"
                 if torch.cuda.device_count() == 0
                 else ""
             )
@@ -187,15 +186,15 @@
 
     # Prepare filters
     w_conv = conv.weight.clone().view(conv.out_channels, -1)
     w_bn = torch.diag(bn.weight.div(torch.sqrt(bn.eps + bn.running_var)))
     fusedconv.weight.copy_(torch.mm(w_bn, w_conv).view(fusedconv.weight.shape))
 
     # Prepare spatial bias
-    b_conv = torch.zeros(conv.weight.shape[0], device=conv.weight.device) if conv.bias is None else conv.bias
+    b_conv = torch.zeros(conv.weight.size(0), device=conv.weight.device) if conv.bias is None else conv.bias
     b_bn = bn.bias - bn.weight.mul(bn.running_mean).div(torch.sqrt(bn.running_var + bn.eps))
     fusedconv.bias.copy_(torch.mm(w_bn, b_conv.reshape(-1, 1)).reshape(-1) + b_bn)
 
     return fusedconv
 
 
 def fuse_deconv_and_bn(deconv, bn):
@@ -218,15 +217,15 @@
 
     # Prepare filters
     w_deconv = deconv.weight.clone().view(deconv.out_channels, -1)
     w_bn = torch.diag(bn.weight.div(torch.sqrt(bn.eps + bn.running_var)))
     fuseddconv.weight.copy_(torch.mm(w_bn, w_deconv).view(fuseddconv.weight.shape))
 
     # Prepare spatial bias
-    b_conv = torch.zeros(deconv.weight.shape[1], device=deconv.weight.device) if deconv.bias is None else deconv.bias
+    b_conv = torch.zeros(deconv.weight.size(1), device=deconv.weight.device) if deconv.bias is None else deconv.bias
     b_bn = bn.bias - bn.weight.mul(bn.running_mean).div(torch.sqrt(bn.running_var + bn.eps))
     fuseddconv.bias.copy_(torch.mm(w_bn, b_conv.reshape(-1, 1)).reshape(-1) + b_bn)
 
     return fuseddconv
 
 
 def model_info(model, detailed=False, verbose=True, imgsz=640):
@@ -343,15 +342,15 @@
     for m in model.modules():
         t = type(m)
         if t is nn.Conv2d:
             pass  # nn.init.kaiming_normal_(m.weight, mode='fan_out', nonlinearity='relu')
         elif t is nn.BatchNorm2d:
             m.eps = 1e-3
             m.momentum = 0.03
-        elif t in {nn.Hardswish, nn.LeakyReLU, nn.ReLU, nn.ReLU6, nn.SiLU}:
+        elif t in [nn.Hardswish, nn.LeakyReLU, nn.ReLU, nn.ReLU6, nn.SiLU]:
             m.inplace = True
 
 
 def scale_img(img, ratio=1.0, same_shape=False, gs=32):
     """Scales and pads an image tensor of shape img(bs,3,y,x) based on given ratio and grid size gs, optionally
     retaining the original shape.
     """
@@ -501,28 +500,14 @@
     x["train_args"] = {k: v for k, v in args.items() if k in DEFAULT_CFG_KEYS}  # strip non-default keys
     # x['model'].args = x['train_args']
     torch.save(x, s or f)
     mb = os.path.getsize(s or f) / 1e6  # file size
     LOGGER.info(f"Optimizer stripped from {f},{f' saved as {s},' if s else ''} {mb:.1f}MB")
 
 
-def convert_optimizer_state_dict_to_fp16(state_dict):
-    """
-    Converts the state_dict of a given optimizer to FP16, focusing on the 'state' key for tensor conversions.
-
-    This method aims to reduce storage size without altering 'param_groups' as they contain non-tensor data.
-    """
-    for state in state_dict["state"].values():
-        for k, v in state.items():
-            if k != "step" and isinstance(v, torch.Tensor) and v.dtype is torch.float32:
-                state[k] = v.half()
-
-    return state_dict
-
-
 def profile(input, ops, n=10, device=None):
     """
     Ultralytics speed, memory and FLOPs profiler.
 
     Example:
         ```python
         from ultralytics.utils.torch_utils import profile
@@ -610,15 +595,14 @@
         if fitness >= self.best_fitness:  # >= 0 to allow for early zero-fitness stage of training
             self.best_epoch = epoch
             self.best_fitness = fitness
         delta = epoch - self.best_epoch  # epochs without improvement
         self.possible_stop = delta >= (self.patience - 1)  # possible stop may occur next epoch
         stop = delta >= self.patience  # stop training if patience exceeded
         if stop:
-            prefix = colorstr("EarlyStopping: ")
             LOGGER.info(
-                f"{prefix}Training stopped early as no improvement observed in last {self.patience} epochs. "
+                f"Stopping training early as no improvement observed in last {self.patience} epochs. "
                 f"Best results observed at epoch {self.best_epoch}, best model saved as best.pt.\n"
                 f"To update EarlyStopping(patience={self.patience}) pass a new patience value, "
                 f"i.e. `patience=300` or use `patience=0` to disable EarlyStopping."
             )
         return stop
```

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/utils/triton.py` & `pyppbox-ultralytics-8.1.7/ultralytics/utils/triton.py`

 * *Files identical despite different names*

### Comparing `pyppbox-ultralytics-8.1.42/ultralytics/utils/tuner.py` & `pyppbox-ultralytics-8.1.7/ultralytics/utils/tuner.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Ultralytics YOLO 🚀, AGPL-3.0 license
 
 import subprocess
 
 from ultralytics.cfg import TASK2DATA, TASK2METRIC, get_save_dir
-from ultralytics.utils import DEFAULT_CFG, DEFAULT_CFG_DICT, LOGGER, NUM_THREADS, checks
+from ultralytics.utils import DEFAULT_CFG, DEFAULT_CFG_DICT, LOGGER, NUM_THREADS
 
 
 def run_ray_tune(
     model, space: dict = None, grace_period: int = 10, gpu_per_trial: int = None, max_samples: int = 10, **train_args
 ):
     """
     Runs hyperparameter tuning using Ray Tune.
@@ -36,32 +36,31 @@
     """
 
     LOGGER.info("💡 Learn about RayTune at https://docs.ultralytics.com/integrations/ray-tune")
     if train_args is None:
         train_args = {}
 
     try:
-        subprocess.run("pip install ray[tune]".split(), check=True)  # do not add single quotes here
+        subprocess.run("pip install ray[tune]".split(), check=True)
 
         import ray
         from ray import tune
         from ray.air import RunConfig
         from ray.air.integrations.wandb import WandbLoggerCallback
         from ray.tune.schedulers import ASHAScheduler
     except ImportError:
-        raise ModuleNotFoundError('Ray Tune required but not found. To install run: pip install "ray[tune]"')
+        raise ModuleNotFoundError('Tuning hyperparameters requires Ray Tune. Install with: pip install "ray[tune]"')
 
     try:
         import wandb
 
         assert hasattr(wandb, "__version__")
     except (ImportError, AssertionError):
         wandb = False
 
-    checks.check_version(ray.__version__, "<=2.9.3", "ray")
     default_space = {
         # 'optimizer': tune.choice(['SGD', 'Adam', 'AdamW', 'NAdam', 'RAdam', 'RMSProp']),
         "lr0": tune.uniform(1e-5, 1e-1),
         "lrf": tune.uniform(0.01, 1.0),  # final OneCycleLR learning rate (lr0 * lrf)
         "momentum": tune.uniform(0.6, 0.98),  # SGD momentum/Adam beta1
         "weight_decay": tune.uniform(0.0, 0.001),  # optimizer weight decay 5e-4
         "warmup_epochs": tune.uniform(0.0, 5.0),  # warmup epochs (fractions ok)
@@ -74,15 +73,14 @@
         "degrees": tune.uniform(0.0, 45.0),  # image rotation (+/- deg)
         "translate": tune.uniform(0.0, 0.9),  # image translation (+/- fraction)
         "scale": tune.uniform(0.0, 0.9),  # image scale (+/- gain)
         "shear": tune.uniform(0.0, 10.0),  # image shear (+/- deg)
         "perspective": tune.uniform(0.0, 0.001),  # image perspective (+/- fraction), range 0-0.001
         "flipud": tune.uniform(0.0, 1.0),  # image flip up-down (probability)
         "fliplr": tune.uniform(0.0, 1.0),  # image flip left-right (probability)
-        "bgr": tune.uniform(0.0, 1.0),  # image channel BGR (probability)
         "mosaic": tune.uniform(0.0, 1.0),  # image mixup (probability)
         "mixup": tune.uniform(0.0, 1.0),  # image mixup (probability)
         "copy_paste": tune.uniform(0.0, 1.0),  # segment copy-paste (probability)
     }
 
     # Put the model in ray store
     task = model.task
```

