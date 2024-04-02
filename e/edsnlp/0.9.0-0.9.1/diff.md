# Comparing `tmp/edsnlp-0.9.0.tar.gz` & `tmp/edsnlp-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edsnlp-0.9.0.tar", last modified: Fri Sep 15 16:31:52 2023, max compression
+gzip compressed data, was "edsnlp-0.9.1.tar", last modified: Fri Sep 22 09:07:12 2023, max compression
```

## Comparing `edsnlp-0.9.0.tar` & `edsnlp-0.9.1.tar`

### file list

```diff
@@ -1,493 +1,493 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.309092 edsnlp-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2023-09-15 16:31:25.000000 edsnlp-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7359 2023-09-15 16:31:52.309092 edsnlp-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3155 2023-09-15 16:31:25.000000 edsnlp-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.249091 edsnlp-0.9.0/demo/
--rw-r--r--   0 runner    (1001) docker     (127)     8685 2023-09-15 16:31:25.000000 edsnlp-0.9.0/demo/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.241090 edsnlp-0.9.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.253091 edsnlp-0.9.0/docs/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.253091 edsnlp-0.9.0/docs/scripts/autorefs/
--rw-r--r--   0 runner    (1001) docker     (127)    17872 2023-09-15 16:31:25.000000 edsnlp-0.9.0/docs/scripts/autorefs/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     9408 2023-09-15 16:31:25.000000 edsnlp-0.9.0/docs/scripts/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (127)     3914 2023-09-15 16:31:25.000000 edsnlp-0.9.0/docs/scripts/griffe_ext.py
--rw-r--r--   0 runner    (1001) docker     (127)     5231 2023-09-15 16:31:25.000000 edsnlp-0.9.0/docs/scripts/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.253091 edsnlp-0.9.0/edsnlp/
--rw-r--r--   0 runner    (1001) docker     (127)      205 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/conjugator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.253091 edsnlp-0.9.0/edsnlp/connectors/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20335 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/connectors/brat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/connectors/labeltool.py
--rw-r--r--   0 runner    (1001) docker     (127)     8130 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/connectors/omop.py
--rw-r--r--   0 runner    (1001) docker     (127)      310 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3909 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/language.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.257091 edsnlp-0.9.0/edsnlp/matchers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/matchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  1217190 2023-09-15 16:31:49.000000 edsnlp-0.9.0/edsnlp/matchers/phrase.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      431 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/matchers/phrase.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     6301 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/matchers/phrase.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    14621 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/matchers/regex.py
--rw-r--r--   0 runner    (1001) docker     (127)    10143 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/matchers/simstring.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.257091 edsnlp-0.9.0/edsnlp/matchers/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      334 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/matchers/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3177 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/matchers/utils/offset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/matchers/utils/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     4620 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/patch_spacy_dot_components.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.257091 edsnlp-0.9.0/edsnlp/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9768 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.257091 edsnlp-0.9.0/edsnlp/pipelines/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.257091 edsnlp-0.9.0/edsnlp/pipelines/core/context/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/core/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/core/context/context.py
--rw-r--r--   0 runner    (1001) docker     (127)      377 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/core/context/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.257091 edsnlp-0.9.0/edsnlp/pipelines/core/contextual_matcher/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/core/contextual_matcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15664 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/core/contextual_matcher/contextual_matcher.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/core/contextual_matcher/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     5522 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/core/contextual_matcher/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.257091 edsnlp-0.9.0/edsnlp/pipelines/core/endlines/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/core/endlines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8241 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/core/endlines/endlines.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/core/endlines/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/core/endlines/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)    22618 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/core/endlines/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.257091 edsnlp-0.9.0/edsnlp/pipelines/core/matcher/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/core/matcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/core/matcher/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     5650 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/core/matcher/matcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.257091 edsnlp-0.9.0/edsnlp/pipelines/core/normalizer/
--rw-r--r--   0 runner    (1001) docker     (127)      356 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/core/normalizer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.261091 edsnlp-0.9.0/edsnlp/pipelines/core/normalizer/accents/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/core/normalizer/accents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/core/normalizer/accents/accents.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/core/normalizer/accents/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      298 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/core/normalizer/accents/patterns.py
--rw-r--r--   0 runner    (1001) docker     (127)     3051 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/core/normalizer/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/core/normalizer/normalizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.261091 edsnlp-0.9.0/edsnlp/pipelines/core/normalizer/pollution/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/core/normalizer/pollution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/core/normalizer/pollution/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/core/normalizer/pollution/patterns.py
--rw-r--r--   0 runner    (1001) docker     (127)     3122 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/core/normalizer/pollution/pollution.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.261091 edsnlp-0.9.0/edsnlp/pipelines/core/normalizer/quotes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/core/normalizer/quotes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      494 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/core/normalizer/quotes/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      854 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/core/normalizer/quotes/patterns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/core/normalizer/quotes/quotes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.261091 edsnlp-0.9.0/edsnlp/pipelines/core/normalizer/remove_lowercase/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/core/normalizer/remove_lowercase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/core/normalizer/remove_lowercase/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.261091 edsnlp-0.9.0/edsnlp/pipelines/core/normalizer/spaces/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/core/normalizer/spaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/core/normalizer/spaces/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/core/normalizer/spaces/spaces.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.261091 edsnlp-0.9.0/edsnlp/pipelines/core/sentences/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/core/sentences/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3337 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/core/sentences/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)  1065666 2023-09-15 16:31:51.000000 edsnlp-0.9.0/edsnlp/pipelines/core/sentences/sentences.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      459 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/core/sentences/sentences.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     3603 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/core/sentences/sentences.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/core/sentences/terms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.265091 edsnlp-0.9.0/edsnlp/pipelines/core/terminology/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/core/terminology/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/core/terminology/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     6927 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/core/terminology/terminology.py
--rw-r--r--   0 runner    (1001) docker     (127)     4196 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/factories.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.265091 edsnlp-0.9.0/edsnlp/pipelines/misc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/misc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.265091 edsnlp-0.9.0/edsnlp/pipelines/misc/consultation_dates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/misc/consultation_dates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7305 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/misc/consultation_dates/consultation_dates.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/misc/consultation_dates/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/misc/consultation_dates/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.265091 edsnlp-0.9.0/edsnlp/pipelines/misc/dates/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/misc/dates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15356 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/misc/dates/dates.py
--rw-r--r--   0 runner    (1001) docker     (127)      864 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/misc/dates/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     9448 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/misc/dates/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.265091 edsnlp-0.9.0/edsnlp/pipelines/misc/dates/patterns/
--rw-r--r--   0 runner    (1001) docker     (127)      233 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/misc/dates/patterns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/misc/dates/patterns/absolute.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.265091 edsnlp-0.9.0/edsnlp/pipelines/misc/dates/patterns/atomic/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/misc/dates/patterns/atomic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/misc/dates/patterns/atomic/days.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/misc/dates/patterns/atomic/delimiters.py
--rw-r--r--   0 runner    (1001) docker     (127)      522 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/misc/dates/patterns/atomic/directions.py
--rw-r--r--   0 runner    (1001) docker     (127)      222 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/misc/dates/patterns/atomic/modes.py
--rw-r--r--   0 runner    (1001) docker     (127)      890 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/misc/dates/patterns/atomic/months.py
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/misc/dates/patterns/atomic/numbers.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/misc/dates/patterns/atomic/time.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/misc/dates/patterns/atomic/units.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/misc/dates/patterns/atomic/years.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/misc/dates/patterns/current.py
--rw-r--r--   0 runner    (1001) docker     (127)      180 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/misc/dates/patterns/duration.py
--rw-r--r--   0 runner    (1001) docker     (127)      300 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/misc/dates/patterns/false_positive.py
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/misc/dates/patterns/relative.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.265091 edsnlp-0.9.0/edsnlp/pipelines/misc/measurements/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/misc/measurements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      969 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/misc/measurements/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    38732 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/misc/measurements/measurements.py
--rw-r--r--   0 runner    (1001) docker     (127)    14152 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/misc/measurements/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.269091 edsnlp-0.9.0/edsnlp/pipelines/misc/reason/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/misc/reason/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      482 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/misc/reason/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/misc/reason/patterns.py
--rw-r--r--   0 runner    (1001) docker     (127)     6295 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/misc/reason/reason.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.269091 edsnlp-0.9.0/edsnlp/pipelines/misc/sections/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/misc/sections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      528 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/misc/sections/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3673 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/misc/sections/patterns.py
--rw-r--r--   0 runner    (1001) docker     (127)     5697 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/misc/sections/sections.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.269091 edsnlp-0.9.0/edsnlp/pipelines/misc/tables/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/misc/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/misc/tables/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/misc/tables/patterns.py
--rw-r--r--   0 runner    (1001) docker     (127)     5225 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/misc/tables/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.269091 edsnlp-0.9.0/edsnlp/pipelines/ner/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.269091 edsnlp-0.9.0/edsnlp/pipelines/ner/adicap/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/adicap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7911 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/adicap/adicap.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/adicap/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/adicap/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      506 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/adicap/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.269091 edsnlp-0.9.0/edsnlp/pipelines/ner/behaviors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/behaviors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.269091 edsnlp-0.9.0/edsnlp/pipelines/ner/behaviors/alcohol/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/behaviors/alcohol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3189 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/behaviors/alcohol/alcohol.py
--rw-r--r--   0 runner    (1001) docker     (127)      344 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/behaviors/alcohol/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/behaviors/alcohol/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.269091 edsnlp-0.9.0/edsnlp/pipelines/ner/behaviors/tobacco/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/behaviors/tobacco/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      344 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/behaviors/tobacco/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/behaviors/tobacco/patterns.py
--rw-r--r--   0 runner    (1001) docker     (127)     3845 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/behaviors/tobacco/tobacco.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.269091 edsnlp-0.9.0/edsnlp/pipelines/ner/cim10/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/cim10/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3087 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/cim10/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/cim10/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.273091 edsnlp-0.9.0/edsnlp/pipelines/ner/covid/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/covid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2157 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/covid/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/covid/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.273091 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.273091 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/aids/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/aids/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4645 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/aids/aids.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/aids/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/aids/patterns.py
--rw-r--r--   0 runner    (1001) docker     (127)     3422 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.273091 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/cerebrovascular_accident/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/cerebrovascular_accident/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3347 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/cerebrovascular_accident/cerebrovascular_accident.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/cerebrovascular_accident/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2834 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/cerebrovascular_accident/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.273091 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/ckd/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/ckd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4420 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/ckd/ckd.py
--rw-r--r--   0 runner    (1001) docker     (127)      505 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/ckd/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2988 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/ckd/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.273091 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/congestive_heart_failure/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/congestive_heart_failure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/congestive_heart_failure/congestive_heart_failure.py
--rw-r--r--   0 runner    (1001) docker     (127)      442 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/congestive_heart_failure/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/congestive_heart_failure/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.273091 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/connective_tissue_disease/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/connective_tissue_disease/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3035 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/connective_tissue_disease/connective_tissue_disease.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/connective_tissue_disease/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/connective_tissue_disease/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.273091 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/copd/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/copd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/copd/copd.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/copd/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2405 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/copd/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.277091 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/dementia/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/dementia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2554 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/dementia/dementia.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/dementia/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/dementia/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.277091 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/diabetes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/diabetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4552 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/diabetes/diabetes.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/diabetes/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/diabetes/patterns.py
--rw-r--r--   0 runner    (1001) docker     (127)      353 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.277091 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/hemiplegia/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/hemiplegia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      362 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/hemiplegia/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/hemiplegia/hemiplegia.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/hemiplegia/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.277091 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/leukemia/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/leukemia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/leukemia/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/leukemia/leukemia.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/leukemia/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.277091 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/liver_disease/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/liver_disease/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/liver_disease/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/liver_disease/liver_disease.py
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/liver_disease/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.277091 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/lymphoma/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/lymphoma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/lymphoma/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2698 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/lymphoma/lymphoma.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/lymphoma/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.277091 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/myocardial_infarction/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/myocardial_infarction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/myocardial_infarction/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3317 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/myocardial_infarction/myocardial_infarction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/myocardial_infarction/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.277091 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/peptic_ulcer_disease/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/peptic_ulcer_disease/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/peptic_ulcer_disease/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      821 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/peptic_ulcer_disease/patterns.py
--rw-r--r--   0 runner    (1001) docker     (127)     2976 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/peptic_ulcer_disease/peptic_ulcer_disease.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.281091 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/peripheral_vascular_disease/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/peripheral_vascular_disease/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/peripheral_vascular_disease/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4341 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/peripheral_vascular_disease/patterns.py
--rw-r--r--   0 runner    (1001) docker     (127)     3121 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/peripheral_vascular_disease/peripheral_vascular_disease.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.281091 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/solid_tumor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/solid_tumor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/solid_tumor/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/solid_tumor/patterns.py
--rw-r--r--   0 runner    (1001) docker     (127)     4317 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/solid_tumor/solid_tumor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/terms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.281091 edsnlp-0.9.0/edsnlp/pipelines/ner/drugs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/drugs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3487 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/drugs/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/drugs/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.281091 edsnlp-0.9.0/edsnlp/pipelines/ner/scores/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/scores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5369 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/scores/base_score.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.281091 edsnlp-0.9.0/edsnlp/pipelines/ner/scores/charlson/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/scores/charlson/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3842 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/scores/charlson/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/scores/charlson/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.281091 edsnlp-0.9.0/edsnlp/pipelines/ner/scores/elston_ellis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/scores/elston_ellis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3261 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/scores/elston_ellis/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      820 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/scores/elston_ellis/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.281091 edsnlp-0.9.0/edsnlp/pipelines/ner/scores/emergency/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/scores/emergency/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.281091 edsnlp-0.9.0/edsnlp/pipelines/ner/scores/emergency/ccmu/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/scores/emergency/ccmu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3416 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/scores/emergency/ccmu/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/scores/emergency/ccmu/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.281091 edsnlp-0.9.0/edsnlp/pipelines/ner/scores/emergency/gemsa/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/scores/emergency/gemsa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3419 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/scores/emergency/gemsa/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      528 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/scores/emergency/gemsa/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.281091 edsnlp-0.9.0/edsnlp/pipelines/ner/scores/emergency/priority/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/scores/emergency/priority/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/scores/emergency/priority/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/scores/emergency/priority/patterns.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/scores/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.281091 edsnlp-0.9.0/edsnlp/pipelines/ner/scores/sofa/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/scores/sofa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3881 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/scores/sofa/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/scores/sofa/patterns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/scores/sofa/sofa.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.285091 edsnlp-0.9.0/edsnlp/pipelines/ner/tnm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/tnm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/tnm/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4829 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/tnm/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/tnm/patterns.py
--rw-r--r--   0 runner    (1001) docker     (127)     4240 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/tnm/tnm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.285091 edsnlp-0.9.0/edsnlp/pipelines/ner/umls/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/umls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4129 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/umls/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4547 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/ner/umls/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.285091 edsnlp-0.9.0/edsnlp/pipelines/qualifiers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/qualifiers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3984 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/qualifiers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      177 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/qualifiers/factories.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.285091 edsnlp-0.9.0/edsnlp/pipelines/qualifiers/family/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/qualifiers/family/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/qualifiers/family/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     7016 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/qualifiers/family/family.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/qualifiers/family/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.285091 edsnlp-0.9.0/edsnlp/pipelines/qualifiers/history/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/qualifiers/history/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/qualifiers/history/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    21415 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/qualifiers/history/history.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/qualifiers/history/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.285091 edsnlp-0.9.0/edsnlp/pipelines/qualifiers/hypothesis/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/qualifiers/hypothesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/qualifiers/hypothesis/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    10625 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/qualifiers/hypothesis/hypothesis.py
--rw-r--r--   0 runner    (1001) docker     (127)    13450 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/qualifiers/hypothesis/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.285091 edsnlp-0.9.0/edsnlp/pipelines/qualifiers/negation/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/qualifiers/negation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      599 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/qualifiers/negation/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    10603 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/qualifiers/negation/negation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2411 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/qualifiers/negation/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.285091 edsnlp-0.9.0/edsnlp/pipelines/qualifiers/reported_speech/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/qualifiers/reported_speech/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/qualifiers/reported_speech/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/qualifiers/reported_speech/patterns.py
--rw-r--r--   0 runner    (1001) docker     (127)     9107 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/qualifiers/reported_speech/reported_speech.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/terminations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.285091 edsnlp-0.9.0/edsnlp/pipelines/trainable/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/trainable/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.289091 edsnlp-0.9.0/edsnlp/pipelines/trainable/layers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/trainable/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14885 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/trainable/layers/crf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.289091 edsnlp-0.9.0/edsnlp/pipelines/trainable/nested_ner/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/trainable/nested_ner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/trainable/nested_ner/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    12934 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/trainable/nested_ner/nested_ner.py
--rw-r--r--   0 runner    (1001) docker     (127)     7042 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/trainable/nested_ner/stack_crf_ner.py
--rw-r--r--   0 runner    (1001) docker     (127)     9682 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/trainable/pytorch_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.289091 edsnlp-0.9.0/edsnlp/pipelines/trainable/span_qualifier/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/trainable/span_qualifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4732 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/trainable/span_qualifier/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     8149 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/trainable/span_qualifier/span_multi_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)    18193 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/trainable/span_qualifier/span_qualifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     5889 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/pipelines/trainable/span_qualifier/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.289091 edsnlp-0.9.0/edsnlp/processing/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9653 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/processing/distributed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/processing/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4129 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/processing/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     6708 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/processing/simple.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/processing/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4130 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/processing/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.289091 edsnlp-0.9.0/edsnlp/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     7192 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/resources/AVC.csv.gz
--rw-r--r--   0 runner    (1001) docker     (127)    95841 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/resources/adicap.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)   604577 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/resources/cim10.csv.gz
--rw-r--r--   0 runner    (1001) docker     (127)   136088 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/resources/drugs.json
--rw-r--r--   0 runner    (1001) docker     (127)   200566 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/resources/verbs.csv.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.293091 edsnlp-0.9.0/edsnlp/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/utils/collections.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2594 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/utils/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2935 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/utils/examples.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/utils/extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8838 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/utils/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      966 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/utils/inclusion.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/utils/lists.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/utils/merge_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/utils/numbers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/utils/regex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/utils/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     3877 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/utils/span_getters.py
--rw-r--r--   0 runner    (1001) docker     (127)    10810 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/utils/training.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.293091 edsnlp-0.9.0/edsnlp/viz/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/viz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5438 2023-09-15 16:31:25.000000 edsnlp-0.9.0/edsnlp/viz/quick_examples.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.253091 edsnlp-0.9.0/edsnlp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7359 2023-09-15 16:31:52.000000 edsnlp-0.9.0/edsnlp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16840 2023-09-15 16:31:52.000000 edsnlp-0.9.0/edsnlp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-15 16:31:52.000000 edsnlp-0.9.0/edsnlp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8217 2023-09-15 16:31:52.000000 edsnlp-0.9.0/edsnlp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      926 2023-09-15 16:31:52.000000 edsnlp-0.9.0/edsnlp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2023-09-15 16:31:52.000000 edsnlp-0.9.0/edsnlp.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.293091 edsnlp-0.9.0/notebooks/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.293091 edsnlp-0.9.0/notebooks/connectors/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2023-09-15 16:31:25.000000 edsnlp-0.9.0/notebooks/connectors/context.py
--rw-r--r--   0 runner    (1001) docker     (127)      129 2023-09-15 16:31:25.000000 edsnlp-0.9.0/notebooks/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.293091 edsnlp-0.9.0/notebooks/dates/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2023-09-15 16:31:25.000000 edsnlp-0.9.0/notebooks/dates/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.293091 edsnlp-0.9.0/notebooks/normalizer/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2023-09-15 16:31:25.000000 edsnlp-0.9.0/notebooks/normalizer/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.293091 edsnlp-0.9.0/notebooks/sections/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2023-09-15 16:31:25.000000 edsnlp-0.9.0/notebooks/sections/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.293091 edsnlp-0.9.0/notebooks/sentences/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2023-09-15 16:31:25.000000 edsnlp-0.9.0/notebooks/sentences/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.293091 edsnlp-0.9.0/notebooks/tokenizer/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2023-09-15 16:31:25.000000 edsnlp-0.9.0/notebooks/tokenizer/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.293091 edsnlp-0.9.0/notebooks/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2023-09-15 16:31:25.000000 edsnlp-0.9.0/notebooks/utilities/context.py
--rw-r--r--   0 runner    (1001) docker     (127)    16708 2023-09-15 16:31:25.000000 edsnlp-0.9.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.293091 edsnlp-0.9.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2023-09-15 16:31:25.000000 edsnlp-0.9.0/scripts/adicap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2023-09-15 16:31:25.000000 edsnlp-0.9.0/scripts/cim10.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2023-09-15 16:31:25.000000 edsnlp-0.9.0/scripts/conjugate_verbs.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2023-09-15 16:31:25.000000 edsnlp-0.9.0/scripts/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2023-09-15 16:31:25.000000 edsnlp-0.9.0/scripts/serve.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-15 16:31:52.309092 edsnlp-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2023-09-15 16:31:25.000000 edsnlp-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.297092 edsnlp-0.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2023-09-15 16:31:25.000000 edsnlp-0.9.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.297092 edsnlp-0.9.0/tests/connectors/
--rw-r--r--   0 runner    (1001) docker     (127)     5850 2023-09-15 16:31:25.000000 edsnlp-0.9.0/tests/connectors/test_brat.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2023-09-15 16:31:25.000000 edsnlp-0.9.0/tests/connectors/test_labeltool.py
--rw-r--r--   0 runner    (1001) docker     (127)     2722 2023-09-15 16:31:25.000000 edsnlp-0.9.0/tests/connectors/test_omop.py
--rw-r--r--   0 runner    (1001) docker     (127)     5681 2023-09-15 16:31:25.000000 edsnlp-0.9.0/tests/extract_docs_code.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.297092 edsnlp-0.9.0/tests/matchers/
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2023-09-15 16:31:25.000000 edsnlp-0.9.0/tests/matchers/test_phrase.py
--rw-r--r--   0 runner    (1001) docker     (127)     6399 2023-09-15 16:31:25.000000 edsnlp-0.9.0/tests/matchers/test_regex.py
--rw-r--r--   0 runner    (1001) docker     (127)     3021 2023-09-15 16:31:25.000000 edsnlp-0.9.0/tests/matchers/test_simstring.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.297092 edsnlp-0.9.0/tests/pipelines/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.297092 edsnlp-0.9.0/tests/pipelines/core/
--rw-r--r--   0 runner    (1001) docker     (127)    12291 2023-09-15 16:31:25.000000 edsnlp-0.9.0/tests/pipelines/core/test_contextual_matcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2023-09-15 16:31:25.000000 edsnlp-0.9.0/tests/pipelines/core/test_endlines.py
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2023-09-15 16:31:25.000000 edsnlp-0.9.0/tests/pipelines/core/test_matcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3294 2023-09-15 16:31:25.000000 edsnlp-0.9.0/tests/pipelines/core/test_normalisation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2023-09-15 16:31:25.000000 edsnlp-0.9.0/tests/pipelines/core/test_sentences.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2023-09-15 16:31:25.000000 edsnlp-0.9.0/tests/pipelines/core/test_terminology.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.297092 edsnlp-0.9.0/tests/pipelines/misc/
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2023-09-15 16:31:25.000000 edsnlp-0.9.0/tests/pipelines/misc/test_consultation_date.py
--rw-r--r--   0 runner    (1001) docker     (127)     8993 2023-09-15 16:31:25.000000 edsnlp-0.9.0/tests/pipelines/misc/test_dates.py
--rw-r--r--   0 runner    (1001) docker     (127)     6740 2023-09-15 16:31:25.000000 edsnlp-0.9.0/tests/pipelines/misc/test_measurements.py
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2023-09-15 16:31:25.000000 edsnlp-0.9.0/tests/pipelines/misc/test_reason.py
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2023-09-15 16:31:25.000000 edsnlp-0.9.0/tests/pipelines/misc/test_sections.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2023-09-15 16:31:25.000000 edsnlp-0.9.0/tests/pipelines/misc/test_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.301092 edsnlp-0.9.0/tests/pipelines/ner/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.301092 edsnlp-0.9.0/tests/pipelines/ner/disorders/
--rw-r--r--   0 runner    (1001) docker     (127)      418 2023-09-15 16:31:25.000000 edsnlp-0.9.0/tests/pipelines/ner/disorders/AIDS.py
--rw-r--r--   0 runner    (1001) docker     (127)      920 2023-09-15 16:31:25.000000 edsnlp-0.9.0/tests/pipelines/ner/disorders/CKD.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2023-09-15 16:31:25.000000 edsnlp-0.9.0/tests/pipelines/ner/disorders/COPD.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2023-09-15 16:31:25.000000 edsnlp-0.9.0/tests/pipelines/ner/disorders/alcohol.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2023-09-15 16:31:25.000000 edsnlp-0.9.0/tests/pipelines/ner/disorders/cerebrovascular_accident.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2023-09-15 16:31:25.000000 edsnlp-0.9.0/tests/pipelines/ner/disorders/congestive_heart_failure.py
--rw-r--r--   0 runner    (1001) docker     (127)      394 2023-09-15 16:31:25.000000 edsnlp-0.9.0/tests/pipelines/ner/disorders/connective_tissue_disease.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2023-09-15 16:31:25.000000 edsnlp-0.9.0/tests/pipelines/ner/disorders/dementia.py
--rw-r--r--   0 runner    (1001) docker     (127)      677 2023-09-15 16:31:25.000000 edsnlp-0.9.0/tests/pipelines/ner/disorders/diabetes.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2023-09-15 16:31:25.000000 edsnlp-0.9.0/tests/pipelines/ner/disorders/hemiplegia.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2023-09-15 16:31:25.000000 edsnlp-0.9.0/tests/pipelines/ner/disorders/leukemia.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2023-09-15 16:31:25.000000 edsnlp-0.9.0/tests/pipelines/ner/disorders/liver_disease.py
--rw-r--r--   0 runner    (1001) docker     (127)      306 2023-09-15 16:31:25.000000 edsnlp-0.9.0/tests/pipelines/ner/disorders/lymphoma.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2023-09-15 16:31:25.000000 edsnlp-0.9.0/tests/pipelines/ner/disorders/myocardial_infarction.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2023-09-15 16:31:25.000000 edsnlp-0.9.0/tests/pipelines/ner/disorders/peptic_ulcer_disease.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2023-09-15 16:31:25.000000 edsnlp-0.9.0/tests/pipelines/ner/disorders/peripheral_vascular_disease.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2023-09-15 16:31:25.000000 edsnlp-0.9.0/tests/pipelines/ner/disorders/solid_tumor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3321 2023-09-15 16:31:25.000000 edsnlp-0.9.0/tests/pipelines/ner/disorders/test_all.py
--rw-r--r--   0 runner    (1001) docker     (127)      585 2023-09-15 16:31:25.000000 edsnlp-0.9.0/tests/pipelines/ner/disorders/tobacco.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2023-09-15 16:31:25.000000 edsnlp-0.9.0/tests/pipelines/ner/test_adicap.py
--rw-r--r--   0 runner    (1001) docker     (127)     3494 2023-09-15 16:31:25.000000 edsnlp-0.9.0/tests/pipelines/ner/test_adicap_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2023-09-15 16:31:25.000000 edsnlp-0.9.0/tests/pipelines/ner/test_cim10.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2023-09-15 16:31:25.000000 edsnlp-0.9.0/tests/pipelines/ner/test_covid.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2023-09-15 16:31:25.000000 edsnlp-0.9.0/tests/pipelines/ner/test_drugs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2023-09-15 16:31:25.000000 edsnlp-0.9.0/tests/pipelines/ner/test_score.py
--rw-r--r--   0 runner    (1001) docker     (127)      977 2023-09-15 16:31:25.000000 edsnlp-0.9.0/tests/pipelines/ner/test_tnm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2023-09-15 16:31:25.000000 edsnlp-0.9.0/tests/pipelines/ner/test_umls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.301092 edsnlp-0.9.0/tests/pipelines/qualifiers/
--rw-r--r--   0 runner    (1001) docker     (127)      185 2023-09-15 16:31:25.000000 edsnlp-0.9.0/tests/pipelines/qualifiers/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2023-09-15 16:31:25.000000 edsnlp-0.9.0/tests/pipelines/qualifiers/test_family.py
--rw-r--r--   0 runner    (1001) docker     (127)     2668 2023-09-15 16:31:25.000000 edsnlp-0.9.0/tests/pipelines/qualifiers/test_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     2815 2023-09-15 16:31:25.000000 edsnlp-0.9.0/tests/pipelines/qualifiers/test_hypothesis.py
--rw-r--r--   0 runner    (1001) docker     (127)     3574 2023-09-15 16:31:25.000000 edsnlp-0.9.0/tests/pipelines/qualifiers/test_negation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3960 2023-09-15 16:31:25.000000 edsnlp-0.9.0/tests/pipelines/qualifiers/test_reported_speech.py
--rw-r--r--   0 runner    (1001) docker     (127)      267 2023-09-15 16:31:25.000000 edsnlp-0.9.0/tests/pipelines/test_pipelines.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.301092 edsnlp-0.9.0/tests/pipelines/trainable/
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2023-09-15 16:31:25.000000 edsnlp-0.9.0/tests/pipelines/trainable/test_nested_ner.py
--rw-r--r--   0 runner    (1001) docker     (127)     5077 2023-09-15 16:31:25.000000 edsnlp-0.9.0/tests/pipelines/trainable/test_span_classifier.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.301092 edsnlp-0.9.0/tests/processing/
--rw-r--r--   0 runner    (1001) docker     (127)     5409 2023-09-15 16:31:25.000000 edsnlp-0.9.0/tests/processing/test_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2023-09-15 16:31:25.000000 edsnlp-0.9.0/tests/test_conjugator.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2023-09-15 16:31:25.000000 edsnlp-0.9.0/tests/test_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2023-09-15 16:31:25.000000 edsnlp-0.9.0/tests/test_language.py
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2023-09-15 16:31:25.000000 edsnlp-0.9.0/tests/test_span_args.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 16:31:52.305092 edsnlp-0.9.0/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2023-09-15 16:31:25.000000 edsnlp-0.9.0/tests/utils/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2023-09-15 16:31:25.000000 edsnlp-0.9.0/tests/utils/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      988 2023-09-15 16:31:25.000000 edsnlp-0.9.0/tests/utils/test_quick_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.250249 edsnlp-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2023-09-22 09:06:49.000000 edsnlp-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7359 2023-09-22 09:07:12.250249 edsnlp-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2023-09-22 09:06:49.000000 edsnlp-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.202248 edsnlp-0.9.1/demo/
+-rw-r--r--   0 runner    (1001) docker     (127)     8685 2023-09-22 09:06:49.000000 edsnlp-0.9.1/demo/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.198248 edsnlp-0.9.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.206248 edsnlp-0.9.1/docs/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.206248 edsnlp-0.9.1/docs/scripts/autorefs/
+-rw-r--r--   0 runner    (1001) docker     (127)    17872 2023-09-22 09:06:49.000000 edsnlp-0.9.1/docs/scripts/autorefs/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9408 2023-09-22 09:06:49.000000 edsnlp-0.9.1/docs/scripts/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3914 2023-09-22 09:06:49.000000 edsnlp-0.9.1/docs/scripts/griffe_ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5231 2023-09-22 09:06:49.000000 edsnlp-0.9.1/docs/scripts/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.206248 edsnlp-0.9.1/edsnlp/
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/conjugator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.206248 edsnlp-0.9.1/edsnlp/connectors/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20335 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/connectors/brat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/connectors/labeltool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8130 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/connectors/omop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3909 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/language.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.206248 edsnlp-0.9.1/edsnlp/matchers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/matchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1217190 2023-09-22 09:07:10.000000 edsnlp-0.9.1/edsnlp/matchers/phrase.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/matchers/phrase.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     6301 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/matchers/phrase.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    14621 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/matchers/regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10143 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/matchers/simstring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.206248 edsnlp-0.9.1/edsnlp/matchers/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/matchers/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3177 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/matchers/utils/offset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/matchers/utils/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4620 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/patch_spacy_dot_components.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.210248 edsnlp-0.9.1/edsnlp/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9768 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.210248 edsnlp-0.9.1/edsnlp/pipelines/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.210248 edsnlp-0.9.1/edsnlp/pipelines/core/context/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/core/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/core/context/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/core/context/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.210248 edsnlp-0.9.1/edsnlp/pipelines/core/contextual_matcher/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/core/contextual_matcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15834 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/core/contextual_matcher/contextual_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/core/contextual_matcher/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5522 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/core/contextual_matcher/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.210248 edsnlp-0.9.1/edsnlp/pipelines/core/endlines/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/core/endlines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8241 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/core/endlines/endlines.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/core/endlines/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/core/endlines/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22618 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/core/endlines/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.210248 edsnlp-0.9.1/edsnlp/pipelines/core/matcher/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/core/matcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/core/matcher/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5650 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/core/matcher/matcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.210248 edsnlp-0.9.1/edsnlp/pipelines/core/normalizer/
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/core/normalizer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.210248 edsnlp-0.9.1/edsnlp/pipelines/core/normalizer/accents/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/core/normalizer/accents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/core/normalizer/accents/accents.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/core/normalizer/accents/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/core/normalizer/accents/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3051 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/core/normalizer/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/core/normalizer/normalizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.210248 edsnlp-0.9.1/edsnlp/pipelines/core/normalizer/pollution/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/core/normalizer/pollution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/core/normalizer/pollution/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/core/normalizer/pollution/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3122 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/core/normalizer/pollution/pollution.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.210248 edsnlp-0.9.1/edsnlp/pipelines/core/normalizer/quotes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/core/normalizer/quotes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/core/normalizer/quotes/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/core/normalizer/quotes/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/core/normalizer/quotes/quotes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.210248 edsnlp-0.9.1/edsnlp/pipelines/core/normalizer/remove_lowercase/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/core/normalizer/remove_lowercase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/core/normalizer/remove_lowercase/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.214249 edsnlp-0.9.1/edsnlp/pipelines/core/normalizer/spaces/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/core/normalizer/spaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/core/normalizer/spaces/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/core/normalizer/spaces/spaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.214249 edsnlp-0.9.1/edsnlp/pipelines/core/sentences/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/core/sentences/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3337 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/core/sentences/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1065666 2023-09-22 09:07:11.000000 edsnlp-0.9.1/edsnlp/pipelines/core/sentences/sentences.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/core/sentences/sentences.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     3603 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/core/sentences/sentences.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/core/sentences/terms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.214249 edsnlp-0.9.1/edsnlp/pipelines/core/terminology/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/core/terminology/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/core/terminology/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6927 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/core/terminology/terminology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4196 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/factories.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.214249 edsnlp-0.9.1/edsnlp/pipelines/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/misc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.214249 edsnlp-0.9.1/edsnlp/pipelines/misc/consultation_dates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/misc/consultation_dates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7305 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/misc/consultation_dates/consultation_dates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/misc/consultation_dates/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/misc/consultation_dates/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.214249 edsnlp-0.9.1/edsnlp/pipelines/misc/dates/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/misc/dates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15446 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/misc/dates/dates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/misc/dates/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9448 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/misc/dates/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.214249 edsnlp-0.9.1/edsnlp/pipelines/misc/dates/patterns/
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/misc/dates/patterns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/misc/dates/patterns/absolute.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.218248 edsnlp-0.9.1/edsnlp/pipelines/misc/dates/patterns/atomic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/misc/dates/patterns/atomic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/misc/dates/patterns/atomic/days.py
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/misc/dates/patterns/atomic/delimiters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/misc/dates/patterns/atomic/directions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/misc/dates/patterns/atomic/modes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/misc/dates/patterns/atomic/months.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/misc/dates/patterns/atomic/numbers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/misc/dates/patterns/atomic/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/misc/dates/patterns/atomic/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/misc/dates/patterns/atomic/years.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/misc/dates/patterns/current.py
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/misc/dates/patterns/duration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/misc/dates/patterns/false_positive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/misc/dates/patterns/relative.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.218248 edsnlp-0.9.1/edsnlp/pipelines/misc/measurements/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/misc/measurements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/misc/measurements/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38732 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/misc/measurements/measurements.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14152 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/misc/measurements/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.218248 edsnlp-0.9.1/edsnlp/pipelines/misc/reason/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/misc/reason/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/misc/reason/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/misc/reason/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6295 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/misc/reason/reason.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.218248 edsnlp-0.9.1/edsnlp/pipelines/misc/sections/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/misc/sections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/misc/sections/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3673 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/misc/sections/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5697 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/misc/sections/sections.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.218248 edsnlp-0.9.1/edsnlp/pipelines/misc/tables/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/misc/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/misc/tables/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/misc/tables/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5225 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/misc/tables/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.218248 edsnlp-0.9.1/edsnlp/pipelines/ner/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.218248 edsnlp-0.9.1/edsnlp/pipelines/ner/adicap/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/adicap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7911 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/adicap/adicap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/adicap/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/adicap/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/adicap/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.218248 edsnlp-0.9.1/edsnlp/pipelines/ner/behaviors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/behaviors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.218248 edsnlp-0.9.1/edsnlp/pipelines/ner/behaviors/alcohol/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/behaviors/alcohol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3189 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/behaviors/alcohol/alcohol.py
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/behaviors/alcohol/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/behaviors/alcohol/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.222248 edsnlp-0.9.1/edsnlp/pipelines/ner/behaviors/tobacco/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/behaviors/tobacco/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/behaviors/tobacco/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/behaviors/tobacco/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3845 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/behaviors/tobacco/tobacco.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.222248 edsnlp-0.9.1/edsnlp/pipelines/ner/cim10/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/cim10/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3087 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/cim10/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/cim10/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.222248 edsnlp-0.9.1/edsnlp/pipelines/ner/covid/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/covid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/covid/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/covid/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.222248 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.222248 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/aids/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/aids/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4645 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/aids/aids.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/aids/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/aids/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3906 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.222248 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/cerebrovascular_accident/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/cerebrovascular_accident/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/cerebrovascular_accident/cerebrovascular_accident.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/cerebrovascular_accident/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/cerebrovascular_accident/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.222248 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/ckd/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/ckd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4420 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/ckd/ckd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/ckd/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2988 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/ckd/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.222248 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/congestive_heart_failure/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/congestive_heart_failure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/congestive_heart_failure/congestive_heart_failure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/congestive_heart_failure/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/congestive_heart_failure/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.222248 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/connective_tissue_disease/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/connective_tissue_disease/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/connective_tissue_disease/connective_tissue_disease.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/connective_tissue_disease/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/connective_tissue_disease/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.222248 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/copd/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/copd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/copd/copd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/copd/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/copd/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.222248 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/dementia/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/dementia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/dementia/dementia.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/dementia/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/dementia/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.226249 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/diabetes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/diabetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4552 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/diabetes/diabetes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/diabetes/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/diabetes/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.226249 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/hemiplegia/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/hemiplegia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/hemiplegia/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/hemiplegia/hemiplegia.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/hemiplegia/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.226249 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/leukemia/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/leukemia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/leukemia/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/leukemia/leukemia.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/leukemia/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.226249 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/liver_disease/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/liver_disease/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/liver_disease/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/liver_disease/liver_disease.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/liver_disease/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.226249 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/lymphoma/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/lymphoma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/lymphoma/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/lymphoma/lymphoma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/lymphoma/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.226249 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/myocardial_infarction/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/myocardial_infarction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/myocardial_infarction/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3317 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/myocardial_infarction/myocardial_infarction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/myocardial_infarction/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.226249 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/peptic_ulcer_disease/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/peptic_ulcer_disease/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/peptic_ulcer_disease/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/peptic_ulcer_disease/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2976 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/peptic_ulcer_disease/peptic_ulcer_disease.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.226249 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/peripheral_vascular_disease/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/peripheral_vascular_disease/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/peripheral_vascular_disease/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4341 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/peripheral_vascular_disease/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3121 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/peripheral_vascular_disease/peripheral_vascular_disease.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.226249 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/solid_tumor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/solid_tumor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/solid_tumor/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/solid_tumor/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4317 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/solid_tumor/solid_tumor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/terms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.230249 edsnlp-0.9.1/edsnlp/pipelines/ner/drugs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/drugs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3487 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/drugs/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/drugs/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.230249 edsnlp-0.9.1/edsnlp/pipelines/ner/scores/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/scores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5369 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/scores/base_score.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.230249 edsnlp-0.9.1/edsnlp/pipelines/ner/scores/charlson/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/scores/charlson/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3842 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/scores/charlson/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/scores/charlson/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.230249 edsnlp-0.9.1/edsnlp/pipelines/ner/scores/elston_ellis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/scores/elston_ellis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3261 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/scores/elston_ellis/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/scores/elston_ellis/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.230249 edsnlp-0.9.1/edsnlp/pipelines/ner/scores/emergency/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/scores/emergency/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.230249 edsnlp-0.9.1/edsnlp/pipelines/ner/scores/emergency/ccmu/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/scores/emergency/ccmu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3416 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/scores/emergency/ccmu/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/scores/emergency/ccmu/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.230249 edsnlp-0.9.1/edsnlp/pipelines/ner/scores/emergency/gemsa/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/scores/emergency/gemsa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3419 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/scores/emergency/gemsa/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/scores/emergency/gemsa/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.230249 edsnlp-0.9.1/edsnlp/pipelines/ner/scores/emergency/priority/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/scores/emergency/priority/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3351 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/scores/emergency/priority/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/scores/emergency/priority/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/scores/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.230249 edsnlp-0.9.1/edsnlp/pipelines/ner/scores/sofa/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/scores/sofa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/scores/sofa/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/scores/sofa/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/scores/sofa/sofa.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.230249 edsnlp-0.9.1/edsnlp/pipelines/ner/tnm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/tnm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/tnm/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4829 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/tnm/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/tnm/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4240 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/tnm/tnm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.230249 edsnlp-0.9.1/edsnlp/pipelines/ner/umls/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/umls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4129 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/umls/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4547 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/ner/umls/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.230249 edsnlp-0.9.1/edsnlp/pipelines/qualifiers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/qualifiers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4520 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/qualifiers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/qualifiers/factories.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.234248 edsnlp-0.9.1/edsnlp/pipelines/qualifiers/family/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/qualifiers/family/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/qualifiers/family/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7001 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/qualifiers/family/family.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/qualifiers/family/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.234248 edsnlp-0.9.1/edsnlp/pipelines/qualifiers/history/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/qualifiers/history/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/qualifiers/history/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21395 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/qualifiers/history/history.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/qualifiers/history/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.234248 edsnlp-0.9.1/edsnlp/pipelines/qualifiers/hypothesis/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/qualifiers/hypothesis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/qualifiers/hypothesis/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10704 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/qualifiers/hypothesis/hypothesis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13359 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/qualifiers/hypothesis/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.234248 edsnlp-0.9.1/edsnlp/pipelines/qualifiers/negation/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/qualifiers/negation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/qualifiers/negation/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11055 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/qualifiers/negation/negation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/qualifiers/negation/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.234248 edsnlp-0.9.1/edsnlp/pipelines/qualifiers/reported_speech/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/qualifiers/reported_speech/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/qualifiers/reported_speech/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/qualifiers/reported_speech/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9096 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/qualifiers/reported_speech/reported_speech.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/terminations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.234248 edsnlp-0.9.1/edsnlp/pipelines/trainable/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/trainable/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.234248 edsnlp-0.9.1/edsnlp/pipelines/trainable/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/trainable/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14885 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/trainable/layers/crf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.234248 edsnlp-0.9.1/edsnlp/pipelines/trainable/nested_ner/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/trainable/nested_ner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/trainable/nested_ner/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12934 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/trainable/nested_ner/nested_ner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7042 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/trainable/nested_ner/stack_crf_ner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9682 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/trainable/pytorch_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.234248 edsnlp-0.9.1/edsnlp/pipelines/trainable/span_qualifier/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/trainable/span_qualifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4732 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/trainable/span_qualifier/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8149 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/trainable/span_qualifier/span_multi_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18193 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/trainable/span_qualifier/span_qualifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5889 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/pipelines/trainable/span_qualifier/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.234248 edsnlp-0.9.1/edsnlp/processing/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9653 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/processing/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/processing/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4129 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/processing/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6708 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/processing/simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/processing/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4130 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/processing/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.238248 edsnlp-0.9.1/edsnlp/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     7192 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/resources/AVC.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    95841 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/resources/adicap.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)   604577 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/resources/cim10.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (127)   136088 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/resources/drugs.json
+-rw-r--r--   0 runner    (1001) docker     (127)   200566 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/resources/verbs.csv.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.238248 edsnlp-0.9.1/edsnlp/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/utils/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/utils/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2935 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/utils/examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/utils/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8838 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/utils/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/utils/inclusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/utils/lists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/utils/merge_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/utils/numbers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/utils/regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/utils/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3877 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/utils/span_getters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10810 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/utils/training.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.238248 edsnlp-0.9.1/edsnlp/viz/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/viz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5438 2023-09-22 09:06:49.000000 edsnlp-0.9.1/edsnlp/viz/quick_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.206248 edsnlp-0.9.1/edsnlp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7359 2023-09-22 09:07:12.000000 edsnlp-0.9.1/edsnlp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16840 2023-09-22 09:07:12.000000 edsnlp-0.9.1/edsnlp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-22 09:07:12.000000 edsnlp-0.9.1/edsnlp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8217 2023-09-22 09:07:12.000000 edsnlp-0.9.1/edsnlp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2023-09-22 09:07:12.000000 edsnlp-0.9.1/edsnlp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2023-09-22 09:07:12.000000 edsnlp-0.9.1/edsnlp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.238248 edsnlp-0.9.1/notebooks/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.238248 edsnlp-0.9.1/notebooks/connectors/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2023-09-22 09:06:49.000000 edsnlp-0.9.1/notebooks/connectors/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2023-09-22 09:06:49.000000 edsnlp-0.9.1/notebooks/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.238248 edsnlp-0.9.1/notebooks/dates/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2023-09-22 09:06:49.000000 edsnlp-0.9.1/notebooks/dates/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.238248 edsnlp-0.9.1/notebooks/normalizer/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2023-09-22 09:06:49.000000 edsnlp-0.9.1/notebooks/normalizer/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.238248 edsnlp-0.9.1/notebooks/sections/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2023-09-22 09:06:49.000000 edsnlp-0.9.1/notebooks/sections/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.238248 edsnlp-0.9.1/notebooks/sentences/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2023-09-22 09:06:49.000000 edsnlp-0.9.1/notebooks/sentences/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.242249 edsnlp-0.9.1/notebooks/tokenizer/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2023-09-22 09:06:49.000000 edsnlp-0.9.1/notebooks/tokenizer/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.242249 edsnlp-0.9.1/notebooks/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2023-09-22 09:06:49.000000 edsnlp-0.9.1/notebooks/utilities/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16708 2023-09-22 09:06:49.000000 edsnlp-0.9.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.242249 edsnlp-0.9.1/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2023-09-22 09:06:49.000000 edsnlp-0.9.1/scripts/adicap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2023-09-22 09:06:49.000000 edsnlp-0.9.1/scripts/cim10.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2023-09-22 09:06:49.000000 edsnlp-0.9.1/scripts/conjugate_verbs.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2023-09-22 09:06:49.000000 edsnlp-0.9.1/scripts/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2023-09-22 09:06:49.000000 edsnlp-0.9.1/scripts/serve.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-22 09:07:12.250249 edsnlp-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2023-09-22 09:06:49.000000 edsnlp-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.242249 edsnlp-0.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2023-09-22 09:06:49.000000 edsnlp-0.9.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.242249 edsnlp-0.9.1/tests/connectors/
+-rw-r--r--   0 runner    (1001) docker     (127)     5850 2023-09-22 09:06:49.000000 edsnlp-0.9.1/tests/connectors/test_brat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2023-09-22 09:06:49.000000 edsnlp-0.9.1/tests/connectors/test_labeltool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2023-09-22 09:06:49.000000 edsnlp-0.9.1/tests/connectors/test_omop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5681 2023-09-22 09:06:49.000000 edsnlp-0.9.1/tests/extract_docs_code.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.242249 edsnlp-0.9.1/tests/matchers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2023-09-22 09:06:49.000000 edsnlp-0.9.1/tests/matchers/test_phrase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6399 2023-09-22 09:06:49.000000 edsnlp-0.9.1/tests/matchers/test_regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3021 2023-09-22 09:06:49.000000 edsnlp-0.9.1/tests/matchers/test_simstring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.242249 edsnlp-0.9.1/tests/pipelines/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.242249 edsnlp-0.9.1/tests/pipelines/core/
+-rw-r--r--   0 runner    (1001) docker     (127)    12291 2023-09-22 09:06:49.000000 edsnlp-0.9.1/tests/pipelines/core/test_contextual_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2023-09-22 09:06:49.000000 edsnlp-0.9.1/tests/pipelines/core/test_endlines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2023-09-22 09:06:49.000000 edsnlp-0.9.1/tests/pipelines/core/test_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3294 2023-09-22 09:06:49.000000 edsnlp-0.9.1/tests/pipelines/core/test_normalisation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2023-09-22 09:06:49.000000 edsnlp-0.9.1/tests/pipelines/core/test_sentences.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2023-09-22 09:06:49.000000 edsnlp-0.9.1/tests/pipelines/core/test_terminology.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.242249 edsnlp-0.9.1/tests/pipelines/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2023-09-22 09:06:49.000000 edsnlp-0.9.1/tests/pipelines/misc/test_consultation_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8993 2023-09-22 09:06:49.000000 edsnlp-0.9.1/tests/pipelines/misc/test_dates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6740 2023-09-22 09:06:49.000000 edsnlp-0.9.1/tests/pipelines/misc/test_measurements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2023-09-22 09:06:49.000000 edsnlp-0.9.1/tests/pipelines/misc/test_reason.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2023-09-22 09:06:49.000000 edsnlp-0.9.1/tests/pipelines/misc/test_sections.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2023-09-22 09:06:49.000000 edsnlp-0.9.1/tests/pipelines/misc/test_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.246249 edsnlp-0.9.1/tests/pipelines/ner/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.246249 edsnlp-0.9.1/tests/pipelines/ner/disorders/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2023-09-22 09:06:49.000000 edsnlp-0.9.1/tests/pipelines/ner/disorders/AIDS.py
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2023-09-22 09:06:49.000000 edsnlp-0.9.1/tests/pipelines/ner/disorders/CKD.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2023-09-22 09:06:49.000000 edsnlp-0.9.1/tests/pipelines/ner/disorders/COPD.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2023-09-22 09:06:49.000000 edsnlp-0.9.1/tests/pipelines/ner/disorders/alcohol.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2023-09-22 09:06:49.000000 edsnlp-0.9.1/tests/pipelines/ner/disorders/cerebrovascular_accident.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2023-09-22 09:06:49.000000 edsnlp-0.9.1/tests/pipelines/ner/disorders/congestive_heart_failure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2023-09-22 09:06:49.000000 edsnlp-0.9.1/tests/pipelines/ner/disorders/connective_tissue_disease.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2023-09-22 09:06:49.000000 edsnlp-0.9.1/tests/pipelines/ner/disorders/dementia.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2023-09-22 09:06:49.000000 edsnlp-0.9.1/tests/pipelines/ner/disorders/diabetes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2023-09-22 09:06:49.000000 edsnlp-0.9.1/tests/pipelines/ner/disorders/hemiplegia.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2023-09-22 09:06:49.000000 edsnlp-0.9.1/tests/pipelines/ner/disorders/leukemia.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2023-09-22 09:06:49.000000 edsnlp-0.9.1/tests/pipelines/ner/disorders/liver_disease.py
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2023-09-22 09:06:49.000000 edsnlp-0.9.1/tests/pipelines/ner/disorders/lymphoma.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2023-09-22 09:06:49.000000 edsnlp-0.9.1/tests/pipelines/ner/disorders/myocardial_infarction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2023-09-22 09:06:49.000000 edsnlp-0.9.1/tests/pipelines/ner/disorders/peptic_ulcer_disease.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2023-09-22 09:06:49.000000 edsnlp-0.9.1/tests/pipelines/ner/disorders/peripheral_vascular_disease.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2023-09-22 09:06:49.000000 edsnlp-0.9.1/tests/pipelines/ner/disorders/solid_tumor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4010 2023-09-22 09:06:49.000000 edsnlp-0.9.1/tests/pipelines/ner/disorders/test_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2023-09-22 09:06:49.000000 edsnlp-0.9.1/tests/pipelines/ner/disorders/tobacco.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2023-09-22 09:06:49.000000 edsnlp-0.9.1/tests/pipelines/ner/test_adicap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3494 2023-09-22 09:06:49.000000 edsnlp-0.9.1/tests/pipelines/ner/test_adicap_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2023-09-22 09:06:49.000000 edsnlp-0.9.1/tests/pipelines/ner/test_cim10.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2023-09-22 09:06:49.000000 edsnlp-0.9.1/tests/pipelines/ner/test_covid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2023-09-22 09:06:49.000000 edsnlp-0.9.1/tests/pipelines/ner/test_drugs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2023-09-22 09:06:49.000000 edsnlp-0.9.1/tests/pipelines/ner/test_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2023-09-22 09:06:49.000000 edsnlp-0.9.1/tests/pipelines/ner/test_tnm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2023-09-22 09:06:49.000000 edsnlp-0.9.1/tests/pipelines/ner/test_umls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.246249 edsnlp-0.9.1/tests/pipelines/qualifiers/
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2023-09-22 09:06:49.000000 edsnlp-0.9.1/tests/pipelines/qualifiers/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2023-09-22 09:06:49.000000 edsnlp-0.9.1/tests/pipelines/qualifiers/test_family.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2668 2023-09-22 09:06:49.000000 edsnlp-0.9.1/tests/pipelines/qualifiers/test_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2815 2023-09-22 09:06:49.000000 edsnlp-0.9.1/tests/pipelines/qualifiers/test_hypothesis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3770 2023-09-22 09:06:49.000000 edsnlp-0.9.1/tests/pipelines/qualifiers/test_negation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3960 2023-09-22 09:06:49.000000 edsnlp-0.9.1/tests/pipelines/qualifiers/test_reported_speech.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2023-09-22 09:06:49.000000 edsnlp-0.9.1/tests/pipelines/test_pipelines.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.246249 edsnlp-0.9.1/tests/pipelines/trainable/
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2023-09-22 09:06:49.000000 edsnlp-0.9.1/tests/pipelines/trainable/test_nested_ner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5077 2023-09-22 09:06:49.000000 edsnlp-0.9.1/tests/pipelines/trainable/test_span_classifier.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.246249 edsnlp-0.9.1/tests/processing/
+-rw-r--r--   0 runner    (1001) docker     (127)     5409 2023-09-22 09:06:49.000000 edsnlp-0.9.1/tests/processing/test_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2023-09-22 09:06:49.000000 edsnlp-0.9.1/tests/test_conjugator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2023-09-22 09:06:49.000000 edsnlp-0.9.1/tests/test_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2023-09-22 09:06:49.000000 edsnlp-0.9.1/tests/test_language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2023-09-22 09:06:49.000000 edsnlp-0.9.1/tests/test_span_args.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 09:07:12.246249 edsnlp-0.9.1/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2023-09-22 09:06:49.000000 edsnlp-0.9.1/tests/utils/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2023-09-22 09:06:49.000000 edsnlp-0.9.1/tests/utils/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2023-09-22 09:06:49.000000 edsnlp-0.9.1/tests/utils/test_quick_examples.py
```

### Comparing `edsnlp-0.9.0/LICENSE` & `edsnlp-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/PKG-INFO` & `edsnlp-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edsnlp
-Version: 0.9.0
+Version: 0.9.1
 Summary: A set of spaCy components to extract information from clinical notes written in French
 Author-email: Data Science - DSN APHP <perceval.wajsburt-ext@aphp.fr>
 License: Copyright 2021 Assistance Publique - Hôpitaux de Paris
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
@@ -26,15 +26,15 @@
 Requires-Dist: loguru
 Requires-Dist: pendulum>=2.1.2
 Requires-Dist: pydantic<2.0.0,>=1.10.2
 Requires-Dist: pysimstring>=1.2.1
 Requires-Dist: regex
 Requires-Dist: rich>=12.0.0
 Requires-Dist: scikit-learn>=1.0.0
-Requires-Dist: spacy<3.5.0,>=3.1
+Requires-Dist: spacy<4.0.0,>=3.1
 Requires-Dist: thinc>=8.1.10
 Requires-Dist: tqdm
 Requires-Dist: umls-downloader>=0.1.1
 Requires-Dist: numpy<1.23.2,>=1.15.0; python_version < "3.8"
 Requires-Dist: numpy>=1.15.0; python_version >= "3.8"
 Requires-Dist: pandas<2.0.0,>=1.1.0; python_version < "3.8"
 Requires-Dist: pandas<2.0.0,>=1.4.0; python_version >= "3.8"
@@ -92,15 +92,15 @@
 ```shell
 pip install edsnlp
 ```
 
 We recommend pinning the library version in your projects, or use a strict package manager like [Poetry](https://python-poetry.org/).
 
 ```shell
-pip install edsnlp==0.9.0
+pip install edsnlp==0.9.1
 ```
 
 ### A first pipeline
 
 Once you've installed the library, let's begin with a very simple example that extracts mentions of COVID19 in a text, and detects whether they are negated.
 
 ```python
```

### Comparing `edsnlp-0.9.0/README.md` & `edsnlp-0.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 ```shell
 pip install edsnlp
 ```
 
 We recommend pinning the library version in your projects, or use a strict package manager like [Poetry](https://python-poetry.org/).
 
 ```shell
-pip install edsnlp==0.9.0
+pip install edsnlp==0.9.1
 ```
 
 ### A first pipeline
 
 Once you've installed the library, let's begin with a very simple example that extracts mentions of COVID19 in a text, and detects whether they are negated.
 
 ```python
```

### Comparing `edsnlp-0.9.0/demo/app.py` & `edsnlp-0.9.1/demo/app.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/docs/scripts/autorefs/plugin.py` & `edsnlp-0.9.1/docs/scripts/autorefs/plugin.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/docs/scripts/bibtex.py` & `edsnlp-0.9.1/docs/scripts/bibtex.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/docs/scripts/griffe_ext.py` & `edsnlp-0.9.1/docs/scripts/griffe_ext.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/docs/scripts/plugin.py` & `edsnlp-0.9.1/docs/scripts/plugin.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/conjugator.py` & `edsnlp-0.9.1/edsnlp/conjugator.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/connectors/brat.py` & `edsnlp-0.9.1/edsnlp/connectors/brat.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/connectors/labeltool.py` & `edsnlp-0.9.1/edsnlp/connectors/labeltool.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/connectors/omop.py` & `edsnlp-0.9.1/edsnlp/connectors/omop.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/language.py` & `edsnlp-0.9.1/edsnlp/language.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/matchers/phrase.cpp` & `edsnlp-0.9.1/edsnlp/matchers/phrase.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 /* Generated by Cython 0.29.36 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h",
+            "/tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h",
             "/usr/include/python3.10/Python.h"
         ],
         "extra_compile_args": [
             "-std=c++11"
         ],
         "include_dirs": [
-            "/tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/core/include",
+            "/tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/core/include",
             "/usr/include/python3.10"
         ],
         "language": "c++",
         "name": "edsnlp.matchers.phrase",
         "sources": [
             "edsnlp/matchers/phrase.pyx"
         ]
@@ -1239,195 +1239,195 @@
 /* "typedefs.pxd":9
  * ctypedef uint64_t flags_t
  * ctypedef uint16_t len_t
  * ctypedef uint16_t tag_t             # <<<<<<<<<<<<<<
  */
 typedef uint16_t __pyx_t_5spacy_8typedefs_tag_t;
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":690
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":690
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":691
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":691
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":692
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":693
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":693
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":697
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":697
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":698
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":698
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":699
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":700
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":700
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":704
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":704
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":705
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":705
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":714
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":714
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":715
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":715
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":716
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":716
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":718
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":719
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":720
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":720
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":722
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":722
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":723
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":723
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":725
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":726
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":727
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -2292,42 +2292,42 @@
   std::vector<int>  first_head;
   std::vector<int>  first_tail;
   std::unordered_set<int>  *roots;
   std::unordered_map<__pyx_t_5spacy_8typedefs_hash_t,int>  *node_map;
   std::unordered_map<__pyx_t_5spacy_8typedefs_hash_t,int>  *edge_map;
 };
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":729
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":730
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":730
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":731
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":733
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":733
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -7540,15 +7540,15 @@
   __Pyx_WriteUnraisable("edsnlp.matchers.phrase.make_spanstruct", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 1);
   __Pyx_pretend_to_initialize(&__pyx_r);
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 1);
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":735
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":735
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -7559,29 +7559,29 @@
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
   __Pyx_TraceCall("PyArray_MultiIterNew1", __pyx_f[2], 735, 0, __PYX_ERR(2, 735, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":736
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":736
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 736, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":735
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -7593,15 +7593,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":738
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":738
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -7612,29 +7612,29 @@
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
   __Pyx_TraceCall("PyArray_MultiIterNew2", __pyx_f[2], 738, 0, __PYX_ERR(2, 738, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":739
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":739
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 739, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":738
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -7646,15 +7646,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":741
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":741
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -7665,29 +7665,29 @@
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
   __Pyx_TraceCall("PyArray_MultiIterNew3", __pyx_f[2], 741, 0, __PYX_ERR(2, 741, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":742
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":742
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 742, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":741
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -7699,15 +7699,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":744
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":744
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -7718,29 +7718,29 @@
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
   __Pyx_TraceCall("PyArray_MultiIterNew4", __pyx_f[2], 744, 0, __PYX_ERR(2, 744, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":745
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":745
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 745, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":744
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -7752,15 +7752,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":747
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":747
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -7771,29 +7771,29 @@
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
   __Pyx_TraceCall("PyArray_MultiIterNew5", __pyx_f[2], 747, 0, __PYX_ERR(2, 747, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":748
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":748
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 748, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":747
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -7805,15 +7805,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":750
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":750
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
@@ -7824,60 +7824,60 @@
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
   __Pyx_TraceCall("PyDataType_SHAPE", __pyx_f[2], 750, 0, __PYX_ERR(2, 750, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":751
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":751
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":752
+    /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":752
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":751
+    /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":751
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":754
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":754
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":750
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
@@ -7888,15 +7888,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":929
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":929
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -7905,33 +7905,33 @@
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_array_base", 0);
   __Pyx_TraceCall("set_array_base", __pyx_f[2], 929, 0, __PYX_ERR(2, 929, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":930
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":931
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":931
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":929
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":929
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -7940,15 +7940,15 @@
   __pyx_L1_error:;
   __Pyx_WriteUnraisable("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":933
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":933
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
@@ -7960,66 +7960,66 @@
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_array_base", 0);
   __Pyx_TraceCall("get_array_base", __pyx_f[2], 933, 0, __PYX_ERR(2, 933, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":934
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":934
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":935
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":935
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":936
+    /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":936
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":935
+    /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":935
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":937
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":937
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":933
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":933
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
@@ -8030,15 +8030,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":941
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -8056,15 +8056,15 @@
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
   __Pyx_TraceCall("import_array", __pyx_f[2], 941, 0, __PYX_ERR(2, 941, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":942
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -8072,53 +8072,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":943
+      /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":943
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 943, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":942
+      /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":944
+    /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 944, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":945
+      /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":945
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 945, __pyx_L5_except_error)
@@ -8126,30 +8126,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 945, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":942
+    /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":941
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -8165,15 +8165,15 @@
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":947
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":947
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -8191,15 +8191,15 @@
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
   __Pyx_TraceCall("import_umath", __pyx_f[2], 947, 0, __PYX_ERR(2, 947, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":948
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -8207,53 +8207,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":949
+      /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":949
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 949, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":948
+      /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":950
+    /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 950, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":951
+      /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":951
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 951, __pyx_L5_except_error)
@@ -8261,30 +8261,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 951, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":948
+    /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":947
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":947
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -8300,15 +8300,15 @@
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":953
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":953
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -8326,15 +8326,15 @@
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
   __Pyx_TraceCall("import_ufunc", __pyx_f[2], 953, 0, __PYX_ERR(2, 953, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":954
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -8342,53 +8342,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":955
+      /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":955
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 955, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":954
+      /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":956
+    /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":956
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 956, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":957
+      /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":957
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 957, __pyx_L5_except_error)
@@ -8396,30 +8396,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 957, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":954
+    /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":953
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":953
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -8435,15 +8435,15 @@
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":967
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":967
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
@@ -8453,25 +8453,25 @@
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
   __Pyx_TraceCall("is_timedelta64_object", __pyx_f[2], 967, 0, __PYX_ERR(2, 967, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":979
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":979
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":967
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":967
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
@@ -8481,15 +8481,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":982
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":982
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
@@ -8499,25 +8499,25 @@
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
   __Pyx_TraceCall("is_datetime64_object", __pyx_f[2], 982, 0, __PYX_ERR(2, 982, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":994
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":994
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":982
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":982
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
@@ -8527,15 +8527,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":997
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":997
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
@@ -8543,25 +8543,25 @@
   npy_datetime __pyx_r;
   __Pyx_TraceDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_TraceCall("get_datetime64_value", __pyx_f[2], 997, 1, __PYX_ERR(2, 997, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":1004
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":1004
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":997
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":997
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
@@ -8570,15 +8570,15 @@
   __Pyx_WriteUnraisable("numpy.get_datetime64_value", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 1);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 1);
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":1007
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":1007
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
@@ -8586,25 +8586,25 @@
   npy_timedelta __pyx_r;
   __Pyx_TraceDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_TraceCall("get_timedelta64_value", __pyx_f[2], 1007, 1, __PYX_ERR(2, 1007, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":1011
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":1011
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":1007
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":1007
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
@@ -8613,15 +8613,15 @@
   __Pyx_WriteUnraisable("numpy.get_timedelta64_value", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 1);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 1);
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":1014
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":1014
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -8629,23 +8629,23 @@
   NPY_DATETIMEUNIT __pyx_r;
   __Pyx_TraceDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_TraceCall("get_datetime64_unit", __pyx_f[2], 1014, 1, __PYX_ERR(2, 1014, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":1018
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":1018
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":1014
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":1014
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -25486,26 +25486,26 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("self.c_map cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_s_self_c_map_cannot_be_converted_t); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":945
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":945
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 945, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__10);
   __Pyx_GIVEREF(__pyx_tuple__10);
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":951
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":951
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__11 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(2, 951, __pyx_L1_error)
```

### Comparing `edsnlp-0.9.0/edsnlp/matchers/phrase.pyx` & `edsnlp-0.9.1/edsnlp/matchers/phrase.pyx`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/matchers/regex.py` & `edsnlp-0.9.1/edsnlp/matchers/regex.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/matchers/simstring.py` & `edsnlp-0.9.1/edsnlp/matchers/simstring.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/matchers/utils/offset.py` & `edsnlp-0.9.1/edsnlp/matchers/utils/offset.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/matchers/utils/text.py` & `edsnlp-0.9.1/edsnlp/matchers/utils/text.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/patch_spacy_dot_components.py` & `edsnlp-0.9.1/edsnlp/patch_spacy_dot_components.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/base.py` & `edsnlp-0.9.1/edsnlp/pipelines/base.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/core/context/context.py` & `edsnlp-0.9.1/edsnlp/pipelines/core/context/context.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/core/contextual_matcher/contextual_matcher.py` & `edsnlp-0.9.1/edsnlp/pipelines/core/contextual_matcher/contextual_matcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -307,28 +307,29 @@
                 limit_to_sentence=limit_to_sentence,
             )
 
             # Getting the matches
             assigned_list = list(matcher["matcher"].match(snippet))
 
             assigned_list = [
-                (span, span)
+                (span, span, matcher["matcher"].regex[0][0])
                 if not match.groups()
                 else (
                     span,
                     create_span(
                         doclike=snippet,
                         start_char=match.start(0),
                         end_char=match.end(0),
                         key=matcher["matcher"].regex[0][0],
                         attr=matcher["matcher"].regex[0][2],
                         alignment_mode=matcher["matcher"].regex[0][5],
                         ignore_excluded=matcher["matcher"].regex[0][3],
                         ignore_space_tokens=matcher["matcher"].regex[0][4],
                     ),
+                    matcher["matcher"].regex[0][0],
                 )
                 for (span, match) in assigned_list
             ]
 
             # assigned_list now contains tuples with
             # - the first element being the span extracted from the group
             # - the second element being the full match
@@ -336,18 +337,18 @@
             if not assigned_list:  # No match was found
                 continue
 
             for assigned in assigned_list:
                 if assigned is None:
                     continue
                 if replace_entity:
-                    replace_key = assigned[1].label_
+                    replace_key = assigned[2]
 
                 # Using he overrid `__setitem__` method from AssignDict here:
-                assigned_dict[assigned[1].label_] = {
+                assigned_dict[assigned[2]] = {
                     "span": assigned[1],  # Full span
                     "value_span": assigned[0],  # Span of the group
                     "value_text": get_text(
                         assigned[0],
                         attr=attr,
                         ignore_excluded=self.ignore_excluded,
                     ),  # Text of the group
@@ -390,21 +391,25 @@
             for replaced in kept_ents:
                 # Propagating attributes from the anchor
                 replaced._.source = source
                 replaced.label_ = self.label
 
         else:
             # Entity expansion
-            expandables = flatten([a["span"] for a in assigned_dict.values()])
+            expandables = [
+                s
+                for s in flatten([a["span"] for a in assigned_dict.values()])
+                if s is not None
+            ]
 
             if self.include_assigned and expandables:
                 span = Span(
                     span.doc,
-                    min(expandables + [span], key=attrgetter("start")).start,
-                    max(expandables + [span], key=attrgetter("end")).end,
+                    min(s.start for s in expandables + [span] if s is not None),
+                    max(s.end for s in expandables + [span] if s is not None),
                     span.label_,
                 )
 
             span._.source = source
             span.label_ = self.label
             kept_ents = [span]
```

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/core/contextual_matcher/factory.py` & `edsnlp-0.9.1/edsnlp/pipelines/core/contextual_matcher/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/core/contextual_matcher/models.py` & `edsnlp-0.9.1/edsnlp/pipelines/core/contextual_matcher/models.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/core/endlines/endlines.py` & `edsnlp-0.9.1/edsnlp/pipelines/core/endlines/endlines.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/core/endlines/functional.py` & `edsnlp-0.9.1/edsnlp/pipelines/core/endlines/functional.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/core/endlines/model.py` & `edsnlp-0.9.1/edsnlp/pipelines/core/endlines/model.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/core/matcher/factory.py` & `edsnlp-0.9.1/edsnlp/pipelines/core/matcher/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/core/matcher/matcher.py` & `edsnlp-0.9.1/edsnlp/pipelines/core/matcher/matcher.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/core/normalizer/accents/accents.py` & `edsnlp-0.9.1/edsnlp/pipelines/core/normalizer/accents/accents.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/core/normalizer/factory.py` & `edsnlp-0.9.1/edsnlp/pipelines/core/normalizer/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/core/normalizer/normalizer.py` & `edsnlp-0.9.1/edsnlp/pipelines/core/normalizer/normalizer.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/core/normalizer/pollution/patterns.py` & `edsnlp-0.9.1/edsnlp/pipelines/core/normalizer/pollution/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/core/normalizer/pollution/pollution.py` & `edsnlp-0.9.1/edsnlp/pipelines/core/normalizer/pollution/pollution.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/core/normalizer/quotes/patterns.py` & `edsnlp-0.9.1/edsnlp/pipelines/core/normalizer/quotes/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/core/normalizer/quotes/quotes.py` & `edsnlp-0.9.1/edsnlp/pipelines/core/normalizer/quotes/quotes.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/core/normalizer/remove_lowercase/factory.py` & `edsnlp-0.9.1/edsnlp/pipelines/core/normalizer/remove_lowercase/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/core/normalizer/spaces/spaces.py` & `edsnlp-0.9.1/edsnlp/pipelines/core/normalizer/spaces/spaces.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/core/sentences/factory.py` & `edsnlp-0.9.1/edsnlp/pipelines/core/sentences/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/core/sentences/sentences.cpp` & `edsnlp-0.9.1/edsnlp/pipelines/core/sentences/sentences.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 /* Generated by Cython 0.29.36 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h",
+            "/tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h",
             "/usr/include/python3.10/Python.h"
         ],
         "extra_compile_args": [
             "-std=c++11"
         ],
         "include_dirs": [
-            "/tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/core/include",
+            "/tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/core/include",
             "/usr/include/python3.10"
         ],
         "language": "c++",
         "name": "edsnlp.pipelines.core.sentences.sentences",
         "sources": [
             "edsnlp/pipelines/core/sentences/sentences.pyx"
         ]
@@ -1169,195 +1169,195 @@
   Py_ssize_t shape[8];
   Py_ssize_t strides[8];
   Py_ssize_t suboffsets[8];
 } __Pyx_memviewslice;
 #define __Pyx_MemoryView_Len(m)  (m.shape[0])
 
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":690
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":690
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":691
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":691
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":692
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":693
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":693
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":697
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":697
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":698
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":698
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":699
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":700
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":700
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":704
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":704
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":705
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":705
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":714
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":714
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":715
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":715
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":716
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":716
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":718
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":719
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":720
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":720
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":722
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":722
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":723
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":723
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":725
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":726
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":727
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1470,42 +1470,42 @@
 struct __pyx_obj_5spacy_6tokens_5token_Token;
 struct __pyx_obj_6edsnlp_9pipelines_4core_9sentences_9sentences_SentenceSegmenter;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":729
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":730
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":730
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":731
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":733
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":733
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -6111,15 +6111,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":735
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":735
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -6128,29 +6128,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":736
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":736
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 736, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":735
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -6161,15 +6161,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":738
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":738
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -6178,29 +6178,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":739
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":739
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 739, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":738
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -6211,15 +6211,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":741
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":741
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -6228,29 +6228,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":742
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":742
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 742, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":741
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -6261,15 +6261,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":744
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":744
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -6278,29 +6278,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":745
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":745
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 745, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":744
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -6311,15 +6311,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":747
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":747
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -6328,29 +6328,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":748
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":748
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 748, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":747
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -6361,212 +6361,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":750
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":750
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":751
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":751
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":752
+    /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":752
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":751
+    /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":751
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":754
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":754
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":750
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":929
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":929
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":930
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":931
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":931
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":929
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":929
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":933
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":933
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":934
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":934
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":935
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":935
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":936
+    /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":936
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":935
+    /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":935
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":937
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":937
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":933
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":933
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":941
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -6582,15 +6582,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":942
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -6598,53 +6598,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":943
+      /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":943
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 943, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":942
+      /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":944
+    /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 944, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":945
+      /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":945
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 945, __pyx_L5_except_error)
@@ -6652,30 +6652,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 945, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":942
+    /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":941
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -6690,15 +6690,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":947
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":947
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -6714,15 +6714,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":948
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -6730,53 +6730,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":949
+      /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":949
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 949, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":948
+      /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":950
+    /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 950, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":951
+      /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":951
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 951, __pyx_L5_except_error)
@@ -6784,30 +6784,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 951, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":948
+    /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":947
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":947
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -6822,15 +6822,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":953
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":953
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -6846,15 +6846,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":954
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -6862,53 +6862,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":955
+      /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":955
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 955, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":954
+      /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":956
+    /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":956
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 956, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":957
+      /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":957
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 957, __pyx_L5_except_error)
@@ -6916,30 +6916,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 957, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":954
+    /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":953
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":953
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -6954,176 +6954,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":967
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":967
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":979
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":979
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":967
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":967
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":982
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":982
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":994
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":994
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":982
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":982
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":997
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":997
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":1004
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":1004
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":997
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":997
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":1007
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":1007
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":1011
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":1011
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":1007
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":1007
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":1014
+/* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":1014
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":1018
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":1018
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":1014
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":1014
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -23292,26 +23292,26 @@
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe1e482f, 0x1527ed7, 0xbbbd922) = (capitalized_shapes_hash, endline_hash, excluded_hash, ignore_excluded, name, newline_hash, punct_chars_hash))" % __pyx_checksum)
  */
   __pyx_tuple__4 = PyTuple_Pack(3, __pyx_int_236865583, __pyx_int_22183639, __pyx_int_196860194); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":945
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":945
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(2, 945, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__5);
   __Pyx_GIVEREF(__pyx_tuple__5);
 
-  /* "../../../../../tmp/build-env-p1gtcw6v/lib/python3.10/site-packages/numpy/__init__.pxd":951
+  /* "../../../../../tmp/build-env-_fpuhfg6/lib/python3.10/site-packages/numpy/__init__.pxd":951
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(2, 951, __pyx_L1_error)
```

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/core/sentences/sentences.pyx` & `edsnlp-0.9.1/edsnlp/pipelines/core/sentences/sentences.pyx`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/core/sentences/terms.py` & `edsnlp-0.9.1/edsnlp/pipelines/core/sentences/terms.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/core/terminology/factory.py` & `edsnlp-0.9.1/edsnlp/pipelines/core/terminology/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/core/terminology/terminology.py` & `edsnlp-0.9.1/edsnlp/pipelines/core/terminology/terminology.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/factories.py` & `edsnlp-0.9.1/edsnlp/pipelines/factories.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/misc/consultation_dates/consultation_dates.py` & `edsnlp-0.9.1/edsnlp/pipelines/misc/consultation_dates/consultation_dates.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/misc/consultation_dates/factory.py` & `edsnlp-0.9.1/edsnlp/pipelines/misc/consultation_dates/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/misc/consultation_dates/patterns.py` & `edsnlp-0.9.1/edsnlp/pipelines/misc/consultation_dates/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/misc/dates/dates.py` & `edsnlp-0.9.1/edsnlp/pipelines/misc/dates/dates.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,15 +164,15 @@
         nlp: Language,
         name: str = "eds.dates",
         *,
         absolute: Optional[List[str]] = None,
         relative: Optional[List[str]] = None,
         duration: Optional[List[str]] = None,
         false_positive: Optional[List[str]] = None,
-        on_ents_only: Union[bool, str, Iterable[str]] = False,
+        on_ents_only: Union[bool, str, Iterable[str]] = None,
         span_getter: Optional[SpanGetterArg] = None,
         merge_mode: Literal["intersect", "align"] = "intersect",
         detect_periods: bool = False,
         detect_time: bool = True,
         period_proximity_threshold: int = 3,
         as_ents: bool = False,
         attr: str = "LOWER",
@@ -223,14 +223,17 @@
         if isinstance(relative, str):
             relative = [relative]
         if isinstance(duration, str):
             relative = [duration]
         if isinstance(false_positive, str):
             false_positive = [false_positive]
 
+        if on_ents_only is None and span_getter is None:
+            on_ents_only = False
+
         if on_ents_only:
             assert span_getter is None, (
                 "Cannot use both `on_ents_only` and " "`span_getter`"
             )
 
             def span_getter(doc):
                 return (span.sent for span in doc.ents)
```

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/misc/dates/factory.py` & `edsnlp-0.9.1/edsnlp/pipelines/misc/dates/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/misc/dates/models.py` & `edsnlp-0.9.1/edsnlp/pipelines/misc/dates/models.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/misc/dates/patterns/absolute.py` & `edsnlp-0.9.1/edsnlp/pipelines/misc/dates/patterns/absolute.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/misc/dates/patterns/atomic/days.py` & `edsnlp-0.9.1/edsnlp/pipelines/misc/dates/patterns/atomic/days.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/misc/dates/patterns/atomic/delimiters.py` & `edsnlp-0.9.1/edsnlp/pipelines/misc/dates/patterns/atomic/delimiters.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/misc/dates/patterns/atomic/directions.py` & `edsnlp-0.9.1/edsnlp/pipelines/misc/dates/patterns/atomic/directions.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/misc/dates/patterns/atomic/months.py` & `edsnlp-0.9.1/edsnlp/pipelines/misc/dates/patterns/atomic/months.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/misc/dates/patterns/atomic/numbers.py` & `edsnlp-0.9.1/edsnlp/pipelines/misc/dates/patterns/atomic/numbers.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/misc/dates/patterns/atomic/time.py` & `edsnlp-0.9.1/edsnlp/pipelines/misc/dates/patterns/atomic/time.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/misc/dates/patterns/relative.py` & `edsnlp-0.9.1/edsnlp/pipelines/misc/dates/patterns/relative.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/misc/measurements/factory.py` & `edsnlp-0.9.1/edsnlp/pipelines/misc/measurements/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/misc/measurements/measurements.py` & `edsnlp-0.9.1/edsnlp/pipelines/misc/measurements/measurements.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/misc/measurements/patterns.py` & `edsnlp-0.9.1/edsnlp/pipelines/misc/measurements/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/misc/reason/patterns.py` & `edsnlp-0.9.1/edsnlp/pipelines/misc/reason/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/misc/reason/reason.py` & `edsnlp-0.9.1/edsnlp/pipelines/misc/reason/reason.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/misc/sections/factory.py` & `edsnlp-0.9.1/edsnlp/pipelines/misc/sections/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/misc/sections/patterns.py` & `edsnlp-0.9.1/edsnlp/pipelines/misc/sections/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/misc/sections/sections.py` & `edsnlp-0.9.1/edsnlp/pipelines/misc/sections/sections.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/misc/tables/factory.py` & `edsnlp-0.9.1/edsnlp/pipelines/misc/tables/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/misc/tables/tables.py` & `edsnlp-0.9.1/edsnlp/pipelines/misc/tables/tables.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/ner/adicap/adicap.py` & `edsnlp-0.9.1/edsnlp/pipelines/ner/adicap/adicap.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/ner/behaviors/alcohol/alcohol.py` & `edsnlp-0.9.1/edsnlp/pipelines/ner/behaviors/alcohol/alcohol.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/ner/behaviors/alcohol/patterns.py` & `edsnlp-0.9.1/edsnlp/pipelines/ner/behaviors/alcohol/patterns.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,12 +29,12 @@
         dict(
             name="stopped",
             regex=r"(?<!non )(?<!pas )(sevr|arret|stop|ancien)",
             window=(-3, 5),
         ),
         dict(
             name="zero_after",
-            regex=r"^[a-z]*\s*:?[\s-]*(0|oui|non(?! sevr))",
+            regex=r"(?=^[a-z]*\s*:?[\s-]*(0|oui|non(?! sevr)))",
             window=6,
         ),
     ],
 )
```

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/ner/behaviors/tobacco/patterns.py` & `edsnlp-0.9.1/edsnlp/pipelines/ner/behaviors/tobacco/patterns.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,15 +28,15 @@
             dict(
                 name="stopped",
                 regex=r"(?<!non )(?<!pas )(\bex\b|sevr|arret|stop|ancien)",
                 window=(-3, 15),
             ),
             dict(
                 name="zero_after",
-                regex=r"^[a-z]*\s*:?[\s-]*(0|non(?! sevr))",
+                regex=r"(?=^[a-z]*\s*:?[\s-]*(0|non(?! sevr)))",
                 window=6,
             ),
             dict(
                 name="PA",
                 regex=rf"{QUANTITY}[^{PUNCT}]{{0,10}}{PA}|{PA}[^{PUNCT}]{{0,10}}{QUANTITY}",
                 window=(-10, 10),
                 reduce_mode="keep_first",
```

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/ner/behaviors/tobacco/tobacco.py` & `edsnlp-0.9.1/edsnlp/pipelines/ner/behaviors/tobacco/tobacco.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/ner/cim10/factory.py` & `edsnlp-0.9.1/edsnlp/pipelines/ner/cim10/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/ner/cim10/patterns.py` & `edsnlp-0.9.1/edsnlp/pipelines/ner/cim10/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/ner/covid/factory.py` & `edsnlp-0.9.1/edsnlp/pipelines/ner/covid/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/aids/aids.py` & `edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/aids/aids.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/aids/factory.py` & `edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/aids/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/aids/patterns.py` & `edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/aids/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/base.py` & `edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -82,14 +82,25 @@
         if not Span.has_extension("detailed_status"):
             Span.set_extension("detailed_status", default="PRESENT")
         if not Span.has_extension("detailled_status"):
             Span.set_extension(
                 "detailled_status",
                 getter=deprecated_getter_factory("detailed_status", "detailed_status"),
             )
+        if not Span.has_extension("negation"):
+            Span.set_extension("negation", default=None)
+        if not Span.has_extension("negation_"):
+            Span.set_extension(
+                "negation_",
+                getter=lambda item: "NEG"
+                if item._.negation is True
+                else "AFF"
+                if item._.negation is False
+                else None,
+            )
 
     def __call__(self, doc: Doc) -> Doc:
         """
         Tags entities.
 
         Parameters
         ----------
@@ -100,11 +111,13 @@
         -------
         doc : Doc
             annotated spaCy Doc object
         """
         spans = list(self.process(doc))
         for span in spans:
             span._.detailed_status = self.detailed_status_mapping[span._.status]
+            if span._.status == 0:
+                span._.negation = True
 
         self.set_spans(doc, filter_spans(spans))
 
         return doc
```

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/cerebrovascular_accident/cerebrovascular_accident.py` & `edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/cerebrovascular_accident/cerebrovascular_accident.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/cerebrovascular_accident/patterns.py` & `edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/cerebrovascular_accident/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/ckd/ckd.py` & `edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/ckd/ckd.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/ckd/patterns.py` & `edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/ckd/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/congestive_heart_failure/congestive_heart_failure.py` & `edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/congestive_heart_failure/congestive_heart_failure.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/congestive_heart_failure/patterns.py` & `edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/congestive_heart_failure/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/connective_tissue_disease/connective_tissue_disease.py` & `edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/connective_tissue_disease/connective_tissue_disease.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/connective_tissue_disease/patterns.py` & `edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/connective_tissue_disease/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/copd/copd.py` & `edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/copd/copd.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/copd/factory.py` & `edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/copd/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/copd/patterns.py` & `edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/copd/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/dementia/dementia.py` & `edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/dementia/dementia.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/dementia/patterns.py` & `edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/dementia/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/diabetes/diabetes.py` & `edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/diabetes/diabetes.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/diabetes/patterns.py` & `edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/diabetes/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/hemiplegia/hemiplegia.py` & `edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/hemiplegia/hemiplegia.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/hemiplegia/patterns.py` & `edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/hemiplegia/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/leukemia/leukemia.py` & `edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/leukemia/leukemia.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/leukemia/patterns.py` & `edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/leukemia/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/liver_disease/liver_disease.py` & `edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/liver_disease/liver_disease.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/liver_disease/patterns.py` & `edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/liver_disease/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/lymphoma/lymphoma.py` & `edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/lymphoma/lymphoma.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/lymphoma/patterns.py` & `edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/lymphoma/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/myocardial_infarction/myocardial_infarction.py` & `edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/myocardial_infarction/myocardial_infarction.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/myocardial_infarction/patterns.py` & `edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/myocardial_infarction/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/peptic_ulcer_disease/patterns.py` & `edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/peptic_ulcer_disease/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/peptic_ulcer_disease/peptic_ulcer_disease.py` & `edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/peptic_ulcer_disease/peptic_ulcer_disease.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/peripheral_vascular_disease/patterns.py` & `edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/peripheral_vascular_disease/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/peripheral_vascular_disease/peripheral_vascular_disease.py` & `edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/peripheral_vascular_disease/peripheral_vascular_disease.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/solid_tumor/patterns.py` & `edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/solid_tumor/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/solid_tumor/solid_tumor.py` & `edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/solid_tumor/solid_tumor.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/ner/disorders/terms.py` & `edsnlp-0.9.1/edsnlp/pipelines/ner/disorders/terms.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/ner/drugs/factory.py` & `edsnlp-0.9.1/edsnlp/pipelines/ner/drugs/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/ner/scores/base_score.py` & `edsnlp-0.9.1/edsnlp/pipelines/ner/scores/base_score.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/ner/scores/charlson/factory.py` & `edsnlp-0.9.1/edsnlp/pipelines/ner/scores/charlson/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/ner/scores/charlson/patterns.py` & `edsnlp-0.9.1/edsnlp/pipelines/ner/scores/charlson/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/ner/scores/elston_ellis/factory.py` & `edsnlp-0.9.1/edsnlp/pipelines/ner/scores/elston_ellis/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/ner/scores/elston_ellis/patterns.py` & `edsnlp-0.9.1/edsnlp/pipelines/ner/scores/elston_ellis/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/ner/scores/emergency/ccmu/factory.py` & `edsnlp-0.9.1/edsnlp/pipelines/ner/scores/emergency/ccmu/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/ner/scores/emergency/ccmu/patterns.py` & `edsnlp-0.9.1/edsnlp/pipelines/ner/scores/emergency/ccmu/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/ner/scores/emergency/gemsa/factory.py` & `edsnlp-0.9.1/edsnlp/pipelines/ner/scores/emergency/gemsa/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/ner/scores/emergency/gemsa/patterns.py` & `edsnlp-0.9.1/edsnlp/pipelines/ner/scores/emergency/gemsa/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/ner/scores/emergency/priority/factory.py` & `edsnlp-0.9.1/edsnlp/pipelines/ner/scores/emergency/priority/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/ner/scores/emergency/priority/patterns.py` & `edsnlp-0.9.1/edsnlp/pipelines/ner/scores/emergency/priority/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/ner/scores/factory.py` & `edsnlp-0.9.1/edsnlp/pipelines/ner/scores/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/ner/scores/sofa/factory.py` & `edsnlp-0.9.1/edsnlp/pipelines/ner/scores/sofa/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/ner/scores/sofa/patterns.py` & `edsnlp-0.9.1/edsnlp/pipelines/ner/scores/sofa/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/ner/scores/sofa/sofa.py` & `edsnlp-0.9.1/edsnlp/pipelines/ner/scores/sofa/sofa.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/ner/tnm/factory.py` & `edsnlp-0.9.1/edsnlp/pipelines/ner/tnm/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/ner/tnm/model.py` & `edsnlp-0.9.1/edsnlp/pipelines/ner/tnm/model.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/ner/tnm/patterns.py` & `edsnlp-0.9.1/edsnlp/pipelines/ner/tnm/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/ner/tnm/tnm.py` & `edsnlp-0.9.1/edsnlp/pipelines/ner/tnm/tnm.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/ner/umls/factory.py` & `edsnlp-0.9.1/edsnlp/pipelines/ner/umls/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/ner/umls/patterns.py` & `edsnlp-0.9.1/edsnlp/pipelines/ner/umls/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/qualifiers/base.py` & `edsnlp-0.9.1/edsnlp/pipelines/qualifiers/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Dict, List, Optional, Set, Union
 
 from loguru import logger
 from spacy.language import Language
 from spacy.tokens import Doc, Span
 
 from edsnlp.matchers.phrase import EDSPhraseMatcher
+from edsnlp.matchers.regex import RegexMatcher
 from edsnlp.pipelines.base import BaseComponent, SpanGetterArg, validate_span_getter
 
 
 def check_normalizer(nlp: Language) -> None:
     components = {name: component for name, component in nlp.pipeline}
     normalizer = components.get("normalizer")
 
@@ -68,25 +69,32 @@
         name: Optional[str] = None,
         *,
         attr: str,
         span_getter: SpanGetterArg,
         on_ents_only: Union[bool, str, List[str], Set[str]],
         explain: bool,
         terms: Dict[str, Optional[List[str]]],
+        regex: Dict[str, Optional[List[str]]] = {},
     ):
         super().__init__(nlp=nlp, name=name)
 
         if attr.upper() == "NORM":
             check_normalizer(nlp)
 
         self.phrase_matcher = EDSPhraseMatcher(vocab=nlp.vocab, attr=attr)
         self.phrase_matcher.build_patterns(nlp=nlp, terms=terms)
 
+        self.regex_matcher = RegexMatcher(attr=attr)
+        self.regex_matcher.build_patterns(regex=regex)
+
         self.on_ents_only = on_ents_only
 
+        if span_getter is None and on_ents_only is None:
+            on_ents_only = True
+
         if on_ents_only:
             assert isinstance(on_ents_only, (list, str, set, bool)), (
                 "The `on_ents_only` argument should be a "
                 "string, a bool, a list or a set of string"
             )
 
             assert span_getter is None, (
@@ -111,18 +119,27 @@
         List[Span]
             List of detected spans
         """
 
         if self.on_ents_only:
             sents = set([ent.sent for ent in self.get_spans(doc)])
 
-            match_iterator = (self.phrase_matcher(s, as_spans=True) for s in sents)
+            match_iterator = (
+                (
+                    *self.phrase_matcher(s, as_spans=True),
+                    *self.regex_matcher(s, as_spans=True),
+                )
+                for s in sents
+            )
 
             matches = chain.from_iterable(match_iterator)
 
         else:
-            matches = self.phrase_matcher(doc, as_spans=True)
+            matches = (
+                *self.phrase_matcher(doc, as_spans=True),
+                *self.regex_matcher(doc, as_spans=True),
+            )
 
         return list(matches)
 
     def __call__(self, doc: Doc) -> Doc:
         return self.process(doc)
```

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/qualifiers/family/factory.py` & `edsnlp-0.9.1/edsnlp/pipelines/qualifiers/family/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/qualifiers/family/family.py` & `edsnlp-0.9.1/edsnlp/pipelines/qualifiers/family/family.py`

 * *Files 6% similar despite different names*

```diff
@@ -105,15 +105,15 @@
         name: Optional[str] = "eds.family",
         *,
         attr: str = "NORM",
         family: Optional[List[str]] = None,
         termination: Optional[List[str]] = None,
         use_sections: bool = True,
         span_getter: SpanGetterArg = None,
-        on_ents_only: Union[bool, str, List[str], Set[str]] = True,
+        on_ents_only: Union[bool, str, List[str], Set[str]] = None,
         explain: bool = False,
     ):
         terms = dict(
             family=patterns.family if family is None else family,
             termination=default_termination if termination is None else termination,
         )
 
@@ -137,20 +137,24 @@
                 "Skipping that step."
             )
 
     def set_extensions(self) -> None:
         super().set_extensions()
         for cls in (Token, Span):
             if not cls.has_extension("family"):
-                cls.set_extension("family", default=False)
+                cls.set_extension("family", default=None)
 
             if not cls.has_extension("family_"):
                 cls.set_extension(
                     "family_",
-                    getter=lambda token: "FAMILY" if token._.family else "PATIENT",
+                    getter=lambda token: "FAMILY"
+                    if token._.family is True
+                    else "PATIENT"
+                    if token._.family is False
+                    else None,
                 )
 
         if not Span.has_extension("family_cues"):
             Span.set_extension("family_cues", default=[])
 
         if not Doc.has_extension("family"):
             Doc.set_extension("family", default=[])
@@ -191,23 +195,19 @@
 
             if self.on_ents_only and not ents:
                 continue
 
             cues = [m for m in sub_matches if m.label_ == "family"]
             cues.extend(sub_sections)
 
-            if not cues:
-                continue
+            family = bool(cues)
 
             if not self.on_ents_only:
                 for token in doc[start:end]:
-                    token._.family = True
+                    token._.family = token._.family or family
 
             for ent in ents:
-                ent._.family = True
+                ent._.family = family
                 if self.explain:
                     ent._.family_cues += cues
-                if not self.on_ents_only and ent._.family:
-                    for token in ent:
-                        token._.family = True
 
         return doc
```

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/qualifiers/family/patterns.py` & `edsnlp-0.9.1/edsnlp/pipelines/qualifiers/family/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/qualifiers/history/factory.py` & `edsnlp-0.9.1/edsnlp/pipelines/qualifiers/history/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/qualifiers/history/history.py` & `edsnlp-0.9.1/edsnlp/pipelines/qualifiers/history/history.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,15 +175,15 @@
         use_sections: bool = False,
         use_dates: bool = False,
         attr: str = "NORM",
         history_limit: int = 14,
         closest_dates_only: bool = True,
         exclude_birthdate: bool = True,
         span_getter: SpanGetterArg = None,
-        on_ents_only: Union[bool, str, List[str], Set[str]] = True,
+        on_ents_only: Union[bool, str, List[str], Set[str]] = None,
         explain: bool = False,
     ):
 
         terms = dict(
             history=patterns.history if history is None else history,
             termination=default_termination if termination is None else termination,
         )
@@ -237,15 +237,15 @@
                     "make sure you provide the `note_datetime` "
                     "context. "
                 )
 
     def set_extensions(self) -> None:
         for cls in (Token, Span):
             if not cls.has_extension("history"):
-                cls.set_extension("history", default=False)
+                cls.set_extension("history", default=None)
 
             if not cls.has_extension("antecedents"):
                 cls.set_extension(
                     "antecedents",
                     getter=deprecated_getter_factory("antecedents", "history"),
                 )
 
@@ -254,15 +254,19 @@
                     "antecedent",
                     getter=deprecated_getter_factory("antecedent", "history"),
                 )
 
             if not cls.has_extension("history_"):
                 cls.set_extension(
                     "history_",
-                    getter=lambda token: "ATCD" if token._.history else "CURRENT",
+                    getter=lambda token: "ATCD"
+                    if token._.history is True
+                    else "CURRENT"
+                    if token._.history is False
+                    else None,
                 )
 
             if not cls.has_extension("antecedents_"):
                 cls.set_extension(
                     "antecedents_",
                     getter=deprecated_getter_factory("antecedents_", "history_"),
                 )
@@ -517,22 +521,18 @@
                 )
                 recent_cues.extend(
                     close_recent_dates if self.closest_dates_only else sub_recent_dates
                 )
 
             history = bool(history_cues) and not bool(recent_cues)
 
-            if not self.on_ents_only:
-                for token in doc[start:end]:
-                    token._.history = token._.history or history
-
             for ent in ents:
                 ent._.history = ent._.history or history
 
                 if self.explain:
                     ent._.history_cues += history_cues
                     ent._.recent_cues += recent_cues
-                if not self.on_ents_only and ent._.history:
+                if not self.on_ents_only:
                     for token in ent:
-                        token._.history = True
+                        token._.history = token._.history or history
 
         return doc
```

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/qualifiers/hypothesis/factory.py` & `edsnlp-0.9.1/edsnlp/pipelines/qualifiers/hypothesis/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/qualifiers/hypothesis/hypothesis.py` & `edsnlp-0.9.1/edsnlp/pipelines/qualifiers/hypothesis/hypothesis.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,15 +145,15 @@
         preceding: Optional[List[str]] = None,
         following: Optional[List[str]] = None,
         verbs_eds: Optional[List[str]] = None,
         verbs_hyp: Optional[List[str]] = None,
         termination: Optional[List[str]] = None,
         attr: str = "NORM",
         span_getter: SpanGetterArg = None,
-        on_ents_only: Union[bool, str, List[str], Set[str]] = True,
+        on_ents_only: Union[bool, str, List[str], Set[str]] = None,
         within_ents: bool = False,
         explain: bool = False,
     ):
         terms = dict(
             pseudo=patterns.pseudo if pseudo is None else pseudo,
             preceding=patterns.preceding if preceding is None else preceding,
             following=patterns.following if following is None else following,
@@ -179,20 +179,24 @@
         self.within_ents = within_ents
         self.set_extensions()
 
     def set_extensions(self) -> None:
         super().set_extensions()
         for cls in (Token, Span):
             if not cls.has_extension("hypothesis"):
-                cls.set_extension("hypothesis", default=False)
+                cls.set_extension("hypothesis", default=None)
 
             if not cls.has_extension("hypothesis_"):
                 cls.set_extension(
                     "hypothesis_",
-                    getter=lambda token: "HYP" if token._.hypothesis else "CERT",
+                    getter=lambda token: "HYP"
+                    if token._.hypothesis is True
+                    else "CERT"
+                    if token._.hypothesis is False
+                    else None,
                 )
 
         if not Span.has_extension("hypothesis_cues"):
             Span.set_extension("hypothesis_cues", default=[])
 
         if not Doc.has_extension("hypothesis"):
             Doc.set_extension("hypothesis", default=[])
@@ -262,36 +266,32 @@
             sub_preceding = [m for m in sub_matches if m.label_ == "preceding"]
             sub_following = [m for m in sub_matches if m.label_ == "following"]
             # Verbs preceding negated content
             sub_preceding += [m for m in sub_matches if m.label_ == "verbs_preceding"]
             # Verbs following negated content
             sub_following += [m for m in sub_matches if m.label_ == "verbs_following"]
 
-            if not sub_preceding + sub_following:
-                continue
-
             if not self.on_ents_only:
                 for token in doc[start:end]:
                     token._.hypothesis = any(
                         m.end <= token.i for m in sub_preceding
                     ) or any(m.start > token.i for m in sub_following)
 
             for ent in ents:
                 if self.within_ents:
                     cues = [m for m in sub_preceding if m.end <= ent.end]
                     cues += [m for m in sub_following if m.start >= ent.start]
                 else:
                     cues = [m for m in sub_preceding if m.end <= ent.start]
                     cues += [m for m in sub_following if m.start >= ent.end]
 
-                hypothesis = ent._.hypothesis or bool(cues)
-
-                ent._.hypothesis = hypothesis
+                hypothesis = bool(cues)
+                ent._.hypothesis = ent._.hypothesis or hypothesis
 
                 if self.explain and hypothesis:
                     ent._.hypothesis_cues += cues
 
                 if not self.on_ents_only and hypothesis:
                     for token in ent:
-                        token._.hypothesis = True
+                        token._.hypothesis = token._.hypothesis or hypothesis
 
         return doc
```

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/qualifiers/hypothesis/patterns.py` & `edsnlp-0.9.1/edsnlp/pipelines/qualifiers/hypothesis/patterns.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,32 @@
-from typing import List
-
-pseudo: List[str] = [
+pseudo = [
     "aucun doute",
     "même si",
     "pas de condition",
     "pas de doute",
     "sans aucun doute",
     "sans condition",
     "sans risque",
 ]
 
-confirmation: List[str] = [
+confirmation = [
     "certain",
     "certaine",
     "certainement",
     "certaines",
     "certains",
     "confirmer",
     "évidemment",
     "évident",
     "évidente",
     "montrer que",
     "visiblement",
 ]
 
-preceding: List[str] = [
+preceding = [
     "à condition",
     "à la condition que",
     "à moins que",
     "au cas où",
     "conditionnellement",
     "discret",
     "discrets",
@@ -71,15 +69,15 @@
     "s'il",
     "soit",
     "sous condition",
     "sous réserve",
     "suspicion",
 ]
 
-following: List[str] = [
+following = [
     "?",
     "envisageable",
     "envisageables",
     "hypothétique",
     "hypothétiquement",
     "hypothétiques",
     "pas certain",
@@ -99,27 +97,27 @@
     "potentiel",
     "potentielle",
     "potentiels",
     "probable",
     "probables",
 ]
 
-verbs_hyp: List[str] = [
+verbs_hyp = [
     "douter",
     "envisager",
     "explorer",
     "rechercher",
     "s'apparenter",
     "sembler",
     "soupçonner",
     "suggérer",
     "suspecter",
 ]
 
-verbs_eds: List[str] = [
+verbs_eds = [
     "abandonner",
     "abolir",
     "aborder",
     "accepter",
     "accidenter",
     "accompagnemer",
     "accompagner",
```

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/qualifiers/negation/factory.py` & `edsnlp-0.9.1/edsnlp/pipelines/qualifiers/negation/factory.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from edsnlp.utils.deprecation import deprecated_factory
 
 from .negation import NegationQualifier
 
 DEFAULT_CONFIG = dict(
     pseudo=None,
     preceding=None,
+    preceding_regex=None,
     following=None,
     verbs=None,
     termination=None,
     attr="NORM",
     span_getter=None,
     on_ents_only=True,
     within_ents=False,
```

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/qualifiers/negation/negation.py` & `edsnlp-0.9.1/edsnlp/pipelines/qualifiers/negation/negation.py`

 * *Files 3% similar despite different names*

```diff
@@ -105,14 +105,16 @@
         The component name.
     attr : str
         spaCy's attribute to use
     pseudo : Optional[List[str]]
         List of pseudo negation cues.
     preceding : Optional[List[str]]
         List of preceding negation cues
+    preceding_regex : Optional[List[str]]
+        List of preceding negation cues, but as regexes.
     following : Optional[List[str]]
         List of following negation cues.
     verbs : Optional[List[str]]
         List of negation verbs.
     termination : Optional[List[str]]
         List of termination terms.
     span_getter : SpanGetterArg
@@ -139,62 +141,73 @@
     def __init__(
         self,
         nlp: Language,
         name: Optional[str] = "eds.negation",
         *,
         pseudo: Optional[List[str]] = None,
         preceding: Optional[List[str]] = None,
+        preceding_regex: Optional[List[str]] = None,
         following: Optional[List[str]] = None,
         verbs: Optional[List[str]] = None,
         termination: Optional[List[str]] = None,
         attr: str = "NORM",
         span_getter: SpanGetterArg = None,
-        on_ents_only: Union[bool, str, List[str], Set[str]] = True,
+        on_ents_only: Union[bool, str, List[str], Set[str]] = None,
         within_ents: bool = False,
         explain: bool = False,
     ):
         terms = dict(
             pseudo=patterns.pseudo if pseudo is None else pseudo,
             preceding=patterns.preceding if preceding is None else preceding,
             following=patterns.following if following is None else following,
             termination=default_termination if termination is None else termination,
             verbs=patterns.verbs if verbs is None else verbs,
         )
         terms["verbs_preceding"], terms["verbs_following"] = self.load_verbs(
             terms["verbs"]
         )
+        regex = dict(
+            preceding=preceding_regex
+            if preceding_regex is not None
+            else patterns.preceding_regex,
+        )
 
         super().__init__(
             nlp=nlp,
             name=name,
             attr=attr,
             explain=explain,
             terms=terms,
+            regex=regex,
             on_ents_only=on_ents_only,
             span_getter=span_getter,
         )
 
         self.within_ents = within_ents
         self.set_extensions()
 
     def set_extensions(self) -> None:
         super().set_extensions()
         for cls in (Token, Span):
             if not cls.has_extension("negation"):
-                cls.set_extension("negation", default=False)
+                cls.set_extension("negation", default=None)
 
             if not cls.has_extension("negated"):
                 cls.set_extension(
                     "negated", getter=deprecated_getter_factory("negated", "negation")
                 )
 
             if not cls.has_extension("negation_"):
                 cls.set_extension(
                     "negation_",
-                    getter=lambda token: "NEG" if token._.negation else "AFF",
+                    getter=lambda token: "NEG"
+                    if token._.negation is True
+                    else "AFF"
+                    if token._.negation is False
+                    else None,
                 )
 
             if not cls.has_extension("polarity_"):
                 cls.set_extension(
                     "polarity_",
                     getter=deprecated_getter_factory("polarity_", "negation_"),
                 )
@@ -260,34 +273,32 @@
             sub_preceding = [m for m in sub_matches if m.label_ == "preceding"]
             sub_following = [m for m in sub_matches if m.label_ == "following"]
             # Verbs preceding negated content
             sub_preceding += [m for m in sub_matches if m.label_ == "verbs_preceding"]
             # Verbs following negated content
             sub_following += [m for m in sub_matches if m.label_ == "verbs_following"]
 
-            if not sub_preceding + sub_following:
-                continue
-
             if not self.on_ents_only:
                 for token in doc[start:end]:
-                    token._.negation = any(
-                        m.end <= token.i for m in sub_preceding
-                    ) or any(m.start > token.i for m in sub_following)
+                    token._.negation = (
+                        token._.negation
+                        or any(m.end <= token.i for m in sub_preceding)
+                        or any(m.start > token.i for m in sub_following)
+                    )
 
             for ent in ents:
                 if self.within_ents:
                     cues = [m for m in sub_preceding if m.end <= ent.end]
                     cues += [m for m in sub_following if m.start >= ent.start]
                 else:
                     cues = [m for m in sub_preceding if m.end <= ent.start]
                     cues += [m for m in sub_following if m.start >= ent.end]
 
-                negation = ent._.negation or bool(cues)
-
-                ent._.negation = negation
+                negation = bool(cues)
+                ent._.negation = ent._.negation or negation
 
                 if self.explain and negation:
                     ent._.negation_cues += cues
 
                 if not self.on_ents_only and negation:
                     for token in ent:
                         token._.negation = True
```

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/qualifiers/negation/patterns.py` & `edsnlp-0.9.1/edsnlp/pipelines/qualifiers/negation/patterns.py`

 * *Files 12% similar despite different names*

```diff
@@ -79,14 +79,19 @@
     "peu d'arguments en",
     "peu d'arguments pour",
     "plus d'aspect de",
     "sans",
     "symptôme atypique",
 ]
 
+preceding_regex = [
+    # ne (up to 3 words separated by spaces or newlines) pas/point/...
+    r"ne(?=[ \n]*(?:\w*[ \n]*){3}(?:pas|point|ni|aucun|jamais|rien))"
+]
+
 following: List[str] = [
     ":0",
     ": 0",
     ":non",
     ": non",
     "absent",
     "absente",
```

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/qualifiers/reported_speech/factory.py` & `edsnlp-0.9.1/edsnlp/pipelines/qualifiers/reported_speech/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/qualifiers/reported_speech/patterns.py` & `edsnlp-0.9.1/edsnlp/pipelines/qualifiers/reported_speech/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/qualifiers/reported_speech/reported_speech.py` & `edsnlp-0.9.1/edsnlp/pipelines/qualifiers/reported_speech/reported_speech.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
         pseudo: Optional[List[str]] = None,
         preceding: Optional[List[str]] = None,
         following: Optional[List[str]] = None,
         quotation: Optional[List[str]] = None,
         verbs: Optional[List[str]] = None,
         attr: str = "NORM",
         span_getter: SpanGetterArg = None,
-        on_ents_only: Union[bool, str, List[str], Set[str]] = True,
+        on_ents_only: Union[bool, str, List[str], Set[str]] = None,
         within_ents: bool = False,
         explain: bool = False,
     ):
 
         terms = dict(
             pseudo=pseudo or [],
             preceding=patterns.preceding if preceding is None else preceding,
@@ -147,22 +147,24 @@
         self.set_extensions()
 
     def set_extensions(self) -> None:
         super().set_extensions()
 
         for cls in (Token, Span):
             if not cls.has_extension("reported_speech"):
-                cls.set_extension("reported_speech", default=False)
+                cls.set_extension("reported_speech", default=None)
 
             if not cls.has_extension("reported_speech_"):
                 cls.set_extension(
                     "reported_speech_",
                     getter=lambda token: "REPORTED"
-                    if token._.reported_speech
-                    else "DIRECT",
+                    if token._.reported_speech is True
+                    else "DIRECT"
+                    if token._.reported_speech is False
+                    else None,
                 )
 
         if not Span.has_extension("reported_speech_cues"):
             Span.set_extension("reported_speech_cues", default=[])
 
     def load_verbs(self, verbs: List[str]) -> List[str]:
         """
@@ -221,17 +223,14 @@
                 continue
 
             sub_preceding = [m for m in sub_matches if m.label_ == "preceding"]
             sub_following = [m for m in sub_matches if m.label_ == "following"]
             sub_verbs = [m for m in sub_matches if m.label_ == "verbs"]
             sub_quotation = [m for m in sub_matches if m.label_ == "quotation"]
 
-            if not sub_preceding + sub_following + sub_verbs + sub_quotation:
-                continue
-
             if not self.on_ents_only:
                 for token in doc[start:end]:
                     token._.reported_speech = (
                         any(m.end <= token.i for m in sub_preceding + sub_verbs)
                         or any(m.start > token.i for m in sub_following)
                         or any(
                             ((m.start < token.i) & (m.end > token.i + 1))
@@ -248,16 +247,16 @@
 
                 cues += [
                     m
                     for m in sub_quotation
                     if (m.start < ent.start) & (m.end > ent.end)
                 ]
 
-                reported_speech = ent._.reported_speech or bool(cues)
-                ent._.reported_speech = reported_speech
+                reported_speech = bool(cues)
+                ent._.reported_speech = ent._.reported_speech or reported_speech
 
                 if self.explain and reported_speech:
                     ent._.reported_speech_cues += cues
 
                 if not self.on_ents_only and reported_speech:
                     for token in ent:
                         token._.reported_speech = True
```

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/terminations.py` & `edsnlp-0.9.1/edsnlp/pipelines/terminations.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/trainable/layers/crf.py` & `edsnlp-0.9.1/edsnlp/pipelines/trainable/layers/crf.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/trainable/nested_ner/factory.py` & `edsnlp-0.9.1/edsnlp/pipelines/trainable/nested_ner/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/trainable/nested_ner/nested_ner.py` & `edsnlp-0.9.1/edsnlp/pipelines/trainable/nested_ner/nested_ner.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/trainable/nested_ner/stack_crf_ner.py` & `edsnlp-0.9.1/edsnlp/pipelines/trainable/nested_ner/stack_crf_ner.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/trainable/pytorch_wrapper.py` & `edsnlp-0.9.1/edsnlp/pipelines/trainable/pytorch_wrapper.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/trainable/span_qualifier/factory.py` & `edsnlp-0.9.1/edsnlp/pipelines/trainable/span_qualifier/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/trainable/span_qualifier/span_multi_classifier.py` & `edsnlp-0.9.1/edsnlp/pipelines/trainable/span_qualifier/span_multi_classifier.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/trainable/span_qualifier/span_qualifier.py` & `edsnlp-0.9.1/edsnlp/pipelines/trainable/span_qualifier/span_qualifier.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/pipelines/trainable/span_qualifier/utils.py` & `edsnlp-0.9.1/edsnlp/pipelines/trainable/span_qualifier/utils.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/processing/distributed.py` & `edsnlp-0.9.1/edsnlp/processing/distributed.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/processing/helpers.py` & `edsnlp-0.9.1/edsnlp/processing/helpers.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/processing/parallel.py` & `edsnlp-0.9.1/edsnlp/processing/parallel.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/processing/simple.py` & `edsnlp-0.9.1/edsnlp/processing/simple.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/processing/wrapper.py` & `edsnlp-0.9.1/edsnlp/processing/wrapper.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/resources/AVC.csv.gz` & `edsnlp-0.9.1/edsnlp/resources/AVC.csv.gz`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/resources/adicap.json.gz` & `edsnlp-0.9.1/edsnlp/resources/adicap.json.gz`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/resources/cim10.csv.gz` & `edsnlp-0.9.1/edsnlp/resources/cim10.csv.gz`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/resources/drugs.json` & `edsnlp-0.9.1/edsnlp/resources/drugs.json`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/resources/verbs.csv.gz` & `edsnlp-0.9.1/edsnlp/resources/verbs.csv.gz`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/utils/colors.py` & `edsnlp-0.9.1/edsnlp/utils/colors.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/utils/deprecation.py` & `edsnlp-0.9.1/edsnlp/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/utils/examples.py` & `edsnlp-0.9.1/edsnlp/utils/examples.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/utils/filter.py` & `edsnlp-0.9.1/edsnlp/utils/filter.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/utils/inclusion.py` & `edsnlp-0.9.1/edsnlp/utils/inclusion.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/utils/merge_configs.py` & `edsnlp-0.9.1/edsnlp/utils/merge_configs.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/utils/numbers.py` & `edsnlp-0.9.1/edsnlp/utils/numbers.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/utils/regex.py` & `edsnlp-0.9.1/edsnlp/utils/regex.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/utils/resources.py` & `edsnlp-0.9.1/edsnlp/utils/resources.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/utils/span_getters.py` & `edsnlp-0.9.1/edsnlp/utils/span_getters.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/utils/training.py` & `edsnlp-0.9.1/edsnlp/utils/training.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp/viz/quick_examples.py` & `edsnlp-0.9.1/edsnlp/viz/quick_examples.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp.egg-info/PKG-INFO` & `edsnlp-0.9.1/edsnlp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edsnlp
-Version: 0.9.0
+Version: 0.9.1
 Summary: A set of spaCy components to extract information from clinical notes written in French
 Author-email: Data Science - DSN APHP <perceval.wajsburt-ext@aphp.fr>
 License: Copyright 2021 Assistance Publique - Hôpitaux de Paris
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
@@ -26,15 +26,15 @@
 Requires-Dist: loguru
 Requires-Dist: pendulum>=2.1.2
 Requires-Dist: pydantic<2.0.0,>=1.10.2
 Requires-Dist: pysimstring>=1.2.1
 Requires-Dist: regex
 Requires-Dist: rich>=12.0.0
 Requires-Dist: scikit-learn>=1.0.0
-Requires-Dist: spacy<3.5.0,>=3.1
+Requires-Dist: spacy<4.0.0,>=3.1
 Requires-Dist: thinc>=8.1.10
 Requires-Dist: tqdm
 Requires-Dist: umls-downloader>=0.1.1
 Requires-Dist: numpy<1.23.2,>=1.15.0; python_version < "3.8"
 Requires-Dist: numpy>=1.15.0; python_version >= "3.8"
 Requires-Dist: pandas<2.0.0,>=1.1.0; python_version < "3.8"
 Requires-Dist: pandas<2.0.0,>=1.4.0; python_version >= "3.8"
@@ -92,15 +92,15 @@
 ```shell
 pip install edsnlp
 ```
 
 We recommend pinning the library version in your projects, or use a strict package manager like [Poetry](https://python-poetry.org/).
 
 ```shell
-pip install edsnlp==0.9.0
+pip install edsnlp==0.9.1
 ```
 
 ### A first pipeline
 
 Once you've installed the library, let's begin with a very simple example that extracts mentions of COVID19 in a text, and detects whether they are negated.
 
 ```python
```

### Comparing `edsnlp-0.9.0/edsnlp.egg-info/SOURCES.txt` & `edsnlp-0.9.1/edsnlp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp.egg-info/entry_points.txt` & `edsnlp-0.9.1/edsnlp.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/edsnlp.egg-info/requires.txt` & `edsnlp-0.9.1/edsnlp.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 loguru
 pendulum>=2.1.2
 pydantic<2.0.0,>=1.10.2
 pysimstring>=1.2.1
 regex
 rich>=12.0.0
 scikit-learn>=1.0.0
-spacy<3.5.0,>=3.1
+spacy<4.0.0,>=3.1
 thinc>=8.1.10
 tqdm
 umls-downloader>=0.1.1
 
 [:python_version < "3.8"]
 numpy<1.23.2,>=1.15.0
 pandas<2.0.0,>=1.1.0
```

### Comparing `edsnlp-0.9.0/pyproject.toml` & `edsnlp-0.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     "loguru",
     "pendulum>=2.1.2",
     "pydantic>=1.10.2,<2.0.0",
     "pysimstring>=1.2.1",
     "regex",
     "rich>=12.0.0",
     "scikit-learn>=1.0.0",
-    "spacy>=3.1,<3.5.0",
+    "spacy>=3.1,<4.0.0",
     "thinc>=8.1.10",
     "tqdm",
     "umls-downloader>=0.1.1",
     "numpy>=1.15.0,<1.23.2; python_version<'3.8'",
     "numpy>=1.15.0; python_version>='3.8'",
     "pandas>=1.1.0,<2.0.0; python_version<'3.8'",
     "pandas>=1.4.0,<2.0.0; python_version>='3.8'",
```

### Comparing `edsnlp-0.9.0/scripts/adicap.py` & `edsnlp-0.9.1/scripts/adicap.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/scripts/cim10.py` & `edsnlp-0.9.1/scripts/cim10.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/scripts/conjugate_verbs.py` & `edsnlp-0.9.1/scripts/conjugate_verbs.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/scripts/serve.py` & `edsnlp-0.9.1/scripts/serve.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/setup.py` & `edsnlp-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/tests/conftest.py` & `edsnlp-0.9.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/tests/connectors/test_brat.py` & `edsnlp-0.9.1/tests/connectors/test_brat.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/tests/connectors/test_omop.py` & `edsnlp-0.9.1/tests/connectors/test_omop.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/tests/extract_docs_code.py` & `edsnlp-0.9.1/tests/extract_docs_code.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/tests/matchers/test_phrase.py` & `edsnlp-0.9.1/tests/matchers/test_phrase.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/tests/matchers/test_regex.py` & `edsnlp-0.9.1/tests/matchers/test_regex.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/tests/matchers/test_simstring.py` & `edsnlp-0.9.1/tests/matchers/test_simstring.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/tests/pipelines/core/test_contextual_matcher.py` & `edsnlp-0.9.1/tests/pipelines/core/test_contextual_matcher.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/tests/pipelines/core/test_endlines.py` & `edsnlp-0.9.1/tests/pipelines/core/test_endlines.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/tests/pipelines/core/test_matcher.py` & `edsnlp-0.9.1/tests/pipelines/core/test_matcher.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/tests/pipelines/core/test_normalisation.py` & `edsnlp-0.9.1/tests/pipelines/core/test_normalisation.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/tests/pipelines/core/test_sentences.py` & `edsnlp-0.9.1/tests/pipelines/core/test_sentences.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/tests/pipelines/core/test_terminology.py` & `edsnlp-0.9.1/tests/pipelines/core/test_terminology.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/tests/pipelines/misc/test_consultation_date.py` & `edsnlp-0.9.1/tests/pipelines/misc/test_consultation_date.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/tests/pipelines/misc/test_dates.py` & `edsnlp-0.9.1/tests/pipelines/misc/test_dates.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/tests/pipelines/misc/test_measurements.py` & `edsnlp-0.9.1/tests/pipelines/misc/test_measurements.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/tests/pipelines/misc/test_reason.py` & `edsnlp-0.9.1/tests/pipelines/misc/test_reason.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/tests/pipelines/misc/test_sections.py` & `edsnlp-0.9.1/tests/pipelines/misc/test_sections.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/tests/pipelines/misc/test_tables.py` & `edsnlp-0.9.1/tests/pipelines/misc/test_tables.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/tests/pipelines/ner/disorders/CKD.py` & `edsnlp-0.9.1/tests/pipelines/ner/disorders/CKD.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/tests/pipelines/ner/disorders/COPD.py` & `edsnlp-0.9.1/tests/pipelines/ner/disorders/COPD.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/tests/pipelines/ner/disorders/alcohol.py` & `edsnlp-0.9.1/tests/pipelines/ner/disorders/alcohol.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/tests/pipelines/ner/disorders/diabetes.py` & `edsnlp-0.9.1/tests/pipelines/ner/disorders/diabetes.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/tests/pipelines/ner/disorders/peripheral_vascular_disease.py` & `edsnlp-0.9.1/tests/pipelines/ner/disorders/peripheral_vascular_disease.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/tests/pipelines/ner/disorders/solid_tumor.py` & `edsnlp-0.9.1/tests/pipelines/ner/disorders/solid_tumor.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/tests/pipelines/ner/disorders/test_all.py` & `edsnlp-0.9.1/tests/pipelines/ner/disorders/test_all.py`

 * *Files 19% similar despite different names*

```diff
@@ -109,7 +109,30 @@
     expect = DisorderTester(
         disorder,
         normalized_nlp,
         **result,
     )
 
     expect.check()
+
+
+def test_behavior_negation(blank_nlp):
+    blank_nlp.add_pipe("eds.normalizer")
+    blank_nlp.add_pipe("eds.tobacco")
+    blank_nlp.add_pipe("eds.alcohol")
+    blank_nlp.add_pipe("eds.negation")
+
+    negated_texts = [
+        "Le patient ne fume aucun truc.",
+        "Le patient fume 0 PA.",
+        "Il ne boit pas d'alcool." "Boit très rarement de l'alcool.",
+    ]
+
+    positive_texts = ["Le patient ne fume que le soir.", "Il ne boit plus d'alcool."]
+
+    for text in negated_texts:
+        doc = blank_nlp(text)
+        assert doc.ents[0]._.negation is True, text
+
+    for text in positive_texts:
+        doc = blank_nlp(text)
+        assert doc.ents[0]._.negation is False, text
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `edsnlp-0.9.0/tests/pipelines/ner/disorders/tobacco.py` & `edsnlp-0.9.1/tests/pipelines/ner/disorders/tobacco.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/tests/pipelines/ner/test_adicap.py` & `edsnlp-0.9.1/tests/pipelines/ner/test_adicap.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/tests/pipelines/ner/test_adicap_decoder.py` & `edsnlp-0.9.1/tests/pipelines/ner/test_adicap_decoder.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/tests/pipelines/ner/test_cim10.py` & `edsnlp-0.9.1/tests/pipelines/ner/test_cim10.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/tests/pipelines/ner/test_drugs.py` & `edsnlp-0.9.1/tests/pipelines/ner/test_drugs.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/tests/pipelines/ner/test_score.py` & `edsnlp-0.9.1/tests/pipelines/ner/test_score.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/tests/pipelines/ner/test_tnm.py` & `edsnlp-0.9.1/tests/pipelines/ner/test_tnm.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/tests/pipelines/ner/test_umls.py` & `edsnlp-0.9.1/tests/pipelines/ner/test_umls.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/tests/pipelines/qualifiers/test_family.py` & `edsnlp-0.9.1/tests/pipelines/qualifiers/test_family.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/tests/pipelines/qualifiers/test_history.py` & `edsnlp-0.9.1/tests/pipelines/qualifiers/test_history.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/tests/pipelines/qualifiers/test_hypothesis.py` & `edsnlp-0.9.1/tests/pipelines/qualifiers/test_hypothesis.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/tests/pipelines/qualifiers/test_negation.py` & `edsnlp-0.9.1/tests/pipelines/qualifiers/test_negation.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,17 @@
     "il y a des <ent polarity_=AFF>métastases</ent>",
     "aucun doute sur les <ent polarity_=AFF>métastases</ent>",
     "il n'y a pas de <ent polarity_=NEG>métastases</ent>",
     "il n'y a pas d' <ent polarity_=NEG>métastases</ent>",
     "il n'y a pas d'<ent polarity_=NEG>métastases</ent>",
     "il n'y a pas d'amélioration de la <ent negated=false>maladie</ent>",
     "<ent negated=true>maladie écartée",
+    "Le patient ne <ent negated=true>fume</ent> pas.",
+    "Le patient ne <ent negated=true>fume vraiment vraiment</ent> pas.",
+    "Le patient ne <ent negated=false>fume</ent> que des cigares.",
 ]
 
 
 @fixture
 def negation_factory(blank_nlp):
 
     default_config = dict(
```

### Comparing `edsnlp-0.9.0/tests/pipelines/qualifiers/test_reported_speech.py` & `edsnlp-0.9.1/tests/pipelines/qualifiers/test_reported_speech.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/tests/pipelines/trainable/test_nested_ner.py` & `edsnlp-0.9.1/tests/pipelines/trainable/test_nested_ner.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/tests/pipelines/trainable/test_span_classifier.py` & `edsnlp-0.9.1/tests/pipelines/trainable/test_span_classifier.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/tests/processing/test_processing.py` & `edsnlp-0.9.1/tests/processing/test_processing.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/tests/test_conjugator.py` & `edsnlp-0.9.1/tests/test_conjugator.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/tests/test_docs.py` & `edsnlp-0.9.1/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/tests/test_language.py` & `edsnlp-0.9.1/tests/test_language.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/tests/test_span_args.py` & `edsnlp-0.9.1/tests/test_span_args.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/tests/utils/test_examples.py` & `edsnlp-0.9.1/tests/utils/test_examples.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/tests/utils/test_filter.py` & `edsnlp-0.9.1/tests/utils/test_filter.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.9.0/tests/utils/test_quick_examples.py` & `edsnlp-0.9.1/tests/utils/test_quick_examples.py`

 * *Files identical despite different names*

