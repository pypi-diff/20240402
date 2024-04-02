# Comparing `tmp/mlx-lm-0.5.0.tar.gz` & `tmp/mlx-lm-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlx-lm-0.5.0.tar", last modified: Mon Mar 25 13:08:56 2024, max compression
+gzip compressed data, was "mlx-lm-0.6.0.tar", last modified: Tue Apr  2 20:54:33 2024, max compression
```

## Comparing `mlx-lm-0.5.0.tar` & `mlx-lm-0.6.0.tar`

### file list

```diff
@@ -1,53 +1,56 @@
-drwxr-xr-x   0 awnihannun   (501) staff       (20)        0 2024-03-25 13:08:56.193394 mlx-lm-0.5.0/
--rw-r--r--   0 awnihannun   (501) staff       (20)       63 2024-01-19 21:42:37.000000 mlx-lm-0.5.0/MANIFEST.in
--rw-r--r--   0 awnihannun   (501) staff       (20)     5058 2024-03-25 13:08:56.193176 mlx-lm-0.5.0/PKG-INFO
--rw-r--r--   0 awnihannun   (501) staff       (20)     4604 2024-03-03 19:16:48.000000 mlx-lm-0.5.0/README.md
-drwxr-xr-x   0 awnihannun   (501) staff       (20)        0 2024-03-25 13:08:56.186100 mlx-lm-0.5.0/mlx_lm/
--rw-r--r--   0 awnihannun   (501) staff       (20)      113 2024-02-28 03:35:15.000000 mlx-lm-0.5.0/mlx_lm/__init__.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     1622 2024-03-21 17:35:13.000000 mlx-lm-0.5.0/mlx_lm/convert.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     3568 2024-03-21 17:35:13.000000 mlx-lm-0.5.0/mlx_lm/fuse.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     3876 2024-03-23 20:25:19.000000 mlx-lm-0.5.0/mlx_lm/generate.py
--rw-r--r--   0 awnihannun   (501) staff       (20)    11309 2024-03-21 17:35:13.000000 mlx-lm-0.5.0/mlx_lm/gguf.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     7499 2024-03-21 17:35:13.000000 mlx-lm-0.5.0/mlx_lm/lora.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     4782 2024-03-15 14:22:39.000000 mlx-lm-0.5.0/mlx_lm/merge.py
-drwxr-xr-x   0 awnihannun   (501) staff       (20)        0 2024-03-25 13:08:56.189963 mlx-lm-0.5.0/mlx_lm/models/
--rw-r--r--   0 awnihannun   (501) staff       (20)        0 2024-01-19 21:42:37.000000 mlx-lm-0.5.0/mlx_lm/models/__init__.py
--rw-r--r--   0 awnihannun   (501) staff       (20)      314 2024-01-19 21:42:37.000000 mlx-lm-0.5.0/mlx_lm/models/base.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     5409 2024-03-25 13:08:25.000000 mlx-lm-0.5.0/mlx_lm/models/cohere.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     5591 2024-03-25 13:08:25.000000 mlx-lm-0.5.0/mlx_lm/models/gemma.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     6307 2024-03-25 13:08:25.000000 mlx-lm-0.5.0/mlx_lm/models/llama.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     7910 2024-03-25 13:08:25.000000 mlx-lm-0.5.0/mlx_lm/models/mixtral.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     5105 2024-03-25 13:08:25.000000 mlx-lm-0.5.0/mlx_lm/models/olmo.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     5961 2024-03-25 13:08:25.000000 mlx-lm-0.5.0/mlx_lm/models/phi.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     6614 2024-03-25 13:08:25.000000 mlx-lm-0.5.0/mlx_lm/models/phixtral.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     7259 2024-03-25 13:08:25.000000 mlx-lm-0.5.0/mlx_lm/models/plamo.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     4990 2024-03-25 13:08:25.000000 mlx-lm-0.5.0/mlx_lm/models/qwen.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     6523 2024-03-25 13:08:25.000000 mlx-lm-0.5.0/mlx_lm/models/qwen2.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     5931 2024-03-25 13:08:25.000000 mlx-lm-0.5.0/mlx_lm/models/stablelm.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     5416 2024-03-25 13:08:25.000000 mlx-lm-0.5.0/mlx_lm/models/starcoder2.py
--rw-r--r--   0 awnihannun   (501) staff       (20)        1 2024-02-28 03:35:15.000000 mlx-lm-0.5.0/mlx_lm/py.typed
--rw-r--r--   0 awnihannun   (501) staff       (20)       59 2024-03-25 13:08:25.000000 mlx-lm-0.5.0/mlx_lm/requirements.txt
--rw-r--r--   0 awnihannun   (501) staff       (20)     1343 2024-03-25 13:08:25.000000 mlx-lm-0.5.0/mlx_lm/sample_utils.py
--rw-r--r--   0 awnihannun   (501) staff       (20)    15866 2024-03-21 17:35:13.000000 mlx-lm-0.5.0/mlx_lm/server.py
-drwxr-xr-x   0 awnihannun   (501) staff       (20)        0 2024-03-25 13:08:56.191144 mlx-lm-0.5.0/mlx_lm/tuner/
--rw-r--r--   0 awnihannun   (501) staff       (20)        0 2024-02-28 03:35:15.000000 mlx-lm-0.5.0/mlx_lm/tuner/__init__.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     3258 2024-03-20 13:42:49.000000 mlx-lm-0.5.0/mlx_lm/tuner/datasets.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     2875 2024-03-25 13:08:25.000000 mlx-lm-0.5.0/mlx_lm/tuner/lora.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     9829 2024-03-25 13:08:25.000000 mlx-lm-0.5.0/mlx_lm/tuner/trainer.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     4540 2024-03-21 17:35:13.000000 mlx-lm-0.5.0/mlx_lm/tuner/utils.py
--rw-r--r--   0 awnihannun   (501) staff       (20)    19508 2024-03-25 13:08:25.000000 mlx-lm-0.5.0/mlx_lm/utils.py
--rw-r--r--   0 awnihannun   (501) staff       (20)       59 2024-03-25 13:08:37.000000 mlx-lm-0.5.0/mlx_lm/version.py
-drwxr-xr-x   0 awnihannun   (501) staff       (20)        0 2024-03-25 13:08:56.192864 mlx-lm-0.5.0/mlx_lm.egg-info/
--rw-r--r--   0 awnihannun   (501) staff       (20)     5058 2024-03-25 13:08:56.000000 mlx-lm-0.5.0/mlx_lm.egg-info/PKG-INFO
--rw-r--r--   0 awnihannun   (501) staff       (20)      970 2024-03-25 13:08:56.000000 mlx-lm-0.5.0/mlx_lm.egg-info/SOURCES.txt
--rw-r--r--   0 awnihannun   (501) staff       (20)        1 2024-03-25 13:08:56.000000 mlx-lm-0.5.0/mlx_lm.egg-info/dependency_links.txt
--rw-r--r--   0 awnihannun   (501) staff       (20)       59 2024-03-25 13:08:56.000000 mlx-lm-0.5.0/mlx_lm.egg-info/requires.txt
--rw-r--r--   0 awnihannun   (501) staff       (20)        7 2024-03-25 13:08:56.000000 mlx-lm-0.5.0/mlx_lm.egg-info/top_level.txt
--rw-r--r--   0 awnihannun   (501) staff       (20)       38 2024-03-25 13:08:56.193439 mlx-lm-0.5.0/setup.cfg
--rw-r--r--   0 awnihannun   (501) staff       (20)      824 2024-02-28 03:35:15.000000 mlx-lm-0.5.0/setup.py
-drwxr-xr-x   0 awnihannun   (501) staff       (20)        0 2024-03-25 13:08:56.192527 mlx-lm-0.5.0/tests/
--rw-r--r--   0 awnihannun   (501) staff       (20)     2892 2024-03-20 13:42:49.000000 mlx-lm-0.5.0/tests/test_datsets.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     4227 2024-03-21 17:35:13.000000 mlx-lm-0.5.0/tests/test_lora.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     9042 2024-03-25 13:08:25.000000 mlx-lm-0.5.0/tests/test_models.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     1303 2024-03-25 13:08:25.000000 mlx-lm-0.5.0/tests/test_sample_utils.py
--rw-r--r--   0 awnihannun   (501) staff       (20)     2955 2024-03-15 14:22:39.000000 mlx-lm-0.5.0/tests/test_utils.py
+drwxr-xr-x   0 awnihannun   (501) staff       (20)        0 2024-04-02 20:54:33.022838 mlx-lm-0.6.0/
+-rw-r--r--   0 awnihannun   (501) staff       (20)       63 2024-01-19 21:42:37.000000 mlx-lm-0.6.0/MANIFEST.in
+-rw-r--r--   0 awnihannun   (501) staff       (20)     5058 2024-04-02 20:54:33.022664 mlx-lm-0.6.0/PKG-INFO
+-rw-r--r--   0 awnihannun   (501) staff       (20)     4604 2024-03-03 19:16:48.000000 mlx-lm-0.6.0/README.md
+drwxr-xr-x   0 awnihannun   (501) staff       (20)        0 2024-04-02 20:54:33.015215 mlx-lm-0.6.0/mlx_lm/
+-rw-r--r--   0 awnihannun   (501) staff       (20)      113 2024-02-28 03:35:15.000000 mlx-lm-0.6.0/mlx_lm/__init__.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     1622 2024-03-21 17:35:13.000000 mlx-lm-0.6.0/mlx_lm/convert.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     3542 2024-04-02 20:54:21.000000 mlx-lm-0.6.0/mlx_lm/fuse.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     3887 2024-04-02 20:54:21.000000 mlx-lm-0.6.0/mlx_lm/generate.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)    11364 2024-04-01 16:35:43.000000 mlx-lm-0.6.0/mlx_lm/gguf.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     7852 2024-04-02 20:54:21.000000 mlx-lm-0.6.0/mlx_lm/lora.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     4770 2024-04-02 20:54:21.000000 mlx-lm-0.6.0/mlx_lm/merge.py
+drwxr-xr-x   0 awnihannun   (501) staff       (20)        0 2024-04-02 20:54:33.019754 mlx-lm-0.6.0/mlx_lm/models/
+-rw-r--r--   0 awnihannun   (501) staff       (20)        0 2024-01-19 21:42:37.000000 mlx-lm-0.6.0/mlx_lm/models/__init__.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)      314 2024-01-19 21:42:37.000000 mlx-lm-0.6.0/mlx_lm/models/base.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     5409 2024-03-25 13:08:25.000000 mlx-lm-0.6.0/mlx_lm/models/cohere.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     8281 2024-04-01 16:35:43.000000 mlx-lm-0.6.0/mlx_lm/models/dbrx.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     5548 2024-04-01 16:35:43.000000 mlx-lm-0.6.0/mlx_lm/models/gemma.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     6307 2024-03-25 13:08:25.000000 mlx-lm-0.6.0/mlx_lm/models/llama.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     7869 2024-04-01 16:35:43.000000 mlx-lm-0.6.0/mlx_lm/models/mixtral.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     5092 2024-04-01 16:35:43.000000 mlx-lm-0.6.0/mlx_lm/models/olmo.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     5961 2024-03-25 13:08:25.000000 mlx-lm-0.6.0/mlx_lm/models/phi.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     6599 2024-04-01 16:35:43.000000 mlx-lm-0.6.0/mlx_lm/models/phixtral.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     7101 2024-04-01 16:35:43.000000 mlx-lm-0.6.0/mlx_lm/models/plamo.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     4990 2024-03-25 13:08:25.000000 mlx-lm-0.6.0/mlx_lm/models/qwen.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     6523 2024-03-25 13:08:25.000000 mlx-lm-0.6.0/mlx_lm/models/qwen2.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     8479 2024-04-02 20:54:21.000000 mlx-lm-0.6.0/mlx_lm/models/qwen2_moe.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     5931 2024-03-25 13:08:25.000000 mlx-lm-0.6.0/mlx_lm/models/stablelm.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     5416 2024-03-25 13:08:25.000000 mlx-lm-0.6.0/mlx_lm/models/starcoder2.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)        1 2024-02-28 03:35:15.000000 mlx-lm-0.6.0/mlx_lm/py.typed
+-rw-r--r--   0 awnihannun   (501) staff       (20)       59 2024-03-25 13:08:25.000000 mlx-lm-0.6.0/mlx_lm/requirements.txt
+-rw-r--r--   0 awnihannun   (501) staff       (20)     1354 2024-04-01 16:35:43.000000 mlx-lm-0.6.0/mlx_lm/sample_utils.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)    15877 2024-04-02 20:54:21.000000 mlx-lm-0.6.0/mlx_lm/server.py
+drwxr-xr-x   0 awnihannun   (501) staff       (20)        0 2024-04-02 20:54:33.020707 mlx-lm-0.6.0/mlx_lm/tuner/
+-rw-r--r--   0 awnihannun   (501) staff       (20)        0 2024-02-28 03:35:15.000000 mlx-lm-0.6.0/mlx_lm/tuner/__init__.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     3258 2024-03-20 13:42:49.000000 mlx-lm-0.6.0/mlx_lm/tuner/datasets.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     2875 2024-03-25 13:08:25.000000 mlx-lm-0.6.0/mlx_lm/tuner/lora.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     9439 2024-04-02 20:54:21.000000 mlx-lm-0.6.0/mlx_lm/tuner/trainer.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     5354 2024-04-02 20:54:21.000000 mlx-lm-0.6.0/mlx_lm/tuner/utils.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)    19526 2024-04-02 20:54:21.000000 mlx-lm-0.6.0/mlx_lm/utils.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)       59 2024-04-02 20:54:21.000000 mlx-lm-0.6.0/mlx_lm/version.py
+drwxr-xr-x   0 awnihannun   (501) staff       (20)        0 2024-04-02 20:54:33.022412 mlx-lm-0.6.0/mlx_lm.egg-info/
+-rw-r--r--   0 awnihannun   (501) staff       (20)     5058 2024-04-02 20:54:33.000000 mlx-lm-0.6.0/mlx_lm.egg-info/PKG-INFO
+-rw-r--r--   0 awnihannun   (501) staff       (20)     1038 2024-04-02 20:54:33.000000 mlx-lm-0.6.0/mlx_lm.egg-info/SOURCES.txt
+-rw-r--r--   0 awnihannun   (501) staff       (20)        1 2024-04-02 20:54:33.000000 mlx-lm-0.6.0/mlx_lm.egg-info/dependency_links.txt
+-rw-r--r--   0 awnihannun   (501) staff       (20)       59 2024-04-02 20:54:33.000000 mlx-lm-0.6.0/mlx_lm.egg-info/requires.txt
+-rw-r--r--   0 awnihannun   (501) staff       (20)        7 2024-04-02 20:54:33.000000 mlx-lm-0.6.0/mlx_lm.egg-info/top_level.txt
+-rw-r--r--   0 awnihannun   (501) staff       (20)       38 2024-04-02 20:54:33.022889 mlx-lm-0.6.0/setup.cfg
+-rw-r--r--   0 awnihannun   (501) staff       (20)      824 2024-02-28 03:35:15.000000 mlx-lm-0.6.0/setup.py
+drwxr-xr-x   0 awnihannun   (501) staff       (20)        0 2024-04-02 20:54:33.021976 mlx-lm-0.6.0/tests/
+-rw-r--r--   0 awnihannun   (501) staff       (20)     2892 2024-03-20 13:42:49.000000 mlx-lm-0.6.0/tests/test_datsets.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     1844 2024-04-01 16:35:43.000000 mlx-lm-0.6.0/tests/test_gguf.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     6052 2024-04-01 16:35:43.000000 mlx-lm-0.6.0/tests/test_lora.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     9705 2024-04-02 20:54:21.000000 mlx-lm-0.6.0/tests/test_models.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     1446 2024-04-01 16:35:43.000000 mlx-lm-0.6.0/tests/test_sample_utils.py
+-rw-r--r--   0 awnihannun   (501) staff       (20)     2955 2024-03-15 14:22:39.000000 mlx-lm-0.6.0/tests/test_utils.py
```

### Comparing `mlx-lm-0.5.0/PKG-INFO` & `mlx-lm-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlx-lm
-Version: 0.5.0
+Version: 0.6.0
 Summary: LLMs on Apple silicon with MLX and the Hugging Face Hub
 Home-page: https://github.com/ml-explore/mlx-examples
 Author: MLX Contributors
 Author-email: mlx@group.apple.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `mlx-lm-0.5.0/README.md` & `mlx-lm-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.5.0/mlx_lm/convert.py` & `mlx-lm-0.6.0/mlx_lm/convert.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.5.0/mlx_lm/fuse.py` & `mlx-lm-0.6.0/mlx_lm/fuse.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import argparse
 import glob
-import json
 import shutil
 from pathlib import Path
 
 from mlx.utils import tree_flatten, tree_unflatten
 
 from .gguf import convert_to_gguf
 from .tuner.lora import LoRALinear
@@ -27,18 +26,18 @@
     )
     parser.add_argument(
         "--save-path",
         default="lora_fused_model",
         help="The path to save the fused model.",
     )
     parser.add_argument(
-        "--adapter-file",
+        "--adapter-path",
         type=str,
-        default="adapters.npz",
-        help="Path to the trained adapter weights (npz or safetensors).",
+        default="adapters",
+        help="Path to the trained adapter weights and config.",
     )
     parser.add_argument(
         "--hf-path",
         type=str,
         default=None,
         help="Path to the original Hugging Face model. Required for upload if --model is a local directory.",
     )
@@ -71,15 +70,15 @@
     print("Loading pretrained model")
     args = parse_arguments()
 
     model_path = get_model_path(args.model)
     model, config, tokenizer = fetch_from_hub(model_path)
 
     model.freeze()
-    model = apply_lora_layers(model, args.adapter_file)
+    model = apply_lora_layers(model, args.adapter_path)
 
     fused_linears = [
         (n, m.to_linear())
         for n, m in model.named_modules()
         if isinstance(m, LoRALinear)
     ]
```

### Comparing `mlx-lm-0.5.0/mlx_lm/generate.py` & `mlx-lm-0.6.0/mlx_lm/generate.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,17 +20,17 @@
     parser.add_argument(
         "--model",
         type=str,
         default="mlx_model",
         help="The path to the local model directory or Hugging Face repo.",
     )
     parser.add_argument(
-        "--adapter-file",
+        "--adapter-path",
         type=str,
-        help="Optional path for the trained adapter weights.",
+        help="Optional path for the trained adapter weights and config.",
     )
     parser.add_argument(
         "--trust-remote-code",
         action="store_true",
         help="Enable trusting remote code for tokenizer",
     )
     parser.add_argument(
@@ -106,15 +106,15 @@
 
     # Building tokenizer_config
     tokenizer_config = {"trust_remote_code": True if args.trust_remote_code else None}
     if args.eos_token is not None:
         tokenizer_config["eos_token"] = args.eos_token
 
     model, tokenizer = load(
-        args.model, adapter_file=args.adapter_file, tokenizer_config=tokenizer_config
+        args.model, adapter_path=args.adapter_path, tokenizer_config=tokenizer_config
     )
 
     if args.use_default_chat_template:
         if tokenizer.chat_template is None:
             tokenizer.chat_template = tokenizer.default_chat_template
 
     if not args.ignore_chat_template and (
```

### Comparing `mlx-lm-0.5.0/mlx_lm/gguf.py` & `mlx-lm-0.6.0/mlx_lm/gguf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import re
 from enum import IntEnum
 from pathlib import Path
-from typing import Iterable, Union
+from typing import Iterable, Optional, Set, Tuple, Union
 
 import mlx.core as mx
 from transformers import AutoTokenizer
 
 
 class TokenType(IntEnum):
     NORMAL = 1
@@ -19,15 +19,17 @@
 class GGMLFileType(IntEnum):
     GGML_TYPE_F16 = 1
 
 
 # copied from https://github.com/ggerganov/llama.cpp/blob/master/convert.py#L455
 class HfVocab:
     def __init__(
-        self, fname_tokenizer: Path, fname_added_tokens: Path | None = None
+        self,
+        fname_tokenizer: Path,
+        fname_added_tokens: Optional[Union[Path, None]] = None,
     ) -> None:
         self.tokenizer = AutoTokenizer.from_pretrained(
             fname_tokenizer,
             cache_dir=fname_tokenizer,
             local_files_only=True,
         )
         self.added_tokens_list = []
@@ -46,52 +48,52 @@
         }
         self.special_ids = set(self.tokenizer.all_special_ids)
         self.vocab_size_base = self.tokenizer.vocab_size
         self.vocab_size = self.vocab_size_base + len(self.added_tokens_list)
         self.fname_tokenizer = fname_tokenizer
         self.fname_added_tokens = fname_added_tokens
 
-    def hf_tokens(self) -> Iterable[tuple[bytes, float, TokenType]]:
+    def hf_tokens(self) -> Iterable[Tuple[bytes, float, TokenType]]:
         reverse_vocab = {
             id: encoded_tok for encoded_tok, id in self.tokenizer.get_vocab().items()
         }
         for token_id in range(self.vocab_size_base):
             if token_id in self.added_tokens_ids:
                 continue
             token_text = reverse_vocab[token_id].encode("utf-8")
             yield token_text, self.get_token_score(token_id), self.get_token_type(
                 token_id, token_text, self.special_ids
             )
 
     def get_token_type(
-        self, token_id: int, token_text: bytes, special_ids: set[int]
+        self, token_id: int, token_text: bytes, special_ids: Set[int]
     ) -> TokenType:
         if re.fullmatch(rb"<0x[0-9A-Fa-f]{2}>", token_text):
             return TokenType.BYTE
         return TokenType.CONTROL if token_id in special_ids else TokenType.NORMAL
 
     def get_token_score(self, token_id: int) -> float:
         return -1000.0
 
-    def added_tokens(self) -> Iterable[tuple[bytes, float, TokenType]]:
+    def added_tokens(self) -> Iterable[Tuple[bytes, float, TokenType]]:
         for text in self.added_tokens_list:
             if text in self.specials:
                 toktype = self.get_token_type(
                     self.specials[text], b"", self.special_ids
                 )
                 score = self.get_token_score(self.specials[text])
             else:
                 toktype = TokenType.USER_DEFINED
                 score = -1000.0
             yield text.encode("utf-8"), score, toktype
 
     def has_newline_token(self):
         return "<0x0A>" in self.tokenizer.vocab or "\n" in self.tokenizer.vocab
 
-    def all_tokens(self) -> Iterable[tuple[bytes, float, TokenType]]:
+    def all_tokens(self) -> Iterable[Tuple[bytes, float, TokenType]]:
         yield from self.hf_tokens()
         yield from self.added_tokens()
 
     def __repr__(self) -> str:
         return f"<HfVocab with {self.vocab_size_base} base tokens and {len(self.added_tokens_list)} added tokens>"
 
     @staticmethod
```

### Comparing `mlx-lm-0.5.0/mlx_lm/lora.py` & `mlx-lm-0.6.0/mlx_lm/lora.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 # Copyright © 2024 Apple Inc.
 
 import argparse
-import json
 import math
 import re
 import types
 from pathlib import Path
 
 import mlx.nn as nn
 import mlx.optimizers as optim
 import numpy as np
 import yaml
 from mlx.utils import tree_flatten
 
 from .tuner.datasets import load_dataset
 from .tuner.trainer import TrainingArgs, TrainingCallback, evaluate, train
-from .tuner.utils import linear_to_lora_layers
-from .utils import load
+from .tuner.utils import build_schedule, linear_to_lora_layers
+from .utils import load, save_config
 
 yaml_loader = yaml.SafeLoader
 yaml_loader.add_implicit_resolver(
     "tag:yaml.org,2002:float",
     re.compile(
         """^(?:
      [-+]?(?:[0-9][0-9_]*)\\.[0-9_]*(?:[eE][-+]?[0-9]+)?
@@ -44,19 +43,20 @@
     "batch_size": 4,
     "iters": 1000,
     "val_batches": 25,
     "learning_rate": 1e-5,
     "steps_per_report": 10,
     "steps_per_eval": 200,
     "resume_adapter_file": None,
-    "adapter_file": "adapters.npz",
+    "adapter_path": "adapters",
     "save_every": 100,
     "test": False,
     "test_batches": 500,
     "max_seq_length": 2048,
+    "lr_schedule": None,
     "lora_parameters": {"rank": 8, "alpha": 16, "dropout": 0.0, "scale": 10.0},
 }
 
 
 def build_parser():
     parser = argparse.ArgumentParser(description="LoRA or QLoRA finetuning.")
     parser.add_argument(
@@ -97,20 +97,20 @@
         "--steps-per-eval",
         type=int,
         help="Number of training steps between validations.",
     )
     parser.add_argument(
         "--resume-adapter-file",
         type=str,
-        help="Load path to resume training with the given adapter weights.",
+        help="Load path to resume training with the given adapters.",
     )
     parser.add_argument(
-        "--adapter-file",
+        "--adapter-path",
         type=str,
-        help="Save/load path for the trained adapter weights.",
+        help="Save/load path for the adapters.",
     )
     parser.add_argument(
         "--save-every",
         type=int,
         help="Save the model every N iterations.",
     )
     parser.add_argument(
@@ -179,49 +179,60 @@
     train_set, valid_set, test_set = load_dataset(args, tokenizer)
 
     # Resume training the given adapters.
     if args.resume_adapter_file is not None:
         print(f"Loading pretrained adapters from {args.resume_adapter_file}")
         model.load_weights(args.resume_adapter_file, strict=False)
 
+    adapter_path = Path(args.adapter_path)
+    adapter_path.mkdir(parents=True, exist_ok=True)
+    save_config(vars(args), adapter_path / "adapter_config.json")
+    adapter_file = adapter_path / "adapters.safetensors"
+
     if args.train:
         print("Training")
         # init training args
         training_args = TrainingArgs(
             batch_size=args.batch_size,
             iters=args.iters,
             val_batches=args.val_batches,
             steps_per_report=args.steps_per_report,
             steps_per_eval=args.steps_per_eval,
             steps_per_save=args.save_every,
-            adapter_file=args.adapter_file,
+            adapter_file=adapter_file,
             max_seq_length=args.max_seq_length,
             grad_checkpoint=args.grad_checkpoint,
         )
 
         model.train()
-        opt = optim.Adam(learning_rate=args.learning_rate)
+        opt = optim.Adam(
+            learning_rate=(
+                build_schedule(args.lr_schedule)
+                if args.lr_schedule
+                else args.learning_rate
+            )
+        )
         # Train model
         train(
             model=model,
             tokenizer=tokenizer,
             args=training_args,
             optimizer=opt,
             train_dataset=train_set,
             val_dataset=valid_set,
             training_callback=training_callback,
         )
 
     # Load the LoRA adapter weights which we assume should exist by this point
-    if not Path(args.adapter_file).is_file():
+    if not adapter_file.is_file():
         raise ValueError(
-            f"Adapter file {args.adapter_file} missing. "
-            "Use --train to learn and save the adapters.npz."
+            f"Adapter file {adapter_file} missing. "
+            "Use --train to learn and save the adapters"
         )
-    model.load_weights(args.adapter_file, strict=False)
+    model.load_weights(str(adapter_file), strict=False)
 
     if args.test:
         print("Testing")
         model.eval()
 
         test_loss = evaluate(
             model=model,
```

### Comparing `mlx-lm-0.5.0/mlx_lm/merge.py` & `mlx-lm-0.6.0/mlx_lm/merge.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Copyright © 2023-2024 Apple Inc.
 
 import argparse
 import glob
-import json
 import shutil
 from pathlib import Path
 from typing import Optional
 
 import mlx.core as mx
 import mlx.nn as nn
 import numpy as np
```

### Comparing `mlx-lm-0.5.0/mlx_lm/models/cohere.py` & `mlx-lm-0.6.0/mlx_lm/models/cohere.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.5.0/mlx_lm/models/gemma.py` & `mlx-lm-0.6.0/mlx_lm/models/gemma.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from dataclasses import dataclass
-from functools import partial
-from typing import Dict, Optional, Tuple, Union
+from typing import Optional, Tuple
 
 import mlx.core as mx
 import mlx.nn as nn
 
 from .base import BaseModelArgs
```

### Comparing `mlx-lm-0.5.0/mlx_lm/models/llama.py` & `mlx-lm-0.6.0/mlx_lm/models/llama.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.5.0/mlx_lm/models/mixtral.py` & `mlx-lm-0.6.0/mlx_lm/models/mixtral.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,28 +139,27 @@
 
         scores = mx.softmax(
             mx.take_along_axis(gates, inds, axis=-1).astype(mx.float32),
             axis=-1,
         ).astype(gates.dtype)
 
         if self.training:
-            mx.eval(inds)
             inds = np.array(inds)
             y = mx.zeros((x.shape[0], ne, x.shape[-1]), x.dtype)
             for e, expert in enumerate(self.experts):
                 idx1, idx2 = map(mx.array, np.where(inds == e))
                 if idx1.size == 0:
                     continue
                 y[idx1, idx2] = expert(x[idx1])
 
             y = (y * scores[:, :, None]).sum(axis=1)
         else:
             y = []
             for xt, st, it in zip(x, scores, inds.tolist()):
-                yt = mx.concatenate([self.experts[e](xt)[:, None] for e in it], axis=-1)
+                yt = mx.stack([self.experts[e](xt) for e in it], axis=-1)
                 yt = (yt * st).sum(axis=-1)
                 y.append(yt[None, :])
             y = mx.concatenate(y)
 
         return y.reshape(orig_shape)
```

### Comparing `mlx-lm-0.5.0/mlx_lm/models/olmo.py` & `mlx-lm-0.6.0/mlx_lm/models/olmo.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from dataclasses import dataclass
 from sys import exit
-from typing import Dict, Optional, Tuple, Union
+from typing import Optional, Tuple
 
 import mlx.core as mx
 import mlx.nn as nn
 
 from .base import BaseModelArgs
 
 try:
```

### Comparing `mlx-lm-0.5.0/mlx_lm/models/phi.py` & `mlx-lm-0.6.0/mlx_lm/models/phi.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.5.0/mlx_lm/models/phixtral.py` & `mlx-lm-0.6.0/mlx_lm/models/phixtral.py`

 * *Files 4% similar despite different names*

```diff
@@ -121,15 +121,15 @@
                     continue
                 y[idx1, idx2] = expert(x[idx1])
 
             y = (y * scores[..., None]).sum(axis=1)
         else:
             y = []
             for xt, st, it in zip(x, scores, inds.tolist()):
-                yt = mx.concatenate([self.mlp[e](xt)[:, None] for e in it], axis=-1)
+                yt = mx.stack([self.mlp[e](xt) for e in it], axis=-1)
                 yt = (yt * st).sum(axis=-1)
                 y.append(yt[None, :])
             y = mx.concatenate(y)
 
         return y.reshape(orig_shape)
```

### Comparing `mlx-lm-0.5.0/mlx_lm/models/plamo.py` & `mlx-lm-0.6.0/mlx_lm/models/plamo.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import dataclass
-from typing import Any, Dict, List, Optional, Tuple, Union
+from typing import Any, List, Optional, Tuple, Union
 
 import mlx.core as mx
 import mlx.nn as nn
 import numpy as np
 
 from .base import BaseModelArgs
 
@@ -179,19 +179,15 @@
 
         mask = None
         if h.shape[1] > 1:
             mask = nn.MultiHeadAttention.create_additive_causal_mask(h.shape[1])
             mask = mask.astype(self.embed_tokens.weight.dtype)
 
         if cache is None:
-            past_key_values_length = 0
             cache = [None for _ in range(len(self.layers.layers))]
-        else:
-            if cache[0] is not None:
-                past_key_values_length = cache[0][0].shape[2]
 
         for e, layer in enumerate(self.layers.layers):
             h, c = layer(h, mask, cache[e])
             if cache is not None:
                 cache[e] = c
             else:
                 cache.append(c)
```

### Comparing `mlx-lm-0.5.0/mlx_lm/models/qwen.py` & `mlx-lm-0.6.0/mlx_lm/models/qwen.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.5.0/mlx_lm/models/qwen2.py` & `mlx-lm-0.6.0/mlx_lm/models/qwen2.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.5.0/mlx_lm/models/stablelm.py` & `mlx-lm-0.6.0/mlx_lm/models/stablelm.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.5.0/mlx_lm/models/starcoder2.py` & `mlx-lm-0.6.0/mlx_lm/models/starcoder2.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.5.0/mlx_lm/sample_utils.py` & `mlx-lm-0.6.0/mlx_lm/sample_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         logits = logits.astype(mx.float32)
 
     # referenced implementation from https://github.com/huggingface/transformers/blob/main/src/transformers/generation/logits_process.py#L449-L460
     probs = mx.softmax(logits / temperature, axis=-1)
 
     # sort probs in ascending order
     sorted_indices = mx.argsort(probs, axis=-1)
-    sorted_probs = probs[..., sorted_indices]
+    sorted_probs = probs[..., sorted_indices.squeeze(0)]
 
     cumulative_probs = mx.cumsum(sorted_probs, axis=-1)
 
     # select tokens with cumulative probs below threshold
     top_probs = mx.where(
         cumulative_probs > 1 - top_p,
         sorted_probs,
```

### Comparing `mlx-lm-0.5.0/mlx_lm/server.py` & `mlx-lm-0.6.0/mlx_lm/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -414,17 +414,17 @@
     parser.add_argument(
         "--model",
         type=str,
         required=True,
         help="The path to the MLX model weights, tokenizer, and config",
     )
     parser.add_argument(
-        "--adapter-file",
+        "--adapter-path",
         type=str,
-        help="Optional path for the trained adapter weights.",
+        help="Optional path for the trained adapter weights and config.",
     )
     parser.add_argument(
         "--host",
         type=str,
         default="127.0.0.1",
         help="Host for the HTTP server (default: 127.0.0.1)",
     )
@@ -441,11 +441,11 @@
     )
     args = parser.parse_args()
 
     # Building tokenizer_config
     tokenizer_config = {"trust_remote_code": True if args.trust_remote_code else None}
 
     MODEL, TOKENIZER = load(
-        args.model, adapter_file=args.adapter_file, tokenizer_config=tokenizer_config
+        args.model, adapter_path=args.adapter_path, tokenizer_config=tokenizer_config
     )
 
     run(args.host, args.port)
```

### Comparing `mlx-lm-0.5.0/mlx_lm/tuner/datasets.py` & `mlx-lm-0.6.0/mlx_lm/tuner/datasets.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.5.0/mlx_lm/tuner/lora.py` & `mlx-lm-0.6.0/mlx_lm/tuner/lora.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.5.0/mlx_lm/tuner/trainer.py` & `mlx-lm-0.6.0/mlx_lm/tuner/trainer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Copyright © 2024 Apple Inc.
 
 import time
 from dataclasses import dataclass, field
 from functools import partial
 from pathlib import Path
+from typing import Union
 
 import mlx.core as mx
 import mlx.nn as nn
 import numpy as np
 from mlx.utils import tree_flatten
 
 
@@ -50,15 +51,15 @@
     steps_per_save: int = field(
         default=100, metadata={"help": "Save the model every number steps"}
     )
     max_seq_length: int = field(
         default=2048, metadata={"help": "Maximum sequence length."}
     )
     adapter_file: str = field(
-        default="adapter.npz",
+        default="adapters.safetensors",
         metadata={"help": "Save/load path for the trained adapter weights."},
     )
     grad_checkpoint: bool = field(
         default=False,
         metadata={"help": "Use gradient checkpointing to reduce memory use."},
     )
 
@@ -168,26 +169,14 @@
     args: TrainingArgs = TrainingArgs(),
     loss: callable = default_loss,
     iterate_batches: callable = iterate_batches,
     training_callback: TrainingCallback = None,
 ):
     print(f"Starting training..., iters: {args.iters}")
 
-    def checkpoints_path(adapter_file) -> str:
-        checkpoints_path = Path("checkpoints")
-        if Path(adapter_file).parent:
-            checkpoints_path = Path(adapter_file).parent / "checkpoints"
-
-        checkpoints_path.mkdir(parents=True, exist_ok=True)
-
-        return str(checkpoints_path)
-
-    # Create checkpoints directory if it does not exist
-    adapter_path = checkpoints_path(args.adapter_file)
-
     if args.grad_checkpoint:
         grad_checkpoint(model.layers[0])
 
     state = [model.state, optimizer.state]
 
     def step(batch):
         # Forward and backward pass
@@ -202,15 +191,15 @@
 
     losses = []
     n_tokens = 0
     trained_tokens = 0
     # Main training loop
     start = time.perf_counter()
     for it, batch in zip(
-        range(args.iters),
+        range(1, args.iters + 1),
         iterate_batches(
             dataset=train_dataset,
             tokenizer=tokenizer,
             batch_size=args.batch_size,
             max_seq_length=args.max_seq_length,
             train=True,
         ),
@@ -219,91 +208,92 @@
         mx.eval(state, lvalue, toks)
 
         # Record loss
         losses.append(lvalue.item())
         n_tokens += toks.item()
 
         # Report training loss if needed
-        if ((it + 1) % args.steps_per_report == 0) or (it + 1 == args.iters):
+        if it % args.steps_per_report == 0 or it == args.iters:
             train_loss = np.mean(losses)
 
             stop = time.perf_counter()
             learning_rate = optimizer.learning_rate.item()
             it_sec = args.steps_per_report / (stop - start)
             tokens_sec = float(n_tokens) / (stop - start)
             trained_tokens += n_tokens
             peak_mem = mx.metal.get_peak_memory() / 2**30
             print(
-                f"Iter {it + 1}: Train loss {train_loss:.3f}, "
+                f"Iter {it}: Train loss {train_loss:.3f}, "
                 f"Learning Rate {learning_rate:.3e}, "
                 f"It/sec {it_sec:.3f}, "
                 f"Tokens/sec {tokens_sec:.3f}, "
                 f"Trained Tokens {trained_tokens}, "
                 f"Peak mem {peak_mem:.3f} GB"
             )
 
             if training_callback is not None:
                 train_info = {
-                    "iteration": it + 1,
+                    "iteration": it,
                     "train_loss": train_loss,
                     "learning_rate": learning_rate,
                     "iterations_per_second": it_sec,
                     "tokens_per_second": tokens_sec,
                     "trained_tokens": trained_tokens,
                     "peak_memory": peak_mem,
                 }
                 training_callback.on_train_loss_report(train_info)
 
             losses = []
             n_tokens = 0
             start = time.perf_counter()
 
         # Report validation loss if needed
-        if it == 0 or ((it + 1) % args.steps_per_eval == 0) or (it + 1 == args.iters):
+        if it == 1 or it % args.steps_per_eval == 0 or it == args.iters:
             stop = time.perf_counter()
             val_loss = evaluate(
                 model=model,
                 dataset=val_dataset,
                 loss=loss,
                 tokenizer=tokenizer,
                 batch_size=args.batch_size,
                 num_batches=args.val_batches,
                 max_seq_length=args.max_seq_length,
                 iterate_batches=iterate_batches,
             )
             val_time = time.perf_counter() - stop
             print(
-                f"Iter {it + 1}: "
-                f"Val loss {val_loss:.3f}, "
-                f"Val took {val_time:.3f}s"
+                f"Iter {it}: " f"Val loss {val_loss:.3f}, " f"Val took {val_time:.3f}s"
             )
 
             if training_callback is not None:
                 val_info = {
-                    "iteration": it + 1,
+                    "iteration": it,
                     "val_loss": val_loss,
                     "val_time": val_time,
                 }
                 training_callback.on_val_loss_report(val_info)
 
             start = time.perf_counter()
 
-        # Save adapter weights if needed
-        if (it + 1) % args.steps_per_save == 0:
-            checkpoint_adapter_file = (
-                f"{adapter_path}/{it + 1}_{Path(args.adapter_file).name}"
+        # Save adapter weights
+        if it % args.steps_per_save == 0:
+            save_adapter(model, args.adapter_file)
+            checkpoint = (
+                Path(args.adapter_file).parent / f"{it:07d}_adapters.safetensors"
+            )
+            save_adapter(model, checkpoint)
+            print(
+                f"Iter {it}: Saved adapter weights to "
+                f"{args.adapter_file} and {checkpoint}."
             )
-            save_adapter(model=model, adapter_file=checkpoint_adapter_file)
-            print(f"Iter {it + 1}: Saved adapter weights to {checkpoint_adapter_file}.")
 
     # save final adapter weights
-    save_adapter(model=model, adapter_file=args.adapter_file)
+    save_adapter(model, args.adapter_file)
     print(f"Saved final adapter weights to {args.adapter_file}.")
 
 
 def save_adapter(
     model: nn.Module,
-    adapter_file: str,
+    adapter_file: Union[str, Path],
 ):
     flattened_tree = tree_flatten(model.trainable_parameters())
-
-    mx.savez(adapter_file, **dict(flattened_tree))
+    mx.save_safetensors(str(adapter_file), dict(flattened_tree))
```

### Comparing `mlx-lm-0.5.0/mlx_lm/tuner/utils.py` & `mlx-lm-0.6.0/mlx_lm/tuner/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,41 @@
-import os
+# Copyright © 2024 Apple Inc.
+import json
+import types
+from pathlib import Path
 from typing import Dict
 
 import mlx.core as mx
 import mlx.nn as nn
+import mlx.optimizers as opt
 from mlx.utils import tree_unflatten
 
 from .lora import LoRALinear
 
 
+def build_schedule(schedule_config: Dict):
+    """
+    Build a learning rate schedule from the given config.
+    """
+    schedule_fn = getattr(opt.schedulers, schedule_config["name"])
+    arguments = schedule_config["arguments"]
+    initial_lr = arguments[0]
+    bound_schedule_fn = schedule_fn(*arguments)
+    if warmup_steps := schedule_config.get("warmup", 0):
+        warmup_init = schedule_config.get("warmup_init", 0.0)
+        warmup_fn = opt.schedulers.linear_schedule(
+            warmup_init, initial_lr, warmup_steps
+        )
+        return opt.schedulers.join_schedules(
+            [warmup_fn, bound_schedule_fn], [warmup_steps + 1]
+        )
+    else:
+        return bound_schedule_fn
+
+
 def linear_to_lora_layers(
     model: nn.Module,
     num_lora_layers: int,
     config: Dict,
 ):
     """
     Convert some of the models linear layers to lora layers.
@@ -45,63 +69,57 @@
     elif model.model_type in [
         "mistral",
         "llama",
         "phi",
         "mixtral",
         "stablelm",
         "qwen2",
+        "qwen2_moe",
         "gemma",
         "starcoder2",
         "cohere",
     ]:
         keys = set(["self_attn.q_proj", "self_attn.v_proj"])
         if model.model_type == "mixtral":
             keys.add("block_sparse_moe.gate")
+        if model.model_type == "qwen2_moe":
+            keys.add("mlp.gate")
+            keys.add("mlp.shared_expert_gate")
     elif model.model_type == "olmo":
         keys = set(["att_proj"])
     elif model.model_type == "phi-msft":
         keys = set(["mixer.Wqkv", "moe.gate"])
+    elif model.model_type == "dbrx":
+        keys = set(["norm_attn_norm.attn.Wqkv", "ffn.router.layer"])
     else:
         raise ValueError(f"Lora does not support {model.model_type}")
 
     for l in model.layers[num_layers - num_lora_layers :]:
-        modules = l.named_modules()
         lora_layers = [(k, to_lora(m)) for k, m in l.named_modules() if k in keys]
         l.update_modules(tree_unflatten(lora_layers))
 
 
-def apply_lora_layers(model: nn.Module, adapter_file: str) -> nn.Module:
+def apply_lora_layers(model: nn.Module, adapter_path: str) -> nn.Module:
     """
     Apply LoRA layers to the model.
 
     Args:
         model (nn.Module): The neural network model.
-        adapter_file (str): Path to the adapter configuration file.
+        adapter_path (str): Path to the adapter configuration file.
 
     Returns:
         nn.Module: The updated model with LoRA layers applied.
     """
-    if not os.path.exists(adapter_file):
-        raise FileNotFoundError(f"The adapter file does not exist: {adapter_file}")
-
-    adapters = list(mx.load(adapter_file).items())
-
-    linear_replacements = []
-    lora_layers = set(
-        [name.replace(".lora_a", "").replace(".lora_b", "") for name, _ in adapters]
-    )
-    for name, module in model.named_modules():
-        if name in lora_layers:
-            replacement_module = LoRALinear.from_linear(module)
-            linear_replacements.append((name, replacement_module))
-
-    model.update_modules(tree_unflatten(linear_replacements))
-
-    model.update(tree_unflatten(adapters))
-
+    adapter_path = Path(adapter_path)
+    if not adapter_path.exists():
+        raise FileNotFoundError(f"The adapter path does not exist: {adapter_path}")
+    with open(adapter_path / "adapter_config.json", "r") as fid:
+        config = types.SimpleNamespace(**json.load(fid))
+    linear_to_lora_layers(model, config.lora_layers, config.lora_parameters)
+    model.load_weights(str(adapter_path / "adapters.safetensors"), strict=False)
     return model
 
 
 def dequantize(model: nn.Module) -> nn.Module:
     """
     Dequantize the quantized linear layers in the model.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mlx-lm-0.5.0/mlx_lm/utils.py` & `mlx-lm-0.6.0/mlx_lm/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import importlib
 import json
 import logging
 import shutil
 import time
 from pathlib import Path
 from textwrap import dedent
-from typing import Any, Callable, Dict, Generator, List, Optional, Tuple, Union
+from typing import Any, Callable, Dict, Generator, Optional, Tuple, Union
 
 import mlx.core as mx
 import mlx.nn as nn
 from huggingface_hub import snapshot_download
 from mlx.utils import tree_flatten
 from transformers import AutoConfig, AutoTokenizer, PreTrainedTokenizer
 
@@ -235,20 +235,21 @@
             temp,
             repetition_penalty,
             repetition_context_size,
             top_p,
         ),
         range(max_tokens),
     ):
-        if token == tokenizer.eos_token_id:
-            break
+        token = token.item()
         if n == 0:
             prompt_time = time.perf_counter() - tic
             tic = time.perf_counter()
-        tokens.append(token.item())
+        if token == tokenizer.eos_token_id:
+            break
+        tokens.append(token)
 
         if verbose:
             s = tokenizer.decode(tokens)
             if formatter:
                 formatter(s[skip:], prob.item())
                 skip = len(s)
             elif s[-1] != REPLACEMENT_CHAR:
@@ -349,41 +350,41 @@
     model.eval()
     return model
 
 
 def load(
     path_or_hf_repo: str,
     tokenizer_config={},
-    adapter_file: Optional[str] = None,
+    adapter_path: Optional[str] = None,
     lazy: bool = False,
 ) -> Tuple[nn.Module, PreTrainedTokenizer]:
     """
     Load the model and tokenizer from a given path or a huggingface repository.
 
     Args:
         path_or_hf_repo (Path): The path or the huggingface repository to load the model from.
         tokenizer_config (dict, optional): Configuration parameters specifically for the tokenizer.
             Defaults to an empty dictionary.
-        adapter_file (str, optional): Path to the adapter file. If provided, applies LoRA layers to the model.
-            Defaults to None.
+        adapter_path (str, optional): Path to the LoRA adapters. If provided, applies LoRA layers
+            to the model. Default: ``None``.
         lazy (bool): If False eval the model parameters to make sure they are
             loaded in memory before returning, otherwise they will be loaded
             when needed. Default: ``False``
     Returns:
         Tuple[nn.Module, PreTrainedTokenizer]: A tuple containing the loaded model and tokenizer.
 
     Raises:
         FileNotFoundError: If config file or safetensors are not found.
         ValueError: If model class or args class are not found.
     """
     model_path = get_model_path(path_or_hf_repo)
 
     model = load_model(model_path, lazy)
-    if adapter_file is not None:
-        model = apply_lora_layers(model, adapter_file)
+    if adapter_path is not None:
+        model = apply_lora_layers(model, adapter_path)
         model.eval()
 
     tokenizer = AutoTokenizer.from_pretrained(model_path, **tokenizer_config)
     return model, tokenizer
 
 
 def fetch_from_hub(
```

### Comparing `mlx-lm-0.5.0/mlx_lm.egg-info/PKG-INFO` & `mlx-lm-0.6.0/mlx_lm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlx-lm
-Version: 0.5.0
+Version: 0.6.0
 Summary: LLMs on Apple silicon with MLX and the Hugging Face Hub
 Home-page: https://github.com/ml-explore/mlx-examples
 Author: MLX Contributors
 Author-email: mlx@group.apple.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `mlx-lm-0.5.0/mlx_lm.egg-info/SOURCES.txt` & `mlx-lm-0.6.0/mlx_lm.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -18,28 +18,31 @@
 mlx_lm.egg-info/SOURCES.txt
 mlx_lm.egg-info/dependency_links.txt
 mlx_lm.egg-info/requires.txt
 mlx_lm.egg-info/top_level.txt
 mlx_lm/models/__init__.py
 mlx_lm/models/base.py
 mlx_lm/models/cohere.py
+mlx_lm/models/dbrx.py
 mlx_lm/models/gemma.py
 mlx_lm/models/llama.py
 mlx_lm/models/mixtral.py
 mlx_lm/models/olmo.py
 mlx_lm/models/phi.py
 mlx_lm/models/phixtral.py
 mlx_lm/models/plamo.py
 mlx_lm/models/qwen.py
 mlx_lm/models/qwen2.py
+mlx_lm/models/qwen2_moe.py
 mlx_lm/models/stablelm.py
 mlx_lm/models/starcoder2.py
 mlx_lm/tuner/__init__.py
 mlx_lm/tuner/datasets.py
 mlx_lm/tuner/lora.py
 mlx_lm/tuner/trainer.py
 mlx_lm/tuner/utils.py
 tests/test_datsets.py
+tests/test_gguf.py
 tests/test_lora.py
 tests/test_models.py
 tests/test_sample_utils.py
 tests/test_utils.py
```

### Comparing `mlx-lm-0.5.0/setup.py` & `mlx-lm-0.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.5.0/tests/test_datsets.py` & `mlx-lm-0.6.0/tests/test_datsets.py`

 * *Files identical despite different names*

### Comparing `mlx-lm-0.5.0/tests/test_models.py` & `mlx-lm-0.6.0/tests/test_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,14 +110,35 @@
         self.model_test_runner(
             model,
             args.model_type,
             args.vocab_size,
             args.n_layers,
         )
 
+    def test_qwen2_moe(self):
+        from mlx_lm.models import qwen2_moe
+
+        args = qwen2_moe.ModelArgs(
+            model_type="qwen2_moe",
+            hidden_size=1024,
+            num_hidden_layers=4,
+            intermediate_size=2048,
+            num_attention_heads=4,
+            rms_norm_eps=1e-5,
+            vocab_size=10_000,
+            num_experts_per_tok=4,
+            num_experts=16,
+            moe_intermediate_size=1024,
+            shared_expert_intermediate_size=2048,
+        )
+        model = qwen2_moe.Model(args)
+        self.model_test_runner(
+            model, args.model_type, args.vocab_size, args.num_hidden_layers
+        )
+
     def test_qwen2(self):
         from mlx_lm.models import qwen2
 
         args = qwen2.ModelArgs(
             model_type="qwen2",
             hidden_size=1024,
             num_hidden_layers=4,
```

### Comparing `mlx-lm-0.5.0/tests/test_sample_utils.py` & `mlx-lm-0.6.0/tests/test_sample_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 import unittest
 from unittest.mock import patch
 
 import mlx.core as mx
 from mlx_lm.sample_utils import top_p_sampling
 
 
-class TestLora(unittest.TestCase):
+class TestSamplingUtils(unittest.TestCase):
     @patch("mlx.core.random.categorical")
     def test_top_p_sampling(self, mock_categorical):
         logits = mx.array([[1.0, 2.0, 3.0, 4.0]])
         top_p = 0.3
         temperature = 1.0
         expected_token = mx.array([3])
         mock_categorical.return_value = expected_token
 
         token = top_p_sampling(logits, top_p, temperature)
         expected_top_probs = mx.array([[0.0, 0.0, 0.0, 0.643914]])
         self.assertTrue(mx.allclose(token, expected_token))
         args, _ = mock_categorical.call_args
+        self.assertTrue(args[0].shape == expected_top_probs.shape)
         self.assertTrue(mx.allclose(args[0], mx.log(expected_top_probs)))
 
         logits = mx.array([[1.0, 2.0, 3.0, 4.0]])
         top_p = 0.9
         temperature = 1.0
         expected_token = mx.array([3])
         mock_categorical.return_value = expected_token
 
         token = top_p_sampling(logits, top_p, temperature)
         expected_top_probs = mx.array([[0.0, 0.0871443, 0.236883, 0.643914]])
         self.assertTrue(mx.allclose(token, expected_token))
         args, _ = mock_categorical.call_args
+        self.assertTrue(args[0].shape == expected_top_probs.shape)
         self.assertTrue(mx.allclose(args[0], mx.log(expected_top_probs)))
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `mlx-lm-0.5.0/tests/test_utils.py` & `mlx-lm-0.6.0/tests/test_utils.py`

 * *Files identical despite different names*

