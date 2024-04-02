# Comparing `tmp/cbcmgr-2.2.8.tar.gz` & `tmp/cbcmgr-2.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbcmgr-2.2.8.tar", last modified: Tue Jan 30 03:06:10 2024, max compression
+gzip compressed data, was "cbcmgr-2.2.9.tar", last modified: Tue Jan 30 22:26:06 2024, max compression
```

## Comparing `cbcmgr-2.2.8.tar` & `cbcmgr-2.2.9.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-01-30 03:06:10.364437 cbcmgr-2.2.8/
--rw-r--r--   0 michael    (501) staff       (20)      291 2024-01-30 03:05:54.000000 cbcmgr-2.2.8/.bumpversion.cfg
--rw-r--r--   0 michael    (501) staff       (20)     3101 2023-08-26 01:02:18.000000 cbcmgr-2.2.8/.gitignore
--rw-r--r--   0 michael    (501) staff       (20)     1074 2023-02-14 15:09:46.000000 cbcmgr-2.2.8/LICENSE.txt
--rw-r--r--   0 michael    (501) staff       (20)     1270 2024-01-18 15:25:57.000000 cbcmgr-2.2.8/Makefile
--rw-r--r--   0 michael    (501) staff       (20)    13895 2024-01-30 03:06:10.364199 cbcmgr-2.2.8/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)    13096 2024-01-30 03:05:54.000000 cbcmgr-2.2.8/README.md
--rw-r--r--   0 michael    (501) staff       (20)        6 2024-01-30 03:05:54.000000 cbcmgr-2.2.8/VERSION
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-01-30 03:06:10.338325 cbcmgr-2.2.8/cbcmgr/
--rw-r--r--   0 michael    (501) staff       (20)      235 2024-01-30 03:05:54.000000 cbcmgr-2.2.8/cbcmgr/__init__.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-01-30 03:06:10.340268 cbcmgr-2.2.8/cbcmgr/api/
--rw-r--r--   0 michael    (501) staff       (20)        0 2023-09-28 20:20:23.000000 cbcmgr-2.2.8/cbcmgr/api/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)     1221 2023-09-28 20:51:47.000000 cbcmgr-2.2.8/cbcmgr/api/load.py
--rw-r--r--   0 michael    (501) staff       (20)     3180 2023-12-20 22:26:35.000000 cbcmgr-2.2.8/cbcmgr/async_pool.py
--rw-r--r--   0 michael    (501) staff       (20)     3377 2024-01-29 23:23:11.000000 cbcmgr-2.2.8/cbcmgr/cb_bucket.py
--rw-r--r--   0 michael    (501) staff       (20)    23151 2024-01-24 01:34:14.000000 cbcmgr-2.2.8/cbcmgr/cb_capella.py
--rw-r--r--   0 michael    (501) staff       (20)     4456 2024-01-18 21:17:37.000000 cbcmgr-2.2.8/cbcmgr/cb_capella_config.py
--rw-r--r--   0 michael    (501) staff       (20)      254 2023-10-06 19:41:34.000000 cbcmgr-2.2.8/cbcmgr/cb_collection.py
--rw-r--r--   0 michael    (501) staff       (20)    11060 2023-11-10 20:00:42.000000 cbcmgr-2.2.8/cbcmgr/cb_connect.py
--rw-r--r--   0 michael    (501) staff       (20)    19073 2024-01-29 23:30:53.000000 cbcmgr-2.2.8/cbcmgr/cb_connect_lite.py
--rw-r--r--   0 michael    (501) staff       (20)    12024 2024-01-29 23:30:53.000000 cbcmgr-2.2.8/cbcmgr/cb_connect_lite_a.py
--rw-r--r--   0 michael    (501) staff       (20)     1443 2023-10-06 18:31:32.000000 cbcmgr-2.2.8/cbcmgr/cb_index.py
--rw-r--r--   0 michael    (501) staff       (20)    29575 2024-01-29 22:20:39.000000 cbcmgr-2.2.8/cbcmgr/cb_management.py
--rw-r--r--   0 michael    (501) staff       (20)     7497 2024-01-30 00:09:39.000000 cbcmgr-2.2.8/cbcmgr/cb_operation_a.py
--rw-r--r--   0 michael    (501) staff       (20)     7967 2024-01-30 03:00:09.000000 cbcmgr-2.2.8/cbcmgr/cb_operation_s.py
--rw-r--r--   0 michael    (501) staff       (20)     3881 2023-07-12 13:52:42.000000 cbcmgr-2.2.8/cbcmgr/cb_pathmap.py
--rw-r--r--   0 michael    (501) staff       (20)      817 2023-10-09 22:38:36.000000 cbcmgr-2.2.8/cbcmgr/cb_rbac.py
--rw-r--r--   0 michael    (501) staff       (20)    13512 2023-11-10 20:16:13.000000 cbcmgr-2.2.8/cbcmgr/cb_session.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-01-30 03:06:10.347169 cbcmgr-2.2.8/cbcmgr/cli/
--rw-r--r--   0 michael    (501) staff       (20)       20 2023-09-21 22:49:06.000000 cbcmgr-2.2.8/cbcmgr/cli/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)    17136 2024-01-30 02:50:51.000000 cbcmgr-2.2.8/cbcmgr/cli/caputil.py
--rw-r--r--   0 michael    (501) staff       (20)     7498 2023-11-10 19:37:42.000000 cbcmgr-2.2.8/cbcmgr/cli/cbcutil.py
--rw-r--r--   0 michael    (501) staff       (20)     4953 2024-01-19 18:26:30.000000 cbcmgr-2.2.8/cbcmgr/cli/cli.py
--rw-r--r--   0 michael    (501) staff       (20)     4954 2023-09-28 16:25:51.000000 cbcmgr-2.2.8/cbcmgr/cli/config.py
--rw-r--r--   0 michael    (501) staff       (20)      388 2023-09-21 22:02:04.000000 cbcmgr-2.2.8/cbcmgr/cli/constants.py
--rw-r--r--   0 michael    (501) staff       (20)     1719 2023-10-06 15:30:45.000000 cbcmgr-2.2.8/cbcmgr/cli/exceptions.py
--rw-r--r--   0 michael    (501) staff       (20)     3296 2023-10-06 20:45:10.000000 cbcmgr-2.2.8/cbcmgr/cli/exec_step.py
--rw-r--r--   0 michael    (501) staff       (20)     4056 2023-09-21 23:01:23.000000 cbcmgr-2.2.8/cbcmgr/cli/export.py
--rw-r--r--   0 michael    (501) staff       (20)     1661 2023-09-21 23:01:23.000000 cbcmgr-2.2.8/cbcmgr/cli/keyformat.py
--rw-r--r--   0 michael    (501) staff       (20)    15655 2023-10-17 19:17:36.000000 cbcmgr-2.2.8/cbcmgr/cli/main.py
--rw-r--r--   0 michael    (501) staff       (20)     1230 2023-09-21 22:49:06.000000 cbcmgr-2.2.8/cbcmgr/cli/mptools.py
--rw-r--r--   0 michael    (501) staff       (20)     4457 2023-09-21 23:04:09.000000 cbcmgr-2.2.8/cbcmgr/cli/pimport.py
--rw-r--r--   0 michael    (501) staff       (20)    15069 2023-09-22 13:46:36.000000 cbcmgr-2.2.8/cbcmgr/cli/randomize.py
--rw-r--r--   0 michael    (501) staff       (20)     1311 2023-09-22 13:50:05.000000 cbcmgr-2.2.8/cbcmgr/cli/relational.py
--rw-r--r--   0 michael    (501) staff       (20)     9788 2024-01-30 02:37:51.000000 cbcmgr-2.2.8/cbcmgr/cli/replicate.py
--rw-r--r--   0 michael    (501) staff       (20)    10495 2023-10-10 22:07:26.000000 cbcmgr-2.2.8/cbcmgr/cli/schema.py
--rwxr-xr-x   0 michael    (501) staff       (20)    21916 2023-11-10 20:16:13.000000 cbcmgr-2.2.8/cbcmgr/cli/sgwutil.py
--rw-r--r--   0 michael    (501) staff       (20)     2184 2024-01-19 18:23:11.000000 cbcmgr-2.2.8/cbcmgr/cli/system.py
--rw-r--r--   0 michael    (501) staff       (20)     2021 2023-07-07 19:01:23.000000 cbcmgr-2.2.8/cbcmgr/config.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-01-30 03:06:10.349002 cbcmgr-2.2.8/cbcmgr/data/
--rw-r--r--   0 michael    (501) staff       (20)   152441 2023-09-21 21:33:24.000000 cbcmgr-2.2.8/cbcmgr/data/data.json
--rw-r--r--   0 michael    (501) staff       (20)    23312 2023-10-10 22:06:12.000000 cbcmgr-2.2.8/cbcmgr/data/schema.json
--rw-r--r--   0 michael    (501) staff       (20)     5103 2023-10-10 22:44:47.000000 cbcmgr-2.2.8/cbcmgr/exceptions.py
--rw-r--r--   0 michael    (501) staff       (20)    12821 2024-01-18 15:18:27.000000 cbcmgr-2.2.8/cbcmgr/httpsessionmgr.py
--rw-r--r--   0 michael    (501) staff       (20)      938 2023-07-12 01:28:33.000000 cbcmgr-2.2.8/cbcmgr/id_format.py
--rw-r--r--   0 michael    (501) staff       (20)     3250 2023-07-14 18:20:35.000000 cbcmgr-2.2.8/cbcmgr/mt_pool.py
--rw-r--r--   0 michael    (501) staff       (20)    11351 2024-01-30 02:20:41.000000 cbcmgr-2.2.8/cbcmgr/restmgr.py
--rw-r--r--   0 michael    (501) staff       (20)     2825 2023-07-07 21:38:37.000000 cbcmgr-2.2.8/cbcmgr/retry.py
--rw-r--r--   0 michael    (501) staff       (20)     7843 2023-05-02 21:24:28.000000 cbcmgr-2.2.8/cbcmgr/schema.py
--rw-r--r--   0 michael    (501) staff       (20)     1883 2023-10-17 21:56:07.000000 cbcmgr-2.2.8/cbcmgr/util.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-01-30 03:06:10.339908 cbcmgr-2.2.8/cbcmgr.egg-info/
--rw-r--r--   0 michael    (501) staff       (20)    13895 2024-01-30 03:06:10.000000 cbcmgr-2.2.8/cbcmgr.egg-info/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)     1692 2024-01-30 03:06:10.000000 cbcmgr-2.2.8/cbcmgr.egg-info/SOURCES.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2024-01-30 03:06:10.000000 cbcmgr-2.2.8/cbcmgr.egg-info/dependency_links.txt
--rw-r--r--   0 michael    (501) staff       (20)      120 2024-01-30 03:06:10.000000 cbcmgr-2.2.8/cbcmgr.egg-info/entry_points.txt
--rw-r--r--   0 michael    (501) staff       (20)      324 2024-01-30 03:06:10.000000 cbcmgr-2.2.8/cbcmgr.egg-info/requires.txt
--rw-r--r--   0 michael    (501) staff       (20)        7 2024-01-30 03:06:10.000000 cbcmgr-2.2.8/cbcmgr.egg-info/top_level.txt
--rw-r--r--   0 michael    (501) staff       (20)      325 2024-01-24 02:18:26.000000 cbcmgr-2.2.8/requirements.txt
--rw-r--r--   0 michael    (501) staff       (20)       38 2024-01-30 03:06:10.364489 cbcmgr-2.2.8/setup.cfg
--rw-r--r--   0 michael    (501) staff       (20)     1949 2024-01-24 02:18:26.000000 cbcmgr-2.2.8/setup.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-01-30 03:06:10.363797 cbcmgr-2.2.8/tests/
--rw-r--r--   0 michael    (501) staff       (20)      202 2023-09-22 20:20:26.000000 cbcmgr-2.2.8/tests/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)     9827 2023-11-11 00:32:14.000000 cbcmgr-2.2.8/tests/common.py
--rw-r--r--   0 michael    (501) staff       (20)      733 2023-11-10 22:58:25.000000 cbcmgr-2.2.8/tests/conftest.py
--rw-r--r--   0 michael    (501) staff       (20)      645 2023-09-22 19:19:42.000000 cbcmgr-2.2.8/tests/employee.js
--rw-r--r--   0 michael    (501) staff       (20)      651 2023-09-22 15:18:24.000000 cbcmgr-2.2.8/tests/input_stdin.dat
--rw-r--r--   0 michael    (501) staff       (20)     2053 2023-09-22 15:08:27.000000 cbcmgr-2.2.8/tests/input_template.json
--rw-r--r--   0 michael    (501) staff       (20)      584 2023-09-22 19:19:42.000000 cbcmgr-2.2.8/tests/insurance.js
--rw-r--r--   0 michael    (501) staff       (20)       56 2023-10-17 23:10:27.000000 cbcmgr-2.2.8/tests/pytest.ini
--rw-r--r--   0 michael    (501) staff       (20)     9974 2024-01-19 18:32:40.000000 cbcmgr-2.2.8/tests/test_1.py
--rw-r--r--   0 michael    (501) staff       (20)     7311 2024-01-19 18:32:40.000000 cbcmgr-2.2.8/tests/test_2.py
--rw-r--r--   0 michael    (501) staff       (20)    10965 2023-11-14 15:09:55.000000 cbcmgr-2.2.8/tests/test_3.py
--rw-r--r--   0 michael    (501) staff       (20)     2532 2023-11-14 15:09:55.000000 cbcmgr-2.2.8/tests/test_4.py
--rwxr-xr-x   0 michael    (501) staff       (20)    10669 2023-11-14 15:09:55.000000 cbcmgr-2.2.8/tests/test_5.py
--rwxr-xr-x   0 michael    (501) staff       (20)     2180 2024-01-30 02:02:52.000000 cbcmgr-2.2.8/tests/test_6.py
--rw-r--r--   0 michael    (501) staff       (20)     2644 2024-01-18 21:32:48.000000 cbcmgr-2.2.8/tests/test_7.py
--rwxr-xr-x   0 michael    (501) staff       (20)      349 2023-09-27 15:02:03.000000 cbcmgr-2.2.8/tests/test_cap_cli.py
--rwxr-xr-x   0 michael    (501) staff       (20)      349 2023-09-22 13:28:57.000000 cbcmgr-2.2.8/tests/test_cli.py
--rwxr-xr-x   0 michael    (501) staff       (20)     9832 2024-01-02 19:57:01.000000 cbcmgr-2.2.8/tests/test_m.py
--rwxr-xr-x   0 michael    (501) staff       (20)    12171 2023-10-06 14:52:16.000000 cbcmgr-2.2.8/tests/test_m_a.py
--rwxr-xr-x   0 michael    (501) staff       (20)     9784 2023-07-14 19:19:56.000000 cbcmgr-2.2.8/tests/test_p.py
--rwxr-xr-x   0 michael    (501) staff       (20)      349 2023-09-22 17:58:39.000000 cbcmgr-2.2.8/tests/test_sgw_cli.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-01-30 22:26:06.484546 cbcmgr-2.2.9/
+-rw-r--r--   0 michael    (501) staff       (20)      291 2024-01-30 22:25:38.000000 cbcmgr-2.2.9/.bumpversion.cfg
+-rw-r--r--   0 michael    (501) staff       (20)     3101 2023-08-26 01:02:18.000000 cbcmgr-2.2.9/.gitignore
+-rw-r--r--   0 michael    (501) staff       (20)     1074 2023-02-14 15:09:46.000000 cbcmgr-2.2.9/LICENSE.txt
+-rw-r--r--   0 michael    (501) staff       (20)     1270 2024-01-18 15:25:57.000000 cbcmgr-2.2.9/Makefile
+-rw-r--r--   0 michael    (501) staff       (20)    13895 2024-01-30 22:26:06.484342 cbcmgr-2.2.9/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)    13096 2024-01-30 22:25:38.000000 cbcmgr-2.2.9/README.md
+-rw-r--r--   0 michael    (501) staff       (20)        6 2024-01-30 22:25:38.000000 cbcmgr-2.2.9/VERSION
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-01-30 22:26:06.456939 cbcmgr-2.2.9/cbcmgr/
+-rw-r--r--   0 michael    (501) staff       (20)      235 2024-01-30 22:25:38.000000 cbcmgr-2.2.9/cbcmgr/__init__.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-01-30 22:26:06.458893 cbcmgr-2.2.9/cbcmgr/api/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2023-09-28 20:20:23.000000 cbcmgr-2.2.9/cbcmgr/api/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)     1221 2023-09-28 20:51:47.000000 cbcmgr-2.2.9/cbcmgr/api/load.py
+-rw-r--r--   0 michael    (501) staff       (20)     3180 2023-12-20 22:26:35.000000 cbcmgr-2.2.9/cbcmgr/async_pool.py
+-rw-r--r--   0 michael    (501) staff       (20)     3377 2024-01-29 23:23:11.000000 cbcmgr-2.2.9/cbcmgr/cb_bucket.py
+-rw-r--r--   0 michael    (501) staff       (20)    23361 2024-01-30 22:25:32.000000 cbcmgr-2.2.9/cbcmgr/cb_capella.py
+-rw-r--r--   0 michael    (501) staff       (20)     4456 2024-01-18 21:17:37.000000 cbcmgr-2.2.9/cbcmgr/cb_capella_config.py
+-rw-r--r--   0 michael    (501) staff       (20)      254 2023-10-06 19:41:34.000000 cbcmgr-2.2.9/cbcmgr/cb_collection.py
+-rw-r--r--   0 michael    (501) staff       (20)    11060 2023-11-10 20:00:42.000000 cbcmgr-2.2.9/cbcmgr/cb_connect.py
+-rw-r--r--   0 michael    (501) staff       (20)    19073 2024-01-29 23:30:53.000000 cbcmgr-2.2.9/cbcmgr/cb_connect_lite.py
+-rw-r--r--   0 michael    (501) staff       (20)    12024 2024-01-29 23:30:53.000000 cbcmgr-2.2.9/cbcmgr/cb_connect_lite_a.py
+-rw-r--r--   0 michael    (501) staff       (20)     1443 2023-10-06 18:31:32.000000 cbcmgr-2.2.9/cbcmgr/cb_index.py
+-rw-r--r--   0 michael    (501) staff       (20)    29575 2024-01-29 22:20:39.000000 cbcmgr-2.2.9/cbcmgr/cb_management.py
+-rw-r--r--   0 michael    (501) staff       (20)     7497 2024-01-30 00:09:39.000000 cbcmgr-2.2.9/cbcmgr/cb_operation_a.py
+-rw-r--r--   0 michael    (501) staff       (20)     7967 2024-01-30 03:00:09.000000 cbcmgr-2.2.9/cbcmgr/cb_operation_s.py
+-rw-r--r--   0 michael    (501) staff       (20)     3881 2023-07-12 13:52:42.000000 cbcmgr-2.2.9/cbcmgr/cb_pathmap.py
+-rw-r--r--   0 michael    (501) staff       (20)      817 2023-10-09 22:38:36.000000 cbcmgr-2.2.9/cbcmgr/cb_rbac.py
+-rw-r--r--   0 michael    (501) staff       (20)    13512 2023-11-10 20:16:13.000000 cbcmgr-2.2.9/cbcmgr/cb_session.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-01-30 22:26:06.472884 cbcmgr-2.2.9/cbcmgr/cli/
+-rw-r--r--   0 michael    (501) staff       (20)       20 2023-09-21 22:49:06.000000 cbcmgr-2.2.9/cbcmgr/cli/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)    17136 2024-01-30 02:50:51.000000 cbcmgr-2.2.9/cbcmgr/cli/caputil.py
+-rw-r--r--   0 michael    (501) staff       (20)     7498 2023-11-10 19:37:42.000000 cbcmgr-2.2.9/cbcmgr/cli/cbcutil.py
+-rw-r--r--   0 michael    (501) staff       (20)     4953 2024-01-19 18:26:30.000000 cbcmgr-2.2.9/cbcmgr/cli/cli.py
+-rw-r--r--   0 michael    (501) staff       (20)     4954 2023-09-28 16:25:51.000000 cbcmgr-2.2.9/cbcmgr/cli/config.py
+-rw-r--r--   0 michael    (501) staff       (20)      388 2023-09-21 22:02:04.000000 cbcmgr-2.2.9/cbcmgr/cli/constants.py
+-rw-r--r--   0 michael    (501) staff       (20)     1719 2023-10-06 15:30:45.000000 cbcmgr-2.2.9/cbcmgr/cli/exceptions.py
+-rw-r--r--   0 michael    (501) staff       (20)     3296 2023-10-06 20:45:10.000000 cbcmgr-2.2.9/cbcmgr/cli/exec_step.py
+-rw-r--r--   0 michael    (501) staff       (20)     4056 2023-09-21 23:01:23.000000 cbcmgr-2.2.9/cbcmgr/cli/export.py
+-rw-r--r--   0 michael    (501) staff       (20)     1661 2023-09-21 23:01:23.000000 cbcmgr-2.2.9/cbcmgr/cli/keyformat.py
+-rw-r--r--   0 michael    (501) staff       (20)    15655 2023-10-17 19:17:36.000000 cbcmgr-2.2.9/cbcmgr/cli/main.py
+-rw-r--r--   0 michael    (501) staff       (20)     1230 2023-09-21 22:49:06.000000 cbcmgr-2.2.9/cbcmgr/cli/mptools.py
+-rw-r--r--   0 michael    (501) staff       (20)     4457 2023-09-21 23:04:09.000000 cbcmgr-2.2.9/cbcmgr/cli/pimport.py
+-rw-r--r--   0 michael    (501) staff       (20)    15069 2023-09-22 13:46:36.000000 cbcmgr-2.2.9/cbcmgr/cli/randomize.py
+-rw-r--r--   0 michael    (501) staff       (20)     1311 2023-09-22 13:50:05.000000 cbcmgr-2.2.9/cbcmgr/cli/relational.py
+-rw-r--r--   0 michael    (501) staff       (20)     9788 2024-01-30 02:37:51.000000 cbcmgr-2.2.9/cbcmgr/cli/replicate.py
+-rw-r--r--   0 michael    (501) staff       (20)    10495 2023-10-10 22:07:26.000000 cbcmgr-2.2.9/cbcmgr/cli/schema.py
+-rwxr-xr-x   0 michael    (501) staff       (20)    21916 2023-11-10 20:16:13.000000 cbcmgr-2.2.9/cbcmgr/cli/sgwutil.py
+-rw-r--r--   0 michael    (501) staff       (20)     2184 2024-01-19 18:23:11.000000 cbcmgr-2.2.9/cbcmgr/cli/system.py
+-rw-r--r--   0 michael    (501) staff       (20)     2021 2023-07-07 19:01:23.000000 cbcmgr-2.2.9/cbcmgr/config.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-01-30 22:26:06.474310 cbcmgr-2.2.9/cbcmgr/data/
+-rw-r--r--   0 michael    (501) staff       (20)   152441 2023-09-21 21:33:24.000000 cbcmgr-2.2.9/cbcmgr/data/data.json
+-rw-r--r--   0 michael    (501) staff       (20)    23312 2023-10-10 22:06:12.000000 cbcmgr-2.2.9/cbcmgr/data/schema.json
+-rw-r--r--   0 michael    (501) staff       (20)     5103 2023-10-10 22:44:47.000000 cbcmgr-2.2.9/cbcmgr/exceptions.py
+-rw-r--r--   0 michael    (501) staff       (20)    12821 2024-01-18 15:18:27.000000 cbcmgr-2.2.9/cbcmgr/httpsessionmgr.py
+-rw-r--r--   0 michael    (501) staff       (20)      938 2023-07-12 01:28:33.000000 cbcmgr-2.2.9/cbcmgr/id_format.py
+-rw-r--r--   0 michael    (501) staff       (20)     3250 2023-07-14 18:20:35.000000 cbcmgr-2.2.9/cbcmgr/mt_pool.py
+-rw-r--r--   0 michael    (501) staff       (20)    11351 2024-01-30 02:20:41.000000 cbcmgr-2.2.9/cbcmgr/restmgr.py
+-rw-r--r--   0 michael    (501) staff       (20)     2825 2023-07-07 21:38:37.000000 cbcmgr-2.2.9/cbcmgr/retry.py
+-rw-r--r--   0 michael    (501) staff       (20)     7843 2023-05-02 21:24:28.000000 cbcmgr-2.2.9/cbcmgr/schema.py
+-rw-r--r--   0 michael    (501) staff       (20)     1883 2023-10-17 21:56:07.000000 cbcmgr-2.2.9/cbcmgr/util.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-01-30 22:26:06.458164 cbcmgr-2.2.9/cbcmgr.egg-info/
+-rw-r--r--   0 michael    (501) staff       (20)    13895 2024-01-30 22:26:06.000000 cbcmgr-2.2.9/cbcmgr.egg-info/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)     1692 2024-01-30 22:26:06.000000 cbcmgr-2.2.9/cbcmgr.egg-info/SOURCES.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2024-01-30 22:26:06.000000 cbcmgr-2.2.9/cbcmgr.egg-info/dependency_links.txt
+-rw-r--r--   0 michael    (501) staff       (20)      120 2024-01-30 22:26:06.000000 cbcmgr-2.2.9/cbcmgr.egg-info/entry_points.txt
+-rw-r--r--   0 michael    (501) staff       (20)      324 2024-01-30 22:26:06.000000 cbcmgr-2.2.9/cbcmgr.egg-info/requires.txt
+-rw-r--r--   0 michael    (501) staff       (20)        7 2024-01-30 22:26:06.000000 cbcmgr-2.2.9/cbcmgr.egg-info/top_level.txt
+-rw-r--r--   0 michael    (501) staff       (20)      325 2024-01-24 02:18:26.000000 cbcmgr-2.2.9/requirements.txt
+-rw-r--r--   0 michael    (501) staff       (20)       38 2024-01-30 22:26:06.484600 cbcmgr-2.2.9/setup.cfg
+-rw-r--r--   0 michael    (501) staff       (20)     1949 2024-01-24 02:18:26.000000 cbcmgr-2.2.9/setup.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-01-30 22:26:06.483783 cbcmgr-2.2.9/tests/
+-rw-r--r--   0 michael    (501) staff       (20)      202 2023-09-22 20:20:26.000000 cbcmgr-2.2.9/tests/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)     9827 2023-11-11 00:32:14.000000 cbcmgr-2.2.9/tests/common.py
+-rw-r--r--   0 michael    (501) staff       (20)      733 2023-11-10 22:58:25.000000 cbcmgr-2.2.9/tests/conftest.py
+-rw-r--r--   0 michael    (501) staff       (20)      645 2023-09-22 19:19:42.000000 cbcmgr-2.2.9/tests/employee.js
+-rw-r--r--   0 michael    (501) staff       (20)      651 2023-09-22 15:18:24.000000 cbcmgr-2.2.9/tests/input_stdin.dat
+-rw-r--r--   0 michael    (501) staff       (20)     2053 2023-09-22 15:08:27.000000 cbcmgr-2.2.9/tests/input_template.json
+-rw-r--r--   0 michael    (501) staff       (20)      584 2023-09-22 19:19:42.000000 cbcmgr-2.2.9/tests/insurance.js
+-rw-r--r--   0 michael    (501) staff       (20)       56 2023-10-17 23:10:27.000000 cbcmgr-2.2.9/tests/pytest.ini
+-rw-r--r--   0 michael    (501) staff       (20)     9974 2024-01-19 18:32:40.000000 cbcmgr-2.2.9/tests/test_1.py
+-rw-r--r--   0 michael    (501) staff       (20)     7311 2024-01-19 18:32:40.000000 cbcmgr-2.2.9/tests/test_2.py
+-rw-r--r--   0 michael    (501) staff       (20)    10965 2023-11-14 15:09:55.000000 cbcmgr-2.2.9/tests/test_3.py
+-rw-r--r--   0 michael    (501) staff       (20)     2532 2023-11-14 15:09:55.000000 cbcmgr-2.2.9/tests/test_4.py
+-rwxr-xr-x   0 michael    (501) staff       (20)    10669 2023-11-14 15:09:55.000000 cbcmgr-2.2.9/tests/test_5.py
+-rwxr-xr-x   0 michael    (501) staff       (20)     2180 2024-01-30 02:02:52.000000 cbcmgr-2.2.9/tests/test_6.py
+-rw-r--r--   0 michael    (501) staff       (20)     2644 2024-01-18 21:32:48.000000 cbcmgr-2.2.9/tests/test_7.py
+-rwxr-xr-x   0 michael    (501) staff       (20)      349 2023-09-27 15:02:03.000000 cbcmgr-2.2.9/tests/test_cap_cli.py
+-rwxr-xr-x   0 michael    (501) staff       (20)      349 2023-09-22 13:28:57.000000 cbcmgr-2.2.9/tests/test_cli.py
+-rwxr-xr-x   0 michael    (501) staff       (20)     9832 2024-01-02 19:57:01.000000 cbcmgr-2.2.9/tests/test_m.py
+-rwxr-xr-x   0 michael    (501) staff       (20)    12171 2023-10-06 14:52:16.000000 cbcmgr-2.2.9/tests/test_m_a.py
+-rwxr-xr-x   0 michael    (501) staff       (20)     9784 2023-07-14 19:19:56.000000 cbcmgr-2.2.9/tests/test_p.py
+-rwxr-xr-x   0 michael    (501) staff       (20)      349 2023-09-22 17:58:39.000000 cbcmgr-2.2.9/tests/test_sgw_cli.py
```

### Comparing `cbcmgr-2.2.8/.gitignore` & `cbcmgr-2.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `cbcmgr-2.2.8/LICENSE.txt` & `cbcmgr-2.2.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cbcmgr-2.2.8/Makefile` & `cbcmgr-2.2.9/Makefile`

 * *Files identical despite different names*

### Comparing `cbcmgr-2.2.8/PKG-INFO` & `cbcmgr-2.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbcmgr
-Version: 2.2.8
+Version: 2.2.9
 Summary: Couchbase connection manager
 Home-page: https://github.com/mminichino/cb-util
 Author: Michael Minichino
 Author-email: info@unix.us.com
 License: MIT License
 Keywords: couchbase,nosql,pycouchbase,database
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,15 +16,15 @@
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# cb-util 2.2.8
+# cb-util 2.2.9
 
 ## Couchbase Utilities
 Couchbase connection manager. Simplifies connecting to a Couchbase cluster and performing data and management operations.
 
 ## Installing
 ```
 $ pip install cbcmgr
```

### Comparing `cbcmgr-2.2.8/README.md` & `cbcmgr-2.2.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# cb-util 2.2.8
+# cb-util 2.2.9
 
 ## Couchbase Utilities
 Couchbase connection manager. Simplifies connecting to a Couchbase cluster and performing data and management operations.
 
 ## Installing
 ```
 $ pip install cbcmgr
```

### Comparing `cbcmgr-2.2.8/cbcmgr/api/load.py` & `cbcmgr-2.2.9/cbcmgr/api/load.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-2.2.8/cbcmgr/async_pool.py` & `cbcmgr-2.2.9/cbcmgr/async_pool.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-2.2.8/cbcmgr/cb_bucket.py` & `cbcmgr-2.2.9/cbcmgr/cb_bucket.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-2.2.8/cbcmgr/cb_capella.py` & `cbcmgr-2.2.9/cbcmgr/cb_capella.py`

 * *Files 1% similar despite different names*

```diff
@@ -520,14 +520,18 @@
 
     def list_clusters(self):
         return self.rest.get_capella(f"/v4/organizations/{self.organization_id}/projects/{self.project_id}/clusters").list()
 
     def get_cluster(self, name):
         return self.rest.get_capella(f"/v4/organizations/{self.organization_id}/projects/{self.project_id}/clusters").by_name(name).unique().record()
 
+    def get_cluster_by_id(self, cluster_id: str):
+        url = f"/v4/organizations/{self.organization_id}/projects/{self.project_id}/clusters/{cluster_id}"
+        return self.rest.get(url).validate().json()
+
     def create_cluster(self, cluster: CapellaCluster):
         cidr_util = NetworkDriver()
         # noinspection PyTypeChecker
         parameters = attrs.asdict(cluster)
         cluster_cidr = cluster.cloudProvider.cidr
         cidr_util.add_network(cluster_cidr)
         cidr_util.get_next_network()
```

### Comparing `cbcmgr-2.2.8/cbcmgr/cb_capella_config.py` & `cbcmgr-2.2.9/cbcmgr/cb_capella_config.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-2.2.8/cbcmgr/cb_connect.py` & `cbcmgr-2.2.9/cbcmgr/cb_connect.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-2.2.8/cbcmgr/cb_connect_lite.py` & `cbcmgr-2.2.9/cbcmgr/cb_connect_lite.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-2.2.8/cbcmgr/cb_connect_lite_a.py` & `cbcmgr-2.2.9/cbcmgr/cb_connect_lite_a.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-2.2.8/cbcmgr/cb_index.py` & `cbcmgr-2.2.9/cbcmgr/cb_index.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-2.2.8/cbcmgr/cb_management.py` & `cbcmgr-2.2.9/cbcmgr/cb_management.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-2.2.8/cbcmgr/cb_operation_a.py` & `cbcmgr-2.2.9/cbcmgr/cb_operation_a.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-2.2.8/cbcmgr/cb_operation_s.py` & `cbcmgr-2.2.9/cbcmgr/cb_operation_s.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-2.2.8/cbcmgr/cb_pathmap.py` & `cbcmgr-2.2.9/cbcmgr/cb_pathmap.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-2.2.8/cbcmgr/cb_rbac.py` & `cbcmgr-2.2.9/cbcmgr/cb_rbac.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-2.2.8/cbcmgr/cb_session.py` & `cbcmgr-2.2.9/cbcmgr/cb_session.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-2.2.8/cbcmgr/cli/caputil.py` & `cbcmgr-2.2.9/cbcmgr/cli/caputil.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-2.2.8/cbcmgr/cli/cbcutil.py` & `cbcmgr-2.2.9/cbcmgr/cli/cbcutil.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-2.2.8/cbcmgr/cli/cli.py` & `cbcmgr-2.2.9/cbcmgr/cli/cli.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-2.2.8/cbcmgr/cli/config.py` & `cbcmgr-2.2.9/cbcmgr/cli/config.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-2.2.8/cbcmgr/cli/exceptions.py` & `cbcmgr-2.2.9/cbcmgr/cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-2.2.8/cbcmgr/cli/exec_step.py` & `cbcmgr-2.2.9/cbcmgr/cli/exec_step.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-2.2.8/cbcmgr/cli/export.py` & `cbcmgr-2.2.9/cbcmgr/cli/export.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-2.2.8/cbcmgr/cli/keyformat.py` & `cbcmgr-2.2.9/cbcmgr/cli/keyformat.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-2.2.8/cbcmgr/cli/main.py` & `cbcmgr-2.2.9/cbcmgr/cli/main.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-2.2.8/cbcmgr/cli/mptools.py` & `cbcmgr-2.2.9/cbcmgr/cli/mptools.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-2.2.8/cbcmgr/cli/pimport.py` & `cbcmgr-2.2.9/cbcmgr/cli/pimport.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-2.2.8/cbcmgr/cli/randomize.py` & `cbcmgr-2.2.9/cbcmgr/cli/randomize.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-2.2.8/cbcmgr/cli/relational.py` & `cbcmgr-2.2.9/cbcmgr/cli/relational.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-2.2.8/cbcmgr/cli/replicate.py` & `cbcmgr-2.2.9/cbcmgr/cli/replicate.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-2.2.8/cbcmgr/cli/schema.py` & `cbcmgr-2.2.9/cbcmgr/cli/schema.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-2.2.8/cbcmgr/cli/sgwutil.py` & `cbcmgr-2.2.9/cbcmgr/cli/sgwutil.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-2.2.8/cbcmgr/cli/system.py` & `cbcmgr-2.2.9/cbcmgr/cli/system.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-2.2.8/cbcmgr/config.py` & `cbcmgr-2.2.9/cbcmgr/config.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-2.2.8/cbcmgr/data/data.json` & `cbcmgr-2.2.9/cbcmgr/data/data.json`

 * *Files identical despite different names*

### Comparing `cbcmgr-2.2.8/cbcmgr/data/schema.json` & `cbcmgr-2.2.9/cbcmgr/data/schema.json`

 * *Files identical despite different names*

### Comparing `cbcmgr-2.2.8/cbcmgr/exceptions.py` & `cbcmgr-2.2.9/cbcmgr/exceptions.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-2.2.8/cbcmgr/httpsessionmgr.py` & `cbcmgr-2.2.9/cbcmgr/httpsessionmgr.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-2.2.8/cbcmgr/id_format.py` & `cbcmgr-2.2.9/cbcmgr/id_format.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-2.2.8/cbcmgr/mt_pool.py` & `cbcmgr-2.2.9/cbcmgr/mt_pool.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-2.2.8/cbcmgr/restmgr.py` & `cbcmgr-2.2.9/cbcmgr/restmgr.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-2.2.8/cbcmgr/retry.py` & `cbcmgr-2.2.9/cbcmgr/retry.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-2.2.8/cbcmgr/schema.py` & `cbcmgr-2.2.9/cbcmgr/schema.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-2.2.8/cbcmgr/util.py` & `cbcmgr-2.2.9/cbcmgr/util.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-2.2.8/cbcmgr.egg-info/PKG-INFO` & `cbcmgr-2.2.9/cbcmgr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbcmgr
-Version: 2.2.8
+Version: 2.2.9
 Summary: Couchbase connection manager
 Home-page: https://github.com/mminichino/cb-util
 Author: Michael Minichino
 Author-email: info@unix.us.com
 License: MIT License
 Keywords: couchbase,nosql,pycouchbase,database
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,15 +16,15 @@
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# cb-util 2.2.8
+# cb-util 2.2.9
 
 ## Couchbase Utilities
 Couchbase connection manager. Simplifies connecting to a Couchbase cluster and performing data and management operations.
 
 ## Installing
 ```
 $ pip install cbcmgr
```

### Comparing `cbcmgr-2.2.8/cbcmgr.egg-info/SOURCES.txt` & `cbcmgr-2.2.9/cbcmgr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cbcmgr-2.2.8/setup.py` & `cbcmgr-2.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-2.2.8/tests/common.py` & `cbcmgr-2.2.9/tests/common.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-2.2.8/tests/conftest.py` & `cbcmgr-2.2.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-2.2.8/tests/employee.js` & `cbcmgr-2.2.9/tests/employee.js`

 * *Files identical despite different names*

### Comparing `cbcmgr-2.2.8/tests/input_stdin.dat` & `cbcmgr-2.2.9/tests/input_stdin.dat`

 * *Files identical despite different names*

### Comparing `cbcmgr-2.2.8/tests/input_template.json` & `cbcmgr-2.2.9/tests/input_template.json`

 * *Files identical despite different names*

### Comparing `cbcmgr-2.2.8/tests/insurance.js` & `cbcmgr-2.2.9/tests/insurance.js`

 * *Files identical despite different names*

### Comparing `cbcmgr-2.2.8/tests/test_1.py` & `cbcmgr-2.2.9/tests/test_1.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-2.2.8/tests/test_2.py` & `cbcmgr-2.2.9/tests/test_2.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-2.2.8/tests/test_3.py` & `cbcmgr-2.2.9/tests/test_3.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-2.2.8/tests/test_4.py` & `cbcmgr-2.2.9/tests/test_4.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-2.2.8/tests/test_5.py` & `cbcmgr-2.2.9/tests/test_5.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-2.2.8/tests/test_6.py` & `cbcmgr-2.2.9/tests/test_6.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-2.2.8/tests/test_7.py` & `cbcmgr-2.2.9/tests/test_7.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-2.2.8/tests/test_m.py` & `cbcmgr-2.2.9/tests/test_m.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-2.2.8/tests/test_m_a.py` & `cbcmgr-2.2.9/tests/test_m_a.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-2.2.8/tests/test_p.py` & `cbcmgr-2.2.9/tests/test_p.py`

 * *Files identical despite different names*

