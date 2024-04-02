# Comparing `tmp/llm-quantkit-0.22.tar.gz` & `tmp/llm-quantkit-0.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm-quantkit-0.22.tar", last modified: Thu Mar 21 23:19:42 2024, max compression
+gzip compressed data, was "llm-quantkit-0.23.tar", last modified: Tue Apr  2 20:50:34 2024, max compression
```

## Comparing `llm-quantkit-0.22.tar` & `llm-quantkit-0.23.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:19:42.785959 llm-quantkit-0.22/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-03-21 23:19:32.000000 llm-quantkit-0.22/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-03-21 23:19:42.785959 llm-quantkit-0.22/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-03-21 23:19:32.000000 llm-quantkit-0.22/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:19:42.785959 llm-quantkit-0.22/llm_quantkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-03-21 23:19:42.000000 llm-quantkit-0.22/llm_quantkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-03-21 23:19:42.000000 llm-quantkit-0.22/llm_quantkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 23:19:42.000000 llm-quantkit-0.22/llm_quantkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-21 23:19:42.000000 llm-quantkit-0.22/llm_quantkit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-03-21 23:19:42.000000 llm-quantkit-0.22/llm_quantkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-21 23:19:42.000000 llm-quantkit-0.22/llm_quantkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-03-21 23:19:32.000000 llm-quantkit-0.22/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 23:19:42.785959 llm-quantkit-0.22/quantkit/
--rw-r--r--   0 runner    (1001) docker     (127)     7592 2024-03-21 23:19:32.000000 llm-quantkit-0.22/quantkit/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    61155 2024-03-21 23:19:32.000000 llm-quantkit-0.22/quantkit/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)    15932 2024-03-21 23:19:32.000000 llm-quantkit-0.22/quantkit/quantkit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-03-21 23:19:32.000000 llm-quantkit-0.22/quantkit/safetensor.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-21 23:19:42.785959 llm-quantkit-0.22/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:50:34.992478 llm-quantkit-0.23/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-02 20:50:24.000000 llm-quantkit-0.23/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4865 2024-04-02 20:50:34.992478 llm-quantkit-0.23/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-04-02 20:50:24.000000 llm-quantkit-0.23/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:50:34.992478 llm-quantkit-0.23/llm_quantkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4865 2024-04-02 20:50:34.000000 llm-quantkit-0.23/llm_quantkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-02 20:50:34.000000 llm-quantkit-0.23/llm_quantkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 20:50:34.000000 llm-quantkit-0.23/llm_quantkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-02 20:50:34.000000 llm-quantkit-0.23/llm_quantkit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-02 20:50:34.000000 llm-quantkit-0.23/llm_quantkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-02 20:50:34.000000 llm-quantkit-0.23/llm_quantkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-02 20:50:24.000000 llm-quantkit-0.23/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:50:34.992478 llm-quantkit-0.23/quantkit/
+-rw-r--r--   0 runner    (1001) docker     (127)     7592 2024-04-02 20:50:24.000000 llm-quantkit-0.23/quantkit/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61155 2024-04-02 20:50:24.000000 llm-quantkit-0.23/quantkit/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15932 2024-04-02 20:50:24.000000 llm-quantkit-0.23/quantkit/quantkit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-04-02 20:50:24.000000 llm-quantkit-0.23/quantkit/safetensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 20:50:34.992478 llm-quantkit-0.23/setup.cfg
```

### Comparing `llm-quantkit-0.22/LICENSE` & `llm-quantkit-0.23/LICENSE`

 * *Files identical despite different names*

### Comparing `llm-quantkit-0.22/PKG-INFO` & `llm-quantkit-0.23/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,48 +1,34 @@
-Metadata-Version: 2.1
-Name: llm-quantkit
-Version: 0.22
-Summary: cli tool for downloading and quantizing LLMs
-Author-email: xhedit <jevd@protonmail.com>
-License: MIT License
-Project-URL: repository, https://github.com/xhedit/quantkit
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: click
-Requires-Dist: torch>=2.0.0
-Requires-Dist: einops
-Requires-Dist: tqdm
-Requires-Dist: transformers
-Requires-Dist: huggingface_hub
-Requires-Dist: safetensors
-Requires-Dist: auto-gptq
-Requires-Dist: autoawq
-Requires-Dist: exl2conv
-Requires-Dist: llama-cpp-conv
-Requires-Dist: sentencepiece
-Requires-Dist: hqq
-Provides-Extra: dev
-
 # quantkit
 
 A tool for downloading and converting HuggingFace models without drama.
 
 <br/>
 
 # Install
+If you're on a machine with an NVIDIA/CUDA GPU and want AWQ/GPTQ support:
+```
+pip3 install llm-quantkit[cuda]
+```
+<br/>
+
+Otherwise, the default install works. <br/>
+
 ```
 pip3 install llm-quantkit
 ```
 <br/>
 
 # Requirements
-This project depends on torch, awq, exl2, gptq, and hqq libraries, some of which are not compatible with Python 3.12. <br/>
+
 If you need a device specific torch, install it first. <br/>
-Python: 3.8, 3.9, 3.10, and 3.11
 
+This project depends on torch, awq, exl2, gptq, and hqq libraries. <br/>
+Some of these dependencies do not support Python 3.12 yet. <br/>
+Supported Pythons: 3.8, 3.9, 3.10, and 3.11<br/>
 
 
 # Usage
 
 ```
 Usage: quantkit [OPTIONS] COMMAND [ARGS]...
 
@@ -63,15 +49,18 @@
 
 The download command defaults to downloading into the HF cache and producing symlinks in the output dir, but there is a --no-cache option which places the model files in the output directory. <br/>
 
 
 AWQ defaults to 4 bits, group size 128, zero-point True. <br />
 GPTQ defaults are 4 bits, group size 128, activation-order False. <br />
 EXL2 defaults to 8 head bits but there is no default bitrate. <br />
-GGUF defaults to no imatrix but there is no default quant-type. <br/>
+GGUF defaults to no imatrix but there is no default quant-type. <br />
+HQQ defaults to 4 bits, group size 64, zero_point=True. <br />
+
+<br/>
 
 # Examples
 
 Download a model from HF and don't use HF cache:
 ```
 quantkit download teknium/Hermes-Trismegistus-Mistral-7B --no-cache
 ```
@@ -136,8 +125,39 @@
 
 Convert a model to HQQ:
 ```
 quantkit hqq mistralai/Mistral-7B-v0.1 -out Mistral-7B-HQQ-w4-gs64
 ```
 <br/>
 
+# Hardware Requirements
+Here's what has worked for me in testing. Drop a PR or Issue with updates for what is possible on various size cards. <br />
+GGUF conversion doesn't need a GPU except for iMatrix and Exllamav2 requires that the largest layer fits on single GPU.
+
+|Model Size|Quant|VRAM|Successful|
+|--|--|--|--|
+|7B|AWQ|24GB|✅|
+|7B|EXL2|24GB|✅|
+|7B|GGUF|24GB|✅|
+|7B|GPTQ|24GB|✅|
+|7B|HQQ|24GB|✅|
+|13B|AWQ|24GB|✅|
+|13B|EXL2|24GB|✅|
+|13B|GGUF|24GB|✅|
+|13B|GPTQ|24GB|:x:|
+|13B|HQQ|24GB|?|
+|34B|AWQ|24GB|:x:|
+|34B|EXL2|24GB|✅|
+|34B|GGUF|24GB|✅|
+|34B|GPTQ|24GB|:x:|
+|34B|HQQ|24GB|?|
+|70B|AWQ|24GB|:x:|
+|70B|EXL2|24GB|✅|
+|70B|GGUF|24GB|✅|
+|70B|GPTQ|24GB|:x:|
+|70B|HQQ|24GB|?|
+
+<br />
+
+# Notes
+
 Still in beta. Llama.cpp offloading is probably not going to work on your platform unless you uninstall llama-cpp-conv and reinstall it with the proper build flags. Look at the llama-cpp-python documentation and follow the revelant command but replace llama-cpp-python with llama-cpp-conv.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `llm-quantkit-0.22/llm_quantkit.egg-info/PKG-INFO` & `llm-quantkit-0.23/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,48 +1,58 @@
 Metadata-Version: 2.1
 Name: llm-quantkit
-Version: 0.22
+Version: 0.23
 Summary: cli tool for downloading and quantizing LLMs
 Author-email: xhedit <jevd@protonmail.com>
 License: MIT License
 Project-URL: repository, https://github.com/xhedit/quantkit
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click
 Requires-Dist: torch>=2.0.0
 Requires-Dist: einops
 Requires-Dist: tqdm
 Requires-Dist: transformers
 Requires-Dist: huggingface_hub
 Requires-Dist: safetensors
-Requires-Dist: auto-gptq
-Requires-Dist: autoawq
 Requires-Dist: exl2conv
 Requires-Dist: llama-cpp-conv
 Requires-Dist: sentencepiece
 Requires-Dist: hqq
-Provides-Extra: dev
+Provides-Extra: cuda
+Requires-Dist: auto-gptq; extra == "cuda"
+Requires-Dist: autoawq; extra == "cuda"
 
 # quantkit
 
 A tool for downloading and converting HuggingFace models without drama.
 
 <br/>
 
 # Install
+If you're on a machine with an NVIDIA/CUDA GPU and want AWQ/GPTQ support:
+```
+pip3 install llm-quantkit[cuda]
+```
+<br/>
+
+Otherwise, the default install works. <br/>
+
 ```
 pip3 install llm-quantkit
 ```
 <br/>
 
 # Requirements
-This project depends on torch, awq, exl2, gptq, and hqq libraries, some of which are not compatible with Python 3.12. <br/>
+
 If you need a device specific torch, install it first. <br/>
-Python: 3.8, 3.9, 3.10, and 3.11
 
+This project depends on torch, awq, exl2, gptq, and hqq libraries. <br/>
+Some of these dependencies do not support Python 3.12 yet. <br/>
+Supported Pythons: 3.8, 3.9, 3.10, and 3.11<br/>
 
 
 # Usage
 
 ```
 Usage: quantkit [OPTIONS] COMMAND [ARGS]...
 
@@ -63,15 +73,18 @@
 
 The download command defaults to downloading into the HF cache and producing symlinks in the output dir, but there is a --no-cache option which places the model files in the output directory. <br/>
 
 
 AWQ defaults to 4 bits, group size 128, zero-point True. <br />
 GPTQ defaults are 4 bits, group size 128, activation-order False. <br />
 EXL2 defaults to 8 head bits but there is no default bitrate. <br />
-GGUF defaults to no imatrix but there is no default quant-type. <br/>
+GGUF defaults to no imatrix but there is no default quant-type. <br />
+HQQ defaults to 4 bits, group size 64, zero_point=True. <br />
+
+<br/>
 
 # Examples
 
 Download a model from HF and don't use HF cache:
 ```
 quantkit download teknium/Hermes-Trismegistus-Mistral-7B --no-cache
 ```
@@ -136,8 +149,39 @@
 
 Convert a model to HQQ:
 ```
 quantkit hqq mistralai/Mistral-7B-v0.1 -out Mistral-7B-HQQ-w4-gs64
 ```
 <br/>
 
+# Hardware Requirements
+Here's what has worked for me in testing. Drop a PR or Issue with updates for what is possible on various size cards. <br />
+GGUF conversion doesn't need a GPU except for iMatrix and Exllamav2 requires that the largest layer fits on single GPU.
+
+|Model Size|Quant|VRAM|Successful|
+|--|--|--|--|
+|7B|AWQ|24GB|✅|
+|7B|EXL2|24GB|✅|
+|7B|GGUF|24GB|✅|
+|7B|GPTQ|24GB|✅|
+|7B|HQQ|24GB|✅|
+|13B|AWQ|24GB|✅|
+|13B|EXL2|24GB|✅|
+|13B|GGUF|24GB|✅|
+|13B|GPTQ|24GB|:x:|
+|13B|HQQ|24GB|?|
+|34B|AWQ|24GB|:x:|
+|34B|EXL2|24GB|✅|
+|34B|GGUF|24GB|✅|
+|34B|GPTQ|24GB|:x:|
+|34B|HQQ|24GB|?|
+|70B|AWQ|24GB|:x:|
+|70B|EXL2|24GB|✅|
+|70B|GGUF|24GB|✅|
+|70B|GPTQ|24GB|:x:|
+|70B|HQQ|24GB|?|
+
+<br />
+
+# Notes
+
 Still in beta. Llama.cpp offloading is probably not going to work on your platform unless you uninstall llama-cpp-conv and reinstall it with the proper build flags. Look at the llama-cpp-python documentation and follow the revelant command but replace llama-cpp-python with llama-cpp-conv.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `llm-quantkit-0.22/pyproject.toml` & `llm-quantkit-0.23/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -3,34 +3,35 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "llm-quantkit"
 description = "cli tool for downloading and quantizing LLMs"
 readme = "README.md"
 license = { text = "MIT License" }
-version = "0.22"
+version = "0.23"
 authors = [{ name = "xhedit", email = "jevd@protonmail.com" }]
 dependencies = [
     "click",
     "torch>=2.0.0",
     "einops",
     "tqdm",
     "transformers",
     "huggingface_hub",
     "safetensors",
-    "auto-gptq",
-    "autoawq",
     "exl2conv",
     "llama-cpp-conv",
     "sentencepiece",
     "hqq",
 ]
 
 [project.optional-dependencies]
-dev = []
+cuda = [
+    "auto-gptq",
+    "autoawq",
+]
 
 [project.urls]
 repository = "https://github.com/xhedit/quantkit"
 
 [project.scripts]
 quantkit = "quantkit.cli:main"
```

### Comparing `llm-quantkit-0.22/quantkit/cli.py` & `llm-quantkit-0.23/quantkit/cli.py`

 * *Files identical despite different names*

### Comparing `llm-quantkit-0.22/quantkit/convert.py` & `llm-quantkit-0.23/quantkit/convert.py`

 * *Files identical despite different names*

### Comparing `llm-quantkit-0.22/quantkit/quantkit.py` & `llm-quantkit-0.23/quantkit/quantkit.py`

 * *Files identical despite different names*

### Comparing `llm-quantkit-0.22/quantkit/safetensor.py` & `llm-quantkit-0.23/quantkit/safetensor.py`

 * *Files identical despite different names*

