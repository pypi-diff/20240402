# Comparing `tmp/featuristic-0.2.0.tar.gz` & `tmp/featuristic-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featuristic-0.2.0.tar", last modified: Fri Mar 29 15:05:53 2024, max compression
+gzip compressed data, was "featuristic-1.0.0.tar", last modified: Tue Apr  2 20:36:43 2024, max compression
```

## Comparing `featuristic-0.2.0.tar` & `featuristic-1.0.0.tar`

### file list

```diff
@@ -1,31 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:05:53.598583 featuristic-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-03-29 15:05:50.000000 featuristic-0.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-03-29 15:05:53.598583 featuristic-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-03-29 15:05:50.000000 featuristic-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 15:05:53.598583 featuristic-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:05:53.594583 featuristic-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:05:53.594583 featuristic-0.2.0/src/featuristic/
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-03-29 15:05:50.000000 featuristic-0.2.0/src/featuristic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:05:53.594583 featuristic-0.2.0/src/featuristic/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-29 15:05:50.000000 featuristic-0.2.0/src/featuristic/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-03-29 15:05:50.000000 featuristic-0.2.0/src/featuristic/datasets/fetch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:05:53.598583 featuristic-0.2.0/src/featuristic/selection/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-29 15:05:50.000000 featuristic-0.2.0/src/featuristic/selection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6889 2024-03-29 15:05:50.000000 featuristic-0.2.0/src/featuristic/selection/genetic_feature_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     8978 2024-03-29 15:05:50.000000 featuristic-0.2.0/src/featuristic/selection/population.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:05:53.598583 featuristic-0.2.0/src/featuristic/synthesis/
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-03-29 15:05:50.000000 featuristic-0.2.0/src/featuristic/synthesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-03-29 15:05:50.000000 featuristic-0.2.0/src/featuristic/synthesis/fitness.py
--rw-r--r--   0 runner    (1001) docker     (127)    13546 2024-03-29 15:05:50.000000 featuristic-0.2.0/src/featuristic/synthesis/genetic_feature_synthesis.py
--rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-03-29 15:05:50.000000 featuristic-0.2.0/src/featuristic/synthesis/mrmr.py
--rw-r--r--   0 runner    (1001) docker     (127)     8885 2024-03-29 15:05:50.000000 featuristic-0.2.0/src/featuristic/synthesis/population.py
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-03-29 15:05:50.000000 featuristic-0.2.0/src/featuristic/synthesis/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-03-29 15:05:50.000000 featuristic-0.2.0/src/featuristic/synthesis/program.py
--rw-r--r--   0 runner    (1001) docker     (127)    18288 2024-03-29 15:05:50.000000 featuristic-0.2.0/src/featuristic/synthesis/symbolic_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-29 15:05:50.000000 featuristic-0.2.0/src/featuristic/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:05:53.598583 featuristic-0.2.0/src/featuristic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-03-29 15:05:53.000000 featuristic-0.2.0/src/featuristic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-03-29 15:05:53.000000 featuristic-0.2.0/src/featuristic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 15:05:53.000000 featuristic-0.2.0/src/featuristic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-29 15:05:53.000000 featuristic-0.2.0/src/featuristic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-29 15:05:53.000000 featuristic-0.2.0/src/featuristic.egg-info/top_level.txt
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2024-04-02 20:36:43.928841 featuristic-1.0.0/
+-rw-r--r--   0 martin     (501) staff       (20)     1054 2024-02-14 09:40:08.000000 featuristic-1.0.0/LICENSE.txt
+-rw-r--r--   0 martin     (501) staff       (20)    13544 2024-04-02 20:36:43.928586 featuristic-1.0.0/PKG-INFO
+-rw-r--r--   0 martin     (501) staff       (20)     4041 2024-04-02 20:27:28.000000 featuristic-1.0.0/pyproject.toml
+-rw-r--r--   0 martin     (501) staff       (20)    10845 2024-04-02 20:33:46.000000 featuristic-1.0.0/readme.md
+-rw-r--r--   0 martin     (501) staff       (20)       38 2024-04-02 20:36:43.928900 featuristic-1.0.0/setup.cfg
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2024-04-02 20:36:43.919994 featuristic-1.0.0/src/
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2024-04-02 20:36:43.921321 featuristic-1.0.0/src/featuristic/
+-rw-r--r--   0 martin     (501) staff       (20)      389 2024-03-29 13:31:43.000000 featuristic-1.0.0/src/featuristic/__init__.py
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2024-04-02 20:36:43.922458 featuristic-1.0.0/src/featuristic/datasets/
+-rw-r--r--   0 martin     (501) staff       (20)       58 2024-03-29 13:31:43.000000 featuristic-1.0.0/src/featuristic/datasets/__init__.py
+-rw-r--r--   0 martin     (501) staff       (20)      673 2024-03-29 13:31:43.000000 featuristic-1.0.0/src/featuristic/datasets/fetch.py
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2024-04-02 20:36:43.923651 featuristic-1.0.0/src/featuristic/selection/
+-rw-r--r--   0 martin     (501) staff       (20)      126 2024-03-22 21:22:13.000000 featuristic-1.0.0/src/featuristic/selection/__init__.py
+-rw-r--r--   0 martin     (501) staff       (20)     6889 2024-03-27 07:32:06.000000 featuristic-1.0.0/src/featuristic/selection/genetic_feature_selection.py
+-rw-r--r--   0 martin     (501) staff       (20)     8978 2024-03-22 21:19:52.000000 featuristic-1.0.0/src/featuristic/selection/population.py
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2024-04-02 20:36:43.925779 featuristic-1.0.0/src/featuristic/synthesis/
+-rw-r--r--   0 martin     (501) staff       (20)      444 2024-04-02 19:32:50.000000 featuristic-1.0.0/src/featuristic/synthesis/__init__.py
+-rw-r--r--   0 martin     (501) staff       (20)     1164 2024-04-02 19:32:50.000000 featuristic-1.0.0/src/featuristic/synthesis/fitness.py
+-rw-r--r--   0 martin     (501) staff       (20)    13226 2024-04-02 19:32:50.000000 featuristic-1.0.0/src/featuristic/synthesis/genetic_feature_synthesis.py
+-rw-r--r--   0 martin     (501) staff       (20)     4294 2024-04-02 19:32:50.000000 featuristic-1.0.0/src/featuristic/synthesis/mrmr.py
+-rw-r--r--   0 martin     (501) staff       (20)    11903 2024-04-02 19:32:50.000000 featuristic-1.0.0/src/featuristic/synthesis/population.py
+-rw-r--r--   0 martin     (501) staff       (20)     1273 2024-03-22 21:20:49.000000 featuristic-1.0.0/src/featuristic/synthesis/preprocess.py
+-rw-r--r--   0 martin     (501) staff       (20)     2399 2024-03-25 16:59:37.000000 featuristic-1.0.0/src/featuristic/synthesis/program.py
+-rw-r--r--   0 martin     (501) staff       (20)    13678 2024-04-02 19:32:50.000000 featuristic-1.0.0/src/featuristic/synthesis/symbolic_functions.py
+-rw-r--r--   0 martin     (501) staff       (20)       55 2024-04-02 20:27:37.000000 featuristic-1.0.0/src/featuristic/version.py
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2024-04-02 20:36:43.927876 featuristic-1.0.0/src/featuristic.egg-info/
+-rw-r--r--   0 martin     (501) staff       (20)    13544 2024-04-02 20:36:43.000000 featuristic-1.0.0/src/featuristic.egg-info/PKG-INFO
+-rw-r--r--   0 martin     (501) staff       (20)     1034 2024-04-02 20:36:43.000000 featuristic-1.0.0/src/featuristic.egg-info/SOURCES.txt
+-rw-r--r--   0 martin     (501) staff       (20)        1 2024-04-02 20:36:43.000000 featuristic-1.0.0/src/featuristic.egg-info/dependency_links.txt
+-rw-r--r--   0 martin     (501) staff       (20)      227 2024-04-02 20:36:43.000000 featuristic-1.0.0/src/featuristic.egg-info/requires.txt
+-rw-r--r--   0 martin     (501) staff       (20)       12 2024-04-02 20:36:43.000000 featuristic-1.0.0/src/featuristic.egg-info/top_level.txt
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2024-04-02 20:36:43.927417 featuristic-1.0.0/tests/
+-rw-r--r--   0 martin     (501) staff       (20)      421 2024-04-02 19:32:50.000000 featuristic-1.0.0/tests/test_datasets.py
+-rw-r--r--   0 martin     (501) staff       (20)      760 2024-04-02 19:32:50.000000 featuristic-1.0.0/tests/test_fitness.py
+-rw-r--r--   0 martin     (501) staff       (20)      824 2024-04-02 19:32:50.000000 featuristic-1.0.0/tests/test_genetic_feature_selection.py
+-rw-r--r--   0 martin     (501) staff       (20)      895 2024-04-02 19:32:50.000000 featuristic-1.0.0/tests/test_genetic_feature_synthesis.py
+-rw-r--r--   0 martin     (501) staff       (20)      510 2024-04-02 19:32:50.000000 featuristic-1.0.0/tests/test_preprocess.py
+-rw-r--r--   0 martin     (501) staff       (20)     1763 2024-04-02 19:32:50.000000 featuristic-1.0.0/tests/test_programs.py
+-rw-r--r--   0 martin     (501) staff       (20)     5443 2024-04-02 19:32:50.000000 featuristic-1.0.0/tests/test_symbolic_functions.py
```

### Comparing `featuristic-0.2.0/LICENSE.txt` & `featuristic-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `featuristic-0.2.0/pyproject.toml` & `featuristic-1.0.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [project]
 name = "featuristic"
 
 # Versions should comply with PEP 440
-version = "0.2.0"
+version = "1.0.0"
 
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
-description = "Genetic Feature Synthesis and Genetic Feature Selection for Machine Learning"
+description = "An open source library using genetic algorithms for automated feature engineering and feature selection"
 
 
 # This is an optional longer description of your project that represents
 # the body of text which users will see when they visit PyPI.
 #
 # Often, this is the same as your README, so you can just read it in from
 # that file directly (as we have already done above)
 #
 # This field corresponds to the "Description" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#description-optional
-readme = "README.md" # Optional
+readme = "readme.md" # Optional
 
 
 # Specify which Python versions you support. In contrast to the
 # 'Programming Language' classifiers above, 'pip install' will check this
 # and refuse to install the project if the version does not match. See
 # https://packaging.python.org/guides/distributing-packages-using-setuptools/#python-requires
 requires-python = ">=3.8"
@@ -71,20 +71,21 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: 3 :: Only",
 ]
 
 
 dependencies = [
-    "matplotlib",
-    "pandas",
-    "Pyarrow",
-    "scikit-learn",
-    "tqdm",
-    "ucimlrepo",
+    "matplotlib >= 3.0.0",
+    "numpy >= 1.25.0",
+    "pandas >= 2.0.0",
+    "Pyarrow >= 15.0.0",
+    "scikit-learn >= 1.4.0",
+    "tqdm >= 4.32.0",
+    "ucimlrepo >= 0.0.5",
 ] # This field lists other packages that your project depends on to run.
 # Any package you put here will be installed by pip when your project is
 # installed, so they must be valid existing projects.
 #
 # For an analysis of this field vs pip's requirements files see:
 # https://packaging.python.org/discussions/install-requires-vs-requirements/
 
@@ -95,25 +96,26 @@
 #
 #   $ pip install sampleproject[dev]
 #
 # Similar to `dependencies` above, these must be valid existing
 # projects.
 [project.optional-dependencies] # Optional
 dev = [
+    "black",
     "build",
+    "coverage",
+    "coveralls",
+    "isort",
     "ipykernel",
+    "nbsphinx",
+    "pre-commit",
+    "pydata_sphinx_theme",
     "pytest",
     "pylint",
-    "pre-commit",
-    "black",
-    "isort",
-    "coverage",
     "Sphinx",
-    "pydata_sphinx_theme",
-    "nbsphinx",
 ]
 
 [tool.setuptools.packages.find]
 where = ["src/"]
 
 
 # [build-system]
```

### Comparing `featuristic-0.2.0/src/featuristic/datasets/fetch.py` & `featuristic-1.0.0/src/featuristic/datasets/fetch.py`

 * *Files identical despite different names*

### Comparing `featuristic-0.2.0/src/featuristic/selection/genetic_feature_selection.py` & `featuristic-1.0.0/src/featuristic/selection/genetic_feature_selection.py`

 * *Files identical despite different names*

### Comparing `featuristic-0.2.0/src/featuristic/selection/population.py` & `featuristic-1.0.0/src/featuristic/selection/population.py`

 * *Files identical despite different names*

### Comparing `featuristic-0.2.0/src/featuristic/synthesis/fitness.py` & `featuristic-1.0.0/src/featuristic/synthesis/fitness.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import warnings
 
 import numpy as np
 import pandas as pd
 import scipy
 import sys
-from scipy.stats import pearsonr, spearmanr
+from scipy.stats import pearsonr
 
 from .program import node_count
 
 
 def fitness_pearson(
     program: dict, parsimony: float, y_true: pd.Series, y_pred: pd.Series
 ):
@@ -30,51 +30,20 @@
 
     y_pred: pd.Series
         The predicted values
     """
 
     with warnings.catch_warnings(record=True) as _:
         warnings.simplefilter("ignore", category=scipy.stats.NearConstantInputWarning)
-
         if y_pred.isna().any():
             return sys.maxsize
 
         if np.isinf(y_pred).any():
             return sys.maxsize
 
         if np.ptp(y_true) == 0 or np.ptp(y_pred) == 0:
             return sys.maxsize
 
         loss = abs(pearsonr(y_true, y_pred).statistic)
         penalty = node_count(program) ** parsimony
         loss /= penalty
         return -loss
-
-
-def fitness_spearman(
-    program: dict, parsimony: float, y_true: pd.Series, y_pred: pd.Series
-):
-    """
-    Compute the fitness of a program based on the Spearman correlation and the parsimony coefficient
-
-    Args:
-    program: dict
-        The program to evaluate
-
-    parsimony: float
-        The parsimony coefficient
-
-    y_true: pd.Series
-        The true values
-
-    y_pred: pd.Series
-        The predicted values
-    """
-    with warnings.catch_warnings(record=True) as _:
-        warnings.simplefilter("ignore", category=scipy.stats.NearConstantInputWarning)
-        if np.ptp(y_true) == 0 or np.ptp(y_pred) == 0:
-            return 0
-
-        loss = abs(spearmanr(y_true, y_pred).statistic)
-        penalty = node_count(program) ** parsimony
-        loss /= -penalty
-        return loss
```

### Comparing `featuristic-0.2.0/src/featuristic/synthesis/genetic_feature_synthesis.py` & `featuristic-1.0.0/src/featuristic/synthesis/genetic_feature_synthesis.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import matplotlib.pyplot as plt
 import matplotlib
 import pandas as pd
 from joblib import cpu_count
 from sklearn.base import BaseEstimator, TransformerMixin
 from tqdm import tqdm
 
-from .fitness import fitness_pearson, fitness_spearman
+from .fitness import fitness_pearson
 from .mrmr import MaxRelevanceMinRedundancy
 from .population import ParallelPopulation, SerialPopulation
 from .program import render_prog
 from .symbolic_functions import SymbolicFunction, operations
 from .preprocess import preprocess_data
 
 
@@ -28,15 +28,14 @@
     a Maximum Relevance Minimum Redundancy (mRMR) algorithm to find those features
     that are most correlated with the target variable while being least correlated with
     each other.
     """
 
     def __init__(
         self,
-        fitness: str = "pearson",
         functions: Union[List[SymbolicFunction] | None] = None,
         num_features: int = 10,
         population_size: int = 100,
         max_generations: int = 25,
         tournament_size: int = 3,
         crossover_proba: float = 0.85,
         parsimony_coefficient: float = 0.001,
@@ -47,18 +46,14 @@
         verbose: bool = False,
     ):
         """
         Initialize the Symbolic Feature Generator.
 
         Args
         ----
-        fitness : str
-            The fitness function to use. Must be one of
-            `("mae", "mse", "pearson", "spearman")`.
-
         functions : list
             The list of functions to use in the programs. If `None` then all the
             built-in functions are used.
 
         num_features : int
             The number of best features to generate. Internally, `3 * num_features`
             programs are generated and the
@@ -117,30 +112,24 @@
         self.tournament_size = tournament_size
         self.crossover_proba = crossover_proba
         self.num_features = num_features
         self.parsimony_coefficient = parsimony_coefficient
 
         self.history = []
         self.hall_of_fame = []
-        self.len_hall_of_fame = self.num_features * 3
+        self.len_hall_of_fame = self.num_features * 5
 
         self.population = None
 
         self.early_termination_iters = early_termination_iters
         self.early_termination_counter = 0
 
         self.return_all_features = return_all_features
 
-        self.fitness = fitness
-        if fitness == "pearson":
-            self.fitness_func = fitness_pearson
-        elif fitness == "spearman":
-            self.fitness_func = fitness_spearman
-        else:
-            raise ValueError("Invalid fitness function")
+        self.fitness_func = fitness_pearson
 
         self.verbose = verbose
 
         self.fit_called = False
 
         if n_jobs == -1:
             self.n_jobs = cpu_count()
@@ -209,17 +198,17 @@
         y : pd.Series
             The target variable.
 
         return
         ------
         returns self
         """
-        X_copy = X.reset_index(drop=True)
-        y_copy = y.reset_index(drop=True)
-        X_copy, y_copy = preprocess_data(X_copy, y_copy)
+        X_copy, y_copy = preprocess_data(
+            X.reset_index(drop=True), y.reset_index(drop=True)
+        )
 
         # Initialize the population
         if self.n_jobs == 1:
             self.population = SerialPopulation(
                 self.population_size,
                 self.functions,
                 self.tournament_size,
@@ -243,14 +232,18 @@
 
         for gen in range(self.max_generations):
             fitness = []
             prediction = self.population.evaluate(X_copy)
             score = self.population.compute_fitness(
                 self.fitness_func, self.parsimony_coefficient, prediction, y_copy
             )
+            # import pdb
+
+            # pdb.set_trace()
+            # score = self.population.apply_parsimony(score, self.parsimony_coefficient)
             # prog_len = [node_count(prog) for prog in self.population.population]
             # clf = np.cov(prog_len, score)[0, 1]
             # vl = np.var(prog_len)
             # parsimony = clf / vl
             # score = [x - (parsimony * y) for x, y in zip(score, prog_len)]
 
             for prog, score in zip(self.population.population, score):
@@ -398,10 +391,7 @@
 
         if ax is None:
             _, ax = plt.subplots()
 
         df = pd.DataFrame(self.history)
         df.plot(x="generation", y=["best_score", "median_score"], ax=ax)
         plt.show()
-
-
-# matplotlib.axes._axes.Axes
```

### Comparing `featuristic-0.2.0/src/featuristic/synthesis/mrmr.py` & `featuristic-1.0.0/src/featuristic/synthesis/mrmr.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,15 @@
         -------
         list
             The list of selected features.
         """
         # set the maximum number of features to select
         k: int = min(self.k, X.shape[1])
 
-        X = X.loc[:, X.nunique() > 1]
+        X = X.loc[:, X.nunique() > 1].dropna(axis=1)
 
         # calculate the f-statistic and the correlation matrix
         f_stat = pd.Series(self.metric(X, y)[0], index=X.columns)
         corr = pd.DataFrame(FLOOR, index=X.columns, columns=X.columns)
 
         # initialize list of selected features and list of excluded features
         selected = []
```

### Comparing `featuristic-0.2.0/src/featuristic/synthesis/population.py` & `featuristic-1.0.0/src/featuristic/synthesis/population.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-""" The population module contains the classes for the population of programs in the 
+""" The population module contains the classes for the population of programs in the
 genetic programming algorithm. """
 
 from copy import deepcopy
 from typing import Callable, List, Self
 
 import numpy as np
 import pandas as pd
 from joblib import Parallel, cpu_count, delayed
 
-from .program import random_prog, select_random_node
+from .program import random_prog, select_random_node, node_count
 from .symbolic_functions import SymbolicFunction
 
 
 class BasePopulation:
     """
     A class to represent the population of symbolic programs in the
     genetic programming algorithm.
@@ -101,19 +101,15 @@
             The true values.
 
         return
         ------
         list
             The fitness of the population.
         """
-        score = [
-            fitness_func(prog, parsimony_coefficient, y, pred)
-            for prog, pred in zip(self.population, prediction)
-        ]
-        return score
+        raise NotImplementedError
 
     def _evaluate_df(self, node: dict, X: pd.DataFrame) -> pd.Series:
         """
         Evaluate the program against the dataframe of features.
 
         Args
         ----
@@ -269,14 +265,80 @@
 
     def evaluate(self, X: pd.DataFrame) -> List[pd.Series]:
         """
         Evaluate the population against the current program.
         """
         return [self._evaluate_df(prog, X) for prog in self.population]
 
+    def compute_fitness(
+        self,
+        fitness_func: Callable,
+        parsimony_coefficient: float,
+        prediction,
+        y: pd.Series,
+    ) -> List[float]:
+        """
+        Compute the fitness of the population.
+
+        Args
+        ----
+
+        fitness_func : callable
+            The fitness function to use.
+
+        parsimony_coefficient : float
+            The parsimony coefficient.
+
+        prediction : list
+            The predicted values.
+
+        y : pd.Series
+            The true values.
+
+        return
+        ------
+        list
+            The fitness of the population.
+        """
+        score = [
+            fitness_func(prog, parsimony_coefficient, y, pred)
+            for prog, pred in zip(self.population, prediction)
+        ]
+        return score
+
+    def apply_parsimony(
+        self, scores: List[float], parsimony_coefficient: float
+    ) -> List[float]:
+        """
+        Apply the parsimony coefficient to the fitness scores.
+
+        Args
+        ----
+        scores : list
+            The fitness scores.
+
+        parsimony_coefficient : float
+            The parsimony coefficient.
+
+        return
+        ------
+        list
+            The updated fitness scores.
+        """
+
+        def _parsimony_coefficient(loss, prog):
+            penalty = node_count(prog) ** parsimony_coefficient
+            loss = loss / penalty
+            return -loss
+
+        return [
+            _parsimony_coefficient(loss, prog)
+            for loss, prog in zip(scores, self.population)
+        ]
+
 
 class ParallelPopulation(BasePopulation):
     """
     A class to represent the population of programs in the genetic programming algorithm where
     the programs are evaluated in parallel via joblib.
     """
 
@@ -309,7 +371,72 @@
     def evaluate(self, X: pd.DataFrame) -> List[pd.Series]:
         """
         Evaluate the population against the current program. This is done in parallel.
         """
         return Parallel(n_jobs=cpu_count())(
             delayed(self._evaluate_df)(prog, X) for prog in self.population
         )
+
+    def compute_fitness(
+        self,
+        fitness_func: Callable,
+        parsimony_coefficient: float,
+        prediction,
+        y: pd.Series,
+    ) -> List[float]:
+        """
+        Compute the fitness of the population.
+
+        Args
+        ----
+
+        fitness_func : callable
+            The fitness function to use.
+
+        parsimony_coefficient : float
+            The parsimony coefficient.
+
+        prediction : list
+            The predicted values.
+
+        y : pd.Series
+            The true values.
+
+        return
+        ------
+        list
+            The fitness of the population.
+        """
+        return Parallel(n_jobs=cpu_count())(
+            delayed(fitness_func)(prog, parsimony_coefficient, y, pred)
+            for prog, pred in zip(self.population, prediction)
+        )
+
+    def apply_parsimony(
+        self, scores: List[float], parsimony_coefficient: float
+    ) -> List[float]:
+        """
+        Apply the parsimony coefficient to the fitness scores.
+
+        Args
+        ----
+        scores : list
+            The fitness scores.
+
+        parsimony_coefficient : float
+            The parsimony coefficient.
+
+        return
+        ------
+        list
+            The updated fitness scores.
+        """
+
+        def _parsimony_coefficient(loss, prog):
+            penalty = node_count(prog) ** parsimony_coefficient
+            loss = loss / penalty
+            return -loss
+
+        return Parallel(n_jobs=cpu_count())(
+            delayed(_parsimony_coefficient)(score, prog)
+            for score, prog in zip(scores, self.population)
+        )
```

### Comparing `featuristic-0.2.0/src/featuristic/synthesis/preprocess.py` & `featuristic-1.0.0/src/featuristic/synthesis/preprocess.py`

 * *Files identical despite different names*

### Comparing `featuristic-0.2.0/src/featuristic/synthesis/program.py` & `featuristic-1.0.0/src/featuristic/synthesis/program.py`

 * *Files identical despite different names*

### Comparing `featuristic-0.2.0/src/featuristic/synthesis/symbolic_functions.py` & `featuristic-1.0.0/src/featuristic/synthesis/symbolic_functions.py`

 * *Files 15% similar despite different names*

```diff
@@ -569,58 +569,58 @@
     def __call__(self, *args):
         return self.func(*args)
 
     def __str__(self):
         return self.format_str
 
 
-class SymbolicAddConstant:
-    """
-    An internal class used to represent the symbolic functions used to generate new
-    features by the GeneticFeatureGenerator class.
-    """
+# class SymbolicAddConstant:
+#     """
+#     An internal class used to represent the symbolic functions used to generate new
+#     features by the GeneticFeatureGenerator class.
+#     """
 
-    def __init__(self):
-        """
-        Initialize the SymbolicFunction class.
-        """
-
-        self.random_constant = np.random.uniform(-1000, 1000)
-        self.arg_count = 1
-        self.format_str = f"add_constant({self.random_constant} + {{}})"
-        self.name = "add_constant"
+#     def __init__(self):
+#         """
+#         Initialize the SymbolicFunction class.
+#         """
 
-    def __call__(self, x):
-        return self.random_constant + x
+#         self.random_constant = np.random.uniform(-1000, 1000)
+#         self.arg_count = 1
+#         self.format_str = f"add_constant({self.random_constant} + {{}})"
+#         self.name = "add_constant"
 
-    def __str__(self):
-        return self.format_str
+#     def __call__(self, x):
+#         return self.random_constant + x
 
+#     def __str__(self):
+#         return self.format_str
 
-class SymbolicMulConstant:
-    """
-    An internal class used to represent the symbolic functions used to generate new
-    features by the GeneticFeatureGenerator class.
-    """
 
-    def __init__(self):
-        """
-        Initialize the SymbolicFunction class.
-        """
-
-        self.random_constant = np.random.uniform(-1000, 1000)
-        self.arg_count = 1
-        self.format_str = f"mul_constant({self.random_constant} + {{}})"
-        self.name = "mul_constant"
+# class SymbolicMulConstant:
+#     """
+#     An internal class used to represent the symbolic functions used to generate new
+#     features by the GeneticFeatureGenerator class.
+#     """
 
-    def __call__(self, x):
-        return self.random_constant * x
+#     def __init__(self):
+#         """
+#         Initialize the SymbolicFunction class.
+#         """
 
-    def __str__(self):
-        return self.format_str
+#         self.random_constant = np.random.uniform(-1000, 1000)
+#         self.arg_count = 1
+#         self.format_str = f"mul_constant({self.random_constant} + {{}})"
+#         self.name = "mul_constant"
+
+#     def __call__(self, x):
+#         return self.random_constant * x
+
+#     def __str__(self):
+#         return self.format_str
 
 
 operations = [
     SymbolicAdd,
     SymbolicSubtract,
     SymbolicMultiply,
     SymbolicDivide,
@@ -628,252 +628,20 @@
     SymbolicSquare,
     SymbolicCube,
     SymbolicAbs,
     SymbolicNegate,
     SymbolicSin,
     SymbolicCos,
     SymbolicTan,
-    # SymbolicAddConstant,
-    # SymbolicMulConstant,
 ]
 
 
 def list_operations() -> List[str]:
     """
     List the available operations.
 
     Returns
     -------
     list
         The list of built-in operations.
     """
     return [op().name for op in operations]
-
-
-# """Functions to use in the symbolic regression"""
-
-# from typing import Callable, List
-
-# import numpy as np
-
-
-# def safe_div(a, b) -> np.ndarray:
-#     """
-#     Perform safe division by avoiding division by zero.
-
-#     Parameters
-#     ----------
-#     a : float
-#         The numerator.
-
-#     b : float
-#         The denominator.
-
-#     Returns
-#     -------
-#     np.ndarray:
-#         The result of the division.
-#     """
-#     return np.select([b != 0], [a / b], default=a)
-
-
-# def negate(a) -> np.ndarray:
-#     """
-#     Negate the input.
-
-#     Parameters
-#     ----------
-#     a : float
-#         The input.
-
-#     Returns
-#     -------
-#     np.ndarray:
-#         The negated input.
-#     """
-#     return np.multiply(a, -1)
-
-
-# def square(a):
-#     """
-#     Square the input.
-
-#     Parameters
-#     ----------
-#     a : float
-#         The input.
-
-#     Returns
-#     -------
-#     np.ndarray:
-#         The squared input.
-#     """
-#     return np.multiply(a, a)
-
-
-# def cube(a):
-#     """
-#     Cube the input.
-
-#     Parameters
-#     ----------
-#     a : float
-#         The input.
-
-#     Returns
-#     -------
-#     np.ndarray:
-#         The cubed input.
-#     """
-#     return np.multiply(np.multiply(a, a), a)
-
-
-# def sin(a):
-#     """
-#     Compute the sine of the input.
-
-#     Parameters
-#     ----------
-#     a : float
-#         The input.
-
-#     Returns
-#     -------
-#     np.ndarray:
-#         The sine of the input.
-#     """
-#     return np.sin(a)
-
-
-# def cos(a):
-#     """
-#     Compute the cosine of the input.
-
-#     Parameters
-#     ----------
-#     a : float
-#         The input.
-
-#     Returns
-#     -------
-#     np.ndarray:
-#         The cosine of the input.
-#     """
-#     return np.cos(a)
-
-
-# def tan(a):
-#     """
-#     Compute the tangent of the input.
-
-#     Parameters
-#     ----------
-#     a : float
-#         The input.
-
-#     Returns
-#     -------
-#     np.ndarray:
-#         The tangent of the input.
-#     """
-#     return np.tan(a)
-
-
-# def sqrt(a):
-#     """
-#     Compute the square root of the input.
-
-#     Parameters
-#     ----------
-#     a : float
-#         The input.
-
-#     Returns
-#     -------
-#     np.ndarray:
-#         The square root of the input.
-#     """
-#     return np.sqrt(np.abs(a))
-
-
-# class SymbolicFunction:
-#     """
-#     An internal class used to represent the symbolic functions used to generate new
-#     features by the GeneticFeatureGenerator class.
-#     """
-
-#     def __init__(self, func: Callable, arg_count: int, format_str: str, name: str):
-#         """
-#         Initialize the SymbolicFunction class.
-
-#         Parameters
-#         ----------
-#         func : function
-#             The function to use.
-
-#         arg_count : int
-#             The number of arguments the function takes.
-
-#         format_str : str
-#             The format string for the function.
-#         """
-#         self.func = func
-#         self.arg_count = arg_count
-#         self.format_str = format_str
-#         self.name = name
-
-#     def __call__(self, *args):
-#         return self.func(*args)
-
-#     def __str__(self):
-#         return self.format_str
-
-
-# class SymbolicAddConstant:
-#     """
-#     An internal class used to represent the symbolic functions used to generate new
-#     features by the GeneticFeatureGenerator class.
-#     """
-
-#     def __init__(self):
-#         """
-#         Initialize the SymbolicFunction class.
-#         """
-
-#         self.random_constant = np.random.uniform(-100, 100)
-#         self.arg_count = 1
-#         self.format_str = "add_constant({} + {})"
-#         self.name = "add_constant"
-
-#     def __call__(self, x):
-#         return self.rand + x
-
-#     def __str__(self):
-#         return self.format_str
-
-
-# operations = [
-#     SymbolicFunction(np.add, 2, "({} + {})", "add"),
-#     SymbolicFunction(np.subtract, 2, "({} - {})", "subtract"),
-#     SymbolicFunction(np.multiply, 2, "({} * {})", "multiply"),
-#     SymbolicFunction(safe_div, 2, "({} / {})", "divide"),
-#     SymbolicFunction(negate, 1, "-({})", "negate"),
-#     SymbolicFunction(np.abs, 1, "abs({})", "abs"),
-#     SymbolicFunction(square, 1, "square({})", "sqaure"),
-#     SymbolicFunction(cube, 1, "cube({})", "cube"),
-#     SymbolicFunction(sin, 1, "sin({})", "sin"),
-#     SymbolicFunction(cos, 1, "cos({})", "cos"),
-#     SymbolicFunction(tan, 1, "tan({})", "tan"),
-#     SymbolicAddConstant(),
-# ]
-
-
-# def list_operations() -> List[str]:
-#     """
-#     List the available operations.
-
-#     Returns
-#     -------
-#     list
-#         The list of built-in operations.
-#     """
-#     return [op.name for op in operations]
```

