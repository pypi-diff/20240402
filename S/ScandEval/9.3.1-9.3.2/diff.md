# Comparing `tmp/scandeval-9.3.1.tar.gz` & `tmp/scandeval-9.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scandeval-9.3.1.tar", max compression
+gzip compressed data, was "scandeval-9.3.2.tar", max compression
```

## Comparing `scandeval-9.3.1.tar` & `scandeval-9.3.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     1082 2024-01-26 19:59:00.103475 scandeval-9.3.1/LICENSE
--rw-r--r--   0        0        0     4117 2024-01-26 19:59:00.104028 scandeval-9.3.1/README.md
--rw-r--r--   0        0        0     2641 2024-01-31 08:13:46.958928 scandeval-9.3.1/pyproject.toml
--rw-r--r--   0        0        0     1091 2024-01-26 19:59:00.106909 scandeval-9.3.1/src/scandeval/__init__.py
--rw-r--r--   0        0        0     9070 2024-01-26 19:59:00.107321 scandeval-9.3.1/src/scandeval/benchmark_config_factory.py
--rw-r--r--   0        0        0    25652 2024-01-29 18:04:03.570978 scandeval-9.3.1/src/scandeval/benchmark_dataset.py
--rw-r--r--   0        0        0    21917 2024-01-29 18:04:03.571277 scandeval-9.3.1/src/scandeval/benchmarker.py
--rw-r--r--   0        0        0     1818 2024-01-26 19:59:00.108090 scandeval-9.3.1/src/scandeval/callbacks.py
--rw-r--r--   0        0        0     8565 2024-01-26 19:59:00.108521 scandeval-9.3.1/src/scandeval/cli.py
--rw-r--r--   0        0        0     7882 2024-01-26 19:59:00.108889 scandeval-9.3.1/src/scandeval/config.py
--rw-r--r--   0        0        0    32847 2024-01-29 18:04:03.571534 scandeval-9.3.1/src/scandeval/dataset_configs.py
--rw-r--r--   0        0        0     1902 2024-01-26 19:59:00.109402 scandeval-9.3.1/src/scandeval/dataset_factory.py
--rw-r--r--   0        0        0     5534 2024-01-26 19:59:00.110106 scandeval-9.3.1/src/scandeval/dataset_tasks.py
--rw-r--r--   0        0        0     1602 2024-01-26 19:59:00.110238 scandeval-9.3.1/src/scandeval/enums.py
--rw-r--r--   0        0        0     2284 2024-01-26 19:59:00.110349 scandeval-9.3.1/src/scandeval/exceptions.py
--rw-r--r--   0        0        0    15163 2024-01-29 18:04:03.571764 scandeval-9.3.1/src/scandeval/finetuning.py
--rw-r--r--   0        0        0    21097 2024-01-29 18:04:03.571916 scandeval-9.3.1/src/scandeval/generation.py
--rw-r--r--   0        0        0     7904 2024-01-06 11:42:03.776659 scandeval-9.3.1/src/scandeval/languages.py
--rw-r--r--   0        0        0    10030 2024-01-29 18:04:03.572388 scandeval-9.3.1/src/scandeval/model_cache.py
--rw-r--r--   0        0        0      878 2024-01-06 11:43:21.383149 scandeval-9.3.1/src/scandeval/model_config.py
--rw-r--r--   0        0        0     2047 2024-01-26 19:59:00.111566 scandeval-9.3.1/src/scandeval/model_loading.py
--rw-r--r--   0        0        0      516 2023-12-04 12:41:34.553463 scandeval-9.3.1/src/scandeval/model_setups/__init__.py
--rw-r--r--   0        0        0     6092 2024-01-29 18:04:03.572598 scandeval-9.3.1/src/scandeval/model_setups/fresh.py
--rw-r--r--   0        0        0    21586 2024-01-29 18:04:03.572720 scandeval-9.3.1/src/scandeval/model_setups/hf.py
--rw-r--r--   0        0        0     4515 2024-01-29 18:04:03.572869 scandeval-9.3.1/src/scandeval/model_setups/local.py
--rw-r--r--   0        0        0     7705 2024-01-29 18:04:03.573015 scandeval-9.3.1/src/scandeval/model_setups/openai.py
--rw-r--r--   0        0        0     7556 2024-01-29 18:04:03.573159 scandeval-9.3.1/src/scandeval/model_setups/utils.py
--rw-r--r--   0        0        0    27085 2024-01-29 18:04:03.573288 scandeval-9.3.1/src/scandeval/named_entity_recognition.py
--rw-r--r--   0        0        0    14203 2024-01-29 18:04:03.573607 scandeval-9.3.1/src/scandeval/openai_models.py
--rw-r--r--   0        0        0     5793 2024-01-29 18:04:03.573957 scandeval-9.3.1/src/scandeval/protocols.py
--rw-r--r--   0        0        0    22466 2024-01-29 18:04:03.574279 scandeval-9.3.1/src/scandeval/question_answering.py
--rw-r--r--   0        0        0    12206 2024-01-26 19:59:00.115561 scandeval-9.3.1/src/scandeval/question_answering_trainer.py
--rw-r--r--   0        0        0     4842 2024-01-29 18:04:03.574541 scandeval-9.3.1/src/scandeval/scores.py
--rw-r--r--   0        0        0    14984 2024-01-29 18:04:03.574705 scandeval-9.3.1/src/scandeval/sequence_classification.py
--rw-r--r--   0        0        0     5965 2024-01-06 11:52:34.791523 scandeval-9.3.1/src/scandeval/speed_benchmark.py
--rw-r--r--   0        0        0     8108 2024-01-29 18:04:03.575019 scandeval-9.3.1/src/scandeval/text_to_text.py
--rw-r--r--   0        0        0     1290 2024-01-26 19:59:00.116613 scandeval-9.3.1/src/scandeval/types.py
--rw-r--r--   0        0        0    21929 2024-01-31 08:13:06.204165 scandeval-9.3.1/src/scandeval/utils.py
--rw-r--r--   0        0        0    13707 2024-01-29 18:04:03.575319 scandeval-9.3.1/src/scandeval/vllm_models.py
--rw-r--r--   0        0        0     6225 1970-01-01 00:00:00.000000 scandeval-9.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1082 2024-01-26 19:59:00.103475 scandeval-9.3.2/LICENSE
+-rw-r--r--   0        0        0     4122 2024-02-05 10:27:47.048683 scandeval-9.3.2/README.md
+-rw-r--r--   0        0        0     2776 2024-02-05 10:28:02.896179 scandeval-9.3.2/pyproject.toml
+-rw-r--r--   0        0        0     1091 2024-01-26 19:59:00.106909 scandeval-9.3.2/src/scandeval/__init__.py
+-rw-r--r--   0        0        0     9047 2024-02-05 10:27:47.051288 scandeval-9.3.2/src/scandeval/benchmark_config_factory.py
+-rw-r--r--   0        0        0    25617 2024-02-05 10:27:47.051442 scandeval-9.3.2/src/scandeval/benchmark_dataset.py
+-rw-r--r--   0        0        0    21963 2024-02-05 10:27:47.051912 scandeval-9.3.2/src/scandeval/benchmarker.py
+-rw-r--r--   0        0        0     1818 2024-01-26 19:59:00.108090 scandeval-9.3.2/src/scandeval/callbacks.py
+-rw-r--r--   0        0        0     8565 2024-01-26 19:59:00.108521 scandeval-9.3.2/src/scandeval/cli.py
+-rw-r--r--   0        0        0     7882 2024-01-26 19:59:00.108889 scandeval-9.3.2/src/scandeval/config.py
+-rw-r--r--   0        0        0    32847 2024-02-03 12:27:34.347337 scandeval-9.3.2/src/scandeval/dataset_configs.py
+-rw-r--r--   0        0        0     1902 2024-01-26 19:59:00.109402 scandeval-9.3.2/src/scandeval/dataset_factory.py
+-rw-r--r--   0        0        0     5533 2024-02-05 10:27:47.052139 scandeval-9.3.2/src/scandeval/dataset_tasks.py
+-rw-r--r--   0        0        0     1602 2024-01-26 19:59:00.110238 scandeval-9.3.2/src/scandeval/enums.py
+-rw-r--r--   0        0        0     2284 2024-01-26 19:59:00.110349 scandeval-9.3.2/src/scandeval/exceptions.py
+-rw-r--r--   0        0        0    15130 2024-02-05 10:27:47.052325 scandeval-9.3.2/src/scandeval/finetuning.py
+-rw-r--r--   0        0        0    21037 2024-02-05 10:27:47.052463 scandeval-9.3.2/src/scandeval/generation.py
+-rw-r--r--   0        0        0     7904 2024-01-06 11:42:03.776659 scandeval-9.3.2/src/scandeval/languages.py
+-rw-r--r--   0        0        0     9970 2024-02-05 10:27:47.052633 scandeval-9.3.2/src/scandeval/model_cache.py
+-rw-r--r--   0        0        0      878 2024-01-06 11:43:21.383149 scandeval-9.3.2/src/scandeval/model_config.py
+-rw-r--r--   0        0        0     2047 2024-01-26 19:59:00.111566 scandeval-9.3.2/src/scandeval/model_loading.py
+-rw-r--r--   0        0        0      516 2023-12-04 12:41:34.553463 scandeval-9.3.2/src/scandeval/model_setups/__init__.py
+-rw-r--r--   0        0        0     6041 2024-02-05 10:27:47.052860 scandeval-9.3.2/src/scandeval/model_setups/fresh.py
+-rw-r--r--   0        0        0    21548 2024-02-05 10:27:47.053000 scandeval-9.3.2/src/scandeval/model_setups/hf.py
+-rw-r--r--   0        0        0     4462 2024-02-05 10:27:47.053249 scandeval-9.3.2/src/scandeval/model_setups/local.py
+-rw-r--r--   0        0        0     7652 2024-02-05 10:27:47.053457 scandeval-9.3.2/src/scandeval/model_setups/openai.py
+-rw-r--r--   0        0        0     7556 2024-01-29 18:04:03.573159 scandeval-9.3.2/src/scandeval/model_setups/utils.py
+-rw-r--r--   0        0        0    26855 2024-02-05 10:27:47.053605 scandeval-9.3.2/src/scandeval/named_entity_recognition.py
+-rw-r--r--   0        0        0    14140 2024-02-05 10:27:47.053816 scandeval-9.3.2/src/scandeval/openai_models.py
+-rw-r--r--   0        0        0     5793 2024-01-29 18:04:03.573957 scandeval-9.3.2/src/scandeval/protocols.py
+-rw-r--r--   0        0        0    22368 2024-02-05 10:27:47.053959 scandeval-9.3.2/src/scandeval/question_answering.py
+-rw-r--r--   0        0        0    12168 2024-02-05 10:27:47.054139 scandeval-9.3.2/src/scandeval/question_answering_trainer.py
+-rw-r--r--   0        0        0     4842 2024-01-29 18:04:03.574541 scandeval-9.3.2/src/scandeval/scores.py
+-rw-r--r--   0        0        0    14925 2024-02-05 10:27:47.054319 scandeval-9.3.2/src/scandeval/sequence_classification.py
+-rw-r--r--   0        0        0     5886 2024-02-05 10:27:47.054526 scandeval-9.3.2/src/scandeval/speed_benchmark.py
+-rw-r--r--   0        0        0     8000 2024-02-05 10:27:47.054742 scandeval-9.3.2/src/scandeval/text_to_text.py
+-rw-r--r--   0        0        0     1290 2024-01-26 19:59:00.116613 scandeval-9.3.2/src/scandeval/types.py
+-rw-r--r--   0        0        0    21940 2024-02-05 10:27:47.054893 scandeval-9.3.2/src/scandeval/utils.py
+-rw-r--r--   0        0        0    14785 2024-02-05 10:27:47.055287 scandeval-9.3.2/src/scandeval/vllm_models.py
+-rw-r--r--   0        0        0     6223 1970-01-01 00:00:00.000000 scandeval-9.3.2/PKG-INFO
```

### Comparing `scandeval-9.3.1/LICENSE` & `scandeval-9.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scandeval-9.3.1/README.md` & `scandeval-9.3.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ### Evaluation of pretrained language models on mono- or multilingual language tasks.
 
 ______________________________________________________________________
 [![PyPI Status](https://badge.fury.io/py/scandeval.svg)](https://pypi.org/project/scandeval/)
 [![Paper](https://img.shields.io/badge/arXiv-2304.00906-b31b1b.svg)](https://arxiv.org/abs/2304.00906)
 [![License](https://img.shields.io/github/license/ScandEval/ScandEval)](https://github.com/ScandEval/ScandEval/blob/main/LICENSE)
 [![LastCommit](https://img.shields.io/github/last-commit/ScandEval/ScandEval)](https://github.com/ScandEval/ScandEval/commits/main)
-[![Code Coverage](https://img.shields.io/badge/Coverage-74%25-yellow.svg)](https://github.com/ScandEval/ScandEval/tree/main/tests)
+[![Code Coverage](https://img.shields.io/badge/Coverage-76%25-yellowgreen.svg)](https://github.com/ScandEval/ScandEval/tree/main/tests)
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.0-4baaaa.svg)](https://github.com/ScandEval/ScandEval/blob/main/CODE_OF_CONDUCT.md)
 
 
 ## Maintainers
 
 - Dan Saattrup Nielsen (@saattrupdan, dan.nielsen@alexandra.dk)
 - Kenneth Enevoldsen (@KennethEnevoldsen, kenneth.enevoldsen@cas.au.dk)
```

### Comparing `scandeval-9.3.1/pyproject.toml` & `scandeval-9.3.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ScandEval"
-version = "9.3.1"
+version = "9.3.2"
 description = "Evaluation of pretrained language models on mono- or multilingual language tasks."
 authors = ["Dan Saattrup Nielsen <dan.nielsen@alexandra.dk>"]
 maintainers = [
     "Dan Saattrup Nielsen <dan.nielsen@alexandra.dk>",
     "Kenneth Enevoldsen <kenneth.enevoldsen@cas.au.dk>",
 ]
 readme = "README.md"
@@ -19,57 +19,56 @@
 datasets = "^2.15.0"
 click = "^8.1.3"
 termcolor = "^2.0.0"
 numpy = "^1.23.0"
 sentencepiece = ">=0.1.96,<1.0.0"
 protobuf = ">=3.20.0,<3.21.0"
 seqeval = "^1.2.2"
-pandas = "^1.4.0"
+pandas = "^2.2.0"
 python-dotenv = ">=0.20.0,<1.0.0"
 sacremoses = ">=0.0.53,<1.0.0"
 jax = ">=0.4.1,<1.0.0"
 flax = ">=0.6.3,<1.0.0"
 jaxlib = ">=0.4.1,<1.0.0"
 pyinfer = ">=0.0.3,<1.0.0"
 openai = ">=0.27.8,<1.0.0"
 tiktoken = ">=0.4.0,<1.0.0"
 levenshtein = ">=0.21.1,<1.0.0"
 einops = ">=0.6.0,<1.0.0"
-bitsandbytes = {markers="sys_platform != 'darwin' or platform_machine != 'arm64'", version = ">=0.40.0.post4,<1.0.0"}
+bitsandbytes = {markers="sys_platform != 'darwin' or platform_machine != 'arm64'", version = ">=0.42.0,<1.0.0"}
 requests = "^2.31.0"
 torch = "^2.1.1"
 transformers = "~4.37.1"  # Only minor upgrades as breaking changes happen often
 accelerate = ">=0.23.0,<1.0.0"
 rouge-score = ">=0.1.2,<1.0.0"
 bert-score = ">=0.3.13,<1.0.0"
 evaluate = ">=0.4.1,<1.0.0"
-vllm = {markers="sys_platform != 'darwin'", version = ">=0.2.7,<1.0.0"}
+vllm = {markers="sys_platform != 'darwin'", version = ">=0.3.0,<1.0.0"}
 demjson3 = "^3.0.6"
-pydantic = ">=1.10.0,<3.0.0"
+pydantic = "^2.6.0"
 lm-format-enforcer = ">=0.8.2,<1.0.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = ">=7.4.0"
 pre-commit = ">=3.3.3"
-black = ">=24.1.0"
-lxml = "^4.9.3"
+lxml = ">=4.9.3"
 pytest-cov = ">=4.1.0"
 readme-coverage-badger = ">=0.1.2"
 ruff = ">=0.1.13"
 mypy = ">=1.8.0"
 
 [tool.poetry.scripts]
 scandeval = "scandeval.cli:benchmark"
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = [
     '--verbose',
     '--durations=10',
-    '--color=yes',
+    '--color=no',
     '-s',
     '-vv',
     '--doctest-modules',
     '--cov=src/scandeval',
 ]
 xfail_strict = true
 filterwarnings = [
@@ -77,36 +76,38 @@
     "ignore::UserWarning",
     "ignore::DeprecationWarning",
     "ignore::ImportWarning",
 ]
 log_cli_level = "info"
 testpaths = ["tests", "src/scandeval"]
 
-[tool.black]
-line-length = 88
-include = '\.pyi?$'
-exclude = '''
-/(
-	\.git
-| \.hg
-| \.mypy_cache
-| \.tox
-| \.venv
-| _build
-| buck-out
-| build
-)/
-'''
-
 [tool.ruff]
-target-version = "py311"
+line-length = 88
+target-version = "py310"
 extend-select = [
     "I",
     "D",
 ]
+exclude = [
+    ".git",
+    ".mypy_cache",
+    ".pytest_cache",
+    ".ruff_cache",
+    ".scandeval_cache",
+    ".venv",
+]
+
+[tool.ruff.format]
+quote-style = "double"
+indent-style = "space"
+docstring-code-format = true
+skip-magic-trailing-comma = true
+
+[tool.ruff.isort]
+split-on-trailing-comma = false
 
 [tool.ruff.pydocstyle]
 convention = "google"
 
 [tool.ruff.extend-per-file-ignores]
 "__init__.py" = ["F401"]
```

### Comparing `scandeval-9.3.1/src/scandeval/__init__.py` & `scandeval-9.3.2/src/scandeval/__init__.py`

 * *Files identical despite different names*

### Comparing `scandeval-9.3.1/src/scandeval/benchmark_config_factory.py` & `scandeval-9.3.2/src/scandeval/benchmark_config_factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,20 +90,18 @@
             Whether to only evaluate on the validation split.
         few_shot:
             Whether to only evaluate the model using few-shot evaluation. Only relevant
             if the model is generative.
     """
     language_codes = get_correct_language_codes(language_codes=language)
     model_languages = prepare_languages(
-        language_codes=model_language,
-        default_language_codes=language_codes,
+        language_codes=model_language, default_language_codes=language_codes
     )
     dataset_languages = prepare_languages(
-        language_codes=dataset_language,
-        default_language_codes=language_codes,
+        language_codes=dataset_language, default_language_codes=language_codes
     )
 
     dataset_tasks = prepare_dataset_tasks(dataset_task=dataset_task)
 
     torch_device = prepare_device(device=device)
 
     return BenchmarkConfig(
@@ -160,16 +158,15 @@
     elif "nb" in languages or "nn" in languages:
         languages = list(set(languages) | {"no"})
 
     return languages
 
 
 def prepare_languages(
-    language_codes: str | list[str] | None,
-    default_language_codes: list[str],
+    language_codes: str | list[str] | None, default_language_codes: list[str]
 ) -> list[Language]:
     """Prepare language(s) for benchmarking.
 
     Args:
         language_codes:
             The language codes of the languages to include for models or datasets.
             If specified then this overrides the `language` parameter for model or
```

### Comparing `scandeval-9.3.1/src/scandeval/benchmark_dataset.py` & `scandeval-9.3.2/src/scandeval/benchmark_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -506,15 +506,15 @@
 
                     if benchmarking_generative_model:
                         prepared_test = prepared_test.map(
                             lambda examples: dict(
                                 text=tokenizer.batch_decode(
                                     sequences=examples["input_ids"],
                                     skip_special_tokens=True,
-                                ),
+                                )
                             ),
                             batched=True,
                             load_from_cache_file=False,
                             keep_in_memory=True,
                         )
 
                     prepared_tests.append(prepared_test)
@@ -523,17 +523,15 @@
                 raise InvalidBenchmark(
                     "Preprocessing of the test dataset could not be done."
                 )
 
         return prepared_train, prepared_val, prepared_tests
 
     def _preprocess_logits_for_metrics(
-        self,
-        model_outputs: torch.Tensor | tuple,
-        labels: torch.Tensor,
+        self, model_outputs: torch.Tensor | tuple, labels: torch.Tensor
     ) -> torch.Tensor | tuple:
         """Ensure that only the logits are returned from the model.
 
         This is to avoid memory issues when the model returns hidden states as well.
 
         Args:
             model_outputs:
@@ -628,17 +626,15 @@
         Returns:
             The data collator.
         """
         pass
 
     @abstractmethod
     def _compute_metrics(
-        self,
-        model_outputs_and_labels: tuple[Predictions, Labels],
-        id2label: list[str],
+        self, model_outputs_and_labels: tuple[Predictions, Labels], id2label: list[str]
     ) -> dict[str, float]:
         """Compute the metrics needed for evaluation.
 
         Args:
             model_outputs_and_labels:
                 The first sequence contains the model outputs and the second sequence
                 contains the true labels.
```

### Comparing `scandeval-9.3.1/src/scandeval/benchmarker.py` & `scandeval-9.3.2/src/scandeval/benchmarker.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,22 +82,30 @@
             f.write("\n" + json_str)
 
 
 class Benchmarker:
     """Benchmarking all the Scandinavian language models.
 
     Attributes:
-        progress_bar: Whether progress bars should be shown.
-        save_results: Whether to save the benchmark results.
-        language: The languages to include in the list.
-        dataset_task: The dataset tasks to include.
-        evaluate_train: Whether to evaluate the training set as well.
-        verbose: Whether to output additional output.
-        token: The authentication token for the Hugging Face Hub.
-        benchmark_results: The benchmark results.
+        progress_bar:
+            Whether progress bars should be shown.
+        save_results:
+            Whether to save the benchmark results.
+        language:
+            The languages to include in the list.
+        dataset_task:
+            The dataset tasks to include.
+        evaluate_train:
+            Whether to evaluate the training set as well.
+        verbose:
+            Whether to output additional output.
+        token:
+            The authentication token for the Hugging Face Hub.
+        benchmark_results:
+            The benchmark results.
     """
 
     def __init__(
         self,
         progress_bar: bool = True,
         save_results: bool = False,
         language: str | list[str] = ["da", "sv", "no"],
@@ -340,18 +348,15 @@
         model_cache_path.mkdir(parents=True, exist_ok=True)
         for model_dir in model_cache_path.iterdir():
             if model_dir.is_dir():
                 for sub_model_dir in model_dir.iterdir():
                     if sub_model_dir.is_dir():
                         rmtree(sub_model_dir)
 
-    def _prepare_model_ids(
-        self,
-        model_id: list[str] | str | None,
-    ) -> list[str]:
+    def _prepare_model_ids(self, model_id: list[str] | str | None) -> list[str]:
         """Prepare the model ID(s) to be benchmarked.
 
         Args:
             model_id:
                 The model ID(s) of the models to benchmark. If None then all model IDs
                 will be retrieved.
 
@@ -359,15 +364,15 @@
             The prepared list of model IDs.
         """
         model_ids: list[str]
 
         # If `model_id` is not specified, then fetch all the relevant model IDs
         if model_id is None:
             model_ids = self._get_model_ids(
-                languages=self.benchmark_config.model_languages,
+                languages=self.benchmark_config.model_languages
             )
 
         # Otherwise, if `model_id` is a string, ensure that it is a list
         elif isinstance(model_id, str):
             model_ids = [model_id]
 
         # Otherwise `model_id` is already a list, so we do nothing
@@ -384,16 +389,15 @@
         model_ids_sorted += [
             m_id for m_id in model_ids if m_id not in benchmarked_model_ids
         ]
 
         return model_ids_sorted
 
     def _prepare_dataset_configs(
-        self,
-        dataset: list[str] | str | None,
+        self, dataset: list[str] | str | None
     ) -> list[DatasetConfig]:
         """Prepare the dataset configuration(s) to be benchmarked.
 
         Args:
             dataset:
                 The datasets to benchmark on. If None then all datasets will be
                 benchmarked. Defaults to None.
@@ -504,16 +508,15 @@
         new_languages = self._model_lists is not None and any(
             lang.code not in self._model_lists for lang in languages
         )
 
         # If the model lists have not been fetched already, then do it
         if self._model_lists is None or new_languages:
             self._model_lists = get_huggingface_model_lists(
-                languages=languages,
-                token=self.benchmark_config.token,
+                languages=languages, token=self.benchmark_config.token
             )
 
         # Extract all the model IDs from the model lists, for the chosen languages
         model_ids: list[str] = list()
         for language in languages:
             model_ids.extend(self._model_lists[language.code])
```

### Comparing `scandeval-9.3.1/src/scandeval/callbacks.py` & `scandeval-9.3.2/src/scandeval/callbacks.py`

 * *Files identical despite different names*

### Comparing `scandeval-9.3.1/src/scandeval/cli.py` & `scandeval-9.3.2/src/scandeval/cli.py`

 * *Files identical despite different names*

### Comparing `scandeval-9.3.1/src/scandeval/config.py` & `scandeval-9.3.2/src/scandeval/config.py`

 * *Files identical despite different names*

### Comparing `scandeval-9.3.1/src/scandeval/dataset_configs.py` & `scandeval-9.3.2/src/scandeval/dataset_configs.py`

 * *Files identical despite different names*

### Comparing `scandeval-9.3.1/src/scandeval/dataset_factory.py` & `scandeval-9.3.2/src/scandeval/dataset_factory.py`

 * *Files identical despite different names*

### Comparing `scandeval-9.3.1/src/scandeval/dataset_tasks.py` & `scandeval-9.3.2/src/scandeval/dataset_tasks.py`

 * *Files 0% similar despite different names*

```diff
@@ -179,15 +179,15 @@
     supertask="text-modelling",
     metrics=[
         MetricConfig(
             name="perplexity",
             pretty_name="Perplexity",
             huggingface_id="perplexity",
             results_key="mean_perplexity",
-        ),
+        )
     ],
     labels=[],
 )
 
 
 SPEED = DatasetTask(
     name="speed",
```

### Comparing `scandeval-9.3.1/src/scandeval/enums.py` & `scandeval-9.3.2/src/scandeval/enums.py`

 * *Files identical despite different names*

### Comparing `scandeval-9.3.1/src/scandeval/exceptions.py` & `scandeval-9.3.2/src/scandeval/exceptions.py`

 * *Files identical despite different names*

### Comparing `scandeval-9.3.1/src/scandeval/finetuning.py` & `scandeval-9.3.2/src/scandeval/finetuning.py`

 * *Files 0% similar despite different names*

```diff
@@ -339,17 +339,15 @@
                     metric_key_prefix="train",
                 )
                 train_scores = trainer.evaluate(**evaluate_inputs)
             scores["train"] = train_scores
 
         with torch.inference_mode():
             evaluate_inputs = evaluate_inputs_fn(
-                dataset=test,
-                prepared_dataset=prepared_test,
-                metric_key_prefix="test",
+                dataset=test, prepared_dataset=prepared_test, metric_key_prefix="test"
             )
             test_scores = trainer.evaluate(**evaluate_inputs)
         scores["test"] = test_scores
 
         return scores
 
     except NaNValueInModelOutput as e:
```

### Comparing `scandeval-9.3.1/src/scandeval/generation.py` & `scandeval-9.3.2/src/scandeval/generation.py`

 * *Files 2% similar despite different names*

```diff
@@ -296,22 +296,18 @@
 
         # Store the cache to disk
         cache.save()
 
     # Fetch the cached predictions for the cached examples
     if len(cached_dataset) > 0:
         model_output = load_cached_model_outputs(
-            cached_dataset=cached_dataset,
-            cache=cache,
-            tokenizer=tokenizer,
+            cached_dataset=cached_dataset, cache=cache, tokenizer=tokenizer
         )
         extracted_labels = extract_labels_fn(
-            input_batch=cached_dataset,
-            model_output=model_output,
-            tokenizer=tokenizer,
+            input_batch=cached_dataset, model_output=model_output, tokenizer=tokenizer
         )
         all_preds.extend(extracted_labels)
 
     if "label" in non_cached_dataset.column_names:
         ground_truth = [
             label.lower() if isinstance(label, str) else label
             for label in non_cached_dataset["label"] + cached_dataset["label"]
@@ -519,16 +515,15 @@
         input_batch=input_batch, model_output=model_output, tokenizer=tokenizer
     )
 
     return model_output, extracted_labels
 
 
 def extract_raw_predictions(
-    generated_sequences: torch.Tensor,
-    tokenizer: Tokenizer,
+    generated_sequences: torch.Tensor, tokenizer: Tokenizer
 ) -> list[str]:
     """Get the raw predictions from the generated sequences.
 
     Args:
         generated_sequences:
             The generated sequences from the model. The outer-most list is the
             batch dimension, the inner-most list is the sequence dimension,
@@ -545,16 +540,15 @@
         .strip()
         for completion_ids in generated_sequences.long()
     ]
     return raw_predictions
 
 
 def get_generation_stopping_criteria(
-    tokenizer: Tokenizer,
-    model: GenerativeModel,
+    tokenizer: Tokenizer, model: GenerativeModel
 ) -> StopWordCriteria:
     """Get the stopping criteria for generation.
 
     Args:
         tokenizer:
             The tokenizer used to tokenize the stop words.
         model:
```

### Comparing `scandeval-9.3.1/src/scandeval/languages.py` & `scandeval-9.3.2/src/scandeval/languages.py`

 * *Files identical despite different names*

### Comparing `scandeval-9.3.1/src/scandeval/model_cache.py` & `scandeval-9.3.2/src/scandeval/model_cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,18 +39,15 @@
         cache:
             The model output cache.
         max_generated_tokens:
             The maximum number of tokens to generate for each example.
     """
 
     def __init__(
-        self,
-        model_cache_dir: Path,
-        cache_name: str,
-        max_generated_tokens: int,
+        self, model_cache_dir: Path, cache_name: str, max_generated_tokens: int
     ):
         """Initialize the model output cache.
 
         Args:
             model_cache_dir:
                 The directory to store the cache in.
             cache_name:
@@ -116,18 +113,15 @@
         del self.cache
 
     def cached_texts(self) -> list[str]:
         """Return the text inputs indexed in the cache."""
         return [key for key in self.cache.keys()]
 
     def add_to_cache(
-        self,
-        model_input: torch.Tensor,
-        model_output: ModelOutput,
-        tokenizer: Tokenizer,
+        self, model_input: torch.Tensor, model_output: ModelOutput, tokenizer: Tokenizer
     ) -> None:
         """Add the model input/output to the cache.
 
         Args:
             model_input:
                 The model input.
             model_output:
@@ -164,15 +158,15 @@
                 )
                 generated_ids = model_output.sequences[sample_idx].tolist()
 
                 # Set up the model output in a GenerativeModelOutput object
                 cached_model_output = GenerativeModelOutput(
                     completion=tokenizer.decode(
                         token_ids=generated_ids, skip_special_tokens=True
-                    ),
+                    )
                 )
                 if store_scores:
                     cached_model_output.top_score_indices = top_scores.indices[
                         sample_idx
                     ].tolist()
                     cached_model_output.top_score_values = top_scores.values[
                         sample_idx
@@ -212,17 +206,15 @@
 
     cached = dataset.select(cached_ids)
     non_cached = dataset.select(unique_non_cached_ids)
     return cached, non_cached
 
 
 def load_cached_model_outputs(
-    cached_dataset: Dataset,
-    cache: ModelCache,
-    tokenizer: Tokenizer,
+    cached_dataset: Dataset, cache: ModelCache, tokenizer: Tokenizer
 ) -> ModelOutput:
     """Load the cached model outputs.
 
     Args:
         cached_dataset:
             The dataset containing the cached examples.
         cache:
```

### Comparing `scandeval-9.3.1/src/scandeval/model_config.py` & `scandeval-9.3.2/src/scandeval/model_config.py`

 * *Files identical despite different names*

### Comparing `scandeval-9.3.1/src/scandeval/model_loading.py` & `scandeval-9.3.2/src/scandeval/model_loading.py`

 * *Files identical despite different names*

### Comparing `scandeval-9.3.1/src/scandeval/model_setups/__init__.py` & `scandeval-9.3.2/src/scandeval/model_setups/__init__.py`

 * *Files identical despite different names*

### Comparing `scandeval-9.3.1/src/scandeval/model_setups/fresh.py` & `scandeval-9.3.2/src/scandeval/model_setups/fresh.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,32 +21,26 @@
 from ..config import BenchmarkConfig, DatasetConfig, ModelConfig
 from ..enums import Framework, ModelType
 from ..exceptions import InvalidBenchmark
 from ..protocols import GenerativeModel, Tokenizer
 from ..utils import block_terminal_output, create_model_cache_dir
 from .utils import align_model_and_tokenizer, setup_model_for_question_answering
 
-FRESH_MODELS: list[str] = [
-    "electra-small",
-    "xlm-roberta-base",
-]
+FRESH_MODELS: list[str] = ["electra-small", "xlm-roberta-base"]
 
 
 class FreshModelSetup:
     """Model setup for fresh models.
 
     Attributes:
         benchmark_config:
             The benchmark configuration.
     """
 
-    def __init__(
-        self,
-        benchmark_config: BenchmarkConfig,
-    ) -> None:
+    def __init__(self, benchmark_config: BenchmarkConfig) -> None:
         """Initialize the FreshModelSetup class.
 
         Args:
             benchmark_config:
                 The benchmark configuration.
         """
         self.benchmark_config = benchmark_config
@@ -81,16 +75,15 @@
             model_id=self._strip_model_id(model_id=model_id),
             framework=Framework.PYTORCH,
             task="fill-mask",
             languages=list(),
             revision="main",
             model_type=ModelType.FRESH,
             model_cache_dir=create_model_cache_dir(
-                cache_dir=self.benchmark_config.cache_dir,
-                model_id=model_id,
+                cache_dir=self.benchmark_config.cache_dir, model_id=model_id
             ),
         )
 
     def load_model(
         self, model_config: ModelConfig, dataset_config: DatasetConfig
     ) -> tuple[Tokenizer, PreTrainedModel | GenerativeModel]:
         """Load a fresh model.
```

### Comparing `scandeval-9.3.1/src/scandeval/model_setups/hf.py` & `scandeval-9.3.2/src/scandeval/model_setups/hf.py`

 * *Files 3% similar despite different names*

```diff
@@ -175,16 +175,15 @@
                 task=model_task,
                 languages=[
                     language_mapping[tag] for tag in tags if tag in language_codes
                 ],
                 revision=revision,
                 model_type=ModelType.HF,
                 model_cache_dir=create_model_cache_dir(
-                    cache_dir=self.benchmark_config.cache_dir,
-                    model_id=model_id,
+                    cache_dir=self.benchmark_config.cache_dir, model_id=model_id
                 ),
             )
 
         # If fetching from the Hugging Face Hub failed then throw a reasonable
         # exception
         except RequestException:
             if internet_connection_available():
@@ -487,17 +486,15 @@
                 )
             except (TimeoutError, RequestError):
                 logger.info(f"Couldn't load model config for {model_id!r}. Retrying.")
                 sleep(5)
                 continue
 
     def _load_tokenizer(
-        self,
-        model: PreTrainedModel | GenerativeModel,
-        model_id: str,
+        self, model: PreTrainedModel | GenerativeModel, model_id: str
     ) -> Tokenizer:
         """Load the tokenizer.
 
         Args:
             model (PreTrainedModel or GenerativeModel):
                 The model, which is used to determine whether to add a prefix space to
                 the tokens.
```

### Comparing `scandeval-9.3.1/src/scandeval/model_setups/local.py` & `scandeval-9.3.2/src/scandeval/model_setups/local.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,18 +19,15 @@
     """Model setup for local Hugging Face Hub models.
 
     Attributes:
         benchmark_config:
             The benchmark configuration.
     """
 
-    def __init__(
-        self,
-        benchmark_config: BenchmarkConfig,
-    ) -> None:
+    def __init__(self, benchmark_config: BenchmarkConfig) -> None:
         """Initialize the LocalModelSetup class.
 
         Args:
             benchmark_config:
                 The benchmark configuration.
         """
         self.benchmark_config = benchmark_config
@@ -113,16 +110,15 @@
             model_id=model_id,
             revision="main",
             framework=framework,
             task=task,
             languages=list(),
             model_type=ModelType.LOCAL,
             model_cache_dir=create_model_cache_dir(
-                cache_dir=self.benchmark_config.cache_dir,
-                model_id=model_id,
+                cache_dir=self.benchmark_config.cache_dir, model_id=model_id
             ),
         )
         return model_config
 
     def load_model(
         self, model_config: ModelConfig, dataset_config: DatasetConfig
     ) -> tuple[Tokenizer, PreTrainedModel | GenerativeModel]:
@@ -135,10 +131,9 @@
                 The dataset configuration.
 
         Returns:
             The tokenizer and model.
         """
         hf_model_setup = HFModelSetup(benchmark_config=self.benchmark_config)
         return hf_model_setup.load_model(
-            model_config=model_config,
-            dataset_config=dataset_config,
+            model_config=model_config, dataset_config=dataset_config
         )
```

### Comparing `scandeval-9.3.1/src/scandeval/model_setups/openai.py` & `scandeval-9.3.2/src/scandeval/model_setups/openai.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,18 +62,15 @@
     """Model setup for OpenAI models.
 
     Attributes:
         benchmark_config:
             The benchmark configuration.
     """
 
-    def __init__(
-        self,
-        benchmark_config: BenchmarkConfig,
-    ) -> None:
+    def __init__(self, benchmark_config: BenchmarkConfig) -> None:
         """Initialize the model setup.
 
         Args:
             benchmark_config:
                 The benchmark configuration.
         """
         self.benchmark_config = benchmark_config
@@ -134,16 +131,15 @@
             model_id=model_id,
             revision="main",
             framework=Framework.API,
             task="text-generation",
             languages=list(),
             model_type=ModelType.OPENAI,
             model_cache_dir=create_model_cache_dir(
-                cache_dir=self.benchmark_config.cache_dir,
-                model_id=model_id,
+                cache_dir=self.benchmark_config.cache_dir, model_id=model_id
             ),
         )
 
     def load_model(
         self, model_config: ModelConfig, dataset_config: DatasetConfig
     ) -> tuple[Tokenizer, PreTrainedModel | GenerativeModel]:
         """Load an OpenAI model.
@@ -200,16 +196,15 @@
                 pass
         else:
             raise ValueError(
                 f"Couldn't find vocab size for the model {model_config.model_id!r}"
             )
 
         tokenizer = OpenAITokenizer(
-            model_config=model_config,
-            hf_model_config=hf_model_config,
+            model_config=model_config, hf_model_config=hf_model_config
         )
         model = OpenAIModel(
             model_config=model_config,
             hf_model_config=hf_model_config,
             benchmark_config=self.benchmark_config,
             tokenizer=tokenizer,
         )
```

### Comparing `scandeval-9.3.1/src/scandeval/model_setups/utils.py` & `scandeval-9.3.2/src/scandeval/model_setups/utils.py`

 * *Files identical despite different names*

### Comparing `scandeval-9.3.1/src/scandeval/named_entity_recognition.py` & `scandeval-9.3.2/src/scandeval/named_entity_recognition.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,17 +63,15 @@
             tag for tag_list in dataset_dict["train"]["labels"] for tag in tag_list
         }
         self.has_misc_tags = "B-MISC" in labels_in_train or "I-MISC" in labels_in_train
 
         return dataset_dict
 
     def _compute_metrics(
-        self,
-        model_outputs_and_labels: tuple[Predictions, Labels],
-        id2label: list[str],
+        self, model_outputs_and_labels: tuple[Predictions, Labels], id2label: list[str]
     ) -> dict[str, float]:
         """Compute the metrics needed for evaluation.
 
         Args:
             model_outputs_and_labels:
                 The first array contains the probability predictions and the second
                 array contains the true labels.
@@ -218,18 +216,15 @@
 
         Returns:
             A dictionary containing the tokenized data as well as labels.
         """
         # Tokenize the texts. We use the `is_split_into_words` argument here because
         # the texts in our dataset are lists of words (with a label for each word)
         tokenized_inputs = tokenizer(
-            examples["tokens"],
-            is_split_into_words=True,
-            truncation=True,
-            padding=True,
+            examples["tokens"], is_split_into_words=True, truncation=True, padding=True
         )
 
         # Extract a mapping between all the tokens and their corresponding word. If the
         # tokenizer is of a "fast" variant then this can be accessed through the
         # `word_ids` method. Otherwise, we have to extract it manually.
         all_labels: list[list[int]] = list()
         labels: list[str]
@@ -258,17 +253,15 @@
                     if tok:
                         for prefix in prefixes_to_remove:
                             if tok.startswith(prefix):
                                 tokens[tok_idx] = tok[len(prefix) :]
 
                 # Replace UNK tokens with the correct word
                 tokens = self._handle_unk_tokens(
-                    tokenizer=tokenizer,
-                    tokens=tokens,
-                    words=words,
+                    tokenizer=tokenizer, tokens=tokens, words=words
                 )
 
                 # Get list of special tokens. Some tokenizers do not record these
                 # properly, which is why we convert the values to their indices and
                 # then back to strings
                 sp_toks = [
                     tokenizer.convert_ids_to_tokens(
@@ -427,37 +420,29 @@
                     batched=True,
                     load_from_cache_file=False,
                     keep_in_memory=True,
                 )
 
             def tokenise(examples: dict) -> BatchEncoding:
                 return kwargs["tokenizer"](
-                    text=examples["text"],
-                    truncation=True,
-                    padding=False,
+                    text=examples["text"], truncation=True, padding=False
                 )
 
             tokenised_dataset = dataset.map(
-                tokenise,
-                batched=True,
-                load_from_cache_file=False,
-                keep_in_memory=True,
+                tokenise, batched=True, load_from_cache_file=False, keep_in_memory=True
             )
 
         else:
             map_fn = partial(
                 self._tokenize_and_align_labels,
                 tokenizer=kwargs["tokenizer"],
                 label2id=kwargs["hf_model_config"].label2id,
             )
             tokenised_dataset = dataset.map(
-                map_fn,
-                batched=True,
-                load_from_cache_file=False,
-                keep_in_memory=True,
+                map_fn, batched=True, load_from_cache_file=False, keep_in_memory=True
             )
 
         return tokenised_dataset
 
     def _load_data_collator(
         self,
         tokenizer: Tokenizer | None = None,
@@ -546,15 +531,15 @@
 
         Returns:
             The examples with the few-shot prompt applied.
         """
 
         def create_label(example: dict) -> str:
             labels: dict[str, list[str]] = {
-                prompt_label: []
+                prompt_label: list()
                 for prompt_label in self.dataset_config.prompt_label_mapping.values()
             }
             for token, label in zip(example["tokens"], example["labels"]):
                 label = label.lower()
                 if label == "o":
                     continue
                 prompt_label = self.dataset_config.prompt_label_mapping[label]
```

### Comparing `scandeval-9.3.1/src/scandeval/openai_models.py` & `scandeval-9.3.2/src/scandeval/openai_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -402,19 +402,15 @@
         generation_kwargs = dict(
             model=model_id,
             max_tokens=max_tokens,
             temperature=temperature,
             top_p=generation_config.top_p,
             n=generation_config.num_return_sequences,
             frequency_penalty=generation_config.repetition_penalty - 1.0,
-            stop=[
-                "\n\n",
-                self.tokenizer.eos_token,
-                self.tokenizer.pad_token,
-            ],
+            stop=["\n\n", self.tokenizer.eos_token, self.tokenizer.pad_token],
         )
 
         for _ in range(60):
             try:
                 if not self.is_chat_model:
                     model_output = openai.Completion.create(
                         prompt=prompt, **generation_kwargs
```

### Comparing `scandeval-9.3.1/src/scandeval/protocols.py` & `scandeval-9.3.2/src/scandeval/protocols.py`

 * *Files identical despite different names*

### Comparing `scandeval-9.3.1/src/scandeval/question_answering.py` & `scandeval-9.3.2/src/scandeval/question_answering.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,16 +59,15 @@
         if not tokenizer.is_fast and not generative_model:
             raise InvalidBenchmark(
                 "Question-answering benchmarks require a fast tokenizer."
             )
 
         if generative_model:
             preprocess_fn = partial(
-                prepare_examples_for_generation,
-                tokenizer=tokenizer,
+                prepare_examples_for_generation, tokenizer=tokenizer
             )
         elif split == "test":
             preprocess_fn = partial(prepare_test_examples, tokenizer=tokenizer)
         else:
             preprocess_fn = partial(prepare_train_examples, tokenizer=tokenizer)
 
         # Preprocess the data and return it
@@ -91,16 +90,15 @@
         except NotImplementedError as e:
             raise InvalidBenchmark(str(e))
 
         # The Trainer hides the columns that are not used by the model (here `id` and
         # `offset_mapping` which we will need for our post-processing), so we put them
         # back
         preprocessed.set_format(
-            type=preprocessed.format["type"],
-            columns=list(preprocessed.features.keys()),
+            type=preprocessed.format["type"], columns=list(preprocessed.features.keys())
         )
 
         # Return the preprocessed dataset
         return preprocessed
 
     def _get_trainer_class(self) -> Type[Trainer]:
         return QuestionAnsweringTrainer
@@ -131,17 +129,15 @@
 
         Returns:
             The data collator.
         """
         return DataCollatorWithPadding(tokenizer=tokenizer)
 
     def _compute_metrics(
-        self,
-        model_outputs_and_labels: tuple[Predictions, Labels],
-        id2label: list[str],
+        self, model_outputs_and_labels: tuple[Predictions, Labels], id2label: list[str]
     ) -> dict[str, float]:
         """Compute the metrics needed for evaluation.
 
         Args:
             model_outputs_and_labels:
                 The first sequence contains the model outputs and the second sequence
                 contains the true labels.
@@ -162,17 +158,15 @@
         else:
             predictions = model_outputs
 
         results: dict[str, float] = dict()
         for cfg in self.dataset_config.task.metrics:
             metric = self._metrics[cfg.name]
             score_dict: dict[str, float] | None = metric.compute(
-                predictions=predictions,
-                references=labels,
-                **cfg.compute_kwargs,
+                predictions=predictions, references=labels, **cfg.compute_kwargs
             )
 
             # The metric returns None if we are running on multi-GPU and the current
             # process is not the main process
             if score_dict is not None:
                 scores = score_dict[cfg.results_key]
                 if isinstance(scores, list):
@@ -288,16 +282,15 @@
             tokenizer:
                 The tokenizer used together with the model.
 
         Returns:
             The predicted labels.
         """
         raw_predictions = extract_raw_predictions(
-            generated_sequences=model_output["sequences"],
-            tokenizer=tokenizer,
+            generated_sequences=model_output["sequences"], tokenizer=tokenizer
         )
 
         predictions = [
             dict(
                 id=id,
                 prediction_text=predicted_answer.lower(),
                 no_answer_probability=0.0,
@@ -457,16 +450,15 @@
                 tokenized_examples.end_positions.append(token_end_index)
                 assert token_end_index >= token_start_index
 
     return tokenized_examples
 
 
 def prepare_test_examples(
-    examples: BatchEncoding,
-    tokenizer: Tokenizer,
+    examples: BatchEncoding, tokenizer: Tokenizer
 ) -> BatchEncoding:
     """Prepare test examples.
 
     Args:
         examples:
             Dictionary of test examples.
         tokenizer:
```

### Comparing `scandeval-9.3.1/src/scandeval/question_answering_trainer.py` & `scandeval-9.3.2/src/scandeval/question_answering_trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,18 +94,15 @@
             self.control,  # type: ignore[has-type]
             output.metrics,
         )
         return output.metrics
 
 
 def postprocess_predictions_and_labels(
-    predictions: list,
-    dataset: Dataset,
-    prepared_dataset: Dataset,
-    cls_token_index: int,
+    predictions: list, dataset: Dataset, prepared_dataset: Dataset, cls_token_index: int
 ) -> tuple[list[dict], list[dict]]:
     """Postprocess the predictions and labels, to allow easier metric computation.
 
     Args:
         predictions:
             A pair of (start_logits, end_logits) predictions.
         dataset:
@@ -148,17 +145,15 @@
             min_null_score=0.0,
             cls_token_index=cls_token_index,
         )
 
         # Create the final prediction dictionary, to be added to the list of
         # predictions
         prediction = dict(
-            id=example["id"],
-            prediction_text=best_answer,
-            no_answer_probability=0.0,
+            id=example["id"], prediction_text=best_answer, no_answer_probability=0.0
         )
 
         # Add the answer to the list of predictions
         predictions.append(prediction)
 
         # Create the associated reference dictionary, to be added to the list of
         # references
```

### Comparing `scandeval-9.3.1/src/scandeval/scores.py` & `scandeval-9.3.2/src/scandeval/scores.py`

 * *Files identical despite different names*

### Comparing `scandeval-9.3.1/src/scandeval/sequence_classification.py` & `scandeval-9.3.2/src/scandeval/sequence_classification.py`

 * *Files 4% similar despite different names*

```diff
@@ -129,17 +129,15 @@
 
         Returns:
             The data collator.
         """
         return DataCollatorWithPadding(tokenizer, padding="longest")
 
     def _compute_metrics(
-        self,
-        model_outputs_and_labels: tuple[Predictions, Labels],
-        id2label: list[str],
+        self, model_outputs_and_labels: tuple[Predictions, Labels], id2label: list[str]
     ) -> dict[str, float]:
         """Compute the metrics needed for evaluation.
 
         Args:
             model_outputs_and_labels:
                 The first sequence contains the model outputs and the second sequence
                 contains the true labels.
@@ -178,17 +176,15 @@
             for label in labels
         ]
 
         results: dict[str, float] = dict()
         for cfg in self.dataset_config.task.metrics:
             metric = self._metrics[cfg.name]
             score_dict: dict[str, float] | None = metric.compute(
-                predictions=predictions,
-                references=labels,
-                **cfg.compute_kwargs,
+                predictions=predictions, references=labels, **cfg.compute_kwargs
             )
 
             # The metric returns None if we are running on multi-GPU and the current
             # process is not the main process
             if score_dict is not None:
                 scores = score_dict[cfg.results_key]
                 if isinstance(scores, list):
@@ -395,16 +391,15 @@
         dataset_config:
             The configuration of the dataset.
 
     Returns:
         The candidate labels with the smallest edit distance to the predicted labels.
     """
     raw_predictions = extract_raw_predictions(
-        generated_sequences=generated_sequences,
-        tokenizer=tokenizer,
+        generated_sequences=generated_sequences, tokenizer=tokenizer
     )
 
     candidate_labels = [
         dataset_config.prompt_label_mapping[lbl] for lbl in dataset_config.id2label
     ]
     new_predicted_labels: list[str] = list()
     for predicted_label in raw_predictions:
```

### Comparing `scandeval-9.3.1/src/scandeval/speed_benchmark.py` & `scandeval-9.3.2/src/scandeval/speed_benchmark.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,20 +109,15 @@
         def predict(doc: str) -> None:
             """Function used to benchmark inference speed of the model."""
             # Raise an error if the tokenizer or model is undefined
             if tokenizer is None or model is None:
                 raise ValueError("Tokenizer and model must not be None.")
 
             # Tokenize the document
-            inputs = tokenizer(
-                doc,
-                padding=True,
-                truncation=True,
-                return_tensors="pt",
-            )
+            inputs = tokenizer(doc, padding=True, truncation=True, return_tensors="pt")
 
             inputs = {name: tensor.to(model.device) for name, tensor in inputs.items()}
 
             # Run inference with the model
             with torch.inference_mode():
                 if is_generative:
                     model.generate(
```

### Comparing `scandeval-9.3.1/src/scandeval/text_to_text.py` & `scandeval-9.3.2/src/scandeval/text_to_text.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,18 +49,15 @@
         """
         tokenizer: Tokenizer = kwargs["tokenizer"]
 
         def tokenise(examples: dict) -> BatchEncoding:
             return tokenizer(text=examples["text"], truncation=True, padding=False)
 
         tokenised = dataset.map(
-            tokenise,
-            batched=True,
-            load_from_cache_file=False,
-            keep_in_memory=True,
+            tokenise, batched=True, load_from_cache_file=False, keep_in_memory=True
         )
 
         return tokenised
 
     def _load_data_collator(
         self,
         tokenizer: Tokenizer | None = None,
@@ -78,17 +75,15 @@
 
         Returns:
             The data collator.
         """
         return DataCollatorWithPadding(tokenizer, padding="longest")
 
     def _compute_metrics(
-        self,
-        model_outputs_and_labels: tuple[Predictions, Labels],
-        id2label: list[str],
+        self, model_outputs_and_labels: tuple[Predictions, Labels], id2label: list[str]
     ) -> dict[str, float]:
         """Compute the metrics needed for evaluation.
 
         Args:
             model_outputs_and_labels:
                 The first sequence contains the model outputs and the second sequence
                 contains the true labels.
@@ -111,17 +106,15 @@
             predictions = model_outputs
 
         results: dict[str, float] = dict()
         for cfg in self.dataset_config.task.metrics:
             metric = self._metrics[cfg.name]
             with HiddenPrints():
                 score_dict: dict[str, float] | None = metric.compute(
-                    predictions=predictions,
-                    references=labels,
-                    **cfg.compute_kwargs,
+                    predictions=predictions, references=labels, **cfg.compute_kwargs
                 )
 
             # The metric returns None if we are running on multi-GPU and the current
             # process is not the main process
             if score_dict is not None:
                 scores = score_dict[cfg.results_key]
                 if isinstance(scores, list):
@@ -225,11 +218,10 @@
             tokenizer:
                 The tokenizer used together with the model.
 
         Returns:
             The predicted labels.
         """
         raw_predictions = extract_raw_predictions(
-            generated_sequences=model_output.sequences,
-            tokenizer=tokenizer,
+            generated_sequences=model_output.sequences, tokenizer=tokenizer
         )
         return raw_predictions
```

### Comparing `scandeval-9.3.1/src/scandeval/types.py` & `scandeval-9.3.2/src/scandeval/types.py`

 * *Files identical despite different names*

### Comparing `scandeval-9.3.1/src/scandeval/utils.py` & `scandeval-9.3.2/src/scandeval/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,29 +49,21 @@
 GENERATIVE_MODEL_TASKS = [
     "text-generation",
     "conversational",
     # "text2text-generation",  # TODO: Add this when we support it
 ]
 
 
-GENERATIVE_DATASET_TASKS = [
-    "knowledge",
-    "common-sense-reasoning",
-]
+GENERATIVE_DATASET_TASKS = ["knowledge", "common-sense-reasoning"]
 
 
-GENERATIVE_DATASET_SUPERTASKS = [
-    "text-to-text",
-    "text-modelling",
-]
+GENERATIVE_DATASET_SUPERTASKS = ["text-to-text", "text-modelling"]
 
 
-SUPERTASKS_USING_LOGPROBS = [
-    "sequence-classification",
-]
+SUPERTASKS_USING_LOGPROBS = ["sequence-classification"]
 
 
 def create_model_cache_dir(cache_dir: str, model_id: str) -> str:
     """Create cache directory for a model.
 
     Args:
         cache_dir:
@@ -171,14 +163,15 @@
     logging.getLogger("datasets").setLevel(logging.ERROR)
     logging.getLogger("openai").setLevel(logging.ERROR)
     logging.getLogger("torch.distributed.distributed_c10d").setLevel(logging.ERROR)
     logging.getLogger("torch.nn.parallel.distributed").setLevel(logging.ERROR)
     logging.getLogger("vllm.engine.llm_engine").setLevel(logging.ERROR)
     logging.getLogger("vllm.transformers_utils.tokenizer").setLevel(logging.ERROR)
     logging.getLogger("vllm.core.scheduler").setLevel(logging.ERROR)
+    logging.getLogger("vllm.model_executor.weight_utils").setLevel(logging.ERROR)
 
     def init_vllm_logger(name: str):
         """Dummy function to initialise vLLM loggers with the ERROR level."""
         vllm_logger = logging.getLogger(name)
         vllm_logger.setLevel(logging.ERROR)
         return vllm_logger
 
@@ -193,16 +186,15 @@
     # Disable most of the `transformers` logging
     tf_logging._default_log_level = logging.CRITICAL
     tf_logging.set_verbosity(logging.CRITICAL)
     logging.getLogger("transformers.trainer").setLevel(logging.CRITICAL)
 
 
 def get_class_by_name(
-    class_name: str | list[str],
-    module_name: str | None = None,
+    class_name: str | list[str], module_name: str | None = None
 ) -> Type | None:
     """Get a class by its name.
 
     Args:
         class_name:
             The name of the class, written in kebab-case. The corresponding class name
             must be the same, but written in PascalCase, and lying in a module with the
@@ -324,16 +316,15 @@
         sep_token=sep_token,
         has_cls_token=has_cls_token,
         has_sep_token=has_sep_token,
     )
 
 
 def get_huggingface_model_lists(
-    languages: list[Language] | None,
-    token: bool | str,
+    languages: list[Language] | None, token: bool | str
 ) -> dict[str, list[str]]:
     """Fetches up-to-date model lists from the Hugging Face Hub.
 
     Args:
         languages:
             The language codes of the language to consider. If None then the models
             will not be filtered on language.
@@ -602,18 +593,17 @@
     Args:
         dataset_config:
             The dataset configuration.
 
     Returns:
         The JSON schema parser.
     """
-    tag_names = list(set(dataset_config.prompt_label_mapping.values()))
+    tag_names = set(dataset_config.prompt_label_mapping.values())
     keys_and_their_types: dict[str, Any] = {
-        tag_name: (conlist(str, max_items=5, unique_items=True), ...)
-        for tag_name in tag_names
+        tag_name: (conlist(str, max_length=5), ...) for tag_name in tag_names
     }
     AnswerFormat = create_model("AnswerFormat", **keys_and_their_types)
     parser = JsonSchemaParser(json_schema=AnswerFormat.schema())
     return parser
 
 
 def should_prompts_be_stripped(
```

### Comparing `scandeval-9.3.1/src/scandeval/vllm_models.py` & `scandeval-9.3.2/src/scandeval/vllm_models.py`

 * *Files 6% similar despite different names*

```diff
@@ -98,22 +98,26 @@
 
             self._model = LLM(
                 model=model_config.model_id,
                 gpu_memory_utilization=0.9,
                 max_model_len=max_model_len,
                 download_dir=str(model_cache_dir),
                 trust_remote_code=trust_remote_code,
+                revision=self.model_config.revision,
+                seed=4242,
             )
             self._model._run_engine = MethodType(
                 _run_engine_with_fixed_progress_bars, self._model
             )
 
     def __del__(self) -> None:
         """Clear the GPU memory used by the model, and remove the model itself."""
         destroy_model_parallel()
+        if hasattr(self, "_model"):
+            del self._model
         clear_memory()
         del self
 
     def generate(
         self,
         inputs: torch.Tensor,
         generation_config: GenerationConfig | None = None,
@@ -261,17 +265,15 @@
             **generation_kwargs:
                 Additional generation kwargs to pass to the model.
 
         Returns:
             The generated sequences.
         """
         return self.generate(
-            inputs=inputs,
-            generation_config=generation_config,
-            **generation_kwargs,
+            inputs=inputs, generation_config=generation_config, **generation_kwargs
         )
 
     def get_logits_processors(self) -> list[Callable] | None:
         """Return the logits processors to use for structured generation."""
         logits_processors = list()
 
         # Add JSON generation constraint if we are benchmarking the NER task
@@ -310,15 +312,29 @@
         """Set the tokenizer to use for generation.
 
         Args:
             tokenizer:
                 The tokenizer to use for generation.
         """
         self.tokenizer = tokenizer
-        self._model.set_tokenizer(tokenizer)
+
+        # This sets the internal tokenizer in the vLLM model. The
+        # `LLM.llm_engine.tokenizer` is a `TokenizerGroup` object, which has a
+        # `tokenizer` attribute that is the actual tokenizer. This is a new change from
+        # `vllm` version 0.3.0, which is a breaking change since the `TokenizerGroup`
+        # doesn't have the same properties and methods as a Hugging Face
+        # `PreTrainedTokenizer` object. To resolve this, we copy all properties and
+        # methods from the `PreTrainedTokenizer` object to the `TokenizerGroup` object,
+        # unless the property or method already exists in the `TokenizerGroup` object.
+        # vLLM issue on this: https://github.com/vllm-project/vllm/issues/2713
+        self._model.llm_engine.tokenizer.tokenizer = tokenizer
+        for attr in dir(tokenizer):
+            if attr.startswith("_") or hasattr(self._model.llm_engine.tokenizer, attr):
+                continue
+            setattr(self._model.llm_engine.tokenizer, attr, getattr(tokenizer, attr))
 
     def to(self, _: torch.device) -> None:
         """Dummy method to make the model compatible with the benchmarking script."""
         pass
 
     def eval(self) -> None:
         """Dummy method to make the model compatible with the benchmarking script."""
@@ -329,17 +345,15 @@
         return []
 
 
 def _run_engine_with_fixed_progress_bars(self, use_tqdm: bool) -> list[RequestOutput]:
     if use_tqdm:
         num_requests = self.llm_engine.get_num_unfinished_requests()
         pbar = tqdm(
-            total=num_requests,
-            leave=False,
-            disable=hasattr(sys, "_called_from_test"),
+            total=num_requests, leave=False, disable=hasattr(sys, "_called_from_test")
         )
 
     # Run the engine.
     outputs: list[RequestOutput] = list()
     while self.llm_engine.has_unfinished_requests():
         step_outputs = self.llm_engine.step()
         for output in step_outputs:
```

### Comparing `scandeval-9.3.1/PKG-INFO` & `scandeval-9.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,69 +1,69 @@
 Metadata-Version: 2.1
 Name: scandeval
-Version: 9.3.1
+Version: 9.3.2
 Summary: Evaluation of pretrained language models on mono- or multilingual language tasks.
 Home-page: https://scandeval.github.io
 License: MIT
 Author: Dan Saattrup Nielsen
 Author-email: dan.nielsen@alexandra.dk
 Maintainer: Dan Saattrup Nielsen
 Maintainer-email: dan.nielsen@alexandra.dk
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: accelerate (>=0.23.0,<1.0.0)
 Requires-Dist: bert-score (>=0.3.13,<1.0.0)
-Requires-Dist: bitsandbytes (>=0.40.0.post4,<1.0.0) ; sys_platform != "darwin" or platform_machine != "arm64"
+Requires-Dist: bitsandbytes (>=0.42.0,<1.0.0) ; sys_platform != "darwin" or platform_machine != "arm64"
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: datasets (>=2.15.0,<3.0.0)
 Requires-Dist: demjson3 (>=3.0.6,<4.0.0)
 Requires-Dist: einops (>=0.6.0,<1.0.0)
 Requires-Dist: evaluate (>=0.4.1,<1.0.0)
 Requires-Dist: flax (>=0.6.3,<1.0.0)
 Requires-Dist: huggingface-hub (>=0.7.0,<1.0.0)
 Requires-Dist: jax (>=0.4.1,<1.0.0)
 Requires-Dist: jaxlib (>=0.4.1,<1.0.0)
 Requires-Dist: levenshtein (>=0.21.1,<1.0.0)
 Requires-Dist: lm-format-enforcer (>=0.8.2,<1.0.0)
 Requires-Dist: numpy (>=1.23.0,<2.0.0)
 Requires-Dist: openai (>=0.27.8,<1.0.0)
-Requires-Dist: pandas (>=1.4.0,<2.0.0)
+Requires-Dist: pandas (>=2.2.0,<3.0.0)
 Requires-Dist: protobuf (>=3.20.0,<3.21.0)
-Requires-Dist: pydantic (>=1.10.0,<3.0.0)
+Requires-Dist: pydantic (>=2.6.0,<3.0.0)
 Requires-Dist: pyinfer (>=0.0.3,<1.0.0)
 Requires-Dist: python-dotenv (>=0.20.0,<1.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: rouge-score (>=0.1.2,<1.0.0)
 Requires-Dist: sacremoses (>=0.0.53,<1.0.0)
 Requires-Dist: sentencepiece (>=0.1.96,<1.0.0)
 Requires-Dist: seqeval (>=1.2.2,<2.0.0)
 Requires-Dist: termcolor (>=2.0.0,<3.0.0)
 Requires-Dist: tiktoken (>=0.4.0,<1.0.0)
 Requires-Dist: torch (>=2.1.1,<3.0.0)
 Requires-Dist: tqdm (>=4.62.0,<5.0.0)
 Requires-Dist: transformers (>=4.37.1,<4.38.0)
-Requires-Dist: vllm (>=0.2.7,<1.0.0) ; sys_platform != "darwin"
+Requires-Dist: vllm (>=0.3.0,<1.0.0) ; sys_platform != "darwin"
 Project-URL: Repository, https://github.com/ScandEval/ScandEval
 Description-Content-Type: text/markdown
 
 <div align='center'>
 <img src="https://raw.githubusercontent.com/ScandEval/ScandEval/main/gfx/scandeval.png" width="517" height="217">
 </div>
 
 ### Evaluation of pretrained language models on mono- or multilingual language tasks.
 
 ______________________________________________________________________
 [![PyPI Status](https://badge.fury.io/py/scandeval.svg)](https://pypi.org/project/scandeval/)
 [![Paper](https://img.shields.io/badge/arXiv-2304.00906-b31b1b.svg)](https://arxiv.org/abs/2304.00906)
 [![License](https://img.shields.io/github/license/ScandEval/ScandEval)](https://github.com/ScandEval/ScandEval/blob/main/LICENSE)
 [![LastCommit](https://img.shields.io/github/last-commit/ScandEval/ScandEval)](https://github.com/ScandEval/ScandEval/commits/main)
-[![Code Coverage](https://img.shields.io/badge/Coverage-74%25-yellow.svg)](https://github.com/ScandEval/ScandEval/tree/main/tests)
+[![Code Coverage](https://img.shields.io/badge/Coverage-76%25-yellowgreen.svg)](https://github.com/ScandEval/ScandEval/tree/main/tests)
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.0-4baaaa.svg)](https://github.com/ScandEval/ScandEval/blob/main/CODE_OF_CONDUCT.md)
 
 
 ## Maintainers
 
 - Dan Saattrup Nielsen (@saattrupdan, dan.nielsen@alexandra.dk)
 - Kenneth Enevoldsen (@KennethEnevoldsen, kenneth.enevoldsen@cas.au.dk)
```

