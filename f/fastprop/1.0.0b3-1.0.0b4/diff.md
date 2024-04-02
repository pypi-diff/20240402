# Comparing `tmp/fastprop-1.0.0b3.tar.gz` & `tmp/fastprop-1.0.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastprop-1.0.0b3.tar", last modified: Wed Feb 28 04:18:04 2024, max compression
+gzip compressed data, was "fastprop-1.0.0b4.tar", last modified: Tue Apr  2 19:02:04 2024, max compression
```

## Comparing `fastprop-1.0.0b3.tar` & `fastprop-1.0.0b4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 04:18:04.055125 fastprop-1.0.0b3/
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-02-28 04:17:56.000000 fastprop-1.0.0b3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12967 2024-02-28 04:18:04.055125 fastprop-1.0.0b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12094 2024-02-28 04:17:56.000000 fastprop-1.0.0b3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 04:18:04.051125 fastprop-1.0.0b3/fastprop/
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-02-28 04:17:56.000000 fastprop-1.0.0b3/fastprop/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 04:18:04.055125 fastprop-1.0.0b3/fastprop/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     7028 2024-02-28 04:17:56.000000 fastprop-1.0.0b3/fastprop/cli/fastprop_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-02-28 04:17:56.000000 fastprop-1.0.0b3/fastprop/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)    25010 2024-02-28 04:17:56.000000 fastprop-1.0.0b3/fastprop/fastprop_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     5250 2024-02-28 04:17:56.000000 fastprop-1.0.0b3/fastprop/hopt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-02-28 04:17:56.000000 fastprop-1.0.0b3/fastprop/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-02-28 04:17:56.000000 fastprop-1.0.0b3/fastprop/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-02-28 04:17:56.000000 fastprop-1.0.0b3/fastprop/shap.py
--rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-02-28 04:17:56.000000 fastprop-1.0.0b3/fastprop/train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 04:18:04.055125 fastprop-1.0.0b3/fastprop/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-02-28 04:17:56.000000 fastprop-1.0.0b3/fastprop/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4945 2024-02-28 04:17:56.000000 fastprop-1.0.0b3/fastprop/utils/calculate_descriptors.py
--rw-r--r--   0 runner    (1001) docker     (127)    37956 2024-02-28 04:17:56.000000 fastprop-1.0.0b3/fastprop/utils/descriptor_lists.py
--rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-02-28 04:17:56.000000 fastprop-1.0.0b3/fastprop/utils/load_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-02-28 04:17:56.000000 fastprop-1.0.0b3/fastprop/utils/select_descriptors.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-02-28 04:17:56.000000 fastprop-1.0.0b3/fastprop/utils/validate_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 04:18:04.055125 fastprop-1.0.0b3/fastprop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12967 2024-02-28 04:18:04.000000 fastprop-1.0.0b3/fastprop.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-02-28 04:18:04.000000 fastprop-1.0.0b3/fastprop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-28 04:18:04.000000 fastprop-1.0.0b3/fastprop.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-28 04:18:04.000000 fastprop-1.0.0b3/fastprop.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-02-28 04:18:04.000000 fastprop-1.0.0b3/fastprop.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-28 04:18:04.000000 fastprop-1.0.0b3/fastprop.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-02-28 04:17:56.000000 fastprop-1.0.0b3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-28 04:18:04.055125 fastprop-1.0.0b3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 04:18:04.055125 fastprop-1.0.0b3/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-02-28 04:17:56.000000 fastprop-1.0.0b3/test/test_fastprop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:02:04.236006 fastprop-1.0.0b4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-02 19:01:59.000000 fastprop-1.0.0b4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12912 2024-04-02 19:02:04.236006 fastprop-1.0.0b4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11996 2024-04-02 19:01:59.000000 fastprop-1.0.0b4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:02:04.232006 fastprop-1.0.0b4/fastprop/
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-02 19:01:59.000000 fastprop-1.0.0b4/fastprop/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:02:04.232006 fastprop-1.0.0b4/fastprop/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     7028 2024-04-02 19:01:59.000000 fastprop-1.0.0b4/fastprop/cli/fastprop_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-02 19:01:59.000000 fastprop-1.0.0b4/fastprop/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26470 2024-04-02 19:01:59.000000 fastprop-1.0.0b4/fastprop/fastprop_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5250 2024-04-02 19:01:59.000000 fastprop-1.0.0b4/fastprop/hopt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-04-02 19:01:59.000000 fastprop-1.0.0b4/fastprop/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-04-02 19:01:59.000000 fastprop-1.0.0b4/fastprop/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-04-02 19:01:59.000000 fastprop-1.0.0b4/fastprop/shap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-04-02 19:01:59.000000 fastprop-1.0.0b4/fastprop/train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:02:04.232006 fastprop-1.0.0b4/fastprop/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-02 19:01:59.000000 fastprop-1.0.0b4/fastprop/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5066 2024-04-02 19:01:59.000000 fastprop-1.0.0b4/fastprop/utils/calculate_descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37956 2024-04-02 19:01:59.000000 fastprop-1.0.0b4/fastprop/utils/descriptor_lists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-04-02 19:01:59.000000 fastprop-1.0.0b4/fastprop/utils/load_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-02 19:01:59.000000 fastprop-1.0.0b4/fastprop/utils/select_descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-02 19:01:59.000000 fastprop-1.0.0b4/fastprop/utils/validate_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:02:04.236006 fastprop-1.0.0b4/fastprop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12912 2024-04-02 19:02:04.000000 fastprop-1.0.0b4/fastprop.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-02 19:02:04.000000 fastprop-1.0.0b4/fastprop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 19:02:04.000000 fastprop-1.0.0b4/fastprop.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-02 19:02:04.000000 fastprop-1.0.0b4/fastprop.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-02 19:02:04.000000 fastprop-1.0.0b4/fastprop.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-02 19:02:04.000000 fastprop-1.0.0b4/fastprop.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-02 19:01:59.000000 fastprop-1.0.0b4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 19:02:04.236006 fastprop-1.0.0b4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:02:04.236006 fastprop-1.0.0b4/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-02 19:01:59.000000 fastprop-1.0.0b4/test/test_fastprop.py
```

### Comparing `fastprop-1.0.0b3/LICENSE` & `fastprop-1.0.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `fastprop-1.0.0b3/PKG-INFO` & `fastprop-1.0.0b4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastprop
-Version: 1.0.0b3
+Version: 1.0.0b4
 Summary: Fast Molecular Property Prediction with mordredcommunity
 Author: Jackson Burns
 License: MIT
 Project-URL: Homepage, https://github.com/JacksonBurns/fastprop
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -20,14 +20,15 @@
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Provides-Extra: hopt
 Requires-Dist: ray[train]; extra == "hopt"
 Requires-Dist: optuna; extra == "hopt"
 Provides-Extra: shap
 Requires-Dist: shap; extra == "shap"
+Requires-Dist: matplotlib; extra == "shap"
 Provides-Extra: bmark
 Requires-Dist: py2opsin; extra == "bmark"
 
 <p align="center">  
   <img alt="fastproplogo" height="400" src="https://raw.githubusercontent.com/JacksonBurns/fastprop/main/fastprop_logo.png">
 </p>
 <h2 align="center">Fast Molecular Property Prediction with <a href="https://github.com/JacksonBurns/mordred-community">mordredcommunity</a></h2>
@@ -47,16 +48,15 @@
 Check out the demo notebook for quick intro to `fastprop` via Google Colab - runs in your browser, GPU included, no install required!
 
 <a target="_blank" href="https://colab.research.google.com/github/JacksonBurns/fastprop/blob/main/fastprop_demo.ipynb">
   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
 </a>
 
 # Installing `fastprop`
-`fastprop` supports Mac, Windows, and Linux on Python versions 3.8 to 3.11 (except 3.11 on Windows).
-As dependencies gradually begin to support Python 3.12 it will be added.
+`fastprop` supports Mac, Windows, and Linux on Python versions 3.8 to 3.12.
 Installing from `pip` or `conda` is the best way to get `fastprop`, but if you need to check out a specific GitHub branch or you want to contribute to `fastprop` a source installation is recommended.
 
 ## `pip` [recommended]
 `fastprop` is available via PyPI with `pip install fastprop`.
 
 To make extending `fastprop` easier and keep the installation size down, dependencies required for hyperparameter optimization and SHAP analysis are _optional_.
 They can be installed with `pip install fastprop[hopt]`, `pip install fastprop[shap]`, or `pip install fastprop[shap,hopt]` to install them both.
```

#### html2text {}

```diff
@@ -1,59 +1,58 @@
-Metadata-Version: 2.1 Name: fastprop Version: 1.0.0b3 Summary: Fast Molecular
+Metadata-Version: 2.1 Name: fastprop Version: 1.0.0b4 Summary: Fast Molecular
 Property Prediction with mordredcommunity Author: Jackson Burns License: MIT
 Project-URL: Homepage, https://github.com/JacksonBurns/fastprop Classifier:
 Programming Language :: Python :: 3 Requires-Python: >=3.8 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: pyyaml Requires-Dist:
 lightning Requires-Dist: mordredcommunity Requires-Dist: astartes[molecules]
 Requires-Dist: tensorboard Requires-Dist: psutil Provides-Extra: dev Requires-
 Dist: black; extra == "dev" Requires-Dist: isort; extra == "dev" Requires-Dist:
 pytest; extra == "dev" Provides-Extra: hopt Requires-Dist: ray[train]; extra ==
 "hopt" Requires-Dist: optuna; extra == "hopt" Provides-Extra: shap Requires-
-Dist: shap; extra == "shap" Provides-Extra: bmark Requires-Dist: py2opsin;
-extra == "bmark"
+Dist: shap; extra == "shap" Requires-Dist: matplotlib; extra == "shap"
+Provides-Extra: bmark Requires-Dist: py2opsin; extra == "bmark"
                                 [fastproplogo]
      ********** FFaasstt MMoolleeccuullaarr PPrrooppeerrttyy PPrreeddiiccttiioonn wwiitthh _mm_oo_rr_dd_rr_ee_dd_cc_oo_mm_mm_uu_nn_ii_tt_yy **********
           [GitHub Repo Stars][PyPI - Downloads][PyPI][PyPI - License]
 # Announcement - Open Beta! `fastprop` is currently in the version 3 open beta
 (1.0.0b3)! Please try `fastprop` on your datasets and let us know what you
 think. Feature requests and bug reports are **very** appreciated! Check out the
 demo notebook for quick intro to `fastprop` via Google Colab - runs in your
 browser, GPU included, no install required! _[_O_p_e_n_ _I_n_ _C_o_l_a_b_]# Installing
 `fastprop` `fastprop` supports Mac, Windows, and Linux on Python versions 3.8
-to 3.11 (except 3.11 on Windows). As dependencies gradually begin to support
-Python 3.12 it will be added. Installing from `pip` or `conda` is the best way
-to get `fastprop`, but if you need to check out a specific GitHub branch or you
-want to contribute to `fastprop` a source installation is recommended. ## `pip`
-[recommended] `fastprop` is available via PyPI with `pip install fastprop`. To
-make extending `fastprop` easier and keep the installation size down,
-dependencies required for hyperparameter optimization and SHAP analysis are
-_optional_. They can be installed with `pip install fastprop[hopt]`, `pip
-install fastprop[shap]`, or `pip install fastprop[shap,hopt]` to install them
-both. If you want to use `fastprop` but not write new code on top of it, you
-may want to install these now - you can always do so later, however, and
-`fastprop` will remind you. ## `conda` - _coming soon!_ ~~`fastprop` is
-available from `conda-forge` with `conda install -c conda-forge fastprop`.~~ ##
-Source To install `fastprop` from GitHub directly you can: 1. Run `pip install
-https://github.com/JacksonBurns/fastprop.git@main` to install from the `main`
-branch (or specify any other branch you like) 2. Clone the repository with `git
-clone https://github.com/JacksonBurns/fastprop.git`, navigate to `fastprop`
-with `cd fastprop`, and run `pip install .` To contribute to `fastprop` please
-follow [this tutorial](https://opensource.com/article/19/7/create-pull-request-
-github) (or something similar) to set up a forked version of `fastprop` and
-open a pull request (similar to above option 2). All contributions are
-appreciated! See [Developing `fastprop`](#developing-fastprop) for more
-details. # About `fastprop` `fastprop` is a package for performing deep-QSPR
-(Quantitative Structure-Property Relationship) with minimal user intervention.
-By passing in a list of SMILES strings, `fastprop` will automatically generate
-and cache a set of molecular descriptors using [`mordredcommunity`](https://
-github.com/JacksonBurns/mordred-community) and train an FNN to predict the
-corresponding properties. See the `examples` and `benchmarks` directories to
-see how to run training - the rest of this documentation will focus on how you
-can run, configure, and customize `fastprop`. ## Paper An academic paper has
-been prepared which describes the `fastprop` approach and walks through the
+to 3.12. Installing from `pip` or `conda` is the best way to get `fastprop`,
+but if you need to check out a specific GitHub branch or you want to contribute
+to `fastprop` a source installation is recommended. ## `pip` [recommended]
+`fastprop` is available via PyPI with `pip install fastprop`. To make extending
+`fastprop` easier and keep the installation size down, dependencies required
+for hyperparameter optimization and SHAP analysis are _optional_. They can be
+installed with `pip install fastprop[hopt]`, `pip install fastprop[shap]`, or
+`pip install fastprop[shap,hopt]` to install them both. If you want to use
+`fastprop` but not write new code on top of it, you may want to install these
+now - you can always do so later, however, and `fastprop` will remind you. ##
+`conda` - _coming soon!_ ~~`fastprop` is available from `conda-forge` with
+`conda install -c conda-forge fastprop`.~~ ## Source To install `fastprop` from
+GitHub directly you can: 1. Run `pip install https://github.com/JacksonBurns/
+fastprop.git@main` to install from the `main` branch (or specify any other
+branch you like) 2. Clone the repository with `git clone https://github.com/
+JacksonBurns/fastprop.git`, navigate to `fastprop` with `cd fastprop`, and run
+`pip install .` To contribute to `fastprop` please follow [this tutorial]
+(https://opensource.com/article/19/7/create-pull-request-github) (or something
+similar) to set up a forked version of `fastprop` and open a pull request
+(similar to above option 2). All contributions are appreciated! See [Developing
+`fastprop`](#developing-fastprop) for more details. # About `fastprop`
+`fastprop` is a package for performing deep-QSPR (Quantitative Structure-
+Property Relationship) with minimal user intervention. By passing in a list of
+SMILES strings, `fastprop` will automatically generate and cache a set of
+molecular descriptors using [`mordredcommunity`](https://github.com/
+JacksonBurns/mordred-community) and train an FNN to predict the corresponding
+properties. See the `examples` and `benchmarks` directories to see how to run
+training - the rest of this documentation will focus on how you can run,
+configure, and customize `fastprop`. ## Paper An academic paper has been
+prepared which describes the `fastprop` approach and walks through the
 `benchmarks` in greater detail. See the `paper` directory for more information.
 ## `fastprop` Framework There are four distinct steps in `fastprop` that define
 its framework: 1. Featurization - transform the input molecules (as SMILES
 strings) into an array of molecular descriptors which are saved 2.
 Preprocessing - clean the descriptors by removing or imputing missing values
 then rescaling the remainder 3. Training - send the processed input to the
 neural network, which is a sample FNN (sequential fully-connected layers with
```

### Comparing `fastprop-1.0.0b3/README.md` & `fastprop-1.0.0b4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,15 @@
 Check out the demo notebook for quick intro to `fastprop` via Google Colab - runs in your browser, GPU included, no install required!
 
 <a target="_blank" href="https://colab.research.google.com/github/JacksonBurns/fastprop/blob/main/fastprop_demo.ipynb">
   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
 </a>
 
 # Installing `fastprop`
-`fastprop` supports Mac, Windows, and Linux on Python versions 3.8 to 3.11 (except 3.11 on Windows).
-As dependencies gradually begin to support Python 3.12 it will be added.
+`fastprop` supports Mac, Windows, and Linux on Python versions 3.8 to 3.12.
 Installing from `pip` or `conda` is the best way to get `fastprop`, but if you need to check out a specific GitHub branch or you want to contribute to `fastprop` a source installation is recommended.
 
 ## `pip` [recommended]
 `fastprop` is available via PyPI with `pip install fastprop`.
 
 To make extending `fastprop` easier and keep the installation size down, dependencies required for hyperparameter optimization and SHAP analysis are _optional_.
 They can be installed with `pip install fastprop[hopt]`, `pip install fastprop[shap]`, or `pip install fastprop[shap,hopt]` to install them both.
```

#### html2text {}

```diff
@@ -3,45 +3,44 @@
           [GitHub Repo Stars][PyPI - Downloads][PyPI][PyPI - License]
 # Announcement - Open Beta! `fastprop` is currently in the version 3 open beta
 (1.0.0b3)! Please try `fastprop` on your datasets and let us know what you
 think. Feature requests and bug reports are **very** appreciated! Check out the
 demo notebook for quick intro to `fastprop` via Google Colab - runs in your
 browser, GPU included, no install required! _[_O_p_e_n_ _I_n_ _C_o_l_a_b_]# Installing
 `fastprop` `fastprop` supports Mac, Windows, and Linux on Python versions 3.8
-to 3.11 (except 3.11 on Windows). As dependencies gradually begin to support
-Python 3.12 it will be added. Installing from `pip` or `conda` is the best way
-to get `fastprop`, but if you need to check out a specific GitHub branch or you
-want to contribute to `fastprop` a source installation is recommended. ## `pip`
-[recommended] `fastprop` is available via PyPI with `pip install fastprop`. To
-make extending `fastprop` easier and keep the installation size down,
-dependencies required for hyperparameter optimization and SHAP analysis are
-_optional_. They can be installed with `pip install fastprop[hopt]`, `pip
-install fastprop[shap]`, or `pip install fastprop[shap,hopt]` to install them
-both. If you want to use `fastprop` but not write new code on top of it, you
-may want to install these now - you can always do so later, however, and
-`fastprop` will remind you. ## `conda` - _coming soon!_ ~~`fastprop` is
-available from `conda-forge` with `conda install -c conda-forge fastprop`.~~ ##
-Source To install `fastprop` from GitHub directly you can: 1. Run `pip install
-https://github.com/JacksonBurns/fastprop.git@main` to install from the `main`
-branch (or specify any other branch you like) 2. Clone the repository with `git
-clone https://github.com/JacksonBurns/fastprop.git`, navigate to `fastprop`
-with `cd fastprop`, and run `pip install .` To contribute to `fastprop` please
-follow [this tutorial](https://opensource.com/article/19/7/create-pull-request-
-github) (or something similar) to set up a forked version of `fastprop` and
-open a pull request (similar to above option 2). All contributions are
-appreciated! See [Developing `fastprop`](#developing-fastprop) for more
-details. # About `fastprop` `fastprop` is a package for performing deep-QSPR
-(Quantitative Structure-Property Relationship) with minimal user intervention.
-By passing in a list of SMILES strings, `fastprop` will automatically generate
-and cache a set of molecular descriptors using [`mordredcommunity`](https://
-github.com/JacksonBurns/mordred-community) and train an FNN to predict the
-corresponding properties. See the `examples` and `benchmarks` directories to
-see how to run training - the rest of this documentation will focus on how you
-can run, configure, and customize `fastprop`. ## Paper An academic paper has
-been prepared which describes the `fastprop` approach and walks through the
+to 3.12. Installing from `pip` or `conda` is the best way to get `fastprop`,
+but if you need to check out a specific GitHub branch or you want to contribute
+to `fastprop` a source installation is recommended. ## `pip` [recommended]
+`fastprop` is available via PyPI with `pip install fastprop`. To make extending
+`fastprop` easier and keep the installation size down, dependencies required
+for hyperparameter optimization and SHAP analysis are _optional_. They can be
+installed with `pip install fastprop[hopt]`, `pip install fastprop[shap]`, or
+`pip install fastprop[shap,hopt]` to install them both. If you want to use
+`fastprop` but not write new code on top of it, you may want to install these
+now - you can always do so later, however, and `fastprop` will remind you. ##
+`conda` - _coming soon!_ ~~`fastprop` is available from `conda-forge` with
+`conda install -c conda-forge fastprop`.~~ ## Source To install `fastprop` from
+GitHub directly you can: 1. Run `pip install https://github.com/JacksonBurns/
+fastprop.git@main` to install from the `main` branch (or specify any other
+branch you like) 2. Clone the repository with `git clone https://github.com/
+JacksonBurns/fastprop.git`, navigate to `fastprop` with `cd fastprop`, and run
+`pip install .` To contribute to `fastprop` please follow [this tutorial]
+(https://opensource.com/article/19/7/create-pull-request-github) (or something
+similar) to set up a forked version of `fastprop` and open a pull request
+(similar to above option 2). All contributions are appreciated! See [Developing
+`fastprop`](#developing-fastprop) for more details. # About `fastprop`
+`fastprop` is a package for performing deep-QSPR (Quantitative Structure-
+Property Relationship) with minimal user intervention. By passing in a list of
+SMILES strings, `fastprop` will automatically generate and cache a set of
+molecular descriptors using [`mordredcommunity`](https://github.com/
+JacksonBurns/mordred-community) and train an FNN to predict the corresponding
+properties. See the `examples` and `benchmarks` directories to see how to run
+training - the rest of this documentation will focus on how you can run,
+configure, and customize `fastprop`. ## Paper An academic paper has been
+prepared which describes the `fastprop` approach and walks through the
 `benchmarks` in greater detail. See the `paper` directory for more information.
 ## `fastprop` Framework There are four distinct steps in `fastprop` that define
 its framework: 1. Featurization - transform the input molecules (as SMILES
 strings) into an array of molecular descriptors which are saved 2.
 Preprocessing - clean the descriptors by removing or imputing missing values
 then rescaling the remainder 3. Training - send the processed input to the
 neural network, which is a sample FNN (sequential fully-connected layers with
```

### Comparing `fastprop-1.0.0b3/fastprop/cli/fastprop_cli.py` & `fastprop-1.0.0b4/fastprop/cli/fastprop_cli.py`

 * *Files identical despite different names*

### Comparing `fastprop-1.0.0b3/fastprop/defaults.py` & `fastprop-1.0.0b4/fastprop/defaults.py`

 * *Files identical despite different names*

### Comparing `fastprop-1.0.0b3/fastprop/fastprop_core.py` & `fastprop-1.0.0b4/fastprop/fastprop_core.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 from pytorch_lightning.callbacks.early_stopping import EarlyStopping
 from pytorch_lightning.loggers import TensorBoardLogger
 from scipy.stats import ttest_ind
 from sklearn.impute import SimpleImputer
 from sklearn.metrics import mean_absolute_percentage_error as mape
 from sklearn.metrics import mean_squared_error as l2_error
 from sklearn.preprocessing import OneHotEncoder, StandardScaler
+from torch import distributed
 from torch.utils.data import Dataset as TorchDataset
 from torchmetrics.functional.classification import (
     auroc,
     binary_accuracy,
     f1_score,
     multiclass_accuracy,
     multiclass_auroc,
@@ -60,14 +61,20 @@
     """Basic PyTorch dataset class.
 
     Args:
         TorchDataset (pytorch.Dataset): PyTorch's dataset class.
     """
 
     def __init__(self, data, targets):
+        """Initialize a basic torch-compatible data
+
+        Args:
+            data (torch.tensor): features
+            targets (torch.tensor): targets
+        """
         self.data = data
         self.length = len(targets)
         self.targets = targets
 
     def __len__(self):
         return self.length
 
@@ -102,32 +109,32 @@
         sampler,
         smiles,
         verbose=True,
     ):
         """Core fastprop model.
 
         Args:
-            feature_scaler (sklearn scaler): Scaler used on feature variables, used for reporting metrics in human-scale.
-            target_scaler (sklearn scaler): Scaler used on target variables, used for reporting metrics in human-scale.
             num_epochs (int): Maximum allowed number of training epochs.
+            input_size (int): Number of input neurons.
             hidden_size (int): Number of neurons in the hidden layers.
-            learning_rate (float): Learning rate.
+            readout_size (int): Number of targets to readout.
+            learning_rate (float): Learning rate for Adam.
             fnn_layers (int): Number of layers in the FNN.
             problem_type (str): Problem type, i.e. regression, multiclass, multilabel, or binary.
-            verbose (bool, optional): Reduces some logging if true. Defaults to False.
-            num_classes (int, optional): Number of classes for multiclass classification. Defaults to None.
-            cleaned_data (numpy.ndarray or torch.Tensor): Descriptors, already subjected to preprocessing (dropping operations)
-            targets (numpy.ndarray or torch.Tensor): Scaled targets in the same order as the descriptors.
-            batch_size (int): Samples/per batch - for small feature sets like in fastprop, set as high as possible.
-            random_seed (int): Seed for RNG.
-            train_size (float): Fraction of data for training.
-            val_size (float): Fraction of data for validation.
-            test_size (float): Fraction of data for test.
-            sampler (str): Type of sampler to use, see astartes for a list of implemented samplers.
-            smiles (list[str], optional): SMILES strings corresponding to the molecules for use in some samplers. Defaults to None.
+            cleaned_data (numpy.ndarray): Descriptors with no missing values.
+            targets (numpy.ndarray): Scaled targets in the same order as the descriptors.
+            target_names (sequence): Sequence of names for the targets.
+            batch_size (int): Number of molecules per training batch in SGD.
+            random_seed (int): Seed for splitting.
+            train_size (float): Fraction of data for training, nonzero.
+            val_size (float): Fraction of data for validation, nonzero.
+            test_size (float): Fraction of data for test, nonzero.
+            sampler (string): Sampling approach passed to astartes, i.e. random, scaffold
+            smiles (sequence): Sequence of SMILES strings corresponding to the features.
+            verbose (bool, optional): Print extra information. Defaults to True.
         """
         super().__init__()
         # used for data preparation and training
         self.random_seed = random_seed
         self.problem_type = problem_type
         self.num_classes = readout_size if self.problem_type == "multiclass" else None
 
@@ -162,14 +169,15 @@
         self.target_names = target_names
 
         # add derived attributes to the hparams attribute manually so that they are saved with checkpoints
         self.hparams["num_classes"] = self.num_classes
         self.save_hyperparameters(ignore=("cleaned_data", "targets", "smiles"))
 
     def _split(self):
+        """Sets self.*_idxs for training, validation, and test"""
         logger.info(f"Sampling dataset with {self.sampler} sampler.")
         split_kwargs = dict(
             train_size=self.train_size,
             val_size=self.val_size,
             test_size=self.test_size,
             sampler=self.sampler,
             random_state=self.random_seed,
@@ -192,14 +200,15 @@
                 *_,
                 self.train_idxs,
                 self.val_idxs,
                 self.test_idxs,
             ) = train_val_test_split_molecules(self.smiles, **split_kwargs)
 
     def setup(self, stage=None):
+        """Split and rescale the data."""
         if stage == "fit":
             self._split()
             logger.info("Imputing and rescaling input features.")
             # it is possible that the randomly chosen training set can have all entries missing a descriptor
             # even if other members of the dataset are valued! They will be zeroed out
             self.mean_imputer = SimpleImputer(missing_values=np.nan, strategy="mean", keep_empty_features=True)
             self.mean_imputer.fit(self.data[self.train_idxs, :])
@@ -223,14 +232,23 @@
                 self.targets = self.target_scaler.fit_transform(self.targets)
 
             # finally, cast everything as needed
             self.data = torch.tensor(self.data, dtype=torch.float32)
             self.targets = torch.tensor(self.targets, dtype=torch.float32)
 
     def _init_dataloader(self, shuffle, idxs):
+        """Helper method to initialize dataloaders.
+
+        Args:
+            shuffle (bool): Passed to torch's DataLoader
+            idxs (np.array): Indexes of overall dataset to include in dataloader.
+
+        Returns:
+            torch.utils.data.Dataloader: Dataloader instance.
+        """
         return torch.utils.data.DataLoader(
             ArbitraryDataset(
                 [self.data[i] for i in idxs],
                 [self.targets[i] for i in idxs],
             ),
             batch_size=self.batch_size,
             shuffle=shuffle,
@@ -244,14 +262,25 @@
     def val_dataloader(self):
         return self._init_dataloader(False, self.val_idxs)
 
     def test_dataloader(self):
         return self._init_dataloader(False, self.test_idxs)
 
     def get_metrics(problem_type):
+        """Get the metrics for training and early stopping based on the problem type.
+
+        Args:
+            problem_type (str): Regression, multilabel, multiclass, or binary.
+
+        Raises:
+            RuntimeError: Unsupported problem types
+
+        Returns:
+            str: names for the two metrics
+        """
         if problem_type == "regression":
             return "mse", "rmse"
         elif problem_type == "multilabel":
             return "bce", "auroc"
         elif problem_type == "multiclass":
             return "kldiv", "auroc"
         elif problem_type == "binary":
@@ -260,14 +289,21 @@
             raise RuntimeError(f"Unsupported problem type '{problem_type}'!")
 
     def forward(self, x):
         x = self.fnn.forward(x)
         x = self.readout(x)
         return x
 
+    def log(self, name, value, **kwargs):
+        if in_distributed := distributed.is_initialized():
+            if not isinstance(value, torch.Tensor):
+                value = torch.tensor(value)
+            value = value.to(self.device)
+        return super().log(name, value, sync_dist=in_distributed, **kwargs)
+
     def configure_optimizers(self):
         optimizer = torch.optim.Adam(self.parameters(), lr=self.learning_rate)
         return {"optimizer": optimizer}
 
     def training_step(self, batch, batch_idx):
         loss = self._machine_loss(batch, reduction="mean")
         self.log(f"train_{self.training_metric}_loss", loss)
@@ -282,27 +318,29 @@
     def test_step(self, batch, batch_idx):
         loss, _, y, y_hat = self._machine_loss(batch, return_all=True)
         self.log(f"test_{self.training_metric}_loss", loss)
         self._human_loss(y_hat.detach().cpu(), y.detach().cpu(), "test")
         return loss
 
     def predict_step(self, X):
+        # calls forward, but applies the appropriate transforms and activations
         X = self.mean_imputer.transform(X)
         X = self.feature_scaler.transform(X)
         X = torch.tensor(X, dtype=torch.float32, device=self.device)
         with torch.inference_mode():
             logits = self.forward(X)
         if self.problem_type == "regression":
             return self.target_scaler.inverse_transform(logits.detach().cpu())
         elif self.problem_type in {"multilabel", "binary"}:
             return torch.sigmoid(logits).detach().cpu()
         elif self.problem_type == "multiclass":
             return torch.nn.functional.softmax(logits, dim=1).detach().cpu()
 
     def _machine_loss(self, batch, reduction="mean", return_all=False):
+        # reports the rescaled loss directly on the logits for computational efficiency
         x, y = batch
         y_hat = self.forward(x)
         if self.problem_type == "regression":
             loss = torch.nn.functional.mse_loss(y_hat, y, reduction=reduction)
         elif self.problem_type in {"multilabel", "binary"}:
             loss = torch.nn.functional.binary_cross_entropy_with_logits(y_hat, y, reduction=reduction)
         else:
@@ -399,16 +437,15 @@
     no_logs=False,
     enable_checkpoints=True,
 ):
     """Run the lightning trainer loop on a given model.
 
     Args:
         outdir (str): Output directory for log files.
-        datamodule (ArbitraryDataModule): Lightning-style datamodule.
-        model (LightingModule): fastprop model architecture itself.
+        lightning_module (LightingModule): fastprop model architecture itself.
         patience (int, optional): Maximum number of epochs to wait before stopping early. Defaults to 5.
         verbose (bool, optional): Set to false for less output. Defaults to True.
         no_logs (bool, optional): Set to true to disable logs. Defaults to False.
         enable_checkpoints (bool, optional): Set to false to disable checkpoint writing. Defaults to True.
 
     Returns:
         list[dict{metric: score}]: Output of lightning model.test and model.validate
@@ -490,29 +527,37 @@
     random_seed,
     hopt=False,
 ):
     """Outer training loop to perform repeats.
 
     Args:
         number_repeats (int): Number of repetitions.
-        number_features (int): Number of features in the input layer.
-        target_scaler (sklearn scaler): Scaler used on target variables, used for reporting metrics in human-scale.
         number_epochs (int): Maximum allowed number of training epochs.
+        input_size (int): Number of input neurons.
         hidden_size (int): Number of neurons in the hidden layers.
-        learning_rate (float): Learning rate.
+        readout_size (int): Number of targets to readout.
+        learning_rate (float): Learning rate for Adam.
         fnn_layers (int): Number of layers in the FNN.
+        output_directory (str): Destination directory for file output.
+        patience (int, optional): Maximum number of epochs to wait before stopping early. Defaults to 5.
         problem_type (str): Problem type, i.e. regression, multiclass, multilabel, or binary.
-        num_classes (int, optional): Number of classes for multiclass classification. Defaults to None.
-        output_directory (str): Output directory for log files.
-        datamodule (pl.DataModule): Basic data module.
-        patience (int): Maximum number of epochs to wait before stopping training early.
-        hopt (bool, optional): Set to true when running hyperparameter optimization to turn off logs, logging, etc. Defaults to False.
+        train_size (float): Fraction of data for training, nonzero.
+        val_size (float): Fraction of data for validation, nonzero.
+        test_size (float): Fraction of data for test, nonzero.
+        sampler (string): Sampling approach passed to astartes, i.e. random, scaffold
+        smiles (sequence): Sequence of SMILES strings corresponding to the features.
+        cleaned_data (numpy.ndarray): Descriptors with no missing values.
+        targets (numpy.ndarray): Scaled targets in the same order as the descriptors.
+        target_names (sequence): Sequence of names for the targets.
+        batch_size (int): Number of molecules per training batch in SGD.
+        random_seed (int): Seed for splitting.
+        hopt (bool, optional): Disables checkpointing and printing when True. Defaults to False.
 
     Returns:
-        list[dict{metric: score}]: Output of lightning model.test and model.validate, one pair per repetition.
+        _type_: _description_
     """
     if not hopt:
         logger.info(f"Run 'tensorboard --logdir {os.path.join(output_directory, 'tensorboard_logs')}' to track training progress.")
     # hopt disables some printing from fastprop, as well as the training loop, disables logging, and disables writing checkpoints
     all_test_results, all_validation_results = [], []
     for i in range(number_repeats):
         # reinitialize model
```

### Comparing `fastprop-1.0.0b3/fastprop/hopt.py` & `fastprop-1.0.0b4/fastprop/hopt.py`

 * *Files identical despite different names*

### Comparing `fastprop-1.0.0b3/fastprop/predict.py` & `fastprop-1.0.0b4/fastprop/predict.py`

 * *Files identical despite different names*

### Comparing `fastprop-1.0.0b3/fastprop/preprocessing.py` & `fastprop-1.0.0b4/fastprop/preprocessing.py`

 * *Files identical despite different names*

### Comparing `fastprop-1.0.0b3/fastprop/shap.py` & `fastprop-1.0.0b4/fastprop/shap.py`

 * *Files identical despite different names*

### Comparing `fastprop-1.0.0b3/fastprop/train.py` & `fastprop-1.0.0b4/fastprop/train.py`

 * *Files identical despite different names*

### Comparing `fastprop-1.0.0b3/fastprop/utils/__init__.py` & `fastprop-1.0.0b4/fastprop/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `fastprop-1.0.0b3/fastprop/utils/calculate_descriptors.py` & `fastprop-1.0.0b4/fastprop/utils/calculate_descriptors.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,21 +23,21 @@
 # the parallelism slower but more memory efficient. We do this manually:
 def _f(in_tuple):
     mordred_calc = Calculator(in_tuple[2], ignore_3D=in_tuple[3])
     mordred_descs = np.array(list(mordred_calc.map(in_tuple[0], nproc=1, quiet=in_tuple[1])))
     return mordred_descs
 
 
-def calculate_mordred_desciptors(descriptors, rdkit_mols, n_procs, strategy: Literal["fast", "low-memory"] = "fast", ignore_3d=True):
+def calculate_mordred_desciptors(descriptors, rdkit_mols, n_procs: int = 2, strategy: Literal["fast", "low-memory"] = "fast", ignore_3d=True):
     """Wraps the mordred descriptor calculator.
 
     Args:
         descriptors (Mordred descriptor instances): Descriptors to calculate
         rdkit_mols (list[rdkit mols]): List of RDKit molecules.
-        n_procs (int): Number of parallel processes.
+        n_procs (int): Number of parallel processes. Defaults to 2.
         strategy (Literal["fast", "low-memory", optional): Parallelization strategy. Defaults to "fast".
         ignore_3d (bool, optional): Include 3D descriptors, if in given list. Defaults to True.
 
     Raises:
         RuntimeError: Invalid choice of parallel strategy.
 
     Returns:
@@ -76,14 +76,15 @@
     Args:
         precomputed (str): Use precomputed descriptors if str is.
         input_file (str): Filepath of input data.
         output_directory (str): Destination directory for caching.
         descriptors (list): fastprop set of descriptors to calculate.
         enable_cache (bool): Allow/disallow caching mechanism.
         mols (list): RDKit molecules.
+        as_df (bool): Set to true to return the result as a pandas DataFrame. Defaults to False.
     """
     descs = None
     if precomputed:
         del mols
         logger.info(f"Loading precomputed descriptors from {precomputed}.")
         descs = load_saved_desc(precomputed)
     else:
```

### Comparing `fastprop-1.0.0b3/fastprop/utils/descriptor_lists.py` & `fastprop-1.0.0b4/fastprop/utils/descriptor_lists.py`

 * *Files identical despite different names*

### Comparing `fastprop-1.0.0b3/fastprop/utils/load_data.py` & `fastprop-1.0.0b4/fastprop/utils/load_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,11 +48,12 @@
         targets = np.delete(targets, error_target_idxs, axis=0)
         rdkit_mols = np.delete(rdkit_mols, error_target_idxs, axis=0)
         smiles = np.delete(smiles, error_target_idxs)
     return targets, rdkit_mols, smiles
 
 
 def load_saved_desc(fpath):
+    # loads descriptors previously saved by fastprop, forces any non-numeric values (missing, strings, etc) to be nan.
     d = pd.read_csv(fpath, low_memory=False)
     d = d.apply(pd.to_numeric, errors="coerce")
     descs = d[d.columns[1:]].to_numpy(dtype=float)
     return descs
```

### Comparing `fastprop-1.0.0b3/fastprop/utils/select_descriptors.py` & `fastprop-1.0.0b4/fastprop/utils/select_descriptors.py`

 * *Files identical despite different names*

### Comparing `fastprop-1.0.0b3/fastprop.egg-info/PKG-INFO` & `fastprop-1.0.0b4/fastprop.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastprop
-Version: 1.0.0b3
+Version: 1.0.0b4
 Summary: Fast Molecular Property Prediction with mordredcommunity
 Author: Jackson Burns
 License: MIT
 Project-URL: Homepage, https://github.com/JacksonBurns/fastprop
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -20,14 +20,15 @@
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Provides-Extra: hopt
 Requires-Dist: ray[train]; extra == "hopt"
 Requires-Dist: optuna; extra == "hopt"
 Provides-Extra: shap
 Requires-Dist: shap; extra == "shap"
+Requires-Dist: matplotlib; extra == "shap"
 Provides-Extra: bmark
 Requires-Dist: py2opsin; extra == "bmark"
 
 <p align="center">  
   <img alt="fastproplogo" height="400" src="https://raw.githubusercontent.com/JacksonBurns/fastprop/main/fastprop_logo.png">
 </p>
 <h2 align="center">Fast Molecular Property Prediction with <a href="https://github.com/JacksonBurns/mordred-community">mordredcommunity</a></h2>
@@ -47,16 +48,15 @@
 Check out the demo notebook for quick intro to `fastprop` via Google Colab - runs in your browser, GPU included, no install required!
 
 <a target="_blank" href="https://colab.research.google.com/github/JacksonBurns/fastprop/blob/main/fastprop_demo.ipynb">
   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
 </a>
 
 # Installing `fastprop`
-`fastprop` supports Mac, Windows, and Linux on Python versions 3.8 to 3.11 (except 3.11 on Windows).
-As dependencies gradually begin to support Python 3.12 it will be added.
+`fastprop` supports Mac, Windows, and Linux on Python versions 3.8 to 3.12.
 Installing from `pip` or `conda` is the best way to get `fastprop`, but if you need to check out a specific GitHub branch or you want to contribute to `fastprop` a source installation is recommended.
 
 ## `pip` [recommended]
 `fastprop` is available via PyPI with `pip install fastprop`.
 
 To make extending `fastprop` easier and keep the installation size down, dependencies required for hyperparameter optimization and SHAP analysis are _optional_.
 They can be installed with `pip install fastprop[hopt]`, `pip install fastprop[shap]`, or `pip install fastprop[shap,hopt]` to install them both.
```

#### html2text {}

```diff
@@ -1,59 +1,58 @@
-Metadata-Version: 2.1 Name: fastprop Version: 1.0.0b3 Summary: Fast Molecular
+Metadata-Version: 2.1 Name: fastprop Version: 1.0.0b4 Summary: Fast Molecular
 Property Prediction with mordredcommunity Author: Jackson Burns License: MIT
 Project-URL: Homepage, https://github.com/JacksonBurns/fastprop Classifier:
 Programming Language :: Python :: 3 Requires-Python: >=3.8 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: pyyaml Requires-Dist:
 lightning Requires-Dist: mordredcommunity Requires-Dist: astartes[molecules]
 Requires-Dist: tensorboard Requires-Dist: psutil Provides-Extra: dev Requires-
 Dist: black; extra == "dev" Requires-Dist: isort; extra == "dev" Requires-Dist:
 pytest; extra == "dev" Provides-Extra: hopt Requires-Dist: ray[train]; extra ==
 "hopt" Requires-Dist: optuna; extra == "hopt" Provides-Extra: shap Requires-
-Dist: shap; extra == "shap" Provides-Extra: bmark Requires-Dist: py2opsin;
-extra == "bmark"
+Dist: shap; extra == "shap" Requires-Dist: matplotlib; extra == "shap"
+Provides-Extra: bmark Requires-Dist: py2opsin; extra == "bmark"
                                 [fastproplogo]
      ********** FFaasstt MMoolleeccuullaarr PPrrooppeerrttyy PPrreeddiiccttiioonn wwiitthh _mm_oo_rr_dd_rr_ee_dd_cc_oo_mm_mm_uu_nn_ii_tt_yy **********
           [GitHub Repo Stars][PyPI - Downloads][PyPI][PyPI - License]
 # Announcement - Open Beta! `fastprop` is currently in the version 3 open beta
 (1.0.0b3)! Please try `fastprop` on your datasets and let us know what you
 think. Feature requests and bug reports are **very** appreciated! Check out the
 demo notebook for quick intro to `fastprop` via Google Colab - runs in your
 browser, GPU included, no install required! _[_O_p_e_n_ _I_n_ _C_o_l_a_b_]# Installing
 `fastprop` `fastprop` supports Mac, Windows, and Linux on Python versions 3.8
-to 3.11 (except 3.11 on Windows). As dependencies gradually begin to support
-Python 3.12 it will be added. Installing from `pip` or `conda` is the best way
-to get `fastprop`, but if you need to check out a specific GitHub branch or you
-want to contribute to `fastprop` a source installation is recommended. ## `pip`
-[recommended] `fastprop` is available via PyPI with `pip install fastprop`. To
-make extending `fastprop` easier and keep the installation size down,
-dependencies required for hyperparameter optimization and SHAP analysis are
-_optional_. They can be installed with `pip install fastprop[hopt]`, `pip
-install fastprop[shap]`, or `pip install fastprop[shap,hopt]` to install them
-both. If you want to use `fastprop` but not write new code on top of it, you
-may want to install these now - you can always do so later, however, and
-`fastprop` will remind you. ## `conda` - _coming soon!_ ~~`fastprop` is
-available from `conda-forge` with `conda install -c conda-forge fastprop`.~~ ##
-Source To install `fastprop` from GitHub directly you can: 1. Run `pip install
-https://github.com/JacksonBurns/fastprop.git@main` to install from the `main`
-branch (or specify any other branch you like) 2. Clone the repository with `git
-clone https://github.com/JacksonBurns/fastprop.git`, navigate to `fastprop`
-with `cd fastprop`, and run `pip install .` To contribute to `fastprop` please
-follow [this tutorial](https://opensource.com/article/19/7/create-pull-request-
-github) (or something similar) to set up a forked version of `fastprop` and
-open a pull request (similar to above option 2). All contributions are
-appreciated! See [Developing `fastprop`](#developing-fastprop) for more
-details. # About `fastprop` `fastprop` is a package for performing deep-QSPR
-(Quantitative Structure-Property Relationship) with minimal user intervention.
-By passing in a list of SMILES strings, `fastprop` will automatically generate
-and cache a set of molecular descriptors using [`mordredcommunity`](https://
-github.com/JacksonBurns/mordred-community) and train an FNN to predict the
-corresponding properties. See the `examples` and `benchmarks` directories to
-see how to run training - the rest of this documentation will focus on how you
-can run, configure, and customize `fastprop`. ## Paper An academic paper has
-been prepared which describes the `fastprop` approach and walks through the
+to 3.12. Installing from `pip` or `conda` is the best way to get `fastprop`,
+but if you need to check out a specific GitHub branch or you want to contribute
+to `fastprop` a source installation is recommended. ## `pip` [recommended]
+`fastprop` is available via PyPI with `pip install fastprop`. To make extending
+`fastprop` easier and keep the installation size down, dependencies required
+for hyperparameter optimization and SHAP analysis are _optional_. They can be
+installed with `pip install fastprop[hopt]`, `pip install fastprop[shap]`, or
+`pip install fastprop[shap,hopt]` to install them both. If you want to use
+`fastprop` but not write new code on top of it, you may want to install these
+now - you can always do so later, however, and `fastprop` will remind you. ##
+`conda` - _coming soon!_ ~~`fastprop` is available from `conda-forge` with
+`conda install -c conda-forge fastprop`.~~ ## Source To install `fastprop` from
+GitHub directly you can: 1. Run `pip install https://github.com/JacksonBurns/
+fastprop.git@main` to install from the `main` branch (or specify any other
+branch you like) 2. Clone the repository with `git clone https://github.com/
+JacksonBurns/fastprop.git`, navigate to `fastprop` with `cd fastprop`, and run
+`pip install .` To contribute to `fastprop` please follow [this tutorial]
+(https://opensource.com/article/19/7/create-pull-request-github) (or something
+similar) to set up a forked version of `fastprop` and open a pull request
+(similar to above option 2). All contributions are appreciated! See [Developing
+`fastprop`](#developing-fastprop) for more details. # About `fastprop`
+`fastprop` is a package for performing deep-QSPR (Quantitative Structure-
+Property Relationship) with minimal user intervention. By passing in a list of
+SMILES strings, `fastprop` will automatically generate and cache a set of
+molecular descriptors using [`mordredcommunity`](https://github.com/
+JacksonBurns/mordred-community) and train an FNN to predict the corresponding
+properties. See the `examples` and `benchmarks` directories to see how to run
+training - the rest of this documentation will focus on how you can run,
+configure, and customize `fastprop`. ## Paper An academic paper has been
+prepared which describes the `fastprop` approach and walks through the
 `benchmarks` in greater detail. See the `paper` directory for more information.
 ## `fastprop` Framework There are four distinct steps in `fastprop` that define
 its framework: 1. Featurization - transform the input molecules (as SMILES
 strings) into an array of molecular descriptors which are saved 2.
 Preprocessing - clean the descriptors by removing or imputing missing values
 then rescaling the remainder 3. Training - send the processed input to the
 neural network, which is a sample FNN (sequential fully-connected layers with
```

### Comparing `fastprop-1.0.0b3/fastprop.egg-info/SOURCES.txt` & `fastprop-1.0.0b4/fastprop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastprop-1.0.0b3/pyproject.toml` & `fastprop-1.0.0b4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=64"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fastprop"
-version = "1.0.0b3"
+version = "1.0.0b4"
 authors = [
     { name = "Jackson Burns" },
 ]
 license = { text = "MIT" }
 description = "Fast Molecular Property Prediction with mordredcommunity"
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -16,15 +16,15 @@
 urls = { Homepage = "https://github.com/JacksonBurns/fastprop" }
 requires-python = ">=3.8"
 dependencies = ["pyyaml", "lightning", "mordredcommunity", "astartes[molecules]", "tensorboard", "psutil"]
 
 [project.optional-dependencies]
 dev = ["black", "isort", "pytest"]
 hopt = ["ray[train]", "optuna"]
-shap = ["shap"]
+shap = ["shap", "matplotlib"]
 bmark = ["py2opsin"]
 
 [project.readme]
 file = "README.md"
 content-type = "text/markdown"
 
 [project.scripts]
```

### Comparing `fastprop-1.0.0b3/test/test_fastprop.py` & `fastprop-1.0.0b4/test/test_fastprop.py`

 * *Files identical despite different names*

