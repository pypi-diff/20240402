# Comparing `tmp/earthstat-0.8.0.tar.gz` & `tmp/earthstat-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "earthstat-0.8.0.tar", last modified: Mon Apr  1 15:26:07 2024, max compression
+gzip compressed data, was "earthstat-0.8.1.tar", last modified: Tue Apr  2 17:43:40 2024, max compression
```

## Comparing `earthstat-0.8.0.tar` & `earthstat-0.8.1.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:26:07.576895 earthstat-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-01 15:25:56.000000 earthstat-0.8.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:26:07.556894 earthstat-0.8.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:26:07.560894 earthstat-0.8.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-01 15:25:56.000000 earthstat-0.8.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-01 15:25:56.000000 earthstat-0.8.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-01 15:25:56.000000 earthstat-0.8.0/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:26:07.560894 earthstat-0.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-01 15:25:56.000000 earthstat-0.8.0/.github/workflows/docs-build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-01 15:25:56.000000 earthstat-0.8.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-01 15:25:56.000000 earthstat-0.8.0/.github/workflows/installation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-01 15:25:56.000000 earthstat-0.8.0/.github/workflows/macos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-01 15:25:56.000000 earthstat-0.8.0/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-01 15:25:56.000000 earthstat-0.8.0/.github/workflows/ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-01 15:25:56.000000 earthstat-0.8.0/.github/workflows/windows.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-01 15:25:56.000000 earthstat-0.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-01 15:25:56.000000 earthstat-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-01 15:25:56.000000 earthstat-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8762 2024-04-01 15:26:07.572894 earthstat-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7662 2024-04-01 15:25:56.000000 earthstat-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:26:07.564894 earthstat-0.8.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-01 15:25:56.000000 earthstat-0.8.0/docs/analysis_aggregation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:26:07.564894 earthstat-0.8.0/docs/assests/
--rw-r--r--   0 runner    (1001) docker     (127)   255545 2024-04-01 15:25:56.000000 earthstat-0.8.0/docs/assests/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    23245 2024-04-01 15:25:56.000000 earthstat-0.8.0/docs/assests/logo_white.png
--rw-r--r--   0 runner    (1001) docker     (127)   751576 2024-04-01 15:25:56.000000 earthstat-0.8.0/docs/assests/workflow.png
--rw-r--r--   0 runner    (1001) docker     (127)   484549 2024-04-01 15:25:56.000000 earthstat-0.8.0/docs/assests/xES_workflow.png
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-01 15:25:56.000000 earthstat-0.8.0/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-01 15:25:56.000000 earthstat-0.8.0/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-01 15:25:56.000000 earthstat-0.8.0/docs/data_compatibility.md
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-01 15:25:56.000000 earthstat-0.8.0/docs/data_converter.md
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-01 15:25:56.000000 earthstat-0.8.0/docs/earthstat.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:26:07.568894 earthstat-0.8.0/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)    17964 2024-04-01 15:25:56.000000 earthstat-0.8.0/docs/examples/intro.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    10313 2024-04-01 15:25:56.000000 earthstat-0.8.0/docs/examples/xES.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-01 15:25:56.000000 earthstat-0.8.0/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-01 15:25:56.000000 earthstat-0.8.0/docs/geo_data_processing.md
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-01 15:25:56.000000 earthstat-0.8.0/docs/geo_meta_extractor.md
--rw-r--r--   0 runner    (1001) docker     (127)     7692 2024-04-01 15:25:56.000000 earthstat-0.8.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-01 15:25:56.000000 earthstat-0.8.0/docs/installation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:26:07.568894 earthstat-0.8.0/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-01 15:25:56.000000 earthstat-0.8.0/docs/overrides/main.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:26:07.568894 earthstat-0.8.0/docs/usage/
--rw-r--r--   0 runner    (1001) docker     (127)     8413 2024-04-01 15:25:56.000000 earthstat-0.8.0/docs/usage/main_usage.md
--rw-r--r--   0 runner    (1001) docker     (127)     5053 2024-04-01 15:25:56.000000 earthstat-0.8.0/docs/usage/xES_usage.md
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-01 15:25:56.000000 earthstat-0.8.0/docs/utils.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:26:07.568894 earthstat-0.8.0/earthstat/
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-01 15:25:56.000000 earthstat-0.8.0/earthstat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:26:07.568894 earthstat-0.8.0/earthstat/analysis_aggregation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 15:25:56.000000 earthstat-0.8.0/earthstat/analysis_aggregation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5563 2024-04-01 15:25:56.000000 earthstat-0.8.0/earthstat/analysis_aggregation/aggregate_process.py
--rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-04-01 15:25:56.000000 earthstat-0.8.0/earthstat/analysis_aggregation/parallel_clip_aggregate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:26:07.568894 earthstat-0.8.0/earthstat/data_compatibility/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 15:25:56.000000 earthstat-0.8.0/earthstat/data_compatibility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-01 15:25:56.000000 earthstat-0.8.0/earthstat/data_compatibility/compatibility_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-01 15:25:56.000000 earthstat-0.8.0/earthstat/data_compatibility/data_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-04-01 15:25:56.000000 earthstat-0.8.0/earthstat/data_compatibility/process_comp_issues.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:26:07.572894 earthstat-0.8.0/earthstat/data_converter/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-01 15:25:56.000000 earthstat-0.8.0/earthstat/data_converter/hdf5_to_tiff.py
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-01 15:25:56.000000 earthstat-0.8.0/earthstat/data_converter/netcdf_to_tiff.py
--rw-r--r--   0 runner    (1001) docker     (127)    14875 2024-04-01 15:25:56.000000 earthstat-0.8.0/earthstat/earthstat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:26:07.572894 earthstat-0.8.0/earthstat/geo_data_processing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 15:25:56.000000 earthstat-0.8.0/earthstat/geo_data_processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-04-01 15:25:56.000000 earthstat-0.8.0/earthstat/geo_data_processing/clip_raster.py
--rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-04-01 15:25:56.000000 earthstat-0.8.0/earthstat/geo_data_processing/rescale_resample_raster.py
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-01 15:25:56.000000 earthstat-0.8.0/earthstat/geo_data_processing/shapefile_process.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:26:07.572894 earthstat-0.8.0/earthstat/geo_meta_extractors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 15:25:56.000000 earthstat-0.8.0/earthstat/geo_meta_extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-01 15:25:56.000000 earthstat-0.8.0/earthstat/geo_meta_extractors/mask_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-04-01 15:25:56.000000 earthstat-0.8.0/earthstat/geo_meta_extractors/predictor_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-01 15:25:56.000000 earthstat-0.8.0/earthstat/geo_meta_extractors/shapefile_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-01 15:25:56.000000 earthstat-0.8.0/earthstat/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:26:07.572894 earthstat-0.8.0/earthstat/xES/
--rw-r--r--   0 runner    (1001) docker     (127)     4787 2024-04-01 15:25:56.000000 earthstat-0.8.0/earthstat/xES/DailyDatasetBuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)     6886 2024-04-01 15:25:56.000000 earthstat-0.8.0/earthstat/xES/DekadalDatasetBuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 15:25:56.000000 earthstat-0.8.0/earthstat/xES/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-01 15:25:56.000000 earthstat-0.8.0/earthstat/xES/cds_api_key_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-04-01 15:25:56.000000 earthstat-0.8.0/earthstat/xES/cds_param.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-01 15:25:56.000000 earthstat-0.8.0/earthstat/xES/download_AgERA5py.py
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-01 15:25:56.000000 earthstat-0.8.0/earthstat/xES/get_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-04-01 15:25:56.000000 earthstat-0.8.0/earthstat/xES/xES_utiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-04-01 15:25:56.000000 earthstat-0.8.0/earthstat/xearthstat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:26:07.572894 earthstat-0.8.0/earthstat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8762 2024-04-01 15:26:07.000000 earthstat-0.8.0/earthstat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-04-01 15:26:07.000000 earthstat-0.8.0/earthstat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 15:26:07.000000 earthstat-0.8.0/earthstat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-01 15:26:07.000000 earthstat-0.8.0/earthstat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-01 15:26:07.000000 earthstat-0.8.0/earthstat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-01 15:26:07.000000 earthstat-0.8.0/earthstat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-04-01 15:25:56.000000 earthstat-0.8.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-01 15:25:56.000000 earthstat-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-01 15:25:56.000000 earthstat-0.8.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-01 15:25:56.000000 earthstat-0.8.0/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 15:26:07.576895 earthstat-0.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:26:07.572894 earthstat-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-01 15:25:56.000000 earthstat-0.8.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-01 15:25:56.000000 earthstat-0.8.0/tests/test_earthstat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:43:40.410692 earthstat-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-02 17:43:26.000000 earthstat-0.8.1/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:43:40.394692 earthstat-0.8.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:43:40.398692 earthstat-0.8.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-02 17:43:26.000000 earthstat-0.8.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-02 17:43:26.000000 earthstat-0.8.1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-02 17:43:26.000000 earthstat-0.8.1/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:43:40.398692 earthstat-0.8.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-02 17:43:26.000000 earthstat-0.8.1/.github/workflows/docs-build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-02 17:43:26.000000 earthstat-0.8.1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-02 17:43:26.000000 earthstat-0.8.1/.github/workflows/installation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-02 17:43:26.000000 earthstat-0.8.1/.github/workflows/macos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-02 17:43:26.000000 earthstat-0.8.1/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-02 17:43:26.000000 earthstat-0.8.1/.github/workflows/ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-02 17:43:26.000000 earthstat-0.8.1/.github/workflows/windows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-02 17:43:26.000000 earthstat-0.8.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-02 17:43:26.000000 earthstat-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-02 17:43:26.000000 earthstat-0.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8762 2024-04-02 17:43:40.410692 earthstat-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7662 2024-04-02 17:43:26.000000 earthstat-0.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:43:40.398692 earthstat-0.8.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-02 17:43:26.000000 earthstat-0.8.1/docs/analysis_aggregation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:43:40.402692 earthstat-0.8.1/docs/assests/
+-rw-r--r--   0 runner    (1001) docker     (127)   255545 2024-04-02 17:43:26.000000 earthstat-0.8.1/docs/assests/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    23245 2024-04-02 17:43:26.000000 earthstat-0.8.1/docs/assests/logo_white.png
+-rw-r--r--   0 runner    (1001) docker     (127)   751576 2024-04-02 17:43:26.000000 earthstat-0.8.1/docs/assests/workflow.png
+-rw-r--r--   0 runner    (1001) docker     (127)   484549 2024-04-02 17:43:26.000000 earthstat-0.8.1/docs/assests/xES_workflow.png
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-02 17:43:26.000000 earthstat-0.8.1/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-02 17:43:26.000000 earthstat-0.8.1/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-02 17:43:26.000000 earthstat-0.8.1/docs/data_compatibility.md
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-02 17:43:26.000000 earthstat-0.8.1/docs/data_converter.md
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-02 17:43:26.000000 earthstat-0.8.1/docs/earthstat.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:43:40.402692 earthstat-0.8.1/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    17964 2024-04-02 17:43:26.000000 earthstat-0.8.1/docs/examples/intro.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    10313 2024-04-02 17:43:26.000000 earthstat-0.8.1/docs/examples/xES.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-02 17:43:26.000000 earthstat-0.8.1/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-02 17:43:26.000000 earthstat-0.8.1/docs/geo_data_processing.md
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-02 17:43:26.000000 earthstat-0.8.1/docs/geo_meta_extractor.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7692 2024-04-02 17:43:26.000000 earthstat-0.8.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-02 17:43:26.000000 earthstat-0.8.1/docs/installation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:43:40.402692 earthstat-0.8.1/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-02 17:43:26.000000 earthstat-0.8.1/docs/overrides/main.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:43:40.402692 earthstat-0.8.1/docs/usage/
+-rw-r--r--   0 runner    (1001) docker     (127)     8413 2024-04-02 17:43:26.000000 earthstat-0.8.1/docs/usage/main_usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5053 2024-04-02 17:43:26.000000 earthstat-0.8.1/docs/usage/xES_usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-02 17:43:26.000000 earthstat-0.8.1/docs/utils.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:43:40.406692 earthstat-0.8.1/earthstat/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-02 17:43:26.000000 earthstat-0.8.1/earthstat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:43:40.406692 earthstat-0.8.1/earthstat/analysis_aggregation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 17:43:26.000000 earthstat-0.8.1/earthstat/analysis_aggregation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5563 2024-04-02 17:43:26.000000 earthstat-0.8.1/earthstat/analysis_aggregation/aggregate_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6039 2024-04-02 17:43:26.000000 earthstat-0.8.1/earthstat/analysis_aggregation/parallel_clip_aggregate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:43:40.406692 earthstat-0.8.1/earthstat/data_compatibility/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 17:43:26.000000 earthstat-0.8.1/earthstat/data_compatibility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-02 17:43:26.000000 earthstat-0.8.1/earthstat/data_compatibility/compatibility_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-02 17:43:26.000000 earthstat-0.8.1/earthstat/data_compatibility/data_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-04-02 17:43:26.000000 earthstat-0.8.1/earthstat/data_compatibility/process_comp_issues.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:43:40.406692 earthstat-0.8.1/earthstat/data_converter/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-02 17:43:26.000000 earthstat-0.8.1/earthstat/data_converter/hdf5_to_tiff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-02 17:43:26.000000 earthstat-0.8.1/earthstat/data_converter/netcdf_to_tiff.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14875 2024-04-02 17:43:26.000000 earthstat-0.8.1/earthstat/earthstat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:43:40.406692 earthstat-0.8.1/earthstat/geo_data_processing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 17:43:26.000000 earthstat-0.8.1/earthstat/geo_data_processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-04-02 17:43:26.000000 earthstat-0.8.1/earthstat/geo_data_processing/clip_raster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-04-02 17:43:26.000000 earthstat-0.8.1/earthstat/geo_data_processing/rescale_resample_raster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-02 17:43:26.000000 earthstat-0.8.1/earthstat/geo_data_processing/shapefile_process.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:43:40.410692 earthstat-0.8.1/earthstat/geo_meta_extractors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 17:43:26.000000 earthstat-0.8.1/earthstat/geo_meta_extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-02 17:43:26.000000 earthstat-0.8.1/earthstat/geo_meta_extractors/mask_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-04-02 17:43:26.000000 earthstat-0.8.1/earthstat/geo_meta_extractors/predictor_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-02 17:43:26.000000 earthstat-0.8.1/earthstat/geo_meta_extractors/shapefile_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-02 17:43:26.000000 earthstat-0.8.1/earthstat/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:43:40.410692 earthstat-0.8.1/earthstat/xES/
+-rw-r--r--   0 runner    (1001) docker     (127)     4787 2024-04-02 17:43:26.000000 earthstat-0.8.1/earthstat/xES/DailyDatasetBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6886 2024-04-02 17:43:26.000000 earthstat-0.8.1/earthstat/xES/DekadalDatasetBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 17:43:26.000000 earthstat-0.8.1/earthstat/xES/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-02 17:43:26.000000 earthstat-0.8.1/earthstat/xES/cds_api_key_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-04-02 17:43:26.000000 earthstat-0.8.1/earthstat/xES/cds_param.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-02 17:43:26.000000 earthstat-0.8.1/earthstat/xES/download_AgERA5py.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-02 17:43:26.000000 earthstat-0.8.1/earthstat/xES/get_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-04-02 17:43:26.000000 earthstat-0.8.1/earthstat/xES/xES_utiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-04-02 17:43:26.000000 earthstat-0.8.1/earthstat/xearthstat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:43:40.410692 earthstat-0.8.1/earthstat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8762 2024-04-02 17:43:40.000000 earthstat-0.8.1/earthstat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-04-02 17:43:40.000000 earthstat-0.8.1/earthstat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 17:43:40.000000 earthstat-0.8.1/earthstat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-02 17:43:40.000000 earthstat-0.8.1/earthstat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-02 17:43:40.000000 earthstat-0.8.1/earthstat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-02 17:43:40.000000 earthstat-0.8.1/earthstat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-04-02 17:43:26.000000 earthstat-0.8.1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-02 17:43:26.000000 earthstat-0.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-02 17:43:26.000000 earthstat-0.8.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-02 17:43:26.000000 earthstat-0.8.1/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 17:43:40.410692 earthstat-0.8.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:43:40.410692 earthstat-0.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-02 17:43:26.000000 earthstat-0.8.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-02 17:43:26.000000 earthstat-0.8.1/tests/test_earthstat.py
```

### Comparing `earthstat-0.8.0/.github/ISSUE_TEMPLATE/config.yml` & `earthstat-0.8.1/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `earthstat-0.8.0/.github/workflows/docs-build.yml` & `earthstat-0.8.1/.github/workflows/docs-build.yml`

 * *Files identical despite different names*

### Comparing `earthstat-0.8.0/.github/workflows/docs.yml` & `earthstat-0.8.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `earthstat-0.8.0/.github/workflows/installation.yml` & `earthstat-0.8.1/.github/workflows/installation.yml`

 * *Files identical despite different names*

### Comparing `earthstat-0.8.0/.github/workflows/macos.yml` & `earthstat-0.8.1/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `earthstat-0.8.0/.github/workflows/pypi.yml` & `earthstat-0.8.1/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `earthstat-0.8.0/.github/workflows/ubuntu.yml` & `earthstat-0.8.1/.github/workflows/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `earthstat-0.8.0/.github/workflows/windows.yml` & `earthstat-0.8.1/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `earthstat-0.8.0/.gitignore` & `earthstat-0.8.1/.gitignore`

 * *Files identical despite different names*

### Comparing `earthstat-0.8.0/LICENSE` & `earthstat-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `earthstat-0.8.0/PKG-INFO` & `earthstat-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: earthstat
-Version: 0.8.0
+Version: 0.8.1
 Summary: EarthStat Library
 Author-email: Abdelrahman Saleh <abdulrahman.amr.ali@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/AbdelrahmanAmr3/earthstat
 Keywords: earthstat
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: earthstat Version: 0.8.0 Summary: EarthStat Library
+Metadata-Version: 2.1 Name: earthstat Version: 0.8.1 Summary: EarthStat Library
 Author-email: Abdelrahman Saleh
 gmail.com> License: MIT License Project-URL: Homepage, https://github.com/
 AbdelrahmanAmr3/earthstat Keywords: earthstat Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Natural Language :: English Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `earthstat-0.8.0/README.md` & `earthstat-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `earthstat-0.8.0/docs/assests/logo.png` & `earthstat-0.8.1/docs/assests/logo.png`

 * *Files identical despite different names*

### Comparing `earthstat-0.8.0/docs/assests/logo_white.png` & `earthstat-0.8.1/docs/assests/logo_white.png`

 * *Files identical despite different names*

### Comparing `earthstat-0.8.0/docs/assests/workflow.png` & `earthstat-0.8.1/docs/assests/workflow.png`

 * *Files identical despite different names*

### Comparing `earthstat-0.8.0/docs/assests/xES_workflow.png` & `earthstat-0.8.1/docs/assests/xES_workflow.png`

 * *Files identical despite different names*

### Comparing `earthstat-0.8.0/docs/contributing.md` & `earthstat-0.8.1/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `earthstat-0.8.0/docs/examples/intro.ipynb` & `earthstat-0.8.1/docs/examples/intro.ipynb`

 * *Files identical despite different names*

### Comparing `earthstat-0.8.0/docs/examples/xES.ipynb` & `earthstat-0.8.1/docs/examples/xES.ipynb`

 * *Files identical despite different names*

### Comparing `earthstat-0.8.0/docs/geo_data_processing.md` & `earthstat-0.8.1/docs/geo_data_processing.md`

 * *Files identical despite different names*

### Comparing `earthstat-0.8.0/docs/geo_meta_extractor.md` & `earthstat-0.8.1/docs/geo_meta_extractor.md`

 * *Files identical despite different names*

### Comparing `earthstat-0.8.0/docs/index.md` & `earthstat-0.8.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `earthstat-0.8.0/docs/installation.md` & `earthstat-0.8.1/docs/installation.md`

 * *Files identical despite different names*

### Comparing `earthstat-0.8.0/docs/usage/main_usage.md` & `earthstat-0.8.1/docs/usage/main_usage.md`

 * *Files identical despite different names*

### Comparing `earthstat-0.8.0/docs/usage/xES_usage.md` & `earthstat-0.8.1/docs/usage/xES_usage.md`

 * *Files identical despite different names*

### Comparing `earthstat-0.8.0/earthstat/analysis_aggregation/aggregate_process.py` & `earthstat-0.8.1/earthstat/analysis_aggregation/aggregate_process.py`

 * *Files identical despite different names*

### Comparing `earthstat-0.8.0/earthstat/analysis_aggregation/parallel_clip_aggregate.py` & `earthstat-0.8.1/earthstat/analysis_aggregation/parallel_clip_aggregate.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import os
 import geopandas as gpd
 import rasterio
 from rasterio.mask import mask
 import pandas as pd
 import numpy as np
 from tqdm import tqdm
-from concurrent.futures import ProcessPoolExecutor, as_completed
+# from concurrent.futures import ProcessPoolExecutor, as_completed
 from shapely.geometry import mapping
+import multiprocessing
 
 from ..utils import extractDateFromFilename, loadTiff
 
 
 def process_and_aggregate_raster(
 
         raster_path,
@@ -91,26 +92,24 @@
         if mask_src:
             mask_src.close()
 
     return aggregated_data
 
 
 def parallelAggregate(
-
     predictor_dir,
     shapefile_path,
     output_csv_path,
     mask_path=None,
     use_mask=False,
     invalid_values=None,
     calculation_mode="overall_mean",
     predictor_name="Value",
     all_touched=False,
     max_workers=None
-
 ):
     """
     Aggregates raster data from a directory in parallel into shapefile geometries, optionally using a mask.
 
     Args:
         predictor_dir (str): Directory containing raster datasets.
         shapefile_path (str): Path to the shapefile.
@@ -123,44 +122,43 @@
         all_touched (bool): Include all pixels touching geometry in the aggregation.
 
     Raises:
         ValueError: If use_mask is True and mask_path is not provided.
 
     Returns a CSV with aggregated data per shapefile geometry. Utilizes multiprocessing for efficiency.
     """
-
     if not max_workers:
         max_workers = os.cpu_count() - 1 if os.cpu_count() > 1 else 1
 
     predictor_paths = loadTiff(predictor_dir)
     data_list = []
 
     shape_file = gpd.read_file(shapefile_path)
 
     if use_mask and not mask_path:
         raise ValueError("Mask path must be provided if use_mask is True.")
 
-    with ProcessPoolExecutor(max_workers=max_workers) as executor:
-
-        futures = [
-
-            executor.submit(
-
-                process_and_aggregate_raster,
-                raster_path,
-                shape_file,
-                invalid_values,
-                use_mask,
-                mask_path,
-                calculation_mode,
-                predictor_name,
-                all_touched
-
-            ) for raster_path in predictor_paths
-        ]
+    # Prepare arguments for starmap
+    task_args = [
+        (
+            raster_path,
+            shape_file,
+            invalid_values,
+            use_mask,
+            mask_path,
+            calculation_mode,
+            predictor_name,
+            all_touched
+        ) for raster_path in predictor_paths
+    ]
+
+    with multiprocessing.Pool(processes=max_workers) as pool:
+        # Wrap pool.imap or pool.imap_unordered for a real-time tqdm progress bar
+        results = list(tqdm(pool.starmap(process_and_aggregate_raster, task_args), total=len(
+            task_args), desc="Processing rasters", unit="raster"))
 
-        for future in tqdm(as_completed(futures), total=len(futures), desc="Processing rasters", unit="raster"):
-            data_list.extend(future.result())
+        for result in results:
+            data_list.extend(result)
 
     df = pd.DataFrame(data_list)
     df[predictor_name] = df[predictor_name].round(3)
     df.to_csv(output_csv_path, index=False)
```

### Comparing `earthstat-0.8.0/earthstat/data_compatibility/compatibility_utils.py` & `earthstat-0.8.1/earthstat/data_compatibility/compatibility_utils.py`

 * *Files identical despite different names*

### Comparing `earthstat-0.8.0/earthstat/data_compatibility/data_compatibility.py` & `earthstat-0.8.1/earthstat/data_compatibility/data_compatibility.py`

 * *Files identical despite different names*

### Comparing `earthstat-0.8.0/earthstat/data_compatibility/process_comp_issues.py` & `earthstat-0.8.1/earthstat/data_compatibility/process_comp_issues.py`

 * *Files identical despite different names*

### Comparing `earthstat-0.8.0/earthstat/data_converter/netcdf_to_tiff.py` & `earthstat-0.8.1/earthstat/data_converter/netcdf_to_tiff.py`

 * *Files identical despite different names*

### Comparing `earthstat-0.8.0/earthstat/earthstat.py` & `earthstat-0.8.1/earthstat/earthstat.py`

 * *Files identical despite different names*

### Comparing `earthstat-0.8.0/earthstat/geo_data_processing/clip_raster.py` & `earthstat-0.8.1/earthstat/geo_data_processing/clip_raster.py`

 * *Files identical despite different names*

### Comparing `earthstat-0.8.0/earthstat/geo_data_processing/rescale_resample_raster.py` & `earthstat-0.8.1/earthstat/geo_data_processing/rescale_resample_raster.py`

 * *Files identical despite different names*

### Comparing `earthstat-0.8.0/earthstat/geo_data_processing/shapefile_process.py` & `earthstat-0.8.1/earthstat/geo_data_processing/shapefile_process.py`

 * *Files identical despite different names*

### Comparing `earthstat-0.8.0/earthstat/geo_meta_extractors/mask_meta.py` & `earthstat-0.8.1/earthstat/geo_meta_extractors/mask_meta.py`

 * *Files identical despite different names*

### Comparing `earthstat-0.8.0/earthstat/geo_meta_extractors/predictor_meta.py` & `earthstat-0.8.1/earthstat/geo_meta_extractors/predictor_meta.py`

 * *Files identical despite different names*

### Comparing `earthstat-0.8.0/earthstat/geo_meta_extractors/shapefile_meta.py` & `earthstat-0.8.1/earthstat/geo_meta_extractors/shapefile_meta.py`

 * *Files identical despite different names*

### Comparing `earthstat-0.8.0/earthstat/utils.py` & `earthstat-0.8.1/earthstat/utils.py`

 * *Files identical despite different names*

### Comparing `earthstat-0.8.0/earthstat/xES/DailyDatasetBuilder.py` & `earthstat-0.8.1/earthstat/xES/DailyDatasetBuilder.py`

 * *Files identical despite different names*

### Comparing `earthstat-0.8.0/earthstat/xES/DekadalDatasetBuilder.py` & `earthstat-0.8.1/earthstat/xES/DekadalDatasetBuilder.py`

 * *Files identical despite different names*

### Comparing `earthstat-0.8.0/earthstat/xES/cds_api_key_manager.py` & `earthstat-0.8.1/earthstat/xES/cds_api_key_manager.py`

 * *Files identical despite different names*

### Comparing `earthstat-0.8.0/earthstat/xES/cds_param.py` & `earthstat-0.8.1/earthstat/xES/cds_param.py`

 * *Files identical despite different names*

### Comparing `earthstat-0.8.0/earthstat/xES/download_AgERA5py.py` & `earthstat-0.8.1/earthstat/xES/download_AgERA5py.py`

 * *Files identical despite different names*

### Comparing `earthstat-0.8.0/earthstat/xES/get_csv.py` & `earthstat-0.8.1/earthstat/xES/get_csv.py`

 * *Files identical despite different names*

### Comparing `earthstat-0.8.0/earthstat/xES/xES_utiles.py` & `earthstat-0.8.1/earthstat/xES/xES_utiles.py`

 * *Files identical despite different names*

### Comparing `earthstat-0.8.0/earthstat/xearthstat.py` & `earthstat-0.8.1/earthstat/xearthstat.py`

 * *Files identical despite different names*

### Comparing `earthstat-0.8.0/earthstat.egg-info/PKG-INFO` & `earthstat-0.8.1/earthstat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: earthstat
-Version: 0.8.0
+Version: 0.8.1
 Summary: EarthStat Library
 Author-email: Abdelrahman Saleh <abdulrahman.amr.ali@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/AbdelrahmanAmr3/earthstat
 Keywords: earthstat
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: earthstat Version: 0.8.0 Summary: EarthStat Library
+Metadata-Version: 2.1 Name: earthstat Version: 0.8.1 Summary: EarthStat Library
 Author-email: Abdelrahman Saleh
 gmail.com> License: MIT License Project-URL: Homepage, https://github.com/
 AbdelrahmanAmr3/earthstat Keywords: earthstat Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Natural Language :: English Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `earthstat-0.8.0/earthstat.egg-info/SOURCES.txt` & `earthstat-0.8.1/earthstat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `earthstat-0.8.0/mkdocs.yml` & `earthstat-0.8.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `earthstat-0.8.0/pyproject.toml` & `earthstat-0.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "earthstat"
-version = "0.8.0"
+version = "0.8.1"
 dynamic = [
     "dependencies",
 ]
 description = "EarthStat Library"
 readme = "README.md"
 requires-python = ">=3.9"
 keywords = [
@@ -50,15 +50,15 @@
 
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 
 [tool.bumpversion]
-current_version = "0.8.0"
+current_version = "0.8.1"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
```

