# Comparing `tmp/gptfast-0.1.0.tar.gz` & `tmp/gptfast-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gptfast-0.1.0.tar", last modified: Mon Feb 19 02:41:22 2024, max compression
+gzip compressed data, was "gptfast-0.2.0.tar", last modified: Tue Apr  2 02:56:17 2024, max compression
```

## Comparing `gptfast-0.1.0.tar` & `gptfast-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,46 @@
-drwxrwxrwx   0        0        0        0 2024-02-19 02:41:22.302033 gptfast-0.1.0/
-drwxrwxrwx   0        0        0        0 2024-02-19 02:41:22.260034 gptfast-0.1.0/GPTFast/
-drwxrwxrwx   0        0        0        0 2024-02-19 02:41:22.271031 gptfast-0.1.0/GPTFast/Core/
--rw-rw-rw-   0        0        0      862 2024-02-17 21:40:40.000000 gptfast-0.1.0/GPTFast/Core/Compile.py
--rw-rw-rw-   0        0        0      796 2024-02-17 23:33:19.000000 gptfast-0.1.0/GPTFast/Core/GPTFast.py
--rw-rw-rw-   0        0        0     5132 2024-02-19 01:59:39.000000 gptfast-0.1.0/GPTFast/Core/KVCache.py
--rw-rw-rw-   0        0        0      213 2024-02-17 21:37:13.000000 gptfast-0.1.0/GPTFast/Core/Quantize.py
--rw-rw-rw-   0        0        0     8575 2024-02-19 01:49:47.000000 gptfast-0.1.0/GPTFast/Core/SpeculativeDecode.py
--rw-rw-rw-   0        0        0      129 2024-02-18 22:34:53.000000 gptfast-0.1.0/GPTFast/Core/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-19 02:41:22.274031 gptfast-0.1.0/GPTFast/Helpers/
--rw-rw-rw-   0        0        0       20 2024-02-18 22:44:55.000000 gptfast-0.1.0/GPTFast/Helpers/__init__.py
--rw-rw-rw-   0        0        0      266 2024-02-18 22:43:42.000000 gptfast-0.1.0/GPTFast/Helpers/timed.py
--rw-rw-rw-   0        0        0        0 2024-02-19 02:23:22.000000 gptfast-0.1.0/GPTFast/__init__.py
--rw-rw-rw-   0        0        0      245 2024-02-19 02:41:22.301035 gptfast-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-02-19 02:41:22.298031 gptfast-0.1.0/gptfast.egg-info/
--rw-rw-rw-   0        0        0      245 2024-02-19 02:41:22.000000 gptfast-0.1.0/gptfast.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      391 2024-02-19 02:41:22.000000 gptfast-0.1.0/gptfast.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-19 02:41:22.000000 gptfast-0.1.0/gptfast.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      376 2024-02-19 02:41:22.000000 gptfast-0.1.0/gptfast.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-02-19 02:41:22.000000 gptfast-0.1.0/gptfast.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-19 02:41:22.302033 gptfast-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      828 2024-02-19 02:41:14.000000 gptfast-0.1.0/setup.py
+drwxrwxrwx   0 kd2374    (1000) kd2374    (1000)        0 2024-04-02 02:56:17.974632 gptfast-0.2.0/
+drwxrwxrwx   0 kd2374    (1000) kd2374    (1000)        0 2024-04-02 02:56:17.327216 gptfast-0.2.0/GPTFast/
+drwxrwxrwx   0 kd2374    (1000) kd2374    (1000)        0 2024-04-02 02:56:17.359228 gptfast-0.2.0/GPTFast/Core/
+drwxrwxrwx   0 kd2374    (1000) kd2374    (1000)        0 2024-04-02 02:56:17.421224 gptfast-0.2.0/GPTFast/Core/Compile/
+-rwxrwxrwx   0 kd2374    (1000) kd2374    (1000)      883 2024-04-01 14:22:48.000000 gptfast-0.2.0/GPTFast/Core/Compile/Compile.py
+-rwxrwxrwx   0 kd2374    (1000) kd2374    (1000)       22 2024-04-02 02:41:49.000000 gptfast-0.2.0/GPTFast/Core/Compile/__init__.py
+drwxrwxrwx   0 kd2374    (1000) kd2374    (1000)        0 2024-04-02 02:56:17.464227 gptfast-0.2.0/GPTFast/Core/Decode/
+-rwxrwxrwx   0 kd2374    (1000) kd2374    (1000)     7805 2024-03-31 14:51:31.000000 gptfast-0.2.0/GPTFast/Core/Decode/SpeculativeDecode.py
+-rwxrwxrwx   0 kd2374    (1000) kd2374    (1000)       32 2024-04-02 02:42:10.000000 gptfast-0.2.0/GPTFast/Core/Decode/__init__.py
+-rwxrwxrwx   0 kd2374    (1000) kd2374    (1000)     1038 2024-04-02 02:43:28.000000 gptfast-0.2.0/GPTFast/Core/GPTFast.py
+drwxrwxrwx   0 kd2374    (1000) kd2374    (1000)        0 2024-04-02 02:56:17.530226 gptfast-0.2.0/GPTFast/Core/KVCache/
+-rwxrwxrwx   0 kd2374    (1000) kd2374    (1000)     4987 2024-04-01 01:20:31.000000 gptfast-0.2.0/GPTFast/Core/KVCache/KVCache.py
+-rwxrwxrwx   0 kd2374    (1000) kd2374    (1000)    13104 2024-04-01 12:59:16.000000 gptfast-0.2.0/GPTFast/Core/KVCache/KVCacheModel.py
+-rwxrwxrwx   0 kd2374    (1000) kd2374    (1000)       51 2024-03-29 01:07:55.000000 gptfast-0.2.0/GPTFast/Core/KVCache/__init__.py
+drwxrwxrwx   0 kd2374    (1000) kd2374    (1000)        0 2024-04-02 02:56:17.574226 gptfast-0.2.0/GPTFast/Core/Quantize/
+-rwxrwxrwx   0 kd2374    (1000) kd2374    (1000)       28 2024-04-02 02:42:58.000000 gptfast-0.2.0/GPTFast/Core/Quantize/__init__.py
+-rwxrwxrwx   0 kd2374    (1000) kd2374    (1000)      213 2024-03-30 04:17:43.000000 gptfast-0.2.0/GPTFast/Core/Quantize/quantize_int8.py
+-rwxrwxrwx   0 kd2374    (1000) kd2374    (1000)      171 2024-03-29 01:08:22.000000 gptfast-0.2.0/GPTFast/Core/__init__.py
+drwxrwxrwx   0 kd2374    (1000) kd2374    (1000)        0 2024-04-02 02:56:17.596228 gptfast-0.2.0/GPTFast/Helpers/
+drwxrwxrwx   0 kd2374    (1000) kd2374    (1000)        0 2024-04-02 02:56:17.663224 gptfast-0.2.0/GPTFast/Helpers/Class/
+-rwxrwxrwx   0 kd2374    (1000) kd2374    (1000)       61 2024-03-29 01:06:14.000000 gptfast-0.2.0/GPTFast/Helpers/Class/__init__.py
+-rwxrwxrwx   0 kd2374    (1000) kd2374    (1000)      556 2024-03-27 21:31:04.000000 gptfast-0.2.0/GPTFast/Helpers/Class/add_str_as_func.py
+-rwxrwxrwx   0 kd2374    (1000) kd2374    (1000)      415 2024-03-27 21:15:34.000000 gptfast-0.2.0/GPTFast/Helpers/Class/get_method_str.py
+drwxrwxrwx   0 kd2374    (1000) kd2374    (1000)        0 2024-04-02 02:56:17.709225 gptfast-0.2.0/GPTFast/Helpers/Eval/
+-rwxrwxrwx   0 kd2374    (1000) kd2374    (1000)       20 2024-04-02 00:49:29.000000 gptfast-0.2.0/GPTFast/Helpers/Eval/__init__.py
+-rwxrwxrwx   0 kd2374    (1000) kd2374    (1000)      266 2024-02-18 22:43:42.000000 gptfast-0.2.0/GPTFast/Helpers/Eval/timed.py
+drwxrwxrwx   0 kd2374    (1000) kd2374    (1000)        0 2024-04-02 02:56:17.864632 gptfast-0.2.0/GPTFast/Helpers/String/
+-rwxrwxrwx   0 kd2374    (1000) kd2374    (1000)      203 2024-04-01 12:49:59.000000 gptfast-0.2.0/GPTFast/Helpers/String/__init__.py
+-rwxrwxrwx   0 kd2374    (1000) kd2374    (1000)     1207 2024-03-27 21:28:02.000000 gptfast-0.2.0/GPTFast/Helpers/String/add_default_parameter.py
+-rwxrwxrwx   0 kd2374    (1000) kd2374    (1000)     1044 2024-03-29 01:07:19.000000 gptfast-0.2.0/GPTFast/Helpers/String/add_input_pos_to_func_str.py
+-rwxrwxrwx   0 kd2374    (1000) kd2374    (1000)     1213 2024-04-01 12:49:33.000000 gptfast-0.2.0/GPTFast/Helpers/String/modify_function_block.py
+-rwxrwxrwx   0 kd2374    (1000) kd2374    (1000)     1669 2024-03-29 01:07:23.000000 gptfast-0.2.0/GPTFast/Helpers/String/modify_if_block.py
+-rwxrwxrwx   0 kd2374    (1000) kd2374    (1000)      369 2024-03-27 21:18:23.000000 gptfast-0.2.0/GPTFast/Helpers/String/shift_left.py
+-rwxrwxrwx   0 kd2374    (1000) kd2374    (1000)      377 2024-03-27 21:18:26.000000 gptfast-0.2.0/GPTFast/Helpers/String/shift_right.py
+-rwxrwxrwx   0 kd2374    (1000) kd2374    (1000)       64 2024-04-01 14:38:02.000000 gptfast-0.2.0/GPTFast/Helpers/__init__.py
+-rwxrwxrwx   0 kd2374    (1000) kd2374    (1000)        0 2024-03-27 21:33:11.000000 gptfast-0.2.0/GPTFast/__init__.py
+-rwxrwxrwx   0 kd2374    (1000) kd2374    (1000)      889 2024-04-02 02:56:17.967635 gptfast-0.2.0/PKG-INFO
+-rwxrwxrwx   0 kd2374    (1000) kd2374    (1000)     5351 2024-02-24 16:42:44.000000 gptfast-0.2.0/README.md
+drwxrwxrwx   0 kd2374    (1000) kd2374    (1000)        0 2024-04-02 02:56:17.959632 gptfast-0.2.0/gptfast.egg-info/
+-rwxrwxrwx   0 kd2374    (1000) kd2374    (1000)      889 2024-04-02 02:56:16.000000 gptfast-0.2.0/gptfast.egg-info/PKG-INFO
+-rwxrwxrwx   0 kd2374    (1000) kd2374    (1000)     1060 2024-04-02 02:56:17.000000 gptfast-0.2.0/gptfast.egg-info/SOURCES.txt
+-rwxrwxrwx   0 kd2374    (1000) kd2374    (1000)        1 2024-04-02 02:56:16.000000 gptfast-0.2.0/gptfast.egg-info/dependency_links.txt
+-rwxrwxrwx   0 kd2374    (1000) kd2374    (1000)      376 2024-04-02 02:56:16.000000 gptfast-0.2.0/gptfast.egg-info/requires.txt
+-rwxrwxrwx   0 kd2374    (1000) kd2374    (1000)        8 2024-04-02 02:56:16.000000 gptfast-0.2.0/gptfast.egg-info/top_level.txt
+-rwxrwxrwx   0 kd2374    (1000) kd2374    (1000)       38 2024-04-02 02:56:17.974632 gptfast-0.2.0/setup.cfg
+-rwxrwxrwx   0 kd2374    (1000) kd2374    (1000)      824 2024-04-02 02:56:04.000000 gptfast-0.2.0/setup.py
```

### Comparing `gptfast-0.1.0/GPTFast/Core/SpeculativeDecode.py` & `gptfast-0.2.0/GPTFast/Core/Decode/SpeculativeDecode.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 #In order for speculative decoding to work, the vocabulary for two models must be the same, i.e. the dictionary with id keys and string tokens must be the same.
 import types
 import torch
 import torch.nn as nn
-from typing import Callable
-from .KVCache import KVCacheModel
+from ..KVCache.KVCacheModel import KVCacheModel
 
 #ok, here's the key behind speculative decoding. We have two models, Mq the small model and Mp the large model. 
 #1. Run Mq on prefix and obtain the distribution for x1 q(x).
 #2. Run Mp on prefix and prefix + x1 concurrently to get the distributions for x2 and p(x).
 #3. If x1 is rejected by Mp, reject and resample x1 from an altered distribution, otherwise keep x1 and x2. 
 
 def speculative_decode_eager(
@@ -60,41 +59,37 @@
         return torch.cat([draft_tokens[:, :n], last_token.unsqueeze(0)], dim=-1).long()
     else: #we accept all tokens from the draft model
         last_token = torch.Tensor([self.sample(model_prob[-1])]).to(device)
         return torch.cat([draft_tokens, last_token.unsqueeze(0)], dim=-1).long()
 
 def speculative_decode_kv_cache(
     self,
-    cur_tokens:torch.Tensor,
+    uncached_tokens:torch.Tensor,
     speculate_k:int,
     **sampling_kwargs
 ) -> torch.Tensor:
 
     assert isinstance(self, KVCacheModel), "Your model must be a KVCache model in order to call speculative_decode_kv_cache."
 
-    device = cur_tokens.device
+    device = uncached_tokens.device
 
     assert hasattr(self, "draft_model"), "You did not prepare your model properly for speculative decoding. Make sure that you add a draft model."
     draft_model = self.draft_model
     
     assert isinstance(draft_model, KVCacheModel), "Your draft model muut be a KVCache model in order to call speculative_decode_kv_cache."
 
-    draft_tokens, draft_prob = draft_model.decode_function(input_ids=cur_tokens, length=speculate_k, return_text=True)
+    draft_tokens, draft_prob = draft_model.decode_function(uncached_input_ids=uncached_tokens, length=speculate_k, return_text=True)
 
     assert len(draft_tokens.shape) == 2 and len(draft_prob.shape) == 2, "Your draft tokens must have shape (1, seq_len) and draft_prob must have shape (seq_len, vocab_size)."
 
-    full_tokens = torch.cat([cur_tokens, draft_tokens], dim=-1).to(device)
+    full_tokens = torch.cat([uncached_tokens, draft_tokens], dim=-1).to(device)
     with torch.no_grad():
         self.forward(full_tokens)
     model_logits = self._prob_history[:, -speculate_k-1:, :].squeeze(0)
     model_prob = torch.nn.functional.softmax(model_logits, dim=-1)
-    
-    assert len(model_prob.shape) == 2, f"Your model_prob must have shape (seq_len, vocab_size), current model_prob shape:"
-
-    assert len(model_prob) == len(draft_prob) + 1, "In order for speculative decoding to work, the main model must generate one more token than the draft model."
 
     p = model_prob[torch.arange(0, speculate_k, device=device), draft_tokens]
     q = draft_prob[torch.arange(0, speculate_k, device=device), draft_tokens]
 
     ratio = p / q
     rand = torch.rand_like(ratio)
 
@@ -102,30 +97,25 @@
 
     if reject_locations.shape[0] != 0:
         n = reject_locations[0].item()
         p = draft_prob[n]
         q = model_prob[n]
         new = q - p
         new = torch.where(new > 0, new, 0.0)
-        last_token = torch.Tensor([self.sample(new, **sampling_kwargs)]).to(device)
-        assert hasattr(self, "rollback_cache"), "Error: In order for speculative decoding to work with a kv cache, you must be able to update it."
-        self.rollback_cache(n + len(cur_tokens))
-        assert hasattr(draft_model, "rollback_cache"), "Error: In order for speculative decoding to work with a kv cache, you must be able to update it."
-        draft_model.rollback_cache(n + len(cur_tokens))
-        
-        return torch.cat([draft_tokens[:, :n], last_token.unsqueeze(0)], dim=-1).long()
+        last_token = self.sample(new, **sampling_kwargs).to(device)
+        self.rollback_cache(self._cached_len - (full_tokens.shape[-1] - n) + 1)
+        draft_model.rollback_cache(draft_model._cached_len - (draft_tokens.shape[-1] - n) + 1)
+        return torch.cat([draft_tokens[:, :n], last_token], dim=-1).long() #maybe? This is what my gut says.
     else: #we accept all tokens from the draft model
-        last_token = torch.Tensor([self.sample(model_prob[-1], **sampling_kwargs)]).to(device)
-        assert hasattr(self, "rollback_cache"), "Error: In order for speculative decoding to work with a kv cache, you must be able to update it."
+        last_token = self.sample(model_prob[-1], **sampling_kwargs).to(device)
         #self.rollback_cache(n + len(cur_tokens) + 1)
-        assert hasattr(draft_model, "rollback_cache"), "Error: In order for speculative decoding to work with a kv cache, you must be able to update it."
-        draft_model.rollback_cache(speculate_k + len(cur_tokens)) #This is a little bit suspect, might have to change this - why are we rejecting the last token when it works?
-
+        draft_model(input_ids=draft_tokens[:, -1].view(1, 1))
+        #draft_model.rollback_cache(draft_model._cached_len + 1) #This is a little bit suspect, might have to change this - why are we rejecting the last token when it works?
         #assume that draft_model already has a kv cache attached.
-        return torch.cat([draft_tokens, last_token.unsqueeze(0)], dim=-1).long()
+        return torch.cat([draft_tokens, last_token], dim=-1).long() #intuitively, this makes sense.
 
 def generate(self, cur_tokens:torch.Tensor, max_tokens:int, speculate_k:int, **sampling_kwargs) -> torch.Tensor:
 
     assert len(cur_tokens.shape) == 2 and cur_tokens.shape[0] == 1, "Your batch size must be 1"
 
     assert hasattr(self, "speculative_decode"), "You must attach speculative decoding as a method of the model"
 
@@ -133,41 +123,40 @@
         new_tokens = self.speculative_decode(cur_tokens, speculate_k, **sampling_kwargs)
         cur_tokens = torch.cat((cur_tokens, new_tokens), dim=1).to(torch.long)
 
     return cur_tokens
 
 def generate_kv_cache(self, cur_tokens:torch.Tensor, max_tokens:int, speculate_k:int, **sampling_kwargs) -> torch.Tensor:
     assert isinstance(self, KVCacheModel), "Your model must be a KVCache model for this to work."
-    assert isinstance(self.draft_model, KVCacheModel), "Your draft model must be a KVCache model for this to work."
-    
+    assert hasattr(self, "draft_model") and isinstance(self.draft_model, KVCacheModel), "You must have a draft model and it must be a KVCacheModel for the generate() method."
     assert len(cur_tokens.shape) == 2 and cur_tokens.shape[0] == 1, "Your batch size must be 1"
-
     assert hasattr(self, "speculative_decode"), "You must attach speculative decoding as a method of the model"
 
     device = cur_tokens.device
 
     #prefill phase
     self.draft_model.prefill(cur_tokens)
-    next_q = self.prefill(cur_tokens)
+    new_q = self.prefill(cur_tokens)
+
+    new_token = self.sample(new_q, **sampling_kwargs).to(device)
 
-    next_token = torch.Tensor([self.sample(next_q[-1], **sampling_kwargs)]).to(device) 
-    cur_tokens = torch.cat((cur_tokens, next_token.unsqueeze(0)), dim=-1).to(torch.long)
+    cur_tokens = torch.cat((cur_tokens, new_token), dim=-1).to(torch.long)
 
     while len(cur_tokens[0]) < max_tokens:
-        new_tokens = self.speculative_decode(cur_tokens, speculate_k, **sampling_kwargs)
+        uncached_tokens = cur_tokens[:, -1].view(1, 1)
+        new_tokens = self.speculative_decode(uncached_tokens, speculate_k, **sampling_kwargs)
         cur_tokens = torch.cat((cur_tokens, new_tokens), dim=-1).to(torch.long)
 
     self.clear()
     self.draft_model.clear()
 
     return cur_tokens    
 
-def add_speculative_decoding(model:nn.Module, draft_model:nn.Module, sample_function:Callable) -> nn.Module:
+def add_speculative_decoding(model:nn.Module, draft_model:nn.Module) -> nn.Module:
     model.draft_model = draft_model
-    model.sample = types.MethodType(sample_function, model)
 
     model.speculative_decode = types.MethodType(speculative_decode_kv_cache, model)
     model.generate = types.MethodType(generate_kv_cache, model)
     return model
```

### Comparing `gptfast-0.1.0/setup.py` & `gptfast-0.2.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gptfast',
-    version='0.1.0',
+    version='0.2.0',
     author="MDK8888",
-    description="Accelerate your transformer models by up to 6x. Native to Huggingface and PyTorch.",
+    description="Accelerate transformer inference by 6-8.5x. Native to Huggingface and PyTorch.",
     packages=find_packages(),
-    install_requires=['torch==2.1.2', 'sympy==1.12', 'typing-extensions==4.9.0', 'networkx==3.2.1', 'jinja2==3.1.3', 'triton==2.1.0', 'fsspec==2023.10.0', 'filelock==3.13.1', 'MarkupSafe==2.1.4', 'mpmath==1.3.0', 'transformers==4.37.2', 'tqdm==4.66.1', 'pyyaml==5.3.1', 'safetensors==0.4.1', 'numpy==1.26.3', 'huggingface-hub==0.20.2', 'tokenizers==0.15.0', 'packaging==23.2', 'regex==2023.12.25', 'requests==2.31.0', 'bitsandbytes==0.42.0', 'accelerate==0.26.1'],
+    install_requires=['torch==2.2.1', 'sympy==1.12', 'typing-extensions==4.9.0', 'networkx==3.2.1', 'jinja2==3.1.3', 'triton==2.2.0', 'fsspec==2023.10.0', 'filelock==3.13.1', 'MarkupSafe==2.1.4', 'mpmath==1.3.0', 'transformers==4.39.2', 'tqdm==4.66.1', 'pyyaml==5.3.1', 'safetensors==0.4.1', 'numpy==1.26.3', 'huggingface-hub==0.20.2', 'tokenizers==0.15.0', 'packaging==23.2', 'regex==2023.12.25', 'requests==2.31.0', 'bitsandbytes==0.43.0', 'accelerate==0.27.2'],
     license="Apache License 2.0",
     package_data={
         '':["LICENSE", "requirements.txt"]
     }
 )
```

