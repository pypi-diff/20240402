# Comparing `tmp/junifer-0.0.4.dev85.tar.gz` & `tmp/junifer-0.0.4.dev90.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "junifer-0.0.4.dev85.tar", last modified: Mon Oct 16 14:54:19 2023, max compression
+gzip compressed data, was "junifer-0.0.4.dev90.tar", last modified: Wed Oct 18 09:16:46 2023, max compression
```

## Comparing `junifer-0.0.4.dev85.tar` & `junifer-0.0.4.dev90.tar`

### file list

```diff
@@ -1,388 +1,389 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.908304 junifer-0.0.4.dev85/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.824304 junifer-0.0.4.dev85/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.824304 junifer-0.0.4.dev85/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/.github/ISSUE_TEMPLATE/dataset-request.yml
--rw-r--r--   0 runner    (1001) docker     (127)      798 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/.github/ISSUE_TEMPLATE/documention-request.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/.github/ISSUE_TEMPLATE/feature-request.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/.github/ISSUE_TEMPLATE/marker-request.yml
--rw-r--r--   0 runner    (1001) docker     (127)      126 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.828304 junifer-0.0.4.dev85/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/.github/workflows/ci-docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/.github/workflows/docs-preview.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      503 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)      983 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      103 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      163 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)    34354 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     6792 2023-10-16 14:54:19.908304 junifer-0.0.4.dev85/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4449 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      847 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)      672 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/conda-env.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.832304 junifer-0.0.4.dev85/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.808304 junifer-0.0.4.dev85/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.832304 junifer-0.0.4.dev85/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      992 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/docs/_static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.832304 junifer-0.0.4.dev85/docs/_static/js/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/docs/_static/js/custom.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.832304 junifer-0.0.4.dev85/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      720 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/docs/_templates/versions.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.836304 junifer-0.0.4.dev85/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      230 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/docs/api/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      154 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/docs/api/configs.rst
--rw-r--r--   0 runner    (1001) docker     (127)      228 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/docs/api/data.rst
--rw-r--r--   0 runner    (1001) docker     (127)      100 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/docs/api/datagrabbers.rst
--rw-r--r--   0 runner    (1001) docker     (127)       95 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/docs/api/datareaders.rst
--rw-r--r--   0 runner    (1001) docker     (127)      503 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       84 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/docs/api/markers.rst
--rw-r--r--   0 runner    (1001) docker     (127)      175 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/docs/api/nilearn.rst
--rw-r--r--   0 runner    (1001) docker     (127)      171 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/docs/api/onthefly.rst
--rw-r--r--   0 runner    (1001) docker     (127)      162 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/docs/api/pipeline.rst
--rw-r--r--   0 runner    (1001) docker     (127)      101 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/docs/api/preprocessing.rst
--rw-r--r--   0 runner    (1001) docker     (127)       56 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/docs/api/stats.rst
--rw-r--r--   0 runner    (1001) docker     (127)       84 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/docs/api/storage.rst
--rw-r--r--   0 runner    (1001) docker     (127)       75 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/docs/api/testing.rst
--rw-r--r--   0 runner    (1001) docker     (127)       78 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/docs/api/utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)    22068 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/docs/builtin.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.836304 junifer-0.0.4.dev85/docs/changes/
--rw-r--r--   0 runner    (1001) docker     (127)      522 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/docs/changes/contributors.inc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.836304 junifer-0.0.4.dev85/docs/changes/newsfragments/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/docs/changes/newsfragments/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      114 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/docs/changes/newsfragments/182.enh
--rw-r--r--   0 runner    (1001) docker     (127)      122 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/docs/changes/newsfragments/233.bugfix
--rw-r--r--   0 runner    (1001) docker     (127)       67 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/docs/changes/newsfragments/245.change
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/docs/changes/newsfragments/245.feature
--rw-r--r--   0 runner    (1001) docker     (127)       86 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/docs/changes/newsfragments/247.doc
--rw-r--r--   0 runner    (1001) docker     (127)       79 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/docs/changes/newsfragments/248.change
--rw-r--r--   0 runner    (1001) docker     (127)      149 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/docs/changes/newsfragments/251.doc
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/docs/changes/newsfragments/253.misc
--rw-r--r--   0 runner    (1001) docker     (127)      148 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/docs/changes/newsfragments/254.feature
--rw-r--r--   0 runner    (1001) docker     (127)      125 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/docs/changes/newsfragments/258.enh
--rw-r--r--   0 runner    (1001) docker     (127)      121 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/docs/changes/newsfragments/259.enh
--rw-r--r--   0 runner    (1001) docker     (127)     5925 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     8580 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/docs/contribution.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.840304 junifer-0.0.4.dev85/docs/extending/
--rw-r--r--   0 runner    (1001) docker     (127)     5155 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/docs/extending/coordinates.rst
--rw-r--r--   0 runner    (1001) docker     (127)    16594 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/docs/extending/datagrabber.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/docs/extending/extension.rst
--rw-r--r--   0 runner    (1001) docker     (127)      843 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/docs/extending/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9803 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/docs/extending/marker.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3200 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/docs/extending/masks.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5559 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/docs/extending/parcellations.rst
--rw-r--r--   0 runner    (1001) docker     (127)      939 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/docs/faq.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4949 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/docs/help.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.840304 junifer-0.0.4.dev85/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)    62148 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/docs/images/junifer_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3326 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/docs/links.inc
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/docs/maintaining.rst
--rw-r--r--   0 runner    (1001) docker     (127)      272 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/docs/redirect.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.840304 junifer-0.0.4.dev85/docs/sphinxext/
--rw-r--r--   0 runner    (1001) docker     (127)      813 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/docs/sphinxext/gh_substitutions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8038 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/docs/starting.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.840304 junifer-0.0.4.dev85/docs/understanding/
--rw-r--r--   0 runner    (1001) docker     (127)     5098 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/docs/understanding/data.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2920 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/docs/understanding/datagrabber.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/docs/understanding/datareader.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/docs/understanding/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/docs/understanding/marker.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/docs/understanding/pipeline.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3778 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/docs/understanding/preprocess.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/docs/understanding/storage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.840304 junifer-0.0.4.dev85/docs/using/
--rw-r--r--   0 runner    (1001) docker     (127)     6383 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/docs/using/codeless.rst
--rw-r--r--   0 runner    (1001) docker     (127)      749 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/docs/using/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/docs/using/masks.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4171 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/docs/using/queueing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/docs/using/running.rst
--rw-r--r--   0 runner    (1001) docker     (127)    14813 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/docs/whats_new.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.844304 junifer-0.0.4.dev85/examples/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/examples/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/examples/norun_hcpfc_pearson.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/examples/norun_ukbvm_gmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/examples/run_compute_parcel_mean.py
--rw-r--r--   0 runner    (1001) docker     (127)     2224 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/examples/run_datagrabber_bids_datalad.py
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/examples/run_ets_rss_marker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3659 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/examples/run_junifer_julearn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/examples/run_run_gmd_mean.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.844304 junifer-0.0.4.dev85/examples/yamls/
--rw-r--r--   0 runner    (1001) docker     (127)      594 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/examples/yamls/gmd_mean.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      417 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/examples/yamls/gmd_mean_htcondor.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      574 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/examples/yamls/ukb_gmd_mean.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/ignore_words.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.844304 junifer-0.0.4.dev85/junifer/
--rw-r--r--   0 runner    (1001) docker     (127)      391 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2023-10-16 14:54:19.000000 junifer-0.0.4.dev85/junifer/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.848304 junifer-0.0.4.dev85/junifer/api/
--rw-r--r--   0 runner    (1001) docker     (127)      257 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11286 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/api/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/api/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)    22716 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/api/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3308 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/api/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.848304 junifer-0.0.4.dev85/junifer/api/res/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.848304 junifer-0.0.4.dev85/junifer/api/res/afni/
--rwxr-xr-x   0 runner    (1001) docker     (127)       51 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/api/res/afni/3dAFNItoNIFTI
--rwxr-xr-x   0 runner    (1001) docker     (127)       44 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/api/res/afni/3dRSFC
--rwxr-xr-x   0 runner    (1001) docker     (127)       44 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/api/res/afni/3dReHo
--rwxr-xr-x   0 runner    (1001) docker     (127)       42 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/api/res/afni/afni
--rwxr-xr-x   0 runner    (1001) docker     (127)     1106 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/api/res/afni/run_afni_docker.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      501 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/api/res/run_conda.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.852304 junifer-0.0.4.dev85/junifer/api/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.852304 junifer-0.0.4.dev85/junifer/api/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)      330 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/api/tests/data/gmd_mean.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      417 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/api/tests/data/gmd_mean_htcondor.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/api/tests/test_api_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5717 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/api/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    24631 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/api/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6107 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/api/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.852304 junifer-0.0.4.dev85/junifer/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/configs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.852304 junifer-0.0.4.dev85/junifer/configs/juseless/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/configs/juseless/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.852304 junifer-0.0.4.dev85/junifer/configs/juseless/datagrabbers/
--rw-r--r--   0 runner    (1001) docker     (127)      452 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/configs/juseless/datagrabbers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/configs/juseless/datagrabbers/aomic_id1000_vbm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/configs/juseless/datagrabbers/camcan_vbm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2184 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/configs/juseless/datagrabbers/ixi_vbm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.852304 junifer-0.0.4.dev85/junifer/configs/juseless/datagrabbers/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/configs/juseless/datagrabbers/tests/test_aomic_id1000_vbm.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/configs/juseless/datagrabbers/tests/test_camcan_vbm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/configs/juseless/datagrabbers/tests/test_ixi_vbm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/configs/juseless/datagrabbers/tests/test_ucla.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/configs/juseless/datagrabbers/tests/test_ukb_vbm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4302 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/configs/juseless/datagrabbers/ucla.py
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/configs/juseless/datagrabbers/ukb_vbm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.856304 junifer-0.0.4.dev85/junifer/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.812304 junifer-0.0.4.dev85/junifer/data/VOIs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.860304 junifer-0.0.4.dev85/junifer/data/VOIs/meta/
--rw-r--r--   0 runner    (1001) docker     (127)      398 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/data/VOIs/meta/CogAC_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      189 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/data/VOIs/meta/CogAR_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/data/VOIs/meta/DMNBuckner_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3372 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/data/VOIs/meta/Dosenbach2010_MNI_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      486 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/data/VOIs/meta/Empathy_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      219 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/data/VOIs/meta/Motor_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      220 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/data/VOIs/meta/MultiTask_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      378 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/data/VOIs/meta/PhysioStress_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3836 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/data/VOIs/meta/Power2011_MNI_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3836 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/data/VOIs/meta/Power2013_MNI_VOIs.tsv
--rw-r--r--   0 runner    (1001) docker     (127)      569 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/data/VOIs/meta/Rew_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      295 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/data/VOIs/meta/Somatosensory_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      323 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/data/VOIs/meta/ToM_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      353 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/data/VOIs/meta/VigAtt_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      518 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/data/VOIs/meta/WM_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      382 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/data/VOIs/meta/eMDN_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      268 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/data/VOIs/meta/eSAD_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      317 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/data/VOIs/meta/extDMN_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      507 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5485 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/data/coordinates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.816304 junifer-0.0.4.dev85/junifer/data/masks/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.860304 junifer-0.0.4.dev85/junifer/data/masks/vickery-patil/
--rw-r--r--   0 runner    (1001) docker     (127)    88270 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)    12862 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean_3mm.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)     8700 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/data/masks/vickery-patil/GMprob0.2_cortex_3mm_NA_rm.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)    11280 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/data/masks.py
--rw-r--r--   0 runner    (1001) docker     (127)    48818 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/data/parcellations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.860304 junifer-0.0.4.dev85/junifer/data/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3240 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/data/tests/test_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/data/tests/test_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13269 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/data/tests/test_masks.py
--rw-r--r--   0 runner    (1001) docker     (127)    31361 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/data/tests/test_parcellations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.864304 junifer-0.0.4.dev85/junifer/datagrabber/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/datagrabber/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.864304 junifer-0.0.4.dev85/junifer/datagrabber/aomic/
--rw-r--r--   0 runner    (1001) docker     (127)      281 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/datagrabber/aomic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4320 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/datagrabber/aomic/id1000.py
--rw-r--r--   0 runner    (1001) docker     (127)     6252 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/datagrabber/aomic/piop1.py
--rw-r--r--   0 runner    (1001) docker     (127)     5871 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/datagrabber/aomic/piop2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.864304 junifer-0.0.4.dev85/junifer/datagrabber/aomic/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4824 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/datagrabber/aomic/tests/test_id1000.py
--rw-r--r--   0 runner    (1001) docker     (127)     5578 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/datagrabber/aomic/tests/test_piop1.py
--rw-r--r--   0 runner    (1001) docker     (127)     5377 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/datagrabber/aomic/tests/test_piop2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6016 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/datagrabber/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    10731 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/datagrabber/datalad_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.864304 junifer-0.0.4.dev85/junifer/datagrabber/hcp1200/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/datagrabber/hcp1200/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/datagrabber/hcp1200/datalad_hcp1200.py
--rw-r--r--   0 runner    (1001) docker     (127)     5575 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/datagrabber/hcp1200/hcp1200.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.868304 junifer-0.0.4.dev85/junifer/datagrabber/hcp1200/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    10765 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/datagrabber/hcp1200/tests/test_hcp1200.py
--rw-r--r--   0 runner    (1001) docker     (127)     4923 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/datagrabber/multiple.py
--rw-r--r--   0 runner    (1001) docker     (127)    10519 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/datagrabber/pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/datagrabber/pattern_datalad.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.868304 junifer-0.0.4.dev85/junifer/datagrabber/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3738 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/datagrabber/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/datagrabber/tests/test_datagrabber_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16496 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/datagrabber/tests/test_datalad_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4955 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/datagrabber/tests/test_multiple.py
--rw-r--r--   0 runner    (1001) docker     (127)     9823 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/datagrabber/tests/test_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     6077 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/datagrabber/tests/test_pattern_datalad.py
--rw-r--r--   0 runner    (1001) docker     (127)     2828 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/datagrabber/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.868304 junifer-0.0.4.dev85/junifer/datareader/
--rw-r--r--   0 runner    (1001) docker     (127)      263 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/datareader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4068 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/datareader/default.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.868304 junifer-0.0.4.dev85/junifer/datareader/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5220 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/datareader/tests/test_default_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.868304 junifer-0.0.4.dev85/junifer/external/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/external/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.816304 junifer-0.0.4.dev85/junifer/external/h5io/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.872304 junifer-0.0.4.dev85/junifer/external/h5io/h5io/
--rw-r--r--   0 runner    (1001) docker     (127)      469 2023-10-16 14:54:05.000000 junifer-0.0.4.dev85/junifer/external/h5io/h5io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28748 2023-10-16 14:54:05.000000 junifer-0.0.4.dev85/junifer/external/h5io/h5io/_h5io.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-10-16 14:54:05.000000 junifer-0.0.4.dev85/junifer/external/h5io/h5io/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2023-10-16 14:54:05.000000 junifer-0.0.4.dev85/junifer/external/h5io/h5io/chunked_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2023-10-16 14:54:05.000000 junifer-0.0.4.dev85/junifer/external/h5io/h5io/chunked_list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.872304 junifer-0.0.4.dev85/junifer/external/nilearn/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/external/nilearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16272 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/external/nilearn/junifer_nifti_spheres_masker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.872304 junifer-0.0.4.dev85/junifer/external/nilearn/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    10370 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/external/nilearn/tests/test_junifer_nifti_spheres_masker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.876304 junifer-0.0.4.dev85/junifer/markers/
--rw-r--r--   0 runner    (1001) docker     (127)      778 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/markers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6109 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/markers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4592 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/markers/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4557 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/markers/ets_rss.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.876304 junifer-0.0.4.dev85/junifer/markers/falff/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/markers/falff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6001 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/markers/falff/falff_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    10620 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/markers/falff/falff_estimator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4550 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/markers/falff/falff_parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     5086 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/markers/falff/falff_spheres.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.876304 junifer-0.0.4.dev85/junifer/markers/falff/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8020 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/markers/falff/tests/test_falff_estimator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4738 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/markers/falff/tests/test_falff_parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     4825 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/markers/falff/tests/test_falff_spheres.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.880304 junifer-0.0.4.dev85/junifer/markers/functional_connectivity/
--rw-r--r--   0 runner    (1001) docker     (127)      499 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/markers/functional_connectivity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5214 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/markers/functional_connectivity/crossparcellation_functional_connectivity.py
--rw-r--r--   0 runner    (1001) docker     (127)     4338 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/markers/functional_connectivity/edge_functional_connectivity_parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     4994 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/markers/functional_connectivity/edge_functional_connectivity_spheres.py
--rw-r--r--   0 runner    (1001) docker     (127)     5178 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/markers/functional_connectivity/functional_connectivity_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3990 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/markers/functional_connectivity/functional_connectivity_parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     4690 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/markers/functional_connectivity/functional_connectivity_spheres.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.880304 junifer-0.0.4.dev85/junifer/markers/functional_connectivity/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2872 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/markers/functional_connectivity/tests/test_crossparcellation_functional_connectivity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_spheres.py
--rw-r--r--   0 runner    (1001) docker     (127)      522 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/markers/functional_connectivity/tests/test_functional_connectivity_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3118 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/markers/functional_connectivity/tests/test_functional_connectivity_parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     4170 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/markers/functional_connectivity/tests/test_functional_connectivity_spheres.py
--rw-r--r--   0 runner    (1001) docker     (127)     8648 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/markers/parcel_aggregation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.880304 junifer-0.0.4.dev85/junifer/markers/reho/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/markers/reho/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3704 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/markers/reho/reho_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    17921 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/markers/reho/reho_estimator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5761 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/markers/reho/reho_parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     6278 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/markers/reho/reho_spheres.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.884304 junifer-0.0.4.dev85/junifer/markers/reho/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8997 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/markers/reho/tests/test_reho_estimator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4812 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/markers/reho/tests/test_reho_parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     4820 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/markers/reho/tests/test_reho_spheres.py
--rw-r--r--   0 runner    (1001) docker     (127)     7372 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/markers/sphere_aggregation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.884304 junifer-0.0.4.dev85/junifer/markers/temporal_snr/
--rw-r--r--   0 runner    (1001) docker     (127)      243 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/markers/temporal_snr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4023 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/markers/temporal_snr/temporal_snr_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3299 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/markers/temporal_snr/temporal_snr_parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     4007 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/markers/temporal_snr/temporal_snr_spheres.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.884304 junifer-0.0.4.dev85/junifer/markers/temporal_snr/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      426 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/markers/temporal_snr/tests/test_temporal_snr_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/markers/temporal_snr/tests/test_temporal_snr_parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/markers/temporal_snr/tests/test_temporal_snr_spheres.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.884304 junifer-0.0.4.dev85/junifer/markers/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6853 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/markers/tests/test_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2619 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/markers/tests/test_ets_rss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/markers/tests/test_marker_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/markers/tests/test_markers_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    21501 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/markers/tests/test_parcel_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/markers/tests/test_sphere_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3777 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/markers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.888304 junifer-0.0.4.dev85/junifer/onthefly/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/onthefly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4309 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/onthefly/read_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.888304 junifer-0.0.4.dev85/junifer/onthefly/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4719 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/onthefly/tests/test_read_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.888304 junifer-0.0.4.dev85/junifer/pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)      282 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5019 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/pipeline/pipeline_step_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3956 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/pipeline/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)      985 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/pipeline/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.892304 junifer-0.0.4.dev85/junifer/pipeline/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5393 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/pipeline/tests/test_pipeline_step_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4105 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/pipeline/tests/test_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/pipeline/tests/test_update_meta_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2801 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/pipeline/tests/test_workdir_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/pipeline/update_meta_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3515 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/pipeline/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7972 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/pipeline/workdir_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.892304 junifer-0.0.4.dev85/junifer/preprocess/
--rw-r--r--   0 runner    (1001) docker     (127)      255 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/preprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5493 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/preprocess/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.892304 junifer-0.0.4.dev85/junifer/preprocess/confounds/
--rw-r--r--   0 runner    (1001) docker     (127)      235 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/preprocess/confounds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21922 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/preprocess/confounds/fmriprep_confound_remover.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.892304 junifer-0.0.4.dev85/junifer/preprocess/confounds/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    21578 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/preprocess/confounds/tests/test_fmriprep_confound_remover.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.892304 junifer-0.0.4.dev85/junifer/preprocess/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/preprocess/tests/test_preprocess_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5879 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.896304 junifer-0.0.4.dev85/junifer/storage/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9459 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/storage/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    35520 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/storage/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)     7473 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/storage/pandas_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    21243 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/storage/sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.896304 junifer-0.0.4.dev85/junifer/storage/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    29337 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/storage/tests/test_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)     4058 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/storage/tests/test_pandas_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    28318 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/storage/tests/test_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     3071 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/storage/tests/test_storage_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11853 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/storage/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7257 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/storage/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.896304 junifer-0.0.4.dev85/junifer/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      235 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.896304 junifer-0.0.4.dev85/junifer/testing/data/
--rw-r--r--   0 runner    (1001) docker     (127)   406849 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/testing/data/sub-0001_task-anticipation_acq-seq_desc-confounds_regressors.tsv
--rw-r--r--   0 runner    (1001) docker     (127)     6366 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/testing/datagrabbers.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/testing/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.900304 junifer-0.0.4.dev85/junifer/testing/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      794 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/testing/tests/test_oasisvmbtesting_datagrabber.py
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/testing/tests/test_partlycloudytesting_datagrabber.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/testing/tests/test_spmauditory_datagrabber.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/testing/tests/test_testing_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)      557 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/testing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.900304 junifer-0.0.4.dev85/junifer/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      373 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     4093 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/tests/test_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.900304 junifer-0.0.4.dev85/junifer/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/utils/fs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8994 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/utils/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.900304 junifer-0.0.4.dev85/junifer/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      923 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/utils/tests/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7754 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/junifer/utils/tests/test_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.848304 junifer-0.0.4.dev85/junifer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6792 2023-10-16 14:54:19.000000 junifer-0.0.4.dev85/junifer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11443 2023-10-16 14:54:19.000000 junifer-0.0.4.dev85/junifer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-16 14:54:19.000000 junifer-0.0.4.dev85/junifer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2023-10-16 14:54:19.000000 junifer-0.0.4.dev85/junifer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      525 2023-10-16 14:54:19.000000 junifer-0.0.4.dev85/junifer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-10-16 14:54:19.000000 junifer-0.0.4.dev85/junifer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5315 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-16 14:54:19.908304 junifer-0.0.4.dev85/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      273 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 14:54:19.904304 junifer-0.0.4.dev85/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     3643 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/tools/create_aomic1000_example_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3840 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/tools/create_aomicpiop1_example_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3762 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/tools/create_aomicpiop2_example_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      999 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/tools/create_bids_example_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/tools/create_bids_example_dataset_sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2773 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/tools/create_hcp1200_example_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2023-10-16 14:54:04.000000 junifer-0.0.4.dev85/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.159799 junifer-0.0.4.dev90/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.119799 junifer-0.0.4.dev90/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.119799 junifer-0.0.4.dev90/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/.github/ISSUE_TEMPLATE/dataset-request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/.github/ISSUE_TEMPLATE/documention-request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/.github/ISSUE_TEMPLATE/feature-request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/.github/ISSUE_TEMPLATE/marker-request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.119799 junifer-0.0.4.dev90/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/.github/workflows/ci-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/.github/workflows/docs-preview.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    34354 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6792 2023-10-18 09:16:46.159799 junifer-0.0.4.dev90/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4449 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/conda-env.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.123798 junifer-0.0.4.dev90/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.099798 junifer-0.0.4.dev90/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.123798 junifer-0.0.4.dev90/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/_static/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.123798 junifer-0.0.4.dev90/docs/_static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/_static/js/custom.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.123798 junifer-0.0.4.dev90/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/_templates/versions.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.123798 junifer-0.0.4.dev90/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/api/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/api/configs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/api/data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/api/datagrabbers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/api/datareaders.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/api/markers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/api/nilearn.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/api/onthefly.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/api/pipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/api/preprocessing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/api/stats.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/api/storage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/api/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/api/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    22068 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/builtin.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.123798 junifer-0.0.4.dev90/docs/changes/
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/changes/contributors.inc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.123798 junifer-0.0.4.dev90/docs/changes/newsfragments/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/changes/newsfragments/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/changes/newsfragments/182.enh
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/changes/newsfragments/233.bugfix
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/changes/newsfragments/245.change
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/changes/newsfragments/245.feature
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/changes/newsfragments/247.doc
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/changes/newsfragments/248.change
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/changes/newsfragments/251.doc
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/changes/newsfragments/253.misc
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/changes/newsfragments/254.feature
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/changes/newsfragments/258.enh
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/changes/newsfragments/259.enh
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/changes/newsfragments/261.misc
+-rw-r--r--   0 runner    (1001) docker     (127)     5925 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8580 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/contribution.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.127799 junifer-0.0.4.dev90/docs/extending/
+-rw-r--r--   0 runner    (1001) docker     (127)     5155 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/extending/coordinates.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    16594 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/extending/datagrabber.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/extending/extension.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/extending/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9803 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/extending/marker.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3200 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/extending/masks.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5559 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/extending/parcellations.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4949 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/help.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.127799 junifer-0.0.4.dev90/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    62148 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/images/junifer_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3326 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/links.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/maintaining.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/redirect.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.127799 junifer-0.0.4.dev90/docs/sphinxext/
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/sphinxext/gh_substitutions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8038 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/starting.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.127799 junifer-0.0.4.dev90/docs/understanding/
+-rw-r--r--   0 runner    (1001) docker     (127)     5098 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/understanding/data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2920 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/understanding/datagrabber.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/understanding/datareader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/understanding/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/understanding/marker.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/understanding/pipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3778 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/understanding/preprocess.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/understanding/storage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.127799 junifer-0.0.4.dev90/docs/using/
+-rw-r--r--   0 runner    (1001) docker     (127)     6383 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/using/codeless.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/using/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/using/masks.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4171 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/using/queueing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/using/running.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    14813 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/whats_new.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.127799 junifer-0.0.4.dev90/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/examples/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/examples/norun_hcpfc_pearson.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/examples/norun_ukbvm_gmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/examples/run_compute_parcel_mean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2224 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/examples/run_datagrabber_bids_datalad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/examples/run_ets_rss_marker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3659 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/examples/run_junifer_julearn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/examples/run_run_gmd_mean.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.127799 junifer-0.0.4.dev90/examples/yamls/
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/examples/yamls/gmd_mean.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/examples/yamls/gmd_mean_htcondor.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/examples/yamls/ukb_gmd_mean.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/ignore_words.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.131799 junifer-0.0.4.dev90/junifer/
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2023-10-18 09:16:45.000000 junifer-0.0.4.dev90/junifer/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.131799 junifer-0.0.4.dev90/junifer/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11286 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/api/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/api/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22716 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/api/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3308 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/api/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.131799 junifer-0.0.4.dev90/junifer/api/res/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.131799 junifer-0.0.4.dev90/junifer/api/res/afni/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       51 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/api/res/afni/3dAFNItoNIFTI
+-rwxr-xr-x   0 runner    (1001) docker     (127)       44 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/api/res/afni/3dRSFC
+-rwxr-xr-x   0 runner    (1001) docker     (127)       44 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/api/res/afni/3dReHo
+-rwxr-xr-x   0 runner    (1001) docker     (127)       42 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/api/res/afni/afni
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1106 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/api/res/afni/run_afni_docker.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      501 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/api/res/run_conda.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.131799 junifer-0.0.4.dev90/junifer/api/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.131799 junifer-0.0.4.dev90/junifer/api/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/api/tests/data/gmd_mean.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/api/tests/data/gmd_mean_htcondor.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/api/tests/test_api_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5717 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/api/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24631 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/api/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6107 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/api/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.131799 junifer-0.0.4.dev90/junifer/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/configs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.131799 junifer-0.0.4.dev90/junifer/configs/juseless/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/configs/juseless/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.135799 junifer-0.0.4.dev90/junifer/configs/juseless/datagrabbers/
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/configs/juseless/datagrabbers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/configs/juseless/datagrabbers/aomic_id1000_vbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/configs/juseless/datagrabbers/camcan_vbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2184 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/configs/juseless/datagrabbers/ixi_vbm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.135799 junifer-0.0.4.dev90/junifer/configs/juseless/datagrabbers/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/configs/juseless/datagrabbers/tests/test_aomic_id1000_vbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/configs/juseless/datagrabbers/tests/test_camcan_vbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/configs/juseless/datagrabbers/tests/test_ixi_vbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3351 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/configs/juseless/datagrabbers/tests/test_ucla.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/configs/juseless/datagrabbers/tests/test_ukb_vbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4302 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/configs/juseless/datagrabbers/ucla.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/configs/juseless/datagrabbers/ukb_vbm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.135799 junifer-0.0.4.dev90/junifer/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.107798 junifer-0.0.4.dev90/junifer/data/VOIs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.135799 junifer-0.0.4.dev90/junifer/data/VOIs/meta/
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/data/VOIs/meta/CogAC_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/data/VOIs/meta/CogAR_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/data/VOIs/meta/DMNBuckner_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3372 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/data/VOIs/meta/Dosenbach2010_MNI_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/data/VOIs/meta/Empathy_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/data/VOIs/meta/Motor_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/data/VOIs/meta/MultiTask_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/data/VOIs/meta/PhysioStress_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3836 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/data/VOIs/meta/Power2011_MNI_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3836 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/data/VOIs/meta/Power2013_MNI_VOIs.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/data/VOIs/meta/Rew_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/data/VOIs/meta/Somatosensory_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/data/VOIs/meta/ToM_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/data/VOIs/meta/VigAtt_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/data/VOIs/meta/WM_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/data/VOIs/meta/eMDN_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/data/VOIs/meta/eSAD_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/data/VOIs/meta/extDMN_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5485 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/data/coordinates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.107798 junifer-0.0.4.dev90/junifer/data/masks/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.135799 junifer-0.0.4.dev90/junifer/data/masks/vickery-patil/
+-rw-r--r--   0 runner    (1001) docker     (127)    88270 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    12862 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean_3mm.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     8700 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/data/masks/vickery-patil/GMprob0.2_cortex_3mm_NA_rm.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    11280 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/data/masks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48818 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/data/parcellations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.139799 junifer-0.0.4.dev90/junifer/data/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3240 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/data/tests/test_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/data/tests/test_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13269 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/data/tests/test_masks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31361 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/data/tests/test_parcellations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.139799 junifer-0.0.4.dev90/junifer/datagrabber/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/datagrabber/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.139799 junifer-0.0.4.dev90/junifer/datagrabber/aomic/
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/datagrabber/aomic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4320 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/datagrabber/aomic/id1000.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6252 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/datagrabber/aomic/piop1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5871 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/datagrabber/aomic/piop2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.139799 junifer-0.0.4.dev90/junifer/datagrabber/aomic/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4824 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/datagrabber/aomic/tests/test_id1000.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5578 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/datagrabber/aomic/tests/test_piop1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5377 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/datagrabber/aomic/tests/test_piop2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6016 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/datagrabber/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10731 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/datagrabber/datalad_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.139799 junifer-0.0.4.dev90/junifer/datagrabber/hcp1200/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/datagrabber/hcp1200/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/datagrabber/hcp1200/datalad_hcp1200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5575 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/datagrabber/hcp1200/hcp1200.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.139799 junifer-0.0.4.dev90/junifer/datagrabber/hcp1200/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    10765 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/datagrabber/hcp1200/tests/test_hcp1200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4923 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/datagrabber/multiple.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10519 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/datagrabber/pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/datagrabber/pattern_datalad.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.139799 junifer-0.0.4.dev90/junifer/datagrabber/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3738 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/datagrabber/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/datagrabber/tests/test_datagrabber_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16496 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/datagrabber/tests/test_datalad_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4955 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/datagrabber/tests/test_multiple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9823 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/datagrabber/tests/test_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6077 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/datagrabber/tests/test_pattern_datalad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/datagrabber/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.139799 junifer-0.0.4.dev90/junifer/datareader/
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/datareader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4068 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/datareader/default.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.139799 junifer-0.0.4.dev90/junifer/datareader/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5220 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/datareader/tests/test_default_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.139799 junifer-0.0.4.dev90/junifer/external/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/external/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.111798 junifer-0.0.4.dev90/junifer/external/h5io/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.143799 junifer-0.0.4.dev90/junifer/external/h5io/h5io/
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/external/h5io/h5io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28748 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/external/h5io/h5io/_h5io.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/external/h5io/h5io/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/external/h5io/h5io/chunked_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/external/h5io/h5io/chunked_list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.143799 junifer-0.0.4.dev90/junifer/external/nilearn/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/external/nilearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16272 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/external/nilearn/junifer_nifti_spheres_masker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.143799 junifer-0.0.4.dev90/junifer/external/nilearn/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    10370 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/external/nilearn/tests/test_junifer_nifti_spheres_masker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.143799 junifer-0.0.4.dev90/junifer/markers/
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6109 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4592 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4557 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/ets_rss.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.143799 junifer-0.0.4.dev90/junifer/markers/falff/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/falff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6001 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/falff/falff_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10620 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/falff/falff_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4550 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/falff/falff_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5086 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/falff/falff_spheres.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.143799 junifer-0.0.4.dev90/junifer/markers/falff/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8020 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/falff/tests/test_falff_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4738 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/falff/tests/test_falff_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4825 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/falff/tests/test_falff_spheres.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.143799 junifer-0.0.4.dev90/junifer/markers/functional_connectivity/
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/functional_connectivity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5214 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/functional_connectivity/crossparcellation_functional_connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4338 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/functional_connectivity/edge_functional_connectivity_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4994 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/functional_connectivity/edge_functional_connectivity_spheres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5178 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/functional_connectivity/functional_connectivity_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3990 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/functional_connectivity/functional_connectivity_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4690 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/functional_connectivity/functional_connectivity_spheres.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.147799 junifer-0.0.4.dev90/junifer/markers/functional_connectivity/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2872 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/functional_connectivity/tests/test_crossparcellation_functional_connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_spheres.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/functional_connectivity/tests/test_functional_connectivity_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3118 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/functional_connectivity/tests/test_functional_connectivity_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4170 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/functional_connectivity/tests/test_functional_connectivity_spheres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8648 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/parcel_aggregation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.147799 junifer-0.0.4.dev90/junifer/markers/reho/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/reho/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3704 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/reho/reho_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17921 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/reho/reho_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5761 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/reho/reho_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6278 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/reho/reho_spheres.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.147799 junifer-0.0.4.dev90/junifer/markers/reho/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8997 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/reho/tests/test_reho_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4812 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/reho/tests/test_reho_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4820 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/reho/tests/test_reho_spheres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7372 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/sphere_aggregation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.147799 junifer-0.0.4.dev90/junifer/markers/temporal_snr/
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/temporal_snr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4023 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/temporal_snr/temporal_snr_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3299 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/temporal_snr/temporal_snr_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4007 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/temporal_snr/temporal_snr_spheres.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.147799 junifer-0.0.4.dev90/junifer/markers/temporal_snr/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/temporal_snr/tests/test_temporal_snr_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/temporal_snr/tests/test_temporal_snr_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/temporal_snr/tests/test_temporal_snr_spheres.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.147799 junifer-0.0.4.dev90/junifer/markers/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6853 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/tests/test_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/tests/test_ets_rss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/tests/test_marker_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/tests/test_markers_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21501 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/tests/test_parcel_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/tests/test_sphere_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3777 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.147799 junifer-0.0.4.dev90/junifer/onthefly/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/onthefly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4309 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/onthefly/read_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.147799 junifer-0.0.4.dev90/junifer/onthefly/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4719 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/onthefly/tests/test_read_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.151799 junifer-0.0.4.dev90/junifer/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5019 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/pipeline/pipeline_step_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3956 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/pipeline/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/pipeline/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.151799 junifer-0.0.4.dev90/junifer/pipeline/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5393 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/pipeline/tests/test_pipeline_step_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4105 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/pipeline/tests/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/pipeline/tests/test_update_meta_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2801 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/pipeline/tests/test_workdir_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/pipeline/update_meta_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3515 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/pipeline/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7972 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/pipeline/workdir_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.151799 junifer-0.0.4.dev90/junifer/preprocess/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/preprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5493 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/preprocess/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.151799 junifer-0.0.4.dev90/junifer/preprocess/confounds/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/preprocess/confounds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21922 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/preprocess/confounds/fmriprep_confound_remover.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.151799 junifer-0.0.4.dev90/junifer/preprocess/confounds/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    21578 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/preprocess/confounds/tests/test_fmriprep_confound_remover.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.151799 junifer-0.0.4.dev90/junifer/preprocess/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/preprocess/tests/test_preprocess_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5879 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.151799 junifer-0.0.4.dev90/junifer/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9459 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/storage/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35520 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/storage/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7473 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/storage/pandas_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21243 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/storage/sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.151799 junifer-0.0.4.dev90/junifer/storage/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    29337 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/storage/tests/test_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4058 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/storage/tests/test_pandas_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28318 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/storage/tests/test_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3071 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/storage/tests/test_storage_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11853 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/storage/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7257 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/storage/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.151799 junifer-0.0.4.dev90/junifer/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.151799 junifer-0.0.4.dev90/junifer/testing/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   406849 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/testing/data/sub-0001_task-anticipation_acq-seq_desc-confounds_regressors.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)     6366 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/testing/datagrabbers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/testing/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.155799 junifer-0.0.4.dev90/junifer/testing/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/testing/tests/test_oasisvmbtesting_datagrabber.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/testing/tests/test_partlycloudytesting_datagrabber.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/testing/tests/test_spmauditory_datagrabber.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/testing/tests/test_testing_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/testing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.155799 junifer-0.0.4.dev90/junifer/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4093 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/tests/test_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.155799 junifer-0.0.4.dev90/junifer/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/utils/fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8994 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/utils/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.155799 junifer-0.0.4.dev90/junifer/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/utils/tests/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7754 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/utils/tests/test_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.131799 junifer-0.0.4.dev90/junifer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6792 2023-10-18 09:16:46.000000 junifer-0.0.4.dev90/junifer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11479 2023-10-18 09:16:46.000000 junifer-0.0.4.dev90/junifer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-18 09:16:46.000000 junifer-0.0.4.dev90/junifer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2023-10-18 09:16:46.000000 junifer-0.0.4.dev90/junifer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2023-10-18 09:16:46.000000 junifer-0.0.4.dev90/junifer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2023-10-18 09:16:46.000000 junifer-0.0.4.dev90/junifer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5315 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-18 09:16:46.159799 junifer-0.0.4.dev90/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.155799 junifer-0.0.4.dev90/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     3643 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/tools/create_aomic1000_example_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3840 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/tools/create_aomicpiop1_example_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3762 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/tools/create_aomicpiop2_example_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/tools/create_bids_example_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/tools/create_bids_example_dataset_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2773 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/tools/create_hcp1200_example_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/tox.ini
```

### Comparing `junifer-0.0.4.dev85/.github/ISSUE_TEMPLATE/bug-report.yml` & `junifer-0.0.4.dev90/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/.github/ISSUE_TEMPLATE/dataset-request.yml` & `junifer-0.0.4.dev90/.github/ISSUE_TEMPLATE/dataset-request.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/.github/ISSUE_TEMPLATE/documention-request.yml` & `junifer-0.0.4.dev90/.github/ISSUE_TEMPLATE/documention-request.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/.github/ISSUE_TEMPLATE/feature-request.yml` & `junifer-0.0.4.dev90/.github/ISSUE_TEMPLATE/feature-request.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/.github/ISSUE_TEMPLATE/marker-request.yml` & `junifer-0.0.4.dev90/.github/ISSUE_TEMPLATE/marker-request.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/.github/workflows/ci-docs.yml` & `junifer-0.0.4.dev90/.github/workflows/ci-docs.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/.github/workflows/ci.yml` & `junifer-0.0.4.dev90/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/.github/workflows/docs-preview.yml` & `junifer-0.0.4.dev90/.github/workflows/docs-preview.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/.github/workflows/docs.yml` & `junifer-0.0.4.dev90/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/.github/workflows/pypi.yml` & `junifer-0.0.4.dev90/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/.gitignore` & `junifer-0.0.4.dev90/.gitignore`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/.pre-commit-config.yaml` & `junifer-0.0.4.dev90/.pre-commit-config.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 ci:
   autofix_prs: false
   autoupdate_commit_msg: "chore: bump pre-commit repositories"
 
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.4.0
+    rev: v4.5.0
     hooks:
       - id: check-ast
       - id: check-docstring-first
       - id: check-executables-have-shebangs
       - id: check-merge-conflict
       - id: check-yaml
       - id: check-toml
       - id: debug-statements
       - id: end-of-file-fixer
       - id: trailing-whitespace
         args: [--markdown-linebreak-ext=md]
   - repo: https://github.com/abravalheri/validate-pyproject
-    rev: v0.12.2
+    rev: v0.15
     hooks:
       - id: validate-pyproject
   - repo: https://github.com/psf/black
-    rev: 23.3.0
+    rev: 23.9.1
     hooks:
       - id: black
         exclude: ^(docs/|examples/|tools/)
         args: [--check]
-  - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.267
+  - repo: https://github.com/astral-sh/ruff-pre-commit
+    rev: v0.1.0
     hooks:
       - id: ruff
+        types_or: [python, jupyter]
         exclude: ^(__init__.py)
-        args: [--format, grouped, --show-fixes]
+        args: [--output-format, grouped, --show-fixes]
   - repo: https://github.com/codespell-project/codespell
-    rev: v2.2.4
+    rev: v2.2.6
     hooks:
       - id: codespell
         exclude: ^(.github/|docs/)
         args: [--config, tox.ini]
   - repo: https://github.com/pre-commit/pygrep-hooks
     rev: v1.10.0
     hooks:
```

### Comparing `junifer-0.0.4.dev85/LICENSE.md` & `junifer-0.0.4.dev90/LICENSE.md`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/PKG-INFO` & `junifer-0.0.4.dev90/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: junifer
-Version: 0.0.4.dev85
+Version: 0.0.4.dev90
 Summary: JUelich NeuroImaging FEature extractoR
 Author-email: Fede Raimondo <f.raimondo@fz-juelich.de>, Synchon Mandal <s.mandal@fz-juelich.de>
 Maintainer-email: Fede Raimondo <f.raimondo@fz-juelich.de>, Synchon Mandal <s.mandal@fz-juelich.de>
 License: AGPL-3.0-only
 Project-URL: homepage, https://juaml.github.io/junifer
 Project-URL: documentation, https://juaml.github.io/junifer
 Project-URL: repository, https://github.com/juaml/junifer
```

### Comparing `junifer-0.0.4.dev85/README.md` & `junifer-0.0.4.dev90/README.md`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/codecov.yml` & `junifer-0.0.4.dev90/codecov.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/conda-env.yml` & `junifer-0.0.4.dev90/conda-env.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/docs/Makefile` & `junifer-0.0.4.dev90/docs/Makefile`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/docs/_static/css/custom.css` & `junifer-0.0.4.dev90/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/docs/_templates/versions.html` & `junifer-0.0.4.dev90/docs/_templates/versions.html`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/docs/builtin.rst` & `junifer-0.0.4.dev90/docs/builtin.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/docs/changes/contributors.inc` & `junifer-0.0.4.dev90/docs/changes/contributors.inc`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/docs/conf.py` & `junifer-0.0.4.dev90/docs/conf.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/docs/contribution.rst` & `junifer-0.0.4.dev90/docs/contribution.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/docs/extending/coordinates.rst` & `junifer-0.0.4.dev90/docs/extending/coordinates.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/docs/extending/datagrabber.rst` & `junifer-0.0.4.dev90/docs/extending/datagrabber.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/docs/extending/extension.rst` & `junifer-0.0.4.dev90/docs/extending/extension.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/docs/extending/index.rst` & `junifer-0.0.4.dev90/docs/extending/index.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/docs/extending/marker.rst` & `junifer-0.0.4.dev90/docs/extending/marker.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/docs/extending/masks.rst` & `junifer-0.0.4.dev90/docs/extending/masks.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/docs/extending/parcellations.rst` & `junifer-0.0.4.dev90/docs/extending/parcellations.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/docs/faq.rst` & `junifer-0.0.4.dev90/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/docs/help.rst` & `junifer-0.0.4.dev90/docs/help.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/docs/images/junifer_logo.png` & `junifer-0.0.4.dev90/docs/images/junifer_logo.png`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/docs/index.rst` & `junifer-0.0.4.dev90/docs/index.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/docs/installation.rst` & `junifer-0.0.4.dev90/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/docs/links.inc` & `junifer-0.0.4.dev90/docs/links.inc`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/docs/maintaining.rst` & `junifer-0.0.4.dev90/docs/maintaining.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/docs/sphinxext/gh_substitutions.py` & `junifer-0.0.4.dev90/docs/sphinxext/gh_substitutions.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/docs/starting.rst` & `junifer-0.0.4.dev90/docs/starting.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/docs/understanding/data.rst` & `junifer-0.0.4.dev90/docs/understanding/data.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/docs/understanding/datagrabber.rst` & `junifer-0.0.4.dev90/docs/understanding/datagrabber.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/docs/understanding/datareader.rst` & `junifer-0.0.4.dev90/docs/understanding/datareader.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/docs/understanding/index.rst` & `junifer-0.0.4.dev90/docs/understanding/index.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/docs/understanding/marker.rst` & `junifer-0.0.4.dev90/docs/understanding/marker.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/docs/understanding/pipeline.rst` & `junifer-0.0.4.dev90/docs/understanding/pipeline.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/docs/understanding/preprocess.rst` & `junifer-0.0.4.dev90/docs/understanding/preprocess.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/docs/understanding/storage.rst` & `junifer-0.0.4.dev90/docs/understanding/storage.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/docs/using/codeless.rst` & `junifer-0.0.4.dev90/docs/using/codeless.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/docs/using/index.rst` & `junifer-0.0.4.dev90/docs/using/index.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/docs/using/masks.rst` & `junifer-0.0.4.dev90/docs/using/masks.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/docs/using/queueing.rst` & `junifer-0.0.4.dev90/docs/using/queueing.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/docs/using/running.rst` & `junifer-0.0.4.dev90/docs/using/running.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/docs/whats_new.rst` & `junifer-0.0.4.dev90/docs/whats_new.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/examples/norun_hcpfc_pearson.py` & `junifer-0.0.4.dev90/examples/norun_hcpfc_pearson.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/examples/norun_ukbvm_gmd.py` & `junifer-0.0.4.dev90/examples/norun_ukbvm_gmd.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/examples/run_compute_parcel_mean.py` & `junifer-0.0.4.dev90/examples/run_compute_parcel_mean.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/examples/run_datagrabber_bids_datalad.py` & `junifer-0.0.4.dev90/examples/run_datagrabber_bids_datalad.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/examples/run_ets_rss_marker.py` & `junifer-0.0.4.dev90/examples/run_ets_rss_marker.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/examples/run_junifer_julearn.py` & `junifer-0.0.4.dev90/examples/run_junifer_julearn.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/examples/run_run_gmd_mean.py` & `junifer-0.0.4.dev90/examples/run_run_gmd_mean.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/examples/yamls/gmd_mean.yaml` & `junifer-0.0.4.dev90/examples/yamls/gmd_mean.yaml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/examples/yamls/ukb_gmd_mean.yaml` & `junifer-0.0.4.dev90/examples/yamls/ukb_gmd_mean.yaml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/api/cli.py` & `junifer-0.0.4.dev90/junifer/api/cli.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/api/decorators.py` & `junifer-0.0.4.dev90/junifer/api/decorators.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/api/functions.py` & `junifer-0.0.4.dev90/junifer/api/functions.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/api/parser.py` & `junifer-0.0.4.dev90/junifer/api/parser.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/api/res/afni/run_afni_docker.sh` & `junifer-0.0.4.dev90/junifer/api/res/afni/run_afni_docker.sh`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/api/tests/test_api_utils.py` & `junifer-0.0.4.dev90/junifer/api/tests/test_api_utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/api/tests/test_cli.py` & `junifer-0.0.4.dev90/junifer/api/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/api/tests/test_functions.py` & `junifer-0.0.4.dev90/junifer/api/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/api/tests/test_parser.py` & `junifer-0.0.4.dev90/junifer/api/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/api/utils.py` & `junifer-0.0.4.dev90/junifer/api/utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/configs/juseless/datagrabbers/aomic_id1000_vbm.py` & `junifer-0.0.4.dev90/junifer/configs/juseless/datagrabbers/aomic_id1000_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/configs/juseless/datagrabbers/camcan_vbm.py` & `junifer-0.0.4.dev90/junifer/configs/juseless/datagrabbers/camcan_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/configs/juseless/datagrabbers/ixi_vbm.py` & `junifer-0.0.4.dev90/junifer/configs/juseless/datagrabbers/ixi_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/configs/juseless/datagrabbers/tests/test_aomic_id1000_vbm.py` & `junifer-0.0.4.dev90/junifer/configs/juseless/datagrabbers/tests/test_aomic_id1000_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/configs/juseless/datagrabbers/tests/test_camcan_vbm.py` & `junifer-0.0.4.dev90/junifer/configs/juseless/datagrabbers/tests/test_camcan_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/configs/juseless/datagrabbers/tests/test_ixi_vbm.py` & `junifer-0.0.4.dev90/junifer/configs/juseless/datagrabbers/tests/test_ixi_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/configs/juseless/datagrabbers/tests/test_ucla.py` & `junifer-0.0.4.dev90/junifer/configs/juseless/datagrabbers/tests/test_ucla.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/configs/juseless/datagrabbers/tests/test_ukb_vbm.py` & `junifer-0.0.4.dev90/junifer/configs/juseless/datagrabbers/tests/test_ukb_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/configs/juseless/datagrabbers/ucla.py` & `junifer-0.0.4.dev90/junifer/configs/juseless/datagrabbers/ucla.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/configs/juseless/datagrabbers/ukb_vbm.py` & `junifer-0.0.4.dev90/junifer/configs/juseless/datagrabbers/ukb_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/data/VOIs/meta/Dosenbach2010_MNI_VOIs.txt` & `junifer-0.0.4.dev90/junifer/data/VOIs/meta/Dosenbach2010_MNI_VOIs.txt`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/data/VOIs/meta/Power2011_MNI_VOIs.txt` & `junifer-0.0.4.dev90/junifer/data/VOIs/meta/Power2011_MNI_VOIs.txt`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/data/VOIs/meta/Power2013_MNI_VOIs.tsv` & `junifer-0.0.4.dev90/junifer/data/VOIs/meta/Power2013_MNI_VOIs.tsv`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/data/VOIs/meta/Rew_VOIs.txt` & `junifer-0.0.4.dev90/junifer/data/VOIs/meta/Rew_VOIs.txt`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/data/VOIs/meta/WM_VOIs.txt` & `junifer-0.0.4.dev90/junifer/data/VOIs/meta/WM_VOIs.txt`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/data/coordinates.py` & `junifer-0.0.4.dev90/junifer/data/coordinates.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean.nii.gz` & `junifer-0.0.4.dev90/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean.nii.gz`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean_3mm.nii.gz` & `junifer-0.0.4.dev90/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean_3mm.nii.gz`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/data/masks/vickery-patil/GMprob0.2_cortex_3mm_NA_rm.nii.gz` & `junifer-0.0.4.dev90/junifer/data/masks/vickery-patil/GMprob0.2_cortex_3mm_NA_rm.nii.gz`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/data/masks.py` & `junifer-0.0.4.dev90/junifer/data/masks.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/data/parcellations.py` & `junifer-0.0.4.dev90/junifer/data/parcellations.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/data/tests/test_coordinates.py` & `junifer-0.0.4.dev90/junifer/data/tests/test_coordinates.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/data/tests/test_data_utils.py` & `junifer-0.0.4.dev90/junifer/data/tests/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/data/tests/test_masks.py` & `junifer-0.0.4.dev90/junifer/data/tests/test_masks.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/data/tests/test_parcellations.py` & `junifer-0.0.4.dev90/junifer/data/tests/test_parcellations.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/data/utils.py` & `junifer-0.0.4.dev90/junifer/data/utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/datagrabber/__init__.py` & `junifer-0.0.4.dev90/junifer/datagrabber/__init__.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/datagrabber/aomic/id1000.py` & `junifer-0.0.4.dev90/junifer/datagrabber/aomic/id1000.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/datagrabber/aomic/piop1.py` & `junifer-0.0.4.dev90/junifer/datagrabber/aomic/piop1.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/datagrabber/aomic/piop2.py` & `junifer-0.0.4.dev90/junifer/datagrabber/aomic/piop2.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/datagrabber/aomic/tests/test_id1000.py` & `junifer-0.0.4.dev90/junifer/datagrabber/aomic/tests/test_id1000.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/datagrabber/aomic/tests/test_piop1.py` & `junifer-0.0.4.dev90/junifer/datagrabber/aomic/tests/test_piop1.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/datagrabber/aomic/tests/test_piop2.py` & `junifer-0.0.4.dev90/junifer/datagrabber/aomic/tests/test_piop2.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/datagrabber/base.py` & `junifer-0.0.4.dev90/junifer/datagrabber/base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/datagrabber/datalad_base.py` & `junifer-0.0.4.dev90/junifer/datagrabber/datalad_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/datagrabber/hcp1200/datalad_hcp1200.py` & `junifer-0.0.4.dev90/junifer/datagrabber/hcp1200/datalad_hcp1200.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/datagrabber/hcp1200/hcp1200.py` & `junifer-0.0.4.dev90/junifer/datagrabber/hcp1200/hcp1200.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/datagrabber/hcp1200/tests/test_hcp1200.py` & `junifer-0.0.4.dev90/junifer/datagrabber/hcp1200/tests/test_hcp1200.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/datagrabber/multiple.py` & `junifer-0.0.4.dev90/junifer/datagrabber/multiple.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/datagrabber/pattern.py` & `junifer-0.0.4.dev90/junifer/datagrabber/pattern.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/datagrabber/pattern_datalad.py` & `junifer-0.0.4.dev90/junifer/datagrabber/pattern_datalad.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/datagrabber/tests/test_base.py` & `junifer-0.0.4.dev90/junifer/datagrabber/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/datagrabber/tests/test_datagrabber_utils.py` & `junifer-0.0.4.dev90/junifer/datagrabber/tests/test_datagrabber_utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/datagrabber/tests/test_datalad_base.py` & `junifer-0.0.4.dev90/junifer/datagrabber/tests/test_datalad_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/datagrabber/tests/test_multiple.py` & `junifer-0.0.4.dev90/junifer/datagrabber/tests/test_multiple.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/datagrabber/tests/test_pattern.py` & `junifer-0.0.4.dev90/junifer/datagrabber/tests/test_pattern.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/datagrabber/tests/test_pattern_datalad.py` & `junifer-0.0.4.dev90/junifer/datagrabber/tests/test_pattern_datalad.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/datagrabber/utils.py` & `junifer-0.0.4.dev90/junifer/datagrabber/utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/datareader/default.py` & `junifer-0.0.4.dev90/junifer/datareader/default.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/datareader/tests/test_default_reader.py` & `junifer-0.0.4.dev90/junifer/datareader/tests/test_default_reader.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/external/h5io/h5io/_h5io.py` & `junifer-0.0.4.dev90/junifer/external/h5io/h5io/_h5io.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/external/h5io/h5io/chunked_array.py` & `junifer-0.0.4.dev90/junifer/external/h5io/h5io/chunked_array.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/external/h5io/h5io/chunked_list.py` & `junifer-0.0.4.dev90/junifer/external/h5io/h5io/chunked_list.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/external/nilearn/junifer_nifti_spheres_masker.py` & `junifer-0.0.4.dev90/junifer/external/nilearn/junifer_nifti_spheres_masker.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/external/nilearn/tests/test_junifer_nifti_spheres_masker.py` & `junifer-0.0.4.dev90/junifer/external/nilearn/tests/test_junifer_nifti_spheres_masker.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/markers/__init__.py` & `junifer-0.0.4.dev90/junifer/markers/__init__.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/markers/base.py` & `junifer-0.0.4.dev90/junifer/markers/base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/markers/collection.py` & `junifer-0.0.4.dev90/junifer/markers/collection.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/markers/ets_rss.py` & `junifer-0.0.4.dev90/junifer/markers/ets_rss.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/markers/falff/falff_base.py` & `junifer-0.0.4.dev90/junifer/markers/falff/falff_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/markers/falff/falff_estimator.py` & `junifer-0.0.4.dev90/junifer/markers/falff/falff_estimator.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/markers/falff/falff_parcels.py` & `junifer-0.0.4.dev90/junifer/markers/falff/falff_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/markers/falff/falff_spheres.py` & `junifer-0.0.4.dev90/junifer/markers/falff/falff_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/markers/falff/tests/test_falff_estimator.py` & `junifer-0.0.4.dev90/junifer/markers/falff/tests/test_falff_estimator.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/markers/falff/tests/test_falff_parcels.py` & `junifer-0.0.4.dev90/junifer/markers/falff/tests/test_falff_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/markers/falff/tests/test_falff_spheres.py` & `junifer-0.0.4.dev90/junifer/markers/falff/tests/test_falff_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/markers/functional_connectivity/crossparcellation_functional_connectivity.py` & `junifer-0.0.4.dev90/junifer/markers/functional_connectivity/crossparcellation_functional_connectivity.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/markers/functional_connectivity/edge_functional_connectivity_parcels.py` & `junifer-0.0.4.dev90/junifer/markers/functional_connectivity/edge_functional_connectivity_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/markers/functional_connectivity/edge_functional_connectivity_spheres.py` & `junifer-0.0.4.dev90/junifer/markers/functional_connectivity/edge_functional_connectivity_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/markers/functional_connectivity/functional_connectivity_base.py` & `junifer-0.0.4.dev90/junifer/markers/functional_connectivity/functional_connectivity_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/markers/functional_connectivity/functional_connectivity_parcels.py` & `junifer-0.0.4.dev90/junifer/markers/functional_connectivity/functional_connectivity_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/markers/functional_connectivity/functional_connectivity_spheres.py` & `junifer-0.0.4.dev90/junifer/markers/functional_connectivity/functional_connectivity_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/markers/functional_connectivity/tests/test_crossparcellation_functional_connectivity.py` & `junifer-0.0.4.dev90/junifer/markers/functional_connectivity/tests/test_crossparcellation_functional_connectivity.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_parcels.py` & `junifer-0.0.4.dev90/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_spheres.py` & `junifer-0.0.4.dev90/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/markers/functional_connectivity/tests/test_functional_connectivity_base.py` & `junifer-0.0.4.dev90/junifer/markers/functional_connectivity/tests/test_functional_connectivity_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/markers/functional_connectivity/tests/test_functional_connectivity_parcels.py` & `junifer-0.0.4.dev90/junifer/markers/functional_connectivity/tests/test_functional_connectivity_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/markers/functional_connectivity/tests/test_functional_connectivity_spheres.py` & `junifer-0.0.4.dev90/junifer/markers/functional_connectivity/tests/test_functional_connectivity_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/markers/parcel_aggregation.py` & `junifer-0.0.4.dev90/junifer/markers/parcel_aggregation.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/markers/reho/reho_base.py` & `junifer-0.0.4.dev90/junifer/markers/reho/reho_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/markers/reho/reho_estimator.py` & `junifer-0.0.4.dev90/junifer/markers/reho/reho_estimator.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/markers/reho/reho_parcels.py` & `junifer-0.0.4.dev90/junifer/markers/reho/reho_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/markers/reho/reho_spheres.py` & `junifer-0.0.4.dev90/junifer/markers/reho/reho_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/markers/reho/tests/test_reho_estimator.py` & `junifer-0.0.4.dev90/junifer/markers/reho/tests/test_reho_estimator.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/markers/reho/tests/test_reho_parcels.py` & `junifer-0.0.4.dev90/junifer/markers/reho/tests/test_reho_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/markers/reho/tests/test_reho_spheres.py` & `junifer-0.0.4.dev90/junifer/markers/reho/tests/test_reho_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/markers/sphere_aggregation.py` & `junifer-0.0.4.dev90/junifer/markers/sphere_aggregation.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/markers/temporal_snr/temporal_snr_base.py` & `junifer-0.0.4.dev90/junifer/markers/temporal_snr/temporal_snr_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/markers/temporal_snr/temporal_snr_parcels.py` & `junifer-0.0.4.dev90/junifer/markers/temporal_snr/temporal_snr_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/markers/temporal_snr/temporal_snr_spheres.py` & `junifer-0.0.4.dev90/junifer/markers/temporal_snr/temporal_snr_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/markers/temporal_snr/tests/test_temporal_snr_parcels.py` & `junifer-0.0.4.dev90/junifer/markers/temporal_snr/tests/test_temporal_snr_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/markers/temporal_snr/tests/test_temporal_snr_spheres.py` & `junifer-0.0.4.dev90/junifer/markers/temporal_snr/tests/test_temporal_snr_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/markers/tests/test_collection.py` & `junifer-0.0.4.dev90/junifer/markers/tests/test_collection.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/markers/tests/test_ets_rss.py` & `junifer-0.0.4.dev90/junifer/markers/tests/test_ets_rss.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/markers/tests/test_marker_utils.py` & `junifer-0.0.4.dev90/junifer/markers/tests/test_marker_utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/markers/tests/test_markers_base.py` & `junifer-0.0.4.dev90/junifer/markers/tests/test_markers_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/markers/tests/test_parcel_aggregation.py` & `junifer-0.0.4.dev90/junifer/markers/tests/test_parcel_aggregation.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/markers/tests/test_sphere_aggregation.py` & `junifer-0.0.4.dev90/junifer/markers/tests/test_sphere_aggregation.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/markers/utils.py` & `junifer-0.0.4.dev90/junifer/markers/utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/onthefly/read_transform.py` & `junifer-0.0.4.dev90/junifer/onthefly/read_transform.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/onthefly/tests/test_read_transform.py` & `junifer-0.0.4.dev90/junifer/onthefly/tests/test_read_transform.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/pipeline/pipeline_step_mixin.py` & `junifer-0.0.4.dev90/junifer/pipeline/pipeline_step_mixin.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/pipeline/registry.py` & `junifer-0.0.4.dev90/junifer/pipeline/registry.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/pipeline/singleton.py` & `junifer-0.0.4.dev90/junifer/pipeline/singleton.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/pipeline/tests/test_pipeline_step_mixin.py` & `junifer-0.0.4.dev90/junifer/pipeline/tests/test_pipeline_step_mixin.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/pipeline/tests/test_registry.py` & `junifer-0.0.4.dev90/junifer/pipeline/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/pipeline/tests/test_update_meta_mixin.py` & `junifer-0.0.4.dev90/junifer/pipeline/tests/test_update_meta_mixin.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/pipeline/tests/test_workdir_manager.py` & `junifer-0.0.4.dev90/junifer/pipeline/tests/test_workdir_manager.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/pipeline/update_meta_mixin.py` & `junifer-0.0.4.dev90/junifer/pipeline/update_meta_mixin.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/pipeline/utils.py` & `junifer-0.0.4.dev90/junifer/pipeline/utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/pipeline/workdir_manager.py` & `junifer-0.0.4.dev90/junifer/pipeline/workdir_manager.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/preprocess/base.py` & `junifer-0.0.4.dev90/junifer/preprocess/base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/preprocess/confounds/fmriprep_confound_remover.py` & `junifer-0.0.4.dev90/junifer/preprocess/confounds/fmriprep_confound_remover.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/preprocess/confounds/tests/test_fmriprep_confound_remover.py` & `junifer-0.0.4.dev90/junifer/preprocess/confounds/tests/test_fmriprep_confound_remover.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/preprocess/tests/test_preprocess_base.py` & `junifer-0.0.4.dev90/junifer/preprocess/tests/test_preprocess_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/stats.py` & `junifer-0.0.4.dev90/junifer/stats.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/storage/base.py` & `junifer-0.0.4.dev90/junifer/storage/base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/storage/hdf5.py` & `junifer-0.0.4.dev90/junifer/storage/hdf5.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/storage/pandas_base.py` & `junifer-0.0.4.dev90/junifer/storage/pandas_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/storage/sqlite.py` & `junifer-0.0.4.dev90/junifer/storage/sqlite.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/storage/tests/test_hdf5.py` & `junifer-0.0.4.dev90/junifer/storage/tests/test_hdf5.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/storage/tests/test_pandas_base.py` & `junifer-0.0.4.dev90/junifer/storage/tests/test_pandas_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/storage/tests/test_sqlite.py` & `junifer-0.0.4.dev90/junifer/storage/tests/test_sqlite.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/storage/tests/test_storage_base.py` & `junifer-0.0.4.dev90/junifer/storage/tests/test_storage_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/storage/tests/test_utils.py` & `junifer-0.0.4.dev90/junifer/storage/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/storage/utils.py` & `junifer-0.0.4.dev90/junifer/storage/utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/testing/data/sub-0001_task-anticipation_acq-seq_desc-confounds_regressors.tsv` & `junifer-0.0.4.dev90/junifer/testing/data/sub-0001_task-anticipation_acq-seq_desc-confounds_regressors.tsv`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/testing/datagrabbers.py` & `junifer-0.0.4.dev90/junifer/testing/datagrabbers.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/testing/registry.py` & `junifer-0.0.4.dev90/junifer/testing/registry.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/testing/tests/test_oasisvmbtesting_datagrabber.py` & `junifer-0.0.4.dev90/junifer/testing/tests/test_oasisvmbtesting_datagrabber.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/testing/tests/test_partlycloudytesting_datagrabber.py` & `junifer-0.0.4.dev90/junifer/testing/tests/test_partlycloudytesting_datagrabber.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/testing/tests/test_spmauditory_datagrabber.py` & `junifer-0.0.4.dev90/junifer/testing/tests/test_spmauditory_datagrabber.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/testing/tests/test_testing_registry.py` & `junifer-0.0.4.dev90/junifer/testing/tests/test_testing_registry.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/testing/utils.py` & `junifer-0.0.4.dev90/junifer/testing/utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/tests/test_stats.py` & `junifer-0.0.4.dev90/junifer/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/utils/logging.py` & `junifer-0.0.4.dev90/junifer/utils/logging.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/utils/tests/test_fs.py` & `junifer-0.0.4.dev90/junifer/utils/tests/test_fs.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer/utils/tests/test_logging.py` & `junifer-0.0.4.dev90/junifer/utils/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/junifer.egg-info/PKG-INFO` & `junifer-0.0.4.dev90/junifer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: junifer
-Version: 0.0.4.dev85
+Version: 0.0.4.dev90
 Summary: JUelich NeuroImaging FEature extractoR
 Author-email: Fede Raimondo <f.raimondo@fz-juelich.de>, Synchon Mandal <s.mandal@fz-juelich.de>
 Maintainer-email: Fede Raimondo <f.raimondo@fz-juelich.de>, Synchon Mandal <s.mandal@fz-juelich.de>
 License: AGPL-3.0-only
 Project-URL: homepage, https://juaml.github.io/junifer
 Project-URL: documentation, https://juaml.github.io/junifer
 Project-URL: repository, https://github.com/juaml/junifer
```

### Comparing `junifer-0.0.4.dev85/junifer.egg-info/SOURCES.txt` & `junifer-0.0.4.dev90/junifer.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -63,14 +63,15 @@
 docs/changes/newsfragments/247.doc
 docs/changes/newsfragments/248.change
 docs/changes/newsfragments/251.doc
 docs/changes/newsfragments/253.misc
 docs/changes/newsfragments/254.feature
 docs/changes/newsfragments/258.enh
 docs/changes/newsfragments/259.enh
+docs/changes/newsfragments/261.misc
 docs/extending/coordinates.rst
 docs/extending/datagrabber.rst
 docs/extending/extension.rst
 docs/extending/index.rst
 docs/extending/marker.rst
 docs/extending/masks.rst
 docs/extending/parcellations.rst
```

### Comparing `junifer-0.0.4.dev85/junifer.egg-info/requires.txt` & `junifer-0.0.4.dev90/junifer.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/pyproject.toml` & `junifer-0.0.4.dev90/pyproject.toml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/tools/create_aomic1000_example_dataset.py` & `junifer-0.0.4.dev90/tools/create_aomic1000_example_dataset.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/tools/create_aomicpiop1_example_dataset.py` & `junifer-0.0.4.dev90/tools/create_aomicpiop1_example_dataset.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/tools/create_aomicpiop2_example_dataset.py` & `junifer-0.0.4.dev90/tools/create_aomicpiop2_example_dataset.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/tools/create_bids_example_dataset.py` & `junifer-0.0.4.dev90/tools/create_bids_example_dataset.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/tools/create_bids_example_dataset_sessions.py` & `junifer-0.0.4.dev90/tools/create_bids_example_dataset_sessions.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/tools/create_hcp1200_example_dataset.py` & `junifer-0.0.4.dev90/tools/create_hcp1200_example_dataset.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev85/tox.ini` & `junifer-0.0.4.dev90/tox.ini`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     pytest
 commands =
     pytest
 
 [testenv:ruff]
 skip_install = true
 deps =
-    ruff
+    ruff>=0.1.0
 commands =
     ruff check {toxinidir}
 
 [testenv:black]
 skip_install = true
 deps =
     black
```

