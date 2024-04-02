# Comparing `tmp/fintorch-0.1.1.tar.gz` & `tmp/fintorch-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fintorch-0.1.1.tar", last modified: Tue Mar 19 09:26:39 2024, max compression
+gzip compressed data, was "fintorch-0.1.2.tar", last modified: Tue Apr  2 19:37:35 2024, max compression
```

## Comparing `fintorch-0.1.1.tar` & `fintorch-0.1.2.tar`

### file list

```diff
@@ -1,44 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:26:39.943632 fintorch-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-19 09:26:34.000000 fintorch-0.1.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-03-19 09:26:34.000000 fintorch-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-03-19 09:26:34.000000 fintorch-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5375 2024-03-19 09:26:39.943632 fintorch-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-03-19 09:26:34.000000 fintorch-0.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:26:39.939632 fintorch-0.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-03-19 09:26:34.000000 fintorch-0.1.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-19 09:26:34.000000 fintorch-0.1.1/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)     4218 2024-03-19 09:26:34.000000 fintorch-0.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-03-19 09:26:34.000000 fintorch-0.1.1/docs/console_script_setup.rst
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-19 09:26:34.000000 fintorch-0.1.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-03-19 09:26:34.000000 fintorch-0.1.1/docs/fintorch.dl.rst
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-03-19 09:26:34.000000 fintorch-0.1.1/docs/fintorch.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-19 09:26:34.000000 fintorch-0.1.1/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-03-19 09:26:34.000000 fintorch-0.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-03-19 09:26:34.000000 fintorch-0.1.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-03-19 09:26:34.000000 fintorch-0.1.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-19 09:26:34.000000 fintorch-0.1.1/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-19 09:26:34.000000 fintorch-0.1.1/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-03-19 09:26:34.000000 fintorch-0.1.1/docs/troubleshooting.rst
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-19 09:26:34.000000 fintorch-0.1.1/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:26:39.943632 fintorch-0.1.1/fintorch/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-19 09:26:34.000000 fintorch-0.1.1/fintorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-03-19 09:26:34.000000 fintorch-0.1.1/fintorch/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:26:39.943632 fintorch-0.1.1/fintorch/dl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 09:26:34.000000 fintorch-0.1.1/fintorch/dl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-19 09:26:34.000000 fintorch-0.1.1/fintorch/fintorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:26:39.943632 fintorch-0.1.1/fintorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5375 2024-03-19 09:26:39.000000 fintorch-0.1.1/fintorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-03-19 09:26:39.000000 fintorch-0.1.1/fintorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 09:26:39.000000 fintorch-0.1.1/fintorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-19 09:26:39.000000 fintorch-0.1.1/fintorch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 09:26:39.000000 fintorch-0.1.1/fintorch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-19 09:26:39.000000 fintorch-0.1.1/fintorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-19 09:26:39.000000 fintorch-0.1.1/fintorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-03-19 09:26:39.943632 fintorch-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-03-19 09:26:34.000000 fintorch-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:26:39.943632 fintorch-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 09:26:34.000000 fintorch-0.1.1/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 09:26:34.000000 fintorch-0.1.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:26:39.943632 fintorch-0.1.1/tests/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-03-19 09:26:34.000000 fintorch-0.1.1/tests/datasets/test_elliptic.py
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-03-19 09:26:34.000000 fintorch-0.1.1/tests/test_fintorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:37:35.347366 fintorch-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-02 19:37:28.000000 fintorch-0.1.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-02 19:37:28.000000 fintorch-0.1.2/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-02 19:37:28.000000 fintorch-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-02 19:37:28.000000 fintorch-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5329 2024-04-02 19:37:35.347366 fintorch-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-04-02 19:37:28.000000 fintorch-0.1.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:37:35.343366 fintorch-0.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-02 19:37:28.000000 fintorch-0.1.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-02 19:37:28.000000 fintorch-0.1.2/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4316 2024-04-02 19:37:28.000000 fintorch-0.1.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-02 19:37:28.000000 fintorch-0.1.2/docs/console_script_setup.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-02 19:37:28.000000 fintorch-0.1.2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-02 19:37:28.000000 fintorch-0.1.2/docs/fintorch.datasets.kaggle.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-02 19:37:28.000000 fintorch-0.1.2/docs/fintorch.datasets.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-02 19:37:28.000000 fintorch-0.1.2/docs/fintorch.dl.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-02 19:37:28.000000 fintorch-0.1.2/docs/fintorch.graph.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-02 19:37:28.000000 fintorch-0.1.2/docs/fintorch.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-02 19:37:28.000000 fintorch-0.1.2/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-02 19:37:28.000000 fintorch-0.1.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-02 19:37:28.000000 fintorch-0.1.2/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-02 19:37:28.000000 fintorch-0.1.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-02 19:37:28.000000 fintorch-0.1.2/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-02 19:37:28.000000 fintorch-0.1.2/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-02 19:37:28.000000 fintorch-0.1.2/docs/troubleshooting.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:37:35.335366 fintorch-0.1.2/docs/tutorials/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:37:35.343366 fintorch-0.1.2/docs/tutorials/elliptical/
+-rw-r--r--   0 runner    (1001) docker     (127)   265110 2024-04-02 19:37:28.000000 fintorch-0.1.2/docs/tutorials/elliptical/actorvizaddrtx.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    25070 2024-04-02 19:37:28.000000 fintorch-0.1.2/docs/tutorials/elliptical/graph.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-02 19:37:28.000000 fintorch-0.1.2/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:37:35.343366 fintorch-0.1.2/fintorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-02 19:37:28.000000 fintorch-0.1.2/fintorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-02 19:37:28.000000 fintorch-0.1.2/fintorch/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:37:35.343366 fintorch-0.1.2/fintorch/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:37:28.000000 fintorch-0.1.2/fintorch/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8190 2024-04-02 19:37:28.000000 fintorch-0.1.2/fintorch/datasets/elliptic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13062 2024-04-02 19:37:28.000000 fintorch-0.1.2/fintorch/datasets/ellipticpp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:37:35.347366 fintorch-0.1.2/fintorch/datasets/kaggle/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:37:28.000000 fintorch-0.1.2/fintorch/datasets/kaggle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-02 19:37:28.000000 fintorch-0.1.2/fintorch/datasets/kaggle/downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:37:35.347366 fintorch-0.1.2/fintorch/dl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:37:28.000000 fintorch-0.1.2/fintorch/dl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-02 19:37:28.000000 fintorch-0.1.2/fintorch/fintorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:37:35.347366 fintorch-0.1.2/fintorch/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:37:28.000000 fintorch-0.1.2/fintorch/graph/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:37:35.347366 fintorch-0.1.2/fintorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5329 2024-04-02 19:37:35.000000 fintorch-0.1.2/fintorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-02 19:37:35.000000 fintorch-0.1.2/fintorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 19:37:35.000000 fintorch-0.1.2/fintorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-02 19:37:35.000000 fintorch-0.1.2/fintorch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 19:37:35.000000 fintorch-0.1.2/fintorch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-02 19:37:35.000000 fintorch-0.1.2/fintorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-02 19:37:35.000000 fintorch-0.1.2/fintorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-02 19:37:35.347366 fintorch-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-02 19:37:28.000000 fintorch-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:37:35.347366 fintorch-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:37:28.000000 fintorch-0.1.2/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 19:37:28.000000 fintorch-0.1.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:37:35.347366 fintorch-0.1.2/tests/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-02 19:37:28.000000 fintorch-0.1.2/tests/datasets/test_elliptic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-04-02 19:37:28.000000 fintorch-0.1.2/tests/datasets/test_ellipticpp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-02 19:37:28.000000 fintorch-0.1.2/tests/test_cli.py
```

### Comparing `fintorch-0.1.1/LICENSE` & `fintorch-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fintorch-0.1.1/PKG-INFO` & `fintorch-0.1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: fintorch
-Version: 0.1.1
+Version: 0.1.2
 Summary: AI4FinTech project repository
-Home-page: https://github.com/boersmamarcel/fintorch
+Home-page: https://github.com/AI4FinTech/fintorch
 Author: Marcel Boersma
 Author-email: boersma.marcel@gmail.com
 License: MIT license
 Keywords: fintorch
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -17,18 +17,17 @@
 Requires-Dist: Click>=7.0
 Requires-Dist: torch
 Requires-Dist: torch_geometric
 Requires-Dist: pytorch_lightning
 Requires-Dist: kaggle
 Requires-Dist: polars
 Requires-Dist: numpy
-Provides-Extra: test
-Requires-Dist: pytest>=3; extra == "test"
-Provides-Extra: dev
-Requires-Dist: sphinx; extra == "dev"
+Requires-Dist: huggingface_hub
+Requires-Dist: seaborn
+Requires-Dist: networkx
 
 ========
 FinTorch
 ========
 
 
 .. image:: https://img.shields.io/pypi/v/fintorch.svg
@@ -50,15 +49,15 @@
 * Free software: MIT license
 * Documentation: https://fintorch.readthedocs.io.
 
 
 Features
 --------
 
-* TODO7
+* TODO8
 
 FinTorch - Machine Learning for FinTech
 =========================================
 
 The integration of AI in the financial sector demands specialized tools that can handle the unique challenges of this field, especially in regulatory compliance and risk management. Building on the familiarity and robustness of PyTorch, FinTorch aims to bridge the gap between AI technology and the financial industry needs.
 
 Goal
```

### Comparing `fintorch-0.1.1/README.rst` & `fintorch-0.1.2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 * Free software: MIT license
 * Documentation: https://fintorch.readthedocs.io.
 
 
 Features
 --------
 
-* TODO7
+* TODO8
 
 FinTorch - Machine Learning for FinTech
 =========================================
 
 The integration of AI in the financial sector demands specialized tools that can handle the unique challenges of this field, especially in regulatory compliance and risk management. Building on the familiarity and robustness of PyTorch, FinTorch aims to bridge the gap between AI technology and the financial industry needs.
 
 Goal
```

### Comparing `fintorch-0.1.1/docs/Makefile` & `fintorch-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fintorch-0.1.1/docs/conf.py` & `fintorch-0.1.2/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,22 @@
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
-extensions = ["sphinx.ext.autodoc", "sphinx.ext.viewcode", "nbsphinx"]
+extensions = [
+    "sphinx.ext.viewcode",
+    "nbsphinx",
+    "sphinx.ext.duration",
+    "sphinx.ext.doctest",
+    "sphinx.ext.autodoc",
+    "sphinx.ext.autosummary",
+]
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 #
```

### Comparing `fintorch-0.1.1/docs/console_script_setup.rst` & `fintorch-0.1.2/docs/console_script_setup.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Console script setup
-*********
+*********************
 
 .. _console-script-setup:
 
 
 Console Script Setup
-=================
+=====================
 
 Optionally, your package can include a console script using Click or argparse (Python 3.2+).
 
 How It Works
 ------------
 
 If the 'command_line_interface' option is set to ['click'] or ['argparse'] during setup, cookiecutter will
```

### Comparing `fintorch-0.1.1/docs/installation.rst` & `fintorch-0.1.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `fintorch-0.1.1/docs/make.bat` & `fintorch-0.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `fintorch-0.1.1/docs/troubleshooting.rst` & `fintorch-0.1.2/docs/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `fintorch-0.1.1/fintorch/cli.py` & `fintorch-0.1.2/fintorch/cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Console script for fintorch."""
 
 import click
 
 from fintorch.datasets import elliptic as e
+from fintorch.datasets import ellipticpp as epp
 
 
 @click.group()
 def fintorch():
     """FinTorch CLI - Your financial AI toolkit"""
     pass
 
@@ -14,15 +15,17 @@
 @fintorch.command()
 @click.argument("dataset")
 def datasets(dataset):
     """Download financial datasets"""
     # Implement your dataset download logic here
     click.echo(f"Downloading dataset: {dataset}")
     if dataset == "elliptic":
-        e.EllipticDataset("~/.fintorch_data", force_reload=True)
+        e.TransactionDataset("~/.fintorch_data", force_reload=True)
+    elif dataset == "ellipticpp":
+        epp.TransactionActorDataset("~/.fintorch_data", force_reload=True)
 
 
 @fintorch.command()
 @click.argument("model")
 def train(model):
     """Train financial models"""
     # Implement your model training logic here
```

### Comparing `fintorch-0.1.1/fintorch.egg-info/PKG-INFO` & `fintorch-0.1.2/fintorch.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: fintorch
-Version: 0.1.1
+Version: 0.1.2
 Summary: AI4FinTech project repository
-Home-page: https://github.com/boersmamarcel/fintorch
+Home-page: https://github.com/AI4FinTech/fintorch
 Author: Marcel Boersma
 Author-email: boersma.marcel@gmail.com
 License: MIT license
 Keywords: fintorch
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -17,18 +17,17 @@
 Requires-Dist: Click>=7.0
 Requires-Dist: torch
 Requires-Dist: torch_geometric
 Requires-Dist: pytorch_lightning
 Requires-Dist: kaggle
 Requires-Dist: polars
 Requires-Dist: numpy
-Provides-Extra: test
-Requires-Dist: pytest>=3; extra == "test"
-Provides-Extra: dev
-Requires-Dist: sphinx; extra == "dev"
+Requires-Dist: huggingface_hub
+Requires-Dist: seaborn
+Requires-Dist: networkx
 
 ========
 FinTorch
 ========
 
 
 .. image:: https://img.shields.io/pypi/v/fintorch.svg
@@ -50,15 +49,15 @@
 * Free software: MIT license
 * Documentation: https://fintorch.readthedocs.io.
 
 
 Features
 --------
 
-* TODO7
+* TODO8
 
 FinTorch - Machine Learning for FinTech
 =========================================
 
 The integration of AI in the financial sector demands specialized tools that can handle the unique challenges of this field, especially in regulatory compliance and risk management. Building on the familiarity and robustness of PyTorch, FinTorch aims to bridge the gap between AI technology and the financial industry needs.
 
 Goal
```

### Comparing `fintorch-0.1.1/fintorch.egg-info/SOURCES.txt` & `fintorch-0.1.2/fintorch.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,49 @@
+CONTRIBUTING.rst
 HISTORY.rst
 LICENSE
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 docs/Makefile
 docs/authors.rst
 docs/conf.py
 docs/console_script_setup.rst
 docs/contributing.rst
+docs/fintorch.datasets.kaggle.rst
+docs/fintorch.datasets.rst
 docs/fintorch.dl.rst
+docs/fintorch.graph.rst
 docs/fintorch.rst
 docs/history.rst
 docs/index.rst
 docs/installation.rst
 docs/make.bat
 docs/modules.rst
 docs/readme.rst
 docs/troubleshooting.rst
 docs/usage.rst
+docs/tutorials/elliptical/actorvizaddrtx.jpg
+docs/tutorials/elliptical/graph.jpg
 fintorch/__init__.py
 fintorch/cli.py
 fintorch/fintorch.py
 fintorch.egg-info/PKG-INFO
 fintorch.egg-info/SOURCES.txt
 fintorch.egg-info/dependency_links.txt
 fintorch.egg-info/entry_points.txt
 fintorch.egg-info/not-zip-safe
 fintorch.egg-info/requires.txt
 fintorch.egg-info/top_level.txt
+fintorch/datasets/__init__.py
+fintorch/datasets/elliptic.py
+fintorch/datasets/ellipticpp.py
+fintorch/datasets/kaggle/__init__.py
+fintorch/datasets/kaggle/downloader.py
 fintorch/dl/__init__.py
+fintorch/graph/__init__.py
 tests/README.md
 tests/__init__.py
-tests/test_fintorch.py
-tests/datasets/test_elliptic.py
+tests/test_cli.py
+tests/datasets/test_elliptic.py
+tests/datasets/test_ellipticpp.py
```

### Comparing `fintorch-0.1.1/setup.py` & `fintorch-0.1.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,22 +13,23 @@
     "Click>=7.0",
     "torch",
     "torch_geometric",
     "pytorch_lightning",
     "kaggle",
     "polars",
     "numpy",
+    "huggingface_hub",
+    "seaborn",
+    "networkx",
 ]
 
 test_requirements = [
     "pytest>=3",
 ]
 
-dev_requirements = ["sphinx"]
-
 setup(
     author="Marcel Boersma",
     author_email="boersma.marcel@gmail.com",
     python_requires=">=3.10",
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Intended Audience :: Developers",
@@ -47,12 +48,11 @@
     long_description=readme + "\n\n" + history,
     include_package_data=True,
     keywords="fintorch",
     name="fintorch",
     packages=find_packages(include=["fintorch", "fintorch.*"]),
     test_suite="tests",
     tests_require=test_requirements,
-    extras_require={"test": test_requirements, "dev": dev_requirements},
-    url="https://github.com/boersmamarcel/fintorch",
-    version="0.1.1",
+    url="https://github.com/AI4FinTech/fintorch",
+    version="0.1.2",
     zip_safe=False,
 )
```

### Comparing `fintorch-0.1.1/tests/datasets/test_elliptic.py` & `fintorch-0.1.2/tests/datasets/test_elliptic.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import os
 
 import pytest
 
-from fintorch.datasets.elliptic import EllipticDataset
+from fintorch.datasets.elliptic import TransactionDataset
 
 
 @pytest.fixture
 def dataset():
     root = "/tmp/data/fintorch/"
-    return EllipticDataset(root)
+    return TransactionDataset(root)
 
 
 def test_raw_file_names(dataset):
     expected_files = [
         "elliptic_bitcoin_dataset/elliptic_txs_features.csv",
         "elliptic_bitcoin_dataset/elliptic_txs_edgelist.csv",
         "elliptic_bitcoin_dataset/elliptic_txs_classes.csv",
     ]
     assert dataset.raw_file_names == expected_files
 
 
 def test_processed_file_names(dataset):
-    expected_files = ["data_v1.pt"]
+    expected_files = ["transaction_graph_v1.pt"]
     assert dataset.processed_file_names == expected_files
 
 
 def test_download(dataset):
     dataset.download()
     assert os.path.exists(dataset.raw_dir)
```

