# Comparing `tmp/message-ix-models-2024.1.29rc1.tar.gz` & `tmp/message-ix-models-2024.4.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "message-ix-models-2024.1.29rc1.tar", last modified: Mon Jan 29 16:27:55 2024, max compression
+gzip compressed data, was "message-ix-models-2024.4.2rc1.tar", last modified: Tue Apr  2 06:09:45 2024, max compression
```

## Comparing `message-ix-models-2024.1.29rc1.tar` & `message-ix-models-2024.4.2rc1.tar`

### file list

```diff
@@ -1,283 +1,284 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:27:55.153145 message-ix-models-2024.1.29rc1/
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:27:55.109144 message-ix-models-2024.1.29rc1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/.github/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:27:55.109144 message-ix-models-2024.1.29rc1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/.github/workflows/pytest.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-01-29 16:27:55.153145 message-ix-models-2024.1.29rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:27:55.113144 message-ix-models-2024.1.29rc1/doc/
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:27:55.117144 message-ix-models-2024.1.29rc1/doc/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    56233 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/doc/_static/combined-logo-white.png
--rw-r--r--   0 runner    (1001) docker     (127)    49140 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/doc/_static/combined-logo-white.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/doc/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)     6608 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/doc/_static/favicon.svg
--rw-r--r--   0 runner    (1001) docker     (127)    22635 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/doc/_static/logo-white.png
--rw-r--r--   0 runner    (1001) docker     (127)    13459 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/doc/_static/message-ix-models-logo-white.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:27:55.117144 message-ix-models-2024.1.29rc1/doc/_template/
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/doc/_template/autosummary-class.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/doc/_template/autosummary-module.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:27:55.117144 message-ix-models-2024.1.29rc1/doc/api/
--rw-r--r--   0 runner    (1001) docker     (127)     6193 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/doc/api/data-sources.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5822 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/doc/api/disutility.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/doc/api/model-bare.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/doc/api/model-build.rst
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/doc/api/model-emissions.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/doc/api/model-snapshot.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/doc/api/model.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/doc/api/project.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:27:55.117144 message-ix-models-2024.1.29rc1/doc/api/report/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/doc/api/report/default-config.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9424 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/doc/api/report/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/doc/api/testing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/doc/api/tools.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5084 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/doc/api/util.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6399 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/doc/api/workflow.rst
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/doc/bibliography.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7947 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/doc/cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6007 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    11025 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/doc/data.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/doc/develop.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/doc/distrib.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/doc/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/doc/main.bib
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/doc/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)    13639 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/doc/migrate.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:27:55.121144 message-ix-models-2024.1.29rc1/doc/pkg-data/
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/doc/pkg-data/codelists.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/doc/pkg-data/iiasa-se.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/doc/pkg-data/node.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/doc/pkg-data/relation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/doc/pkg-data/year.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/doc/releasing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/doc/repro.rst
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/doc/requirements.in
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/doc/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:27:55.121144 message-ix-models-2024.1.29rc1/doc/water/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/doc/water/files.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7291 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/doc/water/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)    15404 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/doc/whatsnew.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:27:55.121144 message-ix-models-2024.1.29rc1/message_ix_models/
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/message_ix_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/message_ix_models/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:27:55.121144 message-ix-models-2024.1.29rc1/message_ix_models/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:27:55.121144 message-ix-models-2024.1.29rc1/message_ix_models/data/cd_links/
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/message_ix_models/data/cd_links/unit.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     7446 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/message_ix_models/data/commodity.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:27:55.121144 message-ix-models-2024.1.29rc1/message_ix_models/data/edits/
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/message_ix_models/data/edits/messageix-transport-core.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4763 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/message_ix_models/data/edits/messageix-transport-input.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:27:55.121144 message-ix-models-2024.1.29rc1/message_ix_models/data/iiasa-se/
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/message_ix_models/data/iiasa-se/def-regions.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/message_ix_models/data/iiasa-se/mappings-R12.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:27:55.121144 message-ix-models-2024.1.29rc1/message_ix_models/data/ipcc/
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/message_ix_models/data/ipcc/1996_v3_t1-2.csv
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/message_ix_models/data/level.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:27:55.125144 message-ix-models-2024.1.29rc1/message_ix_models/data/node/
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/message_ix_models/data/node/ADVANCE.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    18288 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/message_ix_models/data/node/B210-R11.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/message_ix_models/data/node/ISR.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/message_ix_models/data/node/R11.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/message_ix_models/data/node/R12.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/message_ix_models/data/node/R14.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/message_ix_models/data/node/R17.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/message_ix_models/data/node/R20.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5440 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/message_ix_models/data/node/R32.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/message_ix_models/data/node/RCP.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/message_ix_models/data/node/ZMB.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:27:55.125144 message-ix-models-2024.1.29rc1/message_ix_models/data/relation/
--rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/message_ix_models/data/relation/A.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6717 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/message_ix_models/data/relation/B.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    55164 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/message_ix_models/data/relation/CD-LINKS.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:27:55.125144 message-ix-models-2024.1.29rc1/message_ix_models/data/report/
--rw-r--r--   0 runner    (1001) docker     (127)    33450 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/message_ix_models/data/report/global.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:27:55.129145 message-ix-models-2024.1.29rc1/message_ix_models/data/sdmx/
--rw-r--r--   0 runner    (1001) docker     (127)  1026939 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/message_ix_models/data/sdmx/ADVANCE.xml
--rw-r--r--   0 runner    (1001) docker     (127)     8515 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/message_ix_models/data/sdmx/ICONICS_SSP(2017).xml
--rw-r--r--   0 runner    (1001) docker     (127)     8522 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/message_ix_models/data/sdmx/ICONICS_SSP(2024).xml
--rw-r--r--   0 runner    (1001) docker     (127)     7459 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/message_ix_models/data/sdmx/IEA_COUNTRY_IEA(2023).xml
--rw-r--r--   0 runner    (1001) docker     (127)     6857 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/message_ix_models/data/sdmx/IEA_COUNTRY_OECD(2021).xml
--rw-r--r--   0 runner    (1001) docker     (127)     6655 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/message_ix_models/data/sdmx/IEA_COUNTRY_OECD(2022).xml
--rw-r--r--   0 runner    (1001) docker     (127)     6835 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/message_ix_models/data/sdmx/IEA_COUNTRY_OECD(2023).xml
--rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/message_ix_models/data/sdmx/IEA_FLOW_IEA(2023).xml
--rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/message_ix_models/data/sdmx/IEA_FLOW_OECD(2021).xml
--rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/message_ix_models/data/sdmx/IEA_FLOW_OECD(2022).xml
--rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/message_ix_models/data/sdmx/IEA_FLOW_OECD(2023).xml
--rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/message_ix_models/data/sdmx/IEA_PRODUCT_IEA(2023).xml
--rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/message_ix_models/data/sdmx/IEA_PRODUCT_OECD(2021).xml
--rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/message_ix_models/data/sdmx/IEA_PRODUCT_OECD(2022).xml
--rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/message_ix_models/data/sdmx/IEA_PRODUCT_OECD(2023).xml
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/message_ix_models/data/sdmx/IIASA_ECE_AGENCIES(0.1).xml
--rw-r--r--   0 runner    (1001) docker     (127)    72081 2024-01-29 16:26:22.000000 message-ix-models-2024.1.29rc1/message_ix_models/data/technology.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:27:55.105144 message-ix-models-2024.1.29rc1/message_ix_models/data/test/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:27:55.129145 message-ix-models-2024.1.29rc1/message_ix_models/data/test/macro/
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/data/test/macro/kgdp.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:27:55.129145 message-ix-models-2024.1.29rc1/message_ix_models/data/unit/
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/data/unit/snapshot.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/data/unit.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:27:55.129145 message-ix-models-2024.1.29rc1/message_ix_models/data/water/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/data/water/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/data/water/config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    28513 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/data/water/set.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    42152 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/data/water/technology.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:27:55.129145 message-ix-models-2024.1.29rc1/message_ix_models/data/year/
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/data/year/A.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/data/year/B.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:27:55.133144 message-ix-models-2024.1.29rc1/message_ix_models/model/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4803 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/model/bare.py
--rw-r--r--   0 runner    (1001) docker     (127)     5930 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/model/build.py
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/model/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/model/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/model/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     7336 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/model/disutility.py
--rw-r--r--   0 runner    (1001) docker     (127)     5868 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/model/emissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/model/macro.py
--rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/model/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (127)    10942 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/model/structure.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:27:55.133144 message-ix-models-2024.1.29rc1/message_ix_models/model/water/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/model/water/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8335 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/model/water/build.py
--rw-r--r--   0 runner    (1001) docker     (127)     8699 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/model/water/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:27:55.133144 message-ix-models-2024.1.29rc1/message_ix_models/model/water/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/model/water/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32234 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/model/water/data/demands.py
--rw-r--r--   0 runner    (1001) docker     (127)    28442 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/model/water/data/infrastructure.py
--rw-r--r--   0 runner    (1001) docker     (127)     6234 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/model/water/data/irrigation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:27:55.137145 message-ix-models-2024.1.29rc1/message_ix_models/model/water/data/pre_processing/
--rw-r--r--   0 runner    (1001) docker     (127)    12653 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/model/water/data/pre_processing/calculate_ppl_cooling_technology_shares.r
--rw-r--r--   0 runner    (1001) docker     (127)    38780 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/model/water/data/pre_processing/desalination.R
--rw-r--r--   0 runner    (1001) docker     (127)    38900 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/model/water/data/pre_processing/generate_water_constraints.R
--rw-r--r--   0 runner    (1001) docker     (127)    14302 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/model/water/data/pre_processing/generate_water_constraints_monthly.r
--rw-r--r--   0 runner    (1001) docker     (127)    12058 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/model/water/data/pre_processing/groundwater_harmonize.r
--rw-r--r--   0 runner    (1001) docker     (127)    11332 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/model/water/data/pre_processing/hydro_agg_basin.py
--rw-r--r--   0 runner    (1001) docker     (127)    10839 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/model/water/data/pre_processing/hydro_agg_raster.py
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/model/water/data/pre_processing/hydro_agg_spatial.R
--rw-r--r--   0 runner    (1001) docker     (127)    29422 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/model/water/data/water_for_ppl.py
--rw-r--r--   0 runner    (1001) docker     (127)    27720 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/model/water/data/water_supply.py
--rw-r--r--   0 runner    (1001) docker     (127)    51721 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/model/water/reporting.py
--rw-r--r--   0 runner    (1001) docker     (127)     4560 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/model/water/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:27:55.137145 message-ix-models-2024.1.29rc1/message_ix_models/project/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/project/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:27:55.137145 message-ix-models-2024.1.29rc1/message_ix_models/project/advance/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/project/advance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4753 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/project/advance/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:27:55.137145 message-ix-models-2024.1.29rc1/message_ix_models/project/gea/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/project/gea/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:27:55.137145 message-ix-models-2024.1.29rc1/message_ix_models/project/shape/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/project/shape/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:27:55.137145 message-ix-models-2024.1.29rc1/message_ix_models/project/ssp/
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/project/ssp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5013 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/project/ssp/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     8227 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/project/ssp/structure.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:27:55.141145 message-ix-models-2024.1.29rc1/message_ix_models/report/
--rw-r--r--   0 runner    (1001) docker     (127)    14170 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/report/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    14571 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/report/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/report/computations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/report/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7792 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/report/operator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6842 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/report/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     7550 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/report/sim.py
--rw-r--r--   0 runner    (1001) docker     (127)     7228 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/report/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:27:55.141145 message-ix-models-2024.1.29rc1/message_ix_models/testing/
--rw-r--r--   0 runner    (1001) docker     (127)    13514 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/testing/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:27:55.141145 message-ix-models-2024.1.29rc1/message_ix_models/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:27:55.141145 message-ix-models-2024.1.29rc1/message_ix_models/tests/model/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/tests/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/tests/model/test_bare.py
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/tests/model/test_build.py
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/tests/model/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/tests/model/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8858 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/tests/model/test_disutility.py
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/tests/model/test_emissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/tests/model/test_macro.py
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/tests/model/test_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (127)     8650 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/tests/model/test_structure.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:27:55.145145 message-ix-models-2024.1.29rc1/message_ix_models/tests/project/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/tests/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/tests/project/test_advance.py
--rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/tests/project/test_ssp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:27:55.145145 message-ix-models-2024.1.29rc1/message_ix_models/tests/report/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/tests/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/tests/report/test_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/tests/report/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/tests/report/test_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     9991 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/tests/test_report.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/tests/test_testing.py
--rw-r--r--   0 runner    (1001) docker     (127)    12795 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     6073 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/tests/test_workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:27:55.145145 message-ix-models-2024.1.29rc1/message_ix_models/tests/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/tests/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:27:55.145145 message-ix-models-2024.1.29rc1/message_ix_models/tests/tools/iea/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/tests/tools/iea/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3957 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/tests/tools/iea/test_web.py
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/tests/tools/test_advance.py
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/tests/tools/test_exo_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/tests/tools/test_iamc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/tests/tools/test_wb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:27:55.145145 message-ix-models-2024.1.29rc1/message_ix_models/tests/util/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/tests/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/tests/util/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/tests/util/test_click.py
--rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/tests/util/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8433 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/tests/util/test_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/tests/util/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/tests/util/test_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     8190 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/tests/util/test_scenarioinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/tests/util/test_sdmx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:27:55.149145 message-ix-models-2024.1.29rc1/message_ix_models/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/tools/advance.py
--rw-r--r--   0 runner    (1001) docker     (127)    12626 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/tools/exo_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/tools/iamc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:27:55.149145 message-ix-models-2024.1.29rc1/message_ix_models/tools/iea/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/tools/iea/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8999 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/tools/iea/web.py
--rw-r--r--   0 runner    (1001) docker     (127)    11320 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/tools/wb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:27:55.149145 message-ix-models-2024.1.29rc1/message_ix_models/util/
--rw-r--r--   0 runner    (1001) docker     (127)    23949 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/util/_convert_units.py
--rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/util/_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/util/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     7884 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/util/click.py
--rw-r--r--   0 runner    (1001) docker     (127)     8039 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/util/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     6918 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/util/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    13067 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/util/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/util/importlib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/util/ixmp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/util/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     4511 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/util/pooch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/util/pycountry.py
--rw-r--r--   0 runner    (1001) docker     (127)    13614 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/util/scenarioinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     6111 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/util/sdmx.py
--rw-r--r--   0 runner    (1001) docker     (127)    13198 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/message_ix_models/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:27:55.153145 message-ix-models-2024.1.29rc1/message_ix_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-01-29 16:27:54.000000 message-ix-models-2024.1.29rc1/message_ix_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8577 2024-01-29 16:27:55.000000 message-ix-models-2024.1.29rc1/message_ix_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-29 16:27:54.000000 message-ix-models-2024.1.29rc1/message_ix_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-01-29 16:27:54.000000 message-ix-models-2024.1.29rc1/message_ix_models.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-01-29 16:27:54.000000 message-ix-models-2024.1.29rc1/message_ix_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-01-29 16:27:54.000000 message-ix-models-2024.1.29rc1/message_ix_models.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-29 16:27:55.153145 message-ix-models-2024.1.29rc1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:27:55.153145 message-ix-models-2024.1.29rc1/util/
--rwxr-xr-x   0 runner    (1001) docker     (127)      621 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/util/1-prep.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     3730 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/util/2-migrate.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)       66 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/util/reset.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      740 2024-01-29 16:26:25.000000 message-ix-models-2024.1.29rc1/util/settings.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:09:45.768439 message-ix-models-2024.4.2rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:09:45.732439 message-ix-models-2024.4.2rc1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/.github/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:09:45.732439 message-ix-models-2024.4.2rc1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5029 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-04-02 06:09:45.768439 message-ix-models-2024.4.2rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:09:45.736439 message-ix-models-2024.4.2rc1/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:09:45.736439 message-ix-models-2024.4.2rc1/doc/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    56233 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/doc/_static/combined-logo-white.png
+-rw-r--r--   0 runner    (1001) docker     (127)    49140 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/doc/_static/combined-logo-white.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/doc/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     6608 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/doc/_static/favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    22635 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/doc/_static/logo-white.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13459 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/doc/_static/message-ix-models-logo-white.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:09:45.736439 message-ix-models-2024.4.2rc1/doc/_template/
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/doc/_template/autosummary-class.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/doc/_template/autosummary-module.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:09:45.736439 message-ix-models-2024.4.2rc1/doc/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     6193 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/doc/api/data-sources.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5822 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/doc/api/disutility.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/doc/api/model-bare.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/doc/api/model-build.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/doc/api/model-emissions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/doc/api/model-snapshot.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/doc/api/model.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/doc/api/project.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:09:45.736439 message-ix-models-2024.4.2rc1/doc/api/report/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/doc/api/report/default-config.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9424 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/doc/api/report/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/doc/api/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/doc/api/tools.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/doc/api/util.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6399 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/doc/api/workflow.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/doc/bibliography.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9207 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/doc/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6084 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11025 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/doc/data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/doc/develop.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/doc/distrib.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/doc/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/doc/main.bib
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/doc/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)    13639 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/doc/migrate.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:09:45.740439 message-ix-models-2024.4.2rc1/doc/pkg-data/
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/doc/pkg-data/codelists.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/doc/pkg-data/iiasa-se.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/doc/pkg-data/node.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/doc/pkg-data/relation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/doc/pkg-data/year.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/doc/releasing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/doc/repro.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/doc/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/doc/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:09:45.740439 message-ix-models-2024.4.2rc1/doc/water/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/doc/water/files.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7291 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/doc/water/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    17159 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/doc/whatsnew.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:09:45.740439 message-ix-models-2024.4.2rc1/message_ix_models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/message_ix_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/message_ix_models/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:09:45.740439 message-ix-models-2024.4.2rc1/message_ix_models/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:09:45.740439 message-ix-models-2024.4.2rc1/message_ix_models/data/cd_links/
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/message_ix_models/data/cd_links/unit.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     7506 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/message_ix_models/data/commodity.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:09:45.740439 message-ix-models-2024.4.2rc1/message_ix_models/data/edits/
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/message_ix_models/data/edits/messageix-transport-core.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4763 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/message_ix_models/data/edits/messageix-transport-input.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:09:45.740439 message-ix-models-2024.4.2rc1/message_ix_models/data/iiasa-se/
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/message_ix_models/data/iiasa-se/def-regions.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/message_ix_models/data/iiasa-se/mappings-R12.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:09:45.740439 message-ix-models-2024.4.2rc1/message_ix_models/data/ipcc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/message_ix_models/data/ipcc/1996_v3_t1-2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/message_ix_models/data/level.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:09:45.744439 message-ix-models-2024.4.2rc1/message_ix_models/data/node/
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/message_ix_models/data/node/ADVANCE.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    18288 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/message_ix_models/data/node/B210-R11.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/message_ix_models/data/node/ISR.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/message_ix_models/data/node/R11.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/message_ix_models/data/node/R12.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/message_ix_models/data/node/R14.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/message_ix_models/data/node/R17.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/message_ix_models/data/node/R20.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5440 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/message_ix_models/data/node/R32.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/message_ix_models/data/node/RCP.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/message_ix_models/data/node/ZMB.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:09:45.744439 message-ix-models-2024.4.2rc1/message_ix_models/data/relation/
+-rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/message_ix_models/data/relation/A.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6717 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/message_ix_models/data/relation/B.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    55164 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/message_ix_models/data/relation/CD-LINKS.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:09:45.744439 message-ix-models-2024.4.2rc1/message_ix_models/data/report/
+-rw-r--r--   0 runner    (1001) docker     (127)    33450 2024-04-02 06:08:44.000000 message-ix-models-2024.4.2rc1/message_ix_models/data/report/global.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:09:45.748439 message-ix-models-2024.4.2rc1/message_ix_models/data/sdmx/
+-rw-r--r--   0 runner    (1001) docker     (127)  1026939 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/data/sdmx/ADVANCE.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     8515 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/data/sdmx/ICONICS_SSP(2017).xml
+-rw-r--r--   0 runner    (1001) docker     (127)     8522 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/data/sdmx/ICONICS_SSP(2024).xml
+-rw-r--r--   0 runner    (1001) docker     (127)     7459 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/data/sdmx/IEA_COUNTRY_IEA(2023).xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6857 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/data/sdmx/IEA_COUNTRY_OECD(2021).xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6655 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/data/sdmx/IEA_COUNTRY_OECD(2022).xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6835 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/data/sdmx/IEA_COUNTRY_OECD(2023).xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/data/sdmx/IEA_FLOW_IEA(2023).xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/data/sdmx/IEA_FLOW_OECD(2021).xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/data/sdmx/IEA_FLOW_OECD(2022).xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/data/sdmx/IEA_FLOW_OECD(2023).xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/data/sdmx/IEA_PRODUCT_IEA(2023).xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/data/sdmx/IEA_PRODUCT_OECD(2021).xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/data/sdmx/IEA_PRODUCT_OECD(2022).xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/data/sdmx/IEA_PRODUCT_OECD(2023).xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/data/sdmx/IIASA_ECE_AGENCIES(0.1).xml
+-rw-r--r--   0 runner    (1001) docker     (127)    72081 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/data/technology.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:09:45.728439 message-ix-models-2024.4.2rc1/message_ix_models/data/test/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:09:45.748439 message-ix-models-2024.4.2rc1/message_ix_models/data/test/macro/
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/data/test/macro/kgdp.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:09:45.748439 message-ix-models-2024.4.2rc1/message_ix_models/data/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/data/unit/snapshot.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/data/unit.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:09:45.748439 message-ix-models-2024.4.2rc1/message_ix_models/data/water/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/data/water/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/data/water/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    28513 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/data/water/set.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    42152 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/data/water/technology.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:09:45.748439 message-ix-models-2024.4.2rc1/message_ix_models/data/year/
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/data/year/A.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/data/year/B.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:09:45.752439 message-ix-models-2024.4.2rc1/message_ix_models/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/model/bare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5930 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/model/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/model/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/model/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/model/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7374 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/model/disutility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5868 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/model/emissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/model/macro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/model/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10947 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/model/structure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:09:45.752439 message-ix-models-2024.4.2rc1/message_ix_models/model/water/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/model/water/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8335 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/model/water/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8699 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/model/water/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:09:45.752439 message-ix-models-2024.4.2rc1/message_ix_models/model/water/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/model/water/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32234 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/model/water/data/demands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28441 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/model/water/data/infrastructure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6234 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/model/water/data/irrigation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:09:45.756439 message-ix-models-2024.4.2rc1/message_ix_models/model/water/data/pre_processing/
+-rw-r--r--   0 runner    (1001) docker     (127)    12653 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/model/water/data/pre_processing/calculate_ppl_cooling_technology_shares.r
+-rw-r--r--   0 runner    (1001) docker     (127)    38780 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/model/water/data/pre_processing/desalination.R
+-rw-r--r--   0 runner    (1001) docker     (127)    38900 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/model/water/data/pre_processing/generate_water_constraints.R
+-rw-r--r--   0 runner    (1001) docker     (127)    14302 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/model/water/data/pre_processing/generate_water_constraints_monthly.r
+-rw-r--r--   0 runner    (1001) docker     (127)    12058 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/model/water/data/pre_processing/groundwater_harmonize.r
+-rw-r--r--   0 runner    (1001) docker     (127)    11336 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/model/water/data/pre_processing/hydro_agg_basin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10840 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/model/water/data/pre_processing/hydro_agg_raster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/model/water/data/pre_processing/hydro_agg_spatial.R
+-rw-r--r--   0 runner    (1001) docker     (127)    29422 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/model/water/data/water_for_ppl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27720 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/model/water/data/water_supply.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51721 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/model/water/reporting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4560 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/model/water/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:09:45.756439 message-ix-models-2024.4.2rc1/message_ix_models/project/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/project/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:09:45.756439 message-ix-models-2024.4.2rc1/message_ix_models/project/advance/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/project/advance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4753 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/project/advance/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:09:45.756439 message-ix-models-2024.4.2rc1/message_ix_models/project/gea/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/project/gea/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:09:45.756439 message-ix-models-2024.4.2rc1/message_ix_models/project/shape/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/project/shape/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:09:45.756439 message-ix-models-2024.4.2rc1/message_ix_models/project/ssp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/project/ssp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6909 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/project/ssp/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8228 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/project/ssp/structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:09:45.756439 message-ix-models-2024.4.2rc1/message_ix_models/report/
+-rw-r--r--   0 runner    (1001) docker     (127)    14165 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/report/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14572 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/report/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/report/computations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/report/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7831 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/report/operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6741 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/report/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7551 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/report/sim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7242 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/report/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:09:45.756439 message-ix-models-2024.4.2rc1/message_ix_models/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)    11128 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/testing/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:09:45.760439 message-ix-models-2024.4.2rc1/message_ix_models/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:09:45.760439 message-ix-models-2024.4.2rc1/message_ix_models/tests/model/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/tests/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/tests/model/test_bare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/tests/model/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/tests/model/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/tests/model/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8859 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/tests/model/test_disutility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/tests/model/test_emissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/tests/model/test_macro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/tests/model/test_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8751 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/tests/model/test_structure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:09:45.760439 message-ix-models-2024.4.2rc1/message_ix_models/tests/project/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/tests/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/tests/project/test_advance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/tests/project/test_ssp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:09:45.760439 message-ix-models-2024.4.2rc1/message_ix_models/tests/report/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/tests/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/tests/report/test_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/tests/report/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/tests/report/test_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9992 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/tests/test_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/tests/test_testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12952 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6379 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/tests/test_workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:09:45.760439 message-ix-models-2024.4.2rc1/message_ix_models/tests/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/tests/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:09:45.760439 message-ix-models-2024.4.2rc1/message_ix_models/tests/tools/iea/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/tests/tools/iea/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/tests/tools/iea/test_web.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/tests/tools/test_advance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/tests/tools/test_exo_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/tests/tools/test_iamc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/tests/tools/test_wb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:09:45.764439 message-ix-models-2024.4.2rc1/message_ix_models/tests/util/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/tests/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/tests/util/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/tests/util/test_click.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/tests/util/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8554 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/tests/util/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/tests/util/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4559 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/tests/util/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8190 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/tests/util/test_scenarioinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/tests/util/test_sdmx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:09:45.764439 message-ix-models-2024.4.2rc1/message_ix_models/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/tools/advance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12960 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/tools/exo_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/tools/iamc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:09:45.764439 message-ix-models-2024.4.2rc1/message_ix_models/tools/iea/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/tools/iea/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9000 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/tools/iea/web.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11381 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/tools/wb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:09:45.768439 message-ix-models-2024.4.2rc1/message_ix_models/util/
+-rw-r--r--   0 runner    (1001) docker     (127)    24892 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/util/_convert_units.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9585 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/util/_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/util/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10776 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/util/click.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8347 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/util/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7265 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/util/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13164 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/util/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/util/importlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/util/ixmp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3672 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/util/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4512 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/util/pooch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/util/pycountry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13636 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/util/scenarioinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6393 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/util/sdmx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13323 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/message_ix_models/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:09:45.768439 message-ix-models-2024.4.2rc1/message_ix_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-04-02 06:09:45.000000 message-ix-models-2024.4.2rc1/message_ix_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8600 2024-04-02 06:09:45.000000 message-ix-models-2024.4.2rc1/message_ix_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 06:09:45.000000 message-ix-models-2024.4.2rc1/message_ix_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-02 06:09:45.000000 message-ix-models-2024.4.2rc1/message_ix_models.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-02 06:09:45.000000 message-ix-models-2024.4.2rc1/message_ix_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-02 06:09:45.000000 message-ix-models-2024.4.2rc1/message_ix_models.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3482 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 06:09:45.768439 message-ix-models-2024.4.2rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:09:45.768439 message-ix-models-2024.4.2rc1/util/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      621 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/util/1-prep.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3730 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/util/2-migrate.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)       66 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/util/reset.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      740 2024-04-02 06:08:45.000000 message-ix-models-2024.4.2rc1/util/settings.sh
```

### Comparing `message-ix-models-2024.1.29rc1/.github/pull_request_template.md` & `message-ix-models-2024.4.2rc1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/.gitignore` & `message-ix-models-2024.4.2rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/.pre-commit-config.yaml` & `message-ix-models-2024.4.2rc1/.pre-commit-config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -4,24 +4,24 @@
   - id: mypy
     name: mypy
     always_run: true
     require_serial: true
     pass_filenames: false
 
     language: python
-    entry: bash -c ". ${PRE_COMMIT_MYPY_VENV:-/dev/null}/bin/activate 2>/dev/null; mypy $0 $@"
+    entry: bash -c ". ${PRE_COMMIT_MYPY_VENV:-/dev/null}/bin/activate 2>/dev/null; mypy $0 $@; python -m pip list"
     additional_dependencies:
-    - mypy >= 1.8.0
+    - mypy >= 1.9.0
     - plotnine
     - pytest
     - sdmx1
     - types-PyYAML
     - types-tqdm
     - "ixmp @ git+https://github.com/iiasa/ixmp.git@main"
     - "message-ix @ git+https://github.com/iiasa/message_ix.git@main"
     args: ["."]
 - repo: https://github.com/astral-sh/ruff-pre-commit
-  rev: v0.1.13
+  rev: v0.3.2
   hooks:
   - id: ruff
   - id: ruff-format
     args: [ --check ]
```

### Comparing `message-ix-models-2024.1.29rc1/.readthedocs.yaml` & `message-ix-models-2024.4.2rc1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/LICENSE` & `message-ix-models-2024.4.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/PKG-INFO` & `message-ix-models-2024.4.2rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: message-ix-models
-Version: 2024.1.29rc1
+Version: 2024.4.2rc1
 Summary: Tools for the MESSAGEix-GLOBIOM family of models
 Author: IIASA Energy, Climate, and Environment (ECE) Program
 Maintainer-email: Paul Natsuo Kishimoto <mail@paul.kishimoto.name>, Fridolin Glatter <glatter@iiasa.ac.at>
 Project-URL: homepage, https://github.com/iiasa/message-ix-models
 Project-URL: repository, https://github.com/iiasa/message-ix-models
 Project-URL: documentation, https://docs.messageix.org/models
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,14 +15,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: R
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: click
```

### Comparing `message-ix-models-2024.1.29rc1/README.rst` & `message-ix-models-2024.4.2rc1/README.rst`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/doc/Makefile` & `message-ix-models-2024.4.2rc1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/doc/_static/combined-logo-white.png` & `message-ix-models-2024.4.2rc1/doc/_static/combined-logo-white.png`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/doc/_static/combined-logo-white.svg` & `message-ix-models-2024.4.2rc1/doc/_static/combined-logo-white.svg`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/doc/_static/custom.css` & `message-ix-models-2024.4.2rc1/doc/_static/custom.css`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/doc/_static/favicon.svg` & `message-ix-models-2024.4.2rc1/doc/_static/favicon.svg`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/doc/_static/logo-white.png` & `message-ix-models-2024.4.2rc1/doc/_static/logo-white.png`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/doc/_static/message-ix-models-logo-white.svg` & `message-ix-models-2024.4.2rc1/doc/_static/message-ix-models-logo-white.svg`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/doc/_template/autosummary-class.rst` & `message-ix-models-2024.4.2rc1/doc/_template/autosummary-class.rst`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/doc/_template/autosummary-module.rst` & `message-ix-models-2024.4.2rc1/doc/_template/autosummary-module.rst`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/doc/api/data-sources.rst` & `message-ix-models-2024.4.2rc1/doc/api/data-sources.rst`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/doc/api/disutility.rst` & `message-ix-models-2024.4.2rc1/doc/api/disutility.rst`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/doc/api/model-bare.rst` & `message-ix-models-2024.4.2rc1/doc/api/model-bare.rst`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/doc/api/model-build.rst` & `message-ix-models-2024.4.2rc1/doc/api/model-build.rst`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/doc/api/model-emissions.rst` & `message-ix-models-2024.4.2rc1/doc/api/model-emissions.rst`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/doc/api/model-snapshot.rst` & `message-ix-models-2024.4.2rc1/doc/api/model-snapshot.rst`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/doc/api/model.rst` & `message-ix-models-2024.4.2rc1/doc/api/model.rst`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/doc/api/project.rst` & `message-ix-models-2024.4.2rc1/doc/api/project.rst`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/doc/api/report/index.rst` & `message-ix-models-2024.4.2rc1/doc/api/report/index.rst`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/doc/api/tools.rst` & `message-ix-models-2024.4.2rc1/doc/api/tools.rst`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/doc/api/util.rst` & `message-ix-models-2024.4.2rc1/doc/api/util.rst`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
    .adapt_R11_R14
    .as_codes
    broadcast
    cached
    check_support
    convert_units
    copy_column
+   datetime_now_with_tz
    ffill
    identify_nodes
    iter_keys
    load_package_data
    load_private_data
    local_data_path
    make_io
@@ -48,14 +49,15 @@
    minimum_version
    ~node.nodes_ex_world
    package_data_path
    private_data_path
    same_node
    same_time
    series_of_pint_quantity
+   show_versions
 
 .. automodule:: message_ix_models.util
    :members:
    :exclude-members: as_codes, eval_anno
 
 .. autodata:: message_ix_models.util.cache.SKIP_CACHE
```

### Comparing `message-ix-models-2024.1.29rc1/doc/api/workflow.rst` & `message-ix-models-2024.4.2rc1/doc/api/workflow.rst`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/doc/cli.rst` & `message-ix-models-2024.4.2rc1/doc/cli.rst`

 * *Files 16% similar despite different names*

```diff
@@ -4,53 +4,66 @@
 This page describes how to use the :program:`mix-models` command-line interface (CLI) to perform common tasks.
 :program:`mix-models` is organized into **commands** and **subcommands**, sometimes in multiple levels.
 Our goal is that the *semantics* of all commands are similar, so that interacting with each command feels similar.
 
 .. contents::
    :local:
 
-
 Controlling CLI behaviour
 =========================
 
 To support a variety of complex use-cases, the MESSAGEix stack takes configuration and inputs from several places:
 
 :mod:`ixmp` configuration file: :file:`config.json`
 ---------------------------------------------------
+
 :mod:`ixmp` keeps track of named Platforms and their associated databases, and stores information in its :file:`config.json` file.
-See :mod:`ixmp.config`.
+See :ref:`ixmp:configuration` in the documentation.
 List existing platforms::
 
     $ ixmp platform list
 
 To add a specific database, you can use the ixmp CLI [1]_::
 
     $ ixmp platform add [PLATFORMNAME] jdbc oracle [COMPUTER]:[PORT]/[SERVICENAME] [USERNAME] [PASSWORD]
 
 You may also want to make this the *default* platform.
-Unless told otherwise, :mod:`message_ix_models` creates :class:`~ixmp.Platform` objects without any arguments (``mp = ixmp.Platform()``); this loads the default platform.
+Unless told otherwise, :mod:`message_ix_models` creates :class:`~ixmp.Platform` objects without any arguments (:py:`mp = ixmp.Platform()`); this loads the default platform.
 Set the default::
 
     $ ixmp platform add default [PLATFORMNAME]
 
-:mod:`message_ix` stores only one configuration value in :file:`config.json`: ``'message model dir'``, the path to the GAMS model files.
-MESSAGEix-GLOBIOM uses the GAMS model files from the current :mod:`message_ix` ``master`` branch, so you should not set this, or unset it when using :mod:`message_ix_models`.
+:mod:`message_ix` recognizes the following :file:`config.json` value:
+
+``message_model_dir``
+   Path to the GAMS model files.
+   Most code in MESSAGEix-GLOBIOM expects the GAMS model files from the current :mod:`message_ix` ``main`` branch, so you should not set this, or unset it when using :mod:`message_ix_models`.
+
+:mod:`message_ix_models` recognizes the following 2 :file:`config.json` values:
+
+``message_local_data``
+   Path to local data, if it is set and not overridden.
+``no_message_data``
+   If not set or :any:`False`, then the CLI displays a warning message if the private :mod:`message_data` package is not installed::
 
-:mod:`message_ix_models` will use the :file:`config.json` value ``"message_local_data"`` for local data, if it is set and not overridden.
+      Warning: message_data is not installed or cannot be imported; see the documentation via --help
+
+   If set to :any:`True`, then the message is suppressed::
+
+      $ mix-models config set no_message_data true
 
 .. [1] ``[COMPUTER]`` is in this case either the hostname or the IP address.
 
 Environment variables
 ---------------------
 Some code responds to environment variables.
 For example, ixmp responds to ``IXMP_DATA``, which tells it where to find the file :file:`config.json`.
 
 :mod:`message_ix_models` responds to ``MESSAGE_LOCAL_DATA``; see :ref:`the discussion of local data <local-data>`.
 
-
 CLI parameters (arguments and options)
 --------------------------------------
 
 Each command has zero or more arguments and options.
 **Arguments** are mandatory and follow the command name in a certain order.
 **Options**, as the name implies, are not required.
 If an option is omitted, a default value is used; the code and ``--help`` text make clear what the default behaviour is.
@@ -59,32 +72,32 @@
 Consider the following examples::
 
     $ mix-data --opt0=foo cmd1 --opt1=bar arg1 cmd2 --opt2=baz arg2
     $ mix-data --opt0=foo cmd1            arg1 cmd3 --opt3=baz arg3a arg3b
 
 In these examples:
 
-- ``--opt0`` is an option that (potentially) affects **any** command, including the subcommands ``cmd2`` or ``cmd3``.
-- ``--opt1`` and ``arg1`` are an option and mandatory argument to the command ``cmd1``.
-  They might not have any relevance to other ``mix-data`` commands.
-- ``cmd2`` and ``cmd3`` are distinct subcommands of ``cmd1``.
+- :program:`--opt0` is an option that (potentially) affects **any** command, including the subcommands :program:`cmd2` or :program:`cmd3`.
+- :program:`--opt1` and :program:`arg1` are an option and mandatory argument to the command :program:`cmd1`.
+  They might not have any relevance to other :program:`mix-models` commands.
+- :program:`cmd2` and :program:`cmd3` are distinct subcommands of :program:`cmd1`.
 
-  - They *may* respond to ``--opt1`` and ``arg1``, and to ``--opt0``; at least, they *must* not contradict them.
+  - They *may* respond to :program:`--opt1` and :program:`arg1`, and to :program:`--opt0`; at least, they *must* not contradict them.
   - They each may have their own options and arguments, which can be distinct.
 
 .. tip:: Use ``--help`` for any (sub)command to read about its behaviour.
    If the help text does not make the behaviour clear, `file an issue <https://github.com/iiasa/message-ix-models/issues/new>`_.
 
 Configuration files and metadata
 --------------------------------
 For some features of the code, the default behaviour is very elaborate and serves for most uses; but we also provide the option to override it.
 This default behaviour or optional behaviour is defined by reading an input file.
 These are stored in the :ref:`package data <package-data>` directory.
 
-For example, ``mix-models report`` loads reporting configuration from :file:`message_ix_models/data/report/global.yaml`, a YAML file with hundreds of lines.
+For example, :program:`mix-models report` loads reporting configuration from :file:`message_ix_models/data/report/global.yaml`, a YAML file with hundreds of lines.
 Optionally, a different file can be used::
 
     $ mix-models report --config other
 
 …looks for a file :file:`other.yaml` in the :ref:`local data <local-data>` directory or current working directory. Or::
 
     $ mix-models report --config /path/to/another/file.yaml
@@ -95,83 +108,92 @@
 Important CLI options and commands
 ==================================
 
 .. _cli-help:
 
 Top-level options and commands
 ------------------------------
-``mix-models --help`` describes these::
+:program:`mix-models --help` describes these::
 
-    $ mix-models --help
     Usage: mix-models [OPTIONS] COMMAND [ARGS]...
 
       Command-line interface for MESSAGEix-GLOBIOM model tools.
 
       Every tool and script in this repository is accessible through this CLI.
       Scripts are grouped into commands and sub-commands. For help on specific
-      (sub)commands, use --help, e.g.:
+      (sub)commands, use --help, for instance:
 
-              mix-models cd-links --help
-              mix-models cd-links run --help
+              mix-models report --help
+              mix-models ssp gen-structures --help
 
       The top-level options --platform, --model, and --scenario are used by
-      commands that access specific message_ix scenarios; these can also be
-      specified with --url.
+      commands that access specific MESSAGEix scenarios in a specific ixmp
+      platform/database; these can also be specified with --url.
 
-      For more information, see
-      https://docs.messageix.org/projects/models2/en/latest/cli.html
+      For complete documentation, see
+      https://docs.messageix.org/projects/models/en/latest/cli.html
 
     Options:
       --url ixmp://PLATFORM/MODEL/SCENARIO[#VERSION]
                                       Scenario URL.
-      --platform PLATFORM             Configured platform name.
+      --platform PLATFORM             ixmp platform name.
       --model MODEL                   Model name for some commands.
       --scenario SCENARIO             Scenario name for some commands.
-      --version INTEGER               Scenario version.
+      --version INTEGER               Scenario version for some commands.
       --local-data PATH               Base path for local data.
       -v, --verbose                   Print DEBUG-level log messages.
       --help                          Show this message and exit.
 
     Commands:
-      cd-links         CD-LINKS project.
-      dl               Retrieve data from primary sources.
-      engage           ENGAGE project.
-      iiasapp          Import power plant capacity.
-      material         Model with materials accounting.
-      prep-submission  Prepare scenarios for submission to database.
-      report           Postprocess results.
-      res              MESSAGE-GLOBIOM reference energy system (RES).
-      techs            Export data from data/technology.yaml to CSV.
-      transport        MESSAGEix-Transport variant.
+      buildings         MESSAGEix-Buildings model.
+      cd-links          CD-LINKS project.
+      config            Get and set configuration keys.
+      covid             COVID project.
+      engage            ENGAGE project.
+      export-test-data  Prepare data for testing.
+      fetch             Retrieve data from primary sources.
+      iiasapp           Import power plant capacity.
+      last-log          Show the location of the last log file, if any.
+      material          Model with materials accounting.
+      model             MESSAGEix-GLOBIOM reference energy system (RES).
+      navigate          NAVIGATE project.
+      prep-submission   Prepare scenarios for submission to an IIASA Scenario...
+      report            Postprocess results.
+      res               MESSAGEix-GLOBIOM reference energy system (RES).
+      ssp               Shared Socioeconomic Pathways (SSP) project.
+      techs             Export metadata to technology.csv.
+      testing           Manipulate test data.
+      transport         MESSAGEix-Transport variant.
+      water-ix          MESSAGEix-Water and Nexus variant.
 
-To explain further:
+Further information about the top-level options:
 
-``--platform PLATFORM`` or ``--url``
+:program:`--platform PLATFORM` or :program:`--url`
    By default, message_data connects to the default ixmp Platform.
    These options direct it to work with a different Platform.
 
-``--model MODEL --scenario SCENARIO`` or ``--url``
+:program:`--model MODEL --scenario SCENARIO` or :program:`--url`
     Many commands use an *existing* |Scenario| as a starting point, and begin by cloning that Scenario to a new (model name, scenario name).
     For any such command, these top-level options define the starting point/initial Scenario to clone/‘baseline’.
 
-    In contrast, see ``--output-model``, below.
-
+    In contrast, see :program:`--output-model`, below.
 
 Common options
 --------------
+
 Since :mod:`message_ix_models.model` and :mod:`message_ix_models.project` codes often perform similar tasks, their CLI options and arguments are provided in :mod:`.util.click` for easy re-use.
 These include:
 
-``ssp`` argument
+:program:`SSP` argument
    This takes one of the values 'SSP1', 'SSP2', or 'SSP3'.
 
    Commands that will not work for one or more of the SSPs should check the argument value given by the user and raise :class:`NotImplementedError`.
 
-``--output-model NAME`` option
-   This option is a counterpart to the top-level ``--url/--model/--scenario`` options.
+:program:`--output-model NAME` option
+   This option is a counterpart to the top-level :program:`--url`, :program:`--model`, or :program:`--scenario` options.
    A command that starts from one Scenario, and builds one or more Scenarios from it will clone *to* a new (model name, scenario name);
-   ``--output-model`` gives the model name.
+   :program:`--output-model` gives the model name.
 
    Current code generates a variety of fixed (non-configurable) scenario names; use ``--help`` for each command to see which.
 
 
 To employ these in new code, refer to the example of existing code.
```

### Comparing `message-ix-models-2024.1.29rc1/doc/conf.py` & `message-ix-models-2024.4.2rc1/doc/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,14 +139,15 @@
     "m-data": (
         f"https://{_token}:@docs.messageix.org/projects/models-internal/en/latest/",
         # Use a local copy of objects.inv, if the user has one
         (local_inv("message_data"), None),
     ),
     "pandas": ("https://pandas.pydata.org/pandas-docs/stable/", None),
     "pint": ("https://pint.readthedocs.io/en/stable/", None),
+    "platformdirs": ("https://platformdirs.readthedocs.io/en/latest", None),
     "pooch": ("https://www.fatiando.org/pooch/latest/", None),
     "pytest": ("https://docs.pytest.org/en/stable/", None),
     "python": ("https://docs.python.org/3/", None),
     "sdmx": ("https://sdmx1.readthedocs.io/en/stable/", None),
 }
 
 # -- Options for sphinx.ext.linkcode / ixmp.util.sphinx_linkcode_github ----------------
```

### Comparing `message-ix-models-2024.1.29rc1/doc/data.rst` & `message-ix-models-2024.4.2rc1/doc/data.rst`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/doc/develop.rst` & `message-ix-models-2024.4.2rc1/doc/develop.rst`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/doc/distrib.rst` & `message-ix-models-2024.4.2rc1/doc/distrib.rst`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/doc/index.rst` & `message-ix-models-2024.4.2rc1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/doc/make.bat` & `message-ix-models-2024.4.2rc1/doc/make.bat`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/doc/migrate.rst` & `message-ix-models-2024.4.2rc1/doc/migrate.rst`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/doc/pkg-data/codelists.rst` & `message-ix-models-2024.4.2rc1/doc/pkg-data/codelists.rst`

 * *Files 4% similar despite different names*

```diff
@@ -7,20 +7,22 @@
    :local:
 
 .. _commodity-yaml:
 
 Commodities (``commodity.yaml``)
 ================================
 
-These codes hav the following annotations:
+These codes have the following annotations:
 
 ``level`` (mandatory)
    Level where this commodity typically (not exclusively) occurs.
 ``units`` (mandatory)
    Units typically associated with this commodity.
+``iea-eweb-flow`` (optional)
+   List of ``FLOW`` codes from the IEA :ref:`tools-iea-web` associated with this MESSAGEix-GLOBIOM commodity.
 ``iea-eweb-product`` (optional)
    List of ``PRODUCT`` codes from the IEA :ref:`tools-iea-web` associated with this MESSAGEix-GLOBIOM commodity.
 
 .. literalinclude:: ../../message_ix_models/data/commodity.yaml
    :language: yaml
 
 .. _level-yaml:
```

### Comparing `message-ix-models-2024.1.29rc1/doc/pkg-data/iiasa-se.rst` & `message-ix-models-2024.4.2rc1/doc/pkg-data/iiasa-se.rst`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/doc/pkg-data/node.rst` & `message-ix-models-2024.4.2rc1/doc/pkg-data/node.rst`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/doc/pkg-data/relation.rst` & `message-ix-models-2024.4.2rc1/doc/pkg-data/relation.rst`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/doc/pkg-data/year.rst` & `message-ix-models-2024.4.2rc1/doc/pkg-data/year.rst`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/doc/releasing.rst` & `message-ix-models-2024.4.2rc1/doc/releasing.rst`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/doc/repro.rst` & `message-ix-models-2024.4.2rc1/doc/repro.rst`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/doc/requirements.txt` & `message-ix-models-2024.4.2rc1/doc/requirements.txt`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/doc/water/files.rst` & `message-ix-models-2024.4.2rc1/doc/water/files.rst`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/doc/water/index.rst` & `message-ix-models-2024.4.2rc1/doc/water/index.rst`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/doc/whatsnew.rst` & `message-ix-models-2024.4.2rc1/doc/whatsnew.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,36 @@
 What's new
 **********
 
 .. Next release
 .. ============
 
+v2024.4.2
+=========
+
+- The :class:`.SSPUpdate` data provider pulls data from the SSP 2024 "Release 3.0" data files, and handles both the earlier and current structures (:pull:`156`).
+- Improve :class:`.ExoDataSource` with :meth:`.raise_on_extra_kw` utility method, automatic copy of source keyword arguments (:pull:`156`).
+- Expose :func:`.node.nodes_ex_world` for use as a genno (reporting) operator.
+- Raise DeprecationWarning from :func:`.util.sdmx.eval_anno`; remove internal usage of this deprecated method (:pull:`156`).
+- Reduce verbosity when using the :program:`mix-models` CLI when :mod:`message_data` is not installed (:issue:`37`, :pull:`156`).
+- Improve logging (:pull:`156`).
+
+  - Use multi-threaded logging for better performance.
+    Logging to stdout and file is on a separate thread and does not block operations on the main thread.
+  - Add automatic file logging.
+    Log versions of packages to file when using :func:`.workflow.make_click_command`.
+  - New CLI command :program:`mix-models last-log` to retrieve the location of the latest log file.
+- Update :doc:`cli` (:pull:`156`).
+- Improve performance in :func:`.disutility.data_conversion` (:pull:`156`).
+- Use :func:`platformdirs.user_cache_path` in more places; remove cache-path handling code (:pull:`156`).
+- Add :func:`.util.datetime_now_with_tz` (:pull:`156`).
+- Add :func:`.util.show_versions`, wrapping :func:`ixmp.util.show_versions` and returning its output as :class:`str` (:pull:`156`).
+- :func:`.util.private_data_path` returns an alternate, local data path if :mod:`message_data` is not installed (:pull:`156`).
+- Annotate :py:`c="transport"` in :ref:`the commodity code list <commodity-yaml>` with associated :ref:`IEA (E)WEB <tools-iea-web>` flows (:pull:`153`).
+
 v2024.1.29
 ==========
 
 - Add :ref:`tools-iea-web` for handling data from the International Energy Agency (IEA) Extended World Energy Balances (:issue:`25`, :pull:`75`).
 - Add :ref:`tools-wb` and :func:`.assign_income_groups` to assign MESSAGE regions to World Bank income groups (:pull:`144`).
 - Adjust :mod:`.report.compat` for genno version 1.22 (:issue:`141`, :pull:`142`).
 - Raise informative exception from :meth:`.ScenarioInfo.io_units` (:pull:`151`).
```

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/__init__.py` & `message-ix-models-2024.4.2rc1/message_ix_models/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 
 try:
     __version__ = version(__name__)
 except PackageNotFoundError:  # pragma: no cover
     # Package is not installed
     __version__ = "999"
 
-# No logging to stdout (console) by default
-setup_logging(console=False)
+# By default, no logging to console/stdout or to file
+setup_logging(console=False, file=False)
 
 # Use iam_units.registry as the default pint.UnitsRegistry
 pint.set_application_registry(registry)
 
 # Ensure at least one Context instance is created
 Context()
```

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/data/cd_links/unit.yaml` & `message-ix-models-2024.4.2rc1/message_ix_models/data/cd_links/unit.yaml`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/data/commodity.yaml` & `message-ix-models-2024.4.2rc1/message_ix_models/data/commodity.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -137,14 +137,15 @@
   name: Transportation
   description: >-
     For MESSAGEix-Transport, this commodity is not used; it is replaced by a
     disaggregated set of transport service demands (representing e.g. light-
     duty vehicles, civil aviation, freight transport, etc.)
   level: useful
   units: GWa
+  iea-eweb-flow: [DOMESAIR, DOMESNAV, RAIL, ROAD, TRNONSPE]
 
 # The following codes also appear in a recent (2020-02-28) SSP2 scenario, but
 # are not currently used by model.bare.create_res.
 #
 # Aff_CO2_G4M
 # Agri_CH4
 # Agri_N2O
```

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/data/edits/messageix-transport-core.yaml` & `message-ix-models-2024.4.2rc1/message_ix_models/data/edits/messageix-transport-core.yaml`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/data/edits/messageix-transport-input.yaml` & `message-ix-models-2024.4.2rc1/message_ix_models/data/edits/messageix-transport-input.yaml`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/data/iiasa-se/def-regions.yaml` & `message-ix-models-2024.4.2rc1/message_ix_models/data/iiasa-se/def-regions.yaml`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/data/iiasa-se/mappings-R12.yaml` & `message-ix-models-2024.4.2rc1/message_ix_models/data/iiasa-se/mappings-R12.yaml`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/data/ipcc/1996_v3_t1-2.csv` & `message-ix-models-2024.4.2rc1/message_ix_models/data/ipcc/1996_v3_t1-2.csv`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/data/level.yaml` & `message-ix-models-2024.4.2rc1/message_ix_models/data/level.yaml`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/data/node/ADVANCE.yaml` & `message-ix-models-2024.4.2rc1/message_ix_models/data/node/ADVANCE.yaml`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/data/node/B210-R11.yaml` & `message-ix-models-2024.4.2rc1/message_ix_models/data/node/B210-R11.yaml`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/data/node/R11.yaml` & `message-ix-models-2024.4.2rc1/message_ix_models/data/node/R11.yaml`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/data/node/R12.yaml` & `message-ix-models-2024.4.2rc1/message_ix_models/data/node/R12.yaml`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/data/node/R14.yaml` & `message-ix-models-2024.4.2rc1/message_ix_models/data/node/R14.yaml`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/data/node/R17.yaml` & `message-ix-models-2024.4.2rc1/message_ix_models/data/node/R17.yaml`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/data/node/R20.yaml` & `message-ix-models-2024.4.2rc1/message_ix_models/data/node/R20.yaml`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/data/node/R32.yaml` & `message-ix-models-2024.4.2rc1/message_ix_models/data/node/R32.yaml`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/data/node/RCP.yaml` & `message-ix-models-2024.4.2rc1/message_ix_models/data/node/RCP.yaml`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/data/relation/A.yaml` & `message-ix-models-2024.4.2rc1/message_ix_models/data/relation/A.yaml`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/data/relation/B.yaml` & `message-ix-models-2024.4.2rc1/message_ix_models/data/relation/B.yaml`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/data/relation/CD-LINKS.yaml` & `message-ix-models-2024.4.2rc1/message_ix_models/data/relation/CD-LINKS.yaml`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/data/report/global.yaml` & `message-ix-models-2024.4.2rc1/message_ix_models/data/report/global.yaml`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/data/sdmx/ADVANCE.xml` & `message-ix-models-2024.4.2rc1/message_ix_models/data/sdmx/ADVANCE.xml`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/data/sdmx/ICONICS_SSP(2017).xml` & `message-ix-models-2024.4.2rc1/message_ix_models/data/sdmx/ICONICS_SSP(2017).xml`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/data/sdmx/ICONICS_SSP(2024).xml` & `message-ix-models-2024.4.2rc1/message_ix_models/data/sdmx/ICONICS_SSP(2024).xml`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/data/sdmx/IEA_COUNTRY_IEA(2023).xml` & `message-ix-models-2024.4.2rc1/message_ix_models/data/sdmx/IEA_COUNTRY_IEA(2023).xml`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/data/sdmx/IEA_COUNTRY_OECD(2021).xml` & `message-ix-models-2024.4.2rc1/message_ix_models/data/sdmx/IEA_COUNTRY_OECD(2021).xml`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/data/sdmx/IEA_COUNTRY_OECD(2022).xml` & `message-ix-models-2024.4.2rc1/message_ix_models/data/sdmx/IEA_COUNTRY_OECD(2022).xml`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/data/sdmx/IEA_COUNTRY_OECD(2023).xml` & `message-ix-models-2024.4.2rc1/message_ix_models/data/sdmx/IEA_COUNTRY_OECD(2023).xml`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/data/sdmx/IEA_FLOW_IEA(2023).xml` & `message-ix-models-2024.4.2rc1/message_ix_models/data/sdmx/IEA_FLOW_IEA(2023).xml`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/data/sdmx/IEA_FLOW_OECD(2021).xml` & `message-ix-models-2024.4.2rc1/message_ix_models/data/sdmx/IEA_FLOW_OECD(2021).xml`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/data/sdmx/IEA_FLOW_OECD(2022).xml` & `message-ix-models-2024.4.2rc1/message_ix_models/data/sdmx/IEA_FLOW_OECD(2022).xml`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/data/sdmx/IEA_FLOW_OECD(2023).xml` & `message-ix-models-2024.4.2rc1/message_ix_models/data/sdmx/IEA_FLOW_OECD(2023).xml`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/data/sdmx/IEA_PRODUCT_IEA(2023).xml` & `message-ix-models-2024.4.2rc1/message_ix_models/data/sdmx/IEA_PRODUCT_IEA(2023).xml`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/data/sdmx/IEA_PRODUCT_OECD(2021).xml` & `message-ix-models-2024.4.2rc1/message_ix_models/data/sdmx/IEA_PRODUCT_OECD(2021).xml`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/data/sdmx/IEA_PRODUCT_OECD(2022).xml` & `message-ix-models-2024.4.2rc1/message_ix_models/data/sdmx/IEA_PRODUCT_OECD(2022).xml`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/data/sdmx/IEA_PRODUCT_OECD(2023).xml` & `message-ix-models-2024.4.2rc1/message_ix_models/data/sdmx/IEA_PRODUCT_OECD(2023).xml`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/data/sdmx/IIASA_ECE_AGENCIES(0.1).xml` & `message-ix-models-2024.4.2rc1/message_ix_models/data/sdmx/IIASA_ECE_AGENCIES(0.1).xml`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/data/technology.yaml` & `message-ix-models-2024.4.2rc1/message_ix_models/data/technology.yaml`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/data/unit/snapshot.yaml` & `message-ix-models-2024.4.2rc1/message_ix_models/data/unit/snapshot.yaml`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/data/water/set.yaml` & `message-ix-models-2024.4.2rc1/message_ix_models/data/water/set.yaml`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/data/water/technology.yaml` & `message-ix-models-2024.4.2rc1/message_ix_models/data/water/technology.yaml`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/data/year/A.yaml` & `message-ix-models-2024.4.2rc1/message_ix_models/data/year/A.yaml`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/data/year/B.yaml` & `message-ix-models-2024.4.2rc1/message_ix_models/data/year/B.yaml`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/model/bare.py` & `message-ix-models-2024.4.2rc1/message_ix_models/model/bare.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from urllib.parse import urlunsplit
 
 import message_ix
 from sdmx.model.v21 import Code
 
 import message_ix_models
 from message_ix_models import ScenarioInfo, Spec
-from message_ix_models.util import eval_anno
 
 from .build import apply_spec
 from .config import Config
 from .data import get_data
 from .structure import codelists, get_codes
 
 log = logging.getLogger(__name__)
@@ -130,15 +129,17 @@
     # Add levels
     add.set["level"] = get_codes("level")
 
     # Add commodities
     add.set["commodity"] = get_codes("commodity")
 
     # Add units, associated with commodities
-    units = set(eval_anno(commodity, "unit") for commodity in add.set["commodity"])
+    units = set(
+        commodity.eval_annotation(id="unit") for commodity in add.set["commodity"]
+    )
     # Deduplicate by converting to a set and then back; not strictly necessary,
     # but reduces duplicate log entries
     add.set["unit"] = sorted(filter(None, units))
 
     if context.model.res_with_dummies:
         # Add dummy technologies
         add.set["technology"].extend([Code(id="dummy"), Code(id="dummy source")])
```

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/model/build.py` & `message-ix-models-2024.4.2rc1/message_ix_models/model/build.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/model/config.py` & `message-ix-models-2024.4.2rc1/message_ix_models/model/config.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/model/disutility.py` & `message-ix-models-2024.4.2rc1/message_ix_models/model/disutility.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 import logging
 from collections import defaultdict
 from copy import copy
 from functools import partial
 from itertools import product
-from typing import List, Mapping, MutableMapping, Sequence, Union
+from typing import List, Mapping, MutableMapping, Sequence
 
 import message_ix
 import pandas as pd
-from sdmx.model.v21 import Annotation, Code
+from sdmx.model.common import Annotation, Code
 
 from message_ix_models import ScenarioInfo, Spec
 from message_ix_models.model.build import apply_spec
 from message_ix_models.util import (
     broadcast,
-    eval_anno,
     make_io,
     make_matched_dfs,
     make_source_tech,
     merge_data,
     nodes_ex_world,
     same_node,
 )
 
 log = logging.getLogger(__name__)
 
-CodeLike = Union[str, Code]
-
 
 def add(
     scenario: message_ix.Scenario,
     groups: Sequence[Code],
     technologies: Sequence[Code],
     template: Code,
     **options,
@@ -77,17 +74,19 @@
 
     # Add conversion technologies
     for t, g in product(technologies, groups):
         # String formatting arguments
         fmt = dict(technology=t, group=g)
 
         # Format each field in the "input" and "output" annotations
-        input = {k: v.format(**fmt) for k, v in eval_anno(template, id="input").items()}
+        input = {
+            k: v.format(**fmt) for k, v in template.eval_annotation(id="input").items()
+        }
         output = {
-            k: v.format(**fmt) for k, v in eval_anno(template, id="output").items()
+            k: v.format(**fmt) for k, v in template.eval_annotation(id="output").items()
         }
 
         # - Format the ID string from the template
         # - Create new "input" and "output" annotations
         # - Copy other annotations unmodified
         t_code = Code(
             id=template.id.format(**fmt),
@@ -150,38 +149,38 @@
         return df.merge(info.par["duration_period"], left_on=col_name, right_on="year")[
             "value_y"
         ]
 
     return func
 
 
-def data_conversion(info, spec) -> MutableMapping[str, pd.DataFrame]:
+def data_conversion(info, spec: Spec) -> MutableMapping[str, pd.DataFrame]:
     """Generate input and output data for disutility conversion technologies."""
     common = dict(
         mode="all",
         year_vtg=info.Y,
         year_act=info.Y,
         # No subannual detail
         time="year",
         time_origin="year",
         time_dest="year",
     )
 
     # Use the spec to retrieve information
-    technology = spec["add"].set["technology"]
+    technology: List[Code] = spec.add.set["technology"]
 
     # Data to return
     data0: Mapping[str, List[pd.DataFrame]] = defaultdict(list)
 
     # Loop over conversion technologies
     for t in technology:
         # Use the annotations on the technology Code to get information about the
         # commodity, level, and unit
-        input = eval_anno(t, "input")
-        output = eval_anno(t, "output")
+        input = t.eval_annotation(id="input")
+        output = t.eval_annotation(id="output")
         if None in (input, output):
             if t.id == "disutility source":
                 continue  # Data for this tech is from data_source()
             else:  # pragma: no cover
                 raise ValueError(t)  # Error in user input
 
         # Make input and output data frames
@@ -190,40 +189,43 @@
             (output["commodity"], output["level"], output["unit"]),
             1.0,
             on="output",
             technology=t.id,
             **common,
         )
         for par, df in i_o.items():
-            # Broadcast across nodes
-            df = df.pipe(broadcast, node_loc=nodes_ex_world(info.N)).pipe(same_node)
-
             if par == "input":
                 # Add input of disutility
                 df = pd.concat(
                     [df, df.assign(commodity="disutility", unit="-")], ignore_index=True
                 )
 
             data0[par].append(df)
 
-    # Concatenate to a single data frame per parameter
-    data = {par: pd.concat(dfs, ignore_index=True) for par, dfs in data0.items()}
+    # - Concatenate to a single data frame per parameter
+    # - Broadcast across nodes
+    data = {
+        par: pd.concat(dfs, ignore_index=True)
+        .pipe(broadcast, node_loc=nodes_ex_world(info.N))
+        .pipe(same_node)
+        for par, dfs in data0.items()
+    }
 
     # Create data for capacity_factor
     data.update(make_matched_dfs(base=data["input"], capacity_factor=1.0))
 
     return data
 
 
 def data_source(info, spec) -> Mapping[str, pd.DataFrame]:
     """Generate data for a technology that emits the “disutility” commodity."""
     # List of input levels where disutility commodity must exist
     levels = set()
     for t in spec["add"].set["technology"]:
-        input = eval_anno(t, "input")
+        input = t.eval_annotation(id="input")
         if input:
             levels.add(input["level"])
 
     log.info(f"Generate disutility on level(s): {repr(levels)}")
 
     # Use default capacity_factor = 1.0
     result = make_source_tech(
```

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/model/emissions.py` & `message-ix-models-2024.4.2rc1/message_ix_models/model/emissions.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/model/macro.py` & `message-ix-models-2024.4.2rc1/message_ix_models/model/macro.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Tools for calibrating MACRO for MESSAGEix-GLOBIOM.
 
 See :doc:`message-ix:macro` for *general* documentation on MACRO and MESSAGE-MACRO. This
 module contains tools specifically for using these models with MESSAGEix-GLOBIOM.
 """
+
 import logging
 from functools import lru_cache
 from itertools import product
 from pathlib import Path
 from typing import TYPE_CHECKING, List, Literal, Mapping, Optional, Union
 
 import pandas as pd
```

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/model/snapshot.py` & `message-ix-models-2024.4.2rc1/message_ix_models/model/snapshot.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Prepare base models from snapshot data."""
+
 import logging
 from pathlib import Path
 
 import pandas as pd
 from message_ix import Scenario
 from message_ix.models import MACRO
 from tqdm import tqdm
```

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/model/structure.py` & `message-ix-models-2024.4.2rc1/message_ix_models/model/structure.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import click
 import pandas as pd
 import pycountry
 import xarray as xr
 from iam_units import registry
 from sdmx.model.v21 import Annotation, Code, Codelist
 
-from message_ix_models.util import eval_anno, load_package_data, package_data_path
+from message_ix_models.util import load_package_data, package_data_path
 from message_ix_models.util.sdmx import as_codes
 
 log = logging.getLogger(__name__)
 
 
 @lru_cache()
 def codelists(kind: str) -> List[str]:
@@ -122,15 +122,15 @@
     name : str
         Name of the set.
     template : Code
         Must have Python format strings for its its :attr:`id` and :attr:`name`
         attributes.
     """
     # eval() and remove the original annotation
-    dims = eval_anno(template, "_generate")
+    dims = template.eval_annotation(id="_generate")
     template.pop_annotation(id="_generate")
 
     def _base(dim, match):
         """Return codes along dimension `dim`.
 
         If `match` is given, only children matching an expression."""
         dim_codes = data[dim]["add"]
@@ -187,15 +187,15 @@
 
     codes = []  # Accumulate codes
     deferred = []
     for code in as_codes(data[name].get("add", [])):
         if name in {"commodity", "technology"}:
             process_units_anno(name, code, quiet=True)
 
-        if eval_anno(code, "_generate"):
+        if code.eval_annotation(id="_generate"):
             # Requires a call to generate_product(); do these last
             deferred.append(code)
             continue
 
         codes.append(code)
 
         if hierarchical:
```

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/model/water/build.py` & `message-ix-models-2024.4.2rc1/message_ix_models/model/water/build.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/model/water/cli.py` & `message-ix-models-2024.4.2rc1/message_ix_models/model/water/cli.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/model/water/data/__init__.py` & `message-ix-models-2024.4.2rc1/message_ix_models/model/water/data/__init__.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/model/water/data/demands.py` & `message-ix-models-2024.4.2rc1/message_ix_models/model/water/data/demands.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/model/water/data/infrastructure.py` & `message-ix-models-2024.4.2rc1/message_ix_models/model/water/data/infrastructure.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Prepare data for adding techs related to water distribution,
- treatment in urban & rural"""
+treatment in urban & rural"""
 
 from collections import defaultdict
 
 import pandas as pd
 from message_ix import make_df
 
 from message_ix_models.model.water.utils import map_yv_ya_lt
```

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/model/water/data/irrigation.py` & `message-ix-models-2024.4.2rc1/message_ix_models/model/water/data/irrigation.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/model/water/data/pre_processing/calculate_ppl_cooling_technology_shares.r` & `message-ix-models-2024.4.2rc1/message_ix_models/model/water/data/pre_processing/calculate_ppl_cooling_technology_shares.r`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/model/water/data/pre_processing/desalination.R` & `message-ix-models-2024.4.2rc1/message_ix_models/model/water/data/pre_processing/desalination.R`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/model/water/data/pre_processing/generate_water_constraints.R` & `message-ix-models-2024.4.2rc1/message_ix_models/model/water/data/pre_processing/generate_water_constraints.R`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/model/water/data/pre_processing/generate_water_constraints_monthly.r` & `message-ix-models-2024.4.2rc1/message_ix_models/model/water/data/pre_processing/generate_water_constraints_monthly.r`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/model/water/data/pre_processing/groundwater_harmonize.r` & `message-ix-models-2024.4.2rc1/message_ix_models/model/water/data/pre_processing/groundwater_harmonize.r`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/model/water/data/pre_processing/hydro_agg_basin.py` & `message-ix-models-2024.4.2rc1/message_ix_models/model/water/data/pre_processing/hydro_agg_basin.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,17 +152,17 @@
                                 str(year - i) + "-01-01", periods=12, freq="M"
                             )
                         ] - (delta_multiply * delta60)
 
                         final_temp = pd.concat((final_temp, temp), axis=1)
 
                 df_monthly = final_temp
-                df[
-                    pd.date_range(str(year) + "-01-01", periods=12, freq="M")
-                ] = final_temp.groupby(final_temp.columns.month, axis=1).mean()
+                df[pd.date_range(str(year) + "-01-01", periods=12, freq="M")] = (
+                    final_temp.groupby(final_temp.columns.month, axis=1).mean()
+                )
                 # 5 year monthly data
                 df_5y_m = df[df.columns[df.columns.year.isin(years)]]
                 # 5 year annual
                 # 50th quantile - q50
                 df_q50 = (
                     df_monthly.rolling(240, min_periods=1, axis=1)
                     .quantile(0.5, interpolation="linear")
@@ -315,17 +315,17 @@
 
         else:
             final_temp = eflow[
                 pd.date_range(str(year - i) + "-01-01", periods=12, freq="M")
             ]
 
     df_monthly = final_temp
-    eflow[
-        pd.date_range(str(year) + "-01-01", periods=12, freq="M")
-    ] = final_temp.groupby(final_temp.columns.month, axis=1).mean()
+    eflow[pd.date_range(str(year) + "-01-01", periods=12, freq="M")] = (
+        final_temp.groupby(final_temp.columns.month, axis=1).mean()
+    )
 
     eflow_5y_m = eflow[eflow.columns[eflow.columns.year.isin(years)]]
     eflow_5y_m.to_csv(wd11 + f"e-flow_5y_m_7p0_{iso3}.csv")
 
 val_2020_eflow = eflow_5y_m[pd.date_range("2020-01-01", periods=12, freq="M")].values()
 val_2020_eflowy = eflow_5y["2020-12-31"]
 eflow_5y.apply(lambda x: val_2020_eflowy).to_csv(wd11 + f"e-flow_no_climate_{iso3}.csv")
```

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/model/water/data/pre_processing/hydro_agg_raster.py` & `message-ix-models-2024.4.2rc1/message_ix_models/model/water/data/pre_processing/hydro_agg_raster.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 This script aggregates the global gridded data to any
 scale and also adjust unit conversions. The following
 script specifically aggregates global gridded hydrological
 data onto the basin
  mapping used in the nexus module.
 """
+
 import glob
 
 #  Import packages
 import os
 from datetime import datetime as dt
 
 import dask
```

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/model/water/data/pre_processing/hydro_agg_spatial.R` & `message-ix-models-2024.4.2rc1/message_ix_models/model/water/data/pre_processing/hydro_agg_spatial.R`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/model/water/data/water_for_ppl.py` & `message-ix-models-2024.4.2rc1/message_ix_models/model/water/data/water_for_ppl.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/model/water/data/water_supply.py` & `message-ix-models-2024.4.2rc1/message_ix_models/model/water/data/water_supply.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/model/water/reporting.py` & `message-ix-models-2024.4.2rc1/message_ix_models/model/water/reporting.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/model/water/utils.py` & `message-ix-models-2024.4.2rc1/message_ix_models/model/water/utils.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/project/advance/data.py` & `message-ix-models-2024.4.2rc1/message_ix_models/project/advance/data.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/project/ssp/__init__.py` & `message-ix-models-2024.4.2rc1/message_ix_models/project/ssp/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         if value is None:
             value = self._default
         setattr(obj, self._name, parse(value))
 
 
 @click.group("ssp")
 def cli():
-    pass
+    """Shared Socioeconomic Pathways (SSP) project."""
 
 
 @cli.command("gen-structures")
 @common_params("dry_run")
 @click.pass_obj
 def gen_structures(context, **kwargs):
     """(Re)Generate the SSP data structures in SDMX."""
```

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/project/ssp/structure.py` & `message-ix-models-2024.4.2rc1/message_ix_models/project/ssp/structure.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Manipulate data structures for working with the SSPs."""
+
 import logging
 from textwrap import wrap
 from typing import TYPE_CHECKING, Optional
 
 import sdmx
 import sdmx.model.v30 as m
 import sdmx.urn
```

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/report/__init__.py` & `message-ix-models-2024.4.2rc1/message_ix_models/report/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -242,15 +242,15 @@
 
     if context.report.legacy["use"]:
         return _invoke_legacy_reporting(context)
 
     with (
         nullcontext()
         if context.core.verbose
-        else silence_log(["genno", "message_ix_models"])
+        else silence_log("genno message_ix_models")
     ):
         rep, key = prepare_reporter(context)
 
     log_before(context, rep, key)
 
     if context.dry_run:
         return
```

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/report/cli.py` & `message-ix-models-2024.4.2rc1/message_ix_models/report/cli.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/report/compat.py` & `message-ix-models-2024.4.2rc1/message_ix_models/report/compat.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Compatibility code that emulates :mod:`.message_data` reporting."""
+
 import logging
 from functools import partial
 from itertools import chain, count
 from typing import TYPE_CHECKING, Any, Dict, List, Mapping, Optional
 
 from genno import Key, Quantity, quote
 from genno.core.key import iter_keys, single_key
```

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/report/config.py` & `message-ix-models-2024.4.2rc1/message_ix_models/report/config.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/report/operator.py` & `message-ix-models-2024.4.2rc1/message_ix_models/report/operator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """Atomic reporting operations for MESSAGEix-GLOBIOM."""
+
 import itertools
 import logging
 import re
 from typing import TYPE_CHECKING, Any, List, Mapping, Optional, Set, Tuple, Union
 
 import ixmp
 import pandas as pd
 from genno import Quantity
 from genno.core.operator import Operator
 from genno.operator import pow
 from iam_units import convert_gwp
 from iam_units.emissions import SPECIES
 
 from message_ix_models import Context
-from message_ix_models.util import add_par_data
+from message_ix_models.util import add_par_data, nodes_ex_world
 
 if TYPE_CHECKING:
     from pathlib import Path
 
     from genno import Computer, Key
     from sdmx.model.v21 import Code
 
@@ -30,14 +31,15 @@
     "exogenous_data",
     "filter_ts",
     "from_url",
     "get_ts",
     "gwp_factors",
     "make_output_path",
     "model_periods",
+    "nodes_ex_world",
     "remove_ts",
     "share_curtailment",
 ]
 
 
 def codelist_to_groups(
     codes: List["Code"], dim: str = "n"
```

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/report/plot.py` & `message-ix-models-2024.4.2rc1/message_ix_models/report/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Plots for MESSAGEix-GLOBIOM reporting.
 
 The current set functions on time series data stored on the scenario by
 :mod:`message_ix_models.report` or :mod:`message_data` legacy reporting.
 """
+
 import logging
 import re
 from datetime import datetime
 from typing import TYPE_CHECKING, List, Optional, Sequence
 
 import genno.compat.plotnine
 import pandas as pd
@@ -96,17 +97,15 @@
                 c.add(k, "filter_ts", all_data, copy(expr))
         else:
             for k in map(Key, cls.inputs):
                 # Add a computation to get the time series data for a specific variable
                 c.add(k, "get_ts", scenario_key, dict(variable=k.name))
 
         # Add the plot itself
-        # TODO once the genno class returns the added key, change to "return super().…"
-        super().add_tasks(c, key, *inputs[1:], strict=strict)
-        return key
+        return super().add_tasks(c, key, *inputs[1:], strict=strict)
 
     def ggtitle(self, value=None) -> p9.ggtitle:
         """Return :class:`plotnine.ggtitle` including the current date & time."""
         title_pieces = [
             (self.title or self.__doc__ or "").splitlines()[0].rstrip("."),
             f"[{self.unit}]" if self.unit else None,
             value,
```

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/report/sim.py` & `message-ix-models-2024.4.2rc1/message_ix_models/report/sim.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Simulated solution data for testing :mod:`~message_ix_models.report`."""
+
 import logging
 from collections import ChainMap, defaultdict
 from collections.abc import Mapping
 from copy import deepcopy
 from functools import lru_cache
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Sequence, Union
```

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/report/util.py` & `message-ix-models-2024.4.2rc1/message_ix_models/report/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,14 @@
 from genno import Key, Quantity
 from genno.compat.pyam.util import collapse as genno_collapse
 from genno.core.key import single_key
 from iam_units import registry
 from message_ix import Reporter
 from sdmx.model.v21 import Code
 
-from message_ix_models.util import eval_anno
-
 log = logging.getLogger(__name__)
 
 
 #: Replacements used in :meth:`collapse`.
 #: These are applied using :meth:`pandas.DataFrame.replace` with ``regex=True``; see the
 #: documentation of that method.
 #:
@@ -194,10 +192,13 @@
     k2 = rep.add("get_ts", f"ts data {_id}", k1, filters)
     return single_key(rep.add("store_ts", f"copy ts {_id}", "scenario", k2))
 
 
 def add_replacements(dim: str, codes: Iterable[Code]) -> None:
     """Update :data:`REPLACE_DIMS` for dimension `dim` with values from `codes`."""
     for code in codes:
-        label = eval_anno(code, "report")
-        if label is not None:
+        try:
+            label = str(code.get_annotation(id="report").text)
+        except KeyError:
+            pass
+        else:
             REPLACE_DIMS[dim][f"{code.id.title()}$"] = label
```

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/testing/__init__.py` & `message-ix-models-2024.4.2rc1/message_ix_models/testing/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 import logging
 import os
 from base64 import b32hexencode
-from contextlib import contextmanager
 from copy import deepcopy
 from pathlib import Path
 from random import randbytes
 from tempfile import TemporaryDirectory
 
-import click.testing
 import message_ix
 import pandas as pd
 import pytest
-from ixmp import Platform
 from ixmp import config as ixmp_config
 
-from message_ix_models import cli, util
-from message_ix_models.util._logging import mark_time, preserve_log_level
+from message_ix_models import util
+from message_ix_models.util._logging import mark_time
 from message_ix_models.util.context import Context
 
 log = logging.getLogger(__name__)
 
 # pytest hooks
 
 
@@ -44,25 +41,14 @@
         "--jvmargs",
         action="store",
         default="",
         help="Arguments for Java VM used by ixmp JDBCBackend",
     )
 
 
-def pytest_sessionstart():
-    # Quiet logs for some upstream packages
-    for name in (
-        "graphviz._tools",
-        "pycountry.db",
-        "matplotlib.backends",
-        "matplotlib.font_manager",
-    ):
-        logging.getLogger(name).setLevel(logging.DEBUG + 1)
-
-
 # Fixtures
 
 
 @pytest.fixture(scope="session")
 def session_context(pytestconfig, tmp_env):
     """A :class:`.Context` connected to a temporary, in-memory database.
 
@@ -78,24 +64,26 @@
       - If given: the :file:`/cache/` directory under the user's "message local data"
         directory.
 
     - the "message local data" config key to a temporary directory :file:`/data/` under
       the :ref:`pytest tmp_path directory <pytest:tmp_path>`.
 
     """
+    from platformdirs import user_cache_path
+
     ctx = Context.only()
 
     # Temporary, empty local directory for local data
     session_tmp_dir = Path(pytestconfig._tmp_path_factory.mktemp("data"))
 
     # Set the cache path according to whether pytest --local-cache was given. If True,
     # pick up the existing setting from the user environment. If False, use a pytest-
     # managed cache directory that persists across test sessions.
     ctx.cache_path = (
-        ctx.local_data.joinpath("cache")
+        user_cache_path("message-ix-models", ensure_exists=True)
         if pytestconfig.option.local_cache
         # TODO use pytestconfig.cache.mkdir() when pytest >= 6.3 is available
         else Path(pytestconfig.cache.makedir("cache"))
     )
 
     # Other local data in the temporary directory for this session only
     ctx.local_data = session_tmp_dir
@@ -116,18 +104,15 @@
     ixmp_config.add_platform(
         platform_name,
         "jdbc",
         "hsqldb",
         url=f"jdbc:hsqldb:mem://{platform_name}",
         jvmargs=pytestconfig.option.jvmargs,
     )
-
-    # Launch Platform and connect to testdb (reconnect if closed)
-    mp = Platform(name=platform_name)
-    mp.open_db()
+    ixmp_config.save()
 
     ctx.platform_info["name"] = platform_name
 
     try:
         yield ctx
     finally:
         ctx.close_db()
@@ -153,92 +138,30 @@
 @pytest.fixture(scope="function")
 def user_context(request):  # pragma: no cover
     """Context which can access user's configuration, e.g. platform names."""
     # Disabled; this is bad practice
     raise NotImplementedError
 
 
-class CliRunner(click.testing.CliRunner):
-    """Subclass of :class:`click.testing.CliRunner` with extra features."""
-
-    # NB decorator ensures any changes that the CLI makes to the logger level are
-    #    restored
-    @preserve_log_level()
-    def invoke(self, *args, **kwargs):
-        """Invoke the :program:`mix-models` CLI."""
-        result = super().invoke(cli.main, *args, **kwargs)
-
-        # Store the result to be used by assert_exit_0()
-        self.last_result = result
-
-        return result
-
-    def assert_exit_0(self, *args, **kwargs):
-        """Assert a result has exit_code 0, or print its traceback.
-
-        If any `args` or `kwargs` are given, :meth:`.invoke` is first called. Otherwise,
-        the result from the last call of :meth:`.invoke` is used.
-
-        Raises
-        ------
-        AssertionError
-            if the result exit code is not 0. The exception contains the traceback from
-            within the CLI.
-
-        Returns
-        -------
-        click.testing.Result
-        """
-        __tracebackhide__ = True
-
-        if len(args) + len(kwargs):
-            self.invoke(*args, **kwargs)
-
-        # Retrieve the last result
-        result = self.last_result
-
-        if result.exit_code != 0:
-            print(f"{result.exit_code = }\nresult.output =\n{result.output}")
-            # Re-raise the exception triggered within the CLI invocation
-            raise (result.exc_info[1].__context__ or result.exc_info[1]) from None
-
-        return result
-
-    @property
-    def add_command(self):
-        return cli_test_group.add_command
-
-    @contextmanager
-    def temporary_command(self, func: "click.Command", set_target: bool = True):
-        """Temporarily attach command `func` to :func:`cli_test_group`."""
-        assert func.name is not None
-        try:
-            cli_test_group.add_command(func)
-            yield
-        finally:
-            cli_test_group.commands.pop(func.name)
-
-
 @pytest.fixture
-def mix_models_cli(request, test_context, tmp_env):
-    """A :class:`.CliRunner` object that invokes the :program:`mix-models` CLI."""
-    # Require the `test_context` fixture in order to (a) set Context.local_data and (b)
-    # ensure changes to the Context from tested CLI commands are isolated from other
-    # tests
-    yield CliRunner(env=tmp_env)
+def mix_models_cli(session_context, tmp_env):
+    """A :class:`.CliRunner` object that invokes the :program:`mix-models` CLI.
 
+    NB this requires:
 
-@cli.main.group("_test", hidden=True)
-def cli_test_group():
-    """Hidden group of CLI commands.
-
-    Other code which needs to test CLI behaviour **may** attach temporary/throw-away
-    commands to this group and then invoke them using :func:`mix_models_cli`. This
-    avoids the need to expose additional commands for testing purposes only.
+    - The :mod:`ixmp` :func:`.tmp_env` fixture. This sets ``IXMP_DATA`` to a temporary
+      directory managed by :mod:`pytest`.
+    - The :func:`session_context` fixture. This (a) sets :attr:`.Config.local_data` to
+      a temporary directory within ``IXMP_DATA`` and (b) ensures changes to
+      :class:`.Context` made by invoked commands do not reach other tests.
     """
+    from message_ix_models import cli
+    from message_ix_models.util.click import CliRunner
+
+    yield CliRunner(cli.main, cli.__name__, env=tmp_env)
 
 
 # Testing utility functions
 
 
 def bare_res(request, context: Context, solved: bool = False) -> message_ix.Scenario:
     """Return or create a |Scenario| containing the bare RES, for use in testing.
```

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/testing/cli.py` & `message-ix-models-2024.4.2rc1/message_ix_models/testing/cli.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/tests/model/test_bare.py` & `message-ix-models-2024.4.2rc1/message_ix_models/tests/model/test_bare.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/tests/model/test_build.py` & `message-ix-models-2024.4.2rc1/message_ix_models/tests/model/test_build.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/tests/model/test_config.py` & `message-ix-models-2024.4.2rc1/message_ix_models/tests/model/test_config.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/tests/model/test_disutility.py` & `message-ix-models-2024.4.2rc1/message_ix_models/tests/model/test_disutility.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests of :mod:`.model.disutility`."""
+
 from itertools import product
 
 import pandas as pd
 import pandas.testing as pdt
 import pytest
 from message_ix import make_df
 from sdmx.model.v21 import Annotation, Code
```

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/tests/model/test_emissions.py` & `message-ix-models-2024.4.2rc1/message_ix_models/tests/model/test_emissions.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/tests/model/test_macro.py` & `message-ix-models-2024.4.2rc1/message_ix_models/tests/model/test_macro.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/tests/model/test_snapshot.py` & `message-ix-models-2024.4.2rc1/message_ix_models/tests/model/test_snapshot.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/tests/model/test_structure.py` & `message-ix-models-2024.4.2rc1/message_ix_models/tests/model/test_structure.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     codelists,
     generate_set_elements,
     get_codes,
     get_region_codes,
     process_commodity_codes,
     process_units_anno,
 )
-from message_ix_models.util import as_codes, eval_anno
+from message_ix_models.util import as_codes
 
 
 @pytest.mark.parametrize(
     "kind, exp",
     [
         (
             "node",
@@ -93,25 +93,26 @@
         data = get_codes("commodity")
 
         # Some expected commodities are present
         for check in "coal", "electr":
             assert check in data
 
         # Units for one commodity can be retrieved and parsed
+        g = dict(registry=registry)
         coal = data[data.index("coal")]
-        assert isinstance(eval_anno(coal, "units"), registry.Unit)
+        assert isinstance(coal.eval_annotation("units", globals=g), registry.Unit)
 
         # Descriptions are parsed without new lines
         crudeoil = data[data.index("crudeoil")]
         assert "\n" not in str(crudeoil.description)
 
         # Processing a second time does not double-wrap the unit expressions
         process_commodity_codes(data)
         coal = data[data.index("coal")]
-        assert isinstance(eval_anno(coal, "units"), registry.Unit)
+        assert isinstance(coal.eval_annotation("units", globals=g), registry.Unit)
 
     def test_levels(self):
         data = get_codes("level")
 
         # Some expected commodities are present
         for check in "primary", "useful":
             assert check in data
@@ -273,8 +274,10 @@
 def test_process_units_anno():
     # Prepare 2 codes: the parent has a units annotation, the child has none
     codes = as_codes({"foo": {"units": "kg"}, "bar": {"parent": "foo"}})
 
     process_units_anno("", codes[0])
 
     # Parents' units are propagated to the child
-    assert registry.Unit("kg") == eval_anno(codes[1], "units")
+    assert registry.Unit("kg") == codes[1].eval_annotation(
+        "units", dict(registry=registry)
+    )
```

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/tests/project/test_advance.py` & `message-ix-models-2024.4.2rc1/message_ix_models/tests/project/test_advance.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/tests/project/test_ssp.py` & `message-ix-models-2024.4.2rc1/message_ix_models/tests/project/test_ssp.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/tests/report/test_compat.py` & `message-ix-models-2024.4.2rc1/message_ix_models/tests/report/test_compat.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/tests/report/test_config.py` & `message-ix-models-2024.4.2rc1/message_ix_models/tests/report/test_config.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/tests/report/test_operator.py` & `message-ix-models-2024.4.2rc1/message_ix_models/tests/report/test_operator.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/tests/test_cli.py` & `message-ix-models-2024.4.2rc1/message_ix_models/tests/test_cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Basic tests of the command line."""
+
 import ixmp
 import pytest
 from message_ix.testing import make_dantzig
 
 from message_ix_models import util
 
 COMMANDS = [
```

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/tests/test_import.py` & `message-ix-models-2024.4.2rc1/message_ix_models/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/tests/test_report.py` & `message-ix-models-2024.4.2rc1/message_ix_models/tests/test_report.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests for :mod:`message_ix_models.report`."""
+
 from importlib.metadata import version
 
 import numpy as np
 import pandas as pd
 import pandas.testing as pdt
 import pytest
 from ixmp.testing import assert_logs
```

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/tests/test_util.py` & `message-ix-models-2024.4.2rc1/message_ix_models/tests/test_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests of :mod:`message_ix_models.util`."""
+
 import logging
 import re
 from importlib.metadata import version
 from pathlib import Path
 
 import numpy as np
 import pandas as pd
@@ -152,18 +153,19 @@
 
     exp = series_of_pint_quantity(
         [registry("4.9895 kg"), registry("46.2664 kg"), registry("454.9531 kg")],
     )
 
     # With store="quantity", a series of pint.Quantity is returned
     result = convert_units(*args, store="quantity")
-    assert all(
-        np.isclose(a, b, atol=1e-4 * registry.kg)
-        for a, b in zip(exp.values, result.values)
-    )
+    # Will raise a DimensionalityError if units are not equal
+    ratios = [(a / b) for a, b in zip(exp.values, result.values)]
+    # Assert equal units and sufficiently close values
+    for ratio in ratios:
+        assert ratio.dimensionless and np.isclose(ratio, 1, atol=1e-4)
 
     # With store="magnitude", a series of floats
     exp = pd.Series([q.magnitude for q in exp.values], name="bar")
     assert_series_equal(exp, convert_units(*args, store="magnitude"), check_dtype=False)
 
     # Other values for store= are errors
     with pytest.raises(ValueError, match="store = 'foo'"):
```

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/tests/test_workflow.py` & `message-ix-models-2024.4.2rc1/message_ix_models/tests/test_workflow.py`

 * *Files 8% similar despite different names*

```diff
@@ -87,42 +87,44 @@
     return wf
 
 
 @MARK
 def test_make_click_command(mix_models_cli) -> None:
     import click
 
+    from message_ix_models.cli import cli_test_group
+    from message_ix_models.util.click import temporary_command
+
     # make_click_command() runs and generates a command
     name = "make-click-command"
     cmd = make_click_command(f"{__name__}._wf", name=name, slug="test")
     assert isinstance(cmd, click.Command)
 
     # Add this into the hidden CLI test group
-    mix_models_cli.add_command(cmd)
-
-    # Invoke the command with various parameters
-    for params, output in (
-        (["--go", "B"], "nothing returned, workflow will continue with"),
-        (["B"], "Workflow diagram written to"),
-    ):
-        # Command runs and exits with 0
-        result = mix_models_cli.assert_exit_0(["_test", "run"] + params)
-        # Expected log messages or output were printed
-        assert output in result.output
-
-    # Invalid usage
-    for params, output in (
-        (["--go", "C"], "Error: No step(s) matched"),
-        (["--go"], "Error: No target step provided and no default for"),
-        # Step changes_b() fails if changes_a() is not first run
-        (["--go", "--from=[AX]", "B"], "Execute <function changes_b"),
-    ):
-        result = mix_models_cli.invoke(["_test", "run"] + params)
-        assert 0 != result.exit_code
-        assert output in result.output
+    with temporary_command(cli_test_group, cmd):
+        # Invoke the command with various parameters
+        for params, output in (
+            (["--go", "B"], "nothing returned, workflow will continue with"),
+            (["B"], "Workflow diagram written to"),
+        ):
+            # Command runs and exits with 0
+            result = mix_models_cli.assert_exit_0(["_test", "run"] + params)
+            # Expected log messages or output were printed
+            assert output in result.output
+
+        # Invalid usage
+        for params, output in (
+            (["--go", "C"], "Error: No step(s) matched"),
+            (["--go"], "Error: No target step provided and no default for"),
+            # Step changes_b() fails if changes_a() is not first run
+            (["--go", "--from=[AX]", "B"], "Execute <function changes_b"),
+        ):
+            result = mix_models_cli.invoke(["_test", "run"] + params)
+            assert 0 != result.exit_code
+            assert output in result.output
 
 
 @MARK
 def test_workflow(caplog, request, test_context, wf) -> None:
     # Retrieve some information from the fixture
     mp = wf.graph.pop("_base_platform")
 
@@ -142,15 +144,17 @@
     assert "test_tech" in set(s.set("technology"))
     assert 1 == len(s.par("technical_lifetime"))
     # Scenario was solved
     assert s.has_solution()
 
     # Log messages reflect workflow steps executed
     start_index = 1 if caplog.messages[0].startswith("Cull") else 0
-    m = "MESSAGEix-GLOBIOM R14 YB"
+    # This setting obtains the value R11 on some Windows GHA jobs, but is otherwise R14.
+    # TODO Debug and fix.
+    m = f"MESSAGEix-GLOBIOM {test_context.model.regions} YB"
     messages = [
         f"Loaded ixmp://{mp}/{m}/test_workflow#1",
         f"Step runs on ixmp://{mp}/{m}/test_workflow#1",
         "Execute <function changes_a at [^>]*>",
         f"…nothing returned, workflow will continue with {m}/test_workflow#1",
         f"Step runs on ixmp://{mp}/{m}/test_workflow#1",
         "Execute <function changes_b at [^>]*>",
@@ -160,36 +164,36 @@
         "Clone to foo/bar",
         "Execute <function solve at [^>]*>",
     ]
     for expr, message in zip(messages, caplog.messages[start_index:]):
         assert re.match(expr, message)
 
     assert re.match(
-        r"""'B':
+        rf"""'B':
 - <Step changes_b\(\)>
 - 'context':
   - <Context object at \w+ with \d+ keys>
 - 'A':
   - <Step changes_a\(\)>
   - 'context' \(above\)
   - 'base':
-    - <Step load -> MESSAGEix-GLOBIOM R14 YB/test_workflow>
+    - <Step load -> {m}/test_workflow>
     - 'context' \(above\)
     - None""",
         wf.describe("B"),
     )
 
     # Now truncate the workflow at "Model/A"
     wf.truncate("A")
 
     # Description reflects that changes_a() will no longer be called
     assert re.match(
-        r"""'B':
+        rf"""'B':
 - <Step changes_b\(\)>
 - 'context':
   - <Context object at \w+ with \d+ keys>
 - 'A':
-  - <Step load -> MESSAGEix-GLOBIOM R14 YB/test_workflow>
+  - <Step load -> {m}/test_workflow>
   - 'context' \(above\)
   - None""",
         wf.describe("B"),
     )
```

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/tests/tools/iea/test_web.py` & `message-ix-models-2024.4.2rc1/message_ix_models/tests/tools/iea/test_web.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import pandas as pd
 import pytest
 from genno import Computer
 
 from message_ix_models.testing import GHA
 from message_ix_models.tools.exo_data import prepare_computer
 from message_ix_models.tools.iea.web import DIMS, generate_code_lists, load_data
+from message_ix_models.util import HAS_MESSAGE_DATA
 
 
 class TestIEA_EWEB:
     @pytest.mark.parametrize("source", ("IEA_EWEB",))
     @pytest.mark.parametrize(
         "source_kw",
         (
@@ -64,15 +65,17 @@
 
 # NB once there is a fuzzed version of the (IEA, 2023) data available, usage of this
 #    variable can be replaced with list(FILES.keys())
 PROVIDER_EDITION = (
     pytest.param(
         "IEA",
         "2023",
-        marks=pytest.mark.xfail(GHA, reason="No fuzzed version of this data"),
+        marks=pytest.mark.xfail(
+            GHA or not HAS_MESSAGE_DATA, reason="No fuzzed version of this data"
+        ),
     ),
     ("OECD", "2023"),
     ("OECD", "2022"),
     ("OECD", "2023"),
 )
```

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/tests/tools/test_advance.py` & `message-ix-models-2024.4.2rc1/message_ix_models/tests/tools/test_advance.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/tests/tools/test_exo_data.py` & `message-ix-models-2024.4.2rc1/message_ix_models/tests/tools/test_exo_data.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/tests/tools/test_iamc.py` & `message-ix-models-2024.4.2rc1/message_ix_models/tests/tools/test_iamc.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/tests/tools/test_wb.py` & `message-ix-models-2024.4.2rc1/message_ix_models/tests/tools/test_wb.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/tests/util/test_cache.py` & `message-ix-models-2024.4.2rc1/message_ix_models/tests/util/test_cache.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/tests/util/test_click.py` & `message-ix-models-2024.4.2rc1/message_ix_models/tests/util/test_click.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """Basic tests of the command line."""
+
 import click
 
-from message_ix_models.util.click import common_params
+from message_ix_models.cli import cli_test_group
+from message_ix_models.util.click import common_params, temporary_command
 
 
 def test_default_path_cb(session_context, mix_models_cli):
     """Test :func:`.default_path_cb`."""
 
     # Create a hidden command and attach it to the CLI
     @click.command("default_path_cb")
@@ -18,15 +20,15 @@
     # option is *not* given
     cmd = [f"--local-data={session_context.local_data}", "_test", func.name]
 
     # …so default_path_cb() should supply "{local_data}/reporting_output".
     expected = session_context.local_data / "reporting_output"
 
     # Run the command
-    with mix_models_cli.temporary_command(func):
+    with temporary_command(cli_test_group, func):
         result = mix_models_cli.assert_exit_0(cmd)
 
     # The value was stored on, and retrieved from, `ctx`
     assert result.output.startswith(f"{expected}\n")
 
 
 def test_regions(mix_models_cli):
@@ -44,15 +46,15 @@
     @outer.command()
     @common_params("regions")
     @click.pass_obj
     def inner(context, regions):
         print(context.model.regions)
 
     # Give the option for the outer group, but not for the inner command
-    with mix_models_cli.temporary_command(outer):
+    with temporary_command(cli_test_group, outer):
         result = mix_models_cli.assert_exit_0(
             ["_test", "outer", "--regions=ZMB", "inner"]
         )
 
     # Value given to the outer group is stored and available to the inner command
     assert "ZMB" == result.output.strip()
 
@@ -64,15 +66,15 @@
     @click.command("store_context")
     @common_params("ssp")
     @click.pass_obj
     def func(ctx, ssp):
         print(ctx["ssp"])  # Print the value stored on the Context object
 
     # Run the command with a valid value
-    with mix_models_cli.temporary_command(func):
+    with temporary_command(cli_test_group, func):
         result = mix_models_cli.assert_exit_0(["_test", func.name, "SSP2"])
 
     # The value was stored on, and retrieved from, `ctx`
     assert "SSP2\n" == result.output
 
 
 def test_urls_from_file(mix_models_cli, tmp_path):
@@ -91,15 +93,15 @@
 foo/bar#5
 baz/qux#123
 """
     p = tmp_path.joinpath("scenarios.txt")
     p.write_text(text)
 
     # Run the command, referring to the temporary file
-    with mix_models_cli.temporary_command(func):
+    with temporary_command(cli_test_group, func):
         result = mix_models_cli.assert_exit_0(
             ["_test", func.name, f"--urls-from-file={p}"]
         )
 
     # Scenario URLs are parsed to ScenarioInfo objects, and then can be reconstructed →
     # data is round-tripped
     assert text == result.output
```

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/tests/util/test_config.py` & `message-ix-models-2024.4.2rc1/message_ix_models/tests/util/test_config.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/tests/util/test_context.py` & `message-ix-models-2024.4.2rc1/message_ix_models/tests/util/test_context.py`

 * *Files 4% similar despite different names*

```diff
@@ -153,34 +153,36 @@
             dict(model="foo", scenario="bar", version=0) == test_context.scenario_info
         )
 
     def test_write_debug_archive(self, mix_models_cli):
         """:meth:`.write_debug_archive` works."""
         # Create a CLI command attached to the hidden "_test" group
 
-        from message_ix_models.testing import cli_test_group
+        from message_ix_models.cli import cli_test_group
+        from message_ix_models.util.click import temporary_command
 
-        @cli_test_group.command("write-debug-archive")
+        @click.command("write-debug-archive")
         @click.pass_obj
-        def _(context):
+        def command(context):
             # Register one file to be archived
             p = context.core.local_data.joinpath("foo.txt")
             context.core.debug_paths.append(p)
 
             # Write some text to this file
             p.write_text("Here is some debug output in a file.")
 
             # Register a non-existent path
             context.core.debug_paths.append(p.with_name("bar.txt"))
 
             # Write the archive
             context.write_debug_archive()
 
         # Invoke the command; I/O occurs in a temporary directory
-        result = mix_models_cli.invoke(["_test", "write-debug-archive"])
+        with temporary_command(cli_test_group, command):
+            result = mix_models_cli.invoke(["_test", "write-debug-archive"])
 
         # Output path is constructed as expected; file exists
         match = re.search(
             r"Write to: (.*main-_test-write-debug-archive-[\dabcdefT\-]+.zip)",
             result.output,
         )
         assert Path(match.group(1)).exists()
```

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/tests/util/test_node.py` & `message-ix-models-2024.4.2rc1/message_ix_models/tests/util/test_node.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests of :mod:`message_ix_models.util.node`."""
+
 import re
 
 import pandas as pd
 import pytest
 from genno import Quantity
 from message_ix import Scenario, make_df
```

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/tests/util/test_scenarioinfo.py` & `message-ix-models-2024.4.2rc1/message_ix_models/tests/util/test_scenarioinfo.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/tests/util/test_sdmx.py` & `message-ix-models-2024.4.2rc1/message_ix_models/tests/util/test_sdmx.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,31 +3,35 @@
 
 import pytest
 from sdmx.model.v21 import Annotation, Code
 
 from message_ix_models.util.sdmx import eval_anno, make_enum, read
 
 
-def test_eval_anno(caplog):
+def test_eval_anno(caplog, recwarn):
     c = Code()
 
-    assert None is eval_anno(c, "foo")
+    with pytest.warns(DeprecationWarning):
+        assert None is eval_anno(c, "foo")
 
     c.annotations.append(Annotation(id="foo", text="bar baz"))
 
-    with caplog.at_level(logging.DEBUG, logger="message_ix_models"):
+    with caplog.at_level(logging.DEBUG, logger="message_ix_models"), pytest.warns(
+        DeprecationWarning
+    ):
         assert "bar baz" == eval_anno(c, "foo")
 
     assert re.fullmatch(
         r"Could not eval\('bar baz'\): .* \(<string>, line 1\)", caplog.messages[0]
     )
 
     c.annotations.append(Annotation(id="qux", text="3 + 4"))
 
-    assert 7 == eval_anno(c, id="qux")
+    with pytest.warns(DeprecationWarning):
+        assert 7 == eval_anno(c, id="qux")
 
 
 def test_make_enum():
     """:func:`.make_enum` works with :class:`~enum.Flag` and subclasses."""
     from enum import Flag, IntFlag
 
     E = make_enum("ICONICS:SSP(2017)", base=Flag)
```

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/tools/advance.py` & `message-ix-models-2024.4.2rc1/message_ix_models/tools/advance.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Handle data from the ADVANCE project."""
+
 import logging
 from pathlib import Path
 from typing import Optional
 from zipfile import ZipFile
 
 import pandas as pd
 import pint
```

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/tools/exo_data.py` & `message-ix-models-2024.4.2rc1/message_ix_models/tools/exo_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """Generic tools for working with exogenous data sources."""
+
 import logging
 from abc import ABC, abstractmethod
+from copy import deepcopy
 from operator import itemgetter
 from pathlib import Path
 from typing import Any, Dict, Literal, Mapping, Optional, Tuple, Type
 
 from genno import Computer, Key, Quantity, quote
 
 from message_ix_models import ScenarioInfo
@@ -107,14 +109,23 @@
         # Interpolate to the desired set of periods
         kw = dict(fill_value="extrapolate")
         k2 = base_key + "2"
         c.add(k2, "interpolate", base_key + "1", "y::coords", kwargs=kw)
 
         return k2
 
+    def raise_on_extra_kw(self, kwargs) -> None:
+        """Helper for subclasses."""
+        if len(kwargs):
+            log.error(
+                f"Unhandled extra keyword arguments for {type(self).__name__}: "
+                + repr(kwargs)
+            )
+            raise ValueError(kwargs)
+
 
 def prepare_computer(
     context,
     c: "Computer",
     source="test",
     source_kw: Optional[Mapping] = None,
     *,
@@ -159,15 +170,15 @@
         measure = "UNKNOWN"
 
     # Look up input data flow
     source_obj = None
     for cls in SOURCES.values():
         try:
             # Instantiate a Source object to provide this data
-            source_obj = cls(source, source_kw or dict())
+            source_obj = cls(source, deepcopy(source_kw or dict()))
         except Exception:
             pass  # Class does not recognize the arguments
 
     if source_obj is None:
         raise ValueError(f"No source found that can handle {source!r}")
 
     # Add structural information to the Computer
```

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/tools/iamc.py` & `message-ix-models-2024.4.2rc1/message_ix_models/tools/iamc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tools for working with IAMC-structured data."""
+
 from typing import Optional
 
 import pandas as pd
 import sdmx.model.v21 as m
 from sdmx.message import StructureMessage
```

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/tools/iea/web.py` & `message-ix-models-2024.4.2rc1/message_ix_models/tools/iea/web.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tools for IEA (Extended) World Energy Balance (WEB) data."""
+
 import logging
 import zipfile
 from copy import copy
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Dict, Iterable, Optional
 
 import dask.dataframe as dd
```

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/tools/wb.py` & `message-ix-models-2024.4.2rc1/message_ix_models/tools/wb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 """Tools for World Bank data."""
+
 import logging
 from collections import defaultdict
 from functools import lru_cache
 from typing import TYPE_CHECKING, Dict, MutableMapping, Optional
 
 import pandas as pd
 
 if TYPE_CHECKING:
     import sdmx.model.common
 
 log = logging.getLogger(__name__)
 
 
-def assign_income_groups(
+# FIXME Reduce complexity from 12 → ≤11
+def assign_income_groups(  # noqa: C901
     cl_node: "sdmx.model.common.Codelist",
     cl_income_group: "sdmx.model.common.Codelist",
     method: str = "population",
     replace: Optional[Dict[str, str]] = None,
 ) -> None:
     """Annotate `cl_node` with income groups.
 
@@ -63,15 +65,15 @@
         def get_weight(code: "sdmx.model.common.Code") -> float:
             """Weight of the country `code` in aggregation."""
             return 1.0
 
     elif method == "population":
         # Retrieve WB_WDI data for SERIES=SP_POP_TOTAL (Population, total)
         dm = sdmx.Client("WB_WDI").data(
-            "WDI", key="A.SP_POP_TOTL.", params=dict(startperiod=2020, endperiod=2020)
+            "WDI", key="A.SP_POP_TOTL.", params=dict(start_period=2020, end_period=2020)
         )
 
         # Convert to pd.Series with multi-index with levels: REF_AREA, SERIES, FREQ,
         # TIME_PERIOD. Because of the query, there is only 1 value for each unique
         # REF_AREA.
         df = sdmx.to_pandas(dm.data[0])
```

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/util/__init__.py` & `message-ix-models-2024.4.2rc1/message_ix_models/util/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 from collections import ChainMap, defaultdict
+from datetime import datetime
 from functools import partial, update_wrapper
 from importlib.metadata import version
 from itertools import count
 from typing import (
     TYPE_CHECKING,
     Callable,
     Collection,
@@ -17,14 +18,15 @@
 )
 
 import message_ix
 import pandas as pd
 import pint
 
 from ._convert_units import convert_units, series_of_pint_quantity
+from ._logging import mark_time, preserve_log_level, silence_log
 from .cache import cached
 from .common import (
     HAS_MESSAGE_DATA,
     MESSAGE_DATA_PATH,
     MESSAGE_MODELS_PATH,
     Adapter,
     MappingAdapter,
@@ -53,33 +55,38 @@
     "aggregate_codes",
     "as_codes",
     "broadcast",
     "cached",
     "check_support",
     "convert_units",
     "copy_column",
+    "datetime_now_with_tz",
     "eval_anno",
     "ffill",
     "identify_nodes",
     "iter_keys",
     "load_package_data",
     "load_private_data",
     "local_data_path",
     "make_io",
     "make_matched_dfs",
     "make_source_tech",
+    "mark_time",
     "maybe_query",
     "merge_data",
     "minimum_version",
     "package_data_path",
+    "preserve_log_level",
     "private_data_path",
     "replace_par_data",
     "same_node",
     "same_time",
     "series_of_pint_quantity",
+    "show_versions",
+    "silence_log",
     "strip_par_data",
 ]
 
 log = logging.getLogger(__name__)
 
 
 def add_par_data(
@@ -205,15 +212,17 @@
     # Broadcast using matched labels for 1+ dimensions from a data frame
     if labels is not None:
         # Check the dimensions
         for dim in labels.columns:
             _check_dim(dim)
         # Concatenate 1 copy of `df` for each row in `labels`
         df = pd.concat(
-            [df.assign(**row) for _, row in labels.iterrows()], ignore_index=True
+            [df.assign(**row) for _, row in labels.iterrows()],
+            ignore_index=True,
+            sort=False,
         )
 
     # Next, broadcast other dimensions given as keyword arguments
     for dim, levels in kwargs.items():
         _check_dim(dim)
         if len(levels) == 0:
             log.debug(
@@ -222,15 +231,15 @@
             continue
 
         # - Duplicate the data
         # - Drop the existing column named 'dim'
         # - Re-add the column from the constructed MultiIndex
         # - Reindex for sequential row numbers
         df = (
-            pd.concat([df] * len(levels), keys=levels, names=[dim])
+            pd.concat([df] * len(levels), keys=levels, names=[dim], sort=False)
             .drop(dim, axis=1)
             .reset_index(dim)
             .reset_index(drop=True)
         )
     return df
 
 
@@ -274,14 +283,20 @@
 
     :func:`copy_column` is useful in the context of more complicated calls to
     :meth:`~pandas.DataFrame.assign`.
     """
     return lambda df: df[column_name]
 
 
+def datetime_now_with_tz() -> datetime:
+    """Current date and time with time zone information."""
+    tz = datetime.now().astimezone().tzinfo
+    return datetime.now(tz)
+
+
 def ffill(
     df: pd.DataFrame, dim: str, values: Sequence[CodeLike], expr: Optional[str] = None
 ) -> pd.DataFrame:
     """Forward-fill `df` on `dim` to cover `values`.
 
     Parameters
     ----------
@@ -317,16 +332,15 @@
             # Duplicate the data; assign the new_label to `dim`
             dfs.append(group_df.assign(**{dim: new_label}).pipe(_maybe_eval))
 
     return pd.concat(dfs, ignore_index=True)
 
 
 class KeyIterator(Protocol):
-    def __call__(self) -> "genno.Key":
-        ...
+    def __call__(self) -> "genno.Key": ...
 
 
 def iter_keys(base: "genno.Key") -> KeyIterator:
     """Return an iterator over a sequence of keys starting with `base_key`.
 
     This can be used for shorthand when constructing sequences of :mod:`genno`
     computations.
@@ -660,14 +674,32 @@
 
 def same_time(df: pd.DataFrame) -> pd.DataFrame:
     """Fill 'time_origin'/'time_dest' in `df` from 'time'."""
     cols = list(set(df.columns) & {"time_origin", "time_dest"})
     return df.assign(**{c: copy_column("time") for c in cols})
 
 
+def show_versions() -> str:
+    """Output of :func:`ixmp.show_versions`, as a :class:`str`."""
+    from io import StringIO
+
+    from . import ixmp
+    from ._logging import preserve_log_handlers
+
+    # Retrieve package versions
+    buf = StringIO()
+
+    # show_versions() imports pyam-iamc, which in turn imports ixmp4, which removes all
+    # handlers from the root logger (?!). Preserve the message-ix-models logging config.
+    with preserve_log_handlers():
+        ixmp.show_versions(buf)
+
+    return buf.getvalue()
+
+
 # FIXME Reduce complexity from 14 to ≤13
 def strip_par_data(  # noqa: C901
     scenario: message_ix.Scenario,
     set_name: str,
     element: str,
     dry_run: bool = False,
     dump: Optional[Dict[str, pd.DataFrame]] = None,
```

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/util/_convert_units.py` & `message-ix-models-2024.4.2rc1/message_ix_models/util/_convert_units.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/util/cache.py` & `message-ix-models-2024.4.2rc1/message_ix_models/util/cache.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 """Cache data for expensive operations.
 
 This module extends :class:`genno.caching.Encoder` to handle classes common in
 :mod:`message_ix_models`, so these can be used as arguments to cached functions and
 included in the computed cache key:
 
-- :class:`sdmx.model.IdentifiableArtefact`, including :class:`.Code`: hashed as
-  their string representation / ID.
+- :class:`sdmx.model.IdentifiableArtefact`, including :class:`.Code`: hashed as their
+  string representation / ID.
 - :class:`ixmp.Platform`, :class:`xarray.Dataset`: ignored, with a warning logged.
 - :class:`ScenarioInfo`: only the :attr:`~ScenarioInfo.set` entries are hashed.
-
 """
+
 import json
 import logging
 from dataclasses import asdict, is_dataclass
-from typing import Callable
+from typing import TYPE_CHECKING, Callable, Set
 
 import genno.caching
 import ixmp
 import sdmx.model
 import xarray as xr
 
 from .context import Context
 from .scenarioinfo import ScenarioInfo
 
+if TYPE_CHECKING:
+    from pathlib import Path
+
 log = logging.getLogger(__name__)
 
 
 #: Controls whether cached data is returned for functions decorated with
 #: :func:`.cached`. Set to :obj:`True` to force reload.
 SKIP_CACHE = False
 
 # Paths already logged, to decrease verbosity
-PATHS_SEEN = set()
+PATHS_SEEN: Set["Path"] = set()
 
 
 # Show genno how to hash function arguments seen in message_ix_models
 
 
 @genno.caching.Encoder.register
 def _sdmx_identifiable(o: sdmx.model.IdentifiableArtefact):
@@ -69,20 +72,20 @@
     When :data:`.SKIP_CACHE` is true, `func` is always called.
 
     See also
     --------
     :doc:`genno:cache` in the :mod:`genno` documentation
     """
     # Determine and create the cache path
-    cache_path = Context.get_instance(-1).get_cache_path()
-    cache_path.mkdir(exist_ok=True, parents=True)
+    cache_path = Context.get_instance(-1).core.cache_path
 
     if cache_path not in PATHS_SEEN:
         log.debug(f"{func.__name__}() will cache in {cache_path}")
         PATHS_SEEN.add(cache_path)
+        cache_path.mkdir(parents=True, exist_ok=True)
 
     # Use the genno internals to wrap the function.
     cached_load = genno.caching.decorate(
         func, cache_path=cache_path, cache_skip=SKIP_CACHE
     )
 
     if cached_load.__doc__ is not None:
```

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/util/click.py` & `message-ix-models-2024.4.2rc1/message_ix_models/project/ssp/data.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,263 +1,221 @@
-"""Command-line utilities.
-
-These are used for building CLIs using :mod:`click`.
-"""
 import logging
-from datetime import datetime
-from pathlib import Path
-from typing import Callable, List, Optional, Union
-
-import click
-from click import Argument, Choice, Option
-
-from message_ix_models import Context, model
-from message_ix_models.model.structure import codelists
 
-from .scenarioinfo import ScenarioInfo
+from message_ix_models.tools.exo_data import (
+    ExoDataSource,
+    iamc_like_data_for_query,
+    register_source,
+)
+from message_ix_models.util import package_data_path, private_data_path
+
+__all__ = [
+    "SSPOriginal",
+    "SSPUpdate",
+]
 
 log = logging.getLogger(__name__)
 
 
-def common_params(param_names: str):
-    """Decorate a click.command with common parameters `param_names`.
-
-    `param_names` must be a space-separated string of names appearing in :data:`PARAMS`,
-    e.g. ``"ssp force output_model"``. The decorated function receives keyword
-    arguments with these names::
-
-        @click.command()
-        @common_params("ssp force output_model")
-        def mycmd(ssp, force, output_model)
-            # ...
-    """
-
-    # Simplified from click.decorators._param_memo
-    def decorator(f):
-        if not hasattr(f, "__click_params__"):
-            f.__click_params__ = []
-        f.__click_params__.extend(
-            PARAMS[name] for name in reversed(param_names.split())
-        )
-        return f
-
-    return decorator
-
+@register_source
+class SSPOriginal(ExoDataSource):
+    """Provider of exogenous data from the original SSP database.
+
+    To use data from this source, call :func:`.exo_data.prepare_computer` with the
+    arguments:
+
+    - `source`: Any value from :data:`.SSP_2017` or equivalent string, for instance
+      "ICONICS:SSP(2017).2". The specific SSP for which data is returned is determined
+      from the value.
+    - `source_kw` including:
+
+      - "model": one of:
+
+          - IIASA GDP
+          - IIASA-WiC POP
+          - NCAR
+          - OECD Env-Growth
+          - PIK GDP-32
 
-def default_path_cb(*default_parts):
-    """Return a callback function for click.Option handling.
-
-    If no option value is given, the callback uses :meth:`Context.get_local_path` and
-    `default_parts` to provide a path that is relative to local data directory, e.g.
-    the current working directory (see :doc:`/data`).
-    """
-
-    def _callback(context, param, value):
-        value = value or context.obj.get_local_path(*default_parts)
-        setattr(context.obj, param.name, value)
-        return value
-
-    return _callback
-
-
-def exec_cb(expression: str) -> Callable:
-    """Return a callback that :func:`exec`-utes an `expression`.
-
-    The `expression` is executed in a limited context that has only two names available:
-
-    - :py:`context`: the :class:`.Context` instance.
-    - :py:`value`: the value passed to the :mod:`click.Parameter`.
+      - "measure": The measures available differ according to the model; see the source
+        data for details.
 
     Example
     -------
-    >>> @click.command
-    ... @click.option(
-    ...     "--myopt", callback=exec_cb("context.my_mod.my_opt = value + 3")
+    >>> keys = prepare_computer(
+    ...     context,
+    ...     computer,
+    ...     source="ICONICS:SSP(2015).3",
+    ...     source_kw=dict(measure="POP", model="IIASA-WiC POP"),
     ... )
-    ... def cmd(...):
-    ...     ...
+    >>> result = computer.get(keys[0])
     """
 
-    def _cb(context: Union[click.Context, Context], param, value):
-        ctx = context.obj if isinstance(context, click.Context) else context
-        exec(expression, {}, {"context": ctx, "value": value})
-        return value
-
-    return _cb
+    id = "SSP"
 
+    #: Name of file containing the data.
+    filename = "SspDb_country_data_2013-06-12.csv.zip"
 
-def format_sys_argv() -> str:
-    """Format :data:`sys.argv` in a readable manner."""
-    import sys
-
-    lines = ["Invoked:"]
-    indent = ""
-    for item in sys.argv:
-        lines.append(f"{indent}{item} \\")
-        indent = "  "
-
-    return "\n".join(lines)[:-2]
-
+    #: One-to-one correspondence between "model" codes and date fragments in scenario
+    #: codes.
+    model_date = {
+        "IIASA GDP": "130219",
+        "IIASA-WiC POP": "130115",
+        "NCAR": "130115",
+        "OECD Env-Growth": "130325",
+        "PIK GDP-32": "130424",
+    }
+
+    #: Replacements to apply when loading the data.
+    replace = {"billion US$2005/yr": "billion USD_2005/yr"}
+
+    def __init__(self, source, source_kw):
+        s = "ICONICS:SSP(2017)."
+        if not source.startswith(s):
+            raise ValueError(source)
+
+        *parts, ssp_id = source.partition(s)
+
+        # Map the `measure` keyword to a string appearing in the data
+        measure = {
+            "GDP": "GDP|PPP",
+            "POP": "Population",
+        }[source_kw.pop("measure")]
+
+        # Store the model ID, if any
+        model = source_kw.pop("model", None)
+
+        # Determine the date based on the model ID. There is a 1:1 correspondence.
+        date = self.model_date[model]
+
+        self.raise_on_extra_kw(source_kw)
+
+        # Assemble a query string
+        extra = "d" if ssp_id == "4" and model == "IIASA-WiC POP" else ""
+        self.query = (
+            f"SCENARIO == 'SSP{ssp_id}{extra}_v9_{date}' and VARIABLE == '{measure}'"
+            + (f" and MODEL == '{model}'" if model else "")
+        )
+        # log.debug(query)
 
-def store_context(context: Union[click.Context, Context], param, value):
-    """Callback that simply stores a value on the :class:`.Context` object.
+        # Iterate over possible locations for the data file
+        dirs = [private_data_path("ssp"), package_data_path("test", "ssp")]
+        for path in [d.joinpath(self.filename) for d in dirs]:
+            if not path.exists():
+                log.info(f"Not found: {path}")
+                continue
+            if "test" in path.parts:
+                log.warning(f"Reading random data from {path}")
+            break
+
+        self.path = path
+
+    def __call__(self):
+        # Use prepared path, query, and replacements
+        return iamc_like_data_for_query(self.path, self.query, replace=self.replace)
+
+
+@register_source
+class SSPUpdate(ExoDataSource):
+    """Provider of exogenous data from the SSP Update database.
+
+    To use data from this source, call :func:`.exo_data.prepare_computer` with the
+    arguments:
+
+    - `source`: Any value from :data:`.SSP_2024` or equivalent string, for instance
+      "ICONICS:SSP(2024).2".
+    - `release`: One of "3.0" or "preview".
 
-    Use this for parameters that are not used directly in a @click.command() function,
-    but need to be carried by the Context for later use.
+    Example
+    -------
+    >>> keys = prepare_computer(
+    ...     context,
+    ...     computer,
+    ...     source="ICONICS:SSP(2024).3",
+    ...     source_kw=dict(measure="GDP", model="IIASA GDP 2023"),
+    ... )
+    >>> result = computer.get(keys[0])
     """
-    setattr(
-        context.obj if isinstance(context, click.Context) else context,
-        param.name,
-        value,
-    )
-    return value
-
-
-def urls_from_file(
-    context: Union[click.Context, Context], param, value
-) -> List[ScenarioInfo]:
-    """Callback to parse scenario URLs from `value`."""
-    si: List[ScenarioInfo] = []
 
-    if value is None:
-        return si
+    id = "SSP update"
 
-    with click.open_file(value) as f:
-        for line in f:
-            si.append(ScenarioInfo.from_url(url=line))
-
-    # Store on context
-    mm_context = context.obj if isinstance(context, click.Context) else context
-    mm_context.core.scenarios = si
-
-    return si
-
-
-def unique_id() -> str:
-    """Return a unique ID for a CLI invocation.
-
-    The return value resembles "mix-models-debug-3332d415ef65bf2a-2023-02-02T162931" and
-    contains:
-
-    - The CLI name and (sub)commands.
-    - A hash of all the CLI parameters (options and arguments).
-    - The current date and time, in ISO format with Windows-incompatible ":" removed.
-
-    """
-    click_context = click.get_current_context()
+    #: File names containing the data, according to the release.
+    filename = {
+        "3.0": "1706548837040-ssp_basic_drivers_release_3.0_full.csv.gz",
+        "preview": "SSP-Review-Phase-1.csv.gz",
+    }
+
+    def __init__(self, source, source_kw):
+        s = "ICONICS:SSP(2024)."
+        if not source.startswith(s):
+            raise ValueError(source)
+
+        *parts, ssp_id = source.partition(s)
+
+        # Map the `measure` keyword to a 'Variable' dimension code
+        measure = {
+            "GDP": "GDP|PPP",
+            "POP": "Population",
+        }[source_kw.pop("measure")]
+
+        # Store the model code, if any
+        model = source_kw.pop("model", None)
+
+        # Identify the data release date/version/label
+        release = source_kw.pop("release", "3.0")
+
+        self.raise_on_extra_kw(source_kw)
+
+        # Replacements to apply, if any
+        self.replace = {}
+
+        # Prepare query pieces
+        models = []
+        scenarios = []
+
+        if release == "3.0":
+            # Directories in which to locate `self.filename`; stored directly within
+            # message_ix_models
+            dirs = [package_data_path("ssp")]
+
+            scenarios.append(f"SSP{ssp_id}")
+
+            if measure == "GDP|PPP":
+                # Configure to prepend (m="OECD…", s="Historical Reference")
+                # observations to series
+                models.extend({model, "OECD ENV-Growth 2023"})
+                scenarios.append("Historical Reference")
+                self.replace.update(
+                    Model={"OECD ENV-Growth 2023": model},
+                    Scenario={"Historical Reference": scenarios[0]},
+                )
+        elif release == "preview":
+            # Look first in message_data, then in message_ix_models test data
+            dirs = [private_data_path("ssp"), package_data_path("test", "ssp")]
+
+            scenarios.append(f"SSP{ssp_id} - Review Phase 1")
+        else:
+            log.error(
+                f"{release = } invalid for {type(self)}; expected one of: "
+                f"{set(self.filename)}"
+            )
+            raise ValueError(release)
+
+        # Assemble and store a query string
+        self.query = f"Scenario in {scenarios!r} and Variable == '{measure}'" + (
+            f"and Model in {models!r}" if models else ""
+        )
+        # log.info(f"{self.query = }")
 
-    # Collapse CLI (sub)commands and their arguments to a hashable data structure
-    # This also includes CLI options *not* given
-    c: Optional[click.Context] = click_context
-    data = []
-    while c is not None:
-        data.append((c.command.name, tuple(sorted(c.params.items()))))
-        c = c.parent
-
-    # Assemble parts
-    return "-".join(
-        [
-            click_context.command_path.replace(" ", "-"),
-            f"{hash(tuple(reversed(data))):x}",
-            datetime.now().isoformat(timespec="seconds").replace(":", ""),
-        ]
-    )
-
-
-#: Common command-line parameters (arguments and options). See :func:`common_params`.
-PARAMS = {
-    "dest": Option(
-        ["--dest"],
-        callback=store_context,
-        expose_value=False,
-        help="Destination URL for created scenario(s).",
-    ),
-    "dry_run": Option(
-        ["--dry-run"],
-        is_flag=True,
-        callback=store_context,
-        expose_value=False,
-        help="Only show what would be done.",
-    ),
-    "force": Option(
-        ["--force"],
-        is_flag=True,
-        callback=store_context,
-        help="Overwrite or modify existing model/scenario.",
-    ),
-    "nodes": Option(
-        ["--nodes"],
-        help="Code list to use for 'node' dimension.",
-        callback=exec_cb("context.model.regions = value"),
-        type=Choice(codelists("node")),
-        default=model.Config.regions,
-        expose_value=False,
-    ),
-    "output_model": Option(
-        ["--output-model"], help="Model name under which scenarios should be generated."
-    ),
-    "policy_path": Option(
-        ["--policy-path"],
-        callback=default_path_cb("scenario_generation", "policies"),
-        help="Path to policy scripts.",
-    ),
-    "platform_dest": Option(["--platform-dest"], help="Name of destination Platform."),
-    "quiet": Option(
-        ["--quiet"],
-        is_flag=True,
-        expose_value=False,
-        help="Show less or no output.",
-    ),
-    "regions": Option(
-        ["--regions"],
-        help="Code list to use for 'node' dimension.",
-        callback=exec_cb("context.model.regions = value or context.model.regions"),
-        type=Choice(codelists("node")),
-    ),
-    "rep_out_path": Option(
-        ["--rep-out-path"],
-        callback=default_path_cb("reporting_output"),
-        help="Path for reporting output.",
-    ),
-    "rep_template": Option(
-        ["--rep-template"],
-        callback=default_path_cb(
-            "message_data", "tools", "post_processing", "MESSAGEix_WorkDB_Template.xlsx"
-        ),
-        help="Path incl. filename and extension to reporting template.",
-    ),
-    "run_reporting_only": Option(
-        ["--run-reporting-only"],
-        is_flag=True,
-        callback=store_context,
-        help="Run only reporting.",
-    ),
-    "ssp": Argument(
-        ["ssp"], callback=store_context, type=Choice(["SSP1", "SSP2", "SSP3"])
-    ),
-    "urls_from_file": Option(
-        ["--urls-from-file", "-f"],
-        type=click.Path(
-            exists=True,
-            dir_okay=False,
-            resolve_path=True,
-            allow_dash=True,
-            path_type=Path,
-        ),
-        callback=urls_from_file,
-    ),
-    "verbose": Option(
-        # NB cannot use store_callback here; this is processed in the top-level CLI
-        #    before the message_ix_models.Context() object is set up
-        ["--verbose", "-v"],
-        is_flag=True,
-        help="Print DEBUG-level log messages.",
-    ),
-    "years": Option(
-        ["--years"],
-        help="Code list to use for the 'year' dimension.",
-        callback=exec_cb("context.model.years = value"),
-        type=Choice(codelists("year")),
-        default=model.Config.years,
-        # expose_value=False,
-    ),
-}
+        # Iterate over possible locations for the data file
+        for path in [d.joinpath(self.filename[release]) for d in dirs]:
+            if not path.exists():
+                log.info(f"Not found: {path}")
+                continue
+            if "test" in path.parts:
+                log.warning(f"Reading random data from {path}")
+            break
+
+        self.path = path
+
+    def __call__(self):
+        # Use prepared path, query, and replacements
+        return iamc_like_data_for_query(self.path, self.query, replace=self.replace)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/util/common.py` & `message-ix-models-2024.4.2rc1/message_ix_models/util/common.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from genno.operator import concat
 
 log = logging.getLogger(__name__)
 
 try:
     import message_data
 except ImportError:
-    log.warning("message_data is not installed or cannot be imported")
     MESSAGE_DATA_PATH: Optional[Path] = None
     HAS_MESSAGE_DATA = False
 else:  # pragma: no cover  (needs message_data)
     # Root directory of the message_data repository.
     MESSAGE_DATA_PATH = Path(message_data.__file__).parents[1]
     HAS_MESSAGE_DATA = True
 
@@ -254,23 +253,34 @@
     See also
     --------
     :ref:`Choose locations for data <package-data>`
     """
     return _make_path(MESSAGE_MODELS_PATH / "data", *parts)
 
 
-def private_data_path(*parts) -> Path:  # pragma: no cover (needs message_data)
+def private_data_path(*parts) -> Path:
     """Construct a path to a file under :file:`data/` in :mod:`message_data`.
 
-    Use this function to access non-public (e.g. embargoed or proprietary) data stored
-    in the :mod:`message_data` repository.
+    Use this function to access non-public (for instance, embargoed or proprietary) data
+    stored in the :mod:`message_data` repository.
+
+    If the repository is not available, the function falls back to
+    :meth:`.Context.get_local_path`, where users may put files obtained through other
+    messages.
 
     Parameters
     ----------
     parts : sequence of str or Path
         Joined to the base path using :meth:`~pathlib.PurePath.joinpath`.
 
     See also
     --------
     :ref:`Choose locations for data <private-data>`
     """
-    return _make_path(cast(Path, MESSAGE_DATA_PATH) / "data", *parts)
+    if HAS_MESSAGE_DATA:
+        return _make_path(cast(Path, MESSAGE_DATA_PATH) / "data", *parts)
+    else:
+        from .context import Context
+
+        base = Context.get_instance(-1).get_local_path()
+        log.warning(f"message_data not installed; fall back to {base}")
+        return base.joinpath(*parts)
```

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/util/config.py` & `message-ix-models-2024.4.2rc1/message_ix_models/util/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 import ixmp
 
 from .scenarioinfo import ScenarioInfo
 
 log = logging.getLogger(__name__)
 
+ixmp.config.register("no message_data", bool, False)
 ixmp.config.register("message local data", Path, Path.cwd())
 
 
 def _local_data_factory():
     """Default values for :attr:`.Config.local_data."""
     return (
         Path(
@@ -161,21 +162,28 @@
     #: A scenario URL, e.g. as given by the :program:`--url` CLI option.
     url: Optional[str] = None
 
     #: Like :attr:`url`, used by e.g. :meth:`.clone_to_dest`.
     dest: Optional[str] = None
 
     #: Base path for cached data, e.g. as given by the :program:`--cache-path` CLI
-    #: option. Default: :file:`{local_data}/cache/`.
+    #: option. Default: the directory :file:`message-ix-models` within the directory
+    #: given by :func:`.platformdirs.user_cache_path`.
     cache_path: Optional[str] = None
 
     #: Paths of files containing debug outputs. See :meth:`Context.write_debug_archive`.
     debug_paths: Sequence[str] = field(default_factory=list)
 
     #: Whether an operation should be carried out, or only previewed. Different modules
     #: will respect :attr:`dry_run` in distinct ways, if at all, and **should** document
     #: behaviour.
     dry_run: bool = False
 
     #: Flag for causing verbose output to logs or stdout. Different modules will respect
     #: :attr:`verbose` in distinct ways.
     verbose: bool = False
+
+    def __post_init__(self):
+        if self.cache_path is None:
+            from platformdirs import user_cache_path
+
+            self.cache_path = user_cache_path("message-ix-models", ensure_exists=True)
```

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/util/context.py` & `message-ix-models-2024.4.2rc1/message_ix_models/util/context.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 """Context and settings for :mod:`message_ix_models` code."""
+
 import logging
 from copy import deepcopy
 from dataclasses import fields
 from pathlib import Path
 from typing import List
 
 import ixmp
 import message_ix
 from click import BadOptionUsage
 
 from .config import Config
+from .ixmp import parse_url
 
 log = logging.getLogger(__name__)
 
 #: List of Context instances, from first created to last.
 _CONTEXTS: List["Context"] = []
 
 
@@ -133,14 +135,20 @@
         if mp is not None:
             self._mp = mp
 
         _CONTEXTS.append(result)
 
         return result
 
+    def __eq__(self, other) -> bool:
+        # Don't compare contents, only identity, for _CONTEXTS.index()
+        if not isinstance(other, Context):
+            return NotImplemented
+        return id(self) == id(other)
+
     def __repr__(self):
         return f"<{self.__class__.__name__} object at {id(self)} with {len(self)} keys>"
 
     def delete(self):
         """Hide the current Context from future :meth:`.get_instance` calls."""
         # Index of the *last* matching instance
         index = len(_CONTEXTS) - 1 - list(reversed(_CONTEXTS)).index(self)
@@ -265,22 +273,16 @@
 
     def get_cache_path(self, *parts) -> Path:
         """Return a path to a local cache file, i.e. within :attr:`.Config.cache_path`.
 
         The directory containing the resulting path is created if it does not already
         exist.
         """
-        # Construct relative to local_data if cache_path is not defined
-        base = self.core.cache_path or self.core.local_data.joinpath("cache")
-
-        result = base.joinpath(*parts)
-
-        # Ensure the directory exists
-        result.parent.mkdir(parents=True, exist_ok=True)
-
+        result = self.core.cache_path.joinpath(*parts)
+        result.parent.mkdir(parents=True, exist_ok=True)  # Ensure the directory exists
         return result
 
     def get_local_path(self, *parts: str, suffix=None) -> Path:
         """Return a path under :attr:`.Config.local_data`.
 
         Parameters
         ==========
@@ -367,15 +369,15 @@
             if platform or model_name or scenario_name or version:
                 raise BadOptionUsage(
                     "--platform --model --scenario and/or --version",
                     " redundant with --url",
                 )
 
             self.core.url = url
-            urlinfo = ixmp.utils.parse_url(url)
+            urlinfo = parse_url(url)
             platform_info.update(urlinfo[0])
             scenario_info.update(urlinfo[1])
         elif platform:
             platform_info["name"] = platform
 
         # Store information about the target Scenario
         if model_name:
```

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/util/importlib.py` & `message-ix-models-2024.4.2rc1/message_ix_models/util/importlib.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/util/ixmp.py` & `message-ix-models-2024.4.2rc1/message_ix_models/util/ixmp.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 from typing import Dict
 
 try:
     # ixmp 3.8.0 and later
-    from ixmp.util import discard_on_error, maybe_check_out, maybe_commit, parse_url
+    from ixmp.util import (
+        discard_on_error,
+        maybe_check_out,
+        maybe_commit,
+        parse_url,
+        show_versions,
+    )
 except ImportError:
     # ixmp <= 3.7.0
     from contextlib import nullcontext
 
     from ixmp.utils import (  # type: ignore [import-not-found,no-redef]  # noqa: F401
         maybe_check_out,
         maybe_commit,
         parse_url,
+        show_versions,
     )
 
     def discard_on_error(*args):
         return nullcontext()
 
 
 def rename_dims() -> Dict[str, str]:
```

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/util/node.py` & `message-ix-models-2024.4.2rc1/message_ix_models/util/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Utilities for nodes."""
+
 import logging
 from typing import List, Sequence, Union
 
 from message_ix import Scenario
 from sdmx.model.v21 import Code
 
 from .common import Adapter, MappingAdapter  # noqa: F401
@@ -122,12 +123,10 @@
         log.info(f"Identified node codelist {repr(id)}")
         return id
 
 
 def nodes_ex_world(nodes: Sequence[Union[str, Code]]) -> List[Union[str, Code]]:
     """Exclude "World" and anything containing "GLB" from `nodes`.
 
-    May also be used as a reporting computation.
-
-    .. todo:: Make available from :mod:`message_ix_models.report`.
+    May also be used as a genno (reporting) operator.
     """
     return list(filter(lambda n_: "GLB" not in n_ and n_ != "World", nodes))
```

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/util/pooch.py` & `message-ix-models-2024.4.2rc1/message_ix_models/util/pooch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Utilities for using :doc:`Pooch <pooch:about>`."""
+
 import logging
 from pathlib import Path
 from typing import Tuple
 
 import click
 import pooch
```

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/util/pycountry.py` & `message-ix-models-2024.4.2rc1/message_ix_models/util/pycountry.py`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/util/scenarioinfo.py` & `message-ix-models-2024.4.2rc1/message_ix_models/util/scenarioinfo.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """:class:`ScenarioInfo` class."""
+
 import logging
 import re
 from collections import defaultdict
 from dataclasses import InitVar, dataclass, field
 from itertools import product
 from typing import TYPE_CHECKING, Dict, List, Optional
 
 import pandas as pd
 import pint
 import sdmx.model.v21 as sdmx_model
 
 from .ixmp import parse_url
-from .sdmx import eval_anno
 
 if TYPE_CHECKING:
     from message_ix import Scenario
 
 log = logging.getLogger(__name__)
 
 
@@ -231,21 +231,24 @@
 
         .. todo:: Expand this discussion and transfer to the :mod:`message_ix` docs.
 
         See also
         --------
         io_units
         """
+
         try:
             idx = self.set[set_name].index(id)
         except ValueError:
             print(self.set[set_name])
             raise
 
-        return eval_anno(self.set[set_name][idx], "units")
+        return self.set[set_name][idx].eval_annotation(
+            id="units", globals=dict(registry=pint.get_application_registry())
+        )
 
     def io_units(
         self, technology: str, commodity: str, level: Optional[str] = None
     ) -> pint.Unit:
         """Return units for the MESSAGE ``input`` or ``output`` parameter.
 
         These are implicitly determined as the ratio of:
@@ -305,16 +308,14 @@
         2020
         >>> info.Y[:3]
         [2020, 2030, 2040]
         >>> info.Y[-3:]
         [2090, 2100, 2110]
 
         """
-        from message_ix_models.util import eval_anno
-
         # Clear existing values
         if len(self.set["year"]):
             log.debug(f"Discard existing 'year' elements: {repr(self.set['year'])}")
             self.set["year"] = []
         if len(self.set["cat_year"]):
             log.debug(
                 f"Discard existing 'cat_year' elements: {repr(self.set['cat_year'])}"
@@ -329,15 +330,15 @@
         # TODO use sorted() here once supported by sdmx
         for code in codes:
             year = int(code.id)
             # Store the year
             self.set["year"].append(year)
 
             # Check for an annotation 'firstmodelyear: true'
-            if eval_anno(code, "firstmodelyear"):
+            if code.eval_annotation(id="firstmodelyear"):
                 if fmy_set:
                     # No coverage: data that triggers this should not be committed
                     raise ValueError(  # pragma: no cover
                         "≥2 periods are annotated firstmodelyear: true"
                     )
 
                 self.y0 = year
@@ -345,15 +346,15 @@
                 fmy_set = True
 
             # Store the duration_period: either from an annotation, or computed vs. the
             # prior period
             duration_period.append(
                 dict(
                     year=year,
-                    value=eval_anno(code, "duration_period")
+                    value=code.eval_annotation(id="duration_period")
                     or (year - duration_period[-1]["year"]),
                     unit="y",
                 )
             )
 
         # Store
         self.par["duration_period"] = pd.DataFrame(duration_period)
```

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/util/sdmx.py` & `message-ix-models-2024.4.2rc1/message_ix_models/util/sdmx.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """Utilities for handling objects from :mod:`sdmx`."""
+
 import logging
 from datetime import datetime
 from enum import Enum, Flag
 from importlib.metadata import version
 from pathlib import Path
 from typing import TYPE_CHECKING, Dict, List, Mapping, Optional, Union
+from warnings import warn
 
 import sdmx
 import sdmx.message
 from iam_units import registry
 from sdmx.model.v21 import AnnotableArtefact, Annotation, Code, InternationalString
 
 from .common import package_data_path
@@ -19,15 +21,18 @@
     import sdmx.model.common
 
 log = logging.getLogger(__name__)
 
 CodeLike = Union[str, Code]
 
 
-def as_codes(data: Union[List[str], Dict[str, CodeLike]]) -> List[Code]:
+# FIXME Reduce complexity from 13 → ≤11
+def as_codes(  # noqa: C901
+    data: Union[List[str], Dict[str, CodeLike]],
+) -> List[Code]:
     """Convert `data` to a :class:`list` of |Code| objects.
 
     Various inputs are accepted:
 
     - :class:`list` of :class:`str`.
     - :class:`dict`, in which keys are :attr:`~sdmx.model.common.Code.id` and values are
       further :class:`dict` with keys matching other Code attributes.
@@ -95,14 +100,21 @@
     """Retrieve the annotation `id` from `obj`, run :func:`eval` on its contents.
 
     .. deprecated:: 2023.9.12
 
        Use :meth:`sdmx.model.common.AnnotableArtefact.eval_annotation`, which provides
        the same functionality.
     """
+    warn(
+        "message_ix_models.util.eval_anno; use sdmx.model.common.AnnotableArtefact"
+        ".eval_annotation() instead.",
+        DeprecationWarning,
+        stacklevel=2,
+    )
+
     try:
         value = str(obj.get_annotation(id=id).text)
     except KeyError:  # No such attribute
         return None
 
     try:
         return eval(value, {"registry": registry})
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models/workflow.py` & `message-ix-models-2024.4.2rc1/message_ix_models/workflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tools for modeling workflows."""
+
 import logging
 import re
 from typing import (
     TYPE_CHECKING,
     Callable,
     List,
     Literal,
@@ -316,14 +317,16 @@
         "--from", "truncate_step", help="Truncate workflow at matching step(s)."
     )
     @click.argument("target_step", metavar="TARGET", required=False)
     @click.pass_obj
     def _func(context, go, truncate_step, target_step, **kwargs):
         from importlib import import_module
 
+        from message_ix_models.util import show_versions
+
         # Import the module and retrieve the callback function
         module_name, callback_name = wf_callback.rsplit(".", maxsplit=1)
         module = import_module(module_name)
         callback = getattr(module, callback_name)
 
         # Generate the workflow
         wf = callback(context, **kwargs)
@@ -357,15 +360,16 @@
             # Workflow default
             if not wf.default_key:
                 raise click.ClickException(
                     f"No target step provided and no default for {wf}"
                 )
             target_step = wf.default_key
 
-        log.info(f"Execute workflow:\n{wf.describe(target_step)}")
+        log.info(f"Execute workflow\n{wf.describe(target_step)}")
+        log.debug(f"…with package versions:\n{show_versions()}")
 
         if not go:
             path = context.get_local_path(f"{slug}-workflow.svg")
             wf.visualize(str(path))
             log.info(f"Workflow diagram written to {path}")
             return
```

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models.egg-info/PKG-INFO` & `message-ix-models-2024.4.2rc1/message_ix_models.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: message-ix-models
-Version: 2024.1.29rc1
+Version: 2024.4.2rc1
 Summary: Tools for the MESSAGEix-GLOBIOM family of models
 Author: IIASA Energy, Climate, and Environment (ECE) Program
 Maintainer-email: Paul Natsuo Kishimoto <mail@paul.kishimoto.name>, Fridolin Glatter <glatter@iiasa.ac.at>
 Project-URL: homepage, https://github.com/iiasa/message-ix-models
 Project-URL: repository, https://github.com/iiasa/message-ix-models
 Project-URL: documentation, https://docs.messageix.org/models
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,14 +15,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: R
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: click
```

### Comparing `message-ix-models-2024.1.29rc1/message_ix_models.egg-info/SOURCES.txt` & `message-ix-models-2024.4.2rc1/message_ix_models.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 .readthedocs.yaml
 LICENSE
 MANIFEST.in
 README.rst
 conftest.py
 pyproject.toml
 .github/codecov.yml
+.github/dependabot.yml
 .github/pull_request_template.md
 .github/workflows/publish.yaml
 .github/workflows/pytest.yaml
 doc/Makefile
 doc/bibliography.rst
 doc/cli.rst
 doc/conf.py
```

### Comparing `message-ix-models-2024.1.29rc1/pyproject.toml` & `message-ix-models-2024.4.2rc1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,15 @@
   "Operating System :: OS Independent",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
   "Programming Language :: R",
   "Topic :: Scientific/Engineering",
   "Topic :: Scientific/Engineering :: Information Analysis",
 ]
 requires-python = ">=3.8"
 dependencies = [
   "click",
@@ -112,17 +113,18 @@
 no_implicit_optional = false
 
 [tool.pytest.ini_options]
 # Disable faulthandler plugin on Windows to prevent spurious console noise
 addopts = "-p no:faulthandler --cov=message_ix_models --cov-report="
 filterwarnings = "ignore:distutils Version classes.*:DeprecationWarning"
 
-[tool.ruff]
+[tool.ruff.lint]
 select = ["C9", "E", "F", "I", "W"]
-
-[tool.ruff.mccabe]
-max-complexity = 13
+# Exceptions:
+# - .tools.wb.assign_income_groups(): 12 > 11
+# - .util.sdmx.as_codes(): 13 > 11
+mccabe.max-complexity = 11
 
 [tool.setuptools.packages]
 find = {}
 
 [tool.setuptools_scm]
```

### Comparing `message-ix-models-2024.1.29rc1/util/1-prep.sh` & `message-ix-models-2024.4.2rc1/util/1-prep.sh`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/util/2-migrate.sh` & `message-ix-models-2024.4.2rc1/util/2-migrate.sh`

 * *Files identical despite different names*

### Comparing `message-ix-models-2024.1.29rc1/util/settings.sh` & `message-ix-models-2024.4.2rc1/util/settings.sh`

 * *Files identical despite different names*

