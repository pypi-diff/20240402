# Comparing `tmp/dkist-1.4.0rc2.tar.gz` & `tmp/dkist-1.5.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist-1.4.0rc2.tar", last modified: Mon Feb 26 16:02:49 2024, max compression
+gzip compressed data, was "dkist-1.5.0rc1.tar", last modified: Tue Apr  2 20:54:09 2024, max compression
```

## Comparing `dkist-1.4.0rc2.tar` & `dkist-1.5.0rc1.tar`

### file list

```diff
@@ -1,230 +1,249 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:02:49.372792 dkist-1.4.0rc2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:02:49.336792 dkist-1.4.0rc2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:02:49.336792 dkist-1.4.0rc2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/.github/ISSUE_TEMPLATE/BUG_REPORT.md
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/.github/ISSUE_TEMPLATE/FEATURE_REQUEST.md
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/.github/changelog_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:02:49.336792 dkist-1.4.0rc2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/.github/workflows/prepare-release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)    22666 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-02-26 16:02:49.372792 dkist-1.4.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:02:49.336792 dkist-1.4.0rc2/changelog/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/changelog/335.trivial.rst
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/changelog/336.bugfix.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/changelog/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:02:49.336792 dkist-1.4.0rc2/dkist/
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:02:49.336792 dkist-1.4.0rc2/dkist/config/
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12152 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:02:49.340792 dkist-1.4.0rc2/dkist/data/
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/data/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)    13367 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/data/VISP_HEADER.hdr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/data/api_search_values.json
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/data/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:02:49.344792 dkist-1.4.0rc2/dkist/data/test/
--rw-r--r--   0 runner    (1001) docker     (127)     6393 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/data/test/5d_gwcs.asdf
--rw-r--r--   0 runner    (1001) docker     (127)     8295 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/data/test/AGLKO-inv.ecsv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:02:49.348792 dkist-1.4.0rc2/dkist/data/test/EIT/
--rw-r--r--   0 runner    (1001) docker     (127)   141120 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/data/test/EIT/efz20040301.000010_s.fits
--rw-r--r--   0 runner    (1001) docker     (127)   141120 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/data/test/EIT/efz20040301.020010_s.fits
--rw-r--r--   0 runner    (1001) docker     (127)   141120 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/data/test/EIT/efz20040301.030011_s.fits
--rw-r--r--   0 runner    (1001) docker     (127)   141120 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/data/test/EIT/efz20040301.040010_s.fits
--rw-r--r--   0 runner    (1001) docker     (127)   141120 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/data/test/EIT/efz20040301.050010_s.fits
--rw-r--r--   0 runner    (1001) docker     (127)   141120 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/data/test/EIT/efz20040301.060010_s.fits
--rw-r--r--   0 runner    (1001) docker     (127)   141120 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/data/test/EIT/efz20040301.080010_s.fits
--rw-r--r--   0 runner    (1001) docker     (127)   141120 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/data/test/EIT/efz20040301.090010_s.fits
--rw-r--r--   0 runner    (1001) docker     (127)   141120 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/data/test/EIT/efz20040301.100010_s.fits
--rw-r--r--   0 runner    (1001) docker     (127)   141120 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/data/test/EIT/efz20040301.110010_s.fits
--rw-r--r--   0 runner    (1001) docker     (127)   141120 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/data/test/EIT/efz20040301.120010_s.fits
--rw-r--r--   0 runner    (1001) docker     (127)    32769 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/data/test/EIT/eit_test_dataset.asdf
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/data/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    96407 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/data/test/eit_dataset-0.1.0.asdf
--rw-r--r--   0 runner    (1001) docker     (127)    96552 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/data/test/eit_dataset-0.2.0.asdf
--rw-r--r--   0 runner    (1001) docker     (127)    97195 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/data/test/eit_dataset-0.3.0.asdf
--rw-r--r--   0 runner    (1001) docker     (127)    99686 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/data/test/eit_dataset-1.0.0.asdf
--rw-r--r--   0 runner    (1001) docker     (127)    32741 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/data/test/eit_dataset-1.1.0.asdf
--rw-r--r--   0 runner    (1001) docker     (127)    32769 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/data/test/eit_dataset-1.2.0.asdf
--rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/data/test/globus_operation_ls_response.json
--rw-r--r--   0 runner    (1001) docker     (127)    42219 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/data/test/globus_search_response.json
--rw-r--r--   0 runner    (1001) docker     (127)   136848 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/data/test/large_visp.asdf.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:02:49.348792 dkist-1.4.0rc2/dkist/data/test/small_visp/
--rw-r--r--   0 runner    (1001) docker     (127)    25920 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/data/test/small_visp/0.fits
--rw-r--r--   0 runner    (1001) docker     (127)    25920 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/data/test/small_visp/1.fits
--rw-r--r--   0 runner    (1001) docker     (127)    25920 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/data/test/small_visp/2.fits
--rw-r--r--   0 runner    (1001) docker     (127)   104749 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/data/test/small_visp/test_visp.asdf
--rw-r--r--   0 runner    (1001) docker     (127)    22098 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/data/test/test_old_wcs_BRMQY.asdf
--rw-r--r--   0 runner    (1001) docker     (127)   619185 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/data/test/test_tiled_dataset-1.0.0_dataset-1.0.0.asdf
--rw-r--r--   0 runner    (1001) docker     (127)   619217 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/data/test/test_tiled_dataset-1.0.0_dataset-1.1.0.asdf
--rw-r--r--   0 runner    (1001) docker     (127)   599267 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/data/test/test_tiled_dataset-1.0.0_dataset-1.2.0.asdf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:02:49.352792 dkist-1.4.0rc2/dkist/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8400 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/dataset/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:02:49.352792 dkist-1.4.0rc2/dkist/dataset/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/dataset/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5963 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/dataset/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/dataset/tests/test_load_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/dataset/tests/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/dataset/tests/test_tiled_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4507 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/dataset/tiled_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     5086 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/dataset/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/dkist.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:02:49.352792 dkist-1.4.0rc2/dkist/extern/
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/extern/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:02:49.352792 dkist-1.4.0rc2/dkist/io/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:02:49.352792 dkist-1.4.0rc2/dkist/io/asdf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/io/asdf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:02:49.352792 dkist-1.4.0rc2/dkist/io/asdf/converters/
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/io/asdf/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/io/asdf/converters/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/io/asdf/converters/file_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6777 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/io/asdf/converters/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/io/asdf/converters/tiled_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/io/asdf/entry_points.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:02:49.352792 dkist-1.4.0rc2/dkist/io/asdf/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/io/asdf/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:02:49.356792 dkist-1.4.0rc2/dkist/io/asdf/resources/manifests/
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/io/asdf/resources/manifests/dkist-0.9.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/io/asdf/resources/manifests/dkist-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/io/asdf/resources/manifests/dkist-1.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/io/asdf/resources/manifests/dkist-1.2.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/io/asdf/resources/manifests/dkist-wcs-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/io/asdf/resources/manifests/dkist-wcs-1.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/io/asdf/resources/manifests/dkist-wcs-1.2.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:02:49.356792 dkist-1.4.0rc2/dkist/io/asdf/resources/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/io/asdf/resources/schemas/asymmetric_mapping_model-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/io/asdf/resources/schemas/coupled_compound_model-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/io/asdf/resources/schemas/dataset-0.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/io/asdf/resources/schemas/dataset-0.2.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/io/asdf/resources/schemas/dataset-0.3.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/io/asdf/resources/schemas/dataset-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/io/asdf/resources/schemas/dataset-1.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/io/asdf/resources/schemas/file_manager-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/io/asdf/resources/schemas/ravel_model-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/io/asdf/resources/schemas/tiled_dataset-0.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/io/asdf/resources/schemas/tiled_dataset-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/io/asdf/resources/schemas/varying_celestial_transform-1.0.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:02:49.356792 dkist-1.4.0rc2/dkist/io/asdf/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/io/asdf/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/io/asdf/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6763 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/io/asdf/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/io/asdf/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/io/asdf/tests/test_tiled_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/io/dask_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16964 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/io/file_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/io/level_1_dataset_schema.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/io/loaders.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:02:49.360792 dkist-1.4.0rc2/dkist/io/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/io/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10333 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/io/tests/test_file_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/io/tests/test_fits.py
--rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:02:49.360792 dkist-1.4.0rc2/dkist/net/
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/net/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7078 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/net/attr_walker.py
--rw-r--r--   0 runner    (1001) docker     (127)    13825 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/net/attrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5945 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/net/attrs_values.py
--rw-r--r--   0 runner    (1001) docker     (127)    10568 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/net/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:02:49.360792 dkist-1.4.0rc2/dkist/net/globus/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/net/globus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6420 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/net/globus/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     5378 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/net/globus/endpoints.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:02:49.360792 dkist-1.4.0rc2/dkist/net/globus/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/net/globus/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4342 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/net/globus/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     5565 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/net/globus/tests/test_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     8881 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/net/globus/tests/test_transfer.py
--rw-r--r--   0 runner    (1001) docker     (127)    12542 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/net/globus/transfer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6086 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/net/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:02:49.364792 dkist-1.4.0rc2/dkist/net/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/net/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/net/tests/strategies.py
--rw-r--r--   0 runner    (1001) docker     (127)     7207 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/net/tests/test_attr_walker.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/net/tests/test_attrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6203 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/net/tests/test_attrs_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     9132 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/net/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     9241 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/net/tests/test_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:02:49.364792 dkist-1.4.0rc2/dkist/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/tests/coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)     7490 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/tests/generate_aia_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     5393 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/tests/generate_eit_test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/tests/generate_eit_tiled_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/tests/setup_package.py
--rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/tests/test_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:02:49.364792 dkist-1.4.0rc2/dkist/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5745 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/utils/_model_to_graphviz.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5011 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/utils/inventory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/utils/sysinfo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:02:49.364792 dkist-1.4.0rc2/dkist/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/utils/tests/test_inventory.py
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/utils/tests/test_sysinfo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:02:49.364792 dkist-1.4.0rc2/dkist/wcs/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/wcs/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    31861 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/wcs/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:02:49.364792 dkist-1.4.0rc2/dkist/wcs/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5941 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/wcs/tests/test_coupled_compound_model.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    24323 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/dkist/wcs/tests/test_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:02:49.372792 dkist-1.4.0rc2/dkist.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-02-26 16:02:49.000000 dkist-1.4.0rc2/dkist.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6298 2024-02-26 16:02:49.000000 dkist-1.4.0rc2/dkist.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 16:02:49.000000 dkist-1.4.0rc2/dkist.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-02-26 16:02:49.000000 dkist-1.4.0rc2/dkist.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-02-26 16:02:49.000000 dkist-1.4.0rc2/dkist.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-26 16:02:49.000000 dkist-1.4.0rc2/dkist.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:02:49.368792 dkist-1.4.0rc2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     6421 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/docs/developer.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/docs/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:02:49.368792 dkist-1.4.0rc2/docs/logo/
--rw-r--r--   0 runner    (1001) docker     (127)    72150 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/docs/logo/icon_square.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/docs/reference.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:02:49.368792 dkist-1.4.0rc2/docs/topic_guides/
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/docs/topic_guides/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/docs/topic_guides/level1data.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6538 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/docs/topic_guides/loading.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10252 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/docs/topic_guides/net.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/docs/topic_guides/usertools.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:02:49.368792 dkist-1.4.0rc2/docs/tutorial/
--rw-r--r--   0 runner    (1001) docker     (127)     6876 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/docs/tutorial/1_astropy_and_sunpy.md
--rw-r--r--   0 runner    (1001) docker     (127)     7855 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/docs/tutorial/1_astropy_and_sunpy_NOTES.md
--rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/docs/tutorial/2_search_and_asdf_download.md
--rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/docs/tutorial/2_search_and_asdf_download_NOTES.md
--rw-r--r--   0 runner    (1001) docker     (127)     7242 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/docs/tutorial/3_the_dataset.md
--rw-r--r--   0 runner    (1001) docker     (127)     6380 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/docs/tutorial/3_the_dataset_NOTES.md
--rw-r--r--   0 runner    (1001) docker     (127)     6491 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/docs/tutorial/4_more_dataset.md
--rw-r--r--   0 runner    (1001) docker     (127)    10248 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/docs/tutorial/5_downloading_data.md
--rw-r--r--   0 runner    (1001) docker     (127)     5467 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/docs/tutorial/6_visualization.md
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/docs/tutorial/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:02:49.372792 dkist-1.4.0rc2/docs/whatsnew/
--rw-r--r--   0 runner    (1001) docker     (127)     6966 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/docs/whatsnew/1.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/docs/whatsnew/1.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/docs/whatsnew/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/docs/whatsnew/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     5362 2024-02-26 16:02:49.372792 dkist-1.4.0rc2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)       58 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-02-26 16:02:32.000000 dkist-1.4.0rc2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.110747 dkist-1.5.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/.codecov.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/.codespell-dict.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/.codespellrc
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.062747 dkist-1.5.0rc1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.074747 dkist-1.5.0rc1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/.github/ISSUE_TEMPLATE/BUG_REPORT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/.github/ISSUE_TEMPLATE/FEATURE_REQUEST.md
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/.github/ISSUE_TEMPLATE/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.074747 dkist-1.5.0rc1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/.github/workflows/prepare-release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/.github/workflows/sub_package_update.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/.rtd-environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/.ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    23150 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-04-02 20:54:09.110747 dkist-1.5.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.074747 dkist-1.5.0rc1/changelog/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/changelog/309.bugfix.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/changelog/344.trivial.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/changelog/347.feature.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/changelog/349.doc.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/changelog/361.bugfix.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/changelog/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.074747 dkist-1.5.0rc1/dkist/
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-02 20:54:08.000000 dkist-1.5.0rc1/dkist/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.074747 dkist-1.5.0rc1/dkist/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12171 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.078747 dkist-1.5.0rc1/dkist/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    13367 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/VISP_HEADER.hdr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/api_search_values.json
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.082747 dkist-1.5.0rc1/dkist/data/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     6393 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/5d_gwcs.asdf
+-rw-r--r--   0 runner    (1001) docker     (127)     8295 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/AGLKO-inv.ecsv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.086747 dkist-1.5.0rc1/dkist/data/test/EIT/
+-rw-r--r--   0 runner    (1001) docker     (127)   141120 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/EIT/efz20040301.000010_s.fits
+-rw-r--r--   0 runner    (1001) docker     (127)   141120 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/EIT/efz20040301.020010_s.fits
+-rw-r--r--   0 runner    (1001) docker     (127)   141120 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/EIT/efz20040301.030011_s.fits
+-rw-r--r--   0 runner    (1001) docker     (127)   141120 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/EIT/efz20040301.040010_s.fits
+-rw-r--r--   0 runner    (1001) docker     (127)   141120 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/EIT/efz20040301.050010_s.fits
+-rw-r--r--   0 runner    (1001) docker     (127)   141120 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/EIT/efz20040301.060010_s.fits
+-rw-r--r--   0 runner    (1001) docker     (127)   141120 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/EIT/efz20040301.080010_s.fits
+-rw-r--r--   0 runner    (1001) docker     (127)   141120 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/EIT/efz20040301.090010_s.fits
+-rw-r--r--   0 runner    (1001) docker     (127)   141120 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/EIT/efz20040301.100010_s.fits
+-rw-r--r--   0 runner    (1001) docker     (127)   141120 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/EIT/efz20040301.110010_s.fits
+-rw-r--r--   0 runner    (1001) docker     (127)   141120 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/EIT/efz20040301.120010_s.fits
+-rw-r--r--   0 runner    (1001) docker     (127)    32769 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/EIT/eit_test_dataset.asdf
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    96407 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/eit_dataset-0.1.0.asdf
+-rw-r--r--   0 runner    (1001) docker     (127)    96552 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/eit_dataset-0.2.0.asdf
+-rw-r--r--   0 runner    (1001) docker     (127)    97195 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/eit_dataset-0.3.0.asdf
+-rw-r--r--   0 runner    (1001) docker     (127)    99686 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/eit_dataset-1.0.0.asdf
+-rw-r--r--   0 runner    (1001) docker     (127)    32741 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/eit_dataset-1.1.0.asdf
+-rw-r--r--   0 runner    (1001) docker     (127)    32769 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/eit_dataset-1.2.0.asdf
+-rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/globus_operation_ls_response.json
+-rw-r--r--   0 runner    (1001) docker     (127)    42219 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/globus_search_response.json
+-rw-r--r--   0 runner    (1001) docker     (127)   136848 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/large_visp.asdf.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.086747 dkist-1.5.0rc1/dkist/data/test/small_visp/
+-rw-r--r--   0 runner    (1001) docker     (127)    25920 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/small_visp/0.fits
+-rw-r--r--   0 runner    (1001) docker     (127)    25920 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/small_visp/1.fits
+-rw-r--r--   0 runner    (1001) docker     (127)    25920 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/small_visp/2.fits
+-rw-r--r--   0 runner    (1001) docker     (127)   104749 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/small_visp/test_visp.asdf
+-rw-r--r--   0 runner    (1001) docker     (127)    22098 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/test_old_wcs_BRMQY.asdf
+-rw-r--r--   0 runner    (1001) docker     (127)   619185 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/test_tiled_dataset-1.0.0_dataset-1.0.0.asdf
+-rw-r--r--   0 runner    (1001) docker     (127)   619217 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/test_tiled_dataset-1.0.0_dataset-1.1.0.asdf
+-rw-r--r--   0 runner    (1001) docker     (127)   599267 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/test_tiled_dataset-1.0.0_dataset-1.2.0.asdf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.086747 dkist-1.5.0rc1/dkist/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8376 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/dataset/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.090747 dkist-1.5.0rc1/dkist/dataset/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/dataset/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/dataset/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/dataset/tests/test_load_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/dataset/tests/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/dataset/tests/test_tiled_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/dataset/tiled_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5097 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/dataset/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/dkist.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.090747 dkist-1.5.0rc1/dkist/extern/
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/extern/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.090747 dkist-1.5.0rc1/dkist/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.090747 dkist-1.5.0rc1/dkist/io/asdf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.090747 dkist-1.5.0rc1/dkist/io/asdf/converters/
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/converters/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/converters/file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5898 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/converters/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/converters/tiled_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/entry_points.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.090747 dkist-1.5.0rc1/dkist/io/asdf/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.090747 dkist-1.5.0rc1/dkist/io/asdf/resources/manifests/
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/resources/manifests/dkist-0.9.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/resources/manifests/dkist-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/resources/manifests/dkist-1.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/resources/manifests/dkist-1.2.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/resources/manifests/dkist-wcs-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/resources/manifests/dkist-wcs-1.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/resources/manifests/dkist-wcs-1.2.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.094747 dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/asymmetric_mapping_model-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/coupled_compound_model-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/dataset-0.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/dataset-0.2.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/dataset-0.3.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/dataset-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/dataset-1.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/file_manager-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/ravel_model-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/tiled_dataset-0.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/tiled_dataset-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/varying_celestial_transform-1.0.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.094747 dkist-1.5.0rc1/dkist/io/asdf/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6790 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/tests/test_tiled_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/dask_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16928 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/level_1_dataset_schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/loaders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.094747 dkist-1.5.0rc1/dkist/io/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10055 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/tests/test_file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/tests/test_fits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.094747 dkist-1.5.0rc1/dkist/net/
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/net/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7075 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/net/attr_walker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13842 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/net/attrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5952 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/net/attrs_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10609 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/net/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.098747 dkist-1.5.0rc1/dkist/net/globus/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/net/globus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6390 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/net/globus/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/net/globus/endpoints.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.098747 dkist-1.5.0rc1/dkist/net/globus/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/net/globus/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/net/globus/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/net/globus/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5497 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/net/globus/tests/test_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8835 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/net/globus/tests/test_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12487 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/net/globus/transfer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6065 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/net/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.098747 dkist-1.5.0rc1/dkist/net/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/net/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/net/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/net/tests/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7220 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/net/tests/test_attr_walker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/net/tests/test_attrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6237 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/net/tests/test_attrs_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9116 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/net/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9227 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/net/tests/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.098747 dkist-1.5.0rc1/dkist/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7410 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/tests/generate_aia_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5397 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/tests/generate_eit_test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/tests/generate_eit_tiled_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/tests/test_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.102747 dkist-1.5.0rc1/dkist/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5736 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/utils/_model_to_graphviz.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/utils/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/utils/sysinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.102747 dkist-1.5.0rc1/dkist/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/utils/tests/test_inventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/utils/tests/test_sysinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.102747 dkist-1.5.0rc1/dkist/wcs/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/wcs/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    26350 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/wcs/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.102747 dkist-1.5.0rc1/dkist/wcs/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/wcs/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5931 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/wcs/tests/test_coupled_compound_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24398 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/wcs/tests/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.106747 dkist-1.5.0rc1/dkist.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-04-02 20:54:09.000000 dkist-1.5.0rc1/dkist.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6678 2024-04-02 20:54:09.000000 dkist-1.5.0rc1/dkist.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 20:54:09.000000 dkist-1.5.0rc1/dkist.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-02 20:54:09.000000 dkist-1.5.0rc1/dkist.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 20:54:08.000000 dkist-1.5.0rc1/dkist.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-02 20:54:09.000000 dkist-1.5.0rc1/dkist.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-02 20:54:09.000000 dkist-1.5.0rc1/dkist.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.102747 dkist-1.5.0rc1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     6120 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/developer.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.102747 dkist-1.5.0rc1/docs/howto_guides/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/howto_guides/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/howto_guides/reproject_vbi_mosaic.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.102747 dkist-1.5.0rc1/docs/logo/
+-rw-r--r--   0 runner    (1001) docker     (127)    72150 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/logo/icon_square.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/reference.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.102747 dkist-1.5.0rc1/docs/topic_guides/
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/topic_guides/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/topic_guides/level1data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6539 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/topic_guides/loading.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10253 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/topic_guides/net.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/topic_guides/usertools.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.106747 dkist-1.5.0rc1/docs/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (127)     6876 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/tutorial/1_astropy_and_sunpy.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7855 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/tutorial/1_astropy_and_sunpy_NOTES.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/tutorial/2_search_and_asdf_download.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/tutorial/2_search_and_asdf_download_NOTES.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/tutorial/3_the_dataset.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6380 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/tutorial/3_the_dataset_NOTES.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6630 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/tutorial/4_more_dataset.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6106 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/tutorial/5_downloading_data.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/tutorial/6_visualization.md
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/tutorial/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.106747 dkist-1.5.0rc1/docs/whatsnew/
+-rw-r--r--   0 runner    (1001) docker     (127)     6966 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/whatsnew/1.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/whatsnew/1.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/whatsnew/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/whatsnew/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-02 20:54:09.110747 dkist-1.5.0rc1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)       60 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/tox.ini
```

### Comparing `dkist-1.4.0rc2/.github/ISSUE_TEMPLATE/BUG_REPORT.md` & `dkist-1.5.0rc1/.github/ISSUE_TEMPLATE/BUG_REPORT.md`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/.github/ISSUE_TEMPLATE/FEATURE_REQUEST.md` & `dkist-1.5.0rc1/.github/ISSUE_TEMPLATE/FEATURE_REQUEST.md`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/.github/workflows/main.yml` & `dkist-1.5.0rc1/.github/workflows/main.yml`

 * *Files 19% similar despite different names*

```diff
@@ -29,32 +29,55 @@
 
 jobs:
   tests:
     uses: OpenAstronomy/github-actions-workflows/.github/workflows/tox.yml@main
     with:
       default_python: '3.10'
       coverage: 'codecov'
+      posargs: '--color=yes'
       envs: |
         - linux: py312
         - linux: py311
-        - windows: py310-online
-        - macos: py39
-        - linux: build_docs
+        - windows: py311-online
+        - macos: py310
+        - linux: py310-oldestdeps
+    secrets:
+      CODECOV_TOKEN: ${{ secrets.CODECOV_TOKEN }}
+
+  docs:
+    uses: OpenAstronomy/github-actions-workflows/.github/workflows/tox.yml@main
+    with:
+      default_python: '3.10'
+      coverage: 'codecov'
+      envs: |
+        - linux: build_docs-notebooks
           pytest: false
           libraries:
             apt:
               - graphviz
-        - linux: py39-oldestdeps
     secrets:
       CODECOV_TOKEN: ${{ secrets.CODECOV_TOKEN }}
 
+  sdist_verify:
+    runs-on: ubuntu-latest
+    steps:
+      - uses: actions/checkout@v4
+      - uses: actions/setup-python@v5
+        with:
+          python-version: '3.10'
+      - run: python -m pip install -U --user build
+      - run: python -m build . --sdist
+      - run: python -m pip install -U --user twine
+      - run: python -m twine check dist/*
+
   allowed-fail-tests:
     uses: OpenAstronomy/github-actions-workflows/.github/workflows/tox.yml@main
     with:
       coverage: 'codecov'
+      posargs: '--color=yes'
       envs: |
         - linux: py311-devdeps
     secrets:
       CODECOV_TOKEN: ${{ secrets.CODECOV_TOKEN }}
 
   publish:
     needs: [tests]
```

### Comparing `dkist-1.4.0rc2/.github/workflows/prepare-release.yml` & `dkist-1.5.0rc1/.github/workflows/prepare-release.yml`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/CHANGELOG.rst` & `dkist-1.5.0rc1/CHANGELOG.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+1.4.0 (2024-02-26)
+==================
+
+Bug Fixes
+---------
+
+- Correct Fido time searching to use `endTimeMin` and `startTimeMax` (in the correct order) so that searching returns any dataset with a partially or completely overlapping time range. (`#336 <https://github.com/DKISTDC/dkist/pull/336>`_)
+
+
+Trivial/Internal Changes
+------------------------
+
+- Adjust file loading to support single-frame datasets with no time axis. (`#335 <https://github.com/DKISTDC/dkist/pull/335>`_)
+
+
 1.3.0 (2024-02-19)
 ==================
 
 Features
 --------
 
 - Call the DKIST search API to automatically determine valid data search parameters and register those with the Fido client. (`#311 <https://github.com/DKISTDC/dkist/pull/311>`_)
@@ -33,15 +48,15 @@
   The logger can be accessed as ``dkist.log`` to change log levels etc. (`#317 <https://github.com/DKISTDC/dkist/pull/317>`_)
 
 
 Bug Fixes
 ---------
 
 - Bump minimum version of asdf to 2.11.2 to pick up jsonschema bugfix. (`#313 <https://github.com/DKISTDC/dkist/pull/313>`_)
-- Change the ``appdirs`` dependancy for the maintained ``platformdirs`` package. (`#318 <https://github.com/DKISTDC/dkist/pull/318>`_)
+- Change the ``appdirs`` dependency for the maintained ``platformdirs`` package. (`#318 <https://github.com/DKISTDC/dkist/pull/318>`_)
 - Fix an unpinned minimum version of ``asdf-wcs-schemas`` causing potential read errors on newest asdf files with dkist 1.1.0. (`#320 <https://github.com/DKISTDC/dkist/pull/320>`_)
 
 
 1.1.0 (2023-10-27)
 ==================
 
 Backwards Incompatible Changes
@@ -203,15 +218,15 @@
 1.0.0b11 (2023-02-15)
 =====================
 
 Features
 --------
 
 - Add ability to page through the DKIST results and affect the page size. (`#212 <https://github.com/DKISTDC/dkist/pull/212>`_)
-- Fix, and make requried, the unit property on a dataset in ASDF files. (`#221 <https://github.com/DKISTDC/dkist/pull/221>`_)
+- Fix, and make required, the unit property on a dataset in ASDF files. (`#221 <https://github.com/DKISTDC/dkist/pull/221>`_)
 
 
 Bug Fixes
 ---------
 
 - Fix bugs in testing caused by the release of ``pytest 7.2.0``. (`#210 <https://github.com/DKISTDC/dkist/pull/210>`_)
 - Make loading a mosaiced VBI dataset work with ``Dataset.from_asdf``. (`#213 <https://github.com/DKISTDC/dkist/pull/213>`_)
@@ -301,29 +316,29 @@
 v1.0.0b4 (2022-02-16)
 =====================
 
 Features
 --------
 
 - Implement Astropy models to support spatial transforms which change with
-  a thrid pixel axis. (`#148 <https://github.com/DKISTDC/dkist/pull/148>`_)
+  a third pixel axis. (`#148 <https://github.com/DKISTDC/dkist/pull/148>`_)
 - Add ASDF serialization for `VaryingCelestialTransform` and `CoupledCompoundModel`. (`#156 <https://github.com/DKISTDC/dkist/pull/156>`_)
 
 
 Bug Fixes
 ---------
 
 - Fix asdf using old schema and tag versions when saving new files. (`#157 <https://github.com/DKISTDC/dkist/pull/157>`_)
 
 
 Trivial/Internal Changes
 ------------------------
 
 - Migate to the asdf 2.8+ ``Converter`` interface, this bumps various
-  dependancies but should have no effect on reading or writing asdf files. (`#152 <https://github.com/DKISTDC/dkist/pull/152>`_)
+  dependencies but should have no effect on reading or writing asdf files. (`#152 <https://github.com/DKISTDC/dkist/pull/152>`_)
 
 
 v1.0.0b3 (2021-11-30)
 =====================
 
 Features
 --------
@@ -346,15 +361,15 @@
 - Move file handling and download tooling onto `.Dataset.files`, which is now
   a pointer to a class which has all the information to generate the arrays.
 
   Also the loaders generated by the new `.FileManager` class now have a reference
   to the `.FileManager` which generated them, which means that the basepath can
   be dynamically generated by reference. (`#126 <https://github.com/DKISTDC/dkist/pull/126>`_)
 - Modify the `dkist.io.FileManager` class so that most of the functionality
-  exists in the new base class and the dowload method is in the separate child
+  exists in the new base class and the download method is in the separate child
   class. In addition make more of the API private to not confuse end users. (`#130 <https://github.com/DKISTDC/dkist/pull/130>`_)
 
 
 Improved Documentation
 ----------------------
 
 - Write initial guide to the user tools and tidy up the API docs (`#127 <https://github.com/DKISTDC/dkist/pull/127>`_)
@@ -390,15 +405,15 @@
 - Added support for new dataset search parameters (``hasSpectralAxis``, ``hasTemporalAxis``, ``averageDatasetSpectralSamplingMin``, ``averageDatasetSpectralSamplingMax``, ``averageDatasetSpatialSamplingMin``, ``averageDatasetSpatialSamplingMax``, ``averageDatasetTemporalSamplingMin``, ``averageDatasetTemporalSamplingMax``) (`#108 <https://github.com/DKISTDC/dkist/pull/108>`_)
 
 
 Trivial/Internal Changes
 ------------------------
 
 - Support gwcs 0.14 and ndcube 2.0.0b1 (`#86 <https://github.com/DKISTDC/dkist/pull/86>`_)
-- Update Fido client for changes in sunpy 2.1; bump the sunpy dependancy to at least 2.1rc3. (`#89 <https://github.com/DKISTDC/dkist/pull/89>`_)
+- Update Fido client for changes in sunpy 2.1; bump the sunpy dependency to at least 2.1rc3. (`#89 <https://github.com/DKISTDC/dkist/pull/89>`_)
 
 
 v0.1a2 (2020-04-29)
 ===================
 
 Features
 --------
@@ -462,14 +477,14 @@
 - Correctly parse headers when generating gwcses so that only values that change
   along that physical axis are considered. (`#21 <https://github.com/DKISTDC/dkist/pull/21>`_)
 - Reverse the ordering of gWCS objects generated by ``asdf_helpers`` as they are
   cartesian ordered not numpy ordered (`#21 <https://github.com/DKISTDC/dkist/pull/21>`_)
 - Fix incorrect compound model tree splitting when the split needed to happen at the top layer (`#23 <https://github.com/DKISTDC/dkist/pull/23>`_)
 - Fix a lot of bugs in dataset generation and wcs slicing. (`#24 <https://github.com/DKISTDC/dkist/pull/24>`_)
 - Fix incorrect chunks when creating a dask array from a loader_array. (`#26 <https://github.com/DKISTDC/dkist/pull/26>`_)
-- Add support for dask 2+ and make that the minmum version (`#68 <https://github.com/DKISTDC/dkist/pull/68>`_)
+- Add support for dask 2+ and make that the minimum version (`#68 <https://github.com/DKISTDC/dkist/pull/68>`_)
 
 
 Trivial/Internal Changes
 ------------------------
 
 - Migrate the `dkist.Dataset` class to use gWCS's APE 14 API (`#32 <https://github.com/DKISTDC/dkist/pull/32>`_)
```

### Comparing `dkist-1.4.0rc2/CONTRIBUTING.md` & `dkist-1.5.0rc1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/LICENSE.rst` & `dkist-1.5.0rc1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/PKG-INFO` & `dkist-1.5.0rc1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,17 @@
 Metadata-Version: 2.1
 Name: dkist
-Version: 1.4.0rc2
+Version: 1.5.0rc1
 Summary: DKIST User Tools
-Home-page: http://dkist.nso.edu
-Author: NSO / AURA
-Author-email: stuart@cadair.com
-License: BSD 3-Clause
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.9
+Author-email: NSO / AURA <stuart@cadair.com>
+Project-URL: repository, https://github.com/DKISTDC/dkist
+Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE.rst
-Requires-Dist: aiohttp>=3.6
+Requires-Dist: aiohttp>=3.8
 Requires-Dist: asdf>=2.11.2
 Requires-Dist: asdf-astropy>=0.2.0
 Requires-Dist: asdf-coordinates-schemas>=0.1.0
 Requires-Dist: asdf-standard>=1.0.3
 Requires-Dist: asdf-transform-schemas>=0.3.0
 Requires-Dist: asdf-unit-schemas>=0.1.0
 Requires-Dist: asdf-wcs-schemas>=0.3.0
@@ -31,33 +23,38 @@
 Requires-Dist: ndcube[plotting,reproject]>=2.0
 Requires-Dist: numpy>=1.22
 Requires-Dist: parfive[ftp]>=1.5
 Requires-Dist: platformdirs>=3.0
 Requires-Dist: sunpy[asdf,net]>=4.0.7
 Requires-Dist: tqdm>=4.63
 Provides-Extra: tests
-Requires-Dist: pytest-astropy; extra == "tests"
+Requires-Dist: pytest; extra == "tests"
+Requires-Dist: pytest-doctestplus; extra == "tests"
+Requires-Dist: pytest-cov; extra == "tests"
+Requires-Dist: pytest-remotedata; extra == "tests"
 Requires-Dist: pytest-cov; extra == "tests"
 Requires-Dist: pytest-mock; extra == "tests"
 Requires-Dist: pytest-mpl; extra == "tests"
 Requires-Dist: pytest-httpserver; extra == "tests"
 Requires-Dist: hypothesis; extra == "tests"
 Requires-Dist: tox; extra == "tests"
+Requires-Dist: pydot; extra == "tests"
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-astropy; extra == "docs"
 Requires-Dist: sphinx-gallery; extra == "docs"
 Requires-Dist: sphinx-changelog; extra == "docs"
 Requires-Dist: pytest; extra == "docs"
 Requires-Dist: sphinx_autodoc_typehints; extra == "docs"
 Requires-Dist: dkist-sphinx-theme>=1.1.2; extra == "docs"
 Requires-Dist: sphinx-design; extra == "docs"
 Requires-Dist: myst-nb; extra == "docs"
 Requires-Dist: ipywidgets; extra == "docs"
 Requires-Dist: accessible-pygments; extra == "docs"
+Requires-Dist: reproject[all]; extra == "docs"
 
 DKIST User Tools
 ================
 
 .. image:: https://img.shields.io/pypi/v/dkist.svg
    :target: https://pypi.python.org/pypi/dkist/
    :alt: PyPI for dkist package
```

### Comparing `dkist-1.4.0rc2/README.rst` & `dkist-1.5.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/changelog/README.rst` & `dkist-1.5.0rc1/changelog/README.rst`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/dkist/__init__.py` & `dkist-1.5.0rc1/dkist/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 try:
     __version__ = _version(__name__)
 except PackageNotFoundError:
     __version__ = "unknown"
 
 
-__all__ = ['TiledDataset', 'Dataset', 'load_dataset', 'system_info']
+__all__ = ["TiledDataset", "Dataset", "load_dataset", "system_info"]
 
 
 def write_default_config(overwrite=False):
     """
     Writes out the template configuration file for this version of dkist.
 
     This function will save a template config file for manual editing, if a
@@ -26,9 +26,9 @@
     version number, to facilitate comparison of changes.
     """
     import astropy.config as _config
     return _config.create_config_file("dkist", "dkist", overwrite=overwrite)
 
 
 # Do internal imports last (so logger etc is initialised)
-from dkist.dataset import Dataset, TiledDataset, load_dataset  # noqa
-from dkist.utils.sysinfo import system_info  # noqa
+from dkist.dataset import Dataset, TiledDataset, load_dataset
+from dkist.utils.sysinfo import system_info
```

### Comparing `dkist-1.4.0rc2/dkist/conftest.py` & `dkist-1.5.0rc1/dkist/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,36 +10,37 @@
 import astropy.modeling.models as m
 import astropy.units as u
 import gwcs
 import gwcs.coordinate_frames as cf
 from astropy.modeling import Model, Parameter
 from astropy.table import Table
 from astropy.time import Time
+
 from sunpy.coordinates.frames import Helioprojective
 
 from dkist import load_dataset, log
 from dkist.data.test import rootdir
 from dkist.dataset import Dataset
 from dkist.dataset.tiled_dataset import TiledDataset
 from dkist.io import FileManager
 from dkist.io.loaders import AstropyFITSLoader
 
 
 @pytest.fixture
 def caplog_dkist(caplog):
     """
-    A `dkist.log` specifc equivalent to caplog.
+    A `dkist.log` specific equivalent to caplog.
     """
     log.addHandler(caplog.handler)
     return caplog
 
 
 @pytest.fixture
 def array():
-    shape = 2**np.random.randint(2, 7, size=2)
+    shape = 2**np.random.randint(2, 7, size=2)  # noqa: NPY002
     x = np.ones(np.prod(shape)) + 10
     x = x.reshape(shape)
     return da.from_array(x, tuple(shape))
 
 
 class TwoDScale(Model):
     n_inputs = 2
@@ -60,15 +61,15 @@
     """
     A simple 1-1 gwcs that converts from pixels to arcseconds
 
     Note this WCS does not have a correct axis correlation matrix.
     """
     identity = m.Multiply(1*u.arcsec/u.pixel) & m.Multiply(1*u.arcsec/u.pixel)
     sky_frame = cf.CelestialFrame(axes_order=(0, 1),
-                                  name='helioprojective',
+                                  name="helioprojective",
                                   reference_frame=Helioprojective(obstime="2018-01-01"),
                                   unit=(u.arcsec, u.arcsec),
                                   axis_physical_types=("custom:pos.helioprojective.lat",
                                                        "custom:pos.helioprojective.lon"))
     detector_frame = cf.CoordinateFrame(name="detector", naxes=2,
                                         axes_order=(0, 1),
                                         axes_type=("pixel", "pixel"),
@@ -84,15 +85,15 @@
 def identity_gwcs_3d():
     """
     A simple 1-1 gwcs that converts from pixels to arcseconds
     """
     identity = (TwoDScale(1 * u.arcsec / u.pixel) &
                 m.Multiply(1 * u.nm / u.pixel))
 
-    sky_frame = cf.CelestialFrame(axes_order=(0, 1), name='helioprojective',
+    sky_frame = cf.CelestialFrame(axes_order=(0, 1), name="helioprojective",
                                   reference_frame=Helioprojective(obstime="2018-01-01"),
                                   axes_names=("longitude", "latitude"),
                                   unit=(u.arcsec, u.arcsec),
                                   axis_physical_types=("custom:pos.helioprojective.lon", "custom:pos.helioprojective.lat"))
     wave_frame = cf.SpectralFrame(axes_order=(2, ), unit=u.nm, axes_names=("wavelength",))
 
     frame = cf.CompositeFrame([sky_frame, wave_frame])
@@ -113,15 +114,15 @@
 def identity_gwcs_3d_temporal():
     """
     A simple 1-1 gwcs that converts from pixels to arcseconds
     """
     identity = (TwoDScale(1 * u.arcsec / u.pixel) &
                 m.Multiply(1 * u.s / u.pixel))
 
-    sky_frame = cf.CelestialFrame(axes_order=(0, 1), name='helioprojective',
+    sky_frame = cf.CelestialFrame(axes_order=(0, 1), name="helioprojective",
                                   reference_frame=Helioprojective(obstime="2018-01-01"),
                                   axes_names=("longitude", "latitude"),
                                   unit=(u.arcsec, u.arcsec),
                                   axis_physical_types=("custom:pos.helioprojective.lon", "custom:pos.helioprojective.lat"))
     time_frame = cf.TemporalFrame(Time("2020-01-01T00:00", format="isot", scale="utc"),
                                   axes_order=(2,), unit=u.s)
 
@@ -140,15 +141,15 @@
 @pytest.fixture
 def identity_gwcs_4d():
     """
     A simple 1-1 gwcs that converts from pixels to arcseconds
     """
     identity = (TwoDScale(1 * u.arcsec / u.pixel) &
                 m.Multiply(1 * u.nm/u.pixel) & m.Multiply(1 * u.s/u.pixel))
-    sky_frame = cf.CelestialFrame(axes_order=(0, 1), name='helioprojective',
+    sky_frame = cf.CelestialFrame(axes_order=(0, 1), name="helioprojective",
                                   reference_frame=Helioprojective(obstime="2018-01-01"),
                                   unit=(u.arcsec, u.arcsec),
                                   axis_physical_types=("custom:pos.helioprojective.lon", "custom:pos.helioprojective.lat"))
     wave_frame = cf.SpectralFrame(axes_order=(2, ), unit=u.nm)
     time_frame = cf.TemporalFrame(Time("2020-01-01T00:00", format="isot", scale="utc"), axes_order=(3, ), unit=u.s)
 
     frame = cf.CompositeFrame([sky_frame, wave_frame, time_frame])
@@ -163,37 +164,37 @@
     wcs.pixel_shape = (10, 20, 30, 40)
     wcs.array_shape = wcs.pixel_shape[::-1]
 
     return wcs
 
 
 # This function lives in dkist_inventory, but is copied here to avoid a test dep
-def generate_lookup_table(lookup_table, interpolation='linear', points_unit=u.pix, **kwargs):
+def generate_lookup_table(lookup_table, interpolation="linear", points_unit=u.pix, **kwargs):
     if not isinstance(lookup_table, u.Quantity):
         raise TypeError("lookup_table must be a Quantity.")
 
     # The integer location is at the centre of the pixel.
     points = (np.arange(lookup_table.size) - 0) * points_unit
 
     kwargs = {
-        'bounds_error': False,
-        'fill_value': np.nan,
-        'method': interpolation,
+        "bounds_error": False,
+        "fill_value": np.nan,
+        "method": interpolation,
         **kwargs
         }
 
     return m.Tabular1D(points, lookup_table, **kwargs)
 
 
 @pytest.fixture
 def identity_gwcs_5d_stokes(identity_gwcs_4d):
     stokes_frame = cf.StokesFrame(axes_order=(4,))
-    stokes_model = generate_lookup_table([1, 2, 3, 4] * u.one, interpolation='nearest')
+    stokes_model = generate_lookup_table([1, 2, 3, 4] * u.one, interpolation="nearest")
     transform = identity_gwcs_4d.forward_transform
-    frame = cf.CompositeFrame(identity_gwcs_4d.output_frame.frames + [stokes_frame])
+    frame = cf.CompositeFrame([*identity_gwcs_4d.output_frame.frames, stokes_frame])
 
     detector_frame = cf.CoordinateFrame(name="detector", naxes=5,
                                         axes_order=(0, 1, 2, 3, 4),
                                         axes_type=("pixel", "pixel", "pixel", "pixel", "pixel"),
                                         axes_names=("x", "y", "z", "t", "s"),
                                         unit=(u.pix, u.pix, u.pix, u.pix, u.pix))
 
@@ -204,45 +205,45 @@
 
     return wcs
 
 
 @pytest.fixture
 def dataset(array, identity_gwcs):
     meta = {
-        'inventory': {
-            'bucket': 'data',
-            'datasetId': 'test_dataset',
-            'primaryProposalId': 'test_proposal',
-            'asdfObjectKey': 'test_proposal/test_dataset/test_dataset.asdf',
-            'browseMovieObjectKey': 'test_proposal/test_dataset/test_dataset.mp4',
-            'qualityReportObjectKey': 'test_proposal/test_dataset/test_dataset.pdf',
-            'wavelengthMin': 0,
-            'wavelengthMax': 0,
+        "inventory": {
+            "bucket": "data",
+            "datasetId": "test_dataset",
+            "primaryProposalId": "test_proposal",
+            "asdfObjectKey": "test_proposal/test_dataset/test_dataset.asdf",
+            "browseMovieObjectKey": "test_proposal/test_dataset/test_dataset.mp4",
+            "qualityReportObjectKey": "test_proposal/test_dataset/test_dataset.pdf",
+            "wavelengthMin": 0,
+            "wavelengthMax": 0,
         },
-        'headers': Table()
+        "headers": Table()
     }
 
     identity_gwcs.array_shape = array.shape
     identity_gwcs.pixel_shape = array.shape[::-1]
     ds = Dataset(array, wcs=identity_gwcs, meta=meta, unit=u.count)
     # Sanity checks
     assert ds.data is array
     assert ds.wcs is identity_gwcs
 
     # Construct the filename here as a scalar array to make sure that works as
     # it's what dkist-inventory does
-    ds._file_manager = FileManager.from_parts(np.array('test1.fits'), 0, 'float', array.shape,
+    ds._file_manager = FileManager.from_parts(np.array("test1.fits"), 0, "float", array.shape,
                                               loader=AstropyFITSLoader)
 
     return ds
 
 
 @pytest.fixture
 def empty_meta():
-    return {'inventory': {}, 'headers': {}}
+    return {"inventory": {}, "headers": {}}
 
 
 @pytest.fixture
 def dataset_3d(identity_gwcs_3d, empty_meta):
     shape = (25, 50, 50)
     x = np.ones(shape)
     array = da.from_array(x, tuple(shape))
@@ -265,48 +266,48 @@
     return Dataset(array, wcs=identity_gwcs_4d, meta=empty_meta, unit=u.count)
 
 
 @pytest.fixture
 def eit_dataset():
     eitdir = Path(rootdir) / "EIT"
     with asdf.open(eitdir / "eit_test_dataset.asdf") as f:
-        return f.tree['dataset']
+        return f.tree["dataset"]
 
 
 @pytest.fixture
 def simple_tiled_dataset(dataset):
     datasets = [copy.deepcopy(dataset) for i in range(4)]
     for ds in datasets:
-        ds.meta['inventory'] = dataset.meta['inventory']
+        ds.meta["inventory"] = dataset.meta["inventory"]
     dataset_array = np.array(datasets).reshape((2,2))
-    return TiledDataset(dataset_array, dataset.meta['inventory'])
+    return TiledDataset(dataset_array, dataset.meta["inventory"])
 
 
 @pytest.fixture
 def small_visp_dataset():
     """
     This fixture is used to test when the array in the FITS file has a length
     one NAXIS 3.
     """
-    # This asdf file wont work with sunpy less than 4
+    # This asdf file won't work with sunpy less than 4
     pytest.importorskip("sunpy", "4.0.0")
 
     # This dataset was generated by the following code:
     # from dkist_data_simulator.spec214.visp import SimpleVISPDataset
     # from dkist_inventory.asdf_generator import dataset_from_fits
     # import astropy.units as u
 
     # ds = SimpleVISPDataset(n_maps=1, n_steps=3, n_stokes=1, time_delta=10,
     #                        linewave=500*u.nm, detector_shape=(10, 25))
     # ds.generate_files(vispdir)
     # dataset_from_fits(vispdir, "test_visp.asdf")
 
     vispdir = Path(rootdir) / "small_visp"
     with asdf.open(vispdir / "test_visp.asdf") as f:
-        return f.tree['dataset']
+        return f.tree["dataset"]
 
 
 @pytest.fixture(scope="session")
 def large_visp_dataset(tmp_path_factory):
     # This dataset was generated by the following code:
     # from dkist_data_simulator.spec214.visp import SimpleVISPDataset
     # from dkist_inventory.asdf_generator import dataset_from_fits
```

### Comparing `dkist-1.4.0rc2/dkist/data/VISP_HEADER.hdr` & `dkist-1.5.0rc1/dkist/data/VISP_HEADER.hdr`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/dkist/data/api_search_values.json` & `dkist-1.5.0rc1/dkist/data/api_search_values.json`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/dkist/data/test/5d_gwcs.asdf` & `dkist-1.5.0rc1/dkist/data/test/5d_gwcs.asdf`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/dkist/data/test/AGLKO-inv.ecsv` & `dkist-1.5.0rc1/dkist/data/test/AGLKO-inv.ecsv`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/dkist/data/test/EIT/efz20040301.000010_s.fits` & `dkist-1.5.0rc1/dkist/data/test/EIT/efz20040301.000010_s.fits`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/dkist/data/test/EIT/efz20040301.020010_s.fits` & `dkist-1.5.0rc1/dkist/data/test/EIT/efz20040301.020010_s.fits`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/dkist/data/test/EIT/efz20040301.030011_s.fits` & `dkist-1.5.0rc1/dkist/data/test/EIT/efz20040301.030011_s.fits`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/dkist/data/test/EIT/efz20040301.040010_s.fits` & `dkist-1.5.0rc1/dkist/data/test/EIT/efz20040301.040010_s.fits`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/dkist/data/test/EIT/efz20040301.050010_s.fits` & `dkist-1.5.0rc1/dkist/data/test/EIT/efz20040301.050010_s.fits`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/dkist/data/test/EIT/efz20040301.060010_s.fits` & `dkist-1.5.0rc1/dkist/data/test/EIT/efz20040301.060010_s.fits`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/dkist/data/test/EIT/efz20040301.080010_s.fits` & `dkist-1.5.0rc1/dkist/data/test/EIT/efz20040301.080010_s.fits`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/dkist/data/test/EIT/efz20040301.090010_s.fits` & `dkist-1.5.0rc1/dkist/data/test/EIT/efz20040301.090010_s.fits`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/dkist/data/test/EIT/efz20040301.100010_s.fits` & `dkist-1.5.0rc1/dkist/data/test/EIT/efz20040301.100010_s.fits`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/dkist/data/test/EIT/efz20040301.110010_s.fits` & `dkist-1.5.0rc1/dkist/data/test/EIT/efz20040301.110010_s.fits`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/dkist/data/test/EIT/efz20040301.120010_s.fits` & `dkist-1.5.0rc1/dkist/data/test/EIT/efz20040301.120010_s.fits`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/dkist/data/test/EIT/eit_test_dataset.asdf` & `dkist-1.5.0rc1/dkist/data/test/EIT/eit_test_dataset.asdf`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/dkist/data/test/eit_dataset-0.1.0.asdf` & `dkist-1.5.0rc1/dkist/data/test/eit_dataset-0.1.0.asdf`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/dkist/data/test/eit_dataset-0.2.0.asdf` & `dkist-1.5.0rc1/dkist/data/test/eit_dataset-0.2.0.asdf`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/dkist/data/test/eit_dataset-0.3.0.asdf` & `dkist-1.5.0rc1/dkist/data/test/eit_dataset-0.3.0.asdf`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/dkist/data/test/eit_dataset-1.0.0.asdf` & `dkist-1.5.0rc1/dkist/data/test/eit_dataset-1.0.0.asdf`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/dkist/data/test/eit_dataset-1.1.0.asdf` & `dkist-1.5.0rc1/dkist/data/test/eit_dataset-1.1.0.asdf`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/dkist/data/test/eit_dataset-1.2.0.asdf` & `dkist-1.5.0rc1/dkist/data/test/eit_dataset-1.2.0.asdf`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/dkist/data/test/globus_operation_ls_response.json` & `dkist-1.5.0rc1/dkist/data/test/globus_operation_ls_response.json`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/dkist/data/test/globus_search_response.json` & `dkist-1.5.0rc1/dkist/data/test/globus_search_response.json`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/dkist/data/test/large_visp.asdf.gz` & `dkist-1.5.0rc1/dkist/data/test/large_visp.asdf.gz`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/dkist/data/test/small_visp/0.fits` & `dkist-1.5.0rc1/dkist/data/test/small_visp/0.fits`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/dkist/data/test/small_visp/1.fits` & `dkist-1.5.0rc1/dkist/data/test/small_visp/1.fits`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/dkist/data/test/small_visp/2.fits` & `dkist-1.5.0rc1/dkist/data/test/small_visp/2.fits`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/dkist/data/test/small_visp/test_visp.asdf` & `dkist-1.5.0rc1/dkist/data/test/small_visp/test_visp.asdf`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/dkist/data/test/test_old_wcs_BRMQY.asdf` & `dkist-1.5.0rc1/dkist/data/test/test_old_wcs_BRMQY.asdf`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/dkist/data/test/test_tiled_dataset-1.0.0_dataset-1.0.0.asdf` & `dkist-1.5.0rc1/dkist/data/test/test_tiled_dataset-1.0.0_dataset-1.0.0.asdf`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/dkist/data/test/test_tiled_dataset-1.0.0_dataset-1.1.0.asdf` & `dkist-1.5.0rc1/dkist/data/test/test_tiled_dataset-1.0.0_dataset-1.1.0.asdf`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/dkist/data/test/test_tiled_dataset-1.0.0_dataset-1.2.0.asdf` & `dkist-1.5.0rc1/dkist/data/test/test_tiled_dataset-1.0.0_dataset-1.2.0.asdf`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/dkist/dataset/dataset.py` & `dkist-1.5.0rc1/dkist/dataset/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from textwrap import dedent
 
 import numpy as np
 
 import gwcs
 from astropy.wcs.wcsapi.wrappers import SlicedLowLevelWCS
+
 from ndcube.ndcube import NDCube, NDCubeLinkedDescriptor
 
 from dkist.io.file_manager import FileManager
 from dkist.utils.decorators import deprecated
 
 from .utils import dataset_info_str
 
-__all__ = ['Dataset']
+__all__ = ["Dataset"]
 
 
 class FileManagerDescriptor(NDCubeLinkedDescriptor):
     """
     This is a special version of the NDCubeLinked descriptor which gives a
     FileManager object a reference to the cube when it is assigned to the
     attribute.
@@ -52,15 +53,15 @@
         The WCS object containing the axes' information, optional only if
         ``data`` is an `astropy.nddata.NDData` object.
 
     uncertainty : any type, optional
         Uncertainty in the dataset. Should have an attribute uncertainty_type
         that defines what kind of uncertainty is stored, for example "std"
         for standard deviation or "var" for variance. A metaclass defining such
-        an interface is `~astropy.nddata.NDUncertainty` - but isn’t mandatory.
+        an interface is `~astropy.nddata.NDUncertainty` - but isn't mandatory.
         If the uncertainty has no such attribute the uncertainty is stored as
         `~astropy.nddata.UnknownUncertainty`.
         Defaults to None.
 
     mask : any type, optional
         Mask for the dataset. Masks should follow the numpy convention
         that valid data points are marked by `False` and invalid ones with `True`.
@@ -147,15 +148,15 @@
                 # mgrid has to have a stop, so if it's missing from the slice we
                 # add it.
                 stop = slc.stop or files_shape[ax]
                 slc = slice(slc.start, stop, slc.step)
             file_idx.append(slc)
         grid = np.mgrid[tuple(file_idx)]
         file_idx = tuple(grid[i].ravel() for i in range(grid.shape[0]))
-        flat_idx = np.ravel_multi_index(file_idx[::-1], files_shape[::-1], order='F')
+        flat_idx = np.ravel_multi_index(file_idx[::-1], files_shape[::-1], order="F")
 
         # Explicitly create new header table to ensure consistency
         # Otherwise would return a reference sometimes and a new table others
         return self.meta["headers"].copy()[flat_idx]
 
     """
     Properties.
@@ -186,17 +187,17 @@
         A `~.FileManager` helper for interacting with the files backing the data in this ``Dataset``.
         """
         return self._file_manager
 
     @property
     def inventory(self):
         """
-        Convenience attribute to acces the inventory metadata.
+        Convenience attribute to access the inventory metadata.
         """
-        return self.meta['inventory']
+        return self.meta["inventory"]
 
     """
     Dataset loading and saving routines.
     """
 
     @classmethod
     @deprecated(since="1.0.0", alternative="load_dataset")
@@ -222,12 +223,11 @@
     """
 
     def __repr__(self):
         """
         Overload the NDData repr because it does not play nice with the dask delayed io.
         """
         prefix = object.__repr__(self)
-        output = dedent(f"{prefix}\n{self.__str__()}")
-        return output
+        return dedent(f"{prefix}\n{self.__str__()}")
 
     def __str__(self):
         return dataset_info_str(self)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `dkist-1.4.0rc2/dkist/dataset/loader.py` & `dkist-1.5.0rc1/dkist/dataset/loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,29 +119,30 @@
     A path object representing a directory or an ASDF file.
     """
     path = path.expanduser()
     if not path.is_dir():
         if not path.exists():
             raise ValueError(f"{path} does not exist.")
         return _load_from_asdf(path)
-    else:
-        return _load_from_directory(path)
+
+    return _load_from_directory(path)
 
 
 def _load_from_directory(directory):
     """
     Construct a `~dkist.dataset.Dataset` from a directory containing one
     asdf file and a collection of FITS files.
     """
     base_path = Path(directory).expanduser()
     asdf_files = tuple(base_path.glob("*.asdf"))
 
     if not asdf_files:
         raise ValueError(f"No asdf file found in directory {base_path}.")
-    elif len(asdf_files) > 1:
+
+    if len(asdf_files) > 1:
         return _load_from_iterable(asdf_files)
 
     asdf_file = asdf_files[0]
 
     return _load_from_asdf(asdf_file)
 
 
@@ -152,15 +153,15 @@
     from dkist.dataset import TiledDataset
     filepath = Path(filepath).expanduser()
     base_path = filepath.parent
     try:
         with importlib_resources.as_file(importlib_resources.files("dkist.io") / "level_1_dataset_schema.yaml") as schema_path:
             with asdf.open(filepath, custom_schema=schema_path.as_posix(),
                            lazy_load=False, copy_arrays=True) as ff:
-                ds = ff.tree['dataset']
+                ds = ff.tree["dataset"]
                 if isinstance(ds, TiledDataset):
                     for sub in ds.flat:
                         sub.files.basepath = base_path
                 else:
                     ds.files.basepath = base_path
                 return ds
 
@@ -179,13 +180,12 @@
             name = f"{t.__module__}.{name}"
         known_types_docs[name] = func.__doc__.strip()
     return known_types_docs
 
 
 def _formatted_types_docstring(known_types):
     lines = [f"| `{fqn}` - {doc}" for fqn, doc in known_types.items()]
-    docstring = '\n        '.join(lines)
-    return docstring
+    return "\n        ".join(lines)
 
 
 load_dataset.__doc__ = load_dataset.__doc__.format(types_list=_formatted_types_docstring(_known_types_docs()),
                                                    types=", ".join([f"`{t}`" for t in _known_types_docs().keys()]))
```

### Comparing `dkist-1.4.0rc2/dkist/dataset/tests/test_dataset.py` & `dkist-1.5.0rc1/dkist/dataset/tests/test_dataset.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import os
 from pathlib import Path
 
 import dask.array as da
 import numpy as np
 import pytest
 
 import asdf
@@ -16,15 +15,15 @@
 from dkist.io import FileManager
 from dkist.utils.exceptions import DKISTDeprecationWarning
 
 
 @pytest.fixture
 def invalid_asdf(tmp_path):
     filename = Path(tmp_path / "test.asdf")
-    tree = {'spam': 'eggs'}
+    tree = {"spam": "eggs"}
     with asdf.AsdfFile(tree=tree) as af:
         af.write_to(filename)
     return filename
 
 
 def test_load_invalid_asdf(invalid_asdf):
     with pytest.raises(TypeError):
@@ -34,18 +33,18 @@
 def test_missing_quality(dataset):
     assert dataset.quality_report is None
 
 
 def test_init_missing_meta_keys(identity_gwcs):
     data = np.zeros(identity_gwcs.array_shape)
     with pytest.raises(ValueError, match=".*must contain the headers table."):
-        Dataset(data, wcs=identity_gwcs, meta={'inventory': {}})
+        Dataset(data, wcs=identity_gwcs, meta={"inventory": {}})
 
     with pytest.raises(ValueError, match=".*must contain the inventory record."):
-        Dataset(data, wcs=identity_gwcs, meta={'headers': {}})
+        Dataset(data, wcs=identity_gwcs, meta={"headers": {}})
 
 
 def test_repr(dataset, dataset_3d):
     r = repr(dataset)
     assert str(dataset.data) in r
     r = repr(dataset_3d)
     assert str(dataset_3d.data) in r
@@ -68,74 +67,70 @@
 
 def test_dimensions(dataset, dataset_3d):
     for ds in [dataset, dataset_3d]:
         assert_quantity_allclose(ds.dimensions, ds.data.shape*u.pix)
 
 
 def test_load_from_directory():
-    ds = load_dataset(os.path.join(rootdir, 'EIT'))
+    ds = load_dataset(rootdir / "EIT")
     assert isinstance(ds.data, da.Array)
     assert isinstance(ds.wcs, gwcs.WCS)
     assert_quantity_allclose(ds.dimensions, (11, 128, 128)*u.pix)
-    assert ds.files.basepath == Path(os.path.join(rootdir, 'EIT'))
+    assert ds.files.basepath == Path(rootdir / "EIT")
 
 
 def test_from_directory_no_asdf(tmp_path):
-    with pytest.raises(ValueError) as e:
+    with pytest.raises(ValueError, match="No asdf file found"):
         load_dataset(tmp_path)
-        assert "No asdf file found" in str(e)
 
 
 def test_from_not_directory():
-    with pytest.raises(ValueError) as e:
+    with pytest.raises(ValueError, match="does not exist"):
         load_dataset(rootdir / "notadirectory")
-        assert "directory argument" in str(e)
 
 
 def test_load_tiled_dataset():
-    ds = load_dataset(os.path.join(rootdir, 'test_tiled_dataset-1.0.0_dataset-1.1.0.asdf'))
+    ds = load_dataset(rootdir / "test_tiled_dataset-1.0.0_dataset-1.1.0.asdf")
     assert isinstance(ds, TiledDataset)
     assert ds.shape == (3, 3)
 
 
 def test_load_with_old_methods():
     with pytest.warns(DKISTDeprecationWarning):
-        ds = Dataset.from_directory(os.path.join(rootdir, 'EIT'))
+        ds = Dataset.from_directory(rootdir / "EIT")
         assert isinstance(ds.data, da.Array)
         assert isinstance(ds.wcs, gwcs.WCS)
         assert_quantity_allclose(ds.dimensions, (11, 128, 128)*u.pix)
-        assert ds.files.basepath == Path(os.path.join(rootdir, 'EIT'))
+        assert ds.files.basepath == Path(rootdir / "EIT")
 
-    with pytest.warns(DKISTDeprecationWarning) as e:
-        ds = Dataset.from_asdf(os.path.join(rootdir, 'EIT', "eit_test_dataset.asdf"))
+    with pytest.warns(DKISTDeprecationWarning):
+        ds = Dataset.from_asdf(rootdir / "EIT" / "eit_test_dataset.asdf")
         assert isinstance(ds.data, da.Array)
         assert isinstance(ds.wcs, gwcs.WCS)
         assert_quantity_allclose(ds.dimensions, (11, 128, 128)*u.pix)
-        assert ds.files.basepath == Path(os.path.join(rootdir, 'EIT'))
+        assert ds.files.basepath == Path(rootdir / "EIT")
 
 
 def test_from_directory_not_dir():
-    with pytest.raises(ValueError) as e:
-        load_dataset(rootdir / 'EIT' / 'eit_2004-03-01T00_00_10.515000.asdf')
-        assert "must be a directory" in str(e)
+    with pytest.raises(ValueError, match="asdf does not exist"):
+        load_dataset(rootdir / "EIT" / "eit_2004-03-01T00_00_10.515000.asdf")
 
 
 def test_load_with_invalid_input():
-    with pytest.raises(TypeError) as e:
+    with pytest.raises(TypeError, match="Input type .* not recognised."):
         load_dataset(42)
-        assert "Input type not recognised." in str(e)
 
 
 def test_crop_few_slices(dataset_4d):
     sds = dataset_4d[0, 0]
     assert sds.wcs.world_n_dim == 2
 
 
 def test_file_manager():
-    dataset = load_dataset(os.path.join(rootdir, 'EIT'))
+    dataset = load_dataset(rootdir / "EIT")
     assert dataset.files is dataset._file_manager
     with pytest.raises(AttributeError):
         dataset.files = 10
 
     assert len(dataset.files.filenames) == 11
     assert len(dataset.files.filenames) == 11
 
@@ -145,31 +140,31 @@
 
 
 def test_no_file_manager(dataset_3d):
     assert dataset_3d.files is None
 
 
 def test_inventory_propery():
-    dataset = load_dataset(os.path.join(rootdir, 'EIT'))
-    assert dataset.inventory == dataset.meta['inventory']
+    dataset = load_dataset(rootdir / "EIT")
+    assert dataset.inventory == dataset.meta["inventory"]
 
 
 def test_header_slicing_single_index():
-    dataset = load_dataset(os.path.join(rootdir, 'EIT'))
+    dataset = load_dataset(rootdir / "EIT")
     idx = 5
     sliced = dataset[idx]
 
     sliced_headers = dataset.headers[idx]
     # Filenames in the header don't match the names of the files because why would you expect those things to be the same
-    sliced_header_files = sliced_headers['FILENAME'] + '_s.fits'
+    sliced_header_files = sliced_headers["FILENAME"] + "_s.fits"
 
     assert len(sliced.files.filenames) == 1
     assert isinstance(sliced_headers, Row)
     assert sliced.files.filenames[0] == sliced_header_files
-    assert (sliced.headers['DINDEX3'] == sliced_headers['DINDEX3']).all()
+    assert (sliced.headers["DINDEX3"] == sliced_headers["DINDEX3"]).all()
 
 
 def test_header_slicing_3D_slice(large_visp_dataset):
     dataset = large_visp_dataset
     idx = np.s_[:2, 10:15, 0]
     sliced = dataset[idx]
 
@@ -177,9 +172,9 @@
     grid = np.mgrid[{tuple: file_idx, slice: (file_idx,)}[type(file_idx)]]
     file_idx = tuple(grid[i].ravel() for i in range(np.prod(grid.shape[:-2])))
 
     flat_idx = np.ravel_multi_index(file_idx, dataset.data.shape[:-2])
 
     sliced_headers = dataset.headers[flat_idx]
 
-    assert len(sliced.files.filenames) == len(sliced_headers['FILENAME']) == len(sliced.headers)
-    assert (sliced.headers['DINDEX3', 'DINDEX4'] == sliced_headers['DINDEX3', 'DINDEX4']).all()
+    assert len(sliced.files.filenames) == len(sliced_headers["FILENAME"]) == len(sliced.headers)
+    assert (sliced.headers["DINDEX3", "DINDEX4"] == sliced_headers["DINDEX3", "DINDEX4"]).all()
```

### Comparing `dkist-1.4.0rc2/dkist/dataset/tests/test_load_dataset.py` & `dkist-1.5.0rc1/dkist/dataset/tests/test_load_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,55 +45,55 @@
 @pytest.fixture
 def fixture_finder(request):
     if isinstance(request.param, (list, tuple)):
         return [request.getfixturevalue(i) for i in request.param]
     return request.getfixturevalue(request.param)
 
 
-@pytest.mark.parametrize("fixture_finder", (
+@pytest.mark.parametrize("fixture_finder", [
         "asdf_path",
         "asdf_str",
         "single_asdf_in_folder",
         "single_asdf_in_folder_str",
-    ),
+    ],
     indirect=True
 )
 def test_load_single_dataset(fixture_finder):
     ds = load_dataset(fixture_finder)
     assert isinstance(ds, Dataset)
 
 
-@pytest.mark.parametrize("fixture_finder", (
+@pytest.mark.parametrize("fixture_finder", [
         ["asdf_path", "asdf_str", "single_asdf_in_folder", "single_asdf_in_folder_str"],
         ("asdf_path", "asdf_str", "single_asdf_in_folder", "single_asdf_in_folder_str"),
-    ),
+    ],
     indirect=True
 )
 def test_load_multiple(fixture_finder):
     datasets = load_dataset(fixture_finder)
     assert isinstance(datasets, list)
-    assert all([isinstance(ds, Dataset) for ds in datasets])
+    assert all(isinstance(ds, Dataset) for ds in datasets)
 
 
 def test_load_from_results(asdf_path, asdf_str):
     res = Results([asdf_path])
     ds = load_dataset(res)
     assert isinstance(ds, Dataset)
 
     res = Results([asdf_str, asdf_str])
     ds = load_dataset(res)
     assert isinstance(ds, list)
-    assert all([isinstance(ds, Dataset) for ds in ds])
+    assert all(isinstance(ds, Dataset) for ds in ds)
 
 
 def test_multiple_from_dir(multiple_asdf_in_folder):
     ds = load_dataset(multiple_asdf_in_folder)
     assert isinstance(ds, list)
     assert len(ds) == 2
-    assert all([isinstance(d, Dataset) for d in ds])
+    assert all(isinstance(d, Dataset) for d in ds)
 
 
 def test_tiled_dataset(asdf_tileddataset_path):
     ds = load_dataset(asdf_tileddataset_path)
     assert isinstance(ds, TiledDataset)
```

### Comparing `dkist-1.4.0rc2/dkist/dataset/tests/test_plotting.py` & `dkist-1.5.0rc1/dkist/dataset/tests/test_plotting.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 import numpy as np
 import pytest
 
 from astropy.visualization.wcsaxes import WCSAxes
 
 
 @pytest.mark.mpl_image_compare
-@pytest.mark.parametrize("aslice", (np.s_[0, :, :], np.s_[:, 0, :], np.s_[:, :, 0]))
+@pytest.mark.parametrize("aslice", [np.s_[0, :, :], np.s_[:, 0, :], np.s_[:, :, 0]])
 def test_dataset_projection(dataset_3d, aslice):
     pytest.importorskip("ndcube", "2.0.2")  # https://github.com/sunpy/ndcube/pull/509
     ds = dataset_3d[aslice]
     fig = plt.figure()
     ax = plt.subplot(projection=ds)
     assert isinstance(ax, WCSAxes)
     return fig
 
 
 @pytest.mark.mpl_image_compare
-@pytest.mark.parametrize("aslice", (np.s_[0, :, :], np.s_[:, 0, :], np.s_[:, :, 0]))
+@pytest.mark.parametrize("aslice", [np.s_[0, :, :], np.s_[:, 0, :], np.s_[:, :, 0]])
 def test_2d_plot(dataset_3d, aslice):
     fig = plt.figure()
     dataset_3d[aslice].plot()
     return fig
 
 
 @pytest.mark.mpl_image_compare
```

### Comparing `dkist-1.4.0rc2/dkist/dataset/tests/test_tiled_dataset.py` & `dkist-1.5.0rc1/dkist/dataset/tests/test_tiled_dataset.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,56 +6,56 @@
 from dkist import Dataset, TiledDataset
 
 
 def test_tiled_dataset(simple_tiled_dataset, dataset):
     assert isinstance(simple_tiled_dataset, TiledDataset)
     assert simple_tiled_dataset._data[0, 0] in simple_tiled_dataset
     assert 5 not in simple_tiled_dataset
-    assert all([isinstance(t, Dataset) for t in simple_tiled_dataset.flat])
-    assert all([t.shape == (2,) for t in simple_tiled_dataset])
-    assert simple_tiled_dataset.inventory is dataset.meta['inventory']
+    assert all(isinstance(t, Dataset) for t in simple_tiled_dataset.flat)
+    assert all(t.shape == (2,) for t in simple_tiled_dataset)
+    assert simple_tiled_dataset.inventory is dataset.meta["inventory"]
     assert simple_tiled_dataset.shape == (2, 2)
 
 
-@pytest.mark.parametrize("aslice", (np.s_[0,0],
+@pytest.mark.parametrize("aslice", [np.s_[0,0],
                                     np.s_[0],
                                     np.s_[...,0],
                                     np.s_[:,1],
                                     np.s_[1,1],
-                                    np.s_[0:2, :]))
+                                    np.s_[0:2, :]])
 def test_tiled_dataset_slice(simple_tiled_dataset, aslice):
     assert np.all(simple_tiled_dataset[aslice] == simple_tiled_dataset._data[aslice])
 
 
 def test_tiled_dataset_headers(simple_tiled_dataset, dataset):
-    assert len(simple_tiled_dataset.combined_headers) == len(dataset.meta['headers']) * 4
-    assert simple_tiled_dataset.combined_headers.colnames == dataset.meta['headers'].colnames
+    assert len(simple_tiled_dataset.combined_headers) == len(dataset.meta["headers"]) * 4
+    assert simple_tiled_dataset.combined_headers.colnames == dataset.meta["headers"].colnames
 
 
 def test_tiled_dataset_invalid_construction(dataset, dataset_4d):
     with pytest.raises(ValueError, match="inventory record of the first dataset"):
         TiledDataset(np.array((dataset, dataset_4d)))
 
     with pytest.raises(ValueError, match="physical types do not match"):
-        TiledDataset(np.array((dataset, dataset_4d)), inventory=dataset.meta['inventory'])
+        TiledDataset(np.array((dataset, dataset_4d)), inventory=dataset.meta["inventory"])
 
     ds2 = copy.deepcopy(dataset)
-    ds2.meta['inventory'] = {'hello': 'world'}
+    ds2.meta["inventory"] = {"hello": "world"}
     with pytest.raises(ValueError, match="inventory records of all the datasets"):
-        TiledDataset(np.array((dataset, ds2)), dataset.meta['inventory'])
+        TiledDataset(np.array((dataset, ds2)), dataset.meta["inventory"])
 
 
 def test_tiled_dataset_from_components(dataset):
     shape = (2, 2)
     file_managers = [dataset._file_manager] * 4
     wcses = [dataset.wcs] * 4
-    header_tables = [dataset.meta['headers']] * 4
-    inventory = dataset.meta['inventory']
+    header_tables = [dataset.meta["headers"]] * 4
+    inventory = dataset.meta["inventory"]
 
     tiled_ds = TiledDataset._from_components(shape, file_managers, wcses, header_tables, inventory)
     assert isinstance(tiled_ds, TiledDataset)
     assert tiled_ds.shape == shape
-    assert all([isinstance(t, Dataset) for t in tiled_ds.flat])
+    assert all(isinstance(t, Dataset) for t in tiled_ds.flat)
     for ds, fm, headers in zip(tiled_ds.flat, file_managers, header_tables):
         assert ds.files == fm
-        assert ds.meta['inventory'] is inventory
-        assert ds.meta['headers'] is headers
+        assert ds.meta["inventory"] is inventory
+        assert ds.meta["headers"] is headers
```

### Comparing `dkist-1.4.0rc2/dkist/dataset/tiled_dataset.py` & `dkist-1.5.0rc1/dkist/dataset/tiled_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 import numpy as np
 
 from astropy.table import vstack
 
 from .dataset import Dataset
 
-__all__ = ['TiledDataset']
+__all__ = ["TiledDataset"]
 
 
 class TiledDataset(Collection):
     """
     Holds a grid of `.Dataset` objects.
 
     In the case where multiple images are taken in different locations on the
@@ -62,15 +62,15 @@
 
     def __init__(self, dataset_array, inventory=None):
         self._data = np.array(dataset_array, dtype=object)
         self._inventory = inventory or {}
         self._validate_component_datasets(self._data, inventory)
 
     def __contains__(self, x):
-        return any([ele is x for ele in self._data.flat])
+        return any(ele is x for ele in self._data.flat)
 
     def __len__(self):
         return self._data.__len__()
 
     def __iter__(self):
         return self._data.__iter__()
```

### Comparing `dkist-1.4.0rc2/dkist/dataset/utils.py` & `dkist-1.5.0rc1/dkist/dataset/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Helper functions for the Dataset class.
 """
 
 import numpy as np
 
 import gwcs
 
-__all__ = ['dataset_info_str']
+__all__ = ["dataset_info_str"]
 
 
 def dataset_info_str(ds):
     wcs = ds.wcs.low_level_wcs
 
     # Pixel dimensions table
 
@@ -26,110 +26,110 @@
 
     # Find largest between header size and value length
     if hasattr(wcs, "pixel_axis_names"):
         pixel_axis_names = wcs.pixel_axis_names
     elif isinstance(wcs, gwcs.WCS):
         pixel_axis_names = wcs.input_frame.axes_names
     else:
-        pixel_axis_names = [''] * wcs.pixel_n_dim
+        pixel_axis_names = [""] * wcs.pixel_n_dim
 
     pixel_dim_width = max(9, len(str(wcs.pixel_n_dim)))
     pixel_nam_width = max(9, max(len(x) for x in pixel_axis_names))
     pixel_siz_width = max(9, len(str(max(array_shape))))
 
-    s += (('{0:' + str(pixel_dim_width) + 's}').format('Pixel Dim') + '  ' +
-            ('{0:' + str(pixel_nam_width) + 's}').format('Axis Name') + '  ' +
-            ('{0:' + str(pixel_siz_width) + 's}').format('Data size') + '  ' +
-            'Bounds\n')
+    s += (("{0:" + str(pixel_dim_width) + "s}").format("Pixel Dim") + "  " +
+            ("{0:" + str(pixel_nam_width) + "s}").format("Axis Name") + "  " +
+            ("{0:" + str(pixel_siz_width) + "s}").format("Data size") + "  " +
+            "Bounds\n")
 
     for ipix in range(ds.wcs.pixel_n_dim):
-        s += (('{0:' + str(pixel_dim_width) + 'd}').format(ipix) + '  ' +
-                ('{0:' + str(pixel_nam_width) + 's}').format(pixel_axis_names[::-1][ipix] or 'None') + '  ' +
+        s += (("{0:" + str(pixel_dim_width) + "d}").format(ipix) + "  " +
+                ("{0:" + str(pixel_nam_width) + "s}").format(pixel_axis_names[::-1][ipix] or "None") + "  " +
                 (" " * 5 + str(None) if pixel_shape[::-1][ipix] is None else
-                ('{0:' + str(pixel_siz_width) + 'd}').format(pixel_shape[::-1][ipix])) + '  ' +
-                '{:s}'.format(str(None if wcs.pixel_bounds is None else wcs.pixel_bounds[::-1][ipix]) + '\n'))
-    s += '\n'
+                ("{0:" + str(pixel_siz_width) + "d}").format(pixel_shape[::-1][ipix])) + "  " +
+                "{:s}".format(str(None if wcs.pixel_bounds is None else wcs.pixel_bounds[::-1][ipix]) + "\n"))
+    s += "\n"
 
     # World dimensions table
 
     # Find largest between header size and value length
     world_dim_width = max(9, len(str(wcs.world_n_dim)))
     world_nam_width = max(9, max(len(x) if x is not None else 0 for x in wcs.world_axis_names))
     world_typ_width = max(13, max(len(x) if x is not None else 0 for x in wcs.world_axis_physical_types))
 
-    s += (('{0:' + str(world_dim_width) + 's}').format('World Dim') + '  ' +
-            ('{0:' + str(world_nam_width) + 's}').format('Axis Name') + '  ' +
-            ('{0:' + str(world_typ_width) + 's}').format('Physical Type') + '  ' +
-            'Units\n')
+    s += (("{0:" + str(world_dim_width) + "s}").format("World Dim") + "  " +
+            ("{0:" + str(world_nam_width) + "s}").format("Axis Name") + "  " +
+            ("{0:" + str(world_typ_width) + "s}").format("Physical Type") + "  " +
+            "Units\n")
 
     for iwrl in range(wcs.world_n_dim):
 
-        name = wcs.world_axis_names[::-1][iwrl] or 'None'
-        typ = wcs.world_axis_physical_types[::-1][iwrl] or 'None'
-        unit = wcs.world_axis_units[::-1][iwrl] or 'unknown'
-
-        s += (('{0:' + str(world_dim_width) + 'd}').format(iwrl) + '  ' +
-                ('{0:' + str(world_nam_width) + 's}').format(name) + '  ' +
-                ('{0:' + str(world_typ_width) + 's}').format(typ) + '  ' +
-                '{:s}'.format(unit + '\n'))
+        name = wcs.world_axis_names[::-1][iwrl] or "None"
+        typ = wcs.world_axis_physical_types[::-1][iwrl] or "None"
+        unit = wcs.world_axis_units[::-1][iwrl] or "unknown"
+
+        s += (("{0:" + str(world_dim_width) + "d}").format(iwrl) + "  " +
+                ("{0:" + str(world_nam_width) + "s}").format(name) + "  " +
+                ("{0:" + str(world_typ_width) + "s}").format(typ) + "  " +
+                "{:s}".format(unit + "\n"))
 
-    s += '\n'
+    s += "\n"
 
     # Axis correlation matrix
 
     pixel_dim_width = max(3, len(str(wcs.world_n_dim)))
 
-    s += 'Correlation between pixel and world axes:\n\n'
+    s += "Correlation between pixel and world axes:\n\n"
 
-    s += (' ' * world_dim_width + '  ' +
-            ('{0:^' + str(wcs.pixel_n_dim * 5 - 2) + 's}').format('Pixel Dim') +
-            '\n')
+    s += (" " * world_dim_width + "  " +
+            ("{0:^" + str(wcs.pixel_n_dim * 5 - 2) + "s}").format("Pixel Dim") +
+            "\n")
 
-    s += (('{0:' + str(world_dim_width) + 's}').format('World Dim') +
-            ''.join(['  ' + ('{0:' + str(pixel_dim_width) + 'd}').format(ipix)
+    s += (("{0:" + str(world_dim_width) + "s}").format("World Dim") +
+            "".join(["  " + ("{0:" + str(pixel_dim_width) + "d}").format(ipix)
                     for ipix in range(wcs.pixel_n_dim)]) +
-            '\n')
+            "\n")
 
     matrix = wcs.axis_correlation_matrix[::-1, ::-1]
-    matrix_str = np.empty(matrix.shape, dtype='U3')
-    matrix_str[matrix] = 'yes'
-    matrix_str[~matrix] = 'no'
+    matrix_str = np.empty(matrix.shape, dtype="U3")
+    matrix_str[matrix] = "yes"
+    matrix_str[~matrix] = "no"
 
     for iwrl in range(wcs.world_n_dim):
-        s += (('{0:' + str(world_dim_width) + 'd}').format(iwrl) +
-                ''.join(['  ' + ('{0:>' + str(pixel_dim_width) + 's}').format(matrix_str[iwrl, ipix])
+        s += (("{0:" + str(world_dim_width) + "d}").format(iwrl) +
+                "".join(["  " + ("{0:>" + str(pixel_dim_width) + "s}").format(matrix_str[iwrl, ipix])
                         for ipix in range(wcs.pixel_n_dim)]) +
-                '\n')
+                "\n")
 
     # Make sure we get rid of the extra whitespace at the end of some lines
-    return '\n'.join([l.rstrip() for l in s.splitlines()])
+    return "\n".join([line.rstrip() for line in s.splitlines()])
 
 
 def pp_matrix(wcs):
     """
     A small helper function to print a correlation matrix with labels
 
     Parameters
     ----------
     wcs : `BaseHighLevelWCS` or `BaseLowLevelWCS`
     """
-    slen = np.max([len(l) for l in list(wcs.world_axis_names) + list(wcs.pixel_axis_names)])
+    slen = np.max([len(line) for line in list(wcs.world_axis_names) + list(wcs.pixel_axis_names)])
     mstr = wcs.axis_correlation_matrix.astype(f"<U{slen}")
     mstr = np.insert(mstr, 0, wcs.pixel_axis_names, axis=0)
-    world = [''] + list(wcs.world_axis_names)
+    world = ["", *list(wcs.world_axis_names)]
     mstr = np.insert(mstr, 0, world, axis=1)
     for i, col in enumerate(mstr.T):
         wid = np.max([len(a) for a in col])
         mstr[:, i] = np.char.rjust(col, wid)
     print(np.array_str(mstr, max_line_width=1000))
 
 
 def extract_pc_matrix(headers, naxes=None):
     """
-    Given an astropy table of headers extract one or more PC matricies.
+    Given an astropy table of headers extract one or more PC matrices.
     """
     if naxes is None:
         naxes = headers[0]["NAXIS"]
     keys = []
     for i, j in np.ndindex((naxes, naxes)):
         keys.append(f"PC{i+1}_{j+1}")
```

### Comparing `dkist-1.4.0rc2/dkist/io/asdf/converters/dataset.py` & `dkist-1.5.0rc1/dkist/io/asdf/converters/dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/dkist/io/asdf/converters/file_manager.py` & `dkist-1.5.0rc1/dkist/io/asdf/converters/file_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,22 +20,21 @@
             raise ValueError("Currently only loading local asdf files is supported.")
         filepath = Path(url.path)
         if isinstance(filepath, PureWindowsPath):
             # If we are on windows we need to strip the leading /
             filepath = Path(url.path.strip("/"))
         base_path = filepath.parent
 
-        file_manager = FileManager.from_parts(node["fileuris"],
+        return FileManager.from_parts(node["fileuris"],
                                               node["target"],
                                               node["datatype"],
                                               node["shape"],
                                               chunksize=node.get("chunksize", None),
                                               loader=AstropyFITSLoader,
                                               basepath=base_path)
-        return file_manager
 
     def to_yaml_tree(self, obj, tag, ctx):
         node = {}
         node["fileuris"] = obj._striped_external_array.fileuri_array.tolist()
         node["target"] = obj._striped_external_array.target
         node["datatype"] = obj._striped_external_array.dtype
         node["shape"] = obj._striped_external_array.shape
```

### Comparing `dkist-1.4.0rc2/dkist/io/asdf/converters/models.py` & `dkist-1.5.0rc1/dkist/io/asdf/converters/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,36 +19,18 @@
         "dkist.wcs.models.VaryingCelestialTransform2D",
         "dkist.wcs.models.InverseVaryingCelestialTransform2D",
         "dkist.wcs.models.VaryingCelestialTransform3D",
         "dkist.wcs.models.InverseVaryingCelestialTransform3D",
     ]
 
     def select_tag(self, obj, tags, ctx):
-        from dkist.wcs.models import (InverseVaryingCelestialTransform,
-                                      InverseVaryingCelestialTransform2D,
-                                      InverseVaryingCelestialTransform3D,
-                                      VaryingCelestialTransform, VaryingCelestialTransform2D,
-                                      VaryingCelestialTransform3D)
-
-        if isinstance(
-                obj,
-                (VaryingCelestialTransform,
-                 VaryingCelestialTransform2D,
-                 VaryingCelestialTransform3D)
-        ):
-            return "asdf://dkist.nso.edu/tags/varying_celestial_transform-1.1.0"
-        elif isinstance(
-                obj,
-                (InverseVaryingCelestialTransform,
-                 InverseVaryingCelestialTransform2D,
-                 InverseVaryingCelestialTransform3D)
-        ):
+        if obj._is_inverse:
             return "asdf://dkist.nso.edu/tags/inverse_varying_celestial_transform-1.1.0"
-        else:
-            raise ValueError(f"Unsupported object: {obj}")  # pragma: no cover
+
+        return "asdf://dkist.nso.edu/tags/varying_celestial_transform-1.1.0"
 
     def from_yaml_tree_transform(self, node, tag, ctx):
         from dkist.wcs.models import varying_celestial_transform_from_tables
 
         inverse = False
         if "inverse_varying_celestial_transform" in tag:
             inverse = True
@@ -118,25 +100,24 @@
 
         from dkist.wcs.models import CoupledCompoundModel
 
         oper = "&"
 
         left = node["forward"][0]
         if not isinstance(left, Model):
-            raise TypeError("Unknown model type '{0}'".format(node["forward"][0]._tag))  # pragma: no cover
+            raise TypeError("Unknown model type '{}'".format(node["forward"][0]._tag))  # pragma: no cover
 
         right = node["forward"][1]
         if (not isinstance(right, Model) and
                 not (oper == "fix_inputs" and isinstance(right, dict))):
-            raise TypeError("Unknown model type '{0}'".format(node["forward"][1]._tag))  # pragma: no cover
+            raise TypeError("Unknown model type '{}'".format(node["forward"][1]._tag))  # pragma: no cover
 
-        model = CoupledCompoundModel(oper, left, right,
+        return CoupledCompoundModel(oper, left, right,
                                      shared_inputs=node["shared_inputs"])
 
-        return model
 
 
 class RavelConverter(TransformConverterBase):
     """
     ASDF serialization support for Ravel
     """
```

### Comparing `dkist-1.4.0rc2/dkist/io/asdf/converters/tiled_dataset.py` & `dkist-1.5.0rc1/dkist/io/asdf/converters/tiled_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/dkist/io/asdf/entry_points.py` & `dkist-1.5.0rc1/dkist/io/asdf/entry_points.py`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/dkist/io/asdf/resources/manifests/dkist-0.9.0.yaml` & `dkist-1.5.0rc1/dkist/io/asdf/resources/manifests/dkist-0.9.0.yaml`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/dkist/io/asdf/resources/manifests/dkist-1.0.0.yaml` & `dkist-1.5.0rc1/dkist/io/asdf/resources/manifests/dkist-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/dkist/io/asdf/resources/manifests/dkist-1.1.0.yaml` & `dkist-1.5.0rc1/dkist/io/asdf/resources/manifests/dkist-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/dkist/io/asdf/resources/manifests/dkist-1.2.0.yaml` & `dkist-1.5.0rc1/dkist/io/asdf/resources/manifests/dkist-1.2.0.yaml`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/dkist/io/asdf/resources/manifests/dkist-wcs-1.0.0.yaml` & `dkist-1.5.0rc1/dkist/io/asdf/resources/manifests/dkist-wcs-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/dkist/io/asdf/resources/manifests/dkist-wcs-1.1.0.yaml` & `dkist-1.5.0rc1/dkist/io/asdf/resources/manifests/dkist-wcs-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/dkist/io/asdf/resources/manifests/dkist-wcs-1.2.0.yaml` & `dkist-1.5.0rc1/dkist/io/asdf/resources/manifests/dkist-wcs-1.2.0.yaml`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/dkist/io/asdf/resources/schemas/asymmetric_mapping_model-1.0.0.yaml` & `dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/asymmetric_mapping_model-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/dkist/io/asdf/resources/schemas/coupled_compound_model-1.0.0.yaml` & `dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/coupled_compound_model-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/dkist/io/asdf/resources/schemas/dataset-0.1.0.yaml` & `dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/dataset-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/dkist/io/asdf/resources/schemas/dataset-0.2.0.yaml` & `dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/dataset-0.2.0.yaml`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/dkist/io/asdf/resources/schemas/dataset-0.3.0.yaml` & `dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/dataset-0.3.0.yaml`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/dkist/io/asdf/resources/schemas/dataset-1.0.0.yaml` & `dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/dataset-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/dkist/io/asdf/resources/schemas/dataset-1.1.0.yaml` & `dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/dataset-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/dkist/io/asdf/resources/schemas/file_manager-1.0.0.yaml` & `dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/file_manager-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/dkist/io/asdf/resources/schemas/ravel_model-1.0.0.yaml` & `dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/ravel_model-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/dkist/io/asdf/resources/schemas/tiled_dataset-0.1.0.yaml` & `dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/tiled_dataset-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/dkist/io/asdf/resources/schemas/tiled_dataset-1.0.0.yaml` & `dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/tiled_dataset-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/dkist/io/asdf/resources/schemas/varying_celestial_transform-1.0.0.yaml` & `dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/varying_celestial_transform-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/dkist/io/asdf/tests/conftest.py` & `dkist-1.5.0rc1/dkist/io/asdf/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/dkist/io/asdf/tests/test_dataset.py` & `dkist-1.5.0rc1/dkist/io/asdf/tests/test_dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import importlib.resources as importlib_resources
 from pathlib import Path
 
 import numpy as np
 import pytest
-from packaging.version import Version
 
 import asdf
 import astropy.table
 import gwcs
 from asdf.testing.helpers import roundtrip_object
 
 import dkist
@@ -22,15 +21,15 @@
     A fixture to lookup other fixtures.
     """
     return request.getfixturevalue(request.param)
 
 
 @pytest.fixture
 def file_manager():
-    return FileManager.from_parts(['test1.fits', 'test2.fits'], 0, 'float', (10, 10),
+    return FileManager.from_parts(["test1.fits", "test2.fits"], 0, "float", (10, 10),
                                   loader=AstropyFITSLoader)
 
 
 def test_roundtrip_file_manager(file_manager):
     newobj = roundtrip_object(file_manager)
     assert newobj == file_manager
 
@@ -69,24 +68,24 @@
 @pytest.mark.parametrize("tagobj",
                          [
                              "dataset",
                              "simple_tiled_dataset",
                          ],
                          indirect=True)
 def test_save_dataset_without_file_schema(tagobj, tmp_path):
-    tree = {'dataset': tagobj}
+    tree = {"dataset": tagobj}
     with asdf.AsdfFile(tree) as afile:
         afile.write_to(tmp_path / "test.asdf")
 
 
 def test_asdf_tags(dataset, tmp_path):
     """
     Test the tags and extensions used when saving a dataset.
     """
-    tree = {'dataset': dataset}
+    tree = {"dataset": dataset}
     with asdf.AsdfFile(tree) as afile:
         afile.write_to(tmp_path / "test.asdf")
 
     with asdf.open(tmp_path / "test.asdf", _force_raw_types=True) as af:
         assert af.tree["dataset"]._tag == "asdf://dkist.nso.edu/tags/dataset-1.2.0"
         assert af.tree["dataset"]["data"]._tag == "asdf://dkist.nso.edu/tags/file_manager-1.0.0"
 
@@ -97,26 +96,26 @@
 @pytest.mark.parametrize("tagobj",
                          [
                              "dataset",
                              "simple_tiled_dataset",
                          ],
                          indirect=True)
 def test_save_dataset_with_file_schema(tagobj, tmpdir):
-    tree = {'dataset': tagobj}
+    tree = {"dataset": tagobj}
     with importlib_resources.as_file(importlib_resources.files("dkist.io") / "level_1_dataset_schema.yaml") as schema_path:
         with asdf.AsdfFile(tree, custom_schema=schema_path.as_posix()) as afile:
             afile.write_to(Path(tmpdir / "test.asdf"))
 
 
 def test_read_all_schema_versions(eit_dataset_asdf_path):
     """
     This test validates that we can successfully read a full and valid Dataset
     object from files with all versions of the dataset schema.
     """
-    with importlib_resources.as_file(importlib_resources.files("dkist.io") / "level_1_dataset_schema.yaml") as schema_path:
+    with importlib_resources.as_file(importlib_resources.files("dkist.io") / "level_1_dataset_schema.yaml"):
         # Firstly verify that the tag versions in the test filename are the ones used in the file
         with asdf.open(eit_dataset_asdf_path, _force_raw_types=True) as afile:
             assert afile["dataset"]._tag.rsplit("/")[-1] in str(eit_dataset_asdf_path)
 
         with asdf.open(eit_dataset_asdf_path) as afile:
             dataset = afile["dataset"]
             dataset.files.basepath = rootdir / "EIT"
@@ -185,11 +184,12 @@
     wcs = dataset.wcs
     pixel_inputs = [0] * wcs.pixel_n_dim
     world_outputs = wcs.pixel_to_world_values(*pixel_inputs)
 
     # Assert that our stokes fixing code has worked.
     assert world_outputs[-1] == 1
 
-    if Version(gwcs.__version__) > Version("0.21.dev0"):
-        pixel_outputs = wcs.world_to_pixel_values(*world_outputs)
-
-        assert np.allclose(pixel_inputs, pixel_outputs, atol=1e-6)
+    # TODO: Requires https://github.com/spacetelescope/gwcs/pull/457
+    # if Version(gwcs.__version__) > Version("0.22.dev0"):
+    #     pixel_outputs = wcs.world_to_pixel_values(*world_outputs)
+    #
+    #     assert np.allclose(pixel_inputs, pixel_outputs, atol=1e-6)
```

### Comparing `dkist-1.4.0rc2/dkist/io/asdf/tests/test_models.py` & `dkist-1.5.0rc1/dkist/io/asdf/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/dkist/io/asdf/tests/test_tiled_dataset.py` & `dkist-1.5.0rc1/dkist/io/asdf/tests/test_tiled_dataset.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import importlib.resources as importlib_resources
 
 import asdf
 
 
 def test_verify_tiled_dataset_schema(tiled_dataset_asdf_path):
-    with importlib_resources.as_file(importlib_resources.files("dkist.io") / "level_1_dataset_schema.yaml") as schema_path:
+    with importlib_resources.as_file(importlib_resources.files("dkist.io") / "level_1_dataset_schema.yaml"):
 
         # Firstly verify that the tag versions in the test filename are the ones used in the file
         with asdf.open(tiled_dataset_asdf_path, _force_raw_types=True) as afile:
             assert afile["dataset"]._tag.rsplit("/")[-1] in str(tiled_dataset_asdf_path)
             assert afile["dataset"]["datasets"][0][0]._tag.rsplit("/")[-1] in str(tiled_dataset_asdf_path)
```

### Comparing `dkist-1.4.0rc2/dkist/io/dask_utils.py` & `dkist-1.5.0rc1/dkist/io/dask_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from functools import partial
 
 import dask.array as da
 import numpy as np
 
-__all__ = ['stack_loader_array']
+__all__ = ["stack_loader_array"]
 
 
 def stack_loader_array(loader_array, chunksize):
     """
     Stack a loader array along each of its dimensions.
 
     This results in a dask array with the correct chunks and dimensions.
@@ -16,27 +16,32 @@
     ----------
     loader_array : `dkist.io.reference_collections.BaseFITSArrayContainer`
 
     Returns
     -------
     array : `dask.array.Array`
     """
-    # If the chunksize sin't specified then use the whole array shape
+    # If the chunksize isn't specified then use the whole array shape
     chunksize = chunksize or loader_array.flat[0].shape
 
     if loader_array.size == 1:
         return tuple(loader_to_dask(loader_array, chunksize))[0]
     if len(loader_array.shape) == 1:
         return da.stack(loader_to_dask(loader_array, chunksize))
     stacks = []
     for i in range(loader_array.shape[0]):
         stacks.append(stack_loader_array(loader_array[i], chunksize))
     return da.stack(stacks)
 
 
+def _partial_to_array(loader, *, meta, chunks):
+    # Set the name of the array to the filename, that should be unique within the array
+    return da.from_array(loader, meta=meta, chunks=chunks, name=loader.fileuri)
+
+
 def loader_to_dask(loader_array, chunksize):
     """
     Map a call to `dask.array.from_array` onto all the elements in ``loader_array``.
 
     This is done so that an explicit ``meta=`` argument can be provided to
     prevent loading data from disk.
     """
@@ -46,10 +51,10 @@
     loader_array = np.atleast_1d(loader_array)
 
     # The meta argument to from array is used to determine properties of the
     # array, such as dtype. We explicitly specify it here to prevent dask
     # trying to auto calculate it by reading from the actual array on disk.
     meta = np.zeros((0,), dtype=loader_array[0].dtype)
 
-    to_array = partial(da.from_array, meta=meta, chunks=chunksize)
+    to_array = partial(_partial_to_array, meta=meta, chunks=chunksize)
 
     return map(to_array, loader_array)
```

### Comparing `dkist-1.4.0rc2/dkist/io/file_manager.py` & `dkist-1.5.0rc1/dkist/io/file_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,23 +11,24 @@
 * ``FileManager``: The object providing the public API, which can be sliced.
 
 The slicing functionality on the ``FileManager`` object works by constructing a
 view into the original ``StripedExternalArray`` object through the
 ``StripedExternalArrayView`` class.
 """
 import os
-from typing import Any, Tuple, Union, Iterable, Optional
+from typing import Any
 from pathlib import Path
+from collections.abc import Iterable
 
 import dask.array
 import numpy as np
 from parfive import Downloader
 
 try:
-    from numpy.typing import DTypeLike, NDArray  # NOQA
+    from numpy.typing import DTypeLike, NDArray
 except ImportError:
     NDArray = DTypeLike = Iterable
 
 from astropy.wcs.wcsapi.wrappers.sliced_wcs import sanitize_slices
 
 from dkist.io.dask_utils import stack_loader_array
 from dkist.io.loaders import BaseFITSLoader
@@ -47,26 +48,26 @@
         target = self.target == other.target
         dtype = self.dtype == other.dtype
         shape = self.shape == other.shape
 
         return all((uri, target, dtype, shape))
 
     @staticmethod
-    def _output_shape_from_ref_array(shape, loader_array) -> Tuple[int]:
+    def _output_shape_from_ref_array(shape, loader_array) -> tuple[int]:
         # If the first dimension is one we are going to squash it.
         if shape[0] == 1:
             shape = shape[1:]
 
         if loader_array.size == 1:
             return shape
-        else:
-            return tuple(list(loader_array.shape) + list(shape))
+
+        return tuple(list(loader_array.shape) + list(shape))
 
     @property
-    def output_shape(self) -> Tuple[int, ...]:
+    def output_shape(self) -> tuple[int, ...]:
         """
         The final shape of the reconstructed data array.
         """
         return self._output_shape_from_ref_array(self.shape, self.loader_array)
 
     def _generate_array(self) -> dask.array.Array:
         """
@@ -121,15 +122,15 @@
     def basepath(self) -> os.PathLike:
         """
         The path all arrays generated from this ``FileManager`` use to read data from.
         """
         return self._basepath
 
     @basepath.setter
-    def basepath(self, value: Optional[Union[os.PathLike, str]]):
+    def basepath(self, value: os.PathLike | str | None):
         self._basepath = Path(value).expanduser() if value is not None else None
 
     @property
     def fileuri_array(self) -> NDArray[str]:
         """
         An array of relative (to ``basepath``) file uris.
         """
@@ -149,15 +150,15 @@
 class StripedExternalArrayView(BaseStripedExternalArray):
     # This class presents a view int a FITSLoader object It applies a slice to
     # the fileuri_array and loader_array properties Any property which
     # references the sliced objects should be defined in Base or this view
     # class.
     __slots__ = ["parent", "parent_slice"]
 
-    def __init__(self, parent: StripedExternalArray, aslice: Union[tuple, slice, int]):
+    def __init__(self, parent: StripedExternalArray, aslice: tuple | slice | int):
         self.parent = parent
         self.parent_slice = tuple(aslice)
 
     def __getattr__(self, attr):
         return getattr(self.parent, attr)
 
     def __str__(self):
@@ -332,19 +333,19 @@
         overwrite: `bool`
             Set to `True` to overwrite file if it already exists. See
             `parfive.Downloader.simple_download` for details.
 
         Returns
         -------
         results: `parfive.Results`
-            A `~parfive.Results` obejct containing the filepath of the
+            A `~parfive.Results` object containing the filepath of the
             downloaded file if the download was successful, and any errors if it
             was not.
         """
-        dataset_id = self._ndcube.meta['inventory']['datasetId']
+        dataset_id = self._ndcube.meta["inventory"]["datasetId"]
         url = f"{self._metadata_streamer_url}/quality?datasetId={dataset_id}"
         if path is None and self.basepath:
             path = self.basepath
         return Downloader.simple_download([url], path=path, overwrite=overwrite)
 
     def preview_movie(self, path=None, overwrite=None):
         """
@@ -360,19 +361,19 @@
         overwrite: `bool`
             Set to `True` to overwrite file if it already exists. See
             `parfive.Downloader.simple_download` for details.
 
         Returns
         -------
         results: `parfive.Results`
-            A `~parfive.Results` obejct containing the filepath of the
+            A `~parfive.Results` object containing the filepath of the
             downloaded file if the download was successful, and any errors if it
             was not.
         """
-        dataset_id = self._ndcube.meta['inventory']['datasetId']
+        dataset_id = self._ndcube.meta["inventory"]["datasetId"]
         url = f"{self._metadata_streamer_url}/movie?datasetId={dataset_id}"
         if path is None and self.basepath:
             path = self.basepath
         return Downloader.simple_download([url], path=path, overwrite=overwrite)
 
     def download(self, path=None, destination_endpoint=None, progress=True, wait=True, label=None):
         """
```

### Comparing `dkist-1.4.0rc2/dkist/io/level_1_dataset_schema.yaml` & `dkist-1.5.0rc1/dkist/io/level_1_dataset_schema.yaml`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/dkist/io/loaders.py` & `dkist-1.5.0rc1/dkist/io/loaders.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,19 +5,20 @@
 
 import abc
 from pathlib import Path
 
 import numpy as np
 
 from astropy.io import fits
+
 from sunpy.util.decorators import add_common_docstring
 
 from dkist import log
 
-__all__ = ['BaseFITSLoader', 'AstropyFITSLoader']
+__all__ = ["BaseFITSLoader", "AstropyFITSLoader"]
 
 
 common_parameters = """
 
     Parameters
     ----------
     fileuri: `str`
@@ -53,15 +54,15 @@
         self.ndim = len(self.shape)
         self.size = np.prod(self.shape)
 
     def __repr__(self):
         return self.__str__()
 
     def __str__(self):
-        return "<FITS array in {0.fileuri} shape: {0.shape} dtype: {0.dtype}>".format(self)
+        return f"<FITS array in {self.fileuri} shape: {self.shape} dtype: {self.dtype}>"
 
     @property
     def data(self):
         return self[:]
 
     @abc.abstractmethod
     def __getitem__(self, slc):
@@ -74,16 +75,16 @@
     @property
     def absolute_uri(self):
         """
         Construct a non-relative path to the file, using ``basepath`` if provided.
         """
         if self.basepath:
             return self.basepath / self.fileuri
-        else:
-            return Path(self.fileuri)
+
+        return Path(self.fileuri)
 
 
 @add_common_docstring(append=common_parameters)
 class AstropyFITSLoader(BaseFITSLoader):
     """
     Resolve an `~asdf.ExternalArrayReference` to a FITS file using `astropy.io.fits`.
     """
@@ -100,9 +101,9 @@
                        do_not_scale_image_data=True,  # don't scale as we shouldn't need to
                        mode="denywrite") as hdul:
             log.debug("Accessing slice %s from file %s", slc, self.absolute_uri)
 
             hdu = hdul[self.target]
             if hasattr(hdu, "section"):
                 return hdu.section[slc]
-            else:
-                return hdu.data[slc]
+
+            return hdu.data[slc]
```

### Comparing `dkist-1.4.0rc2/dkist/io/tests/test_file_manager.py` & `dkist-1.5.0rc1/dkist/io/tests/test_file_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import pytest
 from numpy.testing import assert_allclose
 
 from dkist import net
 from dkist.data.test import rootdir
 from dkist.io.file_manager import FileManager, StripedExternalArray, StripedExternalArrayView
 
-eitdir = Path(rootdir) / 'EIT'
+eitdir = Path(rootdir) / "EIT"
 
 
 @pytest.fixture
 def file_manager(eit_dataset):
     """
     A file manager
     """
@@ -27,36 +27,36 @@
     """
     return file_manager._striped_external_array.loader_array
 
 
 def test_load_and_slicing(file_manager, loader_array):
     ext_shape = np.array(loader_array, dtype=object).shape
     assert file_manager._striped_external_array.loader_array.shape == ext_shape
-    assert file_manager.output_shape == tuple(list(ext_shape) + [128, 128])
+    assert file_manager.output_shape == (*list(ext_shape), 128, 128)
 
     array = file_manager._generate_array().compute()
     assert isinstance(array, np.ndarray)
     # Validate the data is actually loaded from the FITS
     assert not np.isnan(array).all()
 
     sliced_manager = file_manager[5:8]
     ext_shape = np.array(loader_array[5:8], dtype=object).shape
     assert sliced_manager._striped_external_array.loader_array.shape == ext_shape
-    assert sliced_manager.output_shape == tuple(list(ext_shape) + [128, 128])
+    assert sliced_manager.output_shape == (*list(ext_shape), 128, 128)
 
 
 def test_filenames(file_manager, loader_array):
     assert len(file_manager.filenames) == len(loader_array)
     assert (file_manager.filenames == file_manager._striped_external_array.fileuri_array.flatten()).all()
 
 
 def test_dask(file_manager, loader_array):
     ext_shape = np.array(loader_array, dtype=object).shape
     assert file_manager._striped_external_array.loader_array.shape == ext_shape
-    assert file_manager.output_shape == tuple(list(ext_shape) + [128, 128])
+    assert file_manager.output_shape == (*list(ext_shape), 128, 128)
 
     assert isinstance(file_manager._generate_array(), da.Array)
     assert_allclose(file_manager._generate_array(), np.array(file_manager._generate_array()))
 
 
 def test_collection_getitem(tmpdir, file_manager):
     assert isinstance(file_manager._striped_external_array, StripedExternalArray)
@@ -158,32 +158,30 @@
     assert str(len(sliced_sea)) in repr(sliced_sea)
     assert str(sliced_sea.shape) in repr(sliced_sea)
     assert str(sea) in repr(sliced_sea)
 
 
 @pytest.fixture
 def orchestrate_transfer_mock(mocker):
-    yield mocker.patch("dkist.net.helpers._orchestrate_transfer_task",
+    return mocker.patch("dkist.net.helpers._orchestrate_transfer_task",
                        autospec=True)
 
 
 def test_download_default_keywords(dataset, orchestrate_transfer_mock):
     base_path = Path(net.conf.dataset_path.format(**dataset.meta["inventory"]))
     folder = Path("/{bucket}/{primaryProposalId}/{datasetId}/".format(**dataset.meta["inventory"]))
-    file_list = dataset.files.filenames + [folder / "test_dataset.asdf",
-                                           folder / "test_dataset.mp4",
-                                           folder / "test_dataset.pdf"]
+    file_list = [*dataset.files.filenames, folder / "test_dataset.asdf", folder / "test_dataset.mp4", folder / "test_dataset.pdf"]
     file_list = [base_path / fn for fn in file_list]
 
     dataset.files.download()
 
     orchestrate_transfer_mock.assert_called_once_with(
         file_list,
         recursive=False,
-        destination_path=Path('/~'),
+        destination_path=Path("/~"),
         destination_endpoint=None,
         progress=True,
         wait=True,
         label=None,
     )
 
 
@@ -197,46 +195,42 @@
 def test_download_keywords(dataset, orchestrate_transfer_mock, keywords):
     """
     Assert that keywords are passed through as expected
     """
     base_path = Path(net.conf.dataset_path.format(**dataset.meta["inventory"]))
 
     folder = Path("/{bucket}/{primaryProposalId}/{datasetId}/".format(**dataset.meta["inventory"]))
-    file_list = dataset.files.filenames + [folder / "test_dataset.asdf",
-                                           folder / "test_dataset.mp4",
-                                           folder / "test_dataset.pdf"]
+    file_list = [*dataset.files.filenames, folder / "test_dataset.asdf", folder / "test_dataset.mp4", folder / "test_dataset.pdf"]
     file_list = [base_path / fn for fn in file_list]
 
     dataset.files.download(path="/test/", **keywords)
 
     orchestrate_transfer_mock.assert_called_once_with(
         file_list,
         recursive=False,
-        destination_path=Path('/test'),
+        destination_path=Path("/test"),
         **keywords
     )
 
     if not keywords["destination_endpoint"]:
         assert dataset.files.basepath == Path("/test/")
 
 
 def test_download_path_interpolation(dataset, orchestrate_transfer_mock):
     base_path = Path(net.conf.dataset_path.format(**dataset.meta["inventory"]))
     folder = Path("/{bucket}/{primaryProposalId}/{datasetId}/".format(**dataset.meta["inventory"]))
-    file_list = dataset.files.filenames + [folder / "test_dataset.asdf",
-                                           folder / "test_dataset.mp4",
-                                           folder / "test_dataset.pdf"]
+    file_list = [*dataset.files.filenames, folder / "test_dataset.asdf", folder / "test_dataset.mp4", folder / "test_dataset.pdf"]
     file_list = [base_path / fn for fn in file_list]
 
     dataset.files.download(path="~/{dataset_id}")
 
     orchestrate_transfer_mock.assert_called_once_with(
         file_list,
         recursive=False,
-        destination_path=Path('~/test_dataset/'),
+        destination_path=Path("~/test_dataset/"),
         destination_endpoint=None,
         progress=True,
         wait=True,
         label=None,
     )
 
     assert dataset.files.basepath == Path("~/test_dataset").expanduser()
@@ -250,18 +244,18 @@
     assert len(small_visp_dataset[0:2].files.filenames) == 2
 
     assert len(small_visp_dataset[0].files.filenames) == 1
 
     assert len(small_visp_dataset[:, 5, 5].files.filenames) == 3
 
 
-@pytest.mark.parametrize("kwargs", (
+@pytest.mark.parametrize("kwargs", [
     {},
     {"path": "~/", "overwrite": True}
-))
+])
 def test_download_quality(mocker, small_visp_dataset, kwargs):
     simple_download = mocker.patch("dkist.io.file_manager.Downloader.simple_download")
     from dkist.net import conf
 
     small_visp_dataset.files.quality_report(**kwargs)
 
     # Insert the expected default kwargs
@@ -272,18 +266,18 @@
 
     simple_download.assert_called_once_with(
         [f"{conf.download_endpoint}/quality?datasetId={small_visp_dataset.meta['inventory']['datasetId']}"],
         **kwargs
     )
 
 
-@pytest.mark.parametrize("kwargs", (
+@pytest.mark.parametrize("kwargs", [
     {},
     {"path": "~/", "overwrite": True}
-))
+])
 def test_download_quality_movie(mocker, small_visp_dataset, kwargs):
     simple_download = mocker.patch("dkist.io.file_manager.Downloader.simple_download")
     from dkist.net import conf
 
     small_visp_dataset.files.preview_movie(**kwargs)
 
     # Insert the expected default kwargs
```

### Comparing `dkist-1.4.0rc2/dkist/io/tests/test_fits.py` & `dkist-1.5.0rc1/dkist/io/tests/test_fits.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import asdf
 
 from dkist.data.test import rootdir
 from dkist.io.file_manager import FileManager
 from dkist.io.loaders import AstropyFITSLoader
 
-eitdir = Path(rootdir) / 'EIT'
+eitdir = Path(rootdir) / "EIT"
 
 
 @pytest.fixture
 def relative_ear():
     return asdf.ExternalArrayReference("efz20040301.000010_s.fits",
                                        0,
                                        "float64",
```

### Comparing `dkist-1.4.0rc2/dkist/logger.py` & `dkist-1.5.0rc1/dkist/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 This module contains helpers to use the Python logger to show messages to users.
 
-It is heavily insipired by Astropy's logger, but implemented independantly
+It is heavily insipired by Astropy's logger, but implemented independently
 because Astropy warn you against directly using theirs.
 
 This module sets up the following things:
 
 * A `logging.Logger` subclass which:
   - Tracks the module which triggered the log call.
   - Overrides warnings.showwarnings so that subclasses of given warning classes are displayed using the logger.
@@ -26,15 +26,15 @@
     """
     A knock off AstropyLogger.
     """
     _showwarning_orig = None
 
     def __init__(self, name, level=logging.NOTSET, *, capture_warning_classes=None):
         super().__init__(name, level=level)
-        self.capture_warning_classes = tuple(capture_warning_classes) if capture_warning_classes is not None else tuple()
+        self.capture_warning_classes = tuple(capture_warning_classes) if capture_warning_classes is not None else ()
 
         self.enable_warnings_capture()
 
     def enable_warnings_capture(self):
         if self._showwarning_orig is None:
             self._showwarning_orig = warnings.showwarning
             warnings.showwarning = self._showwarning
```

### Comparing `dkist-1.4.0rc2/dkist/net/__init__.py` & `dkist-1.5.0rc1/dkist/net/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,10 +26,10 @@
 
     attr_max_age = _config.ConfigItem(7,
                                       "The number of days beyond which to refresh search attr values from the Data Center")
 
 
 conf = Conf()
 
-# Put imports after conf so that conf is initalized before import
-from .client import DKISTClient  # noqa
-from .helpers import transfer_complete_datasets  # noqa
+# Put imports after conf so that conf is initialized before import
+from .client import DKISTClient
+from .helpers import transfer_complete_datasets
```

### Comparing `dkist-1.4.0rc2/dkist/net/attr_walker.py` & `dkist-1.5.0rc1/dkist/net/attr_walker.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import astropy.units as u
+
 from sunpy.net.attr import AttrAnd, AttrOr, AttrWalker, DataAttr
 from sunpy.net.attrs import Instrument, Level, Physobs, Provider, Time, Wavelength
 
 from .attrs import *
 
 walker = AttrWalker()
 """
@@ -31,15 +32,15 @@
         params.append(sub_params)
 
     return params
 
 
 @walker.add_creator(AttrAnd, DataAttr)
 def create_new_param(wlk, tree):
-    params = dict()
+    params = {}
 
     # Use the apply dispatcher to convert the attrs to their query parameters
     wlk.apply(tree, params)
 
     return [params]
 
 
@@ -49,151 +50,151 @@
         wlk.apply(sub, params)
 
 
 # Converters from Attrs to ValueAttrs
 # SunPy Attrs
 @walker.add_applier(Time)
 def _(wlk, attr, params):
-    return params.update({'endTimeMin': attr.start.isot,
-                          'startTimeMax': attr.end.isot})
+    return params.update({"endTimeMin": attr.start.isot,
+                          "startTimeMax": attr.end.isot})
 
 
 @walker.add_applier(Instrument)
 def _(wlk, attr, params):
-    return params.update({'instrumentNames': attr.value})
+    return params.update({"instrumentNames": attr.value})
 
 
 @walker.add_applier(Wavelength)
 def _(wlk, attr, params):
-    return params.update({'wavelengthRanges': [attr.min.to_value(u.nm), attr.max.to_value(u.nm)]})
+    return params.update({"wavelengthRanges": [attr.min.to_value(u.nm), attr.max.to_value(u.nm)]})
 
 
 @walker.add_applier(Physobs)
 def _(wlk, attr, params):
     if attr.value.lower() == "stokes_parameters":
-        return params.update({'hasAllStokes': True})
+        return params.update({"hasAllStokes": True})
     if attr.value.lower() == "intensity":
-        return params.update({'hasAllStokes': False})
+        return params.update({"hasAllStokes": False})
     if attr.value.lower() == "spectral_axis":
-        return params.update({'hasSpectralAxis': True})
+        return params.update({"hasSpectralAxis": True})
     if attr.value.lower() == "temporal_axis":
-        return params.update({'hasTemporalAxis': True})
+        return params.update({"hasTemporalAxis": True})
 
     # The client should not have accepted the query if we make it this far.
     raise ValueError(f"Physobs({attr.value}) is not supported by the DKIST client.")  # pragma: no cover
 
 
 # DKIST Attrs
 @walker.add_applier(PageSize)
 def _(wlk, attr, params):
-    return params.update({'pageSize': attr.value})
+    return params.update({"pageSize": attr.value})
 
 
 @walker.add_applier(Page)
 def _(wlk, attr, params):
-    return params.update({'pageNumber': attr.value})
+    return params.update({"pageNumber": attr.value})
 
 
 @walker.add_applier(Dataset)
 def _(wlk, attr, params):
-    return params.update({'datasetIds': attr.value})
+    return params.update({"datasetIds": attr.value})
 
 
 @walker.add_applier(WavelengthBand)
 def _(wlk, attr, params):
-    return params.update({'filterWavelengths': attr.value})
+    return params.update({"filterWavelengths": attr.value})
 
 
 @walker.add_applier(Observable)
 def _(wlk, attr, params):
-    return params.update({'observables': attr.value})
+    return params.update({"observables": attr.value})
 
 
 @walker.add_applier(Experiment)
 def _(wlk, attr, params):
-    return params.update({'primaryExperimentIds': attr.value})
+    return params.update({"primaryExperimentIds": attr.value})
 
 
 @walker.add_applier(Proposal)
 def _(wlk, attr, params):
-    return params.update({'primaryProposalIds': attr.value})
+    return params.update({"primaryProposalIds": attr.value})
 
 
 @walker.add_applier(TargetType)
 def _(wlk, attr, params):
-    return params.update({'targetTypes': attr.value})
+    return params.update({"targetTypes": attr.value})
 
 
 @walker.add_applier(Recipe)
 def _(wlk, attr, params):
-    return params.update({'recipeId': attr.value})
+    return params.update({"recipeId": attr.value})
 
 
 @walker.add_applier(Embargoed)
 def _(wlk, attr, params):
-    return params.update({'isEmbargoed': bool(attr.value)})
+    return params.update({"isEmbargoed": bool(attr.value)})
 
 
 @walker.add_applier(FriedParameter)
 def _(wlk, attr, params):
-    return params.update({'qualityAverageFriedParameterMin': attr.min.to_value(u.cm),
-                          'qualityAverageFriedParameterMax': attr.max.to_value(u.cm)})
+    return params.update({"qualityAverageFriedParameterMin": attr.min.to_value(u.cm),
+                          "qualityAverageFriedParameterMax": attr.max.to_value(u.cm)})
 
 
 @walker.add_applier(PolarimetricAccuracy)
 def _(wlk, attr, params):
-    return params.update({'qualityAveragePolarimetricAccuracyMin': attr.min,
-                          'qualityAveragePolarimetricAccuracyMax': attr.max})
+    return params.update({"qualityAveragePolarimetricAccuracyMin": attr.min,
+                          "qualityAveragePolarimetricAccuracyMax": attr.max})
 
 
 @walker.add_applier(ExposureTime)
 def _(wlk, attr, params):
-    return params.update({'exposureTimeMin': attr.min.to_value(u.s),
-                          'exposureTimeMax': attr.max.to_value(u.s)})
+    return params.update({"exposureTimeMin": attr.min.to_value(u.s),
+                          "exposureTimeMax": attr.max.to_value(u.s)})
 
 
 @walker.add_applier(EmbargoEndTime)
 def _(wlk, attr, params):
-    return params.update({'embargoEndDateMin': attr.start.isot,
-                          'embargoEndDateMax': attr.end.isot})
+    return params.update({"embargoEndDateMin": attr.start.isot,
+                          "embargoEndDateMax": attr.end.isot})
 
 @walker.add_applier(SpectralSampling)
 def _(wlk, attr, params):
-    return params.update({'averageDatasetSpectralSamplingMin': attr.min.to_value(equivalencies=float),
-                          'averageDatasetSpectralSamplingMax': attr.max.to_value(equivalencies=float)})
+    return params.update({"averageDatasetSpectralSamplingMin": attr.min.to_value(equivalencies=float),
+                          "averageDatasetSpectralSamplingMax": attr.max.to_value(equivalencies=float)})
 
 @walker.add_applier(SpatialSampling)
 def _(wlk, attr, params):
-    return params.update({'averageDatasetSpatialSamplingMin': attr.min.to_value(equivalencies=float),
-                          'averageDatasetSpatialSamplingMax': attr.max.to_value(equivalencies=float)})
+    return params.update({"averageDatasetSpatialSamplingMin": attr.min.to_value(equivalencies=float),
+                          "averageDatasetSpatialSamplingMax": attr.max.to_value(equivalencies=float)})
 
 @walker.add_applier(TemporalSampling)
 def _(wlk, attr, params):
-    return params.update({'averageDatasetTemporalSamplingMin': attr.min.to_value(u.s),
-                          'averageDatasetTemporalSamplingMax': attr.max.to_value(u.s)})
+    return params.update({"averageDatasetTemporalSamplingMin": attr.min.to_value(u.s),
+                          "averageDatasetTemporalSamplingMax": attr.max.to_value(u.s)})
 
 @walker.add_applier(BrowseMovie)
 def _(wlk, attr, params):
     values = {}
     if attr.movieurl:
-        values['browseMovieUrl'] = attr.movieurl
+        values["browseMovieUrl"] = attr.movieurl
     if attr.movieobjectkey:
-        values['browseMovieObjectKey'] = attr.movieobjectkey
+        values["browseMovieObjectKey"] = attr.movieobjectkey
 
     return params.update(values)
 
 
 @walker.add_applier(BoundingBox)
 def _(wlk, attr, params):
     search_types = {"containing": "rectangleContainingBoundingBox",
                     "contained": "rectangleContainedByBoundingBox",
                     "intersecting": "rectangleIntersectingBoundingBox"}
 
     # strip all spaces and the outer most ()
-    return params.update({search_types[attr.search_type]: str(attr.hpc_bounding_box_arcsec).replace(' ', '')[1:-1]})
+    return params.update({search_types[attr.search_type]: str(attr.hpc_bounding_box_arcsec).replace(" ", "")[1:-1]})
 
 
 @walker.add_applier(Provider)
 def _(wlk, attr, params):
     """
     Provider is used by client _can_handle_query and not the API.
     """
@@ -204,33 +205,33 @@
     """
     Level is used by client _can_handle_query and not the API.
     """
 
 
 @walker.add_applier(SummitSoftwareVersion)
 def _(wlk, attr, params):
-    return params.update({'highLevelSoftwareVersion': attr.value})
+    return params.update({"highLevelSoftwareVersion": attr.value})
 
 
 @walker.add_applier(WorkflowName)
 def _(wlk, attr, params):
-    return params.update({'workflowName': attr.value})
+    return params.update({"workflowName": attr.value})
 
 
 @walker.add_applier(WorkflowVersion)
 def _(wlk, attr, params):
-    return params.update({'workflowVersion': attr.value})
+    return params.update({"workflowVersion": attr.value})
 
 
 @walker.add_applier(ObservingProgramExecutionID)
 def _(wlk, attr, params):
-    return params.update({'observingProgramExecutionId': attr.value})
+    return params.update({"observingProgramExecutionId": attr.value})
 
 
 @walker.add_applier(InstrumentProgramExecutionID)
 def _(wlk, attr, params):
-    return params.update({'instrumentProgramExecutionId': attr.value})
+    return params.update({"instrumentProgramExecutionId": attr.value})
 
 
 @walker.add_applier(HeaderVersion)
 def _(wlk, attr, params):
-    return params.update({'headerVersion': attr.value})
+    return params.update({"headerVersion": attr.value})
```

### Comparing `dkist-1.4.0rc2/dkist/net/attrs.py` & `dkist-1.5.0rc1/dkist/net/attrs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 """
 Search attributes which are specific to the `dkist.net.DKISTClient`.
 
 Other attributes provided by `sunpy.net.attrs` are supported by the client.
 """
-import astropy.units as _u
+import astropy.units as _u  # noqa: ICN001
+
 import sunpy.net._attrs as _sunpy_attrs
 from sunpy.coordinates.frames import Helioprojective as _Helioprojective
 from sunpy.coordinates.utils import get_rectangle_coordinates as _get_rectangle_coordinates
 from sunpy.net.attr import DataAttr as _DataAttr
 from sunpy.net.attr import Range as _Range
 from sunpy.net.attr import SimpleAttr as _SimpleAttr
 
-__all__ = ['PageSize', 'Page', 'Dataset', 'WavelengthBand', 'Embargoed', 'Observable',
-           'Experiment', 'Proposal', 'TargetType', 'Recipe',
-           'FriedParameter', 'PolarimetricAccuracy', 'ExposureTime',
-           'EmbargoEndTime', 'BrowseMovie', 'BoundingBox',
-           'SpectralSampling', 'SpatialSampling', 'TemporalSampling', 'SummitSoftwareVersion',
-           'WorkflowName', 'WorkflowVersion', 'ObservingProgramExecutionID',
-           'InstrumentProgramExecutionID', 'HeaderVersion']
+__all__ = ["PageSize", "Page", "Dataset", "WavelengthBand", "Embargoed", "Observable",
+           "Experiment", "Proposal", "TargetType", "Recipe",
+           "FriedParameter", "PolarimetricAccuracy", "ExposureTime",
+           "EmbargoEndTime", "BrowseMovie", "BoundingBox",
+           "SpectralSampling", "SpatialSampling", "TemporalSampling", "SummitSoftwareVersion",
+           "WorkflowName", "WorkflowVersion", "ObservingProgramExecutionID",
+           "InstrumentProgramExecutionID", "HeaderVersion"]
 
 
 # SimpleAttrs
 
 class PageSize(_SimpleAttr):
     """
     The number of search results to return.
```

### Comparing `dkist-1.4.0rc2/dkist/net/attrs_values.py` & `dkist-1.5.0rc1/dkist/net/attrs_values.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import urllib
 import datetime as dt
 import importlib.resources
 from pathlib import Path
 
 import platformdirs
 
-from sunpy.net import attrs as sattrs
+from sunpy.net import attrs as sattrs  # noqa: ICN001
 
 import dkist.data
 from dkist import log
 from dkist.net import attrs as dattrs
 from dkist.net import conf as net_conf
 
 __all__ = ["attempt_local_update", "get_search_attrs_values"]
@@ -104,25 +104,25 @@
     success = False
     try:
         _fetch_values_to_file(user_file, timeout=timeout)
         success = True
     except Exception as err:
         log.error("Failed to download new attrs values.")
         log.debug(str(err))
-        # If an error has occured then remove the local file so it isn't
+        # If an error has occurred then remove the local file so it isn't
         # corrupted or invalid.
         user_file.unlink(missing_ok=True)
         if not silence_errors:
             raise
 
         return success
 
     # Test that the file we just saved can be parsed as json
     try:
-        with open(user_file, "r") as f:
+        with open(user_file) as f:
             json.load(f)
     except Exception:
         log.error("Downloaded file is not valid JSON.")
         user_file.unlink(missing_ok=True)
         if not silence_errors:
             raise
         success = False
@@ -154,15 +154,15 @@
     if allow_update and update_needed:
         attempt_local_update(timeout=timeout)
 
     if not update_needed:
         log.debug("No update to attr values needed.")
         log.debug("Using attr values from %s", local_path)
 
-    with open(local_path, "r") as f:
+    with open(local_path) as f:
         search_values = json.load(f)
 
     search_values = {param["parameterName"]: param["values"] for param in search_values["parameterValues"]}
 
     attr_values = {}
     for key, attr in INVENTORY_ATTR_MAP["categorical"].items():
         attr_values[attr] = [(name, "") for name in search_values[key]["categoricalValues"]]
```

### Comparing `dkist-1.4.0rc2/dkist/net/client.py` & `dkist-1.5.0rc1/dkist/net/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 import os
 import json
 import urllib.parse
 import urllib.request
-from typing import Any, List, Mapping, Iterable
+from typing import Any
 from textwrap import dedent
 from functools import partial
 from collections import defaultdict
+from collections.abc import Mapping, Iterable
 
 import aiohttp
 import numpy as np
 import parfive
 
 import astropy.units as u
 from astropy.table import TableAttribute
 from astropy.time import Time
+
 from sunpy.net import attr
-from sunpy.net import attrs as sattrs
+from sunpy.net import attrs as sattrs  # noqa: ICN001
 from sunpy.net.base_client import (BaseClient, QueryResponseRow,
                                    QueryResponseTable, convert_row_to_table)
 from sunpy.util.net import parse_header
 
 from dkist.net.attrs_values import get_search_attrs_values
 from dkist.utils.inventory import INVENTORY_KEY_MAP
 
@@ -33,15 +35,15 @@
     """
     Results of a DKIST Dataset search.
     """
 
     # Define some class properties to better format the results table.
     # TODO: remove experimentDescription from this list, when we can limit the
     # length of the field to something nicer
-    hide_keys: List[str] = [
+    hide_keys: list[str] = [
         "Storage Bucket",
         "Full Stokes",
         "asdf Filename",
         "Recipe Instance ID",
         "Recipe Run ID",
         "Recipe ID",
         "Movie Filename",
@@ -80,21 +82,21 @@
                  "Wavelength Max": u.nm, "Dataset Size": u.Gibyte,
                  "Filter Wavelengths": u.nm, "Average Spectral Sampling": u.nm,
                  "Average Spatial Sampling": u.arcsec, "Average Temporal Sampling": u.s}
 
         for colname in times:
             if colname not in results.colnames:
                 continue  # pragma: no cover
-            if not any([v is None for v in results[colname]]):
+            if not any(v is None for v in results[colname]):
                 results[colname] = Time(results[colname])
 
         for colname, unit in units.items():
             if colname not in results.colnames:
                 continue  # pragma: no cover
-            none_values = np.array(results[colname] == None)
+            none_values = np.array(results[colname] == None)  # E711
             if none_values.any():
                 results[colname][none_values] = np.nan
             results[colname] = u.Quantity(results[colname], unit=unit)
 
         if results and "Wavelength" not in results.colnames:
             results["Wavelength"] = u.Quantity([results["Wavelength Min"], results["Wavelength Max"]]).T
             results.remove_columns(("Wavelength Min", "Wavelength Max"))
@@ -105,15 +107,15 @@
     def from_results(cls, responses: Iterable[Mapping[str, Any]], *, client: "DKISTClient") -> "DKISTQueryResponseTable":
         """
         Construct the results table from the API results.
         """
         total_available_results = 0
         new_results = defaultdict(list)
         for response in responses:
-            total_available_results += response.get('recordCount', 0)
+            total_available_results += response.get("recordCount", 0)
             for result in response["searchResults"]:
                 for key, value in result.items():
                     new_results[INVENTORY_KEY_MAP[key]].append(value)
 
         data = cls._process_table(cls(new_results, client=client))
         data = data._reorder_columns(cls._core_keys.default, remove_empty=True)
         data.total_available_results = total_available_results
@@ -171,16 +173,16 @@
         from dkist.net import conf
 
         query = attr.and_(*args)
         queries = walker.create(query)
 
         results = []
         for url_parameters in queries:
-            if 'pageSize' not in url_parameters:
-                url_parameters.update({'pageSize': conf.default_page_size})
+            if "pageSize" not in url_parameters:
+                url_parameters.update({"pageSize": conf.default_page_size})
             # TODO make this accept and concatenate multiple wavebands in a search
             query_string = urllib.parse.urlencode(url_parameters, doseq=True)
             full_url = f"{self._dataset_search_url}?{query_string}"
             data = urllib.request.urlopen(full_url)
             data = json.loads(data.read())
             results.append(data)
 
@@ -196,15 +198,15 @@
         # The fallback name is just the dataset id.
         name = f"{row['Dataset ID']}.asdf"
 
         if resp:
             cdheader = resp.headers.get("Content-Disposition", None)
             if cdheader:
                 _, params = parse_header(cdheader)
-                name = params.get('filename', "")
+                name = params.get("filename", "")
 
         return str(path).format(file=name, **row.response_block_map)
 
     @convert_row_to_table
     def fetch(self, query_results: QueryResponseTable, *,
               path: os.PathLike = None,
               downloader: parfive.Downloader, **kwargs):
@@ -232,15 +234,15 @@
         # This enables the client to register what kind of searches it can
         # handle, to prevent Fido using the incorrect client.
         from sunpy.net import attrs as a
 
         supported = set(walker.applymm.registry)
         # This function is only called with arguments of the query where they are assumed to be ANDed.
         supported.remove(attr.AttrAnd)
-        query_attrs = set(type(x) for x in query)
+        query_attrs = {type(x) for x in query}
 
         # The DKIST client only requires that one or more of the support attrs be present.
         if not query_attrs.issubset(supported) or len(query_attrs.intersection(supported)) < 1:
             return False
 
         for x in query:
             if isinstance(x, a.Instrument):
@@ -256,15 +258,15 @@
                 if x.value not in (1, "1", "one"):
                     return False
 
         return True
 
     @classmethod
     def _attrs_module(cls):
-        return 'dkist', 'dkist.net.attrs'
+        return "dkist", "dkist.net.attrs"
 
     @classmethod
     def register_values(cls):
         """
         Known search values for DKIST data, currently manually specified.
         """
         return_values = {
```

### Comparing `dkist-1.4.0rc2/dkist/net/globus/auth.py` & `dkist-1.5.0rc1/dkist/net/globus/auth.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,20 +13,20 @@
 from pathlib import Path
 from http.server import HTTPServer, BaseHTTPRequestHandler
 from urllib.parse import parse_qs, urlparse
 
 import globus_sdk
 import platformdirs
 
-CLIENT_ID = 'dd2d62af-0b44-4e2e-9454-1092c94b46b3'
-SCOPES = ('urn:globus:auth:scope:transfer.api.globus.org:all',
-          'openid')
+CLIENT_ID = "dd2d62af-0b44-4e2e-9454-1092c94b46b3"
+SCOPES = ("urn:globus:auth:scope:transfer.api.globus.org:all",
+          "openid")
 
 
-__all__ = ['ensure_globus_authorized', 'get_refresh_token_authorizer']
+__all__ = ["ensure_globus_authorized", "get_refresh_token_authorizer"]
 
 
 class AuthenticationError(Exception):
     """
     An error to be raised if authentication fails.
     """
 
@@ -43,26 +43,26 @@
     def wait_for_code(self):
         return self._auth_code_queue.get(block=True)
 
 
 class RedirectHandler(BaseHTTPRequestHandler):
     def do_GET(self):
         self.send_response(200)
-        self.send_header('Content-type', 'text/html')
+        self.send_header("Content-type", "text/html")
         self.end_headers()
-        self.wfile.write(b'You\'re all set, you can close this window!')
+        self.wfile.write(b"You're all set, you can close this window!")
 
-        code = parse_qs(urlparse(self.path).query).get('code', [''])[0]
+        code = parse_qs(urlparse(self.path).query).get("code", [""])[0]
         self.server.return_code(code)
 
     def log_message(self, format, *args):
         return
 
 
-def start_local_server(listen=('localhost', 0)):
+def start_local_server(listen=("localhost", 0)):
     """
     Start a server which will listen for the OAuth2 callback.
 
     Parameters
     ----------
     listen: `tuple`, optional
         ``(address, port)`` tuple, defaults to localhost and port 0, which
@@ -87,20 +87,20 @@
 def get_cache_contents():
     """
     Read the cache file, return an empty dict if not found or invalid.
     """
     cache_file = get_cache_file_path()
     if not cache_file.exists():
         return {}
-    else:
-        try:
-            with open(cache_file) as fd:
-                return json.load(fd)
-        except (IOError, json.JSONDecodeError):
-            return {}
+
+    try:
+        with open(cache_file) as fd:
+            return json.load(fd)
+    except (OSError, json.JSONDecodeError):
+        return {}
 
 
 def save_auth_cache(auth_cache):
     """
     Write the auth cache to the cache file.
 
     Parameters
@@ -129,23 +129,23 @@
 
 def do_native_app_authentication(client_id, requested_scopes=None):  # pragma: no cover
     """
     Does a Native App authentication flow and returns a
     dict of tokens keyed by service name.
     """
     server = start_local_server()
-    redirect_uri = "http://{a[0]}:{a[1]}".format(a=server.server_address)
+    redirect_uri = f"http://{server.server_address[0]}:{server.server_address[1]}"
 
     client = globus_sdk.NativeAppAuthClient(client_id=client_id)
     client.oauth2_start_flow(requested_scopes=SCOPES,
                              redirect_uri=redirect_uri,
                              refresh_tokens=True)
     url = client.oauth2_get_authorize_url()
 
-    result = webbrowser.open(url, new=1)
+    webbrowser.open(url, new=1)
     print("Waiting for completion of Globus Authentication in your webbrowser...")
     print(f"If your webbrowser has not opened, please go to {url} to authenticate with globus.")
 
     try:
         auth_code = server.wait_for_code()
     except KeyboardInterrupt:
         raise AuthenticationError("Failed to authenticate with Globus.")
@@ -178,23 +178,23 @@
         tokens = get_cache_contents()
     if not tokens:
         tokens = do_native_app_authentication(CLIENT_ID, SCOPES)
         save_auth_cache(tokens)
 
     auth_client = globus_sdk.NativeAppAuthClient(client_id=CLIENT_ID)
 
-    transfer_tokens = tokens['transfer.api.globus.org']
+    transfer_tokens = tokens["transfer.api.globus.org"]
 
     authorizers = {}
     for scope, transfer_tokens in tokens.items():
         authorizers[scope] = globus_sdk.RefreshTokenAuthorizer(
-            transfer_tokens['refresh_token'],
+            transfer_tokens["refresh_token"],
             auth_client,
-            access_token=transfer_tokens['access_token'],
-            expires_at=transfer_tokens['expires_at_seconds'],
+            access_token=transfer_tokens["access_token"],
+            expires_at=transfer_tokens["expires_at_seconds"],
             on_refresh=save_auth_cache)
 
     return authorizers
 
 
 def ensure_globus_authorized(func):
     """
```

### Comparing `dkist-1.4.0rc2/dkist/net/globus/endpoints.py` & `dkist-1.5.0rc1/dkist/net/globus/endpoints.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """
 Functions for interacting with globus endpoints.
 """
 import json
 import urllib
 import pathlib
 import webbrowser
-from functools import lru_cache
+from functools import cache
 
 import globus_sdk
 
 from .auth import ensure_globus_authorized, get_refresh_token_authorizer
 
-__all__ = ['get_data_center_endpoint_id', 'get_endpoint_id', 'get_directory_listing']
+__all__ = ["get_data_center_endpoint_id", "get_endpoint_id", "get_directory_listing"]
 
 
 def get_transfer_client(force_reauth=False):
     """
     Get an authorized transfer client.
 
     Parameters
@@ -23,15 +23,15 @@
     force_reauth : `bool`, optional
         Do not use cached authentication details when `True`.
 
     Returns
     -------
     `globus_sdk.TransferClient`
     """
-    auth = get_refresh_token_authorizer(force_reauth)['transfer.api.globus.org']
+    auth = get_refresh_token_authorizer(force_reauth)["transfer.api.globus.org"]
     return globus_sdk.TransferClient(authorizer=auth)
 
 
 def get_local_endpoint_id():
     """
     Get the endpoint ID of a local Globus Connect Personal endpoint.
 
@@ -51,15 +51,15 @@
 
     if not endpoint_id:
         raise ConnectionError("Can not find a local Globus Connect endpoint.")
 
     return endpoint_id
 
 
-@lru_cache(maxsize=None)
+@cache
 def get_data_center_endpoint_id():
     """
     Query the data center for the current globus endpoint ID.
 
     The endpoint ID is retrieved from the configured dataset searcher endpoint.
     """
     from dkist.net import conf
@@ -89,38 +89,38 @@
     tfr_client : `globus_sdk.TransferClient`
         The transfer client to use to query the endpoint.
 
     """
     tr = None
 
     # If there is a space in the endpoint it's not an id
-    if ' ' not in endpoint:
+    if " " not in endpoint:
         try:
             tr = tfr_client.get_endpoint(endpoint)
             return endpoint
         except globus_sdk.TransferAPIError as e:
             if e.code != "EndpointNotFound":
                 raise
 
     if not tr:
         tr = tfr_client.endpoint_search(endpoint)
 
     responses = tr.data["DATA"]
 
+    if len(responses) == 0:
+        raise ValueError(f"No matches found for endpoint '{endpoint}'")
+
     if len(responses) > 1:
-        display_names = [a['display_name'] for a in responses]
+        display_names = [a["display_name"] for a in responses]
         # If we have one and only one exact display name match use that
         if display_names.count(endpoint) == 1:
-            return responses[display_names.index(endpoint)]['id']
+            return responses[display_names.index(endpoint)]["id"]
         raise ValueError(f"Multiple matches for endpoint '{endpoint}': {display_names}")
 
-    elif len(responses) == 0:
-        raise ValueError(f"No matches found for endpoint '{endpoint}'")
-
-    return responses[0]['id']
+    return responses[0]["id"]
 
 
 @ensure_globus_authorized
 def auto_activate_endpoint(endpoint_id, tfr_client):  # pragma: no cover
     """
     Perform activation of a Globus endpoint.
 
@@ -130,19 +130,19 @@
         The uuid of the endpoint to activate.
 
     tfr_client : `globus_sdk.TransferClient`
         The transfer client to use for the activation.
 
     """
     activation = tfr_client.endpoint_get_activation_requirements(endpoint_id)
-    needs_activation = bool(activation['DATA'])
-    activated = activation['activated']
+    needs_activation = bool(activation["DATA"])
+    activated = activation["activated"]
     if needs_activation and not activated:
         r = tfr_client.endpoint_autoactivate(endpoint_id)
-        if r['code'] == "AutoActivationFailed":
+        if r["code"] == "AutoActivationFailed":
             webbrowser.open(f"https://app.globus.org/file-manager?origin_id={endpoint_id}",
                             new=1)
             input("Press Return after completing activation in your webbrowser...")
             r = tfr_client.endpoint_autoactivate(endpoint_id)
 
 
 @ensure_globus_authorized
@@ -176,10 +176,10 @@
     tc = get_transfer_client()
 
     if endpoint_id is None:
         endpoint_id = get_endpoint_id(endpoint, tc)
         auto_activate_endpoint(endpoint_id, tc)
 
     response = tc.operation_ls(endpoint_id, path=path.as_posix())
-    names = [r['name'] for r in response]
+    names = [r["name"] for r in response]
 
     return [path / n for n in names]
```

### Comparing `dkist-1.4.0rc2/dkist/net/globus/tests/conftest.py` & `dkist-1.5.0rc1/dkist/net/globus/tests/conftest.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 
 from dkist.net.globus.endpoints import get_transfer_client
 
 
 @pytest.fixture()
 def transfer_client(mocker):
     mocker.patch("globus_sdk.TransferClient.get_submission_id",
-                 return_value={'value': "1234"})
+                 return_value={"value": "1234"})
 
     mocker.patch("dkist.net.globus.endpoints.get_refresh_token_authorizer",
-                 return_value={'transfer.api.globus.org': None})
+                 return_value={"transfer.api.globus.org": None})
 
     tc = get_transfer_client()
 
     mocker.patch("dkist.net.globus.endpoints.get_transfer_client",
                  return_value=tc)
     mocker.patch("dkist.net.globus.transfer.get_transfer_client",
                  return_value=tc)
```

### Comparing `dkist-1.4.0rc2/dkist/net/globus/tests/test_auth.py` & `dkist-1.5.0rc1/dkist/net/globus/tests/test_auth.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from dkist.net.globus.auth import (ensure_globus_authorized, get_cache_contents,
                                    get_cache_file_path, get_refresh_token_authorizer,
                                    save_auth_cache, start_local_server)
 
 
 def test_http_server():
     server = start_local_server()
-    redirect_uri = "http://{a[0]}:{a[1]}".format(a=server.server_address)
+    redirect_uri = f"http://{server.server_address[0]}:{server.server_address[1]}"
     inp_code = "wibble"
 
     requests.get(redirect_uri + f"?code={inp_code}")
 
     code = server.wait_for_code()
 
     assert code == inp_code
@@ -70,15 +70,15 @@
     assert filename.exists()
     statinfo = filename.stat()
 
     # Test that the user can read and write
     assert bool(statinfo.mode & stat.S_IRUSR)
     assert bool(statinfo.mode & stat.S_IWUSR)
 
-    if platform.system() != 'Windows':
+    if platform.system() != "Windows":
         # Test that neither "Group" or "Other" have read permissions
         assert not bool(statinfo.mode & stat.S_IRGRP)
         assert not bool(statinfo.mode & stat.S_IROTH)
 
 
 def test_get_refresh_token_authorizer(mocker):
     # An example cache without real tokens
@@ -90,20 +90,20 @@
             "token_type": "Bearer",
             "expires_at_seconds": 1553362861,
             "resource_server": "transfer.api.globus.org"
         }
     }
 
     mocker.patch("dkist.net.globus.auth.get_cache_contents", return_value=cache)
-    auth = get_refresh_token_authorizer()['transfer.api.globus.org']
+    auth = get_refresh_token_authorizer()["transfer.api.globus.org"]
     assert isinstance(auth, globus_sdk.RefreshTokenAuthorizer)
     assert auth.access_token == cache["transfer.api.globus.org"]["access_token"]
 
     mocker.patch("dkist.net.globus.auth.do_native_app_authentication", return_value=cache)
-    auth = get_refresh_token_authorizer(force_reauth=True)['transfer.api.globus.org']
+    auth = get_refresh_token_authorizer(force_reauth=True)["transfer.api.globus.org"]
     assert isinstance(auth, globus_sdk.RefreshTokenAuthorizer)
     assert auth.access_token == cache["transfer.api.globus.org"]["access_token"]
 
 
 def test_ensure_auth_decorator(mocker):
     mock_response = mocker.MagicMock()
     mock_response.status_code = 400
```

### Comparing `dkist-1.4.0rc2/dkist/net/globus/tests/test_endpoints.py` & `dkist-1.5.0rc1/dkist/net/globus/tests/test_endpoints.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,15 +44,15 @@
                         new_callable=mocker.PropertyMock)
 
 
 def test_get_transfer_client(mocker, transfer_client):
     assert isinstance(transfer_client, globus_sdk.TransferClient)
 
 
-@pytest.mark.parametrize("endpoint_id", ("12345", None))
+@pytest.mark.parametrize("endpoint_id", ["12345", None])
 def test_get_local_endpoint_id(mocker, endpoint_id):
     lgcp_mock = mocker.patch("globus_sdk.LocalGlobusConnectPersonal.endpoint_id",
                              new_callable=mocker.PropertyMock)
     lgcp_mock.return_value = endpoint_id
 
     if endpoint_id is None:
         with pytest.raises(ConnectionError):
@@ -64,42 +64,40 @@
 
 def test_get_endpoint_id_search(mocker, mock_search, endpoint_search, transfer_client):
     mock_search.return_value = endpoint_search
 
     transfer_client = get_transfer_client()
 
     # Test exact display name match
-    endpoint_id = get_endpoint_id('NCAR Data Sharing Service', transfer_client)
+    endpoint_id = get_endpoint_id("NCAR Data Sharing Service", transfer_client)
     assert endpoint_id == "dd1ee92a-6d04-11e5-ba46-22000b92c6ec"
 
     # Test multiple match fail
-    with pytest.raises(ValueError) as exc:
+    with pytest.raises(ValueError, match="Multiple"):
         get_endpoint_id(" ", transfer_client)
-    assert "Multiple" in str(exc.value)
 
     # Test just one result
     mock_search.return_value = {"DATA": endpoint_search["DATA"][1:2]}
     endpoint_id = get_endpoint_id(" ", transfer_client)
     assert endpoint_id == "dd1ee92a-6d04-11e5-ba46-22000b92c6ec"
 
     # Test no results
     mock_search.return_value = {"DATA": []}
-    with pytest.raises(ValueError) as e_info:
+    with pytest.raises(ValueError, match="No matches"):
         get_endpoint_id(" ", transfer_client)
-    assert "No matches" in str(e_info.value)
 
 
 def test_get_endpoint_id_uuid(mocker, transfer_client, endpoint_search):
     mocker.patch.object(transfer_client, "get_endpoint",
                         mocker.Mock(return_value=globus_sdk.services.transfer.response.iterable.IterableTransferResponse))
     get_ep_mock = mocker.patch("globus_sdk.services.transfer.response.iterable.IterableTransferResponse.data",
                                new_callable=mocker.PropertyMock)
     get_ep_mock.return_value = {"DATA": endpoint_search["DATA"][1:2]}
 
-    endpoint_id = get_endpoint_id('dd1ee92a-6d04-11e5-ba46-22000b92c6ec', transfer_client)
+    endpoint_id = get_endpoint_id("dd1ee92a-6d04-11e5-ba46-22000b92c6ec", transfer_client)
     assert endpoint_id == "dd1ee92a-6d04-11e5-ba46-22000b92c6ec"
 
 
 def test_get_endpoint_id_invalid_uuid(mocker, mock_search, transfer_client, endpoint_search):
     err = globus_sdk.TransferAPIError(mocker.MagicMock())
     mocker.patch("globus_sdk.TransferClient.get_endpoint",
                  side_effect=err)
@@ -120,19 +118,19 @@
     mocker.patch("dkist.net.globus.endpoints.get_endpoint_id", return_value="12345")
     mocker.patch("dkist.net.globus.endpoints.get_local_endpoint_id",
                  return_value="12345")
     mocker.patch("globus_sdk.TransferClient.operation_ls",
                  return_value=ls_response)
 
     ls = get_directory_listing("/")
-    assert all([isinstance(a, pathlib.Path) for a in ls])
+    assert all(isinstance(a, pathlib.Path) for a in ls)
     assert len(ls) == 13
 
     ls = get_directory_listing("/", "1234")
-    assert all([isinstance(a, pathlib.Path) for a in ls])
+    assert all(isinstance(a, pathlib.Path) for a in ls)
     assert len(ls) == 13
 
 
 def test_get_datacenter_endpoint_id(httpserver):
     httpserver.expect_request("/datasets/v1/config",).respond_with_data(
         json.dumps({"globusDataEndpointID": "example_endpoint_id"}),
     )
```

### Comparing `dkist-1.4.0rc2/dkist/net/globus/tests/test_transfer.py` & `dkist-1.5.0rc1/dkist/net/globus/tests/test_transfer.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,38 +29,38 @@
 @pytest.fixture
 def mock_task_event_list(mocker, transfer_client):
     mock_response = GlobusHTTPResponse(
         json_to_response(
             {
                 "DATA": [
                     {
-                        'DATA_TYPE': 'event',
-                        'code': 'STARTED',
-                        'description': 'started',
-                        'details':
+                        "DATA_TYPE": "event",
+                        "code": "STARTED",
+                        "description": "started",
+                        "details":
                         '{\n  "type": "GridFTP Transfer", \n  "concurrency": 2, \n  "protocol": "Mode S"\n}',
-                        'is_error': False,
-                        'parent_task_id': None,
-                        'time': '2019-05-16 10:13:26+00:00'},
+                        "is_error": False,
+                        "parent_task_id": None,
+                        "time": "2019-05-16 10:13:26+00:00"},
                     {
-                        'DATA_TYPE': 'event',
-                        'code': 'SUCCEEDED',
-                        'description': 'succeeded',
-                        'details': 'Scanned 100 file(s)',
-                        'is_error': False,
-                        'parent_task_id': None,
-                        'time': '2019-05-16 10:13:24+00:00'},
+                        "DATA_TYPE": "event",
+                        "code": "SUCCEEDED",
+                        "description": "succeeded",
+                        "details": "Scanned 100 file(s)",
+                        "is_error": False,
+                        "parent_task_id": None,
+                        "time": "2019-05-16 10:13:24+00:00"},
                     {
-                        'DATA_TYPE': 'event',
-                        'code': 'STARTED',
-                        'description': 'started',
-                        'details': 'Starting sync scan',
-                        'is_error': False,
-                        'parent_task_id': None,
-                        'time': '2019-05-16 10:13:20+00:00'},
+                        "DATA_TYPE": "event",
+                        "code": "STARTED",
+                        "description": "started",
+                        "details": "Starting sync scan",
+                        "is_error": False,
+                        "parent_task_id": None,
+                        "time": "2019-05-16 10:13:20+00:00"},
                 ],
                 "DATA_TYPE": "event_list",
                 "limit": 10,
                 "offset": 0,
                 "total": 3
             }
         ),
@@ -71,99 +71,98 @@
                         return_value=task_list)
 
 
 def test_start_transfer(mocker, transfer_client, mock_endpoints):
     submit_mock = mocker.patch("globus_sdk.TransferClient.submit_transfer",
                                return_value={"task_id": "task_id"})
     mocker.patch("globus_sdk.TransferClient.get_submission_id",
-                 return_value={'value': "wibble"})
+                 return_value={"value": "wibble"})
     file_list = list(map(Path, ["/a/name.fits", "/a/name2.fits"]))
     start_transfer_from_file_list("a", "b", "/", file_list)
     calls = mock_endpoints.call_args_list
     assert calls[0][0][0] == "a"
     assert calls[1][0][0] == "b"
 
     submit_mock.assert_called_once()
-    transfer_manifest = submit_mock.call_args_list[0][0][0]['DATA']
+    transfer_manifest = submit_mock.call_args_list[0][0][0]["DATA"]
 
     for filepath, tfr in zip(file_list, transfer_manifest):
-        assert str(filepath) == tfr['source_path']
-        assert os.path.sep + filepath.name == tfr['destination_path']
+        assert str(filepath) == tfr["source_path"]
+        assert os.path.sep + filepath.name == tfr["destination_path"]
 
 
 def test_start_transfer_src_base(mocker, transfer_client, mock_endpoints):
     submit_mock = mocker.patch("globus_sdk.TransferClient.submit_transfer",
                                return_value={"task_id": "task_id"})
     file_list = list(map(Path, ["/a/b/name.fits", "/a/b/name2.fits"]))
     start_transfer_from_file_list("a", "b", "/", file_list, "/a")
     calls = mock_endpoints.call_args_list
     assert calls[0][0][0] == "a"
     assert calls[1][0][0] == "b"
 
     submit_mock.assert_called_once()
-    transfer_manifest = submit_mock.call_args_list[0][0][0]['DATA']
+    transfer_manifest = submit_mock.call_args_list[0][0][0]["DATA"]
 
     for filepath, tfr in zip(file_list, transfer_manifest):
-        assert str(filepath) == tfr['source_path']
-        assert "{0}b{0}".format(os.path.sep) + filepath.name == tfr['destination_path']
+        assert str(filepath) == tfr["source_path"]
+        assert f"{os.path.sep}b{os.path.sep}" + filepath.name == tfr["destination_path"]
 
 
 def test_process_event_list(transfer_client, mock_task_event_list):
     (events,
      json_events,
      message_events) = _process_task_events("1234", set(), transfer_client)
 
     assert isinstance(events, set)
-    assert all([isinstance(e, tuple) for e in events])
-    assert all([all([isinstance(item, tuple) for item in e]) for e in events])
+    assert all(isinstance(e, tuple) for e in events)
+    assert all(all(isinstance(item, tuple) for item in e) for e in events)
 
     print(events)
     assert len(json_events) == 1
     assert isinstance(json_events, tuple)
     assert isinstance(json_events[0], dict)
-    assert isinstance(json_events[0]['details'], dict)
-    assert json_events[0]['code'] == 'STARTED'
+    assert isinstance(json_events[0]["details"], dict)
+    assert json_events[0]["code"] == "STARTED"
 
     assert len(message_events) == 2
     assert isinstance(message_events, tuple)
     assert isinstance(message_events[0], dict)
-    assert isinstance(message_events[0]['details'], str)
+    assert isinstance(message_events[0]["details"], str)
 
 
 def test_process_event_list_message_only(transfer_client, mock_task_event_list):
     # Filter out the json event
-    prev_events = tuple(map(lambda x: tuple(x.items()),
-                            mock_task_event_list.return_value))
+    prev_events = tuple(tuple(x.items()) for x in mock_task_event_list.return_value)
     prev_events = set(prev_events[0:1])
 
     (events,
      json_events,
      message_events) = _process_task_events("1234", prev_events, transfer_client)
 
     assert isinstance(events, set)
-    assert all([isinstance(e, tuple) for e in events])
-    assert all([all([isinstance(item, tuple) for item in e]) for e in events])
+    assert all(isinstance(e, tuple) for e in events)
+    assert all(all(isinstance(item, tuple) for item in e) for e in events)
 
     assert len(json_events) == 0
     assert isinstance(json_events, tuple)
 
     assert len(message_events) == 2
     assert isinstance(message_events, tuple)
     assert isinstance(message_events[0], dict)
-    assert isinstance(message_events[0]['details'], str)
+    assert isinstance(message_events[0]["details"], str)
 
 
 def test_get_speed():
-    speed = _get_speed({'code': "PROGRESS", 'details': {'mbps': 10}})
+    speed = _get_speed({"code": "PROGRESS", "details": {"mbps": 10}})
     assert speed == 10
     speed = _get_speed({})
     assert speed is None
-    speed = _get_speed({'code': "progress", "details": "hello"})
+    speed = _get_speed({"code": "progress", "details": "hello"})
     assert speed is None
-    speed = _get_speed({'code': "progress", "details": {"hello": "world"}})
+    speed = _get_speed({"code": "progress", "details": {"hello": "world"}})
     assert speed is None
 
 
 @pytest.fixture
 def orchestrate_mocks(mocker):
     wtp = mocker.patch("dkist.net.globus.transfer.watch_transfer_progress",
                        autospec=True)
```

### Comparing `dkist-1.4.0rc2/dkist/net/globus/transfer.py` & `dkist-1.5.0rc1/dkist/net/globus/transfer.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 """
 import copy
 import json
 import time
 import pathlib
 import datetime
 from os import PathLike
-from typing import List, Union, Literal
+from typing import Literal
 
 import globus_sdk
 from tqdm.auto import tqdm
 from tqdm.notebook import tqdm as tqdm_notebook
 
 from .endpoints import (auto_activate_endpoint, get_data_center_endpoint_id,
                         get_endpoint_id, get_local_endpoint_id, get_transfer_client)
 
-__all__ = ['watch_transfer_progress', 'start_transfer_from_file_list']
+__all__ = ["watch_transfer_progress", "start_transfer_from_file_list"]
 
 
 def start_transfer_from_file_list(src_endpoint, dst_endpoint, dst_base_path, file_list,
                                   src_base_path=None, recursive=False, label=None):
     """
     Start a new transfer task for a list of files.
 
@@ -130,56 +130,55 @@
         All the events with json bodies.
 
     message_events : `tuple` of `dict`
         All the events with message bodies.
     """
 
     # Convert all the events into a (key, value) tuple pair
-    events = set(map(lambda x: tuple(x.items()),
-                     tfr_client.task_event_list(task_id)))
+    events = {tuple(x.items()) for x in tfr_client.task_event_list(task_id)}
     # Drop all events we have seen before
     new_events = events.difference(prev_events)
 
     # Filter out the events which are json (start with {)
     json_events = set(filter(lambda x: dict(x).get("details", "").startswith("{"), new_events))
     # All the other events are message events
     message_events = tuple(map(dict, (new_events.difference(json_events))))
 
     def json_loader(x):
         """Modify the event so the json is a dict."""
-        x['details'] = json.loads(x['details'])
+        x["details"] = json.loads(x["details"])
         return x
 
     # If some of the events are json events, load the json.
     if json_events:
         json_events = tuple(map(dict, map(json_loader, map(dict, json_events))))
     else:
-        json_events = tuple()
+        json_events = ()
 
     return events, json_events, message_events
 
 
 def _get_speed(event):
     """
     A helper function to extract the speed from an event.
     """
-    if event.get('code', "").lower() == "progress" and isinstance(event['details'], dict):
-        return event['details'].get("mbps")
+    if event.get("code", "").lower() == "progress" and isinstance(event["details"], dict):
+        return event["details"].get("mbps")
 
 
 def get_progress_bar(*args, **kwargs):  # pragma: no cover
     """
     Return the correct tqdm instance.
     """
     notebook = tqdm is tqdm_notebook
     if not notebook:
-        kwargs['bar_format'] = '{l_bar}{bar}| {n_fmt}/{total_fmt} [{rate_fmt}{postfix}]'
+        kwargs["bar_format"] = "{l_bar}{bar}| {n_fmt}/{total_fmt} [{rate_fmt}{postfix}]"
     else:
         # TODO: Both having this and not having it breaks things.
-        kwargs['total'] = kwargs.get("total", 1e9) or 1e9
+        kwargs["total"] = kwargs.get("total", 1e9) or 1e9
     return tqdm(*args, **kwargs)
 
 
 def watch_transfer_progress(task_id, tfr_client, poll_interval=5,
                             verbose=False, initial_n=None):  # pragma: no cover
     """
     Wait for a Globus transfer task to finish and display a progress bar.
@@ -208,21 +207,21 @@
 
     try:
         while True:
             (prev_events,
              json_events,
              message_events) = _process_task_events(task_id, prev_events, tfr_client)
 
-            if ('code', 'STARTED') not in prev_events and not started:
+            if ("code", "STARTED") not in prev_events and not started:
                 started = True
                 progress.write("PENDING: Starting Transfer")
 
             # Print status messages if verbose or if they are errors
             for event in message_events:
-                if event['is_error'] or verbose:
+                if event["is_error"] or verbose:
                     progress.write(f"{event['code']}: {event['details']}")
 
             for event in json_events:
                 # This block was coded off one example, as I can't find any
                 # documentation of the structure of events. This is why it's
                 # all very tolerant of missing keys etc.
                 if event["is_error"] or verbose:
@@ -241,17 +240,17 @@
             speed = (list(map(_get_speed, json_events)) or [None])[0]
             speed = f"{speed} Mb/s" if speed else ""
             if speed:
                 progress.set_postfix_str(speed)
 
             # Get the status of the task to see how many files we have processed.
             task = tfr_client.get_task(task_id)
-            status = task['status']
-            progress.total = task['files']
-            progress.update((task['files_skipped'] + task['files_transferred']) - progress.n)
+            status = task["status"]
+            progress.total = task["files"]
+            progress.update((task["files_skipped"] + task["files_transferred"]) - progress.n)
 
             # If the status of the task is not active we are finished.
             if status != "ACTIVE":
                 progress.write(f"Task completed with {status} status.")
                 progress.close()
                 break
 
@@ -260,20 +259,20 @@
 
     except KeyboardInterrupt:
         progress.write("Cancelling Task")
         task = tfr_client.cancel_task(task_id)
         progress.close()
 
 
-def _orchestrate_transfer_task(file_list: List[PathLike],
-                               recursive: List[bool],
+def _orchestrate_transfer_task(file_list: list[PathLike],
+                               recursive: list[bool],
                                destination_path: PathLike = "/~/",
                                destination_endpoint: str = None,
                                *,
-                               progress: Union[bool, Literal["verbose"]] = True,
+                               progress: bool | Literal["verbose"] = True,
                                wait: bool = True,
                                label=None):
     """
     Transfer the files given in file_list to the path on ``destination_endpoint``.
 
     Parameters
     ----------
```

### Comparing `dkist-1.4.0rc2/dkist/net/helpers.py` & `dkist-1.5.0rc1/dkist/net/helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,48 +1,50 @@
 """
 Functions and classes for searching and downloading from the data center.
 """
 import datetime
 from os import PathLike
-from typing import List, Union, Literal, Iterable, Optional
+from typing import Literal
 from pathlib import Path
+from collections.abc import Iterable
 
 from astropy import table
+
 from sunpy.net.attr import or_
 from sunpy.net.base_client import QueryResponseRow
 from sunpy.net.fido_factory import UnifiedResponse
 
 from dkist.net.attrs import Dataset
 from dkist.net.client import DKISTClient, DKISTQueryResponseTable
 from dkist.net.globus.transfer import _orchestrate_transfer_task
 from dkist.utils.inventory import path_format_inventory
 
 __all__ = ["transfer_complete_datasets"]
 
 
-def _get_dataset_inventory(dataset_id: Union[str, Iterable[str]]) -> DKISTQueryResponseTable:  # pragma: no cover
+def _get_dataset_inventory(dataset_id: str | Iterable[str]) -> DKISTQueryResponseTable:  # pragma: no cover
     """
     Do a search for a single dataset id
     """
     if isinstance(dataset_id, str):
         search = Dataset(dataset_id)
     else:
         search = or_(*[Dataset(d) for d in dataset_id])
     results = DKISTClient().search(search)
     if len(results) == 0:
         raise ValueError(f"No results available for dataset {dataset_id}")
     return results
 
 
-def transfer_complete_datasets(datasets: Union[str, Iterable[str], QueryResponseRow, DKISTQueryResponseTable, UnifiedResponse],
+def transfer_complete_datasets(datasets: str | Iterable[str] | QueryResponseRow | DKISTQueryResponseTable | UnifiedResponse,
                                path: PathLike = "/~/",
                                destination_endpoint: str = None,
-                               progress: Union[bool, Literal["verbose"]] = True,
+                               progress: bool | Literal["verbose"] = True,
                                wait: bool = True,
-                               label: Optional[str] = None) -> Union[List[str], str]:
+                               label: str | None = None) -> list[str] | str:
     """
     Transfer one or more complete datasets to a path on a globus endpoint.
 
     Parameters
     ----------
     dataset
         The dataset to transfer. This can either be a string dataset id, or it
@@ -95,15 +97,15 @@
     elif isinstance(datasets, UnifiedResponse):
         # If we have a UnifiedResponse object, it could contain one or more dkist tables.
         # Stack them and then treat them like we were passed a single table with many rows.
         datasets = datasets["dkist"]
         if len(datasets) > 1:
             datasets = table.vstack(datasets, metadata_conflicts="silent")
 
-    elif isinstance(datasets, str) or all((isinstance(d, str) for d in datasets)):
+    elif isinstance(datasets, str) or all(isinstance(d, str) for d in datasets):
         # If we are passed just dataset IDs as strings search for them to get the inventory records
         datasets = _get_dataset_inventory(datasets)
 
     else:
         # Anything else, error
         raise TypeError(f"{type(datasets)} is of an unknown type, it should be search results or one or more dataset IDs.")
```

### Comparing `dkist-1.4.0rc2/dkist/net/tests/conftest.py` & `dkist-1.5.0rc1/dkist/net/tests/conftest.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,50 +10,50 @@
     return ("127.0.0.1", 8888)
 
 @pytest.fixture(params=da.__all__)
 def all_dkist_attrs_classes(request):
     return getattr(da, request.param)
 
 
-@pytest.fixture(params=da.__all__ + ['Time', 'Instrument', 'Wavelength', 'Physobs'])
+@pytest.fixture(params=[*da.__all__, "Time", "Instrument", "Wavelength", "Physobs"])
 def all_attrs_classes(request):
     at = getattr(da, request.param, None)
     return at or getattr(a, request.param)
 
 
 @pytest.fixture
 def api_param_names():
     """
     A mapping of attrs to param names in the query string.
 
-    Excludes ones with input dependant query params
+    Excludes ones with input dependent query params
     """
     return {
-        a.Time: ('endTimeMin', 'startTimeMax'),
-        a.Instrument: ('instrumentNames',),
-        a.Wavelength: ('wavelengthRanges',),
-        a.Physobs: ('hasAllStokes',),
-        a.Provider: tuple(),
-        da.Dataset: ('datasetIds',),
-        da.WavelengthBand: ('filterWavelengths',),
-        da.Observable: ('observables',),
-        da.Experiment: ('primaryExperimentIds',),
-        da.Proposal: ('primaryProposalIds',),
-        da.TargetType: ('targetTypes',),
-        da.Recipe: ('recipeId',),
-        da.Embargoed: ('isEmbargoed',),
-        da.FriedParameter: ('qualityAverageFriedParameterMin', 'qualityAverageFriedParameterMax'),
-        da.PolarimetricAccuracy: ('qualityAveragePolarimetricAccuracyMin', 'qualityAveragePolarimetricAccuracyMax'),
-        da.ExposureTime: ('exposureTimeMin', 'exposureTimeMax'),
-        da.EmbargoEndTime: ('embargoEndDateMin', 'embargoEndDateMax'),
-        da.SpectralSampling: ('averageDatasetSpectralSamplingMin', 'averageDatasetSpectralSamplingMax'),
-        da.SpatialSampling: ('averageDatasetSpatialSamplingMin', 'averageDatasetSpatialSamplingMax'),
-        da.TemporalSampling: ('averageDatasetTemporalSamplingMin', 'averageDatasetTemporalSamplingMax'),
-        da.Page: ('pageNumber',),
-        da.PageSize: ('pageSize',),
-        da.SummitSoftwareVersion: ('highLevelSoftwareVersion',),
-        da.WorkflowName: ('workflowName',),
-        da.WorkflowVersion: ('workflowVersion',),
-        da.ObservingProgramExecutionID: ('observingProgramExecutionId',),
-        da.InstrumentProgramExecutionID: ('instrumentProgramExecutionId',),
-        da.HeaderVersion: ('headerVersion',),
+        a.Time: ("endTimeMin", "startTimeMax"),
+        a.Instrument: ("instrumentNames",),
+        a.Wavelength: ("wavelengthRanges",),
+        a.Physobs: ("hasAllStokes",),
+        a.Provider: (),
+        da.Dataset: ("datasetIds",),
+        da.WavelengthBand: ("filterWavelengths",),
+        da.Observable: ("observables",),
+        da.Experiment: ("primaryExperimentIds",),
+        da.Proposal: ("primaryProposalIds",),
+        da.TargetType: ("targetTypes",),
+        da.Recipe: ("recipeId",),
+        da.Embargoed: ("isEmbargoed",),
+        da.FriedParameter: ("qualityAverageFriedParameterMin", "qualityAverageFriedParameterMax"),
+        da.PolarimetricAccuracy: ("qualityAveragePolarimetricAccuracyMin", "qualityAveragePolarimetricAccuracyMax"),
+        da.ExposureTime: ("exposureTimeMin", "exposureTimeMax"),
+        da.EmbargoEndTime: ("embargoEndDateMin", "embargoEndDateMax"),
+        da.SpectralSampling: ("averageDatasetSpectralSamplingMin", "averageDatasetSpectralSamplingMax"),
+        da.SpatialSampling: ("averageDatasetSpatialSamplingMin", "averageDatasetSpatialSamplingMax"),
+        da.TemporalSampling: ("averageDatasetTemporalSamplingMin", "averageDatasetTemporalSamplingMax"),
+        da.Page: ("pageNumber",),
+        da.PageSize: ("pageSize",),
+        da.SummitSoftwareVersion: ("highLevelSoftwareVersion",),
+        da.WorkflowName: ("workflowName",),
+        da.WorkflowVersion: ("workflowVersion",),
+        da.ObservingProgramExecutionID: ("observingProgramExecutionId",),
+        da.InstrumentProgramExecutionID: ("instrumentProgramExecutionId",),
+        da.HeaderVersion: ("headerVersion",),
     }
```

### Comparing `dkist-1.4.0rc2/dkist/net/tests/strategies.py` & `dkist-1.5.0rc1/dkist/net/tests/strategies.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from functools import cache
 
 import hypothesis.strategies as st
 from hypothesis import HealthCheck, assume, settings
 
 import astropy.units as u
 from astropy.time import Time
+
 from sunpy.net import attr
 from sunpy.net import attrs as a
 from sunpy.net.attr import AttrAnd
 from sunpy.net.tests.strategies import TimeDelta, Times, time_attr
 
 from dkist.net import DKISTClient
 from dkist.net.attr_walker import walker
@@ -24,30 +25,30 @@
     Cache this so we only update it once.
     """
     return DKISTClient.register_values()
 
 
 def _generate_from_register_values(attr_type):
     possible_values = get_registered_values()[attr_type]
-    possible_values = list(map(lambda x: x[0], possible_values))
+    possible_values = [x[0] for x in possible_values]
 
     return st.builds(attr_type, st.sampled_from(possible_values))
 
 
 def _supported_attr_types():
     attr_types = list(walker.applymm.registry)
     attr_types.remove(object)
     attr_types.remove(AttrAnd)
     attr_types.remove(a.dkist.BoundingBox)
     return attr_types
 
 
 @st.composite
 def _browse_movie(draw):
-    return a.dkist.BrowseMovie(**draw(st.dictionaries(st.sampled_from(('movieurl', 'movieobjectkey')),
+    return a.dkist.BrowseMovie(**draw(st.dictionaries(st.sampled_from(("movieurl", "movieobjectkey")),
                                st.text(), min_size=1)))
 
 
 def _unit_range(attr_type):
     unit = list(attr_type.__init__.__annotations__.values())
     unit = unit[0] if unit else u.one
```

### Comparing `dkist-1.4.0rc2/dkist/net/tests/test_attr_walker.py` & `dkist-1.5.0rc1/dkist/net/tests/test_attr_walker.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import re
 
 import pytest
 
 import astropy.units as u
 from astropy.coordinates import ICRS, SkyCoord
+
 from sunpy.net import attr
 from sunpy.net import attrs as a
 
 import dkist.net.attrs as da
 from dkist.net.attr_walker import walker
 
 
@@ -19,49 +20,48 @@
 @pytest.fixture
 def query_or_instrument():
     """
     A query which applies or to array types.
     """
     return (a.Instrument("VBI") | a.Instrument("VISP")) & a.Time("2020/06/01", "2020/06/02")
 
-@pytest.fixture(scope="function")
+@pytest.fixture()
 def boundingbox_params():
     """
     Create possible bounding box input coordinates and args
     for inputs to the bounding box tests.
     """
     bottom_left_icrs = SkyCoord(ICRS(ra=1 * u.deg, dec=2 * u.deg, distance=150000000 * u.km),
-                                obstime='2021-01-02T12:34:56')
+                                obstime="2021-01-02T12:34:56")
     top_right_icrs = SkyCoord(ICRS(ra=3 * u.deg, dec=4 * u.deg, distance=150000000 * u.km),
-                              obstime='2021-01-02T12:34:56')
+                              obstime="2021-01-02T12:34:56")
     bottom_left_vector_icrs = SkyCoord([ICRS(ra=1 * u.deg, dec=2 * u.deg, distance=150000000 * u.km),
                                         ICRS(ra=3 * u.deg, dec=4 * u.deg, distance=150000000 * u.km)],
-                                       obstime='2021-01-02T12:34:56')
-    bottom_left = SkyCoord(1 * u.deg, 1 * u.deg, frame='heliographic_stonyhurst', obstime='2021-01-02T12:34:56')
-    top_right = SkyCoord(2 * u.deg, 2 * u.deg, frame='heliographic_stonyhurst', obstime='2021-01-02T12:34:56')
+                                       obstime="2021-01-02T12:34:56")
+    bottom_left = SkyCoord(1 * u.deg, 1 * u.deg, frame="heliographic_stonyhurst", obstime="2021-01-02T12:34:56")
+    top_right = SkyCoord(2 * u.deg, 2 * u.deg, frame="heliographic_stonyhurst", obstime="2021-01-02T12:34:56")
 
     width = 3.4 * u.deg
     height = 1.2 * u.deg
 
-    yield {
+    return {
         # bottom_left, top_right, width, height
         "bottom left vector icrs": [bottom_left_vector_icrs, None, None, None],
         "bottom left top right icrs": [bottom_left_icrs, top_right_icrs, None, None],
         "bottom left top right": [bottom_left, top_right, None, None],
         "bottom left width height": [bottom_left, None, width, height],
     }
 
 
-@pytest.fixture(scope="function",
-                params=["bottom left vector icrs",
+@pytest.fixture(params=["bottom left vector icrs",
                         "bottom left top right icrs",
                         "bottom left top right",
                         "bottom left width height",],)
 def boundingbox_param(request, boundingbox_params):
-    yield boundingbox_params[request.param]
+    return boundingbox_params[request.param]
 
 
 def test_walker_single(all_attrs_classes, api_param_names):
     at = None
 
     if issubclass(all_attrs_classes, da.SpatialSampling):
         at = all_attrs_classes(spatialmin= 1.3 * u.arcsec/u.pix, spatialmax= 1.5 * u.arcsec/u.pix)
@@ -87,60 +87,60 @@
     elif issubclass(all_attrs_classes, attr.Range):
         unit = list(all_attrs_classes.__init__.__annotations__.values())
         unit = unit[0] if unit else u.one
         at = all_attrs_classes(10*unit, 10*unit)
 
     elif issubclass(all_attrs_classes, da.BrowseMovie):
         at = all_attrs_classes(movieurl="klsdjalkjd", movieobjectkey="lkajsd")
-        api_param_names[all_attrs_classes] = ('browseMovieUrl', 'browseMovieObjectKey')
+        api_param_names[all_attrs_classes] = ("browseMovieUrl", "browseMovieObjectKey")
 
     elif issubclass(all_attrs_classes, da.BoundingBox):
         bottom_left = SkyCoord([ICRS(ra=1 * u.deg, dec=2 * u.deg, distance=150000000 * u.km),
                                    ICRS(ra=3 * u.deg, dec=4 * u.deg, distance=150000000 * u.km)],
-                                  obstime='2021-01-02T12:34:56')
+                                  obstime="2021-01-02T12:34:56")
         at = all_attrs_classes(bottom_left=bottom_left)
-        api_param_names[all_attrs_classes] = ('rectangleContainingBoundingBox',)
+        api_param_names[all_attrs_classes] = ("rectangleContainingBoundingBox",)
 
     if not at:
         pytest.skip(f"Not testing {all_attrs_classes!r}")
 
     params = walker.create(at)
     assert isinstance(params, list)
     assert len(params) == 1
     assert isinstance(params[0], dict)
     assert len(params[0]) == len(api_param_names[all_attrs_classes])
     assert not set(api_param_names[all_attrs_classes]).difference(params[0].keys())
 
 
-@pytest.mark.parametrize("search,search_type",
+@pytest.mark.parametrize(("search", "search_type"),
                          [
-                             ('containing', 'rectangleContainingBoundingBox'),
-                             ('contained', 'rectangleContainedByBoundingBox'),
-                             ('intersecting', 'rectangleIntersectingBoundingBox'),
+                             ("containing", "rectangleContainingBoundingBox"),
+                             ("contained", "rectangleContainedByBoundingBox"),
+                             ("intersecting", "rectangleIntersectingBoundingBox"),
                          ]
                          )
 def test_boundingbox(search, search_type, boundingbox_param):
     bb_query = da.BoundingBox(bottom_left=boundingbox_param[0], top_right=boundingbox_param[1],
                        width=boundingbox_param[2], height=boundingbox_param[3], search=search)
 
     out = walker.create(bb_query)
     assert len(out) == 1
-    assert all([isinstance(a, dict) for a in out])
+    assert all(isinstance(a, dict) for a in out)
 
     # can't verify exact coordinates, they change a bit
     for key in out[0].keys():
         assert key == search_type
 
     for value in out[0].values():
         # want to make sure the value is of the format (flt, flt), (flt, flt)
-        coordinate_regex = re.compile(r'^(\()(-?\d+)(\.\d+)?(,)(-?\d+)(\.\d+)?(\))(,)(\()(-?\d+)(\.\d+)?(,)(-?\d+)(\.\d+)?(\))$')
+        coordinate_regex = re.compile(r"^(\()(-?\d+)(\.\d+)?(,)(-?\d+)(\.\d+)?(\))(,)(\()(-?\d+)(\.\d+)?(,)(-?\d+)(\.\d+)?(\))$")
         assert coordinate_regex.search(value)
 
 def test_args_browsemovie():
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match="Either movieurl or movieobjectkey must be specified"):
         da.BrowseMovie()
 
 
 def test_both_physobs():
     params = walker.create(a.Physobs("intensity"))
     assert len(params) == 1
     assert params[0]["hasAllStokes"] is False
@@ -157,30 +157,30 @@
     assert len(params) == 1
     assert params[0]["hasTemporalAxis"] is True
 
 def test_and_simple(query_and_simple):
     out = walker.create(query_and_simple)
     assert len(out) == 1
     assert isinstance(out, list)
-    assert all([isinstance(a, dict) for a in out])
+    assert all(isinstance(a, dict) for a in out)
 
     assert out == [
         {
             "instrumentNames": "VBI",
             "endTimeMin": "2020-06-01T00:00:00.000",
             "startTimeMax": "2020-06-02T00:00:00.000",
         }
     ]
 
 
 def test_or_instrument(query_or_instrument):
     out = walker.create(query_or_instrument)
     assert len(out) == 2
     assert isinstance(out, list)
-    assert all([isinstance(a, dict) for a in out])
+    assert all(isinstance(a, dict) for a in out)
 
     assert out == [
         {
             "instrumentNames": "VBI",
             "endTimeMin": "2020-06-01T00:00:00.000",
             "startTimeMax": "2020-06-02T00:00:00.000",
         },
```

### Comparing `dkist-1.4.0rc2/dkist/net/tests/test_attrs_values.py` & `dkist-1.5.0rc1/dkist/net/tests/test_attrs_values.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,15 +122,15 @@
     assert not success
 
     assert caplog_dkist.record_tuples == [
         ("dkist", logging.INFO, f"Fetching updated search values for the DKIST client to {user_file}"),
         ("dkist", logging.ERROR, "Failed to download new attrs values."),
     ]
 
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match="This is a value error"):
         success = attempt_local_update(silence_errors=False)
 
 
 def _definately_not_json(user_file, *, timeout):
     with open(user_file, "w") as f:
         f.write("This is not json")
 
@@ -147,15 +147,15 @@
         ("dkist", logging.ERROR, "Downloaded file is not valid JSON."),
     ]
 
     with pytest.raises(json.JSONDecodeError):
         success = attempt_local_update(user_file=json_file, silence_errors=False)
 
 
-@pytest.mark.parametrize("user_file, update_needed, allow_update, should_update", [
+@pytest.mark.parametrize(("user_file", "update_needed", "allow_update", "should_update"), [
     ("user_file", False, True, False),
     ("user_file", True, True, True),
     ("user_file", True, False, False),
 ], indirect=["user_file"])
 def test_get_search_attrs_values(mocker, caplog_dkist, values_in_home, user_file, update_needed, allow_update, should_update):
     mocker.patch("dkist.net.attrs_values._get_cached_json",
                  new_callable=lambda: lambda: (user_file, update_needed))
@@ -167,8 +167,8 @@
     if should_update:
         alu_mock.assert_called_once()
     else:
         alu_mock.assert_not_called()
 
     assert isinstance(attr_values, dict)
     # Test that some known attrs are in the result
-    assert set((a.Instrument, a.dkist.HeaderVersion, a.dkist.WorkflowName)).issubset(attr_values.keys())
+    assert {a.Instrument, a.dkist.HeaderVersion, a.dkist.WorkflowName}.issubset(attr_values.keys())
```

### Comparing `dkist-1.4.0rc2/dkist/net/tests/test_client.py` & `dkist-1.5.0rc1/dkist/net/tests/test_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,49 +1,50 @@
 import json
 
-import hypothesis.strategies as st  # noqa
+import hypothesis.strategies as st
 import parfive
 import pytest
 from hypothesis import HealthCheck, given, settings
 
 from sunpy.net import Fido, attr
 from sunpy.net import attrs as a
 from sunpy.net.base_client import QueryResponseRow
 from sunpy.tests.helpers import no_vso
 
 import dkist.net
 from dkist.net.client import DKISTClient, DKISTQueryResponseTable
-from dkist.net.tests import strategies as dst  # noqa
+from dkist.net.tests import strategies as dst
 from dkist.utils.inventory import INVENTORY_KEY_MAP
 
 
 @pytest.fixture
 def client():
     return DKISTClient()
 
 
 @pytest.mark.skip
 @pytest.mark.remote_data
 def test_search(client):
     # TODO: Write an online test to verify real behaviour once there is stable data
-    res = client.search(a.Time("2019/01/01", "2021/01/01"))
+    client.search(a.Time("2019/01/01", "2021/01/01"))
 
 
 @pytest.mark.remote_data
 @pytest.mark.parametrize("time", [
     a.Time("2022/12/27 19:55", "2022/12/27 20:01"), # Time range overlaps the end of the dataset
     a.Time("2022/12/27 19:26", "2022/12/27 19:30"), # Time range overlaps the start of the dataset
     a.Time("2022/12/27 19:30", "2022/12/27 19:35"), # Time range within the dataset
     a.Time("2022/12/27 19:26", "2022/12/27 20:01"), # Time range contains dataset
 ])
 def test_search_by_time(client, time):
         res = client.search(time, a.Instrument("VBI"))
         assert len(res) == 1
         assert res[0]["Primary Proposal ID"] == "pid_1_50"
-        assert res[0]["Start Time"].value == '2022-12-27T19:27:42.338' and res[0]["End Time"].value == '2022-12-27T20:00:09.005'
+        assert res[0]["Start Time"].value == "2022-12-27T19:27:42.338"
+        assert res[0]["End Time"].value == "2022-12-27T20:00:09.005"
 
 @pytest.fixture
 def empty_query_response():
     return DKISTQueryResponseTable()
 
 
 @pytest.fixture
@@ -94,16 +95,16 @@
         ],
     }
 
 
 @pytest.fixture
 def expected_table_keys():
     translated_keys = set(INVENTORY_KEY_MAP.values())
-    removed_keys = {'Wavelength Min', 'Wavelength Max'}
-    added_keys = {'Wavelength'}
+    removed_keys = {"Wavelength Min", "Wavelength Max"}
+    added_keys = {"Wavelength"}
     expected_keys = translated_keys - removed_keys
     expected_keys.update(added_keys)
     return expected_keys
 
 
 @pytest.fixture
 def mocked_client(mocker, client, example_api_response):
@@ -130,22 +131,22 @@
 
 
 def test_query_response_from_results_unknown_field(empty_query_response, example_api_response, expected_table_keys):
     """
     This test asserts that if the API starts returning new fields we don't error, they get passed though verbatim.
     """
     dclient = DKISTClient()
-    example_api_response["searchResults"][0].update({'spamEggs': 'Some Spam'})
+    example_api_response["searchResults"][0].update({"spamEggs": "Some Spam"})
     qr = DKISTQueryResponseTable.from_results([example_api_response], client=dclient)
 
     assert len(qr) == 1
     assert isinstance(qr.client, DKISTClient)
     assert qr.client is dclient
     assert isinstance(qr[0], QueryResponseRow)
-    assert set(qr.colnames).difference(expected_table_keys) == {'spamEggs'}
+    assert set(qr.colnames).difference(expected_table_keys) == {"spamEggs"}
     assert set(qr.colnames).isdisjoint(INVENTORY_KEY_MAP.keys())
 
 
 def test_length_0_qr(empty_query_response):
     assert len(empty_query_response) == 0
     assert str(empty_query_response)
     assert repr(empty_query_response)
@@ -198,33 +199,33 @@
     # It also never passes an AttrAnd, just the components of it
     if isinstance(query, attr.AttrAnd):
         assert client._can_handle_query(*query.attrs)
     else:
         assert client._can_handle_query(query)
 
 
-@pytest.mark.parametrize("query", (
+@pytest.mark.parametrize("query", [
     a.Instrument("bob"),
     a.Physobs("who's got the button"),
     a.Level(2),
     (a.Instrument("VBI"), a.Level(0)),
     (a.Instrument("VBI"), a.Detector("test")),
-    tuple(),
-))
+    (),
+])
 def test_cant_handle_query(client, query):
     """Some examples of invalid queries."""
     assert not client._can_handle_query(query)
 
 
 @no_vso
 @settings(suppress_health_check=[HealthCheck.too_slow, HealthCheck.function_scoped_fixture], deadline=None)
 @given(st.one_of(dst.query_and(), dst.query_or(), dst.query_or_composite()))
 def test_fido_valid(mocker, mocked_client, query):
     # Test that Fido is passing through our queries to our client
-    mocked_search = mocker.patch('dkist.net.client.DKISTClient.search')
+    mocked_search = mocker.patch("dkist.net.client.DKISTClient.search")
     mocked_search.return_value = DKISTQueryResponseTable()
 
     Fido.search(query)
     assert mocked_search.called
 
     if isinstance(query, (attr.DataAttr, attr.AttrAnd)):
         assert mocked_search.call_count == 1
@@ -236,15 +237,15 @@
 def test_fetch_with_headers(httpserver, tmpdir, mocked_client):
     httpserver.expect_request("/download/asdf",
                               query_string="datasetId=abcd").respond_with_data(
                                   b"This isn't an asdf",
                                   headers={"Content-Disposition": "attachment; filename=abcd.asdf"}
                               )
 
-    response = DKISTQueryResponseTable({'Dataset ID': ['abcd']})
+    response = DKISTQueryResponseTable({"Dataset ID": ["abcd"]})
     with dkist.net.conf.set_temp("download_endpoint", httpserver.url_for("/download")):
         downloader = parfive.Downloader()
         mocked_client.fetch(response, downloader=downloader, path=tmpdir / "{file}")
 
     assert len(downloader.http_queue) == 1
 
     results = downloader.download()
```

### Comparing `dkist-1.4.0rc2/dkist/net/tests/test_helpers.py` & `dkist-1.5.0rc1/dkist/net/tests/test_helpers.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from dkist.net.client import DKISTClient, DKISTQueryResponseTable
 from dkist.net.helpers import transfer_complete_datasets
 
 
 @pytest.fixture
 def orchestrate_transfer_mock(mocker):
-    yield mocker.patch("dkist.net.helpers._orchestrate_transfer_task", autospec=True)
+    return mocker.patch("dkist.net.helpers._orchestrate_transfer_task", autospec=True)
 
 
 @pytest.mark.parametrize(
     "keywords",
     [
         {"progress": True, "wait": True, "destination_endpoint": None, "label": None},
         {"progress": True, "wait": False, "destination_endpoint": None, "label": None},
@@ -27,16 +27,16 @@
 def test_download_default_keywords(orchestrate_transfer_mock, keywords):
     transfer_complete_datasets(
         DKISTQueryResponseTable([
             {
                 "Dataset ID": "AAAA",
                 "Primary Proposal ID": "pm_1_10",
                 "Storage Bucket": "data",
-                'Wavelength Max': 856,
-                'Wavelength Min': 854,
+                "Wavelength Max": 856,
+                "Wavelength Min": 854,
             }
         ]),
         **keywords
     )
 
     if keywords["label"] is None:
         keywords["label"] = f"DKIST Python Tools - {datetime.datetime.now().strftime('%Y-%m-%dT%H-%M')} AAAA"
@@ -45,15 +45,15 @@
         recursive=True,
         destination_path=Path("/~"),
         **keywords
     )
 
 
 def test_transfer_unavailable_data(mocker):
-    get_inv_mock = mocker.patch(
+    mocker.patch(
         "dkist.net.client.DKISTClient.search",
         autospec=True,
         return_value=[],
     )
 
     with pytest.raises(ValueError, match="No results available for dataset"):
         transfer_complete_datasets("null")
@@ -64,16 +64,16 @@
         "dkist.net.helpers._get_dataset_inventory",
         autospec=True,
         return_value=DKISTQueryResponseTable([
             {
                 "Dataset ID": "AAAA",
                 "Primary Proposal ID": "pm_1_10",
                 "Storage Bucket": "data",
-                'Wavelength Max': 856,
-                'Wavelength Min': 854,
+                "Wavelength Max": 856,
+                "Wavelength Min": 854,
             }
         ]),
     )
 
     transfer_complete_datasets("AAAA")
 
     orchestrate_transfer_mock.assert_called_once_with(
@@ -94,23 +94,23 @@
         "dkist.net.helpers._get_dataset_inventory",
         autospec=True,
         return_value=DKISTQueryResponseTable([
             {
                 "Dataset ID": "AAAA",
                 "Primary Proposal ID": "pm_1_10",
                 "Storage Bucket": "data",
-                'Wavelength Max': 856,
-                'Wavelength Min': 854,
+                "Wavelength Max": 856,
+                "Wavelength Min": 854,
             },
             {
                 "Dataset ID": "BBBB",
                 "Primary Proposal ID": "pm_1_10",
                 "Storage Bucket": "data",
-                'Wavelength Max': 856,
-                'Wavelength Min': 854,
+                "Wavelength Max": 856,
+                "Wavelength Min": 854,
             }
         ]),
     )
 
     transfer_complete_datasets(["AAAA", "BBBB"])
 
     orchestrate_transfer_mock.assert_has_calls(
@@ -141,16 +141,16 @@
 
 def test_transfer_from_table(orchestrate_transfer_mock, mocker):
     res = DKISTQueryResponseTable(
         {
             "Dataset ID": ["A", "B"],
             "Primary Proposal ID": ["pm_1_10", "pm_2_20"],
             "Storage Bucket": ["data", "data"],
-            'Wavelength Max': [856, 856],
-            'Wavelength Min': [854, 854],
+            "Wavelength Max": [856, 856],
+            "Wavelength Min": [854, 854],
         },
     )
 
     transfer_complete_datasets(res, label="fibble")
 
     kwargs = {"progress": True, "wait": True, "destination_endpoint": None, "label": "fibble"}
     orchestrate_transfer_mock.assert_has_calls(
@@ -173,16 +173,16 @@
 
 def test_transfer_from_length_one_table(orchestrate_transfer_mock, mocker):
     res = DKISTQueryResponseTable(
         {
             "Dataset ID": ["A"],
             "Primary Proposal ID": ["pm_1_10"],
             "Storage Bucket": ["data"],
-            'Wavelength Max': [856],
-            'Wavelength Min': [854],
+            "Wavelength Max": [856],
+            "Wavelength Min": [854],
         },
     )
 
     transfer_complete_datasets(res, label="fibble")
 
     kwargs = {"progress": True, "wait": True, "destination_endpoint": None, "label": "fibble"}
     orchestrate_transfer_mock.assert_has_calls(
@@ -199,16 +199,16 @@
 
 def test_transfer_from_row(orchestrate_transfer_mock, mocker):
     res = DKISTQueryResponseTable(
         {
             "Dataset ID": ["A"],
             "Primary Proposal ID": ["pm_1_10"],
             "Storage Bucket": ["data"],
-            'Wavelength Max': [856],
-            'Wavelength Min': [854],
+            "Wavelength Max": [856],
+            "Wavelength Min": [854],
         },
     )
 
     transfer_complete_datasets(res[0], label="fibble")
 
     kwargs = {"progress": True, "wait": True, "destination_endpoint": None, "label": "fibble"}
     orchestrate_transfer_mock.assert_has_calls(
@@ -226,25 +226,25 @@
 def test_transfer_from_UnifiedResponse(orchestrate_transfer_mock, mocker):
     res = UnifiedResponse(
         DKISTQueryResponseTable(
             {
                 "Dataset ID": ["A"],
                 "Primary Proposal ID": ["pm_1_10"],
                 "Storage Bucket": ["data"],
-            'Wavelength Max': [856],
-            'Wavelength Min': [854],
+            "Wavelength Max": [856],
+            "Wavelength Min": [854],
             },
         ),
         DKISTQueryResponseTable(
             {
                 "Dataset ID": ["B"],
                 "Primary Proposal ID": ["pm_2_20"],
                 "Storage Bucket": ["data"],
-            'Wavelength Max': [856],
-            'Wavelength Min': [854],
+            "Wavelength Max": [856],
+            "Wavelength Min": [854],
             },
         ),
     )
     res._list[0].client = res._list[1].client = DKISTClient()
 
     transfer_complete_datasets(res, label="fibble")
 
@@ -272,16 +272,16 @@
         "dkist.net.helpers._get_dataset_inventory",
         autospec=True,
         return_value=DKISTQueryResponseTable([
             {
                 "Dataset ID": "AAAA",
                 "Primary Proposal ID": "pm_1_10",
                 "Storage Bucket": "data",
-                'Wavelength Max': 856,
-                'Wavelength Min': 854,
+                "Wavelength Max": 856,
+                "Wavelength Min": 854,
                 "Instrument": "HIT",  # Highly Imaginary Telescope
             }
         ]),
     )
 
     transfer_complete_datasets("AAAA", path="{instrument}/{dataset_id}")
```

### Comparing `dkist-1.4.0rc2/dkist/tests/generate_aia_dataset.py` & `dkist-1.5.0rc1/dkist/tests/generate_aia_dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 import os
-import glob
 from pathlib import Path
 
 import numpy as np
 
 import asdf
 import astropy.units as u
 import gwcs
-import sunpy.map
 from astropy.io import fits
 from astropy.modeling.models import (AffineTransformation2D, Multiply,
                                      Pix2Sky_TAN, RotateNative2Celestial, Shift)
 from astropy.time import Time
 from gwcs import coordinate_frames as cf
+
+import sunpy.map
 from sunpy.net import Fido
 from sunpy.net import attrs as a
 from sunpy.net.jsoc import JSOCClient
 from sunpy.time import parse_time
 
 from dkist import load_dataset
-from dkist.asdf_maker.helpers import generate_lookup_table
 
 
 def map_to_transform(smap):
     # crval1u, crval2u = smap.reference_coordinate.Tx, smap.reference_coordinate.Ty
     # cdelt1u, cdelt2u = smap.scale
     # pcu = smap.rotation_matrix * u.arcsec
 
@@ -73,47 +72,49 @@
     from astropy.io.fits.hdu.base import BITPIX2DTYPE
 
     reference_array = np.empty_like(filename_array, dtype=object)
     for i, filepath in enumerate(filename_array.flat):
         with fits.open(filepath) as hdul:
             hdu_index = 1
             hdu = hdul[hdu_index]
-            dtype = BITPIX2DTYPE[hdu.header['BITPIX']]
+            dtype = BITPIX2DTYPE[hdu.header["BITPIX"]]
             shape = tuple(reversed(hdu.shape))
 
             # Convert paths to relative paths
             relative_path = filepath
             if relative_to:
                 relative_path = os.path.relpath(filepath, relative_to)
 
             reference_array.flat[i] = ExternalArrayReference(
                 relative_path, hdu_index, dtype, shape)
 
     return reference_array.tolist()
 
 
 def main():
-    path = Path('~/sunpy/data/jsocflare/').expanduser()
-    files = glob.glob(str(path / '*.fits'))
+    from dkist_inventory.transforms import generate_lookup_table
+
+    path = Path("~/sunpy/data/jsocflare/").expanduser()
+    files = path.glob("*.fits")
 
     # requestid = 'JSOC_20180831_1097'
     requestid = None
 
     if not files:
         if requestid:
             c = JSOCClient()
             filesd = c.get_request(
                 requestid, path=str(path), overwrite=False).wait()
             files = []
             for f in filesd.values():
-                files.append(f['path'])
+                files.append(f["path"])
         else:
             results = Fido.search(
-                a.jsoc.Time('2017-09-06T12:00:00', '2017-09-06T12:02:00'),
-                a.jsoc.Series('aia.lev1_euv_12s'), a.jsoc.Segment('image'),
+                a.jsoc.Time("2017-09-06T12:00:00", "2017-09-06T12:02:00"),
+                a.jsoc.Series("aia.lev1_euv_12s"), a.jsoc.Segment("image"),
                 a.jsoc.Notify("stuart@cadair.com"))
 
             print(results)
 
             files = Fido.fetch(results, path=str(path))
 
     files.sort()
@@ -128,55 +129,54 @@
     seconds = []
     # the wavelength
     waves = []
 
     for i, filepath in enumerate(files):
         with fits.open(filepath) as hdul:
             header = hdul[1].header
-        time = parse_time(header['DATE-OBS'])
+        time = parse_time(header["DATE-OBS"])
         if i == 0:
-            root_header = header
             start_time = time
         inds.append(i)
         times.append(time)
         seconds.append((time - start_time).total_seconds())
-        waves.append(header['WAVELNTH'])
+        waves.append(header["WAVELNTH"])
 
     # Construct an array and sort it by wavelength and time
     arr = np.array((inds, seconds, waves)).T
     sorter = np.lexsort((arr[:, 1], arr[:, 2]))
 
-    # Using this double-sorted array get the list indicies
+    # Using this double-sorted array get the list indices
     list_sorter = np.array(arr[sorter][:, 0], dtype=int)
 
     # Calculate the desired shape of the output array
     n_waves = len(list(set(waves)))
     shape = (n_waves, len(files) // n_waves)
 
     # Construct a 2D array of filenames
     cube = files[list_sorter].reshape(shape)
 
     # Extract a list of coordinates in time and wavelength
     # this assumes all wavelength images are taken at the same time
     time_coords = np.array(
         [t.isoformat() for t in times])[list_sorter].reshape(shape)[0, :]
-    wave_coords = np.array(waves)[list_sorter].reshape(shape)[:, 0]
+    np.array(waves)[list_sorter].reshape(shape)[:, 0]
 
     smap0 = sunpy.map.Map(files[0])
     spatial = map_to_transform(smap0)
 
     timemodel = generate_lookup_table(lookup_table=seconds[:shape[1]]*u.s)
     wavemodel = generate_lookup_table(lookup_table=waves[:shape[0]]*u.AA)
 
     hcubemodel = spatial & timemodel & wavemodel
 
     wave_frame = cf.SpectralFrame(axes_order=(3, ), unit=u.AA, name="wavelength", axes_names=("wavelength", ))
     time_frame = cf.TemporalFrame(
         axes_order=(2, ), unit=u.s, reference_time=Time(time_coords[0]), name="time", axes_names=("time", ))
-    sky_frame = cf.CelestialFrame(axes_order=(0, 1), name='helioprojective',
+    sky_frame = cf.CelestialFrame(axes_order=(0, 1), name="helioprojective",
                                   reference_frame=smap0.coordinate_frame,
                                   axes_names=("helioprojective longitude", "helioprojective latitude"))
 
     sky_frame = cf.CompositeFrame([sky_frame, time_frame, wave_frame])
     detector_frame = cf.CoordinateFrame(name="detector", naxes=4,
                                         axes_order=(0, 1, 2, 3),
                                         axes_type=("pixel", "pixel", "pixel", "pixel"),
@@ -189,23 +189,23 @@
     print(repr(wcs))
 
     print(wcs(*[1*u.pix]*4, with_units=True))
 
     ea = references_from_filenames(cube, relative_to=str(path))
 
     tree = {
-        'gwcs': wcs,
-        'dataset': ea,
+        "gwcs": wcs,
+        "dataset": ea,
     }
 
     with asdf.AsdfFile(tree) as ff:
         # ff.write_to("test.asdf")
-        filename = str(path / "aia_{}.asdf".format(time_coords[0]))
+        filename = str(path / f"aia_{time_coords[0]}.asdf")
         ff.write_to(filename)
-        print("Saved to : {}".format(filename))
+        print(f"Saved to : {filename}")
 
     # import sys; sys.exit(0)
 
     ds = load_dataset(str(path))
     print(repr(ds))
     print(repr(ds.wcs))
     print(ds.wcs(*[1*u.pix]*4, with_units=True))
```

### Comparing `dkist-1.4.0rc2/dkist/tests/generate_eit_test_dataset.py` & `dkist-1.5.0rc1/dkist/tests/generate_eit_test_dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 import numpy as np
 
 import asdf
 import astropy.units as u
 import gwcs
-import sunpy.map
 from astropy.io import fits
 from astropy.modeling.models import (AffineTransformation2D, Multiply,
                                      Pix2Sky_TAN, RotateNative2Celestial, Shift)
 from astropy.table import Table
 from astropy.time import Time
 from gwcs import coordinate_frames as cf
-from sunpy.time import parse_time
 
-from dkist_inventory.asdf_generator import references_from_filenames
-from dkist_inventory.header_parsing import HeaderParser
-from dkist_inventory.transforms import generate_lookup_table
+import sunpy.map
+from sunpy.time import parse_time
 
 
 def map_to_transform(smap):
     # crval1u, crval2u = smap.reference_coordinate.Tx, smap.reference_coordinate.Ty
     # cdelt1u, cdelt2u = smap.scale
     # pcu = smap.rotation_matrix * u.arcsec
 
@@ -55,14 +52,17 @@
     transu.rename("spatial")
 
     return transu
 
 
 def main():
     from dkist.data.test import rootdir
+    from dkist_inventory.asdf_generator import references_from_filenames
+    from dkist_inventory.header_parsing import HeaderParser
+    from dkist_inventory.transforms import generate_lookup_table
     files = list((rootdir / "EIT").glob("*.fits"))
 
     files.sort()
     files = np.array(files)
 
     # For each image get:
     # the index
@@ -74,23 +74,23 @@
 
     headers = []
 
     for i, filepath in enumerate(files):
         with fits.open(filepath) as hdul:
             header = hdul[0].header
             headers.append(dict(header))
-            headers[-1].pop('')
-            headers[-1].pop('COMMENT')
-            headers[-1].pop('HISTORY')
+            headers[-1].pop("")
+            headers[-1].pop("COMMENT")
+            headers[-1].pop("HISTORY")
             headers[-1]["DNAXIS"] = 3
             headers[-1]["DNAXIS3"] = len(files)
             headers[-1]["DAAXES"] = 2
             headers[-1]["DEAXES"] = 1
             headers[-1]["DINDEX3"] = i + 1
-        time = parse_time(header['DATE-OBS'])
+        time = parse_time(header["DATE-OBS"])
         if i == 0:
             start_time = time
         inds.append(i)
         times.append(time)
         seconds.append((time - start_time).to(u.s))
 
     # Extract a list of coordinates in time and wavelength
@@ -100,15 +100,15 @@
     smap0 = sunpy.map.Map(files[0])
     spatial = map_to_transform(smap0)
 
     timemodel = generate_lookup_table(lookup_table=seconds*u.s)
 
     hcubemodel = spatial & timemodel
 
-    sky_frame = cf.CelestialFrame(axes_order=(0, 1), name='helioprojective',
+    sky_frame = cf.CelestialFrame(axes_order=(0, 1), name="helioprojective",
                                   reference_frame=smap0.coordinate_frame,
                                   axes_names=("helioprojective longitude", "helioprojective latitude"))
     time_frame = cf.TemporalFrame(axes_order=(2, ), unit=u.s,
                                   reference_frame=Time(time_coords[0]),
                                   axes_names=("time",))
 
     sky_frame = cf.CompositeFrame([sky_frame, time_frame], name="world")
@@ -131,21 +131,21 @@
     from dkist.dataset import Dataset
 
     meta = {"inventory": {}, "headers": Table(headers)}
     ds = Dataset(ac._generate_array(), wcs, meta=meta, unit=u.count / u.pixel)
     ds._file_manager = ac
 
     tree = {
-        'dataset': ds
+        "dataset": ds
     }
 
     with asdf.AsdfFile(tree) as ff:
         filename = rootdir / "EIT" / "eit_test_dataset.asdf"
         ff.write_to(filename)
-        print("Saved to : {}".format(filename))
+        print(f"Saved to : {filename}")
 
 
     ds.plot()
     import matplotlib.pyplot as plt
     plt.show()
```

### Comparing `dkist-1.4.0rc2/dkist/tests/generate_eit_tiled_dataset.py` & `dkist-1.5.0rc1/dkist/tests/generate_eit_tiled_dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 #!/usr/bin/env python3
 import tempfile
 
 import numpy as np
-from dkist_data_simulator.spec214.vbi import MosaicedVBIBlueDataset
 
 import astropy.units as u
 
 from dkist.data.test import rootdir
-from dkist_inventory.asdf_generator import dataset_from_fits
 
+if __name__ == "__main__":
+    from dkist_data_simulator.spec214.vbi import MosaicedVBIBlueDataset
 
-class DemoMosaicedVBIBlueDataset(MosaicedVBIBlueDataset):
-    @property
-    def data(self):
-        return np.zeros(self.array_shape) + (self.mosaic_keys("MINDEX1") * self.mosaic_keys("MINDEX2"))
+    from dkist_inventory.asdf_generator import dataset_from_fits
 
+    class DemoMosaicedVBIBlueDataset(MosaicedVBIBlueDataset):
+        @property
+        def data(self):
+            return np.zeros(self.array_shape) + (self.mosaic_keys("MINDEX1") * self.mosaic_keys("MINDEX2"))
 
-if __name__ == "__main__":
     mosaic = MosaicedVBIBlueDataset(2, 1, linewave=500*u.nm, detector_shape=(2, 2))
 
     with tempfile.TemporaryDirectory() as tempdir:
         mosaic.generate_files(tempdir, required_only=True)
 
         asdf_filename = rootdir / "test_tiled_dataset.asdf"
         ds = dataset_from_fits(tempdir, asdf_filename)
```

### Comparing `dkist-1.4.0rc2/dkist/tests/test_logger.py` & `dkist-1.5.0rc1/dkist/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/dkist/utils/_model_to_graphviz.py` & `dkist-1.5.0rc1/dkist/utils/_model_to_graphviz.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-This module vizualises compound models by rendering them as a graphviz graph.
+This module visualises compound models by rendering them as a graphviz graph.
 
 It is provided as a helper module which is useful for debugging complex compound models.
 
 It is not tested, incomplete and *should be used at your own risk*.
 """
 
 from functools import singledispatch
@@ -43,24 +43,24 @@
         output_labels = [input_labels[i] for i in model._mapping]
 
     label = repr(model)
     if len(label) > 30:
         label = model.__class__.name
 
     subgraph = pydot.Subgraph(f"{id(model)}_subgraph", label=label)
-    model_node = pydot.Node(name=id(model), label=label, shape='box')
+    model_node = pydot.Node(name=id(model), label=label, shape="box")
     subgraph.add_node(model_node)
 
     for inp, label in zip(inputs, input_labels):
-        input_node = pydot.Node(name=inp, label=label, shape='none')
+        input_node = pydot.Node(name=inp, label=label, shape="none")
         subgraph.add_node(input_node)
         subgraph.add_edge(pydot.Edge(input_node, model_node))
 
     for out, label in zip(outputs, output_labels):
-        output_node = pydot.Node(name=out, label=label, shape='none')
+        output_node = pydot.Node(name=out, label=label, shape="none")
         subgraph.add_node(output_node)
         subgraph.add_edge(pydot.Edge(model_node, output_node))
 
     return subgraph
 
 
 global_int_count = 0
@@ -132,15 +132,15 @@
 
 
 def recursively_find_node(top, name):
     if node := top.get_node(name):
         return node
 
     for sg in top.get_subgraph_list():
-        labels = [n.get_label() for n in sg.get_node_list()]
+        [n.get_label() for n in sg.get_node_list()]
         if node := recursively_find_node(sg, name):
             return node
 
 
 def recursively_find_node_by_label(top, label):
     if top.get_label() == label:
         return top
```

### Comparing `dkist-1.4.0rc2/dkist/utils/inventory.py` & `dkist-1.5.0rc1/dkist/utils/inventory.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 """
 Functions for working with dataset inventory.
 """
 import re
 import string
-from typing import Dict
 from collections import defaultdict
 
 from astropy.table import Table
 
-__all__ = ['dehumanize_inventory', 'humanize_inventory', 'INVENTORY_KEY_MAP']
+__all__ = ["dehumanize_inventory", "humanize_inventory", "INVENTORY_KEY_MAP"]
 
 
 class DefaultMap(defaultdict):
     """
     A tweak of default dict where the default value is the key that's missing.
     """
     def __missing__(self, key):
         return key
 
 
-INVENTORY_KEY_MAP: Dict[str, str] = DefaultMap(None, {
+INVENTORY_KEY_MAP: dict[str, str] = DefaultMap(None, {
         "asdfObjectKey": "asdf Filename",
         "boundingBox": "Bounding Box",
         "browseMovieObjectKey": "Movie Filename",
         "browseMovieUrl": "Preview URL",
         "bucket": "Storage Bucket",
         "contributingExperimentIds": "Experiment IDs",
         "contributingProposalIds": "Proposal IDs",
@@ -74,34 +73,34 @@
         "headerDocumentationUrl": "Header Documentation URL",
         "infoUrl": "Info URL",
         "calibrationDocumentationUrl": "Calibration Documentation URL"
 })
 
 
 def _key_clean(key):
-    key = re.sub('[%s]' % re.escape(string.punctuation), '_', key)
-    key = key.replace(' ', '_')
-    key = ''.join(char for char in key
+    key = re.sub("[%s]" % re.escape(string.punctuation), "_", key)
+    key = key.replace(" ", "_")
+    key = "".join(char for char in key
                     if char.isidentifier() or char.isnumeric())
     return key.lower()
 
 
 def path_format_keys(keymap):
     """
     Return a list of all valid keys for path formatting.
     """
     return tuple(map(_key_clean, keymap.values()))
 
 
 def _path_format_table(keymap=INVENTORY_KEY_MAP):
-    t = Table({'Inventory Keyword': list(keymap.keys()), 'Path Key': path_format_keys(keymap)})
-    return '\n'.join(t.pformat(max_lines=-1, html=True))
+    t = Table({"Inventory Keyword": list(keymap.keys()), "Path Key": path_format_keys(keymap)})
+    return "\n".join(t.pformat(max_lines=-1, html=True))
 
 
-def humanize_inventory(inventory: Dict[str, str]) -> Dict[str, str]:
+def humanize_inventory(inventory: dict[str, str]) -> dict[str, str]:
     """
     Convert an inventory dict to have human readable keys.
     """
     key_converter = DefaultMap(None, INVENTORY_KEY_MAP)
     humanized_inventory = {}
     for key, value in inventory.items():
         humanized_inventory[key_converter[key]] = value
@@ -109,21 +108,21 @@
 
 
 def path_format_inventory(human_inv):
     """
     Given a single humanized inventory record return a dict for formatting paths.
     """
     # Putting this here because of circular imports
-    from ..net.client import DKISTQueryResponseTable as Table
+    from dkist.net.client import DKISTQueryResponseTable as Table
 
     t = Table.from_results([{"searchResults": [human_inv]}], client=None)
     return t[0].response_block_map
 
 
-def dehumanize_inventory(humanized_inventory: Dict[str, str]) -> Dict[str, str]:
+def dehumanize_inventory(humanized_inventory: dict[str, str]) -> dict[str, str]:
     """
     Convert a human readable inventory dict back to the original keys.
     """
     key_converter = DefaultMap(None, {value: key for key, value in INVENTORY_KEY_MAP.items()})
     inventory = {}
     for key, value in humanized_inventory.items():
         inventory[key_converter[key]] = value
```

### Comparing `dkist-1.4.0rc2/dkist/utils/sysinfo.py` & `dkist-1.5.0rc1/dkist/utils/sysinfo.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 import platform
 from importlib.metadata import version, distribution
 
 import sunpy.extern.distro as distro
 from sunpy.util.sysinfo import find_dependencies, get_keys_list, get_requirements
 
-__all__ = ['system_info']
+__all__ = ["system_info"]
 
 
 def system_info():
     """
     Prints one's system info in an "attractive" fashion.
     """
     package_name = "dkist"
     requirements = get_requirements(package_name)
-    base_reqs = get_keys_list(requirements['required'])
+    base_reqs = get_keys_list(requirements["required"])
     missing_packages, installed_packages = find_dependencies(package=package_name)
     extra_prop = {"System": platform.system(),
                   "Arch": f"{platform.architecture()[0]}, ({platform.processor()})",
                   "Python": platform.python_version(),
                   package_name: version(package_name)}
     sys_prop = {**installed_packages, **missing_packages, **extra_prop}
     title_str = f"{package_name} Installation Information"
     print("=" * len(title_str))
     print(title_str)
     print("=" * len(title_str))
     print()
     print("General")
     print("#######")
-    if sys_prop['System'] == "Linux":
+    if sys_prop["System"] == "Linux":
         print(f"OS: {distro.name()} ({distro.version()}, Linux {platform.release()})")
-    elif sys_prop['System'] == "Darwin":
+    elif sys_prop["System"] == "Darwin":
         print(f"OS: Mac OS {platform.mac_ver()[0]}")
-    elif sys_prop['System'] == "Windows":
+    elif sys_prop["System"] == "Windows":
         print(f"OS: Windows {platform.release()} {platform.version()}")
     else:
         print("Unknown OS")
-    for sys_info in ['Arch', package_name]:
-        print(f'{sys_info}: {sys_prop[sys_info]}')
-    print(f'Installation path: {distribution(package_name)._path}')
+    for sys_info in ["Arch", package_name]:
+        print(f"{sys_info}: {sys_prop[sys_info]}")
+    print(f"Installation path: {distribution(package_name)._path}")
     print()
     print("Required Dependencies")
     print("#####################")
     for req in base_reqs:
-        print(f'{req}: {sys_prop[req]}')
+        print(f"{req}: {sys_prop[req]}")
```

### Comparing `dkist-1.4.0rc2/dkist/utils/tests/test_inventory.py` & `dkist-1.5.0rc1/dkist/utils/tests/test_inventory.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
         "hasTemporalAxis": "Has Temporal Axis",
         "averageDatasetSpectralSampling": "Average Spectral Sampling",
         "averageDatasetSpatialSampling": "Average Spatial Sampling",
         "averageDatasetTemporalSampling": "Average Temporal Sampling",
         "qualityReportObjectKey": "Quality Report Filename",
     }
     table = _path_format_table(test_keymap)
-    table = table[table.find('\n')+1:]
+    table = table[table.find("\n")+1:]
 
     assert table == output
 
 
 def test_cycle_single_row():
     tt = DKISTQueryResponseTable.read(rootdir / "AGLKO-inv.ecsv")
     path_format_inventory(dict(tt[0]))
```

### Comparing `dkist-1.4.0rc2/dkist/wcs/models.py` & `dkist-1.5.0rc1/dkist/wcs/models.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from abc import ABC
-from typing import Union, Literal, Iterable
+from typing import Literal
+from itertools import product
+from collections.abc import Iterable
 
 import numpy as np
 
 try:
     from numpy.typing import ArrrayLike  # NOQA
 except ImportError:
     ArrayLike = Iterable
@@ -17,29 +19,28 @@
     "InverseVaryingCelestialTransform",
     "InverseVaryingCelestialTransform2D",
     "InverseVaryingCelestialTransform3D",
     "VaryingCelestialTransform",
     "VaryingCelestialTransform2D",
     "VaryingCelestialTransform3D",
     "BaseVaryingCelestialTransform",
-    "BaseVaryingCelestialTransform2D",
     "generate_celestial_transform",
     "AsymmetricMapping",
     "varying_celestial_transform_from_tables",
     "Ravel",
     "Unravel",
 ]
 
 
 def generate_celestial_transform(
-        crpix: Union[Iterable[float], u.Quantity],
-        cdelt: Union[Iterable[float], u.Quantity],
-        pc: Union[ArrayLike, u.Quantity],
-        crval: Union[Iterable[float], u.Quantity],
-        lon_pole: Union[float, u.Quantity] = None,
+        crpix: Iterable[float] | u.Quantity,
+        cdelt: Iterable[float] | u.Quantity,
+        pc: ArrayLike | u.Quantity,
+        crval: Iterable[float] | u.Quantity,
+        lon_pole: float | u.Quantity = None,
         projection: Model = m.Pix2Sky_TAN(),
 ) -> CompoundModel:
     """
     Create a simple celestial transform from FITS like parameters.
 
     Supports unitful or unitless parameters, but if any parameters have units
     all must have units, if parameters are unitless they are assumed to be in
@@ -97,23 +98,26 @@
 
 
 class BaseVaryingCelestialTransform(Model, ABC):
     """
     Shared components between the forward and reverse varying celestial transforms.
     """
 
-    # This prevents Model from broadcasting the paramters to the inputs
+    # This prevents Model from broadcasting the parameters to the inputs
     standard_broadcasting = False
     _separable = False
     _input_units_allow_dimensionless = True
+    _is_inverse = False
 
     crpix = Parameter()
     cdelt = Parameter()
     lon_pole = Parameter(default=180)
 
+    n_outputs = 2
+
     @staticmethod
     def _validate_table_shapes(pc_table, crval_table):
         table_shape = None
         if pc_table.shape != (2, 2):
             if pc_table.shape[-2:] != (2, 2):
                 raise ValueError("The pc table should be an array of 2x2 matrices.")
             table_shape = pc_table.shape[:-2]
@@ -127,38 +131,48 @@
                 if table_shape != crval_table.shape[:-1]:
                     raise ValueError("The shape of the pc and crval tables should match. "
                                      f"The pc table has shape {table_shape} and the "
                                      f"crval table has shape {crval_table.shape[:-1]}")
             table_shape = crval_table.shape[:-1]
 
         if pc_table.shape == (2, 2):
-            pc_table = np.broadcast_to(pc_table, list(table_shape) + [2, 2], subok=True)
+            pc_table = np.broadcast_to(pc_table, [*list(table_shape), 2, 2], subok=True)
         if crval_table.shape == (2,):
-            crval_table = np.broadcast_to(crval_table, list(table_shape) + [2], subok=True)
+            crval_table = np.broadcast_to(crval_table, [*list(table_shape), 2], subok=True)
 
         return table_shape, pc_table, crval_table
 
     @staticmethod
     def sanitize_index(ind):
         if isinstance(ind, u.Quantity):
             ind = ind.value
         return np.array(np.round(ind), dtype=int)
 
     def __init__(self, *args, crval_table=None, pc_table=None, projection=m.Pix2Sky_TAN(), **kwargs):
         super().__init__(*args, **kwargs)
         (
             self.table_shape,
             self.pc_table,
-            self.crval_table
+            self.crval_table,
         ) = self._validate_table_shapes(np.asanyarray(pc_table), np.asanyarray(crval_table))
 
         if not isinstance(projection, m.Pix2SkyProjection):
             raise TypeError("The projection keyword should be a Pix2SkyProjection model class.")
         self.projection = projection
 
+        if self._is_inverse:
+            self.inputs = ("lon", "lat", "z", "q", "m")[:self.n_inputs]
+            self.outputs = ("x", "y")
+        else:
+            self.inputs = ("x", "y", "z", "q", "m")[:self.n_inputs]
+            self.outputs = ("lon", "lat")
+
+        if len(self.table_shape) != self.n_inputs-2:
+            raise ValueError(f"This model can only be constructed with a {self.n_inputs-2}-dimensional lookup table.")
+
     def transform_at_index(self, ind, crpix=None, cdelt=None, lon_pole=None):
         """
         Generate a spatial model based on an index for the pc and crval tables.
 
         Parameters
         ----------
         zind : int
@@ -180,321 +194,162 @@
 
         fill_val = np.nan
         if isinstance(crpix, u.Quantity):
             fill_val = np.nan * u.deg
         if (np.array(ind) > np.array(self.table_shape) - 1).any() or (np.array(ind) < 0).any():
             return m.Const1D(fill_val) & m.Const1D(fill_val)
 
-        sct = generate_celestial_transform(
+        return generate_celestial_transform(
             crpix=crpix,
             cdelt=cdelt,
             pc=self.pc_table[ind],
             crval=self.crval_table[ind],
             lon_pole=lon_pole,
             projection=self.projection,
         )
 
-        return sct
 
-    def _map_transform(self, x, y, z, crpix, cdelt, lon_pole, inverse=False):
+    def _map_transform(self, *arrays, crpix, cdelt, lon_pole, inverse=False):
         # We need to broadcast the arrays together so they are all the same shape
-        bx, by, bz = np.broadcast_arrays(x, y, z, subok=True)
-        # Convert the z coordinate into an index to the lookup tables
-        zind = self.sanitize_index(bz)
+        barrays = np.broadcast_arrays(*arrays, subok=True)
+        # # Convert the z, q, and m coordinates where present into indices to the lookup tables
+        inds = []
+        for barray in barrays[2:]:
+            inds.append(self.sanitize_index(barray))
 
         # Generate output arrays (ignore units for simplicity)
-        if isinstance(bx, u.Quantity):
-            x_out = np.empty_like(bx.value)
-            y_out = np.empty_like(by.value)
+        if isinstance(barrays[0], u.Quantity):
+            x_out = np.empty_like(barrays[0].value)
+            y_out = np.empty_like(barrays[1].value)
         else:
-            x_out = np.empty_like(bx)
-            y_out = np.empty_like(by)
+            x_out = np.empty_like(barrays[0])
+            y_out = np.empty_like(barrays[1])
 
         # We now loop over every unique value of z and compute the transform.
         # This means we make the minimum number of calls possible to the transform.
-        z_range = np.unique(zind)
-        for zzind in z_range:
+        ranges = [np.unique(ind) for ind in inds]
+        for ind in product(*ranges):
             # Scalar parameters are reshaped to be length one arrays by modeling
-            sct = self.transform_at_index(zzind, crpix[0], cdelt[0], lon_pole[0])
+            sct = self.transform_at_index(ind, crpix=crpix[0], cdelt=cdelt[0], lon_pole=lon_pole[0])
 
             # Call this transform for all values of x, y where z == zind
-            mask = zind == zzind
+            masks = [inds[i] == ind[i] for i in range(len(ind))]
+            if len(masks) > 1:
+                mask = np.logical_and(*masks)
+            else:
+                mask = masks[0]
             if inverse:
-                xx, yy = sct.inverse(bx[mask], by[mask])
+                xx, yy = sct.inverse(barrays[0][mask], barrays[1][mask])
             else:
-                xx, yy = sct(bx[mask], by[mask])
+                xx, yy = sct(barrays[0][mask], barrays[1][mask])
 
             if isinstance(xx, u.Quantity):
                 x_out[mask], y_out[mask] = xx.value, yy.value
             else:
                 x_out[mask], y_out[mask] = xx, yy
 
         # Put the units back
         if isinstance(xx, u.Quantity):
             x_out = x_out << xx.unit
             y_out = y_out << yy.unit
 
         return x_out, y_out
 
+    def evaluate(self, *inputs):
+        # This method has to be able to take an arbitrary number of arrays but also accept not being given kwargs
+        # Fortunately we know how many arrays to expect from the number of inputs
+        # Anything extra is therefore a kwarg
+        arrays = inputs[:self.n_inputs]
+        kwargs = inputs[self.n_inputs:]
+        keys = ["crpix", "cdelt", "lon_pole"]
+        kwargs = dict(zip(keys, kwargs))
+        return self._map_transform(*arrays, inverse=self._is_inverse, **kwargs)
+
+    @property
+    def input_units(self):
+        # NB: x and y are normally on the detector and z is typically the number of raster steps
+        if self._is_inverse:
+            dims = ["z", "q", "m"]
+            {d: u.pix for d in dims[:self.n_inputs]}
+            units = {"lon": u.deg, "lat": u.deg}
+            for d in dims[:self.n_inputs-2]:
+                units[d] = u.pix
+            return units
+
+        dims = ["x", "y", "z", "q", "m"]
+        return {d: u.pix for d in dims[:self.n_inputs]}
+
 
 class VaryingCelestialTransform(BaseVaryingCelestialTransform):
     """
-    A celestial transform which can vary it's pointing and rotation with time.
+    A celestial transform which can vary its pointing and rotation with time.
 
     This model stores a lookup table for the reference pixel ``crval_table``
     and the rotation matrix ``pc_table`` which are indexed with a third pixel
     index (z).
 
     The other parameters (``crpix``, ``cdelt``, and ``lon_pole``) are fixed.
     """
     n_inputs = 3
-    n_outputs = 2
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.inputs = ("x", "y", "z")
-        self.outputs = ("lon", "lat")
-
-        if len(self.table_shape) != 1:
-            raise ValueError("This model can only be constructed with a one dimensional lookup table.")
-
-    @property
-    def input_units(self):
-        # NB: x and y are normally on the detector and z is typically the number of raster steps
-        return {"x": u.pix, "y": u.pix, "z": u.pix}
-
-    def evaluate(self, x, y, z, crpix, cdelt, lon_pole):
-        return self._map_transform(x, y, z, crpix, cdelt, lon_pole)
 
     @property
     def inverse(self):
-        ivct = InverseVaryingCelestialTransform(
+        return InverseVaryingCelestialTransform(
             crpix=self.crpix,
             cdelt=self.cdelt,
             lon_pole=self.lon_pole,
             pc_table=self.pc_table,
             crval_table=self.crval_table,
             projection=self.projection,
         )
-        return ivct
-
-
-class InverseVaryingCelestialTransform(BaseVaryingCelestialTransform):
-    """
-    The inverse of VaryingCelestialTransform.
-
-    This inverse still depends on the pixel coordinate ``z`` to index the lookup tables.
-    """
-    n_inputs = 3
-    n_outputs = 2
-
-    @property
-    def input_units(self):
-        return {"lon": u.deg, "lat": u.deg, "z": u.pix}
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.inputs = ("lon", "lat", "z")
-        self.outputs = ("x", "y")
-
-    def evaluate(self, lon, lat, z, crpix, cdelt, lon_pole, **kwargs):
-        return self._map_transform(lon, lat, z, crpix, cdelt, lon_pole, inverse=True)
-
-
-class BaseVaryingCelestialTransform2D(BaseVaryingCelestialTransform, ABC):
-    def _map_transform(self, x, y, z, q, crpix, cdelt, lon_pole, inverse=False):
-        # We need to broadcast the arrays together so they are all the same shape
-        bx, by, bz, bq = np.broadcast_arrays(x, y, z, q, subok=True)
-        # Convert the z coordinate into an index to the lookup tables
-        zind = self.sanitize_index(bz)
-        qind = self.sanitize_index(bq)
-
-        # Generate output arrays (ignore units for simplicity)
-        if isinstance(bx, u.Quantity):
-            x_out = np.empty_like(bx.value)
-            y_out = np.empty_like(by.value)
-        else:
-            x_out = np.empty_like(bx)
-            y_out = np.empty_like(by)
 
-        # We now loop over every unique value of z and compute the transform.
-        # This means we make the minimum number of calls possible to the transform.
-        z_range = np.unique(zind)  # raster
-        q_range = np.unique(qind)  # other: maps or meas
-        for zz in z_range:
-            for qq in q_range:
-                # Scalar parameters are reshaped to be length one arrays by modeling
-                sct = self.transform_at_index((zz, qq), crpix[0], cdelt[0], lon_pole[0])
-
-                # Call this transform for all values of x, y where z == zind and q == qind
-                mask = np.logical_and(zind == zz, qind == qq)
-                if inverse:
-                    xx, yy = sct.inverse(bx[mask], by[mask])
-                else:
-                    xx, yy = sct(bx[mask], by[mask])
-
-                if isinstance(xx, u.Quantity):
-                    x_out[mask], y_out[mask] = xx.value, yy.value
-                else:
-                    x_out[mask], y_out[mask] = xx, yy
 
-        # Put the units back
-        if isinstance(xx, u.Quantity):
-            x_out = x_out << xx.unit
-            y_out = y_out << yy.unit
-
-        return x_out, y_out
-
-
-class VaryingCelestialTransform2D(BaseVaryingCelestialTransform2D):
+class VaryingCelestialTransform2D(BaseVaryingCelestialTransform):
     n_inputs = 4
-    n_outputs = 2
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.inputs = ("x", "y", "z", "q")
-        self.outputs = ("lon", "lat")
-
-        if len(self.table_shape) != 2:
-            raise ValueError("This model can only be constructed with a two dimensional lookup table.")
-
-    @property
-    def input_units(self):
-        return {"x": u.pix, "y": u.pix, "z": u.pix, "q": u.pix}
-
-    def evaluate(self, x, y, z, q, crpix, cdelt, lon_pole):
-        return self._map_transform(x, y, z, q, crpix, cdelt, lon_pole)
 
     @property
     def inverse(self):
-        ivct = InverseVaryingCelestialTransform2D(
+        return InverseVaryingCelestialTransform2D(
             crpix=self.crpix,
             cdelt=self.cdelt,
             lon_pole=self.lon_pole,
             pc_table=self.pc_table,
             crval_table=self.crval_table,
             projection=self.projection,
         )
-        return ivct
-
-
-class InverseVaryingCelestialTransform2D(BaseVaryingCelestialTransform2D):
-    n_inputs = 4
-    n_outputs = 2
-
-    @property
-    def input_units(self):
-        return {"lon": u.deg, "lat": u.deg, "z": u.pix, "q": u.pix}
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.inputs = ("lon", "lat", "z", "q")
-        self.outputs = ("x", "y")
 
-    def evaluate(self, lon, lat, z, q, crpix, cdelt, lon_pole, **kwargs):
-        return self._map_transform(lon, lat, z, q, crpix, cdelt, lon_pole,
-                                   inverse=True)
 
-class BaseVaryingCelestialTransform3D(BaseVaryingCelestialTransform, ABC):
-    def _map_transform(self, x, y, m, z, q, crpix, cdelt, lon_pole, inverse=False):
-        # We need to broadcast the arrays together so they are all the same shape
-        bx, by, bm, bz, bq = np.broadcast_arrays(x, y, m, z, q, subok=True)
-        # Convert the z coordinate into an index to the lookup tables
-        zind = self.sanitize_index(bz)
-        qind = self.sanitize_index(bq)
-        mind = self.sanitize_index(bm)
-
-        # Generate output arrays (ignore units for simplicity)
-        if isinstance(bx, u.Quantity):
-            x_out = np.empty_like(bx.value)
-            y_out = np.empty_like(by.value)
-        else:
-            x_out = np.empty_like(bx)
-            y_out = np.empty_like(by)
-
-        # We now loop over every unique value of z and compute the transform.
-        # This means we make the minimum number of calls possible to the transform.
-        m_range = np.unique(mind)  # raster
-        q_range = np.unique(qind)  # maps
-        z_range = np.unique(zind)  # meas
-        for mm in m_range:
-            for zz in z_range:
-                for qq in q_range:
-                    # Scalar parameters are reshaped to be length one arrays by modeling
-                    sct = self.transform_at_index((mm, zz, qq), crpix[0], cdelt[0], lon_pole[0])
-
-                    # Call this transform for all values of x, y where z == zind q == qind and m == mind
-                    mask = np.logical_and(np.logical_and(mind == mm, zind == zz), qind == qq)
-                    if inverse:
-                        xx, yy = sct.inverse(bx[mask], by[mask])
-                    else:
-                        xx, yy = sct(bx[mask], by[mask])
-
-                    if isinstance(xx, u.Quantity):
-                        x_out[mask], y_out[mask] = xx.value, yy.value
-                    else:
-                        x_out[mask], y_out[mask] = xx, yy
-
-        # Put the units back
-        if isinstance(xx, u.Quantity):
-            x_out = x_out << xx.unit
-            y_out = y_out << yy.unit
-
-        return x_out, y_out
-
-
-
-class VaryingCelestialTransform3D(BaseVaryingCelestialTransform3D):
+class VaryingCelestialTransform3D(BaseVaryingCelestialTransform):
     n_inputs = 5
-    n_outputs = 2
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.inputs = ("x", "y", "m", "z", "q")
-        self.outputs = ("lon", "lat")
-
-        if len(self.table_shape) != 3:
-            raise ValueError("This model can only be constructed with a three dimensional lookup table.")
-
-    @property
-    def input_units(self):
-        return {"x": u.pix, "y": u.pix, "m": u.pix, "z": u.pix, "q": u.pix}
-
-    def evaluate(self, x, y, m, z, q, crpix, cdelt, lon_pole):
-        return self._map_transform(x, y, m, z, q, crpix, cdelt, lon_pole)
 
     @property
     def inverse(self):
-        ivct = InverseVaryingCelestialTransform3D(
+        return InverseVaryingCelestialTransform3D(
             crpix=self.crpix,
             cdelt=self.cdelt,
             lon_pole=self.lon_pole,
             pc_table=self.pc_table,
             crval_table=self.crval_table,
             projection=self.projection,
         )
-        return ivct
 
 
-class InverseVaryingCelestialTransform3D(BaseVaryingCelestialTransform3D):
-    n_inputs = 5
-    n_outputs = 2
+class InverseVaryingCelestialTransform(BaseVaryingCelestialTransform):
+    n_inputs = 3
+    _is_inverse = True
 
-    @property
-    def input_units(self):
-        return {"lon": u.deg, "lat": u.deg, "m": u.pix, "z": u.pix, "q": u.pix}
+class InverseVaryingCelestialTransform2D(BaseVaryingCelestialTransform):
+    n_inputs = 4
+    _is_inverse = True
 
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.inputs = ("lon", "lat", "m", "z", "q")
-        self.outputs = ("x", "y")
 
-    def evaluate(self, lon, lat, m, z, q, crpix, cdelt, lon_pole, **kwargs):
-        return self._map_transform(lon, lat, m, z, q, crpix, cdelt, lon_pole,
-                                   inverse=True)
+class InverseVaryingCelestialTransform3D(BaseVaryingCelestialTransform):
+    n_inputs = 5
+    _is_inverse = True
+
 
 class CoupledCompoundModel(CompoundModel):
     """
     This class takes two models which share one or more inputs on the forward
     transform, and where the left hand model's inverse is dependent on the
     output of the right hand model's inverse output.
 
@@ -668,28 +523,28 @@
         return f"<AsymmetricMapping({self.mapping}, name={self.name!r})>"
 
 varying_celestial_transform_dict = {
     # Map (num_dims, inverse) to class
     (1, False): VaryingCelestialTransform,
     (2, False): VaryingCelestialTransform2D,
     (3, False): VaryingCelestialTransform3D,
-    (1,  True): InverseVaryingCelestialTransform,
-    (2,  True): InverseVaryingCelestialTransform2D,
-    (3,  True): InverseVaryingCelestialTransform3D,
+    (1, True): InverseVaryingCelestialTransform,
+    (2, True): InverseVaryingCelestialTransform2D,
+    (3, True): InverseVaryingCelestialTransform3D,
 }
 
 def varying_celestial_transform_from_tables(
-        crpix: Union[Iterable[float], u.Quantity],
-        cdelt: Union[Iterable[float], u.Quantity],
-        pc_table: Union[ArrayLike, u.Quantity],
-        crval_table: Union[Iterable[float], u.Quantity],
-        lon_pole: Union[float, u.Quantity] = None,
+        crpix: Iterable[float] | u.Quantity,
+        cdelt: Iterable[float] | u.Quantity,
+        pc_table: ArrayLike | u.Quantity,
+        crval_table: Iterable[float] | u.Quantity,
+        lon_pole: float | u.Quantity = None,
         projection: Model = m.Pix2Sky_TAN(),
         inverse: bool = False,
-        slit: Union[None, Literal[0, 1]] = None,
+        slit: None | Literal[0, 1] = None,
 ) -> BaseVaryingCelestialTransform:
     """
     Generate a `.BaseVaryingCelestialTransform` based on the dimensionality of the tables.
     """
 
     table_shape, _, _ = BaseVaryingCelestialTransform._validate_table_shapes(
         pc_table,
@@ -739,48 +594,49 @@
 
     @inputs.setter
     def inputs(self, value):
         self._inputs = value
 
     @property
     def input_units(self):
-        return {f'x{idx}': u.pix for idx in range(self.n_inputs)}
+        return {f"x{idx}": u.pix for idx in range(self.n_inputs)}
 
     @property
     def outputs(self):
         return self._outputs
 
     @outputs.setter
     def outputs(self, value):
         self._outputs = value
 
     @property
     def return_units(self):
-        return {'y': u.pix}
+        return {"y": u.pix}
 
-    def __init__(self, array_shape, order='C', **kwargs):
+    def __init__(self, array_shape, order="C", **kwargs):
         if len(array_shape) < 2 or np.prod(array_shape) < 1:
             raise ValueError("array_shape must be at least 2D and have values >= 1")
         self.array_shape = tuple(array_shape)
         if order not in ("C", "F"):
             raise ValueError("order kwarg must be one of 'C' or 'F'")
         self.order = order
         super().__init__(**kwargs)
         # super dunder init sets inputs and outputs to default values so set what we want here
-        self.inputs = tuple([f'x{idx}' for idx in range(self.n_inputs)])
-        self.outputs = 'y',
+        self.inputs = tuple([f"x{idx}" for idx in range(self.n_inputs)])
+        self.outputs = "y",
 
     def evaluate(self, *inputs_):
         """Evaluate the forward ravel for a given tuple of pixel values."""
         if hasattr(inputs_[0], "unit"):
             has_units = True
             input_values = [item.to_value(u.pix) for item in inputs_]
         else:
             has_units = False
             input_values = inputs_
+        input_values = [item.flatten() if isinstance(item, np.ndarray) else item for item in input_values]
         # round the index values, but clip them if they exceed the array bounds
         # the bounds are one less than the shape dimension value
         array_bounds = np.array(self.array_shape) - 1
         rounded_inputs = np.clip(np.rint(input_values).astype(int), None, array_bounds[:, np.newaxis])
         result = np.ravel_multi_index(rounded_inputs, self.array_shape, order=self.order).astype(float)
         index = 0 if self.order == "F" else -1
         # Adjust the result to allow a fractional part for interpolation in Tabular1D
@@ -812,15 +668,15 @@
 
     @inputs.setter
     def inputs(self, value):
         self._inputs = value
 
     @property
     def input_units(self):
-        return {'x': u.pix}
+        return {"x": u.pix}
 
     @property
     def n_outputs(self):
         return len(self.array_shape)
 
     @property
     def outputs(self):
@@ -828,27 +684,27 @@
 
     @outputs.setter
     def outputs(self, value):
         self._outputs = value
 
     @property
     def return_units(self):
-        return {f'y{idx}': u.pix for idx in range(self.n_outputs)}
+        return {f"y{idx}": u.pix for idx in range(self.n_outputs)}
 
-    def __init__(self, array_shape, order='C', **kwargs):
+    def __init__(self, array_shape, order="C", **kwargs):
         if len(array_shape) < 2 or np.prod(array_shape) < 1:
             raise ValueError("array_shape must be at least 2D and have values >= 1")
         self.array_shape = array_shape
         if order not in ("C", "F"):
             raise ValueError("order kwarg must be one of 'C' or 'F'")
         self.order = order
         super().__init__(**kwargs)
         # super dunder init sets inputs and outputs to default values so set what we want here
-        self.inputs = 'x',
-        self.outputs = tuple([f'y{idx}' for idx in range(self.n_outputs)])
+        self.inputs = "x",
+        self.outputs = tuple([f"y{idx}" for idx in range(self.n_outputs)])
 
     def evaluate(self, input_):
         """Evaluate the reverse ravel (unravel) for a given pixel value."""
         if hasattr(input_, "unit"):
             has_units = True
             input_value = [item.to_value(u.pix) for item in input_]
             input_value_int = [int(item) for item in input_value]
```

### Comparing `dkist-1.4.0rc2/dkist/wcs/tests/test_coupled_compound_model.py` & `dkist-1.5.0rc1/dkist/wcs/tests/test_coupled_compound_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -129,38 +129,38 @@
                                           [0, 0, 0, 1, 0],
                                           [0, 0, 0, 0, 1]]))
 
 
 def test_coupled_slit_no_repeat(linear_time):
     pc_table = [rotation_matrix(a)[:2, :2] for a in np.linspace(0, 90, 10)] * u.pix
 
-    kwargs = dict(crpix=(5, 5) * u.pix,
-                  cdelt=(1, 1) * u.arcsec/u.pix,
-                  crval_table=(0, 0) * u.arcsec,
-                  lon_pole=180 * u.deg,
-                  slit=1)
+    kwargs = {"crpix": (5, 5) * u.pix,
+              "cdelt": (1, 1) * u.arcsec/u.pix,
+              "crval_table": (0, 0) * u.arcsec,
+              "lon_pole": 180 * u.deg,
+              "slit": 1}
 
     vct_slit = varying_celestial_transform_from_tables(pc_table=pc_table, **kwargs)
 
     tfrm = CoupledCompoundModel("&", vct_slit, linear_time, shared_inputs=1)
     pixel = (0*u.pix, 4*u.pix)
     world = tfrm(*pixel)
     ipixel = tfrm.inverse(*world)
     assert u.allclose(ipixel, pixel, atol=1e-5*u.pix)
 
 
 def test_coupled_slit_with_repeat(linear_time):
     pc_table = [rotation_matrix(a)[:2, :2] for a in np.linspace(0, 90, 15)] * u.pix
     pc_table = pc_table.reshape((5, 3, 2, 2))
 
-    kwargs = dict(crpix=(5, 5) * u.pix,
-                  cdelt=(1, 1) * u.arcsec/u.pix,
-                  crval_table=(0, 0) * u.arcsec,
-                  lon_pole=180 * u.deg,
-                  slit=1)
+    kwargs = {"crpix": (5, 5) * u.pix,
+              "cdelt": (1, 1) * u.arcsec/u.pix,
+              "crval_table": (0, 0) * u.arcsec,
+              "lon_pole": 180 * u.deg,
+              "slit": 1}
 
     vct_slit = varying_celestial_transform_from_tables(pc_table=pc_table, **kwargs)
 
     tfrm = CoupledCompoundModel("&", vct_slit, linear_time & linear_time, shared_inputs=2)
     pixel = (0*u.pix, 0*u.pix, 0*u.pix)
     world = tfrm(*pixel)
     ipixel = tfrm.inverse(*world)
```

### Comparing `dkist-1.4.0rc2/dkist/wcs/tests/test_models.py` & `dkist-1.5.0rc1/dkist/wcs/tests/test_models.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,23 +89,23 @@
     pixel = (0*u.pix, 0*u.pix, 5*u.pix)
     world = vct(*pixel)
     assert np.array(world[0]).shape == ()
     assert u.allclose(world, (359.99804329*u.deg, 0.00017119*u.deg))
     assert u.allclose(vct.inverse(*world, 5*u.pix), pixel[:2], atol=0.01*u.pix)
 
 
-@pytest.mark.parametrize(("pixel", "lon_shape"), (
+@pytest.mark.parametrize(("pixel", "lon_shape"), [
     ((*np.mgrid[0:10, 0:10] * u.pix, np.arange(10) * u.pix), (10, 10)),
     (np.mgrid[0:10, 0:10, 0:5] * u.pix, (10, 10, 5)),
     ((2 * u.pix, 2 * u.pix, np.arange(10) * u.pix), (10,)),
     ((np.arange(10) * u.pix,
       np.arange(10) * u.pix,
       np.arange(10)[..., None] * u.pix), (10, 10)),
     (np.mgrid[0:1024, 0:1000, 0:2] * u.pix, (1024, 1000, 2)),
-))
+])
 def test_varying_transform_pc_shapes(pixel, lon_shape):
     varying_matrix_lt = [rotation_matrix(a)[:2, :2] for a in np.linspace(0, 90, 10)] * u.pix
 
     vct = VaryingCelestialTransform(
         crpix=(5, 5) * u.pix,
         cdelt=(1, 1) * u.arcsec/u.pix,
         crval_table=(0, 0) * u.arcsec,
@@ -263,23 +263,23 @@
     world = vct(*pixel)
     new_pixel = vct.inverse(*world, 0, 0)
 
     assert u.allclose(new_pixel, pixel[:2], atol=0.01)
     assert np.isnan(vct(0, 0, -10, 0)).all()
 
 
-@pytest.mark.parametrize(("pixel", "lon_shape"), (
+@pytest.mark.parametrize(("pixel", "lon_shape"), [
     ((*np.mgrid[0:5, 0:5] * u.pix, np.arange(5) * u.pix, 0 * u.pix), (5, 5)),
     (np.mgrid[0:10, 0:10, 0:5, 0:3] * u.pix, (10, 10, 5, 3)),
     ((2 * u.pix, 2 * u.pix, 0*u.pix, np.arange(3) * u.pix), (3,)),
     ((np.arange(10) * u.pix,
       np.arange(10) * u.pix,
       np.arange(5)[..., None] * u.pix,
       np.arange(3)[..., None, None]), (3, 5, 10)),
-))
+])
 def test_varying_transform_4d_pc_shapes(pixel, lon_shape):
     varying_matrix_lt = [rotation_matrix(a)[:2, :2] for a in np.linspace(0, 90, 15)] * u.pix
     varying_matrix_lt = varying_matrix_lt.reshape((5, 3, 2, 2))
 
     vct = VaryingCelestialTransform2D(
         crpix=(5, 5) * u.pix,
         cdelt=(1, 1) * u.arcsec/u.pix,
@@ -296,19 +296,19 @@
 
 
 def test_vct_dispatch():
     varying_matrix_lt = [rotation_matrix(a)[:2, :2] for a in np.linspace(0, 90, 16)] * u.pix
     varying_matrix_lt = varying_matrix_lt.reshape((2, 2, 2, 2, 2, 2))
     crval_table = list(zip(np.arange(1, 17), np.arange(17, 33))) * u.arcsec
     crval_table = crval_table.reshape((2, 2, 2, 2, 2))
-    kwargs = dict(
-        crpix=(5, 5) * u.pix,
-        cdelt=(1, 1) * u.arcsec/u.pix,
-        lon_pole=180 * u.deg,
-    )
+    kwargs = {
+        "crpix": (5, 5) * u.pix,
+        "cdelt": (1, 1) * u.arcsec/u.pix,
+        "lon_pole": 180 * u.deg,
+    }
 
     vct = varying_celestial_transform_from_tables(
         pc_table=varying_matrix_lt[0, 0, 0],
         crval_table=crval_table[0, 0, 0],
         **kwargs,
     )
     assert isinstance(vct, VaryingCelestialTransform)
@@ -338,27 +338,27 @@
 def test_vct_shape_errors():
     pc_table = [rotation_matrix(a)[:2, :2] for a in np.linspace(0, 90, 15)] * u.pix
     pc_table = pc_table.reshape((5, 3, 2, 2))
 
     crval_table = list(zip(np.arange(1, 16), np.arange(16, 31))) * u.arcsec
     crval_table = crval_table.reshape((5, 3, 2))
 
-    kwargs = dict(
-        crpix=(5, 5) * u.pix,
-        cdelt=(1, 1) * u.arcsec/u.pix,
-        lon_pole=180 * u.deg,
-    )
+    kwargs = {
+        "crpix": (5, 5) * u.pix,
+        "cdelt": (1, 1) * u.arcsec/u.pix,
+        "lon_pole": 180 * u.deg,
+    }
 
-    with pytest.raises(ValueError, match="only be constructed with a one dimensional"):
+    with pytest.raises(ValueError, match="only be constructed with a 1-dimensional"):
         VaryingCelestialTransform(crval_table=crval_table, pc_table=pc_table, **kwargs)
 
-    with pytest.raises(ValueError, match="only be constructed with a two dimensional"):
+    with pytest.raises(ValueError, match="only be constructed with a 2-dimensional"):
         VaryingCelestialTransform2D(crval_table=crval_table[0], pc_table=pc_table[0], **kwargs)
 
-    with pytest.raises(ValueError, match="only be constructed with a three dimensional"):
+    with pytest.raises(ValueError, match="only be constructed with a 3-dimensional"):
         VaryingCelestialTransform3D(crval_table=crval_table[0], pc_table=pc_table[0], **kwargs)
 
 
 @pytest.mark.parametrize("slit", [-1, np.nan, 3, 10])
 def test_vct_slit_bounds(slit):
     crpix=[0, 0]
     cdelt=[1, 1]
@@ -373,15 +373,15 @@
             cdelt=cdelt,
             pc_table=pc_table,
             crval_table=crval_table,
             lon_pole=lon_pole,
             slit=slit,
         )
 
-@pytest.mark.parametrize("num_varying_axes", [pytest.param(1, id='1D'), pytest.param(2, id='2D'), pytest.param(3, id='3D')])
+@pytest.mark.parametrize("num_varying_axes", [pytest.param(1, id="1D"), pytest.param(2, id="2D"), pytest.param(3, id="3D")])
 @pytest.mark.parametrize("slit", [pytest.param(1, id="spectrograph"), pytest.param(None, id="imager")])
 @pytest.mark.parametrize("has_units", [pytest.param(True, id="With Units"), pytest.param(False, id="Without Units")])
 def test_vct(has_units, slit, num_varying_axes):
     if slit:
         num_sensor_axes = 1
         sensor_dims = [5]
     else:
@@ -415,16 +415,16 @@
         for i in range(num_varying_axes):
             varying_axis_pts[i] *= u.pix
         for i in range(num_varying_axes):
             varying_axis_pts_1[i] *= u.pix
         atol *= u.pix
         for i in range(num_sensor_axes):
             sensor_axis_pts[i] *= u.pix
-    grid = np.meshgrid(*sensor_axis_pts, *varying_axis_pts, indexing='ij')
-    grid2 = np.meshgrid(*sensor_axis_pts, *varying_axis_pts_1, indexing='ij')
+    grid = np.meshgrid(*sensor_axis_pts, *varying_axis_pts, indexing="ij")
+    grid2 = np.meshgrid(*sensor_axis_pts, *varying_axis_pts_1, indexing="ij")
     # the portion of the grid due to the varying axes coordinates
     varying_axes_grid = grid[num_sensor_axes:]
 
     vct = varying_celestial_transform_from_tables(
         crpix=crpix,
         cdelt=cdelt,
         pc_table=pc_table,
@@ -444,15 +444,15 @@
     ipixel = vct.inverse(*world, *varying_axes_grid)
     # round trip should be the same as what we started with
     # grid[:num_sensor_axes] is the set of on-sensor coordinates
     assert u.allclose(ipixel, grid[:num_sensor_axes], atol=atol)
 
     # grid2 has coordinates outside the lut boundaries and should have nans
     world2 = vct(*grid2)
-    assert np.any(np.isnan([item for item in world2]))
+    assert np.any(np.isnan(list(world2)))
 
 
 def _evaluate_ravel(array_shape, inputs, order="C"):
     """Evaluate the ravel computation using brute force for comparison with numpy result."""
     # NB: This method does not work with units...
     array_bounds = (array_shape - 1)
     # This if test is to handle multidimensional inputs properly
@@ -460,41 +460,40 @@
         array_bounds = array_bounds[:, np.newaxis]
     rounded_inputs = np.clip(np.rint(inputs).astype(int), None, array_bounds)
     if order == "F":
         array_shape = array_shape[::-1]
         inputs = inputs[::-1]
         rounded_inputs = rounded_inputs[::-1]
     offsets = np.cumprod(array_shape[1:][::-1])[::-1]
-    result = np.dot(offsets, rounded_inputs[:-1]) + inputs[-1]
-    return result
+    return np.dot(offsets, rounded_inputs[:-1]) + inputs[-1]
 
 
 def _evaluate_unravel(array_shape, index, order="C"):
     """Evaluate the reverse ravel computation using brute force for comparison with numpy result."""
     # NB: This method does not work with units...
     if order == "F":
         array_shape = array_shape[::-1]
     offsets = np.cumprod(array_shape[1:][::-1])[::-1]
     curr_offset = index
     # This if test is to handle multidimensional inputs properly
     if isinstance(index, np.ndarray):
-        output_shape = tuple([len(array_shape), len(index)])
+        output_shape = (len(array_shape), len(index))
     else:
         output_shape = len(array_shape)
     indices = np.zeros(output_shape, dtype=float)
     for i, offset in enumerate(offsets):
         indices[i] = np.floor_divide(curr_offset, offset)
         curr_offset = np.remainder(curr_offset, offset)
     indices[-1] = curr_offset
     if order == "F":
         indices = indices[::-1]
     return tuple(indices)
 
 
-@pytest.mark.parametrize("ndim", [pytest.param(2, id='2D'), pytest.param(3, id='3D')])
+@pytest.mark.parametrize("ndim", [pytest.param(2, id="2D"), pytest.param(3, id="3D")])
 @pytest.mark.parametrize("has_units", [pytest.param(True, id="With Units"), pytest.param(False, id="Without Units")])
 @pytest.mark.parametrize("input_type", [pytest.param("array", id="Array Inputs"), pytest.param("scalar", id="Scalar Inputs")])
 def test_ravel_model(ndim, has_units, input_type):
     rng = default_rng()
     array_shape = rng.integers(1, 21, ndim)
     array_bounds = array_shape - 1
     order = "C"
@@ -526,15 +525,15 @@
             assert np.allclose(round_trip, expected_ravel * units)
         else:
             assert np.allclose(ravel_value, expected_ravel)
             assert np.allclose(unraveled_values, expected_unravel)
             assert np.allclose(round_trip, expected_ravel)
 
 
-@pytest.mark.parametrize("ndim", [pytest.param(2, id='2D'), pytest.param(3, id='3D')])
+@pytest.mark.parametrize("ndim", [pytest.param(2, id="2D"), pytest.param(3, id="3D")])
 @pytest.mark.parametrize("has_units", [pytest.param(True, id="With Units"), pytest.param(False, id="Without Units")])
 @pytest.mark.parametrize("input_type", [pytest.param("array", id="Array Inputs"), pytest.param("scalar", id="Scalar Inputs")])
 def test_raveled_tabular1d(ndim, has_units, input_type):
     rng = default_rng()
     array_shape = rng.integers(1, 21, ndim)
     array_bounds = array_shape - 1
     ravel = Ravel(array_shape)
@@ -575,15 +574,15 @@
             assert np.allclose(raveled_tab.inverse.inverse(*inputs), expected_ravel * units)
         else:
             assert np.allclose(raveled_tab(*inputs), expected_ravel)
             assert np.allclose(raveled_tab.inverse(expected_ravel), expected_unravel)
             assert np.allclose(raveled_tab.inverse.inverse(*inputs), expected_ravel)
 
 
-@pytest.mark.parametrize("ndim", [pytest.param(2, id='2D'), pytest.param(3, id='3D')])
+@pytest.mark.parametrize("ndim", [pytest.param(2, id="2D"), pytest.param(3, id="3D")])
 @pytest.mark.parametrize("order", ["C", "F"])
 def test_ravel_ordering(ndim, order):
     rng = default_rng()
     array_shape = rng.integers(2, 21, ndim)
     array_bounds = tuple(np.array(array_shape) - 1)
     ravel = Ravel(array_shape, order=order)
     nelem = np.prod(array_shape)
@@ -591,37 +590,39 @@
     # Make 10 attempts with random numbers
     for _ in range(10):
         inputs = rng.integers(0, array_bounds, len(array_shape))
         ravel_value = ravel(*inputs)
         assert int(ravel_value) == values[tuple(inputs)]
 
 
-@pytest.mark.parametrize("ndim", [pytest.param(2, id='2D'), pytest.param(3, id='3D')])
+@pytest.mark.parametrize("ndim", [pytest.param(2, id="2D"), pytest.param(3, id="3D")])
 @pytest.mark.parametrize("order", ["C", "F"])
 def test_ravel_repr(ndim, order):
     rng = default_rng()
     array_shape = tuple(rng.integers(1, 21, ndim))
     ravel = Ravel(array_shape, order=order)
     unravel = ravel.inverse
-    assert str(array_shape) in repr(ravel) and order in repr(ravel)
-    assert str(array_shape) in repr(unravel) and order in repr(unravel)
+    assert str(array_shape) in repr(ravel)
+    assert order in repr(ravel)
+    assert str(array_shape) in repr(unravel)
+    assert order in repr(unravel)
 
 
 @pytest.mark.parametrize("array_shape", [(0, 1), (1, 0), (1,)])
 @pytest.mark.parametrize("ravel", [Ravel, Unravel])
 def test_ravel_bad_array_shape(array_shape, ravel):
-    with pytest.raises(ValueError) as e:
+    with pytest.raises(ValueError, match="array_shape must be at least 2D and have values >= 1"):
         ravel(array_shape)
 
 
 @pytest.mark.parametrize("order", ["A", "B"])
 @pytest.mark.parametrize("ravel", [Ravel, Unravel])
 def test_ravel_bad_order(order, ravel):
     array_shape=(2, 2, 2)
-    with pytest.raises(ValueError) as e:
+    with pytest.raises(ValueError, match="order kwarg must be one of 'C' or 'F'"):
         ravel(array_shape, order)
 
 
 def test_asymmetric_mapping():
     forward_mapping = [0, 1, 1]
     backward_mapping = [0, 1]
     am = AsymmetricMapping(
```

### Comparing `dkist-1.4.0rc2/dkist.egg-info/PKG-INFO` & `dkist-1.5.0rc1/dkist.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,17 @@
 Metadata-Version: 2.1
 Name: dkist
-Version: 1.4.0rc2
+Version: 1.5.0rc1
 Summary: DKIST User Tools
-Home-page: http://dkist.nso.edu
-Author: NSO / AURA
-Author-email: stuart@cadair.com
-License: BSD 3-Clause
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.9
+Author-email: NSO / AURA <stuart@cadair.com>
+Project-URL: repository, https://github.com/DKISTDC/dkist
+Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE.rst
-Requires-Dist: aiohttp>=3.6
+Requires-Dist: aiohttp>=3.8
 Requires-Dist: asdf>=2.11.2
 Requires-Dist: asdf-astropy>=0.2.0
 Requires-Dist: asdf-coordinates-schemas>=0.1.0
 Requires-Dist: asdf-standard>=1.0.3
 Requires-Dist: asdf-transform-schemas>=0.3.0
 Requires-Dist: asdf-unit-schemas>=0.1.0
 Requires-Dist: asdf-wcs-schemas>=0.3.0
@@ -31,33 +23,38 @@
 Requires-Dist: ndcube[plotting,reproject]>=2.0
 Requires-Dist: numpy>=1.22
 Requires-Dist: parfive[ftp]>=1.5
 Requires-Dist: platformdirs>=3.0
 Requires-Dist: sunpy[asdf,net]>=4.0.7
 Requires-Dist: tqdm>=4.63
 Provides-Extra: tests
-Requires-Dist: pytest-astropy; extra == "tests"
+Requires-Dist: pytest; extra == "tests"
+Requires-Dist: pytest-doctestplus; extra == "tests"
+Requires-Dist: pytest-cov; extra == "tests"
+Requires-Dist: pytest-remotedata; extra == "tests"
 Requires-Dist: pytest-cov; extra == "tests"
 Requires-Dist: pytest-mock; extra == "tests"
 Requires-Dist: pytest-mpl; extra == "tests"
 Requires-Dist: pytest-httpserver; extra == "tests"
 Requires-Dist: hypothesis; extra == "tests"
 Requires-Dist: tox; extra == "tests"
+Requires-Dist: pydot; extra == "tests"
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-astropy; extra == "docs"
 Requires-Dist: sphinx-gallery; extra == "docs"
 Requires-Dist: sphinx-changelog; extra == "docs"
 Requires-Dist: pytest; extra == "docs"
 Requires-Dist: sphinx_autodoc_typehints; extra == "docs"
 Requires-Dist: dkist-sphinx-theme>=1.1.2; extra == "docs"
 Requires-Dist: sphinx-design; extra == "docs"
 Requires-Dist: myst-nb; extra == "docs"
 Requires-Dist: ipywidgets; extra == "docs"
 Requires-Dist: accessible-pygments; extra == "docs"
+Requires-Dist: reproject[all]; extra == "docs"
 
 DKIST User Tools
 ================
 
 .. image:: https://img.shields.io/pypi/v/dkist.svg
    :target: https://pypi.python.org/pypi/dkist/
    :alt: PyPI for dkist package
```

### Comparing `dkist-1.4.0rc2/dkist.egg-info/SOURCES.txt` & `dkist-1.5.0rc1/dkist.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,55 @@
+.codecov.yaml
+.codespell-dict.txt
+.codespellrc
+.coveragerc
+.cruft.json
+.flake8
 .gitignore
 .gitmodules
+.isort.cfg
 .pre-commit-config.yaml
-.readthedocs.yml
+.readthedocs.yaml
+.rtd-environment.yml
+.ruff.toml
 CHANGELOG.rst
 CODE_OF_CONDUCT.md
 CONTRIBUTING.md
 LICENSE.rst
 MANIFEST.in
 README.rst
-codecov.yml
 conftest.py
 pyproject.toml
+pytest.ini
 setup.cfg
 setup.py
 tox.ini
-.github/changelog_filter.py
 .github/ISSUE_TEMPLATE/BUG_REPORT.md
 .github/ISSUE_TEMPLATE/FEATURE_REQUEST.md
 .github/ISSUE_TEMPLATE/config.yml
 .github/workflows/main.yml
 .github/workflows/prepare-release.yml
-changelog/335.trivial.rst
-changelog/336.bugfix.rst
+.github/workflows/sub_package_update.yml
+changelog/309.bugfix.rst
+changelog/344.trivial.rst
+changelog/347.feature.rst
+changelog/349.doc.rst
+changelog/361.bugfix.rst
 changelog/README.rst
 dkist/__init__.py
+dkist/_version.py
 dkist/conftest.py
 dkist/dkist.cfg
 dkist/logger.py
+dkist/version.py
 dkist.egg-info/PKG-INFO
 dkist.egg-info/SOURCES.txt
 dkist.egg-info/dependency_links.txt
 dkist.egg-info/entry_points.txt
+dkist.egg-info/not-zip-safe
 dkist.egg-info/requires.txt
 dkist.egg-info/top_level.txt
 dkist/config/__init__.py
 dkist/data/README.rst
 dkist/data/VISP_HEADER.hdr
 dkist/data/__init__.py
 dkist/data/api_search_values.json
@@ -128,52 +143,55 @@
 dkist/net/attrs_values.py
 dkist/net/client.py
 dkist/net/helpers.py
 dkist/net/globus/__init__.py
 dkist/net/globus/auth.py
 dkist/net/globus/endpoints.py
 dkist/net/globus/transfer.py
+dkist/net/globus/tests/__init__.py
 dkist/net/globus/tests/conftest.py
 dkist/net/globus/tests/test_auth.py
 dkist/net/globus/tests/test_endpoints.py
 dkist/net/globus/tests/test_transfer.py
+dkist/net/tests/__init__.py
 dkist/net/tests/conftest.py
 dkist/net/tests/strategies.py
 dkist/net/tests/test_attr_walker.py
 dkist/net/tests/test_attrs.py
 dkist/net/tests/test_attrs_values.py
 dkist/net/tests/test_client.py
 dkist/net/tests/test_helpers.py
 dkist/tests/__init__.py
-dkist/tests/coveragerc
 dkist/tests/generate_aia_dataset.py
 dkist/tests/generate_eit_test_dataset.py
 dkist/tests/generate_eit_tiled_dataset.py
-dkist/tests/setup_package.py
 dkist/tests/test_logger.py
 dkist/utils/__init__.py
 dkist/utils/_model_to_graphviz.py
 dkist/utils/decorators.py
 dkist/utils/exceptions.py
 dkist/utils/inventory.py
 dkist/utils/sysinfo.py
 dkist/utils/tests/__init__.py
 dkist/utils/tests/test_inventory.py
 dkist/utils/tests/test_sysinfo.py
 dkist/wcs/__init__.py
 dkist/wcs/models.py
+dkist/wcs/tests/__init__.py
 dkist/wcs/tests/test_coupled_compound_model.py
 dkist/wcs/tests/test_models.py
 docs/Makefile
 docs/conf.py
 docs/developer.rst
 docs/index.rst
 docs/installation.rst
 docs/make.bat
 docs/reference.rst
+docs/howto_guides/index.rst
+docs/howto_guides/reproject_vbi_mosaic.md
 docs/logo/icon_square.jpg
 docs/topic_guides/index.rst
 docs/topic_guides/level1data.rst
 docs/topic_guides/loading.rst
 docs/topic_guides/net.rst
 docs/topic_guides/usertools.rst
 docs/tutorial/1_astropy_and_sunpy.md
```

### Comparing `dkist-1.4.0rc2/docs/conf.py` & `dkist-1.5.0rc1/docs/conf.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,113 +1,114 @@
 """
 Configuration file for the Sphinx documentation builder.
 """
 # -- stdlib imports ------------------------------------------------------------
+import datetime
 import os
 import sys
-import datetime
 import warnings
-from pkg_resources import get_distribution
+
 from packaging.version import Version
+from pkg_resources import get_distribution
 
 # -- Check for dependencies ----------------------------------------------------
 doc_requires = get_distribution("dkist").requires(extras=("docs",))
 missing_requirements = []
 for requirement in doc_requires:
     try:
         get_distribution(requirement)
-    except Exception as e:
+    except Exception:
         missing_requirements.append(requirement.name)
 if missing_requirements:
     print(
         f"The {' '.join(missing_requirements)} package(s) could not be found and "
         "is needed to build the documentation, please install the 'docs' requirements."
     )
     sys.exit(1)
 
 # -- Read the Docs Specific Configuration --------------------------------------
 # This needs to be done before sunpy is imported
-on_rtd = os.environ.get('READTHEDOCS', None) == 'True'
+on_rtd = os.environ.get("READTHEDOCS", None) == "True"
 if on_rtd:
-    os.environ['SUNPY_CONFIGDIR'] = '/home/docs/'
-    os.environ['HOME'] = '/home/docs/'
-    os.environ['LANG'] = 'C'
-    os.environ['LC_ALL'] = 'C'
-    os.environ['HIDE_PARFIVE_PROGESS'] = 'True'
+    os.environ["SUNPY_CONFIGDIR"] = "/home/docs/"
+    os.environ["HOME"] = "/home/docs/"
+    os.environ["LANG"] = "C"
+    os.environ["LC_ALL"] = "C"
+    os.environ["HIDE_PARFIVE_PROGESS"] = "True"
 
 # -- Non stdlib imports --------------------------------------------------------
-import dkist  # NOQA
-from dkist import __version__  # NOQA
+import dkist  # noqa
+from dkist import __version__
 
 # -- Project information -------------------------------------------------------
-project = 'DKIST'
-author = 'NSO / AURA'
-copyright = '{}, {}'.format(datetime.datetime.now().year, author)
+project = "DKIST"
+author = "NSO / AURA"
+copyright = f"{datetime.datetime.now().year}, {author}"
 
 # The full version, including alpha/beta/rc tags
 release = __version__
 dkist_version = Version(__version__)
 is_release = not(dkist_version.is_prerelease or dkist_version.is_devrelease)
 
 # We want to ignore all warnings in a release version.
 if is_release:
     warnings.simplefilter("ignore")
 
 # Suppress warnings about overriding directives as we overload some of the
 # doctest extensions.
-suppress_warnings = ['app.add_directive', ]
+suppress_warnings = ["app.add_directive", ]
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
-    'matplotlib.sphinxext.plot_directive',
-    'sphinx_automodapi.automodapi',
-    'sphinx_automodapi.smart_resolver',
-    'sphinx_changelog',
-    'sphinx.ext.autodoc',
-    'sphinx.ext.coverage',
-    'sphinx.ext.doctest',
-    'sphinx.ext.inheritance_diagram',
-    'sphinx.ext.intersphinx',
-    'sphinx.ext.mathjax',
-    'sphinx.ext.napoleon',
-    'sphinx.ext.todo',
-    'sphinx.ext.viewcode',
-    'sphinx_autodoc_typehints',  # must be loaded after napoleon
-    'sunpy.util.sphinx.doctest',
-    'sunpy.util.sphinx.generate',
-    'myst_nb',
-    'sphinx_design',
+    "matplotlib.sphinxext.plot_directive",
+    "sphinx_automodapi.automodapi",
+    "sphinx_automodapi.smart_resolver",
+    "sphinx_changelog",
+    "sphinx.ext.autodoc",
+    "sphinx.ext.coverage",
+    "sphinx.ext.doctest",
+    "sphinx.ext.inheritance_diagram",
+    "sphinx.ext.intersphinx",
+    "sphinx.ext.mathjax",
+    "sphinx.ext.napoleon",
+    "sphinx.ext.todo",
+    "sphinx.ext.viewcode",
+    "sphinx_autodoc_typehints",  # must be loaded after napoleon
+    "sunpy.util.sphinx.doctest",
+    "sunpy.util.sphinx.generate",
+    "myst_nb",
+    "sphinx_design",
 ]
 
 # Add any paths that contain templates here, relative to this directory.
 # templates_path = ['_templates']
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
 
 # Add any extra paths that contain custom files (such as robots.txt or
 # .htaccess) here, relative to this directory. These files are copied
 
-exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store', 'jupyter_execute', '**/*_NOTES.md']
+exclude_patterns = ["_build", "Thumbs.db", ".DS_Store", "jupyter_execute", "**/*_NOTES.md"]
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
-source_suffix = '.rst'
+source_suffix = ".rst"
 
-myst_enable_extensions = ['colon_fence', 'dollarmath', 'substitution']
+myst_enable_extensions = ["colon_fence", "dollarmath", "substitution"]
 
 # The master toctree document.
-master_doc = 'index'
+master_doc = "index"
 
 # The reST default role (used for this markup: `text`) to use for all
 # documents. Set to the "smart" one.
-default_role = 'obj'
+default_role = "obj"
 
 napoleon_use_rtype = False
 
 # Disable google style docstrings
 napoleon_google_docstring = False
 
 # Enable showing inherited members by default
@@ -117,37 +118,26 @@
 typehints_fully_qualified = False
 typehints_use_rtype = napoleon_use_rtype
 typehints_defaults = "comma"
 
 # -- Options for intersphinx extension -----------------------------------------
 # Example configuration for intersphinx: refer to the Python standard library.
 intersphinx_mapping = {
-    "python": (
-        "https://docs.python.org/3/",
-        (None, "http://www.astropy.org/astropy-data/intersphinx/python3.inv"),
-    ),
-    "numpy": (
-        "https://numpy.org/doc/stable/",
-        (None, "http://www.astropy.org/astropy-data/intersphinx/numpy.inv"),
-    ),
-    "scipy": (
-        "https://docs.scipy.org/doc/scipy/",
-        (None, "http://www.astropy.org/astropy-data/intersphinx/scipy.inv"),
-    ),
-    "matplotlib": (
-        "https://matplotlib.org/stable/",
-        (None, "http://www.astropy.org/astropy-data/intersphinx/matplotlib.inv"),
-    ),
+    "python": ("https://docs.python.org/3/", None),
+    "numpy": ("https://numpy.org/doc/stable/", None),
+    "scipy": ("https://docs.scipy.org/doc/scipy/", None),
+    "matplotlib": ("https://matplotlib.org/stable/", None),
     "astropy": ("https://docs.astropy.org/en/stable/", None),
     "parfive": ("https://parfive.readthedocs.io/en/stable/", None),
-    "sunpy": ('https://docs.sunpy.org/en/stable/', None),
-    "ndcube": ('https://docs.sunpy.org/projects/ndcube/en/latest/', None),
-    "gwcs": ('https://gwcs.readthedocs.io/en/latest/', None),
-    "asdf": ('https://asdf.readthedocs.io/en/latest/', None),
-    "dask": ('https://dask.pydata.org/en/latest/', None),
+    "sunpy": ("https://docs.sunpy.org/en/stable/", None),
+    "ndcube": ("https://docs.sunpy.org/projects/ndcube/en/stable/", None),
+    "gwcs": ("https://gwcs.readthedocs.io/en/latest/", None),
+    "asdf": ("https://asdf.readthedocs.io/en/stable/", None),
+    "dask": ("https://dask.pydata.org/en/stable/", None),
+    "reproject": ("https://reproject.readthedocs.io/en/stable/", None),
 }
 
 # -- Options for HTML output ---------------------------------------------------
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 
 from dkist_sphinx_theme.conf.theme import *
@@ -155,27 +145,27 @@
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 # Render inheritance diagrams in SVG
 graphviz_output_format = "svg"
 
 graphviz_dot_args = [
-    '-Nfontsize=10',
-    '-Nfontname=Helvetica Neue, Helvetica, Arial, sans-serif',
-    '-Efontsize=10',
-    '-Efontname=Helvetica Neue, Helvetica, Arial, sans-serif',
-    '-Gfontsize=10',
-    '-Gfontname=Helvetica Neue, Helvetica, Arial, sans-serif'
+    "-Nfontsize=10",
+    "-Nfontname=Helvetica Neue, Helvetica, Arial, sans-serif",
+    "-Efontsize=10",
+    "-Efontname=Helvetica Neue, Helvetica, Arial, sans-serif",
+    "-Gfontsize=10",
+    "-Gfontname=Helvetica Neue, Helvetica, Arial, sans-serif"
 ]
 
 # Use a high-contrast code style from accessible-pygments
 # Our theme isn't using the correct background colours for code blocks, so this
 # isn't as high-contrast as it should be.
 pygments_style = "github-light"
 
 # -- MyST_NB -------------------------------------------------------------------
 nb_execution_allow_errors = False
 nb_execution_in_temp = True
-nb_execution_mode = 'auto'
+nb_execution_mode = "auto"
 nb_execution_timeout = 300
-nb_output_stderr = 'show'
+nb_output_stderr = "show"
 nb_execution_show_tb = True
```

### Comparing `dkist-1.4.0rc2/docs/developer.rst` & `dkist-1.5.0rc1/docs/developer.rst`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/docs/index.rst` & `dkist-1.5.0rc1/docs/index.rst`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 .. toctree::
   :maxdepth: 1
   :hidden:
 
   self
   installation
   tutorial/index
+  howto_guides/index
   topic_guides/index
   reference
   whatsnew/index
   developer
 
 
 .. grid:: 2
@@ -27,14 +28,23 @@
         :link-type: ref
         :text-align: center
 
         :material-outlined:`accessibility_new;8em;sd-text-secondary`
 
         This tutorial walks you through how to search for, download and load DKIST Level one data.
 
+    .. grid-item-card:: How To Guides
+        :link: dkist:howto-guides:index
+        :link-type: ref
+        :text-align: center
+
+        :octicon:`question;8em;sd-text-secondary`
+
+        Walkthroughs on how to achieve a specific task.
+
     .. grid-item-card:: Topic Guides
         :link: dkist:topic-guides:index
         :link-type: ref
         :text-align: center
 
         :material-outlined:`school;8em;sd-text-secondary`
```

### Comparing `dkist-1.4.0rc2/docs/installation.rst` & `dkist-1.5.0rc1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/docs/logo/icon_square.jpg` & `dkist-1.5.0rc1/docs/logo/icon_square.jpg`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/docs/reference.rst` & `dkist-1.5.0rc1/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/docs/topic_guides/level1data.rst` & `dkist-1.5.0rc1/docs/topic_guides/level1data.rst`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/docs/topic_guides/loading.rst` & `dkist-1.5.0rc1/docs/topic_guides/loading.rst`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 Loading and Working with Level One Data
 =======================================
 
 As we saw in the :ref:`dkist:topic-guides:downloading-fits` section, once we have an ASDF file representing a DKIST dataset it can be loaded with `dkist.Dataset`.
 The `dkist.Dataset` class provides access to all the components of the dataset, and is a slightly customised `ndcube.NDCube` object, so all functionality provided by ndcube is applicable to the ``Dataset`` class.
 
-This section of the guide will cover things specifc to the `~dkist.Dataset` class, but will not cover the basics which are in the `ndcube documentation <https://docs.sunpy.org/projects/ndcube>`__.
+This section of the guide will cover things specific to the `~dkist.Dataset` class, but will not cover the basics which are in the `ndcube documentation <https://docs.sunpy.org/projects/ndcube>`__.
 In particular we recommend you read the following sections of the ``ndcube`` documentation:
 
 * :ref:`ndcube:ndcube`
 * :ref:`ndcube:coordinates`
 * :ref:`ndcube:slicing`
 
 before coming back to this guide.
```

### Comparing `dkist-1.4.0rc2/docs/topic_guides/net.rst` & `dkist-1.5.0rc1/docs/topic_guides/net.rst`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 --------------------------------------
 
 .. note::
 
    Download of FITS files is not provided through the ``Fido`` interface.
    As is described below, FITS files can be downloaded for some or all of a dataset after reading the ASDF file.
 
-As is descibed in :ref:`sunpy:sunpy-tutorial-acquiring-data-index`, searches through ``Fido`` use "attrs" which specify the search criteria.
+As is described in :ref:`sunpy:sunpy-tutorial-acquiring-data-index`, searches through ``Fido`` use "attrs" which specify the search criteria.
 A single search can match one or more data providers, for example it is possible to search for DKIST data and data provided by the VSO simultaneously.
 In this guide we will focus on searches only for DKIST data through using the client provided in `dkist.net`.
 
 .. note::
 
    Remember to import `dkist.net` (not just `dkist`) in any script where using Fido, as importing `dkist.net` registers the DKIST client with Fido.
```

### Comparing `dkist-1.4.0rc2/docs/topic_guides/usertools.rst` & `dkist-1.5.0rc1/docs/topic_guides/usertools.rst`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/docs/tutorial/1_astropy_and_sunpy.md` & `dkist-1.5.0rc1/docs/tutorial/1_astropy_and_sunpy.md`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/docs/tutorial/1_astropy_and_sunpy_NOTES.md` & `dkist-1.5.0rc1/docs/tutorial/1_astropy_and_sunpy_NOTES.md`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/docs/tutorial/2_search_and_asdf_download.md` & `dkist-1.5.0rc1/docs/tutorial/2_search_and_asdf_download.md`

 * *Files 2% similar despite different names*

```diff
@@ -45,26 +45,26 @@
 ```
 
 Because we only specified one attr, and it was unique to the dkist client (it started with `a.dkist`) only the DKIST client was used.
 
 If we only want VBI datasets, that are unembargoed, between a specific time range we can use multiple attrs:
 
 ```{code-cell} python
-Fido.search(a.Time("2022-06-02 17:00:00", "2022-06-02 18:00:00") & a.Instrument.vbi & a.dkist.Embargoed(False))
+Fido.search(a.Time("2023/10/16 18:45", "2023/10/16 18:48") & a.Instrument.vbi & a.dkist.Embargoed(False))
 ```
 
 Note how the `a.Time` and `a.Instrument` attrs are not prefixed with `dkist`.
 These are general attrs which can be used to search multiple clients.
 
 So far the returned results have had to match all the attrs provided, because we have used the `&` (logical and) operator to join them.
 If we want results that match either one of multiple options we can use the `|` operator.
-Let's also restrict our search to a particular proposal, `pid_1_123`.
+Let's also restrict our search to a particular proposal, `pid_2_114`.
 
 ```{code-cell} python
-res = Fido.search((a.Instrument.vbi | a.Instrument.visp) & a.dkist.Embargoed(False) & a.dkist.Proposal("pid_1_123"))
+res = Fido.search((a.Instrument.vbi | a.Instrument.visp) & a.dkist.Embargoed(False) & a.dkist.Proposal("pid_2_114"))
 res
 ```
 
 As you can see this has returned two separate tables, one for VBI and one for VISP, even though in fact the VBI table is empty.
 
 ## Working with Results Tables
 
@@ -103,11 +103,11 @@
 ```
 This will download the ASDF file to the sunpy default data directory `~/sunpy/data`, we can customise this with the `path=` keyword argument.
 Note that you can also pass more than one result to be downloaded.
 
 A simple example of both of these is:
 
 ```{code-cell} python
-Fido.fetch(visp[:3], path="~/sunpy/data/{instrument}/{dataset_id}/")
+Fido.fetch(visp[:3], path="~/dkist_data/{instrument}/{dataset_id}/")
 ```
 
 This will put each of our ASDF files in a directory named with the corresponding Dataset ID and Instrument.
```

### Comparing `dkist-1.4.0rc2/docs/tutorial/2_search_and_asdf_download_NOTES.md` & `dkist-1.5.0rc1/docs/tutorial/2_search_and_asdf_download_NOTES.md`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/docs/tutorial/3_the_dataset.md` & `dkist-1.5.0rc1/docs/tutorial/3_the_dataset.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 ---
 jupytext:
   formats: md:myst
   text_representation:
     extension: .md
     format_name: myst
     format_version: 0.13
-    jupytext_version: 1.11.5
+    jupytext_version: 1.16.1
 kernelspec:
-  display_name: Python 3
+  display_name: Python 3 (ipykernel)
   language: python
   name: python3
 ---
 
 (dkist:tutorial:visp-dataset)=
 # Working with a VISP `Dataset`
 
@@ -27,45 +27,43 @@
 This will mean we won't have access to the data arrays in the FITS files, but everything else will function the same.
 
 ## Constructing `Dataset` Objects
 
 We can construct a `Dataset` by providing a path to an ASDF file.
 Here we shall first fetch an ASDF file with Fido and then pass it to `dkist.load_dataset`:
 
-```{code-cell} ipython
----
-tags: [keep-inputs]
----
+```{code-cell} ipython3
+:tags: [keep-inputs]
+
 from astropy.time import Time
 
 import dkist
 import dkist.net
 from sunpy.net import Fido, attrs as a
 ```
 
-```{code-cell} ipython
-# Create DKIST Fido client instance
-res = Fido.search(a.dkist.Dataset('AGLKO')) # This is the dataset selected in the previous tutorial.
-files = Fido.fetch(res)
+```{code-cell} ipython3
+res = Fido.search(a.dkist.Dataset('BKPLX'))
+files = Fido.fetch(res, path="~/dkist_data/{dataset_id}")
 files
 ```
 
 Remember that the file we have downloaded is a single ASDF file, **not** the whole dataset.
 We can use this file to construct the `Dataset`:
 
-```{code-cell} ipython
-ds = dkist.load_dataset(files[0])
+```{code-cell} ipython3
+ds = dkist.load_dataset(files)
 ```
 
 Now we have a `Dataset` object which describes the shape, size and physical dimensions of the array, but doesn't yet contain any of the actual data.
 This may sound unhelpful but we'll see how it can be very powerful.
 
 Let's have a look at the basic representation of the `Dataset`.
 
-```{code-cell} ipython
+```{code-cell} ipython3
 ds
 ```
 
 This gives us a lot of information about the both the *pixel dimensions* of the data (the coordinates of the detector grid) and the *world dimensions* (the physical coordinates of the image).
 Before we go on to using the `Dataset` for inspecting the data, we will take a moment to discuss coordinate systems and consider what the `Dataset` output above means.
 
 ## `Dataset` and `NDCube`: Coordinate aware arrays
@@ -89,96 +87,87 @@
 A key aspect of the `Dataset` is that it is coordinate aware.
 That is, it is able to map between array indices and physical dimensions.
 This means that you can easily convert from a position in the array to a location defined by physical coordinates.
 
 To achieve this, `Dataset` tracks the pixel and world coordinates independently in the `wcs` (World Coordinate System) attribute.
 The output above tells us that we have a 4-dimensional pixel grid and a 5-dimensional world grid:
 
-```{code-cell} python
+```{code-cell} ipython3
 ds.wcs.pixel_n_dim, ds.wcs.world_n_dim
 ```
 
 The next few lines tell us about the data array and the pixel dimensions.
 
-```{code-cell} python
+```{code-cell} ipython3
 ds.data
 ```
 
 This tells us that the data are (or will be) stored in a dask array, and the array dimensions.
 (More on Dask and dask arrays in a later tutorial.)
 
 We can get the corresponding **pixel** axis names with:
 
-```{code-cell} python
+```{code-cell} ipython3
 ds.wcs.pixel_axis_names
 ```
 
-Note that these are in reverse order compared to the `ds` output ealier.
+Note that these are in reverse order compared to the `ds` output earlier.
 This is because they are in *pixel* order rather than *array* order.
 
 Next we see the description of the world coordinates.
-This information is also accessable through the `wcs` attribute:
+This information is also accessible through the `wcs` attribute:
 
-```{code-cell} python
+```{code-cell} ipython3
 ds.wcs.world_axis_names
 ```
 
 This tells us the names of the physical axes, each of which corresponds to a type of phyical observation (lon/lat, time, wavelength, etc.) and has its own units.
 
-```{code-cell} python
+```{code-cell} ipython3
 ds.wcs.world_axis_physical_types, ds.wcs.world_axis_units
 ```
 
 You will have noticed that the pixel and world coordinates have different numbers of dimensions.
 This is because in this dataset the detector is not aligned with the solar latitude/longitude coordinate system, so any change in position along the detector slit will be equivalent to a change in both latitude and longitude.
 To see this, we can look at the physical coordinates which correspond to each array axis, just as we did for the world axes.
 
-```{code-cell} python
+```{code-cell} ipython3
 ds.array_axis_physical_types
 ```
 
 The final piece of output is the axis correlation matrix which summarises which pixel and world axes correspond to each other:
 
-```{code-cell} python
+```{code-cell} ipython3
 ds.wcs.axis_correlation_matrix
 ```
 
 We can use all of this information about the dataset coordinates to convert from pixel to world coordinates or vice versa.
 So if for example we want to plot our data at, say, a particular wavelength, we can find the corresponding array index with `ds.wcs.world_to_array_index()`
 <!-- Actually put a calculation here when the function works -->
 
 ### Slicing Datasets
 
 A useful feature of the `Dataset` class, which it inherits from `NDCube` is the ability to "slice" the dataset and get a smaller dataset, with the array and coordinate information in tact.
 
 For example, to extract the Stokes I component of the dataset we would do:
 
-```{code-cell} python
+```{code-cell} ipython3
 ds[0]
 ```
 
 this is because the stokes axis is the first array axis, and the "I" profile is the first one (0 indexing).
 
 Note how we have dropped a world coordinate, this information is preserved in the `.global_coords` attribute, which contains the coordinate information which applies to the whole dataset:
 
-```{code-cell} python
+```{code-cell} ipython3
 ds[0].global_coords
 ```
 
 We can also slice the data further, as we would for a normal numpy array.
 So for instance we can select a small section of the image in Stokes I at some arbitrary wavelength:
 
-```{code-cell} python
-cropped = ds[0, 400:850, 100, 950:1600]
+```{code-cell} ipython3
+cropped = ds[0, 200:300, 100, 950:1600]
 cropped
 ```
 
 Notice again that this has reduced the dimensionality of the world coordinates as well as of the data itself.
-
-Finally, we can plot our cropped dataset to show the feature we were looking at.
-
-```{code-cell} python
-import matplotlib.pyplot as plt
-
-cropped.plot()
-plt.show()
-```
```

### Comparing `dkist-1.4.0rc2/docs/tutorial/3_the_dataset_NOTES.md` & `dkist-1.5.0rc1/docs/tutorial/3_the_dataset_NOTES.md`

 * *Files 1% similar despite different names*

```diff
@@ -158,15 +158,15 @@
 
 ```{code-cell} ipython
 ds = tds[0, 0]
 ds
 ```
 
 ```{error}
-Due to a known issue with the VBI level 1 FITS headers, the ordering of these tiles in the array are likley incorrect.
+Due to a known issue with the VBI level 1 FITS headers, the ordering of these tiles in the array are likely incorrect.
 ```
 
 The `TiledDataset` stores the FITS headers for all the files of the individual `Dataset`s in the `combined_headers` attribute.
 This means that the metadata can still be inspected in many of the ways we will see in later sessions.
 Later releases of the user tools may also include helper functions for regridding a `TiledDataset` into a single `Dataset` object.
 
 `TiledDataset` also has a `.flat` attribute which let's you iterate over the tiles in order.
```

### Comparing `dkist-1.4.0rc2/docs/tutorial/4_more_dataset.md` & `dkist-1.5.0rc1/docs/tutorial/4_more_dataset.md`

 * *Files 4% similar despite different names*

```diff
@@ -14,17 +14,21 @@
 
 (dkist:tutorial:more-dataset)=
 # More `Dataset`
 
 Firstly we need to re-create our dataset object from the last tutorial.
 
 ```{code-cell} ipython
+from sunpy.net import Fido, attrs as a
 import dkist
+import dkist.net
 
-ds = dkist.load_dataset("~/sunpy/data/VISP/AGLKO")
+res = Fido.search(a.dkist.Dataset('BKPLX'))
+files = Fido.fetch(res, path="~/dkist_data/{dataset_id}")
+ds = dkist.load_dataset(files)
 ```
 
 The `Dataset` object allows us to do some basic inspection of the dataset as a whole without having to download the entire thing, using the metadata in the FITS headers.
 This will save you a good amount of time and also ease the load on the DKIST servers.
 For example, we can check the seeing conditions during the observation and discount any data which will not be of high enough quality to be useful.
 We will go through this as an exercise in a later tutorial.
 
@@ -80,15 +84,15 @@
 
 plt.plot(ds.headers['ATMOS_R0'])
 plt.show()
 ```
 
 ## Tracking files
 
-`Dataset` tracks information about the individual files that make up the datset in the `files` attribute.
+`Dataset` tracks information about the individual files that make up the dataset in the `files` attribute.
 
 ```{code-cell} ipython
 ds.files
 ```
 
 This tells us that our (20, 4096, 4096) data array is stored as 20 files, each containing an array of (4096, 4096).
 Since the filenames are automatically generated from observation metadata, the `files` attribute can also track those before we even download the data.
```

### Comparing `dkist-1.4.0rc2/docs/tutorial/6_visualization.md` & `dkist-1.5.0rc1/docs/tutorial/6_visualization.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 ---
 jupytext:
   formats: md:myst
   text_representation:
     extension: .md
     format_name: myst
     format_version: 0.13
-    jupytext_version: 1.11.5
+    jupytext_version: 1.16.1
 kernelspec:
-  display_name: Python 3
+  display_name: Python 3 (ipykernel)
   language: python
   name: python3
 ---
 
 (dkist:tutorial:visualizing)=
 # Visualizing DKIST Data
 
 In this session we will look at how to take a better look at the actual data once we've downloaded it.
 As usual, first we'll need a dataset.
 We'll use the VISP data we downloaded at the end of the last tutorial.
 
-```{code-cell} python
+```{code-cell} ipython3
 import dkist
 import matplotlib.pyplot as plt
 
 from sunpy.net import Fido, attrs as a
 import dkist.net
 ```
 
-```{code-cell} python
-res = Fido.search(a.dkist.Dataset("AGLKO"))
-asdf_file = Fido.fetch(res)[0]
+```{code-cell} ipython3
+res = Fido.search(a.dkist.Dataset("BKPLX"))
+asdf_file = Fido.fetch(res, path="~/dkist_data/{dataset_id}")
 
 ds = dkist.load_dataset(asdf_file)
 ```
 
 ## Plotting our data
 
 Getting started with plotting a dataset is straightforward.
 `Dataset` provides a `plot()` method which makes a decent default plot of the data.
 
-```{code-cell} python
+```{code-cell} ipython3
 ds.plot()
 plt.show()
 ```
 
 Since our dataset is 4D and most users will only have access to a 2D screen, a slice has to be taken through the data.
 That slice is defined by how the data are ordered and stored in the FITS files.
 In this case, since the FITS files are arrays of the spatial axis vs wavelength, this is the slice that has been plotted for a single polarisation state and scan step.
@@ -55,84 +55,88 @@
 
 Of course, you will probably find you don't always want to slice through the data in the default way.
 In this case, you can use the `plot_axes` argument to `plot()`.
 This takes a list which defines which axes to plot as the slice and which to use as the sliders.
 The list should contain `"x"` and `"y"` in the locations corresponding to the axes we want to plot, and `None` elsewhere.
 The ordering for this is the same as for the pixel dimensions as shown in the `Dataset` summary.
 
-```{code-cell} ipython
+```{code-cell} ipython3
 ds
 ```
 
 So the list needed to specify the default ordering would be `[None, None, 'y', 'x']`.
 If instead we want to plot the image formed by the raster scan at a particular wavelength and Stokes value, we would do this:
 
-```{code-cell} ipython
----
-tags: [skip-execution]
----
++++
+
+```{warning}
+Plotting a raster scan of VISP data is currently very slow due to known performance issues in how varying pointing over the raster is handled. See issue [#256](https://github.com/DKISTDC/dkist/issues/256) for more details.
+```
+
+```{code-cell} ipython3
 ds.plot(plot_axes=[None, 'y', None, 'x'])
 plt.show()
 ```
 
 You may have noticed this plot took somewhat longer to draw than the previous one.
 This is for the same reason as we discussed when talking about reducing the size of dataset downloads: when you slice across the array in a different direction to how it's stored in the files, you have to reference multiple files to create the slice.
 So while the first plot only had to load values from one file at a time, the one above needs to get one line of the array from each of 1000 files in order to draw the slice.
 If you try to animate it, it then needs to do this again at every step.
 
 You can also use `plot_axes` to create a line plot, by specifying only one axis of the data.
 So to plot a spectrum at a fixed Stokes, time and raster location we can tell plot to use the dispersion axis as the x axis.
 
-```{code-cell} ipython
----
-tags: [skip-execution]
----
+```{code-cell} ipython3
 ds.plot(plot_axes=[None, None, 'x', None])
 plt.show()
 ```
 
 It is also possible to slice the data manually and just plot the result.
 This of course creates a new dataset so it will only plot the axes that remain, without sliders or the ability to step through the values of the other axes.
 
-```{code-cell} ipython
+```{code-cell} ipython3
+:tags: [skip-execution]
+
 ds[0, :, 400, :].plot()
 plt.show()
 ```
 
 ## More advanced plotting
 
 For the next few examples we'll go back to using some VBI data.
-Let's use 'AWEMA', which we used in a previous session.
-We haven't actually downloaded the full data for this dataset yet, but the plotting will all still work anyway, and you can download the data later on or in the background if you would like to see the full plots.
 
-```{code-cell} ipython
-res = Fido.search(a.dkist.Dataset("AWEMA"))
-asdf_file = Fido.fetch(res)[0]
+```{code-cell} ipython3
+res = Fido.search(a.dkist.Dataset("AJQWW"))
+asdf_file = Fido.fetch(res, path="~/dkist_data/{dataset_id}")
 
+# We extract the top left tile of the VBI mosaic
 ds = dkist.load_dataset(asdf_file)[0, 0]
 ```
 
 Now let's take a slice of the data and plot it.
 This returns an axes object which we haven't needed before, but this time we'll assign it to a variable so that we can manipulate the plot.
 This allows us to do a number of things with it, such as show the grid of the plot.
 
-```{code-cell} ipython
+```{code-cell} ipython3
 ax = ds[0].plot()
 ax.grid(True)
 ```
 
 What you will probably notice here is that the grid is not aligned with the pixel grid of the image.
 This is because the plot returns a `WCSAxesSubplot`, which is coordinate-aware and automatically uses the world coordinate system for the grid.
 It also supports all the usual ways of manipulating subplots.
 
 Since the `WCSAxesSubplot` is coordinate-aware, we can also use it for plotting coordinates directly, without having to do any manual conversions.
 To do this, we can use the `.plot_coord()` method.
 
-```{code-cell} ipython
+```{code-cell} ipython3
 import astropy.units as u
 from astropy.coordinates import SkyCoord
 
-coord = SkyCoord(-520*u.arcsec, -405*u.arcsec, frame='helioprojective', observer='earth', obstime=ds[0].headers['DATE-AVG'][0])
+coord = SkyCoord(-181*u.arcsec, 112*u.arcsec, frame='helioprojective', observer='earth', obstime=ds.headers['DATE-AVG'][0])
+
+ax = ds[0].plot()
+ax.grid(True)
 # Plot the coordinate as a white circle
 ax.plot_coord(coord, 'wo')
 plt.show()
 ```
```

### Comparing `dkist-1.4.0rc2/docs/tutorial/index.md` & `dkist-1.5.0rc1/docs/tutorial/index.md`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/docs/whatsnew/1.0.rst` & `dkist-1.5.0rc1/docs/whatsnew/1.0.rst`

 * *Files identical despite different names*

### Comparing `dkist-1.4.0rc2/tox.ini` & `dkist-1.5.0rc1/tox.ini`

 * *Files 16% similar despite different names*

```diff
@@ -1,69 +1,87 @@
 [tox]
-envlist = py{39,310,311}{,-devdeps,-oldestdeps,-online},build_docs,codestyle
+min_version = 4.0
 requires =
     setuptools >= 30.3.0
     pip >= 21.0.1
-    #tox-pypi-filter >= 0.12
+    tox-pypi-filter >= 0.14
+envlist =
+    py{310,311,312}
+    py312-devdeps
+    py310-oldestdeps
+    build_docs{,-notebooks}
+    codestyle
 
 [testenv]
-passenv = CC
-setenv =
-    MPLBACKEND = agg
-    COLUMNS = 180
-    PYTEST_COMMAND = pytest {tty:--color=yes} --cov=dkist --cov-config={toxinidir}/setup.cfg --verbose
-    devdeps: PIP_EXTRA_INDEX_URL = https://pypi.anaconda.org/astropy/simple https://pypi.anaconda.org/scipy-wheels-nightly/simple
-extras = tests
-commands =
-    !online: {env:PYTEST_COMMAND} {posargs}
-    online: {env:PYTEST_COMMAND} --remote-data=any {posargs}
+pypi_filter = https://raw.githubusercontent.com/sunpy/sunpy/main/.test_package_pins.txt
+# Run the tests in a temporary directory to make sure that we don't import
+# the package from the source tree
+change_dir = .tmp/{envname}
 description =
     run tests
+    oldestdeps: with the oldest supported version of key dependencies
     devdeps: with the latest developer version of key dependencies
-    oldestdeps: with the oldest supported version of all dependencies
-    online: that require remote data (as well as the offline ones)
+pass_env =
+    # A variable to tell tests we are on a CI system
+    CI
+    # Custom compiler locations (such as ccache)
+    CC
+    # Location of locales (needed by sphinx on some systems)
+    LOCALE_ARCHIVE
+    # If the user has set a LC override we should follow it
+    LC_ALL
+set_env =
+    MPLBACKEND = agg
+    COLUMNS = 180
+    devdeps: PIP_EXTRA_INDEX_URL = https://pypi.anaconda.org/astropy/simple https://pypi.anaconda.org/scientific-python-nightly-wheels/simple
+    # Define the base test command here to allow us to add more flags for each tox factor
+    PYTEST_COMMAND = pytest -vvv -r fEs --pyargs dkist --cov-report=xml --cov=dkist --cov-config={toxinidir}/.coveragerc {toxinidir}/docs
 deps =
-    # Devdeps installs our key dependencies from git to ensure we catch future
-    # breaking changes before they make it to release
+    # For packages which publish nightly wheels this will pull the latest nightly
     devdeps: astropy>=0.0.dev0
     devdeps: numpy>=0.0.dev0
     devdeps: scipy>=0.0.dev0
     devdeps: matplotlib>=0.0.dev0
-    devdeps: git+https://github.com/sunpy/sunpy
+    devdeps: sunpy>=0.0.dev0
     devdeps: git+https://github.com/sunpy/ndcube
     devdeps: git+https://github.com/spacetelescope/gwcs
     devdeps: git+https://github.com/asdf-format/asdf
     devdeps: git+https://github.com/astropy/asdf-astropy
     # Autogenerate oldest dependencies from info in setup.cfg
     oldestdeps: minimum_dependencies
-
-# The oldest deps build runs all our tests against the oldest supported
-# versions
+# The following indicates which extras_require will be installed
+extras =
+    tests
 commands_pre =
     oldestdeps: minimum_dependencies dkist --filename requirements-min.txt
-    # Put the other requirements here to not have pip run more than once
-    #
-    # Very new versions of jsonschema raise warnings, but we don't want to
-    # depend on jsonschema as new asdf (3.0+) does not use it any more.
-    #
-    # The newest cryptography releases break globus
     oldestdeps: pip install -r requirements-min.txt cryptography<42 jsonschema==4.0.1
     pip freeze --all --no-input
-
-[testenv:build_docs]
-changedir = docs
-extras = docs
-description = Invoke sphinx-build to build the HTML docs
 commands =
-    pip freeze --all --no-input
-    # Disable parallel here due to https://github.com/astropy/astropy/issues/14916
-    sphinx-build -j 1 --color -W --keep-going -b html -d _build/.doctrees . _build/html {posargs}
-    python -c 'import pathlib; print("Documentation available under file://\{0\}".format(pathlib.Path(r"{toxinidir}") / "docs" / "_build" / "index.html"))'
+    # To run different commands for different factors exclude the factor from the default command like this
+    # !online: {env:PYTEST_COMMAND} {posargs}
+    # Then specify a specific one like this
+    # online: {env:PYTEST_COMMAND} --remote-data=any {posargs}
+    !online: {env:PYTEST_COMMAND} {posargs}
+    online: {env:PYTEST_COMMAND} --remote-data=any {posargs}
 
 [testenv:codestyle]
+pypi_filter =
 skip_install = true
 description = Run all style and file checks with pre-commit
 deps =
     pre-commit
 commands =
-    pre-commit install --install-hooks
-    pre-commit run --all-files {posargs}
+    pre-commit install-hooks
+    pre-commit run --color always --all-files --show-diff-on-failure
+
+[testenv:build_docs{,-notebooks}]
+description = invoke sphinx-build to build the HTML docs
+change_dir =
+    docs
+extras =
+    docs
+commands =
+    pip freeze --all --no-input
+    # Disable parallel here due to https://github.com/astropy/astropy/issues/14916
+    !notebooks: sphinx-build -j 1 --color -W --keep-going -b html -d _build/.doctrees . _build/html -D nb_execution_mode=off {posargs}
+    notebooks: sphinx-build -j 1 --color -W --keep-going -b html -d _build/.doctrees . _build/html {posargs}
+    python -c 'import pathlib; print("Documentation available under file://\{0\}".format(pathlib.Path(r"{toxinidir}") / "docs" / "_build" / "index.html"))'
```

