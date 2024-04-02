# Comparing `tmp/countess-0.0.54.tar.gz` & `tmp/countess-0.0.55.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "countess-0.0.54.tar", last modified: Thu Mar 28 00:28:15 2024, max compression
+gzip compressed data, was "countess-0.0.55.tar", last modified: Tue Apr  2 03:30:16 2024, max compression
```

## Comparing `countess-0.0.54.tar` & `countess-0.0.55.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-03-28 00:28:15.370469 countess-0.0.54/
--rw-rw-r--   0 nick      (1000) nick      (1000)     1470 2023-10-25 21:13:29.000000 countess-0.0.54/LICENSE.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)       59 2024-03-27 01:45:29.000000 countess-0.0.54/MANIFEST.in
--rw-r--r--   0 nick      (1000) nick      (1000)     2012 2024-03-28 00:28:15.370469 countess-0.0.54/PKG-INFO
--rw-rw-r--   0 nick      (1000) nick      (1000)      685 2024-03-28 00:26:22.000000 countess-0.0.54/README.md
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-03-28 00:28:15.362469 countess-0.0.54/countess/
--rw-rw-r--   0 nick      (1000) nick      (1000)       43 2024-03-28 00:26:22.000000 countess-0.0.54/countess/__init__.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-03-28 00:28:15.366469 countess-0.0.54/countess/core/
--rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-08-11 05:48:22.000000 countess-0.0.54/countess/core/__init__.py
--rw-rw-r--   0 nick      (1000) nick      (1000)      466 2024-03-14 22:01:54.000000 countess-0.0.54/countess/core/cmd.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     4770 2024-03-28 00:06:21.000000 countess-0.0.54/countess/core/config.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2799 2023-11-09 02:30:05.000000 countess-0.0.54/countess/core/logger.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    19950 2024-03-26 05:37:54.000000 countess-0.0.54/countess/core/parameters.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    13075 2024-03-28 00:06:21.000000 countess-0.0.54/countess/core/pipeline.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    25911 2024-03-28 00:06:21.000000 countess-0.0.54/countess/core/plugins.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-03-28 00:28:15.366469 countess-0.0.54/countess/gui/
--rw-rw-r--   0 nick      (1000) nick      (1000)        0 2023-05-25 01:44:18.000000 countess-0.0.54/countess/gui/__init__.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    18416 2024-03-28 00:06:21.000000 countess-0.0.54/countess/gui/config.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-03-28 00:28:15.366469 countess-0.0.54/countess/gui/icons/
--rw-rw-r--   0 nick      (1000) nick      (1000)       90 2024-03-27 01:45:29.000000 countess-0.0.54/countess/gui/icons/add.gif
--rw-rw-r--   0 nick      (1000) nick      (1000)       98 2024-03-27 01:45:29.000000 countess-0.0.54/countess/gui/icons/check.gif
--rw-rw-r--   0 nick      (1000) nick      (1000)       98 2024-03-27 01:45:29.000000 countess-0.0.54/countess/gui/icons/del.gif
--rw-rw-r--   0 nick      (1000) nick      (1000)       62 2024-03-28 00:06:21.000000 countess-0.0.54/countess/gui/icons/hbar.gif
--rw-rw-r--   0 nick      (1000) nick      (1000)       84 2024-03-27 01:45:29.000000 countess-0.0.54/countess/gui/icons/info.gif
--rw-rw-r--   0 nick      (1000) nick      (1000)       71 2024-03-28 00:06:21.000000 countess-0.0.54/countess/gui/icons/redbar.gif
--rw-rw-r--   0 nick      (1000) nick      (1000)       84 2024-03-28 00:06:21.000000 countess-0.0.54/countess/gui/icons/sort_dn.gif
--rw-rw-r--   0 nick      (1000) nick      (1000)       86 2024-03-28 00:06:21.000000 countess-0.0.54/countess/gui/icons/sort_un.gif
--rw-rw-r--   0 nick      (1000) nick      (1000)       88 2024-03-28 00:06:21.000000 countess-0.0.54/countess/gui/icons/sort_up.gif
--rw-rw-r--   0 nick      (1000) nick      (1000)       88 2024-03-27 01:45:29.000000 countess-0.0.54/countess/gui/icons/uncheck.gif
--rw-rw-r--   0 nick      (1000) nick      (1000)       71 2024-03-28 00:06:21.000000 countess-0.0.54/countess/gui/icons/vbar.gif
--rw-rw-r--   0 nick      (1000) nick      (1000)     5105 2024-03-18 03:56:53.000000 countess-0.0.54/countess/gui/logger.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    20283 2024-03-28 00:06:45.000000 countess-0.0.54/countess/gui/main.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     1730 2024-03-28 00:06:21.000000 countess-0.0.54/countess/gui/mini_browser.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    15369 2024-03-28 00:06:21.000000 countess-0.0.54/countess/gui/tabular.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    21302 2024-03-28 00:06:21.000000 countess-0.0.54/countess/gui/tree.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     1675 2024-03-28 00:06:21.000000 countess-0.0.54/countess/gui/widgets.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-03-28 00:28:15.370469 countess-0.0.54/countess/plugins/
--rw-rw-r--   0 nick      (1000) nick      (1000)        0 2023-05-25 01:44:18.000000 countess-0.0.54/countess/plugins/__init__.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2402 2024-03-27 23:12:11.000000 countess-0.0.54/countess/plugins/collate.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2116 2024-03-27 23:12:11.000000 countess-0.0.54/countess/plugins/column.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2245 2024-03-27 23:12:11.000000 countess-0.0.54/countess/plugins/correlation.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     7194 2024-03-28 00:06:21.000000 countess-0.0.54/countess/plugins/csv.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     3844 2024-03-27 23:12:11.000000 countess-0.0.54/countess/plugins/data_table.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     1842 2024-03-27 23:12:11.000000 countess-0.0.54/countess/plugins/expression.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2951 2024-03-15 03:51:29.000000 countess-0.0.54/countess/plugins/fastq.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     4735 2024-03-27 23:12:11.000000 countess-0.0.54/countess/plugins/group_by.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     3339 2024-03-27 23:12:11.000000 countess-0.0.54/countess/plugins/hgvs_parser.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     4541 2024-03-27 23:12:11.000000 countess-0.0.54/countess/plugins/join.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     3348 2023-11-28 03:30:23.000000 countess-0.0.54/countess/plugins/mutagenize.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     3576 2024-03-28 00:06:21.000000 countess-0.0.54/countess/plugins/pivot.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2977 2024-03-28 00:06:21.000000 countess-0.0.54/countess/plugins/python.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     6758 2024-03-27 23:12:11.000000 countess-0.0.54/countess/plugins/regex.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     1902 2024-03-27 23:12:11.000000 countess-0.0.54/countess/plugins/sequence.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     3705 2024-03-27 23:12:11.000000 countess-0.0.54/countess/plugins/variant.py
--rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-08-11 05:39:01.000000 countess-0.0.54/countess/py.typed
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-03-28 00:28:15.370469 countess-0.0.54/countess/utils/
--rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-09-26 22:30:04.000000 countess-0.0.54/countess/utils/__init__.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2768 2024-03-14 02:50:26.000000 countess-0.0.54/countess/utils/pandas.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2996 2024-03-18 21:32:56.000000 countess-0.0.54/countess/utils/parallel.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    17825 2024-03-19 05:10:25.000000 countess-0.0.54/countess/utils/variant.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-03-28 00:28:15.370469 countess-0.0.54/countess.egg-info/
--rw-r--r--   0 nick      (1000) nick      (1000)     2012 2024-03-28 00:28:15.000000 countess-0.0.54/countess.egg-info/PKG-INFO
--rw-rw-r--   0 nick      (1000) nick      (1000)     1619 2024-03-28 00:28:15.000000 countess-0.0.54/countess.egg-info/SOURCES.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)        1 2024-03-28 00:28:15.000000 countess-0.0.54/countess.egg-info/dependency_links.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)     1056 2024-03-28 00:28:15.000000 countess-0.0.54/countess.egg-info/entry_points.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)      310 2024-03-28 00:28:15.000000 countess-0.0.54/countess.egg-info/requires.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)        9 2024-03-28 00:28:15.000000 countess-0.0.54/countess.egg-info/top_level.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)     3152 2024-03-28 00:06:21.000000 countess-0.0.54/pyproject.toml
--rw-rw-r--   0 nick      (1000) nick      (1000)       38 2024-03-28 00:28:15.370469 countess-0.0.54/setup.cfg
--rw-rw-r--   0 nick      (1000) nick      (1000)       39 2023-05-25 01:44:18.000000 countess-0.0.54/setup.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-03-28 00:28:15.370469 countess-0.0.54/tests/
--rw-rw-r--   0 nick      (1000) nick      (1000)      458 2023-12-11 01:11:55.000000 countess-0.0.54/tests/test_cmd.py
--rw-rw-r--   0 nick      (1000) nick      (1000)      481 2023-11-08 23:58:38.000000 countess-0.0.54/tests/test_gui.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     1060 2023-11-09 02:44:32.000000 countess-0.0.54/tests/test_plugins.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-02 03:30:16.761914 countess-0.0.55/
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1470 2023-10-25 21:13:29.000000 countess-0.0.55/LICENSE.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)       59 2024-03-27 01:45:29.000000 countess-0.0.55/MANIFEST.in
+-rw-r--r--   0 nick      (1000) nick      (1000)     2012 2024-04-02 03:30:16.761914 countess-0.0.55/PKG-INFO
+-rw-rw-r--   0 nick      (1000) nick      (1000)      685 2024-04-02 03:29:37.000000 countess-0.0.55/README.md
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-02 03:30:16.753913 countess-0.0.55/countess/
+-rw-rw-r--   0 nick      (1000) nick      (1000)       43 2024-04-02 03:29:37.000000 countess-0.0.55/countess/__init__.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-02 03:30:16.753913 countess-0.0.55/countess/core/
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-08-11 05:48:22.000000 countess-0.0.55/countess/core/__init__.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)      466 2024-03-14 22:01:54.000000 countess-0.0.55/countess/core/cmd.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     4764 2024-04-02 01:29:15.000000 countess-0.0.55/countess/core/config.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2799 2023-11-09 02:30:05.000000 countess-0.0.55/countess/core/logger.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    19161 2024-04-02 03:04:31.000000 countess-0.0.55/countess/core/parameters.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    13908 2024-04-02 03:04:33.000000 countess-0.0.55/countess/core/pipeline.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    25925 2024-04-02 03:04:33.000000 countess-0.0.55/countess/core/plugins.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-02 03:30:16.753913 countess-0.0.55/countess/gui/
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2023-05-25 01:44:18.000000 countess-0.0.55/countess/gui/__init__.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    18436 2024-04-02 03:04:33.000000 countess-0.0.55/countess/gui/config.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-02 03:30:16.757913 countess-0.0.55/countess/gui/icons/
+-rw-rw-r--   0 nick      (1000) nick      (1000)       90 2024-03-27 01:45:29.000000 countess-0.0.55/countess/gui/icons/add.gif
+-rw-rw-r--   0 nick      (1000) nick      (1000)       98 2024-03-27 01:45:29.000000 countess-0.0.55/countess/gui/icons/check.gif
+-rw-rw-r--   0 nick      (1000) nick      (1000)       98 2024-03-27 01:45:29.000000 countess-0.0.55/countess/gui/icons/del.gif
+-rw-rw-r--   0 nick      (1000) nick      (1000)       62 2024-03-28 00:06:21.000000 countess-0.0.55/countess/gui/icons/hbar.gif
+-rw-rw-r--   0 nick      (1000) nick      (1000)       84 2024-03-27 01:45:29.000000 countess-0.0.55/countess/gui/icons/info.gif
+-rw-rw-r--   0 nick      (1000) nick      (1000)       71 2024-03-28 00:06:21.000000 countess-0.0.55/countess/gui/icons/redbar.gif
+-rw-rw-r--   0 nick      (1000) nick      (1000)       84 2024-03-28 00:06:21.000000 countess-0.0.55/countess/gui/icons/sort_dn.gif
+-rw-rw-r--   0 nick      (1000) nick      (1000)       86 2024-03-28 00:06:21.000000 countess-0.0.55/countess/gui/icons/sort_un.gif
+-rw-rw-r--   0 nick      (1000) nick      (1000)       88 2024-03-28 00:06:21.000000 countess-0.0.55/countess/gui/icons/sort_up.gif
+-rw-rw-r--   0 nick      (1000) nick      (1000)       88 2024-03-27 01:45:29.000000 countess-0.0.55/countess/gui/icons/uncheck.gif
+-rw-rw-r--   0 nick      (1000) nick      (1000)       71 2024-03-28 00:06:21.000000 countess-0.0.55/countess/gui/icons/vbar.gif
+-rw-rw-r--   0 nick      (1000) nick      (1000)     5105 2024-03-18 03:56:53.000000 countess-0.0.55/countess/gui/logger.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    20092 2024-04-02 03:04:33.000000 countess-0.0.55/countess/gui/main.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1730 2024-03-28 00:06:21.000000 countess-0.0.55/countess/gui/mini_browser.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    15129 2024-04-02 01:54:52.000000 countess-0.0.55/countess/gui/tabular.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    23070 2024-04-02 01:39:26.000000 countess-0.0.55/countess/gui/tree.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3520 2024-04-02 03:01:22.000000 countess-0.0.55/countess/gui/widgets.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-02 03:30:16.757913 countess-0.0.55/countess/plugins/
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2023-05-25 01:44:18.000000 countess-0.0.55/countess/plugins/__init__.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2402 2024-04-02 03:04:33.000000 countess-0.0.55/countess/plugins/collate.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2116 2024-04-02 03:04:33.000000 countess-0.0.55/countess/plugins/column.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2245 2024-04-02 03:04:33.000000 countess-0.0.55/countess/plugins/correlation.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     7274 2024-04-02 03:04:33.000000 countess-0.0.55/countess/plugins/csv.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3844 2024-04-02 03:04:33.000000 countess-0.0.55/countess/plugins/data_table.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1842 2024-04-02 03:04:33.000000 countess-0.0.55/countess/plugins/expression.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2938 2024-04-02 02:23:40.000000 countess-0.0.55/countess/plugins/fastq.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     4735 2024-04-02 03:04:33.000000 countess-0.0.55/countess/plugins/group_by.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3339 2024-04-02 03:04:33.000000 countess-0.0.55/countess/plugins/hgvs_parser.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     4541 2024-04-02 03:04:33.000000 countess-0.0.55/countess/plugins/join.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3348 2023-11-28 03:30:23.000000 countess-0.0.55/countess/plugins/mutagenize.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3649 2024-03-28 07:10:57.000000 countess-0.0.55/countess/plugins/pivot.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2977 2024-03-28 00:06:21.000000 countess-0.0.55/countess/plugins/python.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     6758 2024-04-02 03:04:33.000000 countess-0.0.55/countess/plugins/regex.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1902 2024-04-02 03:04:33.000000 countess-0.0.55/countess/plugins/sequence.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3705 2024-04-02 03:04:33.000000 countess-0.0.55/countess/plugins/variant.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-08-11 05:39:01.000000 countess-0.0.55/countess/py.typed
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-02 03:30:16.757913 countess-0.0.55/countess/utils/
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-09-26 22:30:04.000000 countess-0.0.55/countess/utils/__init__.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2768 2024-03-14 02:50:26.000000 countess-0.0.55/countess/utils/pandas.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2996 2024-03-18 21:32:56.000000 countess-0.0.55/countess/utils/parallel.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    17825 2024-03-19 05:10:25.000000 countess-0.0.55/countess/utils/variant.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-02 03:30:16.757913 countess-0.0.55/countess.egg-info/
+-rw-r--r--   0 nick      (1000) nick      (1000)     2012 2024-04-02 03:30:16.000000 countess-0.0.55/countess.egg-info/PKG-INFO
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1619 2024-04-02 03:30:16.000000 countess-0.0.55/countess.egg-info/SOURCES.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)        1 2024-04-02 03:30:16.000000 countess-0.0.55/countess.egg-info/dependency_links.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1056 2024-04-02 03:30:16.000000 countess-0.0.55/countess.egg-info/entry_points.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)      310 2024-04-02 03:30:16.000000 countess-0.0.55/countess.egg-info/requires.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)        9 2024-04-02 03:30:16.000000 countess-0.0.55/countess.egg-info/top_level.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3236 2024-04-01 22:33:53.000000 countess-0.0.55/pyproject.toml
+-rw-rw-r--   0 nick      (1000) nick      (1000)       38 2024-04-02 03:30:16.761914 countess-0.0.55/setup.cfg
+-rw-rw-r--   0 nick      (1000) nick      (1000)       39 2023-05-25 01:44:18.000000 countess-0.0.55/setup.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-02 03:30:16.757913 countess-0.0.55/tests/
+-rw-rw-r--   0 nick      (1000) nick      (1000)      476 2024-04-02 01:28:13.000000 countess-0.0.55/tests/test_cmd.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)      498 2024-04-02 01:28:13.000000 countess-0.0.55/tests/test_gui.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1060 2023-11-09 02:44:32.000000 countess-0.0.55/tests/test_plugins.py
```

### Comparing `countess-0.0.54/LICENSE.txt` & `countess-0.0.55/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `countess-0.0.54/PKG-INFO` & `countess-0.0.55/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: countess
-Version: 0.0.54
+Version: 0.0.55
 Summary: CountESS
 Author-email: Nick Moore <nick@zoic.org>, Alan Rubin <alan@rubin.id.au>
 Maintainer-email: Nick Moore <nick@zoic.org>
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
@@ -30,15 +30,15 @@
 Requires-Dist: pylint~=2.17; extra == "dev"
 Requires-Dist: types-psutil~=5.9.5; extra == "dev"
 Requires-Dist: types-ttkthemes~=3.2; extra == "dev"
 Requires-Dist: twine==4.0.2; extra == "dev"
 Requires-Dist: pandas-stubs~=2.1.0; extra == "dev"
 Requires-Dist: pytest~=7.2; extra == "dev"
 
-# CountESS 0.0.54
+# CountESS 0.0.55
 
 This is CountESS, a modular, Python 3 reimplementation of Enrich2.
 
 ## License
 
 BSD 3-clause.  See [LICENSE.txt](LICENSE.txt)
```

### Comparing `countess-0.0.54/README.md` & `countess-0.0.55/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# CountESS 0.0.54
+# CountESS 0.0.55
 
 This is CountESS, a modular, Python 3 reimplementation of Enrich2.
 
 ## License
 
 BSD 3-clause.  See [LICENSE.txt](LICENSE.txt)
```

### Comparing `countess-0.0.54/countess/core/config.py` & `countess-0.0.55/countess/core/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import ast
+import io
 import os.path
 import re
 import sys
 from configparser import ConfigParser
 
 from countess.core.logger import ConsoleLogger, Logger
 from countess.core.pipeline import PipelineGraph, PipelineNode
@@ -13,14 +14,53 @@
     print(f"{n:40s} {a:4d}/{b:4d} {s}")
 
 
 def default_output_callback(output):
     sys.stderr.write(repr(output))
 
 
+def read_config_dict(name: str, base_dir: str, config_dict: dict) -> PipelineNode:
+    if "_module" in config_dict:
+        module_name = config_dict["_module"]
+        class_name = config_dict["_class"]
+        # XXX version = config_dict.get("_version")
+        # XXX hash_digest = config_dict.get("_hash")
+        plugin = load_plugin(module_name, class_name)
+    else:
+        plugin = None
+
+    position_str = config_dict.get("_position")
+    notes = config_dict.get("_notes")
+
+    position = None
+    if position_str:
+        position_match = re.match(r"(\d+) (\d+)$", position_str)
+        if position_match:
+            position = (
+                int(position_match.group(1)) / 1000,
+                int(position_match.group(2)) / 1000,
+            )
+
+    sort = config_dict.get("_sort", "0 0").split()
+
+    # XXX check version and hash_digest and emit warnings.
+
+    config = [(key, ast.literal_eval(val), base_dir) for key, val in config_dict.items() if not key.startswith("_")]
+
+    return PipelineNode(
+        name=name,
+        plugin=plugin,
+        config=config,
+        position=position,
+        notes=notes,
+        sort_column=int(sort[0]),
+        sort_descending=bool(int(sort[1])),
+    )
+
+
 def read_config(
     filename: str,
     logger: Logger = ConsoleLogger(),
 ) -> PipelineGraph:
     """Reads `filenames` and returns a PipelineGraph"""
 
     cp = ConfigParser()
@@ -28,108 +68,77 @@
 
     base_dir = os.path.dirname(filename)
 
     pipeline_graph = PipelineGraph()
     nodes_by_name: dict[str, PipelineNode] = {}
 
     for section_name in cp.sections():
-        config_dict = cp[section_name]
-
-        if "_module" in config_dict:
-            module_name = config_dict["_module"]
-            class_name = config_dict["_class"]
-            # XXX version = config_dict.get("_version")
-            # XXX hash_digest = config_dict.get("_hash")
-            plugin = load_plugin(module_name, class_name)
-        else:
-            plugin = None
-
-        position_str = config_dict.get("_position")
-        notes = config_dict.get("_notes")
-
-        position = None
-        if position_str:
-            position_match = re.match(r"(\d+) (\d+)$", position_str)
-            if position_match:
-                position = (
-                    int(position_match.group(1)) / 1000,
-                    int(position_match.group(2)) / 1000,
-                )
-
-        sort = config_dict.get("_sort", "0 0").split()
-
-        # XXX check version and hash_digest and emit warnings.
-
-        config = [(key, ast.literal_eval(val), base_dir) for key, val in config_dict.items() if not key.startswith("_")]
-
-        node = PipelineNode(
-            name=section_name,
-            plugin=plugin,
-            config=config,
-            position=position,
-            notes=notes,
-            sort_column=int(sort[0]),
-            sort_descending=bool(int(sort[1])),
-        )
-        pipeline_graph.nodes.append(node)
+        config_dict = dict(cp[section_name])
+        node = read_config_dict(section_name, base_dir, config_dict)
 
         for key, val in config_dict.items():
             if key.startswith("_parent."):
                 node.add_parent(nodes_by_name[val])
 
+        pipeline_graph.nodes.append(node)
         nodes_by_name[section_name] = node
 
     return pipeline_graph
 
 
 def write_config(pipeline_graph: PipelineGraph, filename: str):
     """Write `pipeline_graph`'s configuration out to `filename`"""
 
+    pipeline_graph.reset_node_names()
+
     cp = ConfigParser()
     base_dir = os.path.dirname(filename)
 
-    node_names_seen = set()
     for node in pipeline_graph.traverse_nodes():
-        while node.name in node_names_seen:
-            num = 0
-            if match := re.match(r"(.*?)\s+(\d+)$", node.name):
-                node.name = match.group(1)
-                num = int(match.group(2))
-            node.name += f" {num + 1}"
-        node_names_seen.add(node.name)
-
-        cp.add_section(node.name)
-        if node.plugin:
-            cp[node.name].update(
-                {
-                    "_module": node.plugin.__module__,
-                    "_class": node.plugin.__class__.__name__,
-                    "_version": node.plugin.version,
-                    "_hash": node.plugin.hash(),
-                    "_sort": "%d %d" % (node.sort_column, 1 if node.sort_descending else 0),
-                }
-            )
-        if node.position:
-            xx, yy = node.position
-            cp[node.name]["_position"] = "%d %d" % (xx * 1000, yy * 1000)
-        if node.notes:
-            cp[node.name]["_notes"] = node.notes
-        for n, parent in enumerate(node.parent_nodes):
-            cp[node.name][f"_parent.{n}"] = parent.name
-        if node.config:
-            for k, v, _ in node.config:
-                cp[node.name][k] = repr(v)
-        elif node.plugin:
-            for k, v in node.plugin.get_parameters(base_dir):
-                cp[node.name][k] = repr(v)
+        write_config_node(node, cp, base_dir)
 
     with open(filename, "w", encoding="utf-8") as fh:
         cp.write(fh)
 
 
+def write_config_node_string(node: PipelineNode, base_dir: str = ""):
+    cp = ConfigParser()
+    write_config_node(node, cp, base_dir)
+    buf = io.StringIO()
+    cp.write(buf)
+    return buf.getvalue()
+
+
+def write_config_node(node: PipelineNode, cp: ConfigParser, base_dir: str):
+    cp.add_section(node.name)
+    if node.plugin:
+        cp[node.name].update(
+            {
+                "_module": node.plugin.__module__,
+                "_class": node.plugin.__class__.__name__,
+                "_version": node.plugin.version,
+                "_hash": node.plugin.hash(),
+                "_sort": "%d %d" % (node.sort_column, 1 if node.sort_descending else 0),
+            }
+        )
+    if node.position:
+        xx, yy = node.position
+        cp[node.name]["_position"] = "%d %d" % (xx * 1000, yy * 1000)
+    if node.notes:
+        cp[node.name]["_notes"] = node.notes
+    for n, parent in enumerate(node.parent_nodes):
+        cp[node.name][f"_parent.{n}"] = parent.name
+    if node.config:
+        for k, v, _ in node.config:
+            cp[node.name][k] = repr(v)
+    elif node.plugin:
+        for k, v in node.plugin.get_parameters(base_dir):
+            cp[node.name][k] = repr(v)
+
+
 def export_config_graphviz(pipeline_graph: PipelineGraph, filename: str):
     with open(filename, "w", encoding="utf-8") as fh:
         fh.write("digraph {\n")
         for node in pipeline_graph.traverse_nodes():
             label = node.name.replace('"', r"\"")
             if node.child_nodes and not node.parent_nodes:
                 fh.write(f'\t"{label}" [ shape="invhouse" ];\n')
```

### Comparing `countess-0.0.54/countess/core/logger.py` & `countess-0.0.55/countess/core/logger.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.54/countess/core/parameters.py` & `countess-0.0.55/countess/core/parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,49 +154,26 @@
         x = "".join([self.clean_character(c) for c in value_str])
         return x
 
     def copy(self) -> "StringCharacterSetParam":
         return self.__class__(self.label, self.value, self.read_only, character_set=self.character_set)
 
 
-def clean_file_types(file_types):
-    # MacOS in particular is crashy if file_types is not to it's liking.
-    # This leads to very confusing errors.  Better to throw an assertion
-    # error here than bomb out later.  See #27.
-
-    # XXX MacOS also doesn't seem to handle multiple file
-    # extensions, eg: .csv.gz, whereas Linux can.
-    # So maybe this function could accept those and censor
-    # them if running MacOS.
-
-    assert type(file_types) is list
-    for ft in file_types:
-        assert type(ft) in (tuple, list)
-        assert type(ft[0]) is str
-        assert type(ft[1]) in (tuple, list, str)
-        if type(ft[1]) in (tuple, list):
-            for ext in ft[1]:
-                assert type(ext) is str
-                assert ext == "*" or ext == "" or re.match(r"\.\w+$", ext), f"Invalid FileType Extension {ext}"
-
-    return file_types
-
-
 class FileParam(StringParam):
     """A StringParam for holding a filename.  Defaults to `read_only` because
     it really should be populated from a file dialog or simiar."""
 
     file_types = [("Any", "*")]
 
     _hash = None
 
     def __init__(self, label: str, value=None, read_only: bool = True, file_types=None):
         super().__init__(label, value, read_only)
         if file_types is not None:
-            self.file_types = clean_file_types(file_types)
+            self.file_types = file_types
 
     def get_file_hash(self):
         if not self.value:
             return "0"
         try:
             with open(self.value, "rb") as file:
                 try:
@@ -211,19 +188,22 @@
                         digest.update(data)
             return digest.hexdigest()
         except IOError:
             return "0"
 
     def get_parameters(self, key, base_dir="."):
         if self.value:
-            relpath = os.path.relpath(self.value, base_dir)
+            if base_dir:
+                path = os.path.relpath(self.value, base_dir)
+            else:
+                path = os.path.abspath(self.value)
         else:
-            relpath = None
+            path = None
 
-        return [(key, relpath)]
+        return [(key, path)]
 
     def copy(self) -> "FileParam":
         return self.__class__(self.label, self.value, self.read_only, file_types=self.file_types)
 
     def get_hash_value(self) -> str:
         # For reproducability, we don't actually care about the filename, just
         # its hash.
```

### Comparing `countess-0.0.54/countess/core/pipeline.py` & `countess-0.0.55/countess/core/pipeline.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import re
 import time
 from queue import Empty, Queue
 from threading import Thread
 from typing import Any, Optional
 
 from countess.core.logger import Logger
 from countess.core.plugins import BasePlugin, FileInputPlugin, ProcessPlugin, get_plugin_classes
@@ -251,15 +252,25 @@
 
 
 class PipelineGraph:
     def __init__(self):
         self.plugin_classes = get_plugin_classes()
         self.nodes = []
 
+    def reset_node_name(self, node):
+        node_names_seen = set(n.name for n in self.nodes if n != node)
+        while node.name in node_names_seen:
+            num = 1
+            if match := re.match(r"(.*?)\s+(\d+)$", node.name):
+                node.name = match.group(1)
+                num = int(match.group(2))
+            node.name += f" {num + 1}"
+
     def add_node(self, node):
+        self.reset_node_name(node)
         self.nodes.append(node)
 
     def del_node(self, node):
         node.detatch()
         self.nodes.remove(node)
 
     def traverse_nodes(self):
@@ -301,14 +312,25 @@
             time.sleep(10)
 
     def reset(self):
         for node in self.nodes:
             node.result = None
             node.is_dirty = True
 
+    def reset_node_names(self):
+        node_names_seen = set()
+        for node in self.traverse_nodes():
+            while node.name in node_names_seen:
+                num = 0
+                if match := re.match(r"(.*?)\s+(\d+)$", node.name):
+                    node.name = match.group(1)
+                    num = int(match.group(2))
+                node.name += f" {num + 1}"
+            node_names_seen.add(node.name)
+
     def tidy(self):
         """Tidies the graph (sets all the node positions)"""
 
         # XXX This is very arbitrary and not particularly efficient.
         # Some kind of FDP-like algorithm might be nice.
         # Especially if it could include node/line collisions.
         # See #24
```

### Comparing `countess-0.0.54/countess/core/plugins.py` & `countess-0.0.55/countess/core/plugins.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 import hashlib
 import importlib
 import importlib.metadata
 import logging
 import os.path
 from collections.abc import MutableMapping
-from typing import Dict, Iterable, List, Optional, Union
+from typing import Dict, Iterable, List, Optional, Sequence, Union
 
 import numpy as np
 import pandas as pd
 
 from countess.core.logger import Logger
 from countess.core.parameters import (
     ArrayParam,
@@ -183,15 +183,15 @@
 
     file_number = 0
     name = ""
     row_limit = None
     num_inputs = 0
 
     # used by the GUI file dialog
-    file_types: List[tuple[str, Union[str, list[str]]]] = [("Any", "*")]
+    file_types: Sequence[tuple[str, Union[str, list[str]]]] = [("Any", "*")]
     file_params: MutableMapping[str, BaseParam] = {}
 
     def num_files(self) -> int:
         """return the number of 'files' which are to be loaded.  The pipeline
         will call code equivalent to
         `[ p.load_file(n, logger, row_limit) for n in range(0, p.num_files() ]`
         although potentially using threads, multiprocessing, etc."""
```

### Comparing `countess-0.0.54/countess/gui/config.py` & `countess-0.0.55/countess/gui/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # TK based GUI for CountESS
 import math
 import tkinter as tk
 from functools import partial
-from tkinter import filedialog, ttk
+from tkinter import ttk
 from typing import Mapping, MutableMapping, Optional
 
 import numpy as np
 
 from ..core.parameters import (
     ArrayParam,
     BaseParam,
@@ -18,15 +18,22 @@
     FileSaveParam,
     MultiParam,
     SimpleParam,
     TabularMultiParam,
     TextParam,
 )
 from ..core.plugins import BasePlugin
-from .widgets import BooleanCheckbox, add_button, delete_button
+from .widgets import (
+    BooleanCheckbox,
+    add_button,
+    ask_open_filename,
+    ask_open_filenames,
+    ask_saveas_filename,
+    delete_button,
+)
 
 
 def is_nan(v):
     return v is None or v is np.nan or (isinstance(v, float) and math.isnan(v))
 
 
 class ParameterWrapper:
@@ -315,19 +322,19 @@
             self.entry.grid(row=row, column=2)
 
     def add_row_callback(self, *_):
         assert isinstance(self.parameter, ArrayParam)
 
         if isinstance(self.parameter, FileSaveParam):
             file_types = self.parameter.file_types
-            filename = filedialog.asksaveasfilename(filetypes=file_types)
+            filename = ask_saveas_filename(file_types)
             self.parameter.value = filename
         if isinstance(self.parameter, FileArrayParam):
             file_types = self.parameter.file_types
-            filenames = filedialog.askopenfilenames(filetypes=file_types)
+            filenames = ask_open_filenames(file_types)
             self.parameter.add_files(filenames)
         else:
             self.parameter.add_row()
 
         if self.callback is not None:
             self.callback(self.parameter)
 
@@ -343,15 +350,15 @@
 
         self.update()
         if self.callback is not None:
             self.callback(self.parameter)
 
     def change_file_callback(self, *_):
         file_types = self.parameter.file_types
-        filename = filedialog.askopenfilename(filetypes=file_types)
+        filename = ask_open_filename(file_types)
         self.parameter.value = filename
         self.entry["text"] = self.parameter.value
         self.callback(self.parameter)
 
     def set_value(self, value):
         # self.parameter.value is a property, and some cleaning may occur, so we just
         # check before and after to see if it has changed.
```

### Comparing `countess-0.0.54/countess/gui/logger.py` & `countess-0.0.55/countess/gui/logger.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.54/countess/gui/main.py` & `countess-0.0.55/countess/gui/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -264,17 +264,14 @@
     #            self.logger_subframe.progress_hide()
 
     def choose_plugin(self, plugin_class):
         self.node.plugin = plugin_class()
         self.node.prerun(self.logger)
         self.node.is_dirty = True
         self.show_config_subframe()
-        if self.node.name.startswith("NEW "):
-            self.node.name = self.node.plugin.name + self.node.name.removeprefix("NEW")
-            self.name_var.set(self.node.name)
         self.change_callback(self.node)
 
     def destroy(self):
         if self.config_change_task:
             self.frame.after_cancel(self.config_change_task)
         if self.config_subframe:
             self.config_subframe.destroy()
@@ -415,15 +412,15 @@
                 return
         self.config_changed = False
         self.config_filename = None
         if self.graph_wrapper:
             self.graph_wrapper.destroy()
         self.graph = PipelineGraph()
         self.graph_wrapper = GraphWrapper(self.canvas, self.graph, self.node_select)
-        self.graph_wrapper.add_new_node(select=True)
+        self.graph_wrapper.add_new_node()
 
     def config_load(self, filename=None):
         if not filename:
             filename = filedialog.askopenfilename(filetypes=[(".INI Config File", "*.ini")])
         if not filename:
             return
         self.config_filename = filename
```

### Comparing `countess-0.0.54/countess/gui/mini_browser.py` & `countess-0.0.55/countess/gui/mini_browser.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.54/countess/gui/tabular.py` & `countess-0.0.55/countess/gui/tabular.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from math import ceil, floor, isinf, isnan
 from tkinter import ttk
 from typing import Callable, Optional, Union
 
 import pandas as pd
 from pandas.api.types import is_integer_dtype, is_numeric_dtype
 
-from countess.gui.widgets import get_icon
+from countess.gui.widgets import copy_to_clipboard, get_icon
 
 # XXX columns should automatically resize based on information
 # from _column_xscrollcommand which can tell if they're
 # overflowing.  Or maybe use
 #    df['seq'].str.len().max() to get max length of a string column
 # etc etc.
 
@@ -55,14 +55,15 @@
         return "—"
     if value is True:
         return "—T"
     if value is False:
         return "—F"
 
     # remove trailing 0's from floats (%g doesn't align correctly)
+    #     100.0 => "100.000000000000" => "100."
     try:
         if column_format.endswith("f"):
             return (column_format % value).rstrip("0")
         else:
             return column_format % value
     except TypeError:
         return str(value)
@@ -361,22 +362,15 @@
 
     def _column_copy(self, _):
         # If this was a multi-row selection, then replace
         # the copy buffer with a copy of those whole rows.
         if not self.select_rows:
             return  # not multi-row, keep it.
 
+        # Dump TSV into a StringIO ...
         r1, r2 = self.select_rows
         df = self.dataframe.iloc[self.offset + r1 - 1 : self.offset + r2]
         buf = io.StringIO()
         df.to_csv(buf, sep="\t")
 
-        # XXX very cheesy, but self.clipboard_append() etc didn't
-        # seem to work, so this is a terrible workaround ... dump the
-        # TSV into a new tk.Text, select the whole thing and copy it
-        # into the clipboard.
-        top = tk.Toplevel()
-        text = tk.Text(top)
-        text.insert(tk.END, buf.getvalue())
-        text.tag_add("sel", "1.0", tk.END)
-        text.event_generate("<<Copy>>")
-        top.destroy()
+        # ... and then push that onto the clipboard
+        copy_to_clipboard(buf.getvalue())
```

### Comparing `countess-0.0.54/countess/gui/tree.py` & `countess-0.0.55/countess/gui/tree.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,19 +5,21 @@
 # https://github.com/CountESS-Project/CountESS/issues/19
 # for more discussion etc.
 
 import math
 import random
 import re
 import tkinter as tk
+from configparser import ConfigParser
 from enum import Enum, IntFlag
 from functools import partial
 
+from countess.core.config import read_config_dict, write_config_node_string
 from countess.core.pipeline import PipelineNode
-from countess.gui.widgets import get_icon
+from countess.gui.widgets import copy_to_clipboard, get_icon
 
 
 def _limit(value, min_value, max_value):
     return max(min_value, min(max_value, value))
 
 
 def _geometry(widget):
@@ -291,14 +293,15 @@
         self.canvas.bind("<Button-1>", self.on_canvas_button)
         self.canvas.bind("<Button-2>", self.on_canvas_button)
         self.canvas.bind("<Button-3>", self.on_canvas_button)
         self.canvas.bind("<Motion>", self.on_canvas_motion)
         self.canvas.bind("<Leave>", self.on_canvas_leave)
         self.canvas.bind("<Key-Delete>", self.on_canvas_delete)
         self.canvas.bind("<Key-BackSpace>", self.on_canvas_delete)
+        self.canvas.bind("<<Paste>>", self.on_paste)
 
     def label_for_node(self, node):
         label = NodeWrapper(self.canvas, wraplength=125, cursor="hand1", takefocus=True)
         if not node.position:
             node.position = (random.random() * 0.8 + 0.1, random.random() * 0.8 + 0.1)
         # XXX should be more elegant way of answering the question "are we flipped?"
         if self.canvas.winfo_width() >= self.canvas.winfo_height():
@@ -309,14 +312,16 @@
         label.bind("<Button-1>", partial(self.on_mousedown, node), add=True)
         label.bind("<Configure>", partial(self.on_configure, node, label), add=True)
         label.bind("<<GhostRelease>>", partial(self.on_ghost_release, node), add=True)
         label.bind("<Key-Delete>", partial(self.on_delete, node), add=True)
         label.bind("<Key-BackSpace>", partial(self.on_delete, node), add=True)
         label.bind("<Enter>", partial(self.on_enter, node), add=True)
         label.bind("<Leave>", partial(self.on_leave, node), add=True)
+        label.bind("<<Copy>>", partial(self.on_copy, node), add=True)
+        label.bind("<<Cut>>", partial(self.on_cut, node), add=True)
 
         return label
 
     def lines_for_node(self, node):
         return dict(
             (
                 parent_node,
@@ -377,14 +382,41 @@
 
     def on_leave(self, node, event):
         if self.highlight_rectangle is not None:
             self.canvas.delete(self.highlight_rectangle)
             self.highlight_rectangle = None
         self.canvas.focus_set()
 
+    def on_copy(self, node, event):
+        # Copy the selected node's config to the clipboard
+        copy_to_clipboard(write_config_node_string(node))
+
+    def on_cut(self, node, event):
+        self.on_copy(node, event)
+        self.on_delete(node, event)
+
+    def on_paste(self, event):
+        # Try and interpret whatever is in the clipboard as a config
+        # file section and create it as a node!  This lets users
+        # cut and paste between CountESS instances!
+        cp = ConfigParser()
+        cp.read_string(self.canvas.clipboard_get())
+
+        for section_name in cp.sections():
+            config_dict = cp[section_name]
+            node = read_config_dict(section_name, "", config_dict)
+            node.position = self.new_node_position(event.x, event.y)
+            self.add_node(node)
+
+            # try and reconnect parents if they exist
+            nodes_by_name = {n.name: n for n in self.graph.nodes}
+            for key, val in config_dict.items():
+                if key.startswith("_parent.") and val in nodes_by_name:
+                    self.add_parent(nodes_by_name[val], node)
+
     def on_canvas_motion(self, event):
         """Show a preview of line selection when the cursor is over line(s)"""
         items = self.canvas.find_overlapping(event.x - 10, event.y - 10, event.x + 10, event.y + 10)
         for connecting_line, _, _ in self.lines_lookup.values():
             color = "red" if connecting_line.line in items else "black"
             self.canvas.itemconfig(connecting_line.line, fill=color)
 
@@ -414,22 +446,25 @@
         # (you can still create a new node by button-3-dragging from an
         # existing node, and if you really want a disconnected graph you can
         # delete the link to the new node!)
         # if not items:
         #    return
 
         position = self.new_node_position(event.x, event.y)
-        new_node = self.add_new_node(position)
+        new_node = self.add_new_node(position, select=False)
 
         for item in items:
             _, child_node, parent_node = self.lines_lookup[item]
             self.del_parent(parent_node, child_node)
             self.add_parent(new_node, child_node)
             self.add_parent(parent_node, new_node)
 
+        self.highlight_node(new_node)
+        self.node_select_callback(new_node)
+
     def on_canvas_delete(self, event):
         """Delete key on canvas: delete line(s)."""
         items = self.canvas.find_overlapping(event.x - 10, event.y - 10, event.x + 10, event.y + 10)
         for item in items:
             _, child_node, parent_node = self.lines_lookup[item]
             self.del_parent(parent_node, child_node)
 
@@ -456,46 +491,49 @@
         if not event.state & TkEventState.CONTROL:
             self.graph.nodes.remove(node)
             del self.labels[node]
             del self.lines[node]
             event.widget.destroy()
 
         if len(self.graph.nodes) == 0:
-            self.add_new_node(select=True)
+            new_node = self.add_new_node(select=True)
         elif node == self.selected_node:
             # arbitrarily pick another node to show
             new_node = parent_nodes[0] if parent_nodes else child_nodes[0] if child_nodes else list(self.graph.nodes)[0]
             self.highlight_node(new_node)
             self.node_select_callback(new_node)
 
     def find_node_at_position(self, x, y):
         for node, label in self.labels.items():
             nx, ny, nw, nh = _geometry(label)
             if (nx <= x <= nx + nw) and (ny <= y <= ny + nh):
                 return node
         return None
 
-    def add_new_node(self, position=(0.5, 0.5), select=True):
-        new_node = PipelineNode(name=f"NEW {len(self.graph.nodes)+1}", position=position)
+    def add_node(self, new_node, select: bool = True):
         self.graph.add_node(new_node)
         self.labels[new_node] = self.label_for_node(new_node)
         self.labels[new_node].update()
         self.lines[new_node] = {}
         if select:
             self.highlight_node(new_node)
             self.node_select_callback(new_node)
+
+    def add_new_node(self, position=(0.5, 0.5), select: bool = True):
+        new_node = PipelineNode(name="NEW", position=position)
+        self.add_node(new_node, select)
         return new_node
 
     def on_ghost_release(self, start_node, event):
         xl, yl, _wl, _hl = _geometry(event.widget)
         flipped = self.canvas.winfo_height() > self.canvas.winfo_width()
         other_node = self.find_node_at_position(event.x + xl, event.y + yl)
         if other_node is None:
             position = self.new_node_position(event.x + xl, event.y + yl)
-            other_node = self.add_new_node(position)
+            other_node = self.add_new_node(position, select=False)
         elif other_node == start_node:
             return
         elif start_node in other_node.parent_nodes:
             other_node.del_parent(start_node)
             return
         elif other_node in start_node.parent_nodes:
             start_node.del_parent(other_node)
@@ -534,14 +572,19 @@
         connecting_line.destroy()
         child_node.del_parent(parent_node)
 
     def node_changed(self, node):
         """Called when something external updates the node's name, status
         or configuration."""
         flipped = self.canvas.winfo_width() >= self.canvas.winfo_height()
+
+        if node.name.startswith("NEW"):
+            node.name = node.plugin.name
+            self.graph.reset_node_name(node)
+
         self.labels[node].update_node(node, not flipped)
 
     def destroy(self):
         for node_lines in self.lines.values():
             for line in node_lines.values():
                 line.destroy()
         for label in self.labels.values():
```

### Comparing `countess-0.0.54/countess/plugins/collate.py` & `countess-0.0.55/countess/plugins/collate.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.54/countess/plugins/column.py` & `countess-0.0.55/countess/plugins/column.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.54/countess/plugins/correlation.py` & `countess-0.0.55/countess/plugins/correlation.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.54/countess/plugins/csv.py` & `countess-0.0.55/countess/plugins/csv.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import csv
 import gzip
 from io import BufferedWriter, BytesIO
-from typing import Optional, Union
+from typing import List, Optional, Sequence, Tuple, Union
 
 import pandas as pd
 
 from countess import VERSION
 from countess.core.logger import Logger
 from countess.core.parameters import (
     ArrayParam,
@@ -15,24 +15,29 @@
     FileSaveParam,
     MultiParam,
     StringParam,
 )
 from countess.core.plugins import PandasInputFilesPlugin, PandasOutputPlugin
 from countess.utils.pandas import flatten_columns
 
+CSV_FILE_TYPES: Sequence[Tuple[str, Union[str, List[str]]]] = [
+    ("CSV", [".csv", ".csv.gz"]),
+    ("TSV", [".tsv", ".tsv.gz"]),
+    ("TXT", [".txt", ".txt.gz"]),
+]
+
 
 class LoadCsvPlugin(PandasInputFilesPlugin):
     """Load CSV files"""
 
     name = "CSV Load"
     description = "Loads data from CSV or similar delimited text files and assigns types to columns"
     link = "https://countess-project.github.io/CountESS/included-plugins/#csv-reader"
     version = VERSION
-
-    file_types = [("CSV", [".csv", ".gz"]), ("TSV", [".tsv", ".gz"]), ("TXT", ".txt")]
+    file_types = CSV_FILE_TYPES
 
     parameters = {
         "delimiter": ChoiceParam("Delimiter", ",", choices=[",", ";", "TAB", "|", "WHITESPACE"]),
         "quoting": ChoiceParam("Quoting", "None", choices=["None", "Double-Quote", "Quote with Escape"]),
         "comment": ChoiceParam("Comment", "None", choices=["None", "#", ";"]),
         "header": BooleanParam("CSV file has header row?", True),
         "filename_column": StringParam("Filename Column", ""),
@@ -120,16 +125,15 @@
 
 
 class SaveCsvPlugin(PandasOutputPlugin):
     name = "CSV Save"
     description = "Save data as CSV or similar delimited text files"
     link = "https://countess-project.github.io/CountESS/included-plugins/#csv-writer"
     version = VERSION
-
-    file_types = [("CSV", [".csv", ".gz"]), ("TSV", [".tsv", ".gz"]), ("TXT", ".txt")]
+    file_types = CSV_FILE_TYPES
 
     parameters = {
         "header": BooleanParam("CSV header row?", True),
         "filename": FileSaveParam("Filename", file_types=file_types),
         "delimiter": ChoiceParam("Delimiter", ",", choices=[",", ";", "TAB", "|", "SPACE"]),
         "quoting": BooleanParam("Quote all Strings", False),
     }
```

### Comparing `countess-0.0.54/countess/plugins/data_table.py` & `countess-0.0.55/countess/plugins/data_table.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.54/countess/plugins/expression.py` & `countess-0.0.55/countess/plugins/expression.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.54/countess/plugins/fastq.py` & `countess-0.0.55/countess/plugins/fastq.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     in multiple columns."""
 
     name = "FASTQ Load"
     description = "Loads counts from FASTQ files containing either variant or barcodes"
     link = "https://countess-project.github.io/CountESS/included-plugins/#fastq-load"
     version = VERSION
 
-    file_types = [("FASTQ", ".fastq"), ("FASTQ (gzipped)", ".gz")]
+    file_types = [("FASTQ", [".fastq", ".fastq.gz"])]
 
     parameters = {
         "min_avg_quality": FloatParam("Minimum Average Quality", 10),
         "header_column": BooleanParam("Header Column?", False),
         "filename_column": BooleanParam("Filename Column?", False),
         "group": BooleanParam("Group by Sequence?", True),
     }
```

### Comparing `countess-0.0.54/countess/plugins/group_by.py` & `countess-0.0.55/countess/plugins/group_by.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.54/countess/plugins/hgvs_parser.py` & `countess-0.0.55/countess/plugins/hgvs_parser.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.54/countess/plugins/join.py` & `countess-0.0.55/countess/plugins/join.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.54/countess/plugins/mutagenize.py` & `countess-0.0.55/countess/plugins/mutagenize.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.54/countess/plugins/pivot.py` & `countess-0.0.55/countess/plugins/pivot.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,16 @@
     def prepare(self, sources: List[str], row_limit: Optional[int] = None):
         self.input_columns = {}
 
     def process(self, data: pd.DataFrame, source: str, logger: Logger):
         assert isinstance(self.parameters["columns"], PerColumnArrayParam)
         self.input_columns.update(get_all_columns(data))
 
+        data.reset_index(drop=data.index.names == [None], inplace=True)
+
         column_parameters = list(zip(self.input_columns, self.parameters["columns"]))
         index_cols = [col for col, param in column_parameters if param.value == "Index"]
         pivot_cols = [col for col, param in column_parameters if param.value == "Pivot"]
         expand_cols = [col for col, param in column_parameters if param.value == "Expand"]
 
         if not index_cols:
             logger.warning("No columns to index!")
```

### Comparing `countess-0.0.54/countess/plugins/python.py` & `countess-0.0.55/countess/plugins/python.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.54/countess/plugins/regex.py` & `countess-0.0.55/countess/plugins/regex.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.54/countess/plugins/sequence.py` & `countess-0.0.55/countess/plugins/sequence.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.54/countess/plugins/variant.py` & `countess-0.0.55/countess/plugins/variant.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.54/countess/utils/pandas.py` & `countess-0.0.55/countess/utils/pandas.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.54/countess/utils/parallel.py` & `countess-0.0.55/countess/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.54/countess/utils/variant.py` & `countess-0.0.55/countess/utils/variant.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.54/countess.egg-info/PKG-INFO` & `countess-0.0.55/countess.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: countess
-Version: 0.0.54
+Version: 0.0.55
 Summary: CountESS
 Author-email: Nick Moore <nick@zoic.org>, Alan Rubin <alan@rubin.id.au>
 Maintainer-email: Nick Moore <nick@zoic.org>
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
@@ -30,15 +30,15 @@
 Requires-Dist: pylint~=2.17; extra == "dev"
 Requires-Dist: types-psutil~=5.9.5; extra == "dev"
 Requires-Dist: types-ttkthemes~=3.2; extra == "dev"
 Requires-Dist: twine==4.0.2; extra == "dev"
 Requires-Dist: pandas-stubs~=2.1.0; extra == "dev"
 Requires-Dist: pytest~=7.2; extra == "dev"
 
-# CountESS 0.0.54
+# CountESS 0.0.55
 
 This is CountESS, a modular, Python 3 reimplementation of Enrich2.
 
 ## License
 
 BSD 3-clause.  See [LICENSE.txt](LICENSE.txt)
```

### Comparing `countess-0.0.54/countess.egg-info/SOURCES.txt` & `countess-0.0.55/countess.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `countess-0.0.54/countess.egg-info/entry_points.txt` & `countess-0.0.55/countess.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `countess-0.0.54/pyproject.toml` & `countess-0.0.55/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -107,7 +107,11 @@
     "too-many-public-methods",
     "unidiomatic-typecheck",
 ]
 max-line-length = 120
 
 [tool.black]
 line-length = 120
+
+[tool.pytest.ini_options]
+addopts = "--strict-markers"
+markers = [ "slow", "gui" ]
```

### Comparing `countess-0.0.54/tests/test_plugins.py` & `countess-0.0.55/tests/test_plugins.py`

 * *Files identical despite different names*

