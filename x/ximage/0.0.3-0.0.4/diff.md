# Comparing `tmp/ximage-0.0.3.tar.gz` & `tmp/ximage-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ximage-0.0.3.tar", last modified: Mon Dec  4 15:30:54 2023, max compression
+gzip compressed data, was "ximage-0.0.4.tar", last modified: Tue Apr  2 16:31:01 2024, max compression
```

## Comparing `ximage-0.0.3.tar` & `ximage-0.0.4.tar`

### file list

```diff
@@ -1,54 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 15:30:54.688724 ximage-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2023-12-04 15:30:46.000000 ximage-0.0.3/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)     2262 2023-12-04 15:30:46.000000 ximage-0.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      712 2023-12-04 15:30:46.000000 ximage-0.0.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      465 2023-12-04 15:30:46.000000 ximage-0.0.3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      273 2023-12-04 15:30:46.000000 ximage-0.0.3/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)      150 2023-12-04 15:30:46.000000 ximage-0.0.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2023-12-04 15:30:46.000000 ximage-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       51 2023-12-04 15:30:46.000000 ximage-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    13340 2023-12-04 15:30:54.688724 ximage-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9613 2023-12-04 15:30:46.000000 ximage-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 15:30:54.680724 ximage-0.0.3/ci/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2023-12-04 15:30:46.000000 ximage-0.0.3/ci/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)      187 2023-12-04 15:30:46.000000 ximage-0.0.3/ci/environment_latest.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3420 2023-12-04 15:30:46.000000 ximage-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-04 15:30:54.688724 ximage-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-04 15:30:46.000000 ximage-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 15:30:54.680724 ximage-0.0.3/ximage/
--rw-r--r--   0 runner    (1001) docker     (127)      458 2023-12-04 15:30:46.000000 ximage-0.0.3/ximage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-12-04 15:30:54.000000 ximage-0.0.3/ximage/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 15:30:54.684724 ximage-0.0.3/ximage/accessor/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2023-12-04 15:30:46.000000 ximage-0.0.3/ximage/accessor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5659 2023-12-04 15:30:46.000000 ximage-0.0.3/ximage/accessor/methods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 15:30:54.684724 ximage-0.0.3/ximage/labels/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2023-12-04 15:30:46.000000 ximage-0.0.3/ximage/labels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25575 2023-12-04 15:30:46.000000 ximage-0.0.3/ximage/labels/labels.py
--rw-r--r--   0 runner    (1001) docker     (127)     2718 2023-12-04 15:30:46.000000 ximage-0.0.3/ximage/labels/plot_labels.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 15:30:54.684724 ximage-0.0.3/ximage/patch/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2023-12-04 15:30:46.000000 ximage-0.0.3/ximage/patch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8927 2023-12-04 15:30:46.000000 ximage-0.0.3/ximage/patch/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    34420 2023-12-04 15:30:46.000000 ximage-0.0.3/ximage/patch/labels_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2023-12-04 15:30:46.000000 ximage-0.0.3/ximage/patch/plot2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    13938 2023-12-04 15:30:46.000000 ximage-0.0.3/ximage/patch/slices.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 15:30:54.684724 ximage-0.0.3/ximage/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 15:30:54.684724 ximage-0.0.3/ximage/tests/accessor/
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2023-12-04 15:30:46.000000 ximage-0.0.3/ximage/tests/accessor/test_accessor_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2023-12-04 15:30:46.000000 ximage-0.0.3/ximage/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 15:30:54.684724 ximage-0.0.3/ximage/tests/labels/
--rw-r--r--   0 runner    (1001) docker     (127)    20171 2023-12-04 15:30:46.000000 ximage-0.0.3/ximage/tests/labels/test_labels.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2023-12-04 15:30:46.000000 ximage-0.0.3/ximage/tests/labels/test_plot_labels.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 15:30:54.684724 ximage-0.0.3/ximage/tests/patch/
--rw-r--r--   0 runner    (1001) docker     (127)     4404 2023-12-04 15:30:46.000000 ximage-0.0.3/ximage/tests/patch/test_checks_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)    19840 2023-12-04 15:30:46.000000 ximage-0.0.3/ximage/tests/patch/test_labels_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)    13150 2023-12-04 15:30:46.000000 ximage-0.0.3/ximage/tests/patch/test_slices.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 15:30:54.684724 ximage-0.0.3/ximage/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2736 2023-12-04 15:30:46.000000 ximage-0.0.3/ximage/tests/utils/test_checks_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 15:30:54.684724 ximage-0.0.3/ximage/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2023-12-04 15:30:46.000000 ximage-0.0.3/ximage/utils/checks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 15:30:54.688724 ximage-0.0.3/ximage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13340 2023-12-04 15:30:54.000000 ximage-0.0.3/ximage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      951 2023-12-04 15:30:54.000000 ximage-0.0.3/ximage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-04 15:30:54.000000 ximage-0.0.3/ximage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      246 2023-12-04 15:30:54.000000 ximage-0.0.3/ximage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-12-04 15:30:54.000000 ximage-0.0.3/ximage.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:31:01.126219 ximage-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-02 16:30:52.000000 ximage-0.0.4/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-04-02 16:30:52.000000 ximage-0.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-02 16:30:52.000000 ximage-0.0.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-02 16:30:52.000000 ximage-0.0.4/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-02 16:30:52.000000 ximage-0.0.4/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-02 16:30:52.000000 ximage-0.0.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5498 2024-04-02 16:30:52.000000 ximage-0.0.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)    21162 2024-04-02 16:30:52.000000 ximage-0.0.4/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-02 16:30:52.000000 ximage-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-02 16:30:52.000000 ximage-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-02 16:30:52.000000 ximage-0.0.4/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    12931 2024-04-02 16:31:01.126219 ximage-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9206 2024-04-02 16:30:52.000000 ximage-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-02 16:30:52.000000 ximage-0.0.4/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4715 2024-04-02 16:30:52.000000 ximage-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 16:31:01.126219 ximage-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-02 16:30:52.000000 ximage-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:31:01.122219 ximage-0.0.4/ximage/
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-02 16:30:52.000000 ximage-0.0.4/ximage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-02 16:31:00.000000 ximage-0.0.4/ximage/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:31:01.122219 ximage-0.0.4/ximage/accessor/
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-02 16:30:52.000000 ximage-0.0.4/ximage/accessor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7500 2024-04-02 16:30:52.000000 ximage-0.0.4/ximage/accessor/methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:31:01.122219 ximage-0.0.4/ximage/labels/
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-02 16:30:52.000000 ximage-0.0.4/ximage/labels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26435 2024-04-02 16:30:52.000000 ximage-0.0.4/ximage/labels/labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-04-02 16:30:52.000000 ximage-0.0.4/ximage/labels/plot_labels.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:31:01.126219 ximage-0.0.4/ximage/patch/
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-02 16:30:52.000000 ximage-0.0.4/ximage/patch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9980 2024-04-02 16:30:52.000000 ximage-0.0.4/ximage/patch/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35303 2024-04-02 16:30:52.000000 ximage-0.0.4/ximage/patch/labels_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4419 2024-04-02 16:30:52.000000 ximage-0.0.4/ximage/patch/plot2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15161 2024-04-02 16:30:52.000000 ximage-0.0.4/ximage/patch/slices.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:31:01.126219 ximage-0.0.4/ximage/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-04-02 16:30:52.000000 ximage-0.0.4/ximage/utils/checks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:31:01.126219 ximage-0.0.4/ximage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12931 2024-04-02 16:31:01.000000 ximage-0.0.4/ximage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-02 16:31:01.000000 ximage-0.0.4/ximage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 16:31:01.000000 ximage-0.0.4/ximage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-02 16:31:01.000000 ximage-0.0.4/ximage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-02 16:31:01.000000 ximage-0.0.4/ximage.egg-info/top_level.txt
```

### Comparing `ximage-0.0.3/.gitignore` & `ximage-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `ximage-0.0.3/.pre-commit-config.yaml` & `ximage-0.0.4/.pre-commit-config.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -2,21 +2,21 @@
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.5.0
     hooks:
       - id: trailing-whitespace
       - id: end-of-file-fixer
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.1.6
+    rev: v0.3.5
     hooks:
       - id: ruff
         args: [--fix]
 
   - repo: https://github.com/psf/black
-    rev: 23.11.0
+    rev: 24.3.0
     hooks:
     - id: black
       language_version: python3
 
   - repo: https://github.com/keewis/blackdoc
     rev: v0.3.9
     hooks:
```

### Comparing `ximage-0.0.3/LICENSE` & `ximage-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ximage-0.0.3/PKG-INFO` & `ximage-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ximage
-Version: 0.0.3
+Version: 0.0.4
 Summary: xarray-based tools for image/video processing
 Author-email: Gionata Ghiggi <gionata.ghiggi@epfl.ch>
 License: MIT License
         
         Copyright (c) 2023 Gionata Ghiggi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -26,29 +26,28 @@
         SOFTWARE.
         
 Project-URL: homepage, https://github.com/ghiggi/ximage
 Project-URL: repository, https://github.com/ghiggi/ximage
 Project-URL: source, https://github.com/ghiggi/ximage
 Project-URL: tracker, https://github.com/ghiggi/ximage/issues
 Project-URL: documentation, https://ximage.readthedocs.io
-Project-URL: changelog, https://github.com/ghiggi/ximage/CHANGELOG.md
+Project-URL: changelog, https://github.com/ghiggi/ximage/blob/main/CHANGELOG.md
 Keywords: image,video,labelling,patch,extraction
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Requires-Python: >=3.8
@@ -57,14 +56,15 @@
 Requires-Dist: xarray
 Requires-Dist: dask
 Requires-Dist: dask-image
 Requires-Dist: matplotlib
 Requires-Dist: scikit-image
 Provides-Extra: dev
 Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: loghub; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: black[jupyter]; extra == "dev"
 Requires-Dist: blackdoc; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: codespell; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
@@ -88,41 +88,39 @@
 | Activity             | [![PyPI Downloads](https://img.shields.io/pypi/dm/ximage.svg?label=PyPI%20downloads&style=flat)](https://pypi.org/project/ximage/) [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/ximage.svg?label=Conda%20downloads&style=flat)](https://anaconda.org/conda-forge/ximage) |
 | Python Versions      | [![Python Versions](https://img.shields.io/badge/Python-3.8%20%203.9%20%203.10%20%203.11%20%203.12-blue?style=flat)](https://www.python.org/downloads/) |
 | Supported Systems    | [![Linux](https://img.shields.io/github/actions/workflow/status/ghiggi/ximage/.github/workflows/tests.yml?label=Linux&style=flat)](https://github.com/ghiggi/ximage/actions/workflows/tests.yml) [![macOS](https://img.shields.io/github/actions/workflow/status/ghiggi/ximage/.github/workflows/tests.yml?label=macOS&style=flat)](https://github.com/ghiggi/ximage/actions/workflows/tests.yml) [![Windows](https://img.shields.io/github/actions/workflow/status/ghiggi/ximage/.github/workflows/tests_windows.yml?label=Windows&style=flat)](https://github.com/ghiggi/ximage/actions/workflows/tests_windows.yml) |
 | Project Status       | [![Project Status](https://www.repostatus.org/badges/latest/active.svg?style=flat)](https://www.repostatus.org/#active) |
 | Build Status         | [![Tests](https://github.com/ghiggi/ximage/actions/workflows/tests.yml/badge.svg?style=flat)](https://github.com/ghiggi/ximage/actions/workflows/tests.yml) [![Lint](https://github.com/ghiggi/ximage/actions/workflows/lint.yml/badge.svg?style=flat)](https://github.com/ghiggi/ximage/actions/workflows/lint.yml) [![Docs](https://readthedocs.org/projects/ximage/badge/?version=latest&style=flat)](https://ximage.readthedocs.io/en/latest/) |
 | Linting              | [![Black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat)](https://github.com/psf/black) [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json&style=flat)](https://github.com/astral-sh/ruff) [![Codespell](https://img.shields.io/badge/Codespell-enabled-brightgreen?style=flat)](https://github.com/codespell-project/codespell) |
 | Code Coverage        | [![Coveralls](https://coveralls.io/repos/github/ghiggi/ximage/badge.svg?branch=main&style=flat)](https://coveralls.io/github/ghiggi/ximage?branch=main) [![Codecov](https://codecov.io/gh/ghiggi/ximage/branch/main/graph/badge.svg?style=flat)](https://codecov.io/gh/ghiggi/ximage) |
-| Code Quality         | [![Codefactor](https://www.codefactor.io/repository/github/ghiggi/ximage/badge?style=flat)](https://www.codefactor.io/repository/github/ghiggi/ximage) [![Codebeat](https://codebeat.co/badges/14ff831b-f064-4bdd-a2e2-72ffdf28a35a?style=flat)](https://codebeat.co/projects/github-com-ltelab-ximage-main) [![Codacy](https://app.codacy.com/project/badge/Grade/d823c50a7ad14268bd347b5aba384623?style=flat)](https://app.codacy.com/gh/ghiggi/ximage/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade) [![Codescene](https://codescene.io/projects/36773/status-badges/code-health?style=flat)](https://codescene.io/projects/36773) |
-| Code Review          | [![pyOpenSci](https://tinyurl.com/XXXX)](#) |
+| Code Quality         | [![Codefactor](https://www.codefactor.io/repository/github/ghiggi/ximage/badge?style=flat)](https://www.codefactor.io/repository/github/ghiggi/ximage) [![Codebeat](https://codebeat.co/badges/3eab0b92-5b00-4eb7-9834-2e5f9a083b5e?style=flat)](https://codebeat.co/projects/github-com-ghiggi-ximage-main) [![Codacy](https://app.codacy.com/project/badge/Grade/d823c50a7ad14268bd347b5aba384623?style=flat)](https://app.codacy.com/gh/ghiggi/ximage/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade) [![CodeScene](https://codescene.io/projects/41869/status-badges/code-health?style=flat)](https://codescene.io/projects/41869) |
 | License              | [![License](https://img.shields.io/github/license/ghiggi/ximage?style=flat)](https://github.com/ghiggi/ximage/blob/main/LICENSE) |
 | Community            | [![Slack](https://img.shields.io/badge/Slack-ximage-green.svg?logo=slack&style=flat)](https://join.slack.com/t/xarray-tools/shared_invite/zt-28f5r0n75-ygNZN5omemhz72NM~WKUHA) [![GitHub Discussions](https://img.shields.io/badge/GitHub-Discussions-green?logo=github&style=flat)](https://github.com/ghiggi/ximage/discussions) |
 | Citation             | [![DOI](https://zenodo.org/badge/664629093.svg?style=flat)](https://zenodo.org/records/8131553) |
 
  [**Slack**](https://join.slack.com/t/xarray-tools/shared_invite/zt-28f5r0n75-ygNZN5omemhz72NM~WKUHA) | [**Docs**](https://x-image.readthedocs.io/en/latest/)
 
-The `ximage` package is in active development. Feel free to try it out, to report issues or to suggest changes.
 
 ## ℹ️ Software Overview
 
 The software currently enables to:
 
 - label n-dimensional xarray objects
 - extract patches around n-dimensional labels
 - extract patches from n-dimensional xarray objects
 
-Join the [**DISDRODB Slack Workspace**](https://join.slack.com/t/xarray-tools/shared_invite/zt-28f5r0n75-ygNZN5omemhz72NM~WKUHA) to meet the community !
+Join the [**Slack Workspace**](https://join.slack.com/t/xarray-tools/shared_invite/zt-28f5r0n75-ygNZN5omemhz72NM~WKUHA) to meet the community !
 
 ## 🚀 Quick Start
 
 `ximage` provides an easy-to-use interface to manipulate image, videos and n-dimensional arrays with classical image processing techniques.
 
-The `ximage` xarray accessor provides a convenient way to labelling and extract patches in n-dimensional arrays ! 
+The `ximage` xarray accessor provides a convenient way to labelling and extract patches in n-dimensional arrays !
 
-##### Image labelling 
+##### Image labelling
 
 ```python
 min_value_threshold = 1
 max_value_threshold = np.inf
 min_area_threshold = 5
 max_area_threshold = np.inf
 footprint = None
@@ -192,48 +190,55 @@
     ensure_slice_size=ensure_slice_size,
     debug=debug,
     verbose=verbose,
 )
 
 ```
 
-Look at the [Tutorials][tutorial_link] to have an overview of the software !
- 
+#### 📖 Explore the ximage documentation
+
+To discover all `ximage` utilities, please read the [software documentation](https://x-image.readthedocs.io/en/latest/).
+
 ## 🛠️ Installation
 
-### pip
+### conda
 
-`ximage` can be installed via [pip][pip_link] on Linux, Mac, and Windows.
-On Windows you can install [WinPython][winpy_link] to get Python and pip
-running.
-Then, install the `ximage` package by typing the following command in the command terminal:
+ximage can be installed via [conda][conda_link] on Linux, Mac, and Windows.
+Install the package by typing the following command in the terminal:
 
 ```bash
-    pip install ximage
+conda install ximage
 ```
 
-To install the latest development version via pip, see the
-[documentation][doc_install_link].
+In case conda-forge is not set up for your system yet, see the easy to follow instructions on [conda-forge][conda_forge_link].
 
-### conda [NOT YET AVAILABLE]
+[conda_link]: https://docs.conda.io/en/latest/miniconda.html
+[conda_forge_link]: https://github.com/conda-forge/ximage-feedstock#installing-ximage
+
+### pip
 
-`ximage` can be installed via [conda][conda_link] on Linux, Mac, and Windows.
-Install the package by typing the following command in a command terminal:
+`ximage` can be installed also via [pip][pip_link] on Linux, Mac, and Windows.
+On Windows you can install [WinPython][winpy_link] to get Python and pip running.
+
+Install the `ximage` package by typing the following command in the terminal:
 
 ```bash
-    conda install ximage
+pip install ximage
 ```
 
-In case conda-forge is not set up for your system yet, see the easy to follow
-instructions on [conda-forge][conda_forge_link].
+To install the latest development version via pip, see the [documentation][dev_install_link].
+
+[pip_link]: https://pypi.org/project/gpm-api
+[winpy_link]: https://winpython.github.io/
+[dev_install_link]: https://gpm-api.readthedocs.io/en/latest/02_installation.html#installation-for-contributors
 
 ## 💭 Feedback and Contributing Guidelines
 
 If you aim to contribute or discuss the future development of ximage,
-we highly suggest to join the [**DISDRODB Slack Workspace**](https://join.slack.com/t/xarray-tools/shared_invite/zt-28f5r0n75-ygNZN5omemhz72NM~WKUHA)
+we highly suggest to join the [**Slack Workspace**](https://join.slack.com/t/xarray-tools/shared_invite/zt-28f5r0n75-ygNZN5omemhz72NM~WKUHA)
 
 Feel free to also open a [GitHub Issue](https://github.com/ghiggi/ximage/issues) or a
 [GitHub Discussion](https://github.com/ghiggi/ximage/discussions) specific to your questions or ideas.
 
 ## ✍️  Contributors
 
 * [Gionata Ghiggi](https://people.epfl.ch/gionata.ghiggi)
@@ -241,31 +246,19 @@
 
 ## Citation
 
 You can cite the `ximage` software by:
 
 > Ghiggi Gionata & Son Pham-Ba . ghiggi/ximage. Zenodo. https://doi.org/10.5281/zenodo.8131552
 
-If you want to cite a specific version, have a look at the [Zenodo site](https://doi.org/10.5281/zenodo.7753488).
+If you want to cite a specific version, have a look at the [Zenodo site](https://doi.org/10.5281/zenodo.8131552).
+
+## License
+
+The content of this repository is released under the terms of the [MIT](LICENSE) license.
 
 ## 📚 Requirements:
 
 - [xarray](https://docs.xarray.dev/en/stable/)
 - [dask](https://www.dask.org/)
 - [dask_image](https://image.dask.org/en/latest/)
 - [skimage](https://scikit-image.org/)
-
-## License
-
-The content of this repository is released under the terms of the [MIT](LICENSE) license.
-
-
-
-[pip_link]: https://pypi.org/project/ximage
-[conda_link]: https://docs.conda.io/en/latest/miniconda.html
-[conda_forge_link]: https://github.com/conda-forge/ximage-feedstock#installing-ximage
-[conda_pip]: https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-pkgs.html#installing-non-conda-packages
-[pipiflag]: https://pip-python3.readthedocs.io/en/latest/reference/pip_install.html?highlight=i#cmdoption-i
-[winpy_link]: https://winpython.github.io/
-
-[doc_link]: https://x-image.readthedocs.io
-[tutorial_link]: https://github.com/ghiggi/ximage/tree/main#tutorials-and-examples
```

### Comparing `ximage-0.0.3/README.md` & `ximage-0.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,41 +6,39 @@
 | Activity             | [![PyPI Downloads](https://img.shields.io/pypi/dm/ximage.svg?label=PyPI%20downloads&style=flat)](https://pypi.org/project/ximage/) [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/ximage.svg?label=Conda%20downloads&style=flat)](https://anaconda.org/conda-forge/ximage) |
 | Python Versions      | [![Python Versions](https://img.shields.io/badge/Python-3.8%20%203.9%20%203.10%20%203.11%20%203.12-blue?style=flat)](https://www.python.org/downloads/) |
 | Supported Systems    | [![Linux](https://img.shields.io/github/actions/workflow/status/ghiggi/ximage/.github/workflows/tests.yml?label=Linux&style=flat)](https://github.com/ghiggi/ximage/actions/workflows/tests.yml) [![macOS](https://img.shields.io/github/actions/workflow/status/ghiggi/ximage/.github/workflows/tests.yml?label=macOS&style=flat)](https://github.com/ghiggi/ximage/actions/workflows/tests.yml) [![Windows](https://img.shields.io/github/actions/workflow/status/ghiggi/ximage/.github/workflows/tests_windows.yml?label=Windows&style=flat)](https://github.com/ghiggi/ximage/actions/workflows/tests_windows.yml) |
 | Project Status       | [![Project Status](https://www.repostatus.org/badges/latest/active.svg?style=flat)](https://www.repostatus.org/#active) |
 | Build Status         | [![Tests](https://github.com/ghiggi/ximage/actions/workflows/tests.yml/badge.svg?style=flat)](https://github.com/ghiggi/ximage/actions/workflows/tests.yml) [![Lint](https://github.com/ghiggi/ximage/actions/workflows/lint.yml/badge.svg?style=flat)](https://github.com/ghiggi/ximage/actions/workflows/lint.yml) [![Docs](https://readthedocs.org/projects/ximage/badge/?version=latest&style=flat)](https://ximage.readthedocs.io/en/latest/) |
 | Linting              | [![Black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat)](https://github.com/psf/black) [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json&style=flat)](https://github.com/astral-sh/ruff) [![Codespell](https://img.shields.io/badge/Codespell-enabled-brightgreen?style=flat)](https://github.com/codespell-project/codespell) |
 | Code Coverage        | [![Coveralls](https://coveralls.io/repos/github/ghiggi/ximage/badge.svg?branch=main&style=flat)](https://coveralls.io/github/ghiggi/ximage?branch=main) [![Codecov](https://codecov.io/gh/ghiggi/ximage/branch/main/graph/badge.svg?style=flat)](https://codecov.io/gh/ghiggi/ximage) |
-| Code Quality         | [![Codefactor](https://www.codefactor.io/repository/github/ghiggi/ximage/badge?style=flat)](https://www.codefactor.io/repository/github/ghiggi/ximage) [![Codebeat](https://codebeat.co/badges/14ff831b-f064-4bdd-a2e2-72ffdf28a35a?style=flat)](https://codebeat.co/projects/github-com-ltelab-ximage-main) [![Codacy](https://app.codacy.com/project/badge/Grade/d823c50a7ad14268bd347b5aba384623?style=flat)](https://app.codacy.com/gh/ghiggi/ximage/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade) [![Codescene](https://codescene.io/projects/36773/status-badges/code-health?style=flat)](https://codescene.io/projects/36773) |
-| Code Review          | [![pyOpenSci](https://tinyurl.com/XXXX)](#) |
+| Code Quality         | [![Codefactor](https://www.codefactor.io/repository/github/ghiggi/ximage/badge?style=flat)](https://www.codefactor.io/repository/github/ghiggi/ximage) [![Codebeat](https://codebeat.co/badges/3eab0b92-5b00-4eb7-9834-2e5f9a083b5e?style=flat)](https://codebeat.co/projects/github-com-ghiggi-ximage-main) [![Codacy](https://app.codacy.com/project/badge/Grade/d823c50a7ad14268bd347b5aba384623?style=flat)](https://app.codacy.com/gh/ghiggi/ximage/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade) [![CodeScene](https://codescene.io/projects/41869/status-badges/code-health?style=flat)](https://codescene.io/projects/41869) |
 | License              | [![License](https://img.shields.io/github/license/ghiggi/ximage?style=flat)](https://github.com/ghiggi/ximage/blob/main/LICENSE) |
 | Community            | [![Slack](https://img.shields.io/badge/Slack-ximage-green.svg?logo=slack&style=flat)](https://join.slack.com/t/xarray-tools/shared_invite/zt-28f5r0n75-ygNZN5omemhz72NM~WKUHA) [![GitHub Discussions](https://img.shields.io/badge/GitHub-Discussions-green?logo=github&style=flat)](https://github.com/ghiggi/ximage/discussions) |
 | Citation             | [![DOI](https://zenodo.org/badge/664629093.svg?style=flat)](https://zenodo.org/records/8131553) |
 
  [**Slack**](https://join.slack.com/t/xarray-tools/shared_invite/zt-28f5r0n75-ygNZN5omemhz72NM~WKUHA) | [**Docs**](https://x-image.readthedocs.io/en/latest/)
 
-The `ximage` package is in active development. Feel free to try it out, to report issues or to suggest changes.
 
 ## ℹ️ Software Overview
 
 The software currently enables to:
 
 - label n-dimensional xarray objects
 - extract patches around n-dimensional labels
 - extract patches from n-dimensional xarray objects
 
-Join the [**DISDRODB Slack Workspace**](https://join.slack.com/t/xarray-tools/shared_invite/zt-28f5r0n75-ygNZN5omemhz72NM~WKUHA) to meet the community !
+Join the [**Slack Workspace**](https://join.slack.com/t/xarray-tools/shared_invite/zt-28f5r0n75-ygNZN5omemhz72NM~WKUHA) to meet the community !
 
 ## 🚀 Quick Start
 
 `ximage` provides an easy-to-use interface to manipulate image, videos and n-dimensional arrays with classical image processing techniques.
 
-The `ximage` xarray accessor provides a convenient way to labelling and extract patches in n-dimensional arrays ! 
+The `ximage` xarray accessor provides a convenient way to labelling and extract patches in n-dimensional arrays !
 
-##### Image labelling 
+##### Image labelling
 
 ```python
 min_value_threshold = 1
 max_value_threshold = np.inf
 min_area_threshold = 5
 max_area_threshold = np.inf
 footprint = None
@@ -110,48 +108,55 @@
     ensure_slice_size=ensure_slice_size,
     debug=debug,
     verbose=verbose,
 )
 
 ```
 
-Look at the [Tutorials][tutorial_link] to have an overview of the software !
- 
+#### 📖 Explore the ximage documentation
+
+To discover all `ximage` utilities, please read the [software documentation](https://x-image.readthedocs.io/en/latest/).
+
 ## 🛠️ Installation
 
-### pip
+### conda
 
-`ximage` can be installed via [pip][pip_link] on Linux, Mac, and Windows.
-On Windows you can install [WinPython][winpy_link] to get Python and pip
-running.
-Then, install the `ximage` package by typing the following command in the command terminal:
+ximage can be installed via [conda][conda_link] on Linux, Mac, and Windows.
+Install the package by typing the following command in the terminal:
 
 ```bash
-    pip install ximage
+conda install ximage
 ```
 
-To install the latest development version via pip, see the
-[documentation][doc_install_link].
+In case conda-forge is not set up for your system yet, see the easy to follow instructions on [conda-forge][conda_forge_link].
 
-### conda [NOT YET AVAILABLE]
+[conda_link]: https://docs.conda.io/en/latest/miniconda.html
+[conda_forge_link]: https://github.com/conda-forge/ximage-feedstock#installing-ximage
+
+### pip
 
-`ximage` can be installed via [conda][conda_link] on Linux, Mac, and Windows.
-Install the package by typing the following command in a command terminal:
+`ximage` can be installed also via [pip][pip_link] on Linux, Mac, and Windows.
+On Windows you can install [WinPython][winpy_link] to get Python and pip running.
+
+Install the `ximage` package by typing the following command in the terminal:
 
 ```bash
-    conda install ximage
+pip install ximage
 ```
 
-In case conda-forge is not set up for your system yet, see the easy to follow
-instructions on [conda-forge][conda_forge_link].
+To install the latest development version via pip, see the [documentation][dev_install_link].
+
+[pip_link]: https://pypi.org/project/gpm-api
+[winpy_link]: https://winpython.github.io/
+[dev_install_link]: https://gpm-api.readthedocs.io/en/latest/02_installation.html#installation-for-contributors
 
 ## 💭 Feedback and Contributing Guidelines
 
 If you aim to contribute or discuss the future development of ximage,
-we highly suggest to join the [**DISDRODB Slack Workspace**](https://join.slack.com/t/xarray-tools/shared_invite/zt-28f5r0n75-ygNZN5omemhz72NM~WKUHA)
+we highly suggest to join the [**Slack Workspace**](https://join.slack.com/t/xarray-tools/shared_invite/zt-28f5r0n75-ygNZN5omemhz72NM~WKUHA)
 
 Feel free to also open a [GitHub Issue](https://github.com/ghiggi/ximage/issues) or a
 [GitHub Discussion](https://github.com/ghiggi/ximage/discussions) specific to your questions or ideas.
 
 ## ✍️  Contributors
 
 * [Gionata Ghiggi](https://people.epfl.ch/gionata.ghiggi)
@@ -159,31 +164,19 @@
 
 ## Citation
 
 You can cite the `ximage` software by:
 
 > Ghiggi Gionata & Son Pham-Ba . ghiggi/ximage. Zenodo. https://doi.org/10.5281/zenodo.8131552
 
-If you want to cite a specific version, have a look at the [Zenodo site](https://doi.org/10.5281/zenodo.7753488).
+If you want to cite a specific version, have a look at the [Zenodo site](https://doi.org/10.5281/zenodo.8131552).
+
+## License
+
+The content of this repository is released under the terms of the [MIT](LICENSE) license.
 
 ## 📚 Requirements:
 
 - [xarray](https://docs.xarray.dev/en/stable/)
 - [dask](https://www.dask.org/)
 - [dask_image](https://image.dask.org/en/latest/)
 - [skimage](https://scikit-image.org/)
-
-## License
-
-The content of this repository is released under the terms of the [MIT](LICENSE) license.
-
-
-
-[pip_link]: https://pypi.org/project/ximage
-[conda_link]: https://docs.conda.io/en/latest/miniconda.html
-[conda_forge_link]: https://github.com/conda-forge/ximage-feedstock#installing-ximage
-[conda_pip]: https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-pkgs.html#installing-non-conda-packages
-[pipiflag]: https://pip-python3.readthedocs.io/en/latest/reference/pip_install.html?highlight=i#cmdoption-i
-[winpy_link]: https://winpython.github.io/
-
-[doc_link]: https://x-image.readthedocs.io
-[tutorial_link]: https://github.com/ghiggi/ximage/tree/main#tutorials-and-examples
```

### Comparing `ximage-0.0.3/pyproject.toml` & `ximage-0.0.4/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -21,90 +21,81 @@
     "Operating System :: OS Independent",
     "Operating System :: Unix",
     "Operating System :: Microsoft",
     "Operating System :: MacOS",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Image Processing",
 ]
 keywords = ["image", "video", "labelling", "patch", "extraction"]
 dependencies = [
     "xarray",
     "dask",
     "dask-image",
-	"matplotlib",
+    "matplotlib",
     "scikit-image",
 ]
 requires-python = ">=3.8"
 dynamic = ["version"]
 
 [project.optional-dependencies]
-dev = ["pre-commit",
+dev = ["pre-commit", "loghub",
        "black", "black[jupyter]", "blackdoc", "ruff", "codespell",
        "pytest", "pytest-cov", "pytest-mock", "pydantic",
        "pip-tools", "bumpver", "twine",
        "setuptools>=61.0.0", "wheel",
        "sphinx", "sphinx-gallery", "sphinx_rtd_theme", "nbsphinx"]
 
 [project.urls]
 homepage = "https://github.com/ghiggi/ximage"
 repository = "https://github.com/ghiggi/ximage"
 source = "https://github.com/ghiggi/ximage"
 tracker = "https://github.com/ghiggi/ximage/issues"
 documentation = "https://ximage.readthedocs.io"
-changelog = "https://github.com/ghiggi/ximage/CHANGELOG.md"
+changelog = "https://github.com/ghiggi/ximage/blob/main/CHANGELOG.md"
 
 [tool.setuptools_scm]
 write_to = "ximage/_version.py"
 
 [tool.setuptools]
 license-files = ["LICENSE"]
-packages = ["ximage"] # explicitly list the packages in modules
+
+[tool.setuptools.packages.find]
+include = ["ximage*"]
 
 [tool.pytest.ini_options]
 addopts = "--cov --cov-report term-missing --cov-report xml --cov-report lcov:lcov.info"
 
 [tool.black]
-line-length = 100
+line-length = 120
+
 # skip-string-normalization = true
 target-version = [
-    "py37",
     "py38",
     "py39",
     "py310",
     "py311",
 ]
 
 [tool.ruff]
-select = ["F",
-	  "E",
-	  "I",
-	  "W",
-	  "UP",
-	  "Q",
-	  # "SIM",
-	  # "PTH",
-	  #"RET",
-	 ]
-ignore = ["E722"]
+
 line-length = 120
-# Allow autofix for all enabled rules (when `--fix`) is provided.
-fixable = ["A", "B", "C", "D", "E", "F", "G", "I", "N", "Q", "S", "T", "W", "ANN", "ARG", "BLE", "COM", "DJ", "DTZ", "EM", "ERA", "EXE", "FBT", "ICN", "INP", "ISC", "NPY", "PD", "PGH", "PIE", "PL", "PT", "PTH", "PYI", "RET", "RSE", "RUF", "SIM", "SLF", "TCH", "TID", "TRY", "UP", "YTT"]
-unfixable = []
+indent-width = 4
+
+# Addional file to be formatted by ruff (in addition to *py)
+extend-include = ["*.ipynb"]
+
 # Exclude a variety of commonly ignored directories.
 exclude = [
-    "dev*",
-    "ximage/test*",
     ".bzr",
     ".direnv",
     ".eggs",
     ".git",
     ".hg",
     ".mypy_cache",
     ".nox",
@@ -114,14 +105,109 @@
     ".svn",
     ".tox",
     ".venv",
     "__pypackages__",
     "_build",
     "buck-out",
     "build",
+    "docs",
     "dist",
     "node_modules",
     "venv",
 ]
 
+[tool.ruff.format]
+
+# Enable reformatting of code snippets in docstrings.
+docstring-code-format = true
+
+[tool.ruff.lint]
+
+select = [
+    # pydocstyle
+    "D",
+    # Pyflakes
+    "F",
+    # pycodestyle
+    "E",
+    "W",
+    # isort
+    "I",
+    # pyupgrade
+    "UP",
+    # flake8-quotes
+    "Q",
+    # flake8-bugbear
+    "B",
+    # flake8-return
+    "RET",
+    # flake8-unused-arguments
+    "ARG",
+    # flake8-raise
+    "RSE",
+    # flake8-pytest-style
+    "PT",
+    # flake8-simplify
+    "SIM",
+    # Perflint
+    "PERF",
+    # pandas-vet
+    "PD",
+    # pylint
+    "PL",
+    # flake8-commas
+    "COM",
+    # flake8-slots
+    "SLOT",
+    # flake8-comprehensions
+    "C4",
+    # Ruff custom rules
+    "RUF"
+
+    #---------------------
+    #### Future rules ####
+    # flake8-use-pathlib
+    # "PTH",
+    # NumPy-specific rules  (for 2.0)
+    # "NPY",
+    # refurb
+    # "FURB", # require preview
+]
+ignore = [
+    "E722",
+    "PT011", # pytest raised error must be checked if match the expected error msg
+    "PERF203",
+    "B904",
+
+    # Docstyle Rules
+    "D404", # Docstring can't start with "This"
+    "D401", # First sentence must be in imperative mood
+
+    # Complexity rules
+    "PLR0913",
+    "PLR2004",
+    "PLR0912",
+    "PLR0915",
+]
+
+# Allow autofix for all enabled rules (when `--fix`) is provided.
+fixable = ["ALL"]
+unfixable = []
+
+[tool.ruff.lint.pydocstyle]
+convention = "numpy"
+
+[tool.ruff.lint.per-file-ignores]
+
+# Ignore `E402` (import violations) in all Jupyter Notebooks.
+"*.ipynb" = ["E402"]
+
+# Rules to ignore in test files
+"test_*.py" = [
+    "ARG",  # avoid problems with fixtures
+    "D100", "D101","D102", "D103", "D104", "D105",  # Missing docstrings
+]
+"setup.py" = ["D100"]
+"*__init__.py" = ["D104"]
+
 [tool.codespell]
     ignore-words-list = 'nD'
```

### Comparing `ximage-0.0.3/ximage/labels/labels.py` & `ximage-0.0.4/ximage/labels/labels.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,35 @@
-#!/usr/bin/env python3
-"""
-Created on Wed Oct 19 19:34:53 2022
+# -----------------------------------------------------------------------------.
+# MIT License
+
+# Copyright (c) 2024 ximage developers
+#
+# This file is part of ximage.
+
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
+# -----------------------------------------------------------------------------.
+"""Labels identification."""
 
-@author: ghiggi
-"""
 # import dask_image.ndmeasure
 # from dask_image.ndmeasure import as dask_label_image
 import dask.array
 import dask_image.ndmeasure
 import numpy as np
 import xarray as xr
 from skimage.measure import label as label_image
@@ -26,15 +48,15 @@
 
 def _mask_buffer(mask, footprint):
     """Dilate the mask by n pixel in all directions.
 
     If footprint = 0 or None, no dilation occur.
     If footprint is a positive integer, it create a disk(footprint)
     If footprint is a 2D array, it must represent the neighborhood expressed
-    as a 2-D array of 1’s and 0’s.
+    as a 2-D array of 1's and 0's.
     For more info: https://scikit-image.org/docs/stable/api/skimage.morphology.html#skimage.morphology.binary_dilation
 
     """
     # scikitimage > 0.19
     if not isinstance(footprint, (int, np.ndarray, type(None))):
         raise TypeError("`footprint` must be an integer, numpy 2D array or None.")
     if isinstance(footprint, np.ndarray) and footprint.ndim != 2:
@@ -54,17 +76,15 @@
     shape = arr.shape
     if len(shape) != 2:
         raise ValueError("Expecting a 2D array.")
     if np.any(np.array(shape) == 0):
         raise ValueError("Expecting non-zero dimensions.")
 
     # Convert to numpy array
-    arr = np.asanyarray(arr)
-
-    return arr
+    return np.asanyarray(arr)
 
 
 def _no_labels_result(arr):
     """Define results for array without labels."""
     labels = np.zeros(arr.shape)
     n_labels = 0
     values = []
@@ -107,24 +127,24 @@
         ]
         if stats not in valid_stats:
             raise ValueError(f"Valid 'stats' values are: {valid_stats}.")
     # TODO: check stats function works on a dummy array (reduce to single value)
     return stats
 
 
-def _get_label_value_stats(
-    arr, label_arr, label_indices=None, stats="area", labeled_comprehension_kwargs={}
-):
+def _get_label_value_stats(arr, label_arr, label_indices=None, stats="area", labeled_comprehension_kwargs=None):
     """Compute label value statistics over which to later sort on.
 
     If label_indices is None, by default would return the stats of the entire array
     If label_indices is 0, return nan
     If label_indices is not inside label_arr, return 0
     """
     # Check stats argument and label indices
+    if labeled_comprehension_kwargs is None:
+        labeled_comprehension_kwargs = {}
     stats = _check_stats(stats)
     if label_indices is None:
         label_indices = np.unique(label_arr)
     # Compute labels stats values
     if callable(stats):
         labeled_comprehension_kwargs.setdefault("out_dtype", float)
         labeled_comprehension_kwargs.setdefault("default", None)
@@ -136,29 +156,28 @@
             func=stats,
             **labeled_comprehension_kwargs,
         )
     else:
         func = getattr(dask_image.ndmeasure, stats)
         values = func(image=arr, label_image=label_arr, index=label_indices)
     # Compute values
-    values = values.compute()
-    # Return values
-    return values
+    return values.compute()
 
 
 def _get_labels_stats(
     arr,
     label_arr,
     label_indices=None,
     stats="area",
     sort_decreasing=True,
-    labeled_comprehension_kwargs={},
+    labeled_comprehension_kwargs=None,
 ):
     """Return label and label statistics sorted by statistic value."""
-
+    if labeled_comprehension_kwargs is None:
+        labeled_comprehension_kwargs = {}
     if label_indices is None:
         label_indices = np.unique(label_arr)
 
     # Get labels area values
     values = _get_label_value_stats(
         arr,
         label_arr=label_arr,
@@ -184,29 +203,26 @@
 
     """
     # TODO:  Remove keys not in arr to speed up maybe
     return np.vectorize(my_dict.__getitem__)(arr)
 
 
 def _get_labels_with_requested_occurrence(label_arr, vmin, vmax):
-    "Get label indices with requested occurrence."
+    """Get label indices with requested occurrence."""
     # Compute label occurrence
     label_indices, label_occurrence = np.unique(label_arr, return_counts=True)
 
     # Remove label 0 and associate pixel count if present
     if label_indices[0] == 0:
         label_indices = label_indices[1:]
         label_occurrence = label_occurrence[1:]
     # Get index with required occurrence
-    valid_area_indices = np.where(
-        np.logical_and(label_occurrence >= vmin, label_occurrence <= vmax)
-    )[0]
+    valid_area_indices = np.where(np.logical_and(label_occurrence >= vmin, label_occurrence <= vmax))[0]
     # Return list of valid label indices
-    label_indices = label_indices[valid_area_indices] if len(valid_area_indices) > 0 else []
-    return label_indices
+    return label_indices[valid_area_indices] if len(valid_area_indices) > 0 else []
 
 
 def _ensure_valid_label_arr(label_arr):
     """Ensure label_arr does contain only positive values.
 
     NaN values are converted to 0.
     The output array type is int.
@@ -218,37 +234,34 @@
     label_arr[np.isnan(label_arr)] = 0
 
     # Check that label arr values are positive integers
     if not are_all_natural_numbers(label_arr.flatten(), zero_allowed=True):
         raise ValueError("The label array must contain only positive integers.")
 
     # Ensure label array is integer dtype
-    label_arr = label_arr.astype(int)
-    return label_arr
+    return label_arr.astype(int)
 
 
 def _ensure_valid_label_indices(label_indices):
     """Ensure valid label indices are integers and does not contains 0 and NaN."""
     label_indices = np.delete(label_indices, np.where(label_indices == 0)[0].flatten())
     label_indices = np.delete(label_indices, np.where(np.isnan(label_indices))[0].flatten())
-    label_indices = label_indices.astype(int)
-    return label_indices
+    return label_indices.astype(int)
 
 
 def get_label_indices(arr):
     """Get label indices from numpy.ndarray, dask.Array and xr.DataArray.
 
     It removes 0 and NaN values. Output type is int.
     """
     arr = np.asanyarray(arr)
     arr = arr[~np.isnan(arr)]
     arr = arr.astype(int)  # otherwise precision error in unique
     label_indices = np.unique(arr)
-    label_indices = _ensure_valid_label_indices(label_indices)
-    return label_indices
+    return _ensure_valid_label_indices(label_indices)
 
 
 def _check_unique_label_indices(label_indices):
     _, c = np.unique(label_indices, return_counts=True)
     if np.any(c > 1):
         raise ValueError("'label_indices' must be uniques.")
 
@@ -295,17 +308,15 @@
     # - These are some of the labels that were set to 0 because of mask or area filtering
     label_arr[label_arr > max_label] = 0
 
     # Initialize dictionary with keys corresponding to all possible labels indices
     val_dict = _get_new_label_value_dict(label_indices, max_label)
 
     # Redefine the id of the labels
-    labels_arr = _vec_translate(label_arr, val_dict)
-
-    return labels_arr
+    return _vec_translate(label_arr, val_dict)
 
 
 def _xr_redefine_label_array(dataarray, label_indices=None):
     """Relabel a xr.DataArray from 0 to len(label_indices)."""
     relabeled_arr = _np_redefine_label_array(dataarray.data, label_indices=label_indices)
     da_label = dataarray.copy()
     da_label.data = relabeled_arr
@@ -320,47 +331,44 @@
     If label_indices is not unique, raise an error !
 
     Native label values not present in label_indices are set to 0.
     The first label in label_indices becomes 1, the second 2, and so on.
     """
     if isinstance(data, xr.DataArray):
         return _xr_redefine_label_array(data, label_indices=label_indices)
-    elif isinstance(data, (np.ndarray, dask.array.Array)):
+    if isinstance(data, (np.ndarray, dask.array.Array)):
         return _np_redefine_label_array(data, label_indices=label_indices)
-    else:
-        type_data = type(data)
-        raise TypeError(f"This method does not accept {type_data}")
+    raise TypeError(f"This method does not accept {type(data)}")
 
 
 def _check_xr_obj(xr_obj, variable=None):
     """Check xarray object and variable validity."""
     # Check inputs
     if not isinstance(xr_obj, (xr.Dataset, xr.DataArray)):
         raise TypeError("'xr_obj' must be a xr.Dataset or xr.DataArray.")
     if isinstance(xr_obj, xr.Dataset):
         # Check valid variable is specified
         if variable is None:
             raise ValueError("An xr.Dataset 'variable' must be specified.")
         if variable not in xr_obj.data_vars:
             raise ValueError(f"'{variable}' is not a variable of the xr.Dataset.")
-    else:
-        if variable is not None:
-            raise ValueError("'variable' must not be specified when providing a xr.DataArray.")
+    elif variable is not None:
+        raise ValueError("'variable' must not be specified when providing a xr.DataArray.")
 
 
 def _get_labels(
     arr,
     min_value_threshold=-np.inf,
     max_value_threshold=np.inf,
     min_area_threshold=1,
     max_area_threshold=np.inf,
     footprint=None,
     sort_by="area",
     sort_decreasing=True,
-    labeled_comprehension_kwargs={},
+    labeled_comprehension_kwargs=None,
 ):
     """
     Function deriving the labels array and associated labels info.
 
     Parameters
     ----------
     arr : TYPE
@@ -379,15 +387,15 @@
         The default is np.inf.
     footprint : (int, np.ndarray or None), optional
         This argument enables to dilate the mask derived after applying
         min_value_threshold and max_value_threshold.
         If footprint = 0 or None, no dilation occur.
         If footprint is a positive integer, it create a disk(footprint)
         If footprint is a 2D array, it must represent the neighborhood expressed
-        as a 2-D array of 1’s and 0’s.
+        as a 2-D array of 1's and 0's.
         The default is None (no dilation).
     sort_by : (callable or str), optional
         A function or statistics to define the order of the labels.
         Valid string statistics are "area", "maximum", "minimum", "mean",
         "median", "sum", "standard_deviation", "variance".
         The default is "area".
     sort_decreasing : bool, optional
@@ -419,14 +427,16 @@
     # ---------------------------------.
     # TODO: this could be extended to work with dask >2D array
     # - dask_image.ndmeasure.label  https://image.dask.org/en/latest/dask_image.ndmeasure.html
     # - dask_image.ndmorph.binary_dilation https://image.dask.org/en/latest/dask_image.ndmorph.html#dask_image.ndmorph.binary_dilation
 
     # ---------------------------------.
     # Check array validity
+    if labeled_comprehension_kwargs is None:
+        labeled_comprehension_kwargs = {}
     arr = _check_array(arr)
 
     # Check input arguments
     _check_sort_by(sort_by)
 
     # ---------------------------------.
     # Define masks
@@ -461,15 +471,17 @@
 
     # Set NaN pixels to label value 0
     label_arr[mask_nan] = 0
 
     # ---------------------------------.
     # Filter label by area
     label_indices = _get_labels_with_requested_occurrence(
-        label_arr=label_arr, vmin=min_area_threshold, vmax=max_area_threshold
+        label_arr=label_arr,
+        vmin=min_area_threshold,
+        vmax=max_area_threshold,
     )
     if len(label_indices) == 0:
         return _no_labels_result(arr)
 
     # ---------------------------------.
     # Sort labels by statistics (i.e. label area, label max value ...)
     label_indices, values = _get_labels_stats(
@@ -499,15 +511,15 @@
     min_value_threshold=-np.inf,
     max_value_threshold=np.inf,
     min_area_threshold=1,
     max_area_threshold=np.inf,
     footprint=None,
     sort_by="area",
     sort_decreasing=True,
-    labeled_comprehension_kwargs={},
+    labeled_comprehension_kwargs=None,
 ):
     """
     Function deriving the labels array and associated labels info.
 
     Parameters
     ----------
     data_array : xr.DataArray
@@ -526,15 +538,15 @@
         The default is np.inf.
     footprint : (int, np.ndarray or None), optional
         This argument enables to dilate the mask derived after applying
         min_value_threshold and max_value_threshold.
         If footprint = 0 or None, no dilation occur.
         If footprint is a positive integer, it create a disk(footprint)
         If footprint is a 2D array, it must represent the neighborhood expressed
-        as a 2-D array of 1’s and 0’s.
+        as a 2-D array of 1's and 0's.
         The default is None (no dilation).
     sort_by : (callable or str), optional
         A function or statistics to define the order of the labels.
         Valid string statistics are "area", "maximum", "minimum", "mean",
         "median", "sum", "standard_deviation", "variance".
         The default is "area".
     sort_decreasing : bool, optional
@@ -561,14 +573,16 @@
         The DataArray name is defined as "labels_{sort_by}".
     n_labels, int
         Number of labels in the labels array.
     values, np.arrays
         Array of length n_labels with the stats values associated to each label.
     """
     # Extract data from DataArray
+    if labeled_comprehension_kwargs is None:
+        labeled_comprehension_kwargs = {}
     if not isinstance(data_array, xr.DataArray):
         raise TypeError("Expecting xr.DataArray.")
 
     # Get labels
     labels_arr, n_labels, values = _get_labels(
         arr=data_array.data,
         min_value_threshold=min_value_threshold,
@@ -595,15 +609,15 @@
     min_value_threshold=-np.inf,
     max_value_threshold=np.inf,
     min_area_threshold=1,
     max_area_threshold=np.inf,
     footprint=None,
     sort_by="area",
     sort_decreasing=True,
-    labeled_comprehension_kwargs={},
+    labeled_comprehension_kwargs=None,
     label_name="label",
 ):
     """
     Compute labels and and add as a coordinates to an xarray object.
 
     Parameters
     ----------
@@ -626,45 +640,37 @@
         The default is np.inf.
     footprint : (int, np.ndarray or None), optional
         This argument enables to dilate the mask derived after applying
         min_value_threshold and max_value_threshold.
         If footprint = 0 or None, no dilation occur.
         If footprint is a positive integer, it create a disk(footprint)
         If footprint is a 2D array, it must represent the neighborhood expressed
-        as a 2-D array of 1’s and 0’s.
+        as a 2-D array of 1's and 0's.
         The default is None (no dilation).
     sort_by : (callable or str), optional
         A function or statistics to define the order of the labels.
         Valid string statistics are "area", "maximum", "minimum", "mean",
         "median", "sum", "standard_deviation", "variance".
         The default is "area".
     sort_decreasing : bool, optional
         If True, sort labels by decreasing 'sort_by' value.
         The default is True.
     labeled_comprehension_kwargs : dict, optional
         Additional arguments to be passed to dask_image.ndmeasure.labeled_comprehension
-        if sort_by is a callable. May contain
-            out_dtype : dtype, optional
-                Dtype to use for result.
-                The default is float.
-            default : (int, float or None), optional
-                Default return value when a element of index does not exist in the label array.
-                The default is None.
-            pass_positions : bool, optional
-                If True, pass linear indices to 'sort_by' as a second argument.
-                The default is False.
-        The default is {}.
+        if `sort_by` is a callable.
 
     Returns
     -------
     xr_obj : (xr.DataArray or xr.Dataset)
         xarray object with the new label coordinate.
         In the label coordinate, non-labels values are set to np.nan.
     """
     # Check xarray input
+    if labeled_comprehension_kwargs is None:
+        labeled_comprehension_kwargs = {}
     _check_xr_obj(xr_obj=xr_obj, variable=variable)
 
     # Retrieve labels (if available)
     data_array_to_label = xr_obj[variable] if isinstance(xr_obj, xr.Dataset) else xr_obj
 
     da_labels, n_labels, values = _xr_get_labels(
         data_array=data_array_to_label,
@@ -674,25 +680,21 @@
         max_area_threshold=max_area_threshold,
         footprint=footprint,
         sort_by=sort_by,
         sort_decreasing=sort_decreasing,
         labeled_comprehension_kwargs=labeled_comprehension_kwargs,
     )
     if n_labels == 0:
-        raise ValueError(
-            "No patch available. You might want to change the patch generator parameters."
-        )
+        raise ValueError("No patch available. You might want to change the patch generator parameters.")
 
     # Set labels values == 0 to np.nan (useful for plotting)
     da_labels = da_labels.where(da_labels > 0)
 
     # Assign label to xr.DataArray  coordinate
-    xr_obj = xr_obj.assign_coords({label_name: da_labels})
-
-    return xr_obj
+    return xr_obj.assign_coords({label_name: da_labels})
 
 
 def highlight_label(xr_obj, label_name, label_id):
     """Set all labels values to 0 except for 'label_id'."""
     xr_obj = xr_obj.copy(deep=True)  # required otherwise overwrite original data
     label_arr = xr_obj[label_name].data
     label_arr[label_arr != label_id] = 0
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ximage-0.0.3/ximage/patch/checks.py` & `ximage-0.0.4/ximage/patch/checks.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,34 @@
-#!/usr/bin/env python3
-"""
-Created on Mon Jul 10 14:07:16 2023
+# -----------------------------------------------------------------------------.
+# MIT License
 
-@author: ghiggi
-"""
+# Copyright (c) 2024 ximage developers
+#
+# This file is part of ximage.
+
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
+# -----------------------------------------------------------------------------.
+"""Checks for patch extraction function arguments."""
 import numpy as np
 
 from ximage.utils.checks import are_all_integers, are_all_natural_numbers
 
 
 def _ensure_is_dict_argument(arg, dims, arg_name):
     """Ensure argument is a dictionary with same order as dims."""
@@ -17,32 +38,29 @@
         if len(arg) != len(dims):
             raise ValueError(f"{arg_name} must match the number of dimensions of the label array.")
         arg = dict(zip(dims, arg))
     if isinstance(arg, dict):
         dict_dims = np.array(list(arg))
         invalid_dims = dict_dims[np.isin(dict_dims, dims, invert=True)].tolist()
         if len(invalid_dims) > 0:
-            raise ValueError(
-                f"{arg_name} must not contain dimensions {invalid_dims}. It expects only {dims}."
-            )
+            raise ValueError(f"{arg_name} must not contain dimensions {invalid_dims}. It expects only {dims}.")
         missing_dims = np.array(dims)[np.isin(dims, dict_dims, invert=True)].tolist()
         if len(missing_dims) > 0:
             raise ValueError(f"{arg_name} must contain also dimensions {missing_dims}")
     else:
         type_str = type(arg)
         raise TypeError(f"Unrecognized type {type_str} for argument {arg_name}.")
-    # Reorder as function of dims
-    arg = {dim: arg[dim] for dim in dims}
-    return arg
+    # Reorder arguments as function of dims
+    return {dim: arg[dim] for dim in dims}
 
 
 def _replace_full_dimension_flag_value(arg, shape):
     """Replace -1 values with the corresponding dimension shape."""
-    arg = {dim: shape[i] if value == -1 else value for i, (dim, value) in enumerate(arg.items())}
-    return arg
+    # Return argument with positive integer values
+    return {dim: shape[i] if value == -1 else value for i, (dim, value) in enumerate(arg.items())}
 
 
 def check_patch_size(patch_size, dims, shape):
     """
     Check the validity of the patch_size argument based on the array shape.
 
     Parameters
@@ -63,22 +81,20 @@
     -------
     patch_size : dict
         The shape of the patch.
     """
     patch_size = _ensure_is_dict_argument(patch_size, dims=dims, arg_name="patch_size")
     patch_size = _replace_full_dimension_flag_value(patch_size, shape)
     # Check natural number
-    for dim, value in patch_size.items():
+    for value in patch_size.values():
         if not are_all_natural_numbers(value):
-            raise ValueError(
-                "Invalid 'patch_size' values. They must be only positive integer values."
-            )
+            raise ValueError("Invalid 'patch_size' values. They must be only positive integer values.")
     # Check patch size is smaller than array shape
     idx_valid = [value <= max_value for value, max_value in zip(patch_size.values(), shape)]
-    max_allowed_patch_size = {dim: value for dim, value in zip(dims, shape)}
+    max_allowed_patch_size = dict(zip(dims, shape))
     if not all(idx_valid):
         raise ValueError(f"The maximum allowed patch_size values are {max_allowed_patch_size}")
     return patch_size
 
 
 def check_kernel_size(kernel_size, dims, shape):
     """
@@ -102,22 +118,20 @@
     -------
     kernel_size : dict
         The shape of the kernel.
     """
     kernel_size = _ensure_is_dict_argument(kernel_size, dims=dims, arg_name="kernel_size")
     kernel_size = _replace_full_dimension_flag_value(kernel_size, shape)
     # Check natural number
-    for dim, value in kernel_size.items():
+    for value in kernel_size.values():
         if not are_all_natural_numbers(value):
-            raise ValueError(
-                "Invalid 'kernel_size' values. They must be only positive integer values."
-            )
+            raise ValueError("Invalid 'kernel_size' values. They must be only positive integer values.")
     # Check patch size is smaller than array shape
     idx_valid = [value <= max_value for value, max_value in zip(kernel_size.values(), shape)]
-    max_allowed_kernel_size = {dim: value for dim, value in zip(dims, shape)}
+    max_allowed_kernel_size = dict(zip(dims, shape))
     if not all(idx_valid):
         raise ValueError(f"The maximum allowed patch_size values are {max_allowed_kernel_size}")
     return kernel_size
 
 
 def check_buffer(buffer, dims, shape):
     """
@@ -137,15 +151,15 @@
 
     Returns
     -------
     buffer : dict
         The buffer to apply on each dimension.
     """
     buffer = _ensure_is_dict_argument(buffer, dims=dims, arg_name="buffer")
-    for dim, value in buffer.items():
+    for value in buffer.values():
         if not are_all_integers(value):
             raise ValueError("Invalid 'buffer' values. They must be only integer values.")
     return buffer
 
 
 def check_padding(padding, dims, shape):
     """
@@ -166,15 +180,15 @@
 
     Returns
     -------
     padding : dict
         The padding to apply on each dimension.
     """
     padding = _ensure_is_dict_argument(padding, dims=dims, arg_name="padding")
-    for dim, value in padding.items():
+    for value in padding.values():
         if not are_all_integers(value):
             raise ValueError("Invalid 'padding' values. They must be only integer values.")
     return padding
 
 
 def check_partitioning_method(partitioning_method):
     """Check partitioning method."""
@@ -211,23 +225,18 @@
     stride : dict
         The stride to apply on each dimension.
     """
     if partitioning_method is None:
         return None
     # Set default arguments
     if stride is None:
-        if partitioning_method == "tiling":
-            stride = 0
-        else:  # sliding
-            stride = 1
+        stride = 0 if partitioning_method == "tiling" else 1
     stride = _ensure_is_dict_argument(stride, dims=dims, arg_name="stride")
     if partitioning_method == "tiling":
-        for dim, value in stride.items():
+        for value in stride.values():
             if not are_all_integers(value):
                 raise ValueError("Invalid 'stride' values. They must be only integer values.")
     else:  # sliding
-        for dim, value in stride.items():
+        for value in stride.values():
             if not are_all_natural_numbers(value):
-                raise ValueError(
-                    "Invalid 'stride' values. They must be only positive integer (>=1) values."
-                )
+                raise ValueError("Invalid 'stride' values. They must be only positive integer (>=1) values.")
     return stride
```

### Comparing `ximage-0.0.3/ximage/patch/labels_patch.py` & `ximage-0.0.4/ximage/patch/labels_patch.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,34 @@
-#!/usr/bin/env python3
-"""
-Created on Wed Oct 19 19:40:12 2022
+# -----------------------------------------------------------------------------.
+# MIT License
+
+# Copyright (c) 2024 ximage developers
+#
+# This file is part of ximage.
+
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
 
-@author: ghiggi
-"""
+# -----------------------------------------------------------------------------.
+"""Functions to extract patch around labels."""
 import random
 import warnings
 from typing import Callable, Union
 
 import matplotlib.pyplot as plt
 import numpy as np
 import xarray as xr
@@ -85,16 +106,15 @@
         raise TypeError("labels_id must be None or a list or a np.array.")
     if isinstance(labels_id, int):
         labels_id = [labels_id]
     # Get list of valid labels
     valid_labels = np.unique(label_arr[~np.isnan(label_arr)]).astype(int)
     # If labels_id is None, assign the valid_labels
     if isinstance(labels_id, type(None)):
-        labels_id = valid_labels
-        return labels_id
+        return valid_labels
     # If input labels_id is a list, make it a np.array
     labels_id = np.array(labels_id).astype(int)
     # Check labels_id are natural number >= 1
     if np.any(labels_id == 0):
         raise ValueError("labels id must not contain the 0 value.")
     if not are_all_natural_numbers(labels_id):
         raise ValueError("labels id must be positive natural numbers.")
@@ -126,20 +146,18 @@
     Returns
     -------
     n_patches_per_partition: int
        The number of patches to extract from each partition.
     """
     if n_patches_per_partition < 1:
         raise ValueError("n_patches_per_partitions must be a positive integer.")
-    if isinstance(centered_on, str):
-        if centered_on not in ["random"]:
-            if n_patches_per_partition > 1:
-                raise ValueError(
-                    "Only the pre-implemented centered_on='random' method allow n_patches_per_partition values > 1."
-                )
+    if isinstance(centered_on, str) and centered_on not in ["random"] and n_patches_per_partition > 1:
+        raise ValueError(
+            "Only the pre-implemented centered_on='random' method allow n_patches_per_partition values > 1.",
+        )
     return n_patches_per_partition
 
 
 def _check_n_patches_per_label(n_patches_per_label, n_patches_per_partition):
     if n_patches_per_label < n_patches_per_partition:
         raise ValueError("n_patches_per_label must be equal or larger to n_patches_per_partition.")
     return n_patches_per_label
@@ -147,36 +165,33 @@
 
 def _check_callable_centered_on(centered_on):
     """Check validity of callable centered_on."""
     input_shape = (2, 3)
     arr = np.zeros(input_shape)
     point = centered_on(arr)
     if not isinstance(point, (tuple, type(None))):
-        raise ValueError(
-            "The 'centered_on' function should return a point coordinates tuple or None."
-        )
+        raise ValueError("The 'centered_on' function should return a point coordinates tuple or None.")
     if len(point) != len(input_shape):
         raise ValueError(
-            "The 'centered_on' function should return point coordinates having same dimensions has input array."
+            "The 'centered_on' function should return point coordinates having same dimensions has input array.",
         )
     for c, max_value in zip(point, input_shape):
         if c < 0:
             raise ValueError("The point coordinate must be a positive integer.")
         if c >= max_value:
             raise ValueError("The point coordinate must be inside the array shape.")
         if np.isnan(c):
             raise ValueError("The point coordinate must not be np.nan.")
+    # Check case with nan array
     try:
         point = centered_on(arr * np.nan)
-        if point is not None:
-            raise ValueError(
-                "The 'centered_on' function should return None if the input array is a np.nan ndarray."
-            )
-    except:
-        raise ValueError("The 'centered_on' function should be able to deal with a np.nan ndarray.")
+    except Exception as err:
+        raise ValueError(f"The 'centered_on' function should be able to deal with a np.nan ndarray. Error is {err}.")
+    if point is not None:
+        raise ValueError("The 'centered_on' function should return None if the input array is a np.nan ndarray.")
 
 
 def _check_centered_on(centered_on):
     """Check valid centered_on to identify a point in an array."""
     if not (callable(centered_on) or isinstance(centered_on, str)):
         raise TypeError("'centered_on' must be a string or a function.")
     if isinstance(centered_on, str):
@@ -195,83 +210,62 @@
         _check_callable_centered_on(centered_on)
     return centered_on
 
 
 def _get_variable_arr(xr_obj, variable, centered_on):
     """Get variable array (in memory)."""
     if isinstance(xr_obj, xr.DataArray):
-        variable_arr = np.asanyarray(xr_obj.data)
-        return variable_arr
-    else:
-        if centered_on is not None:
-            if variable is None and (centered_on in ["max", "min"] or callable(centered_on)):
-                raise ValueError("'variable' must be specified if 'centered_on' is specified.")
-        if variable is not None:
-            variable_arr = np.asanyarray(xr_obj[variable].data)  # in memory
-
-        else:
-            variable_arr = None
-    return variable_arr
+        return np.asanyarray(xr_obj.data)
+    if centered_on is not None and variable is None and (centered_on in ["max", "min"] or callable(centered_on)):
+        raise ValueError("'variable' must be specified if 'centered_on' is specified.")
+    return np.asanyarray(xr_obj[variable].data) if variable is not None else None
 
 
 def _check_variable_arr(variable_arr, label_arr):
     """Check variable array validity."""
-    if variable_arr is not None:
-        if variable_arr.shape != label_arr.shape:
-            raise ValueError(
-                "Arrays corresponding to 'variable' and 'label_name' must have same shape."
-            )
+    if variable_arr is not None and variable_arr.shape != label_arr.shape:
+        raise ValueError("Arrays corresponding to 'variable' and 'label_name' must have same shape.")
     return variable_arr
 
 
 def _get_point_centroid(arr):
     """Get the coordinate of label bounding box center.
 
     It assumes that the array has been cropped around the label.
     It returns None if all values are non-finite (i.e. np.nan).
     """
     if np.all(~np.isfinite(arr)):
         return None
     centroid = np.array(arr.shape) / 2.0
-    centroid = tuple(centroid.tolist())
-    return centroid
+    return tuple(centroid.tolist())
 
 
 def _get_point_random(arr):
     """Get random point with finite value."""
     is_finite = np.isfinite(arr)
     if np.all(~is_finite):
         return None
     points = np.argwhere(is_finite)
-    random_point = random.choice(points)
-    return random_point
+    return random.choice(points)
 
 
 def _get_point_with_max_value(arr):
     """Get point with maximum value."""
     with warnings.catch_warnings():
         warnings.simplefilter("ignore", category=RuntimeWarning)
         point = np.argwhere(arr == np.nanmax(arr))
-    if len(point) == 0:
-        point = None
-    else:
-        point = tuple(point[0].tolist())
-    return point
+    return None if len(point) == 0 else tuple(point[0].tolist())
 
 
 def _get_point_with_min_value(arr):
     """Get point with minimum value."""
     with warnings.catch_warnings():
         warnings.simplefilter("ignore", category=RuntimeWarning)
         point = np.argwhere(arr == np.nanmin(arr))
-    if len(point) == 0:
-        point = None
-    else:
-        point = tuple(point[0].tolist())
-    return point
+    return None if len(point) == 0 else tuple(point[0].tolist())
 
 
 def _get_point_center_of_mass(arr, integer_index=True):
     """Get the coordinate of the label center of mass.
 
     It uses all cells which have finite values.
     If 0 value should be a non-label area, mask before with np.nan.
@@ -279,16 +273,15 @@
     """
     indices = np.argwhere(np.isfinite(arr))
     if len(indices) == 0:
         return None
     center_of_mass = np.nanmean(indices, axis=0)
     if integer_index:
         center_of_mass = center_of_mass.round().astype(int)
-    center_of_mass = tuple(center_of_mass.tolist())
-    return center_of_mass
+    return tuple(center_of_mass.tolist())
 
 
 def find_point(arr, centered_on: Union[str, Callable] = "max"):
     """Find a specific point coordinate of the array.
 
     If the coordinate can't be find, return None.
     """
@@ -329,21 +322,17 @@
     -------
     list_slices : list
         List of slices to extract the region with non-zero elements in the input array.
     """
     # Return None if all values are zeros
     if not np.any(arr):
         return None
-
     ndims = arr.ndim
     coords = np.nonzero(arr)
-    list_slices = [
-        get_slice_from_idx_bounds(np.min(coords[i]), np.max(coords[i])) for i in range(ndims)
-    ]
-    return list_slices
+    return [get_slice_from_idx_bounds(np.min(coords[i]), np.max(coords[i])) for i in range(ndims)]
 
 
 def _get_patch_list_slices_around_label_point(
     label_arr,
     label_id,
     variable_arr,
     patch_size,
@@ -385,23 +374,25 @@
     # Get label bounding box slices
     list_slices = _get_labels_bbox_slices(label_arr == label_id)
     if list_slices is None:
         return None
     # Apply padding to the slices
     list_slices = pad_slices(list_slices, padding=padding, valid_shape=label_arr.shape)
     # Increase slices to match min_patch_size
-    list_slices = enlarge_slices(list_slices, min_size=min_patch_size, valid_shape=label_arr.shape)
-    return list_slices
+    return enlarge_slices(list_slices, min_size=min_patch_size, valid_shape=label_arr.shape)
 
 
 def _get_patch_list_slices(label_arr, label_id, variable_arr, patch_size, centered_on, padding):
     """Get patch n-dimensional list slices."""
     if not callable(centered_on) and centered_on == "label_bbox":
         list_slices = _get_patch_list_slices_around_label(
-            label_arr=label_arr, label_id=label_id, padding=padding, min_patch_size=patch_size
+            label_arr=label_arr,
+            label_id=label_id,
+            padding=padding,
+            min_patch_size=patch_size,
         )
     else:
         list_slices = _get_patch_list_slices_around_label_point(
             label_arr=label_arr,
             label_id=label_id,
             variable_arr=variable_arr,
             patch_size=patch_size,
@@ -409,22 +400,18 @@
         )
     return list_slices
 
 
 def _get_masked_arrays(label_arr, variable_arr, partition_list_slices):
     """Mask labels and variable arrays outside the partitions area."""
     masked_partition_label_arr = np.zeros(label_arr.shape) * np.nan
-    masked_partition_label_arr[tuple(partition_list_slices)] = label_arr[
-        tuple(partition_list_slices)
-    ]
+    masked_partition_label_arr[tuple(partition_list_slices)] = label_arr[tuple(partition_list_slices)]
     if variable_arr is not None:
         masked_partition_variable_arr = np.zeros(variable_arr.shape) * np.nan
-        masked_partition_variable_arr[tuple(partition_list_slices)] = variable_arr[
-            tuple(partition_list_slices)
-        ]
+        masked_partition_variable_arr[tuple(partition_list_slices)] = variable_arr[tuple(partition_list_slices)]
     else:
         masked_partition_variable_arr = None
     return masked_partition_label_arr, masked_partition_variable_arr
 
 
 def _get_patches_from_partitions_list_slices(
     partitions_list_slices,
@@ -457,26 +444,22 @@
                 variable_arr=masked_variable_arr,
                 label_id=label_id,
                 patch_size=patch_size,
                 centered_on=centered_on,
                 padding=padding,
             )
             if patch_list_slices is not None and patch_list_slices not in patches_list_slices:
-                n += 1
+                n += 1  # noqa PLW2901
                 patches_list_slices.append(patch_list_slices)
     return patches_list_slices
 
 
 def _get_list_isel_dicts(patches_list_slices, dims):
     """Return a list with isel dictionaries."""
-    list_isel_dicts = []
-    for patch_list_slices in patches_list_slices:
-        # list_isel_dicts.append(dict(zip(dims, patch_list_slices)))
-        list_isel_dicts.append({dim: slc for dim, slc in zip(dims, patch_list_slices)})
-    return list_isel_dicts
+    return [dict(zip(dims, patch_list_slices)) for patch_list_slices in patches_list_slices]
 
 
 def _extract_xr_patch(xr_obj, isel_dict, label_name, label_id, highlight_label_id):
     """Extract a xarray patch."""
     # Extract xarray patch around label
     xr_obj_patch = xr_obj.isel(isel_dict)
 
@@ -552,17 +535,15 @@
         if verbose:
             print(f"Label ID: {label_id} ({i}/{n_labels})")
 
         # Subset label_arr around the given label
         label_bbox_slices = _get_labels_bbox_slices(label_arr == label_id)
 
         # Apply padding to the label bounding box
-        label_bbox_slices = pad_slices(
-            label_bbox_slices, padding=padding.values(), valid_shape=label_arr.shape
-        )
+        label_bbox_slices = pad_slices(label_bbox_slices, padding=padding.values(), valid_shape=label_arr.shape)
 
         # --------------------------------------------------------------------.
         # Retrieve partitions list_slices
         if partitioning_method is not None:
             partitions_list_slices = get_nd_partitions_list_slices(
                 label_bbox_slices,
                 arr_shape=label_arr.shape,
@@ -653,14 +634,29 @@
     buffer=0,
     stride=None,
     include_last=True,
     ensure_slice_size=True,
     debug=False,
     verbose=False,
 ):
+    """
+    Returnisel-dictionaries to extract patches around labels.
+
+    The isel-dictionaries are grouped by label_id and returned in a
+    dictionary.
+
+    Please refer to ``get_patches_from_labels`` for a detailed description of
+    the function arguments.
+
+    Return
+    ------
+    dict
+        A dictionary of the form: ``{label_id: list_isel_dicts}``.
+
+    """
     gen = _get_patches_isel_dict_generator(
         xr_obj=xr_obj,
         label_name=label_name,
         patch_size=patch_size,
         variable=variable,
         n_patches=n_patches,
         n_labels=n_labels,
@@ -678,16 +674,15 @@
         buffer=buffer,
         stride=stride,
         include_last=include_last,
         ensure_slice_size=ensure_slice_size,
         debug=debug,
         verbose=verbose,
     )
-    dict_isel_dicts = {int(label_id): list_isel_dicts for label_id, list_isel_dicts in gen}
-    return dict_isel_dicts
+    return {int(label_id): list_isel_dicts for label_id, list_isel_dicts in gen}
 
 
 def get_patches_from_labels(
     xr_obj,
     label_name,
     patch_size,
     variable=None,
@@ -787,16 +782,16 @@
         If 'label_bbox' it extract the patches around the (padded) bounding box of the label.
         If 'label_bbox',the output patch sizes are only ensured to have a minimum patch_size,
         and will likely be of different size.
         Otherwise, the other methods guarantee that the output patches have a common shape.
 
         If centered_on is 'max', 'min' or a custom function, the 'variable' must be specified.
         If centered_on is a custom function, it must:
-            - return None if all array values are non-finite (i.e np.nan)
-            - return a tuple with same length as the array shape.
+        - return None if all array values are non-finite (i.e np.nan)
+        - return a tuple with same length as the array shape.
     padding : (int, tuple, dict), optional
         The padding to apply in each direction around a label prior to
         partitioning (tiling/sliding) or direct patch extraction.
         The default, 0, applies 0 padding in every dimension.
         Negative padding values are allowed !
         If int, the value is applied to all label array dimensions.
         If list or tuple, the length must match the number of dimensions of the array.
```

### Comparing `ximage-0.0.3/ximage/patch/slices.py` & `ximage-0.0.4/ximage/patch/slices.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,46 @@
-#!/usr/bin/env python3
-"""
-Created on Sat Dec 10 18:46:00 2022
+# -----------------------------------------------------------------------------.
+# MIT License
 
-@author: ghiggi
-"""
+# Copyright (c) 2024 ximage developers
+#
+# This file is part of ximage.
+
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
+# -----------------------------------------------------------------------------.
+"""Slices utility functions."""
 import numpy as np
 
 
 def get_slice_size(slc):
     """Get size of the slice.
 
     Note: The actual slice size must not be representative of the true slice if
     slice.stop is larger than the length of object to be sliced.
     """
     if not isinstance(slc, slice):
         raise TypeError("Expecting slice object")
-    size = slc.stop - slc.start
-    return size
+    return slc.stop - slc.start
 
 
 def pad_slice(slc, padding, min_start=0, max_stop=np.inf):
     """
     Increase/decrease the slice with the padding argument.
 
     Does not ensure that all output slices have same size.
@@ -33,22 +53,21 @@
         Padding to be applied to the slice.
     min_start : int, optional
        The minimum value for the start of the new slice.
        The default is 0.
     max_stop : int
         The maximum value for the stop of the new slice.
         The default is np.inf.
+
     Returns
     -------
     list_slices : TYPE
         The list of slices after applying padding.
     """
-
-    new_slice = slice(max(slc.start - padding, min_start), min(slc.stop + padding, max_stop))
-    return new_slice
+    return slice(max(slc.start - padding, min_start), min(slc.stop + padding, max_stop))
 
 
 def pad_slices(list_slices, padding, valid_shape):
     """
     Increase/decrease the list of slices with the padding argument.
 
     Parameters
@@ -67,27 +86,24 @@
     """
     # Check the inputs
     if isinstance(padding, int):
         padding = [padding] * len(list_slices)
     if isinstance(valid_shape, int):
         valid_shape = [valid_shape] * len(list_slices)
     if isinstance(padding, (list, tuple)) and len(padding) != len(list_slices):
-        raise ValueError(
-            "Invalid padding. The length of padding should be the same as the length of list_slices."
-        )
+        raise ValueError("Invalid padding. The length of padding should be the same as the length of list_slices.")
     if isinstance(valid_shape, (list, tuple)) and len(valid_shape) != len(list_slices):
         raise ValueError(
-            "Invalid valid_shape. The length of valid_shape should be the same as the length of list_slices."
+            "Invalid valid_shape. The length of valid_shape should be the same as the length of list_slices.",
         )
     # Apply padding
-    list_slices = [
+    return [
         pad_slice(s, padding=p, min_start=0, max_stop=valid_shape[i])
         for i, (s, p) in enumerate(zip(list_slices, padding))
     ]
-    return list_slices
 
 
 # min_size = 10
 # min_start = 0
 # max_stop = 20
 # slc = slice(1, 5)   # left bound
 # slc = slice(15, 20) # right bound
@@ -109,29 +125,28 @@
         The desired minimum size of the new slice.
     min_start : int, optional
        The minimum value for the start of the new slice.
        The default is 0.
     max_stop : int
         The maximum value for the stop of the new slice.
         The default is np.inf.
+
     Returns
     -------
     slice
         The new slice object with a size of at least min_size and respecting the left and right bounds.
         If the original slice object is already larger than min_size, the original slice is returned.
 
     """
     # Get slice size
     slice_size = get_slice_size(slc)
 
     # If min_size is larger than allowable size, raise error
     if min_size > (max_stop - min_start):
-        raise ValueError(
-            f"'min_size' {min_size} is too large to generate a slice between {min_start} and {max_stop}."
-        )
+        raise ValueError(f"'min_size' {min_size} is too large to generate a slice between {min_start} and {max_stop}.")
 
     # If slice size larger than min_size, return the slice
     if slice_size >= min_size:
         return slc
 
     # Calculate the number of points to add on both sides
     n_indices_to_add = min_size - slice_size
@@ -188,27 +203,36 @@
     """
     # Check the inputs
     if isinstance(min_size, int):
         min_size = [min_size] * len(list_slices)
     if isinstance(valid_shape, int):
         valid_shape = [valid_shape] * len(list_slices)
     if isinstance(min_size, (list, tuple)) and len(min_size) != len(list_slices):
-        raise ValueError(
-            "Invalid min_size. The length of min_size should be the same as the length of list_slices."
-        )
+        raise ValueError("Invalid min_size. The length of min_size should be the same as the length of list_slices.")
     if isinstance(valid_shape, (list, tuple)) and len(valid_shape) != len(list_slices):
         raise ValueError(
-            "Invalid valid_shape. The length of valid_shape should be the same as the length of list_slices."
+            "Invalid valid_shape. The length of valid_shape should be the same as the length of list_slices.",
         )
     # Enlarge the slice
-    list_slices = [
+    return [
         enlarge_slice(slc, min_size=s, min_start=0, max_stop=valid_shape[i])
         for i, (slc, s) in enumerate(zip(list_slices, min_size))
     ]
-    return list_slices
+
+
+def get_idx_bounds_from_slice(slc):
+    """Get start and end indices of the slice.
+
+    Note: For index based selection, use idx_start:idx_end+1 !
+    """
+    if not isinstance(slc, slice):
+        raise TypeError("Expecting slice object")
+    idx_start = slc.start
+    idx_end = slc.stop - 1
+    return idx_start, idx_end
 
 
 def get_slice_from_idx_bounds(idx_start, idx_end):
     """Return the slice required to include the idx bounds."""
     return slice(idx_start, idx_end + 1)
 
 
@@ -233,30 +257,26 @@
 
     Returns
     -------
     slice
         A slice object with the desired size and respecting the left and right bounds.
 
     """
-
     index_slc = slice(index, index + 1)
     try:
         slc = enlarge_slice(index_slc, min_size=size, min_start=min_start, max_stop=max_stop)
     except ValueError:
         print(index, size, min_start, max_stop, index_slc)
-        raise ValueError("'size' {size} is to large to be between {min_start} and {max_stop}.")
+        raise ValueError(f"'size' {size} is to large to be between {min_start} and {max_stop}.")
     return slc
 
 
 def _check_buffer(buffer, slice_size):
-    if buffer < 0:
-        if abs(buffer) * 2 >= slice_size:
-            raise ValueError(
-                "The negative buffer absolute value is larger than half of the slice_size."
-            )
+    if buffer < 0 and abs(buffer) * 2 >= slice_size:
+        raise ValueError("The negative buffer absolute value is larger than half of the slice_size.")
     return buffer
 
 
 def _check_slice_size(slice_size):
     if slice_size <= 0:
         raise ValueError("slice_size must be a positive non-zero integer.")
     return slice_size
@@ -289,29 +309,24 @@
 
 def _check_stride(stride, method):
     if method == "sliding":
         if stride is None:
             stride = 1
         if stride < 1:
             raise ValueError("When sliding, 'stride' must be equal or larger than 1.")
-    else:  # tiling
-        if stride is None:
-            stride = 0
+    elif stride is None:  # tiling
+        stride = 0
     if not isinstance(stride, int):
         raise TypeError("'stride' must be an integer.")
     return stride
 
 
 def _get_partitioning_idxs(start, stop, stride, slice_size, method):
-    if method == "tiling":
-        steps = slice_size + stride
-    else:  # sliding
-        steps = stride
-    idxs = np.arange(start, stop + 1, steps)
-    return idxs
+    steps = slice_size + stride if method == "tiling" else stride  # when sliding
+    return np.arange(start, stop + 1, steps)
 
 
 def get_partitions_slices(
     start,
     stop,
     slice_size,
     method,
@@ -380,38 +395,37 @@
     stride = _check_stride(stride, method)
     buffer = _check_buffer(buffer, slice_size)
     min_start = _check_min_start(min_start, start)
     max_stop = _check_max_stop(max_stop, stop)
 
     # Define slices
     slice_step = 1  # TODO: modify for dilation together with slice_size
-    idxs = _get_partitioning_idxs(
-        start=start, stop=stop, stride=stride, slice_size=slice_size, method=method
-    )
+    idxs = _get_partitioning_idxs(start=start, stop=stop, stride=stride, slice_size=slice_size, method=method)
     slices = [slice(idxs[i], idxs[i] + slice_size, slice_step) for i in range(len(idxs) - 1)]
 
     # Define last slice
     if include_last and idxs[-1] != stop:
         last_slice = slice(idxs[-1], stop)
         if ensure_slice_size:
-            last_slice = enlarge_slice(
-                last_slice, min_size=slice_size, min_start=min_start, max_stop=max_stop
-            )
+            last_slice = enlarge_slice(last_slice, min_size=slice_size, min_start=min_start, max_stop=max_stop)
         slices.append(last_slice)
 
     # Buffer the slices
-    slices = [
-        pad_slice(slc, padding=buffer, min_start=min_start, max_stop=max_stop) for slc in slices
-    ]
-
-    return slices
+    return [pad_slice(slc, padding=buffer, min_start=min_start, max_stop=max_stop) for slc in slices]
 
 
 def get_nd_partitions_list_slices(
-    list_slices, arr_shape, method, kernel_size, stride, buffer, include_last, ensure_slice_size
+    list_slices,
+    arr_shape,
+    method,
+    kernel_size,
+    stride,
+    buffer,
+    include_last,
+    ensure_slice_size,
 ):
     """Return the n-dimensional partitions list of slices of a initial list of slices."""
     import itertools
 
     l_iterables = []
     for i in range(len(list_slices)):
         slice_size = kernel_size[i]
@@ -429,9 +443,8 @@
             include_last=include_last,
             ensure_slice_size=ensure_slice_size,
             min_start=0,
             max_stop=max_stop,
         )
         l_iterables.append(slices)
 
-    tiles_list_slices = list(itertools.product(*l_iterables))
-    return tiles_list_slices
+    return list(itertools.product(*l_iterables))
```

### Comparing `ximage-0.0.3/ximage.egg-info/PKG-INFO` & `ximage-0.0.4/ximage.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ximage
-Version: 0.0.3
+Version: 0.0.4
 Summary: xarray-based tools for image/video processing
 Author-email: Gionata Ghiggi <gionata.ghiggi@epfl.ch>
 License: MIT License
         
         Copyright (c) 2023 Gionata Ghiggi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -26,29 +26,28 @@
         SOFTWARE.
         
 Project-URL: homepage, https://github.com/ghiggi/ximage
 Project-URL: repository, https://github.com/ghiggi/ximage
 Project-URL: source, https://github.com/ghiggi/ximage
 Project-URL: tracker, https://github.com/ghiggi/ximage/issues
 Project-URL: documentation, https://ximage.readthedocs.io
-Project-URL: changelog, https://github.com/ghiggi/ximage/CHANGELOG.md
+Project-URL: changelog, https://github.com/ghiggi/ximage/blob/main/CHANGELOG.md
 Keywords: image,video,labelling,patch,extraction
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Requires-Python: >=3.8
@@ -57,14 +56,15 @@
 Requires-Dist: xarray
 Requires-Dist: dask
 Requires-Dist: dask-image
 Requires-Dist: matplotlib
 Requires-Dist: scikit-image
 Provides-Extra: dev
 Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: loghub; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: black[jupyter]; extra == "dev"
 Requires-Dist: blackdoc; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: codespell; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
@@ -88,41 +88,39 @@
 | Activity             | [![PyPI Downloads](https://img.shields.io/pypi/dm/ximage.svg?label=PyPI%20downloads&style=flat)](https://pypi.org/project/ximage/) [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/ximage.svg?label=Conda%20downloads&style=flat)](https://anaconda.org/conda-forge/ximage) |
 | Python Versions      | [![Python Versions](https://img.shields.io/badge/Python-3.8%20%203.9%20%203.10%20%203.11%20%203.12-blue?style=flat)](https://www.python.org/downloads/) |
 | Supported Systems    | [![Linux](https://img.shields.io/github/actions/workflow/status/ghiggi/ximage/.github/workflows/tests.yml?label=Linux&style=flat)](https://github.com/ghiggi/ximage/actions/workflows/tests.yml) [![macOS](https://img.shields.io/github/actions/workflow/status/ghiggi/ximage/.github/workflows/tests.yml?label=macOS&style=flat)](https://github.com/ghiggi/ximage/actions/workflows/tests.yml) [![Windows](https://img.shields.io/github/actions/workflow/status/ghiggi/ximage/.github/workflows/tests_windows.yml?label=Windows&style=flat)](https://github.com/ghiggi/ximage/actions/workflows/tests_windows.yml) |
 | Project Status       | [![Project Status](https://www.repostatus.org/badges/latest/active.svg?style=flat)](https://www.repostatus.org/#active) |
 | Build Status         | [![Tests](https://github.com/ghiggi/ximage/actions/workflows/tests.yml/badge.svg?style=flat)](https://github.com/ghiggi/ximage/actions/workflows/tests.yml) [![Lint](https://github.com/ghiggi/ximage/actions/workflows/lint.yml/badge.svg?style=flat)](https://github.com/ghiggi/ximage/actions/workflows/lint.yml) [![Docs](https://readthedocs.org/projects/ximage/badge/?version=latest&style=flat)](https://ximage.readthedocs.io/en/latest/) |
 | Linting              | [![Black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat)](https://github.com/psf/black) [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json&style=flat)](https://github.com/astral-sh/ruff) [![Codespell](https://img.shields.io/badge/Codespell-enabled-brightgreen?style=flat)](https://github.com/codespell-project/codespell) |
 | Code Coverage        | [![Coveralls](https://coveralls.io/repos/github/ghiggi/ximage/badge.svg?branch=main&style=flat)](https://coveralls.io/github/ghiggi/ximage?branch=main) [![Codecov](https://codecov.io/gh/ghiggi/ximage/branch/main/graph/badge.svg?style=flat)](https://codecov.io/gh/ghiggi/ximage) |
-| Code Quality         | [![Codefactor](https://www.codefactor.io/repository/github/ghiggi/ximage/badge?style=flat)](https://www.codefactor.io/repository/github/ghiggi/ximage) [![Codebeat](https://codebeat.co/badges/14ff831b-f064-4bdd-a2e2-72ffdf28a35a?style=flat)](https://codebeat.co/projects/github-com-ltelab-ximage-main) [![Codacy](https://app.codacy.com/project/badge/Grade/d823c50a7ad14268bd347b5aba384623?style=flat)](https://app.codacy.com/gh/ghiggi/ximage/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade) [![Codescene](https://codescene.io/projects/36773/status-badges/code-health?style=flat)](https://codescene.io/projects/36773) |
-| Code Review          | [![pyOpenSci](https://tinyurl.com/XXXX)](#) |
+| Code Quality         | [![Codefactor](https://www.codefactor.io/repository/github/ghiggi/ximage/badge?style=flat)](https://www.codefactor.io/repository/github/ghiggi/ximage) [![Codebeat](https://codebeat.co/badges/3eab0b92-5b00-4eb7-9834-2e5f9a083b5e?style=flat)](https://codebeat.co/projects/github-com-ghiggi-ximage-main) [![Codacy](https://app.codacy.com/project/badge/Grade/d823c50a7ad14268bd347b5aba384623?style=flat)](https://app.codacy.com/gh/ghiggi/ximage/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade) [![CodeScene](https://codescene.io/projects/41869/status-badges/code-health?style=flat)](https://codescene.io/projects/41869) |
 | License              | [![License](https://img.shields.io/github/license/ghiggi/ximage?style=flat)](https://github.com/ghiggi/ximage/blob/main/LICENSE) |
 | Community            | [![Slack](https://img.shields.io/badge/Slack-ximage-green.svg?logo=slack&style=flat)](https://join.slack.com/t/xarray-tools/shared_invite/zt-28f5r0n75-ygNZN5omemhz72NM~WKUHA) [![GitHub Discussions](https://img.shields.io/badge/GitHub-Discussions-green?logo=github&style=flat)](https://github.com/ghiggi/ximage/discussions) |
 | Citation             | [![DOI](https://zenodo.org/badge/664629093.svg?style=flat)](https://zenodo.org/records/8131553) |
 
  [**Slack**](https://join.slack.com/t/xarray-tools/shared_invite/zt-28f5r0n75-ygNZN5omemhz72NM~WKUHA) | [**Docs**](https://x-image.readthedocs.io/en/latest/)
 
-The `ximage` package is in active development. Feel free to try it out, to report issues or to suggest changes.
 
 ## ℹ️ Software Overview
 
 The software currently enables to:
 
 - label n-dimensional xarray objects
 - extract patches around n-dimensional labels
 - extract patches from n-dimensional xarray objects
 
-Join the [**DISDRODB Slack Workspace**](https://join.slack.com/t/xarray-tools/shared_invite/zt-28f5r0n75-ygNZN5omemhz72NM~WKUHA) to meet the community !
+Join the [**Slack Workspace**](https://join.slack.com/t/xarray-tools/shared_invite/zt-28f5r0n75-ygNZN5omemhz72NM~WKUHA) to meet the community !
 
 ## 🚀 Quick Start
 
 `ximage` provides an easy-to-use interface to manipulate image, videos and n-dimensional arrays with classical image processing techniques.
 
-The `ximage` xarray accessor provides a convenient way to labelling and extract patches in n-dimensional arrays ! 
+The `ximage` xarray accessor provides a convenient way to labelling and extract patches in n-dimensional arrays !
 
-##### Image labelling 
+##### Image labelling
 
 ```python
 min_value_threshold = 1
 max_value_threshold = np.inf
 min_area_threshold = 5
 max_area_threshold = np.inf
 footprint = None
@@ -192,48 +190,55 @@
     ensure_slice_size=ensure_slice_size,
     debug=debug,
     verbose=verbose,
 )
 
 ```
 
-Look at the [Tutorials][tutorial_link] to have an overview of the software !
- 
+#### 📖 Explore the ximage documentation
+
+To discover all `ximage` utilities, please read the [software documentation](https://x-image.readthedocs.io/en/latest/).
+
 ## 🛠️ Installation
 
-### pip
+### conda
 
-`ximage` can be installed via [pip][pip_link] on Linux, Mac, and Windows.
-On Windows you can install [WinPython][winpy_link] to get Python and pip
-running.
-Then, install the `ximage` package by typing the following command in the command terminal:
+ximage can be installed via [conda][conda_link] on Linux, Mac, and Windows.
+Install the package by typing the following command in the terminal:
 
 ```bash
-    pip install ximage
+conda install ximage
 ```
 
-To install the latest development version via pip, see the
-[documentation][doc_install_link].
+In case conda-forge is not set up for your system yet, see the easy to follow instructions on [conda-forge][conda_forge_link].
 
-### conda [NOT YET AVAILABLE]
+[conda_link]: https://docs.conda.io/en/latest/miniconda.html
+[conda_forge_link]: https://github.com/conda-forge/ximage-feedstock#installing-ximage
+
+### pip
 
-`ximage` can be installed via [conda][conda_link] on Linux, Mac, and Windows.
-Install the package by typing the following command in a command terminal:
+`ximage` can be installed also via [pip][pip_link] on Linux, Mac, and Windows.
+On Windows you can install [WinPython][winpy_link] to get Python and pip running.
+
+Install the `ximage` package by typing the following command in the terminal:
 
 ```bash
-    conda install ximage
+pip install ximage
 ```
 
-In case conda-forge is not set up for your system yet, see the easy to follow
-instructions on [conda-forge][conda_forge_link].
+To install the latest development version via pip, see the [documentation][dev_install_link].
+
+[pip_link]: https://pypi.org/project/gpm-api
+[winpy_link]: https://winpython.github.io/
+[dev_install_link]: https://gpm-api.readthedocs.io/en/latest/02_installation.html#installation-for-contributors
 
 ## 💭 Feedback and Contributing Guidelines
 
 If you aim to contribute or discuss the future development of ximage,
-we highly suggest to join the [**DISDRODB Slack Workspace**](https://join.slack.com/t/xarray-tools/shared_invite/zt-28f5r0n75-ygNZN5omemhz72NM~WKUHA)
+we highly suggest to join the [**Slack Workspace**](https://join.slack.com/t/xarray-tools/shared_invite/zt-28f5r0n75-ygNZN5omemhz72NM~WKUHA)
 
 Feel free to also open a [GitHub Issue](https://github.com/ghiggi/ximage/issues) or a
 [GitHub Discussion](https://github.com/ghiggi/ximage/discussions) specific to your questions or ideas.
 
 ## ✍️  Contributors
 
 * [Gionata Ghiggi](https://people.epfl.ch/gionata.ghiggi)
@@ -241,31 +246,19 @@
 
 ## Citation
 
 You can cite the `ximage` software by:
 
 > Ghiggi Gionata & Son Pham-Ba . ghiggi/ximage. Zenodo. https://doi.org/10.5281/zenodo.8131552
 
-If you want to cite a specific version, have a look at the [Zenodo site](https://doi.org/10.5281/zenodo.7753488).
+If you want to cite a specific version, have a look at the [Zenodo site](https://doi.org/10.5281/zenodo.8131552).
+
+## License
+
+The content of this repository is released under the terms of the [MIT](LICENSE) license.
 
 ## 📚 Requirements:
 
 - [xarray](https://docs.xarray.dev/en/stable/)
 - [dask](https://www.dask.org/)
 - [dask_image](https://image.dask.org/en/latest/)
 - [skimage](https://scikit-image.org/)
-
-## License
-
-The content of this repository is released under the terms of the [MIT](LICENSE) license.
-
-
-
-[pip_link]: https://pypi.org/project/ximage
-[conda_link]: https://docs.conda.io/en/latest/miniconda.html
-[conda_forge_link]: https://github.com/conda-forge/ximage-feedstock#installing-ximage
-[conda_pip]: https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-pkgs.html#installing-non-conda-packages
-[pipiflag]: https://pip-python3.readthedocs.io/en/latest/reference/pip_install.html?highlight=i#cmdoption-i
-[winpy_link]: https://winpython.github.io/
-
-[doc_link]: https://x-image.readthedocs.io
-[tutorial_link]: https://github.com/ghiggi/ximage/tree/main#tutorials-and-examples
```

