# Comparing `tmp/dbdreader-0.5.6.tar.gz` & `tmp/dbdreader-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbdreader-0.5.6.tar", last modified: Mon Jan 15 12:37:08 2024, max compression
+gzip compressed data, was "dbdreader-0.5.7.tar", last modified: Thu Mar 28 08:13:48 2024, max compression
```

## Comparing `dbdreader-0.5.6.tar` & `dbdreader-0.5.7.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 lucas     (1001) kdt       (1030)        0 2024-01-15 12:37:08.096608 dbdreader-0.5.6/
--rw-r--r--   0 lucas     (1001) kdt       (1030)    18009 2024-01-05 10:26:07.000000 dbdreader-0.5.6/COPYING
--rw-r--r--   0 lucas     (1001) kdt       (1030)      704 2024-01-05 10:26:07.000000 dbdreader-0.5.6/COPYRIGHT
--rw-r--r--   0 lucas     (1001) kdt       (1030)      545 2024-01-05 10:26:07.000000 dbdreader-0.5.6/INSTALL.rst
--rw-r--r--   0 lucas     (1001) kdt       (1030)    35147 2024-01-05 10:26:07.000000 dbdreader-0.5.6/LICENSE
--rw-r--r--   0 lucas     (1001) kdt       (1030)      346 2024-01-15 09:42:37.000000 dbdreader-0.5.6/MANIFEST.in
--rw-r--r--   0 lucas     (1001) kdt       (1030)     8748 2024-01-15 12:37:08.096608 dbdreader-0.5.6/PKG-INFO
--rw-r--r--   0 lucas     (1001) kdt       (1030)     8181 2024-01-05 14:30:08.000000 dbdreader-0.5.6/README.rst
-drwxr-xr-x   0 lucas     (1001) kdt       (1030)        0 2024-01-15 12:37:08.087608 dbdreader-0.5.6/dbdreader/
--rw-r--r--   0 lucas     (1001) kdt       (1030)      217 2024-01-15 10:39:56.000000 dbdreader-0.5.6/dbdreader/__init__.py
-drwxr-xr-x   0 lucas     (1001) kdt       (1030)        0 2024-01-15 12:37:08.093608 dbdreader-0.5.6/dbdreader/data/
--rw-r--r--   0 lucas     (1001) kdt       (1030)    58453 2024-01-05 10:26:07.000000 dbdreader-0.5.6/dbdreader/data/01600000.dcd
--rw-r--r--   0 lucas     (1001) kdt       (1030)    65844 2024-01-05 10:26:07.000000 dbdreader-0.5.6/dbdreader/data/01600000.ebd
--rw-r--r--   0 lucas     (1001) kdt       (1030)    25966 2024-01-05 10:26:07.000000 dbdreader-0.5.6/dbdreader/data/01600000.ecd
--rw-r--r--   0 lucas     (1001) kdt       (1030)    22651 2024-01-05 10:26:07.000000 dbdreader-0.5.6/dbdreader/data/01600000.mcg
--rw-r--r--   0 lucas     (1001) kdt       (1030)   124854 2024-01-05 10:26:07.000000 dbdreader-0.5.6/dbdreader/data/01600000.mlg
--rw-r--r--   0 lucas     (1001) kdt       (1030)   199043 2024-01-05 10:26:07.000000 dbdreader-0.5.6/dbdreader/data/01600001.dbd
--rw-r--r--   0 lucas     (1001) kdt       (1030)    67883 2024-01-05 10:26:07.000000 dbdreader-0.5.6/dbdreader/data/01600001.dcd
--rw-r--r--   0 lucas     (1001) kdt       (1030)    73919 2024-01-05 10:26:07.000000 dbdreader-0.5.6/dbdreader/data/01600001.ebd
--rw-r--r--   0 lucas     (1001) kdt       (1030)    28986 2024-01-05 10:26:07.000000 dbdreader-0.5.6/dbdreader/data/01600001.ecd
--rw-r--r--   0 lucas     (1001) kdt       (1030)   701666 2024-01-05 10:26:07.000000 dbdreader-0.5.6/dbdreader/data/amadeus-2014-204-05-000.dbd
--rw-r--r--   0 lucas     (1001) kdt       (1030)   154402 2024-01-05 10:26:07.000000 dbdreader-0.5.6/dbdreader/data/amadeus-2014-204-05-000.ebd
--rw-r--r--   0 lucas     (1001) kdt       (1030)     3658 2024-01-05 10:26:07.000000 dbdreader-0.5.6/dbdreader/data/amadeus-2014-204-05-000.sbd
--rw-r--r--   0 lucas     (1001) kdt       (1030)     4802 2024-01-05 10:26:07.000000 dbdreader-0.5.6/dbdreader/data/amadeus-2014-204-05-000.tbd
--rw-r--r--   0 lucas     (1001) kdt       (1030)      570 2024-01-05 10:26:07.000000 dbdreader-0.5.6/dbdreader/data/amadeus-2014-204-05-001.sbd
--rw-r--r--   0 lucas     (1001) kdt       (1030)     2036 2024-01-05 10:26:07.000000 dbdreader-0.5.6/dbdreader/data/amadeus-2014-204-05-001.tbd
--rw-r--r--   0 lucas     (1001) kdt       (1030)     3736 2024-01-05 10:26:07.000000 dbdreader-0.5.6/dbdreader/data/amadeus-2014-204-05-002.sbd
--rw-r--r--   0 lucas     (1001) kdt       (1030)     3981 2024-01-05 10:26:07.000000 dbdreader-0.5.6/dbdreader/data/amadeus-2014-204-05-002.tbd
--rw-r--r--   0 lucas     (1001) kdt       (1030)   313627 2024-01-05 10:26:07.000000 dbdreader-0.5.6/dbdreader/data/ammonite-2008-028-01-000.mbd
-drwxr-xr-x   0 lucas     (1001) kdt       (1030)        0 2024-01-15 12:37:08.094608 dbdreader-0.5.6/dbdreader/data/cac/
--rw-r--r--   0 lucas     (1001) kdt       (1030)   116841 2024-01-05 10:26:07.000000 dbdreader-0.5.6/dbdreader/data/cac/06a36d4e.cac
--rw-r--r--   0 lucas     (1001) kdt       (1030)    45877 2024-01-05 10:26:07.000000 dbdreader-0.5.6/dbdreader/data/cac/06a36d4e.ccc
--rw-r--r--   0 lucas     (1001) kdt       (1030)    86526 2024-01-05 10:26:07.000000 dbdreader-0.5.6/dbdreader/data/cac/093bd5ed.cac
--rw-r--r--   0 lucas     (1001) kdt       (1030)   116841 2024-01-05 14:30:08.000000 dbdreader-0.5.6/dbdreader/data/cac/0f682cb2.cac
--rw-r--r--   0 lucas     (1001) kdt       (1030)    86526 2024-01-05 10:26:07.000000 dbdreader-0.5.6/dbdreader/data/cac/468fd1be.cac
--rw-r--r--   0 lucas     (1001) kdt       (1030)     1528 2024-01-05 10:26:07.000000 dbdreader-0.5.6/dbdreader/data/cac/61b1780f.cac
--rw-r--r--   0 lucas     (1001) kdt       (1030)    59456 2024-01-05 10:26:07.000000 dbdreader-0.5.6/dbdreader/data/cac/813b137d.cac
--rw-r--r--   0 lucas     (1001) kdt       (1030)     4305 2024-01-05 14:30:08.000000 dbdreader-0.5.6/dbdreader/data/cac/92610b65.cac
--rw-r--r--   0 lucas     (1001) kdt       (1030)     3984 2024-01-05 10:26:07.000000 dbdreader-0.5.6/dbdreader/data/cac/c4ec741e.cac
--rw-r--r--   0 lucas     (1001) kdt       (1030)   115341 2024-01-05 10:26:07.000000 dbdreader-0.5.6/dbdreader/data/cac/d6f44165.cac
--rw-r--r--   0 lucas     (1001) kdt       (1030)     4494 2024-01-15 09:44:02.000000 dbdreader-0.5.6/dbdreader/data/cac/daad1b20.cac
--rw-r--r--   0 lucas     (1001) kdt       (1030)     2081 2024-01-05 10:26:07.000000 dbdreader-0.5.6/dbdreader/data/cac/daad1b20.ccc
--rw-r--r--   0 lucas     (1001) kdt       (1030)     1528 2024-01-05 10:26:07.000000 dbdreader-0.5.6/dbdreader/data/cac/dc76ebd5.cac
-drwxr-xr-x   0 lucas     (1001) kdt       (1030)        0 2024-01-15 12:37:08.094608 dbdreader-0.5.6/dbdreader/data/cac_missing/
--rw-r--r--   0 lucas     (1001) kdt       (1030)   115341 2024-01-05 10:26:07.000000 dbdreader-0.5.6/dbdreader/data/cac_missing/d6f44165.cac
--rw-r--r--   0 lucas     (1001) kdt       (1030)    12019 2024-01-05 14:30:08.000000 dbdreader-0.5.6/dbdreader/data/electa-2023-143-00-050.sbd
--rw-r--r--   0 lucas     (1001) kdt       (1030)    22431 2024-01-05 14:30:08.000000 dbdreader-0.5.6/dbdreader/data/electa-2023-143-00-050.tbd
--rw-r--r--   0 lucas     (1001) kdt       (1030)        0 2024-01-05 10:26:07.000000 dbdreader-0.5.6/dbdreader/data/empty-2014-204-05-000.dbd
--rw-r--r--   0 lucas     (1001) kdt       (1030)   701667 2024-01-05 10:26:07.000000 dbdreader-0.5.6/dbdreader/data/invalid_encoding-2014-204-05-000.dbd
--rw-r--r--   0 lucas     (1001) kdt       (1030)   711851 2024-01-05 10:26:07.000000 dbdreader-0.5.6/dbdreader/data/sebastian-2014-204-05-000.dbd
--rw-r--r--   0 lucas     (1001) kdt       (1030)   262229 2024-01-05 10:26:07.000000 dbdreader-0.5.6/dbdreader/data/sebastian-2014-204-05-000.ebd
--rw-r--r--   0 lucas     (1001) kdt       (1030)    35572 2024-01-05 10:26:07.000000 dbdreader-0.5.6/dbdreader/data/sebastian-2014-204-05-001.dbd
--rw-r--r--   0 lucas     (1001) kdt       (1030)    21839 2024-01-05 10:26:07.000000 dbdreader-0.5.6/dbdreader/data/sebastian-2014-204-05-001.ebd
--rw-r--r--   0 lucas     (1001) kdt       (1030)     2537 2024-01-05 10:26:07.000000 dbdreader-0.5.6/dbdreader/data/unit_887-2021-321-3-0.sbd
--rw-r--r--   0 lucas     (1001) kdt       (1030)     3065 2024-01-05 10:26:07.000000 dbdreader-0.5.6/dbdreader/data/unit_887-2021-321-3-0.tbd
--rw-r--r--   0 lucas     (1001) kdt       (1030)    70547 2024-01-12 10:01:54.000000 dbdreader-0.5.6/dbdreader/dbdreader.py
--rw-r--r--   0 lucas     (1001) kdt       (1030)     6962 2024-01-05 10:26:07.000000 dbdreader-0.5.6/dbdreader/decompress.py
--rw-r--r--   0 lucas     (1001) kdt       (1030)    10202 2024-01-05 10:26:07.000000 dbdreader-0.5.6/dbdreader/scripts.py
-drwxr-xr-x   0 lucas     (1001) kdt       (1030)        0 2024-01-15 12:37:08.088608 dbdreader-0.5.6/dbdreader.egg-info/
--rw-r--r--   0 lucas     (1001) kdt       (1030)     8748 2024-01-15 12:37:08.000000 dbdreader-0.5.6/dbdreader.egg-info/PKG-INFO
--rw-r--r--   0 lucas     (1001) kdt       (1030)     2226 2024-01-15 12:37:08.000000 dbdreader-0.5.6/dbdreader.egg-info/SOURCES.txt
--rw-r--r--   0 lucas     (1001) kdt       (1030)        1 2024-01-15 12:37:08.000000 dbdreader-0.5.6/dbdreader.egg-info/dependency_links.txt
--rw-r--r--   0 lucas     (1001) kdt       (1030)       94 2024-01-15 12:37:08.000000 dbdreader-0.5.6/dbdreader.egg-info/entry_points.txt
--rw-r--r--   0 lucas     (1001) kdt       (1030)       17 2024-01-15 12:37:08.000000 dbdreader-0.5.6/dbdreader.egg-info/requires.txt
--rw-r--r--   0 lucas     (1001) kdt       (1030)       21 2024-01-15 12:37:08.000000 dbdreader-0.5.6/dbdreader.egg-info/top_level.txt
-drwxr-xr-x   0 lucas     (1001) kdt       (1030)        0 2024-01-15 12:37:08.095608 dbdreader-0.5.6/examples/
--rw-r--r--   0 lucas     (1001) kdt       (1030)     3531 2024-01-15 09:46:48.000000 dbdreader-0.5.6/examples/read_multiple_dbd_files.py
--rw-r--r--   0 lucas     (1001) kdt       (1030)      725 2024-01-15 09:47:20.000000 dbdreader-0.5.6/examples/read_single_dbd_file.py
-drwxr-xr-x   0 lucas     (1001) kdt       (1030)        0 2024-01-15 12:37:08.095608 dbdreader-0.5.6/extension/
--rw-r--r--   0 lucas     (1001) kdt       (1030)    10686 2024-01-05 14:30:08.000000 dbdreader-0.5.6/extension/dbdreader.c
--rw-r--r--   0 lucas     (1001) kdt       (1030)     5281 2024-01-05 10:26:07.000000 dbdreader-0.5.6/extension/decompress.c
-drwxr-xr-x   0 lucas     (1001) kdt       (1030)        0 2024-01-15 12:37:08.095608 dbdreader-0.5.6/extension/include/
--rw-r--r--   0 lucas     (1001) kdt       (1030)      812 2024-01-05 14:30:08.000000 dbdreader-0.5.6/extension/include/dbdreader.h
--rw-r--r--   0 lucas     (1001) kdt       (1030)      434 2024-01-05 10:26:07.000000 dbdreader-0.5.6/extension/include/decompress.h
--rw-r--r--   0 lucas     (1001) kdt       (1030)     3739 2024-01-05 14:30:08.000000 dbdreader-0.5.6/extension/py_dbdreader.c
-drwxr-xr-x   0 lucas     (1001) kdt       (1030)        0 2024-01-15 12:37:08.095608 dbdreader-0.5.6/lz4/
-drwxr-xr-x   0 lucas     (1001) kdt       (1030)        0 2024-01-15 12:37:08.096608 dbdreader-0.5.6/lz4/include/
--rw-r--r--   0 lucas     (1001) kdt       (1030)    44421 2024-01-05 10:26:07.000000 dbdreader-0.5.6/lz4/include/lz4.h
--rw-r--r--   0 lucas     (1001) kdt       (1030)   114177 2024-01-05 10:26:07.000000 dbdreader-0.5.6/lz4/lz4.c
--rw-r--r--   0 lucas     (1001) kdt       (1030)       19 2024-01-05 10:26:07.000000 dbdreader-0.5.6/requirements.txt
--rw-r--r--   0 lucas     (1001) kdt       (1030)       38 2024-01-15 12:37:08.096608 dbdreader-0.5.6/setup.cfg
--rwxr-xr-x   0 lucas     (1001) kdt       (1030)     4126 2024-01-15 10:29:58.000000 dbdreader-0.5.6/setup.py
-drwxr-xr-x   0 lucas     (1001) kdt       (1030)        0 2024-01-15 12:37:08.096608 dbdreader-0.5.6/tests/
--rw-r--r--   0 lucas     (1001) kdt       (1030)     1464 2024-01-05 10:26:07.000000 dbdreader-0.5.6/tests/dbd_test.py
--rw-r--r--   0 lucas     (1001) kdt       (1030)     1823 2024-01-05 10:26:07.000000 dbdreader-0.5.6/tests/dbd_test_2.py
--rw-r--r--   0 lucas     (1001) kdt       (1030)    23002 2024-01-15 09:44:30.000000 dbdreader-0.5.6/tests/dbdreader_test.py
--rw-r--r--   0 lucas     (1001) kdt       (1030)     7913 2024-01-15 09:43:50.000000 dbdreader-0.5.6/tests/test_decompress.py
+drwxr-xr-x   0 lucas     (1001) kdt       (1030)        0 2024-03-28 08:13:48.017668 dbdreader-0.5.7/
+-rw-r--r--   0 lucas     (1001) kdt       (1030)    18009 2024-01-05 10:26:07.000000 dbdreader-0.5.7/COPYING
+-rw-r--r--   0 lucas     (1001) kdt       (1030)      704 2024-01-05 10:26:07.000000 dbdreader-0.5.7/COPYRIGHT
+-rw-r--r--   0 lucas     (1001) kdt       (1030)      545 2024-01-05 10:26:07.000000 dbdreader-0.5.7/INSTALL.rst
+-rw-r--r--   0 lucas     (1001) kdt       (1030)    35147 2024-01-05 10:26:07.000000 dbdreader-0.5.7/LICENSE
+-rw-r--r--   0 lucas     (1001) kdt       (1030)      346 2024-01-15 09:42:37.000000 dbdreader-0.5.7/MANIFEST.in
+-rw-r--r--   0 lucas     (1001) kdt       (1030)     8973 2024-03-28 08:13:48.017668 dbdreader-0.5.7/PKG-INFO
+-rw-r--r--   0 lucas     (1001) kdt       (1030)     8406 2024-03-28 08:07:10.000000 dbdreader-0.5.7/README.rst
+drwxr-xr-x   0 lucas     (1001) kdt       (1030)        0 2024-03-28 08:13:48.005668 dbdreader-0.5.7/dbdreader/
+-rw-r--r--   0 lucas     (1001) kdt       (1030)      217 2024-03-28 07:58:42.000000 dbdreader-0.5.7/dbdreader/__init__.py
+drwxr-xr-x   0 lucas     (1001) kdt       (1030)        0 2024-03-28 08:13:48.012668 dbdreader-0.5.7/dbdreader/data/
+-rw-r--r--   0 lucas     (1001) kdt       (1030)    58453 2024-01-05 10:26:07.000000 dbdreader-0.5.7/dbdreader/data/01600000.dcd
+-rw-r--r--   0 lucas     (1001) kdt       (1030)    65844 2024-01-05 10:26:07.000000 dbdreader-0.5.7/dbdreader/data/01600000.ebd
+-rw-r--r--   0 lucas     (1001) kdt       (1030)    25966 2024-01-05 10:26:07.000000 dbdreader-0.5.7/dbdreader/data/01600000.ecd
+-rw-r--r--   0 lucas     (1001) kdt       (1030)    22651 2024-01-05 10:26:07.000000 dbdreader-0.5.7/dbdreader/data/01600000.mcg
+-rw-r--r--   0 lucas     (1001) kdt       (1030)   124854 2024-01-05 10:26:07.000000 dbdreader-0.5.7/dbdreader/data/01600000.mlg
+-rw-r--r--   0 lucas     (1001) kdt       (1030)   199043 2024-01-05 10:26:07.000000 dbdreader-0.5.7/dbdreader/data/01600001.dbd
+-rw-r--r--   0 lucas     (1001) kdt       (1030)    67883 2024-01-05 10:26:07.000000 dbdreader-0.5.7/dbdreader/data/01600001.dcd
+-rw-r--r--   0 lucas     (1001) kdt       (1030)    73919 2024-01-05 10:26:07.000000 dbdreader-0.5.7/dbdreader/data/01600001.ebd
+-rw-r--r--   0 lucas     (1001) kdt       (1030)    28986 2024-01-05 10:26:07.000000 dbdreader-0.5.7/dbdreader/data/01600001.ecd
+-rw-r--r--   0 lucas     (1001) kdt       (1030)   701666 2024-01-05 10:26:07.000000 dbdreader-0.5.7/dbdreader/data/amadeus-2014-204-05-000.dbd
+-rw-r--r--   0 lucas     (1001) kdt       (1030)   154402 2024-01-05 10:26:07.000000 dbdreader-0.5.7/dbdreader/data/amadeus-2014-204-05-000.ebd
+-rw-r--r--   0 lucas     (1001) kdt       (1030)     3658 2024-01-05 10:26:07.000000 dbdreader-0.5.7/dbdreader/data/amadeus-2014-204-05-000.sbd
+-rw-r--r--   0 lucas     (1001) kdt       (1030)     4802 2024-01-05 10:26:07.000000 dbdreader-0.5.7/dbdreader/data/amadeus-2014-204-05-000.tbd
+-rw-r--r--   0 lucas     (1001) kdt       (1030)      570 2024-01-05 10:26:07.000000 dbdreader-0.5.7/dbdreader/data/amadeus-2014-204-05-001.sbd
+-rw-r--r--   0 lucas     (1001) kdt       (1030)     2036 2024-01-05 10:26:07.000000 dbdreader-0.5.7/dbdreader/data/amadeus-2014-204-05-001.tbd
+-rw-r--r--   0 lucas     (1001) kdt       (1030)     3736 2024-01-05 10:26:07.000000 dbdreader-0.5.7/dbdreader/data/amadeus-2014-204-05-002.sbd
+-rw-r--r--   0 lucas     (1001) kdt       (1030)     3981 2024-01-05 10:26:07.000000 dbdreader-0.5.7/dbdreader/data/amadeus-2014-204-05-002.tbd
+-rw-r--r--   0 lucas     (1001) kdt       (1030)   313627 2024-01-05 10:26:07.000000 dbdreader-0.5.7/dbdreader/data/ammonite-2008-028-01-000.mbd
+drwxr-xr-x   0 lucas     (1001) kdt       (1030)        0 2024-03-28 08:13:48.014668 dbdreader-0.5.7/dbdreader/data/cac/
+-rw-r--r--   0 lucas     (1001) kdt       (1030)   116841 2024-01-05 10:26:07.000000 dbdreader-0.5.7/dbdreader/data/cac/06a36d4e.cac
+-rw-r--r--   0 lucas     (1001) kdt       (1030)    45877 2024-01-05 10:26:07.000000 dbdreader-0.5.7/dbdreader/data/cac/06a36d4e.ccc
+-rw-r--r--   0 lucas     (1001) kdt       (1030)    86526 2024-01-05 10:26:07.000000 dbdreader-0.5.7/dbdreader/data/cac/093bd5ed.cac
+-rw-r--r--   0 lucas     (1001) kdt       (1030)   116841 2024-01-05 14:30:08.000000 dbdreader-0.5.7/dbdreader/data/cac/0f682cb2.cac
+-rw-r--r--   0 lucas     (1001) kdt       (1030)    86526 2024-01-05 10:26:07.000000 dbdreader-0.5.7/dbdreader/data/cac/468fd1be.cac
+-rw-r--r--   0 lucas     (1001) kdt       (1030)     1528 2024-01-05 10:26:07.000000 dbdreader-0.5.7/dbdreader/data/cac/61b1780f.cac
+-rw-r--r--   0 lucas     (1001) kdt       (1030)    59456 2024-01-05 10:26:07.000000 dbdreader-0.5.7/dbdreader/data/cac/813b137d.cac
+-rw-r--r--   0 lucas     (1001) kdt       (1030)     4305 2024-01-05 14:30:08.000000 dbdreader-0.5.7/dbdreader/data/cac/92610b65.cac
+-rw-r--r--   0 lucas     (1001) kdt       (1030)     3984 2024-01-05 10:26:07.000000 dbdreader-0.5.7/dbdreader/data/cac/c4ec741e.cac
+-rw-r--r--   0 lucas     (1001) kdt       (1030)   115341 2024-01-05 10:26:07.000000 dbdreader-0.5.7/dbdreader/data/cac/d6f44165.cac
+-rw-r--r--   0 lucas     (1001) kdt       (1030)     4494 2024-01-15 09:44:02.000000 dbdreader-0.5.7/dbdreader/data/cac/daad1b20.cac
+-rw-r--r--   0 lucas     (1001) kdt       (1030)     2081 2024-01-05 10:26:07.000000 dbdreader-0.5.7/dbdreader/data/cac/daad1b20.ccc
+-rw-r--r--   0 lucas     (1001) kdt       (1030)     1528 2024-01-05 10:26:07.000000 dbdreader-0.5.7/dbdreader/data/cac/dc76ebd5.cac
+drwxr-xr-x   0 lucas     (1001) kdt       (1030)        0 2024-03-28 08:13:48.014668 dbdreader-0.5.7/dbdreader/data/cac_missing/
+-rw-r--r--   0 lucas     (1001) kdt       (1030)   115341 2024-01-05 10:26:07.000000 dbdreader-0.5.7/dbdreader/data/cac_missing/d6f44165.cac
+-rw-r--r--   0 lucas     (1001) kdt       (1030)    12019 2024-01-05 14:30:08.000000 dbdreader-0.5.7/dbdreader/data/electa-2023-143-00-050.sbd
+-rw-r--r--   0 lucas     (1001) kdt       (1030)    22431 2024-01-05 14:30:08.000000 dbdreader-0.5.7/dbdreader/data/electa-2023-143-00-050.tbd
+-rw-r--r--   0 lucas     (1001) kdt       (1030)        0 2024-01-05 10:26:07.000000 dbdreader-0.5.7/dbdreader/data/empty-2014-204-05-000.dbd
+-rw-r--r--   0 lucas     (1001) kdt       (1030)   701667 2024-01-05 10:26:07.000000 dbdreader-0.5.7/dbdreader/data/invalid_encoding-2014-204-05-000.dbd
+-rw-r--r--   0 lucas     (1001) kdt       (1030)   711851 2024-01-05 10:26:07.000000 dbdreader-0.5.7/dbdreader/data/sebastian-2014-204-05-000.dbd
+-rw-r--r--   0 lucas     (1001) kdt       (1030)   262229 2024-01-05 10:26:07.000000 dbdreader-0.5.7/dbdreader/data/sebastian-2014-204-05-000.ebd
+-rw-r--r--   0 lucas     (1001) kdt       (1030)    35572 2024-01-05 10:26:07.000000 dbdreader-0.5.7/dbdreader/data/sebastian-2014-204-05-001.dbd
+-rw-r--r--   0 lucas     (1001) kdt       (1030)    21839 2024-01-05 10:26:07.000000 dbdreader-0.5.7/dbdreader/data/sebastian-2014-204-05-001.ebd
+-rw-r--r--   0 lucas     (1001) kdt       (1030)     2537 2024-01-05 10:26:07.000000 dbdreader-0.5.7/dbdreader/data/unit_887-2021-321-3-0.sbd
+-rw-r--r--   0 lucas     (1001) kdt       (1030)     3065 2024-01-05 10:26:07.000000 dbdreader-0.5.7/dbdreader/data/unit_887-2021-321-3-0.tbd
+-rw-r--r--   0 lucas     (1001) kdt       (1030)    70547 2024-01-12 10:01:54.000000 dbdreader-0.5.7/dbdreader/dbdreader.py
+-rw-r--r--   0 lucas     (1001) kdt       (1030)     6962 2024-01-05 10:26:07.000000 dbdreader-0.5.7/dbdreader/decompress.py
+-rw-r--r--   0 lucas     (1001) kdt       (1030)    10202 2024-01-05 10:26:07.000000 dbdreader-0.5.7/dbdreader/scripts.py
+drwxr-xr-x   0 lucas     (1001) kdt       (1030)        0 2024-03-28 08:13:48.005668 dbdreader-0.5.7/dbdreader.egg-info/
+-rw-r--r--   0 lucas     (1001) kdt       (1030)     8973 2024-03-28 08:13:47.000000 dbdreader-0.5.7/dbdreader.egg-info/PKG-INFO
+-rw-r--r--   0 lucas     (1001) kdt       (1030)     2226 2024-03-28 08:13:47.000000 dbdreader-0.5.7/dbdreader.egg-info/SOURCES.txt
+-rw-r--r--   0 lucas     (1001) kdt       (1030)        1 2024-03-28 08:13:47.000000 dbdreader-0.5.7/dbdreader.egg-info/dependency_links.txt
+-rw-r--r--   0 lucas     (1001) kdt       (1030)       94 2024-03-28 08:13:47.000000 dbdreader-0.5.7/dbdreader.egg-info/entry_points.txt
+-rw-r--r--   0 lucas     (1001) kdt       (1030)       17 2024-03-28 08:13:47.000000 dbdreader-0.5.7/dbdreader.egg-info/requires.txt
+-rw-r--r--   0 lucas     (1001) kdt       (1030)       21 2024-03-28 08:13:47.000000 dbdreader-0.5.7/dbdreader.egg-info/top_level.txt
+drwxr-xr-x   0 lucas     (1001) kdt       (1030)        0 2024-03-28 08:13:48.015668 dbdreader-0.5.7/examples/
+-rw-r--r--   0 lucas     (1001) kdt       (1030)     3531 2024-01-15 09:46:48.000000 dbdreader-0.5.7/examples/read_multiple_dbd_files.py
+-rw-r--r--   0 lucas     (1001) kdt       (1030)      725 2024-01-15 09:47:20.000000 dbdreader-0.5.7/examples/read_single_dbd_file.py
+drwxr-xr-x   0 lucas     (1001) kdt       (1030)        0 2024-03-28 08:13:48.015668 dbdreader-0.5.7/extension/
+-rw-r--r--   0 lucas     (1001) kdt       (1030)    10686 2024-01-05 14:30:08.000000 dbdreader-0.5.7/extension/dbdreader.c
+-rw-r--r--   0 lucas     (1001) kdt       (1030)     5281 2024-01-05 10:26:07.000000 dbdreader-0.5.7/extension/decompress.c
+drwxr-xr-x   0 lucas     (1001) kdt       (1030)        0 2024-03-28 08:13:48.015668 dbdreader-0.5.7/extension/include/
+-rw-r--r--   0 lucas     (1001) kdt       (1030)      812 2024-01-05 14:30:08.000000 dbdreader-0.5.7/extension/include/dbdreader.h
+-rw-r--r--   0 lucas     (1001) kdt       (1030)      434 2024-01-05 10:26:07.000000 dbdreader-0.5.7/extension/include/decompress.h
+-rw-r--r--   0 lucas     (1001) kdt       (1030)     3739 2024-01-05 14:30:08.000000 dbdreader-0.5.7/extension/py_dbdreader.c
+drwxr-xr-x   0 lucas     (1001) kdt       (1030)        0 2024-03-28 08:13:48.015668 dbdreader-0.5.7/lz4/
+drwxr-xr-x   0 lucas     (1001) kdt       (1030)        0 2024-03-28 08:13:48.016668 dbdreader-0.5.7/lz4/include/
+-rw-r--r--   0 lucas     (1001) kdt       (1030)    44421 2024-01-05 10:26:07.000000 dbdreader-0.5.7/lz4/include/lz4.h
+-rw-r--r--   0 lucas     (1001) kdt       (1030)   114177 2024-01-05 10:26:07.000000 dbdreader-0.5.7/lz4/lz4.c
+-rw-r--r--   0 lucas     (1001) kdt       (1030)       19 2024-01-05 10:26:07.000000 dbdreader-0.5.7/requirements.txt
+-rw-r--r--   0 lucas     (1001) kdt       (1030)       38 2024-03-28 08:13:48.017668 dbdreader-0.5.7/setup.cfg
+-rwxr-xr-x   0 lucas     (1001) kdt       (1030)     4112 2024-03-28 07:54:32.000000 dbdreader-0.5.7/setup.py
+drwxr-xr-x   0 lucas     (1001) kdt       (1030)        0 2024-03-28 08:13:48.017668 dbdreader-0.5.7/tests/
+-rw-r--r--   0 lucas     (1001) kdt       (1030)     1464 2024-01-05 10:26:07.000000 dbdreader-0.5.7/tests/dbd_test.py
+-rw-r--r--   0 lucas     (1001) kdt       (1030)     1823 2024-01-05 10:26:07.000000 dbdreader-0.5.7/tests/dbd_test_2.py
+-rw-r--r--   0 lucas     (1001) kdt       (1030)    23002 2024-01-15 09:44:30.000000 dbdreader-0.5.7/tests/dbdreader_test.py
+-rw-r--r--   0 lucas     (1001) kdt       (1030)     7913 2024-01-15 09:43:50.000000 dbdreader-0.5.7/tests/test_decompress.py
```

### Comparing `dbdreader-0.5.6/COPYING` & `dbdreader-0.5.7/COPYING`

 * *Files identical despite different names*

### Comparing `dbdreader-0.5.6/COPYRIGHT` & `dbdreader-0.5.7/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `dbdreader-0.5.6/INSTALL.rst` & `dbdreader-0.5.7/INSTALL.rst`

 * *Files identical despite different names*

### Comparing `dbdreader-0.5.6/LICENSE` & `dbdreader-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dbdreader-0.5.6/PKG-INFO` & `dbdreader-0.5.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbdreader
-Version: 0.5.6
+Version: 0.5.7
 Summary: A python module to access binary data files generated by Teledyne WebbResearch gliders
 Home-page: https://dbdreader.readthedocs.io/en/latest/
 Author: Lucas Merckelbach
 Author-email: lucas.merckelbach@hereon.de
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -14,16 +14,35 @@
 License-File: COPYING
 
 |PyPI version| |Docs badge| |License|
 
 DBDREADER
 =========
 
+Synopsis
+--------
+Slocum ocean gliders are autonomous underwater vehicles, used for
+making oceanographic measurements. The data that these devices and
+their sensors collect, are stored in binary data files. The python
+module *dbdreader* provides the utilities to extract the data from the
+binary files, so that they can be further analysed.
+
 Change log
 ----------
+
+Version 0.5.7
+
+* Drops dependency on python 3.10+, introduced in 0.5.6, and should
+  work still with python 3.9.
+
+Version 0.5.6
+
+* Moves data directory under dbdreader, making these files accessible
+  after an pip install
+
 Version 0.5.5
 
 * Makes MultiDBD's get_CTD_sync method compatible with RBR CTD data.
 
 Version 0.5.4
 
 * Adds support for reading compressed data files for windows platform.
@@ -128,21 +147,14 @@
 Version 0.4.5
 
 * dbdreader now ignores the first line of data in each binary file
   
 * dbdreader checks whether the value of the parameters read are finite, ignoring them if they are not.
 
 
-Synopsis
---------
-Slocum ocean gliders are autonomous underwater vehicles, used for
-making oceanographic measurements. The data that these devices and
-their sensors collect, are stored in binary data files. The python
-module *dbdreader* provides the utilities to extract the data from the
-binary files, so that they can be further analysed.
 
 Installation (linux)
 --------------------
 
 The python module *dbdreader* can be installed from source, using the
 standard method to install python code. Note that this method requires
 an C-extension to be build. (The actual reading from files is done in
```

### Comparing `dbdreader-0.5.6/README.rst` & `dbdreader-0.5.7/dbdreader.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,48 @@
+Metadata-Version: 2.1
+Name: dbdreader
+Version: 0.5.7
+Summary: A python module to access binary data files generated by Teledyne WebbResearch gliders
+Home-page: https://dbdreader.readthedocs.io/en/latest/
+Author: Lucas Merckelbach
+Author-email: lucas.merckelbach@hereon.de
+Classifier: Programming Language :: Python :: 3
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: POSIX
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+License-File: COPYING
+
 |PyPI version| |Docs badge| |License|
 
 DBDREADER
 =========
 
+Synopsis
+--------
+Slocum ocean gliders are autonomous underwater vehicles, used for
+making oceanographic measurements. The data that these devices and
+their sensors collect, are stored in binary data files. The python
+module *dbdreader* provides the utilities to extract the data from the
+binary files, so that they can be further analysed.
+
 Change log
 ----------
+
+Version 0.5.7
+
+* Drops dependency on python 3.10+, introduced in 0.5.6, and should
+  work still with python 3.9.
+
+Version 0.5.6
+
+* Moves data directory under dbdreader, making these files accessible
+  after an pip install
+
 Version 0.5.5
 
 * Makes MultiDBD's get_CTD_sync method compatible with RBR CTD data.
 
 Version 0.5.4
 
 * Adds support for reading compressed data files for windows platform.
@@ -113,21 +147,14 @@
 Version 0.4.5
 
 * dbdreader now ignores the first line of data in each binary file
   
 * dbdreader checks whether the value of the parameters read are finite, ignoring them if they are not.
 
 
-Synopsis
---------
-Slocum ocean gliders are autonomous underwater vehicles, used for
-making oceanographic measurements. The data that these devices and
-their sensors collect, are stored in binary data files. The python
-module *dbdreader* provides the utilities to extract the data from the
-binary files, so that they can be further analysed.
 
 Installation (linux)
 --------------------
 
 The python module *dbdreader* can be installed from source, using the
 standard method to install python code. Note that this method requires
 an C-extension to be build. (The actual reading from files is done in
```

### Comparing `dbdreader-0.5.6/dbdreader/data/01600000.dcd` & `dbdreader-0.5.7/dbdreader/data/01600000.dcd`

 * *Files identical despite different names*

### Comparing `dbdreader-0.5.6/dbdreader/data/01600000.ebd` & `dbdreader-0.5.7/dbdreader/data/01600000.ebd`

 * *Files identical despite different names*

### Comparing `dbdreader-0.5.6/dbdreader/data/01600000.ecd` & `dbdreader-0.5.7/dbdreader/data/01600000.ecd`

 * *Files identical despite different names*

### Comparing `dbdreader-0.5.6/dbdreader/data/01600000.mcg` & `dbdreader-0.5.7/dbdreader/data/01600000.mcg`

 * *Files identical despite different names*

### Comparing `dbdreader-0.5.6/dbdreader/data/01600000.mlg` & `dbdreader-0.5.7/dbdreader/data/01600000.mlg`

 * *Files identical despite different names*

### Comparing `dbdreader-0.5.6/dbdreader/data/01600001.dbd` & `dbdreader-0.5.7/dbdreader/data/01600001.dbd`

 * *Files identical despite different names*

### Comparing `dbdreader-0.5.6/dbdreader/data/01600001.dcd` & `dbdreader-0.5.7/dbdreader/data/01600001.dcd`

 * *Files identical despite different names*

### Comparing `dbdreader-0.5.6/dbdreader/data/01600001.ebd` & `dbdreader-0.5.7/dbdreader/data/01600001.ebd`

 * *Files identical despite different names*

### Comparing `dbdreader-0.5.6/dbdreader/data/01600001.ecd` & `dbdreader-0.5.7/dbdreader/data/01600001.ecd`

 * *Files identical despite different names*

### Comparing `dbdreader-0.5.6/dbdreader/data/amadeus-2014-204-05-000.dbd` & `dbdreader-0.5.7/dbdreader/data/amadeus-2014-204-05-000.dbd`

 * *Files identical despite different names*

### Comparing `dbdreader-0.5.6/dbdreader/data/amadeus-2014-204-05-000.ebd` & `dbdreader-0.5.7/dbdreader/data/amadeus-2014-204-05-000.ebd`

 * *Files identical despite different names*

### Comparing `dbdreader-0.5.6/dbdreader/data/amadeus-2014-204-05-000.sbd` & `dbdreader-0.5.7/dbdreader/data/amadeus-2014-204-05-000.sbd`

 * *Files identical despite different names*

### Comparing `dbdreader-0.5.6/dbdreader/data/amadeus-2014-204-05-000.tbd` & `dbdreader-0.5.7/dbdreader/data/amadeus-2014-204-05-000.tbd`

 * *Files identical despite different names*

### Comparing `dbdreader-0.5.6/dbdreader/data/amadeus-2014-204-05-001.sbd` & `dbdreader-0.5.7/dbdreader/data/amadeus-2014-204-05-001.sbd`

 * *Files identical despite different names*

### Comparing `dbdreader-0.5.6/dbdreader/data/amadeus-2014-204-05-001.tbd` & `dbdreader-0.5.7/dbdreader/data/amadeus-2014-204-05-001.tbd`

 * *Files identical despite different names*

### Comparing `dbdreader-0.5.6/dbdreader/data/amadeus-2014-204-05-002.sbd` & `dbdreader-0.5.7/dbdreader/data/amadeus-2014-204-05-002.sbd`

 * *Files identical despite different names*

### Comparing `dbdreader-0.5.6/dbdreader/data/amadeus-2014-204-05-002.tbd` & `dbdreader-0.5.7/dbdreader/data/amadeus-2014-204-05-002.tbd`

 * *Files identical despite different names*

### Comparing `dbdreader-0.5.6/dbdreader/data/ammonite-2008-028-01-000.mbd` & `dbdreader-0.5.7/dbdreader/data/ammonite-2008-028-01-000.mbd`

 * *Files identical despite different names*

### Comparing `dbdreader-0.5.6/dbdreader/data/cac/06a36d4e.cac` & `dbdreader-0.5.7/dbdreader/data/cac/06a36d4e.cac`

 * *Files identical despite different names*

### Comparing `dbdreader-0.5.6/dbdreader/data/cac/06a36d4e.ccc` & `dbdreader-0.5.7/dbdreader/data/cac/06a36d4e.ccc`

 * *Files identical despite different names*

### Comparing `dbdreader-0.5.6/dbdreader/data/cac/093bd5ed.cac` & `dbdreader-0.5.7/dbdreader/data/cac/093bd5ed.cac`

 * *Files identical despite different names*

### Comparing `dbdreader-0.5.6/dbdreader/data/cac/0f682cb2.cac` & `dbdreader-0.5.7/dbdreader/data/cac/0f682cb2.cac`

 * *Files identical despite different names*

### Comparing `dbdreader-0.5.6/dbdreader/data/cac/468fd1be.cac` & `dbdreader-0.5.7/dbdreader/data/cac/468fd1be.cac`

 * *Files identical despite different names*

### Comparing `dbdreader-0.5.6/dbdreader/data/cac/61b1780f.cac` & `dbdreader-0.5.7/dbdreader/data/cac/61b1780f.cac`

 * *Files identical despite different names*

### Comparing `dbdreader-0.5.6/dbdreader/data/cac/813b137d.cac` & `dbdreader-0.5.7/dbdreader/data/cac/813b137d.cac`

 * *Files identical despite different names*

### Comparing `dbdreader-0.5.6/dbdreader/data/cac/92610b65.cac` & `dbdreader-0.5.7/dbdreader/data/cac/92610b65.cac`

 * *Files identical despite different names*

### Comparing `dbdreader-0.5.6/dbdreader/data/cac/c4ec741e.cac` & `dbdreader-0.5.7/dbdreader/data/cac/c4ec741e.cac`

 * *Files identical despite different names*

### Comparing `dbdreader-0.5.6/dbdreader/data/cac/d6f44165.cac` & `dbdreader-0.5.7/dbdreader/data/cac/d6f44165.cac`

 * *Files identical despite different names*

### Comparing `dbdreader-0.5.6/dbdreader/data/cac/daad1b20.cac` & `dbdreader-0.5.7/dbdreader/data/cac/daad1b20.cac`

 * *Files identical despite different names*

### Comparing `dbdreader-0.5.6/dbdreader/data/cac/daad1b20.ccc` & `dbdreader-0.5.7/dbdreader/data/cac/daad1b20.ccc`

 * *Files identical despite different names*

### Comparing `dbdreader-0.5.6/dbdreader/data/cac/dc76ebd5.cac` & `dbdreader-0.5.7/dbdreader/data/cac/dc76ebd5.cac`

 * *Files identical despite different names*

### Comparing `dbdreader-0.5.6/dbdreader/data/cac_missing/d6f44165.cac` & `dbdreader-0.5.7/dbdreader/data/cac_missing/d6f44165.cac`

 * *Files identical despite different names*

### Comparing `dbdreader-0.5.6/dbdreader/data/electa-2023-143-00-050.sbd` & `dbdreader-0.5.7/dbdreader/data/electa-2023-143-00-050.sbd`

 * *Files identical despite different names*

### Comparing `dbdreader-0.5.6/dbdreader/data/electa-2023-143-00-050.tbd` & `dbdreader-0.5.7/dbdreader/data/electa-2023-143-00-050.tbd`

 * *Files identical despite different names*

### Comparing `dbdreader-0.5.6/dbdreader/data/invalid_encoding-2014-204-05-000.dbd` & `dbdreader-0.5.7/dbdreader/data/invalid_encoding-2014-204-05-000.dbd`

 * *Files identical despite different names*

### Comparing `dbdreader-0.5.6/dbdreader/data/sebastian-2014-204-05-000.dbd` & `dbdreader-0.5.7/dbdreader/data/sebastian-2014-204-05-000.dbd`

 * *Files identical despite different names*

### Comparing `dbdreader-0.5.6/dbdreader/data/sebastian-2014-204-05-000.ebd` & `dbdreader-0.5.7/dbdreader/data/sebastian-2014-204-05-000.ebd`

 * *Files identical despite different names*

### Comparing `dbdreader-0.5.6/dbdreader/data/sebastian-2014-204-05-001.dbd` & `dbdreader-0.5.7/dbdreader/data/sebastian-2014-204-05-001.dbd`

 * *Files identical despite different names*

### Comparing `dbdreader-0.5.6/dbdreader/data/sebastian-2014-204-05-001.ebd` & `dbdreader-0.5.7/dbdreader/data/sebastian-2014-204-05-001.ebd`

 * *Files identical despite different names*

### Comparing `dbdreader-0.5.6/dbdreader/data/unit_887-2021-321-3-0.sbd` & `dbdreader-0.5.7/dbdreader/data/unit_887-2021-321-3-0.sbd`

 * *Files identical despite different names*

### Comparing `dbdreader-0.5.6/dbdreader/data/unit_887-2021-321-3-0.tbd` & `dbdreader-0.5.7/dbdreader/data/unit_887-2021-321-3-0.tbd`

 * *Files identical despite different names*

### Comparing `dbdreader-0.5.6/dbdreader/dbdreader.py` & `dbdreader-0.5.7/dbdreader/dbdreader.py`

 * *Files identical despite different names*

### Comparing `dbdreader-0.5.6/dbdreader/decompress.py` & `dbdreader-0.5.7/dbdreader/decompress.py`

 * *Files identical despite different names*

### Comparing `dbdreader-0.5.6/dbdreader/scripts.py` & `dbdreader-0.5.7/dbdreader/scripts.py`

 * *Files identical despite different names*

### Comparing `dbdreader-0.5.6/dbdreader.egg-info/PKG-INFO` & `dbdreader-0.5.7/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,33 @@
-Metadata-Version: 2.1
-Name: dbdreader
-Version: 0.5.6
-Summary: A python module to access binary data files generated by Teledyne WebbResearch gliders
-Home-page: https://dbdreader.readthedocs.io/en/latest/
-Author: Lucas Merckelbach
-Author-email: lucas.merckelbach@hereon.de
-Classifier: Programming Language :: Python :: 3
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: POSIX
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-License-File: COPYING
-
 |PyPI version| |Docs badge| |License|
 
 DBDREADER
 =========
 
+Synopsis
+--------
+Slocum ocean gliders are autonomous underwater vehicles, used for
+making oceanographic measurements. The data that these devices and
+their sensors collect, are stored in binary data files. The python
+module *dbdreader* provides the utilities to extract the data from the
+binary files, so that they can be further analysed.
+
 Change log
 ----------
+
+Version 0.5.7
+
+* Drops dependency on python 3.10+, introduced in 0.5.6, and should
+  work still with python 3.9.
+
+Version 0.5.6
+
+* Moves data directory under dbdreader, making these files accessible
+  after an pip install
+
 Version 0.5.5
 
 * Makes MultiDBD's get_CTD_sync method compatible with RBR CTD data.
 
 Version 0.5.4
 
 * Adds support for reading compressed data files for windows platform.
@@ -128,21 +132,14 @@
 Version 0.4.5
 
 * dbdreader now ignores the first line of data in each binary file
   
 * dbdreader checks whether the value of the parameters read are finite, ignoring them if they are not.
 
 
-Synopsis
---------
-Slocum ocean gliders are autonomous underwater vehicles, used for
-making oceanographic measurements. The data that these devices and
-their sensors collect, are stored in binary data files. The python
-module *dbdreader* provides the utilities to extract the data from the
-binary files, so that they can be further analysed.
 
 Installation (linux)
 --------------------
 
 The python module *dbdreader* can be installed from source, using the
 standard method to install python code. Note that this method requires
 an C-extension to be build. (The actual reading from files is done in
```

### Comparing `dbdreader-0.5.6/dbdreader.egg-info/SOURCES.txt` & `dbdreader-0.5.7/dbdreader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbdreader-0.5.6/examples/read_multiple_dbd_files.py` & `dbdreader-0.5.7/examples/read_multiple_dbd_files.py`

 * *Files identical despite different names*

### Comparing `dbdreader-0.5.6/examples/read_single_dbd_file.py` & `dbdreader-0.5.7/examples/read_single_dbd_file.py`

 * *Files identical despite different names*

### Comparing `dbdreader-0.5.6/extension/dbdreader.c` & `dbdreader-0.5.7/extension/dbdreader.c`

 * *Files identical despite different names*

### Comparing `dbdreader-0.5.6/extension/decompress.c` & `dbdreader-0.5.7/extension/decompress.c`

 * *Files identical despite different names*

### Comparing `dbdreader-0.5.6/extension/include/dbdreader.h` & `dbdreader-0.5.7/extension/include/dbdreader.h`

 * *Files identical despite different names*

### Comparing `dbdreader-0.5.6/extension/py_dbdreader.c` & `dbdreader-0.5.7/extension/py_dbdreader.c`

 * *Files identical despite different names*

### Comparing `dbdreader-0.5.6/lz4/include/lz4.h` & `dbdreader-0.5.7/lz4/include/lz4.h`

 * *Files identical despite different names*

### Comparing `dbdreader-0.5.6/lz4/lz4.c` & `dbdreader-0.5.7/lz4/lz4.c`

 * *Files identical despite different names*

### Comparing `dbdreader-0.5.6/setup.py` & `dbdreader-0.5.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -104,15 +104,15 @@
     author="Lucas Merckelbach",
     author_email="lucas.merckelbach@hereon.de",
     description="A python module to access binary data files generated by Teledyne WebbResearch gliders",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url='https://dbdreader.readthedocs.io/en/latest/',
     packages=['dbdreader'],
-    package_data = {'dbdreader': glob.glob("dbdreader/data/*", root_dir='.')},
+    package_data = {'dbdreader': glob.glob("dbdreader/data/*")},
     include_package_data=True,
     py_modules=[],
     entry_points = {'console_scripts':['dbdrename=dbdreader.scripts:dbdrename',
                                         'cac_gen=dbdreader.scripts:cac_gen'],
                     'gui_scripts':[]
     },
     scripts = [],
```

### Comparing `dbdreader-0.5.6/tests/dbd_test.py` & `dbdreader-0.5.7/tests/dbd_test.py`

 * *Files identical despite different names*

### Comparing `dbdreader-0.5.6/tests/dbd_test_2.py` & `dbdreader-0.5.7/tests/dbd_test_2.py`

 * *Files identical despite different names*

### Comparing `dbdreader-0.5.6/tests/dbdreader_test.py` & `dbdreader-0.5.7/tests/dbdreader_test.py`

 * *Files identical despite different names*

### Comparing `dbdreader-0.5.6/tests/test_decompress.py` & `dbdreader-0.5.7/tests/test_decompress.py`

 * *Files identical despite different names*

