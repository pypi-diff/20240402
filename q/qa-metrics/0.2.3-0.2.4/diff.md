# Comparing `tmp/qa_metrics-0.2.3.tar.gz` & `tmp/qa_metrics-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qa_metrics-0.2.3.tar", last modified: Mon Apr  1 23:54:45 2024, max compression
+gzip compressed data, was "qa_metrics-0.2.4.tar", last modified: Tue Apr  2 00:09:16 2024, max compression
```

## Comparing `qa_metrics-0.2.3.tar` & `qa_metrics-0.2.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 zongxiali   (501) staff       (20)        0 2024-04-01 23:54:45.676061 qa_metrics-0.2.3/
--rw-r--r--   0 zongxiali   (501) staff       (20)     1071 2024-02-27 04:41:04.000000 qa_metrics-0.2.3/LICENSE
--rw-r--r--   0 zongxiali   (501) staff       (20)       69 2024-02-27 04:41:04.000000 qa_metrics-0.2.3/MANIFEST.in
--rw-r--r--   0 zongxiali   (501) staff       (20)     6555 2024-04-01 23:54:45.675554 qa_metrics-0.2.3/PKG-INFO
--rw-r--r--   0 zongxiali   (501) staff       (20)     5845 2024-02-29 04:35:20.000000 qa_metrics-0.2.3/README.md
-drwxr-xr-x   0 zongxiali   (501) staff       (20)        0 2024-04-01 23:54:45.669437 qa_metrics-0.2.3/qa_metrics/
--rw-r--r--   0 zongxiali   (501) staff       (20)     5330 2024-04-01 23:46:22.000000 qa_metrics-0.2.3/qa_metrics/Prompt_LLM.py
--rw-r--r--   0 zongxiali   (501) staff       (20)     2324 2024-03-30 03:21:43.000000 qa_metrics-0.2.3/qa_metrics/__init__.py
--rw-r--r--   0 zongxiali   (501) staff       (20)     1122 2024-03-31 05:04:42.000000 qa_metrics-0.2.3/qa_metrics/em.py
--rw-r--r--   0 zongxiali   (501) staff       (20)     2853 2024-03-31 04:14:56.000000 qa_metrics-0.2.3/qa_metrics/f1.py
--rw-r--r--   0 zongxiali   (501) staff       (20)    15909 2024-04-01 21:03:35.000000 qa_metrics-0.2.3/qa_metrics/pedant.py
--rw-r--r--   0 zongxiali   (501) staff       (20)    14173 2024-03-30 17:42:06.000000 qa_metrics-0.2.3/qa_metrics/transformerMatcher.py
-drwxr-xr-x   0 zongxiali   (501) staff       (20)        0 2024-04-01 23:54:45.674056 qa_metrics-0.2.3/qa_metrics/utils/
--rw-r--r--   0 zongxiali   (501) staff       (20)        0 2024-02-27 04:41:04.000000 qa_metrics-0.2.3/qa_metrics/utils/__init__.py
--rw-r--r--   0 zongxiali   (501) staff       (20)     2724 2024-03-31 04:49:31.000000 qa_metrics-0.2.3/qa_metrics/utils/tools.py
-drwxr-xr-x   0 zongxiali   (501) staff       (20)        0 2024-04-01 23:54:45.673007 qa_metrics-0.2.3/qa_metrics.egg-info/
--rw-r--r--   0 zongxiali   (501) staff       (20)     6555 2024-04-01 23:54:45.000000 qa_metrics-0.2.3/qa_metrics.egg-info/PKG-INFO
--rw-r--r--   0 zongxiali   (501) staff       (20)      423 2024-04-01 23:54:45.000000 qa_metrics-0.2.3/qa_metrics.egg-info/SOURCES.txt
--rw-r--r--   0 zongxiali   (501) staff       (20)        1 2024-04-01 23:54:45.000000 qa_metrics-0.2.3/qa_metrics.egg-info/dependency_links.txt
--rw-r--r--   0 zongxiali   (501) staff       (20)       75 2024-04-01 23:54:45.000000 qa_metrics-0.2.3/qa_metrics.egg-info/requires.txt
--rw-r--r--   0 zongxiali   (501) staff       (20)       11 2024-04-01 23:54:45.000000 qa_metrics-0.2.3/qa_metrics.egg-info/top_level.txt
--rw-r--r--   0 zongxiali   (501) staff       (20)       38 2024-04-01 23:54:45.676274 qa_metrics-0.2.3/setup.cfg
--rw-r--r--   0 zongxiali   (501) staff       (20)     1296 2024-04-01 23:54:37.000000 qa_metrics-0.2.3/setup.py
+drwxr-xr-x   0 zongxiali   (501) staff       (20)        0 2024-04-02 00:09:16.882462 qa_metrics-0.2.4/
+-rw-r--r--   0 zongxiali   (501) staff       (20)     1071 2024-02-27 04:41:04.000000 qa_metrics-0.2.4/LICENSE
+-rw-r--r--   0 zongxiali   (501) staff       (20)       69 2024-02-27 04:41:04.000000 qa_metrics-0.2.4/MANIFEST.in
+-rw-r--r--   0 zongxiali   (501) staff       (20)     6555 2024-04-02 00:09:16.882054 qa_metrics-0.2.4/PKG-INFO
+-rw-r--r--   0 zongxiali   (501) staff       (20)     5845 2024-02-29 04:35:20.000000 qa_metrics-0.2.4/README.md
+drwxr-xr-x   0 zongxiali   (501) staff       (20)        0 2024-04-02 00:09:16.877846 qa_metrics-0.2.4/qa_metrics/
+-rw-r--r--   0 zongxiali   (501) staff       (20)     5344 2024-04-02 00:07:53.000000 qa_metrics-0.2.4/qa_metrics/Prompt_LLM.py
+-rw-r--r--   0 zongxiali   (501) staff       (20)     2324 2024-03-30 03:21:43.000000 qa_metrics-0.2.4/qa_metrics/__init__.py
+-rw-r--r--   0 zongxiali   (501) staff       (20)     1122 2024-03-31 05:04:42.000000 qa_metrics-0.2.4/qa_metrics/em.py
+-rw-r--r--   0 zongxiali   (501) staff       (20)     2853 2024-03-31 04:14:56.000000 qa_metrics-0.2.4/qa_metrics/f1.py
+-rw-r--r--   0 zongxiali   (501) staff       (20)    15909 2024-04-01 21:03:35.000000 qa_metrics-0.2.4/qa_metrics/pedant.py
+-rw-r--r--   0 zongxiali   (501) staff       (20)    14173 2024-03-30 17:42:06.000000 qa_metrics-0.2.4/qa_metrics/transformerMatcher.py
+drwxr-xr-x   0 zongxiali   (501) staff       (20)        0 2024-04-02 00:09:16.880987 qa_metrics-0.2.4/qa_metrics/utils/
+-rw-r--r--   0 zongxiali   (501) staff       (20)        0 2024-02-27 04:41:04.000000 qa_metrics-0.2.4/qa_metrics/utils/__init__.py
+-rw-r--r--   0 zongxiali   (501) staff       (20)     2724 2024-03-31 04:49:31.000000 qa_metrics-0.2.4/qa_metrics/utils/tools.py
+drwxr-xr-x   0 zongxiali   (501) staff       (20)        0 2024-04-02 00:09:16.880402 qa_metrics-0.2.4/qa_metrics.egg-info/
+-rw-r--r--   0 zongxiali   (501) staff       (20)     6555 2024-04-02 00:09:16.000000 qa_metrics-0.2.4/qa_metrics.egg-info/PKG-INFO
+-rw-r--r--   0 zongxiali   (501) staff       (20)      423 2024-04-02 00:09:16.000000 qa_metrics-0.2.4/qa_metrics.egg-info/SOURCES.txt
+-rw-r--r--   0 zongxiali   (501) staff       (20)        1 2024-04-02 00:09:16.000000 qa_metrics-0.2.4/qa_metrics.egg-info/dependency_links.txt
+-rw-r--r--   0 zongxiali   (501) staff       (20)       75 2024-04-02 00:09:16.000000 qa_metrics-0.2.4/qa_metrics.egg-info/requires.txt
+-rw-r--r--   0 zongxiali   (501) staff       (20)       11 2024-04-02 00:09:16.000000 qa_metrics-0.2.4/qa_metrics.egg-info/top_level.txt
+-rw-r--r--   0 zongxiali   (501) staff       (20)       38 2024-04-02 00:09:16.882590 qa_metrics-0.2.4/setup.cfg
+-rw-r--r--   0 zongxiali   (501) staff       (20)     1296 2024-04-02 00:07:57.000000 qa_metrics-0.2.4/setup.py
```

### Comparing `qa_metrics-0.2.3/LICENSE` & `qa_metrics-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `qa_metrics-0.2.3/PKG-INFO` & `qa_metrics-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qa_metrics
-Version: 0.2.3
+Version: 0.2.4
 Summary: This package provides standard and classifier-based short form QA evaluation methods
 Home-page: https://github.com/zli12321/qa_metrics
 Author: Zongxia Li
 Author-email: zli12321@umd.edu
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `qa_metrics-0.2.3/README.md` & `qa_metrics-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `qa_metrics-0.2.3/qa_metrics/Prompt_LLM.py` & `qa_metrics-0.2.4/qa_metrics/Prompt_LLM.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
         return None
 
     except KeyError:
         print("OpenAI API key not found in the environment variables.")
         return None
     
 
-def prompt_claude(prompt, model="claude-v1", anthropic_version="2023-06-01", max_tokens_to_sample=100, temperature=0.7):
+def prompt_claude(prompt, model_engine="claude-v1", anthropic_version="2023-06-01", max_tokens_to_sample=100, temperature=0.7):
     # Set up the API endpoint URL
     url = "https://api.anthropic.com/v1/complete"
 
     # Set up the request headers
     headers = {
         "Content-Type": "application/json",
         "X-API-Key": os.environ["ANTHROPIC_API_KEY"],
@@ -115,15 +115,15 @@
 
     # print(conversation_history)
     conversation_history = "Human: " + prompt + "\nAssistant:"
 
     # Set up the request payload
     payload = {
         "prompt": conversation_history,
-        "model": model,
+        "model": model_engine,
         "max_tokens_to_sample": max_tokens_to_sample,
         "temperature": temperature
     }
 
     try:
         # Send the request to the Anthropic API
         response = requests.post(url, json=payload, headers=headers)
```

### Comparing `qa_metrics-0.2.3/qa_metrics/__init__.py` & `qa_metrics-0.2.4/qa_metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `qa_metrics-0.2.3/qa_metrics/em.py` & `qa_metrics-0.2.4/qa_metrics/em.py`

 * *Files identical despite different names*

### Comparing `qa_metrics-0.2.3/qa_metrics/f1.py` & `qa_metrics-0.2.4/qa_metrics/f1.py`

 * *Files identical despite different names*

### Comparing `qa_metrics-0.2.3/qa_metrics/pedant.py` & `qa_metrics-0.2.4/qa_metrics/pedant.py`

 * *Files identical despite different names*

### Comparing `qa_metrics-0.2.3/qa_metrics/transformerMatcher.py` & `qa_metrics-0.2.4/qa_metrics/transformerMatcher.py`

 * *Files identical despite different names*

### Comparing `qa_metrics-0.2.3/qa_metrics/utils/tools.py` & `qa_metrics-0.2.4/qa_metrics/utils/tools.py`

 * *Files identical despite different names*

### Comparing `qa_metrics-0.2.3/qa_metrics.egg-info/PKG-INFO` & `qa_metrics-0.2.4/qa_metrics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qa-metrics
-Version: 0.2.3
+Version: 0.2.4
 Summary: This package provides standard and classifier-based short form QA evaluation methods
 Home-page: https://github.com/zli12321/qa_metrics
 Author: Zongxia Li
 Author-email: zli12321@umd.edu
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `qa_metrics-0.2.3/setup.py` & `qa_metrics-0.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 import os
 
 
 setup(
     name='qa_metrics',
-    version='0.2.3',
+    version='0.2.4',
     author='Zongxia Li',
     author_email='zli12321@umd.edu',
     description='This package provides standard and classifier-based short form QA evaluation methods',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/zli12321/qa_metrics',
     packages=find_packages(),
```

