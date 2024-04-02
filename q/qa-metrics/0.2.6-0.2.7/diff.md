# Comparing `tmp/qa_metrics-0.2.6.tar.gz` & `tmp/qa_metrics-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qa_metrics-0.2.6.tar", last modified: Tue Apr  2 05:48:32 2024, max compression
+gzip compressed data, was "qa_metrics-0.2.7.tar", last modified: Tue Apr  2 05:56:10 2024, max compression
```

## Comparing `qa_metrics-0.2.6.tar` & `qa_metrics-0.2.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwsr-x   0 zli12321 (14416) activetopic (18517)        0 2024-04-02 05:48:32.588061 qa_metrics-0.2.6/
--rw-rw-r--   0 zli12321 (14416) activetopic (18517)     1071 2024-04-02 05:44:57.000000 qa_metrics-0.2.6/LICENSE
--rw-rw-r--   0 zli12321 (14416) activetopic (18517)       69 2024-04-02 05:44:57.000000 qa_metrics-0.2.6/MANIFEST.in
--rw-r--r--   0 zli12321 (14416) activetopic (18517)     8579 2024-04-02 05:48:32.588061 qa_metrics-0.2.6/PKG-INFO
--rw-rw-r--   0 zli12321 (14416) activetopic (18517)     7749 2024-04-02 05:44:57.000000 qa_metrics-0.2.6/README.md
-drwxrwsr-x   0 zli12321 (14416) activetopic (18517)        0 2024-04-02 05:48:32.587061 qa_metrics-0.2.6/qa_metrics/
--rw-rw-r--   0 zli12321 (14416) activetopic (18517)     2324 2024-04-02 05:44:57.000000 qa_metrics-0.2.6/qa_metrics/__init__.py
--rw-rw-r--   0 zli12321 (14416) activetopic (18517)     1122 2024-04-02 05:44:57.000000 qa_metrics-0.2.6/qa_metrics/em.py
--rw-rw-r--   0 zli12321 (14416) activetopic (18517)     2853 2024-04-02 05:44:57.000000 qa_metrics-0.2.6/qa_metrics/f1.py
--rw-rw-r--   0 zli12321 (14416) activetopic (18517)    15909 2024-04-02 05:44:58.000000 qa_metrics-0.2.6/qa_metrics/pedant.py
--rw-rw-r--   0 zli12321 (14416) activetopic (18517)     6541 2024-04-02 05:44:57.000000 qa_metrics-0.2.6/qa_metrics/prompt_llm.py
--rw-rw-r--   0 zli12321 (14416) activetopic (18517)     1201 2024-04-02 05:44:58.000000 qa_metrics-0.2.6/qa_metrics/prompt_open_llm.py
--rw-rw-r--   0 zli12321 (14416) activetopic (18517)    14173 2024-04-02 05:44:58.000000 qa_metrics-0.2.6/qa_metrics/transformerMatcher.py
-drwxrwsr-x   0 zli12321 (14416) activetopic (18517)        0 2024-04-02 05:48:32.588061 qa_metrics-0.2.6/qa_metrics/utils/
--rw-rw-r--   0 zli12321 (14416) activetopic (18517)        0 2024-04-02 05:44:57.000000 qa_metrics-0.2.6/qa_metrics/utils/__init__.py
--rw-rw-r--   0 zli12321 (14416) activetopic (18517)     2724 2024-04-02 05:44:58.000000 qa_metrics-0.2.6/qa_metrics/utils/tools.py
-drwxrwsr-x   0 zli12321 (14416) activetopic (18517)        0 2024-04-02 05:48:32.587061 qa_metrics-0.2.6/qa_metrics.egg-info/
--rw-r--r--   0 zli12321 (14416) activetopic (18517)     8579 2024-04-02 05:48:32.000000 qa_metrics-0.2.6/qa_metrics.egg-info/PKG-INFO
--rw-rw-r--   0 zli12321 (14416) activetopic (18517)      428 2024-04-02 05:48:32.000000 qa_metrics-0.2.6/qa_metrics.egg-info/SOURCES.txt
--rw-rw-r--   0 zli12321 (14416) activetopic (18517)        1 2024-04-02 05:48:32.000000 qa_metrics-0.2.6/qa_metrics.egg-info/dependency_links.txt
--rw-rw-r--   0 zli12321 (14416) activetopic (18517)       75 2024-04-02 05:48:32.000000 qa_metrics-0.2.6/qa_metrics.egg-info/requires.txt
--rw-rw-r--   0 zli12321 (14416) activetopic (18517)       11 2024-04-02 05:48:32.000000 qa_metrics-0.2.6/qa_metrics.egg-info/top_level.txt
--rw-rw-r--   0 zli12321 (14416) activetopic (18517)       38 2024-04-02 05:48:32.588061 qa_metrics-0.2.6/setup.cfg
--rw-rw-r--   0 zli12321 (14416) activetopic (18517)     1296 2024-04-02 05:48:22.000000 qa_metrics-0.2.6/setup.py
+drwxrwsr-x   0 zli12321 (14416) activetopic (18517)        0 2024-04-02 05:56:10.823579 qa_metrics-0.2.7/
+-rw-rw-r--   0 zli12321 (14416) activetopic (18517)     1071 2024-04-02 05:44:57.000000 qa_metrics-0.2.7/LICENSE
+-rw-rw-r--   0 zli12321 (14416) activetopic (18517)       69 2024-04-02 05:44:57.000000 qa_metrics-0.2.7/MANIFEST.in
+-rw-r--r--   0 zli12321 (14416) activetopic (18517)     8579 2024-04-02 05:56:10.823579 qa_metrics-0.2.7/PKG-INFO
+-rw-rw-r--   0 zli12321 (14416) activetopic (18517)     7749 2024-04-02 05:44:57.000000 qa_metrics-0.2.7/README.md
+drwxrwsr-x   0 zli12321 (14416) activetopic (18517)        0 2024-04-02 05:56:10.822579 qa_metrics-0.2.7/qa_metrics/
+-rw-rw-r--   0 zli12321 (14416) activetopic (18517)     2324 2024-04-02 05:44:57.000000 qa_metrics-0.2.7/qa_metrics/__init__.py
+-rw-rw-r--   0 zli12321 (14416) activetopic (18517)     1122 2024-04-02 05:44:57.000000 qa_metrics-0.2.7/qa_metrics/em.py
+-rw-rw-r--   0 zli12321 (14416) activetopic (18517)     2853 2024-04-02 05:44:57.000000 qa_metrics-0.2.7/qa_metrics/f1.py
+-rw-rw-r--   0 zli12321 (14416) activetopic (18517)    15909 2024-04-02 05:44:58.000000 qa_metrics-0.2.7/qa_metrics/pedant.py
+-rw-rw-r--   0 zli12321 (14416) activetopic (18517)     6541 2024-04-02 05:53:35.000000 qa_metrics-0.2.7/qa_metrics/prompt_llm.py
+-rw-rw-r--   0 zli12321 (14416) activetopic (18517)     1201 2024-04-02 05:44:58.000000 qa_metrics-0.2.7/qa_metrics/prompt_open_llm.py
+-rw-rw-r--   0 zli12321 (14416) activetopic (18517)    14173 2024-04-02 05:44:58.000000 qa_metrics-0.2.7/qa_metrics/transformerMatcher.py
+drwxrwsr-x   0 zli12321 (14416) activetopic (18517)        0 2024-04-02 05:56:10.823579 qa_metrics-0.2.7/qa_metrics/utils/
+-rw-rw-r--   0 zli12321 (14416) activetopic (18517)        0 2024-04-02 05:44:57.000000 qa_metrics-0.2.7/qa_metrics/utils/__init__.py
+-rw-rw-r--   0 zli12321 (14416) activetopic (18517)     2724 2024-04-02 05:44:58.000000 qa_metrics-0.2.7/qa_metrics/utils/tools.py
+drwxrwsr-x   0 zli12321 (14416) activetopic (18517)        0 2024-04-02 05:56:10.823579 qa_metrics-0.2.7/qa_metrics.egg-info/
+-rw-r--r--   0 zli12321 (14416) activetopic (18517)     8579 2024-04-02 05:56:10.000000 qa_metrics-0.2.7/qa_metrics.egg-info/PKG-INFO
+-rw-rw-r--   0 zli12321 (14416) activetopic (18517)      428 2024-04-02 05:56:10.000000 qa_metrics-0.2.7/qa_metrics.egg-info/SOURCES.txt
+-rw-rw-r--   0 zli12321 (14416) activetopic (18517)        1 2024-04-02 05:56:10.000000 qa_metrics-0.2.7/qa_metrics.egg-info/dependency_links.txt
+-rw-rw-r--   0 zli12321 (14416) activetopic (18517)       75 2024-04-02 05:56:10.000000 qa_metrics-0.2.7/qa_metrics.egg-info/requires.txt
+-rw-rw-r--   0 zli12321 (14416) activetopic (18517)       11 2024-04-02 05:56:10.000000 qa_metrics-0.2.7/qa_metrics.egg-info/top_level.txt
+-rw-rw-r--   0 zli12321 (14416) activetopic (18517)       38 2024-04-02 05:56:10.823579 qa_metrics-0.2.7/setup.cfg
+-rw-rw-r--   0 zli12321 (14416) activetopic (18517)     1296 2024-04-02 05:56:00.000000 qa_metrics-0.2.7/setup.py
```

### Comparing `qa_metrics-0.2.6/LICENSE` & `qa_metrics-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `qa_metrics-0.2.6/PKG-INFO` & `qa_metrics-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qa_metrics
-Version: 0.2.6
+Version: 0.2.7
 Summary: This package provides standard and classifier-based short form QA evaluation methods
 Home-page: https://github.com/zli12321/qa_metrics
 Author: Zongxia Li
 Author-email: zli12321@umd.edu
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `qa_metrics-0.2.6/README.md` & `qa_metrics-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `qa_metrics-0.2.6/qa_metrics/__init__.py` & `qa_metrics-0.2.7/qa_metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `qa_metrics-0.2.6/qa_metrics/em.py` & `qa_metrics-0.2.7/qa_metrics/em.py`

 * *Files identical despite different names*

### Comparing `qa_metrics-0.2.6/qa_metrics/f1.py` & `qa_metrics-0.2.7/qa_metrics/f1.py`

 * *Files identical despite different names*

### Comparing `qa_metrics-0.2.6/qa_metrics/pedant.py` & `qa_metrics-0.2.7/qa_metrics/pedant.py`

 * *Files identical despite different names*

### Comparing `qa_metrics-0.2.6/qa_metrics/prompt_llm.py` & `qa_metrics-0.2.7/qa_metrics/prompt_llm.py`

 * *Files identical despite different names*

### Comparing `qa_metrics-0.2.6/qa_metrics/prompt_open_llm.py` & `qa_metrics-0.2.7/qa_metrics/prompt_open_llm.py`

 * *Files identical despite different names*

### Comparing `qa_metrics-0.2.6/qa_metrics/transformerMatcher.py` & `qa_metrics-0.2.7/qa_metrics/transformerMatcher.py`

 * *Files identical despite different names*

### Comparing `qa_metrics-0.2.6/qa_metrics/utils/tools.py` & `qa_metrics-0.2.7/qa_metrics/utils/tools.py`

 * *Files identical despite different names*

### Comparing `qa_metrics-0.2.6/qa_metrics.egg-info/PKG-INFO` & `qa_metrics-0.2.7/qa_metrics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qa-metrics
-Version: 0.2.6
+Version: 0.2.7
 Summary: This package provides standard and classifier-based short form QA evaluation methods
 Home-page: https://github.com/zli12321/qa_metrics
 Author: Zongxia Li
 Author-email: zli12321@umd.edu
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `qa_metrics-0.2.6/setup.py` & `qa_metrics-0.2.7/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 import os
 
 
 setup(
     name='qa_metrics',
-    version='0.2.6',
+    version='0.2.7',
     author='Zongxia Li',
     author_email='zli12321@umd.edu',
     description='This package provides standard and classifier-based short form QA evaluation methods',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/zli12321/qa_metrics',
     packages=find_packages(),
```

