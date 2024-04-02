# Comparing `tmp/aind_exaspim_pipeline_utils-0.7.2.tar.gz` & `tmp/aind_exaspim_pipeline_utils-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aind_exaspim_pipeline_utils-0.7.2.tar", last modified: Tue Feb  6 18:25:25 2024, max compression
+gzip compressed data, was "aind_exaspim_pipeline_utils-0.8.0.tar", last modified: Tue Apr  2 18:15:48 2024, max compression
```

## Comparing `aind_exaspim_pipeline_utils-0.7.2.tar` & `aind_exaspim_pipeline_utils-0.8.0.tar`

### file list

```diff
@@ -1,64 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:25:25.738944 aind_exaspim_pipeline_utils-0.7.2/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-02-06 18:25:10.000000 aind_exaspim_pipeline_utils-0.7.2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:25:25.722945 aind_exaspim_pipeline_utils-0.7.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:25:25.726945 aind_exaspim_pipeline_utils-0.7.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-02-06 18:25:10.000000 aind_exaspim_pipeline_utils-0.7.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-02-06 18:25:10.000000 aind_exaspim_pipeline_utils-0.7.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-02-06 18:25:10.000000 aind_exaspim_pipeline_utils-0.7.2/.github/ISSUE_TEMPLATE/user-story.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:25:25.726945 aind_exaspim_pipeline_utils-0.7.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-02-06 18:25:10.000000 aind_exaspim_pipeline_utils-0.7.2/.github/workflows/lint_and_test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-02-06 18:25:10.000000 aind_exaspim_pipeline_utils-0.7.2/.github/workflows/tag_and_publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-02-06 18:25:10.000000 aind_exaspim_pipeline_utils-0.7.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-02-06 18:25:10.000000 aind_exaspim_pipeline_utils-0.7.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-02-06 18:25:10.000000 aind_exaspim_pipeline_utils-0.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4946 2024-02-06 18:25:25.734944 aind_exaspim_pipeline_utils-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-02-06 18:25:10.000000 aind_exaspim_pipeline_utils-0.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:25:25.726945 aind_exaspim_pipeline_utils-0.7.2/capsule_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-02-06 18:25:10.000000 aind_exaspim_pipeline_utils-0.7.2/capsule_scripts/imagej_postInstall
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-06 18:25:10.000000 aind_exaspim_pipeline_utils-0.7.2/capsule_scripts/imagej_run.sh
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-02-06 18:25:10.000000 aind_exaspim_pipeline_utils-0.7.2/capsule_scripts/n5tozarr_postInstall
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-06 18:25:10.000000 aind_exaspim_pipeline_utils-0.7.2/capsule_scripts/n5tozarr_run.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:25:25.726945 aind_exaspim_pipeline_utils-0.7.2/doc/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-02-06 18:25:10.000000 aind_exaspim_pipeline_utils-0.7.2/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-02-06 18:25:10.000000 aind_exaspim_pipeline_utils-0.7.2/doc/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:25:25.726945 aind_exaspim_pipeline_utils-0.7.2/doc/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:25:25.730944 aind_exaspim_pipeline_utils-0.7.2/doc/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-02-06 18:25:10.000000 aind_exaspim_pipeline_utils-0.7.2/doc/source/_static/dark-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-02-06 18:25:10.000000 aind_exaspim_pipeline_utils-0.7.2/doc/source/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-02-06 18:25:10.000000 aind_exaspim_pipeline_utils-0.7.2/doc/source/_static/light-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-02-06 18:25:10.000000 aind_exaspim_pipeline_utils-0.7.2/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-02-06 18:25:10.000000 aind_exaspim_pipeline_utils-0.7.2/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-02-06 18:25:10.000000 aind_exaspim_pipeline_utils-0.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-06 18:25:25.738944 aind_exaspim_pipeline_utils-0.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-06 18:25:10.000000 aind_exaspim_pipeline_utils-0.7.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:25:25.722945 aind_exaspim_pipeline_utils-0.7.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:25:25.730944 aind_exaspim_pipeline_utils-0.7.2/src/aind_exaspim_pipeline_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-06 18:25:11.000000 aind_exaspim_pipeline_utils-0.7.2/src/aind_exaspim_pipeline_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14652 2024-02-06 18:25:10.000000 aind_exaspim_pipeline_utils-0.7.2/src/aind_exaspim_pipeline_utils/exaspim_manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     7057 2024-02-06 18:25:10.000000 aind_exaspim_pipeline_utils-0.7.2/src/aind_exaspim_pipeline_utils/imagej_macros.py
--rw-r--r--   0 runner    (1001) docker     (127)    23657 2024-02-06 18:25:10.000000 aind_exaspim_pipeline_utils-0.7.2/src/aind_exaspim_pipeline_utils/imagej_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:25:25.730944 aind_exaspim_pipeline_utils-0.7.2/src/aind_exaspim_pipeline_utils/n5tozarr/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-06 18:25:10.000000 aind_exaspim_pipeline_utils-0.7.2/src/aind_exaspim_pipeline_utils/n5tozarr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18825 2024-02-06 18:25:10.000000 aind_exaspim_pipeline_utils-0.7.2/src/aind_exaspim_pipeline_utils/n5tozarr/n5tozarr_da.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:25:25.730944 aind_exaspim_pipeline_utils-0.7.2/src/aind_exaspim_pipeline_utils/qc/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-06 18:25:10.000000 aind_exaspim_pipeline_utils-0.7.2/src/aind_exaspim_pipeline_utils/qc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-02-06 18:25:10.000000 aind_exaspim_pipeline_utils-0.7.2/src/aind_exaspim_pipeline_utils/qc/bigstitcher_log_edge_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-02-06 18:25:10.000000 aind_exaspim_pipeline_utils-0.7.2/src/aind_exaspim_pipeline_utils/qc/create_ng_link.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:25:25.734944 aind_exaspim_pipeline_utils-0.7.2/src/aind_exaspim_pipeline_utils/trigger/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-06 18:25:10.000000 aind_exaspim_pipeline_utils-0.7.2/src/aind_exaspim_pipeline_utils/trigger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26980 2024-02-06 18:25:10.000000 aind_exaspim_pipeline_utils-0.7.2/src/aind_exaspim_pipeline_utils/trigger/capsule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:25:25.734944 aind_exaspim_pipeline_utils-0.7.2/src/aind_exaspim_pipeline_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4946 2024-02-06 18:25:25.000000 aind_exaspim_pipeline_utils-0.7.2/src/aind_exaspim_pipeline_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-02-06 18:25:25.000000 aind_exaspim_pipeline_utils-0.7.2/src/aind_exaspim_pipeline_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-06 18:25:25.000000 aind_exaspim_pipeline_utils-0.7.2/src/aind_exaspim_pipeline_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-02-06 18:25:25.000000 aind_exaspim_pipeline_utils-0.7.2/src/aind_exaspim_pipeline_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-02-06 18:25:25.000000 aind_exaspim_pipeline_utils-0.7.2/src/aind_exaspim_pipeline_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-06 18:25:25.000000 aind_exaspim_pipeline_utils-0.7.2/src/aind_exaspim_pipeline_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:25:25.734944 aind_exaspim_pipeline_utils-0.7.2/src/aind_trigger_codeocean/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-06 18:25:10.000000 aind_exaspim_pipeline_utils-0.7.2/src/aind_trigger_codeocean/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    51638 2024-02-06 18:25:10.000000 aind_exaspim_pipeline_utils-0.7.2/src/aind_trigger_codeocean/pipelines.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:25:25.734944 aind_exaspim_pipeline_utils-0.7.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-06 18:25:10.000000 aind_exaspim_pipeline_utils-0.7.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-02-06 18:25:10.000000 aind_exaspim_pipeline_utils-0.7.2/tests/test_capsule.py
--rw-r--r--   0 runner    (1001) docker     (127)     5059 2024-02-06 18:25:10.000000 aind_exaspim_pipeline_utils-0.7.2/tests/test_imagej_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-02-06 18:25:10.000000 aind_exaspim_pipeline_utils-0.7.2/tests/test_n5tozarr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:48.677715 aind_exaspim_pipeline_utils-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:48.661715 aind_exaspim_pipeline_utils-0.8.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:48.665715 aind_exaspim_pipeline_utils-0.8.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/.github/ISSUE_TEMPLATE/user-story.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:48.665715 aind_exaspim_pipeline_utils-0.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/.github/workflows/lint_and_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/.github/workflows/tag_and_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4947 2024-04-02 18:15:48.677715 aind_exaspim_pipeline_utils-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:48.669715 aind_exaspim_pipeline_utils-0.8.0/capsule_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/capsule_scripts/imagej_postInstall
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/capsule_scripts/imagej_run.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/capsule_scripts/n5tozarr_postInstall
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/capsule_scripts/n5tozarr_run.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:48.669715 aind_exaspim_pipeline_utils-0.8.0/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/doc/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:48.669715 aind_exaspim_pipeline_utils-0.8.0/doc/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:48.669715 aind_exaspim_pipeline_utils-0.8.0/doc/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/doc/source/_static/dark-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/doc/source/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/doc/source/_static/light-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 18:15:48.677715 aind_exaspim_pipeline_utils-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:48.665715 aind_exaspim_pipeline_utils-0.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:48.669715 aind_exaspim_pipeline_utils-0.8.0/src/aind_exaspim_pipeline_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/src/aind_exaspim_pipeline_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14493 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/src/aind_exaspim_pipeline_utils/exaspim_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7057 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/src/aind_exaspim_pipeline_utils/imagej_macros.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24042 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/src/aind_exaspim_pipeline_utils/imagej_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:48.673715 aind_exaspim_pipeline_utils-0.8.0/src/aind_exaspim_pipeline_utils/n5tozarr/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/src/aind_exaspim_pipeline_utils/n5tozarr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18825 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/src/aind_exaspim_pipeline_utils/n5tozarr/n5tozarr_da.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:48.673715 aind_exaspim_pipeline_utils-0.8.0/src/aind_exaspim_pipeline_utils/qc/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/src/aind_exaspim_pipeline_utils/qc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/src/aind_exaspim_pipeline_utils/qc/bigstitcher_log_edge_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6987 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/src/aind_exaspim_pipeline_utils/qc/create_ng_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9669 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/src/aind_exaspim_pipeline_utils/qc/ng_ip_visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:48.673715 aind_exaspim_pipeline_utils-0.8.0/src/aind_exaspim_pipeline_utils/trigger/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/src/aind_exaspim_pipeline_utils/trigger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27230 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/src/aind_exaspim_pipeline_utils/trigger/capsule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:48.673715 aind_exaspim_pipeline_utils-0.8.0/src/aind_exaspim_pipeline_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4947 2024-04-02 18:15:48.000000 aind_exaspim_pipeline_utils-0.8.0/src/aind_exaspim_pipeline_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-02 18:15:48.000000 aind_exaspim_pipeline_utils-0.8.0/src/aind_exaspim_pipeline_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 18:15:48.000000 aind_exaspim_pipeline_utils-0.8.0/src/aind_exaspim_pipeline_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-02 18:15:48.000000 aind_exaspim_pipeline_utils-0.8.0/src/aind_exaspim_pipeline_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-02 18:15:48.000000 aind_exaspim_pipeline_utils-0.8.0/src/aind_exaspim_pipeline_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-02 18:15:48.000000 aind_exaspim_pipeline_utils-0.8.0/src/aind_exaspim_pipeline_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:48.673715 aind_exaspim_pipeline_utils-0.8.0/src/aind_trigger_codeocean/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/src/aind_trigger_codeocean/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51638 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/src/aind_trigger_codeocean/pipelines.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:48.673715 aind_exaspim_pipeline_utils-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/tests/test_capsule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5059 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/tests/test_imagej_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-02 18:15:35.000000 aind_exaspim_pipeline_utils-0.8.0/tests/test_n5tozarr.py
```

### Comparing `aind_exaspim_pipeline_utils-0.7.2/.github/ISSUE_TEMPLATE/bug_report.md` & `aind_exaspim_pipeline_utils-0.8.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.7.2/.github/ISSUE_TEMPLATE/feature_request.md` & `aind_exaspim_pipeline_utils-0.8.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.7.2/.github/ISSUE_TEMPLATE/user-story.md` & `aind_exaspim_pipeline_utils-0.8.0/.github/ISSUE_TEMPLATE/user-story.md`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.7.2/.github/workflows/lint_and_test.yml` & `aind_exaspim_pipeline_utils-0.8.0/.github/workflows/lint_and_test.yml`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.7.2/.github/workflows/tag_and_publish.yml` & `aind_exaspim_pipeline_utils-0.8.0/.github/workflows/tag_and_publish.yml`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.7.2/.gitignore` & `aind_exaspim_pipeline_utils-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.7.2/LICENSE` & `aind_exaspim_pipeline_utils-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.7.2/PKG-INFO` & `aind_exaspim_pipeline_utils-0.8.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: aind_exaspim_pipeline_utils
-Version: 0.7.2
+Version: 0.8.0
 Summary: AIND exaSPIM pipeline utilities.
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: argschema
 Requires-Dist: s3fs
 Requires-Dist: pydantic
 Requires-Dist: psutil
 Requires-Dist: aind-data-schema
 Requires-Dist: aind-codeocean-api==0.3.0
-Requires-Dist: aind-ng-link==1.0.6
+Requires-Dist: aind-ng-link>=1.0.15
 Provides-Extra: dev
 Requires-Dist: aind-exaspim-pipeline-utils[n5tozarr]; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: interrogate; extra == "dev"
 Requires-Dist: isort; extra == "dev"
```

### Comparing `aind_exaspim_pipeline_utils-0.7.2/README.md` & `aind_exaspim_pipeline_utils-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.7.2/doc/Makefile` & `aind_exaspim_pipeline_utils-0.8.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.7.2/doc/make.bat` & `aind_exaspim_pipeline_utils-0.8.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.7.2/doc/source/_static/dark-logo.svg` & `aind_exaspim_pipeline_utils-0.8.0/doc/source/_static/dark-logo.svg`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.7.2/doc/source/_static/favicon.ico` & `aind_exaspim_pipeline_utils-0.8.0/doc/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.7.2/doc/source/_static/light-logo.svg` & `aind_exaspim_pipeline_utils-0.8.0/doc/source/_static/light-logo.svg`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.7.2/doc/source/conf.py` & `aind_exaspim_pipeline_utils-0.8.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.7.2/pyproject.toml` & `aind_exaspim_pipeline_utils-0.8.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 dependencies = [
     'argschema',
     's3fs',
     'pydantic',
     'psutil',
     'aind-data-schema',
     'aind-codeocean-api==0.3.0',
-    'aind-ng-link==1.0.6',
+    'aind-ng-link>=1.0.15',
 ]
 
 [project.optional-dependencies]
 dev = [
     'aind-exaspim-pipeline-utils[n5tozarr]',
     'black',
     'coverage',
```

### Comparing `aind_exaspim_pipeline_utils-0.7.2/src/aind_exaspim_pipeline_utils/exaspim_manifest.py` & `aind_exaspim_pipeline_utils-0.8.0/src/aind_exaspim_pipeline_utils/exaspim_manifest.py`

 * *Files 2% similar despite different names*

```diff
@@ -222,25 +222,19 @@
 
 
 class XMLCreationParameters(AindModel):  # pragma: no cover
     """XML converter capsule parameters."""
 
     ch_name: str = Field(..., title="Channel name, without the ch prefix")
 
-    # input_uri: str = Field(
-    #     ...,
-    #     title="Top level s3 uri for input dataset.",
-    # )
-    #
-    # output_uri: str = Field(
-    #     ...,
-    #     title="Output Zarr dataset path. Must be a local filesystem path or "
-    #           "start with s3:// to trigger S3 direct access. "
-    #           "Must be different from the input_uri. Will be overwritten if exists.",
-    # )
+    input_uri: Optional[str] = Field(
+        None,
+        title="Input Zarr group dataset path. This is the dataset the alignment is running on."
+              "Must be the aind-open-data s3:// path without the SPIM.ome.zarr suffix",
+    )
 
 
 class ExaspimProcessingPipeline(AindModel):  # pragma: no cover
     """ExaSPIM processing pipeline configuration parameters
 
     If a field is None, it is considered to be a disabled step."""
```

### Comparing `aind_exaspim_pipeline_utils-0.7.2/src/aind_exaspim_pipeline_utils/imagej_macros.py` & `aind_exaspim_pipeline_utils-0.8.0/src/aind_exaspim_pipeline_utils/imagej_macros.py`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.7.2/src/aind_exaspim_pipeline_utils/imagej_wrapper.py` & `aind_exaspim_pipeline_utils-0.8.0/src/aind_exaspim_pipeline_utils/imagej_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -432,15 +432,16 @@
         imgloader = root.find("SequenceDescription/ImageLoader")
         url = urlparse(args["input_uri"])
         s3b = ET.Element("s3bucket")
         s3b.text = url.netloc
         imgloader.insert(0, s3b)
         elem_zarr = imgloader.find("zarr")
         # substitute regex pattern in the beginning of elem_zarr.text
-        elem_zarr.text = "/" + url.path.strip("/") + "/SPIM.ome.zarr"
+        # Removed leading slash
+        elem_zarr.text = url.path.strip("/") + "/SPIM.ome.zarr"
         # write the xml file
         tree.write(f"../results/{emr_xml_name}", encoding="utf-8")
 
 
 def create_edge_connectivity_report(num_registrations: int) -> None:  # pragma: no cover
     """Create a report of edge connectivity failures."""
     # Read the log file
@@ -521,15 +522,22 @@
 
 
 def imagej_wrapper_main():  # pragma: no cover
     """Entry point with the manifest config."""
     # logging.basicConfig(format="%(asctime)s %(name)s %(levelname)-7s %(message)s")
     logging.basicConfig(format="%(asctime)s %(levelname)-7s %(message)s")
 
+    # Add a file output, too for the logs
+    file_handler = logging.FileHandler("../results/imagej_wrapper.log")
+    file_handler.setLevel(logging.DEBUG)
+    file_handler.setFormatter(logging.Formatter("%(asctime)s %(name)s %(levelname)-7s %(message)s"))
+
     logger = logging.getLogger()
+    logger.addHandler(file_handler)
+
     pipeline_manifest = get_capsule_manifest()
 
     args = {
         "dataset_xml": "../data/manifest/dataset.xml",
         "session_id": pipeline_manifest.pipeline_suffix,
         "log_level": logging.DEBUG,
         "name": pipeline_manifest.name,
@@ -543,25 +551,25 @@
         args["output_uri"] = fmt_uri(pipeline_manifest.ip_detection.IJwrap.output_uri)
         args["input_uri"] = fmt_uri(pipeline_manifest.ip_detection.IJwrap.input_uri)
 
     logger.setLevel(logging.DEBUG)
     logging.getLogger("botocore").setLevel(logging.INFO)
     logging.getLogger("urllib3").setLevel(logging.INFO)
     logging.getLogger("s3fs").setLevel(logging.INFO)
+    logger.info(f"This is pipeline session {args['session_id']}")
 
     args.update(get_auto_parameters(args))
     process_meta = get_imagej_wrapper_metadata(
         {
             "ip_detection": pipeline_manifest.ip_detection,
             "ip_registrations": pipeline_manifest.ip_registrations,
         },
         input_location=args["input_uri"],
         output_location=args["output_uri"],
     )
-
     write_process_metadata(process_meta, prefix="ipreg")
     ip_det_parameters = pipeline_manifest.ip_detection
     if ip_det_parameters is not None:
         logger.info("Copying input xml %s -> %s", args["dataset_xml"], args["process_xml"])
         shutil.copy(args["dataset_xml"], args["process_xml"])
 
         det_params = pipeline_manifest.ip_detection.dict()
```

### Comparing `aind_exaspim_pipeline_utils-0.7.2/src/aind_exaspim_pipeline_utils/n5tozarr/n5tozarr_da.py` & `aind_exaspim_pipeline_utils-0.8.0/src/aind_exaspim_pipeline_utils/n5tozarr/n5tozarr_da.py`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.7.2/src/aind_exaspim_pipeline_utils/qc/bigstitcher_log_edge_analysis.py` & `aind_exaspim_pipeline_utils-0.8.0/src/aind_exaspim_pipeline_utils/qc/bigstitcher_log_edge_analysis.py`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.7.2/src/aind_exaspim_pipeline_utils/qc/create_ng_link.py` & `aind_exaspim_pipeline_utils-0.8.0/src/aind_exaspim_pipeline_utils/qc/create_ng_link.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 
 # Copied from Jonathan's NG link generator capsule code
 
 import json
 from pathlib import Path
 from urllib.parse import urlparse
 
-from ng_link import NgState, link_utils, xml_parsing
+import s3fs
+from ng_link import NgState, link_utils
+from ng_link.parsers import XmlParser
 import numpy as np
 import os
 
 
 def read_json(json_path: str) -> dict:  # pragma: no cover
     """Read a json file and return a dict."""
     with open(json_path) as f:
@@ -38,14 +40,49 @@
         translation = np.round(translation, 4)
 
         tile_positions[tile_path.name] = translation
 
     return tile_positions
 
 
+def get_tile_positions_s3(dataset_uri: str):  # pragma: no cover
+    """Get the tile positions from the zattrs files.
+    Parameters
+    ----------
+
+    dataset_uri: The S3 prefix to the dataset (e.g. "bucket_name/dataset_name/SPIM.ome.zarr")
+    """
+    tile_positions = {}
+    s3 = s3fs.S3FileSystem()
+    url = urlparse(dataset_uri)
+    dataset_path = url.netloc + "/" + url.path.strip("/")
+    for tile_path in s3.ls(dataset_path):
+        if not s3.isdir(tile_path):
+            continue
+
+        tile_path = Path(tile_path)
+        zattrs_file = str(tile_path / ".zattrs")
+        with s3.open(zattrs_file, "r") as f:
+            zattrs_json = json.load(f)
+
+        scale = zattrs_json["multiscales"][0]["datasets"][0]["coordinateTransformations"][0]["scale"]
+        translation = zattrs_json["multiscales"][0]["datasets"][0]["coordinateTransformations"][1][
+            "translation"
+        ]
+
+        scale = np.array(scale[2:][::-1])
+        translation = np.array(translation[2:][::-1])
+        translation /= scale
+        translation = np.round(translation, 4)
+
+        tile_positions[tile_path.name] = translation
+
+    return tile_positions
+
+
 def create_ng_link(
     dataset_uri: str,
     alignment_output_uri: str,
     xml_path: str = "../results/bigstitcher.xml",
     output_json: str = "../results/ng/process_output.json",
 ) -> str:  # pragma: no cover
     """ "Create a Neuroglancer json file and link file for the given alignment solution.
@@ -66,25 +103,25 @@
     # output_uri = 's3://aind-open-data/exaSPIM_659146_2023-11-10_14-02-06/SPIM.ome.zarr'
     # xml_path = '/root/capsule/data/2023-11-27_s18_th03_l150k_659146/bigstitcher_2023-11-27.xml'
     # dataset_path = '/root/capsule/data/exaSPIM_659146_2023-11-10_14-02-06/SPIM.ome.zarr'
     # alignment_run = '2023-11-27'  # Will be attached to upload name: process_output_{alignment_run}.json
     # output_json_path = '/results'
 
     # XML info
-    vox_sizes: tuple[float, float, float] = xml_parsing.extract_tile_vox_size(xml_path)
-    tile_paths: dict[int, str] = xml_parsing.extract_tile_paths(xml_path)
-    tile_transforms: dict[int, list[dict]] = xml_parsing.extract_tile_transforms(xml_path)
+    vox_sizes: tuple[float, float, float] = XmlParser.extract_tile_vox_size(xml_path)
+    tile_paths: dict[int, str] = XmlParser.extract_tile_paths(xml_path)
+    tile_transforms: dict[int, list[dict]] = XmlParser.extract_tile_transforms(xml_path)
 
     # Color info
     channel: int = link_utils.extract_channel_from_tile_path(tile_paths[0])
     hex_val: int = link_utils.wavelength_to_hex(channel)
     hex_str = f"#{str(hex(hex_val))[2:]}"
 
     # Zattrs info
-    zattrs_positions = get_tile_positions("../data/exaspim_dataset/SPIM.ome.zarr")
+    zattrs_positions = get_tile_positions_s3(dataset_uri)
 
     # Update Translation -- undo zattrs transform
     for tile_id, tf in tile_transforms.items():
         t_path = tile_paths[tile_id]
         zattrs_offset = zattrs_positions[t_path]
 
         nums = [float(val) for val in tf[0]["affine"].split(" ")]
@@ -151,15 +188,15 @@
     bucket_name = url.netloc
 
     # Generate the link
     neuroglancer_link = NgState(
         input_config=input_config,
         mount_service="s3",
         bucket_path=bucket_name,
-        output_json=ng_dir,
+        output_dir=ng_dir,
         json_name=json_name,
     )
     neuroglancer_link.save_state_as_json()
     print(neuroglancer_link.get_url_link())
     thelink = f"https://neuroglancer-demo.appspot.com/#!{alignment_output_uri}/ng/{json_name}"
     with open("../results/ng/ng_link.txt", "a") as f:
         print(thelink, file=f)
```

### Comparing `aind_exaspim_pipeline_utils-0.7.2/src/aind_exaspim_pipeline_utils/trigger/capsule.py` & `aind_exaspim_pipeline_utils-0.8.0/src/aind_exaspim_pipeline_utils/trigger/capsule.py`

 * *Files 1% similar despite different names*

```diff
@@ -480,24 +480,25 @@
         regularize_with_choice="rigid",
     )
 
     ch_name = args.channel
     # Even the flat-fielded fusions goes with the raw dataset prefix
     n5_to_zarr: N5toZarrParameters = N5toZarrParameters(
         voxel_size_zyx=(1.0, 0.748, 0.748),
-        input_uri=f"s3://{args.fusion_output_bucket}/{args.fusion_output_prefix}/fused.n5/ch{ch_name}/",
+        input_uri=f"s3://{args.fusion_output_bucket}/{args.fusion_output_prefix}/fused.n5/setup0/timepoint0/",
         output_uri=f"s3://{args.fusion_output_bucket}/{args.fusion_output_prefix}/fused.zarr/",
     )
 
     zarr_multiscale: ZarrMultiscaleParameters = ZarrMultiscaleParameters(
         voxel_size_zyx=(1.0, 0.748, 0.748),
         input_uri=f"s3://{args.fusion_output_bucket}/{args.fusion_output_prefix}/fused.zarr/",
     )
 
-    xml_creation: XMLCreationParameters = XMLCreationParameters(ch_name=ch_name)
+    xml_creation: XMLCreationParameters = XMLCreationParameters(ch_name=ch_name,
+                                                                input_uri=args.exaspim_data_uri)
 
     processing_manifest: ExaspimProcessingPipeline = ExaspimProcessingPipeline(
         creation_time=args.pipeline_timestamp,
         pipeline_suffix=args.fname_timestamp,
         subject_id=metadata["subject"].get("subject_id"),
         name=metadata["data_description"].get("name"),
         xml_creation=xml_creation,
@@ -515,21 +516,23 @@
         )
 
     return processing_manifest
 
 
 def create_and_upload_emr_config(args, manifest: ExaspimProcessingPipeline):  # pragma: no cover
     """Create EMR command line parameters for the fusion of the present alignment run."""
-    ch_name = args.channel
     config = (
-        f"-x, {args.alignment_output_uri}"
-        f"bigstitcher_emr_{manifest.subject_id}_{manifest.pipeline_suffix}_0.xml,\n"
-        f"--outS3Bucket, {args.fusion_output_bucket}, -o, /{args.fusion_output_prefix}/fused.n5,\n"
-        f"-d, /ch{ch_name}/s0, --storage, N5, --UINT16, --minIntensity=0, "
-        f"--maxIntensity=65535, --preserveAnisotropy\n"
+        f"[\"-x\", \"{args.alignment_output_uri}"
+        f"bigstitcher_emr_{manifest.subject_id}_{manifest.pipeline_suffix}_0.xml\",\n"
+        f"\"--outS3Bucket\", \"{args.fusion_output_bucket}\", "
+        f"\"-o\", \"/{args.fusion_output_prefix}/fused.n5\",\n"
+        f"\"--bdv\", \"0,0\", "
+        f"\"--xmlout\", \"s3://{args.fusion_output_bucket}/{args.fusion_output_prefix}/fused.xml\", "
+        "\"--storage\", \"N5\", \"--UINT16\", \"--minIntensity=0\", "
+        "\"--maxIntensity=65535\", \"--preserveAnisotropy\" ]\n"
     )
     with open("../results/emr_fusion_config.txt", "w") as f:
         f.write(config)
     logger.info("Uploading emr_fusion_config.txt to bucket {}".format(args.manifest_bucket_name))
     s3 = boto3.client("s3")  # Authentication should be available in the environment
     object_name = "/".join((args.manifest_path, "emr_fusion_config.txt"))
     s3.upload_file("../results/emr_fusion_config.txt", args.manifest_bucket_name, object_name)
```

### Comparing `aind_exaspim_pipeline_utils-0.7.2/src/aind_exaspim_pipeline_utils.egg-info/PKG-INFO` & `aind_exaspim_pipeline_utils-0.8.0/src/aind_exaspim_pipeline_utils.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: aind_exaspim_pipeline_utils
-Version: 0.7.2
+Version: 0.8.0
 Summary: AIND exaSPIM pipeline utilities.
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: argschema
 Requires-Dist: s3fs
 Requires-Dist: pydantic
 Requires-Dist: psutil
 Requires-Dist: aind-data-schema
 Requires-Dist: aind-codeocean-api==0.3.0
-Requires-Dist: aind-ng-link==1.0.6
+Requires-Dist: aind-ng-link>=1.0.15
 Provides-Extra: dev
 Requires-Dist: aind-exaspim-pipeline-utils[n5tozarr]; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: interrogate; extra == "dev"
 Requires-Dist: isort; extra == "dev"
```

### Comparing `aind_exaspim_pipeline_utils-0.7.2/src/aind_exaspim_pipeline_utils.egg-info/SOURCES.txt` & `aind_exaspim_pipeline_utils-0.8.0/src/aind_exaspim_pipeline_utils.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 src/aind_exaspim_pipeline_utils.egg-info/requires.txt
 src/aind_exaspim_pipeline_utils.egg-info/top_level.txt
 src/aind_exaspim_pipeline_utils/n5tozarr/__init__.py
 src/aind_exaspim_pipeline_utils/n5tozarr/n5tozarr_da.py
 src/aind_exaspim_pipeline_utils/qc/__init__.py
 src/aind_exaspim_pipeline_utils/qc/bigstitcher_log_edge_analysis.py
 src/aind_exaspim_pipeline_utils/qc/create_ng_link.py
+src/aind_exaspim_pipeline_utils/qc/ng_ip_visualization.py
 src/aind_exaspim_pipeline_utils/trigger/__init__.py
 src/aind_exaspim_pipeline_utils/trigger/capsule.py
 src/aind_trigger_codeocean/__init__.py
 src/aind_trigger_codeocean/pipelines.py
 tests/__init__.py
 tests/test_capsule.py
 tests/test_imagej_wrapper.py
```

### Comparing `aind_exaspim_pipeline_utils-0.7.2/src/aind_exaspim_pipeline_utils.egg-info/entry_points.txt` & `aind_exaspim_pipeline_utils-0.8.0/src/aind_exaspim_pipeline_utils.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.7.2/src/aind_trigger_codeocean/pipelines.py` & `aind_exaspim_pipeline_utils-0.8.0/src/aind_trigger_codeocean/pipelines.py`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.7.2/tests/test_capsule.py` & `aind_exaspim_pipeline_utils-0.8.0/tests/test_capsule.py`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.7.2/tests/test_imagej_wrapper.py` & `aind_exaspim_pipeline_utils-0.8.0/tests/test_imagej_wrapper.py`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.7.2/tests/test_n5tozarr.py` & `aind_exaspim_pipeline_utils-0.8.0/tests/test_n5tozarr.py`

 * *Files identical despite different names*

