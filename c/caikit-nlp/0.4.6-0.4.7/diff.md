# Comparing `tmp/caikit-nlp-0.4.6.tar.gz` & `tmp/caikit-nlp-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caikit-nlp-0.4.6.tar", last modified: Tue Mar 19 17:26:27 2024, max compression
+gzip compressed data, was "caikit-nlp-0.4.7.tar", last modified: Tue Apr  2 18:40:10 2024, max compression
```

## Comparing `caikit-nlp-0.4.6.tar` & `caikit-nlp-0.4.7.tar`

### file list

```diff
@@ -1,183 +1,183 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:26:27.181252 caikit-nlp-0.4.6/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:26:27.157252 caikit-nlp-0.4.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:26:27.157252 caikit-nlp-0.4.6/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/.github/ISSUE_TEMPLATE/user_story.md
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:26:27.157252 caikit-nlp-0.4.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/.github/workflows/build-image.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/.github/workflows/build-library.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/.github/workflows/lint-code.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/.github/workflows/publish-library.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/.prettierignore
--rw-r--r--   0 runner    (1001) docker     (127)    21457 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/.whitesource
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)     7191 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11424 2024-03-19 17:26:27.181252 caikit-nlp-0.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10588 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:26:27.157252 caikit-nlp-0.4.6/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/benchmarks/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:26:27.149252 caikit-nlp-0.4.6/benchmarks/logs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:26:27.157252 caikit-nlp-0.4.6/benchmarks/logs/llama2-7b/
--rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/benchmarks/logs/llama2-7b/20230905_183655.output
--rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/benchmarks/logs/llama2-7b/20230905_184809.output
--rw-r--r--   0 runner    (1001) docker     (127)     9795 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/benchmarks/logs/llama2-7b/20230905_191650.output
--rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/benchmarks/logs/llama2-7b/20230905_194133.output
--rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/benchmarks/logs/llama2-7b/20230906_135211.output
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:26:27.161252 caikit-nlp-0.4.6/caikit_nlp/
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/caikit_nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-19 17:26:27.000000 caikit-nlp-0.4.6/caikit_nlp/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:26:27.161252 caikit-nlp-0.4.6/caikit_nlp/config/
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/caikit_nlp/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/caikit_nlp/config/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:26:27.161252 caikit-nlp-0.4.6/caikit_nlp/data_model/
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/caikit_nlp/data_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/caikit_nlp/data_model/generation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:26:27.161252 caikit-nlp-0.4.6/caikit_nlp/model_management/
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/caikit_nlp/model_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5168 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/caikit_nlp/model_management/tgis_auto_finder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:26:27.161252 caikit-nlp-0.4.6/caikit_nlp/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/caikit_nlp/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:26:27.161252 caikit-nlp-0.4.6/caikit_nlp/modules/text_classification/
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/caikit_nlp/modules/text_classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7859 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/caikit_nlp/modules/text_classification/sequence_classification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:26:27.161252 caikit-nlp-0.4.6/caikit_nlp/modules/text_embedding/
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/caikit_nlp/modules/text_embedding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    39423 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/caikit_nlp/modules/text_embedding/embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/caikit_nlp/modules/text_embedding/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:26:27.165252 caikit-nlp-0.4.6/caikit_nlp/modules/text_generation/
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/caikit_nlp/modules/text_generation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8496 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/caikit_nlp/modules/text_generation/peft_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    51230 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/caikit_nlp/modules/text_generation/peft_prompt_tuning.py
--rw-r--r--   0 runner    (1001) docker     (127)    11624 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/caikit_nlp/modules/text_generation/peft_tgis_remote.py
--rw-r--r--   0 runner    (1001) docker     (127)    26132 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/caikit_nlp/modules/text_generation/text_generation_local.py
--rw-r--r--   0 runner    (1001) docker     (127)    11955 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/caikit_nlp/modules/text_generation/text_generation_tgis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:26:27.165252 caikit-nlp-0.4.6/caikit_nlp/modules/token_classification/
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/caikit_nlp/modules/token_classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15852 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/caikit_nlp/modules/token_classification/filtered_span_classification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:26:27.165252 caikit-nlp-0.4.6/caikit_nlp/modules/tokenization/
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/caikit_nlp/modules/tokenization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/caikit_nlp/modules/tokenization/regex_sentence_splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:26:27.165252 caikit-nlp-0.4.6/caikit_nlp/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/caikit_nlp/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:26:27.165252 caikit-nlp-0.4.6/caikit_nlp/resources/pretrained_model/
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/caikit_nlp/resources/pretrained_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15732 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/caikit_nlp/resources/pretrained_model/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    21429 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/caikit_nlp/resources/pretrained_model/hf_auto_causal_lm.py
--rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/caikit_nlp/resources/pretrained_model/hf_auto_seq2seq_lm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/caikit_nlp/resources/pretrained_model/hf_auto_seq_classifier.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:26:27.169252 caikit-nlp-0.4.6/caikit_nlp/toolkit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/caikit_nlp/toolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/caikit_nlp/toolkit/data_stream_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/caikit_nlp/toolkit/data_type_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/caikit_nlp/toolkit/task_specific_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:26:27.169252 caikit-nlp-0.4.6/caikit_nlp/toolkit/text_generation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/caikit_nlp/toolkit/text_generation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16766 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/caikit_nlp/toolkit/text_generation/model_run_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16535 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/caikit_nlp/toolkit/text_generation/tgis_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/caikit_nlp/toolkit/torch_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/caikit_nlp/toolkit/trainer_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/caikit_nlp/toolkit/verbalizer_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/caikit_nlp/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:26:27.181252 caikit-nlp-0.4.6/caikit_nlp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11424 2024-03-19 17:26:27.000000 caikit-nlp-0.4.6/caikit_nlp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-03-19 17:26:27.000000 caikit-nlp-0.4.6/caikit_nlp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 17:26:27.000000 caikit-nlp-0.4.6/caikit_nlp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-03-19 17:26:27.000000 caikit-nlp-0.4.6/caikit_nlp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-19 17:26:27.000000 caikit-nlp-0.4.6/caikit_nlp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/code-of-conduct.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:26:27.169252 caikit-nlp-0.4.6/examples/
--rw-r--r--   0 runner    (1001) docker     (127)    55479 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/examples/Caikit_Getting_Started.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/examples/compare_local_vs_tgis_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     7104 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/examples/evaluate_model.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      404 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/examples/kill-text-generation-launcher.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/examples/load_and_run_distributed_peft.py
--rw-r--r--   0 runner    (1001) docker     (127)    13678 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/examples/run_fine_tuning.py
--rw-r--r--   0 runner    (1001) docker     (127)    15840 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/examples/run_peft_tuning.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1992 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/examples/text-generation-launcher
--rw-r--r--   0 runner    (1001) docker     (127)    15815 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/examples/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6158 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/prompt_tuning_parameter_selection.md
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/runtime_config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:26:27.169252 caikit-nlp-0.4.6/runtime_template/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1252 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/runtime_template/run_with_gateway.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:26:27.169252 caikit-nlp-0.4.6/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)      657 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/scripts/dump_apis.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      720 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/scripts/fmt.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      231 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/scripts/run_local.sh
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 17:26:27.185252 caikit-nlp-0.4.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/setup_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:26:27.169252 caikit-nlp-0.4.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:26:27.169252 caikit-nlp-0.4.6/tests/data_model/
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/tests/data_model/test_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:26:27.169252 caikit-nlp-0.4.6/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)    10666 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/tests/fixtures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:26:27.169252 caikit-nlp-0.4.6/tests/fixtures/data_model/
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/tests/fixtures/data_model/sample_objects.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:26:27.173252 caikit-nlp-0.4.6/tests/fixtures/tiny_models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:26:27.173252 caikit-nlp-0.4.6/tests/fixtures/tiny_models/BertForSequenceClassification/
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/tests/fixtures/tiny_models/BertForSequenceClassification/config.json
--rw-r--r--   0 runner    (1001) docker     (127)   384767 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/tests/fixtures/tiny_models/BertForSequenceClassification/pytorch_model.bin
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/tests/fixtures/tiny_models/BertForSequenceClassification/special_tokens_map.json
--rw-r--r--   0 runner    (1001) docker     (127)   481096 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/tests/fixtures/tiny_models/BertForSequenceClassification/tf_model.h5
--rw-r--r--   0 runner    (1001) docker     (127)    23061 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/tests/fixtures/tiny_models/BertForSequenceClassification/tokenizer.json
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/tests/fixtures/tiny_models/BertForSequenceClassification/tokenizer_config.json
--rw-r--r--   0 runner    (1001) docker     (127)     4679 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/tests/fixtures/tiny_models/BertForSequenceClassification/vocab.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:26:27.177252 caikit-nlp-0.4.6/tests/fixtures/tiny_models/BloomForCausalLM/
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/tests/fixtures/tiny_models/BloomForCausalLM/config.json
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/tests/fixtures/tiny_models/BloomForCausalLM/generation_config.json
--rw-r--r--   0 runner    (1001) docker     (127)   406260 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/tests/fixtures/tiny_models/BloomForCausalLM/pytorch_model.bin
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/tests/fixtures/tiny_models/BloomForCausalLM/special_tokens_map.json
--rw-r--r--   0 runner    (1001) docker     (127)    33054 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/tests/fixtures/tiny_models/BloomForCausalLM/tokenizer.json
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/tests/fixtures/tiny_models/BloomForCausalLM/tokenizer_config.json
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/tests/fixtures/tiny_models/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:26:27.177252 caikit-nlp-0.4.6/tests/fixtures/tiny_models/T5ForConditionalGeneration/
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/tests/fixtures/tiny_models/T5ForConditionalGeneration/config.json
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/tests/fixtures/tiny_models/T5ForConditionalGeneration/generation_config.json
--rw-r--r--   0 runner    (1001) docker     (127)   546693 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/tests/fixtures/tiny_models/T5ForConditionalGeneration/pytorch_model.bin
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/tests/fixtures/tiny_models/T5ForConditionalGeneration/special_tokens_map.json
--rw-r--r--   0 runner    (1001) docker     (127)   382892 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/tests/fixtures/tiny_models/T5ForConditionalGeneration/tokenizer.json
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/tests/fixtures/tiny_models/T5ForConditionalGeneration/tokenizer_config.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:26:27.177252 caikit-nlp-0.4.6/tests/model_management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/tests/model_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9024 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/tests/model_management/test_tgis_auto_finder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:26:27.177252 caikit-nlp-0.4.6/tests/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/tests/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:26:27.177252 caikit-nlp-0.4.6/tests/modules/text_classification/
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/tests/modules/text_classification/test_sequence_classification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:26:27.177252 caikit-nlp-0.4.6/tests/modules/text_embedding/
--rw-r--r--   0 runner    (1001) docker     (127)    35704 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/tests/modules/text_embedding/test_embedding.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:26:27.181252 caikit-nlp-0.4.6/tests/modules/text_generation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/tests/modules/text_generation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/tests/modules/text_generation/test_peft_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    25729 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/tests/modules/text_generation/test_peft_prompt_tuning.py
--rw-r--r--   0 runner    (1001) docker     (127)     6540 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/tests/modules/text_generation/test_peft_tgis_remote.py
--rw-r--r--   0 runner    (1001) docker     (127)     7254 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/tests/modules/text_generation/test_text_generation_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     8300 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/tests/modules/text_generation/test_text_generation_tgis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:26:27.181252 caikit-nlp-0.4.6/tests/modules/token_classification/
--rw-r--r--   0 runner    (1001) docker     (127)    18398 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/tests/modules/token_classification/test_filtered_span_classification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:26:27.181252 caikit-nlp-0.4.6/tests/modules/tokenization/
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/tests/modules/tokenization/test_regex_sentence_splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:26:27.181252 caikit-nlp-0.4.6/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/tests/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16904 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/tests/resources/test_pretrained_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:26:27.181252 caikit-nlp-0.4.6/tests/toolkit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/tests/toolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/tests/toolkit/test_data_stream_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/tests/toolkit/test_data_type_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/tests/toolkit/test_task_specific_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/tests/toolkit/test_verbalizers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:26:27.181252 caikit-nlp-0.4.6/tests/toolkit/text_generation/
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/tests/toolkit/text_generation/test_model_run_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-03-19 17:26:19.000000 caikit-nlp-0.4.6/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.819068 caikit-nlp-0.4.7/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.791068 caikit-nlp-0.4.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.791068 caikit-nlp-0.4.7/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/.github/ISSUE_TEMPLATE/user_story.md
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.795068 caikit-nlp-0.4.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/.github/workflows/build-image.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/.github/workflows/build-library.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/.github/workflows/lint-code.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/.github/workflows/publish-library.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (127)    21457 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/.whitesource
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)     7191 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11424 2024-04-02 18:40:10.819068 caikit-nlp-0.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10588 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.795068 caikit-nlp-0.4.7/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/benchmarks/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.783068 caikit-nlp-0.4.7/benchmarks/logs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.795068 caikit-nlp-0.4.7/benchmarks/logs/llama2-7b/
+-rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/benchmarks/logs/llama2-7b/20230905_183655.output
+-rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/benchmarks/logs/llama2-7b/20230905_184809.output
+-rw-r--r--   0 runner    (1001) docker     (127)     9795 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/benchmarks/logs/llama2-7b/20230905_191650.output
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/benchmarks/logs/llama2-7b/20230905_194133.output
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/benchmarks/logs/llama2-7b/20230906_135211.output
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.795068 caikit-nlp-0.4.7/caikit_nlp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-02 18:40:10.000000 caikit-nlp-0.4.7/caikit_nlp/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.795068 caikit-nlp-0.4.7/caikit_nlp/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/config/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.795068 caikit-nlp-0.4.7/caikit_nlp/data_model/
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/data_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/data_model/generation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.799068 caikit-nlp-0.4.7/caikit_nlp/model_management/
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/model_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5168 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/model_management/tgis_auto_finder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.799068 caikit-nlp-0.4.7/caikit_nlp/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.799068 caikit-nlp-0.4.7/caikit_nlp/modules/text_classification/
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/modules/text_classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7859 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/modules/text_classification/sequence_classification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.799068 caikit-nlp-0.4.7/caikit_nlp/modules/text_embedding/
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/modules/text_embedding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39423 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/modules/text_embedding/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/modules/text_embedding/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.799068 caikit-nlp-0.4.7/caikit_nlp/modules/text_generation/
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/modules/text_generation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8496 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/modules/text_generation/peft_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51230 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/modules/text_generation/peft_prompt_tuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12248 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/modules/text_generation/peft_tgis_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26132 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/modules/text_generation/text_generation_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12610 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/modules/text_generation/text_generation_tgis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.799068 caikit-nlp-0.4.7/caikit_nlp/modules/token_classification/
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/modules/token_classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16150 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/modules/token_classification/filtered_span_classification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.799068 caikit-nlp-0.4.7/caikit_nlp/modules/tokenization/
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/modules/tokenization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/modules/tokenization/regex_sentence_splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.799068 caikit-nlp-0.4.7/caikit_nlp/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.803068 caikit-nlp-0.4.7/caikit_nlp/resources/pretrained_model/
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/resources/pretrained_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15732 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/resources/pretrained_model/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21429 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/resources/pretrained_model/hf_auto_causal_lm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/resources/pretrained_model/hf_auto_seq2seq_lm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/resources/pretrained_model/hf_auto_seq_classifier.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.803068 caikit-nlp-0.4.7/caikit_nlp/toolkit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/toolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/toolkit/data_stream_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/toolkit/data_type_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/toolkit/task_specific_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.803068 caikit-nlp-0.4.7/caikit_nlp/toolkit/text_generation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/toolkit/text_generation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16766 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/toolkit/text_generation/model_run_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19662 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/toolkit/text_generation/tgis_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/toolkit/torch_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/toolkit/trainer_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/toolkit/verbalizer_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.819068 caikit-nlp-0.4.7/caikit_nlp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11424 2024-04-02 18:40:10.000000 caikit-nlp-0.4.7/caikit_nlp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-04-02 18:40:10.000000 caikit-nlp-0.4.7/caikit_nlp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 18:40:10.000000 caikit-nlp-0.4.7/caikit_nlp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-02 18:40:10.000000 caikit-nlp-0.4.7/caikit_nlp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-02 18:40:10.000000 caikit-nlp-0.4.7/caikit_nlp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/code-of-conduct.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.803068 caikit-nlp-0.4.7/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    55479 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/examples/Caikit_Getting_Started.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/examples/compare_local_vs_tgis_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7104 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/examples/evaluate_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      404 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/examples/kill-text-generation-launcher.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/examples/load_and_run_distributed_peft.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13678 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/examples/run_fine_tuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15840 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/examples/run_peft_tuning.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1992 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/examples/text-generation-launcher
+-rw-r--r--   0 runner    (1001) docker     (127)    15815 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/examples/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6158 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/prompt_tuning_parameter_selection.md
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/runtime_config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.803068 caikit-nlp-0.4.7/runtime_template/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1252 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/runtime_template/run_with_gateway.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.807068 caikit-nlp-0.4.7/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      657 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/scripts/dump_apis.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      720 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/scripts/fmt.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      231 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/scripts/run_local.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 18:40:10.819068 caikit-nlp-0.4.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/setup_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.807068 caikit-nlp-0.4.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.807068 caikit-nlp-0.4.7/tests/data_model/
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/data_model/test_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.807068 caikit-nlp-0.4.7/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)    11719 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/fixtures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.807068 caikit-nlp-0.4.7/tests/fixtures/data_model/
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/fixtures/data_model/sample_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.807068 caikit-nlp-0.4.7/tests/fixtures/tiny_models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.807068 caikit-nlp-0.4.7/tests/fixtures/tiny_models/BertForSequenceClassification/
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/fixtures/tiny_models/BertForSequenceClassification/config.json
+-rw-r--r--   0 runner    (1001) docker     (127)   384767 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/fixtures/tiny_models/BertForSequenceClassification/pytorch_model.bin
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/fixtures/tiny_models/BertForSequenceClassification/special_tokens_map.json
+-rw-r--r--   0 runner    (1001) docker     (127)   481096 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/fixtures/tiny_models/BertForSequenceClassification/tf_model.h5
+-rw-r--r--   0 runner    (1001) docker     (127)    23061 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/fixtures/tiny_models/BertForSequenceClassification/tokenizer.json
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/fixtures/tiny_models/BertForSequenceClassification/tokenizer_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4679 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/fixtures/tiny_models/BertForSequenceClassification/vocab.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.811068 caikit-nlp-0.4.7/tests/fixtures/tiny_models/BloomForCausalLM/
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/fixtures/tiny_models/BloomForCausalLM/config.json
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/fixtures/tiny_models/BloomForCausalLM/generation_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)   406260 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/fixtures/tiny_models/BloomForCausalLM/pytorch_model.bin
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/fixtures/tiny_models/BloomForCausalLM/special_tokens_map.json
+-rw-r--r--   0 runner    (1001) docker     (127)    33054 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/fixtures/tiny_models/BloomForCausalLM/tokenizer.json
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/fixtures/tiny_models/BloomForCausalLM/tokenizer_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/fixtures/tiny_models/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.815068 caikit-nlp-0.4.7/tests/fixtures/tiny_models/T5ForConditionalGeneration/
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/fixtures/tiny_models/T5ForConditionalGeneration/config.json
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/fixtures/tiny_models/T5ForConditionalGeneration/generation_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)   546693 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/fixtures/tiny_models/T5ForConditionalGeneration/pytorch_model.bin
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/fixtures/tiny_models/T5ForConditionalGeneration/special_tokens_map.json
+-rw-r--r--   0 runner    (1001) docker     (127)   382892 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/fixtures/tiny_models/T5ForConditionalGeneration/tokenizer.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/fixtures/tiny_models/T5ForConditionalGeneration/tokenizer_config.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.815068 caikit-nlp-0.4.7/tests/model_management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/model_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9024 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/model_management/test_tgis_auto_finder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.815068 caikit-nlp-0.4.7/tests/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.815068 caikit-nlp-0.4.7/tests/modules/text_classification/
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/modules/text_classification/test_sequence_classification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.815068 caikit-nlp-0.4.7/tests/modules/text_embedding/
+-rw-r--r--   0 runner    (1001) docker     (127)    35704 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/modules/text_embedding/test_embedding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.815068 caikit-nlp-0.4.7/tests/modules/text_generation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/modules/text_generation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/modules/text_generation/test_peft_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25729 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/modules/text_generation/test_peft_prompt_tuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6540 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/modules/text_generation/test_peft_tgis_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7254 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/modules/text_generation/test_text_generation_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8300 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/modules/text_generation/test_text_generation_tgis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.815068 caikit-nlp-0.4.7/tests/modules/token_classification/
+-rw-r--r--   0 runner    (1001) docker     (127)    18398 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/modules/token_classification/test_filtered_span_classification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.815068 caikit-nlp-0.4.7/tests/modules/tokenization/
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/modules/tokenization/test_regex_sentence_splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.815068 caikit-nlp-0.4.7/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16904 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/resources/test_pretrained_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.815068 caikit-nlp-0.4.7/tests/toolkit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/toolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/toolkit/test_data_stream_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/toolkit/test_data_type_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/toolkit/test_task_specific_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/toolkit/test_verbalizers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.819068 caikit-nlp-0.4.7/tests/toolkit/text_generation/
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/toolkit/text_generation/test_model_run_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tox.ini
```

### Comparing `caikit-nlp-0.4.6/.github/ISSUE_TEMPLATE/bug_report.md` & `caikit-nlp-0.4.7/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/.github/ISSUE_TEMPLATE/feature_request.md` & `caikit-nlp-0.4.7/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/.github/ISSUE_TEMPLATE/user_story.md` & `caikit-nlp-0.4.7/.github/ISSUE_TEMPLATE/user_story.md`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/.github/workflows/build-image.yml` & `caikit-nlp-0.4.7/.github/workflows/build-image.yml`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/.github/workflows/build-library.yml` & `caikit-nlp-0.4.7/.github/workflows/build-library.yml`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/.github/workflows/lint-code.yml` & `caikit-nlp-0.4.7/.github/workflows/lint-code.yml`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/.github/workflows/publish-library.yml` & `caikit-nlp-0.4.7/.github/workflows/publish-library.yml`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/.gitignore` & `caikit-nlp-0.4.7/.gitignore`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/.pylintrc` & `caikit-nlp-0.4.7/.pylintrc`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/CONTRIBUTING.md` & `caikit-nlp-0.4.7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/Dockerfile` & `caikit-nlp-0.4.7/Dockerfile`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/LICENSE` & `caikit-nlp-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/PKG-INFO` & `caikit-nlp-0.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: caikit-nlp
-Version: 0.4.6
+Version: 0.4.7
 Summary: Caikit NLP
 License: Apache-2.0
 Project-URL: Source, https://github.com/caikit/caikit-nlp
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: ~=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: caikit[runtime-grpc,runtime-http]<0.27.0,>=0.26.14
+Requires-Dist: caikit[runtime-grpc,runtime-http]<0.27.0,>=0.26.17
 Requires-Dist: caikit-tgis-backend<0.2.0,>=0.1.27
 Requires-Dist: accelerate>=0.22.0
 Requires-Dist: datasets>=2.4.0
 Requires-Dist: huggingface-hub
 Requires-Dist: numpy>=1.22.4
 Requires-Dist: pandas>=1.5.0
 Requires-Dist: scikit-learn>=1.1
```

### Comparing `caikit-nlp-0.4.6/README.md` & `caikit-nlp-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/benchmarks/README.md` & `caikit-nlp-0.4.7/benchmarks/README.md`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/benchmarks/logs/llama2-7b/20230905_183655.output` & `caikit-nlp-0.4.7/benchmarks/logs/llama2-7b/20230905_183655.output`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/benchmarks/logs/llama2-7b/20230905_184809.output` & `caikit-nlp-0.4.7/benchmarks/logs/llama2-7b/20230905_184809.output`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/benchmarks/logs/llama2-7b/20230905_191650.output` & `caikit-nlp-0.4.7/benchmarks/logs/llama2-7b/20230905_191650.output`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/benchmarks/logs/llama2-7b/20230905_194133.output` & `caikit-nlp-0.4.7/benchmarks/logs/llama2-7b/20230905_194133.output`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/benchmarks/logs/llama2-7b/20230906_135211.output` & `caikit-nlp-0.4.7/benchmarks/logs/llama2-7b/20230906_135211.output`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/caikit_nlp/__init__.py` & `caikit-nlp-0.4.7/caikit_nlp/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/caikit_nlp/config/__init__.py` & `caikit-nlp-0.4.7/caikit_nlp/config/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/caikit_nlp/config/config.yml` & `caikit-nlp-0.4.7/caikit_nlp/config/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/caikit_nlp/data_model/__init__.py` & `caikit-nlp-0.4.7/caikit_nlp/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/caikit_nlp/data_model/generation.py` & `caikit-nlp-0.4.7/caikit_nlp/data_model/generation.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/caikit_nlp/model_management/__init__.py` & `caikit-nlp-0.4.7/caikit_nlp/model_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/caikit_nlp/model_management/tgis_auto_finder.py` & `caikit-nlp-0.4.7/caikit_nlp/model_management/tgis_auto_finder.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/caikit_nlp/modules/__init__.py` & `caikit-nlp-0.4.7/caikit_nlp/modules/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,8 +8,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # Local
-from . import text_classification, text_embedding, text_generation, token_classification
+from . import (
+    text_classification,
+    text_embedding,
+    text_generation,
+    token_classification,
+    tokenization,
+)
```

### Comparing `caikit-nlp-0.4.6/caikit_nlp/modules/text_classification/__init__.py` & `caikit-nlp-0.4.7/caikit_nlp/modules/text_classification/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/caikit_nlp/modules/text_classification/sequence_classification.py` & `caikit-nlp-0.4.7/caikit_nlp/modules/text_classification/sequence_classification.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/caikit_nlp/modules/text_embedding/__init__.py` & `caikit-nlp-0.4.7/caikit_nlp/modules/text_embedding/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/caikit_nlp/modules/text_embedding/embedding.py` & `caikit-nlp-0.4.7/caikit_nlp/modules/text_embedding/embedding.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/caikit_nlp/modules/text_embedding/utils.py` & `caikit-nlp-0.4.7/caikit_nlp/modules/text_embedding/utils.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/caikit_nlp/modules/text_generation/__init__.py` & `caikit-nlp-0.4.7/caikit_nlp/modules/text_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/caikit_nlp/modules/text_generation/peft_config.py` & `caikit-nlp-0.4.7/caikit_nlp/modules/text_generation/peft_config.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/caikit_nlp/modules/text_generation/peft_prompt_tuning.py` & `caikit-nlp-0.4.7/caikit_nlp/modules/text_generation/peft_prompt_tuning.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/caikit_nlp/modules/text_generation/peft_tgis_remote.py` & `caikit-nlp-0.4.7/caikit_nlp/modules/text_generation/peft_tgis_remote.py`

 * *Files 6% similar despite different names*

```diff
@@ -198,14 +198,18 @@
         max_time: Optional[float] = None,
         exponential_decay_length_penalty: Optional[
             Union[Tuple[int, float], ExponentialDecayLengthPenalty]
         ] = None,
         stop_sequences: Optional[List[str]] = None,
         seed: Optional[np.uint64] = None,
         preserve_input_text: bool = False,
+        input_tokens: bool = False,
+        generated_tokens: bool = True,
+        token_logprobs: bool = True,
+        token_ranks: bool = True,
     ) -> GeneratedTextResult:
         f"""Run inference against the model running in TGIS.
 
         Args:
            {GENERATE_FUNCTION_TGIS_ARGS}
         Returns:
             GeneratedTextResult
@@ -217,14 +221,18 @@
             self.enable_backend,
             "Backend must be configured and loaded with this module before executing `run` call.",
         )
         verbalized_text = render_verbalizer(self.verbalizer, {"input": text})
         return self.tgis_generation_client.unary_generate(
             text=verbalized_text,
             preserve_input_text=preserve_input_text,
+            input_tokens=input_tokens,
+            generated_tokens=generated_tokens,
+            token_logprobs=token_logprobs,
+            token_ranks=token_ranks,
             max_new_tokens=max_new_tokens,
             min_new_tokens=min_new_tokens,
             truncate_input_tokens=truncate_input_tokens,
             decoding_method=decoding_method,
             top_k=top_k,
             top_p=top_p,
             typical_p=typical_p,
@@ -252,14 +260,18 @@
         max_time: Optional[float] = None,
         exponential_decay_length_penalty: Optional[
             Union[Tuple[int, float], ExponentialDecayLengthPenalty]
         ] = None,
         stop_sequences: Optional[List[str]] = None,
         seed: Optional[np.uint64] = None,
         preserve_input_text: bool = False,
+        input_tokens: bool = False,
+        generated_tokens: bool = True,
+        token_logprobs: bool = True,
+        token_ranks: bool = True,
     ) -> Iterable[GeneratedTextStreamResult]:
         f"""Run output stream inferencing against the model running in TGIS
 
         Args:
             {GENERATE_FUNCTION_TGIS_ARGS}
         Returns:
             Iterable[GeneratedTextStreamResult]
@@ -271,14 +283,18 @@
             "Backend must be configured and loaded with this module \
             before executing `run_stream_out` call.",
         )
         verbalized_text = render_verbalizer(self.verbalizer, {"input": text})
         return self.tgis_generation_client.stream_generate(
             text=verbalized_text,
             preserve_input_text=preserve_input_text,
+            input_tokens=input_tokens,
+            generated_tokens=generated_tokens,
+            token_logprobs=token_logprobs,
+            token_ranks=token_ranks,
             max_new_tokens=max_new_tokens,
             min_new_tokens=min_new_tokens,
             truncate_input_tokens=truncate_input_tokens,
             decoding_method=decoding_method,
             top_k=top_k,
             top_p=top_p,
             typical_p=typical_p,
```

### Comparing `caikit-nlp-0.4.6/caikit_nlp/modules/text_generation/text_generation_local.py` & `caikit-nlp-0.4.7/caikit_nlp/modules/text_generation/text_generation_local.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/caikit_nlp/modules/text_generation/text_generation_tgis.py` & `caikit-nlp-0.4.7/caikit_nlp/modules/text_generation/text_generation_tgis.py`

 * *Files 5% similar despite different names*

```diff
@@ -223,28 +223,35 @@
         max_time: Optional[float] = None,
         exponential_decay_length_penalty: Optional[
             Union[Tuple[int, float], ExponentialDecayLengthPenalty]
         ] = None,
         stop_sequences: Optional[List[str]] = None,
         seed: Optional[np.uint64] = None,
         preserve_input_text: bool = False,
+        input_tokens: bool = False,
+        generated_tokens: bool = True,
+        token_logprobs: bool = True,
+        token_ranks: bool = True,
     ) -> GeneratedTextResult:
         f"""Run inference against the model running in TGIS.
 
         Args:
            {GENERATE_FUNCTION_TGIS_ARGS}
         Returns:
             GeneratedTextResult
                 Generated text result produced by TGIS.
         """
-
         if self._model_loaded:
             return self.tgis_generation_client.unary_generate(
                 text=text,
                 preserve_input_text=preserve_input_text,
+                input_tokens=input_tokens,
+                generated_tokens=generated_tokens,
+                token_logprobs=token_logprobs,
+                token_ranks=token_ranks,
                 max_new_tokens=max_new_tokens,
                 min_new_tokens=min_new_tokens,
                 truncate_input_tokens=truncate_input_tokens,
                 decoding_method=decoding_method,
                 top_k=top_k,
                 top_p=top_p,
                 typical_p=typical_p,
@@ -272,27 +279,35 @@
         max_time: Optional[float] = None,
         exponential_decay_length_penalty: Optional[
             Union[Tuple[int, float], ExponentialDecayLengthPenalty]
         ] = None,
         stop_sequences: Optional[List[str]] = None,
         seed: Optional[np.uint64] = None,
         preserve_input_text: bool = False,
+        input_tokens: bool = False,
+        generated_tokens: bool = True,
+        token_logprobs: bool = True,
+        token_ranks: bool = True,
     ) -> Iterable[GeneratedTextStreamResult]:
         f"""Run output stream inferencing for text generation module.
 
         Args:
             {GENERATE_FUNCTION_TGIS_ARGS}
         Returns:
             Iterable[GeneratedTextStreamResult]
         """
 
         if self._model_loaded:
             return self.tgis_generation_client.stream_generate(
                 text=text,
                 preserve_input_text=preserve_input_text,
+                input_tokens=input_tokens,
+                generated_tokens=generated_tokens,
+                token_logprobs=token_logprobs,
+                token_ranks=token_ranks,
                 max_new_tokens=max_new_tokens,
                 min_new_tokens=min_new_tokens,
                 truncate_input_tokens=truncate_input_tokens,
                 decoding_method=decoding_method,
                 top_k=top_k,
                 top_p=top_p,
                 typical_p=typical_p,
```

### Comparing `caikit-nlp-0.4.6/caikit_nlp/modules/token_classification/__init__.py` & `caikit-nlp-0.4.7/caikit_nlp/modules/token_classification/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/caikit_nlp/modules/token_classification/filtered_span_classification.py` & `caikit-nlp-0.4.7/caikit_nlp/modules/token_classification/filtered_span_classification.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 """This module returns span classification output by splitting
 text into spans and returning classifications for each span. Span
 classifications can be filtered by score threshold and label(s).
 At this time this module is only designed for inference"""
 
 # Standard
 from typing import Iterable, List, Optional, Union
+import itertools
 import os
 
 # First Party
 from caikit.core.exceptions import error_handler
 from caikit.core.modules import (
     ModuleBase,
     ModuleConfig,
@@ -209,21 +210,26 @@
         error.type_check(
             "<NLP96166348E>", float, int, allow_none=True, threshold=threshold
         )
         # TODO: For optimization implement window based approach.
         if threshold is None:
             threshold = self.default_threshold
 
-        # Types on the stream are checked later on iteration
-        if len(text_stream) == 0:
+        # Avoid length check here since it can be time consuming to iterate through stream
+        # Tee stream to 2 - one to check emptiness, one for full iteration + analysis
+        text_streams = itertools.tee(text_stream, 2)
+        try:
+            next(text_streams[0])
+        except StopIteration:
+            # Types on the stream are checked later on iteration
             # Allow empty text case to fall through - some tokenizers or
             # classifiers may error on this
             yield TokenClassificationStreamResult(results=[], processed_index=0)
 
-        for span_output in self._stream_span_output(text_stream):
+        for span_output in self._stream_span_output(text_streams[1]):
             classification_result = self.classifier.run(span_output.text)
             results_to_end_of_span = False
             for classification in classification_result.results:
                 if self.classification_task == TextClassificationTask:
                     label = classification.label
                     start = span_output.start
                     end = span_output.end
```

### Comparing `caikit-nlp-0.4.6/caikit_nlp/modules/tokenization/__init__.py` & `caikit-nlp-0.4.7/caikit_nlp/modules/tokenization/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/caikit_nlp/modules/tokenization/regex_sentence_splitter.py` & `caikit-nlp-0.4.7/caikit_nlp/modules/tokenization/regex_sentence_splitter.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/caikit_nlp/resources/__init__.py` & `caikit-nlp-0.4.7/caikit_nlp/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/caikit_nlp/resources/pretrained_model/__init__.py` & `caikit-nlp-0.4.7/caikit_nlp/resources/pretrained_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/caikit_nlp/resources/pretrained_model/base.py` & `caikit-nlp-0.4.7/caikit_nlp/resources/pretrained_model/base.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/caikit_nlp/resources/pretrained_model/hf_auto_causal_lm.py` & `caikit-nlp-0.4.7/caikit_nlp/resources/pretrained_model/hf_auto_causal_lm.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/caikit_nlp/resources/pretrained_model/hf_auto_seq2seq_lm.py` & `caikit-nlp-0.4.7/caikit_nlp/resources/pretrained_model/hf_auto_seq2seq_lm.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/caikit_nlp/resources/pretrained_model/hf_auto_seq_classifier.py` & `caikit-nlp-0.4.7/caikit_nlp/resources/pretrained_model/hf_auto_seq_classifier.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/caikit_nlp/toolkit/data_stream_wrapper.py` & `caikit-nlp-0.4.7/caikit_nlp/toolkit/data_stream_wrapper.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/caikit_nlp/toolkit/data_type_utils.py` & `caikit-nlp-0.4.7/caikit_nlp/toolkit/data_type_utils.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/caikit_nlp/toolkit/task_specific_utils.py` & `caikit-nlp-0.4.7/caikit_nlp/toolkit/task_specific_utils.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/caikit_nlp/toolkit/text_generation/model_run_utils.py` & `caikit-nlp-0.4.7/caikit_nlp/toolkit/text_generation/model_run_utils.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/caikit_nlp/toolkit/text_generation/tgis_utils.py` & `caikit-nlp-0.4.7/caikit_nlp/toolkit/text_generation/tgis_utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -33,25 +33,39 @@
 from .model_run_utils import GENERATE_FUNCTION_ARGS, VALID_DECODING_METHODS
 
 log = alog.use_channel("TGIS_UTILS")
 error = error_handler.get(log)
 
 GENERATE_FUNCTION_TGIS_ARGS = """
     {}
-    preserve_input_text: str
+    preserve_input_text: bool
         Whether or not the source string should be contained in the generated output,
         e.g., as a prefix.
+    input_tokens: bool
+        Whether or not to include list of input tokens.  
+    generated_tokens: bool
+        Whether or not to include list of individual generated tokens.  
+    token_logprobs: bool
+        Whether or not to include logprob for each returned token.  
+        Applicable only if generated_tokens == true and/or input_tokens == true
+    token_ranks: bool
+        Whether or not to include rank of each returned token.     
+        Applicable only if generated_tokens == true and/or input_tokens == true                             
 """.format(
     GENERATE_FUNCTION_ARGS
 )
 
 
 def validate_inf_params(
     text,
     preserve_input_text,
+    input_tokens,
+    generated_tokens,
+    token_logprobs,
+    token_ranks,
     eos_token,
     max_new_tokens,
     min_new_tokens,
     truncate_input_tokens,
     decoding_method,
     top_k,
     top_p,
@@ -70,14 +84,18 @@
            A special token representing the end of a sentence.
         {}
     """.format(
         GENERATE_FUNCTION_TGIS_ARGS
     )
     error.type_check("<NLP65883535E>", str, text=text)
     error.type_check("<NLP65883537E>", bool, preserve_input_text=preserve_input_text)
+    error.type_check("<NLP65883538E>", bool, input_tokens=input_tokens)
+    error.type_check("<NLP65883539E>", bool, generated_tokens=generated_tokens)
+    error.type_check("<NLP65883540E>", bool, token_logprobs=token_logprobs)
+    error.type_check("<NLP65883541E>", bool, token_ranks=token_ranks)
     error.type_check("<NLP85452188E>", str, allow_none=True, eos_token=eos_token)
     error.type_check(
         "<NLP03860681E>",
         int,
         allow_none=True,
         max_new_tokens=max_new_tokens,
         min_new_tokens=min_new_tokens,
@@ -170,14 +188,18 @@
             "sampling parameters (temperature/top_k/top_p/typical_p/seed) aren't "
             "applicable in greedy decoding mode"
         )
 
 
 def get_params(
     preserve_input_text,
+    input_tokens,
+    generated_tokens,
+    token_logprobs,
+    token_ranks,
     max_new_tokens,
     min_new_tokens,
     truncate_input_tokens,
     decoding_method,
     top_k,
     top_p,
     typical_p,
@@ -207,18 +229,18 @@
         top_p=top_p,
         typical_p=typical_p,
         seed=seed,
     )
 
     res_options = generation_pb2.ResponseOptions(
         input_text=preserve_input_text,
-        generated_tokens=True,
-        input_tokens=False,
-        token_logprobs=True,
-        token_ranks=True,
+        generated_tokens=generated_tokens,
+        input_tokens=input_tokens,
+        token_logprobs=token_logprobs,
+        token_ranks=token_ranks,
     )
     stopping = generation_pb2.StoppingCriteria(
         stop_sequences=stop_sequences,
         max_new_tokens=max_new_tokens,
         min_new_tokens=min_new_tokens,
         time_limit_millis=int(max_time * 1000) if max_time else None,
     )
@@ -264,14 +286,18 @@
         self.producer_id = producer_id
         self.prefix_id = prefix_id
 
     def unary_generate(
         self,
         text,
         preserve_input_text,
+        input_tokens,
+        generated_tokens,
+        token_logprobs,
+        token_ranks,
         max_new_tokens,
         min_new_tokens,
         truncate_input_tokens,
         decoding_method,
         top_k,
         top_p,
         typical_p,
@@ -301,14 +327,18 @@
             self.tgis_client is not None,
             "Backend must be configured and loaded for generate",
         )
 
         validate_inf_params(
             text=text,
             preserve_input_text=preserve_input_text,
+            input_tokens=input_tokens,
+            generated_tokens=generated_tokens,
+            token_logprobs=token_logprobs,
+            token_ranks=token_ranks,
             eos_token=self.eos_token,
             max_new_tokens=max_new_tokens,
             min_new_tokens=min_new_tokens,
             truncate_input_tokens=truncate_input_tokens,
             decoding_method=decoding_method,
             top_k=top_k,
             top_p=top_p,
@@ -321,14 +351,18 @@
             stop_sequences=stop_sequences,
         )
 
         log.debug("Building protobuf request to send to TGIS")
 
         params = get_params(
             preserve_input_text=preserve_input_text,
+            input_tokens=input_tokens,
+            generated_tokens=generated_tokens,
+            token_logprobs=token_logprobs,
+            token_ranks=token_ranks,
             max_new_tokens=max_new_tokens,
             min_new_tokens=min_new_tokens,
             truncate_input_tokens=truncate_input_tokens,
             decoding_method=decoding_method,
             top_k=top_k,
             top_p=top_p,
             typical_p=typical_p,
@@ -362,27 +396,51 @@
         error.value_check(
             "<NLP38899018E>",
             len(batch_response.responses) == 1,
             f"Got {len(batch_response.responses)} responses for a single request",
         )
         response = batch_response.responses[0]
 
+        token_list = []
+        if response.tokens is not None:
+            for token in response.tokens:
+                token_list.append(
+                    GeneratedToken(
+                        text=token.text, logprob=token.logprob, rank=token.rank
+                    )
+                )
+
+        input_token_list = []
+        if response.input_tokens is not None:
+            for token in response.input_tokens:
+                input_token_list.append(
+                    GeneratedToken(
+                        text=token.text, logprob=token.logprob, rank=token.rank
+                    )
+                )
+
         return GeneratedTextResult(
             generated_text=response.text,
             generated_tokens=response.generated_token_count,
             finish_reason=response.stop_reason,
             producer_id=self.producer_id,
             input_token_count=response.input_token_count,
             seed=seed,
+            tokens=token_list,
+            input_tokens=input_token_list,
         )
 
     def stream_generate(
         self,
         text,
         preserve_input_text,
+        input_tokens,
+        generated_tokens,
+        token_logprobs,
+        token_ranks,
         max_new_tokens,
         min_new_tokens,
         truncate_input_tokens,
         decoding_method,
         top_k,
         top_p,
         typical_p,
@@ -412,14 +470,18 @@
             "Backend must be configured and loaded for generate",
         )
         log.debug("Building protobuf request to send to TGIS")
 
         validate_inf_params(
             text=text,
             preserve_input_text=preserve_input_text,
+            input_tokens=input_tokens,
+            generated_tokens=generated_tokens,
+            token_logprobs=token_logprobs,
+            token_ranks=token_ranks,
             eos_token=self.eos_token,
             max_new_tokens=max_new_tokens,
             min_new_tokens=min_new_tokens,
             truncate_input_tokens=truncate_input_tokens,
             decoding_method=decoding_method,
             top_k=top_k,
             top_p=top_p,
@@ -430,14 +492,18 @@
             max_time=max_time,
             exponential_decay_length_penalty=exponential_decay_length_penalty,
             stop_sequences=stop_sequences,
         )
 
         params = get_params(
             preserve_input_text=preserve_input_text,
+            input_tokens=input_tokens,
+            generated_tokens=generated_tokens,
+            token_logprobs=token_logprobs,
+            token_ranks=token_ranks,
             max_new_tokens=max_new_tokens,
             min_new_tokens=min_new_tokens,
             truncate_input_tokens=truncate_input_tokens,
             decoding_method=decoding_method,
             top_k=top_k,
             top_p=top_p,
             typical_p=typical_p,
@@ -472,21 +538,33 @@
             details = TokenStreamDetails(
                 finish_reason=stream_part.stop_reason,
                 generated_tokens=stream_part.generated_token_count,
                 seed=stream_part.seed,
                 input_token_count=stream_part.input_token_count,
             )
             token_list = []
-            for token in stream_part.tokens:
-                token_list.append(
-                    GeneratedToken(text=token.text, logprob=token.logprob)
-                )
+            if stream_part.tokens is not None:
+                for token in stream_part.tokens:
+                    token_list.append(
+                        GeneratedToken(
+                            text=token.text, logprob=token.logprob, rank=token.rank
+                        )
+                    )
+            input_token_list = []
+            if stream_part.input_tokens is not None:
+                for token in stream_part.input_tokens:
+                    input_token_list.append(
+                        GeneratedToken(
+                            text=token.text, logprob=token.logprob, rank=token.rank
+                        )
+                    )
             yield GeneratedTextStreamResult(
                 generated_text=stream_part.text,
                 tokens=token_list,
+                input_tokens=input_token_list,
                 details=details,
             )
 
     def unary_tokenize(
         self,
         text: str,
     ) -> TokenizationResults:
```

### Comparing `caikit-nlp-0.4.6/caikit_nlp/toolkit/torch_run.py` & `caikit-nlp-0.4.7/caikit_nlp/toolkit/torch_run.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/caikit_nlp/toolkit/trainer_utils.py` & `caikit-nlp-0.4.7/caikit_nlp/toolkit/trainer_utils.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/caikit_nlp/toolkit/verbalizer_utils.py` & `caikit-nlp-0.4.7/caikit_nlp/toolkit/verbalizer_utils.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/caikit_nlp.egg-info/PKG-INFO` & `caikit-nlp-0.4.7/caikit_nlp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: caikit-nlp
-Version: 0.4.6
+Version: 0.4.7
 Summary: Caikit NLP
 License: Apache-2.0
 Project-URL: Source, https://github.com/caikit/caikit-nlp
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: ~=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: caikit[runtime-grpc,runtime-http]<0.27.0,>=0.26.14
+Requires-Dist: caikit[runtime-grpc,runtime-http]<0.27.0,>=0.26.17
 Requires-Dist: caikit-tgis-backend<0.2.0,>=0.1.27
 Requires-Dist: accelerate>=0.22.0
 Requires-Dist: datasets>=2.4.0
 Requires-Dist: huggingface-hub
 Requires-Dist: numpy>=1.22.4
 Requires-Dist: pandas>=1.5.0
 Requires-Dist: scikit-learn>=1.1
```

### Comparing `caikit-nlp-0.4.6/caikit_nlp.egg-info/SOURCES.txt` & `caikit-nlp-0.4.7/caikit_nlp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/examples/Caikit_Getting_Started.ipynb` & `caikit-nlp-0.4.7/examples/Caikit_Getting_Started.ipynb`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/examples/compare_local_vs_tgis_models.py` & `caikit-nlp-0.4.7/examples/compare_local_vs_tgis_models.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/examples/evaluate_model.py` & `caikit-nlp-0.4.7/examples/evaluate_model.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/examples/load_and_run_distributed_peft.py` & `caikit-nlp-0.4.7/examples/load_and_run_distributed_peft.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/examples/run_fine_tuning.py` & `caikit-nlp-0.4.7/examples/run_fine_tuning.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/examples/run_peft_tuning.py` & `caikit-nlp-0.4.7/examples/run_peft_tuning.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/examples/text-generation-launcher` & `caikit-nlp-0.4.7/examples/text-generation-launcher`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/examples/utils.py` & `caikit-nlp-0.4.7/examples/utils.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/prompt_tuning_parameter_selection.md` & `caikit-nlp-0.4.7/prompt_tuning_parameter_selection.md`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/pyproject.toml` & `caikit-nlp-0.4.7/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 license = {text = "Apache-2.0"}
 readme = "README.md"
 requires-python = "~=3.9"
 classifiers=[
     "License :: OSI Approved :: Apache Software License"
 ]
 dependencies = [
-    "caikit[runtime-grpc,runtime-http]>=0.26.14,<0.27.0",
+    "caikit[runtime-grpc,runtime-http]>=0.26.17,<0.27.0",
     "caikit-tgis-backend>=0.1.27,<0.2.0",
     # TODO: loosen dependencies
     "accelerate>=0.22.0",
     "datasets>=2.4.0",
     "huggingface-hub",
     "numpy>=1.22.4",
     "pandas>=1.5.0",
```

### Comparing `caikit-nlp-0.4.6/runtime_config.yaml` & `caikit-nlp-0.4.7/runtime_config.yaml`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/runtime_template/run_with_gateway.sh` & `caikit-nlp-0.4.7/runtime_template/run_with_gateway.sh`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/scripts/dump_apis.sh` & `caikit-nlp-0.4.7/scripts/dump_apis.sh`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/scripts/fmt.sh` & `caikit-nlp-0.4.7/scripts/fmt.sh`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/tests/conftest.py` & `caikit-nlp-0.4.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/tests/data_model/test_generation.py` & `caikit-nlp-0.4.7/tests/data_model/test_generation.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/tests/fixtures/__init__.py` & `caikit-nlp-0.4.7/tests/fixtures/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -211,28 +211,44 @@
     def unary_generate(request):
         fake_response = mock.Mock()
         fake_result = mock.Mock()
         fake_result.stop_reason = 5
         fake_result.generated_token_count = 1
         fake_result.text = "moose"
         fake_result.input_token_count = 1
+        token = mock.Mock()
+        token.text = "moose"
+        token.logprob = 0.2
+        token.rank = 1
+        fake_result.tokens = [token]
+        input_tokens = mock.Mock()
+        input_tokens.text = "moose"
+        input_tokens.logprob = 0.2
+        input_tokens.rank = 1
+        fake_result.input_tokens = [input_tokens]
         fake_response.responses = [fake_result]
         return fake_response
 
     @staticmethod
     def stream_generate(request):
         fake_stream = mock.Mock()
         fake_stream.stop_reason = 5
         fake_stream.generated_token_count = 1
         fake_stream.seed = 10
         fake_stream.input_token_count = 1
         token = mock.Mock()
         token.text = "moose"
         token.logprob = 0.2
+        token.rank = 1
         fake_stream.tokens = [token]
+        input_tokens = mock.Mock()
+        input_tokens.text = "moose"
+        input_tokens.logprob = 0.2
+        input_tokens.rank = 1
+        fake_stream.input_tokens = [input_tokens]
         fake_stream.text = "moose"
         for _ in range(3):
             yield fake_stream
 
     @staticmethod
     def tokenize(request):
         fake_response = mock.Mock()
@@ -244,25 +260,35 @@
     @staticmethod
     def validate_unary_generate_response(result):
         assert isinstance(result, GeneratedTextResult)
         assert result.generated_text == "moose"
         assert result.generated_tokens == 1
         assert result.finish_reason == 5
         assert result.input_token_count == 1
+        assert result.tokens[0].text == "moose"
+        assert result.tokens[0].logprob == 0.2
+        assert result.tokens[0].rank == 1
+        assert result.input_tokens[0].text == "moose"
+        assert result.input_tokens[0].logprob == 0.2
+        assert result.input_tokens[0].rank == 1
 
     @staticmethod
     def validate_stream_generate_response(stream_result):
         assert isinstance(stream_result, Iterable)
         # Convert to list to more easily check outputs
         result_list = list(stream_result)
         assert len(result_list) == 3
         first_result = result_list[0]
         assert first_result.generated_text == "moose"
         assert first_result.tokens[0].text == "moose"
         assert first_result.tokens[0].logprob == 0.2
+        assert first_result.tokens[0].rank == 1
+        assert first_result.input_tokens[0].text == "moose"
+        assert first_result.input_tokens[0].logprob == 0.2
+        assert first_result.input_tokens[0].rank == 1
         assert first_result.details.finish_reason == 5
         assert first_result.details.generated_tokens == 1
         assert first_result.details.seed == 10
         assert first_result.details.input_token_count == 1
 
     @staticmethod
     def validate_tokenize_response(result):
```

### Comparing `caikit-nlp-0.4.6/tests/fixtures/data_model/sample_objects.py` & `caikit-nlp-0.4.7/tests/fixtures/data_model/sample_objects.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/tests/fixtures/tiny_models/BertForSequenceClassification/config.json` & `caikit-nlp-0.4.7/tests/fixtures/tiny_models/BertForSequenceClassification/config.json`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/tests/fixtures/tiny_models/BertForSequenceClassification/pytorch_model.bin` & `caikit-nlp-0.4.7/tests/fixtures/tiny_models/BertForSequenceClassification/pytorch_model.bin`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/tests/fixtures/tiny_models/BertForSequenceClassification/tf_model.h5` & `caikit-nlp-0.4.7/tests/fixtures/tiny_models/BertForSequenceClassification/tf_model.h5`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/tests/fixtures/tiny_models/BertForSequenceClassification/tokenizer.json` & `caikit-nlp-0.4.7/tests/fixtures/tiny_models/BertForSequenceClassification/tokenizer.json`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/tests/fixtures/tiny_models/BertForSequenceClassification/vocab.txt` & `caikit-nlp-0.4.7/tests/fixtures/tiny_models/BertForSequenceClassification/vocab.txt`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/tests/fixtures/tiny_models/BloomForCausalLM/config.json` & `caikit-nlp-0.4.7/tests/fixtures/tiny_models/BloomForCausalLM/config.json`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/tests/fixtures/tiny_models/BloomForCausalLM/pytorch_model.bin` & `caikit-nlp-0.4.7/tests/fixtures/tiny_models/BloomForCausalLM/pytorch_model.bin`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/tests/fixtures/tiny_models/BloomForCausalLM/tokenizer.json` & `caikit-nlp-0.4.7/tests/fixtures/tiny_models/BloomForCausalLM/tokenizer.json`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/tests/fixtures/tiny_models/README.md` & `caikit-nlp-0.4.7/tests/fixtures/tiny_models/README.md`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/tests/fixtures/tiny_models/T5ForConditionalGeneration/config.json` & `caikit-nlp-0.4.7/tests/fixtures/tiny_models/T5ForConditionalGeneration/config.json`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/tests/fixtures/tiny_models/T5ForConditionalGeneration/pytorch_model.bin` & `caikit-nlp-0.4.7/tests/fixtures/tiny_models/T5ForConditionalGeneration/pytorch_model.bin`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/tests/fixtures/tiny_models/T5ForConditionalGeneration/special_tokens_map.json` & `caikit-nlp-0.4.7/tests/fixtures/tiny_models/T5ForConditionalGeneration/special_tokens_map.json`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/tests/fixtures/tiny_models/T5ForConditionalGeneration/tokenizer.json` & `caikit-nlp-0.4.7/tests/fixtures/tiny_models/T5ForConditionalGeneration/tokenizer.json`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/tests/fixtures/tiny_models/T5ForConditionalGeneration/tokenizer_config.json` & `caikit-nlp-0.4.7/tests/fixtures/tiny_models/T5ForConditionalGeneration/tokenizer_config.json`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/tests/model_management/test_tgis_auto_finder.py` & `caikit-nlp-0.4.7/tests/model_management/test_tgis_auto_finder.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/tests/modules/text_classification/test_sequence_classification.py` & `caikit-nlp-0.4.7/tests/modules/text_classification/test_sequence_classification.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/tests/modules/text_embedding/test_embedding.py` & `caikit-nlp-0.4.7/tests/modules/text_embedding/test_embedding.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/tests/modules/text_generation/test_peft_config.py` & `caikit-nlp-0.4.7/tests/modules/text_generation/test_peft_config.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/tests/modules/text_generation/test_peft_prompt_tuning.py` & `caikit-nlp-0.4.7/tests/modules/text_generation/test_peft_prompt_tuning.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/tests/modules/text_generation/test_peft_tgis_remote.py` & `caikit-nlp-0.4.7/tests/modules/text_generation/test_peft_tgis_remote.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/tests/modules/text_generation/test_text_generation_local.py` & `caikit-nlp-0.4.7/tests/modules/text_generation/test_text_generation_local.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/tests/modules/text_generation/test_text_generation_tgis.py` & `caikit-nlp-0.4.7/tests/modules/text_generation/test_text_generation_tgis.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/tests/modules/token_classification/test_filtered_span_classification.py` & `caikit-nlp-0.4.7/tests/modules/token_classification/test_filtered_span_classification.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/tests/modules/tokenization/test_regex_sentence_splitter.py` & `caikit-nlp-0.4.7/tests/modules/tokenization/test_regex_sentence_splitter.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/tests/resources/test_pretrained_model.py` & `caikit-nlp-0.4.7/tests/resources/test_pretrained_model.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/tests/toolkit/test_data_stream_wrapper.py` & `caikit-nlp-0.4.7/tests/toolkit/test_data_stream_wrapper.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/tests/toolkit/test_data_type_utils.py` & `caikit-nlp-0.4.7/tests/toolkit/test_data_type_utils.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/tests/toolkit/test_task_specific_utils.py` & `caikit-nlp-0.4.7/tests/toolkit/test_task_specific_utils.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/tests/toolkit/test_verbalizers.py` & `caikit-nlp-0.4.7/tests/toolkit/test_verbalizers.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/tests/toolkit/text_generation/test_model_run_utils.py` & `caikit-nlp-0.4.7/tests/toolkit/text_generation/test_model_run_utils.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.6/tox.ini` & `caikit-nlp-0.4.7/tox.ini`

 * *Files identical despite different names*

