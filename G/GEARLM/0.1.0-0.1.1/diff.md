# Comparing `tmp/GEARLM-0.1.0.tar.gz` & `tmp/GEARLM-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GEARLM-0.1.0.tar", last modified: Tue Apr  2 03:15:54 2024, max compression
+gzip compressed data, was "GEARLM-0.1.1.tar", last modified: Tue Apr  2 04:48:53 2024, max compression
```

## Comparing `GEARLM-0.1.0.tar` & `GEARLM-0.1.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 03:15:54.080109 GEARLM-0.1.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 03:15:54.080109 GEARLM-0.1.0/GEARLM/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 03:15:54.080109 GEARLM-0.1.0/GEARLM/Simulated/
--rw-r--r--   0 root         (0) root         (0)      310 2024-03-22 00:04:17.000000 GEARLM-0.1.0/GEARLM/Simulated/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16116 2024-03-22 00:04:17.000000 GEARLM-0.1.0/GEARLM/Simulated/cache_utils.py
--rw-r--r--   0 root         (0) root         (0)    10002 2024-03-24 20:13:11.000000 GEARLM-0.1.0/GEARLM/Simulated/compress_config.py
--rw-r--r--   0 root         (0) root         (0)    41018 2024-04-02 01:03:28.000000 GEARLM-0.1.0/GEARLM/Simulated/compress_function.py
--rw-r--r--   0 root         (0) root         (0)     1957 2024-03-22 00:04:17.000000 GEARLM-0.1.0/GEARLM/Simulated/cpp_kernels.py
--rw-r--r--   0 root         (0) root         (0)    65060 2024-03-22 00:04:17.000000 GEARLM-0.1.0/GEARLM/Simulated/h2o_llama_self_written.py
--rw-r--r--   0 root         (0) root         (0)    74701 2024-03-26 04:08:05.000000 GEARLM-0.1.0/GEARLM/Simulated/modeling_llama_new.py
--rw-r--r--   0 root         (0) root         (0)    65613 2024-03-22 00:04:17.000000 GEARLM-0.1.0/GEARLM/Simulated/modeling_mistral.py
--rw-r--r--   0 root         (0) root         (0)    68919 2024-03-22 00:04:17.000000 GEARLM-0.1.0/GEARLM/Simulated/modeling_mixtral.py
--rw-r--r--   0 root         (0) root         (0)     3047 2024-03-22 00:04:17.000000 GEARLM-0.1.0/GEARLM/Simulated/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 03:15:54.080109 GEARLM-0.1.0/GEARLM/TrueCompression/
--rw-r--r--   0 root         (0) root         (0)       89 2024-03-22 00:04:17.000000 GEARLM-0.1.0/GEARLM/TrueCompression/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 03:15:54.080109 GEARLM-0.1.0/GEARLM/TrueCompression/models/
--rw-r--r--   0 root         (0) root         (0)    15604 2024-03-22 00:04:17.000000 GEARLM-0.1.0/GEARLM/TrueCompression/models/TrueCompressFunction.py
--rw-r--r--   0 root         (0) root         (0)    70511 2024-03-22 00:04:17.000000 GEARLM-0.1.0/GEARLM/TrueCompression/models/TrueCompressLlama.py
--rw-r--r--   0 root         (0) root         (0)       55 2024-03-22 00:04:17.000000 GEARLM-0.1.0/GEARLM/TrueCompression/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16163 2024-03-22 00:04:17.000000 GEARLM-0.1.0/GEARLM/TrueCompression/models/cache_utils.py
--rw-r--r--   0 root         (0) root         (0)    10007 2024-03-22 00:04:17.000000 GEARLM-0.1.0/GEARLM/TrueCompression/models/compress_config.py
--rw-r--r--   0 root         (0) root         (0)    14351 2024-03-22 00:04:17.000000 GEARLM-0.1.0/GEARLM/TrueCompression/models/compressed_cache_utils.py
--rw-r--r--   0 root         (0) root         (0)     1957 2024-03-22 00:04:17.000000 GEARLM-0.1.0/GEARLM/TrueCompression/models/cpp_kernels.py
--rw-r--r--   0 root         (0) root         (0)    15855 2024-03-22 00:04:17.000000 GEARLM-0.1.0/GEARLM/TrueCompression/models/streaming_cache_utils.py
--rw-r--r--   0 root         (0) root         (0)     2863 2024-03-22 00:04:17.000000 GEARLM-0.1.0/GEARLM/TrueCompression/models/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 03:15:54.080109 GEARLM-0.1.0/GEARLM/TrueCompression/old_models/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 03:15:54.080109 GEARLM-0.1.0/GEARLM/TrueCompression/old_models/CompressUtils/
--rw-r--r--   0 root         (0) root         (0)    20044 2024-03-22 00:04:17.000000 GEARLM-0.1.0/GEARLM/TrueCompression/old_models/CompressUtils/TrueCompressFunction.py
--rw-r--r--   0 root         (0) root         (0)       42 2024-03-22 00:04:17.000000 GEARLM-0.1.0/GEARLM/TrueCompression/old_models/CompressUtils/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11868 2024-03-22 00:04:17.000000 GEARLM-0.1.0/GEARLM/TrueCompression/old_models/CompressUtils/compress_class.py
--rw-r--r--   0 root         (0) root         (0)       53 2024-03-22 00:04:17.000000 GEARLM-0.1.0/GEARLM/TrueCompression/old_models/__init__.py
--rw-r--r--   0 root         (0) root         (0)    63229 2024-03-22 00:04:17.000000 GEARLM-0.1.0/GEARLM/TrueCompression/old_models/modeling_llama_old.py
--rw-r--r--   0 root         (0) root         (0)      379 2024-03-22 00:04:17.000000 GEARLM-0.1.0/GEARLM/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 03:15:54.080109 GEARLM-0.1.0/GEARLM.egg-info/
--rw-r--r--   0 root         (0) root         (0)      421 2024-04-02 03:15:54.000000 GEARLM-0.1.0/GEARLM.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1267 2024-04-02 03:15:54.000000 GEARLM-0.1.0/GEARLM.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-02 03:15:54.000000 GEARLM-0.1.0/GEARLM.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-04-02 03:15:54.000000 GEARLM-0.1.0/GEARLM.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      421 2024-04-02 03:15:54.080109 GEARLM-0.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-02 03:15:54.080109 GEARLM-0.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      852 2024-04-02 03:15:52.000000 GEARLM-0.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 04:48:53.218375 GEARLM-0.1.1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 04:48:53.214375 GEARLM-0.1.1/GEARLM/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 04:48:53.218375 GEARLM-0.1.1/GEARLM/Simulated/
+-rw-r--r--   0 root         (0) root         (0)      310 2024-03-22 00:04:17.000000 GEARLM-0.1.1/GEARLM/Simulated/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16116 2024-03-22 00:04:17.000000 GEARLM-0.1.1/GEARLM/Simulated/cache_utils.py
+-rw-r--r--   0 root         (0) root         (0)    10002 2024-03-24 20:13:11.000000 GEARLM-0.1.1/GEARLM/Simulated/compress_config.py
+-rw-r--r--   0 root         (0) root         (0)    41026 2024-04-02 04:46:21.000000 GEARLM-0.1.1/GEARLM/Simulated/compress_function.py
+-rw-r--r--   0 root         (0) root         (0)     1957 2024-03-22 00:04:17.000000 GEARLM-0.1.1/GEARLM/Simulated/cpp_kernels.py
+-rw-r--r--   0 root         (0) root         (0)    65060 2024-03-22 00:04:17.000000 GEARLM-0.1.1/GEARLM/Simulated/h2o_llama_self_written.py
+-rw-r--r--   0 root         (0) root         (0)    74701 2024-03-26 04:08:05.000000 GEARLM-0.1.1/GEARLM/Simulated/modeling_llama_new.py
+-rw-r--r--   0 root         (0) root         (0)    65613 2024-03-22 00:04:17.000000 GEARLM-0.1.1/GEARLM/Simulated/modeling_mistral.py
+-rw-r--r--   0 root         (0) root         (0)    68919 2024-03-22 00:04:17.000000 GEARLM-0.1.1/GEARLM/Simulated/modeling_mixtral.py
+-rw-r--r--   0 root         (0) root         (0)     3047 2024-03-22 00:04:17.000000 GEARLM-0.1.1/GEARLM/Simulated/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 04:48:53.218375 GEARLM-0.1.1/GEARLM/TrueCompression/
+-rw-r--r--   0 root         (0) root         (0)       89 2024-03-22 00:04:17.000000 GEARLM-0.1.1/GEARLM/TrueCompression/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 04:48:53.218375 GEARLM-0.1.1/GEARLM/TrueCompression/models/
+-rw-r--r--   0 root         (0) root         (0)    15604 2024-03-22 00:04:17.000000 GEARLM-0.1.1/GEARLM/TrueCompression/models/TrueCompressFunction.py
+-rw-r--r--   0 root         (0) root         (0)    70511 2024-03-22 00:04:17.000000 GEARLM-0.1.1/GEARLM/TrueCompression/models/TrueCompressLlama.py
+-rw-r--r--   0 root         (0) root         (0)       55 2024-03-22 00:04:17.000000 GEARLM-0.1.1/GEARLM/TrueCompression/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16163 2024-03-22 00:04:17.000000 GEARLM-0.1.1/GEARLM/TrueCompression/models/cache_utils.py
+-rw-r--r--   0 root         (0) root         (0)    10007 2024-03-22 00:04:17.000000 GEARLM-0.1.1/GEARLM/TrueCompression/models/compress_config.py
+-rw-r--r--   0 root         (0) root         (0)    14351 2024-03-22 00:04:17.000000 GEARLM-0.1.1/GEARLM/TrueCompression/models/compressed_cache_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1957 2024-03-22 00:04:17.000000 GEARLM-0.1.1/GEARLM/TrueCompression/models/cpp_kernels.py
+-rw-r--r--   0 root         (0) root         (0)    15855 2024-03-22 00:04:17.000000 GEARLM-0.1.1/GEARLM/TrueCompression/models/streaming_cache_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2863 2024-03-22 00:04:17.000000 GEARLM-0.1.1/GEARLM/TrueCompression/models/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 04:48:53.218375 GEARLM-0.1.1/GEARLM/TrueCompression/old_models/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 04:48:53.218375 GEARLM-0.1.1/GEARLM/TrueCompression/old_models/CompressUtils/
+-rw-r--r--   0 root         (0) root         (0)    20044 2024-03-22 00:04:17.000000 GEARLM-0.1.1/GEARLM/TrueCompression/old_models/CompressUtils/TrueCompressFunction.py
+-rw-r--r--   0 root         (0) root         (0)       42 2024-03-22 00:04:17.000000 GEARLM-0.1.1/GEARLM/TrueCompression/old_models/CompressUtils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11868 2024-03-22 00:04:17.000000 GEARLM-0.1.1/GEARLM/TrueCompression/old_models/CompressUtils/compress_class.py
+-rw-r--r--   0 root         (0) root         (0)       53 2024-03-22 00:04:17.000000 GEARLM-0.1.1/GEARLM/TrueCompression/old_models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    63229 2024-03-22 00:04:17.000000 GEARLM-0.1.1/GEARLM/TrueCompression/old_models/modeling_llama_old.py
+-rw-r--r--   0 root         (0) root         (0)      379 2024-03-22 00:04:17.000000 GEARLM-0.1.1/GEARLM/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 04:48:53.214375 GEARLM-0.1.1/GEARLM.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      421 2024-04-02 04:48:53.000000 GEARLM-0.1.1/GEARLM.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1267 2024-04-02 04:48:53.000000 GEARLM-0.1.1/GEARLM.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-02 04:48:53.000000 GEARLM-0.1.1/GEARLM.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-04-02 04:48:53.000000 GEARLM-0.1.1/GEARLM.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      421 2024-04-02 04:48:53.218375 GEARLM-0.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-02 04:48:53.218375 GEARLM-0.1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      852 2024-04-02 03:18:35.000000 GEARLM-0.1.1/setup.py
```

### Comparing `GEARLM-0.1.0/GEARLM/Simulated/cache_utils.py` & `GEARLM-0.1.1/GEARLM/Simulated/cache_utils.py`

 * *Files identical despite different names*

### Comparing `GEARLM-0.1.0/GEARLM/Simulated/compress_config.py` & `GEARLM-0.1.1/GEARLM/Simulated/compress_config.py`

 * *Files identical despite different names*

### Comparing `GEARLM-0.1.0/GEARLM/Simulated/compress_function.py` & `GEARLM-0.1.1/GEARLM/Simulated/compress_function.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,29 +181,29 @@
     input = input.permute(0, 2, 1, 3).contiguous().type(dtype)
     return dequantized_input
 def fake_groupwise_channel_asymmetric_quantization_new(
     input: torch.Tensor, quantize_bit, group_size=128
 ):
     batch, num_head, seq_len, sep_dim = input.shape
     dtype = input.dtype
-    group_size = 128
+    # group_size = 128
     input = (
         input.permute(0, 2, 1, 3).contiguous().view(batch, seq_len, sep_dim * num_head)
     )
     input = input.view(batch * seq_len, num_head * sep_dim)
     group_num = input.shape[0] // group_size
     fixed_length = int(group_num * group_size)
     fixed_input = input[:fixed_length,:]
     residual_input = input[fixed_length:,:]
     fixed_input = fixed_input.view(group_num, group_size, num_head * sep_dim)
     mx, mn = fixed_input.max(dim=-2)[0], fixed_input.min(dim=-2)[0]
     mx, mn = mx.unsqueeze(-2), mn.unsqueeze(-2)
 
     scale = (mx - mn) / (2**quantize_bit - 1)
-    quantized_input = (input - mn) / scale
+    quantized_input = (fixed_input - mn) / scale
     quantized_input = F.relu(quantized_input)
     rounded_input = quantized_input.round_()
     dequantized_input = rounded_input * scale + mn
     dequantized_input = dequantized_input.view(group_num * group_size,num_head * sep_dim)
     concat_input = torch.cat((dequantized_input,residual_input),dim=0)
     dequantized_input = concat_input.view(batch, seq_len, num_head, sep_dim)
     dequantized_input = dequantized_input.permute(0, 2, 1, 3)
```

### Comparing `GEARLM-0.1.0/GEARLM/Simulated/cpp_kernels.py` & `GEARLM-0.1.1/GEARLM/Simulated/cpp_kernels.py`

 * *Files identical despite different names*

### Comparing `GEARLM-0.1.0/GEARLM/Simulated/h2o_llama_self_written.py` & `GEARLM-0.1.1/GEARLM/Simulated/h2o_llama_self_written.py`

 * *Files identical despite different names*

### Comparing `GEARLM-0.1.0/GEARLM/Simulated/modeling_llama_new.py` & `GEARLM-0.1.1/GEARLM/Simulated/modeling_llama_new.py`

 * *Files identical despite different names*

### Comparing `GEARLM-0.1.0/GEARLM/Simulated/modeling_mistral.py` & `GEARLM-0.1.1/GEARLM/Simulated/modeling_mistral.py`

 * *Files identical despite different names*

### Comparing `GEARLM-0.1.0/GEARLM/Simulated/modeling_mixtral.py` & `GEARLM-0.1.1/GEARLM/Simulated/modeling_mixtral.py`

 * *Files identical despite different names*

### Comparing `GEARLM-0.1.0/GEARLM/Simulated/utils.py` & `GEARLM-0.1.1/GEARLM/Simulated/utils.py`

 * *Files identical despite different names*

### Comparing `GEARLM-0.1.0/GEARLM/TrueCompression/models/TrueCompressFunction.py` & `GEARLM-0.1.1/GEARLM/TrueCompression/models/TrueCompressFunction.py`

 * *Files identical despite different names*

### Comparing `GEARLM-0.1.0/GEARLM/TrueCompression/models/TrueCompressLlama.py` & `GEARLM-0.1.1/GEARLM/TrueCompression/models/TrueCompressLlama.py`

 * *Files identical despite different names*

### Comparing `GEARLM-0.1.0/GEARLM/TrueCompression/models/cache_utils.py` & `GEARLM-0.1.1/GEARLM/TrueCompression/models/cache_utils.py`

 * *Files identical despite different names*

### Comparing `GEARLM-0.1.0/GEARLM/TrueCompression/models/compress_config.py` & `GEARLM-0.1.1/GEARLM/TrueCompression/models/compress_config.py`

 * *Files identical despite different names*

### Comparing `GEARLM-0.1.0/GEARLM/TrueCompression/models/compressed_cache_utils.py` & `GEARLM-0.1.1/GEARLM/TrueCompression/models/compressed_cache_utils.py`

 * *Files identical despite different names*

### Comparing `GEARLM-0.1.0/GEARLM/TrueCompression/models/cpp_kernels.py` & `GEARLM-0.1.1/GEARLM/TrueCompression/models/cpp_kernels.py`

 * *Files identical despite different names*

### Comparing `GEARLM-0.1.0/GEARLM/TrueCompression/models/streaming_cache_utils.py` & `GEARLM-0.1.1/GEARLM/TrueCompression/models/streaming_cache_utils.py`

 * *Files identical despite different names*

### Comparing `GEARLM-0.1.0/GEARLM/TrueCompression/models/utils.py` & `GEARLM-0.1.1/GEARLM/TrueCompression/models/utils.py`

 * *Files identical despite different names*

### Comparing `GEARLM-0.1.0/GEARLM/TrueCompression/old_models/CompressUtils/TrueCompressFunction.py` & `GEARLM-0.1.1/GEARLM/TrueCompression/old_models/CompressUtils/TrueCompressFunction.py`

 * *Files identical despite different names*

### Comparing `GEARLM-0.1.0/GEARLM/TrueCompression/old_models/CompressUtils/compress_class.py` & `GEARLM-0.1.1/GEARLM/TrueCompression/old_models/CompressUtils/compress_class.py`

 * *Files identical despite different names*

### Comparing `GEARLM-0.1.0/GEARLM/TrueCompression/old_models/modeling_llama_old.py` & `GEARLM-0.1.1/GEARLM/TrueCompression/old_models/modeling_llama_old.py`

 * *Files identical despite different names*

### Comparing `GEARLM-0.1.0/GEARLM.egg-info/SOURCES.txt` & `GEARLM-0.1.1/GEARLM.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `GEARLM-0.1.0/setup.py` & `GEARLM-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.1.0"
+VERSION = "0.1.1"
 DESCRIPTION = "GEARLM"
 LONG_DESCRIPTION = "GEAR: An Efficient KV Cache Compression Recipe for Near-Lossless Generative Inference of LLM"
 
 # Setting up
 setup(
     # the name must match the folder name 'verysimplemodule'
     name="GEARLM",
```

