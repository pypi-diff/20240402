# Comparing `tmp/torch-model-manager-0.0.1.tar.gz` & `tmp/torch-model-manager-1.0.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch-model-manager-0.0.1.tar", last modified: Tue Apr  2 21:00:44 2024, max compression
+gzip compressed data, was "torch-model-manager-1.0.0.dev1.tar", last modified: Tue Apr  2 20:13:11 2024, max compression
```

## Comparing `torch-model-manager-0.0.1.tar` & `torch-model-manager-1.0.0.dev1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 21:00:44.213685 torch-model-manager-0.0.1/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2647 2024-04-02 21:00:44.213685 torch-model-manager-0.0.1/PKG-INFO
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2183 2024-04-02 16:34:05.000000 torch-model-manager-0.0.1/README.md
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 21:00:44.209685 torch-model-manager-0.0.1/core/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       52 2024-04-02 17:11:55.000000 torch-model-manager-0.0.1/core/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    11669 2024-04-02 16:34:05.000000 torch-model-manager-0.0.1/core/torch_model_manager.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-04-02 21:00:44.213685 torch-model-manager-0.0.1/setup.cfg
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      810 2024-04-02 20:58:30.000000 torch-model-manager-0.0.1/setup.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 21:00:44.209685 torch-model-manager-0.0.1/tests/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 16:34:05.000000 torch-model-manager-0.0.1/tests/__init__.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 21:00:44.209685 torch-model-manager-0.0.1/tests/test_core/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 16:34:05.000000 torch-model-manager-0.0.1/tests/test_core/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2447 2024-04-02 16:34:05.000000 torch-model-manager-0.0.1/tests/test_core/test_torch_model_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 21:00:44.209685 torch-model-manager-0.0.1/tests/test_utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 16:34:05.000000 torch-model-manager-0.0.1/tests/test_utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-04-02 16:34:05.000000 torch-model-manager-0.0.1/tests/test_utils/test_helpers.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 21:00:44.209685 torch-model-manager-0.0.1/torch_model_manager.egg-info/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2647 2024-04-02 21:00:44.000000 torch-model-manager-0.0.1/torch_model_manager.egg-info/PKG-INFO
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      464 2024-04-02 21:00:44.000000 torch-model-manager-0.0.1/torch_model_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-04-02 21:00:44.000000 torch-model-manager-0.0.1/torch_model_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       30 2024-04-02 21:00:44.000000 torch-model-manager-0.0.1/torch_model_manager.egg-info/requires.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       17 2024-04-02 21:00:44.000000 torch-model-manager-0.0.1/torch_model_manager.egg-info/top_level.txt
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 21:00:44.209685 torch-model-manager-0.0.1/utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 16:34:05.000000 torch-model-manager-0.0.1/utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     1585 2024-04-02 16:34:05.000000 torch-model-manager-0.0.1/utils/helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 20:13:11.772280 torch-model-manager-1.0.0.dev1/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      481 2024-04-02 20:13:11.772280 torch-model-manager-1.0.0.dev1/PKG-INFO
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2183 2024-04-02 16:34:05.000000 torch-model-manager-1.0.0.dev1/README.md
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 20:13:11.768280 torch-model-manager-1.0.0.dev1/core/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       52 2024-04-02 17:11:55.000000 torch-model-manager-1.0.0.dev1/core/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    11669 2024-04-02 16:34:05.000000 torch-model-manager-1.0.0.dev1/core/torch_model_manager.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-04-02 20:13:11.772280 torch-model-manager-1.0.0.dev1/setup.cfg
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      656 2024-04-02 19:54:15.000000 torch-model-manager-1.0.0.dev1/setup.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 20:13:11.768280 torch-model-manager-1.0.0.dev1/tests/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 16:34:05.000000 torch-model-manager-1.0.0.dev1/tests/__init__.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 20:13:11.768280 torch-model-manager-1.0.0.dev1/tests/test_core/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 16:34:05.000000 torch-model-manager-1.0.0.dev1/tests/test_core/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2447 2024-04-02 16:34:05.000000 torch-model-manager-1.0.0.dev1/tests/test_core/test_torch_model_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 20:13:11.768280 torch-model-manager-1.0.0.dev1/tests/test_utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 16:34:05.000000 torch-model-manager-1.0.0.dev1/tests/test_utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-04-02 16:34:05.000000 torch-model-manager-1.0.0.dev1/tests/test_utils/test_helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 20:13:11.772280 torch-model-manager-1.0.0.dev1/torch_model_manager.egg-info/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      481 2024-04-02 20:13:11.000000 torch-model-manager-1.0.0.dev1/torch_model_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      464 2024-04-02 20:13:11.000000 torch-model-manager-1.0.0.dev1/torch_model_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-04-02 20:13:11.000000 torch-model-manager-1.0.0.dev1/torch_model_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       30 2024-04-02 20:13:11.000000 torch-model-manager-1.0.0.dev1/torch_model_manager.egg-info/requires.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       17 2024-04-02 20:13:11.000000 torch-model-manager-1.0.0.dev1/torch_model_manager.egg-info/top_level.txt
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 20:13:11.772280 torch-model-manager-1.0.0.dev1/utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-02 16:34:05.000000 torch-model-manager-1.0.0.dev1/utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     1585 2024-04-02 16:34:05.000000 torch-model-manager-1.0.0.dev1/utils/helpers.py
```

### Comparing `torch-model-manager-0.0.1/README.md` & `torch-model-manager-1.0.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `torch-model-manager-0.0.1/core/torch_model_manager.py` & `torch-model-manager-1.0.0.dev1/core/torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch-model-manager-0.0.1/tests/test_core/test_torch_model_manager.py` & `torch-model-manager-1.0.0.dev1/tests/test_core/test_torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch-model-manager-0.0.1/tests/test_utils/test_helpers.py` & `torch-model-manager-1.0.0.dev1/tests/test_utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `torch-model-manager-0.0.1/utils/helpers.py` & `torch-model-manager-1.0.0.dev1/utils/helpers.py`

 * *Files identical despite different names*

