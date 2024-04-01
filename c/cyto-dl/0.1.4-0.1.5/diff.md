# Comparing `tmp/cyto-dl-0.1.4.tar.gz` & `tmp/cyto-dl-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyto-dl-0.1.4.tar", last modified: Sat Mar  9 00:10:10 2024, max compression
+gzip compressed data, was "cyto-dl-0.1.5.tar", last modified: Mon Apr  1 23:14:26 2024, max compression
```

## Comparing `cyto-dl-0.1.4.tar` & `cyto-dl-0.1.5.tar`

### file list

```diff
@@ -1,270 +1,275 @@
--rw-r--r--   0        0        0     5431 2024-03-09 00:09:58.326553 cyto-dl-0.1.4/README.md
--rw-r--r--   0        0        0      403 2024-03-09 00:09:58.326553 cyto-dl-0.1.4/configs/callbacks/default.yaml
--rw-r--r--   0        0        0     1250 2024-03-09 00:09:58.326553 cyto-dl-0.1.4/configs/callbacks/early_stopping.yaml
--rw-r--r--   0        0        0       80 2024-03-09 00:09:58.326553 cyto-dl-0.1.4/configs/callbacks/layer_freeze.yaml
--rw-r--r--   0        0        0       83 2024-03-09 00:09:58.326553 cyto-dl-0.1.4/configs/callbacks/learning_rate_monitor.yaml
--rw-r--r--   0        0        0     1298 2024-03-09 00:09:58.326553 cyto-dl-0.1.4/configs/callbacks/model_checkpoint.yaml
--rw-r--r--   0        0        0      402 2024-03-09 00:09:58.326553 cyto-dl-0.1.4/configs/callbacks/model_summary.yaml
--rw-r--r--   0        0        0        0 2024-03-09 00:09:58.326553 cyto-dl-0.1.4/configs/callbacks/none.yaml
--rw-r--r--   0        0        0      160 2024-03-09 00:09:58.326553 cyto-dl-0.1.4/configs/callbacks/outlier_detection.yaml
--rw-r--r--   0        0        0      289 2024-03-09 00:09:58.326553 cyto-dl-0.1.4/configs/callbacks/rich_progress_bar.yaml
--rw-r--r--   0        0        0      758 2024-03-09 00:09:58.326553 cyto-dl-0.1.4/configs/compile.yaml
--rw-r--r--   0        0        0     2634 2024-03-09 00:09:58.326553 cyto-dl-0.1.4/configs/data/classification/single_timepoint.yaml
--rw-r--r--   0        0        0     7077 2024-03-09 00:09:58.326553 cyto-dl-0.1.4/configs/data/im2im/gan.yaml
--rw-r--r--   0        0        0     7427 2024-03-09 00:09:58.326553 cyto-dl-0.1.4/configs/data/im2im/gan_superres.yaml
--rw-r--r--   0        0        0     6880 2024-03-09 00:09:58.326553 cyto-dl-0.1.4/configs/data/im2im/instance_seg.yaml
--rw-r--r--   0        0        0     5879 2024-03-09 00:09:58.326553 cyto-dl-0.1.4/configs/data/im2im/labelfree.yaml
--rw-r--r--   0        0        0     4374 2024-03-09 00:09:58.326553 cyto-dl-0.1.4/configs/data/im2im/mae.yaml
--rw-r--r--   0        0        0     6852 2024-03-09 00:09:58.326553 cyto-dl-0.1.4/configs/data/im2im/segmentation.yaml
--rw-r--r--   0        0        0     8222 2024-03-09 00:09:58.326553 cyto-dl-0.1.4/configs/data/im2im/segmentation_plugin.yaml
--rw-r--r--   0        0        0     7263 2024-03-09 00:09:58.326553 cyto-dl-0.1.4/configs/data/im2im/segmentation_superres.yaml
--rw-r--r--   0        0        0      450 2024-03-09 00:09:58.326553 cyto-dl-0.1.4/configs/data/private/lattice_nuc_sdf.yaml
--rw-r--r--   0        0        0      416 2024-03-09 00:09:58.326553 cyto-dl-0.1.4/configs/data/private/rot_mnist.yaml
--rw-r--r--   0        0        0      450 2024-03-09 00:09:58.326553 cyto-dl-0.1.4/configs/data/private/rot_mnist_vae.yaml
--rw-r--r--   0        0        0     1176 2024-03-09 00:09:58.326553 cyto-dl-0.1.4/configs/data/private/rotated_mnist.yaml
--rw-r--r--   0        0        0     1075 2024-03-09 00:09:58.326553 cyto-dl-0.1.4/configs/data/private/variance_3d.yaml
--rw-r--r--   0        0        0      497 2024-03-09 00:09:58.326553 cyto-dl-0.1.4/configs/data/private/variance_3d_npm1.yaml
--rw-r--r--   0        0        0      770 2024-03-09 00:09:58.326553 cyto-dl-0.1.4/configs/data/private/variance_3d_npm_nuc_v2.yaml
--rw-r--r--   0        0        0     1802 2024-03-09 00:09:58.326553 cyto-dl-0.1.4/configs/data/private/variance_3d_rotate.yaml
--rw-r--r--   0        0        0      547 2024-03-09 00:09:58.326553 cyto-dl-0.1.4/configs/data/private/variance_centerslice.yaml
--rw-r--r--   0        0        0      719 2024-03-09 00:09:58.326553 cyto-dl-0.1.4/configs/data/private/variance_centerslice_resize.yaml
--rw-r--r--   0        0        0      969 2024-03-09 00:09:58.326553 cyto-dl-0.1.4/configs/data/private/variance_npm1.yaml
--rw-r--r--   0        0        0      312 2024-03-09 00:09:58.326553 cyto-dl-0.1.4/configs/data/private/variance_spharm.yaml
--rw-r--r--   0        0        0      462 2024-03-09 00:09:58.326553 cyto-dl-0.1.4/configs/data/test/alternating_batch.yaml
--rw-r--r--   0        0        0      200 2024-03-09 00:09:58.326553 cyto-dl-0.1.4/configs/data/test/omnipose.yaml
--rw-r--r--   0        0        0      200 2024-03-09 00:09:58.326553 cyto-dl-0.1.4/configs/data/test/segmentation.yaml
--rw-r--r--   0        0        0      899 2024-03-09 00:09:58.326553 cyto-dl-0.1.4/configs/debug/default.yaml
--rw-r--r--   0        0        0      125 2024-03-09 00:09:58.326553 cyto-dl-0.1.4/configs/debug/fdr.yaml
--rw-r--r--   0        0        0      223 2024-03-09 00:09:58.326553 cyto-dl-0.1.4/configs/debug/limit.yaml
--rw-r--r--   0        0        0      209 2024-03-09 00:09:58.326553 cyto-dl-0.1.4/configs/debug/overfit.yaml
--rw-r--r--   0        0        0      182 2024-03-09 00:09:58.326553 cyto-dl-0.1.4/configs/debug/profiler.yaml
--rw-r--r--   0        0        0      509 2024-03-09 00:09:58.326553 cyto-dl-0.1.4/configs/eval.yaml
--rw-r--r--   0        0        0      659 2024-03-09 00:09:58.326553 cyto-dl-0.1.4/configs/experiment/classification/per_timepoint.yaml
--rw-r--r--   0        0        0     1065 2024-03-09 00:09:58.326553 cyto-dl-0.1.4/configs/experiment/im2im/gan.yaml
--rw-r--r--   0        0        0     1083 2024-03-09 00:09:58.326553 cyto-dl-0.1.4/configs/experiment/im2im/gan_superres.yaml
--rw-r--r--   0        0        0      932 2024-03-09 00:09:58.326553 cyto-dl-0.1.4/configs/experiment/im2im/instance_seg.yaml
--rw-r--r--   0        0        0      854 2024-03-09 00:09:58.326553 cyto-dl-0.1.4/configs/experiment/im2im/labelfree.yaml
--rw-r--r--   0        0        0      892 2024-03-09 00:09:58.326553 cyto-dl-0.1.4/configs/experiment/im2im/mae.yaml
--rw-r--r--   0        0        0      863 2024-03-09 00:09:58.326553 cyto-dl-0.1.4/configs/experiment/im2im/segmentation.yaml
--rw-r--r--   0        0        0     1126 2024-03-09 00:09:58.326553 cyto-dl-0.1.4/configs/experiment/im2im/segmentation_plugin.yaml
--rw-r--r--   0        0        0      881 2024-03-09 00:09:58.326553 cyto-dl-0.1.4/configs/experiment/im2im/segmentation_superres.yaml
--rw-r--r--   0        0        0     1098 2024-03-09 00:09:58.326553 cyto-dl-0.1.4/configs/experiment/im2im/vit_segmentation.yaml
--rw-r--r--   0        0        0     2741 2024-03-09 00:09:58.326553 cyto-dl-0.1.4/configs/experiment/private/lattice_nuc_sdf.yaml
--rw-r--r--   0        0        0     1583 2024-03-09 00:09:58.326553 cyto-dl-0.1.4/configs/experiment/private/mnist_so2.yaml
--rw-r--r--   0        0        0      989 2024-03-09 00:09:58.326553 cyto-dl-0.1.4/configs/experiment/private/npm1_classical_3d_vae.yaml
--rw-r--r--   0        0        0     2902 2024-03-09 00:09:58.326553 cyto-dl-0.1.4/configs/experiment/private/npm1_classical_scale_inv.yaml
--rw-r--r--   0        0        0     1037 2024-03-09 00:09:58.326553 cyto-dl-0.1.4/configs/experiment/private/npm1_equiv_3d_vae_3dnucalign.yaml
--rw-r--r--   0        0        0     2825 2024-03-09 00:09:58.326553 cyto-dl-0.1.4/configs/experiment/private/npm1_scale_inv_canon_so3.yaml
--rw-r--r--   0        0        0     2568 2024-03-09 00:09:58.330554 cyto-dl-0.1.4/configs/experiment/private/npm1_so2.yaml
--rw-r--r--   0        0        0     3062 2024-03-09 00:09:58.330554 cyto-dl-0.1.4/configs/experiment/private/npm1_so2_scale_inv.yaml
--rw-r--r--   0        0        0     3057 2024-03-09 00:09:58.330554 cyto-dl-0.1.4/configs/experiment/private/npm1_so3_scale_inv.yaml
--rw-r--r--   0        0        0     2325 2024-03-09 00:09:58.330554 cyto-dl-0.1.4/configs/experiment/private/npm1_so3_vae.yaml
--rw-r--r--   0        0        0     2179 2024-03-09 00:09:58.330554 cyto-dl-0.1.4/configs/experiment/private/npm1_so3_vae_seg.yaml
--rw-r--r--   0        0        0      967 2024-03-09 00:09:58.330554 cyto-dl-0.1.4/configs/experiment/private/variance_classical_2d_vae.yaml
--rw-r--r--   0        0        0     1053 2024-03-09 00:09:58.330554 cyto-dl-0.1.4/configs/experiment/private/variance_classical_3d_vae.yaml
--rw-r--r--   0        0        0     1385 2024-03-09 00:09:58.330554 cyto-dl-0.1.4/configs/experiment/private/variance_so2_3d_vae.yaml
--rw-r--r--   0        0        0     1605 2024-03-09 00:09:58.330554 cyto-dl-0.1.4/configs/experiment/private/variance_so2_3d_vae_profiling.yaml
--rw-r--r--   0        0        0     9822 2024-03-09 00:09:58.330554 cyto-dl-0.1.4/configs/experiment/private/variance_spharm.yaml
--rw-r--r--   0        0        0     9728 2024-03-09 00:09:58.330554 cyto-dl-0.1.4/configs/experiment/private/variance_spharm_o2.yaml
--rw-r--r--   0        0        0      309 2024-03-09 00:09:58.330554 cyto-dl-0.1.4/configs/extras/default.yaml
--rw-r--r--   0        0        0     1818 2024-03-09 00:09:58.330554 cyto-dl-0.1.4/configs/hparams_search/mnist_optuna.yaml
--rw-r--r--   0        0        0      431 2024-03-09 00:09:58.330554 cyto-dl-0.1.4/configs/hydra/default.yaml
--rw-r--r--   0        0        0      372 2024-03-09 00:09:58.330554 cyto-dl-0.1.4/configs/logger/comet.yaml
--rw-r--r--   0        0        0      157 2024-03-09 00:09:58.330554 cyto-dl-0.1.4/configs/logger/csv.yaml
--rw-r--r--   0        0        0      148 2024-03-09 00:09:58.330554 cyto-dl-0.1.4/configs/logger/many_loggers.yaml
--rw-r--r--   0        0        0      166 2024-03-09 00:09:58.330554 cyto-dl-0.1.4/configs/logger/mlflow.yaml
--rw-r--r--   0        0        0      277 2024-03-09 00:09:58.330554 cyto-dl-0.1.4/configs/logger/neptune.yaml
--rw-r--r--   0        0        0      258 2024-03-09 00:09:58.330554 cyto-dl-0.1.4/configs/logger/tensorboard.yaml
--rw-r--r--   0        0        0      522 2024-03-09 00:09:58.330554 cyto-dl-0.1.4/configs/logger/wandb.yaml
--rw-r--r--   0        0        0      594 2024-03-09 00:09:58.330554 cyto-dl-0.1.4/configs/model/classification/single_timepoint.yaml
--rw-r--r--   0        0        0     1807 2024-03-09 00:09:58.330554 cyto-dl-0.1.4/configs/model/im2im/gan.yaml
--rw-r--r--   0        0        0     1948 2024-03-09 00:09:58.330554 cyto-dl-0.1.4/configs/model/im2im/gan_superres.yaml
--rw-r--r--   0        0        0     1333 2024-03-09 00:09:58.330554 cyto-dl-0.1.4/configs/model/im2im/instance_seg.yaml
--rw-r--r--   0        0        0     1237 2024-03-09 00:09:58.330554 cyto-dl-0.1.4/configs/model/im2im/labelfree.yaml
--rw-r--r--   0        0        0     1245 2024-03-09 00:09:58.330554 cyto-dl-0.1.4/configs/model/im2im/mae.yaml
--rw-r--r--   0        0        0     1333 2024-03-09 00:09:58.330554 cyto-dl-0.1.4/configs/model/im2im/segmentation.yaml
--rw-r--r--   0        0        0     1246 2024-03-09 00:09:58.330554 cyto-dl-0.1.4/configs/model/im2im/segmentation_plugin.yaml
--rw-r--r--   0        0        0     1472 2024-03-09 00:09:58.330554 cyto-dl-0.1.4/configs/model/im2im/segmentation_superres.yaml
--rw-r--r--   0        0        0     1365 2024-03-09 00:09:58.330554 cyto-dl-0.1.4/configs/model/im2im/vit_segmentation_decoder.yaml
--rw-r--r--   0        0        0      493 2024-03-09 00:09:58.330554 cyto-dl-0.1.4/configs/model/private/classical_image_ae.yaml
--rw-r--r--   0        0        0      536 2024-03-09 00:09:58.330554 cyto-dl-0.1.4/configs/model/private/classical_image_vae.yaml
--rw-r--r--   0        0        0       86 2024-03-09 00:09:58.330554 cyto-dl-0.1.4/configs/model/private/reconstruction_loss/spharm_gaussian.yaml
--rw-r--r--   0        0        0       76 2024-03-09 00:09:58.330554 cyto-dl-0.1.4/configs/model/private/reconstruction_loss/spharm_loss.yaml
--rw-r--r--   0        0        0       56 2024-03-09 00:09:58.330554 cyto-dl-0.1.4/configs/model/private/reconstruction_loss/spharm_mse.yaml
--rw-r--r--   0        0        0       93 2024-03-09 00:09:58.330554 cyto-dl-0.1.4/configs/model/private/reconstruction_loss/spharm_weighted_mse.yaml
--rw-r--r--   0        0        0      316 2024-03-09 00:09:58.330554 cyto-dl-0.1.4/configs/model/private/so3_canon_image_vae.yaml
--rw-r--r--   0        0        0      332 2024-03-09 00:09:58.330554 cyto-dl-0.1.4/configs/model/private/so3_equiv_image_vae.yaml
--rw-r--r--   0        0        0      513 2024-03-09 00:09:58.330554 cyto-dl-0.1.4/configs/model/private/spharm.yaml
--rw-r--r--   0        0        0      501 2024-03-09 00:09:58.330554 cyto-dl-0.1.4/configs/model/private/spharm_so2.yaml
--rw-r--r--   0        0        0      597 2024-03-09 00:09:58.330554 cyto-dl-0.1.4/configs/model/test/base.yaml
--rw-r--r--   0        0        0      613 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/configs/model/test/simple_segmentation.yaml
--rw-r--r--   0        0        0      492 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/configs/paths/default.yaml
--rw-r--r--   0        0        0     1745 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/configs/train.yaml
--rw-r--r--   0        0        0       56 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/configs/trainer/cpu.yaml
--rw-r--r--   0        0        0      394 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/configs/trainer/ddp.yaml
--rw-r--r--   0        0        0      120 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/configs/trainer/ddp_sim.yaml
--rw-r--r--   0        0        0      468 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/configs/trainer/default.yaml
--rw-r--r--   0        0        0       55 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/configs/trainer/gpu.yaml
--rw-r--r--   0        0        0       56 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/configs/trainer/mps.yaml
--rw-r--r--   0        0        0      410 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/cyto_dl/__init__.py
--rw-r--r--   0        0        0       31 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/cyto_dl/api/__init__.py
--rw-r--r--   0        0        0     3707 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/cyto_dl/api/model.py
--rw-r--r--   0        0        0      265 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/cyto_dl/callbacks/__init__.py
--rw-r--r--   0        0        0     6605 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/cyto_dl/callbacks/callback_utils.py
--rw-r--r--   0        0        0    11849 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/cyto_dl/callbacks/latent_walk.py
--rw-r--r--   0        0        0     1918 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/cyto_dl/callbacks/layer_freeze.py
--rw-r--r--   0        0        0     4613 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/cyto_dl/callbacks/model_utils.py
--rw-r--r--   0        0        0     6687 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/cyto_dl/callbacks/outlier_detection.py
--rw-r--r--   0        0        0     3846 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/cyto_dl/compile.py
--rw-r--r--   0        0        0      238 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/cyto_dl/dataframe/__init__.py
--rw-r--r--   0        0        0     8481 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/cyto_dl/dataframe/readers.py
--rw-r--r--   0        0        0      251 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/cyto_dl/dataframe/transforms/__init__.py
--rw-r--r--   0        0        0     4519 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/cyto_dl/dataframe/transforms/filter.py
--rw-r--r--   0        0        0     2931 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/cyto_dl/dataframe/transforms/group_cols.py
--rw-r--r--   0        0        0     2441 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/cyto_dl/dataframe/transforms/misc.py
--rw-r--r--   0        0        0     3376 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/cyto_dl/dataframe/transforms/split.py
--rw-r--r--   0        0        0       86 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/cyto_dl/datamodules/__init__.py
--rw-r--r--   0        0        0     8679 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/cyto_dl/datamodules/czi.py
--rw-r--r--   0        0        0     1837 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/cyto_dl/datamodules/data_dict.py
--rw-r--r--   0        0        0      123 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/cyto_dl/datamodules/dataframe/__init__.py
--rw-r--r--   0        0        0     7058 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/cyto_dl/datamodules/dataframe/dataframe_datamodule.py
--rw-r--r--   0        0        0     4664 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/cyto_dl/datamodules/dataframe/grouped_dataframe_datamodule.py
--rw-r--r--   0        0        0    10538 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/cyto_dl/datamodules/dataframe/utils.py
--rw-r--r--   0        0        0     2885 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/cyto_dl/datamodules/folder.py
--rw-r--r--   0        0        0     7051 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/cyto_dl/datamodules/smartcache.py
--rw-r--r--   0        0        0     2296 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/cyto_dl/datamodules/torchvision.py
--rw-r--r--   0        0        0     3442 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/cyto_dl/eval.py
--rw-r--r--   0        0        0      200 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/cyto_dl/image/__init__.py
--rw-r--r--   0        0        0      213 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/cyto_dl/image/io/__init__.py
--rw-r--r--   0        0        0     2179 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/cyto_dl/image/io/aicsimage_loader.py
--rw-r--r--   0        0        0     1395 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/cyto_dl/image/io/monai_bio_reader.py
--rw-r--r--   0        0        0     1707 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/cyto_dl/image/io/numpy_reader.py
--rw-r--r--   0        0        0     1885 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/cyto_dl/image/io/ome_zarr_reader.py
--rw-r--r--   0        0        0     2464 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/cyto_dl/image/io/polygon_loader.py
--rw-r--r--   0        0        0     1498 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/cyto_dl/image/io/skimage_reader.py
--rw-r--r--   0        0        0      624 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/cyto_dl/image/transforms/__init__.py
--rw-r--r--   0        0        0     1214 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/cyto_dl/image/transforms/bright_sampler.py
--rw-r--r--   0        0        0     2468 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/cyto_dl/image/transforms/clip.py
--rw-r--r--   0        0        0     2247 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/cyto_dl/image/transforms/contrastadjust.py
--rw-r--r--   0        0        0     2173 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/cyto_dl/image/transforms/merge.py
--rw-r--r--   0        0        0     6320 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/cyto_dl/image/transforms/multiscale_cropper.py
--rw-r--r--   0        0        0     2365 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/cyto_dl/image/transforms/pad.py
--rw-r--r--   0        0        0     1355 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/cyto_dl/image/transforms/project.py
--rw-r--r--   0        0        0     3460 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/cyto_dl/image/transforms/rotation_mask_transform.py
--rw-r--r--   0        0        0     1861 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/cyto_dl/image/transforms/save.py
--rw-r--r--   0        0        0     1418 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/cyto_dl/image/transforms/so2_random_rotation.py
--rw-r--r--   0        0        0     4975 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/cyto_dl/image/transforms/track_transforms.py
--rw-r--r--   0        0        0       33 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/cyto_dl/loggers/__init__.py
--rw-r--r--   0        0        0     6183 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/cyto_dl/loggers/mlflow.py
--rw-r--r--   0        0        0        0 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/cyto_dl/models/__init__.py
--rw-r--r--   0        0        0     7267 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/cyto_dl/models/base_model.py
--rw-r--r--   0        0        0     3298 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/cyto_dl/models/basic_model.py
--rw-r--r--   0        0        0      105 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/cyto_dl/models/classification/__init__.py
--rw-r--r--   0        0        0     4454 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/cyto_dl/models/classification/classification.py
--rw-r--r--   0        0        0     3047 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/cyto_dl/models/classification/timepoint_classification.py
--rw-r--r--   0        0        0       38 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/cyto_dl/models/handlers/__init__.py
--rw-r--r--   0        0        0     2832 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/cyto_dl/models/handlers/base_handler.py
--rw-r--r--   0        0        0     1133 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/cyto_dl/models/handlers/image_handler.py
--rw-r--r--   0        0        0     1139 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/cyto_dl/models/handlers/load_image_patch.py
--rw-r--r--   0        0        0       60 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/cyto_dl/models/im2im/__init__.py
--rw-r--r--   0        0        0     6319 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/cyto_dl/models/im2im/gan.py
--rw-r--r--   0        0        0     8426 2024-03-09 00:09:58.334554 cyto-dl-0.1.4/cyto_dl/models/im2im/multi_task.py
--rw-r--r--   0        0        0      324 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/models/im2im/utils/__init__.py
--rw-r--r--   0        0        0    21568 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/models/im2im/utils/instance_seg.py
--rw-r--r--   0        0        0     1531 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/models/im2im/utils/noise_annealer.py
--rw-r--r--   0        0        0      125 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/models/im2im/utils/postprocessing/__init__.py
--rw-r--r--   0        0        0     2410 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/models/im2im/utils/postprocessing/act_thresh_label.py
--rw-r--r--   0        0        0      835 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/models/im2im/utils/postprocessing/auto_thresh.py
--rw-r--r--   0        0        0     1287 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/models/im2im/utils/postprocessing/dict_to_im.py
--rw-r--r--   0        0        0       32 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/models/utils/__init__.py
--rw-r--r--   0        0        0     1264 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/models/utils/mlflow.py
--rw-r--r--   0        0        0      268 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/models/utils/utils.py
--rw-r--r--   0        0        0      284 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/models/vae/__init__.py
--rw-r--r--   0        0        0    10624 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/models/vae/base_vae.py
--rw-r--r--   0        0        0    10648 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/models/vae/image_canon_vae.py
--rw-r--r--   0        0        0    11242 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/models/vae/image_encoder.py
--rw-r--r--   0        0        0     8223 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/models/vae/image_vae.py
--rw-r--r--   0        0        0     9890 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/models/vae/latent_loss_vae.py
--rw-r--r--   0        0        0       39 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/models/vae/o2_spharm_vae/__init__.py
--rw-r--r--   0        0        0     3653 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/models/vae/o2_spharm_vae/o2_spharm_encoder.py
--rw-r--r--   0        0        0     4323 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/models/vae/o2_spharm_vae/o2_spharm_vae.py
--rw-r--r--   0        0        0    11244 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/models/vae/point_cloud_vae.py
--rw-r--r--   0        0        0      144 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/models/vae/priors/__init__.py
--rw-r--r--   0        0        0      574 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/models/vae/priors/abstract_prior.py
--rw-r--r--   0        0        0     5530 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/models/vae/priors/gaussian.py
--rw-r--r--   0        0        0      408 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/models/vae/priors/identity_prior.py
--rw-r--r--   0        0        0     1609 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/models/vae/priors/joint_prior.py
--rw-r--r--   0        0        0     1280 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/models/vae/tabular_vae.py
--rw-r--r--   0        0        0      305 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/nn/__init__.py
--rw-r--r--   0        0        0      118 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/nn/discriminators/__init__.py
--rw-r--r--   0        0        0     1695 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/nn/discriminators/multi_scale_discriminator.py
--rw-r--r--   0        0        0     3816 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/nn/discriminators/n_layer_discriminator.py
--rw-r--r--   0        0        0      151 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/nn/head/__init__.py
--rw-r--r--   0        0        0     3802 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/nn/head/base_head.py
--rw-r--r--   0        0        0     3115 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/nn/head/gan_head.py
--rw-r--r--   0        0        0     2850 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/nn/head/gan_head_superres.py
--rw-r--r--   0        0        0      928 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/nn/head/mae_head.py
--rw-r--r--   0        0        0     2033 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/nn/head/mask_head.py
--rw-r--r--   0        0        0     4415 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/nn/head/res_blocks_head.py
--rw-r--r--   0        0        0     1042 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/nn/hr_skip.py
--rw-r--r--   0        0        0      592 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/nn/losses/__init__.py
--rw-r--r--   0        0        0     1071 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/nn/losses/adversarial_loss.py
--rw-r--r--   0        0        0     1119 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/nn/losses/chamfer_loss.py
--rw-r--r--   0        0        0     1046 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/nn/losses/continuous_bernoulli.py
--rw-r--r--   0        0        0      671 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/nn/losses/cosine_loss.py
--rw-r--r--   0        0        0     4431 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/nn/losses/gan_loss.py
--rw-r--r--   0        0        0      917 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/nn/losses/gaussian_nll_loss.py
--rw-r--r--   0        0        0      873 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/nn/losses/geomloss.py
--rw-r--r--   0        0        0     2155 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/nn/losses/loss_wrapper.py
--rw-r--r--   0        0        0     1015 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/nn/losses/spharm_loss.py
--rw-r--r--   0        0        0      895 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/nn/losses/threshold_loss.py
--rw-r--r--   0        0        0     1105 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/nn/losses/weibull.py
--rw-r--r--   0        0        0      675 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/nn/losses/weighted_mse_loss.py
--rw-r--r--   0        0        0      958 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/nn/mlp.py
--rw-r--r--   0        0        0       61 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/nn/point_cloud/__init__.py
--rw-r--r--   0        0        0    13372 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/nn/point_cloud/dgcnn.py
--rw-r--r--   0        0        0     2732 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/nn/point_cloud/folding_net.py
--rw-r--r--   0        0        0     4934 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/nn/point_cloud/graph_functions.py
--rw-r--r--   0        0        0     5754 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/nn/point_cloud/vnn.py
--rw-r--r--   0        0        0     6848 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/nn/res_unit.py
--rw-r--r--   0        0        0     2555 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/nn/spatial_transformer.py
--rw-r--r--   0        0        0     2571 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/nn/track_sequence_predictor.py
--rw-r--r--   0        0        0      133 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/nn/vits/__init__.py
--rw-r--r--   0        0        0       86 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/nn/vits/blocks/__init__.py
--rw-r--r--   0        0        0     4427 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/nn/vits/blocks/cross_attention.py
--rw-r--r--   0        0        0     5502 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/nn/vits/cross_mae.py
--rw-r--r--   0        0        0    14181 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/nn/vits/mae.py
--rw-r--r--   0        0        0     8323 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/nn/vits/seg.py
--rw-r--r--   0        0        0        0 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/point_cloud/__init__.py
--rw-r--r--   0        0        0       40 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/point_cloud/io/__init__.py
--rw-r--r--   0        0        0     4992 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/point_cloud/io/read_pcloud.py
--rw-r--r--   0        0        0     5355 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/train.py
--rw-r--r--   0        0        0      333 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/utils/__init__.py
--rw-r--r--   0        0        0     1791 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/utils/config.py
--rw-r--r--   0        0        0     2391 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/utils/download_test_data.py
--rw-r--r--   0        0        0     2359 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/utils/dummy_dataset.py
--rw-r--r--   0        0        0      671 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/utils/pylogger.py
--rw-r--r--   0        0        0     3326 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/utils/rich_utils.py
--rw-r--r--   0        0        0     3808 2024-03-09 00:09:58.338554 cyto-dl-0.1.4/cyto_dl/utils/rotation.py
--rw-r--r--   0        0        0      237 2024-03-09 00:09:58.342554 cyto-dl-0.1.4/cyto_dl/utils/spharm/__init__.py
--rw-r--r--   0        0        0     6015 2024-03-09 00:09:58.342554 cyto-dl-0.1.4/cyto_dl/utils/spharm/reconstruction.py
--rw-r--r--   0        0        0     4360 2024-03-09 00:09:58.342554 cyto-dl-0.1.4/cyto_dl/utils/spharm/rotation.py
--rw-r--r--   0        0        0     7103 2024-03-09 00:09:58.342554 cyto-dl-0.1.4/cyto_dl/utils/template_utils.py
--rw-r--r--   0        0        0     2897 2024-03-09 00:09:58.342554 cyto-dl-0.1.4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-09 00:09:58.346554 cyto-dl-0.1.4/tests/__init__.py
--rw-r--r--   0        0        0     3599 2024-03-09 00:09:58.346554 cyto-dl-0.1.4/tests/conftest.py
--rw-r--r--   0        0        0        0 2024-03-09 00:09:58.346554 cyto-dl-0.1.4/tests/helpers/__init__.py
--rw-r--r--   0        0        0      857 2024-03-09 00:09:58.346554 cyto-dl-0.1.4/tests/helpers/package_available.py
--rw-r--r--   0        0        0     4307 2024-03-09 00:09:58.346554 cyto-dl-0.1.4/tests/helpers/run_if.py
--rw-r--r--   0        0        0   259123 2024-03-09 00:09:58.346554 cyto-dl-0.1.4/tests/resources/rand_im.tif
--rw-r--r--   0        0        0      336 2024-03-09 00:09:58.346554 cyto-dl-0.1.4/tests/resources/test.csv
--rw-r--r--   0        0        0      635 2024-03-09 00:09:58.346554 cyto-dl-0.1.4/tests/resources/train.csv
--rw-r--r--   0        0        0      336 2024-03-09 00:09:58.346554 cyto-dl-0.1.4/tests/resources/valid.csv
--rw-r--r--   0        0        0     2675 2024-03-09 00:09:58.346554 cyto-dl-0.1.4/tests/test_alternating_batch_sampler.py
--rw-r--r--   0        0        0     1434 2024-03-09 00:09:58.346554 cyto-dl-0.1.4/tests/test_configs.py
--rw-r--r--   0        0        0     1604 2024-03-09 00:09:58.346554 cyto-dl-0.1.4/tests/test_eval.py
--rw-r--r--   0        0        0     3730 2024-03-09 00:09:58.346554 cyto-dl-0.1.4/tests/test_mlflow_logger.py
--rw-r--r--   0        0        0     1119 2024-03-09 00:09:58.346554 cyto-dl-0.1.4/tests/test_polygon_loader.py
--rw-r--r--   0        0        0     2243 2024-03-09 00:09:58.346554 cyto-dl-0.1.4/tests/test_train.py
--rw-r--r--   0        0        0      143 2024-03-09 00:09:58.346554 cyto-dl-0.1.4/tests/utils.py
--rw-r--r--   0        0        0     6142 1970-01-01 00:00:00.000000 cyto-dl-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     5431 2024-04-01 23:14:18.092902 cyto-dl-0.1.5/README.md
+-rw-r--r--   0        0        0      403 2024-04-01 23:14:18.092902 cyto-dl-0.1.5/configs/callbacks/default.yaml
+-rw-r--r--   0        0        0     1250 2024-04-01 23:14:18.092902 cyto-dl-0.1.5/configs/callbacks/early_stopping.yaml
+-rw-r--r--   0        0        0       80 2024-04-01 23:14:18.092902 cyto-dl-0.1.5/configs/callbacks/layer_freeze.yaml
+-rw-r--r--   0        0        0       83 2024-04-01 23:14:18.092902 cyto-dl-0.1.5/configs/callbacks/learning_rate_monitor.yaml
+-rw-r--r--   0        0        0     1298 2024-04-01 23:14:18.092902 cyto-dl-0.1.5/configs/callbacks/model_checkpoint.yaml
+-rw-r--r--   0        0        0      402 2024-04-01 23:14:18.092902 cyto-dl-0.1.5/configs/callbacks/model_summary.yaml
+-rw-r--r--   0        0        0        0 2024-04-01 23:14:18.092902 cyto-dl-0.1.5/configs/callbacks/none.yaml
+-rw-r--r--   0        0        0      160 2024-04-01 23:14:18.092902 cyto-dl-0.1.5/configs/callbacks/outlier_detection.yaml
+-rw-r--r--   0        0        0      289 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/callbacks/rich_progress_bar.yaml
+-rw-r--r--   0        0        0      758 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/compile.yaml
+-rw-r--r--   0        0        0     2634 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/data/classification/single_timepoint.yaml
+-rw-r--r--   0        0        0     7077 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/data/im2im/gan.yaml
+-rw-r--r--   0        0        0     7427 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/data/im2im/gan_superres.yaml
+-rw-r--r--   0        0        0     6880 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/data/im2im/instance_seg.yaml
+-rw-r--r--   0        0        0     5879 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/data/im2im/labelfree.yaml
+-rw-r--r--   0        0        0     4374 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/data/im2im/mae.yaml
+-rw-r--r--   0        0        0     6852 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/data/im2im/segmentation.yaml
+-rw-r--r--   0        0        0     8222 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/data/im2im/segmentation_plugin.yaml
+-rw-r--r--   0        0        0     7263 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/data/im2im/segmentation_superres.yaml
+-rw-r--r--   0        0        0      450 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/data/private/lattice_nuc_sdf.yaml
+-rw-r--r--   0        0        0      416 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/data/private/rot_mnist.yaml
+-rw-r--r--   0        0        0      450 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/data/private/rot_mnist_vae.yaml
+-rw-r--r--   0        0        0     1176 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/data/private/rotated_mnist.yaml
+-rw-r--r--   0        0        0     1075 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/data/private/variance_3d.yaml
+-rw-r--r--   0        0        0      497 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/data/private/variance_3d_npm1.yaml
+-rw-r--r--   0        0        0      770 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/data/private/variance_3d_npm_nuc_v2.yaml
+-rw-r--r--   0        0        0     1802 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/data/private/variance_3d_rotate.yaml
+-rw-r--r--   0        0        0      547 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/data/private/variance_centerslice.yaml
+-rw-r--r--   0        0        0      719 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/data/private/variance_centerslice_resize.yaml
+-rw-r--r--   0        0        0      969 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/data/private/variance_npm1.yaml
+-rw-r--r--   0        0        0      312 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/data/private/variance_spharm.yaml
+-rw-r--r--   0        0        0      462 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/data/test/alternating_batch.yaml
+-rw-r--r--   0        0        0      200 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/data/test/omnipose.yaml
+-rw-r--r--   0        0        0      200 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/data/test/segmentation.yaml
+-rw-r--r--   0        0        0      899 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/debug/default.yaml
+-rw-r--r--   0        0        0      125 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/debug/fdr.yaml
+-rw-r--r--   0        0        0      223 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/debug/limit.yaml
+-rw-r--r--   0        0        0      209 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/debug/overfit.yaml
+-rw-r--r--   0        0        0      182 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/debug/profiler.yaml
+-rw-r--r--   0        0        0      509 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/eval.yaml
+-rw-r--r--   0        0        0      659 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/experiment/classification/per_timepoint.yaml
+-rw-r--r--   0        0        0     1065 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/experiment/im2im/gan.yaml
+-rw-r--r--   0        0        0     1083 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/experiment/im2im/gan_superres.yaml
+-rw-r--r--   0        0        0      932 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/experiment/im2im/instance_seg.yaml
+-rw-r--r--   0        0        0      854 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/experiment/im2im/labelfree.yaml
+-rw-r--r--   0        0        0      892 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/experiment/im2im/mae.yaml
+-rw-r--r--   0        0        0      863 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/experiment/im2im/segmentation.yaml
+-rw-r--r--   0        0        0     1126 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/experiment/im2im/segmentation_plugin.yaml
+-rw-r--r--   0        0        0      881 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/experiment/im2im/segmentation_superres.yaml
+-rw-r--r--   0        0        0     1098 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/experiment/im2im/vit_segmentation.yaml
+-rw-r--r--   0        0        0     2741 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/experiment/private/lattice_nuc_sdf.yaml
+-rw-r--r--   0        0        0     1583 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/experiment/private/mnist_so2.yaml
+-rw-r--r--   0        0        0      989 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/experiment/private/npm1_classical_3d_vae.yaml
+-rw-r--r--   0        0        0     2902 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/experiment/private/npm1_classical_scale_inv.yaml
+-rw-r--r--   0        0        0     1037 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/experiment/private/npm1_equiv_3d_vae_3dnucalign.yaml
+-rw-r--r--   0        0        0     2825 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/experiment/private/npm1_scale_inv_canon_so3.yaml
+-rw-r--r--   0        0        0     2568 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/experiment/private/npm1_so2.yaml
+-rw-r--r--   0        0        0     3062 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/experiment/private/npm1_so2_scale_inv.yaml
+-rw-r--r--   0        0        0     3057 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/experiment/private/npm1_so3_scale_inv.yaml
+-rw-r--r--   0        0        0     2325 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/experiment/private/npm1_so3_vae.yaml
+-rw-r--r--   0        0        0     2179 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/experiment/private/npm1_so3_vae_seg.yaml
+-rw-r--r--   0        0        0      967 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/experiment/private/variance_classical_2d_vae.yaml
+-rw-r--r--   0        0        0     1053 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/experiment/private/variance_classical_3d_vae.yaml
+-rw-r--r--   0        0        0     1385 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/experiment/private/variance_so2_3d_vae.yaml
+-rw-r--r--   0        0        0     1605 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/experiment/private/variance_so2_3d_vae_profiling.yaml
+-rw-r--r--   0        0        0     9822 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/experiment/private/variance_spharm.yaml
+-rw-r--r--   0        0        0     9728 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/experiment/private/variance_spharm_o2.yaml
+-rw-r--r--   0        0        0      309 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/extras/default.yaml
+-rw-r--r--   0        0        0     1818 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/hparams_search/mnist_optuna.yaml
+-rw-r--r--   0        0        0      431 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/hydra/default.yaml
+-rw-r--r--   0        0        0      372 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/logger/comet.yaml
+-rw-r--r--   0        0        0      157 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/logger/csv.yaml
+-rw-r--r--   0        0        0      148 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/logger/many_loggers.yaml
+-rw-r--r--   0        0        0      166 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/logger/mlflow.yaml
+-rw-r--r--   0        0        0      277 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/logger/neptune.yaml
+-rw-r--r--   0        0        0      258 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/logger/tensorboard.yaml
+-rw-r--r--   0        0        0      522 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/logger/wandb.yaml
+-rw-r--r--   0        0        0      594 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/model/classification/single_timepoint.yaml
+-rw-r--r--   0        0        0     1807 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/model/im2im/gan.yaml
+-rw-r--r--   0        0        0     1948 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/model/im2im/gan_superres.yaml
+-rw-r--r--   0        0        0     1333 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/model/im2im/instance_seg.yaml
+-rw-r--r--   0        0        0     1237 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/model/im2im/labelfree.yaml
+-rw-r--r--   0        0        0     1245 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/model/im2im/mae.yaml
+-rw-r--r--   0        0        0     1333 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/model/im2im/segmentation.yaml
+-rw-r--r--   0        0        0     1246 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/model/im2im/segmentation_plugin.yaml
+-rw-r--r--   0        0        0     1472 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/model/im2im/segmentation_superres.yaml
+-rw-r--r--   0        0        0     1365 2024-04-01 23:14:18.096902 cyto-dl-0.1.5/configs/model/im2im/vit_segmentation_decoder.yaml
+-rw-r--r--   0        0        0      493 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/configs/model/private/classical_image_ae.yaml
+-rw-r--r--   0        0        0      536 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/configs/model/private/classical_image_vae.yaml
+-rw-r--r--   0        0        0       86 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/configs/model/private/reconstruction_loss/spharm_gaussian.yaml
+-rw-r--r--   0        0        0       76 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/configs/model/private/reconstruction_loss/spharm_loss.yaml
+-rw-r--r--   0        0        0       56 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/configs/model/private/reconstruction_loss/spharm_mse.yaml
+-rw-r--r--   0        0        0       93 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/configs/model/private/reconstruction_loss/spharm_weighted_mse.yaml
+-rw-r--r--   0        0        0      316 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/configs/model/private/so3_canon_image_vae.yaml
+-rw-r--r--   0        0        0      332 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/configs/model/private/so3_equiv_image_vae.yaml
+-rw-r--r--   0        0        0      513 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/configs/model/private/spharm.yaml
+-rw-r--r--   0        0        0      501 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/configs/model/private/spharm_so2.yaml
+-rw-r--r--   0        0        0      597 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/configs/model/test/base.yaml
+-rw-r--r--   0        0        0      613 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/configs/model/test/simple_segmentation.yaml
+-rw-r--r--   0        0        0      492 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/configs/paths/default.yaml
+-rw-r--r--   0        0        0     1745 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/configs/train.yaml
+-rw-r--r--   0        0        0       56 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/configs/trainer/cpu.yaml
+-rw-r--r--   0        0        0      394 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/configs/trainer/ddp.yaml
+-rw-r--r--   0        0        0      120 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/configs/trainer/ddp_sim.yaml
+-rw-r--r--   0        0        0      468 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/configs/trainer/default.yaml
+-rw-r--r--   0        0        0       55 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/configs/trainer/gpu.yaml
+-rw-r--r--   0        0        0       56 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/configs/trainer/mps.yaml
+-rw-r--r--   0        0        0      410 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/__init__.py
+-rw-r--r--   0        0        0       31 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/api/__init__.py
+-rw-r--r--   0        0        0     1040 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/api/data.py
+-rw-r--r--   0        0        0     3809 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/api/model.py
+-rw-r--r--   0        0        0      265 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/callbacks/__init__.py
+-rw-r--r--   0        0        0     6605 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/callbacks/callback_utils.py
+-rw-r--r--   0        0        0    11849 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/callbacks/latent_walk.py
+-rw-r--r--   0        0        0     1918 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/callbacks/layer_freeze.py
+-rw-r--r--   0        0        0     4613 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/callbacks/model_utils.py
+-rw-r--r--   0        0        0     6687 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/callbacks/outlier_detection.py
+-rw-r--r--   0        0        0     3846 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/compile.py
+-rw-r--r--   0        0        0      238 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/dataframe/__init__.py
+-rw-r--r--   0        0        0     8481 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/dataframe/readers.py
+-rw-r--r--   0        0        0      251 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/dataframe/transforms/__init__.py
+-rw-r--r--   0        0        0     4519 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/dataframe/transforms/filter.py
+-rw-r--r--   0        0        0     2931 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/dataframe/transforms/group_cols.py
+-rw-r--r--   0        0        0     2441 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/dataframe/transforms/misc.py
+-rw-r--r--   0        0        0     3376 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/dataframe/transforms/split.py
+-rw-r--r--   0        0        0       86 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/datamodules/__init__.py
+-rw-r--r--   0        0        0     9014 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/datamodules/czi.py
+-rw-r--r--   0        0        0     1837 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/datamodules/data_dict.py
+-rw-r--r--   0        0        0      123 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/datamodules/dataframe/__init__.py
+-rw-r--r--   0        0        0     7500 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/datamodules/dataframe/dataframe_datamodule.py
+-rw-r--r--   0        0        0     4856 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/datamodules/dataframe/grouped_dataframe_datamodule.py
+-rw-r--r--   0        0        0    11941 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/datamodules/dataframe/utils.py
+-rw-r--r--   0        0        0     2885 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/datamodules/folder.py
+-rw-r--r--   0        0        0     8044 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/datamodules/smartcache.py
+-rw-r--r--   0        0        0     2296 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/datamodules/torchvision.py
+-rw-r--r--   0        0        0     3442 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/eval.py
+-rw-r--r--   0        0        0      200 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/image/__init__.py
+-rw-r--r--   0        0        0      213 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/image/io/__init__.py
+-rw-r--r--   0        0        0     2630 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/image/io/aicsimage_loader.py
+-rw-r--r--   0        0        0     1908 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/image/io/monai_bio_reader.py
+-rw-r--r--   0        0        0     1707 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/image/io/numpy_reader.py
+-rw-r--r--   0        0        0     1885 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/image/io/ome_zarr_reader.py
+-rw-r--r--   0        0        0     2464 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/image/io/polygon_loader.py
+-rw-r--r--   0        0        0     1498 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/image/io/skimage_reader.py
+-rw-r--r--   0        0        0      624 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/image/transforms/__init__.py
+-rw-r--r--   0        0        0     1214 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/image/transforms/bright_sampler.py
+-rw-r--r--   0        0        0     2468 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/image/transforms/clip.py
+-rw-r--r--   0        0        0     2247 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/image/transforms/contrastadjust.py
+-rw-r--r--   0        0        0     2173 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/image/transforms/merge.py
+-rw-r--r--   0        0        0     6376 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/image/transforms/multiscale_cropper.py
+-rw-r--r--   0        0        0     2365 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/image/transforms/pad.py
+-rw-r--r--   0        0        0     1355 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/image/transforms/project.py
+-rw-r--r--   0        0        0     3460 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/image/transforms/rotation_mask_transform.py
+-rw-r--r--   0        0        0     1861 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/image/transforms/save.py
+-rw-r--r--   0        0        0     1418 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/image/transforms/so2_random_rotation.py
+-rw-r--r--   0        0        0     4975 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/image/transforms/track_transforms.py
+-rw-r--r--   0        0        0       33 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/loggers/__init__.py
+-rw-r--r--   0        0        0     6183 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/loggers/mlflow.py
+-rw-r--r--   0        0        0        0 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/models/__init__.py
+-rw-r--r--   0        0        0     7267 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/models/base_model.py
+-rw-r--r--   0        0        0     3298 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/models/basic_model.py
+-rw-r--r--   0        0        0      105 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/models/classification/__init__.py
+-rw-r--r--   0        0        0     4454 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/models/classification/classification.py
+-rw-r--r--   0        0        0     3047 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/models/classification/timepoint_classification.py
+-rw-r--r--   0        0        0       38 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/models/handlers/__init__.py
+-rw-r--r--   0        0        0     2832 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/models/handlers/base_handler.py
+-rw-r--r--   0        0        0     1133 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/models/handlers/image_handler.py
+-rw-r--r--   0        0        0     1139 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/models/handlers/load_image_patch.py
+-rw-r--r--   0        0        0       60 2024-04-01 23:14:18.100902 cyto-dl-0.1.5/cyto_dl/models/im2im/__init__.py
+-rw-r--r--   0        0        0     6319 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/models/im2im/gan.py
+-rw-r--r--   0        0        0     8946 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/models/im2im/multi_task.py
+-rw-r--r--   0        0        0      324 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/models/im2im/utils/__init__.py
+-rw-r--r--   0        0        0    21568 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/models/im2im/utils/instance_seg.py
+-rw-r--r--   0        0        0     1531 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/models/im2im/utils/noise_annealer.py
+-rw-r--r--   0        0        0      125 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/models/im2im/utils/postprocessing/__init__.py
+-rw-r--r--   0        0        0     2410 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/models/im2im/utils/postprocessing/act_thresh_label.py
+-rw-r--r--   0        0        0      835 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/models/im2im/utils/postprocessing/auto_thresh.py
+-rw-r--r--   0        0        0     1287 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/models/im2im/utils/postprocessing/dict_to_im.py
+-rw-r--r--   0        0        0       32 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/models/utils/__init__.py
+-rw-r--r--   0        0        0     1264 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/models/utils/mlflow.py
+-rw-r--r--   0        0        0      268 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/models/utils/utils.py
+-rw-r--r--   0        0        0      284 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/models/vae/__init__.py
+-rw-r--r--   0        0        0    10624 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/models/vae/base_vae.py
+-rw-r--r--   0        0        0    10648 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/models/vae/image_canon_vae.py
+-rw-r--r--   0        0        0    11242 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/models/vae/image_encoder.py
+-rw-r--r--   0        0        0     8223 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/models/vae/image_vae.py
+-rw-r--r--   0        0        0     9890 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/models/vae/latent_loss_vae.py
+-rw-r--r--   0        0        0       39 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/models/vae/o2_spharm_vae/__init__.py
+-rw-r--r--   0        0        0     3653 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/models/vae/o2_spharm_vae/o2_spharm_encoder.py
+-rw-r--r--   0        0        0     4323 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/models/vae/o2_spharm_vae/o2_spharm_vae.py
+-rw-r--r--   0        0        0    11244 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/models/vae/point_cloud_vae.py
+-rw-r--r--   0        0        0      144 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/models/vae/priors/__init__.py
+-rw-r--r--   0        0        0      574 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/models/vae/priors/abstract_prior.py
+-rw-r--r--   0        0        0     5530 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/models/vae/priors/gaussian.py
+-rw-r--r--   0        0        0      408 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/models/vae/priors/identity_prior.py
+-rw-r--r--   0        0        0     1609 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/models/vae/priors/joint_prior.py
+-rw-r--r--   0        0        0     1280 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/models/vae/tabular_vae.py
+-rw-r--r--   0        0        0      305 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/__init__.py
+-rw-r--r--   0        0        0      118 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/discriminators/__init__.py
+-rw-r--r--   0        0        0     1695 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/discriminators/multi_scale_discriminator.py
+-rw-r--r--   0        0        0     3816 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/discriminators/n_layer_discriminator.py
+-rw-r--r--   0        0        0      151 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/head/__init__.py
+-rw-r--r--   0        0        0     3802 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/head/base_head.py
+-rw-r--r--   0        0        0     3115 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/head/gan_head.py
+-rw-r--r--   0        0        0     2850 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/head/gan_head_superres.py
+-rw-r--r--   0        0        0      928 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/head/mae_head.py
+-rw-r--r--   0        0        0     2033 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/head/mask_head.py
+-rw-r--r--   0        0        0     4415 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/head/res_blocks_head.py
+-rw-r--r--   0        0        0     1042 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/hr_skip.py
+-rw-r--r--   0        0        0      592 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/losses/__init__.py
+-rw-r--r--   0        0        0     1071 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/losses/adversarial_loss.py
+-rw-r--r--   0        0        0     1119 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/losses/chamfer_loss.py
+-rw-r--r--   0        0        0     1046 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/losses/continuous_bernoulli.py
+-rw-r--r--   0        0        0      671 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/losses/cosine_loss.py
+-rw-r--r--   0        0        0     4431 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/losses/gan_loss.py
+-rw-r--r--   0        0        0      917 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/losses/gaussian_nll_loss.py
+-rw-r--r--   0        0        0      873 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/losses/geomloss.py
+-rw-r--r--   0        0        0     2155 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/losses/loss_wrapper.py
+-rw-r--r--   0        0        0     1015 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/losses/spharm_loss.py
+-rw-r--r--   0        0        0      895 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/losses/threshold_loss.py
+-rw-r--r--   0        0        0     1105 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/losses/weibull.py
+-rw-r--r--   0        0        0      675 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/losses/weighted_mse_loss.py
+-rw-r--r--   0        0        0      958 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/mlp.py
+-rw-r--r--   0        0        0       61 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/point_cloud/__init__.py
+-rw-r--r--   0        0        0    13372 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/point_cloud/dgcnn.py
+-rw-r--r--   0        0        0     2732 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/point_cloud/folding_net.py
+-rw-r--r--   0        0        0     4934 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/point_cloud/graph_functions.py
+-rw-r--r--   0        0        0     5754 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/point_cloud/vnn.py
+-rw-r--r--   0        0        0     6848 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/res_unit.py
+-rw-r--r--   0        0        0     2555 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/spatial_transformer.py
+-rw-r--r--   0        0        0     2571 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/track_sequence_predictor.py
+-rw-r--r--   0        0        0      165 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/vits/__init__.py
+-rw-r--r--   0        0        0      171 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/vits/blocks/__init__.py
+-rw-r--r--   0        0        0     4427 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/vits/blocks/cross_attention.py
+-rw-r--r--   0        0        0      848 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/vits/blocks/intermediate_weigher.py
+-rw-r--r--   0        0        0     5249 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/vits/blocks/patchify.py
+-rw-r--r--   0        0        0     5577 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/vits/cross_mae.py
+-rw-r--r--   0        0        0    10645 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/vits/mae.py
+-rw-r--r--   0        0        0    10199 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/vits/seg.py
+-rw-r--r--   0        0        0      208 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/nn/vits/utils.py
+-rw-r--r--   0        0        0        0 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/point_cloud/__init__.py
+-rw-r--r--   0        0        0       40 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/point_cloud/io/__init__.py
+-rw-r--r--   0        0        0     4992 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/point_cloud/io/read_pcloud.py
+-rw-r--r--   0        0        0     5355 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/train.py
+-rw-r--r--   0        0        0      333 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/utils/__init__.py
+-rw-r--r--   0        0        0     1791 2024-04-01 23:14:18.104902 cyto-dl-0.1.5/cyto_dl/utils/config.py
+-rw-r--r--   0        0        0     2391 2024-04-01 23:14:18.108902 cyto-dl-0.1.5/cyto_dl/utils/download_test_data.py
+-rw-r--r--   0        0        0     2359 2024-04-01 23:14:18.108902 cyto-dl-0.1.5/cyto_dl/utils/dummy_dataset.py
+-rw-r--r--   0        0        0      671 2024-04-01 23:14:18.108902 cyto-dl-0.1.5/cyto_dl/utils/pylogger.py
+-rw-r--r--   0        0        0     3326 2024-04-01 23:14:18.108902 cyto-dl-0.1.5/cyto_dl/utils/rich_utils.py
+-rw-r--r--   0        0        0     3808 2024-04-01 23:14:18.108902 cyto-dl-0.1.5/cyto_dl/utils/rotation.py
+-rw-r--r--   0        0        0      237 2024-04-01 23:14:18.108902 cyto-dl-0.1.5/cyto_dl/utils/spharm/__init__.py
+-rw-r--r--   0        0        0     6015 2024-04-01 23:14:18.108902 cyto-dl-0.1.5/cyto_dl/utils/spharm/reconstruction.py
+-rw-r--r--   0        0        0     4360 2024-04-01 23:14:18.108902 cyto-dl-0.1.5/cyto_dl/utils/spharm/rotation.py
+-rw-r--r--   0        0        0     7103 2024-04-01 23:14:18.108902 cyto-dl-0.1.5/cyto_dl/utils/template_utils.py
+-rw-r--r--   0        0        0     2887 2024-04-01 23:14:18.108902 cyto-dl-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-01 23:14:18.112902 cyto-dl-0.1.5/tests/__init__.py
+-rw-r--r--   0        0        0      929 2024-04-01 23:14:18.112902 cyto-dl-0.1.5/tests/api/test_model.py
+-rw-r--r--   0        0        0     3599 2024-04-01 23:14:18.112902 cyto-dl-0.1.5/tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-01 23:14:18.112902 cyto-dl-0.1.5/tests/helpers/__init__.py
+-rw-r--r--   0        0        0      857 2024-04-01 23:14:18.112902 cyto-dl-0.1.5/tests/helpers/package_available.py
+-rw-r--r--   0        0        0     4307 2024-04-01 23:14:18.112902 cyto-dl-0.1.5/tests/helpers/run_if.py
+-rw-r--r--   0        0        0   259123 2024-04-01 23:14:18.112902 cyto-dl-0.1.5/tests/resources/rand_im.tif
+-rw-r--r--   0        0        0      336 2024-04-01 23:14:18.112902 cyto-dl-0.1.5/tests/resources/test.csv
+-rw-r--r--   0        0        0      635 2024-04-01 23:14:18.112902 cyto-dl-0.1.5/tests/resources/train.csv
+-rw-r--r--   0        0        0      336 2024-04-01 23:14:18.112902 cyto-dl-0.1.5/tests/resources/valid.csv
+-rw-r--r--   0        0        0     2675 2024-04-01 23:14:18.112902 cyto-dl-0.1.5/tests/test_alternating_batch_sampler.py
+-rw-r--r--   0        0        0     1434 2024-04-01 23:14:18.112902 cyto-dl-0.1.5/tests/test_configs.py
+-rw-r--r--   0        0        0     1604 2024-04-01 23:14:18.112902 cyto-dl-0.1.5/tests/test_eval.py
+-rw-r--r--   0        0        0     3730 2024-04-01 23:14:18.112902 cyto-dl-0.1.5/tests/test_mlflow_logger.py
+-rw-r--r--   0        0        0     1119 2024-04-01 23:14:18.112902 cyto-dl-0.1.5/tests/test_polygon_loader.py
+-rw-r--r--   0        0        0     2243 2024-04-01 23:14:18.112902 cyto-dl-0.1.5/tests/test_train.py
+-rw-r--r--   0        0        0      143 2024-04-01 23:14:18.112902 cyto-dl-0.1.5/tests/utils.py
+-rw-r--r--   0        0        0     6142 1970-01-01 00:00:00.000000 cyto-dl-0.1.5/PKG-INFO
```

### Comparing `cyto-dl-0.1.4/README.md` & `cyto-dl-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/configs/callbacks/early_stopping.yaml` & `cyto-dl-0.1.5/configs/callbacks/early_stopping.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/configs/callbacks/model_checkpoint.yaml` & `cyto-dl-0.1.5/configs/callbacks/model_checkpoint.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/configs/compile.yaml` & `cyto-dl-0.1.5/configs/compile.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/configs/data/classification/single_timepoint.yaml` & `cyto-dl-0.1.5/configs/data/classification/single_timepoint.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/configs/data/im2im/gan.yaml` & `cyto-dl-0.1.5/configs/data/im2im/gan.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/configs/data/im2im/gan_superres.yaml` & `cyto-dl-0.1.5/configs/data/im2im/gan_superres.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/configs/data/im2im/instance_seg.yaml` & `cyto-dl-0.1.5/configs/data/im2im/instance_seg.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/configs/data/im2im/labelfree.yaml` & `cyto-dl-0.1.5/configs/data/im2im/labelfree.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/configs/data/im2im/mae.yaml` & `cyto-dl-0.1.5/configs/data/im2im/mae.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/configs/data/im2im/segmentation.yaml` & `cyto-dl-0.1.5/configs/data/im2im/segmentation.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/configs/data/im2im/segmentation_plugin.yaml` & `cyto-dl-0.1.5/configs/data/im2im/segmentation_plugin.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/configs/data/im2im/segmentation_superres.yaml` & `cyto-dl-0.1.5/configs/data/im2im/segmentation_superres.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/configs/data/private/rotated_mnist.yaml` & `cyto-dl-0.1.5/configs/data/private/rotated_mnist.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/configs/data/private/variance_3d.yaml` & `cyto-dl-0.1.5/configs/data/private/variance_3d.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/configs/data/private/variance_3d_npm_nuc_v2.yaml` & `cyto-dl-0.1.5/configs/data/private/variance_3d_npm_nuc_v2.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/configs/data/private/variance_3d_rotate.yaml` & `cyto-dl-0.1.5/configs/data/private/variance_3d_rotate.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/configs/data/private/variance_centerslice.yaml` & `cyto-dl-0.1.5/configs/data/private/variance_centerslice.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/configs/data/private/variance_centerslice_resize.yaml` & `cyto-dl-0.1.5/configs/data/private/variance_centerslice_resize.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/configs/data/private/variance_npm1.yaml` & `cyto-dl-0.1.5/configs/data/private/variance_npm1.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/configs/debug/default.yaml` & `cyto-dl-0.1.5/configs/debug/default.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/configs/experiment/classification/per_timepoint.yaml` & `cyto-dl-0.1.5/configs/experiment/classification/per_timepoint.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/configs/experiment/im2im/gan.yaml` & `cyto-dl-0.1.5/configs/experiment/im2im/gan.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/configs/experiment/im2im/gan_superres.yaml` & `cyto-dl-0.1.5/configs/experiment/im2im/gan_superres.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/configs/experiment/im2im/instance_seg.yaml` & `cyto-dl-0.1.5/configs/experiment/im2im/instance_seg.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/configs/experiment/im2im/labelfree.yaml` & `cyto-dl-0.1.5/configs/experiment/im2im/labelfree.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/configs/experiment/im2im/mae.yaml` & `cyto-dl-0.1.5/configs/experiment/im2im/mae.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/configs/experiment/im2im/segmentation.yaml` & `cyto-dl-0.1.5/configs/experiment/im2im/segmentation.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/configs/experiment/im2im/segmentation_plugin.yaml` & `cyto-dl-0.1.5/configs/experiment/im2im/segmentation_plugin.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/configs/experiment/im2im/segmentation_superres.yaml` & `cyto-dl-0.1.5/configs/experiment/im2im/segmentation_superres.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/configs/experiment/im2im/vit_segmentation.yaml` & `cyto-dl-0.1.5/configs/experiment/im2im/vit_segmentation.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/configs/experiment/private/lattice_nuc_sdf.yaml` & `cyto-dl-0.1.5/configs/experiment/private/lattice_nuc_sdf.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/configs/experiment/private/mnist_so2.yaml` & `cyto-dl-0.1.5/configs/experiment/private/mnist_so2.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/configs/experiment/private/npm1_classical_3d_vae.yaml` & `cyto-dl-0.1.5/configs/experiment/private/npm1_classical_3d_vae.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/configs/experiment/private/npm1_classical_scale_inv.yaml` & `cyto-dl-0.1.5/configs/experiment/private/npm1_classical_scale_inv.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/configs/experiment/private/npm1_equiv_3d_vae_3dnucalign.yaml` & `cyto-dl-0.1.5/configs/experiment/private/npm1_equiv_3d_vae_3dnucalign.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/configs/experiment/private/npm1_scale_inv_canon_so3.yaml` & `cyto-dl-0.1.5/configs/experiment/private/npm1_scale_inv_canon_so3.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/configs/experiment/private/npm1_so2.yaml` & `cyto-dl-0.1.5/configs/experiment/private/npm1_so2.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/configs/experiment/private/npm1_so2_scale_inv.yaml` & `cyto-dl-0.1.5/configs/experiment/private/npm1_so2_scale_inv.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/configs/experiment/private/npm1_so3_scale_inv.yaml` & `cyto-dl-0.1.5/configs/experiment/private/npm1_so3_scale_inv.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/configs/experiment/private/npm1_so3_vae.yaml` & `cyto-dl-0.1.5/configs/experiment/private/npm1_so3_vae.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/configs/experiment/private/npm1_so3_vae_seg.yaml` & `cyto-dl-0.1.5/configs/experiment/private/npm1_so3_vae_seg.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/configs/experiment/private/variance_classical_2d_vae.yaml` & `cyto-dl-0.1.5/configs/experiment/private/variance_classical_2d_vae.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/configs/experiment/private/variance_classical_3d_vae.yaml` & `cyto-dl-0.1.5/configs/experiment/private/variance_classical_3d_vae.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/configs/experiment/private/variance_so2_3d_vae.yaml` & `cyto-dl-0.1.5/configs/experiment/private/variance_so2_3d_vae.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/configs/experiment/private/variance_so2_3d_vae_profiling.yaml` & `cyto-dl-0.1.5/configs/experiment/private/variance_so2_3d_vae_profiling.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/configs/experiment/private/variance_spharm.yaml` & `cyto-dl-0.1.5/configs/experiment/private/variance_spharm.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/configs/experiment/private/variance_spharm_o2.yaml` & `cyto-dl-0.1.5/configs/experiment/private/variance_spharm_o2.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/configs/hparams_search/mnist_optuna.yaml` & `cyto-dl-0.1.5/configs/hparams_search/mnist_optuna.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/configs/logger/wandb.yaml` & `cyto-dl-0.1.5/configs/logger/wandb.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/configs/model/classification/single_timepoint.yaml` & `cyto-dl-0.1.5/configs/model/classification/single_timepoint.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/configs/model/im2im/gan.yaml` & `cyto-dl-0.1.5/configs/model/im2im/gan.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/configs/model/im2im/gan_superres.yaml` & `cyto-dl-0.1.5/configs/model/im2im/gan_superres.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/configs/model/im2im/instance_seg.yaml` & `cyto-dl-0.1.5/configs/model/im2im/instance_seg.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/configs/model/im2im/labelfree.yaml` & `cyto-dl-0.1.5/configs/model/im2im/labelfree.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/configs/model/im2im/mae.yaml` & `cyto-dl-0.1.5/configs/model/im2im/mae.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/configs/model/im2im/segmentation.yaml` & `cyto-dl-0.1.5/configs/model/im2im/segmentation.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/configs/model/im2im/segmentation_plugin.yaml` & `cyto-dl-0.1.5/configs/model/im2im/segmentation_plugin.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/configs/model/im2im/segmentation_superres.yaml` & `cyto-dl-0.1.5/configs/model/im2im/segmentation_superres.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/configs/model/im2im/vit_segmentation_decoder.yaml` & `cyto-dl-0.1.5/configs/model/im2im/vit_segmentation_decoder.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/configs/model/private/classical_image_vae.yaml` & `cyto-dl-0.1.5/configs/model/private/classical_image_vae.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/configs/model/private/spharm.yaml` & `cyto-dl-0.1.5/configs/model/private/spharm.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/configs/model/test/base.yaml` & `cyto-dl-0.1.5/configs/model/test/base.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/configs/model/test/simple_segmentation.yaml` & `cyto-dl-0.1.5/configs/model/test/simple_segmentation.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/configs/train.yaml` & `cyto-dl-0.1.5/configs/train.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/api/model.py` & `cyto-dl-0.1.5/cyto_dl/api/model.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,21 +2,20 @@
 from typing import Dict, List, Union
 
 import pyrootutils
 from hydra import compose, initialize_config_dir
 from hydra.core.global_hydra import GlobalHydra
 from omegaconf import OmegaConf, open_dict
 
+from cyto_dl.api.data import ExperimentType
 from cyto_dl.eval import evaluate
 from cyto_dl.train import train as train_model
 from cyto_dl.utils.download_test_data import download_test_data
 from cyto_dl.utils.rich_utils import print_config_tree
 
-DEFAULT_EXPERIMENTS = ["gan", "instance_seg", "labelfree", "segmentation_plugin", "segmentation"]
-
 
 class CytoDLModel:
     def __init__(self):
         self.cfg = None
         self._training = False
         self._predicting = False
 
@@ -41,27 +40,29 @@
         # load config
         self.cfg = OmegaConf.load(config_path)
 
     def load_config_from_dict(self, config: dict):
         """Load configuration from dictionary."""
         self.cfg = config
 
+    # TODO: replace experiment_type str with api.data.ExperimentType -> will
+    # require corresponding changes in ml-segmenter
     def load_default_experiment(
-        self, experiment_name: str, output_dir: str, train=True, overrides: List = []
+        self, experiment_type: str, output_dir: str, train=True, overrides: List = []
     ):
         """Load configuration from directory."""
-        assert experiment_name in DEFAULT_EXPERIMENTS
+        assert experiment_type in {exp_type.value for exp_type in ExperimentType}
         config_dir = self.root / "configs"
 
         GlobalHydra.instance().clear()
         with initialize_config_dir(version_base="1.2", config_dir=str(config_dir)):
             cfg = compose(
                 config_name="train.yaml" if train else "eval.yaml",
                 return_hydra_config=True,
-                overrides=[f"experiment=im2im/{experiment_name}"] + overrides,
+                overrides=[f"experiment=im2im/{experiment_type}"] + overrides,
             )
 
         with open_dict(cfg):
             del cfg["hydra"]
             cfg.extras.enforce_tags = False
             cfg.extras.print_config = False
             cfg["paths"]["output_dir"] = output_dir
```

### Comparing `cyto-dl-0.1.4/cyto_dl/callbacks/callback_utils.py` & `cyto-dl-0.1.5/cyto_dl/callbacks/callback_utils.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/callbacks/latent_walk.py` & `cyto-dl-0.1.5/cyto_dl/callbacks/latent_walk.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/callbacks/layer_freeze.py` & `cyto-dl-0.1.5/cyto_dl/callbacks/layer_freeze.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/callbacks/model_utils.py` & `cyto-dl-0.1.5/cyto_dl/callbacks/model_utils.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/callbacks/outlier_detection.py` & `cyto-dl-0.1.5/cyto_dl/callbacks/outlier_detection.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/compile.py` & `cyto-dl-0.1.5/cyto_dl/compile.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/dataframe/readers.py` & `cyto-dl-0.1.5/cyto_dl/dataframe/readers.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/dataframe/transforms/filter.py` & `cyto-dl-0.1.5/cyto_dl/dataframe/transforms/filter.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/dataframe/transforms/group_cols.py` & `cyto-dl-0.1.5/cyto_dl/dataframe/transforms/group_cols.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/dataframe/transforms/misc.py` & `cyto-dl-0.1.5/cyto_dl/dataframe/transforms/misc.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/dataframe/transforms/split.py` & `cyto-dl-0.1.5/cyto_dl/dataframe/transforms/split.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/datamodules/czi.py` & `cyto-dl-0.1.5/cyto_dl/datamodules/czi.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,15 @@
         out_key: str,
         spatial_dims: int = 3,
         scene_column: str = "scene",
         time_start_column: str = "start",
         time_stop_column: str = "stop",
         time_step_column: str = "step",
         transform: Optional[Callable] = None,
+        dask_load: bool = True,
     ):
         """
         Parameters
         ----------
         csv_path: Union[Path, str]
             path to csv
         img_path_column: str
@@ -49,27 +50,30 @@
             Column in `csv_path` specifying which timepoint in timelapse CZI to stop extracting. If any of `start_column`, `stop_column`, or `step_column`
             are not specified, all timepoints are extracted.
         time_step_column:str="step"
             Column in `csv_path` specifying step between timepoints. For example, values in this column should be `2` if every other timepoint should be run.
             If any of `start_column`, `stop_column`, or `step_column` are not specified, all timepoints are extracted.
         transform: Optional[Callable] = None
             Callable to that accepts numpy array. For example, image normalization functions could be passed here.
+        dask_load: bool = True
+            Whether to use dask to load images. If False, full images are loaded into memory before extracting specified scenes/timepoints.
         """
         super().__init__(None, transform)
         df = pd.read_csv(csv_path)
         self.img_path_column = img_path_column
         self.channel_column = channel_column
         self.scene_column = scene_column
         self.time_start_column = time_start_column
         self.time_stop_column = time_stop_column
         self.time_step_column = time_step_column
         self.out_key = out_key
         if spatial_dims not in (2, 3):
             raise ValueError(f"`spatial_dims` must be 2 or 3, got {spatial_dims}")
         self.spatial_dims = spatial_dims
+        self.dask_load = dask_load
 
         self.img_data = self.get_per_file_args(df)
 
     def _get_scenes(self, row, img):
         scenes = row.get(self.scene_column, -1)
         if scenes != -1:
             scenes = scenes.strip().split(",")
@@ -122,15 +126,18 @@
 
     def _transform(self, index: int):
         img_data = self.img_data.pop()
         img = img_data.pop("img")
         original_path = img_data.pop("original_path")
         scene = img_data.pop("scene")
         img.set_scene(scene)
-        data_i = img.get_image_dask_data(**img_data).compute()
+        if self.dask_load:
+            data_i = img.get_image_dask_data(**img_data).compute()
+        else:
+            data_i = img.get_image_data(**img_data)
         img_data["scene"] = scene
         data_i = self._ensure_channel_first(data_i)
         output_img = (
             apply_transform(self.transform, data_i) if self.transform is not None else data_i
         )
 
         return {
```

### Comparing `cyto-dl-0.1.4/cyto_dl/datamodules/data_dict.py` & `cyto-dl-0.1.5/cyto_dl/datamodules/data_dict.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/datamodules/dataframe/dataframe_datamodule.py` & `cyto-dl-0.1.5/cyto_dl/datamodules/dataframe/dataframe_datamodule.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import torch
 from lightning import LightningDataModule
 from lightning.pytorch.utilities.exceptions import MisconfigurationException
 from monai.data import DataLoader
 from upath import UPath as Path
 
 from .utils import (
-    AlternatingBatchSampler,
     get_canonical_split_name,
     make_multiple_dataframe_splits,
     make_single_dataframe_splits,
     parse_transforms,
 )
 
 
@@ -37,14 +36,15 @@
         columns: Optional[Sequence[str]] = None,
         split_map: Optional[Dict] = None,
         just_inference: bool = False,
         cache_dir: Optional[Union[Path, str]] = None,
         subsample: Optional[Dict] = None,
         refresh_subsample: bool = False,
         seed: int = 42,
+        smartcache_args: Optional[Dict] = None,
         **dataloader_kwargs,
     ):
         """
         Parameters
         ----------
         path: Union[Path, str]
             Path to a dataframe file
@@ -73,14 +73,23 @@
             accelerate batch loading.
 
         subsample: Optional[Dict] = None
             Dictionary with a key per split ("train", "val", "test"), and the
             number of samples of each split to use per epoch. If `None` (default),
             use all the samples in each split per epoch.
 
+        refresh_subsample: bool = False
+            Whether to refresh subsample each time dataloader is called
+
+        seed: int = 42
+            random seed
+
+        smartcache_args: Optional[Dict] = None
+            Arguments to pass to SmartcacheDataset
+
         dataloader_kwargs:
             Additional keyword arguments are passed to the
             torch.utils.data.DataLoader class when instantiating it (aside from
             `shuffle` which is only used for the train dataloader).
             Among these args are `num_workers`, `batch_size`, `shuffle`, etc.
             See the PyTorch docs for more info on these args:
             https://pytorch.org/docs/stable/data.html#torch.utils.data.DataLoader
@@ -98,15 +107,20 @@
         path = Path(path)
 
         # if path is a directory, we assume it is a directory containing multiple
         # dataframes - one per split. otherwise, we assume it is the path to a single
         # dataframe file, which is expected to have a
         if path.is_dir():
             self.datasets = make_multiple_dataframe_splits(
-                path, transforms, columns, just_inference, cache_dir
+                path,
+                transforms,
+                columns,
+                just_inference,
+                cache_dir,
+                smartcache_args=smartcache_args,
             )
         elif path.is_file():
             if split_column is None and not just_inference:
                 raise MisconfigurationException(
                     "When using a single dataframe file, it must have a "
                     "split column, to use for train-val-test splitting."
                 )
@@ -115,14 +129,15 @@
                 path,
                 transforms,
                 split_column,
                 columns,
                 just_inference,
                 split_map,
                 cache_dir,
+                smartcache_args=smartcache_args,
             )
         else:
             raise FileNotFoundError(f"Could not find specified dataframe path {path}")
 
         self.just_inference = just_inference
         self.dataloader_kwargs = dataloader_kwargs
         self.dataloaders = {}
```

### Comparing `cyto-dl-0.1.4/cyto_dl/datamodules/dataframe/grouped_dataframe_datamodule.py` & `cyto-dl-0.1.5/cyto_dl/datamodules/dataframe/grouped_dataframe_datamodule.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,15 @@
         columns: Optional[Sequence[str]] = None,
         split_map: Optional[Dict] = None,
         just_inference: bool = False,
         cache_dir: Optional[Union[Path, str]] = None,
         subsample: Optional[Dict] = None,
         refresh_subsample: bool = False,
         seed: int = 42,
+        smartcache_args: Optional[Dict] = None,
         target_columns: str = None,
         grouping_column: str = None,
         **dataloader_kwargs,
     ):
         """
         Parameters
         ----------
@@ -68,14 +69,17 @@
 
         refresh_subsample: bool = False
             Whether to refresh subsample each time dataloader is called
 
         seed: int = 42
             random seed
 
+        smartcache_args: Optional[Dict] = None
+            Arguments to pass to SmartcacheDataset
+
         target_columns: str = None
             column names in csv corresponding to ground truth types to alternate between
             during training
 
         grouping_column: str = None
             column names in csv corresponding to a factor that should be homogeneous across
             a batch
@@ -101,14 +105,15 @@
             columns=columns,
             split_map=split_map,
             just_inference=just_inference,
             cache_dir=cache_dir,
             subsample=subsample,
             refresh_subsample=refresh_subsample,
             seed=seed,
+            smartcache_args=smartcache_args,
             **dataloader_kwargs,
         )
         self.group_column = grouping_column
         self.target_columns = target_columns
 
     def make_dataloader(self, split):
         kwargs = dict(**self.dataloader_kwargs)
```

### Comparing `cyto-dl-0.1.4/cyto_dl/datamodules/dataframe/utils.py` & `cyto-dl-0.1.5/cyto_dl/datamodules/dataframe/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     import modin.pandas as pd
 except ModuleNotFoundError:
     import pandas as pd
 
 import random
 from typing import Sequence
 
-from monai.data import Dataset, PersistentDataset
+from monai.data import Dataset, PersistentDataset, SmartCacheDataset
 from monai.transforms import Compose, Transform
 from omegaconf import DictConfig, ListConfig
 from torch.utils.data import BatchSampler, Sampler, Subset, SubsetRandomSampler
 from upath import UPath as Path
 
 from cyto_dl.dataframe import read_dataframe
 
@@ -147,32 +147,50 @@
         return min_num_batches * len(self.samplers)
 
 
 def get_canonical_split_name(split):
     for canon in ("train", "val", "test", "predict"):
         if split.startswith(canon) or canon.startswith(split):
             return canon
-    raise ValueError
+    return None
 
 
-def get_dataset(dataframe, transform, split, cache_dir=None):
+def get_dataset(dataframe, transform, split, cache_dir=None, smartcache_args=None):
     data = _DataframeWrapper(dataframe)
+    if smartcache_args is not None and split in ("train", "val"):
+        cache_rate = smartcache_args.get("cache_rate", 0.1)
+        if cache_rate * len(data) >= 1:
+            print(f"Initializing SmartCacheDataset for {split}")
+            return SmartCacheDataset(
+                data,
+                transform=transform,
+                cache_rate=cache_rate,
+                replace_rate=smartcache_args.get("replace_rate", 0.1),
+                num_init_workers=smartcache_args.get("num_init_workers", 4),
+                num_replace_workers=smartcache_args.get("num_replace_workers", 4),
+            )
+        else:
+            print(
+                f"Cache rate {cache_rate} too low for {split} dataset with size {len(data)}, using Dataset."
+            )
     if cache_dir is not None and split in ("train", "val"):
+        print(f"Initializing PersistentDataset for {split} at {cache_dir}")
         return PersistentDataset(data, transform=transform, cache_dir=cache_dir)
     return Dataset(data, transform=transform)
 
 
 def make_single_dataframe_splits(
     dataframe_path,
     transforms,
     split_column,
     columns=None,
     just_inference=False,
     split_map=None,
     cache_dir=None,
+    smartcache_args=None,
 ):
     dataframe = read_dataframe(dataframe_path, columns)
     dataframe[split_column] = dataframe[split_column].astype(np.dtype("O"))
 
     if not just_inference:
         assert dataframe.dtypes[split_column] == np.dtype("O")
 
@@ -197,51 +215,70 @@
             else:
                 _split_cache = None
             datasets[split] = get_dataset(
                 dataframe.loc[dataframe["split"].str.startswith(split)],
                 transforms[split],
                 split,
                 _split_cache,
+                smartcache_args=smartcache_args,
             )
 
     datasets["predict"] = get_dataset(
-        dataframe, transform=transforms["predict"], split="predict", cache_dir=cache_dir
+        dataframe,
+        transform=transforms["predict"],
+        split="predict",
+        cache_dir=cache_dir,
+        smartcache_args=smartcache_args,
     )
     return datasets
 
 
 def make_multiple_dataframe_splits(
-    split_path, transforms, columns=None, just_inference=False, cache_dir=None
+    split_path,
+    transforms,
+    columns=None,
+    just_inference=False,
+    cache_dir=None,
+    smartcache_args=None,
 ):
     split_path = Path(split_path)
     datasets = {}
     predict_df = []
 
     for fpath in chain(split_path.glob("*.csv"), split_path.glob("*.parquet")):
         split = re.findall(r"(.*)\.(?:csv|parquet)", fpath.name)[0]
         split = get_canonical_split_name(split)
+        if split is None:
+            print(f"Skipping {fpath} as it does not match any known split name.")
+            continue
         dataframe = read_dataframe(fpath, required_columns=columns)
         dataframe["split"] = split
 
         if cache_dir is not None:
             _split_cache = Path(cache_dir) / split
             _split_cache.mkdir(exist_ok=True, parents=True)
         else:
             _split_cache = None
 
         if not just_inference:
-            datasets[split] = get_dataset(dataframe, transforms[split], split, _split_cache)
+            datasets[split] = get_dataset(
+                dataframe, transforms[split], split, _split_cache, smartcache_args=smartcache_args
+            )
         predict_df.append(dataframe.copy())
 
+    if len(predict_df) == 0:
+        raise ValueError(f"No valid dataframe files found in {split_path}")
+
     predict_df = pd.concat(predict_df)
     datasets["predict"] = get_dataset(
         predict_df,
         transform=transforms["predict"],
         split="predict",
         cache_dir=cache_dir,
+        smartcache_args=smartcache_args,
     )
 
     return datasets
 
 
 def parse_transforms(transforms):
     if not isinstance(transforms, (DictConfig, dict)):
```

### Comparing `cyto-dl-0.1.4/cyto_dl/datamodules/folder.py` & `cyto-dl-0.1.5/cyto_dl/datamodules/folder.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/datamodules/smartcache.py` & `cyto-dl-0.1.5/cyto_dl/datamodules/smartcache.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 from pathlib import Path
 from typing import Optional, Union
 
 import dask
 import numpy as np
 import pandas as pd
-import tqdm
 from aicsimageio import AICSImage
 from dask.diagnostics import ProgressBar
 from lightning import LightningDataModule
 from monai.data import DataLoader
-from monai.data.dataset import Dataset, SmartCacheDataset
+from monai.data.dataset import CacheDataset, Dataset, SmartCacheDataset
 from monai.transforms import Compose
 from sklearn.model_selection import train_test_split
 
 
 class SmartcacheDatamodule(LightningDataModule):
     """Datamodule for large CZI datasets that don't fit in memory."""
 
     def __init__(
         self,
-        csv_path: Union[Path, str],
+        csv_path: Optional[Union[Path, str]] = None,
         transforms: Compose = None,
         img_data: Optional[Union[Path, str]] = None,
         n_val: int = 20,
         pct_val: float = 0.1,
         img_path_column: str = "raw",
         channel_column: str = "ch",
         spatial_dims: int = 3,
-        neighboring_timepoints: bool = False,
+        num_neighbors: int = 0,
         num_workers: int = 4,
         cache_rate: float = 0.5,
+        replace_rate: float = 0.1,
         **kwargs,
     ):
         """
         Parameters
         ----------
         csv_path: Union[Path, str]
             path to csv with image in `img_path_column` and channel in `channel_column`
@@ -47,72 +47,89 @@
             percentage of images to use for validation. Minimum of pct_val * n_images and n_val is used.
         img_path_column: str
             column in csv_path that contains the path to the image
         channel_column: str
             column in csv_path that contains the channel to use
         spatial_dims: int
             number of spatial dimensions in the image
-        neighboring_timepoints: bool
-            whether to return T and T+1 as a 2 channel image, useful for models incorporating time
+        num_neighbors: int
+            number of neighboring timepoints to use
         num_workers: int
             number of workers to use for loading data. Most be specified here to schedule replacement workers for cache data
         cache_rate: float
             percentage of data to cache
+        replace_rate: float
+            percentage of data to replace
+        kwargs:
+            additional arguments to pass to DataLoader
         """
         super().__init__()
-        self.csv_path = Path(csv_path)
-        (self.csv_path.parents[0] / "loaded_data").mkdir(exist_ok=True, parents=True)
-        self.df = pd.read_csv(csv_path)
+        self.img_data = {}
+        if isinstance(img_data, (str, Path)):
+            # read img_data if it's a path, otherwise set to empty dict
+            self.img_data["train"] = [
+                row._asdict()
+                for row in pd.read_csv(Path(img_data) / "train_img_data.csv").itertuples()
+            ]
+            self.img_data["val"] = [
+                row._asdict()
+                for row in pd.read_csv(Path(img_data) / "val_img_data.csv").itertuples()
+            ]
+        elif csv_path is not None:
+            self.csv_path = Path(csv_path)
+            (self.csv_path.parents[0] / "loaded_data").mkdir(exist_ok=True, parents=True)
+            self.df = pd.read_csv(csv_path)
+        else:
+            raise ValueError("csv_path or img_data must be specified")
         self.num_workers = num_workers
         self.kwargs = kwargs
-        val_size = np.min([n_val, int(len(self.df) * pct_val)])
-        self.val_size = np.max([val_size, 1])
-        # read img_data if it's a path, otherwise set to empty dict
-        if isinstance(img_data, str):
-            self.img_data = pd.read_csv(img_data)
-        else:
-            self.img_data = {}
+
+        self.n_val = n_val
+        self.pct_val = pct_val
+
         self.datasets = {}
         self.img_path_column = img_path_column
         self.channel_column = channel_column
         self.spatial_dims = spatial_dims
         self.transforms = transforms
-        self.neighboring_timepoints = neighboring_timepoints
+        self.num_neighbors = num_neighbors
         self.cache_rate = cache_rate
+        self.replace_rate = replace_rate
 
     def _get_scenes(self, img):
         """Get the number of scenes in an image."""
         return img.scenes
 
     def _get_timepoints(self, img):
         """Get the number of timepoints in an image."""
         timepoints = list(range(img.dims.T))
-        if self.neighboring_timepoints:
-            return timepoints[:-1]
+        if self.num_neighbors > 0:
+            return timepoints[: -self.num_neighbors]
         return timepoints
 
     @dask.delayed
     def _get_file_args(self, row):
         row = row._asdict()
         img = AICSImage(row[self.img_path_column])
         scenes = self._get_scenes(img)
         timepoints = self._get_timepoints(img)
         img_data = []
+        use_neighbors = self.num_neighbors > 0
         for scene in scenes:
             for timepoint in timepoints:
                 img_data.append(
                     {
                         "dimension_order_out": "ZYX"[-self.spatial_dims :]
-                        if not self.neighboring_timepoints
+                        if not use_neighbors
                         else "T" + "ZYX"[-self.spatial_dims :],
                         "C": row[self.channel_column],
                         "scene": scene,
                         "T": timepoint
-                        if not self.neighboring_timepoints
-                        else [timepoint, timepoint + 1],
+                        if not use_neighbors
+                        else [timepoint + i for i in range(self.num_neighbors + 1)],
                         "original_path": row[self.img_path_column],
                     }
                 )
         return img_data
 
     def get_per_file_args(self, df):
         """Parallelize getting the image loading arguments enumerating all
@@ -123,48 +140,58 @@
         return img_data
 
     def prepare_data(self):
         pass
 
     def setup(self, stage=None):
         if stage == "fit":
-            # split df into train/test/val
-            self.df_train, self.df_val = train_test_split(self.df, test_size=self.val_size)
-            # update img_data
-            self.img_data["train"] = self.get_per_file_args(self.df_train)
-            self.img_data["val"] = self.get_per_file_args(self.df_val)
-            pd.DataFrame(self.img_data["train"]).to_csv(
-                f"{self.csv_path.parents[0]}/loaded_data/train_img_data.csv",
-                index=False,
-            )
-            pd.DataFrame(self.img_data["val"]).to_csv(
-                f"{self.csv_path.parents[0]}/loaded_data/val_img_data.csv", index=False
-            )
+            if "train" not in self.img_data or "val" not in self.img_data:
+                # update img_data
+                image_data = self.get_per_file_args(self.df)
+                val_size = np.min([self.n_val, int(len(image_data) * self.pct_val)])
+                val_size = np.max([val_size, 1])
+                self.img_data["train"], self.img_data["val"] = train_test_split(
+                    image_data, test_size=val_size
+                )
+
+                print("Train images:", len(self.img_data["train"]))
+                print("Val images:", len(self.img_data["val"]))
+
+                pd.DataFrame(self.img_data["train"]).to_csv(
+                    f"{self.csv_path.parents[0]}/loaded_data/train_img_data.csv",
+                    index=False,
+                )
+                pd.DataFrame(self.img_data["val"]).to_csv(
+                    f"{self.csv_path.parents[0]}/loaded_data/val_img_data.csv", index=False
+                )
 
             self.datasets["train"] = SmartCacheDataset(
                 self.img_data["train"],
                 transform=self.transforms["train"],
                 cache_rate=self.cache_rate,
-                num_replace_workers=self.num_workers // 2,
+                num_replace_workers=self.num_workers,
+                num_init_workers=self.num_workers,
+                replace_rate=self.replace_rate,
             )
-            self.datasets["val"] = SmartCacheDataset(
+            self.datasets["val"] = CacheDataset(
                 self.img_data["val"],
-                transform=self.transforms["val"],
-                cache_rate=self.cache_rate,
-                num_replace_workers=self.num_workers // 2,
+                transform=self.transforms["valid"],
+                cache_rate=1.0,
+                num_workers=self.num_workers,
             )
 
         elif stage in ("test", "predict"):
             self.img_data[stage] = self.get_per_file_args(self.df)
             self.datasets[stage] = Dataset(self.img_data[stage], transform=self.transforms[stage])
 
     def make_dataloader(self, split):
         # smartcachedataset can't have persistent workers
         self.kwargs["persistent_workers"] = split not in ("train", "val")
-        self.kwargs.pop("num_workers")
+        if "num_workers" in self.kwargs:
+            del self.kwargs["num_workers"]
         return DataLoader(
             self.datasets[split],
             num_workers=self.num_workers,
             **self.kwargs,
         )
 
     def train_dataloader(self):
```

### Comparing `cyto-dl-0.1.4/cyto_dl/datamodules/torchvision.py` & `cyto-dl-0.1.5/cyto_dl/datamodules/torchvision.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/eval.py` & `cyto-dl-0.1.5/cyto_dl/eval.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/image/io/aicsimage_loader.py` & `cyto-dl-0.1.5/cyto_dl/image/io/aicsimage_loader.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import List
 
+import numpy as np
 from aicsimageio import AICSImage
 from monai.data import MetaTensor
 from monai.transforms import Transform
 
 
 class AICSImageLoaderd(Transform):
     """Enumerates scenes and timepoints for dictionary with format.
@@ -16,43 +17,53 @@
     def __init__(
         self,
         path_key: str = "path",
         scene_key: str = "scene",
         kwargs_keys: List = ["dimension_order_out", "C", "T"],
         out_key: str = "raw",
         allow_missing_keys=False,
+        dtype: np.dtype = np.float16,
+        dask_load: bool = True,
     ):
         """
         Parameters
         ----------
         path_key : str = "path"
             Key for the path to the image
         scene_key : str = "scene"
             Key for the scene number
         kwargs_keys : List = ["dimension_order_out", "C", "T"]
             Keys for the kwargs to pass to AICSImage.get_image_dask_data
         out_key : str = "raw"
             Key for the output image
         allow_missing_keys : bool = False
             Whether to allow missing keys in the data dictionary
+        dask_load: bool = True
+            Whether to use dask to load images. If False, full images are loaded into memory before extracting specified scenes/timepoints.
         """
         super().__init__()
         self.path_key = path_key
         self.kwargs_keys = kwargs_keys
         self.allow_missing_keys = allow_missing_keys
         self.out_key = out_key
         self.scene_key = scene_key
+        self.dtype = dtype
+        self.dask_load = dask_load
 
     def __call__(self, data):
         # copying prevents the dataset from being modified inplace - important when using partially cached datasets so that the memory use doesn't increase over time
         data = data.copy()
         if self.path_key not in data and not self.allow_missing_keys:
             raise KeyError(f"Missing key {self.path_key} in data dictionary")
         path = data[self.path_key]
         img = AICSImage(path)
         if self.scene_key in data:
             img.set_scene(data[self.scene_key])
         kwargs = {k: data[k] for k in self.kwargs_keys}
-        img = img.get_image_dask_data(**kwargs).compute()
+        if self.dask_load:
+            img = img.get_image_dask_data(**kwargs).compute()
+        else:
+            img = img.get_image_data(**kwargs)
+        img = img.astype(self.dtype)
         data[self.out_key] = MetaTensor(img, meta={"filename_or_obj": path, "kwargs": kwargs})
 
         return data
```

### Comparing `cyto-dl-0.1.4/cyto_dl/image/io/monai_bio_reader.py` & `cyto-dl-0.1.5/cyto_dl/image/io/skimage_reader.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,48 @@
 """ADAPTED FROM https://github.com/MMV-Lab/mmv_im2im/"""
 
-from typing import Dict, List, Sequence, Tuple, Union
+from typing import Dict, List, Optional, Sequence, Tuple, Union
 
 import numpy as np
-from aicsimageio import AICSImage
 from monai.config import PathLike
 from monai.data import ImageReader
 from monai.data.image_reader import _stack_images
 from monai.utils import ensure_tuple, require_pkg
-from omegaconf import Container, OmegaConf
+from skimage.io import imread
 
 
-@require_pkg(pkg_name="aicsimageio")
-class MonaiBioReader(ImageReader):
-    def __init__(self, **reader_kwargs):
+@require_pkg(pkg_name="skimage")
+class SkimageReader(ImageReader):
+    def __init__(
+        self,
+        channels: Optional[list] = None,
+        transforms: Optional[list] = None,
+    ):
         super().__init__()
-        self.reader_kwargs = {
-            k: OmegaConf.to_container(v) if isinstance(v, Container) else v
-            for k, v in reader_kwargs.items()
-            if v is not None
-        }
+        self.channels = channels
+        self.transforms = transforms
 
     def read(self, data: Union[Sequence[PathLike], PathLike]):
         filenames: Sequence[PathLike] = ensure_tuple(data)
         img_ = []
         for name in filenames:
-            img_.append(AICSImage(f"{name}"))
+            this_im = imread(f"{name}")
+            if self.channels:
+                this_im = this_im[self.channels]
+
+            if self.transforms:
+                for transform in self.transforms:
+                    this_im = transform(this_im)
+            img_.append(this_im)
 
         return img_ if len(filenames) > 1 else img_[0]
 
     def get_data(self, img) -> Tuple[np.ndarray, Dict]:
         img_array: List[np.ndarray] = []
-
         for img_obj in ensure_tuple(img):
-            data = img_obj.get_image_dask_data(**self.reader_kwargs).compute()
+            data = img_obj
             img_array.append(data)
 
         return _stack_images(img_array, {}), {}
 
     def verify_suffix(self, filename: Union[Sequence[PathLike], PathLike]) -> bool:
         return True
```

### Comparing `cyto-dl-0.1.4/cyto_dl/image/io/numpy_reader.py` & `cyto-dl-0.1.5/cyto_dl/image/io/numpy_reader.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/image/io/ome_zarr_reader.py` & `cyto-dl-0.1.5/cyto_dl/image/io/ome_zarr_reader.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/image/io/polygon_loader.py` & `cyto-dl-0.1.5/cyto_dl/image/io/polygon_loader.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/image/transforms/__init__.py` & `cyto-dl-0.1.5/cyto_dl/image/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/image/transforms/bright_sampler.py` & `cyto-dl-0.1.5/cyto_dl/image/transforms/bright_sampler.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/image/transforms/clip.py` & `cyto-dl-0.1.5/cyto_dl/image/transforms/clip.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/image/transforms/contrastadjust.py` & `cyto-dl-0.1.5/cyto_dl/image/transforms/contrastadjust.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/image/transforms/merge.py` & `cyto-dl-0.1.5/cyto_dl/image/transforms/merge.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/image/transforms/multiscale_cropper.py` & `cyto-dl-0.1.5/cyto_dl/image/transforms/multiscale_cropper.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,14 +105,15 @@
             shape = np.asarray(image_dict[im_name].shape[-self.spatial_dims :])
             shape = np.floor_divide(shape, rescale_factor)
             roi_size = np.floor_divide(self.roi_size, rescale_factor)
             max_start_indices_img = shape - roi_size
             max_start_indices = np.minimum(max_start_indices_img, max_start_indices)
             if np.any(max_start_indices < 0):
                 raise ValueError(f"Crop size {roi_size} is too large for image size {shape}")
+            max_start_indices += max_start_indices == 0
         return max_start_indices
 
     def generate_slices(self, image_dict: Dict) -> Dict:
         """Generate dictionary of slices at all scales starting at random point."""
         max_start_indices = self._get_max_start_indices(image_dict)
 
         start_indices = self.R.randint(max_start_indices)
```

### Comparing `cyto-dl-0.1.4/cyto_dl/image/transforms/pad.py` & `cyto-dl-0.1.5/cyto_dl/image/transforms/pad.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/image/transforms/project.py` & `cyto-dl-0.1.5/cyto_dl/image/transforms/project.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/image/transforms/rotation_mask_transform.py` & `cyto-dl-0.1.5/cyto_dl/image/transforms/rotation_mask_transform.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/image/transforms/save.py` & `cyto-dl-0.1.5/cyto_dl/image/transforms/save.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/image/transforms/so2_random_rotation.py` & `cyto-dl-0.1.5/cyto_dl/image/transforms/so2_random_rotation.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/image/transforms/track_transforms.py` & `cyto-dl-0.1.5/cyto_dl/image/transforms/track_transforms.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/loggers/mlflow.py` & `cyto-dl-0.1.5/cyto_dl/loggers/mlflow.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/models/base_model.py` & `cyto-dl-0.1.5/cyto_dl/models/base_model.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/models/basic_model.py` & `cyto-dl-0.1.5/cyto_dl/models/basic_model.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/models/classification/classification.py` & `cyto-dl-0.1.5/cyto_dl/models/classification/classification.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/models/classification/timepoint_classification.py` & `cyto-dl-0.1.5/cyto_dl/models/classification/timepoint_classification.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/models/handlers/base_handler.py` & `cyto-dl-0.1.5/cyto_dl/models/handlers/base_handler.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/models/handlers/image_handler.py` & `cyto-dl-0.1.5/cyto_dl/models/handlers/image_handler.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/models/handlers/load_image_patch.py` & `cyto-dl-0.1.5/cyto_dl/models/handlers/load_image_patch.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/models/im2im/gan.py` & `cyto-dl-0.1.5/cyto_dl/models/im2im/gan.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/models/im2im/multi_task.py` & `cyto-dl-0.1.5/cyto_dl/models/im2im/multi_task.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import sys
+from contextlib import suppress
 from pathlib import Path
 from typing import Dict, List, Union
 
 import torch
 import torch.nn as nn
 from monai.data.meta_tensor import MetaTensor
 from monai.inferers import sliding_window_inference
@@ -216,7 +217,20 @@
         stage = "predict"
         run_heads, io_map = self._get_run_heads(batch, stage, batch_idx)
         if len(run_heads) > 0:
             batch = self._to_tensor(batch)
             save_image = self.should_save_image(batch_idx, stage)
             self.run_forward(batch, stage, save_image, run_heads)
         return io_map
+
+    # utils for smartcache training
+    def on_train_start(self):
+        with suppress(AttributeError):
+            self.trainer.datamodule.train_dataloader().dataset.start()
+
+    def on_train_epoch_end(self):
+        with suppress(AttributeError):
+            self.trainer.datamodule.train_dataloader().dataset.update_cache()
+
+    def on_train_end(self, *args, **kwargs):
+        with suppress(AttributeError):
+            self.trainer.datamodule.train_dataloader().dataset.shutdown()
```

### Comparing `cyto-dl-0.1.4/cyto_dl/models/im2im/utils/instance_seg.py` & `cyto-dl-0.1.5/cyto_dl/models/im2im/utils/instance_seg.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/models/im2im/utils/noise_annealer.py` & `cyto-dl-0.1.5/cyto_dl/models/im2im/utils/noise_annealer.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/models/im2im/utils/postprocessing/act_thresh_label.py` & `cyto-dl-0.1.5/cyto_dl/models/im2im/utils/postprocessing/act_thresh_label.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/models/im2im/utils/postprocessing/auto_thresh.py` & `cyto-dl-0.1.5/cyto_dl/models/im2im/utils/postprocessing/auto_thresh.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/models/im2im/utils/postprocessing/dict_to_im.py` & `cyto-dl-0.1.5/cyto_dl/models/im2im/utils/postprocessing/dict_to_im.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/models/utils/mlflow.py` & `cyto-dl-0.1.5/cyto_dl/models/utils/mlflow.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/models/vae/base_vae.py` & `cyto-dl-0.1.5/cyto_dl/models/vae/base_vae.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/models/vae/image_canon_vae.py` & `cyto-dl-0.1.5/cyto_dl/models/vae/image_canon_vae.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/models/vae/image_encoder.py` & `cyto-dl-0.1.5/cyto_dl/models/vae/image_encoder.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/models/vae/image_vae.py` & `cyto-dl-0.1.5/cyto_dl/models/vae/image_vae.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/models/vae/latent_loss_vae.py` & `cyto-dl-0.1.5/cyto_dl/models/vae/latent_loss_vae.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/models/vae/o2_spharm_vae/o2_spharm_encoder.py` & `cyto-dl-0.1.5/cyto_dl/models/vae/o2_spharm_vae/o2_spharm_encoder.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/models/vae/o2_spharm_vae/o2_spharm_vae.py` & `cyto-dl-0.1.5/cyto_dl/models/vae/o2_spharm_vae/o2_spharm_vae.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/models/vae/point_cloud_vae.py` & `cyto-dl-0.1.5/cyto_dl/models/vae/point_cloud_vae.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/models/vae/priors/abstract_prior.py` & `cyto-dl-0.1.5/cyto_dl/models/vae/priors/abstract_prior.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/models/vae/priors/gaussian.py` & `cyto-dl-0.1.5/cyto_dl/models/vae/priors/gaussian.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/models/vae/priors/joint_prior.py` & `cyto-dl-0.1.5/cyto_dl/models/vae/priors/joint_prior.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/models/vae/tabular_vae.py` & `cyto-dl-0.1.5/cyto_dl/models/vae/tabular_vae.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/nn/discriminators/multi_scale_discriminator.py` & `cyto-dl-0.1.5/cyto_dl/nn/discriminators/multi_scale_discriminator.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/nn/discriminators/n_layer_discriminator.py` & `cyto-dl-0.1.5/cyto_dl/nn/discriminators/n_layer_discriminator.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/nn/head/base_head.py` & `cyto-dl-0.1.5/cyto_dl/nn/head/base_head.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/nn/head/gan_head.py` & `cyto-dl-0.1.5/cyto_dl/nn/head/gan_head.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/nn/head/gan_head_superres.py` & `cyto-dl-0.1.5/cyto_dl/nn/head/gan_head_superres.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/nn/head/mae_head.py` & `cyto-dl-0.1.5/cyto_dl/nn/head/mae_head.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/nn/head/mask_head.py` & `cyto-dl-0.1.5/cyto_dl/nn/head/mask_head.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/nn/head/res_blocks_head.py` & `cyto-dl-0.1.5/cyto_dl/nn/head/res_blocks_head.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/nn/hr_skip.py` & `cyto-dl-0.1.5/cyto_dl/nn/hr_skip.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/nn/losses/__init__.py` & `cyto-dl-0.1.5/cyto_dl/nn/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/nn/losses/adversarial_loss.py` & `cyto-dl-0.1.5/cyto_dl/nn/losses/adversarial_loss.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/nn/losses/chamfer_loss.py` & `cyto-dl-0.1.5/cyto_dl/nn/losses/chamfer_loss.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/nn/losses/continuous_bernoulli.py` & `cyto-dl-0.1.5/cyto_dl/nn/losses/continuous_bernoulli.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/nn/losses/cosine_loss.py` & `cyto-dl-0.1.5/cyto_dl/nn/losses/cosine_loss.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/nn/losses/gan_loss.py` & `cyto-dl-0.1.5/cyto_dl/nn/losses/gan_loss.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/nn/losses/gaussian_nll_loss.py` & `cyto-dl-0.1.5/cyto_dl/nn/losses/gaussian_nll_loss.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/nn/losses/geomloss.py` & `cyto-dl-0.1.5/cyto_dl/nn/losses/geomloss.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/nn/losses/loss_wrapper.py` & `cyto-dl-0.1.5/cyto_dl/nn/losses/loss_wrapper.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/nn/losses/spharm_loss.py` & `cyto-dl-0.1.5/cyto_dl/nn/losses/spharm_loss.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/nn/losses/threshold_loss.py` & `cyto-dl-0.1.5/cyto_dl/nn/losses/threshold_loss.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/nn/losses/weibull.py` & `cyto-dl-0.1.5/cyto_dl/nn/losses/weibull.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/nn/losses/weighted_mse_loss.py` & `cyto-dl-0.1.5/cyto_dl/nn/losses/weighted_mse_loss.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/nn/mlp.py` & `cyto-dl-0.1.5/cyto_dl/nn/mlp.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/nn/point_cloud/dgcnn.py` & `cyto-dl-0.1.5/cyto_dl/nn/point_cloud/dgcnn.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/nn/point_cloud/folding_net.py` & `cyto-dl-0.1.5/cyto_dl/nn/point_cloud/folding_net.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/nn/point_cloud/graph_functions.py` & `cyto-dl-0.1.5/cyto_dl/nn/point_cloud/graph_functions.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/nn/point_cloud/vnn.py` & `cyto-dl-0.1.5/cyto_dl/nn/point_cloud/vnn.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/nn/res_unit.py` & `cyto-dl-0.1.5/cyto_dl/nn/res_unit.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/nn/spatial_transformer.py` & `cyto-dl-0.1.5/cyto_dl/nn/spatial_transformer.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/nn/track_sequence_predictor.py` & `cyto-dl-0.1.5/cyto_dl/nn/track_sequence_predictor.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/nn/vits/blocks/cross_attention.py` & `cyto-dl-0.1.5/cyto_dl/nn/vits/blocks/cross_attention.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/nn/vits/cross_mae.py` & `cyto-dl-0.1.5/cyto_dl/nn/vits/cross_mae.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,18 @@
 from typing import List, Optional
 
 import numpy as np
 import torch
 import torch.nn as nn
-from einops import rearrange, repeat
+from einops import rearrange
 from einops.layers.torch import Rearrange
 from timm.models.layers import trunc_normal_
 
 from cyto_dl.nn.vits.blocks import CrossAttentionBlock
-
-
-def take_indexes(sequences, indexes):
-    return torch.gather(
-        sequences, 0, repeat(indexes.to(sequences.device), "t b -> t b c", c=sequences.shape[-1])
-    )
+from cyto_dl.nn.vits.utils import take_indexes
 
 
 class CrossMAE_Decoder(torch.nn.Module):
     """Decoder inspired by [CrossMAE](https://crossmae.github.io/) where masked tokens only attend
     to visible tokens."""
 
     def __init__(
@@ -90,14 +85,16 @@
         self.init_weight()
 
     def init_weight(self):
         trunc_normal_(self.mask_token, std=0.02)
         trunc_normal_(self.pos_embedding, std=0.02)
 
     def forward(self, features, forward_indexes, backward_indexes):
+        # HACK TODO allow usage of multiple intermediate feature weights, this works when decoder is 0 layers
+        features = features.squeeze(0)
         T, B, C = features.shape
         # we could do cross attention between decoder_dim queries and encoder_dim features, but it seems to work fine having both at decoder_dim for now
         features = self.projection_norm(self.projection(features))
 
         # add cls token
         backward_indexes = torch.cat(
             [torch.zeros(1, backward_indexes.shape[1]).to(backward_indexes), backward_indexes + 1],
@@ -118,16 +115,17 @@
             dim=0,
         )
 
         # unshuffle to original positions for positional embedding so we can do cross attention during decoding
         features = take_indexes(features, backward_indexes)
         features = features + self.pos_embedding
 
-        reshuffled = take_indexes(features, forward_indexes)
-        features, masked = reshuffled[:T], reshuffled[T:]
+        # reshuffle to shuffled positions for cross attention
+        features = take_indexes(features, forward_indexes)
+        features, masked = features[:T], features[T:]
 
         masked = rearrange(masked, "t b c -> b t c")
         features = rearrange(features, "t b c -> b t c")
 
         for transformer in self.transformer:
             masked = transformer(masked, features)
```

### Comparing `cyto-dl-0.1.4/cyto_dl/nn/vits/mae.py` & `cyto-dl-0.1.5/cyto_dl/nn/vits/mae.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,165 +1,36 @@
 # modified from https://github.com/IcarusWizard/MAE/blob/main/model.py#L124
 
 from typing import List, Optional
 
 import numpy as np
 import torch
 import torch.nn as nn
-from einops import rearrange, repeat
+from einops import rearrange
 from einops.layers.torch import Rearrange
 from timm.models.layers import trunc_normal_
 from timm.models.vision_transformer import Block
 
+from cyto_dl.nn.vits.blocks import IntermediateWeigher, Patchify
 from cyto_dl.nn.vits.cross_mae import CrossMAE_Decoder
-
-
-def random_indexes(size: int):
-    forward_indexes = np.arange(size)
-    np.random.shuffle(forward_indexes)
-    backward_indexes = np.argsort(forward_indexes)
-    return forward_indexes, backward_indexes
-
-
-def take_indexes(sequences, indexes):
-    return torch.gather(
-        sequences, 0, repeat(indexes.to(sequences.device), "t b -> t b c", c=sequences.shape[-1])
-    )
-
-
-class Patchify(torch.nn.Module):
-    """Class for converting images to a masked sequence of patches with positional embeddings."""
-
-    def __init__(
-        self,
-        patch_size: List[int],
-        emb_dim: int,
-        n_patches: List[int],
-        spatial_dims: int = 3,
-        context_pixels: List[int] = [0, 0, 0],
-        input_channels: int = 1,
-    ):
-        """
-        Parameters
-        ----------
-        patch_size: List[int]
-            Size of each patch
-        emb_dim: int
-            Dimension of encoder
-        n_patches: List[int]
-            Number of patches in each spatial dimension
-        spatial_dims: int
-            Number of spatial dimensions
-        context_pixels: List[int]
-            Number of extra pixels around each patch to include in convolutional embedding to encoder dimension.
-        input_channels: int
-            Number of input channels
-        """
-        super().__init__()
-        self.n_patches = np.asarray(n_patches)
-        self.spatial_dims = spatial_dims
-
-        self.pos_embedding = torch.nn.Parameter(torch.zeros(np.prod(n_patches), 1, emb_dim))
-
-        context_pixels = context_pixels[:spatial_dims]
-        weight_size = np.asarray(patch_size) + np.round(np.array(context_pixels) * 2).astype(int)
-
-        if spatial_dims == 3:
-            self.conv = nn.Conv3d(
-                in_channels=input_channels,
-                out_channels=emb_dim,
-                kernel_size=weight_size,
-                stride=patch_size,
-                padding=context_pixels,
-            )
-            self.img2token = Rearrange("b c z y x -> (z y x) b c")
-            self.patch2img = Rearrange(
-                "(n_patch_z n_patch_y n_patch_x) b c ->  b c n_patch_z n_patch_y n_patch_x",
-                n_patch_z=n_patches[0],
-                n_patch_y=n_patches[1],
-                n_patch_x=n_patches[2],
-            )
-        elif spatial_dims == 2:
-            self.conv = nn.Conv2d(
-                in_channels=input_channels,
-                out_channels=emb_dim,
-                kernel_size=weight_size,
-                stride=patch_size,
-                padding=context_pixels,
-            )
-            self.img2token = Rearrange("b c y x -> (y x) b c")
-            self.patch2img = Rearrange(
-                "(n_patch_y n_patch_x) b c ->  b c n_patch_y n_patch_x",
-                n_patch_y=n_patches[0],
-                n_patch_x=n_patches[1],
-            )
-
-        self._init_weight()
-
-    def _init_weight(self):
-        trunc_normal_(self.pos_embedding, std=0.02)
-
-    def get_mask(self, img, n_visible_patches, num_patches):
-        B = img.shape[0]
-
-        indexes = [random_indexes(num_patches) for _ in range(B)]
-        # forward indexes : index in image -> shuffledpatch
-        forward_indexes = torch.as_tensor(
-            np.stack([i[0] for i in indexes], axis=-1), dtype=torch.long
-        )
-        # backward indexes : shuffled patch -> index in image
-        backward_indexes = torch.as_tensor(
-            np.stack([i[1] for i in indexes], axis=-1), dtype=torch.long
-        )
-
-        mask = torch.zeros(num_patches, B, 1)
-        # visible patches are first
-        mask[:n_visible_patches] = 1
-        mask = take_indexes(mask, backward_indexes)
-        mask = self.patch2img(mask)
-        # one pixel per masked patch, interpolate to size of input image
-        mask = torch.nn.functional.interpolate(
-            mask, img.shape[-self.spatial_dims :], mode="nearest"
-        )
-
-        return mask.to(img), forward_indexes, backward_indexes
-
-    def forward(self, img, mask_ratio):
-        # generate mask
-        num_patches = np.prod(self.n_patches)
-        n_visible_patches = int(num_patches * (1 - mask_ratio))
-        mask, forward_indexes, backward_indexes = self.get_mask(
-            img, n_visible_patches, num_patches
-        )
-        # generate patches
-        tokens = self.conv(img * mask)
-        tokens = self.img2token(tokens)
-        # add position embedding
-        tokens = tokens + self.pos_embedding
-        if mask_ratio > 0:
-            # extract visible patches
-            tokens = take_indexes(tokens, forward_indexes)[:n_visible_patches]
-
-        # mask is used above to mask out patches, we need to invert it for loss calculation
-        mask = (1 - mask).bool()
-
-        return tokens, mask, forward_indexes, backward_indexes
+from cyto_dl.nn.vits.utils import take_indexes
 
 
 class MAE_Encoder(torch.nn.Module):
     def __init__(
         self,
         num_patches: List[int],
         spatial_dims: int = 3,
         base_patch_size: List[int] = (16, 16, 16),
         emb_dim: Optional[int] = 192,
         num_layer: Optional[int] = 12,
         num_head: Optional[int] = 3,
         context_pixels: Optional[List[int]] = [0, 0, 0],
         input_channels: Optional[int] = 1,
+        n_intermediate_weights: Optional[int] = -1,
     ) -> None:
         """
         Parameters
         ----------
         num_patches: List[int]
             Number of patches in each dimension
         spatial_dims: int
@@ -172,37 +43,59 @@
             Number of transformer layers
         num_head: int
             Number of heads in transformer
         context_pixels: List[int]
             Number of extra pixels around each patch to include in convolutional embedding to encoder dimension.
         input_channels: int
             Number of input channels
+        weight_intermediates: bool
+            Whether to output linear combination of intermediate layers as final output like CrossMAE
         """
         super().__init__()
         self.cls_token = torch.nn.Parameter(torch.zeros(1, 1, emb_dim))
         self.patchify = Patchify(
             base_patch_size, emb_dim, num_patches, spatial_dims, context_pixels, input_channels
         )
-
-        self.transformer = torch.nn.Sequential(
-            *[Block(emb_dim, num_head) for _ in range(num_layer)]
-        )
+        weight_intermediates = n_intermediate_weights > 0
+        if weight_intermediates:
+            self.transformer = torch.nn.ModuleList(
+                [Block(emb_dim, num_head) for _ in range(num_layer)]
+            )
+        else:
+            self.transformer = torch.nn.Sequential(
+                *[Block(emb_dim, num_head) for _ in range(num_layer)]
+            )
 
         self.layer_norm = torch.nn.LayerNorm(emb_dim)
+
+        self.intermediate_weighter = (
+            IntermediateWeigher(num_layer, emb_dim, n_intermediate_weights)
+            if weight_intermediates
+            else None
+        )
         self.init_weight()
 
     def init_weight(self):
         trunc_normal_(self.cls_token, std=0.02)
 
     def forward(self, img, mask_ratio=0.75):
         patches, mask, forward_indexes, backward_indexes = self.patchify(img, mask_ratio)
         patches = torch.cat([self.cls_token.expand(-1, patches.shape[1], -1), patches], dim=0)
         patches = rearrange(patches, "t b c -> b t c")
-        features = self.layer_norm(self.transformer(patches))
-        features = rearrange(features, "b t c -> t b c")
+
+        if self.intermediate_weighter is not None:
+            intermediates = [patches]
+            for block in self.transformer:
+                patches = block(patches)
+                intermediates.append(patches)
+            features = self.layer_norm(self.intermediate_weighter(intermediates))
+            features = rearrange(features, "n b t c -> n t b c")
+        else:
+            features = self.layer_norm(self.transformer(patches))
+            features = rearrange(features, "b t c -> t b c")
         if mask_ratio > 0:
             return features, mask, forward_indexes, backward_indexes
         return features
 
 
 class MAE_Decoder(torch.nn.Module):
     def __init__(
@@ -370,14 +263,15 @@
             spatial_dims,
             base_patch_size,
             emb_dim,
             encoder_layer,
             encoder_head,
             context_pixels,
             input_channels,
+            n_intermediate_weights=-1 if not use_crossmae else decoder_layer,
         )
 
         decoder_class = MAE_Decoder
         if use_crossmae:
             decoder_class = CrossMAE_Decoder
         self.decoder = decoder_class(
             num_patches=num_patches,
```

### Comparing `cyto-dl-0.1.4/cyto_dl/point_cloud/io/read_pcloud.py` & `cyto-dl-0.1.5/cyto_dl/point_cloud/io/read_pcloud.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/train.py` & `cyto-dl-0.1.5/cyto_dl/train.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/utils/config.py` & `cyto-dl-0.1.5/cyto_dl/utils/config.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/utils/download_test_data.py` & `cyto-dl-0.1.5/cyto_dl/utils/download_test_data.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/utils/dummy_dataset.py` & `cyto-dl-0.1.5/cyto_dl/utils/dummy_dataset.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/utils/pylogger.py` & `cyto-dl-0.1.5/cyto_dl/utils/pylogger.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/utils/rich_utils.py` & `cyto-dl-0.1.5/cyto_dl/utils/rich_utils.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/utils/rotation.py` & `cyto-dl-0.1.5/cyto_dl/utils/rotation.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/utils/spharm/reconstruction.py` & `cyto-dl-0.1.5/cyto_dl/utils/spharm/reconstruction.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/utils/spharm/rotation.py` & `cyto-dl-0.1.5/cyto_dl/utils/spharm/rotation.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/cyto_dl/utils/template_utils.py` & `cyto-dl-0.1.5/cyto_dl/utils/template_utils.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/pyproject.toml` & `cyto-dl-0.1.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "pdm-pep517>=1.0.0",
     "numpy>=1.23.5",
 ]
 build-backend = "pdm.pep517.api"
 
 [project]
 name = "cyto-dl"
-version = "0.1.4"
+version = "0.1.5"
 description = "Collection of representation learning models, techniques, callbacks, utils, used to create latent variable models of cell shape, morphology and intracellular organization."
 readme = "README.md"
 authors = [
     { name = "Benji Morris", email = "benjamin.morris@alleninstitute.org" },
     { name = "Guilherme Pires", email = "guilherme.pires@alleninstitute.org" },
     { name = "Ritvik Vasan", email = "ritvik.vasan@alleninstitute.org" },
 ]
@@ -78,20 +78,20 @@
     "Ninja>=1.11.1",
     "torchio>=0.19.1",
 ]
 all = [
     "cyto-dl[equiv,spharm,s3,torchserve,pcloud]",
 ]
 test = [
-    "cyto-dl[all]",
+    "cyto-dl",
     "pytest~=7.2",
     "pytest-cov[toml]~=4.0",
 ]
 docs = [
-    "cyto-dl[all]",
+    "cyto-dl",
     "furo<=2023.3.23",
     "m2r2<=0.3.3.post2",
     "sphinx<=6.1.3",
 ]
 
 [project.urls]
 Homepage = "https://github.com/AllenCellModeling/cyto-dl"
```

### Comparing `cyto-dl-0.1.4/tests/conftest.py` & `cyto-dl-0.1.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/tests/helpers/package_available.py` & `cyto-dl-0.1.5/tests/helpers/package_available.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/tests/helpers/run_if.py` & `cyto-dl-0.1.5/tests/helpers/run_if.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/tests/resources/rand_im.tif` & `cyto-dl-0.1.5/tests/resources/rand_im.tif`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/tests/resources/train.csv` & `cyto-dl-0.1.5/tests/resources/train.csv`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/tests/test_alternating_batch_sampler.py` & `cyto-dl-0.1.5/tests/test_alternating_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/tests/test_configs.py` & `cyto-dl-0.1.5/tests/test_configs.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/tests/test_eval.py` & `cyto-dl-0.1.5/tests/test_eval.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/tests/test_mlflow_logger.py` & `cyto-dl-0.1.5/tests/test_mlflow_logger.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/tests/test_polygon_loader.py` & `cyto-dl-0.1.5/tests/test_polygon_loader.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/tests/test_train.py` & `cyto-dl-0.1.5/tests/test_train.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.4/PKG-INFO` & `cyto-dl-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyto-dl
-Version: 0.1.4
+Version: 0.1.5
 Summary: Collection of representation learning models, techniques, callbacks, utils, used to create latent variable models of cell shape, morphology and intracellular organization.
 Author-email: Benji Morris <benjamin.morris@alleninstitute.org>,Guilherme Pires <guilherme.pires@alleninstitute.org>,Ritvik Vasan <ritvik.vasan@alleninstitute.org>
 Requires-Python: >=3.8,<3.11
 Provides-Extra: all
 Provides-Extra: docs
 Provides-Extra: equiv
 Provides-Extra: pcloud
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyto-dl Version: 0.1.4 Summary: Collection of
+Metadata-Version: 2.1 Name: cyto-dl Version: 0.1.5 Summary: Collection of
 representation learning models, techniques, callbacks, utils, used to create
 latent variable models of cell shape, morphology and intracellular
 organization. Author-email: Benji Morris
 alleninstitute.org>,Guilherme Pires
 alleninstitute.org>,Ritvik Vasan
 alleninstitute.org> Requires-Python: >=3.8,<3.11 Provides-Extra: all Provides-
 Extra: docs Provides-Extra: equiv Provides-Extra: pcloud Provides-Extra: s3
```

