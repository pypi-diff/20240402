# Comparing `tmp/nessai_models-0.4.0.tar.gz` & `tmp/nessai-models-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nessai_models-0.4.0.tar", last modified: Thu Jun 29 11:14:38 2023, max compression
+gzip compressed data, was "nessai-models-0.5.0.tar", last modified: Tue Apr  2 11:21:58 2024, max compression
```

## Comparing `nessai_models-0.4.0.tar` & `nessai-models-0.5.0.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:14:38.989502 nessai_models-0.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:14:38.977502 nessai_models-0.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:14:38.981502 nessai_models-0.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-29 11:14:23.000000 nessai_models-0.4.0/.github/workflows/integration-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-29 11:14:23.000000 nessai_models-0.4.0/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-29 11:14:23.000000 nessai_models-0.4.0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-29 11:14:23.000000 nessai_models-0.4.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-06-29 11:14:23.000000 nessai_models-0.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-29 11:14:23.000000 nessai_models-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-29 11:14:23.000000 nessai_models-0.4.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-06-29 11:14:38.989502 nessai_models-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-06-29 11:14:23.000000 nessai_models-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:14:38.981502 nessai_models-0.4.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-29 11:14:23.000000 nessai_models-0.4.0/examples/basic_example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:14:38.985502 nessai_models-0.4.0/nessai_models/
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-29 11:14:23.000000 nessai_models-0.4.0/nessai_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-06-29 11:14:23.000000 nessai_models-0.4.0/nessai_models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-06-29 11:14:23.000000 nessai_models-0.4.0/nessai_models/brewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-06-29 11:14:23.000000 nessai_models-0.4.0/nessai_models/eggbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-06-29 11:14:23.000000 nessai_models-0.4.0/nessai_models/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-06-29 11:14:23.000000 nessai_models-0.4.0/nessai_models/gaussianmixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-29 11:14:23.000000 nessai_models-0.4.0/nessai_models/halfgaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-06-29 11:14:23.000000 nessai_models-0.4.0/nessai_models/mixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-29 11:14:23.000000 nessai_models-0.4.0/nessai_models/pyramid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-06-29 11:14:23.000000 nessai_models-0.4.0/nessai_models/rosenbrock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-06-29 11:14:23.000000 nessai_models-0.4.0/nessai_models/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:14:38.985502 nessai_models-0.4.0/nessai_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-06-29 11:14:38.000000 nessai_models-0.4.0/nessai_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-29 11:14:38.000000 nessai_models-0.4.0/nessai_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 11:14:38.000000 nessai_models-0.4.0/nessai_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-29 11:14:38.000000 nessai_models-0.4.0/nessai_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-29 11:14:38.000000 nessai_models-0.4.0/nessai_models.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-29 11:14:23.000000 nessai_models-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-29 11:14:38.989502 nessai_models-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-29 11:14:23.000000 nessai_models-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:14:38.989502 nessai_models-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-29 11:14:23.000000 nessai_models-0.4.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-06-29 11:14:23.000000 nessai_models-0.4.0/tests/test_base_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-06-29 11:14:23.000000 nessai_models-0.4.0/tests/test_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-29 11:14:23.000000 nessai_models-0.4.0/tests/test_gaussianmixture.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-29 11:14:23.000000 nessai_models-0.4.0/tests/test_mixture.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-29 11:14:23.000000 nessai_models-0.4.0/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-29 11:14:23.000000 nessai_models-0.4.0/tests/test_nessai_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-06-29 11:14:23.000000 nessai_models-0.4.0/tests/test_pyramid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-06-29 11:14:23.000000 nessai_models-0.4.0/tests/test_rosenbrock.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-29 11:14:23.000000 nessai_models-0.4.0/tests/test_signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:21:58.641554 nessai-models-0.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:21:58.633554 nessai-models-0.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:21:58.637554 nessai-models-0.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-02 11:21:54.000000 nessai-models-0.5.0/.github/workflows/integration-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-02 11:21:54.000000 nessai-models-0.5.0/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-02 11:21:54.000000 nessai-models-0.5.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-02 11:21:54.000000 nessai-models-0.5.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-02 11:21:54.000000 nessai-models-0.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-02 11:21:54.000000 nessai-models-0.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-04-02 11:21:54.000000 nessai-models-0.5.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-04-02 11:21:58.641554 nessai-models-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-04-02 11:21:54.000000 nessai-models-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:21:58.637554 nessai-models-0.5.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-02 11:21:54.000000 nessai-models-0.5.0/examples/basic_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-02 11:21:54.000000 nessai-models-0.5.0/examples/slabspike.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:21:58.641554 nessai-models-0.5.0/nessai_models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-02 11:21:54.000000 nessai-models-0.5.0/nessai_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-04-02 11:21:54.000000 nessai-models-0.5.0/nessai_models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-04-02 11:21:54.000000 nessai-models-0.5.0/nessai_models/brewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-02 11:21:54.000000 nessai-models-0.5.0/nessai_models/eggbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-04-02 11:21:54.000000 nessai-models-0.5.0/nessai_models/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-04-02 11:21:54.000000 nessai-models-0.5.0/nessai_models/gaussianmixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-02 11:21:54.000000 nessai-models-0.5.0/nessai_models/halfgaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-04-02 11:21:54.000000 nessai-models-0.5.0/nessai_models/mixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-02 11:21:54.000000 nessai-models-0.5.0/nessai_models/pyramid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-02 11:21:54.000000 nessai-models-0.5.0/nessai_models/rosenbrock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-04-02 11:21:54.000000 nessai-models-0.5.0/nessai_models/signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-02 11:21:54.000000 nessai-models-0.5.0/nessai_models/slabspike.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:21:58.641554 nessai-models-0.5.0/nessai_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-04-02 11:21:58.000000 nessai-models-0.5.0/nessai_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-02 11:21:58.000000 nessai-models-0.5.0/nessai_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 11:21:58.000000 nessai-models-0.5.0/nessai_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-02 11:21:58.000000 nessai-models-0.5.0/nessai_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-02 11:21:58.000000 nessai-models-0.5.0/nessai_models.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-02 11:21:54.000000 nessai-models-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 11:21:58.641554 nessai-models-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:21:58.641554 nessai-models-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-02 11:21:54.000000 nessai-models-0.5.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-04-02 11:21:54.000000 nessai-models-0.5.0/tests/test_base_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-04-02 11:21:54.000000 nessai-models-0.5.0/tests/test_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-02 11:21:54.000000 nessai-models-0.5.0/tests/test_gaussianmixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-02 11:21:54.000000 nessai-models-0.5.0/tests/test_mixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-02 11:21:54.000000 nessai-models-0.5.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-02 11:21:54.000000 nessai-models-0.5.0/tests/test_nessai_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-02 11:21:54.000000 nessai-models-0.5.0/tests/test_pyramid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-04-02 11:21:54.000000 nessai-models-0.5.0/tests/test_rosenbrock.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-02 11:21:54.000000 nessai-models-0.5.0/tests/test_signals.py
```

### Comparing `nessai_models-0.4.0/.github/workflows/integration-tests.yml` & `nessai-models-0.5.0/.github/workflows/integration-tests.yml`

 * *Files 18% similar despite different names*

```diff
@@ -14,21 +14,21 @@
   integration-tests:
     name: Python ${{ matrix.python-version }} (${{ matrix.os }})
 
     strategy:
       fail-fast: false
       matrix:
         os: [macOS, Ubuntu, Windows]
-        python-version: ["3.7", "3.8", "3.9", "3.10"]
+        python-version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
     runs-on: ${{ matrix.os }}-latest
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v4
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install -e .[dev]
     - name: Print environment variables
```

### Comparing `nessai_models-0.4.0/.github/workflows/lint.yml` & `nessai-models-0.5.0/.github/workflows/tests.yml`

 * *Files 23% similar despite different names*

```diff
@@ -1,37 +1,36 @@
-name: Lint
+name: Unit tests
 
 on:
   push:
     branches: [ main ]
   pull_request:
     branches: [ main ]
 
 concurrency:
   group: ${{ github.workflow }}-${{ github.ref }}
   cancel-in-progress: true
 
 jobs:
-  black:
-    name: Black
-    runs-on: ubuntu-latest
-    steps:
-      - uses: actions/checkout@v2
-      - uses: psf/black@stable
-        with:
-          options: "--check --diff"
-  flake8:
-    name: Flake8
-    runs-on: ubuntu-latest
+  unittests:
+    name: Python ${{ matrix.python-version }} (${{ matrix.os }})
+
+    strategy:
+      fail-fast: false
+      matrix:
+        os: [macOS, Ubuntu, Windows]
+        python-version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
+    runs-on: ${{ matrix.os }}-latest
+
     steps:
-    - uses: actions/checkout@v2
-    - name: Set up Python
-      uses: actions/setup-python@v2
+    - uses: actions/checkout@v4
+    - name: Set up Python ${{ matrix.python-version }}
+      uses: actions/setup-python@v4
       with:
-        python-version: '3.x'
+        python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        python -m pip install flake8
-    - name: Lint with flake8
+        pip install -e .[dev]
+    - name: Test with pytest
       run: |
-        python -m flake8 .
+        python -m pytest --without-integration --without-slow-integration
```

### Comparing `nessai_models-0.4.0/.github/workflows/publish-to-pypi.yml` & `nessai-models-0.5.0/.github/workflows/publish-to-pypi.yml`

 * *Files 1% similar despite different names*

```diff
@@ -5,17 +5,17 @@
     types: [published]
 
 jobs:
   build-n-publish:
     name: Build and publish Python 🐍 distributions 📦 to PyPI
     runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v4
     - name: Set up Python
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: '3.x'
     - name: Install pypa/build
       run: >-
         python -m
         pip install
         build
```

### Comparing `nessai_models-0.4.0/.github/workflows/tests.yml` & `nessai-models-0.5.0/.github/workflows/lint.yml`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,38 @@
-name: Unit tests
+name: Lint
 
 on:
   push:
     branches: [ main ]
   pull_request:
     branches: [ main ]
 
 concurrency:
   group: ${{ github.workflow }}-${{ github.ref }}
   cancel-in-progress: true
 
 jobs:
-  unittests:
-    name: Python ${{ matrix.python-version }} (${{ matrix.os }})
-
-    strategy:
-      fail-fast: false
-      matrix:
-        os: [macOS, Ubuntu, Windows]
-        python-version: ["3.7", "3.8", "3.9", "3.10"]
-    runs-on: ${{ matrix.os }}-latest
-
+  black:
+    name: Black
+    runs-on: ubuntu-latest
+    steps:
+      - uses: actions/checkout@v4
+      - uses: psf/black@stable
+        with:
+          options: "--check --diff"
+          version: "24.2"
+  flake8:
+    name: Flake8
+    runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@v2
-    - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v2
+    - uses: actions/checkout@v4
+    - name: Set up Python
+      uses: actions/setup-python@v4
       with:
-        python-version: ${{ matrix.python-version }}
+        python-version: '3.x'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        pip install -e .[dev]
-    - name: Test with pytest
+        python -m pip install flake8 Flake8-pyproject
+    - name: Lint with flake8
       run: |
-        python -m pytest --without-integration --without-slow-integration
+        python -m flake8 .
```

### Comparing `nessai_models-0.4.0/.gitignore` & `nessai-models-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `nessai_models-0.4.0/CHANGELOG.md` & `nessai-models-0.5.0/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,25 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.5.0] - 2024-04-02
+
+### Added
+
+- Add the `SlabSpike` model class (https://github.com/mj-will/nessai-models/pull/33)
+
+### Changed
+
+- Drop support for Python 3.7 (https://github.com/mj-will/nessai-models/pull/34)
+- Explicit support Python 3.11 and 3.12 (https://github.com/mj-will/nessai-models/pull/34)
+
 ## [0.4.0] - 2023-06-29
 
 ### Added
 
 - Add a Mixture of 1-dimensional distributions likelihood ([#31](https://github.com/mj-will/nessai-models/pull/31))
 
 
@@ -36,12 +47,13 @@
 - Add n-dimensional HalfGaussian ([#8](https://github.com/mj-will/nessai-models/pull/8))
 - Add Gaussian Mixture Model based on a [`cpnest` example](https://github.com/johnveitch/cpnest/blob/master/examples/gaussianmixture.py) ([#5](https://github.com/mj-will/nessai-models/pull/5))
 - Add n-dimensional Egg Box based on the version from [Feroz et al. 2008](https://arxiv.org/abs/0809.3437) ([#11](https://github.com/mj-will/nessai-models/pull/11))
 - Add n-dimensional Pyramid-like model ([#15](https://github.com/mj-will/nessai-models/pull/15))
 - Add basic tests for all models
 - Add a basic example ([#21](https://github.com/mj-will/nessai-models/pull/21))
 
-[Unreleased]: https://github.com/mj-will/nessai-models/compare/v0.4.0...HEAD
+[Unreleased]: https://github.com/mj-will/nessai-models/compare/v0.5.0...HEAD
+[0.5.0]: https://github.com/mj-will/nessai-models/compare/v0.4.0...v0.5.0
 [0.4.0]: https://github.com/mj-will/nessai-models/compare/v0.3.0...v0.4.0
 [0.3.0]: https://github.com/mj-will/nessai-models/compare/v0.2.0...v0.3.0
 [0.2.0]: https://github.com/mj-will/nessai-models/compare/v0.1.0...v0.2.0
 [0.1.0]: https://github.com/mj-will/nessai-models/releases/tag/v0.1.0
```

### Comparing `nessai_models-0.4.0/PKG-INFO` & `nessai-models-0.5.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 Metadata-Version: 2.1
-Name: nessai_models
-Version: 0.4.0
+Name: nessai-models
+Version: 0.5.0
 Summary: Models for nessai
-Home-page: https://github.com/mj-will/nessai-models
-Author: Michael J. Williams
-Author-email: m.williams.4@research.gla.ac.uk
+Author-email: "Michael J. Williams" <michaeljw1@googlemail.com>
 License: MIT
-Keywords: nested sampling,normalising flows,machine learning,nessai
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
+Project-URL: Homepage, https://github.com/mj-will/nessai-models
+Keywords: nested sampling,normalizing flows,machine learning,nessai
+Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Requires-Dist: numpy>=1.9
+Requires-Dist: scipy>0.16
+Requires-Dist: nessai>=0.8.0
 Provides-Extra: dev
+Requires-Dist: black>=24.0; extra == "dev"
+Requires-Dist: flake8; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: pytest>=6.0; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: pytest-integration; extra == "dev"
 
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7105559.svg)](https://doi.org/10.5281/zenodo.7105559)
 [![PyPI](https://img.shields.io/pypi/v/nessai-models)](https://pypi.org/project/nessai-models/)
 [![Integration tests](https://github.com/mj-will/nessai-models/actions/workflows/integration-tests.yml/badge.svg)](https://github.com/mj-will/nessai-models/actions/workflows/integration-tests.yml)
 [![Unit tests](https://github.com/mj-will/nessai-models/actions/workflows/tests.yml/badge.svg)](https://github.com/mj-will/nessai-models/actions/workflows/tests.yml)
 
 # nessai-models
@@ -27,14 +33,15 @@
 
 ## Included models
 
 * n-dimensional unit Gaussian
 * n-dimensional HalfGaussian
 * n-dimensional Rosenbrock
 * n-dimensional mixture of Gaussians
+* n-dimensional slab plus spike model
 * Gaussian mixture using data to based on [this example](https://github.com/johnveitch/cpnest/blob/master/examples/gaussianmixture.py) from `cpnest`
 * n-dimensional Egg Box based on the version in [Feroz et al. 2008](https://arxiv.org/abs/0809.3437)
 * n-dimensional Pyramid-like model
 * n-dimensional Brewer likelihood (Skilling's "Staistical Model") from [Brewer et al.](https://arxiv.org/abs/0912.2380)
 * Linear signal plus Gaussian noise model (`LinearSignal`)
 * Sinusoidal signal plus Gaussian noise model (`SinusoidalSignal`)
 * Mixture of 1-dimensional distributions (`MixtureOfDistributions`)
```

### Comparing `nessai_models-0.4.0/README.md` & `nessai-models-0.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 ## Included models
 
 * n-dimensional unit Gaussian
 * n-dimensional HalfGaussian
 * n-dimensional Rosenbrock
 * n-dimensional mixture of Gaussians
+* n-dimensional slab plus spike model
 * Gaussian mixture using data to based on [this example](https://github.com/johnveitch/cpnest/blob/master/examples/gaussianmixture.py) from `cpnest`
 * n-dimensional Egg Box based on the version in [Feroz et al. 2008](https://arxiv.org/abs/0809.3437)
 * n-dimensional Pyramid-like model
 * n-dimensional Brewer likelihood (Skilling's "Staistical Model") from [Brewer et al.](https://arxiv.org/abs/0912.2380)
 * Linear signal plus Gaussian noise model (`LinearSignal`)
 * Sinusoidal signal plus Gaussian noise model (`SinusoidalSignal`)
 * Mixture of 1-dimensional distributions (`MixtureOfDistributions`)
```

### Comparing `nessai_models-0.4.0/examples/basic_example.py` & `nessai-models-0.5.0/examples/basic_example.py`

 * *Files identical despite different names*

### Comparing `nessai_models-0.4.0/nessai_models/__init__.py` & `nessai-models-0.5.0/nessai_models/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,21 +18,23 @@
 from .gaussian import Gaussian
 from .gaussianmixture import GaussianMixture, GaussianMixtureWithData
 from .halfgaussian import HalfGaussian
 from .mixture import MixtureOfDistributions
 from .pyramid import Pyramid
 from .rosenbrock import Rosenbrock
 from .signals import LinearSignal, SinusoidalSignal
+from .slabspike import SlabSpike
 
 __all__ = [
     "Brewer",
     "EggBox",
     "Gaussian",
     "GaussianMixture",
     "GaussianMixtureWithData",
     "HalfGaussian",
     "LinearSignal",
     "MixtureOfDistributions",
     "Pyramid",
     "Rosenbrock",
     "SinusoidalSignal",
+    "SlabSpike",
 ]
```

### Comparing `nessai_models-0.4.0/nessai_models/base.py` & `nessai-models-0.5.0/nessai_models/base.py`

 * *Files identical despite different names*

### Comparing `nessai_models-0.4.0/nessai_models/brewer.py` & `nessai-models-0.5.0/nessai_models/brewer.py`

 * *Files identical despite different names*

### Comparing `nessai_models-0.4.0/nessai_models/eggbox.py` & `nessai-models-0.5.0/nessai_models/eggbox.py`

 * *Files identical despite different names*

### Comparing `nessai_models-0.4.0/nessai_models/gaussian.py` & `nessai-models-0.5.0/nessai_models/gaussian.py`

 * *Files identical despite different names*

### Comparing `nessai_models-0.4.0/nessai_models/gaussianmixture.py` & `nessai-models-0.5.0/nessai_models/gaussianmixture.py`

 * *Files identical despite different names*

### Comparing `nessai_models-0.4.0/nessai_models/halfgaussian.py` & `nessai-models-0.5.0/nessai_models/halfgaussian.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 N-dimensional Gaussian likelihood
 """
+
 from typing import Sequence, Union
 
 import numpy as np
 from scipy.stats import halfnorm
 
 from .base import NDimensionalModel, UniformPriorMixin
 from .gaussian import compute_gaussian_ln_evidence
```

### Comparing `nessai_models-0.4.0/nessai_models/mixture.py` & `nessai-models-0.5.0/nessai_models/mixture.py`

 * *Files identical despite different names*

### Comparing `nessai_models-0.4.0/nessai_models/pyramid.py` & `nessai-models-0.5.0/nessai_models/pyramid.py`

 * *Files identical despite different names*

### Comparing `nessai_models-0.4.0/nessai_models/rosenbrock.py` & `nessai-models-0.5.0/nessai_models/rosenbrock.py`

 * *Files identical despite different names*

### Comparing `nessai_models-0.4.0/nessai_models/signals.py` & `nessai-models-0.5.0/nessai_models/signals.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Signal plus noise models."""
+
 from abc import abstractmethod
 from typing import Dict, List, Optional
 
 import numpy as np
 
 from .base import BaseModel, UniformPriorMixin
```

### Comparing `nessai_models-0.4.0/nessai_models.egg-info/PKG-INFO` & `nessai-models-0.5.0/nessai_models.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 Metadata-Version: 2.1
 Name: nessai-models
-Version: 0.4.0
+Version: 0.5.0
 Summary: Models for nessai
-Home-page: https://github.com/mj-will/nessai-models
-Author: Michael J. Williams
-Author-email: m.williams.4@research.gla.ac.uk
+Author-email: "Michael J. Williams" <michaeljw1@googlemail.com>
 License: MIT
-Keywords: nested sampling,normalising flows,machine learning,nessai
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
+Project-URL: Homepage, https://github.com/mj-will/nessai-models
+Keywords: nested sampling,normalizing flows,machine learning,nessai
+Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Requires-Dist: numpy>=1.9
+Requires-Dist: scipy>0.16
+Requires-Dist: nessai>=0.8.0
 Provides-Extra: dev
+Requires-Dist: black>=24.0; extra == "dev"
+Requires-Dist: flake8; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: pytest>=6.0; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: pytest-integration; extra == "dev"
 
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7105559.svg)](https://doi.org/10.5281/zenodo.7105559)
 [![PyPI](https://img.shields.io/pypi/v/nessai-models)](https://pypi.org/project/nessai-models/)
 [![Integration tests](https://github.com/mj-will/nessai-models/actions/workflows/integration-tests.yml/badge.svg)](https://github.com/mj-will/nessai-models/actions/workflows/integration-tests.yml)
 [![Unit tests](https://github.com/mj-will/nessai-models/actions/workflows/tests.yml/badge.svg)](https://github.com/mj-will/nessai-models/actions/workflows/tests.yml)
 
 # nessai-models
@@ -27,14 +33,15 @@
 
 ## Included models
 
 * n-dimensional unit Gaussian
 * n-dimensional HalfGaussian
 * n-dimensional Rosenbrock
 * n-dimensional mixture of Gaussians
+* n-dimensional slab plus spike model
 * Gaussian mixture using data to based on [this example](https://github.com/johnveitch/cpnest/blob/master/examples/gaussianmixture.py) from `cpnest`
 * n-dimensional Egg Box based on the version in [Feroz et al. 2008](https://arxiv.org/abs/0809.3437)
 * n-dimensional Pyramid-like model
 * n-dimensional Brewer likelihood (Skilling's "Staistical Model") from [Brewer et al.](https://arxiv.org/abs/0912.2380)
 * Linear signal plus Gaussian noise model (`LinearSignal`)
 * Sinusoidal signal plus Gaussian noise model (`SinusoidalSignal`)
 * Mixture of 1-dimensional distributions (`MixtureOfDistributions`)
```

### Comparing `nessai_models-0.4.0/nessai_models.egg-info/SOURCES.txt` & `nessai-models-0.5.0/nessai_models.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 .gitignore
 .pre-commit-config.yaml
 CHANGELOG.md
 README.md
 pyproject.toml
-setup.cfg
-setup.py
 .github/workflows/integration-tests.yml
 .github/workflows/lint.yml
 .github/workflows/publish-to-pypi.yml
 .github/workflows/tests.yml
 examples/basic_example.py
+examples/slabspike.py
 nessai_models/__init__.py
 nessai_models/base.py
 nessai_models/brewer.py
 nessai_models/eggbox.py
 nessai_models/gaussian.py
 nessai_models/gaussianmixture.py
 nessai_models/halfgaussian.py
 nessai_models/mixture.py
 nessai_models/pyramid.py
 nessai_models/rosenbrock.py
 nessai_models/signals.py
+nessai_models/slabspike.py
 nessai_models.egg-info/PKG-INFO
 nessai_models.egg-info/SOURCES.txt
 nessai_models.egg-info/dependency_links.txt
 nessai_models.egg-info/requires.txt
 nessai_models.egg-info/top_level.txt
 tests/conftest.py
 tests/test_base_models.py
```

### Comparing `nessai_models-0.4.0/tests/conftest.py` & `nessai-models-0.5.0/tests/conftest.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """General configuration for all tests"""
+
 from nessai_models import (
     Brewer,
     EggBox,
     Gaussian,
     GaussianMixture,
     GaussianMixtureWithData,
     HalfGaussian,
     LinearSignal,
     MixtureOfDistributions,
     Pyramid,
     Rosenbrock,
     SinusoidalSignal,
+    SlabSpike,
 )
 import pytest
 
 
 all_models = [
     Brewer,
     EggBox,
@@ -23,14 +25,15 @@
     GaussianMixtureWithData,
     HalfGaussian,
     LinearSignal,
     MixtureOfDistributions,
     Pyramid,
     Rosenbrock,
     SinusoidalSignal,
+    SlabSpike,
 ]
 
 
 @pytest.fixture(params=all_models)
 def ModelClass(request):
     """Model classes fixture.
```

### Comparing `nessai_models-0.4.0/tests/test_base_models.py` & `nessai-models-0.5.0/tests/test_base_models.py`

 * *Files identical despite different names*

### Comparing `nessai_models-0.4.0/tests/test_gaussian.py` & `nessai-models-0.5.0/tests/test_gaussian.py`

 * *Files identical despite different names*

### Comparing `nessai_models-0.4.0/tests/test_gaussianmixture.py` & `nessai-models-0.5.0/tests/test_gaussianmixture.py`

 * *Files identical despite different names*

### Comparing `nessai_models-0.4.0/tests/test_mixture.py` & `nessai-models-0.5.0/tests/test_mixture.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests the for the mixture module."""
+
 import multiprocessing.dummy as mp
 from nessai_models.mixture import MixtureOfDistributions
 import numpy as np
 
 import pytest
```

### Comparing `nessai_models-0.4.0/tests/test_nessai_integration.py` & `nessai-models-0.5.0/tests/test_nessai_integration.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,8 +22,8 @@
         resume=False,
         max_iteration=500,
         stopping=1.0,
         plot=False,
     )
     fs.run(plot=False)
     # Make sure a result is produced
-    os.path.exists(os.path.join(output, "result.json"))
+    assert os.path.isfile(os.path.join(output, "result.hdf5"))
```

### Comparing `nessai_models-0.4.0/tests/test_rosenbrock.py` & `nessai-models-0.5.0/tests/test_rosenbrock.py`

 * *Files identical despite different names*

### Comparing `nessai_models-0.4.0/tests/test_signals.py` & `nessai-models-0.5.0/tests/test_signals.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests for signal-based models"""
+
 import numpy as np
 import pytest
 
 from nessai_models.signals import (
     LinearSignal,
     SinusoidalSignal,
 )
```

