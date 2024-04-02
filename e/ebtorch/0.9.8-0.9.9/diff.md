# Comparing `tmp/ebtorch-0.9.8.tar.gz` & `tmp/ebtorch-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebtorch-0.9.8.tar", last modified: Sat Aug 12 03:22:40 2023, max compression
+gzip compressed data, was "ebtorch-0.9.9.tar", last modified: Sat Aug 12 03:30:44 2023, max compression
```

## Comparing `ebtorch-0.9.8.tar` & `ebtorch-0.9.9.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-12 03:22:40.463837 ebtorch-0.9.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-08-12 03:22:30.000000 ebtorch-0.9.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-08-12 03:22:40.459837 ebtorch-0.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-08-12 03:22:30.000000 ebtorch-0.9.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-12 03:22:40.447836 ebtorch-0.9.8/ebtorch/
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-08-12 03:22:30.000000 ebtorch-0.9.8/ebtorch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-12 03:22:40.451836 ebtorch-0.9.8/ebtorch/data/
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-08-12 03:22:30.000000 ebtorch-0.9.8/ebtorch/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16875 2023-08-12 03:22:30.000000 ebtorch-0.9.8/ebtorch/data/cutmixup.py
--rw-r--r--   0 runner    (1001) docker     (123)     8055 2023-08-12 03:22:30.000000 ebtorch-0.9.8/ebtorch/data/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-12 03:22:40.451836 ebtorch-0.9.8/ebtorch/logging/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-08-12 03:22:30.000000 ebtorch-0.9.8/ebtorch/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-08-12 03:22:30.000000 ebtorch-0.9.8/ebtorch/logging/avgmeter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-08-12 03:22:30.000000 ebtorch-0.9.8/ebtorch/logging/logcsv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-12 03:22:40.455836 ebtorch-0.9.8/ebtorch/nn/
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-08-12 03:22:30.000000 ebtorch-0.9.8/ebtorch/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13998 2023-08-12 03:22:30.000000 ebtorch-0.9.8/ebtorch/nn/architectures.py
--rw-r--r--   0 runner    (1001) docker     (123)    14741 2023-08-12 03:22:30.000000 ebtorch-0.9.8/ebtorch/nn/architectures_resnets_dm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7411 2023-08-12 03:22:30.000000 ebtorch-0.9.8/ebtorch/nn/conv2drp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-08-12 03:22:30.000000 ebtorch-0.9.8/ebtorch/nn/convolutional_flatten.py
--rw-r--r--   0 runner    (1001) docker     (123)    13699 2023-08-12 03:22:30.000000 ebtorch-0.9.8/ebtorch/nn/coordconv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-08-12 03:22:30.000000 ebtorch-0.9.8/ebtorch/nn/debuglayers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-08-12 03:22:30.000000 ebtorch-0.9.8/ebtorch/nn/fieldtransform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-12 03:22:40.455836 ebtorch-0.9.8/ebtorch/nn/functional/
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-08-12 03:22:30.000000 ebtorch-0.9.8/ebtorch/nn/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-08-12 03:22:30.000000 ebtorch-0.9.8/ebtorch/nn/functional/inner_functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     8870 2023-08-12 03:22:30.000000 ebtorch-0.9.8/ebtorch/nn/kwta.py
--rw-r--r--   0 runner    (1001) docker     (123)    13650 2023-08-12 03:22:30.000000 ebtorch-0.9.8/ebtorch/nn/laplacenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-08-12 03:22:30.000000 ebtorch-0.9.8/ebtorch/nn/mish.py
--rw-r--r--   0 runner    (1001) docker     (123)     9902 2023-08-12 03:22:30.000000 ebtorch-0.9.8/ebtorch/nn/nnsemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-08-12 03:22:30.000000 ebtorch-0.9.8/ebtorch/nn/reshapelayers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-08-12 03:22:30.000000 ebtorch-0.9.8/ebtorch/nn/serf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-08-12 03:22:30.000000 ebtorch-0.9.8/ebtorch/nn/serlu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-08-12 03:22:30.000000 ebtorch-0.9.8/ebtorch/nn/sinlu.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-08-12 03:22:30.000000 ebtorch-0.9.8/ebtorch/nn/smelu.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-12 03:22:40.459837 ebtorch-0.9.8/ebtorch/nn/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-08-12 03:22:30.000000 ebtorch-0.9.8/ebtorch/nn/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-08-12 03:22:30.000000 ebtorch-0.9.8/ebtorch/nn/utils/adverutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-08-12 03:22:30.000000 ebtorch-0.9.8/ebtorch/nn/utils/autoclip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-08-12 03:22:30.000000 ebtorch-0.9.8/ebtorch/nn/utils/onlyutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-08-12 03:22:30.000000 ebtorch-0.9.8/ebtorch/nn/utils/patches.py
--rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-08-12 03:22:30.000000 ebtorch-0.9.8/ebtorch/nn/utils/reprutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-12 03:22:40.459837 ebtorch-0.9.8/ebtorch/optim/
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-08-12 03:22:30.000000 ebtorch-0.9.8/ebtorch/optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-08-12 03:22:30.000000 ebtorch-0.9.8/ebtorch/optim/adabound.py
--rw-r--r--   0 runner    (1001) docker     (123)     8821 2023-08-12 03:22:30.000000 ebtorch-0.9.8/ebtorch/optim/adahessian.py
--rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-08-12 03:22:30.000000 ebtorch-0.9.8/ebtorch/optim/adan.py
--rw-r--r--   0 runner    (1001) docker     (123)    20036 2023-08-12 03:22:30.000000 ebtorch-0.9.8/ebtorch/optim/autowu.py
--rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-08-12 03:22:30.000000 ebtorch-0.9.8/ebtorch/optim/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-08-12 03:22:30.000000 ebtorch-0.9.8/ebtorch/optim/lion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-08-12 03:22:30.000000 ebtorch-0.9.8/ebtorch/optim/lookahead.py
--rw-r--r--   0 runner    (1001) docker     (123)     7221 2023-08-12 03:22:30.000000 ebtorch-0.9.8/ebtorch/optim/lookaround.py
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-08-12 03:22:30.000000 ebtorch-0.9.8/ebtorch/optim/radam.py
--rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-08-12 03:22:30.000000 ebtorch-0.9.8/ebtorch/optim/sam.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-12 03:22:40.451836 ebtorch-0.9.8/ebtorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-08-12 03:22:40.000000 ebtorch-0.9.8/ebtorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-08-12 03:22:40.000000 ebtorch-0.9.8/ebtorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-12 03:22:40.000000 ebtorch-0.9.8/ebtorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-12 03:22:40.000000 ebtorch-0.9.8/ebtorch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-12 03:22:40.000000 ebtorch-0.9.8/ebtorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-12 03:22:40.463837 ebtorch-0.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-08-12 03:22:30.000000 ebtorch-0.9.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-12 03:30:44.217166 ebtorch-0.9.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-08-12 03:30:34.000000 ebtorch-0.9.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-08-12 03:30:44.217166 ebtorch-0.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-08-12 03:30:34.000000 ebtorch-0.9.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-12 03:30:44.209166 ebtorch-0.9.9/ebtorch/
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-08-12 03:30:34.000000 ebtorch-0.9.9/ebtorch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-12 03:30:44.213166 ebtorch-0.9.9/ebtorch/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-08-12 03:30:34.000000 ebtorch-0.9.9/ebtorch/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16875 2023-08-12 03:30:34.000000 ebtorch-0.9.9/ebtorch/data/cutmixup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8055 2023-08-12 03:30:34.000000 ebtorch-0.9.9/ebtorch/data/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-12 03:30:44.213166 ebtorch-0.9.9/ebtorch/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-08-12 03:30:34.000000 ebtorch-0.9.9/ebtorch/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-08-12 03:30:34.000000 ebtorch-0.9.9/ebtorch/logging/avgmeter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-08-12 03:30:34.000000 ebtorch-0.9.9/ebtorch/logging/logcsv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-12 03:30:44.213166 ebtorch-0.9.9/ebtorch/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-08-12 03:30:34.000000 ebtorch-0.9.9/ebtorch/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13998 2023-08-12 03:30:34.000000 ebtorch-0.9.9/ebtorch/nn/architectures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14741 2023-08-12 03:30:34.000000 ebtorch-0.9.9/ebtorch/nn/architectures_resnets_dm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7411 2023-08-12 03:30:34.000000 ebtorch-0.9.9/ebtorch/nn/conv2drp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-08-12 03:30:34.000000 ebtorch-0.9.9/ebtorch/nn/convolutional_flatten.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13699 2023-08-12 03:30:34.000000 ebtorch-0.9.9/ebtorch/nn/coordconv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-08-12 03:30:34.000000 ebtorch-0.9.9/ebtorch/nn/debuglayers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-08-12 03:30:34.000000 ebtorch-0.9.9/ebtorch/nn/fieldtransform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-12 03:30:44.213166 ebtorch-0.9.9/ebtorch/nn/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-08-12 03:30:34.000000 ebtorch-0.9.9/ebtorch/nn/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-08-12 03:30:34.000000 ebtorch-0.9.9/ebtorch/nn/functional/inner_functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8870 2023-08-12 03:30:34.000000 ebtorch-0.9.9/ebtorch/nn/kwta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13650 2023-08-12 03:30:34.000000 ebtorch-0.9.9/ebtorch/nn/laplacenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-08-12 03:30:34.000000 ebtorch-0.9.9/ebtorch/nn/mish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9902 2023-08-12 03:30:34.000000 ebtorch-0.9.9/ebtorch/nn/nnsemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-08-12 03:30:34.000000 ebtorch-0.9.9/ebtorch/nn/reshapelayers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-08-12 03:30:34.000000 ebtorch-0.9.9/ebtorch/nn/serf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-08-12 03:30:34.000000 ebtorch-0.9.9/ebtorch/nn/serlu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-08-12 03:30:34.000000 ebtorch-0.9.9/ebtorch/nn/sinlu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-08-12 03:30:34.000000 ebtorch-0.9.9/ebtorch/nn/smelu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-12 03:30:44.213166 ebtorch-0.9.9/ebtorch/nn/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-08-12 03:30:34.000000 ebtorch-0.9.9/ebtorch/nn/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-08-12 03:30:34.000000 ebtorch-0.9.9/ebtorch/nn/utils/adverutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-08-12 03:30:34.000000 ebtorch-0.9.9/ebtorch/nn/utils/autoclip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-08-12 03:30:34.000000 ebtorch-0.9.9/ebtorch/nn/utils/onlyutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-08-12 03:30:34.000000 ebtorch-0.9.9/ebtorch/nn/utils/patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-08-12 03:30:34.000000 ebtorch-0.9.9/ebtorch/nn/utils/reprutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-12 03:30:44.217166 ebtorch-0.9.9/ebtorch/optim/
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-08-12 03:30:34.000000 ebtorch-0.9.9/ebtorch/optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-08-12 03:30:34.000000 ebtorch-0.9.9/ebtorch/optim/adabound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8821 2023-08-12 03:30:34.000000 ebtorch-0.9.9/ebtorch/optim/adahessian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-08-12 03:30:34.000000 ebtorch-0.9.9/ebtorch/optim/adan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20036 2023-08-12 03:30:34.000000 ebtorch-0.9.9/ebtorch/optim/autowu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-08-12 03:30:34.000000 ebtorch-0.9.9/ebtorch/optim/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-08-12 03:30:34.000000 ebtorch-0.9.9/ebtorch/optim/lion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-08-12 03:30:34.000000 ebtorch-0.9.9/ebtorch/optim/lookahead.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7221 2023-08-12 03:30:34.000000 ebtorch-0.9.9/ebtorch/optim/lookaround.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-08-12 03:30:34.000000 ebtorch-0.9.9/ebtorch/optim/radam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-08-12 03:30:34.000000 ebtorch-0.9.9/ebtorch/optim/sam.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-12 03:30:44.209166 ebtorch-0.9.9/ebtorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-08-12 03:30:44.000000 ebtorch-0.9.9/ebtorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-08-12 03:30:44.000000 ebtorch-0.9.9/ebtorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-12 03:30:44.000000 ebtorch-0.9.9/ebtorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-12 03:30:44.000000 ebtorch-0.9.9/ebtorch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-12 03:30:44.000000 ebtorch-0.9.9/ebtorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-12 03:30:44.217166 ebtorch-0.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-08-12 03:30:34.000000 ebtorch-0.9.9/setup.py
```

### Comparing `ebtorch-0.9.8/LICENSE` & `ebtorch-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.8/PKG-INFO` & `ebtorch-0.9.9/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebtorch
-Version: 0.9.8
+Version: 0.9.9
 Summary: Collection of PyTorch additions, extensions, utilities, uses and abuses
 Home-page: https://github.com/emaballarin/ebtorch
 Author: Emanuele Ballarin
 Author-email: emanuele@ballarin.cc
 License: Apache-2.0
 Keywords: Deep Learning,Machine Learning
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ebtorch Version: 0.9.8 Summary: Collection of
+Metadata-Version: 2.1 Name: ebtorch Version: 0.9.9 Summary: Collection of
 PyTorch additions, extensions, utilities, uses and abuses Home-page: https://
 github.com/emaballarin/ebtorch Author: Emanuele Ballarin Author-email:
 emanuele@ballarin.cc License: Apache-2.0 Keywords: Deep Learning,Machine
 Learning Classifier: Development Status :: 4 - Beta Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: Environment ::
 Console Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: Apache Software License Requires-Python: >=3.8 Description-
```

### Comparing `ebtorch-0.9.8/ebtorch/__init__.py` & `ebtorch-0.9.9/ebtorch/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,14 +64,16 @@
 del ScaledERF
 del SERLU
 del SGRUHCell
 del SinLU
 del SmeLU
 del SolvePoisson
 del SolvePoissonTensor
+del WideResNet
+del PreActResNet
 del beta_reco_bce
 del field_transform
 del mishlayer_init
 del patch_rp_train_network
 del pixelwise_bce_mean
 del pixelwise_bce_sum
```

### Comparing `ebtorch-0.9.8/ebtorch/data/__init__.py` & `ebtorch-0.9.9/ebtorch/data/__init__.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.8/ebtorch/data/cutmixup.py` & `ebtorch-0.9.9/ebtorch/data/cutmixup.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.8/ebtorch/data/datasets.py` & `ebtorch-0.9.9/ebtorch/data/datasets.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.8/ebtorch/logging/__init__.py` & `ebtorch-0.9.9/ebtorch/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.8/ebtorch/logging/avgmeter.py` & `ebtorch-0.9.9/ebtorch/logging/avgmeter.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.8/ebtorch/logging/logcsv.py` & `ebtorch-0.9.9/ebtorch/logging/logcsv.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.8/ebtorch/nn/__init__.py` & `ebtorch-0.9.9/ebtorch/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.8/ebtorch/nn/architectures.py` & `ebtorch-0.9.9/ebtorch/nn/architectures.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.8/ebtorch/nn/architectures_resnets_dm.py` & `ebtorch-0.9.9/ebtorch/nn/architectures_resnets_dm.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.8/ebtorch/nn/conv2drp.py` & `ebtorch-0.9.9/ebtorch/nn/conv2drp.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.8/ebtorch/nn/convolutional_flatten.py` & `ebtorch-0.9.9/ebtorch/nn/convolutional_flatten.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.8/ebtorch/nn/coordconv.py` & `ebtorch-0.9.9/ebtorch/nn/coordconv.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.8/ebtorch/nn/debuglayers.py` & `ebtorch-0.9.9/ebtorch/nn/debuglayers.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.8/ebtorch/nn/fieldtransform.py` & `ebtorch-0.9.9/ebtorch/nn/fieldtransform.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.8/ebtorch/nn/functional/__init__.py` & `ebtorch-0.9.9/ebtorch/nn/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.8/ebtorch/nn/functional/inner_functional.py` & `ebtorch-0.9.9/ebtorch/nn/functional/inner_functional.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.8/ebtorch/nn/kwta.py` & `ebtorch-0.9.9/ebtorch/nn/kwta.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.8/ebtorch/nn/laplacenet.py` & `ebtorch-0.9.9/ebtorch/nn/laplacenet.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.8/ebtorch/nn/mish.py` & `ebtorch-0.9.9/ebtorch/nn/mish.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.8/ebtorch/nn/nnsemble.py` & `ebtorch-0.9.9/ebtorch/nn/nnsemble.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.8/ebtorch/nn/reshapelayers.py` & `ebtorch-0.9.9/ebtorch/nn/reshapelayers.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.8/ebtorch/nn/serf.py` & `ebtorch-0.9.9/ebtorch/nn/serf.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.8/ebtorch/nn/serlu.py` & `ebtorch-0.9.9/ebtorch/nn/serlu.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.8/ebtorch/nn/sinlu.py` & `ebtorch-0.9.9/ebtorch/nn/sinlu.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.8/ebtorch/nn/smelu.py` & `ebtorch-0.9.9/ebtorch/nn/smelu.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.8/ebtorch/nn/utils/__init__.py` & `ebtorch-0.9.9/ebtorch/nn/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.8/ebtorch/nn/utils/adverutils.py` & `ebtorch-0.9.9/ebtorch/nn/utils/adverutils.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.8/ebtorch/nn/utils/autoclip.py` & `ebtorch-0.9.9/ebtorch/nn/utils/autoclip.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.8/ebtorch/nn/utils/onlyutils.py` & `ebtorch-0.9.9/ebtorch/nn/utils/onlyutils.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.8/ebtorch/nn/utils/patches.py` & `ebtorch-0.9.9/ebtorch/nn/utils/patches.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.8/ebtorch/nn/utils/reprutils.py` & `ebtorch-0.9.9/ebtorch/nn/utils/reprutils.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.8/ebtorch/optim/__init__.py` & `ebtorch-0.9.9/ebtorch/optim/__init__.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.8/ebtorch/optim/adabound.py` & `ebtorch-0.9.9/ebtorch/optim/adabound.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.8/ebtorch/optim/adahessian.py` & `ebtorch-0.9.9/ebtorch/optim/adahessian.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.8/ebtorch/optim/adan.py` & `ebtorch-0.9.9/ebtorch/optim/adan.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.8/ebtorch/optim/autowu.py` & `ebtorch-0.9.9/ebtorch/optim/autowu.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.8/ebtorch/optim/custom.py` & `ebtorch-0.9.9/ebtorch/optim/custom.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.8/ebtorch/optim/lion.py` & `ebtorch-0.9.9/ebtorch/optim/lion.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.8/ebtorch/optim/lookahead.py` & `ebtorch-0.9.9/ebtorch/optim/lookahead.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.8/ebtorch/optim/lookaround.py` & `ebtorch-0.9.9/ebtorch/optim/lookaround.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.8/ebtorch/optim/radam.py` & `ebtorch-0.9.9/ebtorch/optim/radam.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.8/ebtorch/optim/sam.py` & `ebtorch-0.9.9/ebtorch/optim/sam.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.8/ebtorch.egg-info/PKG-INFO` & `ebtorch-0.9.9/ebtorch.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebtorch
-Version: 0.9.8
+Version: 0.9.9
 Summary: Collection of PyTorch additions, extensions, utilities, uses and abuses
 Home-page: https://github.com/emaballarin/ebtorch
 Author: Emanuele Ballarin
 Author-email: emanuele@ballarin.cc
 License: Apache-2.0
 Keywords: Deep Learning,Machine Learning
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ebtorch Version: 0.9.8 Summary: Collection of
+Metadata-Version: 2.1 Name: ebtorch Version: 0.9.9 Summary: Collection of
 PyTorch additions, extensions, utilities, uses and abuses Home-page: https://
 github.com/emaballarin/ebtorch Author: Emanuele Ballarin Author-email:
 emanuele@ballarin.cc License: Apache-2.0 Keywords: Deep Learning,Machine
 Learning Classifier: Development Status :: 4 - Beta Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: Environment ::
 Console Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: Apache Software License Requires-Python: >=3.8 Description-
```

### Comparing `ebtorch-0.9.8/ebtorch.egg-info/SOURCES.txt` & `ebtorch-0.9.9/ebtorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.8/setup.py` & `ebtorch-0.9.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 check_dependencies(DEPENDENCY_PACKAGE_NAMES)
 
 PACKAGENAME: str = "ebtorch"
 
 
 setup(
     name=PACKAGENAME,
-    version="0.9.8",
+    version="0.9.9",
     author="Emanuele Ballarin",
     author_email="emanuele@ballarin.cc",
     url="https://github.com/emaballarin/ebtorch",
     description="Collection of PyTorch additions, extensions, utilities, uses and abuses",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     keywords=["Deep Learning", "Machine Learning"],
```

