# Comparing `tmp/deampy-1.3.8.tar.gz` & `tmp/deampy-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deampy-1.3.8.tar", last modified: Wed Jan 31 16:02:14 2024, max compression
+gzip compressed data, was "deampy-1.3.9.tar", last modified: Tue Apr  2 18:57:20 2024, max compression
```

## Comparing `deampy-1.3.8.tar` & `deampy-1.3.9.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2024-01-31 16:02:14.037129 deampy-1.3.8/
--rw-rw-rw-   0        0        0     1108 2023-09-20 19:39:29.000000 deampy-1.3.8/LICENSE
--rw-rw-rw-   0        0        0      477 2024-01-31 16:02:14.036131 deampy-1.3.8/PKG-INFO
--rw-rw-rw-   0        0        0       59 2023-09-20 19:39:29.000000 deampy-1.3.8/README.md
-drwxrwxrwx   0        0        0        0 2024-01-31 16:02:13.985240 deampy-1.3.8/deampy/
--rw-rw-rw-   0        0        0      262 2023-09-20 19:39:29.000000 deampy-1.3.8/deampy/__init__.py
--rw-rw-rw-   0        0        0    22678 2023-09-20 19:39:29.000000 deampy-1.3.8/deampy/data_structure.py
--rw-rw-rw-   0        0        0     9513 2023-09-20 19:39:29.000000 deampy-1.3.8/deampy/decision_tree.py
--rw-rw-rw-   0        0        0     2096 2023-09-20 19:39:29.000000 deampy-1.3.8/deampy/discrete_event_sim.py
--rw-rw-rw-   0        0        0   147709 2023-11-09 17:09:13.000000 deampy-1.3.8/deampy/econ_eval.py
--rw-rw-rw-   0        0        0     5053 2023-09-20 19:39:29.000000 deampy-1.3.8/deampy/format_functions.py
--rw-rw-rw-   0        0        0     9288 2023-09-20 19:39:29.000000 deampy-1.3.8/deampy/in_out_functions.py
--rw-rw-rw-   0        0        0     9637 2023-09-20 19:39:29.000000 deampy-1.3.8/deampy/markov.py
--rw-rw-rw-   0        0        0     1907 2023-09-20 19:39:29.000000 deampy-1.3.8/deampy/models.py
-drwxrwxrwx   0        0        0        0 2024-01-31 16:02:14.004514 deampy-1.3.8/deampy/optimization/
--rw-rw-rw-   0        0        0        0 2023-09-20 19:39:29.000000 deampy-1.3.8/deampy/optimization/__init__.py
--rw-rw-rw-   0        0        0    26227 2023-09-20 19:39:29.000000 deampy-1.3.8/deampy/optimization/appx_policy_itr.py
--rw-rw-rw-   0        0        0     1079 2023-09-20 19:39:29.000000 deampy-1.3.8/deampy/optimization/learning_exploring_rules.py
--rw-rw-rw-   0        0        0      298 2023-09-20 19:39:29.000000 deampy-1.3.8/deampy/optimization/opt_support.py
--rw-rw-rw-   0        0        0     8766 2023-09-20 19:39:29.000000 deampy-1.3.8/deampy/optimization/stoch_approx.py
--rw-rw-rw-   0        0        0    21553 2023-09-20 19:39:29.000000 deampy-1.3.8/deampy/parameter_estimation.py
--rw-rw-rw-   0        0        0    24387 2023-11-16 03:14:19.000000 deampy-1.3.8/deampy/parameters.py
-drwxrwxrwx   0        0        0        0 2024-01-31 16:02:14.021832 deampy-1.3.8/deampy/plots/
--rw-rw-rw-   0        0        0        0 2023-09-20 19:39:29.000000 deampy-1.3.8/deampy/plots/__init__.py
--rw-rw-rw-   0        0        0     7501 2023-11-09 17:27:55.000000 deampy-1.3.8/deampy/plots/econ_eval_plots.py
--rw-rw-rw-   0        0        0     1368 2023-09-20 19:39:29.000000 deampy-1.3.8/deampy/plots/eff_sample_size.py
--rw-rw-rw-   0        0        0     7019 2023-09-20 19:39:29.000000 deampy-1.3.8/deampy/plots/histogram.py
--rw-rw-rw-   0        0        0     2825 2023-10-13 19:50:23.000000 deampy-1.3.8/deampy/plots/plot_support.py
--rw-rw-rw-   0        0        0     6492 2023-09-20 19:39:29.000000 deampy-1.3.8/deampy/plots/pop_pyramids.py
--rw-rw-rw-   0        0        0    26140 2023-11-14 02:11:09.000000 deampy-1.3.8/deampy/plots/prob_dists.py
--rw-rw-rw-   0        0        0    10328 2024-01-31 15:50:48.000000 deampy-1.3.8/deampy/plots/sample_paths.py
--rw-rw-rw-   0        0        0    42089 2023-11-14 02:10:47.000000 deampy-1.3.8/deampy/random_variates.py
--rw-rw-rw-   0        0        0    16282 2023-09-20 19:39:29.000000 deampy-1.3.8/deampy/regression_models.py
--rw-rw-rw-   0        0        0     9436 2023-09-20 19:39:29.000000 deampy-1.3.8/deampy/sample_path.py
--rw-rw-rw-   0        0        0     6676 2023-09-20 19:39:29.000000 deampy-1.3.8/deampy/sensitivity_analysis.py
--rw-rw-rw-   0        0        0    44324 2023-10-30 00:56:25.000000 deampy-1.3.8/deampy/statistics.py
-drwxrwxrwx   0        0        0        0 2024-01-31 16:02:14.032051 deampy-1.3.8/deampy/support/
--rw-rw-rw-   0        0        0        0 2023-09-20 19:39:30.000000 deampy-1.3.8/deampy/support/__init__.py
--rw-rw-rw-   0        0        0    10009 2023-09-20 19:39:30.000000 deampy-1.3.8/deampy/support/econ_eval_support.py
--rw-rw-rw-   0        0        0      659 2023-09-20 19:39:30.000000 deampy-1.3.8/deampy/support/misc_classes.py
--rw-rw-rw-   0        0        0     7094 2023-09-20 19:39:30.000000 deampy-1.3.8/deampy/support/misc_functions.py
--rw-rw-rw-   0        0        0     6635 2023-09-20 19:39:30.000000 deampy-1.3.8/deampy/support/simulation.py
-drwxrwxrwx   0        0        0        0 2024-01-31 16:02:14.034107 deampy-1.3.8/deampy.egg-info/
--rw-rw-rw-   0        0        0      477 2024-01-31 16:02:13.000000 deampy-1.3.8/deampy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1135 2024-01-31 16:02:13.000000 deampy-1.3.8/deampy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-31 16:02:13.000000 deampy-1.3.8/deampy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-01-31 16:02:13.000000 deampy-1.3.8/deampy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-01-31 16:02:13.000000 deampy-1.3.8/deampy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-01-31 16:02:14.038178 deampy-1.3.8/setup.cfg
--rw-rw-rw-   0        0        0      706 2024-01-31 16:02:00.000000 deampy-1.3.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 18:57:20.529688 deampy-1.3.9/
+-rw-rw-rw-   0        0        0     1108 2023-09-20 19:39:29.000000 deampy-1.3.9/LICENSE
+-rw-rw-rw-   0        0        0      477 2024-04-02 18:57:20.527694 deampy-1.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0       59 2023-09-20 19:39:29.000000 deampy-1.3.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 18:57:20.471843 deampy-1.3.9/deampy/
+-rw-rw-rw-   0        0        0      262 2023-09-20 19:39:29.000000 deampy-1.3.9/deampy/__init__.py
+-rw-rw-rw-   0        0        0    22678 2023-09-20 19:39:29.000000 deampy-1.3.9/deampy/data_structure.py
+-rw-rw-rw-   0        0        0     9513 2023-09-20 19:39:29.000000 deampy-1.3.9/deampy/decision_tree.py
+-rw-rw-rw-   0        0        0     2096 2023-09-20 19:39:29.000000 deampy-1.3.9/deampy/discrete_event_sim.py
+-rw-rw-rw-   0        0        0   147709 2023-11-09 17:09:13.000000 deampy-1.3.9/deampy/econ_eval.py
+-rw-rw-rw-   0        0        0     5053 2023-09-20 19:39:29.000000 deampy-1.3.9/deampy/format_functions.py
+-rw-rw-rw-   0        0        0     9288 2023-09-20 19:39:29.000000 deampy-1.3.9/deampy/in_out_functions.py
+-rw-rw-rw-   0        0        0     9637 2023-09-20 19:39:29.000000 deampy-1.3.9/deampy/markov.py
+-rw-rw-rw-   0        0        0     1907 2023-09-20 19:39:29.000000 deampy-1.3.9/deampy/models.py
+drwxrwxrwx   0        0        0        0 2024-04-02 18:57:20.492787 deampy-1.3.9/deampy/optimization/
+-rw-rw-rw-   0        0        0        0 2023-09-20 19:39:29.000000 deampy-1.3.9/deampy/optimization/__init__.py
+-rw-rw-rw-   0        0        0    26227 2023-09-20 19:39:29.000000 deampy-1.3.9/deampy/optimization/appx_policy_itr.py
+-rw-rw-rw-   0        0        0     1079 2023-09-20 19:39:29.000000 deampy-1.3.9/deampy/optimization/learning_exploring_rules.py
+-rw-rw-rw-   0        0        0      298 2023-09-20 19:39:29.000000 deampy-1.3.9/deampy/optimization/opt_support.py
+-rw-rw-rw-   0        0        0     8766 2023-09-20 19:39:29.000000 deampy-1.3.9/deampy/optimization/stoch_approx.py
+-rw-rw-rw-   0        0        0    21553 2023-09-20 19:39:29.000000 deampy-1.3.9/deampy/parameter_estimation.py
+-rw-rw-rw-   0        0        0    24387 2023-11-16 03:14:19.000000 deampy-1.3.9/deampy/parameters.py
+drwxrwxrwx   0        0        0        0 2024-04-02 18:57:20.511736 deampy-1.3.9/deampy/plots/
+-rw-rw-rw-   0        0        0        0 2023-09-20 19:39:29.000000 deampy-1.3.9/deampy/plots/__init__.py
+-rw-rw-rw-   0        0        0     7501 2023-11-09 17:27:55.000000 deampy-1.3.9/deampy/plots/econ_eval_plots.py
+-rw-rw-rw-   0        0        0     1368 2023-09-20 19:39:29.000000 deampy-1.3.9/deampy/plots/eff_sample_size.py
+-rw-rw-rw-   0        0        0     7019 2023-09-20 19:39:29.000000 deampy-1.3.9/deampy/plots/histogram.py
+-rw-rw-rw-   0        0        0     2825 2023-10-13 19:50:23.000000 deampy-1.3.9/deampy/plots/plot_support.py
+-rw-rw-rw-   0        0        0     6492 2023-09-20 19:39:29.000000 deampy-1.3.9/deampy/plots/pop_pyramids.py
+-rw-rw-rw-   0        0        0    26140 2023-11-14 02:11:09.000000 deampy-1.3.9/deampy/plots/prob_dists.py
+-rw-rw-rw-   0        0        0    10328 2024-01-31 15:50:48.000000 deampy-1.3.9/deampy/plots/sample_paths.py
+-rw-rw-rw-   0        0        0    42089 2023-11-14 02:10:47.000000 deampy-1.3.9/deampy/random_variates.py
+-rw-rw-rw-   0        0        0    16282 2023-09-20 19:39:29.000000 deampy-1.3.9/deampy/regression_models.py
+-rw-rw-rw-   0        0        0     9436 2023-09-20 19:39:29.000000 deampy-1.3.9/deampy/sample_path.py
+-rw-rw-rw-   0        0        0     6676 2023-09-20 19:39:29.000000 deampy-1.3.9/deampy/sensitivity_analysis.py
+-rw-rw-rw-   0        0        0    47843 2024-04-02 18:56:41.000000 deampy-1.3.9/deampy/statistics.py
+drwxrwxrwx   0        0        0        0 2024-04-02 18:57:20.522708 deampy-1.3.9/deampy/support/
+-rw-rw-rw-   0        0        0        0 2023-09-20 19:39:30.000000 deampy-1.3.9/deampy/support/__init__.py
+-rw-rw-rw-   0        0        0    10009 2023-09-20 19:39:30.000000 deampy-1.3.9/deampy/support/econ_eval_support.py
+-rw-rw-rw-   0        0        0      659 2023-09-20 19:39:30.000000 deampy-1.3.9/deampy/support/misc_classes.py
+-rw-rw-rw-   0        0        0     7094 2023-09-20 19:39:30.000000 deampy-1.3.9/deampy/support/misc_functions.py
+-rw-rw-rw-   0        0        0     6635 2023-09-20 19:39:30.000000 deampy-1.3.9/deampy/support/simulation.py
+drwxrwxrwx   0        0        0        0 2024-04-02 18:57:20.525699 deampy-1.3.9/deampy.egg-info/
+-rw-rw-rw-   0        0        0      477 2024-04-02 18:57:20.000000 deampy-1.3.9/deampy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1135 2024-04-02 18:57:20.000000 deampy-1.3.9/deampy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 18:57:20.000000 deampy-1.3.9/deampy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-04-02 18:57:20.000000 deampy-1.3.9/deampy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-02 18:57:20.000000 deampy-1.3.9/deampy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-02 18:57:20.529688 deampy-1.3.9/setup.cfg
+-rw-rw-rw-   0        0        0      706 2024-04-02 18:56:58.000000 deampy-1.3.9/setup.py
```

### Comparing `deampy-1.3.8/LICENSE` & `deampy-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `deampy-1.3.8/deampy/data_structure.py` & `deampy-1.3.9/deampy/data_structure.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.8/deampy/decision_tree.py` & `deampy-1.3.9/deampy/decision_tree.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.8/deampy/discrete_event_sim.py` & `deampy-1.3.9/deampy/discrete_event_sim.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.8/deampy/econ_eval.py` & `deampy-1.3.9/deampy/econ_eval.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.8/deampy/format_functions.py` & `deampy-1.3.9/deampy/format_functions.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.8/deampy/in_out_functions.py` & `deampy-1.3.9/deampy/in_out_functions.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.8/deampy/markov.py` & `deampy-1.3.9/deampy/markov.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.8/deampy/models.py` & `deampy-1.3.9/deampy/models.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.8/deampy/optimization/appx_policy_itr.py` & `deampy-1.3.9/deampy/optimization/appx_policy_itr.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.8/deampy/optimization/learning_exploring_rules.py` & `deampy-1.3.9/deampy/optimization/learning_exploring_rules.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.8/deampy/optimization/stoch_approx.py` & `deampy-1.3.9/deampy/optimization/stoch_approx.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.8/deampy/parameter_estimation.py` & `deampy-1.3.9/deampy/parameter_estimation.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.8/deampy/parameters.py` & `deampy-1.3.9/deampy/parameters.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.8/deampy/plots/econ_eval_plots.py` & `deampy-1.3.9/deampy/plots/econ_eval_plots.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.8/deampy/plots/eff_sample_size.py` & `deampy-1.3.9/deampy/plots/eff_sample_size.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.8/deampy/plots/histogram.py` & `deampy-1.3.9/deampy/plots/histogram.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.8/deampy/plots/plot_support.py` & `deampy-1.3.9/deampy/plots/plot_support.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.8/deampy/plots/pop_pyramids.py` & `deampy-1.3.9/deampy/plots/pop_pyramids.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.8/deampy/plots/prob_dists.py` & `deampy-1.3.9/deampy/plots/prob_dists.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.8/deampy/plots/sample_paths.py` & `deampy-1.3.9/deampy/plots/sample_paths.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.8/deampy/random_variates.py` & `deampy-1.3.9/deampy/random_variates.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.8/deampy/regression_models.py` & `deampy-1.3.9/deampy/regression_models.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.8/deampy/sample_path.py` & `deampy-1.3.9/deampy/sample_path.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.8/deampy/sensitivity_analysis.py` & `deampy-1.3.9/deampy/sensitivity_analysis.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.8/deampy/statistics.py` & `deampy-1.3.9/deampy/statistics.py`

 * *Files 24% similar despite different names*

```diff
@@ -53,15 +53,15 @@
                  [z21, z22, ..., z2n],  # values of second controlling variable
                  ...
                 ]
     :return: partial correlation between x and y given the set of controlling variables z
     """
 
     np_z = np.array(z).T
-    
+
     Z = sm.add_constant(np_z)
     # fit f(z) to x
     fitted_xz = sm.OLS(x, Z).fit()
     # fit f(z) to y
     fitted_yz = sm.OLS(y, Z).fit()
     # residuals f(z) - x
     x_residuals = fitted_xz.predict() - x
@@ -71,38 +71,33 @@
     coef, p = pearsonr(x_residuals, y_residuals)
     return coef, p
 
 
 class _Statistics(object):
     def __init__(self, name=None):
         """ abstract method to be overridden in derived classes"""
-        self.name = name        # name of this statistics
-        self._n = 0              # number of data points
-        self._mean = 0           # sample mean
-        self._stDev = 0          # sample standard deviation
+        self.name = name  # name of this statistics
+        self._n = 0  # number of data points
+        self._mean = 0  # sample mean
+        self._stDev = 0  # sample standard deviation
         self._max = -sys.float_info.max  # maximum
-        self._min = sys.float_info.max   # minimum
-
-    def get_n(self):
-        """ abstract method to be overridden in derived classes
-        :returns mean (to be calculated in the subclass) """
-        raise NotImplementedError("This is an abstract method and needs to be implemented in derived classes.")
+        self._min = sys.float_info.max  # minimum
 
     def get_mean(self):
         """ abstract method to be overridden in derived classes
         :returns mean (to be calculated in the subclass) """
         raise NotImplementedError("This is an abstract method and needs to be implemented in derived classes.")
 
     def get_stdev(self):
         """ abstract method to be overridden in derived classes
         :returns standard deviation (to be calculated in the subclass) """
         raise NotImplementedError("This is an abstract method and needs to be implemented in derived classes.")
 
     def get_var(self):
-        return self.get_stdev()**2
+        return self.get_stdev() ** 2
 
     def get_min(self):
         """ abstract method to be overridden in derived classes
         :returns minimum (to be calculated in the subclass) """
         raise NotImplementedError("This is an abstract method and needs to be implemented in derived classes.")
 
     def get_max(self):
@@ -118,15 +113,15 @@
 
     def get_t_half_length(self, alpha):
         """
         :param alpha: significance level (between 0 and 1)
         :returns half-length of 100(1-alpha)% t-confidence interval """
 
         if self._n > 1:
-            return stat.t.ppf(1 - alpha / 2, self.get_n() - 1) * self.get_stdev() / np.sqrt(self.get_n())
+            return stat.t.ppf(1 - alpha / 2, self._n - 1) * self.get_stdev() / np.sqrt(self._n)
         else:
             return math.nan
 
     def get_t_CI(self, alpha):
         """ calculates t-based confidence interval for population mean
         :param alpha: significance level (between 0 and 1)
         :return: a list [l, u]
@@ -147,15 +142,15 @@
 
         # observations should be either 0 or 1
         for d in data:
             if d not in (0, 1):
                 raise ValueError('Wilson score interval can only be calculated for binary (0 or 1) outcomes.')
         return proportion_confint(count=sum(data), nobs=self._n, alpha=alpha, method='wilson')
 
-    def get_bootstrap_CI(self, alpha, num_samples):
+    def get_bootstrap_CI(self, alpha, num_samples=None):
         """ calculates empirical bootstrap confidence interval (abstract method to be overridden in derived classes)
         :param alpha: significance level
         :param num_samples: number of bootstrap samples
         :returns a list [L, U] """
         raise NotImplementedError("This is an abstract method and needs to be implemented in derived classes.")
 
     def get_PI(self, alpha):
@@ -175,29 +170,31 @@
                 F.format_number(self.get_mean(), digits),
                 F.format_interval(self.get_t_CI(alpha), digits),
                 F.format_interval(self.get_PI(alpha), digits),
                 F.format_number(self.get_stdev(), digits),
                 F.format_number(self.get_min(), digits),
                 F.format_number(self.get_max(), digits)]
 
-    def get_interval(self, interval_type='c', alpha=0.05, multiplier=1):
+    def get_interval(self, interval_type='c', alpha=0.05, multiplier=1, num_of_bootstrap_samples=None):
         """
         :param interval_type: (string) 'c' for t-based confidence interval,
                                        'cb' for bootstrap confidence interval,
                                        'p' for percentile interval, and
                                        'w' for Wilson score interval (only for binary outcomes)
         :param alpha: significance level
         :param multiplier: to multiply the estimate and the interval by the provided value
         :return: a list [L, U]
         """
 
         if interval_type == 'c':
             interval = self.get_t_CI(alpha)
         elif interval_type == 'cb':
-            interval = self.get_bootstrap_CI(alpha, NUM_BOOTSTRAP_SAMPLES)
+            if num_of_bootstrap_samples is None:
+                num_of_bootstrap_samples = NUM_BOOTSTRAP_SAMPLES
+            interval = self.get_bootstrap_CI(alpha, num_of_bootstrap_samples)
         elif interval_type == 'p':
             interval = self.get_PI(alpha)
         elif interval_type == 'w':
             if isinstance(self, SummaryStat) or isinstance(self, DifferenceStatPaired):
                 interval = self.get_proportion_CI(alpha)
             else:
                 raise ValueError(
@@ -206,15 +203,15 @@
             interval = None
         else:
             raise ValueError('Invalid interval type.')
         if interval is not None:
             if multiplier > 0:
                 return [v * multiplier for v in interval]
             else:
-                return [interval[1]*multiplier, interval[0]*multiplier]
+                return [interval[1] * multiplier, interval[0] * multiplier]
         else:
             return None
 
     def get_formatted_mean_and_interval(self, interval_type='c',
                                         alpha=0.05, deci=None, sig_digits=None, form=None, multiplier=1):
         """
         :param interval_type: (string) 'c' for t-based confidence interval,
@@ -224,15 +221,15 @@
         :param deci: digits to round the numbers to
         :param sig_digits: number of significant digits
         :param form: ',' to format as number, '%' to format as percentage, and '$' to format as currency
         :param multiplier: to multiply the estimate and the interval by the provided value
         :return: (string) estimate and interval formatted as specified
         """
 
-        estimate = self.get_mean()*multiplier
+        estimate = self.get_mean() * multiplier
         interval = self.get_interval(interval_type=interval_type, alpha=alpha, multiplier=multiplier)
 
         return F.format_estimate_interval(estimate=estimate,
                                           interval=interval,
                                           deci=deci,
                                           sig_digits=sig_digits,
                                           format=form)
@@ -279,17 +276,14 @@
         self._total = np.sum(self._data)
         self._mean = np.mean(self._data)
         if self._n > 1:
             self._stDev = np.std(self._data, ddof=1)  # unbiased estimator of the standard deviation
         else:
             self._stDev = math.nan
 
-    def get_n(self):
-        return self._n
-
     def get_total(self):
         return self._total
 
     def get_mean(self):
         return self._mean
 
     def get_stdev(self):
@@ -304,21 +298,24 @@
     def get_percentile(self, q):
         """
         :param q: percentile to compute (q in range [0, 100])
         :returns: qth percentile """
 
         return np.percentile(self._data, q)
 
-    def get_bootstrap_CI(self, alpha, num_samples):
+    def get_bootstrap_CI(self, alpha, num_samples=None):
         """ calculates the empirical bootstrap confidence interval
         :param alpha: significance level (between 0 and 1)
         :param num_samples: number of bootstrap samples
         :return: a list [l, u]
         """
 
+        if num_samples is None:
+            num_samples = NUM_BOOTSTRAP_SAMPLES
+
         # set random number generator seed
         rng = np.random.RandomState(1)
 
         # initialize delta array
         delta = np.zeros(num_samples)
 
         # obtain bootstrap samples
@@ -338,15 +335,15 @@
         return self._get_proportion_CI(data=self._data, alpha=alpha)
 
     def get_PI(self, alpha=0.05):
         """
         :param alpha: significance level (between 0 and 1)
         :return: percentile interval in the format of list [l, u]
         """
-        return [self.get_percentile(100*alpha/2), self.get_percentile(100*(1-alpha/2))]
+        return [self.get_percentile(100 * alpha / 2), self.get_percentile(100 * (1 - alpha / 2))]
 
     @staticmethod
     def get_array_from_formatted_interval(interval):
         """
         :param interval: (string) of form '[a, b]'
         :return: (np.array) [a, b]
         """
@@ -369,14 +366,15 @@
         array = np.array(formatted_text.split(' ')).astype(float)
 
         return array[0], array[1:]
 
 
 class DiscreteTimeStat(_Statistics):
     """ to calculate statistics on observations accumulating over time """
+
     def __init__(self, name=None):
         _Statistics.__init__(self, name)
         self._total = 0
         self._sumSquared = 0
 
     def record(self, obs):
         """ gets the next observation and update the current information"""
@@ -384,28 +382,25 @@
         self._sumSquared += obs ** 2
         self._n += 1
         if obs > self._max:
             self._max = obs
         if obs < self._min:
             self._min = obs
 
-    def get_n(self):
-        return self._n
-
     def get_total(self):
         return self._total
 
     def get_mean(self):
         if self._n > 0:
             return self._total / self._n
         else:
             return 0
 
     def get_stdev(self):
-        if self._n>1:
+        if self._n > 1:
             return math.sqrt(
                 (self._sumSquared - self._total ** 2 / self._n)
                 / (self._n - 1)
             )
         else:
             return 0
 
@@ -415,25 +410,26 @@
     def get_max(self):
         return self._max
 
     def get_percentile(self, q):
         """ percentiles cannot be calculated for this statistics """
         return None
 
-    def get_bootstrap_CI(self, alpha, num_samples):
+    def get_bootstrap_CI(self, alpha, num_samples=None):
         """ bootstrap confidence intervals cannot be calculated for this statistics """
         return None
 
     def get_PI(self, alpha):
         """ percentile intervals cannot be calculated for this statistics """
         return None
 
 
 class ContinuousTimeStat(_Statistics):
     """ to calculate statistics on the area-under-the-curve for observations accumulating over time """
+
     def __init__(self, initial_time, ave_method='step', name=None):
         """
         :param initial_time: it is assumed that the value of this sample path is zero at the initial time
         :param ave_method: to calculate the area under the curve,
             'step' assumes that changes occurred at the time where observations are recorded,
             'linear' assumes uses trapezoid approach to calculate the area under the curve
                     (v2 + v2 ) * deltaT / 2
@@ -470,23 +466,20 @@
             self._min = self._lastObsValue
 
         self._n += 1
         if self._aveMethod == 'step':
             self._area += self._lastObsValue * (time - self._lastObsTime)
             self._areaSquared += (self._lastObsValue ** 2) * (time - self._lastObsTime)
         else:
-            self._area += (self._lastObsValue + increment/2) * (time - self._lastObsTime)
-            self._areaSquared += ((self._lastObsValue + increment/2) ** 2) * (time - self._lastObsTime)
+            self._area += (self._lastObsValue + increment / 2) * (time - self._lastObsTime)
+            self._areaSquared += ((self._lastObsValue + increment / 2) ** 2) * (time - self._lastObsTime)
 
         self._lastObsTime = time
         self._lastObsValue += increment
 
-    def get_n(self):
-        return self._n
-
     def get_mean(self):
         if self._lastObsTime - self._initialTime > 0:
             return self._area / (self._lastObsTime - self._initialTime)
         else:
             return 0
 
     def get_stdev(self):
@@ -502,15 +495,15 @@
     def get_max(self):
         return self._max
 
     def get_percentile(self, q):
         """ percentiles cannot be calculated for this statistics """
         return None
 
-    def get_bootstrap_CI(self, alpha, num_samples):
+    def get_bootstrap_CI(self, alpha, num_samples=None):
         """ bootstrap confidence intervals cannot be calculated for this statistics """
         return None
 
     def get_PI(self, alpha):
         """ percentile intervals cannot be calculated for this statistics """
         return None
 
@@ -519,35 +512,35 @@
     def __init__(self, x, y_ref, name=None):
         """
         :param x: list or numpy.array of first set of observations
         :param y_ref: list or numpy.array of second set of observations (the reference) 
         """
         _Statistics.__init__(self, name)
 
-        if type(x) == list:
+        if isinstance(x, list):
             self._x = np.array(x)
-        elif type(x) == np.ndarray:
+        elif isinstance(x, np.ndarray):
             self._x = x
         else:
             raise ValueError("The argument x can be either a list of numbers or a numpy.array.")
 
-        if type(y_ref) == list:
+        if isinstance(y_ref, list):
             self._y_ref = np.array(y_ref)
-        elif type(y_ref) == np.ndarray:
+        elif isinstance(y_ref, np.ndarray):
             self._y_ref = y_ref
         else:
             raise ValueError("The argument y_ref can be either a list of numbers or a numpy.array.")
 
         if len(self._x) == 0:
             raise ValueError("x is empty for the comparative statistics '" + name + "'.")
         if len(self._y_ref) == 0:
             raise ValueError("y_ref is empty for the comparative statistics '" + name + "'.")
 
-        self._x_n = len(self._x)        # number of observations for x
-        self._y_n = len(self._y_ref)    # number of observations for y_ref
+        self._x_n = len(self._x)  # number of observations for x
+        self._y_n = len(self._y_ref)  # number of observations for y_ref
 
 
 class _DifferenceStat(_ComparativeStat):
 
     def __init__(self, x, y_ref, name=None):
         """
         :param x: list or numpy.array of first set of observations
@@ -559,25 +552,22 @@
 class DifferenceStatPaired(_DifferenceStat):
 
     def __init__(self, x, y_ref, name=None):
         """
         :param x: list or numpy.array of first set of observations
         :param y_ref: list or numpy.array of second set of observations
         """
-        _DifferenceStat.__init__(self,  x, y_ref, name)
+        _DifferenceStat.__init__(self, x, y_ref, name)
         # create a summary statistics for the element-wise difference
 
         if len(self._x) != len(self._y_ref):
             raise ValueError('Two samples (x and y_ref) should have the same size.')
 
         self._dStat = SummaryStat(self._x - self._y_ref, name)
 
-    def get_n(self):
-        return self._dStat.get_n()
-
     def get_mean(self):
         return self._dStat.get_mean()
 
     def get_stdev(self):
         return self._dStat.get_stdev()
 
     def get_min(self):
@@ -588,15 +578,15 @@
 
     def get_percentile(self, q):
         return self._dStat.get_percentile(q)
 
     def get_t_CI(self, alpha):
         return self._dStat.get_t_CI(alpha)
 
-    def get_bootstrap_CI(self, alpha, num_samples):
+    def get_bootstrap_CI(self, alpha, num_samples=None):
         return self._dStat.get_bootstrap_CI(alpha, num_samples)
 
     def get_proportion_CI(self, alpha=0.05):
         return self._get_proportion_CI(data=self._x - self._y_ref, alpha=alpha)
 
     def get_PI(self, alpha):
         return self._dStat.get_PI(alpha)
@@ -712,15 +702,15 @@
                + (sig_y ** 2.0 / self._y_n) ** 2 / (self._y_n - 1)
         df = round(df_n / df_d, 0)
 
         # t distribution quantile
         t_q = stat.t.ppf(1 - (alpha / 2), df)
         st_dev = (sig_x ** 2.0 / self._x_n + sig_y ** 2.0 / self._y_n) ** 0.5
 
-        return t_q*st_dev
+        return t_q * st_dev
 
     def get_t_CI(self, alpha):
 
         interval = self.get_t_half_length(alpha)
         diff = np.mean(self._x) - np.mean(self._y_ref)
 
         return [diff - interval, diff + interval]
@@ -754,32 +744,29 @@
         """
         _RatioStat.__init__(self, x, y_ref, name)
 
         if len(self._x) != len(self._y_ref):
             raise ValueError('Two samples (x and y_ref) should have the same size.')
 
         # add element-wise ratio
-        ratio = np.zeros(len(self._x))
+        self.ratios = np.zeros(len(self._x))
         for i in range(len(self._x)):
             # for 0 in the denominator variable, check whether numerator is also 0
             if self._y_ref[i] == 0:
-                ratio[i] = math.nan
+                self.ratios[i] = math.nan
                 warnings.warn("For ratio statistics '{}', "
                               "the denominator of ratio with index {} is 0."
                               "The ratio is not computable.".format(name, i))
                 self._ifComputable = False
             else:
                 # for non-zero denominators, calculate ratio
-                ratio[i] = 1.0*self._x[i] / self._y_ref[i]
+                self.ratios[i] = 1.0 * self._x[i] / self._y_ref[i]
 
         # create summary stat for element-wise ratio
-        self._ratioStat = SummaryStat(ratio, name)
-
-    def get_n(self):
-        return self._ratioStat.get_n()
+        self._ratioStat = SummaryStat(self.ratios, name)
 
     def get_mean(self):
         if self._ifComputable:
             return self._ratioStat.get_mean()
         else:
             return math.nan
 
@@ -803,27 +790,98 @@
 
     def get_t_CI(self, alpha):
         if self._ifComputable:
             return self._ratioStat.get_t_CI(alpha)
         else:
             return math.nan
 
-    def get_bootstrap_CI(self, alpha, num_samples):
+    def get_bootstrap_CI(self, alpha, num_samples=None):
         if self._ifComputable:
             return self._ratioStat.get_bootstrap_CI(alpha, num_samples)
         else:
             return math.nan
 
     def get_PI(self, alpha):
         if self._ifComputable:
             return self._ratioStat.get_PI(alpha)
         else:
             return [math.nan, math.nan]
 
 
+class RatioOfMeansStatPaired(_RatioStat):
+
+    def __init__(self, x, y_ref, name=None):
+        """
+        :param x: list or numpy.array of first set of observations
+        :param y_ref: list or numpy.array of second set of observations
+        """
+        _RatioStat.__init__(self, x, y_ref, name)
+
+        if len(self._x) != len(self._y_ref):
+            raise ValueError('Two samples (x and y_ref) should have the same size.')
+
+        # add element-wise ratio
+        self.ratios = np.zeros(len(self._x))
+        for i in range(len(self._x)):
+            # for 0 in the denominator variable, check whether numerator is also 0
+            if self._y_ref[i] == 0:
+                self.ratios[i] = math.nan
+                warnings.warn("For ratio statistics '{}', "
+                              "the denominator of ratio with index {} is 0."
+                              "The confidence or prediction interval will not be computable.".format(name, i))
+                self._ifComputable = False
+            else:
+                # for non-zero denominators, calculate ratio
+                self.ratios[i] = 1.0 * self._x[i] / self._y_ref[i]
+
+    def get_mean(self):
+        return np.mean(self._x) / np.mean(self._y_ref)
+
+    def get_stdev(self):
+        return np.nan
+
+    def get_min(self):
+        return np.nan
+
+    def get_max(self):
+        return np.nan
+
+    def get_percentile(self, q):
+        return np.nan
+
+    def get_t_CI(self, alpha):
+        return [np.nan, np.nan]
+
+    def get_bootstrap_CI(self, alpha, num_samples=None):
+
+        if num_samples is None:
+            num_samples = NUM_BOOTSTRAP_SAMPLES
+
+        # set random number generator seed
+        rng = np.random.RandomState(1)
+
+        # initialize delta array
+        delta = np.zeros(num_samples)
+
+        mean = self.get_mean()
+
+        # obtain bootstrap samples
+        for i in range(num_samples):
+            i_s = rng.choice(range(len(self._x)), size=len(self._x), replace=True)
+            x_i = self._x[i_s]
+            y_i = self._y_ref[i_s]
+            delta[i] = np.mean(x_i) / np.mean(y_i) - mean
+
+        # return [l, u]
+        return mean - np.percentile(delta, [100 * (1 - alpha / 2.0), 100 * alpha / 2.0])
+
+    def get_PI(self, alpha):
+        return [np.nan, np.nan]
+
+
 class RatioStatIndp(_RatioStat):
 
     def __init__(self, x, y_ref, name=None):
         """
         :param x: list or numpy.array of first set of observations
         :param y_ref: list or numpy.array of second set of observations (reference)
 
@@ -856,15 +914,15 @@
 
     def get_mean(self):
         """
         for independent variable x and y, E(x/y) = E(x)*E(1/y)
         :return: E(x/y)
         """
 
-        return np.average(self._x)*np.average(1/self._y_ref)
+        return np.average(self._x) * np.average(1 / self._y_ref)
 
     def get_stdev(self):
         """
         for independent variable x and y, var(x/y) = E(x^2)*E(1/y^2)-E(x)^2*(E(1/y)^2)
         :return: std(x/y)
         """
         var = np.mean(self._x ** 2) * np.mean(1.0 / self._y_ref ** 2) - \
@@ -923,66 +981,114 @@
         # if self._x_n > 1 and self._y_n > 1:
         #     mean = self.get_mean()
         #     hl = self.get_t_half_length(alpha)
         #     return [mean - hl, mean + hl]
         # else:
         #     return [math.nan, math.nan]
 
-    def get_bootstrap_CI(self, alpha, num_samples):
+    def get_bootstrap_CI(self, alpha, num_samples=None):
         """
         :param alpha: confidence level
         :param num_samples: number of samples
         :return: empirical bootstrap confidence interval
         """
 
+        if num_samples is None:
+            num_samples = NUM_BOOTSTRAP_SAMPLES
+
         # set random number generator seed
         rng = np.random.RandomState(1)
 
         # initialize delta array
         delta = np.zeros(num_samples)
 
         # obtain bootstrap samples
         n = max(self._x_n, self._y_n)
         mean = self.get_mean()
         for i in range(num_samples):
             x_i = rng.choice(self._x, size=n, replace=True)
             y_i = rng.choice(self._y_ref, size=n, replace=True)
-            ratios_i = np.divide(x_i, y_i)
-            delta[i] = np.mean(ratios_i) - mean
+            ratios_i = np.average(x_i) * np.average(1 / y_i)
+            delta[i] = ratios_i - mean
 
         # return [l, u]
         return mean - np.percentile(delta, [100 * (1 - alpha / 2.0), 100 * alpha / 2.0])
 
-        # # set random number generator seed
-        # rng = np.random.RandomState(1)
-        #
-        # # initialize ratio array
-        # ratio = np.zeros(num_samples)
-        #
-        # # obtain bootstrap samples
-        # n = max(self._x_n, self._y_n)
-        # for i in range(num_samples):
-        #     x_i = rng.choice(self._x, size=n, replace=True)
-        #     y_i = rng.choice(self._y_ref, size=n, replace=True)
-        #     r_temp = np.divide(x_i, y_i)
-        #     ratio[i] = np.mean(r_temp)
-        #
-        # return np.percentile(ratio, [100 * alpha / 2.0, 100 * (1 - alpha / 2.0)])
-
     def get_PI(self, alpha):
 
         if not self._XOverYSimulated:
             self._simulate_x_over_y()
 
         if self._ifComputable:
             return self._sum_stat_sample_ratio.get_PI(alpha)
         else:
             return [math.nan, math.nan]
 
 
+class RatioOfMeansStatIndp(_RatioStat):
+
+    def __init__(self, x, y_ref, name=None):
+        """
+        :param x: list or numpy.array of first set of observations
+        :param y_ref: list or numpy.array of second set of observations
+        """
+        _RatioStat.__init__(self, x, y_ref, name)
+
+    def get_mean(self):
+        """
+        :return: the ratio of the means of x and y_ref"""
+        return np.mean(self._x) / np.mean(self._y_ref)
+
+    def get_stdev(self):
+        return np.nan
+
+    def get_min(self):
+        return np.nan
+
+    def get_max(self):
+        return np.nan
+
+    def get_percentile(self, q):
+        return np.nan
+
+    def get_t_CI(self, alpha):
+        return [np.nan, np.nan]
+
+    def get_bootstrap_CI(self, alpha, num_samples=None):
+        """
+         :param alpha: confidence level
+         :param num_samples: number of samples
+         :return: empirical bootstrap confidence interval
+         """
+
+        if num_samples is None:
+            num_samples = NUM_BOOTSTRAP_SAMPLES
+
+        # set random number generator seed
+        rng = np.random.RandomState(1)
+
+        # initialize delta array
+        delta = np.zeros(num_samples)
+
+        # obtain bootstrap samples
+        n = max(self._x_n, self._y_n)
+        mean = self.get_mean()
+        for i in range(num_samples):
+            x_i = rng.choice(self._x, size=n, replace=True)
+            y_i = rng.choice(self._y_ref, size=n, replace=True)
+            ratios_i = np.average(x_i) / np.average(y_i)
+            delta[i] = ratios_i - mean
+
+        # return [l, u]
+        return mean - np.percentile(delta, [100 * (1 - alpha / 2.0), 100 * alpha / 2.0])
+
+    def get_PI(self, alpha):
+        return [np.nan, np.nan]
+
+
 class _RelativeDifference(_ComparativeStat):
     """ class to make inference about (X-Y_ref)/Y_ref or (Y_ref-X)/Y_ref"""
 
     def __init__(self, x, y_ref, order=0, name=None):
         """
         :param x: list or numpy.array of first set of observations
         :param y_ref: list or numpy.array of second set of observations used as the reference values
@@ -1015,25 +1121,22 @@
                 ratio[i] = math.nan
                 warnings.warn("For ratio statistics '{}', "
                               "the denominator of ratio with index {} is 0."
                               "The ratio is not computable.".format(name, i))
                 self._ifComputable = False
             # for non-zero denominators, calculate ratio
             else:
-                ratio[i] = 1.0*self._x[i] / self._y_ref[i]
+                ratio[i] = 1.0 * self._x[i] / self._y_ref[i]
 
         # create summary stat for element-wise ratio
         if self._order == 0:
             self._relativeDiffStat = SummaryStat(ratio - 1, name)
         else:
             self._relativeDiffStat = SummaryStat(1 - ratio, name)
 
-    def get_n(self):
-        return self._relativeDiffStat.get_n()
-
     def get_mean(self):
         if self._ifComputable:
             return self._relativeDiffStat.get_mean()
         else:
             return math.nan
 
     def get_stdev(self):
@@ -1056,174 +1159,213 @@
 
     def get_t_CI(self, alpha):
         if self._ifComputable:
             return self._relativeDiffStat.get_t_CI(alpha)
         else:
             return [math.nan, math.nan]
 
-    def get_bootstrap_CI(self, alpha, num_samples):
+    def get_bootstrap_CI(self, alpha, num_samples=None):
+
+        if num_samples is None:
+            num_samples = NUM_BOOTSTRAP_SAMPLES
+
         if self._ifComputable:
             return self._relativeDiffStat.get_bootstrap_CI(alpha, num_samples)
         else:
             return [math.nan, math.nan]
 
     def get_PI(self, alpha):
         if self._ifComputable:
             return self._relativeDiffStat.get_PI(alpha)
         else:
             return [math.nan, math.nan]
 
 
-class RelativeDifferenceIndp(_RelativeDifference):
+class RelativeDiffOfMeansPaired(_RelativeDifference):
+
     def __init__(self, x, y_ref, order=0, name=None):
         """
         :param x: list or numpy.array of first set of observations
         :param y_ref: list or numpy.array of second set of observations
         :param order: set to 0 to calculate (X-Y_ref)/Y_ref and to 1 to calculate (Y_ref-X)/Y_ref
         """
         _RelativeDifference.__init__(self, x, y_ref, order, name)
 
-        self._XMinusYOverYSimulated = False
+        if len(self._x) != len(self._y_ref):
+            raise ValueError('Two samples should have the same size.')
 
-    def _simulate_x_minus_y_over_y(self):
+        self._ratioOfMeans = RatioOfMeansStatPaired(x, y_ref, name)
 
-        # generate random realizations for random variable (X-Y)/Y
-        rng = np.random.RandomState(1)
-        # find the maximum of the number of observations
-        max_n = max(self._x_n, self._y_n, NUM_BOOTSTRAP_SAMPLES)
-        x_resample = rng.choice(self._x, size=max_n, replace=True)
-        y_resample = rng.choice(self._y_ref, size=max_n, replace=True)
+    def get_mean(self):
+        if self._order == 0:
+            return self._ratioOfMeans.get_mean() - 1
+        else:
+            return 1 - self._ratioOfMeans.get_mean()
 
-        self._XMinusYOverYSimulated = True
-        self._ifComputable = True
+    def get_stdev(self):
+        return np.nan
+
+    def get_min(self):
+        return np.nan
+
+    def get_max(self):
+        return np.nan
+
+    def get_percentile(self, q):
+        return np.nan
+
+    def get_t_CI(self, alpha):
+        return [np.nan, np.nan]
+
+    def get_bootstrap_CI(self, alpha, num_samples=None):
+
+        interval = self._ratioOfMeans.get_bootstrap_CI(alpha, num_samples)
         if self._order == 0:
-            try:
-                self._sum_stat_sample_relativeRatio = SummaryStat(
-                    np.divide(x_resample-y_resample, y_resample), self.name)
-            except ZeroDivisionError:
-                warnings.warn("For ratio statistics '{}', "
-                              "one element of y_ref is 0.".format(self.name))
-                self._ifComputable = False
+            return [interval[0] - 1, interval[1] - 1]
         else:
-            try:
-                self._sum_stat_sample_relativeRatio = SummaryStat(
-                    np.divide(y_resample-x_resample, y_resample), self.name)
-            except ZeroDivisionError:
-                warnings.warn("For ratio statistics '{}', "
-                              "one element of y_ref is 0.".format(self.name))
-                self._ifComputable = False
+            return [1 - interval[1], 1 - interval[0]]
+
+    def get_PI(self, alpha):
+        return [np.nan, np.nan]
+
+
+class RelativeDifferenceIndp(_RelativeDifference):
+    def __init__(self, x, y_ref, order=0, name=None):
+        """
+        :param x: list or numpy.array of first set of observations
+        :param y_ref: list or numpy.array of second set of observations
+        :param order: set to 0 to calculate (X-Y_ref)/Y_ref and to 1 to calculate (Y_ref-X)/Y_ref
+        """
+        _RelativeDifference.__init__(self, x, y_ref, order, name)
+
+        self._ratioStat = RatioStatIndp(x, y_ref, name)
 
     def get_mean(self):
         """
         for independent variable x and y, E((x-y)/y) = E(x)*E(1/y) - 1
         :return: E((x-y)/y) or E((y-x)/y)
         """
         if self._order == 0:
-            return np.average(self._x) * np.average(1 / self._y_ref) - 1
+            return self._ratioStat.get_mean() - 1
         else:
-            return 1 - np.average(self._x) * np.average(1 / self._y_ref)
+            return 1 - self._ratioStat.get_mean()
 
     def get_stdev(self):
         """
         for independent variable x and y, var(x/y) = E(x^2)*E(1/y^2)-E(x)^2*(E(1/y)^2)
         and var(x/y - 1) = var(x/y)
         :return: std(x/y - 1)
         """
-        if self._ifComputable:
-            var = np.mean(self._x ** 2) * np.mean(1.0 / self._y_ref ** 2) - \
-                  (np.mean(self._x) ** 2) * (np.mean(1.0 / self._y_ref) ** 2)
-            return np.sqrt(var)
-        else:
-            return math.nan
+        return self._ratioStat.get_stdev()
 
     def get_min(self):
 
-        if not self._XMinusYOverYSimulated:
-            self._simulate_x_minus_y_over_y()
-        if self._ifComputable:
-            return self._sum_stat_sample_relativeRatio.get_min()
+        if self._order == 0:
+            return self._ratioStat.get_min() - 1
         else:
-            return math.nan
+            return 1 - self._ratioStat.get_max()
 
     def get_max(self):
 
-        if not self._XMinusYOverYSimulated:
-            self._simulate_x_minus_y_over_y()
-        if self._ifComputable:
-            return self._sum_stat_sample_relativeRatio.get_max()
+        if self._order == 0:
+            return self._ratioStat.get_max() - 1
         else:
-            return math.nan
+            return 1 - self._ratioStat.get_min()
 
     def get_percentile(self, q):
         """
         for independent variable x and y, percentiles are given after re-sampling
         :param q: the percentile want to return, in [0,100]
         :return: qth percentile of sample (x-y)/y
         """
 
-        if not self._XMinusYOverYSimulated:
-            self._simulate_x_minus_y_over_y()
-        if self._ifComputable:
-            return self._sum_stat_sample_relativeRatio.get_percentile(q)
+        if self._order == 0:
+            return self._ratioStat.get_percentile(q) - 1
         else:
-            return [math.nan, math.nan]
+            return 1 - self._ratioStat.get_percentile(100 - q)
 
     def get_t_half_length(self, alpha):
         """ cannot be calculated for ratio statistics """
 
         return math.nan
 
-        # if not self._XMinusYOverYSimulated:
-        #     self._simulate_x_minus_y_over_y()
-        # if self._ifComputable:
-        #     return self._sum_stat_sample_relativeRatio.get_t_half_length(alpha)
-        # else:
-        #     return math.nan
-
     def get_t_CI(self, alpha):
         """ cannot be calculated for ratio statistics """
 
         return [math.nan, math.nan]
 
-        # if self._x_n > 1 and self._y_n>1:
-        #     mean = self.get_mean()
-        #     hl = self.get_t_half_length(alpha)
-        #     return [mean - hl, mean + hl]
-        # else:
-        #     return [math.nan, math.nan]
-
-    def get_bootstrap_CI(self, alpha, num_samples):
+    def get_bootstrap_CI(self, alpha, num_samples=None):
         """
         :param alpha: confidence level
         :param num_samples: number of samples
         :return: empirical bootstrap confidence interval
         """
 
-        # set random number generator seed
-        rng = np.random.RandomState(1)
+        if num_samples is None:
+            num_samples = NUM_BOOTSTRAP_SAMPLES
 
-        # initialize ratio array
-        delta = np.zeros(num_samples)
+        interval = self._ratioStat.get_bootstrap_CI(alpha, num_samples)
 
-        # obtain bootstrap samples
-        n = max(self._x_n, self._y_n)
-        mean = self.get_mean()
-        for i in range(num_samples):
-            x_i = rng.choice(self._x, size=n, replace=True)
-            y_i = rng.choice(self._y_ref, size=n, replace=True)
-            if self._order == 0:
-                ratios_i = np.divide(x_i, y_i) - 1
-            else:
-                ratios_i = 1 - np.divide(x_i, y_i)
-            delta[i] = np.mean(ratios_i) - mean
-
-        return mean - np.percentile(delta, [100 * (1 - alpha / 2.0), 100 * alpha / 2.0])
-        # return np.percentile(ratio, [100 * alpha / 2.0, 100 * (1 - alpha / 2.0)])
+        if self._order == 0:
+            return [interval[0] - 1, interval[0] - 1]
+        else:
+            return [1 - interval[1], 1 - interval[0]]
 
     def get_PI(self, alpha):
 
-        if not self._XMinusYOverYSimulated:
-            self._simulate_x_minus_y_over_y()
-        if self._ifComputable:
-            return self._sum_stat_sample_relativeRatio.get_PI(alpha)
+        interval = self._ratioStat.get_PI(alpha)
+        if self._order == 0:
+            return [interval[0] - 1, interval[1] - 1]
         else:
-            return [math.nan, math.nan]
+            return [1 - interval[1], 1 - interval[0]]
+
+
+class RelativeDiffOfMeansIndp(_RelativeDifference):
+
+    def __init__(self, x, y_ref, order=0, name=None):
+        """
+        :param x: list or numpy.array of first set of observations
+        :param y_ref: list or numpy.array of second set of observations
+        :param order: set to 0 to calculate (X-Y_ref)/Y_ref and to 1 to calculate (Y_ref-X)/Y_ref
+        """
+        _RelativeDifference.__init__(self, x, y_ref, order, name)
+
+        self._ratioOfMeans = RatioOfMeansStatIndp(x, y_ref, name)
+
+    def get_mean(self):
+        """
+        :return: the relative difference of means of x and y_ref"""
+        if self._order == 0:
+            return self._ratioOfMeans.get_mean() - 1
+        else:
+            return 1 - self._ratioOfMeans.get_mean()
+
+    def get_stdev(self):
+        return np.nan
+
+    def get_min(self):
+        return np.nan
+
+    def get_max(self):
+        return np.nan
+
+    def get_percentile(self, q):
+        return np.nan
+
+    def get_t_CI(self, alpha):
+        return [np.nan, np.nan]
+
+    def get_bootstrap_CI(self, alpha, num_samples=None):
+        """
+         :param alpha: confidence level
+         :param num_samples: number of samples
+         :return: empirical bootstrap confidence interval
+         """
+
+        interval = self._ratioOfMeans.get_bootstrap_CI(alpha, num_samples)
+        if self._order == 0:
+            return [interval[0] - 1, interval[1] - 1]
+        else:
+            return [1 - interval[1], 1 - interval[0]]
+
+    def get_PI(self, alpha):
+        return [np.nan, np.nan]
```

### Comparing `deampy-1.3.8/deampy/support/econ_eval_support.py` & `deampy-1.3.9/deampy/support/econ_eval_support.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.8/deampy/support/misc_classes.py` & `deampy-1.3.9/deampy/support/misc_classes.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.8/deampy/support/misc_functions.py` & `deampy-1.3.9/deampy/support/misc_functions.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.8/deampy/support/simulation.py` & `deampy-1.3.9/deampy/support/simulation.py`

 * *Files identical despite different names*

### Comparing `deampy-1.3.8/deampy.egg-info/SOURCES.txt` & `deampy-1.3.9/deampy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deampy-1.3.8/setup.py` & `deampy-1.3.9/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 # read the contents of your README file
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='deampy',
-    version='1.3.8',
+    version='1.3.9',
     install_requires=['numpy', 'matplotlib', 'scipy', 'statsmodels', 'scikit-learn'],
     packages=['deampy', 'deampy.optimization', 'deampy.plots', 'deampy.support'],
     url='https://github.com/modeling-health-care-decisions/deampy',
     license='MIT License',
     author='Reza Yaesoubi',
     author_email='reza.yaesoubi@yale.edu',
     description='Decision analysis in medicine and public health',
```

