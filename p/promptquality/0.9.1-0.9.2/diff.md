# Comparing `tmp/promptquality-0.9.1.tar.gz` & `tmp/promptquality-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptquality-0.9.1.tar", max compression
+gzip compressed data, was "promptquality-0.9.2.tar", max compression
```

## Comparing `promptquality-0.9.1.tar` & `promptquality-0.9.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0    10946 2023-09-14 01:15:15.670682 promptquality-0.9.1/LICENSE
--rw-r--r--   0        0        0      759 2023-09-14 01:15:15.670682 promptquality-0.9.1/README.md
--rw-r--r--   0        0        0     3252 2023-09-14 01:15:16.474694 promptquality-0.9.1/pyproject.toml
--rw-r--r--   0        0        0      659 2023-09-14 01:15:16.474694 promptquality-0.9.1/src/promptquality/__init__.py
--rw-r--r--   0        0        0        0 2023-09-14 01:15:15.670682 promptquality-0.9.1/src/promptquality/constants/__init__.py
--rw-r--r--   0        0        0      188 2023-09-14 01:15:15.670682 promptquality-0.9.1/src/promptquality/constants/config.py
--rw-r--r--   0        0        0       96 2023-09-14 01:15:15.670682 promptquality-0.9.1/src/promptquality/constants/dataset_format.py
--rw-r--r--   0        0        0       80 2023-09-14 01:15:15.670682 promptquality-0.9.1/src/promptquality/constants/integrations.py
--rw-r--r--   0        0        0      172 2023-09-14 01:15:15.670682 promptquality-0.9.1/src/promptquality/constants/job.py
--rw-r--r--   0        0        0      988 2023-09-14 01:15:15.670682 promptquality-0.9.1/src/promptquality/constants/models.py
--rw-r--r--   0        0        0     1085 2023-09-14 01:15:15.670682 promptquality-0.9.1/src/promptquality/constants/routes.py
--rw-r--r--   0        0        0      150 2023-09-14 01:15:15.670682 promptquality-0.9.1/src/promptquality/constants/run.py
--rw-r--r--   0        0        0      224 2023-09-14 01:15:15.670682 promptquality-0.9.1/src/promptquality/constants/scorers.py
--rw-r--r--   0        0        0     1840 2023-09-14 01:15:15.670682 promptquality-0.9.1/src/promptquality/get_metrics.py
--rw-r--r--   0        0        0     1652 2023-09-14 01:15:15.670682 promptquality-0.9.1/src/promptquality/get_rows.py
--rw-r--r--   0        0        0    16918 2023-09-14 01:15:15.670682 promptquality-0.9.1/src/promptquality/helpers.py
--rw-r--r--   0        0        0      543 2023-09-14 01:15:15.670682 promptquality-0.9.1/src/promptquality/integrations.py
--rw-r--r--   0        0        0     1097 2023-09-14 01:15:15.670682 promptquality-0.9.1/src/promptquality/job_progress.py
--rw-r--r--   0        0        0      473 2023-09-14 01:15:15.670682 promptquality-0.9.1/src/promptquality/login.py
--rw-r--r--   0        0        0     2614 2023-09-14 01:15:15.670682 promptquality-0.9.1/src/promptquality/run.py
--rw-r--r--   0        0        0     3335 2023-09-14 01:15:15.670682 promptquality-0.9.1/src/promptquality/run_sweep.py
--rw-r--r--   0        0        0     1328 2023-09-14 01:15:15.670682 promptquality-0.9.1/src/promptquality/set_config.py
--rw-r--r--   0        0        0        0 2023-09-14 01:15:15.670682 promptquality-0.9.1/src/promptquality/types/__init__.py
--rw-r--r--   0        0        0     7898 2023-09-14 01:15:15.670682 promptquality-0.9.1/src/promptquality/types/config.py
--rw-r--r--   0        0        0      415 2023-09-14 01:15:15.670682 promptquality-0.9.1/src/promptquality/types/custom_scorer.py
--rw-r--r--   0        0        0      569 2023-09-14 01:15:15.670682 promptquality-0.9.1/src/promptquality/types/pagination.py
--rw-r--r--   0        0        0     1729 2023-09-14 01:15:15.670682 promptquality-0.9.1/src/promptquality/types/rows.py
--rw-r--r--   0        0        0     5817 2023-09-14 01:15:15.670682 promptquality-0.9.1/src/promptquality/types/run.py
--rw-r--r--   0        0        0      976 2023-09-14 01:15:15.670682 promptquality-0.9.1/src/promptquality/types/settings.py
--rw-r--r--   0        0        0     1792 2023-09-14 01:15:15.670682 promptquality-0.9.1/src/promptquality/types/user_submitted_metrics.py
--rw-r--r--   0        0        0        0 2023-09-14 01:15:15.670682 promptquality-0.9.1/src/promptquality/utils/__init__.py
--rw-r--r--   0        0        0     7163 2023-09-14 01:15:15.670682 promptquality-0.9.1/src/promptquality/utils/api_client.py
--rw-r--r--   0        0        0      124 2023-09-14 01:15:15.670682 promptquality-0.9.1/src/promptquality/utils/config.py
--rw-r--r--   0        0        0     3928 2023-09-14 01:15:15.670682 promptquality-0.9.1/src/promptquality/utils/dataset.py
--rw-r--r--   0        0        0      296 2023-09-14 01:15:15.670682 promptquality-0.9.1/src/promptquality/utils/dependencies.py
--rw-r--r--   0        0        0       60 2023-09-14 01:15:15.670682 promptquality-0.9.1/src/promptquality/utils/logger.py
--rw-r--r--   0        0        0    24559 2023-09-14 01:15:15.670682 promptquality-0.9.1/src/promptquality/utils/name.py
--rw-r--r--   0        0        0     1625 2023-09-14 01:15:15.670682 promptquality-0.9.1/src/promptquality/utils/request.py
--rw-r--r--   0        0        0      718 2023-09-14 01:15:15.670682 promptquality-0.9.1/src/promptquality/utils/scorer.py
--rw-r--r--   0        0        0     2250 1970-01-01 00:00:00.000000 promptquality-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0    10946 2023-07-11 00:10:00.760192 promptquality-0.9.2/LICENSE
+-rw-r--r--   0        0        0      759 2023-09-12 00:35:26.228008 promptquality-0.9.2/README.md
+-rw-r--r--   0        0        0     3252 2023-09-27 16:23:45.551936 promptquality-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0      659 2023-09-27 16:23:45.552108 promptquality-0.9.2/src/promptquality/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 21:43:06.067406 promptquality-0.9.2/src/promptquality/constants/__init__.py
+-rw-r--r--   0        0        0      188 2023-08-31 05:57:56.722824 promptquality-0.9.2/src/promptquality/constants/config.py
+-rw-r--r--   0        0        0       96 2023-09-12 16:21:43.041897 promptquality-0.9.2/src/promptquality/constants/dataset_format.py
+-rw-r--r--   0        0        0       80 2023-07-18 06:58:59.840574 promptquality-0.9.2/src/promptquality/constants/integrations.py
+-rw-r--r--   0        0        0      172 2023-07-18 19:06:28.648679 promptquality-0.9.2/src/promptquality/constants/job.py
+-rw-r--r--   0        0        0      988 2023-09-12 00:35:26.231154 promptquality-0.9.2/src/promptquality/constants/models.py
+-rw-r--r--   0        0        0     1085 2023-09-12 00:35:26.231511 promptquality-0.9.2/src/promptquality/constants/routes.py
+-rw-r--r--   0        0        0      150 2023-07-18 19:06:28.649190 promptquality-0.9.2/src/promptquality/constants/run.py
+-rw-r--r--   0        0        0      224 2023-09-12 00:35:26.231752 promptquality-0.9.2/src/promptquality/constants/scorers.py
+-rw-r--r--   0        0        0     1840 2023-07-20 19:27:28.461109 promptquality-0.9.2/src/promptquality/get_metrics.py
+-rw-r--r--   0        0        0     1652 2023-09-13 21:06:22.903167 promptquality-0.9.2/src/promptquality/get_rows.py
+-rw-r--r--   0        0        0    16918 2023-09-13 21:02:40.977013 promptquality-0.9.2/src/promptquality/helpers.py
+-rw-r--r--   0        0        0      543 2023-07-20 19:27:28.461687 promptquality-0.9.2/src/promptquality/integrations.py
+-rw-r--r--   0        0        0     1097 2023-08-31 05:57:56.724567 promptquality-0.9.2/src/promptquality/job_progress.py
+-rw-r--r--   0        0        0      473 2023-09-12 00:35:26.232507 promptquality-0.9.2/src/promptquality/login.py
+-rw-r--r--   0        0        0     2614 2023-09-12 00:35:26.232992 promptquality-0.9.2/src/promptquality/run.py
+-rw-r--r--   0        0        0     3335 2023-09-12 00:35:26.233248 promptquality-0.9.2/src/promptquality/run_sweep.py
+-rw-r--r--   0        0        0     1328 2023-09-12 00:35:26.233554 promptquality-0.9.2/src/promptquality/set_config.py
+-rw-r--r--   0        0        0        0 2023-07-12 21:27:15.179023 promptquality-0.9.2/src/promptquality/types/__init__.py
+-rw-r--r--   0        0        0     7898 2023-08-31 05:57:56.727387 promptquality-0.9.2/src/promptquality/types/config.py
+-rw-r--r--   0        0        0      415 2023-09-14 01:13:18.212015 promptquality-0.9.2/src/promptquality/types/custom_scorer.py
+-rw-r--r--   0        0        0      569 2023-09-13 21:06:22.903557 promptquality-0.9.2/src/promptquality/types/pagination.py
+-rw-r--r--   0        0        0     1729 2023-09-14 01:13:18.212170 promptquality-0.9.2/src/promptquality/types/rows.py
+-rw-r--r--   0        0        0     5817 2023-09-12 16:21:43.045249 promptquality-0.9.2/src/promptquality/types/run.py
+-rw-r--r--   0        0        0      975 2023-09-27 16:23:45.552267 promptquality-0.9.2/src/promptquality/types/settings.py
+-rw-r--r--   0        0        0     1792 2023-09-14 01:13:18.212484 promptquality-0.9.2/src/promptquality/types/user_submitted_metrics.py
+-rw-r--r--   0        0        0        0 2023-07-13 21:34:38.612950 promptquality-0.9.2/src/promptquality/utils/__init__.py
+-rw-r--r--   0        0        0     7163 2023-09-13 21:06:22.904728 promptquality-0.9.2/src/promptquality/utils/api_client.py
+-rw-r--r--   0        0        0      124 2023-08-31 05:57:56.729532 promptquality-0.9.2/src/promptquality/utils/config.py
+-rw-r--r--   0        0        0     3928 2023-09-12 16:21:43.046266 promptquality-0.9.2/src/promptquality/utils/dataset.py
+-rw-r--r--   0        0        0      296 2023-09-12 16:21:43.047868 promptquality-0.9.2/src/promptquality/utils/dependencies.py
+-rw-r--r--   0        0        0       60 2023-07-15 00:13:08.502687 promptquality-0.9.2/src/promptquality/utils/logger.py
+-rw-r--r--   0        0        0    24559 2023-07-26 21:39:39.128777 promptquality-0.9.2/src/promptquality/utils/name.py
+-rw-r--r--   0        0        0     1625 2023-08-09 01:06:19.068025 promptquality-0.9.2/src/promptquality/utils/request.py
+-rw-r--r--   0        0        0      718 2023-09-12 00:35:26.237406 promptquality-0.9.2/src/promptquality/utils/scorer.py
+-rw-r--r--   0        0        0     2250 1970-01-01 00:00:00.000000 promptquality-0.9.2/PKG-INFO
```

### Comparing `promptquality-0.9.1/LICENSE` & `promptquality-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `promptquality-0.9.1/README.md` & `promptquality-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `promptquality-0.9.1/pyproject.toml` & `promptquality-0.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "promptquality"
-version = "0.9.1"
+version = "0.9.2"
 description = "🦸 Supercharge your prompts with Galileo's Prompt Inspector!"
 authors = ["Galileo Technologies Inc. <team@rungalileo.io>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://www.rungalileo.io/llm-studio"
 repository = "https://github.com/rungalileo/promptquality"
 documentation = "https://docs.rungalileo.io/galileo/python-sdks/promptquality-sdk/"
```

### Comparing `promptquality-0.9.1/src/promptquality/__init__.py` & `promptquality-0.9.2/src/promptquality/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 from promptquality.login import login
 from promptquality.run import run
 from promptquality.run_sweep import run_sweep
 from promptquality.set_config import set_config
 from promptquality.types.custom_scorer import CustomScorer
 from promptquality.types.settings import Settings
 
-__version__ = "0.9.1"
+__version__ = "0.9.2"
```

### Comparing `promptquality-0.9.1/src/promptquality/constants/models.py` & `promptquality-0.9.2/src/promptquality/constants/models.py`

 * *Files identical despite different names*

### Comparing `promptquality-0.9.1/src/promptquality/constants/routes.py` & `promptquality-0.9.2/src/promptquality/constants/routes.py`

 * *Files identical despite different names*

### Comparing `promptquality-0.9.1/src/promptquality/get_metrics.py` & `promptquality-0.9.2/src/promptquality/get_metrics.py`

 * *Files identical despite different names*

### Comparing `promptquality-0.9.1/src/promptquality/get_rows.py` & `promptquality-0.9.2/src/promptquality/get_rows.py`

 * *Files identical despite different names*

### Comparing `promptquality-0.9.1/src/promptquality/helpers.py` & `promptquality-0.9.2/src/promptquality/helpers.py`

 * *Files identical despite different names*

### Comparing `promptquality-0.9.1/src/promptquality/integrations.py` & `promptquality-0.9.2/src/promptquality/integrations.py`

 * *Files identical despite different names*

### Comparing `promptquality-0.9.1/src/promptquality/job_progress.py` & `promptquality-0.9.2/src/promptquality/job_progress.py`

 * *Files identical despite different names*

### Comparing `promptquality-0.9.1/src/promptquality/run.py` & `promptquality-0.9.2/src/promptquality/run.py`

 * *Files identical despite different names*

### Comparing `promptquality-0.9.1/src/promptquality/run_sweep.py` & `promptquality-0.9.2/src/promptquality/run_sweep.py`

 * *Files identical despite different names*

### Comparing `promptquality-0.9.1/src/promptquality/set_config.py` & `promptquality-0.9.2/src/promptquality/set_config.py`

 * *Files identical despite different names*

### Comparing `promptquality-0.9.1/src/promptquality/types/config.py` & `promptquality-0.9.2/src/promptquality/types/config.py`

 * *Files identical despite different names*

### Comparing `promptquality-0.9.1/src/promptquality/types/pagination.py` & `promptquality-0.9.2/src/promptquality/types/pagination.py`

 * *Files identical despite different names*

### Comparing `promptquality-0.9.1/src/promptquality/types/rows.py` & `promptquality-0.9.2/src/promptquality/types/rows.py`

 * *Files identical despite different names*

### Comparing `promptquality-0.9.1/src/promptquality/types/run.py` & `promptquality-0.9.2/src/promptquality/types/run.py`

 * *Files identical despite different names*

### Comparing `promptquality-0.9.1/src/promptquality/types/settings.py` & `promptquality-0.9.2/src/promptquality/types/settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,9 +25,9 @@
     api_version: Optional[str] = None
 
     model_config = ConfigDict(
         # Avoid Pydantic's protected namespace warning since we want to use
         # `model_alias` as a field name.
         protected_namespaces=(),
         # Disallow extra fields.
-        extra="forbid",
+        extra="allow",
     )
```

### Comparing `promptquality-0.9.1/src/promptquality/types/user_submitted_metrics.py` & `promptquality-0.9.2/src/promptquality/types/user_submitted_metrics.py`

 * *Files identical despite different names*

### Comparing `promptquality-0.9.1/src/promptquality/utils/api_client.py` & `promptquality-0.9.2/src/promptquality/utils/api_client.py`

 * *Files identical despite different names*

### Comparing `promptquality-0.9.1/src/promptquality/utils/dataset.py` & `promptquality-0.9.2/src/promptquality/utils/dataset.py`

 * *Files identical despite different names*

### Comparing `promptquality-0.9.1/src/promptquality/utils/name.py` & `promptquality-0.9.2/src/promptquality/utils/name.py`

 * *Files identical despite different names*

### Comparing `promptquality-0.9.1/src/promptquality/utils/request.py` & `promptquality-0.9.2/src/promptquality/utils/request.py`

 * *Files identical despite different names*

### Comparing `promptquality-0.9.1/src/promptquality/utils/scorer.py` & `promptquality-0.9.2/src/promptquality/utils/scorer.py`

 * *Files identical despite different names*

### Comparing `promptquality-0.9.1/PKG-INFO` & `promptquality-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptquality
-Version: 0.9.1
+Version: 0.9.2
 Summary: 🦸 Supercharge your prompts with Galileo's Prompt Inspector!
 Home-page: https://www.rungalileo.io/llm-studio
 License: Apache-2.0
 Keywords: prompt,nlp,llm,quality,language_models,galileo
 Author: Galileo Technologies Inc.
 Author-email: team@rungalileo.io
 Requires-Python: >=3.8,<3.12
```

