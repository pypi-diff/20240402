# Comparing `tmp/torch-model-manager-0.0.1.dev1.tar.gz` & `tmp/torch-model-manager-0.0.1.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch-model-manager-0.0.1.dev1.tar", last modified: Tue Apr  2 21:04:33 2024, max compression
+gzip compressed data, was "torch-model-manager-0.0.1.dev2.tar", last modified: Tue Apr  2 21:27:48 2024, max compression
```

## Comparing `torch-model-manager-0.0.1.dev1.tar` & `torch-model-manager-0.0.1.dev2.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 21:04:33.743726 torch-model-manager-0.0.1.dev1/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2706 2024-04-02 21:04:33.743726 torch-model-manager-0.0.1.dev1/PKG-INFO
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2183 2024-04-02 16:34:05.000000 torch-model-manager-0.0.1.dev1/README.md
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 21:04:33.735726 torch-model-manager-0.0.1.dev1/core/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       52 2024-04-02 17:11:55.000000 torch-model-manager-0.0.1.dev1/core/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    11669 2024-04-02 16:34:05.000000 torch-model-manager-0.0.1.dev1/core/torch_model_manager.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-04-02 21:04:33.743726 torch-model-manager-0.0.1.dev1/setup.cfg
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      815 2024-04-02 21:04:16.000000 torch-model-manager-0.0.1.dev1/setup.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 21:04:33.739726 torch-model-manager-0.0.1.dev1/tests/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 16:34:05.000000 torch-model-manager-0.0.1.dev1/tests/__init__.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 21:04:33.739726 torch-model-manager-0.0.1.dev1/tests/test_core/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 16:34:05.000000 torch-model-manager-0.0.1.dev1/tests/test_core/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2447 2024-04-02 16:34:05.000000 torch-model-manager-0.0.1.dev1/tests/test_core/test_torch_model_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 21:04:33.739726 torch-model-manager-0.0.1.dev1/tests/test_utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 16:34:05.000000 torch-model-manager-0.0.1.dev1/tests/test_utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-04-02 16:34:05.000000 torch-model-manager-0.0.1.dev1/tests/test_utils/test_helpers.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 21:04:33.743726 torch-model-manager-0.0.1.dev1/torch_model_manager.egg-info/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2706 2024-04-02 21:04:33.000000 torch-model-manager-0.0.1.dev1/torch_model_manager.egg-info/PKG-INFO
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      464 2024-04-02 21:04:33.000000 torch-model-manager-0.0.1.dev1/torch_model_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-04-02 21:04:33.000000 torch-model-manager-0.0.1.dev1/torch_model_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       30 2024-04-02 21:04:33.000000 torch-model-manager-0.0.1.dev1/torch_model_manager.egg-info/requires.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       17 2024-04-02 21:04:33.000000 torch-model-manager-0.0.1.dev1/torch_model_manager.egg-info/top_level.txt
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 21:04:33.743726 torch-model-manager-0.0.1.dev1/utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 16:34:05.000000 torch-model-manager-0.0.1.dev1/utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     1585 2024-04-02 16:34:05.000000 torch-model-manager-0.0.1.dev1/utils/helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 21:27:48.176405 torch-model-manager-0.0.1.dev2/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2706 2024-04-02 21:27:48.176405 torch-model-manager-0.0.1.dev2/PKG-INFO
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2183 2024-04-02 16:34:05.000000 torch-model-manager-0.0.1.dev2/README.md
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-04-02 21:27:48.176405 torch-model-manager-0.0.1.dev2/setup.cfg
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      840 2024-04-02 21:25:35.000000 torch-model-manager-0.0.1.dev2/setup.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 21:27:48.164405 torch-model-manager-0.0.1.dev2/tests/
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 21:27:48.168405 torch-model-manager-0.0.1.dev2/tests/test_torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 16:34:05.000000 torch-model-manager-0.0.1.dev2/tests/test_torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-04-02 21:24:16.000000 torch-model-manager-0.0.1.dev2/tests/test_torch_model_manager/test_torch_model_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 21:27:48.172405 torch-model-manager-0.0.1.dev2/tests/test_utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 16:34:05.000000 torch-model-manager-0.0.1.dev2/tests/test_utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-04-02 16:34:05.000000 torch-model-manager-0.0.1.dev2/tests/test_utils/test_helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 21:27:48.172405 torch-model-manager-0.0.1.dev2/torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       52 2024-04-02 17:11:55.000000 torch-model-manager-0.0.1.dev2/torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    11669 2024-04-02 16:34:05.000000 torch-model-manager-0.0.1.dev2/torch_model_manager/torch_model_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 21:27:48.176405 torch-model-manager-0.0.1.dev2/torch_model_manager.egg-info/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2706 2024-04-02 21:27:48.000000 torch-model-manager-0.0.1.dev2/torch_model_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      506 2024-04-02 21:27:48.000000 torch-model-manager-0.0.1.dev2/torch_model_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-04-02 21:27:48.000000 torch-model-manager-0.0.1.dev2/torch_model_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       30 2024-04-02 21:27:48.000000 torch-model-manager-0.0.1.dev2/torch_model_manager.egg-info/requires.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-04-02 21:27:48.000000 torch-model-manager-0.0.1.dev2/torch_model_manager.egg-info/top_level.txt
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 21:27:48.176405 torch-model-manager-0.0.1.dev2/utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 16:34:05.000000 torch-model-manager-0.0.1.dev2/utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     1585 2024-04-02 16:34:05.000000 torch-model-manager-0.0.1.dev2/utils/helpers.py
```

### Comparing `torch-model-manager-0.0.1.dev1/PKG-INFO` & `torch-model-manager-0.0.1.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.0.1.dev1
+Version: 0.0.1.dev2
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `torch-model-manager-0.0.1.dev1/README.md` & `torch-model-manager-0.0.1.dev2/README.md`

 * *Files identical despite different names*

### Comparing `torch-model-manager-0.0.1.dev1/core/torch_model_manager.py` & `torch-model-manager-0.0.1.dev2/torch_model_manager/torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch-model-manager-0.0.1.dev1/setup.py` & `torch-model-manager-0.0.1.dev2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='torch-model-manager',
-    version='0.0.1.dev1',
+    version='0.0.1.dev2',
     description='A package for managing PyTorch models',
     author='Billal MOKHTARI',
     author_email='mokhtaribillal1@gmail.com',
-    packages=find_packages(),
+    packages=find_packages(exclude=['tests', 'docs']),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url = 'https://github.com/Billal-MOKHTARI/torch-model-manager',
     install_requires=[
         'torch',
         'numpy',
         'torchvision',
```

### Comparing `torch-model-manager-0.0.1.dev1/tests/test_core/test_torch_model_manager.py` & `torch-model-manager-0.0.1.dev2/tests/test_torch_model_manager/test_torch_model_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import unittest
 import pytest
 import sys
 import os
 sys.path.append(os.path.abspath(os.path.join(os.path.dirname(__file__), '../..')))
-from core import torch_model_manager
+from torch_model_manager import torch_model_manager
 
 from torchvision import models
 import torch.nn as nn
 
 class TestTorchModelManager(unittest.TestCase):
     def setUp(self) -> None:
         self.model = models.vgg16(pretrained=True)
```

### Comparing `torch-model-manager-0.0.1.dev1/tests/test_utils/test_helpers.py` & `torch-model-manager-0.0.1.dev2/tests/test_utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `torch-model-manager-0.0.1.dev1/torch_model_manager.egg-info/PKG-INFO` & `torch-model-manager-0.0.1.dev2/torch_model_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.0.1.dev1
+Version: 0.0.1.dev2
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `torch-model-manager-0.0.1.dev1/utils/helpers.py` & `torch-model-manager-0.0.1.dev2/utils/helpers.py`

 * *Files identical despite different names*

