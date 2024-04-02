# Comparing `tmp/torchao-nightly-2024.4.1.tar.gz` & `tmp/torchao-nightly-2024.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchao-nightly-2024.4.1.tar", last modified: Mon Apr  1 00:21:27 2024, max compression
+gzip compressed data, was "torchao-nightly-2024.4.2.tar", last modified: Tue Apr  2 00:18:52 2024, max compression
```

## Comparing `torchao-nightly-2024.4.1.tar` & `torchao-nightly-2024.4.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:21:27.986942 torchao-nightly-2024.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-01 00:21:14.000000 torchao-nightly-2024.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-04-01 00:21:27.986942 torchao-nightly-2024.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5062 2024-04-01 00:21:14.000000 torchao-nightly-2024.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 00:21:27.986942 torchao-nightly-2024.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-01 00:21:14.000000 torchao-nightly-2024.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:21:27.982942 torchao-nightly-2024.4.1/torchao/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-01 00:21:14.000000 torchao-nightly-2024.4.1/torchao/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:21:27.982942 torchao-nightly-2024.4.1/torchao/dtypes/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-01 00:21:14.000000 torchao-nightly-2024.4.1/torchao/dtypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20810 2024-04-01 00:21:14.000000 torchao-nightly-2024.4.1/torchao/dtypes/nf4tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)    12448 2024-04-01 00:21:14.000000 torchao-nightly-2024.4.1/torchao/dtypes/uint4.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:21:27.982942 torchao-nightly-2024.4.1/torchao/kernel/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 00:21:14.000000 torchao-nightly-2024.4.1/torchao/kernel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7389 2024-04-01 00:21:14.000000 torchao-nightly-2024.4.1/torchao/kernel/autotuner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-04-01 00:21:14.000000 torchao-nightly-2024.4.1/torchao/kernel/intmm.py
--rw-r--r--   0 runner    (1001) docker     (127)    11512 2024-04-01 00:21:14.000000 torchao-nightly-2024.4.1/torchao/kernel/intmm_triton.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:21:27.986942 torchao-nightly-2024.4.1/torchao/quantization/
--rw-r--r--   0 runner    (1001) docker     (127)    46611 2024-04-01 00:21:14.000000 torchao-nightly-2024.4.1/torchao/quantization/GPTQ.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-01 00:21:14.000000 torchao-nightly-2024.4.1/torchao/quantization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-01 00:21:14.000000 torchao-nightly-2024.4.1/torchao/quantization/dynamic_quant.py
--rw-r--r--   0 runner    (1001) docker     (127)     6254 2024-04-01 00:21:14.000000 torchao-nightly-2024.4.1/torchao/quantization/quant_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    19107 2024-04-01 00:21:14.000000 torchao-nightly-2024.4.1/torchao/quantization/quant_primitives.py
--rw-r--r--   0 runner    (1001) docker     (127)     9159 2024-04-01 00:21:14.000000 torchao-nightly-2024.4.1/torchao/quantization/smoothquant.py
--rw-r--r--   0 runner    (1001) docker     (127)    17574 2024-04-01 00:21:14.000000 torchao-nightly-2024.4.1/torchao/quantization/subclass.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-01 00:21:14.000000 torchao-nightly-2024.4.1/torchao/quantization/unified.py
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-04-01 00:21:14.000000 torchao-nightly-2024.4.1/torchao/quantization/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-04-01 00:21:14.000000 torchao-nightly-2024.4.1/torchao/quantization/weight_only.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:21:27.986942 torchao-nightly-2024.4.1/torchao/sparsity/
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-01 00:21:14.000000 torchao-nightly-2024.4.1/torchao/sparsity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-04-01 00:21:14.000000 torchao-nightly-2024.4.1/torchao/sparsity/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-04-01 00:21:14.000000 torchao-nightly-2024.4.1/torchao/sparsity/wanda.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:21:27.986942 torchao-nightly-2024.4.1/torchao_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-04-01 00:21:27.000000 torchao-nightly-2024.4.1/torchao_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-01 00:21:27.000000 torchao-nightly-2024.4.1/torchao_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 00:21:27.000000 torchao-nightly-2024.4.1/torchao_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-01 00:21:27.000000 torchao-nightly-2024.4.1/torchao_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-01 00:21:27.000000 torchao-nightly-2024.4.1/torchao_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:18:52.431520 torchao-nightly-2024.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-02 00:18:42.000000 torchao-nightly-2024.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-04-02 00:18:52.431520 torchao-nightly-2024.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5062 2024-04-02 00:18:42.000000 torchao-nightly-2024.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 00:18:52.431520 torchao-nightly-2024.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-02 00:18:42.000000 torchao-nightly-2024.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:18:52.427520 torchao-nightly-2024.4.2/torchao/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-02 00:18:42.000000 torchao-nightly-2024.4.2/torchao/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:18:52.427520 torchao-nightly-2024.4.2/torchao/dtypes/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-02 00:18:42.000000 torchao-nightly-2024.4.2/torchao/dtypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20810 2024-04-02 00:18:42.000000 torchao-nightly-2024.4.2/torchao/dtypes/nf4tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12448 2024-04-02 00:18:42.000000 torchao-nightly-2024.4.2/torchao/dtypes/uint4.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:18:52.427520 torchao-nightly-2024.4.2/torchao/kernel/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 00:18:42.000000 torchao-nightly-2024.4.2/torchao/kernel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7389 2024-04-02 00:18:42.000000 torchao-nightly-2024.4.2/torchao/kernel/autotuner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-04-02 00:18:42.000000 torchao-nightly-2024.4.2/torchao/kernel/intmm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11512 2024-04-02 00:18:42.000000 torchao-nightly-2024.4.2/torchao/kernel/intmm_triton.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:18:52.427520 torchao-nightly-2024.4.2/torchao/quantization/
+-rw-r--r--   0 runner    (1001) docker     (127)    46651 2024-04-02 00:18:42.000000 torchao-nightly-2024.4.2/torchao/quantization/GPTQ.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-02 00:18:42.000000 torchao-nightly-2024.4.2/torchao/quantization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-02 00:18:42.000000 torchao-nightly-2024.4.2/torchao/quantization/dynamic_quant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6266 2024-04-02 00:18:42.000000 torchao-nightly-2024.4.2/torchao/quantization/quant_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19180 2024-04-02 00:18:42.000000 torchao-nightly-2024.4.2/torchao/quantization/quant_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9159 2024-04-02 00:18:42.000000 torchao-nightly-2024.4.2/torchao/quantization/smoothquant.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17574 2024-04-02 00:18:42.000000 torchao-nightly-2024.4.2/torchao/quantization/subclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-02 00:18:42.000000 torchao-nightly-2024.4.2/torchao/quantization/unified.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-04-02 00:18:42.000000 torchao-nightly-2024.4.2/torchao/quantization/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-04-02 00:18:42.000000 torchao-nightly-2024.4.2/torchao/quantization/weight_only.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:18:52.427520 torchao-nightly-2024.4.2/torchao/sparsity/
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-02 00:18:42.000000 torchao-nightly-2024.4.2/torchao/sparsity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-04-02 00:18:42.000000 torchao-nightly-2024.4.2/torchao/sparsity/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-04-02 00:18:42.000000 torchao-nightly-2024.4.2/torchao/sparsity/wanda.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:18:52.431520 torchao-nightly-2024.4.2/torchao_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-04-02 00:18:52.000000 torchao-nightly-2024.4.2/torchao_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-02 00:18:52.000000 torchao-nightly-2024.4.2/torchao_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 00:18:52.000000 torchao-nightly-2024.4.2/torchao_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-02 00:18:52.000000 torchao-nightly-2024.4.2/torchao_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-02 00:18:52.000000 torchao-nightly-2024.4.2/torchao_nightly.egg-info/top_level.txt
```

### Comparing `torchao-nightly-2024.4.1/LICENSE` & `torchao-nightly-2024.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `torchao-nightly-2024.4.1/PKG-INFO` & `torchao-nightly-2024.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchao-nightly
-Version: 2024.4.1
+Version: 2024.4.2
 Summary: Package for applying ao techniques to GPU models
 Home-page: https://github.com/pytorch-labs/ao
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch
 Requires-Dist: numpy
 Requires-Dist: sentencepiece
```

### Comparing `torchao-nightly-2024.4.1/README.md` & `torchao-nightly-2024.4.2/README.md`

 * *Files identical despite different names*

### Comparing `torchao-nightly-2024.4.1/setup.py` & `torchao-nightly-2024.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `torchao-nightly-2024.4.1/torchao/dtypes/nf4tensor.py` & `torchao-nightly-2024.4.2/torchao/dtypes/nf4tensor.py`

 * *Files identical despite different names*

### Comparing `torchao-nightly-2024.4.1/torchao/dtypes/uint4.py` & `torchao-nightly-2024.4.2/torchao/dtypes/uint4.py`

 * *Files identical despite different names*

### Comparing `torchao-nightly-2024.4.1/torchao/kernel/autotuner.py` & `torchao-nightly-2024.4.2/torchao/kernel/autotuner.py`

 * *Files identical despite different names*

### Comparing `torchao-nightly-2024.4.1/torchao/kernel/intmm.py` & `torchao-nightly-2024.4.2/torchao/kernel/intmm.py`

 * *Files identical despite different names*

### Comparing `torchao-nightly-2024.4.1/torchao/kernel/intmm_triton.py` & `torchao-nightly-2024.4.2/torchao/kernel/intmm_triton.py`

 * *Files identical despite different names*

### Comparing `torchao-nightly-2024.4.1/torchao/quantization/GPTQ.py` & `torchao-nightly-2024.4.2/torchao/quantization/GPTQ.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import torch.fx as fx
 import torch.nn as nn
 import torch.nn.functional as F
 
 # from model import Transformer  # pyre-ignore[21]
 from torch.utils._pytree import tree_flatten, tree_unflatten
 
-from .utils import TORCH_VERSION_AFTER_2_4
+from .utils import TORCH_VERSION_AFTER_2_3
 from typing import Any, Dict, Tuple, Optional
 from .unified import Quantizer
 from functools import reduce
 from math import gcd
 
 aten = torch.ops.aten
 
@@ -85,15 +85,15 @@
             self._max_seq_length = calibration_seq_length
             self.calibration_seq_length = calibration_seq_length
 
             # need to take inps and convert to corrent input
             # for model
             self.input_prep_func = (
                 input_prep_func if input_prep_func is not None
-                else lambda x: x
+                else lambda x: (x,)
             )
 
             self.pad_calibration_inputs = pad_calibration_inputs
             self.pad_token = pad_token
 
             self.inputs = None
 
@@ -176,14 +176,15 @@
 
             # pad or truncate to the right size
             if T >= self.calibration_seq_length:
                 inps = inps[: self.calibration_seq_length]
             else:
                 inps = F.pad(inps, (self.pad_token, self.calibration_seq_length - T))
 
+            inps = inps.unsqueeze(0)
             model_in = self.input_prep_func(inps)
 
             self.add_input(model_in)
 
             # output `something` with correct shape to keep eval going
             return torch.randn(
                 (1, T, self.vocab_size), dtype=torch.bfloat16, device=self._device
@@ -542,15 +543,15 @@
 
         #  `combine_qparams_list_func`.
         all_qparams = self.combine_qparams_list_func(all_qparams)
         Q = self.quantize_func(DQ, all_qparams)
         return Q, DQ.to(orig_dtype), all_qparams
 
 
-if TORCH_VERSION_AFTER_2_4:
+if TORCH_VERSION_AFTER_2_3:
     from .quant_primitives import (
         get_group_qparams_symmetric,
         group_quantize_tensor_symmetric,
         per_token_dynamic_quant,
     )
 
     class GPTQQuantizer(Quantizer):
```

### Comparing `torchao-nightly-2024.4.1/torchao/quantization/__init__.py` & `torchao-nightly-2024.4.2/torchao/quantization/__init__.py`

 * *Files identical despite different names*

### Comparing `torchao-nightly-2024.4.1/torchao/quantization/dynamic_quant.py` & `torchao-nightly-2024.4.2/torchao/quantization/dynamic_quant.py`

 * *Files identical despite different names*

### Comparing `torchao-nightly-2024.4.1/torchao/quantization/quant_api.py` & `torchao-nightly-2024.4.2/torchao/quantization/quant_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,18 +42,22 @@
     "TwoStepQuantizer",
 ]
 
 if TORCH_VERSION_AFTER_2_3:
     from .GPTQ import (
         Int8DynActInt4WeightQuantizer,
         Int8DynActInt4WeightGPTQQuantizer,
+        Int4WeightQuantizer,
+        Int4WeightGPTQQuantizer,
     )
     __all__ += [
         "Int8DynActInt4WeightQuantizer",
         "Int8DynActInt4WeightGPTQQuantizer",
+        "Int4WeightQuantizer",
+        "Int4WeightGPTQQuantizer",
     ]
 
 
 def _replace_with_custom_fn_if_matches_filter(
     model,
     replacement_fn,
     filter_fn,
@@ -192,10 +196,7 @@
         filter_fn = lambda mod, *args: isinstance(
             mod, torch.nn.Conv2d
         ) and mod.kernel_size == (1, 1)
 
     _replace_with_custom_fn_if_matches_filter(
         model, replace_conv2d_1x1, filter_fn=filter_fn
     )
-
-if TORCH_VERSION_AFTER_2_3:
-    from .GPTQ import Int8DynActInt4WeightQuantizer, Int8DynActInt4WeightGPTQQuantizer
```

### Comparing `torchao-nightly-2024.4.1/torchao/quantization/quant_primitives.py` & `torchao-nightly-2024.4.2/torchao/quantization/quant_primitives.py`

 * *Files 2% similar despite different names*

```diff
@@ -466,14 +466,15 @@
 ):
     scales, zeros = unpack_tinygemm_scales_and_zeros(scales_and_zeros)
     return groupwise_affine_dequantize_tensor_from_qparams(
         w_int4x8, scales, zeros, n_bit, groupsize
     )
 
 
+# TODO: replace this with torch.ao.quantization.PerChannelMinMaxObserver
 def get_group_qparams_symmetric(w, n_bit=4, groupsize=128, precision=torch.float32):
     # needed for GPTQ with padding
     if groupsize > w.shape[-1]:
         groupsize = w.shape[-1]
     assert groupsize > 1
     assert w.shape[-1] % groupsize == 0
     assert w.dim() == 2
```

### Comparing `torchao-nightly-2024.4.1/torchao/quantization/smoothquant.py` & `torchao-nightly-2024.4.2/torchao/quantization/smoothquant.py`

 * *Files identical despite different names*

### Comparing `torchao-nightly-2024.4.1/torchao/quantization/subclass.py` & `torchao-nightly-2024.4.2/torchao/quantization/subclass.py`

 * *Files identical despite different names*

### Comparing `torchao-nightly-2024.4.1/torchao/quantization/unified.py` & `torchao-nightly-2024.4.2/torchao/quantization/unified.py`

 * *Files identical despite different names*

### Comparing `torchao-nightly-2024.4.1/torchao/quantization/utils.py` & `torchao-nightly-2024.4.2/torchao/quantization/utils.py`

 * *Files identical despite different names*

### Comparing `torchao-nightly-2024.4.1/torchao/quantization/weight_only.py` & `torchao-nightly-2024.4.2/torchao/quantization/weight_only.py`

 * *Files identical despite different names*

### Comparing `torchao-nightly-2024.4.1/torchao/sparsity/utils.py` & `torchao-nightly-2024.4.2/torchao/sparsity/utils.py`

 * *Files identical despite different names*

### Comparing `torchao-nightly-2024.4.1/torchao/sparsity/wanda.py` & `torchao-nightly-2024.4.2/torchao/sparsity/wanda.py`

 * *Files identical despite different names*

### Comparing `torchao-nightly-2024.4.1/torchao_nightly.egg-info/PKG-INFO` & `torchao-nightly-2024.4.2/torchao_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchao-nightly
-Version: 2024.4.1
+Version: 2024.4.2
 Summary: Package for applying ao techniques to GPU models
 Home-page: https://github.com/pytorch-labs/ao
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch
 Requires-Dist: numpy
 Requires-Dist: sentencepiece
```

### Comparing `torchao-nightly-2024.4.1/torchao_nightly.egg-info/SOURCES.txt` & `torchao-nightly-2024.4.2/torchao_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

