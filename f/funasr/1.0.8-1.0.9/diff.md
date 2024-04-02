# Comparing `tmp/funasr-1.0.8.tar.gz` & `tmp/funasr-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funasr-1.0.8.tar", last modified: Wed Feb 21 08:26:36 2024, max compression
+gzip compressed data, was "funasr-1.0.9.tar", last modified: Wed Feb 21 08:29:49 2024, max compression
```

## Comparing `funasr-1.0.8.tar` & `funasr-1.0.9.tar`

### file list

```diff
@@ -1,367 +1,367 @@
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:26:36.401245 funasr-1.0.8/
--rw-r--r--   0 zhifu      (502) staff       (20)    20490 2024-02-21 08:26:36.400995 funasr-1.0.8/PKG-INFO
--rw-r--r--   0 zhifu      (502) staff       (20)    19527 2024-02-05 02:42:05.000000 funasr-1.0.8/README.md
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:26:36.136832 funasr-1.0.8/funasr/
--rw-r--r--   0 zhifu      (502) staff       (20)     1010 2024-01-24 03:44:05.000000 funasr-1.0.8/funasr/__init__.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:26:36.149605 funasr-1.0.8/funasr/auto/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:05.000000 funasr-1.0.8/funasr/auto/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3629 2024-02-19 08:42:47.000000 funasr-1.0.8/funasr/auto/auto_frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)    21242 2024-02-21 06:46:02.000000 funasr-1.0.8/funasr/auto/auto_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)       66 2024-01-24 03:44:05.000000 funasr-1.0.8/funasr/auto/auto_tokenizer.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:26:36.171676 funasr-1.0.8/funasr/bin/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:05.000000 funasr-1.0.8/funasr/bin/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4791 2024-02-19 13:25:36.000000 funasr-1.0.8/funasr/bin/compute_audio_cmvn.py
--rw-r--r--   0 zhifu      (502) staff       (20)      882 2024-01-24 03:44:05.000000 funasr-1.0.8/funasr/bin/inference.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     8387 2024-01-24 03:44:05.000000 funasr-1.0.8/funasr/bin/tokenize_text.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7841 2024-02-20 08:49:24.000000 funasr-1.0.8/funasr/bin/train.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:26:36.172894 funasr-1.0.8/funasr/datasets/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:05.000000 funasr-1.0.8/funasr/datasets/__init__.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:26:36.176202 funasr-1.0.8/funasr/datasets/audio_datasets/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:05.000000 funasr-1.0.8/funasr/datasets/audio_datasets/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3727 2024-02-19 12:29:57.000000 funasr-1.0.8/funasr/datasets/audio_datasets/datasets.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4767 2024-02-17 09:59:57.000000 funasr-1.0.8/funasr/datasets/audio_datasets/index_ds.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1420 2024-02-20 09:39:14.000000 funasr-1.0.8/funasr/datasets/audio_datasets/preprocessor.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10756 2024-02-06 13:23:23.000000 funasr-1.0.8/funasr/datasets/audio_datasets/samplers.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3506 2024-02-19 08:51:10.000000 funasr-1.0.8/funasr/datasets/audio_datasets/scp2jsonl.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:26:36.179039 funasr-1.0.8/funasr/download/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:05.000000 funasr-1.0.8/funasr/download/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      455 2024-02-16 15:18:51.000000 funasr-1.0.8/funasr/download/download_dataset_from_hub.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4516 2024-02-20 10:38:43.000000 funasr-1.0.8/funasr/download/download_from_hub.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10841 2024-01-24 03:44:05.000000 funasr-1.0.8/funasr/download/file.py
--rw-r--r--   0 zhifu      (502) staff       (20)      778 2024-01-24 03:44:05.000000 funasr-1.0.8/funasr/download/name_maps_from_hub.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2088 2024-01-24 03:44:05.000000 funasr-1.0.8/funasr/download/runtime_sdk_download_tool.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:26:36.181518 funasr-1.0.8/funasr/frontends/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:05.000000 funasr-1.0.8/funasr/frontends/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12449 2024-01-24 03:44:05.000000 funasr-1.0.8/funasr/frontends/default.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1405 2024-01-24 03:44:05.000000 funasr-1.0.8/funasr/frontends/eend_ola_feature.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5625 2024-01-24 03:44:05.000000 funasr-1.0.8/funasr/frontends/fused.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4796 2024-01-24 03:44:05.000000 funasr-1.0.8/funasr/frontends/s3prl.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:26:36.186166 funasr-1.0.8/funasr/frontends/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)       30 2024-01-24 03:44:05.000000 funasr-1.0.8/funasr/frontends/utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2731 2024-01-24 03:44:05.000000 funasr-1.0.8/funasr/frontends/utils/beamformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6789 2024-01-24 03:44:05.000000 funasr-1.0.8/funasr/frontends/utils/complex_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5532 2024-01-24 03:44:05.000000 funasr-1.0.8/funasr/frontends/utils/dnn_beamformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2840 2024-01-24 03:44:05.000000 funasr-1.0.8/funasr/frontends/utils/dnn_wpe.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7975 2024-01-24 03:44:05.000000 funasr-1.0.8/funasr/frontends/utils/feature_transform.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4581 2024-01-24 03:44:05.000000 funasr-1.0.8/funasr/frontends/utils/frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2581 2024-01-24 03:44:05.000000 funasr-1.0.8/funasr/frontends/utils/log_mel.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2695 2024-01-24 03:44:05.000000 funasr-1.0.8/funasr/frontends/utils/mask_estimator.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8361 2024-01-24 03:44:05.000000 funasr-1.0.8/funasr/frontends/utils/stft.py
--rw-r--r--   0 zhifu      (502) staff       (20)    20355 2024-02-19 13:37:03.000000 funasr-1.0.8/funasr/frontends/wav_frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2690 2024-01-24 03:44:05.000000 funasr-1.0.8/funasr/frontends/windowing.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:26:36.186636 funasr-1.0.8/funasr/losses/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:05.000000 funasr-1.0.8/funasr/losses/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4367 2024-01-24 03:44:05.000000 funasr-1.0.8/funasr/losses/label_smoothing_loss.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:26:36.201761 funasr-1.0.8/funasr/metrics/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:05.000000 funasr-1.0.8/funasr/metrics/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8572 2024-01-24 03:44:05.000000 funasr-1.0.8/funasr/metrics/common.py
--rw-r--r--   0 zhifu      (502) staff       (20)      699 2024-01-24 03:44:05.000000 funasr-1.0.8/funasr/metrics/compute_acc.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2078 2024-01-24 03:44:05.000000 funasr-1.0.8/funasr/metrics/compute_eer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6714 2024-01-24 03:44:05.000000 funasr-1.0.8/funasr/metrics/compute_min_dcf.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     5189 2024-01-24 03:44:05.000000 funasr-1.0.8/funasr/metrics/compute_wer.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:26:36.202454 funasr-1.0.8/funasr/models/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:05.000000 funasr-1.0.8/funasr/models/__init__.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:26:36.208102 funasr-1.0.8/funasr/models/bat/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:05.000000 funasr-1.0.8/funasr/models/bat/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8239 2024-01-24 03:44:05.000000 funasr-1.0.8/funasr/models/bat/attention.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8724 2024-01-24 03:44:05.000000 funasr-1.0.8/funasr/models/bat/cif_predictor.py
--rw-r--r--   0 zhifu      (502) staff       (20)    22042 2024-01-24 03:44:05.000000 funasr-1.0.8/funasr/models/bat/conformer_chunk_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    16711 2024-01-24 03:44:05.000000 funasr-1.0.8/funasr/models/bat/model.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:26:36.215533 funasr-1.0.8/funasr/models/bicif_paraformer/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:05.000000 funasr-1.0.8/funasr/models/bicif_paraformer/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    15354 2024-01-24 03:44:05.000000 funasr-1.0.8/funasr/models/bicif_paraformer/cif_predictor.py
--rw-r--r--   0 zhifu      (502) staff       (20)    15296 2024-02-21 05:03:32.000000 funasr-1.0.8/funasr/models/bicif_paraformer/model.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:26:36.218188 funasr-1.0.8/funasr/models/branchformer/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:05.000000 funasr-1.0.8/funasr/models/branchformer/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3508 2024-01-24 03:44:05.000000 funasr-1.0.8/funasr/models/branchformer/cgmlp.py
--rw-r--r--   0 zhifu      (502) staff       (20)    20859 2024-01-24 03:44:05.000000 funasr-1.0.8/funasr/models/branchformer/encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5282 2024-01-24 03:44:05.000000 funasr-1.0.8/funasr/models/branchformer/fastformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)      360 2024-01-24 03:44:05.000000 funasr-1.0.8/funasr/models/branchformer/model.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:26:36.237374 funasr-1.0.8/funasr/models/campplus/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:05.000000 funasr-1.0.8/funasr/models/campplus/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6329 2024-01-26 01:59:39.000000 funasr-1.0.8/funasr/models/campplus/cluster_backend.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10878 2024-01-24 03:44:05.000000 funasr-1.0.8/funasr/models/campplus/components.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4911 2024-02-06 13:23:23.000000 funasr-1.0.8/funasr/models/campplus/model.py
--rw-r--r--   0 zhifu      (502) staff       (20)    17199 2024-01-31 02:30:07.000000 funasr-1.0.8/funasr/models/campplus/utils.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:26:36.239148 funasr-1.0.8/funasr/models/conformer/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:05.000000 funasr-1.0.8/funasr/models/conformer/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    45295 2024-02-20 06:05:58.000000 funasr-1.0.8/funasr/models/conformer/encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)      373 2024-01-24 03:44:05.000000 funasr-1.0.8/funasr/models/conformer/model.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:26:36.240604 funasr-1.0.8/funasr/models/contextual_paraformer/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/contextual_paraformer/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    41044 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/contextual_paraformer/decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    23074 2024-02-21 05:05:12.000000 funasr-1.0.8/funasr/models/contextual_paraformer/model.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:26:36.241658 funasr-1.0.8/funasr/models/ct_transformer/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/ct_transformer/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    14884 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/ct_transformer/model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3023 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/ct_transformer/utils.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:26:36.243493 funasr-1.0.8/funasr/models/ct_transformer_streaming/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/ct_transformer_streaming/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      851 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/ct_transformer_streaming/attention.py
--rw-r--r--   0 zhifu      (502) staff       (20)    14574 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/ct_transformer_streaming/encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7044 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/ct_transformer_streaming/model.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:26:36.245117 funasr-1.0.8/funasr/models/ctc/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/ctc/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6286 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/ctc/ctc.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:26:36.248843 funasr-1.0.8/funasr/models/data2vec/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/data2vec/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5157 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/data2vec/data2vec.py
--rw-r--r--   0 zhifu      (502) staff       (20)    20866 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/data2vec/data2vec_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5833 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/data2vec/data_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4474 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/data2vec/ema_module.py
--rw-r--r--   0 zhifu      (502) staff       (20)      442 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/data2vec/grad_multiply.py
--rw-r--r--   0 zhifu      (502) staff       (20)    26457 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/data2vec/multihead_attention.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4021 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/data2vec/quant_noise.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4857 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/data2vec/utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12732 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/data2vec/wav2vec2.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:26:36.249647 funasr-1.0.8/funasr/models/e_branchformer/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/e_branchformer/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    17193 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/e_branchformer/encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)      362 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/e_branchformer/model.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:26:36.250981 funasr-1.0.8/funasr/models/eend/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/eend/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9482 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/eend/e2e_diar_eend_ola.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1875 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/eend/eend_ola_dataloader.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4766 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/eend/encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2768 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/eend/encoder_decoder_attractor.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:26:36.252583 funasr-1.0.8/funasr/models/eend/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/eend/utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9352 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/eend/utils/feature.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5230 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/eend/utils/kaldi_data.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1447 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/eend/utils/losses.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3386 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/eend/utils/power.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7331 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/eend/utils/report.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:26:36.277965 funasr-1.0.8/funasr/models/emotion2vec/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/emotion2vec/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5556 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/emotion2vec/audio.py
--rw-r--r--   0 zhifu      (502) staff       (20)    20985 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/emotion2vec/base.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9535 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/emotion2vec/fairseq_modules.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9052 2024-01-31 02:30:07.000000 funasr-1.0.8/funasr/models/emotion2vec/model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9339 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/emotion2vec/modules.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3203 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/emotion2vec/timm_modules.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:26:36.279550 funasr-1.0.8/funasr/models/eres2net/
--rw-r--r--   0 zhifu      (502) staff       (20)       69 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/eres2net/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    15424 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/eres2net/eres2net.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10188 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/eres2net/eres2net_aug.py
--rw-r--r--   0 zhifu      (502) staff       (20)      948 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/eres2net/fusion.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:26:36.283975 funasr-1.0.8/funasr/models/fsmn_vad_streaming/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/fsmn_vad_streaming/__init__.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     9361 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/fsmn_vad_streaming/encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    32489 2024-02-21 05:05:30.000000 funasr-1.0.8/funasr/models/fsmn_vad_streaming/model.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:26:36.289970 funasr-1.0.8/funasr/models/language_model/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/language_model/__init__.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:26:36.294942 funasr-1.0.8/funasr/models/language_model/rnn/
--rw-r--r--   0 zhifu      (502) staff       (20)       30 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/language_model/rnn/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4080 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/language_model/rnn/argument.py
--rw-r--r--   0 zhifu      (502) staff       (20)    67021 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/language_model/rnn/attentions.py
--rw-r--r--   0 zhifu      (502) staff       (20)    49489 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/language_model/rnn/decoders.py
--rw-r--r--   0 zhifu      (502) staff       (20)    14206 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/language_model/rnn/encoders.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5825 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/language_model/seq_rnn_lm.py
--rw-r--r--   0 zhifu      (502) staff       (20)    18578 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/language_model/transformer_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4274 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/language_model/transformer_lm.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:26:36.296563 funasr-1.0.8/funasr/models/lora/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/lora/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12553 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/lora/layers.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1839 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/lora/utils.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:26:36.300035 funasr-1.0.8/funasr/models/mfcca/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/mfcca/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11761 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/mfcca/e2e_asr_mfcca.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10175 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/mfcca/encoder_layer_mfcca.py
--rw-r--r--   0 zhifu      (502) staff       (20)    17831 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/mfcca/mfcca_encoder.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:26:36.302548 funasr-1.0.8/funasr/models/model_hf/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-02-19 02:44:52.000000 funasr-1.0.8/funasr/models/model_hf/__init__.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:26:36.303394 funasr-1.0.8/funasr/models/monotonic_aligner/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/monotonic_aligner/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9334 2024-02-21 05:07:59.000000 funasr-1.0.8/funasr/models/monotonic_aligner/model.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:26:36.309852 funasr-1.0.8/funasr/models/mossformer/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/mossformer/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2847 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/mossformer/e2e_ss.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10105 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/mossformer/mossformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1341 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/mossformer/mossformer_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11905 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/mossformer/mossformer_encoder.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:26:36.315386 funasr-1.0.8/funasr/models/normalize/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/normalize/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3382 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/normalize/global_mvn.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2283 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/normalize/utterance_mvn.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:26:36.321456 funasr-1.0.8/funasr/models/paraformer/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/paraformer/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    24197 2024-02-06 13:23:23.000000 funasr-1.0.8/funasr/models/paraformer/cif_predictor.py
--rw-r--r--   0 zhifu      (502) staff       (20)    24451 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/paraformer/decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    22824 2024-02-21 05:02:24.000000 funasr-1.0.8/funasr/models/paraformer/model.py
--rw-r--r--   0 zhifu      (502) staff       (20)    17203 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/paraformer/search.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:26:36.325355 funasr-1.0.8/funasr/models/paraformer_streaming/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/paraformer_streaming/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    28218 2024-02-21 05:07:59.000000 funasr-1.0.8/funasr/models/paraformer_streaming/model.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:26:36.330308 funasr-1.0.8/funasr/models/rwkv_bat/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/rwkv_bat/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/rwkv_bat/model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4700 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/rwkv_bat/rwkv.py
--rw-r--r--   0 zhifu      (502) staff       (20)    19560 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/rwkv_bat/rwkv_attention.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4840 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/rwkv_bat/rwkv_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3129 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/rwkv_bat/rwkv_feed_forward.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7246 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/rwkv_bat/rwkv_subsampling.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:26:36.333374 funasr-1.0.8/funasr/models/sa_asr/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/sa_asr/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1693 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/sa_asr/attention.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)    20122 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/sa_asr/beam_search_sa_asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)    18881 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/sa_asr/e2e_sa_asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)    28869 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/sa_asr/transformer_decoder.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:26:36.337077 funasr-1.0.8/funasr/models/sanm/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/sanm/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    25896 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/sanm/attention.py
--rw-r--r--   0 zhifu      (502) staff       (20)    18407 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/sanm/decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    17622 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/sanm/encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)      692 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/sanm/model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1078 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/sanm/positionwise_feed_forward.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:26:36.345791 funasr-1.0.8/funasr/models/scama/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/scama/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    37307 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/scama/beam_search.py
--rw-r--r--   0 zhifu      (502) staff       (20)    19965 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/scama/chunk_utilis.py
--rw-r--r--   0 zhifu      (502) staff       (20)    42404 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/scama/decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    28398 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/scama/encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    29216 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/scama/model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2586 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/scama/utils.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:26:36.346458 funasr-1.0.8/funasr/models/seaco_paraformer/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/seaco_paraformer/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    25738 2024-02-21 06:46:02.000000 funasr-1.0.8/funasr/models/seaco_paraformer/model.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:26:36.348152 funasr-1.0.8/funasr/models/sond/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/sond/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12324 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/sond/attention.py
--rw-r--r--   0 zhifu      (502) staff       (20)    23635 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/sond/e2e_diar_sond.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:26:36.351278 funasr-1.0.8/funasr/models/sond/encoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/sond/encoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      909 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/sond/encoder/ci_scorers.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11010 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/sond/encoder/conv_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    19855 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/sond/encoder/ecapa_tdnn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13990 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/sond/encoder/fsmn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    41076 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/sond/encoder/resnet34_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    21259 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/sond/encoder/self_attention_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3330 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/sond/label_aggregation.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:26:36.352320 funasr-1.0.8/funasr/models/sond/pooling/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/sond/pooling/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3785 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/sond/pooling/pooling_layers.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3567 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/sond/pooling/statistic_pooling.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1389 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/sond/sv_decoder.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:26:36.354194 funasr-1.0.8/funasr/models/specaug/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/specaug/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10331 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/specaug/mask_along_axis.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6110 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/specaug/profileaug.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6734 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/specaug/specaug.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2530 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/specaug/time_warp.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:26:36.356892 funasr-1.0.8/funasr/models/transducer/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/transducer/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    23148 2024-02-20 06:05:58.000000 funasr-1.0.8/funasr/models/transducer/beam_search_transducer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2112 2024-02-20 06:05:58.000000 funasr-1.0.8/funasr/models/transducer/joint_network.py
--rw-r--r--   0 zhifu      (502) staff       (20)    19120 2024-02-21 05:09:56.000000 funasr-1.0.8/funasr/models/transducer/model.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12243 2024-02-20 06:05:58.000000 funasr-1.0.8/funasr/models/transducer/rnn_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8500 2024-02-20 06:05:58.000000 funasr-1.0.8/funasr/models/transducer/rnnt_decoder.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:26:36.360984 funasr-1.0.8/funasr/models/transformer/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/transformer/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    19728 2024-02-20 06:05:58.000000 funasr-1.0.8/funasr/models/transformer/attention.py
--rw-r--r--   0 zhifu      (502) staff       (20)    24724 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/transformer/decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    18442 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/transformer/embedding.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13124 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/transformer/encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5156 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/transformer/layer_norm.py
--rw-r--r--   0 zhifu      (502) staff       (20)    17052 2024-02-21 05:09:05.000000 funasr-1.0.8/funasr/models/transformer/model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1045 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/transformer/positionwise_feed_forward.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:26:36.363260 funasr-1.0.8/funasr/models/transformer/scorers/
--rw-r--r--   0 zhifu      (502) staff       (20)       30 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/transformer/scorers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5059 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/transformer/scorers/ctc.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13951 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/transformer/scorers/ctc_prefix_score.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1798 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/transformer/scorers/length_bonus.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5938 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/transformer/scorers/scorer_interface.py
--rw-r--r--   0 zhifu      (502) staff       (20)    17315 2024-02-05 02:42:05.000000 funasr-1.0.8/funasr/models/transformer/search.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:26:36.369445 funasr-1.0.8/funasr/models/transformer/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/transformer/utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      957 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/transformer/utils/add_sos_eos.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4244 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/transformer/utils/dynamic_conv.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4863 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/transformer/utils/dynamic_conv2d.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3590 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/transformer/utils/lightconv.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4230 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/transformer/utils/lightconv2d.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1654 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/transformer/utils/mask.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4800 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/transformer/utils/multi_layer_conv.py
--rw-r--r--   0 zhifu      (502) staff       (20)    23561 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/transformer/utils/nets_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4294 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/transformer/utils/repeat.py
--rw-r--r--   0 zhifu      (502) staff       (20)    21882 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/transformer/utils/subsampling.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1898 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/transformer/utils/subsampling_without_posenc.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2782 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/transformer/utils/vgg2l.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:26:36.370616 funasr-1.0.8/funasr/models/uniasr/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/uniasr/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    19037 2024-01-24 09:01:27.000000 funasr-1.0.8/funasr/models/uniasr/beam_search.py
--rw-r--r--   0 zhifu      (502) staff       (20)    44328 2024-01-24 09:01:27.000000 funasr-1.0.8/funasr/models/uniasr/model.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:26:36.371168 funasr-1.0.8/funasr/models/whisper/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/whisper/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9882 2024-02-05 02:42:05.000000 funasr-1.0.8/funasr/models/whisper/model.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:26:36.373332 funasr-1.0.8/funasr/models/whisper/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/whisper/utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4214 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/whisper/utils/audio.py
--rw-r--r--   0 zhifu      (502) staff       (20)    30110 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/whisper/utils/decoding.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10100 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/whisper/utils/tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    16176 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/whisper/utils/transcribe.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5226 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/whisper/utils/utils.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:26:36.373872 funasr-1.0.8/funasr/models/xvector/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/xvector/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10000 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/models/xvector/e2e_sv.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:26:36.375456 funasr-1.0.8/funasr/optimizers/
--rw-r--r--   0 zhifu      (502) staff       (20)      446 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/optimizers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5643 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/optimizers/fairseq_adam.py
--rw-r--r--   0 zhifu      (502) staff       (20)      747 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/optimizers/sgd.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3226 2024-02-17 08:45:57.000000 funasr-1.0.8/funasr/register.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:26:36.376682 funasr-1.0.8/funasr/schedulers/
--rw-r--r--   0 zhifu      (502) staff       (20)      852 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/schedulers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1679 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/schedulers/abs_scheduler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1986 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/schedulers/noam_lr.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3577 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/schedulers/tri_stage_scheduler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1413 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/schedulers/warmup_lr.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:26:36.386299 funasr-1.0.8/funasr/tokenizer/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/tokenizer/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3463 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/tokenizer/abs_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2153 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/tokenizer/build_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3034 2024-02-20 03:45:18.000000 funasr-1.0.8/funasr/tokenizer/char_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1423 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/tokenizer/cleaner.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1968 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/tokenizer/korean_cleaner.py
--rw-r--r--   0 zhifu      (502) staff       (20)    16530 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/tokenizer/phoneme_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1674 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/tokenizer/sentencepiece_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2019 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/tokenizer/token_id_converter.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1998 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/tokenizer/word_tokenizer.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:26:36.390358 funasr-1.0.8/funasr/train_utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/train_utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      987 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/train_utils/add_gradient_noise.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7007 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/train_utils/average_nbest_models.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2681 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/train_utils/device_funcs.py
--rw-r--r--   0 zhifu      (502) staff       (20)      971 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/train_utils/forward_adaptor.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1930 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/train_utils/initialize.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4341 2024-02-21 06:46:59.000000 funasr-1.0.8/funasr/train_utils/load_pretrained_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2275 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/train_utils/model_summary.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1615 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/train_utils/recursive_op.py
--rw-r--r--   0 zhifu      (502) staff       (20)      167 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/train_utils/set_all_random_seed.py
--rw-r--r--   0 zhifu      (502) staff       (20)    17108 2024-02-21 08:25:50.000000 funasr-1.0.8/funasr/train_utils/trainer.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:26:36.397051 funasr-1.0.8/funasr/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2145 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/utils/datadir_writer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4941 2024-01-30 06:21:05.000000 funasr-1.0.8/funasr/utils/load_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1609 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/utils/misc.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9218 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/utils/postprocess_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10757 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/utils/prepare_data.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6761 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/utils/speaker_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6558 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/utils/timestamp_tools.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4185 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/utils/types.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1202 2024-01-24 03:44:06.000000 funasr-1.0.8/funasr/utils/vad_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)        6 2024-02-21 08:26:21.000000 funasr-1.0.8/funasr/version.txt
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:26:36.144104 funasr-1.0.8/funasr.egg-info/
--rw-r--r--   0 zhifu      (502) staff       (20)    20490 2024-02-21 08:26:36.000000 funasr-1.0.8/funasr.egg-info/PKG-INFO
--rw-r--r--   0 zhifu      (502) staff       (20)    11155 2024-02-21 08:26:36.000000 funasr-1.0.8/funasr.egg-info/SOURCES.txt
--rw-r--r--   0 zhifu      (502) staff       (20)        1 2024-02-21 08:26:36.000000 funasr-1.0.8/funasr.egg-info/dependency_links.txt
--rw-r--r--   0 zhifu      (502) staff       (20)       59 2024-02-21 08:26:36.000000 funasr-1.0.8/funasr.egg-info/entry_points.txt
--rw-r--r--   0 zhifu      (502) staff       (20)      664 2024-02-21 08:26:36.000000 funasr-1.0.8/funasr.egg-info/requires.txt
--rw-r--r--   0 zhifu      (502) staff       (20)        7 2024-02-21 08:26:36.000000 funasr-1.0.8/funasr.egg-info/top_level.txt
--rw-r--r--   0 zhifu      (502) staff       (20)       38 2024-02-21 08:26:36.401370 funasr-1.0.8/setup.cfg
--rw-r--r--   0 zhifu      (502) staff       (20)     3832 2024-02-19 08:43:24.000000 funasr-1.0.8/setup.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:26:36.400277 funasr-1.0.8/tests/
--rw-r--r--   0 zhifu      (502) staff       (20)    27007 2024-01-24 03:44:06.000000 funasr-1.0.8/tests/test_asr_inference_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1310 2024-01-24 03:44:06.000000 funasr-1.0.8/tests/test_asr_vad_punc_inference_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)      804 2024-01-24 03:44:06.000000 funasr-1.0.8/tests/test_lm_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2055 2024-01-24 03:44:06.000000 funasr-1.0.8/tests/test_punctuation_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1583 2024-01-24 03:44:06.000000 funasr-1.0.8/tests/test_sv_inference_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1741 2024-01-24 03:44:06.000000 funasr-1.0.8/tests/test_tp_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2298 2024-01-24 03:44:06.000000 funasr-1.0.8/tests/test_vad_inference_pipeline.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:29:49.897737 funasr-1.0.9/
+-rw-r--r--   0 zhifu      (502) staff       (20)    20490 2024-02-21 08:29:49.897470 funasr-1.0.9/PKG-INFO
+-rw-r--r--   0 zhifu      (502) staff       (20)    19527 2024-02-05 02:42:05.000000 funasr-1.0.9/README.md
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:29:49.741392 funasr-1.0.9/funasr/
+-rw-r--r--   0 zhifu      (502) staff       (20)     1010 2024-01-24 03:44:05.000000 funasr-1.0.9/funasr/__init__.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:29:49.744598 funasr-1.0.9/funasr/auto/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:05.000000 funasr-1.0.9/funasr/auto/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3629 2024-02-19 08:42:47.000000 funasr-1.0.9/funasr/auto/auto_frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    21560 2024-02-21 08:28:58.000000 funasr-1.0.9/funasr/auto/auto_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)       66 2024-01-24 03:44:05.000000 funasr-1.0.9/funasr/auto/auto_tokenizer.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:29:49.746490 funasr-1.0.9/funasr/bin/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:05.000000 funasr-1.0.9/funasr/bin/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4791 2024-02-19 13:25:36.000000 funasr-1.0.9/funasr/bin/compute_audio_cmvn.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      882 2024-01-24 03:44:05.000000 funasr-1.0.9/funasr/bin/inference.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     8387 2024-01-24 03:44:05.000000 funasr-1.0.9/funasr/bin/tokenize_text.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7841 2024-02-20 08:49:24.000000 funasr-1.0.9/funasr/bin/train.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:29:49.746846 funasr-1.0.9/funasr/datasets/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:05.000000 funasr-1.0.9/funasr/datasets/__init__.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:29:49.750222 funasr-1.0.9/funasr/datasets/audio_datasets/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:05.000000 funasr-1.0.9/funasr/datasets/audio_datasets/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3727 2024-02-19 12:29:57.000000 funasr-1.0.9/funasr/datasets/audio_datasets/datasets.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4767 2024-02-17 09:59:57.000000 funasr-1.0.9/funasr/datasets/audio_datasets/index_ds.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1420 2024-02-20 09:39:14.000000 funasr-1.0.9/funasr/datasets/audio_datasets/preprocessor.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10756 2024-02-06 13:23:23.000000 funasr-1.0.9/funasr/datasets/audio_datasets/samplers.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3506 2024-02-19 08:51:10.000000 funasr-1.0.9/funasr/datasets/audio_datasets/scp2jsonl.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:29:49.755975 funasr-1.0.9/funasr/download/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:05.000000 funasr-1.0.9/funasr/download/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      455 2024-02-16 15:18:51.000000 funasr-1.0.9/funasr/download/download_dataset_from_hub.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4516 2024-02-20 10:38:43.000000 funasr-1.0.9/funasr/download/download_from_hub.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10841 2024-01-24 03:44:05.000000 funasr-1.0.9/funasr/download/file.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      778 2024-01-24 03:44:05.000000 funasr-1.0.9/funasr/download/name_maps_from_hub.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2088 2024-01-24 03:44:05.000000 funasr-1.0.9/funasr/download/runtime_sdk_download_tool.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:29:49.758679 funasr-1.0.9/funasr/frontends/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:05.000000 funasr-1.0.9/funasr/frontends/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12449 2024-01-24 03:44:05.000000 funasr-1.0.9/funasr/frontends/default.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1405 2024-01-24 03:44:05.000000 funasr-1.0.9/funasr/frontends/eend_ola_feature.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5625 2024-01-24 03:44:05.000000 funasr-1.0.9/funasr/frontends/fused.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4796 2024-01-24 03:44:05.000000 funasr-1.0.9/funasr/frontends/s3prl.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:29:49.762499 funasr-1.0.9/funasr/frontends/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)       30 2024-01-24 03:44:05.000000 funasr-1.0.9/funasr/frontends/utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2731 2024-01-24 03:44:05.000000 funasr-1.0.9/funasr/frontends/utils/beamformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6789 2024-01-24 03:44:05.000000 funasr-1.0.9/funasr/frontends/utils/complex_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5532 2024-01-24 03:44:05.000000 funasr-1.0.9/funasr/frontends/utils/dnn_beamformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2840 2024-01-24 03:44:05.000000 funasr-1.0.9/funasr/frontends/utils/dnn_wpe.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7975 2024-01-24 03:44:05.000000 funasr-1.0.9/funasr/frontends/utils/feature_transform.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4581 2024-01-24 03:44:05.000000 funasr-1.0.9/funasr/frontends/utils/frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2581 2024-01-24 03:44:05.000000 funasr-1.0.9/funasr/frontends/utils/log_mel.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2695 2024-01-24 03:44:05.000000 funasr-1.0.9/funasr/frontends/utils/mask_estimator.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8361 2024-01-24 03:44:05.000000 funasr-1.0.9/funasr/frontends/utils/stft.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    20355 2024-02-19 13:37:03.000000 funasr-1.0.9/funasr/frontends/wav_frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2690 2024-01-24 03:44:05.000000 funasr-1.0.9/funasr/frontends/windowing.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:29:49.762974 funasr-1.0.9/funasr/losses/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:05.000000 funasr-1.0.9/funasr/losses/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4367 2024-01-24 03:44:05.000000 funasr-1.0.9/funasr/losses/label_smoothing_loss.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:29:49.764908 funasr-1.0.9/funasr/metrics/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:05.000000 funasr-1.0.9/funasr/metrics/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8572 2024-01-24 03:44:05.000000 funasr-1.0.9/funasr/metrics/common.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      699 2024-01-24 03:44:05.000000 funasr-1.0.9/funasr/metrics/compute_acc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2078 2024-01-24 03:44:05.000000 funasr-1.0.9/funasr/metrics/compute_eer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6714 2024-01-24 03:44:05.000000 funasr-1.0.9/funasr/metrics/compute_min_dcf.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     5189 2024-01-24 03:44:05.000000 funasr-1.0.9/funasr/metrics/compute_wer.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:29:49.765185 funasr-1.0.9/funasr/models/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:05.000000 funasr-1.0.9/funasr/models/__init__.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:29:49.766711 funasr-1.0.9/funasr/models/bat/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:05.000000 funasr-1.0.9/funasr/models/bat/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8239 2024-01-24 03:44:05.000000 funasr-1.0.9/funasr/models/bat/attention.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8724 2024-01-24 03:44:05.000000 funasr-1.0.9/funasr/models/bat/cif_predictor.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    22042 2024-01-24 03:44:05.000000 funasr-1.0.9/funasr/models/bat/conformer_chunk_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    16711 2024-01-24 03:44:05.000000 funasr-1.0.9/funasr/models/bat/model.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:29:49.767645 funasr-1.0.9/funasr/models/bicif_paraformer/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:05.000000 funasr-1.0.9/funasr/models/bicif_paraformer/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    15354 2024-01-24 03:44:05.000000 funasr-1.0.9/funasr/models/bicif_paraformer/cif_predictor.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    15296 2024-02-21 05:03:32.000000 funasr-1.0.9/funasr/models/bicif_paraformer/model.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:29:49.769748 funasr-1.0.9/funasr/models/branchformer/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:05.000000 funasr-1.0.9/funasr/models/branchformer/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3508 2024-01-24 03:44:05.000000 funasr-1.0.9/funasr/models/branchformer/cgmlp.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    20859 2024-01-24 03:44:05.000000 funasr-1.0.9/funasr/models/branchformer/encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5282 2024-01-24 03:44:05.000000 funasr-1.0.9/funasr/models/branchformer/fastformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      360 2024-01-24 03:44:05.000000 funasr-1.0.9/funasr/models/branchformer/model.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:29:49.771571 funasr-1.0.9/funasr/models/campplus/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:05.000000 funasr-1.0.9/funasr/models/campplus/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6329 2024-01-26 01:59:39.000000 funasr-1.0.9/funasr/models/campplus/cluster_backend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10878 2024-01-24 03:44:05.000000 funasr-1.0.9/funasr/models/campplus/components.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4911 2024-02-06 13:23:23.000000 funasr-1.0.9/funasr/models/campplus/model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    17199 2024-01-31 02:30:07.000000 funasr-1.0.9/funasr/models/campplus/utils.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:29:49.773199 funasr-1.0.9/funasr/models/conformer/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:05.000000 funasr-1.0.9/funasr/models/conformer/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    45295 2024-02-20 06:05:58.000000 funasr-1.0.9/funasr/models/conformer/encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      373 2024-01-24 03:44:05.000000 funasr-1.0.9/funasr/models/conformer/model.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:29:49.774344 funasr-1.0.9/funasr/models/contextual_paraformer/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/contextual_paraformer/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    41044 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/contextual_paraformer/decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    23074 2024-02-21 05:05:12.000000 funasr-1.0.9/funasr/models/contextual_paraformer/model.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:29:49.775557 funasr-1.0.9/funasr/models/ct_transformer/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/ct_transformer/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    14884 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/ct_transformer/model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3023 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/ct_transformer/utils.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:29:49.776777 funasr-1.0.9/funasr/models/ct_transformer_streaming/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/ct_transformer_streaming/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      851 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/ct_transformer_streaming/attention.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    14574 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/ct_transformer_streaming/encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7044 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/ct_transformer_streaming/model.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:29:49.777201 funasr-1.0.9/funasr/models/ctc/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/ctc/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6286 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/ctc/ctc.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:29:49.780746 funasr-1.0.9/funasr/models/data2vec/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/data2vec/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5157 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/data2vec/data2vec.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    20866 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/data2vec/data2vec_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5833 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/data2vec/data_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4474 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/data2vec/ema_module.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      442 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/data2vec/grad_multiply.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    26457 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/data2vec/multihead_attention.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4021 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/data2vec/quant_noise.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4857 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/data2vec/utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12732 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/data2vec/wav2vec2.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:29:49.781580 funasr-1.0.9/funasr/models/e_branchformer/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/e_branchformer/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    17193 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/e_branchformer/encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      362 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/e_branchformer/model.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:29:49.782899 funasr-1.0.9/funasr/models/eend/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/eend/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9482 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/eend/e2e_diar_eend_ola.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1875 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/eend/eend_ola_dataloader.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4766 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/eend/encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2768 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/eend/encoder_decoder_attractor.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:29:49.785477 funasr-1.0.9/funasr/models/eend/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/eend/utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9352 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/eend/utils/feature.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5230 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/eend/utils/kaldi_data.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1447 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/eend/utils/losses.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3386 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/eend/utils/power.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7331 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/eend/utils/report.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:29:49.787485 funasr-1.0.9/funasr/models/emotion2vec/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/emotion2vec/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5556 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/emotion2vec/audio.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    20985 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/emotion2vec/base.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9535 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/emotion2vec/fairseq_modules.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9052 2024-01-31 02:30:07.000000 funasr-1.0.9/funasr/models/emotion2vec/model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9339 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/emotion2vec/modules.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3203 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/emotion2vec/timm_modules.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:29:49.788553 funasr-1.0.9/funasr/models/eres2net/
+-rw-r--r--   0 zhifu      (502) staff       (20)       69 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/eres2net/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    15424 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/eres2net/eres2net.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10188 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/eres2net/eres2net_aug.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      948 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/eres2net/fusion.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:29:49.789354 funasr-1.0.9/funasr/models/fsmn_vad_streaming/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/fsmn_vad_streaming/__init__.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     9361 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/fsmn_vad_streaming/encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    32489 2024-02-21 05:05:30.000000 funasr-1.0.9/funasr/models/fsmn_vad_streaming/model.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:29:49.792070 funasr-1.0.9/funasr/models/language_model/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/language_model/__init__.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:29:49.794668 funasr-1.0.9/funasr/models/language_model/rnn/
+-rw-r--r--   0 zhifu      (502) staff       (20)       30 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/language_model/rnn/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4080 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/language_model/rnn/argument.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    67021 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/language_model/rnn/attentions.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    49489 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/language_model/rnn/decoders.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    14206 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/language_model/rnn/encoders.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5825 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/language_model/seq_rnn_lm.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    18578 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/language_model/transformer_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4274 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/language_model/transformer_lm.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:29:49.796180 funasr-1.0.9/funasr/models/lora/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/lora/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12553 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/lora/layers.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1839 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/lora/utils.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:29:49.800544 funasr-1.0.9/funasr/models/mfcca/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/mfcca/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11761 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/mfcca/e2e_asr_mfcca.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10175 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/mfcca/encoder_layer_mfcca.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    17831 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/mfcca/mfcca_encoder.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:29:49.801379 funasr-1.0.9/funasr/models/model_hf/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-02-19 02:44:52.000000 funasr-1.0.9/funasr/models/model_hf/__init__.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:29:49.802054 funasr-1.0.9/funasr/models/monotonic_aligner/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/monotonic_aligner/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9334 2024-02-21 05:07:59.000000 funasr-1.0.9/funasr/models/monotonic_aligner/model.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:29:49.824863 funasr-1.0.9/funasr/models/mossformer/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/mossformer/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2847 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/mossformer/e2e_ss.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10105 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/mossformer/mossformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1341 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/mossformer/mossformer_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11905 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/mossformer/mossformer_encoder.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:29:49.825854 funasr-1.0.9/funasr/models/normalize/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/normalize/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3382 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/normalize/global_mvn.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2283 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/normalize/utterance_mvn.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:29:49.828280 funasr-1.0.9/funasr/models/paraformer/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/paraformer/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    24197 2024-02-06 13:23:23.000000 funasr-1.0.9/funasr/models/paraformer/cif_predictor.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    24451 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/paraformer/decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    22803 2024-02-21 08:28:58.000000 funasr-1.0.9/funasr/models/paraformer/model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    17203 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/paraformer/search.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:29:49.829678 funasr-1.0.9/funasr/models/paraformer_streaming/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/paraformer_streaming/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    28218 2024-02-21 05:07:59.000000 funasr-1.0.9/funasr/models/paraformer_streaming/model.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:29:49.832905 funasr-1.0.9/funasr/models/rwkv_bat/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/rwkv_bat/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/rwkv_bat/model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4700 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/rwkv_bat/rwkv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    19560 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/rwkv_bat/rwkv_attention.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4840 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/rwkv_bat/rwkv_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3129 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/rwkv_bat/rwkv_feed_forward.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7246 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/rwkv_bat/rwkv_subsampling.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:29:49.837612 funasr-1.0.9/funasr/models/sa_asr/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/sa_asr/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1693 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/sa_asr/attention.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)    20122 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/sa_asr/beam_search_sa_asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    18881 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/sa_asr/e2e_sa_asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    28869 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/sa_asr/transformer_decoder.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:29:49.842359 funasr-1.0.9/funasr/models/sanm/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/sanm/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    25896 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/sanm/attention.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    18407 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/sanm/decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    17622 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/sanm/encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      692 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/sanm/model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1078 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/sanm/positionwise_feed_forward.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:29:49.845857 funasr-1.0.9/funasr/models/scama/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/scama/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    37307 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/scama/beam_search.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    19965 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/scama/chunk_utilis.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    42404 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/scama/decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    28398 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/scama/encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    29216 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/scama/model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2586 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/scama/utils.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:29:49.847749 funasr-1.0.9/funasr/models/seaco_paraformer/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/seaco_paraformer/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    25738 2024-02-21 06:46:02.000000 funasr-1.0.9/funasr/models/seaco_paraformer/model.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:29:49.850196 funasr-1.0.9/funasr/models/sond/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/sond/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12324 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/sond/attention.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    23635 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/sond/e2e_diar_sond.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:29:49.852957 funasr-1.0.9/funasr/models/sond/encoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/sond/encoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      909 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/sond/encoder/ci_scorers.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11010 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/sond/encoder/conv_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    19855 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/sond/encoder/ecapa_tdnn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13990 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/sond/encoder/fsmn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    41076 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/sond/encoder/resnet34_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    21259 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/sond/encoder/self_attention_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3330 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/sond/label_aggregation.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:29:49.853954 funasr-1.0.9/funasr/models/sond/pooling/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/sond/pooling/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3785 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/sond/pooling/pooling_layers.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3567 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/sond/pooling/statistic_pooling.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1389 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/sond/sv_decoder.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:29:49.855985 funasr-1.0.9/funasr/models/specaug/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/specaug/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10331 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/specaug/mask_along_axis.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6110 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/specaug/profileaug.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6734 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/specaug/specaug.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2530 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/specaug/time_warp.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:29:49.859097 funasr-1.0.9/funasr/models/transducer/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/transducer/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    23148 2024-02-20 06:05:58.000000 funasr-1.0.9/funasr/models/transducer/beam_search_transducer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2112 2024-02-20 06:05:58.000000 funasr-1.0.9/funasr/models/transducer/joint_network.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    19120 2024-02-21 05:09:56.000000 funasr-1.0.9/funasr/models/transducer/model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12243 2024-02-20 06:05:58.000000 funasr-1.0.9/funasr/models/transducer/rnn_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8500 2024-02-20 06:05:58.000000 funasr-1.0.9/funasr/models/transducer/rnnt_decoder.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:29:49.862565 funasr-1.0.9/funasr/models/transformer/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/transformer/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    19728 2024-02-20 06:05:58.000000 funasr-1.0.9/funasr/models/transformer/attention.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    24724 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/transformer/decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    18442 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/transformer/embedding.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13124 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/transformer/encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5156 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/transformer/layer_norm.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    17052 2024-02-21 05:09:05.000000 funasr-1.0.9/funasr/models/transformer/model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1045 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/transformer/positionwise_feed_forward.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:29:49.864390 funasr-1.0.9/funasr/models/transformer/scorers/
+-rw-r--r--   0 zhifu      (502) staff       (20)       30 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/transformer/scorers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5059 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/transformer/scorers/ctc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13951 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/transformer/scorers/ctc_prefix_score.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1798 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/transformer/scorers/length_bonus.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5938 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/transformer/scorers/scorer_interface.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    17315 2024-02-05 02:42:05.000000 funasr-1.0.9/funasr/models/transformer/search.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:29:49.870239 funasr-1.0.9/funasr/models/transformer/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/transformer/utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      957 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/transformer/utils/add_sos_eos.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4244 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/transformer/utils/dynamic_conv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4863 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/transformer/utils/dynamic_conv2d.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3590 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/transformer/utils/lightconv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4230 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/transformer/utils/lightconv2d.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1654 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/transformer/utils/mask.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4800 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/transformer/utils/multi_layer_conv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    23561 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/transformer/utils/nets_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4294 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/transformer/utils/repeat.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    21882 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/transformer/utils/subsampling.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1898 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/transformer/utils/subsampling_without_posenc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2782 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/transformer/utils/vgg2l.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:29:49.872097 funasr-1.0.9/funasr/models/uniasr/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/uniasr/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    19037 2024-01-24 09:01:27.000000 funasr-1.0.9/funasr/models/uniasr/beam_search.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    44328 2024-01-24 09:01:27.000000 funasr-1.0.9/funasr/models/uniasr/model.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:29:49.874650 funasr-1.0.9/funasr/models/whisper/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/whisper/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9882 2024-02-05 02:42:05.000000 funasr-1.0.9/funasr/models/whisper/model.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:29:49.877519 funasr-1.0.9/funasr/models/whisper/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/whisper/utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4214 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/whisper/utils/audio.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    30110 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/whisper/utils/decoding.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10100 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/whisper/utils/tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    16176 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/whisper/utils/transcribe.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5226 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/whisper/utils/utils.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:29:49.878415 funasr-1.0.9/funasr/models/xvector/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/xvector/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10000 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/models/xvector/e2e_sv.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:29:49.880109 funasr-1.0.9/funasr/optimizers/
+-rw-r--r--   0 zhifu      (502) staff       (20)      446 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/optimizers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5643 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/optimizers/fairseq_adam.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      747 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/optimizers/sgd.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3226 2024-02-17 08:45:57.000000 funasr-1.0.9/funasr/register.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:29:49.882034 funasr-1.0.9/funasr/schedulers/
+-rw-r--r--   0 zhifu      (502) staff       (20)      852 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/schedulers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1679 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/schedulers/abs_scheduler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1986 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/schedulers/noam_lr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3577 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/schedulers/tri_stage_scheduler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1413 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/schedulers/warmup_lr.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:29:49.885888 funasr-1.0.9/funasr/tokenizer/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/tokenizer/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3463 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/tokenizer/abs_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2153 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/tokenizer/build_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3034 2024-02-20 03:45:18.000000 funasr-1.0.9/funasr/tokenizer/char_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1423 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/tokenizer/cleaner.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1968 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/tokenizer/korean_cleaner.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    16530 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/tokenizer/phoneme_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1674 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/tokenizer/sentencepiece_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2019 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/tokenizer/token_id_converter.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1998 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/tokenizer/word_tokenizer.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:29:49.890491 funasr-1.0.9/funasr/train_utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/train_utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      987 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/train_utils/add_gradient_noise.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7007 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/train_utils/average_nbest_models.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2681 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/train_utils/device_funcs.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      971 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/train_utils/forward_adaptor.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1930 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/train_utils/initialize.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4341 2024-02-21 06:46:59.000000 funasr-1.0.9/funasr/train_utils/load_pretrained_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2275 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/train_utils/model_summary.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1615 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/train_utils/recursive_op.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      167 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/train_utils/set_all_random_seed.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    17108 2024-02-21 08:25:50.000000 funasr-1.0.9/funasr/train_utils/trainer.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:29:49.894155 funasr-1.0.9/funasr/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2145 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/utils/datadir_writer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4941 2024-01-30 06:21:05.000000 funasr-1.0.9/funasr/utils/load_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1609 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/utils/misc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9218 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/utils/postprocess_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10757 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/utils/prepare_data.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6761 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/utils/speaker_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7031 2024-02-21 08:28:58.000000 funasr-1.0.9/funasr/utils/timestamp_tools.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4185 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/utils/types.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1202 2024-01-24 03:44:06.000000 funasr-1.0.9/funasr/utils/vad_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)        6 2024-02-21 08:29:23.000000 funasr-1.0.9/funasr/version.txt
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:29:49.743130 funasr-1.0.9/funasr.egg-info/
+-rw-r--r--   0 zhifu      (502) staff       (20)    20490 2024-02-21 08:29:49.000000 funasr-1.0.9/funasr.egg-info/PKG-INFO
+-rw-r--r--   0 zhifu      (502) staff       (20)    11155 2024-02-21 08:29:49.000000 funasr-1.0.9/funasr.egg-info/SOURCES.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)        1 2024-02-21 08:29:49.000000 funasr-1.0.9/funasr.egg-info/dependency_links.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)       59 2024-02-21 08:29:49.000000 funasr-1.0.9/funasr.egg-info/entry_points.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)      664 2024-02-21 08:29:49.000000 funasr-1.0.9/funasr.egg-info/requires.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)        7 2024-02-21 08:29:49.000000 funasr-1.0.9/funasr.egg-info/top_level.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)       38 2024-02-21 08:29:49.897798 funasr-1.0.9/setup.cfg
+-rw-r--r--   0 zhifu      (502) staff       (20)     3832 2024-02-19 08:43:24.000000 funasr-1.0.9/setup.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2024-02-21 08:29:49.897089 funasr-1.0.9/tests/
+-rw-r--r--   0 zhifu      (502) staff       (20)    27007 2024-01-24 03:44:06.000000 funasr-1.0.9/tests/test_asr_inference_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1310 2024-01-24 03:44:06.000000 funasr-1.0.9/tests/test_asr_vad_punc_inference_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      804 2024-01-24 03:44:06.000000 funasr-1.0.9/tests/test_lm_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2055 2024-01-24 03:44:06.000000 funasr-1.0.9/tests/test_punctuation_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1583 2024-01-24 03:44:06.000000 funasr-1.0.9/tests/test_sv_inference_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1741 2024-01-24 03:44:06.000000 funasr-1.0.9/tests/test_tp_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2298 2024-01-24 03:44:06.000000 funasr-1.0.9/tests/test_vad_inference_pipeline.py
```

### Comparing `funasr-1.0.8/PKG-INFO` & `funasr-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funasr
-Version: 1.0.8
+Version: 1.0.9
 Summary: FunASR: A Fundamental End-to-End Speech Recognition Toolkit
 Home-page: https://github.com/alibaba-damo-academy/FunASR.git
 Author: Speech Lab of Alibaba Group
 Author-email: funasr@list.alibaba-inc.com
 License: The MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `funasr-1.0.8/README.md` & `funasr-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/__init__.py` & `funasr-1.0.9/funasr/__init__.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/auto/auto_frontend.py` & `funasr-1.0.9/funasr/auto/auto_frontend.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/auto/auto_model.py` & `funasr-1.0.9/funasr/auto/auto_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -375,20 +375,22 @@
                         else:
                             result[k] += " " + restored_data[j][k]
                     else:
                         if k not in result:
                             result[k] = restored_data[j][k]
                         else:
                             result[k] += restored_data[j][k]
-                            
+            
+            return_raw_text = kwargs.get('return_raw_text', False)            
             # step.3 compute punc model
             if self.punc_model is not None:
                 self.punc_kwargs.update(cfg)
                 punc_res = self.inference(result["text"], model=self.punc_model, kwargs=self.punc_kwargs, disable_pbar=True, **cfg)
                 raw_text = copy.copy(result["text"])
+                if return_raw_text: result['raw_text'] = raw_text
                 result["text"] = punc_res[0]["text"]
             else:
                 raw_text = None
                 
             # speaker embedding cluster after resorted
             if self.spk_model is not None and kwargs.get('return_spk_res', True):
                 if raw_text is None:
@@ -399,34 +401,36 @@
                 # del result['spk_embedding']
                 sv_output = postprocess(all_segments, None, labels, spk_embedding.cpu())
                 if self.spk_mode == 'vad_segment':  # recover sentence_list
                     sentence_list = []
                     for res, vadsegment in zip(restored_data, vadsegments):
                         if 'timestamp' not in res:
                             logging.error("Only 'iic/speech_paraformer-large-vad-punc_asr_nat-zh-cn-16k-common-vocab8404-pytorch' \
-                                and 'iic/speech_seaco_paraformer_large_asr_nat-zh-cn-16k-common-vocab8404-pytorch'\
-                                can predict timestamp, and speaker diarization relies on timestamps.")
-                        sentence_list.append({"start": vadsegment[0],\
-                                                "end": vadsegment[1],
-                                                "sentence": res['text'],
-                                                "timestamp": res['timestamp']})
+                                           and 'iic/speech_seaco_paraformer_large_asr_nat-zh-cn-16k-common-vocab8404-pytorch'\
+                                           can predict timestamp, and speaker diarization relies on timestamps.")
+                        sentence_list.append({"start": vadsegment[0],
+                                              "end": vadsegment[1],
+                                              "sentence": res['text'],
+                                              "timestamp": res['timestamp']})
                 elif self.spk_mode == 'punc_segment':
                     if 'timestamp' not in result:
                         logging.error("Only 'iic/speech_paraformer-large-vad-punc_asr_nat-zh-cn-16k-common-vocab8404-pytorch' \
-                            and 'iic/speech_seaco_paraformer_large_asr_nat-zh-cn-16k-common-vocab8404-pytorch'\
-                            can predict timestamp, and speaker diarization relies on timestamps.")
-                    sentence_list = timestamp_sentence(punc_res[0]['punc_array'], \
-                                                        result['timestamp'], \
-                                                        raw_text)
+                                       and 'iic/speech_seaco_paraformer_large_asr_nat-zh-cn-16k-common-vocab8404-pytorch'\
+                                       can predict timestamp, and speaker diarization relies on timestamps.")
+                    sentence_list = timestamp_sentence(punc_res[0]['punc_array'],
+                                                       result['timestamp'],
+                                                       raw_text,
+                                                       return_raw_text=return_raw_text)
                 distribute_spk(sentence_list, sv_output)
                 result['sentence_info'] = sentence_list
             elif kwargs.get("sentence_timestamp", False):
-                sentence_list = timestamp_sentence(punc_res[0]['punc_array'], \
-                                                        result['timestamp'], \
-                                                        raw_text)
+                sentence_list = timestamp_sentence(punc_res[0]['punc_array'],
+                                                   result['timestamp'],
+                                                   raw_text,
+                                                   return_raw_text=return_raw_text)
                 result['sentence_info'] = sentence_list
             if "spk_embedding" in result: del result['spk_embedding']
                     
             result["key"] = key
             results_ret_list.append(result)
             end_asr_total = time.time()
             time_escape_total_per_sample = end_asr_total - beg_asr_total
```

### Comparing `funasr-1.0.8/funasr/bin/compute_audio_cmvn.py` & `funasr-1.0.9/funasr/bin/compute_audio_cmvn.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/bin/inference.py` & `funasr-1.0.9/funasr/bin/inference.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/bin/tokenize_text.py` & `funasr-1.0.9/funasr/bin/tokenize_text.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/bin/train.py` & `funasr-1.0.9/funasr/bin/train.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/datasets/audio_datasets/datasets.py` & `funasr-1.0.9/funasr/datasets/audio_datasets/datasets.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/datasets/audio_datasets/index_ds.py` & `funasr-1.0.9/funasr/datasets/audio_datasets/index_ds.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/datasets/audio_datasets/preprocessor.py` & `funasr-1.0.9/funasr/datasets/audio_datasets/preprocessor.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/datasets/audio_datasets/samplers.py` & `funasr-1.0.9/funasr/datasets/audio_datasets/samplers.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/datasets/audio_datasets/scp2jsonl.py` & `funasr-1.0.9/funasr/datasets/audio_datasets/scp2jsonl.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/download/download_from_hub.py` & `funasr-1.0.9/funasr/download/download_from_hub.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/download/file.py` & `funasr-1.0.9/funasr/download/file.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/download/name_maps_from_hub.py` & `funasr-1.0.9/funasr/download/name_maps_from_hub.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/download/runtime_sdk_download_tool.py` & `funasr-1.0.9/funasr/download/runtime_sdk_download_tool.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/frontends/default.py` & `funasr-1.0.9/funasr/frontends/default.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/frontends/eend_ola_feature.py` & `funasr-1.0.9/funasr/frontends/eend_ola_feature.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/frontends/fused.py` & `funasr-1.0.9/funasr/frontends/fused.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/frontends/s3prl.py` & `funasr-1.0.9/funasr/frontends/s3prl.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/frontends/utils/beamformer.py` & `funasr-1.0.9/funasr/frontends/utils/beamformer.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/frontends/utils/complex_utils.py` & `funasr-1.0.9/funasr/frontends/utils/complex_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/frontends/utils/dnn_beamformer.py` & `funasr-1.0.9/funasr/frontends/utils/dnn_beamformer.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/frontends/utils/dnn_wpe.py` & `funasr-1.0.9/funasr/frontends/utils/dnn_wpe.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/frontends/utils/feature_transform.py` & `funasr-1.0.9/funasr/frontends/utils/feature_transform.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/frontends/utils/frontend.py` & `funasr-1.0.9/funasr/frontends/utils/frontend.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/frontends/utils/log_mel.py` & `funasr-1.0.9/funasr/frontends/utils/log_mel.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/frontends/utils/mask_estimator.py` & `funasr-1.0.9/funasr/frontends/utils/mask_estimator.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/frontends/utils/stft.py` & `funasr-1.0.9/funasr/frontends/utils/stft.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/frontends/wav_frontend.py` & `funasr-1.0.9/funasr/frontends/wav_frontend.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/frontends/windowing.py` & `funasr-1.0.9/funasr/frontends/windowing.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/losses/label_smoothing_loss.py` & `funasr-1.0.9/funasr/losses/label_smoothing_loss.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/metrics/common.py` & `funasr-1.0.9/funasr/metrics/common.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/metrics/compute_acc.py` & `funasr-1.0.9/funasr/metrics/compute_acc.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/metrics/compute_eer.py` & `funasr-1.0.9/funasr/metrics/compute_eer.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/metrics/compute_min_dcf.py` & `funasr-1.0.9/funasr/metrics/compute_min_dcf.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/metrics/compute_wer.py` & `funasr-1.0.9/funasr/metrics/compute_wer.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/bat/attention.py` & `funasr-1.0.9/funasr/models/bat/attention.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/bat/cif_predictor.py` & `funasr-1.0.9/funasr/models/bat/cif_predictor.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/bat/conformer_chunk_encoder.py` & `funasr-1.0.9/funasr/models/bat/conformer_chunk_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/bat/model.py` & `funasr-1.0.9/funasr/models/bat/model.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/bicif_paraformer/cif_predictor.py` & `funasr-1.0.9/funasr/models/bicif_paraformer/cif_predictor.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/bicif_paraformer/model.py` & `funasr-1.0.9/funasr/models/bicif_paraformer/model.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/branchformer/cgmlp.py` & `funasr-1.0.9/funasr/models/branchformer/cgmlp.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/branchformer/encoder.py` & `funasr-1.0.9/funasr/models/branchformer/encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/branchformer/fastformer.py` & `funasr-1.0.9/funasr/models/branchformer/fastformer.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/campplus/cluster_backend.py` & `funasr-1.0.9/funasr/models/campplus/cluster_backend.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/campplus/components.py` & `funasr-1.0.9/funasr/models/campplus/components.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/campplus/model.py` & `funasr-1.0.9/funasr/models/campplus/model.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/campplus/utils.py` & `funasr-1.0.9/funasr/models/campplus/utils.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/conformer/encoder.py` & `funasr-1.0.9/funasr/models/conformer/encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/contextual_paraformer/decoder.py` & `funasr-1.0.9/funasr/models/contextual_paraformer/decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/contextual_paraformer/model.py` & `funasr-1.0.9/funasr/models/contextual_paraformer/model.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/ct_transformer/model.py` & `funasr-1.0.9/funasr/models/ct_transformer/model.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/ct_transformer/utils.py` & `funasr-1.0.9/funasr/models/ct_transformer/utils.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/ct_transformer_streaming/attention.py` & `funasr-1.0.9/funasr/models/ct_transformer_streaming/attention.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/ct_transformer_streaming/encoder.py` & `funasr-1.0.9/funasr/models/ct_transformer_streaming/encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/ct_transformer_streaming/model.py` & `funasr-1.0.9/funasr/models/ct_transformer_streaming/model.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/ctc/ctc.py` & `funasr-1.0.9/funasr/models/ctc/ctc.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/data2vec/data2vec.py` & `funasr-1.0.9/funasr/models/data2vec/data2vec.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/data2vec/data2vec_encoder.py` & `funasr-1.0.9/funasr/models/data2vec/data2vec_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/data2vec/data_utils.py` & `funasr-1.0.9/funasr/models/data2vec/data_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/data2vec/ema_module.py` & `funasr-1.0.9/funasr/models/data2vec/ema_module.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/data2vec/multihead_attention.py` & `funasr-1.0.9/funasr/models/data2vec/multihead_attention.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/data2vec/quant_noise.py` & `funasr-1.0.9/funasr/models/data2vec/quant_noise.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/data2vec/utils.py` & `funasr-1.0.9/funasr/models/data2vec/utils.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/data2vec/wav2vec2.py` & `funasr-1.0.9/funasr/models/data2vec/wav2vec2.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/e_branchformer/encoder.py` & `funasr-1.0.9/funasr/models/e_branchformer/encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/eend/e2e_diar_eend_ola.py` & `funasr-1.0.9/funasr/models/eend/e2e_diar_eend_ola.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/eend/eend_ola_dataloader.py` & `funasr-1.0.9/funasr/models/eend/eend_ola_dataloader.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/eend/encoder.py` & `funasr-1.0.9/funasr/models/eend/encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/eend/encoder_decoder_attractor.py` & `funasr-1.0.9/funasr/models/eend/encoder_decoder_attractor.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/eend/utils/feature.py` & `funasr-1.0.9/funasr/models/eend/utils/feature.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/eend/utils/kaldi_data.py` & `funasr-1.0.9/funasr/models/eend/utils/kaldi_data.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/eend/utils/losses.py` & `funasr-1.0.9/funasr/models/eend/utils/losses.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/eend/utils/power.py` & `funasr-1.0.9/funasr/models/eend/utils/power.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/eend/utils/report.py` & `funasr-1.0.9/funasr/models/eend/utils/report.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/emotion2vec/audio.py` & `funasr-1.0.9/funasr/models/emotion2vec/audio.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/emotion2vec/base.py` & `funasr-1.0.9/funasr/models/emotion2vec/base.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/emotion2vec/fairseq_modules.py` & `funasr-1.0.9/funasr/models/emotion2vec/fairseq_modules.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/emotion2vec/model.py` & `funasr-1.0.9/funasr/models/emotion2vec/model.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/emotion2vec/modules.py` & `funasr-1.0.9/funasr/models/emotion2vec/modules.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/emotion2vec/timm_modules.py` & `funasr-1.0.9/funasr/models/emotion2vec/timm_modules.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/eres2net/eres2net.py` & `funasr-1.0.9/funasr/models/eres2net/eres2net.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/eres2net/eres2net_aug.py` & `funasr-1.0.9/funasr/models/eres2net/eres2net_aug.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/eres2net/fusion.py` & `funasr-1.0.9/funasr/models/eres2net/fusion.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/fsmn_vad_streaming/encoder.py` & `funasr-1.0.9/funasr/models/fsmn_vad_streaming/encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/fsmn_vad_streaming/model.py` & `funasr-1.0.9/funasr/models/fsmn_vad_streaming/model.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/language_model/rnn/argument.py` & `funasr-1.0.9/funasr/models/language_model/rnn/argument.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/language_model/rnn/attentions.py` & `funasr-1.0.9/funasr/models/language_model/rnn/attentions.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/language_model/rnn/decoders.py` & `funasr-1.0.9/funasr/models/language_model/rnn/decoders.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/language_model/rnn/encoders.py` & `funasr-1.0.9/funasr/models/language_model/rnn/encoders.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/language_model/seq_rnn_lm.py` & `funasr-1.0.9/funasr/models/language_model/seq_rnn_lm.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/language_model/transformer_encoder.py` & `funasr-1.0.9/funasr/models/language_model/transformer_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/language_model/transformer_lm.py` & `funasr-1.0.9/funasr/models/language_model/transformer_lm.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/lora/layers.py` & `funasr-1.0.9/funasr/models/lora/layers.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/lora/utils.py` & `funasr-1.0.9/funasr/models/lora/utils.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/mfcca/e2e_asr_mfcca.py` & `funasr-1.0.9/funasr/models/mfcca/e2e_asr_mfcca.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/mfcca/encoder_layer_mfcca.py` & `funasr-1.0.9/funasr/models/mfcca/encoder_layer_mfcca.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/mfcca/mfcca_encoder.py` & `funasr-1.0.9/funasr/models/mfcca/mfcca_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/monotonic_aligner/model.py` & `funasr-1.0.9/funasr/models/monotonic_aligner/model.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/mossformer/e2e_ss.py` & `funasr-1.0.9/funasr/models/mossformer/e2e_ss.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/mossformer/mossformer.py` & `funasr-1.0.9/funasr/models/mossformer/mossformer.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/mossformer/mossformer_decoder.py` & `funasr-1.0.9/funasr/models/mossformer/mossformer_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/mossformer/mossformer_encoder.py` & `funasr-1.0.9/funasr/models/mossformer/mossformer_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/normalize/global_mvn.py` & `funasr-1.0.9/funasr/models/normalize/global_mvn.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/normalize/utterance_mvn.py` & `funasr-1.0.9/funasr/models/normalize/utterance_mvn.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/paraformer/cif_predictor.py` & `funasr-1.0.9/funasr/models/paraformer/cif_predictor.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/paraformer/decoder.py` & `funasr-1.0.9/funasr/models/paraformer/decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/paraformer/model.py` & `funasr-1.0.9/funasr/models/paraformer/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -533,15 +533,14 @@
                     token = tokenizer.ids2tokens(token_int)
                     text_postprocessed = tokenizer.tokens2text(token)
                     if not hasattr(tokenizer, "bpemodel"):
                         text_postprocessed, _ = postprocess_utils.sentence_postprocess(token)
                     
                     result_i = {"key": key[i], "text": text_postprocessed}
 
-                    
                     if ibest_writer is not None:
                         ibest_writer["token"][key[i]] = " ".join(token)
                         # ibest_writer["text"][key[i]] = text
                         ibest_writer["text"][key[i]] = text_postprocessed
                 else:
                     result_i = {"key": key[i], "token_int": token_int}
                 results.append(result_i)
```

### Comparing `funasr-1.0.8/funasr/models/paraformer/search.py` & `funasr-1.0.9/funasr/models/paraformer/search.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/paraformer_streaming/model.py` & `funasr-1.0.9/funasr/models/paraformer_streaming/model.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/rwkv_bat/rwkv.py` & `funasr-1.0.9/funasr/models/rwkv_bat/rwkv.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/rwkv_bat/rwkv_attention.py` & `funasr-1.0.9/funasr/models/rwkv_bat/rwkv_attention.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/rwkv_bat/rwkv_encoder.py` & `funasr-1.0.9/funasr/models/rwkv_bat/rwkv_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/rwkv_bat/rwkv_feed_forward.py` & `funasr-1.0.9/funasr/models/rwkv_bat/rwkv_feed_forward.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/rwkv_bat/rwkv_subsampling.py` & `funasr-1.0.9/funasr/models/rwkv_bat/rwkv_subsampling.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/sa_asr/attention.py` & `funasr-1.0.9/funasr/models/sa_asr/attention.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/sa_asr/beam_search_sa_asr.py` & `funasr-1.0.9/funasr/models/sa_asr/beam_search_sa_asr.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/sa_asr/e2e_sa_asr.py` & `funasr-1.0.9/funasr/models/sa_asr/e2e_sa_asr.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/sa_asr/transformer_decoder.py` & `funasr-1.0.9/funasr/models/sa_asr/transformer_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/sanm/attention.py` & `funasr-1.0.9/funasr/models/sanm/attention.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/sanm/decoder.py` & `funasr-1.0.9/funasr/models/sanm/decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/sanm/encoder.py` & `funasr-1.0.9/funasr/models/sanm/encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/sanm/model.py` & `funasr-1.0.9/funasr/models/sanm/model.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/sanm/positionwise_feed_forward.py` & `funasr-1.0.9/funasr/models/sanm/positionwise_feed_forward.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/scama/beam_search.py` & `funasr-1.0.9/funasr/models/scama/beam_search.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/scama/chunk_utilis.py` & `funasr-1.0.9/funasr/models/scama/chunk_utilis.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/scama/decoder.py` & `funasr-1.0.9/funasr/models/scama/decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/scama/encoder.py` & `funasr-1.0.9/funasr/models/scama/encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/scama/model.py` & `funasr-1.0.9/funasr/models/scama/model.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/scama/utils.py` & `funasr-1.0.9/funasr/models/scama/utils.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/seaco_paraformer/model.py` & `funasr-1.0.9/funasr/models/seaco_paraformer/model.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/sond/attention.py` & `funasr-1.0.9/funasr/models/sond/attention.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/sond/e2e_diar_sond.py` & `funasr-1.0.9/funasr/models/sond/e2e_diar_sond.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/sond/encoder/ci_scorers.py` & `funasr-1.0.9/funasr/models/sond/encoder/ci_scorers.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/sond/encoder/conv_encoder.py` & `funasr-1.0.9/funasr/models/sond/encoder/conv_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/sond/encoder/ecapa_tdnn_encoder.py` & `funasr-1.0.9/funasr/models/sond/encoder/ecapa_tdnn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/sond/encoder/fsmn_encoder.py` & `funasr-1.0.9/funasr/models/sond/encoder/fsmn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/sond/encoder/resnet34_encoder.py` & `funasr-1.0.9/funasr/models/sond/encoder/resnet34_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/sond/encoder/self_attention_encoder.py` & `funasr-1.0.9/funasr/models/sond/encoder/self_attention_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/sond/label_aggregation.py` & `funasr-1.0.9/funasr/models/sond/label_aggregation.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/sond/pooling/pooling_layers.py` & `funasr-1.0.9/funasr/models/sond/pooling/pooling_layers.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/sond/pooling/statistic_pooling.py` & `funasr-1.0.9/funasr/models/sond/pooling/statistic_pooling.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/sond/sv_decoder.py` & `funasr-1.0.9/funasr/models/sond/sv_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/specaug/mask_along_axis.py` & `funasr-1.0.9/funasr/models/specaug/mask_along_axis.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/specaug/profileaug.py` & `funasr-1.0.9/funasr/models/specaug/profileaug.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/specaug/specaug.py` & `funasr-1.0.9/funasr/models/specaug/specaug.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/specaug/time_warp.py` & `funasr-1.0.9/funasr/models/specaug/time_warp.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/transducer/beam_search_transducer.py` & `funasr-1.0.9/funasr/models/transducer/beam_search_transducer.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/transducer/joint_network.py` & `funasr-1.0.9/funasr/models/transducer/joint_network.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/transducer/model.py` & `funasr-1.0.9/funasr/models/transducer/model.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/transducer/rnn_decoder.py` & `funasr-1.0.9/funasr/models/transducer/rnn_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/transducer/rnnt_decoder.py` & `funasr-1.0.9/funasr/models/transducer/rnnt_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/transformer/attention.py` & `funasr-1.0.9/funasr/models/transformer/attention.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/transformer/decoder.py` & `funasr-1.0.9/funasr/models/transformer/decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/transformer/embedding.py` & `funasr-1.0.9/funasr/models/transformer/embedding.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/transformer/encoder.py` & `funasr-1.0.9/funasr/models/transformer/encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/transformer/layer_norm.py` & `funasr-1.0.9/funasr/models/transformer/layer_norm.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/transformer/model.py` & `funasr-1.0.9/funasr/models/transformer/model.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/transformer/positionwise_feed_forward.py` & `funasr-1.0.9/funasr/models/transformer/positionwise_feed_forward.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/transformer/scorers/ctc.py` & `funasr-1.0.9/funasr/models/transformer/scorers/ctc.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/transformer/scorers/ctc_prefix_score.py` & `funasr-1.0.9/funasr/models/transformer/scorers/ctc_prefix_score.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/transformer/scorers/length_bonus.py` & `funasr-1.0.9/funasr/models/transformer/scorers/length_bonus.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/transformer/scorers/scorer_interface.py` & `funasr-1.0.9/funasr/models/transformer/scorers/scorer_interface.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/transformer/search.py` & `funasr-1.0.9/funasr/models/transformer/search.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/transformer/utils/add_sos_eos.py` & `funasr-1.0.9/funasr/models/transformer/utils/add_sos_eos.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/transformer/utils/dynamic_conv.py` & `funasr-1.0.9/funasr/models/transformer/utils/dynamic_conv.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/transformer/utils/dynamic_conv2d.py` & `funasr-1.0.9/funasr/models/transformer/utils/dynamic_conv2d.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/transformer/utils/lightconv.py` & `funasr-1.0.9/funasr/models/transformer/utils/lightconv.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/transformer/utils/lightconv2d.py` & `funasr-1.0.9/funasr/models/transformer/utils/lightconv2d.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/transformer/utils/mask.py` & `funasr-1.0.9/funasr/models/transformer/utils/mask.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/transformer/utils/multi_layer_conv.py` & `funasr-1.0.9/funasr/models/transformer/utils/multi_layer_conv.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/transformer/utils/nets_utils.py` & `funasr-1.0.9/funasr/models/transformer/utils/nets_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/transformer/utils/repeat.py` & `funasr-1.0.9/funasr/models/transformer/utils/repeat.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/transformer/utils/subsampling.py` & `funasr-1.0.9/funasr/models/transformer/utils/subsampling.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/transformer/utils/subsampling_without_posenc.py` & `funasr-1.0.9/funasr/models/transformer/utils/subsampling_without_posenc.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/transformer/utils/vgg2l.py` & `funasr-1.0.9/funasr/models/transformer/utils/vgg2l.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/uniasr/beam_search.py` & `funasr-1.0.9/funasr/models/uniasr/beam_search.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/uniasr/model.py` & `funasr-1.0.9/funasr/models/uniasr/model.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/whisper/model.py` & `funasr-1.0.9/funasr/models/whisper/model.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/whisper/utils/audio.py` & `funasr-1.0.9/funasr/models/whisper/utils/audio.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/whisper/utils/decoding.py` & `funasr-1.0.9/funasr/models/whisper/utils/decoding.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/whisper/utils/tokenizer.py` & `funasr-1.0.9/funasr/models/whisper/utils/tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/whisper/utils/transcribe.py` & `funasr-1.0.9/funasr/models/whisper/utils/transcribe.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/whisper/utils/utils.py` & `funasr-1.0.9/funasr/models/whisper/utils/utils.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/models/xvector/e2e_sv.py` & `funasr-1.0.9/funasr/models/xvector/e2e_sv.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/optimizers/fairseq_adam.py` & `funasr-1.0.9/funasr/optimizers/fairseq_adam.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/optimizers/sgd.py` & `funasr-1.0.9/funasr/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/register.py` & `funasr-1.0.9/funasr/register.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/schedulers/__init__.py` & `funasr-1.0.9/funasr/schedulers/__init__.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/schedulers/abs_scheduler.py` & `funasr-1.0.9/funasr/schedulers/abs_scheduler.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/schedulers/noam_lr.py` & `funasr-1.0.9/funasr/schedulers/noam_lr.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/schedulers/tri_stage_scheduler.py` & `funasr-1.0.9/funasr/schedulers/tri_stage_scheduler.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/schedulers/warmup_lr.py` & `funasr-1.0.9/funasr/schedulers/warmup_lr.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/tokenizer/abs_tokenizer.py` & `funasr-1.0.9/funasr/tokenizer/abs_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/tokenizer/build_tokenizer.py` & `funasr-1.0.9/funasr/tokenizer/build_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/tokenizer/char_tokenizer.py` & `funasr-1.0.9/funasr/tokenizer/char_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/tokenizer/cleaner.py` & `funasr-1.0.9/funasr/tokenizer/cleaner.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/tokenizer/korean_cleaner.py` & `funasr-1.0.9/funasr/tokenizer/korean_cleaner.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/tokenizer/phoneme_tokenizer.py` & `funasr-1.0.9/funasr/tokenizer/phoneme_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/tokenizer/sentencepiece_tokenizer.py` & `funasr-1.0.9/funasr/tokenizer/sentencepiece_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/tokenizer/token_id_converter.py` & `funasr-1.0.9/funasr/tokenizer/token_id_converter.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/tokenizer/word_tokenizer.py` & `funasr-1.0.9/funasr/tokenizer/word_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/train_utils/add_gradient_noise.py` & `funasr-1.0.9/funasr/train_utils/add_gradient_noise.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/train_utils/average_nbest_models.py` & `funasr-1.0.9/funasr/train_utils/average_nbest_models.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/train_utils/device_funcs.py` & `funasr-1.0.9/funasr/train_utils/device_funcs.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/train_utils/forward_adaptor.py` & `funasr-1.0.9/funasr/train_utils/forward_adaptor.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/train_utils/initialize.py` & `funasr-1.0.9/funasr/train_utils/initialize.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/train_utils/load_pretrained_model.py` & `funasr-1.0.9/funasr/train_utils/load_pretrained_model.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/train_utils/model_summary.py` & `funasr-1.0.9/funasr/train_utils/model_summary.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/train_utils/recursive_op.py` & `funasr-1.0.9/funasr/train_utils/recursive_op.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/train_utils/trainer.py` & `funasr-1.0.9/funasr/train_utils/trainer.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/utils/datadir_writer.py` & `funasr-1.0.9/funasr/utils/datadir_writer.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/utils/load_utils.py` & `funasr-1.0.9/funasr/utils/load_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/utils/misc.py` & `funasr-1.0.9/funasr/utils/misc.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/utils/postprocess_utils.py` & `funasr-1.0.9/funasr/utils/postprocess_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/utils/prepare_data.py` & `funasr-1.0.9/funasr/utils/prepare_data.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/utils/speaker_utils.py` & `funasr-1.0.9/funasr/utils/speaker_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/utils/timestamp_tools.py` & `funasr-1.0.9/funasr/utils/timestamp_tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -94,15 +94,15 @@
     res = []
     for char, timestamp in zip(new_char_list, timestamp_list):
         if char != '<sil>':
             res.append([int(timestamp[0] * 1000), int(timestamp[1] * 1000)])
     return res_txt, res
 
 
-def timestamp_sentence(punc_id_list, timestamp_postprocessed, text_postprocessed):
+def timestamp_sentence(punc_id_list, timestamp_postprocessed, text_postprocessed, return_raw_text=False):
     punc_list = ['，', '。', '？', '、']
     res = []
     if text_postprocessed is None:
         return res
     if timestamp_postprocessed is None:
         return res
     if len(timestamp_postprocessed) == 0:
@@ -138,23 +138,32 @@
             else:
                 sentence_text += text
             sentence_text_seg += text + ' '
         ts_list.append(timestamp)
 
         punc_id = int(punc_id) if punc_id is not None else 1
         sentence_end = timestamp[1] if timestamp is not None else sentence_end
-
+        sentence_text_seg = sentence_text_seg[:-1] if sentence_text_seg[-1] == ' ' else sentence_text_seg
         if punc_id > 1:
             sentence_text += punc_list[punc_id - 2]
-            res.append({
-                'text': sentence_text,
-                "start": sentence_start,
-                "end": sentence_end,
-                "timestamp": ts_list
-            })
+            if return_raw_text:
+                res.append({
+                    'text': sentence_text,
+                    "start": sentence_start,
+                    "end": sentence_end,
+                    "timestamp": ts_list,
+                    'raw_text': sentence_text_seg,
+                })
+            else:
+                res.append({
+                    'text': sentence_text,
+                    "start": sentence_start,
+                    "end": sentence_end,
+                    "timestamp": ts_list,
+                })
             sentence_text = ''
             sentence_text_seg = ''
             ts_list = []
             sentence_start = sentence_end
     return res
```

### Comparing `funasr-1.0.8/funasr/utils/types.py` & `funasr-1.0.9/funasr/utils/types.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr/utils/vad_utils.py` & `funasr-1.0.9/funasr/utils/vad_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr.egg-info/PKG-INFO` & `funasr-1.0.9/funasr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funasr
-Version: 1.0.8
+Version: 1.0.9
 Summary: FunASR: A Fundamental End-to-End Speech Recognition Toolkit
 Home-page: https://github.com/alibaba-damo-academy/FunASR.git
 Author: Speech Lab of Alibaba Group
 Author-email: funasr@list.alibaba-inc.com
 License: The MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `funasr-1.0.8/funasr.egg-info/SOURCES.txt` & `funasr-1.0.9/funasr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/funasr.egg-info/requires.txt` & `funasr-1.0.9/funasr.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/setup.py` & `funasr-1.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/tests/test_asr_inference_pipeline.py` & `funasr-1.0.9/tests/test_asr_inference_pipeline.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/tests/test_asr_vad_punc_inference_pipeline.py` & `funasr-1.0.9/tests/test_asr_vad_punc_inference_pipeline.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/tests/test_lm_pipeline.py` & `funasr-1.0.9/tests/test_lm_pipeline.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/tests/test_punctuation_pipeline.py` & `funasr-1.0.9/tests/test_punctuation_pipeline.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/tests/test_sv_inference_pipeline.py` & `funasr-1.0.9/tests/test_sv_inference_pipeline.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/tests/test_tp_pipeline.py` & `funasr-1.0.9/tests/test_tp_pipeline.py`

 * *Files identical despite different names*

### Comparing `funasr-1.0.8/tests/test_vad_inference_pipeline.py` & `funasr-1.0.9/tests/test_vad_inference_pipeline.py`

 * *Files identical despite different names*

