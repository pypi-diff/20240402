# Comparing `tmp/caf.toolkit-0.7.0.tar.gz` & `tmp/caf.toolkit-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caf.toolkit-0.7.0.tar", last modified: Thu Mar  7 08:58:54 2024, max compression
+gzip compressed data, was "caf.toolkit-0.7.1.tar", last modified: Tue Apr  2 13:42:05 2024, max compression
```

## Comparing `caf.toolkit-0.7.0.tar` & `caf.toolkit-0.7.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 08:58:54.472179 caf.toolkit-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-03-07 08:58:49.000000 caf.toolkit-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6005 2024-03-07 08:58:54.472179 caf.toolkit-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-03-07 08:58:49.000000 caf.toolkit-0.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-03-07 08:58:49.000000 caf.toolkit-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-03-07 08:58:54.476179 caf.toolkit-0.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 08:58:54.464179 caf.toolkit-0.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 08:58:54.464179 caf.toolkit-0.7.0/src/caf/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 08:58:54.476179 caf.toolkit-0.7.0/src/caf/toolkit/
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-03-07 08:58:49.000000 caf.toolkit-0.7.0/src/caf/toolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7741 2024-03-07 08:58:49.000000 caf.toolkit-0.7.0/src/caf/toolkit/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-03-07 08:58:54.476179 caf.toolkit-0.7.0/src/caf/toolkit/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    10945 2024-03-07 08:58:49.000000 caf.toolkit-0.7.0/src/caf/toolkit/arguments.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 08:58:54.468179 caf.toolkit-0.7.0/src/caf/toolkit/concurrency/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-07 08:58:49.000000 caf.toolkit-0.7.0/src/caf/toolkit/concurrency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18488 2024-03-07 08:58:49.000000 caf.toolkit-0.7.0/src/caf/toolkit/concurrency/multiprocessing_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     9848 2024-03-07 08:58:49.000000 caf.toolkit-0.7.0/src/caf/toolkit/config_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 08:58:54.472179 caf.toolkit-0.7.0/src/caf/toolkit/core/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-07 08:58:49.000000 caf.toolkit-0.7.0/src/caf/toolkit/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-03-07 08:58:49.000000 caf.toolkit-0.7.0/src/caf/toolkit/core/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    19245 2024-03-07 08:58:49.000000 caf.toolkit-0.7.0/src/caf/toolkit/cost_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6787 2024-03-07 08:58:49.000000 caf.toolkit-0.7.0/src/caf/toolkit/io.py
--rw-r--r--   0 runner    (1001) docker     (127)    23533 2024-03-07 08:58:49.000000 caf.toolkit-0.7.0/src/caf/toolkit/log_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9181 2024-03-07 08:58:49.000000 caf.toolkit-0.7.0/src/caf/toolkit/math_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 08:58:54.472179 caf.toolkit-0.7.0/src/caf/toolkit/pandas_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-03-07 08:58:49.000000 caf.toolkit-0.7.0/src/caf/toolkit/pandas_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21565 2024-03-07 08:58:49.000000 caf.toolkit-0.7.0/src/caf/toolkit/pandas_utils/df_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)    13045 2024-03-07 08:58:49.000000 caf.toolkit-0.7.0/src/caf/toolkit/pandas_utils/numpy_conversions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-03-07 08:58:49.000000 caf.toolkit-0.7.0/src/caf/toolkit/pandas_utils/utility.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 08:58:49.000000 caf.toolkit-0.7.0/src/caf/toolkit/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-03-07 08:58:49.000000 caf.toolkit-0.7.0/src/caf/toolkit/timing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5341 2024-03-07 08:58:49.000000 caf.toolkit-0.7.0/src/caf/toolkit/toolbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-03-07 08:58:49.000000 caf.toolkit-0.7.0/src/caf/toolkit/tqdm_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    46719 2024-03-07 08:58:49.000000 caf.toolkit-0.7.0/src/caf/toolkit/translation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-03-07 08:58:49.000000 caf.toolkit-0.7.0/src/caf/toolkit/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 08:58:54.472179 caf.toolkit-0.7.0/src/caf.toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6005 2024-03-07 08:58:54.000000 caf.toolkit-0.7.0/src/caf.toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-03-07 08:58:54.000000 caf.toolkit-0.7.0/src/caf.toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 08:58:54.000000 caf.toolkit-0.7.0/src/caf.toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-03-07 08:58:54.000000 caf.toolkit-0.7.0/src/caf.toolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-07 08:58:54.000000 caf.toolkit-0.7.0/src/caf.toolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 08:58:54.472179 caf.toolkit-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-03-07 08:58:49.000000 caf.toolkit-0.7.0/tests/test_arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)    11457 2024-03-07 08:58:49.000000 caf.toolkit-0.7.0/tests/test_config_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    34459 2024-03-07 08:58:49.000000 caf.toolkit-0.7.0/tests/test_cost_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9101 2024-03-07 08:58:49.000000 caf.toolkit-0.7.0/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (127)    19878 2024-03-07 08:58:49.000000 caf.toolkit-0.7.0/tests/test_log_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5716 2024-03-07 08:58:49.000000 caf.toolkit-0.7.0/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)    12271 2024-03-07 08:58:49.000000 caf.toolkit-0.7.0/tests/test_math_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-03-07 08:58:49.000000 caf.toolkit-0.7.0/tests/test_timing.py
--rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-03-07 08:58:49.000000 caf.toolkit-0.7.0/tests/test_toolbox.py
--rw-r--r--   0 runner    (1001) docker     (127)    55383 2024-03-07 08:58:49.000000 caf.toolkit-0.7.0/tests/test_translation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:42:05.770882 caf.toolkit-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-04-02 13:42:01.000000 caf.toolkit-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6005 2024-04-02 13:42:05.770882 caf.toolkit-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-04-02 13:42:01.000000 caf.toolkit-0.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-04-02 13:42:01.000000 caf.toolkit-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-02 13:42:05.770882 caf.toolkit-0.7.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:42:05.762882 caf.toolkit-0.7.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:42:05.762882 caf.toolkit-0.7.1/src/caf/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:42:05.774881 caf.toolkit-0.7.1/src/caf/toolkit/
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-02 13:42:01.000000 caf.toolkit-0.7.1/src/caf/toolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7741 2024-04-02 13:42:01.000000 caf.toolkit-0.7.1/src/caf/toolkit/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-02 13:42:05.774881 caf.toolkit-0.7.1/src/caf/toolkit/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10945 2024-04-02 13:42:01.000000 caf.toolkit-0.7.1/src/caf/toolkit/arguments.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:42:05.766882 caf.toolkit-0.7.1/src/caf/toolkit/concurrency/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-02 13:42:01.000000 caf.toolkit-0.7.1/src/caf/toolkit/concurrency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18488 2024-04-02 13:42:01.000000 caf.toolkit-0.7.1/src/caf/toolkit/concurrency/multiprocessing_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9848 2024-04-02 13:42:01.000000 caf.toolkit-0.7.1/src/caf/toolkit/config_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:42:05.766882 caf.toolkit-0.7.1/src/caf/toolkit/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-02 13:42:01.000000 caf.toolkit-0.7.1/src/caf/toolkit/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-02 13:42:01.000000 caf.toolkit-0.7.1/src/caf/toolkit/core/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23129 2024-04-02 13:42:01.000000 caf.toolkit-0.7.1/src/caf/toolkit/cost_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6805 2024-04-02 13:42:01.000000 caf.toolkit-0.7.1/src/caf/toolkit/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24179 2024-04-02 13:42:01.000000 caf.toolkit-0.7.1/src/caf/toolkit/log_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9181 2024-04-02 13:42:01.000000 caf.toolkit-0.7.1/src/caf/toolkit/math_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:42:05.766882 caf.toolkit-0.7.1/src/caf/toolkit/pandas_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-02 13:42:01.000000 caf.toolkit-0.7.1/src/caf/toolkit/pandas_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21565 2024-04-02 13:42:01.000000 caf.toolkit-0.7.1/src/caf/toolkit/pandas_utils/df_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13045 2024-04-02 13:42:01.000000 caf.toolkit-0.7.1/src/caf/toolkit/pandas_utils/numpy_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-02 13:42:01.000000 caf.toolkit-0.7.1/src/caf/toolkit/pandas_utils/utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 13:42:01.000000 caf.toolkit-0.7.1/src/caf/toolkit/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-04-02 13:42:01.000000 caf.toolkit-0.7.1/src/caf/toolkit/timing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5341 2024-04-02 13:42:01.000000 caf.toolkit-0.7.1/src/caf/toolkit/toolbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-02 13:42:01.000000 caf.toolkit-0.7.1/src/caf/toolkit/tqdm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52038 2024-04-02 13:42:01.000000 caf.toolkit-0.7.1/src/caf/toolkit/translation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-02 13:42:01.000000 caf.toolkit-0.7.1/src/caf/toolkit/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:42:05.770882 caf.toolkit-0.7.1/src/caf.toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6005 2024-04-02 13:42:05.000000 caf.toolkit-0.7.1/src/caf.toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-02 13:42:05.000000 caf.toolkit-0.7.1/src/caf.toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 13:42:05.000000 caf.toolkit-0.7.1/src/caf.toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-02 13:42:05.000000 caf.toolkit-0.7.1/src/caf.toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-02 13:42:05.000000 caf.toolkit-0.7.1/src/caf.toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:42:05.770882 caf.toolkit-0.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-02 13:42:01.000000 caf.toolkit-0.7.1/tests/test_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11457 2024-04-02 13:42:01.000000 caf.toolkit-0.7.1/tests/test_config_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40119 2024-04-02 13:42:01.000000 caf.toolkit-0.7.1/tests/test_cost_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9101 2024-04-02 13:42:01.000000 caf.toolkit-0.7.1/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21442 2024-04-02 13:42:01.000000 caf.toolkit-0.7.1/tests/test_log_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5716 2024-04-02 13:42:01.000000 caf.toolkit-0.7.1/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12271 2024-04-02 13:42:01.000000 caf.toolkit-0.7.1/tests/test_math_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-04-02 13:42:01.000000 caf.toolkit-0.7.1/tests/test_timing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-04-02 13:42:01.000000 caf.toolkit-0.7.1/tests/test_toolbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63860 2024-04-02 13:42:01.000000 caf.toolkit-0.7.1/tests/test_translation.py
```

### Comparing `caf.toolkit-0.7.0/LICENSE` & `caf.toolkit-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.7.0/PKG-INFO` & `caf.toolkit-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caf.toolkit
-Version: 0.7.0
+Version: 0.7.1
 Summary: A toolkit of transport planning and appraisal functionalities
 Author: Transport for the North
 License: Copyright © Transport for the North (“TfN”) (2023).
         
         
         Use of this software and associated documentation files (“the Software”) by you indicates your acceptance of the terms and conditions below (“the Licence”).
         We make available the Software to you on the basis of this Licence. We do not sell the Software to you. We remain the owners of the Software at all times.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: caf.toolkit Version: 0.7.0 Summary: A toolkit of
+Metadata-Version: 2.1 Name: caf.toolkit Version: 0.7.1 Summary: A toolkit of
 transport planning and appraisal functionalities Author: Transport for the
 North License: Copyright Â© Transport for the North (âTfNâ) (2023). Use of
 this software and associated documentation files (âthe Softwareâ) by you
 indicates your acceptance of the terms and conditions below (âthe
 Licenceâ). We make available the Software to you on the basis of this
 Licence. We do not sell the Software to you. We remain the owners of the
 Software at all times. We grant you a non-exclusive, worldwide, royalty-free,
```

### Comparing `caf.toolkit-0.7.0/README.md` & `caf.toolkit-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.7.0/pyproject.toml` & `caf.toolkit-0.7.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -107,14 +107,15 @@
     "D202",    # Temporary compatibility with black
 ]
 
 # Tests
 [tool.pytest.ini_options]
 pythonpath = ["src"]
 addopts = '--cov=caf --cov-report=xml --doctest-modules -n auto'
+# addopts = '--cov=caf --cov-report=xml --doctest-modules'
 doctest_optionflags = "NORMALIZE_WHITESPACE"
 markers = [
     "serial: marks tests to not run in parallel",
 ]
 
 [tool.coverage.report]
 include_namespace_packages = true
```

### Comparing `caf.toolkit-0.7.0/src/caf/toolkit/__init__.py` & `caf.toolkit-0.7.1/src/caf/toolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.7.0/src/caf/toolkit/__main__.py` & `caf.toolkit-0.7.1/src/caf/toolkit/__main__.py`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.7.0/src/caf/toolkit/arguments.py` & `caf.toolkit-0.7.1/src/caf/toolkit/arguments.py`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.7.0/src/caf/toolkit/concurrency/multiprocessing_wrapper.py` & `caf.toolkit-0.7.1/src/caf/toolkit/concurrency/multiprocessing_wrapper.py`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.7.0/src/caf/toolkit/config_base.py` & `caf.toolkit-0.7.1/src/caf/toolkit/config_base.py`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.7.0/src/caf/toolkit/cost_utils.py` & `caf.toolkit-0.7.1/src/caf/toolkit/cost_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -49,23 +49,27 @@
         Average values for each of the cost distribution bins.
 
     trip_vals:
         Trip values for each of the cost distribution bins.
 
     band_share_vals:
         Band share values for each of the cost distribution bins.
+
+    weighted_avg_vals:
+        Weighted average values for each of the cost distribution bins.
     """
 
     df: pd.DataFrame
 
     # Default arguments
     min_col: str = "min"
     max_col: str = "max"
     avg_col: str = "ave"
     trips_col: str = "trips"
+    weighted_avg_col: str = "weighted_ave"
 
     # Ideas
     units: str = "km"
 
     @pydantic.model_validator(mode="after")
     def check_df_col_names(self) -> CostDistribution:
         """Check the given columns are in the given dataframe."""
@@ -75,24 +79,29 @@
 
         # Check columns are in df
         err_cols = {}
         for col_name, col_val in cols.items():
             if col_val not in self.df:
                 err_cols.update({col_name: col_val})
 
+        # Add in the weighted_avg_col if not already in df
+        cols.update({"weighted_avg_col": getattr(self, "weighted_avg_col")})
+        if self.weighted_avg_col not in self.df.columns:
+            self.df[self.weighted_avg_col] = self.df[self.avg_col]
+
         # Throw error if missing columns found
         if err_cols != dict():
             raise ValueError(
                 "Not all the given column names exist in the given df. "
                 f"The following columns are missing:{err_cols}\n"
                 f"With the following in the Df: {self.df.columns}"
             )
 
         # Tidy up df
-        self.df = pd_utils.reindex_cols(self.df, cols.values())
+        self.df = pd_utils.reindex_cols(self.df, list(cols.values()))
         return self
 
     def __len__(self):
         """Get the number of bins in this cost distribution."""
         return len(self.bin_edges) - 1
 
     def __eq__(self, other):
@@ -137,14 +146,54 @@
 
     @property
     def band_share_vals(self) -> np.ndarray:
         """Band share values for each of the cost distribution bins."""
         trip_vals = self.trip_vals
         return trip_vals / np.sum(trip_vals)
 
+    @staticmethod
+    def calculate_weighted_averages(
+        matrix: np.ndarray, cost_matrix: np.ndarray, bin_edges: list[float] | np.ndarray
+    ):
+        """
+        Calculate weighted averages of bins in a cost distribution.
+
+        Parameters
+        ----------
+        matrix: np.ndarray
+            The matrix to calculate the cost distribution for. This matrix
+            should be the same shape as cost_matrix
+
+        cost_matrix: np.ndarray
+            A matrix of cost relating to matrix. This matrix
+            should be the same shape as matrix
+
+        bin_edges: list[float] | np.ndarray
+            Defines a monotonically increasing array of bin edges, including the
+            rightmost edge, allowing for non-uniform bin widths. This argument
+            is passed straight into `numpy.histogram`
+
+        Returns
+        -------
+        np.ndarray
+            An array to be passed into a dataframe as a column.
+        """
+        df = pd.DataFrame(
+            {
+                "cost": pd.DataFrame(cost_matrix).stack(),
+                "demand": pd.DataFrame(matrix).stack(),
+            }
+        )
+        df["bin"] = pd.cut(df["cost"], bins=bin_edges)
+        df["weighted"] = df["cost"] * df["demand"]
+        grouped = df.groupby("bin", observed=False)[["weighted", "demand"]].sum().reset_index()
+        grouped["bin_centres"] = grouped["bin"].apply(lambda x: x.mid)
+        grouped["averages"] = grouped["weighted"] / grouped["demand"]
+        return grouped["averages"].fillna(grouped["bin_centres"].astype("float")).to_numpy()
+
     @classmethod
     def from_data(
         cls,
         matrix: np.ndarray,
         cost_matrix: np.ndarray,
         min_bounds: Optional[list[float] | np.ndarray] = None,
         max_bounds: Optional[list[float] | np.ndarray] = None,
@@ -190,21 +239,24 @@
             min_bounds=min_bounds,
             max_bounds=max_bounds,
         )
         distribution = cost_distribution(
             matrix=matrix, cost_matrix=cost_matrix, bin_edges=bin_edges
         )
 
+        averages = cls.calculate_weighted_averages(matrix, cost_matrix, bin_edges)
+
         # Covert data into instance of this class
         df = pd.DataFrame(
             {
                 cls.min_col: bin_edges[:-1],
                 cls.max_col: bin_edges[1:],
                 cls.avg_col: (np.array(bin_edges[:-1]) + np.array(bin_edges[1:])) / 2,
                 cls.trips_col: distribution,
+                cls.weighted_avg_col: averages,
             }
         )
         return CostDistribution(df=df)
 
     @staticmethod
     def from_data_no_bins(
         matrix: np.ndarray,
@@ -248,14 +300,15 @@
     @staticmethod
     def from_file(
         filepath: os.PathLike,
         min_col: str = "min",
         max_col: str = "max",
         avg_col: str = "ave",
         trips_col: str = "trips",
+        weighted_avg_col: str = "weighted_ave",
     ) -> CostDistribution:
         """Build an instance from a file on disk.
 
         Parameters
         ----------
         filepath:
             Path to the file to read in.
@@ -272,28 +325,34 @@
             The column of data at `filepath` that contains the average cost
             value of each band.
 
         trips_col:
             The column of data at `filepath` that contains the number of trips
             of each cost band.
 
+        weighted_avg_col:
+            The column of data at 'filepath' that contains the weighted average
+            cost value of each band. If the read in df does not contain this
+            column, it will default to the avg_col.
+
         Returns
         -------
         cost_distribution:
             An instance containing the data at filepath.
         """
         if not os.path.isfile(filepath):
             raise ValueError(f"'{filepath}' is not the location of a file.")
-        use_cols = [min_col, max_col, avg_col, trips_col]
+        use_cols = [min_col, max_col, avg_col, trips_col, weighted_avg_col]
         return CostDistribution(
             df=pd.read_csv(filepath, usecols=use_cols),
             min_col=min_col,
             max_col=max_col,
             avg_col=avg_col,
             trips_col=trips_col,
+            weighted_avg_col=weighted_avg_col,
         )
 
     def __validate_similar_bin_edges(self, other: CostDistribution) -> None:
         """Check whether other is using the same bins as self.
 
         Parameters
         ----------
@@ -638,7 +697,51 @@
     n_bins = int(max_value**n_bin_pow)
     bins = (np.array(range(2, n_bins + 1)) / n_bins) ** log_factor * max_value
     bins = np.floor(bins)
 
     # Add the first and last item
     bins = np.insert(bins, 0, 0)
     return np.insert(bins, len(bins), final_val)
+
+
+def intrazonal_cost_infill(
+    cost: np.ndarray,
+    multiplier: float = 0.5,
+    min_axis: int = 1,
+) -> np.ndarray:
+    """
+    Infill the intra-zonal costs of a cost matrix.
+
+    The intra-zonal costs are usually the diagonal of a cost matrix. Standard
+    TAG procedure for infilling these costs is to take half the minimum cost
+    for each zone. By default, this function takes the minimum value from each
+    row (ignoring 0s) and multiplies that by 0.5 to get the infill value for
+    each intra-zonal. Note that if any costs already exist for the
+    intra-zonals, they will be overwritten.
+    The diagonal infill is calculated similar to:
+    `cost.min(axis=min_axis * multiplier`
+
+    Parameters
+    ----------
+    cost:
+        The square, 2D cost matrix to infill.
+
+    multiplier:
+        The value to multiply the minimum values by to calculate the infill value.
+
+    min_axis:
+        The axis to calculate the minimum value across.
+
+    Returns
+    -------
+    infilled_cost:
+        A copy of the input `cost`, but with the diagonal infilled.
+    """
+    # Ensure we don't pick up the diagonals or 0s in the minimum check
+    nonzero_cost = np.where(cost == 0, np.inf, cost)
+    np.fill_diagonal(nonzero_cost, np.inf)
+
+    # Infill a copy of cost
+    infill = nonzero_cost.min(axis=min_axis) * multiplier
+    infilled_cost = cost.copy()
+    np.fill_diagonal(infilled_cost, infill)
+    return infilled_cost
```

### Comparing `caf.toolkit-0.7.0/src/caf/toolkit/io.py` & `caf.toolkit-0.7.1/src/caf/toolkit/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,21 +126,21 @@
         if match:
             raise MissingColumnsError(name, [match.group(1)]) from err
 
         if isinstance(kwargs.get("dtype"), dict):
             # Check what column can't be converted to dtypes
             columns: dict[str, type] = kwargs.pop("dtype")
             df = pd.read_csv(path, **kwargs)
-            for c, t in columns.items():
+            for col, _type in columns.items():
                 try:
-                    df[c].astype(t)
+                    df[col].astype(_type)
                 except ValueError:
                     raise ValueError(
-                        f"Column '{c}' in {name} has values "
-                        f"which cannot be converted to {t}"
+                        f"Column '{col}' in {name} has values "
+                        f"which cannot be converted to {_type}"
                     ) from err
         raise
 
     return df
 
 
 def read_csv_matrix(
```

### Comparing `caf.toolkit-0.7.0/src/caf/toolkit/log_helpers.py` & `caf.toolkit-0.7.1/src/caf/toolkit/log_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 # Built-Ins
 import functools
 import getpass
 import logging
 import os
 import platform
+import warnings
 from typing import Annotated, Any, Iterable, Optional
 
 # Third Party
 import psutil
 import pydantic
 from psutil import _common
 from pydantic import dataclasses, types
@@ -42,14 +43,20 @@
     r"(?:-(?P<prerelease>(?:0|[1-9]\d*|\d*[a-zA-Z-][0-9a-zA-Z-]*)"
     r"(?:\.(?:0|[1-9]\d*|\d*[a-zA-Z-][0-9a-zA-Z-]*))*))?"
     r"(?:\+(?P<buildmetadata>[0-9a-zA-Z-]+(?:\.[0-9a-zA-Z-]+)*))?$"
 )
 
 
 # # # CLASSES # # #
+
+
+class LoggingWarning(Warning):
+    """Warnings from the `LogHelper` and other toolkit logging functionality."""
+
+
 @dataclasses.dataclass
 class ToolDetails:
     """Information about the current tool.
 
     Attributes
     ----------
     name: str
@@ -257,26 +264,48 @@
         self.logger = logging.getLogger(self.logger_name)
         self.logger.setLevel(logging.DEBUG)
 
         self.tool_details = tool_details
         self._warning_logger: logging.Logger | None = None
 
         if console:
-            handler = get_console_handler()
-            self.logger.addHandler(handler)
+            self.add_console_handler()
 
         if log_file is not None:
-            handler = get_file_handler(log_file)
-            self.logger.addHandler(handler)
+            self.add_file_handler(log_file)
 
-        self.write_instantiate_message()
+        if len(self.logger.handlers) > 0:
+            self.write_instantiate_message()
+        else:
+            warnings.warn(
+                "LogHelper initialised without any logging handlers, "
+                "`logging.basicConfig` will be called with default parameters "
+                "at first log attempt if no handlers are added before that.",
+                LoggingWarning,
+            )
 
         if warning_capture:
             self.capture_warnings()
 
+    def add_handler(self, handler: logging.Handler) -> None:
+        """Add custom `handler` to the logger.
+
+        This will also add handler to the warnings logger if
+        warnings capture is enabled.
+
+        Parameters
+        ----------
+        handler : logging.Handler
+            Handler to add.
+        """
+        self.logger.addHandler(handler)
+
+        if self._warning_logger is not None:
+            self._warning_logger.addHandler(handler)
+
     def add_console_handler(
         self,
         ch_format: str = DEFAULT_CONSOLE_FORMAT,
         datetime_format: str = DEFAULT_CONSOLE_DATETIME,
         log_level: int = logging.INFO,
     ) -> None:
         """Add custom console handler to the logger.
@@ -295,18 +324,15 @@
             The logging level to give to the StreamHandler.
 
         See Also
         --------
         `get_console_handler`
         """
         handler = get_console_handler(ch_format, datetime_format, log_level)
-        self.logger.addHandler(handler)
-
-        if self._warning_logger is not None:
-            self._warning_logger.addHandler(handler)
+        self.add_handler(handler)
 
     def add_file_handler(
         self,
         log_file: os.PathLike,
         fh_format: str = DEFAULT_FILE_FORMAT,
         datetime_format: str = DEFAULT_FILE_DATETIME,
         log_level: int = logging.DEBUG,
@@ -331,18 +357,15 @@
             The logging level to give to the FileHandler.
 
         See Also
         --------
         `get_file_handler`
         """
         handler = get_file_handler(log_file, fh_format, datetime_format, log_level)
-        self.logger.addHandler(handler)
-
-        if self._warning_logger is not None:
-            self._warning_logger.addHandler(handler)
+        self.add_handler(handler)
 
     def capture_warnings(self) -> None:
         """Capture warnings using logging.
 
         Runs `logging.captureWarnings(True)` to capture warnings then
         adds all the handlers from the root `logger`.
```

### Comparing `caf.toolkit-0.7.0/src/caf/toolkit/math_utils.py` & `caf.toolkit-0.7.1/src/caf/toolkit/math_utils.py`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.7.0/src/caf/toolkit/pandas_utils/df_handling.py` & `caf.toolkit-0.7.1/src/caf/toolkit/pandas_utils/df_handling.py`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.7.0/src/caf/toolkit/pandas_utils/numpy_conversions.py` & `caf.toolkit-0.7.1/src/caf/toolkit/pandas_utils/numpy_conversions.py`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.7.0/src/caf/toolkit/pandas_utils/utility.py` & `caf.toolkit-0.7.1/src/caf/toolkit/pandas_utils/utility.py`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.7.0/src/caf/toolkit/timing.py` & `caf.toolkit-0.7.1/src/caf/toolkit/timing.py`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.7.0/src/caf/toolkit/toolbox.py` & `caf.toolkit-0.7.1/src/caf/toolkit/toolbox.py`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.7.0/src/caf/toolkit/tqdm_utils.py` & `caf.toolkit-0.7.1/src/caf/toolkit/tqdm_utils.py`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.7.0/src/caf/toolkit/translation.py` & `caf.toolkit-0.7.1/src/caf/toolkit/translation.py`

 * *Files 2% similar despite different names*

```diff
@@ -230,22 +230,22 @@
             f"Some zones in `{name}.index` have not been defined in "
             f"`row_translation`. These zones will be dropped before "
             f"translating.\n"
             f"Additional rows count: {len(missing_rows)}\n"
             f"Total value dropped: {total_value_dropped}"
         )
 
-    # Throw a warning if any index values are in the matrix, but not in the
+    # Throw a warning if any column values are in the matrix, but not in the
     # col_translation. These values will just be dropped.
     translation_from = col_translation[translation_from_col].unique()
-    missing_cols = set(matrix.index.to_list()) - set(translation_from)
+    missing_cols = set(matrix.columns.to_list()) - set(translation_from)
     if len(missing_cols) > 0:
         total_value_dropped = matrix[list(missing_cols)].to_numpy().sum()
         warnings.warn(
-            f"Some zones in `{name}.index` have not been defined in "
+            f"Some zones in `{name}.columns` have not been defined in "
             f"`col_translation`. These zones will be dropped before "
             f"translating.\n"
             f"Additional rows count: {len(missing_cols)}\n"
             f"Total value dropped: {total_value_dropped}"
         )
 
 
@@ -313,14 +313,15 @@
 
     Raises
     ------
     ValueError:
         Will raise an error if matrix is not a square array, or if translation
         does not have the same number of rows as matrix.
     """
+    # pylint: disable=too-many-locals
     # Init
     translation_from_col = "from_id"
     translation_to_col = "to_id"
     translation_factors_col = "factors"
 
     # ## OPTIONALLY CHECK INPUT SHAPES ## #
     row_translation = translation
@@ -339,17 +340,22 @@
     to_id_vals = list(range(translation.shape[1]))
 
     # Convert numpy arrays into pandas arrays
     dimension_cols = {translation_from_col: from_id_vals, translation_to_col: to_id_vals}
     pd_row_translation = pd_utils.n_dimensional_array_to_dataframe(
         mat=row_translation, dimension_cols=dimension_cols, value_col=translation_factors_col
     ).reset_index()
+    zero_mask = pd_row_translation[translation_factors_col] == 0
+    pd_row_translation = pd_row_translation[~zero_mask]
+
     pd_col_translation = pd_utils.n_dimensional_array_to_dataframe(
         mat=col_translation, dimension_cols=dimension_cols, value_col=translation_factors_col
     ).reset_index()
+    zero_mask = pd_col_translation[translation_factors_col] == 0
+    pd_col_translation = pd_col_translation[~zero_mask]
 
     return pandas_matrix_zone_translation(
         matrix=pd.DataFrame(data=matrix, columns=from_id_vals, index=from_id_vals),
         translation=pd_row_translation,
         col_translation=pd_col_translation,
         translation_from_col=translation_from_col,
         translation_to_col=translation_to_col,
@@ -477,26 +483,159 @@
             f"Before: {vector.sum()}\n"
             f"After: {out_vector.sum()}"
         )
 
     return out_vector
 
 
+def pandas_long_matrix_zone_translation(
+    matrix: pd.DataFrame,
+    index_col_1_name: str,
+    index_col_2_name: str,
+    values_col: str,
+    translation: pd.DataFrame,
+    translation_from_col: str,
+    translation_to_col: str,
+    translation_factors_col: str,
+    col_translation: Optional[pd.DataFrame] = None,
+    translation_dtype: Optional[np.dtype] = None,
+    index_col_1_out_name: Optional[str] = None,
+    index_col_2_out_name: Optional[str] = None,
+    check_totals: bool = True,
+) -> pd.DataFrame:
+    """Efficiently translates a pandas matrix between index systems.
+
+    Parameters
+    ----------
+    matrix:
+        The matrix to translate, in long format. Must contain columns:
+        [`index_col_1_name`, `index_col_2_name`, `value_col`].
+
+    index_col_1_name:
+        The name of the first column in `matrix` to translate index system.
+
+    index_col_2_name:
+        The name of the second column in `matrix` to translate index system.
+
+    values_col:
+        The name of the column in `matrix` detailing the values to translate.
+
+    translation:
+        A pandas DataFrame defining the weights to use when translating.
+        Needs to contain columns:
+        `translation_from_col`, `translation_to_col`, `translation_factors_col`.
+        When `col_translation` is None, this defines the translation to use
+        for both the rows and columns. When `col_translation` is set, this
+        defines the translation to use for the rows.
+
+    col_translation:
+        A matrix defining the weights to use to translate the columns.
+        Takes an input of the same format as `translation`. When None,
+        `translation` is used as the column translation.
+
+    translation_from_col:
+        The name of the column in `translation` and `col_translation`
+        containing the current index and column values of `matrix`.
+
+    translation_to_col:
+        The name of the column in `translation` and `col_translation`
+        containing the desired output index and column values. This
+        will define the output index and column format.
+
+    translation_factors_col:
+        The name of the column in `translation` and `col_translation`
+        containing the translation weights between `translation_from_col` and
+        `translation_to_col`. Where zone pairs do not exist, they will be
+        infilled with `translate_infill`.
+
+    translation_dtype:
+        The numpy datatype to use to do the translation. If None, then the
+        dtype of `vector` is used. Where such high precision
+        isn't needed, a more memory and time efficient data type can be used.
+
+    check_totals:
+        Whether to check that the input and output matrices sum to the same
+        total.
+
+    index_col_1_out_name:
+        The name to give to `index_col_1_name` on return.
+
+    index_col_2_out_name:
+        The name to give to `index_col_2_name` on return.
+
+    Returns
+    -------
+    translated_matrix:
+        matrix, translated into to_unique_index system.
+
+    Raises
+    ------
+    ValueError:
+        If matrix is not a square array, or if translation any inputs are not
+        the correct format.
+    """
+    # pylint: disable=too-many-arguments, too-many-locals
+    # Init
+    keep_cols = [index_col_1_name, index_col_2_name, values_col]
+    all_cols = matrix.columns.tolist()
+
+    if index_col_1_out_name is None:
+        index_col_1_out_name = index_col_1_name
+    if index_col_2_out_name is None:
+        index_col_2_out_name = index_col_2_name
+
+    # Drop any columns we're not keeping
+    drop_cols = set(all_cols) - set(keep_cols)
+    if len(drop_cols) > 0:
+        warnings.warn(f"Extra columns found in matrix, dropping the following: {drop_cols}")
+    matrix = pd_utils.reindex_cols(df=matrix, columns=keep_cols)
+
+    # Convert to wide to translate
+    wide_mat = pd_utils.long_to_wide_infill(
+        df=matrix,
+        index_col=index_col_1_name,
+        columns_col=index_col_2_name,
+        values_col=values_col,
+    )
+
+    translated_wide_mat = pandas_matrix_zone_translation(
+        matrix=wide_mat,
+        translation=translation,
+        translation_from_col=translation_from_col,
+        translation_to_col=translation_to_col,
+        translation_factors_col=translation_factors_col,
+        col_translation=col_translation,
+        translation_dtype=translation_dtype,
+        check_totals=check_totals,
+    )
+
+    # Convert back
+    return pd_utils.wide_to_long_infill(
+        df=translated_wide_mat,
+        index_col_1_name=index_col_1_out_name,
+        index_col_2_name=index_col_2_out_name,
+        value_col_name=values_col,
+    )
+
+
 def pandas_matrix_zone_translation(
     matrix: pd.DataFrame,
     translation: pd.DataFrame,
     translation_from_col: str,
     translation_to_col: str,
     translation_factors_col: str,
     col_translation: Optional[pd.DataFrame] = None,
     translation_dtype: Optional[np.dtype] = None,
     check_totals: bool = True,
 ) -> pd.DataFrame:
     """Efficiently translates a pandas matrix between index systems.
 
+    Only works on wide matrices and not long. If translating long matrices,
+    use `pandas_long_matrix_zone_translation` instead.
+
     Parameters
     ----------
     matrix:
         The matrix to translate. The index and columns need to be the
         values being translated. This CANNOT be a "long" matrix.
 
     translation:
@@ -553,19 +692,21 @@
     if col_translation is None:
         col_translation = translation.copy()
     assert col_translation is not None
 
     # Set the index dtypes to match and validate
     (
         matrix.index,
+        matrix.columns,
         row_translation[translation_from_col],
         col_translation[translation_from_col],
     ) = pd_utils.cast_to_common_type(
         [
             matrix.index,
+            matrix.columns,
             row_translation[translation_from_col],
             col_translation[translation_from_col],
         ]
     )
 
     _pandas_matrix_validation(
         matrix=matrix,
@@ -576,27 +717,32 @@
 
     # Build dictionary of repeated kwargs
     common_kwargs: _MultiVectorKwargs = {
         "translation_from_col": translation_from_col,
         "translation_to_col": translation_to_col,
         "translation_factors_col": translation_factors_col,
         "translation_dtype": translation_dtype,
-        "check_totals": check_totals,
+        "check_totals": False,
     }
 
-    half_done = pandas_multi_vector_zone_translation(
-        vector=matrix,
-        translation=row_translation,
-        **common_kwargs,
-    )
-    translated = pandas_multi_vector_zone_translation(
-        vector=half_done.transpose(),
-        translation=col_translation,
-        **common_kwargs,
-    ).transpose()
+    with warnings.catch_warnings():
+        # Ignore the warnings we've already checked for
+        msg = ".*zones will be dropped.*"
+        warnings.filterwarnings(action="ignore", message=msg, category=UserWarning)
+
+        half_done = pandas_multi_vector_zone_translation(
+            vector=matrix,
+            translation=row_translation,
+            **common_kwargs,
+        )
+        translated = pandas_multi_vector_zone_translation(
+            vector=half_done.transpose(),
+            translation=col_translation,
+            **common_kwargs,
+        ).transpose()
 
     if not check_totals:
         return translated
 
     if not math_utils.is_almost_equal(matrix.to_numpy().sum(), translated.to_numpy().sum()):
         raise ValueError(
             f"Some values seem to have been dropped during the translation. "
@@ -1033,21 +1179,21 @@
             raise ValueError(
                 "The input vector is MultiIndexed and does not "
                 f"contain the expected column, {translation_from_col}."
                 "Either rename the correct index level, or input "
                 "a vector with a single index to use."
             )
     else:
+        vector.index, translation[translation_from_col] = pd_utils.cast_to_common_type(
+            [vector.index, translation[translation_from_col]],
+        )
         missing_rows = set(vector.index.to_list()) - set(translation_from)
         if len(missing_rows) > 0:
             _vector_missing_warning(vector, list(missing_rows))
 
-        vector.index, translation[translation_from_col] = pd_utils.cast_to_common_type(
-            [vector.index, translation[translation_from_col]],
-        )
         # Doesn't matter if it already equals this, quicker than checking.
         vector.index.names = [translation_from_col]
         ind_names = []
 
     # trans_vector should now contain the correct index level if an error hasn't
     # been raised
     translated = (
```

### Comparing `caf.toolkit-0.7.0/src/caf/toolkit/validators.py` & `caf.toolkit-0.7.1/src/caf/toolkit/validators.py`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.7.0/src/caf.toolkit.egg-info/PKG-INFO` & `caf.toolkit-0.7.1/src/caf.toolkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caf.toolkit
-Version: 0.7.0
+Version: 0.7.1
 Summary: A toolkit of transport planning and appraisal functionalities
 Author: Transport for the North
 License: Copyright © Transport for the North (“TfN”) (2023).
         
         
         Use of this software and associated documentation files (“the Software”) by you indicates your acceptance of the terms and conditions below (“the Licence”).
         We make available the Software to you on the basis of this Licence. We do not sell the Software to you. We remain the owners of the Software at all times.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: caf.toolkit Version: 0.7.0 Summary: A toolkit of
+Metadata-Version: 2.1 Name: caf.toolkit Version: 0.7.1 Summary: A toolkit of
 transport planning and appraisal functionalities Author: Transport for the
 North License: Copyright Â© Transport for the North (âTfNâ) (2023). Use of
 this software and associated documentation files (âthe Softwareâ) by you
 indicates your acceptance of the terms and conditions below (âthe
 Licenceâ). We make available the Software to you on the basis of this
 Licence. We do not sell the Software to you. We remain the owners of the
 Software at all times. We grant you a non-exclusive, worldwide, royalty-free,
```

### Comparing `caf.toolkit-0.7.0/src/caf.toolkit.egg-info/SOURCES.txt` & `caf.toolkit-0.7.1/src/caf.toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.7.0/tests/test_arguments.py` & `caf.toolkit-0.7.1/tests/test_arguments.py`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.7.0/tests/test_config_base.py` & `caf.toolkit-0.7.1/tests/test_config_base.py`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.7.0/tests/test_cost_utils.py` & `caf.toolkit-0.7.1/tests/test_cost_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -37,14 +37,17 @@
         self.min_bounds = self.bin_edges[:-1]
         self.max_bounds = self.bin_edges[1:]
 
         if self.distribution.sum() == 0:
             self.normalised_distribution = np.zeros_like(self.distribution)
         else:
             self.normalised_distribution = self.distribution / self.distribution.sum()
+            self.weighted_avg = cost_utils.CostDistribution.calculate_weighted_averages(
+                matrix=self.matrix, cost_matrix=self.cost_matrix, bin_edges=self.bin_edges
+            )
 
 
 @dataclasses.dataclass
 class DynamicCostDistFnResults(CostDistFnResults):
     """Inputs and expected results for a cost_distribution function"""
 
     # Inputs
@@ -68,33 +71,36 @@
     """Inputs and expected results for a CostDistribution class."""
 
     # Inputs
     min_col: str = "min"
     max_col: str = "max"
     avg_col: str = "ave"
     trips_col: str = "trips"
+    weighted_avg_col: str = "weighted_ave"
 
     def __post_init__(self):
         super().__post_init__()
 
         self.avg_bounds = (self.min_bounds + self.max_bounds) / 2
         self.df = pd.DataFrame(
             {
                 self.min_col: self.min_bounds,
                 self.max_col: self.max_bounds,
                 self.avg_col: self.avg_bounds,
                 self.trips_col: self.distribution,
+                self.weighted_avg_col: self.weighted_avg,
             }
         )
         self.normalised_df = pd.DataFrame(
             {
                 self.min_col: self.min_bounds,
                 self.max_col: self.max_bounds,
                 self.avg_col: self.avg_bounds,
                 self.trips_col: self.normalised_distribution,
+                self.weighted_avg_col: self.weighted_avg,
             }
         )
 
         self.cost_dist_instance = cost_utils.CostDistribution(**self.constructor_kwargs)
 
     @property
     def constructor_kwargs(self) -> dict[str, Any]:
@@ -111,14 +117,15 @@
     def default_name_df(self) -> pd.DataFrame:
         """Get the internal pandas dataframe using the default col names."""
         naming_dict = {
             self.min_col: "min",
             self.max_col: "max",
             self.avg_col: "ave",
             self.trips_col: "trips",
+            self.weighted_avg_col: "weighted_ave",
         }
         return self.df.rename(columns=naming_dict)
 
 
 @dataclasses.dataclass
 class DynamicCostDistClassResults(CostDistClassResults, DynamicCostDistFnResults):
     """Inputs and expected results for a CostDistribution class w/ dynamic bounds."""
@@ -348,14 +355,24 @@
     )
     def test_correct_init(self, io_str: str, request):
         """Test the class constructor creates the correct DF internally."""
         input_and_results: CostDistClassResults = request.getfixturevalue(io_str)
         cost_dist = cost_utils.CostDistribution(**input_and_results.constructor_kwargs)
         pd.testing.assert_frame_equal(cost_dist.df, input_and_results.df)
 
+    def test_default_weighted_average(self, cost_dist_1d_class):
+        dist_df = cost_utils.CostDistribution(**cost_dist_1d_class.constructor_kwargs).df.drop(
+            "weighted_ave", axis=1
+        )
+        test_dist = cost_utils.CostDistribution(dist_df).df
+        ave_col = test_dist["ave"]
+        weight_col = test_dist["weighted_ave"]
+        weight_col.name = "ave"
+        pd.testing.assert_series_equal(ave_col, weight_col)
+
     @pytest.mark.parametrize(
         "io_str",
         ["cost_dist_1d_class", "cost_dist_2d_class", "cost_dist_2d_class_cols"],
     )
     def test_init_wrong_col(self, io_str: str, request):
         """Test the class constructor throws errors with bad column names."""
         input_and_results: CostDistClassResults = request.getfixturevalue(io_str)
@@ -876,7 +893,146 @@
     )
     def test_kwarg_passing(self, dist_str: str, request):
         """Check that the expected distribution is returned."""
         cost_dist: DynamicCostDistFnResults = request.getfixturevalue(dist_str)
         result, bins = cost_utils.dynamic_cost_distribution(**cost_dist.get_kwargs())
         np.testing.assert_almost_equal(result, cost_dist.distribution)
         np.testing.assert_almost_equal(bins, cost_dist.bin_edges)
+
+
+class TestIntrazonalCostInfill:
+    """Tests for the intrazonal_cost_infill function"""
+
+    @dataclasses.dataclass
+    class IzResults:
+        """Inputs and expected results for intrazonal_cost_infill()"""
+
+        # Inputs
+        cost_matrix: np.ndarray
+        multiplier: float
+        min_axis: int
+
+        # Results
+        result: np.ndarray
+
+        def get_kwargs(self) -> dict[str, Any]:
+            return {
+                "cost": self.cost_matrix,
+                "multiplier": self.multiplier,
+                "min_axis": self.min_axis,
+            }
+
+    @pytest.fixture(name="normal_array", scope="class")
+    def fixture_normal_array(self):
+        """Create a simple test with no edge cases"""
+        cost_matrix = np.array(
+            [
+                [54.0, 72.0, 61.0, 97.0, 72.0],
+                [41.0, 84.0, 98.0, 32.0, 32.0],
+                [4.0, 33.0, 67.0, 14.0, 26.0],
+                [73.0, 46.0, 14.0, 8.0, 51.0],
+                [2.0, 14.0, 58.0, 53.0, 40.0],
+            ]
+        )
+        result = np.array(
+            [
+                [61.0, 72.0, 61.0, 97.0, 72.0],
+                [41.0, 32.0, 98.0, 32.0, 32.0],
+                [4.0, 33.0, 4.0, 14.0, 26.0],
+                [73.0, 46.0, 14.0, 14.0, 51.0],
+                [2.0, 14.0, 58.0, 53.0, 2.0],
+            ]
+        )
+        return self.IzResults(
+            cost_matrix=cost_matrix,
+            multiplier=1,
+            min_axis=1,
+            result=result,
+        )
+
+    @pytest.fixture(name="min_axis_array", scope="class")
+    def fixture_min_axis_array(self, normal_array):
+        """Test for min across columns (different min_axis)."""
+        result = np.array(
+            [
+                [2.0, 72.0, 61.0, 97.0, 72.0],
+                [41.0, 14.0, 98.0, 32.0, 32.0],
+                [4.0, 33.0, 14.0, 14.0, 26.0],
+                [73.0, 46.0, 14.0, 14.0, 51.0],
+                [2.0, 14.0, 58.0, 53.0, 26.0],
+            ]
+        )
+        return self.IzResults(
+            cost_matrix=normal_array.cost_matrix,
+            multiplier=1,
+            min_axis=0,
+            result=result,
+        )
+
+    @pytest.fixture(name="zeroes_array", scope="class")
+    def fixture_zeroes_array(self, normal_array):
+        """zero values should be returned in-place, expect in diagonal.
+
+        Zero values should not count towards the minimum check.
+        """
+        idx = (np.array([0, 0, 2, 4, 4]), np.array([0, 1, 1, 2, 4]))
+        non_diag_idx = (np.array([0, 2, 4]), np.array([1, 1, 2]))
+
+        cost_matrix = normal_array.cost_matrix.copy()
+        cost_matrix[idx] = 0
+
+        result = normal_array.result.copy()
+        result[non_diag_idx] = 0
+
+        return self.IzResults(
+            cost_matrix=cost_matrix,
+            multiplier=normal_array.multiplier,
+            min_axis=normal_array.min_axis,
+            result=result,
+        )
+
+    @pytest.fixture(name="inf_array", scope="class")
+    def fixture_inf_array(self, normal_array):
+        """Inf values should be returned in-place, expect in diagonal."""
+        idx = (np.array([0, 0, 2, 4, 4]), np.array([0, 1, 1, 2, 4]))
+        non_diag_idx = (np.array([0, 2, 4]), np.array([1, 1, 2]))
+
+        cost_matrix = normal_array.cost_matrix.copy()
+        cost_matrix[idx] = np.inf
+
+        result = normal_array.result.copy()
+        result[non_diag_idx] = np.inf
+
+        return self.IzResults(
+            cost_matrix=cost_matrix,
+            multiplier=normal_array.multiplier,
+            min_axis=normal_array.min_axis,
+            result=result,
+        )
+
+    @pytest.mark.parametrize(
+        "io_str", ["normal_array", "zeroes_array", "inf_array", "min_axis_array"]
+    )
+    def test_correct_result(self, io_str: str, request):
+        """Test that the correct results are achieved"""
+        io: TestIntrazonalCostInfill.IzResults = request.getfixturevalue(io_str)
+        result = cost_utils.intrazonal_cost_infill(**io.get_kwargs())
+        np.testing.assert_almost_equal(result, io.result)
+
+    @pytest.mark.parametrize(
+        "io_str", ["normal_array", "zeroes_array", "inf_array", "min_axis_array"]
+    )
+    @pytest.mark.parametrize("multiplier", [0, 0.5, 2])
+    def test_different_multiplier(self, io_str: str, multiplier: float, request):
+        """Test that the multiplier is being applied correctly."""
+        io: TestIntrazonalCostInfill.IzResults = request.getfixturevalue(io_str)
+
+        # Calculate the new result
+        new_diag = np.diagonal(io.result) * multiplier
+        expected_result = io.result.copy()
+        np.fill_diagonal(expected_result, new_diag)
+
+        # Calculate and test the result
+        result = cost_utils.intrazonal_cost_infill(
+            **io.get_kwargs() | {"multiplier": multiplier}
+        )
+        np.testing.assert_almost_equal(result, expected_result)
```

### Comparing `caf.toolkit-0.7.0/tests/test_io.py` & `caf.toolkit-0.7.1/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.7.0/tests/test_log_helpers.py` & `caf.toolkit-0.7.1/tests/test_log_helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # Third Party
 import psutil
 import pydantic
 import pytest
 
 # Local Imports
 from caf.toolkit import LogHelper, SystemInformation, TemporaryLogFile, ToolDetails
-from caf.toolkit.log_helpers import capture_warnings, get_logger
+from caf.toolkit.log_helpers import LoggingWarning, capture_warnings, get_logger
 
 # # # Constants # # #
 _LOG_WARNINGS = [
     ("testing warning: runtime warning", RuntimeWarning),
     ("testing warning: user warning", UserWarning),
 ]
 # Note: ImportWarnings aren't logged by default
@@ -435,14 +435,48 @@
         del warnings_logger  # Fixture clears handlers from logger
 
         with LogHelper("test", log_init.details):
             _run_warnings()
 
         _check_warnings(caplog.text)
 
+    def test_no_handlers_warning(self, log_init: LogInitDetails) -> None:
+        """Test LogHelper warns when no handlers are defined."""
+        with pytest.warns(
+            LoggingWarning, match="LogHelper initialised without any logging handlers"
+        ):
+            with LogHelper(
+                "test", log_init.details, console=False, warning_capture=False
+            ) as helper:
+                assert helper.logger.handlers == [], "incorrect handlers"
+
+    @pytest.mark.parametrize("warning_capture", [False, True])
+    def test_add_handler(
+        self, log_init: LogInitDetails, warning_capture: bool, warnings_logger: logging.Logger
+    ) -> None:
+        """Test creating LogHelper without loggers and adding StreamHandler after."""
+        # pylint: disable=protected-access
+        stream = logging.StreamHandler()
+
+        with LogHelper(
+            "test", log_init.details, console=False, warning_capture=warning_capture
+        ) as helper:
+            assert helper.logger.handlers == [], "logger already has handlers"
+            assert warnings_logger.handlers == [], "warnings logger already has handlers"
+
+            helper.add_handler(stream)
+            assert helper.logger.handlers == [stream], "list of handlers is incorrect"
+
+            if warning_capture:
+                assert warnings_logger.handlers == [
+                    stream
+                ], "handler not added to warnings logger"
+            else:
+                assert warnings_logger.handlers == [], "handlers added to warnings logger"
+
 
 class TestTemporaryLogFile:
     # pylint: disable=too-few-public-methods
     """Test `TemporaryLogFile` class."""
 
     def test_log_file(self, tmp_path: pathlib.Path) -> None:
         """Test log file handler is added and removed correctly."""
```

### Comparing `caf.toolkit-0.7.0/tests/test_main.py` & `caf.toolkit-0.7.1/tests/test_main.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
 
 class TestParseArgs:
     """Test `parse_args` function to make sure it returns the correct arguments."""
 
     @pytest.mark.parametrize("type_", ["translate", "matrix_translate"])
     def test_min_parameters(self, dummy_files: dict[str, pathlib.Path], type_) -> None:
-        """Testing running with bare minumum arguments."""
+        """Testing running with bare minimum arguments."""
         sys.argv = [
             "caf.toolkit",
             type_,
             str(dummy_files["data_file"]),
             str(dummy_files["translation_file"]),
         ]
```

### Comparing `caf.toolkit-0.7.0/tests/test_math_utils.py` & `caf.toolkit-0.7.1/tests/test_math_utils.py`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.7.0/tests/test_timing.py` & `caf.toolkit-0.7.1/tests/test_timing.py`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.7.0/tests/test_toolbox.py` & `caf.toolkit-0.7.1/tests/test_toolbox.py`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.7.0/tests/test_translation.py` & `caf.toolkit-0.7.1/tests/test_translation.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,18 +11,17 @@
 
 # Third Party
 import numpy as np
 import pandas as pd
 import pytest
 
 # Local Imports
-# pylint: disable=import-error,wrong-import-position
-from caf.toolkit import io, translation
-
-# pylint: enable=import-error,wrong-import-position
+from caf.toolkit import io
+from caf.toolkit import pandas_utils as pd_utils
+from caf.toolkit import translation
 
 # # # CONSTANTS # # #
 
 
 # # # CLASSES # # #
 @dataclasses.dataclass
 class NumpyVectorResults:
@@ -311,14 +310,89 @@
         )
 
         if self.col_translation is None:
             return kwargs
         return kwargs | {"col_translation": self.col_translation.df}
 
 
+@dataclasses.dataclass
+class PandasLongMatrixResults:
+    """Collection of I/O data for a pandas matrix translation"""
+
+    wide_results: dataclasses.InitVar[PandasMatrixResults]
+    index_col_1_name: str = "production"
+    index_col_2_name: str = "attraction"
+    values_col: str = "values"
+    index_col_1_out_name: Optional[str] = None
+    index_col_2_out_name: Optional[str] = None
+
+    def __post_init__(self, wide_results: PandasMatrixResults):
+        """Produce the new expected input and outputs."""
+        if self.index_col_1_out_name is None:
+            self.index_col_1_out_name = self.index_col_1_name
+        if self.index_col_2_out_name is None:
+            self.index_col_2_out_name = self.index_col_2_name
+
+        self.df = pd_utils.wide_to_long_infill(
+            df=wide_results.mat,
+            index_col_1_name=self.index_col_1_name,
+            index_col_2_name=self.index_col_2_name,
+            value_col_name=self.values_col,
+        )
+
+        self.expected_result = pd_utils.wide_to_long_infill(
+            df=wide_results.expected_result,
+            index_col_1_name=self.index_col_1_out_name,
+            index_col_2_name=self.index_col_2_out_name,
+            value_col_name=self.values_col,
+        )
+
+        # Misc args to carry over
+        self.translation_dtype = wide_results.translation_dtype
+        self.translation = wide_results.translation
+        self.col_translation = wide_results.col_translation
+
+    def update_output_cols(self, index_col_1_out_name: str, index_col_2_out_name: str) -> None:
+        """Update the expected result alongside this."""
+        self.expected_result.rename(
+            columns={
+                self.index_col_1_name: index_col_1_out_name,
+                self.index_col_2_name: index_col_2_out_name,
+            },
+            inplace=True,
+        )
+        self.index_col_1_out_name = index_col_1_out_name
+        self.index_col_2_out_name = index_col_2_out_name
+
+    def input_kwargs(
+        self,
+        check_totals: bool = True,
+        **kwargs,
+    ) -> dict[str, Any]:
+        """Return a dictionary of key-word arguments"""
+        kwargs = (
+            {
+                "matrix": self.df,
+                "index_col_1_name": self.index_col_1_name,
+                "index_col_2_name": self.index_col_2_name,
+                "values_col": self.values_col,
+                "index_col_1_out_name": self.index_col_1_out_name,
+                "index_col_2_out_name": self.index_col_2_out_name,
+                "translation_dtype": self.translation_dtype,
+                "check_totals": check_totals,
+            }
+            | self.translation.to_kwargs()
+            | kwargs
+        )
+
+        if self.col_translation is None:
+            return kwargs
+        return kwargs | {"col_translation": self.col_translation.df}
+
+
 # # # FIXTURES # # #
 @pytest.fixture(name="simple_np_int_translation", scope="class")
 def fixture_simple_np_int_translation() -> np.ndarray:
     """Generate a simple 5 to 3 complete translation array"""
     return np.array(
         [
             [1, 0, 0],
@@ -723,14 +797,47 @@
     return PandasMatrixResults(
         np_matrix=np_matrix_incomplete.mat,
         np_expected_result=np_matrix_incomplete.expected_result,
         translation=incomplete_pd_int_translation,
     )
 
 
+# ## PANDAS LONG MATRIX FIXTURES ## #
+@pytest.fixture(name="pd_long_matrix_aggregation", scope="class")
+def fixture_pd_long_matrix_aggregation(
+    pd_matrix_aggregation: PandasMatrixResults,
+) -> PandasLongMatrixResults:
+    """Convert fixture to long format."""
+    return PandasLongMatrixResults(wide_results=pd_matrix_aggregation)
+
+
+@pytest.fixture(name="pd_long_matrix_aggregation2", scope="class")
+def fixture_pd_long_matrix_aggregation2(
+    pd_matrix_aggregation2: PandasMatrixResults,
+) -> PandasLongMatrixResults:
+    """Convert fixture to long format."""
+    return PandasLongMatrixResults(wide_results=pd_matrix_aggregation2)
+
+
+@pytest.fixture(name="pd_long_matrix_split", scope="class")
+def fixture_pd_long_matrix_split(
+    pd_matrix_split: PandasMatrixResults,
+) -> PandasLongMatrixResults:
+    """Convert fixture to long format."""
+    return PandasLongMatrixResults(wide_results=pd_matrix_split)
+
+
+@pytest.fixture(name="pd_long_matrix_dtype", scope="class")
+def fixture_pd_long_matrix_dtype(
+    pd_matrix_dtype: PandasMatrixResults,
+) -> PandasLongMatrixResults:
+    """Convert fixture to long format."""
+    return PandasLongMatrixResults(wide_results=pd_matrix_dtype)
+
+
 # # # TESTS # # #
 @pytest.mark.usefixtures(
     "np_vector_aggregation",
     "np_vector_split",
     "np_incomplete",
     "np_translation_dtype",
 )
@@ -1033,15 +1140,15 @@
         pd_vector: PandasMultiVectorResults = request.getfixturevalue(pd_vector_str)
 
         # Add some additional data to the translation
         new_rows = pd_vector.translation.create_dummy_rows()
         new_trans = pd_vector.translation.df.copy()
         new_trans = pd.concat([new_trans, new_rows], ignore_index=True)
 
-        # Check that the transaltion still works as before
+        # Check that the translation still works as before
         result = translation.pandas_multi_vector_zone_translation(
             **(pd_vector.input_kwargs() | {"translation": new_trans})
         )
         pd.testing.assert_frame_equal(result, pd_vector.expected_result, check_dtype=False)
 
     @pytest.mark.parametrize(
         "pd_vector_str",
@@ -1070,24 +1177,30 @@
         with pytest.raises(ValueError, match="The input vector is MultiIndexed"):
             translation.pandas_multi_vector_zone_translation(
                 **(pd_multi_vector_multiindex.input_kwargs() | {"vector": new_vector})
             )
 
     def test_multiindex(self, pd_multi_vector_multiindex: PandasMultiVectorResults):
         """Test that a multiindex is allowed."""
+        # Setup
         new_vector = pd_multi_vector_multiindex.vector.copy()
         new_vector.index.names = ["from_zone_id"]
         factors = [1, 2, 3, 2, 5, 3, 6, 8, 2, 3]
         multiindex = pd.MultiIndex.from_product(
             [new_vector.index, ["A", "B"]], names=["from_zone_id", "extra_seg"]
         )
         multi_vector = new_vector.mul(pd.Series(data=factors, index=multiindex), axis="index")
-        result = translation.pandas_multi_vector_zone_translation(
-            **(pd_multi_vector_multiindex.input_kwargs() | {"vector": multi_vector})
-        )
+
+        # Expect a multiindex warning
+        with pytest.warns(UserWarning, match="input vector is MultiIndexed"):
+            result = translation.pandas_multi_vector_zone_translation(
+                **(pd_multi_vector_multiindex.input_kwargs() | {"vector": multi_vector})
+            )
+
+        # Calculate the expected result
         expected = pd.DataFrame(
             {
                 0: {
                     (1, "A"): 32.0,
                     (1, "B"): 44.75,
                     (2, "A"): 48.0,
                     (2, "B"): 33.5,
@@ -1233,26 +1346,60 @@
         request,
     ):
         """Test translation works as expected
 
         Tests the matrix aggregation, using 2 different translations, and
         translation splitting.
         """
-        pd_mat = request.getfixturevalue(pd_matrix_str)
+        pd_mat: PandasMatrixResults = request.getfixturevalue(pd_matrix_str)
         result = translation.pandas_matrix_zone_translation(
             **pd_mat.input_kwargs(check_totals=check_totals)
         )
 
         # Need to enforce types so this works in linux
         if sys.platform.startswith("linux"):
             if any(x in ["int32", "int64"] for x in result.dtypes):
                 result = result.astype(pd_mat.expected_result.dtypes[1])
 
         pd.testing.assert_frame_equal(result, pd_mat.expected_result)
 
+    def test_additional_index(self, pd_matrix_str: str, check_totals: bool, request):
+        """Check a warning is raised if no translation exists for an index value."""
+        pd_mat: PandasMatrixResults = request.getfixturevalue(pd_matrix_str)
+
+        # Make new row to add
+        add_df = pd.DataFrame(
+            data=np.expand_dims(np.zeros(pd_mat.mat.shape[0]), 0),
+            columns=pd_mat.mat.columns,
+            index=[pd_mat.mat.index.max() + 1],
+        )
+        new_df = pd.concat([pd_mat.mat, add_df])
+
+        # Expect the error
+        msg = "zones in `matrix.index` have not been defined in `row_translation`"
+        with pytest.warns(UserWarning, match=msg):
+            translation.pandas_matrix_zone_translation(
+                **pd_mat.input_kwargs(check_totals=check_totals) | {"matrix": new_df}
+            )
+
+    def test_additional_column(self, pd_matrix_str: str, check_totals: bool, request):
+        """Check a warning is raised if no translation exists for a column value."""
+        pd_mat: PandasMatrixResults = request.getfixturevalue(pd_matrix_str)
+
+        # Add an additional columns
+        new_df = pd_mat.mat.copy()
+        new_df[pd_mat.mat.columns.max() + 1] = np.zeros(pd_mat.mat.shape[1])
+
+        # Expect the error
+        msg = "zones in `matrix.columns` have not been defined in `col_translation`"
+        with pytest.warns(UserWarning, match=msg):
+            translation.pandas_matrix_zone_translation(
+                **pd_mat.input_kwargs(check_totals=check_totals) | {"matrix": new_df}
+            )
+
     @pytest.mark.parametrize("row", [True, False])
     def test_check_allow_similar_types(
         self,
         pd_matrix_str: str,
         row: bool,
         check_totals: bool,
         request,
@@ -1317,14 +1464,87 @@
         if sys.platform.startswith("linux"):
             if any(x in ["int32", "int64"] for x in result.dtypes):
                 result = result.astype(pd_mat.expected_result.dtypes[1])
 
         pd.testing.assert_frame_equal(result, pd_mat.expected_result)
 
 
+@pytest.mark.parametrize(
+    "pd_matrix_str, check_totals",
+    [
+        ("pd_long_matrix_aggregation", True),
+        ("pd_long_matrix_aggregation", False),
+        ("pd_long_matrix_aggregation2", True),
+        ("pd_long_matrix_aggregation2", False),
+        ("pd_long_matrix_split", True),
+        ("pd_long_matrix_split", False),
+        ("pd_long_matrix_dtype", False),
+    ],
+)
+class TestLongPandasMatrixParams:
+    """Tests for caf.toolkit.translation.pandas_long_matrix_zone_translation"""
+
+    def test_translation_correct(
+        self,
+        pd_matrix_str: str,
+        check_totals: bool,
+        request,
+    ):
+        """Test translation works as expected
+
+        Tests the matrix aggregation, using 2 different translations, and
+        translation splitting.
+        """
+        pd_mat: PandasLongMatrixResults = request.getfixturevalue(pd_matrix_str)
+        result = translation.pandas_long_matrix_zone_translation(
+            **pd_mat.input_kwargs(check_totals=check_totals)
+        )
+
+        # Dtypes are checked in TestPandasMatrixParams.test_correct_results test. Ignore here.
+        pd.testing.assert_frame_equal(result, pd_mat.expected_result, check_dtype=False)
+
+    def test_different_output_names(
+        self,
+        pd_matrix_str: str,
+        check_totals: bool,
+        request,
+    ):
+        """Test translation works with different output column names."""
+        pd_mat: PandasLongMatrixResults = request.getfixturevalue(pd_matrix_str)
+        pd_mat.update_output_cols(
+            index_col_1_out_name="Origin", index_col_2_out_name="Destination"
+        )
+        result = translation.pandas_long_matrix_zone_translation(
+            **pd_mat.input_kwargs(check_totals=check_totals)
+        )
+
+        # Dtypes are checked in TestPandasMatrixParams.test_correct_results test. Ignore here.
+        pd.testing.assert_frame_equal(result, pd_mat.expected_result, check_dtype=False)
+
+    def test_additional_cols(
+        self,
+        pd_matrix_str: str,
+        check_totals: bool,
+        request,
+    ):
+        """Test a warning is raised when there are additional columns."""
+        pd_mat: PandasLongMatrixResults = request.getfixturevalue(pd_matrix_str)
+        new_mat = pd_mat.df.copy()
+        new_mat["extra_col"] = 0
+
+        msg = "Extra columns found in matrix"
+        with pytest.warns(UserWarning, match=msg):
+            result = translation.pandas_long_matrix_zone_translation(
+                **pd_mat.input_kwargs(check_totals=check_totals) | {"matrix": new_mat}
+            )
+
+        # Dtypes are checked in TestPandasMatrixParams.test_correct_results test. Ignore here.
+        pd.testing.assert_frame_equal(result, pd_mat.expected_result, check_dtype=False)
+
+
 # ## READ FILE TRANSLATION FIXTURES & TESTS ## #
 @dataclasses.dataclass
 class PandasFileVectorResults:
     """Parameters and results for vector file translation tests."""
 
     vector_path: pathlib.Path
     vector_zone_column: str
```

