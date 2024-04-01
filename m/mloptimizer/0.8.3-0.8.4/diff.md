# Comparing `tmp/mloptimizer-0.8.3.tar.gz` & `tmp/mloptimizer-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mloptimizer-0.8.3.tar", last modified: Sun Mar 31 23:26:48 2024, max compression
+gzip compressed data, was "mloptimizer-0.8.4.tar", last modified: Mon Apr  1 22:30:06 2024, max compression
```

## Comparing `mloptimizer-0.8.3.tar` & `mloptimizer-0.8.4.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 23:26:48.651300 mloptimizer-0.8.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-03-31 23:26:45.000000 mloptimizer-0.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-31 23:26:45.000000 mloptimizer-0.8.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10775 2024-03-31 23:26:48.651300 mloptimizer-0.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7481 2024-03-31 23:26:45.000000 mloptimizer-0.8.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 23:26:48.639299 mloptimizer-0.8.3/mloptimizer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 23:26:45.000000 mloptimizer-0.8.3/mloptimizer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 23:26:48.639299 mloptimizer-0.8.3/mloptimizer/aux/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-31 23:26:45.000000 mloptimizer-0.8.3/mloptimizer/aux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9420 2024-03-31 23:26:45.000000 mloptimizer-0.8.3/mloptimizer/aux/alg_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     5154 2024-03-31 23:26:45.000000 mloptimizer-0.8.3/mloptimizer/aux/plots.py
--rw-r--r--   0 runner    (1001) docker     (127)     7228 2024-03-31 23:26:45.000000 mloptimizer-0.8.3/mloptimizer/aux/tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-03-31 23:26:45.000000 mloptimizer-0.8.3/mloptimizer/aux/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 23:26:48.639299 mloptimizer-0.8.3/mloptimizer/conf/
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-03-31 23:26:45.000000 mloptimizer-0.8.3/mloptimizer/conf/CatBoostClassifier_default_HyperparamSpace.json
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-03-31 23:26:45.000000 mloptimizer-0.8.3/mloptimizer/conf/CustomXGBClassifier_default_HyperparamSpace.json
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-03-31 23:26:45.000000 mloptimizer-0.8.3/mloptimizer/conf/DecisionTreeClassifier_default_HyperparamSpace.json
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-03-31 23:26:45.000000 mloptimizer-0.8.3/mloptimizer/conf/ExtraTreesClassifier_default_HyperparamSpace.json
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-03-31 23:26:45.000000 mloptimizer-0.8.3/mloptimizer/conf/GradientBoostingClassifier_default_HyperparamSpace.json
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-03-31 23:26:45.000000 mloptimizer-0.8.3/mloptimizer/conf/RandomForestClassifier_default_HyperparamSpace.json
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-03-31 23:26:45.000000 mloptimizer-0.8.3/mloptimizer/conf/SVC_default_HyperparamSpace.json
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-03-31 23:26:45.000000 mloptimizer-0.8.3/mloptimizer/conf/XGBClassifier_default_HyperparamSpace.json
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-03-31 23:26:45.000000 mloptimizer-0.8.3/mloptimizer/conf/default_hyperparameter_spaces.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 23:26:48.643299 mloptimizer-0.8.3/mloptimizer/core/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-31 23:26:45.000000 mloptimizer-0.8.3/mloptimizer/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8190 2024-03-31 23:26:45.000000 mloptimizer-0.8.3/mloptimizer/core/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-03-31 23:26:45.000000 mloptimizer-0.8.3/mloptimizer/core/keras.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 23:26:48.643299 mloptimizer-0.8.3/mloptimizer/evaluation/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-03-31 23:26:45.000000 mloptimizer-0.8.3/mloptimizer/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-03-31 23:26:45.000000 mloptimizer-0.8.3/mloptimizer/evaluation/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)    11198 2024-03-31 23:26:45.000000 mloptimizer-0.8.3/mloptimizer/evaluation/model_evaluation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 23:26:48.643299 mloptimizer-0.8.3/mloptimizer/genetic/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-31 23:26:45.000000 mloptimizer-0.8.3/mloptimizer/genetic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-03-31 23:26:45.000000 mloptimizer-0.8.3/mloptimizer/genetic/deapoptimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    12819 2024-03-31 23:26:45.000000 mloptimizer-0.8.3/mloptimizer/genetic/garunner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-03-31 23:26:45.000000 mloptimizer-0.8.3/mloptimizer/genetic/individual.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 23:26:48.643299 mloptimizer-0.8.3/mloptimizer/hyperparams/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-31 23:26:45.000000 mloptimizer-0.8.3/mloptimizer/hyperparams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-03-31 23:26:45.000000 mloptimizer-0.8.3/mloptimizer/hyperparams/hyperparam.py
--rw-r--r--   0 runner    (1001) docker     (127)     6010 2024-03-31 23:26:45.000000 mloptimizer-0.8.3/mloptimizer/hyperparams/hyperspace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 23:26:48.643299 mloptimizer-0.8.3/mloptimizer/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 23:26:45.000000 mloptimizer-0.8.3/mloptimizer/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 23:26:48.643299 mloptimizer-0.8.3/mloptimizer/test/test_aux/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 23:26:45.000000 mloptimizer-0.8.3/mloptimizer/test/test_aux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-03-31 23:26:45.000000 mloptimizer-0.8.3/mloptimizer/test/test_aux/test_CustomXGBClassifier.py
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-03-31 23:26:45.000000 mloptimizer-0.8.3/mloptimizer/test/test_aux/test_alg_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-03-31 23:26:45.000000 mloptimizer-0.8.3/mloptimizer/test/test_aux/test_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-03-31 23:26:45.000000 mloptimizer-0.8.3/mloptimizer/test/test_aux/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 23:26:48.643299 mloptimizer-0.8.3/mloptimizer/test/test_evaluation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 23:26:45.000000 mloptimizer-0.8.3/mloptimizer/test/test_evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-03-31 23:26:45.000000 mloptimizer-0.8.3/mloptimizer/test/test_evaluation/test_model_evaluation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 23:26:48.643299 mloptimizer-0.8.3/mloptimizer/test/test_genoptimizer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 23:26:45.000000 mloptimizer-0.8.3/mloptimizer/test/test_genoptimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7404 2024-03-31 23:26:45.000000 mloptimizer-0.8.3/mloptimizer/test/test_genoptimizer/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 23:26:48.647300 mloptimizer-0.8.3/mloptimizer/test/test_hyperparams/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 23:26:45.000000 mloptimizer-0.8.3/mloptimizer/test/test_hyperparams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-03-31 23:26:45.000000 mloptimizer-0.8.3/mloptimizer/test/test_hyperparams/test_hyperparam.py
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-03-31 23:26:45.000000 mloptimizer-0.8.3/mloptimizer/test/test_hyperparams/test_hyperspace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 23:26:48.647300 mloptimizer-0.8.3/mloptimizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10775 2024-03-31 23:26:48.000000 mloptimizer-0.8.3/mloptimizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-03-31 23:26:48.000000 mloptimizer-0.8.3/mloptimizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 23:26:48.000000 mloptimizer-0.8.3/mloptimizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-03-31 23:26:48.000000 mloptimizer-0.8.3/mloptimizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-31 23:26:48.000000 mloptimizer-0.8.3/mloptimizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-03-31 23:26:45.000000 mloptimizer-0.8.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 23:26:48.651300 mloptimizer-0.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     7692 2024-03-31 23:26:45.000000 mloptimizer-0.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:30:06.734282 mloptimizer-0.8.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10784 2024-04-01 22:30:06.734282 mloptimizer-0.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7490 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:30:06.718282 mloptimizer-0.8.4/mloptimizer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:30:06.722282 mloptimizer-0.8.4/mloptimizer/aux/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/aux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9420 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/aux/alg_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5154 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/aux/plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7228 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/aux/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/aux/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:30:06.722282 mloptimizer-0.8.4/mloptimizer/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/conf/CatBoostClassifier_default_HyperparamSpace.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/conf/CustomXGBClassifier_default_HyperparamSpace.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/conf/DecisionTreeClassifier_default_HyperparamSpace.json
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/conf/ExtraTreesClassifier_default_HyperparamSpace.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/conf/GradientBoostingClassifier_default_HyperparamSpace.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/conf/RandomForestClassifier_default_HyperparamSpace.json
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/conf/SVC_default_HyperparamSpace.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/conf/XGBClassifier_default_HyperparamSpace.json
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/conf/default_hyperparameter_spaces.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:30:06.722282 mloptimizer-0.8.4/mloptimizer/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8190 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/core/keras.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:30:06.726282 mloptimizer-0.8.4/mloptimizer/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/evaluation/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11198 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/evaluation/model_evaluation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:30:06.726282 mloptimizer-0.8.4/mloptimizer/genetic/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/genetic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/genetic/deapoptimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12819 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/genetic/garunner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/genetic/individual.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:30:06.726282 mloptimizer-0.8.4/mloptimizer/hyperparams/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/hyperparams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/hyperparams/hyperparam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6010 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/hyperparams/hyperspace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:30:06.726282 mloptimizer-0.8.4/mloptimizer/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:30:06.726282 mloptimizer-0.8.4/mloptimizer/test/test_aux/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/test/test_aux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/test/test_aux/test_CustomXGBClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/test/test_aux/test_alg_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/test/test_aux/test_plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/test/test_aux/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:30:06.726282 mloptimizer-0.8.4/mloptimizer/test/test_evaluation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/test/test_evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/test/test_evaluation/test_model_evaluation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:30:06.726282 mloptimizer-0.8.4/mloptimizer/test/test_genoptimizer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/test/test_genoptimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7404 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/test/test_genoptimizer/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:30:06.726282 mloptimizer-0.8.4/mloptimizer/test/test_hyperparams/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/test/test_hyperparams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/test/test_hyperparams/test_hyperparam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/mloptimizer/test/test_hyperparams/test_hyperspace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:30:06.726282 mloptimizer-0.8.4/mloptimizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10784 2024-04-01 22:30:06.000000 mloptimizer-0.8.4/mloptimizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-01 22:30:06.000000 mloptimizer-0.8.4/mloptimizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 22:30:06.000000 mloptimizer-0.8.4/mloptimizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-01 22:30:06.000000 mloptimizer-0.8.4/mloptimizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-01 22:30:06.000000 mloptimizer-0.8.4/mloptimizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 22:30:06.734282 mloptimizer-0.8.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     7692 2024-04-01 22:30:03.000000 mloptimizer-0.8.4/setup.py
```

### Comparing `mloptimizer-0.8.3/LICENSE` & `mloptimizer-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.8.3/PKG-INFO` & `mloptimizer-0.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mloptimizer
-Version: 0.8.3
+Version: 0.8.4
 Summary: mloptimizer is a Python library for optimizing hyperparameters of machine learning algorithms using genetic algorithms.
 Home-page: https://github.com/Caparrini/mloptimizer
 Author: Antonio Caparrini López, Javier Arroyo Gallardo
 Author-email: acaparri@ucm.es
 Project-URL: Source, https://github.com/Caparrini/mloptimizer
 Keywords: xgboost,genetic,deap
 Classifier: Development Status :: 3 - Alpha
@@ -140,19 +140,19 @@
 # 1) Load the dataset and get the features and target
 X, y = load_iris(return_X_y=True)
 
 # 2) Define the hyperparameter space (a default space is provided for some algorithms)
 hyperparameter_space = HyperparameterSpace.get_default_hyperparameter_space(DecisionTreeClassifier)
 
 # 3) Create the optimizer and optimize the classifier
-opt = Optimizer(model_class=DecisionTreeClassifier, features=X, labels=y, hyperparam_space=hyperparameter_space)
+opt = Optimizer(estimator_class=DecisionTreeClassifier, features=X, labels=y, hyperparam_space=hyperparameter_space)
 
 # 4) Optimize the classifier, the optimization returns the best estimator found in the optimization process
 # - 10 generations starting with a population of 10 individuals, other parameters are set to default
-clf = opt.optimize_clf(population=10, generations=10)
+clf = opt.optimize_clf(population_size=10, generations=10)
 ```
 Other algorithms can be used, such as `RandomForestClassifier` or `XGBClassifier` which have a 
 default hyperparameter space defined in the library.
 Even if the algorithm is not included in the default hyperparameter space, you can define your own hyperparameter space
 following the documentation.
 
 The optimization will create a directory in the current folder with a name like `YYYYMMDD_nnnnnnnnnn_SklearnOptimizer`.
```

### Comparing `mloptimizer-0.8.3/README.md` & `mloptimizer-0.8.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -62,19 +62,19 @@
 # 1) Load the dataset and get the features and target
 X, y = load_iris(return_X_y=True)
 
 # 2) Define the hyperparameter space (a default space is provided for some algorithms)
 hyperparameter_space = HyperparameterSpace.get_default_hyperparameter_space(DecisionTreeClassifier)
 
 # 3) Create the optimizer and optimize the classifier
-opt = Optimizer(model_class=DecisionTreeClassifier, features=X, labels=y, hyperparam_space=hyperparameter_space)
+opt = Optimizer(estimator_class=DecisionTreeClassifier, features=X, labels=y, hyperparam_space=hyperparameter_space)
 
 # 4) Optimize the classifier, the optimization returns the best estimator found in the optimization process
 # - 10 generations starting with a population of 10 individuals, other parameters are set to default
-clf = opt.optimize_clf(population=10, generations=10)
+clf = opt.optimize_clf(population_size=10, generations=10)
 ```
 Other algorithms can be used, such as `RandomForestClassifier` or `XGBClassifier` which have a 
 default hyperparameter space defined in the library.
 Even if the algorithm is not included in the default hyperparameter space, you can define your own hyperparameter space
 following the documentation.
 
 The optimization will create a directory in the current folder with a name like `YYYYMMDD_nnnnnnnnnn_SklearnOptimizer`.
```

### Comparing `mloptimizer-0.8.3/mloptimizer/aux/alg_wrapper.py` & `mloptimizer-0.8.4/mloptimizer/aux/alg_wrapper.py`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.8.3/mloptimizer/aux/plots.py` & `mloptimizer-0.8.4/mloptimizer/aux/plots.py`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.8.3/mloptimizer/aux/tracker.py` & `mloptimizer-0.8.4/mloptimizer/aux/tracker.py`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.8.3/mloptimizer/aux/utils.py` & `mloptimizer-0.8.4/mloptimizer/aux/utils.py`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.8.3/mloptimizer/conf/CatBoostClassifier_default_HyperparamSpace.json` & `mloptimizer-0.8.4/mloptimizer/conf/CatBoostClassifier_default_HyperparamSpace.json`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.8.3/mloptimizer/conf/CustomXGBClassifier_default_HyperparamSpace.json` & `mloptimizer-0.8.4/mloptimizer/conf/CustomXGBClassifier_default_HyperparamSpace.json`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.8.3/mloptimizer/conf/DecisionTreeClassifier_default_HyperparamSpace.json` & `mloptimizer-0.8.4/mloptimizer/conf/DecisionTreeClassifier_default_HyperparamSpace.json`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.8.3/mloptimizer/conf/ExtraTreesClassifier_default_HyperparamSpace.json` & `mloptimizer-0.8.4/mloptimizer/conf/ExtraTreesClassifier_default_HyperparamSpace.json`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.8.3/mloptimizer/conf/GradientBoostingClassifier_default_HyperparamSpace.json` & `mloptimizer-0.8.4/mloptimizer/conf/GradientBoostingClassifier_default_HyperparamSpace.json`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.8.3/mloptimizer/conf/RandomForestClassifier_default_HyperparamSpace.json` & `mloptimizer-0.8.4/mloptimizer/conf/RandomForestClassifier_default_HyperparamSpace.json`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.8.3/mloptimizer/conf/SVC_default_HyperparamSpace.json` & `mloptimizer-0.8.4/mloptimizer/conf/SVC_default_HyperparamSpace.json`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.8.3/mloptimizer/conf/XGBClassifier_default_HyperparamSpace.json` & `mloptimizer-0.8.4/mloptimizer/conf/XGBClassifier_default_HyperparamSpace.json`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.8.3/mloptimizer/conf/default_hyperparameter_spaces.json` & `mloptimizer-0.8.4/mloptimizer/conf/default_hyperparameter_spaces.json`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.8.3/mloptimizer/core/base.py` & `mloptimizer-0.8.4/mloptimizer/core/base.py`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.8.3/mloptimizer/core/keras.py` & `mloptimizer-0.8.4/mloptimizer/core/keras.py`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.8.3/mloptimizer/evaluation/evaluator.py` & `mloptimizer-0.8.4/mloptimizer/evaluation/evaluator.py`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.8.3/mloptimizer/evaluation/model_evaluation.py` & `mloptimizer-0.8.4/mloptimizer/evaluation/model_evaluation.py`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.8.3/mloptimizer/genetic/deapoptimizer.py` & `mloptimizer-0.8.4/mloptimizer/genetic/deapoptimizer.py`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.8.3/mloptimizer/genetic/garunner.py` & `mloptimizer-0.8.4/mloptimizer/genetic/garunner.py`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.8.3/mloptimizer/genetic/individual.py` & `mloptimizer-0.8.4/mloptimizer/genetic/individual.py`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.8.3/mloptimizer/hyperparams/hyperparam.py` & `mloptimizer-0.8.4/mloptimizer/hyperparams/hyperparam.py`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.8.3/mloptimizer/hyperparams/hyperspace.py` & `mloptimizer-0.8.4/mloptimizer/hyperparams/hyperspace.py`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.8.3/mloptimizer/test/test_aux/test_CustomXGBClassifier.py` & `mloptimizer-0.8.4/mloptimizer/test/test_aux/test_CustomXGBClassifier.py`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.8.3/mloptimizer/test/test_aux/test_alg_wrapper.py` & `mloptimizer-0.8.4/mloptimizer/test/test_aux/test_alg_wrapper.py`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.8.3/mloptimizer/test/test_aux/test_plots.py` & `mloptimizer-0.8.4/mloptimizer/test/test_aux/test_plots.py`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.8.3/mloptimizer/test/test_aux/test_utils.py` & `mloptimizer-0.8.4/mloptimizer/test/test_aux/test_utils.py`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.8.3/mloptimizer/test/test_evaluation/test_model_evaluation.py` & `mloptimizer-0.8.4/mloptimizer/test/test_evaluation/test_model_evaluation.py`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.8.3/mloptimizer/test/test_genoptimizer/test_base.py` & `mloptimizer-0.8.4/mloptimizer/test/test_genoptimizer/test_base.py`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.8.3/mloptimizer/test/test_hyperparams/test_hyperparam.py` & `mloptimizer-0.8.4/mloptimizer/test/test_hyperparams/test_hyperparam.py`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.8.3/mloptimizer/test/test_hyperparams/test_hyperspace.py` & `mloptimizer-0.8.4/mloptimizer/test/test_hyperparams/test_hyperspace.py`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.8.3/mloptimizer.egg-info/PKG-INFO` & `mloptimizer-0.8.4/mloptimizer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mloptimizer
-Version: 0.8.3
+Version: 0.8.4
 Summary: mloptimizer is a Python library for optimizing hyperparameters of machine learning algorithms using genetic algorithms.
 Home-page: https://github.com/Caparrini/mloptimizer
 Author: Antonio Caparrini López, Javier Arroyo Gallardo
 Author-email: acaparri@ucm.es
 Project-URL: Source, https://github.com/Caparrini/mloptimizer
 Keywords: xgboost,genetic,deap
 Classifier: Development Status :: 3 - Alpha
@@ -140,19 +140,19 @@
 # 1) Load the dataset and get the features and target
 X, y = load_iris(return_X_y=True)
 
 # 2) Define the hyperparameter space (a default space is provided for some algorithms)
 hyperparameter_space = HyperparameterSpace.get_default_hyperparameter_space(DecisionTreeClassifier)
 
 # 3) Create the optimizer and optimize the classifier
-opt = Optimizer(model_class=DecisionTreeClassifier, features=X, labels=y, hyperparam_space=hyperparameter_space)
+opt = Optimizer(estimator_class=DecisionTreeClassifier, features=X, labels=y, hyperparam_space=hyperparameter_space)
 
 # 4) Optimize the classifier, the optimization returns the best estimator found in the optimization process
 # - 10 generations starting with a population of 10 individuals, other parameters are set to default
-clf = opt.optimize_clf(population=10, generations=10)
+clf = opt.optimize_clf(population_size=10, generations=10)
 ```
 Other algorithms can be used, such as `RandomForestClassifier` or `XGBClassifier` which have a 
 default hyperparameter space defined in the library.
 Even if the algorithm is not included in the default hyperparameter space, you can define your own hyperparameter space
 following the documentation.
 
 The optimization will create a directory in the current folder with a name like `YYYYMMDD_nnnnnnnnnn_SklearnOptimizer`.
```

### Comparing `mloptimizer-0.8.3/mloptimizer.egg-info/SOURCES.txt` & `mloptimizer-0.8.4/mloptimizer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.8.3/mloptimizer.egg-info/requires.txt` & `mloptimizer-0.8.4/mloptimizer.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `mloptimizer-0.8.3/setup.py` & `mloptimizer-0.8.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     name="mloptimizer",  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version="0.8.3",  # Required
+    version="0.8.4",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="mloptimizer is a Python library "
                 "for optimizing hyperparameters of machine learning algorithms using genetic algorithms.",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
```

