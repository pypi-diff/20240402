# Comparing `tmp/linfa_vi-1.6.3.tar.gz` & `tmp/linfa_vi-1.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linfa_vi-1.6.3.tar", last modified: Thu Mar 28 15:14:35 2024, max compression
+gzip compressed data, was "linfa_vi-1.6.5.tar", last modified: Tue Apr  2 01:05:12 2024, max compression
```

## Comparing `linfa_vi-1.6.3.tar` & `linfa_vi-1.6.5.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:14:35.016849 linfa_vi-1.6.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-03-28 15:14:19.000000 linfa_vi-1.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8023 2024-03-28 15:14:35.016849 linfa_vi-1.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-03-28 15:14:19.000000 linfa_vi-1.6.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:14:35.012848 linfa_vi-1.6.3/linfa/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-28 15:14:19.000000 linfa_vi-1.6.3/linfa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7380 2024-03-28 15:14:19.000000 linfa_vi-1.6.3/linfa/discrepancy.py
--rw-r--r--   0 runner    (1001) docker     (127)    13040 2024-03-28 15:14:19.000000 linfa_vi-1.6.3/linfa/maf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-03-28 15:14:19.000000 linfa_vi-1.6.3/linfa/mlp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:14:35.012848 linfa_vi-1.6.3/linfa/models/
--rw-r--r--   0 runner    (1001) docker     (127)     7866 2024-03-28 15:14:19.000000 linfa_vi-1.6.3/linfa/models/circuit_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-03-28 15:14:19.000000 linfa_vi-1.6.3/linfa/models/discrepancy_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-03-28 15:14:19.000000 linfa_vi-1.6.3/linfa/models/highdim_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-03-28 15:14:19.000000 linfa_vi-1.6.3/linfa/models/trivial_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    15589 2024-03-28 15:14:19.000000 linfa_vi-1.6.3/linfa/nofas.py
--rw-r--r--   0 runner    (1001) docker     (127)     7415 2024-03-28 15:14:19.000000 linfa_vi-1.6.3/linfa/plot_res.py
--rw-r--r--   0 runner    (1001) docker     (127)    18670 2024-03-28 15:14:19.000000 linfa_vi-1.6.3/linfa/run_experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)    19039 2024-03-28 15:14:19.000000 linfa_vi-1.6.3/linfa/run_experiment_mf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:14:35.012848 linfa_vi-1.6.3/linfa/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-28 15:14:19.000000 linfa_vi-1.6.3/linfa/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-03-28 15:14:19.000000 linfa_vi-1.6.3/linfa/tests/plot_expected_re.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-03-28 15:14:19.000000 linfa_vi-1.6.3/linfa/tests/post_process.py
--rw-r--r--   0 runner    (1001) docker     (127)     5095 2024-03-28 15:14:19.000000 linfa_vi-1.6.3/linfa/tests/test_discr_01_onlydiscr.py
--rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-03-28 15:14:19.000000 linfa_vi-1.6.3/linfa/tests/test_discr_02_LF_nodiscr_LFData_TP1.py
--rw-r--r--   0 runner    (1001) docker     (127)     6240 2024-03-28 15:14:19.000000 linfa_vi-1.6.3/linfa/tests/test_discr_03_LF_nodiscr_LFData_TP15.py
--rw-r--r--   0 runner    (1001) docker     (127)     5856 2024-03-28 15:14:19.000000 linfa_vi-1.6.3/linfa/tests/test_discr_04_LF_nodiscr_HFData_TP1.py
--rw-r--r--   0 runner    (1001) docker     (127)     6044 2024-03-28 15:14:19.000000 linfa_vi-1.6.3/linfa/tests/test_discr_05_LF_nodiscr_HFData_TP15.py
--rw-r--r--   0 runner    (1001) docker     (127)     7518 2024-03-28 15:14:19.000000 linfa_vi-1.6.3/linfa/tests/test_discr_06_LF_withdiscr_HFData_TP1.py
--rw-r--r--   0 runner    (1001) docker     (127)     7789 2024-03-28 15:14:19.000000 linfa_vi-1.6.3/linfa/tests/test_discr_07_LF_withdiscr_HFData_TP15.py
--rw-r--r--   0 runner    (1001) docker     (127)    41029 2024-03-28 15:14:19.000000 linfa_vi-1.6.3/linfa/tests/test_linfa.py
--rw-r--r--   0 runner    (1001) docker     (127)     8608 2024-03-28 15:14:19.000000 linfa_vi-1.6.3/linfa/tests/test_prior.py
--rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-03-28 15:14:19.000000 linfa_vi-1.6.3/linfa/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 15:14:35.016849 linfa_vi-1.6.3/linfa_vi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8023 2024-03-28 15:14:35.000000 linfa_vi-1.6.3/linfa_vi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-03-28 15:14:35.000000 linfa_vi-1.6.3/linfa_vi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 15:14:35.000000 linfa_vi-1.6.3/linfa_vi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-28 15:14:35.000000 linfa_vi-1.6.3/linfa_vi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-28 15:14:35.000000 linfa_vi-1.6.3/linfa_vi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-03-28 15:14:19.000000 linfa_vi-1.6.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 15:14:35.016849 linfa_vi-1.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 15:14:19.000000 linfa_vi-1.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:05:12.503475 linfa_vi-1.6.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-02 01:05:06.000000 linfa_vi-1.6.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8023 2024-04-02 01:05:12.503475 linfa_vi-1.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-04-02 01:05:06.000000 linfa_vi-1.6.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:05:12.495475 linfa_vi-1.6.5/linfa/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-02 01:05:06.000000 linfa_vi-1.6.5/linfa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7380 2024-04-02 01:05:06.000000 linfa_vi-1.6.5/linfa/discrepancy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13040 2024-04-02 01:05:06.000000 linfa_vi-1.6.5/linfa/maf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-04-02 01:05:06.000000 linfa_vi-1.6.5/linfa/mlp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:05:12.499475 linfa_vi-1.6.5/linfa/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     7866 2024-04-02 01:05:06.000000 linfa_vi-1.6.5/linfa/models/circuit_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-04-02 01:05:06.000000 linfa_vi-1.6.5/linfa/models/discrepancy_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-02 01:05:06.000000 linfa_vi-1.6.5/linfa/models/highdim_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-02 01:05:06.000000 linfa_vi-1.6.5/linfa/models/trivial_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15589 2024-04-02 01:05:06.000000 linfa_vi-1.6.5/linfa/nofas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7415 2024-04-02 01:05:06.000000 linfa_vi-1.6.5/linfa/plot_res.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18670 2024-04-02 01:05:06.000000 linfa_vi-1.6.5/linfa/run_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19039 2024-04-02 01:05:06.000000 linfa_vi-1.6.5/linfa/run_experiment_mf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:05:12.499475 linfa_vi-1.6.5/linfa/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-02 01:05:06.000000 linfa_vi-1.6.5/linfa/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-02 01:05:06.000000 linfa_vi-1.6.5/linfa/tests/plot_expected_re.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-02 01:05:06.000000 linfa_vi-1.6.5/linfa/tests/post_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5095 2024-04-02 01:05:06.000000 linfa_vi-1.6.5/linfa/tests/test_discr_01_onlydiscr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-04-02 01:05:06.000000 linfa_vi-1.6.5/linfa/tests/test_discr_02_LF_nodiscr_LFData_TP1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6240 2024-04-02 01:05:06.000000 linfa_vi-1.6.5/linfa/tests/test_discr_03_LF_nodiscr_LFData_TP15.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5856 2024-04-02 01:05:06.000000 linfa_vi-1.6.5/linfa/tests/test_discr_04_LF_nodiscr_HFData_TP1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6044 2024-04-02 01:05:06.000000 linfa_vi-1.6.5/linfa/tests/test_discr_05_LF_nodiscr_HFData_TP15.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7518 2024-04-02 01:05:06.000000 linfa_vi-1.6.5/linfa/tests/test_discr_06_LF_withdiscr_HFData_TP1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7789 2024-04-02 01:05:06.000000 linfa_vi-1.6.5/linfa/tests/test_discr_07_LF_withdiscr_HFData_TP15.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41029 2024-04-02 01:05:06.000000 linfa_vi-1.6.5/linfa/tests/test_linfa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8608 2024-04-02 01:05:06.000000 linfa_vi-1.6.5/linfa/tests/test_prior.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-04-02 01:05:06.000000 linfa_vi-1.6.5/linfa/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:05:12.499475 linfa_vi-1.6.5/linfa_vi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8023 2024-04-02 01:05:12.000000 linfa_vi-1.6.5/linfa_vi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-02 01:05:12.000000 linfa_vi-1.6.5/linfa_vi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 01:05:12.000000 linfa_vi-1.6.5/linfa_vi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-02 01:05:12.000000 linfa_vi-1.6.5/linfa_vi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-02 01:05:12.000000 linfa_vi-1.6.5/linfa_vi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-02 01:05:06.000000 linfa_vi-1.6.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 01:05:12.503475 linfa_vi-1.6.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 01:05:06.000000 linfa_vi-1.6.5/setup.py
```

### Comparing `linfa_vi-1.6.3/LICENSE` & `linfa_vi-1.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.6.3/PKG-INFO` & `linfa_vi-1.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linfa_vi
-Version: 1.6.3
+Version: 1.6.5
 Summary: A Python library for inference with normalizing flow and annealing
 Author-email: resDesLab  <daniele.schiavazzi@gmail.com>
 License: Copyright © 2023 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `linfa_vi-1.6.3/README.md` & `linfa_vi-1.6.5/README.md`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.6.3/linfa/discrepancy.py` & `linfa_vi-1.6.5/linfa/discrepancy.py`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.6.3/linfa/maf.py` & `linfa_vi-1.6.5/linfa/maf.py`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.6.3/linfa/mlp.py` & `linfa_vi-1.6.5/linfa/mlp.py`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.6.3/linfa/models/circuit_models.py` & `linfa_vi-1.6.5/linfa/models/circuit_models.py`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.6.3/linfa/models/discrepancy_models.py` & `linfa_vi-1.6.5/linfa/models/discrepancy_models.py`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.6.3/linfa/models/highdim_models.py` & `linfa_vi-1.6.5/linfa/models/highdim_models.py`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.6.3/linfa/models/trivial_models.py` & `linfa_vi-1.6.5/linfa/models/trivial_models.py`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.6.3/linfa/nofas.py` & `linfa_vi-1.6.5/linfa/nofas.py`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.6.3/linfa/plot_res.py` & `linfa_vi-1.6.5/linfa/plot_res.py`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.6.3/linfa/run_experiment.py` & `linfa_vi-1.6.5/linfa/run_experiment.py`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.6.3/linfa/run_experiment_mf.py` & `linfa_vi-1.6.5/linfa/run_experiment_mf.py`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.6.3/linfa/tests/plot_expected_re.py` & `linfa_vi-1.6.5/linfa/tests/plot_expected_re.py`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.6.3/linfa/tests/post_process.py` & `linfa_vi-1.6.5/linfa/tests/post_process.py`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.6.3/linfa/tests/test_discr_01_onlydiscr.py` & `linfa_vi-1.6.5/linfa/tests/test_discr_01_onlydiscr.py`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.6.3/linfa/tests/test_discr_02_LF_nodiscr_LFData_TP1.py` & `linfa_vi-1.6.5/linfa/tests/test_discr_02_LF_nodiscr_LFData_TP1.py`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.6.3/linfa/tests/test_discr_03_LF_nodiscr_LFData_TP15.py` & `linfa_vi-1.6.5/linfa/tests/test_discr_03_LF_nodiscr_LFData_TP15.py`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.6.3/linfa/tests/test_discr_04_LF_nodiscr_HFData_TP1.py` & `linfa_vi-1.6.5/linfa/tests/test_discr_04_LF_nodiscr_HFData_TP1.py`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.6.3/linfa/tests/test_discr_05_LF_nodiscr_HFData_TP15.py` & `linfa_vi-1.6.5/linfa/tests/test_discr_05_LF_nodiscr_HFData_TP15.py`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.6.3/linfa/tests/test_discr_06_LF_withdiscr_HFData_TP1.py` & `linfa_vi-1.6.5/linfa/tests/test_discr_06_LF_withdiscr_HFData_TP1.py`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.6.3/linfa/tests/test_discr_07_LF_withdiscr_HFData_TP15.py` & `linfa_vi-1.6.5/linfa/tests/test_discr_07_LF_withdiscr_HFData_TP15.py`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.6.3/linfa/tests/test_linfa.py` & `linfa_vi-1.6.5/linfa/tests/test_linfa.py`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.6.3/linfa/tests/test_prior.py` & `linfa_vi-1.6.5/linfa/tests/test_prior.py`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.6.3/linfa/transform.py` & `linfa_vi-1.6.5/linfa/transform.py`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.6.3/linfa_vi.egg-info/PKG-INFO` & `linfa_vi-1.6.5/linfa_vi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linfa_vi
-Version: 1.6.3
+Version: 1.6.5
 Summary: A Python library for inference with normalizing flow and annealing
 Author-email: resDesLab  <daniele.schiavazzi@gmail.com>
 License: Copyright © 2023 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `linfa_vi-1.6.3/linfa_vi.egg-info/SOURCES.txt` & `linfa_vi-1.6.5/linfa_vi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.6.3/pyproject.toml` & `linfa_vi-1.6.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "linfa_vi"
-version = "1.6.3"
+version = "1.6.5"
 description = "A Python library for inference with normalizing flow and annealing"
 readme = "README.md"
 authors = [{ name = "resDesLab ", email = "daniele.schiavazzi@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

