# Comparing `tmp/mixician-0.1.8.tar.gz` & `tmp/mixician-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mixician-0.1.8.tar", max compression
+gzip compressed data, was "mixician-0.1.9.tar", max compression
```

## Comparing `mixician-0.1.8.tar` & `mixician-0.1.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1066 2024-02-06 16:06:54.432243 mixician-0.1.8/LICENSE
--rw-r--r--   0        0        0      680 2024-03-01 16:02:26.037264 mixician-0.1.8/README.md
--rw-r--r--   0        0        0     1103 2024-03-17 11:32:59.368328 mixician-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      160 2024-03-01 13:24:23.435804 mixician-0.1.8/src/mixician/__init__.py
--rw-r--r--   0        0        0      386 2024-02-10 15:14:02.379150 mixician-0.1.8/src/mixician/balancers/__init__.py
--rw-r--r--   0        0        0     3280 2024-03-01 16:04:32.045270 mixician-0.1.8/src/mixician/balancers/balance_with_probs.py
--rw-r--r--   0        0        0     1983 2024-02-10 15:14:02.380054 mixician-0.1.8/src/mixician/balancers/base.py
--rw-r--r--   0        0        0     1239 2024-02-10 15:14:02.380441 mixician-0.1.8/src/mixician/balancers/compute_divergence.py
--rw-r--r--   0        0        0      529 2024-03-03 17:17:38.549190 mixician-0.1.8/src/mixician/calculators/__init__.py
--rw-r--r--   0        0        0     2431 2024-03-17 03:53:08.172177 mixician-0.1.8/src/mixician/calculators/base.py
--rw-r--r--   0        0        0     6205 2024-03-16 17:11:35.519006 mixician-0.1.8/src/mixician/calculators/calculate_with_components.py
--rw-r--r--   0        0        0     6394 2024-03-17 03:54:23.170091 mixician-0.1.8/src/mixician/calculators/calculate_with_self_balancing_components.py
--rw-r--r--   0        0        0      318 2024-03-01 10:48:41.506487 mixician-0.1.8/src/mixician/dataloaders/__init__.py
--rw-r--r--   0        0        0     3046 2024-03-15 15:46:26.560292 mixician-0.1.8/src/mixician/dataloaders/base.py
--rw-r--r--   0        0        0     1084 2024-03-01 16:04:32.028718 mixician-0.1.8/src/mixician/dataloaders/load_config.py
--rw-r--r--   0        0        0     2507 2024-03-01 16:04:32.040086 mixician-0.1.8/src/mixician/dataloaders/load_dataframe.py
--rw-r--r--   0        0        0     1041 2024-03-01 10:48:41.508066 mixician-0.1.8/src/mixician/dataloaders/set_path.py
--rw-r--r--   0        0        0       23 2024-03-01 10:48:41.508285 mixician-0.1.8/src/mixician/examples/__init__.py
--rw-r--r--   0        0        0      318 2024-03-15 13:43:10.951967 mixician-0.1.8/src/mixician/examples/calculate_value_based_ensemble_score/config_case_01.yml
--rw-r--r--   0        0        0      389 2024-03-15 13:38:43.482890 mixician-0.1.8/src/mixician/examples/calculate_value_based_ensemble_score/config_case_02.yml
--rw-r--r--   0        0        0      350 2024-03-17 06:56:44.744252 mixician-0.1.8/src/mixician/examples/calculate_value_based_ensemble_score/config_case_03.yml
--rw-r--r--   0        0        0   234012 2024-03-17 11:31:11.384662 mixician-0.1.8/src/mixician/examples/calculate_value_based_ensemble_score/optimize_parameters_with_paradance.ipynb
--rw-r--r--   0        0        0   139781 2024-03-15 11:20:35.696462 mixician-0.1.8/src/mixician/examples/calculate_value_based_ensemble_score/self_balancing_value_based_ensemble_score.ipynb
--rw-r--r--   0        0        0    99364 2024-03-04 02:24:41.337337 mixician-0.1.8/src/mixician/examples/calculate_value_based_ensemble_score/value_based_ensemble_score.ipynb
--rw-r--r--   0        0        0      328 2024-03-17 06:55:26.053262 mixician-0.1.8/src/mixician/examples/dataset/__init__.py
--rw-r--r--   0        0        0     5494 2024-03-17 06:55:31.932574 mixician-0.1.8/src/mixician/examples/dataset/utils.py
--rw-r--r--   0        0        0        0 2024-02-22 14:48:02.118917 mixician-0.1.8/src/mixician/optimization/__init__.py
--rw-r--r--   0        0        0       85 2024-03-01 16:04:32.027861 mixician-0.1.8/src/mixician/visualization/__init__.py
--rw-r--r--   0        0        0     3444 2024-03-17 06:55:26.768336 mixician-0.1.8/src/mixician/visualization/plot_distributions.py
--rw-r--r--   0        0        0     1813 1970-01-01 00:00:00.000000 mixician-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-02-06 16:06:54.432243 mixician-0.1.9/LICENSE
+-rw-r--r--   0        0        0      680 2024-03-01 16:02:26.037264 mixician-0.1.9/README.md
+-rw-r--r--   0        0        0     1103 2024-03-17 16:52:17.044994 mixician-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      160 2024-03-01 13:24:23.435804 mixician-0.1.9/src/mixician/__init__.py
+-rw-r--r--   0        0        0      386 2024-02-10 15:14:02.379150 mixician-0.1.9/src/mixician/balancers/__init__.py
+-rw-r--r--   0        0        0     3280 2024-03-01 16:04:32.045270 mixician-0.1.9/src/mixician/balancers/balance_with_probs.py
+-rw-r--r--   0        0        0     1983 2024-02-10 15:14:02.380054 mixician-0.1.9/src/mixician/balancers/base.py
+-rw-r--r--   0        0        0     1239 2024-02-10 15:14:02.380441 mixician-0.1.9/src/mixician/balancers/compute_divergence.py
+-rw-r--r--   0        0        0      529 2024-03-03 17:17:38.549190 mixician-0.1.9/src/mixician/calculators/__init__.py
+-rw-r--r--   0        0        0     2431 2024-03-17 03:53:08.172177 mixician-0.1.9/src/mixician/calculators/base.py
+-rw-r--r--   0        0        0     6205 2024-03-16 17:11:35.519006 mixician-0.1.9/src/mixician/calculators/calculate_with_components.py
+-rw-r--r--   0        0        0     6406 2024-03-17 12:38:24.200326 mixician-0.1.9/src/mixician/calculators/calculate_with_self_balancing_components.py
+-rw-r--r--   0        0        0      318 2024-03-01 10:48:41.506487 mixician-0.1.9/src/mixician/dataloaders/__init__.py
+-rw-r--r--   0        0        0     3046 2024-03-15 15:46:26.560292 mixician-0.1.9/src/mixician/dataloaders/base.py
+-rw-r--r--   0        0        0     1084 2024-03-01 16:04:32.028718 mixician-0.1.9/src/mixician/dataloaders/load_config.py
+-rw-r--r--   0        0        0     2507 2024-03-01 16:04:32.040086 mixician-0.1.9/src/mixician/dataloaders/load_dataframe.py
+-rw-r--r--   0        0        0     1041 2024-03-01 10:48:41.508066 mixician-0.1.9/src/mixician/dataloaders/set_path.py
+-rw-r--r--   0        0        0       23 2024-03-01 10:48:41.508285 mixician-0.1.9/src/mixician/examples/__init__.py
+-rw-r--r--   0        0        0      318 2024-03-15 13:43:10.951967 mixician-0.1.9/src/mixician/examples/calculate_value_based_ensemble_score/config_case_01.yml
+-rw-r--r--   0        0        0      389 2024-03-15 13:38:43.482890 mixician-0.1.9/src/mixician/examples/calculate_value_based_ensemble_score/config_case_02.yml
+-rw-r--r--   0        0        0      350 2024-03-17 06:56:44.744252 mixician-0.1.9/src/mixician/examples/calculate_value_based_ensemble_score/config_case_03.yml
+-rw-r--r--   0        0        0    85979 2024-03-17 12:41:55.866935 mixician-0.1.9/src/mixician/examples/calculate_value_based_ensemble_score/optimize_parameters_with_paradance.ipynb
+-rw-r--r--   0        0        0   139781 2024-03-15 11:20:35.696462 mixician-0.1.9/src/mixician/examples/calculate_value_based_ensemble_score/self_balancing_value_based_ensemble_score.ipynb
+-rw-r--r--   0        0        0    99364 2024-03-04 02:24:41.337337 mixician-0.1.9/src/mixician/examples/calculate_value_based_ensemble_score/value_based_ensemble_score.ipynb
+-rw-r--r--   0        0        0      328 2024-03-17 06:55:26.053262 mixician-0.1.9/src/mixician/examples/dataset/__init__.py
+-rw-r--r--   0        0        0     5494 2024-03-17 06:55:31.932574 mixician-0.1.9/src/mixician/examples/dataset/utils.py
+-rw-r--r--   0        0        0        0 2024-02-22 14:48:02.118917 mixician-0.1.9/src/mixician/optimization/__init__.py
+-rw-r--r--   0        0        0       85 2024-03-01 16:04:32.027861 mixician-0.1.9/src/mixician/visualization/__init__.py
+-rw-r--r--   0        0        0     3444 2024-03-17 06:55:26.768336 mixician-0.1.9/src/mixician/visualization/plot_distributions.py
+-rw-r--r--   0        0        0     1813 1970-01-01 00:00:00.000000 mixician-0.1.9/PKG-INFO
```

### Comparing `mixician-0.1.8/LICENSE` & `mixician-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mixician-0.1.8/README.md` & `mixician-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `mixician-0.1.8/pyproject.toml` & `mixician-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mixician"
-version = "0.1.8"
+version = "0.1.9"
 description = "An advanced hybrid ranking engine for recommendation systems, designed to automate the optimization of algorithms and parameters tailored to diverse business objectives."
 authors = ["Yin Cheng <yin.sjtu@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/yinsn/Mixician"
 repository = "https://github.com/yinsn/Mixician"
 packages = [{ include = "mixician", from = "src" }]
```

### Comparing `mixician-0.1.8/src/mixician/balancers/balance_with_probs.py` & `mixician-0.1.9/src/mixician/balancers/balance_with_probs.py`

 * *Files identical despite different names*

### Comparing `mixician-0.1.8/src/mixician/balancers/base.py` & `mixician-0.1.9/src/mixician/balancers/base.py`

 * *Files identical despite different names*

### Comparing `mixician-0.1.8/src/mixician/balancers/compute_divergence.py` & `mixician-0.1.9/src/mixician/balancers/compute_divergence.py`

 * *Files identical despite different names*

### Comparing `mixician-0.1.8/src/mixician/calculators/__init__.py` & `mixician-0.1.9/src/mixician/calculators/__init__.py`

 * *Files identical despite different names*

### Comparing `mixician-0.1.8/src/mixician/calculators/base.py` & `mixician-0.1.9/src/mixician/calculators/base.py`

 * *Files identical despite different names*

### Comparing `mixician-0.1.8/src/mixician/calculators/calculate_with_components.py` & `mixician-0.1.9/src/mixician/calculators/calculate_with_components.py`

 * *Files identical despite different names*

### Comparing `mixician-0.1.8/src/mixician/calculators/calculate_with_self_balancing_components.py` & `mixician-0.1.9/src/mixician/calculators/calculate_with_self_balancing_components.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
         self.cumulative_product_scores = np.prod(self.cumulative_product_scores, axis=1)
 
     def plot_self_balancing_projected_distribution(self) -> None:
         """Plots the projected data distribution after applying logarithm PCA and balancing weights."""
         if self.cumulative_product_scores is None:
             self._calculate_cumulative_product_scores()
         self.viewer_instance.plot_logarithm_array_distribution(
-            scores=self.cumulative_product_scores,
+            scores=np.asarray(self.cumulative_product_scores),
             legend=r"$\log_{10}{(\text{cumulative\_product\_scores})}$",
         )
 
     def update(self, pca_weights: np.ndarray) -> None:
         """Updates the PCA weights with the provided weights."""
         self.update_pca_weights(pca_weights)
         self.calculte_balanced_weights()
```

### Comparing `mixician-0.1.8/src/mixician/dataloaders/base.py` & `mixician-0.1.9/src/mixician/dataloaders/base.py`

 * *Files identical despite different names*

### Comparing `mixician-0.1.8/src/mixician/dataloaders/load_config.py` & `mixician-0.1.9/src/mixician/dataloaders/load_config.py`

 * *Files identical despite different names*

### Comparing `mixician-0.1.8/src/mixician/dataloaders/load_dataframe.py` & `mixician-0.1.9/src/mixician/dataloaders/load_dataframe.py`

 * *Files identical despite different names*

### Comparing `mixician-0.1.8/src/mixician/dataloaders/set_path.py` & `mixician-0.1.9/src/mixician/dataloaders/set_path.py`

 * *Files identical despite different names*

### Comparing `mixician-0.1.8/src/mixician/examples/calculate_value_based_ensemble_score/self_balancing_value_based_ensemble_score.ipynb` & `mixician-0.1.9/src/mixician/examples/calculate_value_based_ensemble_score/self_balancing_value_based_ensemble_score.ipynb`

 * *Files identical despite different names*

### Comparing `mixician-0.1.8/src/mixician/examples/calculate_value_based_ensemble_score/value_based_ensemble_score.ipynb` & `mixician-0.1.9/src/mixician/examples/calculate_value_based_ensemble_score/value_based_ensemble_score.ipynb`

 * *Files identical despite different names*

### Comparing `mixician-0.1.8/src/mixician/examples/dataset/utils.py` & `mixician-0.1.9/src/mixician/examples/dataset/utils.py`

 * *Files identical despite different names*

### Comparing `mixician-0.1.8/src/mixician/visualization/plot_distributions.py` & `mixician-0.1.9/src/mixician/visualization/plot_distributions.py`

 * *Files identical despite different names*

### Comparing `mixician-0.1.8/PKG-INFO` & `mixician-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mixician
-Version: 0.1.8
+Version: 0.1.9
 Summary: An advanced hybrid ranking engine for recommendation systems, designed to automate the optimization of algorithms and parameters tailored to diverse business objectives.
 Home-page: https://github.com/yinsn/Mixician
 License: MIT
 Author: Yin Cheng
 Author-email: yin.sjtu@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

