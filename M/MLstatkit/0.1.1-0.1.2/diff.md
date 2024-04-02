# Comparing `tmp/MLstatkit-0.1.1.tar.gz` & `tmp/MLstatkit-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MLstatkit-0.1.1.tar", last modified: Mon Apr  1 21:29:23 2024, max compression
+gzip compressed data, was "MLstatkit-0.1.2.tar", last modified: Mon Apr  1 21:41:19 2024, max compression
```

## Comparing `MLstatkit-0.1.1.tar` & `MLstatkit-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 brritanyhuang   (501) staff       (20)        0 2024-04-01 21:29:23.069870 MLstatkit-0.1.1/
--rw-r--r--   0 brritanyhuang   (501) staff       (20)     1072 2024-04-01 20:44:17.000000 MLstatkit-0.1.1/LICENSE
-drwxr-xr-x   0 brritanyhuang   (501) staff       (20)        0 2024-04-01 21:29:23.069036 MLstatkit-0.1.1/MLstatkit/
--rw-r--r--   0 brritanyhuang   (501) staff       (20)        0 2024-04-01 20:44:17.000000 MLstatkit-0.1.1/MLstatkit/__init__.py
--rw-r--r--   0 brritanyhuang   (501) staff       (20)     6374 2024-04-01 20:44:17.000000 MLstatkit-0.1.1/MLstatkit/stats.py
-drwxr-xr-x   0 brritanyhuang   (501) staff       (20)        0 2024-04-01 21:29:23.069578 MLstatkit-0.1.1/MLstatkit.egg-info/
--rw-r--r--   0 brritanyhuang   (501) staff       (20)     7426 2024-04-01 21:29:22.000000 MLstatkit-0.1.1/MLstatkit.egg-info/PKG-INFO
--rw-r--r--   0 brritanyhuang   (501) staff       (20)      231 2024-04-01 21:29:23.000000 MLstatkit-0.1.1/MLstatkit.egg-info/SOURCES.txt
--rw-r--r--   0 brritanyhuang   (501) staff       (20)        1 2024-04-01 21:29:22.000000 MLstatkit-0.1.1/MLstatkit.egg-info/dependency_links.txt
--rw-r--r--   0 brritanyhuang   (501) staff       (20)       32 2024-04-01 21:29:22.000000 MLstatkit-0.1.1/MLstatkit.egg-info/requires.txt
--rw-r--r--   0 brritanyhuang   (501) staff       (20)       10 2024-04-01 21:29:22.000000 MLstatkit-0.1.1/MLstatkit.egg-info/top_level.txt
--rw-r--r--   0 brritanyhuang   (501) staff       (20)     7426 2024-04-01 21:29:23.069741 MLstatkit-0.1.1/PKG-INFO
--rw-r--r--   0 brritanyhuang   (501) staff       (20)     6379 2024-04-01 21:28:23.000000 MLstatkit-0.1.1/README.md
--rw-r--r--   0 brritanyhuang   (501) staff       (20)       38 2024-04-01 21:29:23.069912 MLstatkit-0.1.1/setup.cfg
--rw-r--r--   0 brritanyhuang   (501) staff       (20)     1390 2024-04-01 21:07:40.000000 MLstatkit-0.1.1/setup.py
+drwxr-xr-x   0 brritanyhuang   (501) staff       (20)        0 2024-04-01 21:41:19.952805 MLstatkit-0.1.2/
+-rw-r--r--   0 brritanyhuang   (501) staff       (20)     1072 2024-04-01 20:44:17.000000 MLstatkit-0.1.2/LICENSE
+drwxr-xr-x   0 brritanyhuang   (501) staff       (20)        0 2024-04-01 21:41:19.951943 MLstatkit-0.1.2/MLstatkit/
+-rw-r--r--   0 brritanyhuang   (501) staff       (20)        0 2024-04-01 20:44:17.000000 MLstatkit-0.1.2/MLstatkit/__init__.py
+-rw-r--r--   0 brritanyhuang   (501) staff       (20)     6446 2024-04-01 21:39:19.000000 MLstatkit-0.1.2/MLstatkit/stats.py
+drwxr-xr-x   0 brritanyhuang   (501) staff       (20)        0 2024-04-01 21:41:19.952482 MLstatkit-0.1.2/MLstatkit.egg-info/
+-rw-r--r--   0 brritanyhuang   (501) staff       (20)     7493 2024-04-01 21:41:19.000000 MLstatkit-0.1.2/MLstatkit.egg-info/PKG-INFO
+-rw-r--r--   0 brritanyhuang   (501) staff       (20)      231 2024-04-01 21:41:19.000000 MLstatkit-0.1.2/MLstatkit.egg-info/SOURCES.txt
+-rw-r--r--   0 brritanyhuang   (501) staff       (20)        1 2024-04-01 21:41:19.000000 MLstatkit-0.1.2/MLstatkit.egg-info/dependency_links.txt
+-rw-r--r--   0 brritanyhuang   (501) staff       (20)       37 2024-04-01 21:41:19.000000 MLstatkit-0.1.2/MLstatkit.egg-info/requires.txt
+-rw-r--r--   0 brritanyhuang   (501) staff       (20)       10 2024-04-01 21:41:19.000000 MLstatkit-0.1.2/MLstatkit.egg-info/top_level.txt
+-rw-r--r--   0 brritanyhuang   (501) staff       (20)     7493 2024-04-01 21:41:19.952671 MLstatkit-0.1.2/PKG-INFO
+-rw-r--r--   0 brritanyhuang   (501) staff       (20)     6446 2024-04-01 21:40:42.000000 MLstatkit-0.1.2/README.md
+-rw-r--r--   0 brritanyhuang   (501) staff       (20)       38 2024-04-01 21:41:19.952851 MLstatkit-0.1.2/setup.cfg
+-rw-r--r--   0 brritanyhuang   (501) staff       (20)     1398 2024-04-01 21:41:13.000000 MLstatkit-0.1.2/setup.py
```

### Comparing `MLstatkit-0.1.1/LICENSE` & `MLstatkit-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `MLstatkit-0.1.1/MLstatkit/stats.py` & `MLstatkit-0.1.2/MLstatkit/stats.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pandas as pd
 import numpy as np
 import scipy.stats
 from sklearn.metrics import roc_auc_score, average_precision_score, f1_score
-
+from tqdm.auto import tqdm
 
 def Delong_test(true, prob_A, prob_B):
     """
     Perform DeLong's test for comparing the AUCs of two models.
 
     Parameters
     ----------
@@ -137,15 +137,15 @@
         original_score = f1_score(y_true, y_pred, average=average)
     else:
         raise ValueError(f"Unsupported score function: {score_func_str}")
     
     bootstrapped_scores = []
     rng = np.random.RandomState(42)  # Control reproducibility
     
-    for _ in range(n_bootstraps):
+    for _ in tqdm(range(n_bootstraps), desc=f"Bootstrapping {score_func_str}"):
         # Randomly sample with replacement
         indices = rng.randint(0, len(y_prob), len(y_prob))
         if len(np.unique(y_true[indices])) < 2:
             continue  # Skip this loop iteration if sample is not valid
         
         if score_func_str == 'auroc':
             score = roc_auc_score(y_true[indices], y_prob[indices], average=average)
```

### Comparing `MLstatkit-0.1.1/MLstatkit.egg-info/PKG-INFO` & `MLstatkit-0.1.2/MLstatkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MLstatkit
-Version: 0.1.1
+Version: 0.1.2
 Summary: MLstatkit is a comprehensive Python library designed to seamlessly integrate established statistical methods into machine learning projects.
 Home-page: https://github.com/Brritany/MLstatkit
 Author: Yong-Zhen Huang
 Author-email: m946111005@tmu.edu.tw
 License: UNKNOWN
 Project-URL: Tracker, https://github.com/Brritany/MLstatkit/issues
 Keywords: python,statistics,Delong test,Bootstrapping
@@ -156,10 +156,11 @@
 
 ## License
 
 MLstatkit is distributed under the MIT License. For more information, see the LICENSE file in the GitHub repository.
 
 ### Update log
 
+- `0.1.2`  Add `Bootstrapping` operation process progress display.
 - `0.1.1`  Update `README.md`, `setup.py`. Add `CONTRIBUTING.md`.
 - `0.1.0`  First edition
```

### Comparing `MLstatkit-0.1.1/PKG-INFO` & `MLstatkit-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MLstatkit
-Version: 0.1.1
+Version: 0.1.2
 Summary: MLstatkit is a comprehensive Python library designed to seamlessly integrate established statistical methods into machine learning projects.
 Home-page: https://github.com/Brritany/MLstatkit
 Author: Yong-Zhen Huang
 Author-email: m946111005@tmu.edu.tw
 License: UNKNOWN
 Project-URL: Tracker, https://github.com/Brritany/MLstatkit/issues
 Keywords: python,statistics,Delong test,Bootstrapping
@@ -156,10 +156,11 @@
 
 ## License
 
 MLstatkit is distributed under the MIT License. For more information, see the LICENSE file in the GitHub repository.
 
 ### Update log
 
+- `0.1.2`  Add `Bootstrapping` operation process progress display.
 - `0.1.1`  Update `README.md`, `setup.py`. Add `CONTRIBUTING.md`.
 - `0.1.0`  First edition
```

### Comparing `MLstatkit-0.1.1/README.md` & `MLstatkit-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -132,9 +132,10 @@
 
 ## License
 
 MLstatkit is distributed under the MIT License. For more information, see the LICENSE file in the GitHub repository.
 
 ### Update log
 
+- `0.1.2`  Add `Bootstrapping` operation process progress display.
 - `0.1.1`  Update `README.md`, `setup.py`. Add `CONTRIBUTING.md`.
 - `0.1.0`  First edition
```

### Comparing `MLstatkit-0.1.1/setup.py` & `MLstatkit-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="MLstatkit",
-    version="0.1.1",
+    version="0.1.2",
     description="MLstatkit is a comprehensive Python library designed to seamlessly integrate established statistical methods into machine learning projects.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/Brritany/MLstatkit',
     project_urls={
         'Tracker': 'https://github.com/Brritany/MLstatkit/issues',
     },
     author="Yong-Zhen Huang",
     author_email="m946111005@tmu.edu.tw",
     packages=find_packages(),
     keywords=['python', 'statistics', 'Delong test', 'Bootstrapping'],
     install_requires=[
-        "pandas", "numpy", "scipy", "scikit-learn"
+        "pandas", "numpy", "scipy", "scikit-learn", "tqdm"
     ],
     include_package_data=True,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Science/Research",
         "Natural Language :: English",
         "Topic :: Scientific/Engineering",
```

