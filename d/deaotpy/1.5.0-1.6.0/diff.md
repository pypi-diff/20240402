# Comparing `tmp/deaotpy-1.5.0.tar.gz` & `tmp/deaotpy-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deaotpy-1.5.0.tar", last modified: Tue Apr  2 15:47:04 2024, max compression
+gzip compressed data, was "deaotpy-1.6.0.tar", last modified: Tue Apr  2 20:37:47 2024, max compression
```

## Comparing `deaotpy-1.5.0.tar` & `deaotpy-1.6.0.tar`

### file list

```diff
@@ -1,96 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:47:04.739648 deaotpy-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-02 15:42:30.000000 deaotpy-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-02 15:42:30.000000 deaotpy-1.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    16441 2024-04-02 15:47:04.739648 deaotpy-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13858 2024-04-02 15:42:30.000000 deaotpy-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:47:04.715649 deaotpy-1.5.0/aot/
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-02 15:42:31.000000 deaotpy-1.5.0/aot/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 15:47:02.000000 deaotpy-1.5.0/aot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:47:04.719648 deaotpy-1.5.0/aot/configs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 15:47:02.000000 deaotpy-1.5.0/aot/configs/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5579 2024-04-02 15:42:31.000000 deaotpy-1.5.0/aot/configs/default.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:47:04.723649 deaotpy-1.5.0/aot/configs/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 15:47:02.000000 deaotpy-1.5.0/aot/configs/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-02 15:42:31.000000 deaotpy-1.5.0/aot/configs/models/aotb.py
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-02 15:42:31.000000 deaotpy-1.5.0/aot/configs/models/aotl.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-02 15:42:31.000000 deaotpy-1.5.0/aot/configs/models/aots.py
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-02 15:42:31.000000 deaotpy-1.5.0/aot/configs/models/aott.py
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-02 15:42:31.000000 deaotpy-1.5.0/aot/configs/models/deaotb.py
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-02 15:42:31.000000 deaotpy-1.5.0/aot/configs/models/deaotl.py
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-02 15:42:31.000000 deaotpy-1.5.0/aot/configs/models/deaots.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-02 15:42:31.000000 deaotpy-1.5.0/aot/configs/models/deaott.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      957 2024-04-02 15:42:31.000000 deaotpy-1.5.0/aot/configs/models/default.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      420 2024-04-02 15:42:31.000000 deaotpy-1.5.0/aot/configs/models/default_deaot.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-02 15:42:31.000000 deaotpy-1.5.0/aot/configs/models/r101_aotl.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-02 15:42:31.000000 deaotpy-1.5.0/aot/configs/models/r50_aotl.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-02 15:42:31.000000 deaotpy-1.5.0/aot/configs/models/r50_deaotl.py
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-02 15:42:31.000000 deaotpy-1.5.0/aot/configs/models/rs101_aotl.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-02 15:42:31.000000 deaotpy-1.5.0/aot/configs/models/swinb_aotl.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-02 15:42:31.000000 deaotpy-1.5.0/aot/configs/models/swinb_deaotl.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-02 15:42:31.000000 deaotpy-1.5.0/aot/configs/pre.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-02 15:42:31.000000 deaotpy-1.5.0/aot/configs/pre_dav.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-02 15:42:31.000000 deaotpy-1.5.0/aot/configs/pre_ytb.py
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-02 15:42:31.000000 deaotpy-1.5.0/aot/configs/pre_ytb_dav.py
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-02 15:42:31.000000 deaotpy-1.5.0/aot/configs/ytb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:47:04.723649 deaotpy-1.5.0/aot/dataloaders/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:42:31.000000 deaotpy-1.5.0/aot/dataloaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14300 2024-04-02 15:42:31.000000 deaotpy-1.5.0/aot/dataloaders/eval_datasets.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    19828 2024-04-02 15:42:31.000000 deaotpy-1.5.0/aot/dataloaders/image_transforms.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    24642 2024-04-02 15:42:31.000000 deaotpy-1.5.0/aot/dataloaders/train_datasets.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    23571 2024-04-02 15:42:31.000000 deaotpy-1.5.0/aot/dataloaders/video_transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:47:04.723649 deaotpy-1.5.0/aot/networks/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:42:31.000000 deaotpy-1.5.0/aot/networks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:47:04.727649 deaotpy-1.5.0/aot/networks/decoders/
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-02 15:42:31.000000 deaotpy-1.5.0/aot/networks/decoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-02 15:42:31.000000 deaotpy-1.5.0/aot/networks/decoders/fpn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:47:04.727649 deaotpy-1.5.0/aot/networks/encoders/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1381 2024-04-02 15:42:31.000000 deaotpy-1.5.0/aot/networks/encoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8416 2024-04-02 15:42:31.000000 deaotpy-1.5.0/aot/networks/encoders/mobilenetv2.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7895 2024-04-02 15:42:31.000000 deaotpy-1.5.0/aot/networks/encoders/mobilenetv3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:47:04.727649 deaotpy-1.5.0/aot/networks/encoders/resnest/
--rwxr-xr-x   0 runner    (1001) docker     (127)       23 2024-04-02 15:42:31.000000 deaotpy-1.5.0/aot/networks/encoders/resnest/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3343 2024-04-02 15:42:31.000000 deaotpy-1.5.0/aot/networks/encoders/resnest/resnest.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16470 2024-04-02 15:42:31.000000 deaotpy-1.5.0/aot/networks/encoders/resnest/resnet.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4467 2024-04-02 15:42:31.000000 deaotpy-1.5.0/aot/networks/encoders/resnest/splat.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6688 2024-04-02 15:42:31.000000 deaotpy-1.5.0/aot/networks/encoders/resnet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:47:04.731649 deaotpy-1.5.0/aot/networks/encoders/swin/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-02 15:42:31.000000 deaotpy-1.5.0/aot/networks/encoders/swin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-02 15:42:31.000000 deaotpy-1.5.0/aot/networks/encoders/swin/build.py
--rw-r--r--   0 runner    (1001) docker     (127)    27341 2024-04-02 15:42:31.000000 deaotpy-1.5.0/aot/networks/encoders/swin/swin_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:47:04.731649 deaotpy-1.5.0/aot/networks/engines/
--rwxr-xr-x   0 runner    (1001) docker     (127)      685 2024-04-02 15:42:31.000000 deaotpy-1.5.0/aot/networks/engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24634 2024-04-02 15:42:31.000000 deaotpy-1.5.0/aot/networks/engines/aot_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-04-02 15:42:31.000000 deaotpy-1.5.0/aot/networks/engines/deaot_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:47:04.731649 deaotpy-1.5.0/aot/networks/layers/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:42:31.000000 deaotpy-1.5.0/aot/networks/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32778 2024-04-02 15:42:31.000000 deaotpy-1.5.0/aot/networks/layers/attention.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5111 2024-04-02 15:42:31.000000 deaotpy-1.5.0/aot/networks/layers/basic.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6698 2024-04-02 15:42:31.000000 deaotpy-1.5.0/aot/networks/layers/loss.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1700 2024-04-02 15:42:31.000000 deaotpy-1.5.0/aot/networks/layers/normalization.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2806 2024-04-02 15:42:31.000000 deaotpy-1.5.0/aot/networks/layers/position.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    24828 2024-04-02 15:42:31.000000 deaotpy-1.5.0/aot/networks/layers/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:47:04.735648 deaotpy-1.5.0/aot/networks/models/
--rwxr-xr-x   0 runner    (1001) docker     (127)      336 2024-04-02 15:42:31.000000 deaotpy-1.5.0/aot/networks/models/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4530 2024-04-02 15:42:31.000000 deaotpy-1.5.0/aot/networks/models/aot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-04-02 15:42:31.000000 deaotpy-1.5.0/aot/networks/models/deaot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:47:04.735648 deaotpy-1.5.0/aot/utils/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:42:32.000000 deaotpy-1.5.0/aot/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6200 2024-04-02 15:42:32.000000 deaotpy-1.5.0/aot/utils/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-02 15:42:32.000000 deaotpy-1.5.0/aot/utils/cp_ckpt.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3561 2024-04-02 15:42:32.000000 deaotpy-1.5.0/aot/utils/ema.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      443 2024-04-02 15:42:32.000000 deaotpy-1.5.0/aot/utils/eval.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6075 2024-04-02 15:42:32.000000 deaotpy-1.5.0/aot/utils/image.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3454 2024-04-02 15:42:32.000000 deaotpy-1.5.0/aot/utils/learning.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      829 2024-04-02 15:42:32.000000 deaotpy-1.5.0/aot/utils/math.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      860 2024-04-02 15:42:32.000000 deaotpy-1.5.0/aot/utils/meters.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1102 2024-04-02 15:42:32.000000 deaotpy-1.5.0/aot/utils/metric.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:47:04.739648 deaotpy-1.5.0/deaotpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16441 2024-04-02 15:47:04.000000 deaotpy-1.5.0/deaotpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-02 15:47:04.000000 deaotpy-1.5.0/deaotpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 15:47:04.000000 deaotpy-1.5.0/deaotpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-02 15:47:04.000000 deaotpy-1.5.0/deaotpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-02 15:47:04.000000 deaotpy-1.5.0/deaotpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-02 15:42:30.000000 deaotpy-1.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-02 15:42:30.000000 deaotpy-1.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 15:47:04.739648 deaotpy-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-04-02 15:42:30.000000 deaotpy-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:37:47.863124 deaotpy-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-02 20:17:42.000000 deaotpy-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16438 2024-04-02 20:37:47.863124 deaotpy-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-04-02 20:17:42.000000 deaotpy-1.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:37:47.831124 deaotpy-1.6.0/aot/
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13858 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:37:47.835124 deaotpy-1.6.0/aot/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/configs/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5579 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/configs/default.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:37:47.843124 deaotpy-1.6.0/aot/configs/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/configs/models/aotb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/configs/models/aotl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/configs/models/aots.py
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/configs/models/aott.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/configs/models/deaotb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/configs/models/deaotl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/configs/models/deaots.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/configs/models/deaott.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      957 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/configs/models/default.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      420 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/configs/models/default_deaot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/configs/models/r101_aotl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/configs/models/r50_aotl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/configs/models/r50_deaotl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/configs/models/rs101_aotl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/configs/models/swinb_aotl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/configs/models/swinb_deaotl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/configs/pre.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/configs/pre_dav.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/configs/pre_ytb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/configs/pre_ytb_dav.py
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/configs/ytb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:37:47.843124 deaotpy-1.6.0/aot/dataloaders/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/dataloaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14304 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/dataloaders/eval_datasets.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19828 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/dataloaders/image_transforms.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24646 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/dataloaders/train_datasets.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23575 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/dataloaders/video_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:37:47.843124 deaotpy-1.6.0/aot/networks/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/networks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:37:47.847124 deaotpy-1.6.0/aot/networks/decoders/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/networks/decoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/networks/decoders/fpn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:37:47.847124 deaotpy-1.6.0/aot/networks/encoders/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1381 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/networks/encoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8420 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/networks/encoders/mobilenetv2.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7899 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/networks/encoders/mobilenetv3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:37:47.847124 deaotpy-1.6.0/aot/networks/encoders/resnest/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       23 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/networks/encoders/resnest/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3343 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/networks/encoders/resnest/resnest.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16474 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/networks/encoders/resnest/resnet.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4467 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/networks/encoders/resnest/splat.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6692 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/networks/encoders/resnet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:37:47.851124 deaotpy-1.6.0/aot/networks/encoders/swin/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/networks/encoders/swin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/networks/encoders/swin/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27345 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/networks/encoders/swin/swin_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:37:47.851124 deaotpy-1.6.0/aot/networks/engines/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      685 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/networks/engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24646 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/networks/engines/aot_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/networks/engines/deaot_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:37:47.855124 deaotpy-1.6.0/aot/networks/layers/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/networks/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32782 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/networks/layers/attention.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5111 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/networks/layers/basic.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6698 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/networks/layers/loss.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1700 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/networks/layers/normalization.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2810 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/networks/layers/position.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24836 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/networks/layers/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:37:47.855124 deaotpy-1.6.0/aot/networks/managers/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    25895 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/networks/managers/evaluator.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    29712 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/networks/managers/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:37:47.855124 deaotpy-1.6.0/aot/networks/models/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      336 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/networks/models/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4546 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/networks/models/aot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/networks/models/deaot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:37:47.855124 deaotpy-1.6.0/aot/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)    12850 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/tools/demo.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3472 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/tools/eval.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2668 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/tools/train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:37:47.859124 deaotpy-1.6.0/aot/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6200 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/utils/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/utils/cp_ckpt.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3561 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/utils/ema.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      443 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/utils/eval.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6075 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/utils/image.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3454 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/utils/learning.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      829 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/utils/math.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      860 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/utils/meters.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1102 2024-04-02 20:17:45.000000 deaotpy-1.6.0/aot/utils/metric.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:37:47.863124 deaotpy-1.6.0/deaotpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16438 2024-04-02 20:37:47.000000 deaotpy-1.6.0/deaotpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-04-02 20:37:47.000000 deaotpy-1.6.0/deaotpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 20:37:47.000000 deaotpy-1.6.0/deaotpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-02 20:37:47.000000 deaotpy-1.6.0/deaotpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-02 20:37:47.000000 deaotpy-1.6.0/deaotpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-02 20:17:42.000000 deaotpy-1.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 20:37:47.863124 deaotpy-1.6.0/setup.cfg
```

### Comparing `deaotpy-1.5.0/LICENSE` & `deaotpy-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deaotpy-1.5.0/PKG-INFO` & `deaotpy-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 Metadata-Version: 2.1
 Name: deaotpy
-Version: 1.5.0
+Version: 1.6.0
 Summary: Decoupling Features in Hierarchical Propagation for Video Object Segmentation.
-Home-page: https://github.com/yoxu515/aot-benchmark
 License: BSD 3-Clause License
         
         Copyright (c) 2020, z-x-yang
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
@@ -29,15 +28,16 @@
         FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
         DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
         SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
         CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         
-Keywords: machine-learning,deep-learning,pytorch,vision,object segmentation,video
+Project-URL: repository, https://github.com/yoxu515/aot-benchmark
+Keywords: deep-learning,pytorch,vision,object-segmentation,video
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.10
```

### Comparing `deaotpy-1.5.0/README.md` & `deaotpy-1.6.0/aot/README.md`

 * *Files identical despite different names*

### Comparing `deaotpy-1.5.0/aot/LICENSE` & `deaotpy-1.6.0/aot/LICENSE`

 * *Files identical despite different names*

### Comparing `deaotpy-1.5.0/aot/configs/default.py` & `deaotpy-1.6.0/aot/configs/default.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.5.0/aot/configs/models/default.py` & `deaotpy-1.6.0/aot/configs/models/default.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.5.0/aot/configs/models/r101_aotl.py` & `deaotpy-1.6.0/aot/configs/models/r101_aotl.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.5.0/aot/configs/models/r50_aotl.py` & `deaotpy-1.6.0/aot/configs/models/r50_aotl.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.5.0/aot/configs/models/r50_deaotl.py` & `deaotpy-1.6.0/aot/configs/models/r50_deaotl.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.5.0/aot/configs/models/rs101_aotl.py` & `deaotpy-1.6.0/aot/configs/models/rs101_aotl.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.5.0/aot/configs/models/swinb_aotl.py` & `deaotpy-1.6.0/aot/configs/models/swinb_aotl.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.5.0/aot/configs/models/swinb_deaotl.py` & `deaotpy-1.6.0/aot/configs/models/swinb_deaotl.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.5.0/aot/configs/pre.py` & `deaotpy-1.6.0/aot/configs/pre.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.5.0/aot/configs/pre_dav.py` & `deaotpy-1.6.0/aot/configs/pre_dav.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.5.0/aot/configs/pre_ytb.py` & `deaotpy-1.6.0/aot/configs/pre_ytb.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.5.0/aot/configs/pre_ytb_dav.py` & `deaotpy-1.6.0/aot/configs/pre_ytb_dav.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.5.0/aot/dataloaders/eval_datasets.py` & `deaotpy-1.6.0/aot/dataloaders/eval_datasets.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import json
 import cv2
 from PIL import Image
 
 import numpy as np
 from torch.utils.data import Dataset
 
-from utils.image import _palette
+from aot.utils.image import _palette
 
 
 class VOSTest(Dataset):
     def __init__(self,
                  image_root,
                  label_root,
                  seq_name,
```

### Comparing `deaotpy-1.5.0/aot/dataloaders/image_transforms.py` & `deaotpy-1.6.0/aot/dataloaders/image_transforms.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.5.0/aot/dataloaders/train_datasets.py` & `deaotpy-1.6.0/aot/dataloaders/train_datasets.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from PIL import Image
 
 import numpy as np
 import torch
 from torch.utils.data import Dataset
 import torchvision.transforms as TF
 
-import dataloaders.image_transforms as IT
+import aot.dataloaders.image_transforms as IT
 
 cv2.setNumThreads(0)
 
 
 def _get_images(sample):
     return [sample['ref_img'], sample['prev_img']] + sample['curr_img']
```

### Comparing `deaotpy-1.5.0/aot/dataloaders/video_transforms.py` & `deaotpy-1.6.0/aot/dataloaders/video_transforms.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import random
 import cv2
 import numpy as np
 from PIL import Image
 
 import torch
 import torchvision.transforms as TF
-import dataloaders.image_transforms as IT
+import aot.dataloaders.image_transforms as IT
 
 cv2.setNumThreads(0)
 
 
 class Resize(object):
     """Rescale the image in a sample to a given size.
```

### Comparing `deaotpy-1.5.0/aot/networks/decoders/fpn.py` & `deaotpy-1.6.0/aot/networks/decoders/fpn.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
-from networks.layers.basic import ConvGN
+from aot.networks.layers.basic import ConvGN
 
 
 class FPNSegmentationHead(nn.Module):
     def __init__(self,
                  in_dim,
                  out_dim,
                  decode_intermediate_input=True,
```

### Comparing `deaotpy-1.5.0/aot/networks/encoders/__init__.py` & `deaotpy-1.6.0/aot/networks/encoders/__init__.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.5.0/aot/networks/encoders/mobilenetv2.py` & `deaotpy-1.6.0/aot/networks/encoders/mobilenetv2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from torch import nn
 from torch import Tensor
 from typing import Callable, Optional, List
-from utils.learning import freeze_params
+from aot.utils.learning import freeze_params
 
 __all__ = ['MobileNetV2']
 
 
 def _make_divisible(v: float,
                     divisor: int,
                     min_value: Optional[int] = None) -> int:
```

### Comparing `deaotpy-1.5.0/aot/networks/encoders/mobilenetv3.py` & `deaotpy-1.6.0/aot/networks/encoders/mobilenetv3.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 Andrew Howard, Mark Sandler, Grace Chu, Liang-Chieh Chen, Bo Chen, Mingxing Tan, Weijun Wang, Yukun Zhu, Ruoming Pang, Vijay Vasudevan, Quoc V. Le, Hartwig Adam. (2019).
 Searching for MobileNetV3
 arXiv preprint arXiv:1905.02244.
 """
 
 import torch.nn as nn
 import math
-from utils.learning import freeze_params
+from aot.utils.learning import freeze_params
 
 
 def _make_divisible(v, divisor, min_value=None):
     """
     This function is taken from the original tf repo.
     It ensures that all layers have a channel number that is divisible by 8
     It can be seen here:
```

### Comparing `deaotpy-1.5.0/aot/networks/encoders/resnest/resnest.py` & `deaotpy-1.6.0/aot/networks/encoders/resnest/resnest.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.5.0/aot/networks/encoders/resnest/resnet.py` & `deaotpy-1.6.0/aot/networks/encoders/resnest/resnet.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import math
 import torch.nn as nn
 
 from .splat import SplAtConv2d, DropBlock2D
-from utils.learning import freeze_params
+from aot.utils.learning import freeze_params
 
 __all__ = ['ResNet', 'Bottleneck']
 
 _url_format = 'https://s3.us-west-1.wasabisys.com/resnest/torch/{}-{}.pth'
 
 _model_sha256 = {name: checksum for checksum, name in []}
```

### Comparing `deaotpy-1.5.0/aot/networks/encoders/resnest/splat.py` & `deaotpy-1.6.0/aot/networks/encoders/resnest/splat.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.5.0/aot/networks/encoders/resnet.py` & `deaotpy-1.6.0/aot/networks/encoders/resnet.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import math
 import torch.nn as nn
-from utils.learning import freeze_params
+from aot.utils.learning import freeze_params
 
 
 class Bottleneck(nn.Module):
     expansion = 4
 
     def __init__(self,
                  inplanes,
```

### Comparing `deaotpy-1.5.0/aot/networks/encoders/swin/build.py` & `deaotpy-1.6.0/aot/networks/encoders/swin/build.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.5.0/aot/networks/encoders/swin/swin_transformer.py` & `deaotpy-1.6.0/aot/networks/encoders/swin/swin_transformer.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 import numpy as np
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 import torch.utils.checkpoint as checkpoint
 
-from networks.layers.basic import DropPath
+from aot.networks.layers.basic import DropPath
 
 
 def _ntuple(n):
     def parse(x):
         if isinstance(x, collections.abc.Iterable):
             return x
         return tuple(repeat(x, n))
```

### Comparing `deaotpy-1.5.0/aot/networks/engines/__init__.py` & `deaotpy-1.6.0/aot/networks/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.5.0/aot/networks/engines/aot_engine.py` & `deaotpy-1.6.0/aot/networks/engines/aot_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
 import numpy as np
 
-from utils.math import generate_permute_matrix
-from utils.image import one_hot_mask
+from aot.utils.math import generate_permute_matrix
+from aot.utils.image import one_hot_mask
 
-from networks.layers.basic import seq_to_2d
+from aot.networks.layers.basic import seq_to_2d
 
 
 class AOTEngine(nn.Module):
     def __init__(self,
                  aot_model,
                  gpu_id=0,
                  long_term_mem_gap=9999,
```

### Comparing `deaotpy-1.5.0/aot/networks/engines/deaot_engine.py` & `deaotpy-1.6.0/aot/networks/engines/deaot_engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 
 from utils.image import one_hot_mask
 
-from networks.layers.basic import seq_to_2d
-from networks.engines.aot_engine import AOTEngine, AOTInferEngine
+from aot.networks.layers.basic import seq_to_2d
+from aot.networks.engines.aot_engine import AOTEngine, AOTInferEngine
 
 
 class DeAOTEngine(AOTEngine):
     def __init__(self,
                  aot_model,
                  gpu_id=0,
                  long_term_mem_gap=9999,
```

### Comparing `deaotpy-1.5.0/aot/networks/layers/attention.py` & `deaotpy-1.6.0/aot/networks/layers/attention.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import math
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
-from networks.layers.basic import DropOutLogit, ScaleOffset, DWConv2d
+from aot.networks.layers.basic import DropOutLogit, ScaleOffset, DWConv2d
 
 
 def multiply_by_ychunks(x, y, chunks=1):
     if chunks <= 1:
         return x @ y
     else:
         return torch.cat([x @ _y for _y in y.chunk(chunks, dim=-1)], dim=-1)
```

### Comparing `deaotpy-1.5.0/aot/networks/layers/basic.py` & `deaotpy-1.6.0/aot/networks/layers/basic.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.5.0/aot/networks/layers/loss.py` & `deaotpy-1.6.0/aot/networks/layers/loss.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.5.0/aot/networks/layers/normalization.py` & `deaotpy-1.6.0/aot/networks/layers/normalization.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.5.0/aot/networks/layers/position.py` & `deaotpy-1.6.0/aot/networks/layers/position.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import math
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
-from utils.math import truncated_normal_
+from aot.utils.math import truncated_normal_
 
 
 class Downsample2D(nn.Module):
     def __init__(self, mode='nearest', scale=4):
         super().__init__()
         self.mode = mode
         self.scale = scale
```

### Comparing `deaotpy-1.5.0/aot/networks/layers/transformer.py` & `deaotpy-1.6.0/aot/networks/layers/transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import torch
 import torch.nn.functional as F
 from torch import nn
 
-from networks.layers.basic import DropPath, GroupNorm1D, GNActDWConv2d, seq_to_2d, ScaleOffset, mask_out
-from networks.layers.attention import silu, MultiheadAttention, MultiheadLocalAttentionV2, MultiheadLocalAttentionV3, GatedPropagation, LocalGatedPropagation
+from aot.networks.layers.basic import DropPath, GroupNorm1D, GNActDWConv2d, seq_to_2d, ScaleOffset, mask_out
+from aot.networks.layers.attention import silu, MultiheadAttention, MultiheadLocalAttentionV2, MultiheadLocalAttentionV3, GatedPropagation, LocalGatedPropagation
 
 
 def _get_norm(indim, type='ln', groups=8):
     if type == 'gn':
         return GroupNorm1D(indim, groups)
     else:
         return nn.LayerNorm(indim)
```

### Comparing `deaotpy-1.5.0/aot/networks/models/aot.py` & `deaotpy-1.6.0/aot/networks/models/aot.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import torch.nn as nn
 
-from networks.encoders import build_encoder
-from networks.layers.transformer import LongShortTermTransformer
-from networks.decoders import build_decoder
-from networks.layers.position import PositionEmbeddingSine
+from aot.networks.encoders import build_encoder
+from aot.networks.layers.transformer import LongShortTermTransformer
+from aot.networks.decoders import build_decoder
+from aot.networks.layers.position import PositionEmbeddingSine
 
 
 class AOT(nn.Module):
     def __init__(self, cfg, encoder='mobilenetv2', decoder='fpn'):
         super().__init__()
         self.cfg = cfg
         self.max_obj_num = cfg.MODEL_MAX_OBJ_NUM
```

### Comparing `deaotpy-1.5.0/aot/networks/models/deaot.py` & `deaotpy-1.6.0/aot/networks/models/deaot.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import torch.nn as nn
 
-from networks.layers.transformer import DualBranchGPM
-from networks.models.aot import AOT
-from networks.decoders import build_decoder
+from aot.networks.layers.transformer import DualBranchGPM
+from aot.networks.models.aot import AOT
+from aot.networks.decoders import build_decoder
 
 
 class DeAOT(AOT):
     def __init__(self, cfg, encoder='mobilenetv2', decoder='fpn'):
         super().__init__(cfg, encoder, decoder)
 
         self.LSTT = DualBranchGPM(
```

### Comparing `deaotpy-1.5.0/aot/utils/checkpoint.py` & `deaotpy-1.6.0/aot/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.5.0/aot/utils/cp_ckpt.py` & `deaotpy-1.6.0/aot/utils/cp_ckpt.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.5.0/aot/utils/ema.py` & `deaotpy-1.6.0/aot/utils/ema.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.5.0/aot/utils/image.py` & `deaotpy-1.6.0/aot/utils/image.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.5.0/aot/utils/learning.py` & `deaotpy-1.6.0/aot/utils/learning.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.5.0/aot/utils/math.py` & `deaotpy-1.6.0/aot/utils/math.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.5.0/aot/utils/meters.py` & `deaotpy-1.6.0/aot/utils/meters.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.5.0/aot/utils/metric.py` & `deaotpy-1.6.0/aot/utils/metric.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.5.0/deaotpy.egg-info/PKG-INFO` & `deaotpy-1.6.0/deaotpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 Metadata-Version: 2.1
 Name: deaotpy
-Version: 1.5.0
+Version: 1.6.0
 Summary: Decoupling Features in Hierarchical Propagation for Video Object Segmentation.
-Home-page: https://github.com/yoxu515/aot-benchmark
 License: BSD 3-Clause License
         
         Copyright (c) 2020, z-x-yang
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
@@ -29,15 +28,16 @@
         FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
         DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
         SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
         CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         
-Keywords: machine-learning,deep-learning,pytorch,vision,object segmentation,video
+Project-URL: repository, https://github.com/yoxu515/aot-benchmark
+Keywords: deep-learning,pytorch,vision,object-segmentation,video
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.10
```

### Comparing `deaotpy-1.5.0/deaotpy.egg-info/SOURCES.txt` & `deaotpy-1.6.0/deaotpy.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 LICENSE
-MANIFEST.in
 README.md
 pyproject.toml
-requirements.txt
-setup.py
 aot/LICENSE
+aot/README.md
 aot/__init__.py
 aot/configs/__init__.py
 aot/configs/default.py
 aot/configs/pre.py
 aot/configs/pre_dav.py
 aot/configs/pre_ytb.py
 aot/configs/pre_ytb_dav.py
 aot/configs/ytb.py
-aot/configs/models/__init__.py
 aot/configs/models/aotb.py
 aot/configs/models/aotl.py
 aot/configs/models/aots.py
 aot/configs/models/aott.py
 aot/configs/models/deaotb.py
 aot/configs/models/deaotl.py
 aot/configs/models/deaots.py
@@ -55,17 +52,22 @@
 aot/networks/layers/__init__.py
 aot/networks/layers/attention.py
 aot/networks/layers/basic.py
 aot/networks/layers/loss.py
 aot/networks/layers/normalization.py
 aot/networks/layers/position.py
 aot/networks/layers/transformer.py
+aot/networks/managers/evaluator.py
+aot/networks/managers/trainer.py
 aot/networks/models/__init__.py
 aot/networks/models/aot.py
 aot/networks/models/deaot.py
+aot/tools/demo.py
+aot/tools/eval.py
+aot/tools/train.py
 aot/utils/__init__.py
 aot/utils/checkpoint.py
 aot/utils/cp_ckpt.py
 aot/utils/ema.py
 aot/utils/eval.py
 aot/utils/image.py
 aot/utils/learning.py
```

