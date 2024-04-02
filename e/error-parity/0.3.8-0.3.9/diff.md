# Comparing `tmp/error-parity-0.3.8.tar.gz` & `tmp/error-parity-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "error-parity-0.3.8.tar", last modified: Fri Nov 17 16:34:52 2023, max compression
+gzip compressed data, was "error-parity-0.3.9.tar", last modified: Wed Mar 20 16:32:34 2024, max compression
```

## Comparing `error-parity-0.3.8.tar` & `error-parity-0.3.9.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 16:34:52.259232 error-parity-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2023-11-17 16:34:40.000000 error-parity-0.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-11-17 16:34:40.000000 error-parity-0.3.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5463 2023-11-17 16:34:52.259232 error-parity-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3548 2023-11-17 16:34:40.000000 error-parity-0.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 16:34:52.255232 error-parity-0.3.8/error_parity/
--rwxr-xr-x   0 runner    (1001) docker     (127)      330 2023-11-17 16:34:40.000000 error-parity-0.3.8/error_parity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2023-11-17 16:34:40.000000 error-parity-0.3.8/error_parity/_commons.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2023-11-17 16:34:40.000000 error-parity-0.3.8/error_parity/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     7089 2023-11-17 16:34:40.000000 error-parity-0.3.8/error_parity/binarize.py
--rw-r--r--   0 runner    (1001) docker     (127)    17869 2023-11-17 16:34:40.000000 error-parity-0.3.8/error_parity/classifiers.py
--rw-r--r--   0 runner    (1001) docker     (127)    14390 2023-11-17 16:34:40.000000 error-parity-0.3.8/error_parity/cvxpy_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12217 2023-11-17 16:34:40.000000 error-parity-0.3.8/error_parity/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)    16234 2023-11-17 16:34:40.000000 error-parity-0.3.8/error_parity/pareto_curve.py
--rw-r--r--   0 runner    (1001) docker     (127)    10619 2023-11-17 16:34:40.000000 error-parity-0.3.8/error_parity/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     5202 2023-11-17 16:34:40.000000 error-parity-0.3.8/error_parity/roc_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14890 2023-11-17 16:34:40.000000 error-parity-0.3.8/error_parity/threshold_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 16:34:52.255232 error-parity-0.3.8/error_parity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5463 2023-11-17 16:34:52.000000 error-parity-0.3.8/error_parity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      693 2023-11-17 16:34:52.000000 error-parity-0.3.8/error_parity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-17 16:34:52.000000 error-parity-0.3.8/error_parity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      253 2023-11-17 16:34:52.000000 error-parity-0.3.8/error_parity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-11-17 16:34:52.000000 error-parity-0.3.8/error_parity.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 16:34:52.259232 error-parity-0.3.8/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2023-11-17 16:34:40.000000 error-parity-0.3.8/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2023-11-17 16:34:40.000000 error-parity-0.3.8/requirements/main.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-11-17 16:34:40.000000 error-parity-0.3.8/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-17 16:34:52.259232 error-parity-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3493 2023-11-17 16:34:40.000000 error-parity-0.3.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 16:34:52.259232 error-parity-0.3.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-17 16:34:40.000000 error-parity-0.3.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3098 2023-11-17 16:34:40.000000 error-parity-0.3.8/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2023-11-17 16:34:40.000000 error-parity-0.3.8/tests/test_cvxpy_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6438 2023-11-17 16:34:40.000000 error-parity-0.3.8/tests/test_equal_odds.py
--rw-r--r--   0 runner    (1001) docker     (127)      900 2023-11-17 16:34:40.000000 error-parity-0.3.8/tests/test_evaluation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 16:32:34.915878 error-parity-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-20 16:32:30.000000 error-parity-0.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-20 16:32:30.000000 error-parity-0.3.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5976 2024-03-20 16:32:34.915878 error-parity-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-03-20 16:32:30.000000 error-parity-0.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 16:32:34.911878 error-parity-0.3.9/error_parity/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      330 2024-03-20 16:32:30.000000 error-parity-0.3.9/error_parity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-03-20 16:32:30.000000 error-parity-0.3.9/error_parity/_commons.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-20 16:32:30.000000 error-parity-0.3.9/error_parity/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7089 2024-03-20 16:32:30.000000 error-parity-0.3.9/error_parity/binarize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17869 2024-03-20 16:32:30.000000 error-parity-0.3.9/error_parity/classifiers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15976 2024-03-20 16:32:30.000000 error-parity-0.3.9/error_parity/cvxpy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12217 2024-03-20 16:32:30.000000 error-parity-0.3.9/error_parity/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16234 2024-03-20 16:32:30.000000 error-parity-0.3.9/error_parity/pareto_curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10619 2024-03-20 16:32:30.000000 error-parity-0.3.9/error_parity/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5202 2024-03-20 16:32:30.000000 error-parity-0.3.9/error_parity/roc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17179 2024-03-20 16:32:30.000000 error-parity-0.3.9/error_parity/threshold_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 16:32:34.915878 error-parity-0.3.9/error_parity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5976 2024-03-20 16:32:34.000000 error-parity-0.3.9/error_parity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-03-20 16:32:34.000000 error-parity-0.3.9/error_parity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 16:32:34.000000 error-parity-0.3.9/error_parity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-20 16:32:34.000000 error-parity-0.3.9/error_parity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-20 16:32:34.000000 error-parity-0.3.9/error_parity.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 16:32:34.915878 error-parity-0.3.9/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-20 16:32:30.000000 error-parity-0.3.9/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-20 16:32:30.000000 error-parity-0.3.9/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-20 16:32:30.000000 error-parity-0.3.9/requirements/main.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-20 16:32:30.000000 error-parity-0.3.9/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 16:32:34.915878 error-parity-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-03-20 16:32:30.000000 error-parity-0.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 16:32:34.915878 error-parity-0.3.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 16:32:30.000000 error-parity-0.3.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-03-20 16:32:30.000000 error-parity-0.3.9/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7413 2024-03-20 16:32:30.000000 error-parity-0.3.9/tests/test_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-03-20 16:32:30.000000 error-parity-0.3.9/tests/test_cvxpy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-03-20 16:32:30.000000 error-parity-0.3.9/tests/test_evaluation.py
```

### Comparing `error-parity-0.3.8/LICENSE` & `error-parity-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `error-parity-0.3.8/PKG-INFO` & `error-parity-0.3.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: error-parity
-Version: 0.3.8
+Version: 0.3.9
 Summary: Achieve error-rate parity between protected groups for any predictor
 Home-page: https://github.com/socialfoundations/error-parity
 Author: AndreFCruz
 License: MIT
 Keywords: ml,optimization,fairness,error-parity,equal-odds
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -50,26 +50,32 @@
 Requires-Dist: tqdm; extra == "all"
 Requires-Dist: mypy; extra == "all"
 
 # error-parity
 
 ![Tests status](https://github.com/socialfoundations/error-parity/actions/workflows/python-package.yml/badge.svg)
 ![PyPI status](https://github.com/socialfoundations/error-parity/actions/workflows/python-publish.yml/badge.svg)
+![Documentation status](https://github.com/socialfoundations/error-parity/actions/workflows/python-docs.yml/badge.svg)
 ![PyPI version](https://badgen.net/pypi/v/error-parity)
 ![OSI license](https://badgen.net/pypi/license/error-parity)
 ![Python compatibility](https://badgen.net/pypi/python/error-parity)
 <!-- ![PyPI version](https://img.shields.io/pypi/v/error-parity) -->
 <!-- ![OSI license](https://img.shields.io/pypi/l/error-parity) -->
 <!-- ![Compatible python versions](https://img.shields.io/pypi/pyversions/error-parity) -->
 
+> Work presented as an _oral at ICLR 2024_, titled ["Unprocessing Seven Years of Algorithmic Fairness"](https://openreview.net/forum?id=jr03SfWsBS).
+
+
 Fast postprocessing of any score-based predictor to meet fairness criteria.
 
 The `error-parity` package can achieve strict or relaxed fairness constraint fulfillment, 
 which can be useful to compare ML models at equal fairness levels.
 
+Package documentation available [here](https://socialfoundations.github.io/error-parity/).
+
 
 ## Installing
 
 Install package from [PyPI](https://pypi.org/project/error-parity/):
 ```
 pip install error-parity
 ```
@@ -87,17 +93,17 @@
 
 ```py
 from error_parity import RelaxedThresholdOptimizer
 
 # Given any trained model that outputs real-valued scores
 fair_clf = RelaxedThresholdOptimizer(
     predictor=lambda X: model.predict_proba(X)[:, -1],   # for sklearn API
-    # predictor=model,  # use this for a callable model
-    constraint="equalized_odds",
-    tolerance=0.05,     # fairness constraint tolerance
+    # predictor=model,            # use this for a callable model
+    constraint="equalized_odds",  # other constraints are available
+    tolerance=0.05,               # fairness constraint tolerance
 )
 
 # Fit the fairness adjustment on some data
 # This will find the optimal _fair classifier_
 fair_clf.fit(X=X, y=y, group=group)
 
 # Now you can use `fair_clf` as any other classifier
@@ -126,18 +132,24 @@
   - use `constraint="equalized_odds"`;
 - [x] equal opportunity;
   - i.e., equal group-specific TPR;
   - use `constraint="true_positive_rate_parity"`;
 - [x] predictive equality;
   - i.e., equal group-specific FPR;
   - use `constraint="false_positive_rate_parity"`;
-
-Road-map:
-- [ ] demographic parity;
+- [x] demographic parity;
   - i.e., equal group-specific predicted prevalence;
+  - use `constraint="demographic_parity"`;
 
 
 ## Citing
 
-This repository contains code and supplementary materials for the following preprint:
-
-> André F. Cruz and Moritz Hardt. "Unprocessing Seven Years of Algorithmic Fairness." [arXiv preprint, 2023](https://arxiv.org/pdf/2306.07261.pdf).
+```
+@inproceedings{
+  cruz2024unprocessing,
+  title={Unprocessing Seven Years of Algorithmic Fairness},
+  author={Andr{\'e} Cruz and Moritz Hardt},
+  booktitle={The Twelfth International Conference on Learning Representations},
+  year={2024},
+  url={https://openreview.net/forum?id=jr03SfWsBS}
+}
+```
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `error-parity-0.3.8/README.md` & `error-parity-0.3.9/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 # error-parity
 
 ![Tests status](https://github.com/socialfoundations/error-parity/actions/workflows/python-package.yml/badge.svg)
 ![PyPI status](https://github.com/socialfoundations/error-parity/actions/workflows/python-publish.yml/badge.svg)
+![Documentation status](https://github.com/socialfoundations/error-parity/actions/workflows/python-docs.yml/badge.svg)
 ![PyPI version](https://badgen.net/pypi/v/error-parity)
 ![OSI license](https://badgen.net/pypi/license/error-parity)
 ![Python compatibility](https://badgen.net/pypi/python/error-parity)
 <!-- ![PyPI version](https://img.shields.io/pypi/v/error-parity) -->
 <!-- ![OSI license](https://img.shields.io/pypi/l/error-parity) -->
 <!-- ![Compatible python versions](https://img.shields.io/pypi/pyversions/error-parity) -->
 
+> Work presented as an _oral at ICLR 2024_, titled ["Unprocessing Seven Years of Algorithmic Fairness"](https://openreview.net/forum?id=jr03SfWsBS).
+
+
 Fast postprocessing of any score-based predictor to meet fairness criteria.
 
 The `error-parity` package can achieve strict or relaxed fairness constraint fulfillment, 
 which can be useful to compare ML models at equal fairness levels.
 
+Package documentation available [here](https://socialfoundations.github.io/error-parity/).
+
 
 ## Installing
 
 Install package from [PyPI](https://pypi.org/project/error-parity/):
 ```
 pip install error-parity
 ```
@@ -35,17 +41,17 @@
 
 ```py
 from error_parity import RelaxedThresholdOptimizer
 
 # Given any trained model that outputs real-valued scores
 fair_clf = RelaxedThresholdOptimizer(
     predictor=lambda X: model.predict_proba(X)[:, -1],   # for sklearn API
-    # predictor=model,  # use this for a callable model
-    constraint="equalized_odds",
-    tolerance=0.05,     # fairness constraint tolerance
+    # predictor=model,            # use this for a callable model
+    constraint="equalized_odds",  # other constraints are available
+    tolerance=0.05,               # fairness constraint tolerance
 )
 
 # Fit the fairness adjustment on some data
 # This will find the optimal _fair classifier_
 fair_clf.fit(X=X, y=y, group=group)
 
 # Now you can use `fair_clf` as any other classifier
@@ -74,18 +80,24 @@
   - use `constraint="equalized_odds"`;
 - [x] equal opportunity;
   - i.e., equal group-specific TPR;
   - use `constraint="true_positive_rate_parity"`;
 - [x] predictive equality;
   - i.e., equal group-specific FPR;
   - use `constraint="false_positive_rate_parity"`;
-
-Road-map:
-- [ ] demographic parity;
+- [x] demographic parity;
   - i.e., equal group-specific predicted prevalence;
+  - use `constraint="demographic_parity"`;
 
 
 ## Citing
 
-This repository contains code and supplementary materials for the following preprint:
-
-> André F. Cruz and Moritz Hardt. "Unprocessing Seven Years of Algorithmic Fairness." [arXiv preprint, 2023](https://arxiv.org/pdf/2306.07261.pdf).
+```
+@inproceedings{
+  cruz2024unprocessing,
+  title={Unprocessing Seven Years of Algorithmic Fairness},
+  author={Andr{\'e} Cruz and Moritz Hardt},
+  booktitle={The Twelfth International Conference on Learning Representations},
+  year={2024},
+  url={https://openreview.net/forum?id=jr03SfWsBS}
+}
+```
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `error-parity-0.3.8/error_parity/_commons.py` & `error-parity-0.3.9/error_parity/_commons.py`

 * *Files identical despite different names*

### Comparing `error-parity-0.3.8/error_parity/binarize.py` & `error-parity-0.3.9/error_parity/binarize.py`

 * *Files identical despite different names*

### Comparing `error-parity-0.3.8/error_parity/classifiers.py` & `error-parity-0.3.9/error_parity/classifiers.py`

 * *Files identical despite different names*

### Comparing `error-parity-0.3.8/error_parity/cvxpy_utils.py` & `error-parity-0.3.9/error_parity/cvxpy_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,19 +12,20 @@
 
 
 # Maximum distance from solution to feasibility or optimality
 SOLUTION_TOLERANCE = 1e-9
 
 # Set of all fairness constraints with a cvxpy LP implementation
 ALL_CONSTRAINTS = {
-    "equalized_odds",
-    "true_positive_rate_parity",
-    "false_positive_rate_parity",
-    "true_negative_rate_parity",
-    "false_negative_rate_parity",
+    "equalized_odds",           # equal TPR and equal FPR across groups
+    "true_positive_rate_parity",    # TPR parity, same as FNR parity
+    "false_positive_rate_parity",   # FPR parity, same as TNR parity
+    "true_negative_rate_parity",    # TNR parity, same as FPR parity
+    "false_negative_rate_parity",   # FNR parity, same as TPR parity
+    "demographic_parity",       # equal positive prediction rates across groups
 }
 
 NOT_SUPPORTED_CONSTRAINTS_ERROR_MESSAGE = (
     "Currently only the following constraints are supported: {}.".format(
         ", ".join(sorted(ALL_CONSTRAINTS))
     )
 )
@@ -228,14 +229,15 @@
 def compute_fair_optimum(
     *,
     fairness_constraint: str,
     tolerance: float,
     groupwise_roc_hulls: dict[int, np.ndarray],
     group_sizes_label_pos: np.ndarray,
     group_sizes_label_neg: np.ndarray,
+    groupwise_prevalence: np.ndarray,
     global_prevalence: float,
     false_positive_cost: float = 1.0,
     false_negative_cost: float = 1.0,
 ) -> tuple[np.ndarray, np.ndarray]:
     """Computes the solution to finding the optimal fair (equal odds) classifier.
 
     Can relax the equal odds constraint by some given tolerance.
@@ -282,19 +284,20 @@
     """
     if fairness_constraint not in ALL_CONSTRAINTS:
         raise ValueError(NOT_SUPPORTED_CONSTRAINTS_ERROR_MESSAGE)
 
     n_groups = len(groupwise_roc_hulls)
     if n_groups != len(group_sizes_label_neg) or n_groups != len(group_sizes_label_pos):
         raise ValueError(
-            f"Invalid arguments; all of the following should have the same "
-            f"length: groupwise_roc_hulls, group_sizes_label_neg, group_sizes_label_pos;"
+            "Invalid arguments; all of the following should have the same "
+            "length: groupwise_roc_hulls, group_sizes_label_neg, group_sizes_label_pos;"
+            f"got: {len(groupwise_roc_hulls)}, {len(group_sizes_label_neg)}, {len(group_sizes_label_pos)};"
         )
 
-    # Group-wise ROC points
+    # Group-wise ROC points --- in the form (FPR, TPR)
     groupwise_roc_points_vars = [
         cp.Variable(shape=2, name=f"ROC point for group {i}", nonneg=True)
         for i in range(n_groups)
     ]
 
     # Define global ROC point as a linear combination of the group-wise ROC points
     global_roc_point_var = cp.Variable(shape=2, name="Global ROC point", nonneg=True)
@@ -303,15 +306,17 @@
         global_roc_point_var[0]
         == group_sizes_label_neg @ np.array([p[0] for p in groupwise_roc_points_vars]),
         # Global TPR is the average of group TPRs weighted by LPs in each group
         global_roc_point_var[1]
         == group_sizes_label_pos @ np.array([p[1] for p in groupwise_roc_points_vars]),
     ]
 
-    ### APPLY FAIRNESS CONSTRAINTS
+    # ** APPLY FAIRNESS CONSTRAINTS **
+    # NOTE: feature request: compatibility with multiple constraints simultaneously
+
     # If "equalized_odds"
     # > i.e., constrain l-inf distance between any two groups' ROCs being less than `tolerance`
     if fairness_constraint == "equalized_odds":
         constraints += [
             cp.norm_inf(groupwise_roc_points_vars[i] - groupwise_roc_points_vars[j])
             <= tolerance
             for i, j in product(range(n_groups), range(n_groups))
@@ -319,39 +324,61 @@
         ]
 
     # If some rate parity, i.e., parity of one of {TPR, FPR, TNR, FNR}
     # i.e., constrain absolute distance between any two groups' rate metric
     elif fairness_constraint.endswith("rate_parity"):
         roc_idx_of_interest: int
         if (
-            fairness_constraint == "true_positive_rate_parity"
-            or fairness_constraint == "false_negative_rate_parity"
+            fairness_constraint == "true_positive_rate_parity"      # TPR
+            or fairness_constraint == "false_negative_rate_parity"  # FNR
         ):
             roc_idx_of_interest = 1
 
         elif (
-            fairness_constraint == "false_positive_rate_parity"
-            or fairness_constraint == "false_negative_rate_parity"
+            fairness_constraint == "false_positive_rate_parity"     # FPR
+            or fairness_constraint == "true_negative_rate_parity"   # TNR
         ):
             roc_idx_of_interest = 0
 
         else:
-            # This point should never be reached as fairness constraint was previously validated
+            # This point should never be reached as fairness_constraint was previously validated
             raise ValueError(NOT_SUPPORTED_CONSTRAINTS_ERROR_MESSAGE)
 
         constraints += [
             cp.abs(
                 groupwise_roc_points_vars[i][roc_idx_of_interest]
                 - groupwise_roc_points_vars[j][roc_idx_of_interest]
             )
             <= tolerance
             for i, j in product(range(n_groups), range(n_groups))
             if i < j
         ]
 
+    # If demographic parity, i.e., equal positive prediction rates across groups
+    # note: this ignores the labels Y and only considers predictions Y_hat
+    elif fairness_constraint == "demographic_parity":
+
+        # NOTE: PPR = TPR * prevalence + FPR * (1 - prevalence)
+        def group_positive_prediction_rate(group_idx: int):
+            """Computes group-wise PPR as a function of the ROC cvxpy vars."""
+            group_prevalence = groupwise_prevalence[group_idx]
+            group_tpr = groupwise_roc_points_vars[group_idx][1]
+            group_fpr = groupwise_roc_points_vars[group_idx][0]
+
+            return group_tpr * group_prevalence + group_fpr * (1 - group_prevalence)
+
+        # Add constraints on the absolute difference between group-wos
+        constraints += [
+            cp.abs(
+                group_positive_prediction_rate(i) - group_positive_prediction_rate(j)
+            ) <= tolerance
+            for i, j in product(range(n_groups), range(n_groups))
+            if i < j
+        ]
+
     # TODO: implement other constraints here
     else:
         raise NotImplementedError(NOT_SUPPORTED_CONSTRAINTS_ERROR_MESSAGE)
 
     # Constraints for points in respective group-wise ROC curves
     for idx in range(n_groups):
         constraints += make_cvxpy_point_in_polygon_constraints(
```

### Comparing `error-parity-0.3.8/error_parity/evaluation.py` & `error-parity-0.3.9/error_parity/evaluation.py`

 * *Files identical despite different names*

### Comparing `error-parity-0.3.8/error_parity/pareto_curve.py` & `error-parity-0.3.9/error_parity/pareto_curve.py`

 * *Files identical despite different names*

### Comparing `error-parity-0.3.8/error_parity/plotting.py` & `error-parity-0.3.9/error_parity/plotting.py`

 * *Files identical despite different names*

### Comparing `error-parity-0.3.8/error_parity/roc_utils.py` & `error-parity-0.3.9/error_parity/roc_utils.py`

 * *Files identical despite different names*

### Comparing `error-parity-0.3.8/error_parity/threshold_optimizer.py` & `error-parity-0.3.9/error_parity/threshold_optimizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,37 +84,48 @@
         if self.constraint not in ALL_CONSTRAINTS:
             raise ValueError(NOT_SUPPORTED_CONSTRAINTS_ERROR_MESSAGE)
 
         # Initialize instance variables
         self._groupwise_roc_data: dict = None
         self._groupwise_roc_hulls: dict = None
         self._groupwise_roc_points: np.ndarray = None
+        self._groupwise_prevalence: np.ndarray = None
         self._global_roc_point: np.ndarray = None
         self._global_prevalence: float = None
         self._realized_classifier: EnsembleGroupwiseClassifiers = None
 
     @property
+    def groupwise_roc_data(self) -> dict:
+        """Group-specific ROC data containing (FPR, TPR, threshold) triplets."""
+        return self._groupwise_roc_data
+
+    @property
+    def groupwise_roc_hulls(self) -> dict:
+        """Group-specific ROC convex hulls achieved by underlying predictor."""
+        return self._groupwise_roc_hulls
+
+    @property
     def groupwise_roc_points(self) -> np.ndarray:
         """Group-specific ROC points achieved by solution."""
         return self._groupwise_roc_points
 
     @property
+    def groupwise_prevalence(self) -> np.ndarray:
+        """Group-specific prevalence, i.e., P(Y=1|A=a)"""
+        return self._groupwise_prevalence
+
+    @property
     def global_roc_point(self) -> np.ndarray:
         """Global ROC point achieved by solution."""
         return self._global_roc_point
 
     @property
-    def groupwise_roc_hulls(self) -> dict:
-        """Group-specific ROC convex hulls achieved by underlying predictor."""
-        return self._groupwise_roc_hulls
-
-    @property
-    def groupwise_roc_data(self) -> dict:
-        """Group-specific ROC data containing (FPR, TPR, threshold) triplets."""
-        return self._groupwise_roc_data
+    def global_prevalence(self) -> np.ndarray:
+        """Global prevalence, i.e., P(Y=1)."""
+        return self._global_prevalence
 
     def cost(
         self,
         false_pos_cost: float = None,
         false_neg_cost: float = None,
     ) -> float:
         """Computes the theoretical cost of the solution found.
@@ -143,46 +154,63 @@
             fpr=global_fpr,
             fnr=1 - global_tpr,
             prevalence=self._global_prevalence,
             false_pos_cost=false_pos_cost or self.false_pos_cost,
             false_neg_cost=false_neg_cost or self.false_neg_cost,
         )
 
-    def constraint_violation(self) -> float:
-        """Constraint violation of the LP solution found.
+    def constraint_violation(self, constraint_name: str = None) -> float:
+        """Theoretical constraint violation of the LP solution found.
+
+        Parameters
+        ----------
+        constraint_name : str, optional
+            Optionally, may provide another constraint name that will be used
+            instead of this classifier's self.constraint;
 
         Returns
         -------
         float
             The fairness constraint violation.
         """
         self._check_fit_status()
 
-        if self.constraint not in ALL_CONSTRAINTS:
+        if constraint_name is not None:
+            logging.warning(
+                f"Calculating constraint violation for {constraint_name} constraint;\n"
+                f"Note: this classifier was fitted with a {self.constraint} constraint;"
+            )
+        else:
+            constraint_name = self.constraint
+
+        if constraint_name not in ALL_CONSTRAINTS:
             raise ValueError(NOT_SUPPORTED_CONSTRAINTS_ERROR_MESSAGE)
 
-        if self.constraint == "equalized_odds":
+        if constraint_name == "equalized_odds":
             return self.equalized_odds_violation()
 
-        elif self.constraint.endswith("rate_parity"):
+        elif constraint_name.endswith("rate_parity"):
             constraint_to_error_type = {
                 "true_positive_rate_parity": "fn",
                 "false_positive_rate_parity": "fp",
                 "true_negative_rate_parity": "fp",
                 "false_negative_rate_parity": "fn",
             }
 
             return self.error_rate_parity_constraint_violation(
-                error_type=constraint_to_error_type[self.constraint],
+                error_type=constraint_to_error_type[constraint_name],
             )
 
+        elif constraint_name == "demographic_parity":
+            return self.demographic_parity_violation()
+
         else:
             raise NotImplementedError(
                 f"Standalone constraint violation not yet computed for "
-                f"constraint='{self.constraint}'."
+                f"constraint='{constraint_name}'."
             )
 
     def error_rate_parity_constraint_violation(self, error_type: str) -> float:
         """Computes the theoretical violation of an error-rate parity constraint.
 
         Parameters
         ----------
@@ -204,15 +232,17 @@
                 f"{valid_error_types}."
             )
 
         roc_idx_of_interest = 0 if error_type == "fp" else 1
 
         return self._max_l_inf_between_points(
             points=[
-                np.reshape(roc_point[roc_idx_of_interest], newshape=(1,))
+                np.reshape(     # NOTE: must pass an array object, not scalars
+                    roc_point[roc_idx_of_interest],  # use only FPR or TPR (whichever was constrained)
+                    newshape=(1,))
                 for roc_point in self.groupwise_roc_points
             ],
         )
 
     def equalized_odds_violation(self) -> float:
         """Computes the theoretical violation of the equal odds constraint
         (i.e., the maximum l-inf distance between the ROC point of any pair
@@ -226,14 +256,39 @@
         self._check_fit_status()
 
         # Compute l-inf distance between each pair of groups
         return self._max_l_inf_between_points(
             points=self.groupwise_roc_points,
         )
 
+    def demographic_parity_violation(self) -> float:
+        """Computes the theoretical violation of the demographic parity constraint.
+
+        That is, the maximum distance between groups' PPR (positive prediction
+        rate).
+
+        Returns
+        -------
+        float
+            The demographic parity constraint violation.
+        """
+        self._check_fit_status()
+
+        # Compute groups' PPR (positive prediction rate)
+        return self._max_l_inf_between_points(  # TODO: check
+            points=[
+                # NOTE: must pass an array object, not scalars
+                np.reshape(
+                    group_tpr * group_prev + group_fpr * (1 - group_prev),
+                    newshape=(1,),
+                )
+                for (group_fpr, group_tpr), group_prev in zip(self.groupwise_roc_points, self.groupwise_prevalence)
+            ],
+        )
+
     @staticmethod
     def _max_l_inf_between_points(points: list[float | np.ndarray]) -> float:
         # Number of points (should correspond to the number of groups)
         n_points = len(points)
 
         # Compute l-inf distance between each pair of groups
         l_inf_constraint_violation = [
@@ -296,24 +351,29 @@
         # Relative group sizes for LN and LP samples
         group_sizes_label_neg = np.array(
             [np.sum(1 - y[group == g]) for g in unique_groups]
         )
         group_sizes_label_pos = np.array([np.sum(y[group == g]) for g in unique_groups])
 
         if np.sum(group_sizes_label_neg) + np.sum(group_sizes_label_pos) != len(y):
-            raise RuntimeError(f"Failed sanity check. Are you using non-binary labels?")
+            raise RuntimeError("Failed sanity check. Are you using non-binary labels?")
 
         # Convert to relative sizes
         group_sizes_label_neg = group_sizes_label_neg.astype(float) / np.sum(
             group_sizes_label_neg
         )
         group_sizes_label_pos = group_sizes_label_pos.astype(float) / np.sum(
             group_sizes_label_pos
         )
 
+        # Compute group-wise prevalence rates
+        self._groupwise_prevalence = np.array(
+            [np.mean(y[group == g]) for g in unique_groups]
+        )
+
         # Compute group-wise ROC curves
         if y_scores is None:
             y_scores = self.predictor(X)
 
         # Flatten y_scores array if needed
         if isinstance(y_scores, np.ndarray) and len(y_scores.shape) > 1:
             y_scores = y_scores.ravel()
@@ -359,15 +419,16 @@
         # Find the group-wise optima that fulfill the fairness criteria
         self._groupwise_roc_points, self._global_roc_point = compute_fair_optimum(
             fairness_constraint=self.constraint,
             tolerance=self.tolerance,
             groupwise_roc_hulls=self._groupwise_roc_hulls,
             group_sizes_label_pos=group_sizes_label_pos,
             group_sizes_label_neg=group_sizes_label_neg,
-            global_prevalence=self._global_prevalence,
+            groupwise_prevalence=self.groupwise_prevalence,
+            global_prevalence=self.global_prevalence,
             false_positive_cost=self.false_pos_cost,
             false_negative_cost=self.false_neg_cost,
         )
 
         # Construct each group-specific classifier
         all_rand_clfs = {
             g: RandomizedClassifier.construct_at_target_ROC(
@@ -427,11 +488,10 @@
             uninitialized.
         """
         if self._realized_classifier is None:
             if not raise_error:
                 return False
 
             raise RuntimeError(
-                "This classifier has not yet been fitted to any data."
-            )
+                "This classifier has not yet been fitted to any data.")
 
         return True
```

### Comparing `error-parity-0.3.8/error_parity.egg-info/PKG-INFO` & `error-parity-0.3.9/error_parity.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: error-parity
-Version: 0.3.8
+Version: 0.3.9
 Summary: Achieve error-rate parity between protected groups for any predictor
 Home-page: https://github.com/socialfoundations/error-parity
 Author: AndreFCruz
 License: MIT
 Keywords: ml,optimization,fairness,error-parity,equal-odds
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -50,26 +50,32 @@
 Requires-Dist: tqdm; extra == "all"
 Requires-Dist: mypy; extra == "all"
 
 # error-parity
 
 ![Tests status](https://github.com/socialfoundations/error-parity/actions/workflows/python-package.yml/badge.svg)
 ![PyPI status](https://github.com/socialfoundations/error-parity/actions/workflows/python-publish.yml/badge.svg)
+![Documentation status](https://github.com/socialfoundations/error-parity/actions/workflows/python-docs.yml/badge.svg)
 ![PyPI version](https://badgen.net/pypi/v/error-parity)
 ![OSI license](https://badgen.net/pypi/license/error-parity)
 ![Python compatibility](https://badgen.net/pypi/python/error-parity)
 <!-- ![PyPI version](https://img.shields.io/pypi/v/error-parity) -->
 <!-- ![OSI license](https://img.shields.io/pypi/l/error-parity) -->
 <!-- ![Compatible python versions](https://img.shields.io/pypi/pyversions/error-parity) -->
 
+> Work presented as an _oral at ICLR 2024_, titled ["Unprocessing Seven Years of Algorithmic Fairness"](https://openreview.net/forum?id=jr03SfWsBS).
+
+
 Fast postprocessing of any score-based predictor to meet fairness criteria.
 
 The `error-parity` package can achieve strict or relaxed fairness constraint fulfillment, 
 which can be useful to compare ML models at equal fairness levels.
 
+Package documentation available [here](https://socialfoundations.github.io/error-parity/).
+
 
 ## Installing
 
 Install package from [PyPI](https://pypi.org/project/error-parity/):
 ```
 pip install error-parity
 ```
@@ -87,17 +93,17 @@
 
 ```py
 from error_parity import RelaxedThresholdOptimizer
 
 # Given any trained model that outputs real-valued scores
 fair_clf = RelaxedThresholdOptimizer(
     predictor=lambda X: model.predict_proba(X)[:, -1],   # for sklearn API
-    # predictor=model,  # use this for a callable model
-    constraint="equalized_odds",
-    tolerance=0.05,     # fairness constraint tolerance
+    # predictor=model,            # use this for a callable model
+    constraint="equalized_odds",  # other constraints are available
+    tolerance=0.05,               # fairness constraint tolerance
 )
 
 # Fit the fairness adjustment on some data
 # This will find the optimal _fair classifier_
 fair_clf.fit(X=X, y=y, group=group)
 
 # Now you can use `fair_clf` as any other classifier
@@ -126,18 +132,24 @@
   - use `constraint="equalized_odds"`;
 - [x] equal opportunity;
   - i.e., equal group-specific TPR;
   - use `constraint="true_positive_rate_parity"`;
 - [x] predictive equality;
   - i.e., equal group-specific FPR;
   - use `constraint="false_positive_rate_parity"`;
-
-Road-map:
-- [ ] demographic parity;
+- [x] demographic parity;
   - i.e., equal group-specific predicted prevalence;
+  - use `constraint="demographic_parity"`;
 
 
 ## Citing
 
-This repository contains code and supplementary materials for the following preprint:
-
-> André F. Cruz and Moritz Hardt. "Unprocessing Seven Years of Algorithmic Fairness." [arXiv preprint, 2023](https://arxiv.org/pdf/2306.07261.pdf).
+```
+@inproceedings{
+  cruz2024unprocessing,
+  title={Unprocessing Seven Years of Algorithmic Fairness},
+  author={Andr{\'e} Cruz and Moritz Hardt},
+  booktitle={The Twelfth International Conference on Learning Representations},
+  year={2024},
+  url={https://openreview.net/forum?id=jr03SfWsBS}
+}
+```
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `error-parity-0.3.8/error_parity.egg-info/SOURCES.txt` & `error-parity-0.3.9/error_parity.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 error_parity/threshold_optimizer.py
 error_parity.egg-info/PKG-INFO
 error_parity.egg-info/SOURCES.txt
 error_parity.egg-info/dependency_links.txt
 error_parity.egg-info/requires.txt
 error_parity.egg-info/top_level.txt
 requirements/dev.txt
+requirements/docs.txt
 requirements/main.txt
 requirements/test.txt
 tests/__init__.py
 tests/conftest.py
+tests/test_constraints.py
 tests/test_cvxpy_utils.py
-tests/test_equal_odds.py
 tests/test_evaluation.py
```

### Comparing `error-parity-0.3.8/setup.py` & `error-parity-0.3.9/setup.py`

 * *Files identical despite different names*

### Comparing `error-parity-0.3.8/tests/conftest.py` & `error-parity-0.3.9/tests/conftest.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,25 +9,39 @@
 
 from __future__ import annotations
 from typing import Iterable
 
 import pytest
 import numpy as np
 
+from error_parity.cvxpy_utils import ALL_CONSTRAINTS
+
 
 @pytest.fixture(params=[42])
 def random_seed(request) -> int:
     return request.param
 
 
 @pytest.fixture
 def rng(random_seed: int) -> np.random.Generator:
     return np.random.default_rng(random_seed)
 
 
+@pytest.fixture(params=[0.01, 0.02, 0.05, 0.1, 0.2, 1.0])
+def constraint_slack(request) -> float:
+    """Fixture for constraint slack/violation (fairness tolerance)."""
+    return request.param
+
+
+@pytest.fixture(params=list(ALL_CONSTRAINTS))
+def fairness_constraint(request) -> float:
+    """Fixture for the fairness constraint to test."""
+    return request.param
+
+
 @pytest.fixture(params=[1_000, 10_000, 100_000])
 def num_samples(request) -> int:
     return request.param
 
 
 @pytest.fixture
 def y_pred_scores(num_samples: int, rng) -> np.ndarray:
```

### Comparing `error-parity-0.3.8/tests/test_cvxpy_utils.py` & `error-parity-0.3.9/tests/test_cvxpy_utils.py`

 * *Files identical despite different names*

### Comparing `error-parity-0.3.8/tests/test_equal_odds.py` & `error-parity-0.3.9/tests/test_constraints.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """Test the relaxed equal odds constraint fulfillment.
 """
 
-import logging
 from itertools import product
 
 import pytest
 import numpy as np
 from sklearn.metrics import roc_auc_score
 
 from error_parity import RelaxedThresholdOptimizer
 from error_parity.cvxpy_utils import SOLUTION_TOLERANCE, calc_cost_of_point
 from error_parity.roc_utils import compute_roc_point_from_predictions
+from error_parity.evaluation import evaluate_fairness
 
 
 def test_synthetic_data_generation(
     y_true: np.ndarray,
     y_pred_scores: np.ndarray,
     sensitive_attribute: np.ndarray,
 ):
@@ -28,31 +28,26 @@
             y_score=y_pred_scores[group_filter],
         )
         # print(f"Group {g} AUC: {group_auc:.3}")
 
         assert 0.52 < group_auc < 0.98
 
 
-@pytest.fixture(params=[0.01, 0.02, 0.05, 0.1, 0.2, 1.0])
-def constraint_slack(request) -> float:
-    """aka. fairness tolerance"""
-    return request.param
-
-
 def get_metric_abs_tolerance(group_size: int) -> float:
     """Reasonable value for metric fulfillment given the inherent randomization
     of predictions and the size of the group over which the metric is computed.
     """
     return (0.1 * group_size) ** (-1 / 1.5)
     # return group_size ** (-1/2)
 
 
 def check_metric_tolerance(
     theory_val: float, empirical_val, group_size: int, metric_name: str = ""
 ) -> bool:
+    """Checks that the empirical value is within a reasonable tolerance of the expected theoretical value."""
     assert np.isclose(
         theory_val,
         empirical_val,
         atol=get_metric_abs_tolerance(group_size),
         rtol=0.01,
     ), f"> '{metric_name}' mismatch; expected {theory_val:.3}; got {empirical_val:.3};"
 
@@ -61,21 +56,23 @@
     with pytest.raises(ValueError) as excinfo:
         clf = RelaxedThresholdOptimizer(
             predictor=print,
             constraint="random constraint name",
         )
 
 
-def test_equalized_odds_constraint_relaxation(
+def test_constraint_fulfillment(
     y_true: np.ndarray,
     y_pred_scores: np.ndarray,
     sensitive_attribute: np.ndarray,
+    fairness_constraint: str,
     constraint_slack: float,
     random_seed: int,
 ):
+    """Tests fairness constraint fulfillment at the given slack level."""
     num_samples = len(y_true)
     unique_groups = np.unique(
         sensitive_attribute
     )  # return is sorted in ascending order
     label_prevalence = np.mean(y_true)
 
     # Predictor function
@@ -83,28 +80,28 @@
     predictor = lambda idx: y_pred_scores[idx]
 
     # Hence, for this example, the features are the sample indices
     X_features = np.arange(num_samples)
 
     clf = RelaxedThresholdOptimizer(
         predictor=predictor,
-        constraint="equalized_odds",
+        constraint=fairness_constraint,
         tolerance=constraint_slack,
         false_pos_cost=1,
         false_neg_cost=1,
         seed=random_seed,
     )
 
     # Fit postprocessing to data
     clf.fit(X=X_features, y=y_true, group=sensitive_attribute)
 
     # Check that theoretical solution fulfills relaxed constraint
-    assert clf.equalized_odds_violation() <= constraint_slack + SOLUTION_TOLERANCE, (
-        f"Solution fails to hit the target EO constraint; "
-        f"got: {clf.equalized_odds_violation()}; "
+    assert clf.constraint_violation() <= constraint_slack + SOLUTION_TOLERANCE, (
+        f"Solution fails to fulfill the '{fairness_constraint}' inequality; "
+        f"got: {clf.constraint_violation()}; "
         f"expected less than {constraint_slack};"
     )
 
     # Optimal binarized predictions
     y_pred_binary = clf(X_features, group=sensitive_attribute)
 
     # Check realized group-specific ROC points
@@ -138,50 +135,69 @@
         check_metric_tolerance(
             target_tpr,
             actual_tpr,
             g_size * g_label_prevalence,
             metric_name=f"group {g} TPR",
         )
 
-    # Check realized constraint violation
-    groupwise_differences = [
-        np.linalg.norm(
-            actual_group_roc_points[i] - actual_group_roc_points[j],
-            ord=np.inf,
-        )
-        for i, j in product(unique_groups, unique_groups)
-        if i < j
-    ]
-
     # > empirical tolerance for constraint violation depends on the smallest group size
     smallest_denominator = min(
         np.sum(labels[sensitive_attribute == g])
         for g in unique_groups
         for labels in (y_true, 1 - y_true)
     )
-    actual_equalized_odds_violation = np.max(groupwise_differences)
+
+    # Compute realized constraint violation
+    empirical_fairness_results = evaluate_fairness(
+        y_true=y_true,
+        y_pred=y_pred_binary,
+        sensitive_attribute=sensitive_attribute,
+    )
+
+    empirical_constraint_violation: float
+    if fairness_constraint == "equalized_odds":
+        empirical_constraint_violation = empirical_fairness_results["equalized_odds_diff"]
+
+    elif fairness_constraint in {"true_positive_rate_parity", "false_negative_rate_parity"}:
+        empirical_constraint_violation = empirical_fairness_results["tpr_diff"]
+
+    elif fairness_constraint in {"false_positive_rate_parity", "true_negative_rate_parity"}:
+        empirical_constraint_violation = empirical_fairness_results["fpr_diff"]
+
+    elif fairness_constraint == "demographic_parity":
+        empirical_constraint_violation = empirical_fairness_results["ppr_diff"]
+
+    else:
+        raise NotImplementedError(f"Tests not implemented for constraint {fairness_constraint}")
+
+    # Assert realized constraint violation is close to theoretical solution found
     check_metric_tolerance(
-        empirical_val=max(actual_equalized_odds_violation - constraint_slack, 0),
+        # NOTE: it's fine if actual violation is below slack (and not fine if above)
+        empirical_val=max(empirical_constraint_violation - constraint_slack, 0),
         theory_val=0.0,
         group_size=smallest_denominator,
-        metric_name="EO violation above slack",
+        metric_name=f"{fairness_constraint} violation above slack",
     )
 
     # Check realized global ROC point
     target_fpr, target_tpr = clf.global_roc_point
     actual_fpr, actual_tpr = compute_roc_point_from_predictions(
         y_true=y_true,
         y_pred_binary=y_pred_binary,
     )
+
+    # Check realized global FPR
     check_metric_tolerance(
         target_fpr,
         actual_fpr,
         group_size=np.sum(1 - y_true),
         metric_name="global FPR",
     )
+
+    # Check realized global TPR
     check_metric_tolerance(
         target_tpr,
         actual_tpr,
         group_size=np.sum(y_true),
         metric_name="global TPR",
     )
```

