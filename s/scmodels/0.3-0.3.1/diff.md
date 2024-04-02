# Comparing `tmp/scmodels-0.3.tar.gz` & `tmp/scmodels-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scmodels-0.3.tar", last modified: Thu Feb 22 20:53:33 2024, max compression
+gzip compressed data, was "scmodels-0.3.1.tar", last modified: Tue Apr  2 09:12:37 2024, max compression
```

## Comparing `scmodels-0.3.tar` & `scmodels-0.3.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 maichmueller   (501) staff       (20)        0 2024-02-22 20:53:33.064463 scmodels-0.3/
--rw-r--r--   0 maichmueller   (501) staff       (20)     1075 2024-02-22 11:22:23.000000 scmodels-0.3/LICENSE.md
--rw-r--r--   0 maichmueller   (501) staff       (20)    12684 2024-02-22 20:53:33.064184 scmodels-0.3/PKG-INFO
--rw-r--r--   0 maichmueller   (501) staff       (20)    10385 2024-02-22 20:50:27.000000 scmodels-0.3/README.md
--rw-r--r--   0 maichmueller   (501) staff       (20)     1322 2024-02-22 20:50:27.000000 scmodels-0.3/pyproject.toml
--rw-r--r--   0 maichmueller   (501) staff       (20)       77 2024-02-22 17:25:32.000000 scmodels-0.3/requirements.txt
--rw-r--r--   0 maichmueller   (501) staff       (20)       38 2024-02-22 20:53:33.064516 scmodels-0.3/setup.cfg
-drwxr-xr-x   0 maichmueller   (501) staff       (20)        0 2024-02-22 20:53:33.060047 scmodels-0.3/src/
-drwxr-xr-x   0 maichmueller   (501) staff       (20)        0 2024-02-22 20:53:33.061738 scmodels-0.3/src/scmodels/
--rw-r--r--   0 maichmueller   (501) staff       (20)       21 2024-02-22 17:25:32.000000 scmodels-0.3/src/scmodels/__init__.py
--rw-r--r--   0 maichmueller   (501) staff       (20)     4458 2024-02-22 17:25:32.000000 scmodels-0.3/src/scmodels/parser.py
--rw-r--r--   0 maichmueller   (501) staff       (20)    45009 2024-02-22 17:25:32.000000 scmodels-0.3/src/scmodels/scm.py
-drwxr-xr-x   0 maichmueller   (501) staff       (20)        0 2024-02-22 20:53:33.063739 scmodels-0.3/src/scmodels.egg-info/
--rw-r--r--   0 maichmueller   (501) staff       (20)    12684 2024-02-22 20:53:33.000000 scmodels-0.3/src/scmodels.egg-info/PKG-INFO
--rw-r--r--   0 maichmueller   (501) staff       (20)      316 2024-02-22 20:53:33.000000 scmodels-0.3/src/scmodels.egg-info/SOURCES.txt
--rw-r--r--   0 maichmueller   (501) staff       (20)        1 2024-02-22 20:53:33.000000 scmodels-0.3/src/scmodels.egg-info/dependency_links.txt
--rw-r--r--   0 maichmueller   (501) staff       (20)      103 2024-02-22 20:53:33.000000 scmodels-0.3/src/scmodels.egg-info/requires.txt
--rw-r--r--   0 maichmueller   (501) staff       (20)        9 2024-02-22 20:53:33.000000 scmodels-0.3/src/scmodels.egg-info/top_level.txt
-drwxr-xr-x   0 maichmueller   (501) staff       (20)        0 2024-02-22 20:53:33.063371 scmodels-0.3/test/
--rw-r--r--   0 maichmueller   (501) staff       (20)    11760 2024-02-22 17:25:32.000000 scmodels-0.3/test/test_scm.py
+drwxr-xr-x   0 maichmueller   (501) staff       (20)        0 2024-04-02 09:12:37.694341 scmodels-0.3.1/
+-rw-r--r--   0 maichmueller   (501) staff       (20)     1075 2024-02-22 11:22:23.000000 scmodels-0.3.1/LICENSE.md
+-rw-r--r--   0 maichmueller   (501) staff       (20)    13247 2024-04-02 09:12:37.694081 scmodels-0.3.1/PKG-INFO
+-rw-r--r--   0 maichmueller   (501) staff       (20)    10946 2024-02-23 11:20:19.000000 scmodels-0.3.1/README.md
+-rw-r--r--   0 maichmueller   (501) staff       (20)     1324 2024-04-02 09:11:54.000000 scmodels-0.3.1/pyproject.toml
+-rw-r--r--   0 maichmueller   (501) staff       (20)       77 2024-02-22 20:59:48.000000 scmodels-0.3.1/requirements.txt
+-rw-r--r--   0 maichmueller   (501) staff       (20)       38 2024-04-02 09:12:37.694400 scmodels-0.3.1/setup.cfg
+drwxr-xr-x   0 maichmueller   (501) staff       (20)        0 2024-04-02 09:12:37.686882 scmodels-0.3.1/src/
+drwxr-xr-x   0 maichmueller   (501) staff       (20)        0 2024-04-02 09:12:37.691755 scmodels-0.3.1/src/scmodels/
+-rw-r--r--   0 maichmueller   (501) staff       (20)       21 2024-02-22 20:59:48.000000 scmodels-0.3.1/src/scmodels/__init__.py
+-rw-r--r--   0 maichmueller   (501) staff       (20)     4409 2024-02-23 11:36:20.000000 scmodels-0.3.1/src/scmodels/parser.py
+-rw-r--r--   0 maichmueller   (501) staff       (20)    47605 2024-04-02 08:57:33.000000 scmodels-0.3.1/src/scmodels/scm.py
+drwxr-xr-x   0 maichmueller   (501) staff       (20)        0 2024-04-02 09:12:37.693675 scmodels-0.3.1/src/scmodels.egg-info/
+-rw-r--r--   0 maichmueller   (501) staff       (20)    13247 2024-04-02 09:12:37.000000 scmodels-0.3.1/src/scmodels.egg-info/PKG-INFO
+-rw-r--r--   0 maichmueller   (501) staff       (20)      316 2024-04-02 09:12:37.000000 scmodels-0.3.1/src/scmodels.egg-info/SOURCES.txt
+-rw-r--r--   0 maichmueller   (501) staff       (20)        1 2024-04-02 09:12:37.000000 scmodels-0.3.1/src/scmodels.egg-info/dependency_links.txt
+-rw-r--r--   0 maichmueller   (501) staff       (20)      103 2024-04-02 09:12:37.000000 scmodels-0.3.1/src/scmodels.egg-info/requires.txt
+-rw-r--r--   0 maichmueller   (501) staff       (20)        9 2024-04-02 09:12:37.000000 scmodels-0.3.1/src/scmodels.egg-info/top_level.txt
+drwxr-xr-x   0 maichmueller   (501) staff       (20)        0 2024-04-02 09:12:37.693313 scmodels-0.3.1/test/
+-rw-r--r--   0 maichmueller   (501) staff       (20)    14070 2024-04-01 20:23:29.000000 scmodels-0.3.1/test/test_scm.py
```

### Comparing `scmodels-0.3/LICENSE.md` & `scmodels-0.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `scmodels-0.3/PKG-INFO` & `scmodels-0.3.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scmodels
-Version: 0.3
+Version: 0.3.1
 Summary: Structural Causal Models
 Author-email: Michael Aichmueller <m.aichmueller@gmail.com>
 License: 
         The MIT License (MIT)
         
         Copyright (c) 2019 Michael
         
@@ -45,19 +45,20 @@
 Requires-Dist: matplotlib>=3.0
 Requires-Dist: sympy>=1.9.0
 Requires-Dist: networkx>=2.0
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 
-| OS        |                                               Status                                               |
-| :-------------: |:--------------------------------------------------------------------------------------------------:|
-| Linux       | ![L Py 3.7 - 3.12](https://github.com/maichmueller/scm/workflows/L%20Py%203.7%20-%203.9/badge.svg) |
-| Windows | ![W Py 3.7 - 3.12](https://github.com/maichmueller/scm/workflows/W%20Py%203.7%20-%203.9/badge.svg) |
-| Mac | ![M Py 3.7 - 3.12](https://github.com/maichmueller/scm/workflows/M%20Py%203.7%20-%203.9/badge.svg) |
+| OS        |                                                                                        Status                                                                                        |
+| :-------------: |:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
+| Linux       | [![Py 3.[7-12]](https://github.com/maichmueller/scmodels/actions/workflows/pytest_linux.yml/badge.svg)](https://github.com/maichmueller/scmodels/actions/workflows/pytest_linux.yml) |
+| Mac |   [![Py 3.[7-12]](https://github.com/maichmueller/scmodels/actions/workflows/pytest_mac.yml/badge.svg)](https://github.com/maichmueller/scmodels/actions/workflows/pytest_mac.yml)   |
+| Windows |   [![Py 3.[7-12]](https://github.com/maichmueller/scmodels/actions/workflows/pytest_win.yml/badge.svg)](https://github.com/maichmueller/scmodels/actions/workflows/pytest_win.yml)   |
+
 
 A Python package implementing Structural Causal Models (SCM).
 
 The library uses the CAS library [SymPy](https://github.com/sympy/sympy) to allow the user to state arbitrary assignment functions and noise distributions as supported by SymPy and builds the DAG with [networkx](https://github.com/networkx/networkx).
 
 It supports the features:
   - Sampling
@@ -136,17 +137,17 @@
 
 One can construct the SCM via an assignment map with the variables as keys
 and a tuple defining the assignment and the noise.
 
 ### 2-Tuple: Assignments via SymPy parsing
 
 To refer to SymPy's string parsing capability (this includes numpy functions) provide a dict entry
-with a 2-tuples as values of the form:
+with 2-tuples as values of the form:
 
-`'var': ('assignment name string', noise)`
+`'var': ('assignment string', noise)`
 
 
 
 
 ```python
 from sympy.stats import LogLogistic, LogNormal, Normal, Bernoulli, StudentT, Exponential
 
@@ -174,26 +175,26 @@
 }
 
 myscm2 = SCM(assignment_map)
 ```
 
 Agreements:
 - the name of the noise distribution provided in its constructor
-(e.g. `Normal("N", mean=2, std=1)`) has to align with the noise variable
-name (`N`) of the assignment string.
+(e.g. `Normal("N", mean=2, std=1)`) must align with the noise variable
+name (`N`) in the assignment string.
 - Multiple noise models in the assignment must be wrapped in an iterable (e.g. a list `[]`, or tuple `()`)
 
 ### 3-Tuple: Assignments with arbitrary callables
 
 One can also declare the SCM via specifying the variable assignment in a dictionary with the
 variables as keys and as values a sequence of length 3 of the form:
 
 `'var': (['parent1', 'parent2', ...], Callable, Noise)`
 
-This allows the user to supply complex functions outside the space of analytical functions.
+This allows the user to supply functions that are not limited to predefined function sets of `scmodels`' dependencies.
 
 
 ```python
 import numpy as np
 
 
 def Y_assignment(p, z, x):
@@ -228,17 +229,16 @@
     )
 }
 
 myscm3 = SCM(functional_map)
 ```
 
 Agreements:
-- The callable's first parameter MUST be the noise input (unless the noise distribution is `None`).
-- The order of variables in the parents list determines the semantic order of input for parameters in the functional
-(left to right).
+- The callable's first parameter MUST be the noise inputs in the order that they are given, e.g. see variable $W$. If the noise distribution list contains only `None`, then they have to be omitted from the parameter list of the callable.
+- The order of variables in the parents list determines the order of input for parameters in the functional past the noise parameters (left to right).
 
 # Features
 
 ## Prettyprint
 
 The SCM supports a form of informative printing of its current setup,
 which includes mentioning active interventions and the assignments.
@@ -288,28 +288,29 @@
 
 ```python
 my_new_callable = lambda n, z: n + z
 
 myscm.intervention({"X": (None, my_new_callable, None)})
 ```
 
-For the example of the do-intervention $\text{do}(X=1)$,
-one can use the helper method `do_intervention`. The pendant for noise interventions is called `soft_intervention`:
+For the example of a do-intervention $\text{do}(X=1)$, the helper method `do_intervention` is provided. Its counterpart for noise interventions is `soft_intervention`:
 
 
 ```python
 myscm.do_intervention([("X", 1)])
 
 from sympy.stats import FiniteRV
 
 myscm.soft_intervention([("X", FiniteRV(str(myscm["X"].noise), density={-1: .5, 1: .5}))])
 ```
 
-Calling `undo_intervention` restores the original state of all variables from construction time, that have been passed. One can optionally specify,
-If no variables are specified (`variables=None`), all interventions are undone.
+Refer to the `sympy` docs for more information on building random variables.
+
+Calling `undo_intervention` restores the original state of *all* variables.
+If variables are specified (`variables=['X', 'Y']`), any interventions on *only those variables* are undone.
 
 
 ```python
 myscm.undo_intervention(variables=["X"])
 ```
 
 ## Sampling
@@ -321,24 +322,24 @@
 n = 5
 samples = myscm.sample(n)
 
 display_data(samples)
 ```
 
 
-|    |        Z |         V |         X |         W |       Y |
-|----|----------|-----------|-----------|-----------|---------|
-|  0 | 0.458971 |  0.468603 | 15.9773   |  8.69091  | 6.41055 |
-|  1 | 0.938629 |  1.93863  | 19.7012   |  3.42096  | 8.39799 |
-|  2 | 0.372148 |  1.37215  |  0.106642 |  1.74083  | 4.11586 |
-|  3 | 1.24888  | -0.187831 | 13.9063   |  0.159301 | 7.66862 |
-|  4 | 0.64198  |  1.64198  | 15.8582   | -2.54485  | 6.30742 |
+|    |        Z |        V |          X |         W |         Y |
+|----|----------|----------|------------|-----------|-----------|
+|  0 | 1.32652  |  2.32652 |  7.33384   |   3.20107 |  6.52168  |
+|  1 | 1.13431  |  2.13431 |  3.8058    | 854.798   |  5.46616  |
+|  2 | 0.573739 | -1.31797 |  1.77705   |  -2.68093 |  5.23906  |
+|  3 | 1.21373  |  2.21373 | 30.1412    |   2.0016  | 11.172    |
+|  4 | 0.117316 |  1.11732 |  0.0147985 |   1.35366 |  0.950457 |
 
 
-If infinite sampling is desired, one can also receive a sampling generator through
+If infinite sampling is desired, one can also receive a sampling generator through 
 
 
 ```python
 container = {var: [] for var in myscm}
 sampler = myscm.sample_iter(container)
 ```
 
@@ -349,36 +350,36 @@
 for i in range(n):
     next(sampler)
 
 display_data(container)
 ```
 
 
-|    |         Z |         V |            X |            W |        Y |
-|----|-----------|-----------|--------------|--------------|----------|
-|  0 | 0.553284  | -0.327667 |   3.26078    | -0.502014    |  4.59572 |
-|  1 | 0.687976  |  1.68798  |   2.28624    |  1.82078     |  4.26111 |
-|  2 | 0.0625212 |  1.06252  |   0.00814341 |  0.154892    |  2.11432 |
-|  3 | 3.81834   |  4.81834  | 143.274      |  6.59465e+08 | 21.3589  |
-|  4 | 0.204415  | -2.32999  |   0.863289   | -0.637428    |  2.62001 |
+|    |         Z |         V |         X |        W |       Y |
+|----|-----------|-----------|-----------|----------|---------|
+|  0 | 0.630663  | -0.151095 | 3.73489   |  2.18306 | 5.02001 |
+|  1 | 0.0978569 |  1.09786  | 0.0875172 | 77.555   | 2.47965 |
+|  2 | 0.225186  |  1.22519  | 0.264414  |  6.47678 | 3.98214 |
+|  3 | 0.143525  |  1.14352  | 0.254132  | 28.4377  | 3.5462  |
+|  4 | 1.13363   |  1.15934  | 6.6198    |  1.38153 | 7.38624 |
 
 
 If the target container is not provided, the generator returns a new `dict` for every sample.
 
 
 ```python
 sample = next(myscm.sample_iter())
 
 display_data(sample)
 ```
 
 
-|    |         Z |         V |        X |         W |       Y |
-|----|-----------|-----------|----------|-----------|---------|
-|  0 | 0.0794389 | 0.0927472 | 0.132214 | 0.0471177 | 3.73759 |
+|    |        Z |       V |         X |       W |       Y |
+|----|----------|---------|-----------|---------|---------|
+|  0 | 0.124314 | 1.12431 | 0.0717258 | 2.43763 | 3.94194 |
 
 
 ## Plotting
 If you have graphviz installed, you can plot the DAG by calling
 
 ```python
 myscm.plot(node_size=1000, alpha=1)
```

### Comparing `scmodels-0.3/README.md` & `scmodels-0.3.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-| OS        |                                               Status                                               |
-| :-------------: |:--------------------------------------------------------------------------------------------------:|
-| Linux       | ![L Py 3.7 - 3.12](https://github.com/maichmueller/scm/workflows/L%20Py%203.7%20-%203.9/badge.svg) |
-| Windows | ![W Py 3.7 - 3.12](https://github.com/maichmueller/scm/workflows/W%20Py%203.7%20-%203.9/badge.svg) |
-| Mac | ![M Py 3.7 - 3.12](https://github.com/maichmueller/scm/workflows/M%20Py%203.7%20-%203.9/badge.svg) |
+| OS        |                                                                                        Status                                                                                        |
+| :-------------: |:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
+| Linux       | [![Py 3.[7-12]](https://github.com/maichmueller/scmodels/actions/workflows/pytest_linux.yml/badge.svg)](https://github.com/maichmueller/scmodels/actions/workflows/pytest_linux.yml) |
+| Mac |   [![Py 3.[7-12]](https://github.com/maichmueller/scmodels/actions/workflows/pytest_mac.yml/badge.svg)](https://github.com/maichmueller/scmodels/actions/workflows/pytest_mac.yml)   |
+| Windows |   [![Py 3.[7-12]](https://github.com/maichmueller/scmodels/actions/workflows/pytest_win.yml/badge.svg)](https://github.com/maichmueller/scmodels/actions/workflows/pytest_win.yml)   |
+
 
 A Python package implementing Structural Causal Models (SCM).
 
 The library uses the CAS library [SymPy](https://github.com/sympy/sympy) to allow the user to state arbitrary assignment functions and noise distributions as supported by SymPy and builds the DAG with [networkx](https://github.com/networkx/networkx).
 
 It supports the features:
   - Sampling
@@ -85,17 +86,17 @@
 
 One can construct the SCM via an assignment map with the variables as keys
 and a tuple defining the assignment and the noise.
 
 ### 2-Tuple: Assignments via SymPy parsing
 
 To refer to SymPy's string parsing capability (this includes numpy functions) provide a dict entry
-with a 2-tuples as values of the form:
+with 2-tuples as values of the form:
 
-`'var': ('assignment name string', noise)`
+`'var': ('assignment string', noise)`
 
 
 
 
 ```python
 from sympy.stats import LogLogistic, LogNormal, Normal, Bernoulli, StudentT, Exponential
 
@@ -123,26 +124,26 @@
 }
 
 myscm2 = SCM(assignment_map)
 ```
 
 Agreements:
 - the name of the noise distribution provided in its constructor
-(e.g. `Normal("N", mean=2, std=1)`) has to align with the noise variable
-name (`N`) of the assignment string.
+(e.g. `Normal("N", mean=2, std=1)`) must align with the noise variable
+name (`N`) in the assignment string.
 - Multiple noise models in the assignment must be wrapped in an iterable (e.g. a list `[]`, or tuple `()`)
 
 ### 3-Tuple: Assignments with arbitrary callables
 
 One can also declare the SCM via specifying the variable assignment in a dictionary with the
 variables as keys and as values a sequence of length 3 of the form:
 
 `'var': (['parent1', 'parent2', ...], Callable, Noise)`
 
-This allows the user to supply complex functions outside the space of analytical functions.
+This allows the user to supply functions that are not limited to predefined function sets of `scmodels`' dependencies.
 
 
 ```python
 import numpy as np
 
 
 def Y_assignment(p, z, x):
@@ -177,17 +178,16 @@
     )
 }
 
 myscm3 = SCM(functional_map)
 ```
 
 Agreements:
-- The callable's first parameter MUST be the noise input (unless the noise distribution is `None`).
-- The order of variables in the parents list determines the semantic order of input for parameters in the functional
-(left to right).
+- The callable's first parameter MUST be the noise inputs in the order that they are given, e.g. see variable $W$. If the noise distribution list contains only `None`, then they have to be omitted from the parameter list of the callable.
+- The order of variables in the parents list determines the order of input for parameters in the functional past the noise parameters (left to right).
 
 # Features
 
 ## Prettyprint
 
 The SCM supports a form of informative printing of its current setup,
 which includes mentioning active interventions and the assignments.
@@ -237,28 +237,29 @@
 
 ```python
 my_new_callable = lambda n, z: n + z
 
 myscm.intervention({"X": (None, my_new_callable, None)})
 ```
 
-For the example of the do-intervention $\text{do}(X=1)$,
-one can use the helper method `do_intervention`. The pendant for noise interventions is called `soft_intervention`:
+For the example of a do-intervention $\text{do}(X=1)$, the helper method `do_intervention` is provided. Its counterpart for noise interventions is `soft_intervention`:
 
 
 ```python
 myscm.do_intervention([("X", 1)])
 
 from sympy.stats import FiniteRV
 
 myscm.soft_intervention([("X", FiniteRV(str(myscm["X"].noise), density={-1: .5, 1: .5}))])
 ```
 
-Calling `undo_intervention` restores the original state of all variables from construction time, that have been passed. One can optionally specify,
-If no variables are specified (`variables=None`), all interventions are undone.
+Refer to the `sympy` docs for more information on building random variables.
+
+Calling `undo_intervention` restores the original state of *all* variables.
+If variables are specified (`variables=['X', 'Y']`), any interventions on *only those variables* are undone.
 
 
 ```python
 myscm.undo_intervention(variables=["X"])
 ```
 
 ## Sampling
@@ -270,24 +271,24 @@
 n = 5
 samples = myscm.sample(n)
 
 display_data(samples)
 ```
 
 
-|    |        Z |         V |         X |         W |       Y |
-|----|----------|-----------|-----------|-----------|---------|
-|  0 | 0.458971 |  0.468603 | 15.9773   |  8.69091  | 6.41055 |
-|  1 | 0.938629 |  1.93863  | 19.7012   |  3.42096  | 8.39799 |
-|  2 | 0.372148 |  1.37215  |  0.106642 |  1.74083  | 4.11586 |
-|  3 | 1.24888  | -0.187831 | 13.9063   |  0.159301 | 7.66862 |
-|  4 | 0.64198  |  1.64198  | 15.8582   | -2.54485  | 6.30742 |
+|    |        Z |        V |          X |         W |         Y |
+|----|----------|----------|------------|-----------|-----------|
+|  0 | 1.32652  |  2.32652 |  7.33384   |   3.20107 |  6.52168  |
+|  1 | 1.13431  |  2.13431 |  3.8058    | 854.798   |  5.46616  |
+|  2 | 0.573739 | -1.31797 |  1.77705   |  -2.68093 |  5.23906  |
+|  3 | 1.21373  |  2.21373 | 30.1412    |   2.0016  | 11.172    |
+|  4 | 0.117316 |  1.11732 |  0.0147985 |   1.35366 |  0.950457 |
 
 
-If infinite sampling is desired, one can also receive a sampling generator through
+If infinite sampling is desired, one can also receive a sampling generator through 
 
 
 ```python
 container = {var: [] for var in myscm}
 sampler = myscm.sample_iter(container)
 ```
 
@@ -298,36 +299,36 @@
 for i in range(n):
     next(sampler)
 
 display_data(container)
 ```
 
 
-|    |         Z |         V |            X |            W |        Y |
-|----|-----------|-----------|--------------|--------------|----------|
-|  0 | 0.553284  | -0.327667 |   3.26078    | -0.502014    |  4.59572 |
-|  1 | 0.687976  |  1.68798  |   2.28624    |  1.82078     |  4.26111 |
-|  2 | 0.0625212 |  1.06252  |   0.00814341 |  0.154892    |  2.11432 |
-|  3 | 3.81834   |  4.81834  | 143.274      |  6.59465e+08 | 21.3589  |
-|  4 | 0.204415  | -2.32999  |   0.863289   | -0.637428    |  2.62001 |
+|    |         Z |         V |         X |        W |       Y |
+|----|-----------|-----------|-----------|----------|---------|
+|  0 | 0.630663  | -0.151095 | 3.73489   |  2.18306 | 5.02001 |
+|  1 | 0.0978569 |  1.09786  | 0.0875172 | 77.555   | 2.47965 |
+|  2 | 0.225186  |  1.22519  | 0.264414  |  6.47678 | 3.98214 |
+|  3 | 0.143525  |  1.14352  | 0.254132  | 28.4377  | 3.5462  |
+|  4 | 1.13363   |  1.15934  | 6.6198    |  1.38153 | 7.38624 |
 
 
 If the target container is not provided, the generator returns a new `dict` for every sample.
 
 
 ```python
 sample = next(myscm.sample_iter())
 
 display_data(sample)
 ```
 
 
-|    |         Z |         V |        X |         W |       Y |
-|----|-----------|-----------|----------|-----------|---------|
-|  0 | 0.0794389 | 0.0927472 | 0.132214 | 0.0471177 | 3.73759 |
+|    |        Z |       V |         X |       W |       Y |
+|----|----------|---------|-----------|---------|---------|
+|  0 | 0.124314 | 1.12431 | 0.0717258 | 2.43763 | 3.94194 |
 
 
 ## Plotting
 If you have graphviz installed, you can plot the DAG by calling
 
 ```python
 myscm.plot(node_size=1000, alpha=1)
```

### Comparing `scmodels-0.3/pyproject.toml` & `scmodels-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'scmodels'
-version = '0.3'
+version = '0.3.1'
 authors = [
     { name = 'Michael Aichmueller', email = 'm.aichmueller@gmail.com' }
 ]
 license = { file = "LICENSE.md" }
 description = 'Structural Causal Models'
 readme = "README.md"
 keywords = [
```

### Comparing `scmodels-0.3/src/scmodels/parser.py` & `scmodels-0.3.1/src/scmodels/parser.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,12 @@
-from collections import deque, defaultdict
 import re as regex
 
 import sympy
 from sympy.functions import *
 from sympy.stats import *
-from sympy.stats.rv import RandomSymbol
-
 
 from typing import *
 
 all_stats_imports = set(sympy.stats.__all__)
 
 var_p = regex.compile(r"(?<=([(]|[)*+-/%]))\w+(?=([)*+-/%]+|$))|^\w+(?=([)*+-/%]+|$))")
 digit_p = regex.compile(r"^\d+$")
@@ -34,15 +31,14 @@
     -------
     dict,
         The functional map of variables with their parents, assignment strings, and noise models as needed to construct
         an SCM object.
     """
     functional_map = dict()
     for assignment in assignment_strs:
-
         # split the assignment 'X = f(Parents, Noise), Noise ~ D' into [X, f(Parents, Noise), Noise ~ D]
         assign_var, assignment_n_noise = assignment.split("=", 1)
         assign_noise_split = assignment_n_noise.split(",", 1)
 
         if len(assign_noise_split) == 1:
             # this is the case when there was no ',' separating functional body and noise distribution specification
             assign_str = assign_noise_split[0]
@@ -50,15 +46,17 @@
         else:
             assign_str, noise_str = assign_noise_split
             _, model_sym = allocate_noise_model(strip_whitespaces(noise_str).split("/"))
         functional_map[assign_var.strip()] = assign_str.strip(), model_sym
     return functional_map
 
 
-def extract_parents(assignment_str: str, noise_var: List[Union[str, sympy.Symbol]]) -> List[str]:
+def extract_parents(
+    assignment_str: str, noise_var: List[Union[str, sympy.Symbol]]
+) -> List[str]:
     """
     Extract the parent variables in an assignment string.
 
     Examples
     --------
     For the following assignment
 
@@ -105,17 +103,19 @@
 def allocate_noise_model(noise_assignments: List[str]):
     model_symbs = [None] * len(noise_assignments)
     noise_vars = [None] * len(noise_assignments)
     for i, noise_assignment in enumerate(noise_assignments):
         noise_var, model = noise_assignment.split("~")
         noise_vars[i] = noise_var
         par_idx = model.find("(") + 1
-        if model[:par_idx-1] not in all_stats_imports:
+        if model[: par_idx - 1] not in all_stats_imports:
             # crude check whether the noise model is supported
-            raise ValueError(f"noise model {model[:par_idx-1]} not supported. Check for spelling errors.")
+            raise ValueError(
+                f"noise model {model[:par_idx - 1]} not supported. Check for spelling errors."
+            )
         model = model[:par_idx] + r'"' + noise_var + r'",' + model[par_idx:]
-        exec(f"model_symbs[i] = {model}")
+        model_symbs[i] = eval(model)
     return noise_vars, model_symbs
 
 
 def strip_whitespaces(s: str):
     return "".join(s.split())
```

### Comparing `scmodels-0.3/src/scmodels/scm.py` & `scmodels-0.3.1/src/scmodels/scm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,45 +1,59 @@
 import logging
 import warnings
 from collections import deque, defaultdict
 from copy import deepcopy
+from dataclasses import dataclass
 from itertools import repeat
 from typing import (
     List,
     Union,
     Dict,
     Tuple,
     Iterable,
     Set,
     Hashable,
     Optional,
     Sequence,
     Iterator,
     Callable,
+    Generator,
+    Type,
 )
-
+from re import compile
 import matplotlib.pyplot as plt
 import networkx as nx
 import numpy as np
 import pandas as pd
 import sympy
 from networkx.drawing.nx_agraph import graphviz_layout
-from sympy.core.singleton import SingletonRegistry
 from sympy.stats import sample, sample_iter, random_symbols
 from sympy.stats.rv import RandomSymbol
 from sympy.functions import *
 
 from scmodels.parser import parse_assignments, extract_parents
 
-RV = RandomSymbol
+RV: Type[RandomSymbol] = RandomSymbol
 AssignmentSeq = Sequence[str]
 AssignmentMap = Dict[str, Union[Tuple[str, RV], Tuple[List[str], Callable, RV]]]
 
 
 class Assignment:
+    noise_prefix = "__noise"
+    noise_suffix = "__"
+    noise_argsep = "@"
+    noise_sep = ":"
+    noise_regex = compile(
+        f"^{noise_prefix}{noise_argsep}"
+        + r"[\w^~&%$!()]*"
+        + noise_sep
+        + r"[\w^~&%$!()]*"
+        + noise_suffix
+    )
+
     def __init__(
         self,
         functor: Callable,
         parents: Sequence[str],
         desc: Optional[str] = None,
     ):
         assert callable(functor), "Passed functor must be callable."
@@ -63,32 +77,37 @@
     def __call__(self, *args, **kwargs):
         args = list(args) + [None] * (len(self) - len(args))
         for var in kwargs:
             if var in self.parents_order:
                 args[self.parents_order[var]] = kwargs[var]
         return self.functor(*args)
 
-    def __str__(self):
+    def __repr__(self):
         if self.descriptor is None:
             return "__unknown__"
         return self.descriptor
 
     @staticmethod
-    def noise_argname(
-        name: Union[str, RV], node_name: Optional[Union[str, sympy.Symbol]] = None
-    ):
+    def noise_argname(name: Union[str, RV], node_name: Union[str, sympy.Symbol] = ""):
         return (
-            f"__"
-            f"noise"
-            f"{'/' if node_name is not None and bool(str(node_name)) else ''}{node_name}"
-            f"{'/' if str(name) else ''}{name}"
-            f"__"
+            f"{Assignment.noise_prefix}"
+            f"{Assignment.noise_argsep}{node_name}"
+            f"{Assignment.noise_sep}{name}"
+            f"{Assignment.noise_suffix}"
         )
 
 
+@dataclass(frozen=True)
+class ColliderView:
+    parent_left: str
+    parent_right: str
+    child: str
+    is_v_structure: Optional[bool] = None
+
+
 class SCM:
     """
     Class building a Structural Causal Model.
 
     With this class one can sample causally from the underlying graph and perform interventions. Do-interventions and
     soft-interventions, as well as more general interventions targeting one or more variables with arbitrary
     changes to the assignment and/or noise structure (including parent-child relationship changes) are supported.
@@ -105,34 +124,22 @@
     (assignment_key, rv_key, noise_key, noise_repr_key) = (
         "assignment",
         "rv",
         "noise",
         "noise_repr",
     )
 
+    @dataclass(frozen=True)
     class NodeView:
-        """
-        A view of the variable's associated attributes
-        """
-
-        def __init__(
-            self,
-            var: str,
-            parents: List[str],
-            assignment: Assignment,
-            rv: RV,
-            noise: RV,
-            noise_repr: str,
-        ):
-            self.variable = var
-            self.parents = parents
-            self.assignment = assignment
-            self.rv = rv
-            self.noise = noise
-            self.noise_repr = noise_repr
+        var: str
+        parents: List[str]
+        assignment: Assignment
+        rv: RV
+        noise: List[RV]
+        noise_repr: List[str]
 
     def __init__(
         self,
         assignments: Union[AssignmentMap, AssignmentSeq],
         variable_tex_names: Optional[Dict] = None,
         seed: Optional[int] = None,
         scm_name: str = "Structural Causal Model",
@@ -230,22 +237,70 @@
             # the variable names as they can be used by the plot function to draw the names in TeX mode.
             self.var_draw_dict: Dict = variable_tex_names
         else:
             self.var_draw_dict = {name: name for name in self.get_variables()}
 
     def __getitem__(self, var):
         attr_dict = self.dag.nodes[var]
-        return SCM.NodeView(var, self.dag.pred[var], **attr_dict)
-
-    def __str__(self):
-        return self.str()
+        return SCM.NodeView(var, list(self.dag.pred[var]), **attr_dict)
 
     def __iter__(self):
         return self._causal_iterator()
 
+    def __str__(self):
+        """
+        Computes a string representation of the SCM. Specifically, returns a string of the form:
+
+        'Structural Causal Model of `nr_variables` variables: X_0, X_1, ...
+         Following variables are actively intervened on: [`list(intervened variables)`]
+         Current Functional Functions are:
+         X_0 := f(N) = `X_0 functional_string_representation` [ NoiseRepr ]
+         X_1 := f(N, X_0) = `X_1 functional_string_representation` [ NoiseRepr ]
+         ...'
+
+        Returns
+        -------
+        str,
+            the representation.
+        """
+        variables = self.get_variables()
+        nr_vars = len(variables)
+        lines = [
+            f"Structural Causal Model of {nr_vars} "
+            + ("variables: " if nr_vars > 1 else "variable: ")
+            + ", ".join(variables[0:10])
+            + (", ..." if nr_vars > 10 else ""),
+            f"Variables with active interventions: {list(self.interventions_backup_attr.keys())}",
+            "Assignments:",
+        ]
+        max_var_space = max([len(var_name) for var_name in variables])
+        for node in self.dag.nodes:
+            parents_vars = [pred for pred in self.dag.predecessors(node)]
+            node_view = self[node]
+            noise_vars = []
+            for noise_symbol in node_view.noise:
+                noise_str = (
+                    str(noise_symbol)
+                    if isinstance(noise_symbol, RV)
+                    else Assignment.noise_argname("")
+                )
+                noise_vars.append(noise_str)
+            parents_vars = noise_vars + parents_vars
+            args_str = ", ".join(parents_vars)
+            line = f"{str(node).rjust(max_var_space)} := f({args_str}) = {str(node_view.assignment)}"
+            if noise_vars:
+                # add explanation to the noise term
+                noise_definitions = [
+                    f"{noise_str} ~ {str(noise_repr)}"
+                    for noise_str, noise_repr in zip(noise_vars, node_view.noise_repr)
+                ]
+                line += f"\t [ " f"{', '.join(noise_definitions)}" f" ]"
+            lines.append(line)
+        return "\n".join(lines)
+
     def sample(
         self,
         n: int,
         variables: Optional[Sequence[Hashable]] = None,
         seed: Optional[Union[int, np.random.Generator]] = None,
     ):
         """
@@ -320,28 +375,28 @@
             the dataframe containing the samples of all the variables needed for the selection.
         """
         if seed is None:
             seed = self.rng_state
         else:
             seed = np.random.default_rng(seed)
         vars_ordered = list(self._causal_iterator(variables))
-        noise_iters: Dict[str, List[Tuple[Optional[str], Iterable]]] = dict()
+        noise_iters: Dict[str, List[Tuple[Optional[str], Iterator]]] = dict()
         for node in vars_ordered:
             noise_gens = self.dag.nodes[node][self.noise_key]
             if noise_gens:
                 noise_iters[node] = []
                 for noise_gen in noise_gens:
                     noise_iter = sample_iter(
                         noise_gen,
                         seed=seed,
                     )
 
                     noise_iters[node].append(
                         (
-                            Assignment.noise_argname(noise_gen, node_name=node),
+                            Assignment.noise_argname(noise_gen, node),
                             noise_iter,
                         )
                     )
             else:
                 noise_iters[node] = [(None, repeat(None))]
 
         if container is None:
@@ -365,15 +420,19 @@
                 samples[node].append(data)
             yield samples
 
     def intervention(
         self,
         interventions: Dict[
             str,
-            Tuple[Optional[List[str]], Optional[Union[str, Callable]], Optional[RV]],
+            Tuple[
+                Optional[List[str]],
+                Optional[Union[str, Callable]],
+                Optional[Union[RV, Sequence[RV]]],
+            ],
         ],
     ):
         """
         Method to apply interventions on the specified variables.
 
         One can set any variable to a new functional and noise model, thus redefining its parents and their
         dependency structure. Using this method will enable the user to call sample, plot etc. on the SCM just like
@@ -392,15 +451,15 @@
                    the old parent structure or the new parent structure (if provided) has to be fit with the
                    positional input of the function.
                    Pass 'None' to leave the original assignment intact.
                 3. The new noise distribution. Ascertain that the new distributions name symbol overlaps with
                    the previous name symbol.
                    Pass 'None' to leave the original noise distribution intact.
         """
-        interventional_map = dict()
+        intervention_assignment_map = dict()
 
         for var, items in interventions.items():
             if var not in self.get_variables():
                 logging.warning(f"Variable '{var}' not found in graph. Omitting it.")
                 continue
 
             if not isinstance(items, Sequence):
@@ -419,27 +478,27 @@
                 items[2] = existing_attr.noise
 
             if items[1] is None:
                 # no new assignment given
                 items[1] = existing_attr.assignment
 
             # whether the assignment is new or old: we have to parse it
-            if callable(items[1]) and items[0] is None:
-                # Rebuild the parents for the assignment, because no new parent info is given,
-                # but a callable assignment needs a parents list
-                sorted_parents = sorted(
-                    self.get_variable_args(var).items(),
-                    key=lambda k: k[1],
-                )
-                items[0] = [
-                    parent
-                    for parent, _ in sorted_parents[
-                        1:
-                    ]  # element 0 is the noise name (must be removed)
-                ]
+            if callable(items[1]):
+                if items[0] is None:
+                    # Rebuild the parents for the assignment, because no new parent info is given,
+                    # but a callable assignment needs a parents list
+                    # we are sorting by the positional index of the parent when passed as arg to the assignment
+                    sorted_parents = sorted(
+                        filter(
+                            lambda elem: SCM.is_not_noise_variable(elem[0]),
+                            self.get_variable_args(var).items(),
+                        ),
+                        key=lambda k: k[1],
+                    )
+                    items[0] = [parent for parent, _ in sorted_parents]
             elif isinstance(items[1], str):
                 # We reach this space only if a new assignment was provided, since existing assignments are already
                 # converted to a callable.
                 # In string assignments the parents list is deduced:
                 items.pop(0)
             else:
                 raise ValueError(
@@ -455,37 +514,37 @@
 
             if var not in self.interventions_backup_parent:
                 # the same logic goes for the parents backup.
                 parent_backup = list(self.dag.predecessors(var))
                 self.interventions_backup_parent[var] = parent_backup
                 self.dag.remove_edges_from([(parent, var) for parent in parent_backup])
             # patch up the attr dict as the provided items were merely strings and now need to be parsed by sympy.
-            interventional_map[var] = items
-        self.insert(interventional_map)
+            intervention_assignment_map[var] = items
+        self.insert(intervention_assignment_map)
 
-    def do_intervention(self, var_val_pairs: Sequence[Tuple[str, float]]):
+    def do_intervention(self, var_val_pairs: Iterable[Tuple[str, float]]):
         """
         Perform do-interventions, i.e. setting specific variables to a constant value.
-        This method removes the noise influence of the intervened variables.
+        This method removes the noise and parent influence of the intervened variables.
 
         Convenience wrapper around ``interventions`` method.
 
         Parameters
         ----------
-        var_val_pairs Sequence of str-float tuple,
+        var_val_pairs, Iterable of str-float tuples,
             the variables to intervene on with their new values.
         """
         interventions_dict = dict()
         for var, val in var_val_pairs:
             interventions_dict[var] = (None, str(val), None)
         self.intervention(interventions_dict)
 
     def soft_intervention(
         self,
-        var_noise_pairs: Sequence[Tuple[str, RV]],
+        var_noise_pairs: Sequence[Tuple[str, Sequence[RV]]],
     ):
         """
         Perform noise interventions, i.e. modifying the noise variable of specific variables.
 
         Convenience wrapper around ``interventions`` method.
 
         Parameters
@@ -553,28 +612,71 @@
         bool,
             A boolean indicating whether x is d-separated from y by s.
         """
         return nx.d_separated(
             self.dag, set(x), set(y), set(s) if s is not None else set()
         )
 
+    def moral_graph(self):
+        """
+        Returns the moral graph of the underlying DAG.
+
+        The moral graph is the underlying DAG with all edges made undirected and collider parents connected.
+
+        Notes
+        -----
+        "Unmarried" parents of a common child are being "married" by this process, hence the name "moral graph".
+
+        Returns
+        -------
+        nx.Graph,
+            an undirected graph which connects all parents of collider nodes
+        """
+        return nx.moral_graph(self.dag)
+
+    def collider_iter(
+        self, only_v_structure: bool = False
+    ) -> Generator[ColliderView, None, None]:
+        """
+        Provide a generator that yields all colliders of the underlying DAG.
+
+        Colliders are triples of nodes (parent, child, other_parent)
+        in which both parent and other_parent causally affect the child,
+        but not each other.
+
+        Returns
+        -------
+        Generator[ColliderView, None, None],
+            the colliders/v-structures found
+        """
+        dag = self.dag
+        for par1, child, par2 in nx.compute_v_structures(dag):
+            adj_parents = dag.has_edge(par1, par2) or dag.has_edge(par2, par1)
+            if adj_parents and only_v_structure:
+                continue
+            ordered_parents = self._order_parents_by_arg_index(
+                self.get_variable_args(child), (par1, par2)
+            )
+            yield ColliderView(*ordered_parents, child, is_v_structure=not adj_parents)
+
     def is_dag(self):
         """
         Check whether the current DAG is indeed a DAG
+
         Returns
         -------
         bool,
             A boolean indicating whether the current graphical model is indeed a DAG.
         """
         return nx.is_directed_acyclic_graph(self.dag)
 
     def insert(self, assignments: Union[AssignmentSeq, AssignmentMap]):
         """
-        Method to insert variables into the graph. The passable assignments are the same as for the constructor of
-        the SCM class.
+        Method to insert variables into the graph.
+        The accepted assignments are the same as for the constructor of the SCM class.
 
         Parameters
         ----------
         assignments, Sequence of str or dictionary of nodes to assignment tuples
             The assignments to add to the graph.
 
         """
@@ -633,15 +735,15 @@
 
             # note that we have to ALWAYS ensure that the assignment func and the list of extended parents
             # (i.e. noise models + actual parent variables) is in exactly the same order as given to the
             # lambdifying call! Otherwise, the Assignment class will assign the wrong positional order to the
             # variables and call the functor incorrectly (since the order differs from when the sympy assignment
             # was lambdified)
             noise_and_parents = [
-                Assignment.noise_argname(noise_model, node_name=node_name)
+                Assignment.noise_argname(noise_model, node_name)
                 for noise_model in noise_model_list
             ] + list(parents)
             assignment = Assignment(
                 assignment_func, noise_and_parents, desc=assignment_str
             )
             attr_dict = {
                 self.assignment_key: assignment,
@@ -744,65 +846,14 @@
             alpha=alpha,
             **kwargs,
         )
         if savepath is not None:
             fig.savefig(savepath)
         return fig, ax
 
-    def str(self):
-        """
-        Computes a string representation of the SCM. Specifically, returns a string of the form:
-
-        'Structural Causal Model of `nr_variables` variables: X_0, X_1, ...
-         Following variables are actively intervened on: [`list(intervened variables)`]
-         Current Functional Functions are:
-         X_0 := f(N) = `X_0 functional_string_representation`
-         X_1 := f(N, X_0) = `X_1 functional_string_representation`
-         ...'
-
-        Returns
-        -------
-        str,
-            the representation.
-        """
-        variables = self.get_variables()
-        nr_vars = len(variables)
-        lines = [
-            f"Structural Causal Model of {nr_vars} "
-            + ("variables: " if nr_vars > 1 else "variable: ")
-            + ", ".join(variables[0:10])
-            + (", ..." if nr_vars > 10 else ""),
-            f"Variables with active interventions: {list(self.interventions_backup_attr.keys())}",
-            "Assignments:",
-        ]
-        max_var_space = max([len(var_name) for var_name in variables])
-        for node in self.dag.nodes:
-            parents_vars = [pred for pred in self.dag.predecessors(node)]
-            node_view = self[node]
-            noise_vars = []
-            for noise_symbol in node_view.noise:
-                noise_str = (
-                    str(noise_symbol)
-                    if isinstance(noise_symbol, RV)
-                    else Assignment.noise_argname("")
-                )
-                noise_vars.append(noise_str)
-            parents_vars = noise_vars + parents_vars
-            args_str = ", ".join(parents_vars)
-            line = f"{str(node).rjust(max_var_space)} := f({args_str}) = {str(node_view.assignment)}"
-            if noise_vars:
-                # add explanation to the noise term
-                noise_definitions = [
-                    f"{noise_str} ~ {str(noise_repr)}"
-                    for noise_str, noise_repr in zip(noise_vars, node_view.noise_repr)
-                ]
-                line += f"\t [ " f"{', '.join(noise_definitions)}" f" ]"
-            lines.append(line)
-        return "\n".join(lines)
-
     def get_variables(self, causal_order: bool = True) -> List[str]:
         """
         Get a list of the variables in the SCM.
 
         Parameters
         ----------
         causal_order: bool (optional),
@@ -900,29 +951,51 @@
                         var_causal_priority[parent], var_causal_priority[nn] + 1
                     )
                     queue.append(parent)
                 visited_nodes.add(nn)
         for key, _ in sorted(var_causal_priority.items(), key=lambda x: -x[1]):
             yield key
 
+    @staticmethod
+    def is_noise_variable(var: str) -> bool:
+        return Assignment.noise_regex.match(var) is not None
+
+    @staticmethod
+    def is_not_noise_variable(var: str) -> bool:
+        return not SCM.is_noise_variable(var)
+
+    @staticmethod
+    def _order_parents_by_arg_index(
+        arg_order: Dict[str, int], parents: Sequence[str]
+    ) -> List[str]:
+        return [
+            parent
+            for parent, _ in sorted(
+                ((par, arg_order[par]) for par in parents),
+                key=lambda p: p[1],
+            )
+        ]
+
 
 def lambdify_assignment(
-    parents: Iterable[str], assignment_str: str, noise_model_list: Optional[List[RV]]
+    parents: Iterable[str],
+    assignment_str: str,
+    noise_model_list: Optional[Iterable[RV]],
 ):
     """
     Parse the provided assignment string with sympy and then lambdifies it, to be used as a normal function.
 
     Parameters
     ----------
     assignment_str: str,
         the assignment to parse.
     parents: Iterable,
         the parents' names.
-    noise_model: RV,
-        the random variable inside the assignment.
+    noise_model_list: Iterable[RV],
+        iterable over the random variables inside the assignment.
 
     Returns
     -------
     function,
         the lambdified assignment.
     """
 
@@ -963,51 +1036,53 @@
     ----------
     scm: SCM,
         The scm is needed for variable RV lookup.
     assignment: str,
         the assignment to parse.
     parents: Iterable,
         the parents' names.
-    noise_model: RV,
-        the random variable inside the assignment.
+    noise_model_list: Iterable[RV],
+        iterable over the random variables inside the assignment.
 
     Returns
     -------
     RV,
         the sympified assignment.
     """
     symbols = []
     # we allocate the symbols with the actual RVs to produce the assignment as RV itself
     for noise_model in noise_model_list:
         symbols.append(noise_model)
         # Allocate the noise model variable as random symbol
         exec(f"{str(noise_model)} = noise_model")
     for par in parents:
         par_rv = scm[par].rv
-        exec(f"{str(par)} = par_rv")
-        exec(f"symbols.append({str(par)})")
+        # add the random variable to the local variables under the name provided by `par` to
+        # allow sympy to sympify the assignment with all variable names having local correspondents
+        locals()[par] = par_rv
+        symbols.append(par_rv)
     if isinstance(assignment, str):
         rv = sympy.sympify(eval(assignment))
     elif callable(assignment):
         rv = assignment(*symbols)
     else:
         raise ValueError(
             f"Passed assignment has to be str or callable. Given: {type(assignment)}."
         )
     return rv
 
 
-def extract_rv_desc(rvs: Optional[List[RV]]):
+def extract_rv_desc(rvs: Optional[Iterable[RV]]):
     """
-    Extracts a human readable string description of the random variable.
+    Extracts a human-readable string description of the random variable.
 
     Parameters
     ----------
-    rv: RV,
-        the random variable.
+    rvs: Iterable[RV],
+        the random variables.
 
     Returns
     -------
     str, the description.
     """
     all_descs = []
     if rvs is not None:
@@ -1175,15 +1250,14 @@
             rightmost_child = max(
                 (x for x, y in [leaf_pos_[child] for child in children])
             )
             leaf_pos_[root_] = ((leftmost_child + rightmost_child) / 2, vert_loc_)
         else:
             leaf_count = 1
             leaf_pos_[root_] = (leftmost_, vert_loc_)
-        #        pos[root] = (leftmost + (leaf_count-1)*dx/2., vert_loc)
         print(leaf_count)
         return root_pos_, leaf_pos_, leaf_count
 
     x_center = width / 2.0
     if isinstance(graph, nx.DiGraph):
         leaf_count = len(
             [
```

### Comparing `scmodels-0.3/src/scmodels.egg-info/PKG-INFO` & `scmodels-0.3.1/src/scmodels.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scmodels
-Version: 0.3
+Version: 0.3.1
 Summary: Structural Causal Models
 Author-email: Michael Aichmueller <m.aichmueller@gmail.com>
 License: 
         The MIT License (MIT)
         
         Copyright (c) 2019 Michael
         
@@ -45,19 +45,20 @@
 Requires-Dist: matplotlib>=3.0
 Requires-Dist: sympy>=1.9.0
 Requires-Dist: networkx>=2.0
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 
-| OS        |                                               Status                                               |
-| :-------------: |:--------------------------------------------------------------------------------------------------:|
-| Linux       | ![L Py 3.7 - 3.12](https://github.com/maichmueller/scm/workflows/L%20Py%203.7%20-%203.9/badge.svg) |
-| Windows | ![W Py 3.7 - 3.12](https://github.com/maichmueller/scm/workflows/W%20Py%203.7%20-%203.9/badge.svg) |
-| Mac | ![M Py 3.7 - 3.12](https://github.com/maichmueller/scm/workflows/M%20Py%203.7%20-%203.9/badge.svg) |
+| OS        |                                                                                        Status                                                                                        |
+| :-------------: |:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
+| Linux       | [![Py 3.[7-12]](https://github.com/maichmueller/scmodels/actions/workflows/pytest_linux.yml/badge.svg)](https://github.com/maichmueller/scmodels/actions/workflows/pytest_linux.yml) |
+| Mac |   [![Py 3.[7-12]](https://github.com/maichmueller/scmodels/actions/workflows/pytest_mac.yml/badge.svg)](https://github.com/maichmueller/scmodels/actions/workflows/pytest_mac.yml)   |
+| Windows |   [![Py 3.[7-12]](https://github.com/maichmueller/scmodels/actions/workflows/pytest_win.yml/badge.svg)](https://github.com/maichmueller/scmodels/actions/workflows/pytest_win.yml)   |
+
 
 A Python package implementing Structural Causal Models (SCM).
 
 The library uses the CAS library [SymPy](https://github.com/sympy/sympy) to allow the user to state arbitrary assignment functions and noise distributions as supported by SymPy and builds the DAG with [networkx](https://github.com/networkx/networkx).
 
 It supports the features:
   - Sampling
@@ -136,17 +137,17 @@
 
 One can construct the SCM via an assignment map with the variables as keys
 and a tuple defining the assignment and the noise.
 
 ### 2-Tuple: Assignments via SymPy parsing
 
 To refer to SymPy's string parsing capability (this includes numpy functions) provide a dict entry
-with a 2-tuples as values of the form:
+with 2-tuples as values of the form:
 
-`'var': ('assignment name string', noise)`
+`'var': ('assignment string', noise)`
 
 
 
 
 ```python
 from sympy.stats import LogLogistic, LogNormal, Normal, Bernoulli, StudentT, Exponential
 
@@ -174,26 +175,26 @@
 }
 
 myscm2 = SCM(assignment_map)
 ```
 
 Agreements:
 - the name of the noise distribution provided in its constructor
-(e.g. `Normal("N", mean=2, std=1)`) has to align with the noise variable
-name (`N`) of the assignment string.
+(e.g. `Normal("N", mean=2, std=1)`) must align with the noise variable
+name (`N`) in the assignment string.
 - Multiple noise models in the assignment must be wrapped in an iterable (e.g. a list `[]`, or tuple `()`)
 
 ### 3-Tuple: Assignments with arbitrary callables
 
 One can also declare the SCM via specifying the variable assignment in a dictionary with the
 variables as keys and as values a sequence of length 3 of the form:
 
 `'var': (['parent1', 'parent2', ...], Callable, Noise)`
 
-This allows the user to supply complex functions outside the space of analytical functions.
+This allows the user to supply functions that are not limited to predefined function sets of `scmodels`' dependencies.
 
 
 ```python
 import numpy as np
 
 
 def Y_assignment(p, z, x):
@@ -228,17 +229,16 @@
     )
 }
 
 myscm3 = SCM(functional_map)
 ```
 
 Agreements:
-- The callable's first parameter MUST be the noise input (unless the noise distribution is `None`).
-- The order of variables in the parents list determines the semantic order of input for parameters in the functional
-(left to right).
+- The callable's first parameter MUST be the noise inputs in the order that they are given, e.g. see variable $W$. If the noise distribution list contains only `None`, then they have to be omitted from the parameter list of the callable.
+- The order of variables in the parents list determines the order of input for parameters in the functional past the noise parameters (left to right).
 
 # Features
 
 ## Prettyprint
 
 The SCM supports a form of informative printing of its current setup,
 which includes mentioning active interventions and the assignments.
@@ -288,28 +288,29 @@
 
 ```python
 my_new_callable = lambda n, z: n + z
 
 myscm.intervention({"X": (None, my_new_callable, None)})
 ```
 
-For the example of the do-intervention $\text{do}(X=1)$,
-one can use the helper method `do_intervention`. The pendant for noise interventions is called `soft_intervention`:
+For the example of a do-intervention $\text{do}(X=1)$, the helper method `do_intervention` is provided. Its counterpart for noise interventions is `soft_intervention`:
 
 
 ```python
 myscm.do_intervention([("X", 1)])
 
 from sympy.stats import FiniteRV
 
 myscm.soft_intervention([("X", FiniteRV(str(myscm["X"].noise), density={-1: .5, 1: .5}))])
 ```
 
-Calling `undo_intervention` restores the original state of all variables from construction time, that have been passed. One can optionally specify,
-If no variables are specified (`variables=None`), all interventions are undone.
+Refer to the `sympy` docs for more information on building random variables.
+
+Calling `undo_intervention` restores the original state of *all* variables.
+If variables are specified (`variables=['X', 'Y']`), any interventions on *only those variables* are undone.
 
 
 ```python
 myscm.undo_intervention(variables=["X"])
 ```
 
 ## Sampling
@@ -321,24 +322,24 @@
 n = 5
 samples = myscm.sample(n)
 
 display_data(samples)
 ```
 
 
-|    |        Z |         V |         X |         W |       Y |
-|----|----------|-----------|-----------|-----------|---------|
-|  0 | 0.458971 |  0.468603 | 15.9773   |  8.69091  | 6.41055 |
-|  1 | 0.938629 |  1.93863  | 19.7012   |  3.42096  | 8.39799 |
-|  2 | 0.372148 |  1.37215  |  0.106642 |  1.74083  | 4.11586 |
-|  3 | 1.24888  | -0.187831 | 13.9063   |  0.159301 | 7.66862 |
-|  4 | 0.64198  |  1.64198  | 15.8582   | -2.54485  | 6.30742 |
+|    |        Z |        V |          X |         W |         Y |
+|----|----------|----------|------------|-----------|-----------|
+|  0 | 1.32652  |  2.32652 |  7.33384   |   3.20107 |  6.52168  |
+|  1 | 1.13431  |  2.13431 |  3.8058    | 854.798   |  5.46616  |
+|  2 | 0.573739 | -1.31797 |  1.77705   |  -2.68093 |  5.23906  |
+|  3 | 1.21373  |  2.21373 | 30.1412    |   2.0016  | 11.172    |
+|  4 | 0.117316 |  1.11732 |  0.0147985 |   1.35366 |  0.950457 |
 
 
-If infinite sampling is desired, one can also receive a sampling generator through
+If infinite sampling is desired, one can also receive a sampling generator through 
 
 
 ```python
 container = {var: [] for var in myscm}
 sampler = myscm.sample_iter(container)
 ```
 
@@ -349,36 +350,36 @@
 for i in range(n):
     next(sampler)
 
 display_data(container)
 ```
 
 
-|    |         Z |         V |            X |            W |        Y |
-|----|-----------|-----------|--------------|--------------|----------|
-|  0 | 0.553284  | -0.327667 |   3.26078    | -0.502014    |  4.59572 |
-|  1 | 0.687976  |  1.68798  |   2.28624    |  1.82078     |  4.26111 |
-|  2 | 0.0625212 |  1.06252  |   0.00814341 |  0.154892    |  2.11432 |
-|  3 | 3.81834   |  4.81834  | 143.274      |  6.59465e+08 | 21.3589  |
-|  4 | 0.204415  | -2.32999  |   0.863289   | -0.637428    |  2.62001 |
+|    |         Z |         V |         X |        W |       Y |
+|----|-----------|-----------|-----------|----------|---------|
+|  0 | 0.630663  | -0.151095 | 3.73489   |  2.18306 | 5.02001 |
+|  1 | 0.0978569 |  1.09786  | 0.0875172 | 77.555   | 2.47965 |
+|  2 | 0.225186  |  1.22519  | 0.264414  |  6.47678 | 3.98214 |
+|  3 | 0.143525  |  1.14352  | 0.254132  | 28.4377  | 3.5462  |
+|  4 | 1.13363   |  1.15934  | 6.6198    |  1.38153 | 7.38624 |
 
 
 If the target container is not provided, the generator returns a new `dict` for every sample.
 
 
 ```python
 sample = next(myscm.sample_iter())
 
 display_data(sample)
 ```
 
 
-|    |         Z |         V |        X |         W |       Y |
-|----|-----------|-----------|----------|-----------|---------|
-|  0 | 0.0794389 | 0.0927472 | 0.132214 | 0.0471177 | 3.73759 |
+|    |        Z |       V |         X |       W |       Y |
+|----|----------|---------|-----------|---------|---------|
+|  0 | 0.124314 | 1.12431 | 0.0717258 | 2.43763 | 3.94194 |
 
 
 ## Plotting
 If you have graphviz installed, you can plot the DAG by calling
 
 ```python
 myscm.plot(node_size=1000, alpha=1)
```

### Comparing `scmodels-0.3/test/test_scm.py` & `scmodels-0.3.1/test/test_scm.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 import random
 import numpy as np
 import pandas as pd
 import pytest
+
 from numpy.polynomial.polynomial import Polynomial
 from test.build_scm import *
+
+from scmodels import SCM
 from scmodels.parser import parse_assignments, extract_parents
+from sympy.stats import *
 
 
 def manual_sample_linandpoly(n, dtype, names, seed):
     def x1(n, x0):
         return 1 + n + Polynomial([0, 0, 2])(x0)
 
     def x2(n, x0, x1):
@@ -265,15 +269,15 @@
 
 def test_scm_softintervention():
     seed = 0
     cn = build_scm_linandpoly(seed=seed)
     n = 100
     standard_sample = cn.sample(n, seed=seed)
     # do the intervention
-    cn.soft_intervention([("X_2", FiniteRV(str(cn["X_2"].noise), density={0: 1.0}))])
+    cn.soft_intervention([("X_2", FiniteRV(cn["X_2"].noise[0].name, density={0: 1.0}))])
     sample = cn.sample(n)
     assignment = cn["X_2"].assignment
     manual_x2 = assignment(0, sample["X_0"], sample["X_1"])
     diff = (sample["X_2"] - manual_x2).abs()
     assert np.all(diff == 0.0)
 
     # from here on the cn should work as normal again
@@ -340,14 +344,38 @@
         rng.exponential(scale=1, size=n) * rng.standard_t(df=0.5, size=n) + manual_y
     )
     assert (samples["X"] == 1).all()
     assert np.isclose(np.mean(samples["Y"]), np.mean(manual_y))
     assert np.isclose(np.mean(samples["Z"]), np.mean(manual_z))
 
 
+def test_compositional_noise_intervention():
+    cn = SCM(
+        [
+            "X = N, N ~ Normal(0,1)",
+            "Y = B**2 + X, B ~ Normal(0,1)",
+            "Z = T*M + Y, M ~ Exponential(1) / T ~ StudentT(0.5)",
+            "V = L + 2 * (X**2), L ~ Normal(0,1)",
+        ],
+        seed=0,
+    )
+    noise_prev = cn["Z"].noise
+    interv_noise = [Normal("K", -3.14, 2.713), Normal("D", 1.41, 7)]
+    interv_assignment = lambda k, d, v: (k + d) * v / 2
+    intervention_dict = {"Z": (["V"], interv_assignment, interv_noise)}
+    cn.intervention(intervention_dict)
+    assert cn["Z"] is not None
+    assert cn["Z"].parents == ["V"]
+    assert cn["Z"].noise == interv_noise
+    cn.undo_intervention()
+    assert cn["Z"] is not None
+    assert cn["Z"].parents == ["Y"]
+    assert cn["Z"].noise == noise_prev
+
+
 def test_compositional_noise_multi():
     cn = SCM(
         [
             "X = 1",
             "Y = N**P + X, N ~ Normal(0,1) / P ~ Bernoulli(0.5)",
             "Z = exp(T) - log(M) * N + Y, M ~ Exponential(1) / T ~ StudentT(0.5) / N ~ Normal(0, 2)",
         ],
@@ -361,7 +389,47 @@
         np.exp(rng.standard_t(df=0.5, size=n))
         - np.log(rng.exponential(scale=1, size=n)) * rng.normal(0, 2, size=n)
         + manual_y
     )
     assert (samples["X"] == 1).all()
     assert np.isclose(np.mean(samples["Y"]), np.mean(manual_y))
     assert np.isclose(np.mean(samples["Z"]), np.mean(manual_z))
+
+
+def test_collider_iter():
+    cn = SCM(
+        [
+            "X = 1",
+            "Y = 1",
+            "Z = X + Y",
+            # v-structure: (X, Y -> Z)
+            "A = Y + Z",
+            # v-structure: (Y, Z -> A)
+            "B = X + Z + A",
+            # v-structure: (X, Z -> B),
+            # v-structure: (X, A -> B),
+            # v-structure: (Z, A -> B)
+            "C = A + B",
+            # collider, but not v-structure: (A, B -> C) because A -> B as well
+            "D = 2 * B",
+            # NOT collider: (?, B -> D)
+        ]
+    )
+    colliders = list(cn.collider_iter())
+    collider_tuples = [(c.parent_left, c.parent_right, c.child) for c in colliders]
+    assert len(colliders) == 6
+    assert ("X", "Y", "Z") in collider_tuples
+    assert ("Y", "Z", "A") in collider_tuples
+    assert ("X", "Z", "B") in collider_tuples
+    assert ("X", "A", "B") in collider_tuples
+    assert ("Z", "A", "B") in collider_tuples
+    assert ("A", "B", "C") in collider_tuples
+
+    colliders = list(cn.collider_iter(True))
+    collider_tuples = [(c.parent_left, c.parent_right, c.child) for c in colliders]
+    assert len(colliders) == 2
+    assert ("X", "Y", "Z") in collider_tuples
+    assert ("Y", "Z", "A") not in collider_tuples
+    assert ("X", "Z", "B") not in collider_tuples
+    assert ("X", "A", "B") in collider_tuples
+    assert ("Z", "A", "B") not in collider_tuples
+    assert ("A", "B", "C") not in collider_tuples
```

