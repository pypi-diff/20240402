# Comparing `tmp/bitmat-tl-0.1.6.tar.gz` & `tmp/bitmat-tl-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitmat-tl-0.1.6.tar", last modified: Mon Apr  1 18:07:35 2024, max compression
+gzip compressed data, was "bitmat-tl-0.1.7.tar", last modified: Mon Apr  1 21:47:19 2024, max compression
```

## Comparing `bitmat-tl-0.1.6.tar` & `bitmat-tl-0.1.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-01 18:07:35.015289 bitmat-tl-0.1.6/
--rw-rw-r--   0 marco     (1000) marco     (1000)    11357 2024-03-31 16:42:10.000000 bitmat-tl-0.1.6/LICENSE
--rw-r--r--   0 marco     (1000) marco     (1000)      710 2024-04-01 18:07:35.015289 bitmat-tl-0.1.6/PKG-INFO
--rw-rw-r--   0 marco     (1000) marco     (1000)       98 2024-03-26 17:02:00.000000 bitmat-tl-0.1.6/README.md
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-01 18:07:35.011289 bitmat-tl-0.1.6/bitmat/
--rw-rw-r--   0 marco     (1000) marco     (1000)        0 2024-03-30 14:45:20.000000 bitmat-tl-0.1.6/bitmat/__init__.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     1077 2024-04-01 18:07:20.000000 bitmat-tl-0.1.6/bitmat/bitlinear.py
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-01 18:07:35.011289 bitmat-tl-0.1.6/bitmat/triton_kernels/
--rw-rw-r--   0 marco     (1000) marco     (1000)        0 2024-03-31 10:45:17.000000 bitmat-tl-0.1.6/bitmat/triton_kernels/__init__.py
--rw-rw-r--   0 marco     (1000) marco     (1000)    12721 2024-03-31 16:41:21.000000 bitmat-tl-0.1.6/bitmat/triton_kernels/bitmat_kernel.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     5241 2024-03-26 17:02:00.000000 bitmat-tl-0.1.6/bitmat/triton_kernels/rmsnorm_kernel.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     7037 2024-03-26 17:02:00.000000 bitmat-tl-0.1.6/bitmat/triton_kernels/utils.py
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-01 18:07:35.011289 bitmat-tl-0.1.6/bitmat/utils/
--rw-rw-r--   0 marco     (1000) marco     (1000)        0 2024-03-26 17:02:00.000000 bitmat-tl-0.1.6/bitmat/utils/__init__.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     2463 2024-03-31 18:04:18.000000 bitmat-tl-0.1.6/bitmat/utils/bitmat.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     1750 2024-03-31 19:24:56.000000 bitmat-tl-0.1.6/bitmat/utils/convert_hf_model.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     2161 2024-03-31 10:09:31.000000 bitmat-tl-0.1.6/bitmat/utils/packing.py
--rw-rw-r--   0 marco     (1000) marco     (1000)      379 2024-03-31 17:11:38.000000 bitmat-tl-0.1.6/bitmat/utils/rmsnorm.py
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-01 18:07:35.011289 bitmat-tl-0.1.6/bitmat_tl.egg-info/
--rw-r--r--   0 marco     (1000) marco     (1000)      710 2024-04-01 18:07:34.000000 bitmat-tl-0.1.6/bitmat_tl.egg-info/PKG-INFO
--rw-rw-r--   0 marco     (1000) marco     (1000)      502 2024-04-01 18:07:34.000000 bitmat-tl-0.1.6/bitmat_tl.egg-info/SOURCES.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)        1 2024-04-01 18:07:34.000000 bitmat-tl-0.1.6/bitmat_tl.egg-info/dependency_links.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)       45 2024-04-01 18:07:34.000000 bitmat-tl-0.1.6/bitmat_tl.egg-info/requires.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)        7 2024-04-01 18:07:34.000000 bitmat-tl-0.1.6/bitmat_tl.egg-info/top_level.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)       38 2024-04-01 18:07:35.015289 bitmat-tl-0.1.6/setup.cfg
--rw-rw-r--   0 marco     (1000) marco     (1000)      780 2024-04-01 18:06:22.000000 bitmat-tl-0.1.6/setup.py
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-01 21:47:19.571923 bitmat-tl-0.1.7/
+-rw-rw-r--   0 marco     (1000) marco     (1000)    11357 2024-03-31 16:42:10.000000 bitmat-tl-0.1.7/LICENSE
+-rw-r--r--   0 marco     (1000) marco     (1000)     3339 2024-04-01 21:47:19.571923 bitmat-tl-0.1.7/PKG-INFO
+-rw-rw-r--   0 marco     (1000) marco     (1000)     2727 2024-04-01 21:47:17.000000 bitmat-tl-0.1.7/README.md
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-01 21:47:19.571923 bitmat-tl-0.1.7/bitmat/
+-rw-rw-r--   0 marco     (1000) marco     (1000)       83 2024-04-01 21:43:18.000000 bitmat-tl-0.1.7/bitmat/__init__.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)     1061 2024-04-01 19:33:07.000000 bitmat-tl-0.1.7/bitmat/bitlinear.py
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-01 21:47:19.571923 bitmat-tl-0.1.7/bitmat/triton_kernels/
+-rw-rw-r--   0 marco     (1000) marco     (1000)        0 2024-03-31 10:45:17.000000 bitmat-tl-0.1.7/bitmat/triton_kernels/__init__.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)    12750 2024-04-01 19:35:36.000000 bitmat-tl-0.1.7/bitmat/triton_kernels/bitmat_kernel.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)     5241 2024-03-26 17:02:00.000000 bitmat-tl-0.1.7/bitmat/triton_kernels/rmsnorm_kernel.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)     7037 2024-03-26 17:02:00.000000 bitmat-tl-0.1.7/bitmat/triton_kernels/utils.py
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-01 21:47:19.571923 bitmat-tl-0.1.7/bitmat/utils/
+-rw-rw-r--   0 marco     (1000) marco     (1000)        0 2024-03-26 17:02:00.000000 bitmat-tl-0.1.7/bitmat/utils/__init__.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)     2413 2024-04-01 21:28:16.000000 bitmat-tl-0.1.7/bitmat/utils/bitmat.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)     2987 2024-04-01 21:28:16.000000 bitmat-tl-0.1.7/bitmat/utils/convert_hf_model.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)     2161 2024-03-31 10:09:31.000000 bitmat-tl-0.1.7/bitmat/utils/packing.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)      379 2024-03-31 17:11:38.000000 bitmat-tl-0.1.7/bitmat/utils/rmsnorm.py
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-01 21:47:19.571923 bitmat-tl-0.1.7/bitmat_tl.egg-info/
+-rw-r--r--   0 marco     (1000) marco     (1000)     3339 2024-04-01 21:47:19.000000 bitmat-tl-0.1.7/bitmat_tl.egg-info/PKG-INFO
+-rw-rw-r--   0 marco     (1000) marco     (1000)      502 2024-04-01 21:47:19.000000 bitmat-tl-0.1.7/bitmat_tl.egg-info/SOURCES.txt
+-rw-rw-r--   0 marco     (1000) marco     (1000)        1 2024-04-01 21:47:19.000000 bitmat-tl-0.1.7/bitmat_tl.egg-info/dependency_links.txt
+-rw-rw-r--   0 marco     (1000) marco     (1000)       45 2024-04-01 21:47:19.000000 bitmat-tl-0.1.7/bitmat_tl.egg-info/requires.txt
+-rw-rw-r--   0 marco     (1000) marco     (1000)        7 2024-04-01 21:47:19.000000 bitmat-tl-0.1.7/bitmat_tl.egg-info/top_level.txt
+-rw-rw-r--   0 marco     (1000) marco     (1000)       38 2024-04-01 21:47:19.571923 bitmat-tl-0.1.7/setup.cfg
+-rw-rw-r--   0 marco     (1000) marco     (1000)      780 2024-04-01 21:30:16.000000 bitmat-tl-0.1.7/setup.py
```

### Comparing `bitmat-tl-0.1.6/LICENSE` & `bitmat-tl-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.1.6/bitmat/bitlinear.py` & `bitmat-tl-0.1.7/bitmat/bitlinear.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,10 +23,10 @@
             torch.nn.init.constant_(self.bias, 0)
 
     def forward(self, x):
         x = self.norm(x)
         output = bitmat(self.weight, x)
         if self.bias is not None:
             output += self.bias.unsqueeze(0).expand_as(output)
-        return bitmat(self.weight, x)
+        return output
```

### Comparing `bitmat-tl-0.1.6/bitmat/triton_kernels/bitmat_kernel.py` & `bitmat-tl-0.1.7/bitmat/triton_kernels/bitmat_kernel.py`

 * *Files 1% similar despite different names*

```diff
@@ -291,10 +291,11 @@
             a.stride(0), b.stride(0), c.stride(0),
             ACTIVATION=activation
         )
         try:
             c[0][0][0].item()
         except RuntimeError:
             raise RuntimeError("Illegal memory access, it means that the kernel failed most probably to OOM, try to reduce batch size or matrix size.")
+    torch.cuda.empty_cache()
     return c
```

### Comparing `bitmat-tl-0.1.6/bitmat/triton_kernels/rmsnorm_kernel.py` & `bitmat-tl-0.1.7/bitmat/triton_kernels/rmsnorm_kernel.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.1.6/bitmat/triton_kernels/utils.py` & `bitmat-tl-0.1.7/bitmat/triton_kernels/utils.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.1.6/bitmat/utils/bitmat.py` & `bitmat-tl-0.1.7/bitmat/utils/bitmat.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,16 @@
     Quantizes the activations and returns the scale for each row.
     """
     scale = (127 / torch.max(x.abs().max(dim=-1).values, torch.tensor(1e-5))).unsqueeze(-1)
     return torch.clamp((x * scale), -127, 128).to(torch.int8), scale
 
 
 class BitMat(torch.autograd.Function):
+    @staticmethod
+    @torch.cuda.amp.custom_fwd
     def forward(ctx, W, X, scale_w=None):
         """
         During the forward pass, we ternarize the weights, pack them and then quantize the activations.
         We then perform the bit matrix multiplication and return the scaled results.
         ternarization:
         scale_w = 1 / mean(abs(W))                              | STE
         W = clip(round(W * scale_w), -1, 1)                     | STE
@@ -34,30 +36,30 @@
         quantization:
         scale_x = 127 / max(abs(X))                             | STE
         X = clip(round(X * scale_x), -127, 128)                 | STE
         bit matrix multiplication:
         Y = X @ w_packed.t()                                    | dot product
         Y = Y / (scale_w * scale_x)                             | STE
         """
-        if W.training:
+        if scale_w is None:
             W, scale_w = terniarize(W)
             packed_w = pack_ternary(W, 4)
+            ctx.save_for_backward(X)
             X, scale_x = quantize_activations(X)
-            ctx.save_for_backward(X, scale_x)
             y = batched_bitmat(X, packed_w)
             return y / scale_w / scale_x
         else:
-            assert scale_w is not None, "scale_w must be provided during inference"
             X, scale_x = quantize_activations(X)
             y = batched_bitmat(X, W)
             return y / scale_w / scale_x
 
 
     @staticmethod
+    @torch.cuda.amp.custom_bwd
     def backward(ctx, grad_output):
-        X, scale_x = ctx.saved_tensors
+        X = ctx.saved_tensors[0]
         # get dW
-        grad_W = grad_output @ (X / scale_x).t().to(torch.float16) # TODO: check dim
+        grad_W = X.transpose(1, 2) @ grad_output
         return grad_W, None, None
 
 def bitmat(W: torch.Tensor, X: torch.Tensor) -> torch.Tensor:
     return BitMat.apply(W, X)
```

### Comparing `bitmat-tl-0.1.6/bitmat/utils/packing.py` & `bitmat-tl-0.1.7/bitmat/utils/packing.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.1.6/setup.py` & `bitmat-tl-0.1.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='bitmat-tl',
-    version='0.1.6',
+    version='0.1.7',
     author='Marco Lironi',
     author_email='marcolironi@astramind.ai',
     description='An efficent implementation for the paper: "The Era of 1-bit LLMs"',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/astramind-ai/BitMat/tree/main',
     packages=find_packages(),
```

