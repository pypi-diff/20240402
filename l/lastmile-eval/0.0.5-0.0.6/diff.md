# Comparing `tmp/lastmile-eval-0.0.5.tar.gz` & `tmp/lastmile-eval-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lastmile-eval-0.0.5.tar", last modified: Mon Apr  1 20:49:49 2024, max compression
+gzip compressed data, was "lastmile-eval-0.0.6.tar", last modified: Tue Apr  2 00:42:07 2024, max compression
```

## Comparing `lastmile-eval-0.0.5.tar` & `lastmile-eval-0.0.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:49:49.447381 lastmile-eval-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-01 20:49:43.000000 lastmile-eval-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-01 20:49:49.447381 lastmile-eval-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-01 20:49:43.000000 lastmile-eval-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-01 20:49:43.000000 lastmile-eval-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-01 20:49:43.000000 lastmile-eval-0.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 20:49:49.447381 lastmile-eval-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:49:49.443381 lastmile-eval-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:49:49.443381 lastmile-eval-0.0.5/src/lastmile_eval/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:49:49.443381 lastmile-eval-0.0.5/src/lastmile_eval/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-04-01 20:49:43.000000 lastmile-eval-0.0.5/src/lastmile_eval/examples/rag.py
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-04-01 20:49:43.000000 lastmile-eval-0.0.5/src/lastmile_eval/examples/text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:49:49.443381 lastmile-eval-0.0.5/src/lastmile_eval/rag/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-01 20:49:43.000000 lastmile-eval-0.0.5/src/lastmile_eval/rag/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:49:49.447381 lastmile-eval-0.0.5/src/lastmile_eval/text/
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-01 20:49:43.000000 lastmile-eval-0.0.5/src/lastmile_eval/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-01 20:49:43.000000 lastmile-eval-0.0.5/src/lastmile_eval/text/batch_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    15203 2024-04-01 20:49:43.000000 lastmile-eval-0.0.5/src/lastmile_eval/text/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-01 20:49:43.000000 lastmile-eval-0.0.5/src/lastmile_eval/text/metrics_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     6119 2024-04-01 20:49:43.000000 lastmile-eval-0.0.5/src/lastmile_eval/text/openai_batch_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:49:43.000000 lastmile-eval-0.0.5/src/lastmile_eval/text/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-04-01 20:49:43.000000 lastmile-eval-0.0.5/src/lastmile_eval/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:49:49.447381 lastmile-eval-0.0.5/src/lastmile_eval.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-01 20:49:49.000000 lastmile-eval-0.0.5/src/lastmile_eval.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-01 20:49:49.000000 lastmile-eval-0.0.5/src/lastmile_eval.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 20:49:49.000000 lastmile-eval-0.0.5/src/lastmile_eval.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-01 20:49:49.000000 lastmile-eval-0.0.5/src/lastmile_eval.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-01 20:49:49.000000 lastmile-eval-0.0.5/src/lastmile_eval.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:49:49.447381 lastmile-eval-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-04-01 20:49:43.000000 lastmile-eval-0.0.5/tests/test_custom_llm_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     9004 2024-04-01 20:49:43.000000 lastmile-eval-0.0.5/tests/test_default_text_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-04-01 20:49:43.000000 lastmile-eval-0.0.5/tests/test_rag_scores_e2e.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:42:07.889550 lastmile-eval-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-02 00:42:03.000000 lastmile-eval-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8176 2024-04-02 00:42:07.885550 lastmile-eval-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7391 2024-04-02 00:42:03.000000 lastmile-eval-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-02 00:42:03.000000 lastmile-eval-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-02 00:42:03.000000 lastmile-eval-0.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 00:42:07.889550 lastmile-eval-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:42:07.881550 lastmile-eval-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:42:07.881550 lastmile-eval-0.0.6/src/lastmile_eval/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:42:07.885550 lastmile-eval-0.0.6/src/lastmile_eval/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-02 00:42:03.000000 lastmile-eval-0.0.6/src/lastmile_eval/examples/rag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-04-02 00:42:03.000000 lastmile-eval-0.0.6/src/lastmile_eval/examples/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:42:07.885550 lastmile-eval-0.0.6/src/lastmile_eval/rag/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-02 00:42:03.000000 lastmile-eval-0.0.6/src/lastmile_eval/rag/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:42:07.885550 lastmile-eval-0.0.6/src/lastmile_eval/text/
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-02 00:42:03.000000 lastmile-eval-0.0.6/src/lastmile_eval/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-02 00:42:03.000000 lastmile-eval-0.0.6/src/lastmile_eval/text/batch_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15203 2024-04-02 00:42:03.000000 lastmile-eval-0.0.6/src/lastmile_eval/text/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-02 00:42:03.000000 lastmile-eval-0.0.6/src/lastmile_eval/text/metrics_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6119 2024-04-02 00:42:03.000000 lastmile-eval-0.0.6/src/lastmile_eval/text/openai_batch_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 00:42:03.000000 lastmile-eval-0.0.6/src/lastmile_eval/text/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-04-02 00:42:03.000000 lastmile-eval-0.0.6/src/lastmile_eval/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:42:07.885550 lastmile-eval-0.0.6/src/lastmile_eval.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8176 2024-04-02 00:42:07.000000 lastmile-eval-0.0.6/src/lastmile_eval.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-02 00:42:07.000000 lastmile-eval-0.0.6/src/lastmile_eval.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 00:42:07.000000 lastmile-eval-0.0.6/src/lastmile_eval.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-02 00:42:07.000000 lastmile-eval-0.0.6/src/lastmile_eval.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-02 00:42:07.000000 lastmile-eval-0.0.6/src/lastmile_eval.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:42:07.885550 lastmile-eval-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-04-02 00:42:03.000000 lastmile-eval-0.0.6/tests/test_custom_llm_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9004 2024-04-02 00:42:03.000000 lastmile-eval-0.0.6/tests/test_default_text_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-04-02 00:42:03.000000 lastmile-eval-0.0.6/tests/test_rag_scores_e2e.py
```

### Comparing `lastmile-eval-0.0.5/LICENSE` & `lastmile-eval-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lastmile-eval-0.0.5/pyproject.toml` & `lastmile-eval-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "lastmile-eval"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="LastMile AI" },
 ]
 description = "An API to measure evaluation criteria (ex: faithfulness) of generative AI outputs"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `lastmile-eval-0.0.5/src/lastmile_eval/examples/rag.py` & `lastmile-eval-0.0.6/src/lastmile_eval/examples/rag.py`

 * *Files 6% similar despite different names*

```diff
@@ -66,17 +66,14 @@
     which we will use for rendering prompt input/settings/metadata on the client
     """
 
     data = [data1] * 2
 
     responses = ["""client rendering""", """metadata mapping"""]
 
-    # f"{data1}. Query: {questions[0]}",
-    # f"{data1}. Query: {questions[1]}",
-
     print(f"Input batch:")
     df = pd.DataFrame(
         {"question": questions, "data": data, "response": responses}
     )
     print(df)
 
     api_token = get_lastmile_api_token()
```

### Comparing `lastmile-eval-0.0.5/src/lastmile_eval/examples/text.py` & `lastmile-eval-0.0.6/src/lastmile_eval/examples/text.py`

 * *Files identical despite different names*

### Comparing `lastmile-eval-0.0.5/src/lastmile_eval/text/__init__.py` & `lastmile-eval-0.0.6/src/lastmile_eval/text/__init__.py`

 * *Files identical despite different names*

### Comparing `lastmile-eval-0.0.5/src/lastmile_eval/text/batch_lib.py` & `lastmile-eval-0.0.6/src/lastmile_eval/text/batch_lib.py`

 * *Files identical despite different names*

### Comparing `lastmile-eval-0.0.5/src/lastmile_eval/text/metrics.py` & `lastmile-eval-0.0.6/src/lastmile_eval/text/metrics.py`

 * *Files identical despite different names*

### Comparing `lastmile-eval-0.0.5/src/lastmile_eval/text/metrics_lib.py` & `lastmile-eval-0.0.6/src/lastmile_eval/text/metrics_lib.py`

 * *Files identical despite different names*

### Comparing `lastmile-eval-0.0.5/src/lastmile_eval/text/openai_batch_lib.py` & `lastmile-eval-0.0.6/src/lastmile_eval/text/openai_batch_lib.py`

 * *Files identical despite different names*

### Comparing `lastmile-eval-0.0.5/src/lastmile_eval/utils.py` & `lastmile-eval-0.0.6/src/lastmile_eval/utils.py`

 * *Files identical despite different names*

### Comparing `lastmile-eval-0.0.5/src/lastmile_eval.egg-info/SOURCES.txt` & `lastmile-eval-0.0.6/src/lastmile_eval.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lastmile-eval-0.0.5/tests/test_custom_llm_metrics.py` & `lastmile-eval-0.0.6/tests/test_custom_llm_metrics.py`

 * *Files identical despite different names*

### Comparing `lastmile-eval-0.0.5/tests/test_default_text_metrics.py` & `lastmile-eval-0.0.6/tests/test_default_text_metrics.py`

 * *Files identical despite different names*

### Comparing `lastmile-eval-0.0.5/tests/test_rag_scores_e2e.py` & `lastmile-eval-0.0.6/tests/test_rag_scores_e2e.py`

 * *Files identical despite different names*

