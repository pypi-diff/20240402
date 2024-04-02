# Comparing `tmp/torch_ecg-0.0.8.tar.gz` & `tmp/torch_ecg-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/torch_ecg-0.0.8.tar", last modified: Mon Mar 28 16:42:03 2022, max compression
+gzip compressed data, was "dist/torch_ecg-0.0.9.tar", last modified: Wed Mar 30 15:13:52 2022, max compression
```

## Comparing `torch_ecg-0.0.8.tar` & `torch_ecg-0.0.9.tar`

### file list

```diff
@@ -1,172 +1,175 @@
-drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-03-28 16:42:03.000000 torch_ecg-0.0.8/
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    14426 2022-03-27 02:40:45.000000 torch_ecg-0.0.8/README.md
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     1330 2022-03-28 15:33:03.000000 torch_ecg-0.0.8/setup.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)       38 2022-03-28 16:42:03.000000 torch_ecg-0.0.8/setup.cfg
-drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-03-28 16:42:03.000000 torch_ecg-0.0.8/torch_ecg/
-drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-03-28 16:42:03.000000 torch_ecg-0.0.8/torch_ecg/preprocessors/
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      473 2022-03-24 09:32:39.000000 torch_ecg-0.0.8/torch_ecg/preprocessors/__init__.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     2152 2022-03-28 08:48:29.000000 torch_ecg-0.0.8/torch_ecg/preprocessors/resample.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     5697 2022-03-28 08:48:29.000000 torch_ecg-0.0.8/torch_ecg/preprocessors/normalize.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     5783 2022-03-28 08:48:29.000000 torch_ecg-0.0.8/torch_ecg/preprocessors/preproc_manager.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     2137 2022-03-28 08:48:29.000000 torch_ecg-0.0.8/torch_ecg/preprocessors/baseline_remove.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     2121 2022-03-28 08:48:29.000000 torch_ecg-0.0.8/torch_ecg/preprocessors/bandpass.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      859 2022-03-24 09:32:39.000000 torch_ecg-0.0.8/torch_ecg/__init__.py
-drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-03-28 16:42:03.000000 torch_ecg-0.0.8/torch_ecg/augmenters/
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    20236 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/augmenters/stretch_compress.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     2854 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/augmenters/cutmix.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     4964 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/augmenters/random_masking.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     3497 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/augmenters/random_flip.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      636 2022-03-24 09:32:39.000000 torch_ecg-0.0.8/torch_ecg/augmenters/__init__.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    11018 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/augmenters/baseline_wander.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     3915 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/augmenters/mixup.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     6317 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/augmenters/augmenter_manager.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     2471 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/augmenters/base.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     4556 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/augmenters/random_renormalize.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     3105 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/augmenters/label_smooth.py
-drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-03-28 16:42:03.000000 torch_ecg-0.0.8/torch_ecg/databases/
-drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-03-28 16:42:03.000000 torch_ecg-0.0.8/torch_ecg/databases/aux_data/
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    28258 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/databases/aux_data/cinc2021_aux_data.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      458 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/databases/aux_data/__init__.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     6078 2022-03-27 02:26:51.000000 torch_ecg-0.0.8/torch_ecg/databases/aux_data/physionet_dbs.csv.tar.gz
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    51295 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/databases/aux_data/cinc2020_aux_data.py
-drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-03-28 16:42:03.000000 torch_ecg-0.0.8/torch_ecg/databases/physionet_databases/
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    67467 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/databases/physionet_databases/cinc2020.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    94226 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/databases/physionet_databases/cinc2021.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    13331 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/databases/physionet_databases/apnea_ecg.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    32370 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/databases/physionet_databases/ludb.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    15197 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/databases/physionet_databases/mitdb.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      708 2022-03-24 09:32:39.000000 torch_ecg-0.0.8/torch_ecg/databases/physionet_databases/__init__.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    24734 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/databases/physionet_databases/ltafdb.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     9765 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/databases/physionet_databases/cinc2017.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     3312 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/databases/physionet_databases/cinc2018.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    17779 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/databases/physionet_databases/afdb.py
-drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-03-28 16:42:03.000000 torch_ecg-0.0.8/torch_ecg/databases/nsrr_databases/
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      104 2022-03-24 09:32:39.000000 torch_ecg-0.0.8/torch_ecg/databases/nsrr_databases/__init__.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    71967 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/databases/nsrr_databases/shhs.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      870 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/databases/__init__.py
-drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-03-28 16:42:03.000000 torch_ecg-0.0.8/torch_ecg/databases/cpsc_databases/
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    22526 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/databases/cpsc_databases/cpsc2018.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    14599 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/databases/cpsc_databases/cpsc2019.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    61714 2022-03-27 08:25:33.000000 torch_ecg-0.0.8/torch_ecg/databases/cpsc_databases/cpsc2021.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      257 2022-03-24 09:32:39.000000 torch_ecg-0.0.8/torch_ecg/databases/cpsc_databases/__init__.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    32777 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/databases/cpsc_databases/cpsc2020.py
-drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-03-28 16:42:03.000000 torch_ecg-0.0.8/torch_ecg/databases/datasets/
-drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-03-28 16:42:03.000000 torch_ecg-0.0.8/torch_ecg/databases/datasets/ludb/
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      137 2022-03-24 09:32:39.000000 torch_ecg-0.0.8/torch_ecg/databases/datasets/ludb/__init__.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     3696 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/databases/datasets/ludb/ludb_cfg.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     8108 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/databases/datasets/ludb/ludb_dataset.py
-drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-03-28 16:42:03.000000 torch_ecg-0.0.8/torch_ecg/databases/datasets/cinc2020/
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     6372 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/databases/datasets/cinc2020/cinc2020_cfg.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      161 2022-03-24 09:32:39.000000 torch_ecg-0.0.8/torch_ecg/databases/datasets/cinc2020/__init__.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    15424 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/databases/datasets/cinc2020/cinc2020_dataset.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)        0 2022-03-24 09:32:39.000000 torch_ecg-0.0.8/torch_ecg/databases/datasets/__init__.py
-drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-03-28 16:42:03.000000 torch_ecg-0.0.8/torch_ecg/databases/datasets/cpsc2021/
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    61592 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/databases/datasets/cpsc2021/cpsc2021_dataset.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      161 2022-03-24 09:32:39.000000 torch_ecg-0.0.8/torch_ecg/databases/datasets/cpsc2021/__init__.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     8585 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/databases/datasets/cpsc2021/cpsc2021_cfg.py
-drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-03-28 16:42:03.000000 torch_ecg-0.0.8/torch_ecg/databases/datasets/cpsc2020/
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)        0 2022-03-24 09:32:39.000000 torch_ecg-0.0.8/torch_ecg/databases/datasets/cpsc2020/cpsc2020_dataset.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)        0 2022-03-24 09:32:39.000000 torch_ecg-0.0.8/torch_ecg/databases/datasets/cpsc2020/cpsc2020_cfg.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)        0 2022-03-24 09:32:39.000000 torch_ecg-0.0.8/torch_ecg/databases/datasets/cpsc2020/__init__.py
-drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-03-28 16:42:03.000000 torch_ecg-0.0.8/torch_ecg/databases/datasets/cpsc2019/
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     4307 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/databases/datasets/cpsc2019/cpsc2019_cfg.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      161 2022-03-24 09:32:39.000000 torch_ecg-0.0.8/torch_ecg/databases/datasets/cpsc2019/__init__.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     6738 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/databases/datasets/cpsc2019/cpsc2019_dataset.py
-drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-03-28 16:42:03.000000 torch_ecg-0.0.8/torch_ecg/databases/datasets/cinc2021/
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      161 2022-03-24 09:32:39.000000 torch_ecg-0.0.8/torch_ecg/databases/datasets/cinc2021/__init__.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     6568 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/databases/datasets/cinc2021/cinc2021_cfg.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    19921 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/databases/datasets/cinc2021/cinc2021_dataset.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    24594 2022-03-28 08:48:29.000000 torch_ecg-0.0.8/torch_ecg/databases/base.py
-drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-03-28 16:42:03.000000 torch_ecg-0.0.8/torch_ecg/models/
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    17383 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/models/loss.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)   149046 2022-03-28 14:17:53.000000 torch_ecg-0.0.8/torch_ecg/models/_nets.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      254 2022-03-24 09:32:39.000000 torch_ecg-0.0.8/torch_ecg/models/__init__.py
-drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-03-28 16:42:03.000000 torch_ecg-0.0.8/torch_ecg/models/unets/
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      223 2022-03-24 09:32:39.000000 torch_ecg-0.0.8/torch_ecg/models/unets/__init__.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    21625 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/models/unets/ecg_unet.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    25438 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/models/unets/ecg_subtract_unet.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     9053 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/models/rr_lstm.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    13932 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/models/ecg_seq_lab_net.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    16518 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/models/ecg_crnn.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      489 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/models/ecg_fcn.py
-drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-03-28 16:42:03.000000 torch_ecg-0.0.8/torch_ecg/models/transformers/
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)       81 2022-03-24 09:32:39.000000 torch_ecg-0.0.8/torch_ecg/models/transformers/__init__.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     3407 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/models/transformers/transformer.py
-drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-03-28 16:42:03.000000 torch_ecg-0.0.8/torch_ecg/models/cnn/
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    29119 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/models/cnn/densenet.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     1377 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/models/cnn/ho_resnet.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    34355 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/models/cnn/resnet.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      224 2022-03-24 09:32:39.000000 torch_ecg-0.0.8/torch_ecg/models/cnn/__init__.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    29950 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/models/cnn/mobilenet.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     1721 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/models/cnn/darknet.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     2697 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/models/cnn/efficientnet.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    33937 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/models/cnn/xception.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     8142 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/models/cnn/vgg.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    15375 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/models/cnn/multi_scopic.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     5226 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/models/grad_cam.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     2958 2022-03-28 08:48:29.000000 torch_ecg-0.0.8/torch_ecg/cfg.py
-drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-03-28 16:42:03.000000 torch_ecg-0.0.8/torch_ecg/_preprocessors/
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      690 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/_preprocessors/__init__.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     8790 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/_preprocessors/base.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     2251 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/_preprocessors/resample.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     7082 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/_preprocessors/normalize.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     5903 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/_preprocessors/preproc_manager.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     2228 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/_preprocessors/baseline_remove.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     2649 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/_preprocessors/bandpass.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)       22 2022-03-28 16:40:36.000000 torch_ecg-0.0.8/torch_ecg/version.py
-drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-03-28 16:42:03.000000 torch_ecg-0.0.8/torch_ecg/model_configs/
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     4614 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/model_configs/__init__.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      500 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/model_configs/mlp.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      560 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/model_configs/rnn.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     2326 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/model_configs/rr_lstm.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     2681 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/model_configs/ecg_seq_lab_net.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     2781 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/model_configs/ecg_unet.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     9325 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/model_configs/ecg_crnn.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     2545 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/model_configs/ati_cnn.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     1156 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/model_configs/ecg_yolo.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      989 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/model_configs/attn.py
-drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-03-28 16:42:03.000000 torch_ecg-0.0.8/torch_ecg/model_configs/cnn/
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      956 2022-03-24 09:32:39.000000 torch_ecg-0.0.8/torch_ecg/model_configs/cnn/densenet.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    16643 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/model_configs/cnn/resnet.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     3867 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/model_configs/cnn/__init__.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     4213 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/model_configs/cnn/mobilenet.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     1961 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/model_configs/cnn/xception.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     1776 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/model_configs/cnn/cpsc.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     1679 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/model_configs/cnn/vgg.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     3080 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/model_configs/cnn/multi_scopic.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     3858 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/torch_ecg/model_configs/ecg_subtract_unet.py
-drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-03-28 16:42:03.000000 torch_ecg-0.0.8/torch_ecg/utils/
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    31144 2022-03-28 08:48:29.000000 torch_ecg-0.0.8/torch_ecg/utils/utils_signal.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     6540 2022-03-28 08:48:29.000000 torch_ecg-0.0.8/torch_ecg/utils/rpeaks.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     8285 2022-03-28 08:48:29.000000 torch_ecg-0.0.8/torch_ecg/utils/utils_signal_t.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     4634 2022-03-28 16:40:36.000000 torch_ecg-0.0.8/torch_ecg/utils/download.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    18063 2022-03-28 08:48:29.000000 torch_ecg-0.0.8/torch_ecg/utils/loggers.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)        0 2022-03-24 09:32:39.000000 torch_ecg-0.0.8/torch_ecg/utils/__init__.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     1292 2022-03-28 08:48:29.000000 torch_ecg-0.0.8/torch_ecg/utils/utils_metrics.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    12504 2022-03-28 08:48:29.000000 torch_ecg-0.0.8/torch_ecg/utils/preproc.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     3695 2022-03-28 08:48:29.000000 torch_ecg-0.0.8/torch_ecg/utils/edr.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    25234 2022-03-28 08:48:29.000000 torch_ecg-0.0.8/torch_ecg/utils/trainer.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    27056 2022-03-28 08:48:29.000000 torch_ecg-0.0.8/torch_ecg/utils/ecg_arrhythmia_knowledge.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     7054 2022-03-28 08:48:29.000000 torch_ecg-0.0.8/torch_ecg/utils/outputs.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    31532 2022-03-28 08:48:29.000000 torch_ecg-0.0.8/torch_ecg/utils/utils_interval.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     3303 2022-03-28 08:48:29.000000 torch_ecg-0.0.8/torch_ecg/utils/nas.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    46011 2022-03-28 08:48:29.000000 torch_ecg-0.0.8/torch_ecg/utils/misc.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    19403 2022-03-28 08:48:29.000000 torch_ecg-0.0.8/torch_ecg/utils/pantompkins.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    28784 2022-03-28 08:48:29.000000 torch_ecg-0.0.8/torch_ecg/utils/utils_nn.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    17482 2022-03-28 16:42:03.000000 torch_ecg-0.0.8/PKG-INFO
-drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-03-28 16:42:03.000000 torch_ecg-0.0.8/test/
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    28388 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/test/test_pipelines.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     8907 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/test/test_model_configs.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     4753 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/test/test_cnn.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     1944 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/test/test_nets.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      404 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/test/test_preprocessors_t.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      844 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/test/test_loss.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      437 2021-11-14 11:44:55.000000 torch_ecg-0.0.8/test/test_augmenters.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     4659 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/test/test_downstream_tasks.py
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      420 2022-03-27 06:56:28.000000 torch_ecg-0.0.8/test/test_preprocessors.py
-drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-03-28 16:42:03.000000 torch_ecg-0.0.8/torch_ecg.egg-info/
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)       10 2022-03-28 16:42:03.000000 torch_ecg-0.0.8/torch_ecg.egg-info/top_level.txt
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     5407 2022-03-28 16:42:03.000000 torch_ecg-0.0.8/torch_ecg.egg-info/SOURCES.txt
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)        1 2022-03-28 16:42:03.000000 torch_ecg-0.0.8/torch_ecg.egg-info/dependency_links.txt
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    17482 2022-03-28 16:42:03.000000 torch_ecg-0.0.8/torch_ecg.egg-info/PKG-INFO
--rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      206 2022-03-28 16:42:03.000000 torch_ecg-0.0.8/torch_ecg.egg-info/requires.txt
+drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-03-30 15:13:52.000000 torch_ecg-0.0.9/
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    14426 2022-03-27 02:40:45.000000 torch_ecg-0.0.9/README.md
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     1316 2022-03-30 07:24:20.000000 torch_ecg-0.0.9/setup.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)       38 2022-03-30 15:13:52.000000 torch_ecg-0.0.9/setup.cfg
+drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-03-30 15:13:52.000000 torch_ecg-0.0.9/torch_ecg/
+drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-03-30 15:13:52.000000 torch_ecg-0.0.9/torch_ecg/preprocessors/
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      473 2022-03-24 09:32:39.000000 torch_ecg-0.0.9/torch_ecg/preprocessors/__init__.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     2152 2022-03-28 08:48:29.000000 torch_ecg-0.0.9/torch_ecg/preprocessors/resample.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     5697 2022-03-28 08:48:29.000000 torch_ecg-0.0.9/torch_ecg/preprocessors/normalize.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     5783 2022-03-28 08:48:29.000000 torch_ecg-0.0.9/torch_ecg/preprocessors/preproc_manager.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     2137 2022-03-28 08:48:29.000000 torch_ecg-0.0.9/torch_ecg/preprocessors/baseline_remove.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     2121 2022-03-28 08:48:29.000000 torch_ecg-0.0.9/torch_ecg/preprocessors/bandpass.py
+drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-03-30 15:13:52.000000 torch_ecg-0.0.9/torch_ecg/components/
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     9527 2022-03-30 15:10:21.000000 torch_ecg-0.0.9/torch_ecg/components/metrics.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    18063 2022-03-30 07:24:20.000000 torch_ecg-0.0.9/torch_ecg/components/loggers.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)        0 2022-03-30 07:24:20.000000 torch_ecg-0.0.9/torch_ecg/components/__init__.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    27998 2022-03-30 15:10:21.000000 torch_ecg-0.0.9/torch_ecg/components/trainer.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    12264 2022-03-30 07:24:20.000000 torch_ecg-0.0.9/torch_ecg/components/outputs.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     3303 2022-03-30 07:24:20.000000 torch_ecg-0.0.9/torch_ecg/components/nas.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      902 2022-03-30 07:24:20.000000 torch_ecg-0.0.9/torch_ecg/__init__.py
+drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-03-30 15:13:52.000000 torch_ecg-0.0.9/torch_ecg/augmenters/
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    20236 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/augmenters/stretch_compress.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     2854 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/augmenters/cutmix.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     4964 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/augmenters/random_masking.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     3497 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/augmenters/random_flip.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      636 2022-03-24 09:32:39.000000 torch_ecg-0.0.9/torch_ecg/augmenters/__init__.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    11018 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/augmenters/baseline_wander.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     3915 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/augmenters/mixup.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     6317 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/augmenters/augmenter_manager.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     2471 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/augmenters/base.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     4556 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/augmenters/random_renormalize.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     3105 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/augmenters/label_smooth.py
+drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-03-30 15:13:52.000000 torch_ecg-0.0.9/torch_ecg/databases/
+drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-03-30 15:13:52.000000 torch_ecg-0.0.9/torch_ecg/databases/aux_data/
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    28258 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/databases/aux_data/cinc2021_aux_data.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      458 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/databases/aux_data/__init__.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     6078 2022-03-27 02:26:51.000000 torch_ecg-0.0.9/torch_ecg/databases/aux_data/physionet_dbs.csv.tar.gz
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    51295 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/databases/aux_data/cinc2020_aux_data.py
+drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-03-30 15:13:52.000000 torch_ecg-0.0.9/torch_ecg/databases/physionet_databases/
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    67467 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/databases/physionet_databases/cinc2020.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    94226 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/databases/physionet_databases/cinc2021.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    13331 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/databases/physionet_databases/apnea_ecg.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    32370 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/databases/physionet_databases/ludb.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    15197 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/databases/physionet_databases/mitdb.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      708 2022-03-24 09:32:39.000000 torch_ecg-0.0.9/torch_ecg/databases/physionet_databases/__init__.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    24734 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/databases/physionet_databases/ltafdb.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     9765 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/databases/physionet_databases/cinc2017.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     3312 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/databases/physionet_databases/cinc2018.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    17779 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/databases/physionet_databases/afdb.py
+drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-03-30 15:13:52.000000 torch_ecg-0.0.9/torch_ecg/databases/nsrr_databases/
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      104 2022-03-24 09:32:39.000000 torch_ecg-0.0.9/torch_ecg/databases/nsrr_databases/__init__.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    71967 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/databases/nsrr_databases/shhs.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      870 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/databases/__init__.py
+drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-03-30 15:13:52.000000 torch_ecg-0.0.9/torch_ecg/databases/cpsc_databases/
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    22526 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/databases/cpsc_databases/cpsc2018.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    14599 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/databases/cpsc_databases/cpsc2019.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    61714 2022-03-27 08:25:33.000000 torch_ecg-0.0.9/torch_ecg/databases/cpsc_databases/cpsc2021.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      257 2022-03-24 09:32:39.000000 torch_ecg-0.0.9/torch_ecg/databases/cpsc_databases/__init__.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    32777 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/databases/cpsc_databases/cpsc2020.py
+drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-03-30 15:13:52.000000 torch_ecg-0.0.9/torch_ecg/databases/datasets/
+drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-03-30 15:13:52.000000 torch_ecg-0.0.9/torch_ecg/databases/datasets/ludb/
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      137 2022-03-24 09:32:39.000000 torch_ecg-0.0.9/torch_ecg/databases/datasets/ludb/__init__.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     3696 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/databases/datasets/ludb/ludb_cfg.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     8108 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/databases/datasets/ludb/ludb_dataset.py
+drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-03-30 15:13:52.000000 torch_ecg-0.0.9/torch_ecg/databases/datasets/cinc2020/
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     6372 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/databases/datasets/cinc2020/cinc2020_cfg.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      161 2022-03-24 09:32:39.000000 torch_ecg-0.0.9/torch_ecg/databases/datasets/cinc2020/__init__.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    15424 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/databases/datasets/cinc2020/cinc2020_dataset.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      920 2022-03-30 07:24:20.000000 torch_ecg-0.0.9/torch_ecg/databases/datasets/__init__.py
+drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-03-30 15:13:52.000000 torch_ecg-0.0.9/torch_ecg/databases/datasets/cpsc2021/
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    61592 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/databases/datasets/cpsc2021/cpsc2021_dataset.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      161 2022-03-24 09:32:39.000000 torch_ecg-0.0.9/torch_ecg/databases/datasets/cpsc2021/__init__.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     8585 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/databases/datasets/cpsc2021/cpsc2021_cfg.py
+drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-03-30 15:13:52.000000 torch_ecg-0.0.9/torch_ecg/databases/datasets/cpsc2020/
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)        0 2022-03-24 09:32:39.000000 torch_ecg-0.0.9/torch_ecg/databases/datasets/cpsc2020/cpsc2020_dataset.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)        0 2022-03-24 09:32:39.000000 torch_ecg-0.0.9/torch_ecg/databases/datasets/cpsc2020/cpsc2020_cfg.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)        0 2022-03-24 09:32:39.000000 torch_ecg-0.0.9/torch_ecg/databases/datasets/cpsc2020/__init__.py
+drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-03-30 15:13:52.000000 torch_ecg-0.0.9/torch_ecg/databases/datasets/cpsc2019/
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     4307 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/databases/datasets/cpsc2019/cpsc2019_cfg.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      161 2022-03-24 09:32:39.000000 torch_ecg-0.0.9/torch_ecg/databases/datasets/cpsc2019/__init__.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     6738 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/databases/datasets/cpsc2019/cpsc2019_dataset.py
+drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-03-30 15:13:52.000000 torch_ecg-0.0.9/torch_ecg/databases/datasets/cinc2021/
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      161 2022-03-24 09:32:39.000000 torch_ecg-0.0.9/torch_ecg/databases/datasets/cinc2021/__init__.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     6568 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/databases/datasets/cinc2021/cinc2021_cfg.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    19921 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/databases/datasets/cinc2021/cinc2021_dataset.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    24594 2022-03-28 08:48:29.000000 torch_ecg-0.0.9/torch_ecg/databases/base.py
+drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-03-30 15:13:52.000000 torch_ecg-0.0.9/torch_ecg/models/
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    17383 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/models/loss.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)   149046 2022-03-28 14:17:53.000000 torch_ecg-0.0.9/torch_ecg/models/_nets.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      254 2022-03-24 09:32:39.000000 torch_ecg-0.0.9/torch_ecg/models/__init__.py
+drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-03-30 15:13:52.000000 torch_ecg-0.0.9/torch_ecg/models/unets/
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      223 2022-03-24 09:32:39.000000 torch_ecg-0.0.9/torch_ecg/models/unets/__init__.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    21625 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/models/unets/ecg_unet.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    25438 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/models/unets/ecg_subtract_unet.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     9058 2022-03-30 07:24:20.000000 torch_ecg-0.0.9/torch_ecg/models/rr_lstm.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    13937 2022-03-30 07:24:20.000000 torch_ecg-0.0.9/torch_ecg/models/ecg_seq_lab_net.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    16523 2022-03-30 07:24:20.000000 torch_ecg-0.0.9/torch_ecg/models/ecg_crnn.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      489 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/models/ecg_fcn.py
+drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-03-30 15:13:52.000000 torch_ecg-0.0.9/torch_ecg/models/transformers/
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)       81 2022-03-24 09:32:39.000000 torch_ecg-0.0.9/torch_ecg/models/transformers/__init__.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     3407 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/models/transformers/transformer.py
+drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-03-30 15:13:52.000000 torch_ecg-0.0.9/torch_ecg/models/cnn/
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    29119 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/models/cnn/densenet.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     1377 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/models/cnn/ho_resnet.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    34355 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/models/cnn/resnet.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      224 2022-03-24 09:32:39.000000 torch_ecg-0.0.9/torch_ecg/models/cnn/__init__.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    29950 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/models/cnn/mobilenet.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     1721 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/models/cnn/darknet.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     2697 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/models/cnn/efficientnet.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    33937 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/models/cnn/xception.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     8142 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/models/cnn/vgg.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    15375 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/models/cnn/multi_scopic.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     5226 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/models/grad_cam.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     3008 2022-03-30 07:24:20.000000 torch_ecg-0.0.9/torch_ecg/cfg.py
+drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-03-30 15:13:52.000000 torch_ecg-0.0.9/torch_ecg/_preprocessors/
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      690 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/_preprocessors/__init__.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     8790 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/_preprocessors/base.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     2251 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/_preprocessors/resample.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     7082 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/_preprocessors/normalize.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     5903 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/_preprocessors/preproc_manager.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     2228 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/_preprocessors/baseline_remove.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     2649 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/_preprocessors/bandpass.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)       22 2022-03-30 15:10:21.000000 torch_ecg-0.0.9/torch_ecg/version.py
+drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-03-30 15:13:52.000000 torch_ecg-0.0.9/torch_ecg/model_configs/
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     4614 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/model_configs/__init__.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      500 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/model_configs/mlp.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      560 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/model_configs/rnn.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     2326 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/model_configs/rr_lstm.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     2681 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/model_configs/ecg_seq_lab_net.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     2781 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/model_configs/ecg_unet.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     9325 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/model_configs/ecg_crnn.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     2545 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/model_configs/ati_cnn.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     1156 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/model_configs/ecg_yolo.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      989 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/model_configs/attn.py
+drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-03-30 15:13:52.000000 torch_ecg-0.0.9/torch_ecg/model_configs/cnn/
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      956 2022-03-24 09:32:39.000000 torch_ecg-0.0.9/torch_ecg/model_configs/cnn/densenet.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    16643 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/model_configs/cnn/resnet.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     3867 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/model_configs/cnn/__init__.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     4213 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/model_configs/cnn/mobilenet.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     1961 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/model_configs/cnn/xception.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     1776 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/model_configs/cnn/cpsc.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     1679 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/model_configs/cnn/vgg.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     3080 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/model_configs/cnn/multi_scopic.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     3858 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/torch_ecg/model_configs/ecg_subtract_unet.py
+drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-03-30 15:13:52.000000 torch_ecg-0.0.9/torch_ecg/utils/
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    31144 2022-03-28 08:48:29.000000 torch_ecg-0.0.9/torch_ecg/utils/utils_signal.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     6540 2022-03-28 08:48:29.000000 torch_ecg-0.0.9/torch_ecg/utils/rpeaks.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     8285 2022-03-28 08:48:29.000000 torch_ecg-0.0.9/torch_ecg/utils/utils_signal_t.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     4634 2022-03-28 16:40:36.000000 torch_ecg-0.0.9/torch_ecg/utils/download.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)        0 2022-03-24 09:32:39.000000 torch_ecg-0.0.9/torch_ecg/utils/__init__.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    21173 2022-03-30 15:10:21.000000 torch_ecg-0.0.9/torch_ecg/utils/utils_metrics.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    12504 2022-03-28 08:48:29.000000 torch_ecg-0.0.9/torch_ecg/utils/preproc.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     3695 2022-03-28 08:48:29.000000 torch_ecg-0.0.9/torch_ecg/utils/edr.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    27056 2022-03-28 08:48:29.000000 torch_ecg-0.0.9/torch_ecg/utils/ecg_arrhythmia_knowledge.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    31532 2022-03-28 08:48:29.000000 torch_ecg-0.0.9/torch_ecg/utils/utils_interval.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    47552 2022-03-30 15:10:21.000000 torch_ecg-0.0.9/torch_ecg/utils/misc.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    19403 2022-03-28 08:48:29.000000 torch_ecg-0.0.9/torch_ecg/utils/pantompkins.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    28784 2022-03-28 08:48:29.000000 torch_ecg-0.0.9/torch_ecg/utils/utils_nn.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    17482 2022-03-30 15:13:52.000000 torch_ecg-0.0.9/PKG-INFO
+drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-03-30 15:13:52.000000 torch_ecg-0.0.9/test/
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    28388 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/test/test_pipelines.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     8907 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/test/test_model_configs.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     4753 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/test/test_cnn.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     1944 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/test/test_nets.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      404 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/test/test_preprocessors_t.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      844 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/test/test_loss.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      437 2021-11-14 11:44:55.000000 torch_ecg-0.0.9/test/test_augmenters.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     4659 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/test/test_downstream_tasks.py
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      420 2022-03-27 06:56:28.000000 torch_ecg-0.0.9/test/test_preprocessors.py
+drwxrwxr-x   0 wenhao    (1002) wenhao    (1003)        0 2022-03-30 15:13:52.000000 torch_ecg-0.0.9/torch_ecg.egg-info/
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)       10 2022-03-30 15:13:51.000000 torch_ecg-0.0.9/torch_ecg.egg-info/top_level.txt
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)     5492 2022-03-30 15:13:51.000000 torch_ecg-0.0.9/torch_ecg.egg-info/SOURCES.txt
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)        1 2022-03-30 15:13:51.000000 torch_ecg-0.0.9/torch_ecg.egg-info/dependency_links.txt
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)    17482 2022-03-30 15:13:51.000000 torch_ecg-0.0.9/torch_ecg.egg-info/PKG-INFO
+-rw-rw-r--   0 wenhao    (1002) wenhao    (1003)      206 2022-03-30 15:13:51.000000 torch_ecg-0.0.9/torch_ecg.egg-info/requires.txt
```

### Comparing `torch_ecg-0.0.8/README.md` & `torch_ecg-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/setup.py` & `torch_ecg-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,17 +28,15 @@
             "references*",
             "docs*",
             "benchmarks*",
             "tests*",
             "sample*",
         ]
     ),
-    package_data={
-        "torch_ecg.databases.aux_data": ["*.tar.gz"]
-    },
+    package_data={"torch_ecg.databases.aux_data": ["*.tar.gz"]},
     # entry_points=,
     classifiers=[
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
```

### Comparing `torch_ecg-0.0.8/torch_ecg/preprocessors/resample.py` & `torch_ecg-0.0.9/torch_ecg/preprocessors/resample.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/preprocessors/normalize.py` & `torch_ecg-0.0.9/torch_ecg/preprocessors/normalize.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/preprocessors/preproc_manager.py` & `torch_ecg-0.0.9/torch_ecg/preprocessors/preproc_manager.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/preprocessors/baseline_remove.py` & `torch_ecg-0.0.9/torch_ecg/preprocessors/baseline_remove.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/preprocessors/bandpass.py` & `torch_ecg-0.0.9/torch_ecg/preprocessors/bandpass.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/__init__.py` & `torch_ecg-0.0.9/torch_ecg/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -17,20 +17,22 @@
 from . import utils
 from . import _preprocessors
 from . import preprocessors
 from . import augmenters
 from . import databases
 from . import models
 from . import model_configs
+from . import components
 from .version import __version__
 
 
 __all__ = [
     "utils",
     "_preprocessors",
     "preprocessors",
     "augmenters",
     "databases",
+    "components",
     "models",
     "model_configs",
     "__version__",
 ]
```

### Comparing `torch_ecg-0.0.8/torch_ecg/augmenters/stretch_compress.py` & `torch_ecg-0.0.9/torch_ecg/augmenters/stretch_compress.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/augmenters/cutmix.py` & `torch_ecg-0.0.9/torch_ecg/augmenters/cutmix.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/augmenters/random_masking.py` & `torch_ecg-0.0.9/torch_ecg/augmenters/random_masking.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/augmenters/random_flip.py` & `torch_ecg-0.0.9/torch_ecg/augmenters/random_flip.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/augmenters/__init__.py` & `torch_ecg-0.0.9/torch_ecg/augmenters/__init__.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/augmenters/baseline_wander.py` & `torch_ecg-0.0.9/torch_ecg/augmenters/baseline_wander.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/augmenters/mixup.py` & `torch_ecg-0.0.9/torch_ecg/augmenters/mixup.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/augmenters/augmenter_manager.py` & `torch_ecg-0.0.9/torch_ecg/augmenters/augmenter_manager.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/augmenters/base.py` & `torch_ecg-0.0.9/torch_ecg/augmenters/base.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/augmenters/random_renormalize.py` & `torch_ecg-0.0.9/torch_ecg/augmenters/random_renormalize.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/augmenters/label_smooth.py` & `torch_ecg-0.0.9/torch_ecg/augmenters/label_smooth.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/databases/aux_data/cinc2021_aux_data.py` & `torch_ecg-0.0.9/torch_ecg/databases/aux_data/cinc2021_aux_data.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/databases/aux_data/physionet_dbs.csv.tar.gz` & `torch_ecg-0.0.9/torch_ecg/databases/aux_data/physionet_dbs.csv.tar.gz`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/databases/aux_data/cinc2020_aux_data.py` & `torch_ecg-0.0.9/torch_ecg/databases/aux_data/cinc2020_aux_data.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/databases/physionet_databases/cinc2020.py` & `torch_ecg-0.0.9/torch_ecg/databases/physionet_databases/cinc2020.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/databases/physionet_databases/cinc2021.py` & `torch_ecg-0.0.9/torch_ecg/databases/physionet_databases/cinc2021.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/databases/physionet_databases/apnea_ecg.py` & `torch_ecg-0.0.9/torch_ecg/databases/physionet_databases/apnea_ecg.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/databases/physionet_databases/ludb.py` & `torch_ecg-0.0.9/torch_ecg/databases/physionet_databases/ludb.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/databases/physionet_databases/mitdb.py` & `torch_ecg-0.0.9/torch_ecg/databases/physionet_databases/mitdb.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/databases/physionet_databases/__init__.py` & `torch_ecg-0.0.9/torch_ecg/databases/physionet_databases/__init__.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/databases/physionet_databases/ltafdb.py` & `torch_ecg-0.0.9/torch_ecg/databases/physionet_databases/ltafdb.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/databases/physionet_databases/cinc2017.py` & `torch_ecg-0.0.9/torch_ecg/databases/physionet_databases/cinc2017.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/databases/physionet_databases/cinc2018.py` & `torch_ecg-0.0.9/torch_ecg/databases/physionet_databases/cinc2018.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/databases/physionet_databases/afdb.py` & `torch_ecg-0.0.9/torch_ecg/databases/physionet_databases/afdb.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/databases/nsrr_databases/shhs.py` & `torch_ecg-0.0.9/torch_ecg/databases/nsrr_databases/shhs.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/databases/__init__.py` & `torch_ecg-0.0.9/torch_ecg/databases/__init__.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/databases/cpsc_databases/cpsc2018.py` & `torch_ecg-0.0.9/torch_ecg/databases/cpsc_databases/cpsc2018.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/databases/cpsc_databases/cpsc2019.py` & `torch_ecg-0.0.9/torch_ecg/databases/cpsc_databases/cpsc2019.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/databases/cpsc_databases/cpsc2021.py` & `torch_ecg-0.0.9/torch_ecg/databases/cpsc_databases/cpsc2021.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/databases/cpsc_databases/cpsc2020.py` & `torch_ecg-0.0.9/torch_ecg/databases/cpsc_databases/cpsc2020.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/databases/datasets/ludb/ludb_cfg.py` & `torch_ecg-0.0.9/torch_ecg/databases/datasets/ludb/ludb_cfg.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/databases/datasets/ludb/ludb_dataset.py` & `torch_ecg-0.0.9/torch_ecg/databases/datasets/ludb/ludb_dataset.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/databases/datasets/cinc2020/cinc2020_cfg.py` & `torch_ecg-0.0.9/torch_ecg/databases/datasets/cinc2020/cinc2020_cfg.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/databases/datasets/cinc2020/cinc2020_dataset.py` & `torch_ecg-0.0.9/torch_ecg/databases/datasets/cinc2020/cinc2020_dataset.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/databases/datasets/cpsc2021/cpsc2021_dataset.py` & `torch_ecg-0.0.9/torch_ecg/databases/datasets/cpsc2021/cpsc2021_dataset.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/databases/datasets/cpsc2021/cpsc2021_cfg.py` & `torch_ecg-0.0.9/torch_ecg/databases/datasets/cpsc2021/cpsc2021_cfg.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/databases/datasets/cpsc2019/cpsc2019_cfg.py` & `torch_ecg-0.0.9/torch_ecg/databases/datasets/cpsc2019/cpsc2019_cfg.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/databases/datasets/cpsc2019/cpsc2019_dataset.py` & `torch_ecg-0.0.9/torch_ecg/databases/datasets/cpsc2019/cpsc2019_dataset.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/databases/datasets/cinc2021/cinc2021_cfg.py` & `torch_ecg-0.0.9/torch_ecg/databases/datasets/cinc2021/cinc2021_cfg.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/databases/datasets/cinc2021/cinc2021_dataset.py` & `torch_ecg-0.0.9/torch_ecg/databases/datasets/cinc2021/cinc2021_dataset.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/databases/base.py` & `torch_ecg-0.0.9/torch_ecg/databases/base.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/models/loss.py` & `torch_ecg-0.0.9/torch_ecg/models/loss.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/models/_nets.py` & `torch_ecg-0.0.9/torch_ecg/models/_nets.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/models/unets/ecg_unet.py` & `torch_ecg-0.0.9/torch_ecg/models/unets/ecg_unet.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/models/unets/ecg_subtract_unet.py` & `torch_ecg-0.0.9/torch_ecg/models/unets/ecg_subtract_unet.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/models/rr_lstm.py` & `torch_ecg-0.0.9/torch_ecg/models/rr_lstm.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from torch import Tensor
 import torch.nn.functional as F
 
 from ..cfg import CFG, DEFAULTS
 from ..model_configs.rr_lstm import RR_LSTM_CONFIG
 from ..utils.misc import dict_to_str
 from ..utils.utils_nn import compute_module_size, SizeMixin, CkptMixin
-from ..utils.outputs import BaseOutput
+from ..components.outputs import BaseOutput
 from ..models._nets import (
     Mish,
     Swish,
     Activations,
     NonLocalBlock,
     SEBlock,
     GlobalContextBlock,
```

### Comparing `torch_ecg-0.0.8/torch_ecg/models/ecg_seq_lab_net.py` & `torch_ecg-0.0.9/torch_ecg/models/ecg_seq_lab_net.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 from ..utils.utils_nn import (
     compute_conv_output_shape,
     compute_module_size,
     SizeMixin,
     CkptMixin,
 )
 from ..utils.misc import dict_to_str
-from ..utils.outputs import SequenceLabelingOutput
+from ..components.outputs import SequenceLabelingOutput
 from ..model_configs.ecg_seq_lab_net import ECG_SEQ_LAB_NET_CONFIG
 from ._nets import (
     Mish,
     Swish,
     Activations,
     Bn_Activation,
     Conv_Bn_Activation,
```

### Comparing `torch_ecg-0.0.8/torch_ecg/models/ecg_crnn.py` & `torch_ecg-0.0.9/torch_ecg/models/ecg_crnn.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from ..utils.utils_nn import (
     compute_conv_output_shape,
     compute_module_size,
     SizeMixin,
     CkptMixin,
 )
 from ..utils.misc import dict_to_str
-from ..utils.outputs import BaseOutput
+from ..components.outputs import BaseOutput
 from ._nets import (
     Mish,
     Swish,
     Activations,
     Bn_Activation,
     Conv_Bn_Activation,
     DownSample,
```

### Comparing `torch_ecg-0.0.8/torch_ecg/models/transformers/transformer.py` & `torch_ecg-0.0.9/torch_ecg/models/transformers/transformer.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/models/cnn/densenet.py` & `torch_ecg-0.0.9/torch_ecg/models/cnn/densenet.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/models/cnn/ho_resnet.py` & `torch_ecg-0.0.9/torch_ecg/models/cnn/ho_resnet.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/models/cnn/resnet.py` & `torch_ecg-0.0.9/torch_ecg/models/cnn/resnet.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/models/cnn/mobilenet.py` & `torch_ecg-0.0.9/torch_ecg/models/cnn/mobilenet.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/models/cnn/darknet.py` & `torch_ecg-0.0.9/torch_ecg/models/cnn/darknet.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/models/cnn/efficientnet.py` & `torch_ecg-0.0.9/torch_ecg/models/cnn/efficientnet.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/models/cnn/xception.py` & `torch_ecg-0.0.9/torch_ecg/models/cnn/xception.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/models/cnn/vgg.py` & `torch_ecg-0.0.9/torch_ecg/models/cnn/vgg.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/models/cnn/multi_scopic.py` & `torch_ecg-0.0.9/torch_ecg/models/cnn/multi_scopic.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/models/grad_cam.py` & `torch_ecg-0.0.9/torch_ecg/models/grad_cam.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/cfg.py` & `torch_ecg-0.0.9/torch_ecg/cfg.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,15 +21,16 @@
 
 
 class CFG(ED):
     """
     this class is created in order to renew the `update` method,
     to fit the hierarchical structure of configurations
 
-    for example:
+    Examples
+    --------
     >>> c = CFG(hehe={"a":1,"b":2})
     >>> c.update(hehe={"a":-1})
     >>> c
     {'hehe': {'a': -1, 'b': 2}}
     >>> c.__update__(hehe={"a":-10})
     >>> c
     {'hehe': {'a': -10}}
@@ -51,18 +52,19 @@
             d.update(**kwargs)
         for k, v in d.items():
             try:
                 setattr(self, k, v)
             except:
                 dict.__setitem__(self, k, v)
         # Class attributes
+        exclude_fields = ["update", "pop"]
         for k in self.__class__.__dict__:
-            if not (k.startswith("__") and k.endswith("__")) and not k in (
-                "update",
-                "pop",
+            if (
+                not (k.startswith("__") and k.endswith("__"))
+                and not k in exclude_fields
             ):
                 setattr(self, k, getattr(self, k))
 
     def __update__(
         self, new_cfg: Optional[MutableMapping] = None, **kwargs
     ) -> NoReturn:
         """
```

### Comparing `torch_ecg-0.0.8/torch_ecg/_preprocessors/__init__.py` & `torch_ecg-0.0.9/torch_ecg/_preprocessors/__init__.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/_preprocessors/base.py` & `torch_ecg-0.0.9/torch_ecg/_preprocessors/base.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/_preprocessors/resample.py` & `torch_ecg-0.0.9/torch_ecg/_preprocessors/resample.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/_preprocessors/normalize.py` & `torch_ecg-0.0.9/torch_ecg/_preprocessors/normalize.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/_preprocessors/preproc_manager.py` & `torch_ecg-0.0.9/torch_ecg/_preprocessors/preproc_manager.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/_preprocessors/baseline_remove.py` & `torch_ecg-0.0.9/torch_ecg/_preprocessors/baseline_remove.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/_preprocessors/bandpass.py` & `torch_ecg-0.0.9/torch_ecg/_preprocessors/bandpass.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/model_configs/__init__.py` & `torch_ecg-0.0.9/torch_ecg/model_configs/__init__.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/model_configs/rnn.py` & `torch_ecg-0.0.9/torch_ecg/model_configs/rnn.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/model_configs/rr_lstm.py` & `torch_ecg-0.0.9/torch_ecg/model_configs/rr_lstm.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/model_configs/ecg_seq_lab_net.py` & `torch_ecg-0.0.9/torch_ecg/model_configs/ecg_seq_lab_net.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/model_configs/ecg_unet.py` & `torch_ecg-0.0.9/torch_ecg/model_configs/ecg_unet.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/model_configs/ecg_crnn.py` & `torch_ecg-0.0.9/torch_ecg/model_configs/ecg_crnn.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/model_configs/ati_cnn.py` & `torch_ecg-0.0.9/torch_ecg/model_configs/ati_cnn.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/model_configs/ecg_yolo.py` & `torch_ecg-0.0.9/torch_ecg/model_configs/ecg_yolo.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/model_configs/attn.py` & `torch_ecg-0.0.9/torch_ecg/model_configs/attn.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/model_configs/cnn/densenet.py` & `torch_ecg-0.0.9/torch_ecg/model_configs/cnn/densenet.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/model_configs/cnn/resnet.py` & `torch_ecg-0.0.9/torch_ecg/model_configs/cnn/resnet.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/model_configs/cnn/__init__.py` & `torch_ecg-0.0.9/torch_ecg/model_configs/cnn/__init__.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/model_configs/cnn/mobilenet.py` & `torch_ecg-0.0.9/torch_ecg/model_configs/cnn/mobilenet.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/model_configs/cnn/xception.py` & `torch_ecg-0.0.9/torch_ecg/model_configs/cnn/xception.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/model_configs/cnn/cpsc.py` & `torch_ecg-0.0.9/torch_ecg/model_configs/cnn/cpsc.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/model_configs/cnn/vgg.py` & `torch_ecg-0.0.9/torch_ecg/model_configs/cnn/vgg.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/model_configs/cnn/multi_scopic.py` & `torch_ecg-0.0.9/torch_ecg/model_configs/cnn/multi_scopic.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/model_configs/ecg_subtract_unet.py` & `torch_ecg-0.0.9/torch_ecg/model_configs/ecg_subtract_unet.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/utils/utils_signal.py` & `torch_ecg-0.0.9/torch_ecg/utils/utils_signal.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/utils/rpeaks.py` & `torch_ecg-0.0.9/torch_ecg/utils/rpeaks.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/utils/utils_signal_t.py` & `torch_ecg-0.0.9/torch_ecg/utils/utils_signal_t.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/utils/download.py` & `torch_ecg-0.0.9/torch_ecg/utils/download.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/utils/loggers.py` & `torch_ecg-0.0.9/torch_ecg/components/loggers.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/utils/preproc.py` & `torch_ecg-0.0.9/torch_ecg/utils/preproc.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/utils/edr.py` & `torch_ecg-0.0.9/torch_ecg/utils/edr.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/utils/trainer.py` & `torch_ecg-0.0.9/torch_ecg/components/trainer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Abstract base class for trainers,
 in order to replace the functions for classes in the training pipelines
 
 """
 
-import textwrap
+import textwrap, logging
 from pathlib import Path
 from copy import deepcopy
 from abc import ABC, abstractmethod
 from collections import deque, OrderedDict
 from typing import NoReturn, Optional, Union, Tuple, Dict, List
 
 import numpy as np
@@ -21,24 +21,24 @@
 from torch import nn
 from torch import optim
 from torch.nn.parallel import DistributedDataParallel as DDP, DataParallel as DP
 from torch.utils.data.dataset import Dataset
 from torch.utils.data import DataLoader
 import torch_optimizer as extra_optim
 
-from .utils_nn import default_collate_fn as collate_fn
-from .misc import (
+from .loggers import LoggerManager
+from ..utils.utils_nn import default_collate_fn as collate_fn
+from ..utils.misc import (
     dicts_equal,
     init_logger,
     get_date_str,
     dict_to_str,
     str2bool,
     ReprMixin,
 )
-from .loggers import LoggerManager
 from ..augmenters import AugmenterManager
 from ..models.loss import (
     BCEWithLogitsWithClassWeightLoss,
     MaskedBCEWithLogitsLoss,
     FocalLoss,
     AsymmetricLoss,
 )
@@ -198,48 +198,63 @@
                 self.log_manager.log_metrics(
                     metrics=eval_res,
                     step=self.global_step,
                     epoch=self.epoch,
                     part="val",
                 )
 
-                # update best model and best metric
-                if eval_res[self.train_config.monitor] > self.best_metric:
-                    self.best_metric = eval_res[self.train_config.monitor]
-                    self.best_state_dict = self._model.state_dict()
-                    self.best_eval_res = deepcopy(eval_res)
-                    self.best_epoch = self.epoch
-                    self.pseudo_best_epoch = self.epoch
-                elif self.train_config.early_stopping:
-                    if (
-                        eval_res[self.train_config.monitor]
-                        >= self.best_metric - self.train_config.early_stopping.min_delta
-                    ):
+                # update best model and best metric if monitor is set
+                if self.train_config.monitor is not None:
+                    if eval_res[self.train_config.monitor] > self.best_metric:
+                        self.best_metric = eval_res[self.train_config.monitor]
+                        self.best_state_dict = self._model.state_dict()
+                        self.best_eval_res = deepcopy(eval_res)
+                        self.best_epoch = self.epoch
                         self.pseudo_best_epoch = self.epoch
-                    elif (
-                        self.epoch - self.pseudo_best_epoch
-                        >= self.train_config.early_stopping.patience
-                    ):
-                        msg = f"early stopping is triggered at epoch {self.epoch}"
-                        self.log_manager.log_message(msg)
-                        break
-
-                msg = textwrap.dedent(
-                    f"""
-                    best metric = {self.best_metric},
-                    obtained at epoch {self.best_epoch}
-                """
-                )
-                self.log_manager.log_message(msg)
+                    elif self.train_config.early_stopping:
+                        if (
+                            eval_res[self.train_config.monitor]
+                            >= self.best_metric
+                            - self.train_config.early_stopping.min_delta
+                        ):
+                            self.pseudo_best_epoch = self.epoch
+                        elif (
+                            self.epoch - self.pseudo_best_epoch
+                            >= self.train_config.early_stopping.patience
+                        ):
+                            msg = f"early stopping is triggered at epoch {self.epoch}"
+                            self.log_manager.log_message(msg)
+                            break
+
+                    msg = textwrap.dedent(
+                        f"""
+                        best metric = {self.best_metric},
+                        obtained at epoch {self.best_epoch}
+                    """
+                    )
+                    self.log_manager.log_message(msg)
 
-                # save checkpoint
-                save_suffix = f"epochloss_{self.epoch_loss:.5f}_metric_{eval_res[self.train_config.monitor]:.2f}"
+                    # save checkpoint
+                    save_suffix = f"epochloss_{self.epoch_loss:.5f}_metric_{eval_res[self.train_config.monitor]:.2f}"
+                else:
+                    save_suffix = f"epochloss_{self.epoch_loss:.5f}"
                 save_filename = f"{self.save_prefix}{self.epoch}_{get_date_str()}_{save_suffix}.pth.tar"
                 save_path = self.train_config.checkpoints / save_filename
-                self.save_checkpoint(str(save_path))
+                if self.train_config.keep_checkpoint_max != 0:
+                    self.save_checkpoint(str(save_path))
+                    self.saved_models.append(save_path)
+                # remove outdated models
+                if len(self.saved_models) > self.train_config.keep_checkpoint_max > 0:
+                    model_to_remove = self.saved_models.popleft()
+                    try:
+                        os.remove(model_to_remove)
+                    except:
+                        self.log_manager.log_message(
+                            f"failed to remove {str(model_to_remove)}"
+                        )
 
                 # update learning rate using lr_scheduler
                 if self.train_config.lr_scheduler.lower() == "plateau":
                     self._update_lr(eval_res)
 
                 self.log_manager.epoch_end(self.epoch)
 
@@ -253,19 +268,29 @@
                 save_suffix = (
                     f"metric_{self.best_eval_res[self.train_config.monitor]:.2f}"
                 )
                 save_filename = f"BestModel_{self.save_prefix}{self.best_epoch}_{get_date_str()}_{save_suffix}.pth.tar"
             save_path = self.train_config.model_dir / save_filename
             self.save_checkpoint(path=str(save_path))
             self.log_manager.log_message(f"best model is saved at {save_path}")
+        elif self.train_config.monitor is None:
+            self.log_manager.log_message(
+                "no monitor is set, no model is selected and saved as the best model"
+            )
+            self.best_state_dict = self._model.state_dict()
         else:
             raise ValueError("No best model found!")
 
         self.log_manager.close()
 
+        if not self.best_state_dict:
+            # in case no best model is found,
+            # e.g. monitor is not set, or keep_checkpoint_max is 0
+            self.best_state_dict = self._model.state_dict()
+
         return self.best_state_dict
 
     def train_one_epoch(self, pbar: tqdm) -> NoReturn:
         """finished, checked,
 
         train one epoch, and update the progress bar
 
@@ -340,15 +365,15 @@
         raise NotImplementedError
 
     @property
     def required_train_config_fields(self) -> List[str]:
         """ """
         return [
             "classes",
-            "monitor",
+            # "monitor",  # can be None
             "n_epochs",
             "batch_size",
             "log_step",
             "optimizer",
             "lr_scheduler",
             "learning_rate",
         ] + self.extra_required_train_config_fields
@@ -448,48 +473,83 @@
         train_config: dict,
             training configuration
 
         """
         _default_config = CFG(deepcopy(self.__DEFATULT_CONFIGS__))
         _default_config.update(train_config)
         self._train_config = CFG(deepcopy(_default_config))
-        if not self.train_config.get("model_dir", None):
-            self._train_config.model_dir = self.train_config.checkpoints
-        self._train_config.model_dir = Path(self._train_config.model_dir)
+
+        # check validity of the config
         self._validate_train_config()
 
+        # set aliases
         self.n_epochs = self.train_config.n_epochs
         self.batch_size = self.train_config.batch_size
         self.lr = self.train_config.learning_rate
 
-        if not self.lazy:
-            self._setup_dataloaders()
-
+        # setup log manager first
         self._setup_log_manager()
-
         msg = (
             f"training configurations are as follows:\n{dict_to_str(self.train_config)}"
         )
         self.log_manager.log_message(msg)
 
-        self._setup_augmenter_manager()
+        # setup directories
+        self._setup_directories()
 
-        self.train_config.checkpoints.mkdir(parents=True, exist_ok=True)
-        self.train_config.model_dir.mkdir(parents=True, exist_ok=True)
+        # setup callbacks
+        self._setup_callbacks()
+
+        # setup data loaders
+        if not self.lazy:
+            self._setup_dataloaders()
+
+        # setup augmenters manager
+        self._setup_augmenter_manager()
 
     def extra_log_suffix(self) -> str:
         """ """
         return f"{self._model.__name__}_{self.train_config.optimizer}_LR_{self.lr}_BS_{self.batch_size}"
 
     def _setup_log_manager(self) -> NoReturn:
         """finished, checked,"""
         config = {"log_suffix": self.extra_log_suffix()}
         config.update(self.train_config)
         self.log_manager = LoggerManager.from_config(config=config)
 
+    def _setup_directories(self) -> NoReturn:
+        """finished, checked,"""
+        if not self.train_config.get("model_dir", None):
+            self._train_config.model_dir = self.train_config.checkpoints
+        self._train_config.model_dir = Path(self._train_config.model_dir)
+        self.train_config.checkpoints.mkdir(parents=True, exist_ok=True)
+        self.train_config.model_dir.mkdir(parents=True, exist_ok=True)
+
+    def _setup_callbacks(self) -> NoReturn:
+        """finished, checked,"""
+        self._train_config.monitor = self.train_config.get("monitor", None)
+        if self.train_config.monitor is None:
+            assert (
+                self.train_config.lr_scheduler.lower() != "plateau"
+            ), "monitor is not specified, lr_scheduler should not be ReduceLROnPlateau"
+        self._train_config.keep_checkpoint_max = self.train_config.get(
+            "keep_checkpoint_max", 1
+        )
+        if self._train_config.keep_checkpoint_max < 0:
+            self._train_config.keep_checkpoint_max = -1
+            self.log_manager.log_message(
+                msg="keep_checkpoint_max is set to -1, all checkpoints will be kept",
+                level=logging.WARNING,
+            )
+        elif self._train_config.keep_checkpoint_max == 0:
+            self.log_manager.log_message(
+                msg="keep_checkpoint_max is set to 0, no checkpoint will be kept",
+                level=logging.WARNING,
+            )
+
     def _setup_augmenter_manager(self) -> NoReturn:
         """finished, checked,"""
         self.augmenter_manager = AugmenterManager.from_config(config=self.train_config)
 
     @abstractmethod
     def _setup_dataloaders(
         self,
```

### Comparing `torch_ecg-0.0.8/torch_ecg/utils/ecg_arrhythmia_knowledge.py` & `torch_ecg-0.0.9/torch_ecg/utils/ecg_arrhythmia_knowledge.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/utils/utils_interval.py` & `torch_ecg-0.0.9/torch_ecg/utils/utils_interval.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/utils/nas.py` & `torch_ecg-0.0.9/torch_ecg/components/nas.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/utils/misc.py` & `torch_ecg-0.0.9/torch_ecg/utils/misc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """
 """
 import os, sys, re, logging, datetime, random
 from pathlib import Path
-from functools import reduce
+from functools import reduce, wraps
 from collections import namedtuple
 from glob import glob
 from copy import deepcopy
 from typing import (
     Union,
     Optional,
     NoReturn,
     Any,
     List,
     Dict,
     Tuple,
     Sequence,
     Iterable,
+    Callable,
 )
 from numbers import Real, Number
 
 import numpy as np
 import pandas as pd
 from scipy import interpolate
 from sklearn.utils import compute_class_weight
@@ -56,14 +57,15 @@
     "default_class_repr",
     "ReprMixin",
     "MovingAverage",
     "uniform",
     "nildent",
     "isclass",
     "strafified_train_test_split",
+    "add_docstring",
 ]
 
 
 def get_record_list_recursive(db_dir: Union[str, Path], rec_ext: str) -> List[str]:
     """finished, checked,
 
     get the list of records in `db_dir` recursively,
@@ -1507,7 +1509,54 @@
     test_indices = []
     for n in item_names:
         item_test_indices = item_indices[n][: round(test_ratio * len(item_indices[n]))]
         test_indices += item_test_indices
     df_test = df.loc[df.index.isin(test_indices)].reset_index(drop=True)
     df_train = df.loc[~df.index.isin(test_indices)].reset_index(drop=True)
     return df_train, df_test
+
+
+def add_docstring(doc: str, mode: str = "replace") -> Callable:
+    """
+    decorator to add docstring to a function
+
+    Parameters
+    ----------
+    doc: str,
+        the docstring to be added
+    mode: str, default "replace",
+        the mode of the docstring,
+        can be "replace", "append" or "prepend",
+        case insensitive
+
+    """
+
+    def decorator(func: Callable) -> Callable:
+        """ """
+
+        @wraps(func)
+        def wrapper(*args, **kwargs) -> Callable:
+            """ """
+            return func(*args, **kwargs)
+
+        pattern = "(\s^\n){1,}"
+        if mode.lower() == "replace":
+            wrapper.__doc__ = doc
+        elif mode.lower() == "append":
+            tmp = re.sub(pattern, "", wrapper.__doc__)
+            new_lines = 1 - (len(tmp) - len(tmp.rstrip("\n")))
+            tmp = re.sub(pattern, "", doc)
+            new_lines -= len(tmp) - len(tmp.lstrip("\n"))
+            new_lines = max(0, new_lines) * "\n"
+            wrapper.__doc__ += new_lines + doc
+        elif mode.lower() == "prepend":
+            tmp = re.sub(pattern, "", doc)
+            new_lines = 1 - (len(tmp) - len(tmp.rstrip("\n")))
+            tmp = re.sub(pattern, "", wrapper.__doc__)
+            new_lines -= len(tmp) - len(tmp.lstrip("\n"))
+            new_lines = max(0, new_lines) * "\n"
+            wrapper.__doc__ = doc + new_lines + wrapper.__doc__
+        else:
+            raise ValueError(f"mode {mode} is not supported")
+        return wrapper
+
+    return decorator
```

### Comparing `torch_ecg-0.0.8/torch_ecg/utils/pantompkins.py` & `torch_ecg-0.0.9/torch_ecg/utils/pantompkins.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg/utils/utils_nn.py` & `torch_ecg-0.0.9/torch_ecg/utils/utils_nn.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/PKG-INFO` & `torch_ecg-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch_ecg
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Deep Learning Framework for ECG Processing Tasks Based on PyTorch
 Home-page: https://github.com/DeepPSP/torch_ecg
 Author: DeepPSP
 Author-email: wenh06@gmail.com
 License: MIT
 Description: # [torch_ecg](https://github.com/DeepPSP/torch_ecg/)
```

### Comparing `torch_ecg-0.0.8/test/test_pipelines.py` & `torch_ecg-0.0.9/test/test_pipelines.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/test/test_model_configs.py` & `torch_ecg-0.0.9/test/test_model_configs.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/test/test_cnn.py` & `torch_ecg-0.0.9/test/test_cnn.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/test/test_nets.py` & `torch_ecg-0.0.9/test/test_nets.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/test/test_loss.py` & `torch_ecg-0.0.9/test/test_loss.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/test/test_downstream_tasks.py` & `torch_ecg-0.0.9/test/test_downstream_tasks.py`

 * *Files identical despite different names*

### Comparing `torch_ecg-0.0.8/torch_ecg.egg-info/SOURCES.txt` & `torch_ecg-0.0.9/torch_ecg.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -31,14 +31,20 @@
 torch_ecg/augmenters/cutmix.py
 torch_ecg/augmenters/label_smooth.py
 torch_ecg/augmenters/mixup.py
 torch_ecg/augmenters/random_flip.py
 torch_ecg/augmenters/random_masking.py
 torch_ecg/augmenters/random_renormalize.py
 torch_ecg/augmenters/stretch_compress.py
+torch_ecg/components/__init__.py
+torch_ecg/components/loggers.py
+torch_ecg/components/metrics.py
+torch_ecg/components/nas.py
+torch_ecg/components/outputs.py
+torch_ecg/components/trainer.py
 torch_ecg/databases/__init__.py
 torch_ecg/databases/base.py
 torch_ecg/databases/aux_data/__init__.py
 torch_ecg/databases/aux_data/cinc2020_aux_data.py
 torch_ecg/databases/aux_data/cinc2021_aux_data.py
 torch_ecg/databases/aux_data/physionet_dbs.csv.tar.gz
 torch_ecg/databases/cpsc_databases/__init__.py
@@ -125,20 +131,16 @@
 torch_ecg/preprocessors/normalize.py
 torch_ecg/preprocessors/preproc_manager.py
 torch_ecg/preprocessors/resample.py
 torch_ecg/utils/__init__.py
 torch_ecg/utils/download.py
 torch_ecg/utils/ecg_arrhythmia_knowledge.py
 torch_ecg/utils/edr.py
-torch_ecg/utils/loggers.py
 torch_ecg/utils/misc.py
-torch_ecg/utils/nas.py
-torch_ecg/utils/outputs.py
 torch_ecg/utils/pantompkins.py
 torch_ecg/utils/preproc.py
 torch_ecg/utils/rpeaks.py
-torch_ecg/utils/trainer.py
 torch_ecg/utils/utils_interval.py
 torch_ecg/utils/utils_metrics.py
 torch_ecg/utils/utils_nn.py
 torch_ecg/utils/utils_signal.py
 torch_ecg/utils/utils_signal_t.py
```

### Comparing `torch_ecg-0.0.8/torch_ecg.egg-info/PKG-INFO` & `torch_ecg-0.0.9/torch_ecg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-ecg
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Deep Learning Framework for ECG Processing Tasks Based on PyTorch
 Home-page: https://github.com/DeepPSP/torch_ecg
 Author: DeepPSP
 Author-email: wenh06@gmail.com
 License: MIT
 Description: # [torch_ecg](https://github.com/DeepPSP/torch_ecg/)
```

