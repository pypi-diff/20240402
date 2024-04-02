# Comparing `tmp/keyrings.alt-5.0.0.tar.gz` & `tmp/keyrings.alt-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keyrings.alt-5.0.0.tar", last modified: Mon Jul 24 00:13:06 2023, max compression
+gzip compressed data, was "keyrings.alt-5.0.1.tar", last modified: Tue Apr  2 01:05:50 2024, max compression
```

## Comparing `keyrings.alt-5.0.0.tar` & `keyrings.alt-5.0.1.tar`

### file list

```diff
@@ -1,56 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:13:06.673857 keyrings.alt-5.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:13:06.669857 keyrings.alt-5.0.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:13:06.669857 keyrings.alt-5.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/NEWS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-07-24 00:13:06.673857 keyrings.alt-5.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:13:06.669857 keyrings.alt-5.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:13:06.669857 keyrings.alt-5.0.0/keyrings/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/keyrings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:13:06.669857 keyrings.alt-5.0.0/keyrings/alt/
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/keyrings/alt/Gnome.py
--rw-r--r--   0 runner    (1001) docker     (123)    12428 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/keyrings/alt/Google.py
--rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/keyrings/alt/Windows.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/keyrings/alt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/keyrings/alt/_win_crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/keyrings/alt/escape.py
--rw-r--r--   0 runner    (1001) docker     (123)     7721 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/keyrings/alt/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/keyrings/alt/file_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/keyrings/alt/keyczar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/keyrings/alt/multi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:13:06.669857 keyrings.alt-5.0.0/keyrings.alt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-07-24 00:13:06.000000 keyrings.alt-5.0.0/keyrings.alt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-24 00:13:06.000000 keyrings.alt-5.0.0/keyrings.alt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 00:13:06.000000 keyrings.alt-5.0.0/keyrings.alt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-24 00:13:06.000000 keyrings.alt-5.0.0/keyrings.alt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-24 00:13:06.000000 keyrings.alt-5.0.0/keyrings.alt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-24 00:13:06.000000 keyrings.alt-5.0.0/keyrings.alt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-24 00:13:06.673857 keyrings.alt-5.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 00:13:06.673857 keyrings.alt-5.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/tests/mocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/tests/test_Gnome.py
--rw-r--r--   0 runner    (1001) docker     (123)    15281 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/tests/test_Google.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/tests/test_Windows.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/tests/test_crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)     7819 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/tests/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/tests/test_keyczar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/tests/test_multi.py
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/towncrier.toml
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-24 00:12:40.000000 keyrings.alt-5.0.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:05:50.099679 keyrings.alt-5.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-02 01:05:28.000000 keyrings.alt-5.0.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-02 01:05:28.000000 keyrings.alt-5.0.1/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:05:50.091679 keyrings.alt-5.0.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-02 01:05:28.000000 keyrings.alt-5.0.1/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-02 01:05:28.000000 keyrings.alt-5.0.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:05:50.091679 keyrings.alt-5.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-04-02 01:05:28.000000 keyrings.alt-5.0.1/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-02 01:05:28.000000 keyrings.alt-5.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-02 01:05:28.000000 keyrings.alt-5.0.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-02 01:05:28.000000 keyrings.alt-5.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-04-02 01:05:28.000000 keyrings.alt-5.0.1/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-04-02 01:05:50.099679 keyrings.alt-5.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-02 01:05:28.000000 keyrings.alt-5.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-02 01:05:28.000000 keyrings.alt-5.0.1/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-02 01:05:28.000000 keyrings.alt-5.0.1/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:05:50.091679 keyrings.alt-5.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-02 01:05:28.000000 keyrings.alt-5.0.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-02 01:05:28.000000 keyrings.alt-5.0.1/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-02 01:05:28.000000 keyrings.alt-5.0.1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:05:50.091679 keyrings.alt-5.0.1/keyrings/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-02 01:05:28.000000 keyrings.alt-5.0.1/keyrings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:05:50.095679 keyrings.alt-5.0.1/keyrings/alt/
+-rw-r--r--   0 runner    (1001) docker     (127)     4366 2024-04-02 01:05:28.000000 keyrings.alt-5.0.1/keyrings/alt/Gnome.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12240 2024-04-02 01:05:28.000000 keyrings.alt-5.0.1/keyrings/alt/Google.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-04-02 01:05:28.000000 keyrings.alt-5.0.1/keyrings/alt/Windows.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 01:05:28.000000 keyrings.alt-5.0.1/keyrings/alt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-04-02 01:05:28.000000 keyrings.alt-5.0.1/keyrings/alt/_win_crypto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-02 01:05:28.000000 keyrings.alt-5.0.1/keyrings/alt/escape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7671 2024-04-02 01:05:28.000000 keyrings.alt-5.0.1/keyrings/alt/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6488 2024-04-02 01:05:28.000000 keyrings.alt-5.0.1/keyrings/alt/file_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-04-02 01:05:28.000000 keyrings.alt-5.0.1/keyrings/alt/keyczar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-04-02 01:05:28.000000 keyrings.alt-5.0.1/keyrings/alt/multi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:05:50.095679 keyrings.alt-5.0.1/keyrings.alt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-04-02 01:05:50.000000 keyrings.alt-5.0.1/keyrings.alt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-02 01:05:50.000000 keyrings.alt-5.0.1/keyrings.alt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 01:05:50.000000 keyrings.alt-5.0.1/keyrings.alt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-02 01:05:50.000000 keyrings.alt-5.0.1/keyrings.alt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-02 01:05:50.000000 keyrings.alt-5.0.1/keyrings.alt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-02 01:05:50.000000 keyrings.alt-5.0.1/keyrings.alt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-02 01:05:28.000000 keyrings.alt-5.0.1/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-02 01:05:28.000000 keyrings.alt-5.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-02 01:05:28.000000 keyrings.alt-5.0.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-02 01:05:28.000000 keyrings.alt-5.0.1/ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-02 01:05:50.099679 keyrings.alt-5.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:05:50.095679 keyrings.alt-5.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 01:05:28.000000 keyrings.alt-5.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6356 2024-04-02 01:05:28.000000 keyrings.alt-5.0.1/tests/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-02 01:05:28.000000 keyrings.alt-5.0.1/tests/test_Gnome.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15283 2024-04-02 01:05:28.000000 keyrings.alt-5.0.1/tests/test_Google.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-02 01:05:28.000000 keyrings.alt-5.0.1/tests/test_Windows.py
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-02 01:05:28.000000 keyrings.alt-5.0.1/tests/test_crypto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7838 2024-04-02 01:05:28.000000 keyrings.alt-5.0.1/tests/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-04-02 01:05:28.000000 keyrings.alt-5.0.1/tests/test_keyczar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-02 01:05:28.000000 keyrings.alt-5.0.1/tests/test_multi.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-02 01:05:28.000000 keyrings.alt-5.0.1/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-02 01:05:28.000000 keyrings.alt-5.0.1/tox.ini
```

### Comparing `keyrings.alt-5.0.0/.github/workflows/main.yml` & `keyrings.alt-5.0.1/.github/workflows/main.yml`

 * *Files 19% similar despite different names*

```diff
@@ -1,100 +1,98 @@
 name: tests
 
-on: [push, pull_request]
+on:
+  merge_group:
+  push:
+    branches-ignore:
+    # temporary GH branches relating to merge queues (jaraco/skeleton#93)
+    - gh-readonly-queue/**
+    tags:
+    # required if branches-ignore is supplied (jaraco/skeleton#103)
+    - '**'
+  pull_request:
 
 permissions:
   contents: read
 
 env:
-  # Environment variables to support color support (jaraco/skeleton#66):
-  # Request colored output from CLI tools supporting it. Different tools
-  # interpret the value differently. For some, just being set is sufficient.
-  # For others, it must be a non-zero integer. For yet others, being set
-  # to a non-empty value is sufficient. For tox, it must be one of
-  # <blank>, 0, 1, false, no, off, on, true, yes. The only enabling value
-  # in common is "1".
+  # Environment variable to support color support (jaraco/skeleton#66)
   FORCE_COLOR: 1
-  # MyPy's color enforcement (must be a non-zero number)
-  MYPY_FORCE_COLOR: -42
-  # Recognized by the `py` package, dependency of `pytest` (must be "1")
-  PY_COLORS: 1
-  # Make tox-wrapped tools see color requests
-  TOX_TESTENV_PASSENV: >-
-    FORCE_COLOR
-    MYPY_FORCE_COLOR
-    NO_COLOR
-    PY_COLORS
-    PYTEST_THEME
-    PYTEST_THEME_MODE
 
   # Suppress noisy pip warnings
   PIP_DISABLE_PIP_VERSION_CHECK: 'true'
   PIP_NO_PYTHON_VERSION_WARNING: 'true'
   PIP_NO_WARN_SCRIPT_LOCATION: 'true'
 
-  # Disable the spinner, noise in GHA; TODO(webknjaz): Fix this upstream
-  # Must be "1".
-  TOX_PARALLEL_NO_SPINNER: 1
+  # Ensure tests can sense settings about the environment
+  TOX_OVERRIDE: >-
+    testenv.pass_env+=GITHUB_*,FORCE_COLOR
 
 
 jobs:
   test:
     strategy:
       matrix:
         python:
         - "3.8"
-        - "3.11"
         - "3.12"
         platform:
         - ubuntu-latest
         - macos-latest
         - windows-latest
         include:
         - python: "3.9"
           platform: ubuntu-latest
         - python: "3.10"
           platform: ubuntu-latest
-        - python: pypy3.9
+        - python: "3.11"
+          platform: ubuntu-latest
+        - python: pypy3.10
           platform: ubuntu-latest
     runs-on: ${{ matrix.platform }}
-    continue-on-error: ${{ matrix.python == '3.12' }}
+    continue-on-error: ${{ matrix.python == '3.13' }}
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python }}
           allow-prereleases: true
       - name: Install tox
-        run: |
-          python -m pip install tox
+        run: python -m pip install tox
       - name: Run
         run: tox
 
-  docs:
+  collateral:
+    strategy:
+      fail-fast: false
+      matrix:
+        job:
+        - diffcov
+        - docs
     runs-on: ubuntu-latest
-    env:
-      TOXENV: docs
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
+        with:
+          fetch-depth: 0
       - name: Setup Python
         uses: actions/setup-python@v4
+        with:
+          python-version: 3.x
       - name: Install tox
-        run: |
-          python -m pip install tox
-      - name: Run
-        run: tox
+        run: python -m pip install tox
+      - name: Eval ${{ matrix.job }}
+        run: tox -e ${{ matrix.job }}
 
   check:  # This job does nothing and is only used for the branch protection
     if: always()
 
     needs:
     - test
-    - docs
+    - collateral
 
     runs-on: ubuntu-latest
 
     steps:
     - name: Decide whether the needed jobs succeeded or failed
       uses: re-actors/alls-green@release/v1
       with:
@@ -105,20 +103,19 @@
       contents: write
     needs:
     - check
     if: github.event_name == 'push' && contains(github.ref, 'refs/tags/')
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
           python-version: 3.x
       - name: Install tox
-        run: |
-          python -m pip install tox
+        run: python -m pip install tox
       - name: Run
         run: tox -e release
         env:
           TWINE_PASSWORD: ${{ secrets.PYPI_TOKEN }}
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```

### Comparing `keyrings.alt-5.0.0/LICENSE` & `keyrings.alt-5.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `keyrings.alt-5.0.0/NEWS.rst` & `keyrings.alt-5.0.1/NEWS.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+v5.0.1
+======
+
+Bugfixes
+--------
+
+- Fix encoding warnings.
+
+
 v5.0.0
 ======
 
 Features
 --------
 
 - Require Python 3.8 or later.
```

### Comparing `keyrings.alt-5.0.0/PKG-INFO` & `keyrings.alt-5.0.1/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,24 @@
-Metadata-Version: 2.1
-Name: keyrings.alt
-Version: 5.0.0
-Summary: Alternate keyring implementations
-Home-page: https://github.com/jaraco/keyrings.alt
-Author: Jason R. Coombs
-Author-email: jaraco@jaraco.com
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.8
-Provides-Extra: testing
-Provides-Extra: docs
-License-File: LICENSE
-
 .. image:: https://img.shields.io/pypi/v/keyrings.alt.svg
    :target: https://pypi.org/project/keyrings.alt
 
 .. image:: https://img.shields.io/pypi/pyversions/keyrings.alt.svg
 
-.. image:: https://github.com/jaraco/keyrings.alt/workflows/tests/badge.svg
+.. image:: https://github.com/jaraco/keyrings.alt/actions/workflows/main.yml/badge.svg
    :target: https://github.com/jaraco/keyrings.alt/actions?query=workflow%3A%22tests%22
    :alt: tests
 
 .. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
     :target: https://github.com/astral-sh/ruff
     :alt: Ruff
 
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-   :target: https://github.com/psf/black
-   :alt: Code style: Black
-
 .. .. image:: https://readthedocs.org/projects/PROJECT_RTD/badge/?version=latest
 ..    :target: https://PROJECT_RTD.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://img.shields.io/badge/skeleton-2023-informational
+.. image:: https://img.shields.io/badge/skeleton-2024-informational
    :target: https://blog.jaraco.com/skeleton
 
 .. image:: https://tidelift.com/badges/package/pypi/keyrings.alt
    :target: https://tidelift.com/subscription/pkg/pypi-keyrings.alt?utm_source=pypi-keyrings.alt&utm_medium=readme
 
 Alternate keyring backend implementations for use with the
 `keyring package <https://pypi.python.org/pypi/keyring>`_.
```

### Comparing `keyrings.alt-5.0.0/docs/conf.py` & `keyrings.alt-5.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `keyrings.alt-5.0.0/docs/index.rst` & `keyrings.alt-5.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `keyrings.alt-5.0.0/keyrings/alt/Gnome.py` & `keyrings.alt-5.0.1/keyrings/alt/Gnome.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,16 @@
 
     gi.require_version('GnomeKeyring', '1.0')
     from gi.repository import GnomeKeyring
 except (ImportError, ValueError, AttributeError):
     pass
 
 from jaraco.classes import properties
-
 from keyring.backend import KeyringBackend
-from keyring.errors import PasswordSetError, PasswordDeleteError
+from keyring.errors import PasswordDeleteError, PasswordSetError
 
 
 class Keyring(KeyringBackend):
     """Gnome Keyring"""
 
     KEYRING_NAME = None
     """
@@ -76,15 +75,15 @@
         GnomeKeyring.Attribute.list_append_string(attrs, 'service', service)
         GnomeKeyring.Attribute.list_append_string(
             attrs, 'application', 'python-keyring'
         )
         result = GnomeKeyring.item_create_sync(
             self.keyring_name,
             GnomeKeyring.ItemType.NETWORK_PASSWORD,
-            "Password for '%s' on '%s'" % (username, service),
+            f"Password for '{username}' on '{service}'",
             attrs,
             password,
             True,
         )[0]
         if result == GnomeKeyring.Result.CANCELLED:
             # The user pressed "Cancel" when prompted to unlock their keyring.
             raise PasswordSetError("Cancelled by user")
```

### Comparing `keyrings.alt-5.0.0/keyrings/alt/Google.py` & `keyrings.alt-5.0.1/keyrings/alt/Google.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,33 @@
-from __future__ import absolute_import
-
-import os
-import sys
-import copy
-import codecs
 import base64
+import codecs
+import copy
 import io
+import os
 import pickle
+import sys
 
 try:
     import gdata.docs.service
 except ImportError:
     pass
 
 from jaraco.classes import properties
+from jaraco.context import ExceptionTrap
+from keyring import credentials, errors
+from keyring.backend import KeyringBackend
 
 from . import keyczar
-from keyring import errors
-from keyring import credentials
-from keyring.backend import KeyringBackend
-from keyring.errors import ExceptionRaisedContext
 
 
 class EnvironCredential(credentials.EnvironCredential):
     """Retrieve credentials from specifically named environment variables"""
 
     def __init__(self):
-        super(EnvironCredential, self).__init__(
-            'GOOGLE_KEYRING_USER', 'GOOGLE_KEYRING_PASSWORD'
-        )
+        super().__init__('GOOGLE_KEYRING_USER', 'GOOGLE_KEYRING_PASSWORD')
 
 
 class DocsKeyring(KeyringBackend):
     """Backend that stores keyring on Google Docs.
     Note that login and any other initialisation is deferred until it is
     actually required to allow this keyring class to be added to the
     global _all_keyring list.
@@ -75,19 +70,21 @@
     def priority(cls):
         if not cls._has_gdata():
             raise RuntimeError("Requires gdata")
         if not keyczar.has_keyczar():
             raise RuntimeError("Requires keyczar")
         return 3
 
+    # For Python 3.8 compatibility
+    passes = ExceptionTrap().passes
+
+    @passes
     @classmethod
     def _has_gdata(cls):
-        with ExceptionRaisedContext() as exc:
-            gdata.__name__
-        return not bool(exc)
+        gdata.__name__
 
     def get_password(self, service, username):
         """Get password of the username for the service"""
         result = self._get_entry(self._keyring, service, username)
         if result:
             result = self._decrypt(result)
         return result
@@ -125,16 +122,16 @@
                     return
                 else:
                     raise errors.PasswordSetError(
                         'Failed write after conflict detected'
                     )
             else:
                 raise errors.PasswordSetError(
-                    'Conflict detected, service:%s and username:%s was '
-                    'set to a different value by someone else' % (service, username)
+                    f'Conflict detected, service:{service} and username:{username} was '
+                    'set to a different value by someone else'
                 )
 
         raise errors.PasswordSetError('Could not save keyring')
 
     def delete_password(self, service, username):
         return self._del_entry(self._keyring, service, username)
 
@@ -217,16 +214,15 @@
 
         if not docs.entry:
             if self.can_create:
                 docs_entry = None
                 keyring_dict = {}
             else:
                 raise errors.InitError(
-                    '%s not found in %s and create not permitted'
-                    % (self._get_doc_title(), self.collection)
+                    f'{self._get_doc_title()} not found in {self.collection} and create not permitted'
                 )
         else:
             docs_entry = docs.entry[0]
             file_contents = ''
             try:
                 url = docs_entry.content.src
                 url += '&exportFormat=txt'
@@ -322,21 +318,21 @@
     variables
     """
 
     def __init__(self):
         crypter = keyczar.EnvironCrypter()
         credential = EnvironCredential()
         source = os.environ.get('GOOGLE_KEYRING_SOURCE')
-        super(KeyczarDocsKeyring, self).__init__(credential, source, crypter)
+        super().__init__(credential, source, crypter)
 
     def supported(self):
         """
         Return if this keyring supports current environment:
         -1: not applicable
         0: suitable
         1: recommended
         """
         try:
             __import__('keyczar.keyczar')
-            return super(KeyczarDocsKeyring, self).supported()
+            return super().supported()
         except ImportError:
             return -1
```

### Comparing `keyrings.alt-5.0.0/keyrings/alt/Windows.py` & `keyrings.alt-5.0.1/keyrings/alt/Windows.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,41 @@
-import sys
 import base64
 import platform
+import sys
 
 from jaraco.classes import properties
-
+from jaraco.context import ExceptionTrap
 from keyring.backend import KeyringBackend
-from keyring.errors import PasswordDeleteError, ExceptionRaisedContext
+from keyring.errors import PasswordDeleteError
+
 from . import file_base
 
 try:
     import winreg
 except ImportError:
     pass
 
 try:
     from . import _win_crypto
 except ImportError:
     pass
 
 
+# For Python 3.8 compatibility
+passes = ExceptionTrap().passes
+
+
+@passes
 def has_wincrypto():
     """
     Does this environment have wincrypto?
     Should return False even when Mercurial's Demand Import allowed import of
     _win_crypto, so accesses an attribute of the module.
     """
-    with ExceptionRaisedContext() as exc:
-        _win_crypto.__name__
-    return not bool(exc)
+    _win_crypto.__name__
 
 
 class EncryptedKeyring(file_base.Keyring):
     """
     A File-based keyring secured by Windows Crypto API.
     """
 
@@ -88,15 +92,15 @@
             hkey = winreg.OpenKey(winreg.HKEY_CURRENT_USER, key)
             password_saved = winreg.QueryValueEx(hkey, username)[0]
             password_base64 = password_saved.encode('ascii')
             # decode with base64
             password_encrypted = base64.decodebytes(password_base64)
             # decrypted the password
             password = _win_crypto.decrypt(password_encrypted).decode('utf-8')
-        except EnvironmentError:
+        except OSError:
             password = None
         return password
 
     def set_password(self, service, username, password):
         """Write the password to the registry"""
         # encrypt the password
         password_encrypted = _win_crypto.encrypt(password.encode('utf-8'))
@@ -115,28 +119,28 @@
         try:
             key_name = self._key_for_service(service)
             hkey = winreg.OpenKey(
                 winreg.HKEY_CURRENT_USER, key_name, 0, winreg.KEY_ALL_ACCESS
             )
             winreg.DeleteValue(hkey, username)
             winreg.CloseKey(hkey)
-        except WindowsError:
+        except OSError:
             e = sys.exc_info()[1]
             raise PasswordDeleteError(e)
         self._delete_key_if_empty(service)
 
     def _delete_key_if_empty(self, service):
         key_name = self._key_for_service(service)
         key = winreg.OpenKey(
             winreg.HKEY_CURRENT_USER, key_name, 0, winreg.KEY_ALL_ACCESS
         )
         try:
             winreg.EnumValue(key, 0)
             return
-        except WindowsError:
+        except OSError:
             pass
         winreg.CloseKey(key)
 
         # it's empty; delete everything
         while key_name != 'Software':
             parent, sep, base = key_name.rpartition('\\')
             key = winreg.OpenKey(
```

### Comparing `keyrings.alt-5.0.0/keyrings/alt/_win_crypto.py` & `keyrings.alt-5.0.1/keyrings/alt/_win_crypto.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from __future__ import unicode_literals
-
 from ctypes import (
-    Structure,
     POINTER,
+    WINFUNCTYPE,
+    Structure,
+    WinDLL,
+    byref,
+    c_char_p,
     c_void_p,
     cast,
     create_string_buffer,
-    c_char_p,
-    byref,
     memmove,
+    windll,
 )
-from ctypes import windll, WinDLL, WINFUNCTYPE
 
 try:
     from ctypes import wintypes
 except ValueError:
     # see http://bugs.python.org/issue16396
     raise ImportError("wintypes")
```

### Comparing `keyrings.alt-5.0.0/keyrings/alt/escape.py` & `keyrings.alt-5.0.1/keyrings/alt/escape.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 """
 
 import re
 import string
 
 LEGAL_CHARS = (
     getattr(string, 'letters', None)  # Python 2
-    or getattr(string, 'ascii_letters')  # Python 3
+    or string.ascii_letters  # Python 3
 ) + string.digits
 
 ESCAPE_FMT = "_%02X"
 
 
 def _escape_char(c):
     "Single char escape. Return the char, escaped if not already legal"
```

### Comparing `keyrings.alt-5.0.0/keyrings/alt/file.py` & `keyrings.alt-5.0.1/keyrings/alt/file.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-from __future__ import with_statement
-
+import configparser
+import getpass
+import json
 import os
 import sys
-import json
-import getpass
-import configparser
 
 from jaraco.classes import properties
 
-from .escape import escape as escape_for_ini
 from keyrings.alt.file_base import Keyring, decodebytes, encodebytes
 
+from .escape import escape as escape_for_ini
+
 
 class PlaintextKeyring(Keyring):
     """Simple File Keyring with no encryption"""
 
     priority = 0.5  # type: ignore
     "Applicable for all platforms, but not recommended"
 
@@ -42,21 +41,21 @@
 
     def __init__(self):
         vars(self).update(self._get_crypto_impl())
 
     @staticmethod
     def _get_crypto_impl():
         try:
-            from Cryptodome.Protocol import KDF  # noqa: F401
-            from Cryptodome.Cipher import AES  # noqa: F401
             import Cryptodome.Random as Random  # noqa: F401
+            from Cryptodome.Cipher import AES  # noqa: F401
+            from Cryptodome.Protocol import KDF  # noqa: F401
         except ImportError:
-            from Crypto.Protocol import KDF  # noqa: F401
-            from Crypto.Cipher import AES  # noqa: F401
             import Crypto.Random as Random  # noqa: F401
+            from Crypto.Cipher import AES  # noqa: F401
+            from Crypto.Protocol import KDF  # noqa: F401
         return locals()
 
     def _create_cipher(self, password, salt, IV):
         """
         Create the cipher object to encrypt or decrypt a payload.
         """
         pw = self.KDF.PBKDF2(password, salt, dkLen=self.block_size)
@@ -76,15 +75,15 @@
             return password
 
 
 class EncryptedKeyring(Encrypted, Keyring):
     """PyCryptodome File Keyring"""
 
     filename = 'crypted_pass.cfg'
-    pw_prefix = 'pw:'.encode()
+    pw_prefix = b'pw:'
 
     @properties.classproperty
     def priority(cls):
         "Applicable for all platforms, but not recommended."
         try:
             cls._get_crypto_impl()
         except ImportError:  # pragma: no cover
@@ -119,15 +118,15 @@
         """
         Check if the file exists and has the expected password reference.
         """
         if not os.path.exists(self.file_path):
             return False
         self._migrate()
         config = configparser.RawConfigParser()
-        config.read(self.file_path)
+        config.read(self.file_path, encoding='utf-8')
         try:
             config.get(
                 escape_for_ini('keyring-setting'), escape_for_ini('password reference')
             )
         except (configparser.NoSectionError, configparser.NoOptionError):
             return False
         try:
@@ -153,16 +152,15 @@
 
         # remove pointless crypto module name
         if scheme.startswith('PyCrypto '):
             scheme = scheme[9:]
 
         if scheme != self.scheme:
             raise ValueError(
-                "Encryption scheme mismatch "
-                "(exp.: %s, found: %s)" % (self.scheme, scheme)
+                "Encryption scheme mismatch " f"(exp.: {self.scheme}, found: {scheme})"
             )
 
     def _check_version(self, config):
         """
         check for a valid version
         an existing scheme implies an existing version as well
```

### Comparing `keyrings.alt-5.0.0/keyrings/alt/file_base.py` & `keyrings.alt-5.0.1/keyrings/alt/file_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-from __future__ import with_statement
-
-import os
 import abc
 import configparser
-from base64 import encodebytes, decodebytes
+import os
+from base64 import decodebytes, encodebytes
 
 from jaraco.classes import properties
-
-from keyring.errors import PasswordDeleteError
 from keyring.backend import KeyringBackend
+from keyring.errors import PasswordDeleteError
 from keyring.util import platform_
+
 from .escape import escape as escape_for_ini
 
 
 class FileBacked:
     @abc.abstractproperty
     def filename(self):
         """
@@ -92,15 +90,15 @@
         assoc = self._generate_assoc(service, username)
         service = escape_for_ini(service)
         username = escape_for_ini(username)
 
         # load the passwords from the file
         config = configparser.RawConfigParser()
         if os.path.exists(self.file_path):
-            config.read(self.file_path)
+            config.read(self.file_path, encoding='utf-8')
 
         # fetch the password
         try:
             password_base64 = config.get(service, username).encode()
             # decode with base64
             password_encrypted = decodebytes(password_base64)
             # decrypt the password with associated data
@@ -134,52 +132,52 @@
 
     def _write_config_value(self, service, key, value):
         # ensure the file exists
         self._ensure_file_path()
 
         # load the keyring from the disk
         config = configparser.RawConfigParser()
-        config.read(self.file_path)
+        config.read(self.file_path, encoding='utf-8')
 
         service = escape_for_ini(service)
         key = escape_for_ini(key)
 
         # update the keyring with the password
         if not config.has_section(service):
             config.add_section(service)
         config.set(service, key, value)
 
         # save the keyring back to the file
-        with open(self.file_path, 'w') as config_file:
+        with open(self.file_path, 'w', encoding='utf-8') as config_file:
             config.write(config_file)
 
     def _ensure_file_path(self):
         """
         Ensure the storage path exists.
         If it doesn't, create it with "go-rwx" permissions.
         """
         storage_root = os.path.dirname(self.file_path)
         needs_storage_root = storage_root and not os.path.isdir(storage_root)
         if needs_storage_root:  # pragma: no cover
             os.makedirs(storage_root)
         if not os.path.isfile(self.file_path):
             # create the file without group/world permissions
-            with open(self.file_path, 'w'):
+            with open(self.file_path, 'w', encoding='utf-8'):
                 pass
             user_read_write = 0o600
             os.chmod(self.file_path, user_read_write)
 
     def delete_password(self, service, username):
         """Delete the password for the username of the service."""
         service = escape_for_ini(service)
         username = escape_for_ini(username)
         config = configparser.RawConfigParser()
         if os.path.exists(self.file_path):
-            config.read(self.file_path)
+            config.read(self.file_path, encoding='utf-8')
         try:
             if not config.remove_option(service, username):
                 raise PasswordDeleteError("Password not found")
         except configparser.NoSectionError:
             raise PasswordDeleteError("Password not found")
         # update the file
-        with open(self.file_path, 'w') as config_file:
+        with open(self.file_path, 'w', encoding='utf-8') as config_file:
             config.write(config_file)
```

### Comparing `keyrings.alt-5.0.0/keyrings/alt/keyczar.py` & `keyrings.alt-5.0.1/keyrings/alt/keyczar.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,27 @@
-from __future__ import absolute_import
-
-import os
 import abc
+import os
+
+from jaraco.context import ExceptionTrap
 
 try:
     from keyczar import keyczar
 except ImportError:
     pass
 
 import keyring.backend
-from keyring import errors
 
 
+# For Python 3.8 compatibility
+passes = ExceptionTrap().passes
+
+
+@passes
 def has_keyczar():
-    with errors.ExceptionRaisedContext() as exc:
-        keyczar.__name__
-    return not bool(exc)
+    keyczar.__name__
 
 
 class BaseCrypter(keyring.backend.Crypter):
     """Base Keyczar keyset encryption and decryption.
     The keyset initialisation is deferred until required.
     """
```

### Comparing `keyrings.alt-5.0.0/keyrings/alt/multi.py` & `keyrings.alt-5.0.1/keyrings/alt/multi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import itertools
 
 from jaraco.classes import properties
-
-from keyring.backend import KeyringBackend
 from keyring import errors
+from keyring.backend import KeyringBackend
 
 
 class MultipartKeyringWrapper(KeyringBackend):
-
     """A wrapper around an existing keyring that breaks the password into
     smaller parts to handle implementations that have limits on the maximum
     length of passwords i.e. Windows Vault
     """
 
     def __init__(self, keyring, max_password_size=512):
         self._keyring = keyring
```

### Comparing `keyrings.alt-5.0.0/keyrings.alt.egg-info/SOURCES.txt` & `keyrings.alt-5.0.1/keyrings.alt.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 NEWS.rst
 README.rst
 SECURITY.md
 conftest.py
 mypy.ini
 pyproject.toml
 pytest.ini
+ruff.toml
 setup.cfg
 towncrier.toml
 tox.ini
 .github/FUNDING.yml
 .github/dependabot.yml
 .github/workflows/main.yml
 docs/conf.py
```

### Comparing `keyrings.alt-5.0.0/setup.cfg` & `keyrings.alt-5.0.1/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -9,38 +9,28 @@
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 
 [options]
-packages = find_namespace:
 include_package_data = true
 python_requires = >=3.8
 install_requires = 
 	jaraco.classes
-
-[options.packages.find]
-exclude = 
-	build*
-	dist*
-	docs*
-	tests*
+	jaraco.context
 
 [options.extras_require]
 testing = 
-	pytest >= 6
+	pytest >= 6, != 8.1.1
 	pytest-checkdocs >= 2.4
-	pytest-black >= 0.3.7; \
-	python_implementation != "PyPy"
 	pytest-cov
-	pytest-mypy >= 0.9.1; \
-	python_implementation != "PyPy"
+	pytest-mypy
 	pytest-enabler >= 2.2
-	pytest-ruff
+	pytest-ruff >= 0.2.1
 	
 	backports.unittest_mock
 	keyring >= 20
 	
 	pycryptodomex
 	pycryptodome
```

### Comparing `keyrings.alt-5.0.0/tests/mocks.py` & `keyrings.alt-5.0.1/tests/mocks.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,15 +131,15 @@
         converter=None,
     ):
         self._put_data = None
         if not hasattr(self, '_put_count'):
             self._put_count = 0
         if hasattr(self, '_put_err'):
             # allow for a list of errors
-            if type(self._put_err) == list:
+            if isinstance(self._put_err, list):
                 put_err = self._put_err.pop(0)
                 if not len(self._put_err):
                     delattr(self, '_put_err')
             else:
                 put_err = self._put_err
             if type(put_err) == tuple:
                 raise put_err[0](put_err[1])
@@ -167,15 +167,15 @@
                 raise self._request_err()
         if hasattr(self, '_request_response'):
             return MockHttpResponse(self._request_response)
 
 
 class MockHttpResponse(io.BytesIO):
     def __init__(self, response_dict):
-        super(MockHttpResponse, self).__init__(response_dict.get('data', ''))
+        super().__init__(response_dict.get('data', ''))
         self.status = response_dict.get('status', 200)
         self.reason = response_dict.get('reason', '')
 
 
 class MockListFeed:
     @property
     def entry(self):
```

### Comparing `keyrings.alt-5.0.0/tests/test_Gnome.py` & `keyrings.alt-5.0.1/tests/test_Gnome.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-import types
 import sys
+import types
 import unittest
 
 from keyring.testing.backend import BackendBasicTests
 from keyring.testing.util import NoNoneDictMutator
+
 from keyrings.alt import Gnome
 
 
 def ImportBlesser(*names, **changes):
     """A context manager to temporarily make it possible to import a module"""
     for name in names:
         changes[name] = types.ModuleType(name)
```

### Comparing `keyrings.alt-5.0.0/tests/test_Google.py` & `keyrings.alt-5.0.1/tests/test_Google.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-import codecs
 import base64
-import unittest
+import codecs
 import pickle
+import unittest
 
+from keyring import errors
+from keyring.backend import NullCrypter
+from keyring.credentials import SimpleCredential
 from keyring.testing.backend import BackendBasicTests
+
 from keyrings.alt import Google
-from keyring.credentials import SimpleCredential
-from keyring.backend import NullCrypter
-from keyring import errors
+
 from . import mocks
 
 
 def is_gdata_supported():
     try:
         __import__('gdata.service')
     except ImportError:
```

### Comparing `keyrings.alt-5.0.0/tests/test_Windows.py` & `keyrings.alt-5.0.1/tests/test_Windows.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-from __future__ import print_function
-
 import sys
 
 import pytest
+from keyring.testing.backend import BackendBasicTests
 
 from keyrings.alt import Windows
-from keyring.testing.backend import BackendBasicTests
+
 from .test_file import FileKeyringTests
 
 
 def is_win32_crypto_supported():
     try:
         __import__('keyrings.alt._win_crypto')
     except ImportError:
```

### Comparing `keyrings.alt-5.0.0/tests/test_crypto.py` & `keyrings.alt-5.0.1/tests/test_crypto.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import getpass
 from unittest import mock
 
 import pytest
 
-from .test_file import FileKeyringTests
-
 from keyrings.alt import file
 
+from .test_file import FileKeyringTests
+
 
 def is_crypto_supported():
     try:
         __import__('Cryptodome.Cipher.AES')
         __import__('Cryptodome.Protocol.KDF')
         __import__('Cryptodome.Random')
     except ImportError:
```

### Comparing `keyrings.alt-5.0.0/tests/test_file.py` & `keyrings.alt-5.0.1/tests/test_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,23 @@
-import os
-import tempfile
-import sys
+import configparser
 import errno
 import getpass
-import configparser
-
-import pytest
+import os
+import sys
+import tempfile
 from unittest import mock
 
+import pytest
+from keyring.errors import PasswordDeleteError
 from keyring.testing.backend import BackendBasicTests
 from keyring.testing.util import random_string
 
 from keyrings.alt import file
-from keyrings.alt.file_base import encodebytes
 from keyrings.alt.escape import escape as escape_for_ini
-
-from keyring.errors import PasswordDeleteError
+from keyrings.alt.file_base import encodebytes
 
 
 class FileKeyringTests(BackendBasicTests):
     @pytest.fixture(autouse=True)
     def _init_properties_for_file(self):
         self.keyring.file_path = tempfile.mktemp()
         yield
@@ -33,19 +31,19 @@
             e = sys.exc_info()[1]
             if e.errno != errno.ENOENT:  # No such file or directory
                 raise
 
     def get_config(self):
         # setting a password triggers keyring file creation
         config = configparser.RawConfigParser()
-        config.read(self.keyring.file_path)
+        config.read(self.keyring.file_path, encoding='utf-8')
         return config
 
     def save_config(self, config):
-        with open(self.keyring.file_path, 'w') as config_file:
+        with open(self.keyring.file_path, 'w', encoding='utf-8') as config_file:
             config.write(config_file)
 
     def test_encrypt_decrypt(self):
         password = random_string(20)
         # keyring.encrypt expects bytes
         password = password.encode('utf-8')
         encrypted = self.keyring.encrypt(password)
@@ -53,15 +51,15 @@
         assert password == self.keyring.decrypt(encrypted)
 
     def test_encrypt_decrypt_without_assoc(self):
         # generate keyring
         self.set_password('system', 'user', 'password')
         config = self.get_config()
         # generate and save password without assoc data
-        encrypted = self.keyring.encrypt('password'.encode('utf-8'))
+        encrypted = self.keyring.encrypt(b'password')
         password_base64 = '\n' + encodebytes(encrypted).decode()
         config.set('system', 'user', password_base64)
         self.save_config(config)
         assert self.keyring.get_password('system', 'user') == 'password'
 
     def test_delete_password(self):
         self.set_password('system', 'user', 'password')
```

### Comparing `keyrings.alt-5.0.0/tests/test_keyczar.py` & `keyrings.alt-5.0.1/tests/test_keyczar.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
 import unittest
 
 from keyrings.alt import keyczar
+
 from . import mocks
 
 
 class KeyczarCrypterTestCase(unittest.TestCase):
-
     """Test the keyczar crypter"""
 
     def setUp(self):
         self._orig_keyczar = keyczar.keyczar if hasattr(keyczar, 'keyczar') else None
         keyczar.keyczar = mocks.MockKeyczar()
 
     def tearDown(self):
```

### Comparing `keyrings.alt-5.0.0/tests/test_multi.py` & `keyrings.alt-5.0.1/tests/test_multi.py`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import unittest
 
+import keyring.errors
 from keyring.backend import KeyringBackend
+
 from keyrings.alt import multi
-import keyring.errors
 
 
 class MultipartKeyringWrapperTestCase(unittest.TestCase):
-
     """Test the wrapper that breaks passwords into smaller chunks"""
 
     class MockKeyring(KeyringBackend):
         priority = 1  # type: ignore
 
         def __init__(self):
             self.passwords = {}
```

