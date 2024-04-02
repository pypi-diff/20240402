# Comparing `tmp/modnet-0.4.1.tar.gz` & `tmp/modnet-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/modnet-0.4.1.tar", last modified: Sat Jul 29 11:01:49 2023, max compression
+gzip compressed data, was "dist/modnet-0.4.2.tar", last modified: Tue Apr  2 15:48:47 2024, max compression
```

## Comparing `modnet-0.4.1.tar` & `modnet-0.4.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-07-29 11:01:49.000000 modnet-0.4.1/
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     1078 2022-01-10 10:10:32.000000 modnet-0.4.1/LICENSE.md
--rw-r--r--   0 ppdebreuck   (501) staff       (20)       48 2022-01-10 10:10:32.000000 modnet-0.4.1/MANIFEST.in
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     6135 2023-07-29 11:01:49.000000 modnet-0.4.1/PKG-INFO
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     4243 2023-07-11 13:21:01.000000 modnet-0.4.1/README.md
-drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-07-29 11:01:49.000000 modnet-0.4.1/modnet/
--rw-r--r--   0 ppdebreuck   (501) staff       (20)       22 2023-07-28 12:19:26.000000 modnet-0.4.1/modnet/__init__.py
-drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-07-29 11:01:49.000000 modnet-0.4.1/modnet/data/
--rw-r--r--   0 ppdebreuck   (501) staff       (20) 13666623 2021-11-08 13:57:41.000000 modnet-0.4.1/modnet/data/Features_cross
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     4055 2022-05-12 10:28:50.000000 modnet-0.4.1/modnet/ext_data.py
-drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-07-29 11:01:49.000000 modnet-0.4.1/modnet/featurizers/
--rw-r--r--   0 ppdebreuck   (501) staff       (20)      264 2021-02-15 14:07:41.000000 modnet-0.4.1/modnet/featurizers/__init__.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)    12534 2023-07-28 12:09:44.000000 modnet-0.4.1/modnet/featurizers/featurizers.py
-drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-07-29 11:01:49.000000 modnet-0.4.1/modnet/featurizers/presets/
--rw-r--r--   0 ppdebreuck   (501) staff       (20)      978 2023-07-11 13:21:01.000000 modnet-0.4.1/modnet/featurizers/presets/__init__.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)    10080 2023-07-28 12:09:44.000000 modnet-0.4.1/modnet/featurizers/presets/debreuck_2020.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     9303 2023-07-28 12:09:44.000000 modnet-0.4.1/modnet/featurizers/presets/matminer_2023.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)    16049 2023-07-28 12:09:44.000000 modnet-0.4.1/modnet/featurizers/presets/matminer_all_2023.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)      623 2023-07-28 12:09:44.000000 modnet-0.4.1/modnet/featurizers/utils.py
-drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-07-29 11:01:49.000000 modnet-0.4.1/modnet/hyper_opt/
--rw-r--r--   0 ppdebreuck   (501) staff       (20)       63 2022-01-12 21:23:06.000000 modnet-0.4.1/modnet/hyper_opt/__init__.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)    27250 2023-07-28 12:18:53.000000 modnet-0.4.1/modnet/hyper_opt/fit_genetic.py
-drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-07-29 11:01:49.000000 modnet-0.4.1/modnet/matbench/
--rw-r--r--   0 ppdebreuck   (501) staff       (20)      116 2021-02-15 14:07:41.000000 modnet-0.4.1/modnet/matbench/__init__.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)    11640 2023-07-11 13:21:01.000000 modnet-0.4.1/modnet/matbench/benchmark.py
-drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-07-29 11:01:49.000000 modnet-0.4.1/modnet/model_presets/
--rw-r--r--   0 ppdebreuck   (501) staff       (20)      166 2022-01-10 10:10:32.000000 modnet-0.4.1/modnet/model_presets/__init__.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     2292 2021-08-16 13:22:38.000000 modnet-0.4.1/modnet/model_presets/presets.py
-drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-07-29 11:01:49.000000 modnet-0.4.1/modnet/models/
--rw-r--r--   0 ppdebreuck   (501) staff       (20)      190 2022-05-10 12:28:41.000000 modnet-0.4.1/modnet/models/__init__.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)    14851 2023-07-11 14:46:35.000000 modnet-0.4.1/modnet/models/bayesian.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)    17885 2023-07-13 18:28:15.000000 modnet-0.4.1/modnet/models/ensemble.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)    59819 2023-07-28 12:09:44.000000 modnet-0.4.1/modnet/models/vanilla.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)    41902 2023-07-28 12:09:44.000000 modnet-0.4.1/modnet/preprocessing.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     6345 2022-05-19 13:18:13.000000 modnet-0.4.1/modnet/sklearn.py
-drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-07-29 11:01:49.000000 modnet-0.4.1/modnet/tests/
--rw-r--r--   0 ppdebreuck   (501) staff       (20)        0 2020-09-16 10:22:36.000000 modnet-0.4.1/modnet/tests/__init__.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     3410 2023-07-11 13:21:01.000000 modnet-0.4.1/modnet/tests/conftest.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     4444 2023-07-11 13:21:01.000000 modnet-0.4.1/modnet/tests/test_benchmark.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)      563 2021-01-14 10:39:09.000000 modnet-0.4.1/modnet/tests/test_ext_data.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)      771 2023-07-11 13:21:01.000000 modnet-0.4.1/modnet/tests/test_hyper_opt.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     9497 2023-07-11 13:21:01.000000 modnet-0.4.1/modnet/tests/test_model.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)    18202 2023-07-11 13:24:52.000000 modnet-0.4.1/modnet/tests/test_preprocessing.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     3110 2022-05-19 13:18:13.000000 modnet-0.4.1/modnet/tests/test_sklearn.py
--rw-r--r--   0 ppdebreuck   (501) staff       (20)      737 2021-02-15 14:07:41.000000 modnet-0.4.1/modnet/utils.py
-drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2023-07-29 11:01:49.000000 modnet-0.4.1/modnet.egg-info/
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     6135 2023-07-29 11:01:48.000000 modnet-0.4.1/modnet.egg-info/PKG-INFO
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     1110 2023-07-29 11:01:48.000000 modnet-0.4.1/modnet.egg-info/SOURCES.txt
--rw-r--r--   0 ppdebreuck   (501) staff       (20)        1 2023-07-29 11:01:48.000000 modnet-0.4.1/modnet.egg-info/dependency_links.txt
--rw-r--r--   0 ppdebreuck   (501) staff       (20)      223 2023-07-29 11:01:48.000000 modnet-0.4.1/modnet.egg-info/requires.txt
--rw-r--r--   0 ppdebreuck   (501) staff       (20)        7 2023-07-29 11:01:48.000000 modnet-0.4.1/modnet.egg-info/top_level.txt
--rw-r--r--   0 ppdebreuck   (501) staff       (20)      118 2023-07-29 11:01:49.000000 modnet-0.4.1/setup.cfg
--rw-r--r--   0 ppdebreuck   (501) staff       (20)     2085 2023-07-11 13:21:01.000000 modnet-0.4.1/setup.py
+drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2024-04-02 15:48:47.000000 modnet-0.4.2/
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     1078 2022-01-10 10:10:32.000000 modnet-0.4.2/LICENSE.md
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)       48 2022-01-10 10:10:32.000000 modnet-0.4.2/MANIFEST.in
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     6057 2024-04-02 15:48:47.000000 modnet-0.4.2/PKG-INFO
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     4243 2023-07-11 13:21:01.000000 modnet-0.4.2/README.md
+drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2024-04-02 15:48:47.000000 modnet-0.4.2/modnet/
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)       22 2024-03-28 10:26:50.000000 modnet-0.4.2/modnet/__init__.py
+drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2024-04-02 15:48:47.000000 modnet-0.4.2/modnet/data/
+-rw-r--r--   0 ppdebreuck   (501) staff       (20) 13666623 2021-11-08 13:57:41.000000 modnet-0.4.2/modnet/data/Features_cross
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     4055 2022-05-12 10:28:50.000000 modnet-0.4.2/modnet/ext_data.py
+drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2024-04-02 15:48:47.000000 modnet-0.4.2/modnet/featurizers/
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)      264 2021-02-15 14:07:41.000000 modnet-0.4.2/modnet/featurizers/__init__.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)    12908 2024-04-02 15:48:26.000000 modnet-0.4.2/modnet/featurizers/featurizers.py
+drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2024-04-02 15:48:47.000000 modnet-0.4.2/modnet/featurizers/presets/
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)      978 2023-07-11 13:21:01.000000 modnet-0.4.2/modnet/featurizers/presets/__init__.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)    10080 2023-07-28 12:09:44.000000 modnet-0.4.2/modnet/featurizers/presets/debreuck_2020.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     9303 2023-07-28 12:09:44.000000 modnet-0.4.2/modnet/featurizers/presets/matminer_2023.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)    16049 2023-07-28 12:09:44.000000 modnet-0.4.2/modnet/featurizers/presets/matminer_all_2023.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)      623 2023-07-28 12:09:44.000000 modnet-0.4.2/modnet/featurizers/utils.py
+drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2024-04-02 15:48:47.000000 modnet-0.4.2/modnet/hyper_opt/
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)       63 2022-01-12 21:23:06.000000 modnet-0.4.2/modnet/hyper_opt/__init__.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)    27301 2024-03-28 10:26:50.000000 modnet-0.4.2/modnet/hyper_opt/fit_genetic.py
+drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2024-04-02 15:48:47.000000 modnet-0.4.2/modnet/matbench/
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)      116 2021-02-15 14:07:41.000000 modnet-0.4.2/modnet/matbench/__init__.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)    11640 2023-07-11 13:21:01.000000 modnet-0.4.2/modnet/matbench/benchmark.py
+drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2024-04-02 15:48:47.000000 modnet-0.4.2/modnet/model_presets/
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)      166 2022-01-10 10:10:32.000000 modnet-0.4.2/modnet/model_presets/__init__.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     2292 2021-08-16 13:22:38.000000 modnet-0.4.2/modnet/model_presets/presets.py
+drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2024-04-02 15:48:47.000000 modnet-0.4.2/modnet/models/
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)      402 2024-02-07 15:47:41.000000 modnet-0.4.2/modnet/models/__init__.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)    15169 2024-04-02 15:48:26.000000 modnet-0.4.2/modnet/models/bayesian.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)    17887 2024-03-28 10:26:50.000000 modnet-0.4.2/modnet/models/ensemble.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)    60314 2024-03-28 10:26:50.000000 modnet-0.4.2/modnet/models/vanilla.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)    41991 2024-03-28 10:26:50.000000 modnet-0.4.2/modnet/preprocessing.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     6344 2024-03-28 10:26:50.000000 modnet-0.4.2/modnet/sklearn.py
+drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2024-04-02 15:48:47.000000 modnet-0.4.2/modnet/tests/
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)        0 2020-09-16 10:22:36.000000 modnet-0.4.2/modnet/tests/__init__.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     4550 2024-04-02 15:48:26.000000 modnet-0.4.2/modnet/tests/conftest.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     4444 2023-07-11 13:21:01.000000 modnet-0.4.2/modnet/tests/test_benchmark.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)      563 2021-01-14 10:39:09.000000 modnet-0.4.2/modnet/tests/test_ext_data.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)      771 2024-04-02 15:48:22.000000 modnet-0.4.2/modnet/tests/test_hyper_opt.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     9504 2024-02-07 15:47:41.000000 modnet-0.4.2/modnet/tests/test_model.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)    17907 2024-04-02 15:48:26.000000 modnet-0.4.2/modnet/tests/test_preprocessing.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     3110 2022-05-19 13:18:13.000000 modnet-0.4.2/modnet/tests/test_sklearn.py
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)      737 2021-02-15 14:07:41.000000 modnet-0.4.2/modnet/utils.py
+drwxr-xr-x   0 ppdebreuck   (501) staff       (20)        0 2024-04-02 15:48:47.000000 modnet-0.4.2/modnet.egg-info/
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     6057 2024-04-02 15:48:47.000000 modnet-0.4.2/modnet.egg-info/PKG-INFO
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     1110 2024-04-02 15:48:47.000000 modnet-0.4.2/modnet.egg-info/SOURCES.txt
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)        1 2024-04-02 15:48:47.000000 modnet-0.4.2/modnet.egg-info/dependency_links.txt
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)      206 2024-04-02 15:48:47.000000 modnet-0.4.2/modnet.egg-info/requires.txt
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)        7 2024-04-02 15:48:47.000000 modnet-0.4.2/modnet.egg-info/top_level.txt
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)      118 2024-04-02 15:48:47.000000 modnet-0.4.2/setup.cfg
+-rw-r--r--   0 ppdebreuck   (501) staff       (20)     1877 2024-04-02 15:48:26.000000 modnet-0.4.2/setup.py
```

### Comparing `modnet-0.4.1/LICENSE.md` & `modnet-0.4.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `modnet-0.4.1/PKG-INFO` & `modnet-0.4.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modnet
-Version: 0.4.1
+Version: 0.4.2
 Summary: MODNet, the Material Optimal Descriptor Network for materials properties prediction. 
 Home-page: https://github.com/ppdebreuck/modnet
 Author: Pierre-Paul De Breuck
 Author-email: pierre-paul.debreuck@uclouvain.be
 License: UNKNOWN
 Project-URL: GitHub, https://github.com/ppdebreuck/modnet
 Project-URL: Documentation, https://modnet.readthedocs.io
@@ -106,21 +106,20 @@
         
         <a name="License"></a>
         ## License
         
         MODNet is released under the MIT License.
         
 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+Provides-Extra: bayesian
 Provides-Extra: test
 Provides-Extra: dev
```

### Comparing `modnet-0.4.1/README.md` & `modnet-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `modnet-0.4.1/modnet/data/Features_cross` & `modnet-0.4.2/modnet/data/Features_cross`

 * *Files identical despite different names*

### Comparing `modnet-0.4.1/modnet/ext_data.py` & `modnet-0.4.2/modnet/ext_data.py`

 * *Files identical despite different names*

### Comparing `modnet-0.4.1/modnet/featurizers/featurizers.py` & `modnet-0.4.2/modnet/featurizers/featurizers.py`

 * *Files 13% similar despite different names*

```diff
@@ -137,15 +137,18 @@
                 )
             else:
                 _featurizers = MultipleFeaturizer(featurizers)
             if self._n_jobs is not None:
                 _featurizers.set_n_jobs(self._n_jobs)
 
             return _featurizers.featurize_dataframe(
-                df, column, multiindex=True, ignore_errors=True
+                df,
+                column,
+                multiindex=True,
+                ignore_errors=getattr(self, "ignore_errors", True),
             )
         elif mode == "single":
 
             for featurizer in featurizers:
 
                 if column not in df:
                     column = ("Input Data", column)
@@ -160,15 +163,18 @@
                     )
                 featurizer.set_n_jobs(1)
                 LOG.info(
                     f"Applying featurizer {featurizer.__class__.__name__} to column {column!r}."
                 )
                 start = time.monotonic_ns()
                 df = featurizer.featurize_dataframe(
-                    df, column, multiindex=True, ignore_errors=True
+                    df,
+                    column,
+                    multiindex=True,
+                    ignore_errors=getattr(self, "ignore_errors", True),
                 )
                 LOG.info(
                     f"Applied featurizer {featurizer.__class__.__name__} to column {column!r} in {(time.monotonic_ns() - start) * 1e-9} seconds"
                 )
             LOG.info("Applied all featurizers")
 
             return df
@@ -219,17 +225,17 @@
                 LOG.info(
                     "There are non-integer compositions in the dataset, and featurizers that need them. "
                     "Computing..."
                 )
                 df["integer_composition"] = [
                     Composition(
                         comp.get_integer_formula_and_factor(
-                            max_denominator=10
-                            if getattr(self, "fast_oxid", False)
-                            else 100
+                            max_denominator=(
+                                10 if getattr(self, "fast_oxid", False) else 100
+                            )
                         )[0]
                     )
                     for comp in df["composition"].values
                 ]
                 # df["integer_composition"] = df["composition"].apply(
                 # lambda c: c.get_integer_formula_and_factor(
                 #         max_denominator=10 if getattr(self, "fast_oxid", False) else 100
@@ -240,15 +246,19 @@
             if getattr(self, "fast_oxid", False):
                 df = CompositionToOxidComposition(
                     all_oxi_states=False, max_sites=-1
                 ).featurize_dataframe(df, col_id=col_comp)
             else:
                 df = CompositionToOxidComposition(
                     max_sites=-1 if getattr(self, "continuous_only", False) else None
-                ).featurize_dataframe(df, col_id=col_comp, ignore_errors=True)
+                ).featurize_dataframe(
+                    df,
+                    col_id=col_comp,
+                    ignore_errors=getattr(self, "ignore_errors", True),
+                )
             df = self._fit_apply_featurizers(
                 df,
                 self.oxid_composition_featurizers,
                 "composition_oxid",
                 mode=self.featurizer_mode,
             )
             df = df.rename(columns={"Input Data": ""})
@@ -307,15 +317,18 @@
             fingerprint_name = fingerprint.__class__.__name__
             if fingerprint_name == "SOAP":
                 fingerprint.fit(df["Input data|structure"])
             site_stats_fingerprint = SiteStatsFingerprint(
                 fingerprint, stats=self.site_stats
             )
             df = site_stats_fingerprint.featurize_dataframe(
-                df, "Input data|structure", multiindex=False, ignore_errors=True
+                df,
+                "Input data|structure",
+                multiindex=False,
+                ignore_errors=getattr(self, "ignore_errors", True),
             )
 
             if aliases:
                 fingerprint_name = aliases.get(fingerprint_name, fingerprint_name)
             if "|" not in fingerprint_name:
                 fingerprint_name += "|"
             df.columns = [
```

### Comparing `modnet-0.4.1/modnet/featurizers/presets/__init__.py` & `modnet-0.4.2/modnet/featurizers/presets/__init__.py`

 * *Files identical despite different names*

### Comparing `modnet-0.4.1/modnet/featurizers/presets/debreuck_2020.py` & `modnet-0.4.2/modnet/featurizers/presets/debreuck_2020.py`

 * *Files identical despite different names*

### Comparing `modnet-0.4.1/modnet/featurizers/presets/matminer_2023.py` & `modnet-0.4.2/modnet/featurizers/presets/matminer_2023.py`

 * *Files identical despite different names*

### Comparing `modnet-0.4.1/modnet/featurizers/presets/matminer_all_2023.py` & `modnet-0.4.2/modnet/featurizers/presets/matminer_all_2023.py`

 * *Files identical despite different names*

### Comparing `modnet-0.4.1/modnet/featurizers/utils.py` & `modnet-0.4.2/modnet/featurizers/utils.py`

 * *Files identical despite different names*

### Comparing `modnet-0.4.1/modnet/hyper_opt/fit_genetic.py` & `modnet-0.4.2/modnet/hyper_opt/fit_genetic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from __future__ import annotations
+import math
 import random
 from typing import List, Optional, Dict, Union, Callable
 import numpy as np
 import tensorflow as tf
 from sklearn.model_selection import train_test_split
 from modnet.preprocessing import MODData
 from modnet.models import MODNetModel, EnsembleMODNetModel
 from modnet.utils import LOG
 import multiprocessing
 import tqdm
 
 
 class Individual:
-
     """Class representing a set of hyperparameters for the genetic algorithm."""
 
     def __init__(
         self,
         max_feat: int,
         num_classes: dict,
         multi_label: bool,
@@ -86,24 +86,20 @@
         """Does the crossover of two parents and returns a 'child' which has a mix of the parents hyperparams.
 
         Args:
             partner (Individual): Partner individual.
         Returns:
             Individual: Child.
         """
-
-        genes_from_mother = random.sample(
-            range(len(self.genes)), k=len(self.genes) // 2
-        )  # creates indices to take randomly half the genes from one parent, and half the genes from the other
+        # creates indices to take randomly half the genes from one parent, and half the genes from the other
+        mother_genes = random.sample(self.genes.keys(), k=len(self.genes) // 2)
 
         child_genes = {
-            list(self.genes.keys())[i]: list(self.genes.values())[i]
-            if i in genes_from_mother
-            else list(partner.genes.values())[i]
-            for i in range(len(self.genes))
+            gene: self.genes[gene] if gene in mother_genes else partner.genes[gene]
+            for gene in self.genes
         }
 
         child = Individual(
             max_feat=self.max_feat,
             num_classes=self.num_classes,
             multi_label=self.multi_label,
             loss=self.genes["loss"],
@@ -234,15 +230,18 @@
             impute_missing=self.genes["impute_missing"],
             xscale_before_impute=self.genes["xscale_before_impute"],
             callbacks=callbacks,
             verbose=0,
             **self.fit_params,
         )
 
-        self.val_loss = model.evaluate(val_data)
+        self.val_loss = model.evaluate(
+            val_data,
+            loss=self.genes["loss"],
+        )
         self.model = model
 
     def refit_model(self, data: MODData, n_models=10, n_jobs=1, fast: bool = False):
         """Refit inner model on specified data.
         Args:
             data (MODData): Training data
             fast (bool, optional): Limited epoch for testing or debugging only. Defaults to False.
@@ -435,17 +434,17 @@
         Returns:
             val_losses, models, individuals
         """
 
         from modnet.matbench.benchmark import matbench_kfold_splits
         import os
 
-        os.environ[
-            "TF_CPP_MIN_LOG_LEVEL"
-        ] = "2"  # many models will be fitted => reduce output
+        os.environ["TF_CPP_MIN_LOG_LEVEL"] = (
+            "2"  # many models will be fitted => reduce output
+        )
 
         num_nested_folds = 5
         if nested:
             num_nested_folds = nested
         if num_nested_folds <= 1:
             num_nested_folds = 5
 
@@ -570,14 +569,15 @@
         for j in range(1, num_generations):
             LOG.info("Generation number {}".format(j))
 
             # select parents
             weights = [
                 1 / lw**5 for lw in val_loss[ranking]
             ]  # **5 in order to give relatively more importance to the best individuals
+            weights = [1e-5 if math.isnan(weight) else weight for weight in weights]
             weights = [w / sum(weights) for w in weights]
             # selection: weighted choice of the parents -> parents with a low MAE have more chance to be selected
             parents_1 = random.choices(
                 individuals[ranking], weights=weights, k=size_pop
             )
             parents_2 = random.choices(
                 individuals[ranking], weights=weights, k=size_pop
```

### Comparing `modnet-0.4.1/modnet/matbench/benchmark.py` & `modnet-0.4.2/modnet/matbench/benchmark.py`

 * *Files identical despite different names*

### Comparing `modnet-0.4.1/modnet/model_presets/presets.py` & `modnet-0.4.2/modnet/model_presets/presets.py`

 * *Files identical despite different names*

### Comparing `modnet-0.4.1/modnet/models/bayesian.py` & `modnet-0.4.2/modnet/models/bayesian.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 """This submodule defines the `BayesianMODNetModel`, an extension to the vanilla
 model that incorporates probabilistic `DenseVariational` layers from TensorFlow
 Probability.
 
 """
 
-from typing import Optional, Dict, List, Tuple
+import warnings
 from functools import partial
+from typing import Dict, List, Optional, Tuple
 
 import numpy as np
 import pandas as pd
 import tensorflow as tf
-import tensorflow_probability as tfp
+
+try:
+    import tensorflow_probability as tfp
+except ImportError:
+    raise ImportError(
+        "`tensorflow-probability` is required for Bayesian models: install modnet[bayesian]."
+    )
 
 from modnet import __version__
 from modnet.models.vanilla import MODNetModel
 from modnet.preprocessing import MODData
 
 __all__ = ("BayesianMODNetModel",)
 
@@ -73,14 +80,19 @@
             act: A string defining a tf.keras activation function to pass to use
                 in the `tf.keras.layers.Dense` layers.
             out_act: A string defining a tf.keras activation function to pass to use
                 for the last output layer
 
         """
 
+        warnings.warn(
+            "BayesianMODNetModel is deprecated and may be removed in the future.",
+            DeprecationWarning,
+        )
+
         self.__modnet_version__ = __version__
 
         if n_feat is None:
             n_feat = 64
         self.n_feat = n_feat
         self.weights = weights
         self.num_classes = num_classes
```

### Comparing `modnet-0.4.1/modnet/models/ensemble.py` & `modnet-0.4.2/modnet/models/ensemble.py`

 * *Files 0% similar despite different names*

```diff
@@ -251,17 +251,17 @@
             - The settings of the best-performing preset.
 
         """
 
         from modnet.matbench.benchmark import matbench_kfold_splits
         import os
 
-        os.environ[
-            "TF_CPP_MIN_LOG_LEVEL"
-        ] = "2"  # many models will be fitted => reduce output
+        os.environ["TF_CPP_MIN_LOG_LEVEL"] = (
+            "2"  # many models will be fitted => reduce output
+        )
 
         if callbacks is None:
             es = tf.keras.callbacks.EarlyStopping(
                 monitor="loss",
                 min_delta=0.001,
                 patience=100,
                 verbose=verbose,
```

### Comparing `modnet-0.4.1/modnet/models/vanilla.py` & `modnet-0.4.2/modnet/models/vanilla.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """This submodule defines the "vanilla" `MODNetModel`, i.e. a single
 model with deterministic weights and outputs.
 
 """
+
 from collections import defaultdict
 from typing import List, Tuple, Dict, Optional, Callable, Any, Union
 
 from pathlib import Path
 import multiprocessing
 
 import pandas as pd
 import numpy as np
 import warnings
 from sklearn.preprocessing import StandardScaler, MinMaxScaler
 from sklearn.model_selection import train_test_split
-from sklearn.metrics import mean_absolute_error, roc_auc_score
+from sklearn.metrics import mean_absolute_error, mean_squared_error, roc_auc_score
 from sklearn.impute import SimpleImputer
 from sklearn.pipeline import Pipeline
 import tensorflow as tf
 
 from modnet.preprocessing import MODData
 from modnet.utils import LOG
 from modnet import __version__
@@ -354,15 +355,14 @@
                     y_inner = tf.keras.utils.to_categorical(
                         training_data.df_targets[targ].values,
                         num_classes=self.num_classes[targ],
                     )
                     if loss is None:
                         loss = "categorical_crossentropy"
             else:
-
                 y_inner = training_data.df_targets[prop].values.astype(
                     np.float64, copy=False
                 )
             if custom_data is not None:
                 val_data = None
                 val_fraction = 0
                 metrics = []
@@ -531,17 +531,17 @@
             - The settings of the best-performing preset.
 
         """
 
         from modnet.matbench.benchmark import matbench_kfold_splits
         import os
 
-        os.environ[
-            "TF_CPP_MIN_LOG_LEVEL"
-        ] = "2"  # many models will be fitted => reduce output
+        os.environ["TF_CPP_MIN_LOG_LEVEL"] = (
+            "2"  # many models will be fitted => reduce output
+        )
 
         if callbacks is None:
             es = tf.keras.callbacks.EarlyStopping(
                 monitor="loss",
                 min_delta=0.001,
                 patience=100,
                 verbose=verbose,
@@ -670,15 +670,15 @@
                 out_act=self.out_act,
                 num_classes=self.num_classes,
             ).model
             self.n_feat = n_feat
             self.fit(
                 data,
                 val_fraction=0,
-                learning_rate=best_preset["lr"],
+                lr=best_preset["lr"],
                 epochs=best_preset["epochs"],
                 batch_size=best_preset["batch_size"],
                 loss=best_preset["loss"],
                 callbacks=callbacks,
                 verbose=verbose,
                 **fit_params,
             )
@@ -754,17 +754,21 @@
                 for j, name in enumerate(props):
                     p_dic[name] = p[i][:, j]
         predictions = pd.DataFrame(p_dic)
         predictions.index = test_data.structure_ids
 
         return predictions
 
-    def evaluate(self, test_data: MODData) -> pd.DataFrame:
+    def evaluate(
+        self,
+        test_data: MODData,
+        loss: Union[str, Callable] = "mae",
+    ) -> pd.DataFrame:
         """Evaluates predictions on the passed MODData by returning the corresponding score:
-            - for regression: MAE
+            - for regression: loss function provided in loss argument. Defaults to mae.
             - for classification: negative ROC AUC.
             averaged over the targets when multi-target.
 
         Parameters:
             test_data: A featurized and feature-selected `MODData`
                 object containing the descriptors used in training.
 
@@ -808,15 +812,24 @@
                         except ValueError:
                             scores.append(float("nan"))
                     score.append(np.nanmean(scores))
             else:
                 y_true = test_data.df_targets[prop].values.astype(
                     np.float64, copy=False
                 )
-                score.append(mean_absolute_error(y_true, y_pred[i]))
+                if loss == "mae":
+                    loss = mean_absolute_error
+                elif loss == "mse":
+                    loss = mean_squared_error
+                elif isinstance(loss, str):
+                    raise RuntimeError(
+                        f"Loss {loss} not recognized. Use mae, mse or a callable."
+                    )
+                else:
+                    score.append(loss(y_true, y_pred[i]))
 
         return np.mean(score)
 
     def _make_picklable(self):
         """
         transforms inner keras model to jsons so that th MODNet object becomes picklable.
         """
```

### Comparing `modnet-0.4.1/modnet/preprocessing.py` & `modnet-0.4.2/modnet/preprocessing.py`

 * *Files 0% similar despite different names*

```diff
@@ -920,23 +920,24 @@
             if self.num_classes[targ] >= 2:
                 support = np.zeros(self.num_classes[targ])
                 for i in range(self.num_classes[targ]):
                     support[i] = (self.df_targets[targ].values == i).sum()
                 max_support = support.max()
                 for i in range(self.num_classes[targ]):
                     idxs = np.where(self.df_targets[targ].values == i)[0]
-                    sampled_x, sampled_y, sampled_struct = resample(
-                        self.df_featurized.iloc[idxs],
-                        self.df_targets.iloc[idxs],
-                        self.df_structure.iloc[idxs],
-                        n_samples=int(max_support - support[i]),
-                    )
-                    self.df_featurized = self.df_featurized.append(sampled_x)
-                    self.df_targets = self.df_targets.append(sampled_y)
-                    self.df_structure = self.df_structure.append(sampled_struct)
+                    if max_support - support[i] > 0:
+                        sampled_x, sampled_y, sampled_struct = resample(
+                            self.df_featurized.iloc[idxs],
+                            self.df_targets.iloc[idxs],
+                            self.df_structure.iloc[idxs],
+                            n_samples=int(max_support - support[i]),
+                        )
+                        self.df_featurized = self.df_featurized.append(sampled_x)
+                        self.df_targets = self.df_targets.append(sampled_y)
+                        self.df_structure = self.df_structure.append(sampled_struct)
 
     @property
     def structures(self) -> List[Union[Structure, CompositionContainer]]:
         """Returns the list of pymatgen `Structure` objects."""
         return list(self.df_structure["structure"])
 
     @property
```

### Comparing `modnet-0.4.1/modnet/sklearn.py` & `modnet-0.4.2/modnet/sklearn.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,14 @@
   (see https://scikit-learn.org/stable/modules/generated/sklearn.pipeline.Pipeline.html#sklearn.pipeline.Pipeline.fit)
 * Another note about the __init__ method of sklearn derived estimators:
   The method should ONLY set the instance variables. In particular, "every keyword argument accepted by __init__
   should correspond to an attribute on the instance" (as stated in sklearn's developer documentation)
   (see https://scikit-learn.org/stable/developers/develop.html#instantiation).
 """
 
-
 from sklearn.base import BaseEstimator
 from sklearn.base import RegressorMixin
 from sklearn.base import TransformerMixin
 from typing import Union, Dict
 from modnet.preprocessing import (
     get_features_relevance_redundancy,
     get_cross_nmi,
```

### Comparing `modnet-0.4.1/modnet/tests/conftest.py` & `modnet-0.4.2/modnet/tests/conftest.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import pytest
 from pathlib import Path
+from modnet.preprocessing import CompositionContainer
 
 from modnet.utils import get_hash_of_file
+from pymatgen.core import Structure
 
 
 _TEST_DATA_HASHES = {
     "MP_2018.6_subset.zip": (
         "d7d75e646dbde539645c8c0b065fd82cbe93f81d3500809655bd13d0acf2027c"
         "1786091a73f53985b08868c5be431a3c700f7f1776002df28ebf3a12a79ab1a1"
     ),
@@ -37,15 +39,32 @@
         raise RuntimeError(
             f"Cannot verify hash of {filename} as it was not provided, will not load pickle."
         )
     # Loading pickles can be dangerous, so lets at least check that the MD5 matches
     # what it was when created
     assert get_hash_of_file(data_file) == _TEST_DATA_HASHES[filename]
 
-    return MODData.load(data_file)
+    moddata = MODData.load(data_file)
+    # For forwards compatibility with pymatgen, we have to patch our old test data to have the following attributes
+    # to allow for depickling
+    # This is hopefully only a temporary solution, and in future, we should serialize pymatgen objects
+    # with Monty's `from_dict`/`to_dict` to avoid having to hack this private interface
+    for ind, s in enumerate(moddata.structures):
+        if isinstance(s, Structure):
+            # assume all previous data was periodic
+            moddata.structures[ind].lattice._pbc = [True, True, True]
+            for jnd, site in enumerate(s.sites):
+                # assume all of our previous data had ordered sites
+                moddata.structures[ind].sites[jnd].label = str(next(iter(site.species)))
+                # required for the global structure.is_ordered to work
+                moddata.structures[ind].sites[jnd].species._n_atoms = 1.0
+        elif isinstance(s, CompositionContainer):
+            moddata.structures[ind].composition._n_atoms = s.composition._natoms
+
+    return moddata
 
 
 @pytest.fixture(scope="function")
 def subset_moddata():
     """Loads the 100-structure featurized subset of MP.2018.6 for use
     in other tests, checking only the hash.
```

### Comparing `modnet-0.4.1/modnet/tests/test_benchmark.py` & `modnet-0.4.2/modnet/tests/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `modnet-0.4.1/modnet/tests/test_ext_data.py` & `modnet-0.4.2/modnet/tests/test_ext_data.py`

 * *Files identical despite different names*

### Comparing `modnet-0.4.1/modnet/tests/test_hyper_opt.py` & `modnet-0.4.2/modnet/tests/test_hyper_opt.py`

 * *Files identical despite different names*

### Comparing `modnet-0.4.1/modnet/tests/test_model.py` & `modnet-0.4.2/modnet/tests/test_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,14 @@
         n_feat=10,
     )
 
     model.fit(data, epochs=2)
     model.predict(data)
 
 
-@pytest.mark.slow
 def test_train_small_model_presets(subset_moddata, tf_session):
     """Tests the `fit_preset()` method."""
     from modnet.model_presets import gen_presets
     from modnet.models import MODNetModel
 
     modified_presets = gen_presets(100, 100)[:2]
 
@@ -101,14 +100,15 @@
     for num_nested, nested_option in zip([5, 1, 5], [5, 0, 1]):
         results = model.fit_preset(
             data,
             presets=modified_presets,
             nested=nested_option,
             val_fraction=0.2,
             n_jobs=1,
+            refit=True,
         )
         models = results[0]
         assert len(models) == len(modified_presets)
         assert len(models[0]) == num_nested
 
 
 def test_model_integration(subset_moddata, tf_session):
@@ -289,14 +289,15 @@
     model.predict(data, return_unc=True)
 
 
 @pytest.mark.slow
 def test_train_small_bootstrap_presets(small_moddata, tf_session):
     """Tests the `fit_preset()` method."""
     import time
+
     from modnet.model_presets import gen_presets
     from modnet.models import EnsembleMODNetModel
 
     start = time.time()
     modified_presets = gen_presets(100, 100)[:2]
 
     for ind, preset in enumerate(modified_presets):
```

### Comparing `modnet-0.4.1/modnet/tests/test_preprocessing.py` & `modnet-0.4.2/modnet/tests/test_preprocessing.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,22 @@
 def check_column_values(new: MODData, reference: MODData, tolerance=0.03):
     """Utiliy function  to check that moddata values haven't
     changed between initial calculation.
 
     Allows for some columns to be checked more loosely (see inline comment below).
 
     """
+    new_cols = set(new.df_featurized.columns)
+    old_cols = set(reference.df_featurized.columns)
+
+    # Check that the new df only adds new columns and is not missing anything
+    assert not (old_cols - new_cols)
+
     error_cols = set()
-    for col in new.df_featurized.columns:
+    for col in old_cols:
         if not (
             np.absolute(
                 (
                     new.df_featurized[col].to_numpy()
                     - reference.df_featurized[col].to_numpy()
                 )
                 / (reference.df_featurized[col].to_numpy() + 1e-6)
@@ -345,22 +351,14 @@
     targets = old.targets
 
     names = old.names
     featurizer = Matminer2023Featurizer()
     featurizer.featurizer_mode = featurizer_mode
     new = MODData(structures, targets, target_names=names, featurizer=featurizer)
     new.featurize(fast=False, n_jobs=1)
-
-    new_cols = sorted(new.df_featurized.columns.tolist())
-    old_cols = sorted(old.df_featurized.columns.tolist())
-
-    for i in range(len(old_cols)):
-        assert new_cols[i] == old_cols[i]
-
-    np.testing.assert_array_equal(old_cols, new_cols)
     check_column_values(new, old, tolerance=0.03)
 
 
 @pytest.mark.parametrize("featurizer_mode", ["multi", "single"])
 def test_small_moddata_composition_featurization(
     small_moddata_composition_2023, featurizer_mode
 ):
@@ -372,21 +370,14 @@
 
     featurizer = CompositionOnlyMatminer2023Featurizer()
     featurizer.featurizer_mode = featurizer_mode
 
     new = MODData(materials=compositions, featurizer=featurizer)
     new.featurize(fast=False, n_jobs=1)
 
-    new_cols = sorted(new.df_featurized.columns.tolist())
-    ref_cols = sorted(reference.df_featurized.columns.tolist())
-
-    for i in range(len(ref_cols)):
-        # print(new_cols[i], ref_cols[i])
-        assert new_cols[i] == ref_cols[i]
-
     # assert relative error below 3 percent
     check_column_values(new, reference, tolerance=0.03)
 
 
 def test_small_moddata_feature_selection_classif(small_moddata_2023):
     """This test creates classifier MODData and test the feature selection method"""
```

### Comparing `modnet-0.4.1/modnet/tests/test_sklearn.py` & `modnet-0.4.2/modnet/tests/test_sklearn.py`

 * *Files identical despite different names*

### Comparing `modnet-0.4.1/modnet/utils.py` & `modnet-0.4.2/modnet/utils.py`

 * *Files identical despite different names*

### Comparing `modnet-0.4.1/modnet.egg-info/PKG-INFO` & `modnet-0.4.2/modnet.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modnet
-Version: 0.4.1
+Version: 0.4.2
 Summary: MODNet, the Material Optimal Descriptor Network for materials properties prediction. 
 Home-page: https://github.com/ppdebreuck/modnet
 Author: Pierre-Paul De Breuck
 Author-email: pierre-paul.debreuck@uclouvain.be
 License: UNKNOWN
 Project-URL: GitHub, https://github.com/ppdebreuck/modnet
 Project-URL: Documentation, https://modnet.readthedocs.io
@@ -106,21 +106,20 @@
         
         <a name="License"></a>
         ## License
         
         MODNet is released under the MIT License.
         
 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+Provides-Extra: bayesian
 Provides-Extra: test
 Provides-Extra: dev
```

### Comparing `modnet-0.4.1/modnet.egg-info/SOURCES.txt` & `modnet-0.4.2/modnet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modnet-0.4.1/setup.py` & `modnet-0.4.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-import setuptools
 import re
 
+import setuptools
+
 with open("README.md", "r") as f:
     long_description = f.read()
 
 with open("modnet/__init__.py", "r") as f:
     lines = ""
     for item in f.readlines():
         lines += item + "\n"
 
 
 version = re.search('__version__ = "(.*)"', lines).group(1)
 
-tests_require = ("pytest>=6.0", "pytest-cov>=2.10", "flake8>=3.8")
-dev_require = ("pre-commit~=2.11",)
+tests_require = ("pytest~=8.0", "pytest-cov~=5.0", "flake8~=7.0")
+dev_require = ("pre-commit~=3.7",)
 
 setuptools.setup(
     name="modnet",
     version=version,
     author="Pierre-Paul De Breuck",
     author_email="pierre-paul.debreuck@uclouvain.be",
     description="MODNet, the Material Optimal Descriptor Network for materials properties prediction. ",
@@ -28,36 +29,32 @@
         "GitHub": "https://github.com/ppdebreuck/modnet",
         "Documentation": "https://modnet.readthedocs.io",
     },
     include_package_data=True,
     packages=setuptools.find_packages(),
     install_requires=[
         "pandas~=1.5",
-        "tensorflow~=2.10",
-        "tensorflow-probability~=0.18",
-        "pymatgen>=2022.9",
-        "matminer~=0.8",
-        "numpy>=1.20",
-        "scikit-learn~=1.1",
-        "emmet-core<0.57",  # Can remove after https://github.com/materialsproject/api/issues/819
-        "pydantic~=1.10",
+        "tensorflow~=2.10,<2.12",
+        "pymatgen>=2023",
+        "matminer~=0.9",
+        "numpy>=1.24",
+        "scikit-learn~=1.3",
     ],
     tests_require=tests_require,
     test_suite="modnet.tests",
     extras_require={
+        "bayesian": ["tensorflow-probability==0.18"],
         "test": tests_require,
         "dev": dev_require,
     },
     classifiers=[
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3",
         "Intended Audience :: Science/Research",
         "Topic :: Scientific/Engineering :: Information Analysis",
         "Topic :: Scientific/Engineering :: Physics",
         "Topic :: Scientific/Engineering :: Chemistry",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires=">=3.8",
+    python_requires=">=3.9",
 )
```

