# Comparing `tmp/jupyter-analysis-tools-0.1.6.dev5.tar.gz` & `tmp/jupyter-analysis-tools-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyter-analysis-tools-0.1.6.dev5.tar", last modified: Thu Apr 20 13:42:34 2023, max compression
+gzip compressed data, was "jupyter-analysis-tools-0.1.7.tar", last modified: Tue Apr  2 12:04:41 2024, max compression
```

## Comparing `jupyter-analysis-tools-0.1.6.dev5.tar` & `jupyter-analysis-tools-0.1.7.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:42:34.329642 jupyter-analysis-tools-0.1.6.dev5/
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-20 13:42:23.000000 jupyter-analysis-tools-0.1.6.dev5/.cookiecutterrc
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-04-20 13:42:34.329642 jupyter-analysis-tools-0.1.6.dev5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-04-20 13:42:23.000000 jupyter-analysis-tools-0.1.6.dev5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:42:34.321642 jupyter-analysis-tools-0.1.6.dev5/ci/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/ci/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:42:34.313642 jupyter-analysis-tools-0.1.6.dev5/ci/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:42:34.317642 jupyter-analysis-tools-0.1.6.dev5/ci/templates/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:42:34.321642 jupyter-analysis-tools-0.1.6.dev5/ci/templates/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/ci/templates/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/ci/templates/.github/workflows/ci-cd.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/ci/templates/.github/workflows/coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/ci/templates/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/ci/templates/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/ci/templates/.github/workflows/tests.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)     4495 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/ci/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:42:34.325642 jupyter-analysis-tools-0.1.6.dev5/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:42:34.325642 jupyter-analysis-tools-0.1.6.dev5/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/docs/_templates/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/docs/_templates/module.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-04-20 13:42:23.000000 jupyter-analysis-tools-0.1.6.dev5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/docs/readme.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:42:34.325642 jupyter-analysis-tools-0.1.6.dev5/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/docs/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/docs/spelling_wordlist.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 13:42:34.329642 jupyter-analysis-tools-0.1.6.dev5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:42:34.317642 jupyter-analysis-tools-0.1.6.dev5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:42:34.329642 jupyter-analysis-tools-0.1.6.dev5/src/jupyter_analysis_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-20 13:42:23.000000 jupyter-analysis-tools-0.1.6.dev5/src/jupyter_analysis_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/src/jupyter_analysis_tools/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    14557 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/src/jupyter_analysis_tools/binning.py
--rw-r--r--   0 runner    (1001) docker     (123)     4322 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/src/jupyter_analysis_tools/datalocations.py
--rw-r--r--   0 runner    (1001) docker     (123)    16254 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/src/jupyter_analysis_tools/distrib.py
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/src/jupyter_analysis_tools/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/src/jupyter_analysis_tools/notebook_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/src/jupyter_analysis_tools/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/src/jupyter_analysis_tools/readdata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4402 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/src/jupyter_analysis_tools/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/src/jupyter_analysis_tools/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:42:34.329642 jupyter-analysis-tools-0.1.6.dev5/src/jupyter_analysis_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-04-20 13:42:34.000000 jupyter-analysis-tools-0.1.6.dev5/src/jupyter_analysis_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-04-20 13:42:34.000000 jupyter-analysis-tools-0.1.6.dev5/src/jupyter_analysis_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 13:42:34.000000 jupyter-analysis-tools-0.1.6.dev5/src/jupyter_analysis_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-20 13:42:34.000000 jupyter-analysis-tools-0.1.6.dev5/src/jupyter_analysis_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 13:42:34.329642 jupyter-analysis-tools-0.1.6.dev5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/tests/test_jupyter_analysis_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-04-20 13:42:05.000000 jupyter-analysis-tools-0.1.6.dev5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:04:41.625085 jupyter-analysis-tools-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-02 12:04:23.000000 jupyter-analysis-tools-0.1.7/.cookiecutterrc
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-02 12:04:23.000000 jupyter-analysis-tools-0.1.7/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-02 12:04:23.000000 jupyter-analysis-tools-0.1.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-02 12:04:23.000000 jupyter-analysis-tools-0.1.7/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    28944 2024-04-02 12:04:23.000000 jupyter-analysis-tools-0.1.7/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-04-02 12:04:23.000000 jupyter-analysis-tools-0.1.7/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-02 12:04:23.000000 jupyter-analysis-tools-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-02 12:04:23.000000 jupyter-analysis-tools-0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    33004 2024-04-02 12:04:41.625085 jupyter-analysis-tools-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-04-02 12:04:23.000000 jupyter-analysis-tools-0.1.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:04:41.617085 jupyter-analysis-tools-0.1.7/ci/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-02 12:04:23.000000 jupyter-analysis-tools-0.1.7/ci/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:04:41.613085 jupyter-analysis-tools-0.1.7/ci/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:04:41.613085 jupyter-analysis-tools-0.1.7/ci/templates/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:04:41.621085 jupyter-analysis-tools-0.1.7/ci/templates/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-02 12:04:23.000000 jupyter-analysis-tools-0.1.7/ci/templates/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-02 12:04:23.000000 jupyter-analysis-tools-0.1.7/ci/templates/.github/workflows/ci-cd.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4570 2024-04-02 12:04:23.000000 jupyter-analysis-tools-0.1.7/ci/templates/.github/workflows/coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-02 12:04:23.000000 jupyter-analysis-tools-0.1.7/ci/templates/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-02 12:04:23.000000 jupyter-analysis-tools-0.1.7/ci/templates/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-04-02 12:04:23.000000 jupyter-analysis-tools-0.1.7/ci/templates/.github/workflows/tests.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4495 2024-04-02 12:04:23.000000 jupyter-analysis-tools-0.1.7/ci/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:04:41.621085 jupyter-analysis-tools-0.1.7/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:04:41.621085 jupyter-analysis-tools-0.1.7/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-02 12:04:23.000000 jupyter-analysis-tools-0.1.7/docs/_templates/class.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-02 12:04:23.000000 jupyter-analysis-tools-0.1.7/docs/_templates/module.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-02 12:04:23.000000 jupyter-analysis-tools-0.1.7/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-02 12:04:23.000000 jupyter-analysis-tools-0.1.7/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-04-02 12:04:23.000000 jupyter-analysis-tools-0.1.7/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-02 12:04:23.000000 jupyter-analysis-tools-0.1.7/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-02 12:04:23.000000 jupyter-analysis-tools-0.1.7/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-02 12:04:23.000000 jupyter-analysis-tools-0.1.7/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-02 12:04:23.000000 jupyter-analysis-tools-0.1.7/docs/readme.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:04:41.621085 jupyter-analysis-tools-0.1.7/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-02 12:04:23.000000 jupyter-analysis-tools-0.1.7/docs/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-02 12:04:23.000000 jupyter-analysis-tools-0.1.7/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-02 12:04:23.000000 jupyter-analysis-tools-0.1.7/docs/spelling_wordlist.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-02 12:04:23.000000 jupyter-analysis-tools-0.1.7/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-04-02 12:04:23.000000 jupyter-analysis-tools-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 12:04:41.625085 jupyter-analysis-tools-0.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:04:41.617085 jupyter-analysis-tools-0.1.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:04:41.625085 jupyter-analysis-tools-0.1.7/src/jupyter_analysis_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-02 12:04:23.000000 jupyter-analysis-tools-0.1.7/src/jupyter_analysis_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-04-02 12:04:23.000000 jupyter-analysis-tools-0.1.7/src/jupyter_analysis_tools/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14557 2024-04-02 12:04:23.000000 jupyter-analysis-tools-0.1.7/src/jupyter_analysis_tools/binning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4322 2024-04-02 12:04:23.000000 jupyter-analysis-tools-0.1.7/src/jupyter_analysis_tools/datalocations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16417 2024-04-02 12:04:23.000000 jupyter-analysis-tools-0.1.7/src/jupyter_analysis_tools/distrib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-04-02 12:04:23.000000 jupyter-analysis-tools-0.1.7/src/jupyter_analysis_tools/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-02 12:04:23.000000 jupyter-analysis-tools-0.1.7/src/jupyter_analysis_tools/notebook_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-02 12:04:23.000000 jupyter-analysis-tools-0.1.7/src/jupyter_analysis_tools/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-02 12:04:23.000000 jupyter-analysis-tools-0.1.7/src/jupyter_analysis_tools/readdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4402 2024-04-02 12:04:23.000000 jupyter-analysis-tools-0.1.7/src/jupyter_analysis_tools/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-04-02 12:04:23.000000 jupyter-analysis-tools-0.1.7/src/jupyter_analysis_tools/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:04:41.625085 jupyter-analysis-tools-0.1.7/src/jupyter_analysis_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    33004 2024-04-02 12:04:41.000000 jupyter-analysis-tools-0.1.7/src/jupyter_analysis_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-02 12:04:41.000000 jupyter-analysis-tools-0.1.7/src/jupyter_analysis_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 12:04:41.000000 jupyter-analysis-tools-0.1.7/src/jupyter_analysis_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-02 12:04:41.000000 jupyter-analysis-tools-0.1.7/src/jupyter_analysis_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:04:41.625085 jupyter-analysis-tools-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-02 12:04:23.000000 jupyter-analysis-tools-0.1.7/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-02 12:04:23.000000 jupyter-analysis-tools-0.1.7/tests/test_jupyter_analysis_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-04-02 12:04:23.000000 jupyter-analysis-tools-0.1.7/tox.ini
```

### Comparing `jupyter-analysis-tools-0.1.6.dev5/.cookiecutterrc` & `jupyter-analysis-tools-0.1.7/.cookiecutterrc`

 * *Files 8% similar despite different names*

```diff
@@ -16,12 +16,12 @@
     repo_main_branch:          'main'
     package_name:              'jupyter_analysis_tools'
     distribution_name:         'jupyter-analysis-tools'
     project_short_description: 'Yet another Python library with helpers and utilities for data analysis and processing.'
     release_date:              'today'
     year_from:                 '2018'
     year_to:                   '2023'
-    version:                   '0.1.6-dev.5'
+    version:                   '0.1.7'
     pypi_host:                 'pypi.org'
     license:                   'MIT license'
     sphinx_theme:              'furo'
     extra_context:             {'exclude_existing': "['AUTHORS.rst', 'CHANGELOG.md', 'src/jupyter_analysis_tools/__init__.py']"}
```

### Comparing `jupyter-analysis-tools-0.1.6.dev5/.pre-commit-config.yaml` & `jupyter-analysis-tools-0.1.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `jupyter-analysis-tools-0.1.6.dev5/CONTRIBUTING.rst` & `jupyter-analysis-tools-0.1.7/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `jupyter-analysis-tools-0.1.6.dev5/LICENSE` & `jupyter-analysis-tools-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter-analysis-tools-0.1.6.dev5/README.rst` & `jupyter-analysis-tools-0.1.7/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 | |supported-versions| |wheel| |downloads|
 | |cicd| |coverage|
 
 .. |version| image:: https://img.shields.io/pypi/v/jupyter-analysis-tools.svg
     :target: https://pypi.org/project/jupyter-analysis-tools
     :alt: PyPI Package latest release
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/BAMresearch/jupyter-analysis-tools/v0.1.6-dev.5.svg
-    :target: https://github.com/BAMresearch/jupyter-analysis-tools/compare/v0.1.6-dev.5...main
+.. |commits-since| image:: https://img.shields.io/github/commits-since/BAMresearch/jupyter-analysis-tools/v0.1.7.svg
+    :target: https://github.com/BAMresearch/jupyter-analysis-tools/compare/v0.1.7...main
     :alt: Commits since latest release
 
 .. |license| image:: https://img.shields.io/pypi/l/jupyter-analysis-tools.svg
     :target: https://en.wikipedia.org/wiki/MIT_license
     :alt: License
 
 .. |supported-versions| image:: https://img.shields.io/pypi/pyversions/jupyter-analysis-tools.svg
```

### Comparing `jupyter-analysis-tools-0.1.6.dev5/ci/templates/.github/workflows/build.yml` & `jupyter-analysis-tools-0.1.7/ci/templates/.github/workflows/build.yml`

 * *Files 20% similar despite different names*

```diff
@@ -17,49 +17,43 @@
 
       {{ ci.checkout() }}
 
       {{ ci.setup_python() }}
 
       {{ ci.pip_install_req() }}
 
-      {{ ci.set_version() }}
-
       - name: Build
         run: tox -e build -v
 
-      - name: Upload package artifact for publishing job
-        uses: actions/upload-artifact@v3
-        with:
-          name: packages
-          path: dist/*.whl
-
-      - name: Upload source artifact for publishing job
-        # upload source package only once
-        if: {{"${{ matrix.os == 'ubuntu-latest' }}"}}
-        uses: actions/upload-artifact@v3
+      - name: Upload packages for publishing job
+        uses: actions/upload-artifact@v4
         with:
-          name: packages
-          path: dist/*.tar.gz
+          name: {{"packages-${{ matrix.os }}"}}
+          path: |
+              dist/*.whl
+              dist/*.tar.gz
 
   publish:
     needs: [build]
     runs-on: 'ubuntu-latest'
     steps:
 
       {{ ci.checkout() }}
 
       {{ ci.pip_install_req() }}
 
       - name: Download package artifacts
-        uses: actions/download-artifact@v3
+        uses: actions/download-artifact@v4
         with:
-          name: packages
+          pattern: packages-*
+          merge-multiple: true
           path: dist
 
       - name: Check generated packages
         run: twine check dist/*.*
 
       - name: Upload packages
         env:
           TWINE_PASSWORD: {{'"${{ secrets.'+pypi_token+' }}"'}}
+          TWINE_NON_INTERACTIVE: 1
         run: |
-          twine upload -u __token__ -r {{ pypi_repo }} dist/*.*
+          twine upload --disable-progress-bar --skip-existing -u __token__ -r {{ pypi_repo }} dist/*.*
```

### Comparing `jupyter-analysis-tools-0.1.6.dev5/ci/templates/.github/workflows/ci-cd.yml` & `jupyter-analysis-tools-0.1.7/ci/templates/.github/workflows/ci-cd.yml`

 * *Files 20% similar despite different names*

```diff
@@ -34,25 +34,25 @@
     needs: [tests, docs]  # coverage report is added to the docs webpage
     uses: ./.github/workflows/coverage.yml
 
 {#- Some Jinja macros for reusing recurring workflow job steps -#}
 
 {%- macro checkout(depth=1) -%}
       - name: Checking out the repo
-        uses: actions/checkout@v3
+        uses: actions/checkout@v4
         {%- if depth != 1 +%}
         with:
           fetch-depth: {{ depth }}
         {%- endif -%}
 {%- endmacro -%}
 
 {%- macro setup_python(arch, py=py_ver, req=['ci/requirements.txt']) -%}
       # see *py_ver* in ci/update.py
       - name: Setting up Python {{ py }}
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: '{{ py }}'
           {% if arch %}
           architecture: '{{ arch }}'
           {% endif %}
           cache: pip
           cache-dependency-path: |
@@ -62,27 +62,8 @@
 {%- endmacro -%}
 
 {% macro pip_install_req() -%}
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           python -m pip install --progress-bar=off -r ci/requirements.txt
-{%- endmacro -%}
-
-{% macro set_version() -%}
-      - name: Get latest tags
-        run: |
-          git pull --tags
-          echo "git_tag_head='$(git tag --points-at HEAD)'" >> $GITHUB_ENV
-          echo "git_tag_head='$(git tag --points-at HEAD)'"
-
-      - name: Set version number
-        # modify source files to reflect the current version
-        # (relevant for pre-releases indicated by tag only)
-        # Does not modify the git history
-        if: {{"${{ env.git_tag_head }}"}}  # there is a tag at the latest commit
-        shell: python
-        run: |
-          from semantic_release.history import set_new_version, get_current_version
-          cv = get_current_version()
-          print(f"Setting current version '{cv}':", set_new_version(cv))
 {%- endmacro +%}
```

### Comparing `jupyter-analysis-tools-0.1.6.dev5/ci/templates/.github/workflows/coverage.yml` & `jupyter-analysis-tools-0.1.7/ci/templates/.github/workflows/coverage.yml`

 * *Files 2% similar despite different names*

```diff
@@ -21,29 +21,29 @@
       {{ ci.checkout() }}
 
       {{ ci.setup_python() }}
 
       {{ ci.pip_install_req() }}
 
       - name: Download coverage data
-        uses: actions/download-artifact@v3
+        uses: actions/download-artifact@v4
         with:
           name: coverage
 
       - name: Combine and report
         id: combine
         run: |
           set -x
           pwd && ls -la
           coverage combine coverage.*
           python3 -c 'import coverage,pprint; cov=coverage.Coverage(); cov.load();pprint.pprint(list(cov.get_data()._file_map.keys()))'
           coverage html --debug=pathmap
 
       - name: Upload HTML report
-        uses: actions/upload-artifact@v3
+        uses: actions/upload-artifact@v4
         with:
           name: html_report
           path: htmlcov
 
       - name: Get total
         id: total
         run: |
@@ -71,32 +71,32 @@
 
       - name: Summarize
         run: |
           echo '### Total coverage: {{'${{ env.total }}'}}%' >> $GITHUB_STEP_SUMMARY
 
       - name: Checkout documentation pages branch
         if: {{"${{ github.ref == 'refs/heads/main' }}"}}
-        uses: actions/checkout@v3
+        uses: actions/checkout@v4
         with:
           ref: gh-pages
           path: pages
 
       - name: Purge old documentation files
         run: cd pages && git rm -rf . || true
 
       - name: Download previously generated documentation
         if: {{"${{ github.ref == 'refs/heads/main' }}"}}
-        uses: actions/download-artifact@v3
+        uses: actions/download-artifact@v4
         with:
           name: docs
           path: pages
 
       - name: Download coverage HTML report
         if: {{"${{ github.ref == 'refs/heads/main' }}"}}
-        uses: actions/download-artifact@v3
+        uses: actions/download-artifact@v4
         with:
           name: html_report
           path: {{"pages/${{ env.report_dir }}"}}
 
       - name: Push to report repo
         if: {{"${{ github.ref == 'refs/heads/main' }}"}}
         env:
```

#### html2text {}

```diff
@@ -1,35 +1,35 @@
 name: Coverage # Controls when the action will run. on: workflow_call: {%
 import '.github/workflows/ci-cd.yml' as ci with context %}{# Use some Jinja
 macros -#} env: DOCS_URL: {{ docs_url }} COV_REPORT_BASE_DIR: {
 { cov_report_path }} jobs: combine: name: Combine coverage data runs-on:
 ubuntu-latest outputs: total: {{ '${{ steps.total.outputs.total }}' }} steps: {
 { ci.checkout() }} {{ ci.setup_python() }} {{ ci.pip_install_req() }} - name:
-Download coverage data uses: actions/download-artifact@v3 with: name: coverage
+Download coverage data uses: actions/download-artifact@v4 with: name: coverage
 - name: Combine and report id: combine run: | set -x pwd && ls -la coverage
 combine coverage.* python3 -c 'import coverage,pprint; cov=coverage.Coverage();
 cov.load();pprint.pprint(list(cov.get_data()._file_map.keys()))' coverage html
---debug=pathmap - name: Upload HTML report uses: actions/upload-artifact@v3
+--debug=pathmap - name: Upload HTML report uses: actions/upload-artifact@v4
 with: name: html_report path: htmlcov - name: Get total id: total run: | echo
 "total=$(coverage report --format=total)" >> $GITHUB_OUTPUT publish: name:
 Publish coverage report needs: combine runs-on: ubuntu-latest steps: - name:
 Compute info for later steps id: info run: | set -xe export SHA10=$(echo {{ '${
 { github.sha }}' }} | cut -c 1-10) export SLUG=$(date +'%Y%m%d')_$SHA10 export
 REPORT_DIR=$COV_REPORT_BASE_DIR/$SLUG export REF={{'"${{ github.ref }}"'}} echo
 "total={{'${{ needs.combine.outputs.total }}'}}" >> $GITHUB_ENV echo
 "sha10=$SHA10" >> $GITHUB_ENV echo "slug=$SLUG" >> $GITHUB_ENV echo
 "report_dir=$REPORT_DIR" >> $GITHUB_ENV echo "branch=${REF#refs/heads/}" >>
 $GITHUB_ENV - name: Summarize run: | echo '### Total coverage: {{'${{ env.total
 }}'}}%' >> $GITHUB_STEP_SUMMARY - name: Checkout documentation pages branch if:
-{{"${{ github.ref == 'refs/heads/main' }}"}} uses: actions/checkout@v3 with:
+{{"${{ github.ref == 'refs/heads/main' }}"}} uses: actions/checkout@v4 with:
 ref: gh-pages path: pages - name: Purge old documentation files run: cd pages
 && git rm -rf . || true - name: Download previously generated documentation if:
-{{"${{ github.ref == 'refs/heads/main' }}"}} uses: actions/download-artifact@v3
+{{"${{ github.ref == 'refs/heads/main' }}"}} uses: actions/download-artifact@v4
 with: name: docs path: pages - name: Download coverage HTML report if: {{"${
-{ github.ref == 'refs/heads/main' }}"}} uses: actions/download-artifact@v3
+{ github.ref == 'refs/heads/main' }}"}} uses: actions/download-artifact@v4
 with: name: html_report path: {{"pages/${{ env.report_dir }}"}} - name: Push to
 report repo if: {{"${{ github.ref == 'refs/heads/main' }}"}} env:
 COMMIT_MESSAGE: {{'${{ github.event.head_commit.message }}'}} REDIR_HTML: {
 {'"pages/${{ env.COV_REPORT_BASE_DIR }}/index.html"'}} BADGE_JSON: {{'"pages/${
 { env.COV_REPORT_BASE_DIR }}/cov.json"'}} REPORT_URL: {{'"${{ env.DOCS_URL }}/$
 {{ env.report_dir }}"'}} run: | set -xe # Make the redirect to the latest
 report. echo "
```

### Comparing `jupyter-analysis-tools-0.1.6.dev5/ci/templates/.github/workflows/docs.yml` & `jupyter-analysis-tools-0.1.7/ci/templates/.github/workflows/docs.yml`

 * *Files 16% similar despite different names*

```diff
@@ -14,24 +14,22 @@
 
       {{ ci.checkout(depth=0) }}
 
       {{ ci.setup_python() }}
 
       {{ ci.pip_install_req() }}
 
-      {{ ci.set_version() }}
-
       - name: Check
         run: tox -e check -v
 
       - name: Generate documentation
         run: tox -e docs -v
 
       - name: Upload docs for finalization later
-        uses: actions/upload-artifact@v3
+        uses: actions/upload-artifact@v4
         with:
           name: docs
           path: dist/docs
 
       # - name: Upload generated documentation
       #   uses: peaceiris/actions-gh-pages@v3
       #   with:
```

### Comparing `jupyter-analysis-tools-0.1.6.dev5/ci/templates/.github/workflows/release.yml` & `jupyter-analysis-tools-0.1.7/ci/templates/.github/workflows/release.yml`

 * *Files 26% similar despite different names*

```diff
@@ -22,19 +22,18 @@
           git config user.email "${GITHUB_ACTOR}@users.noreply.github.com"
 
       {{ ci.setup_python() }}
 
       {{ ci.pip_install_req() }}
 
       - name: Determine a version number
+        env:
+          GH_TOKEN: {{'${{ secrets.GITHUB_TOKEN }}'}}
         shell: sh
         run: |
           set -x
+          NEWVER=$(semantic-release version --print)
+          sed -i -e "s/v\([0-9]\+\.\)\{3\}/v$NEWVER./" README.rst
+          sed -i -e "s/\([0-9]\+\.\)\{2\}[0-9]\+/$NEWVER/" .cookiecutterrc
+          git add README.rst .cookiecutterrc
           # creates a release only if there are relevant changes/commits starting with 'fix/feat()'
-          semantic-release publish -D version_source=commit \
-            -D commit_author="${GITHUB_ACTOR} <${GITHUB_ACTOR}@users.noreply.github.com>"
-          if [ -z "$(git tag --points-at HEAD)" ]; then
-            # no release, no relevant changes, make prerelease tag
-            semantic-release version -D version_source=tag --prerelease
-          fi
-          git push
-          git push --tags
+          semantic-release version
```

### Comparing `jupyter-analysis-tools-0.1.6.dev5/ci/templates/.github/workflows/tests.yml` & `jupyter-analysis-tools-0.1.7/ci/templates/.github/workflows/tests.yml`

 * *Files 1% similar despite different names*

```diff
@@ -48,11 +48,11 @@
       - name: Run tests
         run: tox -e {{'${{ env.TOX_ENV }}'}} -v
 
       - name: Rename coverage data uniquely
         run: {{ 'mv .coverage coverage.${{ env.TOX_ENV }}.${{ matrix.os }}' }}
 
       - name: Upload coverage data for next step
-        uses: actions/upload-artifact@v3
+        uses: actions/upload-artifact@v4
         with:
           name: coverage
           path: coverage.*
```

### Comparing `jupyter-analysis-tools-0.1.6.dev5/ci/update.py` & `jupyter-analysis-tools-0.1.7/ci/update.py`

 * *Files identical despite different names*

### Comparing `jupyter-analysis-tools-0.1.6.dev5/docs/_templates/class.rst` & `jupyter-analysis-tools-0.1.7/docs/_templates/class.rst`

 * *Files identical despite different names*

### Comparing `jupyter-analysis-tools-0.1.6.dev5/docs/_templates/module.rst` & `jupyter-analysis-tools-0.1.7/docs/_templates/module.rst`

 * *Files identical despite different names*

### Comparing `jupyter-analysis-tools-0.1.6.dev5/docs/conf.py` & `jupyter-analysis-tools-0.1.7/docs/conf.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 templates_path = ["_templates"]
 source_suffix = ".rst"
 master_doc = "index"
 project = "Jupyter Analysis Tools"
 year = "2018-2023"
 author = "Ingo Breßler"
 copyright = "{0}, {1}".format(year, author)
-version = "0.1.6-dev.5"
+version = "0.1.7"
 release = version
 commit_id = None
 try:
     commit_id = (
         subprocess.check_output(["git", "rev-parse", "--short", "HEAD"]).strip().decode("ascii")
     )
 except subprocess.CalledProcessError as e:
@@ -73,8 +73,11 @@
 
 linkcheck_ignore = [
     join(
         project_meta["project"]["urls"]["documentation"],
         project_meta["tool"]["coverage"]["report"]["path"],
     )
     + r".*",
+    # attempted fix of '406 Client Error: Not Acceptable for url'
+    # https://github.com/sphinx-doc/sphinx/issues/1331
+    join(project_meta["project"]["urls"]["repository"], "commit", r"[0-9a-fA-F]+")
 ]
```

### Comparing `jupyter-analysis-tools-0.1.6.dev5/pyproject.toml` & `jupyter-analysis-tools-0.1.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -52,32 +52,26 @@
 [tool.coverage.report]
 path = "coverage-report"
 
 # on version numbers: https://peps.python.org/pep-0440/
 # and bottom of https://softwareengineering.stackexchange.com/a/151558
 [tool.semantic_release]
 #major_on_zero = false # no major release when current major version is zero
-version_variable = [                        # version location
+version_variables = [                        # version location
     "src/jupyter_analysis_tools/__init__.py:__version__",
     "docs/conf.py:version",
 ]
-version_pattern = [
-    "README.rst:v{version}.svg",
-    "README.rst:v{version}...main",
-    ".cookiecutterrc:version:                   '{version}'",
-]
-version_source = "tag"
-prerelease_tag = "dev"
-branch = "main"                             # branch to make releases of
-changelog_file = "CHANGELOG.md"             # changelog file
-build_command = "python3 -m build"          # build dists
-upload_to_release = false                   # auto-create GitHub release
-upload_to_pypi = false                      # don't auto-upload to PyPI
-remove_dist = false                         # don't remove dists
-#patch_without_tag = false                   # patch release by default
+[tool.semantic_release.commit_parser_options]
+allowed_tags = ["build", "chore", "ci", "docs", "feat", "fix", "perf", "style", "refactor", "test"]
+minor_tags = ["feat"]
+patch_tags = ["fix", "perf"]
+[tool.semantic_release.changelog]
+exclude_commit_patterns = ["chore", ".*\\bGHA\\b.*", ".*\\b[gG][hH] actions?\\b.*"]
+[tool.semantic_release.publish]
+upload_to_vcs_release = false
 
 [tool.black]
 line-length = 100
 preview = true
 
 [tool.isort]
 profile = "black"
```

### Comparing `jupyter-analysis-tools-0.1.6.dev5/src/jupyter_analysis_tools/analysis.py` & `jupyter-analysis-tools-0.1.7/src/jupyter_analysis_tools/analysis.py`

 * *Files identical despite different names*

### Comparing `jupyter-analysis-tools-0.1.6.dev5/src/jupyter_analysis_tools/binning.py` & `jupyter-analysis-tools-0.1.7/src/jupyter_analysis_tools/binning.py`

 * *Files identical despite different names*

### Comparing `jupyter-analysis-tools-0.1.6.dev5/src/jupyter_analysis_tools/datalocations.py` & `jupyter-analysis-tools-0.1.7/src/jupyter_analysis_tools/datalocations.py`

 * *Files identical despite different names*

### Comparing `jupyter-analysis-tools-0.1.6.dev5/src/jupyter_analysis_tools/distrib.py` & `jupyter-analysis-tools-0.1.7/src/jupyter_analysis_tools/distrib.py`

 * *Files 0% similar despite different names*

```diff
@@ -286,16 +286,19 @@
             lw=0,
             alpha=0.1,
             label=f"uncertainties (lvl: {self.uncertRatioMedian(peakRange):.3g})",
         )
         if showFullRange:
             ax.set_xlim((self.x.min(), self.x.max()))
         ax.set_xlabel(self.xlabel)
-        ax.legend(prop=font_manager.FontProperties(family="monospace"))
         ax.grid(True)
+        legend = ax.legend(prop=font_manager.FontProperties(family="monospace"))
+        # make the legend background more transparent
+        legend.get_frame().set_alpha(None)
+        legend.get_frame().set_facecolor((1, 1, 1, 0.2))
 
     def plot(self, ax, distPar, name=""):
         """plot complete distribution as loaded from file"""
         lbl = (
             "from file, "
             + name
             + area(self.x, self.y, showArea=True)
```

### Comparing `jupyter-analysis-tools-0.1.6.dev5/src/jupyter_analysis_tools/git.py` & `jupyter-analysis-tools-0.1.7/src/jupyter_analysis_tools/git.py`

 * *Files identical despite different names*

### Comparing `jupyter-analysis-tools-0.1.6.dev5/src/jupyter_analysis_tools/notebook_utils.py` & `jupyter-analysis-tools-0.1.7/src/jupyter_analysis_tools/notebook_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,19 @@
 # notebook_utils.py
 
 import json
 import os
 import urllib
 
 import ipykernel
-from notebook import notebookapp
+
+try:
+    from notebook import notebookapp
+except ImportError:
+    from notebook import app as notebookapp
 
 
 def currentNBpath():
     """Returns the absolute path of the Notebook or None if it cannot be determined
     NOTE: works only for *Jupyter Notebook* (not Jupyter Lab)
     and when the security is token-based or there is also no password.
     """
```

### Comparing `jupyter-analysis-tools-0.1.6.dev5/src/jupyter_analysis_tools/plotting.py` & `jupyter-analysis-tools-0.1.7/src/jupyter_analysis_tools/plotting.py`

 * *Files identical despite different names*

### Comparing `jupyter-analysis-tools-0.1.6.dev5/src/jupyter_analysis_tools/readdata.py` & `jupyter-analysis-tools-0.1.7/src/jupyter_analysis_tools/readdata.py`

 * *Files identical despite different names*

### Comparing `jupyter-analysis-tools-0.1.6.dev5/src/jupyter_analysis_tools/utils.py` & `jupyter-analysis-tools-0.1.7/src/jupyter_analysis_tools/utils.py`

 * *Files identical despite different names*

### Comparing `jupyter-analysis-tools-0.1.6.dev5/src/jupyter_analysis_tools/widgets.py` & `jupyter-analysis-tools-0.1.7/src/jupyter_analysis_tools/widgets.py`

 * *Files identical despite different names*

### Comparing `jupyter-analysis-tools-0.1.6.dev5/src/jupyter_analysis_tools.egg-info/SOURCES.txt` & `jupyter-analysis-tools-0.1.7/src/jupyter_analysis_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jupyter-analysis-tools-0.1.6.dev5/tox.ini` & `jupyter-analysis-tools-0.1.7/tox.ini`

 * *Files identical despite different names*

