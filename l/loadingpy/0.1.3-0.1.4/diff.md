# Comparing `tmp/loadingpy-0.1.3.tar.gz` & `tmp/loadingpy-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loadingpy-0.1.3.tar", last modified: Mon Jan 29 08:40:06 2024, max compression
+gzip compressed data, was "loadingpy-0.1.4.tar", max compression
```

## Comparing `loadingpy-0.1.3.tar` & `loadingpy-0.1.4.tar`

### file list

```diff
@@ -1,22 +1,10 @@
-drwxr-xr-x   0 wared      (501) staff       (20)        0 2024-01-29 08:40:06.243687 loadingpy-0.1.3/
--rw-r--r--   0 wared      (501) staff       (20)     1070 2024-01-29 08:36:41.000000 loadingpy-0.1.3/LICENCE
--rw-r--r--   0 wared      (501) staff       (20)     2732 2024-01-29 08:40:06.243430 loadingpy-0.1.3/PKG-INFO
--rw-r--r--   0 wared      (501) staff       (20)     2460 2024-01-29 08:36:41.000000 loadingpy-0.1.3/README.md
--rw-r--r--   0 wared      (501) staff       (20)      442 2024-01-29 08:37:05.000000 loadingpy-0.1.3/pyproject.toml
--rw-r--r--   0 wared      (501) staff       (20)       38 2024-01-29 08:40:06.243745 loadingpy-0.1.3/setup.cfg
-drwxr-xr-x   0 wared      (501) staff       (20)        0 2024-01-29 08:40:06.239755 loadingpy-0.1.3/src/
-drwxr-xr-x   0 wared      (501) staff       (20)        0 2024-01-29 08:40:06.241838 loadingpy-0.1.3/src/loadingpy/
--rw-r--r--   0 wared      (501) staff       (20)      183 2024-01-29 08:36:41.000000 loadingpy-0.1.3/src/loadingpy/__init__.py
--rw-r--r--   0 wared      (501) staff       (20)      243 2024-01-29 08:36:41.000000 loadingpy-0.1.3/src/loadingpy/alias.py
--rw-r--r--   0 wared      (501) staff       (20)     6578 2024-01-29 08:36:41.000000 loadingpy-0.1.3/src/loadingpy/basic_bar.py
--rw-r--r--   0 wared      (501) staff       (20)     1599 2024-01-29 08:36:41.000000 loadingpy-0.1.3/src/loadingpy/colored_bar.py
--rw-r--r--   0 wared      (501) staff       (20)     3773 2024-01-29 08:36:41.000000 loadingpy-0.1.3/src/loadingpy/loading_bar.py
--rw-r--r--   0 wared      (501) staff       (20)        0 2024-01-29 08:36:41.000000 loadingpy-0.1.3/src/loadingpy/py.typed
--rw-r--r--   0 wared      (501) staff       (20)     4382 2024-01-29 08:37:19.000000 loadingpy-0.1.3/src/loadingpy/training_bar.py
-drwxr-xr-x   0 wared      (501) staff       (20)        0 2024-01-29 08:40:06.243186 loadingpy-0.1.3/src/loadingpy.egg-info/
--rw-r--r--   0 wared      (501) staff       (20)     2732 2024-01-29 08:40:06.000000 loadingpy-0.1.3/src/loadingpy.egg-info/PKG-INFO
--rw-r--r--   0 wared      (501) staff       (20)      391 2024-01-29 08:40:06.000000 loadingpy-0.1.3/src/loadingpy.egg-info/SOURCES.txt
--rw-r--r--   0 wared      (501) staff       (20)        1 2024-01-29 08:40:06.000000 loadingpy-0.1.3/src/loadingpy.egg-info/dependency_links.txt
--rw-r--r--   0 wared      (501) staff       (20)       10 2024-01-29 08:40:06.000000 loadingpy-0.1.3/src/loadingpy.egg-info/top_level.txt
-drwxr-xr-x   0 wared      (501) staff       (20)        0 2024-01-29 08:40:06.242670 loadingpy-0.1.3/tests/
--rw-r--r--   0 wared      (501) staff       (20)     2185 2024-01-29 08:36:41.000000 loadingpy-0.1.3/tests/test_loadingpy.py
+-rw-r--r--   0        0        0     2460 2024-01-29 08:36:41.239047 loadingpy-0.1.4/README.md
+-rw-r--r--   0        0        0      349 2024-04-02 16:02:10.670421 loadingpy-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      183 2024-01-29 08:36:41.239386 loadingpy-0.1.4/src/loadingpy/__init__.py
+-rw-r--r--   0        0        0      243 2024-01-29 08:36:41.239447 loadingpy-0.1.4/src/loadingpy/alias.py
+-rw-r--r--   0        0        0     6578 2024-01-29 08:36:41.239608 loadingpy-0.1.4/src/loadingpy/basic_bar.py
+-rw-r--r--   0        0        0     1599 2024-01-29 08:36:41.239748 loadingpy-0.1.4/src/loadingpy/colored_bar.py
+-rw-r--r--   0        0        0     4973 2024-04-02 15:43:14.261502 loadingpy-0.1.4/src/loadingpy/loading_bar.py
+-rw-r--r--   0        0        0        0 2024-01-29 08:36:41.239944 loadingpy-0.1.4/src/loadingpy/py.typed
+-rw-r--r--   0        0        0     4382 2024-01-29 08:37:19.654308 loadingpy-0.1.4/src/loadingpy/training_bar.py
+-rw-r--r--   0        0        0     3020 1970-01-01 00:00:00.000000 loadingpy-0.1.4/PKG-INFO
```

### Comparing `loadingpy-0.1.3/PKG-INFO` & `loadingpy-0.1.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: loadingpy
-Version: 0.1.3
-Summary: fancy progress bar
-Author-email: Edouard Yvinec <edouardyvinec@hotmail.fr>
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENCE
-
 # loadingpy
 
 In this repository, we provide a custom made progress bar for python iterables. This library can be used as is or modified for any purposes (see licence).
 
 ## for deep learning
 
 There is now a new progress bar available for deep learning purposes (I guess it could be leveraged for other stuff as well...). Say, you want to train a model using a dataset $D$ over $e$ epochs. Using `TrainBar`you can get a double progress bar (first for the epochs and second for the steps in the current epoch) on a single line. you can check the [test](tests/test_loadingpy.py) or this simple example:
@@ -55,8 +45,8 @@
 | argument | description | type |
 | :---: | :---: | :---: |
 | iterable | python object that can be iterated over | can be a list, tuple, range, np.ndarray, torch.Tensor, dataset,... |
 | monitoring | a python object (or list of python objects) that will be printed after each iteration using the following format f'{monitoring}'. IF they are updated during the loop, make sure to update inplace, in order to see the changes | an be a tensor, float or list of these |
 | naming | if you want to add a descritpion prefix to the monitoring variables | str or list of str |
 | total_steps | number of iterations to perform (if you set it to a lower value than the length of the iterable, then the process will stop after the given total_steps) | int |
 | base_str | prefix description of the loop we are iterating over | str |
-| color | which color to use for the loading bar | str |
+| color | which color to use for the loading bar | str |
```

### Comparing `loadingpy-0.1.3/README.md` & `loadingpy-0.1.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: loadingpy
+Version: 0.1.4
+Summary: 
+License: MIT
+Author: Edouard Yvinec
+Author-email: edouardyvinec@hotmail.fr
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Description-Content-Type: text/markdown
+
 # loadingpy
 
 In this repository, we provide a custom made progress bar for python iterables. This library can be used as is or modified for any purposes (see licence).
 
 ## for deep learning
 
 There is now a new progress bar available for deep learning purposes (I guess it could be leveraged for other stuff as well...). Say, you want to train a model using a dataset $D$ over $e$ epochs. Using `TrainBar`you can get a double progress bar (first for the epochs and second for the steps in the current epoch) on a single line. you can check the [test](tests/test_loadingpy.py) or this simple example:
@@ -45,8 +62,8 @@
 | argument | description | type |
 | :---: | :---: | :---: |
 | iterable | python object that can be iterated over | can be a list, tuple, range, np.ndarray, torch.Tensor, dataset,... |
 | monitoring | a python object (or list of python objects) that will be printed after each iteration using the following format f'{monitoring}'. IF they are updated during the loop, make sure to update inplace, in order to see the changes | an be a tensor, float or list of these |
 | naming | if you want to add a descritpion prefix to the monitoring variables | str or list of str |
 | total_steps | number of iterations to perform (if you set it to a lower value than the length of the iterable, then the process will stop after the given total_steps) | int |
 | base_str | prefix description of the loop we are iterating over | str |
-| color | which color to use for the loading bar | str |
+| color | which color to use for the loading bar | str |
```

### Comparing `loadingpy-0.1.3/src/loadingpy/basic_bar.py` & `loadingpy-0.1.4/src/loadingpy/basic_bar.py`

 * *Files identical despite different names*

### Comparing `loadingpy-0.1.3/src/loadingpy/colored_bar.py` & `loadingpy-0.1.4/src/loadingpy/colored_bar.py`

 * *Files identical despite different names*

### Comparing `loadingpy-0.1.3/src/loadingpy/training_bar.py` & `loadingpy-0.1.4/src/loadingpy/training_bar.py`

 * *Files identical despite different names*

