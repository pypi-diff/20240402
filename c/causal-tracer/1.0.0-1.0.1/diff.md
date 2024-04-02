# Comparing `tmp/causal_tracer-1.0.0.tar.gz` & `tmp/causal_tracer-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "causal_tracer-1.0.0.tar", max compression
+gzip compressed data, was "causal_tracer-1.0.1.tar", max compression
```

## Comparing `causal_tracer-1.0.0.tar` & `causal_tracer-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1069 2023-08-17 11:22:43.701278 causal_tracer-1.0.0/LICENSE
--rw-r--r--   0        0        0     6618 2023-08-17 11:22:43.701278 causal_tracer-1.0.0/README.md
--rw-r--r--   0        0        0      647 2023-08-17 11:22:44.609315 causal_tracer-1.0.0/causal_tracer/__init__.py
--rw-r--r--   0        0        0     9331 2023-08-17 11:22:43.701278 causal_tracer-1.0.0/causal_tracer/causal_tracing/AsyncTracePatchProcessor.py
--rw-r--r--   0        0        0    15518 2023-08-17 11:22:43.701278 causal_tracer-1.0.0/causal_tracer/causal_tracing/CausalTracer.py
--rw-r--r--   0        0        0      465 2023-08-17 11:22:43.701278 causal_tracer-1.0.0/causal_tracer/causal_tracing/HiddenFlow.py
--rw-r--r--   0        0        0     1499 2023-08-17 11:22:43.701278 causal_tracer-1.0.0/causal_tracer/causal_tracing/LayerConfig.py
--rw-r--r--   0        0        0      258 2023-08-17 11:22:43.701278 causal_tracer-1.0.0/causal_tracer/causal_tracing/guess_subject.py
--rw-r--r--   0        0        0      614 2023-08-17 11:22:43.701278 causal_tracer-1.0.0/causal_tracer/causal_tracing/pick_noise_level.py
--rw-r--r--   0        0        0     2032 2023-08-17 11:22:43.701278 causal_tracer-1.0.0/causal_tracer/causal_tracing/plot_hidden_flow_heatmap.py
--rw-r--r--   0        0        0      683 2023-08-17 11:22:43.701278 causal_tracer-1.0.0/causal_tracer/lib/PseudoFuture.py
--rw-r--r--   0        0        0     4845 2023-08-17 11:22:43.701278 causal_tracer-1.0.0/causal_tracer/lib/TraceLayer.py
--rw-r--r--   0        0        0     3008 2023-08-17 11:22:43.701278 causal_tracer-1.0.0/causal_tracer/lib/TraceLayerDict.py
--rw-r--r--   0        0        0       93 2023-08-17 11:22:43.701278 causal_tracer-1.0.0/causal_tracer/lib/constants.py
--rw-r--r--   0        0        0     1996 2023-08-17 11:22:43.701278 causal_tracer-1.0.0/causal_tracer/lib/layer_matching.py
--rw-r--r--   0        0        0      266 2023-08-17 11:22:43.701278 causal_tracer-1.0.0/causal_tracer/lib/logger.py
--rw-r--r--   0        0        0     8492 2023-08-17 11:22:43.705278 causal_tracer-1.0.0/causal_tracer/lib/token_utils.py
--rw-r--r--   0        0        0     2162 2023-08-17 11:22:43.705278 causal_tracer-1.0.0/causal_tracer/lib/torch_utils.py
--rw-r--r--   0        0        0      953 2023-08-17 11:22:43.705278 causal_tracer-1.0.0/causal_tracer/lib/util.py
--rw-r--r--   0        0        0      765 2023-08-17 11:22:44.609315 causal_tracer-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     7088 1970-01-01 00:00:00.000000 causal_tracer-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-02 10:44:11.346377 causal_tracer-1.0.1/LICENSE
+-rw-r--r--   0        0        0     7631 2024-04-02 10:44:11.346377 causal_tracer-1.0.1/README.md
+-rw-r--r--   0        0        0      647 2024-04-02 10:44:12.218375 causal_tracer-1.0.1/causal_tracer/__init__.py
+-rw-r--r--   0        0        0     9331 2024-04-02 10:44:11.346377 causal_tracer-1.0.1/causal_tracer/causal_tracing/AsyncTracePatchProcessor.py
+-rw-r--r--   0        0        0    15518 2024-04-02 10:44:11.346377 causal_tracer-1.0.1/causal_tracer/causal_tracing/CausalTracer.py
+-rw-r--r--   0        0        0      465 2024-04-02 10:44:11.346377 causal_tracer-1.0.1/causal_tracer/causal_tracing/HiddenFlow.py
+-rw-r--r--   0        0        0     1499 2024-04-02 10:44:11.346377 causal_tracer-1.0.1/causal_tracer/causal_tracing/LayerConfig.py
+-rw-r--r--   0        0        0      258 2024-04-02 10:44:11.346377 causal_tracer-1.0.1/causal_tracer/causal_tracing/guess_subject.py
+-rw-r--r--   0        0        0      614 2024-04-02 10:44:11.346377 causal_tracer-1.0.1/causal_tracer/causal_tracing/pick_noise_level.py
+-rw-r--r--   0        0        0     2032 2024-04-02 10:44:11.346377 causal_tracer-1.0.1/causal_tracer/causal_tracing/plot_hidden_flow_heatmap.py
+-rw-r--r--   0        0        0      683 2024-04-02 10:44:11.346377 causal_tracer-1.0.1/causal_tracer/lib/PseudoFuture.py
+-rw-r--r--   0        0        0     4611 2024-04-02 10:44:11.346377 causal_tracer-1.0.1/causal_tracer/lib/TraceLayer.py
+-rw-r--r--   0        0        0     2738 2024-04-02 10:44:11.346377 causal_tracer-1.0.1/causal_tracer/lib/TraceLayerDict.py
+-rw-r--r--   0        0        0       93 2024-04-02 10:44:11.346377 causal_tracer-1.0.1/causal_tracer/lib/constants.py
+-rw-r--r--   0        0        0     1996 2024-04-02 10:44:11.346377 causal_tracer-1.0.1/causal_tracer/lib/layer_matching.py
+-rw-r--r--   0        0        0      266 2024-04-02 10:44:11.346377 causal_tracer-1.0.1/causal_tracer/lib/logger.py
+-rw-r--r--   0        0        0     8492 2024-04-02 10:44:11.346377 causal_tracer-1.0.1/causal_tracer/lib/token_utils.py
+-rw-r--r--   0        0        0     1640 2024-04-02 10:44:11.346377 causal_tracer-1.0.1/causal_tracer/lib/torch_utils.py
+-rw-r--r--   0        0        0      953 2024-04-02 10:44:11.346377 causal_tracer-1.0.1/causal_tracer/lib/util.py
+-rw-r--r--   0        0        0      844 2024-04-02 10:44:12.218375 causal_tracer-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     8270 1970-01-01 00:00:00.000000 causal_tracer-1.0.1/PKG-INFO
```

### Comparing `causal_tracer-1.0.0/LICENSE` & `causal_tracer-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `causal_tracer-1.0.0/README.md` & `causal_tracer-1.0.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Causal Tracer
 
 [![ci](https://img.shields.io/github/actions/workflow/status/chanind/causal-tracer/ci.yaml?branch=main)](https://github.com/chanind/causal-tracer)
+[![Codecov](https://img.shields.io/codecov/c/github/chanind/causal-tracer/main)](https://codecov.io/gh/chanind/causal-tracer)
 [![PyPI](https://img.shields.io/pypi/v/causal-tracer?color=blue)](https://pypi.org/project/causal-tracer/)
 
 Causal trace plots for transformer language models.
 
 Demo:
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1rOA_r7Gv6bGjXNfUvrqk9Gt3dLwZNvGJ?usp=sharing)
 
@@ -27,38 +28,38 @@
 ```
 
 ## Basic usage
 
 If you're generating causal traces for a Llama-based model or GPT2, you don't need any further configuration.
 
 ```python
-from transformers import AutoModel, AutoTokenizer
+from transformers import AutoModelForCausalLM, AutoTokenizer
 from causal_tracer import CausalTracer, plot_hidden_flow_heatmap
 
-model = AutoModel.from_pretrained("gpt2-medium")
-tokenizer = AutoTokenizer.from-pretrained("gpt2-medium")
+model = AutoModelForCausalLM.from_pretrained("gpt2-medium")
+tokenizer = AutoTokenizer.from_pretrained("gpt2-medium")
 tracer = CausalTracer(model, tokenizer)
 
 # perform causal tracing across hidden layers (residual stream) of the model
 hidden_layer_flow = tracer.calculate_hidden_flow(
   "The Space Needle is located in the city of",
   subject="The Space Needle",
 )
 # plot the result
 plot_hidden_flow_heatmap(hidden_layer_flow)
 ```
 
 You can also generate causal traces of MLP layers or attention layers in the transformer.
 
 ```python
-from transformers import AutoModel, AutoTokenizer
+from transformers import AutoModelForCausalLM, AutoTokenizer
 from causal_tracer import CausalTracer, plot_hidden_flow_heatmap
 
-model = AutoModel.from_pretrained("gpt2-medium")
-tokenizer = AutoTokenizer.from-pretrained("gpt2-medium")
+model = AutoModelForCausalLM.from_pretrained("gpt2-medium")
+tokenizer = AutoTokenizer.from_pretrained("gpt2-medium")
 tracer = CausalTracer(model, tokenizer)
 
 # perform causal tracing across MLP layers of the model
 mlp_layer_flow = tracer.calculate_hidden_flow(
   "The Space Needle is located in the city of",
   subject="The Space Needle",
   kind="mlp",
@@ -119,10 +120,29 @@
   embedding_layer="wte",
 )
 tracer = CausalTracer(model, tokenizer, layer_config=custom_layer_config)
 ```
 
 Note that `hidden_layers_matcher`, `attention_layers_matcher`, and `mlp_layers_matcher` are template strings, containg `{num}` in the middle. During processing, `{num}` will get replaced with the layer number. These strings correspond to the named modules of the transformer. You find all the named modules of a Pytorch model by running `model.named_modules()`.
 
+## Using hidden flow results directly
+
+If you want to use the results of the `tracer.calculate_hidden_flow()` method in downstream tasks instead of just making a plot, the returned `HiddenFlow` object contains a number of fields which can be further analyzed. The full `HiddenFlow` dataclass types are below:
+
+```python
+class HiddenFlow:
+    scores: torch.Tensor
+    low_score: float
+    high_score: float
+    input_ids: torch.Tensor
+    input_tokens: list[str]
+    subject_range: tuple[int, int]
+    answer: str
+    kind: LayerKind # one of "hidden", "attention", or "mlp"
+    layer_outputs: OrderedDict[str, torch.Tensor]
+```
+
+Of particular interest, the `score` attribute contains the full matrix of causal tracing scores. The `layer_outputs` attribute contains the uncorrupted layer activations for each layer of the type being analyzed.
+
 ## Contributing
 
 Contributions are welcome! If you submit code, please make sure to add or update tests coverage along with your change. This repo uses Black for code formatting, MyPy for type checking, and Flake8 for linting.
```

### Comparing `causal_tracer-1.0.0/causal_tracer/__init__.py` & `causal_tracer-1.0.1/causal_tracer/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 
 from causal_tracer.causal_tracing.CausalTracer import CausalTracer, HiddenFlowQuery
 from causal_tracer.causal_tracing.HiddenFlow import HiddenFlow
 from causal_tracer.causal_tracing.plot_hidden_flow_heatmap import (
     plot_hidden_flow_heatmap,
 )
 from causal_tracer.causal_tracing.LayerConfig import (
```

### Comparing `causal_tracer-1.0.0/causal_tracer/causal_tracing/AsyncTracePatchProcessor.py` & `causal_tracer-1.0.1/causal_tracer/causal_tracing/AsyncTracePatchProcessor.py`

 * *Files identical despite different names*

### Comparing `causal_tracer-1.0.0/causal_tracer/causal_tracing/CausalTracer.py` & `causal_tracer-1.0.1/causal_tracer/causal_tracing/CausalTracer.py`

 * *Files identical despite different names*

### Comparing `causal_tracer-1.0.0/causal_tracer/causal_tracing/LayerConfig.py` & `causal_tracer-1.0.1/causal_tracer/causal_tracing/LayerConfig.py`

 * *Files identical despite different names*

### Comparing `causal_tracer-1.0.0/causal_tracer/causal_tracing/pick_noise_level.py` & `causal_tracer-1.0.1/causal_tracer/causal_tracing/pick_noise_level.py`

 * *Files identical despite different names*

### Comparing `causal_tracer-1.0.0/causal_tracer/causal_tracing/plot_hidden_flow_heatmap.py` & `causal_tracer-1.0.1/causal_tracer/causal_tracing/plot_hidden_flow_heatmap.py`

 * *Files identical despite different names*

### Comparing `causal_tracer-1.0.0/causal_tracer/lib/PseudoFuture.py` & `causal_tracer-1.0.1/causal_tracer/lib/PseudoFuture.py`

 * *Files identical despite different names*

### Comparing `causal_tracer-1.0.0/causal_tracer/lib/TraceLayer.py` & `causal_tracer-1.0.1/causal_tracer/lib/TraceLayer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 """
 Utilities for instrumenting a torch model.
 
 Trace will hook one layer at a time.
-TraceDict will hook multiple layers at once.
-subsequence slices intervals from Sequential modules.
-get_module, replace_module, get_parameter resolve dotted names.
-set_requires_grad recursively sets requires_grad in module parameters.
 
 Copied from https://github.com/kmeng01/rome/blob/main/util/nethook.py
 """
 
 from __future__ import annotations
 
 import contextlib
```

### Comparing `causal_tracer-1.0.0/causal_tracer/lib/TraceLayerDict.py` & `causal_tracer-1.0.1/causal_tracer/lib/TraceLayerDict.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,9 @@
 """
-Utilities for instrumenting a torch model.
-
-Trace will hook one layer at a time.
 TraceDict will hook multiple layers at once.
-subsequence slices intervals from Sequential modules.
-get_module, replace_module, get_parameter resolve dotted names.
-set_requires_grad recursively sets requires_grad in module parameters.
 
 Copied from https://github.com/kmeng01/rome/blob/main/util/nethook.py
 """
 
 from __future__ import annotations
 
 import contextlib
```

### Comparing `causal_tracer-1.0.0/causal_tracer/lib/layer_matching.py` & `causal_tracer-1.0.1/causal_tracer/lib/layer_matching.py`

 * *Files identical despite different names*

### Comparing `causal_tracer-1.0.0/causal_tracer/lib/token_utils.py` & `causal_tracer-1.0.1/causal_tracer/lib/token_utils.py`

 * *Files identical despite different names*

### Comparing `causal_tracer-1.0.0/causal_tracer/lib/torch_utils.py` & `causal_tracer-1.0.1/causal_tracer/lib/torch_utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,29 +11,14 @@
     """
     for n, m in model.named_modules():
         if n == name:
             return m
     raise LookupError(name)
 
 
-def set_requires_grad(requires_grad: bool, *models: nn.Module) -> None:
-    """
-    Sets requires_grad true or false for all parameters within the
-    models passed.
-    """
-    for model in models:
-        if isinstance(model, nn.Module):
-            for param in model.parameters():
-                param.requires_grad = requires_grad
-        elif isinstance(model, (nn.Parameter, torch.Tensor)):
-            model.requires_grad = requires_grad
-        else:
-            raise TypeError(f"unknown type {type(model)}")
-
-
 def untuple_tensor(x: torch.Tensor | tuple[torch.Tensor, ...]) -> torch.Tensor:
     return x[0] if isinstance(x, tuple) else x
 
 
 T = TypeVar("T", torch.Tensor, dict[Any, Any], list[Any], tuple[Any, ...])
```

### Comparing `causal_tracer-1.0.0/causal_tracer/lib/util.py` & `causal_tracer-1.0.1/causal_tracer/lib/util.py`

 * *Files identical despite different names*

### Comparing `causal_tracer-1.0.0/pyproject.toml` & `causal_tracer-1.0.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [tool.poetry]
 name = "causal-tracer"
-version = "1.0.0"
+version = "1.0.1"
 description = ""
 authors = ["David Chanin <chanindav@gmail.com>"]
 readme = "README.md"
 packages = [{include = "causal_tracer"}]
+repository = "https://github.com/chanind/causal-tracer"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 transformers = "^4.28.1"
 matplotlib = "^3.7.1"
 tqdm = "^4.66.1"
 
@@ -17,20 +18,21 @@
 pytest = "^7.3.1"
 black = "^23.3.0"
 mypy = "^1.2.0"
 torch = "2.0.0"
 flake8 = "^6.0.0"
 syrupy = "^4.0.8"
 sentencepiece = "^0.1.99"
+pytest-cov = "^4.1.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.semantic_release]
 version_variables = [
     "causal_tracer/__init__.py:__version__",
     "pyproject.toml:version"
 ]
 branch = "main"
 upload_to_vcs_elease = true
-build_command = "pip install poetry && poetry build"
+build_command = "pip install poetry && poetry build"
```

### Comparing `causal_tracer-1.0.0/PKG-INFO` & `causal_tracer-1.0.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 Metadata-Version: 2.1
 Name: causal-tracer
-Version: 1.0.0
+Version: 1.0.1
 Summary: 
+Home-page: https://github.com/chanind/causal-tracer
 Author: David Chanin
 Author-email: chanindav@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: tqdm (>=4.66.1,<5.0.0)
 Requires-Dist: transformers (>=4.28.1,<5.0.0)
+Project-URL: Repository, https://github.com/chanind/causal-tracer
 Description-Content-Type: text/markdown
 
 # Causal Tracer
 
 [![ci](https://img.shields.io/github/actions/workflow/status/chanind/causal-tracer/ci.yaml?branch=main)](https://github.com/chanind/causal-tracer)
+[![Codecov](https://img.shields.io/codecov/c/github/chanind/causal-tracer/main)](https://codecov.io/gh/chanind/causal-tracer)
 [![PyPI](https://img.shields.io/pypi/v/causal-tracer?color=blue)](https://pypi.org/project/causal-tracer/)
 
 Causal trace plots for transformer language models.
 
 Demo:
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1rOA_r7Gv6bGjXNfUvrqk9Gt3dLwZNvGJ?usp=sharing)
 
@@ -42,38 +46,38 @@
 ```
 
 ## Basic usage
 
 If you're generating causal traces for a Llama-based model or GPT2, you don't need any further configuration.
 
 ```python
-from transformers import AutoModel, AutoTokenizer
+from transformers import AutoModelForCausalLM, AutoTokenizer
 from causal_tracer import CausalTracer, plot_hidden_flow_heatmap
 
-model = AutoModel.from_pretrained("gpt2-medium")
-tokenizer = AutoTokenizer.from-pretrained("gpt2-medium")
+model = AutoModelForCausalLM.from_pretrained("gpt2-medium")
+tokenizer = AutoTokenizer.from_pretrained("gpt2-medium")
 tracer = CausalTracer(model, tokenizer)
 
 # perform causal tracing across hidden layers (residual stream) of the model
 hidden_layer_flow = tracer.calculate_hidden_flow(
   "The Space Needle is located in the city of",
   subject="The Space Needle",
 )
 # plot the result
 plot_hidden_flow_heatmap(hidden_layer_flow)
 ```
 
 You can also generate causal traces of MLP layers or attention layers in the transformer.
 
 ```python
-from transformers import AutoModel, AutoTokenizer
+from transformers import AutoModelForCausalLM, AutoTokenizer
 from causal_tracer import CausalTracer, plot_hidden_flow_heatmap
 
-model = AutoModel.from_pretrained("gpt2-medium")
-tokenizer = AutoTokenizer.from-pretrained("gpt2-medium")
+model = AutoModelForCausalLM.from_pretrained("gpt2-medium")
+tokenizer = AutoTokenizer.from_pretrained("gpt2-medium")
 tracer = CausalTracer(model, tokenizer)
 
 # perform causal tracing across MLP layers of the model
 mlp_layer_flow = tracer.calculate_hidden_flow(
   "The Space Needle is located in the city of",
   subject="The Space Needle",
   kind="mlp",
@@ -134,11 +138,30 @@
   embedding_layer="wte",
 )
 tracer = CausalTracer(model, tokenizer, layer_config=custom_layer_config)
 ```
 
 Note that `hidden_layers_matcher`, `attention_layers_matcher`, and `mlp_layers_matcher` are template strings, containg `{num}` in the middle. During processing, `{num}` will get replaced with the layer number. These strings correspond to the named modules of the transformer. You find all the named modules of a Pytorch model by running `model.named_modules()`.
 
+## Using hidden flow results directly
+
+If you want to use the results of the `tracer.calculate_hidden_flow()` method in downstream tasks instead of just making a plot, the returned `HiddenFlow` object contains a number of fields which can be further analyzed. The full `HiddenFlow` dataclass types are below:
+
+```python
+class HiddenFlow:
+    scores: torch.Tensor
+    low_score: float
+    high_score: float
+    input_ids: torch.Tensor
+    input_tokens: list[str]
+    subject_range: tuple[int, int]
+    answer: str
+    kind: LayerKind # one of "hidden", "attention", or "mlp"
+    layer_outputs: OrderedDict[str, torch.Tensor]
+```
+
+Of particular interest, the `score` attribute contains the full matrix of causal tracing scores. The `layer_outputs` attribute contains the uncorrupted layer activations for each layer of the type being analyzed.
+
 ## Contributing
 
 Contributions are welcome! If you submit code, please make sure to add or update tests coverage along with your change. This repo uses Black for code formatting, MyPy for type checking, and Flake8 for linting.
```

