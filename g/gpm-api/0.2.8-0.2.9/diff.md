# Comparing `tmp/gpm_api-0.2.8.tar.gz` & `tmp/gpm_api-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpm_api-0.2.8.tar", last modified: Mon Dec  4 10:58:43 2023, max compression
+gzip compressed data, was "gpm_api-0.2.9.tar", last modified: Thu Dec 21 09:38:50 2023, max compression
```

## Comparing `gpm_api-0.2.8.tar` & `gpm_api-0.2.9.tar`

### file list

```diff
@@ -1,188 +1,193 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 10:58:43.977179 gpm_api-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)      257 2023-12-04 10:58:34.000000 gpm_api-0.2.8/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2023-12-04 10:58:34.000000 gpm_api-0.2.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      111 2023-12-04 10:58:34.000000 gpm_api-0.2.8/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (127)      711 2023-12-04 10:58:34.000000 gpm_api-0.2.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      783 2023-12-04 10:58:34.000000 gpm_api-0.2.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      390 2023-12-04 10:58:34.000000 gpm_api-0.2.8/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)      262 2023-12-04 10:58:34.000000 gpm_api-0.2.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)      376 2023-12-04 10:58:34.000000 gpm_api-0.2.8/CITATION.bib
--rw-r--r--   0 runner    (1001) docker     (127)      373 2023-12-04 10:58:34.000000 gpm_api-0.2.8/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)    19844 2023-12-04 10:58:34.000000 gpm_api-0.2.8/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2023-12-04 10:58:34.000000 gpm_api-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       51 2023-12-04 10:58:34.000000 gpm_api-0.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    13546 2023-12-04 10:58:43.977179 gpm_api-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9362 2023-12-04 10:58:34.000000 gpm_api-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 10:58:43.949179 gpm_api-0.2.8/ci/
--rw-r--r--   0 runner    (1001) docker     (127)      320 2023-12-04 10:58:34.000000 gpm_api-0.2.8/ci/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)      312 2023-12-04 10:58:34.000000 gpm_api-0.2.8/ci/environment_latest.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 10:58:43.949179 gpm_api-0.2.8/gpm_api/
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-12-04 10:58:43.000000 gpm_api-0.2.8/gpm_api/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 10:58:43.953179 gpm_api-0.2.8/gpm_api/accessor/
--rw-r--r--   0 runner    (1001) docker     (127)      212 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/accessor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20840 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/accessor/methods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 10:58:43.953179 gpm_api-0.2.8/gpm_api/bucket/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/bucket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3970 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/bucket/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2928 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/bucket/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2637 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/bucket/io.py
--rw-r--r--   0 runner    (1001) docker     (127)    14352 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/bucket/processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3451 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/bucket/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/bucket/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16268 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/bucket/writers.py
--rw-r--r--   0 runner    (1001) docker     (127)    10560 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6449 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/configs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 10:58:43.957179 gpm_api-0.2.8/gpm_api/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)     4759 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/dataset/attrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6625 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/dataset/conventions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5124 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/dataset/coords.py
--rw-r--r--   0 runner    (1001) docker     (127)    25761 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/dataset/crs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10112 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3274 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/dataset/datatree.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 10:58:43.957179 gpm_api-0.2.8/gpm_api/dataset/decoding/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/dataset/decoding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/dataset/decoding/cf.py
--rw-r--r--   0 runner    (1001) docker     (127)     7688 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/dataset/decoding/coordinates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2923 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/dataset/decoding/dataarray_attrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/dataset/decoding/decode_2a_pmw.py
--rw-r--r--   0 runner    (1001) docker     (127)     9058 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/dataset/decoding/decode_2a_radar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/dataset/decoding/routines.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/dataset/decoding/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5770 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/dataset/dimensions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9434 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/dataset/granule.py
--rw-r--r--   0 runner    (1001) docker     (127)     6711 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/dataset/groups_variables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 10:58:43.957179 gpm_api-0.2.8/gpm_api/encoding/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/encoding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5062 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/encoding/encode_2a_radar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2348 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/encoding/routines.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 10:58:43.957179 gpm_api-0.2.8/gpm_api/etc/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/etc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2269 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/etc/country_acronyms.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    12467 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/etc/country_bounds.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    12467 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/etc/country_extent.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/etc/pmw_frequency.yml
--rw-r--r--   0 runner    (1001) docker     (127)    30602 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/etc/product_def.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 10:58:43.961179 gpm_api-0.2.8/gpm_api/io/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10110 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/io/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3484 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/io/data_integrity.py
--rw-r--r--   0 runner    (1001) docker     (127)    33674 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/io/download.py
--rw-r--r--   0 runner    (1001) docker     (127)    10453 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/io/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10937 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/io/find.py
--rw-r--r--   0 runner    (1001) docker     (127)     8221 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/io/ges_disc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6646 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/io/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     8395 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/io/local.py
--rw-r--r--   0 runner    (1001) docker     (127)    12144 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/io/pps.py
--rw-r--r--   0 runner    (1001) docker     (127)     7792 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/io/products.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 10:58:43.961179 gpm_api-0.2.8/gpm_api/retrievals/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/retrievals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/retrievals/retrieval_2a_pmw.py
--rw-r--r--   0 runner    (1001) docker     (127)    18213 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/retrievals/retrieval_2a_radar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/retrievals/routines.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 10:58:43.961179 gpm_api-0.2.8/gpm_api/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/scripts/download_gpm_daily_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/scripts/download_gpm_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/scripts/download_gpm_monthly_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 10:58:43.961179 gpm_api-0.2.8/gpm_api/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 10:58:43.945179 gpm_api-0.2.8/gpm_api/tests/0_tmp/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 10:58:43.965179 gpm_api-0.2.8/gpm_api/tests/0_tmp/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)     6358 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/tests/0_tmp/dataset/0_create_test_files.py
--rw-r--r--   0 runner    (1001) docker     (127)    11507 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/tests/0_tmp/dataset/dev_encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/tests/0_tmp/dataset/test_attrs_decoding.py
--rw-r--r--   0 runner    (1001) docker     (127)     3201 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/tests/0_tmp/dataset/test_crs_cf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/tests/0_tmp/dataset/test_dataset_concatenation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2542 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/tests/0_tmp/dataset/test_dataset_regularity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/tests/0_tmp/dataset/test_dataset_valid_geolocation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4859 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/tests/0_tmp/dataset/test_decode_2a_dpr.py
--rw-r--r--   0 runner    (1001) docker     (127)     4582 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/tests/0_tmp/dataset/test_granule_creation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3646 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/tests/0_tmp/dataset/test_parallel_reading.py
--rw-r--r--   0 runner    (1001) docker     (127)     3203 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/tests/0_tmp/dataset/test_pmw_channel_coords.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/tests/0_tmp/dataset/test_retrievals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/tests/0_tmp/dataset/test_unvalid_coordinates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 10:58:43.965179 gpm_api-0.2.8/gpm_api/tests/0_tmp/io/
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/tests/0_tmp/io/test_archive.py
--rw-r--r--   0 runner    (1001) docker     (127)     6108 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/tests/0_tmp/io/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      889 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/tests/0_tmp/io/test_disk.py
--rw-r--r--   0 runner    (1001) docker     (127)     6806 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/tests/0_tmp/io/test_download.py
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/tests/0_tmp/io/test_downloads.py
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/tests/0_tmp/io/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/tests/0_tmp/io/test_find_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/tests/0_tmp/io/test_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/tests/0_tmp/io/test_pps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 10:58:43.965179 gpm_api-0.2.8/gpm_api/tests/0_tmp/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)     2660 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/tests/0_tmp/visualization/test_plot_multiorbit_gmi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/tests/0_tmp/visualization/test_plot_multiorbit_pmw_polar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/tests/0_tmp/visualization/test_plot_orbit_pmw_custom_kwargs.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12145 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 10:58:43.969179 gpm_api-0.2.8/gpm_api/tests/test_dataset/
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/tests/test_dataset/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 10:58:43.969179 gpm_api-0.2.8/gpm_api/tests/test_dataset/decoding/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/tests/test_dataset/decoding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/tests/test_dataset/decoding/test_attrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/tests/test_dataset/decoding/test_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (127)     4541 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/tests/test_dataset/test_attrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5937 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/tests/test_dataset/test_coords.py
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/tests/test_dataset/test_crs.py
--rw-r--r--   0 runner    (1001) docker     (127)      477 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/tests/test_dataset/test_datatree.py
--rw-r--r--   0 runner    (1001) docker     (127)     6319 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/tests/test_dataset/test_dimensions.py
--rw-r--r--   0 runner    (1001) docker     (127)    15256 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/tests/test_dataset/test_granule.py
--rw-r--r--   0 runner    (1001) docker     (127)     3103 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/tests/test_dataset/test_granule_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     4616 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/tests/test_dataset/test_groups_variables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 10:58:43.969179 gpm_api-0.2.8/gpm_api/tests/test_io/
--rw-r--r--   0 runner    (1001) docker     (127)     3275 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/tests/test_io/test_data_integrity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3482 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/tests/test_io/test_disk.py
--rw-r--r--   0 runner    (1001) docker     (127)    13827 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/tests/test_io/test_download.py
--rw-r--r--   0 runner    (1001) docker     (127)     9855 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/tests/test_io/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    19540 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/tests/test_io/test_find.py
--rw-r--r--   0 runner    (1001) docker     (127)     3430 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/tests/test_io/test_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    20922 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/tests/test_io/test_io_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/tests/test_io/test_local.py
--rw-r--r--   0 runner    (1001) docker     (127)      933 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/tests/test_io/test_pps.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/tests/test_io/test_products.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 10:58:43.969179 gpm_api-0.2.8/gpm_api/tests/test_utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/tests/test_utils/test_geospatial.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/tests/test_utils/test_list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 10:58:43.969179 gpm_api-0.2.8/gpm_api/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6158 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/tests/utils/hdf5.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 10:58:43.973179 gpm_api-0.2.8/gpm_api/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9289 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/utils/archive.py
--rw-r--r--   0 runner    (1001) docker     (127)     7587 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/utils/area.py
--rw-r--r--   0 runner    (1001) docker     (127)    35506 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3075 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/utils/collocation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/utils/continents.py
--rw-r--r--   0 runner    (1001) docker     (127)     2672 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/utils/countries.py
--rw-r--r--   0 runner    (1001) docker     (127)      491 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/utils/dask.py
--rw-r--r--   0 runner    (1001) docker     (127)    10532 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/utils/geospatial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/utils/list.py
--rw-r--r--   0 runner    (1001) docker     (127)    13347 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/utils/manipulations.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/utils/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)    22547 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/utils/slices.py
--rw-r--r--   0 runner    (1001) docker     (127)     7184 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/utils/time.py
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/utils/timing.py
--rw-r--r--   0 runner    (1001) docker     (127)    31033 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/utils/utils_cmap.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/utils/warnings.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/utils/xarray.py
--rw-r--r--   0 runner    (1001) docker     (127)      529 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/utils/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 10:58:43.973179 gpm_api-0.2.8/gpm_api/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)      320 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7518 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/visualization/grid.py
--rw-r--r--   0 runner    (1001) docker     (127)    12803 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/visualization/orbit.py
--rw-r--r--   0 runner    (1001) docker     (127)    26263 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/visualization/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     7814 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/visualization/plot_3d.py
--rw-r--r--   0 runner    (1001) docker     (127)    11915 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/visualization/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4138 2023-12-04 10:58:35.000000 gpm_api-0.2.8/gpm_api/visualization/title.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 10:58:43.977179 gpm_api-0.2.8/gpm_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13546 2023-12-04 10:58:43.000000 gpm_api-0.2.8/gpm_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5179 2023-12-04 10:58:43.000000 gpm_api-0.2.8/gpm_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-04 10:58:43.000000 gpm_api-0.2.8/gpm_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      279 2023-12-04 10:58:43.000000 gpm_api-0.2.8/gpm_api.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      356 2023-12-04 10:58:43.000000 gpm_api-0.2.8/gpm_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-12-04 10:58:43.000000 gpm_api-0.2.8/gpm_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4363 2023-12-04 10:58:35.000000 gpm_api-0.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-04 10:58:43.977179 gpm_api-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-04 10:58:35.000000 gpm_api-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 09:38:50.665635 gpm_api-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2023-12-21 09:38:38.000000 gpm_api-0.2.9/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2023-12-21 09:38:38.000000 gpm_api-0.2.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2023-12-21 09:38:38.000000 gpm_api-0.2.9/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2023-12-21 09:38:38.000000 gpm_api-0.2.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2023-12-21 09:38:38.000000 gpm_api-0.2.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2023-12-21 09:38:38.000000 gpm_api-0.2.9/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2023-12-21 09:38:38.000000 gpm_api-0.2.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2023-12-21 09:38:38.000000 gpm_api-0.2.9/CITATION.bib
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2023-12-21 09:38:38.000000 gpm_api-0.2.9/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)    19844 2023-12-21 09:38:38.000000 gpm_api-0.2.9/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2023-12-21 09:38:38.000000 gpm_api-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2023-12-21 09:38:38.000000 gpm_api-0.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    18177 2023-12-21 09:38:50.665635 gpm_api-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13934 2023-12-21 09:38:38.000000 gpm_api-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 09:38:50.637635 gpm_api-0.2.9/ci/
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2023-12-21 09:38:38.000000 gpm_api-0.2.9/ci/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2023-12-21 09:38:38.000000 gpm_api-0.2.9/ci/environment_latest.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 09:38:50.637635 gpm_api-0.2.9/gpm_api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2023-12-21 09:38:50.000000 gpm_api-0.2.9/gpm_api/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 09:38:50.641635 gpm_api-0.2.9/gpm_api/accessor/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/accessor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20995 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/accessor/methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 09:38:50.641635 gpm_api-0.2.9/gpm_api/bucket/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/bucket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3970 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/bucket/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2928 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/bucket/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/bucket/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14352 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/bucket/processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3451 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/bucket/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/bucket/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16268 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/bucket/writers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10560 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6449 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/configs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 09:38:50.641635 gpm_api-0.2.9/gpm_api/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)     4759 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/dataset/attrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6625 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/dataset/conventions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5124 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/dataset/coords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25761 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/dataset/crs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10145 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3274 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/dataset/datatree.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 09:38:50.645635 gpm_api-0.2.9/gpm_api/dataset/decoding/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/dataset/decoding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/dataset/decoding/cf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7688 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/dataset/decoding/coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2923 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/dataset/decoding/dataarray_attrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/dataset/decoding/decode_2a_pmw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9058 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/dataset/decoding/decode_2a_radar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/dataset/decoding/routines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/dataset/decoding/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5770 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/dataset/dimensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9434 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/dataset/granule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6711 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/dataset/groups_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 09:38:50.645635 gpm_api-0.2.9/gpm_api/encoding/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/encoding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5062 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/encoding/encode_2a_radar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/encoding/routines.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 09:38:50.645635 gpm_api-0.2.9/gpm_api/etc/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/etc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/etc/continent_extent.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/etc/country_acronyms.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    12467 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/etc/country_bounds.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    12467 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/etc/country_extent.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/etc/pmw_frequency.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    38040 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/etc/product_def.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 09:38:50.649635 gpm_api-0.2.9/gpm_api/io/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14463 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/io/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/io/data_integrity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33747 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/io/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10256 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/io/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10906 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/io/find.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8221 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/io/ges_disc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6646 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/io/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8395 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/io/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12171 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/io/pps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15327 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/io/products.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 09:38:50.649635 gpm_api-0.2.9/gpm_api/retrievals/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/retrievals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/retrievals/retrieval_2a_pmw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18213 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/retrievals/retrieval_2a_radar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/retrievals/routines.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 09:38:50.649635 gpm_api-0.2.9/gpm_api/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/scripts/download_gpm_daily_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/scripts/download_gpm_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/scripts/download_gpm_monthly_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 09:38:50.649635 gpm_api-0.2.9/gpm_api/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 09:38:50.633635 gpm_api-0.2.9/gpm_api/tests/0_tmp/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 09:38:50.649635 gpm_api-0.2.9/gpm_api/tests/0_tmp/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)     6358 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/tests/0_tmp/dataset/0_create_test_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11507 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/tests/0_tmp/dataset/dev_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/tests/0_tmp/dataset/test_attrs_decoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3201 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/tests/0_tmp/dataset/test_crs_cf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/tests/0_tmp/dataset/test_dataset_concatenation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2542 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/tests/0_tmp/dataset/test_dataset_regularity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/tests/0_tmp/dataset/test_dataset_valid_geolocation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4859 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/tests/0_tmp/dataset/test_decode_2a_dpr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4582 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/tests/0_tmp/dataset/test_granule_creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3646 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/tests/0_tmp/dataset/test_parallel_reading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/tests/0_tmp/dataset/test_pmw_channel_coords.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/tests/0_tmp/dataset/test_retrievals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/tests/0_tmp/dataset/test_unvalid_coordinates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 09:38:50.653635 gpm_api-0.2.9/gpm_api/tests/0_tmp/io/
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/tests/0_tmp/io/test_archive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6116 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/tests/0_tmp/io/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/tests/0_tmp/io/test_disk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6806 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/tests/0_tmp/io/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/tests/0_tmp/io/test_downloads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/tests/0_tmp/io/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/tests/0_tmp/io/test_find_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/tests/0_tmp/io/test_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/tests/0_tmp/io/test_pps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 09:38:50.653635 gpm_api-0.2.9/gpm_api/tests/0_tmp/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)     2660 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/tests/0_tmp/visualization/test_plot_multiorbit_gmi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/tests/0_tmp/visualization/test_plot_multiorbit_pmw_polar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/tests/0_tmp/visualization/test_plot_orbit_pmw_custom_kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13371 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 09:38:50.653635 gpm_api-0.2.9/gpm_api/tests/test_accessor/
+-rw-r--r--   0 runner    (1001) docker     (127)     7620 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/tests/test_accessor/test_accessor_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 09:38:50.653635 gpm_api-0.2.9/gpm_api/tests/test_dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/tests/test_dataset/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 09:38:50.653635 gpm_api-0.2.9/gpm_api/tests/test_dataset/decoding/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/tests/test_dataset/decoding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/tests/test_dataset/decoding/test_attrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/tests/test_dataset/decoding/test_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4541 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/tests/test_dataset/test_attrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5937 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/tests/test_dataset/test_coords.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/tests/test_dataset/test_crs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/tests/test_dataset/test_datatree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6319 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/tests/test_dataset/test_dimensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15256 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/tests/test_dataset/test_granule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3103 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/tests/test_dataset/test_granule_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4616 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/tests/test_dataset/test_groups_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 09:38:50.657635 gpm_api-0.2.9/gpm_api/tests/test_io/
+-rw-r--r--   0 runner    (1001) docker     (127)     3275 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/tests/test_io/test_data_integrity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3484 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/tests/test_io/test_disk.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13829 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/tests/test_io/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9684 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/tests/test_io/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19587 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/tests/test_io/test_find.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/tests/test_io/test_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21115 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/tests/test_io/test_io_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/tests/test_io/test_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/tests/test_io/test_pps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/tests/test_io/test_products.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 09:38:50.657635 gpm_api-0.2.9/gpm_api/tests/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)    10541 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/tests/test_utils/test_geospatial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/tests/test_utils/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15209 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/tests/test_utils/test_slices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9632 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/tests/test_utils/test_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23957 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/tests/test_utils/test_utils_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/tests/test_utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 09:38:50.657635 gpm_api-0.2.9/gpm_api/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6158 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/tests/utils/hdf5.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 09:38:50.661635 gpm_api-0.2.9/gpm_api/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9289 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/utils/archive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7587 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/utils/area.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35665 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3080 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/utils/collocation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/utils/dask.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14050 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/utils/geospatial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/utils/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13347 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/utils/manipulations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/utils/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24131 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/utils/slices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7560 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/utils/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/utils/timing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31033 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/utils/utils_cmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/utils/warnings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/utils/xarray.py
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/utils/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 09:38:50.661635 gpm_api-0.2.9/gpm_api/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7518 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/visualization/grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12803 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/visualization/orbit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26263 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/visualization/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7814 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/visualization/plot_3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11914 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/visualization/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4138 2023-12-21 09:38:38.000000 gpm_api-0.2.9/gpm_api/visualization/title.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 09:38:50.661635 gpm_api-0.2.9/gpm_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18177 2023-12-21 09:38:50.000000 gpm_api-0.2.9/gpm_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5369 2023-12-21 09:38:50.000000 gpm_api-0.2.9/gpm_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-21 09:38:50.000000 gpm_api-0.2.9/gpm_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2023-12-21 09:38:50.000000 gpm_api-0.2.9/gpm_api.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2023-12-21 09:38:50.000000 gpm_api-0.2.9/gpm_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2023-12-21 09:38:50.000000 gpm_api-0.2.9/gpm_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4412 2023-12-21 09:38:38.000000 gpm_api-0.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-21 09:38:50.665635 gpm_api-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-21 09:38:38.000000 gpm_api-0.2.9/setup.py
```

### Comparing `gpm_api-0.2.8/.gitignore` & `gpm_api-0.2.9/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 *~
 .DS_Store
 .vscode
 .Rhistory
 
 # Folders
 /dask-worker-space/
-gpm_api/tests/dataset/test_granule_data
 
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 gpm_api/__pycache__/
 gpm_api/utils/__pycache__/
@@ -62,14 +61,15 @@
 nosetests.xml
 coverage.xml
 *.cover
 *.py,cover
 .hypothesis/
 .pytest_cache/
 cover/
+lcov.info
 
 # Translations
 *.mo
 *.pot
 
 # Django stuff:
 *.log
```

### Comparing `gpm_api-0.2.8/.pre-commit-config.yaml` & `gpm_api-0.2.9/.pre-commit-config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -2,27 +2,27 @@
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.5.0
     hooks:
       - id: trailing-whitespace
       - id: end-of-file-fixer
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.1.0
+    rev: v0.1.8
     hooks:
       - id: ruff
         args: [--fix]
 
   - repo: https://github.com/psf/black
-    rev: 23.9.1
+    rev: 23.12.0
     hooks:
     - id: black
       language_version: python3
 
   - repo: https://github.com/keewis/blackdoc
-    rev: v0.3.8
+    rev: v0.3.9
     hooks:
     - id: blackdoc
       additional_dependencies: ["black[jupyter]"]
 
   - repo: https://github.com/codespell-project/codespell
     rev: v2.2.6
     hooks:
```

### Comparing `gpm_api-0.2.8/.readthedocs.yaml` & `gpm_api-0.2.9/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/CONTRIBUTING.rst` & `gpm_api-0.2.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/LICENSE` & `gpm_api-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/PKG-INFO` & `gpm_api-0.2.9/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpm_api
-Version: 0.2.8
+Version: 0.2.9
 Summary: Python API for the Global Precipitation Mission Data Archive
 Author-email: Gionata Ghiggi <gionata.ghiggi@epfl.ch>
 License: MIT License
         
         Copyright (c) 2023 Gionata Ghiggi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -21,18 +21,19 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: Homepage, https://github.com/ghiggi/gpm_api
-Project-URL: Source, https://github.com/ghiggi/gpm_api
-Project-URL: Tracker, https://github.com/ghiggi/gpm_api/issues
-Project-URL: Documentation, https://gpm_api.readthedocs.io
+Project-URL: homepage, https://github.com/ghiggi/gpm_api
+Project-URL: repository, https://github.com/ghiggi/gpm_api
+Project-URL: source, https://github.com/ghiggi/gpm_api
+Project-URL: tracker, https://github.com/ghiggi/gpm_api/issues
+Project-URL: documentation, https://gpm_api.readthedocs.io
 Project-URL: changelog, https://github.com/ghigg/gpm_api/CHANGELOG.md
 Keywords: GPM,Precipitation,API,DPR,PMW,IMERG
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
@@ -89,37 +90,47 @@
 Requires-Dist: wheel; extra == "dev"
 Requires-Dist: sphinx; extra == "dev"
 Requires-Dist: sphinx-gallery; extra == "dev"
 Requires-Dist: sphinx-book-theme; extra == "dev"
 Requires-Dist: nbsphinx; extra == "dev"
 Requires-Dist: sphinx_mdinclude; extra == "dev"
 
-# Welcome to GPM-API
-[![DOI](https://zenodo.org/badge/286664485.svg)](https://zenodo.org/badge/latestdoi/286664485)
-[![PyPI version](https://badge.fury.io/py/gpm_api.svg)](https://badge.fury.io/py/gpm_api)
-[![Conda Version](https://img.shields.io/conda/vn/conda-forge/gpm_api.svg)](https://anaconda.org/conda-forge/gpm_api)
-[![Tests](https://github.com/ghiggi/gpm_api/actions/workflows/tests.yml/badge.svg)](https://github.com/ghiggi/gpm_api/actions/workflows/tests.yml)
-[![Coverage Status](https://coveralls.io/repos/github/ghiggi/gpm_api/badge.svg?branch=main)](https://coveralls.io/github/ghiggi/gpm_api?branch=main)
-[![Documentation Status](https://readthedocs.org/projects/gpm-api/badge/?version=latest)](https://gpm-api.readthedocs.io/en/latest/?badge=latest)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
-[![License](https://img.shields.io/github/license/ghiggi/gpm_api)](https://github.com/ghiggi/gpm_api/blob/master/LICENSE)
+# 📦 Welcome to GPM-API
+
+|                      |                                                |
+| -------------------- | ---------------------------------------------- |
+| Deployment           | [![PyPI](https://badge.fury.io/py/gpm_api.svg?style=flat)](https://pypi.org/project/gpm_api/) [![Conda](https://img.shields.io/conda/vn/conda-forge/gpm_api.svg?logo=conda-forge&logoColor=white&style=flat)](https://anaconda.org/conda-forge/gpm_api) |
+| Activity             | [![PyPI Downloads](https://img.shields.io/pypi/dm/gpm_api.svg?label=PyPI%20downloads&style=flat)](https://pypi.org/project/gpm_api/) [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/gpm_api.svg?label=Conda%20downloads&style=flat)](https://anaconda.org/conda-forge/gpm_api) |
+| Python Versions      | [![Python Versions](https://img.shields.io/badge/Python-3.8%20%203.9%20%203.10%20%203.11%20%203.12-blue?style=flat)](https://www.python.org/downloads/) |
+| Supported Systems    | [![Linux](https://img.shields.io/github/actions/workflow/status/ghiggi/gpm_api/.github/workflows/tests.yml?label=Linux&style=flat)](https://github.com/ghiggi/gpm_api/actions/workflows/tests.yml) [![macOS](https://img.shields.io/github/actions/workflow/status/ghiggi/gpm_api/.github/workflows/tests.yml?label=macOS&style=flat)](https://github.com/ghiggi/gpm_api/actions/workflows/tests.yml) [![Windows](https://img.shields.io/github/actions/workflow/status/ghiggi/gpm_api/.github/workflows/tests_windows.yml?label=Windows&style=flat)](https://github.com/ghiggi/gpm_api/actions/workflows/tests_windows.yml) |
+| Project Status       | [![Project Status](https://www.repostatus.org/badges/latest/active.svg?style=flat)](https://www.repostatus.org/#active) |
+| Build Status         | [![Tests](https://github.com/ghiggi/gpm_api/actions/workflows/tests.yml/badge.svg?style=flat)](https://github.com/ghiggi/gpm_api/actions/workflows/tests.yml) [![Lint](https://github.com/ghiggi/gpm_api/actions/workflows/lint.yml/badge.svg?style=flat)](https://github.com/ghiggi/gpm_api/actions/workflows/lint.yml) [![Docs](https://readthedocs.org/projects/gpm_api/badge/?version=latest&style=flat)](https://gpm_api.readthedocs.io/en/latest/) |
+| Linting              | [![Black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat)](https://github.com/psf/black) [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json&style=flat)](https://github.com/astral-sh/ruff) [![Codespell](https://img.shields.io/badge/Codespell-enabled-brightgreen?style=flat)](https://github.com/codespell-project/codespell) |
+| Code Coverage        | [![Coveralls](https://coveralls.io/repos/github/ghiggi/gpm_api/badge.svg?branch=main&style=flat)](https://coveralls.io/github/ghiggi/gpm_api?branch=main) [![Codecov](https://codecov.io/gh/ghiggi/gpm_api/branch/main/graph/badge.svg?style=flat)](https://codecov.io/gh/ghiggi/gpm_api) |
+| Code Quality         | [![Codefactor](https://www.codefactor.io/repository/github/ghiggi/gpm_api/badge?style=flat)](https://www.codefactor.io/repository/github/ghiggi/gpm_api) [![Codebeat](https://codebeat.co/badges/236abcf2-cbae-4ca9-8a2d-3b70495bb16b?style=flat)](https://codebeat.co/projects/github-com-ghiggi-gpm_api-main) [![Codacy](https://app.codacy.com/project/badge/Grade/bee842cb10004ad8bb9288256f2fc8af?style=flat)](https://app.codacy.com/gh/ghiggi/gpm_api/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade) [![Codescene](https://codescene.io/projects/36767/status-badges/code-health?style=flat)](https://codescene.io/projects/36767) |
+| Code Review          | [![pyOpenSci](https://tinyurl.com/XXXX)](#) [![OpenSSF Best Practices](https://www.bestpractices.dev/projects/XXXX/badge?style=flat)](#) |
+| License              | [![License](https://img.shields.io/github/license/ghiggi/gpm_api?style=flat)](https://github.com/ghiggi/gpm_api/blob/main/LICENSE) |
+| Community            | [![Slack](https://img.shields.io/badge/Slack-gpm_api-green.svg?logo=slack&style=flat)](https://join.slack.com/t/gpmapi/shared_invite/zt-28vkxzjs1-~cIYci2o3G0qEEoQJVMQRg) [![GitHub Discussions](https://img.shields.io/badge/GitHub-Discussions-green?logo=github&style=flat)](https://github.com/ghiggi/gpm_api/discussions) |
+| Citation             | [![DOI](https://zenodo.org/badge/286664485.svg?style=flat)](https://doi.org/10.5281/zenodo.10255084) |
+
+ [**Slack**](https://join.slack.com/t/gpmapi/shared_invite/zt-28vkxzjs1-~cIYci2o3G0qEEoQJVMQRg) | [**Docs**](https://gpm-api.readthedocs.io/en/latest/)
 
 The GPM-API is still in development. Feel free to try it out and to report issues or to suggest changes.
 
-## Quick start
+## 🚀 Quick start
 GPM-API provides an easy-to-use python interface to download, read, process and visualize most
 of the products of the Global Precipitation Measurement Mission (GPM) data archive.
 
 The list of available products can be retrieved using:
 
 ```python
 import gpm_api
 
-gpm_api.available_products(product_type="RS")  # research products
-gpm_api.available_products(product_type="NRT") # near-real-time products
+gpm_api.available_products(product_types="RS")  # research products
+gpm_api.available_products(product_types="NRT") # near-real-time products
 
 ```
 
 Before starting using GPM-API, we highly suggest to save into a configuration file:
 1. your credentials to access the [NASA Precipitation Processing System (PPS) servers][PPS_link]
 2. the directory on the local disk where to save the GPM dataset of interest.
 
@@ -137,14 +148,17 @@
 
 # You can check that the config file has been correctly created with:
 configs = gpm_api.read_configs()
 print(configs)
 
 ```
 
+-----------------------------------------------------------------------------------------
+#### 📥 Download GPM data
+
 Now you can either start to download GPM data within python:
 
 ```python
 import gpm_api
 import datetime
 
 product = "2A-DPR"
@@ -164,14 +178,16 @@
 ```
 
 or from the terminal using i.e. `download_daily_gpm_data <product> <year> <month> <day>`:
 
 ```bash
     download_daily_gpm_data 2A-DPR 2022 7 22
 ```
+-----------------------------------------------------------------------------------------
+#### 💫 Open GPM files into xarray
 
 A GPM granule can be opened in python using:
 
 ```python
 import gpm_api
 
 ds = gpm_api.open_granule(<path_to_granule>)
@@ -193,17 +209,24 @@
 ds = gpm_api.open_dataset(product=product,
                           product_type=product_type,
                           version=version
                           start_time=start_time,
                           end_time=end_time)
 ```
 
-Look at the [Tutorials][tutorial_link] to learn how to analyse and visualize the GPM products !
+-----------------------------------------------------------------------------------------
+#### 📖 Explore the GPM-API documentation
+
+To discover all GPM-API download, manipulation, analysis and plotting utilities, or how to contribute your custom retrieval to GPM-API:
+- please read the software documentation available at [[https://disdrodb.readthedocs.io/en/latest/](https://gpm-api.readthedocs.io/en/latest/)].
+- dive into the Jupyter Notebooks [Tutorials][tutorial_link] tutorials.
 
-## Installation
+-----------------------------------------------------------------------------------------
+
+## 🛠️ Installation
 
 
 ### pip
 
 GPM-API can be installed via [pip][pip_link] on Linux, Mac, and Windows.
 On Windows you can install [WinPython][winpy_link] to get Python and pip
 running.
@@ -224,19 +247,35 @@
 
     conda install gpm_api
 
 In case conda forge is not set up for your system yet, see the easy to follow
 instructions on [conda forge][conda_forge_link].
 
 
-## Documentation for GPM-API
+## 💭 Feedback and Contributing Guidelines
+
+If you aim to contribute your data or discuss the future development of GPM-API,
+we highly suggest to join the [**GPM-API Slack Workspace**](https://join.slack.com/t/gpmapi/shared_invite/zt-28vkxzjs1-~cIYci2o3G0qEEoQJVMQRg)
+
+Feel free to also open a [GitHub Issue](https://github.com/ghiggi/gpm_api/issues) or a [GitHub Discussion](https://github.com/ghiggi/gpm_api/discussions) specific to your questions or ideas.
 
-You can find the documentation under [gpm_api.readthedocs.io][doc_link]
+## Citation
+
+You can cite the GPM-API software by:
+
+> Ghiggi Gionata & XXXX . ghiggi/gpm_api. Zenodo. https://doi.org/10.5281/zenodo.7753488
+
+If you want to cite a specific software version, have a look at the [Zenodo site](https://doi.org/10.5281/zenodo.7753488).
+
+## License
 
-### Tutorials and Examples
+The content of this repository is released under the terms of the [MIT license](LICENSE).
+
+
+### Tutorials
 
 The documentation also includes some [tutorials][tut_link], showing the most important use cases of GPM-API.
 These tutorial are also available as Jupyter Notebooks and in Google Colab:
 
 - 1. Download the GPM products [[Notebook][tut1_download_link]][[Colab][colab1_download_link]]
 - 2. Introduction to the IMERG products [[Notebook][tut2_imerg_link]][[Colab][colab2_imerg_link]]
 - 2. Introduction to the PMW 1B and 1C products [[Notebook][tut2_pmw1bc_link]][[Colab][colab_pmw1bc_link]]
@@ -246,26 +285,14 @@
 - 2. Introduction to the Latent Heating products [[Notebook][tut2_lh_link]][[Colab][colab2_lh_link]]
 - 2. Introduction to the ENVironment products [[Notebook][tut2_env_link]][[Colab][colab2_env_link]]
 - 3. Introduction to image labeling and patch extraction [[Notebook][tut3_label_link]][[Colab][colab3_label_link]]
 - 3. Introduction to image patch extraction [[Notebook][tut3_patch_link]][[Colab][colab3_patch_link]]
 
 The associated python scripts are also provided in the `tutorial` folder.
 
-## Citation
-
-If you are using GPM-API in your publication please cite our paper:
-
-TODO: GMD
-
-You can cite the Zenodo code publication of GPM-API by:
-
-> Ghiggi Gionata & XXXX . ghiggi/gpm_api. Zenodo. https://doi.org/10.5281/zenodo.7753488
-
-If you want to cite a specific version, have a look at the [Zenodo site](https://doi.org/10.5281/zenodo.7753488).
-
 ## Requirements:
 
 - [xarray](https://docs.xarray.dev/en/stable/)
 - [dask](https://www.dask.org/)
 - [cartopy](https://scitools.org.uk/cartopy/docs/latest/)
 - [pyresample](https://pyresample.readthedocs.io/en/latest/)
 - [h5py](https://github.com/h5py/h5py)
@@ -274,18 +301,14 @@
 
 ### Optional
 
 - [zarr](https://zarr.readthedocs.io/en/stable/)
 - [dask_image](https://image.dask.org/en/latest/)
 - [skimage](https://scikit-image.org/)
 
-## License
-
-The content of this repository is released under the terms of the [MIT](LICENSE) license.
-
 [PPS_link]: https://gpm.nasa.gov/data/sources/pps-research
 [tutorial_link]: https://github.com/ghiggi/gpm_api/tree/master#tutorials-and-examples
 
 [pip_link]: https://pypi.org/project/gstools
 [conda_link]: https://docs.conda.io/en/latest/miniconda.html
 [conda_forge_link]: https://github.com/conda-forge/gpm_api-feedstock#installing-gpm_api
 [conda_pip]: https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-pkgs.html#installing-non-conda-packages
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `gpm_api-0.2.8/gpm_api/_config.py` & `gpm_api-0.2.9/gpm_api/_config.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/accessor/methods.py` & `gpm_api-0.2.9/gpm_api/accessor/methods.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,15 +138,15 @@
         )
 
     #### Profile utility
     def get_variable_at_bin(self, bin, variable=None):
         """Retrieve variable values at specific range bins."""
         from gpm_api.utils.manipulations import get_variable_at_bin
 
-        return get_variable_at_bin(self._obj, bin=bin, variable=None)
+        return get_variable_at_bin(self._obj, bin=bin, variable=variable)
 
     def get_height_at_bin(self, bin):
         """Retrieve height values at specific range bins."""
         from gpm_api.utils.manipulations import get_height_at_bin
 
         return get_height_at_bin(self._obj, bin=bin)
 
@@ -305,22 +305,22 @@
         return get_slices_contiguous_granules(self._obj, min_size=min_size)
 
     def get_slices_valid_geolocation(self, min_size=2):
         from gpm_api.utils.checks import get_slices_valid_geolocation
 
         return get_slices_valid_geolocation(self._obj, min_size=min_size)
 
-    def get_slices_regular(self, min_size=2):
+    def get_slices_regular(self, min_size=None):
         from gpm_api.utils.checks import get_slices_regular
 
         return get_slices_regular(self._obj, min_size=min_size)
 
     #### Plotting utility
     def plot_transect_line(
-        self, ax=None, add_direction=True, text_kwargs={}, line_kwargs={}, **common_kwargs
+        self, ax, add_direction=True, text_kwargs={}, line_kwargs={}, **common_kwargs
     ):
         from gpm_api.visualization.profile import plot_transect_line
 
         p = plot_transect_line(
             self._obj,
             ax=ax,
             add_direction=add_direction,
@@ -348,58 +348,66 @@
             edgecolor=edgecolor,
             alpha=alpha,
             add_background=add_background,
             **kwargs,
         )
         return p
 
-    def plot_swath_lines(self, ax=None, linestyle="--", color="k", **kwargs):
+    def plot_swath_lines(self, ax=None, x="lon", y="lat", linestyle="--", color="k", **kwargs):
         from gpm_api.visualization.orbit import plot_swath_lines
 
-        p = plot_swath_lines(self._obj, ax=ax, linestyle=linestyle, color=color, **kwargs)
+        p = plot_swath_lines(self._obj, ax=ax, x=x, y=y, linestyle=linestyle, color=color, **kwargs)
         return p
 
     def plot_map_mesh(
         self,
+        x="lon",
+        y="lat",
         ax=None,
         edgecolors="k",
         linewidth=0.1,
         add_background=True,
         fig_kwargs={},
         subplot_kwargs={},
         **plot_kwargs,
     ):
         from gpm_api.visualization.plot import plot_map_mesh
 
         p = plot_map_mesh(
             xr_obj=self._obj,
+            x=x,
+            y=y,
             ax=ax,
             edgecolors=edgecolors,
             linewidth=linewidth,
             add_background=add_background,
             fig_kwargs=fig_kwargs,
             subplot_kwargs=subplot_kwargs,
             **plot_kwargs,
         )
         return p
 
     def plot_map_mesh_centroids(
         self,
+        x="lon",
+        y="lat",
         ax=None,
         c="r",
         s=1,
         add_background=True,
         fig_kwargs={},
         subplot_kwargs={},
         **plot_kwargs,
     ):
         from gpm_api.visualization.plot import plot_map_mesh_centroids
 
         p = plot_map_mesh_centroids(
             self._obj,
+            x=x,
+            y=y,
             ax=ax,
             c=c,
             s=s,
             add_background=add_background,
             fig_kwargs=fig_kwargs,
             subplot_kwargs=subplot_kwargs,
             **plot_kwargs,
@@ -485,16 +493,16 @@
         cbar_kwargs={},
         **plot_kwargs,
     ):
         from gpm_api.visualization.plot import plot_map
 
         da = self._obj[variable]
         p = plot_map(
+            da,
             ax=ax,
-            da=da,
             x=x,
             y=y,
             add_colorbar=add_colorbar,
             rgb=rgb,
             add_swath_lines=add_swath_lines,
             add_background=add_background,
             interpolation=interpolation,
@@ -563,15 +571,15 @@
 
         return available_retrievals(self._obj)
 
     def retrieve(self, name, **kwargs):
         """Retrieve a GPM-API variable."""
         from gpm_api.retrievals.routines import get_retrieval_variable
 
-        return get_retrieval_variable(self._obj, retrieval=name, **kwargs)
+        return get_retrieval_variable(self._obj, name=name, **kwargs)
 
     def slice_range_at_temperature(self, temperature, variable_temperature="airTemperature"):
         """Slice the 3D arrays along a specific isotherm."""
         from gpm_api.utils.manipulations import slice_range_at_temperature
 
         return slice_range_at_temperature(
             self._obj, temperature=temperature, variable_temperature=variable_temperature
@@ -630,15 +638,15 @@
         cbar_kwargs={},
         **plot_kwargs,
     ):
         from gpm_api.visualization.plot import plot_map
 
         da = self._obj
         p = plot_map(
-            da=da,
+            da,
             ax=ax,
             x=x,
             y=y,
             add_colorbar=add_colorbar,
             add_swath_lines=add_swath_lines,
             add_background=add_background,
             rgb=rgb,
```

### Comparing `gpm_api-0.2.8/gpm_api/bucket/analysis.py` & `gpm_api-0.2.9/gpm_api/bucket/analysis.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/bucket/dataset.py` & `gpm_api-0.2.9/gpm_api/bucket/dataset.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/bucket/io.py` & `gpm_api-0.2.9/gpm_api/bucket/io.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/bucket/processing.py` & `gpm_api-0.2.9/gpm_api/bucket/processing.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/bucket/readers.py` & `gpm_api-0.2.9/gpm_api/bucket/readers.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/bucket/utils.py` & `gpm_api-0.2.9/gpm_api/bucket/utils.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/bucket/writers.py` & `gpm_api-0.2.9/gpm_api/bucket/writers.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/checks.py` & `gpm_api-0.2.9/gpm_api/checks.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/configs.py` & `gpm_api-0.2.9/gpm_api/configs.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/dataset/attrs.py` & `gpm_api-0.2.9/gpm_api/dataset/attrs.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/dataset/conventions.py` & `gpm_api-0.2.9/gpm_api/dataset/conventions.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/dataset/coords.py` & `gpm_api-0.2.9/gpm_api/dataset/coords.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/dataset/crs.py` & `gpm_api-0.2.9/gpm_api/dataset/crs.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/dataset/dataset.py` & `gpm_api-0.2.9/gpm_api/dataset/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -239,20 +239,20 @@
     -------
     xarray.Dataset
 
     """
     ## Check scan_mode
     scan_mode = check_scan_mode(scan_mode, product, version=version)
     ## Check valid product and variables
-    check_product(product, product_type=product_type)
+    product = check_product(product, product_type=product_type)
     variables = check_variables(variables)
     groups = check_groups(groups)
     # Check valid start/end time
     start_time, end_time = check_start_end_time(start_time, end_time)
-    check_valid_time_request(start_time, end_time, product)
+    start_time, end_time = check_valid_time_request(start_time, end_time, product)
 
     ##------------------------------------------------------------------------.
     # Find filepaths
     filepaths = find_filepaths(
         storage="local",
         version=version,
         product=product,
```

### Comparing `gpm_api-0.2.8/gpm_api/dataset/datatree.py` & `gpm_api-0.2.9/gpm_api/dataset/datatree.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/dataset/decoding/cf.py` & `gpm_api-0.2.9/gpm_api/dataset/decoding/cf.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/dataset/decoding/coordinates.py` & `gpm_api-0.2.9/gpm_api/dataset/decoding/coordinates.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/dataset/decoding/dataarray_attrs.py` & `gpm_api-0.2.9/gpm_api/dataset/decoding/dataarray_attrs.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/dataset/decoding/decode_2a_pmw.py` & `gpm_api-0.2.9/gpm_api/dataset/decoding/decode_2a_pmw.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/dataset/decoding/decode_2a_radar.py` & `gpm_api-0.2.9/gpm_api/dataset/decoding/decode_2a_radar.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/dataset/decoding/routines.py` & `gpm_api-0.2.9/gpm_api/dataset/decoding/routines.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,19 +24,19 @@
 
     return decode_function
 
 
 def decode_variables(ds, product):
     """Decode the variables of a given GPM product."""
     # Decode variables of 2A-<RADAR> products
-    if product in available_products(product_category="RADAR", product_level="2A"):
+    if product in available_products(product_categories="RADAR", product_levels="2A"):
         ds = _get_decoding_function("gpm_api.dataset.decoding.decode_2a_radar")(ds)
 
     # Decode variables of 2A-<PMW> products
-    if product in available_products(product_category="PMW", product_level="2A"):
+    if product in available_products(product_categories="PMW", product_levels="2A"):
         ds = _get_decoding_function("gpm_api.dataset.decoding.decode_2a_pmw")(ds)
 
     # if ds.attrs.get("TotalQualityCode"):
     #     TotalQualityCode = ds.attrs.get("TotalQualityCode")
     #     ds["TotalQualityCode"] = xr.DataArray(
     #         np.repeat(TotalQualityCode, ds.dims["along_track"]), dims=["along_track"]
     #     )
```

### Comparing `gpm_api-0.2.8/gpm_api/dataset/decoding/utils.py` & `gpm_api-0.2.9/gpm_api/dataset/decoding/utils.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/dataset/dimensions.py` & `gpm_api-0.2.9/gpm_api/dataset/dimensions.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/dataset/granule.py` & `gpm_api-0.2.9/gpm_api/dataset/granule.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/dataset/groups_variables.py` & `gpm_api-0.2.9/gpm_api/dataset/groups_variables.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/encoding/encode_2a_radar.py` & `gpm_api-0.2.9/gpm_api/encoding/encode_2a_radar.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/encoding/routines.py` & `gpm_api-0.2.9/gpm_api/encoding/routines.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         raise ValueError(f"get_encoding_dict function not found in the {module_name} module.")
     return func
 
 
 def get_product_encoding_dict(product):
     """Read encoding dictionary from GPM product YAML file."""
     # Define retrievals for 2A-<RADAR> products
-    if product in available_products(product_category="RADAR", product_level="2A"):
+    if product in available_products(product_categories="RADAR", product_levels="2A"):
         module_name = "gpm_api.dataset.encoding.encode_2a_radar"
         return _get_encoding_function(module_name)()
     else:
         return None
 
 
 def _get_dataset_keys(ds):
```

### Comparing `gpm_api-0.2.8/gpm_api/etc/country_acronyms.yaml` & `gpm_api-0.2.9/gpm_api/etc/country_acronyms.yaml`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/etc/country_bounds.yaml` & `gpm_api-0.2.9/gpm_api/etc/country_bounds.yaml`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/etc/country_extent.yaml` & `gpm_api-0.2.9/gpm_api/etc/country_extent.yaml`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/etc/pmw_frequency.yml` & `gpm_api-0.2.9/gpm_api/etc/pmw_frequency.yml`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/io/checks.py` & `gpm_api-0.2.9/gpm_api/io/find.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,278 +1,317 @@
 #!/usr/bin/env python3
 """
-Created on Sun Aug 14 20:02:18 2022
+Created on Thu Oct 26 17:04:07 2023
+
 @author: ghiggi
 """
 import datetime
-import os
+import warnings
 
+import dask
 import numpy as np
+import pandas as pd
 
+from gpm_api._config import config
+from gpm_api.io.checks import (
+    check_date,
+    check_product,
+    check_product_type,
+    check_product_version,
+    check_start_end_time,
+    check_storage,
+    check_valid_time_request,
+)
+from gpm_api.io.filter import filter_filepaths
+from gpm_api.io.ges_disc import get_gesdisc_daily_filepaths
+from gpm_api.io.info import get_version_from_filepaths
+from gpm_api.io.local import get_local_daily_filepaths
+from gpm_api.io.pps import get_pps_daily_filepaths
+from gpm_api.io.products import available_products
+from gpm_api.utils.list import flatten_list
+from gpm_api.utils.warnings import GPMDownloadWarning
 
-def check_base_dir(base_dir):
-    """Check base directory path.
+VERSION_WARNING = config.get("warn_multiple_product_versions")
 
-    If base_dir ends with "GPM" directory, it removes it from the base_dir path.
-    If base_dir does not end with "GPM", the GPM directory will be created.
-    Parameters
-    ----------
-    base_dir : str
-        Base directory where the GPM directory is located.
-    Returns
-    -------
-    base_dir: str
-        Base directory where the GPM directory is located.
-    """
-    # Check base_dir does not end with /
-    if base_dir[-1] == os.path.sep:
-        base_dir = base_dir[0:-1]
-    # Retrieve last folder name
-    dir_name = os.path.basename(base_dir)
-    # If ends with GPM, take the parent directory path
-    if dir_name == "GPM":
-        base_dir = os.path.dirname(base_dir)
-    return base_dir
-
-
-def check_filepaths(filepaths):
-    if isinstance(filepaths, str):
-        filepaths = [filepaths]
-    if not isinstance(filepaths, list):
-        raise TypeError("Expecting a list of filepaths.")
-    return filepaths
 
+def _get_all_daily_filepaths(storage, date, product, product_type, version, verbose):
+    """Return the find_daily_filepaths_func.
 
-def check_variables(variables):
-    if not isinstance(variables, (str, list, np.ndarray, type(None))):
-        raise TypeError("'variables' must be a either a str, list, np.ndarray or None.")
-    if variables is None:
-        return None
-    if isinstance(variables, str):
-        variables = [variables]
-    elif isinstance(variables, list):
-        variables = np.array(variables)
-    return variables
-
-
-def check_groups(groups):
-    if not isinstance(groups, (str, list, np.ndarray, type(None))):
-        raise TypeError("'groups' must be a either a str, list, np.ndarray or None.")
-    if isinstance(groups, str):
-        groups = [groups]
-    elif isinstance(groups, list):
-        groups = np.array(groups)
-    return groups
-
-
-def check_storage(storage):
-    """Check storage."""
-    if not isinstance(storage, str):
-        raise TypeError("'storage' must be a string.")
-    valid_storages = ["ges_disc", "pps", "local"]
-    if storage.lower() not in valid_storages:
-        raise ValueError(f"{storage} is an invalid storage. Valid values are {valid_storages}.")
-    return storage.lower()
-
-
-def check_remote_storage(storage):
-    """Check storage is remote."""
-    if not isinstance(storage, str):
-        raise TypeError("'storage' must be a string.")
-    valid_storages = ["ges_disc", "pps"]
-    if storage.lower() not in valid_storages:
-        raise ValueError(
-            f"{storage} is an invalid remote storage. Valid values are {valid_storages}."
+    This functions returns a tuple ([filepaths][available_version])
+    """
+    if storage == "local":
+        filepaths = get_local_daily_filepaths(
+            product=product,
+            product_type=product_type,
+            date=date,
+            version=version,
+            verbose=verbose,
         )
-    return storage.lower()
-
-
-def check_version(version):
-    if not isinstance(version, int):
-        raise ValueError("Please specify the GPM version with an integer between 5 and 7.")
-    if version not in [4, 5, 6, 7]:
-        raise ValueError("Download/Reading have been implemented only for GPM versions 5, 6 and 7.")
-
-
-def check_product_version(version, product):
-    from gpm_api.io.products import available_versions, get_last_product_version
-
-    if version is None:
-        version = get_last_product_version(product)
-    check_version(version)
-    # Check valid version for such product
-    valid_versions = available_versions(product)
-    if version not in valid_versions:
-        raise ValueError(f"Valid versions for product {product} are {valid_versions}.")
-    return version
-
-
-def check_product(product, product_type):
-    from gpm_api.io.products import available_products
+    elif storage == "pps":
+        filepaths = get_pps_daily_filepaths(
+            product=product,
+            product_type=product_type,
+            date=date,
+            version=version,
+            verbose=verbose,
+        )
+    elif storage == "ges_disc":
+        filepaths = get_gesdisc_daily_filepaths(
+            product=product,
+            product_type=product_type,
+            date=date,
+            version=version,
+            verbose=verbose,
+        )
+    else:
+        raise ValueError(f"Invalid storage {storage}.")
+    return filepaths
 
-    if not isinstance(product, str):
-        raise ValueError("'Ask for a single product at time.'product' must be a single string.")
-    if product not in available_products(product_type=product_type):
-        raise ValueError("Please provide a valid GPM product --> gpm_api.available_products().")
 
+def _check_correct_version(filepaths, product, version):
+    """Check the file version is correct.
 
-def check_product_type(product_type):
-    if not isinstance(product_type, str):
-        raise ValueError("Please specify the product_type as a string..")
-    if product_type not in ["RS", "NRT"]:
-        raise ValueError("Please specify the product_type as 'RS' or 'NRT'.")
+    Several products are not available to the last version.
+    So to archive data correctly on the user side, we check that the file version
+    actually match the asked version, and otherwise we download the last available version.
+    """
+    global VERSION_WARNING  # To just warn once. Maybe to be defined at each download call
 
+    if len(filepaths) == 0:
+        return filepaths, version
 
-def check_product_category(product_category):
-    if not isinstance(product_category, str):
-        raise ValueError("Please specify the product_category as a string.")
-    valid_values = ["RADAR", "PMW", "CMB", "IMERG"]
-    if product_category not in valid_values:
+    files_versions = np.unique(get_version_from_filepaths(filepaths, integer=True)).tolist()
+    if len(files_versions) > 1:
         raise ValueError(
-            f"{product_category} is an invalid product_category. Valid values are {valid_values}."
+            f"Multiple file versions found: {files_versions}. Please report their occurrence !"
         )
+    files_version = files_versions[0]
+    if files_version != version:
+        if VERSION_WARNING:
+            VERSION_WARNING = False
+            msg = f"The last available version for {product} product is version {files_version}! "
+            msg += f"Starting the download of version {files_version}."
+            warnings.warn(msg, GPMDownloadWarning)
+    return filepaths, files_version
+
+
+def _ensure_valid_start_date(start_date, product):
+    """Ensure that the product directory exists for start_date."""
+    if product == "2A-SAPHIR-MT1-CLIM":
+        min_start_date = "2011-10-13 00:00:00"
+    elif "1A-" in product or "1B-" in product:
+        min_start_date = "1997-12-07 00:00:00"
+    elif product in available_products(product_categories="PMW"):
+        min_start_date = "1987-07-09 00:00:00"
+    elif product in available_products(product_categories="RADAR") or product in available_products(
+        product_categories="CMB"
+    ):
+        min_start_date = "1997-12-07 00:00:00"
+    elif "IMERG" in product:
+        min_start_date = "2000-06-01 00:00:00"
+    else:
+        min_start_date = "1987-07-09 00:00:00"
+    min_start_date = datetime.datetime.fromisoformat(min_start_date)
+    start_date = max(start_date, min_start_date)
+    return start_date
+
+
+def find_daily_filepaths(
+    storage,
+    date,
+    product,
+    product_type,
+    version,
+    start_time=None,
+    end_time=None,
+    verbose=False,
+):
+    """
+    Retrieve GPM data filepaths for a specific day and product.
 
+    Parameters
+    ----------
+    date : datetime.date
+        Single date for which to retrieve the data.
+    product : str
+        GPM product acronym. See gpm_api.available_products()
+    start_time : datetime.datetime
+        Filtering start time.
+    end_time : datetime.datetime
+        Filtering end time.
+    product_type : str, optional
+        GPM product type. Either 'RS' (Research) or 'NRT' (Near-Real-Time).
+    version : int, optional
+        GPM version of the data to retrieve if product_type = 'RS'.
+    verbose : bool, optional
+        Default is False.
 
-def check_product_level(product_level):
-    if not isinstance(product_level, str):
-        raise ValueError("Please specify the product_level as a string.")
-    valid_values = ["1A", "1B", "1C", "2A", "2B"]
-    if product_level not in valid_values:
-        raise ValueError(
-            f"{product_level} is an invalid product_level. Currently accepted values are {valid_values}."
-        )
-
+    Returns
+    -------
+    pps_fpaths: list
+        List of file paths on the NASA PPS server.
+    available_version: list
+        List of available versions.
 
-def check_product_validity(product, product_type=None):
-    """Check product validity."""
-    from gpm_api.io.products import available_products  # circular otherwise
-
-    if product not in available_products(product_type=product_type):
-        if product_type is None:
-            raise ValueError(
-                f"The {product} product is not available. See gpm_api.available_products()."
-            )
-        else:
-            raise ValueError(
-                f"The {product} product is not available as {product_type} product_type."
+    """
+    ##------------------------------------------------------------------------.
+    # Check date
+    date = check_date(date)
+
+    ##------------------------------------------------------------------------.
+    # Retrieve list of available files on pps
+    filepaths = _get_all_daily_filepaths(
+        storage=storage,
+        product=product,
+        product_type=product_type,
+        date=date,
+        version=version,
+        verbose=verbose,
+    )
+    if len(filepaths) == 0:
+        if storage == "local" and verbose:
+            version_str = str(int(version))
+            print(
+                f"The GPM product {product} (V0{version_str}) on date {date} has not been downloaded !"
             )
+        return [], []
 
-
-def check_time(time):
-    """Check time validity.
-
-    It returns a datetime.datetime object to seconds precision.
+    ##------------------------------------------------------------------------.
+    # Filter the GPM daily file list (for product, start_time & end time)
+    # - The version mismatch is raised later eventually !
+    filepaths = filter_filepaths(
+        filepaths,
+        product=product,
+        product_type=product_type,
+        version=None,  # important to not filter !
+        start_time=start_time,
+        end_time=end_time,
+    )
+    if len(filepaths) == 0:
+        return [], []
+
+    ## -----------------------------------------------------------------------.
+    ## Check correct version and return the available version
+    filepaths, available_version = _check_correct_version(
+        filepaths=filepaths, product=product, version=version
+    )
+    return filepaths, [available_version]
+
+
+def find_filepaths(
+    storage,
+    product,
+    start_time,
+    end_time,
+    product_type="RS",
+    version=None,
+    verbose=True,
+    parallel=True,
+):
+    """
+    Retrieve GPM data filepaths on local disk for a specific time period and product.
 
     Parameters
     ----------
-    time : (datetime.datetime, datetime.date, np.datetime64, str)
-        Time object.
-        Accepted types: datetime.datetime, datetime.date, np.datetime64, str
-        If string type, it expects the isoformat 'YYYY-MM-DD hh:mm:ss'.
+    product : str
+        GPM product acronym. See gpm_api.available_products()
+    start_time : datetime.datetime
+        Start time.
+    end_time : datetime.datetime
+        End time.
+    product_type : str, optional
+        GPM product type. Either 'RS' (Research) or 'NRT' (Near-Real-Time).
+    version : int, optional
+        GPM version of the data to retrieve if product_type = 'RS'.
+    verbose : bool, optional
+        Whether to print processing details. The default is True.
+    parallel : bool, optional
+        Whether to loop over dates in parallel.
+        The default is True.
 
     Returns
     -------
-    time : datetime.datetime
-        datetime.datetime object
+    filepaths : list
+        List of GPM filepaths.
 
     """
-    if not isinstance(time, (datetime.datetime, datetime.date, np.datetime64, np.ndarray, str)):
-        raise TypeError(
-            "Specify time with datetime.datetime objects or a "
-            "string of format 'YYYY-MM-DD hh:mm:ss'."
-        )
-    # If numpy array with datetime64 (and size=1)
-    if isinstance(time, np.ndarray):
-        if np.issubdtype(time.dtype, np.datetime64):
-            if time.size == 1:
-                time = time[0].astype("datetime64[s]").tolist()
-            else:
-                raise ValueError("Expecting a single timestep!")
-        else:
-            raise ValueError("The numpy array does not have a np.datetime64 dtype!")
-
-    # If np.datetime64, convert to datetime.datetime
-    if isinstance(time, np.datetime64):
-        time = time.astype("datetime64[s]").tolist()
-    # If datetime.date, convert to datetime.datetime
-    if not isinstance(time, (datetime.datetime, str)):
-        time = datetime.datetime(time.year, time.month, time.day, 0, 0, 0)
-    if isinstance(time, str):
-        try:
-            time = datetime.datetime.fromisoformat(time)
-        except ValueError:
-            raise ValueError("The time string must have format 'YYYY-MM-DD hh:mm:ss'")
-
-    # If datetime object carries timezone that is not UTC, raise error
-    if time.tzinfo is not None:
-        if str(time.tzinfo) != "UTC":
-            raise ValueError("The datetime object must be in UTC timezone if timezone is given.")
-        else:
-            # If UTC, strip timezone information
-            time = time.replace(tzinfo=None)
-
-    return time
-
-
-def check_date(date):
-    """Check is a datetime.date object."""
-    if date is None:
-        raise ValueError("date cannot be None")
-
-    # Use check_time to convert to datetime.datetime
-    datetime_obj = check_time(date)
-    return datetime_obj.date()
-
-
-def check_start_end_time(start_time, end_time):
-    """Check start_time and end_time value validity."""
-    start_time = check_time(start_time)
-    end_time = check_time(end_time)
-    # Check start_time and end_time are chronological
-    if start_time > end_time:
-        raise ValueError("Provide start_time occurring before of end_time.")
-    # Check start_time and end_time are in the past
-    if start_time > datetime.datetime.utcnow():
-        raise ValueError("Provide a start_time occurring in the past.")
-    if end_time > datetime.datetime.utcnow():
-        raise ValueError("Provide a end_time occurring in the past.")
-    return (start_time, end_time)
-
-
-def check_valid_time_request(start_time, end_time, product):
-    """Check validity of the time request."""
-    from gpm_api.io.products import get_product_end_time, get_product_start_time
-
-    product_start_time = get_product_start_time(product)
-    product_end_time = get_product_end_time(product)
-    if start_time < product_start_time:
-        raise ValueError(f"{product} production started the {product_start_time}.")
-    if end_time > product_end_time:
-        raise ValueError(f"{product} production ended the {get_product_end_time}.")
-
+    # -------------------------------------------------------------------------.
+    ## Checks input arguments
+    storage = check_storage(storage)
+    version = check_product_version(version, product)
+    product_type = check_product_type(product_type=product_type)
+    product = check_product(product=product, product_type=product_type)
+    start_time, end_time = check_start_end_time(start_time, end_time)
+    start_time, end_time = check_valid_time_request(start_time, end_time, product)
+
+    # Retrieve sequence of dates
+    # - Specify start_date - 1 day to include data potentially on previous day directory
+    # --> Example granules starting at 23:XX:XX in the day before and extending to 01:XX:XX
+    start_date = datetime.datetime(start_time.year, start_time.month, start_time.day)
+    start_date = start_date - datetime.timedelta(days=1)
+    start_date = _ensure_valid_start_date(start_date=start_date, product=product)
+    end_date = datetime.datetime(end_time.year, end_time.month, end_time.day)
+    date_range = pd.date_range(start=start_date, end=end_date, freq="D")
+    dates = list(date_range.to_pydatetime())
 
-def check_scan_mode(scan_mode, product, version):
-    """Checks the validity of scan_mode."""
     # -------------------------------------------------------------------------.
-    # Get valid scan modes
-    from gpm_api.io.products import available_scan_modes
+    # If NRT, all data lies in a single directory at PPS
+    if storage == "pps" and product_type == "NRT":
+        dates = [dates[0]]
+        parallel = False
 
-    scan_modes = available_scan_modes(product, version)
+    # -------------------------------------------------------------------------.
+    # Loop over dates and retrieve available filepaths
+    if parallel:
+        list_delayed = []
+        verbose_arg = verbose
+        for i, date in enumerate(dates):
+            verbose = False if i == 0 else verbose_arg
+            del_op = dask.delayed(find_daily_filepaths)(
+                storage=storage,
+                version=version,
+                product=product,
+                product_type=product_type,
+                date=date,
+                start_time=start_time,
+                end_time=end_time,
+                verbose=verbose,
+            )
+            list_delayed.append(del_op)
+        # Get filepaths list for each date
+        list_filepaths = dask.compute(*list_delayed)
+        list_filepaths = [tpl[0] for tpl in list_filepaths]  # tpl[1] is the available version
+
+    else:
+        # TODO list
+        # - start_time and end_time filtering could be done only on first and last iteration
+        # - misleading error message can occur on last iteration if end_time is close to 00:00:00
+        #   and the searched granule is in previous day directory
+        list_filepaths = []
+        verbose_arg = verbose
+        for i, date in enumerate(dates):
+            verbose = False if i == 0 else verbose_arg
+            filepaths, _ = find_daily_filepaths(
+                storage=storage,
+                version=version,
+                product=product,
+                product_type=product_type,
+                date=date,
+                start_time=start_time,
+                end_time=end_time,
+                verbose=verbose,
+            )
+            # Concatenate filepaths
+            list_filepaths += filepaths
 
-    # Infer scan mode if not specified
-    if scan_mode is None:
-        scan_mode = scan_modes[0]
-        if len(scan_modes) > 1:
-            print(f"'scan_mode' has not been specified. Default to {scan_mode}.")
+    filepaths = flatten_list(list_filepaths)
 
     # -------------------------------------------------------------------------.
-    # Check that a single scan mode is specified
-    if scan_mode is not None and not isinstance(scan_mode, str):
-        raise ValueError("Specify a single 'scan_mode'.")
+    # Check unique version
+    # - TODO, warning if same integer but different letter
+    # - TODO: error if different integer
 
     # -------------------------------------------------------------------------.
-    # Check that a valid scan mode is specified
-    if scan_mode is not None and scan_mode not in scan_modes:
-        raise ValueError(f"For {product} product, valid scan_modes are {scan_modes}.")
+    # Return sorted filepaths
+    filepaths = sorted(filepaths)
 
-    # -------------------------------------------------------------------------.
-    return scan_mode
+    return filepaths
```

### Comparing `gpm_api-0.2.8/gpm_api/io/data_integrity.py` & `gpm_api-0.2.9/gpm_api/io/data_integrity.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,18 +101,18 @@
     Returns
     -------
     filepaths, list
         List of file paths which are corrupted.
 
     """
     # Check valid product and variables
-    check_product(product, product_type=product_type)
+    product = check_product(product, product_type=product_type)
     # Check valid start/end time
     start_time, end_time = check_start_end_time(start_time, end_time)
-    check_valid_time_request(start_time, end_time, product)
+    start_time, end_time = check_valid_time_request(start_time, end_time, product=product)
     # Find filepaths
     filepaths = find_filepaths(
         storage="local",
         version=version,
         product=product,
         product_type=product_type,
         start_time=start_time,
```

### Comparing `gpm_api-0.2.8/gpm_api/io/download.py` & `gpm_api-0.2.9/gpm_api/io/download.py`

 * *Files 1% similar despite different names*

```diff
@@ -696,16 +696,16 @@
     int
         0 if everything went fine.
 
     """
     # -------------------------------------------------------------------------.
     ## Check input arguments
     date = check_date(date)
-    check_product_type(product_type=product_type)
-    check_product(product=product, product_type=product_type)
+    product_type = check_product_type(product_type=product_type)
+    product = check_product(product=product, product_type=product_type)
     storage = check_remote_storage(storage)
     # -------------------------------------------------------------------------.
     ## Retrieve the list of files available on NASA PPS server
     remote_filepaths, available_version = find_daily_filepaths(
         storage=storage,
         product=product,
         product_type=product_type,
@@ -851,19 +851,19 @@
     retry : int, optional,
         The number of attempts to redownload the corrupted files. The default is 1.
         Only applies if check_integrity is True !
     """
     # -------------------------------------------------------------------------.
     ## Checks input arguments
     storage = check_remote_storage(storage)
-    check_product_type(product_type=product_type)
-    check_product(product=product, product_type=product_type)
+    product_type = check_product_type(product_type=product_type)
+    product = check_product(product=product, product_type=product_type)
     version = check_product_version(version, product)
     start_time, end_time = check_start_end_time(start_time, end_time)
-    check_valid_time_request(start_time, end_time, product)
+    start_time, end_time = check_valid_time_request(start_time, end_time, product)
     # -------------------------------------------------------------------------.
     # Retrieve sequence of dates
     # - Specify start_date - 1 day to include data potentially on previous day directory
     # --> Example granules starting at 23:XX:XX in the day before and extending to 01:XX:XX
     start_date = datetime.datetime(start_time.year, start_time.month, start_time.day)
     start_date = start_date - datetime.timedelta(days=1)
     end_date = datetime.datetime(end_time.year, end_time.month, end_time.day)
```

### Comparing `gpm_api-0.2.8/gpm_api/io/filter.py` & `gpm_api-0.2.9/gpm_api/io/filter.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,15 +84,14 @@
     -------
 
     filepaths : list
         Returns the filepaths subset.
         If no valid filepaths, return an empty list.
 
     """
-
     try:
         info_dict = get_info_from_filepath(filepath)
     except ValueError:
         return None
 
     # Filter by version
     if version is not None:
@@ -158,15 +157,15 @@
     # Check filepaths
     if isinstance(filepaths, type(None)):
         return []
     filepaths = check_filepaths(filepaths)
     if len(filepaths) == 0:
         return []
     # Check product validity
-    check_product(product=product, product_type=product_type)
+    product = check_product(product=product, product_type=product_type)
     # Check start_time and end_time
     if start_time is not None or end_time is not None:
         if start_time is None:
             start_time = datetime.datetime(1998, 1, 1, 0, 0, 0)  # GPM start mission
         if end_time is None:
             end_time = datetime.datetime.now()  # Current time
     # Filter filepaths
@@ -201,26 +200,25 @@
     Returns
     ----------
     filepaths : list
         List of valid filepaths.
         If no valid filepaths, returns an empty list !
 
     """
-    # return filter_filepaths(filepaths, product=product, product_type=product_type)
     # -------------------------------------------------------------------------.
     # Check filepaths
     if isinstance(filepaths, type(None)):
         return []
     filepaths = check_filepaths(filepaths)
     if len(filepaths) == 0:
         return []
 
     # -------------------------------------------------------------------------.
     # Check product validity
-    check_product(product=product, product_type=product_type)
+    product = check_product(product=product, product_type=product_type)
 
     # -------------------------------------------------------------------------.
     # Retrieve GPM filename dictionary
     product_pattern = get_product_pattern(product)
 
     # -------------------------------------------------------------------------.
     # Subset by specific product
@@ -250,15 +248,14 @@
 
     Returns
     ----------
     filepaths : list
         List of valid filepaths.
         If no valid filepaths, returns an empty list !
     """
-    # return filter_filepaths(filepaths, start_time=start_time, end_time=end_time)
     # -------------------------------------------------------------------------.
     # Check filepaths
     if isinstance(filepaths, type(None)):
         return []
     filepaths = check_filepaths(filepaths)
     if len(filepaths) == 0:
         return []
@@ -313,26 +310,25 @@
 
     Returns
     ----------
     filepaths : list
         List of valid filepaths.
         If no valid filepaths, returns an empty list !
     """
-    # return filter_filepaths(filepaths, version=version)
     # -------------------------------------------------------------------------.
     # Check filepaths
     if isinstance(filepaths, type(None)):
         return []
     filepaths = check_filepaths(filepaths)
     if len(filepaths) == 0:
         return []
 
     # -------------------------------------------------------------------------.
     # Check version validity
-    check_version(version)
+    version = check_version(version)
 
     # -------------------------------------------------------------------------.
     # Retrieve GPM granules version
     l_version = get_version_from_filepaths(filepaths)
 
     # -------------------------------------------------------------------------.
     # Select valid filepaths
```

### Comparing `gpm_api-0.2.8/gpm_api/io/find.py` & `gpm_api-0.2.9/gpm_api/io/pps.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,318 +1,359 @@
 #!/usr/bin/env python3
 """
-Created on Thu Oct 26 17:04:07 2023
+Created on Thu Oct 13 17:45:37 2022
 
 @author: ghiggi
 """
 import datetime
-import warnings
+import subprocess
 
-import dask
-import numpy as np
-import pandas as pd
+from dateutil.relativedelta import relativedelta
 
-from gpm_api._config import config
+from gpm_api.configs import get_pps_password, get_pps_username
 from gpm_api.io.checks import (
-    check_date,
-    check_product,
     check_product_type,
+    check_product_validity,
     check_product_version,
-    check_start_end_time,
-    check_storage,
-    check_valid_time_request,
 )
-from gpm_api.io.filter import filter_filepaths
-from gpm_api.io.ges_disc import get_gesdisc_daily_filepaths
-from gpm_api.io.info import get_version_from_filepaths
-from gpm_api.io.local import get_local_daily_filepaths
-from gpm_api.io.pps import get_pps_daily_filepaths
-from gpm_api.io.products import available_products
-from gpm_api.utils.list import flatten_list
-from gpm_api.utils.warnings import GPMDownloadWarning
-
-VERSION_WARNING = config.get("warn_multiple_product_versions")
-
-
-def _get_all_daily_filepaths(storage, date, product, product_type, version, verbose):
-    """Return the find_daily_filepaths_func.
-
-    This functions returns a tuple ([filepaths][available_version])
-    """
-    if storage == "local":
-        filepaths = get_local_daily_filepaths(
-            product=product,
-            product_type=product_type,
-            date=date,
-            version=version,
-            verbose=verbose,
-        )
-    elif storage == "pps":
-        filepaths = get_pps_daily_filepaths(
-            product=product,
-            product_type=product_type,
-            date=date,
-            version=version,
-            verbose=verbose,
-        )
-    elif storage == "ges_disc":
-        filepaths = get_gesdisc_daily_filepaths(
-            product=product,
-            product_type=product_type,
-            date=date,
-            version=version,
-            verbose=verbose,
-        )
+from gpm_api.io.products import available_products, get_product_info
+
+####--------------------------------------------------------------------------.
+#####################
+#### Directories ####
+#####################
+
+
+def _get_pps_text_server(product_type):
+    """Return the url to the PPS text servers."""
+    if product_type == "NRT":
+        url_text_server = "https://jsimpsonhttps.pps.eosdis.nasa.gov/text"
     else:
-        raise ValueError(f"Invalid storage {storage}.")
-    return filepaths
+        url_text_server = "https://arthurhouhttps.pps.eosdis.nasa.gov/text"
+    return url_text_server
 
 
-def _check_correct_version(filepaths, product, version):
-    """Check the file version is correct.
+def _get_pps_data_server(product_type):
+    """Return the url to the PPS data servers."""
+    if product_type == "NRT":
+        url_data_server = "ftps://jsimpsonftps.pps.eosdis.nasa.gov/data"
+    else:
+        url_data_server = "ftps://arthurhouftps.pps.eosdis.nasa.gov"
+    return url_data_server
 
-    If 'version' is the last version, we retrieve data from 'gpmalldata' directory.
-    But many products are not available to the last version.
-    So to archive data correctly on the user side, we check that the file version
-    actually match the asked version, and otherwise we download the last available version.
-    """
-    global VERSION_WARNING  # To just warn once. Maybe to be defined at each download call
 
-    if len(filepaths) == 0:
-        return filepaths, version
+def _get_pps_nrt_product_folder_name(product):
+    """ "Retrieve NASA PPS server folder name for NRT product_type."""
+    folder_name = get_product_info(product).get("pps_nrt_dir", None)
+    if folder_name is None:
+        raise ValueError(
+            f"The pps_nrt_dir key of the {product} product is not specified in the config files."
+        )
+    return folder_name
+
 
-    files_versions = np.unique(get_version_from_filepaths(filepaths, integer=True)).tolist()
-    if len(files_versions) > 1:
+def _get_pps_rs_product_folder_name(product):
+    """ "Retrieve NASA PPS server folder name for RS product_type."""
+    folder_name = get_product_info(product).get("pps_rs_dir", None)
+    if folder_name is None:
         raise ValueError(
-            f"Multiple file versions found: {files_versions}. Please report their occurrence !"
+            f"The pps_rs_dir key of the {product} product is not specified in the config files."
         )
-    files_version = files_versions[0]
-    if files_version != version:
-        if VERSION_WARNING:
-            VERSION_WARNING = False
-            msg = f"The last available version for {product} product is version {files_version}! "
-            msg += f"Starting the download of version {files_version}."
-            warnings.warn(msg, GPMDownloadWarning)
-    return filepaths, files_version
-
-
-def _ensure_valid_start_date(start_date, product):
-    """Ensure that the product directory exists for start_date."""
-    if product == "2A-SAPHIR-MT1-CLIM":
-        min_start_date = "2011-10-13 00:00:00"
-    elif "1A-" in product or "1B-" in product:
-        min_start_date = "1997-12-07 00:00:00"
-    elif product in available_products(product_category="PMW"):
-        min_start_date = "1987-07-09 00:00:00"
-    elif product in available_products(product_category="RADAR") or product in available_products(
-        product_category="CMB"
-    ):
-        min_start_date = "1997-12-07 00:00:00"
-    elif "IMERG" in product:
-        min_start_date = "2000-06-01 00:00:00"
+    return folder_name
+
+
+def _get_pps_nrt_product_dir(product, date):
+    """
+    Retrieve the NASA PPS server directory structure where NRT data are stored.
+
+    Parameters
+    ----------
+    product : str
+        GPM product name. See: gpm_api.available_products() .
+    date : datetime.date
+        Single date for which to retrieve the data.
+        Note: this is currently only needed when retrieving IMERG data.
+    """
+    folder_name = _get_pps_nrt_product_folder_name(product)
+    # Specify the directory tree
+    if product in available_products(product_types="NRT", product_categories="IMERG"):
+        directory_tree = f"{folder_name}/{datetime.datetime.strftime(date, '%Y%m')}"
     else:
-        min_start_date = "1987-07-09 00:00:00"
-    min_start_date = datetime.datetime.fromisoformat(min_start_date)
-    start_date = max(start_date, min_start_date)
-    return start_date
-
-
-def find_daily_filepaths(
-    storage,
-    date,
-    product,
-    product_type,
-    version,
-    start_time=None,
-    end_time=None,
-    verbose=False,
-):
+        directory_tree = folder_name
+    return directory_tree
+
+
+def _get_pps_rs_product_dir(product, date, version):
     """
-    Retrieve GPM data filepaths for a specific day and product.
+    Retrieve the NASA PPS server directory structure where RS data are stored.
 
     Parameters
     ----------
+    product : str
+        GPM product name. See: gpm_api.available_products() .
     date : datetime.date
         Single date for which to retrieve the data.
+    version : int
+        GPM version of the data to retrieve if product_type = 'RS'.
+    """
+    version = check_product_version(version, product)
+    product = check_product_validity(product, product_type="RS")
+
+    # Retrieve NASA server folder name for RS
+    folder_name = _get_pps_rs_product_folder_name(product)
+
+    # Specify the directory tree for current RS version
+    if version == 7:
+        directory_tree = "/".join(
+            [
+                "gpmdata",
+                datetime.datetime.strftime(date, "%Y/%m/%d"),
+                folder_name,
+            ]
+        )
+    # Specify the directory tree for old RS version
+    else:  #  version in [4, 5, 6]:
+        version_str = "V0" + str(int(version))
+        directory_tree = "/".join(
+            [
+                "gpmallversions",
+                version_str,
+                datetime.datetime.strftime(date, "%Y/%m/%d"),
+                folder_name,
+            ]
+        )
+
+    # Return the directory tree
+    return directory_tree
+
+
+def _get_pps_directory_tree(product, product_type, date, version):
+    """
+    Retrieve the NASA PPS server directory tree where the GPM data are stored.
+
+    The directory tree structure for product_type="RS" is:
+        - <gpmallversions>/V0<version>/<pps_rs_dir>/YYYY/MM/DD
+        -  The L3 monthly products are saved in the YYYY/MM/01 directory
+
+    The directory tree structure for product_type="NRT" is:
+        - IMERG-ER and IMERG-FR: imerg/<early/late>/YYYY/MM/
+        - Otherwise <pps_nrt_dir>/
+
+    Parameters
+    ----------
     product : str
-        GPM product acronym. See gpm_api.available_products()
-    start_time : datetime.datetime
-        Filtering start time.
-    end_time : datetime.datetime
-        Filtering end time.
-    product_type : str, optional
+        GPM product name. See: gpm_api.available_products() .
+    product_type : str
         GPM product type. Either 'RS' (Research) or 'NRT' (Near-Real-Time).
-    version : int, optional
+    date : datetime.date
+        Single date for which to retrieve the data.
+    version : int
         GPM version of the data to retrieve if product_type = 'RS'.
-    verbose : bool, optional
-        Default is False.
 
     Returns
     -------
-    pps_fpaths: list
-        List of file paths on the NASA PPS server.
-    available_version: list
-        List of available versions.
+    directory_tree : str
+        DIrectory tree on the NASA PPS server where the data are stored.
+    """
+    product_type = check_product_type(product_type)
+    if product_type == "NRT":
+        return _get_pps_nrt_product_dir(product, date)
+    else:  # product_type == "RS"
+        return _get_pps_rs_product_dir(product, date, version)
 
+
+def get_pps_product_directory(product, product_type, date, version, server_type):
     """
-    ##------------------------------------------------------------------------.
-    # Check date
-    date = check_date(date)
-
-    ##------------------------------------------------------------------------.
-    # Retrieve list of available files on pps
-    filepaths = _get_all_daily_filepaths(
-        storage=storage,
-        product=product,
-        product_type=product_type,
-        date=date,
-        version=version,
-        verbose=verbose,
-    )
-    if len(filepaths) == 0:
-        if storage == "local" and verbose:
-            version_str = str(int(version))
-            print(
-                f"The GPM product {product} (V0{version_str}) on date {date} has not been downloaded !"
-            )
-        return [], []
-
-    ##------------------------------------------------------------------------.
-    # Filter the GPM daily file list (for product, start_time & end time)
-    # - The version mismatch is raised later eventually !
-    filepaths = filter_filepaths(
-        filepaths,
-        product=product,
-        product_type=product_type,
-        version=None,  # important to not filter !
-        start_time=start_time,
-        end_time=end_time,
-    )
-    if len(filepaths) == 0:
-        return [], []
+    Retrieve the NASA PPS server product directory path at specific date.
 
-    ## -----------------------------------------------------------------------.
-    ## Check correct version and return the available version
-    filepaths, available_version = _check_correct_version(
-        filepaths=filepaths, product=product, version=version
+    The data list is retrieved using https.
+    The data stored are retrieved using ftps.
+
+    Parameters
+    ----------
+    product : str
+        GPM product name. See: gpm_api.available_products() .
+    product_type : str
+        GPM product type. Either 'RS' (Research) or 'NRT' (Near-Real-Time).
+    date : datetime.date
+        Single date for which to retrieve the data.
+    version : int
+        GPM version of the data to retrieve if product_type = 'RS'.
+    server_type: str
+        Either "text" or "data"
+
+    Returns
+    -------
+    url_product_dir : str
+        url of the NASA PPS server where the data are listed.
+    """
+    # Retrieve server URL
+    if server_type == "text":
+        url_server = _get_pps_text_server(product_type)
+    else:
+        url_server = _get_pps_data_server(product_type)
+    # Retrieve directory tree structure
+    dir_structure = _get_pps_directory_tree(
+        product=product, product_type=product_type, date=date, version=version
     )
-    return filepaths, [available_version]
+    # Define product directory where data are listed
+    url_product_dir = f"{url_server}/{dir_structure}"
+    return url_product_dir
+
+
+####--------------------------------------------------------------------------.
+############################
+#### Filepath retrieval ####
+############################
+
+
+def __get_pps_file_list(url_product_dir):
+    # Retrieve GPM-API configs
+    username = get_pps_username()
+    password = get_pps_password()
+    # Ensure url_file_list ends with "/"
+    if url_product_dir[-1] != "/":
+        url_product_dir = url_product_dir + "/"
+    # Define curl command
+    # -k is required with curl > 7.71 otherwise results in "unauthorized access".
+    cmd = f"curl -k --user {username}:{password} {url_product_dir}"
+    # Run command
+    args = cmd.split()
+    process = subprocess.Popen(args, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+    stdout = process.communicate()[0].decode()
+    # Check if server is available
+    if stdout == "":
+        raise ValueError("The PPS server is currently unavailable. Sorry for the inconvenience.")
+    # Check if there are data are available
+    if stdout[0] == "<":
+        raise ValueError("No data found on PPS.")
+    else:
+        # Retrieve filepaths
+        filepaths = stdout.split()
+    # Return file paths
+    return filepaths
 
 
-def find_filepaths(
-    storage,
-    product,
-    start_time,
-    end_time,
-    product_type="RS",
-    version=None,
-    verbose=True,
-    parallel=True,
-):
+def _get_pps_file_list(url_product_dir, product, date, version, verbose=True):
     """
-    Retrieve GPM data filepaths on local disk for a specific time period and product.
+    Retrieve the filepaths of the files available on the NASA PPS server for a specific day.
+
+    The query is done using https !
+    The function does not return the full PPS server url, but the filepath
+    from the server root: i.e: '/gpmdata/2020/07/05/radar/<...>.HDF5'
+    The returned filepaths can includes more than one product !!!
+
+    Parameters
+    ----------
+    url_product_dir : str
+        The PPS product directory url.
+    product : str
+        GPM product acronym. See gpm_api.available_products() .
+    date : datetime
+        Single date for which to retrieve the data.
+    verbose : bool, optional
+        Default is False. Whether to specify when data are not available for a specific date.
+    """
+    try:
+        filepaths = __get_pps_file_list(url_product_dir)
+    except Exception as e:
+        # If url not exist, raise an error
+        if "The PPS server is currently unavailable." in str(e):
+            raise e
+        elif "No data found on PPS." in str(e):
+            # If no filepath (empty directory), print message if verbose=True
+            if verbose:
+                version_str = str(int(version))
+                msg = f"No data found on GES DISC on date {date} for product {product} (V0{version_str})"
+                print(msg)
+            filepaths = []
+        else:
+            raise ValueError("Undefined error. The error is {e}.")
+    return filepaths
+
+
+def get_pps_daily_filepaths(product, product_type, date, version, verbose=True):
+    """
+    Retrieve the complete url to the files available on the NASA PPS server for a specific day and product.
 
     Parameters
     ----------
     product : str
-        GPM product acronym. See gpm_api.available_products()
-    start_time : datetime.datetime
-        Start time.
-    end_time : datetime.datetime
-        End time.
+        GPM product acronym. See gpm_api.available_products() .
+    date : datetime
+        Single date for which to retrieve the data.
     product_type : str, optional
         GPM product type. Either 'RS' (Research) or 'NRT' (Near-Real-Time).
     version : int, optional
         GPM version of the data to retrieve if product_type = 'RS'.
     verbose : bool, optional
-        Whether to print processing details. The default is True.
-    parallel : bool, optional
-        Whether to loop over dates in parallel.
+        Whether to specify when data are not available for a specific date.
         The default is True.
-
-    Returns
-    -------
-    filepaths : list
-        List of GPM filepaths.
-
     """
-    # -------------------------------------------------------------------------.
-    ## Checks input arguments
-    storage = check_storage(storage)
-    version = check_product_version(version, product)
-    check_product_type(product_type=product_type)
-    check_product(product=product, product_type=product_type)
-    start_time, end_time = check_start_end_time(start_time, end_time)
-    check_valid_time_request(start_time, end_time, product)
-
-    # Retrieve sequence of dates
-    # - Specify start_date - 1 day to include data potentially on previous day directory
-    # --> Example granules starting at 23:XX:XX in the day before and extending to 01:XX:XX
-    start_date = datetime.datetime(start_time.year, start_time.month, start_time.day)
-    start_date = start_date - datetime.timedelta(days=1)
-    start_date = _ensure_valid_start_date(start_date=start_date, product=product)
-    end_date = datetime.datetime(end_time.year, end_time.month, end_time.day)
-    date_range = pd.date_range(start=start_date, end=end_date, freq="D")
-    dates = list(date_range.to_pydatetime())
-
-    # -------------------------------------------------------------------------.
-    # If NRT, all data lies in a single directory at PPS
-    if storage == "pps" and product_type == "NRT":
-        dates = [dates[0]]
-        parallel = False
-
-    # -------------------------------------------------------------------------.
-    # Loop over dates and retrieve available filepaths
-    if parallel:
-        list_delayed = []
-        verbose_arg = verbose
-        for i, date in enumerate(dates):
-            verbose = False if i == 0 else verbose_arg
-            del_op = dask.delayed(find_daily_filepaths)(
-                storage=storage,
-                version=version,
-                product=product,
-                product_type=product_type,
-                date=date,
-                start_time=start_time,
-                end_time=end_time,
-                verbose=verbose,
-            )
-            list_delayed.append(del_op)
-        # Get filepaths list for each date
-        list_filepaths = dask.compute(*list_delayed)
-        list_filepaths = [tpl[0] for tpl in list_filepaths]  # tpl[1] is the available version
+    # Retrieve url to product directory
+    url_product_dir = get_pps_product_directory(
+        product=product,
+        product_type=product_type,
+        date=date,
+        version=version,
+        server_type="text",
+    )
+    # Retrieve filepaths from the PPS base directory of the server
+    # - If empty: return []
+    # - Example /gpmdata/2020/07/05/radar/<...>.HDF5'
+    filepaths = _get_pps_file_list(
+        url_product_dir=url_product_dir,
+        product=product,
+        date=date,
+        version=version,
+        verbose=verbose,
+    )
+    # Define the complete url of pps filepaths
+    # Filepaths start with a "/"
+    url_data_server = _get_pps_data_server(product_type)
+    filepaths = [f"{url_data_server}{filepath}" for filepath in filepaths]
+    return filepaths
 
-    else:
-        # TODO list
-        # - start_time and end_time filtering could be done only on first and last iteration
-        # - misleading error message can occur on last iteration if end_time is close to 00:00:00
-        #   and the searched granule is in previous day directory
-        list_filepaths = []
-        verbose_arg = verbose
-        for i, date in enumerate(dates):
-            verbose = False if i == 0 else verbose_arg
-            filepaths, _ = find_daily_filepaths(
-                storage=storage,
-                version=version,
-                product=product,
-                product_type=product_type,
-                date=date,
-                start_time=start_time,
-                end_time=end_time,
-                verbose=verbose,
-            )
-            # Concatenate filepaths
-            list_filepaths += filepaths
-
-    filepaths = flatten_list(list_filepaths)
-
-    # -------------------------------------------------------------------------.
-    # Check unique version
-    # - TODO, warning if same integer but different letter
-    # - TODO: error if different integer
-
-    # -------------------------------------------------------------------------.
-    # Return sorted filepaths
-    filepaths = sorted(filepaths)
 
-    return filepaths
+def define_pps_filepath(product, product_type, date, version, filename):
+    """Define PPS filepath from filename."""
+    # Retrieve product directory url
+    url_product_dir = get_pps_product_directory(
+        product=product,
+        product_type=product_type,
+        date=date,
+        version=version,
+        server_type="data",
+    )
+    # Define PPS filepath
+    fpath = f"{url_product_dir}/{filename}"
+    return fpath
+
+
+####--------------------------------------------------------------------------.
+#################
+#### Utility ####
+#################
+
+
+def find_first_pps_granule_filepath(product: str, product_type: str, version: int) -> str:
+    """Return the PPS filepath of the first available granule."""
+    from gpm_api.io.find import find_filepaths
+
+    # Retrieve product start_time from product.yaml file.
+    start_time = get_product_info(product).get("start_time", None)
+    if start_time is None:
+        raise ValueError(f"{product} product start_time is not provided in the product.yaml file.")
+
+    # Find filepath
+    end_time = start_time + relativedelta(days=1)
+    pps_filepaths = find_filepaths(
+        storage="pps",
+        product=product,
+        start_time=start_time,
+        end_time=end_time,
+        version=version,
+        product_type=product_type,
+    )
+    if len(pps_filepaths) == 0:
+        raise ValueError(f"No PPS files found for {product} product around {start_time}.")
+    return pps_filepaths[0]
```

### Comparing `gpm_api-0.2.8/gpm_api/io/ges_disc.py` & `gpm_api-0.2.9/gpm_api/io/ges_disc.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/io/info.py` & `gpm_api-0.2.9/gpm_api/io/info.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/io/local.py` & `gpm_api-0.2.9/gpm_api/io/local.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/retrievals/retrieval_2a_radar.py` & `gpm_api-0.2.9/gpm_api/retrievals/retrieval_2a_radar.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/retrievals/routines.py` & `gpm_api-0.2.9/gpm_api/retrievals/routines.py`

 * *Files 12% similar despite different names*

```diff
@@ -46,18 +46,18 @@
 
 
 def available_retrievals(ds):
     """Decode the variables of a given GPM product."""
     # Retrieve products
     product = _infer_product(ds)
     # Define retrievals for 2A-<RADAR> products
-    if product in available_products(product_category="RADAR", product_level="2A"):
+    if product in available_products(product_categories="RADAR", product_levels="2A"):
         module_name = "gpm_api.retrievals.retrieval_2a_radar"
         return _get_available_retrievals(module_name)
-    if product in available_products(product_category="PMW", product_level="2A"):
+    if product in available_products(product_categories="PMW", product_levels="2A"):
         module_name = "gpm_api.retrievals.retrieval_2a_pmw"
         return _get_available_retrievals(module_name)
 
 
 def check_retrieval_validity(ds, retrieval):
     """Check retrieval validity."""
     product = ds.attrs["gpm_api_product"]
@@ -68,21 +68,21 @@
         )
     if retrieval not in valid_retrievals:
         raise ValueError(
             f"{retrieval} is an invalid retrieval for {product}. Available retrievals are {valid_retrievals}"
         )
 
 
-def get_retrieval_variable(ds, retrieval, *args, **kwargs):
+def get_retrieval_variable(ds, name, *args, **kwargs):
     """Compute the requested variable."""
     # Retrieve products
     product = _infer_product(ds)
 
     # Define retrievals for 2A-<RADAR> products
-    if product in available_products(product_category="RADAR", product_level="2A"):
+    if product in available_products(product_categories="RADAR", product_levels="2A"):
         module_name = "gpm_api.retrievals.retrieval_2a_radar"
-        check_retrieval_validity(ds, retrieval)
-        return _get_retrieval_function(module_name, retrieval)(ds, *args, **kwargs)
-    if product in available_products(product_category="PMW", product_level="2A"):
+        check_retrieval_validity(ds, name)
+        return _get_retrieval_function(module_name, name)(ds, *args, **kwargs)
+    if product in available_products(product_categories="PMW", product_levels="2A"):
         module_name = "gpm_api.^retrievals.retrieval_2a_pmw"
-        check_retrieval_validity(ds, retrieval)
-        return _get_retrieval_function(module_name, retrieval)(ds, *args, **kwargs)
+        check_retrieval_validity(ds, name)
+        return _get_retrieval_function(module_name, name)(ds, *args, **kwargs)
```

### Comparing `gpm_api-0.2.8/gpm_api/scripts/download_gpm_daily_data.py` & `gpm_api-0.2.9/gpm_api/scripts/download_gpm_monthly_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 """
-Created on Mon Mar 13 11:48:22 2023
+Created on Mon Mar 13 12:11:27 2023
 
 @author: ghiggi
 """
 import sys
 import warnings
 
 import click
@@ -15,62 +15,55 @@
 
 # -------------------------------------------------------------------------.
 # Click Command Line Interface decorator
 @click.command()
 @click.argument("product", type=str)
 @click.argument("year", type=int)
 @click.argument("month", type=int)
-@click.argument("day", type=int)
 @click.option("--product_type", type=str, show_default=True, default="RS")
 @click.option("--storage", type=str, show_default=True, default="pps")
 @click.option("--version", type=int, show_default=True, default=None)
 @click.option("--n_threads", type=int, default=4)
 @click.option("--transfer_tool", type=str, default="curl")
 @click.option("--progress_bar", type=bool, default=False)
 @click.option("--force_download", type=bool, default=False)
 @click.option("--check_integrity", type=bool, default=True)
 @click.option("--remove_corrupted", type=bool, default=True)
 @click.option("--verbose", type=bool, default=True)
 @click.option("--retry", type=int, default=1)
-def download_gpm_daily_data(
+def download_gpm_monthly_data(
     product,
     year,
     month,
-    day,
     product_type="RS",
-    version=None,
     storage="pps",
+    version=None,
     n_threads=4,
     transfer_tool="curl",
     progress_bar=False,
     force_download=False,
     check_integrity=True,
     remove_corrupted=True,
     verbose=True,
     retry=1,
 ):
-    """Download the GPM product for a specific date."""
-    from gpm_api.io.download import download_daily_data
+    """Download the GPM product for a specific month."""
+    from gpm_api.io.download import download_monthly_data
 
-    _ = download_daily_data(
+    _ = download_monthly_data(
         product=product,
         year=year,
         month=month,
-        day=day,
         product_type=product_type,
         version=version,
         storage=storage,
         n_threads=n_threads,
         transfer_tool=transfer_tool,
         progress_bar=progress_bar,
         force_download=force_download,
         check_integrity=check_integrity,
         remove_corrupted=remove_corrupted,
         verbose=verbose,
         retry=retry,
     )
 
-    return
-
-
-if __name__ == "__main__":
-    download_gpm_daily_data()
+    return None
```

### Comparing `gpm_api-0.2.8/gpm_api/scripts/download_gpm_files.py` & `gpm_api-0.2.9/gpm_api/scripts/download_gpm_files.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,12 +51,8 @@
         force_download=force_download,
         remove_corrupted=remove_corrupted,
         progress_bar=progress_bar,
         verbose=verbose,
         retry=retry,
     )
 
-    return
-
-
-if __name__ == "__main__":
-    download_gpm_files()
+    return None
```

### Comparing `gpm_api-0.2.8/gpm_api/scripts/download_gpm_monthly_data.py` & `gpm_api-0.2.9/gpm_api/scripts/download_gpm_daily_data.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 """
-Created on Mon Mar 13 12:11:27 2023
+Created on Mon Mar 13 11:48:22 2023
 
 @author: ghiggi
 """
 import sys
 import warnings
 
 import click
@@ -15,59 +15,58 @@
 
 # -------------------------------------------------------------------------.
 # Click Command Line Interface decorator
 @click.command()
 @click.argument("product", type=str)
 @click.argument("year", type=int)
 @click.argument("month", type=int)
+@click.argument("day", type=int)
 @click.option("--product_type", type=str, show_default=True, default="RS")
 @click.option("--storage", type=str, show_default=True, default="pps")
 @click.option("--version", type=int, show_default=True, default=None)
 @click.option("--n_threads", type=int, default=4)
 @click.option("--transfer_tool", type=str, default="curl")
 @click.option("--progress_bar", type=bool, default=False)
 @click.option("--force_download", type=bool, default=False)
 @click.option("--check_integrity", type=bool, default=True)
 @click.option("--remove_corrupted", type=bool, default=True)
 @click.option("--verbose", type=bool, default=True)
 @click.option("--retry", type=int, default=1)
-def download_gpm_monthly_data(
+def download_gpm_daily_data(
     product,
     year,
     month,
+    day,
     product_type="RS",
-    storage="pps",
     version=None,
+    storage="pps",
     n_threads=4,
     transfer_tool="curl",
     progress_bar=False,
     force_download=False,
     check_integrity=True,
     remove_corrupted=True,
     verbose=True,
     retry=1,
 ):
-    """Download the GPM product for a specific month."""
-    from gpm_api.io.download import download_monthly_data
+    """Download the GPM product for a specific date."""
+    from gpm_api.io.download import download_daily_data
 
-    _ = download_monthly_data(
+    _ = download_daily_data(
         product=product,
         year=year,
         month=month,
+        day=day,
         product_type=product_type,
         version=version,
         storage=storage,
         n_threads=n_threads,
         transfer_tool=transfer_tool,
         progress_bar=progress_bar,
         force_download=force_download,
         check_integrity=check_integrity,
         remove_corrupted=remove_corrupted,
         verbose=verbose,
         retry=retry,
     )
 
-    return
-
-
-if __name__ == "__main__":
-    download_gpm_monthly_data()
+    return None
```

### Comparing `gpm_api-0.2.8/gpm_api/tests/0_tmp/dataset/0_create_test_files.py` & `gpm_api-0.2.9/gpm_api/tests/0_tmp/dataset/0_create_test_files.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/tests/0_tmp/dataset/dev_encoding.py` & `gpm_api-0.2.9/gpm_api/tests/0_tmp/dataset/dev_encoding.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/tests/0_tmp/dataset/test_attrs_decoding.py` & `gpm_api-0.2.9/gpm_api/tests/0_tmp/dataset/test_attrs_decoding.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/tests/0_tmp/dataset/test_crs_cf.py` & `gpm_api-0.2.9/gpm_api/tests/0_tmp/dataset/test_crs_cf.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/tests/0_tmp/dataset/test_dataset_concatenation.py` & `gpm_api-0.2.9/gpm_api/tests/0_tmp/dataset/test_dataset_concatenation.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/tests/0_tmp/dataset/test_dataset_regularity.py` & `gpm_api-0.2.9/gpm_api/tests/0_tmp/dataset/test_dataset_regularity.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/tests/0_tmp/dataset/test_dataset_valid_geolocation.py` & `gpm_api-0.2.9/gpm_api/tests/0_tmp/dataset/test_dataset_valid_geolocation.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/tests/0_tmp/dataset/test_decode_2a_dpr.py` & `gpm_api-0.2.9/gpm_api/tests/0_tmp/dataset/test_decode_2a_dpr.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/tests/0_tmp/dataset/test_granule_creation.py` & `gpm_api-0.2.9/gpm_api/tests/0_tmp/dataset/test_granule_creation.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/tests/0_tmp/dataset/test_parallel_reading.py` & `gpm_api-0.2.9/gpm_api/tests/0_tmp/dataset/test_parallel_reading.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/tests/0_tmp/dataset/test_pmw_channel_coords.py` & `gpm_api-0.2.9/gpm_api/tests/0_tmp/dataset/test_pmw_channel_coords.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/tests/0_tmp/dataset/test_retrievals.py` & `gpm_api-0.2.9/gpm_api/tests/0_tmp/dataset/test_retrievals.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/tests/0_tmp/dataset/test_unvalid_coordinates.py` & `gpm_api-0.2.9/gpm_api/tests/0_tmp/dataset/test_unvalid_coordinates.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/tests/0_tmp/io/test_archive.py` & `gpm_api-0.2.9/gpm_api/tests/0_tmp/io/test_archive.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/tests/0_tmp/io/test_dataset.py` & `gpm_api-0.2.9/gpm_api/tests/0_tmp/io/test_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,18 +38,18 @@
     "2A-GMI",
     "2B-GPM-CORRA",
     "2B-GPM-CSH",
     "2A-GPM-SLH",
 ]
 products = ["2B-TRMM-CORRA", "2B-TRMM-CSH", "2A-TRMM-SLH", "1B-TMI", "1C-TMI", "2A-ENV-PR", "2A-PR"]
 
-products = gpm_api.available_products(product_category="CMB")
-products = gpm_api.available_products(product_category="IMERG")
-products = gpm_api.available_products(product_category="RADAR")
-products = gpm_api.available_products(product_category="PMW")
+products = gpm_api.available_products(product_categories="CMB")
+products = gpm_api.available_products(product_categories="IMERG")
+products = gpm_api.available_products(product_categories="RADAR")
+products = gpm_api.available_products(product_categories="PMW")
 
 
 start_time = datetime.datetime.strptime("2018-07-01 08:00:00", "%Y-%m-%d %H:%M:%S")
 end_time = datetime.datetime.strptime("2018-07-01 09:00:00", "%Y-%m-%d %H:%M:%S")
 product_type = "RS"
 
 #### Download products
```

### Comparing `gpm_api-0.2.8/gpm_api/tests/0_tmp/io/test_disk.py` & `gpm_api-0.2.9/gpm_api/tests/0_tmp/io/test_disk.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/tests/0_tmp/io/test_download.py` & `gpm_api-0.2.9/gpm_api/tests/0_tmp/io/test_download.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/tests/0_tmp/io/test_downloads.py` & `gpm_api-0.2.9/gpm_api/tests/0_tmp/io/test_downloads.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import datetime
 import numpy as np
 
 ##-----------------------------------------------------------------------------.
 ## Retrieve RS data
 version = 7
 product_type = "RS"
-products = gpm_api.available_products(product_type="RS")()
+products = gpm_api.available_products(product_types="RS")()
 
 # Only GPM
 start_time = datetime.datetime.strptime("2020-08-09 15:00:00", "%Y-%m-%d %H:%M:%S")
 end_time = datetime.datetime.strptime("2020-08-09 17:00:00", "%Y-%m-%d %H:%M:%S")
 
 # Both GPM-TRMM
 start_time = datetime.datetime.strptime("2014-08-09 00:00:00", "%Y-%m-%d %H:%M:%S")
@@ -34,15 +34,15 @@
         verbose=True,
     )
 
 ##-----------------------------------------------------------------------------.
 ## Retrieve NRT data
 version = 6
 product_type = "NRT"
-products = gpm_api.available_products(product_type="NRT")
+products = gpm_api.available_products(product_types="NRT")
 
 date = datetime.date.fromisoformat("2020-08-17")
 
 start_time = datetime.datetime.strptime("2020-08-17 00:00:00", "%Y-%m-%d %H:%M:%S")
 end_time = datetime.datetime.strptime("2020-08-17 04:00:00", "%Y-%m-%d %H:%M:%S")
 
 for product in products:
```

### Comparing `gpm_api-0.2.8/gpm_api/tests/0_tmp/io/test_filter.py` & `gpm_api-0.2.9/gpm_api/tests/0_tmp/io/test_filter.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/tests/0_tmp/io/test_find_filters.py` & `gpm_api-0.2.9/gpm_api/tests/0_tmp/io/test_find_filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,29 +17,29 @@
     filter_by_time,
 )
 from gpm_api.io.pps import find_pps_daily_filepaths
 
 # -------------------------------------------------------------------------.
 version = 7
 product_type = "RS"
-products = gpm_api.available_products(product_type=product_type)
+products = gpm_api.available_products(product_types=product_type)
 
 date = datetime.date.fromisoformat("2020-08-17")
 start_time = datetime.datetime.strptime("2020-08-17 00:00:00", "%Y-%m-%d %H:%M:%S")
 end_time = datetime.datetime.strptime("2020-08-17 04:00:00", "%Y-%m-%d %H:%M:%S")
 
 product = "2A-DPR"
 flag_first_date = False
 verbose = True
 force_download = False
 
 # -------------------------------------------------------------------------.
 date = check_date(date)
-check_product_type(product_type=product_type)
-check_product(product=product, product_type=product_type)
+product_type = check_product_type(product_type=product_type)
+product = check_product(product=product, product_type=product_type)
 
 
 # -------------------------------------------------------------------------.
 ## Retrieve the list of files available on NASA PPS server
 (pps_fpaths, local_filepaths) = find_pps_daily_filepaths(
     product=product,
     product_type=product_type,
```

### Comparing `gpm_api-0.2.8/gpm_api/tests/0_tmp/io/test_info.py` & `gpm_api-0.2.9/gpm_api/tests/0_tmp/io/test_info.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/tests/0_tmp/io/test_pps.py` & `gpm_api-0.2.9/gpm_api/tests/0_tmp/io/test_pps.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/tests/0_tmp/visualization/test_plot_multiorbit_gmi.py` & `gpm_api-0.2.9/gpm_api/tests/0_tmp/visualization/test_plot_multiorbit_gmi.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/tests/0_tmp/visualization/test_plot_multiorbit_pmw_polar.py` & `gpm_api-0.2.9/gpm_api/tests/0_tmp/visualization/test_plot_multiorbit_pmw_polar.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/tests/0_tmp/visualization/test_plot_orbit_pmw_custom_kwargs.py` & `gpm_api-0.2.9/gpm_api/tests/0_tmp/visualization/test_plot_orbit_pmw_custom_kwargs.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/tests/conftest.py` & `gpm_api-0.2.9/gpm_api/tests/conftest.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import pytest
 import datetime
 from typing import Any, List, Dict, Tuple, Iterable
 from gpm_api.io.products import get_info_dict, available_products
+from gpm_api.utils import geospatial
 import posixpath as pxp
 import ntpath as ntp
 import gpm_api.configs
 import os
+from pytest_mock import MockerFixture
 from unittest.mock import patch
 
 
 @pytest.fixture(scope="session", autouse=True)
 def mock_configuration() -> Iterable[Dict[str, str]]:
     """Patch the user configuration for entire session
 
@@ -56,32 +58,33 @@
 
     return list(set([info_dict["product_category"] for info_dict in get_info_dict().values()]))
 
 
 @pytest.fixture
 def product_levels() -> List[str]:
     """Return a list of product levels from the info dict"""
+    from gpm_api.io.products import get_available_product_levels
 
-    # Available in gpm_api.io.checks.check_product_level()
-    return ["1A", "1B", "1C", "2A", "2B"]
+    return get_available_product_levels(full=False)  #  ["1A", "1B", "1C", "2A", "2B", "3B"]
 
 
 @pytest.fixture
 def versions() -> List[int]:
     """Return a list of versions"""
+    from gpm_api.io.products import get_available_versions
 
-    # Available in gpm_api.io.checks.check_version()
-    return [4, 5, 6, 7]
+    return get_available_versions()
 
 
 @pytest.fixture
 def products() -> List[str]:
     """Return a list of all products regardless of type"""
+    from gpm_api.io.products import get_available_products
 
-    return available_products()
+    return get_available_products()
 
 
 @pytest.fixture
 def product_info() -> Dict[str, dict]:
     """Return a dictionary of product info"""
 
     return get_info_dict()
@@ -381,7 +384,40 @@
 
 
 @pytest.fixture
 def local_filepaths_windows(local_filepaths) -> List[str]:
     """Return the local filepath list as windows paths"""
 
     return [ntp.join(*path) for path in local_filepaths]
+
+
+@pytest.fixture
+def set_is_orbit_to_true(
+    mocker: MockerFixture,
+) -> None:
+    mocker.patch("gpm_api.checks.is_orbit", return_value=True)
+    mocker.patch("gpm_api.checks.is_grid", return_value=False)
+    mocker.patch("gpm_api.utils.checks.is_orbit", return_value=True)
+    mocker.patch("gpm_api.utils.checks.is_grid", return_value=False)
+
+
+@pytest.fixture
+def set_is_grid_to_true(
+    mocker: MockerFixture,
+) -> None:
+    mocker.patch("gpm_api.checks.is_grid", return_value=True)
+    mocker.patch("gpm_api.checks.is_orbit", return_value=False)
+    mocker.patch("gpm_api.utils.checks.is_grid", return_value=True)
+    mocker.patch("gpm_api.utils.checks.is_orbit", return_value=False)
+
+
+ExtentDictionary = Dict[str, Tuple[float, float, float, float]]
+
+
+@pytest.fixture
+def country_extent_dictionary() -> ExtentDictionary:
+    return geospatial._get_country_extent_dictionary()
+
+
+@pytest.fixture
+def continent_extent_dictionary() -> ExtentDictionary:
+    return geospatial._get_continent_extent_dictionary()
```

### Comparing `gpm_api-0.2.8/gpm_api/tests/test_dataset/conftest.py` & `gpm_api-0.2.9/gpm_api/tests/test_dataset/conftest.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/tests/test_dataset/decoding/test_attrs.py` & `gpm_api-0.2.9/gpm_api/tests/test_dataset/decoding/test_attrs.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/tests/test_dataset/decoding/test_coordinates.py` & `gpm_api-0.2.9/gpm_api/tests/test_dataset/decoding/test_coordinates.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/tests/test_dataset/test_attrs.py` & `gpm_api-0.2.9/gpm_api/tests/test_dataset/test_attrs.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/tests/test_dataset/test_coords.py` & `gpm_api-0.2.9/gpm_api/tests/test_dataset/test_coords.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/tests/test_dataset/test_crs.py` & `gpm_api-0.2.9/gpm_api/tests/test_dataset/test_crs.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/tests/test_dataset/test_dimensions.py` & `gpm_api-0.2.9/gpm_api/tests/test_dataset/test_dimensions.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/tests/test_dataset/test_granule.py` & `gpm_api-0.2.9/gpm_api/tests/test_dataset/test_granule.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/tests/test_dataset/test_granule_files.py` & `gpm_api-0.2.9/gpm_api/tests/test_dataset/test_granule_files.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/tests/test_dataset/test_groups_variables.py` & `gpm_api-0.2.9/gpm_api/tests/test_dataset/test_groups_variables.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/tests/test_io/test_data_integrity.py` & `gpm_api-0.2.9/gpm_api/tests/test_io/test_data_integrity.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/tests/test_io/test_disk.py` & `gpm_api-0.2.9/gpm_api/tests/test_io/test_disk.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
                 dir_pattern = local._get_local_dir_pattern(
                     product,
                     product_type,
                     version,
                 )
 
                 # Work only on product if product_type are compatible
-                if product in available_products(product_type=product_type):
+                if product in available_products(product_types=product_type):
                     product_category = get_product_category(product)
                     if product_type == "NRT":
                         assert "V0" not in dir_pattern
                         assert dir_pattern == os.path.join(
                             "GPM", product_type, product_category, product
                         )
                     elif product_type == "RS":
@@ -59,15 +59,15 @@
                     product=product,
                     product_type=product_type,
                     version=version,
                     date=date,
                 )
 
                 # Work only on product if product_type are compatible
-                if product in available_products(product_type=product_type):
+                if product in available_products(product_types=product_type):
                     product_category = get_product_category(product)
                     if product_type == "NRT":
                         assert "V0" not in dir_path
                         assert dir_path == os.path.join(
                             base_dir,
                             os.path.join("GPM", product_type, product_category, product),
                             date.strftime("%Y"),
```

### Comparing `gpm_api-0.2.8/gpm_api/tests/test_io/test_download.py` & `gpm_api-0.2.9/gpm_api/tests/test_io/test_download.py`

 * *Files 0% similar despite different names*

```diff
@@ -212,15 +212,15 @@
 
         It may be useful as boilerplate to increase the number of tests here in the
         future.
         """
 
         # Assume files pass file integrity check by mocking return as empty
         for product_type in product_types:
-            for product in available_products(product_type=product_type):
+            for product in available_products(product_types=product_type):
                 start_time = get_product_start_time(product)
                 if start_time is None:
                     continue
                 res = dl.download_archive(
                     product=product,
                     start_time=start_time,
                     end_time=start_time + datetime.timedelta(hours=1),
@@ -272,15 +272,15 @@
     mocker.patch.object(dl, "run", autospec=True, return_value=None)
     mocker.patch.object(dl, "find_daily_filepaths", autospec=True, return_value=([], versions))
 
     # Mocking empty responses will cause a DownloadWarning. Test that it is raised
     with pytest.warns(GPMDownloadWarning):
         for version in versions:
             for product_type in product_types:
-                for product in available_products(product_type=product_type):
+                for product in available_products(product_types=product_type):
                     dl._download_daily_data(
                         storage=storage,
                         date=datetime.datetime(2022, 9, 7, 12, 0, 0),
                         version=version,
                         product=product,
                         product_type=product_type,
                         start_time=None,
```

### Comparing `gpm_api-0.2.8/gpm_api/tests/test_io/test_filter.py` & `gpm_api-0.2.9/gpm_api/tests/test_io/test_filter.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 from gpm_api.io import filter
 from typing import Dict, Any, List
 import datetime
+from gpm_api.io.filter import (
+    filter_by_product,
+    filter_by_time,
+    filter_by_version,
+    is_granule_within_time,
+    filter_filepaths,
+)
 
 
 def test_granule_within_time() -> None:
     """Test is_granule_within_time()"""
 
     # Set a file time 01.01.14 01:00 to 04:00 (start, end)
     file_time = ("2014-01-01T01:00:00Z", "2014-01-01T04:00:00Z")
@@ -14,15 +21,15 @@
         ("2014-01-01T00:00:00Z", "2014-01-01T05:00:00Z"),  # Crosses start
         ("2014-01-01T02:00:00Z", "2014-01-01T03:00:00Z"),  # Within
         ("2014-01-01T03:00:00Z", "2014-01-01T05:00:00Z"),  # Crosses end
     ]
 
     for start_time, end_time in true_assumptions:
         assert (
-            filter.is_granule_within_time(
+            is_granule_within_time(
                 start_time=start_time,
                 end_time=end_time,
                 file_start_time=file_time[0],
                 file_end_time=file_time[1],
             )
             is True
         )
@@ -34,15 +41,15 @@
         ("2014-01-01T00:00:00Z", "2014-01-01T00:59:59Z"),  # Before start
         ("2014-01-01T05:00:00Z", "2014-01-01T06:00:00Z"),  # After end
         ("2014-01-01T04:00:00Z", "2014-01-01T05:00:00Z"),  # Starts at end
     ]
 
     for start_time, end_time in false_assumptions:
         assert (
-            filter.is_granule_within_time(
+            is_granule_within_time(
                 start_time=start_time,
                 end_time=end_time,
                 file_start_time=file_time[0],
                 file_end_time=file_time[1],
             )
             is False
         )
@@ -63,42 +70,42 @@
             if (
                 info_dict["year"] == 2019
                 and info_dict["product"] == self.product
                 and info_dict["version"] == 7
             ):
                 count_2019 += 1
 
-        res = filter.filter_filepaths(
+        res = filter_filepaths(
             filepaths=list(remote_filepaths.keys()),
             product=self.product,
             start_time=datetime.datetime(2019, 1, 1),
             end_time=datetime.datetime(2019, 12, 31, 23, 59, 59),
             version=7,
         )
 
         assert len(res) == count_2019
 
     def test_none_filepath(
         self,
         remote_filepaths: Dict[str, Dict[str, Any]],
     ) -> None:
-        res = filter.filter_filepaths(
+        res = filter_filepaths(
             filepaths=None,
             product=self.product,
             start_time=datetime.datetime(2019, 1, 1),
             end_time=datetime.datetime(2019, 12, 31, 23, 59, 59),
             version=7,
         )
         assert res == []
 
     def test_empty_filepath_list(
         self,
         remote_filepaths: Dict[str, Dict[str, Any]],
     ) -> None:
-        res = filter.filter_filepaths(
+        res = filter_filepaths(
             filepaths=[],
             product=self.product,
             start_time=datetime.datetime(2019, 1, 1),
             end_time=datetime.datetime(2019, 12, 31, 23, 59, 59),
             version=7,
         )
         assert res == []
@@ -107,193 +114,174 @@
         self,
         remote_filepaths: Dict[str, Dict[str, Any]],
     ) -> None:
         count_until_2019 = 0
         for remote_filepath, info_dict in remote_filepaths.items():
             if info_dict["year"] == 2019 and info_dict["product"] == self.product:
                 count_until_2019 += 1
-        res = filter.filter_filepaths(
+        res = filter_filepaths(
             filepaths=list(remote_filepaths.keys()),
             product=self.product,
             start_time=None,
             end_time=datetime.datetime(2019, 12, 31, 23, 59, 59),
             version=7,
         )
 
         assert len(res) == count_until_2019
 
-    def test_empty_end_time(
-        self,
-        remote_filepaths: Dict[str, Dict[str, Any]],
-    ) -> None:
+    def test_empty_end_time(self, remote_filepaths: Dict[str, Dict[str, Any]]) -> None:
         """Test empty end time (Error as time given (datetime.datetime.now())
         requires date to be less than now() in supportive
         function checks.check_start_end_time)"""
 
         count_from_2019 = 0
         for remote_filepath, info_dict in remote_filepaths.items():
             if info_dict["year"] >= 2019 and info_dict["product"] == self.product:
                 count_from_2019 += 1
 
-        res = filter.filter_filepaths(
+        res = filter_filepaths(
             filepaths=list(remote_filepaths.keys()),
             product=self.product,
             start_time=datetime.datetime(2019, 1, 1),
             end_time=None,
             version=7,
         )
         assert len(res) == count_from_2019
 
     def test_unmatched_version(
         self,
         remote_filepaths: Dict[str, Dict[str, Any]],
     ) -> None:
-        res = filter.filter_filepaths(
+        res = filter_filepaths(
             filepaths=list(remote_filepaths.keys()),
             product=self.product,
             start_time=datetime.datetime(2019, 1, 1),
             end_time=datetime.datetime(2019, 12, 31, 23, 59, 59),
             version=0,
         )
         assert res == []
 
     def test_unmatched_product(
         self,
         remote_filepaths: Dict[str, Dict[str, Any]],
     ) -> None:
-        res = filter.filter_filepaths(
+        res = filter_filepaths(
             filepaths=list(remote_filepaths.keys()),
             product="1A-GMI",
             start_time=datetime.datetime(2019, 1, 1),
             end_time=datetime.datetime(2019, 12, 31, 23, 59, 59),
             version=7,
         )
         assert res == []
 
 
-def test_filter_by_time(
-    remote_filepaths: Dict[str, Dict[str, Any]],
-) -> None:
+def test_filter_by_time(remote_filepaths: Dict[str, Dict[str, Any]]) -> None:
     """Test filter filepaths"""
 
     # Test year filtering
     # Count and assert 2019 paths
     count_2019 = 0
     for remote_filepath, info_dict in remote_filepaths.items():
         if info_dict["year"] == 2019:
             count_2019 += 1
 
-    res = filter.filter_by_time(
+    res = filter_by_time(
         filepaths=list(remote_filepaths.keys()),
         start_time=datetime.datetime(2019, 1, 1),
         end_time=datetime.datetime(2019, 12, 31, 23, 59, 59),
     )
 
     assert len(res) == count_2019
 
     # Test None filepaths
-    res = filter.filter_by_time(
+    res = filter_by_time(
         filepaths=None,
         start_time=datetime.datetime(2019, 1, 1),
         end_time=datetime.datetime(2019, 12, 31, 23, 59, 59),
     )
 
     assert res == []
 
     # Test empty filepath list
-    res = filter.filter_by_time(
+    res = filter_by_time(
         filepaths=[],
         start_time=datetime.datetime(2019, 1, 1),
         end_time=datetime.datetime(2019, 12, 31, 23, 59, 59),
     )
 
     assert res == []
 
     # Test empty start time
     count_until_2019 = 0
     for remote_filepath, info_dict in remote_filepaths.items():
         if info_dict["year"] == 2019:
             count_until_2019 += 1
-    res = filter.filter_by_time(
+    res = filter_by_time(
         filepaths=list(remote_filepaths.keys()),
         start_time=None,
         end_time=datetime.datetime(2019, 12, 31, 23, 59, 59),
     )
 
     assert len(res) == count_until_2019
 
     # Test empty end time (should default to utcnow which will technically be
     # in the past by the time it gets to the function)
     count_from_2019 = 0
     for remote_filepath, info_dict in remote_filepaths.items():
         if info_dict["year"] >= 2019:
             count_from_2019 += 1
 
-    res = filter.filter_by_time(
+    res = filter_by_time(
         filepaths=list(remote_filepaths.keys()),
         start_time=datetime.datetime(2019, 1, 1),
         end_time=None,
     )
 
     # Test granule starting on previous day
     count_previous_day = 0
     for remote_filepath, info_dict in remote_filepaths.items():
         if info_dict["start_time"].day != info_dict["end_time"].day:
             count_previous_day += 1
 
-    res = filter.filter_by_time(
+    res = filter_by_time(
         filepaths=list(remote_filepaths.keys()),
         start_time=datetime.datetime(2020, 7, 6, 0, 0, 20),
         end_time=datetime.datetime(2020, 7, 6, 0, 0, 30),
     )
 
     assert len(res) == count_previous_day
 
 
 def test_filter_by_product(
     remote_filepaths: Dict[str, Dict[str, Any]],
-    products: List[str],
 ) -> None:
     """Test filter by product
 
     Use predefined remote_filepaths list to validate filter"""
 
     # Check 2A-DPR
     products_2A_DPR = 0
     for remote_filepath, info_dict in remote_filepaths.items():
         # Ensure exists in remote_filepath list
         if info_dict["product"] == "2A-DPR":
             products_2A_DPR += 1
 
     assert products_2A_DPR > 0, "The test remote_filepaths fixture does not contain expected value"
 
-    filtered_filepaths = filter.filter_by_product(
+    filtered_filepaths = filter_by_product(
         filepaths=list(remote_filepaths.keys()),
         product="2A-DPR",
     )
-
     assert len(filtered_filepaths) == products_2A_DPR
 
     # Test None filepath
-    assert (
-        filter.filter_by_product(
-            filepaths=None,
-            product="2A-DPR",
-        )
-        == []
-    )
+    assert filter_by_product(filepaths=None, product="2A-DPR") == []
 
     # Test empty filepaths
-    assert (
-        filter.filter_by_product(
-            filepaths=[],
-            product="2A-DPR",
-        )
-        == []
-    )
+    assert filter_by_product(filepaths=[], product="2A-DPR") == []
 
 
 def test_filter_by_version(
     remote_filepaths: Dict[str, Dict[str, Any]],
     versions: List[int],
 ) -> None:
     """Test filtering by version"""
@@ -303,18 +291,18 @@
         paths_with_matching_version = 0
         for remote_filepath, info_dict in remote_filepaths.items():
             if info_dict["version"] == version:
                 paths_with_matching_version += 1
 
         # Only test if there are matching versions in remote_filepaths
         if paths_with_matching_version > 0:
-            res = filter.filter_by_version(list(remote_filepaths.keys()), version)
+            res = filter_by_version(list(remote_filepaths.keys()), version)
 
             assert len(res) == paths_with_matching_version
 
         # Test None filepaths
-        res = filter.filter_by_version(None, version)
+        res = filter_by_version(None, version)
         assert res == []
 
         # Test empty filepaths list
-        res = filter.filter_by_version([], version)
+        res = filter_by_version([], version)
         assert res == []
```

### Comparing `gpm_api-0.2.8/gpm_api/tests/test_io/test_find.py` & `gpm_api-0.2.9/gpm_api/tests/test_io/test_find.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,20 @@
 
 import pytest
 from pytest_mock.plugin import MockerFixture
 
 from gpm_api.io import find
 from gpm_api.io.products import available_products
 from gpm_api.utils.warnings import GPMDownloadWarning
+from gpm_api.io.find import (
+    _get_all_daily_filepaths,
+    _check_correct_version,
+    find_daily_filepaths,
+    find_filepaths,
+)
 
 
 class TestGetDailyFilepaths:
     """Test _get_all_daily_filepaths"""
 
     date = datetime.datetime(2020, 12, 31)
     mock_filenames = [
@@ -22,15 +28,15 @@
     def test_local_non_existent_files(
         self,
     ) -> None:
         """Test _get_all_daily_filepaths for "local" storage with non-existent files"""
 
         storage = "local"
 
-        returned_filepaths = find._get_all_daily_filepaths(
+        returned_filepaths = _get_all_daily_filepaths(
             storage=storage,
             date=self.date,
             product="1C-GMI",
             product_type="RS",
             version=7,
             verbose=True,
         )
@@ -49,20 +55,20 @@
 
         # Mock os.listdir to return a list of filenames
         mocker.patch("gpm_api.io.local.os.listdir", return_value=self.mock_filenames)
         mocker.patch("gpm_api.io.local.os.path.exists", return_value=True)
 
         # Test with existing files (mocked)
         for product_type in ["RS", "NRT"]:
-            for product in available_products(product_type=product_type):
+            for product in available_products(product_types=product_type):
                 info = product_info[product]
                 version = info["available_versions"][-1]
                 product_category = info["product_category"]
 
-                returned_filepaths = find._get_all_daily_filepaths(
+                returned_filepaths = _get_all_daily_filepaths(
                     storage=storage,
                     date=self.date,
                     product=product,
                     product_type=product_type,
                     version=version,
                     verbose=True,
                 )
@@ -118,19 +124,19 @@
     ) -> None:
         """Test _get_all_daily_filepaths for "pps" storage with RS version 7 products"""
 
         storage = "pps"
         product_type = "RS"
         version = 7
 
-        for product in available_products(product_type=product_type, version=version):
+        for product in available_products(product_types=product_type, versions=version):
             info = product_info[product]
             pps_dir = info["pps_rs_dir"]
 
-            returned_filepaths = find._get_all_daily_filepaths(
+            returned_filepaths = _get_all_daily_filepaths(
                 storage=storage,
                 date=self.date,
                 product=product,
                 product_type=product_type,
                 version=version,
                 verbose=True,
             )
@@ -146,23 +152,23 @@
         product_info: Dict[str, dict],
     ) -> None:
         """Test _get_all_daily_filepaths for "pps" storage with RS lower version products"""
 
         storage = "pps"
         product_type = "RS"
 
-        for product in available_products(product_type=product_type):
+        for product in available_products(product_types=product_type):
             info = product_info[product]
             pps_dir = info["pps_rs_dir"]
 
             for version in info["available_versions"]:
                 if version == 7:
                     continue
 
-                returned_filepaths = find._get_all_daily_filepaths(
+                returned_filepaths = _get_all_daily_filepaths(
                     storage=storage,
                     date=self.date,
                     product=product,
                     product_type=product_type,
                     version=version,
                     verbose=True,
                 )
@@ -178,23 +184,23 @@
         product_info: Dict[str, dict],
     ) -> None:
         """Test _get_all_daily_filepaths for "pps" storage with NRT products (except IMERG)"""
 
         storage = "pps"
         product_type = "NRT"
 
-        for product in available_products(product_type=product_type):
+        for product in available_products(product_types=product_type):
             info = product_info[product]
             if info["product_category"] == "IMERG":
                 continue
 
             version = info["available_versions"][-1]
             pps_dir = info["pps_nrt_dir"]
 
-            returned_filepaths = find._get_all_daily_filepaths(
+            returned_filepaths = _get_all_daily_filepaths(
                 storage=storage,
                 date=self.date,
                 product=product,
                 product_type=product_type,
                 version=version,
                 verbose=True,
             )
@@ -212,21 +218,21 @@
         """Test _get_all_daily_filepaths for "pps" storage with NRT IMERG products"""
 
         storage = "pps"
         product_type = "NRT"
         product_category = "IMERG"
 
         for product in available_products(
-            product_type=product_type, product_category=product_category
+            product_types=product_type, product_categories=product_category
         ):
             info = product_info[product]
             version = info["available_versions"][-1]
             pps_dir = info["pps_nrt_dir"]
 
-            returned_filepaths = find._get_all_daily_filepaths(
+            returned_filepaths = _get_all_daily_filepaths(
                 storage=storage,
                 date=self.date,
                 product=product,
                 product_type=product_type,
                 version=version,
                 verbose=True,
             )
@@ -248,15 +254,15 @@
         # Mock missing dirs
         del info["pps_rs_dir"]
         del info["pps_nrt_dir"]
         mocker.patch("gpm_api.io.products.get_product_info", return_value=info)
 
         for product_type in ["RS", "NRT"]:
             with pytest.raises(ValueError):
-                find._get_all_daily_filepaths(
+                _get_all_daily_filepaths(
                     storage=storage,
                     date=self.date,
                     product=product,
                     product_type=product_type,
                     version=version,
                     verbose=True,
                 )
@@ -288,15 +294,15 @@
 
         for product, info in product_info.items():
             version = info["available_versions"][-1]
             ges_disc_dir = info["ges_disc_dir"]
             if ges_disc_dir is None:
                 continue
 
-            returned_filepaths = find._get_all_daily_filepaths(
+            returned_filepaths = _get_all_daily_filepaths(
                 storage=storage,
                 date=self.date,
                 product=product,
                 product_type=None,
                 version=version,
                 verbose=True,
             )
@@ -316,15 +322,15 @@
 
         storage = "invalid"
         product = "1C-GMI"
         product_type = "RS"
         version = 7
 
         with pytest.raises(ValueError):
-            find._get_all_daily_filepaths(
+            _get_all_daily_filepaths(
                 storage=storage,
                 date=self.date,
                 product=product,
                 product_type=product_type,
                 version=version,
                 verbose=True,
             )
@@ -339,35 +345,35 @@
     product = "2A-DPR"
     version = 7
     filepath_template = "2A.GPM.DPR.V9-20211125.20200705-S170044-E183317.036092.V0{}A.HDF5"
 
     # Test correct version
     files_version = [7] * 3
     filepaths = [filepath_template.format(v) for v in files_version]
-    returned_filepaths, returned_version = find._check_correct_version(
+    returned_filepaths, returned_version = _check_correct_version(
         filepaths=filepaths, product=product, version=version
     )
     assert returned_filepaths == filepaths
     assert returned_version == version
 
     # Test incorrect version
     files_version = [6] * 3
     filepaths = [filepath_template.format(v) for v in files_version]
     with pytest.raises(GPMDownloadWarning):
-        find._check_correct_version(filepaths=filepaths, product=product, version=version)
+        _check_correct_version(filepaths=filepaths, product=product, version=version)
 
     # Test multiple versions
     files_version = [6, 7, 7]
     filepaths = [filepath_template.format(v) for v in files_version]
     with pytest.raises(ValueError):
-        find._check_correct_version(filepaths=filepaths, product=product, version=version)
+        _check_correct_version(filepaths=filepaths, product=product, version=version)
 
     # Test empty list
     filepaths = []
-    _, returned_version = find._check_correct_version(
+    _, returned_version = _check_correct_version(
         filepaths=filepaths, product=product, version=version
     )
     assert returned_version == version
 
 
 def test_find_daily_filepaths(
     mocker: MockerFixture,
@@ -419,51 +425,51 @@
         "product_type": product_type,
         "version": version,
         "start_time": start_time,
         "end_time": end_time,
         "verbose": True,
     }
 
-    returned_filepaths, returned_versions = find.find_daily_filepaths(**kwargs)
+    returned_filepaths, returned_versions = find_daily_filepaths(**kwargs)
 
     assert returned_versions[0] == version
     returned_filepath = returned_filepaths[0]
 
     # Check date checked
     assert str(date_checked) in returned_filepath
 
     # Check all _get_all_daily_filepaths kwargs passed
     assert f"storage:{storage}" in returned_filepath
     assert f"product:{product}" in returned_filepath
     assert f"product_type:{product_type}" in returned_filepath
     assert f"date:{date_checked}" in returned_filepath
     assert f"version:{version}" in returned_filepath
-    assert f"verbose:True" in returned_filepath
+    assert "verbose:True" in returned_filepath
 
     # Check all filter_filepaths kwargs passed
     assert f"product-filtered:{product}" in returned_filepath
     assert f"product_type-filtered:{product_type}" in returned_filepath
-    assert f"version-filtered:None" in returned_filepath
+    assert "version-filtered:None" in returned_filepath
     assert f"start_time-filtered:{start_time}" in returned_filepath
     assert f"end_time-filtered:{end_time}" in returned_filepath
 
     # Check all _check_correct_version kwargs passed
     assert f"product-version-checked:{product}" in returned_filepath
     assert f"version-version-checked:{version}" in returned_filepath
 
     # Check empty filtered filepaths list
     patch_filter_filepaths.side_effect = lambda filepaths, **kwargs: []
-    returned_filepaths, returned_versions = find.find_daily_filepaths(**kwargs)
+    returned_filepaths, returned_versions = find_daily_filepaths(**kwargs)
     assert returned_filepaths == []
     assert returned_versions == []
 
     # Check empty filepaths list
     patch_get_all_daily_filepaths.side_effect = lambda **kwargs: []
     kwargs["storage"] = "local"
-    returned_filepaths, returned_versions = find.find_daily_filepaths(**kwargs)
+    returned_filepaths, returned_versions = find_daily_filepaths(**kwargs)
     assert returned_filepaths == []
     assert returned_versions == []
 
 
 def test_find_filepaths(
     mocker: MockerFixture,
 ) -> None:
@@ -499,16 +505,16 @@
         "product": product,
         "product_type": product_type,
         "start_time": start_time,
         "end_time": end_time,
         "verbose": verbose,
     }
 
-    returned_filepaths = find.find_filepaths(**kwargs, parallel=False)
-    returned_filepaths_parallel = find.find_filepaths(**kwargs, parallel=True)
+    returned_filepaths = find_filepaths(**kwargs, parallel=False)
+    returned_filepaths_parallel = find_filepaths(**kwargs, parallel=True)
     assert returned_filepaths == returned_filepaths_parallel
 
     # Check all find_daily_filepaths kwargs passed
     returned_filepath = returned_filepaths[
         -1
     ]  # Take last filepath, because "verbose" is not passed to first date
     assert f"storage:{storage}" in returned_filepath
@@ -530,9 +536,9 @@
     for date in [start_date + datetime.timedelta(days=i) for i in range(n_days)]:
         filtered = list(filter(lambda fp: f"date:{date}" in fp, returned_filepaths))
         assert len(filtered) == n_filepath_per_day, "Date is missing"
 
     # Test NRT products: single date
     product_type = "NRT"
     kwargs["product_type"] = product_type
-    returned_filepaths = find.find_filepaths(**kwargs, parallel=False)
+    returned_filepaths = find_filepaths(**kwargs, parallel=False)
     assert len(returned_filepaths) == n_filepath_per_day, "More days than expected"
```

### Comparing `gpm_api-0.2.8/gpm_api/tests/test_io/test_info.py` & `gpm_api-0.2.9/gpm_api/tests/test_io/test_info.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/tests/test_io/test_io_checks.py` & `gpm_api-0.2.9/gpm_api/tests/test_io/test_io_checks.py`

 * *Files 0% similar despite different names*

```diff
@@ -198,15 +198,15 @@
 
     # Check if outside range
     with pytest.raises(ValueError):
         checks.check_version(123)
 
     # Check available range should not raise exception
     for version in versions:
-        checks.check_version(version)
+        assert version == checks.check_version(version)
         # Should run without raising Exception
 
     # Try versions outside of range
     for version in list(range(0, 3)) + list(range(8, 10)):
         with pytest.raises(ValueError):
             checks.check_version(version)
 
@@ -246,16 +246,16 @@
 
     Depends on available_products(), test ambiguous product names similar to
     those that exist
     """
 
     # Test a product that does exist
     for product_type in product_types:
-        for product in available_products(product_type=product_type):
-            checks.check_product(product, product_type=product_type)
+        for product in available_products(product_types=product_type):
+            assert product == checks.check_product(product, product_type=product_type)
             # Should run without raising Exception
 
     # Test a product that isn't a string
     for product_type in product_types:
         for product in [("IMERG"), 123, None]:
             with pytest.raises(ValueError):
                 checks.check_product(product, product_type=product_type)
@@ -264,15 +264,15 @@
 def test_check_product_type(
     product_types: List[str],
 ) -> None:
     """Test check_product_type()"""
 
     # Test a product_type that does exist
     for product_type in product_types:
-        checks.check_product_type(product_type)
+        assert product_type == checks.check_product_type(product_type)
         # Should run without raising Exception
 
     # Test a product_type that doesn't exist
     for product_type in ["IMERG", 123, None]:
         with pytest.raises(ValueError):
             checks.check_product_type(product_type)
 
@@ -285,15 +285,15 @@
     # Test types that aren't strings
     for product_category in [123, None]:
         with pytest.raises(ValueError):
             checks.check_product_category(product_category)
 
     # Test a product_category that does exist
     for product_category in product_categories:
-        checks.check_product_category(product_category)
+        assert product_category == checks.check_product_category(product_category)
         # Should run without raising Exception
 
     # Test a product_category that doesn't exist
     for product_category in ["NOT", "A", "CATEGORY"]:
         with pytest.raises(ValueError):
             checks.check_product_category(product_category)
 
@@ -306,15 +306,15 @@
     # Test types that aren't strings
     for product_level in [123, None]:
         with pytest.raises(ValueError):
             checks.check_product_level(product_level)
 
     # Test a product_level that does exist
     for product_level in product_levels:
-        checks.check_product_level(product_level)
+        assert product_level == checks.check_product_level(product_level)
     # Should run without raising Exception
 
     # Test a product_level that doesn't exist
     for product_level in ["NOT", "A", "LEVEL"]:
         with pytest.raises(ValueError):
             checks.check_product_level(product_level)
 
@@ -322,16 +322,16 @@
 def test_check_product_validity(
     product_types: List[str],
 ) -> None:
     """Test check_product_validity()"""
 
     # Test a product that does exist
     for product_type in product_types:
-        for product in available_products(product_type=product_type):
-            checks.check_product_validity(product, product_type=product_type)
+        for product in available_products(product_types=product_type):
+            assert product == checks.check_product_validity(product, product_type=product_type)
             # Should run without raising Exception
 
     # Test a product that doesn't exist
     for product_type in product_types:
         for product in [("IMERG"), 123, None]:
             with pytest.raises(ValueError):
                 checks.check_product_validity(product, product_type=product_type)
@@ -555,15 +555,17 @@
         valid_start_time = info["start_time"]
         valid_end_time = info["end_time"]
 
         if valid_start_time is not None:
             # Check valid times
             start_time = valid_start_time
             end_time = valid_start_time + datetime.timedelta(days=1)
-            checks.check_valid_time_request(start_time, end_time, product)
+            assert (start_time, end_time) == checks.check_valid_time_request(
+                start_time, end_time, product
+            )
 
             # Check invalid start time
             start_time = valid_start_time - datetime.timedelta(days=1)
             end_time = valid_start_time + datetime.timedelta(days=1)
             with check.raises(ValueError):
                 checks.check_valid_time_request(start_time, end_time, product)
```

### Comparing `gpm_api-0.2.8/gpm_api/tests/test_io/test_local.py` & `gpm_api-0.2.9/gpm_api/tests/test_io/test_local.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/tests/test_io/test_pps.py` & `gpm_api-0.2.9/gpm_api/tests/test_io/test_pps.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,19 +10,19 @@
     Depends on gpm_api.io.pps._get_pps_nrt_product_folder_name()
     """
 
     date = datetime.datetime(2021, 1, 1).date()
 
     for product in products:
         # Only work on NRT products
-        if product in available_products(product_type="NRT"):
+        if product in available_products(product_types="NRT"):
             # Dependent on dir forming private function
             foldername = pps._get_pps_nrt_product_folder_name(product)
 
             res = pps._get_pps_nrt_product_dir(product, date)
             if product in available_products(
-                product_type="NRT",
-                product_category="IMERG",
+                product_types="NRT",
+                product_categories="IMERG",
             ):
                 assert res == f"{foldername}/{date.strftime('%Y%m')}"
             else:
                 assert res == foldername
```

### Comparing `gpm_api-0.2.8/gpm_api/tests/test_io/test_products.py` & `gpm_api-0.2.9/gpm_api/tests/test_io/test_products.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/tests/test_utils/test_list.py` & `gpm_api-0.2.9/gpm_api/tests/test_utils/test_list.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/tests/utils/hdf5.py` & `gpm_api-0.2.9/gpm_api/tests/utils/hdf5.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/utils/archive.py` & `gpm_api-0.2.9/gpm_api/utils/archive.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/utils/area.py` & `gpm_api-0.2.9/gpm_api/utils/area.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/utils/checks.py` & `gpm_api-0.2.9/gpm_api/utils/checks.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,26 @@
     list_slices_intersection,
     list_slices_sort,
     list_slices_union,
 )
 
 ORBIT_TIME_TOLERANCE = np.timedelta64(3, "s")
 
-# TODO: raise ValueError("Unrecognized GPM xarray object.") has decorator check?
+
+def _check_is_orbit_or_grid(function):
+    """Decorator function to check if input is orbit or grid. Raise ValueError if not."""
+
+    @functools.wraps(function)
+    def wrapper(*args, **kwargs):
+        xr_obj = args[0]
+        if not is_orbit(xr_obj) and not is_grid(xr_obj):
+            raise ValueError("Unrecognized GPM xarray object.")
+        return function(*args, **kwargs)
+
+    return wrapper
 
 
 ####--------------------------------------------------------------------------.
 ##########################
 #### Regular granules ####
 ##########################
 
@@ -53,14 +64,15 @@
     bool_arr = np.diff(granule_ids) <= 1
 
     # Add True to last position
     bool_arr = np.append(bool_arr, True)
     return bool_arr
 
 
+@_check_is_orbit_or_grid
 def get_slices_contiguous_granules(xr_obj, min_size=2):
     """
     Return a list of slices ensuring contiguous granules.
 
     Output format: [slice(start,stop), slice(start,stop),...]
 
     The minimum size of the output slices is 2.
@@ -102,16 +114,14 @@
         )
 
         # Select only slices with at least 2 scans
         list_slices = list_slices_filter(list_slices, min_size=min_size)
 
         # Return list of contiguous scan slices
         return list_slices
-    else:
-        raise ValueError("Unrecognized GPM xarray object.")
 
 
 def check_missing_granules(xr_obj):
     """
     Check no missing granules in the GPM Dataset.
 
     Parameters
@@ -127,36 +137,34 @@
         raise ValueError(msg)
 
 
 def check_contiguous_granules(xr_obj):
     return check_missing_granules(xr_obj)
 
 
+@_check_is_orbit_or_grid
 def has_contiguous_granules(xr_obj):
     """Checks GPM object is composed of consecutive granules."""
     from gpm_api.checks import is_grid, is_orbit
 
     if is_orbit(xr_obj):
         return bool(np.all(_is_contiguous_granule(xr_obj["gpm_granule_id"].data)))
     if is_grid(xr_obj):
         return has_regular_time(xr_obj)
-    else:
-        raise ValueError("Unrecognized GPM xarray object.")
 
 
+@_check_is_orbit_or_grid
 def has_missing_granules(xr_obj):
     """Checks GPM object has missing granules."""
     from gpm_api.checks import is_grid, is_orbit
 
     if is_orbit(xr_obj):
         return bool(np.any(~_is_contiguous_granule(xr_obj["gpm_granule_id"].data)))
     if is_grid(xr_obj):
-        return ~has_regular_time(xr_obj)
-    else:
-        raise ValueError("Unrecognized GPM xarray object.")
+        return not has_regular_time(xr_obj)
 
 
 ####--------------------------------------------------------------------------.
 ############################
 #### Regular timesteps  ####
 ############################
 
@@ -164,27 +172,26 @@
 def _get_timesteps(xr_obj):
     """Get timesteps with second precision from xarray object."""
     timesteps = xr_obj["time"].values
     timesteps = timesteps.astype("M8[s]")
     return timesteps
 
 
+@_check_is_orbit_or_grid
 def _infer_time_tolerance(xr_obj):
     """Infer time interval tolerance between timesteps."""
     from gpm_api.checks import is_grid, is_orbit
 
     # For GPM ORBIT objects, use the ORBIT_TIME_TOLERANCE
     if is_orbit(xr_obj):
         tolerance = ORBIT_TIME_TOLERANCE
     # For GPM GRID objects, infer it from the time difference between first two timesteps
     elif is_grid(xr_obj):
         timesteps = _get_timesteps(xr_obj)
         tolerance = np.diff(timesteps[0:2])[0]
-    else:
-        raise ValueError("Unrecognized GPM xarray object.")
     return tolerance
 
 
 def _is_regular_time(xr_obj, tolerance=None):
     """Return a boolean array indicating if the next regular timestep is present."""
     # Retrieve timesteps
     timesteps = _get_timesteps(xr_obj)
@@ -208,16 +215,17 @@
 
     Parameters
     ----------
     xr_obj : (xr.Dataset, xr.DataArray)
         GPM xarray object.
     tolerance : np.timedelta, optional
         The timedelta tolerance to define regular vs. non-regular timesteps.
-        If None, it uses the first 2 timesteps to derive the tolerance timedelta.
         The default is None.
+        If GPM GRID object, it uses the first 2 timesteps to derive the tolerance timedelta.
+        If GPM ORBIT object, it uses the ORBIT_TIME_TOLERANCE.
     min_size : int
         Minimum size for a slice to be returned.
 
     Returns
     -------
     list_slices : list
         List of slice object to select regular time intervals.
@@ -263,15 +271,15 @@
     ----------
     xr_obj : (xr.Dataset, xr.DataArray)
         GPM xarray object.
     tolerance : np.timedelta, optional
         The timedelta tolerance to define regular vs. non-regular timesteps.
         The default is None.
         If GPM GRID object, it uses the first 2 timesteps to derive the tolerance timedelta.
-        If GPM ORBIT object, it uses the gpm_api.utils.time.ORBIT_TIME_TOLERANCE.
+        If GPM ORBIT object, it uses the ORBIT_TIME_TOLERANCE.
         It is discouraged to use this function for GPM ORBIT objects !
 
     Returns
     -------
     list_slices : list
         List of slice object to select intervals with non-regular timesteps.
     """
@@ -309,15 +317,15 @@
     ----------
     xr_obj : xr.Dataset or xr.DataArray
         xarray object.
     tolerance : np.timedelta, optional
         The timedelta tolerance to define regular vs. non-regular timesteps.
         The default is None.
         If GPM GRID object, it uses the first 2 timesteps to derive the tolerance timedelta.
-        If GPM ORBIT object, it uses the gpm_api.utils.time.ORBIT_TIME_TOLERANCE
+        If GPM ORBIT object, it uses the ORBIT_TIME_TOLERANCE
     verbose : bool
         If True, it prints the time interval when the non contiguous scans occurs.
         The default is True.
 
     Returns
     -------
 
@@ -560,16 +568,19 @@
     None.
     """
     list_discontinuous_slices = get_slices_non_contiguous_scans(xr_obj)
     n_discontinuous = len(list_discontinuous_slices)
     if n_discontinuous > 0:
         # Retrieve discontinuous timesteps interval
         timesteps = _get_timesteps(xr_obj)
+        discontinuous_timestep_idx = [
+            slice(slc.start - 1, slc.stop) for slc in list_discontinuous_slices
+        ]
         list_discontinuous = [
-            (timesteps[slc][0], timesteps[slc][-1]) for slc in list_discontinuous_slices
+            (timesteps[slc][0], timesteps[slc][-1]) for slc in discontinuous_timestep_idx
         ]
         first_problematic_timestep = list_discontinuous[0][0]
         # Print non-contiguous scans
         if verbose:
             for start, stop in list_discontinuous:
                 print(f"- Missing scans between {start} and {stop}")
         # Raise error and highlight first non-contiguous scan
@@ -609,14 +620,15 @@
 
     True = Valid, False = Invalid
     """
     bool_arr = ~np.isnan(xr_obj[x])
     return bool_arr
 
 
+@_check_is_orbit_or_grid
 def get_slices_valid_geolocation(xr_obj, min_size=2):
     """Return a list of along-track slices ensuring valid geolocation.
 
     Output format: [slice(start,stop), slice(start,stop),...]
 
     The minimum size of the output slices is 2.
 
@@ -642,29 +654,27 @@
     if is_orbit(xr_obj):
         # - Get invalid coordinates
         invalid_coords = _is_non_valid_geolocation(xr_obj, x="lon")
         # - Identify cross-track index that along-track are always invalid
         idx_cross_track_not_all_invalid = np.where(~invalid_coords.all("along_track"))[0]
         # - If all invalid, return empty list
         if len(idx_cross_track_not_all_invalid) == 0:
-            list_slices = []
-            return list_slices
+            return []
         # - Select only cross-track index that are not all invalid along-track
         invalid_coords = invalid_coords.isel(cross_track=idx_cross_track_not_all_invalid)
         # - Now identify scans across which there are still invalid coordinates
         invalid_scans = invalid_coords.any(dim="cross_track")
         valid_scans = ~invalid_scans
         # - Now identify valid along-track slices
         list_slices = get_list_slices_from_bool_arr(
             valid_scans, include_false=False, skip_consecutive_false=True
         )
         # Select only slices with at least 2 scans
         list_slices = list_slices_filter(list_slices, min_size=min_size)
         return list_slices
-    return None
 
 
 def get_slices_non_valid_geolocation(xr_obj):
     """Return a list of along-track slices with non-valid geolocation.
 
     Output format: [slice(start,stop), slice(start,stop),...]
 
@@ -716,24 +726,23 @@
         # Raise error and highlight first non-contiguous scan
         msg = f"There are {n_invalid_scan_slices} swath portions with non-valid geolocation."
         msg += f"The first occur at {first_problematic_timestep}."
         raise ValueError(msg)
     return
 
 
+@_check_is_orbit_or_grid
 def has_valid_geolocation(xr_obj):
     """Checks GPM object has valid geolocation."""
     if is_orbit(xr_obj):
         list_invalid_slices = get_slices_non_valid_geolocation(xr_obj)
         n_invalid_scan_slices = len(list_invalid_slices)
         return n_invalid_scan_slices == 0
     if is_grid(xr_obj):
         return True
-    else:
-        raise ValueError("Unrecognized GPM xarray object.")
 
 
 def apply_on_valid_geolocation(function):
     """A decorator that apply the get_slices_<function> only on portions
     with valid geolocation."""
 
     @functools.wraps(function)
@@ -826,16 +835,16 @@
     from gpm_api.utils.slices import list_slices_intersection
 
     # Assume lats, lons having shape (y, x) with x=along_track direction
     swath_def = xr_obj.gpm_api.pyresample_area
     lats_side0 = swath_def.lats[0, :]
     lats_side2 = swath_def.lats[-1, :]
     # Get valid slices
-    list_slices1 = _get_non_wobbling_lats(lats_side0, threshold=100)
-    list_slices2 = _get_non_wobbling_lats(lats_side2, threshold=100)
+    list_slices1 = _get_non_wobbling_lats(lats_side0, threshold=threshold)
+    list_slices2 = _get_non_wobbling_lats(lats_side2, threshold=threshold)
     list_slices = list_slices_intersection(list_slices1, list_slices2)
     return list_slices
 
 
 @apply_on_valid_geolocation
 def get_slices_wobbling_swath(xr_obj, threshold=100):
     """Return the along-track slices along which the swath is wobbling.
@@ -854,30 +863,30 @@
 
 ####---------------------------------------------------------------------------
 #####################################
 #### Check GPM object regularity ####
 #####################################
 
 
+@_check_is_orbit_or_grid
 def is_regular(xr_obj):
     """Checks the GPM object is regular.
 
     For GPM ORBITS, it checks that the scans are contiguous.
     For GPM GRID, it checks that the timesteps are regularly spaced.
     """
     from gpm_api.checks import is_grid, is_orbit
 
     if is_orbit(xr_obj):
         return has_contiguous_scans(xr_obj)
     elif is_grid(xr_obj):
         return has_regular_time(xr_obj)
-    else:
-        raise ValueError("Unrecognized GPM xarray object.")
 
 
+@_check_is_orbit_or_grid
 def get_slices_regular(xr_obj, min_size=None):
     """
     Return a list of slices to select regular GPM objects.
 
     For GPM ORBITS, it returns slices to select contiguouse scans with valid geolocation.
     For GPM GRID, it returns slices to select periods with regular timesteps.
 
@@ -910,16 +919,14 @@
         # Find swath portions meeting all the requirements
         list_slices = list_slices_intersection(list_slices_geolocation, list_slices_contiguous)
 
         return list_slices
     elif is_grid(xr_obj):
         min_size = 1 if min_size is None else min_size
         return get_slices_regular_time(xr_obj, min_size=min_size)
-    else:
-        raise ValueError("Unrecognized GPM xarray object.")
 
 
 ####--------------------------------------------------------------------------.
 #### Get slices from GPM object variable values
 
 
 def _check_criteria(criteria):
@@ -938,15 +945,15 @@
     # Identify regions where the value occurs
     da_bool = da == value
     # Collapse other dimension than dim
     dims_apply_over = list(dims.difference(dim))
     bool_arr = (
         da_bool.all(dim=dims_apply_over).data
         if criteria == "all"
-        else da_bool.all(dim=dims_apply_over).data
+        else da_bool.any(dim=dims_apply_over).data
     )
     # Get list of slices with contiguous value
     list_slices = get_list_slices_from_bool_arr(
         bool_arr, include_false=False, skip_consecutive_false=True
     )
     return list_slices
```

### Comparing `gpm_api-0.2.8/gpm_api/utils/collocation.py` & `gpm_api-0.2.9/gpm_api/utils/collocation.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,20 +13,20 @@
 
 def _get_collocation_defaults_args(product, variables, groups, version, scan_modes):
     """Get collocation defaults arguments."""
     if scan_modes is None:
         scan_modes = gpm_api.available_scan_modes(product=product, version=version)
     if isinstance(scan_modes, str):
         scan_modes = [scan_modes]
-    if product not in gpm_api.available_products(product_category="PMW"):
+    if product not in gpm_api.available_products(product_categories="PMW"):
         if len(scan_modes) > 1:
             raise ValueError("Multiple scan modes can be specified only for PMW products!")
     # PMW defaults
     if variables is None and groups is None:
-        if product in gpm_api.available_products(product_level="2A", product_category="PMW"):
+        if product in gpm_api.available_products(product_levels="2A", product_categories="PMW"):
             variables = [
                 "surfacePrecipitation",
                 "mostLikelyPrecipitation",
                 "cloudWaterPath",  # kg/m2
                 "rainWaterPath",  # kg/m2
                 "iceWaterPath",  # kg/m2
             ]
```

### Comparing `gpm_api-0.2.8/gpm_api/utils/geospatial.py` & `gpm_api-0.2.9/gpm_api/utils/geospatial.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,63 +1,165 @@
 #!/usr/bin/env python3
 """
 Created on Wed Aug 17 09:30:29 2022
 
 @author: ghiggi
 """
+import difflib
+import os
 import warnings
+from typing import Union
 
 import numpy as np
 import xarray as xr
 
+from gpm_api import _root_path
 from gpm_api.checks import is_grid, is_orbit
 from gpm_api.utils.slices import get_list_slices_from_indices
+from gpm_api.utils.yaml import read_yaml_file
 
 # Shapely bounds: (xmin, ymin, xmax, ymax)
 # Matlotlib extent: (xmin, xmax, ymin, ymax)
 # Cartopy extent: (xmin, xmax, ymin, ymax)
 # GPM-API extent: (xmin, xmax, ymin, ymax)
 
 #### TODO:
 # - croup_around(point, distance)
 # - get_extent_around(point, distance)
-# - rename file crop.py?
+
+
+def _extend_lonlat_extent(extent, x):
+    """
+    Extend the lat/lon extent by x degrees in every direction.
+
+    Parameters
+    ----------
+    extent : (tuple)
+        A tuple of four values representing the lat/lon extent.
+        The extent format must be [xmin, xmax, ymin, ymax]
+    x : float
+        The number of degrees to extend the extent in every direction.
+
+    Returns
+    -------
+    new_extent, tuple
+        The extended extent.
+    """
+    xmin, xmax, ymin, ymax = extent
+    xmin = max(xmin - x, -180)
+    xmax = min(xmax + x, 180)
+    ymin = max(ymin - x, -90)
+    ymax = min(ymax + x, 90)
+    new_extent = (xmin, xmax, ymin, ymax)
+    return new_extent
+
+
+def _get_country_extent_dictionary():
+    countries_extent_fpath = os.path.join(_root_path, "gpm_api", "etc", "country_extent.yaml")
+    countries_extent_dict = read_yaml_file(countries_extent_fpath)
+    return countries_extent_dict
+
+
+def get_country_extent(name, padding=0.2):
+    # Check country format
+    if not isinstance(name, str):
+        raise TypeError("Please provide the country name as a string.")
+    # Get country extent dictionary
+    countries_extent_dict = _get_country_extent_dictionary()
+    # Create same dictionary with lower case keys
+    countries_lower_extent_dict = {s.lower(): v for s, v in countries_extent_dict.items()}
+    # Get list of valid countries
+    valid_countries = list(countries_extent_dict.keys())
+    valid_countries_lower = list(countries_lower_extent_dict)
+    if name.lower() in valid_countries_lower:
+        extent = countries_lower_extent_dict[name.lower()]
+        extent = _extend_lonlat_extent(extent, padding)
+        return extent
+    else:
+        possible_match = difflib.get_close_matches(name, valid_countries, n=1, cutoff=0.6)
+        if len(possible_match) == 0:
+            raise ValueError("Provide a valid country name.")
+        else:
+            possible_match = possible_match[0]
+            raise ValueError(f"No matching country. Maybe are you looking for '{possible_match}'?")
+
+
+def _get_continent_extent_dictionary():
+    continents_extent_fpath = os.path.join(_root_path, "gpm_api", "etc", "continent_extent.yaml")
+    continents_extent_dict = read_yaml_file(continents_extent_fpath)
+    return continents_extent_dict
+
+
+def get_continent_extent(name, padding=0):
+    # Check country format
+    if not isinstance(name, str):
+        raise TypeError("Please provide the continent name as a string.")
+
+    # Create same dictionary with lower case keys
+    continent_extent_dict = _get_continent_extent_dictionary()
+    continent_lower_extent_dict = {s.lower(): v for s, v in continent_extent_dict.items()}
+    # Get list of valid continents
+    valid_continent = list(continent_extent_dict.keys())
+    valid_continent_lower = list(continent_lower_extent_dict)
+    if name.lower() in valid_continent_lower:
+        extent = continent_lower_extent_dict[name.lower()]
+        extent = _extend_lonlat_extent(extent, padding)
+        return extent
+    else:
+        possible_match = difflib.get_close_matches(name, valid_continent, n=1, cutoff=0.6)
+        if len(possible_match) == 0:
+            raise ValueError(f"Provide a valid continent name from {valid_continent}.")
+        else:
+            possible_match = possible_match[0]
+            raise ValueError(
+                f"No matching continent. Maybe are you looking for '{possible_match}'?"
+            )
 
 
 def unwrap_longitude_degree(x, period=360):
     """Unwrap longitude array."""
     x = np.asarray(x)
     mod = period / 2
     return (x + mod) % (2 * mod) - mod
 
 
-def get_extent(xr_obj, padding=0):
+def _is_crossing_dateline(lon: Union[list, np.ndarray]):
+    """Check if the longitude array is crossing the dateline."""
+
+    lon = np.asarray(lon)
+    diff = np.diff(lon)
+    return np.any(np.abs(diff) > 180)
+
+
+def get_extent(xr_obj, padding: Union[int, float, tuple, list] = 0):
     """Get geographic extent.
 
     The extent follows the matplotlib/cartopy format (xmin, xmax, ymin, ymax)
     The padding tuple is expected to follow the format (x, y)
     """
     if isinstance(padding, (int, float)):
         padding = (padding, padding)
     elif isinstance(padding, (tuple, list)):
         if len(padding) != 2:
             raise ValueError("Expecting a padding (x, y) tuple of length 2.")
     else:
         raise TypeError("Accepted padding type are int, float, list or tuple.")
     lon = xr_obj["lon"].data
     lat = xr_obj["lat"].data
+
+    if _is_crossing_dateline(lon):
+        raise NotImplementedError(
+            "The object cross the dateline. The extent can't be currently defined."
+        )
+
     lon_min = max(-180, np.nanmin(lon).item() - padding[0])
     lon_max = min(180, np.nanmax(lon).item() + padding[0])
     lat_min = max(-90, np.nanmin(lat).item() - padding[1])
     lat_max = min(90, np.nanmax(lat).item() + padding[1])
 
-    if lon_min > lon_max:
-        raise NotImplementedError(
-            "The object cross the dateline. The extent can't be currently be defined."
-        )
     extent = tuple([lon_min, lon_max, lat_min, lat_max])
     return extent
 
 
 def crop_by_country(xr_obj, name):
     """
     Crop an xarray object based on the specified country name.
@@ -72,16 +174,14 @@
     Returns
     -------
     xr_obj : xr.DataArray or xr.Dataset
         Cropped xarray object.
 
     """
 
-    from gpm_api.utils.countries import get_country_extent
-
     extent = get_country_extent(name)
     return crop(xr_obj=xr_obj, extent=extent)
 
 
 def crop_by_continent(xr_obj, name):
     """
     Crop an xarray object based on the specified continent name.
@@ -96,16 +196,14 @@
     Returns
     -------
     xr_obj : xr.DataArray or xr.Dataset
         Cropped xarray object.
 
     """
 
-    from gpm_api.utils.continents import get_continent_extent
-
     extent = get_continent_extent(name)
     return crop(xr_obj=xr_obj, extent=extent)
 
 
 def get_crop_slices_by_extent(xr_obj, extent):
     """Compute the xarray object slices which are within the specified extent.
 
@@ -163,16 +261,14 @@
     Parameters
     ----------
     xr_obj : xr.DataArray or xr.Dataset
         xarray object.
     name : str
         Continent name.
     """
-    from gpm_api.utils.continents import get_continent_extent
-
     extent = get_continent_extent(name)
     return get_crop_slices_by_extent(xr_obj=xr_obj, extent=extent)
 
 
 def get_crop_slices_by_country(xr_obj, name):
     """Compute the xarray object slices which are within the specified country.
 
@@ -182,16 +278,14 @@
     Parameters
     ----------
     xr_obj : xr.DataArray or xr.Dataset
         xarray object.
     name : str
         Country name.
     """
-    from gpm_api.utils.countries import get_country_extent
-
     extent = get_country_extent(name)
     return get_crop_slices_by_extent(xr_obj=xr_obj, extent=extent)
 
 
 def crop(xr_obj, extent):
     """
     Crop a xarray object based on the provided bounding box.
```

### Comparing `gpm_api-0.2.8/gpm_api/utils/list.py` & `gpm_api-0.2.9/gpm_api/utils/list.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/utils/manipulations.py` & `gpm_api-0.2.9/gpm_api/utils/manipulations.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/utils/parallel.py` & `gpm_api-0.2.9/gpm_api/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/utils/slices.py` & `gpm_api-0.2.9/gpm_api/utils/slices.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 #!/usr/bin/env python3
 """
 Created on Sat Dec 10 18:46:00 2022
 
 @author: ghiggi
 """
-from functools import reduce
 
 import numpy as np
 
 ####---------------------------------------------------------------------------.
 #### Tools for list_slices
 
 
@@ -58,35 +57,83 @@
     list_indices = [np.arange(slc.start, slc.stop, slc.step) for slc in list_slices]
     indices, counts = np.unique(np.concatenate(list_indices), return_counts=True)
     if check_non_intersecting and np.any(counts > 1):
         raise ValueError("The list of slices contains intersecting slices!")
     return indices
 
 
-def list_slices_intersection(*args):
+def _get_slices_intersection(slc1, slc2, min_size=1):
+    """Return the intersecting slices from two slices."""
+    if not isinstance(slc1, slice) or not isinstance(slc2, slice):
+        raise TypeError("Expecting slice objects")
+
+    start = max(slc1.start, slc2.start)
+    stop = min(slc1.stop, slc2.stop)
+
+    if stop - start < min_size:
+        return None
+
+    return slice(start, stop)
+
+
+def list_slices_intersection(*args, min_size=1):
     """Return the intersecting slices from multiple list of slices."""
-    list_indices = [get_indices_from_list_slices(l_slc) for l_slc in list(args)]
-    intersect_indices = reduce(np.intersect1d, list_indices)
-    return get_list_slices_from_indices(intersect_indices)
+    if len(args) == 0:
+        return []
+
+    list_slices = [slice(-np.inf, np.inf)]
+
+    for i in range(len(args)):
+        list_slices = [
+            _get_slices_intersection(slc1, slc2, min_size)
+            for slc1 in list_slices
+            for slc2 in args[i]
+        ]
+        list_slices = [slc for slc in list_slices if slc is not None]
+        if len(list_slices) == 0:
+            return []
+
+    return list_slices
 
 
 def list_slices_union(*args):
     """Return the union slices from multiple list of slices."""
     list_indices = [get_indices_from_list_slices(l_slc) for l_slc in list(args)]
     union_indices = np.unique(np.concatenate(list_indices))
     return get_list_slices_from_indices(union_indices)
 
 
+def _get_slices_difference(slc1, slc2):
+    """Return the list of slices covered by slc1 not intersecting slc2."""
+    slice_left = slice(slc1.start, min(slc1.stop, slc2.start))
+    slice_right = slice(max(slc1.start, slc2.stop), slc1.stop)
+
+    slices = []
+
+    if get_slice_size(slice_left) > 0:
+        slices.append(slice_left)
+
+    if get_slice_size(slice_right) > 0:
+        slices.append(slice_right)
+
+    return slices
+
+
 def list_slices_difference(list_slices1, list_slices2):
     """Return the list of slices covered by list_slices1 not intersecting list_slices2."""
-    list_indices1 = get_indices_from_list_slices(list_slices1)
-    list_indices2 = get_indices_from_list_slices(list_slices2)
-    diff_indices = np.setdiff1d(list_indices1, list_indices2)
-    list_slices = get_list_slices_from_indices(diff_indices)
-    return list_slices
+    if len(list_slices2) == 0:
+        return list_slices1
+
+    list_slices = [
+        [slc for slc1 in list_slices1 for slc in _get_slices_difference(slc1, slc2)]
+        for slc2 in list_slices2
+    ]
+    return list_slices_intersection(
+        *list_slices, min_size=0
+    )  # min_size=0 to keep holes from list_slices2
 
 
 def list_slices_combine(*args):
     """Combine together a list of list_slices, without any additional operation."""
     return [slc for list_slices in args for slc in list_slices]
 
 
@@ -291,44 +338,48 @@
         The default is np.inf.
     Returns
     -------
     list_slices : TYPE
         The list of slices after applying padding.
     """
 
-    new_slice = slice(max(slc.start - padding, 0), min(slc.stop + padding, max_stop))
+    new_slice = slice(max(slc.start - padding, min_start), min(slc.stop + padding, max_stop))
     return new_slice
 
 
 def pad_slices(list_slices, padding, valid_shape):
     """
     Increase/decrease the list of slices with the padding argument.
 
     Parameters
     ----------
     list_slices : list
         List of slice objects.
     padding : (int or tuple)
         Padding to be applied on each slice.
-    valid_shape : tuple
+    valid_shape : (int or tuple)
         The shape of the array which the slices should be valid on.
 
     Returns
     -------
     list_slices : TYPE
         The list of slices after applying padding.
     """
     # Check the inputs
     if isinstance(padding, int):
         padding = [padding] * len(list_slices)
     if isinstance(valid_shape, int):
         valid_shape = [valid_shape] * len(list_slices)
-    if isinstance(padding, (list, tuple)) and len(padding) != len(valid_shape):
+    if isinstance(padding, (list, tuple)) and len(padding) != len(list_slices):
+        raise ValueError(
+            "Invalid padding. The length of padding should be the same as the length of list_slices."
+        )
+    if isinstance(valid_shape, (list, tuple)) and len(valid_shape) != len(list_slices):
         raise ValueError(
-            "Invalid padding. The length of padding should be the same as the length of valid_shape."
+            "Invalid valid_shape. The length of valid_shape should be the same as the length of list_slices."
         )
     # Apply padding
     list_slices = [
         pad_slice(s, padding=p, min_start=0, max_stop=valid_shape[i])
         for i, (s, p) in enumerate(zip(list_slices, padding))
     ]
     return list_slices
@@ -421,30 +472,34 @@
 
     Parameters
     ----------
     list_slices : list
         List of slice objects.
     min_size : (int or tuple)
         Minimum size of the output slice.
-    valid_shape : tuple
+    valid_shape : (int or tuple)
         The shape of the array which the slices should be valid on.
 
     Returns
     -------
     list_slices : list
         The list of slices after enlarging it (if necessary).
     """
     # Check the inputs
     if isinstance(min_size, int):
         min_size = [min_size] * len(list_slices)
     if isinstance(valid_shape, int):
         valid_shape = [valid_shape] * len(list_slices)
-    if isinstance(min_size, (list, tuple)) and len(min_size) != len(min_size):
+    if isinstance(min_size, (list, tuple)) and len(min_size) != len(list_slices):
+        raise ValueError(
+            "Invalid min_size. The length of min_size should be the same as the length of list_slices."
+        )
+    if isinstance(valid_shape, (list, tuple)) and len(valid_shape) != len(list_slices):
         raise ValueError(
-            "Invalid min_size. The length of min_size should be the same as the length of valid_shape."
+            "Invalid valid_shape. The length of valid_shape should be the same as the length of list_slices."
         )
     # Enlarge the slice
     list_slices = [
         enlarge_slice(slc, min_size=s, min_start=0, max_stop=valid_shape[i])
         for i, (slc, s) in enumerate(zip(list_slices, min_size))
     ]
     return list_slices
```

### Comparing `gpm_api-0.2.8/gpm_api/utils/time.py` & `gpm_api-0.2.9/gpm_api/utils/time.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
     # Get 1D dimension of the coordinate
     dim_coords = list(xr_obj["time"].dims)
 
     # If no dimension, it means that nothing to be subsetted
     # - Likely the time dimension has been dropped ...
     if len(dim_coords) == 0:
-        return {}
+        raise ValueError("Impossible to subset a non-dimensional time coordinate.")
 
     # If dimension > 1, not clear how to collapse to 1D the boolean array
     if len(dim_coords) != 1:
         raise ValueError(
             "Impossible to subset a non-dimensional time coordinate with dimension >=2."
         )
 
@@ -151,14 +151,16 @@
 
      Returns
     -------
     timesteps, np.array
         Timesteps array of type datetime64[ns]
 
     """
+    if len(timesteps) == 0:
+        return timesteps
     # Retrieve input dtype
     timesteps_dtype = timesteps.dtype
     # Convert timesteps to float
     timesteps_num = timesteps.astype(float)
     # Convert NaT to np.nan
     timesteps_num[is_nat(timesteps)] = np.nan
     # Create pd.Series
@@ -173,24 +175,28 @@
     # Convert back to numpy array input dtype
     timesteps = series.to_numpy().astype(timesteps_dtype)
     return timesteps
 
 
 def infill_timesteps(timesteps, limit):
     """Infill missing timesteps if less than <limit> consecutive."""
-    # Check at least two time steps available to infill
-    if len(timesteps) <= 2:
-        return timesteps
-
     # Interpolate if maximum <limit> timesteps are missing
     timesteps = interpolate_nat(timesteps, method="linear", limit=limit, limit_area="inside")
 
     # Check if there are still residual NaT
     if np.any(is_nat(timesteps)):
-        raise ValueError(f"More than {limit} consecutive timesteps are NaT.")
+        if len(timesteps) <= 2:
+            error_message = "Not enough timesteps available to infill NaTs."
+        elif is_nat(timesteps[0]) or is_nat(timesteps[-1]):
+            error_message = (
+                "NaTs present at the beginning or at the end of the timesteps cannot be inferred."
+            )
+        else:
+            error_message = f"More than {limit} consecutive timesteps are NaT."
+        raise ValueError(error_message)
 
     return timesteps
 
 
 def ensure_time_validity(xr_obj, limit=10):
     """
     Attempt to correct the time coordinate if less than 'limit' consecutive NaT values are present.
@@ -201,15 +207,15 @@
     ----------
     xr_obj : (xr.Dataset, xr.DataArray)
         GPM xarray object.
 
     Returns
     -------
     xr_obj : (xr.Dataset, xr.DataArray)
-        GPM xarray object..
+        GPM xarray object.
 
     """
     timesteps = xr_obj["time"].values
     timesteps = infill_timesteps(timesteps, limit=limit)
     if "time" not in list(xr_obj.dims):
         xr_obj["time"].data = timesteps
     else:
```

### Comparing `gpm_api-0.2.8/gpm_api/utils/timing.py` & `gpm_api-0.2.9/gpm_api/utils/timing.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/utils/utils_cmap.py` & `gpm_api-0.2.9/gpm_api/utils/utils_cmap.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/utils/yaml.py` & `gpm_api-0.2.9/gpm_api/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/visualization/grid.py` & `gpm_api-0.2.9/gpm_api/visualization/grid.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/visualization/orbit.py` & `gpm_api-0.2.9/gpm_api/visualization/orbit.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/visualization/plot.py` & `gpm_api-0.2.9/gpm_api/visualization/plot.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/visualization/plot_3d.py` & `gpm_api-0.2.9/gpm_api/visualization/plot_3d.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api/visualization/profile.py` & `gpm_api-0.2.9/gpm_api/visualization/profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -266,15 +266,15 @@
         ax.text(lon_l, lat_l, "L", **text_kwargs, **common_kwargs)
 
 
 def plot_transect(
     da,
     ax=None,
     add_colorbar=True,
-    zoom=False,
+    zoom=True,
     fig_kwargs={},
     cbar_kwargs={},
     **plot_kwargs,
 ):
     """Plot GPM transect."""
     # - Check inputs
     check_is_transect(da)
```

### Comparing `gpm_api-0.2.8/gpm_api/visualization/title.py` & `gpm_api-0.2.9/gpm_api/visualization/title.py`

 * *Files identical despite different names*

### Comparing `gpm_api-0.2.8/gpm_api.egg-info/PKG-INFO` & `gpm_api-0.2.9/gpm_api.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpm-api
-Version: 0.2.8
+Version: 0.2.9
 Summary: Python API for the Global Precipitation Mission Data Archive
 Author-email: Gionata Ghiggi <gionata.ghiggi@epfl.ch>
 License: MIT License
         
         Copyright (c) 2023 Gionata Ghiggi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -21,18 +21,19 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: Homepage, https://github.com/ghiggi/gpm_api
-Project-URL: Source, https://github.com/ghiggi/gpm_api
-Project-URL: Tracker, https://github.com/ghiggi/gpm_api/issues
-Project-URL: Documentation, https://gpm_api.readthedocs.io
+Project-URL: homepage, https://github.com/ghiggi/gpm_api
+Project-URL: repository, https://github.com/ghiggi/gpm_api
+Project-URL: source, https://github.com/ghiggi/gpm_api
+Project-URL: tracker, https://github.com/ghiggi/gpm_api/issues
+Project-URL: documentation, https://gpm_api.readthedocs.io
 Project-URL: changelog, https://github.com/ghigg/gpm_api/CHANGELOG.md
 Keywords: GPM,Precipitation,API,DPR,PMW,IMERG
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
@@ -89,37 +90,47 @@
 Requires-Dist: wheel; extra == "dev"
 Requires-Dist: sphinx; extra == "dev"
 Requires-Dist: sphinx-gallery; extra == "dev"
 Requires-Dist: sphinx-book-theme; extra == "dev"
 Requires-Dist: nbsphinx; extra == "dev"
 Requires-Dist: sphinx_mdinclude; extra == "dev"
 
-# Welcome to GPM-API
-[![DOI](https://zenodo.org/badge/286664485.svg)](https://zenodo.org/badge/latestdoi/286664485)
-[![PyPI version](https://badge.fury.io/py/gpm_api.svg)](https://badge.fury.io/py/gpm_api)
-[![Conda Version](https://img.shields.io/conda/vn/conda-forge/gpm_api.svg)](https://anaconda.org/conda-forge/gpm_api)
-[![Tests](https://github.com/ghiggi/gpm_api/actions/workflows/tests.yml/badge.svg)](https://github.com/ghiggi/gpm_api/actions/workflows/tests.yml)
-[![Coverage Status](https://coveralls.io/repos/github/ghiggi/gpm_api/badge.svg?branch=main)](https://coveralls.io/github/ghiggi/gpm_api?branch=main)
-[![Documentation Status](https://readthedocs.org/projects/gpm-api/badge/?version=latest)](https://gpm-api.readthedocs.io/en/latest/?badge=latest)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
-[![License](https://img.shields.io/github/license/ghiggi/gpm_api)](https://github.com/ghiggi/gpm_api/blob/master/LICENSE)
+# 📦 Welcome to GPM-API
+
+|                      |                                                |
+| -------------------- | ---------------------------------------------- |
+| Deployment           | [![PyPI](https://badge.fury.io/py/gpm_api.svg?style=flat)](https://pypi.org/project/gpm_api/) [![Conda](https://img.shields.io/conda/vn/conda-forge/gpm_api.svg?logo=conda-forge&logoColor=white&style=flat)](https://anaconda.org/conda-forge/gpm_api) |
+| Activity             | [![PyPI Downloads](https://img.shields.io/pypi/dm/gpm_api.svg?label=PyPI%20downloads&style=flat)](https://pypi.org/project/gpm_api/) [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/gpm_api.svg?label=Conda%20downloads&style=flat)](https://anaconda.org/conda-forge/gpm_api) |
+| Python Versions      | [![Python Versions](https://img.shields.io/badge/Python-3.8%20%203.9%20%203.10%20%203.11%20%203.12-blue?style=flat)](https://www.python.org/downloads/) |
+| Supported Systems    | [![Linux](https://img.shields.io/github/actions/workflow/status/ghiggi/gpm_api/.github/workflows/tests.yml?label=Linux&style=flat)](https://github.com/ghiggi/gpm_api/actions/workflows/tests.yml) [![macOS](https://img.shields.io/github/actions/workflow/status/ghiggi/gpm_api/.github/workflows/tests.yml?label=macOS&style=flat)](https://github.com/ghiggi/gpm_api/actions/workflows/tests.yml) [![Windows](https://img.shields.io/github/actions/workflow/status/ghiggi/gpm_api/.github/workflows/tests_windows.yml?label=Windows&style=flat)](https://github.com/ghiggi/gpm_api/actions/workflows/tests_windows.yml) |
+| Project Status       | [![Project Status](https://www.repostatus.org/badges/latest/active.svg?style=flat)](https://www.repostatus.org/#active) |
+| Build Status         | [![Tests](https://github.com/ghiggi/gpm_api/actions/workflows/tests.yml/badge.svg?style=flat)](https://github.com/ghiggi/gpm_api/actions/workflows/tests.yml) [![Lint](https://github.com/ghiggi/gpm_api/actions/workflows/lint.yml/badge.svg?style=flat)](https://github.com/ghiggi/gpm_api/actions/workflows/lint.yml) [![Docs](https://readthedocs.org/projects/gpm_api/badge/?version=latest&style=flat)](https://gpm_api.readthedocs.io/en/latest/) |
+| Linting              | [![Black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat)](https://github.com/psf/black) [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json&style=flat)](https://github.com/astral-sh/ruff) [![Codespell](https://img.shields.io/badge/Codespell-enabled-brightgreen?style=flat)](https://github.com/codespell-project/codespell) |
+| Code Coverage        | [![Coveralls](https://coveralls.io/repos/github/ghiggi/gpm_api/badge.svg?branch=main&style=flat)](https://coveralls.io/github/ghiggi/gpm_api?branch=main) [![Codecov](https://codecov.io/gh/ghiggi/gpm_api/branch/main/graph/badge.svg?style=flat)](https://codecov.io/gh/ghiggi/gpm_api) |
+| Code Quality         | [![Codefactor](https://www.codefactor.io/repository/github/ghiggi/gpm_api/badge?style=flat)](https://www.codefactor.io/repository/github/ghiggi/gpm_api) [![Codebeat](https://codebeat.co/badges/236abcf2-cbae-4ca9-8a2d-3b70495bb16b?style=flat)](https://codebeat.co/projects/github-com-ghiggi-gpm_api-main) [![Codacy](https://app.codacy.com/project/badge/Grade/bee842cb10004ad8bb9288256f2fc8af?style=flat)](https://app.codacy.com/gh/ghiggi/gpm_api/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade) [![Codescene](https://codescene.io/projects/36767/status-badges/code-health?style=flat)](https://codescene.io/projects/36767) |
+| Code Review          | [![pyOpenSci](https://tinyurl.com/XXXX)](#) [![OpenSSF Best Practices](https://www.bestpractices.dev/projects/XXXX/badge?style=flat)](#) |
+| License              | [![License](https://img.shields.io/github/license/ghiggi/gpm_api?style=flat)](https://github.com/ghiggi/gpm_api/blob/main/LICENSE) |
+| Community            | [![Slack](https://img.shields.io/badge/Slack-gpm_api-green.svg?logo=slack&style=flat)](https://join.slack.com/t/gpmapi/shared_invite/zt-28vkxzjs1-~cIYci2o3G0qEEoQJVMQRg) [![GitHub Discussions](https://img.shields.io/badge/GitHub-Discussions-green?logo=github&style=flat)](https://github.com/ghiggi/gpm_api/discussions) |
+| Citation             | [![DOI](https://zenodo.org/badge/286664485.svg?style=flat)](https://doi.org/10.5281/zenodo.10255084) |
+
+ [**Slack**](https://join.slack.com/t/gpmapi/shared_invite/zt-28vkxzjs1-~cIYci2o3G0qEEoQJVMQRg) | [**Docs**](https://gpm-api.readthedocs.io/en/latest/)
 
 The GPM-API is still in development. Feel free to try it out and to report issues or to suggest changes.
 
-## Quick start
+## 🚀 Quick start
 GPM-API provides an easy-to-use python interface to download, read, process and visualize most
 of the products of the Global Precipitation Measurement Mission (GPM) data archive.
 
 The list of available products can be retrieved using:
 
 ```python
 import gpm_api
 
-gpm_api.available_products(product_type="RS")  # research products
-gpm_api.available_products(product_type="NRT") # near-real-time products
+gpm_api.available_products(product_types="RS")  # research products
+gpm_api.available_products(product_types="NRT") # near-real-time products
 
 ```
 
 Before starting using GPM-API, we highly suggest to save into a configuration file:
 1. your credentials to access the [NASA Precipitation Processing System (PPS) servers][PPS_link]
 2. the directory on the local disk where to save the GPM dataset of interest.
 
@@ -137,14 +148,17 @@
 
 # You can check that the config file has been correctly created with:
 configs = gpm_api.read_configs()
 print(configs)
 
 ```
 
+-----------------------------------------------------------------------------------------
+#### 📥 Download GPM data
+
 Now you can either start to download GPM data within python:
 
 ```python
 import gpm_api
 import datetime
 
 product = "2A-DPR"
@@ -164,14 +178,16 @@
 ```
 
 or from the terminal using i.e. `download_daily_gpm_data <product> <year> <month> <day>`:
 
 ```bash
     download_daily_gpm_data 2A-DPR 2022 7 22
 ```
+-----------------------------------------------------------------------------------------
+#### 💫 Open GPM files into xarray
 
 A GPM granule can be opened in python using:
 
 ```python
 import gpm_api
 
 ds = gpm_api.open_granule(<path_to_granule>)
@@ -193,17 +209,24 @@
 ds = gpm_api.open_dataset(product=product,
                           product_type=product_type,
                           version=version
                           start_time=start_time,
                           end_time=end_time)
 ```
 
-Look at the [Tutorials][tutorial_link] to learn how to analyse and visualize the GPM products !
+-----------------------------------------------------------------------------------------
+#### 📖 Explore the GPM-API documentation
+
+To discover all GPM-API download, manipulation, analysis and plotting utilities, or how to contribute your custom retrieval to GPM-API:
+- please read the software documentation available at [[https://disdrodb.readthedocs.io/en/latest/](https://gpm-api.readthedocs.io/en/latest/)].
+- dive into the Jupyter Notebooks [Tutorials][tutorial_link] tutorials.
 
-## Installation
+-----------------------------------------------------------------------------------------
+
+## 🛠️ Installation
 
 
 ### pip
 
 GPM-API can be installed via [pip][pip_link] on Linux, Mac, and Windows.
 On Windows you can install [WinPython][winpy_link] to get Python and pip
 running.
@@ -224,19 +247,35 @@
 
     conda install gpm_api
 
 In case conda forge is not set up for your system yet, see the easy to follow
 instructions on [conda forge][conda_forge_link].
 
 
-## Documentation for GPM-API
+## 💭 Feedback and Contributing Guidelines
+
+If you aim to contribute your data or discuss the future development of GPM-API,
+we highly suggest to join the [**GPM-API Slack Workspace**](https://join.slack.com/t/gpmapi/shared_invite/zt-28vkxzjs1-~cIYci2o3G0qEEoQJVMQRg)
+
+Feel free to also open a [GitHub Issue](https://github.com/ghiggi/gpm_api/issues) or a [GitHub Discussion](https://github.com/ghiggi/gpm_api/discussions) specific to your questions or ideas.
 
-You can find the documentation under [gpm_api.readthedocs.io][doc_link]
+## Citation
+
+You can cite the GPM-API software by:
+
+> Ghiggi Gionata & XXXX . ghiggi/gpm_api. Zenodo. https://doi.org/10.5281/zenodo.7753488
+
+If you want to cite a specific software version, have a look at the [Zenodo site](https://doi.org/10.5281/zenodo.7753488).
+
+## License
 
-### Tutorials and Examples
+The content of this repository is released under the terms of the [MIT license](LICENSE).
+
+
+### Tutorials
 
 The documentation also includes some [tutorials][tut_link], showing the most important use cases of GPM-API.
 These tutorial are also available as Jupyter Notebooks and in Google Colab:
 
 - 1. Download the GPM products [[Notebook][tut1_download_link]][[Colab][colab1_download_link]]
 - 2. Introduction to the IMERG products [[Notebook][tut2_imerg_link]][[Colab][colab2_imerg_link]]
 - 2. Introduction to the PMW 1B and 1C products [[Notebook][tut2_pmw1bc_link]][[Colab][colab_pmw1bc_link]]
@@ -246,26 +285,14 @@
 - 2. Introduction to the Latent Heating products [[Notebook][tut2_lh_link]][[Colab][colab2_lh_link]]
 - 2. Introduction to the ENVironment products [[Notebook][tut2_env_link]][[Colab][colab2_env_link]]
 - 3. Introduction to image labeling and patch extraction [[Notebook][tut3_label_link]][[Colab][colab3_label_link]]
 - 3. Introduction to image patch extraction [[Notebook][tut3_patch_link]][[Colab][colab3_patch_link]]
 
 The associated python scripts are also provided in the `tutorial` folder.
 
-## Citation
-
-If you are using GPM-API in your publication please cite our paper:
-
-TODO: GMD
-
-You can cite the Zenodo code publication of GPM-API by:
-
-> Ghiggi Gionata & XXXX . ghiggi/gpm_api. Zenodo. https://doi.org/10.5281/zenodo.7753488
-
-If you want to cite a specific version, have a look at the [Zenodo site](https://doi.org/10.5281/zenodo.7753488).
-
 ## Requirements:
 
 - [xarray](https://docs.xarray.dev/en/stable/)
 - [dask](https://www.dask.org/)
 - [cartopy](https://scitools.org.uk/cartopy/docs/latest/)
 - [pyresample](https://pyresample.readthedocs.io/en/latest/)
 - [h5py](https://github.com/h5py/h5py)
@@ -274,18 +301,14 @@
 
 ### Optional
 
 - [zarr](https://zarr.readthedocs.io/en/stable/)
 - [dask_image](https://image.dask.org/en/latest/)
 - [skimage](https://scikit-image.org/)
 
-## License
-
-The content of this repository is released under the terms of the [MIT](LICENSE) license.
-
 [PPS_link]: https://gpm.nasa.gov/data/sources/pps-research
 [tutorial_link]: https://github.com/ghiggi/gpm_api/tree/master#tutorials-and-examples
 
 [pip_link]: https://pypi.org/project/gstools
 [conda_link]: https://docs.conda.io/en/latest/miniconda.html
 [conda_forge_link]: https://github.com/conda-forge/gpm_api-feedstock#installing-gpm_api
 [conda_pip]: https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-pkgs.html#installing-non-conda-packages
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `gpm_api-0.2.8/gpm_api.egg-info/SOURCES.txt` & `gpm_api-0.2.9/gpm_api.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 gpm_api/dataset/decoding/decode_2a_radar.py
 gpm_api/dataset/decoding/routines.py
 gpm_api/dataset/decoding/utils.py
 gpm_api/encoding/__init__.py
 gpm_api/encoding/encode_2a_radar.py
 gpm_api/encoding/routines.py
 gpm_api/etc/__init__.py
+gpm_api/etc/continent_extent.yaml
 gpm_api/etc/country_acronyms.yaml
 gpm_api/etc/country_bounds.yaml
 gpm_api/etc/country_extent.yaml
 gpm_api/etc/pmw_frequency.yml
 gpm_api/etc/product_def.yml
 gpm_api/io/__init__.py
 gpm_api/io/checks.py
@@ -103,14 +104,15 @@
 gpm_api/tests/0_tmp/io/test_filter.py
 gpm_api/tests/0_tmp/io/test_find_filters.py
 gpm_api/tests/0_tmp/io/test_info.py
 gpm_api/tests/0_tmp/io/test_pps.py
 gpm_api/tests/0_tmp/visualization/test_plot_multiorbit_gmi.py
 gpm_api/tests/0_tmp/visualization/test_plot_multiorbit_pmw_polar.py
 gpm_api/tests/0_tmp/visualization/test_plot_orbit_pmw_custom_kwargs.py
+gpm_api/tests/test_accessor/test_accessor_methods.py
 gpm_api/tests/test_dataset/conftest.py
 gpm_api/tests/test_dataset/test_attrs.py
 gpm_api/tests/test_dataset/test_coords.py
 gpm_api/tests/test_dataset/test_crs.py
 gpm_api/tests/test_dataset/test_datatree.py
 gpm_api/tests/test_dataset/test_dimensions.py
 gpm_api/tests/test_dataset/test_granule.py
@@ -127,23 +129,25 @@
 gpm_api/tests/test_io/test_info.py
 gpm_api/tests/test_io/test_io_checks.py
 gpm_api/tests/test_io/test_local.py
 gpm_api/tests/test_io/test_pps.py
 gpm_api/tests/test_io/test_products.py
 gpm_api/tests/test_utils/test_geospatial.py
 gpm_api/tests/test_utils/test_list.py
+gpm_api/tests/test_utils/test_slices.py
+gpm_api/tests/test_utils/test_time.py
+gpm_api/tests/test_utils/test_utils_checks.py
+gpm_api/tests/test_utils/utils.py
 gpm_api/tests/utils/__init__.py
 gpm_api/tests/utils/hdf5.py
 gpm_api/utils/__init__.py
 gpm_api/utils/archive.py
 gpm_api/utils/area.py
 gpm_api/utils/checks.py
 gpm_api/utils/collocation.py
-gpm_api/utils/continents.py
-gpm_api/utils/countries.py
 gpm_api/utils/dask.py
 gpm_api/utils/geospatial.py
 gpm_api/utils/list.py
 gpm_api/utils/manipulations.py
 gpm_api/utils/parallel.py
 gpm_api/utils/slices.py
 gpm_api/utils/time.py
```

### Comparing `gpm_api-0.2.8/pyproject.toml` & `gpm_api-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -61,18 +61,19 @@
        "black[jupyter]", "blackdoc", "codespell", "ruff",
        "pytest", "pytest-cov", "pytest-mock", "pydantic", "pytest-check",
        "pytest-watcher", "pip-tools", "bumpver", "twine",
        "setuptools>=61.0.0", "wheel",
        "sphinx", "sphinx-gallery", "sphinx-book-theme", "nbsphinx", "sphinx_mdinclude"]
 
 [project.urls]
-Homepage = "https://github.com/ghiggi/gpm_api"
-Source = "https://github.com/ghiggi/gpm_api"
-Tracker = "https://github.com/ghiggi/gpm_api/issues"
-Documentation = "https://gpm_api.readthedocs.io"
+homepage = "https://github.com/ghiggi/gpm_api"
+repository = "https://github.com/ghiggi/gpm_api"
+source = "https://github.com/ghiggi/gpm_api"
+tracker = "https://github.com/ghiggi/gpm_api/issues"
+documentation = "https://gpm_api.readthedocs.io"
 changelog = "https://github.com/ghigg/gpm_api/CHANGELOG.md"
 
 [tool.setuptools_scm]
 write_to = "gpm_api/_version.py"
 
 [tool.setuptools]
 license-files = ["LICENSE"]
```

