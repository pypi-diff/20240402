# Comparing `tmp/yadg-5.0.1.tar.gz` & `tmp/yadg-5.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yadg-5.0.1.tar", last modified: Tue Dec  5 10:12:36 2023, max compression
+gzip compressed data, was "yadg-5.0.2.tar", last modified: Wed Dec 13 17:47:33 2023, max compression
```

## Comparing `yadg-5.0.1.tar` & `yadg-5.0.2.tar`

### file list

```diff
@@ -1,118 +1,116 @@
-drwxrwxrwx   0        0        0        0 2023-12-05 10:12:36.608371 yadg-5.0.1/
--rw-rw-rw-   0        0        0    35823 2023-11-29 07:58:45.000000 yadg-5.0.1/LICENSE
--rw-rw-rw-   0        0        0       53 2023-11-29 07:58:45.000000 yadg-5.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     4671 2023-12-05 10:12:36.607646 yadg-5.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3340 2023-11-29 07:58:45.000000 yadg-5.0.1/README.md
--rw-rw-rw-   0        0        0      211 2023-12-05 10:12:36.611550 yadg-5.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1765 2023-12-04 15:48:16.000000 yadg-5.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-12-05 10:12:36.278156 yadg-5.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-12-05 10:12:36.612546 yadg-5.0.1/src/yadg/
--rw-rw-rw-   0        0        0      204 2023-11-29 07:58:45.000000 yadg-5.0.1/src/yadg/__init__.py
--rw-rw-rw-   0        0        0      518 2023-12-05 10:12:36.612546 yadg-5.0.1/src/yadg/_version.py
-drwxrwxrwx   0        0        0        0 2023-12-05 10:12:36.389707 yadg-5.0.1/src/yadg/core/
--rw-rw-rw-   0        0        0     7307 2023-11-29 07:58:45.000000 yadg-5.0.1/src/yadg/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-05 10:12:36.406504 yadg-5.0.1/src/yadg/dgutils/
--rw-rw-rw-   0        0        0      490 2023-11-29 07:58:45.000000 yadg-5.0.1/src/yadg/dgutils/__init__.py
--rw-rw-rw-   0        0        0     2273 2023-11-29 07:58:45.000000 yadg-5.0.1/src/yadg/dgutils/btools.py
--rw-rw-rw-   0        0        0    13680 2023-11-29 07:58:45.000000 yadg-5.0.1/src/yadg/dgutils/dateutils.py
--rw-rw-rw-   0        0        0      676 2023-11-29 07:58:45.000000 yadg-5.0.1/src/yadg/dgutils/helpers.py
--rw-rw-rw-   0        0        0     2299 2023-11-29 07:58:45.000000 yadg-5.0.1/src/yadg/dgutils/pintutils.py
--rw-rw-rw-   0        0        0     6070 2023-11-29 07:58:45.000000 yadg-5.0.1/src/yadg/dgutils/utils.py
-drwxrwxrwx   0        0        0        0 2023-12-05 10:12:36.407938 yadg-5.0.1/src/yadg/extractors/
--rw-rw-rw-   0        0        0     2908 2023-11-29 07:58:45.000000 yadg-5.0.1/src/yadg/extractors/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-05 10:12:36.409526 yadg-5.0.1/src/yadg/extractors/agilentch/
--rw-rw-rw-   0        0        0      166 2023-11-29 07:58:45.000000 yadg-5.0.1/src/yadg/extractors/agilentch/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-05 10:12:36.411594 yadg-5.0.1/src/yadg/extractors/agilentdx/
--rw-rw-rw-   0        0        0      166 2023-11-29 07:58:45.000000 yadg-5.0.1/src/yadg/extractors/agilentdx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-05 10:12:36.413503 yadg-5.0.1/src/yadg/extractors/eclabmpr/
--rw-rw-rw-   0        0        0      167 2023-11-29 07:58:45.000000 yadg-5.0.1/src/yadg/extractors/eclabmpr/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-05 10:12:36.416505 yadg-5.0.1/src/yadg/extractors/eclabmpt/
--rw-rw-rw-   0        0        0      167 2023-11-29 07:58:45.000000 yadg-5.0.1/src/yadg/extractors/eclabmpt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-05 10:12:36.418506 yadg-5.0.1/src/yadg/extractors/panalyticalxrdml/
--rw-rw-rw-   0        0        0      185 2023-11-29 07:58:45.000000 yadg-5.0.1/src/yadg/extractors/panalyticalxrdml/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-05 10:12:36.420504 yadg-5.0.1/src/yadg/extractors/phispe/
--rw-rw-rw-   0        0        0      155 2023-11-29 07:58:45.000000 yadg-5.0.1/src/yadg/extractors/phispe/__init__.py
--rw-rw-rw-   0        0        0     6218 2023-11-29 07:58:45.000000 yadg-5.0.1/src/yadg/main.py
-drwxrwxrwx   0        0        0        0 2023-12-05 10:12:36.425434 yadg-5.0.1/src/yadg/parsers/
--rw-rw-rw-   0        0        0        0 2023-11-29 07:58:45.000000 yadg-5.0.1/src/yadg/parsers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-05 10:12:36.433464 yadg-5.0.1/src/yadg/parsers/basiccsv/
--rw-rw-rw-   0        0        0     1570 2023-11-29 07:58:45.000000 yadg-5.0.1/src/yadg/parsers/basiccsv/__init__.py
--rw-rw-rw-   0        0        0     7011 2023-11-29 07:58:45.000000 yadg-5.0.1/src/yadg/parsers/basiccsv/main.py
-drwxrwxrwx   0        0        0        0 2023-12-05 10:12:36.447451 yadg-5.0.1/src/yadg/parsers/chromdata/
--rw-rw-rw-   0        0        0     2750 2023-11-29 07:58:45.000000 yadg-5.0.1/src/yadg/parsers/chromdata/__init__.py
--rw-rw-rw-   0        0        0     8006 2023-12-04 15:48:16.000000 yadg-5.0.1/src/yadg/parsers/chromdata/empalccsv.py
--rw-rw-rw-   0        0        0     7849 2023-12-04 15:48:16.000000 yadg-5.0.1/src/yadg/parsers/chromdata/empalcxlsx.py
--rw-rw-rw-   0        0        0     4399 2023-11-29 07:58:45.000000 yadg-5.0.1/src/yadg/parsers/chromdata/fusioncsv.py
--rw-rw-rw-   0        0        0     4925 2023-11-29 07:58:45.000000 yadg-5.0.1/src/yadg/parsers/chromdata/fusionjson.py
--rw-rw-rw-   0        0        0     2374 2023-11-29 07:58:45.000000 yadg-5.0.1/src/yadg/parsers/chromdata/fusionzip.py
-drwxrwxrwx   0        0        0        0 2023-12-05 10:12:36.477074 yadg-5.0.1/src/yadg/parsers/chromtrace/
--rw-rw-rw-   0        0        0     3586 2023-11-29 07:58:45.000000 yadg-5.0.1/src/yadg/parsers/chromtrace/__init__.py
--rw-rw-rw-   0        0        0     4838 2023-11-29 07:58:45.000000 yadg-5.0.1/src/yadg/parsers/chromtrace/agilentch.py
--rw-rw-rw-   0        0        0     6454 2023-11-29 07:58:45.000000 yadg-5.0.1/src/yadg/parsers/chromtrace/agilentcsv.py
--rw-rw-rw-   0        0        0     3309 2023-11-29 07:58:45.000000 yadg-5.0.1/src/yadg/parsers/chromtrace/agilentdx.py
--rw-rw-rw-   0        0        0     6167 2023-11-29 07:58:45.000000 yadg-5.0.1/src/yadg/parsers/chromtrace/ezchromasc.py
--rw-rw-rw-   0        0        0     3660 2023-11-29 07:58:45.000000 yadg-5.0.1/src/yadg/parsers/chromtrace/fusionjson.py
--rw-rw-rw-   0        0        0     2591 2023-11-29 07:58:45.000000 yadg-5.0.1/src/yadg/parsers/chromtrace/fusionzip.py
-drwxrwxrwx   0        0        0        0 2023-12-05 10:12:36.479081 yadg-5.0.1/src/yadg/parsers/dummy/
--rw-rw-rw-   0        0        0     2648 2023-11-29 07:58:45.000000 yadg-5.0.1/src/yadg/parsers/dummy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-05 10:12:36.490815 yadg-5.0.1/src/yadg/parsers/electrochem/
--rw-rw-rw-   0        0        0     2672 2023-11-29 07:58:45.000000 yadg-5.0.1/src/yadg/parsers/electrochem/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-05 10:12:36.523410 yadg-5.0.1/src/yadg/parsers/electrochem/eclabcommon/
--rw-rw-rw-   0        0        0        0 2023-11-29 07:58:45.000000 yadg-5.0.1/src/yadg/parsers/electrochem/eclabcommon/__init__.py
--rw-rw-rw-   0        0        0     7097 2023-11-29 07:58:45.000000 yadg-5.0.1/src/yadg/parsers/electrochem/eclabcommon/mpr_columns.py
--rw-rw-rw-   0        0        0     3339 2023-11-29 07:58:45.000000 yadg-5.0.1/src/yadg/parsers/electrochem/eclabcommon/mpt_columns.py
--rw-rw-rw-   0        0        0     4573 2023-09-03 19:08:33.000000 yadg-5.0.1/src/yadg/parsers/electrochem/eclabcommon/parameters.yml
--rw-rw-rw-   0        0        0    35159 2023-11-29 07:58:45.000000 yadg-5.0.1/src/yadg/parsers/electrochem/eclabcommon/techniques.py
--rw-rw-rw-   0        0        0     4642 2023-09-03 18:29:02.000000 yadg-5.0.1/src/yadg/parsers/electrochem/eclabcommon/techniques.yml
--rw-rw-rw-   0        0        0    22055 2023-11-29 07:58:45.000000 yadg-5.0.1/src/yadg/parsers/electrochem/eclabmpr.py
--rw-rw-rw-   0        0        0     9735 2023-11-29 07:58:45.000000 yadg-5.0.1/src/yadg/parsers/electrochem/eclabmpt.py
--rw-rw-rw-   0        0        0     4553 2023-11-29 07:58:45.000000 yadg-5.0.1/src/yadg/parsers/electrochem/tomatojson.py
-drwxrwxrwx   0        0        0        0 2023-12-05 10:12:36.528413 yadg-5.0.1/src/yadg/parsers/flowdata/
--rw-rw-rw-   0        0        0     1026 2023-11-29 07:58:45.000000 yadg-5.0.1/src/yadg/parsers/flowdata/__init__.py
--rw-rw-rw-   0        0        0     6855 2023-12-04 15:48:16.000000 yadg-5.0.1/src/yadg/parsers/flowdata/drycal.py
--rw-rw-rw-   0        0        0     1848 2023-11-29 07:58:46.000000 yadg-5.0.1/src/yadg/parsers/flowdata/main.py
-drwxrwxrwx   0        0        0        0 2023-12-05 10:12:36.533410 yadg-5.0.1/src/yadg/parsers/masstrace/
--rw-rw-rw-   0        0        0     2675 2023-11-29 07:58:46.000000 yadg-5.0.1/src/yadg/parsers/masstrace/__init__.py
--rw-rw-rw-   0        0        0     9445 2023-11-29 07:58:46.000000 yadg-5.0.1/src/yadg/parsers/masstrace/quadstarsac.py
-drwxrwxrwx   0        0        0        0 2023-12-05 10:12:36.537415 yadg-5.0.1/src/yadg/parsers/meascsv/
--rw-rw-rw-   0        0        0     3433 2023-11-29 07:58:46.000000 yadg-5.0.1/src/yadg/parsers/meascsv/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-05 10:12:36.541409 yadg-5.0.1/src/yadg/parsers/qftrace/
--rw-rw-rw-   0        0        0     1903 2023-11-29 07:58:46.000000 yadg-5.0.1/src/yadg/parsers/qftrace/__init__.py
--rw-rw-rw-   0        0        0     3981 2023-11-29 07:58:46.000000 yadg-5.0.1/src/yadg/parsers/qftrace/labviewcsv.py
-drwxrwxrwx   0        0        0        0 2023-12-05 10:12:36.545410 yadg-5.0.1/src/yadg/parsers/xpstrace/
--rw-rw-rw-   0        0        0     1696 2023-11-29 07:58:46.000000 yadg-5.0.1/src/yadg/parsers/xpstrace/__init__.py
--rw-rw-rw-   0        0        0    12037 2023-11-29 07:58:46.000000 yadg-5.0.1/src/yadg/parsers/xpstrace/phispe.py
-drwxrwxrwx   0        0        0        0 2023-12-05 10:12:36.560356 yadg-5.0.1/src/yadg/parsers/xrdtrace/
--rw-rw-rw-   0        0        0     2108 2023-11-29 07:58:46.000000 yadg-5.0.1/src/yadg/parsers/xrdtrace/__init__.py
--rw-rw-rw-   0        0        0     1962 2023-11-29 07:58:46.000000 yadg-5.0.1/src/yadg/parsers/xrdtrace/common.py
--rw-rw-rw-   0        0        0     5098 2023-11-29 07:58:46.000000 yadg-5.0.1/src/yadg/parsers/xrdtrace/panalyticalcsv.py
--rw-rw-rw-   0        0        0     8775 2023-11-29 07:58:46.000000 yadg-5.0.1/src/yadg/parsers/xrdtrace/panalyticalxrdml.py
--rw-rw-rw-   0        0        0     2513 2023-11-29 07:58:46.000000 yadg-5.0.1/src/yadg/parsers/xrdtrace/panalyticalxy.py
--rw-rw-rw-   0        0        0     7749 2023-11-29 07:58:46.000000 yadg-5.0.1/src/yadg/subcommands.py
-drwxrwxrwx   0        0        0        0 2023-12-05 10:12:36.604373 yadg-5.0.1/src/yadg.egg-info/
--rw-rw-rw-   0        0        0     4671 2023-12-05 10:12:36.000000 yadg-5.0.1/src/yadg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2978 2023-12-05 10:12:36.000000 yadg-5.0.1/src/yadg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-05 10:12:36.000000 yadg-5.0.1/src/yadg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-12-05 10:12:36.000000 yadg-5.0.1/src/yadg.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      288 2023-12-05 10:12:36.000000 yadg-5.0.1/src/yadg.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-12-05 10:12:36.000000 yadg-5.0.1/src/yadg.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-12-05 10:12:36.601463 yadg-5.0.1/tests/
--rw-rw-rw-   0        0        0     9838 2023-11-29 07:58:46.000000 yadg-5.0.1/tests/test_basiccsv.py
--rw-rw-rw-   0        0        0     8998 2023-12-04 15:48:16.000000 yadg-5.0.1/tests/test_chromdata.py
--rw-rw-rw-   0        0        0     6975 2023-11-29 07:58:46.000000 yadg-5.0.1/tests/test_chromtrace.py
--rw-rw-rw-   0        0        0     4013 2023-12-04 15:48:16.000000 yadg-5.0.1/tests/test_drycal.py
--rw-rw-rw-   0        0        0     4019 2023-11-29 07:58:46.000000 yadg-5.0.1/tests/test_dummy.py
--rw-rw-rw-   0        0        0    18144 2023-11-29 07:58:46.000000 yadg-5.0.1/tests/test_electrochem.py
--rw-rw-rw-   0        0        0     1255 2023-11-29 07:58:46.000000 yadg-5.0.1/tests/test_encoding.py
--rw-rw-rw-   0        0        0     4876 2023-11-29 07:58:46.000000 yadg-5.0.1/tests/test_externaldate.py
--rw-rw-rw-   0        0        0      851 2023-11-29 07:58:46.000000 yadg-5.0.1/tests/test_extract.py
--rw-rw-rw-   0        0        0     1637 2023-11-29 07:58:46.000000 yadg-5.0.1/tests/test_locale.py
--rw-rw-rw-   0        0        0     1717 2023-11-29 07:58:46.000000 yadg-5.0.1/tests/test_masstrace.py
--rw-rw-rw-   0        0        0      699 2023-11-29 07:58:46.000000 yadg-5.0.1/tests/test_meascsv.py
--rw-rw-rw-   0        0        0      760 2023-11-29 07:58:46.000000 yadg-5.0.1/tests/test_preset.py
--rw-rw-rw-   0        0        0     2082 2023-11-29 07:58:46.000000 yadg-5.0.1/tests/test_qftrace.py
--rw-rw-rw-   0        0        0     2116 2023-11-29 07:58:46.000000 yadg-5.0.1/tests/test_timezones.py
--rw-rw-rw-   0        0        0     1682 2023-11-29 07:58:46.000000 yadg-5.0.1/tests/test_xpstrace.py
--rw-rw-rw-   0        0        0     1338 2023-11-29 07:58:46.000000 yadg-5.0.1/tests/test_xrdtrace.py
--rw-rw-rw-   0        0        0     7212 2023-11-29 07:58:46.000000 yadg-5.0.1/tests/test_yadg.py
--rw-rw-rw-   0        0        0    83365 2023-11-29 07:58:47.000000 yadg-5.0.1/versioneer.py
+drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2023-12-13 17:47:33.362087 yadg-5.0.2/
+-rw-r--r--   0 kraus     (1000) kraus     (1000)    35149 2023-09-01 17:04:55.000000 yadg-5.0.2/LICENSE
+-rw-r--r--   0 kraus     (1000) kraus     (1000)       51 2023-09-01 17:04:55.000000 yadg-5.0.2/MANIFEST.in
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     4574 2023-12-13 17:47:33.362087 yadg-5.0.2/PKG-INFO
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     3281 2023-12-13 17:42:48.000000 yadg-5.0.2/README.md
+-rw-r--r--   0 kraus     (1000) kraus     (1000)      199 2023-12-13 17:47:33.362087 yadg-5.0.2/setup.cfg
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     1704 2023-12-13 17:42:48.000000 yadg-5.0.2/setup.py
+drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2023-12-13 17:47:33.332087 yadg-5.0.2/src/
+drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2023-12-13 17:47:33.362087 yadg-5.0.2/src/yadg/
+-rw-r--r--   0 kraus     (1000) kraus     (1000)      196 2023-09-01 17:04:55.000000 yadg-5.0.2/src/yadg/__init__.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)      497 2023-12-13 17:47:33.362087 yadg-5.0.2/src/yadg/_version.py
+drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2023-12-13 17:47:33.338754 yadg-5.0.2/src/yadg/core/
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     7116 2023-09-01 17:04:55.000000 yadg-5.0.2/src/yadg/core/__init__.py
+drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2023-12-13 17:47:33.342087 yadg-5.0.2/src/yadg/dgutils/
+-rw-r--r--   0 kraus     (1000) kraus     (1000)      472 2023-09-01 17:04:55.000000 yadg-5.0.2/src/yadg/dgutils/__init__.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     2198 2023-12-13 17:42:48.000000 yadg-5.0.2/src/yadg/dgutils/btools.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)    13263 2023-09-01 17:04:55.000000 yadg-5.0.2/src/yadg/dgutils/dateutils.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)      651 2023-09-01 17:04:55.000000 yadg-5.0.2/src/yadg/dgutils/helpers.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     2218 2023-09-01 17:04:55.000000 yadg-5.0.2/src/yadg/dgutils/pintutils.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     5897 2023-09-01 17:04:55.000000 yadg-5.0.2/src/yadg/dgutils/utils.py
+drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2023-12-13 17:47:33.342087 yadg-5.0.2/src/yadg/extractors/
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     2814 2023-12-13 17:42:48.000000 yadg-5.0.2/src/yadg/extractors/__init__.py
+drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2023-12-13 17:47:33.342087 yadg-5.0.2/src/yadg/extractors/agilentch/
+-rw-r--r--   0 kraus     (1000) kraus     (1000)      158 2023-09-01 17:04:55.000000 yadg-5.0.2/src/yadg/extractors/agilentch/__init__.py
+drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2023-12-13 17:47:33.342087 yadg-5.0.2/src/yadg/extractors/agilentdx/
+-rw-r--r--   0 kraus     (1000) kraus     (1000)      158 2023-09-01 17:04:55.000000 yadg-5.0.2/src/yadg/extractors/agilentdx/__init__.py
+drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2023-12-13 17:47:33.342087 yadg-5.0.2/src/yadg/extractors/eclabmpr/
+-rw-r--r--   0 kraus     (1000) kraus     (1000)      159 2023-09-01 17:04:55.000000 yadg-5.0.2/src/yadg/extractors/eclabmpr/__init__.py
+drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2023-12-13 17:47:33.342087 yadg-5.0.2/src/yadg/extractors/eclabmpt/
+-rw-r--r--   0 kraus     (1000) kraus     (1000)      159 2023-09-01 17:04:55.000000 yadg-5.0.2/src/yadg/extractors/eclabmpt/__init__.py
+drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2023-12-13 17:47:33.342087 yadg-5.0.2/src/yadg/extractors/panalyticalxrdml/
+-rw-r--r--   0 kraus     (1000) kraus     (1000)      177 2023-09-01 17:04:55.000000 yadg-5.0.2/src/yadg/extractors/panalyticalxrdml/__init__.py
+drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2023-12-13 17:47:33.342087 yadg-5.0.2/src/yadg/extractors/phispe/
+-rw-r--r--   0 kraus     (1000) kraus     (1000)      147 2023-09-01 17:04:55.000000 yadg-5.0.2/src/yadg/extractors/phispe/__init__.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     6017 2023-12-13 17:42:48.000000 yadg-5.0.2/src/yadg/main.py
+drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2023-12-13 17:47:33.345421 yadg-5.0.2/src/yadg/parsers/
+-rw-r--r--   0 kraus     (1000) kraus     (1000)        0 2023-09-01 17:04:55.000000 yadg-5.0.2/src/yadg/parsers/__init__.py
+drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2023-12-13 17:47:33.345421 yadg-5.0.2/src/yadg/parsers/basiccsv/
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     1521 2023-12-13 17:42:48.000000 yadg-5.0.2/src/yadg/parsers/basiccsv/__init__.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     6781 2023-12-13 17:42:48.000000 yadg-5.0.2/src/yadg/parsers/basiccsv/main.py
+drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2023-12-13 17:47:33.345421 yadg-5.0.2/src/yadg/parsers/chromdata/
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     2658 2023-12-13 17:42:48.000000 yadg-5.0.2/src/yadg/parsers/chromdata/__init__.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     7782 2023-12-13 17:42:48.000000 yadg-5.0.2/src/yadg/parsers/chromdata/empalccsv.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     7630 2023-12-13 17:42:48.000000 yadg-5.0.2/src/yadg/parsers/chromdata/empalcxlsx.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     4254 2023-12-13 17:42:48.000000 yadg-5.0.2/src/yadg/parsers/chromdata/fusioncsv.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     4769 2023-12-13 17:42:48.000000 yadg-5.0.2/src/yadg/parsers/chromdata/fusionjson.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     2307 2023-12-13 17:42:48.000000 yadg-5.0.2/src/yadg/parsers/chromdata/fusionzip.py
+drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2023-12-13 17:47:33.348754 yadg-5.0.2/src/yadg/parsers/chromtrace/
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     3470 2023-12-13 17:42:48.000000 yadg-5.0.2/src/yadg/parsers/chromtrace/__init__.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     4677 2023-12-13 17:42:48.000000 yadg-5.0.2/src/yadg/parsers/chromtrace/agilentch.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     6274 2023-12-13 17:42:48.000000 yadg-5.0.2/src/yadg/parsers/chromtrace/agilentcsv.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     3223 2023-12-13 17:42:48.000000 yadg-5.0.2/src/yadg/parsers/chromtrace/agilentdx.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     5998 2023-12-13 17:42:48.000000 yadg-5.0.2/src/yadg/parsers/chromtrace/ezchromasc.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     3549 2023-12-13 17:42:48.000000 yadg-5.0.2/src/yadg/parsers/chromtrace/fusionjson.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     2510 2023-12-13 17:42:48.000000 yadg-5.0.2/src/yadg/parsers/chromtrace/fusionzip.py
+drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2023-12-13 17:47:33.348754 yadg-5.0.2/src/yadg/parsers/dummy/
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     2551 2023-12-13 17:42:48.000000 yadg-5.0.2/src/yadg/parsers/dummy/__init__.py
+drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2023-12-13 17:47:33.348754 yadg-5.0.2/src/yadg/parsers/electrochem/
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     2585 2023-12-13 17:42:48.000000 yadg-5.0.2/src/yadg/parsers/electrochem/__init__.py
+drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2023-12-13 17:47:33.348754 yadg-5.0.2/src/yadg/parsers/electrochem/eclabcommon/
+-rw-r--r--   0 kraus     (1000) kraus     (1000)        0 2023-09-01 17:04:55.000000 yadg-5.0.2/src/yadg/parsers/electrochem/eclabcommon/__init__.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     6904 2023-09-01 17:04:55.000000 yadg-5.0.2/src/yadg/parsers/electrochem/eclabcommon/mpr_columns.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     3252 2023-09-01 17:04:55.000000 yadg-5.0.2/src/yadg/parsers/electrochem/eclabcommon/mpt_columns.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)    33969 2023-12-13 17:43:31.000000 yadg-5.0.2/src/yadg/parsers/electrochem/eclabcommon/techniques.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)    21452 2023-12-13 17:42:48.000000 yadg-5.0.2/src/yadg/parsers/electrochem/eclabmpr.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     9455 2023-12-13 17:42:48.000000 yadg-5.0.2/src/yadg/parsers/electrochem/eclabmpt.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     4411 2023-09-01 17:04:55.000000 yadg-5.0.2/src/yadg/parsers/electrochem/tomatojson.py
+drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2023-12-13 17:47:33.348754 yadg-5.0.2/src/yadg/parsers/flowdata/
+-rw-r--r--   0 kraus     (1000) kraus     (1000)      988 2023-09-01 17:04:55.000000 yadg-5.0.2/src/yadg/parsers/flowdata/__init__.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     6627 2023-12-13 17:42:48.000000 yadg-5.0.2/src/yadg/parsers/flowdata/drycal.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     1781 2023-12-13 17:42:48.000000 yadg-5.0.2/src/yadg/parsers/flowdata/main.py
+drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2023-12-13 17:47:33.352087 yadg-5.0.2/src/yadg/parsers/masstrace/
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     2586 2023-12-13 17:42:48.000000 yadg-5.0.2/src/yadg/parsers/masstrace/__init__.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     9181 2023-12-13 17:42:48.000000 yadg-5.0.2/src/yadg/parsers/masstrace/quadstarsac.py
+drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2023-12-13 17:47:33.352087 yadg-5.0.2/src/yadg/parsers/meascsv/
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     3317 2023-12-13 17:42:48.000000 yadg-5.0.2/src/yadg/parsers/meascsv/__init__.py
+drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2023-12-13 17:47:33.352087 yadg-5.0.2/src/yadg/parsers/qftrace/
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     1833 2023-09-01 17:04:55.000000 yadg-5.0.2/src/yadg/parsers/qftrace/__init__.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     3851 2023-12-13 17:42:48.000000 yadg-5.0.2/src/yadg/parsers/qftrace/labviewcsv.py
+drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2023-12-13 17:47:33.352087 yadg-5.0.2/src/yadg/parsers/xpstrace/
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     1627 2023-09-01 17:04:55.000000 yadg-5.0.2/src/yadg/parsers/xpstrace/__init__.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)    11662 2023-12-13 17:42:48.000000 yadg-5.0.2/src/yadg/parsers/xpstrace/phispe.py
+drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2023-12-13 17:47:33.352087 yadg-5.0.2/src/yadg/parsers/xrdtrace/
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     2034 2023-12-13 17:42:48.000000 yadg-5.0.2/src/yadg/parsers/xrdtrace/__init__.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     1900 2023-09-01 17:04:55.000000 yadg-5.0.2/src/yadg/parsers/xrdtrace/common.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     4928 2023-12-13 17:42:48.000000 yadg-5.0.2/src/yadg/parsers/xrdtrace/panalyticalcsv.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     8497 2023-12-13 17:42:48.000000 yadg-5.0.2/src/yadg/parsers/xrdtrace/panalyticalxrdml.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     2426 2023-12-13 17:42:48.000000 yadg-5.0.2/src/yadg/parsers/xrdtrace/panalyticalxy.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     7544 2023-12-13 17:42:48.000000 yadg-5.0.2/src/yadg/subcommands.py
+drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2023-12-13 17:47:33.358754 yadg-5.0.2/src/yadg.egg-info/
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     4574 2023-12-13 17:47:33.000000 yadg-5.0.2/src/yadg.egg-info/PKG-INFO
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     2866 2023-12-13 17:47:33.000000 yadg-5.0.2/src/yadg.egg-info/SOURCES.txt
+-rw-r--r--   0 kraus     (1000) kraus     (1000)        1 2023-12-13 17:47:33.000000 yadg-5.0.2/src/yadg.egg-info/dependency_links.txt
+-rw-r--r--   0 kraus     (1000) kraus     (1000)       49 2023-12-13 17:47:33.000000 yadg-5.0.2/src/yadg.egg-info/entry_points.txt
+-rw-r--r--   0 kraus     (1000) kraus     (1000)      288 2023-12-13 17:47:33.000000 yadg-5.0.2/src/yadg.egg-info/requires.txt
+-rw-r--r--   0 kraus     (1000) kraus     (1000)        5 2023-12-13 17:47:33.000000 yadg-5.0.2/src/yadg.egg-info/top_level.txt
+drwxr-xr-x   0 kraus     (1000) kraus     (1000)        0 2023-12-13 17:47:33.358754 yadg-5.0.2/tests/
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     9557 2023-09-01 17:04:55.000000 yadg-5.0.2/tests/test_basiccsv.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     8734 2023-12-13 17:42:48.000000 yadg-5.0.2/tests/test_chromdata.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     6767 2023-09-01 17:04:55.000000 yadg-5.0.2/tests/test_chromtrace.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     3894 2023-12-13 17:42:48.000000 yadg-5.0.2/tests/test_drycal.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     3891 2023-09-01 17:04:55.000000 yadg-5.0.2/tests/test_dummy.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)    18511 2023-12-13 17:43:31.000000 yadg-5.0.2/tests/test_electrochem.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     1216 2023-09-01 17:04:55.000000 yadg-5.0.2/tests/test_encoding.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     4728 2023-09-01 17:04:55.000000 yadg-5.0.2/tests/test_externaldate.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)      826 2023-09-01 17:04:55.000000 yadg-5.0.2/tests/test_extract.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     1582 2023-12-13 17:42:48.000000 yadg-5.0.2/tests/test_locale.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     1652 2023-09-01 17:04:56.000000 yadg-5.0.2/tests/test_masstrace.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)      678 2023-09-01 17:04:56.000000 yadg-5.0.2/tests/test_meascsv.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)      730 2023-09-01 17:04:56.000000 yadg-5.0.2/tests/test_preset.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     2013 2023-09-01 17:04:56.000000 yadg-5.0.2/tests/test_qftrace.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     2058 2023-09-01 17:04:56.000000 yadg-5.0.2/tests/test_timezones.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     1623 2023-09-01 17:04:56.000000 yadg-5.0.2/tests/test_xpstrace.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     1293 2023-09-01 17:04:56.000000 yadg-5.0.2/tests/test_xrdtrace.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)     6999 2023-12-13 17:42:48.000000 yadg-5.0.2/tests/test_yadg.py
+-rw-r--r--   0 kraus     (1000) kraus     (1000)    81176 2023-09-01 17:04:56.000000 yadg-5.0.2/versioneer.py
```

### Comparing `yadg-5.0.1/LICENSE` & `yadg-5.0.2/LICENSE`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,674 +1,674 @@
-                    GNU GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-                            Preamble
-
-  The GNU General Public License is a free, copyleft license for
-software and other kinds of works.
-
-  The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works.  By contrast,
-the GNU General Public License is intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users.  We, the Free Software Foundation, use the
-GNU General Public License for most of our software; it applies also to
-any other work released this way by its authors.  You can apply it to
-your programs, too.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-  To protect your rights, we need to prevent others from denying you
-these rights or asking you to surrender the rights.  Therefore, you have
-certain responsibilities if you distribute copies of the software, or if
-you modify it: responsibilities to respect the freedom of others.
-
-  For example, if you distribute copies of such a program, whether
-gratis or for a fee, you must pass on to the recipients the same
-freedoms that you received.  You must make sure that they, too, receive
-or can get the source code.  And you must show them these terms so they
-know their rights.
-
-  Developers that use the GNU GPL protect your rights with two steps:
-(1) assert copyright on the software, and (2) offer you this License
-giving you legal permission to copy, distribute and/or modify it.
-
-  For the developers' and authors' protection, the GPL clearly explains
-that there is no warranty for this free software.  For both users' and
-authors' sake, the GPL requires that modified versions be marked as
-changed, so that their problems will not be attributed erroneously to
-authors of previous versions.
-
-  Some devices are designed to deny users access to install or run
-modified versions of the software inside them, although the manufacturer
-can do so.  This is fundamentally incompatible with the aim of
-protecting users' freedom to change the software.  The systematic
-pattern of such abuse occurs in the area of products for individuals to
-use, which is precisely where it is most unacceptable.  Therefore, we
-have designed this version of the GPL to prohibit the practice for those
-products.  If such problems arise substantially in other domains, we
-stand ready to extend this provision to those domains in future versions
-of the GPL, as needed to protect the freedom of users.
-
-  Finally, every program is threatened constantly by software patents.
-States should not allow patents to restrict development and use of
-software on general-purpose computers, but in those that do, we wish to
-avoid the special danger that patents applied to a free program could
-make it effectively proprietary.  To prevent this, the GPL assures that
-patents cannot be used to render the program non-free.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-                       TERMS AND CONDITIONS
-
-  0. Definitions.
-
-  "This License" refers to version 3 of the GNU General Public License.
-
-  "Copyright" also means copyright-like laws that apply to other kinds of
-works, such as semiconductor masks.
-
-  "The Program" refers to any copyrightable work licensed under this
-License.  Each licensee is addressed as "you".  "Licensees" and
-"recipients" may be individuals or organizations.
-
-  To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of an
-exact copy.  The resulting work is called a "modified version" of the
-earlier work or a work "based on" the earlier work.
-
-  A "covered work" means either the unmodified Program or a work based
-on the Program.
-
-  To "propagate" a work means to do anything with it that, without
-permission, would make you directly or secondarily liable for
-infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy.  Propagation includes copying,
-distribution (with or without modification), making available to the
-public, and in some countries other activities as well.
-
-  To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies.  Mere interaction with a user through
-a computer network, with no transfer of a copy, is not conveying.
-
-  An interactive user interface displays "Appropriate Legal Notices"
-to the extent that it includes a convenient and prominently visible
-feature that (1) displays an appropriate copyright notice, and (2)
-tells the user that there is no warranty for the work (except to the
-extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License.  If
-the interface presents a list of user commands or options, such as a
-menu, a prominent item in the list meets this criterion.
-
-  1. Source Code.
-
-  The "source code" for a work means the preferred form of the work
-for making modifications to it.  "Object code" means any non-source
-form of a work.
-
-  A "Standard Interface" means an interface that either is an official
-standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that
-is widely used among developers working in that language.
-
-  The "System Libraries" of an executable work include anything, other
-than the work as a whole, that (a) is included in the normal form of
-packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that
-Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form.  A
-"Major Component", in this context, means a major essential component
-(kernel, window system, and so on) of the specific operating system
-(if any) on which the executable work runs, or a compiler used to
-produce the work, or an object code interpreter used to run it.
-
-  The "Corresponding Source" for a work in object code form means all
-the source code needed to generate, install, and (for an executable
-work) run the object code and to modify the work, including scripts to
-control those activities.  However, it does not include the work's
-System Libraries, or general-purpose tools or generally available free
-programs which are used unmodified in performing those activities but
-which are not part of the work.  For example, Corresponding Source
-includes interface definition files associated with source files for
-the work, and the source code for shared libraries and dynamically
-linked subprograms that the work is specifically designed to require,
-such as by intimate data communication or control flow between those
-subprograms and other parts of the work.
-
-  The Corresponding Source need not include anything that users
-can regenerate automatically from other parts of the Corresponding
-Source.
-
-  The Corresponding Source for a work in source code form is that
-same work.
-
-  2. Basic Permissions.
-
-  All rights granted under this License are granted for the term of
-copyright on the Program, and are irrevocable provided the stated
-conditions are met.  This License explicitly affirms your unlimited
-permission to run the unmodified Program.  The output from running a
-covered work is covered by this License only if the output, given its
-content, constitutes a covered work.  This License acknowledges your
-rights of fair use or other equivalent, as provided by copyright law.
-
-  You may make, run and propagate covered works that you do not
-convey, without conditions so long as your license otherwise remains
-in force.  You may convey covered works to others for the sole purpose
-of having them make modifications exclusively for you, or provide you
-with facilities for running those works, provided that you comply with
-the terms of this License in conveying all material for which you do
-not control copyright.  Those thus making or running the covered works
-for you must do so exclusively on your behalf, under your direction
-and control, on terms that prohibit them from making any copies of
-your copyrighted material outside their relationship with you.
-
-  Conveying under any other circumstances is permitted solely under
-the conditions stated below.  Sublicensing is not allowed; section 10
-makes it unnecessary.
-
-  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-  No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article
-11 of the WIPO copyright treaty adopted on 20 December 1996, or
-similar laws prohibiting or restricting circumvention of such
-measures.
-
-  When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such circumvention
-is effected by exercising rights under this License with respect to
-the covered work, and you disclaim any intention to limit operation or
-modification of the work as a means of enforcing, against the work's
-users, your or third parties' legal rights to forbid circumvention of
-technological measures.
-
-  4. Conveying Verbatim Copies.
-
-  You may convey verbatim copies of the Program's source code as you
-receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice;
-keep intact all notices stating that this License and any
-non-permissive terms added in accord with section 7 apply to the code;
-keep intact all notices of the absence of any warranty; and give all
-recipients a copy of this License along with the Program.
-
-  You may charge any price or no price for each copy that you convey,
-and you may offer support or warranty protection for a fee.
-
-  5. Conveying Modified Source Versions.
-
-  You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified
-    it, and giving a relevant date.
-
-    b) The work must carry prominent notices stating that it is
-    released under this License and any conditions added under section
-    7.  This requirement modifies the requirement in section 4 to
-    "keep intact all notices".
-
-    c) You must license the entire work, as a whole, under this
-    License to anyone who comes into possession of a copy.  This
-    License will therefore apply, along with any applicable section 7
-    additional terms, to the whole of the work, and all its parts,
-    regardless of how they are packaged.  This License gives no
-    permission to license the work in any other way, but it does not
-    invalidate such permission if you have separately received it.
-
-    d) If the work has interactive user interfaces, each must display
-    Appropriate Legal Notices; however, if the Program has interactive
-    interfaces that do not display Appropriate Legal Notices, your
-    work need not make them do so.
-
-  A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work,
-and which are not combined with it such as to form a larger program,
-in or on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not
-used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit.  Inclusion of a covered work
-in an aggregate does not cause this License to apply to the other
-parts of the aggregate.
-
-  6. Conveying Non-Source Forms.
-
-  You may convey a covered work in object code form under the terms
-of sections 4 and 5, provided that you also convey the
-machine-readable Corresponding Source under the terms of this License,
-in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by the
-    Corresponding Source fixed on a durable physical medium
-    customarily used for software interchange.
-
-    b) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by a
-    written offer, valid for at least three years and valid for as
-    long as you offer spare parts or customer support for that product
-    model, to give anyone who possesses the object code either (1) a
-    copy of the Corresponding Source for all the software in the
-    product that is covered by this License, on a durable physical
-    medium customarily used for software interchange, for a price no
-    more than your reasonable cost of physically performing this
-    conveying of source, or (2) access to copy the
-    Corresponding Source from a network server at no charge.
-
-    c) Convey individual copies of the object code with a copy of the
-    written offer to provide the Corresponding Source.  This
-    alternative is allowed only occasionally and noncommercially, and
-    only if you received the object code with such an offer, in accord
-    with subsection 6b.
-
-    d) Convey the object code by offering access from a designated
-    place (gratis or for a charge), and offer equivalent access to the
-    Corresponding Source in the same way through the same place at no
-    further charge.  You need not require recipients to copy the
-    Corresponding Source along with the object code.  If the place to
-    copy the object code is a network server, the Corresponding Source
-    may be on a different server (operated by you or a third party)
-    that supports equivalent copying facilities, provided you maintain
-    clear directions next to the object code saying where to find the
-    Corresponding Source.  Regardless of what server hosts the
-    Corresponding Source, you remain obligated to ensure that it is
-    available for as long as needed to satisfy these requirements.
-
-    e) Convey the object code using peer-to-peer transmission, provided
-    you inform other peers where the object code and Corresponding
-    Source of the work are being offered to the general public at no
-    charge under subsection 6d.
-
-  A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be
-included in conveying the object code work.
-
-  A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal, family,
-or household purposes, or (2) anything designed or sold for incorporation
-into a dwelling.  In determining whether a product is a consumer product,
-doubtful cases shall be resolved in favor of coverage.  For a particular
-product received by a particular user, "normally used" refers to a
-typical or common use of that class of product, regardless of the status
-of the particular user or of the way in which the particular user
-actually uses, or expects or is expected to use, the product.  A product
-is a consumer product regardless of whether the product has substantial
-commercial, industrial or non-consumer uses, unless such uses represent
-the only significant mode of use of the product.
-
-  "Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to install
-and execute modified versions of a covered work in that User Product from
-a modified version of its Corresponding Source.  The information must
-suffice to ensure that the continued functioning of the modified object
-code is in no case prevented or interfered with solely because
-modification has been made.
-
-  If you convey an object code work under this section in, or with, or
-specifically for use in, a User Product, and the conveying occurs as
-part of a transaction in which the right of possession and use of the
-User Product is transferred to the recipient in perpetuity or for a
-fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied
-by the Installation Information.  But this requirement does not apply
-if neither you nor any third party retains the ability to install
-modified object code on the User Product (for example, the work has
-been installed in ROM).
-
-  The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or updates
-for a work that has been modified or installed by the recipient, or for
-the User Product in which it has been modified or installed.  Access to a
-network may be denied when the modification itself materially and
-adversely affects the operation of the network or violates the rules and
-protocols for communication across the network.
-
-  Corresponding Source conveyed, and Installation Information provided,
-in accord with this section must be in a format that is publicly
-documented (and with an implementation available to the public in
-source code form), and must require no special password or key for
-unpacking, reading or copying.
-
-  7. Additional Terms.
-
-  "Additional permissions" are terms that supplement the terms of this
-License by making exceptions from one or more of its conditions.
-Additional permissions that are applicable to the entire Program shall
-be treated as though they were included in this License, to the extent
-that they are valid under applicable law.  If additional permissions
-apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by
-this License without regard to the additional permissions.
-
-  When you convey a copy of a covered work, you may at your option
-remove any additional permissions from that copy, or from any part of
-it.  (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.)  You may place
-additional permissions on material, added by you to a covered work,
-for which you have or can give appropriate copyright permission.
-
-  Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders of
-that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the
-    terms of sections 15 and 16 of this License; or
-
-    b) Requiring preservation of specified reasonable legal notices or
-    author attributions in that material or in the Appropriate Legal
-    Notices displayed by works containing it; or
-
-    c) Prohibiting misrepresentation of the origin of that material, or
-    requiring that modified versions of such material be marked in
-    reasonable ways as different from the original version; or
-
-    d) Limiting the use for publicity purposes of names of licensors or
-    authors of the material; or
-
-    e) Declining to grant rights under trademark law for use of some
-    trade names, trademarks, or service marks; or
-
-    f) Requiring indemnification of licensors and authors of that
-    material by anyone who conveys the material (or modified versions of
-    it) with contractual assumptions of liability to the recipient, for
-    any liability that these contractual assumptions directly impose on
-    those licensors and authors.
-
-  All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10.  If the Program as you
-received it, or any part of it, contains a notice stating that it is
-governed by this License along with a term that is a further
-restriction, you may remove that term.  If a license document contains
-a further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms
-of that license document, provided that the further restriction does
-not survive such relicensing or conveying.
-
-  If you add terms to a covered work in accord with this section, you
-must place, in the relevant source files, a statement of the
-additional terms that apply to those files, or a notice indicating
-where to find the applicable terms.
-
-  Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions;
-the above requirements apply either way.
-
-  8. Termination.
-
-  You may not propagate or modify a covered work except as expressly
-provided under this License.  Any attempt otherwise to propagate or
-modify it is void, and will automatically terminate your rights under
-this License (including any patent licenses granted under the third
-paragraph of section 11).
-
-  However, if you cease all violation of this License, then your
-license from a particular copyright holder is reinstated (a)
-provisionally, unless and until the copyright holder explicitly and
-finally terminates your license, and (b) permanently, if the copyright
-holder fails to notify you of the violation by some reasonable means
-prior to 60 days after the cessation.
-
-  Moreover, your license from a particular copyright holder is
-reinstated permanently if the copyright holder notifies you of the
-violation by some reasonable means, this is the first time you have
-received notice of violation of this License (for any work) from that
-copyright holder, and you cure the violation prior to 30 days after
-your receipt of the notice.
-
-  Termination of your rights under this section does not terminate the
-licenses of parties who have received copies or rights from you under
-this License.  If your rights have been terminated and not permanently
-reinstated, you do not qualify to receive new licenses for the same
-material under section 10.
-
-  9. Acceptance Not Required for Having Copies.
-
-  You are not required to accept this License in order to receive or
-run a copy of the Program.  Ancillary propagation of a covered work
-occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance.  However,
-nothing other than this License grants you permission to propagate or
-modify any covered work.  These actions infringe copyright if you do
-not accept this License.  Therefore, by modifying or propagating a
-covered work, you indicate your acceptance of this License to do so.
-
-  10. Automatic Licensing of Downstream Recipients.
-
-  Each time you convey a covered work, the recipient automatically
-receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License.  You are not responsible
-for enforcing compliance by third parties with this License.
-
-  An "entity transaction" is a transaction transferring control of an
-organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations.  If propagation of a covered
-work results from an entity transaction, each party to that
-transaction who receives a copy of the work also receives whatever
-licenses to the work the party's predecessor in interest had or could
-give under the previous paragraph, plus a right to possession of the
-Corresponding Source of the work from the predecessor in interest, if
-the predecessor has it or can get it with reasonable efforts.
-
-  You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License.  For example, you may
-not impose a license fee, royalty, or other charge for exercise of
-rights granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that
-any patent claim is infringed by making, using, selling, offering for
-sale, or importing the Program or any portion of it.
-
-  11. Patents.
-
-  A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based.  The
-work thus licensed is called the contributor's "contributor version".
-
-  A contributor's "essential patent claims" are all patent claims
-owned or controlled by the contributor, whether already acquired or
-hereafter acquired, that would be infringed by some manner, permitted
-by this License, of making, using, or selling its contributor version,
-but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version.  For
-purposes of this definition, "control" includes the right to grant
-patent sublicenses in a manner consistent with the requirements of
-this License.
-
-  Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to
-make, use, sell, offer for sale, import and otherwise run, modify and
-propagate the contents of its contributor version.
-
-  In the following three paragraphs, a "patent license" is any express
-agreement or commitment, however denominated, not to enforce a patent
-(such as an express permission to practice a patent or covenant not to
-sue for patent infringement).  To "grant" such a patent license to a
-party means to make such an agreement or commitment not to enforce a
-patent against the party.
-
-  If you convey a covered work, knowingly relying on a patent license,
-and the Corresponding Source of the work is not available for anyone
-to copy, free of charge and under the terms of this License, through a
-publicly available network server or other readily accessible means,
-then you must either (1) cause the Corresponding Source to be so
-available, or (2) arrange to deprive yourself of the benefit of the
-patent license for this particular work, or (3) arrange, in a manner
-consistent with the requirements of this License, to extend the patent
-license to downstream recipients.  "Knowingly relying" means you have
-actual knowledge that, but for the patent license, your conveying the
-covered work in a country, or your recipient's use of the covered work
-in a country, would infringe one or more identifiable patents in that
-country that you have reason to believe are valid.
-
-  If, pursuant to or in connection with a single transaction or
-arrangement, you convey, or propagate by procuring conveyance of, a
-covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify
-or convey a specific copy of the covered work, then the patent license
-you grant is automatically extended to all recipients of the covered
-work and works based on it.
-
-  A patent license is "discriminatory" if it does not include within
-the scope of its coverage, prohibits the exercise of, or is
-conditioned on the non-exercise of one or more of the rights that are
-specifically granted under this License.  You may not convey a covered
-work if you are a party to an arrangement with a third party that is
-in the business of distributing software, under which you make payment
-to the third party based on the extent of your activity of conveying
-the work, and under which the third party grants, to any of the
-parties who would receive the covered work from you, a discriminatory
-patent license (a) in connection with copies of the covered work
-conveyed by you (or copies made from those copies), or (b) primarily
-for and in connection with specific products or compilations that
-contain the covered work, unless you entered into that arrangement,
-or that patent license was granted, prior to 28 March 2007.
-
-  Nothing in this License shall be construed as excluding or limiting
-any implied license or other defenses to infringement that may
-otherwise be available to you under applicable patent law.
-
-  12. No Surrender of Others' Freedom.
-
-  If conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you may
-not convey it at all.  For example, if you agree to terms that obligate you
-to collect a royalty for further conveying from those to whom you convey
-the Program, the only way you could satisfy both those terms and this
-License would be to refrain entirely from conveying the Program.
-
-  13. Use with the GNU Affero General Public License.
-
-  Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU Affero General Public License into a single
-combined work, and to convey the resulting work.  The terms of this
-License will continue to apply to the part which is the covered work,
-but the special requirements of the GNU Affero General Public License,
-section 13, concerning interaction through a network will apply to the
-combination as such.
-
-  14. Revised Versions of this License.
-
-  The Free Software Foundation may publish revised and/or new versions of
-the GNU General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-  Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation.  If the Program does not specify a version number of the
-GNU General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-  If the Program specifies that a proxy can decide which future
-versions of the GNU General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
-
-  Later license versions may give you additional or different
-permissions.  However, no additional obligations are imposed on any
-author or copyright holder as a result of your choosing to follow a
-later version.
-
-  15. Disclaimer of Warranty.
-
-  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-  16. Limitation of Liability.
-
-  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGES.
-
-  17. Interpretation of Sections 15 and 16.
-
-  If the disclaimer of warranty and limitation of liability provided
-above cannot be given local legal effect according to their terms,
-reviewing courts shall apply local law that most closely approximates
-an absolute waiver of all civil liability in connection with the
-Program, unless a warranty or assumption of liability accompanies a
-copy of the Program in return for a fee.
-
-                     END OF TERMS AND CONDITIONS
-
-            How to Apply These Terms to Your New Programs
-
-  If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-state the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
-  If the program does terminal interaction, make it output a short
-notice like this when it starts in an interactive mode:
-
-    <program>  Copyright (C) <year>  <name of author>
-    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions; type `show c' for details.
-
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, your program's commands
-might be different; for a GUI interface, you would use an "about box".
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<https://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
-<https://www.gnu.org/licenses/why-not-lgpl.html>.
+                    GNU GENERAL PUBLIC LICENSE
+                       Version 3, 29 June 2007
+
+ Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+                            Preamble
+
+  The GNU General Public License is a free, copyleft license for
+software and other kinds of works.
+
+  The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works.  By contrast,
+the GNU General Public License is intended to guarantee your freedom to
+share and change all versions of a program--to make sure it remains free
+software for all its users.  We, the Free Software Foundation, use the
+GNU General Public License for most of our software; it applies also to
+any other work released this way by its authors.  You can apply it to
+your programs, too.
+
+  When we speak of free software, we are referring to freedom, not
+price.  Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+  To protect your rights, we need to prevent others from denying you
+these rights or asking you to surrender the rights.  Therefore, you have
+certain responsibilities if you distribute copies of the software, or if
+you modify it: responsibilities to respect the freedom of others.
+
+  For example, if you distribute copies of such a program, whether
+gratis or for a fee, you must pass on to the recipients the same
+freedoms that you received.  You must make sure that they, too, receive
+or can get the source code.  And you must show them these terms so they
+know their rights.
+
+  Developers that use the GNU GPL protect your rights with two steps:
+(1) assert copyright on the software, and (2) offer you this License
+giving you legal permission to copy, distribute and/or modify it.
+
+  For the developers' and authors' protection, the GPL clearly explains
+that there is no warranty for this free software.  For both users' and
+authors' sake, the GPL requires that modified versions be marked as
+changed, so that their problems will not be attributed erroneously to
+authors of previous versions.
+
+  Some devices are designed to deny users access to install or run
+modified versions of the software inside them, although the manufacturer
+can do so.  This is fundamentally incompatible with the aim of
+protecting users' freedom to change the software.  The systematic
+pattern of such abuse occurs in the area of products for individuals to
+use, which is precisely where it is most unacceptable.  Therefore, we
+have designed this version of the GPL to prohibit the practice for those
+products.  If such problems arise substantially in other domains, we
+stand ready to extend this provision to those domains in future versions
+of the GPL, as needed to protect the freedom of users.
+
+  Finally, every program is threatened constantly by software patents.
+States should not allow patents to restrict development and use of
+software on general-purpose computers, but in those that do, we wish to
+avoid the special danger that patents applied to a free program could
+make it effectively proprietary.  To prevent this, the GPL assures that
+patents cannot be used to render the program non-free.
+
+  The precise terms and conditions for copying, distribution and
+modification follow.
+
+                       TERMS AND CONDITIONS
+
+  0. Definitions.
+
+  "This License" refers to version 3 of the GNU General Public License.
+
+  "Copyright" also means copyright-like laws that apply to other kinds of
+works, such as semiconductor masks.
+
+  "The Program" refers to any copyrightable work licensed under this
+License.  Each licensee is addressed as "you".  "Licensees" and
+"recipients" may be individuals or organizations.
+
+  To "modify" a work means to copy from or adapt all or part of the work
+in a fashion requiring copyright permission, other than the making of an
+exact copy.  The resulting work is called a "modified version" of the
+earlier work or a work "based on" the earlier work.
+
+  A "covered work" means either the unmodified Program or a work based
+on the Program.
+
+  To "propagate" a work means to do anything with it that, without
+permission, would make you directly or secondarily liable for
+infringement under applicable copyright law, except executing it on a
+computer or modifying a private copy.  Propagation includes copying,
+distribution (with or without modification), making available to the
+public, and in some countries other activities as well.
+
+  To "convey" a work means any kind of propagation that enables other
+parties to make or receive copies.  Mere interaction with a user through
+a computer network, with no transfer of a copy, is not conveying.
+
+  An interactive user interface displays "Appropriate Legal Notices"
+to the extent that it includes a convenient and prominently visible
+feature that (1) displays an appropriate copyright notice, and (2)
+tells the user that there is no warranty for the work (except to the
+extent that warranties are provided), that licensees may convey the
+work under this License, and how to view a copy of this License.  If
+the interface presents a list of user commands or options, such as a
+menu, a prominent item in the list meets this criterion.
+
+  1. Source Code.
+
+  The "source code" for a work means the preferred form of the work
+for making modifications to it.  "Object code" means any non-source
+form of a work.
+
+  A "Standard Interface" means an interface that either is an official
+standard defined by a recognized standards body, or, in the case of
+interfaces specified for a particular programming language, one that
+is widely used among developers working in that language.
+
+  The "System Libraries" of an executable work include anything, other
+than the work as a whole, that (a) is included in the normal form of
+packaging a Major Component, but which is not part of that Major
+Component, and (b) serves only to enable use of the work with that
+Major Component, or to implement a Standard Interface for which an
+implementation is available to the public in source code form.  A
+"Major Component", in this context, means a major essential component
+(kernel, window system, and so on) of the specific operating system
+(if any) on which the executable work runs, or a compiler used to
+produce the work, or an object code interpreter used to run it.
+
+  The "Corresponding Source" for a work in object code form means all
+the source code needed to generate, install, and (for an executable
+work) run the object code and to modify the work, including scripts to
+control those activities.  However, it does not include the work's
+System Libraries, or general-purpose tools or generally available free
+programs which are used unmodified in performing those activities but
+which are not part of the work.  For example, Corresponding Source
+includes interface definition files associated with source files for
+the work, and the source code for shared libraries and dynamically
+linked subprograms that the work is specifically designed to require,
+such as by intimate data communication or control flow between those
+subprograms and other parts of the work.
+
+  The Corresponding Source need not include anything that users
+can regenerate automatically from other parts of the Corresponding
+Source.
+
+  The Corresponding Source for a work in source code form is that
+same work.
+
+  2. Basic Permissions.
+
+  All rights granted under this License are granted for the term of
+copyright on the Program, and are irrevocable provided the stated
+conditions are met.  This License explicitly affirms your unlimited
+permission to run the unmodified Program.  The output from running a
+covered work is covered by this License only if the output, given its
+content, constitutes a covered work.  This License acknowledges your
+rights of fair use or other equivalent, as provided by copyright law.
+
+  You may make, run and propagate covered works that you do not
+convey, without conditions so long as your license otherwise remains
+in force.  You may convey covered works to others for the sole purpose
+of having them make modifications exclusively for you, or provide you
+with facilities for running those works, provided that you comply with
+the terms of this License in conveying all material for which you do
+not control copyright.  Those thus making or running the covered works
+for you must do so exclusively on your behalf, under your direction
+and control, on terms that prohibit them from making any copies of
+your copyrighted material outside their relationship with you.
+
+  Conveying under any other circumstances is permitted solely under
+the conditions stated below.  Sublicensing is not allowed; section 10
+makes it unnecessary.
+
+  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+  No covered work shall be deemed part of an effective technological
+measure under any applicable law fulfilling obligations under article
+11 of the WIPO copyright treaty adopted on 20 December 1996, or
+similar laws prohibiting or restricting circumvention of such
+measures.
+
+  When you convey a covered work, you waive any legal power to forbid
+circumvention of technological measures to the extent such circumvention
+is effected by exercising rights under this License with respect to
+the covered work, and you disclaim any intention to limit operation or
+modification of the work as a means of enforcing, against the work's
+users, your or third parties' legal rights to forbid circumvention of
+technological measures.
+
+  4. Conveying Verbatim Copies.
+
+  You may convey verbatim copies of the Program's source code as you
+receive it, in any medium, provided that you conspicuously and
+appropriately publish on each copy an appropriate copyright notice;
+keep intact all notices stating that this License and any
+non-permissive terms added in accord with section 7 apply to the code;
+keep intact all notices of the absence of any warranty; and give all
+recipients a copy of this License along with the Program.
+
+  You may charge any price or no price for each copy that you convey,
+and you may offer support or warranty protection for a fee.
+
+  5. Conveying Modified Source Versions.
+
+  You may convey a work based on the Program, or the modifications to
+produce it from the Program, in the form of source code under the
+terms of section 4, provided that you also meet all of these conditions:
+
+    a) The work must carry prominent notices stating that you modified
+    it, and giving a relevant date.
+
+    b) The work must carry prominent notices stating that it is
+    released under this License and any conditions added under section
+    7.  This requirement modifies the requirement in section 4 to
+    "keep intact all notices".
+
+    c) You must license the entire work, as a whole, under this
+    License to anyone who comes into possession of a copy.  This
+    License will therefore apply, along with any applicable section 7
+    additional terms, to the whole of the work, and all its parts,
+    regardless of how they are packaged.  This License gives no
+    permission to license the work in any other way, but it does not
+    invalidate such permission if you have separately received it.
+
+    d) If the work has interactive user interfaces, each must display
+    Appropriate Legal Notices; however, if the Program has interactive
+    interfaces that do not display Appropriate Legal Notices, your
+    work need not make them do so.
+
+  A compilation of a covered work with other separate and independent
+works, which are not by their nature extensions of the covered work,
+and which are not combined with it such as to form a larger program,
+in or on a volume of a storage or distribution medium, is called an
+"aggregate" if the compilation and its resulting copyright are not
+used to limit the access or legal rights of the compilation's users
+beyond what the individual works permit.  Inclusion of a covered work
+in an aggregate does not cause this License to apply to the other
+parts of the aggregate.
+
+  6. Conveying Non-Source Forms.
+
+  You may convey a covered work in object code form under the terms
+of sections 4 and 5, provided that you also convey the
+machine-readable Corresponding Source under the terms of this License,
+in one of these ways:
+
+    a) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by the
+    Corresponding Source fixed on a durable physical medium
+    customarily used for software interchange.
+
+    b) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by a
+    written offer, valid for at least three years and valid for as
+    long as you offer spare parts or customer support for that product
+    model, to give anyone who possesses the object code either (1) a
+    copy of the Corresponding Source for all the software in the
+    product that is covered by this License, on a durable physical
+    medium customarily used for software interchange, for a price no
+    more than your reasonable cost of physically performing this
+    conveying of source, or (2) access to copy the
+    Corresponding Source from a network server at no charge.
+
+    c) Convey individual copies of the object code with a copy of the
+    written offer to provide the Corresponding Source.  This
+    alternative is allowed only occasionally and noncommercially, and
+    only if you received the object code with such an offer, in accord
+    with subsection 6b.
+
+    d) Convey the object code by offering access from a designated
+    place (gratis or for a charge), and offer equivalent access to the
+    Corresponding Source in the same way through the same place at no
+    further charge.  You need not require recipients to copy the
+    Corresponding Source along with the object code.  If the place to
+    copy the object code is a network server, the Corresponding Source
+    may be on a different server (operated by you or a third party)
+    that supports equivalent copying facilities, provided you maintain
+    clear directions next to the object code saying where to find the
+    Corresponding Source.  Regardless of what server hosts the
+    Corresponding Source, you remain obligated to ensure that it is
+    available for as long as needed to satisfy these requirements.
+
+    e) Convey the object code using peer-to-peer transmission, provided
+    you inform other peers where the object code and Corresponding
+    Source of the work are being offered to the general public at no
+    charge under subsection 6d.
+
+  A separable portion of the object code, whose source code is excluded
+from the Corresponding Source as a System Library, need not be
+included in conveying the object code work.
+
+  A "User Product" is either (1) a "consumer product", which means any
+tangible personal property which is normally used for personal, family,
+or household purposes, or (2) anything designed or sold for incorporation
+into a dwelling.  In determining whether a product is a consumer product,
+doubtful cases shall be resolved in favor of coverage.  For a particular
+product received by a particular user, "normally used" refers to a
+typical or common use of that class of product, regardless of the status
+of the particular user or of the way in which the particular user
+actually uses, or expects or is expected to use, the product.  A product
+is a consumer product regardless of whether the product has substantial
+commercial, industrial or non-consumer uses, unless such uses represent
+the only significant mode of use of the product.
+
+  "Installation Information" for a User Product means any methods,
+procedures, authorization keys, or other information required to install
+and execute modified versions of a covered work in that User Product from
+a modified version of its Corresponding Source.  The information must
+suffice to ensure that the continued functioning of the modified object
+code is in no case prevented or interfered with solely because
+modification has been made.
+
+  If you convey an object code work under this section in, or with, or
+specifically for use in, a User Product, and the conveying occurs as
+part of a transaction in which the right of possession and use of the
+User Product is transferred to the recipient in perpetuity or for a
+fixed term (regardless of how the transaction is characterized), the
+Corresponding Source conveyed under this section must be accompanied
+by the Installation Information.  But this requirement does not apply
+if neither you nor any third party retains the ability to install
+modified object code on the User Product (for example, the work has
+been installed in ROM).
+
+  The requirement to provide Installation Information does not include a
+requirement to continue to provide support service, warranty, or updates
+for a work that has been modified or installed by the recipient, or for
+the User Product in which it has been modified or installed.  Access to a
+network may be denied when the modification itself materially and
+adversely affects the operation of the network or violates the rules and
+protocols for communication across the network.
+
+  Corresponding Source conveyed, and Installation Information provided,
+in accord with this section must be in a format that is publicly
+documented (and with an implementation available to the public in
+source code form), and must require no special password or key for
+unpacking, reading or copying.
+
+  7. Additional Terms.
+
+  "Additional permissions" are terms that supplement the terms of this
+License by making exceptions from one or more of its conditions.
+Additional permissions that are applicable to the entire Program shall
+be treated as though they were included in this License, to the extent
+that they are valid under applicable law.  If additional permissions
+apply only to part of the Program, that part may be used separately
+under those permissions, but the entire Program remains governed by
+this License without regard to the additional permissions.
+
+  When you convey a copy of a covered work, you may at your option
+remove any additional permissions from that copy, or from any part of
+it.  (Additional permissions may be written to require their own
+removal in certain cases when you modify the work.)  You may place
+additional permissions on material, added by you to a covered work,
+for which you have or can give appropriate copyright permission.
+
+  Notwithstanding any other provision of this License, for material you
+add to a covered work, you may (if authorized by the copyright holders of
+that material) supplement the terms of this License with terms:
+
+    a) Disclaiming warranty or limiting liability differently from the
+    terms of sections 15 and 16 of this License; or
+
+    b) Requiring preservation of specified reasonable legal notices or
+    author attributions in that material or in the Appropriate Legal
+    Notices displayed by works containing it; or
+
+    c) Prohibiting misrepresentation of the origin of that material, or
+    requiring that modified versions of such material be marked in
+    reasonable ways as different from the original version; or
+
+    d) Limiting the use for publicity purposes of names of licensors or
+    authors of the material; or
+
+    e) Declining to grant rights under trademark law for use of some
+    trade names, trademarks, or service marks; or
+
+    f) Requiring indemnification of licensors and authors of that
+    material by anyone who conveys the material (or modified versions of
+    it) with contractual assumptions of liability to the recipient, for
+    any liability that these contractual assumptions directly impose on
+    those licensors and authors.
+
+  All other non-permissive additional terms are considered "further
+restrictions" within the meaning of section 10.  If the Program as you
+received it, or any part of it, contains a notice stating that it is
+governed by this License along with a term that is a further
+restriction, you may remove that term.  If a license document contains
+a further restriction but permits relicensing or conveying under this
+License, you may add to a covered work material governed by the terms
+of that license document, provided that the further restriction does
+not survive such relicensing or conveying.
+
+  If you add terms to a covered work in accord with this section, you
+must place, in the relevant source files, a statement of the
+additional terms that apply to those files, or a notice indicating
+where to find the applicable terms.
+
+  Additional terms, permissive or non-permissive, may be stated in the
+form of a separately written license, or stated as exceptions;
+the above requirements apply either way.
+
+  8. Termination.
+
+  You may not propagate or modify a covered work except as expressly
+provided under this License.  Any attempt otherwise to propagate or
+modify it is void, and will automatically terminate your rights under
+this License (including any patent licenses granted under the third
+paragraph of section 11).
+
+  However, if you cease all violation of this License, then your
+license from a particular copyright holder is reinstated (a)
+provisionally, unless and until the copyright holder explicitly and
+finally terminates your license, and (b) permanently, if the copyright
+holder fails to notify you of the violation by some reasonable means
+prior to 60 days after the cessation.
+
+  Moreover, your license from a particular copyright holder is
+reinstated permanently if the copyright holder notifies you of the
+violation by some reasonable means, this is the first time you have
+received notice of violation of this License (for any work) from that
+copyright holder, and you cure the violation prior to 30 days after
+your receipt of the notice.
+
+  Termination of your rights under this section does not terminate the
+licenses of parties who have received copies or rights from you under
+this License.  If your rights have been terminated and not permanently
+reinstated, you do not qualify to receive new licenses for the same
+material under section 10.
+
+  9. Acceptance Not Required for Having Copies.
+
+  You are not required to accept this License in order to receive or
+run a copy of the Program.  Ancillary propagation of a covered work
+occurring solely as a consequence of using peer-to-peer transmission
+to receive a copy likewise does not require acceptance.  However,
+nothing other than this License grants you permission to propagate or
+modify any covered work.  These actions infringe copyright if you do
+not accept this License.  Therefore, by modifying or propagating a
+covered work, you indicate your acceptance of this License to do so.
+
+  10. Automatic Licensing of Downstream Recipients.
+
+  Each time you convey a covered work, the recipient automatically
+receives a license from the original licensors, to run, modify and
+propagate that work, subject to this License.  You are not responsible
+for enforcing compliance by third parties with this License.
+
+  An "entity transaction" is a transaction transferring control of an
+organization, or substantially all assets of one, or subdividing an
+organization, or merging organizations.  If propagation of a covered
+work results from an entity transaction, each party to that
+transaction who receives a copy of the work also receives whatever
+licenses to the work the party's predecessor in interest had or could
+give under the previous paragraph, plus a right to possession of the
+Corresponding Source of the work from the predecessor in interest, if
+the predecessor has it or can get it with reasonable efforts.
+
+  You may not impose any further restrictions on the exercise of the
+rights granted or affirmed under this License.  For example, you may
+not impose a license fee, royalty, or other charge for exercise of
+rights granted under this License, and you may not initiate litigation
+(including a cross-claim or counterclaim in a lawsuit) alleging that
+any patent claim is infringed by making, using, selling, offering for
+sale, or importing the Program or any portion of it.
+
+  11. Patents.
+
+  A "contributor" is a copyright holder who authorizes use under this
+License of the Program or a work on which the Program is based.  The
+work thus licensed is called the contributor's "contributor version".
+
+  A contributor's "essential patent claims" are all patent claims
+owned or controlled by the contributor, whether already acquired or
+hereafter acquired, that would be infringed by some manner, permitted
+by this License, of making, using, or selling its contributor version,
+but do not include claims that would be infringed only as a
+consequence of further modification of the contributor version.  For
+purposes of this definition, "control" includes the right to grant
+patent sublicenses in a manner consistent with the requirements of
+this License.
+
+  Each contributor grants you a non-exclusive, worldwide, royalty-free
+patent license under the contributor's essential patent claims, to
+make, use, sell, offer for sale, import and otherwise run, modify and
+propagate the contents of its contributor version.
+
+  In the following three paragraphs, a "patent license" is any express
+agreement or commitment, however denominated, not to enforce a patent
+(such as an express permission to practice a patent or covenant not to
+sue for patent infringement).  To "grant" such a patent license to a
+party means to make such an agreement or commitment not to enforce a
+patent against the party.
+
+  If you convey a covered work, knowingly relying on a patent license,
+and the Corresponding Source of the work is not available for anyone
+to copy, free of charge and under the terms of this License, through a
+publicly available network server or other readily accessible means,
+then you must either (1) cause the Corresponding Source to be so
+available, or (2) arrange to deprive yourself of the benefit of the
+patent license for this particular work, or (3) arrange, in a manner
+consistent with the requirements of this License, to extend the patent
+license to downstream recipients.  "Knowingly relying" means you have
+actual knowledge that, but for the patent license, your conveying the
+covered work in a country, or your recipient's use of the covered work
+in a country, would infringe one or more identifiable patents in that
+country that you have reason to believe are valid.
+
+  If, pursuant to or in connection with a single transaction or
+arrangement, you convey, or propagate by procuring conveyance of, a
+covered work, and grant a patent license to some of the parties
+receiving the covered work authorizing them to use, propagate, modify
+or convey a specific copy of the covered work, then the patent license
+you grant is automatically extended to all recipients of the covered
+work and works based on it.
+
+  A patent license is "discriminatory" if it does not include within
+the scope of its coverage, prohibits the exercise of, or is
+conditioned on the non-exercise of one or more of the rights that are
+specifically granted under this License.  You may not convey a covered
+work if you are a party to an arrangement with a third party that is
+in the business of distributing software, under which you make payment
+to the third party based on the extent of your activity of conveying
+the work, and under which the third party grants, to any of the
+parties who would receive the covered work from you, a discriminatory
+patent license (a) in connection with copies of the covered work
+conveyed by you (or copies made from those copies), or (b) primarily
+for and in connection with specific products or compilations that
+contain the covered work, unless you entered into that arrangement,
+or that patent license was granted, prior to 28 March 2007.
+
+  Nothing in this License shall be construed as excluding or limiting
+any implied license or other defenses to infringement that may
+otherwise be available to you under applicable patent law.
+
+  12. No Surrender of Others' Freedom.
+
+  If conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License.  If you cannot convey a
+covered work so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you may
+not convey it at all.  For example, if you agree to terms that obligate you
+to collect a royalty for further conveying from those to whom you convey
+the Program, the only way you could satisfy both those terms and this
+License would be to refrain entirely from conveying the Program.
+
+  13. Use with the GNU Affero General Public License.
+
+  Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU Affero General Public License into a single
+combined work, and to convey the resulting work.  The terms of this
+License will continue to apply to the part which is the covered work,
+but the special requirements of the GNU Affero General Public License,
+section 13, concerning interaction through a network will apply to the
+combination as such.
+
+  14. Revised Versions of this License.
+
+  The Free Software Foundation may publish revised and/or new versions of
+the GNU General Public License from time to time.  Such new versions will
+be similar in spirit to the present version, but may differ in detail to
+address new problems or concerns.
+
+  Each version is given a distinguishing version number.  If the
+Program specifies that a certain numbered version of the GNU General
+Public License "or any later version" applies to it, you have the
+option of following the terms and conditions either of that numbered
+version or of any later version published by the Free Software
+Foundation.  If the Program does not specify a version number of the
+GNU General Public License, you may choose any version ever published
+by the Free Software Foundation.
+
+  If the Program specifies that a proxy can decide which future
+versions of the GNU General Public License can be used, that proxy's
+public statement of acceptance of a version permanently authorizes you
+to choose that version for the Program.
+
+  Later license versions may give you additional or different
+permissions.  However, no additional obligations are imposed on any
+author or copyright holder as a result of your choosing to follow a
+later version.
+
+  15. Disclaimer of Warranty.
+
+  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+  16. Limitation of Liability.
+
+  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+SUCH DAMAGES.
+
+  17. Interpretation of Sections 15 and 16.
+
+  If the disclaimer of warranty and limitation of liability provided
+above cannot be given local legal effect according to their terms,
+reviewing courts shall apply local law that most closely approximates
+an absolute waiver of all civil liability in connection with the
+Program, unless a warranty or assumption of liability accompanies a
+copy of the Program in return for a fee.
+
+                     END OF TERMS AND CONDITIONS
+
+            How to Apply These Terms to Your New Programs
+
+  If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these terms.
+
+  To do so, attach the following notices to the program.  It is safest
+to attach them to the start of each source file to most effectively
+state the exclusion of warranty; and each file should have at least
+the "copyright" line and a pointer to where the full notice is found.
+
+    <one line to give the program's name and a brief idea of what it does.>
+    Copyright (C) <year>  <name of author>
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+  If the program does terminal interaction, make it output a short
+notice like this when it starts in an interactive mode:
+
+    <program>  Copyright (C) <year>  <name of author>
+    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+    This is free software, and you are welcome to redistribute it
+    under certain conditions; type `show c' for details.
+
+The hypothetical commands `show w' and `show c' should show the appropriate
+parts of the General Public License.  Of course, your program's commands
+might be different; for a GUI interface, you would use an "about box".
+
+  You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU GPL, see
+<https://www.gnu.org/licenses/>.
+
+  The GNU General Public License does not permit incorporating your program
+into proprietary programs.  If your program is a subroutine library, you
+may consider it more useful to permit linking proprietary applications with
+the library.  If this is what you want to do, use the GNU Lesser General
+Public License instead of this License.  But first, please read
+<https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `yadg-5.0.1/PKG-INFO` & `yadg-5.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,97 +1,97 @@
-Metadata-Version: 2.1
-Name: yadg
-Version: 5.0.1
-Summary: yet another datagram
-Home-page: https://github.com/dgbowl/yadg
-Author: Peter Kraus
-Author-email: peter@tondon.de
-Project-URL: Bug Tracker, https://github.com/dgbowl/yadg/issues
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy
-Requires-Dist: scipy
-Requires-Dist: pint>=0.22
-Requires-Dist: pyyaml
-Requires-Dist: uncertainties
-Requires-Dist: striprtf
-Requires-Dist: tzlocal
-Requires-Dist: packaging
-Requires-Dist: python-dateutil
-Requires-Dist: openpyxl>=3.0.0
-Requires-Dist: h5netcdf~=1.0
-Requires-Dist: xarray-datatree==0.0.12
-Requires-Dist: dgbowl-schemas>=116
-Requires-Dist: requests
-Provides-Extra: testing
-Requires-Dist: pytest; extra == "testing"
-Provides-Extra: docs
-Requires-Dist: sphinx~=7.2; extra == "docs"
-Requires-Dist: sphinx-rtd-theme~=1.3.0; extra == "docs"
-Requires-Dist: sphinx-autodoc-typehints<1.20.0; extra == "docs"
-Requires-Dist: autodoc-pydantic>=2.0.0; extra == "docs"
-
-[![DOI](https://joss.theoj.org/papers/10.21105/joss.04166/status.svg)](https://doi.org/10.21105/joss.04166)
-[![Documentation](https://badgen.net/badge/docs/dgbowl.github.io/grey?icon=firefox)](https://dgbowl.github.io/yadg)
-[![PyPi version](https://badgen.net/pypi/v/yadg/?icon=pypi)](https://pypi.org/project/yadg)
-[![Github link](https://badgen.net/github/tag/dgbowl/yadg/?icon=github)](https://github.com/dgbowl/yadg/)
-[![Github status](https://badgen.net/github/checks/dgbowl/yadg/?icon=github)](https://github.com/dgbowl/yadg/actions/workflows/push-master.yml)
-
-
-# ![yet another datagram](./docs/source/images/yadg_banner.png)
-
-Set of tools to process raw instrument data according to a *dataschema* into a standardised form called *datagram*, annotated with metadata, provenance information, timestamps, units, and uncertainties. Developed by the [Materials for Energy Conversion](https://www.empa.ch/web/s501) lab at Empa (Dübendorf, CH) and by the [ConCat lab](https://www.tu.berlin/en/concat) at Technische Universität Berlin (Berlin, DE).
-
-![schema to datagram with yadg](./docs/source/images/schema_yadg_datagram.png)
-
-### Capabilities:
-- Parsing **tabulated data** using CSV parsing functionality, including Bronkhorst and DryCal output formats.
-- Parsing **chromatography data** from gas and liquid chromatography, including several Agilent, Masshunter, and Fusion formats.
-- Parsing **reflection coefficient** traces from network analysers.
-- Parsing **potentiostat files** for electrochemistry applications. Supports BioLogic file formats.
-- Parsing **spectroscopy files** including common XPS, XRD and MS formats.
-
-### Features:
-- timezone-aware timestamping using Unix timestamps
-- automatic uncertainty determination using data contained in the raw files, instrument specification, or last significant digit
-- uncertainty propagation to derived quantities
-- tagging of data with units
-- extensive *dataschema* and *datagram* validation using provided specifications
-- mandatory metadata (such as provenance) is enforced
-
-The full list of capabilities and features is listed in the [project documentation](http://dgbowl.github.io/yadg).
-
-### Installation:
-The released versions of `yadg` are available on the Python Package Index (PyPI) under [yadg](https://pypi.org/project/yadg). Those can be installed using:
-
-```bash
-    pip install yadg
-```
-
-If you wish to install the current development version as an editable installation, check out the `master` branch using git, and install `yadg` as an editable package using pip:
-
-```bash
-   git clone git@github.com:dgbowl/yadg.git
-   cd yadg
-   pip install -e .
-```
-
-Additional targets `yadg[testing]` and `yadg[docs]` are available and can be specified in the above commands, if testing and/or documentation capabilities are required.
-
-### Contributors:
-- [Peter Kraus](http://github.com/PeterKraus)
-- [Nicolas Vetsch](http://github.com/vetschn)
-
-### Acknowledgements
-
-This project has received funding from the following sources:
-
-- European Union’s Horizon 2020 programme under grant agreement No 957189.
-- DFG's Emmy Noether Programme under grant number 490703766.
-
-The project is also part of BATTERY 2030+, the large-scale European research initiative for inventing the sustainable batteries of the future.
+Metadata-Version: 2.1
+Name: yadg
+Version: 5.0.2
+Summary: yet another datagram
+Home-page: https://github.com/dgbowl/yadg
+Author: Peter Kraus
+Author-email: peter@tondon.de
+Project-URL: Bug Tracker, https://github.com/dgbowl/yadg/issues
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: pint>=0.22
+Requires-Dist: pyyaml
+Requires-Dist: uncertainties
+Requires-Dist: striprtf
+Requires-Dist: tzlocal
+Requires-Dist: packaging
+Requires-Dist: python-dateutil
+Requires-Dist: openpyxl>=3.0.0
+Requires-Dist: h5netcdf~=1.0
+Requires-Dist: xarray-datatree==0.0.12
+Requires-Dist: dgbowl-schemas>=116
+Requires-Dist: requests
+Provides-Extra: testing
+Requires-Dist: pytest; extra == "testing"
+Provides-Extra: docs
+Requires-Dist: sphinx~=7.2; extra == "docs"
+Requires-Dist: sphinx-rtd-theme~=1.3.0; extra == "docs"
+Requires-Dist: sphinx-autodoc-typehints<1.20.0; extra == "docs"
+Requires-Dist: autodoc-pydantic>=2.0.0; extra == "docs"
+
+[![DOI](https://joss.theoj.org/papers/10.21105/joss.04166/status.svg)](https://doi.org/10.21105/joss.04166)
+[![Documentation](https://badgen.net/badge/docs/dgbowl.github.io/grey?icon=firefox)](https://dgbowl.github.io/yadg)
+[![PyPi version](https://badgen.net/pypi/v/yadg/?icon=pypi)](https://pypi.org/project/yadg)
+[![Github link](https://badgen.net/github/tag/dgbowl/yadg/?icon=github)](https://github.com/dgbowl/yadg/)
+[![Github status](https://badgen.net/github/checks/dgbowl/yadg/?icon=github)](https://github.com/dgbowl/yadg/actions/workflows/push-master.yml)
+
+
+# ![yet another datagram](./docs/source/images/yadg_banner.png)
+
+Set of tools to process raw instrument data according to a *dataschema* into a standardised form called *datagram*, annotated with metadata, provenance information, timestamps, units, and uncertainties. Developed by the [Materials for Energy Conversion](https://www.empa.ch/web/s501) lab at Empa (Dübendorf, CH) and by the [ConCat lab](https://www.tu.berlin/en/concat) at Technische Universität Berlin (Berlin, DE).
+
+![schema to datagram with yadg](./docs/source/images/schema_yadg_datagram.png)
+
+### Capabilities:
+- Parsing **tabulated data** using CSV parsing functionality, including Bronkhorst and DryCal output formats.
+- Parsing **chromatography data** from gas and liquid chromatography, including several Agilent, Masshunter, and Fusion formats.
+- Parsing **reflection coefficient** traces from network analysers.
+- Parsing **potentiostat files** for electrochemistry applications. Supports BioLogic file formats.
+- Parsing **spectroscopy files** including common XPS, XRD and MS formats.
+
+### Features:
+- timezone-aware timestamping using Unix timestamps
+- automatic uncertainty determination using data contained in the raw files, instrument specification, or last significant digit
+- uncertainty propagation to derived quantities
+- tagging of data with units
+- extensive *dataschema* and *datagram* validation using provided specifications
+- mandatory metadata (such as provenance) is enforced
+
+The full list of capabilities and features is listed in the [project documentation](http://dgbowl.github.io/yadg).
+
+### Installation:
+The released versions of `yadg` are available on the Python Package Index (PyPI) under [yadg](https://pypi.org/project/yadg). Those can be installed using:
+
+```bash
+    pip install yadg
+```
+
+If you wish to install the current development version as an editable installation, check out the `master` branch using git, and install `yadg` as an editable package using pip:
+
+```bash
+   git clone git@github.com:dgbowl/yadg.git
+   cd yadg
+   pip install -e .
+```
+
+Additional targets `yadg[testing]` and `yadg[docs]` are available and can be specified in the above commands, if testing and/or documentation capabilities are required.
+
+### Contributors:
+- [Peter Kraus](http://github.com/PeterKraus)
+- [Nicolas Vetsch](http://github.com/vetschn)
+
+### Acknowledgements
+
+This project has received funding from the following sources:
+
+- European Union’s Horizon 2020 programme under grant agreement No 957189.
+- DFG's Emmy Noether Programme under grant number 490703766.
+
+The project is also part of BATTERY 2030+, the large-scale European research initiative for inventing the sustainable batteries of the future.
```

### Comparing `yadg-5.0.1/README.md` & `yadg-5.0.2/README.md`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-[![DOI](https://joss.theoj.org/papers/10.21105/joss.04166/status.svg)](https://doi.org/10.21105/joss.04166)
-[![Documentation](https://badgen.net/badge/docs/dgbowl.github.io/grey?icon=firefox)](https://dgbowl.github.io/yadg)
-[![PyPi version](https://badgen.net/pypi/v/yadg/?icon=pypi)](https://pypi.org/project/yadg)
-[![Github link](https://badgen.net/github/tag/dgbowl/yadg/?icon=github)](https://github.com/dgbowl/yadg/)
-[![Github status](https://badgen.net/github/checks/dgbowl/yadg/?icon=github)](https://github.com/dgbowl/yadg/actions/workflows/push-master.yml)
-
-
-# ![yet another datagram](./docs/source/images/yadg_banner.png)
-
-Set of tools to process raw instrument data according to a *dataschema* into a standardised form called *datagram*, annotated with metadata, provenance information, timestamps, units, and uncertainties. Developed by the [Materials for Energy Conversion](https://www.empa.ch/web/s501) lab at Empa (Dübendorf, CH) and by the [ConCat lab](https://www.tu.berlin/en/concat) at Technische Universität Berlin (Berlin, DE).
-
-![schema to datagram with yadg](./docs/source/images/schema_yadg_datagram.png)
-
-### Capabilities:
-- Parsing **tabulated data** using CSV parsing functionality, including Bronkhorst and DryCal output formats.
-- Parsing **chromatography data** from gas and liquid chromatography, including several Agilent, Masshunter, and Fusion formats.
-- Parsing **reflection coefficient** traces from network analysers.
-- Parsing **potentiostat files** for electrochemistry applications. Supports BioLogic file formats.
-- Parsing **spectroscopy files** including common XPS, XRD and MS formats.
-
-### Features:
-- timezone-aware timestamping using Unix timestamps
-- automatic uncertainty determination using data contained in the raw files, instrument specification, or last significant digit
-- uncertainty propagation to derived quantities
-- tagging of data with units
-- extensive *dataschema* and *datagram* validation using provided specifications
-- mandatory metadata (such as provenance) is enforced
-
-The full list of capabilities and features is listed in the [project documentation](http://dgbowl.github.io/yadg).
-
-### Installation:
-The released versions of `yadg` are available on the Python Package Index (PyPI) under [yadg](https://pypi.org/project/yadg). Those can be installed using:
-
-```bash
-    pip install yadg
-```
-
-If you wish to install the current development version as an editable installation, check out the `master` branch using git, and install `yadg` as an editable package using pip:
-
-```bash
-   git clone git@github.com:dgbowl/yadg.git
-   cd yadg
-   pip install -e .
-```
-
-Additional targets `yadg[testing]` and `yadg[docs]` are available and can be specified in the above commands, if testing and/or documentation capabilities are required.
-
-### Contributors:
-- [Peter Kraus](http://github.com/PeterKraus)
-- [Nicolas Vetsch](http://github.com/vetschn)
-
-### Acknowledgements
-
-This project has received funding from the following sources:
-
-- European Union’s Horizon 2020 programme under grant agreement No 957189.
-- DFG's Emmy Noether Programme under grant number 490703766.
-
-The project is also part of BATTERY 2030+, the large-scale European research initiative for inventing the sustainable batteries of the future.
+[![DOI](https://joss.theoj.org/papers/10.21105/joss.04166/status.svg)](https://doi.org/10.21105/joss.04166)
+[![Documentation](https://badgen.net/badge/docs/dgbowl.github.io/grey?icon=firefox)](https://dgbowl.github.io/yadg)
+[![PyPi version](https://badgen.net/pypi/v/yadg/?icon=pypi)](https://pypi.org/project/yadg)
+[![Github link](https://badgen.net/github/tag/dgbowl/yadg/?icon=github)](https://github.com/dgbowl/yadg/)
+[![Github status](https://badgen.net/github/checks/dgbowl/yadg/?icon=github)](https://github.com/dgbowl/yadg/actions/workflows/push-master.yml)
+
+
+# ![yet another datagram](./docs/source/images/yadg_banner.png)
+
+Set of tools to process raw instrument data according to a *dataschema* into a standardised form called *datagram*, annotated with metadata, provenance information, timestamps, units, and uncertainties. Developed by the [Materials for Energy Conversion](https://www.empa.ch/web/s501) lab at Empa (Dübendorf, CH) and by the [ConCat lab](https://www.tu.berlin/en/concat) at Technische Universität Berlin (Berlin, DE).
+
+![schema to datagram with yadg](./docs/source/images/schema_yadg_datagram.png)
+
+### Capabilities:
+- Parsing **tabulated data** using CSV parsing functionality, including Bronkhorst and DryCal output formats.
+- Parsing **chromatography data** from gas and liquid chromatography, including several Agilent, Masshunter, and Fusion formats.
+- Parsing **reflection coefficient** traces from network analysers.
+- Parsing **potentiostat files** for electrochemistry applications. Supports BioLogic file formats.
+- Parsing **spectroscopy files** including common XPS, XRD and MS formats.
+
+### Features:
+- timezone-aware timestamping using Unix timestamps
+- automatic uncertainty determination using data contained in the raw files, instrument specification, or last significant digit
+- uncertainty propagation to derived quantities
+- tagging of data with units
+- extensive *dataschema* and *datagram* validation using provided specifications
+- mandatory metadata (such as provenance) is enforced
+
+The full list of capabilities and features is listed in the [project documentation](http://dgbowl.github.io/yadg).
+
+### Installation:
+The released versions of `yadg` are available on the Python Package Index (PyPI) under [yadg](https://pypi.org/project/yadg). Those can be installed using:
+
+```bash
+    pip install yadg
+```
+
+If you wish to install the current development version as an editable installation, check out the `master` branch using git, and install `yadg` as an editable package using pip:
+
+```bash
+   git clone git@github.com:dgbowl/yadg.git
+   cd yadg
+   pip install -e .
+```
+
+Additional targets `yadg[testing]` and `yadg[docs]` are available and can be specified in the above commands, if testing and/or documentation capabilities are required.
+
+### Contributors:
+- [Peter Kraus](http://github.com/PeterKraus)
+- [Nicolas Vetsch](http://github.com/vetschn)
+
+### Acknowledgements
+
+This project has received funding from the following sources:
+
+- European Union’s Horizon 2020 programme under grant agreement No 957189.
+- DFG's Emmy Noether Programme under grant number 490703766.
+
+The project is also part of BATTERY 2030+, the large-scale European research initiative for inventing the sustainable batteries of the future.
```

### Comparing `yadg-5.0.1/src/yadg/core/__init__.py` & `yadg-5.0.2/src/yadg/core/__init__.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,191 +1,191 @@
-from importlib import metadata
-import logging
-import importlib
-from typing import Callable
-from zoneinfo import ZoneInfo
-from dgbowl_schemas.yadg.dataschema import DataSchema
-from datatree import DataTree
-import xarray as xr
-import numpy as np
-from .. import dgutils, core
-
-
-datagram_version = metadata.version("yadg")
-logger = logging.getLogger(__name__)
-
-
-def infer_datagram_handler(parser: str) -> tuple[Callable, str]:
-    """
-    Helper function to distribute work to parsers.
-
-    Parameters
-    ----------
-    parser
-        Name of the parser from schema.
-
-    Returns
-    -------
-    (process, version): tuple[Callable, str]
-        A tuple containing the handler function as :class:`Callable` and the handler
-        version as :class:`str`.
-    """
-    modname = f"yadg.parsers.{parser}"
-    try:
-        m = importlib.import_module(modname)
-        func = getattr(m, "process")
-        return func
-    except ImportError as e:
-        logger.critical(f"could not import module '{modname}'")
-        raise e
-
-
-def process_schema(dataschema: DataSchema, strict_merge: bool = False) -> DataTree:
-    """
-    Main worker function of **yadg**.
-
-    Takes in a :class:`DataSchema` object and returns a single annotated
-    `datagram` created from the `dataschema`. It is the job of the user to supply a
-    validated `schema`.
-
-    Parameters
-    ----------
-    dataschema: DataSchema
-        A fully validated `dataschema` object.
-
-    Returns
-    -------
-    datagram: DataTree
-        An unvalidated `datagram`. The `parser`\\ s included in **yadg** should return
-        a valid `datagram`; any custom `parser`\\ s might not do so. Use the function
-        :meth:`yadg.core.validators.validate_datagram` to validate the resulting `datagram`.
-    """
-
-    if strict_merge:
-        concatmode = "identical"
-    else:
-        concatmode = "drop_conflicts"
-
-    root = DataTree()
-    root.attrs = {
-        "provenance": "yadg process",
-        "date": dgutils.now(asstr=True),
-        "input_schema": dataschema.json(),
-        "datagram_version": core.datagram_version,
-    }
-    root.attrs.update(dgutils.get_yadg_metadata())
-
-    while hasattr(dataschema, "update"):
-        dataschema = dataschema.update()
-
-    for si, step in enumerate(dataschema.steps):
-        logger.info("Processing step %d:", si)
-
-        # Backfill default timezone, locale, encoding.
-        if step.extractor.timezone is None:
-            tz = ZoneInfo(dataschema.step_defaults.timezone)
-        else:
-            tz = ZoneInfo(step.extractor.timezone)
-        if step.extractor.locale is None:
-            loc = dataschema.step_defaults.locale
-        else:
-            loc = step.extractor.locale
-        if step.extractor.encoding is None:
-            enc = dataschema.step_defaults.encoding
-        else:
-            enc = step.extractor.encoding
-
-        if step.tag is None:
-            step.tag = f"{si}"
-
-        handler = infer_datagram_handler(step.parser)
-        todofiles = step.input.paths()
-        if len(todofiles) == 0:
-            logger.warning("No files processed by step '%s'.", step.tag)
-        vals = None
-        for tf in todofiles:
-            logger.info("Processing file '%s'.", tf)
-            fvals = handler(
-                fn=tf,
-                encoding=enc,
-                timezone=tz,
-                locale=loc,
-                filetype=step.extractor.filetype,
-                parameters=step.parameters,
-            )
-            if isinstance(fvals, DataTree):
-                tasks = [(k, v.to_dataset()) for k, v in fvals.items()]
-            else:
-                tasks = [(None, fvals)]
-            for task in tasks:
-                name, dset = task
-                for k in dset:
-                    assert (
-                        "/" not in k
-                    ), f"The character '/' cannot be used in variable names: '{k}'."
-                if not hasattr(dset, "uts"):
-                    dset = dset.expand_dims("uts")
-                if len(dset.uts.coords) == 0:
-                    dset["uts"] = np.zeros(dset.uts.size)
-                    dset.attrs["fulldate"] = False
-                if (
-                    not dset.attrs.get("fulldate", True)
-                    or step.externaldate is not None
-                ):
-                    ts, fulldate = dgutils.complete_timestamps(
-                        timesteps=dset.uts.values,
-                        fn=tf,
-                        spec=step.externaldate,
-                        timezone=tz,
-                    )
-                    dset["uts"] = ts
-                    if fulldate:
-                        dset.attrs.pop("fulldate", None)
-                    else:
-                        dset.attrs["fulldate"] = int(fulldate)
-                if name is None:
-                    fvals = dset
-                else:
-                    fvals[name] = DataTree(dset)
-            if vals is None:
-                vals = fvals
-            elif isinstance(vals, xr.Dataset):
-                try:
-                    vals = xr.concat([vals, fvals], dim="uts", combine_attrs=concatmode)
-                except xr.MergeError:
-                    raise RuntimeError(
-                        "Merging metadata from multiple files has failed, as some of the "
-                        "values differ between files. This might be caused by trying to "
-                        "parse data obtained using different techniques/protocols in a "
-                        "single step. If you are certain this is what you want, try using "
-                        "yadg with the '--ignore-merge-errors' option."
-                    )
-            elif isinstance(vals, DataTree):
-                for k, v in fvals.items():
-                    if k in vals:  # pylint: disable=E1135
-                        try:
-                            newv = xr.concat(
-                                [vals[k].ds, v.ds],  # pylint: disable=E1136
-                                dim="uts",
-                                combine_attrs=concatmode,
-                            )
-                        except xr.MergeError:
-                            raise RuntimeError(
-                                "Merging metadata from multiple files has failed, as some of the "
-                                "values differ between files. This might be caused by trying to "
-                                "parse data obtained using different techniques/protocols in a "
-                                "single step. If you are certain this is what you want, try using "
-                                "yadg with the '--ignore-merge-errors' option."
-                            )
-                    else:
-                        newv = v.ds
-                    vals[k] = DataTree(newv)  # pylint: disable=E1137
-        if isinstance(vals, xr.Dataset):
-            stepdt = DataTree.from_dict({"/": vals})
-        elif isinstance(vals, DataTree):
-            stepdt = vals
-        else:
-            stepdt = DataTree()
-        stepdt.name = step.tag
-        stepdt.attrs = dict(parser=step.parser)
-        stepdt.parent = root
-    return root
+from importlib import metadata
+import logging
+import importlib
+from typing import Callable
+from zoneinfo import ZoneInfo
+from dgbowl_schemas.yadg.dataschema import DataSchema
+from datatree import DataTree
+import xarray as xr
+import numpy as np
+from .. import dgutils, core
+
+
+datagram_version = metadata.version("yadg")
+logger = logging.getLogger(__name__)
+
+
+def infer_datagram_handler(parser: str) -> tuple[Callable, str]:
+    """
+    Helper function to distribute work to parsers.
+
+    Parameters
+    ----------
+    parser
+        Name of the parser from schema.
+
+    Returns
+    -------
+    (process, version): tuple[Callable, str]
+        A tuple containing the handler function as :class:`Callable` and the handler
+        version as :class:`str`.
+    """
+    modname = f"yadg.parsers.{parser}"
+    try:
+        m = importlib.import_module(modname)
+        func = getattr(m, "process")
+        return func
+    except ImportError as e:
+        logger.critical(f"could not import module '{modname}'")
+        raise e
+
+
+def process_schema(dataschema: DataSchema, strict_merge: bool = False) -> DataTree:
+    """
+    Main worker function of **yadg**.
+
+    Takes in a :class:`DataSchema` object and returns a single annotated
+    `datagram` created from the `dataschema`. It is the job of the user to supply a
+    validated `schema`.
+
+    Parameters
+    ----------
+    dataschema: DataSchema
+        A fully validated `dataschema` object.
+
+    Returns
+    -------
+    datagram: DataTree
+        An unvalidated `datagram`. The `parser`\\ s included in **yadg** should return
+        a valid `datagram`; any custom `parser`\\ s might not do so. Use the function
+        :meth:`yadg.core.validators.validate_datagram` to validate the resulting `datagram`.
+    """
+
+    if strict_merge:
+        concatmode = "identical"
+    else:
+        concatmode = "drop_conflicts"
+
+    root = DataTree()
+    root.attrs = {
+        "provenance": "yadg process",
+        "date": dgutils.now(asstr=True),
+        "input_schema": dataschema.json(),
+        "datagram_version": core.datagram_version,
+    }
+    root.attrs.update(dgutils.get_yadg_metadata())
+
+    while hasattr(dataschema, "update"):
+        dataschema = dataschema.update()
+
+    for si, step in enumerate(dataschema.steps):
+        logger.info("Processing step %d:", si)
+
+        # Backfill default timezone, locale, encoding.
+        if step.extractor.timezone is None:
+            tz = ZoneInfo(dataschema.step_defaults.timezone)
+        else:
+            tz = ZoneInfo(step.extractor.timezone)
+        if step.extractor.locale is None:
+            loc = dataschema.step_defaults.locale
+        else:
+            loc = step.extractor.locale
+        if step.extractor.encoding is None:
+            enc = dataschema.step_defaults.encoding
+        else:
+            enc = step.extractor.encoding
+
+        if step.tag is None:
+            step.tag = f"{si}"
+
+        handler = infer_datagram_handler(step.parser)
+        todofiles = step.input.paths()
+        if len(todofiles) == 0:
+            logger.warning("No files processed by step '%s'.", step.tag)
+        vals = None
+        for tf in todofiles:
+            logger.info("Processing file '%s'.", tf)
+            fvals = handler(
+                fn=tf,
+                encoding=enc,
+                timezone=tz,
+                locale=loc,
+                filetype=step.extractor.filetype,
+                parameters=step.parameters,
+            )
+            if isinstance(fvals, DataTree):
+                tasks = [(k, v.to_dataset()) for k, v in fvals.items()]
+            else:
+                tasks = [(None, fvals)]
+            for task in tasks:
+                name, dset = task
+                for k in dset:
+                    assert (
+                        "/" not in k
+                    ), f"The character '/' cannot be used in variable names: '{k}'."
+                if not hasattr(dset, "uts"):
+                    dset = dset.expand_dims("uts")
+                if len(dset.uts.coords) == 0:
+                    dset["uts"] = np.zeros(dset.uts.size)
+                    dset.attrs["fulldate"] = False
+                if (
+                    not dset.attrs.get("fulldate", True)
+                    or step.externaldate is not None
+                ):
+                    ts, fulldate = dgutils.complete_timestamps(
+                        timesteps=dset.uts.values,
+                        fn=tf,
+                        spec=step.externaldate,
+                        timezone=tz,
+                    )
+                    dset["uts"] = ts
+                    if fulldate:
+                        dset.attrs.pop("fulldate", None)
+                    else:
+                        dset.attrs["fulldate"] = int(fulldate)
+                if name is None:
+                    fvals = dset
+                else:
+                    fvals[name] = DataTree(dset)
+            if vals is None:
+                vals = fvals
+            elif isinstance(vals, xr.Dataset):
+                try:
+                    vals = xr.concat([vals, fvals], dim="uts", combine_attrs=concatmode)
+                except xr.MergeError:
+                    raise RuntimeError(
+                        "Merging metadata from multiple files has failed, as some of the "
+                        "values differ between files. This might be caused by trying to "
+                        "parse data obtained using different techniques/protocols in a "
+                        "single step. If you are certain this is what you want, try using "
+                        "yadg with the '--ignore-merge-errors' option."
+                    )
+            elif isinstance(vals, DataTree):
+                for k, v in fvals.items():
+                    if k in vals:  # pylint: disable=E1135
+                        try:
+                            newv = xr.concat(
+                                [vals[k].ds, v.ds],  # pylint: disable=E1136
+                                dim="uts",
+                                combine_attrs=concatmode,
+                            )
+                        except xr.MergeError:
+                            raise RuntimeError(
+                                "Merging metadata from multiple files has failed, as some of the "
+                                "values differ between files. This might be caused by trying to "
+                                "parse data obtained using different techniques/protocols in a "
+                                "single step. If you are certain this is what you want, try using "
+                                "yadg with the '--ignore-merge-errors' option."
+                            )
+                    else:
+                        newv = v.ds
+                    vals[k] = DataTree(newv)  # pylint: disable=E1137
+        if isinstance(vals, xr.Dataset):
+            stepdt = DataTree.from_dict({"/": vals})
+        elif isinstance(vals, DataTree):
+            stepdt = vals
+        else:
+            stepdt = DataTree()
+        stepdt.name = step.tag
+        stepdt.attrs = dict(parser=step.parser)
+        stepdt.parent = root
+    return root
```

### Comparing `yadg-5.0.1/src/yadg/dgutils/btools.py` & `yadg-5.0.2/src/yadg/dgutils/btools.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,75 +1,75 @@
-import numpy as np
-from typing import Union, Any
-
-
-def read_pascal_string(pascal_bytes: bytes, encoding: str = "windows-1252") -> str:
-    """Parses a length-prefixed string given some encoding.
-
-    Parameters
-    ----------
-    bytes
-        The bytes of the string starting at the length-prefix byte.
-
-    encoding
-        The encoding of the string to be converted.
-
-    Returns
-    -------
-    str
-        The string decoded from the input bytes.
-
-    """
-    mul = 2 if encoding in {"utf-16"} else 1
-    lstr = int.from_bytes(pascal_bytes[0:1], byteorder="big") * mul
-    if len(pascal_bytes) < lstr + 1:
-        raise ValueError("Insufficient number of bytes.")
-    string_bytes = pascal_bytes[1 : lstr + 1]
-    return string_bytes.decode(encoding)
-
-
-def read_value(
-    data: bytes,
-    offset: int,
-    dtype: Union[np.dtype, str],
-    encoding: str = "windows-1252",
-) -> Any:
-    """Reads a single value or a set of values from a buffer at a certain offset.
-
-    Just a handy wrapper for np.frombuffer(..., count=1) With the added benefit of
-    allowing the 'pascal' keyword as an indicator for a length-prefixed
-    string.
-
-    The read value is converted to a built-in datatype using
-    np.dtype.item().
-
-    Parameters
-    ----------
-    data
-        An object that exposes the buffer interface. Here always bytes.
-
-    offset
-        Start reading the buffer from this offset (in bytes).
-
-    dtype
-        Data-type to read in.
-
-    encoding
-        The encoding of the bytes to be converted.
-
-    Returns
-    -------
-    Any
-        The unpacked and converted value from the buffer.
-
-    """
-    if dtype == "pascal":
-        # Allow the use of 'pascal' in all of the dtype maps.
-        return read_pascal_string(data[offset:], encoding="windows-1252")
-    elif dtype in {"utf-8", "utf-16"}:
-        return read_pascal_string(data[offset:], encoding=dtype)
-    value = np.frombuffer(data, offset=offset, dtype=dtype, count=1)
-    item = value.item()
-    if value.dtype.names:
-        item = [i.decode(encoding) if isinstance(i, bytes) else i for i in item]
-        return dict(zip(value.dtype.names, item))
-    return item.decode(encoding) if isinstance(item, bytes) else item
+import numpy as np
+from typing import Union, Any
+
+
+def read_pascal_string(pascal_bytes: bytes, encoding: str = "windows-1252") -> str:
+    """Parses a length-prefixed string given some encoding.
+
+    Parameters
+    ----------
+    bytes
+        The bytes of the string starting at the length-prefix byte.
+
+    encoding
+        The encoding of the string to be converted.
+
+    Returns
+    -------
+    str
+        The string decoded from the input bytes.
+
+    """
+    mul = 2 if encoding in {"utf-16"} else 1
+    lstr = int.from_bytes(pascal_bytes[0:1], byteorder="big") * mul
+    if len(pascal_bytes) < lstr + 1:
+        raise ValueError("Insufficient number of bytes.")
+    string_bytes = pascal_bytes[1 : lstr + 1]
+    return string_bytes.decode(encoding)
+
+
+def read_value(
+    data: bytes,
+    offset: int,
+    dtype: Union[np.dtype, str],
+    encoding: str = "windows-1252",
+) -> Any:
+    """Reads a single value or a set of values from a buffer at a certain offset.
+
+    Just a handy wrapper for np.frombuffer(..., count=1) With the added benefit of
+    allowing the 'pascal' keyword as an indicator for a length-prefixed
+    string.
+
+    The read value is converted to a built-in datatype using
+    np.dtype.item().
+
+    Parameters
+    ----------
+    data
+        An object that exposes the buffer interface. Here always bytes.
+
+    offset
+        Start reading the buffer from this offset (in bytes).
+
+    dtype
+        Data-type to read in.
+
+    encoding
+        The encoding of the bytes to be converted.
+
+    Returns
+    -------
+    Any
+        The unpacked and converted value from the buffer.
+
+    """
+    if dtype == "pascal":
+        # Allow the use of 'pascal' in all of the dtype maps.
+        return read_pascal_string(data[offset:], encoding="windows-1252")
+    elif dtype in {"utf-8", "utf-16"}:
+        return read_pascal_string(data[offset:], encoding=dtype)
+    value = np.frombuffer(data, offset=offset, dtype=dtype, count=1)
+    item = value.item()
+    if value.dtype.names:
+        item = [i.decode(encoding) if isinstance(i, bytes) else i for i in item]
+        return dict(zip(value.dtype.names, item))
+    return item.decode(encoding) if isinstance(item, bytes) else item
```

### Comparing `yadg-5.0.1/src/yadg/dgutils/dateutils.py` & `yadg-5.0.2/src/yadg/dgutils/dateutils.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,417 +1,417 @@
-import os
-import pickle
-import json
-import datetime
-import dateutil.parser
-import logging
-from zoneinfo import ZoneInfo
-import numpy as np
-from typing import Callable, Union, Mapping, Iterable
-from dgbowl_schemas.yadg.dataschema_5_0.externaldate import ExternalDate
-from dgbowl_schemas.yadg.dataschema_5_0.timestamp import TimestampSpec
-
-
-logger = logging.getLogger(__name__)
-
-
-def now(
-    asstr: bool = False, tz: datetime.timezone = datetime.timezone.utc
-) -> Union[float, str]:
-    """
-    Wrapper around datetime.now()
-
-    A convenience function for returning the current time as a ISO 8601 or as a unix timestamp.
-    """
-    dt = datetime.datetime.now(tz=tz)
-    if asstr:
-        return dt.strftime("%Y-%m-%d %H:%M:%S")
-    else:
-        return dt.timestamp()
-
-
-def ole_to_uts(ole_timestamp: float, timezone: ZoneInfo) -> float:
-    """
-    Converts a Microsoft OLE timestamp into a POSIX timestamp.
-
-    The OLE automation date format is a floating point value, counting
-    days since midnight 30 December 1899. Hours and minutes are
-    represented as fractional days.
-
-    https://devblogs.microsoft.com/oldnewthing/20030905-02/?p=42653
-
-    Parameters
-    ----------
-    ole_timestamp
-        A timestamp in Microsoft OLE format.
-    timezone
-        String desribing the timezone.
-
-    Returns
-    -------
-    time: float
-        The corresponding Unix timestamp.
-
-    """
-    ole_base = datetime.datetime(year=1899, month=12, day=30, tzinfo=timezone)
-    ole_delta = datetime.timedelta(days=ole_timestamp)
-    time = ole_base + ole_delta
-    return time.timestamp()
-
-
-def str_to_uts(
-    *, timestamp: str, timezone: ZoneInfo, format: str = None, strict: bool = True
-) -> Union[float, None]:
-    """
-    Converts a string to POSIX timestamp.
-
-    If the optional ``format`` is specified, the ``timestamp`` string is processed
-    using the :func:`datetime.datetime.strptime` function; if no ``format`` is
-    supplied, an ISO 8601 format is assumed and an attempt to parse using
-    :func:`dateutil.parser.parse` is made.
-
-    Parameters
-    ----------
-    timestamp
-        A string containing the timestamp.
-
-    format
-        Optional format string for parsing of the ``timestamp``.
-
-    timezone
-        Optional timezone of the ``timestamp``. By default, "UTC".
-
-    strict
-        Whether to re-raise any parsing errors.
-
-    Returns
-    -------
-    uts: Union[float, None]
-        Returns the POSIX timestamp if successful, otherwise None.
-
-    """
-
-    try:
-        if format is None:
-            dt = dateutil.parser.parse(timestamp)
-        else:
-            dt = datetime.datetime.strptime(timestamp, format)
-
-        local_tz = timezone if dt.tzinfo is None else dt.tzinfo
-        local_dt = dt.replace(tzinfo=local_tz)
-        utc_dt = local_dt.astimezone(datetime.timezone.utc)
-        return utc_dt.timestamp()
-    except (dateutil.parser.ParserError, ValueError) as e:
-        if strict:
-            raise e
-        else:
-            logger.info(
-                "Parsing timestamp '%s' with format '%s' was not successful.",
-                str(timestamp),
-                format,
-            )
-            return None
-
-
-def infer_timestamp_from(
-    *,
-    headers: list = None,
-    spec: TimestampSpec = None,
-    timezone: ZoneInfo,
-) -> tuple[list, Callable, bool]:
-    """
-    Convenience function for timestamping
-
-    Given a set of headers, and an optional specification, return an array containing
-    column indices from which a timestamp in a given row can be computed, as well as the
-    function which will compute the timestamp given the returned array.
-
-    Parameters
-    ----------
-    headers
-        An array of strings. If `spec` is not supplied, must contain either "uts"
-        :class:`(float)` or "timestep" :class:`(str)` (conforming to ISO 8601).
-
-    spec
-        A specification of timestamp elements with associated column indices and
-        optional formats. Currently accepted combinations of keys are: "uts"; "timestamp";
-        "date" and / or "time".
-
-    tz
-        Timezone to use for conversion. By default, UTC is used.
-
-    Returns
-    -------
-    (datecolumns, datefunc, fulldate): tuple[list, Callable, bool]
-        A tuple containing a list of indices of columns, a Callable to which the
-        columns have to be passed to obtain a uts timestamp, and whether the determined
-        timestamp is full or partial.
-
-    """
-
-    if spec is not None:
-        if hasattr(spec, "uts"):
-            return [spec.uts.index], float, True
-        elif hasattr(spec, "timestamp"):
-
-            def retfunc(value):
-                return str_to_uts(
-                    timestamp=value, format=spec.timestamp.format, timezone=timezone
-                )
-
-            return [spec.timestamp.index], retfunc, True
-        elif hasattr(spec, "date") or hasattr(spec, "time"):
-            specdict = {
-                "date": datetime.datetime.fromtimestamp(0).timestamp,
-                "time": datetime.datetime.fromtimestamp(0).timestamp,
-            }
-            cols = [None, None]
-            if spec.date is not None:
-
-                def datefn(value):
-                    return str_to_uts(
-                        timestamp=value, format=spec.date.format, timezone=timezone
-                    )
-
-                cols[0] = spec.date.index
-                specdict["date"] = datefn
-            if spec.time is not None:
-                if spec.time.format is not None:
-
-                    def timefn(value):
-                        t = datetime.datetime.strptime(value, spec.time.format)
-                        td = datetime.timedelta(
-                            hours=t.hour,
-                            minutes=t.minute,
-                            seconds=t.second,
-                            microseconds=t.microsecond,
-                        )
-                        return td.total_seconds()
-
-                else:
-                    logger.debug(
-                        "Assuming specified column containing the time is in ISO 8601 format"
-                    )
-
-                    def timefn(value):
-                        t = datetime.time.fromisoformat(value)
-                        td = datetime.timedelta(
-                            hours=t.hour,
-                            minutes=t.minute,
-                            seconds=t.second,
-                            microseconds=t.microsecond,
-                        )
-                        return td.total_seconds()
-
-                cols[1] = spec.time.index
-                specdict["time"] = timefn
-            if cols[0] is None:
-                return [cols[1]], specdict["time"], False
-            elif cols[1] is None:
-                return [cols[0]], specdict["date"], False
-            else:
-
-                def retfn(date, time):
-                    return specdict["date"](date) + specdict["time"](time)
-
-                return cols, retfn, True
-    elif "uts" in headers:
-        logger.debug(
-            "No timestamp spec provided, assuming column 'uts' is a valid unix timestamp"
-        )
-        return [headers.index("uts")], float, True
-    elif "timestamp" in headers:
-        logger.debug(
-            "No timestamp spec provided, assuming column 'timestamp' is a valid ISO 8601 timestamp"
-        )
-
-        def retfunc(value):
-            return str_to_uts(timestamp=value, timezone=timezone)
-
-        return [headers.index("timestamp")], retfunc, True
-    else:
-        assert False, "dateutils: A valid timestamp could not be deduced."
-
-
-def complete_timestamps(
-    *,
-    timesteps: list,
-    fn: str,
-    spec: ExternalDate,
-    timezone: ZoneInfo,
-) -> list[float]:
-    """
-    Timestamp completing function.
-
-    This function allows for completing or overriding the uts timestamps determined by
-    the individual parsers. **yadg** enters this function for any parser which does not
-    return a full timestamp, as well as if the ``externaldate`` specification is
-    specified by the user.
-
-    The ``externaldate`` specification is as follows:
-
-    .. autopydantic_model:: dgbowl_schemas.yadg.dataschema_5_0.externaldate.ExternalDate
-       :noindex:
-
-    The ``using`` key specifies how an external timestamp is created. Only one entry in
-    ``using`` is permitted. By default, this entry is:
-
-    .. code-block:: yaml
-
-        using:
-          filename:
-            format: "%Y-%m-%d-%H-%M-%S"
-            len: 19
-
-    Which means the code will attempt to deduce the timestamp from the path of the
-    processed file (``fn``), using the first 19 characters of the base filename
-    according to the above format (eg. "2021-12-31-13-45-00").
-
-    If ``file`` is specified, the handling of timestamps is handed off to
-    :func:`timestamps_from_file`.
-
-    The ``mode`` key specifies whether the offsets determined in this function are
-    added to the current timestamps (eg. date offset being added to time) or whether
-    they should replace the existing timestamps completely.
-
-    As a measure of last resort, the ``mtime`` of the ``fn`` is used. ``mtime`` is
-    preferred to ``ctime``, as the former has a more consistent cross-platform
-    behaviour.
-
-    Parameters
-    ----------
-    timesteps
-        A list of timesteps generated from a single file, ``fn``.
-
-    fn
-        Filename used to create ``timesteps``.
-
-    spec
-        ``externaldate`` specification part of the `schema`.
-
-    timezone
-        Timezone, defaults to "UTC".
-
-    """
-    delta = None
-
-    fulldate = True
-    if spec is not None:
-        replace = spec.mode == "replace"
-        method = spec.using
-    else:
-        replace = False
-        method = None
-
-    if hasattr(method, "file"):
-        delta = timestamps_from_file(
-            method.file.path, method.file.type, method.file.match, timezone
-        )
-    elif hasattr(method, "isostring"):
-        delta = str_to_uts(
-            timestamp=method.isostring, format=None, timezone=timezone, strict=True
-        )
-    elif hasattr(method, "utsoffset"):
-        delta = method.utsoffset
-    elif hasattr(method, "filename"):
-        basename = os.path.basename(fn)
-        filename, ext = os.path.splitext(basename)
-        string = filename[: method.filename.len]
-        delta = str_to_uts(
-            timestamp=string,
-            format=method.filename.format,
-            timezone=timezone,
-            strict=False,
-        )
-
-    if delta is None:
-        logger.warning("Timestamp completion failed. Using 'mtime'.")
-        delta = os.path.getmtime(fn)
-        fulldate = False
-
-    if isinstance(delta, float):
-        delta = [delta] * len(timesteps)
-
-    assert len(delta) == len(timesteps)
-
-    if replace:
-        timesteps = delta
-    else:
-        timesteps = timesteps + delta
-
-    return timesteps, fulldate
-
-
-def timestamps_from_file(
-    path: str,
-    type: str,
-    match: str,
-    timezone: ZoneInfo,
-) -> Union[float, list[float]]:
-    """
-    Load timestamps from file.
-
-    This function enables loading timestamps from file specified by the ``path``.
-    The currently supported file formats include ``json`` and ``pkl``, which must
-    contain a top-level :class:`Mapping` with a key that is matched by ``match``,
-    or a top-level :class:`Iterable`, both containing :class:`str` or :class:`float`
-    -like objects that can be processed into an Unix timestamp.
-
-    Parameters
-    ----------
-    path
-        Location of the external file.
-
-    type
-        Type of the external file. Currently, ``"json", "pkl"`` are supported.
-
-    match
-        An optional key to match if the object in ``path`` is a :class:`Mapping`.
-
-    timezone
-        An optional timezone string, defaults to "UTC"
-
-    Returns
-    -------
-    parseddata: Union[float, list[float]]
-        A single or a list of POSIX timestamps.
-
-    """
-    assert os.path.exists(path), f"timestamps_from_file: path '{path}' doesn't exist."
-    assert os.path.isfile(path), f"timestamps_from_file: Path '{path}' is not a file."
-
-    if type == "pkl":
-        logger.debug("Loading '%s' as pickle.", path)
-        with open(path, "rb") as infile:
-            data = pickle.load(infile)
-    elif type == "json":
-        logger.debug("Loading '%s' as json.", path)
-        with open(path, "r") as infile:
-            data = json.load(infile)
-    elif type == "agilent.log":
-        logger.critical("Type 'agilent.log' not yet supported.")
-        data = None
-
-    if data is None:
-        return data
-    elif isinstance(data, Iterable):
-        if isinstance(data, Mapping):
-            assert match in data
-            data = data[match]
-        if isinstance(data, Iterable):
-            parseddata = []
-            for i in data:
-                if isinstance(i, str):
-                    delta = str_to_uts(
-                        timestamp=i, format=None, timezone=timezone, strict=True
-                    )
-                    parseddata.append(delta)
-                elif isinstance(i, (int, float, np.number)):
-                    parseddata.append(float(i))
-            return parseddata
-        else:
-            if isinstance(data, str):
-                return str_to_uts(
-                    timestamp=data, format=None, timezone=timezone, strict=True
-                )
-            else:
-                return float(data)
+import os
+import pickle
+import json
+import datetime
+import dateutil.parser
+import logging
+from zoneinfo import ZoneInfo
+import numpy as np
+from typing import Callable, Union, Mapping, Iterable
+from dgbowl_schemas.yadg.dataschema_5_0.externaldate import ExternalDate
+from dgbowl_schemas.yadg.dataschema_5_0.timestamp import TimestampSpec
+
+
+logger = logging.getLogger(__name__)
+
+
+def now(
+    asstr: bool = False, tz: datetime.timezone = datetime.timezone.utc
+) -> Union[float, str]:
+    """
+    Wrapper around datetime.now()
+
+    A convenience function for returning the current time as a ISO 8601 or as a unix timestamp.
+    """
+    dt = datetime.datetime.now(tz=tz)
+    if asstr:
+        return dt.strftime("%Y-%m-%d %H:%M:%S")
+    else:
+        return dt.timestamp()
+
+
+def ole_to_uts(ole_timestamp: float, timezone: ZoneInfo) -> float:
+    """
+    Converts a Microsoft OLE timestamp into a POSIX timestamp.
+
+    The OLE automation date format is a floating point value, counting
+    days since midnight 30 December 1899. Hours and minutes are
+    represented as fractional days.
+
+    https://devblogs.microsoft.com/oldnewthing/20030905-02/?p=42653
+
+    Parameters
+    ----------
+    ole_timestamp
+        A timestamp in Microsoft OLE format.
+    timezone
+        String desribing the timezone.
+
+    Returns
+    -------
+    time: float
+        The corresponding Unix timestamp.
+
+    """
+    ole_base = datetime.datetime(year=1899, month=12, day=30, tzinfo=timezone)
+    ole_delta = datetime.timedelta(days=ole_timestamp)
+    time = ole_base + ole_delta
+    return time.timestamp()
+
+
+def str_to_uts(
+    *, timestamp: str, timezone: ZoneInfo, format: str = None, strict: bool = True
+) -> Union[float, None]:
+    """
+    Converts a string to POSIX timestamp.
+
+    If the optional ``format`` is specified, the ``timestamp`` string is processed
+    using the :func:`datetime.datetime.strptime` function; if no ``format`` is
+    supplied, an ISO 8601 format is assumed and an attempt to parse using
+    :func:`dateutil.parser.parse` is made.
+
+    Parameters
+    ----------
+    timestamp
+        A string containing the timestamp.
+
+    format
+        Optional format string for parsing of the ``timestamp``.
+
+    timezone
+        Optional timezone of the ``timestamp``. By default, "UTC".
+
+    strict
+        Whether to re-raise any parsing errors.
+
+    Returns
+    -------
+    uts: Union[float, None]
+        Returns the POSIX timestamp if successful, otherwise None.
+
+    """
+
+    try:
+        if format is None:
+            dt = dateutil.parser.parse(timestamp)
+        else:
+            dt = datetime.datetime.strptime(timestamp, format)
+
+        local_tz = timezone if dt.tzinfo is None else dt.tzinfo
+        local_dt = dt.replace(tzinfo=local_tz)
+        utc_dt = local_dt.astimezone(datetime.timezone.utc)
+        return utc_dt.timestamp()
+    except (dateutil.parser.ParserError, ValueError) as e:
+        if strict:
+            raise e
+        else:
+            logger.info(
+                "Parsing timestamp '%s' with format '%s' was not successful.",
+                str(timestamp),
+                format,
+            )
+            return None
+
+
+def infer_timestamp_from(
+    *,
+    headers: list = None,
+    spec: TimestampSpec = None,
+    timezone: ZoneInfo,
+) -> tuple[list, Callable, bool]:
+    """
+    Convenience function for timestamping
+
+    Given a set of headers, and an optional specification, return an array containing
+    column indices from which a timestamp in a given row can be computed, as well as the
+    function which will compute the timestamp given the returned array.
+
+    Parameters
+    ----------
+    headers
+        An array of strings. If `spec` is not supplied, must contain either "uts"
+        :class:`(float)` or "timestep" :class:`(str)` (conforming to ISO 8601).
+
+    spec
+        A specification of timestamp elements with associated column indices and
+        optional formats. Currently accepted combinations of keys are: "uts"; "timestamp";
+        "date" and / or "time".
+
+    tz
+        Timezone to use for conversion. By default, UTC is used.
+
+    Returns
+    -------
+    (datecolumns, datefunc, fulldate): tuple[list, Callable, bool]
+        A tuple containing a list of indices of columns, a Callable to which the
+        columns have to be passed to obtain a uts timestamp, and whether the determined
+        timestamp is full or partial.
+
+    """
+
+    if spec is not None:
+        if hasattr(spec, "uts"):
+            return [spec.uts.index], float, True
+        elif hasattr(spec, "timestamp"):
+
+            def retfunc(value):
+                return str_to_uts(
+                    timestamp=value, format=spec.timestamp.format, timezone=timezone
+                )
+
+            return [spec.timestamp.index], retfunc, True
+        elif hasattr(spec, "date") or hasattr(spec, "time"):
+            specdict = {
+                "date": datetime.datetime.fromtimestamp(0).timestamp,
+                "time": datetime.datetime.fromtimestamp(0).timestamp,
+            }
+            cols = [None, None]
+            if spec.date is not None:
+
+                def datefn(value):
+                    return str_to_uts(
+                        timestamp=value, format=spec.date.format, timezone=timezone
+                    )
+
+                cols[0] = spec.date.index
+                specdict["date"] = datefn
+            if spec.time is not None:
+                if spec.time.format is not None:
+
+                    def timefn(value):
+                        t = datetime.datetime.strptime(value, spec.time.format)
+                        td = datetime.timedelta(
+                            hours=t.hour,
+                            minutes=t.minute,
+                            seconds=t.second,
+                            microseconds=t.microsecond,
+                        )
+                        return td.total_seconds()
+
+                else:
+                    logger.debug(
+                        "Assuming specified column containing the time is in ISO 8601 format"
+                    )
+
+                    def timefn(value):
+                        t = datetime.time.fromisoformat(value)
+                        td = datetime.timedelta(
+                            hours=t.hour,
+                            minutes=t.minute,
+                            seconds=t.second,
+                            microseconds=t.microsecond,
+                        )
+                        return td.total_seconds()
+
+                cols[1] = spec.time.index
+                specdict["time"] = timefn
+            if cols[0] is None:
+                return [cols[1]], specdict["time"], False
+            elif cols[1] is None:
+                return [cols[0]], specdict["date"], False
+            else:
+
+                def retfn(date, time):
+                    return specdict["date"](date) + specdict["time"](time)
+
+                return cols, retfn, True
+    elif "uts" in headers:
+        logger.debug(
+            "No timestamp spec provided, assuming column 'uts' is a valid unix timestamp"
+        )
+        return [headers.index("uts")], float, True
+    elif "timestamp" in headers:
+        logger.debug(
+            "No timestamp spec provided, assuming column 'timestamp' is a valid ISO 8601 timestamp"
+        )
+
+        def retfunc(value):
+            return str_to_uts(timestamp=value, timezone=timezone)
+
+        return [headers.index("timestamp")], retfunc, True
+    else:
+        assert False, "dateutils: A valid timestamp could not be deduced."
+
+
+def complete_timestamps(
+    *,
+    timesteps: list,
+    fn: str,
+    spec: ExternalDate,
+    timezone: ZoneInfo,
+) -> list[float]:
+    """
+    Timestamp completing function.
+
+    This function allows for completing or overriding the uts timestamps determined by
+    the individual parsers. **yadg** enters this function for any parser which does not
+    return a full timestamp, as well as if the ``externaldate`` specification is
+    specified by the user.
+
+    The ``externaldate`` specification is as follows:
+
+    .. autopydantic_model:: dgbowl_schemas.yadg.dataschema_5_0.externaldate.ExternalDate
+       :noindex:
+
+    The ``using`` key specifies how an external timestamp is created. Only one entry in
+    ``using`` is permitted. By default, this entry is:
+
+    .. code-block:: yaml
+
+        using:
+          filename:
+            format: "%Y-%m-%d-%H-%M-%S"
+            len: 19
+
+    Which means the code will attempt to deduce the timestamp from the path of the
+    processed file (``fn``), using the first 19 characters of the base filename
+    according to the above format (eg. "2021-12-31-13-45-00").
+
+    If ``file`` is specified, the handling of timestamps is handed off to
+    :func:`timestamps_from_file`.
+
+    The ``mode`` key specifies whether the offsets determined in this function are
+    added to the current timestamps (eg. date offset being added to time) or whether
+    they should replace the existing timestamps completely.
+
+    As a measure of last resort, the ``mtime`` of the ``fn`` is used. ``mtime`` is
+    preferred to ``ctime``, as the former has a more consistent cross-platform
+    behaviour.
+
+    Parameters
+    ----------
+    timesteps
+        A list of timesteps generated from a single file, ``fn``.
+
+    fn
+        Filename used to create ``timesteps``.
+
+    spec
+        ``externaldate`` specification part of the `schema`.
+
+    timezone
+        Timezone, defaults to "UTC".
+
+    """
+    delta = None
+
+    fulldate = True
+    if spec is not None:
+        replace = spec.mode == "replace"
+        method = spec.using
+    else:
+        replace = False
+        method = None
+
+    if hasattr(method, "file"):
+        delta = timestamps_from_file(
+            method.file.path, method.file.type, method.file.match, timezone
+        )
+    elif hasattr(method, "isostring"):
+        delta = str_to_uts(
+            timestamp=method.isostring, format=None, timezone=timezone, strict=True
+        )
+    elif hasattr(method, "utsoffset"):
+        delta = method.utsoffset
+    elif hasattr(method, "filename"):
+        basename = os.path.basename(fn)
+        filename, ext = os.path.splitext(basename)
+        string = filename[: method.filename.len]
+        delta = str_to_uts(
+            timestamp=string,
+            format=method.filename.format,
+            timezone=timezone,
+            strict=False,
+        )
+
+    if delta is None:
+        logger.warning("Timestamp completion failed. Using 'mtime'.")
+        delta = os.path.getmtime(fn)
+        fulldate = False
+
+    if isinstance(delta, float):
+        delta = [delta] * len(timesteps)
+
+    assert len(delta) == len(timesteps)
+
+    if replace:
+        timesteps = delta
+    else:
+        timesteps = timesteps + delta
+
+    return timesteps, fulldate
+
+
+def timestamps_from_file(
+    path: str,
+    type: str,
+    match: str,
+    timezone: ZoneInfo,
+) -> Union[float, list[float]]:
+    """
+    Load timestamps from file.
+
+    This function enables loading timestamps from file specified by the ``path``.
+    The currently supported file formats include ``json`` and ``pkl``, which must
+    contain a top-level :class:`Mapping` with a key that is matched by ``match``,
+    or a top-level :class:`Iterable`, both containing :class:`str` or :class:`float`
+    -like objects that can be processed into an Unix timestamp.
+
+    Parameters
+    ----------
+    path
+        Location of the external file.
+
+    type
+        Type of the external file. Currently, ``"json", "pkl"`` are supported.
+
+    match
+        An optional key to match if the object in ``path`` is a :class:`Mapping`.
+
+    timezone
+        An optional timezone string, defaults to "UTC"
+
+    Returns
+    -------
+    parseddata: Union[float, list[float]]
+        A single or a list of POSIX timestamps.
+
+    """
+    assert os.path.exists(path), f"timestamps_from_file: path '{path}' doesn't exist."
+    assert os.path.isfile(path), f"timestamps_from_file: Path '{path}' is not a file."
+
+    if type == "pkl":
+        logger.debug("Loading '%s' as pickle.", path)
+        with open(path, "rb") as infile:
+            data = pickle.load(infile)
+    elif type == "json":
+        logger.debug("Loading '%s' as json.", path)
+        with open(path, "r") as infile:
+            data = json.load(infile)
+    elif type == "agilent.log":
+        logger.critical("Type 'agilent.log' not yet supported.")
+        data = None
+
+    if data is None:
+        return data
+    elif isinstance(data, Iterable):
+        if isinstance(data, Mapping):
+            assert match in data
+            data = data[match]
+        if isinstance(data, Iterable):
+            parseddata = []
+            for i in data:
+                if isinstance(i, str):
+                    delta = str_to_uts(
+                        timestamp=i, format=None, timezone=timezone, strict=True
+                    )
+                    parseddata.append(delta)
+                elif isinstance(i, (int, float, np.number)):
+                    parseddata.append(float(i))
+            return parseddata
+        else:
+            if isinstance(data, str):
+                return str_to_uts(
+                    timestamp=data, format=None, timezone=timezone, strict=True
+                )
+            else:
+                return float(data)
```

### Comparing `yadg-5.0.1/src/yadg/dgutils/pintutils.py` & `yadg-5.0.2/src/yadg/dgutils/pintutils.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,81 +1,81 @@
-"""
-``pint`` compatibility functions in **yadg**.
-
-This package defines ``ureg``, a :class:`pint.UnitRegistry` used for validation of
-`datagrams` in **yadg**. The default SI :class:`pint.UnitRegistry` is extended
-by definitions of fractional quantities (%, ppm, etc.), standard volumetric
-quantities (smL/min, sccm), and other dimensionless "units" present in several
-file types.
-"""
-import logging
-from typing import Union
-import pint
-
-logger = logging.getLogger(__name__)
-
-ureg = pint.UnitRegistry(
-    preprocessors=[
-        lambda s: s.replace("%%", " permille "),
-        lambda s: s.replace("%", " percent "),
-    ]
-)
-
-definitions = """
-parts_per_hundred = 1e-2 count = percent
-parts_per_thousand = 1e-3 count = ‰ = promile = permille
-parts_per_million = 1e-6 count = ppm
-parts_per_billion = 1e-9 count = ppb
-
-standard_milliliter = milliliter = smL
-standard_liter = liter = sL
-standard_cubic_centimeter_minute = cm^3/min = sccm
-
-refractive_index_units = [] = RIU
-"""
-
-for line in definitions.split("\n"):
-    line = line.strip()
-    if len(line) > 0 and not line.startswith("#"):
-        ureg.define(line)
-
-
-def _sanitize_helper(unit: str) -> str:
-    unit = unit.replace("Bar", "bar")
-    if unit in ["deg C", "Deg C"]:
-        return "degC"
-    else:
-        return unit
-
-
-def sanitize_units(
-    units: Union[str, dict[str, str], list[str]]
-) -> Union[str, dict[str, str], list[str]]:
-    """
-    Unit sanitizer.
-
-    This sanitizer should be used where user-supplied units are likely to occur,
-    such as in the parsers :mod:`yadg.parsers.basiccsv`. Currently, only two
-    replacements are done:
-
-      - "Bar" is replaced with "bar"
-      - "Deg C" is replace with "degC
-
-    Use with caution.
-
-    Parameters
-    ----------
-    units
-        Object containing string units.
-
-    """
-    if isinstance(units, list):
-        for i in range(len(units)):
-            units[i] = _sanitize_helper(units[i])
-    elif isinstance(units, dict):
-        for k, v in units.items():
-            units[k] = _sanitize_helper(v)
-    elif isinstance(units, str):
-        units = _sanitize_helper(units)
-    else:
-        logger.error("Supplied type of 'units' not understood: '%s'", str(type(units)))
-    return units
+"""
+``pint`` compatibility functions in **yadg**.
+
+This package defines ``ureg``, a :class:`pint.UnitRegistry` used for validation of
+`datagrams` in **yadg**. The default SI :class:`pint.UnitRegistry` is extended
+by definitions of fractional quantities (%, ppm, etc.), standard volumetric
+quantities (smL/min, sccm), and other dimensionless "units" present in several
+file types.
+"""
+import logging
+from typing import Union
+import pint
+
+logger = logging.getLogger(__name__)
+
+ureg = pint.UnitRegistry(
+    preprocessors=[
+        lambda s: s.replace("%%", " permille "),
+        lambda s: s.replace("%", " percent "),
+    ]
+)
+
+definitions = """
+parts_per_hundred = 1e-2 count = percent
+parts_per_thousand = 1e-3 count = ‰ = promile = permille
+parts_per_million = 1e-6 count = ppm
+parts_per_billion = 1e-9 count = ppb
+
+standard_milliliter = milliliter = smL
+standard_liter = liter = sL
+standard_cubic_centimeter_minute = cm^3/min = sccm
+
+refractive_index_units = [] = RIU
+"""
+
+for line in definitions.split("\n"):
+    line = line.strip()
+    if len(line) > 0 and not line.startswith("#"):
+        ureg.define(line)
+
+
+def _sanitize_helper(unit: str) -> str:
+    unit = unit.replace("Bar", "bar")
+    if unit in ["deg C", "Deg C"]:
+        return "degC"
+    else:
+        return unit
+
+
+def sanitize_units(
+    units: Union[str, dict[str, str], list[str]]
+) -> Union[str, dict[str, str], list[str]]:
+    """
+    Unit sanitizer.
+
+    This sanitizer should be used where user-supplied units are likely to occur,
+    such as in the parsers :mod:`yadg.parsers.basiccsv`. Currently, only two
+    replacements are done:
+
+      - "Bar" is replaced with "bar"
+      - "Deg C" is replace with "degC
+
+    Use with caution.
+
+    Parameters
+    ----------
+    units
+        Object containing string units.
+
+    """
+    if isinstance(units, list):
+        for i in range(len(units)):
+            units[i] = _sanitize_helper(units[i])
+    elif isinstance(units, dict):
+        for k, v in units.items():
+            units[k] = _sanitize_helper(v)
+    elif isinstance(units, str):
+        units = _sanitize_helper(units)
+    else:
+        logger.error("Supplied type of 'units' not understood: '%s'", str(type(units)))
+    return units
```

### Comparing `yadg-5.0.1/src/yadg/dgutils/utils.py` & `yadg-5.0.2/src/yadg/dgutils/utils.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,173 +1,173 @@
-import logging
-import os
-from typing import Union
-from dgbowl_schemas.yadg import to_dataschema
-from dgbowl_schemas.yadg.dataschema import DataSchema
-
-from .. import dgutils
-
-logger = logging.getLogger(__name__)
-
-
-def calib_3to4(oldcal: dict, caltype: str) -> dict:
-    newcal = {}
-    if caltype == "calfile":
-        for k, v in oldcal["detectors"].items():
-            pd = {
-                "window": (v.get("window", 3) - 1) // 2,
-                "polyorder": v.get("poly", 2),
-                "prominence": v.get("prominence", 1.0),
-                "threshold": v.get("threshold", 1.0),
-            }
-            sp = {}
-            for kk, vv in v["species"].items():
-                if kk == "units" and vv == "min":
-                    continue
-                spec = {
-                    "l": vv["l"] * 60.0,
-                    "r": vv["r"] * 60.0,
-                    "calib": {"inverse": {"slope": vv.get("rf", 1.0)}},
-                }
-                sp[kk] = spec
-            id = {"det_1": 0, "det_2": 1}[v["id"]]
-            newcal[k] = {"id": id, "peakdetect": pd, "species": sp}
-    elif caltype == "Tcalfile":
-        newcal = {"T": {"T_f": {"calib": {"linear": oldcal}}, "unit": "degC"}}
-    elif caltype == "MFCcalfile":
-        newcal = {}
-        for k, v in oldcal.items():
-            items = v.get("content", {k: 1.0})
-            for kk, vv in items.items():
-                if kk not in newcal:
-                    newcal[kk] = {"unit": "ml/min"}
-                newcal[kk][k] = {
-                    "calib": {
-                        "linear": {
-                            "slope": v.get("slope", 1.0),
-                            "intercept": v.get("intercept", 0.0),
-                        }
-                    },
-                    "fraction": vv,
-                }
-    return newcal
-
-
-def schema_3to4(oldschema: list) -> dict:
-    newschema = {
-        "metadata": {
-            "provenance": {
-                "type": "yadg update",
-                "metadata": {
-                    "yadg": dgutils.get_yadg_metadata(),
-                    "update_schema": {"updater": "schema_3to4"},
-                },
-            },
-            "version": "4.1",
-            "timezone": "localtime",
-        },
-        "steps": [],
-    }
-    for oldstep in oldschema:
-        newstep = {}
-
-        newstep["parser"] = oldstep["datagram"]
-        if newstep["parser"] == "gctrace":
-            newstep["parser"] = "chromtrace"
-
-        if "paths" in oldstep["import"]:
-            oldstep["import"]["files"] = oldstep["import"].pop("paths")
-        newstep["input"] = oldstep["import"]
-
-        if oldstep.get("export", None) is not None:
-            newstep["tag"] = oldstep["export"]
-
-        parameters = {}
-        for k, v in oldstep["parameters"].items():
-            if k in ["Tcalfile", "MFCcalfile", "calfile"]:
-                logger.warning(
-                    "Parsing of post-processing parameter '%s' has been removed in "
-                    "yadg-5.0, please use dgpost-2.0 to reproduce this functionality.",
-                    k,
-                )
-            elif k == "method" and v == "q0refl":
-                logger.warning(
-                    "Parsing of post-processing parameter '%s' has been removed in "
-                    "yadg-5.0, please use dgpost-2.0 to reproduce this functionality.",
-                    k,
-                )
-            else:
-                parameters[k] = v
-        if parameters != {}:
-            newstep["parameters"] = parameters
-        newschema["steps"].append(newstep)
-
-    return newschema
-
-
-def update_schema(object: Union[list, dict]) -> dict:
-    """
-    Yadg's update worker function.
-
-    This is the main function called when **yadg** is executed as ``yadg update``.
-    The main idea is to allow a simple update pathway from older versions of `schema` and
-    ``datagram`` files to the current latest and greatest.
-
-    Currently supports:
-
-     - updating ``DataSchema`` version 3.1 to 4.0 using routines in ``yadg``
-     - updating ``DataSchema`` version 4.0 and above to the latest ``DataSchema``
-
-    Parameters
-    ----------
-    object
-        The object to be updated
-
-    Returns
-    -------
-    newobj: dict
-        The updated and validated `"datagram"` or `"schema"`.
-
-    """
-
-    if isinstance(object, list):
-        logger.info("Updating list-style DataSchema")
-        newobj = schema_3to4(object)
-    elif isinstance(object, dict):
-        logger.info("Updating dict-style DataSchema")
-        newobj = object
-    else:
-        raise ValueError(f"Supplied object is of incorrect type: {type(object)}")
-    newobj = to_dataschema(**newobj)
-    while hasattr(newobj, "update"):
-        newobj = newobj.update()
-    return newobj
-
-
-def schema_from_preset(preset: DataSchema, folder: str) -> DataSchema:
-    preset.metadata.provenance.type = "yadg preset"
-    for step in preset.steps:
-        for fi, fn in enumerate(step.input.files):
-            if os.path.isabs(fn):
-                logger.warning(
-                    "Item '%s' in '%s' is an absolute path and will not be patched.",
-                    fn,
-                    step,
-                )
-            else:
-                step.input.files[fi] = os.path.abspath(os.path.join(folder, fn))
-        if (
-            step.externaldate is not None
-            and hasattr(step.externaldate.using, "file")
-            and step.externaldate.using.file is not None
-        ):
-            oldf = step.externaldate.using.file.path
-            if os.path.isabs(oldf):
-                logger.warning(
-                    "Specified externaldate file '%s' is an absolute path "
-                    "and will not be patched.",
-                    oldf,
-                )
-            else:
-                newf = os.path.abspath(os.path.join(folder, oldf))
-                step.externaldate.using.file.path = newf
-    return preset
+import logging
+import os
+from typing import Union
+from dgbowl_schemas.yadg import to_dataschema
+from dgbowl_schemas.yadg.dataschema import DataSchema
+
+from .. import dgutils
+
+logger = logging.getLogger(__name__)
+
+
+def calib_3to4(oldcal: dict, caltype: str) -> dict:
+    newcal = {}
+    if caltype == "calfile":
+        for k, v in oldcal["detectors"].items():
+            pd = {
+                "window": (v.get("window", 3) - 1) // 2,
+                "polyorder": v.get("poly", 2),
+                "prominence": v.get("prominence", 1.0),
+                "threshold": v.get("threshold", 1.0),
+            }
+            sp = {}
+            for kk, vv in v["species"].items():
+                if kk == "units" and vv == "min":
+                    continue
+                spec = {
+                    "l": vv["l"] * 60.0,
+                    "r": vv["r"] * 60.0,
+                    "calib": {"inverse": {"slope": vv.get("rf", 1.0)}},
+                }
+                sp[kk] = spec
+            id = {"det_1": 0, "det_2": 1}[v["id"]]
+            newcal[k] = {"id": id, "peakdetect": pd, "species": sp}
+    elif caltype == "Tcalfile":
+        newcal = {"T": {"T_f": {"calib": {"linear": oldcal}}, "unit": "degC"}}
+    elif caltype == "MFCcalfile":
+        newcal = {}
+        for k, v in oldcal.items():
+            items = v.get("content", {k: 1.0})
+            for kk, vv in items.items():
+                if kk not in newcal:
+                    newcal[kk] = {"unit": "ml/min"}
+                newcal[kk][k] = {
+                    "calib": {
+                        "linear": {
+                            "slope": v.get("slope", 1.0),
+                            "intercept": v.get("intercept", 0.0),
+                        }
+                    },
+                    "fraction": vv,
+                }
+    return newcal
+
+
+def schema_3to4(oldschema: list) -> dict:
+    newschema = {
+        "metadata": {
+            "provenance": {
+                "type": "yadg update",
+                "metadata": {
+                    "yadg": dgutils.get_yadg_metadata(),
+                    "update_schema": {"updater": "schema_3to4"},
+                },
+            },
+            "version": "4.1",
+            "timezone": "localtime",
+        },
+        "steps": [],
+    }
+    for oldstep in oldschema:
+        newstep = {}
+
+        newstep["parser"] = oldstep["datagram"]
+        if newstep["parser"] == "gctrace":
+            newstep["parser"] = "chromtrace"
+
+        if "paths" in oldstep["import"]:
+            oldstep["import"]["files"] = oldstep["import"].pop("paths")
+        newstep["input"] = oldstep["import"]
+
+        if oldstep.get("export", None) is not None:
+            newstep["tag"] = oldstep["export"]
+
+        parameters = {}
+        for k, v in oldstep["parameters"].items():
+            if k in ["Tcalfile", "MFCcalfile", "calfile"]:
+                logger.warning(
+                    "Parsing of post-processing parameter '%s' has been removed in "
+                    "yadg-5.0, please use dgpost-2.0 to reproduce this functionality.",
+                    k,
+                )
+            elif k == "method" and v == "q0refl":
+                logger.warning(
+                    "Parsing of post-processing parameter '%s' has been removed in "
+                    "yadg-5.0, please use dgpost-2.0 to reproduce this functionality.",
+                    k,
+                )
+            else:
+                parameters[k] = v
+        if parameters != {}:
+            newstep["parameters"] = parameters
+        newschema["steps"].append(newstep)
+
+    return newschema
+
+
+def update_schema(object: Union[list, dict]) -> dict:
+    """
+    Yadg's update worker function.
+
+    This is the main function called when **yadg** is executed as ``yadg update``.
+    The main idea is to allow a simple update pathway from older versions of `schema` and
+    ``datagram`` files to the current latest and greatest.
+
+    Currently supports:
+
+     - updating ``DataSchema`` version 3.1 to 4.0 using routines in ``yadg``
+     - updating ``DataSchema`` version 4.0 and above to the latest ``DataSchema``
+
+    Parameters
+    ----------
+    object
+        The object to be updated
+
+    Returns
+    -------
+    newobj: dict
+        The updated and validated `"datagram"` or `"schema"`.
+
+    """
+
+    if isinstance(object, list):
+        logger.info("Updating list-style DataSchema")
+        newobj = schema_3to4(object)
+    elif isinstance(object, dict):
+        logger.info("Updating dict-style DataSchema")
+        newobj = object
+    else:
+        raise ValueError(f"Supplied object is of incorrect type: {type(object)}")
+    newobj = to_dataschema(**newobj)
+    while hasattr(newobj, "update"):
+        newobj = newobj.update()
+    return newobj
+
+
+def schema_from_preset(preset: DataSchema, folder: str) -> DataSchema:
+    preset.metadata.provenance.type = "yadg preset"
+    for step in preset.steps:
+        for fi, fn in enumerate(step.input.files):
+            if os.path.isabs(fn):
+                logger.warning(
+                    "Item '%s' in '%s' is an absolute path and will not be patched.",
+                    fn,
+                    step,
+                )
+            else:
+                step.input.files[fi] = os.path.abspath(os.path.join(folder, fn))
+        if (
+            step.externaldate is not None
+            and hasattr(step.externaldate.using, "file")
+            and step.externaldate.using.file is not None
+        ):
+            oldf = step.externaldate.using.file.path
+            if os.path.isabs(oldf):
+                logger.warning(
+                    "Specified externaldate file '%s' is an absolute path "
+                    "and will not be patched.",
+                    oldf,
+                )
+            else:
+                newf = os.path.abspath(os.path.join(folder, oldf))
+                step.externaldate.using.file.path = newf
+    return preset
```

### Comparing `yadg-5.0.1/src/yadg/parsers/basiccsv/__init__.py` & `yadg-5.0.2/src/yadg/parsers/basiccsv/__init__.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-"""
-Handles the reading and processing of any tabular files, as long as the first line
-contains the column headers. By default, the second should contain the units. The
-columns of the table must be separated using a separator such as ``,``, ``;``,
-or ``\\t``.
-
-.. warning::
-
-  Since ``yadg-5.0``, the parser handles sparse tables (i.e. tables with missing
-  data) by back-filling empty cells with ``np.NaNs``.
-
-.. note::
-
-  :mod:`~yadg.parsers.basiccsv` attempts to deduce the timestamp from the column
-  headers, using :func:`yadg.dgutils.dateutils.infer_timestamp_from`. Alternatively,
-  the column(s) containing the timestamp data and their format can be provided using
-  parameters.
-
-Usage
-`````
-Available since ``yadg-4.0``. The parser supports the following parameters:
-
-.. _yadg.parsers.basiccsv.model:
-
-.. autopydantic_model:: dgbowl_schemas.yadg.dataschema_5_0.step.BasicCSV
-
-Schema
-``````
-The primary functionality of :mod:`~yadg.parsers.basiccsv` is to load the tabular
-data, and determine the Unix timestamp. The headers of the tabular data are taken
-`verbatim` from the file, and appear as ``data_vars`` of the :class:`xarray.Dataset`.
-The single ``coord`` for the ``data_vars`` is the deduced Unix timestamp, ``uts``.
-
-.. code-block:: yaml
-
-  xr.Dataset:
-    coords:
-      uts:            !!float               # Unix timestamp
-    data_vars:
-      {{ headers }}:  (uts)                 # Populated from file headers
-
-Module Functions
-````````````````
-
-"""
-
-from .main import process
-
-__all__ = ["process"]
+"""
+Handles the reading and processing of any tabular files, as long as the first line
+contains the column headers. By default, the second should contain the units. The
+columns of the table must be separated using a separator such as ``,``, ``;``,
+or ``\\t``.
+
+.. warning::
+
+  Since ``yadg-5.0``, the parser handles sparse tables (i.e. tables with missing
+  data) by back-filling empty cells with ``np.NaNs``.
+
+.. note::
+
+  :mod:`~yadg.parsers.basiccsv` attempts to deduce the timestamp from the column
+  headers, using :func:`yadg.dgutils.dateutils.infer_timestamp_from`. Alternatively,
+  the column(s) containing the timestamp data and their format can be provided using
+  parameters.
+
+Usage
+`````
+Available since ``yadg-4.0``. The parser supports the following parameters:
+
+.. _yadg.parsers.basiccsv.model:
+
+.. autopydantic_model:: dgbowl_schemas.yadg.dataschema_5_0.step.BasicCSV
+
+Schema
+``````
+The primary functionality of :mod:`~yadg.parsers.basiccsv` is to load the tabular
+data, and determine the Unix timestamp. The headers of the tabular data are taken
+`verbatim` from the file, and appear as ``data_vars`` of the :class:`xarray.Dataset`.
+The single ``coord`` for the ``data_vars`` is the deduced Unix timestamp, ``uts``.
+
+.. code-block:: yaml
+
+  xr.Dataset:
+    coords:
+      uts:            !!float               # Unix timestamp
+    data_vars:
+      {{ headers }}:  (uts)                 # Populated from file headers
+
+Module Functions
+````````````````
+
+"""
+
+from .main import process
+
+__all__ = ["process"]
```

### Comparing `yadg-5.0.1/src/yadg/parsers/basiccsv/main.py` & `yadg-5.0.2/src/yadg/parsers/basiccsv/main.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,230 +1,230 @@
-import logging
-from uncertainties.core import str_to_number_with_uncert as tuple_fromstr
-from typing import Callable, Any
-from pydantic import BaseModel
-import locale as lc
-from ... import dgutils
-
-import numpy as np
-import xarray as xr
-
-logger = logging.getLogger(__name__)
-
-
-def process_row(
-    headers: list,
-    items: list,
-    datefunc: Callable,
-    datecolumns: list,
-) -> tuple[dict, dict]:
-    """
-    A function that processes a row of a table.
-
-    This is the main worker function of :mod:`~yadg.parsers.basiccsv`, but is often
-    re-used by any other parser that needs to process tabular data.
-
-    Parameters
-    ----------
-    headers
-        A list of headers of the table.
-
-    items
-        A list of values corresponding to the headers. Must be the same length as headers.
-
-    units
-        A dict for looking up the units corresponding to a certain header.
-
-    datefunc
-        A function that will generate ``uts`` given a list of values.
-
-    datecolumns
-        Column indices that need to be passed to ``datefunc`` to generate uts.
-
-    Returns
-    -------
-    vals, devs
-        A tuple of result dictionaries, with the first element containing the values
-        and the second element containing the deviations of the values.
-
-    """
-    assert len(headers) == len(items), (
-        f"process_row: Length mismatch between provided headers: "
-        f"{headers} and  provided items: {items}."
-    )
-
-    vals = {}
-    devs = {}
-    columns = [column.strip() for column in items]
-
-    # Process raw data, assign sigma and units
-    vals["uts"] = datefunc(*[columns[i] for i in datecolumns])
-    for ci, header in enumerate(headers):
-        if ci in datecolumns:
-            continue
-        elif columns[ci] == "":
-            continue
-        try:
-            val, dev = tuple_fromstr(lc.delocalize(columns[ci]))
-            vals[header] = val
-            devs[header] = dev
-        except ValueError:
-            vals[header] = columns[ci]
-
-    return vals, devs
-
-
-def append_dicts(
-    vals: dict[str, Any],
-    devs: dict[str, Any],
-    data: dict[str, list[Any]],
-    meta: dict[str, list[Any]],
-    fn: str = None,
-    li: int = 0,
-) -> None:
-    if "_fn" in meta and fn is not None:
-        meta["_fn"].append(str(fn))
-    for k, v in vals.items():
-        if k not in data:
-            data[k] = [None if isinstance(v, str) else np.nan] * li
-        data[k].append(v)
-    for k, v in devs.items():
-        if k not in meta:
-            meta[k] = [np.nan] * li
-        meta[k].append(v)
-
-    for k in set(data) - set(vals):
-        data[k].append(np.nan)
-    for k in set(meta) - set(devs):
-        if k != "_fn":
-            meta[k].append(np.nan)
-
-
-def dicts_to_dataset(
-    data: dict[str, list[Any]],
-    meta: dict[str, list[Any]],
-    units: dict[str, str] = dict(),
-    fulldate: bool = True,
-) -> xr.Dataset:
-    darrs = {}
-    for k, v in data.items():
-        attrs = {}
-        u = units.get(k, None)
-        if u is not None:
-            attrs["units"] = u
-        if k == "uts":
-            continue
-        darrs[k] = xr.DataArray(data=v, dims=["uts"], attrs=attrs)
-        if k in meta and darrs[k].dtype.kind in {"i", "u", "f", "c", "m", "M"}:
-            err = f"{k}_std_err"
-            darrs[k].attrs["ancillary_variables"] = err
-            attrs["standard_name"] = f"{k} standard error"
-            darrs[err] = xr.DataArray(data=meta[k], dims=["uts"], attrs=attrs)
-    if "uts" in data:
-        coords = dict(uts=data.pop("uts"))
-    else:
-        coords = dict()
-    if fulldate:
-        attrs = dict()
-    else:
-        attrs = dict(fulldate=False)
-    return xr.Dataset(data_vars=darrs, coords=coords, attrs=attrs)
-
-
-def process(
-    *,
-    fn: str,
-    encoding: str,
-    locale: str,
-    timezone: str,
-    parameters: BaseModel,
-    **kwargs: dict,
-) -> xr.Dataset:
-    """
-    A basic csv parser.
-
-    This parser processes a csv file. The header of the csv file consists of one or two
-    lines, with the column headers in the first line and the units in the second. The
-    parser also attempts to parse column names to produce a timestamp, and save all other
-    columns as floats or strings.
-
-    Parameters
-    ----------
-    fn
-        File to process
-
-    encoding
-        Encoding of ``fn``, by default "utf-8".
-
-    timezone
-        A string description of the timezone. Default is "localtime".
-
-    parameters
-        Parameters for :class:`~dgbowl_schemas.yadg.dataschema_5_0.step.BasicCSV`.
-
-    Returns
-    -------
-    :class:`xarray.Dataset`
-        No metadata is returned by the :mod:`~yadg.parsers.basiccsv` parser. The full
-        date might not be returned, eg. when only time is specified in columns.
-
-    """
-
-    if hasattr(parameters, "strip"):
-        strip = parameters.strip
-    else:
-        strip = None
-
-    # Load file, extract headers and get timestamping function
-    with open(fn, "r", encoding=encoding) as infile:
-        # This decode/encode is done to account for some csv files that have a BOM
-        # at the beginning of each line.
-        lines = [i.encode().decode(encoding) for i in infile.readlines()]
-    assert len(lines) >= 2
-    headers = [h.strip().strip(strip) for h in lines[0].split(parameters.sep)]
-
-    for hi, header in enumerate(headers):
-        if "/" in header:
-            logger.warning("Replacing '/' for '_' in header '%s'.", header)
-            headers[hi] = header.replace("/", "_")
-
-    datecolumns, datefunc, fulldate = dgutils.infer_timestamp_from(
-        headers=headers, spec=parameters.timestamp, timezone=timezone
-    )
-
-    # Populate units
-    units = parameters.units
-    if units is None:
-        units = {}
-        _units = [c.strip().strip(strip) for c in lines[1].split(parameters.sep)]
-        for header in headers:
-            units[header] = _units.pop(0)
-        si = 2
-    else:
-        for header in headers:
-            if header not in units:
-                logger.warning(
-                    "Using implicit dimensionless unit ' ' for '%s'.", header
-                )
-                units[header] = " "
-            elif units[header] == "":
-                units[header] = " "
-        si = 1
-
-    units = dgutils.sanitize_units(units)
-
-    # Process rows
-    old_loc = lc.getlocale(category=lc.LC_NUMERIC)
-    lc.setlocale(lc.LC_NUMERIC, locale=locale)
-    data_vals = {}
-    meta_vals = {"_fn": []}
-    for li, line in enumerate(lines[si:]):
-        vals, devs = process_row(
-            headers,
-            [i.strip().strip(strip) for i in line.split(parameters.sep)],
-            datefunc,
-            datecolumns,
-        )
-        append_dicts(vals, devs, data_vals, meta_vals, fn, li)
-    lc.setlocale(category=lc.LC_NUMERIC, locale=old_loc)
-
-    return dicts_to_dataset(data_vals, meta_vals, units, fulldate)
+import logging
+from uncertainties.core import str_to_number_with_uncert as tuple_fromstr
+from typing import Callable, Any
+from pydantic import BaseModel
+import locale as lc
+from ... import dgutils
+
+import numpy as np
+import xarray as xr
+
+logger = logging.getLogger(__name__)
+
+
+def process_row(
+    headers: list,
+    items: list,
+    datefunc: Callable,
+    datecolumns: list,
+) -> tuple[dict, dict]:
+    """
+    A function that processes a row of a table.
+
+    This is the main worker function of :mod:`~yadg.parsers.basiccsv`, but is often
+    re-used by any other parser that needs to process tabular data.
+
+    Parameters
+    ----------
+    headers
+        A list of headers of the table.
+
+    items
+        A list of values corresponding to the headers. Must be the same length as headers.
+
+    units
+        A dict for looking up the units corresponding to a certain header.
+
+    datefunc
+        A function that will generate ``uts`` given a list of values.
+
+    datecolumns
+        Column indices that need to be passed to ``datefunc`` to generate uts.
+
+    Returns
+    -------
+    vals, devs
+        A tuple of result dictionaries, with the first element containing the values
+        and the second element containing the deviations of the values.
+
+    """
+    assert len(headers) == len(items), (
+        f"process_row: Length mismatch between provided headers: "
+        f"{headers} and  provided items: {items}."
+    )
+
+    vals = {}
+    devs = {}
+    columns = [column.strip() for column in items]
+
+    # Process raw data, assign sigma and units
+    vals["uts"] = datefunc(*[columns[i] for i in datecolumns])
+    for ci, header in enumerate(headers):
+        if ci in datecolumns:
+            continue
+        elif columns[ci] == "":
+            continue
+        try:
+            val, dev = tuple_fromstr(lc.delocalize(columns[ci]))
+            vals[header] = val
+            devs[header] = dev
+        except ValueError:
+            vals[header] = columns[ci]
+
+    return vals, devs
+
+
+def append_dicts(
+    vals: dict[str, Any],
+    devs: dict[str, Any],
+    data: dict[str, list[Any]],
+    meta: dict[str, list[Any]],
+    fn: str = None,
+    li: int = 0,
+) -> None:
+    if "_fn" in meta and fn is not None:
+        meta["_fn"].append(str(fn))
+    for k, v in vals.items():
+        if k not in data:
+            data[k] = [None if isinstance(v, str) else np.nan] * li
+        data[k].append(v)
+    for k, v in devs.items():
+        if k not in meta:
+            meta[k] = [np.nan] * li
+        meta[k].append(v)
+
+    for k in set(data) - set(vals):
+        data[k].append(np.nan)
+    for k in set(meta) - set(devs):
+        if k != "_fn":
+            meta[k].append(np.nan)
+
+
+def dicts_to_dataset(
+    data: dict[str, list[Any]],
+    meta: dict[str, list[Any]],
+    units: dict[str, str] = dict(),
+    fulldate: bool = True,
+) -> xr.Dataset:
+    darrs = {}
+    for k, v in data.items():
+        attrs = {}
+        u = units.get(k, None)
+        if u is not None:
+            attrs["units"] = u
+        if k == "uts":
+            continue
+        darrs[k] = xr.DataArray(data=v, dims=["uts"], attrs=attrs)
+        if k in meta and darrs[k].dtype.kind in {"i", "u", "f", "c", "m", "M"}:
+            err = f"{k}_std_err"
+            darrs[k].attrs["ancillary_variables"] = err
+            attrs["standard_name"] = f"{k} standard error"
+            darrs[err] = xr.DataArray(data=meta[k], dims=["uts"], attrs=attrs)
+    if "uts" in data:
+        coords = dict(uts=data.pop("uts"))
+    else:
+        coords = dict()
+    if fulldate:
+        attrs = dict()
+    else:
+        attrs = dict(fulldate=False)
+    return xr.Dataset(data_vars=darrs, coords=coords, attrs=attrs)
+
+
+def process(
+    *,
+    fn: str,
+    encoding: str,
+    locale: str,
+    timezone: str,
+    parameters: BaseModel,
+    **kwargs: dict,
+) -> xr.Dataset:
+    """
+    A basic csv parser.
+
+    This parser processes a csv file. The header of the csv file consists of one or two
+    lines, with the column headers in the first line and the units in the second. The
+    parser also attempts to parse column names to produce a timestamp, and save all other
+    columns as floats or strings.
+
+    Parameters
+    ----------
+    fn
+        File to process
+
+    encoding
+        Encoding of ``fn``, by default "utf-8".
+
+    timezone
+        A string description of the timezone. Default is "localtime".
+
+    parameters
+        Parameters for :class:`~dgbowl_schemas.yadg.dataschema_5_0.step.BasicCSV`.
+
+    Returns
+    -------
+    :class:`xarray.Dataset`
+        No metadata is returned by the :mod:`~yadg.parsers.basiccsv` parser. The full
+        date might not be returned, eg. when only time is specified in columns.
+
+    """
+
+    if hasattr(parameters, "strip"):
+        strip = parameters.strip
+    else:
+        strip = None
+
+    # Load file, extract headers and get timestamping function
+    with open(fn, "r", encoding=encoding) as infile:
+        # This decode/encode is done to account for some csv files that have a BOM
+        # at the beginning of each line.
+        lines = [i.encode().decode(encoding) for i in infile.readlines()]
+    assert len(lines) >= 2
+    headers = [h.strip().strip(strip) for h in lines[0].split(parameters.sep)]
+
+    for hi, header in enumerate(headers):
+        if "/" in header:
+            logger.warning("Replacing '/' for '_' in header '%s'.", header)
+            headers[hi] = header.replace("/", "_")
+
+    datecolumns, datefunc, fulldate = dgutils.infer_timestamp_from(
+        headers=headers, spec=parameters.timestamp, timezone=timezone
+    )
+
+    # Populate units
+    units = parameters.units
+    if units is None:
+        units = {}
+        _units = [c.strip().strip(strip) for c in lines[1].split(parameters.sep)]
+        for header in headers:
+            units[header] = _units.pop(0)
+        si = 2
+    else:
+        for header in headers:
+            if header not in units:
+                logger.warning(
+                    "Using implicit dimensionless unit ' ' for '%s'.", header
+                )
+                units[header] = " "
+            elif units[header] == "":
+                units[header] = " "
+        si = 1
+
+    units = dgutils.sanitize_units(units)
+
+    # Process rows
+    old_loc = lc.getlocale(category=lc.LC_NUMERIC)
+    lc.setlocale(lc.LC_NUMERIC, locale=locale)
+    data_vals = {}
+    meta_vals = {"_fn": []}
+    for li, line in enumerate(lines[si:]):
+        vals, devs = process_row(
+            headers,
+            [i.strip().strip(strip) for i in line.split(parameters.sep)],
+            datefunc,
+            datecolumns,
+        )
+        append_dicts(vals, devs, data_vals, meta_vals, fn, li)
+    lc.setlocale(category=lc.LC_NUMERIC, locale=old_loc)
+
+    return dicts_to_dataset(data_vals, meta_vals, units, fulldate)
```

### Comparing `yadg-5.0.1/src/yadg/parsers/chromdata/empalccsv.py` & `yadg-5.0.2/src/yadg/parsers/chromdata/empalcxlsx.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,224 +1,219 @@
-"""
-**empalccsv**: Processing Empa's online LC exported data (csv)
---------------------------------------------------------------
-
-This is a structured format produced by the export from Agilent's Online LC device
-at Empa. It contains three sections:
-
-  - metadata section,
-  - table containing sampling information,
-  - table containing analysed chromatography data.
-
-.. codeauthor:: Peter Kraus
-"""
-import logging
-import datetime
-from uncertainties.core import str_to_number_with_uncert as tuple_fromstr
-import xarray as xr
-import numpy as np
-
-logger = logging.getLogger(__name__)
-
-
-def process(*, fn: str, encoding: str, **kwargs: dict) -> xr.Dataset:
-    """
-    Custom Agilent Online LC csv export format.
-
-    Multiple chromatograms per file, with multiple detectors.
-
-    Parameters
-    ----------
-    fn
-        Filename to process.
-
-    encoding
-        Encoding used to open the file.
-
-    Returns
-    -------
-    :class:`xarray.Dataset`
-
-    """
-
-    with open(fn, "r", encoding=encoding, errors="ignore") as infile:
-        lines = infile.readlines()
-
-    metadata = {}
-    while len(lines) > 0:
-        line = lines.pop(0)
-        if len(lines) == 0:
-            raise RuntimeError(
-                f"Last line of file '{fn}' read during metadata section."
-            )
-        elif line.strip() == "":
-            break
-        elif line.strip().startswith("Sequence name"):
-            metadata["sequence"] = line.split(":,")[1]
-        elif line.strip().startswith("Description"):
-            metadata["description"] = line.split(":,")[1]
-        elif line.strip().startswith("Acquired by"):
-            metadata["username"] = line.split(":,")[1]
-        elif line.strip().startswith("Data path"):
-            metadata["datafile"] = line.split(":,")[1]
-        elif line.strip().startswith("Report version"):
-            metadata["version"] = int(line.split(":,")[1])
-
-    if metadata.get("version", None) is None:
-        raise RuntimeError(f"Report version in file '{fn}' was not specified.")
-
-    samples = {}
-    while len(lines) > 0:
-        line = lines.pop(0)
-        if len(lines) == 0:
-            raise RuntimeError(f"Last line of file '{fn}' read during samples section.")
-        elif line.strip() == "":
-            break
-        elif "Line#" in line:
-            headers = [i.strip() for i in line.split(",")]
-        else:
-            data = [i.strip() for i in line.split(",")]
-            sample = {
-                "location": data[headers.index("Location")],
-                "injection date": data[headers.index("Injection Date")],
-                "acquisition": {
-                    "method": data[headers.index("Acq Method Name")],
-                    "version": data[headers.index("Acq Method Version")],
-                },
-                "integration": {
-                    "method": data[headers.index("Injection DA Method Name")],
-                    "version": data[headers.index("Injection DA Method Version")],
-                },
-                "offset": data[headers.index("Time offset")],
-            }
-            if sample["offset"] != "":
-                sn = data[headers.index("Sample Name")]
-                samples[sn] = sample
-
-    svals = samples.values()
-    if len(svals) == 0:
-        raise RuntimeError(
-            f"No complete sample data found in file '{fn}'. "
-            "Have you added time offsets?"
-        )
-    r = next(iter(svals))
-    # check that acquisition and integration methods are consistent throughout file:
-    if any([s["acquisition"]["method"] != r["acquisition"]["method"] for s in svals]):
-        logger.warning("Acquisition method is inconsistent in file '%s'.", fn)
-    if any([s["integration"]["method"] != r["integration"]["method"] for s in svals]):
-        logger.warning("Integration method is inconsistent in file '%s'.", fn)
-
-    metadata["method"] = r["acquisition"]["method"]
-
-    species = set()
-    while len(lines) > 0:
-        line = lines.pop(0)
-        if len(lines) == 0:
-            break
-        elif line.strip() == "":
-            break
-        elif "Line#" in line:
-            headers = [i.strip() for i in line.split(",")]
-        else:
-            data = [i.strip() for i in line.split(",")]
-            sn = data[headers.index("Sample Name")]
-            cn = data[headers.index("Compound")]
-            species.add(cn)
-
-            h = data[headers.index("Peak Height")]
-            if h != "":
-                if "height" not in samples[sn]:
-                    samples[sn]["height"] = {}
-                samples[sn]["height"][cn] = tuple_fromstr(h)
-
-            A = data[headers.index("Area")]
-            if A != "":
-                if "area" not in samples[sn]:
-                    samples[sn]["area"] = {}
-                samples[sn]["area"][cn] = tuple_fromstr(A)
-
-            if metadata["version"] == 2:
-                c = data[headers.index("Concentration")]
-            else:
-                logger.warning(
-                    "Report version '%d' in file '%s' not understood.",
-                    metadata["version"],
-                    fn,
-                )
-                c = data[headers.index("Concentration")]
-            if c != "":
-                if "concentration" not in samples[sn]:
-                    samples[sn]["concentration"] = {}
-                samples[sn]["concentration"][cn] = tuple_fromstr(c)
-
-            rt = data[headers.index("RT [min]")]
-            if rt != "":
-                if "retention time" not in samples[sn]:
-                    samples[sn]["retention time"] = {}
-                samples[sn]["retention time"][cn] = tuple_fromstr(rt)
-    units = {
-        "height": None,
-        "area": None,
-        "concentration": "mmol/l",
-        "retention time": "min",
-    }
-    species = sorted(species)
-    data = []
-    for k, v in samples.items():
-        # Remove unnecessary parameters
-        del v["acquisition"]
-        del v["integration"]
-        v["sampleid"] = k
-        # Process offset to uts
-        offset = v.pop("offset")
-        t = None
-        for fmt in {"%H:%M:%S"}:
-            try:
-                t = datetime.datetime.strptime(offset, fmt)
-            except ValueError:
-                continue
-        if t is None:
-            try:
-                td = datetime.timedelta(minutes=float(offset))
-            except ValueError:
-                raise RuntimeError(
-                    f"It was not possible to parse offset '{offset}' present in file "
-                    f"'{fn}' using known formats."
-                )
-        else:
-            td = datetime.timedelta(hours=t.hour, minutes=t.minute, seconds=t.second)
-        point = {"uts": td.total_seconds()}
-        vals = {}
-        devs = {}
-        for kk in {"height", "area", "concentration", "retention time"}:
-            val = v.get(kk, {})
-            vals[kk], devs[kk] = zip(*[val.get(cn, (np.nan, np.nan)) for cn in species])
-        point["vals"] = vals
-        point["devs"] = devs
-        data.append(point)
-
-    data_vars = {}
-    for kk in {"height", "area", "concentration", "retention time"}:
-        data_vars[kk] = (
-            ["uts", "species"],
-            [i["vals"][kk] for i in data],
-            {"anciliary_variables": f"{kk}_std_err"},
-        )
-        data_vars[f"{kk}_std_err"] = (
-            ["uts", "species"],
-            [i["devs"][kk] for i in data],
-            {"standard_name": f"{kk} standard_error"},
-        )
-        if units[kk] is not None:
-            data_vars[kk][2]["units"] = units[kk]
-            data_vars[f"{kk}_std_err"][2]["units"] = units[kk]
-
-    ds = xr.Dataset(
-        data_vars=data_vars,
-        coords={
-            "species": (["species"], species),
-            "uts": (["uts"], [i["uts"] for i in data]),
-        },
-        attrs=metadata,
-    )
-
-    return ds
+"""
+**empalcxlsx**: Processing Empa's online LC exported data (xlsx)
+----------------------------------------------------------------
+
+This is a structured format produced by the export from Agilent's Online LC device
+at Empa. It contains three sections:
+
+  - metadata section,
+  - table containing sampling information,
+  - table containing analysed chromatography data.
+
+
+.. codeauthor:: Peter Kraus
+"""
+import logging
+import datetime
+import openpyxl
+from uncertainties.core import str_to_number_with_uncert as tuple_fromstr
+import xarray as xr
+import numpy as np
+
+logger = logging.getLogger(__name__)
+
+
+def process(*, fn: str, **kwargs: dict) -> xr.Dataset:
+    """
+    Fusion xlsx export format.
+
+    Multiple chromatograms per file, with multiple detectors.
+
+    Parameters
+    ----------
+    fn
+        Filename to process.
+
+    Returns
+    -------
+    :class:`xarray.Dataset`
+
+    """
+    try:
+        wb = openpyxl.load_workbook(
+            filename=fn,
+            read_only=True,
+        )
+    except TypeError:
+        raise RuntimeError(
+            f"Could not read the file '{fn}' using openpyxl. Try to open and save the "
+            f"file in Excel."
+        )
+
+    ws = wb["Page 1"]
+    metadata = {}
+    for row in ws.rows:
+        val = row[1].value if len(row) > 1 else ""
+        if row[0].value.startswith("Sequence name"):
+            metadata["sequence"] = val
+        elif row[0].value.startswith("Description"):
+            metadata["description"] = val
+        elif row[0].value.startswith("Acquired by"):
+            metadata["username"] = val
+        elif row[0].value.startswith("Data path"):
+            metadata["datafile"] = val
+        elif row[0].value.startswith("Report version"):
+            metadata["version"] = int(val)
+
+    if metadata.get("version", None) is None:
+        raise RuntimeError(f"Report version in file '{fn}' was not specified.")
+
+    ws = wb["Page 2"]
+    samples = {}
+    for row in ws.rows:
+        if "Line#" in row[0].value:
+            headers = [i.value.replace("\n", "").replace(" ", "") for i in row]
+        else:
+            data = [str(i.value) if i.value is not None else None for i in row]
+            sample = {
+                "location": data[headers.index("Location")],
+                "injection date": data[headers.index("InjectionDate")],
+                "acquisition": {
+                    "method": data[headers.index("AcqMethodName")],
+                    "version": data[headers.index("AcqMethodVersion")],
+                },
+                "integration": {
+                    "method": data[headers.index("InjectionDAMethodName")],
+                    "version": data[headers.index("InjectionDAMethodVersion")],
+                },
+                "offset": data[headers.index("Timeoffset")],
+            }
+            if sample["offset"] is not None:
+                sn = data[headers.index("SampleName")]
+                sn = sn.replace(" ", "").replace("\n", "")
+                samples[sn] = sample
+
+    svals = samples.values()
+    if len(svals) == 0:
+        raise RuntimeError(
+            f"No complete sample data found in file '{fn}'. "
+            "Have you added time offsets?"
+        )
+    r = next(iter(svals))
+    # check that acquisition and integration methods are consistent throughout file:
+    if any([s["acquisition"]["method"] != r["acquisition"]["method"] for s in svals]):
+        logger.warning("Acquisition method is inconsistent in file '%s'.", fn)
+    if any([s["integration"]["method"] != r["integration"]["method"] for s in svals]):
+        logger.warning("Integration method is inconsistent in file '%s'.", fn)
+
+    metadata["method"] = r["acquisition"]["method"].replace("\n", "").replace(" ", "")
+
+    species = set()
+    ws = wb["Page 3"]
+    for row in ws.rows:
+        if "Line#" in str(row[0].value):
+            headers = [i.value.replace("\n", "").replace(" ", "") for i in row]
+        else:
+            data = [str(i.value) if i.value is not None else None for i in row]
+            sn = data[headers.index("SampleName")].replace("\n", "").replace(" ", "")
+            cn = data[headers.index("Compound")]
+            species.add(cn)
+
+            h = data[headers.index("PeakHeight")]
+            if h is not None:
+                if "height" not in samples[sn]:
+                    samples[sn]["height"] = {}
+                samples[sn]["height"][cn] = tuple_fromstr(h)
+
+            A = data[headers.index("Area")]
+            if A is not None:
+                if "area" not in samples[sn]:
+                    samples[sn]["area"] = {}
+                samples[sn]["area"][cn] = tuple_fromstr(A)
+
+            if metadata["version"] == 2:
+                c = data[headers.index("Concentration")]
+            else:
+                logger.warning(
+                    "Report version '%d' in file '%s' not understood.",
+                    metadata["version"],
+                    fn,
+                )
+                c = data[headers.index("Concentration")]
+            if c is not None:
+                if "concentration" not in samples[sn]:
+                    samples[sn]["concentration"] = {}
+                samples[sn]["concentration"][cn] = tuple_fromstr(c)
+
+            rt = data[headers.index("RT[min]")]
+            if rt is not None:
+                if "retention time" not in samples[sn]:
+                    samples[sn]["retention time"] = {}
+                samples[sn]["retention time"][cn] = tuple_fromstr(rt)
+
+    units = {
+        "height": None,
+        "area": None,
+        "concentration": "mmol/l",
+        "retention time": "min",
+    }
+    species = sorted(species)
+    data = []
+    for k, v in samples.items():
+        # Remove unnecessary parameters
+        del v["acquisition"]
+        del v["integration"]
+        v["sampleid"] = k
+        # Process offset to uts
+        offset = v.pop("offset")
+        t = None
+        for fmt in {"%H:%M:%S"}:
+            try:
+                t = datetime.datetime.strptime(offset, fmt)
+            except ValueError:
+                continue
+        if t is None:
+            try:
+                td = datetime.timedelta(minutes=float(offset))
+            except ValueError:
+                raise RuntimeError(
+                    f"It was not possible to parse offset '{offset}' present in file "
+                    f"'{fn}' using known formats."
+                )
+        else:
+            td = datetime.timedelta(hours=t.hour, minutes=t.minute, seconds=t.second)
+        point = {"uts": td.total_seconds()}
+        vals = {}
+        devs = {}
+        for kk in {"height", "area", "concentration", "retention time"}:
+            val = v.get(kk, {})
+            vals[kk], devs[kk] = zip(*[val.get(cn, (np.nan, np.nan)) for cn in species])
+        point["vals"] = vals
+        point["devs"] = devs
+        data.append(point)
+
+    data_vars = {}
+    for kk in {"height", "area", "concentration", "retention time"}:
+        data_vars[kk] = (
+            ["uts", "species"],
+            [i["vals"][kk] for i in data],
+            {"anciliary_variables": f"{kk}_std_err"},
+        )
+        data_vars[f"{kk}_std_err"] = (
+            ["uts", "species"],
+            [i["devs"][kk] for i in data],
+            {"standard_name": f"{kk} standard_error"},
+        )
+        if units[kk] is not None:
+            data_vars[kk][2]["units"] = units[kk]
+            data_vars[f"{kk}_std_err"][2]["units"] = units[kk]
+
+    ds = xr.Dataset(
+        data_vars=data_vars,
+        coords={
+            "species": (["species"], species),
+            "uts": (["uts"], [i["uts"] for i in data]),
+        },
+        attrs=metadata,
+    )
+
+    return ds
```

### Comparing `yadg-5.0.1/src/yadg/parsers/chromdata/fusioncsv.py` & `yadg-5.0.2/src/yadg/parsers/chromdata/fusioncsv.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,145 +1,145 @@
-"""
-**fusioncsv**: Processing Inficon Fusion csv export format (csv).
-------------------------------------------------------------------
-
-This is a tabulated format, including the concentrations, mole fractions, peak
-areas, and retention times. The latter is ignored by this parser.
-
-.. warning::
-
-    As also mentioned in the ``csv`` files themselves, the use of this filetype
-    is discouraged, and the ``json`` files (or a zipped archive of them) should
-    be parsed instead.
-
-.. codeauthor:: Peter Kraus
-"""
-import logging
-from zoneinfo import ZoneInfo
-from ...dgutils.dateutils import str_to_uts
-from uncertainties.core import str_to_number_with_uncert as tuple_fromstr
-import xarray as xr
-import numpy as np
-
-logger = logging.getLogger(__name__)
-
-data_names = {
-    "Concentration": "concentration",
-    "NormalizedConcentration": "xout",
-    "Area": "area",
-    "RT(s)": "retention time",
-}
-
-data_units = {
-    "concentration": "%",
-    "xout": "%",
-    "area": None,
-    "retention time": "s",
-}
-
-
-def process(
-    *, fn: str, encoding: str, timezone: ZoneInfo, **kwargs: dict
-) -> xr.Dataset:
-    """
-    Fusion csv export format.
-
-    Multiple chromatograms per file, with multiple detectors.
-
-    Parameters
-    ----------
-    fn
-        Filename to process.
-
-    encoding
-        Encoding used to open the file.
-
-    timezone
-        Timezone information. This should be ``"localtime"``.
-
-    Returns
-    -------
-    :class:`xarray.Dataset`
-
-    """
-
-    with open(fn, "r", encoding=encoding, errors="ignore") as infile:
-        lines = infile.readlines()
-
-    data = []
-    species = set()
-    for line in lines[3:]:
-        if "SampleName" in line:
-            header = [i.strip() for i in line.split(",")]
-            sni = header.index("SampleName")
-            method = header[0]
-            for ii, i in enumerate(header):
-                if i == "":
-                    header[ii] = header[ii - 1]
-        elif "Detectors" in line:
-            detectors = [i.replace('"', "").strip() for i in line.split(",")]
-            for ii, i in enumerate(detectors):
-                if i == "":
-                    detectors[ii] = detectors[ii - 1]
-        elif "Time" in line:
-            samples = [i.replace('"', "").strip() for i in line.split(",")]
-            time = samples[0]
-            if time == "Time (GMT 120 mins)":
-                offset = "+02:00"
-            elif time == "Time (GMT 60 mins)":
-                offset = "+01:00"
-            else:
-                logger.error("offset '%s' not understood", time)
-                offset = "+00:00"
-        elif "% RSD" in line:
-            continue
-        else:
-            items = line.split(",")
-            point = {
-                "concentration": {},
-                "xout": {},
-                "area": {},
-                "retention time": {},
-                "sampleid": items[sni],
-                "uts": str_to_uts(timestamp=f"{items[0]}{offset}", timezone=timezone),
-            }
-            for ii, i in enumerate(items[2:]):
-                ii += 2
-                species.add(samples[ii])
-                point[data_names[header[ii]]][samples[ii]] = tuple_fromstr(i)
-            data.append(point)
-
-    species = sorted(species)
-    data_vars = {}
-    for kk in {"concentration", "xout", "area", "retention time"}:
-        vals = []
-        devs = []
-        for i in range(len(data)):
-            ivals, idevs = zip(
-                *[data[i][kk].get(cn, (np.nan, np.nan)) for cn in species]
-            )
-            vals.append(ivals)
-            devs.append(idevs)
-        data_vars[kk] = (
-            ["uts", "species"],
-            vals,
-            {"anciliary_variables": f"{kk}_std_err"},
-        )
-        data_vars[f"{kk}_std_err"] = (
-            ["uts", "species"],
-            devs,
-            {"standard_name": f"{kk} standard_error"},
-        )
-        if data_units[kk] is not None:
-            data_vars[kk][2]["units"] = data_units[kk]
-            data_vars[f"{kk}_std_err"][2]["units"] = data_units[kk]
-
-    ds = xr.Dataset(
-        data_vars=data_vars,
-        coords={
-            "species": (["species"], species),
-            "uts": (["uts"], [i["uts"] for i in data]),
-        },
-        attrs=dict(method=method),
-    )
-
-    return ds
+"""
+**fusioncsv**: Processing Inficon Fusion csv export format (csv).
+------------------------------------------------------------------
+
+This is a tabulated format, including the concentrations, mole fractions, peak
+areas, and retention times. The latter is ignored by this parser.
+
+.. warning::
+
+    As also mentioned in the ``csv`` files themselves, the use of this filetype
+    is discouraged, and the ``json`` files (or a zipped archive of them) should
+    be parsed instead.
+
+.. codeauthor:: Peter Kraus
+"""
+import logging
+from zoneinfo import ZoneInfo
+from ...dgutils.dateutils import str_to_uts
+from uncertainties.core import str_to_number_with_uncert as tuple_fromstr
+import xarray as xr
+import numpy as np
+
+logger = logging.getLogger(__name__)
+
+data_names = {
+    "Concentration": "concentration",
+    "NormalizedConcentration": "xout",
+    "Area": "area",
+    "RT(s)": "retention time",
+}
+
+data_units = {
+    "concentration": "%",
+    "xout": "%",
+    "area": None,
+    "retention time": "s",
+}
+
+
+def process(
+    *, fn: str, encoding: str, timezone: ZoneInfo, **kwargs: dict
+) -> xr.Dataset:
+    """
+    Fusion csv export format.
+
+    Multiple chromatograms per file, with multiple detectors.
+
+    Parameters
+    ----------
+    fn
+        Filename to process.
+
+    encoding
+        Encoding used to open the file.
+
+    timezone
+        Timezone information. This should be ``"localtime"``.
+
+    Returns
+    -------
+    :class:`xarray.Dataset`
+
+    """
+
+    with open(fn, "r", encoding=encoding, errors="ignore") as infile:
+        lines = infile.readlines()
+
+    data = []
+    species = set()
+    for line in lines[3:]:
+        if "SampleName" in line:
+            header = [i.strip() for i in line.split(",")]
+            sni = header.index("SampleName")
+            method = header[0]
+            for ii, i in enumerate(header):
+                if i == "":
+                    header[ii] = header[ii - 1]
+        elif "Detectors" in line:
+            detectors = [i.replace('"', "").strip() for i in line.split(",")]
+            for ii, i in enumerate(detectors):
+                if i == "":
+                    detectors[ii] = detectors[ii - 1]
+        elif "Time" in line:
+            samples = [i.replace('"', "").strip() for i in line.split(",")]
+            time = samples[0]
+            if time == "Time (GMT 120 mins)":
+                offset = "+02:00"
+            elif time == "Time (GMT 60 mins)":
+                offset = "+01:00"
+            else:
+                logger.error("offset '%s' not understood", time)
+                offset = "+00:00"
+        elif "% RSD" in line:
+            continue
+        else:
+            items = line.split(",")
+            point = {
+                "concentration": {},
+                "xout": {},
+                "area": {},
+                "retention time": {},
+                "sampleid": items[sni],
+                "uts": str_to_uts(timestamp=f"{items[0]}{offset}", timezone=timezone),
+            }
+            for ii, i in enumerate(items[2:]):
+                ii += 2
+                species.add(samples[ii])
+                point[data_names[header[ii]]][samples[ii]] = tuple_fromstr(i)
+            data.append(point)
+
+    species = sorted(species)
+    data_vars = {}
+    for kk in {"concentration", "xout", "area", "retention time"}:
+        vals = []
+        devs = []
+        for i in range(len(data)):
+            ivals, idevs = zip(
+                *[data[i][kk].get(cn, (np.nan, np.nan)) for cn in species]
+            )
+            vals.append(ivals)
+            devs.append(idevs)
+        data_vars[kk] = (
+            ["uts", "species"],
+            vals,
+            {"anciliary_variables": f"{kk}_std_err"},
+        )
+        data_vars[f"{kk}_std_err"] = (
+            ["uts", "species"],
+            devs,
+            {"standard_name": f"{kk} standard_error"},
+        )
+        if data_units[kk] is not None:
+            data_vars[kk][2]["units"] = data_units[kk]
+            data_vars[f"{kk}_std_err"][2]["units"] = data_units[kk]
+
+    ds = xr.Dataset(
+        data_vars=data_vars,
+        coords={
+            "species": (["species"], species),
+            "uts": (["uts"], [i["uts"] for i in data]),
+        },
+        attrs=dict(method=method),
+    )
+
+    return ds
```

### Comparing `yadg-5.0.1/src/yadg/parsers/chromdata/fusionjson.py` & `yadg-5.0.2/src/yadg/parsers/chromdata/fusionjson.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,156 +1,156 @@
-"""
-**fusionjson**: Processing Inficon Fusion json data format (json).
-------------------------------------------------------------------
-
-This is a fairly detailed data format, including the traces, the calibration applied,
-and also the integrated peak areas and other processed information, which are parsed
-by this module.
-
-.. note ::
-
-    To parse the raw trace data, use the :mod:`~yadg.parsers.chromtrace` module.
-
-.. warning ::
-
-    The detectors in the json files are not necessarily in a consistent order. To
-    avoid inconsistent parsing of species which appear in both detectors, the
-    detector keys are sorted. **Species present in both detectors** will be
-    **overwritten by the last detector** in alphabetical order.
-
-Exposed metadata:
-`````````````````
-
-.. code-block:: yaml
-
-    params:
-      method:   !!str
-      username: None
-      version:  !!str
-      datafile: !!str
-
-.. codeauthor:: Peter Kraus
-"""
-import json
-import logging
-from zoneinfo import ZoneInfo
-from ...dgutils.dateutils import str_to_uts
-import xarray as xr
-import numpy as np
-
-logger = logging.getLogger(__name__)
-
-
-def process(
-    *, fn: str, encoding: str, timezone: ZoneInfo, **kwargs: dict
-) -> xr.Dataset:
-    """
-    Fusion json format.
-
-    One chromatogram per file with multiple traces, and pre-analysed results.
-    Only a subset of the metadata is retained, including the method name,
-    detector names, and information about assigned peaks.
-
-    Parameters
-    ----------
-    fn
-        Filename to process.
-
-    encoding
-        Encoding used to open the file.
-
-    timezone
-        Timezone information. This should be ``"localtime"``.
-
-    Returns
-    -------
-    :class:`xarray.Dataset`
-
-    """
-
-    with open(fn, "r", encoding=encoding, errors="ignore") as infile:
-        jsdata = json.load(infile)
-    metadata = {
-        "method": jsdata.get("methodName", "n/a"),
-        "version": jsdata.get("softwareVersion", {}).get("version", None),
-        "datafile": jsdata.get("sequence", {}).get("location", None),
-    }
-    uts = str_to_uts(timestamp=jsdata["runTimeStamp"], timezone=timezone)
-
-    sampleid = jsdata.get("annotations", {}).get("name", None)
-    if sampleid is not None:
-        metadata["sampleid"] = sampleid
-
-    units = {
-        "height": None,
-        "area": None,
-        "concentration": "%",
-        "xout": "%",
-        "retention time": "s",
-    }
-
-    raw = {
-        "height": {},
-        "area": {},
-        "concentration": {},
-        "xout": {},
-        "retention time": {},
-    }
-
-    species = set()
-
-    # sort detector keys to ensure alphabetic order for ID matching
-    for detname in sorted(jsdata["detectors"].keys()):
-        detdict = jsdata["detectors"][detname]
-        if "analysis" in detdict:
-            for peak in detdict["analysis"]["peaks"]:
-                if "label" not in peak:
-                    continue
-                else:
-                    species.add(peak["label"])
-                if "height" in peak:
-                    raw["height"][peak["label"]] = (float(peak["height"]), 1.0)
-                if "area" in peak:
-                    raw["area"][peak["label"]] = (float(peak["area"]), 0.01)
-                if "concentration" in peak:
-                    raw["concentration"][peak["label"]] = (
-                        float(peak["concentration"]),
-                        float(peak["concentration"]) * 1e-3,
-                    )
-                if "normalizedConcentration" in peak:
-                    raw["xout"][peak["label"]] = (
-                        float(peak["normalizedConcentration"]),
-                        float(peak["normalizedConcentration"]) * 1e-3,
-                    )
-                if "top" in peak:
-                    raw["retention time"][peak["label"]] = (float(peak["top"]), 0.01)
-        else:
-            logger.warning("'analysis' of chromatogram not present in file '%s'", fn)
-
-    valve = jsdata.get("annotations", {}).get("valcoPosition", None)
-    if valve is not None:
-        raw["valve"] = valve
-
-    species = sorted(species)
-    data_vars = {}
-    for k, v in units.items():
-        vals, devs = zip(*[raw[k].get(s, (np.nan, np.nan)) for s in species])
-        data_vars[k] = (
-            ["uts", "species"],
-            [vals],
-            {"ancillary_variables": f"{k}_std_err"},
-        )
-        data_vars[f"{k}_std_err"] = (
-            ["uts", "species"],
-            [devs],
-            {"standard_name": f"{k} stdandard_error"},
-        )
-        if v is not None:
-            data_vars[k][2]["units"] = v
-            data_vars[f"{k}_std_err"][2]["units"] = v
-
-    ds = xr.Dataset(
-        data_vars=data_vars,
-        coords={"species": (["species"], species), "uts": (["uts"], [uts])},
-        attrs=metadata,
-    )
-    return ds
+"""
+**fusionjson**: Processing Inficon Fusion json data format (json).
+------------------------------------------------------------------
+
+This is a fairly detailed data format, including the traces, the calibration applied,
+and also the integrated peak areas and other processed information, which are parsed
+by this module.
+
+.. note ::
+
+    To parse the raw trace data, use the :mod:`~yadg.parsers.chromtrace` module.
+
+.. warning ::
+
+    The detectors in the json files are not necessarily in a consistent order. To
+    avoid inconsistent parsing of species which appear in both detectors, the
+    detector keys are sorted. **Species present in both detectors** will be
+    **overwritten by the last detector** in alphabetical order.
+
+Exposed metadata:
+`````````````````
+
+.. code-block:: yaml
+
+    params:
+      method:   !!str
+      username: None
+      version:  !!str
+      datafile: !!str
+
+.. codeauthor:: Peter Kraus
+"""
+import json
+import logging
+from zoneinfo import ZoneInfo
+from ...dgutils.dateutils import str_to_uts
+import xarray as xr
+import numpy as np
+
+logger = logging.getLogger(__name__)
+
+
+def process(
+    *, fn: str, encoding: str, timezone: ZoneInfo, **kwargs: dict
+) -> xr.Dataset:
+    """
+    Fusion json format.
+
+    One chromatogram per file with multiple traces, and pre-analysed results.
+    Only a subset of the metadata is retained, including the method name,
+    detector names, and information about assigned peaks.
+
+    Parameters
+    ----------
+    fn
+        Filename to process.
+
+    encoding
+        Encoding used to open the file.
+
+    timezone
+        Timezone information. This should be ``"localtime"``.
+
+    Returns
+    -------
+    :class:`xarray.Dataset`
+
+    """
+
+    with open(fn, "r", encoding=encoding, errors="ignore") as infile:
+        jsdata = json.load(infile)
+    metadata = {
+        "method": jsdata.get("methodName", "n/a"),
+        "version": jsdata.get("softwareVersion", {}).get("version", None),
+        "datafile": jsdata.get("sequence", {}).get("location", None),
+    }
+    uts = str_to_uts(timestamp=jsdata["runTimeStamp"], timezone=timezone)
+
+    sampleid = jsdata.get("annotations", {}).get("name", None)
+    if sampleid is not None:
+        metadata["sampleid"] = sampleid
+
+    units = {
+        "height": None,
+        "area": None,
+        "concentration": "%",
+        "xout": "%",
+        "retention time": "s",
+    }
+
+    raw = {
+        "height": {},
+        "area": {},
+        "concentration": {},
+        "xout": {},
+        "retention time": {},
+    }
+
+    species = set()
+
+    # sort detector keys to ensure alphabetic order for ID matching
+    for detname in sorted(jsdata["detectors"].keys()):
+        detdict = jsdata["detectors"][detname]
+        if "analysis" in detdict:
+            for peak in detdict["analysis"]["peaks"]:
+                if "label" not in peak:
+                    continue
+                else:
+                    species.add(peak["label"])
+                if "height" in peak:
+                    raw["height"][peak["label"]] = (float(peak["height"]), 1.0)
+                if "area" in peak:
+                    raw["area"][peak["label"]] = (float(peak["area"]), 0.01)
+                if "concentration" in peak:
+                    raw["concentration"][peak["label"]] = (
+                        float(peak["concentration"]),
+                        float(peak["concentration"]) * 1e-3,
+                    )
+                if "normalizedConcentration" in peak:
+                    raw["xout"][peak["label"]] = (
+                        float(peak["normalizedConcentration"]),
+                        float(peak["normalizedConcentration"]) * 1e-3,
+                    )
+                if "top" in peak:
+                    raw["retention time"][peak["label"]] = (float(peak["top"]), 0.01)
+        else:
+            logger.warning("'analysis' of chromatogram not present in file '%s'", fn)
+
+    valve = jsdata.get("annotations", {}).get("valcoPosition", None)
+    if valve is not None:
+        raw["valve"] = valve
+
+    species = sorted(species)
+    data_vars = {}
+    for k, v in units.items():
+        vals, devs = zip(*[raw[k].get(s, (np.nan, np.nan)) for s in species])
+        data_vars[k] = (
+            ["uts", "species"],
+            [vals],
+            {"ancillary_variables": f"{k}_std_err"},
+        )
+        data_vars[f"{k}_std_err"] = (
+            ["uts", "species"],
+            [devs],
+            {"standard_name": f"{k} stdandard_error"},
+        )
+        if v is not None:
+            data_vars[k][2]["units"] = v
+            data_vars[f"{k}_std_err"][2]["units"] = v
+
+    ds = xr.Dataset(
+        data_vars=data_vars,
+        coords={"species": (["species"], species), "uts": (["uts"], [uts])},
+        attrs=metadata,
+    )
+    return ds
```

### Comparing `yadg-5.0.1/src/yadg/parsers/chromdata/fusionzip.py` & `yadg-5.0.2/src/yadg/parsers/chromdata/fusionzip.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-"""
-**fusionzip**: Processing Inficon Fusion zipped data format (zip).
-------------------------------------------------------------------
-
-This is a wrapper parser which unzips the provided zip file, and then uses
-the :mod:`yadg.parsers.chromdata.fusionjson` parser to parse every data
-file present in the archive.
-
-.. codeauthor:: Peter Kraus
-"""
-import zipfile
-import tempfile
-import os
-import xarray as xr
-
-from .fusionjson import process as processjson
-
-
-def process(*, fn: str, encoding: str, timezone: str, **kwargs: dict) -> xr.Dataset:
-    """
-    Fusion zip file format.
-
-    The Fusion GC's can export their json formats as a zip archive of a folder
-    of jsons. This parser allows for parsing of this zip archive directly,
-    without the user having to unzip & move the data.
-
-    Parameters
-    ----------
-    fn
-        Filename to process.
-
-    encoding
-        Not used as the file is binary.
-
-    timezone
-        Timezone information. This should be ``"localtime"``.
-
-    Returns
-    -------
-    :class:`xarray.Dataset`
-        The data from the inidividual json files contained in the zip archive are
-        concatenated into a single :class:`xarray.Dataset`. This might fail if the metadata
-        in the json files differs, or if the dimensions are not easily concatenable.
-
-    """
-
-    zf = zipfile.ZipFile(fn)
-    with tempfile.TemporaryDirectory() as tempdir:
-        zf.extractall(tempdir)
-        ds = None
-        for ffn in sorted(os.listdir(tempdir)):
-            ffn = os.path.join(tempdir, ffn)
-            if ffn.endswith("fusion-data"):
-                ids = processjson(fn=ffn, encoding=encoding, timezone=timezone)
-                if ds is None:
-                    ds = ids
-                else:
-                    try:
-                        ds = xr.concat([ds, ids], dim="uts", combine_attrs="identical")
-                    except xr.MergeError:
-                        raise RuntimeError(
-                            "Merging metadata from the unzipped fusion-json files has failed. "
-                            "This might be caused by trying to parse data obtained using "
-                            "different chromatographic methods. Please check the contents "
-                            "of the unzipped files."
-                        )
-    return ds
+"""
+**fusionzip**: Processing Inficon Fusion zipped data format (zip).
+------------------------------------------------------------------
+
+This is a wrapper parser which unzips the provided zip file, and then uses
+the :mod:`yadg.parsers.chromdata.fusionjson` parser to parse every data
+file present in the archive.
+
+.. codeauthor:: Peter Kraus
+"""
+import zipfile
+import tempfile
+import os
+import xarray as xr
+
+from .fusionjson import process as processjson
+
+
+def process(*, fn: str, encoding: str, timezone: str, **kwargs: dict) -> xr.Dataset:
+    """
+    Fusion zip file format.
+
+    The Fusion GC's can export their json formats as a zip archive of a folder
+    of jsons. This parser allows for parsing of this zip archive directly,
+    without the user having to unzip & move the data.
+
+    Parameters
+    ----------
+    fn
+        Filename to process.
+
+    encoding
+        Not used as the file is binary.
+
+    timezone
+        Timezone information. This should be ``"localtime"``.
+
+    Returns
+    -------
+    :class:`xarray.Dataset`
+        The data from the inidividual json files contained in the zip archive are
+        concatenated into a single :class:`xarray.Dataset`. This might fail if the metadata
+        in the json files differs, or if the dimensions are not easily concatenable.
+
+    """
+
+    zf = zipfile.ZipFile(fn)
+    with tempfile.TemporaryDirectory() as tempdir:
+        zf.extractall(tempdir)
+        ds = None
+        for ffn in sorted(os.listdir(tempdir)):
+            ffn = os.path.join(tempdir, ffn)
+            if ffn.endswith("fusion-data"):
+                ids = processjson(fn=ffn, encoding=encoding, timezone=timezone)
+                if ds is None:
+                    ds = ids
+                else:
+                    try:
+                        ds = xr.concat([ds, ids], dim="uts", combine_attrs="identical")
+                    except xr.MergeError:
+                        raise RuntimeError(
+                            "Merging metadata from the unzipped fusion-json files has failed. "
+                            "This might be caused by trying to parse data obtained using "
+                            "different chromatographic methods. Please check the contents "
+                            "of the unzipped files."
+                        )
+    return ds
```

### Comparing `yadg-5.0.1/src/yadg/parsers/chromtrace/__init__.py` & `yadg-5.0.2/src/yadg/parsers/chromtrace/__init__.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,116 +1,116 @@
-"""
-Handles the parsing of raw traces present in chromatography files, whether the source is
-a liquid chromatograph (LC) or a gas chromatograph (GC). The basic function of the
-parser is to:
-
-#. read in the raw data and create timestamped `traces`
-#. collect `metadata` such as the method information, sample ID, etc.
-
-:mod:`~yadg.parsers.chromtrace` loads the chromatographic data from the specified
-file, determines the uncertainties of the signal (y-axis), and explicitly
-populates the points in the time axis (x-axis), when required.
-
-Usage
-`````
-Available since ``yadg-4.0``. The parser supports the following parameters:
-
-.. _yadg.parsers.chromtrace.model:
-
-.. autopydantic_model:: dgbowl_schemas.yadg.dataschema_5_0.step.ChromTrace
-
-.. _yadg.parsers.chromtrace.formats:
-
-Formats
-```````
-The ``filetypes`` currently supported by the parser are:
-
- - EZ-Chrom ASCII export (``ezchrom.asc``):
-   see :mod:`~yadg.parsers.chromtrace.ezchromasc`
- - Agilent Chemstation Chromtab (``agilent.csv``):
-   see :mod:`~yadg.parsers.chromtrace.agilentcsv`
- - Agilent OpenLab binary signal (``agilent.ch``):
-   see :mod:`~yadg.parsers.chromtrace.agilentch`
- - Agilent OpenLab data archive (``agilent.dx``):
-   see :mod:`~yadg.parsers.chromtrace.agilentdx`
- - Inficon Fusion JSON format (``fusion.json``):
-   see :mod:`~yadg.parsers.chromtrace.fusionjson`
- - Inficon Fusion zip archive (``fusion.zip``):
-   see :mod:`~yadg.parsers.chromtrace.fusionzip`
-
-.. _yadg.parsers.chromtrace.provides:
-
-Schema
-``````
-The data is returned as a :class:`datatree.DataTree`, containing a :class:`xarray.Dataset`
-for each trace / detector name:
-
-.. code-block:: yaml
-
-  datatree.DataTree:
-    {{ detector_name }}  !!xr.Dataset
-      coords:
-        uts:             !!float               # Timestamp of the chromatogram
-        elution_time:    !!float               # The time axis of the chromatogram (s)
-      data_vars:
-        signal:          (uts, elution_time)   # The ordinate axis of the chromatogram
-
-When multiple chromatograms are parsed, they are concatenated separately per detector
-name. An error might occur during this concatenation if the ``elution_time`` axis changes
-dimensions or coordinates between different timesteps.
-
-.. note::
-
-  To parse processed data in the raw data files, such as integrated peak areas or
-  concentrations, use the :mod:`~yadg.parsers.chromdata` parser instead.
-
-Module Functions
-````````````````
-
-"""
-
-import logging
-import datatree
-
-from . import (
-    ezchromasc,
-    agilentcsv,
-    agilentch,
-    agilentdx,
-    fusionjson,
-    fusionzip,
-)
-
-logger = logging.getLogger(__name__)
-
-
-def process(
-    *,
-    filetype: str,
-    **kwargs: dict,
-) -> datatree.DataTree:
-    """
-    Unified raw chromatogram parser. Forwards ``kwargs`` to the worker functions
-    based on the supplied ``filetype``.
-
-    Parameters
-    ----------
-    filetype
-        Discriminator used to select the appropriate worker function.
-
-    Returns
-    -------
-    :class:`datatree.DataTree`
-
-    """
-    if filetype == "ezchrom.asc":
-        return ezchromasc.process(**kwargs)
-    elif filetype == "agilent.csv":
-        return agilentcsv.process(**kwargs)
-    elif filetype == "agilent.dx":
-        return agilentdx.process(**kwargs)
-    elif filetype == "agilent.ch":
-        return agilentch.process(**kwargs)
-    elif filetype == "fusion.json":
-        return fusionjson.process(**kwargs)
-    elif filetype == "fusion.zip":
-        return fusionzip.process(**kwargs)
+"""
+Handles the parsing of raw traces present in chromatography files, whether the source is
+a liquid chromatograph (LC) or a gas chromatograph (GC). The basic function of the
+parser is to:
+
+#. read in the raw data and create timestamped `traces`
+#. collect `metadata` such as the method information, sample ID, etc.
+
+:mod:`~yadg.parsers.chromtrace` loads the chromatographic data from the specified
+file, determines the uncertainties of the signal (y-axis), and explicitly
+populates the points in the time axis (x-axis), when required.
+
+Usage
+`````
+Available since ``yadg-4.0``. The parser supports the following parameters:
+
+.. _yadg.parsers.chromtrace.model:
+
+.. autopydantic_model:: dgbowl_schemas.yadg.dataschema_5_0.step.ChromTrace
+
+.. _yadg.parsers.chromtrace.formats:
+
+Formats
+```````
+The ``filetypes`` currently supported by the parser are:
+
+ - EZ-Chrom ASCII export (``ezchrom.asc``):
+   see :mod:`~yadg.parsers.chromtrace.ezchromasc`
+ - Agilent Chemstation Chromtab (``agilent.csv``):
+   see :mod:`~yadg.parsers.chromtrace.agilentcsv`
+ - Agilent OpenLab binary signal (``agilent.ch``):
+   see :mod:`~yadg.parsers.chromtrace.agilentch`
+ - Agilent OpenLab data archive (``agilent.dx``):
+   see :mod:`~yadg.parsers.chromtrace.agilentdx`
+ - Inficon Fusion JSON format (``fusion.json``):
+   see :mod:`~yadg.parsers.chromtrace.fusionjson`
+ - Inficon Fusion zip archive (``fusion.zip``):
+   see :mod:`~yadg.parsers.chromtrace.fusionzip`
+
+.. _yadg.parsers.chromtrace.provides:
+
+Schema
+``````
+The data is returned as a :class:`datatree.DataTree`, containing a :class:`xarray.Dataset`
+for each trace / detector name:
+
+.. code-block:: yaml
+
+  datatree.DataTree:
+    {{ detector_name }}  !!xr.Dataset
+      coords:
+        uts:             !!float               # Timestamp of the chromatogram
+        elution_time:    !!float               # The time axis of the chromatogram (s)
+      data_vars:
+        signal:          (uts, elution_time)   # The ordinate axis of the chromatogram
+
+When multiple chromatograms are parsed, they are concatenated separately per detector
+name. An error might occur during this concatenation if the ``elution_time`` axis changes
+dimensions or coordinates between different timesteps.
+
+.. note::
+
+  To parse processed data in the raw data files, such as integrated peak areas or
+  concentrations, use the :mod:`~yadg.parsers.chromdata` parser instead.
+
+Module Functions
+````````````````
+
+"""
+
+import logging
+import datatree
+
+from . import (
+    ezchromasc,
+    agilentcsv,
+    agilentch,
+    agilentdx,
+    fusionjson,
+    fusionzip,
+)
+
+logger = logging.getLogger(__name__)
+
+
+def process(
+    *,
+    filetype: str,
+    **kwargs: dict,
+) -> datatree.DataTree:
+    """
+    Unified raw chromatogram parser. Forwards ``kwargs`` to the worker functions
+    based on the supplied ``filetype``.
+
+    Parameters
+    ----------
+    filetype
+        Discriminator used to select the appropriate worker function.
+
+    Returns
+    -------
+    :class:`datatree.DataTree`
+
+    """
+    if filetype == "ezchrom.asc":
+        return ezchromasc.process(**kwargs)
+    elif filetype == "agilent.csv":
+        return agilentcsv.process(**kwargs)
+    elif filetype == "agilent.dx":
+        return agilentdx.process(**kwargs)
+    elif filetype == "agilent.ch":
+        return agilentch.process(**kwargs)
+    elif filetype == "fusion.json":
+        return fusionjson.process(**kwargs)
+    elif filetype == "fusion.zip":
+        return fusionzip.process(**kwargs)
```

### Comparing `yadg-5.0.1/src/yadg/parsers/chromtrace/agilentch.py` & `yadg-5.0.2/src/yadg/parsers/chromtrace/agilentch.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,161 +1,161 @@
-"""
-**agilentch**: Processing Agilent OpenLab binary signal trace files (CH and IT).
---------------------------------------------------------------------------------
-
-Currently supports version "179" of the files. Version information is defined in
-the `magic_values` (parameters & metadata) and `data_dtypes` (data) dictionaries.
-
-Adapted from `ImportAgilent.m <https://bit.ly/3HSelIR>`_ and
-`aston <https://github.com/bovee/Aston>`_.
-
-File Structure of ``.ch`` files
-```````````````````````````````
-.. code ::
-
-    0x0000 "version magic"
-    0x0108 "data offset"
-    0x011a "x-axis minimum (ms)"
-    0x011e "x-axis maximum (ms)"
-    0x035a "sample ID"
-    0x0559 "description"
-    0x0758 "username"
-    0x0957 "timestamp"
-    0x09e5 "instrument name"
-    0x09bc "inlet"
-    0x0a0e "method"
-    0x104c "y-axis unit"
-    0x1075 "detector name"
-    0x1274 "y-axis intercept"
-    0x127c "y-axis slope"
-
-Data is stored in a consecutive set of ``<f8``, starting at the offset (calculated
-as ``offset =  ("data offset" - 1) * 512``) until the end of the file.
-
-.. codeauthor:: Peter Kraus
-"""
-import numpy as np
-from zoneinfo import ZoneInfo
-from ... import dgutils
-from ...dgutils.dateutils import str_to_uts
-import xarray as xr
-from datatree import DataTree
-
-magic_values = {}
-magic_values["179"] = {
-    0x035A: ("sampleid", "utf-16"),
-    0x0559: ("description", "utf-16"),
-    0x0A0E: ("method", "utf-16"),
-    0x0758: ("username", "utf-16"),
-    0x0957: ("timestamp", "utf-16"),
-    0x09E5: ("instrument", "utf-16"),
-    0x09BC: ("inlet", "utf-16"),
-    0x104C: ("yunit", "utf-16"),
-    0x1075: ("tracetitle", "utf-16"),
-    0x0108: ("offset", ">i4"),  # (x-1) * 512
-    0x011A: ("xmin", ">f4"),  # / 60000
-    0x011E: ("xmax", ">f4"),  # / 60000
-    0x1274: ("intercept", ">f8"),
-    0x127C: ("slope", ">f8"),
-}
-
-data_dtypes = {}
-data_dtypes["179"] = (8, "<f8")
-
-
-def process(*, fn: str, timezone: ZoneInfo, **kwargs: dict) -> DataTree:
-    """
-    Agilent OpenLAB signal trace parser
-
-    One chromatogram per file with a single trace. Binary data format.
-
-    Parameters
-    ----------
-    fn
-        Filename to process.
-
-    encoding
-        Not used as the file is binary.
-
-    timezone
-        Timezone information. This should be ``"localtime"``.
-
-    Returns
-    -------
-    class:`datatree.DataTree`
-        A :class:`datatree.DataTree` containing one :class:`xarray.Dataset` per detector. As
-        there is only one detector data in each CH file, this nesting is only for
-        consistency with other filetypes.
-
-    """
-
-    with open(fn, "rb") as inf:
-        ch = inf.read()
-
-    magic = dgutils.read_value(ch, 0, "utf-8")
-    pars = {}
-    if magic in magic_values.keys():
-        for offset, (tag, dtype) in magic_values[magic].items():
-            v = dgutils.read_value(ch, offset, dtype)
-            pars[tag] = v
-    pars["end"] = len(ch)
-    dsize, ddtype = data_dtypes[magic]
-    pars["start"] = (pars["offset"] - 1) * 512
-    nbytes = pars["end"] - pars["start"]
-    assert nbytes % dsize == 0
-    npoints = nbytes // dsize
-
-    metadata = dict()
-    for k in ["sampleid", "username", "method"]:
-        metadata[k] = pars[k]
-    metadata["version"] = str(magic)
-
-    xsn = np.linspace(pars["xmin"] / 1000, pars["xmax"] / 1000, num=npoints)
-    xss = np.ones(npoints) * xsn[0]
-    ysn = (
-        np.frombuffer(
-            ch,
-            offset=pars["start"],
-            dtype=ddtype,
-            count=npoints,
-        )
-        * pars["slope"]
-    )
-    yss = np.ones(npoints) * pars["slope"]
-
-    detector, title = pars["tracetitle"].split(",")
-
-    uts = str_to_uts(
-        timestamp=pars["timestamp"], format="%d-%b-%y, %H:%M:%S", timezone=timezone
-    )
-
-    ds = xr.Dataset(
-        data_vars={
-            "signal": (
-                ["uts", "elution_time"],
-                [ysn],
-                {"units": pars["yunit"], "ancillary_variables": "signal_std_err"},
-            ),
-            "signal_std_err": (
-                ["uts", "elution_time"],
-                [yss],
-                {"units": pars["yunit"], "standard_name": "signal standard_error"},
-            ),
-            "elution_time_std_err": (
-                ["elution_time"],
-                xss,
-                {"units": "s", "standard_name": "elution_time standard_error"},
-            ),
-        },
-        coords={
-            "elution_time": (
-                ["elution_time"],
-                xsn,
-                {"units": "s", "ancillary_variables": "elution_time_std_err"},
-            ),
-            "uts": (["uts"], [uts]),
-        },
-        attrs={"title": title},
-    )
-    dt = DataTree.from_dict({detector: ds})
-    dt.attrs = metadata
-    return dt
+"""
+**agilentch**: Processing Agilent OpenLab binary signal trace files (CH and IT).
+--------------------------------------------------------------------------------
+
+Currently supports version "179" of the files. Version information is defined in
+the `magic_values` (parameters & metadata) and `data_dtypes` (data) dictionaries.
+
+Adapted from `ImportAgilent.m <https://bit.ly/3HSelIR>`_ and
+`aston <https://github.com/bovee/Aston>`_.
+
+File Structure of ``.ch`` files
+```````````````````````````````
+.. code ::
+
+    0x0000 "version magic"
+    0x0108 "data offset"
+    0x011a "x-axis minimum (ms)"
+    0x011e "x-axis maximum (ms)"
+    0x035a "sample ID"
+    0x0559 "description"
+    0x0758 "username"
+    0x0957 "timestamp"
+    0x09e5 "instrument name"
+    0x09bc "inlet"
+    0x0a0e "method"
+    0x104c "y-axis unit"
+    0x1075 "detector name"
+    0x1274 "y-axis intercept"
+    0x127c "y-axis slope"
+
+Data is stored in a consecutive set of ``<f8``, starting at the offset (calculated
+as ``offset =  ("data offset" - 1) * 512``) until the end of the file.
+
+.. codeauthor:: Peter Kraus
+"""
+import numpy as np
+from zoneinfo import ZoneInfo
+from ... import dgutils
+from ...dgutils.dateutils import str_to_uts
+import xarray as xr
+from datatree import DataTree
+
+magic_values = {}
+magic_values["179"] = {
+    0x035A: ("sampleid", "utf-16"),
+    0x0559: ("description", "utf-16"),
+    0x0A0E: ("method", "utf-16"),
+    0x0758: ("username", "utf-16"),
+    0x0957: ("timestamp", "utf-16"),
+    0x09E5: ("instrument", "utf-16"),
+    0x09BC: ("inlet", "utf-16"),
+    0x104C: ("yunit", "utf-16"),
+    0x1075: ("tracetitle", "utf-16"),
+    0x0108: ("offset", ">i4"),  # (x-1) * 512
+    0x011A: ("xmin", ">f4"),  # / 60000
+    0x011E: ("xmax", ">f4"),  # / 60000
+    0x1274: ("intercept", ">f8"),
+    0x127C: ("slope", ">f8"),
+}
+
+data_dtypes = {}
+data_dtypes["179"] = (8, "<f8")
+
+
+def process(*, fn: str, timezone: ZoneInfo, **kwargs: dict) -> DataTree:
+    """
+    Agilent OpenLAB signal trace parser
+
+    One chromatogram per file with a single trace. Binary data format.
+
+    Parameters
+    ----------
+    fn
+        Filename to process.
+
+    encoding
+        Not used as the file is binary.
+
+    timezone
+        Timezone information. This should be ``"localtime"``.
+
+    Returns
+    -------
+    class:`datatree.DataTree`
+        A :class:`datatree.DataTree` containing one :class:`xarray.Dataset` per detector. As
+        there is only one detector data in each CH file, this nesting is only for
+        consistency with other filetypes.
+
+    """
+
+    with open(fn, "rb") as inf:
+        ch = inf.read()
+
+    magic = dgutils.read_value(ch, 0, "utf-8")
+    pars = {}
+    if magic in magic_values.keys():
+        for offset, (tag, dtype) in magic_values[magic].items():
+            v = dgutils.read_value(ch, offset, dtype)
+            pars[tag] = v
+    pars["end"] = len(ch)
+    dsize, ddtype = data_dtypes[magic]
+    pars["start"] = (pars["offset"] - 1) * 512
+    nbytes = pars["end"] - pars["start"]
+    assert nbytes % dsize == 0
+    npoints = nbytes // dsize
+
+    metadata = dict()
+    for k in ["sampleid", "username", "method"]:
+        metadata[k] = pars[k]
+    metadata["version"] = str(magic)
+
+    xsn = np.linspace(pars["xmin"] / 1000, pars["xmax"] / 1000, num=npoints)
+    xss = np.ones(npoints) * xsn[0]
+    ysn = (
+        np.frombuffer(
+            ch,
+            offset=pars["start"],
+            dtype=ddtype,
+            count=npoints,
+        )
+        * pars["slope"]
+    )
+    yss = np.ones(npoints) * pars["slope"]
+
+    detector, title = pars["tracetitle"].split(",")
+
+    uts = str_to_uts(
+        timestamp=pars["timestamp"], format="%d-%b-%y, %H:%M:%S", timezone=timezone
+    )
+
+    ds = xr.Dataset(
+        data_vars={
+            "signal": (
+                ["uts", "elution_time"],
+                [ysn],
+                {"units": pars["yunit"], "ancillary_variables": "signal_std_err"},
+            ),
+            "signal_std_err": (
+                ["uts", "elution_time"],
+                [yss],
+                {"units": pars["yunit"], "standard_name": "signal standard_error"},
+            ),
+            "elution_time_std_err": (
+                ["elution_time"],
+                xss,
+                {"units": "s", "standard_name": "elution_time standard_error"},
+            ),
+        },
+        coords={
+            "elution_time": (
+                ["elution_time"],
+                xsn,
+                {"units": "s", "ancillary_variables": "elution_time_std_err"},
+            ),
+            "uts": (["uts"], [uts]),
+        },
+        attrs={"title": title},
+    )
+    dt = DataTree.from_dict({detector: ds})
+    dt.attrs = metadata
+    return dt
```

### Comparing `yadg-5.0.1/src/yadg/parsers/chromtrace/agilentdx.py` & `yadg-5.0.2/src/yadg/parsers/chromtrace/agilentdx.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,86 +1,86 @@
-"""
-**agilentch**: Processing Agilent OpenLab data archive files (DX).
-------------------------------------------------------------------
-
-This is a wrapper parser which unzips the provided DX file, and then uses the
-:mod:`yadg.parsers.chromtrace.agilentch` parser to parse every CH file present in
-the archive. The IT files in the archive are currently ignored.
-
-In addition to the metadata exposed by the CH parser, the ``datafile`` entry
-is populated with the corresponding name of the CH file. The ``fn`` entry in each
-timestep contains the parent DX file.
-
-.. note::
-
-   Currently the timesteps from multiple CH files (if present) are appended in the
-   timesteps array without any further sorting.
-
-.. codeauthor:: Peter Kraus
-"""
-import zipfile
-import tempfile
-import os
-from .agilentch import process as processch
-from datatree import DataTree
-import xarray as xr
-
-
-def process(*, fn: str, encoding: str, timezone: str, **kwargs: dict) -> DataTree:
-    """
-    Agilent OpenLab DX archive parser.
-
-    This is a simple wrapper around the Agilent OpenLab signal trace parser in
-    :mod:`yadg.parsers.chromtrace.agilentch`. This wrapper first un-zips the DX
-    file into a temporary directory, and then processess all CH files found
-    within the archive, concatenating timesteps from multiple files.
-
-    Parameters
-    ----------
-    fn
-        Filename to process.
-
-    encoding
-        Not used as the file is binary.
-
-    timezone
-        Timezone information. This should be ``"localtime"``.
-
-    Returns
-    -------
-    class:`datatree.DataTree`
-        A :class:`datatree.DataTree` containing one :class:`xarray.Dataset` per detector. If
-        multiple timesteps are found in the zip archive, the :class:`datatree.DataTrees`
-        are collated along the ``uts`` dimension.
-
-    """
-
-    zf = zipfile.ZipFile(fn)
-    with tempfile.TemporaryDirectory() as tempdir:
-        zf.extractall(tempdir)
-        dt = None
-        for ffn in os.listdir(tempdir):
-            if ffn.endswith("CH"):
-                path = os.path.join(tempdir, ffn)
-                fdt = processch(fn=path, encoding=encoding, timezone=timezone)
-                if dt is None:
-                    dt = fdt
-                elif isinstance(dt, DataTree):
-                    for k, v in fdt.items():
-                        if k in dt:  # pylint: disable=E1135
-                            try:
-                                newv = xr.concat(
-                                    [dt[k].ds, v.ds],  # pylint: disable=E1136
-                                    dim="uts",
-                                    combine_attrs="identical",
-                                )
-                            except xr.MergeError:
-                                raise RuntimeError(
-                                    "Merging metadata from the unzipped agilent-ch files has failed. "
-                                    "This is a bug. Please open an issue on GitHub."
-                                )
-                        else:
-                            newv = v.ds
-                        dt[k] = DataTree(newv)  # pylint: disable=E1137
-                else:
-                    raise RuntimeError("We should not get here.")
-    return dt
+"""
+**agilentch**: Processing Agilent OpenLab data archive files (DX).
+------------------------------------------------------------------
+
+This is a wrapper parser which unzips the provided DX file, and then uses the
+:mod:`yadg.parsers.chromtrace.agilentch` parser to parse every CH file present in
+the archive. The IT files in the archive are currently ignored.
+
+In addition to the metadata exposed by the CH parser, the ``datafile`` entry
+is populated with the corresponding name of the CH file. The ``fn`` entry in each
+timestep contains the parent DX file.
+
+.. note::
+
+   Currently the timesteps from multiple CH files (if present) are appended in the
+   timesteps array without any further sorting.
+
+.. codeauthor:: Peter Kraus
+"""
+import zipfile
+import tempfile
+import os
+from .agilentch import process as processch
+from datatree import DataTree
+import xarray as xr
+
+
+def process(*, fn: str, encoding: str, timezone: str, **kwargs: dict) -> DataTree:
+    """
+    Agilent OpenLab DX archive parser.
+
+    This is a simple wrapper around the Agilent OpenLab signal trace parser in
+    :mod:`yadg.parsers.chromtrace.agilentch`. This wrapper first un-zips the DX
+    file into a temporary directory, and then processess all CH files found
+    within the archive, concatenating timesteps from multiple files.
+
+    Parameters
+    ----------
+    fn
+        Filename to process.
+
+    encoding
+        Not used as the file is binary.
+
+    timezone
+        Timezone information. This should be ``"localtime"``.
+
+    Returns
+    -------
+    class:`datatree.DataTree`
+        A :class:`datatree.DataTree` containing one :class:`xarray.Dataset` per detector. If
+        multiple timesteps are found in the zip archive, the :class:`datatree.DataTrees`
+        are collated along the ``uts`` dimension.
+
+    """
+
+    zf = zipfile.ZipFile(fn)
+    with tempfile.TemporaryDirectory() as tempdir:
+        zf.extractall(tempdir)
+        dt = None
+        for ffn in os.listdir(tempdir):
+            if ffn.endswith("CH"):
+                path = os.path.join(tempdir, ffn)
+                fdt = processch(fn=path, encoding=encoding, timezone=timezone)
+                if dt is None:
+                    dt = fdt
+                elif isinstance(dt, DataTree):
+                    for k, v in fdt.items():
+                        if k in dt:  # pylint: disable=E1135
+                            try:
+                                newv = xr.concat(
+                                    [dt[k].ds, v.ds],  # pylint: disable=E1136
+                                    dim="uts",
+                                    combine_attrs="identical",
+                                )
+                            except xr.MergeError:
+                                raise RuntimeError(
+                                    "Merging metadata from the unzipped agilent-ch files has failed. "
+                                    "This is a bug. Please open an issue on GitHub."
+                                )
+                        else:
+                            newv = v.ds
+                        dt[k] = DataTree(newv)  # pylint: disable=E1137
+                else:
+                    raise RuntimeError("We should not get here.")
+    return dt
```

### Comparing `yadg-5.0.1/src/yadg/parsers/chromtrace/ezchromasc.py` & `yadg-5.0.2/src/yadg/parsers/chromtrace/ezchromasc.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,169 +1,169 @@
-"""
-**ezchromasc**: Processing EZ-Chrom ASCII export files (dat.asc).
------------------------------------------------------------------
-
-This file format includes one timestep with multiple traces in each ASCII file. It
-contains a header section, and a sequence of Y datapoints (``signal``) for each detector.
-The X-axis (``elution_time``) is assumed to be uniform between traces, and its units have
-to be deduced from the header.
-
-.. codeauthor:: Peter Kraus
-"""
-import numpy as np
-import logging
-from zoneinfo import ZoneInfo
-from uncertainties.core import str_to_number_with_uncert as tuple_fromstr
-from ...dgutils.dateutils import str_to_uts
-import xarray as xr
-from datatree import DataTree
-
-logger = logging.getLogger(__name__)
-
-
-def process(*, fn: str, encoding: str, timezone: ZoneInfo, **kwargs: dict) -> DataTree:
-    """
-    EZ-Chrome ASCII export file parser.
-
-    One chromatogram per file with multiple traces. A header section is followed by
-    y-values for each trace. x-values have to be deduced using number of points,
-    frequency, and x-multiplier. Method name is available, but detector names are not.
-    They are assigned their numerical index in the file.
-
-    Parameters
-    ----------
-    fn
-        Filename to process.
-
-    encoding
-        Encoding used to open the file.
-
-    timezone
-        Timezone information. This should be ``"localtime"``.
-
-
-    Returns
-    -------
-    class:`datatree.DataTree`
-        A :class:`datatree.DataTree` containing one :class:`xarray.Dataset` per detector.
-
-    """
-
-    with open(fn, "r", encoding=encoding, errors="ignore") as infile:
-        lines = infile.readlines()
-    metadata = {}
-    data = {}
-
-    for line in lines:
-        for key in ["Version", "Method", "User Name"]:
-            if line.startswith(key):
-                k = key.lower().replace(" ", "")
-                metadata[k] = line.split(f"{key}:")[1].strip()
-        for key in ["Sample ID"]:  # , "Data File"]:
-            if line.startswith(key):
-                k = key.lower().replace(" ", "")
-                metadata[k] = line.split(f"{key}:")[1].strip()
-        if line.startswith("Acquisition Date and Time:"):
-            uts = str_to_uts(
-                timestamp=line.split("Time:")[1].strip(),
-                format="%m/%d/%Y %I:%M:%S %p",
-                timezone=timezone,
-            )
-        if line.startswith("Sampling Rate:"):
-            assert (
-                "Hz" in line
-            ), f"datasc: Incorrect units for rate in file {fn}: {line}"
-            parts = line.split("\t")
-            samplerates = [float(each.strip()) for each in parts[1:-1]]
-        if line.startswith("Total Data Points:"):
-            assert (
-                "Pts." in line
-            ), f"datasc: Incorrect units for number of points in file {fn}: {line}"
-            parts = line.split("\t")
-            npoints = [int(each.strip()) for each in parts[1:-1]]
-        if line.startswith("X Axis Title:"):
-            parts = line.split("\t")
-            xunits = [each.strip() for each in parts[1:]]
-        if line.startswith("Y Axis Title:"):
-            parts = line.split("\t")
-            yunits = [each.strip() for each in parts[1:]]
-            if "25 V" in yunits:
-                logger.warning("Implicit conversion of y-axis unit from '25 V' to 'V'.")
-                yunits = [i.replace("25 V", "V") for i in yunits]
-        if line.startswith("X Axis Multiplier:"):
-            parts = line.split("\t")
-            xmuls = [float(each.strip()) for each in parts[1:]]
-        if line.startswith("Y Axis Multiplier:"):
-            parts = line.split("\t")
-            ymuls = [float(each.strip()) for each in parts[1:]]
-        if ":" not in line:
-            si = lines.index(line)
-            break
-    assert (
-        len(samplerates)
-        == len(npoints)
-        == len(xunits)
-        == len(yunits)
-        == len(xmuls)
-        == len(ymuls)
-    ), f"datasc: Inconsistent number of traces in {fn}."
-
-    data = {}
-    units = {}
-    for ti, npts in enumerate(npoints):
-        assert (
-            xunits[ti] == "Minutes"
-        ), f"datasc: X units label of trace {ti} in {fn} was not understood."
-        dt = 60
-        xmul = xmuls[ti] * dt / samplerates[ti]
-        ymul = ymuls[ti]
-        xsn = np.arange(npts) * xmul
-        xss = np.ones(npts) * xmul
-        ysn, yss = zip(*[tuple_fromstr(li) for li in lines[si : si + npts]])
-        si += npts
-        data[f"{ti}"] = {
-            "t": (xsn, xss),
-            "y": (np.array(ysn) * ymul, np.array(yss) * ymul),
-        }
-        units[f"{ti}"] = {"t": "s", "y": yunits[ti]}
-
-    traces = sorted(data.keys())
-    vals = {}
-    for ti in traces:
-        fvals = xr.Dataset(
-            data_vars={
-                "signal": (
-                    ["uts", "elution_time"],
-                    [data[ti]["y"][0]],
-                    {"units": units[ti]["y"], "ancillary_variables": "signal_std_err"},
-                ),
-                "signal_std_err": (
-                    ["uts", "elution_time"],
-                    [data[ti]["y"][1]],
-                    {"units": units[ti]["y"], "standard_name": "signal standard_error"},
-                ),
-                "elution_time_std_err": (
-                    ["elution_time"],
-                    data[ti]["t"][1],
-                    {
-                        "units": units[ti]["t"],
-                        "standard_name": "elution_time standard_error",
-                    },
-                ),
-            },
-            coords={
-                "elution_time": (
-                    ["elution_time"],
-                    data[ti]["t"][0],
-                    {
-                        "units": units[ti]["t"],
-                        "ancillary_variables": "elution_time_std_err",
-                    },
-                ),
-                "uts": (["uts"], [uts]),
-            },
-            attrs={},
-        )
-        vals[ti] = fvals
-    dt = DataTree.from_dict(vals)
-    dt.attrs = metadata
-    return dt
+"""
+**ezchromasc**: Processing EZ-Chrom ASCII export files (dat.asc).
+-----------------------------------------------------------------
+
+This file format includes one timestep with multiple traces in each ASCII file. It
+contains a header section, and a sequence of Y datapoints (``signal``) for each detector.
+The X-axis (``elution_time``) is assumed to be uniform between traces, and its units have
+to be deduced from the header.
+
+.. codeauthor:: Peter Kraus
+"""
+import numpy as np
+import logging
+from zoneinfo import ZoneInfo
+from uncertainties.core import str_to_number_with_uncert as tuple_fromstr
+from ...dgutils.dateutils import str_to_uts
+import xarray as xr
+from datatree import DataTree
+
+logger = logging.getLogger(__name__)
+
+
+def process(*, fn: str, encoding: str, timezone: ZoneInfo, **kwargs: dict) -> DataTree:
+    """
+    EZ-Chrome ASCII export file parser.
+
+    One chromatogram per file with multiple traces. A header section is followed by
+    y-values for each trace. x-values have to be deduced using number of points,
+    frequency, and x-multiplier. Method name is available, but detector names are not.
+    They are assigned their numerical index in the file.
+
+    Parameters
+    ----------
+    fn
+        Filename to process.
+
+    encoding
+        Encoding used to open the file.
+
+    timezone
+        Timezone information. This should be ``"localtime"``.
+
+
+    Returns
+    -------
+    class:`datatree.DataTree`
+        A :class:`datatree.DataTree` containing one :class:`xarray.Dataset` per detector.
+
+    """
+
+    with open(fn, "r", encoding=encoding, errors="ignore") as infile:
+        lines = infile.readlines()
+    metadata = {}
+    data = {}
+
+    for line in lines:
+        for key in ["Version", "Method", "User Name"]:
+            if line.startswith(key):
+                k = key.lower().replace(" ", "")
+                metadata[k] = line.split(f"{key}:")[1].strip()
+        for key in ["Sample ID"]:  # , "Data File"]:
+            if line.startswith(key):
+                k = key.lower().replace(" ", "")
+                metadata[k] = line.split(f"{key}:")[1].strip()
+        if line.startswith("Acquisition Date and Time:"):
+            uts = str_to_uts(
+                timestamp=line.split("Time:")[1].strip(),
+                format="%m/%d/%Y %I:%M:%S %p",
+                timezone=timezone,
+            )
+        if line.startswith("Sampling Rate:"):
+            assert (
+                "Hz" in line
+            ), f"datasc: Incorrect units for rate in file {fn}: {line}"
+            parts = line.split("\t")
+            samplerates = [float(each.strip()) for each in parts[1:-1]]
+        if line.startswith("Total Data Points:"):
+            assert (
+                "Pts." in line
+            ), f"datasc: Incorrect units for number of points in file {fn}: {line}"
+            parts = line.split("\t")
+            npoints = [int(each.strip()) for each in parts[1:-1]]
+        if line.startswith("X Axis Title:"):
+            parts = line.split("\t")
+            xunits = [each.strip() for each in parts[1:]]
+        if line.startswith("Y Axis Title:"):
+            parts = line.split("\t")
+            yunits = [each.strip() for each in parts[1:]]
+            if "25 V" in yunits:
+                logger.warning("Implicit conversion of y-axis unit from '25 V' to 'V'.")
+                yunits = [i.replace("25 V", "V") for i in yunits]
+        if line.startswith("X Axis Multiplier:"):
+            parts = line.split("\t")
+            xmuls = [float(each.strip()) for each in parts[1:]]
+        if line.startswith("Y Axis Multiplier:"):
+            parts = line.split("\t")
+            ymuls = [float(each.strip()) for each in parts[1:]]
+        if ":" not in line:
+            si = lines.index(line)
+            break
+    assert (
+        len(samplerates)
+        == len(npoints)
+        == len(xunits)
+        == len(yunits)
+        == len(xmuls)
+        == len(ymuls)
+    ), f"datasc: Inconsistent number of traces in {fn}."
+
+    data = {}
+    units = {}
+    for ti, npts in enumerate(npoints):
+        assert (
+            xunits[ti] == "Minutes"
+        ), f"datasc: X units label of trace {ti} in {fn} was not understood."
+        dt = 60
+        xmul = xmuls[ti] * dt / samplerates[ti]
+        ymul = ymuls[ti]
+        xsn = np.arange(npts) * xmul
+        xss = np.ones(npts) * xmul
+        ysn, yss = zip(*[tuple_fromstr(li) for li in lines[si : si + npts]])
+        si += npts
+        data[f"{ti}"] = {
+            "t": (xsn, xss),
+            "y": (np.array(ysn) * ymul, np.array(yss) * ymul),
+        }
+        units[f"{ti}"] = {"t": "s", "y": yunits[ti]}
+
+    traces = sorted(data.keys())
+    vals = {}
+    for ti in traces:
+        fvals = xr.Dataset(
+            data_vars={
+                "signal": (
+                    ["uts", "elution_time"],
+                    [data[ti]["y"][0]],
+                    {"units": units[ti]["y"], "ancillary_variables": "signal_std_err"},
+                ),
+                "signal_std_err": (
+                    ["uts", "elution_time"],
+                    [data[ti]["y"][1]],
+                    {"units": units[ti]["y"], "standard_name": "signal standard_error"},
+                ),
+                "elution_time_std_err": (
+                    ["elution_time"],
+                    data[ti]["t"][1],
+                    {
+                        "units": units[ti]["t"],
+                        "standard_name": "elution_time standard_error",
+                    },
+                ),
+            },
+            coords={
+                "elution_time": (
+                    ["elution_time"],
+                    data[ti]["t"][0],
+                    {
+                        "units": units[ti]["t"],
+                        "ancillary_variables": "elution_time_std_err",
+                    },
+                ),
+                "uts": (["uts"], [uts]),
+            },
+            attrs={},
+        )
+        vals[ti] = fvals
+    dt = DataTree.from_dict(vals)
+    dt.attrs = metadata
+    return dt
```

### Comparing `yadg-5.0.1/src/yadg/parsers/chromtrace/fusionjson.py` & `yadg-5.0.2/src/yadg/parsers/chromtrace/fusionjson.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,111 +1,111 @@
-"""
-**fusionjson**: Processing Inficon Fusion json data format (json).
-------------------------------------------------------------------
-
-This is a fairly detailed data format, including the traces, the calibration applied,
-and also the integrated peak areas. If the peak areas are present, this is returned
-in the list of timesteps as a ``"peaks"`` entry.
-
-Exposed metadata:
-`````````````````
-
-.. code-block:: yaml
-
-    method:   !!str
-    sampleid: !!str
-    version:  !!str
-    datafile: !!str
-
-.. codeauthor:: Peter Kraus
-"""
-import json
-from zoneinfo import ZoneInfo
-import numpy as np
-from ...dgutils.dateutils import str_to_uts
-import xarray as xr
-from datatree import DataTree
-
-
-def process(*, fn: str, encoding: str, timezone: ZoneInfo, **kwargs: dict) -> DataTree:
-    """
-    Fusion json format.
-
-    One chromatogram per file with multiple traces, and integrated peak areas.
-
-    .. warning::
-
-        To parse the integrated data present in these files, use the
-        :mod:`~yadg.parsers.chromdata` parser.
-
-    Only a subset of the metadata is retained, including the method name,
-    detector names, and information about assigned peaks.
-
-    Parameters
-    ----------
-    fn
-        Filename to process.
-
-    encoding
-        Encoding used to open the file.
-
-    timezone
-        Timezone information. This should be ``"localtime"``.
-
-    Returns
-    -------
-    class:`datatree.DataTree`
-        A :class:`datatree.DataTree` containing one :class:`xarray.Dataset` per detector.
-
-    """
-
-    with open(fn, "r", encoding=encoding, errors="ignore") as infile:
-        jsdata = json.load(infile)
-    metadata = {
-        "method": jsdata.get("methodName", "n/a"),
-        "sampleid": jsdata.get("annotations", {}).get("name", None),
-        "version": jsdata.get("softwareVersion", {}).get("version", None),
-        "datafile": jsdata.get("sequence", {}).get("location", None),
-    }
-    uts = str_to_uts(timestamp=jsdata["runTimeStamp"], timezone=timezone)
-
-    # sort detector keys to ensure alphabetic order for ID matching
-    traces = sorted(jsdata["detectors"].keys())
-    vals = {}
-    for detname in traces:
-        detdict = jsdata["detectors"][detname]
-        fvals = xr.Dataset(
-            data_vars={
-                "signal": (
-                    ["uts", "elution_time"],
-                    [detdict["values"]],
-                    {"ancillary_variables": "signal_std_err"},
-                ),
-                "signal_std_err": (
-                    ["uts", "elution_time"],
-                    [np.ones(detdict["nValuesExpected"])],
-                    {"standard_name": "signal standard_error"},
-                ),
-                "elution_time_std_err": (
-                    ["elution_time"],
-                    np.ones(detdict["nValuesExpected"]) / detdict["nValuesPerSecond"],
-                    {"units": "s", "standard_name": "elution_time standard_error"},
-                ),
-            },
-            coords={
-                "elution_time": (
-                    ["elution_time"],
-                    np.arange(detdict["nValuesExpected"]) / detdict["nValuesPerSecond"],
-                    {"units": "s", "ancillary_variables": "elution_time_std_err"},
-                ),
-                "uts": (["uts"], [uts]),
-            },
-            attrs={},
-        )
-        valve = jsdata.get("annotations", {}).get("valcoPosition", None)
-        if valve is not None:
-            fvals["valve"] = valve
-        vals[detname] = fvals
-
-    dt = DataTree.from_dict(vals)
-    dt.attrs = metadata
-    return dt
+"""
+**fusionjson**: Processing Inficon Fusion json data format (json).
+------------------------------------------------------------------
+
+This is a fairly detailed data format, including the traces, the calibration applied,
+and also the integrated peak areas. If the peak areas are present, this is returned
+in the list of timesteps as a ``"peaks"`` entry.
+
+Exposed metadata:
+`````````````````
+
+.. code-block:: yaml
+
+    method:   !!str
+    sampleid: !!str
+    version:  !!str
+    datafile: !!str
+
+.. codeauthor:: Peter Kraus
+"""
+import json
+from zoneinfo import ZoneInfo
+import numpy as np
+from ...dgutils.dateutils import str_to_uts
+import xarray as xr
+from datatree import DataTree
+
+
+def process(*, fn: str, encoding: str, timezone: ZoneInfo, **kwargs: dict) -> DataTree:
+    """
+    Fusion json format.
+
+    One chromatogram per file with multiple traces, and integrated peak areas.
+
+    .. warning::
+
+        To parse the integrated data present in these files, use the
+        :mod:`~yadg.parsers.chromdata` parser.
+
+    Only a subset of the metadata is retained, including the method name,
+    detector names, and information about assigned peaks.
+
+    Parameters
+    ----------
+    fn
+        Filename to process.
+
+    encoding
+        Encoding used to open the file.
+
+    timezone
+        Timezone information. This should be ``"localtime"``.
+
+    Returns
+    -------
+    class:`datatree.DataTree`
+        A :class:`datatree.DataTree` containing one :class:`xarray.Dataset` per detector.
+
+    """
+
+    with open(fn, "r", encoding=encoding, errors="ignore") as infile:
+        jsdata = json.load(infile)
+    metadata = {
+        "method": jsdata.get("methodName", "n/a"),
+        "sampleid": jsdata.get("annotations", {}).get("name", None),
+        "version": jsdata.get("softwareVersion", {}).get("version", None),
+        "datafile": jsdata.get("sequence", {}).get("location", None),
+    }
+    uts = str_to_uts(timestamp=jsdata["runTimeStamp"], timezone=timezone)
+
+    # sort detector keys to ensure alphabetic order for ID matching
+    traces = sorted(jsdata["detectors"].keys())
+    vals = {}
+    for detname in traces:
+        detdict = jsdata["detectors"][detname]
+        fvals = xr.Dataset(
+            data_vars={
+                "signal": (
+                    ["uts", "elution_time"],
+                    [detdict["values"]],
+                    {"ancillary_variables": "signal_std_err"},
+                ),
+                "signal_std_err": (
+                    ["uts", "elution_time"],
+                    [np.ones(detdict["nValuesExpected"])],
+                    {"standard_name": "signal standard_error"},
+                ),
+                "elution_time_std_err": (
+                    ["elution_time"],
+                    np.ones(detdict["nValuesExpected"]) / detdict["nValuesPerSecond"],
+                    {"units": "s", "standard_name": "elution_time standard_error"},
+                ),
+            },
+            coords={
+                "elution_time": (
+                    ["elution_time"],
+                    np.arange(detdict["nValuesExpected"]) / detdict["nValuesPerSecond"],
+                    {"units": "s", "ancillary_variables": "elution_time_std_err"},
+                ),
+                "uts": (["uts"], [uts]),
+            },
+            attrs={},
+        )
+        valve = jsdata.get("annotations", {}).get("valcoPosition", None)
+        if valve is not None:
+            fvals["valve"] = valve
+        vals[detname] = fvals
+
+    dt = DataTree.from_dict(vals)
+    dt.attrs = metadata
+    return dt
```

### Comparing `yadg-5.0.1/src/yadg/parsers/chromtrace/fusionzip.py` & `yadg-5.0.2/src/yadg/parsers/chromtrace/fusionzip.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,81 +1,81 @@
-"""
-**fusionzip**: Processing Inficon Fusion zipped data format (zip).
-------------------------------------------------------------------
-
-This is a wrapper parser which unzips the provided zip file, and then uses
-the :mod:`yadg.parsers.chromtrace.fusionjson` parser to parse every data
-file present in the archive.
-
-Exposed metadata:
-`````````````````
-
-.. code-block:: yaml
-
-    method:   !!str
-    sampleid: !!str
-    version:  !!str
-    datafile: !!str
-
-.. codeauthor:: Peter Kraus
-"""
-import zipfile
-import tempfile
-import os
-import xarray as xr
-from datatree import DataTree
-
-from .fusionjson import process as processjson
-
-
-def process(*, fn: str, encoding: str, timezone: str, **kwargs: dict) -> DataTree:
-    """
-    Fusion zip file format.
-
-    The Fusion GC's can export their json formats as a zip archive of a folder
-    of jsons. This parser allows for parsing of this zip archive directly,
-    without the user having to unzip & move the data.
-
-    Parameters
-    ----------
-    fn
-        Filename to process.
-
-    encoding
-        Not used as the file is binary.
-
-    timezone
-        Timezone information. This should be ``"localtime"``.
-
-    Returns
-    -------
-    class:`datatree.DataTree`
-        A :class:`datatree.DataTree` containing one :class:`xarray.Dataset` per detector. If
-        multiple timesteps are found in the zip archive, the :class:`datatree.DataTrees`
-        are collated along the ``uts`` dimension.
-
-    """
-
-    zf = zipfile.ZipFile(fn)
-    with tempfile.TemporaryDirectory() as tempdir:
-        zf.extractall(tempdir)
-        dt = None
-        for ffn in sorted(os.listdir(tempdir)):
-            path = os.path.join(tempdir, ffn)
-            if ffn.endswith("fusion-data"):
-                fdt = processjson(fn=path, encoding=encoding, timezone=timezone)
-                if dt is None:
-                    dt = fdt
-                elif isinstance(dt, DataTree):
-                    for k, v in fdt.items():
-                        if k in dt:  # pylint: disable=E1135
-                            newv = xr.concat(
-                                [dt[k].ds, v.ds],  # pylint: disable=E1136
-                                dim="uts",
-                                combine_attrs="identical",
-                            )
-                        else:
-                            newv = v.ds
-                        dt[k] = DataTree(newv)  # pylint: disable=E1137
-                else:
-                    raise RuntimeError("We should not get here.")
-    return dt
+"""
+**fusionzip**: Processing Inficon Fusion zipped data format (zip).
+------------------------------------------------------------------
+
+This is a wrapper parser which unzips the provided zip file, and then uses
+the :mod:`yadg.parsers.chromtrace.fusionjson` parser to parse every data
+file present in the archive.
+
+Exposed metadata:
+`````````````````
+
+.. code-block:: yaml
+
+    method:   !!str
+    sampleid: !!str
+    version:  !!str
+    datafile: !!str
+
+.. codeauthor:: Peter Kraus
+"""
+import zipfile
+import tempfile
+import os
+import xarray as xr
+from datatree import DataTree
+
+from .fusionjson import process as processjson
+
+
+def process(*, fn: str, encoding: str, timezone: str, **kwargs: dict) -> DataTree:
+    """
+    Fusion zip file format.
+
+    The Fusion GC's can export their json formats as a zip archive of a folder
+    of jsons. This parser allows for parsing of this zip archive directly,
+    without the user having to unzip & move the data.
+
+    Parameters
+    ----------
+    fn
+        Filename to process.
+
+    encoding
+        Not used as the file is binary.
+
+    timezone
+        Timezone information. This should be ``"localtime"``.
+
+    Returns
+    -------
+    class:`datatree.DataTree`
+        A :class:`datatree.DataTree` containing one :class:`xarray.Dataset` per detector. If
+        multiple timesteps are found in the zip archive, the :class:`datatree.DataTrees`
+        are collated along the ``uts`` dimension.
+
+    """
+
+    zf = zipfile.ZipFile(fn)
+    with tempfile.TemporaryDirectory() as tempdir:
+        zf.extractall(tempdir)
+        dt = None
+        for ffn in sorted(os.listdir(tempdir)):
+            path = os.path.join(tempdir, ffn)
+            if ffn.endswith("fusion-data"):
+                fdt = processjson(fn=path, encoding=encoding, timezone=timezone)
+                if dt is None:
+                    dt = fdt
+                elif isinstance(dt, DataTree):
+                    for k, v in fdt.items():
+                        if k in dt:  # pylint: disable=E1135
+                            newv = xr.concat(
+                                [dt[k].ds, v.ds],  # pylint: disable=E1136
+                                dim="uts",
+                                combine_attrs="identical",
+                            )
+                        else:
+                            newv = v.ds
+                        dt[k] = DataTree(newv)  # pylint: disable=E1137
+                else:
+                    raise RuntimeError("We should not get here.")
+    return dt
```

### Comparing `yadg-5.0.1/src/yadg/parsers/electrochem/__init__.py` & `yadg-5.0.2/src/yadg/parsers/electrochem/__init__.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,87 +1,87 @@
-"""
-This module handles the reading and processing of files containing electrochemical
-data, including BioLogic's EC-Lab file formats. The basic function of the parser is to:
-
-#. Read in the technique data and create timesteps.
-#. Collect metadata, such as the measurement settings and the loops
-   contained in a given file.
-#. Collect data describing the technique parameter sequences.
-
-Usage
-`````
-Available since ``yadg-4.0``. The parser supports the following parameters:
-
-.. _yadg.parsers.electrochem.model:
-
-.. autopydantic_model:: dgbowl_schemas.yadg.dataschema_5_0.step.ElectroChem
-
-.. _yadg.parsers.electrochem.formats:
-
-Formats
-```````
-The ``filetypes`` currently supported by the parser are:
-
- - EC-Lab raw data binary file and parameter settings (``eclab.mpr``),
-   see :mod:`~yadg.parsers.electrochem.eclabmpr`
- - EC-Lab human-readable text export of data (``eclab.mpt``),
-   see :mod:`~yadg.parsers.electrochem.eclabmpt`
- - tomato's structured json output (``tomato.json``),
-   see :mod:`~yadg.parsers.electrochem.tomatojson`
-
-Schema
-``````
-Depending on the filetype, the output :class:`xarray.Dataset` may contain multiple
-derived values. However, all filetypes will report at least the following:
-
-.. code-block:: yaml
-
-  xr.Dataset:
-    coords:
-      uts:      !!float
-    data_vars:
-      Ewe:      (uts)    # Potential of the working electrode (V)
-      Ece:      (uts)    # Potential of the counter electrode (V)
-      I:        (uts)    # Applied current (A)
-
-In some cases, average values (i.e. ``<Ewe>`` or ``<I>``) may be reported instead
-of the instantaneous data.
-
-.. warning::
-
-  In previous versions of :mod:`yadg`, the :mod:`~yadg.parsers.electrochem` parser
-  optionally transposed data from impedance spectroscopy, grouping the datapoints
-  in each scan into a single "trace". This behaviour has been removed in ``yadg-5.0``.
-
-Module Functions
-````````````````
-
-"""
-import xarray as xr
-from . import eclabmpr, eclabmpt, tomatojson
-
-
-def process(
-    *,
-    filetype: str,
-    **kwargs: dict,
-) -> xr.Dataset:
-    """
-    Unified parser for electrochemistry data. Forwards ``kwargs`` to the worker functions
-    based on the supplied ``filetype``.
-
-    Parameters
-    ----------
-    filetype
-        Discriminator used to select the appropriate worker function.
-
-    Returns
-    -------
-    :class:`xarray.Dataset`
-
-    """
-    if filetype == "eclab.mpr":
-        return eclabmpr.process(**kwargs)
-    elif filetype == "eclab.mpt":
-        return eclabmpt.process(**kwargs)
-    elif filetype == "tomato.json":
-        return tomatojson.process(**kwargs)
+"""
+This module handles the reading and processing of files containing electrochemical
+data, including BioLogic's EC-Lab file formats. The basic function of the parser is to:
+
+#. Read in the technique data and create timesteps.
+#. Collect metadata, such as the measurement settings and the loops
+   contained in a given file.
+#. Collect data describing the technique parameter sequences.
+
+Usage
+`````
+Available since ``yadg-4.0``. The parser supports the following parameters:
+
+.. _yadg.parsers.electrochem.model:
+
+.. autopydantic_model:: dgbowl_schemas.yadg.dataschema_5_0.step.ElectroChem
+
+.. _yadg.parsers.electrochem.formats:
+
+Formats
+```````
+The ``filetypes`` currently supported by the parser are:
+
+ - EC-Lab raw data binary file and parameter settings (``eclab.mpr``),
+   see :mod:`~yadg.parsers.electrochem.eclabmpr`
+ - EC-Lab human-readable text export of data (``eclab.mpt``),
+   see :mod:`~yadg.parsers.electrochem.eclabmpt`
+ - tomato's structured json output (``tomato.json``),
+   see :mod:`~yadg.parsers.electrochem.tomatojson`
+
+Schema
+``````
+Depending on the filetype, the output :class:`xarray.Dataset` may contain multiple
+derived values. However, all filetypes will report at least the following:
+
+.. code-block:: yaml
+
+  xr.Dataset:
+    coords:
+      uts:      !!float
+    data_vars:
+      Ewe:      (uts)    # Potential of the working electrode (V)
+      Ece:      (uts)    # Potential of the counter electrode (V)
+      I:        (uts)    # Applied current (A)
+
+In some cases, average values (i.e. ``<Ewe>`` or ``<I>``) may be reported instead
+of the instantaneous data.
+
+.. warning::
+
+  In previous versions of :mod:`yadg`, the :mod:`~yadg.parsers.electrochem` parser
+  optionally transposed data from impedance spectroscopy, grouping the datapoints
+  in each scan into a single "trace". This behaviour has been removed in ``yadg-5.0``.
+
+Module Functions
+````````````````
+
+"""
+import xarray as xr
+from . import eclabmpr, eclabmpt, tomatojson
+
+
+def process(
+    *,
+    filetype: str,
+    **kwargs: dict,
+) -> xr.Dataset:
+    """
+    Unified parser for electrochemistry data. Forwards ``kwargs`` to the worker functions
+    based on the supplied ``filetype``.
+
+    Parameters
+    ----------
+    filetype
+        Discriminator used to select the appropriate worker function.
+
+    Returns
+    -------
+    :class:`xarray.Dataset`
+
+    """
+    if filetype == "eclab.mpr":
+        return eclabmpr.process(**kwargs)
+    elif filetype == "eclab.mpt":
+        return eclabmpt.process(**kwargs)
+    elif filetype == "tomato.json":
+        return tomatojson.process(**kwargs)
```

### Comparing `yadg-5.0.1/src/yadg/parsers/electrochem/eclabcommon/mpr_columns.py` & `yadg-5.0.2/src/yadg/parsers/electrochem/eclabcommon/mpr_columns.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,193 +1,193 @@
-import numpy as np
-
-# Module header starting after each MODULE keyword.
-module_header_dtype = np.dtype(
-    [
-        ("short_name", "|S10"),
-        ("long_name", "|S25"),
-        ("length", "<u4"),
-        ("version", "<u4"),
-        ("date", "|S8"),
-    ]
-)
-
-
-# Relates the offset in the settings data to the corresponding dtype and
-# name. Maybe watch out for very long pascal strings as they may span
-# over the entire zero padding and shift the offsets.
-settings_dtypes = {
-    0x0007: ("pascal", "comments"),
-    0x0107: ("<f4", "active_material_mass"),
-    0x010B: ("<f4", "at_x"),
-    0x010F: ("<f4", "molecular_weight"),
-    0x0113: ("<f4", "atomic_weight"),
-    0x0117: ("<f4", "acquisition_start"),
-    0x011B: ("<u2", "e_transferred"),
-    0x011E: ("pascal", "electrode_material"),
-    0x01C0: ("pascal", "electrolyte"),
-    0x0211: ("<f4", "electrode_area"),
-    0x0215: ("pascal", "reference_electrode"),
-    0x024C: ("<f4", "characteristic_mass"),
-    0x025C: ("<f4", "battery_capacity"),
-    0x0260: ("|u1", "battery_capacity_unit"),
-    # NOTE: The compliance limits are apparently not always at this
-    # offset, hence commented out...
-    # 0x19d2: ("<f4", "compliance_min"),
-    # 0x19d6: ("<f4", "compliance_max"),
-}
-
-
-# Maps the flag column ID bytes to the corresponding bitmask and name.
-flag_columns = {
-    0x0001: (0b00000011, "mode"),
-    0x0002: (0b00000100, "ox or red"),
-    0x0003: (0b00001000, "error"),
-    0x0015: (0b00010000, "control changes"),
-    0x001F: (0b00100000, "Ns changes"),
-    # NOTE: I think the missing bitmask (0b01000000) is a stop bit. It
-    # sometimes appears in the flag byte of the very last data point.
-    0x0041: (0b10000000, "counter inc."),
-}
-
-
-# Maps the data column ID bytes to the corresponding dtype, name and
-# unit.
-data_columns = {
-    0x0004: ("<f8", "time", "s"),
-    0x0005: ("<f4", "control_V_I", "V/mA"),
-    0x0006: ("<f4", "Ewe", "V"),
-    0x0007: ("<f8", "dq", "mA·h"),
-    0x0008: ("<f4", "I", "mA"),
-    0x0009: ("<f4", "Ece", "V"),
-    0x000B: ("<f8", "<I>", "mA"),
-    0x000D: ("<f8", "(Q-Qo)", "mA·h"),
-    0x0010: ("<f4", "Analog IN 1", "V"),
-    0x0011: ("<f4", "Analog IN 2", "V"),
-    0x0013: ("<f4", "control_V", "V"),
-    0x0014: ("<f4", "control_I", "mA"),
-    0x0017: ("<f8", "dQ", "mA·h"),
-    0x0018: ("<f8", "cycle number", None),
-    0x0020: ("<f4", "freq", "Hz"),
-    0x0021: ("<f4", "|Ewe|", "V"),
-    0x0022: ("<f4", "|I|", "A"),
-    0x0023: ("<f4", "Phase(Z)", "deg"),
-    0x0024: ("<f4", "|Z|", "Ω"),
-    0x0025: ("<f4", "Re(Z)", "Ω"),
-    0x0026: ("<f4", "-Im(Z)", "Ω"),
-    0x0027: ("<u2", "I Range", None),
-    0x0046: ("<f4", "P", "W"),
-    0x004A: ("<f8", "Energy", "W·h"),
-    0x004B: ("<f4", "Analog OUT", "V"),
-    0x004C: ("<f4", "<I>", "mA"),
-    0x004D: ("<f4", "<Ewe>", "V"),
-    0x004E: ("<f4", "Cs⁻²", "µF⁻²"),
-    0x0060: ("<f4", "|Ece|", "V"),
-    0x0062: ("<f4", "Phase(Zce)", "deg"),
-    0x0063: ("<f4", "|Zce|", "Ω"),
-    0x0064: ("<f4", "Re(Zce)", "Ω"),
-    0x0065: ("<f4", "-Im(Zce)", "Ω"),
-    0x007B: ("<f8", "Energy charge", "W·h"),
-    0x007C: ("<f8", "Energy discharge", "W·h"),
-    0x007D: ("<f8", "Capacitance charge", "µF"),
-    0x007E: ("<f8", "Capacitance discharge", "µF"),
-    0x0083: ("<u2", "Ns", None),
-    0x00A3: ("<f4", "|Estack|", "V"),
-    0x00A8: ("<f4", "Rcmp", "Ω"),
-    0x00A9: ("<f4", "Cs", "µF"),
-    0x00AC: ("<f4", "Cp", "µF"),
-    0x00AD: ("<f4", "Cp⁻²", "µF⁻²"),
-    0x00AE: ("<f4", "<Ewe>", "V"),
-    0x00F1: ("<f4", "|E1|", "V"),
-    0x00F2: ("<f4", "|E2|", "V"),
-    0x010F: ("<f4", "Phase(Z1)", "deg"),
-    0x0110: ("<f4", "Phase(Z2)", "deg"),
-    0x012D: ("<f4", "|Z1|", "Ω"),
-    0x012E: ("<f4", "|Z2|", "Ω"),
-    0x014B: ("<f4", "Re(Z1)", "Ω"),
-    0x014C: ("<f4", "Re(Z2)", "Ω"),
-    0x0169: ("<f4", "-Im(Z1)", "Ω"),
-    0x016A: ("<f4", "-Im(Z2)", "Ω"),
-    0x0187: ("<f4", "<E1>", "V"),
-    0x0188: ("<f4", "<E2>", "V"),
-    0x01A6: ("<f4", "Phase(Zstack)", "deg"),
-    0x01A7: ("<f4", "|Zstack|", "Ω"),
-    0x01A8: ("<f4", "Re(Zstack)", "Ω"),
-    0x01A9: ("<f4", "-Im(Zstack)", "Ω"),
-    0x01AA: ("<f4", "<Estack>", "V"),
-    0x01AE: ("<f4", "Phase(Zwe-ce)", "deg"),
-    0x01AF: ("<f4", "|Zwe-ce|", "Ω"),
-    0x01B0: ("<f4", "Re(Zwe-ce)", "Ω"),
-    0x01B1: ("<f4", "-Im(Zwe-ce)", "Ω"),
-    0x01B2: ("<f4", "(Q-Qo)", "C"),
-    0x01B3: ("<f4", "dQ", "C"),
-    0x01B9: ("<f4", "<Ece>", "V"),
-    0x01CE: ("<f4", "Temperature", "°C"),
-    0x01D3: ("<f8", "Q charge or discharge", "mA·h"),
-    0x01D4: ("<u4", "half cycle", None),
-    0x01D5: ("<u4", "z cycle", None),
-    0x01D7: ("<f4", "<Ece>", "V"),
-    0x01D9: ("<f4", "THD Ewe", "%"),
-    0x01DA: ("<f4", "THD I", "%"),
-    0x01DB: ("<f4", "THD Ece", "%"),
-    0x01DC: ("<f4", "NSD Ewe", "%"),
-    0x01DD: ("<f4", "NSD I", "%"),
-    0x01DE: ("<f4", "NSD Ece", "%"),
-    0x01DF: ("<f4", "NSR Ewe", "%"),
-    0x01E0: ("<f4", "NSR I", "%"),
-    0x01E1: ("<f4", "NSR Ece", "%"),
-    0x01E6: ("<f4", "|Ewe h2|", "V"),
-    0x01E7: ("<f4", "|Ewe h3|", "V"),
-    0x01E8: ("<f4", "|Ewe h4|", "V"),
-    0x01E9: ("<f4", "|Ewe h5|", "V"),
-    0x01EA: ("<f4", "|Ewe h6|", "V"),
-    0x01EB: ("<f4", "|Ewe h7|", "V"),
-    0x01EC: ("<f4", "|I h2|", "A"),
-    0x01ED: ("<f4", "|I h3|", "A"),
-    0x01EE: ("<f4", "|I h4|", "A"),
-    0x01EF: ("<f4", "|I h5|", "A"),
-    0x01F0: ("<f4", "|I h6|", "A"),
-    0x01F1: ("<f4", "|I h7|", "A"),
-    0x01F2: ("<f4", "|Ece h2|", "V"),
-    0x01F3: ("<f4", "|Ece h3|", "V"),
-    0x01F4: ("<f4", "|Ece h4|", "V"),
-    0x01F5: ("<f4", "|Ece h5|", "V"),
-    0x01F6: ("<f4", "|Ece h6|", "V"),
-    0x01F7: ("<f4", "|Ece h7|", "V"),
-}
-
-
-# Relates the offset in log data to the corresponding dtype and name.
-# NOTE: The safety limits are maybe at 0x200?
-# NOTE: The log also seems to contain the settings again. These are left
-# away for now.
-# NOTE: Looking at .mpl files, the log module appears to consist of
-# multiple 'modify on' sections, each starting with an OLE timestamp.
-log_dtypes = {
-    0x0009: ("|u1", "channel_number"),
-    0x00AB: ("<u2", "channel_sn"),
-    0x01F8: ("<f4", "Ewe_ctrl_min"),
-    0x01FC: ("<f4", "Ewe_ctrl_max"),
-    0x0249: ("<f8", "ole_timestamp"),
-    0x0251: ("pascal", "filename"),
-    0x0351: ("pascal", "host"),
-    0x0384: ("pascal", "address"),
-    0x03B7: ("pascal", "ec_lab_version"),
-    0x03BE: ("pascal", "server_version"),
-    0x03C5: ("pascal", "interpreter_version"),
-    0x03CF: ("pascal", "device_sn"),
-    0x0922: ("|u1", "averaging_points"),
-}
-
-
-extdev_dtypes = {
-    0x0036: ("pascal", "Analog IN 1"),
-    0x0052: ("<f4", "Analog IN 1 max V"),
-    0x0056: ("<f4", "Analog IN 1 min V"),
-    0x005A: ("<f4", "Analog IN 1 max x"),
-    0x005E: ("<f4", "Analog IN 1 min x"),
-    0x0063: ("pascal", "Analog IN 2"),
-    0x007F: ("<f4", "Analog IN 2 max V"),
-    0x0083: ("<f4", "Analog IN 2 min V"),
-    0x0087: ("<f4", "Analog IN 2 max x"),
-    0x008B: ("<f4", "Analog IN 2 min x"),
-}
+import numpy as np
+
+# Module header starting after each MODULE keyword.
+module_header_dtype = np.dtype(
+    [
+        ("short_name", "|S10"),
+        ("long_name", "|S25"),
+        ("length", "<u4"),
+        ("version", "<u4"),
+        ("date", "|S8"),
+    ]
+)
+
+
+# Relates the offset in the settings data to the corresponding dtype and
+# name. Maybe watch out for very long pascal strings as they may span
+# over the entire zero padding and shift the offsets.
+settings_dtypes = {
+    0x0007: ("pascal", "comments"),
+    0x0107: ("<f4", "active_material_mass"),
+    0x010B: ("<f4", "at_x"),
+    0x010F: ("<f4", "molecular_weight"),
+    0x0113: ("<f4", "atomic_weight"),
+    0x0117: ("<f4", "acquisition_start"),
+    0x011B: ("<u2", "e_transferred"),
+    0x011E: ("pascal", "electrode_material"),
+    0x01C0: ("pascal", "electrolyte"),
+    0x0211: ("<f4", "electrode_area"),
+    0x0215: ("pascal", "reference_electrode"),
+    0x024C: ("<f4", "characteristic_mass"),
+    0x025C: ("<f4", "battery_capacity"),
+    0x0260: ("|u1", "battery_capacity_unit"),
+    # NOTE: The compliance limits are apparently not always at this
+    # offset, hence commented out...
+    # 0x19d2: ("<f4", "compliance_min"),
+    # 0x19d6: ("<f4", "compliance_max"),
+}
+
+
+# Maps the flag column ID bytes to the corresponding bitmask and name.
+flag_columns = {
+    0x0001: (0b00000011, "mode"),
+    0x0002: (0b00000100, "ox or red"),
+    0x0003: (0b00001000, "error"),
+    0x0015: (0b00010000, "control changes"),
+    0x001F: (0b00100000, "Ns changes"),
+    # NOTE: I think the missing bitmask (0b01000000) is a stop bit. It
+    # sometimes appears in the flag byte of the very last data point.
+    0x0041: (0b10000000, "counter inc."),
+}
+
+
+# Maps the data column ID bytes to the corresponding dtype, name and
+# unit.
+data_columns = {
+    0x0004: ("<f8", "time", "s"),
+    0x0005: ("<f4", "control_V_I", "V/mA"),
+    0x0006: ("<f4", "Ewe", "V"),
+    0x0007: ("<f8", "dq", "mA·h"),
+    0x0008: ("<f4", "I", "mA"),
+    0x0009: ("<f4", "Ece", "V"),
+    0x000B: ("<f8", "<I>", "mA"),
+    0x000D: ("<f8", "(Q-Qo)", "mA·h"),
+    0x0010: ("<f4", "Analog IN 1", "V"),
+    0x0011: ("<f4", "Analog IN 2", "V"),
+    0x0013: ("<f4", "control_V", "V"),
+    0x0014: ("<f4", "control_I", "mA"),
+    0x0017: ("<f8", "dQ", "mA·h"),
+    0x0018: ("<f8", "cycle number", None),
+    0x0020: ("<f4", "freq", "Hz"),
+    0x0021: ("<f4", "|Ewe|", "V"),
+    0x0022: ("<f4", "|I|", "A"),
+    0x0023: ("<f4", "Phase(Z)", "deg"),
+    0x0024: ("<f4", "|Z|", "Ω"),
+    0x0025: ("<f4", "Re(Z)", "Ω"),
+    0x0026: ("<f4", "-Im(Z)", "Ω"),
+    0x0027: ("<u2", "I Range", None),
+    0x0046: ("<f4", "P", "W"),
+    0x004A: ("<f8", "Energy", "W·h"),
+    0x004B: ("<f4", "Analog OUT", "V"),
+    0x004C: ("<f4", "<I>", "mA"),
+    0x004D: ("<f4", "<Ewe>", "V"),
+    0x004E: ("<f4", "Cs⁻²", "µF⁻²"),
+    0x0060: ("<f4", "|Ece|", "V"),
+    0x0062: ("<f4", "Phase(Zce)", "deg"),
+    0x0063: ("<f4", "|Zce|", "Ω"),
+    0x0064: ("<f4", "Re(Zce)", "Ω"),
+    0x0065: ("<f4", "-Im(Zce)", "Ω"),
+    0x007B: ("<f8", "Energy charge", "W·h"),
+    0x007C: ("<f8", "Energy discharge", "W·h"),
+    0x007D: ("<f8", "Capacitance charge", "µF"),
+    0x007E: ("<f8", "Capacitance discharge", "µF"),
+    0x0083: ("<u2", "Ns", None),
+    0x00A3: ("<f4", "|Estack|", "V"),
+    0x00A8: ("<f4", "Rcmp", "Ω"),
+    0x00A9: ("<f4", "Cs", "µF"),
+    0x00AC: ("<f4", "Cp", "µF"),
+    0x00AD: ("<f4", "Cp⁻²", "µF⁻²"),
+    0x00AE: ("<f4", "<Ewe>", "V"),
+    0x00F1: ("<f4", "|E1|", "V"),
+    0x00F2: ("<f4", "|E2|", "V"),
+    0x010F: ("<f4", "Phase(Z1)", "deg"),
+    0x0110: ("<f4", "Phase(Z2)", "deg"),
+    0x012D: ("<f4", "|Z1|", "Ω"),
+    0x012E: ("<f4", "|Z2|", "Ω"),
+    0x014B: ("<f4", "Re(Z1)", "Ω"),
+    0x014C: ("<f4", "Re(Z2)", "Ω"),
+    0x0169: ("<f4", "-Im(Z1)", "Ω"),
+    0x016A: ("<f4", "-Im(Z2)", "Ω"),
+    0x0187: ("<f4", "<E1>", "V"),
+    0x0188: ("<f4", "<E2>", "V"),
+    0x01A6: ("<f4", "Phase(Zstack)", "deg"),
+    0x01A7: ("<f4", "|Zstack|", "Ω"),
+    0x01A8: ("<f4", "Re(Zstack)", "Ω"),
+    0x01A9: ("<f4", "-Im(Zstack)", "Ω"),
+    0x01AA: ("<f4", "<Estack>", "V"),
+    0x01AE: ("<f4", "Phase(Zwe-ce)", "deg"),
+    0x01AF: ("<f4", "|Zwe-ce|", "Ω"),
+    0x01B0: ("<f4", "Re(Zwe-ce)", "Ω"),
+    0x01B1: ("<f4", "-Im(Zwe-ce)", "Ω"),
+    0x01B2: ("<f4", "(Q-Qo)", "C"),
+    0x01B3: ("<f4", "dQ", "C"),
+    0x01B9: ("<f4", "<Ece>", "V"),
+    0x01CE: ("<f4", "Temperature", "°C"),
+    0x01D3: ("<f8", "Q charge or discharge", "mA·h"),
+    0x01D4: ("<u4", "half cycle", None),
+    0x01D5: ("<u4", "z cycle", None),
+    0x01D7: ("<f4", "<Ece>", "V"),
+    0x01D9: ("<f4", "THD Ewe", "%"),
+    0x01DA: ("<f4", "THD I", "%"),
+    0x01DB: ("<f4", "THD Ece", "%"),
+    0x01DC: ("<f4", "NSD Ewe", "%"),
+    0x01DD: ("<f4", "NSD I", "%"),
+    0x01DE: ("<f4", "NSD Ece", "%"),
+    0x01DF: ("<f4", "NSR Ewe", "%"),
+    0x01E0: ("<f4", "NSR I", "%"),
+    0x01E1: ("<f4", "NSR Ece", "%"),
+    0x01E6: ("<f4", "|Ewe h2|", "V"),
+    0x01E7: ("<f4", "|Ewe h3|", "V"),
+    0x01E8: ("<f4", "|Ewe h4|", "V"),
+    0x01E9: ("<f4", "|Ewe h5|", "V"),
+    0x01EA: ("<f4", "|Ewe h6|", "V"),
+    0x01EB: ("<f4", "|Ewe h7|", "V"),
+    0x01EC: ("<f4", "|I h2|", "A"),
+    0x01ED: ("<f4", "|I h3|", "A"),
+    0x01EE: ("<f4", "|I h4|", "A"),
+    0x01EF: ("<f4", "|I h5|", "A"),
+    0x01F0: ("<f4", "|I h6|", "A"),
+    0x01F1: ("<f4", "|I h7|", "A"),
+    0x01F2: ("<f4", "|Ece h2|", "V"),
+    0x01F3: ("<f4", "|Ece h3|", "V"),
+    0x01F4: ("<f4", "|Ece h4|", "V"),
+    0x01F5: ("<f4", "|Ece h5|", "V"),
+    0x01F6: ("<f4", "|Ece h6|", "V"),
+    0x01F7: ("<f4", "|Ece h7|", "V"),
+}
+
+
+# Relates the offset in log data to the corresponding dtype and name.
+# NOTE: The safety limits are maybe at 0x200?
+# NOTE: The log also seems to contain the settings again. These are left
+# away for now.
+# NOTE: Looking at .mpl files, the log module appears to consist of
+# multiple 'modify on' sections, each starting with an OLE timestamp.
+log_dtypes = {
+    0x0009: ("|u1", "channel_number"),
+    0x00AB: ("<u2", "channel_sn"),
+    0x01F8: ("<f4", "Ewe_ctrl_min"),
+    0x01FC: ("<f4", "Ewe_ctrl_max"),
+    0x0249: ("<f8", "ole_timestamp"),
+    0x0251: ("pascal", "filename"),
+    0x0351: ("pascal", "host"),
+    0x0384: ("pascal", "address"),
+    0x03B7: ("pascal", "ec_lab_version"),
+    0x03BE: ("pascal", "server_version"),
+    0x03C5: ("pascal", "interpreter_version"),
+    0x03CF: ("pascal", "device_sn"),
+    0x0922: ("|u1", "averaging_points"),
+}
+
+
+extdev_dtypes = {
+    0x0036: ("pascal", "Analog IN 1"),
+    0x0052: ("<f4", "Analog IN 1 max V"),
+    0x0056: ("<f4", "Analog IN 1 min V"),
+    0x005A: ("<f4", "Analog IN 1 max x"),
+    0x005E: ("<f4", "Analog IN 1 min x"),
+    0x0063: ("pascal", "Analog IN 2"),
+    0x007F: ("<f4", "Analog IN 2 max V"),
+    0x0083: ("<f4", "Analog IN 2 min V"),
+    0x0087: ("<f4", "Analog IN 2 max x"),
+    0x008B: ("<f4", "Analog IN 2 min x"),
+}
```

### Comparing `yadg-5.0.1/src/yadg/parsers/electrochem/eclabcommon/techniques.py` & `yadg-5.0.2/src/yadg/parsers/electrochem/eclabcommon/techniques.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,1217 +1,1218 @@
-"""
-**eclabtechniques**: Parameters for implemented techniques.
------------------------------------------------------------
-
-Implemented techniques:
-
-    - CA - Chronoamperometry / Chronocoulometry
-    - CP - Chronopotentiometry
-    - CV - Cyclic Voltammetry
-    - GCPL - Galvanostatic Cycling with Potential Limitation
-    - GEIS - Galvano Electrochemical Impedance Spectroscopy
-    - LOOP - Loop
-    - LSV - Linear Sweep Voltammetry
-    - MB - Modulo Bat
-    - OCV - Open Circuit Voltage
-    - PEIS - Potentio Electrochemical Impedance Spectroscopy
-    - WAIT - Wait
-    - ZIR - IR compensation (PEIS)
-
-The module also implements resolution determination for parameters of techniques,
-in :func:`get_resolution`.
-
-"""
-import re
-import numpy as np
-from typing import Union
-import bisect
-import logging
-
-logger = logging.getLogger(__name__)
-
-
-# Short helper function for constructing params.
-def _prepend_ns(settings: list[str], params: list) -> list[str]:
-    """Prepends the 'Ns' parameter to the parameters if present.
-
-    Parameters
-    ----------
-    settings
-        The list of settings from the start of an .mpt or .mps file.
-    params
-        A list containing the first part of the technique parameter
-        names. The Ns is prepended to this if present in the settings.
-
-    Returns
-    -------
-    list[str]
-        The 'Ns'-prepended parameters or the unchanged parameters.
-
-    """
-    ns_match = re.search(r"^Ns.+", "\n".join(settings))
-    if ns_match:
-        return ["Ns"] + params
-    return params
-
-
-# ~~~~~~~~~~~~~ Chronoamperometry / Chronocoulometry ~~~~~~~~~~~~~
-def _ca_params(settings: list[str]) -> list[str]:
-    """Constructs the parameter names for the CA technique."""
-    params = [
-        "Ei",
-        "Ei_vs",
-        "ti",
-        "Imax",
-        "Imax_unit",
-        "Imin",
-        "Imin_unit",
-        "dQM",
-        "dQM_unit",
-        "record",
-        "dI",
-        "dI_unit",
-        "dQ",
-        "dQ_unit",
-        "dt",
-        "dta",
-        "E_range_min",
-        "E_range_max",
-        "I_range",
-        "I_range_min",
-        "I_range_max",
-        "I_range_init",
-        "bandwidth",
-        "goto_Ns",
-        "nc_cycles",
-    ]
-    return _prepend_ns(settings, params)
-
-
-_ca_params_dtypes = [
-    np.dtype(
-        [
-            ("Ei", "<f4"),
-            ("Ei_vs", "|u1"),
-            ("ti", "<f4"),
-            ("Imax", "<f4"),
-            ("Imax_unit", "|u1"),
-            ("Imin", "<f4"),
-            ("Imin_unit", "|u1"),
-            ("dQM", "<f4"),
-            ("dQM_unit", "|u1"),
-            ("record", "|u1"),
-            ("dI", "<f4"),
-            ("dI_unit", "|u1"),
-            ("dQ", "<f4"),
-            ("dQ_unit", "|u1"),
-            ("dt", "<f4"),
-            ("dta", "<f4"),
-            ("E_range_min", "<f4"),
-            ("E_range_max", "<f4"),
-            ("I_range", "|u1"),
-            ("I_range_min", "|u1"),
-            ("I_range_max", "|u1"),
-            ("I_range_init", "|u1"),
-            ("bandwidth", "u1"),
-            ("goto_Ns", "<u4"),
-            ("nc_cycles", "<u4"),
-        ]
-    )
-]
-
-
-# ~~~~~~~~~~~~~ Chronopotentiometry ~~~~~~~~~~~~~
-def _cp_params(settings: list[str]) -> list[str]:
-    """Constructs the parameter names for the CP technique."""
-    params = [
-        "Is",
-        "Is_unit",
-        "Is_vs",
-        "ts",
-        "EM",
-        "dQM",
-        "dQM_unit",
-        "record",
-        "dEs",
-        "dts",
-        "E_range_min",
-        "E_range_max",
-        "I_range",
-        "bandwidth",
-        "goto_Ns",
-        "nc_cycles",
-    ]
-    return _prepend_ns(settings, params)
-
-
-_cp_params_dtypes = [
-    np.dtype(
-        [
-            ("Is", "<f4"),
-            ("Is_unit", "|u1"),
-            ("Is_vs", "|u1"),
-            ("ts", "<f4"),
-            ("EM", "<f4"),
-            ("dQM", "<f4"),
-            ("dQM_unit", "|u1"),
-            ("record", "|u1"),
-            ("dEs", "<f4"),
-            ("dts", "<f4"),
-            ("E_range_min", "<f4"),
-            ("E_range_max", "<f4"),
-            ("I_range", "|u1"),
-            ("bandwidth", "|u1"),
-            ("goto_Ns", "<u4"),
-            ("nc_cycles", "<u4"),
-        ]
-    )
-]
-
-
-# ~~~~~~~~~~~~~ Cyclic Voltammetry ~~~~~~~~~~~~~
-def _cv_params(settings: list[str]) -> list[str]:
-    """Constructs the parameter names for the CV technique."""
-    params = [
-        "Ei",
-        "Ei_vs",
-        "dE/dt",
-        "dE/dt_unit",
-        "E1",
-        "E1_vs",
-        "step_percent",
-        "N",
-        "E_range_min",
-        "E_range_max",
-        "I_range",
-        "I_range_min",
-        "I_range_max",
-        "I_range_init",
-        "bandwidth",
-        "E2",
-        "E2_vs",
-        "nc_cycles",
-        "reverse_scan",
-        "Ef",
-        "Ef_vs",
-    ]
-    return params
-
-
-_cv_params_dtypes = [
-    np.dtype(
-        [
-            ("Ei", "<f4"),
-            ("Ei_vs", "|u1"),
-            ("dE/dt", "<f4"),
-            ("dE/dt_unit", "|u1"),
-            ("E1", "<f4"),
-            ("E1_vs", "|u1"),
-            ("step_percent", "|u1"),
-            ("N", "<u4"),
-            ("E_range_min", "<f4"),
-            ("E_range_max", "<f4"),
-            ("I_range", "|u1"),
-            ("I_range_min", "|u1"),
-            ("I_range_max", "|u1"),
-            ("I_range_init", "|u1"),
-            ("bandwidth", "u1"),
-            ("E2", "<f4"),
-            ("E2_vs", "|u1"),
-            ("nc_cycles", "<u4"),
-            ("reverse_scan", "|u1"),
-            ("Ef", "<f4"),
-            ("Ef_vs", "|u1"),
-        ]
-    )
-]
-
-
-# ~~~~~~~~~~~~~ Galvanostatic Cycling with Potential Limitation ~~~~~~~~~~~~~
-def _gcpl_params(settings: list[str]) -> list[str]:
-    """Constructs the parameter names for the GCPL technique."""
-    params = [
-        "set_I/C",
-        "Is",
-        "Is_unit",
-        "Is_vs",
-        "N",
-        "I_sign",
-        "t1",
-        "I_range",
-        "bandwidth",
-        "dE1",
-        "dt1",
-        "EM",
-        "tM",
-        "Im",
-        "Im_unit",
-        "dI/dt",
-        "dI/dt_unit",
-        "E_range_min",
-        "E_range_max",
-        "dq",
-        "dq_unit",
-        "dtq",
-        "dQM",
-        "dQM_unit",
-        "dxM",
-        "tR",
-        "dER/dt",
-        "dER",
-        "dtR",
-        "EL",
-        "goto_Ns",
-        "nc_cycles",
-    ]
-    return _prepend_ns(settings, params)
-
-
-_gcpl_params_dtypes = [
-    np.dtype(
-        [
-            ("set_I/C", "|u1"),
-            ("Is", "<f4"),
-            ("Is_unit", "|u1"),
-            ("Is_vs", "|u1"),
-            ("N", "f4"),
-            ("I_sign", "|u1"),
-            ("t1", "<f4"),
-            ("I_range", "|u1"),
-            ("bandwidth", "|u1"),
-            ("dE1", "<f4"),
-            ("dt1", "<f4"),
-            ("EM", "<f4"),
-            ("tM", "<f4"),
-            ("Im", "<f4"),
-            ("Im_unit", "|u1"),
-            ("dI/dt", "<f4"),
-            ("dI/dt_unit", "|u1"),
-            ("E_range_min", "<f4"),
-            ("E_range_max", "<f4"),
-            ("dq", "<f4"),
-            ("dq_unit", "|u1"),
-            ("dtq", "<f4"),
-            ("dQM", "<f4"),
-            ("dQM_unit", "|u1"),
-            ("dxM", "<f4"),
-            ("tR", "<f4"),
-            ("dER/dt", "<f4"),
-            ("dER", "<f4"),
-            ("dtR", "<f4"),
-            ("EL", "<f4"),
-            ("goto_Ns", "<u4"),
-            ("nc_cycles", "<u4"),
-        ]
-    )
-]
-
-
-# ~~~~~~~~~~~~~ Galvano Electrochemical Impedance Spectroscopy ~~~~~~~~~~~~~
-def _geis_params(settings: list[str]) -> list[str]:
-    """Constructs the parameter names for the GEIS technique."""
-    params = [
-        "sine_mode",
-        "Is",
-        "Is_unit",
-        "Is_vs",
-        "tIs",
-        "record",
-        "dE",
-        "dt",
-        "fi",
-        "fi_unit",
-        "ff",
-        "ff_unit",
-        "Nd",
-        "points",
-        "spacing",
-        "Ia/Va",
-        "Ia",
-        "Ia_unit",
-        "va_pourcent",  # Random French parameter name?
-        "pw",
-        "Na",
-        "corr",
-    ]
-    params = _prepend_ns(settings, params)
-    lim_nb_match = re.search(r"^lim_nb\s+(?P<val>.+)", "\n".join(settings))
-    if lim_nb_match:
-        lim_nb = int(max(lim_nb_match["val"].split()))
-        params.append("lim_nb")
-        for i, __ in enumerate(range(lim_nb), 1):
-            limit = [
-                f"limit_type{i}",
-                f"limit_comp{i}",
-                f"limit_value{i}",
-                f"limit_unit{i}",
-            ]
-            params += limit
-    params += [
-        "E_range_min",
-        "E_range_max",
-        "I_range",
-        "bandwidth",
-        "nc_cycles",
-        "goto_Ns",
-        "nr_cycles",
-        "inc_cycle",
-    ]
-    return params
-
-
-_geis_params_dtype = [
-    np.dtype(
-        [
-            ("sine_mode", "|u1"),
-            ("Is", "<f4"),
-            ("Is_unit", "|u1"),
-            ("Is_vs", "|u1"),
-            ("tIs", "<f4"),
-            ("record", "|u1"),
-            ("dE", "<f4"),
-            ("dt", "<f4"),
-            ("fi", "<f4"),
-            ("fi_unit", "|u1"),
-            ("ff", "<f4"),
-            ("ff_unit", "|u1"),
-            ("Nd", "<u4"),
-            ("points", "|u1"),
-            ("spacing", "|u1"),
-            ("Ia/Va", "|u1"),
-            ("Ia", "<f4"),
-            ("Ia_unit", "|u1"),
-            ("va_pourcent", "<f4"),
-            ("pw", "<f4"),
-            ("Na", "<u4"),
-            ("corr", "|u1"),
-            ("lim_nb", "|u1"),
-            ("limit_type1", "|u1"),
-            ("limit_comp1", "|u1"),
-            ("limit_value1", "<f4"),
-            ("limit_unit1", "|u1"),
-            ("limit_type2", "|u1"),
-            ("limit_comp2", "|u1"),
-            ("limit_value2", "<f4"),
-            ("limit_unit2", "|u1"),
-            ("limit_type3", "|u1"),
-            ("limit_comp3", "|u1"),
-            ("limit_value3", "<f4"),
-            ("limit_unit3", "|u1"),
-            ("limit_type4", "|u1"),
-            ("limit_comp4", "|u1"),
-            ("limit_value4", "<f4"),
-            ("limit_unit4", "|u1"),
-            ("limit_type5", "|u1"),
-            ("limit_comp5", "|u1"),
-            ("limit_value5", "<f4"),
-            ("limit_unit5", "|u1"),
-            ("limit_type6", "|u1"),
-            ("limit_comp6", "|u1"),
-            ("limit_value6", "<f4"),
-            ("limit_unit6", "|u1"),
-            ("E_range_min", "<f4"),
-            ("E_range_max", "<f4"),
-            ("I_range", "|u1"),
-            ("bandwidth", "|u1"),
-            ("nc_cycles", "<u4"),
-            ("goto_Ns", "<u4"),
-            ("nr_cycles", "<u4"),
-            ("inc_cycle", "<u4"),
-        ]
-    )
-]
-
-
-# ~~~~~~~~~~~~~ Loop ~~~~~~~~~~~~~
-def _loop_params(settings: list[str]) -> list[str]:
-    """Constructs the parameter names for the LOOP technique."""
-    params = ["goto_Ne", "nt_times"]
-    return params
-
-
-# ~~~~~~~~~~~~~ Linear Sweep Voltammetry ~~~~~~~~~~~~~
-def _lsv_params(settings: list[str]) -> list[str]:
-    """Constructs the parameter names for the LSV technique."""
-    params = [
-        "tR",
-        "dER/dt",
-        "dER",
-        "dtR",
-        "dE/dt",
-        "dE/dt_unit",
-        "Ei",
-        "Ei_vs",
-        "EL",
-        "EL_vs",
-        "record",
-        "dI",
-        "dI_unit",
-        "tI",
-        "step_percent",
-        "N",
-        "E_range_min",
-        "E_range_max",
-        "I_range",
-        "I_range_min",
-        "I_range_max",
-        "I_range_init",
-        "bandwidth",
-    ]
-    return params
-
-
-# ~~~~~~~~~~~~~ Linear Sweep Voltammetry ~~~~~~~~~~~~~
-_lsv_params_dtype = [
-    np.dtype(
-        [
-            ("tR", "<f4"),
-            ("dER/dt", "<f4"),
-            ("dER", "<f4"),
-            ("dtR", "<f4"),
-            ("dE/dt", "<f4"),
-            ("dE/dt_unit", "|u1"),
-            ("Ei", "<f4"),
-            ("Ei_vs", "|u1"),
-            ("EL", "<f4"),
-            ("EL_vs", "|u1"),
-            ("record", "|u1"),
-            ("dI", "<f4"),
-            ("dI_unit", "|u1"),
-            ("tI", "<f4"),
-            ("step_percent", "|u1"),
-            ("N", "<u4"),
-            ("E_range_min", "<f4"),
-            ("E_range_max", "<f4"),
-            ("I_range", "|u1"),
-            ("I_range_min", "|u1"),
-            ("I_range_max", "|u1"),
-            ("I_range_init", "|u1"),
-            ("bandwidth", "|u1"),
-        ]
-    )
-]
-
-
-# ~~~~~~~~~~~~~ Modulo Bat ~~~~~~~~~~~~~
-def _mb_params(settings: list[str]) -> list[str]:
-    """Constructs the parameter names for the MB technique."""
-    params = [
-        "ctrl_type",
-        "apply_I/C",
-        "ctrl1_val",
-        "ctrl1_val_unit",
-        "ctrl1_val_vs",
-        "ctrl2_val",
-        "ctrl2_val_unit",
-        "ctrl2_val_vs",
-        "ctrl3_val",
-        "ctrl3_val_unit",
-        "ctrl3_val_vs",
-        "N",
-        "charge/discharge",
-    ]
-    params = _prepend_ns(settings, params)
-    n1_match = re.search(r"N1\s+", "\n".join(settings))
-    print(f"{n1_match=}")
-    if n1_match:
-        n1 = [
-            "charge/discharge_1",
-            "apply_I/C_1",
-            "N1",
-            "ctrl4_val_unit",
-            "ctrl4_val_vs",
-        ]
-        params += n1
-    params += [
-        "ctrl_seq",
-        "ctrl_repeat",
-        "ctrl_trigger",
-        "ctrl_TO_t",
-        "ctrl_TO_t_unit",
-        "ctrl_Nd",
-        "ctrl_Na",
-        "ctrl_corr",
-    ]
-    lim_nb_match = re.search(r"lim_nb\s+(?P<val>.+)", "\n".join(settings))
-    if lim_nb_match:
-        lim_nb = int(max(lim_nb_match["val"].split()))
-        params.append("lim_nb")
-        for i, __ in enumerate(range(lim_nb), 1):
-            lim = [
-                f"lim{i}_type",
-                f"lim{i}_comp",
-                f"lim{i}_Q",
-                f"lim{i}_value",
-                f"lim{i}_value_unit",
-                f"lim{i}_action",
-                f"lim{i}_seq",
-            ]
-            params += lim
-    rec_nb_match = re.search(r"rec_nb\s+(?P<val>.+)", "\n".join(settings))
-    if rec_nb_match:
-        rec_nb = int(max(rec_nb_match["val"].split()))
-        params.append("rec_nb")
-        for i, __ in enumerate(range(rec_nb), 1):
-            rec = [f"rec{i}_type", f"rec{i}_value", f"rec{i}_value_unit"]
-            params += rec
-    params += [
-        "E_range_min",
-        "E_range_max",
-        "I_range",
-        "I_range_min",
-        "I_range_max",
-        "I_range_init",
-        "auto_rest",
-        "bandwidth",
-    ]
-    return params
-
-
-_mb_params_dtypes = [
-    np.dtype(
-        [
-            ("ctrl_type", "|u1"),
-            ("apply_I/C", "|u1"),
-            ("ctrl1_val", "<f4"),
-            ("ctrl1_val_unit", "|u1"),
-            ("ctrl1_val_vs", "|u1"),
-            ("ctrl2_val", "<f4"),
-            ("ctrl2_val_unit", "|u1"),
-            ("ctrl2_val_vs", "|u1"),
-            ("ctrl3_val", "<f4"),
-            ("ctrl3_val_unit", "|u1"),
-            ("ctrl3_val_vs", "|u1"),
-            ("N", "<f4"),
-            ("charge/discharge", "|u1"),
-            ("charge/discharge_1", "|u1"),
-            ("apply_I/C_1", "|u1"),
-            ("N1", "<f4"),
-            ("ctrl4_val", "<f4"),
-            ("ctrl4_val_unit", "|u1"),
-            ("ctrl_seq", "<u4"),
-            ("ctrl_repeat", "<u4"),
-            ("ctrl_trigger", "|u1"),
-            ("ctrl_TO_t", "<f4"),
-            ("ctrl_TO_t_unit", "|u1"),
-            ("ctrl_Nd", "<u4"),
-            ("ctrl_Na", "<u4"),
-            ("ctrl_corr", "|u1"),
-            ("lim_nb", "|u1"),
-            ("lim1_type", "|u1"),
-            ("lim1_comp", "|u1"),
-            ("lim1_Q", "|u1"),
-            ("lim1_value", "<f4"),
-            ("lim1_value_unit", "|u1"),
-            ("lim1_action", "|u1"),
-            ("lim1_seq", "<u4"),
-            ("lim2_type", "|u1"),
-            ("lim2_comp", "|u1"),
-            ("lim2_Q", "|u1"),
-            ("lim2_value", "<f4"),
-            ("lim2_value_unit", "|u1"),
-            ("lim2_action", "|u1"),
-            ("lim2_seq", "<u4"),
-            ("lim3_type", "|u1"),
-            ("lim3_comp", "|u1"),
-            ("lim3_Q", "|u1"),
-            ("lim3_value", "<f4"),
-            ("lim3_value_unit", "|u1"),
-            ("lim3_action", "|u1"),
-            ("lim3_seq", "<u4"),
-            ("rec_nb", "|u1"),
-            ("rec1_type", "|u1"),
-            ("rec1_value", "<f4"),
-            ("rec1_value_unit", "|u1"),
-            ("rec2_type", "|u1"),
-            ("rec2_value", "<f4"),
-            ("rec2_value_unit", "|u1"),
-            ("rec3_type", "|u1"),
-            ("rec3_value", "<f4"),
-            ("rec3_value_unit", "|u1"),
-            ("E_range_min", "<f4"),
-            ("E_range_max", "<f4"),
-            ("I_range", "|u1"),
-            ("I_range_min", "|u1"),
-            ("I_range_max", "|u1"),
-            ("I_range_init", "|u1"),
-            ("auto_rest", "|u1"),
-            ("bandwidth", "|u1"),
-        ]
-    ),
-    np.dtype(
-        [
-            ("ctrl_type", "|u1"),
-            ("apply_I/C", "|u1"),
-            ("ctrl1_val", "<f4"),
-            ("ctrl1_val_unit", "|u1"),
-            ("ctrl1_val_vs", "|u1"),
-            ("ctrl2_val", "<f4"),
-            ("ctrl2_val_unit", "|u1"),
-            ("ctrl2_val_vs", "|u1"),
-            ("ctrl3_val", "<f4"),
-            ("ctrl3_val_unit", "|u1"),
-            ("ctrl3_val_vs", "|u1"),
-            ("N", "<f4"),
-            ("charge/discharge", "|u1"),
-            ("ctrl_seq", "<u4"),
-            ("ctrl_repeat", "<u4"),
-            ("ctrl_trigger", "|u1"),
-            ("ctrl_TO_t", "<f4"),
-            ("ctrl_TO_t_unit", "|u1"),
-            ("ctrl_Nd", "<u4"),
-            ("ctrl_Na", "<u4"),
-            ("ctrl_corr", "|u1"),
-            ("lim_nb", "|u1"),
-            ("lim1_type", "|u1"),
-            ("lim1_comp", "|u1"),
-            ("lim1_Q", "|u1"),
-            ("lim1_value", "<f4"),
-            ("lim1_value_unit", "|u1"),
-            ("lim1_action", "|u1"),
-            ("lim1_seq", "<u4"),
-            ("lim2_type", "|u1"),
-            ("lim2_comp", "|u1"),
-            ("lim2_Q", "|u1"),
-            ("lim2_value", "<f4"),
-            ("lim2_value_unit", "|u1"),
-            ("lim2_action", "|u1"),
-            ("lim2_seq", "<u4"),
-            ("lim3_type", "|u1"),
-            ("lim3_comp", "|u1"),
-            ("lim3_Q", "|u1"),
-            ("lim3_value", "<f4"),
-            ("lim3_value_unit", "|u1"),
-            ("lim3_action", "|u1"),
-            ("lim3_seq", "<u4"),
-            ("rec_nb", "|u1"),
-            ("rec1_type", "|u1"),
-            ("rec1_value", "<f4"),
-            ("rec1_value_unit", "|u1"),
-            ("rec2_type", "|u1"),
-            ("rec2_value", "<f4"),
-            ("rec2_value_unit", "|u1"),
-            ("rec3_type", "|u1"),
-            ("rec3_value", "<f4"),
-            ("rec3_value_unit", "|u1"),
-            ("E_range_min", "<f4"),
-            ("E_range_max", "<f4"),
-            ("I_range", "|u1"),
-            ("I_range_min", "|u1"),
-            ("I_range_max", "|u1"),
-            ("I_range_init", "|u1"),
-            ("auto_rest", "|u1"),
-            ("bandwidth", "|u1"),
-        ]
-    ),
-    np.dtype(
-        [
-            ("ctrl_type", "|u1"),
-            ("apply_I/C", "|u1"),
-            ("current/potential", "|u1"),
-            ("ctrl1_val", "<f4"),
-            ("ctrl1_val_unit", "|u1"),
-            ("ctrl1_val_vs", "|u1"),
-            ("ctrl2_val", "<f4"),
-            ("ctrl2_val_unit", "|u1"),
-            ("ctrl2_val_vs", "|u1"),
-            ("ctrl3_val", "<f4"),
-            ("ctrl3_val_unit", "|u1"),
-            ("ctrl3_val_vs", "|u1"),
-            ("N", "<f4"),
-            ("charge/discharge", "|u1"),
-            ("charge/discharge_1", "|u1"),
-            ("apply_I/C_1", "|u1"),
-            ("N1", "<f4"),
-            ("ctrl4_val", "<f4"),
-            ("ctrl4_val_unit", "|u1"),
-            ("ctrl_seq", "<u4"),
-            ("ctrl_repeat", "<u4"),
-            ("ctrl_trigger", "|u1"),
-            ("ctrl_TO_t", "<f4"),
-            ("ctrl_TO_t_unit", "|u1"),
-            ("ctrl_Nd", "<u4"),
-            ("ctrl_Na", "<u4"),
-            ("ctrl_corr", "|u1"),
-            ("lim_nb", "|u1"),
-            ("lim1_type", "|u1"),
-            ("lim1_comp", "|u1"),
-            ("lim1_Q", "|u1"),
-            ("lim1_value", "<f4"),
-            ("lim1_value_unit", "|u1"),
-            ("lim1_action", "|u1"),
-            ("lim1_seq", "<u4"),
-            ("lim2_type", "|u1"),
-            ("lim2_comp", "|u1"),
-            ("lim2_Q", "|u1"),
-            ("lim2_value", "<f4"),
-            ("lim2_value_unit", "|u1"),
-            ("lim2_action", "|u1"),
-            ("lim2_seq", "<u4"),
-            ("lim3_type", "|u1"),
-            ("lim3_comp", "|u1"),
-            ("lim3_Q", "|u1"),
-            ("lim3_value", "<f4"),
-            ("lim3_value_unit", "|u1"),
-            ("lim3_action", "|u1"),
-            ("lim3_seq", "<u4"),
-            ("rec_nb", "|u1"),
-            ("rec1_type", "|u1"),
-            ("rec1_value", "<f4"),
-            ("rec1_value_unit", "|u1"),
-            ("rec2_type", "|u1"),
-            ("rec2_value", "<f4"),
-            ("rec2_value_unit", "|u1"),
-            ("rec3_type", "|u1"),
-            ("rec3_value", "<f4"),
-            ("rec3_value_unit", "|u1"),
-            ("E_range_min", "<f4"),
-            ("E_range_max", "<f4"),
-            ("I_range", "|u1"),
-            ("I_range_min", "|u1"),
-            ("I_range_max", "|u1"),
-            ("I_range_init", "|u1"),
-            ("auto_rest", "|u1"),
-            ("bandwidth", "|u1"),
-        ]
-    ),
-]
-
-
-# ~~~~~~~~~~~~~ Open Circuit Voltage ~~~~~~~~~~~~~
-def _ocv_params(settings: list[str]) -> list[str]:
-    """Constructs the parameter names for the OCV technique."""
-    params = ["tR", "dER/dt"]
-    record_match = re.search(r"^record.+", "\n".join(settings))
-    if record_match:
-        params += ["record"]
-    params += ["dER", "dtR", "E_range_min", "E_range_max"]
-    return params
-
-
-_ocv_params_dtypes = [
-    np.dtype(
-        [
-            ("tR", "<f4"),
-            ("dER/dt", "<f4"),
-            ("record", "|u1"),
-            ("dER", "<f4"),
-            ("dtR", "<f4"),
-            ("E_range_min", "<f4"),
-            ("E_range_max", "<f4"),
-        ]
-    ),
-    np.dtype(
-        [
-            ("tR", "<f4"),
-            ("dER/dt", "<f4"),
-            ("dER", "<f4"),
-            ("dtR", "<f4"),
-            ("E_range_min", "<f4"),
-            ("E_range_max", "<f4"),
-        ]
-    ),
-]
-
-
-# ~~~~~~~~~~~~~ Potentio Electrochemical Impedance Spectroscopy ~~~~~~~~~~~~~
-def _peis_params(settings: list[str]) -> list[str]:
-    """Constructs the parameter names for the PEIS technique."""
-    params = [
-        "sine_mode",
-        "E",
-        "E_vs",
-        "tE",
-        "record",
-        "dI",
-        "dI_unit",
-        "dt",
-        "fi",
-        "fi_unit",
-        "ff",
-        "ff_unit",
-        "Nd",
-        "points",
-        "spacing",
-        "Va",
-        "pw",
-        "Na",
-        "corr",
-    ]
-    params = _prepend_ns(settings, params)
-    lim_nb_match = re.search(r"^lim_nb\s+(?P<val>.+)", "\n".join(settings))
-    if lim_nb_match:
-        lim_nb = int(max(lim_nb_match["val"].split()))
-        params.append("lim_nb")
-        for i, __ in enumerate(range(lim_nb), 1):
-            limit = [
-                f"limit_type{i}",
-                f"limit_comp{i}",
-                f"limit_value{i}",
-                f"limit_unit{i}",
-            ]
-            params += limit
-    params += [
-        "E_range_min",
-        "E_range_max",
-        "I_range",
-        "bandwidth",
-        "nc_cycles",
-        "goto_Ns",
-        "nr_cycles",
-        "inc_cycle",
-    ]
-    return params
-
-
-_peis_params_dtypes = [
-    np.dtype(
-        [
-            ("sine_mode", "|u1"),
-            ("E", "<f4"),
-            ("E_vs", "|u1"),
-            ("tE", "<f4"),
-            ("record", "|u1"),
-            ("dI", "<f4"),
-            ("dI_unit", "|u1"),
-            ("dt", "<f4"),
-            ("fi", "<f4"),
-            ("fi_unit", "|u1"),
-            ("ff", "<f4"),
-            ("ff_unit", "|u1"),
-            ("Nd", "<u4"),
-            ("points", "|u1"),
-            ("spacing", "|u1"),
-            ("Va", "<f4"),
-            ("pw", "<f4"),
-            ("Na", "<u4"),
-            ("corr", "|u1"),
-            ("lim_nb", "|u1"),
-            ("limit_type1", "|u1"),
-            ("limit_comp1", "|u1"),
-            ("limit_value1", "<f4"),
-            ("limit_unit1", "|u1"),
-            ("limit_type2", "|u1"),
-            ("limit_comp2", "|u1"),
-            ("limit_value2", "<f4"),
-            ("limit_unit2", "|u1"),
-            ("limit_type3", "|u1"),
-            ("limit_comp3", "|u1"),
-            ("limit_value3", "<f4"),
-            ("limit_unit3", "|u1"),
-            ("limit_type4", "|u1"),
-            ("limit_comp4", "|u1"),
-            ("limit_value4", "<f4"),
-            ("limit_unit4", "|u1"),
-            ("limit_type5", "|u1"),
-            ("limit_comp5", "|u1"),
-            ("limit_value5", "<f4"),
-            ("limit_unit5", "|u1"),
-            ("limit_type6", "|u1"),
-            ("limit_comp6", "|u1"),
-            ("limit_value6", "<f4"),
-            ("limit_unit6", "|u1"),
-            ("E_range_min", "<f4"),
-            ("E_range_max", "<f4"),
-            ("I_range", "|u1"),
-            ("bandwidth", "|u1"),
-            ("nc_cycles", "<u4"),
-            ("goto_Ns", "<u4"),
-            ("nr_cycles", "<u4"),
-            ("inc_cycle", "<u4"),
-        ]
-    )
-]
-
-
-# ~~~~~~~~~~~~~ Wait ~~~~~~~~~~~~~
-def _wait_params(settings: list[str]) -> list[str]:
-    """Constructs the parameter names for the WAIT technique."""
-    params = [
-        "select",
-        "td",
-        "from",
-        "tech_num",
-        "ole_date",
-        "ole_time",
-        "record",
-        "dE",
-        "dI",
-        "dI_unit",
-        "dt",
-    ]
-    return params
-
-
-_wait_params_dtypes = [
-    np.dtype(
-        [
-            ("select", "|u1"),
-            ("td", "<u4"),
-            ("from", "|u1"),
-            ("tech_num", "|u1"),
-            ("ole_date", "<f4"),  # Why the hell would they split this?!
-            ("ole_time", "<f4"),
-            ("record", "|u1"),
-            ("dE", "<f4"),
-            ("dI", "<f4"),
-            ("dI_unit", "|u1"),
-            ("dt", "<f4"),
-        ]
-    )
-]
-
-
-# ~~~~~~~~~~~~~ IR compensation (PEIS) ~~~~~~~~~~~~~
-def _zir_params(settings: list[str]) -> list[str]:
-    """Constructs the parameter names for the ZIR technique."""
-    params = [
-        "E",
-        "E_vs",
-        "f",
-        "f_unit",
-        "Va",
-        "pw",
-        "Na",
-        "E_range_min",
-        "E_range_max",
-        "I_range",
-        "bandwidth",
-        "comp_level",
-        "use_results",
-        "comp_mode",
-    ]
-    return params
-
-
-_zir_params_dtypes = [
-    np.dtype(
-        [
-            ("E", "<f4"),
-            ("E_vs", "|u1"),
-            ("f", "<f4"),
-            ("f_unit", "|u1"),
-            ("Va", "<f4"),
-            ("pw", "<f4"),
-            ("Na", "<u4"),
-            ("E_range_min", "<f4"),
-            ("E_range_max", "<f4"),
-            ("I_range", "|u1"),
-            ("bandwidth", "|u1"),
-            ("comp_level", "|u1"),
-            ("use_results", "|u1"),
-            ("comp_mode", "|u1"),
-        ]
-    )
-]
-
-
-def technique_params(technique: str, settings: list[str]) -> tuple[str, list]:
-    """Constructs the parameter names for different techniques.
-
-    Parameters
-    ----------
-    technique
-        The full name of the technique.
-
-    settings
-        The list of settings from the start of an .mpt or .mps file.
-
-    Returns
-    -------
-    tuple[str, list]
-        The short technique name and a full list of technique parameter
-        names depending on what is present in the file.
-
-    """
-    if technique == "Chronoamperometry / Chronocoulometry":
-        return "CA", _ca_params(settings)
-    if technique == "Chronopotentiometry":
-        return "CP", _cp_params(settings)
-    if technique == "Cyclic Voltammetry":
-        return "CV", _cv_params(settings)
-    if technique == "Galvano Electrochemical Impedance Spectroscopy":
-        return "GEIS", _geis_params(settings)
-    if technique == "Galvanostatic Cycling with Potential Limitation":
-        return "GCPL", _gcpl_params(settings)
-    if technique == "IR compensation (PEIS)":
-        return "ZIR", _zir_params(settings)
-    if technique == "Linear Sweep Voltammetry":
-        return "LSV", _lsv_params(settings)
-    if technique == "Loop":
-        return "LOOP", _loop_params(settings)
-    if technique == "Modulo Bat":
-        return "mb", _mb_params(settings)
-    if technique == "Open Circuit Voltage":
-        return "OCV", _ocv_params(settings)
-    if technique == "Potentio Electrochemical Impedance Spectroscopy":
-        return "PEIS", _peis_params(settings)
-    if technique == "Wait":
-        return "WAIT", _wait_params(settings)
-    raise NotImplementedError(f"'{technique}' not implemented.")
-
-
-# Maps the technique byte to its corresponding dtype.
-technique_params_dtypes = {
-    0x04: ("GCPL", _gcpl_params_dtypes),
-    0x06: ("CV", _cv_params_dtypes),
-    0x0B: ("OCV", _ocv_params_dtypes),
-    0x18: ("CA", _ca_params_dtypes),
-    0x19: ("CP", _cp_params_dtypes),
-    0x1C: ("WAIT", _wait_params_dtypes),
-    0x1D: ("PEIS", _peis_params_dtypes),
-    0x1E: ("GEIS", _geis_params_dtype),
-    0x32: ("ZIR", _zir_params_dtypes),
-    0x6C: ("LSV", _lsv_params_dtype),
-    0x7F: ("MB", _mb_params_dtypes),
-}
-
-param_map = {
-    "I_range": (
-        ("1 A", 9, 1),
-        ("100 mA", 10, 1e-1),
-        ("10 mA", 11, 1e-2),
-        ("1 mA", 12, 1e-3),
-        ("100 µA", 13, 1e-4),
-        ("10 µA", 14, 1e-5),
-        ("1 µA", 15, 1e-6),
-        ("10 µA", 21, 1e-5),
-        ("1 µA", 22, 1e-6),
-        ("100 nA", 23, 1e-7),
-        ("10 nA", 24, 1e-8),
-        ("1 A", 37, 1),
-        ("100 mA", 38, 1e-1),
-        ("10 mA", 39, 1e-2),
-        ("1 mA", 40, 1e-3),
-        ("Auto", None, None),
-    ),
-    "Is_unit": (
-        ("A", 0),  # guess
-        ("mA", 1),
-        ("µA", 2),
-        ("nA", 3),  # guess
-        ("pA", 4),  # guess
-    ),
-    "set_I/C": (
-        ("I", 0),
-        ("C", 1),  # guess
-    ),
-    "apply_I/C": (
-        ("I", 0),
-        ("C", 1),
-    ),
-}
-
-
-def param_from_key(
-    param: str, key: Union[int, str], to_str: bool = True
-) -> Union[str, float]:
-    """
-    Convert a supplied key of a certain parameter to its string or float value.
-
-    The function uses the map defined in ``param_map`` to convert between the
-    entries in the tuples, which contain the :class:`str` value of the parameter
-    (present in ``.mpt`` files), the :class:`int` value of the parameter (present
-    in ``.mpr`` files), and the corresponding :class:`float` value in SI units.
-
-    Parameters
-    ----------
-    param
-        The name of the parameter, a key within the ``param_map``. If ``param``
-        is not present in ``param_map``, the supplied key is returned back.
-
-    key
-        The key of the parameter that is to be converted to a different representation.
-
-    to_str
-        A switch between :class:`str` and :class:`float` output.
-
-    Returns
-    -------
-    key: Union[str, float, int]
-        The key converted to the requested format.
-
-    """
-    ii = 1 if isinstance(key, int) else 0
-    if param in param_map:
-        for i in param_map[param]:
-            if i[ii] == key:
-                if to_str:
-                    return i[0]
-                else:
-                    return i[2]
-        raise ValueError(f"element '{key}' for parameter '{param}' not understood.")
-    return key
-
-
-def get_resolution(
-    name: str, value: float, unit: str, Erange: float, Irange: float
-) -> float:
-    """
-    Function that returns the resolution of a property based on its name, value,
-    E-range and I-range.
-
-    The values used here are hard-coded from VMP-3 potentiostats. Generally, the
-    resolution is returned, however in some cases only the accuracy is specified
-    (currently ``freq`` and ``Phase``).
-
-    """
-    if name in {"control_V/I", "control_V_I"}:
-        raise RuntimeError("")
-    elif name in {"control_V"}:
-        # VMP-3: bisect function between 5 µV and 300 µV, as the
-        # voltage is stored in a 16-bit int.
-        if Erange >= 20.0:
-            return 305.18e-6
-        else:
-            res = [5e-6, 10e-6, 20e-6, 50e-6, 100e-6, 150e-6, 200e-6, 300e-6, 305.18e-6]
-            i = bisect.bisect_right(res, Erange / np.iinfo(np.uint16).max)
-            return res[i]
-    elif name in {"control_I"}:
-        # VMP-3: 0.004% of FSR, 760 µV at 10 µA I-range
-        return max(Irange * 0.004 / 100, 760e-12)
-    elif unit in {"V", "mV", "μV"}:
-        # VMP-3: 0.0015% of FSR, 75 µV minimum
-        return max(Erange * 0.0015 / 100, 75e-6)
-    elif unit in {"A", "mA", "µA", "nA", "pA"}:
-        # VMP-3: 0.004% of FSR
-        if Irange is None:
-            logger.warning("'I range' not specified. Using 1 A.")
-            Irange = 1.0
-        return Irange * 0.004 / 100
-    elif unit in {"Hz"}:
-        # VMP-3: using accuracy: 1% of value
-        return value * 0.01
-    elif unit in {"deg"}:
-        # VMP-3: using accuracy: 1 degree
-        return 1.0
-    elif unit in {"Ω", "S", "W"}:
-        # [Ω] = [V]/[A];
-        # [S] = [A]/[V];
-        # [W] = [A]*[V];
-        return max(
-            get_resolution("U", value, "V", Erange, Irange),
-            get_resolution("I", value, "A", Erange, Irange),
-        )
-    elif unit in {"C"}:
-        # [C] = [A]*[s];
-        return get_resolution("I", value, "A", Erange, Irange)
-    elif unit in {"mA·h"}:
-        return get_resolution("Q", value / 3.6, "C", Erange, Irange)
-    elif unit in {"W·h"}:
-        return get_resolution("P", value / 3600, "W", Erange, Irange)
-    elif unit in {"µF"}:
-        # [F] = [C]/[V]
-        return max(
-            get_resolution("Q", value * 1e-6, "C", Erange, Irange),
-            get_resolution("U", value * 1e-6, "V", Erange, Irange),
-        )
-    elif unit in {"s"}:
-        # Based on the EC-Lib documentation,
-        # 50 us is a safe upper limit for timebase
-        return 50e-6
-    elif unit in {"%"}:
-        return 0.1
-    else:
-        raise RuntimeError(
-            f"Could not get resolution of quantity '{name}' with unit '{unit}."
-        )
+"""
+**eclabtechniques**: Parameters for implemented techniques.
+-----------------------------------------------------------
+
+Implemented techniques:
+
+    - CA - Chronoamperometry / Chronocoulometry
+    - CP - Chronopotentiometry
+    - CV - Cyclic Voltammetry
+    - GCPL - Galvanostatic Cycling with Potential Limitation
+    - GEIS - Galvano Electrochemical Impedance Spectroscopy
+    - LOOP - Loop
+    - LSV - Linear Sweep Voltammetry
+    - MB - Modulo Bat
+    - OCV - Open Circuit Voltage
+    - PEIS - Potentio Electrochemical Impedance Spectroscopy
+    - WAIT - Wait
+    - ZIR - IR compensation (PEIS)
+
+The module also implements resolution determination for parameters of techniques,
+in :func:`get_resolution`.
+
+"""
+import re
+import numpy as np
+from typing import Union
+import bisect
+import logging
+
+logger = logging.getLogger(__name__)
+
+
+# Short helper function for constructing params.
+def _prepend_ns(settings: list[str], params: list) -> list[str]:
+    """Prepends the 'Ns' parameter to the parameters if present.
+
+    Parameters
+    ----------
+    settings
+        The list of settings from the start of an .mpt or .mps file.
+    params
+        A list containing the first part of the technique parameter
+        names. The Ns is prepended to this if present in the settings.
+
+    Returns
+    -------
+    list[str]
+        The 'Ns'-prepended parameters or the unchanged parameters.
+
+    """
+    ns_match = re.search(r"^Ns.+", "\n".join(settings))
+    if ns_match:
+        return ["Ns"] + params
+    return params
+
+
+# ~~~~~~~~~~~~~ Chronoamperometry / Chronocoulometry ~~~~~~~~~~~~~
+def _ca_params(settings: list[str]) -> list[str]:
+    """Constructs the parameter names for the CA technique."""
+    params = [
+        "Ei",
+        "Ei_vs",
+        "ti",
+        "Imax",
+        "Imax_unit",
+        "Imin",
+        "Imin_unit",
+        "dQM",
+        "dQM_unit",
+        "record",
+        "dI",
+        "dI_unit",
+        "dQ",
+        "dQ_unit",
+        "dt",
+        "dta",
+        "E_range_min",
+        "E_range_max",
+        "I_range",
+        "I_range_min",
+        "I_range_max",
+        "I_range_init",
+        "bandwidth",
+        "goto_Ns",
+        "nc_cycles",
+    ]
+    return _prepend_ns(settings, params)
+
+
+_ca_params_dtypes = [
+    np.dtype(
+        [
+            ("Ei", "<f4"),
+            ("Ei_vs", "|u1"),
+            ("ti", "<f4"),
+            ("Imax", "<f4"),
+            ("Imax_unit", "|u1"),
+            ("Imin", "<f4"),
+            ("Imin_unit", "|u1"),
+            ("dQM", "<f4"),
+            ("dQM_unit", "|u1"),
+            ("record", "|u1"),
+            ("dI", "<f4"),
+            ("dI_unit", "|u1"),
+            ("dQ", "<f4"),
+            ("dQ_unit", "|u1"),
+            ("dt", "<f4"),
+            ("dta", "<f4"),
+            ("E_range_min", "<f4"),
+            ("E_range_max", "<f4"),
+            ("I_range", "|u1"),
+            ("I_range_min", "|u1"),
+            ("I_range_max", "|u1"),
+            ("I_range_init", "|u1"),
+            ("bandwidth", "u1"),
+            ("goto_Ns", "<u4"),
+            ("nc_cycles", "<u4"),
+        ]
+    )
+]
+
+
+# ~~~~~~~~~~~~~ Chronopotentiometry ~~~~~~~~~~~~~
+def _cp_params(settings: list[str]) -> list[str]:
+    """Constructs the parameter names for the CP technique."""
+    params = [
+        "Is",
+        "Is_unit",
+        "Is_vs",
+        "ts",
+        "EM",
+        "dQM",
+        "dQM_unit",
+        "record",
+        "dEs",
+        "dts",
+        "E_range_min",
+        "E_range_max",
+        "I_range",
+        "bandwidth",
+        "goto_Ns",
+        "nc_cycles",
+    ]
+    return _prepend_ns(settings, params)
+
+
+_cp_params_dtypes = [
+    np.dtype(
+        [
+            ("Is", "<f4"),
+            ("Is_unit", "|u1"),
+            ("Is_vs", "|u1"),
+            ("ts", "<f4"),
+            ("EM", "<f4"),
+            ("dQM", "<f4"),
+            ("dQM_unit", "|u1"),
+            ("record", "|u1"),
+            ("dEs", "<f4"),
+            ("dts", "<f4"),
+            ("E_range_min", "<f4"),
+            ("E_range_max", "<f4"),
+            ("I_range", "|u1"),
+            ("bandwidth", "|u1"),
+            ("goto_Ns", "<u4"),
+            ("nc_cycles", "<u4"),
+        ]
+    )
+]
+
+
+# ~~~~~~~~~~~~~ Cyclic Voltammetry ~~~~~~~~~~~~~
+def _cv_params(settings: list[str]) -> list[str]:
+    """Constructs the parameter names for the CV technique."""
+    params = [
+        "Ei",
+        "Ei_vs",
+        "dE/dt",
+        "dE/dt_unit",
+        "E1",
+        "E1_vs",
+        "step_percent",
+        "N",
+        "E_range_min",
+        "E_range_max",
+        "I_range",
+        "I_range_min",
+        "I_range_max",
+        "I_range_init",
+        "bandwidth",
+        "E2",
+        "E2_vs",
+        "nc_cycles",
+        "reverse_scan",
+        "Ef",
+        "Ef_vs",
+    ]
+    return params
+
+
+_cv_params_dtypes = [
+    np.dtype(
+        [
+            ("Ei", "<f4"),
+            ("Ei_vs", "|u1"),
+            ("dE/dt", "<f4"),
+            ("dE/dt_unit", "|u1"),
+            ("E1", "<f4"),
+            ("E1_vs", "|u1"),
+            ("step_percent", "|u1"),
+            ("N", "<u4"),
+            ("E_range_min", "<f4"),
+            ("E_range_max", "<f4"),
+            ("I_range", "|u1"),
+            ("I_range_min", "|u1"),
+            ("I_range_max", "|u1"),
+            ("I_range_init", "|u1"),
+            ("bandwidth", "u1"),
+            ("E2", "<f4"),
+            ("E2_vs", "|u1"),
+            ("nc_cycles", "<u4"),
+            ("reverse_scan", "|u1"),
+            ("Ef", "<f4"),
+            ("Ef_vs", "|u1"),
+        ]
+    )
+]
+
+
+# ~~~~~~~~~~~~~ Galvanostatic Cycling with Potential Limitation ~~~~~~~~~~~~~
+def _gcpl_params(settings: list[str]) -> list[str]:
+    """Constructs the parameter names for the GCPL technique."""
+    params = [
+        "set_I/C",
+        "Is",
+        "Is_unit",
+        "Is_vs",
+        "N",
+        "I_sign",
+        "t1",
+        "I_range",
+        "bandwidth",
+        "dE1",
+        "dt1",
+        "EM",
+        "tM",
+        "Im",
+        "Im_unit",
+        "dI/dt",
+        "dI/dt_unit",
+        "E_range_min",
+        "E_range_max",
+        "dq",
+        "dq_unit",
+        "dtq",
+        "dQM",
+        "dQM_unit",
+        "dxM",
+        "tR",
+        "dER/dt",
+        "dER",
+        "dtR",
+        "EL",
+        "goto_Ns",
+        "nc_cycles",
+    ]
+    return _prepend_ns(settings, params)
+
+
+_gcpl_params_dtypes = [
+    np.dtype(
+        [
+            ("set_I/C", "|u1"),
+            ("Is", "<f4"),
+            ("Is_unit", "|u1"),
+            ("Is_vs", "|u1"),
+            ("N", "f4"),
+            ("I_sign", "|u1"),
+            ("t1", "<f4"),
+            ("I_range", "|u1"),
+            ("bandwidth", "|u1"),
+            ("dE1", "<f4"),
+            ("dt1", "<f4"),
+            ("EM", "<f4"),
+            ("tM", "<f4"),
+            ("Im", "<f4"),
+            ("Im_unit", "|u1"),
+            ("dI/dt", "<f4"),
+            ("dI/dt_unit", "|u1"),
+            ("E_range_min", "<f4"),
+            ("E_range_max", "<f4"),
+            ("dq", "<f4"),
+            ("dq_unit", "|u1"),
+            ("dtq", "<f4"),
+            ("dQM", "<f4"),
+            ("dQM_unit", "|u1"),
+            ("dxM", "<f4"),
+            ("tR", "<f4"),
+            ("dER/dt", "<f4"),
+            ("dER", "<f4"),
+            ("dtR", "<f4"),
+            ("EL", "<f4"),
+            ("goto_Ns", "<u4"),
+            ("nc_cycles", "<u4"),
+        ]
+    )
+]
+
+
+# ~~~~~~~~~~~~~ Galvano Electrochemical Impedance Spectroscopy ~~~~~~~~~~~~~
+def _geis_params(settings: list[str]) -> list[str]:
+    """Constructs the parameter names for the GEIS technique."""
+    params = [
+        "sine_mode",
+        "Is",
+        "Is_unit",
+        "Is_vs",
+        "tIs",
+        "record",
+        "dE",
+        "dt",
+        "fi",
+        "fi_unit",
+        "ff",
+        "ff_unit",
+        "Nd",
+        "points",
+        "spacing",
+        "Ia/Va",
+        "Ia",
+        "Ia_unit",
+        "va_pourcent",  # Random French parameter name?
+        "pw",
+        "Na",
+        "corr",
+    ]
+    params = _prepend_ns(settings, params)
+    lim_nb_match = re.search(r"^lim_nb\s+(?P<val>.+)", "\n".join(settings))
+    if lim_nb_match:
+        lim_nb = int(max(lim_nb_match["val"].split()))
+        params.append("lim_nb")
+        for i, __ in enumerate(range(lim_nb), 1):
+            limit = [
+                f"limit_type{i}",
+                f"limit_comp{i}",
+                f"limit_value{i}",
+                f"limit_unit{i}",
+            ]
+            params += limit
+    params += [
+        "E_range_min",
+        "E_range_max",
+        "I_range",
+        "bandwidth",
+        "nc_cycles",
+        "goto_Ns",
+        "nr_cycles",
+        "inc_cycle",
+    ]
+    return params
+
+
+_geis_params_dtype = [
+    np.dtype(
+        [
+            ("sine_mode", "|u1"),
+            ("Is", "<f4"),
+            ("Is_unit", "|u1"),
+            ("Is_vs", "|u1"),
+            ("tIs", "<f4"),
+            ("record", "|u1"),
+            ("dE", "<f4"),
+            ("dt", "<f4"),
+            ("fi", "<f4"),
+            ("fi_unit", "|u1"),
+            ("ff", "<f4"),
+            ("ff_unit", "|u1"),
+            ("Nd", "<u4"),
+            ("points", "|u1"),
+            ("spacing", "|u1"),
+            ("Ia/Va", "|u1"),
+            ("Ia", "<f4"),
+            ("Ia_unit", "|u1"),
+            ("va_pourcent", "<f4"),
+            ("pw", "<f4"),
+            ("Na", "<u4"),
+            ("corr", "|u1"),
+            ("lim_nb", "|u1"),
+            ("limit_type1", "|u1"),
+            ("limit_comp1", "|u1"),
+            ("limit_value1", "<f4"),
+            ("limit_unit1", "|u1"),
+            ("limit_type2", "|u1"),
+            ("limit_comp2", "|u1"),
+            ("limit_value2", "<f4"),
+            ("limit_unit2", "|u1"),
+            ("limit_type3", "|u1"),
+            ("limit_comp3", "|u1"),
+            ("limit_value3", "<f4"),
+            ("limit_unit3", "|u1"),
+            ("limit_type4", "|u1"),
+            ("limit_comp4", "|u1"),
+            ("limit_value4", "<f4"),
+            ("limit_unit4", "|u1"),
+            ("limit_type5", "|u1"),
+            ("limit_comp5", "|u1"),
+            ("limit_value5", "<f4"),
+            ("limit_unit5", "|u1"),
+            ("limit_type6", "|u1"),
+            ("limit_comp6", "|u1"),
+            ("limit_value6", "<f4"),
+            ("limit_unit6", "|u1"),
+            ("E_range_min", "<f4"),
+            ("E_range_max", "<f4"),
+            ("I_range", "|u1"),
+            ("bandwidth", "|u1"),
+            ("nc_cycles", "<u4"),
+            ("goto_Ns", "<u4"),
+            ("nr_cycles", "<u4"),
+            ("inc_cycle", "<u4"),
+        ]
+    )
+]
+
+
+# ~~~~~~~~~~~~~ Loop ~~~~~~~~~~~~~
+def _loop_params(settings: list[str]) -> list[str]:
+    """Constructs the parameter names for the LOOP technique."""
+    params = ["goto_Ne", "nt_times"]
+    return params
+
+
+# ~~~~~~~~~~~~~ Linear Sweep Voltammetry ~~~~~~~~~~~~~
+def _lsv_params(settings: list[str]) -> list[str]:
+    """Constructs the parameter names for the LSV technique."""
+    params = [
+        "tR",
+        "dER/dt",
+        "dER",
+        "dtR",
+        "dE/dt",
+        "dE/dt_unit",
+        "Ei",
+        "Ei_vs",
+        "EL",
+        "EL_vs",
+        "record",
+        "dI",
+        "dI_unit",
+        "tI",
+        "step_percent",
+        "N",
+        "E_range_min",
+        "E_range_max",
+        "I_range",
+        "I_range_min",
+        "I_range_max",
+        "I_range_init",
+        "bandwidth",
+    ]
+    return params
+
+
+# ~~~~~~~~~~~~~ Linear Sweep Voltammetry ~~~~~~~~~~~~~
+_lsv_params_dtype = [
+    np.dtype(
+        [
+            ("tR", "<f4"),
+            ("dER/dt", "<f4"),
+            ("dER", "<f4"),
+            ("dtR", "<f4"),
+            ("dE/dt", "<f4"),
+            ("dE/dt_unit", "|u1"),
+            ("Ei", "<f4"),
+            ("Ei_vs", "|u1"),
+            ("EL", "<f4"),
+            ("EL_vs", "|u1"),
+            ("record", "|u1"),
+            ("dI", "<f4"),
+            ("dI_unit", "|u1"),
+            ("tI", "<f4"),
+            ("step_percent", "|u1"),
+            ("N", "<u4"),
+            ("E_range_min", "<f4"),
+            ("E_range_max", "<f4"),
+            ("I_range", "|u1"),
+            ("I_range_min", "|u1"),
+            ("I_range_max", "|u1"),
+            ("I_range_init", "|u1"),
+            ("bandwidth", "|u1"),
+        ]
+    )
+]
+
+
+# ~~~~~~~~~~~~~ Modulo Bat ~~~~~~~~~~~~~
+def _mb_params(settings: list[str]) -> list[str]:
+    """Constructs the parameter names for the MB technique."""
+    params = [
+        "ctrl_type",
+        "apply_I/C",
+        "ctrl1_val",
+        "ctrl1_val_unit",
+        "ctrl1_val_vs",
+        "ctrl2_val",
+        "ctrl2_val_unit",
+        "ctrl2_val_vs",
+        "ctrl3_val",
+        "ctrl3_val_unit",
+        "ctrl3_val_vs",
+        "N",
+        "charge/discharge",
+    ]
+    params = _prepend_ns(settings, params)
+    n1_match = re.search(r"N1\s+", "\n".join(settings))
+    print(f"{n1_match=}")
+    if n1_match:
+        n1 = [
+            "charge/discharge_1",
+            "apply_I/C_1",
+            "N1",
+            "ctrl4_val_unit",
+            "ctrl4_val_vs",
+        ]
+        params += n1
+    params += [
+        "ctrl_seq",
+        "ctrl_repeat",
+        "ctrl_trigger",
+        "ctrl_TO_t",
+        "ctrl_TO_t_unit",
+        "ctrl_Nd",
+        "ctrl_Na",
+        "ctrl_corr",
+    ]
+    lim_nb_match = re.search(r"lim_nb\s+(?P<val>.+)", "\n".join(settings))
+    if lim_nb_match:
+        lim_nb = int(max(lim_nb_match["val"].split()))
+        params.append("lim_nb")
+        for i, __ in enumerate(range(lim_nb), 1):
+            lim = [
+                f"lim{i}_type",
+                f"lim{i}_comp",
+                f"lim{i}_Q",
+                f"lim{i}_value",
+                f"lim{i}_value_unit",
+                f"lim{i}_action",
+                f"lim{i}_seq",
+            ]
+            params += lim
+    rec_nb_match = re.search(r"rec_nb\s+(?P<val>.+)", "\n".join(settings))
+    if rec_nb_match:
+        rec_nb = int(max(rec_nb_match["val"].split()))
+        params.append("rec_nb")
+        for i, __ in enumerate(range(rec_nb), 1):
+            rec = [f"rec{i}_type", f"rec{i}_value", f"rec{i}_value_unit"]
+            params += rec
+    params += [
+        "E_range_min",
+        "E_range_max",
+        "I_range",
+        "I_range_min",
+        "I_range_max",
+        "I_range_init",
+        "auto_rest",
+        "bandwidth",
+    ]
+    return params
+
+
+_mb_params_dtypes = [
+    np.dtype(
+        [
+            ("ctrl_type", "|u1"),
+            ("apply_I/C", "|u1"),
+            ("ctrl1_val", "<f4"),
+            ("ctrl1_val_unit", "|u1"),
+            ("ctrl1_val_vs", "|u1"),
+            ("ctrl2_val", "<f4"),
+            ("ctrl2_val_unit", "|u1"),
+            ("ctrl2_val_vs", "|u1"),
+            ("ctrl3_val", "<f4"),
+            ("ctrl3_val_unit", "|u1"),
+            ("ctrl3_val_vs", "|u1"),
+            ("N", "<f4"),
+            ("charge/discharge", "|u1"),
+            ("charge/discharge_1", "|u1"),
+            ("apply_I/C_1", "|u1"),
+            ("N1", "<f4"),
+            ("ctrl4_val", "<f4"),
+            ("ctrl4_val_unit", "|u1"),
+            ("ctrl_seq", "<u4"),
+            ("ctrl_repeat", "<u4"),
+            ("ctrl_trigger", "|u1"),
+            ("ctrl_TO_t", "<f4"),
+            ("ctrl_TO_t_unit", "|u1"),
+            ("ctrl_Nd", "<u4"),
+            ("ctrl_Na", "<u4"),
+            ("ctrl_corr", "|u1"),
+            ("lim_nb", "|u1"),
+            ("lim1_type", "|u1"),
+            ("lim1_comp", "|u1"),
+            ("lim1_Q", "|u1"),
+            ("lim1_value", "<f4"),
+            ("lim1_value_unit", "|u1"),
+            ("lim1_action", "|u1"),
+            ("lim1_seq", "<u4"),
+            ("lim2_type", "|u1"),
+            ("lim2_comp", "|u1"),
+            ("lim2_Q", "|u1"),
+            ("lim2_value", "<f4"),
+            ("lim2_value_unit", "|u1"),
+            ("lim2_action", "|u1"),
+            ("lim2_seq", "<u4"),
+            ("lim3_type", "|u1"),
+            ("lim3_comp", "|u1"),
+            ("lim3_Q", "|u1"),
+            ("lim3_value", "<f4"),
+            ("lim3_value_unit", "|u1"),
+            ("lim3_action", "|u1"),
+            ("lim3_seq", "<u4"),
+            ("rec_nb", "|u1"),
+            ("rec1_type", "|u1"),
+            ("rec1_value", "<f4"),
+            ("rec1_value_unit", "|u1"),
+            ("rec2_type", "|u1"),
+            ("rec2_value", "<f4"),
+            ("rec2_value_unit", "|u1"),
+            ("rec3_type", "|u1"),
+            ("rec3_value", "<f4"),
+            ("rec3_value_unit", "|u1"),
+            ("E_range_min", "<f4"),
+            ("E_range_max", "<f4"),
+            ("I_range", "|u1"),
+            ("I_range_min", "|u1"),
+            ("I_range_max", "|u1"),
+            ("I_range_init", "|u1"),
+            ("auto_rest", "|u1"),
+            ("bandwidth", "|u1"),
+        ]
+    ),
+    np.dtype(
+        [
+            ("ctrl_type", "|u1"),
+            ("apply_I/C", "|u1"),
+            ("ctrl1_val", "<f4"),
+            ("ctrl1_val_unit", "|u1"),
+            ("ctrl1_val_vs", "|u1"),
+            ("ctrl2_val", "<f4"),
+            ("ctrl2_val_unit", "|u1"),
+            ("ctrl2_val_vs", "|u1"),
+            ("ctrl3_val", "<f4"),
+            ("ctrl3_val_unit", "|u1"),
+            ("ctrl3_val_vs", "|u1"),
+            ("N", "<f4"),
+            ("charge/discharge", "|u1"),
+            ("ctrl_seq", "<u4"),
+            ("ctrl_repeat", "<u4"),
+            ("ctrl_trigger", "|u1"),
+            ("ctrl_TO_t", "<f4"),
+            ("ctrl_TO_t_unit", "|u1"),
+            ("ctrl_Nd", "<u4"),
+            ("ctrl_Na", "<u4"),
+            ("ctrl_corr", "|u1"),
+            ("lim_nb", "|u1"),
+            ("lim1_type", "|u1"),
+            ("lim1_comp", "|u1"),
+            ("lim1_Q", "|u1"),
+            ("lim1_value", "<f4"),
+            ("lim1_value_unit", "|u1"),
+            ("lim1_action", "|u1"),
+            ("lim1_seq", "<u4"),
+            ("lim2_type", "|u1"),
+            ("lim2_comp", "|u1"),
+            ("lim2_Q", "|u1"),
+            ("lim2_value", "<f4"),
+            ("lim2_value_unit", "|u1"),
+            ("lim2_action", "|u1"),
+            ("lim2_seq", "<u4"),
+            ("lim3_type", "|u1"),
+            ("lim3_comp", "|u1"),
+            ("lim3_Q", "|u1"),
+            ("lim3_value", "<f4"),
+            ("lim3_value_unit", "|u1"),
+            ("lim3_action", "|u1"),
+            ("lim3_seq", "<u4"),
+            ("rec_nb", "|u1"),
+            ("rec1_type", "|u1"),
+            ("rec1_value", "<f4"),
+            ("rec1_value_unit", "|u1"),
+            ("rec2_type", "|u1"),
+            ("rec2_value", "<f4"),
+            ("rec2_value_unit", "|u1"),
+            ("rec3_type", "|u1"),
+            ("rec3_value", "<f4"),
+            ("rec3_value_unit", "|u1"),
+            ("E_range_min", "<f4"),
+            ("E_range_max", "<f4"),
+            ("I_range", "|u1"),
+            ("I_range_min", "|u1"),
+            ("I_range_max", "|u1"),
+            ("I_range_init", "|u1"),
+            ("auto_rest", "|u1"),
+            ("bandwidth", "|u1"),
+        ]
+    ),
+    np.dtype(
+        [
+            ("ctrl_type", "|u1"),
+            ("apply_I/C", "|u1"),
+            ("current/potential", "|u1"),
+            ("ctrl1_val", "<f4"),
+            ("ctrl1_val_unit", "|u1"),
+            ("ctrl1_val_vs", "|u1"),
+            ("ctrl2_val", "<f4"),
+            ("ctrl2_val_unit", "|u1"),
+            ("ctrl2_val_vs", "|u1"),
+            ("ctrl3_val", "<f4"),
+            ("ctrl3_val_unit", "|u1"),
+            ("ctrl3_val_vs", "|u1"),
+            ("N", "<f4"),
+            ("charge/discharge", "|u1"),
+            ("charge/discharge_1", "|u1"),
+            ("apply_I/C_1", "|u1"),
+            ("N1", "<f4"),
+            ("ctrl4_val", "<f4"),
+            ("ctrl4_val_unit", "|u1"),
+            ("ctrl_seq", "<u4"),
+            ("ctrl_repeat", "<u4"),
+            ("ctrl_trigger", "|u1"),
+            ("ctrl_TO_t", "<f4"),
+            ("ctrl_TO_t_unit", "|u1"),
+            ("ctrl_Nd", "<u4"),
+            ("ctrl_Na", "<u4"),
+            ("ctrl_corr", "|u1"),
+            ("lim_nb", "|u1"),
+            ("lim1_type", "|u1"),
+            ("lim1_comp", "|u1"),
+            ("lim1_Q", "|u1"),
+            ("lim1_value", "<f4"),
+            ("lim1_value_unit", "|u1"),
+            ("lim1_action", "|u1"),
+            ("lim1_seq", "<u4"),
+            ("lim2_type", "|u1"),
+            ("lim2_comp", "|u1"),
+            ("lim2_Q", "|u1"),
+            ("lim2_value", "<f4"),
+            ("lim2_value_unit", "|u1"),
+            ("lim2_action", "|u1"),
+            ("lim2_seq", "<u4"),
+            ("lim3_type", "|u1"),
+            ("lim3_comp", "|u1"),
+            ("lim3_Q", "|u1"),
+            ("lim3_value", "<f4"),
+            ("lim3_value_unit", "|u1"),
+            ("lim3_action", "|u1"),
+            ("lim3_seq", "<u4"),
+            ("rec_nb", "|u1"),
+            ("rec1_type", "|u1"),
+            ("rec1_value", "<f4"),
+            ("rec1_value_unit", "|u1"),
+            ("rec2_type", "|u1"),
+            ("rec2_value", "<f4"),
+            ("rec2_value_unit", "|u1"),
+            ("rec3_type", "|u1"),
+            ("rec3_value", "<f4"),
+            ("rec3_value_unit", "|u1"),
+            ("E_range_min", "<f4"),
+            ("E_range_max", "<f4"),
+            ("I_range", "|u1"),
+            ("I_range_min", "|u1"),
+            ("I_range_max", "|u1"),
+            ("I_range_init", "|u1"),
+            ("auto_rest", "|u1"),
+            ("bandwidth", "|u1"),
+        ]
+    ),
+]
+
+
+# ~~~~~~~~~~~~~ Open Circuit Voltage ~~~~~~~~~~~~~
+def _ocv_params(settings: list[str]) -> list[str]:
+    """Constructs the parameter names for the OCV technique."""
+    params = ["tR", "dER/dt"]
+    record_match = re.search(r"^record.+", "\n".join(settings))
+    if record_match:
+        params += ["record"]
+    params += ["dER", "dtR", "E_range_min", "E_range_max"]
+    return params
+
+
+_ocv_params_dtypes = [
+    np.dtype(
+        [
+            ("tR", "<f4"),
+            ("dER/dt", "<f4"),
+            ("record", "|u1"),
+            ("dER", "<f4"),
+            ("dtR", "<f4"),
+            ("E_range_min", "<f4"),
+            ("E_range_max", "<f4"),
+        ]
+    ),
+    np.dtype(
+        [
+            ("tR", "<f4"),
+            ("dER/dt", "<f4"),
+            ("dER", "<f4"),
+            ("dtR", "<f4"),
+            ("E_range_min", "<f4"),
+            ("E_range_max", "<f4"),
+        ]
+    ),
+]
+
+
+# ~~~~~~~~~~~~~ Potentio Electrochemical Impedance Spectroscopy ~~~~~~~~~~~~~
+def _peis_params(settings: list[str]) -> list[str]:
+    """Constructs the parameter names for the PEIS technique."""
+    params = [
+        "sine_mode",
+        "E",
+        "E_vs",
+        "tE",
+        "record",
+        "dI",
+        "dI_unit",
+        "dt",
+        "fi",
+        "fi_unit",
+        "ff",
+        "ff_unit",
+        "Nd",
+        "points",
+        "spacing",
+        "Va",
+        "pw",
+        "Na",
+        "corr",
+    ]
+    params = _prepend_ns(settings, params)
+    lim_nb_match = re.search(r"^lim_nb\s+(?P<val>.+)", "\n".join(settings))
+    if lim_nb_match:
+        lim_nb = int(max(lim_nb_match["val"].split()))
+        params.append("lim_nb")
+        for i, __ in enumerate(range(lim_nb), 1):
+            limit = [
+                f"limit_type{i}",
+                f"limit_comp{i}",
+                f"limit_value{i}",
+                f"limit_unit{i}",
+            ]
+            params += limit
+    params += [
+        "E_range_min",
+        "E_range_max",
+        "I_range",
+        "bandwidth",
+        "nc_cycles",
+        "goto_Ns",
+        "nr_cycles",
+        "inc_cycle",
+    ]
+    return params
+
+
+_peis_params_dtypes = [
+    np.dtype(
+        [
+            ("sine_mode", "|u1"),
+            ("E", "<f4"),
+            ("E_vs", "|u1"),
+            ("tE", "<f4"),
+            ("record", "|u1"),
+            ("dI", "<f4"),
+            ("dI_unit", "|u1"),
+            ("dt", "<f4"),
+            ("fi", "<f4"),
+            ("fi_unit", "|u1"),
+            ("ff", "<f4"),
+            ("ff_unit", "|u1"),
+            ("Nd", "<u4"),
+            ("points", "|u1"),
+            ("spacing", "|u1"),
+            ("Va", "<f4"),
+            ("pw", "<f4"),
+            ("Na", "<u4"),
+            ("corr", "|u1"),
+            ("lim_nb", "|u1"),
+            ("limit_type1", "|u1"),
+            ("limit_comp1", "|u1"),
+            ("limit_value1", "<f4"),
+            ("limit_unit1", "|u1"),
+            ("limit_type2", "|u1"),
+            ("limit_comp2", "|u1"),
+            ("limit_value2", "<f4"),
+            ("limit_unit2", "|u1"),
+            ("limit_type3", "|u1"),
+            ("limit_comp3", "|u1"),
+            ("limit_value3", "<f4"),
+            ("limit_unit3", "|u1"),
+            ("limit_type4", "|u1"),
+            ("limit_comp4", "|u1"),
+            ("limit_value4", "<f4"),
+            ("limit_unit4", "|u1"),
+            ("limit_type5", "|u1"),
+            ("limit_comp5", "|u1"),
+            ("limit_value5", "<f4"),
+            ("limit_unit5", "|u1"),
+            ("limit_type6", "|u1"),
+            ("limit_comp6", "|u1"),
+            ("limit_value6", "<f4"),
+            ("limit_unit6", "|u1"),
+            ("E_range_min", "<f4"),
+            ("E_range_max", "<f4"),
+            ("I_range", "|u1"),
+            ("bandwidth", "|u1"),
+            ("nc_cycles", "<u4"),
+            ("goto_Ns", "<u4"),
+            ("nr_cycles", "<u4"),
+            ("inc_cycle", "<u4"),
+        ]
+    )
+]
+
+
+# ~~~~~~~~~~~~~ Wait ~~~~~~~~~~~~~
+def _wait_params(settings: list[str]) -> list[str]:
+    """Constructs the parameter names for the WAIT technique."""
+    params = [
+        "select",
+        "td",
+        "from",
+        "tech_num",
+        "ole_date",
+        "ole_time",
+        "record",
+        "dE",
+        "dI",
+        "dI_unit",
+        "dt",
+    ]
+    return params
+
+
+_wait_params_dtypes = [
+    np.dtype(
+        [
+            ("select", "|u1"),
+            ("td", "<u4"),
+            ("from", "|u1"),
+            ("tech_num", "|u1"),
+            ("ole_date", "<f4"),  # Why the hell would they split this?!
+            ("ole_time", "<f4"),
+            ("record", "|u1"),
+            ("dE", "<f4"),
+            ("dI", "<f4"),
+            ("dI_unit", "|u1"),
+            ("dt", "<f4"),
+        ]
+    )
+]
+
+
+# ~~~~~~~~~~~~~ IR compensation (PEIS) ~~~~~~~~~~~~~
+def _zir_params(settings: list[str]) -> list[str]:
+    """Constructs the parameter names for the ZIR technique."""
+    params = [
+        "E",
+        "E_vs",
+        "f",
+        "f_unit",
+        "Va",
+        "pw",
+        "Na",
+        "E_range_min",
+        "E_range_max",
+        "I_range",
+        "bandwidth",
+        "comp_level",
+        "use_results",
+        "comp_mode",
+    ]
+    return params
+
+
+_zir_params_dtypes = [
+    np.dtype(
+        [
+            ("E", "<f4"),
+            ("E_vs", "|u1"),
+            ("f", "<f4"),
+            ("f_unit", "|u1"),
+            ("Va", "<f4"),
+            ("pw", "<f4"),
+            ("Na", "<u4"),
+            ("E_range_min", "<f4"),
+            ("E_range_max", "<f4"),
+            ("I_range", "|u1"),
+            ("bandwidth", "|u1"),
+            ("comp_level", "|u1"),
+            ("use_results", "|u1"),
+            ("comp_mode", "|u1"),
+        ]
+    )
+]
+
+
+def technique_params(technique: str, settings: list[str]) -> tuple[str, list]:
+    """Constructs the parameter names for different techniques.
+
+    Parameters
+    ----------
+    technique
+        The full name of the technique.
+
+    settings
+        The list of settings from the start of an .mpt or .mps file.
+
+    Returns
+    -------
+    tuple[str, list]
+        The short technique name and a full list of technique parameter
+        names depending on what is present in the file.
+
+    """
+    if technique == "Chronoamperometry / Chronocoulometry":
+        return "CA", _ca_params(settings)
+    if technique == "Chronopotentiometry":
+        return "CP", _cp_params(settings)
+    if technique == "Cyclic Voltammetry":
+        return "CV", _cv_params(settings)
+    if technique == "Galvano Electrochemical Impedance Spectroscopy":
+        return "GEIS", _geis_params(settings)
+    if technique == "Galvanostatic Cycling with Potential Limitation":
+        return "GCPL", _gcpl_params(settings)
+    if technique == "IR compensation (PEIS)":
+        return "ZIR", _zir_params(settings)
+    if technique == "Linear Sweep Voltammetry":
+        return "LSV", _lsv_params(settings)
+    if technique == "Loop":
+        return "LOOP", _loop_params(settings)
+    if technique == "Modulo Bat":
+        return "mb", _mb_params(settings)
+    if technique == "Open Circuit Voltage":
+        return "OCV", _ocv_params(settings)
+    if technique == "Potentio Electrochemical Impedance Spectroscopy":
+        return "PEIS", _peis_params(settings)
+    if technique == "Wait":
+        return "WAIT", _wait_params(settings)
+    raise NotImplementedError(f"'{technique}' not implemented.")
+
+
+# Maps the technique byte to its corresponding dtype.
+technique_params_dtypes = {
+    0x04: ("GCPL", _gcpl_params_dtypes),
+    0x06: ("CV", _cv_params_dtypes),
+    0x0B: ("OCV", _ocv_params_dtypes),
+    0x18: ("CA", _ca_params_dtypes),
+    0x19: ("CP", _cp_params_dtypes),
+    0x1C: ("WAIT", _wait_params_dtypes),
+    0x1D: ("PEIS", _peis_params_dtypes),
+    0x1E: ("GEIS", _geis_params_dtype),
+    0x32: ("ZIR", _zir_params_dtypes),
+    0x6C: ("LSV", _lsv_params_dtype),
+    0x7F: ("MB", _mb_params_dtypes),
+}
+
+param_map = {
+    "I_range": (
+        ("1 A", 9, 1),
+        ("100 mA", 10, 1e-1),
+        ("10 mA", 11, 1e-2),
+        ("1 mA", 12, 1e-3),
+        ("100 µA", 13, 1e-4),
+        ("10 µA", 14, 1e-5),
+        ("1 µA", 15, 1e-6),
+        ("10 µA", 21, 1e-5),
+        ("1 µA", 22, 1e-6),
+        ("100 nA", 23, 1e-7),
+        ("10 nA", 24, 1e-8),
+        ("1 A", 37, 1),
+        ("100 mA", 38, 1e-1),
+        ("10 mA", 39, 1e-2),
+        ("1 mA", 40, 1e-3),
+        ("10 A", 65, 1e1),
+        ("Auto", None, None),
+    ),
+    "Is_unit": (
+        ("A", 0),  # guess
+        ("mA", 1),
+        ("µA", 2),
+        ("nA", 3),  # guess
+        ("pA", 4),  # guess
+    ),
+    "set_I/C": (
+        ("I", 0),
+        ("C", 1),  # guess
+    ),
+    "apply_I/C": (
+        ("I", 0),
+        ("C", 1),
+    ),
+}
+
+
+def param_from_key(
+    param: str, key: Union[int, str], to_str: bool = True
+) -> Union[str, float]:
+    """
+    Convert a supplied key of a certain parameter to its string or float value.
+
+    The function uses the map defined in ``param_map`` to convert between the
+    entries in the tuples, which contain the :class:`str` value of the parameter
+    (present in ``.mpt`` files), the :class:`int` value of the parameter (present
+    in ``.mpr`` files), and the corresponding :class:`float` value in SI units.
+
+    Parameters
+    ----------
+    param
+        The name of the parameter, a key within the ``param_map``. If ``param``
+        is not present in ``param_map``, the supplied key is returned back.
+
+    key
+        The key of the parameter that is to be converted to a different representation.
+
+    to_str
+        A switch between :class:`str` and :class:`float` output.
+
+    Returns
+    -------
+    key: Union[str, float, int]
+        The key converted to the requested format.
+
+    """
+    ii = 1 if isinstance(key, int) else 0
+    if param in param_map:
+        for i in param_map[param]:
+            if i[ii] == key:
+                if to_str:
+                    return i[0]
+                else:
+                    return i[2]
+        raise ValueError(f"element '{key}' for parameter '{param}' not understood.")
+    return key
+
+
+def get_resolution(
+    name: str, value: float, unit: str, Erange: float, Irange: float
+) -> float:
+    """
+    Function that returns the resolution of a property based on its name, value,
+    E-range and I-range.
+
+    The values used here are hard-coded from VMP-3 potentiostats. Generally, the
+    resolution is returned, however in some cases only the accuracy is specified
+    (currently ``freq`` and ``Phase``).
+
+    """
+    if name in {"control_V/I", "control_V_I"}:
+        raise RuntimeError("")
+    elif name in {"control_V"}:
+        # VMP-3: bisect function between 5 µV and 300 µV, as the
+        # voltage is stored in a 16-bit int.
+        if Erange >= 20.0:
+            return 305.18e-6
+        else:
+            res = [5e-6, 10e-6, 20e-6, 50e-6, 100e-6, 150e-6, 200e-6, 300e-6, 305.18e-6]
+            i = bisect.bisect_right(res, Erange / np.iinfo(np.uint16).max)
+            return res[i]
+    elif name in {"control_I"}:
+        # VMP-3: 0.004% of FSR, 760 µV at 10 µA I-range
+        return max(Irange * 0.004 / 100, 760e-12)
+    elif unit in {"V", "mV", "μV"}:
+        # VMP-3: 0.0015% of FSR, 75 µV minimum
+        return max(Erange * 0.0015 / 100, 75e-6)
+    elif unit in {"A", "mA", "µA", "nA", "pA"}:
+        # VMP-3: 0.004% of FSR
+        if Irange is None:
+            logger.warning("'I range' not specified. Using 1 A.")
+            Irange = 1.0
+        return Irange * 0.004 / 100
+    elif unit in {"Hz"}:
+        # VMP-3: using accuracy: 1% of value
+        return value * 0.01
+    elif unit in {"deg"}:
+        # VMP-3: using accuracy: 1 degree
+        return 1.0
+    elif unit in {"Ω", "S", "W"}:
+        # [Ω] = [V]/[A];
+        # [S] = [A]/[V];
+        # [W] = [A]*[V];
+        return max(
+            get_resolution("U", value, "V", Erange, Irange),
+            get_resolution("I", value, "A", Erange, Irange),
+        )
+    elif unit in {"C"}:
+        # [C] = [A]*[s];
+        return get_resolution("I", value, "A", Erange, Irange)
+    elif unit in {"mA·h"}:
+        return get_resolution("Q", value / 3.6, "C", Erange, Irange)
+    elif unit in {"W·h"}:
+        return get_resolution("P", value / 3600, "W", Erange, Irange)
+    elif unit in {"µF"}:
+        # [F] = [C]/[V]
+        return max(
+            get_resolution("Q", value * 1e-6, "C", Erange, Irange),
+            get_resolution("U", value * 1e-6, "V", Erange, Irange),
+        )
+    elif unit in {"s"}:
+        # Based on the EC-Lib documentation,
+        # 50 us is a safe upper limit for timebase
+        return 50e-6
+    elif unit in {"%"}:
+        return 0.1
+    else:
+        raise RuntimeError(
+            f"Could not get resolution of quantity '{name}' with unit '{unit}."
+        )
```

### Comparing `yadg-5.0.1/src/yadg/parsers/electrochem/eclabmpr.py` & `yadg-5.0.2/src/yadg/parsers/electrochem/eclabmpr.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,603 +1,603 @@
-"""
-**eclabmpr**: Processing of BioLogic's EC-Lab binary modular files.
--------------------------------------------------------------------
-
-``.mpr`` files are structured in a set of "modules", one concerning
-settings, one for actual data, one for logs, and an optional loops
-module. The parameter sequences can be found in the settings module.
-
-This code is partly an adaptation of the `galvani module by Chris
-Kerr <https://github.com/echemdata/galvani>`_, and builds on the work done
-by the previous civilian service member working on the project, Jonas Krieger.
-
-.. _yadg.parsers.electrochem.eclabmpr.techniques:
-
-These are the implemented techniques for which the technique parameter
-sequences can be parsed:
-
-+------+-------------------------------------------------+
-| CA   | Chronoamperometry / Chronocoulometry            |
-+------+-------------------------------------------------+
-| CP   | Chronopotentiometry                             |
-+------+-------------------------------------------------+
-| CV   | Cyclic Voltammetry                              |
-+------+-------------------------------------------------+
-| GCPL | Galvanostatic Cycling with Potential Limitation |
-+------+-------------------------------------------------+
-| GEIS | Galvano Electrochemical Impedance Spectroscopy  |
-+------+-------------------------------------------------+
-| LOOP | Loop                                            |
-+------+-------------------------------------------------+
-| LSV  | Linear Sweep Voltammetry                        |
-+------+-------------------------------------------------+
-| MB   | Modulo Bat                                      |
-+------+-------------------------------------------------+
-| OCV  | Open Circuit Voltage                            |
-+------+-------------------------------------------------+
-| PEIS | Potentio Electrochemical Impedance Spectroscopy |
-+------+-------------------------------------------------+
-| WAIT | Wait                                            |
-+------+-------------------------------------------------+
-| ZIR  | IR compensation (PEIS)                          |
-+------+-------------------------------------------------+
-
-.. note::
-
-    ``.mpt`` files can contain more data than the corresponding binary
-    ``.mpr`` file.
-
-File Structure of ``.mpr`` Files
-````````````````````````````````
-
-At a top level, ``.mpr`` files are made up of a number of modules,
-separated by the ``MODULE`` keyword. In all the files I have seen, the
-first module is the settings module, followed by the data module, the
-log module and then an optional loop module.
-
-.. code-block::
-
-    0x0000 BIO-LOGIC MODULAR FILE  # File magic.
-    0x0034 MODULE                  # Module magic.
-    ...                            # Module 1.
-    0x???? MODULE                  # Module magic.
-    ...                            # Module 2.
-    0x???? MODULE                  # Module magic.
-    ...                            # Module 3.
-    0x???? MODULE                  # Module magic.
-    ...                            # Module 4.
-
-After splitting the entire file on ``MODULE``, each module starts with a
-header that is structured like this (offsets from start of module):
-
-.. code-block::
-
-    0x0000 short_name  # Short name, e.g. VMP Set.
-    0x000A long_name   # Longer name, e.g. VMP settings.
-    0x0023 length      # Number of bytes in module data.
-    0x0027 version     # Module version.
-    0x002B date        # Acquisition date in ASCII, e.g. 08/10/21.
-    ...                # Module data.
-
-The contents of each module's data vary wildly depending on the used
-technique, the module and perhaps the software version, the settings in
-EC-Lab, etc. Here a quick overview (offsets from start of module data).
-
-*Settings Module*
-
-.. code-block::
-
-    0x0000 technique_id           # Unique technique ID.
-    ...                           # ???
-    0x0007 comments               # Pascal string.
-    ...                           # Zero padding.
-    # Cell Characteristics.
-    0x0107 active_material_mass   # Mass of active material
-    0x010B at_x                   # at x =
-    0x010F molecular_weight       # Molecular weight of active material
-    0x0113 atomic_weight          # Atomic weight of intercalated ion
-    0x0117 acquisition_start      # Acquisition started a: xo =
-    0x011B e_transferred          # Number of e- transferred
-    0x011E electrode_material     # Pascal string.
-    ...                           # Zero Padding
-    0x01C0 electrolyte            # Pascal string.
-    ...                           # Zero Padding, ???.
-    0x0211 electrode_area         # Electrode surface area
-    0x0215 reference_electrode    # Pascal string
-    ...                           # Zero padding
-    0x024C characteristic_mass    # Characteristic mass
-    ...                           # ???
-    0x025C battery_capacity       # Battery capacity C =
-    0x0260 battery_capacity_unit  # Unit of the battery capacity.
-    ...                           # ???
-    # Technique parameters can randomly be found at 0x0572, 0x1845 or
-    # 0x1846. All you can do is guess and try until it fits.
-    0x1845 ns                     # Number of sequences.
-    0x1847 n_params               # Number of technique parameters.
-    0x1849 params                 # ns sets of n_params parameters.
-    ...                           # ???
-
-*Data Module*
-
-.. code-block::
-
-    0x0000 n_datapoints  # Number of datapoints.
-    0x0004 n_columns     # Number of values per datapoint.
-    0x0005 column_ids    # n_columns unique column IDs.
-    ...
-    # Depending on module version, datapoints start 0x0195 or 0x0196.
-    # Length of each datapoint depends on number and IDs of columns.
-    0x0195 datapoints    # n_datapoints points of data.
-
-*Log Module*
-
-.. code-block::
-
-    ...                         # ???
-    0x0009 channel_number       # Zero-based channel number.
-    ...                         # ???
-    0x00AB channel_sn           # Channel serial number.
-    ...                         # ???
-    0x01F8 Ewe_ctrl_min         # Ewe ctrl range min.
-    0x01FC Ewe_ctrl_max         # Ewe ctrl range max.
-    ...                         # ???
-    0x0249 ole_timestamp        # Timestamp in OLE format.
-    0x0251 filename             # Pascal String.
-    ...                         # Zero padding, ???.
-    0x0351 host                 # IP address of host, Pascal string.
-    ...                         # Zero padding.
-    0x0384 address              # IP address / COM port of potentiostat.
-    ...                         # Zero padding.
-    0x03B7 ec_lab_version       # EC-Lab version (software)
-    ...                         # Zero padding.
-    0x03BE server_version       # Internet server version (firmware)
-    ...                         # Zero padding.
-    0x03C5 interpreter_version  # Command interpretor version (firmware)
-    ...                         # Zero padding.
-    0x03CF device_sn            # Device serial number.
-    ...                         # Zero padding.
-    0x0922 averaging_points     # Smooth data on ... points.
-    ...                         # ???
-
-*Loop Module*
-
-.. code-block::
-
-    0x0000 n_indexes  # Number of loop indexes.
-    0x0004 indexes    # n_indexes indexes at which loops start in data.
-    ...               # ???
-
-
-Metadata
-````````
-The metadata will contain the information from the *Settings module*. This should
-include information about the technique, as well as any explicitly parsed cell
-characteristics data specified in EC-Lab.
-
-.. admonition:: TODO
-
-    https://github.com/dgbowl/yadg/issues/12
-
-    The mapping between metadata parameters between ``.mpr`` and ``.mpt`` files
-    is not yet complete. In ``.mpr`` files, some technique parameters in the settings
-    module correspond to entries in drop-down lists in EC-Lab. These values are
-    stored as single-byte values in ``.mpr`` files.
-
-The metadata also contains the infromation from the *Log module*, which contains
-more general parameters, like software, firmware and server versions, channel number,
-host address and an acquisition start timestamp in Microsoft OLE format.
-
-.. note::
-
-    If the ``.mpr`` file contains an ``ExtDev`` module (containing parameters
-    of any external sensors plugged into the device), the ``log`` is usually
-    not present and therefore the full timestamp cannot be calculated.
-
-.. codeauthor:: Nicolas Vetsch
-"""
-import logging
-from zoneinfo import ZoneInfo
-import xarray as xr
-import numpy as np
-from ...dgutils.dateutils import ole_to_uts
-from ...dgutils.btools import read_value
-from .eclabcommon.techniques import (
-    technique_params_dtypes,
-    param_from_key,
-    get_resolution,
-)
-from .eclabcommon.mpr_columns import (
-    module_header_dtype,
-    settings_dtypes,
-    flag_columns,
-    data_columns,
-    log_dtypes,
-    extdev_dtypes,
-)
-from yadg.parsers.basiccsv.main import append_dicts, dicts_to_dataset
-
-logger = logging.getLogger(__name__)
-
-
-def process_settings(data: bytes) -> tuple[dict, list]:
-    """Processes the contents of settings modules.
-
-    Parameters
-    ----------
-    data
-        The data to parse through.
-
-    Returns
-    -------
-    dict
-        The parsed settings.
-
-    """
-    settings = {}
-    # First parse the settings right at the top of the data block.
-    technique, params_dtypes = technique_params_dtypes[data[0x0000]]
-    settings["technique"] = technique
-    for offset, (dtype, name) in settings_dtypes.items():
-        settings[name] = read_value(data, offset, dtype)
-    # Then determine the technique parameters. The parameters' offset
-    # changes depending on the technique present and apparently on some
-    # other factor that is unclear to me.
-    params_offset = None
-    for offset in (0x0572, 0x1845, 0x1846):
-        logger.debug("Trying to find the technique parameters at 0x%x.", offset)
-        n_params = read_value(data, offset + 0x0002, "<u2")
-        for dtype in params_dtypes:
-            if len(dtype) == n_params:
-                params_dtype, params_offset = dtype, offset
-                logger.debug("Determined %d parameters at 0x%x.", n_params, offset)
-                break
-        if params_offset is not None:
-            break
-    if params_offset is None:
-        raise NotImplementedError("Unknown parameter offset or technique dtype.")
-    logger.debug("Reading number of parameter sequences at 0x%x.", params_offset)
-    ns = read_value(data, params_offset, "<u2")
-    logger.debug("Reading %d parameter sequences of %d parameters.", ns, n_params)
-    rawparams = np.frombuffer(
-        data,
-        offset=params_offset + 0x0004,
-        dtype=params_dtype,
-        count=ns,
-    )
-    pardicts = [dict(zip(value.dtype.names, value.item())) for value in rawparams]
-    params = []
-    for pardict in pardicts:
-        for k, v in pardict.items():
-            # MPR quirk: I_range off by one
-            if k == "I_range":
-                v += 1
-            pardict[k] = param_from_key(k, v, to_str=True)
-            # Handle NaNs and +/-Inf in params here
-            if np.isnan(v) or np.isinf(v):
-                pardict[k] = str(v)
-        params.append(pardict)
-    return settings, params
-
-
-def parse_columns(column_ids: list[int]) -> tuple[list, list, list, dict]:
-    """Puts together column info from a list of data column IDs.
-
-    Note
-    ----
-    The binary layout of the data in the `.mpr` file is described by a
-    sequence of column IDs. Some column IDs relate to (flags) which are
-    all packed into a single byte.
-
-    Parameters
-    ----------
-    column_ids
-        A list of column IDs.
-
-    Returns
-    -------
-    tuple[list, list, list, dict]
-        The column names, dtypes, units and a dictionary of flag names
-        and bitmasks.
-
-    """
-    names = []
-    dtypes = []
-    units = []
-    flags = {}
-    for id in column_ids:
-        if id in flag_columns:
-            bitmask, name = flag_columns[id]
-            flags[name] = bitmask
-            # Flags column only needs to be added once.
-            if "flags" not in names:
-                names.append("flags")
-                dtypes.append("|u1")
-                units.append(None)
-        elif id in data_columns:
-            dtype, name, unit = data_columns[id]
-            names.append(name)
-            dtypes.append(dtype)
-            units.append(unit)
-        else:
-            name = f"unknown_{len(names)}"
-            logger.warning("Unknown column ID '%d' was assigned into '%s'.", id, name)
-            names.append(name)
-            dtypes.append("<f4")
-            units.append("")
-    return names, dtypes, units, flags
-
-
-def process_data(
-    data: bytes,
-    version: int,
-    Eranges: list[float],
-    Iranges: list[float],
-    controls: list[str],
-):
-    """Processes the contents of data modules.
-
-    Parameters
-    ----------
-    data
-        The data to parse through.
-
-    version
-        Module version from the data module header.
-
-    Returns
-    -------
-    list[dict]
-        Processed data ([{column -> value}, ..., {column -> value}]). If
-        the column unit is set to None, the value is an int. Otherwise,
-        the value is a dict with value ("n"), sigma ("s"), and unit
-        ("u").
-
-    """
-    n_datapoints = read_value(data, 0x0000, "<u4")
-    n_columns = read_value(data, 0x0004, "|u1")
-    column_ids = np.frombuffer(data, offset=0x005, dtype="<u2", count=n_columns)
-    # Length of each datapoint depends on number and IDs of columns.
-    namelist, dtypelist, unitlist, flaglist = parse_columns(column_ids)
-    units = {k: v for k, v in zip(namelist, unitlist) if v is not None}
-    data_dtype = np.dtype(list(zip(namelist, dtypelist)))
-    # Depending on module version, datapoints start at 0x0195 or 0x0196.
-    if version == 2:
-        offset = 0x0195
-    elif version == 3:
-        offset = 0x0196
-    else:
-        raise NotImplementedError(f"Unknown data module version: {version}")
-    allvals = dict()
-    allmeta = dict()
-    values = np.frombuffer(data, offset=offset, dtype=data_dtype, count=n_datapoints)
-    values = [dict(zip(value.dtype.names, value.item())) for value in values]
-    for vi, vals in enumerate(values):
-        # Lets split this into two loops: get the indices first, then the data
-        for (name, value), unit in list(zip(vals.items(), unitlist)):
-            if unit is None:
-                intv = int(value)
-                if name == "I Range":
-                    vals[name] = param_from_key("I_range", intv)
-                else:
-                    vals[name] = intv
-        if flaglist:
-            # logger.debug("Extracting flag values.")
-            flag_bits = vals.pop("flags")
-            for name, bitmask in flaglist.items():
-                # Two's complement hack to find the position of the
-                # rightmost set bit.
-                shift = (bitmask & -bitmask).bit_length() - 1
-                # Rightshift flag by that amount.
-                vals[name] = (flag_bits & bitmask) >> shift
-
-        if "Ns" in vals:
-            Erange = Eranges[vals["Ns"]]
-            Irstr = Iranges[vals["Ns"]]
-        else:
-            Erange = Eranges[0]
-            Irstr = Iranges[0]
-        if "I Range" in vals:
-            Irstr = vals["I Range"]
-        Irange = param_from_key("I_range", Irstr, to_str=False)
-        devs = {}
-        if "control_V_I" in vals:
-            icv = controls[vals["Ns"]]
-            name = f"control_{icv}"
-            vals[name] = vals.pop("control_V_I")
-            units[name] = "mA" if icv in {"I", "C"} else "V"
-        for name, value in vals.items():
-            unit = units.get(name)
-            if unit is None:
-                continue
-            devs[name] = get_resolution(name, value, unit, Erange, Irange)
-
-        append_dicts(vals, devs, allvals, allmeta, li=vi)
-
-    ds = dicts_to_dataset(allvals, allmeta, units, fulldate=False)
-    return ds
-
-
-def process_log(data: bytes) -> dict:
-    """Processes the contents of log modules.
-
-    Parameters
-    ----------
-    data
-        The data to parse through.
-
-    Returns
-    -------
-    dict
-        The parsed log.
-
-    """
-    log = {}
-    for offset, (dtype, name) in log_dtypes.items():
-        log[name] = read_value(data, offset, dtype)
-    return log
-
-
-def process_loop(data: bytes) -> dict:
-    """Processes the contents of loop modules.
-
-    Parameters
-    ----------
-    data
-        The data to parse through.
-
-    Returns
-    -------
-    dict
-        The parsed loops.
-
-    """
-    n_indexes = read_value(data, 0x0000, "<u4")
-    indexes = np.frombuffer(data, offset=0x0004, dtype="<u4", count=n_indexes)
-    return {"n_indexes": n_indexes, "indexes": indexes}
-
-
-def process_ext(data: bytes) -> dict:
-    """Processes the contents of external device modules.
-
-    Parameters
-    ----------
-    data
-        The data to parse through.
-
-    Returns
-    -------
-    dict
-        The parsed log.
-
-    """
-    ext = {}
-    for offset, (dtype, name) in extdev_dtypes.items():
-        ext[name] = read_value(data, offset, dtype)
-
-    return ext
-
-
-def process_modules(contents: bytes) -> tuple[dict, list, list, dict, dict]:
-    """Handles the processing of all modules.
-
-    Parameters
-    ----------
-    contents
-        The contents of an .mpr file, minus the file magic.
-
-    Returns
-    -------
-    tuple[dict, list, dict, dict]
-        The processed settings, data, log, and loop modules. If they are
-        not present in the provided modules, returns None instead.
-
-    """
-    modules = contents.split(b"MODULE")[1:]
-    settings = log = loop = ext = None
-    for module in modules:
-        header = read_value(module, 0x0000, module_header_dtype)
-        name = header["short_name"].strip()
-        logger.debug("Read '%s' module.", name)
-        module_data = module[module_header_dtype.itemsize :]
-        if name == "VMP Set":
-            settings, params = process_settings(module_data)
-            Eranges = []
-            Iranges = []
-            ctrls = []
-            for el in params:
-                E_range_max = el.get("E_range_max", float("inf"))
-                E_range_min = el.get("E_range_min", float("-inf"))
-                Eranges.append(E_range_max - E_range_min)
-                Iranges.append(el.get("I_range", "Auto"))
-                if "set_I/C" in el:
-                    ctrls.append(el["set_I/C"])
-                elif "apply_I/C" in el:
-                    ctrls.append(el["apply_I/C"])
-                else:
-                    ctrls.append(None)
-        elif name == "VMP data":
-            ds = process_data(module_data, header["version"], Eranges, Iranges, ctrls)
-        elif name == "VMP LOG":
-            log = process_log(module_data)
-        elif name == "VMP loop":
-            loop = process_loop(module_data)
-        elif name == "VMP ExtDev":
-            ext = process_ext(module_data)
-        else:
-            raise NotImplementedError(f"Unknown module: {name}.")
-    if ext is not None:
-        # replace names, units, and correct sigmas in data with headers present in ext
-        for k in {"Analog IN 1", "Analog IN 2"}:
-            parts = ext[k].split("/")
-            if len(parts) == 1:
-                n = parts[0]
-                u = " "
-            else:
-                n, u = parts
-            if k in ds:
-                ds[n] = ds[k]
-                ds[n].attrs = {"units": u, "ancillary_variables": f"{n}_std_err"}
-                del ds[k]
-                devs = ds[f"{k}_std_err"]
-                fac = ext[k + " max x"] - ext[k + " min x"]
-                fac = fac / (ext[k + " max V"] - ext[k + " min V"])
-                ds[f"{n}_std_err"] = devs * fac
-                ds[f"{n}_std_err"].attrs = {
-                    "units": u,
-                    "standard_name": f"{n} standard_error",
-                }
-                del ds[f"{k}_std_err"]
-        settings.update(ext)
-    return settings, params, ds, log, loop
-
-
-def process(
-    *,
-    fn: str,
-    timezone: ZoneInfo,
-    **kwargs: dict,
-) -> xr.Dataset:
-    """Processes EC-Lab raw data binary files.
-
-    Parameters
-    ----------
-    fn
-        The file containing the data to parse.
-
-    encoding
-        Encoding of ``fn``, by default "windows-1252".
-
-    timezone
-        A string description of the timezone. Default is "localtime".
-
-    Returns
-    -------
-    :class:`xarray.Dataset`
-        The full date is specified only if the "LOG" module is present.
-
-    """
-    file_magic = b"BIO-LOGIC MODULAR FILE\x1a                         \x00\x00\x00\x00"
-    with open(fn, "rb") as mpr_file:
-        assert mpr_file.read(len(file_magic)) == file_magic, "invalid file magic"
-        mpr = mpr_file.read()
-    settings, params, ds, log, loop = process_modules(mpr)
-    assert settings is not None, "no settings module"
-    assert ds is not None, "no data module"
-    # Arrange all the data into the correct format.
-    # TODO: Metadata could be handled in a nicer way.
-    metadata = {"settings": settings, "params": params}
-    if log is None:
-        logger.warning("No 'log' module present in mpr file. Timestamps incomplete.")
-        start_time = 0
-        fulldate = False
-    else:
-        metadata["log"] = log
-        start_time = ole_to_uts(log["ole_timestamp"], timezone=timezone)
-        fulldate = True
-    if "time" in ds:
-        ds["uts"] = ds["time"] + start_time
-    else:
-        ds["uts"] = [start_time]
-    if fulldate:
-        del ds.attrs["fulldate"]
-    ds.attrs.update(metadata)
-    return ds
+"""
+**eclabmpr**: Processing of BioLogic's EC-Lab binary modular files.
+-------------------------------------------------------------------
+
+``.mpr`` files are structured in a set of "modules", one concerning
+settings, one for actual data, one for logs, and an optional loops
+module. The parameter sequences can be found in the settings module.
+
+This code is partly an adaptation of the `galvani module by Chris
+Kerr <https://github.com/echemdata/galvani>`_, and builds on the work done
+by the previous civilian service member working on the project, Jonas Krieger.
+
+.. _yadg.parsers.electrochem.eclabmpr.techniques:
+
+These are the implemented techniques for which the technique parameter
+sequences can be parsed:
+
++------+-------------------------------------------------+
+| CA   | Chronoamperometry / Chronocoulometry            |
++------+-------------------------------------------------+
+| CP   | Chronopotentiometry                             |
++------+-------------------------------------------------+
+| CV   | Cyclic Voltammetry                              |
++------+-------------------------------------------------+
+| GCPL | Galvanostatic Cycling with Potential Limitation |
++------+-------------------------------------------------+
+| GEIS | Galvano Electrochemical Impedance Spectroscopy  |
++------+-------------------------------------------------+
+| LOOP | Loop                                            |
++------+-------------------------------------------------+
+| LSV  | Linear Sweep Voltammetry                        |
++------+-------------------------------------------------+
+| MB   | Modulo Bat                                      |
++------+-------------------------------------------------+
+| OCV  | Open Circuit Voltage                            |
++------+-------------------------------------------------+
+| PEIS | Potentio Electrochemical Impedance Spectroscopy |
++------+-------------------------------------------------+
+| WAIT | Wait                                            |
++------+-------------------------------------------------+
+| ZIR  | IR compensation (PEIS)                          |
++------+-------------------------------------------------+
+
+.. note::
+
+    ``.mpt`` files can contain more data than the corresponding binary
+    ``.mpr`` file.
+
+File Structure of ``.mpr`` Files
+````````````````````````````````
+
+At a top level, ``.mpr`` files are made up of a number of modules,
+separated by the ``MODULE`` keyword. In all the files I have seen, the
+first module is the settings module, followed by the data module, the
+log module and then an optional loop module.
+
+.. code-block::
+
+    0x0000 BIO-LOGIC MODULAR FILE  # File magic.
+    0x0034 MODULE                  # Module magic.
+    ...                            # Module 1.
+    0x???? MODULE                  # Module magic.
+    ...                            # Module 2.
+    0x???? MODULE                  # Module magic.
+    ...                            # Module 3.
+    0x???? MODULE                  # Module magic.
+    ...                            # Module 4.
+
+After splitting the entire file on ``MODULE``, each module starts with a
+header that is structured like this (offsets from start of module):
+
+.. code-block::
+
+    0x0000 short_name  # Short name, e.g. VMP Set.
+    0x000A long_name   # Longer name, e.g. VMP settings.
+    0x0023 length      # Number of bytes in module data.
+    0x0027 version     # Module version.
+    0x002B date        # Acquisition date in ASCII, e.g. 08/10/21.
+    ...                # Module data.
+
+The contents of each module's data vary wildly depending on the used
+technique, the module and perhaps the software version, the settings in
+EC-Lab, etc. Here a quick overview (offsets from start of module data).
+
+*Settings Module*
+
+.. code-block::
+
+    0x0000 technique_id           # Unique technique ID.
+    ...                           # ???
+    0x0007 comments               # Pascal string.
+    ...                           # Zero padding.
+    # Cell Characteristics.
+    0x0107 active_material_mass   # Mass of active material
+    0x010B at_x                   # at x =
+    0x010F molecular_weight       # Molecular weight of active material
+    0x0113 atomic_weight          # Atomic weight of intercalated ion
+    0x0117 acquisition_start      # Acquisition started a: xo =
+    0x011B e_transferred          # Number of e- transferred
+    0x011E electrode_material     # Pascal string.
+    ...                           # Zero Padding
+    0x01C0 electrolyte            # Pascal string.
+    ...                           # Zero Padding, ???.
+    0x0211 electrode_area         # Electrode surface area
+    0x0215 reference_electrode    # Pascal string
+    ...                           # Zero padding
+    0x024C characteristic_mass    # Characteristic mass
+    ...                           # ???
+    0x025C battery_capacity       # Battery capacity C =
+    0x0260 battery_capacity_unit  # Unit of the battery capacity.
+    ...                           # ???
+    # Technique parameters can randomly be found at 0x0572, 0x1845 or
+    # 0x1846. All you can do is guess and try until it fits.
+    0x1845 ns                     # Number of sequences.
+    0x1847 n_params               # Number of technique parameters.
+    0x1849 params                 # ns sets of n_params parameters.
+    ...                           # ???
+
+*Data Module*
+
+.. code-block::
+
+    0x0000 n_datapoints  # Number of datapoints.
+    0x0004 n_columns     # Number of values per datapoint.
+    0x0005 column_ids    # n_columns unique column IDs.
+    ...
+    # Depending on module version, datapoints start 0x0195 or 0x0196.
+    # Length of each datapoint depends on number and IDs of columns.
+    0x0195 datapoints    # n_datapoints points of data.
+
+*Log Module*
+
+.. code-block::
+
+    ...                         # ???
+    0x0009 channel_number       # Zero-based channel number.
+    ...                         # ???
+    0x00AB channel_sn           # Channel serial number.
+    ...                         # ???
+    0x01F8 Ewe_ctrl_min         # Ewe ctrl range min.
+    0x01FC Ewe_ctrl_max         # Ewe ctrl range max.
+    ...                         # ???
+    0x0249 ole_timestamp        # Timestamp in OLE format.
+    0x0251 filename             # Pascal String.
+    ...                         # Zero padding, ???.
+    0x0351 host                 # IP address of host, Pascal string.
+    ...                         # Zero padding.
+    0x0384 address              # IP address / COM port of potentiostat.
+    ...                         # Zero padding.
+    0x03B7 ec_lab_version       # EC-Lab version (software)
+    ...                         # Zero padding.
+    0x03BE server_version       # Internet server version (firmware)
+    ...                         # Zero padding.
+    0x03C5 interpreter_version  # Command interpretor version (firmware)
+    ...                         # Zero padding.
+    0x03CF device_sn            # Device serial number.
+    ...                         # Zero padding.
+    0x0922 averaging_points     # Smooth data on ... points.
+    ...                         # ???
+
+*Loop Module*
+
+.. code-block::
+
+    0x0000 n_indexes  # Number of loop indexes.
+    0x0004 indexes    # n_indexes indexes at which loops start in data.
+    ...               # ???
+
+
+Metadata
+````````
+The metadata will contain the information from the *Settings module*. This should
+include information about the technique, as well as any explicitly parsed cell
+characteristics data specified in EC-Lab.
+
+.. admonition:: TODO
+
+    https://github.com/dgbowl/yadg/issues/12
+
+    The mapping between metadata parameters between ``.mpr`` and ``.mpt`` files
+    is not yet complete. In ``.mpr`` files, some technique parameters in the settings
+    module correspond to entries in drop-down lists in EC-Lab. These values are
+    stored as single-byte values in ``.mpr`` files.
+
+The metadata also contains the infromation from the *Log module*, which contains
+more general parameters, like software, firmware and server versions, channel number,
+host address and an acquisition start timestamp in Microsoft OLE format.
+
+.. note::
+
+    If the ``.mpr`` file contains an ``ExtDev`` module (containing parameters
+    of any external sensors plugged into the device), the ``log`` is usually
+    not present and therefore the full timestamp cannot be calculated.
+
+.. codeauthor:: Nicolas Vetsch
+"""
+import logging
+from zoneinfo import ZoneInfo
+import xarray as xr
+import numpy as np
+from ...dgutils.dateutils import ole_to_uts
+from ...dgutils.btools import read_value
+from .eclabcommon.techniques import (
+    technique_params_dtypes,
+    param_from_key,
+    get_resolution,
+)
+from .eclabcommon.mpr_columns import (
+    module_header_dtype,
+    settings_dtypes,
+    flag_columns,
+    data_columns,
+    log_dtypes,
+    extdev_dtypes,
+)
+from yadg.parsers.basiccsv.main import append_dicts, dicts_to_dataset
+
+logger = logging.getLogger(__name__)
+
+
+def process_settings(data: bytes) -> tuple[dict, list]:
+    """Processes the contents of settings modules.
+
+    Parameters
+    ----------
+    data
+        The data to parse through.
+
+    Returns
+    -------
+    dict
+        The parsed settings.
+
+    """
+    settings = {}
+    # First parse the settings right at the top of the data block.
+    technique, params_dtypes = technique_params_dtypes[data[0x0000]]
+    settings["technique"] = technique
+    for offset, (dtype, name) in settings_dtypes.items():
+        settings[name] = read_value(data, offset, dtype)
+    # Then determine the technique parameters. The parameters' offset
+    # changes depending on the technique present and apparently on some
+    # other factor that is unclear to me.
+    params_offset = None
+    for offset in (0x0572, 0x1845, 0x1846):
+        logger.debug("Trying to find the technique parameters at 0x%x.", offset)
+        n_params = read_value(data, offset + 0x0002, "<u2")
+        for dtype in params_dtypes:
+            if len(dtype) == n_params:
+                params_dtype, params_offset = dtype, offset
+                logger.debug("Determined %d parameters at 0x%x.", n_params, offset)
+                break
+        if params_offset is not None:
+            break
+    if params_offset is None:
+        raise NotImplementedError("Unknown parameter offset or technique dtype.")
+    logger.debug("Reading number of parameter sequences at 0x%x.", params_offset)
+    ns = read_value(data, params_offset, "<u2")
+    logger.debug("Reading %d parameter sequences of %d parameters.", ns, n_params)
+    rawparams = np.frombuffer(
+        data,
+        offset=params_offset + 0x0004,
+        dtype=params_dtype,
+        count=ns,
+    )
+    pardicts = [dict(zip(value.dtype.names, value.item())) for value in rawparams]
+    params = []
+    for pardict in pardicts:
+        for k, v in pardict.items():
+            # MPR quirk: I_range off by one
+            if k == "I_range":
+                v += 1
+            pardict[k] = param_from_key(k, v, to_str=True)
+            # Handle NaNs and +/-Inf in params here
+            if np.isnan(v) or np.isinf(v):
+                pardict[k] = str(v)
+        params.append(pardict)
+    return settings, params
+
+
+def parse_columns(column_ids: list[int]) -> tuple[list, list, list, dict]:
+    """Puts together column info from a list of data column IDs.
+
+    Note
+    ----
+    The binary layout of the data in the `.mpr` file is described by a
+    sequence of column IDs. Some column IDs relate to (flags) which are
+    all packed into a single byte.
+
+    Parameters
+    ----------
+    column_ids
+        A list of column IDs.
+
+    Returns
+    -------
+    tuple[list, list, list, dict]
+        The column names, dtypes, units and a dictionary of flag names
+        and bitmasks.
+
+    """
+    names = []
+    dtypes = []
+    units = []
+    flags = {}
+    for id in column_ids:
+        if id in flag_columns:
+            bitmask, name = flag_columns[id]
+            flags[name] = bitmask
+            # Flags column only needs to be added once.
+            if "flags" not in names:
+                names.append("flags")
+                dtypes.append("|u1")
+                units.append(None)
+        elif id in data_columns:
+            dtype, name, unit = data_columns[id]
+            names.append(name)
+            dtypes.append(dtype)
+            units.append(unit)
+        else:
+            name = f"unknown_{len(names)}"
+            logger.warning("Unknown column ID '%d' was assigned into '%s'.", id, name)
+            names.append(name)
+            dtypes.append("<f4")
+            units.append("")
+    return names, dtypes, units, flags
+
+
+def process_data(
+    data: bytes,
+    version: int,
+    Eranges: list[float],
+    Iranges: list[float],
+    controls: list[str],
+):
+    """Processes the contents of data modules.
+
+    Parameters
+    ----------
+    data
+        The data to parse through.
+
+    version
+        Module version from the data module header.
+
+    Returns
+    -------
+    list[dict]
+        Processed data ([{column -> value}, ..., {column -> value}]). If
+        the column unit is set to None, the value is an int. Otherwise,
+        the value is a dict with value ("n"), sigma ("s"), and unit
+        ("u").
+
+    """
+    n_datapoints = read_value(data, 0x0000, "<u4")
+    n_columns = read_value(data, 0x0004, "|u1")
+    column_ids = np.frombuffer(data, offset=0x005, dtype="<u2", count=n_columns)
+    # Length of each datapoint depends on number and IDs of columns.
+    namelist, dtypelist, unitlist, flaglist = parse_columns(column_ids)
+    units = {k: v for k, v in zip(namelist, unitlist) if v is not None}
+    data_dtype = np.dtype(list(zip(namelist, dtypelist)))
+    # Depending on module version, datapoints start at 0x0195 or 0x0196.
+    if version == 2:
+        offset = 0x0195
+    elif version == 3:
+        offset = 0x0196
+    else:
+        raise NotImplementedError(f"Unknown data module version: {version}")
+    allvals = dict()
+    allmeta = dict()
+    values = np.frombuffer(data, offset=offset, dtype=data_dtype, count=n_datapoints)
+    values = [dict(zip(value.dtype.names, value.item())) for value in values]
+    for vi, vals in enumerate(values):
+        # Lets split this into two loops: get the indices first, then the data
+        for (name, value), unit in list(zip(vals.items(), unitlist)):
+            if unit is None:
+                intv = int(value)
+                if name == "I Range":
+                    vals[name] = param_from_key("I_range", intv)
+                else:
+                    vals[name] = intv
+        if flaglist:
+            # logger.debug("Extracting flag values.")
+            flag_bits = vals.pop("flags")
+            for name, bitmask in flaglist.items():
+                # Two's complement hack to find the position of the
+                # rightmost set bit.
+                shift = (bitmask & -bitmask).bit_length() - 1
+                # Rightshift flag by that amount.
+                vals[name] = (flag_bits & bitmask) >> shift
+
+        if "Ns" in vals:
+            Erange = Eranges[vals["Ns"]]
+            Irstr = Iranges[vals["Ns"]]
+        else:
+            Erange = Eranges[0]
+            Irstr = Iranges[0]
+        if "I Range" in vals:
+            Irstr = vals["I Range"]
+        Irange = param_from_key("I_range", Irstr, to_str=False)
+        devs = {}
+        if "control_V_I" in vals:
+            icv = controls[vals["Ns"]]
+            name = f"control_{icv}"
+            vals[name] = vals.pop("control_V_I")
+            units[name] = "mA" if icv in {"I", "C"} else "V"
+        for name, value in vals.items():
+            unit = units.get(name)
+            if unit is None:
+                continue
+            devs[name] = get_resolution(name, value, unit, Erange, Irange)
+
+        append_dicts(vals, devs, allvals, allmeta, li=vi)
+
+    ds = dicts_to_dataset(allvals, allmeta, units, fulldate=False)
+    return ds
+
+
+def process_log(data: bytes) -> dict:
+    """Processes the contents of log modules.
+
+    Parameters
+    ----------
+    data
+        The data to parse through.
+
+    Returns
+    -------
+    dict
+        The parsed log.
+
+    """
+    log = {}
+    for offset, (dtype, name) in log_dtypes.items():
+        log[name] = read_value(data, offset, dtype)
+    return log
+
+
+def process_loop(data: bytes) -> dict:
+    """Processes the contents of loop modules.
+
+    Parameters
+    ----------
+    data
+        The data to parse through.
+
+    Returns
+    -------
+    dict
+        The parsed loops.
+
+    """
+    n_indexes = read_value(data, 0x0000, "<u4")
+    indexes = np.frombuffer(data, offset=0x0004, dtype="<u4", count=n_indexes)
+    return {"n_indexes": n_indexes, "indexes": indexes}
+
+
+def process_ext(data: bytes) -> dict:
+    """Processes the contents of external device modules.
+
+    Parameters
+    ----------
+    data
+        The data to parse through.
+
+    Returns
+    -------
+    dict
+        The parsed log.
+
+    """
+    ext = {}
+    for offset, (dtype, name) in extdev_dtypes.items():
+        ext[name] = read_value(data, offset, dtype)
+
+    return ext
+
+
+def process_modules(contents: bytes) -> tuple[dict, list, list, dict, dict]:
+    """Handles the processing of all modules.
+
+    Parameters
+    ----------
+    contents
+        The contents of an .mpr file, minus the file magic.
+
+    Returns
+    -------
+    tuple[dict, list, dict, dict]
+        The processed settings, data, log, and loop modules. If they are
+        not present in the provided modules, returns None instead.
+
+    """
+    modules = contents.split(b"MODULE")[1:]
+    settings = log = loop = ext = None
+    for module in modules:
+        header = read_value(module, 0x0000, module_header_dtype)
+        name = header["short_name"].strip()
+        logger.debug("Read '%s' module.", name)
+        module_data = module[module_header_dtype.itemsize :]
+        if name == "VMP Set":
+            settings, params = process_settings(module_data)
+            Eranges = []
+            Iranges = []
+            ctrls = []
+            for el in params:
+                E_range_max = el.get("E_range_max", float("inf"))
+                E_range_min = el.get("E_range_min", float("-inf"))
+                Eranges.append(E_range_max - E_range_min)
+                Iranges.append(el.get("I_range", "Auto"))
+                if "set_I/C" in el:
+                    ctrls.append(el["set_I/C"])
+                elif "apply_I/C" in el:
+                    ctrls.append(el["apply_I/C"])
+                else:
+                    ctrls.append(None)
+        elif name == "VMP data":
+            ds = process_data(module_data, header["version"], Eranges, Iranges, ctrls)
+        elif name == "VMP LOG":
+            log = process_log(module_data)
+        elif name == "VMP loop":
+            loop = process_loop(module_data)
+        elif name == "VMP ExtDev":
+            ext = process_ext(module_data)
+        else:
+            raise NotImplementedError(f"Unknown module: {name}.")
+    if ext is not None:
+        # replace names, units, and correct sigmas in data with headers present in ext
+        for k in {"Analog IN 1", "Analog IN 2"}:
+            parts = ext[k].split("/")
+            if len(parts) == 1:
+                n = parts[0]
+                u = " "
+            else:
+                n, u = parts
+            if k in ds:
+                ds[n] = ds[k]
+                ds[n].attrs = {"units": u, "ancillary_variables": f"{n}_std_err"}
+                del ds[k]
+                devs = ds[f"{k}_std_err"]
+                fac = ext[k + " max x"] - ext[k + " min x"]
+                fac = fac / (ext[k + " max V"] - ext[k + " min V"])
+                ds[f"{n}_std_err"] = devs * fac
+                ds[f"{n}_std_err"].attrs = {
+                    "units": u,
+                    "standard_name": f"{n} standard_error",
+                }
+                del ds[f"{k}_std_err"]
+        settings.update(ext)
+    return settings, params, ds, log, loop
+
+
+def process(
+    *,
+    fn: str,
+    timezone: ZoneInfo,
+    **kwargs: dict,
+) -> xr.Dataset:
+    """Processes EC-Lab raw data binary files.
+
+    Parameters
+    ----------
+    fn
+        The file containing the data to parse.
+
+    encoding
+        Encoding of ``fn``, by default "windows-1252".
+
+    timezone
+        A string description of the timezone. Default is "localtime".
+
+    Returns
+    -------
+    :class:`xarray.Dataset`
+        The full date is specified only if the "LOG" module is present.
+
+    """
+    file_magic = b"BIO-LOGIC MODULAR FILE\x1a                         \x00\x00\x00\x00"
+    with open(fn, "rb") as mpr_file:
+        assert mpr_file.read(len(file_magic)) == file_magic, "invalid file magic"
+        mpr = mpr_file.read()
+    settings, params, ds, log, loop = process_modules(mpr)
+    assert settings is not None, "no settings module"
+    assert ds is not None, "no data module"
+    # Arrange all the data into the correct format.
+    # TODO: Metadata could be handled in a nicer way.
+    metadata = {"settings": settings, "params": params}
+    if log is None:
+        logger.warning("No 'log' module present in mpr file. Timestamps incomplete.")
+        start_time = 0
+        fulldate = False
+    else:
+        metadata["log"] = log
+        start_time = ole_to_uts(log["ole_timestamp"], timezone=timezone)
+        fulldate = True
+    if "time" in ds:
+        ds["uts"] = ds["time"] + start_time
+    else:
+        ds["uts"] = [start_time]
+    if fulldate:
+        del ds.attrs["fulldate"]
+    ds.attrs.update(metadata)
+    return ds
```

### Comparing `yadg-5.0.1/src/yadg/parsers/electrochem/eclabmpt.py` & `yadg-5.0.2/src/yadg/parsers/electrochem/eclabmpt.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,280 +1,280 @@
-"""
-**eclabmpt**: Processing of BioLogic's EC-Lab ASCII export files.
------------------------------------------------------------------
-
-``.mpt`` files are made up of a header portion (with the technique
-parameter sequences and an optional loops section) and a tab-separated
-data table.
-
-A list of techniques supported by this parser is shown in `the techniques table
-<yadg.parsers.electrochem.eclabmpr.techniques>`_.
-
-File Structure of ``.mpt`` Files
-````````````````````````````````
-
-These human-readable files are sectioned into headerlines and datalines.
-The header part of the ``.mpt`` files is made up of information that can be found
-in the settings, log and loop modules of the binary ``.mpr`` file.
-
-If no header is present, the timestamps will instead be calculated from
-the file's ``mtime()``.
-
-
-Metadata
-````````
-The metadata will contain the information from the header of the file.
-
-.. note ::
-
-    The mapping between metadata parameters between ``.mpr`` and ``.mpt`` files
-    is not yet complete.
-
-.. codeauthor:: Nicolas Vetsch
-"""
-import re
-import logging
-import locale as lc
-import xarray as xr
-from zoneinfo import ZoneInfo
-from ...dgutils.dateutils import str_to_uts
-from .eclabcommon.techniques import get_resolution, technique_params, param_from_key
-from .eclabcommon.mpt_columns import column_units
-from yadg.parsers.basiccsv.main import append_dicts, dicts_to_dataset
-
-logger = logging.getLogger(__name__)
-
-
-def process_header(lines: list[str], timezone: str) -> tuple[dict, list, dict]:
-    """Processes the header lines.
-
-    Parameters
-    ----------
-    lines
-        The header lines, starting at line 3 (which is an empty line),
-        right after the `"Nb header lines : "` line.
-
-    Returns
-    -------
-    tuple[dict, dict]
-        A dictionary containing the settings (and the technique
-        parameters) and a dictionary containing the loop indexes.
-
-    """
-    sections = "\n".join(lines).split("\n\n")
-    # Can happen that no settings are present but just a loops section.
-    assert not sections[1].startswith("Number of loops : "), "no settings present"
-    # Again, we need the acquisition time to get timestamped data.
-    assert len(sections) >= 3, "no settings present"
-    technique = sections[1].strip()
-    settings_lines = sections[2].split("\n")
-    technique, params_keys = technique_params(technique, settings_lines)
-    params = settings_lines[-len(params_keys) :]
-
-    # The sequence param columns are always allocated 20 characters.
-    n_sequences = int(len(params[0]) / 20)
-    params_values = []
-    for seq in range(1, n_sequences):
-        values = []
-        for param in params:
-            try:
-                val = lc.atof(param[seq * 20 : (seq + 1) * 20])
-            except ValueError:
-                val = param[seq * 20 : (seq + 1) * 20].strip()
-            values.append(val)
-        params_values.append(values)
-    params = [dict(zip(params_keys, values)) for values in params_values]
-    settings_lines = [line.strip() for line in settings_lines[: -len(params_keys)]]
-
-    # Parse the acquisition timestamp.
-    timestamp_re = re.compile(r"Acquisition started on : (?P<val>.+)")
-    timestamp_match = timestamp_re.search("\n".join(settings_lines))
-    timestamp = timestamp_match["val"]
-    for format in ("%m/%d/%Y %H:%M:%S", "%m.%d.%Y %H:%M:%S", "%m/%d/%Y %H:%M:%S.%f"):
-        uts = str_to_uts(
-            timestamp=timestamp, format=format, timezone=timezone, strict=False
-        )
-        if uts is not None:
-            break
-    if uts is None:
-        raise NotImplementedError(f"Time format for {timestamp} not implemented.")
-
-    loops = None
-    if len(sections) >= 4 and sections[-1].startswith("Number of loops : "):
-        # The header contains a loops section.
-        loops_lines = sections[-1].split("\n")
-        n_loops = int(loops_lines[0].split(":")[-1])
-        indexes = []
-        for n in range(n_loops):
-            index = loops_lines[n + 1].split("to")[0].split()[-1]
-            indexes.append(int(index))
-        loops = {"n_loops": n_loops, "indexes": indexes}
-    settings = {
-        "posix_timestamp": uts,
-        "technique": technique,
-        "raw": "\n".join(lines),
-    }
-    return settings, params, loops
-
-
-def process_data(
-    lines: list[str],
-    Eranges: list[float],
-    Iranges: list[float],
-    controls: list[str],
-):
-    """Processes the data lines.
-
-    Parameters
-    ----------
-    lines
-        The data lines, starting right after the last header section.
-        The first line is an empty line, the column names can be found
-        on the second line.
-
-    Returns
-    -------
-    dict
-        A dictionary containing the datapoints in the format
-        ([{column -> value}, ..., {column -> value}]). If the column
-        unit is set to None, the value is an int. Otherwise, the value
-        is a dict with value ("n"), sigma ("s"), and unit ("u").
-
-    """
-    # At this point the first two lines have already been read.
-    # Remove extra column due to an extra tab in .mpt file column names.
-    names = lines[1].split("\t")[:-1]
-    units = dict()
-    columns = list()
-    for n in names:
-        c, u = column_units[n]
-        columns.append(c)
-        if u is not None:
-            units[c] = u
-    data_lines = lines[2:]
-    allvals = dict()
-    allmeta = dict()
-    for li, line in enumerate(data_lines):
-        values = line.split("\t")
-        vals = dict()
-        for name, value in list(zip(columns, values)):
-            if units.get(name) is None:
-                ival = int(lc.atof(value))
-                if name == "I Range":
-                    vals[name] = param_from_key("I_range", ival)
-                else:
-                    vals[name] = ival
-            else:
-                try:
-                    fval = lc.atof(value)
-                    vals[name] = fval
-                except ValueError:
-                    sval = value.strip()
-                    vals[name] = sval
-        if "Ns" in vals:
-            Erange = Eranges[vals["Ns"]]
-            Irstr = Iranges[vals["Ns"]]
-        else:
-            Erange = Eranges[0]
-            Irstr = Iranges[0]
-        if "I Range" in vals:
-            Irstr = vals["I Range"]
-        Irange = param_from_key("I_range", Irstr, to_str=False)
-        devs = {}
-        if "control_V_I" in vals:
-            icv = controls[vals["Ns"]]
-            name = f"control_{icv}"
-            vals[name] = vals.pop("control_V_I")
-            units[name] = "mA" if icv in {"I", "C"} else "V"
-        for col, val in vals.items():
-            unit = units.get(col)
-            if unit is None:
-                continue
-            assert isinstance(val, float), "`n` should not be string"
-            devs[col] = get_resolution(col, val, unit, Erange, Irange)
-
-        append_dicts(vals, devs, allvals, allmeta, li=li)
-
-    ds = dicts_to_dataset(allvals, allmeta, units, fulldate=False)
-    return ds
-
-
-def process(
-    *,
-    fn: str,
-    encoding: str,
-    locale: str,
-    timezone: ZoneInfo,
-    **kwargs: dict,
-) -> xr.Dataset:
-    """Processes EC-Lab human-readable text export files.
-
-    Parameters
-    ----------
-    fn
-        The file containing the data to parse.
-
-    encoding
-        Encoding of ``fn``, by default "windows-1252".
-
-    timezone
-        A string description of the timezone. Default is "UTC".
-
-    Returns
-    -------
-    :class:`xarray.Dataset`
-        The full date may not be specified if header is not present.
-
-    """
-    file_magic = "EC-Lab ASCII FILE\n"
-    with open(fn, "r", encoding=encoding) as mpt_file:
-        assert mpt_file.read(len(file_magic)) == file_magic, "invalid file magic"
-        mpt = mpt_file.read()
-    lines = mpt.split("\n")
-    nb_header_lines = int(lines[0].split()[-1])
-    header_lines = lines[: nb_header_lines - 3]
-    data_lines = lines[nb_header_lines - 3 :]
-    settings, params = {}, []
-
-    # Store current LC_NUMERIC before we do anything:
-    old_loc = lc.getlocale(category=lc.LC_NUMERIC)
-    lc.setlocale(lc.LC_NUMERIC, locale=locale)
-    if nb_header_lines <= 3:
-        logger.warning("Header contains no settings and hence no timestamp.")
-        start_time = 0.0
-        fulldate = False
-        Eranges = [20.0]
-        Iranges = ["Auto"]
-        ctrls = [None]
-    else:
-        settings, params, _ = process_header(header_lines, timezone)
-        start_time = settings.get("posix_timestamp")
-        fulldate = True
-        Eranges = []
-        Iranges = []
-        ctrls = []
-        for el in params:
-            E_range_max = el.get("E_range_max", float("inf"))
-            E_range_min = el.get("E_range_min", float("-inf"))
-            Eranges.append(E_range_max - E_range_min)
-            Iranges.append(el.get("I_range", "Auto"))
-            if "set_I/C" in el:
-                ctrls.append(el["set_I/C"])
-            elif "apply_I/C" in el:
-                ctrls.append(el["apply_I/C"])
-            else:
-                ctrls.append(None)
-    # Arrange all the data into the correct format.
-    # TODO: Metadata could be handled in a nicer way.
-    metadata = {"settings": settings, "params": params}
-
-    ds = process_data(data_lines, Eranges, Iranges, ctrls)
-    if "time" in ds:
-        ds["uts"] = ds["time"] + start_time
-    else:
-        ds["uts"] = [start_time]
-    if fulldate:
-        del ds.attrs["fulldate"]
-    ds.attrs.update(metadata)
-    # reset to original LC_NUMERIC
-    lc.setlocale(category=lc.LC_NUMERIC, locale=old_loc)
-    return ds
+"""
+**eclabmpt**: Processing of BioLogic's EC-Lab ASCII export files.
+-----------------------------------------------------------------
+
+``.mpt`` files are made up of a header portion (with the technique
+parameter sequences and an optional loops section) and a tab-separated
+data table.
+
+A list of techniques supported by this parser is shown in `the techniques table
+<yadg.parsers.electrochem.eclabmpr.techniques>`_.
+
+File Structure of ``.mpt`` Files
+````````````````````````````````
+
+These human-readable files are sectioned into headerlines and datalines.
+The header part of the ``.mpt`` files is made up of information that can be found
+in the settings, log and loop modules of the binary ``.mpr`` file.
+
+If no header is present, the timestamps will instead be calculated from
+the file's ``mtime()``.
+
+
+Metadata
+````````
+The metadata will contain the information from the header of the file.
+
+.. note ::
+
+    The mapping between metadata parameters between ``.mpr`` and ``.mpt`` files
+    is not yet complete.
+
+.. codeauthor:: Nicolas Vetsch
+"""
+import re
+import logging
+import locale as lc
+import xarray as xr
+from zoneinfo import ZoneInfo
+from ...dgutils.dateutils import str_to_uts
+from .eclabcommon.techniques import get_resolution, technique_params, param_from_key
+from .eclabcommon.mpt_columns import column_units
+from yadg.parsers.basiccsv.main import append_dicts, dicts_to_dataset
+
+logger = logging.getLogger(__name__)
+
+
+def process_header(lines: list[str], timezone: str) -> tuple[dict, list, dict]:
+    """Processes the header lines.
+
+    Parameters
+    ----------
+    lines
+        The header lines, starting at line 3 (which is an empty line),
+        right after the `"Nb header lines : "` line.
+
+    Returns
+    -------
+    tuple[dict, dict]
+        A dictionary containing the settings (and the technique
+        parameters) and a dictionary containing the loop indexes.
+
+    """
+    sections = "\n".join(lines).split("\n\n")
+    # Can happen that no settings are present but just a loops section.
+    assert not sections[1].startswith("Number of loops : "), "no settings present"
+    # Again, we need the acquisition time to get timestamped data.
+    assert len(sections) >= 3, "no settings present"
+    technique = sections[1].strip()
+    settings_lines = sections[2].split("\n")
+    technique, params_keys = technique_params(technique, settings_lines)
+    params = settings_lines[-len(params_keys) :]
+
+    # The sequence param columns are always allocated 20 characters.
+    n_sequences = int(len(params[0]) / 20)
+    params_values = []
+    for seq in range(1, n_sequences):
+        values = []
+        for param in params:
+            try:
+                val = lc.atof(param[seq * 20 : (seq + 1) * 20])
+            except ValueError:
+                val = param[seq * 20 : (seq + 1) * 20].strip()
+            values.append(val)
+        params_values.append(values)
+    params = [dict(zip(params_keys, values)) for values in params_values]
+    settings_lines = [line.strip() for line in settings_lines[: -len(params_keys)]]
+
+    # Parse the acquisition timestamp.
+    timestamp_re = re.compile(r"Acquisition started on : (?P<val>.+)")
+    timestamp_match = timestamp_re.search("\n".join(settings_lines))
+    timestamp = timestamp_match["val"]
+    for format in ("%m/%d/%Y %H:%M:%S", "%m.%d.%Y %H:%M:%S", "%m/%d/%Y %H:%M:%S.%f"):
+        uts = str_to_uts(
+            timestamp=timestamp, format=format, timezone=timezone, strict=False
+        )
+        if uts is not None:
+            break
+    if uts is None:
+        raise NotImplementedError(f"Time format for {timestamp} not implemented.")
+
+    loops = None
+    if len(sections) >= 4 and sections[-1].startswith("Number of loops : "):
+        # The header contains a loops section.
+        loops_lines = sections[-1].split("\n")
+        n_loops = int(loops_lines[0].split(":")[-1])
+        indexes = []
+        for n in range(n_loops):
+            index = loops_lines[n + 1].split("to")[0].split()[-1]
+            indexes.append(int(index))
+        loops = {"n_loops": n_loops, "indexes": indexes}
+    settings = {
+        "posix_timestamp": uts,
+        "technique": technique,
+        "raw": "\n".join(lines),
+    }
+    return settings, params, loops
+
+
+def process_data(
+    lines: list[str],
+    Eranges: list[float],
+    Iranges: list[float],
+    controls: list[str],
+):
+    """Processes the data lines.
+
+    Parameters
+    ----------
+    lines
+        The data lines, starting right after the last header section.
+        The first line is an empty line, the column names can be found
+        on the second line.
+
+    Returns
+    -------
+    dict
+        A dictionary containing the datapoints in the format
+        ([{column -> value}, ..., {column -> value}]). If the column
+        unit is set to None, the value is an int. Otherwise, the value
+        is a dict with value ("n"), sigma ("s"), and unit ("u").
+
+    """
+    # At this point the first two lines have already been read.
+    # Remove extra column due to an extra tab in .mpt file column names.
+    names = lines[1].split("\t")[:-1]
+    units = dict()
+    columns = list()
+    for n in names:
+        c, u = column_units[n]
+        columns.append(c)
+        if u is not None:
+            units[c] = u
+    data_lines = lines[2:]
+    allvals = dict()
+    allmeta = dict()
+    for li, line in enumerate(data_lines):
+        values = line.split("\t")
+        vals = dict()
+        for name, value in list(zip(columns, values)):
+            if units.get(name) is None:
+                ival = int(lc.atof(value))
+                if name == "I Range":
+                    vals[name] = param_from_key("I_range", ival)
+                else:
+                    vals[name] = ival
+            else:
+                try:
+                    fval = lc.atof(value)
+                    vals[name] = fval
+                except ValueError:
+                    sval = value.strip()
+                    vals[name] = sval
+        if "Ns" in vals:
+            Erange = Eranges[vals["Ns"]]
+            Irstr = Iranges[vals["Ns"]]
+        else:
+            Erange = Eranges[0]
+            Irstr = Iranges[0]
+        if "I Range" in vals:
+            Irstr = vals["I Range"]
+        Irange = param_from_key("I_range", Irstr, to_str=False)
+        devs = {}
+        if "control_V_I" in vals:
+            icv = controls[vals["Ns"]]
+            name = f"control_{icv}"
+            vals[name] = vals.pop("control_V_I")
+            units[name] = "mA" if icv in {"I", "C"} else "V"
+        for col, val in vals.items():
+            unit = units.get(col)
+            if unit is None:
+                continue
+            assert isinstance(val, float), "`n` should not be string"
+            devs[col] = get_resolution(col, val, unit, Erange, Irange)
+
+        append_dicts(vals, devs, allvals, allmeta, li=li)
+
+    ds = dicts_to_dataset(allvals, allmeta, units, fulldate=False)
+    return ds
+
+
+def process(
+    *,
+    fn: str,
+    encoding: str,
+    locale: str,
+    timezone: ZoneInfo,
+    **kwargs: dict,
+) -> xr.Dataset:
+    """Processes EC-Lab human-readable text export files.
+
+    Parameters
+    ----------
+    fn
+        The file containing the data to parse.
+
+    encoding
+        Encoding of ``fn``, by default "windows-1252".
+
+    timezone
+        A string description of the timezone. Default is "UTC".
+
+    Returns
+    -------
+    :class:`xarray.Dataset`
+        The full date may not be specified if header is not present.
+
+    """
+    file_magic = "EC-Lab ASCII FILE\n"
+    with open(fn, "r", encoding=encoding) as mpt_file:
+        assert mpt_file.read(len(file_magic)) == file_magic, "invalid file magic"
+        mpt = mpt_file.read()
+    lines = mpt.split("\n")
+    nb_header_lines = int(lines[0].split()[-1])
+    header_lines = lines[: nb_header_lines - 3]
+    data_lines = lines[nb_header_lines - 3 :]
+    settings, params = {}, []
+
+    # Store current LC_NUMERIC before we do anything:
+    old_loc = lc.getlocale(category=lc.LC_NUMERIC)
+    lc.setlocale(lc.LC_NUMERIC, locale=locale)
+    if nb_header_lines <= 3:
+        logger.warning("Header contains no settings and hence no timestamp.")
+        start_time = 0.0
+        fulldate = False
+        Eranges = [20.0]
+        Iranges = ["Auto"]
+        ctrls = [None]
+    else:
+        settings, params, _ = process_header(header_lines, timezone)
+        start_time = settings.get("posix_timestamp")
+        fulldate = True
+        Eranges = []
+        Iranges = []
+        ctrls = []
+        for el in params:
+            E_range_max = el.get("E_range_max", float("inf"))
+            E_range_min = el.get("E_range_min", float("-inf"))
+            Eranges.append(E_range_max - E_range_min)
+            Iranges.append(el.get("I_range", "Auto"))
+            if "set_I/C" in el:
+                ctrls.append(el["set_I/C"])
+            elif "apply_I/C" in el:
+                ctrls.append(el["apply_I/C"])
+            else:
+                ctrls.append(None)
+    # Arrange all the data into the correct format.
+    # TODO: Metadata could be handled in a nicer way.
+    metadata = {"settings": settings, "params": params}
+
+    ds = process_data(data_lines, Eranges, Iranges, ctrls)
+    if "time" in ds:
+        ds["uts"] = ds["time"] + start_time
+    else:
+        ds["uts"] = [start_time]
+    if fulldate:
+        del ds.attrs["fulldate"]
+    ds.attrs.update(metadata)
+    # reset to original LC_NUMERIC
+    lc.setlocale(category=lc.LC_NUMERIC, locale=old_loc)
+    return ds
```

### Comparing `yadg-5.0.1/src/yadg/parsers/electrochem/tomatojson.py` & `yadg-5.0.2/src/yadg/parsers/electrochem/tomatojson.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,142 +1,142 @@
-"""
-**tomatojson**: Processing of tomato electrochemistry outputs.
---------------------------------------------------------------
-
-This module parses the electrochemistry ``json`` files generated by tomato.
-
-.. warning::
-
-    This parser is brand-new in `yadg-4.1` and the interface is unstable.
-
-Four sections are expected in each tomato data file:
-
-- ``technique`` section, describing the current technique,
-- ``previous`` section, containing status information of the previous file,
-- ``current`` section, containing status information of the current file,
-- ``data`` section, containing the timesteps.
-
-The reason why both ``previous`` and ``current`` are requires is that the device
-status is recorded at the time of data polling, which means the values in ``current``
-might be invalid (after the run has finished) or not in sync with the ``data`` (if
-a technique change happened). However, ``previous`` may not be present in the first
-data file of an experiment.
-
-To determine the measurement errors, the values from BioLogic manual are used: for
-measured voltages (:math:`E_{\\text{we}}` and :math:`E_{\\text{ce}}`) this corresponds
-to a constant uncertainty of 0.004% of the applied E-range with a maximum of 75 uV,
-while for currents (:math:`I`) this is a constant uncertainty of 0.0015% of the applied
-I-range with a maximum of 0.76 uA.
-
-.. codeauthor:: Peter Kraus
-"""
-
-import json
-import logging
-import xarray as xr
-
-logger = logging.getLogger(__name__)
-
-I_ranges = {
-    "1 A": 1e0,
-    "100 mA": 1e-1,
-    "10 mA": 1e-2,
-    "1 mA": 1e-3,
-    "100 uA": 1e-4,
-    "10 uA": 1e-5,
-    "1 uA": 1e-6,
-    "100 pA": 1e-7,
-}
-
-
-def process(*, fn: str, **kwargs: dict) -> xr.Dataset:
-    with open(fn, "r") as infile:
-        jsdata = json.load(infile)
-
-    technique = jsdata["technique"]
-    previous = jsdata.get("previous", None)
-    current = jsdata["current"]
-
-    if "uts" in technique:
-        uts = technique["uts"]
-        fulldate = True
-    else:
-        uts = 0
-        fulldate = False
-
-    uts += technique["start_time"]
-
-    if previous is None:
-        meta = current
-    elif current["status"] == "STOP":
-        meta = previous
-    elif previous["elapsed_time"] > technique["start_time"]:
-        meta = previous
-    else:
-        meta = current
-
-    I_range = I_ranges[meta["I_range"]]
-    E_range = meta["E_range"]["max"] - meta["E_range"]["min"]
-
-    data_vars = {
-        "loop number": [],
-        "technique": [],
-        "index": [],
-        "time": [],
-        "Ewe": [],
-        "Ewe_std_err": [],
-        "Ece": [],
-        "Ece_std_err": [],
-        "I": [],
-        "I_std_err": [],
-        "cycle": [],
-    }
-
-    for point in jsdata["data"]:
-        for k, v in point.items():
-            if k == "time":
-                data_vars[k].append(uts + v)
-            elif k in {"Ewe", "Ece"}:
-                data_vars[k].append(v)
-                data_vars[f"{k}_std_err"].append(max(E_range * 0.0015 / 100, 75e-6))
-            elif k in {"I"}:
-                data_vars[k].append(v)
-                data_vars[f"{k}_std_err"].append(max(I_range * 0.004 / 100, 760e-12))
-            elif k in {"cycle"}:
-                data_vars[k].append(v)
-            else:
-                logger.cricital(f"parameter {k}: {v} not understood.")
-        data_vars["loop number"].append(technique["loop_number"])
-        data_vars["technique"].append(technique["name"])
-        data_vars["index"].append(technique["index"])
-
-    data_vars["cycle number"] = data_vars.pop("cycle")
-    uts = data_vars.pop("time")
-
-    data_vars = {k: v for k, v in data_vars.items() if len(v) > 0}
-
-    for k in data_vars:
-        if k in {"Ewe", "Ece", "I"}:
-            data_vars[k] = (
-                ["uts"],
-                data_vars[k],
-                {
-                    "units": "A" if k == "I" else "V",
-                    "ancillary_variables": f"{k}_std_err",
-                },
-            )
-        elif k.endswith("_std_err"):
-            data_vars[k] = (
-                ["uts"],
-                data_vars[k],
-                {
-                    "units": "A" if k == "I" else "V",
-                    "standard_name": f"{k.replace('_std_err', '')} standard_error",
-                },
-            )
-        else:
-            data_vars[k] = (["uts"], data_vars[k])
-
-    ds = xr.Dataset(data_vars, coords=dict(uts=uts))
-    if not fulldate:
-        ds.attrs["fulldate"] = False
-    return ds
+"""
+**tomatojson**: Processing of tomato electrochemistry outputs.
+--------------------------------------------------------------
+
+This module parses the electrochemistry ``json`` files generated by tomato.
+
+.. warning::
+
+    This parser is brand-new in `yadg-4.1` and the interface is unstable.
+
+Four sections are expected in each tomato data file:
+
+- ``technique`` section, describing the current technique,
+- ``previous`` section, containing status information of the previous file,
+- ``current`` section, containing status information of the current file,
+- ``data`` section, containing the timesteps.
+
+The reason why both ``previous`` and ``current`` are requires is that the device
+status is recorded at the time of data polling, which means the values in ``current``
+might be invalid (after the run has finished) or not in sync with the ``data`` (if
+a technique change happened). However, ``previous`` may not be present in the first
+data file of an experiment.
+
+To determine the measurement errors, the values from BioLogic manual are used: for
+measured voltages (:math:`E_{\\text{we}}` and :math:`E_{\\text{ce}}`) this corresponds
+to a constant uncertainty of 0.004% of the applied E-range with a maximum of 75 uV,
+while for currents (:math:`I`) this is a constant uncertainty of 0.0015% of the applied
+I-range with a maximum of 0.76 uA.
+
+.. codeauthor:: Peter Kraus
+"""
+
+import json
+import logging
+import xarray as xr
+
+logger = logging.getLogger(__name__)
+
+I_ranges = {
+    "1 A": 1e0,
+    "100 mA": 1e-1,
+    "10 mA": 1e-2,
+    "1 mA": 1e-3,
+    "100 uA": 1e-4,
+    "10 uA": 1e-5,
+    "1 uA": 1e-6,
+    "100 pA": 1e-7,
+}
+
+
+def process(*, fn: str, **kwargs: dict) -> xr.Dataset:
+    with open(fn, "r") as infile:
+        jsdata = json.load(infile)
+
+    technique = jsdata["technique"]
+    previous = jsdata.get("previous", None)
+    current = jsdata["current"]
+
+    if "uts" in technique:
+        uts = technique["uts"]
+        fulldate = True
+    else:
+        uts = 0
+        fulldate = False
+
+    uts += technique["start_time"]
+
+    if previous is None:
+        meta = current
+    elif current["status"] == "STOP":
+        meta = previous
+    elif previous["elapsed_time"] > technique["start_time"]:
+        meta = previous
+    else:
+        meta = current
+
+    I_range = I_ranges[meta["I_range"]]
+    E_range = meta["E_range"]["max"] - meta["E_range"]["min"]
+
+    data_vars = {
+        "loop number": [],
+        "technique": [],
+        "index": [],
+        "time": [],
+        "Ewe": [],
+        "Ewe_std_err": [],
+        "Ece": [],
+        "Ece_std_err": [],
+        "I": [],
+        "I_std_err": [],
+        "cycle": [],
+    }
+
+    for point in jsdata["data"]:
+        for k, v in point.items():
+            if k == "time":
+                data_vars[k].append(uts + v)
+            elif k in {"Ewe", "Ece"}:
+                data_vars[k].append(v)
+                data_vars[f"{k}_std_err"].append(max(E_range * 0.0015 / 100, 75e-6))
+            elif k in {"I"}:
+                data_vars[k].append(v)
+                data_vars[f"{k}_std_err"].append(max(I_range * 0.004 / 100, 760e-12))
+            elif k in {"cycle"}:
+                data_vars[k].append(v)
+            else:
+                logger.cricital(f"parameter {k}: {v} not understood.")
+        data_vars["loop number"].append(technique["loop_number"])
+        data_vars["technique"].append(technique["name"])
+        data_vars["index"].append(technique["index"])
+
+    data_vars["cycle number"] = data_vars.pop("cycle")
+    uts = data_vars.pop("time")
+
+    data_vars = {k: v for k, v in data_vars.items() if len(v) > 0}
+
+    for k in data_vars:
+        if k in {"Ewe", "Ece", "I"}:
+            data_vars[k] = (
+                ["uts"],
+                data_vars[k],
+                {
+                    "units": "A" if k == "I" else "V",
+                    "ancillary_variables": f"{k}_std_err",
+                },
+            )
+        elif k.endswith("_std_err"):
+            data_vars[k] = (
+                ["uts"],
+                data_vars[k],
+                {
+                    "units": "A" if k == "I" else "V",
+                    "standard_name": f"{k.replace('_std_err', '')} standard_error",
+                },
+            )
+        else:
+            data_vars[k] = (["uts"], data_vars[k])
+
+    ds = xr.Dataset(data_vars, coords=dict(uts=uts))
+    if not fulldate:
+        ds.attrs["fulldate"] = False
+    return ds
```

### Comparing `yadg-5.0.1/src/yadg/parsers/flowdata/__init__.py` & `yadg-5.0.2/src/yadg/parsers/flowdata/__init__.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-"""
-Handles the reading and processing of flow controller or flow meter data.
-
-Usage
-`````
-Available since ``yadg-4.0``. The parser supports the following parameters:
-
-.. _yadg.parsers.flowdata.model:
-
-.. autopydantic_model:: dgbowl_schemas.yadg.dataschema_5_0.step.FlowData
-
-.. _yadg.parsers.flowdata.formats:
-
-Formats
-```````
-The ``filetypes`` currently supported by the parser are:
-
-  - DryCal log file text output (``drycal.txt``),
-    see :mod:`~yadg.parsers.flowdata.drycal`
-  - DryCal log file tabulated output (``drycal.csv``),
-    see :mod:`~yadg.parsers.flowdata.drycal`
-  - DryCal log file document file (``drycal.rtf``),
-    see :mod:`~yadg.parsers.flowdata.drycal`
-
-.. _yadg.parsers.flowdata.provides:
-
-Schema
-``````
-The parser is used to extract all tabular data in the input file. This parser processes
-additional calibration information analogously to :mod:`~yadg.parsers.basiccsv`.
-
-Module Functions
-````````````````
-
-"""
-from .main import process
-
-__all__ = ["process"]
+"""
+Handles the reading and processing of flow controller or flow meter data.
+
+Usage
+`````
+Available since ``yadg-4.0``. The parser supports the following parameters:
+
+.. _yadg.parsers.flowdata.model:
+
+.. autopydantic_model:: dgbowl_schemas.yadg.dataschema_5_0.step.FlowData
+
+.. _yadg.parsers.flowdata.formats:
+
+Formats
+```````
+The ``filetypes`` currently supported by the parser are:
+
+  - DryCal log file text output (``drycal.txt``),
+    see :mod:`~yadg.parsers.flowdata.drycal`
+  - DryCal log file tabulated output (``drycal.csv``),
+    see :mod:`~yadg.parsers.flowdata.drycal`
+  - DryCal log file document file (``drycal.rtf``),
+    see :mod:`~yadg.parsers.flowdata.drycal`
+
+.. _yadg.parsers.flowdata.provides:
+
+Schema
+``````
+The parser is used to extract all tabular data in the input file. This parser processes
+additional calibration information analogously to :mod:`~yadg.parsers.basiccsv`.
+
+Module Functions
+````````````````
+
+"""
+from .main import process
+
+__all__ = ["process"]
```

### Comparing `yadg-5.0.1/src/yadg/parsers/flowdata/drycal.py` & `yadg-5.0.2/src/yadg/parsers/flowdata/drycal.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,228 +1,228 @@
-"""
-**drycal**: File parser for DryCal log files.
----------------------------------------------
-
-This module includes functions for parsing converted documents (``rtf``) and
-tabulated exports (``txt``, ``csv``).
-
-The DryCal files only contain the timestamps of the datapoints, not the date. Therefore,
-the date has to be supplied either using the ``date`` argument in parameters, or is
-parsed from the prefix of the filename.
-
-.. codeauthor:: Peter Kraus
-"""
-from striprtf.striprtf import rtf_to_text
-from ..basiccsv.main import process_row, append_dicts, dicts_to_dataset
-from ... import dgutils
-from pydantic import BaseModel
-from typing import Optional
-from datatree import DataTree
-from zoneinfo import ZoneInfo
-
-
-class TimeDate(BaseModel):
-    class TimestampSpec(BaseModel, extra="forbid"):
-        index: Optional[int] = None
-        format: Optional[str] = None
-
-    date: Optional[TimestampSpec] = None
-    time: Optional[TimestampSpec] = None
-
-
-def rtf(
-    fn: str,
-    encoding: str,
-    timezone: ZoneInfo,
-) -> DataTree:
-    """
-    RTF version of the drycal parser.
-
-    This is intended to parse legacy drycal DOC files, which have been converted to RTF
-    using other means.
-
-    Parameters
-    ----------
-    fn
-        Filename to parse.
-
-    encoding
-        Encoding to use for parsing ``fn``.
-
-    calib
-        A calibration spec.
-
-    Returns
-    -------
-    (timesteps, metadata, None): tuple[list, dict, None]
-        A standard data - metadata - common data output tuple.
-    """
-    with open(fn, "r", encoding=encoding) as infile:
-        rtf = infile.read()
-    lines = rtf_to_text(rtf).split("\n")
-    for li in range(len(lines)):
-        if lines[li].startswith("Sample"):
-            si = li
-        elif lines[li].startswith("1|"):
-            di = li
-            break
-    # Metadata processing for rtf files is in columns, not rows.
-    ml = []
-    metadata = dict()
-    for line in lines[:si]:
-        if line.strip() != "":
-            items = [i.strip() for i in line.split("|")]
-            if len(items) > 1:
-                ml.append(items)
-    assert len(ml) == 2 and len(ml[0]) == len(ml[1])
-    for i in range(len(ml[0])):
-        if ml[0][i] != "":
-            metadata[ml[0][i]] = ml[1][i]
-
-    # Process data table
-    dl = []
-    dl.append(" ".join(lines[si:di]))
-    for line in lines[di:]:
-        if line.strip() != "":
-            dl.append(line)
-    headers, units, data = drycal_table(dl, sep="|")
-    datecolumns, datefunc, _ = dgutils.infer_timestamp_from(
-        spec=TimeDate(time={"index": 4, "format": "%I:%M:%S %p"}), timezone=timezone
-    )
-
-    # Process rows
-    data_vals = {}
-    meta_vals = {"_fn": []}
-    for pi, point in enumerate(data):
-        vals, devs = process_row(headers[1:], point[1:], datefunc, datecolumns)
-        append_dicts(vals, devs, data_vals, meta_vals, fn, pi)
-
-    return dicts_to_dataset(data_vals, meta_vals, units, False)
-
-
-def sep(
-    fn: str,
-    sep: str,
-    encoding: str,
-    timezone: ZoneInfo,
-) -> DataTree:
-    """
-    Generic drycal parser, using ``sep`` as separator string.
-
-    This is intended to parse other export formats from DryCal, such as txt and csv files.
-
-    Parameters
-    ----------
-    fn
-        Filename to parse.
-
-    date
-        A unix timestamp float corresponding to the day (or other offset) to be added to
-        each line in the measurement table.
-
-    sep
-        The separator character used to split lines in ``fn``.
-
-    encoding
-        Encoding to use for parsing ``fn``.
-
-    calib
-        A calibration spec.
-
-    Returns
-    -------
-    (timesteps, metadata, None): tuple[list, dict, None]
-        A standard data - metadata - common data output tuple.
-    """
-    with open(fn, "r", encoding=encoding) as infile:
-        lines = infile.readlines()
-    for li in range(len(lines)):
-        if lines[li].startswith("Sample"):
-            si = li
-        elif lines[li].startswith(f"1{sep}"):
-            di = li
-            break
-    # Metadata processing for csv files is standard.
-    metadata = dict()
-    for line in lines[:si]:
-        if line.strip() != "":
-            items = [i.strip() for i in line.split(sep)]
-            if len(items) == 2:
-                metadata[items[0]] = items[1]
-
-    # Process data table
-    dl = list()
-    dl.append(" ".join(lines[si:di]))
-    for line in lines[di:]:
-        if line.strip() != "":
-            dl.append(line)
-    headers, units, data = drycal_table(dl, sep=sep)
-
-    if "AM" in data[0][-1].upper() or "PM" in data[0][-1].upper():
-        fmt = "%I:%M:%S %p"
-    else:
-        fmt = "%H:%M:%S"
-    datecolumns, datefunc, _ = dgutils.infer_timestamp_from(
-        spec=TimeDate(time={"index": 4, "format": fmt}), timezone=timezone
-    )
-
-    # Process rows
-    data_vals = {}
-    meta_vals = {"_fn": []}
-    for pi, point in enumerate(data):
-        vals, devs = process_row(headers[1:], point[1:], datefunc, datecolumns)
-        append_dicts(vals, devs, data_vals, meta_vals, fn, pi)
-
-    return dicts_to_dataset(data_vals, meta_vals, units, False)
-
-
-def drycal_table(lines: list, sep: str = ",") -> tuple[list, dict, list]:
-    """
-    DryCal table-processing function.
-
-    Given a table with headers and units in the first line, and data in the following
-    lines, this function returns the headers, units, and data extracted from the table.
-    The returned values are always of :class:`(str)` type, any post-processing is done
-    in the calling routine.
-
-    Parameters
-    ----------
-    lines
-        A list containing the lines to be parsed
-
-    sep
-        The separator string used to split each line into individual items
-
-    Returns
-    -------
-    (headers, units, data): tuple[list, dict, list]
-        A tuple of a list of the stripped headers, dictionary of header-unit key-value
-        pairs, and a list of lists containing the rows of the table.
-    """
-    items = [i.strip() for i in lines[0].split(sep)]
-    headers = []
-    units = {}
-    data = []
-    trim = False
-    for item in items:
-        for rs in [". ", " "]:
-            parts = item.split(rs)
-            if len(parts) == 2:
-                break
-        headers.append(parts[0])
-        if len(parts) == 2:
-            units[parts[0]] = parts[1]
-        else:
-            units[parts[0]] = " "
-    if items[-1] == "":
-        trim = True
-        headers = headers[:-1]
-    for line in lines[1:]:
-        cols = line.split(sep)
-        assert len(cols) == len(items)
-        if trim:
-            data.append(cols[:-1])
-        else:
-            data.append(cols)
-
-    units = dgutils.sanitize_units(units)
-    return headers, units, data
+"""
+**drycal**: File parser for DryCal log files.
+---------------------------------------------
+
+This module includes functions for parsing converted documents (``rtf``) and
+tabulated exports (``txt``, ``csv``).
+
+The DryCal files only contain the timestamps of the datapoints, not the date. Therefore,
+the date has to be supplied either using the ``date`` argument in parameters, or is
+parsed from the prefix of the filename.
+
+.. codeauthor:: Peter Kraus
+"""
+from striprtf.striprtf import rtf_to_text
+from ..basiccsv.main import process_row, append_dicts, dicts_to_dataset
+from ... import dgutils
+from pydantic import BaseModel
+from typing import Optional
+from datatree import DataTree
+from zoneinfo import ZoneInfo
+
+
+class TimeDate(BaseModel):
+    class TimestampSpec(BaseModel, extra="forbid"):
+        index: Optional[int] = None
+        format: Optional[str] = None
+
+    date: Optional[TimestampSpec] = None
+    time: Optional[TimestampSpec] = None
+
+
+def rtf(
+    fn: str,
+    encoding: str,
+    timezone: ZoneInfo,
+) -> DataTree:
+    """
+    RTF version of the drycal parser.
+
+    This is intended to parse legacy drycal DOC files, which have been converted to RTF
+    using other means.
+
+    Parameters
+    ----------
+    fn
+        Filename to parse.
+
+    encoding
+        Encoding to use for parsing ``fn``.
+
+    calib
+        A calibration spec.
+
+    Returns
+    -------
+    (timesteps, metadata, None): tuple[list, dict, None]
+        A standard data - metadata - common data output tuple.
+    """
+    with open(fn, "r", encoding=encoding) as infile:
+        rtf = infile.read()
+    lines = rtf_to_text(rtf).split("\n")
+    for li in range(len(lines)):
+        if lines[li].startswith("Sample"):
+            si = li
+        elif lines[li].startswith("1|"):
+            di = li
+            break
+    # Metadata processing for rtf files is in columns, not rows.
+    ml = []
+    metadata = dict()
+    for line in lines[:si]:
+        if line.strip() != "":
+            items = [i.strip() for i in line.split("|")]
+            if len(items) > 1:
+                ml.append(items)
+    assert len(ml) == 2 and len(ml[0]) == len(ml[1])
+    for i in range(len(ml[0])):
+        if ml[0][i] != "":
+            metadata[ml[0][i]] = ml[1][i]
+
+    # Process data table
+    dl = []
+    dl.append(" ".join(lines[si:di]))
+    for line in lines[di:]:
+        if line.strip() != "":
+            dl.append(line)
+    headers, units, data = drycal_table(dl, sep="|")
+    datecolumns, datefunc, _ = dgutils.infer_timestamp_from(
+        spec=TimeDate(time={"index": 4, "format": "%I:%M:%S %p"}), timezone=timezone
+    )
+
+    # Process rows
+    data_vals = {}
+    meta_vals = {"_fn": []}
+    for pi, point in enumerate(data):
+        vals, devs = process_row(headers[1:], point[1:], datefunc, datecolumns)
+        append_dicts(vals, devs, data_vals, meta_vals, fn, pi)
+
+    return dicts_to_dataset(data_vals, meta_vals, units, False)
+
+
+def sep(
+    fn: str,
+    sep: str,
+    encoding: str,
+    timezone: ZoneInfo,
+) -> DataTree:
+    """
+    Generic drycal parser, using ``sep`` as separator string.
+
+    This is intended to parse other export formats from DryCal, such as txt and csv files.
+
+    Parameters
+    ----------
+    fn
+        Filename to parse.
+
+    date
+        A unix timestamp float corresponding to the day (or other offset) to be added to
+        each line in the measurement table.
+
+    sep
+        The separator character used to split lines in ``fn``.
+
+    encoding
+        Encoding to use for parsing ``fn``.
+
+    calib
+        A calibration spec.
+
+    Returns
+    -------
+    (timesteps, metadata, None): tuple[list, dict, None]
+        A standard data - metadata - common data output tuple.
+    """
+    with open(fn, "r", encoding=encoding) as infile:
+        lines = infile.readlines()
+    for li in range(len(lines)):
+        if lines[li].startswith("Sample"):
+            si = li
+        elif lines[li].startswith(f"1{sep}"):
+            di = li
+            break
+    # Metadata processing for csv files is standard.
+    metadata = dict()
+    for line in lines[:si]:
+        if line.strip() != "":
+            items = [i.strip() for i in line.split(sep)]
+            if len(items) == 2:
+                metadata[items[0]] = items[1]
+
+    # Process data table
+    dl = list()
+    dl.append(" ".join(lines[si:di]))
+    for line in lines[di:]:
+        if line.strip() != "":
+            dl.append(line)
+    headers, units, data = drycal_table(dl, sep=sep)
+
+    if "AM" in data[0][-1].upper() or "PM" in data[0][-1].upper():
+        fmt = "%I:%M:%S %p"
+    else:
+        fmt = "%H:%M:%S"
+    datecolumns, datefunc, _ = dgutils.infer_timestamp_from(
+        spec=TimeDate(time={"index": 4, "format": fmt}), timezone=timezone
+    )
+
+    # Process rows
+    data_vals = {}
+    meta_vals = {"_fn": []}
+    for pi, point in enumerate(data):
+        vals, devs = process_row(headers[1:], point[1:], datefunc, datecolumns)
+        append_dicts(vals, devs, data_vals, meta_vals, fn, pi)
+
+    return dicts_to_dataset(data_vals, meta_vals, units, False)
+
+
+def drycal_table(lines: list, sep: str = ",") -> tuple[list, dict, list]:
+    """
+    DryCal table-processing function.
+
+    Given a table with headers and units in the first line, and data in the following
+    lines, this function returns the headers, units, and data extracted from the table.
+    The returned values are always of :class:`(str)` type, any post-processing is done
+    in the calling routine.
+
+    Parameters
+    ----------
+    lines
+        A list containing the lines to be parsed
+
+    sep
+        The separator string used to split each line into individual items
+
+    Returns
+    -------
+    (headers, units, data): tuple[list, dict, list]
+        A tuple of a list of the stripped headers, dictionary of header-unit key-value
+        pairs, and a list of lists containing the rows of the table.
+    """
+    items = [i.strip() for i in lines[0].split(sep)]
+    headers = []
+    units = {}
+    data = []
+    trim = False
+    for item in items:
+        for rs in [". ", " "]:
+            parts = item.split(rs)
+            if len(parts) == 2:
+                break
+        headers.append(parts[0])
+        if len(parts) == 2:
+            units[parts[0]] = parts[1]
+        else:
+            units[parts[0]] = " "
+    if items[-1] == "":
+        trim = True
+        headers = headers[:-1]
+    for line in lines[1:]:
+        cols = line.split(sep)
+        assert len(cols) == len(items)
+        if trim:
+            data.append(cols[:-1])
+        else:
+            data.append(cols)
+
+    units = dgutils.sanitize_units(units)
+    return headers, units, data
```

### Comparing `yadg-5.0.1/src/yadg/parsers/flowdata/main.py` & `yadg-5.0.2/src/yadg/parsers/flowdata/main.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-import logging
-import xarray as xr
-from zoneinfo import ZoneInfo
-from . import drycal
-
-logger = logging.getLogger(__name__)
-
-
-def process(
-    *,
-    fn: str,
-    filetype: str,
-    encoding: str,
-    timezone: ZoneInfo,
-    **kwargs: dict,
-) -> xr.Dataset:
-    """
-    Flow meter data processor
-
-    This parser processes flow meter data.
-
-    Parameters
-    ----------
-    fn
-        File to process
-
-    encoding
-        Encoding of ``fn``, by default "utf-8".
-
-    timezone
-        A string description of the timezone. Default is "localtime".
-
-    parameters
-        Parameters for :class:`~dgbowl_schemas.yadg.dataschema_5_0.step.FlowData`.
-
-    Returns
-    -------
-    :class:`xarray.Dataset`
-
-    """
-
-    if filetype.startswith("drycal"):
-
-        if filetype.endswith(".rtf") or fn.endswith("rtf"):
-            vals = drycal.rtf(fn, encoding, timezone)
-        elif filetype.endswith(".csv") or fn.endswith("csv"):
-            vals = drycal.sep(fn, ",", encoding, timezone)
-        elif filetype.endswith(".txt") or fn.endswith("txt"):
-            vals = drycal.sep(fn, "\t", encoding, timezone)
-
-        # check timestamps are increasing:
-        warn = True
-        ndays = 0
-        utslist = vals.uts.values
-        for i in range(1, vals.uts.size):
-            if utslist[i] < utslist[i - 1]:
-                if warn:
-                    logger.warning("DryCal log crossing day boundary. Adding offset.")
-                    warn = False
-                uts = utslist[i] + ndays * 86400
-                while uts < utslist[i - 1]:
-                    ndays += 1
-                    uts = utslist[i] + ndays * 86400
-                utslist[i] = uts
-        vals["uts"] = xr.DataArray(data=utslist, dims=["uts"])
-        vals.attrs["fulldate"] = False
-    return vals
+import logging
+import xarray as xr
+from zoneinfo import ZoneInfo
+from . import drycal
+
+logger = logging.getLogger(__name__)
+
+
+def process(
+    *,
+    fn: str,
+    filetype: str,
+    encoding: str,
+    timezone: ZoneInfo,
+    **kwargs: dict,
+) -> xr.Dataset:
+    """
+    Flow meter data processor
+
+    This parser processes flow meter data.
+
+    Parameters
+    ----------
+    fn
+        File to process
+
+    encoding
+        Encoding of ``fn``, by default "utf-8".
+
+    timezone
+        A string description of the timezone. Default is "localtime".
+
+    parameters
+        Parameters for :class:`~dgbowl_schemas.yadg.dataschema_5_0.step.FlowData`.
+
+    Returns
+    -------
+    :class:`xarray.Dataset`
+
+    """
+
+    if filetype.startswith("drycal"):
+
+        if filetype.endswith(".rtf") or fn.endswith("rtf"):
+            vals = drycal.rtf(fn, encoding, timezone)
+        elif filetype.endswith(".csv") or fn.endswith("csv"):
+            vals = drycal.sep(fn, ",", encoding, timezone)
+        elif filetype.endswith(".txt") or fn.endswith("txt"):
+            vals = drycal.sep(fn, "\t", encoding, timezone)
+
+        # check timestamps are increasing:
+        warn = True
+        ndays = 0
+        utslist = vals.uts.values
+        for i in range(1, vals.uts.size):
+            if utslist[i] < utslist[i - 1]:
+                if warn:
+                    logger.warning("DryCal log crossing day boundary. Adding offset.")
+                    warn = False
+                uts = utslist[i] + ndays * 86400
+                while uts < utslist[i - 1]:
+                    ndays += 1
+                    uts = utslist[i] + ndays * 86400
+                utslist[i] = uts
+        vals["uts"] = xr.DataArray(data=utslist, dims=["uts"])
+        vals.attrs["fulldate"] = False
+    return vals
```

### Comparing `yadg-5.0.1/src/yadg/parsers/masstrace/quadstarsac.py` & `yadg-5.0.2/src/yadg/parsers/masstrace/quadstarsac.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,264 +1,264 @@
-"""
-**quadstarsac**: Processing of Quadstar 32-bit scan analog data.
-----------------------------------------------------------------
-
-The `sac2dat.c code from Dr. Moritz Bubek <https://www.bubek.org/sac2dat.php>`_
-was a really useful stepping stone for this Python file parser.
-
-Pretty much the entire file format has been reverse engineered. There
-are still one or two unknown fields.
-
-File Structure of `.sac` Files
-``````````````````````````````
-
-.. code-block:: python
-
-    0x00 "data_index"
-    0x02 "software_id"
-    0x06 "version_major"
-    0x07 "version_minor"
-    0x08 "second"
-    0x09 "minute"
-    0x0a "hour"
-    0x0b "day"
-    0x0c "month"
-    0x0d "year"
-    0x0f "author"
-    0x64 "n_timesteps"
-    0x68 "n_traces"
-    0x6a "timestep_length"
-    ...
-    # Not sure what sits from 0x6e to 0xc2.
-    ...
-    0xc2 "uts_base_s"
-    0xc6 "uts_base_ms"
-    # Trace header. Read these 9 bytes for every trace (n_traces).
-    0xc8 + (n * 0x09) "type"
-    0xc9 + (n * 0x09) "info_position"
-    0xcd + (n * 0x09) "data_position"
-    ...
-    # Trace info. Read these 137 bytes for every trace where type != 0x11.
-    info_position + 0x00 "data_format"
-    info_position + 0x02 "y_title"
-    info_position + 0x0f "y_unit"
-    info_position + 0x1d "x_title"
-    info_position + 0x2a "x_unit"
-    info_position + 0x38 "comment"
-    info_position + 0x7a "first_mass"
-    info_position + 0x7e "scan_width"
-    info_position + 0x80 "values_per_mass"
-    info_position + 0x81 "zoom_start"
-    info_position + 0x85 "zoom_end"
-    ...
-    # UTS offset. Read these 6 bytes for every timestep (n_timesteps).
-    0xc2 + (n * timestep_length) "uts_offset_s"
-    0xc6 + (n * timestep_length) "uts_offset_ms"
-    # Read everything remaining below for every timestep and every trace
-    # where type != 0x11.
-    data_position + (n * timestep_length) + 0x00 "n_datapoints"
-    data_position + (n * timestep_length) + 0x04 "data_range"
-    # Datapoints. Read these 4 bytes (scan_width * values_per_mass)
-    # times.
-    data_position + (n * timestep_length) + 0x06 "datapoints"
-    ...
-
-.. codeauthor:: Nicolas Vetsch
-"""
-import numpy as np
-from datatree import DataTree
-import xarray as xr
-import yadg.dgutils as dgutils
-
-# The general header at the top of .sac files.
-general_header_dtype = np.dtype(
-    [
-        ("data_index", "<i2"),
-        ("software_id", "<i4"),
-        ("version_major", "|u1"),
-        ("version_minor", "|u1"),
-        ("S", "|u1"),
-        ("M", "|u1"),
-        ("H", "|u1"),
-        ("d", "|u1"),
-        ("m", "|u1"),
-        ("y", "|u1"),
-        ("username", "|S86"),
-        ("n_timesteps", "<i4"),
-        ("n_traces", "<i2"),
-        ("timestep_length", "<i4"),
-    ]
-)
-
-
-trace_header_dtype = np.dtype(
-    [
-        ("type", "|u1"),
-        ("info_position", "<i4"),
-        ("data_position", "<i4"),
-    ]
-)
-
-
-trace_info_dtype = np.dtype(
-    [
-        ("data_format", "<u2"),
-        ("y_title", "|S13"),
-        ("y_unit", "|S13"),
-        ("unknown_a", "|u1"),
-        ("x_title", "|S13"),
-        ("x_unit", "|S13"),
-        ("comment", "|S59"),
-        ("unknown_b", "|u4"),
-        ("unknown_c", "|u4"),
-        ("first_mass", "<f4"),
-        ("scan_width", "<u2"),
-        ("values_per_mass", "|u1"),
-        ("zoom_start", "<f4"),
-        ("zoom_end", "<f4"),
-    ]
-)
-
-
-def _find_first_data_position(scan_headers: list[dict]) -> int:
-    """Finds the data position of the first scan containing any data."""
-    for header in scan_headers:
-        if header["type"] != 0x11:
-            continue
-        return header["data_position"]
-
-
-def process(
-    *,
-    fn: str,
-    **kwargs: dict,
-) -> DataTree:
-    """Processes a Quadstar 32-bit analog data .sac file.
-
-    Parameters
-    ----------
-    fn
-        The file containing the trace(s) to parse.
-
-    Returns
-    -------
-    :class:`datatree.DataTree`
-        A :class:`datatree.DataTree` containing one :class:`xarray.Dataset` per mass trace.
-        The traces in the Quadstar ``.sac`` files are not named, therefore their index
-        is used as the :class:`xarray.Dataset` name.
-
-    """
-    with open(fn, "rb") as sac_file:
-        sac = sac_file.read()
-    meta = dgutils.read_value(sac, 0x0000, general_header_dtype)
-    uts_base_s = dgutils.read_value(sac, 0x00C2, "<u4")
-    # The ms part of the timestamps is actually saved as tenths of ms so
-    # multiplying this by 0.1 here.
-    uts_base_ms = dgutils.read_value(sac, 0x00C6, "<u2") * 1e-1
-    uts_base = uts_base_s + uts_base_ms * 1e-3
-    trace_headers = np.frombuffer(
-        sac,
-        offset=0x00C8,
-        dtype=trace_header_dtype,
-        count=meta["n_traces"],
-    )
-    # Find the data position of the first data-containing timestep.
-    data_pos_0 = _find_first_data_position(trace_headers)
-    traces = {}
-    for n in range(meta["n_timesteps"]):
-        ts_offset = n * meta["timestep_length"]
-        uts_offset_s = dgutils.read_value(sac, data_pos_0 - 0x0006 + ts_offset, "<u4")
-        uts_offset_ms = (
-            dgutils.read_value(sac, data_pos_0 - 0x0002 + ts_offset, "<u2") * 1e-1
-        )
-        uts_timestamp = uts_base + (uts_offset_s + uts_offset_ms * 1e-3)
-        for ti, header in enumerate(trace_headers):
-            if header["type"] != 0x11:
-                continue
-            info = dgutils.read_value(sac, header["info_position"], trace_info_dtype)
-            # Construct the mass data.
-            ndm = info["values_per_mass"]
-            mvals, dm = np.linspace(
-                info["first_mass"],
-                info["first_mass"] + info["scan_width"],
-                info["scan_width"] * ndm,
-                endpoint=False,
-                retstep=True,
-            )
-            mdevs = np.ones(len(mvals)) * dm
-            # Read and construct the y data.
-            ts_data_pos = header["data_position"] + ts_offset
-            # Determine the detector's full scale range.
-            fsr = 10 ** dgutils.read_value(sac, ts_data_pos + 0x0004, "<i2")
-            # The n_datapoints value at timestep_data_position is
-            # sometimes wrong. Calculating this here works, however.
-            n_datapoints = info["scan_width"] * info["values_per_mass"]
-            yvals = np.frombuffer(
-                sac, offset=ts_data_pos + 0x0006, dtype="<f4", count=n_datapoints
-            ).copy()
-            # Once a y_value leaves the FSR it jumps to the maximum
-            # of a float32. These values should be NaNs instead.
-            yvals[yvals > fsr] = np.nan
-            # TODO: Determine the correct accuracy from fsr. The 32bit
-            # ADC is a guess that seems to put the error in the correct
-            # order of magnitude.
-            sigma_adc = np.ones(len(yvals)) * fsr / 2**32
-            # Determine error based on contributions of neighboring masses.
-            # The upper limit on contribution from peak at next integer mass is 50ppm.
-            prev_neighbor = np.roll(yvals, ndm)
-            prev_neighbor[:ndm] = np.nan
-            next_neighbor = np.roll(yvals, -ndm)
-            next_neighbor[-ndm:] = np.nan
-            sigma_neighbor = np.fmax(prev_neighbor, next_neighbor) * 50e-6
-            # Pick the maximum error here
-            ydevs = np.fmax(sigma_adc, sigma_neighbor)
-            ds = xr.Dataset(
-                data_vars={
-                    "fsr": fsr,
-                    "mass_to_charge_std_err": (
-                        ["mass_to_charge"],
-                        mdevs,
-                        {
-                            "units": info["x_unit"],
-                            "standard_name": "mass_to_charge standard_error",
-                        },
-                    ),
-                    "y": (
-                        ["uts", "mass_to_charge"],
-                        [yvals],
-                        {"units": info["y_unit"], "ancilliary_variables": "y_std_err"},
-                    ),
-                    "y_std_err": (
-                        ["uts", "mass_to_charge"],
-                        [ydevs],
-                        {"units": info["y_unit"], "standard_name": "y standard_error"},
-                    ),
-                },
-                coords={
-                    "mass_to_charge": (
-                        ["mass_to_charge"],
-                        mvals,
-                        {
-                            "units": info["x_unit"],
-                            "ancillary_variables": "mass_to_charge_std_err",
-                        },
-                    ),
-                    "uts": (["uts"], [uts_timestamp]),
-                },
-                attrs=info,
-            )
-            if f"{ti}" not in traces:
-                traces[f"{ti}"] = ds
-            else:
-                try:
-                    traces[f"{ti}"] = xr.concat(
-                        [traces[f"{ti}"], ds], dim="uts", combine_attrs="identical"
-                    )
-                except xr.MergeError:
-                    raise RuntimeError(
-                        "Merging metadata from the individual traces has failed. "
-                        "This is a bug. Please open an issue on GitHub."
-                    )
-
-    ret = DataTree.from_dict(traces)
-    ret.attrs = meta
-    return ret
+"""
+**quadstarsac**: Processing of Quadstar 32-bit scan analog data.
+----------------------------------------------------------------
+
+The `sac2dat.c code from Dr. Moritz Bubek <https://www.bubek.org/sac2dat.php>`_
+was a really useful stepping stone for this Python file parser.
+
+Pretty much the entire file format has been reverse engineered. There
+are still one or two unknown fields.
+
+File Structure of `.sac` Files
+``````````````````````````````
+
+.. code-block:: python
+
+    0x00 "data_index"
+    0x02 "software_id"
+    0x06 "version_major"
+    0x07 "version_minor"
+    0x08 "second"
+    0x09 "minute"
+    0x0a "hour"
+    0x0b "day"
+    0x0c "month"
+    0x0d "year"
+    0x0f "author"
+    0x64 "n_timesteps"
+    0x68 "n_traces"
+    0x6a "timestep_length"
+    ...
+    # Not sure what sits from 0x6e to 0xc2.
+    ...
+    0xc2 "uts_base_s"
+    0xc6 "uts_base_ms"
+    # Trace header. Read these 9 bytes for every trace (n_traces).
+    0xc8 + (n * 0x09) "type"
+    0xc9 + (n * 0x09) "info_position"
+    0xcd + (n * 0x09) "data_position"
+    ...
+    # Trace info. Read these 137 bytes for every trace where type != 0x11.
+    info_position + 0x00 "data_format"
+    info_position + 0x02 "y_title"
+    info_position + 0x0f "y_unit"
+    info_position + 0x1d "x_title"
+    info_position + 0x2a "x_unit"
+    info_position + 0x38 "comment"
+    info_position + 0x7a "first_mass"
+    info_position + 0x7e "scan_width"
+    info_position + 0x80 "values_per_mass"
+    info_position + 0x81 "zoom_start"
+    info_position + 0x85 "zoom_end"
+    ...
+    # UTS offset. Read these 6 bytes for every timestep (n_timesteps).
+    0xc2 + (n * timestep_length) "uts_offset_s"
+    0xc6 + (n * timestep_length) "uts_offset_ms"
+    # Read everything remaining below for every timestep and every trace
+    # where type != 0x11.
+    data_position + (n * timestep_length) + 0x00 "n_datapoints"
+    data_position + (n * timestep_length) + 0x04 "data_range"
+    # Datapoints. Read these 4 bytes (scan_width * values_per_mass)
+    # times.
+    data_position + (n * timestep_length) + 0x06 "datapoints"
+    ...
+
+.. codeauthor:: Nicolas Vetsch
+"""
+import numpy as np
+from datatree import DataTree
+import xarray as xr
+import yadg.dgutils as dgutils
+
+# The general header at the top of .sac files.
+general_header_dtype = np.dtype(
+    [
+        ("data_index", "<i2"),
+        ("software_id", "<i4"),
+        ("version_major", "|u1"),
+        ("version_minor", "|u1"),
+        ("S", "|u1"),
+        ("M", "|u1"),
+        ("H", "|u1"),
+        ("d", "|u1"),
+        ("m", "|u1"),
+        ("y", "|u1"),
+        ("username", "|S86"),
+        ("n_timesteps", "<i4"),
+        ("n_traces", "<i2"),
+        ("timestep_length", "<i4"),
+    ]
+)
+
+
+trace_header_dtype = np.dtype(
+    [
+        ("type", "|u1"),
+        ("info_position", "<i4"),
+        ("data_position", "<i4"),
+    ]
+)
+
+
+trace_info_dtype = np.dtype(
+    [
+        ("data_format", "<u2"),
+        ("y_title", "|S13"),
+        ("y_unit", "|S13"),
+        ("unknown_a", "|u1"),
+        ("x_title", "|S13"),
+        ("x_unit", "|S13"),
+        ("comment", "|S59"),
+        ("unknown_b", "|u4"),
+        ("unknown_c", "|u4"),
+        ("first_mass", "<f4"),
+        ("scan_width", "<u2"),
+        ("values_per_mass", "|u1"),
+        ("zoom_start", "<f4"),
+        ("zoom_end", "<f4"),
+    ]
+)
+
+
+def _find_first_data_position(scan_headers: list[dict]) -> int:
+    """Finds the data position of the first scan containing any data."""
+    for header in scan_headers:
+        if header["type"] != 0x11:
+            continue
+        return header["data_position"]
+
+
+def process(
+    *,
+    fn: str,
+    **kwargs: dict,
+) -> DataTree:
+    """Processes a Quadstar 32-bit analog data .sac file.
+
+    Parameters
+    ----------
+    fn
+        The file containing the trace(s) to parse.
+
+    Returns
+    -------
+    :class:`datatree.DataTree`
+        A :class:`datatree.DataTree` containing one :class:`xarray.Dataset` per mass trace.
+        The traces in the Quadstar ``.sac`` files are not named, therefore their index
+        is used as the :class:`xarray.Dataset` name.
+
+    """
+    with open(fn, "rb") as sac_file:
+        sac = sac_file.read()
+    meta = dgutils.read_value(sac, 0x0000, general_header_dtype)
+    uts_base_s = dgutils.read_value(sac, 0x00C2, "<u4")
+    # The ms part of the timestamps is actually saved as tenths of ms so
+    # multiplying this by 0.1 here.
+    uts_base_ms = dgutils.read_value(sac, 0x00C6, "<u2") * 1e-1
+    uts_base = uts_base_s + uts_base_ms * 1e-3
+    trace_headers = np.frombuffer(
+        sac,
+        offset=0x00C8,
+        dtype=trace_header_dtype,
+        count=meta["n_traces"],
+    )
+    # Find the data position of the first data-containing timestep.
+    data_pos_0 = _find_first_data_position(trace_headers)
+    traces = {}
+    for n in range(meta["n_timesteps"]):
+        ts_offset = n * meta["timestep_length"]
+        uts_offset_s = dgutils.read_value(sac, data_pos_0 - 0x0006 + ts_offset, "<u4")
+        uts_offset_ms = (
+            dgutils.read_value(sac, data_pos_0 - 0x0002 + ts_offset, "<u2") * 1e-1
+        )
+        uts_timestamp = uts_base + (uts_offset_s + uts_offset_ms * 1e-3)
+        for ti, header in enumerate(trace_headers):
+            if header["type"] != 0x11:
+                continue
+            info = dgutils.read_value(sac, header["info_position"], trace_info_dtype)
+            # Construct the mass data.
+            ndm = info["values_per_mass"]
+            mvals, dm = np.linspace(
+                info["first_mass"],
+                info["first_mass"] + info["scan_width"],
+                info["scan_width"] * ndm,
+                endpoint=False,
+                retstep=True,
+            )
+            mdevs = np.ones(len(mvals)) * dm
+            # Read and construct the y data.
+            ts_data_pos = header["data_position"] + ts_offset
+            # Determine the detector's full scale range.
+            fsr = 10 ** dgutils.read_value(sac, ts_data_pos + 0x0004, "<i2")
+            # The n_datapoints value at timestep_data_position is
+            # sometimes wrong. Calculating this here works, however.
+            n_datapoints = info["scan_width"] * info["values_per_mass"]
+            yvals = np.frombuffer(
+                sac, offset=ts_data_pos + 0x0006, dtype="<f4", count=n_datapoints
+            ).copy()
+            # Once a y_value leaves the FSR it jumps to the maximum
+            # of a float32. These values should be NaNs instead.
+            yvals[yvals > fsr] = np.nan
+            # TODO: Determine the correct accuracy from fsr. The 32bit
+            # ADC is a guess that seems to put the error in the correct
+            # order of magnitude.
+            sigma_adc = np.ones(len(yvals)) * fsr / 2**32
+            # Determine error based on contributions of neighboring masses.
+            # The upper limit on contribution from peak at next integer mass is 50ppm.
+            prev_neighbor = np.roll(yvals, ndm)
+            prev_neighbor[:ndm] = np.nan
+            next_neighbor = np.roll(yvals, -ndm)
+            next_neighbor[-ndm:] = np.nan
+            sigma_neighbor = np.fmax(prev_neighbor, next_neighbor) * 50e-6
+            # Pick the maximum error here
+            ydevs = np.fmax(sigma_adc, sigma_neighbor)
+            ds = xr.Dataset(
+                data_vars={
+                    "fsr": fsr,
+                    "mass_to_charge_std_err": (
+                        ["mass_to_charge"],
+                        mdevs,
+                        {
+                            "units": info["x_unit"],
+                            "standard_name": "mass_to_charge standard_error",
+                        },
+                    ),
+                    "y": (
+                        ["uts", "mass_to_charge"],
+                        [yvals],
+                        {"units": info["y_unit"], "ancilliary_variables": "y_std_err"},
+                    ),
+                    "y_std_err": (
+                        ["uts", "mass_to_charge"],
+                        [ydevs],
+                        {"units": info["y_unit"], "standard_name": "y standard_error"},
+                    ),
+                },
+                coords={
+                    "mass_to_charge": (
+                        ["mass_to_charge"],
+                        mvals,
+                        {
+                            "units": info["x_unit"],
+                            "ancillary_variables": "mass_to_charge_std_err",
+                        },
+                    ),
+                    "uts": (["uts"], [uts_timestamp]),
+                },
+                attrs=info,
+            )
+            if f"{ti}" not in traces:
+                traces[f"{ti}"] = ds
+            else:
+                try:
+                    traces[f"{ti}"] = xr.concat(
+                        [traces[f"{ti}"], ds], dim="uts", combine_attrs="identical"
+                    )
+                except xr.MergeError:
+                    raise RuntimeError(
+                        "Merging metadata from the individual traces has failed. "
+                        "This is a bug. Please open an issue on GitHub."
+                    )
+
+    ret = DataTree.from_dict(traces)
+    ret.attrs = meta
+    return ret
```

### Comparing `yadg-5.0.1/src/yadg/parsers/meascsv/__init__.py` & `yadg-5.0.2/src/yadg/parsers/meascsv/__init__.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,116 +1,116 @@
-"""
-This parser handles the reading and processing of the legacy log files created by
-the LabView interface for the MCPT instrument. These files contain information about
-the timestamp, temperatures, and inlet / process flows.
-
-.. admonition:: DEPRECATED in ``yadg-4.0``
-
-    As of ``yadg-4.0``, this parser is deprecated and should not be used for new data.
-    Please consider switching to the :mod:`~yadg.parsers.basiccsv` parser.
-
-Usage
-`````
-Available since ``yadg-3.0``. Deprecated since ``yadg-4.0``. The parser supports the
-following parameters:
-
-.. _yadg.parsers.meascsv.model:
-
-.. autopydantic_model:: dgbowl_schemas.yadg.dataschema_5_0.step.MeasCSV
-
-.. _parsers_meascsv_provides:
-
-Schema
-``````
-The parser is used to extract all of the tabular data in the input file, storing
-them in the same format as :mod:`~yadg.parsers.basiccsv`, using the column headers
-as keys.
-
-"""
-
-import logging
-from pydantic import BaseModel
-from zoneinfo import ZoneInfo
-from ..basiccsv.main import process_row, append_dicts, dicts_to_dataset
-from ... import dgutils
-import xarray as xr
-
-logger = logging.getLogger(__name__)
-
-
-def process(
-    *,
-    fn: str,
-    encoding: str,
-    timezone: ZoneInfo,
-    parameters: BaseModel,
-    **kwargs: dict,
-) -> xr.Dataset:
-    """
-    Legacy MCPT measurement log parser.
-
-    This parser is included to maintain parity with older schemas and datagrams.
-    It is essentially a wrapper around :func:`yadg.parsers.basiccsv.main.process_row`.
-
-    .. admonition:: DEPRECATED in ``yadg-4.0``
-
-        For new applications, please use the :mod:`~yadg.parsers.basiccsv` parser.
-
-    Parameters
-    ----------
-    fn
-        File to process
-
-    encoding
-        Encoding of ``fn``, by default "utf-8".
-
-    timezone
-        A string description of the timezone. Default is "localtime".
-
-    parameters
-        Parameters for :class:`~dgbowl_schemas.yadg.dataschema_5_0.step.MeasCSV`.
-
-    Returns
-    -------
-    :class:`xarray.Dataset`
-        A :class:`xarray.Dataset` containing the timesteps, metadata, and full date tag. No
-        metadata is returned. The full date is always provided in :mod:`~yadg.parsers.meascsv`
-        compatible files.
-
-    """
-    logger.warning("This parser is deprecated. Please switch to 'basiccsv'.")
-
-    with open(fn, "r", encoding=encoding) as infile:
-        lines = [i.strip() for i in infile.readlines()]
-
-    headers = [i.strip() for i in lines.pop(0).split(";")]
-
-    for hi, header in enumerate(headers):
-        if "/" in header:
-            logger.warning("Replacing '/' for '_' in header '%s'.", header)
-            headers[hi] = header.replace("/", "_")
-
-    _units = [i.strip() for i in lines.pop(0).split(";")]
-    units = {}
-    for h in headers:
-        units[h] = _units.pop(0)
-
-    units = dgutils.sanitize_units(units)
-
-    datecolumns, datefunc, fulldate = dgutils.infer_timestamp_from(
-        spec=parameters.timestamp,
-        timezone=timezone,
-    )
-
-    # Process rows
-    data_vals = {}
-    meta_vals = {"_fn": []}
-    for li, line in enumerate(lines):
-        vals, devs = process_row(
-            headers,
-            line.split(";"),
-            datefunc,
-            datecolumns,
-        )
-        append_dicts(vals, devs, data_vals, meta_vals, fn, li)
-
-    return dicts_to_dataset(data_vals, meta_vals, units, fulldate)
+"""
+This parser handles the reading and processing of the legacy log files created by
+the LabView interface for the MCPT instrument. These files contain information about
+the timestamp, temperatures, and inlet / process flows.
+
+.. admonition:: DEPRECATED in ``yadg-4.0``
+
+    As of ``yadg-4.0``, this parser is deprecated and should not be used for new data.
+    Please consider switching to the :mod:`~yadg.parsers.basiccsv` parser.
+
+Usage
+`````
+Available since ``yadg-3.0``. Deprecated since ``yadg-4.0``. The parser supports the
+following parameters:
+
+.. _yadg.parsers.meascsv.model:
+
+.. autopydantic_model:: dgbowl_schemas.yadg.dataschema_5_0.step.MeasCSV
+
+.. _parsers_meascsv_provides:
+
+Schema
+``````
+The parser is used to extract all of the tabular data in the input file, storing
+them in the same format as :mod:`~yadg.parsers.basiccsv`, using the column headers
+as keys.
+
+"""
+
+import logging
+from pydantic import BaseModel
+from zoneinfo import ZoneInfo
+from ..basiccsv.main import process_row, append_dicts, dicts_to_dataset
+from ... import dgutils
+import xarray as xr
+
+logger = logging.getLogger(__name__)
+
+
+def process(
+    *,
+    fn: str,
+    encoding: str,
+    timezone: ZoneInfo,
+    parameters: BaseModel,
+    **kwargs: dict,
+) -> xr.Dataset:
+    """
+    Legacy MCPT measurement log parser.
+
+    This parser is included to maintain parity with older schemas and datagrams.
+    It is essentially a wrapper around :func:`yadg.parsers.basiccsv.main.process_row`.
+
+    .. admonition:: DEPRECATED in ``yadg-4.0``
+
+        For new applications, please use the :mod:`~yadg.parsers.basiccsv` parser.
+
+    Parameters
+    ----------
+    fn
+        File to process
+
+    encoding
+        Encoding of ``fn``, by default "utf-8".
+
+    timezone
+        A string description of the timezone. Default is "localtime".
+
+    parameters
+        Parameters for :class:`~dgbowl_schemas.yadg.dataschema_5_0.step.MeasCSV`.
+
+    Returns
+    -------
+    :class:`xarray.Dataset`
+        A :class:`xarray.Dataset` containing the timesteps, metadata, and full date tag. No
+        metadata is returned. The full date is always provided in :mod:`~yadg.parsers.meascsv`
+        compatible files.
+
+    """
+    logger.warning("This parser is deprecated. Please switch to 'basiccsv'.")
+
+    with open(fn, "r", encoding=encoding) as infile:
+        lines = [i.strip() for i in infile.readlines()]
+
+    headers = [i.strip() for i in lines.pop(0).split(";")]
+
+    for hi, header in enumerate(headers):
+        if "/" in header:
+            logger.warning("Replacing '/' for '_' in header '%s'.", header)
+            headers[hi] = header.replace("/", "_")
+
+    _units = [i.strip() for i in lines.pop(0).split(";")]
+    units = {}
+    for h in headers:
+        units[h] = _units.pop(0)
+
+    units = dgutils.sanitize_units(units)
+
+    datecolumns, datefunc, fulldate = dgutils.infer_timestamp_from(
+        spec=parameters.timestamp,
+        timezone=timezone,
+    )
+
+    # Process rows
+    data_vals = {}
+    meta_vals = {"_fn": []}
+    for li, line in enumerate(lines):
+        vals, devs = process_row(
+            headers,
+            line.split(";"),
+            datefunc,
+            datecolumns,
+        )
+        append_dicts(vals, devs, data_vals, meta_vals, fn, li)
+
+    return dicts_to_dataset(data_vals, meta_vals, units, fulldate)
```

### Comparing `yadg-5.0.1/src/yadg/parsers/qftrace/__init__.py` & `yadg-5.0.2/src/yadg/parsers/qftrace/__init__.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-"""
-The module handles the reading and processing of the network analyzer
-traces, containing the reflection coefficient as a function of the sweeped frequency,
-:math:`\\Gamma(f)`.
-
-:mod:`~yadg.parsers.qftrace` loads the reflection trace data, determines the
-uncertainties of the signal (y-axis), and explicitly populates the points in
-the time axis (x-axis).
-
-Usage
-`````
-Available since ``yadg-3.0``. The parser supports the following parameters:
-
-.. _yadg.parsers.qftrace.model:
-
-.. autopydantic_model:: dgbowl_schemas.yadg.dataschema_5_0.step.QFTrace
-
-.. _yadg.parsers.qftrace.formats:
-
- - LabView output in a tab-separated format (``csv``):
-   :mod:`~yadg.parsers.qftrace.labviewcsv`
-
-.. _yadg.parsers.qftrace.provides:
-
-Schema
-``````
-For filetypes containing the reflection trace data, the schema is as follows:
-
-.. code-block:: yaml
-
-  datatree.DataTree:
-    S11:
-      coords:
-        uts:        !!float
-        freq:       !!float       # Field frequency (Hz)
-      data_vars:
-        Re(G):      (uts, freq)   # Imaginary part of the reflection coefficient
-        Im(G)       (uts, freq)   # Real part of the reflection coefficient
-        average:    (uts)         # Number of scans averaged to form a single trace
-        bandwidth:  (uts)         # Filter bandwidth (Hz)
-
-Module Functions
-````````````````
-
-"""
-from . import labviewcsv
-import datatree
-
-
-def process(
-    *,
-    filetype: str,
-    **kwargs: dict,
-) -> datatree.DataTree:
-    """
-    VNA reflection trace parser. Forwards ``kwargs`` to the worker functions
-    based on the supplied ``filetype``.
-
-    Parameters
-    ----------
-    filetype
-        Discriminator used to select the appropriate worker function.
-
-    Returns
-    -------
-    :class:`datatree.DataTree`
-
-    """
-    if filetype == "labview.csv":
-        return labviewcsv.process(**kwargs)
+"""
+The module handles the reading and processing of the network analyzer
+traces, containing the reflection coefficient as a function of the sweeped frequency,
+:math:`\\Gamma(f)`.
+
+:mod:`~yadg.parsers.qftrace` loads the reflection trace data, determines the
+uncertainties of the signal (y-axis), and explicitly populates the points in
+the time axis (x-axis).
+
+Usage
+`````
+Available since ``yadg-3.0``. The parser supports the following parameters:
+
+.. _yadg.parsers.qftrace.model:
+
+.. autopydantic_model:: dgbowl_schemas.yadg.dataschema_5_0.step.QFTrace
+
+.. _yadg.parsers.qftrace.formats:
+
+ - LabView output in a tab-separated format (``csv``):
+   :mod:`~yadg.parsers.qftrace.labviewcsv`
+
+.. _yadg.parsers.qftrace.provides:
+
+Schema
+``````
+For filetypes containing the reflection trace data, the schema is as follows:
+
+.. code-block:: yaml
+
+  datatree.DataTree:
+    S11:
+      coords:
+        uts:        !!float
+        freq:       !!float       # Field frequency (Hz)
+      data_vars:
+        Re(G):      (uts, freq)   # Imaginary part of the reflection coefficient
+        Im(G)       (uts, freq)   # Real part of the reflection coefficient
+        average:    (uts)         # Number of scans averaged to form a single trace
+        bandwidth:  (uts)         # Filter bandwidth (Hz)
+
+Module Functions
+````````````````
+
+"""
+from . import labviewcsv
+import datatree
+
+
+def process(
+    *,
+    filetype: str,
+    **kwargs: dict,
+) -> datatree.DataTree:
+    """
+    VNA reflection trace parser. Forwards ``kwargs`` to the worker functions
+    based on the supplied ``filetype``.
+
+    Parameters
+    ----------
+    filetype
+        Discriminator used to select the appropriate worker function.
+
+    Returns
+    -------
+    :class:`datatree.DataTree`
+
+    """
+    if filetype == "labview.csv":
+        return labviewcsv.process(**kwargs)
```

### Comparing `yadg-5.0.1/src/yadg/parsers/qftrace/labviewcsv.py` & `yadg-5.0.2/src/yadg/parsers/qftrace/labviewcsv.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,130 +1,130 @@
-"""
-**labviewcsv**: Processing Agilent LabVIEW CSV files
-----------------------------------------------------
-
-Used to process files generated using Agilent PNA-L N5320C via its LabVIEW driver.
-This file format includes a header, with the values of bandwidth and averaging,
-and three tab-separated columns containing the frequency :math:`f`, and the real
-and imaginary parts of the complex reflection coefficient :math:`\\Gamma(f)`.
-
-Timestamps are determined from file name. One trace per file. As the set-up for
-which this format was designed always uses the ``S11`` port, the name of the trace
-is hard-coded to this value.
-
-.. codeauthor:: Peter Kraus
-"""
-
-from uncertainties.core import str_to_number_with_uncert as tuple_fromstr
-import xarray as xr
-import datatree
-
-
-def process(
-    *,
-    fn: str,
-    encoding: str = "utf-8",
-    **kwargs: dict,
-) -> datatree.DataTree:
-    """
-    VNA reflection trace parser for Agilent's LabVIEW driver.
-
-    Parameters
-    ----------
-    fn
-        File to process
-
-    encoding
-        Encoding of ``fn``, by default "utf-8".
-
-    Returns
-    -------
-    :class:`datatree.DataTree`
-        A :class:`datatree.DataTree` containing a single :class:`xarray.Dataset` with the
-        ``S11`` (reflection) trace.
-
-    """
-
-    with open(fn, "r", encoding=encoding) as infile:
-        lines = infile.readlines()
-    assert (
-        len(lines) > 2
-    ), f"qftrace: Only {len(lines)-1} points supplied in {fn}; fitting impossible."
-
-    # process header
-    bw = [10000.0, 1.0]
-    avg = 15
-    if ";" in lines[0]:
-        items = lines.pop(0).split(";")
-        for item in items:
-            if item.startswith("BW"):
-                bw = tuple_fromstr(item.split("=")[-1].strip())
-            if item.startswith("AVG"):
-                avg = int(item.split("=")[-1].strip())
-    fsbw = bw[0] / avg
-
-    # calculate precision of trace
-    freq = {"vals": [], "devs": []}
-    real = {"vals": [], "devs": []}
-    imag = {"vals": [], "devs": []}
-    for line in lines:
-        f, re, im = line.strip().split()
-        fn, fs = tuple_fromstr(f)
-        fs = max(fs, fsbw)
-        ren, res = tuple_fromstr(re)
-        imn, ims = tuple_fromstr(im)
-        freq["vals"].append(fn)
-        freq["devs"].append(fs)
-        real["vals"].append(ren)
-        real["devs"].append(res)
-        imag["vals"].append(imn)
-        imag["devs"].append(ims)
-
-    vals = xr.Dataset(
-        data_vars={
-            "Re(G)": (
-                ["freq"],
-                real["vals"],
-                {"ancillary_variables": "Re(G)_std_err"},
-            ),
-            "Re(G)_std_err": (
-                ["freq"],
-                real["devs"],
-                {"standard_name": "Re(G) standard_error"},
-            ),
-            "Im(G)": (
-                ["freq"],
-                imag["vals"],
-                {"ancillary_variables": "Im(G)_std_err"},
-            ),
-            "Im(G)_std_err": (
-                ["freq"],
-                imag["devs"],
-                {"standard_name": "Im(G) standard_error"},
-            ),
-            "average": avg,
-            "bandwidth": (
-                [],
-                bw[0],
-                {"units": "Hz", "ancillary_variables": "bandwidth_std_err"},
-            ),
-            "bandwidth_std_err": (
-                [],
-                bw[1],
-                {"units": "Hz", "standard_name": "bandwidth standard_error"},
-            ),
-        },
-        coords={
-            "freq": (
-                ["freq"],
-                freq["vals"],
-                {"units": "Hz", "ancillary_variables": "freq_std_err"},
-            ),
-            "freq_std_err": (
-                ["freq"],
-                freq["devs"],
-                {"units": "Hz", "standard_name": "freq standard_error"},
-            ),
-        },
-    )
-
-    return datatree.DataTree.from_dict(dict(S11=vals))
+"""
+**labviewcsv**: Processing Agilent LabVIEW CSV files
+----------------------------------------------------
+
+Used to process files generated using Agilent PNA-L N5320C via its LabVIEW driver.
+This file format includes a header, with the values of bandwidth and averaging,
+and three tab-separated columns containing the frequency :math:`f`, and the real
+and imaginary parts of the complex reflection coefficient :math:`\\Gamma(f)`.
+
+Timestamps are determined from file name. One trace per file. As the set-up for
+which this format was designed always uses the ``S11`` port, the name of the trace
+is hard-coded to this value.
+
+.. codeauthor:: Peter Kraus
+"""
+
+from uncertainties.core import str_to_number_with_uncert as tuple_fromstr
+import xarray as xr
+import datatree
+
+
+def process(
+    *,
+    fn: str,
+    encoding: str = "utf-8",
+    **kwargs: dict,
+) -> datatree.DataTree:
+    """
+    VNA reflection trace parser for Agilent's LabVIEW driver.
+
+    Parameters
+    ----------
+    fn
+        File to process
+
+    encoding
+        Encoding of ``fn``, by default "utf-8".
+
+    Returns
+    -------
+    :class:`datatree.DataTree`
+        A :class:`datatree.DataTree` containing a single :class:`xarray.Dataset` with the
+        ``S11`` (reflection) trace.
+
+    """
+
+    with open(fn, "r", encoding=encoding) as infile:
+        lines = infile.readlines()
+    assert (
+        len(lines) > 2
+    ), f"qftrace: Only {len(lines)-1} points supplied in {fn}; fitting impossible."
+
+    # process header
+    bw = [10000.0, 1.0]
+    avg = 15
+    if ";" in lines[0]:
+        items = lines.pop(0).split(";")
+        for item in items:
+            if item.startswith("BW"):
+                bw = tuple_fromstr(item.split("=")[-1].strip())
+            if item.startswith("AVG"):
+                avg = int(item.split("=")[-1].strip())
+    fsbw = bw[0] / avg
+
+    # calculate precision of trace
+    freq = {"vals": [], "devs": []}
+    real = {"vals": [], "devs": []}
+    imag = {"vals": [], "devs": []}
+    for line in lines:
+        f, re, im = line.strip().split()
+        fn, fs = tuple_fromstr(f)
+        fs = max(fs, fsbw)
+        ren, res = tuple_fromstr(re)
+        imn, ims = tuple_fromstr(im)
+        freq["vals"].append(fn)
+        freq["devs"].append(fs)
+        real["vals"].append(ren)
+        real["devs"].append(res)
+        imag["vals"].append(imn)
+        imag["devs"].append(ims)
+
+    vals = xr.Dataset(
+        data_vars={
+            "Re(G)": (
+                ["freq"],
+                real["vals"],
+                {"ancillary_variables": "Re(G)_std_err"},
+            ),
+            "Re(G)_std_err": (
+                ["freq"],
+                real["devs"],
+                {"standard_name": "Re(G) standard_error"},
+            ),
+            "Im(G)": (
+                ["freq"],
+                imag["vals"],
+                {"ancillary_variables": "Im(G)_std_err"},
+            ),
+            "Im(G)_std_err": (
+                ["freq"],
+                imag["devs"],
+                {"standard_name": "Im(G) standard_error"},
+            ),
+            "average": avg,
+            "bandwidth": (
+                [],
+                bw[0],
+                {"units": "Hz", "ancillary_variables": "bandwidth_std_err"},
+            ),
+            "bandwidth_std_err": (
+                [],
+                bw[1],
+                {"units": "Hz", "standard_name": "bandwidth standard_error"},
+            ),
+        },
+        coords={
+            "freq": (
+                ["freq"],
+                freq["vals"],
+                {"units": "Hz", "ancillary_variables": "freq_std_err"},
+            ),
+            "freq_std_err": (
+                ["freq"],
+                freq["devs"],
+                {"units": "Hz", "standard_name": "freq standard_error"},
+            ),
+        },
+    )
+
+    return datatree.DataTree.from_dict(dict(S11=vals))
```

### Comparing `yadg-5.0.1/src/yadg/parsers/xpstrace/__init__.py` & `yadg-5.0.2/src/yadg/parsers/xpstrace/__init__.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-"""
-This module handles the reading and processing of X-ray photoelectron spectroscopy
-data, including determining the uncertainties of the signal (y-axis), and explicitly
-populating the points in the energy axis (``E``).
-
-Usage
-`````
-Available since ``yadg-4.1``. The parser supports the following parameters:
-
-.. _yadg.parsers.xpstrace.model:
-
-.. autopydantic_model:: dgbowl_schemas.yadg.dataschema_5_0.step.XPSTrace
-
-.. _yadg.parsers.xpstrace.formats:
-
-Formats
-```````
-The ``filetypes`` currently supported by the parser are:
-
- - ULVAC PHI Multipak XPS traces (``phi.spe``),
-   see :mod:`~yadg.parsers.xpstrace.phispe`
-
-.. _yadg.parsers.xpstrace.provides:
-
-Provides
-````````
-The raw data is stored, for each timestep, using the following format:
-
-.. code-block:: yaml
-
-  datatree.DataTree:
-    {{ trace_name }}      !!xr.Dataset
-      coords:
-        uts:              !!float
-        E:                !!float      # binding energies (eV)
-      data_vals:
-        y:                (uts, E)     # signal
-
-Module Functions
-````````````````
-
-"""
-import datatree
-from . import phispe
-
-
-def process(
-    *,
-    filetype: str,
-    **kwargs: dict,
-) -> datatree.DataTree:
-    """
-    Unified x-ray photoelectron spectroscopy parser. Forwards ``kwargs`` to the worker
-    functions based on the supplied ``filetype``.
-
-    This parser processes XPS scans in signal(energy) format.
-
-    Parameters
-    ----------
-    filetype
-        Discriminator used to select the appropriate worker function.
-
-    Returns
-    -------
-    :class:`datatree.DataTree`
-
-    """
-    if filetype == "phi.spe":
-        return phispe.process(**kwargs)
+"""
+This module handles the reading and processing of X-ray photoelectron spectroscopy
+data, including determining the uncertainties of the signal (y-axis), and explicitly
+populating the points in the energy axis (``E``).
+
+Usage
+`````
+Available since ``yadg-4.1``. The parser supports the following parameters:
+
+.. _yadg.parsers.xpstrace.model:
+
+.. autopydantic_model:: dgbowl_schemas.yadg.dataschema_5_0.step.XPSTrace
+
+.. _yadg.parsers.xpstrace.formats:
+
+Formats
+```````
+The ``filetypes`` currently supported by the parser are:
+
+ - ULVAC PHI Multipak XPS traces (``phi.spe``),
+   see :mod:`~yadg.parsers.xpstrace.phispe`
+
+.. _yadg.parsers.xpstrace.provides:
+
+Provides
+````````
+The raw data is stored, for each timestep, using the following format:
+
+.. code-block:: yaml
+
+  datatree.DataTree:
+    {{ trace_name }}      !!xr.Dataset
+      coords:
+        uts:              !!float
+        E:                !!float      # binding energies (eV)
+      data_vals:
+        y:                (uts, E)     # signal
+
+Module Functions
+````````````````
+
+"""
+import datatree
+from . import phispe
+
+
+def process(
+    *,
+    filetype: str,
+    **kwargs: dict,
+) -> datatree.DataTree:
+    """
+    Unified x-ray photoelectron spectroscopy parser. Forwards ``kwargs`` to the worker
+    functions based on the supplied ``filetype``.
+
+    This parser processes XPS scans in signal(energy) format.
+
+    Parameters
+    ----------
+    filetype
+        Discriminator used to select the appropriate worker function.
+
+    Returns
+    -------
+    :class:`datatree.DataTree`
+
+    """
+    if filetype == "phi.spe":
+        return phispe.process(**kwargs)
```

### Comparing `yadg-5.0.1/src/yadg/parsers/xpstrace/phispe.py` & `yadg-5.0.2/src/yadg/parsers/xpstrace/phispe.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,375 +1,375 @@
-"""
-**phispe**: Processing of ULVAC PHI Multipak XPS traces.
---------------------------------------------------------
-
-The `IGOR .spe import script by jjweimer <https://www.wavemetrics.com/project/phispefileloader>`_
-was pretty helpful for writing this parser.
-
-File Structure of ``.spe`` Files
-````````````````````````````````
-
-These binary files actually contain an ASCII file header, delimited by
-`"SOFH\n"` and `"EOFH\n"`.
-
-The binding energies corresponding to the datapoints in the later part
-of the file can be found from the `"SpectralRegDef"` entries in this
-header. Each of these entries look something like:
-
-.. code-block::
-
-    2 2 F1s 9 161 -0.1250 695.0 675.0 695.0 680.0    0.160000 29.35 AREA
-
-This maps as follows:
-
-.. code-block::
-
-    2           trace_number
-    2           trace_number (again?)
-    F1s         name
-    9           atomic_number
-    161         num_datapoints
-    -0.1250     step
-    695.0       start
-    675.0       stop
-    695.0       ?
-    680.0       ?
-    0.160000    dwell_time
-    29.35       e_pass
-    AREA        description (?)
-
-After the file header, the binary part starts with a short data header
-(offsets given from start of data header):
-
-.. code-block::
-
-    0x0000 group                # Data group number.
-    0x0004 num_traces           # Number of traces in file
-    0x0008 trace_header_size    # Combined lengths of all trace headers.
-    0x000c data_header_size     # Length of this data header.
-
-After this follow ``num_traces`` trace headers that are each structured
-something like this:
-
-.. code-block::
-
-    0x0000 trace_number          # Number of the trace.
-    0x0004 bool_01               # ???
-    0x0008 bool_02               # ???
-    0x000c trace_number_again    # Number of the trace. Again?
-    0x0010 bool_03               # ???
-    0x0014 num_datapoints        # Number of datapoints in trace.
-    0x0018 bool_04               # ???
-    0x001c bool_05               # ???
-    0x0020 string_01             # ???
-    0x0024 string_02             # ???
-    0x0028 string_03             # ???
-    0x002c int_02                # ???
-    0x0030 string_04             # ???
-    0x0034 string_05             # ???
-    0x0038 y_unit                # The unit of the datapoints.
-    0x003c int_05                # ???
-    0x0040 int_06                # ???
-    0x0044 int_07                # ???
-    0x0048 data_dtype            # Data type for datapoints (f4 / f8).
-    0x004c num_data_bytes        # Unsure about this one.
-    0x0050 num_datapoints_tot    # This one as well.
-    0x0054 int_10                # ???
-    0x0058 int_11                # ???
-    0x005c end_of_data           # Byte offset of the end-of-data.
-
-After the trace headers follow the datapoints. After the number of
-datapoints there is a single 32bit float with the trace's dwelling time
-again.
-
-Uncertainties
-`````````````
-The uncertainties of ``"E"`` are taken as the step-width of
-the linearly spaced energy values.
-
-The uncertainties ``"s"`` of ``"y"`` are currently set to a constant
-value of ``12.5`` counts per second as all the signals in the files seen so
-far only seem to take on values in those steps.
-
-.. admonition:: TODO
-
-    https://github.com/dgbowl/yadg/issues/13
-
-    Determining the uncertainty of the counts per second signal in XPS
-    traces from the phispe parser should be done in a better way.
-
-.. codeauthor:: Nicolas Vetsch
-"""
-
-import re
-import numpy as np
-import xarray as xr
-import datatree
-import yadg.dgutils as dgutils
-
-data_header_dtype = np.dtype(
-    [
-        ("group", "<u4"),
-        ("num_traces", "<u4"),
-        ("trace_header_size", "<u4"),
-        ("data_header_size", "<u4"),
-    ]
-)
-
-trace_header_dtype = np.dtype(
-    [
-        ("trace_number", "<u4"),
-        ("bool_01", "<u4"),
-        ("bool_02", "<u4"),
-        ("trace_number_again", "<u4"),
-        ("bool_03", "<u4"),
-        ("num_datapoints", "<u4"),
-        ("bool_04", "<u4"),
-        ("bool_05", "<u4"),
-        ("string_01", "|S4"),  # pnt?
-        ("string_02", "|S4"),
-        ("string_03", "|S4"),  # sar?
-        ("int_02", "<u4"),
-        ("string_04", "|S4"),
-        ("string_05", "|S4"),
-        ("y_unit", "|S4"),
-        ("int_05", "<u4"),
-        ("int_06", "<u4"),
-        ("int_07", "<u4"),
-        ("data_dtype", "|S4"),
-        ("num_data_bytes", "<u4"),
-        ("num_datapoints_tot", "<u4"),
-        ("int_10", "<u4"),
-        ("int_11", "<u4"),
-        ("end_of_data", "<u4"),
-    ]
-)
-
-
-def camel_to_snake(s: str) -> str:
-    """Converts CamelCase strings to snake_case.
-
-    From https://stackoverflow.com/a/1176023
-
-    Parameters
-    ----------
-    s
-        The CamelCase input string.
-
-    Returns
-    -------
-    str
-        The snake_case equivalent of s.
-
-    """
-    s = re.sub(r"(.)([A-Z][a-z]+)", r"\1_\2", s)
-    return re.sub(r"([a-z0-9])([A-Z])", r"\1_\2", s).lower()
-
-
-def _process_header(spe: list[bytes]) -> dict:
-    """Processes the file header at the top of `.spe` files.
-
-    Parameters
-    ----------
-    spe
-        The lines of bytes read from file.
-
-    Returns
-    -------
-    dict
-        The file header parsed into a dictionary. Some entries (keys)
-        occur more than once. The corresponding values are joined into
-        a list.
-
-    """
-    header_lines = spe[spe.index(b"SOFH\n") + 1 : spe.index(b"EOFH\n")]
-    header = {}
-    for line in header_lines:
-        key, value = line.split(b":")
-        key, value = camel_to_snake(key.decode().strip()), value.decode().strip()
-        if key in header:
-            header[key] = [header[key]] + [value]
-        else:
-            header[key] = value
-    return header
-
-
-def _process_trace_defs(header: dict) -> list[dict]:
-    """Processes the trace definition strings given in the file header.
-
-    These strings look something like the following:
-    `2 2 F1s 9 161 -0.1250 695.0 675.0 695.0 680.0    0.160000 29.35 AREA`
-
-    Parameters
-    ----------
-    header
-        The file header parsed into a dictionary. The "SpectralRegDef"
-        entry contains a list of trace definition strings.
-
-    Returns
-    -------
-    list[dict]
-        A list of trace definition dictionaries describind the kind of
-        trace and the binding energy ranges.
-
-    """
-    trace_defs = []
-    for trace_def in header.get("spectral_reg_def"):
-        trace_def = trace_def.split()
-        trace_defs.append(
-            {
-                "trace_number": int(trace_def[0]),
-                "name": trace_def[2],
-                "atomic_number": trace_def[3],
-                "num_datapoints": int(trace_def[4]),
-                "step": float(trace_def[5]),
-                "start": float(trace_def[6]),
-                "stop": float(trace_def[7]),
-                "dwell_time": trace_def[10],
-                "e_pass": trace_def[11],
-                "description": trace_def[12],
-            }
-        )
-    return trace_defs
-
-
-def _process_traces(spe: list[bytes], trace_defs: list[dict]) -> dict:
-    """Processes the spectral traces in the file.
-
-    Parameters
-    ----------
-    spe
-        The lines of bytes read from file.
-
-    trace_defs
-        The list of trace definitions parsed from the file header.
-
-    Returns
-    -------
-    dict
-        A dictionary containing the binding energies constructed from
-        the trace definitions and the corrresponding XPS traces.
-
-    """
-    data = b"".join(spe[spe.index(b"EOFH\n") + 1 :])
-    data_header = dgutils.read_value(data, 0x0000, data_header_dtype)
-    assert data_header["num_traces"] == len(trace_defs)
-    # All trace headers I have seen are 192 (0xc0) bytes long.
-    assert data_header["trace_header_size"] / trace_header_dtype.itemsize == len(
-        trace_defs
-    )
-    assert data_header["data_header_size"] == data_header_dtype.itemsize
-    trace_headers = np.frombuffer(
-        data,
-        offset=0x0010,
-        dtype=trace_header_dtype,
-        count=len(trace_defs),
-    )
-    traces = {}
-    for trace_header, trace_def in zip(trace_headers, trace_defs):
-        assert trace_header["trace_number"] == trace_def["trace_number"]
-        assert trace_header["num_datapoints"] == trace_def["num_datapoints"]
-        # Contruct the binding energies from trace_def.
-        energies, dE = np.linspace(
-            trace_def["start"],
-            trace_def["stop"],
-            trace_def["num_datapoints"],
-            endpoint=True,
-            retstep=True,
-        )
-        # Construct data from trace_header
-        data_dtype = np.dtype(f'{trace_header["data_dtype"].decode()}')
-        data_offset = trace_header["end_of_data"] - trace_header["num_data_bytes"]
-        datapoints = np.frombuffer(
-            data,
-            offset=data_offset,
-            dtype=data_dtype,
-            count=trace_header["num_datapoints"],
-        )
-        dwell_time = dgutils.read_value(data, trace_header["end_of_data"], "<f4")
-        np.testing.assert_almost_equal(dwell_time, float(trace_def["dwell_time"]))
-        # TODO: Figure out the correct error. This signal count should
-        # somehow be a Poisson distribution, i.e. the error should be
-        # something like s ~ sqrt(n). The counts per second only seem to
-        # be taking values in steps of 12.5cps, so taking this as error.
-        traces[str(trace_def["trace_number"])] = {
-            "name": trace_def["name"],
-            "atomic_number": trace_def["atomic_number"],
-            "dwell_time": trace_def["dwell_time"],
-            "e_pass": trace_def["e_pass"],
-            "description": trace_def["description"],
-            "yvals": datapoints,
-            "ydevs": np.ones(len(datapoints)) * 12.5,
-            "yunit": "counts / s",
-            "Evals": energies,
-            "Edevs": np.ones(len(energies)) * abs(dE),
-            "Eunit": "eV",
-        }
-    return traces
-
-
-def process(
-    *,
-    fn: str,
-    **kwargs: dict,
-) -> datatree.DataTree:
-    """Processes ULVAC-PHI Multipak XPS data.
-
-    Parameters
-    ----------
-    fn
-        The file containing the data to parse.
-
-    Returns
-    -------
-    :class:`datatree.DataTree`
-        Returns a :class:`datatree.DataTree` containing a :class:`xarray.Dataset` for each
-        XPS trace present in the input file.
-
-    """
-    with open(fn, "rb") as spe_file:
-        spe = spe_file.readlines()
-    header = _process_header(spe)
-    software_id, version = header.get("software_version").split()
-    meta = {
-        "params": {
-            "software_id": software_id,
-            "version": version,
-            "username": header.get("operator"),
-        },
-        "file_header": header,
-    }
-    trace_defs = _process_trace_defs(header)
-    traces = _process_traces(spe, trace_defs)
-    vals = {}
-    for v in traces.values():
-        fvals = xr.Dataset(
-            data_vars={
-                "y": (
-                    ["E"],
-                    v["yvals"],
-                    {"units": v["yunit"], "ancillary_variables": "y_std_err"},
-                ),
-                "y_std_err": (
-                    ["E"],
-                    v["ydevs"],
-                    {"units": v["yunit"], "standard_name": "y standard_error"},
-                ),
-                "E_std_err": (
-                    ["E"],
-                    v["Edevs"],
-                    {"units": v["Eunit"], "standard_name": "E standard_error"},
-                ),
-            },
-            coords={
-                "E": (
-                    ["E"],
-                    v["Evals"],
-                    {"units": v["Eunit"], "ancillary_variables": "E_std_err"},
-                ),
-            },
-        )
-        vals[v["name"]] = fvals
-
-    dt = datatree.DataTree.from_dict(vals)
-    dt.attrs = meta
-    return dt
+"""
+**phispe**: Processing of ULVAC PHI Multipak XPS traces.
+--------------------------------------------------------
+
+The `IGOR .spe import script by jjweimer <https://www.wavemetrics.com/project/phispefileloader>`_
+was pretty helpful for writing this parser.
+
+File Structure of ``.spe`` Files
+````````````````````````````````
+
+These binary files actually contain an ASCII file header, delimited by
+`"SOFH\n"` and `"EOFH\n"`.
+
+The binding energies corresponding to the datapoints in the later part
+of the file can be found from the `"SpectralRegDef"` entries in this
+header. Each of these entries look something like:
+
+.. code-block::
+
+    2 2 F1s 9 161 -0.1250 695.0 675.0 695.0 680.0    0.160000 29.35 AREA
+
+This maps as follows:
+
+.. code-block::
+
+    2           trace_number
+    2           trace_number (again?)
+    F1s         name
+    9           atomic_number
+    161         num_datapoints
+    -0.1250     step
+    695.0       start
+    675.0       stop
+    695.0       ?
+    680.0       ?
+    0.160000    dwell_time
+    29.35       e_pass
+    AREA        description (?)
+
+After the file header, the binary part starts with a short data header
+(offsets given from start of data header):
+
+.. code-block::
+
+    0x0000 group                # Data group number.
+    0x0004 num_traces           # Number of traces in file
+    0x0008 trace_header_size    # Combined lengths of all trace headers.
+    0x000c data_header_size     # Length of this data header.
+
+After this follow ``num_traces`` trace headers that are each structured
+something like this:
+
+.. code-block::
+
+    0x0000 trace_number          # Number of the trace.
+    0x0004 bool_01               # ???
+    0x0008 bool_02               # ???
+    0x000c trace_number_again    # Number of the trace. Again?
+    0x0010 bool_03               # ???
+    0x0014 num_datapoints        # Number of datapoints in trace.
+    0x0018 bool_04               # ???
+    0x001c bool_05               # ???
+    0x0020 string_01             # ???
+    0x0024 string_02             # ???
+    0x0028 string_03             # ???
+    0x002c int_02                # ???
+    0x0030 string_04             # ???
+    0x0034 string_05             # ???
+    0x0038 y_unit                # The unit of the datapoints.
+    0x003c int_05                # ???
+    0x0040 int_06                # ???
+    0x0044 int_07                # ???
+    0x0048 data_dtype            # Data type for datapoints (f4 / f8).
+    0x004c num_data_bytes        # Unsure about this one.
+    0x0050 num_datapoints_tot    # This one as well.
+    0x0054 int_10                # ???
+    0x0058 int_11                # ???
+    0x005c end_of_data           # Byte offset of the end-of-data.
+
+After the trace headers follow the datapoints. After the number of
+datapoints there is a single 32bit float with the trace's dwelling time
+again.
+
+Uncertainties
+`````````````
+The uncertainties of ``"E"`` are taken as the step-width of
+the linearly spaced energy values.
+
+The uncertainties ``"s"`` of ``"y"`` are currently set to a constant
+value of ``12.5`` counts per second as all the signals in the files seen so
+far only seem to take on values in those steps.
+
+.. admonition:: TODO
+
+    https://github.com/dgbowl/yadg/issues/13
+
+    Determining the uncertainty of the counts per second signal in XPS
+    traces from the phispe parser should be done in a better way.
+
+.. codeauthor:: Nicolas Vetsch
+"""
+
+import re
+import numpy as np
+import xarray as xr
+import datatree
+import yadg.dgutils as dgutils
+
+data_header_dtype = np.dtype(
+    [
+        ("group", "<u4"),
+        ("num_traces", "<u4"),
+        ("trace_header_size", "<u4"),
+        ("data_header_size", "<u4"),
+    ]
+)
+
+trace_header_dtype = np.dtype(
+    [
+        ("trace_number", "<u4"),
+        ("bool_01", "<u4"),
+        ("bool_02", "<u4"),
+        ("trace_number_again", "<u4"),
+        ("bool_03", "<u4"),
+        ("num_datapoints", "<u4"),
+        ("bool_04", "<u4"),
+        ("bool_05", "<u4"),
+        ("string_01", "|S4"),  # pnt?
+        ("string_02", "|S4"),
+        ("string_03", "|S4"),  # sar?
+        ("int_02", "<u4"),
+        ("string_04", "|S4"),
+        ("string_05", "|S4"),
+        ("y_unit", "|S4"),
+        ("int_05", "<u4"),
+        ("int_06", "<u4"),
+        ("int_07", "<u4"),
+        ("data_dtype", "|S4"),
+        ("num_data_bytes", "<u4"),
+        ("num_datapoints_tot", "<u4"),
+        ("int_10", "<u4"),
+        ("int_11", "<u4"),
+        ("end_of_data", "<u4"),
+    ]
+)
+
+
+def camel_to_snake(s: str) -> str:
+    """Converts CamelCase strings to snake_case.
+
+    From https://stackoverflow.com/a/1176023
+
+    Parameters
+    ----------
+    s
+        The CamelCase input string.
+
+    Returns
+    -------
+    str
+        The snake_case equivalent of s.
+
+    """
+    s = re.sub(r"(.)([A-Z][a-z]+)", r"\1_\2", s)
+    return re.sub(r"([a-z0-9])([A-Z])", r"\1_\2", s).lower()
+
+
+def _process_header(spe: list[bytes]) -> dict:
+    """Processes the file header at the top of `.spe` files.
+
+    Parameters
+    ----------
+    spe
+        The lines of bytes read from file.
+
+    Returns
+    -------
+    dict
+        The file header parsed into a dictionary. Some entries (keys)
+        occur more than once. The corresponding values are joined into
+        a list.
+
+    """
+    header_lines = spe[spe.index(b"SOFH\n") + 1 : spe.index(b"EOFH\n")]
+    header = {}
+    for line in header_lines:
+        key, value = line.split(b":")
+        key, value = camel_to_snake(key.decode().strip()), value.decode().strip()
+        if key in header:
+            header[key] = [header[key]] + [value]
+        else:
+            header[key] = value
+    return header
+
+
+def _process_trace_defs(header: dict) -> list[dict]:
+    """Processes the trace definition strings given in the file header.
+
+    These strings look something like the following:
+    `2 2 F1s 9 161 -0.1250 695.0 675.0 695.0 680.0    0.160000 29.35 AREA`
+
+    Parameters
+    ----------
+    header
+        The file header parsed into a dictionary. The "SpectralRegDef"
+        entry contains a list of trace definition strings.
+
+    Returns
+    -------
+    list[dict]
+        A list of trace definition dictionaries describind the kind of
+        trace and the binding energy ranges.
+
+    """
+    trace_defs = []
+    for trace_def in header.get("spectral_reg_def"):
+        trace_def = trace_def.split()
+        trace_defs.append(
+            {
+                "trace_number": int(trace_def[0]),
+                "name": trace_def[2],
+                "atomic_number": trace_def[3],
+                "num_datapoints": int(trace_def[4]),
+                "step": float(trace_def[5]),
+                "start": float(trace_def[6]),
+                "stop": float(trace_def[7]),
+                "dwell_time": trace_def[10],
+                "e_pass": trace_def[11],
+                "description": trace_def[12],
+            }
+        )
+    return trace_defs
+
+
+def _process_traces(spe: list[bytes], trace_defs: list[dict]) -> dict:
+    """Processes the spectral traces in the file.
+
+    Parameters
+    ----------
+    spe
+        The lines of bytes read from file.
+
+    trace_defs
+        The list of trace definitions parsed from the file header.
+
+    Returns
+    -------
+    dict
+        A dictionary containing the binding energies constructed from
+        the trace definitions and the corrresponding XPS traces.
+
+    """
+    data = b"".join(spe[spe.index(b"EOFH\n") + 1 :])
+    data_header = dgutils.read_value(data, 0x0000, data_header_dtype)
+    assert data_header["num_traces"] == len(trace_defs)
+    # All trace headers I have seen are 192 (0xc0) bytes long.
+    assert data_header["trace_header_size"] / trace_header_dtype.itemsize == len(
+        trace_defs
+    )
+    assert data_header["data_header_size"] == data_header_dtype.itemsize
+    trace_headers = np.frombuffer(
+        data,
+        offset=0x0010,
+        dtype=trace_header_dtype,
+        count=len(trace_defs),
+    )
+    traces = {}
+    for trace_header, trace_def in zip(trace_headers, trace_defs):
+        assert trace_header["trace_number"] == trace_def["trace_number"]
+        assert trace_header["num_datapoints"] == trace_def["num_datapoints"]
+        # Contruct the binding energies from trace_def.
+        energies, dE = np.linspace(
+            trace_def["start"],
+            trace_def["stop"],
+            trace_def["num_datapoints"],
+            endpoint=True,
+            retstep=True,
+        )
+        # Construct data from trace_header
+        data_dtype = np.dtype(f'{trace_header["data_dtype"].decode()}')
+        data_offset = trace_header["end_of_data"] - trace_header["num_data_bytes"]
+        datapoints = np.frombuffer(
+            data,
+            offset=data_offset,
+            dtype=data_dtype,
+            count=trace_header["num_datapoints"],
+        )
+        dwell_time = dgutils.read_value(data, trace_header["end_of_data"], "<f4")
+        np.testing.assert_almost_equal(dwell_time, float(trace_def["dwell_time"]))
+        # TODO: Figure out the correct error. This signal count should
+        # somehow be a Poisson distribution, i.e. the error should be
+        # something like s ~ sqrt(n). The counts per second only seem to
+        # be taking values in steps of 12.5cps, so taking this as error.
+        traces[str(trace_def["trace_number"])] = {
+            "name": trace_def["name"],
+            "atomic_number": trace_def["atomic_number"],
+            "dwell_time": trace_def["dwell_time"],
+            "e_pass": trace_def["e_pass"],
+            "description": trace_def["description"],
+            "yvals": datapoints,
+            "ydevs": np.ones(len(datapoints)) * 12.5,
+            "yunit": "counts / s",
+            "Evals": energies,
+            "Edevs": np.ones(len(energies)) * abs(dE),
+            "Eunit": "eV",
+        }
+    return traces
+
+
+def process(
+    *,
+    fn: str,
+    **kwargs: dict,
+) -> datatree.DataTree:
+    """Processes ULVAC-PHI Multipak XPS data.
+
+    Parameters
+    ----------
+    fn
+        The file containing the data to parse.
+
+    Returns
+    -------
+    :class:`datatree.DataTree`
+        Returns a :class:`datatree.DataTree` containing a :class:`xarray.Dataset` for each
+        XPS trace present in the input file.
+
+    """
+    with open(fn, "rb") as spe_file:
+        spe = spe_file.readlines()
+    header = _process_header(spe)
+    software_id, version = header.get("software_version").split()
+    meta = {
+        "params": {
+            "software_id": software_id,
+            "version": version,
+            "username": header.get("operator"),
+        },
+        "file_header": header,
+    }
+    trace_defs = _process_trace_defs(header)
+    traces = _process_traces(spe, trace_defs)
+    vals = {}
+    for v in traces.values():
+        fvals = xr.Dataset(
+            data_vars={
+                "y": (
+                    ["E"],
+                    v["yvals"],
+                    {"units": v["yunit"], "ancillary_variables": "y_std_err"},
+                ),
+                "y_std_err": (
+                    ["E"],
+                    v["ydevs"],
+                    {"units": v["yunit"], "standard_name": "y standard_error"},
+                ),
+                "E_std_err": (
+                    ["E"],
+                    v["Edevs"],
+                    {"units": v["Eunit"], "standard_name": "E standard_error"},
+                ),
+            },
+            coords={
+                "E": (
+                    ["E"],
+                    v["Evals"],
+                    {"units": v["Eunit"], "ancillary_variables": "E_std_err"},
+                ),
+            },
+        )
+        vals[v["name"]] = fvals
+
+    dt = datatree.DataTree.from_dict(vals)
+    dt.attrs = meta
+    return dt
```

### Comparing `yadg-5.0.1/src/yadg/parsers/xrdtrace/__init__.py` & `yadg-5.0.2/src/yadg/parsers/xrdtrace/__init__.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,74 +1,74 @@
-"""
-This module handles the reading and processing of X-ray diffraction data. It loads X-ray
-diffraction data, determines reasonable uncertainties of the signal intensity (y-axis),
-and explicitly populates the angle axis (:math:`2\\theta`), if necessary.
-
-Usage
-`````
-Available since ``yadg-4.0``. The parser supports the following parameters:
-
-.. _yadg.parsers.xrdtrace.model:
-
-.. autopydantic_model:: dgbowl_schemas.yadg.dataschema_5_0.step.XRDTrace
-
-.. _yadg.parsers.xrdtrace.formats:
-
-Formats
-```````
-The ``filetypes`` currently supported by the parser are:
-
- - PANalytical ``xrdml`` files (``panalytical.xrdml``),
-   see :mod:`~yadg.parsers.xrdtrace.panalyticalxrdml`
- - PANalytical ``csv`` files (``panalytical.csv``),
-   see :mod:`~yadg.parsers.xrdtrace.panalyticalcsv`
- - PANalytical ``xy`` files (``panalytical.xy``),
-   see :mod:`~yadg.parsers.xrdtrace.panalyticalxy`
-
-.. _yadg.parsers.xrdtrace.provides:
-
-Provides
-````````
-The raw data is stored, for each timestep, using the following format:
-
-.. code-block:: yaml
-
-  xr.Dataset:
-    coords:
-      uts:         !!float
-      angle:       !!float            # Diffraction angle (deg)
-    data_vals:
-      intensity:   (uts, angle)       # Detector intensity (counts)
-
-"""
-import xarray as xr
-from . import panalyticalxrdml, panalyticalcsv, panalyticalxy
-
-
-def process(
-    *,
-    filetype: str,
-    **kwargs: dict,
-) -> xr.Dataset:
-    """
-    Unified X-ray diffractogram data parser. Forwards ``kwargs`` to the worker
-    functions based on the supplied ``filetype``.
-
-    This parser processes XPS scans in signal(energy) format.
-
-    Parameters
-    ----------
-    filetype
-        Discriminator used to select the appropriate worker function.
-
-    Returns
-    -------
-    :class:`xarray.Dataset`
-
-
-    """
-    if filetype == "panalytical.xrdml":
-        return panalyticalxrdml.process(**kwargs)
-    elif filetype == "panalytical.csv":
-        return panalyticalcsv.process(**kwargs)
-    elif filetype == "panalytical.xy":
-        return panalyticalxy.process(**kwargs)
+"""
+This module handles the reading and processing of X-ray diffraction data. It loads X-ray
+diffraction data, determines reasonable uncertainties of the signal intensity (y-axis),
+and explicitly populates the angle axis (:math:`2\\theta`), if necessary.
+
+Usage
+`````
+Available since ``yadg-4.0``. The parser supports the following parameters:
+
+.. _yadg.parsers.xrdtrace.model:
+
+.. autopydantic_model:: dgbowl_schemas.yadg.dataschema_5_0.step.XRDTrace
+
+.. _yadg.parsers.xrdtrace.formats:
+
+Formats
+```````
+The ``filetypes`` currently supported by the parser are:
+
+ - PANalytical ``xrdml`` files (``panalytical.xrdml``),
+   see :mod:`~yadg.parsers.xrdtrace.panalyticalxrdml`
+ - PANalytical ``csv`` files (``panalytical.csv``),
+   see :mod:`~yadg.parsers.xrdtrace.panalyticalcsv`
+ - PANalytical ``xy`` files (``panalytical.xy``),
+   see :mod:`~yadg.parsers.xrdtrace.panalyticalxy`
+
+.. _yadg.parsers.xrdtrace.provides:
+
+Provides
+````````
+The raw data is stored, for each timestep, using the following format:
+
+.. code-block:: yaml
+
+  xr.Dataset:
+    coords:
+      uts:         !!float
+      angle:       !!float            # Diffraction angle (deg)
+    data_vals:
+      intensity:   (uts, angle)       # Detector intensity (counts)
+
+"""
+import xarray as xr
+from . import panalyticalxrdml, panalyticalcsv, panalyticalxy
+
+
+def process(
+    *,
+    filetype: str,
+    **kwargs: dict,
+) -> xr.Dataset:
+    """
+    Unified X-ray diffractogram data parser. Forwards ``kwargs`` to the worker
+    functions based on the supplied ``filetype``.
+
+    This parser processes XPS scans in signal(energy) format.
+
+    Parameters
+    ----------
+    filetype
+        Discriminator used to select the appropriate worker function.
+
+    Returns
+    -------
+    :class:`xarray.Dataset`
+
+
+    """
+    if filetype == "panalytical.xrdml":
+        return panalyticalxrdml.process(**kwargs)
+    elif filetype == "panalytical.csv":
+        return panalyticalcsv.process(**kwargs)
+    elif filetype == "panalytical.xy":
+        return panalyticalxy.process(**kwargs)
```

### Comparing `yadg-5.0.1/src/yadg/parsers/xrdtrace/panalyticalcsv.py` & `yadg-5.0.2/src/yadg/parsers/xrdtrace/panalyticalcsv.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,170 +1,170 @@
-"""
-panalyticalcsv: Processing of PANalytical XRD ``csv`` files
------------------------------------------------------------
-
-File Structure
-``````````````
-
-These files are split into a ``[Measurement conditions]`` and a ``[Scan points]``
-section. The former stores the metadata and the latter all the datapoints.
-
-Uncertainties
-`````````````
-The uncertainties of ``"angle"`` are taken from the number of significant figures.
-
-The uncertainties of ``"intensity"`` are taken from the number of significant figures.
-
-.. codeauthor::
-    Nicolas Vetsch,
-    Peter Kraus
-"""
-
-from ...dgutils import dateutils
-from .common import panalytical_comment, snake_case
-from uncertainties.core import str_to_number_with_uncert as tuple_fromstr
-import xarray as xr
-import numpy as np
-
-# Converting camelCase xrdml keys to snake_case.
-
-
-def _process_comments(comments: list[str]) -> dict:
-    ret = {}
-    for line in comments:
-        ret.update(panalytical_comment(line))
-    return ret
-
-
-def _process_header(header: str) -> dict:
-    """
-    Processes the header section, staring with the ``[Measurement conditions]`` line.
-
-    Parameters
-    ----------
-    header
-        The header portion as a string.
-
-    Returns
-    -------
-    header: dict
-        A dictionary containing the processed metadata.
-
-    """
-    header_lines = header.split("\n")[1:-1]
-    header = dict([line.split(",", 1) for line in header_lines])
-    # Process comment entries.
-    comments = []
-    for key in list(header.keys()):
-        if key.startswith("Comment"):
-            comments.append(header.pop(key).strip('"'))
-    comments = _process_comments(comments)
-    # Renaming the keys.
-    for key in list(header.keys()):
-        header[snake_case(key)] = header.pop(key)
-    header.update(comments)
-    return header
-
-
-def _process_data(data: str) -> tuple[list, list]:
-    """
-    Processes the data section, starting with the ``[Scan points]`` line.
-
-    Parameters
-    ----------
-    data
-        The data portion as a string.
-
-    Returns
-    -------
-    avals, adevs, ivals, idevs
-        The values and uncertainties in angle and intensity.
-
-    """
-    data_lines = data.split("\n")[1:-1]
-    columns = data_lines[0].split(",")
-    assert columns == ["Angle", "Intensity"], "Unexpected columns."
-    datapoints = [line.split(",") for line in data_lines[1:]]
-    angle, intensity = [list(d) for d in zip(*datapoints)]
-    avals, adevs = list(zip(*[tuple_fromstr(a) for a in angle]))
-    ivals, idevs = list(zip(*[tuple_fromstr(i) for i in intensity]))
-    return avals, adevs, ivals, idevs
-
-
-def process(
-    *,
-    fn: str,
-    encoding: str = "utf-8",
-    timezone: str = "UTC",
-    **kwargs: dict,
-) -> xr.Dataset:
-    """
-    Processes a PANalytical XRD csv file. All information contained in the header
-    of the csv file is stored in the metadata.
-
-    Parameters
-    ----------
-    fn
-        The file containing the trace(s) to parse.
-
-    encoding
-        Encoding of ``fn``, by default "utf-8".
-
-    timezone
-        A string description of the timezone. Default is "UTC".
-
-    Returns
-    -------
-    :class:`xarray.Dataset`
-        Data containing the timesteps and metadata. This filetype contains the full
-        date specification.
-
-    """
-    with open(fn, "r", encoding=encoding) as csv_file:
-        csv = csv_file.read()
-    # Split file into its sections.
-    __, header, data = csv.split("[")
-    assert header.startswith("Measurement conditions"), "Unexpected section."
-    assert data.startswith("Scan points"), "Unexpected section."
-    header = _process_header(header)
-    # Process the data trace.
-    angle, _, insty, _ = _process_data(data)
-    adiff = np.abs(np.diff(angle)) * 0.5
-    adiff = np.append(adiff, adiff[-1])
-    idevs = np.ones(len(insty))
-    # Process the metadata.
-    uts = dateutils.str_to_uts(
-        timestamp=header["file_date_and_time"],
-        format="%d/%B/%Y %H:%M",
-        timezone=timezone,
-    )
-    header["fulldate"] = True
-    # Build Datasets
-    vals = xr.Dataset(
-        data_vars={
-            "intensity": (
-                ["uts", "angle"],
-                np.reshape(insty, (1, -1)),
-                {"units": "counts", "ancillary_variables": "intensity_std_err"},
-            ),
-            "intensity_std_err": (
-                ["uts", "angle"],
-                np.reshape(idevs, (1, -1)),
-                {"units": "counts", "standard_name": "intensity standard_error"},
-            ),
-            "angle_std_err": (
-                ["uts", "angle"],
-                np.reshape(adiff, (1, -1)),
-                {"units": "deg", "standard_name": "angle standard_error"},
-            ),
-        },
-        coords={
-            "uts": (["uts"], [uts]),
-            "angle": (
-                ["angle"],
-                list(angle),
-                {"units": "deg", "ancillary_variables": "angle_std_err"},
-            ),
-        },
-        attrs=header,
-    )
-    return vals
+"""
+panalyticalcsv: Processing of PANalytical XRD ``csv`` files
+-----------------------------------------------------------
+
+File Structure
+``````````````
+
+These files are split into a ``[Measurement conditions]`` and a ``[Scan points]``
+section. The former stores the metadata and the latter all the datapoints.
+
+Uncertainties
+`````````````
+The uncertainties of ``"angle"`` are taken from the number of significant figures.
+
+The uncertainties of ``"intensity"`` are taken from the number of significant figures.
+
+.. codeauthor::
+    Nicolas Vetsch,
+    Peter Kraus
+"""
+
+from ...dgutils import dateutils
+from .common import panalytical_comment, snake_case
+from uncertainties.core import str_to_number_with_uncert as tuple_fromstr
+import xarray as xr
+import numpy as np
+
+# Converting camelCase xrdml keys to snake_case.
+
+
+def _process_comments(comments: list[str]) -> dict:
+    ret = {}
+    for line in comments:
+        ret.update(panalytical_comment(line))
+    return ret
+
+
+def _process_header(header: str) -> dict:
+    """
+    Processes the header section, staring with the ``[Measurement conditions]`` line.
+
+    Parameters
+    ----------
+    header
+        The header portion as a string.
+
+    Returns
+    -------
+    header: dict
+        A dictionary containing the processed metadata.
+
+    """
+    header_lines = header.split("\n")[1:-1]
+    header = dict([line.split(",", 1) for line in header_lines])
+    # Process comment entries.
+    comments = []
+    for key in list(header.keys()):
+        if key.startswith("Comment"):
+            comments.append(header.pop(key).strip('"'))
+    comments = _process_comments(comments)
+    # Renaming the keys.
+    for key in list(header.keys()):
+        header[snake_case(key)] = header.pop(key)
+    header.update(comments)
+    return header
+
+
+def _process_data(data: str) -> tuple[list, list]:
+    """
+    Processes the data section, starting with the ``[Scan points]`` line.
+
+    Parameters
+    ----------
+    data
+        The data portion as a string.
+
+    Returns
+    -------
+    avals, adevs, ivals, idevs
+        The values and uncertainties in angle and intensity.
+
+    """
+    data_lines = data.split("\n")[1:-1]
+    columns = data_lines[0].split(",")
+    assert columns == ["Angle", "Intensity"], "Unexpected columns."
+    datapoints = [line.split(",") for line in data_lines[1:]]
+    angle, intensity = [list(d) for d in zip(*datapoints)]
+    avals, adevs = list(zip(*[tuple_fromstr(a) for a in angle]))
+    ivals, idevs = list(zip(*[tuple_fromstr(i) for i in intensity]))
+    return avals, adevs, ivals, idevs
+
+
+def process(
+    *,
+    fn: str,
+    encoding: str = "utf-8",
+    timezone: str = "UTC",
+    **kwargs: dict,
+) -> xr.Dataset:
+    """
+    Processes a PANalytical XRD csv file. All information contained in the header
+    of the csv file is stored in the metadata.
+
+    Parameters
+    ----------
+    fn
+        The file containing the trace(s) to parse.
+
+    encoding
+        Encoding of ``fn``, by default "utf-8".
+
+    timezone
+        A string description of the timezone. Default is "UTC".
+
+    Returns
+    -------
+    :class:`xarray.Dataset`
+        Data containing the timesteps and metadata. This filetype contains the full
+        date specification.
+
+    """
+    with open(fn, "r", encoding=encoding) as csv_file:
+        csv = csv_file.read()
+    # Split file into its sections.
+    __, header, data = csv.split("[")
+    assert header.startswith("Measurement conditions"), "Unexpected section."
+    assert data.startswith("Scan points"), "Unexpected section."
+    header = _process_header(header)
+    # Process the data trace.
+    angle, _, insty, _ = _process_data(data)
+    adiff = np.abs(np.diff(angle)) * 0.5
+    adiff = np.append(adiff, adiff[-1])
+    idevs = np.ones(len(insty))
+    # Process the metadata.
+    uts = dateutils.str_to_uts(
+        timestamp=header["file_date_and_time"],
+        format="%d/%B/%Y %H:%M",
+        timezone=timezone,
+    )
+    header["fulldate"] = True
+    # Build Datasets
+    vals = xr.Dataset(
+        data_vars={
+            "intensity": (
+                ["uts", "angle"],
+                np.reshape(insty, (1, -1)),
+                {"units": "counts", "ancillary_variables": "intensity_std_err"},
+            ),
+            "intensity_std_err": (
+                ["uts", "angle"],
+                np.reshape(idevs, (1, -1)),
+                {"units": "counts", "standard_name": "intensity standard_error"},
+            ),
+            "angle_std_err": (
+                ["uts", "angle"],
+                np.reshape(adiff, (1, -1)),
+                {"units": "deg", "standard_name": "angle standard_error"},
+            ),
+        },
+        coords={
+            "uts": (["uts"], [uts]),
+            "angle": (
+                ["angle"],
+                list(angle),
+                {"units": "deg", "ancillary_variables": "angle_std_err"},
+            ),
+        },
+        attrs=header,
+    )
+    return vals
```

### Comparing `yadg-5.0.1/src/yadg/parsers/xrdtrace/panalyticalxrdml.py` & `yadg-5.0.2/src/yadg/parsers/xrdtrace/panalyticalxrdml.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,278 +1,278 @@
-"""
-panalyticalxrdml: Processing of PANalytical XRD ``xml`` files
--------------------------------------------------------------
-
-File Structure
-``````````````
-
-These are xml-formatted files, which we here parse using the :mod:`xml.etree`
-library into a Python :class:`dict`.
-
-.. note::
-
-    The ``angle`` returned from this parser is based on a linear interpolation of
-    the start and end point of the scan, and is the :math:`2\\theta`. The values
-    of :math:`\\omega` are discarded.
-
-.. warning::
-
-    This parser is fairly new and untested. As a result, the returned metadata
-    contain only a subset of the available metadata in the XML file. If something
-    important is missing, please contact us!
-
-Uncertainties
-`````````````
-The uncertainties of in ``"angle"`` are taken as the step-width of
-the linearly spaced :math:`2\\theta` values.
-
-The uncertainties of of ``"intensity"`` are currently set to a constant
-value of 1.0 count as all the supported files seem to produce integer values.
-
-.. codeauthor::
-    Nicolas Vetsch,
-    Peter Kraus
-"""
-
-from collections import defaultdict
-from typing import Union
-from xml.etree import ElementTree
-import numpy as np
-import xarray as xr
-from zoneinfo import ZoneInfo
-
-from uncertainties.core import str_to_number_with_uncert as tuple_fromstr
-from .common import panalytical_comment
-from ...dgutils import dateutils
-
-
-def etree_to_dict(e: ElementTree.Element) -> dict:
-    """Recursively converts an ElementTree.Element into a dictionary.
-
-    Element attributes are stored into `"@"`-prefixed attribute keys.
-    Element text is stored into `"#text"` for all nodes.
-
-    From https://stackoverflow.com/a/10076823.
-
-    Parameters
-    ----------
-    e
-        The ElementTree root Element.
-
-    Returns
-    -------
-    dict
-        ElementTree parsed into a dictionary.
-
-    """
-    d = {e.tag: {} if e.attrib else None}
-    children = list(e)
-    if children:
-        dd = defaultdict(list)
-        for dc in map(etree_to_dict, children):
-            for k, v in dc.items():
-                dd[k].append(v)
-        d = {e.tag: {k: v[0] if len(v) == 1 else v for k, v in dd.items()}}
-    if e.attrib:
-        d[e.tag].update(("@" + k, v) for k, v in e.attrib.items())
-    if e.text:
-        text = e.text.strip()
-        if children or e.attrib:
-            if text:
-                d[e.tag]["#text"] = text
-        else:
-            d[e.tag] = text
-    return d
-
-
-def _process_values(d: Union[dict, str]) -> Union[dict, str]:
-    """
-    Recursively parses dicts in the following format:
-
-    .. code::
-
-        {"key": {"#text": ..., "@unit": ...}, ...}
-
-    into a single string:
-
-    .. code::
-
-        {"key": f"{#text} {@unit}", ...}
-
-    """
-    # TODO
-    # If not "#text" or @tribute just snake_case and recurse.
-    if isinstance(d, dict):
-        if "@unit" in d and "#text" in d:
-            return f"{d['#text']} {d['@unit']}"
-        elif "@version" in d and "#text" in d:
-            return f"{d['#text']} {d['@version']}"
-        else:
-            for k, v in d.items():
-                d[k] = _process_values(v)
-    return d
-
-
-def _process_scan(scan: dict) -> dict:
-    """
-    Parses the scan section of the file. Creates the explicit positions based
-    on the number of measured intensities and the start & end position.
-
-    """
-    header = scan.pop("header")
-    dpts = scan.pop("dataPoints")
-    counting_time = _process_values(dpts.pop("commonCountingTime"))
-    ivals, idevs = list(
-        zip(*[tuple_fromstr(c) for c in dpts["intensities"].pop("#text").split()])
-    )
-    iunit = dpts["intensities"].pop("@unit")
-    timestamp = header.pop("startTimeStamp")
-
-    dp = {
-        "intensity": {"vals": ivals, "devs": idevs, "unit": iunit},
-        "timestamp": timestamp,
-        "counting_time": counting_time,
-    }
-
-    positions = _process_values(dpts.pop("positions"))
-    for v in positions:
-        pos = np.linspace(
-            float(v["startPosition"]), float(v["endPosition"]), num=len(ivals)
-        )
-        adiff = np.abs(np.diff(pos)) * 0.5
-        adiff = np.append(adiff, adiff[-1])
-        dp[v["@axis"]] = {
-            "vals": pos,
-            "devs": adiff,
-            "unit": v["@unit"],
-        }
-    return dp
-
-
-def _process_comment(comment: dict) -> dict:
-    """ """
-    entry = comment.pop("entry")
-    ret = {}
-    for line in entry:
-        ret.update(panalytical_comment(line))
-    return ret
-
-
-def _process_measurement(measurement: dict, timezone: str):
-    """
-    A function that processes each section of the XRD XML file.
-    """
-    # Comment.
-    comment = measurement["comment"].pop("entry")
-    for line in comment:
-        if "PHD Lower Level" in line and "PHD Upper Level" in line:
-            __, values = list(zip(*[s.split(" = ") for s in line.split(", ")]))
-    keys = ["phd_lower_level", "phd_upper_level"]
-    measurement["comment"] = dict(zip(keys, values))
-    # Wavelength.
-    wavelength = _process_values(measurement.pop("usedWavelength"))
-    measurement["wavelength"] = wavelength
-    # Incident beam path.
-    incident_beam_path = _process_values(measurement.pop("incidentBeamPath"))
-    measurement["incident_beam_path"] = incident_beam_path
-    # Diffracted beam path.
-    diffracted_beam_path = _process_values(measurement.pop("diffractedBeamPath"))
-    measurement["diffracted_beam_path"] = diffracted_beam_path
-    scan = _process_scan(measurement.pop("scan"))
-    trace = {"angle": scan.pop("2Theta"), "intensity": scan.pop("intensity")}
-    meta = measurement
-    meta["counting_time"] = scan.pop("counting_time")
-    trace["uts"] = dateutils.str_to_uts(
-        timestamp=scan.pop("timestamp"), timezone=timezone
-    )
-    return trace, meta
-
-
-def process(
-    *,
-    fn: str,
-    timezone: ZoneInfo,
-    **kwargs: dict,
-) -> xr.Dataset:
-    """Processes a PANalytical xrdml file.
-
-    Parameters
-    ----------
-    fn
-        The file containing the trace(s) to parse.
-
-    timezone
-        A string description of the timezone. Default is "UTC".
-
-    Returns
-    -------
-    :class:`xarray.Dataset`
-        Data containing the timesteps, and metadata. This filetype contains the full
-        date specification.
-
-    """
-    it = ElementTree.iterparse(fn)
-    # Removing xmlns prefixes from all tags.
-    # From https://stackoverflow.com/a/25920989.
-    for __, e in it:
-        __, xmlns_present, postfix = e.tag.partition("}")
-        if xmlns_present:
-            e.tag = postfix  # Strip away all xmlns prefixes.
-    root = it.root
-    xrd = etree_to_dict(root)
-    # Start processing the xml contents.
-    measurements = xrd["xrdMeasurements"]
-    assert measurements["@status"] == "Completed", "Incomplete measurement."
-    comment = _process_comment(measurements["comment"])
-    # Renaming some entries because I want to.
-    sample = measurements["sample"]
-    sample["prepared_by"] = sample.pop("preparedBy")
-    sample["type"] = sample.pop("@type")
-    # Process measurement data.
-    data, meta = _process_measurement(measurements["xrdMeasurement"], timezone)
-    data["fn"] = fn
-    # Shove unused data into meta
-    meta["sample"] = sample
-    meta["comment"] = comment
-    meta["fulldate"] = True
-    # Build Datasets
-    vals = xr.Dataset(
-        data_vars={
-            "intensity": (
-                ["uts", "angle"],
-                np.reshape(data["intensity"]["vals"], (1, -1)),
-                {
-                    "units": data["intensity"]["unit"],
-                    "ancillary_variables": "intensity_std_err",
-                },
-            ),
-            "intensity_std_err": (
-                ["uts", "angle"],
-                np.reshape(data["intensity"]["devs"], (1, -1)),
-                {
-                    "units": data["intensity"]["unit"],
-                    "standard_name": "intensity standard_error",
-                },
-            ),
-            "angle_std_err": (
-                ["uts", "angle"],
-                np.reshape(data["angle"]["devs"], (1, -1)),
-                {
-                    "units": data["angle"]["unit"],
-                    "standard_name": "angle standard_error",
-                },
-            ),
-        },
-        coords={
-            "uts": (["uts"], [data["uts"]]),
-            "angle": (
-                ["angle"],
-                data["angle"]["vals"],
-                {
-                    "units": data["angle"]["unit"],
-                    "ancillary_variables": "angle_std_err",
-                },
-            ),
-        },
-        attrs=meta,
-    )
-    return vals
+"""
+panalyticalxrdml: Processing of PANalytical XRD ``xml`` files
+-------------------------------------------------------------
+
+File Structure
+``````````````
+
+These are xml-formatted files, which we here parse using the :mod:`xml.etree`
+library into a Python :class:`dict`.
+
+.. note::
+
+    The ``angle`` returned from this parser is based on a linear interpolation of
+    the start and end point of the scan, and is the :math:`2\\theta`. The values
+    of :math:`\\omega` are discarded.
+
+.. warning::
+
+    This parser is fairly new and untested. As a result, the returned metadata
+    contain only a subset of the available metadata in the XML file. If something
+    important is missing, please contact us!
+
+Uncertainties
+`````````````
+The uncertainties of in ``"angle"`` are taken as the step-width of
+the linearly spaced :math:`2\\theta` values.
+
+The uncertainties of of ``"intensity"`` are currently set to a constant
+value of 1.0 count as all the supported files seem to produce integer values.
+
+.. codeauthor::
+    Nicolas Vetsch,
+    Peter Kraus
+"""
+
+from collections import defaultdict
+from typing import Union
+from xml.etree import ElementTree
+import numpy as np
+import xarray as xr
+from zoneinfo import ZoneInfo
+
+from uncertainties.core import str_to_number_with_uncert as tuple_fromstr
+from .common import panalytical_comment
+from ...dgutils import dateutils
+
+
+def etree_to_dict(e: ElementTree.Element) -> dict:
+    """Recursively converts an ElementTree.Element into a dictionary.
+
+    Element attributes are stored into `"@"`-prefixed attribute keys.
+    Element text is stored into `"#text"` for all nodes.
+
+    From https://stackoverflow.com/a/10076823.
+
+    Parameters
+    ----------
+    e
+        The ElementTree root Element.
+
+    Returns
+    -------
+    dict
+        ElementTree parsed into a dictionary.
+
+    """
+    d = {e.tag: {} if e.attrib else None}
+    children = list(e)
+    if children:
+        dd = defaultdict(list)
+        for dc in map(etree_to_dict, children):
+            for k, v in dc.items():
+                dd[k].append(v)
+        d = {e.tag: {k: v[0] if len(v) == 1 else v for k, v in dd.items()}}
+    if e.attrib:
+        d[e.tag].update(("@" + k, v) for k, v in e.attrib.items())
+    if e.text:
+        text = e.text.strip()
+        if children or e.attrib:
+            if text:
+                d[e.tag]["#text"] = text
+        else:
+            d[e.tag] = text
+    return d
+
+
+def _process_values(d: Union[dict, str]) -> Union[dict, str]:
+    """
+    Recursively parses dicts in the following format:
+
+    .. code::
+
+        {"key": {"#text": ..., "@unit": ...}, ...}
+
+    into a single string:
+
+    .. code::
+
+        {"key": f"{#text} {@unit}", ...}
+
+    """
+    # TODO
+    # If not "#text" or @tribute just snake_case and recurse.
+    if isinstance(d, dict):
+        if "@unit" in d and "#text" in d:
+            return f"{d['#text']} {d['@unit']}"
+        elif "@version" in d and "#text" in d:
+            return f"{d['#text']} {d['@version']}"
+        else:
+            for k, v in d.items():
+                d[k] = _process_values(v)
+    return d
+
+
+def _process_scan(scan: dict) -> dict:
+    """
+    Parses the scan section of the file. Creates the explicit positions based
+    on the number of measured intensities and the start & end position.
+
+    """
+    header = scan.pop("header")
+    dpts = scan.pop("dataPoints")
+    counting_time = _process_values(dpts.pop("commonCountingTime"))
+    ivals, idevs = list(
+        zip(*[tuple_fromstr(c) for c in dpts["intensities"].pop("#text").split()])
+    )
+    iunit = dpts["intensities"].pop("@unit")
+    timestamp = header.pop("startTimeStamp")
+
+    dp = {
+        "intensity": {"vals": ivals, "devs": idevs, "unit": iunit},
+        "timestamp": timestamp,
+        "counting_time": counting_time,
+    }
+
+    positions = _process_values(dpts.pop("positions"))
+    for v in positions:
+        pos = np.linspace(
+            float(v["startPosition"]), float(v["endPosition"]), num=len(ivals)
+        )
+        adiff = np.abs(np.diff(pos)) * 0.5
+        adiff = np.append(adiff, adiff[-1])
+        dp[v["@axis"]] = {
+            "vals": pos,
+            "devs": adiff,
+            "unit": v["@unit"],
+        }
+    return dp
+
+
+def _process_comment(comment: dict) -> dict:
+    """ """
+    entry = comment.pop("entry")
+    ret = {}
+    for line in entry:
+        ret.update(panalytical_comment(line))
+    return ret
+
+
+def _process_measurement(measurement: dict, timezone: str):
+    """
+    A function that processes each section of the XRD XML file.
+    """
+    # Comment.
+    comment = measurement["comment"].pop("entry")
+    for line in comment:
+        if "PHD Lower Level" in line and "PHD Upper Level" in line:
+            __, values = list(zip(*[s.split(" = ") for s in line.split(", ")]))
+    keys = ["phd_lower_level", "phd_upper_level"]
+    measurement["comment"] = dict(zip(keys, values))
+    # Wavelength.
+    wavelength = _process_values(measurement.pop("usedWavelength"))
+    measurement["wavelength"] = wavelength
+    # Incident beam path.
+    incident_beam_path = _process_values(measurement.pop("incidentBeamPath"))
+    measurement["incident_beam_path"] = incident_beam_path
+    # Diffracted beam path.
+    diffracted_beam_path = _process_values(measurement.pop("diffractedBeamPath"))
+    measurement["diffracted_beam_path"] = diffracted_beam_path
+    scan = _process_scan(measurement.pop("scan"))
+    trace = {"angle": scan.pop("2Theta"), "intensity": scan.pop("intensity")}
+    meta = measurement
+    meta["counting_time"] = scan.pop("counting_time")
+    trace["uts"] = dateutils.str_to_uts(
+        timestamp=scan.pop("timestamp"), timezone=timezone
+    )
+    return trace, meta
+
+
+def process(
+    *,
+    fn: str,
+    timezone: ZoneInfo,
+    **kwargs: dict,
+) -> xr.Dataset:
+    """Processes a PANalytical xrdml file.
+
+    Parameters
+    ----------
+    fn
+        The file containing the trace(s) to parse.
+
+    timezone
+        A string description of the timezone. Default is "UTC".
+
+    Returns
+    -------
+    :class:`xarray.Dataset`
+        Data containing the timesteps, and metadata. This filetype contains the full
+        date specification.
+
+    """
+    it = ElementTree.iterparse(fn)
+    # Removing xmlns prefixes from all tags.
+    # From https://stackoverflow.com/a/25920989.
+    for __, e in it:
+        __, xmlns_present, postfix = e.tag.partition("}")
+        if xmlns_present:
+            e.tag = postfix  # Strip away all xmlns prefixes.
+    root = it.root
+    xrd = etree_to_dict(root)
+    # Start processing the xml contents.
+    measurements = xrd["xrdMeasurements"]
+    assert measurements["@status"] == "Completed", "Incomplete measurement."
+    comment = _process_comment(measurements["comment"])
+    # Renaming some entries because I want to.
+    sample = measurements["sample"]
+    sample["prepared_by"] = sample.pop("preparedBy")
+    sample["type"] = sample.pop("@type")
+    # Process measurement data.
+    data, meta = _process_measurement(measurements["xrdMeasurement"], timezone)
+    data["fn"] = fn
+    # Shove unused data into meta
+    meta["sample"] = sample
+    meta["comment"] = comment
+    meta["fulldate"] = True
+    # Build Datasets
+    vals = xr.Dataset(
+        data_vars={
+            "intensity": (
+                ["uts", "angle"],
+                np.reshape(data["intensity"]["vals"], (1, -1)),
+                {
+                    "units": data["intensity"]["unit"],
+                    "ancillary_variables": "intensity_std_err",
+                },
+            ),
+            "intensity_std_err": (
+                ["uts", "angle"],
+                np.reshape(data["intensity"]["devs"], (1, -1)),
+                {
+                    "units": data["intensity"]["unit"],
+                    "standard_name": "intensity standard_error",
+                },
+            ),
+            "angle_std_err": (
+                ["uts", "angle"],
+                np.reshape(data["angle"]["devs"], (1, -1)),
+                {
+                    "units": data["angle"]["unit"],
+                    "standard_name": "angle standard_error",
+                },
+            ),
+        },
+        coords={
+            "uts": (["uts"], [data["uts"]]),
+            "angle": (
+                ["angle"],
+                data["angle"]["vals"],
+                {
+                    "units": data["angle"]["unit"],
+                    "ancillary_variables": "angle_std_err",
+                },
+            ),
+        },
+        attrs=meta,
+    )
+    return vals
```

### Comparing `yadg-5.0.1/src/yadg.egg-info/PKG-INFO` & `yadg-5.0.2/src/yadg.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,97 +1,97 @@
-Metadata-Version: 2.1
-Name: yadg
-Version: 5.0.1
-Summary: yet another datagram
-Home-page: https://github.com/dgbowl/yadg
-Author: Peter Kraus
-Author-email: peter@tondon.de
-Project-URL: Bug Tracker, https://github.com/dgbowl/yadg/issues
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy
-Requires-Dist: scipy
-Requires-Dist: pint>=0.22
-Requires-Dist: pyyaml
-Requires-Dist: uncertainties
-Requires-Dist: striprtf
-Requires-Dist: tzlocal
-Requires-Dist: packaging
-Requires-Dist: python-dateutil
-Requires-Dist: openpyxl>=3.0.0
-Requires-Dist: h5netcdf~=1.0
-Requires-Dist: xarray-datatree==0.0.12
-Requires-Dist: dgbowl-schemas>=116
-Requires-Dist: requests
-Provides-Extra: testing
-Requires-Dist: pytest; extra == "testing"
-Provides-Extra: docs
-Requires-Dist: sphinx~=7.2; extra == "docs"
-Requires-Dist: sphinx-rtd-theme~=1.3.0; extra == "docs"
-Requires-Dist: sphinx-autodoc-typehints<1.20.0; extra == "docs"
-Requires-Dist: autodoc-pydantic>=2.0.0; extra == "docs"
-
-[![DOI](https://joss.theoj.org/papers/10.21105/joss.04166/status.svg)](https://doi.org/10.21105/joss.04166)
-[![Documentation](https://badgen.net/badge/docs/dgbowl.github.io/grey?icon=firefox)](https://dgbowl.github.io/yadg)
-[![PyPi version](https://badgen.net/pypi/v/yadg/?icon=pypi)](https://pypi.org/project/yadg)
-[![Github link](https://badgen.net/github/tag/dgbowl/yadg/?icon=github)](https://github.com/dgbowl/yadg/)
-[![Github status](https://badgen.net/github/checks/dgbowl/yadg/?icon=github)](https://github.com/dgbowl/yadg/actions/workflows/push-master.yml)
-
-
-# ![yet another datagram](./docs/source/images/yadg_banner.png)
-
-Set of tools to process raw instrument data according to a *dataschema* into a standardised form called *datagram*, annotated with metadata, provenance information, timestamps, units, and uncertainties. Developed by the [Materials for Energy Conversion](https://www.empa.ch/web/s501) lab at Empa (Dübendorf, CH) and by the [ConCat lab](https://www.tu.berlin/en/concat) at Technische Universität Berlin (Berlin, DE).
-
-![schema to datagram with yadg](./docs/source/images/schema_yadg_datagram.png)
-
-### Capabilities:
-- Parsing **tabulated data** using CSV parsing functionality, including Bronkhorst and DryCal output formats.
-- Parsing **chromatography data** from gas and liquid chromatography, including several Agilent, Masshunter, and Fusion formats.
-- Parsing **reflection coefficient** traces from network analysers.
-- Parsing **potentiostat files** for electrochemistry applications. Supports BioLogic file formats.
-- Parsing **spectroscopy files** including common XPS, XRD and MS formats.
-
-### Features:
-- timezone-aware timestamping using Unix timestamps
-- automatic uncertainty determination using data contained in the raw files, instrument specification, or last significant digit
-- uncertainty propagation to derived quantities
-- tagging of data with units
-- extensive *dataschema* and *datagram* validation using provided specifications
-- mandatory metadata (such as provenance) is enforced
-
-The full list of capabilities and features is listed in the [project documentation](http://dgbowl.github.io/yadg).
-
-### Installation:
-The released versions of `yadg` are available on the Python Package Index (PyPI) under [yadg](https://pypi.org/project/yadg). Those can be installed using:
-
-```bash
-    pip install yadg
-```
-
-If you wish to install the current development version as an editable installation, check out the `master` branch using git, and install `yadg` as an editable package using pip:
-
-```bash
-   git clone git@github.com:dgbowl/yadg.git
-   cd yadg
-   pip install -e .
-```
-
-Additional targets `yadg[testing]` and `yadg[docs]` are available and can be specified in the above commands, if testing and/or documentation capabilities are required.
-
-### Contributors:
-- [Peter Kraus](http://github.com/PeterKraus)
-- [Nicolas Vetsch](http://github.com/vetschn)
-
-### Acknowledgements
-
-This project has received funding from the following sources:
-
-- European Union’s Horizon 2020 programme under grant agreement No 957189.
-- DFG's Emmy Noether Programme under grant number 490703766.
-
-The project is also part of BATTERY 2030+, the large-scale European research initiative for inventing the sustainable batteries of the future.
+Metadata-Version: 2.1
+Name: yadg
+Version: 5.0.2
+Summary: yet another datagram
+Home-page: https://github.com/dgbowl/yadg
+Author: Peter Kraus
+Author-email: peter@tondon.de
+Project-URL: Bug Tracker, https://github.com/dgbowl/yadg/issues
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: pint>=0.22
+Requires-Dist: pyyaml
+Requires-Dist: uncertainties
+Requires-Dist: striprtf
+Requires-Dist: tzlocal
+Requires-Dist: packaging
+Requires-Dist: python-dateutil
+Requires-Dist: openpyxl>=3.0.0
+Requires-Dist: h5netcdf~=1.0
+Requires-Dist: xarray-datatree==0.0.12
+Requires-Dist: dgbowl-schemas>=116
+Requires-Dist: requests
+Provides-Extra: testing
+Requires-Dist: pytest; extra == "testing"
+Provides-Extra: docs
+Requires-Dist: sphinx~=7.2; extra == "docs"
+Requires-Dist: sphinx-rtd-theme~=1.3.0; extra == "docs"
+Requires-Dist: sphinx-autodoc-typehints<1.20.0; extra == "docs"
+Requires-Dist: autodoc-pydantic>=2.0.0; extra == "docs"
+
+[![DOI](https://joss.theoj.org/papers/10.21105/joss.04166/status.svg)](https://doi.org/10.21105/joss.04166)
+[![Documentation](https://badgen.net/badge/docs/dgbowl.github.io/grey?icon=firefox)](https://dgbowl.github.io/yadg)
+[![PyPi version](https://badgen.net/pypi/v/yadg/?icon=pypi)](https://pypi.org/project/yadg)
+[![Github link](https://badgen.net/github/tag/dgbowl/yadg/?icon=github)](https://github.com/dgbowl/yadg/)
+[![Github status](https://badgen.net/github/checks/dgbowl/yadg/?icon=github)](https://github.com/dgbowl/yadg/actions/workflows/push-master.yml)
+
+
+# ![yet another datagram](./docs/source/images/yadg_banner.png)
+
+Set of tools to process raw instrument data according to a *dataschema* into a standardised form called *datagram*, annotated with metadata, provenance information, timestamps, units, and uncertainties. Developed by the [Materials for Energy Conversion](https://www.empa.ch/web/s501) lab at Empa (Dübendorf, CH) and by the [ConCat lab](https://www.tu.berlin/en/concat) at Technische Universität Berlin (Berlin, DE).
+
+![schema to datagram with yadg](./docs/source/images/schema_yadg_datagram.png)
+
+### Capabilities:
+- Parsing **tabulated data** using CSV parsing functionality, including Bronkhorst and DryCal output formats.
+- Parsing **chromatography data** from gas and liquid chromatography, including several Agilent, Masshunter, and Fusion formats.
+- Parsing **reflection coefficient** traces from network analysers.
+- Parsing **potentiostat files** for electrochemistry applications. Supports BioLogic file formats.
+- Parsing **spectroscopy files** including common XPS, XRD and MS formats.
+
+### Features:
+- timezone-aware timestamping using Unix timestamps
+- automatic uncertainty determination using data contained in the raw files, instrument specification, or last significant digit
+- uncertainty propagation to derived quantities
+- tagging of data with units
+- extensive *dataschema* and *datagram* validation using provided specifications
+- mandatory metadata (such as provenance) is enforced
+
+The full list of capabilities and features is listed in the [project documentation](http://dgbowl.github.io/yadg).
+
+### Installation:
+The released versions of `yadg` are available on the Python Package Index (PyPI) under [yadg](https://pypi.org/project/yadg). Those can be installed using:
+
+```bash
+    pip install yadg
+```
+
+If you wish to install the current development version as an editable installation, check out the `master` branch using git, and install `yadg` as an editable package using pip:
+
+```bash
+   git clone git@github.com:dgbowl/yadg.git
+   cd yadg
+   pip install -e .
+```
+
+Additional targets `yadg[testing]` and `yadg[docs]` are available and can be specified in the above commands, if testing and/or documentation capabilities are required.
+
+### Contributors:
+- [Peter Kraus](http://github.com/PeterKraus)
+- [Nicolas Vetsch](http://github.com/vetschn)
+
+### Acknowledgements
+
+This project has received funding from the following sources:
+
+- European Union’s Horizon 2020 programme under grant agreement No 957189.
+- DFG's Emmy Noether Programme under grant number 490703766.
+
+The project is also part of BATTERY 2030+, the large-scale European research initiative for inventing the sustainable batteries of the future.
```

### Comparing `yadg-5.0.1/src/yadg.egg-info/SOURCES.txt` & `yadg-5.0.2/src/yadg.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -48,17 +48,15 @@
 src/yadg/parsers/electrochem/__init__.py
 src/yadg/parsers/electrochem/eclabmpr.py
 src/yadg/parsers/electrochem/eclabmpt.py
 src/yadg/parsers/electrochem/tomatojson.py
 src/yadg/parsers/electrochem/eclabcommon/__init__.py
 src/yadg/parsers/electrochem/eclabcommon/mpr_columns.py
 src/yadg/parsers/electrochem/eclabcommon/mpt_columns.py
-src/yadg/parsers/electrochem/eclabcommon/parameters.yml
 src/yadg/parsers/electrochem/eclabcommon/techniques.py
-src/yadg/parsers/electrochem/eclabcommon/techniques.yml
 src/yadg/parsers/flowdata/__init__.py
 src/yadg/parsers/flowdata/drycal.py
 src/yadg/parsers/flowdata/main.py
 src/yadg/parsers/masstrace/__init__.py
 src/yadg/parsers/masstrace/quadstarsac.py
 src/yadg/parsers/meascsv/__init__.py
 src/yadg/parsers/qftrace/__init__.py
```

### Comparing `yadg-5.0.1/tests/test_chromdata.py` & `yadg-5.0.2/tests/test_chromdata.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,264 +1,264 @@
-import pytest
-import os
-import yaml
-from tests.utils import (
-    datagram_from_input,
-    standard_datagram_test,
-    compare_result_dicts,
-    dg_get_quantity,
-)
-from yadg.core import process_schema
-from dgbowl_schemas.yadg import to_dataschema
-
-
-def special_datagram_test(datagram, testspec):
-    for i in {"height", "area", "concentration", "xout", "retention time"}:
-        if i not in testspec:
-            continue
-        ret = dg_get_quantity(datagram, testspec["step"], i, testspec["point"])
-        for k, v in testspec[i].items():
-            rval = ret["n"].sel(dict(species=k))
-            rdev = ret["s"].sel(dict(species=k))
-            ru = ret["u"]
-            print(f"{testspec[i]=}")
-            print(f"{ret['n'].sel(dict(species=k))=}")
-            compare_result_dicts({"n": rval, "s": rdev, "u": ru}, v)
-        assert ret["n"].uts == testspec["uts"]
-
-
-@pytest.mark.parametrize(
-    "input, ts",
-    [
-        (
-            {  # ts0 - fusion-json
-                "folders": ["."],
-                "prefix": "15p",
-                "suffix": "fusion-data",
-                "parameters": {
-                    "filetype": "fusion.json",
-                },
-            },
-            {
-                "nsteps": 1,
-                "step": 0,
-                "nrows": 3,
-                "method": "AS_Cal_20220204",
-                "point": 1,
-                "height": {
-                    "MeOH": {"n": 0.0, "s": 1.0},
-                },
-                "area": {
-                    "O2": {"n": 1034.53, "s": 0.01, "u": None},
-                },
-                "concentration": {
-                    "CO": {"n": 0.02911539, "s": 0.0000291, "u": "%"},
-                },
-                "xout": {
-                    "C2H6": {"n": 0.22425762, "s": 0.00022426, "u": "%"},
-                },
-                "retention time": {
-                    "C2H6": {"n": 43.78, "s": 0.01, "u": "s"},
-                },
-                "uts": 1654697826.467,
-            },
-        ),
-        (
-            {  # ts1 - fusion-zip
-                "folders": ["."],
-                "prefix": "20220608",
-                "suffix": "zip",
-                "parameters": {
-                    "filetype": "fusion.zip",
-                },
-            },
-            {
-                "nsteps": 1,
-                "step": 0,
-                "nrows": 15,
-                "method": "AS_Cal_20220204",
-                "point": 13,
-                "height": {
-                    "MeOH": {"n": 0.0, "s": 1.0},
-                },
-                "area": {
-                    "O2": {"n": 1034.53, "s": 0.01},
-                },
-                "concentration": {
-                    "CO": {"n": 0.02911539, "s": 0.0000291, "u": "%"},
-                },
-                "xout": {
-                    "C2H6": {"n": 0.22425762, "s": 0.00022426, "u": "%"},
-                },
-                "retention time": {
-                    "C2H6": {"n": 43.78, "s": 0.01, "u": "s"},
-                },
-                "uts": 1654697826.467,
-            },
-        ),
-        (
-            {  # ts1 - fusion-csv
-                "folders": ["."],
-                "prefix": "20220608",
-                "suffix": "csv",
-                "parameters": {
-                    "filetype": "fusion.csv",
-                },
-            },
-            {
-                "nsteps": 1,
-                "step": 0,
-                "nrows": 15,
-                "method": "AS_Cal_20220204",
-                "point": 1,
-                "area": {
-                    "O2": {"n": 1034.53, "s": 0.001, "u": None},
-                },
-                "concentration": {
-                    "CO": {"n": 0.02911539, "s": 1e-8, "u": "%"},
-                },
-                "xout": {
-                    "C2H6": {"n": 0.22425762, "s": 1e-8, "u": "%"},
-                },
-                "retention time": {
-                    "C2H6": {"n": 43.78, "s": 0.01, "u": "s"},
-                },
-                "uts": 1654697826.0,
-            },
-        ),
-        (
-            {  # ts2 - empalc.csv
-                "folders": ["."],
-                "suffix": "20p_v2.csv",
-                "parameters": {
-                    "filetype": "empalc.csv",
-                },
-                "externaldate": {"using": {"utsoffset": 0}},
-            },
-            {
-                "nsteps": 1,
-                "step": 0,
-                "nrows": 18,
-                "method": "CO2RR_ChA_FTI_0.6mL_40uL_45dgr_32min.amx",
-                "point": 17,
-                "height": {
-                    "Formic acid": {"n": 3436.903, "s": 0.001, "u": None},
-                },
-                "area": {
-                    "Formic acid": {"n": 155913.098, "s": 0.001, "u": None},
-                },
-                "concentration": {
-                    "Formic acid": {"n": 18.7521, "s": 0.0001, "u": "mmol/l"},
-                },
-                "retention time": {
-                    "Formic acid": {"n": 15.671, "s": 0.001, "u": "min"},
-                },
-                "uts": 20400.0,
-            },
-        ),
-        (
-            {  # ts2 - empalc.csv
-                "folders": ["."],
-                "suffix": "25p_v2.csv",
-                "parameters": {
-                    "filetype": "empalc.csv",
-                },
-                "externaldate": {"using": {"utsoffset": 0}},
-            },
-            {
-                "nsteps": 1,
-                "step": 0,
-                "nrows": 19,
-                "method": "CO2RR_ChA_FTI_0.6mL_40uL_45dgr_32min.amx",
-                "point": 18,
-                "height": {
-                    "Ethanol": {"n": 25495.948, "s": 0.001, "u": None},
-                },
-                "area": {
-                    "Ethanol": {"n": 2745541.097, "s": 0.001, "u": None},
-                },
-                "concentration": {
-                    "Ethanol": {"n": 254.4736, "s": 0.0001, "u": "mmol/l"},
-                },
-                "retention time": {
-                    "Ethanol": {"n": 21.098, "s": 0.001, "u": "min"},
-                },
-                "uts": 21600.0,
-            },
-        ),
-        (
-            {  # ts2 - empalc.xlsx
-                "folders": ["."],
-                "suffix": "25p_v2.xlsx",
-                "parameters": {
-                    "filetype": "empalc.xlsx",
-                },
-                "externaldate": {"using": {"utsoffset": 0}},
-            },
-            {
-                "nsteps": 1,
-                "step": 0,
-                "nrows": 19,
-                "method": "CO2RR_ChA_FTI_0.6mL_40uL_45dgr_32min.amx",
-                "point": 18,
-                "height": {
-                    "Ethanol": {"n": 25495.948, "s": 0.001},
-                },
-                "area": {
-                    "Ethanol": {"n": 2745541.097, "s": 0.001, "u": None},
-                },
-                "concentration": {
-                    "Ethanol": {"n": 254.4736, "s": 0.0001, "u": "mmol/l"},
-                },
-                "retention time": {
-                    "Ethanol": {"n": 21.098, "s": 0.001, "u": "min"},
-                },
-                "uts": 21600.0,
-            },
-        ),
-        (
-            {  # ts3 - empalc.xlsx with newlines
-                "folders": ["."],
-                "suffix": "newlines.xlsx",
-                "parameters": {
-                    "filetype": "empalc.xlsx",
-                },
-                "externaldate": {"using": {"utsoffset": 0}},
-            },
-            {
-                "nsteps": 1,
-                "step": 0,
-                "nrows": 20,
-                "method": "CO2RR_ChA_FTI_0.6mL_40uL_45dgr_32min.amx",
-                "point": 18,
-                "height": {
-                    "Ethanol": {"n": 464.048, "s": 0.001},
-                },
-                "area": {
-                    "Ethanol": {"n": 26514.098, "s": 0.001},
-                },
-                "concentration": {
-                    "Ethanol": {"n": 2.4303, "s": 0.0001, "u": "mmol/l"},
-                },
-                "retention time": {
-                    "Ethanol": {"n": 20.74, "s": 0.01, "u": "min"},
-                },
-                "uts": 21600.0,
-            },
-        ),
-    ],
-)
-def test_datagram_from_chromdata(input, ts, datadir):
-    os.chdir(datadir)
-    ret = datagram_from_input(input, "chromdata", datadir, version="4.2")
-    standard_datagram_test(ret, ts)
-    special_datagram_test(ret, ts)
-
-
-def test_lock_stock_chromdata(datadir):
-    os.chdir(datadir)
-    with open("lock_stock_dataschema.yml", "r") as inf:
-        schema = yaml.safe_load(inf)
-    ret = process_schema(to_dataschema(**schema))
-    print(f"{ret=}")
-    for k in {"height", "concentration", "retention time", "area"}:
-        assert ret["LC"][k].shape == (7, 2)
+import pytest
+import os
+import yaml
+from tests.utils import (
+    datagram_from_input,
+    standard_datagram_test,
+    compare_result_dicts,
+    dg_get_quantity,
+)
+from yadg.core import process_schema
+from dgbowl_schemas.yadg import to_dataschema
+
+
+def special_datagram_test(datagram, testspec):
+    for i in {"height", "area", "concentration", "xout", "retention time"}:
+        if i not in testspec:
+            continue
+        ret = dg_get_quantity(datagram, testspec["step"], i, testspec["point"])
+        for k, v in testspec[i].items():
+            rval = ret["n"].sel(dict(species=k))
+            rdev = ret["s"].sel(dict(species=k))
+            ru = ret["u"]
+            print(f"{testspec[i]=}")
+            print(f"{ret['n'].sel(dict(species=k))=}")
+            compare_result_dicts({"n": rval, "s": rdev, "u": ru}, v)
+        assert ret["n"].uts == testspec["uts"]
+
+
+@pytest.mark.parametrize(
+    "input, ts",
+    [
+        (
+            {  # ts0 - fusion-json
+                "folders": ["."],
+                "prefix": "15p",
+                "suffix": "fusion-data",
+                "parameters": {
+                    "filetype": "fusion.json",
+                },
+            },
+            {
+                "nsteps": 1,
+                "step": 0,
+                "nrows": 3,
+                "method": "AS_Cal_20220204",
+                "point": 1,
+                "height": {
+                    "MeOH": {"n": 0.0, "s": 1.0},
+                },
+                "area": {
+                    "O2": {"n": 1034.53, "s": 0.01, "u": None},
+                },
+                "concentration": {
+                    "CO": {"n": 0.02911539, "s": 0.0000291, "u": "%"},
+                },
+                "xout": {
+                    "C2H6": {"n": 0.22425762, "s": 0.00022426, "u": "%"},
+                },
+                "retention time": {
+                    "C2H6": {"n": 43.78, "s": 0.01, "u": "s"},
+                },
+                "uts": 1654697826.467,
+            },
+        ),
+        (
+            {  # ts1 - fusion-zip
+                "folders": ["."],
+                "prefix": "20220608",
+                "suffix": "zip",
+                "parameters": {
+                    "filetype": "fusion.zip",
+                },
+            },
+            {
+                "nsteps": 1,
+                "step": 0,
+                "nrows": 15,
+                "method": "AS_Cal_20220204",
+                "point": 13,
+                "height": {
+                    "MeOH": {"n": 0.0, "s": 1.0},
+                },
+                "area": {
+                    "O2": {"n": 1034.53, "s": 0.01},
+                },
+                "concentration": {
+                    "CO": {"n": 0.02911539, "s": 0.0000291, "u": "%"},
+                },
+                "xout": {
+                    "C2H6": {"n": 0.22425762, "s": 0.00022426, "u": "%"},
+                },
+                "retention time": {
+                    "C2H6": {"n": 43.78, "s": 0.01, "u": "s"},
+                },
+                "uts": 1654697826.467,
+            },
+        ),
+        (
+            {  # ts1 - fusion-csv
+                "folders": ["."],
+                "prefix": "20220608",
+                "suffix": "csv",
+                "parameters": {
+                    "filetype": "fusion.csv",
+                },
+            },
+            {
+                "nsteps": 1,
+                "step": 0,
+                "nrows": 15,
+                "method": "AS_Cal_20220204",
+                "point": 1,
+                "area": {
+                    "O2": {"n": 1034.53, "s": 0.001, "u": None},
+                },
+                "concentration": {
+                    "CO": {"n": 0.02911539, "s": 1e-8, "u": "%"},
+                },
+                "xout": {
+                    "C2H6": {"n": 0.22425762, "s": 1e-8, "u": "%"},
+                },
+                "retention time": {
+                    "C2H6": {"n": 43.78, "s": 0.01, "u": "s"},
+                },
+                "uts": 1654697826.0,
+            },
+        ),
+        (
+            {  # ts2 - empalc.csv
+                "folders": ["."],
+                "suffix": "20p_v2.csv",
+                "parameters": {
+                    "filetype": "empalc.csv",
+                },
+                "externaldate": {"using": {"utsoffset": 0}},
+            },
+            {
+                "nsteps": 1,
+                "step": 0,
+                "nrows": 18,
+                "method": "CO2RR_ChA_FTI_0.6mL_40uL_45dgr_32min.amx",
+                "point": 17,
+                "height": {
+                    "Formic acid": {"n": 3436.903, "s": 0.001, "u": None},
+                },
+                "area": {
+                    "Formic acid": {"n": 155913.098, "s": 0.001, "u": None},
+                },
+                "concentration": {
+                    "Formic acid": {"n": 18.7521, "s": 0.0001, "u": "mmol/l"},
+                },
+                "retention time": {
+                    "Formic acid": {"n": 15.671, "s": 0.001, "u": "min"},
+                },
+                "uts": 20400.0,
+            },
+        ),
+        (
+            {  # ts2 - empalc.csv
+                "folders": ["."],
+                "suffix": "25p_v2.csv",
+                "parameters": {
+                    "filetype": "empalc.csv",
+                },
+                "externaldate": {"using": {"utsoffset": 0}},
+            },
+            {
+                "nsteps": 1,
+                "step": 0,
+                "nrows": 19,
+                "method": "CO2RR_ChA_FTI_0.6mL_40uL_45dgr_32min.amx",
+                "point": 18,
+                "height": {
+                    "Ethanol": {"n": 25495.948, "s": 0.001, "u": None},
+                },
+                "area": {
+                    "Ethanol": {"n": 2745541.097, "s": 0.001, "u": None},
+                },
+                "concentration": {
+                    "Ethanol": {"n": 254.4736, "s": 0.0001, "u": "mmol/l"},
+                },
+                "retention time": {
+                    "Ethanol": {"n": 21.098, "s": 0.001, "u": "min"},
+                },
+                "uts": 21600.0,
+            },
+        ),
+        (
+            {  # ts2 - empalc.xlsx
+                "folders": ["."],
+                "suffix": "25p_v2.xlsx",
+                "parameters": {
+                    "filetype": "empalc.xlsx",
+                },
+                "externaldate": {"using": {"utsoffset": 0}},
+            },
+            {
+                "nsteps": 1,
+                "step": 0,
+                "nrows": 19,
+                "method": "CO2RR_ChA_FTI_0.6mL_40uL_45dgr_32min.amx",
+                "point": 18,
+                "height": {
+                    "Ethanol": {"n": 25495.948, "s": 0.001},
+                },
+                "area": {
+                    "Ethanol": {"n": 2745541.097, "s": 0.001, "u": None},
+                },
+                "concentration": {
+                    "Ethanol": {"n": 254.4736, "s": 0.0001, "u": "mmol/l"},
+                },
+                "retention time": {
+                    "Ethanol": {"n": 21.098, "s": 0.001, "u": "min"},
+                },
+                "uts": 21600.0,
+            },
+        ),
+        (
+            {  # ts3 - empalc.xlsx with newlines
+                "folders": ["."],
+                "suffix": "newlines.xlsx",
+                "parameters": {
+                    "filetype": "empalc.xlsx",
+                },
+                "externaldate": {"using": {"utsoffset": 0}},
+            },
+            {
+                "nsteps": 1,
+                "step": 0,
+                "nrows": 20,
+                "method": "CO2RR_ChA_FTI_0.6mL_40uL_45dgr_32min.amx",
+                "point": 18,
+                "height": {
+                    "Ethanol": {"n": 464.048, "s": 0.001},
+                },
+                "area": {
+                    "Ethanol": {"n": 26514.098, "s": 0.001},
+                },
+                "concentration": {
+                    "Ethanol": {"n": 2.4303, "s": 0.0001, "u": "mmol/l"},
+                },
+                "retention time": {
+                    "Ethanol": {"n": 20.74, "s": 0.01, "u": "min"},
+                },
+                "uts": 21600.0,
+            },
+        ),
+    ],
+)
+def test_datagram_from_chromdata(input, ts, datadir):
+    os.chdir(datadir)
+    ret = datagram_from_input(input, "chromdata", datadir, version="4.2")
+    standard_datagram_test(ret, ts)
+    special_datagram_test(ret, ts)
+
+
+def test_lock_stock_chromdata(datadir):
+    os.chdir(datadir)
+    with open("lock_stock_dataschema.yml", "r") as inf:
+        schema = yaml.safe_load(inf)
+    ret = process_schema(to_dataschema(**schema))
+    print(f"{ret=}")
+    for k in {"height", "concentration", "retention time", "area"}:
+        assert ret["LC"][k].shape == (7, 2)
```

### Comparing `yadg-5.0.1/tests/test_drycal.py` & `yadg-5.0.2/tests/test_drycal.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,119 +1,119 @@
-import pytest
-import os
-import yaml
-from tests.utils import (
-    datagram_from_input,
-    standard_datagram_test,
-    pars_datagram_test,
-)
-from yadg.core import process_schema
-from dgbowl_schemas.yadg import to_dataschema
-
-
-@pytest.mark.parametrize(
-    "input, ts",
-    [
-        (
-            {  # ts0 - rtf parser, supplied date
-                "case": "Cp_100mA_1mindelay.rtf",
-                "parameters": {"filetype": "drycal.rtf"},
-                "externaldate": {"from": {"isostring": "2021-09-17"}},
-            },
-            {
-                "nsteps": 1,
-                "step": 0,
-                "nrows": 110,
-                "point": 0,
-                "pars": {
-                    "Temp": {"sigma": 0.1, "value": 27.4, "unit": "degC"},
-                    "uts": {"value": 1631880613.0},
-                },
-            },
-        ),
-        (
-            {  # ts1 - default sep parser, date from fn
-                "case": "20211011_DryCal_out.csv",
-                "parameters": {"filetype": "drycal.csv"},
-                "externaldate": {"from": {"filename": {"format": "%Y%m%d", "len": 8}}},
-            },
-            {
-                "nsteps": 1,
-                "step": 0,
-                "nrows": 29,
-                "point": 0,
-                "pars": {
-                    "Temp": {"sigma": 0.1, "value": 24.3, "unit": "degC"},
-                    "uts": {"value": 1633956333.0},
-                },
-            },
-        ),
-        (
-            {  # ts2 - default sep parser, date from fn, sigma from length
-                "case": "2021-10-11_DryCal_out.txt",
-                "parameters": {"filetype": "drycal.txt"},
-                "externaldate": {
-                    "from": {"filename": {"format": "%Y-%m-%d", "len": 10}}
-                },
-            },
-            {
-                "nsteps": 1,
-                "step": 0,
-                "nrows": 29,
-                "point": 28,
-                "pars": {
-                    "Pressure": {"sigma": 0.001, "value": 971.0, "unit": "mbar"},
-                    "uts": {"value": 1633958360.0},
-                },
-            },
-        ),
-        (
-            {  # ts3 - default sep parser, date from fn
-                "case": "2021-10-11_DryCal_out.txt",
-                "parameters": {"filetype": "drycal.txt"},
-                "externaldate": {
-                    "from": {"filename": {"format": "%Y-%m-%d", "len": 10}}
-                },
-            },
-            {
-                "nsteps": 1,
-                "step": 0,
-                "nrows": 29,
-                "point": 28,
-                "pars": {
-                    "DryCal": {"sigma": 0.0001, "value": 14.848, "unit": "smL/min"},
-                    "Pressure": {"sigma": 0.001, "value": 971.0, "unit": "mbar"},
-                },
-            },
-        ),
-        (
-            {  # ts4 - overnight run
-                "case": "20220721-porosity-study-20p-Cu-200mA-EDLC-01-flow.csv",
-                "parameters": {"filetype": "drycal.csv"},
-                "externaldate": {"from": {"filename": {"format": "%Y%m%d", "len": 8}}},
-            },
-            {
-                "nsteps": 1,
-                "step": 0,
-                "nrows": 77,
-                "point": 76,
-                "pars": {
-                    "Temp": {"sigma": 0.1, "value": 28.6, "unit": "degC"},
-                    "uts": {"value": 1658475079.0},
-                },
-            },
-        ),
-    ],
-)
-def test_datagram_from_drycal(input, ts, datadir):
-    ret = datagram_from_input(input, "flowdata", datadir)
-    standard_datagram_test(ret, ts)
-    pars_datagram_test(ret, ts)
-
-
-def test_lock_stock_drycal(datadir):
-    os.chdir(datadir)
-    with open("lock_stock_dataschema.yml", "r") as inf:
-        schema = yaml.safe_load(inf)
-    ret = process_schema(to_dataschema(**schema))
-    print(f"{ret=}")
-    assert ret["outlet"]["DryCal"].shape == (187,)
+import pytest
+import os
+import yaml
+from tests.utils import (
+    datagram_from_input,
+    standard_datagram_test,
+    pars_datagram_test,
+)
+from yadg.core import process_schema
+from dgbowl_schemas.yadg import to_dataschema
+
+
+@pytest.mark.parametrize(
+    "input, ts",
+    [
+        (
+            {  # ts0 - rtf parser, supplied date
+                "case": "Cp_100mA_1mindelay.rtf",
+                "parameters": {"filetype": "drycal.rtf"},
+                "externaldate": {"from": {"isostring": "2021-09-17"}},
+            },
+            {
+                "nsteps": 1,
+                "step": 0,
+                "nrows": 110,
+                "point": 0,
+                "pars": {
+                    "Temp": {"sigma": 0.1, "value": 27.4, "unit": "degC"},
+                    "uts": {"value": 1631880613.0},
+                },
+            },
+        ),
+        (
+            {  # ts1 - default sep parser, date from fn
+                "case": "20211011_DryCal_out.csv",
+                "parameters": {"filetype": "drycal.csv"},
+                "externaldate": {"from": {"filename": {"format": "%Y%m%d", "len": 8}}},
+            },
+            {
+                "nsteps": 1,
+                "step": 0,
+                "nrows": 29,
+                "point": 0,
+                "pars": {
+                    "Temp": {"sigma": 0.1, "value": 24.3, "unit": "degC"},
+                    "uts": {"value": 1633956333.0},
+                },
+            },
+        ),
+        (
+            {  # ts2 - default sep parser, date from fn, sigma from length
+                "case": "2021-10-11_DryCal_out.txt",
+                "parameters": {"filetype": "drycal.txt"},
+                "externaldate": {
+                    "from": {"filename": {"format": "%Y-%m-%d", "len": 10}}
+                },
+            },
+            {
+                "nsteps": 1,
+                "step": 0,
+                "nrows": 29,
+                "point": 28,
+                "pars": {
+                    "Pressure": {"sigma": 0.001, "value": 971.0, "unit": "mbar"},
+                    "uts": {"value": 1633958360.0},
+                },
+            },
+        ),
+        (
+            {  # ts3 - default sep parser, date from fn
+                "case": "2021-10-11_DryCal_out.txt",
+                "parameters": {"filetype": "drycal.txt"},
+                "externaldate": {
+                    "from": {"filename": {"format": "%Y-%m-%d", "len": 10}}
+                },
+            },
+            {
+                "nsteps": 1,
+                "step": 0,
+                "nrows": 29,
+                "point": 28,
+                "pars": {
+                    "DryCal": {"sigma": 0.0001, "value": 14.848, "unit": "smL/min"},
+                    "Pressure": {"sigma": 0.001, "value": 971.0, "unit": "mbar"},
+                },
+            },
+        ),
+        (
+            {  # ts4 - overnight run
+                "case": "20220721-porosity-study-20p-Cu-200mA-EDLC-01-flow.csv",
+                "parameters": {"filetype": "drycal.csv"},
+                "externaldate": {"from": {"filename": {"format": "%Y%m%d", "len": 8}}},
+            },
+            {
+                "nsteps": 1,
+                "step": 0,
+                "nrows": 77,
+                "point": 76,
+                "pars": {
+                    "Temp": {"sigma": 0.1, "value": 28.6, "unit": "degC"},
+                    "uts": {"value": 1658475079.0},
+                },
+            },
+        ),
+    ],
+)
+def test_datagram_from_drycal(input, ts, datadir):
+    ret = datagram_from_input(input, "flowdata", datadir)
+    standard_datagram_test(ret, ts)
+    pars_datagram_test(ret, ts)
+
+
+def test_lock_stock_drycal(datadir):
+    os.chdir(datadir)
+    with open("lock_stock_dataschema.yml", "r") as inf:
+        schema = yaml.safe_load(inf)
+    ret = process_schema(to_dataschema(**schema))
+    print(f"{ret=}")
+    assert ret["outlet"]["DryCal"].shape == (187,)
```

### Comparing `yadg-5.0.1/tests/test_encoding.py` & `yadg-5.0.2/tests/test_encoding.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-import pytest
-from tests.utils import datagram_from_input, standard_datagram_test
-
-
-@pytest.mark.parametrize(
-    "input, ts",
-    [
-        (
-            {  # ts1 - BOM requires utf-8-sig encoding
-                "case": "log 2021-09-17 11-26-14.140.csv",
-                "parser": "basiccsv",
-                "encoding": "utf-8-sig",
-                "parameters": {
-                    "timestamp": {
-                        "timestamp": {"index": 0, "format": '"%Y-%m-%d %H:%M:%S.%f"'}
-                    },
-                    "units": {},
-                },
-            },
-            {
-                "nsteps": 1,
-                "step": 0,
-                "nrows": 239,
-                "point": 0,
-                "pars": {"uts": {"value": 1631877974.045}},
-                "errortype": ValueError,
-                "errorexpr": "ufeff",
-            },
-        ),
-    ],
-)
-def test_datagram(input, ts, datadir):
-    ret = datagram_from_input(input, input["parser"], datadir)
-    standard_datagram_test(ret, ts)
-
-    fail_input = input.copy()
-    del fail_input["encoding"]
-    with pytest.raises(ts["errortype"], match=ts["errorexpr"]):
-        datagram_from_input(fail_input, fail_input["parser"], datadir)
+import pytest
+from tests.utils import datagram_from_input, standard_datagram_test
+
+
+@pytest.mark.parametrize(
+    "input, ts",
+    [
+        (
+            {  # ts1 - BOM requires utf-8-sig encoding
+                "case": "log 2021-09-17 11-26-14.140.csv",
+                "parser": "basiccsv",
+                "encoding": "utf-8-sig",
+                "parameters": {
+                    "timestamp": {
+                        "timestamp": {"index": 0, "format": '"%Y-%m-%d %H:%M:%S.%f"'}
+                    },
+                    "units": {},
+                },
+            },
+            {
+                "nsteps": 1,
+                "step": 0,
+                "nrows": 239,
+                "point": 0,
+                "pars": {"uts": {"value": 1631877974.045}},
+                "errortype": ValueError,
+                "errorexpr": "ufeff",
+            },
+        ),
+    ],
+)
+def test_datagram(input, ts, datadir):
+    ret = datagram_from_input(input, input["parser"], datadir)
+    standard_datagram_test(ret, ts)
+
+    fail_input = input.copy()
+    del fail_input["encoding"]
+    with pytest.raises(ts["errortype"], match=ts["errorexpr"]):
+        datagram_from_input(fail_input, fail_input["parser"], datadir)
```

### Comparing `yadg-5.0.1/tests/test_extract.py` & `yadg-5.0.2/tests/test_extract.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-import pytest
-import os
-from yadg.extractors import extract
-import datatree
-from .utils import compare_datatrees
-
-
-@pytest.mark.parametrize(
-    "filetype, infile, outfile",
-    [
-        ("marda:biologic-mpr", "cp.mpr", "ref.cp.mpr.nc"),
-        ("marda:biologic-mpt", "cp.mpt", "ref.cp.mpt.nc"),
-        ("marda:agilent-ch", "hplc.CH", "ref.hplc.ch.nc"),
-        ("marda:agilent-dx", "hplc.dx", "ref.hplc.dx.nc"),
-        ("marda:phi-spe", "xps.spe", "ref.xps.spe.nc"),
-        ("marda:panalytical-xrdml", "xrd.xrdml", "ref.xrd.xrdml.nc"),
-    ],
-)
-def test_extract_marda(filetype, infile, outfile, datadir):
-    os.chdir(datadir)
-    ret = extract(filetype=filetype, path=infile)
-    # ret.to_netcdf(outfile, engine="h5netcdf")
-    ref = datatree.open_datatree(outfile)
-    print(f"{ret=}")
-    compare_datatrees(ret, ref)
+import pytest
+import os
+from yadg.extractors import extract
+import datatree
+from .utils import compare_datatrees
+
+
+@pytest.mark.parametrize(
+    "filetype, infile, outfile",
+    [
+        ("marda:biologic-mpr", "cp.mpr", "ref.cp.mpr.nc"),
+        ("marda:biologic-mpt", "cp.mpt", "ref.cp.mpt.nc"),
+        ("marda:agilent-ch", "hplc.CH", "ref.hplc.ch.nc"),
+        ("marda:agilent-dx", "hplc.dx", "ref.hplc.dx.nc"),
+        ("marda:phi-spe", "xps.spe", "ref.xps.spe.nc"),
+        ("marda:panalytical-xrdml", "xrd.xrdml", "ref.xrd.xrdml.nc"),
+    ],
+)
+def test_extract_marda(filetype, infile, outfile, datadir):
+    os.chdir(datadir)
+    ret = extract(filetype=filetype, path=infile)
+    # ret.to_netcdf(outfile, engine="h5netcdf")
+    ref = datatree.open_datatree(outfile)
+    print(f"{ret=}")
+    compare_datatrees(ret, ref)
```

### Comparing `yadg-5.0.1/tests/test_masstrace.py` & `yadg-5.0.2/tests/test_xpstrace.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,65 +1,59 @@
-import json
-import os
-import pytest
-
-from tests.utils import (
-    datagram_from_input,
-    standard_datagram_test,
-    dg_get_quantity,
-    compare_result_dicts,
-)
-
-# Tests for the quadstar parser:
-# TODO: Implement more thorough tests.
-
-
-@pytest.mark.parametrize(
-    "input, ts",
-    [
-        (  # ts0 - airdemo.sac
-            {"case": "airdemo.sac", "parameters": {"tracetype": "quadstar.sac"}},
-            {
-                "nsteps": 1,
-                "step": 0,
-                "nrows": 21,
-                "point": 0,
-            },
-        ),
-        (  # ts1 - test.sac
-            {"case": "test.sac", "parameters": {"tracetype": "quadstar.sac"}},
-            {
-                "nsteps": 1,
-                "step": 0,
-                "nrows": 188,
-                "point": 0,
-            },
-        ),
-    ],
-)
-def test_datagram_from_quadstar(input, ts, datadir):
-    ret = datagram_from_input(input, "masstrace", datadir)
-    standard_datagram_test(ret, ts)
-
-
-@pytest.mark.parametrize(
-    "input",
-    [
-        (
-            {  # ts0 - test.sac
-                "case": "test.sac",
-                "parameters": {"tracetype": "quadstar.sac"},
-            }
-        ),
-    ],
-)
-def test_masstrace_compare_raw_values(input, datadir):
-    os.chdir(datadir)
-    with open("test_traces.json", "r") as infile:
-        ref = json.load(infile)["traces"]
-    dg = datagram_from_input(input, "masstrace", datadir)
-    step = dg["0"]
-    for k in ["1", "2"]:
-        for kk in ["mass_to_charge", "y"]:
-            print(f"{k=}, {kk=}")
-            ret = dg_get_quantity(step, k, col=kk, utsrow=0)
-            compare_result_dicts(ret, ref[k][kk])
+import json
+import os
+import pytest
+
+from tests.utils import (
+    datagram_from_input,
+    standard_datagram_test,
+    compare_result_dicts,
+    dg_get_quantity,
+)
+
+
+@pytest.mark.parametrize(
+    "input, ts",
+    [
+        (  # ts0 - test0.spe
+            {"case": "test0.spe", "parameters": {"tracetype": "phi.spe"}},
+            {"nsteps": 1, "step": 0, "nrows": 1, "point": 0},
+        ),
+        (  # ts1 - test1.spe
+            {"case": "test1.spe", "parameters": {"tracetype": "phi.spe"}},
+            {"nsteps": 1, "step": 0, "nrows": 1, "point": 0},
+        ),
+        (  # ts2 - check concatenation
+            {
+                "files": ["test0.spe", "test0b.spe"],
+                "parameters": {"tracetype": "phi.spe"},
+            },
+            {"nsteps": 1, "step": 0, "nrows": 2, "point": 0},
+        ),
+    ],
+)
+def test_datagram_from_xpstrace(input, ts, datadir):
+    ret = datagram_from_input(input, "xpstrace", datadir)
+    print(f"{ret=}")
+    standard_datagram_test(ret, ts)
+
+
+@pytest.mark.parametrize(
+    "input",
+    [
+        (
+            {  # ts0 - test0.spe
+                "case": "test0.spe",
+                "parameters": {"tracetype": "phi.spe"},
+            }
+        ),
+    ],
+)
+def test_xpstrace_compare_raw_values(input, datadir):
+    os.chdir(datadir)
+    with open("test0.json", "r") as infile:
+        ref = json.load(infile)["traces"]
+    dg = datagram_from_input(input, "xpstrace", datadir)
+    step = dg["0"]
+    for k in {"1su", "F1s"}:
+        for kk in {"y", "E"}:
+            ret = dg_get_quantity(step, k, col=kk, utsrow=0)
+            compare_result_dicts(ret, ref[k][kk])
```

### Comparing `yadg-5.0.1/tests/test_meascsv.py` & `yadg-5.0.2/tests/test_meascsv.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from tests.utils import (
-    datagram_from_input,
-    standard_datagram_test,
-    dg_get_quantity,
-    compare_result_dicts,
-)
-
-
-def test_datagram_from_meascsv(datadir):
-    input = {
-        "case": "data_3.1.0/00-experiment/measurement.csv",
-        "parameters": {},
-    }
-    ret = datagram_from_input(input, "meascsv", datadir)
-    standard_datagram_test(ret, {"nsteps": 1, "step": 0, "nrows": 1662, "point": 0})
-
-    val = dg_get_quantity(ret, step="0", col="T_f", utsrow=0)
-    compare_result_dicts(val, {"n": 20.9, "s": 0.1, "u": "degC"})
-
-    val = dg_get_quantity(ret, step=0, col="T_f", utsrow=100)
-    compare_result_dicts(val, {"n": 455.1, "s": 0.1, "u": "degC"})
+from tests.utils import (
+    datagram_from_input,
+    standard_datagram_test,
+    dg_get_quantity,
+    compare_result_dicts,
+)
+
+
+def test_datagram_from_meascsv(datadir):
+    input = {
+        "case": "data_3.1.0/00-experiment/measurement.csv",
+        "parameters": {},
+    }
+    ret = datagram_from_input(input, "meascsv", datadir)
+    standard_datagram_test(ret, {"nsteps": 1, "step": 0, "nrows": 1662, "point": 0})
+
+    val = dg_get_quantity(ret, step="0", col="T_f", utsrow=0)
+    compare_result_dicts(val, {"n": 20.9, "s": 0.1, "u": "degC"})
+
+    val = dg_get_quantity(ret, step=0, col="T_f", utsrow=100)
+    compare_result_dicts(val, {"n": 455.1, "s": 0.1, "u": "degC"})
```

### Comparing `yadg-5.0.1/tests/test_preset.py` & `yadg-5.0.2/tests/test_preset.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-import pytest
-import os
-import json
-from tests.utils import standard_datagram_test
-from dgbowl_schemas.yadg import to_dataschema
-
-import yadg.dgutils
-import yadg.core
-
-
-@pytest.mark.parametrize(
-    "input, ts",
-    [
-        ("data_1", {"nsteps": 2, "step": 0, "nrows": 1662}),
-        ("data_2", {"nsteps": 2, "step": 0, "nrows": 2}),
-    ],
-)
-def test_preset(input, ts, datadir):
-    os.chdir(datadir)
-
-    with open(f"{input}.preset.json") as infile:
-        preset = json.load(infile)
-
-    schema = to_dataschema(**preset)
-    while hasattr(schema, "update"):
-        schema = schema.update()
-    ds = yadg.dgutils.schema_from_preset(schema, input)
-
-    ret = yadg.core.process_schema(ds)
-    standard_datagram_test(ret, ts)
+import pytest
+import os
+import json
+from tests.utils import standard_datagram_test
+from dgbowl_schemas.yadg import to_dataschema
+
+import yadg.dgutils
+import yadg.core
+
+
+@pytest.mark.parametrize(
+    "input, ts",
+    [
+        ("data_1", {"nsteps": 2, "step": 0, "nrows": 1662}),
+        ("data_2", {"nsteps": 2, "step": 0, "nrows": 2}),
+    ],
+)
+def test_preset(input, ts, datadir):
+    os.chdir(datadir)
+
+    with open(f"{input}.preset.json") as infile:
+        preset = json.load(infile)
+
+    schema = to_dataschema(**preset)
+    while hasattr(schema, "update"):
+        schema = schema.update()
+    ds = yadg.dgutils.schema_from_preset(schema, input)
+
+    ret = yadg.core.process_schema(ds)
+    standard_datagram_test(ret, ts)
```

### Comparing `yadg-5.0.1/tests/test_qftrace.py` & `yadg-5.0.2/tests/test_qftrace.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-import pytest
-import os
-import json
-from tests.utils import (
-    datagram_from_input,
-    standard_datagram_test,
-    compare_result_dicts,
-    dg_get_quantity,
-)
-
-
-@pytest.mark.parametrize(
-    "input, ts",
-    [
-        (
-            {  # ts0 - 01-inert
-                "folders": ["data_3.1.0/01-inert"],
-                "parameters": {},
-            },
-            {
-                "nsteps": 1,
-                "step": 0,
-                "nrows": 1,
-                "point": 0,
-                "tracelen": 20001,
-                "npeaks": 2,
-                "peak": 0,
-                "test": {
-                    "S11": {
-                        "i": 0,
-                        "f": {"n": 7.1e9, "s": 1e3, "u": "Hz"},
-                        "re": {"n": -0.0192804, "s": 1e-8, "u": " "},
-                        "im": {"n": 0.9448405, "s": 1e-7, "u": " "},
-                    }
-                },
-            },
-        )
-    ],
-)
-def test_datagram_from_qftrace(input, ts, datadir):
-    os.chdir(datadir)
-    dg = datagram_from_input(input, "qftrace", datadir)
-    step = dg["0"]
-    standard_datagram_test(step, ts)
-    for k, v in {
-        "freq": {"n": 7.1e9, "s": 1e3, "u": "Hz"},
-        "Re(G)": {"n": -0.0192804, "s": 1e-8, "u": None},
-        "Im(G)": {"n": 0.9448405, "s": 1e-7, "u": None},
-    }.items():
-        ret = dg_get_quantity(step, "S11", col=k, utsrow=0)
-        print(f"{ret=}")
-        point = {"n": ret["n"][0], "s": ret["s"][0], "u": ret["u"]}
-        compare_result_dicts(point, v)
-
-
-def test_qftrace_compare_raw_values(datadir):
-    input = {
-        "folders": ["data_3.1.0/01-inert"],
-        "parameters": {},
-    }
-    os.chdir(datadir)
-    dg = datagram_from_input(input, "qftrace", datadir)
-    step = dg["0"]
-    with open("yvals.json", "r") as infile:
-        ref = json.load(infile)["traces"]["S11"]
-    for k in {"freq", "Re(G)", "Im(G)"}:
-        ret = dg_get_quantity(step, "S11", col=k, utsrow=0)
-        print(f"{ret=}")
-        compare_result_dicts(ret, ref[k])
+import pytest
+import os
+import json
+from tests.utils import (
+    datagram_from_input,
+    standard_datagram_test,
+    compare_result_dicts,
+    dg_get_quantity,
+)
+
+
+@pytest.mark.parametrize(
+    "input, ts",
+    [
+        (
+            {  # ts0 - 01-inert
+                "folders": ["data_3.1.0/01-inert"],
+                "parameters": {},
+            },
+            {
+                "nsteps": 1,
+                "step": 0,
+                "nrows": 1,
+                "point": 0,
+                "tracelen": 20001,
+                "npeaks": 2,
+                "peak": 0,
+                "test": {
+                    "S11": {
+                        "i": 0,
+                        "f": {"n": 7.1e9, "s": 1e3, "u": "Hz"},
+                        "re": {"n": -0.0192804, "s": 1e-8, "u": " "},
+                        "im": {"n": 0.9448405, "s": 1e-7, "u": " "},
+                    }
+                },
+            },
+        )
+    ],
+)
+def test_datagram_from_qftrace(input, ts, datadir):
+    os.chdir(datadir)
+    dg = datagram_from_input(input, "qftrace", datadir)
+    step = dg["0"]
+    standard_datagram_test(step, ts)
+    for k, v in {
+        "freq": {"n": 7.1e9, "s": 1e3, "u": "Hz"},
+        "Re(G)": {"n": -0.0192804, "s": 1e-8, "u": None},
+        "Im(G)": {"n": 0.9448405, "s": 1e-7, "u": None},
+    }.items():
+        ret = dg_get_quantity(step, "S11", col=k, utsrow=0)
+        print(f"{ret=}")
+        point = {"n": ret["n"][0], "s": ret["s"][0], "u": ret["u"]}
+        compare_result_dicts(point, v)
+
+
+def test_qftrace_compare_raw_values(datadir):
+    input = {
+        "folders": ["data_3.1.0/01-inert"],
+        "parameters": {},
+    }
+    os.chdir(datadir)
+    dg = datagram_from_input(input, "qftrace", datadir)
+    step = dg["0"]
+    with open("yvals.json", "r") as infile:
+        ref = json.load(infile)["traces"]["S11"]
+    for k in {"freq", "Re(G)", "Im(G)"}:
+        ret = dg_get_quantity(step, "S11", col=k, utsrow=0)
+        print(f"{ret=}")
+        compare_result_dicts(ret, ref[k])
```

### Comparing `yadg-5.0.1/versioneer.py` & `yadg-5.0.2/versioneer.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,2189 +1,2189 @@
-# Version: 0.22
-
-"""The Versioneer - like a rocketeer, but for versions.
-
-The Versioneer
-==============
-
-* like a rocketeer, but for versions!
-* https://github.com/python-versioneer/python-versioneer
-* Brian Warner
-* License: Public Domain
-* Compatible with: Python 3.6, 3.7, 3.8, 3.9, 3.10 and pypy3
-* [![Latest Version][pypi-image]][pypi-url]
-* [![Build Status][travis-image]][travis-url]
-
-This is a tool for managing a recorded version number in distutils/setuptools-based
-python projects. The goal is to remove the tedious and error-prone "update
-the embedded version string" step from your release process. Making a new
-release should be as easy as recording a new tag in your version-control
-system, and maybe making new tarballs.
-
-
-## Quick Install
-
-* `pip install versioneer` to somewhere in your $PATH
-* add a `[versioneer]` section to your setup.cfg (see [Install](INSTALL.md))
-* run `versioneer install` in your source tree, commit the results
-* Verify version information with `python setup.py version`
-
-## Version Identifiers
-
-Source trees come from a variety of places:
-
-* a version-control system checkout (mostly used by developers)
-* a nightly tarball, produced by build automation
-* a snapshot tarball, produced by a web-based VCS browser, like github's
-  "tarball from tag" feature
-* a release tarball, produced by "setup.py sdist", distributed through PyPI
-
-Within each source tree, the version identifier (either a string or a number,
-this tool is format-agnostic) can come from a variety of places:
-
-* ask the VCS tool itself, e.g. "git describe" (for checkouts), which knows
-  about recent "tags" and an absolute revision-id
-* the name of the directory into which the tarball was unpacked
-* an expanded VCS keyword ($Id$, etc)
-* a `_version.py` created by some earlier build step
-
-For released software, the version identifier is closely related to a VCS
-tag. Some projects use tag names that include more than just the version
-string (e.g. "myproject-1.2" instead of just "1.2"), in which case the tool
-needs to strip the tag prefix to extract the version identifier. For
-unreleased software (between tags), the version identifier should provide
-enough information to help developers recreate the same tree, while also
-giving them an idea of roughly how old the tree is (after version 1.2, before
-version 1.3). Many VCS systems can report a description that captures this,
-for example `git describe --tags --dirty --always` reports things like
-"0.7-1-g574ab98-dirty" to indicate that the checkout is one revision past the
-0.7 tag, has a unique revision id of "574ab98", and is "dirty" (it has
-uncommitted changes).
-
-The version identifier is used for multiple purposes:
-
-* to allow the module to self-identify its version: `myproject.__version__`
-* to choose a name and prefix for a 'setup.py sdist' tarball
-
-## Theory of Operation
-
-Versioneer works by adding a special `_version.py` file into your source
-tree, where your `__init__.py` can import it. This `_version.py` knows how to
-dynamically ask the VCS tool for version information at import time.
-
-`_version.py` also contains `$Revision$` markers, and the installation
-process marks `_version.py` to have this marker rewritten with a tag name
-during the `git archive` command. As a result, generated tarballs will
-contain enough information to get the proper version.
-
-To allow `setup.py` to compute a version too, a `versioneer.py` is added to
-the top level of your source tree, next to `setup.py` and the `setup.cfg`
-that configures it. This overrides several distutils/setuptools commands to
-compute the version when invoked, and changes `setup.py build` and `setup.py
-sdist` to replace `_version.py` with a small static file that contains just
-the generated version data.
-
-## Installation
-
-See [INSTALL.md](./INSTALL.md) for detailed installation instructions.
-
-## Version-String Flavors
-
-Code which uses Versioneer can learn about its version string at runtime by
-importing `_version` from your main `__init__.py` file and running the
-`get_versions()` function. From the "outside" (e.g. in `setup.py`), you can
-import the top-level `versioneer.py` and run `get_versions()`.
-
-Both functions return a dictionary with different flavors of version
-information:
-
-* `['version']`: A condensed version string, rendered using the selected
-  style. This is the most commonly used value for the project's version
-  string. The default "pep440" style yields strings like `0.11`,
-  `0.11+2.g1076c97`, or `0.11+2.g1076c97.dirty`. See the "Styles" section
-  below for alternative styles.
-
-* `['full-revisionid']`: detailed revision identifier. For Git, this is the
-  full SHA1 commit id, e.g. "1076c978a8d3cfc70f408fe5974aa6c092c949ac".
-
-* `['date']`: Date and time of the latest `HEAD` commit. For Git, it is the
-  commit date in ISO 8601 format. This will be None if the date is not
-  available.
-
-* `['dirty']`: a boolean, True if the tree has uncommitted changes. Note that
-  this is only accurate if run in a VCS checkout, otherwise it is likely to
-  be False or None
-
-* `['error']`: if the version string could not be computed, this will be set
-  to a string describing the problem, otherwise it will be None. It may be
-  useful to throw an exception in setup.py if this is set, to avoid e.g.
-  creating tarballs with a version string of "unknown".
-
-Some variants are more useful than others. Including `full-revisionid` in a
-bug report should allow developers to reconstruct the exact code being tested
-(or indicate the presence of local changes that should be shared with the
-developers). `version` is suitable for display in an "about" box or a CLI
-`--version` output: it can be easily compared against release notes and lists
-of bugs fixed in various releases.
-
-The installer adds the following text to your `__init__.py` to place a basic
-version in `YOURPROJECT.__version__`:
-
-    from ._version import get_versions
-    __version__ = get_versions()['version']
-    del get_versions
-
-## Styles
-
-The setup.cfg `style=` configuration controls how the VCS information is
-rendered into a version string.
-
-The default style, "pep440", produces a PEP440-compliant string, equal to the
-un-prefixed tag name for actual releases, and containing an additional "local
-version" section with more detail for in-between builds. For Git, this is
-TAG[+DISTANCE.gHEX[.dirty]] , using information from `git describe --tags
---dirty --always`. For example "0.11+2.g1076c97.dirty" indicates that the
-tree is like the "1076c97" commit but has uncommitted changes (".dirty"), and
-that this commit is two revisions ("+2") beyond the "0.11" tag. For released
-software (exactly equal to a known tag), the identifier will only contain the
-stripped tag, e.g. "0.11".
-
-Other styles are available. See [details.md](details.md) in the Versioneer
-source tree for descriptions.
-
-## Debugging
-
-Versioneer tries to avoid fatal errors: if something goes wrong, it will tend
-to return a version of "0+unknown". To investigate the problem, run `setup.py
-version`, which will run the version-lookup code in a verbose mode, and will
-display the full contents of `get_versions()` (including the `error` string,
-which may help identify what went wrong).
-
-## Known Limitations
-
-Some situations are known to cause problems for Versioneer. This details the
-most significant ones. More can be found on Github
-[issues page](https://github.com/python-versioneer/python-versioneer/issues).
-
-### Subprojects
-
-Versioneer has limited support for source trees in which `setup.py` is not in
-the root directory (e.g. `setup.py` and `.git/` are *not* siblings). The are
-two common reasons why `setup.py` might not be in the root:
-
-* Source trees which contain multiple subprojects, such as
-  [Buildbot](https://github.com/buildbot/buildbot), which contains both
-  "master" and "slave" subprojects, each with their own `setup.py`,
-  `setup.cfg`, and `tox.ini`. Projects like these produce multiple PyPI
-  distributions (and upload multiple independently-installable tarballs).
-* Source trees whose main purpose is to contain a C library, but which also
-  provide bindings to Python (and perhaps other languages) in subdirectories.
-
-Versioneer will look for `.git` in parent directories, and most operations
-should get the right version string. However `pip` and `setuptools` have bugs
-and implementation details which frequently cause `pip install .` from a
-subproject directory to fail to find a correct version string (so it usually
-defaults to `0+unknown`).
-
-`pip install --editable .` should work correctly. `setup.py install` might
-work too.
-
-Pip-8.1.1 is known to have this problem, but hopefully it will get fixed in
-some later version.
-
-[Bug #38](https://github.com/python-versioneer/python-versioneer/issues/38) is tracking
-this issue. The discussion in
-[PR #61](https://github.com/python-versioneer/python-versioneer/pull/61) describes the
-issue from the Versioneer side in more detail.
-[pip PR#3176](https://github.com/pypa/pip/pull/3176) and
-[pip PR#3615](https://github.com/pypa/pip/pull/3615) contain work to improve
-pip to let Versioneer work correctly.
-
-Versioneer-0.16 and earlier only looked for a `.git` directory next to the
-`setup.cfg`, so subprojects were completely unsupported with those releases.
-
-### Editable installs with setuptools <= 18.5
-
-`setup.py develop` and `pip install --editable .` allow you to install a
-project into a virtualenv once, then continue editing the source code (and
-test) without re-installing after every change.
-
-"Entry-point scripts" (`setup(entry_points={"console_scripts": ..})`) are a
-convenient way to specify executable scripts that should be installed along
-with the python package.
-
-These both work as expected when using modern setuptools. When using
-setuptools-18.5 or earlier, however, certain operations will cause
-`pkg_resources.DistributionNotFound` errors when running the entrypoint
-script, which must be resolved by re-installing the package. This happens
-when the install happens with one version, then the egg_info data is
-regenerated while a different version is checked out. Many setup.py commands
-cause egg_info to be rebuilt (including `sdist`, `wheel`, and installing into
-a different virtualenv), so this can be surprising.
-
-[Bug #83](https://github.com/python-versioneer/python-versioneer/issues/83) describes
-this one, but upgrading to a newer version of setuptools should probably
-resolve it.
-
-
-## Updating Versioneer
-
-To upgrade your project to a new release of Versioneer, do the following:
-
-* install the new Versioneer (`pip install -U versioneer` or equivalent)
-* edit `setup.cfg`, if necessary, to include any new configuration settings
-  indicated by the release notes. See [UPGRADING](./UPGRADING.md) for details.
-* re-run `versioneer install` in your source tree, to replace
-  `SRC/_version.py`
-* commit any changed files
-
-## Future Directions
-
-This tool is designed to make it easily extended to other version-control
-systems: all VCS-specific components are in separate directories like
-src/git/ . The top-level `versioneer.py` script is assembled from these
-components by running make-versioneer.py . In the future, make-versioneer.py
-will take a VCS name as an argument, and will construct a version of
-`versioneer.py` that is specific to the given VCS. It might also take the
-configuration arguments that are currently provided manually during
-installation by editing setup.py . Alternatively, it might go the other
-direction and include code from all supported VCS systems, reducing the
-number of intermediate scripts.
-
-## Similar projects
-
-* [setuptools_scm](https://github.com/pypa/setuptools_scm/) - a non-vendored build-time
-  dependency
-* [minver](https://github.com/jbweston/miniver) - a lightweight reimplementation of
-  versioneer
-* [versioningit](https://github.com/jwodder/versioningit) - a PEP 518-based setuptools
-  plugin
-
-## License
-
-To make Versioneer easier to embed, all its code is dedicated to the public
-domain. The `_version.py` that it creates is also in the public domain.
-Specifically, both are released under the Creative Commons "Public Domain
-Dedication" license (CC0-1.0), as described in
-https://creativecommons.org/publicdomain/zero/1.0/ .
-
-[pypi-image]: https://img.shields.io/pypi/v/versioneer.svg
-[pypi-url]: https://pypi.python.org/pypi/versioneer/
-[travis-image]:
-https://img.shields.io/travis/com/python-versioneer/python-versioneer.svg
-[travis-url]: https://travis-ci.com/github/python-versioneer/python-versioneer
-
-"""
-# pylint:disable=invalid-name,import-outside-toplevel,missing-function-docstring
-# pylint:disable=missing-class-docstring,too-many-branches,too-many-statements
-# pylint:disable=raise-missing-from,too-many-lines,too-many-locals,import-error
-# pylint:disable=too-few-public-methods,redefined-outer-name,consider-using-with
-# pylint:disable=attribute-defined-outside-init,too-many-arguments
-
-import configparser
-import errno
-import json
-import os
-import re
-import subprocess
-import sys
-from typing import Callable, Dict
-import functools
-
-
-class VersioneerConfig:
-    """Container for Versioneer configuration parameters."""
-
-
-def get_root():
-    """Get the project root directory.
-
-    We require that all commands are run from the project root, i.e. the
-    directory that contains setup.py, setup.cfg, and versioneer.py .
-    """
-    root = os.path.realpath(os.path.abspath(os.getcwd()))
-    setup_py = os.path.join(root, "setup.py")
-    versioneer_py = os.path.join(root, "versioneer.py")
-    if not (os.path.exists(setup_py) or os.path.exists(versioneer_py)):
-        # allow 'python path/to/setup.py COMMAND'
-        root = os.path.dirname(os.path.realpath(os.path.abspath(sys.argv[0])))
-        setup_py = os.path.join(root, "setup.py")
-        versioneer_py = os.path.join(root, "versioneer.py")
-    if not (os.path.exists(setup_py) or os.path.exists(versioneer_py)):
-        err = (
-            "Versioneer was unable to run the project root directory. "
-            "Versioneer requires setup.py to be executed from "
-            "its immediate directory (like 'python setup.py COMMAND'), "
-            "or in a way that lets it use sys.argv[0] to find the root "
-            "(like 'python path/to/setup.py COMMAND')."
-        )
-        raise VersioneerBadRootError(err)
-    try:
-        # Certain runtime workflows (setup.py install/develop in a setuptools
-        # tree) execute all dependencies in a single python process, so
-        # "versioneer" may be imported multiple times, and python's shared
-        # module-import table will cache the first one. So we can't use
-        # os.path.dirname(__file__), as that will find whichever
-        # versioneer.py was first imported, even in later projects.
-        my_path = os.path.realpath(os.path.abspath(__file__))
-        me_dir = os.path.normcase(os.path.splitext(my_path)[0])
-        vsr_dir = os.path.normcase(os.path.splitext(versioneer_py)[0])
-        if me_dir != vsr_dir:
-            print(
-                "Warning: build in %s is using versioneer.py from %s"
-                % (os.path.dirname(my_path), versioneer_py)
-            )
-    except NameError:
-        pass
-    return root
-
-
-def get_config_from_root(root):
-    """Read the project setup.cfg file to determine Versioneer config."""
-    # This might raise OSError (if setup.cfg is missing), or
-    # configparser.NoSectionError (if it lacks a [versioneer] section), or
-    # configparser.NoOptionError (if it lacks "VCS="). See the docstring at
-    # the top of versioneer.py for instructions on writing your setup.cfg .
-    setup_cfg = os.path.join(root, "setup.cfg")
-    parser = configparser.ConfigParser()
-    with open(setup_cfg, "r") as cfg_file:
-        parser.read_file(cfg_file)
-    VCS = parser.get("versioneer", "VCS")  # mandatory
-
-    # Dict-like interface for non-mandatory entries
-    section = parser["versioneer"]
-
-    cfg = VersioneerConfig()
-    cfg.VCS = VCS
-    cfg.style = section.get("style", "")
-    cfg.versionfile_source = section.get("versionfile_source")
-    cfg.versionfile_build = section.get("versionfile_build")
-    cfg.tag_prefix = section.get("tag_prefix")
-    if cfg.tag_prefix in ("''", '""'):
-        cfg.tag_prefix = ""
-    cfg.parentdir_prefix = section.get("parentdir_prefix")
-    cfg.verbose = section.get("verbose")
-    return cfg
-
-
-class NotThisMethod(Exception):
-    """Exception raised if a method is not valid for the current scenario."""
-
-
-# these dictionaries contain VCS-specific tools
-LONG_VERSION_PY: Dict[str, str] = {}
-HANDLERS: Dict[str, Dict[str, Callable]] = {}
-
-
-def register_vcs_handler(vcs, method):  # decorator
-    """Create decorator to mark a method as the handler of a VCS."""
-
-    def decorate(f):
-        """Store f in HANDLERS[vcs][method]."""
-        HANDLERS.setdefault(vcs, {})[method] = f
-        return f
-
-    return decorate
-
-
-def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False, env=None):
-    """Call the given command(s)."""
-    assert isinstance(commands, list)
-    process = None
-
-    popen_kwargs = {}
-    if sys.platform == "win32":
-        # This hides the console window if pythonw.exe is used
-        startupinfo = subprocess.STARTUPINFO()
-        startupinfo.dwFlags |= subprocess.STARTF_USESHOWWINDOW
-        popen_kwargs["startupinfo"] = startupinfo
-
-    for command in commands:
-        dispcmd = str([command] + args)
-        try:
-            # remember shell=False, so use git.cmd on windows, not just git
-            process = subprocess.Popen(
-                [command] + args,
-                cwd=cwd,
-                env=env,
-                stdout=subprocess.PIPE,
-                stderr=(subprocess.PIPE if hide_stderr else None),
-                **popen_kwargs,
-            )
-            break
-        except OSError:
-            e = sys.exc_info()[1]
-            if e.errno == errno.ENOENT:
-                continue
-            if verbose:
-                print("unable to run %s" % dispcmd)
-                print(e)
-            return None, None
-    else:
-        if verbose:
-            print("unable to find command, tried %s" % (commands,))
-        return None, None
-    stdout = process.communicate()[0].strip().decode()
-    if process.returncode != 0:
-        if verbose:
-            print("unable to run %s (error)" % dispcmd)
-            print("stdout was %s" % stdout)
-        return None, process.returncode
-    return stdout, process.returncode
-
-
-LONG_VERSION_PY[
-    "git"
-] = r'''
-# This file helps to compute a version number in source trees obtained from
-# git-archive tarball (such as those provided by githubs download-from-tag
-# feature). Distribution tarballs (built by setup.py sdist) and build
-# directories (produced by setup.py build) will contain a much shorter file
-# that just contains the computed version number.
-
-# This file is released into the public domain. Generated by
-# versioneer-0.22 (https://github.com/python-versioneer/python-versioneer)
-
-"""Git implementation of _version.py."""
-
-import errno
-import os
-import re
-import subprocess
-import sys
-from typing import Callable, Dict
-import functools
-
-
-def get_keywords():
-    """Get the keywords needed to look up the version information."""
-    # these strings will be replaced by git during git-archive.
-    # setup.py/versioneer.py will grep for the variable names, so they must
-    # each be defined on a line of their own. _version.py will just call
-    # get_keywords().
-    git_refnames = "%(DOLLAR)sFormat:%%d%(DOLLAR)s"
-    git_full = "%(DOLLAR)sFormat:%%H%(DOLLAR)s"
-    git_date = "%(DOLLAR)sFormat:%%ci%(DOLLAR)s"
-    keywords = {"refnames": git_refnames, "full": git_full, "date": git_date}
-    return keywords
-
-
-class VersioneerConfig:
-    """Container for Versioneer configuration parameters."""
-
-
-def get_config():
-    """Create, populate and return the VersioneerConfig() object."""
-    # these strings are filled in when 'setup.py versioneer' creates
-    # _version.py
-    cfg = VersioneerConfig()
-    cfg.VCS = "git"
-    cfg.style = "%(STYLE)s"
-    cfg.tag_prefix = "%(TAG_PREFIX)s"
-    cfg.parentdir_prefix = "%(PARENTDIR_PREFIX)s"
-    cfg.versionfile_source = "%(VERSIONFILE_SOURCE)s"
-    cfg.verbose = False
-    return cfg
-
-
-class NotThisMethod(Exception):
-    """Exception raised if a method is not valid for the current scenario."""
-
-
-LONG_VERSION_PY: Dict[str, str] = {}
-HANDLERS: Dict[str, Dict[str, Callable]] = {}
-
-
-def register_vcs_handler(vcs, method):  # decorator
-    """Create decorator to mark a method as the handler of a VCS."""
-    def decorate(f):
-        """Store f in HANDLERS[vcs][method]."""
-        if vcs not in HANDLERS:
-            HANDLERS[vcs] = {}
-        HANDLERS[vcs][method] = f
-        return f
-    return decorate
-
-
-def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False,
-                env=None):
-    """Call the given command(s)."""
-    assert isinstance(commands, list)
-    process = None
-
-    popen_kwargs = {}
-    if sys.platform == "win32":
-        # This hides the console window if pythonw.exe is used
-        startupinfo = subprocess.STARTUPINFO()
-        startupinfo.dwFlags |= subprocess.STARTF_USESHOWWINDOW
-        popen_kwargs["startupinfo"] = startupinfo
-
-    for command in commands:
-        try:
-            dispcmd = str([command] + args)
-            # remember shell=False, so use git.cmd on windows, not just git
-            process = subprocess.Popen([command] + args, cwd=cwd, env=env,
-                                       stdout=subprocess.PIPE,
-                                       stderr=(subprocess.PIPE if hide_stderr
-                                               else None), **popen_kwargs)
-            break
-        except OSError:
-            e = sys.exc_info()[1]
-            if e.errno == errno.ENOENT:
-                continue
-            if verbose:
-                print("unable to run %%s" %% dispcmd)
-                print(e)
-            return None, None
-    else:
-        if verbose:
-            print("unable to find command, tried %%s" %% (commands,))
-        return None, None
-    stdout = process.communicate()[0].strip().decode()
-    if process.returncode != 0:
-        if verbose:
-            print("unable to run %%s (error)" %% dispcmd)
-            print("stdout was %%s" %% stdout)
-        return None, process.returncode
-    return stdout, process.returncode
-
-
-def versions_from_parentdir(parentdir_prefix, root, verbose):
-    """Try to determine the version from the parent directory name.
-
-    Source tarballs conventionally unpack into a directory that includes both
-    the project name and a version string. We will also support searching up
-    two directory levels for an appropriately named parent directory
-    """
-    rootdirs = []
-
-    for _ in range(3):
-        dirname = os.path.basename(root)
-        if dirname.startswith(parentdir_prefix):
-            return {"version": dirname[len(parentdir_prefix):],
-                    "full-revisionid": None,
-                    "dirty": False, "error": None, "date": None}
-        rootdirs.append(root)
-        root = os.path.dirname(root)  # up a level
-
-    if verbose:
-        print("Tried directories %%s but none started with prefix %%s" %%
-              (str(rootdirs), parentdir_prefix))
-    raise NotThisMethod("rootdir doesn't start with parentdir_prefix")
-
-
-@register_vcs_handler("git", "get_keywords")
-def git_get_keywords(versionfile_abs):
-    """Extract version information from the given file."""
-    # the code embedded in _version.py can just fetch the value of these
-    # keywords. When used from setup.py, we don't want to import _version.py,
-    # so we do it with a regexp instead. This function is not used from
-    # _version.py.
-    keywords = {}
-    try:
-        with open(versionfile_abs, "r") as fobj:
-            for line in fobj:
-                if line.strip().startswith("git_refnames ="):
-                    mo = re.search(r'=\s*"(.*)"', line)
-                    if mo:
-                        keywords["refnames"] = mo.group(1)
-                if line.strip().startswith("git_full ="):
-                    mo = re.search(r'=\s*"(.*)"', line)
-                    if mo:
-                        keywords["full"] = mo.group(1)
-                if line.strip().startswith("git_date ="):
-                    mo = re.search(r'=\s*"(.*)"', line)
-                    if mo:
-                        keywords["date"] = mo.group(1)
-    except OSError:
-        pass
-    return keywords
-
-
-@register_vcs_handler("git", "keywords")
-def git_versions_from_keywords(keywords, tag_prefix, verbose):
-    """Get version information from git keywords."""
-    if "refnames" not in keywords:
-        raise NotThisMethod("Short version file found")
-    date = keywords.get("date")
-    if date is not None:
-        # Use only the last line.  Previous lines may contain GPG signature
-        # information.
-        date = date.splitlines()[-1]
-
-        # git-2.2.0 added "%%cI", which expands to an ISO-8601 -compliant
-        # datestamp. However we prefer "%%ci" (which expands to an "ISO-8601
-        # -like" string, which we must then edit to make compliant), because
-        # it's been around since git-1.5.3, and it's too difficult to
-        # discover which version we're using, or to work around using an
-        # older one.
-        date = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
-    refnames = keywords["refnames"].strip()
-    if refnames.startswith("$Format"):
-        if verbose:
-            print("keywords are unexpanded, not using")
-        raise NotThisMethod("unexpanded keywords, not a git-archive tarball")
-    refs = {r.strip() for r in refnames.strip("()").split(",")}
-    # starting in git-1.8.3, tags are listed as "tag: foo-1.0" instead of
-    # just "foo-1.0". If we see a "tag: " prefix, prefer those.
-    TAG = "tag: "
-    tags = {r[len(TAG):] for r in refs if r.startswith(TAG)}
-    if not tags:
-        # Either we're using git < 1.8.3, or there really are no tags. We use
-        # a heuristic: assume all version tags have a digit. The old git %%d
-        # expansion behaves like git log --decorate=short and strips out the
-        # refs/heads/ and refs/tags/ prefixes that would let us distinguish
-        # between branches and tags. By ignoring refnames without digits, we
-        # filter out many common branch names like "release" and
-        # "stabilization", as well as "HEAD" and "master".
-        tags = {r for r in refs if re.search(r'\d', r)}
-        if verbose:
-            print("discarding '%%s', no digits" %% ",".join(refs - tags))
-    if verbose:
-        print("likely tags: %%s" %% ",".join(sorted(tags)))
-    for ref in sorted(tags):
-        # sorting will prefer e.g. "2.0" over "2.0rc1"
-        if ref.startswith(tag_prefix):
-            r = ref[len(tag_prefix):]
-            # Filter out refs that exactly match prefix or that don't start
-            # with a number once the prefix is stripped (mostly a concern
-            # when prefix is '')
-            if not re.match(r'\d', r):
-                continue
-            if verbose:
-                print("picking %%s" %% r)
-            return {"version": r,
-                    "full-revisionid": keywords["full"].strip(),
-                    "dirty": False, "error": None,
-                    "date": date}
-    # no suitable tags, so version is "0+unknown", but full hex is still there
-    if verbose:
-        print("no suitable tags, using unknown + full revision id")
-    return {"version": "0+unknown",
-            "full-revisionid": keywords["full"].strip(),
-            "dirty": False, "error": "no suitable tags", "date": None}
-
-
-@register_vcs_handler("git", "pieces_from_vcs")
-def git_pieces_from_vcs(tag_prefix, root, verbose, runner=run_command):
-    """Get version from 'git describe' in the root of the source tree.
-
-    This only gets called if the git-archive 'subst' keywords were *not*
-    expanded, and _version.py hasn't already been rewritten with a short
-    version string, meaning we're inside a checked out source tree.
-    """
-    GITS = ["git"]
-    if sys.platform == "win32":
-        GITS = ["git.cmd", "git.exe"]
-
-    # GIT_DIR can interfere with correct operation of Versioneer.
-    # It may be intended to be passed to the Versioneer-versioned project,
-    # but that should not change where we get our version from.
-    env = os.environ.copy()
-    env.pop("GIT_DIR", None)
-    runner = functools.partial(runner, env=env)
-
-    _, rc = runner(GITS, ["rev-parse", "--git-dir"], cwd=root,
-                   hide_stderr=True)
-    if rc != 0:
-        if verbose:
-            print("Directory %%s not under git control" %% root)
-        raise NotThisMethod("'git rev-parse --git-dir' returned error")
-
-    MATCH_ARGS = ["--match", "%%s*" %% tag_prefix] if tag_prefix else []
-
-    # if there is a tag matching tag_prefix, this yields TAG-NUM-gHEX[-dirty]
-    # if there isn't one, this yields HEX[-dirty] (no NUM)
-    describe_out, rc = runner(GITS, ["describe", "--tags", "--dirty",
-                                     "--always", "--long", *MATCH_ARGS],
-                              cwd=root)
-    # --long was added in git-1.5.5
-    if describe_out is None:
-        raise NotThisMethod("'git describe' failed")
-    describe_out = describe_out.strip()
-    full_out, rc = runner(GITS, ["rev-parse", "HEAD"], cwd=root)
-    if full_out is None:
-        raise NotThisMethod("'git rev-parse' failed")
-    full_out = full_out.strip()
-
-    pieces = {}
-    pieces["long"] = full_out
-    pieces["short"] = full_out[:7]  # maybe improved later
-    pieces["error"] = None
-
-    branch_name, rc = runner(GITS, ["rev-parse", "--abbrev-ref", "HEAD"],
-                             cwd=root)
-    # --abbrev-ref was added in git-1.6.3
-    if rc != 0 or branch_name is None:
-        raise NotThisMethod("'git rev-parse --abbrev-ref' returned error")
-    branch_name = branch_name.strip()
-
-    if branch_name == "HEAD":
-        # If we aren't exactly on a branch, pick a branch which represents
-        # the current commit. If all else fails, we are on a branchless
-        # commit.
-        branches, rc = runner(GITS, ["branch", "--contains"], cwd=root)
-        # --contains was added in git-1.5.4
-        if rc != 0 or branches is None:
-            raise NotThisMethod("'git branch --contains' returned error")
-        branches = branches.split("\n")
-
-        # Remove the first line if we're running detached
-        if "(" in branches[0]:
-            branches.pop(0)
-
-        # Strip off the leading "* " from the list of branches.
-        branches = [branch[2:] for branch in branches]
-        if "master" in branches:
-            branch_name = "master"
-        elif not branches:
-            branch_name = None
-        else:
-            # Pick the first branch that is returned. Good or bad.
-            branch_name = branches[0]
-
-    pieces["branch"] = branch_name
-
-    # parse describe_out. It will be like TAG-NUM-gHEX[-dirty] or HEX[-dirty]
-    # TAG might have hyphens.
-    git_describe = describe_out
-
-    # look for -dirty suffix
-    dirty = git_describe.endswith("-dirty")
-    pieces["dirty"] = dirty
-    if dirty:
-        git_describe = git_describe[:git_describe.rindex("-dirty")]
-
-    # now we have TAG-NUM-gHEX or HEX
-
-    if "-" in git_describe:
-        # TAG-NUM-gHEX
-        mo = re.search(r'^(.+)-(\d+)-g([0-9a-f]+)$', git_describe)
-        if not mo:
-            # unparsable. Maybe git-describe is misbehaving?
-            pieces["error"] = ("unable to parse git-describe output: '%%s'"
-                               %% describe_out)
-            return pieces
-
-        # tag
-        full_tag = mo.group(1)
-        if not full_tag.startswith(tag_prefix):
-            if verbose:
-                fmt = "tag '%%s' doesn't start with prefix '%%s'"
-                print(fmt %% (full_tag, tag_prefix))
-            pieces["error"] = ("tag '%%s' doesn't start with prefix '%%s'"
-                               %% (full_tag, tag_prefix))
-            return pieces
-        pieces["closest-tag"] = full_tag[len(tag_prefix):]
-
-        # distance: number of commits since tag
-        pieces["distance"] = int(mo.group(2))
-
-        # commit: short hex revision ID
-        pieces["short"] = mo.group(3)
-
-    else:
-        # HEX: no tags
-        pieces["closest-tag"] = None
-        count_out, rc = runner(GITS, ["rev-list", "HEAD", "--count"], cwd=root)
-        pieces["distance"] = int(count_out)  # total number of commits
-
-    # commit date: see ISO-8601 comment in git_versions_from_keywords()
-    date = runner(GITS, ["show", "-s", "--format=%%ci", "HEAD"], cwd=root)[0].strip()
-    # Use only the last line.  Previous lines may contain GPG signature
-    # information.
-    date = date.splitlines()[-1]
-    pieces["date"] = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
-
-    return pieces
-
-
-def plus_or_dot(pieces):
-    """Return a + if we don't already have one, else return a ."""
-    if "+" in pieces.get("closest-tag", ""):
-        return "."
-    return "+"
-
-
-def render_pep440(pieces):
-    """Build up version string, with post-release "local version identifier".
-
-    Our goal: TAG[+DISTANCE.gHEX[.dirty]] . Note that if you
-    get a tagged build and then dirty it, you'll get TAG+0.gHEX.dirty
-
-    Exceptions:
-    1: no tags. git_describe was just HEX. 0+untagged.DISTANCE.gHEX[.dirty]
-    """
-    if pieces["closest-tag"]:
-        rendered = pieces["closest-tag"]
-        if pieces["distance"] or pieces["dirty"]:
-            rendered += plus_or_dot(pieces)
-            rendered += "%%d.g%%s" %% (pieces["distance"], pieces["short"])
-            if pieces["dirty"]:
-                rendered += ".dirty"
-    else:
-        # exception #1
-        rendered = "0+untagged.%%d.g%%s" %% (pieces["distance"],
-                                          pieces["short"])
-        if pieces["dirty"]:
-            rendered += ".dirty"
-    return rendered
-
-
-def render_pep440_branch(pieces):
-    """TAG[[.dev0]+DISTANCE.gHEX[.dirty]] .
-
-    The ".dev0" means not master branch. Note that .dev0 sorts backwards
-    (a feature branch will appear "older" than the master branch).
-
-    Exceptions:
-    1: no tags. 0[.dev0]+untagged.DISTANCE.gHEX[.dirty]
-    """
-    if pieces["closest-tag"]:
-        rendered = pieces["closest-tag"]
-        if pieces["distance"] or pieces["dirty"]:
-            if pieces["branch"] != "master":
-                rendered += ".dev0"
-            rendered += plus_or_dot(pieces)
-            rendered += "%%d.g%%s" %% (pieces["distance"], pieces["short"])
-            if pieces["dirty"]:
-                rendered += ".dirty"
-    else:
-        # exception #1
-        rendered = "0"
-        if pieces["branch"] != "master":
-            rendered += ".dev0"
-        rendered += "+untagged.%%d.g%%s" %% (pieces["distance"],
-                                          pieces["short"])
-        if pieces["dirty"]:
-            rendered += ".dirty"
-    return rendered
-
-
-def pep440_split_post(ver):
-    """Split pep440 version string at the post-release segment.
-
-    Returns the release segments before the post-release and the
-    post-release version number (or -1 if no post-release segment is present).
-    """
-    vc = str.split(ver, ".post")
-    return vc[0], int(vc[1] or 0) if len(vc) == 2 else None
-
-
-def render_pep440_pre(pieces):
-    """TAG[.postN.devDISTANCE] -- No -dirty.
-
-    Exceptions:
-    1: no tags. 0.post0.devDISTANCE
-    """
-    if pieces["closest-tag"]:
-        if pieces["distance"]:
-            # update the post release segment
-            tag_version, post_version = pep440_split_post(pieces["closest-tag"])
-            rendered = tag_version
-            if post_version is not None:
-                rendered += ".post%%d.dev%%d" %% (post_version+1, pieces["distance"])
-            else:
-                rendered += ".post0.dev%%d" %% (pieces["distance"])
-        else:
-            # no commits, use the tag as the version
-            rendered = pieces["closest-tag"]
-    else:
-        # exception #1
-        rendered = "0.post0.dev%%d" %% pieces["distance"]
-    return rendered
-
-
-def render_pep440_post(pieces):
-    """TAG[.postDISTANCE[.dev0]+gHEX] .
-
-    The ".dev0" means dirty. Note that .dev0 sorts backwards
-    (a dirty tree will appear "older" than the corresponding clean one),
-    but you shouldn't be releasing software with -dirty anyways.
-
-    Exceptions:
-    1: no tags. 0.postDISTANCE[.dev0]
-    """
-    if pieces["closest-tag"]:
-        rendered = pieces["closest-tag"]
-        if pieces["distance"] or pieces["dirty"]:
-            rendered += ".post%%d" %% pieces["distance"]
-            if pieces["dirty"]:
-                rendered += ".dev0"
-            rendered += plus_or_dot(pieces)
-            rendered += "g%%s" %% pieces["short"]
-    else:
-        # exception #1
-        rendered = "0.post%%d" %% pieces["distance"]
-        if pieces["dirty"]:
-            rendered += ".dev0"
-        rendered += "+g%%s" %% pieces["short"]
-    return rendered
-
-
-def render_pep440_post_branch(pieces):
-    """TAG[.postDISTANCE[.dev0]+gHEX[.dirty]] .
-
-    The ".dev0" means not master branch.
-
-    Exceptions:
-    1: no tags. 0.postDISTANCE[.dev0]+gHEX[.dirty]
-    """
-    if pieces["closest-tag"]:
-        rendered = pieces["closest-tag"]
-        if pieces["distance"] or pieces["dirty"]:
-            rendered += ".post%%d" %% pieces["distance"]
-            if pieces["branch"] != "master":
-                rendered += ".dev0"
-            rendered += plus_or_dot(pieces)
-            rendered += "g%%s" %% pieces["short"]
-            if pieces["dirty"]:
-                rendered += ".dirty"
-    else:
-        # exception #1
-        rendered = "0.post%%d" %% pieces["distance"]
-        if pieces["branch"] != "master":
-            rendered += ".dev0"
-        rendered += "+g%%s" %% pieces["short"]
-        if pieces["dirty"]:
-            rendered += ".dirty"
-    return rendered
-
-
-def render_pep440_old(pieces):
-    """TAG[.postDISTANCE[.dev0]] .
-
-    The ".dev0" means dirty.
-
-    Exceptions:
-    1: no tags. 0.postDISTANCE[.dev0]
-    """
-    if pieces["closest-tag"]:
-        rendered = pieces["closest-tag"]
-        if pieces["distance"] or pieces["dirty"]:
-            rendered += ".post%%d" %% pieces["distance"]
-            if pieces["dirty"]:
-                rendered += ".dev0"
-    else:
-        # exception #1
-        rendered = "0.post%%d" %% pieces["distance"]
-        if pieces["dirty"]:
-            rendered += ".dev0"
-    return rendered
-
-
-def render_git_describe(pieces):
-    """TAG[-DISTANCE-gHEX][-dirty].
-
-    Like 'git describe --tags --dirty --always'.
-
-    Exceptions:
-    1: no tags. HEX[-dirty]  (note: no 'g' prefix)
-    """
-    if pieces["closest-tag"]:
-        rendered = pieces["closest-tag"]
-        if pieces["distance"]:
-            rendered += "-%%d-g%%s" %% (pieces["distance"], pieces["short"])
-    else:
-        # exception #1
-        rendered = pieces["short"]
-    if pieces["dirty"]:
-        rendered += "-dirty"
-    return rendered
-
-
-def render_git_describe_long(pieces):
-    """TAG-DISTANCE-gHEX[-dirty].
-
-    Like 'git describe --tags --dirty --always -long'.
-    The distance/hash is unconditional.
-
-    Exceptions:
-    1: no tags. HEX[-dirty]  (note: no 'g' prefix)
-    """
-    if pieces["closest-tag"]:
-        rendered = pieces["closest-tag"]
-        rendered += "-%%d-g%%s" %% (pieces["distance"], pieces["short"])
-    else:
-        # exception #1
-        rendered = pieces["short"]
-    if pieces["dirty"]:
-        rendered += "-dirty"
-    return rendered
-
-
-def render(pieces, style):
-    """Render the given version pieces into the requested style."""
-    if pieces["error"]:
-        return {"version": "unknown",
-                "full-revisionid": pieces.get("long"),
-                "dirty": None,
-                "error": pieces["error"],
-                "date": None}
-
-    if not style or style == "default":
-        style = "pep440"  # the default
-
-    if style == "pep440":
-        rendered = render_pep440(pieces)
-    elif style == "pep440-branch":
-        rendered = render_pep440_branch(pieces)
-    elif style == "pep440-pre":
-        rendered = render_pep440_pre(pieces)
-    elif style == "pep440-post":
-        rendered = render_pep440_post(pieces)
-    elif style == "pep440-post-branch":
-        rendered = render_pep440_post_branch(pieces)
-    elif style == "pep440-old":
-        rendered = render_pep440_old(pieces)
-    elif style == "git-describe":
-        rendered = render_git_describe(pieces)
-    elif style == "git-describe-long":
-        rendered = render_git_describe_long(pieces)
-    else:
-        raise ValueError("unknown style '%%s'" %% style)
-
-    return {"version": rendered, "full-revisionid": pieces["long"],
-            "dirty": pieces["dirty"], "error": None,
-            "date": pieces.get("date")}
-
-
-def get_versions():
-    """Get version information or return default if unable to do so."""
-    # I am in _version.py, which lives at ROOT/VERSIONFILE_SOURCE. If we have
-    # __file__, we can work backwards from there to the root. Some
-    # py2exe/bbfreeze/non-CPython implementations don't do __file__, in which
-    # case we can only use expanded keywords.
-
-    cfg = get_config()
-    verbose = cfg.verbose
-
-    try:
-        return git_versions_from_keywords(get_keywords(), cfg.tag_prefix,
-                                          verbose)
-    except NotThisMethod:
-        pass
-
-    try:
-        root = os.path.realpath(__file__)
-        # versionfile_source is the relative path from the top of the source
-        # tree (where the .git directory might live) to this file. Invert
-        # this to find the root from __file__.
-        for _ in cfg.versionfile_source.split('/'):
-            root = os.path.dirname(root)
-    except NameError:
-        return {"version": "0+unknown", "full-revisionid": None,
-                "dirty": None,
-                "error": "unable to find root of source tree",
-                "date": None}
-
-    try:
-        pieces = git_pieces_from_vcs(cfg.tag_prefix, root, verbose)
-        return render(pieces, cfg.style)
-    except NotThisMethod:
-        pass
-
-    try:
-        if cfg.parentdir_prefix:
-            return versions_from_parentdir(cfg.parentdir_prefix, root, verbose)
-    except NotThisMethod:
-        pass
-
-    return {"version": "0+unknown", "full-revisionid": None,
-            "dirty": None,
-            "error": "unable to compute version", "date": None}
-'''
-
-
-@register_vcs_handler("git", "get_keywords")
-def git_get_keywords(versionfile_abs):
-    """Extract version information from the given file."""
-    # the code embedded in _version.py can just fetch the value of these
-    # keywords. When used from setup.py, we don't want to import _version.py,
-    # so we do it with a regexp instead. This function is not used from
-    # _version.py.
-    keywords = {}
-    try:
-        with open(versionfile_abs, "r") as fobj:
-            for line in fobj:
-                if line.strip().startswith("git_refnames ="):
-                    mo = re.search(r'=\s*"(.*)"', line)
-                    if mo:
-                        keywords["refnames"] = mo.group(1)
-                if line.strip().startswith("git_full ="):
-                    mo = re.search(r'=\s*"(.*)"', line)
-                    if mo:
-                        keywords["full"] = mo.group(1)
-                if line.strip().startswith("git_date ="):
-                    mo = re.search(r'=\s*"(.*)"', line)
-                    if mo:
-                        keywords["date"] = mo.group(1)
-    except OSError:
-        pass
-    return keywords
-
-
-@register_vcs_handler("git", "keywords")
-def git_versions_from_keywords(keywords, tag_prefix, verbose):
-    """Get version information from git keywords."""
-    if "refnames" not in keywords:
-        raise NotThisMethod("Short version file found")
-    date = keywords.get("date")
-    if date is not None:
-        # Use only the last line.  Previous lines may contain GPG signature
-        # information.
-        date = date.splitlines()[-1]
-
-        # git-2.2.0 added "%cI", which expands to an ISO-8601 -compliant
-        # datestamp. However we prefer "%ci" (which expands to an "ISO-8601
-        # -like" string, which we must then edit to make compliant), because
-        # it's been around since git-1.5.3, and it's too difficult to
-        # discover which version we're using, or to work around using an
-        # older one.
-        date = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
-    refnames = keywords["refnames"].strip()
-    if refnames.startswith("$Format"):
-        if verbose:
-            print("keywords are unexpanded, not using")
-        raise NotThisMethod("unexpanded keywords, not a git-archive tarball")
-    refs = {r.strip() for r in refnames.strip("()").split(",")}
-    # starting in git-1.8.3, tags are listed as "tag: foo-1.0" instead of
-    # just "foo-1.0". If we see a "tag: " prefix, prefer those.
-    TAG = "tag: "
-    tags = {r[len(TAG) :] for r in refs if r.startswith(TAG)}
-    if not tags:
-        # Either we're using git < 1.8.3, or there really are no tags. We use
-        # a heuristic: assume all version tags have a digit. The old git %d
-        # expansion behaves like git log --decorate=short and strips out the
-        # refs/heads/ and refs/tags/ prefixes that would let us distinguish
-        # between branches and tags. By ignoring refnames without digits, we
-        # filter out many common branch names like "release" and
-        # "stabilization", as well as "HEAD" and "master".
-        tags = {r for r in refs if re.search(r"\d", r)}
-        if verbose:
-            print("discarding '%s', no digits" % ",".join(refs - tags))
-    if verbose:
-        print("likely tags: %s" % ",".join(sorted(tags)))
-    for ref in sorted(tags):
-        # sorting will prefer e.g. "2.0" over "2.0rc1"
-        if ref.startswith(tag_prefix):
-            r = ref[len(tag_prefix) :]
-            # Filter out refs that exactly match prefix or that don't start
-            # with a number once the prefix is stripped (mostly a concern
-            # when prefix is '')
-            if not re.match(r"\d", r):
-                continue
-            if verbose:
-                print("picking %s" % r)
-            return {
-                "version": r,
-                "full-revisionid": keywords["full"].strip(),
-                "dirty": False,
-                "error": None,
-                "date": date,
-            }
-    # no suitable tags, so version is "0+unknown", but full hex is still there
-    if verbose:
-        print("no suitable tags, using unknown + full revision id")
-    return {
-        "version": "0+unknown",
-        "full-revisionid": keywords["full"].strip(),
-        "dirty": False,
-        "error": "no suitable tags",
-        "date": None,
-    }
-
-
-@register_vcs_handler("git", "pieces_from_vcs")
-def git_pieces_from_vcs(tag_prefix, root, verbose, runner=run_command):
-    """Get version from 'git describe' in the root of the source tree.
-
-    This only gets called if the git-archive 'subst' keywords were *not*
-    expanded, and _version.py hasn't already been rewritten with a short
-    version string, meaning we're inside a checked out source tree.
-    """
-    GITS = ["git"]
-    if sys.platform == "win32":
-        GITS = ["git.cmd", "git.exe"]
-
-    # GIT_DIR can interfere with correct operation of Versioneer.
-    # It may be intended to be passed to the Versioneer-versioned project,
-    # but that should not change where we get our version from.
-    env = os.environ.copy()
-    env.pop("GIT_DIR", None)
-    runner = functools.partial(runner, env=env)
-
-    _, rc = runner(GITS, ["rev-parse", "--git-dir"], cwd=root, hide_stderr=True)
-    if rc != 0:
-        if verbose:
-            print("Directory %s not under git control" % root)
-        raise NotThisMethod("'git rev-parse --git-dir' returned error")
-
-    MATCH_ARGS = ["--match", "%s*" % tag_prefix] if tag_prefix else []
-
-    # if there is a tag matching tag_prefix, this yields TAG-NUM-gHEX[-dirty]
-    # if there isn't one, this yields HEX[-dirty] (no NUM)
-    describe_out, rc = runner(
-        GITS,
-        ["describe", "--tags", "--dirty", "--always", "--long", *MATCH_ARGS],
-        cwd=root,
-    )
-    # --long was added in git-1.5.5
-    if describe_out is None:
-        raise NotThisMethod("'git describe' failed")
-    describe_out = describe_out.strip()
-    full_out, rc = runner(GITS, ["rev-parse", "HEAD"], cwd=root)
-    if full_out is None:
-        raise NotThisMethod("'git rev-parse' failed")
-    full_out = full_out.strip()
-
-    pieces = {}
-    pieces["long"] = full_out
-    pieces["short"] = full_out[:7]  # maybe improved later
-    pieces["error"] = None
-
-    branch_name, rc = runner(GITS, ["rev-parse", "--abbrev-ref", "HEAD"], cwd=root)
-    # --abbrev-ref was added in git-1.6.3
-    if rc != 0 or branch_name is None:
-        raise NotThisMethod("'git rev-parse --abbrev-ref' returned error")
-    branch_name = branch_name.strip()
-
-    if branch_name == "HEAD":
-        # If we aren't exactly on a branch, pick a branch which represents
-        # the current commit. If all else fails, we are on a branchless
-        # commit.
-        branches, rc = runner(GITS, ["branch", "--contains"], cwd=root)
-        # --contains was added in git-1.5.4
-        if rc != 0 or branches is None:
-            raise NotThisMethod("'git branch --contains' returned error")
-        branches = branches.split("\n")
-
-        # Remove the first line if we're running detached
-        if "(" in branches[0]:
-            branches.pop(0)
-
-        # Strip off the leading "* " from the list of branches.
-        branches = [branch[2:] for branch in branches]
-        if "master" in branches:
-            branch_name = "master"
-        elif not branches:
-            branch_name = None
-        else:
-            # Pick the first branch that is returned. Good or bad.
-            branch_name = branches[0]
-
-    pieces["branch"] = branch_name
-
-    # parse describe_out. It will be like TAG-NUM-gHEX[-dirty] or HEX[-dirty]
-    # TAG might have hyphens.
-    git_describe = describe_out
-
-    # look for -dirty suffix
-    dirty = git_describe.endswith("-dirty")
-    pieces["dirty"] = dirty
-    if dirty:
-        git_describe = git_describe[: git_describe.rindex("-dirty")]
-
-    # now we have TAG-NUM-gHEX or HEX
-
-    if "-" in git_describe:
-        # TAG-NUM-gHEX
-        mo = re.search(r"^(.+)-(\d+)-g([0-9a-f]+)$", git_describe)
-        if not mo:
-            # unparsable. Maybe git-describe is misbehaving?
-            pieces["error"] = "unable to parse git-describe output: '%s'" % describe_out
-            return pieces
-
-        # tag
-        full_tag = mo.group(1)
-        if not full_tag.startswith(tag_prefix):
-            if verbose:
-                fmt = "tag '%s' doesn't start with prefix '%s'"
-                print(fmt % (full_tag, tag_prefix))
-            pieces["error"] = "tag '%s' doesn't start with prefix '%s'" % (
-                full_tag,
-                tag_prefix,
-            )
-            return pieces
-        pieces["closest-tag"] = full_tag[len(tag_prefix) :]
-
-        # distance: number of commits since tag
-        pieces["distance"] = int(mo.group(2))
-
-        # commit: short hex revision ID
-        pieces["short"] = mo.group(3)
-
-    else:
-        # HEX: no tags
-        pieces["closest-tag"] = None
-        count_out, rc = runner(GITS, ["rev-list", "HEAD", "--count"], cwd=root)
-        pieces["distance"] = int(count_out)  # total number of commits
-
-    # commit date: see ISO-8601 comment in git_versions_from_keywords()
-    date = runner(GITS, ["show", "-s", "--format=%ci", "HEAD"], cwd=root)[0].strip()
-    # Use only the last line.  Previous lines may contain GPG signature
-    # information.
-    date = date.splitlines()[-1]
-    pieces["date"] = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
-
-    return pieces
-
-
-def do_vcs_install(manifest_in, versionfile_source, ipy):
-    """Git-specific installation logic for Versioneer.
-
-    For Git, this means creating/changing .gitattributes to mark _version.py
-    for export-subst keyword substitution.
-    """
-    GITS = ["git"]
-    if sys.platform == "win32":
-        GITS = ["git.cmd", "git.exe"]
-    files = [manifest_in, versionfile_source]
-    if ipy:
-        files.append(ipy)
-    try:
-        my_path = __file__
-        if my_path.endswith(".pyc") or my_path.endswith(".pyo"):
-            my_path = os.path.splitext(my_path)[0] + ".py"
-        versioneer_file = os.path.relpath(my_path)
-    except NameError:
-        versioneer_file = "versioneer.py"
-    files.append(versioneer_file)
-    present = False
-    try:
-        with open(".gitattributes", "r") as fobj:
-            for line in fobj:
-                if line.strip().startswith(versionfile_source):
-                    if "export-subst" in line.strip().split()[1:]:
-                        present = True
-                        break
-    except OSError:
-        pass
-    if not present:
-        with open(".gitattributes", "a+") as fobj:
-            fobj.write(f"{versionfile_source} export-subst\n")
-        files.append(".gitattributes")
-    run_command(GITS, ["add", "--"] + files)
-
-
-def versions_from_parentdir(parentdir_prefix, root, verbose):
-    """Try to determine the version from the parent directory name.
-
-    Source tarballs conventionally unpack into a directory that includes both
-    the project name and a version string. We will also support searching up
-    two directory levels for an appropriately named parent directory
-    """
-    rootdirs = []
-
-    for _ in range(3):
-        dirname = os.path.basename(root)
-        if dirname.startswith(parentdir_prefix):
-            return {
-                "version": dirname[len(parentdir_prefix) :],
-                "full-revisionid": None,
-                "dirty": False,
-                "error": None,
-                "date": None,
-            }
-        rootdirs.append(root)
-        root = os.path.dirname(root)  # up a level
-
-    if verbose:
-        print(
-            "Tried directories %s but none started with prefix %s"
-            % (str(rootdirs), parentdir_prefix)
-        )
-    raise NotThisMethod("rootdir doesn't start with parentdir_prefix")
-
-
-SHORT_VERSION_PY = """
-# This file was generated by 'versioneer.py' (0.22) from
-# revision-control system data, or from the parent directory name of an
-# unpacked source archive. Distribution tarballs contain a pre-generated copy
-# of this file.
-
-import json
-
-version_json = '''
-%s
-'''  # END VERSION_JSON
-
-
-def get_versions():
-    return json.loads(version_json)
-"""
-
-
-def versions_from_file(filename):
-    """Try to determine the version from _version.py if present."""
-    try:
-        with open(filename) as f:
-            contents = f.read()
-    except OSError:
-        raise NotThisMethod("unable to read _version.py")
-    mo = re.search(
-        r"version_json = '''\n(.*)'''  # END VERSION_JSON", contents, re.M | re.S
-    )
-    if not mo:
-        mo = re.search(
-            r"version_json = '''\r\n(.*)'''  # END VERSION_JSON", contents, re.M | re.S
-        )
-    if not mo:
-        raise NotThisMethod("no version_json in _version.py")
-    return json.loads(mo.group(1))
-
-
-def write_to_version_file(filename, versions):
-    """Write the given version number to the given _version.py file."""
-    os.unlink(filename)
-    contents = json.dumps(versions, sort_keys=True, indent=1, separators=(",", ": "))
-    with open(filename, "w") as f:
-        f.write(SHORT_VERSION_PY % contents)
-
-    print("set %s to '%s'" % (filename, versions["version"]))
-
-
-def plus_or_dot(pieces):
-    """Return a + if we don't already have one, else return a ."""
-    if "+" in pieces.get("closest-tag", ""):
-        return "."
-    return "+"
-
-
-def render_pep440(pieces):
-    """Build up version string, with post-release "local version identifier".
-
-    Our goal: TAG[+DISTANCE.gHEX[.dirty]] . Note that if you
-    get a tagged build and then dirty it, you'll get TAG+0.gHEX.dirty
-
-    Exceptions:
-    1: no tags. git_describe was just HEX. 0+untagged.DISTANCE.gHEX[.dirty]
-    """
-    if pieces["closest-tag"]:
-        rendered = pieces["closest-tag"]
-        if pieces["distance"] or pieces["dirty"]:
-            rendered += plus_or_dot(pieces)
-            rendered += "%d.g%s" % (pieces["distance"], pieces["short"])
-            if pieces["dirty"]:
-                rendered += ".dirty"
-    else:
-        # exception #1
-        rendered = "0+untagged.%d.g%s" % (pieces["distance"], pieces["short"])
-        if pieces["dirty"]:
-            rendered += ".dirty"
-    return rendered
-
-
-def render_pep440_branch(pieces):
-    """TAG[[.dev0]+DISTANCE.gHEX[.dirty]] .
-
-    The ".dev0" means not master branch. Note that .dev0 sorts backwards
-    (a feature branch will appear "older" than the master branch).
-
-    Exceptions:
-    1: no tags. 0[.dev0]+untagged.DISTANCE.gHEX[.dirty]
-    """
-    if pieces["closest-tag"]:
-        rendered = pieces["closest-tag"]
-        if pieces["distance"] or pieces["dirty"]:
-            if pieces["branch"] != "master":
-                rendered += ".dev0"
-            rendered += plus_or_dot(pieces)
-            rendered += "%d.g%s" % (pieces["distance"], pieces["short"])
-            if pieces["dirty"]:
-                rendered += ".dirty"
-    else:
-        # exception #1
-        rendered = "0"
-        if pieces["branch"] != "master":
-            rendered += ".dev0"
-        rendered += "+untagged.%d.g%s" % (pieces["distance"], pieces["short"])
-        if pieces["dirty"]:
-            rendered += ".dirty"
-    return rendered
-
-
-def pep440_split_post(ver):
-    """Split pep440 version string at the post-release segment.
-
-    Returns the release segments before the post-release and the
-    post-release version number (or -1 if no post-release segment is present).
-    """
-    vc = str.split(ver, ".post")
-    return vc[0], int(vc[1] or 0) if len(vc) == 2 else None
-
-
-def render_pep440_pre(pieces):
-    """TAG[.postN.devDISTANCE] -- No -dirty.
-
-    Exceptions:
-    1: no tags. 0.post0.devDISTANCE
-    """
-    if pieces["closest-tag"]:
-        if pieces["distance"]:
-            # update the post release segment
-            tag_version, post_version = pep440_split_post(pieces["closest-tag"])
-            rendered = tag_version
-            if post_version is not None:
-                rendered += ".post%d.dev%d" % (post_version + 1, pieces["distance"])
-            else:
-                rendered += ".post0.dev%d" % (pieces["distance"])
-        else:
-            # no commits, use the tag as the version
-            rendered = pieces["closest-tag"]
-    else:
-        # exception #1
-        rendered = "0.post0.dev%d" % pieces["distance"]
-    return rendered
-
-
-def render_pep440_post(pieces):
-    """TAG[.postDISTANCE[.dev0]+gHEX] .
-
-    The ".dev0" means dirty. Note that .dev0 sorts backwards
-    (a dirty tree will appear "older" than the corresponding clean one),
-    but you shouldn't be releasing software with -dirty anyways.
-
-    Exceptions:
-    1: no tags. 0.postDISTANCE[.dev0]
-    """
-    if pieces["closest-tag"]:
-        rendered = pieces["closest-tag"]
-        if pieces["distance"] or pieces["dirty"]:
-            rendered += ".post%d" % pieces["distance"]
-            if pieces["dirty"]:
-                rendered += ".dev0"
-            rendered += plus_or_dot(pieces)
-            rendered += "g%s" % pieces["short"]
-    else:
-        # exception #1
-        rendered = "0.post%d" % pieces["distance"]
-        if pieces["dirty"]:
-            rendered += ".dev0"
-        rendered += "+g%s" % pieces["short"]
-    return rendered
-
-
-def render_pep440_post_branch(pieces):
-    """TAG[.postDISTANCE[.dev0]+gHEX[.dirty]] .
-
-    The ".dev0" means not master branch.
-
-    Exceptions:
-    1: no tags. 0.postDISTANCE[.dev0]+gHEX[.dirty]
-    """
-    if pieces["closest-tag"]:
-        rendered = pieces["closest-tag"]
-        if pieces["distance"] or pieces["dirty"]:
-            rendered += ".post%d" % pieces["distance"]
-            if pieces["branch"] != "master":
-                rendered += ".dev0"
-            rendered += plus_or_dot(pieces)
-            rendered += "g%s" % pieces["short"]
-            if pieces["dirty"]:
-                rendered += ".dirty"
-    else:
-        # exception #1
-        rendered = "0.post%d" % pieces["distance"]
-        if pieces["branch"] != "master":
-            rendered += ".dev0"
-        rendered += "+g%s" % pieces["short"]
-        if pieces["dirty"]:
-            rendered += ".dirty"
-    return rendered
-
-
-def render_pep440_old(pieces):
-    """TAG[.postDISTANCE[.dev0]] .
-
-    The ".dev0" means dirty.
-
-    Exceptions:
-    1: no tags. 0.postDISTANCE[.dev0]
-    """
-    if pieces["closest-tag"]:
-        rendered = pieces["closest-tag"]
-        if pieces["distance"] or pieces["dirty"]:
-            rendered += ".post%d" % pieces["distance"]
-            if pieces["dirty"]:
-                rendered += ".dev0"
-    else:
-        # exception #1
-        rendered = "0.post%d" % pieces["distance"]
-        if pieces["dirty"]:
-            rendered += ".dev0"
-    return rendered
-
-
-def render_git_describe(pieces):
-    """TAG[-DISTANCE-gHEX][-dirty].
-
-    Like 'git describe --tags --dirty --always'.
-
-    Exceptions:
-    1: no tags. HEX[-dirty]  (note: no 'g' prefix)
-    """
-    if pieces["closest-tag"]:
-        rendered = pieces["closest-tag"]
-        if pieces["distance"]:
-            rendered += "-%d-g%s" % (pieces["distance"], pieces["short"])
-    else:
-        # exception #1
-        rendered = pieces["short"]
-    if pieces["dirty"]:
-        rendered += "-dirty"
-    return rendered
-
-
-def render_git_describe_long(pieces):
-    """TAG-DISTANCE-gHEX[-dirty].
-
-    Like 'git describe --tags --dirty --always -long'.
-    The distance/hash is unconditional.
-
-    Exceptions:
-    1: no tags. HEX[-dirty]  (note: no 'g' prefix)
-    """
-    if pieces["closest-tag"]:
-        rendered = pieces["closest-tag"]
-        rendered += "-%d-g%s" % (pieces["distance"], pieces["short"])
-    else:
-        # exception #1
-        rendered = pieces["short"]
-    if pieces["dirty"]:
-        rendered += "-dirty"
-    return rendered
-
-
-def render(pieces, style):
-    """Render the given version pieces into the requested style."""
-    if pieces["error"]:
-        return {
-            "version": "unknown",
-            "full-revisionid": pieces.get("long"),
-            "dirty": None,
-            "error": pieces["error"],
-            "date": None,
-        }
-
-    if not style or style == "default":
-        style = "pep440"  # the default
-
-    if style == "pep440":
-        rendered = render_pep440(pieces)
-    elif style == "pep440-branch":
-        rendered = render_pep440_branch(pieces)
-    elif style == "pep440-pre":
-        rendered = render_pep440_pre(pieces)
-    elif style == "pep440-post":
-        rendered = render_pep440_post(pieces)
-    elif style == "pep440-post-branch":
-        rendered = render_pep440_post_branch(pieces)
-    elif style == "pep440-old":
-        rendered = render_pep440_old(pieces)
-    elif style == "git-describe":
-        rendered = render_git_describe(pieces)
-    elif style == "git-describe-long":
-        rendered = render_git_describe_long(pieces)
-    else:
-        raise ValueError("unknown style '%s'" % style)
-
-    return {
-        "version": rendered,
-        "full-revisionid": pieces["long"],
-        "dirty": pieces["dirty"],
-        "error": None,
-        "date": pieces.get("date"),
-    }
-
-
-class VersioneerBadRootError(Exception):
-    """The project root directory is unknown or missing key files."""
-
-
-def get_versions(verbose=False):
-    """Get the project version from whatever source is available.
-
-    Returns dict with two keys: 'version' and 'full'.
-    """
-    if "versioneer" in sys.modules:
-        # see the discussion in cmdclass.py:get_cmdclass()
-        del sys.modules["versioneer"]
-
-    root = get_root()
-    cfg = get_config_from_root(root)
-
-    assert cfg.VCS is not None, "please set [versioneer]VCS= in setup.cfg"
-    handlers = HANDLERS.get(cfg.VCS)
-    assert handlers, "unrecognized VCS '%s'" % cfg.VCS
-    verbose = verbose or cfg.verbose
-    assert (
-        cfg.versionfile_source is not None
-    ), "please set versioneer.versionfile_source"
-    assert cfg.tag_prefix is not None, "please set versioneer.tag_prefix"
-
-    versionfile_abs = os.path.join(root, cfg.versionfile_source)
-
-    # extract version from first of: _version.py, VCS command (e.g. 'git
-    # describe'), parentdir. This is meant to work for developers using a
-    # source checkout, for users of a tarball created by 'setup.py sdist',
-    # and for users of a tarball/zipball created by 'git archive' or github's
-    # download-from-tag feature or the equivalent in other VCSes.
-
-    get_keywords_f = handlers.get("get_keywords")
-    from_keywords_f = handlers.get("keywords")
-    if get_keywords_f and from_keywords_f:
-        try:
-            keywords = get_keywords_f(versionfile_abs)
-            ver = from_keywords_f(keywords, cfg.tag_prefix, verbose)
-            if verbose:
-                print("got version from expanded keyword %s" % ver)
-            return ver
-        except NotThisMethod:
-            pass
-
-    try:
-        ver = versions_from_file(versionfile_abs)
-        if verbose:
-            print("got version from file %s %s" % (versionfile_abs, ver))
-        return ver
-    except NotThisMethod:
-        pass
-
-    from_vcs_f = handlers.get("pieces_from_vcs")
-    if from_vcs_f:
-        try:
-            pieces = from_vcs_f(cfg.tag_prefix, root, verbose)
-            ver = render(pieces, cfg.style)
-            if verbose:
-                print("got version from VCS %s" % ver)
-            return ver
-        except NotThisMethod:
-            pass
-
-    try:
-        if cfg.parentdir_prefix:
-            ver = versions_from_parentdir(cfg.parentdir_prefix, root, verbose)
-            if verbose:
-                print("got version from parentdir %s" % ver)
-            return ver
-    except NotThisMethod:
-        pass
-
-    if verbose:
-        print("unable to compute version")
-
-    return {
-        "version": "0+unknown",
-        "full-revisionid": None,
-        "dirty": None,
-        "error": "unable to compute version",
-        "date": None,
-    }
-
-
-def get_version():
-    """Get the short version string for this project."""
-    return get_versions()["version"]
-
-
-def get_cmdclass(cmdclass=None):
-    """Get the custom setuptools/distutils subclasses used by Versioneer.
-
-    If the package uses a different cmdclass (e.g. one from numpy), it
-    should be provide as an argument.
-    """
-    if "versioneer" in sys.modules:
-        del sys.modules["versioneer"]
-        # this fixes the "python setup.py develop" case (also 'install' and
-        # 'easy_install .'), in which subdependencies of the main project are
-        # built (using setup.py bdist_egg) in the same python process. Assume
-        # a main project A and a dependency B, which use different versions
-        # of Versioneer. A's setup.py imports A's Versioneer, leaving it in
-        # sys.modules by the time B's setup.py is executed, causing B to run
-        # with the wrong versioneer. Setuptools wraps the sub-dep builds in a
-        # sandbox that restores sys.modules to it's pre-build state, so the
-        # parent is protected against the child's "import versioneer". By
-        # removing ourselves from sys.modules here, before the child build
-        # happens, we protect the child from the parent's versioneer too.
-        # Also see https://github.com/python-versioneer/python-versioneer/issues/52
-
-    cmds = {} if cmdclass is None else cmdclass.copy()
-
-    # we add "version" to both distutils and setuptools
-    try:
-        from setuptools import Command
-    except ImportError:
-        from distutils.core import Command
-
-    class cmd_version(Command):
-        description = "report generated version string"
-        user_options = []
-        boolean_options = []
-
-        def initialize_options(self):
-            pass
-
-        def finalize_options(self):
-            pass
-
-        def run(self):
-            vers = get_versions(verbose=True)
-            print("Version: %s" % vers["version"])
-            print(" full-revisionid: %s" % vers.get("full-revisionid"))
-            print(" dirty: %s" % vers.get("dirty"))
-            print(" date: %s" % vers.get("date"))
-            if vers["error"]:
-                print(" error: %s" % vers["error"])
-
-    cmds["version"] = cmd_version
-
-    # we override "build_py" in both distutils and setuptools
-    #
-    # most invocation pathways end up running build_py:
-    #  distutils/build -> build_py
-    #  distutils/install -> distutils/build ->..
-    #  setuptools/bdist_wheel -> distutils/install ->..
-    #  setuptools/bdist_egg -> distutils/install_lib -> build_py
-    #  setuptools/install -> bdist_egg ->..
-    #  setuptools/develop -> ?
-    #  pip install:
-    #   copies source tree to a tempdir before running egg_info/etc
-    #   if .git isn't copied too, 'git describe' will fail
-    #   then does setup.py bdist_wheel, or sometimes setup.py install
-    #  setup.py egg_info -> ?
-
-    # we override different "build_py" commands for both environments
-    if "build_py" in cmds:
-        _build_py = cmds["build_py"]
-    elif "setuptools" in sys.modules:
-        from setuptools.command.build_py import build_py as _build_py
-    else:
-        from distutils.command.build_py import build_py as _build_py
-
-    class cmd_build_py(_build_py):
-        def run(self):
-            root = get_root()
-            cfg = get_config_from_root(root)
-            versions = get_versions()
-            _build_py.run(self)
-            # now locate _version.py in the new build/ directory and replace
-            # it with an updated value
-            if cfg.versionfile_build:
-                target_versionfile = os.path.join(self.build_lib, cfg.versionfile_build)
-                print("UPDATING %s" % target_versionfile)
-                write_to_version_file(target_versionfile, versions)
-
-    cmds["build_py"] = cmd_build_py
-
-    if "build_ext" in cmds:
-        _build_ext = cmds["build_ext"]
-    elif "setuptools" in sys.modules:
-        from setuptools.command.build_ext import build_ext as _build_ext
-    else:
-        from distutils.command.build_ext import build_ext as _build_ext
-
-    class cmd_build_ext(_build_ext):
-        def run(self):
-            root = get_root()
-            cfg = get_config_from_root(root)
-            versions = get_versions()
-            _build_ext.run(self)
-            if self.inplace:
-                # build_ext --inplace will only build extensions in
-                # build/lib<..> dir with no _version.py to write to.
-                # As in place builds will already have a _version.py
-                # in the module dir, we do not need to write one.
-                return
-            # now locate _version.py in the new build/ directory and replace
-            # it with an updated value
-            target_versionfile = os.path.join(self.build_lib, cfg.versionfile_build)
-            print("UPDATING %s" % target_versionfile)
-            write_to_version_file(target_versionfile, versions)
-
-    cmds["build_ext"] = cmd_build_ext
-
-    if "cx_Freeze" in sys.modules:  # cx_freeze enabled?
-        from cx_Freeze.dist import build_exe as _build_exe
-
-        # nczeczulin reports that py2exe won't like the pep440-style string
-        # as FILEVERSION, but it can be used for PRODUCTVERSION, e.g.
-        # setup(console=[{
-        #   "version": versioneer.get_version().split("+", 1)[0], # FILEVERSION
-        #   "product_version": versioneer.get_version(),
-        #   ...
-
-        class cmd_build_exe(_build_exe):
-            def run(self):
-                root = get_root()
-                cfg = get_config_from_root(root)
-                versions = get_versions()
-                target_versionfile = cfg.versionfile_source
-                print("UPDATING %s" % target_versionfile)
-                write_to_version_file(target_versionfile, versions)
-
-                _build_exe.run(self)
-                os.unlink(target_versionfile)
-                with open(cfg.versionfile_source, "w") as f:
-                    LONG = LONG_VERSION_PY[cfg.VCS]
-                    f.write(
-                        LONG
-                        % {
-                            "DOLLAR": "$",
-                            "STYLE": cfg.style,
-                            "TAG_PREFIX": cfg.tag_prefix,
-                            "PARENTDIR_PREFIX": cfg.parentdir_prefix,
-                            "VERSIONFILE_SOURCE": cfg.versionfile_source,
-                        }
-                    )
-
-        cmds["build_exe"] = cmd_build_exe
-        del cmds["build_py"]
-
-    if "py2exe" in sys.modules:  # py2exe enabled?
-        from py2exe.distutils_buildexe import py2exe as _py2exe
-
-        class cmd_py2exe(_py2exe):
-            def run(self):
-                root = get_root()
-                cfg = get_config_from_root(root)
-                versions = get_versions()
-                target_versionfile = cfg.versionfile_source
-                print("UPDATING %s" % target_versionfile)
-                write_to_version_file(target_versionfile, versions)
-
-                _py2exe.run(self)
-                os.unlink(target_versionfile)
-                with open(cfg.versionfile_source, "w") as f:
-                    LONG = LONG_VERSION_PY[cfg.VCS]
-                    f.write(
-                        LONG
-                        % {
-                            "DOLLAR": "$",
-                            "STYLE": cfg.style,
-                            "TAG_PREFIX": cfg.tag_prefix,
-                            "PARENTDIR_PREFIX": cfg.parentdir_prefix,
-                            "VERSIONFILE_SOURCE": cfg.versionfile_source,
-                        }
-                    )
-
-        cmds["py2exe"] = cmd_py2exe
-
-    # we override different "sdist" commands for both environments
-    if "sdist" in cmds:
-        _sdist = cmds["sdist"]
-    elif "setuptools" in sys.modules:
-        from setuptools.command.sdist import sdist as _sdist
-    else:
-        from distutils.command.sdist import sdist as _sdist
-
-    class cmd_sdist(_sdist):
-        def run(self):
-            versions = get_versions()
-            self._versioneer_generated_versions = versions
-            # unless we update this, the command will keep using the old
-            # version
-            self.distribution.metadata.version = versions["version"]
-            return _sdist.run(self)
-
-        def make_release_tree(self, base_dir, files):
-            root = get_root()
-            cfg = get_config_from_root(root)
-            _sdist.make_release_tree(self, base_dir, files)
-            # now locate _version.py in the new base_dir directory
-            # (remembering that it may be a hardlink) and replace it with an
-            # updated value
-            target_versionfile = os.path.join(base_dir, cfg.versionfile_source)
-            print("UPDATING %s" % target_versionfile)
-            write_to_version_file(
-                target_versionfile, self._versioneer_generated_versions
-            )
-
-    cmds["sdist"] = cmd_sdist
-
-    return cmds
-
-
-CONFIG_ERROR = """
-setup.cfg is missing the necessary Versioneer configuration. You need
-a section like:
-
- [versioneer]
- VCS = git
- style = pep440
- versionfile_source = src/myproject/_version.py
- versionfile_build = myproject/_version.py
- tag_prefix =
- parentdir_prefix = myproject-
-
-You will also need to edit your setup.py to use the results:
-
- import versioneer
- setup(version=versioneer.get_version(),
-       cmdclass=versioneer.get_cmdclass(), ...)
-
-Please read the docstring in ./versioneer.py for configuration instructions,
-edit setup.cfg, and re-run the installer or 'python versioneer.py setup'.
-"""
-
-SAMPLE_CONFIG = """
-# See the docstring in versioneer.py for instructions. Note that you must
-# re-run 'versioneer.py setup' after changing this section, and commit the
-# resulting files.
-
-[versioneer]
-#VCS = git
-#style = pep440
-#versionfile_source =
-#versionfile_build =
-#tag_prefix =
-#parentdir_prefix =
-
-"""
-
-OLD_SNIPPET = """
-from ._version import get_versions
-__version__ = get_versions()['version']
-del get_versions
-"""
-
-INIT_PY_SNIPPET = """
-from . import {0}
-__version__ = {0}.get_versions()['version']
-"""
-
-
-def do_setup():
-    """Do main VCS-independent setup function for installing Versioneer."""
-    root = get_root()
-    try:
-        cfg = get_config_from_root(root)
-    except (OSError, configparser.NoSectionError, configparser.NoOptionError) as e:
-        if isinstance(e, (OSError, configparser.NoSectionError)):
-            print("Adding sample versioneer config to setup.cfg", file=sys.stderr)
-            with open(os.path.join(root, "setup.cfg"), "a") as f:
-                f.write(SAMPLE_CONFIG)
-        print(CONFIG_ERROR, file=sys.stderr)
-        return 1
-
-    print(" creating %s" % cfg.versionfile_source)
-    with open(cfg.versionfile_source, "w") as f:
-        LONG = LONG_VERSION_PY[cfg.VCS]
-        f.write(
-            LONG
-            % {
-                "DOLLAR": "$",
-                "STYLE": cfg.style,
-                "TAG_PREFIX": cfg.tag_prefix,
-                "PARENTDIR_PREFIX": cfg.parentdir_prefix,
-                "VERSIONFILE_SOURCE": cfg.versionfile_source,
-            }
-        )
-
-    ipy = os.path.join(os.path.dirname(cfg.versionfile_source), "__init__.py")
-    if os.path.exists(ipy):
-        try:
-            with open(ipy, "r") as f:
-                old = f.read()
-        except OSError:
-            old = ""
-        module = os.path.splitext(os.path.basename(cfg.versionfile_source))[0]
-        snippet = INIT_PY_SNIPPET.format(module)
-        if OLD_SNIPPET in old:
-            print(" replacing boilerplate in %s" % ipy)
-            with open(ipy, "w") as f:
-                f.write(old.replace(OLD_SNIPPET, snippet))
-        elif snippet not in old:
-            print(" appending to %s" % ipy)
-            with open(ipy, "a") as f:
-                f.write(snippet)
-        else:
-            print(" %s unmodified" % ipy)
-    else:
-        print(" %s doesn't exist, ok" % ipy)
-        ipy = None
-
-    # Make sure both the top-level "versioneer.py" and versionfile_source
-    # (PKG/_version.py, used by runtime code) are in MANIFEST.in, so
-    # they'll be copied into source distributions. Pip won't be able to
-    # install the package without this.
-    manifest_in = os.path.join(root, "MANIFEST.in")
-    simple_includes = set()
-    try:
-        with open(manifest_in, "r") as f:
-            for line in f:
-                if line.startswith("include "):
-                    for include in line.split()[1:]:
-                        simple_includes.add(include)
-    except OSError:
-        pass
-    # That doesn't cover everything MANIFEST.in can do
-    # (http://docs.python.org/2/distutils/sourcedist.html#commands), so
-    # it might give some false negatives. Appending redundant 'include'
-    # lines is safe, though.
-    if "versioneer.py" not in simple_includes:
-        print(" appending 'versioneer.py' to MANIFEST.in")
-        with open(manifest_in, "a") as f:
-            f.write("include versioneer.py\n")
-    else:
-        print(" 'versioneer.py' already in MANIFEST.in")
-    if cfg.versionfile_source not in simple_includes:
-        print(
-            " appending versionfile_source ('%s') to MANIFEST.in"
-            % cfg.versionfile_source
-        )
-        with open(manifest_in, "a") as f:
-            f.write("include %s\n" % cfg.versionfile_source)
-    else:
-        print(" versionfile_source already in MANIFEST.in")
-
-    # Make VCS-specific changes. For git, this means creating/changing
-    # .gitattributes to mark _version.py for export-subst keyword
-    # substitution.
-    do_vcs_install(manifest_in, cfg.versionfile_source, ipy)
-    return 0
-
-
-def scan_setup_py():
-    """Validate the contents of setup.py against Versioneer's expectations."""
-    found = set()
-    setters = False
-    errors = 0
-    with open("setup.py", "r") as f:
-        for line in f.readlines():
-            if "import versioneer" in line:
-                found.add("import")
-            if "versioneer.get_cmdclass()" in line:
-                found.add("cmdclass")
-            if "versioneer.get_version()" in line:
-                found.add("get_version")
-            if "versioneer.VCS" in line:
-                setters = True
-            if "versioneer.versionfile_source" in line:
-                setters = True
-    if len(found) != 3:
-        print("")
-        print("Your setup.py appears to be missing some important items")
-        print("(but I might be wrong). Please make sure it has something")
-        print("roughly like the following:")
-        print("")
-        print(" import versioneer")
-        print(" setup( version=versioneer.get_version(),")
-        print("        cmdclass=versioneer.get_cmdclass(),  ...)")
-        print("")
-        errors += 1
-    if setters:
-        print("You should remove lines like 'versioneer.VCS = ' and")
-        print("'versioneer.versionfile_source = ' . This configuration")
-        print("now lives in setup.cfg, and should be removed from setup.py")
-        print("")
-        errors += 1
-    return errors
-
-
-if __name__ == "__main__":
-    cmd = sys.argv[1]
-    if cmd == "setup":
-        errors = do_setup()
-        errors += scan_setup_py()
-        if errors:
-            sys.exit(1)
+# Version: 0.22
+
+"""The Versioneer - like a rocketeer, but for versions.
+
+The Versioneer
+==============
+
+* like a rocketeer, but for versions!
+* https://github.com/python-versioneer/python-versioneer
+* Brian Warner
+* License: Public Domain
+* Compatible with: Python 3.6, 3.7, 3.8, 3.9, 3.10 and pypy3
+* [![Latest Version][pypi-image]][pypi-url]
+* [![Build Status][travis-image]][travis-url]
+
+This is a tool for managing a recorded version number in distutils/setuptools-based
+python projects. The goal is to remove the tedious and error-prone "update
+the embedded version string" step from your release process. Making a new
+release should be as easy as recording a new tag in your version-control
+system, and maybe making new tarballs.
+
+
+## Quick Install
+
+* `pip install versioneer` to somewhere in your $PATH
+* add a `[versioneer]` section to your setup.cfg (see [Install](INSTALL.md))
+* run `versioneer install` in your source tree, commit the results
+* Verify version information with `python setup.py version`
+
+## Version Identifiers
+
+Source trees come from a variety of places:
+
+* a version-control system checkout (mostly used by developers)
+* a nightly tarball, produced by build automation
+* a snapshot tarball, produced by a web-based VCS browser, like github's
+  "tarball from tag" feature
+* a release tarball, produced by "setup.py sdist", distributed through PyPI
+
+Within each source tree, the version identifier (either a string or a number,
+this tool is format-agnostic) can come from a variety of places:
+
+* ask the VCS tool itself, e.g. "git describe" (for checkouts), which knows
+  about recent "tags" and an absolute revision-id
+* the name of the directory into which the tarball was unpacked
+* an expanded VCS keyword ($Id$, etc)
+* a `_version.py` created by some earlier build step
+
+For released software, the version identifier is closely related to a VCS
+tag. Some projects use tag names that include more than just the version
+string (e.g. "myproject-1.2" instead of just "1.2"), in which case the tool
+needs to strip the tag prefix to extract the version identifier. For
+unreleased software (between tags), the version identifier should provide
+enough information to help developers recreate the same tree, while also
+giving them an idea of roughly how old the tree is (after version 1.2, before
+version 1.3). Many VCS systems can report a description that captures this,
+for example `git describe --tags --dirty --always` reports things like
+"0.7-1-g574ab98-dirty" to indicate that the checkout is one revision past the
+0.7 tag, has a unique revision id of "574ab98", and is "dirty" (it has
+uncommitted changes).
+
+The version identifier is used for multiple purposes:
+
+* to allow the module to self-identify its version: `myproject.__version__`
+* to choose a name and prefix for a 'setup.py sdist' tarball
+
+## Theory of Operation
+
+Versioneer works by adding a special `_version.py` file into your source
+tree, where your `__init__.py` can import it. This `_version.py` knows how to
+dynamically ask the VCS tool for version information at import time.
+
+`_version.py` also contains `$Revision$` markers, and the installation
+process marks `_version.py` to have this marker rewritten with a tag name
+during the `git archive` command. As a result, generated tarballs will
+contain enough information to get the proper version.
+
+To allow `setup.py` to compute a version too, a `versioneer.py` is added to
+the top level of your source tree, next to `setup.py` and the `setup.cfg`
+that configures it. This overrides several distutils/setuptools commands to
+compute the version when invoked, and changes `setup.py build` and `setup.py
+sdist` to replace `_version.py` with a small static file that contains just
+the generated version data.
+
+## Installation
+
+See [INSTALL.md](./INSTALL.md) for detailed installation instructions.
+
+## Version-String Flavors
+
+Code which uses Versioneer can learn about its version string at runtime by
+importing `_version` from your main `__init__.py` file and running the
+`get_versions()` function. From the "outside" (e.g. in `setup.py`), you can
+import the top-level `versioneer.py` and run `get_versions()`.
+
+Both functions return a dictionary with different flavors of version
+information:
+
+* `['version']`: A condensed version string, rendered using the selected
+  style. This is the most commonly used value for the project's version
+  string. The default "pep440" style yields strings like `0.11`,
+  `0.11+2.g1076c97`, or `0.11+2.g1076c97.dirty`. See the "Styles" section
+  below for alternative styles.
+
+* `['full-revisionid']`: detailed revision identifier. For Git, this is the
+  full SHA1 commit id, e.g. "1076c978a8d3cfc70f408fe5974aa6c092c949ac".
+
+* `['date']`: Date and time of the latest `HEAD` commit. For Git, it is the
+  commit date in ISO 8601 format. This will be None if the date is not
+  available.
+
+* `['dirty']`: a boolean, True if the tree has uncommitted changes. Note that
+  this is only accurate if run in a VCS checkout, otherwise it is likely to
+  be False or None
+
+* `['error']`: if the version string could not be computed, this will be set
+  to a string describing the problem, otherwise it will be None. It may be
+  useful to throw an exception in setup.py if this is set, to avoid e.g.
+  creating tarballs with a version string of "unknown".
+
+Some variants are more useful than others. Including `full-revisionid` in a
+bug report should allow developers to reconstruct the exact code being tested
+(or indicate the presence of local changes that should be shared with the
+developers). `version` is suitable for display in an "about" box or a CLI
+`--version` output: it can be easily compared against release notes and lists
+of bugs fixed in various releases.
+
+The installer adds the following text to your `__init__.py` to place a basic
+version in `YOURPROJECT.__version__`:
+
+    from ._version import get_versions
+    __version__ = get_versions()['version']
+    del get_versions
+
+## Styles
+
+The setup.cfg `style=` configuration controls how the VCS information is
+rendered into a version string.
+
+The default style, "pep440", produces a PEP440-compliant string, equal to the
+un-prefixed tag name for actual releases, and containing an additional "local
+version" section with more detail for in-between builds. For Git, this is
+TAG[+DISTANCE.gHEX[.dirty]] , using information from `git describe --tags
+--dirty --always`. For example "0.11+2.g1076c97.dirty" indicates that the
+tree is like the "1076c97" commit but has uncommitted changes (".dirty"), and
+that this commit is two revisions ("+2") beyond the "0.11" tag. For released
+software (exactly equal to a known tag), the identifier will only contain the
+stripped tag, e.g. "0.11".
+
+Other styles are available. See [details.md](details.md) in the Versioneer
+source tree for descriptions.
+
+## Debugging
+
+Versioneer tries to avoid fatal errors: if something goes wrong, it will tend
+to return a version of "0+unknown". To investigate the problem, run `setup.py
+version`, which will run the version-lookup code in a verbose mode, and will
+display the full contents of `get_versions()` (including the `error` string,
+which may help identify what went wrong).
+
+## Known Limitations
+
+Some situations are known to cause problems for Versioneer. This details the
+most significant ones. More can be found on Github
+[issues page](https://github.com/python-versioneer/python-versioneer/issues).
+
+### Subprojects
+
+Versioneer has limited support for source trees in which `setup.py` is not in
+the root directory (e.g. `setup.py` and `.git/` are *not* siblings). The are
+two common reasons why `setup.py` might not be in the root:
+
+* Source trees which contain multiple subprojects, such as
+  [Buildbot](https://github.com/buildbot/buildbot), which contains both
+  "master" and "slave" subprojects, each with their own `setup.py`,
+  `setup.cfg`, and `tox.ini`. Projects like these produce multiple PyPI
+  distributions (and upload multiple independently-installable tarballs).
+* Source trees whose main purpose is to contain a C library, but which also
+  provide bindings to Python (and perhaps other languages) in subdirectories.
+
+Versioneer will look for `.git` in parent directories, and most operations
+should get the right version string. However `pip` and `setuptools` have bugs
+and implementation details which frequently cause `pip install .` from a
+subproject directory to fail to find a correct version string (so it usually
+defaults to `0+unknown`).
+
+`pip install --editable .` should work correctly. `setup.py install` might
+work too.
+
+Pip-8.1.1 is known to have this problem, but hopefully it will get fixed in
+some later version.
+
+[Bug #38](https://github.com/python-versioneer/python-versioneer/issues/38) is tracking
+this issue. The discussion in
+[PR #61](https://github.com/python-versioneer/python-versioneer/pull/61) describes the
+issue from the Versioneer side in more detail.
+[pip PR#3176](https://github.com/pypa/pip/pull/3176) and
+[pip PR#3615](https://github.com/pypa/pip/pull/3615) contain work to improve
+pip to let Versioneer work correctly.
+
+Versioneer-0.16 and earlier only looked for a `.git` directory next to the
+`setup.cfg`, so subprojects were completely unsupported with those releases.
+
+### Editable installs with setuptools <= 18.5
+
+`setup.py develop` and `pip install --editable .` allow you to install a
+project into a virtualenv once, then continue editing the source code (and
+test) without re-installing after every change.
+
+"Entry-point scripts" (`setup(entry_points={"console_scripts": ..})`) are a
+convenient way to specify executable scripts that should be installed along
+with the python package.
+
+These both work as expected when using modern setuptools. When using
+setuptools-18.5 or earlier, however, certain operations will cause
+`pkg_resources.DistributionNotFound` errors when running the entrypoint
+script, which must be resolved by re-installing the package. This happens
+when the install happens with one version, then the egg_info data is
+regenerated while a different version is checked out. Many setup.py commands
+cause egg_info to be rebuilt (including `sdist`, `wheel`, and installing into
+a different virtualenv), so this can be surprising.
+
+[Bug #83](https://github.com/python-versioneer/python-versioneer/issues/83) describes
+this one, but upgrading to a newer version of setuptools should probably
+resolve it.
+
+
+## Updating Versioneer
+
+To upgrade your project to a new release of Versioneer, do the following:
+
+* install the new Versioneer (`pip install -U versioneer` or equivalent)
+* edit `setup.cfg`, if necessary, to include any new configuration settings
+  indicated by the release notes. See [UPGRADING](./UPGRADING.md) for details.
+* re-run `versioneer install` in your source tree, to replace
+  `SRC/_version.py`
+* commit any changed files
+
+## Future Directions
+
+This tool is designed to make it easily extended to other version-control
+systems: all VCS-specific components are in separate directories like
+src/git/ . The top-level `versioneer.py` script is assembled from these
+components by running make-versioneer.py . In the future, make-versioneer.py
+will take a VCS name as an argument, and will construct a version of
+`versioneer.py` that is specific to the given VCS. It might also take the
+configuration arguments that are currently provided manually during
+installation by editing setup.py . Alternatively, it might go the other
+direction and include code from all supported VCS systems, reducing the
+number of intermediate scripts.
+
+## Similar projects
+
+* [setuptools_scm](https://github.com/pypa/setuptools_scm/) - a non-vendored build-time
+  dependency
+* [minver](https://github.com/jbweston/miniver) - a lightweight reimplementation of
+  versioneer
+* [versioningit](https://github.com/jwodder/versioningit) - a PEP 518-based setuptools
+  plugin
+
+## License
+
+To make Versioneer easier to embed, all its code is dedicated to the public
+domain. The `_version.py` that it creates is also in the public domain.
+Specifically, both are released under the Creative Commons "Public Domain
+Dedication" license (CC0-1.0), as described in
+https://creativecommons.org/publicdomain/zero/1.0/ .
+
+[pypi-image]: https://img.shields.io/pypi/v/versioneer.svg
+[pypi-url]: https://pypi.python.org/pypi/versioneer/
+[travis-image]:
+https://img.shields.io/travis/com/python-versioneer/python-versioneer.svg
+[travis-url]: https://travis-ci.com/github/python-versioneer/python-versioneer
+
+"""
+# pylint:disable=invalid-name,import-outside-toplevel,missing-function-docstring
+# pylint:disable=missing-class-docstring,too-many-branches,too-many-statements
+# pylint:disable=raise-missing-from,too-many-lines,too-many-locals,import-error
+# pylint:disable=too-few-public-methods,redefined-outer-name,consider-using-with
+# pylint:disable=attribute-defined-outside-init,too-many-arguments
+
+import configparser
+import errno
+import json
+import os
+import re
+import subprocess
+import sys
+from typing import Callable, Dict
+import functools
+
+
+class VersioneerConfig:
+    """Container for Versioneer configuration parameters."""
+
+
+def get_root():
+    """Get the project root directory.
+
+    We require that all commands are run from the project root, i.e. the
+    directory that contains setup.py, setup.cfg, and versioneer.py .
+    """
+    root = os.path.realpath(os.path.abspath(os.getcwd()))
+    setup_py = os.path.join(root, "setup.py")
+    versioneer_py = os.path.join(root, "versioneer.py")
+    if not (os.path.exists(setup_py) or os.path.exists(versioneer_py)):
+        # allow 'python path/to/setup.py COMMAND'
+        root = os.path.dirname(os.path.realpath(os.path.abspath(sys.argv[0])))
+        setup_py = os.path.join(root, "setup.py")
+        versioneer_py = os.path.join(root, "versioneer.py")
+    if not (os.path.exists(setup_py) or os.path.exists(versioneer_py)):
+        err = (
+            "Versioneer was unable to run the project root directory. "
+            "Versioneer requires setup.py to be executed from "
+            "its immediate directory (like 'python setup.py COMMAND'), "
+            "or in a way that lets it use sys.argv[0] to find the root "
+            "(like 'python path/to/setup.py COMMAND')."
+        )
+        raise VersioneerBadRootError(err)
+    try:
+        # Certain runtime workflows (setup.py install/develop in a setuptools
+        # tree) execute all dependencies in a single python process, so
+        # "versioneer" may be imported multiple times, and python's shared
+        # module-import table will cache the first one. So we can't use
+        # os.path.dirname(__file__), as that will find whichever
+        # versioneer.py was first imported, even in later projects.
+        my_path = os.path.realpath(os.path.abspath(__file__))
+        me_dir = os.path.normcase(os.path.splitext(my_path)[0])
+        vsr_dir = os.path.normcase(os.path.splitext(versioneer_py)[0])
+        if me_dir != vsr_dir:
+            print(
+                "Warning: build in %s is using versioneer.py from %s"
+                % (os.path.dirname(my_path), versioneer_py)
+            )
+    except NameError:
+        pass
+    return root
+
+
+def get_config_from_root(root):
+    """Read the project setup.cfg file to determine Versioneer config."""
+    # This might raise OSError (if setup.cfg is missing), or
+    # configparser.NoSectionError (if it lacks a [versioneer] section), or
+    # configparser.NoOptionError (if it lacks "VCS="). See the docstring at
+    # the top of versioneer.py for instructions on writing your setup.cfg .
+    setup_cfg = os.path.join(root, "setup.cfg")
+    parser = configparser.ConfigParser()
+    with open(setup_cfg, "r") as cfg_file:
+        parser.read_file(cfg_file)
+    VCS = parser.get("versioneer", "VCS")  # mandatory
+
+    # Dict-like interface for non-mandatory entries
+    section = parser["versioneer"]
+
+    cfg = VersioneerConfig()
+    cfg.VCS = VCS
+    cfg.style = section.get("style", "")
+    cfg.versionfile_source = section.get("versionfile_source")
+    cfg.versionfile_build = section.get("versionfile_build")
+    cfg.tag_prefix = section.get("tag_prefix")
+    if cfg.tag_prefix in ("''", '""'):
+        cfg.tag_prefix = ""
+    cfg.parentdir_prefix = section.get("parentdir_prefix")
+    cfg.verbose = section.get("verbose")
+    return cfg
+
+
+class NotThisMethod(Exception):
+    """Exception raised if a method is not valid for the current scenario."""
+
+
+# these dictionaries contain VCS-specific tools
+LONG_VERSION_PY: Dict[str, str] = {}
+HANDLERS: Dict[str, Dict[str, Callable]] = {}
+
+
+def register_vcs_handler(vcs, method):  # decorator
+    """Create decorator to mark a method as the handler of a VCS."""
+
+    def decorate(f):
+        """Store f in HANDLERS[vcs][method]."""
+        HANDLERS.setdefault(vcs, {})[method] = f
+        return f
+
+    return decorate
+
+
+def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False, env=None):
+    """Call the given command(s)."""
+    assert isinstance(commands, list)
+    process = None
+
+    popen_kwargs = {}
+    if sys.platform == "win32":
+        # This hides the console window if pythonw.exe is used
+        startupinfo = subprocess.STARTUPINFO()
+        startupinfo.dwFlags |= subprocess.STARTF_USESHOWWINDOW
+        popen_kwargs["startupinfo"] = startupinfo
+
+    for command in commands:
+        dispcmd = str([command] + args)
+        try:
+            # remember shell=False, so use git.cmd on windows, not just git
+            process = subprocess.Popen(
+                [command] + args,
+                cwd=cwd,
+                env=env,
+                stdout=subprocess.PIPE,
+                stderr=(subprocess.PIPE if hide_stderr else None),
+                **popen_kwargs,
+            )
+            break
+        except OSError:
+            e = sys.exc_info()[1]
+            if e.errno == errno.ENOENT:
+                continue
+            if verbose:
+                print("unable to run %s" % dispcmd)
+                print(e)
+            return None, None
+    else:
+        if verbose:
+            print("unable to find command, tried %s" % (commands,))
+        return None, None
+    stdout = process.communicate()[0].strip().decode()
+    if process.returncode != 0:
+        if verbose:
+            print("unable to run %s (error)" % dispcmd)
+            print("stdout was %s" % stdout)
+        return None, process.returncode
+    return stdout, process.returncode
+
+
+LONG_VERSION_PY[
+    "git"
+] = r'''
+# This file helps to compute a version number in source trees obtained from
+# git-archive tarball (such as those provided by githubs download-from-tag
+# feature). Distribution tarballs (built by setup.py sdist) and build
+# directories (produced by setup.py build) will contain a much shorter file
+# that just contains the computed version number.
+
+# This file is released into the public domain. Generated by
+# versioneer-0.22 (https://github.com/python-versioneer/python-versioneer)
+
+"""Git implementation of _version.py."""
+
+import errno
+import os
+import re
+import subprocess
+import sys
+from typing import Callable, Dict
+import functools
+
+
+def get_keywords():
+    """Get the keywords needed to look up the version information."""
+    # these strings will be replaced by git during git-archive.
+    # setup.py/versioneer.py will grep for the variable names, so they must
+    # each be defined on a line of their own. _version.py will just call
+    # get_keywords().
+    git_refnames = "%(DOLLAR)sFormat:%%d%(DOLLAR)s"
+    git_full = "%(DOLLAR)sFormat:%%H%(DOLLAR)s"
+    git_date = "%(DOLLAR)sFormat:%%ci%(DOLLAR)s"
+    keywords = {"refnames": git_refnames, "full": git_full, "date": git_date}
+    return keywords
+
+
+class VersioneerConfig:
+    """Container for Versioneer configuration parameters."""
+
+
+def get_config():
+    """Create, populate and return the VersioneerConfig() object."""
+    # these strings are filled in when 'setup.py versioneer' creates
+    # _version.py
+    cfg = VersioneerConfig()
+    cfg.VCS = "git"
+    cfg.style = "%(STYLE)s"
+    cfg.tag_prefix = "%(TAG_PREFIX)s"
+    cfg.parentdir_prefix = "%(PARENTDIR_PREFIX)s"
+    cfg.versionfile_source = "%(VERSIONFILE_SOURCE)s"
+    cfg.verbose = False
+    return cfg
+
+
+class NotThisMethod(Exception):
+    """Exception raised if a method is not valid for the current scenario."""
+
+
+LONG_VERSION_PY: Dict[str, str] = {}
+HANDLERS: Dict[str, Dict[str, Callable]] = {}
+
+
+def register_vcs_handler(vcs, method):  # decorator
+    """Create decorator to mark a method as the handler of a VCS."""
+    def decorate(f):
+        """Store f in HANDLERS[vcs][method]."""
+        if vcs not in HANDLERS:
+            HANDLERS[vcs] = {}
+        HANDLERS[vcs][method] = f
+        return f
+    return decorate
+
+
+def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False,
+                env=None):
+    """Call the given command(s)."""
+    assert isinstance(commands, list)
+    process = None
+
+    popen_kwargs = {}
+    if sys.platform == "win32":
+        # This hides the console window if pythonw.exe is used
+        startupinfo = subprocess.STARTUPINFO()
+        startupinfo.dwFlags |= subprocess.STARTF_USESHOWWINDOW
+        popen_kwargs["startupinfo"] = startupinfo
+
+    for command in commands:
+        try:
+            dispcmd = str([command] + args)
+            # remember shell=False, so use git.cmd on windows, not just git
+            process = subprocess.Popen([command] + args, cwd=cwd, env=env,
+                                       stdout=subprocess.PIPE,
+                                       stderr=(subprocess.PIPE if hide_stderr
+                                               else None), **popen_kwargs)
+            break
+        except OSError:
+            e = sys.exc_info()[1]
+            if e.errno == errno.ENOENT:
+                continue
+            if verbose:
+                print("unable to run %%s" %% dispcmd)
+                print(e)
+            return None, None
+    else:
+        if verbose:
+            print("unable to find command, tried %%s" %% (commands,))
+        return None, None
+    stdout = process.communicate()[0].strip().decode()
+    if process.returncode != 0:
+        if verbose:
+            print("unable to run %%s (error)" %% dispcmd)
+            print("stdout was %%s" %% stdout)
+        return None, process.returncode
+    return stdout, process.returncode
+
+
+def versions_from_parentdir(parentdir_prefix, root, verbose):
+    """Try to determine the version from the parent directory name.
+
+    Source tarballs conventionally unpack into a directory that includes both
+    the project name and a version string. We will also support searching up
+    two directory levels for an appropriately named parent directory
+    """
+    rootdirs = []
+
+    for _ in range(3):
+        dirname = os.path.basename(root)
+        if dirname.startswith(parentdir_prefix):
+            return {"version": dirname[len(parentdir_prefix):],
+                    "full-revisionid": None,
+                    "dirty": False, "error": None, "date": None}
+        rootdirs.append(root)
+        root = os.path.dirname(root)  # up a level
+
+    if verbose:
+        print("Tried directories %%s but none started with prefix %%s" %%
+              (str(rootdirs), parentdir_prefix))
+    raise NotThisMethod("rootdir doesn't start with parentdir_prefix")
+
+
+@register_vcs_handler("git", "get_keywords")
+def git_get_keywords(versionfile_abs):
+    """Extract version information from the given file."""
+    # the code embedded in _version.py can just fetch the value of these
+    # keywords. When used from setup.py, we don't want to import _version.py,
+    # so we do it with a regexp instead. This function is not used from
+    # _version.py.
+    keywords = {}
+    try:
+        with open(versionfile_abs, "r") as fobj:
+            for line in fobj:
+                if line.strip().startswith("git_refnames ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["refnames"] = mo.group(1)
+                if line.strip().startswith("git_full ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["full"] = mo.group(1)
+                if line.strip().startswith("git_date ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["date"] = mo.group(1)
+    except OSError:
+        pass
+    return keywords
+
+
+@register_vcs_handler("git", "keywords")
+def git_versions_from_keywords(keywords, tag_prefix, verbose):
+    """Get version information from git keywords."""
+    if "refnames" not in keywords:
+        raise NotThisMethod("Short version file found")
+    date = keywords.get("date")
+    if date is not None:
+        # Use only the last line.  Previous lines may contain GPG signature
+        # information.
+        date = date.splitlines()[-1]
+
+        # git-2.2.0 added "%%cI", which expands to an ISO-8601 -compliant
+        # datestamp. However we prefer "%%ci" (which expands to an "ISO-8601
+        # -like" string, which we must then edit to make compliant), because
+        # it's been around since git-1.5.3, and it's too difficult to
+        # discover which version we're using, or to work around using an
+        # older one.
+        date = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
+    refnames = keywords["refnames"].strip()
+    if refnames.startswith("$Format"):
+        if verbose:
+            print("keywords are unexpanded, not using")
+        raise NotThisMethod("unexpanded keywords, not a git-archive tarball")
+    refs = {r.strip() for r in refnames.strip("()").split(",")}
+    # starting in git-1.8.3, tags are listed as "tag: foo-1.0" instead of
+    # just "foo-1.0". If we see a "tag: " prefix, prefer those.
+    TAG = "tag: "
+    tags = {r[len(TAG):] for r in refs if r.startswith(TAG)}
+    if not tags:
+        # Either we're using git < 1.8.3, or there really are no tags. We use
+        # a heuristic: assume all version tags have a digit. The old git %%d
+        # expansion behaves like git log --decorate=short and strips out the
+        # refs/heads/ and refs/tags/ prefixes that would let us distinguish
+        # between branches and tags. By ignoring refnames without digits, we
+        # filter out many common branch names like "release" and
+        # "stabilization", as well as "HEAD" and "master".
+        tags = {r for r in refs if re.search(r'\d', r)}
+        if verbose:
+            print("discarding '%%s', no digits" %% ",".join(refs - tags))
+    if verbose:
+        print("likely tags: %%s" %% ",".join(sorted(tags)))
+    for ref in sorted(tags):
+        # sorting will prefer e.g. "2.0" over "2.0rc1"
+        if ref.startswith(tag_prefix):
+            r = ref[len(tag_prefix):]
+            # Filter out refs that exactly match prefix or that don't start
+            # with a number once the prefix is stripped (mostly a concern
+            # when prefix is '')
+            if not re.match(r'\d', r):
+                continue
+            if verbose:
+                print("picking %%s" %% r)
+            return {"version": r,
+                    "full-revisionid": keywords["full"].strip(),
+                    "dirty": False, "error": None,
+                    "date": date}
+    # no suitable tags, so version is "0+unknown", but full hex is still there
+    if verbose:
+        print("no suitable tags, using unknown + full revision id")
+    return {"version": "0+unknown",
+            "full-revisionid": keywords["full"].strip(),
+            "dirty": False, "error": "no suitable tags", "date": None}
+
+
+@register_vcs_handler("git", "pieces_from_vcs")
+def git_pieces_from_vcs(tag_prefix, root, verbose, runner=run_command):
+    """Get version from 'git describe' in the root of the source tree.
+
+    This only gets called if the git-archive 'subst' keywords were *not*
+    expanded, and _version.py hasn't already been rewritten with a short
+    version string, meaning we're inside a checked out source tree.
+    """
+    GITS = ["git"]
+    if sys.platform == "win32":
+        GITS = ["git.cmd", "git.exe"]
+
+    # GIT_DIR can interfere with correct operation of Versioneer.
+    # It may be intended to be passed to the Versioneer-versioned project,
+    # but that should not change where we get our version from.
+    env = os.environ.copy()
+    env.pop("GIT_DIR", None)
+    runner = functools.partial(runner, env=env)
+
+    _, rc = runner(GITS, ["rev-parse", "--git-dir"], cwd=root,
+                   hide_stderr=True)
+    if rc != 0:
+        if verbose:
+            print("Directory %%s not under git control" %% root)
+        raise NotThisMethod("'git rev-parse --git-dir' returned error")
+
+    MATCH_ARGS = ["--match", "%%s*" %% tag_prefix] if tag_prefix else []
+
+    # if there is a tag matching tag_prefix, this yields TAG-NUM-gHEX[-dirty]
+    # if there isn't one, this yields HEX[-dirty] (no NUM)
+    describe_out, rc = runner(GITS, ["describe", "--tags", "--dirty",
+                                     "--always", "--long", *MATCH_ARGS],
+                              cwd=root)
+    # --long was added in git-1.5.5
+    if describe_out is None:
+        raise NotThisMethod("'git describe' failed")
+    describe_out = describe_out.strip()
+    full_out, rc = runner(GITS, ["rev-parse", "HEAD"], cwd=root)
+    if full_out is None:
+        raise NotThisMethod("'git rev-parse' failed")
+    full_out = full_out.strip()
+
+    pieces = {}
+    pieces["long"] = full_out
+    pieces["short"] = full_out[:7]  # maybe improved later
+    pieces["error"] = None
+
+    branch_name, rc = runner(GITS, ["rev-parse", "--abbrev-ref", "HEAD"],
+                             cwd=root)
+    # --abbrev-ref was added in git-1.6.3
+    if rc != 0 or branch_name is None:
+        raise NotThisMethod("'git rev-parse --abbrev-ref' returned error")
+    branch_name = branch_name.strip()
+
+    if branch_name == "HEAD":
+        # If we aren't exactly on a branch, pick a branch which represents
+        # the current commit. If all else fails, we are on a branchless
+        # commit.
+        branches, rc = runner(GITS, ["branch", "--contains"], cwd=root)
+        # --contains was added in git-1.5.4
+        if rc != 0 or branches is None:
+            raise NotThisMethod("'git branch --contains' returned error")
+        branches = branches.split("\n")
+
+        # Remove the first line if we're running detached
+        if "(" in branches[0]:
+            branches.pop(0)
+
+        # Strip off the leading "* " from the list of branches.
+        branches = [branch[2:] for branch in branches]
+        if "master" in branches:
+            branch_name = "master"
+        elif not branches:
+            branch_name = None
+        else:
+            # Pick the first branch that is returned. Good or bad.
+            branch_name = branches[0]
+
+    pieces["branch"] = branch_name
+
+    # parse describe_out. It will be like TAG-NUM-gHEX[-dirty] or HEX[-dirty]
+    # TAG might have hyphens.
+    git_describe = describe_out
+
+    # look for -dirty suffix
+    dirty = git_describe.endswith("-dirty")
+    pieces["dirty"] = dirty
+    if dirty:
+        git_describe = git_describe[:git_describe.rindex("-dirty")]
+
+    # now we have TAG-NUM-gHEX or HEX
+
+    if "-" in git_describe:
+        # TAG-NUM-gHEX
+        mo = re.search(r'^(.+)-(\d+)-g([0-9a-f]+)$', git_describe)
+        if not mo:
+            # unparsable. Maybe git-describe is misbehaving?
+            pieces["error"] = ("unable to parse git-describe output: '%%s'"
+                               %% describe_out)
+            return pieces
+
+        # tag
+        full_tag = mo.group(1)
+        if not full_tag.startswith(tag_prefix):
+            if verbose:
+                fmt = "tag '%%s' doesn't start with prefix '%%s'"
+                print(fmt %% (full_tag, tag_prefix))
+            pieces["error"] = ("tag '%%s' doesn't start with prefix '%%s'"
+                               %% (full_tag, tag_prefix))
+            return pieces
+        pieces["closest-tag"] = full_tag[len(tag_prefix):]
+
+        # distance: number of commits since tag
+        pieces["distance"] = int(mo.group(2))
+
+        # commit: short hex revision ID
+        pieces["short"] = mo.group(3)
+
+    else:
+        # HEX: no tags
+        pieces["closest-tag"] = None
+        count_out, rc = runner(GITS, ["rev-list", "HEAD", "--count"], cwd=root)
+        pieces["distance"] = int(count_out)  # total number of commits
+
+    # commit date: see ISO-8601 comment in git_versions_from_keywords()
+    date = runner(GITS, ["show", "-s", "--format=%%ci", "HEAD"], cwd=root)[0].strip()
+    # Use only the last line.  Previous lines may contain GPG signature
+    # information.
+    date = date.splitlines()[-1]
+    pieces["date"] = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
+
+    return pieces
+
+
+def plus_or_dot(pieces):
+    """Return a + if we don't already have one, else return a ."""
+    if "+" in pieces.get("closest-tag", ""):
+        return "."
+    return "+"
+
+
+def render_pep440(pieces):
+    """Build up version string, with post-release "local version identifier".
+
+    Our goal: TAG[+DISTANCE.gHEX[.dirty]] . Note that if you
+    get a tagged build and then dirty it, you'll get TAG+0.gHEX.dirty
+
+    Exceptions:
+    1: no tags. git_describe was just HEX. 0+untagged.DISTANCE.gHEX[.dirty]
+    """
+    if pieces["closest-tag"]:
+        rendered = pieces["closest-tag"]
+        if pieces["distance"] or pieces["dirty"]:
+            rendered += plus_or_dot(pieces)
+            rendered += "%%d.g%%s" %% (pieces["distance"], pieces["short"])
+            if pieces["dirty"]:
+                rendered += ".dirty"
+    else:
+        # exception #1
+        rendered = "0+untagged.%%d.g%%s" %% (pieces["distance"],
+                                          pieces["short"])
+        if pieces["dirty"]:
+            rendered += ".dirty"
+    return rendered
+
+
+def render_pep440_branch(pieces):
+    """TAG[[.dev0]+DISTANCE.gHEX[.dirty]] .
+
+    The ".dev0" means not master branch. Note that .dev0 sorts backwards
+    (a feature branch will appear "older" than the master branch).
+
+    Exceptions:
+    1: no tags. 0[.dev0]+untagged.DISTANCE.gHEX[.dirty]
+    """
+    if pieces["closest-tag"]:
+        rendered = pieces["closest-tag"]
+        if pieces["distance"] or pieces["dirty"]:
+            if pieces["branch"] != "master":
+                rendered += ".dev0"
+            rendered += plus_or_dot(pieces)
+            rendered += "%%d.g%%s" %% (pieces["distance"], pieces["short"])
+            if pieces["dirty"]:
+                rendered += ".dirty"
+    else:
+        # exception #1
+        rendered = "0"
+        if pieces["branch"] != "master":
+            rendered += ".dev0"
+        rendered += "+untagged.%%d.g%%s" %% (pieces["distance"],
+                                          pieces["short"])
+        if pieces["dirty"]:
+            rendered += ".dirty"
+    return rendered
+
+
+def pep440_split_post(ver):
+    """Split pep440 version string at the post-release segment.
+
+    Returns the release segments before the post-release and the
+    post-release version number (or -1 if no post-release segment is present).
+    """
+    vc = str.split(ver, ".post")
+    return vc[0], int(vc[1] or 0) if len(vc) == 2 else None
+
+
+def render_pep440_pre(pieces):
+    """TAG[.postN.devDISTANCE] -- No -dirty.
+
+    Exceptions:
+    1: no tags. 0.post0.devDISTANCE
+    """
+    if pieces["closest-tag"]:
+        if pieces["distance"]:
+            # update the post release segment
+            tag_version, post_version = pep440_split_post(pieces["closest-tag"])
+            rendered = tag_version
+            if post_version is not None:
+                rendered += ".post%%d.dev%%d" %% (post_version+1, pieces["distance"])
+            else:
+                rendered += ".post0.dev%%d" %% (pieces["distance"])
+        else:
+            # no commits, use the tag as the version
+            rendered = pieces["closest-tag"]
+    else:
+        # exception #1
+        rendered = "0.post0.dev%%d" %% pieces["distance"]
+    return rendered
+
+
+def render_pep440_post(pieces):
+    """TAG[.postDISTANCE[.dev0]+gHEX] .
+
+    The ".dev0" means dirty. Note that .dev0 sorts backwards
+    (a dirty tree will appear "older" than the corresponding clean one),
+    but you shouldn't be releasing software with -dirty anyways.
+
+    Exceptions:
+    1: no tags. 0.postDISTANCE[.dev0]
+    """
+    if pieces["closest-tag"]:
+        rendered = pieces["closest-tag"]
+        if pieces["distance"] or pieces["dirty"]:
+            rendered += ".post%%d" %% pieces["distance"]
+            if pieces["dirty"]:
+                rendered += ".dev0"
+            rendered += plus_or_dot(pieces)
+            rendered += "g%%s" %% pieces["short"]
+    else:
+        # exception #1
+        rendered = "0.post%%d" %% pieces["distance"]
+        if pieces["dirty"]:
+            rendered += ".dev0"
+        rendered += "+g%%s" %% pieces["short"]
+    return rendered
+
+
+def render_pep440_post_branch(pieces):
+    """TAG[.postDISTANCE[.dev0]+gHEX[.dirty]] .
+
+    The ".dev0" means not master branch.
+
+    Exceptions:
+    1: no tags. 0.postDISTANCE[.dev0]+gHEX[.dirty]
+    """
+    if pieces["closest-tag"]:
+        rendered = pieces["closest-tag"]
+        if pieces["distance"] or pieces["dirty"]:
+            rendered += ".post%%d" %% pieces["distance"]
+            if pieces["branch"] != "master":
+                rendered += ".dev0"
+            rendered += plus_or_dot(pieces)
+            rendered += "g%%s" %% pieces["short"]
+            if pieces["dirty"]:
+                rendered += ".dirty"
+    else:
+        # exception #1
+        rendered = "0.post%%d" %% pieces["distance"]
+        if pieces["branch"] != "master":
+            rendered += ".dev0"
+        rendered += "+g%%s" %% pieces["short"]
+        if pieces["dirty"]:
+            rendered += ".dirty"
+    return rendered
+
+
+def render_pep440_old(pieces):
+    """TAG[.postDISTANCE[.dev0]] .
+
+    The ".dev0" means dirty.
+
+    Exceptions:
+    1: no tags. 0.postDISTANCE[.dev0]
+    """
+    if pieces["closest-tag"]:
+        rendered = pieces["closest-tag"]
+        if pieces["distance"] or pieces["dirty"]:
+            rendered += ".post%%d" %% pieces["distance"]
+            if pieces["dirty"]:
+                rendered += ".dev0"
+    else:
+        # exception #1
+        rendered = "0.post%%d" %% pieces["distance"]
+        if pieces["dirty"]:
+            rendered += ".dev0"
+    return rendered
+
+
+def render_git_describe(pieces):
+    """TAG[-DISTANCE-gHEX][-dirty].
+
+    Like 'git describe --tags --dirty --always'.
+
+    Exceptions:
+    1: no tags. HEX[-dirty]  (note: no 'g' prefix)
+    """
+    if pieces["closest-tag"]:
+        rendered = pieces["closest-tag"]
+        if pieces["distance"]:
+            rendered += "-%%d-g%%s" %% (pieces["distance"], pieces["short"])
+    else:
+        # exception #1
+        rendered = pieces["short"]
+    if pieces["dirty"]:
+        rendered += "-dirty"
+    return rendered
+
+
+def render_git_describe_long(pieces):
+    """TAG-DISTANCE-gHEX[-dirty].
+
+    Like 'git describe --tags --dirty --always -long'.
+    The distance/hash is unconditional.
+
+    Exceptions:
+    1: no tags. HEX[-dirty]  (note: no 'g' prefix)
+    """
+    if pieces["closest-tag"]:
+        rendered = pieces["closest-tag"]
+        rendered += "-%%d-g%%s" %% (pieces["distance"], pieces["short"])
+    else:
+        # exception #1
+        rendered = pieces["short"]
+    if pieces["dirty"]:
+        rendered += "-dirty"
+    return rendered
+
+
+def render(pieces, style):
+    """Render the given version pieces into the requested style."""
+    if pieces["error"]:
+        return {"version": "unknown",
+                "full-revisionid": pieces.get("long"),
+                "dirty": None,
+                "error": pieces["error"],
+                "date": None}
+
+    if not style or style == "default":
+        style = "pep440"  # the default
+
+    if style == "pep440":
+        rendered = render_pep440(pieces)
+    elif style == "pep440-branch":
+        rendered = render_pep440_branch(pieces)
+    elif style == "pep440-pre":
+        rendered = render_pep440_pre(pieces)
+    elif style == "pep440-post":
+        rendered = render_pep440_post(pieces)
+    elif style == "pep440-post-branch":
+        rendered = render_pep440_post_branch(pieces)
+    elif style == "pep440-old":
+        rendered = render_pep440_old(pieces)
+    elif style == "git-describe":
+        rendered = render_git_describe(pieces)
+    elif style == "git-describe-long":
+        rendered = render_git_describe_long(pieces)
+    else:
+        raise ValueError("unknown style '%%s'" %% style)
+
+    return {"version": rendered, "full-revisionid": pieces["long"],
+            "dirty": pieces["dirty"], "error": None,
+            "date": pieces.get("date")}
+
+
+def get_versions():
+    """Get version information or return default if unable to do so."""
+    # I am in _version.py, which lives at ROOT/VERSIONFILE_SOURCE. If we have
+    # __file__, we can work backwards from there to the root. Some
+    # py2exe/bbfreeze/non-CPython implementations don't do __file__, in which
+    # case we can only use expanded keywords.
+
+    cfg = get_config()
+    verbose = cfg.verbose
+
+    try:
+        return git_versions_from_keywords(get_keywords(), cfg.tag_prefix,
+                                          verbose)
+    except NotThisMethod:
+        pass
+
+    try:
+        root = os.path.realpath(__file__)
+        # versionfile_source is the relative path from the top of the source
+        # tree (where the .git directory might live) to this file. Invert
+        # this to find the root from __file__.
+        for _ in cfg.versionfile_source.split('/'):
+            root = os.path.dirname(root)
+    except NameError:
+        return {"version": "0+unknown", "full-revisionid": None,
+                "dirty": None,
+                "error": "unable to find root of source tree",
+                "date": None}
+
+    try:
+        pieces = git_pieces_from_vcs(cfg.tag_prefix, root, verbose)
+        return render(pieces, cfg.style)
+    except NotThisMethod:
+        pass
+
+    try:
+        if cfg.parentdir_prefix:
+            return versions_from_parentdir(cfg.parentdir_prefix, root, verbose)
+    except NotThisMethod:
+        pass
+
+    return {"version": "0+unknown", "full-revisionid": None,
+            "dirty": None,
+            "error": "unable to compute version", "date": None}
+'''
+
+
+@register_vcs_handler("git", "get_keywords")
+def git_get_keywords(versionfile_abs):
+    """Extract version information from the given file."""
+    # the code embedded in _version.py can just fetch the value of these
+    # keywords. When used from setup.py, we don't want to import _version.py,
+    # so we do it with a regexp instead. This function is not used from
+    # _version.py.
+    keywords = {}
+    try:
+        with open(versionfile_abs, "r") as fobj:
+            for line in fobj:
+                if line.strip().startswith("git_refnames ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["refnames"] = mo.group(1)
+                if line.strip().startswith("git_full ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["full"] = mo.group(1)
+                if line.strip().startswith("git_date ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["date"] = mo.group(1)
+    except OSError:
+        pass
+    return keywords
+
+
+@register_vcs_handler("git", "keywords")
+def git_versions_from_keywords(keywords, tag_prefix, verbose):
+    """Get version information from git keywords."""
+    if "refnames" not in keywords:
+        raise NotThisMethod("Short version file found")
+    date = keywords.get("date")
+    if date is not None:
+        # Use only the last line.  Previous lines may contain GPG signature
+        # information.
+        date = date.splitlines()[-1]
+
+        # git-2.2.0 added "%cI", which expands to an ISO-8601 -compliant
+        # datestamp. However we prefer "%ci" (which expands to an "ISO-8601
+        # -like" string, which we must then edit to make compliant), because
+        # it's been around since git-1.5.3, and it's too difficult to
+        # discover which version we're using, or to work around using an
+        # older one.
+        date = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
+    refnames = keywords["refnames"].strip()
+    if refnames.startswith("$Format"):
+        if verbose:
+            print("keywords are unexpanded, not using")
+        raise NotThisMethod("unexpanded keywords, not a git-archive tarball")
+    refs = {r.strip() for r in refnames.strip("()").split(",")}
+    # starting in git-1.8.3, tags are listed as "tag: foo-1.0" instead of
+    # just "foo-1.0". If we see a "tag: " prefix, prefer those.
+    TAG = "tag: "
+    tags = {r[len(TAG) :] for r in refs if r.startswith(TAG)}
+    if not tags:
+        # Either we're using git < 1.8.3, or there really are no tags. We use
+        # a heuristic: assume all version tags have a digit. The old git %d
+        # expansion behaves like git log --decorate=short and strips out the
+        # refs/heads/ and refs/tags/ prefixes that would let us distinguish
+        # between branches and tags. By ignoring refnames without digits, we
+        # filter out many common branch names like "release" and
+        # "stabilization", as well as "HEAD" and "master".
+        tags = {r for r in refs if re.search(r"\d", r)}
+        if verbose:
+            print("discarding '%s', no digits" % ",".join(refs - tags))
+    if verbose:
+        print("likely tags: %s" % ",".join(sorted(tags)))
+    for ref in sorted(tags):
+        # sorting will prefer e.g. "2.0" over "2.0rc1"
+        if ref.startswith(tag_prefix):
+            r = ref[len(tag_prefix) :]
+            # Filter out refs that exactly match prefix or that don't start
+            # with a number once the prefix is stripped (mostly a concern
+            # when prefix is '')
+            if not re.match(r"\d", r):
+                continue
+            if verbose:
+                print("picking %s" % r)
+            return {
+                "version": r,
+                "full-revisionid": keywords["full"].strip(),
+                "dirty": False,
+                "error": None,
+                "date": date,
+            }
+    # no suitable tags, so version is "0+unknown", but full hex is still there
+    if verbose:
+        print("no suitable tags, using unknown + full revision id")
+    return {
+        "version": "0+unknown",
+        "full-revisionid": keywords["full"].strip(),
+        "dirty": False,
+        "error": "no suitable tags",
+        "date": None,
+    }
+
+
+@register_vcs_handler("git", "pieces_from_vcs")
+def git_pieces_from_vcs(tag_prefix, root, verbose, runner=run_command):
+    """Get version from 'git describe' in the root of the source tree.
+
+    This only gets called if the git-archive 'subst' keywords were *not*
+    expanded, and _version.py hasn't already been rewritten with a short
+    version string, meaning we're inside a checked out source tree.
+    """
+    GITS = ["git"]
+    if sys.platform == "win32":
+        GITS = ["git.cmd", "git.exe"]
+
+    # GIT_DIR can interfere with correct operation of Versioneer.
+    # It may be intended to be passed to the Versioneer-versioned project,
+    # but that should not change where we get our version from.
+    env = os.environ.copy()
+    env.pop("GIT_DIR", None)
+    runner = functools.partial(runner, env=env)
+
+    _, rc = runner(GITS, ["rev-parse", "--git-dir"], cwd=root, hide_stderr=True)
+    if rc != 0:
+        if verbose:
+            print("Directory %s not under git control" % root)
+        raise NotThisMethod("'git rev-parse --git-dir' returned error")
+
+    MATCH_ARGS = ["--match", "%s*" % tag_prefix] if tag_prefix else []
+
+    # if there is a tag matching tag_prefix, this yields TAG-NUM-gHEX[-dirty]
+    # if there isn't one, this yields HEX[-dirty] (no NUM)
+    describe_out, rc = runner(
+        GITS,
+        ["describe", "--tags", "--dirty", "--always", "--long", *MATCH_ARGS],
+        cwd=root,
+    )
+    # --long was added in git-1.5.5
+    if describe_out is None:
+        raise NotThisMethod("'git describe' failed")
+    describe_out = describe_out.strip()
+    full_out, rc = runner(GITS, ["rev-parse", "HEAD"], cwd=root)
+    if full_out is None:
+        raise NotThisMethod("'git rev-parse' failed")
+    full_out = full_out.strip()
+
+    pieces = {}
+    pieces["long"] = full_out
+    pieces["short"] = full_out[:7]  # maybe improved later
+    pieces["error"] = None
+
+    branch_name, rc = runner(GITS, ["rev-parse", "--abbrev-ref", "HEAD"], cwd=root)
+    # --abbrev-ref was added in git-1.6.3
+    if rc != 0 or branch_name is None:
+        raise NotThisMethod("'git rev-parse --abbrev-ref' returned error")
+    branch_name = branch_name.strip()
+
+    if branch_name == "HEAD":
+        # If we aren't exactly on a branch, pick a branch which represents
+        # the current commit. If all else fails, we are on a branchless
+        # commit.
+        branches, rc = runner(GITS, ["branch", "--contains"], cwd=root)
+        # --contains was added in git-1.5.4
+        if rc != 0 or branches is None:
+            raise NotThisMethod("'git branch --contains' returned error")
+        branches = branches.split("\n")
+
+        # Remove the first line if we're running detached
+        if "(" in branches[0]:
+            branches.pop(0)
+
+        # Strip off the leading "* " from the list of branches.
+        branches = [branch[2:] for branch in branches]
+        if "master" in branches:
+            branch_name = "master"
+        elif not branches:
+            branch_name = None
+        else:
+            # Pick the first branch that is returned. Good or bad.
+            branch_name = branches[0]
+
+    pieces["branch"] = branch_name
+
+    # parse describe_out. It will be like TAG-NUM-gHEX[-dirty] or HEX[-dirty]
+    # TAG might have hyphens.
+    git_describe = describe_out
+
+    # look for -dirty suffix
+    dirty = git_describe.endswith("-dirty")
+    pieces["dirty"] = dirty
+    if dirty:
+        git_describe = git_describe[: git_describe.rindex("-dirty")]
+
+    # now we have TAG-NUM-gHEX or HEX
+
+    if "-" in git_describe:
+        # TAG-NUM-gHEX
+        mo = re.search(r"^(.+)-(\d+)-g([0-9a-f]+)$", git_describe)
+        if not mo:
+            # unparsable. Maybe git-describe is misbehaving?
+            pieces["error"] = "unable to parse git-describe output: '%s'" % describe_out
+            return pieces
+
+        # tag
+        full_tag = mo.group(1)
+        if not full_tag.startswith(tag_prefix):
+            if verbose:
+                fmt = "tag '%s' doesn't start with prefix '%s'"
+                print(fmt % (full_tag, tag_prefix))
+            pieces["error"] = "tag '%s' doesn't start with prefix '%s'" % (
+                full_tag,
+                tag_prefix,
+            )
+            return pieces
+        pieces["closest-tag"] = full_tag[len(tag_prefix) :]
+
+        # distance: number of commits since tag
+        pieces["distance"] = int(mo.group(2))
+
+        # commit: short hex revision ID
+        pieces["short"] = mo.group(3)
+
+    else:
+        # HEX: no tags
+        pieces["closest-tag"] = None
+        count_out, rc = runner(GITS, ["rev-list", "HEAD", "--count"], cwd=root)
+        pieces["distance"] = int(count_out)  # total number of commits
+
+    # commit date: see ISO-8601 comment in git_versions_from_keywords()
+    date = runner(GITS, ["show", "-s", "--format=%ci", "HEAD"], cwd=root)[0].strip()
+    # Use only the last line.  Previous lines may contain GPG signature
+    # information.
+    date = date.splitlines()[-1]
+    pieces["date"] = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
+
+    return pieces
+
+
+def do_vcs_install(manifest_in, versionfile_source, ipy):
+    """Git-specific installation logic for Versioneer.
+
+    For Git, this means creating/changing .gitattributes to mark _version.py
+    for export-subst keyword substitution.
+    """
+    GITS = ["git"]
+    if sys.platform == "win32":
+        GITS = ["git.cmd", "git.exe"]
+    files = [manifest_in, versionfile_source]
+    if ipy:
+        files.append(ipy)
+    try:
+        my_path = __file__
+        if my_path.endswith(".pyc") or my_path.endswith(".pyo"):
+            my_path = os.path.splitext(my_path)[0] + ".py"
+        versioneer_file = os.path.relpath(my_path)
+    except NameError:
+        versioneer_file = "versioneer.py"
+    files.append(versioneer_file)
+    present = False
+    try:
+        with open(".gitattributes", "r") as fobj:
+            for line in fobj:
+                if line.strip().startswith(versionfile_source):
+                    if "export-subst" in line.strip().split()[1:]:
+                        present = True
+                        break
+    except OSError:
+        pass
+    if not present:
+        with open(".gitattributes", "a+") as fobj:
+            fobj.write(f"{versionfile_source} export-subst\n")
+        files.append(".gitattributes")
+    run_command(GITS, ["add", "--"] + files)
+
+
+def versions_from_parentdir(parentdir_prefix, root, verbose):
+    """Try to determine the version from the parent directory name.
+
+    Source tarballs conventionally unpack into a directory that includes both
+    the project name and a version string. We will also support searching up
+    two directory levels for an appropriately named parent directory
+    """
+    rootdirs = []
+
+    for _ in range(3):
+        dirname = os.path.basename(root)
+        if dirname.startswith(parentdir_prefix):
+            return {
+                "version": dirname[len(parentdir_prefix) :],
+                "full-revisionid": None,
+                "dirty": False,
+                "error": None,
+                "date": None,
+            }
+        rootdirs.append(root)
+        root = os.path.dirname(root)  # up a level
+
+    if verbose:
+        print(
+            "Tried directories %s but none started with prefix %s"
+            % (str(rootdirs), parentdir_prefix)
+        )
+    raise NotThisMethod("rootdir doesn't start with parentdir_prefix")
+
+
+SHORT_VERSION_PY = """
+# This file was generated by 'versioneer.py' (0.22) from
+# revision-control system data, or from the parent directory name of an
+# unpacked source archive. Distribution tarballs contain a pre-generated copy
+# of this file.
+
+import json
+
+version_json = '''
+%s
+'''  # END VERSION_JSON
+
+
+def get_versions():
+    return json.loads(version_json)
+"""
+
+
+def versions_from_file(filename):
+    """Try to determine the version from _version.py if present."""
+    try:
+        with open(filename) as f:
+            contents = f.read()
+    except OSError:
+        raise NotThisMethod("unable to read _version.py")
+    mo = re.search(
+        r"version_json = '''\n(.*)'''  # END VERSION_JSON", contents, re.M | re.S
+    )
+    if not mo:
+        mo = re.search(
+            r"version_json = '''\r\n(.*)'''  # END VERSION_JSON", contents, re.M | re.S
+        )
+    if not mo:
+        raise NotThisMethod("no version_json in _version.py")
+    return json.loads(mo.group(1))
+
+
+def write_to_version_file(filename, versions):
+    """Write the given version number to the given _version.py file."""
+    os.unlink(filename)
+    contents = json.dumps(versions, sort_keys=True, indent=1, separators=(",", ": "))
+    with open(filename, "w") as f:
+        f.write(SHORT_VERSION_PY % contents)
+
+    print("set %s to '%s'" % (filename, versions["version"]))
+
+
+def plus_or_dot(pieces):
+    """Return a + if we don't already have one, else return a ."""
+    if "+" in pieces.get("closest-tag", ""):
+        return "."
+    return "+"
+
+
+def render_pep440(pieces):
+    """Build up version string, with post-release "local version identifier".
+
+    Our goal: TAG[+DISTANCE.gHEX[.dirty]] . Note that if you
+    get a tagged build and then dirty it, you'll get TAG+0.gHEX.dirty
+
+    Exceptions:
+    1: no tags. git_describe was just HEX. 0+untagged.DISTANCE.gHEX[.dirty]
+    """
+    if pieces["closest-tag"]:
+        rendered = pieces["closest-tag"]
+        if pieces["distance"] or pieces["dirty"]:
+            rendered += plus_or_dot(pieces)
+            rendered += "%d.g%s" % (pieces["distance"], pieces["short"])
+            if pieces["dirty"]:
+                rendered += ".dirty"
+    else:
+        # exception #1
+        rendered = "0+untagged.%d.g%s" % (pieces["distance"], pieces["short"])
+        if pieces["dirty"]:
+            rendered += ".dirty"
+    return rendered
+
+
+def render_pep440_branch(pieces):
+    """TAG[[.dev0]+DISTANCE.gHEX[.dirty]] .
+
+    The ".dev0" means not master branch. Note that .dev0 sorts backwards
+    (a feature branch will appear "older" than the master branch).
+
+    Exceptions:
+    1: no tags. 0[.dev0]+untagged.DISTANCE.gHEX[.dirty]
+    """
+    if pieces["closest-tag"]:
+        rendered = pieces["closest-tag"]
+        if pieces["distance"] or pieces["dirty"]:
+            if pieces["branch"] != "master":
+                rendered += ".dev0"
+            rendered += plus_or_dot(pieces)
+            rendered += "%d.g%s" % (pieces["distance"], pieces["short"])
+            if pieces["dirty"]:
+                rendered += ".dirty"
+    else:
+        # exception #1
+        rendered = "0"
+        if pieces["branch"] != "master":
+            rendered += ".dev0"
+        rendered += "+untagged.%d.g%s" % (pieces["distance"], pieces["short"])
+        if pieces["dirty"]:
+            rendered += ".dirty"
+    return rendered
+
+
+def pep440_split_post(ver):
+    """Split pep440 version string at the post-release segment.
+
+    Returns the release segments before the post-release and the
+    post-release version number (or -1 if no post-release segment is present).
+    """
+    vc = str.split(ver, ".post")
+    return vc[0], int(vc[1] or 0) if len(vc) == 2 else None
+
+
+def render_pep440_pre(pieces):
+    """TAG[.postN.devDISTANCE] -- No -dirty.
+
+    Exceptions:
+    1: no tags. 0.post0.devDISTANCE
+    """
+    if pieces["closest-tag"]:
+        if pieces["distance"]:
+            # update the post release segment
+            tag_version, post_version = pep440_split_post(pieces["closest-tag"])
+            rendered = tag_version
+            if post_version is not None:
+                rendered += ".post%d.dev%d" % (post_version + 1, pieces["distance"])
+            else:
+                rendered += ".post0.dev%d" % (pieces["distance"])
+        else:
+            # no commits, use the tag as the version
+            rendered = pieces["closest-tag"]
+    else:
+        # exception #1
+        rendered = "0.post0.dev%d" % pieces["distance"]
+    return rendered
+
+
+def render_pep440_post(pieces):
+    """TAG[.postDISTANCE[.dev0]+gHEX] .
+
+    The ".dev0" means dirty. Note that .dev0 sorts backwards
+    (a dirty tree will appear "older" than the corresponding clean one),
+    but you shouldn't be releasing software with -dirty anyways.
+
+    Exceptions:
+    1: no tags. 0.postDISTANCE[.dev0]
+    """
+    if pieces["closest-tag"]:
+        rendered = pieces["closest-tag"]
+        if pieces["distance"] or pieces["dirty"]:
+            rendered += ".post%d" % pieces["distance"]
+            if pieces["dirty"]:
+                rendered += ".dev0"
+            rendered += plus_or_dot(pieces)
+            rendered += "g%s" % pieces["short"]
+    else:
+        # exception #1
+        rendered = "0.post%d" % pieces["distance"]
+        if pieces["dirty"]:
+            rendered += ".dev0"
+        rendered += "+g%s" % pieces["short"]
+    return rendered
+
+
+def render_pep440_post_branch(pieces):
+    """TAG[.postDISTANCE[.dev0]+gHEX[.dirty]] .
+
+    The ".dev0" means not master branch.
+
+    Exceptions:
+    1: no tags. 0.postDISTANCE[.dev0]+gHEX[.dirty]
+    """
+    if pieces["closest-tag"]:
+        rendered = pieces["closest-tag"]
+        if pieces["distance"] or pieces["dirty"]:
+            rendered += ".post%d" % pieces["distance"]
+            if pieces["branch"] != "master":
+                rendered += ".dev0"
+            rendered += plus_or_dot(pieces)
+            rendered += "g%s" % pieces["short"]
+            if pieces["dirty"]:
+                rendered += ".dirty"
+    else:
+        # exception #1
+        rendered = "0.post%d" % pieces["distance"]
+        if pieces["branch"] != "master":
+            rendered += ".dev0"
+        rendered += "+g%s" % pieces["short"]
+        if pieces["dirty"]:
+            rendered += ".dirty"
+    return rendered
+
+
+def render_pep440_old(pieces):
+    """TAG[.postDISTANCE[.dev0]] .
+
+    The ".dev0" means dirty.
+
+    Exceptions:
+    1: no tags. 0.postDISTANCE[.dev0]
+    """
+    if pieces["closest-tag"]:
+        rendered = pieces["closest-tag"]
+        if pieces["distance"] or pieces["dirty"]:
+            rendered += ".post%d" % pieces["distance"]
+            if pieces["dirty"]:
+                rendered += ".dev0"
+    else:
+        # exception #1
+        rendered = "0.post%d" % pieces["distance"]
+        if pieces["dirty"]:
+            rendered += ".dev0"
+    return rendered
+
+
+def render_git_describe(pieces):
+    """TAG[-DISTANCE-gHEX][-dirty].
+
+    Like 'git describe --tags --dirty --always'.
+
+    Exceptions:
+    1: no tags. HEX[-dirty]  (note: no 'g' prefix)
+    """
+    if pieces["closest-tag"]:
+        rendered = pieces["closest-tag"]
+        if pieces["distance"]:
+            rendered += "-%d-g%s" % (pieces["distance"], pieces["short"])
+    else:
+        # exception #1
+        rendered = pieces["short"]
+    if pieces["dirty"]:
+        rendered += "-dirty"
+    return rendered
+
+
+def render_git_describe_long(pieces):
+    """TAG-DISTANCE-gHEX[-dirty].
+
+    Like 'git describe --tags --dirty --always -long'.
+    The distance/hash is unconditional.
+
+    Exceptions:
+    1: no tags. HEX[-dirty]  (note: no 'g' prefix)
+    """
+    if pieces["closest-tag"]:
+        rendered = pieces["closest-tag"]
+        rendered += "-%d-g%s" % (pieces["distance"], pieces["short"])
+    else:
+        # exception #1
+        rendered = pieces["short"]
+    if pieces["dirty"]:
+        rendered += "-dirty"
+    return rendered
+
+
+def render(pieces, style):
+    """Render the given version pieces into the requested style."""
+    if pieces["error"]:
+        return {
+            "version": "unknown",
+            "full-revisionid": pieces.get("long"),
+            "dirty": None,
+            "error": pieces["error"],
+            "date": None,
+        }
+
+    if not style or style == "default":
+        style = "pep440"  # the default
+
+    if style == "pep440":
+        rendered = render_pep440(pieces)
+    elif style == "pep440-branch":
+        rendered = render_pep440_branch(pieces)
+    elif style == "pep440-pre":
+        rendered = render_pep440_pre(pieces)
+    elif style == "pep440-post":
+        rendered = render_pep440_post(pieces)
+    elif style == "pep440-post-branch":
+        rendered = render_pep440_post_branch(pieces)
+    elif style == "pep440-old":
+        rendered = render_pep440_old(pieces)
+    elif style == "git-describe":
+        rendered = render_git_describe(pieces)
+    elif style == "git-describe-long":
+        rendered = render_git_describe_long(pieces)
+    else:
+        raise ValueError("unknown style '%s'" % style)
+
+    return {
+        "version": rendered,
+        "full-revisionid": pieces["long"],
+        "dirty": pieces["dirty"],
+        "error": None,
+        "date": pieces.get("date"),
+    }
+
+
+class VersioneerBadRootError(Exception):
+    """The project root directory is unknown or missing key files."""
+
+
+def get_versions(verbose=False):
+    """Get the project version from whatever source is available.
+
+    Returns dict with two keys: 'version' and 'full'.
+    """
+    if "versioneer" in sys.modules:
+        # see the discussion in cmdclass.py:get_cmdclass()
+        del sys.modules["versioneer"]
+
+    root = get_root()
+    cfg = get_config_from_root(root)
+
+    assert cfg.VCS is not None, "please set [versioneer]VCS= in setup.cfg"
+    handlers = HANDLERS.get(cfg.VCS)
+    assert handlers, "unrecognized VCS '%s'" % cfg.VCS
+    verbose = verbose or cfg.verbose
+    assert (
+        cfg.versionfile_source is not None
+    ), "please set versioneer.versionfile_source"
+    assert cfg.tag_prefix is not None, "please set versioneer.tag_prefix"
+
+    versionfile_abs = os.path.join(root, cfg.versionfile_source)
+
+    # extract version from first of: _version.py, VCS command (e.g. 'git
+    # describe'), parentdir. This is meant to work for developers using a
+    # source checkout, for users of a tarball created by 'setup.py sdist',
+    # and for users of a tarball/zipball created by 'git archive' or github's
+    # download-from-tag feature or the equivalent in other VCSes.
+
+    get_keywords_f = handlers.get("get_keywords")
+    from_keywords_f = handlers.get("keywords")
+    if get_keywords_f and from_keywords_f:
+        try:
+            keywords = get_keywords_f(versionfile_abs)
+            ver = from_keywords_f(keywords, cfg.tag_prefix, verbose)
+            if verbose:
+                print("got version from expanded keyword %s" % ver)
+            return ver
+        except NotThisMethod:
+            pass
+
+    try:
+        ver = versions_from_file(versionfile_abs)
+        if verbose:
+            print("got version from file %s %s" % (versionfile_abs, ver))
+        return ver
+    except NotThisMethod:
+        pass
+
+    from_vcs_f = handlers.get("pieces_from_vcs")
+    if from_vcs_f:
+        try:
+            pieces = from_vcs_f(cfg.tag_prefix, root, verbose)
+            ver = render(pieces, cfg.style)
+            if verbose:
+                print("got version from VCS %s" % ver)
+            return ver
+        except NotThisMethod:
+            pass
+
+    try:
+        if cfg.parentdir_prefix:
+            ver = versions_from_parentdir(cfg.parentdir_prefix, root, verbose)
+            if verbose:
+                print("got version from parentdir %s" % ver)
+            return ver
+    except NotThisMethod:
+        pass
+
+    if verbose:
+        print("unable to compute version")
+
+    return {
+        "version": "0+unknown",
+        "full-revisionid": None,
+        "dirty": None,
+        "error": "unable to compute version",
+        "date": None,
+    }
+
+
+def get_version():
+    """Get the short version string for this project."""
+    return get_versions()["version"]
+
+
+def get_cmdclass(cmdclass=None):
+    """Get the custom setuptools/distutils subclasses used by Versioneer.
+
+    If the package uses a different cmdclass (e.g. one from numpy), it
+    should be provide as an argument.
+    """
+    if "versioneer" in sys.modules:
+        del sys.modules["versioneer"]
+        # this fixes the "python setup.py develop" case (also 'install' and
+        # 'easy_install .'), in which subdependencies of the main project are
+        # built (using setup.py bdist_egg) in the same python process. Assume
+        # a main project A and a dependency B, which use different versions
+        # of Versioneer. A's setup.py imports A's Versioneer, leaving it in
+        # sys.modules by the time B's setup.py is executed, causing B to run
+        # with the wrong versioneer. Setuptools wraps the sub-dep builds in a
+        # sandbox that restores sys.modules to it's pre-build state, so the
+        # parent is protected against the child's "import versioneer". By
+        # removing ourselves from sys.modules here, before the child build
+        # happens, we protect the child from the parent's versioneer too.
+        # Also see https://github.com/python-versioneer/python-versioneer/issues/52
+
+    cmds = {} if cmdclass is None else cmdclass.copy()
+
+    # we add "version" to both distutils and setuptools
+    try:
+        from setuptools import Command
+    except ImportError:
+        from distutils.core import Command
+
+    class cmd_version(Command):
+        description = "report generated version string"
+        user_options = []
+        boolean_options = []
+
+        def initialize_options(self):
+            pass
+
+        def finalize_options(self):
+            pass
+
+        def run(self):
+            vers = get_versions(verbose=True)
+            print("Version: %s" % vers["version"])
+            print(" full-revisionid: %s" % vers.get("full-revisionid"))
+            print(" dirty: %s" % vers.get("dirty"))
+            print(" date: %s" % vers.get("date"))
+            if vers["error"]:
+                print(" error: %s" % vers["error"])
+
+    cmds["version"] = cmd_version
+
+    # we override "build_py" in both distutils and setuptools
+    #
+    # most invocation pathways end up running build_py:
+    #  distutils/build -> build_py
+    #  distutils/install -> distutils/build ->..
+    #  setuptools/bdist_wheel -> distutils/install ->..
+    #  setuptools/bdist_egg -> distutils/install_lib -> build_py
+    #  setuptools/install -> bdist_egg ->..
+    #  setuptools/develop -> ?
+    #  pip install:
+    #   copies source tree to a tempdir before running egg_info/etc
+    #   if .git isn't copied too, 'git describe' will fail
+    #   then does setup.py bdist_wheel, or sometimes setup.py install
+    #  setup.py egg_info -> ?
+
+    # we override different "build_py" commands for both environments
+    if "build_py" in cmds:
+        _build_py = cmds["build_py"]
+    elif "setuptools" in sys.modules:
+        from setuptools.command.build_py import build_py as _build_py
+    else:
+        from distutils.command.build_py import build_py as _build_py
+
+    class cmd_build_py(_build_py):
+        def run(self):
+            root = get_root()
+            cfg = get_config_from_root(root)
+            versions = get_versions()
+            _build_py.run(self)
+            # now locate _version.py in the new build/ directory and replace
+            # it with an updated value
+            if cfg.versionfile_build:
+                target_versionfile = os.path.join(self.build_lib, cfg.versionfile_build)
+                print("UPDATING %s" % target_versionfile)
+                write_to_version_file(target_versionfile, versions)
+
+    cmds["build_py"] = cmd_build_py
+
+    if "build_ext" in cmds:
+        _build_ext = cmds["build_ext"]
+    elif "setuptools" in sys.modules:
+        from setuptools.command.build_ext import build_ext as _build_ext
+    else:
+        from distutils.command.build_ext import build_ext as _build_ext
+
+    class cmd_build_ext(_build_ext):
+        def run(self):
+            root = get_root()
+            cfg = get_config_from_root(root)
+            versions = get_versions()
+            _build_ext.run(self)
+            if self.inplace:
+                # build_ext --inplace will only build extensions in
+                # build/lib<..> dir with no _version.py to write to.
+                # As in place builds will already have a _version.py
+                # in the module dir, we do not need to write one.
+                return
+            # now locate _version.py in the new build/ directory and replace
+            # it with an updated value
+            target_versionfile = os.path.join(self.build_lib, cfg.versionfile_build)
+            print("UPDATING %s" % target_versionfile)
+            write_to_version_file(target_versionfile, versions)
+
+    cmds["build_ext"] = cmd_build_ext
+
+    if "cx_Freeze" in sys.modules:  # cx_freeze enabled?
+        from cx_Freeze.dist import build_exe as _build_exe
+
+        # nczeczulin reports that py2exe won't like the pep440-style string
+        # as FILEVERSION, but it can be used for PRODUCTVERSION, e.g.
+        # setup(console=[{
+        #   "version": versioneer.get_version().split("+", 1)[0], # FILEVERSION
+        #   "product_version": versioneer.get_version(),
+        #   ...
+
+        class cmd_build_exe(_build_exe):
+            def run(self):
+                root = get_root()
+                cfg = get_config_from_root(root)
+                versions = get_versions()
+                target_versionfile = cfg.versionfile_source
+                print("UPDATING %s" % target_versionfile)
+                write_to_version_file(target_versionfile, versions)
+
+                _build_exe.run(self)
+                os.unlink(target_versionfile)
+                with open(cfg.versionfile_source, "w") as f:
+                    LONG = LONG_VERSION_PY[cfg.VCS]
+                    f.write(
+                        LONG
+                        % {
+                            "DOLLAR": "$",
+                            "STYLE": cfg.style,
+                            "TAG_PREFIX": cfg.tag_prefix,
+                            "PARENTDIR_PREFIX": cfg.parentdir_prefix,
+                            "VERSIONFILE_SOURCE": cfg.versionfile_source,
+                        }
+                    )
+
+        cmds["build_exe"] = cmd_build_exe
+        del cmds["build_py"]
+
+    if "py2exe" in sys.modules:  # py2exe enabled?
+        from py2exe.distutils_buildexe import py2exe as _py2exe
+
+        class cmd_py2exe(_py2exe):
+            def run(self):
+                root = get_root()
+                cfg = get_config_from_root(root)
+                versions = get_versions()
+                target_versionfile = cfg.versionfile_source
+                print("UPDATING %s" % target_versionfile)
+                write_to_version_file(target_versionfile, versions)
+
+                _py2exe.run(self)
+                os.unlink(target_versionfile)
+                with open(cfg.versionfile_source, "w") as f:
+                    LONG = LONG_VERSION_PY[cfg.VCS]
+                    f.write(
+                        LONG
+                        % {
+                            "DOLLAR": "$",
+                            "STYLE": cfg.style,
+                            "TAG_PREFIX": cfg.tag_prefix,
+                            "PARENTDIR_PREFIX": cfg.parentdir_prefix,
+                            "VERSIONFILE_SOURCE": cfg.versionfile_source,
+                        }
+                    )
+
+        cmds["py2exe"] = cmd_py2exe
+
+    # we override different "sdist" commands for both environments
+    if "sdist" in cmds:
+        _sdist = cmds["sdist"]
+    elif "setuptools" in sys.modules:
+        from setuptools.command.sdist import sdist as _sdist
+    else:
+        from distutils.command.sdist import sdist as _sdist
+
+    class cmd_sdist(_sdist):
+        def run(self):
+            versions = get_versions()
+            self._versioneer_generated_versions = versions
+            # unless we update this, the command will keep using the old
+            # version
+            self.distribution.metadata.version = versions["version"]
+            return _sdist.run(self)
+
+        def make_release_tree(self, base_dir, files):
+            root = get_root()
+            cfg = get_config_from_root(root)
+            _sdist.make_release_tree(self, base_dir, files)
+            # now locate _version.py in the new base_dir directory
+            # (remembering that it may be a hardlink) and replace it with an
+            # updated value
+            target_versionfile = os.path.join(base_dir, cfg.versionfile_source)
+            print("UPDATING %s" % target_versionfile)
+            write_to_version_file(
+                target_versionfile, self._versioneer_generated_versions
+            )
+
+    cmds["sdist"] = cmd_sdist
+
+    return cmds
+
+
+CONFIG_ERROR = """
+setup.cfg is missing the necessary Versioneer configuration. You need
+a section like:
+
+ [versioneer]
+ VCS = git
+ style = pep440
+ versionfile_source = src/myproject/_version.py
+ versionfile_build = myproject/_version.py
+ tag_prefix =
+ parentdir_prefix = myproject-
+
+You will also need to edit your setup.py to use the results:
+
+ import versioneer
+ setup(version=versioneer.get_version(),
+       cmdclass=versioneer.get_cmdclass(), ...)
+
+Please read the docstring in ./versioneer.py for configuration instructions,
+edit setup.cfg, and re-run the installer or 'python versioneer.py setup'.
+"""
+
+SAMPLE_CONFIG = """
+# See the docstring in versioneer.py for instructions. Note that you must
+# re-run 'versioneer.py setup' after changing this section, and commit the
+# resulting files.
+
+[versioneer]
+#VCS = git
+#style = pep440
+#versionfile_source =
+#versionfile_build =
+#tag_prefix =
+#parentdir_prefix =
+
+"""
+
+OLD_SNIPPET = """
+from ._version import get_versions
+__version__ = get_versions()['version']
+del get_versions
+"""
+
+INIT_PY_SNIPPET = """
+from . import {0}
+__version__ = {0}.get_versions()['version']
+"""
+
+
+def do_setup():
+    """Do main VCS-independent setup function for installing Versioneer."""
+    root = get_root()
+    try:
+        cfg = get_config_from_root(root)
+    except (OSError, configparser.NoSectionError, configparser.NoOptionError) as e:
+        if isinstance(e, (OSError, configparser.NoSectionError)):
+            print("Adding sample versioneer config to setup.cfg", file=sys.stderr)
+            with open(os.path.join(root, "setup.cfg"), "a") as f:
+                f.write(SAMPLE_CONFIG)
+        print(CONFIG_ERROR, file=sys.stderr)
+        return 1
+
+    print(" creating %s" % cfg.versionfile_source)
+    with open(cfg.versionfile_source, "w") as f:
+        LONG = LONG_VERSION_PY[cfg.VCS]
+        f.write(
+            LONG
+            % {
+                "DOLLAR": "$",
+                "STYLE": cfg.style,
+                "TAG_PREFIX": cfg.tag_prefix,
+                "PARENTDIR_PREFIX": cfg.parentdir_prefix,
+                "VERSIONFILE_SOURCE": cfg.versionfile_source,
+            }
+        )
+
+    ipy = os.path.join(os.path.dirname(cfg.versionfile_source), "__init__.py")
+    if os.path.exists(ipy):
+        try:
+            with open(ipy, "r") as f:
+                old = f.read()
+        except OSError:
+            old = ""
+        module = os.path.splitext(os.path.basename(cfg.versionfile_source))[0]
+        snippet = INIT_PY_SNIPPET.format(module)
+        if OLD_SNIPPET in old:
+            print(" replacing boilerplate in %s" % ipy)
+            with open(ipy, "w") as f:
+                f.write(old.replace(OLD_SNIPPET, snippet))
+        elif snippet not in old:
+            print(" appending to %s" % ipy)
+            with open(ipy, "a") as f:
+                f.write(snippet)
+        else:
+            print(" %s unmodified" % ipy)
+    else:
+        print(" %s doesn't exist, ok" % ipy)
+        ipy = None
+
+    # Make sure both the top-level "versioneer.py" and versionfile_source
+    # (PKG/_version.py, used by runtime code) are in MANIFEST.in, so
+    # they'll be copied into source distributions. Pip won't be able to
+    # install the package without this.
+    manifest_in = os.path.join(root, "MANIFEST.in")
+    simple_includes = set()
+    try:
+        with open(manifest_in, "r") as f:
+            for line in f:
+                if line.startswith("include "):
+                    for include in line.split()[1:]:
+                        simple_includes.add(include)
+    except OSError:
+        pass
+    # That doesn't cover everything MANIFEST.in can do
+    # (http://docs.python.org/2/distutils/sourcedist.html#commands), so
+    # it might give some false negatives. Appending redundant 'include'
+    # lines is safe, though.
+    if "versioneer.py" not in simple_includes:
+        print(" appending 'versioneer.py' to MANIFEST.in")
+        with open(manifest_in, "a") as f:
+            f.write("include versioneer.py\n")
+    else:
+        print(" 'versioneer.py' already in MANIFEST.in")
+    if cfg.versionfile_source not in simple_includes:
+        print(
+            " appending versionfile_source ('%s') to MANIFEST.in"
+            % cfg.versionfile_source
+        )
+        with open(manifest_in, "a") as f:
+            f.write("include %s\n" % cfg.versionfile_source)
+    else:
+        print(" versionfile_source already in MANIFEST.in")
+
+    # Make VCS-specific changes. For git, this means creating/changing
+    # .gitattributes to mark _version.py for export-subst keyword
+    # substitution.
+    do_vcs_install(manifest_in, cfg.versionfile_source, ipy)
+    return 0
+
+
+def scan_setup_py():
+    """Validate the contents of setup.py against Versioneer's expectations."""
+    found = set()
+    setters = False
+    errors = 0
+    with open("setup.py", "r") as f:
+        for line in f.readlines():
+            if "import versioneer" in line:
+                found.add("import")
+            if "versioneer.get_cmdclass()" in line:
+                found.add("cmdclass")
+            if "versioneer.get_version()" in line:
+                found.add("get_version")
+            if "versioneer.VCS" in line:
+                setters = True
+            if "versioneer.versionfile_source" in line:
+                setters = True
+    if len(found) != 3:
+        print("")
+        print("Your setup.py appears to be missing some important items")
+        print("(but I might be wrong). Please make sure it has something")
+        print("roughly like the following:")
+        print("")
+        print(" import versioneer")
+        print(" setup( version=versioneer.get_version(),")
+        print("        cmdclass=versioneer.get_cmdclass(),  ...)")
+        print("")
+        errors += 1
+    if setters:
+        print("You should remove lines like 'versioneer.VCS = ' and")
+        print("'versioneer.versionfile_source = ' . This configuration")
+        print("now lives in setup.cfg, and should be removed from setup.py")
+        print("")
+        errors += 1
+    return errors
+
+
+if __name__ == "__main__":
+    cmd = sys.argv[1]
+    if cmd == "setup":
+        errors = do_setup()
+        errors += scan_setup_py()
+        if errors:
+            sys.exit(1)
```

