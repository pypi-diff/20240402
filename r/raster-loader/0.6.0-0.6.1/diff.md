# Comparing `tmp/raster-loader-0.6.0.tar.gz` & `tmp/raster-loader-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raster-loader-0.6.0.tar", last modified: Mon Mar 25 15:44:35 2024, max compression
+gzip compressed data, was "raster-loader-0.6.1.tar", last modified: Tue Apr  2 16:09:58 2024, max compression
```

## Comparing `raster-loader-0.6.0.tar` & `raster-loader-0.6.1.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:44:35.736936 raster-loader-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-25 15:44:25.000000 raster-loader-0.6.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-25 15:44:25.000000 raster-loader-0.6.0/.env
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:44:35.720936 raster-loader-0.6.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:44:35.720936 raster-loader-0.6.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-03-25 15:44:25.000000 raster-loader-0.6.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-03-25 15:44:25.000000 raster-loader-0.6.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-03-25 15:44:25.000000 raster-loader-0.6.0/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:44:35.720936 raster-loader-0.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-03-25 15:44:25.000000 raster-loader-0.6.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-03-25 15:44:25.000000 raster-loader-0.6.0/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-03-25 15:44:25.000000 raster-loader-0.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-03-25 15:44:25.000000 raster-loader-0.6.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-03-25 15:44:25.000000 raster-loader-0.6.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-03-25 15:44:25.000000 raster-loader-0.6.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     7998 2024-03-25 15:44:25.000000 raster-loader-0.6.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-03-25 15:44:25.000000 raster-loader-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-03-25 15:44:25.000000 raster-loader-0.6.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     7057 2024-03-25 15:44:35.736936 raster-loader-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-03-25 15:44:25.000000 raster-loader-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-03-25 15:44:25.000000 raster-loader-0.6.0/ROADMAP.md
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-03-25 15:44:25.000000 raster-loader-0.6.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:44:35.716936 raster-loader-0.6.0/docker/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:44:35.720936 raster-loader-0.6.0/docker/raster_loader/
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-03-25 15:44:25.000000 raster-loader-0.6.0/docker/raster_loader/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-03-25 15:44:25.000000 raster-loader-0.6.0/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:44:35.724936 raster-loader-0.6.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-25 15:44:25.000000 raster-loader-0.6.0/docs/.pages
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-03-25 15:44:25.000000 raster-loader-0.6.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-03-25 15:44:25.000000 raster-loader-0.6.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:44:35.724936 raster-loader-0.6.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:44:35.724936 raster-loader-0.6.0/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     8109 2024-03-25 15:44:25.000000 raster-loader-0.6.0/docs/source/_static/carto-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-03-25 15:44:25.000000 raster-loader-0.6.0/docs/source/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-03-25 15:44:25.000000 raster-loader-0.6.0/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:44:35.724936 raster-loader-0.6.0/docs/source/developer_guide/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-25 15:44:25.000000 raster-loader-0.6.0/docs/source/developer_guide/contribute.md
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-25 15:44:25.000000 raster-loader-0.6.0/docs/source/developer_guide/roadmap.md
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-03-25 15:44:25.000000 raster-loader-0.6.0/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:44:35.724936 raster-loader-0.6.0/docs/source/user_guide/
--rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-03-25 15:44:25.000000 raster-loader-0.6.0/docs/source/user_guide/cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-03-25 15:44:25.000000 raster-loader-0.6.0/docs/source/user_guide/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:44:35.724936 raster-loader-0.6.0/docs/source/user_guide/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-03-25 15:44:25.000000 raster-loader-0.6.0/docs/source/user_guide/modules/raster_loader.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-03-25 15:44:25.000000 raster-loader-0.6.0/docs/source/user_guide/use_with_python.rst
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-25 15:44:25.000000 raster-loader-0.6.0/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:44:35.724936 raster-loader-0.6.0/raster_loader/
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-03-25 15:44:25.000000 raster-loader-0.6.0/raster_loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-25 15:44:35.000000 raster-loader-0.6.0/raster_loader/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:44:35.724936 raster-loader-0.6.0/raster_loader/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-03-25 15:44:25.000000 raster-loader-0.6.0/raster_loader/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5684 2024-03-25 15:44:25.000000 raster-loader-0.6.0/raster_loader/cli/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-03-25 15:44:25.000000 raster-loader-0.6.0/raster_loader/cli/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6887 2024-03-25 15:44:25.000000 raster-loader-0.6.0/raster_loader/cli/snowflake.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-03-25 15:44:25.000000 raster-loader-0.6.0/raster_loader/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-03-25 15:44:25.000000 raster-loader-0.6.0/raster_loader/geo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:44:35.728936 raster-loader-0.6.0/raster_loader/io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 15:44:25.000000 raster-loader-0.6.0/raster_loader/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9105 2024-03-25 15:44:25.000000 raster-loader-0.6.0/raster_loader/io/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (127)    10867 2024-03-25 15:44:25.000000 raster-loader-0.6.0/raster_loader/io/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4952 2024-03-25 15:44:25.000000 raster-loader-0.6.0/raster_loader/io/datawarehouse.py
--rw-r--r--   0 runner    (1001) docker     (127)     8066 2024-03-25 15:44:25.000000 raster-loader-0.6.0/raster_loader/io/snowflake.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:44:35.728936 raster-loader-0.6.0/raster_loader/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-03-25 15:44:25.000000 raster-loader-0.6.0/raster_loader/tests/.env.sample
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 15:44:25.000000 raster-loader-0.6.0/raster_loader/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:44:35.728936 raster-loader-0.6.0/raster_loader/tests/bigquery/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 15:44:25.000000 raster-loader-0.6.0/raster_loader/tests/bigquery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6313 2024-03-25 15:44:25.000000 raster-loader-0.6.0/raster_loader/tests/bigquery/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    21502 2024-03-25 15:44:25.000000 raster-loader-0.6.0/raster_loader/tests/bigquery/test_io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:44:35.732936 raster-loader-0.6.0/raster_loader/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)  1050018 2024-03-25 15:44:25.000000 raster-loader-0.6.0/raster_loader/tests/fixtures/expected_blocksize_512.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   262888 2024-03-25 15:44:25.000000 raster-loader-0.6.0/raster_loader/tests/fixtures/expected_custom_column.npy
--rw-r--r--   0 runner    (1001) docker     (127)   263638 2024-03-25 15:44:25.000000 raster-loader-0.6.0/raster_loader/tests/fixtures/expected_custom_column.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   525108 2024-03-25 15:44:25.000000 raster-loader-0.6.0/raster_loader/tests/fixtures/expected_custom_multiple_column.npy
--rw-r--r--   0 runner    (1001) docker     (127)   525873 2024-03-25 15:44:25.000000 raster-loader-0.6.0/raster_loader/tests/fixtures/expected_custom_multiple_column.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   262916 2024-03-25 15:44:25.000000 raster-loader-0.6.0/raster_loader/tests/fixtures/expected_default_column.npy
--rw-r--r--   0 runner    (1001) docker     (127)   263598 2024-03-25 15:44:25.000000 raster-loader-0.6.0/raster_loader/tests/fixtures/expected_default_column.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   525094 2024-03-25 15:44:25.000000 raster-loader-0.6.0/raster_loader/tests/fixtures/expected_default_multiple_column.npy
--rw-r--r--   0 runner    (1001) docker     (127)   525845 2024-03-25 15:44:25.000000 raster-loader-0.6.0/raster_loader/tests/fixtures/expected_multiple_column.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   729781 2024-03-25 15:44:25.000000 raster-loader-0.6.0/raster_loader/tests/fixtures/mosaic.tif
--rw-r--r--   0 runner    (1001) docker     (127)   286093 2024-03-25 15:44:25.000000 raster-loader-0.6.0/raster_loader/tests/fixtures/mosaic_cog.tif
--rw-r--r--   0 runner    (1001) docker     (127)    70360 2024-03-25 15:44:25.000000 raster-loader-0.6.0/raster_loader/tests/fixtures/mosaic_cog_1_1.tif
--rw-r--r--   0 runner    (1001) docker     (127)    32945 2024-03-25 15:44:25.000000 raster-loader-0.6.0/raster_loader/tests/fixtures/mosaic_cog_1_2.tif
--rw-r--r--   0 runner    (1001) docker     (127)   262727 2024-03-25 15:44:25.000000 raster-loader-0.6.0/raster_loader/tests/fixtures/mosaic_cog_2_1.tif
--rw-r--r--   0 runner    (1001) docker     (127)   262727 2024-03-25 15:44:25.000000 raster-loader-0.6.0/raster_loader/tests/fixtures/mosaic_cog_2_2.tif
--rw-r--r--   0 runner    (1001) docker     (127)   245271 2024-03-25 15:44:25.000000 raster-loader-0.6.0/raster_loader/tests/fixtures/mosaic_cog_512.tif
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-03-25 15:44:25.000000 raster-loader-0.6.0/raster_loader/tests/mocks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:44:35.732936 raster-loader-0.6.0/raster_loader/tests/snowflake/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 15:44:25.000000 raster-loader-0.6.0/raster_loader/tests/snowflake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8610 2024-03-25 15:44:25.000000 raster-loader-0.6.0/raster_loader/tests/snowflake/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    19965 2024-03-25 15:44:25.000000 raster-loader-0.6.0/raster_loader/tests/snowflake/test_io.py
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-03-25 15:44:25.000000 raster-loader-0.6.0/raster_loader/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-03-25 15:44:25.000000 raster-loader-0.6.0/raster_loader/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 15:44:35.736936 raster-loader-0.6.0/raster_loader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7057 2024-03-25 15:44:35.000000 raster-loader-0.6.0/raster_loader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-03-25 15:44:35.000000 raster-loader-0.6.0/raster_loader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 15:44:35.000000 raster-loader-0.6.0/raster_loader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-03-25 15:44:35.000000 raster-loader-0.6.0/raster_loader.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 15:44:35.000000 raster-loader-0.6.0/raster_loader.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-03-25 15:44:35.000000 raster-loader-0.6.0/raster_loader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-25 15:44:35.000000 raster-loader-0.6.0/raster_loader.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-03-25 15:44:25.000000 raster-loader-0.6.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-25 15:44:25.000000 raster-loader-0.6.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-03-25 15:44:35.736936 raster-loader-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-03-25 15:44:25.000000 raster-loader-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:09:58.675689 raster-loader-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-02 16:09:50.000000 raster-loader-0.6.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-02 16:09:50.000000 raster-loader-0.6.1/.env
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:09:58.663689 raster-loader-0.6.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:09:58.663689 raster-loader-0.6.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-02 16:09:50.000000 raster-loader-0.6.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-02 16:09:50.000000 raster-loader-0.6.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-02 16:09:50.000000 raster-loader-0.6.1/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:09:58.663689 raster-loader-0.6.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-02 16:09:50.000000 raster-loader-0.6.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-04-02 16:09:50.000000 raster-loader-0.6.1/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-04-02 16:09:50.000000 raster-loader-0.6.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-02 16:09:50.000000 raster-loader-0.6.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-02 16:09:50.000000 raster-loader-0.6.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-04-02 16:09:50.000000 raster-loader-0.6.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7998 2024-04-02 16:09:50.000000 raster-loader-0.6.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-02 16:09:50.000000 raster-loader-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-02 16:09:50.000000 raster-loader-0.6.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     7144 2024-04-02 16:09:58.675689 raster-loader-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5333 2024-04-02 16:09:50.000000 raster-loader-0.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-02 16:09:50.000000 raster-loader-0.6.1/ROADMAP.md
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-02 16:09:50.000000 raster-loader-0.6.1/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:09:58.659689 raster-loader-0.6.1/docker/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:09:58.663689 raster-loader-0.6.1/docker/raster_loader/
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-02 16:09:50.000000 raster-loader-0.6.1/docker/raster_loader/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-02 16:09:50.000000 raster-loader-0.6.1/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:09:58.663689 raster-loader-0.6.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-02 16:09:50.000000 raster-loader-0.6.1/docs/.pages
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-02 16:09:50.000000 raster-loader-0.6.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-02 16:09:50.000000 raster-loader-0.6.1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:09:58.663689 raster-loader-0.6.1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:09:58.663689 raster-loader-0.6.1/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     8109 2024-04-02 16:09:50.000000 raster-loader-0.6.1/docs/source/_static/carto-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-02 16:09:50.000000 raster-loader-0.6.1/docs/source/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-04-02 16:09:50.000000 raster-loader-0.6.1/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:09:58.663689 raster-loader-0.6.1/docs/source/developer_guide/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-02 16:09:50.000000 raster-loader-0.6.1/docs/source/developer_guide/contribute.md
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-02 16:09:50.000000 raster-loader-0.6.1/docs/source/developer_guide/roadmap.md
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-02 16:09:50.000000 raster-loader-0.6.1/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:09:58.663689 raster-loader-0.6.1/docs/source/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-04-02 16:09:50.000000 raster-loader-0.6.1/docs/source/user_guide/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-02 16:09:50.000000 raster-loader-0.6.1/docs/source/user_guide/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:09:58.663689 raster-loader-0.6.1/docs/source/user_guide/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-02 16:09:50.000000 raster-loader-0.6.1/docs/source/user_guide/modules/raster_loader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-02 16:09:50.000000 raster-loader-0.6.1/docs/source/user_guide/use_with_python.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-02 16:09:50.000000 raster-loader-0.6.1/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:09:58.667689 raster-loader-0.6.1/raster_loader/
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-02 16:09:50.000000 raster-loader-0.6.1/raster_loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-02 16:09:58.000000 raster-loader-0.6.1/raster_loader/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:09:58.667689 raster-loader-0.6.1/raster_loader/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-02 16:09:50.000000 raster-loader-0.6.1/raster_loader/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5931 2024-04-02 16:09:50.000000 raster-loader-0.6.1/raster_loader/cli/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-02 16:09:50.000000 raster-loader-0.6.1/raster_loader/cli/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7134 2024-04-02 16:09:50.000000 raster-loader-0.6.1/raster_loader/cli/snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-02 16:09:50.000000 raster-loader-0.6.1/raster_loader/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-04-02 16:09:50.000000 raster-loader-0.6.1/raster_loader/geo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:09:58.667689 raster-loader-0.6.1/raster_loader/io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 16:09:50.000000 raster-loader-0.6.1/raster_loader/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9191 2024-04-02 16:09:50.000000 raster-loader-0.6.1/raster_loader/io/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10925 2024-04-02 16:09:50.000000 raster-loader-0.6.1/raster_loader/io/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4952 2024-04-02 16:09:50.000000 raster-loader-0.6.1/raster_loader/io/datawarehouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8152 2024-04-02 16:09:50.000000 raster-loader-0.6.1/raster_loader/io/snowflake.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:09:58.667689 raster-loader-0.6.1/raster_loader/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-02 16:09:50.000000 raster-loader-0.6.1/raster_loader/tests/.env.sample
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 16:09:50.000000 raster-loader-0.6.1/raster_loader/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:09:58.667689 raster-loader-0.6.1/raster_loader/tests/bigquery/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 16:09:50.000000 raster-loader-0.6.1/raster_loader/tests/bigquery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6313 2024-04-02 16:09:50.000000 raster-loader-0.6.1/raster_loader/tests/bigquery/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21502 2024-04-02 16:09:50.000000 raster-loader-0.6.1/raster_loader/tests/bigquery/test_io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:09:58.675689 raster-loader-0.6.1/raster_loader/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)  1050018 2024-04-02 16:09:50.000000 raster-loader-0.6.1/raster_loader/tests/fixtures/expected_blocksize_512.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   262888 2024-04-02 16:09:50.000000 raster-loader-0.6.1/raster_loader/tests/fixtures/expected_custom_column.npy
+-rw-r--r--   0 runner    (1001) docker     (127)   263638 2024-04-02 16:09:50.000000 raster-loader-0.6.1/raster_loader/tests/fixtures/expected_custom_column.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   525108 2024-04-02 16:09:50.000000 raster-loader-0.6.1/raster_loader/tests/fixtures/expected_custom_multiple_column.npy
+-rw-r--r--   0 runner    (1001) docker     (127)   525873 2024-04-02 16:09:50.000000 raster-loader-0.6.1/raster_loader/tests/fixtures/expected_custom_multiple_column.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   262916 2024-04-02 16:09:50.000000 raster-loader-0.6.1/raster_loader/tests/fixtures/expected_default_column.npy
+-rw-r--r--   0 runner    (1001) docker     (127)   263598 2024-04-02 16:09:50.000000 raster-loader-0.6.1/raster_loader/tests/fixtures/expected_default_column.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   525094 2024-04-02 16:09:50.000000 raster-loader-0.6.1/raster_loader/tests/fixtures/expected_default_multiple_column.npy
+-rw-r--r--   0 runner    (1001) docker     (127)   525845 2024-04-02 16:09:50.000000 raster-loader-0.6.1/raster_loader/tests/fixtures/expected_multiple_column.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   729781 2024-04-02 16:09:50.000000 raster-loader-0.6.1/raster_loader/tests/fixtures/mosaic.tif
+-rw-r--r--   0 runner    (1001) docker     (127)   286093 2024-04-02 16:09:50.000000 raster-loader-0.6.1/raster_loader/tests/fixtures/mosaic_cog.tif
+-rw-r--r--   0 runner    (1001) docker     (127)    70360 2024-04-02 16:09:50.000000 raster-loader-0.6.1/raster_loader/tests/fixtures/mosaic_cog_1_1.tif
+-rw-r--r--   0 runner    (1001) docker     (127)    32945 2024-04-02 16:09:50.000000 raster-loader-0.6.1/raster_loader/tests/fixtures/mosaic_cog_1_2.tif
+-rw-r--r--   0 runner    (1001) docker     (127)   262727 2024-04-02 16:09:50.000000 raster-loader-0.6.1/raster_loader/tests/fixtures/mosaic_cog_2_1.tif
+-rw-r--r--   0 runner    (1001) docker     (127)   262727 2024-04-02 16:09:50.000000 raster-loader-0.6.1/raster_loader/tests/fixtures/mosaic_cog_2_2.tif
+-rw-r--r--   0 runner    (1001) docker     (127)   245271 2024-04-02 16:09:50.000000 raster-loader-0.6.1/raster_loader/tests/fixtures/mosaic_cog_512.tif
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-02 16:09:50.000000 raster-loader-0.6.1/raster_loader/tests/mocks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:09:58.675689 raster-loader-0.6.1/raster_loader/tests/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 16:09:50.000000 raster-loader-0.6.1/raster_loader/tests/snowflake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8610 2024-04-02 16:09:50.000000 raster-loader-0.6.1/raster_loader/tests/snowflake/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19965 2024-04-02 16:09:50.000000 raster-loader-0.6.1/raster_loader/tests/snowflake/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-02 16:09:50.000000 raster-loader-0.6.1/raster_loader/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-02 16:09:50.000000 raster-loader-0.6.1/raster_loader/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:09:58.675689 raster-loader-0.6.1/raster_loader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7144 2024-04-02 16:09:58.000000 raster-loader-0.6.1/raster_loader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-04-02 16:09:58.000000 raster-loader-0.6.1/raster_loader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 16:09:58.000000 raster-loader-0.6.1/raster_loader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-02 16:09:58.000000 raster-loader-0.6.1/raster_loader.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 16:09:58.000000 raster-loader-0.6.1/raster_loader.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-02 16:09:58.000000 raster-loader-0.6.1/raster_loader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-02 16:09:58.000000 raster-loader-0.6.1/raster_loader.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-02 16:09:50.000000 raster-loader-0.6.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-02 16:09:50.000000 raster-loader-0.6.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-02 16:09:58.679689 raster-loader-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-02 16:09:50.000000 raster-loader-0.6.1/setup.py
```

### Comparing `raster-loader-0.6.0/.github/ISSUE_TEMPLATE/bug_report.md` & `raster-loader-0.6.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `raster-loader-0.6.0/.github/ISSUE_TEMPLATE/feature_request.md` & `raster-loader-0.6.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `raster-loader-0.6.0/.github/pull_request_template.md` & `raster-loader-0.6.1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `raster-loader-0.6.0/.github/workflows/ci.yml` & `raster-loader-0.6.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `raster-loader-0.6.0/.github/workflows/pypi-publish.yml` & `raster-loader-0.6.1/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `raster-loader-0.6.0/.gitignore` & `raster-loader-0.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `raster-loader-0.6.0/.readthedocs.yml` & `raster-loader-0.6.1/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `raster-loader-0.6.0/CHANGELOG.md` & `raster-loader-0.6.1/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,23 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.6.1] - 2024-04-02
+
+### Enhancements
+- Add a argument to skip interactive question on upload failure (#138)
+
+### Bug Fixes
+- fix: shapely.wkt import (#136)
+- fix: update pip commands to make it compatible with zsh (#137)
+
 ## [0.6.0] - 2024-03-25
 
 ### Enhancements
 - Add labels to BQ uploaded tables (#131)
 - Support input URLs and more connection credential types (#129)
 
 ### Bug Fixes
```

### Comparing `raster-loader-0.6.0/CONTRIBUTING.md` & `raster-loader-0.6.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `raster-loader-0.6.0/LICENSE` & `raster-loader-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `raster-loader-0.6.0/Makefile` & `raster-loader-0.6.1/Makefile`

 * *Files identical despite different names*

### Comparing `raster-loader-0.6.0/PKG-INFO` & `raster-loader-0.6.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raster-loader
-Version: 0.6.0
+Version: 0.6.1
 Summary: Python library for loading GIS raster data to standard cloud-based data warehouses that don't natively support raster data.
 Home-page: https://github.com/cartodb/raster-loader
 Author: CARTO
 License: BSD 3-Clause
 Keywords: carto,raster,gis,data warehouse,bigquery,snowflake
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -58,15 +58,18 @@
 ## Documentation
 
 The Raster Loader documentation is available at [raster-loader.readthedocs.io](https://raster-loader.readthedocs.io).
 
 ## Install
 
 ```bash
-pip install raster-loader
+pip install -U raster-loader
+
+pip install -U raster-loader"[bigquery]"
+pip install -U raster-loader"[snowflake]"
 ```
 
 ### Installing from source
 
 ```bash
 git clone https://github.com/cartodb/raster-loader
 cd raster-loader
```

### Comparing `raster-loader-0.6.0/README.md` & `raster-loader-0.6.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,18 @@
 ## Documentation
 
 The Raster Loader documentation is available at [raster-loader.readthedocs.io](https://raster-loader.readthedocs.io).
 
 ## Install
 
 ```bash
-pip install raster-loader
+pip install -U raster-loader
+
+pip install -U raster-loader"[bigquery]"
+pip install -U raster-loader"[snowflake]"
 ```
 
 ### Installing from source
 
 ```bash
 git clone https://github.com/cartodb/raster-loader
 cd raster-loader
```

### Comparing `raster-loader-0.6.0/ROADMAP.md` & `raster-loader-0.6.1/ROADMAP.md`

 * *Files identical despite different names*

### Comparing `raster-loader-0.6.0/conftest.py` & `raster-loader-0.6.1/conftest.py`

 * *Files identical despite different names*

### Comparing `raster-loader-0.6.0/docker/raster_loader/Dockerfile` & `raster-loader-0.6.1/docker/raster_loader/Dockerfile`

 * *Files identical despite different names*

### Comparing `raster-loader-0.6.0/docs/Makefile` & `raster-loader-0.6.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `raster-loader-0.6.0/docs/make.bat` & `raster-loader-0.6.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `raster-loader-0.6.0/docs/source/_static/carto-logo.png` & `raster-loader-0.6.1/docs/source/_static/carto-logo.png`

 * *Files identical despite different names*

### Comparing `raster-loader-0.6.0/docs/source/conf.py` & `raster-loader-0.6.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `raster-loader-0.6.0/docs/source/index.rst` & `raster-loader-0.6.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `raster-loader-0.6.0/docs/source/user_guide/cli.rst` & `raster-loader-0.6.1/docs/source/user_guide/cli.rst`

 * *Files identical despite different names*

### Comparing `raster-loader-0.6.0/docs/source/user_guide/installation.rst` & `raster-loader-0.6.1/docs/source/user_guide/installation.rst`

 * *Files 4% similar despite different names*

```diff
@@ -3,37 +3,36 @@
 Installing Raster Loader
 ========================
 
 Raster Loader is available on PyPI_ and can be installed with pip_:
 
 .. code-block:: bash
 
-   pip install raster-loader[all]
+   pip install -U raster-loader
 
 To install from source:
 
 .. code-block:: bash
 
    git clone https://github.com/cartodb/raster-loader
    cd raster-loader
-   pip install .[all]
+   pip install -U .
 
 .. tip::
 
    In most cases, it is recommended to install Raster Loader in a virtual environment.
    Use venv_ to create and manage your virtual environment.
 
-The above will install the dependencies required to work with both Snowflake and
-BigQuery. In case you only want to work with one of them, you can install the
+The above will install the dependencies required to work with both BigQuery and Snowflake and. In case you only want to work with one of them, you can install the
 dependencies for each of them separately:
 
 .. code-block:: bash
 
-   pip install raster-loader[snowflake]
-   pip install raster-loader[bigquery]
+   pip install -U raster-loader"[bigquery]"
+   pip install -U raster-loader"[snowflake]"
 
 After installing the Raster Loader package, you will have access to the
 :ref:`carto CLI <cli>`. To make sure the installation was successful, run the
 following command in your terminal:
 
 .. code-block:: bash
```

### Comparing `raster-loader-0.6.0/docs/source/user_guide/use_with_python.rst` & `raster-loader-0.6.1/docs/source/user_guide/use_with_python.rst`

 * *Files identical despite different names*

### Comparing `raster-loader-0.6.0/raster_loader/cli/bigquery.py` & `raster-loader-0.6.1/raster_loader/cli/bigquery.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,27 +67,34 @@
 )
 @click.option(
     "--append",
     help="Append records into a table if it already exists.",
     default=False,
     is_flag=True,
 )
+@click.option(
+    "--cleanup-on-failure",
+    help="Clean up resources if the upload fails. Useful for non-interactive scripts.",
+    default=False,
+    is_flag=True,
+)
 @catch_exception()
 def upload(
     file_path,
     file_url,
     project,
     token,
     dataset,
     table,
     band,
     band_name,
     chunk_size,
     overwrite=False,
     append=False,
+    cleanup_on_failure=False,
 ):
     from raster_loader.io.common import (
         get_number_of_blocks,
         print_band_information,
         get_block_dims,
     )
 
@@ -147,14 +154,15 @@
     connector.upload_raster(
         source,
         fqn,
         bands_info,
         chunk_size,
         overwrite=overwrite,
         append=append,
+        cleanup_on_failure=cleanup_on_failure,
     )
 
     click.echo("Raster file uploaded to Google BigQuery")
     return 0
 
 
 @bigquery.command(help="Load and describe a table from BigQuery")
```

### Comparing `raster-loader-0.6.0/raster_loader/cli/info.py` & `raster-loader-0.6.1/raster_loader/cli/info.py`

 * *Files identical despite different names*

### Comparing `raster-loader-0.6.0/raster_loader/cli/snowflake.py` & `raster-loader-0.6.1/raster_loader/cli/snowflake.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,20 @@
 )
 @click.option(
     "--append",
     help="Append records into a table if it already exists.",
     default=False,
     is_flag=True,
 )
+@click.option(
+    "--cleanup-on-failure",
+    help="Clean up resources if the upload fails. Useful for non-interactive scripts.",
+    default=False,
+    is_flag=True,
+)
 @catch_exception()
 def upload(
     account,
     username,
     password,
     token,
     role,
@@ -84,14 +90,15 @@
     schema,
     table,
     band,
     band_name,
     chunk_size,
     overwrite=False,
     append=False,
+    cleanup_on_failure=False,
 ):
     from raster_loader.io.common import (
         get_number_of_blocks,
         print_band_information,
         get_block_dims,
     )
 
@@ -158,14 +165,15 @@
     connector.upload_raster(
         source,
         fqn,
         bands_info,
         chunk_size,
         overwrite=overwrite,
         append=append,
+        cleanup_on_failure=cleanup_on_failure,
     )
 
     click.echo("Raster file uploaded to Snowflake")
     return 0
 
 
 @snowflake.command(help="Load and describe a table from Snowflake")
```

### Comparing `raster-loader-0.6.0/raster_loader/errors.py` & `raster-loader-0.6.1/raster_loader/errors.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 def import_error_bigquery():  # pragma: no cover
     msg = (
         "Google Cloud BigQuery client is not installed.\n"
         "Please install Google Cloud BigQuery dependencies to use this function.\n"
-        "run `pip install -U raster-loader[bigquery]` to install from pypi."
+        'run `pip install -U raster-loader"[bigquery]"` to install from pypi.'
     )
     raise ImportError(msg)
 
 
 def import_error_snowflake():  # pragma: no cover
     msg = (
         "Snowflake client is not installed.\n"
         "Please install Snowflake dependencies to use this function.\n"
-        "run `pip install -U raster-loader[snowflake]` to install from pypi."
+        'run `pip install -U raster-loader"[snowflake]"` to install from pypi.'
     )
     raise ImportError(msg)
 
 
 class IncompatibleRasterException(Exception):
     def __init__(self):
         self.message = (
```

### Comparing `raster-loader-0.6.0/raster_loader/geo.py` & `raster-loader-0.6.1/raster_loader/geo.py`

 * *Files identical despite different names*

### Comparing `raster-loader-0.6.0/raster_loader/io/bigquery.py` & `raster-loader-0.6.1/raster_loader/io/bigquery.py`

 * *Files 5% similar despite different names*

```diff
@@ -99,14 +99,15 @@
         self,
         file_path: str,
         fqn: str,
         bands_info: List[Tuple[int, str]] = [(1, None)],
         chunk_size: int = None,
         overwrite: bool = False,
         append: bool = False,
+        cleanup_on_failure: bool = False,
     ):
         """Write a raster file to a BigQuery table."""
         print("Loading raster file to BigQuery...")
 
         append_records = False
 
         try:
@@ -192,28 +193,28 @@
             print("Updating labels...")
             self.update_labels(fqn, self.get_labels(__version__))
 
         except IncompatibleRasterException as e:
             raise IOError("Error uploading to BigQuery: {}".format(e.message))
 
         except KeyboardInterrupt:
-            delete = ask_yes_no_question(
+            delete = cleanup_on_failure or ask_yes_no_question(
                 "Would you like to delete the partially uploaded table? [yes/no] "
             )
 
             if delete:
                 self.delete_table(fqn)
 
             raise KeyboardInterrupt
 
         except rasterio.errors.CRSError as e:
             raise e
 
         except Exception as e:
-            delete = ask_yes_no_question(
+            delete = cleanup_on_failure or ask_yes_no_question(
                 (
                     "Error uploading to BigQuery. "
                     "Would you like to delete the partially uploaded table? [yes/no] "
                 )
             )
 
             if delete:
```

### Comparing `raster-loader-0.6.0/raster_loader/io/common.py` & `raster-loader-0.6.1/raster_loader/io/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 import numpy as np
 
 from typing import Iterable
 from typing import Callable
 from typing import List
 from typing import Tuple
 from affine import Affine
+from shapely import wkt  # Can not use directly from shapely.wkt
+
 import rio_cogeo
 import rasterio
 import quadbin
 
 from raster_loader.geo import raster_bounds
 from raster_loader.errors import (
     error_not_google_compatible,
@@ -128,15 +130,15 @@
                 "type": raster_band_type(raster_dataset, band),
                 "band_name": band_field_name(band_name, band, band_rename_function),
             }
             bands_metadata.append(meta)
 
         # compute whole bounds for metadata
         bounds_geog = raster_bounds(raster_dataset, transformer, "wkt")
-        bounds_polygon = shapely.Polygon(shapely.wkt.loads(bounds_geog))
+        bounds_polygon = shapely.Polygon(wkt.loads(bounds_geog))
         bounds_coords = list(bounds_polygon.bounds)
         center_coords = list(*bounds_polygon.centroid.coords)
         center_coords.append(resolution)
 
         pixel_resolution = int(resolution + math.log(block_width * block_height, 4))
         if pixel_resolution > 26:
             raise ValueError(
```

### Comparing `raster-loader-0.6.0/raster_loader/io/datawarehouse.py` & `raster-loader-0.6.1/raster_loader/io/datawarehouse.py`

 * *Files identical despite different names*

### Comparing `raster-loader-0.6.0/raster_loader/io/snowflake.py` & `raster-loader-0.6.1/raster_loader/io/snowflake.py`

 * *Files 4% similar despite different names*

```diff
@@ -169,14 +169,15 @@
         self,
         file_path: str,
         fqn: str,
         bands_info: List[Tuple[int, str]] = None,
         chunk_size: int = None,
         overwrite: bool = False,
         append: bool = False,
+        cleanup_on_failure: bool = False,
     ) -> bool:
         print("Loading raster file to Snowflake...")
 
         bands_info = bands_info or [(1, None)]
 
         append_records = False
 
@@ -236,28 +237,28 @@
 
             self.write_metadata(metadata, append_records, fqn)
 
         except IncompatibleRasterException as e:
             raise IOError("Error uploading to Snowflake: {}".format(e.message))
 
         except KeyboardInterrupt:
-            delete = ask_yes_no_question(
+            delete = cleanup_on_failure or ask_yes_no_question(
                 "Would you like to delete the partially uploaded table? [yes/no] "
             )
 
             if delete:
                 self.delete_table(fqn)
 
             raise KeyboardInterrupt
 
         except rasterio.errors.CRSError as e:
             raise e
 
         except Exception as e:
-            delete = ask_yes_no_question(
+            delete = cleanup_on_failure or ask_yes_no_question(
                 (
                     "Error uploading to Snowflake. "
                     "Would you like to delete the partially uploaded table? [yes/no] "
                 )
             )
 
             if delete:
```

### Comparing `raster-loader-0.6.0/raster_loader/tests/bigquery/test_cli.py` & `raster-loader-0.6.1/raster_loader/tests/bigquery/test_cli.py`

 * *Files identical despite different names*

### Comparing `raster-loader-0.6.0/raster_loader/tests/bigquery/test_io.py` & `raster-loader-0.6.1/raster_loader/tests/bigquery/test_io.py`

 * *Files identical despite different names*

### Comparing `raster-loader-0.6.0/raster_loader/tests/fixtures/expected_blocksize_512.pkl` & `raster-loader-0.6.1/raster_loader/tests/fixtures/expected_blocksize_512.pkl`

 * *Files identical despite different names*

### Comparing `raster-loader-0.6.0/raster_loader/tests/fixtures/expected_custom_column.npy` & `raster-loader-0.6.1/raster_loader/tests/fixtures/expected_custom_column.npy`

 * *Files identical despite different names*

### Comparing `raster-loader-0.6.0/raster_loader/tests/fixtures/expected_custom_column.pkl` & `raster-loader-0.6.1/raster_loader/tests/fixtures/expected_custom_column.pkl`

 * *Files identical despite different names*

### Comparing `raster-loader-0.6.0/raster_loader/tests/fixtures/expected_custom_multiple_column.npy` & `raster-loader-0.6.1/raster_loader/tests/fixtures/expected_custom_multiple_column.npy`

 * *Files identical despite different names*

### Comparing `raster-loader-0.6.0/raster_loader/tests/fixtures/expected_custom_multiple_column.pkl` & `raster-loader-0.6.1/raster_loader/tests/fixtures/expected_custom_multiple_column.pkl`

 * *Files identical despite different names*

### Comparing `raster-loader-0.6.0/raster_loader/tests/fixtures/expected_default_column.npy` & `raster-loader-0.6.1/raster_loader/tests/fixtures/expected_default_column.npy`

 * *Files identical despite different names*

### Comparing `raster-loader-0.6.0/raster_loader/tests/fixtures/expected_default_column.pkl` & `raster-loader-0.6.1/raster_loader/tests/fixtures/expected_default_column.pkl`

 * *Files identical despite different names*

### Comparing `raster-loader-0.6.0/raster_loader/tests/fixtures/expected_default_multiple_column.npy` & `raster-loader-0.6.1/raster_loader/tests/fixtures/expected_default_multiple_column.npy`

 * *Files identical despite different names*

### Comparing `raster-loader-0.6.0/raster_loader/tests/fixtures/expected_multiple_column.pkl` & `raster-loader-0.6.1/raster_loader/tests/fixtures/expected_multiple_column.pkl`

 * *Files identical despite different names*

### Comparing `raster-loader-0.6.0/raster_loader/tests/fixtures/mosaic.tif` & `raster-loader-0.6.1/raster_loader/tests/fixtures/mosaic.tif`

 * *Files identical despite different names*

### Comparing `raster-loader-0.6.0/raster_loader/tests/fixtures/mosaic_cog.tif` & `raster-loader-0.6.1/raster_loader/tests/fixtures/mosaic_cog.tif`

 * *Files identical despite different names*

### Comparing `raster-loader-0.6.0/raster_loader/tests/fixtures/mosaic_cog_1_1.tif` & `raster-loader-0.6.1/raster_loader/tests/fixtures/mosaic_cog_1_1.tif`

 * *Files identical despite different names*

### Comparing `raster-loader-0.6.0/raster_loader/tests/fixtures/mosaic_cog_1_2.tif` & `raster-loader-0.6.1/raster_loader/tests/fixtures/mosaic_cog_1_2.tif`

 * *Files identical despite different names*

### Comparing `raster-loader-0.6.0/raster_loader/tests/fixtures/mosaic_cog_2_1.tif` & `raster-loader-0.6.1/raster_loader/tests/fixtures/mosaic_cog_2_1.tif`

 * *Files identical despite different names*

### Comparing `raster-loader-0.6.0/raster_loader/tests/fixtures/mosaic_cog_2_2.tif` & `raster-loader-0.6.1/raster_loader/tests/fixtures/mosaic_cog_2_2.tif`

 * *Files identical despite different names*

### Comparing `raster-loader-0.6.0/raster_loader/tests/fixtures/mosaic_cog_512.tif` & `raster-loader-0.6.1/raster_loader/tests/fixtures/mosaic_cog_512.tif`

 * *Files identical despite different names*

### Comparing `raster-loader-0.6.0/raster_loader/tests/mocks.py` & `raster-loader-0.6.1/raster_loader/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `raster-loader-0.6.0/raster_loader/tests/snowflake/test_cli.py` & `raster-loader-0.6.1/raster_loader/tests/snowflake/test_cli.py`

 * *Files identical despite different names*

### Comparing `raster-loader-0.6.0/raster_loader/tests/snowflake/test_io.py` & `raster-loader-0.6.1/raster_loader/tests/snowflake/test_io.py`

 * *Files identical despite different names*

### Comparing `raster-loader-0.6.0/raster_loader/utils.py` & `raster-loader-0.6.1/raster_loader/utils.py`

 * *Files identical despite different names*

### Comparing `raster-loader-0.6.0/raster_loader.egg-info/PKG-INFO` & `raster-loader-0.6.1/raster_loader.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raster-loader
-Version: 0.6.0
+Version: 0.6.1
 Summary: Python library for loading GIS raster data to standard cloud-based data warehouses that don't natively support raster data.
 Home-page: https://github.com/cartodb/raster-loader
 Author: CARTO
 License: BSD 3-Clause
 Keywords: carto,raster,gis,data warehouse,bigquery,snowflake
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -58,15 +58,18 @@
 ## Documentation
 
 The Raster Loader documentation is available at [raster-loader.readthedocs.io](https://raster-loader.readthedocs.io).
 
 ## Install
 
 ```bash
-pip install raster-loader
+pip install -U raster-loader
+
+pip install -U raster-loader"[bigquery]"
+pip install -U raster-loader"[snowflake]"
 ```
 
 ### Installing from source
 
 ```bash
 git clone https://github.com/cartodb/raster-loader
 cd raster-loader
```

### Comparing `raster-loader-0.6.0/raster_loader.egg-info/SOURCES.txt` & `raster-loader-0.6.1/raster_loader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `raster-loader-0.6.0/setup.cfg` & `raster-loader-0.6.1/setup.cfg`

 * *Files identical despite different names*

