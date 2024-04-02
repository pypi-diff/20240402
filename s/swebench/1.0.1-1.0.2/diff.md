# Comparing `tmp/swebench-1.0.1.tar.gz` & `tmp/swebench-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swebench-1.0.1.tar", last modified: Mon Apr  1 03:16:07 2024, max compression
+gzip compressed data, was "swebench-1.0.2.tar", last modified: Tue Apr  2 13:57:35 2024, max compression
```

## Comparing `swebench-1.0.1.tar` & `swebench-1.0.2.tar`

### file list

```diff
@@ -1,61 +1,62 @@
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-01 03:16:07.242584 swebench-1.0.1/
--rw-r--r--   0 johnbyang   (501) staff       (20)     1159 2024-04-01 03:02:22.000000 swebench-1.0.1/LICENSE
--rw-r--r--   0 johnbyang   (501) staff       (20)     6210 2024-04-01 03:16:07.242504 swebench-1.0.1/PKG-INFO
--rw-r--r--   0 johnbyang   (501) staff       (20)     5154 2024-03-14 23:15:56.000000 swebench-1.0.1/README.md
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-01 03:16:07.234831 swebench-1.0.1/inference/
--rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-03-14 17:15:25.000000 swebench-1.0.1/inference/__init__.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-01 03:16:07.235425 swebench-1.0.1/inference/llamao/
--rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-03-14 17:15:25.000000 swebench-1.0.1/inference/llamao/__init__.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     2491 2024-03-19 11:00:02.000000 swebench-1.0.1/inference/llamao/distributed_attention.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    37884 2024-03-19 11:00:02.000000 swebench-1.0.1/inference/llamao/modeling_flash_llama.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-01 03:16:07.236783 swebench-1.0.1/inference/make_datasets/
--rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-03-14 17:15:25.000000 swebench-1.0.1/inference/make_datasets/__init__.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    18785 2024-03-19 11:00:02.000000 swebench-1.0.1/inference/make_datasets/bm25_retrieval.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    14957 2024-03-14 17:15:25.000000 swebench-1.0.1/inference/make_datasets/create_instance.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     8534 2024-03-19 11:00:02.000000 swebench-1.0.1/inference/make_datasets/create_text_dataset.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     2618 2024-03-19 11:00:02.000000 swebench-1.0.1/inference/make_datasets/eval_retrieval.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     7717 2024-03-19 11:00:02.000000 swebench-1.0.1/inference/make_datasets/tokenize_dataset.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    10607 2024-03-19 11:00:02.000000 swebench-1.0.1/inference/make_datasets/utils.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)    19671 2024-03-28 15:18:33.000000 swebench-1.0.1/inference/run_api.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)    10090 2024-03-28 15:18:33.000000 swebench-1.0.1/inference/run_live.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    15798 2024-03-14 17:15:25.000000 swebench-1.0.1/inference/run_llama.py
--rw-r--r--   0 johnbyang   (501) staff       (20)       84 2024-04-01 03:02:22.000000 swebench-1.0.1/pyproject.toml
--rw-r--r--   0 johnbyang   (501) staff       (20)      111 2024-04-01 03:16:07.242792 swebench-1.0.1/setup.cfg
--rw-r--r--   0 johnbyang   (501) staff       (20)     1329 2024-04-01 03:15:29.000000 swebench-1.0.1/setup.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-01 03:16:07.236947 swebench-1.0.1/swebench/
--rw-r--r--   0 johnbyang   (501) staff       (20)     1672 2024-04-01 03:15:43.000000 swebench-1.0.1/swebench/__init__.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-01 03:16:07.238482 swebench-1.0.1/swebench/collect/
--rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-01 03:02:22.000000 swebench-1.0.1/swebench/collect/__init__.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     6693 2024-04-01 03:02:22.000000 swebench-1.0.1/swebench/collect/build_dataset.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     2677 2024-04-01 03:02:22.000000 swebench-1.0.1/swebench/collect/build_dataset_ft.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     4633 2024-04-01 03:02:22.000000 swebench-1.0.1/swebench/collect/get_tasks_pipeline.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     3671 2024-04-01 03:02:22.000000 swebench-1.0.1/swebench/collect/get_top_pypi.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     1751 2024-04-01 03:02:22.000000 swebench-1.0.1/swebench/collect/print_pulls.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    14635 2024-04-01 03:02:22.000000 swebench-1.0.1/swebench/collect/utils.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-01 03:16:07.240002 swebench-1.0.1/swebench/harness/
--rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-01 03:02:22.000000 swebench-1.0.1/swebench/harness/__init__.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    18925 2024-04-01 03:05:16.000000 swebench-1.0.1/swebench/harness/constants.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    30156 2024-04-01 03:10:55.000000 swebench-1.0.1/swebench/harness/context_manager.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     7478 2024-04-01 03:07:22.000000 swebench-1.0.1/swebench/harness/engine_evaluation.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     6331 2024-04-01 03:07:49.000000 swebench-1.0.1/swebench/harness/engine_validation.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)    11060 2024-04-01 03:02:22.000000 swebench-1.0.1/swebench/harness/run_evaluation.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    14820 2024-04-01 03:09:44.000000 swebench-1.0.1/swebench/harness/utils.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-01 03:16:07.241176 swebench-1.0.1/swebench/metrics/
--rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-01 03:02:22.000000 swebench-1.0.1/swebench/metrics/__init__.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     2131 2024-04-01 03:02:22.000000 swebench-1.0.1/swebench/metrics/conversion.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     3850 2024-04-01 03:02:22.000000 swebench-1.0.1/swebench/metrics/getters.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     5832 2024-04-01 03:02:22.000000 swebench-1.0.1/swebench/metrics/log_parsers.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     2969 2024-04-01 03:02:22.000000 swebench-1.0.1/swebench/metrics/metrics.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     4244 2024-04-01 03:02:22.000000 swebench-1.0.1/swebench/metrics/monitor.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    10627 2024-04-01 03:02:22.000000 swebench-1.0.1/swebench/metrics/report.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-01 03:16:07.242062 swebench-1.0.1/swebench/versioning/
--rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-01 03:02:22.000000 swebench-1.0.1/swebench/versioning/__init__.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     2214 2024-04-01 03:02:22.000000 swebench-1.0.1/swebench/versioning/constants.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    15492 2024-04-01 03:02:22.000000 swebench-1.0.1/swebench/versioning/get_versions.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     1221 2024-04-01 03:02:22.000000 swebench-1.0.1/swebench/versioning/utils.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-01 03:16:07.242231 swebench-1.0.1/swebench.egg-info/
--rw-r--r--   0 johnbyang   (501) staff       (20)     6210 2024-04-01 03:16:07.000000 swebench-1.0.1/swebench.egg-info/PKG-INFO
--rw-r--r--   0 johnbyang   (501) staff       (20)     1524 2024-04-01 03:16:07.000000 swebench-1.0.1/swebench.egg-info/SOURCES.txt
--rw-r--r--   0 johnbyang   (501) staff       (20)        1 2024-04-01 03:16:07.000000 swebench-1.0.1/swebench.egg-info/dependency_links.txt
--rw-r--r--   0 johnbyang   (501) staff       (20)       76 2024-04-01 03:16:07.000000 swebench-1.0.1/swebench.egg-info/requires.txt
--rw-r--r--   0 johnbyang   (501) staff       (20)       19 2024-04-01 03:16:07.000000 swebench-1.0.1/swebench.egg-info/top_level.txt
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-02 13:57:35.986966 swebench-1.0.2/
+-rw-r--r--   0 johnbyang   (501) staff       (20)     1159 2024-04-02 05:16:15.000000 swebench-1.0.2/LICENSE
+-rw-r--r--   0 johnbyang   (501) staff       (20)     6326 2024-04-02 13:57:35.986887 swebench-1.0.2/PKG-INFO
+-rw-r--r--   0 johnbyang   (501) staff       (20)     5270 2024-04-02 05:49:19.000000 swebench-1.0.2/README.md
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-02 13:57:35.977476 swebench-1.0.2/inference/
+-rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-03-14 17:15:25.000000 swebench-1.0.2/inference/__init__.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-02 13:57:35.978031 swebench-1.0.2/inference/llamao/
+-rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-03-14 17:15:25.000000 swebench-1.0.2/inference/llamao/__init__.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     2491 2024-03-19 11:00:02.000000 swebench-1.0.2/inference/llamao/distributed_attention.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    37884 2024-03-19 11:00:02.000000 swebench-1.0.2/inference/llamao/modeling_flash_llama.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-02 13:57:35.979527 swebench-1.0.2/inference/make_datasets/
+-rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-03-14 17:15:25.000000 swebench-1.0.2/inference/make_datasets/__init__.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    18785 2024-03-19 11:00:02.000000 swebench-1.0.2/inference/make_datasets/bm25_retrieval.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    14957 2024-03-14 17:15:25.000000 swebench-1.0.2/inference/make_datasets/create_instance.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     8534 2024-03-19 11:00:02.000000 swebench-1.0.2/inference/make_datasets/create_text_dataset.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     2618 2024-03-19 11:00:02.000000 swebench-1.0.2/inference/make_datasets/eval_retrieval.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     7717 2024-03-19 11:00:02.000000 swebench-1.0.2/inference/make_datasets/tokenize_dataset.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    10607 2024-03-19 11:00:02.000000 swebench-1.0.2/inference/make_datasets/utils.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)    19671 2024-03-28 15:18:33.000000 swebench-1.0.2/inference/run_api.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)    10090 2024-03-28 15:18:33.000000 swebench-1.0.2/inference/run_live.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    15798 2024-03-14 17:15:25.000000 swebench-1.0.2/inference/run_llama.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)       84 2024-04-02 05:16:15.000000 swebench-1.0.2/pyproject.toml
+-rw-r--r--   0 johnbyang   (501) staff       (20)      111 2024-04-02 13:57:35.987229 swebench-1.0.2/setup.cfg
+-rw-r--r--   0 johnbyang   (501) staff       (20)     1329 2024-04-02 05:16:15.000000 swebench-1.0.2/setup.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-02 13:57:35.979815 swebench-1.0.2/swebench/
+-rw-r--r--   0 johnbyang   (501) staff       (20)     1691 2024-04-02 13:57:17.000000 swebench-1.0.2/swebench/__init__.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-02 13:57:35.982137 swebench-1.0.2/swebench/collect/
+-rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.0.2/swebench/collect/__init__.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     6693 2024-04-02 05:16:15.000000 swebench-1.0.2/swebench/collect/build_dataset.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     2677 2024-04-02 05:16:15.000000 swebench-1.0.2/swebench/collect/build_dataset_ft.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     4633 2024-04-02 05:16:15.000000 swebench-1.0.2/swebench/collect/get_tasks_pipeline.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     3671 2024-04-02 05:16:15.000000 swebench-1.0.2/swebench/collect/get_top_pypi.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     1751 2024-04-02 05:16:15.000000 swebench-1.0.2/swebench/collect/print_pulls.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    14635 2024-04-02 05:16:15.000000 swebench-1.0.2/swebench/collect/utils.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-02 13:57:35.983705 swebench-1.0.2/swebench/harness/
+-rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.0.2/swebench/harness/__init__.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    18925 2024-04-02 05:16:15.000000 swebench-1.0.2/swebench/harness/constants.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    30156 2024-04-02 05:16:15.000000 swebench-1.0.2/swebench/harness/context_manager.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     7478 2024-04-02 05:16:15.000000 swebench-1.0.2/swebench/harness/engine_evaluation.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     6331 2024-04-02 05:16:15.000000 swebench-1.0.2/swebench/harness/engine_validation.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)    10392 2024-04-02 13:57:05.000000 swebench-1.0.2/swebench/harness/run_evaluation.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    14820 2024-04-02 05:16:15.000000 swebench-1.0.2/swebench/harness/utils.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-02 13:57:35.985262 swebench-1.0.2/swebench/metrics/
+-rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.0.2/swebench/metrics/__init__.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)      730 2024-04-02 05:16:15.000000 swebench-1.0.2/swebench/metrics/constants.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     2178 2024-04-02 05:16:15.000000 swebench-1.0.2/swebench/metrics/conversion.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     4625 2024-04-02 13:57:05.000000 swebench-1.0.2/swebench/metrics/getters.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     5746 2024-04-02 05:16:15.000000 swebench-1.0.2/swebench/metrics/log_parsers.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     2829 2024-04-02 05:16:15.000000 swebench-1.0.2/swebench/metrics/metrics.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     4338 2024-04-02 05:16:15.000000 swebench-1.0.2/swebench/metrics/monitor.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    10931 2024-04-02 13:57:05.000000 swebench-1.0.2/swebench/metrics/report.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-02 13:57:35.986306 swebench-1.0.2/swebench/versioning/
+-rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.0.2/swebench/versioning/__init__.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     2214 2024-04-02 05:16:15.000000 swebench-1.0.2/swebench/versioning/constants.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    15492 2024-04-02 05:16:15.000000 swebench-1.0.2/swebench/versioning/get_versions.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     1221 2024-04-02 05:16:15.000000 swebench-1.0.2/swebench/versioning/utils.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-02 13:57:35.986581 swebench-1.0.2/swebench.egg-info/
+-rw-r--r--   0 johnbyang   (501) staff       (20)     6326 2024-04-02 13:57:35.000000 swebench-1.0.2/swebench.egg-info/PKG-INFO
+-rw-r--r--   0 johnbyang   (501) staff       (20)     1543 2024-04-02 13:57:35.000000 swebench-1.0.2/swebench.egg-info/SOURCES.txt
+-rw-r--r--   0 johnbyang   (501) staff       (20)        1 2024-04-02 13:57:35.000000 swebench-1.0.2/swebench.egg-info/dependency_links.txt
+-rw-r--r--   0 johnbyang   (501) staff       (20)       76 2024-04-02 13:57:35.000000 swebench-1.0.2/swebench.egg-info/requires.txt
+-rw-r--r--   0 johnbyang   (501) staff       (20)       19 2024-04-02 13:57:35.000000 swebench-1.0.2/swebench.egg-info/top_level.txt
```

### Comparing `swebench-1.0.1/LICENSE` & `swebench-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `swebench-1.0.1/PKG-INFO` & `swebench-1.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swebench
-Version: 1.0.1
+Version: 1.0.2
 Summary: The official SWE-bench package - a benchmark for evaluating LMs on software engineering
 Home-page: https://swebench.com
 Author: John Yang
 Author-email: byjohnyang@gmail.com
 Project-URL: Documentation, https://github.com/princeton-nlp/SWE-bench
 Project-URL: Bug Reports, http://github.com/princeton-nlp/SWE-bench/issues
 Project-URL: Source Code, http://github.com/princeton-nlp/SWE-bench
@@ -47,14 +47,17 @@
     </br>
     <a href="https://www.python.org/">
         <img alt="Build" src="https://img.shields.io/badge/Python-3.8+-1f425f.svg?color=purple">
     </a>
     <a href="https://copyright.princeton.edu/policy">
         <img alt="License" src="https://img.shields.io/badge/License-MIT-blue">
     </a>
+    <a href="https://badge.fury.io/py/swebench">
+        <img src="https://badge.fury.io/py/swebench.svg">
+    </a>
 </p>
 
 Please refer our [website](http://swe-bench.github.io) for the public leaderboard and the [change log](https://github.com/princeton-nlp/SWE-bench/blob/master/CHANGELOG.md) for information on the latest updates to the SWE-bench benchmark.
 
 ## 👋 Overview
 SWE-bench is a benchmark for evaluating large language models on real world software issues collected from GitHub.
 Given a *codebase* and an *issue*, a language model is tasked with generating a *patch* that resolves the described problem.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: swebench Version: 1.0.1 Summary: The official SWE-
+Metadata-Version: 2.1 Name: swebench Version: 1.0.2 Summary: The official SWE-
 bench package - a benchmark for evaluating LMs on software engineering Home-
 page: https://swebench.com Author: John Yang Author-email: byjohnyang@gmail.com
 Project-URL: Documentation, https://github.com/princeton-nlp/SWE-bench Project-
 URL: Bug Reports, http://github.com/princeton-nlp/SWE-bench/issues Project-URL:
 Source Code, http://github.com/princeton-nlp/SWE-bench Project-URL: Website,
 https://swebench.com Keywords: nlp,benchmark,code Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
@@ -13,15 +13,16 @@
 datasets Requires-Dist: ghapi Requires-Dist: GitPython Requires-Dist: python-
 dotenv Requires-Dist: requests Requires-Dist: rich
                              _[_K_a_w_i_ _t_h_e_ _S_W_E_-_L_l_a_m_a_]
 | [æ¥æ¬èª](docs/README_JP.md) | [English](https://github.com/princeton-nlp/
                                  SWE-bench) |
 ---
  Code and data for our ICLR 2024 paper _S_W_E_-_b_e_n_c_h_:_ _C_a_n_ _L_a_n_g_u_a_g_e_ _M_o_d_e_l_s_ _R_e_s_o_l_v_e
-                   _R_e_a_l_-_W_o_r_l_d_ _G_i_t_H_u_b_ _I_s_s_u_e_s_?_[_B_u_i_l_d_]_[_L_i_c_e_n_s_e_]
+      _R_e_a_l_-_W_o_r_l_d_ _G_i_t_H_u_b_ _I_s_s_u_e_s_?_[_B_u_i_l_d_]_[_L_i_c_e_n_s_e_]_[_h_t_t_p_s_:_/_/_b_a_d_g_e_._f_u_r_y_._i_o_/_p_y_/
+                                 _s_w_e_b_e_n_c_h_._s_v_g_]
 Please refer our [website](http://swe-bench.github.io) for the public
 leaderboard and the [change log](https://github.com/princeton-nlp/SWE-bench/
 blob/master/CHANGELOG.md) for information on the latest updates to the SWE-
 bench benchmark. ## ð Overview SWE-bench is a benchmark for evaluating large
 language models on real world software issues collected from GitHub. Given a
 *codebase* and an *issue*, a language model is tasked with generating a *patch*
 that resolves the described problem. [assets/teaser.png]## ð Set Up To build
```

### Comparing `swebench-1.0.1/README.md` & `swebench-1.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,17 @@
     </br>
     <a href="https://www.python.org/">
         <img alt="Build" src="https://img.shields.io/badge/Python-3.8+-1f425f.svg?color=purple">
     </a>
     <a href="https://copyright.princeton.edu/policy">
         <img alt="License" src="https://img.shields.io/badge/License-MIT-blue">
     </a>
+    <a href="https://badge.fury.io/py/swebench">
+        <img src="https://badge.fury.io/py/swebench.svg">
+    </a>
 </p>
 
 Please refer our [website](http://swe-bench.github.io) for the public leaderboard and the [change log](https://github.com/princeton-nlp/SWE-bench/blob/master/CHANGELOG.md) for information on the latest updates to the SWE-bench benchmark.
 
 ## 👋 Overview
 SWE-bench is a benchmark for evaluating large language models on real world software issues collected from GitHub.
 Given a *codebase* and an *issue*, a language model is tasked with generating a *patch* that resolves the described problem.
```

#### html2text {}

```diff
@@ -1,13 +1,14 @@
                              _[_K_a_w_i_ _t_h_e_ _S_W_E_-_L_l_a_m_a_]
 | [æ¥æ¬èª](docs/README_JP.md) | [English](https://github.com/princeton-nlp/
                                  SWE-bench) |
 ---
  Code and data for our ICLR 2024 paper _S_W_E_-_b_e_n_c_h_:_ _C_a_n_ _L_a_n_g_u_a_g_e_ _M_o_d_e_l_s_ _R_e_s_o_l_v_e
-                   _R_e_a_l_-_W_o_r_l_d_ _G_i_t_H_u_b_ _I_s_s_u_e_s_?_[_B_u_i_l_d_]_[_L_i_c_e_n_s_e_]
+      _R_e_a_l_-_W_o_r_l_d_ _G_i_t_H_u_b_ _I_s_s_u_e_s_?_[_B_u_i_l_d_]_[_L_i_c_e_n_s_e_]_[_h_t_t_p_s_:_/_/_b_a_d_g_e_._f_u_r_y_._i_o_/_p_y_/
+                                 _s_w_e_b_e_n_c_h_._s_v_g_]
 Please refer our [website](http://swe-bench.github.io) for the public
 leaderboard and the [change log](https://github.com/princeton-nlp/SWE-bench/
 blob/master/CHANGELOG.md) for information on the latest updates to the SWE-
 bench benchmark. ## ð Overview SWE-bench is a benchmark for evaluating large
 language models on real world software issues collected from GitHub. Given a
 *codebase* and an *issue*, a language model is tasked with generating a *patch*
 that resolves the described problem. [assets/teaser.png]## ð Set Up To build
```

### Comparing `swebench-1.0.1/inference/llamao/distributed_attention.py` & `swebench-1.0.2/inference/llamao/distributed_attention.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.1/inference/llamao/modeling_flash_llama.py` & `swebench-1.0.2/inference/llamao/modeling_flash_llama.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.1/inference/make_datasets/bm25_retrieval.py` & `swebench-1.0.2/inference/make_datasets/bm25_retrieval.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.1/inference/make_datasets/create_instance.py` & `swebench-1.0.2/inference/make_datasets/create_instance.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.1/inference/make_datasets/create_text_dataset.py` & `swebench-1.0.2/inference/make_datasets/create_text_dataset.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.1/inference/make_datasets/eval_retrieval.py` & `swebench-1.0.2/inference/make_datasets/eval_retrieval.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.1/inference/make_datasets/tokenize_dataset.py` & `swebench-1.0.2/inference/make_datasets/tokenize_dataset.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.1/inference/make_datasets/utils.py` & `swebench-1.0.2/inference/make_datasets/utils.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.1/inference/run_api.py` & `swebench-1.0.2/inference/run_api.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.1/inference/run_live.py` & `swebench-1.0.2/inference/run_live.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.1/inference/run_llama.py` & `swebench-1.0.2/inference/run_llama.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.1/setup.py` & `swebench-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.1/swebench/__init__.py` & `swebench-1.0.2/swebench/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.0.1"
+__version__ = "1.0.2"
 
 from swebench.collect.build_dataset import main as build_dataset
 from swebench.collect.get_tasks_pipeline import main as get_tasks_pipeline
 from swebench.collect.print_pulls import main as print_pulls
 
 from swebench.harness.constants import (
     KEY_INSTANCE_ID,
@@ -26,14 +26,15 @@
     convert_log_to_ground_truth
 )
 
 from swebench.metrics.getters import (
     get_diffs,
     get_logs_eval,
     get_logs_gold,
+    get_eval_refs,
 )
 
 from swebench.metrics.log_parsers import (
     MAP_REPO_TO_PARSER,
 )
 
 from swebench.metrics.metrics import (
```

### Comparing `swebench-1.0.1/swebench/collect/build_dataset.py` & `swebench-1.0.2/swebench/collect/build_dataset.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.1/swebench/collect/build_dataset_ft.py` & `swebench-1.0.2/swebench/collect/build_dataset_ft.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.1/swebench/collect/get_tasks_pipeline.py` & `swebench-1.0.2/swebench/collect/get_tasks_pipeline.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.1/swebench/collect/get_top_pypi.py` & `swebench-1.0.2/swebench/collect/get_top_pypi.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.1/swebench/collect/print_pulls.py` & `swebench-1.0.2/swebench/collect/print_pulls.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.1/swebench/collect/utils.py` & `swebench-1.0.2/swebench/collect/utils.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.1/swebench/harness/constants.py` & `swebench-1.0.2/swebench/harness/constants.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.1/swebench/harness/context_manager.py` & `swebench-1.0.2/swebench/harness/context_manager.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.1/swebench/harness/engine_evaluation.py` & `swebench-1.0.2/swebench/harness/engine_evaluation.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.1/swebench/harness/engine_validation.py` & `swebench-1.0.2/swebench/harness/engine_validation.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.1/swebench/harness/run_evaluation.py` & `swebench-1.0.2/swebench/harness/run_evaluation.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from swebench.harness.constants import (
     KEY_INSTANCE_ID,
     KEY_MODEL,
     KEY_PREDICTION,
 )
 from swebench.harness.engine_evaluation import main as eval_engine
 from swebench.harness.utils import get_instances
+from swebench.metrics.getters import get_eval_refs
 
 logging.basicConfig(
     level=logging.INFO, format="%(asctime)s - %(levelname)s - %(message)s"
 )
 logger = logging.getLogger("run_evaluation")
 
 
@@ -69,48 +70,31 @@
     num_processes: int = -1,
 ):
     """
     Runs evaluation on predictions for each model/repo/version combination.
 
     Args:
         predictions_path (str): Path to the predictions file.
-        swe_bench_tasks (str): Path to the SWE-bench tasks file OR [dev|test].
+        swe_bench_tasks (str): Path to the SWE-bench tasks file OR HF dataset name.
         log_dir (str): Path to the directory where logs will be saved.
         testbed (str): Path to the directory where testbeds will be saved.
         skip_existing (bool): Whether to skip evaluations for predictions that already have logs.
         timeout (int): Timeout for each evaluation.
         verbose (bool): Whether to print verbose output.
 
     Raises:
         ValueError: If log_dir is not a directory, testbed is not a directory, or swe_bench_tasks does not exist.
     """
     # Validate arguments
     if not os.path.exists(log_dir) or not os.path.isdir(log_dir):
         raise ValueError("--log_dir must exist and point at a directory")
     if not os.path.exists(testbed) or not os.path.isdir(testbed):
         raise ValueError("--testbed must exist and point at a directory")
-
-    if not os.path.exists(swe_bench_tasks) and swe_bench_tasks not in ["dev", "test"]:
-        raise ValueError("--swe_bench_tasks does not exist OR is not [dev|test]")
-
-    tasks = None
-    if os.path.exists(swe_bench_tasks):
-        # If local path is provided, load from path
-        tasks = json.load(open(os.path.abspath(swe_bench_tasks)))
-    else:
-        # If dev/test split is provided, load from HuggingFace datasets
-        temp = load_dataset('princeton-nlp/SWE-bench', split=swe_bench_tasks)
-        assert(temp, datasets.arrow_dataset.Dataset)
-        temp = temp.to_dict()
-        tasks = []
-        for idx in range(len(temp[KEY_INSTANCE_ID])):
-            task_instance = {}
-            for k in temp.keys():
-                task_instance[k] = temp[k][idx]
-            tasks.append(task_instance)
+    
+    tasks = list(get_eval_refs(swe_bench_tasks).values())
 
     # Verify arguments are formatted correctly
     if not isinstance(tasks, list):
         raise ValueError(f"{swe_bench_tasks} must contain an array of tasks")
     tasks_map = {t[KEY_INSTANCE_ID]: t for t in tasks}
     predictions_path = os.path.abspath(predictions_path)
     validate_predictions(predictions_path, [t[KEY_INSTANCE_ID] for t in tasks])
@@ -219,24 +203,24 @@
             pool.map(eval_engine, eval_args)
             pool.close()
             pool.join()
     finally:
         # Clean up
         for temp_dir in temp_dirs:
             # Kill all processes that are using the temp directory
-            subprocess.run(f"lsof +D {temp_dir} | awk 'NR>1 {{print $2}}' | xargs kill".split())
+            subprocess.run(f"lsof +D {temp_dir} | awk 'NR>1 {{print $2}}' | xargs kill", shell=True, capture_output=True)
             # Remove temp directory
             shutil.rmtree(temp_dir, ignore_errors=True)
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(description=__doc__)
     parser.add_argument("--predictions_path", type=str, help="Path to predictions file (must be .json)", required=True)
     parser.add_argument("--log_dir", type=str, help="Path to log directory", required=True)
-    parser.add_argument("--swe_bench_tasks", type=str, help="Path to SWE-bench task instances file", required=True)
+    parser.add_argument("--swe_bench_tasks", type=str, help="Path to dataset file or HF datasets name", required=True)
     parser.add_argument("--testbed", type=str, help="Path to testbed directory", required=True)
     parser.add_argument("--conda_link", type=str, default=None, help="(Optional) URL to conda installation to use")
     parser.add_argument("--log_suffix", type=str, help="(Optional) Suffix to append to log file names", default=None)
     parser.add_argument("--skip_existing", action="store_true", help="(Optional) Skip existing logs")
     parser.add_argument("--timeout", type=int, help="(Optional) Timeout in seconds (default: 900)", default=900)
     parser.add_argument("--verbose", action="store_true", help="(Optional) Verbose mode")
     parser.add_argument("--num_processes", type=int, help="(Optional) Number of processes to use.", default=-1)
```

### Comparing `swebench-1.0.1/swebench/harness/utils.py` & `swebench-1.0.2/swebench/harness/utils.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.1/swebench/metrics/conversion.py` & `swebench-1.0.2/swebench/metrics/conversion.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 import json, os
 
-from swebench.metrics.log_parsers import MAP_REPO_TO_PARSER, TestStatus
-from swebench.metrics.getters import (
-    get_file_name_from_lp,
-    get_repo_from_lp,
-    log_path_to_sms,
+from swebench.metrics.constants import (
     FAIL_TO_PASS,
     FAIL_TO_FAIL,
     PASS_TO_PASS,
     PASS_TO_FAIL,
+    TestStatus,
+)
+from swebench.metrics.getters import (
+    get_file_name_from_lp,
+    get_repo_from_lp,
+    log_path_to_sms,
     test_failed,
     test_passed,
 )
+from swebench.metrics.log_parsers import MAP_REPO_TO_PARSER
 
 
 def convert_log_to_ground_truth(
     log_fp: list, save_dir: str = None, verbose: bool = False
 ) -> dict:
     """
     Convert log file generated from check instances into ground truth dict
```

### Comparing `swebench-1.0.1/swebench/metrics/getters.py` & `swebench-1.0.2/swebench/metrics/getters.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 import re
-
+import json
+import os
+from datasets import load_from_disk, load_dataset
+
+from swebench.metrics.constants import (
+    APPLY_PATCH_FAIL,
+    APPLY_PATCH_PASS,
+    RESET_FAILED,
+    TESTS_ERROR,
+    TESTS_TIMEOUT,
+)
+from swebench.harness.constants import KEY_INSTANCE_ID
 from swebench.metrics.log_parsers import MAP_REPO_TO_PARSER, TestStatus
-
-
-# Evaluation Log Constants
-APPLY_PATCH_FAIL = ">>>>> Patch Apply Failed"
-APPLY_PATCH_PASS = ">>>>> Applied Patch"
-INSTALL_FAIL = ">>>>> Init Failed"
-INSTALL_PASS = ">>>>> Init Succeeded"
-RESET_FAILED = ">>>>> Reset Failed"
-TESTS_TIMEOUT = ">>>>> Tests Timed Out"
-TESTS_ERROR = ">>>>> Tests Errored"
-
-# Result Categories
-FAIL_TO_PASS = "FAIL_TO_PASS"
-FAIL_TO_FAIL = "FAIL_TO_FAIL"
-PASS_TO_PASS = "PASS_TO_PASS"
-PASS_TO_FAIL = "PASS_TO_FAIL"
+from typing import Tuple
 
 
 def get_diffs(sm_1: dict, sm_2: dict) -> dict:
     """
     Get differences between two test status maps
 
     Args:
@@ -37,15 +33,15 @@
     for diff in diffs:
         if diff[0] not in diff_map:
             diff_map[diff[0]] = []
         diff_map[diff[0]].append(diff[1])
     return diff_map
 
 
-def get_logs_eval(log_fp: str) -> (dict, bool):
+def get_logs_eval(log_fp: str) -> Tuple[dict, bool]:
     """
     Retrieve evaluation results for a task instance from its corresponding log file
 
     Args:
         log_fp (str): path to log file
     Returns:
         bool: whether the patch applied successfully
@@ -61,15 +57,15 @@
             return {}, False
 
         # Get status map of evaluation results
         content = content.split(f"{APPLY_PATCH_PASS} (pred)")[-1]
         return log_parser(content), True
 
 
-def get_logs_gold(log_fp: str) -> (str, str):
+def get_logs_gold(log_fp: str) -> Tuple[str, str]:
     """
     Retrieve pre-patch, post-patch test logs from a validation log file
 
     Args:
         log_fp (str): path to log file
     Returns:
         str: pre-patch, post-patch test logs
@@ -88,15 +84,15 @@
 
 get_id_from_lp = lambda x: get_file_name_from_lp(x).split(".")[0]
 
 
 get_repo_from_lp = lambda x: get_id_from_lp(x).rsplit("-", 1)[0].replace("__", "/")
 
 
-def log_path_to_sms(log_fp: str, log_parser) -> (list, bool):
+def log_path_to_sms(log_fp: str, log_parser) -> Tuple[list, bool]:
     """
     Wrapper for getting log data from log_parser file
 
     Args:
         log_fp (str): path to log file
         log_parser (function): function to parse log file
     Returns:
@@ -124,7 +120,33 @@
 
 
 test_passed = lambda case, sm: case in sm and sm[case] == TestStatus.PASSED.value
 
 test_failed = lambda case, sm: case not in sm or any(
     [sm[case] == status for status in [TestStatus.FAILED.value, TestStatus.ERROR.value]]
 )
+
+
+def get_eval_refs(data_path_or_name):
+    decode_keys = False
+    if os.path.isfile(data_path_or_name):
+        if data_path_or_name.endswith(".jsonl"):
+            data = [json.loads(l) for l in open(data_path_or_name).readlines()]
+        elif data_path_or_name.endswith(".json"):
+            data = json.load(open(data_path_or_name, "r"))
+    elif os.path.isdir(data_path_or_name):
+        data = load_from_disk(data_path_or_name)
+        decode_keys = True
+    else:
+        data = load_dataset(data_path_or_name)
+        decode_keys = True
+    if isinstance(data, dict):
+        all_data = list()
+        for split in data.keys():
+            all_data.extend(data[split])
+        data = all_data
+    if decode_keys:
+        for datum in data:
+            for key in ["PASS_TO_PASS", "FAIL_TO_PASS"]:
+                datum[key] = json.loads(datum[key])
+    return {d[KEY_INSTANCE_ID]: d for d in data}
+
```

### Comparing `swebench-1.0.1/swebench/metrics/log_parsers.py` & `swebench-1.0.2/swebench/metrics/log_parsers.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,10 @@
 import re
 
-from enum import Enum
-
-
-class TestStatus(Enum):
-    FAILED = "FAILED"
-    PASSED = "PASSED"
-    SKIPPED = "SKIPPED"
-    ERROR = "ERROR"
+from swebench.metrics.constants import TestStatus
 
 
 def parse_log_pytest(log: str) -> dict:
     """
     Parser for test logs generated with PyTest framework
 
     Args:
```

### Comparing `swebench-1.0.1/swebench/metrics/metrics.py` & `swebench-1.0.2/swebench/metrics/metrics.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,15 @@
-from enum import Enum
 from statistics import mean
-from swebench.metrics.getters import (
-    FAIL_TO_FAIL, FAIL_TO_PASS,
-    PASS_TO_FAIL, PASS_TO_PASS,
+from swebench.metrics.constants import (
+    FAIL_TO_PASS,
+    PASS_TO_PASS,
+    ResolvedStatus,
 )
 
 
-class ResolvedStatus(Enum):
-    NO = "RESOLVED_NO"
-    PARTIAL = "RESOLVED_PARTIAL"
-    FULL = "RESOLVED_FULL"
-
-
 def compute_fail_to_pass(report: dict) -> float:
     """
     Compute fail-to-pass metric. Accepts single report as argument.
     """
     total = len(report[FAIL_TO_PASS]["success"]) + len(report[FAIL_TO_PASS]["failure"])
     if total == 0:
         return 1
@@ -90,8 +84,8 @@
     p2p = compute_pass_to_pass(report)
 
     if f2p == 1 and p2p == 1:
         return ResolvedStatus.FULL.value
     elif f2p < 1 and f2p > 0 and p2p == 1:
         return ResolvedStatus.PARTIAL.value
     else:
-        return ResolvedStatus.NO.value
+        return ResolvedStatus.NO.value
```

### Comparing `swebench-1.0.1/swebench/metrics/monitor.py` & `swebench-1.0.2/swebench/metrics/monitor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 import glob
 import os
 
+from swebench.metrics.constants import (
+    APPLY_PATCH_FAIL,
+    APPLY_PATCH_PASS,
+    TESTS_TIMEOUT
+)
 from swebench.metrics.getters import (
-    log_path_to_sms, get_diffs, get_repo_from_lp,
-    APPLY_PATCH_FAIL, APPLY_PATCH_PASS, TESTS_TIMEOUT
+    log_path_to_sms,
+    get_diffs,
+    get_repo_from_lp,
 )
 from swebench.metrics.log_parsers import MAP_REPO_TO_PARSER
+from typing import Tuple
 
 
 def monitor_validation(
     path_to_logs: str, log_prefix: str = None
-) -> (list, list, list, list):
+) -> Tuple[list, list, list, list]:
     """
     Check log files generated from a `check_instances` run to see how many instances were successfully
     installed and/or tested.
 
     Args:
         path_to_logs (str): path to log files
         log_prefix (str): prefix of log files
@@ -75,15 +82,15 @@
         + len(timeout)
         == count
     )
 
     return failed_install, corrupt_test_patch, corrupt_patch, timeout, success
 
 
-def monitor_logs_same_diff(log_dir: str, repo: str = None) -> (list, list):
+def monitor_logs_same_diff(log_dir: str, repo: str = None) -> Tuple[list, list]:
     """
     Given a log directory and repo, return a list of logs where pre-test
     and post-test logs are same/different
 
     Args:
         log_dir (str): path to log files
         repo (str): repo name
```

### Comparing `swebench-1.0.1/swebench/metrics/report.py` & `swebench-1.0.2/swebench/metrics/report.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,37 @@
 import glob, json, os
 
 from collections import Counter
-from swebench.metrics.getters import (
-    get_file_name_from_lp,
-    get_logs_eval,
-    get_id_from_lp,
+from swebench.harness.constants import (
+    INSTALL_FAIL,
+    KEY_INSTANCE_ID,
+)
+from swebench.metrics.constants import (
     FAIL_TO_FAIL,
     FAIL_TO_PASS,
     PASS_TO_FAIL,
     PASS_TO_PASS,
+)
+from swebench.metrics.getters import (
+    get_file_name_from_lp,
+    get_logs_eval,
+    get_id_from_lp,
     test_failed,
     test_passed,
+    get_eval_refs,
 )
-from swebench.metrics.log_parsers import TestStatus
 from swebench.metrics.metrics import (
     compute_fail_to_pass_unweighted,
     compute_fail_to_pass_weighted,
     compute_pass_to_pass_unweighted,
     compute_pass_to_pass_weighted,
     get_resolution_status,
+    ResolvedStatus,
 )
+from typing import Tuple
 
 
 ### MARK - Eval Report Generation
 
 
 def get_eval_report(
     eval_sm: dict,
@@ -115,31 +123,30 @@
 
 
 def get_eval_reports_for_logs(
     eval_logs: list,
     swe_bench_tasks: str,
     callback: callable = None,
     verbose: bool = False,
-) -> (dict, dict):
+) -> Tuple[dict, dict]:
     """
     Wrapper for getting eval report for a list of evaluation log paths.
 
     Args:
         eval_logs (list): list of paths to evaluation logs
         swe_bench_tasks (str): path to eval task instances (swe-bench.json)
         callback (callable): callback function for evaluation logs
         verbose (bool): whether to print verbose output
     Returns:
         reports_patch_success (dict): dict of eval reports for patch apply successes
         reports_patch_failure (dict): dict of eval reports for patch apply failures
     """
     reports_patch_success = {}
     reports_patch_failure = {}
-    eval_refs = json.load(open(swe_bench_tasks))
-    eval_refs = {t['instance_id']: t for t in eval_refs}
+    eval_refs = get_eval_refs(swe_bench_tasks)
 
     for eval_log in eval_logs:
         # Remove task instances that do not satisfy callback
         if callback is not None and not callback(eval_log):
             continue
 
         # Get gold results
@@ -190,15 +197,15 @@
 
 
 def get_model_eval_summary(
     predicts_path: str,
     eval_dir: str,
     swe_bench_tasks: str,
     repo: str = None,
-):
+) -> dict:
     """
     Generate a summary of model evaluation results.
 
     Args:
         predicts_path (str): path to predictions file
         eval_dir (str): path to directory of evaluation logs
         swe_bench_tasks (str): path to eval references (swe-bench-eval-refs.json)
@@ -209,15 +216,15 @@
     with open(predicts_path) as f:
         for line in f.readlines():
             preds.append(json.loads(line))
 
     # Filter by repo if provided
     criteria_eval_sm = None
     if repo is not None:
-        criteria_pred = lambda pred: repo in pred["instance_id"]
+        criteria_pred = lambda pred: repo in pred[KEY_INSTANCE_ID]
         criteria_eval_sm = lambda eval_log: repo in eval_log
         preds = [x for x in preds if criteria_pred(x)]
 
     # Get reports
     reports_patch_success, reports_patch_failure = get_eval_reports_for_dir(
         eval_dir, swe_bench_tasks, callback=criteria_eval_sm, verbose=False
     )
@@ -253,70 +260,76 @@
         }
 
     return summary
 
 
 def get_model_report(
     model: str, predictions_path: str, swe_bench_tasks: str, log_dir: str
-):
+) -> dict:
     """
     Generate a report of model evaluation results from predictions, task instances,
     and evaluation logs.
 
     Args:
         model (str): model name
         predictions_path (str): path to predictions file
         swe_bench_tasks (str): path to eval references (swe-bench-eval-refs.json)
         log_dir (str): path to directory of evaluation logs
     Returns:
         report_map (dict): map of repo to report
     """
-    eval_refs = json.load(open(swe_bench_tasks))
-    eval_refs = [{key: t[key] for key in ["instance_id", "FAIL_TO_PASS", "PASS_TO_PASS"]} for t in eval_refs]
-    eval_refs = {t['instance_id']: t for t in eval_refs}
+    eval_refs = get_eval_refs(swe_bench_tasks)
+    for k, v in eval_refs.items():
+        eval_refs[k] = {key: v[key] for key in [KEY_INSTANCE_ID, FAIL_TO_PASS, PASS_TO_PASS]}
 
     # Get predictions
     predictions = []
     if predictions_path.endswith("jsonl"):
         with open(predictions_path) as f:
             for line in f.readlines():
                 predictions.append(json.loads(line))
     else:
         predictions = json.load(open(predictions_path))
     report_map = {}
 
     # Iterate through predictions
     for p in predictions:
-        repo = p["instance_id"].split(".")[0].rsplit("-", 1)[0].replace("__", "/")
+        repo = p[KEY_INSTANCE_ID].split(".")[0].rsplit("-", 1)[0].replace("__", "/")
         if repo not in report_map:
             report_map[repo] = {
                 "none": [],
                 "generated": [],
                 "with_logs": [],
+                "install_fail": [],
                 "applied": [],
                 "resolved": [],
             }
 
         # Check if the model patch exists
         if p["model_patch"] == None:
-            report_map[repo]["none"].append(p['instance_id'])
+            report_map[repo]["none"].append(p[KEY_INSTANCE_ID])
             continue
-        report_map[repo]["generated"].append(p['instance_id'])
+        report_map[repo]["generated"].append(p[KEY_INSTANCE_ID])
 
         # Get log file
-        log_path = os.path.join(log_dir, f"{p['instance_id']}.{model}.eval.log")
+        log_path = os.path.join(log_dir, f"{p[KEY_INSTANCE_ID]}.{model}.eval.log")
         if not os.path.exists(log_path):
             continue
-        report_map[repo]["with_logs"].append(p['instance_id'])
+        report_map[repo]["with_logs"].append(p[KEY_INSTANCE_ID])
+
+        # Check if install succeeded
+        if INSTALL_FAIL in open(log_path).read():
+            report_map[repo]["install_fail"].append(p[KEY_INSTANCE_ID])
+            continue
 
         # Get evaluation logs
         eval_sm, found = get_logs_eval(log_path)
 
         if not found:
             continue
-        report_map[repo]["applied"].append(p['instance_id'])
+        report_map[repo]["applied"].append(p[KEY_INSTANCE_ID])
 
-        report = get_eval_report(eval_sm, eval_refs[p["instance_id"]])
-        if get_resolution_status(report) == "RESOLVED_FULL":
-            report_map[repo]["resolved"].append(p['instance_id'])
+        report = get_eval_report(eval_sm, eval_refs[p[KEY_INSTANCE_ID]])
+        if get_resolution_status(report) == ResolvedStatus.FULL.value:
+            report_map[repo]["resolved"].append(p[KEY_INSTANCE_ID])
 
     return report_map
```

### Comparing `swebench-1.0.1/swebench/versioning/constants.py` & `swebench-1.0.2/swebench/versioning/constants.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.1/swebench/versioning/get_versions.py` & `swebench-1.0.2/swebench/versioning/get_versions.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.1/swebench/versioning/utils.py` & `swebench-1.0.2/swebench/versioning/utils.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.1/swebench.egg-info/PKG-INFO` & `swebench-1.0.2/swebench.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swebench
-Version: 1.0.1
+Version: 1.0.2
 Summary: The official SWE-bench package - a benchmark for evaluating LMs on software engineering
 Home-page: https://swebench.com
 Author: John Yang
 Author-email: byjohnyang@gmail.com
 Project-URL: Documentation, https://github.com/princeton-nlp/SWE-bench
 Project-URL: Bug Reports, http://github.com/princeton-nlp/SWE-bench/issues
 Project-URL: Source Code, http://github.com/princeton-nlp/SWE-bench
@@ -47,14 +47,17 @@
     </br>
     <a href="https://www.python.org/">
         <img alt="Build" src="https://img.shields.io/badge/Python-3.8+-1f425f.svg?color=purple">
     </a>
     <a href="https://copyright.princeton.edu/policy">
         <img alt="License" src="https://img.shields.io/badge/License-MIT-blue">
     </a>
+    <a href="https://badge.fury.io/py/swebench">
+        <img src="https://badge.fury.io/py/swebench.svg">
+    </a>
 </p>
 
 Please refer our [website](http://swe-bench.github.io) for the public leaderboard and the [change log](https://github.com/princeton-nlp/SWE-bench/blob/master/CHANGELOG.md) for information on the latest updates to the SWE-bench benchmark.
 
 ## 👋 Overview
 SWE-bench is a benchmark for evaluating large language models on real world software issues collected from GitHub.
 Given a *codebase* and an *issue*, a language model is tasked with generating a *patch* that resolves the described problem.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: swebench Version: 1.0.1 Summary: The official SWE-
+Metadata-Version: 2.1 Name: swebench Version: 1.0.2 Summary: The official SWE-
 bench package - a benchmark for evaluating LMs on software engineering Home-
 page: https://swebench.com Author: John Yang Author-email: byjohnyang@gmail.com
 Project-URL: Documentation, https://github.com/princeton-nlp/SWE-bench Project-
 URL: Bug Reports, http://github.com/princeton-nlp/SWE-bench/issues Project-URL:
 Source Code, http://github.com/princeton-nlp/SWE-bench Project-URL: Website,
 https://swebench.com Keywords: nlp,benchmark,code Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
@@ -13,15 +13,16 @@
 datasets Requires-Dist: ghapi Requires-Dist: GitPython Requires-Dist: python-
 dotenv Requires-Dist: requests Requires-Dist: rich
                              _[_K_a_w_i_ _t_h_e_ _S_W_E_-_L_l_a_m_a_]
 | [æ¥æ¬èª](docs/README_JP.md) | [English](https://github.com/princeton-nlp/
                                  SWE-bench) |
 ---
  Code and data for our ICLR 2024 paper _S_W_E_-_b_e_n_c_h_:_ _C_a_n_ _L_a_n_g_u_a_g_e_ _M_o_d_e_l_s_ _R_e_s_o_l_v_e
-                   _R_e_a_l_-_W_o_r_l_d_ _G_i_t_H_u_b_ _I_s_s_u_e_s_?_[_B_u_i_l_d_]_[_L_i_c_e_n_s_e_]
+      _R_e_a_l_-_W_o_r_l_d_ _G_i_t_H_u_b_ _I_s_s_u_e_s_?_[_B_u_i_l_d_]_[_L_i_c_e_n_s_e_]_[_h_t_t_p_s_:_/_/_b_a_d_g_e_._f_u_r_y_._i_o_/_p_y_/
+                                 _s_w_e_b_e_n_c_h_._s_v_g_]
 Please refer our [website](http://swe-bench.github.io) for the public
 leaderboard and the [change log](https://github.com/princeton-nlp/SWE-bench/
 blob/master/CHANGELOG.md) for information on the latest updates to the SWE-
 bench benchmark. ## ð Overview SWE-bench is a benchmark for evaluating large
 language models on real world software issues collected from GitHub. Given a
 *codebase* and an *issue*, a language model is tasked with generating a *patch*
 that resolves the described problem. [assets/teaser.png]## ð Set Up To build
```

### Comparing `swebench-1.0.1/swebench.egg-info/SOURCES.txt` & `swebench-1.0.2/swebench.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 setup.py
-./setup.py
 inference/__init__.py
 inference/run_api.py
 inference/run_live.py
 inference/run_llama.py
 inference/llamao/__init__.py
 inference/llamao/distributed_attention.py
 inference/llamao/modeling_flash_llama.py
@@ -35,14 +34,15 @@
 swebench/harness/constants.py
 swebench/harness/context_manager.py
 swebench/harness/engine_evaluation.py
 swebench/harness/engine_validation.py
 swebench/harness/run_evaluation.py
 swebench/harness/utils.py
 swebench/metrics/__init__.py
+swebench/metrics/constants.py
 swebench/metrics/conversion.py
 swebench/metrics/getters.py
 swebench/metrics/log_parsers.py
 swebench/metrics/metrics.py
 swebench/metrics/monitor.py
 swebench/metrics/report.py
 swebench/versioning/__init__.py
```

