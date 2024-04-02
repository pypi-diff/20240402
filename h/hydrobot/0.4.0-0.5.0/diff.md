# Comparing `tmp/hydrobot-0.4.0.tar.gz` & `tmp/hydrobot-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydrobot-0.4.0.tar", last modified: Tue Jan 30 02:11:51 2024, max compression
+gzip compressed data, was "hydrobot-0.5.0.tar", last modified: Tue Apr  2 20:04:32 2024, max compression
```

## Comparing `hydrobot-0.4.0.tar` & `hydrobot-0.5.0.tar`

### file list

```diff
@@ -1,94 +1,93 @@
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-01-30 02:11:51.031528 hydrobot-0.4.0/
--rw-r--r--   0 nic       (1000) nic       (1000)      292 2023-09-27 02:03:08.000000 hydrobot-0.4.0/.editorconfig
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-01-30 02:11:51.001528 hydrobot-0.4.0/.github/
--rw-r--r--   0 nic       (1000) nic       (1000)      333 2023-09-27 02:03:08.000000 hydrobot-0.4.0/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 nic       (1000) nic       (1000)     1207 2023-10-16 02:52:42.000000 hydrobot-0.4.0/.gitignore
--rw-r--r--   0 nic       (1000) nic       (1000)      514 2023-12-12 21:50:38.000000 hydrobot-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0 nic       (1000) nic       (1000)     1068 2023-12-12 21:50:38.000000 hydrobot-0.4.0/.readthedocs.yaml
--rw-r--r--   0 nic       (1000) nic       (1000)      212 2023-10-16 02:52:42.000000 hydrobot-0.4.0/AUTHORS.rst
--rw-r--r--   0 nic       (1000) nic       (1000)     7004 2023-12-18 02:34:17.000000 hydrobot-0.4.0/CONTRIBUTING.rst
--rw-r--r--   0 nic       (1000) nic       (1000)     1170 2024-01-30 01:58:59.000000 hydrobot-0.4.0/HISTORY.rst
--rw-r--r--   0 nic       (1000) nic       (1000)     1610 2023-10-16 02:47:23.000000 hydrobot-0.4.0/LICENSE
--rw-r--r--   0 nic       (1000) nic       (1000)      298 2023-12-12 21:50:38.000000 hydrobot-0.4.0/MANIFEST.in
--rw-r--r--   0 nic       (1000) nic       (1000)     2336 2023-12-12 21:50:38.000000 hydrobot-0.4.0/Makefile
--rw-r--r--   0 nic       (1000) nic       (1000)     3153 2024-01-30 02:11:51.021528 hydrobot-0.4.0/PKG-INFO
--rw-r--r--   0 nic       (1000) nic       (1000)     1446 2024-01-30 01:39:43.000000 hydrobot-0.4.0/README.rst
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-01-30 02:11:51.001528 hydrobot-0.4.0/docs/
--rw-r--r--   0 nic       (1000) nic       (1000)      609 2023-11-02 03:51:37.000000 hydrobot-0.4.0/docs/Makefile
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-01-30 02:11:51.001528 hydrobot-0.4.0/docs/_build/
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-01-30 02:11:51.001528 hydrobot-0.4.0/docs/_build/html/
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-01-30 02:11:51.011528 hydrobot-0.4.0/docs/_build/html/_static/
--rw-r--r--   0 nic       (1000) nic       (1000)      286 2023-12-12 21:10:33.000000 hydrobot-0.4.0/docs/_build/html/_static/file.png
--rw-r--r--   0 nic       (1000) nic       (1000)       90 2023-12-12 21:10:33.000000 hydrobot-0.4.0/docs/_build/html/_static/minus.png
--rw-r--r--   0 nic       (1000) nic       (1000)       90 2023-12-12 21:10:33.000000 hydrobot-0.4.0/docs/_build/html/_static/plus.png
--rw-r--r--   0 nic       (1000) nic       (1000)       28 2023-09-27 02:03:08.000000 hydrobot-0.4.0/docs/authors.rst
--rwxr-xr-x   0 nic       (1000) nic       (1000)     5087 2023-12-12 21:50:38.000000 hydrobot-0.4.0/docs/conf.py
--rw-r--r--   0 nic       (1000) nic       (1000)       33 2023-09-27 02:03:08.000000 hydrobot-0.4.0/docs/contributing.rst
--rw-r--r--   0 nic       (1000) nic       (1000)       28 2023-09-27 02:03:08.000000 hydrobot-0.4.0/docs/history.rst
--rw-r--r--   0 nic       (1000) nic       (1000)     1190 2023-12-12 21:50:38.000000 hydrobot-0.4.0/docs/hydrobot.rst
--rw-r--r--   0 nic       (1000) nic       (1000)      305 2023-11-02 03:51:37.000000 hydrobot-0.4.0/docs/index.rst
--rw-r--r--   0 nic       (1000) nic       (1000)     1555 2023-12-12 21:50:38.000000 hydrobot-0.4.0/docs/installation.rst
--rw-r--r--   0 nic       (1000) nic       (1000)      806 2023-11-02 03:51:37.000000 hydrobot-0.4.0/docs/make.bat
--rw-r--r--   0 nic       (1000) nic       (1000)       61 2023-12-12 21:10:41.000000 hydrobot-0.4.0/docs/modules.rst
--rw-r--r--   0 nic       (1000) nic       (1000)       27 2023-09-27 02:03:08.000000 hydrobot-0.4.0/docs/readme.rst
--rw-r--r--   0 nic       (1000) nic       (1000)       71 2023-11-02 03:51:37.000000 hydrobot-0.4.0/docs/usage.rst
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-01-30 02:11:51.011528 hydrobot-0.4.0/hydrobot/
--rw-r--r--   0 nic       (1000) nic       (1000)      153 2024-01-30 02:04:18.000000 hydrobot-0.4.0/hydrobot/__init__.py
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-01-30 02:11:51.011528 hydrobot-0.4.0/hydrobot/config/
--rw-r--r--   0 nic       (1000) nic       (1000)       79 2024-01-29 01:08:42.000000 hydrobot-0.4.0/hydrobot/config/QualityCodeEvaluator_QC_config.csv
--rw-r--r--   0 nic       (1000) nic       (1000)       55 2024-01-29 01:08:42.000000 hydrobot-0.4.0/hydrobot/config/TwoLevelQualityCodeEvaluator_QC_config.csv
--rw-r--r--   0 nic       (1000) nic       (1000)     3162 2024-01-29 01:08:42.000000 hydrobot-0.4.0/hydrobot/data_acquisition.py
--rw-r--r--   0 nic       (1000) nic       (1000)     9236 2024-01-30 01:55:17.000000 hydrobot-0.4.0/hydrobot/data_sources.py
--rw-r--r--   0 nic       (1000) nic       (1000)    13754 2024-01-30 01:39:43.000000 hydrobot-0.4.0/hydrobot/evaluator.py
--rw-r--r--   0 nic       (1000) nic       (1000)     7516 2024-01-29 01:08:42.000000 hydrobot-0.4.0/hydrobot/filters.py
--rw-r--r--   0 nic       (1000) nic       (1000)     5563 2024-01-29 01:08:42.000000 hydrobot-0.4.0/hydrobot/plotter.py
--rw-r--r--   0 nic       (1000) nic       (1000)    54158 2024-01-30 01:55:17.000000 hydrobot-0.4.0/hydrobot/processor.py
--rw-r--r--   0 nic       (1000) nic       (1000)     1806 2024-01-30 01:55:17.000000 hydrobot-0.4.0/hydrobot/utils.py
--rw-r--r--   0 nic       (1000) nic       (1000)    30917 2024-01-30 00:26:40.000000 hydrobot-0.4.0/hydrobot/xml_data_structure.py
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-01-30 02:11:51.021528 hydrobot-0.4.0/hydrobot.egg-info/
--rw-r--r--   0 nic       (1000) nic       (1000)     3153 2024-01-30 02:11:50.000000 hydrobot-0.4.0/hydrobot.egg-info/PKG-INFO
--rw-r--r--   0 nic       (1000) nic       (1000)     2114 2024-01-30 02:11:50.000000 hydrobot-0.4.0/hydrobot.egg-info/SOURCES.txt
--rw-r--r--   0 nic       (1000) nic       (1000)        1 2024-01-30 02:11:50.000000 hydrobot-0.4.0/hydrobot.egg-info/dependency_links.txt
--rw-r--r--   0 nic       (1000) nic       (1000)      296 2024-01-30 02:11:50.000000 hydrobot-0.4.0/hydrobot.egg-info/requires.txt
--rw-r--r--   0 nic       (1000) nic       (1000)        9 2024-01-30 02:11:50.000000 hydrobot-0.4.0/hydrobot.egg-info/top_level.txt
--rw-r--r--   0 nic       (1000) nic       (1000)      422 2024-01-29 01:08:42.000000 hydrobot-0.4.0/old_setup.cfg
--rw-r--r--   0 nic       (1000) nic       (1000)     1571 2024-01-29 01:08:42.000000 hydrobot-0.4.0/old_setup.py
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-01-30 02:11:51.011528 hydrobot-0.4.0/prototypes/
--rw-r--r--   0 nic       (1000) nic       (1000)     2031 2024-01-30 01:55:17.000000 hydrobot-0.4.0/prototypes/Class_script.py
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-01-30 02:11:51.021528 hydrobot-0.4.0/prototypes/Jupyter_notebooks/
--rw-r--r--   0 nic       (1000) nic       (1000)   299418 2023-11-21 00:21:33.000000 hydrobot-0.4.0/prototypes/Jupyter_notebooks/All_Sites_Atmospheric_Pressure.ipynb
--rw-r--r--   0 nic       (1000) nic       (1000)   376016 2023-11-21 00:21:33.000000 hydrobot-0.4.0/prototypes/Jupyter_notebooks/Saddle_Road_Spike_Removal.ipynb
--rw-r--r--   0 nic       (1000) nic       (1000)   432396 2023-11-21 00:21:33.000000 hydrobot-0.4.0/prototypes/Jupyter_notebooks/Time_Series_Analysis.ipynb
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-01-30 02:11:51.021528 hydrobot-0.4.0/prototypes/output_dump/
--rw-r--r--   0 nic       (1000) nic       (1000)      144 2023-11-02 01:24:43.000000 hydrobot-0.4.0/prototypes/output_dump/.gitignore
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-01-30 02:11:51.021528 hydrobot-0.4.0/prototypes/py_scripts/
--rw-r--r--   0 nic       (1000) nic       (1000)     1515 2024-01-29 01:08:42.000000 hydrobot-0.4.0/prototypes/py_scripts/atmospheric_spike_removal.py
--rw-r--r--   0 nic       (1000) nic       (1000)     1051 2023-12-12 21:50:38.000000 hydrobot-0.4.0/prototypes/py_scripts/example_plot_script.py
--rw-r--r--   0 nic       (1000) nic       (1000)     1568 2023-12-12 21:50:38.000000 hydrobot-0.4.0/prototypes/py_scripts/gap_finder.py
--rw-r--r--   0 nic       (1000) nic       (1000)     1319 2023-12-12 21:50:38.000000 hydrobot-0.4.0/prototypes/py_scripts/new_ws_plot_with_check_data.py
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-01-30 02:11:51.021528 hydrobot-0.4.0/prototypes/py_scripts/output_dump/
--rw-r--r--   0 nic       (1000) nic       (1000)      144 2023-11-02 01:24:43.000000 hydrobot-0.4.0/prototypes/py_scripts/output_dump/.gitignore
--rw-r--r--   0 nic       (1000) nic       (1000)     1001 2024-01-29 01:44:22.000000 hydrobot-0.4.0/prototypes/py_scripts/plot_with_check_data.py
--rw-r--r--   0 nic       (1000) nic       (1000)     4222 2024-01-29 01:08:42.000000 hydrobot-0.4.0/prototypes/py_scripts/process_script.py
--rw-r--r--   0 nic       (1000) nic       (1000)      933 2023-12-03 22:14:39.000000 hydrobot-0.4.0/prototypes/py_scripts/spike_removal_util.py
--rw-r--r--   0 nic       (1000) nic       (1000)     3509 2024-01-29 01:08:42.000000 hydrobot-0.4.0/prototypes/py_scripts/stage_full_process.py
--rw-r--r--   0 nic       (1000) nic       (1000)     3627 2024-01-29 01:08:42.000000 hydrobot-0.4.0/prototypes/py_scripts/water_temp_full_process.py
--rw-r--r--   0 nic       (1000) nic       (1000)     1927 2023-11-02 02:57:00.000000 hydrobot-0.4.0/prototypes/py_scripts/water_temp_spike_removal.py
--rw-r--r--   0 nic       (1000) nic       (1000)     1419 2024-01-29 01:08:42.000000 hydrobot-0.4.0/prototypes/site_list_reader.py
--rw-r--r--   0 nic       (1000) nic       (1000)      443 2024-01-29 01:08:42.000000 hydrobot-0.4.0/prototypes/site_parameters.json
--rw-r--r--   0 nic       (1000) nic       (1000)     3070 2024-01-30 02:08:50.000000 hydrobot-0.4.0/pyproject.toml
--rw-r--r--   0 nic       (1000) nic       (1000)     2404 2024-01-30 01:39:43.000000 hydrobot-0.4.0/requirements_dev.txt
--rw-r--r--   0 nic       (1000) nic       (1000)      506 2023-12-11 22:10:08.000000 hydrobot-0.4.0/requirements_test.txt
--rw-r--r--   0 nic       (1000) nic       (1000)       38 2024-01-30 02:11:51.031528 hydrobot-0.4.0/setup.cfg
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-01-30 02:11:51.021528 hydrobot-0.4.0/tests/
--rw-r--r--   0 nic       (1000) nic       (1000)    53248 2023-12-10 21:16:55.000000 hydrobot-0.4.0/tests/.coverage
--rw-r--r--   0 nic       (1000) nic       (1000)       38 2023-11-02 02:57:00.000000 hydrobot-0.4.0/tests/__init__.py
--rw-r--r--   0 nic       (1000) nic       (1000)     1007 2024-01-29 01:08:42.000000 hydrobot-0.4.0/tests/conftest.py
--rw-r--r--   0 nic       (1000) nic       (1000)      245 2023-11-02 01:24:43.000000 hydrobot-0.4.0/tests/site_list_response.xml
--rw-r--r--   0 nic       (1000) nic       (1000)     1007 2024-01-29 01:08:42.000000 hydrobot-0.4.0/tests/test_data_sources.py
--rw-r--r--   0 nic       (1000) nic       (1000)    12753 2024-01-30 01:39:43.000000 hydrobot-0.4.0/tests/test_evaluator.py
--rw-r--r--   0 nic       (1000) nic       (1000)     9481 2024-01-29 01:08:42.000000 hydrobot-0.4.0/tests/test_filters.py
--rw-r--r--   0 nic       (1000) nic       (1000)    11415 2024-01-30 01:54:09.000000 hydrobot-0.4.0/tests/test_integration.py
--rw-r--r--   0 nic       (1000) nic       (1000)    20075 2024-01-30 01:54:22.000000 hydrobot-0.4.0/tests/test_processor.py
--rw-r--r--   0 nic       (1000) nic       (1000)     9712 2024-01-29 01:08:42.000000 hydrobot-0.4.0/tests/test_xml_data_structure.py
--rw-r--r--   0 nic       (1000) nic       (1000)    11975 2024-01-29 01:08:42.000000 hydrobot-0.4.0/tests/xml_test_data_file.xml
+drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-02 20:04:32.582867 hydrobot-0.5.0/
+-rw-r--r--   0 nic       (1000) nic       (1000)      292 2023-09-27 02:03:08.000000 hydrobot-0.5.0/.editorconfig
+drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-02 20:04:32.562867 hydrobot-0.5.0/.github/
+-rw-r--r--   0 nic       (1000) nic       (1000)      333 2023-09-27 02:03:08.000000 hydrobot-0.5.0/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 nic       (1000) nic       (1000)     1207 2023-10-16 02:52:42.000000 hydrobot-0.5.0/.gitignore
+-rw-r--r--   0 nic       (1000) nic       (1000)      514 2024-03-11 01:19:58.000000 hydrobot-0.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 nic       (1000) nic       (1000)     1068 2024-03-11 01:19:58.000000 hydrobot-0.5.0/.readthedocs.yaml
+-rw-r--r--   0 nic       (1000) nic       (1000)      212 2023-10-16 02:52:42.000000 hydrobot-0.5.0/AUTHORS.rst
+-rw-r--r--   0 nic       (1000) nic       (1000)     7004 2024-03-11 01:19:58.000000 hydrobot-0.5.0/CONTRIBUTING.rst
+-rw-r--r--   0 nic       (1000) nic       (1000)     1368 2024-04-02 19:57:10.000000 hydrobot-0.5.0/HISTORY.rst
+-rw-r--r--   0 nic       (1000) nic       (1000)     1610 2023-10-16 02:47:23.000000 hydrobot-0.5.0/LICENSE
+-rw-r--r--   0 nic       (1000) nic       (1000)      298 2024-03-11 01:19:58.000000 hydrobot-0.5.0/MANIFEST.in
+-rw-r--r--   0 nic       (1000) nic       (1000)     2336 2024-03-11 01:19:58.000000 hydrobot-0.5.0/Makefile
+-rw-r--r--   0 nic       (1000) nic       (1000)     6556 2024-04-02 20:04:32.582867 hydrobot-0.5.0/PKG-INFO
+-rw-r--r--   0 nic       (1000) nic       (1000)     4823 2024-04-02 19:49:26.000000 hydrobot-0.5.0/README.rst
+drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-02 20:04:32.562867 hydrobot-0.5.0/docs/
+-rw-r--r--   0 nic       (1000) nic       (1000)      609 2023-11-02 03:51:37.000000 hydrobot-0.5.0/docs/Makefile
+drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-02 20:04:32.552868 hydrobot-0.5.0/docs/_build/
+drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-02 20:04:32.552868 hydrobot-0.5.0/docs/_build/html/
+drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-02 20:04:32.562867 hydrobot-0.5.0/docs/_build/html/_static/
+-rw-r--r--   0 nic       (1000) nic       (1000)      286 2023-12-12 21:10:33.000000 hydrobot-0.5.0/docs/_build/html/_static/file.png
+-rw-r--r--   0 nic       (1000) nic       (1000)       90 2023-12-12 21:10:33.000000 hydrobot-0.5.0/docs/_build/html/_static/minus.png
+-rw-r--r--   0 nic       (1000) nic       (1000)       90 2023-12-12 21:10:33.000000 hydrobot-0.5.0/docs/_build/html/_static/plus.png
+-rw-r--r--   0 nic       (1000) nic       (1000)       28 2023-09-27 02:03:08.000000 hydrobot-0.5.0/docs/authors.rst
+-rwxr-xr-x   0 nic       (1000) nic       (1000)     5087 2024-03-11 01:19:58.000000 hydrobot-0.5.0/docs/conf.py
+-rw-r--r--   0 nic       (1000) nic       (1000)       33 2023-09-27 02:03:08.000000 hydrobot-0.5.0/docs/contributing.rst
+-rw-r--r--   0 nic       (1000) nic       (1000)       28 2023-09-27 02:03:08.000000 hydrobot-0.5.0/docs/history.rst
+-rw-r--r--   0 nic       (1000) nic       (1000)     1190 2024-03-11 01:19:58.000000 hydrobot-0.5.0/docs/hydrobot.rst
+-rw-r--r--   0 nic       (1000) nic       (1000)      305 2023-11-02 03:51:37.000000 hydrobot-0.5.0/docs/index.rst
+-rw-r--r--   0 nic       (1000) nic       (1000)     1555 2024-03-11 01:19:58.000000 hydrobot-0.5.0/docs/installation.rst
+-rw-r--r--   0 nic       (1000) nic       (1000)      806 2023-11-02 03:51:37.000000 hydrobot-0.5.0/docs/make.bat
+-rw-r--r--   0 nic       (1000) nic       (1000)       61 2023-12-12 21:10:41.000000 hydrobot-0.5.0/docs/modules.rst
+-rw-r--r--   0 nic       (1000) nic       (1000)       27 2023-09-27 02:03:08.000000 hydrobot-0.5.0/docs/readme.rst
+-rw-r--r--   0 nic       (1000) nic       (1000)       71 2023-11-02 03:51:37.000000 hydrobot-0.5.0/docs/usage.rst
+drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-02 20:04:32.572867 hydrobot-0.5.0/hydrobot/
+-rw-r--r--   0 nic       (1000) nic       (1000)      153 2024-04-02 20:01:08.000000 hydrobot-0.5.0/hydrobot/__init__.py
+drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-02 20:04:32.572867 hydrobot-0.5.0/hydrobot/config/
+-rw-r--r--   0 nic       (1000) nic       (1000)      105 2024-03-11 01:19:58.000000 hydrobot-0.5.0/hydrobot/config/QualityCodeEvaluator_QC_config.csv
+-rw-r--r--   0 nic       (1000) nic       (1000)       55 2024-03-11 01:19:58.000000 hydrobot-0.5.0/hydrobot/config/TwoLevelQualityCodeEvaluator_QC_config.csv
+-rw-r--r--   0 nic       (1000) nic       (1000)     5728 2024-04-01 22:51:29.000000 hydrobot-0.5.0/hydrobot/data_acquisition.py
+-rw-r--r--   0 nic       (1000) nic       (1000)     8005 2024-04-02 01:09:54.000000 hydrobot-0.5.0/hydrobot/data_sources.py
+-rw-r--r--   0 nic       (1000) nic       (1000)    32675 2024-04-02 00:34:08.000000 hydrobot-0.5.0/hydrobot/data_structure.py
+-rw-r--r--   0 nic       (1000) nic       (1000)    13768 2024-04-01 22:51:29.000000 hydrobot-0.5.0/hydrobot/evaluator.py
+-rw-r--r--   0 nic       (1000) nic       (1000)     7516 2024-03-11 01:19:58.000000 hydrobot-0.5.0/hydrobot/filters.py
+-rw-r--r--   0 nic       (1000) nic       (1000)    20727 2024-04-01 22:51:29.000000 hydrobot-0.5.0/hydrobot/plotter.py
+-rw-r--r--   0 nic       (1000) nic       (1000)    52042 2024-04-02 20:02:29.000000 hydrobot-0.5.0/hydrobot/processor.py
+-rw-r--r--   0 nic       (1000) nic       (1000)     7778 2024-04-01 22:51:29.000000 hydrobot-0.5.0/hydrobot/utils.py
+drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-02 20:04:32.572867 hydrobot-0.5.0/hydrobot.egg-info/
+-rw-r--r--   0 nic       (1000) nic       (1000)     6556 2024-04-02 20:04:32.000000 hydrobot-0.5.0/hydrobot.egg-info/PKG-INFO
+-rw-r--r--   0 nic       (1000) nic       (1000)     1981 2024-04-02 20:04:32.000000 hydrobot-0.5.0/hydrobot.egg-info/SOURCES.txt
+-rw-r--r--   0 nic       (1000) nic       (1000)        1 2024-04-02 20:04:32.000000 hydrobot-0.5.0/hydrobot.egg-info/dependency_links.txt
+-rw-r--r--   0 nic       (1000) nic       (1000)      311 2024-04-02 20:04:32.000000 hydrobot-0.5.0/hydrobot.egg-info/requires.txt
+-rw-r--r--   0 nic       (1000) nic       (1000)        9 2024-04-02 20:04:32.000000 hydrobot-0.5.0/hydrobot.egg-info/top_level.txt
+-rw-r--r--   0 nic       (1000) nic       (1000)      422 2024-03-11 01:19:58.000000 hydrobot-0.5.0/old_setup.cfg
+-rw-r--r--   0 nic       (1000) nic       (1000)     1571 2024-03-11 01:19:58.000000 hydrobot-0.5.0/old_setup.py
+drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-02 20:04:32.572867 hydrobot-0.5.0/prototypes/
+-rw-r--r--   0 nic       (1000) nic       (1000)     4257 2024-04-02 20:02:29.000000 hydrobot-0.5.0/prototypes/Class_script.py
+drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-02 20:04:32.572867 hydrobot-0.5.0/prototypes/output_dump/
+-rw-r--r--   0 nic       (1000) nic       (1000)      144 2023-11-02 01:24:43.000000 hydrobot-0.5.0/prototypes/output_dump/.gitignore
+drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-02 20:04:32.572867 hydrobot-0.5.0/prototypes/py_scripts/
+-rw-r--r--   0 nic       (1000) nic       (1000)     1515 2024-03-11 01:19:58.000000 hydrobot-0.5.0/prototypes/py_scripts/atmospheric_spike_removal.py
+-rw-r--r--   0 nic       (1000) nic       (1000)     1051 2024-03-11 01:19:58.000000 hydrobot-0.5.0/prototypes/py_scripts/example_plot_script.py
+-rw-r--r--   0 nic       (1000) nic       (1000)     1581 2024-04-01 22:51:29.000000 hydrobot-0.5.0/prototypes/py_scripts/gap_finder.py
+-rw-r--r--   0 nic       (1000) nic       (1000)     1319 2024-03-11 01:19:58.000000 hydrobot-0.5.0/prototypes/py_scripts/new_ws_plot_with_check_data.py
+drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-02 20:04:32.572867 hydrobot-0.5.0/prototypes/py_scripts/output_dump/
+-rw-r--r--   0 nic       (1000) nic       (1000)      144 2023-11-02 01:24:43.000000 hydrobot-0.5.0/prototypes/py_scripts/output_dump/.gitignore
+-rw-r--r--   0 nic       (1000) nic       (1000)     1001 2024-03-11 01:19:58.000000 hydrobot-0.5.0/prototypes/py_scripts/plot_with_check_data.py
+-rw-r--r--   0 nic       (1000) nic       (1000)     4222 2024-03-11 01:19:58.000000 hydrobot-0.5.0/prototypes/py_scripts/process_script.py
+-rw-r--r--   0 nic       (1000) nic       (1000)      933 2023-12-03 22:14:39.000000 hydrobot-0.5.0/prototypes/py_scripts/spike_removal_util.py
+-rw-r--r--   0 nic       (1000) nic       (1000)     3509 2024-03-11 01:19:58.000000 hydrobot-0.5.0/prototypes/py_scripts/stage_full_process.py
+-rw-r--r--   0 nic       (1000) nic       (1000)     3627 2024-03-11 01:19:58.000000 hydrobot-0.5.0/prototypes/py_scripts/water_temp_full_process.py
+-rw-r--r--   0 nic       (1000) nic       (1000)     1927 2023-11-02 02:57:00.000000 hydrobot-0.5.0/prototypes/py_scripts/water_temp_spike_removal.py
+drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-02 20:04:32.572867 hydrobot-0.5.0/prototypes/script_dump/
+-rw-r--r--   0 nic       (1000) nic       (1000)      144 2024-03-11 01:19:58.000000 hydrobot-0.5.0/prototypes/script_dump/.gitignore
+-rw-r--r--   0 nic       (1000) nic       (1000)     1419 2024-03-11 01:19:58.000000 hydrobot-0.5.0/prototypes/site_list_reader.py
+-rw-r--r--   0 nic       (1000) nic       (1000)      443 2024-03-11 01:19:58.000000 hydrobot-0.5.0/prototypes/site_parameters.json
+-rw-r--r--   0 nic       (1000) nic       (1000)     3088 2024-04-02 20:01:08.000000 hydrobot-0.5.0/pyproject.toml
+-rw-r--r--   0 nic       (1000) nic       (1000)     2419 2024-04-02 20:02:29.000000 hydrobot-0.5.0/requirements_dev.txt
+-rw-r--r--   0 nic       (1000) nic       (1000)      506 2024-03-11 01:19:58.000000 hydrobot-0.5.0/requirements_test.txt
+-rw-r--r--   0 nic       (1000) nic       (1000)       38 2024-04-02 20:04:32.582867 hydrobot-0.5.0/setup.cfg
+drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-02 20:04:32.572867 hydrobot-0.5.0/tests/
+-rw-r--r--   0 nic       (1000) nic       (1000)    53248 2024-02-26 00:40:14.000000 hydrobot-0.5.0/tests/.coverage
+-rw-r--r--   0 nic       (1000) nic       (1000)       38 2023-11-02 02:57:00.000000 hydrobot-0.5.0/tests/__init__.py
+-rw-r--r--   0 nic       (1000) nic       (1000)     1007 2024-03-11 01:19:58.000000 hydrobot-0.5.0/tests/conftest.py
+-rw-r--r--   0 nic       (1000) nic       (1000)      245 2023-11-02 01:24:43.000000 hydrobot-0.5.0/tests/site_list_response.xml
+-rw-r--r--   0 nic       (1000) nic       (1000)     2929 2024-03-11 01:19:58.000000 hydrobot-0.5.0/tests/test_data_sources.py
+-rw-r--r--   0 nic       (1000) nic       (1000)     9730 2024-04-02 00:40:43.000000 hydrobot-0.5.0/tests/test_data_structure.py
+-rw-r--r--   0 nic       (1000) nic       (1000)    12753 2024-03-11 01:19:58.000000 hydrobot-0.5.0/tests/test_evaluator.py
+-rw-r--r--   0 nic       (1000) nic       (1000)     9481 2024-03-11 01:19:58.000000 hydrobot-0.5.0/tests/test_filters.py
+-rw-r--r--   0 nic       (1000) nic       (1000)    24981 2024-04-02 01:02:45.000000 hydrobot-0.5.0/tests/test_processor.py
+-rw-r--r--   0 nic       (1000) nic       (1000)     2557 2024-04-01 22:51:29.000000 hydrobot-0.5.0/tests/test_utils.py
+-rw-r--r--   0 nic       (1000) nic       (1000)    24135 2024-04-02 01:19:50.000000 hydrobot-0.5.0/tests/test_web_integration.py
+-rw-r--r--   0 nic       (1000) nic       (1000)    13995 2024-04-02 00:42:31.000000 hydrobot-0.5.0/tests/xml_test_data_file.xml
```

### Comparing `hydrobot-0.4.0/.gitignore` & `hydrobot-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `hydrobot-0.4.0/.pre-commit-config.yaml` & `hydrobot-0.5.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `hydrobot-0.4.0/.readthedocs.yaml` & `hydrobot-0.5.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `hydrobot-0.4.0/CONTRIBUTING.rst` & `hydrobot-0.5.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `hydrobot-0.4.0/HISTORY.rst` & `hydrobot-0.5.0/HISTORY.rst`

 * *Files 27% similar despite different names*

```diff
@@ -53,7 +53,14 @@
 
 * Implementing the QC0 data removal tool promised in 0.3.1
 
 0.4.0 (2024-01-30)
 ------------------
 
 * XML backend and exporting support added.
+
+0.5.0 (2024-04-03) - Alpha Release
+----------------------------------
+
+* Plotly diagnostics added.
+* Support for external (to Hilltop) check data added.
+* Hybrid workflow supported and documented.
```

### Comparing `hydrobot-0.4.0/LICENSE` & `hydrobot-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hydrobot-0.4.0/Makefile` & `hydrobot-0.5.0/Makefile`

 * *Files identical despite different names*

### Comparing `hydrobot-0.4.0/docs/Makefile` & `hydrobot-0.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hydrobot-0.4.0/docs/conf.py` & `hydrobot-0.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `hydrobot-0.4.0/docs/hydrobot.rst` & `hydrobot-0.5.0/docs/hydrobot.rst`

 * *Files identical despite different names*

### Comparing `hydrobot-0.4.0/docs/installation.rst` & `hydrobot-0.5.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `hydrobot-0.4.0/docs/make.bat` & `hydrobot-0.5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `hydrobot-0.4.0/hydrobot/data_sources.py` & `hydrobot-0.5.0/hydrobot/data_sources.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Handling for different types of data sources."""
 import csv
-import re
 from pathlib import Path
 
 import numpy as np
 import pandas as pd
 
 
 class QualityCodeEvaluator:
@@ -44,18 +43,20 @@
         -------
         int
             The Quality code
 
         """
         diff = np.abs(base_datum - check_datum)
         if diff < self.qc_600_limit:
-            return 600
-        if diff < self.qc_500_limit:
-            return 500
-        return 400
+            qc = 600
+        elif diff < self.qc_500_limit:
+            qc = 500
+        else:
+            qc = 400
+        return qc
 
 
 class TwoLevelQualityCodeEvaluator(QualityCodeEvaluator):
     """QualityCodeEvaluator for standards such as water level.
 
     Fixed error up to given threshold, percentage error after that.
     """
@@ -83,21 +84,18 @@
             Threshold between QC 500 and QC 600 for percentage portion
         limit_percent_threshold
             Value at which the evaluator transitions between linear and percentage
             QC comparison
         name : str
             Name of the data source
         """
-        QualityCodeEvaluator.__init__(self, qc_500_limit, qc_600_limit)
-        # self.qc_500_limit = qc_500_limit
-        # self.qc_600_limit = qc_600_limit
+        QualityCodeEvaluator.__init__(self, qc_500_limit, qc_600_limit, name)
         self.qc_500_percent = qc_500_percent
         self.qc_600_percent = qc_600_percent
         self.limit_percent_threshold = limit_percent_threshold
-        self.name = name
 
     def find_qc(self, base_datum, check_datum):
         """Find the base quality codes with two stages.
 
         The two stages are: a flat and percentage QC threshold.
 
         Parameters
@@ -113,25 +111,29 @@
             The Quality code
 
         """
         if base_datum < self.limit_percent_threshold:
             # flat qc check
             diff = np.abs(base_datum - check_datum)
             if diff < self.qc_600_limit:
-                return 600
-            if diff < self.qc_500_limit:
-                return 500
-            return 400
-        # percent qc check
-        diff = np.abs(base_datum / check_datum - 1) * 100
-        if diff < self.qc_600_percent:
-            return 600
-        if diff < self.qc_500_percent:
-            return 500
-        return 400
+                qc = 600
+            elif diff < self.qc_500_limit:
+                qc = 500
+            else:
+                qc = 400
+        else:
+            # percent qc check
+            diff = np.abs(base_datum / check_datum - 1) * 100
+            if diff < self.qc_600_percent:
+                qc = 600
+            elif diff < self.qc_500_percent:
+                qc = 500
+            else:
+                qc = 400
+        return qc
 
 
 def get_qc_evaluator_dict():
     """Return all qc_evaluators in a dictionary.
 
     Returns
     -------
@@ -194,68 +196,31 @@
         f"qc_evaluator {qc_evaluator_name} not found in the config file. "
         f"Available qc_evaluators are {list(qce_dict.keys())}."
     )
 
 
 def series_export_to_csv(
     file_location: str,
-    site_name: str,
-    measurement_name: str,
-    std_series: pd.Series | None,
-    check_series: pd.Series | None,
-    qc_series: pd.Series | None,
+    series: list[pd.Series],
 ) -> None:
     """Export the 3 main series to csv.
 
     Parameters
     ----------
     file_location : str
         Where the files are exported to
-    site_name : str
-        Site name
-    measurement_name : str
-        Measurement name
-    std_series : pd.Series
-        Standard series
-    check_series : pd.Series
-        Check series
-    qc_series : pd.Series
-        Quality code series
+    series : pd.Series
+        Pandas series to be exported
 
     Returns
     -------
     None, but makes files
     """
-    if std_series is not None:
-        std_series.to_csv(
-            str(file_location)
-            + "std_"
-            + site_name
-            + "-"
-            + re.sub("[^A-Za-z0-9]+", "_", measurement_name)
-            + ".csv"
-        )
-    if check_series is not None:
-        check_series.to_csv(
-            str(file_location)
-            + "check_"
-            + site_name
-            + "-"
-            + re.sub("[^A-Za-z0-9]+", "_", measurement_name)
-            + ".csv"
-        )
-    if qc_series is not None:
-        qc_series.to_csv(
-            str(file_location)
-            + "QC_"
-            + site_name
-            + "-"
-            + re.sub("[^A-Za-z0-9]+", "_", measurement_name)
-            + ".csv"
-        )
+    export_df = pd.DataFrame(series).T
+    export_df.to_csv(str(file_location))
 
 
 def hilltop_export(
     file_location: str,
     site_name: str,
     measurement_name: str,
     std_series: pd.Series,
@@ -284,22 +249,15 @@
     -------
     None, but makes files
     """
     qc_series = qc_series.reindex(std_series.index, method="ffill")
     std_series.name = "std"
     qc_series.name = "qual"
     export_df = std_series.to_frame().join(qc_series)
-    export_df.to_csv(
-        str(file_location)
-        + "hilltop_combined_std_QC_"
-        + site_name
-        + "-"
-        + re.sub("[^A-Za-z0-9]+", "_", measurement_name)
-        + ".csv"
-    )
+    export_df.to_csv(str(file_location) + "_std_qc.csv")
 
     keys = [
         "Sitename",
         "Inspection_Date",
         "Inspection_Time",
         "External S.G.",
         "Recorder Time",
@@ -320,15 +278,9 @@
             pd.Series(check_series.index, index=check_series.index),
             pd.Series(-1, index=check_series.index),
             pd.Series("hydrobot comment", index=check_series.index),
         ],
         axis=1,
         keys=keys,
     )
-    export_check_df.to_csv(
-        str(file_location)
-        + "hilltop_check_import_"
-        + site_name
-        + "-"
-        + re.sub("[^A-Za-z0-9]+", "_", measurement_name)
-        + ".csv"
-    )
+
+    export_check_df.to_csv(str(file_location) + "_check.csv")
```

### Comparing `hydrobot-0.4.0/hydrobot/evaluator.py` & `hydrobot-0.5.0/hydrobot/evaluator.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     idx0 = np.flatnonzero(np.r_[True, np.diff(np.isnan(data)) != 0, True])
     count = np.diff(idx0)
     idx = idx0[:-1]
     valid_mask = pd.isna(data.iloc[idx])
     out_idx = idx[valid_mask]
     out_count = count[valid_mask]
     indices = data.iloc[out_idx].index
-    out = zip(indices, out_count)
+    out = zip(indices, out_count, strict=True)
 
     return list(out)
 
 
 def small_gap_closer(series: pd.Series, gap_limit: int) -> pd.Series:
     """
     Remove small gaps from a series.
@@ -390,14 +390,15 @@
                 .fillna(base_series.median())
                 .asfreq(frequency)
             )
         else:
             return_dict[qc] = base_data_meets_qc(base_series, qc_series, qc).asfreq(
                 frequency
             )
+
     return return_dict
 
 
 def max_qc_limiter(qc_series: pd.Series, max_qc) -> pd.Series:
     """
     Enforce max_qc on a QC series.
```

### Comparing `hydrobot-0.4.0/hydrobot/filters.py` & `hydrobot-0.5.0/hydrobot/filters.py`

 * *Files identical despite different names*

### Comparing `hydrobot-0.4.0/hydrobot/processor.py` & `hydrobot-0.5.0/hydrobot/processor.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 from annalist.annalist import Annalist
 from annalist.decorators import ClassLogger
 from hilltoppy import Hilltop
 
 from hydrobot import (
     data_acquisition,
     data_sources,
+    data_structure,
     evaluator,
     filters,
     plotter,
     utils,
-    xml_data_structure,
 )
 
 annalizer = Annalist()
 
 DEFAULTS = {
     "high_clip": 20000,
     "low_clip": 0,
@@ -145,26 +145,35 @@
                 f"Site '{site}' not found for both base_url and hts combos."
                 f"Available sites in standard_hts are: "
                 f"{[s for s in standard_hilltop.available_sites]}"
                 f"Available sites in check_hts are: "
                 f"{[s for s in check_hilltop.available_sites]}"
             )
 
+        # standard
         available_standard_measurements = standard_hilltop.get_measurement_list(site)
-        if standard_measurement_name in list(
+        self._standard_measurement_name = standard_measurement_name
+        matches = re.search(r"([^\[\n]+)(\[(.+)\])?", standard_measurement_name)
+
+        if matches is not None:
+            self.standard_item_name = matches.groups()[0].strip(" ")
+            self.standard_data_source_name = matches.groups()[2]
+            if self.standard_data_source_name is None:
+                self.standard_data_source_name = self.standard_item_name
+        if standard_measurement_name not in list(
             available_standard_measurements.MeasurementName
         ):
-            self._standard_measurement_name = standard_measurement_name
-        else:
             raise ValueError(
                 f"Standard measurement name '{standard_measurement_name}' not found at"
                 f" site '{site}'. "
                 "Available measurements are "
                 f"{list(available_standard_measurements.MeasurementName)}"
             )
+
+        # check
         available_check_measurements = check_hilltop.get_measurement_list(site)
         self._check_measurement_name = check_measurement_name
         matches = re.search(r"([^\[\n]+)(\[(.+)\])?", check_measurement_name)
 
         if matches is not None:
             self.check_item_name = matches.groups()[0].strip(" ")
             self.check_data_source_name = matches.groups()[2]
@@ -189,25 +198,23 @@
         self._quality_code_evaluator = data_sources.get_qc_evaluator(
             standard_measurement_name
         )
         self._stale = True
         self._no_data = True
         self._standard_series = pd.Series({})
         self._check_series = pd.Series({})
-        self._check_data = pd.DataFrame({})
         self._quality_series = pd.Series({})
 
-        self.raw_standard_series = None
+        self.raw_standard_series = pd.Series({})
         self.raw_standard_blob = None
         self.raw_standard_xml = None
-        self.raw_quality_series = None
+        self.raw_quality_series = pd.Series({})
         self.raw_quality_blob = None
         self.raw_quality_xml = None
-        self.raw_check_data = None
-        self.raw_check_series = None
+        self.raw_check_data = pd.DataFrame({})
         self.raw_check_blob = None
         self.raw_check_xml = None
 
         # Load data for the first time
         self.import_data(from_date=self.from_date, to_date=self.to_date)
 
     @property
@@ -279,15 +286,15 @@
         return self._check_hts
 
     @property
     def quality_code_evaluator(self):  # type: ignore
         """Measurement property."""
         return self._quality_code_evaluator
 
-    @ClassLogger  # type: ignore
+    @ClassLogger
     @quality_code_evaluator.setter
     def quality_code_evaluator(self, value):
         self._quality_code_evaluator = value
         self._stale = True
 
     @property
     def defaults(self):  # type: ignore
@@ -305,33 +312,22 @@
 
     @ClassLogger  # type: ignore
     @standard_series.setter
     def standard_series(self, value):
         self._standard_series = value
 
     @property
-    def check_data(self):  # type: ignore
-        """pd.DataFrame: The DataFrame containing check data."""
-        return self._check_data
-
-    @check_data.setter
-    def check_data(self, value):
-        self._check_data = value
-        self._check_series = self._check_data[self.check_item_name]
-
-    @property
     def check_series(self):  # type: ignore
         """pd.Series: The series containing check data."""
         return self._check_series
 
     @ClassLogger  # type: ignore
     @check_series.setter
     def check_series(self, value):
         self._check_series = value
-        self._check_data[self.check_item_name] = value
 
     @property
     def quality_series(self):  # type: ignore
         """
         pd.Series: The quality series data.
 
         Setting this property will mark the data as stale.
@@ -345,31 +341,26 @@
         self._stale = True
 
     @ClassLogger
     def import_standard(
         self,
         from_date: str | None = None,
         to_date: str | None = None,
-        overwrite: bool = False,
     ):
         """
         Import standard data.
 
         Parameters
         ----------
         from_date : str or None, optional
             The start date for data retrieval. If None, defaults to earliest available
             data.
         to_date : str or None, optional
             The end date for data retrieval. If None, defaults to latest available
             data.
-        overwrite : bool, optional
-            If True, overwrite existing data with newly acquired data for overlapping
-            timestamps. If False, keep existing data and only add new datapoints if
-            they don't already exist.
 
         Returns
         -------
         None
 
         Raises
         ------
@@ -394,146 +385,119 @@
         the Standard Series in the instance.
         The data is parsed and formatted according to the item_info in the data source.
 
         Examples
         --------
         >>> processor = Processor(...)  # initialize processor instance
         >>> processor.import_standard(
-        ...     from_date='2022-01-01', to_date='2022-01-10', overwrite=True
+        ...     from_date='2022-01-01', to_date='2022-01-10'
         ... )
         """
         xml_tree, blob_list = data_acquisition.get_data(
             self._base_url,
             self._standard_hts,
             self._site,
             self._standard_measurement_name,
             from_date,
             to_date,
             tstype="Standard",
         )
 
-        if isinstance(self._standard_series, pd.Series):
-            warnings.warn(
-                "Just letting you know that you're overwriting the raw data."
-                " I couldn't figure out how else to do this."
-                " I can probably do it but I have other things to do right now."
-                " TODO: Remove unprofessional warnings from code.",
-                stacklevel=1,
-            )
-            curr_series = self._standard_series
-        else:
-            warnings.warn(
-                "Existing Standard Series should be pandas.Series, but found "
-                f"{type(self._standard_series)}. Setting to empty pd.Series",
-                stacklevel=1,
-            )
-            curr_series = pd.Series({})
-        insert_series = pd.Series({})
         blob_found = False
 
-        if blob_list is None or len(blob_list) == 0:
-            raise ValueError("No standard data found within specified date range.")
         date_format = "Calendar"
         data_source_list = []
-        for blob in blob_list:
-            data_source_list += [blob.data_source.name]
-            if (blob.data_source.name == self._standard_measurement_name) and (
-                blob.data_source.ts_type == "StdSeries"
-            ):
-                insert_series = blob.data.timeseries
-                date_format = blob.data.date_format
-                if insert_series is not None:
-                    # Found it. Now we extract it.
-                    blob_found = True
-                    self.raw_standard_blob = blob
-                    self.raw_standard_xml = xml_tree
-                    self.raw_standard_series = insert_series
-        if not blob_found:
-            raise ValueError(
-                f"Standard Data Not Found under name "
-                f"{self._standard_measurement_name}. "
-                f"Available data sources are: {data_source_list}"
+        if blob_list is None or len(blob_list) == 0:
+            warnings.warn(
+                "No standard data found within specified date range.",
+                stacklevel=1,
             )
+        else:
+            for blob in blob_list:
+                data_source_list += [blob.data_source.name]
+                if (blob.data_source.name == self.standard_data_source_name) and (
+                    blob.data_source.ts_type == "StdSeries"
+                ):
+                    self.raw_standard_series = blob.data.timeseries
+                    date_format = blob.data.date_format
+                    if self.raw_standard_series is not None:
+                        # Found it. Now we extract it.
+                        blob_found = True
+                        self.raw_standard_blob = blob
+                        self.raw_standard_xml = xml_tree
+            if not blob_found:
+                raise ValueError(
+                    f"Standard Data Not Found under name "
+                    f"{self._standard_measurement_name}. "
+                    f"Available data sources are: {data_source_list}"
+                )
 
-        if not isinstance(insert_series, pd.Series):
-            raise TypeError(
-                f"Expecting pd.Series for Standard data, but got {type(insert_series)}"
-                "from parser."
-            )
-        if not insert_series.empty:
-            if date_format == "mowsecs":
-                insert_series.index = utils.mowsecs_to_datetime_index(
-                    insert_series.index
+            if not isinstance(self.raw_standard_series, pd.Series):
+                raise TypeError(
+                    f"Expecting pd.Series for Standard data, but got {type(self.raw_standard_series)}"
+                    "from parser."
+                )
+            if not self.raw_standard_series.empty:
+                if date_format == "mowsecs":
+                    self.raw_standard_series.index = utils.mowsecs_to_datetime_index(
+                        self.raw_standard_series.index
+                    )
+                else:
+                    self.raw_standard_series.index = pd.to_datetime(
+                        self.raw_standard_series.index
+                    )
+                self.raw_standard_series = self.raw_standard_series.asfreq(
+                    self._frequency, fill_value=np.NaN
                 )
+            if self.raw_standard_blob is not None:
+                fmt = self.raw_standard_blob.data_source.item_info[0].item_format
+                div = self.raw_standard_blob.data_source.item_info[0].divisor
             else:
-                insert_series.index = pd.to_datetime(insert_series.index)
-            insert_series = insert_series.asfreq(self._frequency, method="ffill")
-        if not curr_series.empty:
-            if overwrite:
-                # Combine, but overwrite overlapping timestamps with newly acquired
-                # data
-                self._standard_series = insert_series.combine_first(
-                    curr_series
-                ).sort_index()
+                warnings.warn(
+                    "Could not extract standard data format from data source. "
+                    "Defaulting to float format.",
+                    stacklevel=1,
+                )
+                fmt = "F"
+                div = 1
+            if div is None or div == "None":
+                div = 1
+            if fmt == "I":
+                self.raw_standard_series = self.raw_standard_series.astype(int) / int(
+                    div
+                )
+            elif fmt == "F":
+                self.raw_standard_series = self.raw_standard_series.astype(
+                    np.float32
+                ) / float(div)
+            elif fmt == "D":  # Not sure if this would ever really happen, but...
+                self.raw_standard_series = utils.mowsecs_to_datetime_index(
+                    self.raw_standard_series
+                )
             else:
-                # Combine, keeping all existing values and only adding new datapoints
-                # if they don't already exist.
-                self._standard_series = curr_series.combine_first(
-                    insert_series
-                ).sort_index()
-        else:
-            self._standard_series = insert_series
-        if self.raw_standard_blob is not None:
-            fmt = self.raw_standard_blob.data_source.item_info[0].item_format
-            div = self.raw_standard_blob.data_source.item_info[0].divisor
-        else:
-            warnings.warn(
-                "Could not extract standard data format from data source. "
-                "Defaulting to float format.",
-                stacklevel=1,
-            )
-            fmt = "F"
-            div = 1
-        if div is None or div == "None":
-            div = 1
-        if fmt == "I":
-            self.standard_series = self._standard_series.astype(int) / int(div)
-        elif fmt == "F":
-            self.standard_series = self._standard_series.astype(np.float32) / float(div)
-        elif fmt == "D":  # Not sure if this would ever really happen, but...
-            self.standard_series = utils.mowsecs_to_datetime_index(
-                self._standard_series
-            )
-        else:
-            raise ValueError(f"Unknown Format Spec: {fmt}")
-        self.raw_standard_series = self._standard_series
+                raise ValueError(f"Unknown Format Spec: {fmt}")
+            self.standard_series = self.raw_standard_series
 
     @ClassLogger
     def import_quality(
         self,
         from_date: str | None = None,
         to_date: str | None = None,
-        overwrite: bool = False,
     ):
         """
         Import quality data.
 
         Parameters
         ----------
         from_date : str or None, optional
             The start date for data retrieval. If None, defaults to earliest available
             data.
         to_date : str or None, optional
             The end date for data retrieval. If None, defaults to latest available
             data.
-        overwrite : bool, optional
-            If True, overwrite existing data with newly acquired data for overlapping
-            timestamps.
-            If False, keep existing data and only add new datapoints if they don't
-            already exist.
 
         Returns
         -------
         None
 
         Raises
         ------
@@ -568,106 +532,78 @@
             self._site,
             self._standard_measurement_name,
             from_date,
             to_date,
             tstype="Quality",
         )
 
-        if isinstance(self._quality_series, pd.Series):
-            curr_series = self._quality_series
-        else:
-            warnings.warn(
-                "Existing Quality Series should be pandas.Series, but found "
-                f"{type(self._quality_series)}. Setting to empty pd.Series",
-                stacklevel=1,
-            )
-            curr_series = pd.Series({})
-        insert_series = pd.Series({})
         blob_found = False
 
         if blob_list is None or len(blob_list) == 0:
             warnings.warn(
                 "No Quality data available for the range specified.",
-                stacklevel=2,
+                stacklevel=1,
             )
         else:
             date_format = "Calendar"
             for blob in blob_list:
-                if (blob.data_source.name == self._standard_measurement_name) and (
+                if (blob.data_source.name == self.standard_data_source_name) and (
                     blob.data_source.ts_type == "StdQualSeries"
                 ):
                     # Found it. Now we extract it.
                     blob_found = True
 
-                    insert_series = blob.data.timeseries
+                    self.raw_quality_series = blob.data.timeseries
                     date_format = blob.data.date_format
-                    if insert_series is not None:
+                    if self.raw_quality_series is not None:
                         # Found it. Now we extract it.
                         blob_found = True
                         self.raw_quality_blob = blob
                         self.raw_quality_xml = xml_tree
             if not blob_found:
                 warnings.warn(
                     "No Quality data found in the server response.",
                     stacklevel=2,
                 )
 
-            if not isinstance(insert_series, pd.Series):
+            if not isinstance(self.raw_quality_series, pd.Series):
                 raise TypeError(
                     f"Expecting pd.Series for Quality data, but got "
-                    f"{type(insert_series)} from parser."
+                    f"{type(self.raw_quality_series)} from parser."
                 )
-            if not insert_series.empty:
+            if not self.raw_quality_series.empty:
                 if date_format == "mowsecs":
-                    insert_series.index = utils.mowsecs_to_datetime_index(
-                        insert_series.index
+                    self.raw_quality_series.index = utils.mowsecs_to_datetime_index(
+                        self.raw_quality_series.index
                     )
                 else:
-                    insert_series.index = pd.to_datetime(insert_series.index)
+                    self.raw_quality_series.index = pd.to_datetime(
+                        self.raw_quality_series.index
+                    )
 
-            if not curr_series.empty:
-                if overwrite:
-                    # Combine, but overwrite overlapping timestamps with newly acquired
-                    # data
-                    self._quality_series = insert_series.combine_first(
-                        curr_series
-                    ).sort_index()
-                else:
-                    # Combine, keeping all existing values and only adding new
-                    # datapoints if they don't already exist.
-                    self._quality_series = curr_series.combine_first(
-                        insert_series
-                    ).sort_index()
-            elif not insert_series.empty:
-                self._quality_series = insert_series
-            self.quality_series = self._quality_series.astype(int)
-            self.raw_quality_series = self.quality_series.astype(int)
+            self.quality_series = self.raw_quality_series.astype(int)
+            self._quality_series.name = self._standard_measurement_name + " [Quality]"
 
     @ClassLogger
     def import_check(
         self,
         from_date: str | None = None,
         to_date: str | None = None,
-        overwrite: bool = False,
     ):
         """
         Import Check data.
 
         Parameters
         ----------
         from_date : str or None, optional
             The start date for data retrieval. If None, defaults to earliest available
             data.
         to_date : str or None, optional
             The end date for data retrieval. If None, defaults to latest available
             data.
-        overwrite : bool, optional
-            If True, overwrite existing data with newly acquired data for overlapping
-            timestamps. If False, keep existing data and only add new datapoints if
-            they don't already exist.
 
         Returns
         -------
         None
 
         Raises
         ------
@@ -681,17 +617,16 @@
                 empty DataFrame.
             - If no Check data is available for the specified date range.
             - If the Check data source is not found in the server response.
 
         Notes
         -----
         This method imports Check data from the specified server based on the provided
-        parameters. It retrieves data using the `data_acquisition.get_data` function
-        and updates the Check data in the instance. The data is parsed and formatted
-        according to the item_info in the data source.
+        parameters. It retrieves data using the `data_acquisition.get_data` function.
+        The data is parsed and formatted according to the item_info in the data source.
 
         Examples
         --------
         >>> processor = Processor(...)  # initialize processor instance
         >>> processor.import_check(
         ...     from_date='2022-01-01', to_date='2022-01-10', overwrite=True
         ... )
@@ -701,24 +636,15 @@
             self._check_hts,
             self._site,
             self._check_measurement_name,
             from_date,
             to_date,
             tstype="Check",
         )
-        if isinstance(self._check_data, pd.DataFrame):
-            curr_data = self._check_data
-        else:
-            warnings.warn(
-                "Existing Check Data should be pandas.DataFrame, but found "
-                f"{type(self._check_data)}. Setting to empty pd.DataFrame",
-                stacklevel=1,
-            )
-            curr_data = pd.DataFrame({})
-        insert_data = pd.DataFrame({})
+        import_data = pd.DataFrame({})
         blob_found = False
 
         date_format = "Calendar"
         if blob_list is None or len(blob_list) == 0:
             warnings.warn(
                 "No Check data available for the range specified.",
                 stacklevel=2,
@@ -732,87 +658,76 @@
                 ):
                     # Found it. Now we extract it.
                     blob_found = True
 
                     date_format = blob.data.date_format
 
                     # This could be a pd.Series
-                    insert_data = blob.data.timeseries
-                    if insert_data is not None:
+                    import_data = blob.data.timeseries
+                    if import_data is not None:
                         self.raw_check_blob = blob
                         self.raw_check_xml = xml_tree
-                        self.raw_check_data = insert_data
+                        self.raw_check_data = import_data
             if not blob_found:
                 warnings.warn(
                     f"Check data {self.check_data_source_name} not found in server "
                     f"response. Available options are {data_source_options}",
                     stacklevel=2,
                 )
 
-            if not isinstance(insert_data, pd.DataFrame):
+            if not isinstance(self.raw_check_data, pd.DataFrame):
                 raise TypeError(
-                    f"Expecting pd.DataFrame for Check data, but got {type(insert_data)}"
+                    f"Expecting pd.DataFrame for Check data, but got {type(self.raw_check_data)}"
                     "from parser."
                 )
-            if not insert_data.empty:
+            if not self.raw_check_data.empty:
                 if date_format == "mowsecs":
-                    insert_data.index = utils.mowsecs_to_datetime_index(
-                        insert_data.index
+                    self.raw_check_data.index = utils.mowsecs_to_datetime_index(
+                        self.raw_check_data.index
                     )
                 else:
-                    insert_data.index = pd.to_datetime(insert_data.index)
+                    self.raw_check_data.index = pd.to_datetime(
+                        self.raw_check_data.index
+                    )
 
-            if not curr_data.empty:
-                if overwrite:
-                    # Combine, but overwrite overlapping timestamps with newly acquired
-                    # data
-                    self._check_data = insert_data.combine_first(curr_data).sort_index()
-                else:
-                    # Combine, keeping all existing values and only adding new datapoints
-                    # if they don't already exist.
-                    self._check_data = curr_data.combine_first(insert_data).sort_index()
-            elif not insert_data.empty:
-                self._check_data = insert_data
-            if not self._check_data.empty and self.raw_check_blob is not None:
+            if not self.raw_check_data.empty and self.raw_check_blob is not None:
                 # TODO: Maybe this should happen in the parser?
                 for i, item in enumerate(self.raw_check_blob.data_source.item_info):
                     fmt = item.item_format
                     div = item.divisor
-                    col = self._check_data.iloc[:, i]
+                    col = self.raw_check_data.iloc[:, i]
                     if fmt == "I":
-                        self._check_data.iloc[:, i] = col.astype(int) / int(div)
+                        self.raw_check_data.iloc[:, i] = col.astype(int) / int(div)
                     elif fmt == "F":
-                        self._check_data.iloc[:, i] = col.astype(np.float32) / float(
+                        self.raw_check_data.iloc[:, i] = col.astype(np.float32) / float(
                             div
                         )
                     elif fmt == "D":
-                        if self._check_data.iloc[:, i].dtype != pd.Timestamp:
+                        if self.raw_check_data.iloc[:, i].dtype != pd.Timestamp:
                             if date_format == "mowsecs":
-                                self._check_data.iloc[
+                                self.raw_check_data.iloc[
                                     :, i
                                 ] = utils.mowsecs_to_datetime_index(col)
                             else:
-                                self._check_data.iloc[:, i] = col.astype(pd.Timestamp)
+                                self.raw_check_data.iloc[:, i] = col.astype(
+                                    pd.Timestamp
+                                )
                     elif fmt == "S":
-                        self._check_data.iloc[:, i] = col.astype(str)
+                        self.raw_check_data.iloc[:, i] = col.astype(str)
 
-            self.check_data = self._check_data
-            self.raw_check_data = self.check_data
-            if not self._check_data.empty:
-                self.check_series = self.check_data[self.check_item_name]
-                self.raw_check_series = self.check_data[self.check_item_name]
+            if not self.raw_check_data.empty:
+                self.check_series = self.raw_check_data[self.check_item_name]
             else:
                 self.check_series = pd.Series({})
-                self.raw_check_series = pd.Series({})
+            self._check_series.name = self._standard_measurement_name + " [Check]"
 
     def import_data(
         self,
         from_date: str | None = None,
         to_date: str | None = None,
-        overwrite: bool = False,
         standard: bool = True,
         check: bool = True,
         quality: bool = True,
     ):
         """
         Import data using the class parameter range.
 
@@ -847,32 +762,79 @@
         if (
             self._standard_series is not None
             and not self._standard_series.empty
             and self._quality_series is not None
             and not self._quality_series.empty
             and self._check_series is not None
             and not self._check_series.empty
-            and self._check_data is not None
-            and not self._check_data.empty
         ):
             warnings.warn(
-                "Just letting you know that you're overwriting the raw data."
-                " I couldn't figure out how else to do this."
-                " I can probably do it but I have other things to do right now."
-                " TODO: Remove unprofessional warnings from code.",
+                "When you reimport, you are overwriting your data. You will lose all"
+                "progess up to this point.",
                 stacklevel=1,
             )
         if standard:
-            self.import_standard(from_date, to_date, overwrite)
+            self.import_standard(from_date, to_date)
         if quality:
-            self.import_quality(from_date, to_date, overwrite)
+            self.import_quality(from_date, to_date)
         if check:
-            self.import_check(from_date, to_date, overwrite)
+            self.import_check(from_date, to_date)
         self._stale = False
 
+    @ClassLogger
+    def add_standard(self, extra_standard):
+        """
+        Incorporate extra standard data into the standard series using utils.merge_series.
+
+        Parameters
+        ----------
+        extra_standard
+            extra standard data
+
+        Returns
+        -------
+        None, but adds data to self.standard_series
+        """
+        combined = utils.merge_series(self.standard_series, extra_standard)
+        self.standard_series = combined
+
+    @ClassLogger
+    def add_check(self, extra_check):
+        """
+        Incorporate extra check data into the check series using utils.merge_series.
+
+        Parameters
+        ----------
+        extra_check
+            extra check data
+
+        Returns
+        -------
+        None, but adds data to self.check_series
+        """
+        combined = utils.merge_series(self.check_series, extra_check)
+        self.check_series = combined
+
+    @ClassLogger
+    def add_quality(self, extra_quality):
+        """
+        Incorporate extra quality data into the quality series using utils.merge_series.
+
+        Parameters
+        ----------
+        extra_quality
+            extra quality data
+
+        Returns
+        -------
+        None, but adds data to self.quality_series
+        """
+        combined = utils.merge_series(self.quality_series, extra_quality)
+        self.quality_series = combined
+
     # @stale_warning  # type: ignore
     @ClassLogger
     def gap_closer(self, gap_limit: int | None = None):
         """
         Close small gaps in the standard series.
 
         Parameters
@@ -985,19 +947,14 @@
         """
         if low_clip is None:
             low_clip = float(self._defaults["low_clip"])
         if high_clip is None:
             high_clip = float(self._defaults["high_clip"])
 
         self.standard_series = filters.clip(self._standard_series, low_clip, high_clip)
-        self.check_series = filters.clip(
-            pd.Series(self._check_series),
-            low_clip,
-            high_clip,
-        )
 
     # @stale_warning  # type: ignore
     @ClassLogger
     def remove_outliers(self, span: int | None = None, delta: float | None = None):
         """
         Remove outliers from the data.
 
@@ -1200,28 +1157,32 @@
         self.standard_series = self._standard_series.asfreq(self._frequency)
 
     @ClassLogger
     def data_exporter(
         self,
         file_location,
         ftype="xml",
-        standard=True,
-        quality=True,
-        check=False,
+        standard: bool = True,
+        quality: bool = True,
+        check: bool = False,
         trimmed=True,
     ):
         """
         Export data to CSV file.
 
         Parameters
         ----------
         file_location : str
-            The file path where the file will be saved.
+            The file path where the file will be saved. If 'ftype' is "csv" or "xml",
+            this should be a full file path including extension. If 'ftype' is
+            "hilltop_csv", multiple files will be created, so 'file_location' should be
+            a prefix that will be appended with "_std_qc.csv" for the file containing
+            the standard and quality data, and "_check.csv" for the check data file.
         ftype : str, optional
-            Avalable options are "xml", "csv".
+            Avalable options are "xml", "hilltop_csv", "csv".
         trimmed : bool, optional
             If True, export trimmed data; otherwise, export the full data.
             Default is True.
 
         Returns
         -------
         None
@@ -1232,45 +1193,48 @@
 
         Examples
         --------
         >>> processor = Processor(base_url="https://hilltop-server.com", site="Site1")
         >>> processor.data_exporter("output.xml", trimmed=True)
         >>> # Check the generated XML file at 'output.xml'
         """
+        export_selections = [standard, quality, check]
         if trimmed:
             std_series = filters.trim_series(
                 self._standard_series,
                 self._check_series,
             )
         else:
             std_series = self._standard_series
 
         if ftype == "csv":
-            data_sources.series_export_to_csv(
-                file_location,
-                self._site,
-                self._quality_code_evaluator.name,
-                std_series,
-                self._check_series,
+            all_series = [
+                self._standard_series,
                 self._quality_series,
-            )
+                self._check_series,
+            ]
+            export_list = [
+                i for (i, v) in zip(all_series, export_selections, strict=True) if v
+            ]
+            data_sources.series_export_to_csv(file_location, series=export_list)
         if ftype == "hilltop_csv":
+            print("At the exporter:", self.quality_series.index.dtype)
             data_sources.hilltop_export(
                 file_location,
                 self._site,
                 self._quality_code_evaluator.name,
                 std_series,
                 self._check_series,
                 self._quality_series,
             )
         if ftype == "xml":
             blob_list = self.to_xml_data_structure(
                 standard=standard, quality=quality, check=check
             )
-            xml_data_structure.write_hilltop_xml(blob_list, file_location)
+            data_structure.write_hilltop_xml(blob_list, file_location)
 
     def diagnosis(self):
         """
         Provide a diagnosis of the data.
 
         Returns
         -------
@@ -1292,34 +1256,36 @@
         evaluator.diagnose_data(
             self._standard_series,
             self._check_series,
             self._quality_series,
             self._frequency,
         )
 
-    def plot_qc_series(self, show=True):
+    def plot_qc_series(self, check=False, show=True):
         """Implement qc_plotter()."""
-        plotter.qc_plotter(
+        fig = plotter.qc_plotter_plotly(
             self._standard_series,
-            self._check_series,
+            (self._check_series if check else None),
             self._quality_series,
             self._frequency,
             show=show,
         )
+        return fig
 
     def plot_comparison_qc_series(self, show=True):
         """Implement comparison_qc_plotter()."""
-        plotter.comparison_qc_plotter(
+        fig = plotter.comparison_qc_plotter_plotly(
             self._standard_series,
             self.raw_standard_series,
             self._check_series,
             self._quality_series,
             self._frequency,
             show=show,
         )
+        return fig
 
     def plot_gaps(self, span=None, show=True):
         """
         Plot gaps in the data.
 
         Parameters
         ----------
@@ -1389,15 +1355,15 @@
 
     def to_xml_data_structure(self, standard=True, quality=True, check=True):
         """
         Convert Processor object data to a list of XML data structures.
 
         Returns
         -------
-        list of xml_data_structure.DataSourceBlob
+        list of data_structure.DataSourceBlob
             List of DataSourceBlob instances representing the data in the Processor
             object.
 
         Notes
         -----
         This method converts the data in the Processor object, including standard,
         check, and quality series, into a list of DataSourceBlob instances. Each
@@ -1415,44 +1381,46 @@
         selections = [standard, quality, check]
         dtypes = ["standard", "quality", "check"]
         blobs = [
             self.raw_standard_blob,
             self.raw_quality_blob,
             self.raw_check_blob,
         ]
-        selected_types = [dt for sel, dt in zip(selections, dtypes) if sel]
-        selected_blobs = [blob for sel, blob in zip(selections, blobs) if sel]
+        selected_types = [dt for sel, dt in zip(selections, dtypes, strict=True) if sel]
+        selected_blobs = [
+            blob for sel, blob in zip(selections, blobs, strict=True) if sel
+        ]
 
-        for dtype, raw_blob in zip(selected_types, selected_blobs):
+        for dtype, raw_blob in zip(selected_types, selected_blobs, strict=True):
             if raw_blob is None:
                 raise ValueError(
-                    "Can't reconstruct the data structure without having an xml import"
+                    f"Can't reconstruct the {dtype} data structure without having an xml import"
                     " to mimic."
                 )
             if (
                 hasattr(raw_blob, "data_source")
                 and raw_blob.data_source is not None
                 and hasattr(raw_blob.data_source, "item_info")
                 and (raw_blob.data_source.item_info) is not None
             ):
                 item_info_list = []
                 for i, info in enumerate(raw_blob.data_source.item_info):
-                    item_info = xml_data_structure.ItemInfo(
+                    item_info = data_structure.ItemInfo(
                         item_number=i,
                         item_name=info.item_name,
                         item_format=info.item_format,
                         divisor=info.divisor,
                         units=info.units,
                         format=info.format,
                     )
                     item_info_list += [item_info]
             else:
                 item_info_list = []
 
-            data_source = xml_data_structure.DataSource(
+            data_source = data_structure.DataSource(
                 name=self._standard_measurement_name,
                 num_items=raw_blob.data_source.num_items,
                 ts_type=raw_blob.data_source.ts_type,
                 data_type=raw_blob.data_source.data_type,
                 interpolation=raw_blob.data_source.interpolation,
                 item_format=raw_blob.data_source.item_format,
                 item_info=raw_blob.data_source.item_info,
@@ -1472,26 +1440,24 @@
                     timeseries = self._quality_series
                 else:
                     raise TypeError(
                         "Quality Series should be pd.Series, "
                         f"found {type(self._quality_series)}"
                     )
             elif dtype == "check":
-                if isinstance(self._check_data, pd.DataFrame):
-                    timeseries = self._check_data
+                if isinstance(self._check_series, pd.Series):
+                    timeseries = self.raw_check_data
+                    timeseries[self.check_item_name] = self._check_series
                 else:
                     raise TypeError(
-                        "Check Data should be pd.DataFrame, "
-                        f"found {type(self._check_data)}"
+                        "Check Data should be pd.Series, "
+                        f"found {type(self._check_series)}"
                     )
             else:
                 raise ValueError("No data found for export.")
-            # timeseries.index = utils.datetime_index_to_mowsecs(
-            #     timeseries.index
-            # )
             if (
                 hasattr(raw_blob.data_source, "item_info")
                 and raw_blob.data_source.item_info is not None
             ):
                 for i, info in enumerate(raw_blob.data_source.item_info):
                     if info.item_format == "F":
                         pattern = re.compile(r"#+\.?(#*)")
@@ -1505,21 +1471,21 @@
                             timeseries.iloc[:, i] = timeseries.iloc[:, i].map(
                                 lambda x, f=float_format: f.format(x)
                             )
                         elif isinstance(timeseries, pd.Series):
                             timeseries = timeseries.map(
                                 lambda x, f=float_format: f.format(x)
                             )
-            data = xml_data_structure.Data(
+            data = data_structure.Data(
                 date_format=raw_blob.data.date_format,
                 num_items=raw_blob.data.num_items,
                 timeseries=timeseries,
             )
 
-            data_blob = xml_data_structure.DataSourceBlob(
+            data_blob = data_structure.DataSourceBlob(
                 site_name=raw_blob.site_name,
                 data_source=data_source,
                 data=data,
             )
 
             data_blob_list += [data_blob]
         return data_blob_list
```

### Comparing `hydrobot-0.4.0/hydrobot/xml_data_structure.py` & `hydrobot-0.5.0/hydrobot/data_structure.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """DataSourceBlob Object."""
 import re
+import warnings
 from xml.etree import ElementTree
 
 import pandas as pd
 from defusedxml import ElementTree as DefusedElementTree
 
 
 class ItemInfo:
@@ -81,15 +82,15 @@
         """
         if isinstance(source, str):
             # If the source is a string, treat it as raw XML
             root = DefusedElementTree.fromstring(source)
         elif isinstance(source, ElementTree.Element):
             # If the source is an ElementTree object, use it directly
             root = source
-        elif isinstance(source, (bytes, bytearray)):
+        elif isinstance(source, bytes | bytearray):
             # If the source is a bytes or bytearray, assume it's
             # XML content and decode it.
             root = DefusedElementTree.fromstring(source.decode())
         elif hasattr(source, "read"):
             # If the source has a 'read' method, treat it as a
             # file-like object.
             root = DefusedElementTree.parse(source).getroot()
@@ -250,15 +251,15 @@
         """
         if isinstance(source, str):
             # If the source is a string, treat it as raw XML
             root = DefusedElementTree.fromstring(source)
         elif isinstance(source, ElementTree.Element):
             # If the source is an ElementTree object, use it directly
             root = source
-        elif isinstance(source, (bytes, bytearray)):
+        elif isinstance(source, bytes | bytearray):
             # If the source is a bytes or bytearray, assume it's
             # XML content and decode it.
             root = DefusedElementTree.fromstring(source.decode())
         elif hasattr(source, "read"):
             # If the source has a 'read' method, treat it as a
             # file-like object.
             root = DefusedElementTree.parse(source).getroot()
@@ -276,31 +277,48 @@
         ts_type = root.findtext("TSType")
         data_type = root.findtext("DataType")
         interpolation = root.findtext("Interpolation")
         item_format = root.findtext("ItemFormat")
 
         item_infos_raw = root.findall("ItemInfo")
         if (len(item_infos_raw) != num_items) and (num_items > 1):
-            raise ValueError(
+            warnings.warn(
                 f"Malformed Hilltop XML. DataSource {name} expects {num_items} "
-                f"ItemInfo(s), but found {len(item_infos_raw)}"
+                f"ItemInfo(s), but found {len(item_infos_raw)}",
+                stacklevel=1,
             )
 
+        # Hilltop sometimes sends more item infos than it actually has items.
+        # To account for this we need to sort the item infos by item number,
+        # then only select the first num_items item infos.
+
         item_info_list = []
         for info in item_infos_raw:
             item_info_list += [ItemInfo.from_xml(info)]
 
+        info_dict = {}
+        for item_info in item_info_list:
+            info_dict[item_info.item_number] = item_info
+
+        sorted_item_nums = sorted(list(info_dict.keys()))
+        final_info_list = []
+        if len(info_dict) > 0:
+            for i in range(num_items):
+                final_info_list += [info_dict[sorted_item_nums[i]]]
+        else:
+            final_info_list = []
+
         return cls(
             name,
             num_items,
             str(ts_type),
             str(data_type),
             str(interpolation),
             str(item_format),
-            item_info_list,
+            final_info_list,
         )
 
     def to_xml_tree(self):
         """
         Convert the DataSource instance to an XML ElementTree.
 
         Returns
@@ -435,15 +453,15 @@
         """
         if isinstance(source, str):
             # If the source is a string, treat it as raw XML
             root = DefusedElementTree.fromstring(source)
         elif isinstance(source, ElementTree.Element):
             # If the source is an ElementTree object, use it directly
             root = source
-        elif isinstance(source, (bytes, bytearray)):
+        elif isinstance(source, bytes | bytearray):
             # If the source is a bytes or bytearray, assume it's
             # XML content and decode it.
             root = DefusedElementTree.fromstring(source.decode())
         elif hasattr(source, "read"):
             # If the source has a 'read' method, treat it as a
             # file-like object.
             root = DefusedElementTree.parse(source).getroot()
@@ -470,14 +488,16 @@
                 if child.text is not None:
                     timestamp, data_val = child.text.split(" ")
                     data_dict = {
                         "T": timestamp,
                         "V": data_val,
                     }
                     data_list += [data_dict]
+            elif child.tag == "Gap":
+                pass
             else:
                 raise ValueError(
                     "Possibly Malformed XML: Data items not tagged with 'E' or 'V'."
                 )
 
         if num_items > 1:
             timeseries = pd.DataFrame(data_list).set_index("T")
@@ -517,38 +537,52 @@
             "Data",
             attrib={
                 "DateFormat": self.date_format,
                 "NumItems": str(self.num_items),
             },
         )
 
-        if self.num_items == 1:
-            if isinstance(self.timeseries, pd.Series):
-                for idx, val in self.timeseries.items():
-                    element = ElementTree.SubElement(data_root, "V")
-                    element.text = f"{idx} {val}"
-            else:
-                raise TypeError(
-                    "pandas Series expected for data with single field."
-                    f" Found {type(self.timeseries)}."
-                )
-        else:
-            if isinstance(self.timeseries, pd.DataFrame):
-                for date, row in self.timeseries.iterrows():
+        if isinstance(self.timeseries, pd.Series):
+            for date, val in self.timeseries.items():
+                if pd.isna(val):
+                    element = ElementTree.SubElement(data_root, "Gap")
+                else:
+                    element = ElementTree.SubElement(data_root, "E")
+                    timestamp = ElementTree.SubElement(element, "T")
+                    timestamp.text = str(date)
+                    val_item = ElementTree.SubElement(element, "I1")
+                    val_item.text = str(val)
+        elif isinstance(self.timeseries, pd.DataFrame):
+            for date, row in self.timeseries.iterrows():
+                if pd.isna(row).all():
+                    # If all values in a row are NaNs, insert a Gap.
+                    element = ElementTree.SubElement(data_root, "Gap")
+                else:
                     element = ElementTree.SubElement(data_root, "E")
                     timestamp = ElementTree.SubElement(element, "T")
                     timestamp.text = str(date)
                     for i, val in enumerate(row):
+                        # If only one field in the element is a NaN, leave it blank?
                         val_item = ElementTree.SubElement(element, f"I{i+1}")
-                        val_item.text = str(val)
+                        if not pd.isna(val):
+                            val_item.text = str(val)
+
+        # Collapse all duplicate Gap tags into a single Gap marker:
+        current_gap_count = 0
+        gaps_to_remove = []
+        for elem in data_root:
+            if elem.tag == "Gap":
+                current_gap_count += 1
+                if current_gap_count > 1:
+                    gaps_to_remove.append(elem)
             else:
-                raise TypeError(
-                    "pandas DataFrame expected for data with multiple fields."
-                    f" Found {type(self.timeseries)}."
-                )
+                current_gap_count = 0
+        for gap in gaps_to_remove:
+            data_root.remove(gap)
+
         return data_root
 
     def __repr__(self):
         """Overwriting the __repr__ to mimic xml tree structure."""
         repr = f"""
     <Data DateFormat="{self.date_format}" NumItems="{self.num_items}">
         """
@@ -672,15 +706,15 @@
         """
         if isinstance(source, str):
             # If the source is a string, treat it as raw XML
             root = DefusedElementTree.fromstring(source)
         elif isinstance(source, ElementTree.Element):
             # If the source is an ElementTree object, use it directly
             root = source
-        elif isinstance(source, (bytes, bytearray)):
+        elif isinstance(source, bytes | bytearray):
             # If the source is a bytes or bytearray, assume it's
             # XML content and decode it.
             root = DefusedElementTree.fromstring(source.decode())
         elif hasattr(source, "read"):
             # If the source has a 'read' method, treat it as a
             # file-like object.
             root = DefusedElementTree.parse(source).getroot()
@@ -789,30 +823,35 @@
         root = DefusedElementTree.fromstring(source)
     elif isinstance(source, ElementTree.Element):
         # If the source is an Element object, use it directly as root
         root = source
     elif isinstance(source, ElementTree.ElementTree):
         # If the source is an ElementTree object, get the root
         root = source.getroot()
-    elif isinstance(source, (bytes, bytearray)):
+    elif isinstance(source, bytes | bytearray):
         # If the source is a bytes or bytearray, assume it's
         # XML content and decode it.
         root = DefusedElementTree.fromstring(source.decode())
     elif hasattr(source, "read"):
         # If the source has a 'read' method, treat it as a
         # file-like object.
         root = DefusedElementTree.parse(source).getroot()
     else:
         raise ValueError("Unsupported XML source type.")
 
     if root.tag == "HilltopServer":
         ElementTree.indent(root, space="\t")
         print("Hilltop xml possibly returned no data. Check for yourself:")
         ElementTree.dump(root)
-        return None
+        err_text = root.findtext("Error")
+        if "No data from " in str(err_text):
+            warnings.warn(str(err_text), stacklevel=1)
+            return None
+        else:
+            raise ValueError(err_text)
     elif root.tag != "Hilltop":
         raise ValueError(
             f"Possibly malformed Hilltop xml. Root tag is '{root.tag}',"
             " should be 'Hilltop'."
         )
     data_source_blob_list = []
     for child in root.iter():
@@ -826,36 +865,43 @@
                     info.item_name for info in data_source_blob.data_source.item_info
                 ]
                 item_numbers = [
                     int(info.item_number)
                     for info in data_source_blob.data_source.item_info
                 ]
 
-                sorted_pairs = sorted(zip(item_numbers, item_names), key=lambda x: x[0])
+                sorted_pairs = sorted(
+                    zip(item_numbers, item_names, strict=True), key=lambda x: x[0]
+                )
                 sorted_items = sorted(
-                    zip(item_numbers, data_source_blob.data_source.item_info),
+                    zip(
+                        item_numbers,
+                        data_source_blob.data_source.item_info,
+                        strict=True,
+                    ),
                     key=lambda x: x[0],
                 )
 
-                _, sorted_item_names = zip(*sorted_pairs)
-                _, sorted_item_list = zip(*sorted_items)
+                _, sorted_item_names = zip(*sorted_pairs, strict=True)
+                _, sorted_item_list = zip(*sorted_items, strict=True)
 
                 sorted_item_names = list(sorted_item_names)
                 data_source_blob.data_source.item_info = list(sorted_item_list)
 
             else:
                 sorted_item_names = []
             if len(sorted_item_names) > 1 and isinstance(
                 data_source_blob.data.timeseries, pd.DataFrame
             ):
                 cols = {
                     col: name
                     for col, name in zip(
                         data_source_blob.data.timeseries.columns,
                         sorted_item_names,
+                        strict=True,
                     )
                 }
                 data_source_blob.data.timeseries = (
                     data_source_blob.data.timeseries.rename(columns=cols)
                 )
             elif len(sorted_item_names) > 0:
                 data_source_blob.data.timeseries.name = sorted_item_names[0]
```

### Comparing `hydrobot-0.4.0/hydrobot.egg-info/SOURCES.txt` & `hydrobot-0.5.0/hydrobot.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -29,49 +29,48 @@
 docs/usage.rst
 docs/_build/html/_static/file.png
 docs/_build/html/_static/minus.png
 docs/_build/html/_static/plus.png
 hydrobot/__init__.py
 hydrobot/data_acquisition.py
 hydrobot/data_sources.py
+hydrobot/data_structure.py
 hydrobot/evaluator.py
 hydrobot/filters.py
 hydrobot/plotter.py
 hydrobot/processor.py
 hydrobot/utils.py
-hydrobot/xml_data_structure.py
 hydrobot.egg-info/PKG-INFO
 hydrobot.egg-info/SOURCES.txt
 hydrobot.egg-info/dependency_links.txt
 hydrobot.egg-info/requires.txt
 hydrobot.egg-info/top_level.txt
 hydrobot/config/QualityCodeEvaluator_QC_config.csv
 hydrobot/config/TwoLevelQualityCodeEvaluator_QC_config.csv
 prototypes/Class_script.py
 prototypes/site_list_reader.py
 prototypes/site_parameters.json
-prototypes/Jupyter_notebooks/All_Sites_Atmospheric_Pressure.ipynb
-prototypes/Jupyter_notebooks/Saddle_Road_Spike_Removal.ipynb
-prototypes/Jupyter_notebooks/Time_Series_Analysis.ipynb
 prototypes/output_dump/.gitignore
 prototypes/py_scripts/atmospheric_spike_removal.py
 prototypes/py_scripts/example_plot_script.py
 prototypes/py_scripts/gap_finder.py
 prototypes/py_scripts/new_ws_plot_with_check_data.py
 prototypes/py_scripts/plot_with_check_data.py
 prototypes/py_scripts/process_script.py
 prototypes/py_scripts/spike_removal_util.py
 prototypes/py_scripts/stage_full_process.py
 prototypes/py_scripts/water_temp_full_process.py
 prototypes/py_scripts/water_temp_spike_removal.py
 prototypes/py_scripts/output_dump/.gitignore
+prototypes/script_dump/.gitignore
 tests/.coverage
 tests/__init__.py
 tests/conftest.py
 tests/site_list_response.xml
 tests/test_data_sources.py
+tests/test_data_structure.py
 tests/test_evaluator.py
 tests/test_filters.py
-tests/test_integration.py
 tests/test_processor.py
-tests/test_xml_data_structure.py
+tests/test_utils.py
+tests/test_web_integration.py
 tests/xml_test_data_file.xml
```

### Comparing `hydrobot-0.4.0/old_setup.py` & `hydrobot-0.5.0/old_setup.py`

 * *Files identical despite different names*

### Comparing `hydrobot-0.4.0/prototypes/py_scripts/atmospheric_spike_removal.py` & `hydrobot-0.5.0/prototypes/py_scripts/atmospheric_spike_removal.py`

 * *Files identical despite different names*

### Comparing `hydrobot-0.4.0/prototypes/py_scripts/example_plot_script.py` & `hydrobot-0.5.0/prototypes/py_scripts/example_plot_script.py`

 * *Files identical despite different names*

### Comparing `hydrobot-0.4.0/prototypes/py_scripts/gap_finder.py` & `hydrobot-0.5.0/prototypes/py_scripts/gap_finder.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 idx0 = np.flatnonzero(np.r_[True, np.diff(np.isnan(base_data["Value"])) != 0, True])
 count = np.diff(idx0)
 idx = idx0[:-1]
 valid_mask = np.isnan(base_data["Value"][idx])
 out_idx = idx[valid_mask]
 out_count = count[valid_mask]
-out = zip(base_data.index[out_idx], out_count)
+out = zip(base_data.index[out_idx], out_count, strict=True)
 print([o for o in out])
 
 
 nans = base_data[base_data["Value"].isna()]
 fake_nans = nans
 fake_nans["Value"] = 1000
```

### Comparing `hydrobot-0.4.0/prototypes/py_scripts/new_ws_plot_with_check_data.py` & `hydrobot-0.5.0/prototypes/py_scripts/new_ws_plot_with_check_data.py`

 * *Files identical despite different names*

### Comparing `hydrobot-0.4.0/prototypes/py_scripts/plot_with_check_data.py` & `hydrobot-0.5.0/prototypes/py_scripts/plot_with_check_data.py`

 * *Files identical despite different names*

### Comparing `hydrobot-0.4.0/prototypes/py_scripts/process_script.py` & `hydrobot-0.5.0/prototypes/py_scripts/process_script.py`

 * *Files identical despite different names*

### Comparing `hydrobot-0.4.0/prototypes/py_scripts/spike_removal_util.py` & `hydrobot-0.5.0/prototypes/py_scripts/spike_removal_util.py`

 * *Files identical despite different names*

### Comparing `hydrobot-0.4.0/prototypes/py_scripts/stage_full_process.py` & `hydrobot-0.5.0/prototypes/py_scripts/stage_full_process.py`

 * *Files identical despite different names*

### Comparing `hydrobot-0.4.0/prototypes/py_scripts/water_temp_full_process.py` & `hydrobot-0.5.0/prototypes/py_scripts/water_temp_full_process.py`

 * *Files identical despite different names*

### Comparing `hydrobot-0.4.0/prototypes/py_scripts/water_temp_spike_removal.py` & `hydrobot-0.5.0/prototypes/py_scripts/water_temp_spike_removal.py`

 * *Files identical despite different names*

### Comparing `hydrobot-0.4.0/prototypes/site_list_reader.py` & `hydrobot-0.5.0/prototypes/site_list_reader.py`

 * *Files identical despite different names*

### Comparing `hydrobot-0.4.0/pyproject.toml` & `hydrobot-0.5.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hydrobot"
 description = "A suite of processing tools for Hilltop hydrological data."
-version = "0.4.0"
+version = "0.5.0"
 authors = [
     { name = "Nic Mostert", email = "nicolas.mostert@horizons.govt.nz" },
     { name = "Sam Irvine", email = "sam.irvine@horizons.govt.nz" }
 ]
-requires-python = "==3.11.6"
+requires-python = "==3.11.*"
 dependencies = [
     "hilltop-py>=2.3.1",
-    "data-annalist>=0.3.6",
+    "data-annalist>=0.4.1",
     "matplotlib>=3.8.0",
-    "defusedxml>=0.7.1"
+    "defusedxml>=0.7.1",
+    "plotly>=5.20.0"
 ]
 classifiers=[
-    "Development Status :: 2 - Pre-Alpha",
+    "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Natural Language :: English",
     "Programming Language :: Python :: 3.11",
 ]
 license = {text = "GNU General Public License v3"}
 readme = "README.rst"
@@ -95,15 +96,15 @@
 
 [tool.ruff.per-file-ignores]
 "tests/*" = ["S311", "S101", "F841"]
 "docs/*" = ["I001"]
 "prototypes" = ["D"]
 
 [tool.bumpversion]
-current_version = "0.4.0"
+current_version = "0.5.0"
 commit = true
 tag = true
 tag_name = "{new_version}"
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = "{current_version}"
```

### Comparing `hydrobot-0.4.0/requirements_dev.txt` & `hydrobot-0.5.0/requirements_dev.txt`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,15 @@
 pathtools==0.1.2
 patsy==0.5.3
 pexpect==4.8.0
 pickleshare==0.7.5
 Pillow==10.0.1
 pkginfo==1.9.6
 platformdirs==3.10.0
+plotly==5.20.0
 pluggy==1.3.0
 pre-commit==3.5.0
 prompt-toolkit==3.0.39
 psutil==5.9.5
 ptyprocess==0.7.0
 pure-eval==0.2.2
 py==1.11.0
```

### Comparing `hydrobot-0.4.0/tests/.coverage` & `hydrobot-0.5.0/tests/.coverage`

 * *Files 11% similar despite different names*

#### sqlite3 {} .dump

```diff
@@ -12,34 +12,39 @@
     unique (key)
     -- Possible keys:
     --  'has_arcs' boolean      -- Is this data recording branches?
     --  'sys_argv' text         -- The coverage command line that recorded the data.
     --  'version' text          -- The version of coverage.py that made the file.
     --  'when' text             -- Datetime when the file was created.
 );
-INSERT INTO meta VALUES('version','7.3.2');
+INSERT INTO meta VALUES('version','7.3.1');
 INSERT INTO meta VALUES('has_arcs','0');
 CREATE TABLE file (
     -- A row per file measured.
     id integer primary key,
     path text,
     unique (path)
 );
 INSERT INTO file VALUES(1,'/home/nic/repos/hydrobot/tests/__init__.py');
-INSERT INTO file VALUES(2,'/home/nic/repos/hydrobot/tests/test_data_sources.py');
-INSERT INTO file VALUES(3,'/home/nic/repos/hydrobot/hydrobot/__init__.py');
-INSERT INTO file VALUES(4,'/home/nic/repos/hydrobot/hydrobot/data_sources.py');
-INSERT INTO file VALUES(5,'/home/nic/repos/hydrobot/tests/test_evaluator.py');
-INSERT INTO file VALUES(6,'/home/nic/repos/hydrobot/hydrobot/evaluator.py');
-INSERT INTO file VALUES(7,'/home/nic/repos/hydrobot/tests/test_filters.py');
-INSERT INTO file VALUES(8,'/home/nic/repos/hydrobot/hydrobot/filters.py');
-INSERT INTO file VALUES(9,'/home/nic/repos/hydrobot/tests/test_processor.py');
-INSERT INTO file VALUES(10,'/home/nic/repos/hydrobot/hydrobot/processor.py');
-INSERT INTO file VALUES(11,'/home/nic/repos/hydrobot/hydrobot/data_acquisition.py');
-INSERT INTO file VALUES(12,'/home/nic/repos/hydrobot/hydrobot/plotter.py');
+INSERT INTO file VALUES(2,'/home/nic/repos/hydrobot/tests/conftest.py');
+INSERT INTO file VALUES(3,'/home/nic/repos/hydrobot/tests/test_data_sources.py');
+INSERT INTO file VALUES(4,'/home/nic/repos/hydrobot/hydrobot/__init__.py');
+INSERT INTO file VALUES(5,'/home/nic/repos/hydrobot/hydrobot/data_sources.py');
+INSERT INTO file VALUES(6,'/home/nic/repos/hydrobot/tests/test_evaluator.py');
+INSERT INTO file VALUES(7,'/home/nic/repos/hydrobot/hydrobot/evaluator.py');
+INSERT INTO file VALUES(8,'/home/nic/repos/hydrobot/tests/test_filters.py');
+INSERT INTO file VALUES(9,'/home/nic/repos/hydrobot/hydrobot/filters.py');
+INSERT INTO file VALUES(10,'/home/nic/repos/hydrobot/tests/test_integration.py');
+INSERT INTO file VALUES(11,'/home/nic/repos/hydrobot/hydrobot/processor.py');
+INSERT INTO file VALUES(12,'/home/nic/repos/hydrobot/hydrobot/data_acquisition.py');
+INSERT INTO file VALUES(13,'/home/nic/repos/hydrobot/hydrobot/xml_data_structure.py');
+INSERT INTO file VALUES(14,'/home/nic/repos/hydrobot/hydrobot/plotter.py');
+INSERT INTO file VALUES(15,'/home/nic/repos/hydrobot/hydrobot/utils.py');
+INSERT INTO file VALUES(16,'/home/nic/repos/hydrobot/tests/test_processor.py');
+INSERT INTO file VALUES(17,'/home/nic/repos/hydrobot/tests/test_xml_data_structure.py');
 CREATE TABLE context (
     -- A row per context measured.
     id integer primary key,
     context text,
     unique (context)
 );
 INSERT INTO context VALUES(1,'');
@@ -50,25 +55,30 @@
     context_id integer,         -- foreign key to `context`.
     numbits blob,               -- see the numbits functions in coverage.numbits
     foreign key (file_id) references file (id),
     foreign key (context_id) references context (id),
     unique (file_id, context_id)
 );
 INSERT INTO line_bits VALUES(1,1,X'02');
-INSERT INTO line_bits VALUES(2,1,X'd6ec942d');
-INSERT INTO line_bits VALUES(3,1,X'3a');
-INSERT INTO line_bits VALUES(4,1,X'de2c002e02007e86400000e4050000002030eedcbf120038f007');
-INSERT INTO line_bits VALUES(5,1,X'f0b69fffcff38fcd66b3793f9b99cdcb36b66dd9c6b62def3c63e07fff1903fffbcff50d');
-INSERT INTO line_bits VALUES(6,1,X'760900e02f0100803b260000b006cf0900807b9e120000f026008077020060020040020000000000800000000010');
-INSERT INTO line_bits VALUES(7,1,X'7aede7c72081211dc87492a4e498bc1ce00c');
-INSERT INTO line_bits VALUES(8,1,X'ba04004812009024010080480600004002');
-INSERT INTO line_bits VALUES(9,1,X'f62a085836d964fb9f846dddcfde02');
-INSERT INTO line_bits VALUES(10,1,X'daab1f0100000000b0fd8f795b00070ef87b5ac738c6318e718c631ce318c77ae38d639fff2e7eff5bfc0600003a33c00018000c00ec01000c4080000201');
-INSERT INTO line_bits VALUES(11,1,X'ba04020000402310000000fe7d02');
-INSERT INTO line_bits VALUES(12,1,X'56020000000004000000000020000040');
+INSERT INTO line_bits VALUES(2,1,X'660000c0');
+INSERT INTO line_bits VALUES(3,1,X'aed9295b');
+INSERT INTO line_bits VALUES(4,1,X'3a');
+INSERT INTO line_bits VALUES(5,1,X'de2c002e02007e86400000e4050010e02030eef2fd9b00c0817f0000f0efdf3ffe000080ff13c0b7b73f');
+INSERT INTO line_bits VALUES(6,1,X'e26d3fff9fe71f9bcd66b3fdccccccbcd4c6b62db5b16d4b779e62e07fff2906fef79fd64fef0d');
+INSERT INTO line_bits VALUES(7,1,X'762500807f090000dc313f000070ff0dc08f0c0100703f9e12000000781300c03b010030010020010000f8e3bc080000ff4c0200c81f00009c');
+INSERT INTO line_bits VALUES(8,1,X'f6dacfcfff8f41020c1912804c27494a8ec94300c0f4ed6edbf4dc9e75a6d66ddbd66ddbb62d');
+INSERT INTO line_bits VALUES(9,1,X'7209002051040048920000402407000020211f000000f84e0000d81c0000d803');
+INSERT INTO line_bits VALUES(10,1,X'f626000000f8ff0ffe5355d5b6f2a7aa6a5bf1a7aa6a5b09000000f8ff8ff3fc9fb7b66050e2494b5ad28a3822000000c0ff7f9ce7ff');
+INSERT INTO line_bits VALUES(11,1,X'ba2f80fe080000000000b6ff010000802c5b0017706f807fbfff690c1a3468c0800103c63160bdf5d637e8db010000000000f0cf0178f7ef3e1086038007b88176000000000000ff0c58f0740fc25000783b0000000000c0bf011b7cca0f84a100f7c7c03ef4030000001800f8330000008f03000080ff31000000e07d0c0000000000f600000000f0ef80cd38000000007011060000683e0000003cfcfb770500804f0001080000002000000000020000fe367cffc53f070e0ec0fd8f7b9e01');
+INSERT INTO line_bits VALUES(12,1,X'ea4a20000000fca71218');
+INSERT INTO line_bits VALUES(13,1,X'6ed60f0000f80d000000a400187c050080d9b61500ac3f000000ff18000000480170f006f74f0000009c6ded0a00c03a0000370000009002e0e01700ec150000f0f1817f5000000000000000eb0100f00600000052000cb415000036540002000000480b801fde769e8d7d369600000000e0dd04');
+INSERT INTO line_bits VALUES(14,1,X'56020000000004000000000020000040000000000030');
+INSERT INTO line_bits VALUES(15,1,X'5a0200000010');
+INSERT INTO line_bits VALUES(16,1,X'd4ef0a82c0b2c92603000b060000100000000000400000000000000000000000000002000000000000000000000080000000000000000000000000000000000008');
+INSERT INTO line_bits VALUES(17,1,X'ea32000060103cff4a00000001100000400004000010000100000480000080');
 CREATE TABLE arc (
     -- If recording branches, a row per context per from/to line transition executed.
     file_id integer,            -- foreign key to `file`.
     context_id integer,         -- foreign key to `context`.
     fromno integer,             -- line number jumped from.
     tono integer,               -- line number jumped to.
     foreign key (file_id) references file (id),
@@ -89,8 +99,13 @@
 INSERT INTO tracer VALUES(6,'');
 INSERT INTO tracer VALUES(7,'');
 INSERT INTO tracer VALUES(8,'');
 INSERT INTO tracer VALUES(9,'');
 INSERT INTO tracer VALUES(10,'');
 INSERT INTO tracer VALUES(11,'');
 INSERT INTO tracer VALUES(12,'');
+INSERT INTO tracer VALUES(13,'');
+INSERT INTO tracer VALUES(14,'');
+INSERT INTO tracer VALUES(15,'');
+INSERT INTO tracer VALUES(16,'');
+INSERT INTO tracer VALUES(17,'');
 COMMIT;
```

### Comparing `hydrobot-0.4.0/tests/conftest.py` & `hydrobot-0.5.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hydrobot-0.4.0/tests/test_evaluator.py` & `hydrobot-0.5.0/tests/test_evaluator.py`

 * *Files identical despite different names*

### Comparing `hydrobot-0.4.0/tests/test_filters.py` & `hydrobot-0.5.0/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `hydrobot-0.4.0/tests/test_processor.py` & `hydrobot-0.5.0/tests/test_processor.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 import numpy as np
 import pandas as pd
 import pytest
 from annalist.annalist import Annalist
 from defusedxml import ElementTree as DefusedElementTree
 from hilltoppy import Hilltop
 
-from hydrobot import data_sources, processor, utils, xml_data_structure
+from hydrobot import data_sources, data_structure, processor, utils
 from hydrobot.data_sources import QualityCodeEvaluator
-from hydrobot.xml_data_structure import parse_xml
+from hydrobot.data_structure import parse_xml
 
 ann = Annalist()
 
 SITES = [
     "Slimy Bog at Dirt Road",
     "Mid Stream at Cowtoilet Farm",
     "Mostly Cowpiss River at Greenwash Pastures",
@@ -240,15 +240,15 @@
 
     pr = processor.Processor(
         base_url="https://greenwashed.and.pleasant/",
         site=SITES[1],
         standard_hts="GreenPasturesAreNaturalAndEcoFriendlyISwear.hts",
         standard_measurement_name=MEASUREMENTS[1],
         check_measurement_name=CHECK_MEASUREMENTS[1],
-        frequency="5T",
+        frequency="5min",
     )
 
     captured = capsys.readouterr()
     ann_output = captured.err.split("\n")
 
     correct = [
         "standard_series | Mid Stream at Cowtoilet Farm",
@@ -338,28 +338,28 @@
 
     # However, in this case, we need to patch the INSTANCE as imported in
     # data_acquisition. Not sure if this makes sense to me, but it works.
     monkeypatch.setattr("hydrobot.data_acquisition.get_hilltop_xml", get_mock_xml_data)
 
     data_source_blob_list = []
 
-    for check, meas in zip(CHECK_MEASUREMENTS, MEASUREMENTS):
+    for check, meas in zip(CHECK_MEASUREMENTS, MEASUREMENTS, strict=True):
         pr = processor.Processor(
             base_url="https://greenwashed.and.pleasant/",
             site=SITES[1],
             standard_hts="GreenPasturesAreNaturalAndEcoFriendlyISwear.hts",
             standard_measurement_name=meas,
             check_measurement_name=check,
-            frequency="5T",
+            frequency="5min",
         )
 
         data_source_blob_list += pr.to_xml_data_structure()
 
     output_path = tmp_path / "output.xml"
-    xml_data_structure.write_hilltop_xml(data_source_blob_list, output_path)
+    data_structure.write_hilltop_xml(data_source_blob_list, output_path)
 
     with open(output_path) as f:
         output_xml = f.read()
 
     with open(sample_data_source_xml_file) as f:
         sample_data_source_xml = f.read()
 
@@ -368,23 +368,23 @@
 
     assert ElementTree.indent(input_tree) == ElementTree.indent(output_tree)
 
     for blob in data_source_blob_list:
         assert blob.site_name == SITES[1]
 
 
-def test_import_range(
+def test_import_data(
     monkeypatch,
     mock_site_list,
     mock_measurement_list,
     mock_get_data,
     mock_qc_evaluator_dict,
 ):
     """
-    Test the import_range method of the Processor class.
+    Test the import_data method of the Processor class.
 
     Parameters
     ----------
     monkeypatch : pytest.MonkeyPatch
         Pytest fixture for monkeypatching.
     mock_site_list : List[str]
         Mocked list of site names.
@@ -393,24 +393,24 @@
     mock_get_data : Callable
         Mocked get_data function.
     mock_qc_evaluator_dict : Dict[str, Any]
         Mocked QC evaluator dictionary.
 
     Notes
     -----
-    This test function checks the import_range method of the Processor class.
+    This test function checks the import_data method of the Processor class.
     It mocks relevant functions and classes for the test.
 
     Assertions
     ----------
     - For each index in standard_series, quality_series, and check_series, it is within
         the specified date range.
-    - The import_range method updates the series with new data and retains existing
+    - The import_data method updates the series with new data and retains existing
         changes without overwriting.
-    - The import_range method overwrites existing data when the 'overwrite' parameter
+    - The import_data method overwrites existing data when the 'overwrite' parameter
         is set to True.
 
     """
 
     def get_mock_site_list(*args, **kwargs):
         _ = args, kwargs
         return mock_site_list
@@ -446,15 +446,15 @@
     to_date = "2023/01/01 00:20"
 
     pr = processor.Processor(
         base_url="https://greenwashed.and.pleasant/",
         site=SITES[1],
         standard_hts="GreenPasturesAreNaturalAndEcoFriendlyISwear.hts",
         standard_measurement_name=MEASUREMENTS[0],
-        frequency="5T",
+        frequency="5min",
         from_date=from_date,
         to_date=to_date,
     )
 
     for idx in pr.standard_series.index:
         assert idx >= pd.to_datetime(from_date)
         assert idx <= pd.to_datetime(to_date)
@@ -463,58 +463,14 @@
         assert idx >= pd.to_datetime(from_date)
         assert idx <= pd.to_datetime(to_date)
 
     for idx in pr.check_series.index:
         assert idx >= pd.to_datetime(from_date)
         assert idx <= pd.to_datetime(to_date)
 
-    # Making changes to the existing series
-    pr.standard_series.iloc[0] = 111
-    pr.quality_series.iloc[0] = 222
-    pr.check_series.iloc[0] = 333
-
-    # Updating processor object with more data to the existing series
-    pr.import_data(
-        from_date=None,
-        to_date=None,
-        standard=True,
-        quality=True,
-        check=True,
-        overwrite=False,
-    )
-
-    # Check that new data is added
-    assert pr.standard_series.index[-1] == pd.to_datetime("2023-01-01 00:45")
-    assert pr.quality_series.index[-1] == pd.to_datetime("2023-01-01 00:00")
-    assert pr.check_series.index[-1] == pd.to_datetime("2023-01-01 00:45")
-
-    # Check that changed data is not overwritten
-    assert (
-        pr.standard_series.iloc[0] == 111
-    ), "The 'overwrite' flag in import_data seems to be broken"
-    assert (
-        pr.quality_series.iloc[0] == 222
-    ), "The 'overwrite' flag in import_data seems to be broken"
-    assert (
-        pr.check_series.iloc[0] == 333
-    ), "The 'overwrite' flag in import_data seems to be broken"
-
-    # Updating processor object again, this time overwriting everything
-    pr.import_data(
-        from_date=None,
-        to_date=None,
-        standard=True,
-        quality=True,
-        check=True,
-        overwrite=True,
-    )
-    assert int(pr.standard_series.iloc[0]) == 10
-    assert int(pr.quality_series.iloc[0]) == 500
-    assert float(pr.check_series.iloc[0]) == 9.0
-
 
 def test_gap_closer(
     monkeypatch,
     mock_site_list,
     mock_measurement_list,
     mock_get_data,
     mock_qc_evaluator_dict,
@@ -588,15 +544,15 @@
     monkeypatch.setattr("hydrobot.data_acquisition.get_data", get_mock_get_data)
 
     pr = processor.Processor(
         base_url="https://greenwashed.and.pleasant/",
         site=SITES[1],
         standard_hts="GreenPasturesAreNaturalAndEcoFriendlyISwear.hts",
         standard_measurement_name=MEASUREMENTS[0],
-        frequency="5T",
+        frequency="5min",
     )
 
     # Checking that the data points I want to delete actually exist:
     start_idx = "2023-01-01 00:20:00"
     end_idx = "2023-01-01 00:25:00"
     assert pd.to_datetime(start_idx) in pr.standard_series
     assert pd.to_datetime(end_idx) in pr.standard_series
@@ -629,7 +585,172 @@
     # Check that gap was closed
     assert (
         pd.to_datetime(start_idx) not in pr.standard_series
     ), "processor.gap_closer appears to be broken."
     assert (
         pd.to_datetime(end_idx) not in pr.standard_series
     ), "processor.gap_closer appears to be broken."
+
+
+def test_data_export(
+    monkeypatch,
+    mock_site_list,
+    mock_measurement_list,
+    mock_get_data,
+    mock_qc_evaluator_dict,
+    tmp_path,
+):
+    """
+    Test the 'gap_closer' method of the Processor class.
+
+    Parameters
+    ----------
+    monkeypatch : pytest.MonkeyPatch
+        Pytest fixture to modify or mock modules during testing.
+    mock_site_list : pytest fixture
+        Mocked response for the site list.
+    mock_measurement_list : pytest fixture
+        Mocked response for the measurement list.
+    mock_get_data : pytest fixture
+        Mock response for the get_data server call method.
+    mock_qc_evaluator_dict : pytest fixture
+        Mocked response for the quality control evaluator dictionary.
+
+    Notes
+    -----
+    - This test checks the functionality of the 'gap_closer' method in the Processor
+        class.
+    - It involves creating a Processor object, making a gap in the data, inserting NaNs,
+        and then closing the gap.
+    - Assertions are made to ensure that the gap is properly created, NaNs are inserted,
+        and the gap is closed.
+
+    Assertions
+    ----------
+    - The data points that are intended to be deleted actually exist before the gap
+        creation.
+    - After creating a small gap, check that the gap was made by confirming the absence
+        of the specified data points.
+    - Check that NaNs are correctly inserted into the specified positions in the data.
+    - After closing the gaps, verify that the specified data points are no longer
+        present in the data.
+
+    """
+
+    def get_mock_site_list(*args, **kwargs):
+        _ = args, kwargs
+        return mock_site_list
+
+    def get_mock_measurement_list(*args, **kwargs):
+        _ = args, kwargs
+        return mock_measurement_list
+
+    def get_mock_get_data(*args, **kwargs):
+        xml, data_func = mock_get_data
+        return xml, data_func(*args, **kwargs)
+
+    def get_mock_qc_evaluator_dict(*args, **kwargs):
+        _ = args, kwargs
+        return mock_qc_evaluator_dict
+
+    ann.configure(stream_format_str="%(function_name)s | %(site)s")
+
+    # Here we patch the Hilltop Class
+    monkeypatch.setattr(Hilltop, "get_site_list", get_mock_site_list)
+    monkeypatch.setattr(Hilltop, "get_measurement_list", get_mock_measurement_list)
+    monkeypatch.setattr(
+        data_sources,
+        "get_qc_evaluator_dict",
+        get_mock_qc_evaluator_dict,
+    )
+
+    # However, in this case, we need to patch the INSTANCE as imported in
+    # data_acquisition. Not sure if this makes sense to me, but it works.
+    monkeypatch.setattr("hydrobot.data_acquisition.get_data", get_mock_get_data)
+
+    pr = processor.Processor(
+        base_url="https://greenwashed.and.pleasant/",
+        site=SITES[1],
+        standard_hts="GreenPasturesAreNaturalAndEcoFriendlyISwear.hts",
+        standard_measurement_name=MEASUREMENTS[0],
+        frequency="5min",
+    )
+
+    # Checking that the data points I want to delete actually exist:
+    start_idx = "2023-01-01 00:20:00"
+    end_idx = "2023-01-01 00:25:00"
+    assert pd.to_datetime(start_idx) in pr.standard_series
+    assert pd.to_datetime(end_idx) in pr.standard_series
+
+    # =======================Make a small gap========================
+    print("Gappy Chappy")
+    pr.delete_range(start_idx, end_idx)
+
+    gap_path_csv = tmp_path / "gap_output.csv"
+    gap_path_hilltop_csv = tmp_path / "gap_output_hilltop"
+    gap_path_xml = tmp_path / "gap_output.xml"
+
+    pr.data_exporter(gap_path_csv, ftype="csv")
+
+    read_csv_df = pd.read_csv(gap_path_csv)
+    # Check that the csv was filled in with nans where there are no quality values
+    assert pd.isna(read_csv_df["General Nastiness [Quality]"].iloc[1])
+
+    # The hilltop_csv format outputs two files:
+    # one for standard and qc together,
+    # and one for check data alone.
+    pr.data_exporter(gap_path_hilltop_csv, ftype="hilltop_csv")
+    hilltop_path_std_qc = tmp_path / "gap_output_hilltop_std_qc.csv"
+    hilltop_path_check = tmp_path / "gap_output_hilltop_check.csv"
+
+    read_hilltop_std_qc_csv_df = pd.read_csv(hilltop_path_std_qc)
+    read_hilltop_check_csv_df = pd.read_csv(hilltop_path_check)
+
+    # Check that the deleted values have not been filled somehow
+    assert start_idx not in list(read_hilltop_std_qc_csv_df.index)
+    assert start_idx not in list(read_hilltop_check_csv_df.index)
+
+    print("Before xml export:", pr.quality_series.index)
+    pr.data_exporter(gap_path_xml, ftype="xml")
+    print("After xml export:", pr.quality_series.index)
+    gap_path_xml_tree = DefusedElementTree.fromstring(gap_path_xml.read_text())
+    gap_path_blob = data_structure.parse_xml(gap_path_xml_tree)
+
+    std_indices = gap_path_blob[0].data.timeseries.index
+    assert pd.Timestamp(start_idx) not in list(std_indices)
+
+    # =======================Insert Nans========================
+    # This is how we internally represent gaps. They need to be converted to the Gap
+    # tag for xml export.
+    print("Before nans:", pr.quality_series.index)
+    pr.insert_missing_nans()
+    print("After nans:", pr.quality_series.index)
+
+    pr.data_exporter(gap_path_csv, ftype="csv")
+
+    read_csv_df = pd.read_csv(gap_path_csv)
+    # Check that the csv was filled in with nans where there are no quality values
+    # assert pd.isna(read_csv_df["General Nastiness [Quality]"].iloc[1])
+
+    # The hilltop_csv format outputs two files:
+    # one for standard and qc together,
+    # and one for check data alone.
+    pr.data_exporter(gap_path_hilltop_csv, ftype="hilltop_csv")
+
+    read_hilltop_std_qc_csv_df = pd.read_csv(hilltop_path_std_qc)
+    read_hilltop_check_csv_df = pd.read_csv(hilltop_path_check)
+
+    # Check that the deleted values have not been filled somehow
+    # assert start_idx not in list(read_hilltop_std_qc_csv_df.index)
+    # assert start_idx not in list(read_hilltop_check_csv_df.index)
+    print(read_hilltop_std_qc_csv_df)
+    print(read_hilltop_check_csv_df)
+    # assert start_idx not in list(read_hilltop_std_qc_csv_df.index)
+
+    pr.data_exporter(gap_path_xml, ftype="xml")
+
+    print(gap_path_xml.read_text())
+    gap_path_xml_tree = DefusedElementTree.fromstring(gap_path_xml.read_text())
+    gap_path_blob = data_structure.parse_xml(gap_path_xml_tree)
+
+    std_indices = gap_path_blob[0].data.timeseries.index
+    assert start_idx not in list(std_indices)
```

### Comparing `hydrobot-0.4.0/tests/test_xml_data_structure.py` & `hydrobot-0.5.0/tests/test_data_structure.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from xml.etree import ElementTree
 
 import pandas as pd
 import pytest
 from defusedxml import ElementTree as DefusedElementTree
 
-from hydrobot import xml_data_structure
+from hydrobot import data_structure
 
 
 @pytest.fixture()
 def correct_blobs():
     """
     PyTest fixture providing a list of correct DataSourceBlob dictionaries for testing.
 
@@ -51,15 +51,15 @@
         pd.Series,
         pd.Series,
         pd.DataFrame,
     ]
 
     blob_list = []
     for ds in datasources:
-        for ts, dt in zip(tstypes, data_types):
+        for ts, dt in zip(tstypes, data_types, strict=True):
             blob = {
                 "site_name": sitename,
                 "data_source_name": ds,
                 "ts_type": ts,
                 "data_type": dt,
             }
             blob_list.append(blob)
@@ -92,15 +92,15 @@
       matches the corresponding value in the correct_blobs list.
     - For each parsed DataSourceBlob instance, assert that the 'data_source.ts_type'
       matches the corresponding value in the correct_blobs list.
     """
     with open(sample_data_source_xml_file) as f:
         sample_data_source_xml = f
 
-        blob_list = xml_data_structure.parse_xml(sample_data_source_xml)
+        blob_list = data_structure.parse_xml(sample_data_source_xml)
 
         for i, blob in enumerate(blob_list):
             assert blob.site_name == correct_blobs[i]["site_name"]
             assert blob.data_source.name == correct_blobs[i]["data_source_name"]
             assert blob.data_source.ts_type == correct_blobs[i]["ts_type"]
             assert isinstance(blob.data.timeseries, correct_blobs[i]["data_type"])
 
@@ -130,15 +130,15 @@
       matches the corresponding value in the correct_blobs list.
     - For each parsed DataSourceBlob instance, assert that the 'data_source.ts_type'
       matches the corresponding value in the correct_blobs list.
     """
     with open(sample_data_source_xml_file) as f:
         sample_data_source_xml = f.read()
 
-    blob_list = xml_data_structure.parse_xml(sample_data_source_xml)
+    blob_list = data_structure.parse_xml(sample_data_source_xml)
 
     for i, blob in enumerate(blob_list):
         assert blob.site_name == correct_blobs[i]["site_name"]
         assert blob.data_source.name == correct_blobs[i]["data_source_name"]
         assert blob.data_source.ts_type == correct_blobs[i]["ts_type"]
         assert isinstance(blob.data.timeseries, correct_blobs[i]["data_type"])
 
@@ -168,15 +168,15 @@
       matches the corresponding value in the correct_blobs list.
     - For each parsed DataSourceBlob instance, assert that the 'data_source.ts_type'
       matches the corresponding value in the correct_blobs list.
     """
     with open(sample_data_source_xml_file, "rb") as f:
         sample_data_source_xml = f.read()
 
-    blob_list = xml_data_structure.parse_xml(sample_data_source_xml)
+    blob_list = data_structure.parse_xml(sample_data_source_xml)
 
     for i, blob in enumerate(blob_list):
         assert blob.site_name == correct_blobs[i]["site_name"]
         assert blob.data_source.name == correct_blobs[i]["data_source_name"]
         assert blob.data_source.ts_type == correct_blobs[i]["ts_type"]
         assert isinstance(blob.data.timeseries, correct_blobs[i]["data_type"])
 
@@ -207,15 +207,15 @@
     - For each parsed DataSourceBlob instance, assert that the 'data_source.ts_type'
       matches the corresponding value in the correct_blobs list.
     """
     with open(sample_data_source_xml_file) as f:
         xml_string = f.read()
         sample_data_source_xml = DefusedElementTree.fromstring(xml_string)
 
-    blob_list = xml_data_structure.parse_xml(sample_data_source_xml)
+    blob_list = data_structure.parse_xml(sample_data_source_xml)
 
     for i, blob in enumerate(blob_list):
         assert blob.site_name == correct_blobs[i]["site_name"]
         assert blob.data_source.name == correct_blobs[i]["data_source_name"]
         assert blob.data_source.ts_type == correct_blobs[i]["ts_type"]
         assert isinstance(blob.data.timeseries, correct_blobs[i]["data_type"])
 
@@ -243,18 +243,19 @@
     ----------
     - Assert that the canonicalized content of the generated XML matches the
         canonicalized content of the expected XML from the sample data source XML file.
     """
     with open(sample_data_source_xml_file) as f:
         sample_data_source_xml = f.read()
 
-    blob_list = xml_data_structure.parse_xml(sample_data_source_xml)
+    blob_list = data_structure.parse_xml(sample_data_source_xml)
 
     output_path = tmp_path / "output.xml"
-    xml_data_structure.write_hilltop_xml(blob_list, output_path)
+    # output_path = "output.xml"
+    data_structure.write_hilltop_xml(blob_list, output_path)
 
     with open(output_path) as f:
         output_xml = f.read()
 
     assert ElementTree.canonicalize(
         sample_data_source_xml,
         strip_text=True,
```

### Comparing `hydrobot-0.4.0/tests/xml_test_data_file.xml` & `hydrobot-0.5.0/tests/xml_test_data_file.xml`

 * *Files 22% similar despite different names*

#### Comparing `hydrobot-0.4.0/tests/xml_test_data_file.xml` & `hydrobot-0.5.0/tests/xml_test_data_file.xml`

```diff
@@ -12,35 +12,68 @@
         <ItemFormat>I</ItemFormat>
         <Divisor>1</Divisor>
         <Units>out of 10</Units>
         <Format>#.###</Format>
       </ItemInfo>
     </DataSource>
     <Data DateFormat="mowsecs" NumItems="1">
-      <V>2619302400 10</V>
-      <V>2619302700 9</V>
-      <V>2619303000 8</V>
-      <V>2619303300 10</V>
-      <V>2619303600 10</V>
-      <V>2619303900 9</V>
-      <V>2619304200 10</V>
-      <V>2619304500 6</V>
-      <V>2619304800 10</V>
-      <V>2619305100 10</V>
+      <E>
+        <T>2619302400</T>
+        <I1>10</I1>
+      </E>
+      <E>
+        <T>2619302700</T>
+        <I1>9</I1>
+      </E>
+      <E>
+        <T>2619303000</T>
+        <I1>8</I1>
+      </E>
+      <E>
+        <T>2619303300</T>
+        <I1>10</I1>
+      </E>
+      <E>
+        <T>2619303600</T>
+        <I1>10</I1>
+      </E>
+      <E>
+        <T>2619303900</T>
+        <I1>9</I1>
+      </E>
+      <E>
+        <T>2619304200</T>
+        <I1>10</I1>
+      </E>
+      <E>
+        <T>2619304500</T>
+        <I1>6</I1>
+      </E>
+      <E>
+        <T>2619304800</T>
+        <I1>10</I1>
+      </E>
+      <E>
+        <T>2619305100</T>
+        <I1>10</I1>
+      </E>
     </Data>
   </Measurement>
   <Measurement SiteName="Mid Stream at Cowtoilet Farm">
     <DataSource Name="General Nastiness" NumItems="1">
       <TSType>StdQualSeries</TSType>
       <DataType>SimpleTimeSeries</DataType>
       <Interpolation>Event</Interpolation>
       <ItemFormat>0</ItemFormat>
     </DataSource>
     <Data DateFormat="mowsecs" NumItems="1">
-      <V>2619302400 500</V>
+      <E>
+        <T>2619302400</T>
+        <I1>500</I1>
+      </E>
     </Data>
   </Measurement>
   <Measurement SiteName="Mid Stream at Cowtoilet Farm">
     <DataSource Name="General Nastiness" NumItems="3">
       <TSType>CheckSeries</TSType>
       <DataType>SimpleTimeSeries</DataType>
       <Interpolation>Discrete</Interpolation>
@@ -105,35 +138,68 @@
         <ItemFormat>F</ItemFormat>
         <Divisor>1</Divisor>
         <Units>t/s</Units>
         <Format>####.#</Format>
       </ItemInfo>
     </DataSource>
     <Data DateFormat="mowsecs" NumItems="1">
-      <V>2619302400 174.3</V>
-      <V>2619302700 7.4</V>
-      <V>2619303000 1882.1</V>
-      <V>2619303300 12.4</V>
-      <V>2619303600 104.0</V>
-      <V>2619303900 1145.0</V>
-      <V>2619304200 6234.6</V>
-      <V>2619304500 6.1</V>
-      <V>2619304800 9991.0</V>
-      <V>2619305100 4.0</V>
+      <E>
+        <T>2619302400</T>
+        <I1>174.3</I1>
+      </E>
+      <E>
+        <T>2619302700</T>
+        <I1>7.4</I1>
+      </E>
+      <E>
+        <T>2619303000</T>
+        <I1>1882.1</I1>
+      </E>
+      <E>
+        <T>2619303300</T>
+        <I1>12.4</I1>
+      </E>
+      <E>
+        <T>2619303600</T>
+        <I1>104.0</I1>
+      </E>
+      <E>
+        <T>2619303900</T>
+        <I1>1145.0</I1>
+      </E>
+      <E>
+        <T>2619304200</T>
+        <I1>6234.6</I1>
+      </E>
+      <E>
+        <T>2619304500</T>
+        <I1>6.1</I1>
+      </E>
+      <E>
+        <T>2619304800</T>
+        <I1>9991.0</I1>
+      </E>
+      <E>
+        <T>2619305100</T>
+        <I1>4.0</I1>
+      </E>
     </Data>
   </Measurement>
   <Measurement SiteName="Mid Stream at Cowtoilet Farm">
     <DataSource Name="Number of Actual Whole Human Turds Floating By" NumItems="1">
       <TSType>StdQualSeries</TSType>
       <DataType>Turds per Second</DataType>
       <Interpolation>Event</Interpolation>
       <ItemFormat>0</ItemFormat>
     </DataSource>
     <Data DateFormat="mowsecs" NumItems="1">
-      <V>2619302400 200</V>
+      <E>
+        <T>2619302400</T>
+        <I1>200</I1>
+      </E>
     </Data>
   </Measurement>
   <Measurement SiteName="Mid Stream at Cowtoilet Farm">
     <DataSource Name="Number of Actual Whole Human Turds Floating By" NumItems="4">
       <TSType>CheckSeries</TSType>
       <DataType>Turds per Second</DataType>
       <Interpolation>Discrete</Interpolation>
@@ -209,35 +275,68 @@
         <ItemFormat>I</ItemFormat>
         <Divisor>1</Divisor>
         <Units>ppm</Units>
         <Format>##</Format>
       </ItemInfo>
     </DataSource>
     <Data DateFormat="mowsecs" NumItems="1">
-      <V>2619302400 1</V>
-      <V>2619302700 7</V>
-      <V>2619303000 1</V>
-      <V>2619303300 1</V>
-      <V>2619303600 1</V>
-      <V>2619303900 1</V>
-      <V>2619304200 6</V>
-      <V>2619304500 6</V>
-      <V>2619304800 9</V>
-      <V>2619305100 4</V>
+      <E>
+        <T>2619302400</T>
+        <I1>1</I1>
+      </E>
+      <E>
+        <T>2619302700</T>
+        <I1>7</I1>
+      </E>
+      <E>
+        <T>2619303000</T>
+        <I1>1</I1>
+      </E>
+      <E>
+        <T>2619303300</T>
+        <I1>1</I1>
+      </E>
+      <E>
+        <T>2619303600</T>
+        <I1>1</I1>
+      </E>
+      <E>
+        <T>2619303900</T>
+        <I1>1</I1>
+      </E>
+      <E>
+        <T>2619304200</T>
+        <I1>6</I1>
+      </E>
+      <E>
+        <T>2619304500</T>
+        <I1>6</I1>
+      </E>
+      <E>
+        <T>2619304800</T>
+        <I1>9</I1>
+      </E>
+      <E>
+        <T>2619305100</T>
+        <I1>4</I1>
+      </E>
     </Data>
   </Measurement>
   <Measurement SiteName="Mid Stream at Cowtoilet Farm">
     <DataSource Name="Dead Cow Concentration" NumItems="1">
       <TSType>StdQualSeries</TSType>
       <DataType>Dead Cows</DataType>
       <Interpolation>Event</Interpolation>
       <ItemFormat>0</ItemFormat>
     </DataSource>
     <Data DateFormat="mowsecs" NumItems="1">
-      <V>2619302400 600</V>
+      <E>
+        <T>2619302399</T>
+        <I1>600</I1>
+      </E>
     </Data>
   </Measurement>
   <Measurement SiteName="Mid Stream at Cowtoilet Farm">
     <DataSource Name="Dead Cow Concentration" NumItems="3">
       <TSType>CheckSeries</TSType>
       <DataType>Dead Cows</DataType>
       <Interpolation>Discrete</Interpolation>
```

