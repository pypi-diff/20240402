# Comparing `tmp/qa_metrics-0.2.1.tar.gz` & `tmp/qa_metrics-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qa_metrics-0.2.1.tar", last modified: Mon Apr  1 23:40:35 2024, max compression
+gzip compressed data, was "qa_metrics-0.2.2.tar", last modified: Mon Apr  1 23:47:51 2024, max compression
```

## Comparing `qa_metrics-0.2.1.tar` & `qa_metrics-0.2.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 zongxiali   (501) staff       (20)        0 2024-04-01 23:40:35.007649 qa_metrics-0.2.1/
--rw-r--r--   0 zongxiali   (501) staff       (20)     1071 2024-02-27 04:41:04.000000 qa_metrics-0.2.1/LICENSE
--rw-r--r--   0 zongxiali   (501) staff       (20)       69 2024-02-27 04:41:04.000000 qa_metrics-0.2.1/MANIFEST.in
--rw-r--r--   0 zongxiali   (501) staff       (20)     6555 2024-04-01 23:40:35.007305 qa_metrics-0.2.1/PKG-INFO
--rw-r--r--   0 zongxiali   (501) staff       (20)     5845 2024-02-29 04:35:20.000000 qa_metrics-0.2.1/README.md
-drwxr-xr-x   0 zongxiali   (501) staff       (20)        0 2024-04-01 23:40:35.000704 qa_metrics-0.2.1/qa_metrics/
--rw-r--r--   0 zongxiali   (501) staff       (20)     5330 2024-04-01 23:38:55.000000 qa_metrics-0.2.1/qa_metrics/Prompt_LLM.py
--rw-r--r--   0 zongxiali   (501) staff       (20)     2324 2024-03-30 03:21:43.000000 qa_metrics-0.2.1/qa_metrics/__init__.py
--rw-r--r--   0 zongxiali   (501) staff       (20)     1122 2024-03-31 05:04:42.000000 qa_metrics-0.2.1/qa_metrics/em.py
--rw-r--r--   0 zongxiali   (501) staff       (20)     2853 2024-03-31 04:14:56.000000 qa_metrics-0.2.1/qa_metrics/f1.py
--rw-r--r--   0 zongxiali   (501) staff       (20)    15909 2024-04-01 21:03:35.000000 qa_metrics-0.2.1/qa_metrics/pedant.py
--rw-r--r--   0 zongxiali   (501) staff       (20)    14173 2024-03-30 17:42:06.000000 qa_metrics-0.2.1/qa_metrics/transformerMatcher.py
-drwxr-xr-x   0 zongxiali   (501) staff       (20)        0 2024-04-01 23:40:35.006056 qa_metrics-0.2.1/qa_metrics/utils/
--rw-r--r--   0 zongxiali   (501) staff       (20)        0 2024-02-27 04:41:04.000000 qa_metrics-0.2.1/qa_metrics/utils/__init__.py
--rw-r--r--   0 zongxiali   (501) staff       (20)     2724 2024-03-31 04:49:31.000000 qa_metrics-0.2.1/qa_metrics/utils/tools.py
-drwxr-xr-x   0 zongxiali   (501) staff       (20)        0 2024-04-01 23:40:35.005121 qa_metrics-0.2.1/qa_metrics.egg-info/
--rw-r--r--   0 zongxiali   (501) staff       (20)     6555 2024-04-01 23:40:34.000000 qa_metrics-0.2.1/qa_metrics.egg-info/PKG-INFO
--rw-r--r--   0 zongxiali   (501) staff       (20)      398 2024-04-01 23:40:34.000000 qa_metrics-0.2.1/qa_metrics.egg-info/SOURCES.txt
--rw-r--r--   0 zongxiali   (501) staff       (20)        1 2024-04-01 23:40:34.000000 qa_metrics-0.2.1/qa_metrics.egg-info/dependency_links.txt
--rw-r--r--   0 zongxiali   (501) staff       (20)       75 2024-04-01 23:40:34.000000 qa_metrics-0.2.1/qa_metrics.egg-info/requires.txt
--rw-r--r--   0 zongxiali   (501) staff       (20)       11 2024-04-01 23:40:34.000000 qa_metrics-0.2.1/qa_metrics.egg-info/top_level.txt
--rw-r--r--   0 zongxiali   (501) staff       (20)       38 2024-04-01 23:40:35.007763 qa_metrics-0.2.1/setup.cfg
--rw-r--r--   0 zongxiali   (501) staff       (20)     1296 2024-04-01 23:40:28.000000 qa_metrics-0.2.1/setup.py
+drwxr-xr-x   0 zongxiali   (501) staff       (20)        0 2024-04-01 23:47:51.066779 qa_metrics-0.2.2/
+-rw-r--r--   0 zongxiali   (501) staff       (20)     1071 2024-02-27 04:41:04.000000 qa_metrics-0.2.2/LICENSE
+-rw-r--r--   0 zongxiali   (501) staff       (20)       69 2024-02-27 04:41:04.000000 qa_metrics-0.2.2/MANIFEST.in
+-rw-r--r--   0 zongxiali   (501) staff       (20)     6555 2024-04-01 23:47:51.066382 qa_metrics-0.2.2/PKG-INFO
+-rw-r--r--   0 zongxiali   (501) staff       (20)     5845 2024-02-29 04:35:20.000000 qa_metrics-0.2.2/README.md
+drwxr-xr-x   0 zongxiali   (501) staff       (20)        0 2024-04-01 23:47:51.062007 qa_metrics-0.2.2/qa_metrics/
+-rw-r--r--   0 zongxiali   (501) staff       (20)     5330 2024-04-01 23:46:22.000000 qa_metrics-0.2.2/qa_metrics/Prompt_LLM.py
+-rw-r--r--   0 zongxiali   (501) staff       (20)     2324 2024-03-30 03:21:43.000000 qa_metrics-0.2.2/qa_metrics/__init__.py
+-rw-r--r--   0 zongxiali   (501) staff       (20)     1122 2024-03-31 05:04:42.000000 qa_metrics-0.2.2/qa_metrics/em.py
+-rw-r--r--   0 zongxiali   (501) staff       (20)     2853 2024-03-31 04:14:56.000000 qa_metrics-0.2.2/qa_metrics/f1.py
+-rw-r--r--   0 zongxiali   (501) staff       (20)    15909 2024-04-01 21:03:35.000000 qa_metrics-0.2.2/qa_metrics/pedant.py
+-rw-r--r--   0 zongxiali   (501) staff       (20)    14173 2024-03-30 17:42:06.000000 qa_metrics-0.2.2/qa_metrics/transformerMatcher.py
+drwxr-xr-x   0 zongxiali   (501) staff       (20)        0 2024-04-01 23:47:51.065550 qa_metrics-0.2.2/qa_metrics/utils/
+-rw-r--r--   0 zongxiali   (501) staff       (20)        0 2024-02-27 04:41:04.000000 qa_metrics-0.2.2/qa_metrics/utils/__init__.py
+-rw-r--r--   0 zongxiali   (501) staff       (20)     2724 2024-03-31 04:49:31.000000 qa_metrics-0.2.2/qa_metrics/utils/tools.py
+drwxr-xr-x   0 zongxiali   (501) staff       (20)        0 2024-04-01 23:47:51.064928 qa_metrics-0.2.2/qa_metrics.egg-info/
+-rw-r--r--   0 zongxiali   (501) staff       (20)     6555 2024-04-01 23:47:50.000000 qa_metrics-0.2.2/qa_metrics.egg-info/PKG-INFO
+-rw-r--r--   0 zongxiali   (501) staff       (20)      423 2024-04-01 23:47:50.000000 qa_metrics-0.2.2/qa_metrics.egg-info/SOURCES.txt
+-rw-r--r--   0 zongxiali   (501) staff       (20)        1 2024-04-01 23:47:50.000000 qa_metrics-0.2.2/qa_metrics.egg-info/dependency_links.txt
+-rw-r--r--   0 zongxiali   (501) staff       (20)       75 2024-04-01 23:47:50.000000 qa_metrics-0.2.2/qa_metrics.egg-info/requires.txt
+-rw-r--r--   0 zongxiali   (501) staff       (20)       11 2024-04-01 23:47:50.000000 qa_metrics-0.2.2/qa_metrics.egg-info/top_level.txt
+-rw-r--r--   0 zongxiali   (501) staff       (20)       38 2024-04-01 23:47:51.066934 qa_metrics-0.2.2/setup.cfg
+-rw-r--r--   0 zongxiali   (501) staff       (20)     1296 2024-04-01 23:47:44.000000 qa_metrics-0.2.2/setup.py
```

### Comparing `qa_metrics-0.2.1/LICENSE` & `qa_metrics-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qa_metrics-0.2.1/PKG-INFO` & `qa_metrics-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qa_metrics
-Version: 0.2.1
+Version: 0.2.2
 Summary: This package provides standard and classifier-based short form QA evaluation methods
 Home-page: https://github.com/zli12321/qa_metrics
 Author: Zongxia Li
 Author-email: zli12321@umd.edu
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `qa_metrics-0.2.1/README.md` & `qa_metrics-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `qa_metrics-0.2.1/qa_metrics/Prompt_LLM.py` & `qa_metrics-0.2.2/qa_metrics/Prompt_LLM.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
         return None
 
     except KeyError:
         print("OpenAI API key not found in the environment variables.")
         return None
     
 
-def propmt_claude(prompt, model="claude-v1", anthropic_version="2023-06-01", max_tokens_to_sample=100, temperature=0.7):
+def prompt_claude(prompt, model="claude-v1", anthropic_version="2023-06-01", max_tokens_to_sample=100, temperature=0.7):
     # Set up the API endpoint URL
     url = "https://api.anthropic.com/v1/complete"
 
     # Set up the request headers
     headers = {
         "Content-Type": "application/json",
         "X-API-Key": os.environ["ANTHROPIC_API_KEY"],
```

### Comparing `qa_metrics-0.2.1/qa_metrics/__init__.py` & `qa_metrics-0.2.2/qa_metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `qa_metrics-0.2.1/qa_metrics/em.py` & `qa_metrics-0.2.2/qa_metrics/em.py`

 * *Files identical despite different names*

### Comparing `qa_metrics-0.2.1/qa_metrics/f1.py` & `qa_metrics-0.2.2/qa_metrics/f1.py`

 * *Files identical despite different names*

### Comparing `qa_metrics-0.2.1/qa_metrics/pedant.py` & `qa_metrics-0.2.2/qa_metrics/pedant.py`

 * *Files identical despite different names*

### Comparing `qa_metrics-0.2.1/qa_metrics/transformerMatcher.py` & `qa_metrics-0.2.2/qa_metrics/transformerMatcher.py`

 * *Files identical despite different names*

### Comparing `qa_metrics-0.2.1/qa_metrics/utils/tools.py` & `qa_metrics-0.2.2/qa_metrics/utils/tools.py`

 * *Files identical despite different names*

### Comparing `qa_metrics-0.2.1/qa_metrics.egg-info/PKG-INFO` & `qa_metrics-0.2.2/qa_metrics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qa-metrics
-Version: 0.2.1
+Version: 0.2.2
 Summary: This package provides standard and classifier-based short form QA evaluation methods
 Home-page: https://github.com/zli12321/qa_metrics
 Author: Zongxia Li
 Author-email: zli12321@umd.edu
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `qa_metrics-0.2.1/setup.py` & `qa_metrics-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 import os
 
 
 setup(
     name='qa_metrics',
-    version='0.2.1',
+    version='0.2.2',
     author='Zongxia Li',
     author_email='zli12321@umd.edu',
     description='This package provides standard and classifier-based short form QA evaluation methods',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/zli12321/qa_metrics',
     packages=find_packages(),
```

