# Comparing `tmp/steering_vectors-0.8.0.tar.gz` & `tmp/steering_vectors-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "steering_vectors-0.8.0.tar", max compression
+gzip compressed data, was "steering_vectors-0.9.0.tar", max compression
```

## Comparing `steering_vectors-0.8.0.tar` & `steering_vectors-0.9.0.tar`

### file list

```diff
@@ -1,11 +1,13 @@
--rw-r--r--   0        0        0     1073 2024-02-21 16:43:50.330794 steering_vectors-0.8.0/LICENSE
--rw-r--r--   0        0        0     4073 2024-02-21 16:43:50.330794 steering_vectors-0.8.0/README.md
--rw-r--r--   0        0        0      971 2024-02-21 16:43:51.286801 steering_vectors-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      900 2024-02-21 16:43:51.286801 steering_vectors-0.8.0/steering_vectors/__init__.py
--rw-r--r--   0        0        0     2799 2024-02-21 16:43:50.330794 steering_vectors-0.8.0/steering_vectors/aggregators.py
--rw-r--r--   0        0        0     6750 2024-02-21 16:43:50.330794 steering_vectors-0.8.0/steering_vectors/layer_matching.py
--rw-r--r--   0        0        0     3266 2024-02-21 16:43:50.330794 steering_vectors-0.8.0/steering_vectors/record_activations.py
--rw-r--r--   0        0        0     8313 2024-02-21 16:43:50.330794 steering_vectors-0.8.0/steering_vectors/steering_vector.py
--rw-r--r--   0        0        0      637 2024-02-21 16:43:50.330794 steering_vectors-0.8.0/steering_vectors/torch_utils.py
--rw-r--r--   0        0        0     5834 2024-02-21 16:43:50.330794 steering_vectors-0.8.0/steering_vectors/train_steering_vector.py
--rw-r--r--   0        0        0     4735 1970-01-01 00:00:00.000000 steering_vectors-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-02-21 17:01:40.424220 steering_vectors-0.9.0/LICENSE
+-rw-r--r--   0        0        0     4073 2024-02-21 17:01:40.424220 steering_vectors-0.9.0/README.md
+-rw-r--r--   0        0        0     1003 2024-02-21 17:01:41.408208 steering_vectors-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      910 2024-02-21 17:01:41.408208 steering_vectors-0.9.0/steering_vectors/__init__.py
+-rw-r--r--   0        0        0     2799 2024-02-21 17:01:40.424220 steering_vectors-0.9.0/steering_vectors/aggregators.py
+-rw-r--r--   0        0        0     6709 2024-02-21 17:01:40.424220 steering_vectors-0.9.0/steering_vectors/layer_matching.py
+-rw-r--r--   0        0        0     3250 2024-02-21 17:01:40.424220 steering_vectors-0.9.0/steering_vectors/record_activations.py
+-rw-r--r--   0        0        0     8305 2024-02-21 17:01:40.424220 steering_vectors-0.9.0/steering_vectors/steering_vector.py
+-rw-r--r--   0        0        0     1647 2024-02-21 17:01:40.424220 steering_vectors-0.9.0/steering_vectors/token_utils.py
+-rw-r--r--   0        0        0      637 2024-02-21 17:01:40.424220 steering_vectors-0.9.0/steering_vectors/torch_utils.py
+-rw-r--r--   0        0        0     6703 2024-02-21 17:01:40.424220 steering_vectors-0.9.0/steering_vectors/train_steering_vector.py
+-rw-r--r--   0        0        0      584 2024-02-21 17:01:40.424220 steering_vectors-0.9.0/steering_vectors/utils.py
+-rw-r--r--   0        0        0     4735 1970-01-01 00:00:00.000000 steering_vectors-0.9.0/PKG-INFO
```

### Comparing `steering_vectors-0.8.0/LICENSE` & `steering_vectors-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `steering_vectors-0.8.0/README.md` & `steering_vectors-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `steering_vectors-0.8.0/pyproject.toml` & `steering_vectors-0.9.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "steering-vectors"
-version = "0.8.0"
+version = "0.9.0"
 description = "Steering vectors for transformer language models in Pytorch / Huggingface"
 authors = [
     "David Chanin <chanindav@gmail.com>",
     "Daniel Tan <dtch009@gmail.com>",
 ]
 readme = "README.md"
 license = "MIT"
@@ -24,14 +24,15 @@
 furo = "^2023.9.10"
 pygments = "^2.17.2"
 torch = "^2.1.2"
 protobuf = "^4.25.2"
 flake8 = "^7.0.0"
 sentencepiece = "^0.1.99"
 sphinx-autodoc-typehints = "^1.25.2"
+flake8-tidy-imports = "^4.10.0"
 
 [tool.isort]
 profile = "black"
 
 [tool.semantic_release]
 version_variables = [
     "steering_vectors/__init__.py:__version__",
```

### Comparing `steering_vectors-0.8.0/steering_vectors/__init__.py` & `steering_vectors-0.9.0/steering_vectors/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.8.0"
+__version__ = "0.9.0"
 
 from .aggregators import (
     Aggregator,
     logistic_aggregator,
     mean_aggregator,
     pca_aggregator,
 )
@@ -10,27 +10,27 @@
     LayerMatcher,
     LayerType,
     ModelLayerConfig,
     get_num_matching_layers,
     guess_and_enhance_layer_config,
 )
 from .record_activations import record_activations
-from .steering_vector import PatchOperator, SteeringPatchHandle, SteeringVector
+from .steering_vector import PatchDeltaOperator, SteeringPatchHandle, SteeringVector
 from .train_steering_vector import SteeringVectorTrainingSample, train_steering_vector
 
 __all__ = [
     "Aggregator",
     "mean_aggregator",
     "pca_aggregator",
     "logistic_aggregator",
     "LayerType",
     "LayerMatcher",
     "ModelLayerConfig",
     "get_num_matching_layers",
     "guess_and_enhance_layer_config",
-    "PatchOperator",
+    "PatchDeltaOperator",
     "record_activations",
     "SteeringVector",
     "SteeringPatchHandle",
     "train_steering_vector",
     "SteeringVectorTrainingSample",
 ]
```

### Comparing `steering_vectors-0.8.0/steering_vectors/aggregators.py` & `steering_vectors-0.9.0/steering_vectors/aggregators.py`

 * *Files identical despite different names*

### Comparing `steering_vectors-0.8.0/steering_vectors/layer_matching.py` & `steering_vectors-0.9.0/steering_vectors/layer_matching.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import re
 from collections import defaultdict
-from typing import Callable, Iterable, Literal, Optional, Union
+from typing import Callable, Iterable, Literal
 
 from torch import nn
 
-LayerMatcher = Union[str, Callable[[nn.Module, int], str]]
+LayerMatcher = str | Callable[[nn.Module, int], str]
 
 
 def collect_matching_layers(model: nn.Module, layer_matcher: LayerMatcher) -> list[str]:
     """
     Find all layers in the model that match the layer_matcher, in order by layer_num.
     layer_matcher can be a string formatted like "transformer.h.{num}.mlp" or a callable
     If layer_matcher is a callable, it should take in a model and layer_num and return
     a string representing the layer name corresponding to that layer number.
     If layer_matcher is a string, it's considered a template and MUST contain a "{num}" portion
     """
     matcher_callable = _layer_matcher_to_callable(layer_matcher)
     all_layer_names = dict(model.named_modules()).keys()
     matching_layers = []
-    for layer_num, layer in enumerate(model.modules()):
+    for layer_num in range(len(all_layer_names)):
         layer_name = matcher_callable(model, layer_num)
         if layer_name in all_layer_names:
             matching_layers.append(layer_name)
         else:
             break
     return matching_layers
 
@@ -113,15 +113,15 @@
         dict(model.named_modules()).keys(),
         filter=lambda guess: "ln_2" in guess or "post_attention_layernorm" in guess,
     )
 
 
 # broken into a separate function for easier testing
 def _guess_block_matcher_from_layers(
-    layers: Iterable[str], filter: Optional[Callable[[str], bool]] = None
+    layers: Iterable[str], filter: Callable[[str], bool] | None = None
 ) -> str | None:
     counts_by_guess: dict[str, int] = defaultdict(int)
 
     for layer in layers:
         if re.match(LAYER_GUESS_RE, layer):
             guess = re.sub(LAYER_GUESS_RE, r"\1.{num}\3", layer)
             if filter is None or filter(guess):
@@ -149,15 +149,15 @@
     "mlp": guess_mlp_matcher,
     "input_layernorm": guess_input_layernorm_matcher,
     "post_attention_layernorm": guess_post_attention_layernorm_matcher,
 }
 
 
 def enhance_model_config_matchers(
-    model: nn.Module, config: ModelLayerConfig, layer_type: Optional[LayerType] = None
+    model: nn.Module, config: ModelLayerConfig, layer_type: LayerType | None = None
 ) -> ModelLayerConfig:
     """Returns a new layer config, attempting to fill-in missing layer matchers"""
     enhanced_config: ModelLayerConfig = {**config}
     types_to_guess: Iterable[LayerType] = (
         [layer_type] if layer_type is not None else _LAYER_TYPE_TO_GUESSER.keys()
     )
     for guess_layer_type in types_to_guess:
@@ -166,16 +166,16 @@
         ):
             enhanced_config[guess_layer_type] = layer_matcher
     return enhanced_config
 
 
 def guess_and_enhance_layer_config(
     model: nn.Module,
-    layer_config: Optional[ModelLayerConfig] = None,
-    layer_type: Optional[LayerType] = None,
+    layer_config: ModelLayerConfig | None = None,
+    layer_type: LayerType | None = None,
 ) -> ModelLayerConfig:
     """
     Try to guess any missing parts of the layer config, after checking against predefined configs.
     If layer_type is provided, only guess the layer_matcher for that layer type.
     """
     layer_config = enhance_model_config_matchers(
         model, layer_config or {}, layer_type=layer_type
```

### Comparing `steering_vectors-0.8.0/steering_vectors/record_activations.py` & `steering_vectors-0.9.0/steering_vectors/record_activations.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from collections import defaultdict
 from contextlib import contextmanager
-from typing import Any, Generator, Optional, Sequence, cast
+from typing import Any, Generator, Sequence, cast
 
 from torch import Tensor, nn
 from torch.utils.hooks import RemovableHandle
 
 from .layer_matching import (
     LayerType,
     ModelLayerConfig,
@@ -14,17 +14,17 @@
 from .torch_utils import get_module, untuple_tensor
 
 
 @contextmanager
 def record_activations(
     model: nn.Module,
     layer_type: LayerType = "decoder_block",
-    layer_config: Optional[ModelLayerConfig] = None,
+    layer_config: ModelLayerConfig | None = None,
     clone_activations: bool = True,
-    layer_nums: Optional[Sequence[int]] = None,
+    layer_nums: Sequence[int] | None = None,
 ) -> Generator[dict[int, list[Tensor]], None, None]:
     """
     Record the model activations at each layer of type `layer_type`.
     This function will record every forward pass through the model
     at all layers of the given layer_type.
 
     Args:
```

### Comparing `steering_vectors-0.8.0/steering_vectors/steering_vector.py` & `steering_vectors-0.9.0/steering_vectors/steering_vector.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from contextlib import contextmanager
 from dataclasses import dataclass, replace
-from typing import Any, Callable, Generator, Optional, overload
+from typing import Any, Callable, Generator, overload
 
 import torch
 from torch import Tensor, nn
 from torch.utils.hooks import RemovableHandle
 
 from .layer_matching import (
     LayerType,
     ModelLayerConfig,
     collect_matching_layers,
     guess_and_enhance_layer_config,
 )
 from .torch_utils import get_module, untuple_tensor
 
-PatchOperator = Callable[[Tensor, Tensor], Tensor]
+PatchDeltaOperator = Callable[[Tensor, Tensor], Tensor]
 
 
 @dataclass
 class SteeringPatchHandle:
     """
     A handle that can be used to remove a steering patch from a model after
     running `steering_vector.patch_activations()`.
@@ -38,16 +38,16 @@
 
     layer_activations: dict[int, Tensor]
     layer_type: LayerType = "decoder_block"
 
     def patch_activations(
         self,
         model: nn.Module,
-        layer_config: Optional[ModelLayerConfig] = None,
-        operator: Optional[PatchOperator] = None,
+        layer_config: ModelLayerConfig | None = None,
+        operator: PatchDeltaOperator | None = None,
         multiplier: float = 1.0,
         min_token_index: int | None = None,
         token_indices: list[int] | slice | Tensor | None = None,
     ) -> SteeringPatchHandle:
         """
         Patch the activations of the given model with this steering vector.
         This will modify the model in-place, and return a handle that can be used to undo the patching.
@@ -107,16 +107,16 @@
             hooks.append(handle)
         return SteeringPatchHandle(hooks)
 
     @contextmanager
     def apply(
         self,
         model: nn.Module,
-        layer_config: Optional[ModelLayerConfig] = None,
-        operator: Optional[PatchOperator] = None,
+        layer_config: ModelLayerConfig | None = None,
+        operator: PatchDeltaOperator | None = None,
         multiplier: float = 1.0,
         min_token_index: int = 0,
         token_indices: list[int] | slice | Tensor | None = None,
     ) -> Generator[None, None, None]:
         """
         Apply this steering vector to the given model. Tokens to patch
         can be selected using either `min_token_index` or `token_indices`, but not both.
@@ -157,16 +157,16 @@
         self, dtype: torch.dtype, non_blocking: bool = False, copy: bool = False
     ) -> "SteeringVector":
         ...
 
     @overload
     def to(
         self,
-        device: Optional[torch.device | str] = None,
-        dtype: Optional[torch.dtype] = None,
+        device: torch.device | str | None = None,
+        dtype: torch.dtype | None = None,
         non_blocking: bool = False,
         copy: bool = False,
     ) -> "SteeringVector":
         ...
 
     @overload
     def to(
@@ -186,15 +186,15 @@
         }
         return replace(self, layer_activations=layer_activations)
 
 
 def _create_additive_hook(
     target_activation: Tensor,
     token_indices: list[int] | slice | Tensor,
-    operator: PatchOperator | None = None,
+    operator: PatchDeltaOperator | None = None,
 ) -> Any:
     """Create a hook function that adds the given target_activation to the model output"""
 
     def hook_fn(_m: Any, _inputs: Any, outputs: Any) -> Any:
         original_tensor = untuple_tensor(outputs)
         act = target_activation.to(original_tensor.device)
         delta = act
```

### Comparing `steering_vectors-0.8.0/steering_vectors/torch_utils.py` & `steering_vectors-0.9.0/steering_vectors/torch_utils.py`

 * *Files identical despite different names*

### Comparing `steering_vectors-0.8.0/steering_vectors/train_steering_vector.py` & `steering_vectors-0.9.0/steering_vectors/train_steering_vector.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,44 +1,46 @@
 from collections import defaultdict
 from dataclasses import dataclass
-from typing import Callable, Optional
+from typing import Callable, Sequence
 
 import torch
 from torch import Tensor, nn
-from tqdm import tqdm
 from transformers import PreTrainedTokenizerBase
 
 from steering_vectors.aggregators import Aggregator, mean_aggregator
+from steering_vectors.token_utils import adjust_read_indices_for_padding, fix_pad_token
+from steering_vectors.utils import batchify
 
 from .layer_matching import LayerType, ModelLayerConfig, guess_and_enhance_layer_config
 from .record_activations import record_activations
 from .steering_vector import SteeringVector
 
 
 @dataclass
 class SteeringVectorTrainingSample:
     positive_str: str
     negative_str: str
-    read_positive_token_index: Optional[int] = None
-    read_negative_token_index: Optional[int] = None
+    read_positive_token_index: int | None = None
+    read_negative_token_index: int | None = None
 
 
 @torch.no_grad()
 def train_steering_vector(
     model: nn.Module,
     tokenizer: PreTrainedTokenizerBase,
-    training_samples: list[SteeringVectorTrainingSample] | list[tuple[str, str]],
-    layers: Optional[list[int]] = None,
+    training_samples: Sequence[SteeringVectorTrainingSample | tuple[str, str]],
+    layers: list[int] | None = None,
     layer_type: LayerType = "decoder_block",
-    layer_config: Optional[ModelLayerConfig] = None,
+    layer_config: ModelLayerConfig | None = None,
     move_to_cpu: bool = False,
     read_token_index: int | Callable[[str], int] = -1,
     show_progress: bool = False,
     aggregator: Aggregator = mean_aggregator(),
-    # TODO: add more options to control training
+    batch_size: int = 1,
+    tqdm_desc: str = "Training steering vector",
 ) -> SteeringVector:
     """
     Train a steering vector for the given model.
 
     Args:
         model: The model to train the steering vector for
         tokenizer: The tokenizer to use
@@ -53,97 +55,122 @@
             If not provided, this will be inferred automatically.
         move_to_cpu: If True, move the activations to the CPU before training. Default False.
         read_token_index: The index of the token to read the activations from. Default -1, meaning final token.
         show_progress: If True, show a progress bar. Default False.
         aggregator: A function that takes the positive and negative activations for a
             layer and returns a single vector. Default is mean_aggregator.
     """
+    fix_pad_token(tokenizer)
     layer_config = guess_and_enhance_layer_config(model, layer_config, layer_type)
     pos_activations: dict[int, list[Tensor]] = defaultdict(list)
     neg_activations: dict[int, list[Tensor]] = defaultdict(list)
 
-    if isinstance(training_samples[0], tuple):
-        sv_training_samples: list[SteeringVectorTrainingSample] = [
-            SteeringVectorTrainingSample(sample[0], sample[1], None, None)  # type: ignore
-            for sample in training_samples
-        ]
-    else:
-        sv_training_samples = training_samples  # type: ignore[assignment]
-
-    # TODO: batching
-    for training_sample in tqdm(
-        sv_training_samples,
-        disable=not show_progress,
-        desc="Training steering vector",
+    for raw_batch in batchify(
+        training_samples,
+        batch_size=batch_size,
+        show_progress=show_progress,
+        tqdm_desc=tqdm_desc,
     ):
-        pos_index = _get_token_index(
-            training_sample.read_positive_token_index,
-            read_token_index,
-            training_sample.positive_str,
-        )
-        neg_index = _get_token_index(
-            training_sample.read_negative_token_index,
-            read_token_index,
-            training_sample.negative_str,
-        )
+        batch = _formalize_batch(raw_batch)
+        pos_indices = []
+        neg_indices = []
+        pos_prompts = []
+        neg_prompts = []
+        for training_sample in batch:
+            pos_prompts.append(training_sample.positive_str)
+            pos_indices.append(
+                _get_token_index(
+                    training_sample.read_positive_token_index,
+                    read_token_index,
+                    training_sample.positive_str,
+                )
+            )
+            neg_prompts.append(training_sample.negative_str)
+            neg_indices.append(
+                _get_token_index(
+                    training_sample.read_negative_token_index,
+                    read_token_index,
+                    training_sample.negative_str,
+                )
+            )
         pos_acts = _extract_activations(
             model,
             tokenizer,
-            training_sample.positive_str,
+            pos_prompts,
             layer_type=layer_type,
             layer_config=layer_config,
             layers=layers,
-            read_token_index=pos_index,
+            read_token_indices=pos_indices,
         )
         neg_acts = _extract_activations(
             model,
             tokenizer,
-            training_sample.negative_str,
+            neg_prompts,
             layer_type=layer_type,
             layer_config=layer_config,
             layers=layers,
-            read_token_index=neg_index,
+            read_token_indices=neg_indices,
         )
         for layer_num, pos_act in pos_acts.items():
             if move_to_cpu:
                 pos_act = pos_act.cpu()
             pos_activations[layer_num].append(pos_act)
         for layer_num, neg_act in neg_acts.items():
             if move_to_cpu:
                 neg_act = neg_act.cpu()
             neg_activations[layer_num].append(neg_act)
     layer_activations = {}
     for layer_num in pos_activations.keys():
         layer_pos_acts = pos_activations[layer_num]
         layer_neg_acts = neg_activations[layer_num]
-        # TODO: allow controlling how to combine activations, not just mean
         direction_vec = aggregator(
-            torch.stack(layer_pos_acts), torch.stack(layer_neg_acts)
+            torch.concat(layer_pos_acts), torch.concat(layer_neg_acts)
         )
         layer_activations[layer_num] = direction_vec
     return SteeringVector(layer_activations, layer_type)
 
 
+def _formalize_batch(
+    batch: Sequence[SteeringVectorTrainingSample | tuple[str, str]]
+) -> list[SteeringVectorTrainingSample]:
+    return [_formalize_sample(sample) for sample in batch]
+
+
+def _formalize_sample(
+    sample: SteeringVectorTrainingSample | tuple[str, str]
+) -> SteeringVectorTrainingSample:
+    if isinstance(sample, tuple):
+        return SteeringVectorTrainingSample(sample[0], sample[1])
+    else:
+        return sample
+
+
 def _extract_activations(
     model: nn.Module,
     tokenizer: PreTrainedTokenizerBase,
-    prompt: str,
+    prompts: Sequence[str],
     layer_type: LayerType,
     layer_config: ModelLayerConfig,
     layers: list[int] | None,
-    read_token_index: int,
+    read_token_indices: Sequence[int],
 ) -> dict[int, Tensor]:
-    input = tokenizer(prompt, return_tensors="pt").to(model.device)
+    input = tokenizer(prompts, return_tensors="pt", padding=True)
+    adjusted_read_indices = adjust_read_indices_for_padding(
+        torch.tensor(read_token_indices), input["attention_mask"]
+    ).to(model.device)
+    batch_indices = torch.arange(len(prompts))
     results = {}
     with record_activations(
         model, layer_type, layer_config, layer_nums=layers
     ) as record:
-        model(**input)
+        model(**input.to(model.device))
     for layer_num, activation in record.items():
-        results[layer_num] = activation[-1][0, read_token_index].detach()
+        results[layer_num] = activation[-1][
+            batch_indices, adjusted_read_indices
+        ].detach()
     return results
 
 
 def _get_token_index(
     custom_idx: int | None, default_idx: int | Callable[[str], int], prompt: str
 ) -> int:
     if custom_idx is None:
```

### Comparing `steering_vectors-0.8.0/PKG-INFO` & `steering_vectors-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: steering-vectors
-Version: 0.8.0
+Version: 0.9.0
 Summary: Steering vectors for transformer language models in Pytorch / Huggingface
 License: MIT
 Author: David Chanin
 Author-email: chanindav@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

