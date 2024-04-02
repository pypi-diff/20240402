# Comparing `tmp/cfm_task_models-0.0.8.tar.gz` & `tmp/cfm_task_models-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfm_task_models-0.0.8.tar", max compression
+gzip compressed data, was "cfm_task_models-0.0.9.tar", max compression
```

## Comparing `cfm_task_models-0.0.8.tar` & `cfm_task_models-0.0.9.tar`

### file list

```diff
@@ -1,96 +1,96 @@
--rw-r--r--   0        0        0     1050 2024-03-01 18:18:42.354337 cfm_task_models-0.0.8/README.md
--rw-r--r--   0        0        0       71 2024-03-01 19:31:47.463444 cfm_task_models-0.0.8/cfm_task_models/__init__.py
--rw-r--r--   0        0        0      174 2024-03-20 22:56:34.874427 cfm_task_models-0.0.8/cfm_task_models/legacy/__init__.py
--rw-r--r--   0        0        0    22317 2024-03-20 22:22:50.212151 cfm_task_models-0.0.8/cfm_task_models/legacy/assigners.py
--rw-r--r--   0        0        0     2129 2024-03-20 23:22:48.791679 cfm_task_models-0.0.8/cfm_task_models/legacy/builder_legacy.py
--rw-r--r--   0        0        0    20232 2024-03-20 22:57:03.406538 cfm_task_models-0.0.8/cfm_task_models/legacy/condconv.py
--rw-r--r--   0        0        0     7634 2024-03-20 22:46:54.180562 cfm_task_models-0.0.8/cfm_task_models/legacy/losses.py
--rw-r--r--   0        0        0    20225 2024-03-22 17:43:24.916237 cfm_task_models-0.0.8/cfm_task_models/legacy/mmdet_extras.py
--rw-r--r--   0        0        0    62060 2024-03-20 23:15:37.610230 cfm_task_models-0.0.8/cfm_task_models/legacy/reppoints.py
--rw-r--r--   0        0        0     4104 2024-03-20 22:16:19.555000 cfm_task_models-0.0.8/cfm_task_models/legacy/utils.py
--rw-r--r--   0        0        0    11831 2024-02-26 21:57:20.823993 cfm_task_models-0.0.8/cfm_task_models/mask-rcnn_swin-t-p4-w7_fpn_1x_coco.py
--rw-r--r--   0        0        0      200 2024-03-01 17:03:16.188337 cfm_task_models-0.0.8/cfm_task_models/miminstaller.py
--rw-r--r--   0        0        0     9095 2024-02-26 21:57:20.823993 cfm_task_models-0.0.8/cfm_task_models/mmdet_dataset_download.py
--rw-r--r--   0        0        0      444 2024-02-21 18:41:59.002182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1141 2024-02-21 18:41:59.002182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/LICENSE
--rw-r--r--   0        0        0    48226 2024-02-21 18:41:59.006182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/MODELHUB.md
--rw-r--r--   0        0        0    30329 2024-02-21 18:41:59.006182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/README.md
--rw-r--r--   0        0        0     2780 2024-02-21 18:41:59.006182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/SECURITY.md
--rw-r--r--   0        0        0     1315 2024-02-21 18:41:59.006182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/SUPPORT.md
--rw-r--r--   0        0        0        0 2024-02-29 00:44:16.638946 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/__init__.py
--rw-r--r--   0        0        0    11568 2024-02-21 18:41:59.006182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/config.py
--rw-r--r--   0        0        0      414 2024-02-21 18:41:59.006182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/configs/simmim/simmim_finetune__swin_base__img224_window7__800ep.yaml
--rw-r--r--   0        0        0      470 2024-02-21 18:41:59.006182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/configs/simmim/simmim_finetune__swinv2_base__img224_window14__800ep.yaml
--rw-r--r--   0        0        0      489 2024-02-21 18:41:59.006182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/configs/simmim/simmim_pretrain__swin_base__img192_window6__800ep.yaml
--rw-r--r--   0        0        0      564 2024-02-21 18:41:59.006182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/configs/simmim/simmim_pretrain__swinv2_base__img192_window12__800ep.yaml
--rw-r--r--   0        0        0      357 2024-02-21 18:41:59.006182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/configs/swin/swin_base_patch4_window12_384_22kto1k_finetune.yaml
--rw-r--r--   0        0        0      349 2024-02-21 18:41:59.006182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/configs/swin/swin_base_patch4_window12_384_finetune.yaml
--rw-r--r--   0        0        0      184 2024-02-21 18:41:59.006182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/configs/swin/swin_base_patch4_window7_224.yaml
--rw-r--r--   0        0        0      353 2024-02-21 18:41:59.006182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/configs/swin/swin_base_patch4_window7_224_22k.yaml
--rw-r--r--   0        0        0      313 2024-02-21 18:41:59.006182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/configs/swin/swin_base_patch4_window7_224_22kto1k_finetune.yaml
--rw-r--r--   0        0        0      359 2024-02-21 18:41:59.006182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/configs/swin/swin_large_patch4_window12_384_22kto1k_finetune.yaml
--rw-r--r--   0        0        0      355 2024-02-21 18:41:59.006182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/configs/swin/swin_large_patch4_window7_224_22k.yaml
--rw-r--r--   0        0        0      315 2024-02-21 18:41:59.006182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/configs/swin/swin_large_patch4_window7_224_22kto1k_finetune.yaml
--rw-r--r--   0        0        0      184 2024-02-21 18:41:59.006182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/configs/swin/swin_small_patch4_window7_224.yaml
--rw-r--r--   0        0        0      353 2024-02-21 18:41:59.006182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/configs/swin/swin_small_patch4_window7_224_22k.yaml
--rw-r--r--   0        0        0      313 2024-02-21 18:41:59.006182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/configs/swin/swin_small_patch4_window7_224_22kto1k_finetune.yaml
--rw-r--r--   0        0        0      208 2024-02-21 18:41:59.006182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/configs/swin/swin_tiny_c24_patch4_window8_256.yaml
--rw-r--r--   0        0        0      182 2024-02-21 18:41:59.006182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/configs/swin/swin_tiny_patch4_window7_224.yaml
--rw-r--r--   0        0        0      351 2024-02-21 18:41:59.006182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/configs/swin/swin_tiny_patch4_window7_224_22k.yaml
--rw-r--r--   0        0        0      311 2024-02-21 18:41:59.006182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/configs/swin/swin_tiny_patch4_window7_224_22kto1k_finetune.yaml
--rw-r--r--   0        0        0      197 2024-02-21 18:41:59.006182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/configs/swinmlp/swin_mlp_base_patch4_window7_224.yaml
--rw-r--r--   0        0        0      221 2024-02-21 18:41:59.006182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/configs/swinmlp/swin_mlp_tiny_c12_patch4_window8_256.yaml
--rw-r--r--   0        0        0      220 2024-02-21 18:41:59.006182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/configs/swinmlp/swin_mlp_tiny_c24_patch4_window8_256.yaml
--rw-r--r--   0        0        0      222 2024-02-21 18:41:59.006182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/configs/swinmlp/swin_mlp_tiny_c6_patch4_window8_256.yaml
--rw-r--r--   0        0        0      697 2024-02-21 18:41:59.006182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/configs/swinmoe/swin_moe_base_patch4_window12_192_16expert_32gpu_22k.yaml
--rw-r--r--   0        0        0      696 2024-02-21 18:41:59.006182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/configs/swinmoe/swin_moe_base_patch4_window12_192_32expert_32gpu_22k.yaml
--rw-r--r--   0        0        0      696 2024-02-21 18:41:59.006182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/configs/swinmoe/swin_moe_base_patch4_window12_192_8expert_32gpu_22k.yaml
--rw-r--r--   0        0        0      734 2024-02-21 18:41:59.006182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/configs/swinmoe/swin_moe_base_patch4_window12_192_cosine_router_32expert_32gpu_22k.yaml
--rw-r--r--   0        0        0      540 2024-02-21 18:41:59.006182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/configs/swinmoe/swin_moe_base_patch4_window12_192_densebaseline_22k.yaml
--rw-r--r--   0        0        0      697 2024-02-21 18:41:59.006182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/configs/swinmoe/swin_moe_small_patch4_window12_192_16expert_32gpu_22k.yaml
--rw-r--r--   0        0        0      696 2024-02-21 18:41:59.006182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/configs/swinmoe/swin_moe_small_patch4_window12_192_32expert_32gpu_22k.yaml
--rw-r--r--   0        0        0      696 2024-02-21 18:41:59.006182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/configs/swinmoe/swin_moe_small_patch4_window12_192_64expert_64gpu_22k.yaml
--rw-r--r--   0        0        0      696 2024-02-21 18:41:59.006182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/configs/swinmoe/swin_moe_small_patch4_window12_192_8expert_32gpu_22k.yaml
--rw-r--r--   0        0        0      734 2024-02-21 18:41:59.006182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/configs/swinmoe/swin_moe_small_patch4_window12_192_cosine_router_32expert_32gpu_22k.yaml
--rw-r--r--   0        0        0      540 2024-02-21 18:41:59.006182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/configs/swinmoe/swin_moe_small_patch4_window12_192_densebaseline_22k.yaml
--rw-r--r--   0        0        0      376 2024-02-21 18:41:59.006182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/configs/swinv2/swinv2_base_patch4_window12_192_22k.yaml
--rw-r--r--   0        0        0      393 2024-02-21 18:41:59.006182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/configs/swinv2/swinv2_base_patch4_window12to16_192to256_22kto1k_ft.yaml
--rw-r--r--   0        0        0      413 2024-02-21 18:41:59.006182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/configs/swinv2/swinv2_base_patch4_window12to24_192to384_22kto1k_ft.yaml
--rw-r--r--   0        0        0      214 2024-02-21 18:41:59.006182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/configs/swinv2/swinv2_base_patch4_window16_256.yaml
--rw-r--r--   0        0        0      212 2024-02-21 18:41:59.006182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/configs/swinv2/swinv2_base_patch4_window8_256.yaml
--rw-r--r--   0        0        0      378 2024-02-21 18:41:59.006182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/configs/swinv2/swinv2_large_patch4_window12_192_22k.yaml
--rw-r--r--   0        0        0      394 2024-02-21 18:41:59.006182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/configs/swinv2/swinv2_large_patch4_window12to16_192to256_22kto1k_ft.yaml
--rw-r--r--   0        0        0      415 2024-02-21 18:41:59.006182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/configs/swinv2/swinv2_large_patch4_window12to24_192to384_22kto1k_ft.yaml
--rw-r--r--   0        0        0      214 2024-02-21 18:41:59.006182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/configs/swinv2/swinv2_small_patch4_window16_256.yaml
--rw-r--r--   0        0        0      212 2024-02-21 18:41:59.006182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/configs/swinv2/swinv2_small_patch4_window8_256.yaml
--rw-r--r--   0        0        0      212 2024-02-21 18:41:59.006182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/configs/swinv2/swinv2_tiny_patch4_window16_256.yaml
--rw-r--r--   0        0        0      210 2024-02-21 18:41:59.006182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/configs/swinv2/swinv2_tiny_patch4_window8_256.yaml
--rw-r--r--   0        0        0   930622 2024-02-21 18:41:59.022182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/figures/teaser.png
--rw-r--r--   0        0        0    12112 2024-02-21 18:41:59.022182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/get_started.md
--rw-r--r--   0        0        0      343 2024-02-21 18:41:59.022182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/kernels/window_process/setup.py
--rw-r--r--   0        0        0     3704 2024-02-21 18:41:59.022182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/kernels/window_process/swin_window_process.cpp
--rw-r--r--   0        0        0     9693 2024-02-21 18:41:59.022182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/kernels/window_process/swin_window_process_kernel.cu
--rw-r--r--   0        0        0     9592 2024-02-21 18:41:59.022182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/kernels/window_process/unit_test.py
--rw-r--r--   0        0        0     2015 2024-02-21 18:41:59.022182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/kernels/window_process/window_process.py
--rw-r--r--   0        0        0     1451 2024-02-21 18:41:59.022182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/logger.py
--rw-r--r--   0        0        0     5467 2024-02-21 18:41:59.022182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/lr_scheduler.py
--rw-r--r--   0        0        0    14883 2024-02-21 18:41:59.022182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/main.py
--rw-r--r--   0        0        0    16224 2024-02-21 18:41:59.022182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/main_moe.py
--rw-r--r--   0        0        0    13692 2024-02-21 18:41:59.022182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/main_simmim_ft.py
--rw-r--r--   0        0        0     9414 2024-02-21 18:41:59.022182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/main_simmim_pt.py
--rw-r--r--   0        0        0       30 2024-02-21 18:41:59.022182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/models/__init__.py
--rw-r--r--   0        0        0     7136 2024-02-21 18:41:59.022182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/models/build.py
--rw-r--r--   0        0        0     7119 2024-02-21 18:41:59.022182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/models/simmim.py
--rw-r--r--   0        0        0    18508 2024-02-21 18:41:59.022182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/models/swin_mlp.py
--rw-r--r--   0        0        0    26070 2024-02-21 18:41:59.022182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/models/swin_transformer.py
--rw-r--r--   0        0        0    38203 2024-02-21 18:41:59.022182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/models/swin_transformer_moe.py
--rw-r--r--   0        0        0    32110 2024-02-26 21:57:20.823993 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/models/swin_transformer_v2.py
--rw-r--r--   0        0        0     6183 2024-02-21 18:41:59.022182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/optimizer.py
--rw-r--r--   0        0        0     9598 2024-02-21 18:41:59.022182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/utils.py
--rw-r--r--   0        0        0    11397 2024-02-21 18:41:59.022182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/utils_moe.py
--rw-r--r--   0        0        0     8415 2024-02-21 18:41:59.022182 cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/utils_simmim.py
--rw-r--r--   0        0        0        0 2024-02-29 00:45:15.587064 cfm_task_models-0.0.8/cfm_task_models/models/__init__.py
--rw-r--r--   0        0        0    54973 2024-03-22 17:45:48.768651 cfm_task_models-0.0.8/cfm_task_models/playground.ipynb
--rw-r--r--   0        0        0    15374 2024-03-22 17:01:24.928691 cfm_task_models-0.0.8/cfm_task_models/split_utils.py
--rw-r--r--   0        0        0     1462 2024-03-22 17:47:59.925029 cfm_task_models-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1714 1970-01-01 00:00:00.000000 cfm_task_models-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1050 2024-03-01 18:18:42.354337 cfm_task_models-0.0.9/README.md
+-rw-r--r--   0        0        0       71 2024-03-01 19:31:47.463444 cfm_task_models-0.0.9/cfm_task_models/__init__.py
+-rw-r--r--   0        0        0      174 2024-03-20 22:56:34.874427 cfm_task_models-0.0.9/cfm_task_models/legacy/__init__.py
+-rw-r--r--   0        0        0    22317 2024-03-20 22:22:50.212151 cfm_task_models-0.0.9/cfm_task_models/legacy/assigners.py
+-rw-r--r--   0        0        0     2129 2024-03-20 23:22:48.791679 cfm_task_models-0.0.9/cfm_task_models/legacy/builder_legacy.py
+-rw-r--r--   0        0        0    20232 2024-03-20 22:57:03.406538 cfm_task_models-0.0.9/cfm_task_models/legacy/condconv.py
+-rw-r--r--   0        0        0     7634 2024-03-20 22:46:54.180562 cfm_task_models-0.0.9/cfm_task_models/legacy/losses.py
+-rw-r--r--   0        0        0    20225 2024-03-22 17:43:24.916237 cfm_task_models-0.0.9/cfm_task_models/legacy/mmdet_extras.py
+-rw-r--r--   0        0        0    62055 2024-03-22 18:08:38.348420 cfm_task_models-0.0.9/cfm_task_models/legacy/reppoints.py
+-rw-r--r--   0        0        0     4104 2024-03-20 22:16:19.555000 cfm_task_models-0.0.9/cfm_task_models/legacy/utils.py
+-rw-r--r--   0        0        0    11831 2024-02-26 21:57:20.823993 cfm_task_models-0.0.9/cfm_task_models/mask-rcnn_swin-t-p4-w7_fpn_1x_coco.py
+-rw-r--r--   0        0        0      200 2024-03-01 17:03:16.188337 cfm_task_models-0.0.9/cfm_task_models/miminstaller.py
+-rw-r--r--   0        0        0     9095 2024-02-26 21:57:20.823993 cfm_task_models-0.0.9/cfm_task_models/mmdet_dataset_download.py
+-rw-r--r--   0        0        0      444 2024-02-21 18:41:59.002182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1141 2024-02-21 18:41:59.002182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/LICENSE
+-rw-r--r--   0        0        0    48226 2024-02-21 18:41:59.006182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/MODELHUB.md
+-rw-r--r--   0        0        0    30329 2024-02-21 18:41:59.006182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/README.md
+-rw-r--r--   0        0        0     2780 2024-02-21 18:41:59.006182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/SECURITY.md
+-rw-r--r--   0        0        0     1315 2024-02-21 18:41:59.006182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/SUPPORT.md
+-rw-r--r--   0        0        0        0 2024-02-29 00:44:16.638946 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/__init__.py
+-rw-r--r--   0        0        0    11568 2024-02-21 18:41:59.006182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/config.py
+-rw-r--r--   0        0        0      414 2024-02-21 18:41:59.006182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/configs/simmim/simmim_finetune__swin_base__img224_window7__800ep.yaml
+-rw-r--r--   0        0        0      470 2024-02-21 18:41:59.006182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/configs/simmim/simmim_finetune__swinv2_base__img224_window14__800ep.yaml
+-rw-r--r--   0        0        0      489 2024-02-21 18:41:59.006182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/configs/simmim/simmim_pretrain__swin_base__img192_window6__800ep.yaml
+-rw-r--r--   0        0        0      564 2024-02-21 18:41:59.006182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/configs/simmim/simmim_pretrain__swinv2_base__img192_window12__800ep.yaml
+-rw-r--r--   0        0        0      357 2024-02-21 18:41:59.006182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/configs/swin/swin_base_patch4_window12_384_22kto1k_finetune.yaml
+-rw-r--r--   0        0        0      349 2024-02-21 18:41:59.006182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/configs/swin/swin_base_patch4_window12_384_finetune.yaml
+-rw-r--r--   0        0        0      184 2024-02-21 18:41:59.006182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/configs/swin/swin_base_patch4_window7_224.yaml
+-rw-r--r--   0        0        0      353 2024-02-21 18:41:59.006182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/configs/swin/swin_base_patch4_window7_224_22k.yaml
+-rw-r--r--   0        0        0      313 2024-02-21 18:41:59.006182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/configs/swin/swin_base_patch4_window7_224_22kto1k_finetune.yaml
+-rw-r--r--   0        0        0      359 2024-02-21 18:41:59.006182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/configs/swin/swin_large_patch4_window12_384_22kto1k_finetune.yaml
+-rw-r--r--   0        0        0      355 2024-02-21 18:41:59.006182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/configs/swin/swin_large_patch4_window7_224_22k.yaml
+-rw-r--r--   0        0        0      315 2024-02-21 18:41:59.006182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/configs/swin/swin_large_patch4_window7_224_22kto1k_finetune.yaml
+-rw-r--r--   0        0        0      184 2024-02-21 18:41:59.006182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/configs/swin/swin_small_patch4_window7_224.yaml
+-rw-r--r--   0        0        0      353 2024-02-21 18:41:59.006182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/configs/swin/swin_small_patch4_window7_224_22k.yaml
+-rw-r--r--   0        0        0      313 2024-02-21 18:41:59.006182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/configs/swin/swin_small_patch4_window7_224_22kto1k_finetune.yaml
+-rw-r--r--   0        0        0      208 2024-02-21 18:41:59.006182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/configs/swin/swin_tiny_c24_patch4_window8_256.yaml
+-rw-r--r--   0        0        0      182 2024-02-21 18:41:59.006182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/configs/swin/swin_tiny_patch4_window7_224.yaml
+-rw-r--r--   0        0        0      351 2024-02-21 18:41:59.006182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/configs/swin/swin_tiny_patch4_window7_224_22k.yaml
+-rw-r--r--   0        0        0      311 2024-02-21 18:41:59.006182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/configs/swin/swin_tiny_patch4_window7_224_22kto1k_finetune.yaml
+-rw-r--r--   0        0        0      197 2024-02-21 18:41:59.006182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/configs/swinmlp/swin_mlp_base_patch4_window7_224.yaml
+-rw-r--r--   0        0        0      221 2024-02-21 18:41:59.006182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/configs/swinmlp/swin_mlp_tiny_c12_patch4_window8_256.yaml
+-rw-r--r--   0        0        0      220 2024-02-21 18:41:59.006182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/configs/swinmlp/swin_mlp_tiny_c24_patch4_window8_256.yaml
+-rw-r--r--   0        0        0      222 2024-02-21 18:41:59.006182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/configs/swinmlp/swin_mlp_tiny_c6_patch4_window8_256.yaml
+-rw-r--r--   0        0        0      697 2024-02-21 18:41:59.006182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/configs/swinmoe/swin_moe_base_patch4_window12_192_16expert_32gpu_22k.yaml
+-rw-r--r--   0        0        0      696 2024-02-21 18:41:59.006182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/configs/swinmoe/swin_moe_base_patch4_window12_192_32expert_32gpu_22k.yaml
+-rw-r--r--   0        0        0      696 2024-02-21 18:41:59.006182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/configs/swinmoe/swin_moe_base_patch4_window12_192_8expert_32gpu_22k.yaml
+-rw-r--r--   0        0        0      734 2024-02-21 18:41:59.006182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/configs/swinmoe/swin_moe_base_patch4_window12_192_cosine_router_32expert_32gpu_22k.yaml
+-rw-r--r--   0        0        0      540 2024-02-21 18:41:59.006182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/configs/swinmoe/swin_moe_base_patch4_window12_192_densebaseline_22k.yaml
+-rw-r--r--   0        0        0      697 2024-02-21 18:41:59.006182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/configs/swinmoe/swin_moe_small_patch4_window12_192_16expert_32gpu_22k.yaml
+-rw-r--r--   0        0        0      696 2024-02-21 18:41:59.006182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/configs/swinmoe/swin_moe_small_patch4_window12_192_32expert_32gpu_22k.yaml
+-rw-r--r--   0        0        0      696 2024-02-21 18:41:59.006182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/configs/swinmoe/swin_moe_small_patch4_window12_192_64expert_64gpu_22k.yaml
+-rw-r--r--   0        0        0      696 2024-02-21 18:41:59.006182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/configs/swinmoe/swin_moe_small_patch4_window12_192_8expert_32gpu_22k.yaml
+-rw-r--r--   0        0        0      734 2024-02-21 18:41:59.006182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/configs/swinmoe/swin_moe_small_patch4_window12_192_cosine_router_32expert_32gpu_22k.yaml
+-rw-r--r--   0        0        0      540 2024-02-21 18:41:59.006182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/configs/swinmoe/swin_moe_small_patch4_window12_192_densebaseline_22k.yaml
+-rw-r--r--   0        0        0      376 2024-02-21 18:41:59.006182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/configs/swinv2/swinv2_base_patch4_window12_192_22k.yaml
+-rw-r--r--   0        0        0      393 2024-02-21 18:41:59.006182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/configs/swinv2/swinv2_base_patch4_window12to16_192to256_22kto1k_ft.yaml
+-rw-r--r--   0        0        0      413 2024-02-21 18:41:59.006182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/configs/swinv2/swinv2_base_patch4_window12to24_192to384_22kto1k_ft.yaml
+-rw-r--r--   0        0        0      214 2024-02-21 18:41:59.006182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/configs/swinv2/swinv2_base_patch4_window16_256.yaml
+-rw-r--r--   0        0        0      212 2024-02-21 18:41:59.006182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/configs/swinv2/swinv2_base_patch4_window8_256.yaml
+-rw-r--r--   0        0        0      378 2024-02-21 18:41:59.006182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/configs/swinv2/swinv2_large_patch4_window12_192_22k.yaml
+-rw-r--r--   0        0        0      394 2024-02-21 18:41:59.006182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/configs/swinv2/swinv2_large_patch4_window12to16_192to256_22kto1k_ft.yaml
+-rw-r--r--   0        0        0      415 2024-02-21 18:41:59.006182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/configs/swinv2/swinv2_large_patch4_window12to24_192to384_22kto1k_ft.yaml
+-rw-r--r--   0        0        0      214 2024-02-21 18:41:59.006182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/configs/swinv2/swinv2_small_patch4_window16_256.yaml
+-rw-r--r--   0        0        0      212 2024-02-21 18:41:59.006182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/configs/swinv2/swinv2_small_patch4_window8_256.yaml
+-rw-r--r--   0        0        0      212 2024-02-21 18:41:59.006182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/configs/swinv2/swinv2_tiny_patch4_window16_256.yaml
+-rw-r--r--   0        0        0      210 2024-02-21 18:41:59.006182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/configs/swinv2/swinv2_tiny_patch4_window8_256.yaml
+-rw-r--r--   0        0        0   930622 2024-02-21 18:41:59.022182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/figures/teaser.png
+-rw-r--r--   0        0        0    12112 2024-02-21 18:41:59.022182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/get_started.md
+-rw-r--r--   0        0        0      343 2024-02-21 18:41:59.022182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/kernels/window_process/setup.py
+-rw-r--r--   0        0        0     3704 2024-02-21 18:41:59.022182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/kernels/window_process/swin_window_process.cpp
+-rw-r--r--   0        0        0     9693 2024-02-21 18:41:59.022182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/kernels/window_process/swin_window_process_kernel.cu
+-rw-r--r--   0        0        0     9592 2024-02-21 18:41:59.022182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/kernels/window_process/unit_test.py
+-rw-r--r--   0        0        0     2015 2024-02-21 18:41:59.022182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/kernels/window_process/window_process.py
+-rw-r--r--   0        0        0     1451 2024-02-21 18:41:59.022182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/logger.py
+-rw-r--r--   0        0        0     5467 2024-02-21 18:41:59.022182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/lr_scheduler.py
+-rw-r--r--   0        0        0    14883 2024-02-21 18:41:59.022182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/main.py
+-rw-r--r--   0        0        0    16224 2024-02-21 18:41:59.022182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/main_moe.py
+-rw-r--r--   0        0        0    13692 2024-02-21 18:41:59.022182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/main_simmim_ft.py
+-rw-r--r--   0        0        0     9414 2024-02-21 18:41:59.022182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/main_simmim_pt.py
+-rw-r--r--   0        0        0       30 2024-02-21 18:41:59.022182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/models/__init__.py
+-rw-r--r--   0        0        0     7136 2024-02-21 18:41:59.022182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/models/build.py
+-rw-r--r--   0        0        0     7119 2024-02-21 18:41:59.022182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/models/simmim.py
+-rw-r--r--   0        0        0    18508 2024-02-21 18:41:59.022182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/models/swin_mlp.py
+-rw-r--r--   0        0        0    26070 2024-02-21 18:41:59.022182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/models/swin_transformer.py
+-rw-r--r--   0        0        0    38203 2024-02-21 18:41:59.022182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/models/swin_transformer_moe.py
+-rw-r--r--   0        0        0    32110 2024-02-26 21:57:20.823993 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/models/swin_transformer_v2.py
+-rw-r--r--   0        0        0     6183 2024-02-21 18:41:59.022182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/optimizer.py
+-rw-r--r--   0        0        0     9598 2024-02-21 18:41:59.022182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/utils.py
+-rw-r--r--   0        0        0    11397 2024-02-21 18:41:59.022182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/utils_moe.py
+-rw-r--r--   0        0        0     8415 2024-02-21 18:41:59.022182 cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/utils_simmim.py
+-rw-r--r--   0        0        0        0 2024-02-29 00:45:15.587064 cfm_task_models-0.0.9/cfm_task_models/models/__init__.py
+-rw-r--r--   0        0        0    51363 2024-03-22 18:08:17.216362 cfm_task_models-0.0.9/cfm_task_models/playground.ipynb
+-rw-r--r--   0        0        0    15374 2024-03-22 17:01:24.928691 cfm_task_models-0.0.9/cfm_task_models/split_utils.py
+-rw-r--r--   0        0        0     1462 2024-03-22 18:09:01.816484 cfm_task_models-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1714 1970-01-01 00:00:00.000000 cfm_task_models-0.0.9/PKG-INFO
```

### Comparing `cfm_task_models-0.0.8/README.md` & `cfm_task_models-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `cfm_task_models-0.0.8/cfm_task_models/legacy/assigners.py` & `cfm_task_models-0.0.9/cfm_task_models/legacy/assigners.py`

 * *Files identical despite different names*

### Comparing `cfm_task_models-0.0.8/cfm_task_models/legacy/builder_legacy.py` & `cfm_task_models-0.0.9/cfm_task_models/legacy/builder_legacy.py`

 * *Files identical despite different names*

### Comparing `cfm_task_models-0.0.8/cfm_task_models/legacy/condconv.py` & `cfm_task_models-0.0.9/cfm_task_models/legacy/condconv.py`

 * *Files identical despite different names*

### Comparing `cfm_task_models-0.0.8/cfm_task_models/legacy/losses.py` & `cfm_task_models-0.0.9/cfm_task_models/legacy/losses.py`

 * *Files identical despite different names*

### Comparing `cfm_task_models-0.0.8/cfm_task_models/legacy/mmdet_extras.py` & `cfm_task_models-0.0.9/cfm_task_models/legacy/mmdet_extras.py`

 * *Files identical despite different names*

### Comparing `cfm_task_models-0.0.8/cfm_task_models/legacy/reppoints.py` & `cfm_task_models-0.0.9/cfm_task_models/legacy/reppoints.py`

 * *Files 0% similar despite different names*

```diff
@@ -419,15 +419,15 @@
             assert 0
         return torch.stack([out_x.flatten(), out_y.flatten()], dim=-1)
 
     def forward(self, feats):
         if not self.mask_head:
             return multi_apply(self.forward_single, feats)
         else:
-            self.pred_instances = Instances((0,0)) # just a dumy image shape
+            self.pred_instances = Instances() # just a dumy image shape
             bbox_res = multi_apply(self.forward_single, feats, controller=self.controller) # cls_out, pts_out_init, pts_out_refine, controller_out
             device = bbox_res[1][0].device
             self.level_sum = tuple(accumulate([0]+[r[:,0].numel() for r in bbox_res[1]][:-1]))
             self.image_sum = torch.tensor([r[0,0].numel() for r in bbox_res[1]])
             self.pred_instances.fpn_levels = torch.cat([torch.tensor([i]*r[:,0].numel()).to(device) for i,r in enumerate(bbox_res[1])])
             self.pred_instances.im_inds = torch.cat([torch.cat([torch.tensor([i]*img.numel()).to(device) for i,img in enumerate(r[:,0])]) for r in bbox_res[1]])
```

### Comparing `cfm_task_models-0.0.8/cfm_task_models/legacy/utils.py` & `cfm_task_models-0.0.9/cfm_task_models/legacy/utils.py`

 * *Files identical despite different names*

### Comparing `cfm_task_models-0.0.8/cfm_task_models/mask-rcnn_swin-t-p4-w7_fpn_1x_coco.py` & `cfm_task_models-0.0.9/cfm_task_models/mask-rcnn_swin-t-p4-w7_fpn_1x_coco.py`

 * *Files identical despite different names*

### Comparing `cfm_task_models-0.0.8/cfm_task_models/mmdet_dataset_download.py` & `cfm_task_models-0.0.9/cfm_task_models/mmdet_dataset_download.py`

 * *Files identical despite different names*

### Comparing `cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/LICENSE` & `cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/LICENSE`

 * *Files identical despite different names*

### Comparing `cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/MODELHUB.md` & `cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/MODELHUB.md`

 * *Files identical despite different names*

### Comparing `cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/README.md` & `cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/README.md`

 * *Files identical despite different names*

### Comparing `cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/SECURITY.md` & `cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/SECURITY.md`

 * *Files identical despite different names*

### Comparing `cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/SUPPORT.md` & `cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/SUPPORT.md`

 * *Files identical despite different names*

### Comparing `cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/config.py` & `cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/config.py`

 * *Files identical despite different names*

### Comparing `cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/configs/simmim/simmim_pretrain__swinv2_base__img192_window12__800ep.yaml` & `cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/configs/simmim/simmim_pretrain__swinv2_base__img192_window12__800ep.yaml`

 * *Files identical despite different names*

### Comparing `cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/configs/swinmoe/swin_moe_base_patch4_window12_192_16expert_32gpu_22k.yaml` & `cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/configs/swinmoe/swin_moe_base_patch4_window12_192_16expert_32gpu_22k.yaml`

 * *Files identical despite different names*

### Comparing `cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/configs/swinmoe/swin_moe_base_patch4_window12_192_32expert_32gpu_22k.yaml` & `cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/configs/swinmoe/swin_moe_base_patch4_window12_192_32expert_32gpu_22k.yaml`

 * *Files identical despite different names*

### Comparing `cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/configs/swinmoe/swin_moe_base_patch4_window12_192_8expert_32gpu_22k.yaml` & `cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/configs/swinmoe/swin_moe_base_patch4_window12_192_8expert_32gpu_22k.yaml`

 * *Files identical despite different names*

### Comparing `cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/configs/swinmoe/swin_moe_base_patch4_window12_192_cosine_router_32expert_32gpu_22k.yaml` & `cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/configs/swinmoe/swin_moe_base_patch4_window12_192_cosine_router_32expert_32gpu_22k.yaml`

 * *Files identical despite different names*

### Comparing `cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/configs/swinmoe/swin_moe_base_patch4_window12_192_densebaseline_22k.yaml` & `cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/configs/swinmoe/swin_moe_base_patch4_window12_192_densebaseline_22k.yaml`

 * *Files identical despite different names*

### Comparing `cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/configs/swinmoe/swin_moe_small_patch4_window12_192_16expert_32gpu_22k.yaml` & `cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/configs/swinmoe/swin_moe_small_patch4_window12_192_16expert_32gpu_22k.yaml`

 * *Files identical despite different names*

### Comparing `cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/configs/swinmoe/swin_moe_small_patch4_window12_192_32expert_32gpu_22k.yaml` & `cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/configs/swinmoe/swin_moe_small_patch4_window12_192_32expert_32gpu_22k.yaml`

 * *Files identical despite different names*

### Comparing `cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/configs/swinmoe/swin_moe_small_patch4_window12_192_64expert_64gpu_22k.yaml` & `cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/configs/swinmoe/swin_moe_small_patch4_window12_192_64expert_64gpu_22k.yaml`

 * *Files identical despite different names*

### Comparing `cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/configs/swinmoe/swin_moe_small_patch4_window12_192_8expert_32gpu_22k.yaml` & `cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/configs/swinmoe/swin_moe_small_patch4_window12_192_8expert_32gpu_22k.yaml`

 * *Files identical despite different names*

### Comparing `cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/configs/swinmoe/swin_moe_small_patch4_window12_192_cosine_router_32expert_32gpu_22k.yaml` & `cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/configs/swinmoe/swin_moe_small_patch4_window12_192_cosine_router_32expert_32gpu_22k.yaml`

 * *Files identical despite different names*

### Comparing `cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/configs/swinmoe/swin_moe_small_patch4_window12_192_densebaseline_22k.yaml` & `cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/configs/swinmoe/swin_moe_small_patch4_window12_192_densebaseline_22k.yaml`

 * *Files identical despite different names*

### Comparing `cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/figures/teaser.png` & `cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/figures/teaser.png`

 * *Files identical despite different names*

### Comparing `cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/get_started.md` & `cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/get_started.md`

 * *Files identical despite different names*

### Comparing `cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/kernels/window_process/swin_window_process.cpp` & `cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/kernels/window_process/swin_window_process.cpp`

 * *Files identical despite different names*

### Comparing `cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/kernels/window_process/swin_window_process_kernel.cu` & `cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/kernels/window_process/swin_window_process_kernel.cu`

 * *Files identical despite different names*

### Comparing `cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/kernels/window_process/unit_test.py` & `cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/kernels/window_process/unit_test.py`

 * *Files identical despite different names*

### Comparing `cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/kernels/window_process/window_process.py` & `cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/kernels/window_process/window_process.py`

 * *Files identical despite different names*

### Comparing `cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/logger.py` & `cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/logger.py`

 * *Files identical despite different names*

### Comparing `cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/lr_scheduler.py` & `cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/main.py` & `cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/main.py`

 * *Files identical despite different names*

### Comparing `cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/main_moe.py` & `cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/main_moe.py`

 * *Files identical despite different names*

### Comparing `cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/main_simmim_ft.py` & `cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/main_simmim_ft.py`

 * *Files identical despite different names*

### Comparing `cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/main_simmim_pt.py` & `cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/main_simmim_pt.py`

 * *Files identical despite different names*

### Comparing `cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/models/build.py` & `cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/models/build.py`

 * *Files identical despite different names*

### Comparing `cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/models/simmim.py` & `cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/models/simmim.py`

 * *Files identical despite different names*

### Comparing `cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/models/swin_mlp.py` & `cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/models/swin_mlp.py`

 * *Files identical despite different names*

### Comparing `cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/models/swin_transformer.py` & `cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/models/swin_transformer.py`

 * *Files identical despite different names*

### Comparing `cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/models/swin_transformer_moe.py` & `cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/models/swin_transformer_moe.py`

 * *Files identical despite different names*

### Comparing `cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/models/swin_transformer_v2.py` & `cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/models/swin_transformer_v2.py`

 * *Files identical despite different names*

### Comparing `cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/optimizer.py` & `cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/optimizer.py`

 * *Files identical despite different names*

### Comparing `cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/utils.py` & `cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/utils.py`

 * *Files identical despite different names*

### Comparing `cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/utils_moe.py` & `cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/utils_moe.py`

 * *Files identical despite different names*

### Comparing `cfm_task_models-0.0.8/cfm_task_models/models/Swin-Transformer/utils_simmim.py` & `cfm_task_models-0.0.9/cfm_task_models/models/Swin-Transformer/utils_simmim.py`

 * *Files identical despite different names*

### Comparing `cfm_task_models-0.0.8/cfm_task_models/playground.ipynb` & `cfm_task_models-0.0.9/cfm_task_models/playground.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9979166666666667%*

 * *Differences: {"'cells'": "{6: {'outputs': [], 'source': ['a = Instances()\\n', '\\n', 'fk = "*

 * *            'torch.Tensor([[[3,4]],[[4,5]],[[5,6]]])\\n\', "device = \'cuda\'\\n", \'a.fpn_levels '*

 * *            '= torch.cat([torch.tensor([i]*r[:,0].numel()).to(device) for i,r in '*

 * *            "enumerate(fk)])']}}"}*

```diff
@@ -278,99 +278,21 @@
                 "    break\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 14,
             "metadata": {},
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "[<DetDataSample(\n",
-                        "\n",
-                        "    META INFORMATION\n",
-                        "    img_shape: (427, 512)\n",
-                        "    img_path: '../data/coco/train2017/000000578037.jpg'\n",
-                        "    img_id: 578037\n",
-                        "    ori_shape: (427, 640)\n",
-                        "\n",
-                        "    DATA FIELDS\n",
-                        "    ignored_instances: <InstanceData(\n",
-                        "        \n",
-                        "            META INFORMATION\n",
-                        "        \n",
-                        "            DATA FIELDS\n",
-                        "            bboxes: HorizontalBoxes(\n",
-                        "                tensor([], size=(0, 4)))\n",
-                        "            labels: tensor([], dtype=torch.int64)\n",
-                        "            masks: BitmapMasks(num_masks=0, height=427, width=512)\n",
-                        "        ) at 0x7fce442ba430>\n",
-                        "    gt_instances: <InstanceData(\n",
-                        "        \n",
-                        "            META INFORMATION\n",
-                        "        \n",
-                        "            DATA FIELDS\n",
-                        "            bboxes: HorizontalBoxes(\n",
-                        "                tensor([[449.9900,  25.8800, 512.0000,  70.7800],\n",
-                        "                        [224.1400,  61.2700, 322.7500, 382.9600],\n",
-                        "                        [442.5600,  83.0300, 512.0000, 316.2200],\n",
-                        "                        [292.3400,  91.6600, 347.4300, 265.0600],\n",
-                        "                        [381.0900,  91.2200, 418.5100, 188.1400],\n",
-                        "                        [417.5800,  86.0700, 460.8600, 205.3300],\n",
-                        "                        [231.5300, 358.0400, 307.2600, 394.7000],\n",
-                        "                        [396.9500, 106.4800, 412.1000, 140.8500],\n",
-                        "                        [424.0800, 112.2600, 441.9000, 148.1100],\n",
-                        "                        [457.0500,  81.7300, 479.0400, 122.9700],\n",
-                        "                        [459.5500, 115.6300, 512.0000, 160.8600]]))\n",
-                        "            labels: tensor([25,  0,  0,  0,  0,  0, 36, 24, 24,  0, 24])\n",
-                        "            masks: BitmapMasks(num_masks=11, height=427, width=512)\n",
-                        "        ) at 0x7fce442bafa0>\n",
-                        ") at 0x7fce442bafd0>, <DetDataSample(\n",
-                        "\n",
-                        "    META INFORMATION\n",
-                        "    img_shape: (426, 512)\n",
-                        "    img_path: '../data/coco/train2017/000000220471.jpg'\n",
-                        "    img_id: 220471\n",
-                        "    ori_shape: (426, 640)\n",
-                        "\n",
-                        "    DATA FIELDS\n",
-                        "    ignored_instances: <InstanceData(\n",
-                        "        \n",
-                        "            META INFORMATION\n",
-                        "        \n",
-                        "            DATA FIELDS\n",
-                        "            bboxes: HorizontalBoxes(\n",
-                        "                tensor([], size=(0, 4)))\n",
-                        "            labels: tensor([], dtype=torch.int64)\n",
-                        "            masks: BitmapMasks(num_masks=0, height=426, width=512)\n",
-                        "        ) at 0x7fce442ba0a0>\n",
-                        "    gt_instances: <InstanceData(\n",
-                        "        \n",
-                        "            META INFORMATION\n",
-                        "        \n",
-                        "            DATA FIELDS\n",
-                        "            bboxes: HorizontalBoxes(\n",
-                        "                tensor([[181.0400, 169.4400, 330.3800, 321.6500],\n",
-                        "                        [323.3600, 151.4900, 504.8400, 299.5400],\n",
-                        "                        [316.9800, 254.6400, 512.0000, 403.9800],\n",
-                        "                        [  0.0000, 131.7800, 129.7900, 232.9200],\n",
-                        "                        [407.2800,  26.2000, 512.0000, 196.1400],\n",
-                        "                        [138.9200,   5.7400, 251.8800, 156.0400],\n",
-                        "                        [  0.0000,  68.1200, 512.0000, 421.2100]]))\n",
-                        "            labels: tensor([48, 48, 48, 48, 41, 41, 60])\n",
-                        "            masks: BitmapMasks(num_masks=7, height=426, width=512)\n",
-                        "        ) at 0x7fce442ba7f0>\n",
-                        ") at 0x7fce442ba7c0>]\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
-                "print(list(data['data_samples']))"
+                "a = Instances()\n",
+                "\n",
+                "fk = torch.Tensor([[[3,4]],[[4,5]],[[5,6]]])\n",
+                "device = 'cuda'\n",
+                "a.fpn_levels = torch.cat([torch.tensor([i]*r[:,0].numel()).to(device) for i,r in enumerate(fk)])"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 69,
             "metadata": {},
             "outputs": [
```

### Comparing `cfm_task_models-0.0.8/cfm_task_models/split_utils.py` & `cfm_task_models-0.0.9/cfm_task_models/split_utils.py`

 * *Files identical despite different names*

### Comparing `cfm_task_models-0.0.8/pyproject.toml` & `cfm_task_models-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cfm-task-models"
-version = "0.0.8"
+version = "0.0.9"
 description = "CFM - model zoo"
 authors = ["Alon Harell <aharell@sfu.ca>", "Masoud Khairi Atani <masoud_khairi_atani@sfu.ca>"]
 # exclude = ["tests/*"]
 packages = [
    { include = "cfm_task_models" }
 #    { include = "utils" },
 #    { include = "compressai_local"}
```

### Comparing `cfm_task_models-0.0.8/PKG-INFO` & `cfm_task_models-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfm-task-models
-Version: 0.0.8
+Version: 0.0.9
 Summary: CFM - model zoo
 Author: Alon Harell
 Author-email: aharell@sfu.ca
 Requires-Python: >=3.9.5,<=3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

