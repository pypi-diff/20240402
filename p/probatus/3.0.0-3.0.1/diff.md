# Comparing `tmp/probatus-3.0.0.tar.gz` & `tmp/probatus-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "probatus-3.0.0.tar", last modified: Sun Mar 17 21:00:32 2024, max compression
+gzip compressed data, was "probatus-3.0.1.tar", last modified: Tue Apr  2 14:13:53 2024, max compression
```

## Comparing `probatus-3.0.0.tar` & `probatus-3.0.1.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 21:00:32.198057 probatus-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-03-17 20:57:46.000000 probatus-3.0.0/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)     5801 2024-03-17 21:00:32.198057 probatus-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-03-17 20:57:46.000000 probatus-3.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 21:00:32.190057 probatus-3.0.0/probatus/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-17 20:57:46.000000 probatus-3.0.0/probatus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 21:00:32.190057 probatus-3.0.0/probatus/feature_elimination/
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-03-17 20:57:46.000000 probatus-3.0.0/probatus/feature_elimination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    67698 2024-03-17 20:57:46.000000 probatus-3.0.0/probatus/feature_elimination/feature_elimination.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 21:00:32.190057 probatus-3.0.0/probatus/interpret/
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-03-17 20:57:46.000000 probatus-3.0.0/probatus/interpret/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20815 2024-03-17 20:57:46.000000 probatus-3.0.0/probatus/interpret/model_interpret.py
--rw-r--r--   0 runner    (1001) docker     (127)    13274 2024-03-17 20:57:46.000000 probatus-3.0.0/probatus/interpret/shap_dependence.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 21:00:32.190057 probatus-3.0.0/probatus/sample_similarity/
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-03-17 20:57:46.000000 probatus-3.0.0/probatus/sample_similarity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28520 2024-03-17 20:57:46.000000 probatus-3.0.0/probatus/sample_similarity/resemblance_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 21:00:32.194057 probatus-3.0.0/probatus/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-03-17 20:57:46.000000 probatus-3.0.0/probatus/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-03-17 20:57:46.000000 probatus-3.0.0/probatus/utils/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9908 2024-03-17 20:57:46.000000 probatus-3.0.0/probatus/utils/arrayfuncs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-03-17 20:57:46.000000 probatus-3.0.0/probatus/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-03-17 20:57:46.000000 probatus-3.0.0/probatus/utils/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-03-17 20:57:46.000000 probatus-3.0.0/probatus/utils/missing_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-03-17 20:57:46.000000 probatus-3.0.0/probatus/utils/plots.py
--rw-r--r--   0 runner    (1001) docker     (127)     5723 2024-03-17 20:57:46.000000 probatus-3.0.0/probatus/utils/scoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     9448 2024-03-17 20:57:46.000000 probatus-3.0.0/probatus/utils/shap_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-03-17 20:57:46.000000 probatus-3.0.0/probatus/utils/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 21:00:32.194057 probatus-3.0.0/probatus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5801 2024-03-17 21:00:32.000000 probatus-3.0.0/probatus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-03-17 21:00:32.000000 probatus-3.0.0/probatus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-17 21:00:32.000000 probatus-3.0.0/probatus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-03-17 21:00:32.000000 probatus-3.0.0/probatus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-17 21:00:32.000000 probatus-3.0.0/probatus.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-03-17 20:57:46.000000 probatus-3.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-17 21:00:32.198057 probatus-3.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 21:00:32.186057 probatus-3.0.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 21:00:32.194057 probatus-3.0.0/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-17 20:57:46.000000 probatus-3.0.0/tests/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-03-17 20:57:46.000000 probatus-3.0.0/tests/docs/test_docstring.py
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-03-17 20:57:46.000000 probatus-3.0.0/tests/docs/test_notebooks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 21:00:32.194057 probatus-3.0.0/tests/feature_elimination/
--rw-r--r--   0 runner    (1001) docker     (127)    20689 2024-03-17 20:57:46.000000 probatus-3.0.0/tests/feature_elimination/test_feature_elimination.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 21:00:32.194057 probatus-3.0.0/tests/interpret/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-17 20:57:46.000000 probatus-3.0.0/tests/interpret/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10235 2024-03-17 20:57:46.000000 probatus-3.0.0/tests/interpret/test_model_interpret.py
--rw-r--r--   0 runner    (1001) docker     (127)     5682 2024-03-17 20:57:46.000000 probatus-3.0.0/tests/interpret/test_shap_dependence.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 21:00:32.194057 probatus-3.0.0/tests/sample_similarity/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-17 20:57:46.000000 probatus-3.0.0/tests/sample_similarity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9219 2024-03-17 20:57:46.000000 probatus-3.0.0/tests/sample_similarity/test_resemblance_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 21:00:32.194057 probatus-3.0.0/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-17 20:57:46.000000 probatus-3.0.0/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7313 2024-03-17 20:57:46.000000 probatus-3.0.0/tests/utils/test_utils_array_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:53.550460 probatus-3.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-02 14:10:39.000000 probatus-3.0.1/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)     5906 2024-04-02 14:13:53.550460 probatus-3.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-02 14:10:39.000000 probatus-3.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:53.538460 probatus-3.0.1/probatus/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-02 14:10:39.000000 probatus-3.0.1/probatus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:53.542460 probatus-3.0.1/probatus/feature_elimination/
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-02 14:10:39.000000 probatus-3.0.1/probatus/feature_elimination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67539 2024-04-02 14:10:39.000000 probatus-3.0.1/probatus/feature_elimination/feature_elimination.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:53.542460 probatus-3.0.1/probatus/interpret/
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-02 14:10:39.000000 probatus-3.0.1/probatus/interpret/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21141 2024-04-02 14:10:39.000000 probatus-3.0.1/probatus/interpret/model_interpret.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13462 2024-04-02 14:10:39.000000 probatus-3.0.1/probatus/interpret/shap_dependence.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:53.542460 probatus-3.0.1/probatus/sample_similarity/
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-02 14:10:39.000000 probatus-3.0.1/probatus/sample_similarity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28296 2024-04-02 14:10:39.000000 probatus-3.0.1/probatus/sample_similarity/resemblance_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:53.542460 probatus-3.0.1/probatus/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-02 14:10:39.000000 probatus-3.0.1/probatus/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-04-02 14:10:39.000000 probatus-3.0.1/probatus/utils/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9517 2024-04-02 14:10:39.000000 probatus-3.0.1/probatus/utils/arrayfuncs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-02 14:10:39.000000 probatus-3.0.1/probatus/utils/base_class_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-04-02 14:10:39.000000 probatus-3.0.1/probatus/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-02 14:10:39.000000 probatus-3.0.1/probatus/utils/missing_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-04-02 14:10:39.000000 probatus-3.0.1/probatus/utils/plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5723 2024-04-02 14:10:39.000000 probatus-3.0.1/probatus/utils/scoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9864 2024-04-02 14:10:39.000000 probatus-3.0.1/probatus/utils/shap_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-02 14:10:39.000000 probatus-3.0.1/probatus/utils/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:53.546460 probatus-3.0.1/probatus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5906 2024-04-02 14:13:53.000000 probatus-3.0.1/probatus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-02 14:13:53.000000 probatus-3.0.1/probatus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 14:13:53.000000 probatus-3.0.1/probatus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-02 14:13:53.000000 probatus-3.0.1/probatus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-02 14:13:53.000000 probatus-3.0.1/probatus.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-04-02 14:10:39.000000 probatus-3.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 14:13:53.550460 probatus-3.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:53.538460 probatus-3.0.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:53.542460 probatus-3.0.1/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:10:39.000000 probatus-3.0.1/tests/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-02 14:10:39.000000 probatus-3.0.1/tests/docs/test_docstring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-02 14:10:39.000000 probatus-3.0.1/tests/docs/test_notebooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:53.542460 probatus-3.0.1/tests/feature_elimination/
+-rw-r--r--   0 runner    (1001) docker     (127)    20131 2024-04-02 14:10:39.000000 probatus-3.0.1/tests/feature_elimination/test_feature_elimination.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:53.546460 probatus-3.0.1/tests/interpret/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:10:39.000000 probatus-3.0.1/tests/interpret/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8968 2024-04-02 14:10:39.000000 probatus-3.0.1/tests/interpret/test_model_interpret.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5945 2024-04-02 14:10:39.000000 probatus-3.0.1/tests/interpret/test_shap_dependence.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:53.546460 probatus-3.0.1/tests/sample_similarity/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:10:39.000000 probatus-3.0.1/tests/sample_similarity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7932 2024-04-02 14:10:39.000000 probatus-3.0.1/tests/sample_similarity/test_resemblance_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:13:53.546460 probatus-3.0.1/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:10:39.000000 probatus-3.0.1/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-02 14:10:39.000000 probatus-3.0.1/tests/utils/test_base_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7289 2024-04-02 14:10:39.000000 probatus-3.0.1/tests/utils/test_utils_array_funcs.py
```

### Comparing `probatus-3.0.0/LICENCE` & `probatus-3.0.1/LICENCE`

 * *Files identical despite different names*

### Comparing `probatus-3.0.0/PKG-INFO` & `probatus-3.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: probatus
-Version: 3.0.0
+Version: 3.0.1
 Summary: Validation of binary classifiers and data used to develop them
 Author-email: "ING Bank N.V." <reinier.koops@ing.com>
 License: Copyright (c) 2020 ING Bank N.V.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -17,30 +17,33 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENCE
 Requires-Dist: scikit-learn>=0.22.2
 Requires-Dist: pandas>=1.0.0
 Requires-Dist: matplotlib>=3.1.1
 Requires-Dist: scipy>=1.4.0
 Requires-Dist: joblib>=0.13.2
 Requires-Dist: tqdm>=4.41.0
-Requires-Dist: shap<0.43.0,>=0.41.0
+Requires-Dist: shap==0.43.0; python_version == "3.8"
+Requires-Dist: shap>=0.43.0; python_version != "3.8"
 Requires-Dist: numpy>=1.23.2
 Requires-Dist: numba>=0.57.0
+Requires-Dist: loguru>=0.7.2
 Provides-Extra: dev
 Requires-Dist: black>=19.10b0; extra == "dev"
 Requires-Dist: pre-commit>=2.5.0; extra == "dev"
 Requires-Dist: mypy>=0.770; extra == "dev"
 Requires-Dist: pytest>=6.0.0; extra == "dev"
 Requires-Dist: pytest-cov>=2.10.0; extra == "dev"
 Requires-Dist: pyflakes; extra == "dev"
@@ -49,28 +52,27 @@
 Requires-Dist: jupyter>=1.0.0; extra == "dev"
 Requires-Dist: tabulate>=0.8.7; extra == "dev"
 Requires-Dist: nbconvert>=6.0.7; extra == "dev"
 Requires-Dist: pre-commit>=2.7.1; extra == "dev"
 Requires-Dist: isort>=5.12.0; extra == "dev"
 Requires-Dist: codespell>=2.2.4; extra == "dev"
 Requires-Dist: ruff>=0.2.2; extra == "dev"
+Requires-Dist: lightgbm>=3.3.0; extra == "dev"
+Requires-Dist: catboost>=1.2; python_version != "3.8" and extra == "dev"
+Requires-Dist: catboost<1.2; python_version == "3.8" and extra == "dev"
+Requires-Dist: xgboost>=1.5.0; extra == "dev"
+Requires-Dist: scipy>=1.4.0; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: mkdocs>=1.5.3; extra == "docs"
 Requires-Dist: mkdocs-jupyter>=0.24.3; extra == "docs"
 Requires-Dist: mkdocs-material>=9.5.13; extra == "docs"
 Requires-Dist: mkdocstrings>=0.24.1; extra == "docs"
 Requires-Dist: mkdocstrings-python>=1.8.0; extra == "docs"
-Provides-Extra: extras
-Requires-Dist: lightgbm>=3.3.0; extra == "extras"
-Requires-Dist: catboost<1.2; python_version == "3.8" and extra == "extras"
-Requires-Dist: catboost>=1.1; python_version != "3.8" and extra == "extras"
-Requires-Dist: xgboost>=1.5.0; extra == "extras"
-Requires-Dist: scipy>=1.4.0; extra == "extras"
 Provides-Extra: all
-Requires-Dist: probatus[dev,docs,extras]; extra == "all"
+Requires-Dist: probatus[dev,docs]; extra == "all"
 
 <img src="https://github.com/ing-bank/probatus/raw/main/docs/img/logo_large.png" width="120" align="right">
 
 [![pytest](https://github.com/ing-bank/probatus/workflows/Development/badge.svg)](https://github.com/ing-bank/probatus/actions?query=workflow%3A%22Development%22)
 [![PyPi Version](https://img.shields.io/pypi/pyversions/probatus)](#)
 [![PyPI](https://img.shields.io/pypi/v/probatus)](#)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/probatus)](#)
```

### Comparing `probatus-3.0.0/README.md` & `probatus-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `probatus-3.0.0/probatus/__init__.py` & `probatus-3.0.1/probatus/__init__.py`

 * *Files identical despite different names*

### Comparing `probatus-3.0.0/probatus/feature_elimination/__init__.py` & `probatus-3.0.1/probatus/feature_elimination/__init__.py`

 * *Files identical despite different names*

### Comparing `probatus-3.0.0/probatus/feature_elimination/feature_elimination.py` & `probatus-3.0.1/probatus/feature_elimination/feature_elimination.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 from joblib import Parallel, delayed
 from sklearn.base import clone, is_classifier, is_regressor
 from sklearn.model_selection import check_cv
 from sklearn.model_selection._search import BaseSearchCV
+from loguru import logger
 
 from probatus.utils import (
     BaseFitComputePlotClass,
     assure_pandas_series,
     calculate_shap_importance,
     get_single_scorer,
     preprocess_data,
@@ -152,17 +153,16 @@
                 Number of cores to run in parallel while fitting across folds. None means 1 unless in a
                 `joblib.parallel_backend` context. -1 means using all processors.
 
             verbose (int, optional):
                 Controls verbosity of the output:
 
                 - 0 - neither prints nor warnings are shown
-                - 1 - 50 - only most important warnings
-                - 51 - 100 - shows other warnings and prints
-                - above 100 - presents all prints and all warnings (including SHAP warnings).
+                - 1 - only most important warnings
+                - 2 - shows all prints and all warnings.
 
             random_state (int, optional):
                 Random state set at each round of feature elimination. If it is None, the results will not be
                 reproducible and in random search at each iteration a different hyperparameters might be tested. For
                 reproducible results set it to an integer.
         """  # noqa
         self.clf = clf
@@ -391,15 +391,15 @@
             clf = clf.fit(X_train, y_train)
 
         # Score the model
         score_train = self.scorer.scorer(clf, X_train, y_train)
         score_val = self.scorer.scorer(clf, X_val, y_val)
 
         # Compute SHAP values
-        shap_values = shap_calc(clf, X_val, verbose=self.verbose, **shap_kwargs)
+        shap_values = shap_calc(clf, X_val, verbose=self.verbose, random_state=self.random_state, **shap_kwargs)
         return shap_values, score_train, score_val
 
     def fit(
         self,
         X,
         y,
         sample_weight=None,
@@ -533,15 +533,15 @@
         # Setting up the min_features_to_select parameter.
         if columns_to_keep is None:
             pass
         else:
             self.min_features_to_select = 0
             # This ensures that, if columns_to_keep is provided ,
             # the last features remaining are only the columns_to_keep.
-            if self.verbose > 50:
+            if self.verbose > 1:
                 warnings.warn(f"Minimum features to select : {stopping_criteria}")
 
         while len(current_features_set) > stopping_criteria:
             round_number += 1
 
             # Get current dataset info
             current_features_set = remaining_features
@@ -606,21 +606,21 @@
             )
 
             # Report results
             self._report_current_results(
                 round_number=round_number,
                 current_features_set=current_features_set,
                 features_to_remove=features_to_remove,
-                train_metric_mean=np.round(np.mean(scores_train), 3),
-                train_metric_std=np.round(np.std(scores_train), 3),
-                val_metric_mean=np.round(np.mean(scores_val), 3),
-                val_metric_std=np.round(np.std(scores_val), 3),
+                train_metric_mean=np.mean(scores_train),
+                train_metric_std=np.std(scores_train),
+                val_metric_mean=np.mean(scores_val),
+                val_metric_std=np.std(scores_val),
             )
-            if self.verbose > 50:
-                print(
+            if self.verbose > 1:
+                logger.info(
                     f"Round: {round_number}, Current number of features: {len(current_features_set)}, "
                     f'Current performance: Train {self.report_df.loc[round_number]["train_metric_mean"]} '
                     f'+/- {self.report_df.loc[round_number]["train_metric_std"]}, CV Validation '
                     f'{self.report_df.loc[round_number]["val_metric_mean"]} '
                     f'+/- {self.report_df.loc[round_number]["val_metric_std"]}. \n'
                     f"Features left: {remaining_features}. "
                     f"Removed features at the end of the round: {features_to_remove}"
@@ -837,16 +837,16 @@
 
         else:
             raise ValueError(
                 "The parameter best_method can take values of 'best', 'best_coherent' or 'best_parsimonious'"
             )
 
         # Log shap_report for users who want to inspect / debug
-        if self.verbose > 50:
-            print(shap_report)
+        if self.verbose > 1:
+            logger.info(shap_report)
 
         return best_num_features
 
     def _get_feature_names(self, num_features):
         """
         Helper function that takes num_features and returns the associated list of column/feature names.
 
@@ -1106,18 +1106,17 @@
             n_jobs (int, optional):
                 Number of cores to run in parallel while fitting across folds. None means 1 unless in a
                 `joblib.parallel_backend` context. -1 means using all processors.
 
             verbose (int, optional):
                 Controls verbosity of the output:
 
-                - 0 - nether prints nor warnings are shown
-                - 1 - 50 - only most important warnings
-                - 51 - 100 - shows other warnings and prints
-                - above 100 - presents all prints and all warnings (including SHAP warnings).
+                - 0 - neither prints nor warnings are shown
+                - 1 - only most important warnings
+                - 2 - shows all prints and all warnings.
 
             random_state (int, optional):
                 Random state set at each round of feature elimination. If it is None, the results will not be
                 reproducible and in random search at each iteration a different hyperparameters might be tested. For
                 reproducible results set it to integer.
 
             early_stopping_rounds (int, optional):
@@ -1206,15 +1205,16 @@
 
         fit_params = {
             "X": X_train,
             "y": y_train,
             "eval_set": [(X_val, y_val)],
             "callbacks": [early_stopping(self.early_stopping_rounds, first_metric_only=True)],
         }
-        if self.verbose >= 100:
+
+        if self.verbose >= 2:
             fit_params["callbacks"].append(log_evaluation(1))
         else:
             fit_params["callbacks"].append(log_evaluation(0))
         if sample_weight is not None:
             fit_params["sample_weight"] = sample_weight.iloc[train_index]
             fit_params["eval_sample_weight"] = [sample_weight.iloc[val_index]]
         return fit_params
@@ -1501,9 +1501,9 @@
         clf = clf.fit(**fit_params)
 
         # Score the model
         score_train = self.scorer.scorer(clf, X_train, y_train)
         score_val = self.scorer.scorer(clf, X_val, y_val)
 
         # Compute SHAP values
-        shap_values = shap_calc(clf, X_val, verbose=self.verbose, **shap_kwargs)
+        shap_values = shap_calc(clf, X_val, verbose=self.verbose, random_state=self.random_state, **shap_kwargs)
         return shap_values, score_train, score_val
```

### Comparing `probatus-3.0.0/probatus/interpret/__init__.py` & `probatus-3.0.1/probatus/interpret/__init__.py`

 * *Files identical despite different names*

### Comparing `probatus-3.0.0/probatus/interpret/model_interpret.py` & `probatus-3.0.1/probatus/interpret/model_interpret.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 
     <img src="../img/model_interpret_importance.png" width="320" />
     <img src="../img/model_interpret_summary.png" width="320" />
     <img src="../img/model_interpret_dep.png" width="320" />
     <img src="../img/model_interpret_sample.png" width="320" />
     """
 
-    def __init__(self, clf, scoring="roc_auc", verbose=0):
+    def __init__(self, clf, scoring="roc_auc", verbose=0, random_state=None):
         """
         Initializes the class.
 
         Args:
             clf (binary classifier):
                 Model fitted on X_train.
 
@@ -94,21 +94,25 @@
                 ([link](https://scikit-learn.org/stable/modules/model_evaluation.html)).
                 Another option is using probatus.utils.Scorer to define a custom metric.
 
             verbose (int, optional):
                 Controls verbosity of the output:
 
                 - 0 - neither prints nor warnings are shown
-                - 1 - 50 - only most important warnings
-                - 51 - 100 - shows other warnings and prints
-                - above 100 - presents all prints and all warnings (including SHAP warnings).
+                - 1 - only most important warnings
+                - 2 - shows all prints and all warnings.
+
+            random_state (int, optional):
+                Random state set for the nr of samples. If it is None, the results will not be reproducible. For
+                reproducible results set it to an integer.
         """
         self.clf = clf
         self.scorer = get_single_scorer(scoring)
         self.verbose = verbose
+        self.random_state = random_state
 
     def fit(
         self,
         X_train,
         X_test,
         y_train,
         y_test,
@@ -182,40 +186,43 @@
         ) = self._prep_shap_related_variables(
             clf=self.clf,
             X=self.X_train,
             y=self.y_train,
             column_names=self.column_names,
             class_names=self.class_names,
             verbose=self.verbose,
+            random_state=self.random_state,
             **shap_kwargs,
         )
 
         (
             self.shap_values_test,
             self.expected_value_test,
             self.tdp_test,
         ) = self._prep_shap_related_variables(
             clf=self.clf,
             X=self.X_test,
             y=self.y_test,
             column_names=self.column_names,
             class_names=self.class_names,
             verbose=self.verbose,
+            random_state=self.random_state,
             **shap_kwargs,
         )
 
         self.fitted = True
 
     @staticmethod
     def _prep_shap_related_variables(
         clf,
         X,
         y,
         approximate=False,
         verbose=0,
+        random_state=None,
         column_names=None,
         class_names=None,
         **shap_kwargs,
     ):
         """
         The function prepares the variables related to shap that are used to interpret the model.
 
@@ -224,14 +231,15 @@
                 Shap values, expected value of the explainer, and fitted TreeDependencePlotter for a given dataset.
         """
         shap_values, explainer = shap_calc(
             clf,
             X,
             approximate=approximate,
             verbose=verbose,
+            random_state=random_state,
             return_explainer=True,
             **shap_kwargs,
         )
 
         expected_value = explainer.expected_value
 
         # For sklearn models the expected values consists of two elements (negative_class and positive_class)
```

### Comparing `probatus-3.0.0/probatus/interpret/shap_dependence.py` & `probatus-3.0.1/probatus/interpret/shap_dependence.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,32 +48,36 @@
 
     bdp.plot(feature=2)
     ```
 
     <img src="../img/model_interpret_dep.png"/>
     """
 
-    def __init__(self, clf, verbose=0):
+    def __init__(self, clf, verbose=0, random_state=None):
         """
         Initializes the class.
 
         Args:
             clf (model object):
                 Binary classification model or pipeline.
 
             verbose (int, optional):
                 Controls verbosity of the output:
 
                 - 0 - neither prints nor warnings are shown
-                - 1 - 50 - only most important warnings regarding data properties are shown (excluding SHAP warnings)
-                - 51 - 100 - shows most important warnings, prints of the feature removal process
-                - above 100 - presents all prints and all warnings (including SHAP warnings).
+                - 1 - only most important warnings
+                - 2 - shows all prints and all warnings.
+
+            random_state (int, optional):
+                Random state set for the nr of samples. If it is None, the results will not be reproducible. For
+                reproducible results set it to an integer.
         """
         self.clf = clf
         self.verbose = verbose
+        self.random_state = random_state
 
     def __repr__(self):
         """
         Represent string method.
         """
         return f"Shap dependence plotter for {self.clf.__class__.__name__}"
 
@@ -109,15 +113,22 @@
         self.y = preprocess_labels(y, y_name="y", index=self.X.index, verbose=self.verbose)
 
         # Set class names
         self.class_names = class_names
         if self.class_names is None:
             self.class_names = ["Negative Class", "Positive Class"]
 
-        self.shap_vals_df = shap_to_df(self.clf, self.X, precalc_shap=precalc_shap, verbose=self.verbose, **shap_kwargs)
+        self.shap_vals_df = shap_to_df(
+            self.clf,
+            self.X,
+            precalc_shap=precalc_shap,
+            verbose=self.verbose,
+            random_state=self.random_state,
+            **shap_kwargs,
+        )
 
         self.fitted = True
         return self
 
     def compute(self):
         """
         Computes the report returned to the user, namely the SHAP values generated on the dataset.
```

### Comparing `probatus-3.0.0/probatus/sample_similarity/__init__.py` & `probatus-3.0.1/probatus/sample_similarity/__init__.py`

 * *Files identical despite different names*

### Comparing `probatus-3.0.0/probatus/sample_similarity/resemblance_model.py` & `probatus-3.0.1/probatus/sample_similarity/resemblance_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 
 import warnings
 
 import matplotlib.pyplot as plt
+from loguru import logger
 import numpy as np
 import pandas as pd
 from shap import summary_plot
 from sklearn.inspection import permutation_importance
 from sklearn.model_selection import train_test_split
 
 from probatus.utils import BaseFitComputePlotClass, get_single_scorer, preprocess_data, preprocess_labels
@@ -72,17 +73,16 @@
             n_jobs (int, optional):
                 Number of parallel executions. If -1 use all available cores. By default 1.
 
             verbose (int, optional):
                 Controls verbosity of the output:
 
                 - 0 - neither prints nor warnings are shown
-                - 1 - 50 - only most important warnings
-                - 51 - 100 - shows other warnings and prints
-                - above 100 - presents all prints and all warnings (including SHAP warnings).
+                - 1 - only most important warnings
+                - 2 - shows all prints and all warnings.
 
             random_state (int, optional):
                 Random state set at each round of feature elimination. If it is None, the results will not be
                 reproducible and in random search at each iteration a different hyperparameters might be tested. For
                 reproducible results set it to an integer.
         """  # noqa
         self.clf = clf
@@ -174,16 +174,16 @@
         self.train_score = np.round(self.scorer.score(self.clf, self.X_train, self.y_train), 3)
         self.test_score = np.round(self.scorer.score(self.clf, self.X_test, self.y_test), 3)
 
         self.results_text = (
             f"Train {self.scorer.metric_name}: {np.round(self.train_score, 3)},\n"
             f"Test {self.scorer.metric_name}: {np.round(self.test_score, 3)}."
         )
-        if self.verbose > 50:
-            print(f"Finished model training: \n{self.results_text}")
+        if self.verbose > 1:
+            logger.info(f"Finished model training: \n{self.results_text}")
 
         if self.verbose > 0:
             if self.train_score > self.test_score:
                 warnings.warn(
                     f"Train {self.scorer.metric_name} > Test {self.scorer.metric_name}, which might indicate "
                     f"an overfit. \n Strong overfit might lead to misleading conclusions when analysing "
                     f"feature importance. Consider retraining with more regularization applied to the model."
@@ -339,17 +339,16 @@
             n_jobs (int, optional):
                 Number of parallel executions. If -1 use all available cores. By default 1.
 
             verbose (int, optional):
                 Controls verbosity of the output:
 
                 - 0 - neither prints nor warnings are shown
-                - 1 - 50 - only most important warnings
-                - 51 - 100 - shows other warnings and prints
-                - above 100 - presents all prints and all warnings (including SHAP warnings).
+                - 1 - only most important warnings
+                - 2 - shows all prints and all warnings.
 
             random_state (int, optional):
                 Random state set at each round of feature elimination. If it is None, the results will not be
                 reproducible and in random search at each iteration a different hyperparameters might be tested. For
                 reproducible results set it to integer.
         """  # noqa
         super().__init__(
@@ -568,17 +567,16 @@
             n_jobs (int, optional):
                 Number of parallel executions. If -1 use all available cores. By default 1.
 
             verbose (int, optional):
                 Controls verbosity of the output:
 
                 - 0 - neither prints nor warnings are shown
-                - 1 - 50 - only most important warnings
-                - 51 - 100 - shows other warnings and prints
-                - above 100 - presents all prints and all warnings (including SHAP warnings).
+                - 1 - only most important warnings
+                - 2 - shows all prints and all warnings.
 
             random_state (int, optional):
                 Random state set at each round of feature elimination. If it is None, the results will not be
                 reproducible and in random search at each iteration a different hyperparameters might be tested. For
                 reproducible results set it to integer.
         """  # noqa
         super().__init__(
@@ -626,15 +624,17 @@
 
         Returns:
             (SHAPImportanceResemblance):
                 Fitted object.
         """
         super().fit(X1=X1, X2=X2, column_names=column_names, class_names=class_names)
 
-        self.shap_values_test = shap_calc(self.clf, self.X_test, verbose=self.verbose, **shap_kwargs)
+        self.shap_values_test = shap_calc(
+            self.clf, self.X_test, verbose=self.verbose, random_state=self.random_state, **shap_kwargs
+        )
         self.report = calculate_shap_importance(self.shap_values_test, self.column_names)
         return self
 
     def plot(self, plot_type="bar", show=True, **summary_plot_kwargs):
         """
         Plots the resulting AUC of the model as well as the feature importances.
```

### Comparing `probatus-3.0.0/probatus/utils/__init__.py` & `probatus-3.0.1/probatus/utils/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 from .warnings import ApproximationWarning
 from ._utils import (
     class_name_from_object,
     assure_list_of_strings,
     assure_list_values_allowed,
 )
 from .plots import plot_distributions_of_feature
-from .interface import BaseFitComputeClass, BaseFitComputePlotClass
+from .base_class_interface import BaseFitComputeClass, BaseFitComputePlotClass
 
 __all__ = [
     "NotFittedError",
     "DimensionalityError",
     "UnsupportedModelError",
     "NotInstalledError",
     "Scorer",
```

### Comparing `probatus-3.0.0/probatus/utils/_utils.py` & `probatus-3.0.1/probatus/utils/_utils.py`

 * *Files identical despite different names*

### Comparing `probatus-3.0.0/probatus/utils/arrayfuncs.py` & `probatus-3.0.1/probatus/utils/arrayfuncs.py`

 * *Files 3% similar despite different names*

```diff
@@ -185,17 +185,17 @@
             feature names. If not provided the existing feature names are used or default feature names are
             generated.
 
         verbose (int, optional):
             Controls verbosity of the output:
 
             - 0 - neither prints nor warnings are shown
-            - 1 - 50 - only most important warnings regarding data properties are shown (excluding SHAP warnings)
-            - 51 - 100 - shows most important warnings, prints of the feature removal process
-            - above 100 - presents all prints and all warnings (including SHAP warnings).
+            - 1 - only most important warnings
+            - 2 - shows all prints and all warnings.
+
 
     Returns:
         (pd.DataFrame):
             Preprocessed dataset.
     """
     if X_name is None:
         X_name = "X"
@@ -251,17 +251,16 @@
             going to be ordered based on provided index, otherwise, the current index of y is overwritten by index
             argument.
 
     verbose (int, optional):
         Controls verbosity of the output:
 
         - 0 - neither prints nor warnings are shown
-        - 1 - 50 - only most important warnings regarding data properties are shown (excluding SHAP warnings)
-        - 51 - 100 - shows most important warnings, prints of the feature removal process
-        - above 100 - presents all prints and all warnings (including SHAP warnings).
+        - 1 - only most important warnings
+        - 2 - shows all prints and all warnings.
 
     Returns:
         (pd.Series):
             Labels in the form of pd.Series.
     """
     if y_name is None:
         y_name = "y"
```

### Comparing `probatus-3.0.0/probatus/utils/exceptions.py` & `probatus-3.0.1/probatus/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `probatus-3.0.0/probatus/utils/interface.py` & `probatus-3.0.1/probatus/utils/base_class_interface.py`

 * *Files identical despite different names*

### Comparing `probatus-3.0.0/probatus/utils/missing_helpers.py` & `probatus-3.0.1/probatus/utils/missing_helpers.py`

 * *Files identical despite different names*

### Comparing `probatus-3.0.0/probatus/utils/plots.py` & `probatus-3.0.1/probatus/utils/plots.py`

 * *Files identical despite different names*

### Comparing `probatus-3.0.0/probatus/utils/scoring.py` & `probatus-3.0.1/probatus/utils/scoring.py`

 * *Files identical despite different names*

### Comparing `probatus-3.0.0/probatus/utils/shap_helpers.py` & `probatus-3.0.1/probatus/utils/shap_helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,24 +19,25 @@
 
 
 import warnings
 
 import numpy as np
 import pandas as pd
 from shap import Explainer
-from shap.explainers._tree import Tree
+from shap.explainers import TreeExplainer
 from shap.utils import sample
 from sklearn.pipeline import Pipeline
 
 
 def shap_calc(
     model,
     X,
     return_explainer=False,
     verbose=0,
+    random_state=None,
     sample_size=100,
     approximate=False,
     check_additivity=True,
     **shap_kwargs,
 ):
     """
     Helper function to calculate the shapley values for a given model.
@@ -50,23 +51,26 @@
 
         return_explainer (boolean):
             if True, returns a a tuple (shap_values, explainer).
 
         verbose (int, optional):
             Controls verbosity of the output:
 
-            - 0 - nether prints nor warnings are shown
-            - 1 - 50 - only most important warnings
-            - 51 - 100 - shows other warnings and prints
-            - above 100 - presents all prints and all warnings (including SHAP warnings).
+            - 0 - neither prints nor warnings are shown
+            - 1 - only most important warnings
+            - 2 - shows all prints and all warnings.
+
+        random_state (int, optional):
+            Random state set for the nr of samples. If it is None, the results will not be reproducible. For
+            reproducible results set it to an integer.
 
-         approximate (boolean):
+        approximate (boolean):
             if True uses shap approximations - less accurate, but very fast. It applies to tree-based explainers only.
 
-         check_additivity (boolean):
+        check_additivity (boolean):
             if False SHAP will disable the additivity check for tree-based models.
 
         **shap_kwargs: kwargs of the shap.Explainer
 
     Returns:
         (np.ndarray or tuple(np.ndarray, shap.Explainer)):
             shapley_values for the model, optionally also returns the explainer.
@@ -78,15 +82,15 @@
                 "The provided model is a Pipeline. Unfortunately, the features based on SHAP do not support "
                 "pipelines, because they cannot be used in combination with shap.Explainer. Please apply any "
                 "data transformations before running the probatus module."
             )
         )
     # Suppress warnings regarding XGboost and Lightgbm models.
     with warnings.catch_warnings():
-        if verbose <= 100:
+        if verbose <= 1:
             warnings.simplefilter("ignore")
 
         # For tree explainers, do not pass masker when feature_perturbation is
         # tree_path_dependent, or when X contains categorical features
         # related to issue:
         # https://github.com/slundberg/shap/issues/480
         if shap_kwargs.get("feature_perturbation") == "tree_path_dependent" or X.select_dtypes("category").shape[1] > 0:
@@ -96,21 +100,25 @@
             # Create the background data,required for non tree based models.
             # A single datapoint can passed as mask
             # (https://github.com/slundberg/shap/issues/955#issuecomment-569837201)
             if X.shape[0] < sample_size:
                 sample_size = int(np.ceil(X.shape[0] * 0.2))
             else:
                 pass
-            mask = sample(X, sample_size)
+            mask = sample(X, sample_size, random_state=random_state)
             explainer = Explainer(model, masker=mask, **shap_kwargs)
 
         # For tree-explainers allow for using check_additivity and approximate arguments
-        if isinstance(explainer, Tree):
-            # Calculate Shap values
+        if isinstance(explainer, TreeExplainer):
             shap_values = explainer.shap_values(X, check_additivity=check_additivity, approximate=approximate)
+
+            # From SHAP version 0.43+ https://github.com/shap/shap/pull/3121 required to
+            # get the second dimension of calculated Shap values.
+            if not isinstance(shap_values, list) and len(shap_values.shape) == 3:
+                shap_values = shap_values[:, :, 1]
         else:
             # Calculate Shap values
             shap_values = explainer.shap_values(X)
 
         if isinstance(shap_values, list) and len(shap_values) == 2:
             warnings.warn(
                 "Shap values are related to the output probabilities of class 1 for this model, instead of " "log odds."
```

### Comparing `probatus-3.0.0/probatus/utils/warnings.py` & `probatus-3.0.1/probatus/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `probatus-3.0.0/probatus.egg-info/PKG-INFO` & `probatus-3.0.1/probatus.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: probatus
-Version: 3.0.0
+Version: 3.0.1
 Summary: Validation of binary classifiers and data used to develop them
 Author-email: "ING Bank N.V." <reinier.koops@ing.com>
 License: Copyright (c) 2020 ING Bank N.V.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -17,30 +17,33 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENCE
 Requires-Dist: scikit-learn>=0.22.2
 Requires-Dist: pandas>=1.0.0
 Requires-Dist: matplotlib>=3.1.1
 Requires-Dist: scipy>=1.4.0
 Requires-Dist: joblib>=0.13.2
 Requires-Dist: tqdm>=4.41.0
-Requires-Dist: shap<0.43.0,>=0.41.0
+Requires-Dist: shap==0.43.0; python_version == "3.8"
+Requires-Dist: shap>=0.43.0; python_version != "3.8"
 Requires-Dist: numpy>=1.23.2
 Requires-Dist: numba>=0.57.0
+Requires-Dist: loguru>=0.7.2
 Provides-Extra: dev
 Requires-Dist: black>=19.10b0; extra == "dev"
 Requires-Dist: pre-commit>=2.5.0; extra == "dev"
 Requires-Dist: mypy>=0.770; extra == "dev"
 Requires-Dist: pytest>=6.0.0; extra == "dev"
 Requires-Dist: pytest-cov>=2.10.0; extra == "dev"
 Requires-Dist: pyflakes; extra == "dev"
@@ -49,28 +52,27 @@
 Requires-Dist: jupyter>=1.0.0; extra == "dev"
 Requires-Dist: tabulate>=0.8.7; extra == "dev"
 Requires-Dist: nbconvert>=6.0.7; extra == "dev"
 Requires-Dist: pre-commit>=2.7.1; extra == "dev"
 Requires-Dist: isort>=5.12.0; extra == "dev"
 Requires-Dist: codespell>=2.2.4; extra == "dev"
 Requires-Dist: ruff>=0.2.2; extra == "dev"
+Requires-Dist: lightgbm>=3.3.0; extra == "dev"
+Requires-Dist: catboost>=1.2; python_version != "3.8" and extra == "dev"
+Requires-Dist: catboost<1.2; python_version == "3.8" and extra == "dev"
+Requires-Dist: xgboost>=1.5.0; extra == "dev"
+Requires-Dist: scipy>=1.4.0; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: mkdocs>=1.5.3; extra == "docs"
 Requires-Dist: mkdocs-jupyter>=0.24.3; extra == "docs"
 Requires-Dist: mkdocs-material>=9.5.13; extra == "docs"
 Requires-Dist: mkdocstrings>=0.24.1; extra == "docs"
 Requires-Dist: mkdocstrings-python>=1.8.0; extra == "docs"
-Provides-Extra: extras
-Requires-Dist: lightgbm>=3.3.0; extra == "extras"
-Requires-Dist: catboost<1.2; python_version == "3.8" and extra == "extras"
-Requires-Dist: catboost>=1.1; python_version != "3.8" and extra == "extras"
-Requires-Dist: xgboost>=1.5.0; extra == "extras"
-Requires-Dist: scipy>=1.4.0; extra == "extras"
 Provides-Extra: all
-Requires-Dist: probatus[dev,docs,extras]; extra == "all"
+Requires-Dist: probatus[dev,docs]; extra == "all"
 
 <img src="https://github.com/ing-bank/probatus/raw/main/docs/img/logo_large.png" width="120" align="right">
 
 [![pytest](https://github.com/ing-bank/probatus/workflows/Development/badge.svg)](https://github.com/ing-bank/probatus/actions?query=workflow%3A%22Development%22)
 [![PyPi Version](https://img.shields.io/pypi/pyversions/probatus)](#)
 [![PyPI](https://img.shields.io/pypi/v/probatus)](#)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/probatus)](#)
```

### Comparing `probatus-3.0.0/probatus.egg-info/SOURCES.txt` & `probatus-3.0.1/probatus.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 probatus/interpret/model_interpret.py
 probatus/interpret/shap_dependence.py
 probatus/sample_similarity/__init__.py
 probatus/sample_similarity/resemblance_model.py
 probatus/utils/__init__.py
 probatus/utils/_utils.py
 probatus/utils/arrayfuncs.py
+probatus/utils/base_class_interface.py
 probatus/utils/exceptions.py
-probatus/utils/interface.py
 probatus/utils/missing_helpers.py
 probatus/utils/plots.py
 probatus/utils/scoring.py
 probatus/utils/shap_helpers.py
 probatus/utils/warnings.py
 tests/docs/__init__.py
 tests/docs/test_docstring.py
@@ -30,8 +30,9 @@
 tests/feature_elimination/test_feature_elimination.py
 tests/interpret/__init__.py
 tests/interpret/test_model_interpret.py
 tests/interpret/test_shap_dependence.py
 tests/sample_similarity/__init__.py
 tests/sample_similarity/test_resemblance_model.py
 tests/utils/__init__.py
+tests/utils/test_base_class.py
 tests/utils/test_utils_array_funcs.py
```

### Comparing `probatus-3.0.0/probatus.egg-info/requires.txt` & `probatus-3.0.1/probatus.egg-info/requires.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 scikit-learn>=0.22.2
 pandas>=1.0.0
 matplotlib>=3.1.1
 scipy>=1.4.0
 joblib>=0.13.2
 tqdm>=4.41.0
-shap<0.43.0,>=0.41.0
 numpy>=1.23.2
 numba>=0.57.0
+loguru>=0.7.2
+
+[:python_version != "3.8"]
+shap>=0.43.0
+
+[:python_version == "3.8"]
+shap==0.43.0
 
 [all]
-probatus[dev,docs,extras]
+probatus[dev,docs]
 
 [dev]
 black>=19.10b0
 pre-commit>=2.5.0
 mypy>=0.770
 pytest>=6.0.0
 pytest-cov>=2.10.0
@@ -23,25 +29,23 @@
 jupyter>=1.0.0
 tabulate>=0.8.7
 nbconvert>=6.0.7
 pre-commit>=2.7.1
 isort>=5.12.0
 codespell>=2.2.4
 ruff>=0.2.2
+lightgbm>=3.3.0
+xgboost>=1.5.0
+scipy>=1.4.0
+
+[dev:python_version != "3.8"]
+catboost>=1.2
+
+[dev:python_version == "3.8"]
+catboost<1.2
 
 [docs]
 mkdocs>=1.5.3
 mkdocs-jupyter>=0.24.3
 mkdocs-material>=9.5.13
 mkdocstrings>=0.24.1
 mkdocstrings-python>=1.8.0
-
-[extras]
-lightgbm>=3.3.0
-xgboost>=1.5.0
-scipy>=1.4.0
-
-[extras:python_version != "3.8"]
-catboost>=1.1
-
-[extras:python_version == "3.8"]
-catboost<1.2
```

### Comparing `probatus-3.0.0/pyproject.toml` & `probatus-3.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "probatus"
-version = "3.0.0"
+version = "3.0.1"
 requires-python= ">=3.8"
 description = "Validation of binary classifiers and data used to develop them"
 readme = { file = "README.md", content-type = "text/markdown" }
 authors = [
     { name = "ING Bank N.V.", email = "reinier.koops@ing.com" }
 ]
 license = { file = "LICENCE" }
@@ -16,29 +16,32 @@
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "scikit-learn>=0.22.2",
     "pandas>=1.0.0",
     "matplotlib>=3.1.1",
     "scipy>=1.4.0",
     "joblib>=0.13.2",
     "tqdm>=4.41.0",
-    "shap>=0.41.0,<0.43.0",
+    "shap==0.43.0 ; python_version == '3.8'",
+    "shap>=0.43.0 ; python_version != '3.8'",
     "numpy>=1.23.2",
     "numba>=0.57.0",
+    "loguru>=0.7.2",
 ]
 
 [project.urls]
 Homepage = "https://ing-bank.github.io/probatus/"
 Documentation = "https://ing-bank.github.io/probatus/api/feature_elimination.html"
 Repository = "https://github.com/ing-bank/probatus.git"
 Changelog = "https://github.com/ing-bank/probatus/blob/main/CHANGELOG.md"
@@ -58,32 +61,31 @@
     "jupyter>=1.0.0",
     "tabulate>=0.8.7",
     "nbconvert>=6.0.7",
     "pre-commit>=2.7.1",
     "isort>=5.12.0",
     "codespell>=2.2.4",
     "ruff>=0.2.2",
+    "lightgbm>=3.3.0",
+    # https://github.com/catboost/catboost/issues/2371
+    "catboost>=1.2 ; python_version != '3.8'",
+    "catboost<1.2 ; python_version == '3.8'",
+    "xgboost>=1.5.0",
+    "scipy>=1.4.0",
 ]
 docs = [
     "mkdocs>=1.5.3",
     "mkdocs-jupyter>=0.24.3",
     "mkdocs-material>=9.5.13",
     "mkdocstrings>=0.24.1",
     "mkdocstrings-python>=1.8.0",
 ]
-extras = [
-    "lightgbm>=3.3.0",
-    # https://github.com/catboost/catboost/issues/2371
-    "catboost<1.2 ; python_version == '3.8'",
-    "catboost>=1.1 ; python_version != '3.8'",
-    "xgboost>=1.5.0",
-    "scipy>=1.4.0",
-]
+
 # Separating these allow for more install flexibility.
-all = ["probatus[dev,docs,extras]"]
+all = ["probatus[dev,docs]"]
 
 [tool.setuptools.packages.find]
 exclude = ["tests", "notebooks", "docs"]
 
 [tool.nbqa.addopts]
 # E402: Ignores imports not at the top of file for IPYNB since this makes copy-pasting easier.
 ruff = ["--fix", "--ignore=E402"]
@@ -124,8 +126,8 @@
 filter_files = true
 extend_skip = ["__init__.py", "docs"]
 
 [tool.codespell]
 skip = "**.egg-info*"
 
 [tool.black]
-line-length = 120
+line-length = 120
```

### Comparing `probatus-3.0.0/tests/docs/test_docstring.py` & `probatus-3.0.1/tests/docs/test_docstring.py`

 * *Files identical despite different names*

### Comparing `probatus-3.0.0/tests/docs/test_notebooks.py` & `probatus-3.0.1/tests/docs/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `probatus-3.0.0/tests/feature_elimination/test_feature_elimination.py` & `probatus-3.0.1/tests/feature_elimination/test_feature_elimination.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import os
 
 import pandas as pd
 import pytest
+from lightgbm import LGBMClassifier
 from sklearn.datasets import make_classification
 from sklearn.ensemble import RandomForestClassifier
 from sklearn.linear_model import LogisticRegression
-from sklearn.metrics import get_scorer
 from sklearn.model_selection import RandomizedSearchCV, StratifiedGroupKFold, StratifiedKFold
 from sklearn.pipeline import Pipeline
 from sklearn.preprocessing import StandardScaler
 from sklearn.svm import SVC
-from sklearn.tree import DecisionTreeClassifier
+from xgboost import XGBClassifier
 
 from probatus.feature_elimination import EarlyStoppingShapRFECV, ShapRFECV
 from probatus.utils import preprocess_labels
 
 
 @pytest.fixture(scope="function")
 def X():
@@ -27,68 +27,23 @@
             "col_2": [0, 0, 0, 0, 0, 0, 0, 1],
             "col_3": [1, 0, 1, 0, 1, 0, 1, 0],
         },
         index=[1, 2, 3, 4, 5, 6, 7, 8],
     )
 
 
-@pytest.fixture(scope="session")
-def catboost_classifier_class():
-    """This fixture allows to reuse the import of the CatboostClassifier class across different tests.
-
-    It is equivalent to importing the package at the beginning of the file.
-
-    Importing catboost multiple times results in a ValueError: I/O operation on closed file.
-
-    """
-    from catboost import CatBoostClassifier
-
-    return CatBoostClassifier
-
-
 @pytest.fixture(scope="function")
 def y():
     """
     Fixture for y.
     """
     return pd.Series([1, 0, 1, 0, 1, 0, 1, 0], index=[1, 2, 3, 4, 5, 6, 7, 8])
 
 
 @pytest.fixture(scope="function")
-def X_multi():
-    """
-    Fixture for multi-class X.
-    """
-    return pd.DataFrame(
-        {
-            "col_1": [1, 1, 1, 1, 0, 1, 0, 0],
-            "col_2": [0, 0, 0, 0, 1, 0, 1, 1],
-            "col_3": [1, 0, 2, 0, 2, 0, 1, 0],
-        },
-        index=[1, 2, 3, 4, 5, 6, 7, 8],
-    )
-
-
-@pytest.fixture(scope="function")
-def y_multi():
-    """
-    Fixture for multi-class y.
-    """
-    return pd.Series([1, 0, 2, 0, 2, 0, 1, 0], index=[1, 2, 3, 4, 5, 6, 7, 8])
-
-
-@pytest.fixture(scope="function")
-def y_reg():
-    """
-    Fixture for y.
-    """
-    return pd.Series([100, 1, 101, 2, 99, -1, 102, 1], index=[1, 2, 3, 4, 5, 6, 7, 8])
-
-
-@pytest.fixture(scope="function")
 def sample_weight():
     """
     Fixture for sample_weight.
     """
     return pd.Series([1, 1, 1, 1, 1, 1, 1, 1], index=[1, 2, 3, 4, 5, 6, 7, 8])
 
 
@@ -96,163 +51,161 @@
 def groups():
     """
     Fixture for groups.
     """
     return pd.Series(["grp1", "grp1", "grp1", "grp1", "grp2", "grp2", "grp2", "grp2"], index=[1, 2, 3, 4, 5, 6, 7, 8])
 
 
-def test_shap_rfe_randomized_search(X, y):
+@pytest.fixture(scope="function")
+def XGBoost_classifier(random_state):
+    """This fixture allows to reuse the import of the XGBClassifier class across different tests."""
+    model = XGBClassifier(n_estimators=200, max_depth=3, random_state=random_state)
+    return model
+
+
+def test_shap_rfe_randomized_search(X, y, randomized_search_decision_tree_classifier, random_state):
     """
     Test with RandomizedSearchCV.
     """
-    clf = DecisionTreeClassifier(max_depth=1)
-    param_grid = {"criterion": ["gini"], "min_samples_split": [1, 2]}
-    search = RandomizedSearchCV(clf, param_grid, cv=2, n_iter=2)
-    shap_elimination = ShapRFECV(search, step=0.8, cv=2, scoring="roc_auc", n_jobs=4, random_state=1)
+    search = randomized_search_decision_tree_classifier
+    shap_elimination = ShapRFECV(search, step=0.8, cv=2, scoring="roc_auc", n_jobs=4, random_state=random_state)
     report = shap_elimination.fit_compute(X, y)
 
     assert report.shape[0] == 2
     assert shap_elimination.get_reduced_features_set(1) == ["col_3"]
 
     _ = shap_elimination.plot(show=False)
 
 
-def test_shap_rfe_multi_class(X, y):
-    clf = DecisionTreeClassifier(max_depth=1, random_state=1)
-
+def test_shap_rfe_multi_class(X, y, decision_tree_classifier, random_state):
     shap_elimination = ShapRFECV(
-        clf,
+        decision_tree_classifier,
         cv=2,
         scoring="roc_auc_ovr",
-        random_state=1,
+        random_state=random_state,
     )
 
     report = shap_elimination.fit_compute(X, y, approximate=False, check_additivity=False)
 
     assert report.shape[0] == 3
     assert shap_elimination.get_reduced_features_set(1) == ["col_3"]
 
 
-def test_shap_rfe(X, y, sample_weight):
+def test_shap_rfe(X, y, sample_weight, decision_tree_classifier, random_state):
     """
     Test with ShapRFECV.
     """
-    clf = DecisionTreeClassifier(max_depth=1, random_state=1)
     shap_elimination = ShapRFECV(
-        clf,
-        random_state=1,
+        decision_tree_classifier,
+        random_state=random_state,
         step=1,
         cv=2,
         scoring="roc_auc",
         n_jobs=4,
     )
     report = shap_elimination.fit_compute(X, y, sample_weight=sample_weight, approximate=True, check_additivity=False)
 
     assert report.shape[0] == 3
     assert shap_elimination.get_reduced_features_set(1) == ["col_3"]
 
 
-def test_shap_rfe_group_cv(X, y, groups, sample_weight):
+def test_shap_rfe_group_cv(X, y, groups, sample_weight, decision_tree_classifier, random_state):
     """
     Test ShapRFECV with StratifiedGroupKFold.
     """
-    clf = DecisionTreeClassifier(max_depth=1, random_state=1)
-    cv = StratifiedGroupKFold(n_splits=2, shuffle=True, random_state=1)
+    cv = StratifiedGroupKFold(n_splits=2, shuffle=True, random_state=random_state)
     shap_elimination = ShapRFECV(
-        clf,
-        random_state=1,
+        decision_tree_classifier,
+        random_state=random_state,
         step=1,
         cv=cv,
         scoring="roc_auc",
         n_jobs=4,
     )
     report = shap_elimination.fit_compute(
         X, y, groups=groups, sample_weight=sample_weight, approximate=True, check_additivity=False
     )
 
     assert report.shape[0] == 3
     assert shap_elimination.get_reduced_features_set(1) == ["col_3"]
 
 
-def test_shap_pipeline_error(X, y):
+def test_shap_pipeline_error(X, y, decision_tree_classifier, random_state):
     """
     Test with ShapRFECV for pipelines.
     """
     clf = Pipeline(
         [
             ("scaler", StandardScaler()),
-            ("dt", DecisionTreeClassifier(max_depth=1, random_state=1)),
+            ("dt", decision_tree_classifier),
         ]
     )
     with pytest.raises(TypeError):
         shap_elimination = ShapRFECV(
             clf,
-            random_state=1,
+            random_state=random_state,
             step=1,
             cv=2,
             scoring="roc_auc",
             n_jobs=4,
         )
         shap_elimination = shap_elimination.fit(X, y, approximate=True, check_additivity=False)
 
 
-def test_shap_rfe_linear_model(X, y):
+def test_shap_rfe_linear_model(X, y, random_state):
     """
     Test ShapRFECV with linear model.
     """
-    clf = LogisticRegression(C=1, random_state=1)
-    shap_elimination = ShapRFECV(clf, random_state=1, step=1, cv=2, scoring="roc_auc", n_jobs=4)
+    clf = LogisticRegression(C=1, random_state=random_state)
+    shap_elimination = ShapRFECV(clf, random_state=random_state, step=1, cv=2, scoring="roc_auc", n_jobs=4)
     report = shap_elimination.fit_compute(X, y)
 
     assert report.shape[0] == 3
     assert shap_elimination.get_reduced_features_set(1) == ["col_3"]
 
 
-def test_shap_rfe_svm(X, y):
+def test_shap_rfe_svm(X, y, random_state):
     """
     Test with ShapRFECV with SVM.
     """
-    clf = SVC(C=1, kernel="linear", probability=True)
-    shap_elimination = ShapRFECV(clf, random_state=1, step=1, cv=2, scoring="roc_auc", n_jobs=4)
+    clf = SVC(C=1, kernel="linear", probability=True, random_state=random_state)
+    shap_elimination = ShapRFECV(clf, random_state=random_state, step=1, cv=2, scoring="roc_auc", n_jobs=4)
     shap_elimination = shap_elimination.fit(X, y)
     report = shap_elimination.compute()
 
     assert report.shape[0] == 3
     assert shap_elimination.get_reduced_features_set(1) == ["col_3"]
 
 
-def test_shap_rfe_cols_to_keep(X, y):
+def test_shap_rfe_cols_to_keep(X, y, decision_tree_classifier, random_state):
     """
     Test for shap_rfe_cv with features to keep parameter.
     """
-    clf = DecisionTreeClassifier(max_depth=1, random_state=1)
     shap_elimination = ShapRFECV(
-        clf,
-        random_state=1,
+        decision_tree_classifier,
+        random_state=random_state,
         step=2,
         cv=2,
         scoring="roc_auc",
         n_jobs=4,
         min_features_to_select=1,
     )
     report = shap_elimination.fit_compute(X, y, columns_to_keep=["col_2", "col_3"])
 
     assert report.shape[0] == 2
     reduced_feature_set = set(shap_elimination.get_reduced_features_set(num_features=2))
     assert reduced_feature_set == {"col_2", "col_3"}
 
 
-def test_shap_rfe_randomized_search_cols_to_keep(X, y):
+def test_shap_rfe_randomized_search_cols_to_keep(X, y, randomized_search_decision_tree_classifier, random_state):
     """
     Test with ShapRFECV with column to keep param.
     """
-    clf = DecisionTreeClassifier(max_depth=1)
-    param_grid = {"criterion": ["gini"], "min_samples_split": [1, 2]}
-    search = RandomizedSearchCV(clf, param_grid, cv=2, n_iter=2)
-    shap_elimination = ShapRFECV(search, step=0.8, cv=2, scoring="roc_auc", n_jobs=4, random_state=1)
+    search = randomized_search_decision_tree_classifier
+    shap_elimination = ShapRFECV(search, step=0.8, cv=2, scoring="roc_auc", n_jobs=4, random_state=random_state)
     report = shap_elimination.fit_compute(X, y, columns_to_keep=["col_2", "col_3"])
 
     assert report.shape[0] == 2
     reduced_feature_set = set(shap_elimination.get_reduced_features_set(num_features=2))
     assert reduced_feature_set == {"col_2", "col_3"}
 
 
@@ -270,31 +223,30 @@
         current_num_of_features=5, num_features_to_remove=1, min_num_features_to_keep=5
     )
     assert 4 == ShapRFECV._calculate_number_of_features_to_remove(
         current_num_of_features=5, num_features_to_remove=7, min_num_features_to_keep=1
     )
 
 
-def test_shap_automatic_num_feature_selection():
+def test_shap_automatic_num_feature_selection(decision_tree_classifier, random_state):
     """
     Test automatic num feature selection methods
     """
     X = pd.DataFrame(
         {
             "col_1": [1, 0, 1, 0, 1, 0, 1, 0],
             "col_2": [0, 0, 0, 0, 0, 1, 1, 1],
             "col_3": [1, 1, 1, 0, 0, 0, 0, 0],
         }
     )
     y = pd.Series([0, 0, 0, 0, 1, 1, 1, 1])
 
-    clf = DecisionTreeClassifier(max_depth=1, random_state=1)
     shap_elimination = ShapRFECV(
-        clf,
-        random_state=1,
+        decision_tree_classifier,
+        random_state=random_state,
         step=1,
         cv=2,
         scoring="roc_auc",
         n_jobs=1,
     )
     _ = shap_elimination.fit_compute(X, y, approximate=True, check_additivity=False)
 
@@ -305,382 +257,381 @@
     best_parsimonious_features = shap_elimination.get_reduced_features_set(num_features="best_parsimonious")
 
     assert best_features == ["col_2"]
     assert best_coherent_features == ["col_1", "col_2", "col_3"]
     assert best_parsimonious_features == ["col_2"]
 
 
-def test_get_feature_shap_values_per_fold(X, y):
+def test_get_feature_shap_values_per_fold(X, y, decision_tree_classifier, random_state):
     """
     Test with ShapRFECV with features per fold.
     """
-    clf = DecisionTreeClassifier(max_depth=1)
-    shap_elimination = ShapRFECV(clf)
+    shap_elimination = ShapRFECV(decision_tree_classifier, scoring="roc_auc", random_state=random_state)
     (
         shap_values,
         train_score,
         test_score,
     ) = shap_elimination._get_feature_shap_values_per_fold(
         X,
         y,
-        clf,
+        decision_tree_classifier,
         train_index=[2, 3, 4, 5, 6, 7],
         val_index=[0, 1],
-        scorer=get_scorer("roc_auc"),
     )
     assert test_score == 1
     assert train_score > 0.9
     assert shap_values.shape == (2, 3)
 
 
-def test_shap_rfe_same_features_are_kept_after_each_run():
+def test_shap_rfe_same_features_are_kept_after_each_run(random_state_1234):
     """
     Test a use case which appears to be flickering with Probatus 1.8.9 and lower.
 
     Expected result: every run the same outcome.
     Probatus <= 1.8.9: A different order every time.
     """
-    SEED = 1234
-
     feature_names = [(f"f{num}") for num in range(1, 21)]
 
     # Code from tutorial on probatus documentation
     X, y = make_classification(
         n_samples=100,
         class_sep=0.05,
         n_informative=6,
         n_features=20,
-        random_state=SEED,
+        random_state=random_state_1234,
         n_redundant=10,
         n_clusters_per_class=1,
     )
     X = pd.DataFrame(X, columns=feature_names)
 
     random_forest = RandomForestClassifier(
-        random_state=SEED,
+        random_state=random_state_1234,
         n_estimators=70,
         max_features="log2",
         criterion="entropy",
         class_weight="balanced",
     )
 
     shap_elimination = ShapRFECV(
         random_forest,
         step=0.2,
         cv=5,
         scoring="f1_macro",
         n_jobs=1,
-        random_state=SEED,
+        random_state=random_state_1234,
     )
 
-    report = shap_elimination.fit_compute(X, y, check_additivity=True, seed=SEED)
+    report = shap_elimination.fit_compute(X, y, check_additivity=True)
     # Return the set of features with the best validation accuracy
 
     kept_features = list(report.iloc[[report["val_metric_mean"].idxmax() - 1]]["features_set"].to_list()[0])
 
     # Results from the first run
-    assert ["f2", "f3", "f6", "f10", "f11", "f12", "f13", "f14", "f15", "f17", "f18", "f19", "f20"] == kept_features
+    assert [
+        "f1",
+        "f2",
+        "f3",
+        "f5",
+        "f6",
+        "f10",
+        "f11",
+        "f12",
+        "f13",
+        "f14",
+        "f15",
+        "f16",
+        "f17",
+        "f18",
+        "f19",
+        "f20",
+    ] == kept_features
 
 
-def test_shap_rfe_penalty_factor(X, y):
+def test_shap_rfe_penalty_factor(X, y, decision_tree_classifier, random_state):
     """
     Test ShapRFECV with shap_variance_penalty_factor
     """
-    clf = DecisionTreeClassifier(max_depth=1, random_state=1)
     shap_elimination = ShapRFECV(
-        clf,
-        random_state=1,
+        decision_tree_classifier,
+        random_state=random_state,
         step=1,
         cv=2,
         scoring="roc_auc",
         n_jobs=1,
     )
     report = shap_elimination.fit_compute(
         X, y, shap_variance_penalty_factor=1.0, approximate=True, check_additivity=False
     )
 
     assert report.shape[0] == 3
     assert shap_elimination.get_reduced_features_set(1) == ["col_1"]
 
 
 @pytest.mark.skipif(os.environ.get("SKIP_LIGHTGBM") == "true", reason="LightGBM tests disabled")
-def test_complex_dataset(complex_data, complex_lightgbm):
+def test_complex_dataset(complex_data, complex_lightgbm, random_state_1):
     """
     Test on complex dataset.
     """
     X, y = complex_data
 
     param_grid = {
         "n_estimators": [5, 7, 10],
         "num_leaves": [3, 5, 7, 10],
     }
-    search = RandomizedSearchCV(complex_lightgbm, param_grid, n_iter=1)
+    search = RandomizedSearchCV(complex_lightgbm, param_grid, n_iter=1, random_state=random_state_1)
 
-    shap_elimination = ShapRFECV(clf=search, step=1, cv=10, scoring="roc_auc", n_jobs=3, verbose=50)
+    shap_elimination = ShapRFECV(
+        clf=search, step=1, cv=10, scoring="roc_auc", n_jobs=3, verbose=1, random_state=random_state_1
+    )
 
     report = shap_elimination.fit_compute(X, y)
 
     assert report.shape[0] == X.shape[1]
 
 
 @pytest.mark.skipif(os.environ.get("SKIP_LIGHTGBM") == "true", reason="LightGBM tests disabled")
-def test_shap_rfe_early_stopping_lightGBM(complex_data):
+def test_shap_rfe_early_stopping_lightGBM(complex_data, random_state):
     """
     Test EarlyStoppingShapRFECV with a LGBMClassifier.
     """
-    from lightgbm import LGBMClassifier
-
-    clf = LGBMClassifier(n_estimators=200, max_depth=3)
+    clf = LGBMClassifier(n_estimators=200, max_depth=3, random_state=random_state)
     X, y = complex_data
 
     shap_elimination = EarlyStoppingShapRFECV(
         clf,
-        random_state=1,
+        random_state=random_state,
         step=1,
         cv=10,
         scoring="roc_auc",
         n_jobs=4,
         early_stopping_rounds=5,
         eval_metric="auc",
     )
     report = shap_elimination.fit_compute(X, y, approximate=False, check_additivity=False)
 
     assert report.shape[0] == 5
     assert shap_elimination.get_reduced_features_set(1) == ["f5"]
 
 
 @pytest.mark.skipif(os.environ.get("SKIP_LIGHTGBM") == "true", reason="LightGBM tests disabled")
-def test_shap_rfe_early_stopping_XGBoost(complex_data):
+def test_shap_rfe_early_stopping_XGBoost(XGBoost_classifier, complex_data, random_state):
     """
     Test EarlyStoppingShapRFECV with a LGBMClassifier.
     """
-    from xgboost import XGBClassifier
-
-    clf = XGBClassifier(n_estimators=200, max_depth=3, random_state=42)
     X, y = complex_data
     X["f1_categorical"] = X["f1_categorical"].astype(float)
 
     shap_elimination = EarlyStoppingShapRFECV(
-        clf,
-        random_state=1,
+        XGBoost_classifier,
+        random_state=random_state,
         step=1,
         cv=10,
         scoring="roc_auc",
         n_jobs=4,
         early_stopping_rounds=5,
         eval_metric="auc",
     )
     report = shap_elimination.fit_compute(X, y, approximate=False, check_additivity=False)
 
     assert report.shape[0] == 5
     assert shap_elimination.get_reduced_features_set(1) == ["f4"]
 
 
-# For now this test fails, catboost has issues with categorical variables and
-@pytest.mark.xfail
 @pytest.mark.skipif(os.environ.get("SKIP_LIGHTGBM") == "true", reason="LightGBM tests disabled")
-def test_shap_rfe_early_stopping_CatBoost(complex_data, catboost_classifier_class):
+def test_shap_rfe_early_stopping_CatBoost(complex_data_with_categorical, catboost_classifier, random_state):
     """
     Test EarlyStoppingShapRFECV with a CatBoostClassifier.
     """
-    clf = catboost_classifier_class(random_seed=42)
-    X, y = complex_data
+    X, y = complex_data_with_categorical
 
     shap_elimination = EarlyStoppingShapRFECV(
-        clf,
-        random_state=1,
+        catboost_classifier,
+        random_state=random_state,
         step=1,
         cv=10,
         scoring="roc_auc",
         n_jobs=4,
         early_stopping_rounds=5,
         eval_metric="auc",
     )
     report = shap_elimination.fit_compute(X, y, approximate=False, check_additivity=False)
 
     assert report.shape[0] == 5
     assert shap_elimination.get_reduced_features_set(1)[0] in ["f4", "f5"]
 
 
 @pytest.mark.skipif(os.environ.get("SKIP_LIGHTGBM") == "true", reason="LightGBM tests disabled")
-def test_shap_rfe_randomized_search_early_stopping_lightGBM(complex_data):
+def test_shap_rfe_randomized_search_early_stopping_lightGBM(complex_data, random_state):
     """
     Test EarlyStoppingShapRFECV with RandomizedSearchCV and a LGBMClassifier on complex dataset.
     """
-    from lightgbm import LGBMClassifier
-
-    clf = LGBMClassifier(n_estimators=200)
+    clf = LGBMClassifier(n_estimators=200, random_state=random_state)
     X, y = complex_data
 
     param_grid = {
         "max_depth": [3, 4, 5],
     }
-    search = RandomizedSearchCV(clf, param_grid, cv=2, n_iter=2)
+    search = RandomizedSearchCV(clf, param_grid, cv=2, n_iter=2, random_state=random_state)
     shap_elimination = EarlyStoppingShapRFECV(
         search,
         step=1,
         cv=10,
         scoring="roc_auc",
         early_stopping_rounds=5,
         eval_metric="auc",
         n_jobs=4,
-        verbose=50,
-        random_state=1,
+        verbose=1,
+        random_state=random_state,
     )
     report = shap_elimination.fit_compute(X, y)
 
     assert report.shape[0] == X.shape[1]
     assert shap_elimination.get_reduced_features_set(1) == ["f5"]
 
     _ = shap_elimination.plot(show=False)
 
 
 @pytest.mark.skipif(os.environ.get("SKIP_LIGHTGBM") == "true", reason="LightGBM tests disabled")
-def test_get_feature_shap_values_per_fold_early_stopping_lightGBM(complex_data):
+def test_get_feature_shap_values_per_fold_early_stopping_lightGBM(complex_data, random_state):
     """
     Test with ShapRFECV with features per fold.
     """
-    from lightgbm import LGBMClassifier
-
-    clf = LGBMClassifier(n_estimators=200, max_depth=3)
+    clf = LGBMClassifier(n_estimators=200, max_depth=3, random_state=random_state)
     X, y = complex_data
     y = preprocess_labels(y, y_name="y", index=X.index)
 
-    shap_elimination = EarlyStoppingShapRFECV(clf, early_stopping_rounds=5)
+    shap_elimination = EarlyStoppingShapRFECV(
+        clf, early_stopping_rounds=5, scoring="roc_auc", random_state=random_state
+    )
     (
         shap_values,
         train_score,
         test_score,
     ) = shap_elimination._get_feature_shap_values_per_fold(
         X,
         y,
         clf,
         train_index=list(range(5, 50)),
         val_index=[0, 1, 2, 3, 4],
-        scorer=get_scorer("roc_auc"),
     )
     assert test_score > 0.6
     assert train_score > 0.6
     assert shap_values.shape == (5, 5)
 
 
 @pytest.mark.skipif(os.environ.get("SKIP_LIGHTGBM") == "true", reason="LightGBM tests disabled")
-def test_get_feature_shap_values_per_fold_early_stopping_CatBoost(complex_data, catboost_classifier_class):
+def test_get_feature_shap_values_per_fold_early_stopping_CatBoost(
+    complex_data_with_categorical, catboost_classifier, random_state
+):
     """
     Test with ShapRFECV with features per fold.
     """
-    clf = catboost_classifier_class(random_seed=42)
-    X, y = complex_data
-    X["f1_categorical"] = X["f1_categorical"].astype(str).astype("category")
+    X, y = complex_data_with_categorical
     y = preprocess_labels(y, y_name="y", index=X.index)
 
-    shap_elimination = EarlyStoppingShapRFECV(clf, early_stopping_rounds=5)
+    shap_elimination = EarlyStoppingShapRFECV(
+        catboost_classifier, early_stopping_rounds=5, scoring="roc_auc", random_state=random_state
+    )
     (
         shap_values,
         train_score,
         test_score,
     ) = shap_elimination._get_feature_shap_values_per_fold(
         X,
         y,
-        clf,
+        catboost_classifier,
         train_index=list(range(5, 50)),
         val_index=[0, 1, 2, 3, 4],
-        scorer=get_scorer("roc_auc"),
     )
     assert test_score > 0
     assert train_score > 0.6
     assert shap_values.shape == (5, 5)
 
 
 @pytest.mark.skipif(os.environ.get("SKIP_LIGHTGBM") == "true", reason="LightGBM tests disabled")
-def test_get_feature_shap_values_per_fold_early_stopping_XGBoost(complex_data):
+def test_get_feature_shap_values_per_fold_early_stopping_XGBoost(XGBoost_classifier, complex_data, random_state):
     """
     Test with ShapRFECV with features per fold.
     """
-    from xgboost import XGBClassifier
-
-    clf = XGBClassifier(n_estimators=200, max_depth=3, random_state=42)
     X, y = complex_data
-    X["f1_categorical"] = X["f1_categorical"].astype(float)
     y = preprocess_labels(y, y_name="y", index=X.index)
 
-    shap_elimination = EarlyStoppingShapRFECV(clf, early_stopping_rounds=5)
+    shap_elimination = EarlyStoppingShapRFECV(
+        XGBoost_classifier, early_stopping_rounds=5, scoring="roc_auc", random_state=random_state
+    )
     (
         shap_values,
         train_score,
         test_score,
     ) = shap_elimination._get_feature_shap_values_per_fold(
         X,
         y,
-        clf,
+        XGBoost_classifier,
         train_index=list(range(5, 50)),
         val_index=[0, 1, 2, 3, 4],
-        scorer=get_scorer("roc_auc"),
     )
     assert test_score > 0
     assert train_score > 0.6
     assert shap_values.shape == (5, 5)
 
 
 @pytest.mark.skipif(os.environ.get("SKIP_LIGHTGBM") == "true", reason="LightGBM tests disabled")
-def test_EarlyStoppingShapRFECV_no_categorical(complex_data):
+def test_EarlyStoppingShapRFECV_no_categorical(complex_data, random_state):
     """Test EarlyStoppingShapRFECV when no categorical features are present."""
-    from lightgbm import LGBMClassifier
-
-    clf = LGBMClassifier(n_estimators=50, max_depth=3, num_leaves=3)
+    clf = LGBMClassifier(n_estimators=50, max_depth=3, num_leaves=3, random_state=random_state)
 
     shap_elimination = EarlyStoppingShapRFECV(
         clf=clf,
         step=0.33,
         cv=5,
         scoring="accuracy",
         eval_metric="logloss",
         early_stopping_rounds=5,
+        random_state=random_state,
     )
     X, y = complex_data
     X = X.drop(columns=["f1_categorical"])
     report = shap_elimination.fit_compute(X, y, feature_perturbation="tree_path_dependent")
 
     assert report.shape[0] == X.shape[1]
     assert shap_elimination.get_reduced_features_set(1) == ["f5"]
 
     _ = shap_elimination.plot(show=False)
 
 
 @pytest.mark.skipif(os.environ.get("SKIP_LIGHTGBM") == "true", reason="LightGBM tests disabled")
-def test_LightGBM_stratified_kfold():
+def test_LightGBM_stratified_kfold(random_state):
     """
     Test added to check for https://github.com/ing-bank/probatus/issues/170.
     """
-    from lightgbm import LGBMClassifier
-
     X = pd.DataFrame(
         [
             [1, 2, 3, 4, 5, 101, 102, 103, 104, 105],
             [-1, -2, 2, -5, -7, 1, 2, 5, -1, 3],
             ["a", "b"] * 5,  # noisy categorical will dropped first
         ]
     ).transpose()
     X[2] = X[2].astype("category")
     X[1] = X[1].astype("float")
     X[0] = X[0].astype("float")
     y = [0] * 5 + [1] * 5
 
-    clf = LGBMClassifier()
+    clf = LGBMClassifier(random_state=random_state)
     n_iter = 2
     n_folds = 3
 
     for _ in range(n_iter):
-        skf = StratifiedKFold(n_folds, shuffle=True, random_state=42)
+        skf = StratifiedKFold(n_folds, shuffle=True, random_state=random_state)
         shap_elimination = EarlyStoppingShapRFECV(
             clf=clf,
             step=1 / (n_iter + 1),
             cv=skf,
             scoring="accuracy",
             eval_metric="logloss",
             early_stopping_rounds=5,
+            random_state=random_state,
         )
         report = shap_elimination.fit_compute(X, y, feature_perturbation="tree_path_dependent")
 
     assert report.shape[0] == X.shape[1]
 
     shap_elimination.plot(show=False)
```

### Comparing `probatus-3.0.0/tests/interpret/test_model_interpret.py` & `probatus-3.0.1/tests/interpret/test_model_interpret.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,67 +1,17 @@
 import os
 
 import numpy as np
 import pandas as pd
 import pytest
-from sklearn.linear_model import LogisticRegression
-from sklearn.tree import DecisionTreeClassifier
 
 from probatus.interpret import ShapModelInterpreter
 
 
 @pytest.fixture(scope="function")
-def X_train():
-    """
-    Fixture.
-    """
-    return pd.DataFrame({"col_1": [1, 1, 1, 1], "col_2": [0, 0, 0, 0], "col_3": [1, 0, 1, 0]}, index=[1, 2, 3, 4])
-
-
-@pytest.fixture(scope="function")
-def y_train():
-    """
-    Fixture.
-    """
-    return pd.Series([1, 0, 1, 0], index=[1, 2, 3, 4])
-
-
-@pytest.fixture(scope="function")
-def X_test():
-    """
-    Fixture.
-    """
-    return pd.DataFrame({"col_1": [1, 1, 1, 1], "col_2": [0, 0, 0, 0], "col_3": [1, 0, 1, 0]}, index=[5, 6, 7, 8])
-
-
-@pytest.fixture(scope="function")
-def y_test():
-    """
-    Fixture.
-    """
-    return pd.Series([0, 0, 1, 0], index=[5, 6, 7, 8])
-
-
-@pytest.fixture(scope="function")
-def fitted_tree(X_train, y_train):
-    """
-    Fixture.
-    """
-    return DecisionTreeClassifier(max_depth=1, random_state=1).fit(X_train, y_train)
-
-
-@pytest.fixture(scope="function")
-def fitted_lin(X_train, y_train):
-    """
-    Fixture.
-    """
-    return LogisticRegression(random_state=1).fit(X_train, y_train)
-
-
-@pytest.fixture(scope="function")
 def expected_feature_importance():
     """
     Fixture.
     """
     return pd.DataFrame(
         {
             "mean_abs_shap_value_test": [0.5, 0.0, 0.0],
@@ -85,27 +35,23 @@
             "mean_shap_value_test": [-0.4, 0.0, 0.0],
             "mean_shap_value_train": [-0.4, 0.0, 0.0],
         },
         index=["col_3", "col_1", "col_2"],
     )
 
 
-def test_shap_interpret(fitted_tree, X_train, y_train, X_test, y_test, expected_feature_importance):
+def test_shap_interpret(fitted_tree, X_train, y_train, X_test, y_test, expected_feature_importance, random_state):
     """
     Test.
     """
     class_names = ["neg", "pos"]
 
-    shap_interpret = ShapModelInterpreter(fitted_tree)
+    shap_interpret = ShapModelInterpreter(fitted_tree, random_state=random_state)
     shap_interpret.fit(X_train, X_test, y_train, y_test, class_names=class_names)
 
-    # Check parameters
-    assert shap_interpret.fitted
-    shap_interpret._check_if_fitted
-
     assert shap_interpret.class_names == class_names
     assert shap_interpret.train_score == 1
     assert shap_interpret.test_score == pytest.approx(0.833, 0.01)
 
     # Check expected shap values
     assert (np.mean(np.abs(shap_interpret.shap_values_test), axis=0) == [0, 0, 0.5]).all()
     assert (np.mean(np.abs(shap_interpret.shap_values_train), axis=0) == [0, 0, 0.5]).all()
@@ -132,28 +78,24 @@
     assert not (isinstance(ax5, list))
     assert not (isinstance(ax6, list))
     assert isinstance(ax7, list) and len(ax7) == 2
     assert isinstance(ax8, list) and len(ax8) == 2
 
 
 def test_shap_interpret_lin_models(
-    fitted_lin, X_train, y_train, X_test, y_test, expected_feature_importance_lin_models
+    fitted_logistic_regression, X_train, y_train, X_test, y_test, expected_feature_importance_lin_models, random_state
 ):
     """
     Test.
     """
     class_names = ["neg", "pos"]
 
-    shap_interpret = ShapModelInterpreter(fitted_lin)
+    shap_interpret = ShapModelInterpreter(fitted_logistic_regression, random_state=random_state)
     shap_interpret.fit(X_train, X_test, y_train, y_test, class_names=class_names)
 
-    # Check parameters
-    assert shap_interpret.fitted
-    shap_interpret._check_if_fitted
-
     assert shap_interpret.class_names == class_names
     assert shap_interpret.train_score == 1
     assert shap_interpret.test_score == pytest.approx(0.833, 0.01)
 
     # Check expected shap values
     assert (np.round(np.mean(np.abs(shap_interpret.shap_values_test), axis=0), 2) == [0, 0, 0.4]).all()
     assert (np.round(np.mean(np.abs(shap_interpret.shap_values_train), axis=0), 2) == [0, 0, 0.4]).all()
@@ -181,82 +123,72 @@
     assert not (isinstance(ax5, list))
     assert not (isinstance(ax6, list))
     assert isinstance(ax7, list) and len(ax7) == 2
     assert isinstance(ax8, list) and len(ax8) == 2
 
 
 def test_shap_interpret_fit_compute_lin_models(
-    fitted_lin, X_train, y_train, X_test, y_test, expected_feature_importance_lin_models
+    fitted_logistic_regression, X_train, y_train, X_test, y_test, expected_feature_importance_lin_models, random_state
 ):
     """
     Test.
     """
     class_names = ["neg", "pos"]
 
-    shap_interpret = ShapModelInterpreter(fitted_lin)
+    shap_interpret = ShapModelInterpreter(fitted_logistic_regression, random_state=random_state)
     importance_df = shap_interpret.fit_compute(X_train, X_test, y_train, y_test, class_names=class_names)
     importance_df = importance_df.round(2)
 
-    # Check parameters
-    assert shap_interpret.fitted
-    shap_interpret._check_if_fitted
-
     assert shap_interpret.class_names == class_names
     assert shap_interpret.train_score == 1
 
     assert shap_interpret.test_score == pytest.approx(0.833, 0.01)
 
     # Check expected shap values
     assert (np.round(np.mean(np.abs(shap_interpret.shap_values_test), axis=0), 2) == [0, 0, 0.4]).all()
     assert (np.round(np.mean(np.abs(shap_interpret.shap_values_train), axis=0), 2) == [0, 0, 0.4]).all()
 
     pd.testing.assert_frame_equal(expected_feature_importance_lin_models, importance_df)
 
 
-def test_shap_interpret_fit_compute(fitted_tree, X_train, y_train, X_test, y_test, expected_feature_importance):
+def test_shap_interpret_fit_compute(
+    fitted_tree, X_train, y_train, X_test, y_test, expected_feature_importance, random_state
+):
     """
     Test.
     """
     class_names = ["neg", "pos"]
 
-    shap_interpret = ShapModelInterpreter(fitted_tree)
+    shap_interpret = ShapModelInterpreter(fitted_tree, random_state=random_state)
     importance_df = shap_interpret.fit_compute(X_train, X_test, y_train, y_test, class_names=class_names)
 
-    # Check parameters
-    assert shap_interpret.fitted
-    shap_interpret._check_if_fitted
-
     assert shap_interpret.class_names == class_names
     assert shap_interpret.train_score == 1
     assert shap_interpret.test_score == pytest.approx(0.833, 0.01)
 
     # Check expected shap values
     assert (np.mean(np.abs(shap_interpret.shap_values_test), axis=0) == [0, 0, 0.5]).all()
     assert (np.mean(np.abs(shap_interpret.shap_values_train), axis=0) == [0, 0, 0.5]).all()
 
     pd.testing.assert_frame_equal(expected_feature_importance, importance_df)
 
 
 @pytest.mark.skipif(os.environ.get("SKIP_LIGHTGBM") == "true", reason="LightGBM tests disabled")
-def test_shap_interpret_complex_data(complex_data_split, complex_fitted_lightgbm):
+def test_shap_interpret_complex_data(complex_data_split_with_categorical, complex_fitted_lightgbm, random_state):
     """
     Test lightgbm.
     """
     class_names = ["neg", "pos"]
-    X_train, X_test, y_train, y_test = complex_data_split
+    X_train, X_test, y_train, y_test = complex_data_split_with_categorical
 
-    shap_interpret = ShapModelInterpreter(complex_fitted_lightgbm, verbose=50)
+    shap_interpret = ShapModelInterpreter(complex_fitted_lightgbm, verbose=1, random_state=random_state)
     importance_df = shap_interpret.fit_compute(
         X_train, X_test, y_train, y_test, class_names=class_names, approximate=False, check_additivity=False
     )
 
-    # Check parameters
-    assert shap_interpret.fitted
-    shap_interpret._check_if_fitted
-
     assert shap_interpret.class_names == class_names
     assert importance_df.shape[0] == X_train.shape[1]
 
     # Check if plots work for such dataset
     ax1 = shap_interpret.plot("importance", target_set="test", show=False)
     ax2 = shap_interpret.plot("summary", target_set="test", show=False)
     ax3 = shap_interpret.plot("dependence", target_columns="f2_missing", target_set="test", show=False)
```

### Comparing `probatus-3.0.0/tests/interpret/test_shap_dependence.py` & `probatus-3.0.1/tests/interpret/test_shap_dependence.py`

 * *Files 10% similar despite different names*

```diff
@@ -67,21 +67,21 @@
             [-0.108687, 0.081187, -0.205833],
             [-0.092020, -0.164646, -0.176667],
         ]
     )
 
 
 @pytest.fixture(scope="function")
-def clf(X_y):
+def clf(X_y, random_state):
     """
     Fixture.
     """
     X, y = X_y
 
-    model = RandomForestClassifier(random_state=42, n_estimators=10, max_depth=5)
+    model = RandomForestClassifier(random_state=random_state, n_estimators=10, max_depth=5)
 
     model.fit(X, y)
     return model
 
 
 @pytest.fixture(scope="function")
 def expected_feat_importances():
@@ -93,58 +93,58 @@
             "Feature Name": {0: 2, 1: 1, 2: 0},
             "Shap absolute importance": {0: 0.2199, 1: 0.1271, 2: 0.1022},
             "Shap signed importance": {0: 0.0292, 1: -0.0149, 2: -0.0076},
         }
     )
 
 
-def test_not_fitted(clf):
+def test_not_fitted(clf, random_state):
     """
     Test.
     """
-    plotter = DependencePlotter(clf)
+    plotter = DependencePlotter(clf, random_state)
     assert plotter.fitted is False
 
 
 @pytest.mark.skipif(os.environ.get("SKIP_LIGHTGBM") == "true", reason="LightGBM tests disabled")
-def test_fit_complex(complex_data_split, complex_fitted_lightgbm):
+def test_fit_complex(complex_data_split, complex_fitted_lightgbm, random_state):
     """
     Test.
     """
-    X_train, X_test, y_train, y_test = complex_data_split
+    _, X_test, _, y_test = complex_data_split
 
-    plotter = DependencePlotter(complex_fitted_lightgbm)
+    plotter = DependencePlotter(complex_fitted_lightgbm, random_state=random_state)
 
     plotter.fit(X_test, y_test)
 
     pd.testing.assert_frame_equal(plotter.X, X_test)
     pd.testing.assert_series_equal(plotter.y, pd.Series(y_test, index=X_test.index))
     assert plotter.fitted is True
 
     # Check if plotting does not cause errors
     _ = plotter.plot(feature="f2_missing", show=False)
 
 
-def test_get_X_y_shap_with_q_cut_normal(X_y, clf):
+def test_get_X_y_shap_with_q_cut_normal(X_y, clf, random_state):
     """
     Test.
     """
     X, y = X_y
 
-    plotter = DependencePlotter(clf).fit(X, y)
+    plotter = DependencePlotter(clf, random_state).fit(X, y)
     plotter.min_q, plotter.max_q = 0, 1
 
-    X_cut, y_cut, shap_val = plotter._get_X_y_shap_with_q_cut(0)
+    X_cut, y_cut, _ = plotter._get_X_y_shap_with_q_cut(0)
     assert np.isclose(X[0], X_cut).all()
     assert y.equals(y_cut)
 
     plotter.min_q = 0.2
     plotter.max_q = 0.8
 
-    X_cut, y_cut, shap_val = plotter._get_X_y_shap_with_q_cut(0)
+    X_cut, y_cut, _ = plotter._get_X_y_shap_with_q_cut(0)
     assert np.isclose(
         X_cut,
         [
             -1.48382902,
             -0.44947744,
             -1.38101231,
             -0.18261804,
@@ -154,61 +154,61 @@
             -2.10917352,
             -1.25945582,
         ],
     ).all()
     assert np.equal(y_cut.values, [1, 0, 0, 1, 1, 0, 0, 0, 0]).all()
 
 
-def test_get_X_y_shap_with_q_cut_unfitted(clf):
+def test_get_X_y_shap_with_q_cut_unfitted(clf, random_state):
     """
     Test.
     """
-    plotter = DependencePlotter(clf)
+    plotter = DependencePlotter(clf, random_state)
     with pytest.raises(NotFittedError):
         plotter._get_X_y_shap_with_q_cut(0)
 
 
-def test_get_X_y_shap_with_q_cut_input(X_y, clf):
+def test_get_X_y_shap_with_q_cut_input(X_y, clf, random_state):
     """
     Test.
     """
-    plotter = DependencePlotter(clf).fit(X_y[0], X_y[1])
+    plotter = DependencePlotter(clf, random_state).fit(X_y[0], X_y[1])
     with pytest.raises(ValueError):
         plotter._get_X_y_shap_with_q_cut("not a feature")
 
 
-def test_plot_normal(X_y, clf):
+def test_plot_normal(X_y, clf, random_state):
     """
     Test.
     """
-    plotter = DependencePlotter(clf).fit(X_y[0], X_y[1])
+    plotter = DependencePlotter(clf, random_state).fit(X_y[0], X_y[1])
     _ = plotter.plot(feature=0)
 
 
-def test_plot_class_names(X_y, clf):
+def test_plot_class_names(X_y, clf, random_state):
     """
     Test.
     """
-    plotter = DependencePlotter(clf).fit(X_y[0], X_y[1], class_names=["a", "b"])
+    plotter = DependencePlotter(clf, random_state).fit(X_y[0], X_y[1], class_names=["a", "b"])
     _ = plotter.plot(feature=0)
     assert plotter.class_names == ["a", "b"]
 
 
-def test_plot_input(X_y, clf):
+def test_plot_input(X_y, clf, random_state):
     """
     Test.
     """
-    plotter = DependencePlotter(clf).fit(X_y[0], X_y[1])
+    plotter = DependencePlotter(clf, random_state).fit(X_y[0], X_y[1])
     with pytest.raises(ValueError):
         plotter.plot(feature="not a feature")
     with pytest.raises(TypeError):
         plotter.plot(feature=0, bins=5.0)
     with pytest.raises(ValueError):
         plotter.plot(feature=0, min_q=1, max_q=0)
 
 
-def test__repr__(clf):
+def test__repr__(clf, random_state):
     """
     Test string representation.
     """
-    plotter = DependencePlotter(clf)
+    plotter = DependencePlotter(clf, random_state)
     assert str(plotter) == "Shap dependence plotter for RandomForestClassifier"
```

### Comparing `probatus-3.0.0/tests/utils/test_utils_array_funcs.py` & `probatus-3.0.1/tests/utils/test_utils_array_funcs.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,23 +221,23 @@
 def test_preprocess_labels():
     """
     Test.
     """
     y1 = pd.Series([1, 0, 1, 0, 1])
     index_1 = np.array([5, 4, 3, 2, 1])
 
-    y1_output = preprocess_labels(y1, y_name="y1", index=index_1, verbose=150)
+    y1_output = preprocess_labels(y1, y_name="y1", index=index_1, verbose=2)
     pd.testing.assert_series_equal(y1_output, pd.Series([1, 0, 1, 0, 1], index=index_1))
 
     y2 = [False, False, False, False, False]
-    y2_output = preprocess_labels(y2, y_name="y2", verbose=150)
+    y2_output = preprocess_labels(y2, y_name="y2", verbose=2)
     pd.testing.assert_series_equal(y2_output, pd.Series(y2))
 
     y3 = np.array([0, 1, 2, 3, 4])
-    y3_output = preprocess_labels(y3, y_name="y3", verbose=150)
+    y3_output = preprocess_labels(y3, y_name="y3", verbose=2)
     pd.testing.assert_series_equal(y3_output, pd.Series(y3))
 
     y4 = pd.Series(["2", "1", "3", "2", "1"])
     index4 = pd.Index([0, 2, 1, 3, 4])
     y4_output = preprocess_labels(y4, y_name="y4", index=index4, verbose=0)
     pd.testing.assert_series_equal(y4_output, pd.Series(["2", "3", "1", "2", "1"], index=index4))
 
@@ -248,21 +248,19 @@
     """
     X1 = pd.DataFrame({"cat": ["a", "b", "c"], "missing": [1, np.nan, 2], "num_1": [1, 2, 3]})
 
     target_column_names_X1 = ["1", "2", "3"]
     X1_expected_output = pd.DataFrame({"1": ["a", "b", "c"], "2": [1, np.nan, 2], "3": [1, 2, 3]})
 
     X1_expected_output["1"] = X1_expected_output["1"].astype("category")
-    X1_output, output_column_names_X1 = preprocess_data(
-        X1, X_name="X1", column_names=target_column_names_X1, verbose=150
-    )
+    X1_output, output_column_names_X1 = preprocess_data(X1, X_name="X1", column_names=target_column_names_X1, verbose=2)
     assert target_column_names_X1 == output_column_names_X1
     pd.testing.assert_frame_equal(X1_output, X1_expected_output)
 
     X2 = np.array([[1, 3, 2], [1, 2, 2], [1, 2, 3]])
 
     target_column_names_X1 = [0, 1, 2]
     X2_expected_output = pd.DataFrame(X2, columns=target_column_names_X1)
-    X2_output, output_column_names_X2 = preprocess_data(X2, X_name="X2", column_names=None, verbose=150)
+    X2_output, output_column_names_X2 = preprocess_data(X2, X_name="X2", column_names=None, verbose=2)
 
     assert target_column_names_X1 == output_column_names_X2
     pd.testing.assert_frame_equal(X2_output, X2_expected_output)
```

