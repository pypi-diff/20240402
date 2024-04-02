# Comparing `tmp/blissdata-1.0.2.tar.gz` & `tmp/blissdata-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blissdata-1.0.2.tar", last modified: Fri Feb 23 12:37:43 2024, max compression
+gzip compressed data, was "blissdata-1.0.3.tar", last modified: Wed Mar  6 15:51:38 2024, max compression
```

## Comparing `blissdata-1.0.2.tar` & `blissdata-1.0.3.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-23 12:37:43.639915 blissdata-1.0.2/
--rw-rw-rw-   0 root         (0) root         (0)     7651 2024-02-21 14:11:54.000000 blissdata-1.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1478 2024-02-23 12:37:43.639915 blissdata-1.0.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      115 2024-02-21 14:11:54.000000 blissdata-1.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-23 12:37:43.623915 blissdata-1.0.2/blissdata/
--rw-rw-rw-   0 root         (0) root         (0)      198 2024-02-23 12:36:29.000000 blissdata-1.0.2/blissdata/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-23 12:37:43.627915 blissdata-1.0.2/blissdata/beacon/
--rw-rw-rw-   0 root         (0) root         (0)       27 2024-02-21 14:11:54.000000 blissdata-1.0.2/blissdata/beacon/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3477 2024-02-21 14:11:54.000000 blissdata-1.0.2/blissdata/beacon/_base.py
--rw-rw-rw-   0 root         (0) root         (0)      682 2024-02-21 14:11:54.000000 blissdata-1.0.2/blissdata/beacon/config.py
--rw-rw-rw-   0 root         (0) root         (0)     2109 2024-02-21 14:11:54.000000 blissdata-1.0.2/blissdata/beacon/data.py
--rw-rw-rw-   0 root         (0) root         (0)     4435 2024-02-21 14:11:54.000000 blissdata-1.0.2/blissdata/beacon/files.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-23 12:37:43.627915 blissdata-1.0.2/blissdata/h5api/
--rw-rw-rw-   0 root         (0) root         (0)       68 2024-02-21 14:11:54.000000 blissdata-1.0.2/blissdata/h5api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1867 2024-02-21 14:11:54.000000 blissdata-1.0.2/blissdata/h5api/abstract.py
--rw-rw-rw-   0 root         (0) root         (0)     4464 2024-02-21 14:11:54.000000 blissdata-1.0.2/blissdata/h5api/dynamic_hdf5.py
--rw-rw-rw-   0 root         (0) root         (0)      757 2024-02-21 14:11:54.000000 blissdata-1.0.2/blissdata/h5api/file_arguments.py
--rw-rw-rw-   0 root         (0) root         (0)     3458 2024-02-21 14:11:54.000000 blissdata-1.0.2/blissdata/h5api/static_hdf5.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-23 12:37:43.627915 blissdata-1.0.2/blissdata/h5api/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-23 12:36:29.000000 blissdata-1.0.2/blissdata/h5api/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4726 2024-02-21 14:11:54.000000 blissdata-1.0.2/blissdata/h5api/utils/bliss.py
--rw-rw-rw-   0 root         (0) root         (0)     8268 2024-02-21 14:11:54.000000 blissdata-1.0.2/blissdata/h5api/utils/hdf5.py
--rw-rw-rw-   0 root         (0) root         (0)     2572 2024-02-21 14:11:54.000000 blissdata-1.0.2/blissdata/h5api/utils/hdf5_retry.py
--rw-rw-rw-   0 root         (0) root         (0)     8634 2024-02-21 14:11:54.000000 blissdata-1.0.2/blissdata/h5api/utils/lima.py
--rw-rw-rw-   0 root         (0) root         (0)      423 2024-02-21 14:11:54.000000 blissdata-1.0.2/blissdata/h5api/utils/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-23 12:37:43.627915 blissdata-1.0.2/blissdata/lima/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-23 12:36:29.000000 blissdata-1.0.2/blissdata/lima/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13089 2024-02-21 14:11:54.000000 blissdata-1.0.2/blissdata/lima/client.py
--rw-rw-rw-   0 root         (0) root         (0)    14000 2024-02-21 14:11:54.000000 blissdata-1.0.2/blissdata/lima/image_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-23 12:37:43.631915 blissdata-1.0.2/blissdata/redis_engine/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-23 12:36:29.000000 blissdata-1.0.2/blissdata/redis_engine/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-23 12:37:43.631915 blissdata-1.0.2/blissdata/redis_engine/encoding/
--rw-rw-rw-   0 root         (0) root         (0)     1193 2024-02-21 14:11:54.000000 blissdata-1.0.2/blissdata/redis_engine/encoding/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      714 2024-02-21 14:11:54.000000 blissdata-1.0.2/blissdata/redis_engine/encoding/json.py
--rw-rw-rw-   0 root         (0) root         (0)     5096 2024-02-21 14:11:54.000000 blissdata-1.0.2/blissdata/redis_engine/encoding/numeric.py
--rw-rw-rw-   0 root         (0) root         (0)     1017 2024-02-21 14:11:54.000000 blissdata-1.0.2/blissdata/redis_engine/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1122 2024-02-21 14:11:54.000000 blissdata-1.0.2/blissdata/redis_engine/identities.py
--rw-rw-rw-   0 root         (0) root         (0)    12437 2024-02-21 14:11:54.000000 blissdata-1.0.2/blissdata/redis_engine/memory_tracker.py
--rw-rw-rw-   0 root         (0) root         (0)    11592 2024-02-21 14:11:54.000000 blissdata-1.0.2/blissdata/redis_engine/scan.py
--rw-rw-rw-   0 root         (0) root         (0)    19913 2024-02-21 14:11:54.000000 blissdata-1.0.2/blissdata/redis_engine/sink.py
--rw-rw-rw-   0 root         (0) root         (0)    15515 2024-02-21 14:11:54.000000 blissdata-1.0.2/blissdata/redis_engine/store.py
--rw-rw-rw-   0 root         (0) root         (0)    19002 2024-02-21 14:11:54.000000 blissdata-1.0.2/blissdata/redis_engine/stream.py
--rw-rw-rw-   0 root         (0) root         (0)     1370 2024-02-21 14:11:54.000000 blissdata-1.0.2/blissdata/scan.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-23 12:37:43.631915 blissdata-1.0.2/blissdata/schemas/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-23 12:36:29.000000 blissdata-1.0.2/blissdata/schemas/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9673 2024-02-21 14:11:54.000000 blissdata-1.0.2/blissdata/schemas/scan_info.py
--rw-rw-rw-   0 root         (0) root         (0)     3224 2024-02-21 14:11:54.000000 blissdata-1.0.2/blissdata/schemas/scan_info_display.py
--rw-rw-rw-   0 root         (0) root         (0)     6411 2024-02-21 14:11:54.000000 blissdata-1.0.2/blissdata/stream.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-23 12:37:43.631915 blissdata-1.0.2/blissdata/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-23 12:36:29.000000 blissdata-1.0.2/blissdata/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-23 12:37:43.631915 blissdata-1.0.2/blissdata/tests/beacon/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-23 12:36:29.000000 blissdata-1.0.2/blissdata/tests/beacon/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      929 2024-02-21 14:11:54.000000 blissdata-1.0.2/blissdata/tests/beacon/test_config.py
--rw-rw-rw-   0 root         (0) root         (0)     1823 2024-02-21 14:11:54.000000 blissdata-1.0.2/blissdata/tests/beacon/test_data.py
--rw-rw-rw-   0 root         (0) root         (0)     3240 2024-02-21 14:11:54.000000 blissdata-1.0.2/blissdata/tests/beacon/test_files.py
--rw-rw-rw-   0 root         (0) root         (0)     1383 2024-02-21 14:11:54.000000 blissdata-1.0.2/blissdata/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-23 12:37:43.635915 blissdata-1.0.2/blissdata/tests/h5api/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-23 12:36:29.000000 blissdata-1.0.2/blissdata/tests/h5api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12926 2024-02-21 14:11:54.000000 blissdata-1.0.2/blissdata/tests/h5api/scanner.py
--rw-rw-rw-   0 root         (0) root         (0)    10269 2024-02-21 14:11:54.000000 blissdata-1.0.2/blissdata/tests/h5api/test_dynamic_files.py
--rw-rw-rw-   0 root         (0) root         (0)     6775 2024-02-21 14:11:54.000000 blissdata-1.0.2/blissdata/tests/h5api/test_static_files.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-23 12:37:43.635915 blissdata-1.0.2/blissdata/tests/redis_engine/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-23 12:36:29.000000 blissdata-1.0.2/blissdata/tests/redis_engine/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      310 2024-02-21 14:11:54.000000 blissdata-1.0.2/blissdata/tests/redis_engine/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-23 12:37:43.635915 blissdata-1.0.2/blissdata/tests/redis_engine/encoding/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-23 12:36:29.000000 blissdata-1.0.2/blissdata/tests/redis_engine/encoding/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6039 2024-02-21 14:11:54.000000 blissdata-1.0.2/blissdata/tests/redis_engine/encoding/test_numeric.py
--rw-rw-rw-   0 root         (0) root         (0)    17635 2024-02-21 14:11:54.000000 blissdata-1.0.2/blissdata/tests/redis_engine/test_memory_tracker.py
--rw-rw-rw-   0 root         (0) root         (0)     2759 2024-02-21 14:11:54.000000 blissdata-1.0.2/blissdata/tests/redis_engine/test_scan.py
--rw-rw-rw-   0 root         (0) root         (0)     6963 2024-02-21 14:11:54.000000 blissdata-1.0.2/blissdata/tests/redis_engine/test_search.py
--rw-rw-rw-   0 root         (0) root         (0)    20620 2024-02-21 14:11:54.000000 blissdata-1.0.2/blissdata/tests/redis_engine/test_streaming.py
--rw-rw-rw-   0 root         (0) root         (0)      719 2024-02-21 14:11:54.000000 blissdata-1.0.2/blissdata/tests/redis_engine/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-23 12:37:43.635915 blissdata-1.0.2/blissdata.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1478 2024-02-23 12:37:43.000000 blissdata-1.0.2/blissdata.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2140 2024-02-23 12:37:43.000000 blissdata-1.0.2/blissdata.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-23 12:37:43.000000 blissdata-1.0.2/blissdata.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       77 2024-02-23 12:37:43.000000 blissdata-1.0.2/blissdata.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      292 2024-02-23 12:37:43.000000 blissdata-1.0.2/blissdata.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-02-23 12:37:43.000000 blissdata-1.0.2/blissdata.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       96 2024-02-21 14:11:54.000000 blissdata-1.0.2/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1128 2024-02-23 12:37:43.639915 blissdata-1.0.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       69 2024-02-21 14:11:54.000000 blissdata-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 15:51:38.111285 blissdata-1.0.3/
+-rw-r--r--   0 root         (0) root         (0)     7651 2024-02-27 12:07:10.000000 blissdata-1.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1478 2024-03-06 15:51:38.111285 blissdata-1.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      115 2024-02-27 12:07:10.000000 blissdata-1.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 15:51:38.099285 blissdata-1.0.3/blissdata/
+-rw-rw-rw-   0 root         (0) root         (0)      198 2024-03-06 14:35:40.000000 blissdata-1.0.3/blissdata/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 15:51:38.099285 blissdata-1.0.3/blissdata/beacon/
+-rw-r--r--   0 root         (0) root         (0)       27 2024-02-27 12:07:10.000000 blissdata-1.0.3/blissdata/beacon/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3477 2024-02-27 12:07:10.000000 blissdata-1.0.3/blissdata/beacon/_base.py
+-rw-r--r--   0 root         (0) root         (0)      682 2024-02-27 12:07:10.000000 blissdata-1.0.3/blissdata/beacon/config.py
+-rw-r--r--   0 root         (0) root         (0)     2109 2024-02-27 12:07:10.000000 blissdata-1.0.3/blissdata/beacon/data.py
+-rw-r--r--   0 root         (0) root         (0)     4435 2024-02-27 12:07:10.000000 blissdata-1.0.3/blissdata/beacon/files.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 15:51:38.103285 blissdata-1.0.3/blissdata/h5api/
+-rw-r--r--   0 root         (0) root         (0)       68 2024-02-27 12:07:10.000000 blissdata-1.0.3/blissdata/h5api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1867 2024-02-27 12:07:10.000000 blissdata-1.0.3/blissdata/h5api/abstract.py
+-rw-r--r--   0 root         (0) root         (0)     4464 2024-02-27 12:07:10.000000 blissdata-1.0.3/blissdata/h5api/dynamic_hdf5.py
+-rw-r--r--   0 root         (0) root         (0)      757 2024-02-27 12:07:10.000000 blissdata-1.0.3/blissdata/h5api/file_arguments.py
+-rw-r--r--   0 root         (0) root         (0)     3458 2024-02-27 12:07:10.000000 blissdata-1.0.3/blissdata/h5api/static_hdf5.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 15:51:38.103285 blissdata-1.0.3/blissdata/h5api/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-06 15:50:37.000000 blissdata-1.0.3/blissdata/h5api/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4614 2024-03-06 13:10:42.000000 blissdata-1.0.3/blissdata/h5api/utils/bliss.py
+-rw-rw-rw-   0 root         (0) root         (0)     9281 2024-03-06 13:10:42.000000 blissdata-1.0.3/blissdata/h5api/utils/hdf5.py
+-rw-r--r--   0 root         (0) root         (0)     2572 2024-02-27 12:07:10.000000 blissdata-1.0.3/blissdata/h5api/utils/hdf5_retry.py
+-rw-r--r--   0 root         (0) root         (0)     8634 2024-02-27 12:07:10.000000 blissdata-1.0.3/blissdata/h5api/utils/lima.py
+-rw-r--r--   0 root         (0) root         (0)      423 2024-02-27 12:07:10.000000 blissdata-1.0.3/blissdata/h5api/utils/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 15:51:38.103285 blissdata-1.0.3/blissdata/lima/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-06 15:50:37.000000 blissdata-1.0.3/blissdata/lima/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13089 2024-02-27 12:07:10.000000 blissdata-1.0.3/blissdata/lima/client.py
+-rw-r--r--   0 root         (0) root         (0)    14000 2024-02-27 12:07:10.000000 blissdata-1.0.3/blissdata/lima/image_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 15:51:38.103285 blissdata-1.0.3/blissdata/redis_engine/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-06 15:50:37.000000 blissdata-1.0.3/blissdata/redis_engine/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 15:51:38.103285 blissdata-1.0.3/blissdata/redis_engine/encoding/
+-rw-r--r--   0 root         (0) root         (0)     1193 2024-02-27 12:07:10.000000 blissdata-1.0.3/blissdata/redis_engine/encoding/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      714 2024-02-27 12:07:10.000000 blissdata-1.0.3/blissdata/redis_engine/encoding/json.py
+-rw-r--r--   0 root         (0) root         (0)     5096 2024-02-27 12:07:10.000000 blissdata-1.0.3/blissdata/redis_engine/encoding/numeric.py
+-rw-r--r--   0 root         (0) root         (0)     1017 2024-02-27 12:07:10.000000 blissdata-1.0.3/blissdata/redis_engine/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     1122 2024-02-27 12:07:10.000000 blissdata-1.0.3/blissdata/redis_engine/identities.py
+-rw-r--r--   0 root         (0) root         (0)    12437 2024-02-27 12:07:10.000000 blissdata-1.0.3/blissdata/redis_engine/memory_tracker.py
+-rw-rw-rw-   0 root         (0) root         (0)    11599 2024-03-06 15:50:36.000000 blissdata-1.0.3/blissdata/redis_engine/scan.py
+-rw-r--r--   0 root         (0) root         (0)    19913 2024-02-27 12:07:10.000000 blissdata-1.0.3/blissdata/redis_engine/sink.py
+-rw-r--r--   0 root         (0) root         (0)    15515 2024-02-27 12:07:10.000000 blissdata-1.0.3/blissdata/redis_engine/store.py
+-rw-rw-rw-   0 root         (0) root         (0)    19223 2024-03-06 15:50:36.000000 blissdata-1.0.3/blissdata/redis_engine/stream.py
+-rw-r--r--   0 root         (0) root         (0)     1370 2024-02-27 12:07:10.000000 blissdata-1.0.3/blissdata/scan.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 15:51:38.107285 blissdata-1.0.3/blissdata/schemas/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-06 15:50:37.000000 blissdata-1.0.3/blissdata/schemas/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9673 2024-02-27 12:07:10.000000 blissdata-1.0.3/blissdata/schemas/scan_info.py
+-rw-r--r--   0 root         (0) root         (0)     3224 2024-02-27 12:07:10.000000 blissdata-1.0.3/blissdata/schemas/scan_info_display.py
+-rw-r--r--   0 root         (0) root         (0)     6411 2024-02-27 12:07:10.000000 blissdata-1.0.3/blissdata/stream.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 15:51:38.107285 blissdata-1.0.3/blissdata/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-06 15:50:37.000000 blissdata-1.0.3/blissdata/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 15:51:38.107285 blissdata-1.0.3/blissdata/tests/beacon/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-06 15:50:37.000000 blissdata-1.0.3/blissdata/tests/beacon/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      929 2024-02-27 12:07:10.000000 blissdata-1.0.3/blissdata/tests/beacon/test_config.py
+-rw-r--r--   0 root         (0) root         (0)     1823 2024-02-27 12:07:10.000000 blissdata-1.0.3/blissdata/tests/beacon/test_data.py
+-rw-r--r--   0 root         (0) root         (0)     3240 2024-02-27 12:07:10.000000 blissdata-1.0.3/blissdata/tests/beacon/test_files.py
+-rw-r--r--   0 root         (0) root         (0)     1383 2024-02-27 12:07:10.000000 blissdata-1.0.3/blissdata/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 15:51:38.107285 blissdata-1.0.3/blissdata/tests/h5api/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-06 15:50:37.000000 blissdata-1.0.3/blissdata/tests/h5api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12914 2024-03-06 13:10:42.000000 blissdata-1.0.3/blissdata/tests/h5api/scanner.py
+-rw-r--r--   0 root         (0) root         (0)    10269 2024-02-27 12:07:10.000000 blissdata-1.0.3/blissdata/tests/h5api/test_dynamic_files.py
+-rw-r--r--   0 root         (0) root         (0)     6775 2024-02-27 12:07:10.000000 blissdata-1.0.3/blissdata/tests/h5api/test_static_files.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 15:51:38.107285 blissdata-1.0.3/blissdata/tests/redis_engine/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-06 15:50:37.000000 blissdata-1.0.3/blissdata/tests/redis_engine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      310 2024-02-27 12:07:10.000000 blissdata-1.0.3/blissdata/tests/redis_engine/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 15:51:38.107285 blissdata-1.0.3/blissdata/tests/redis_engine/encoding/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-06 15:50:37.000000 blissdata-1.0.3/blissdata/tests/redis_engine/encoding/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6039 2024-02-27 12:07:10.000000 blissdata-1.0.3/blissdata/tests/redis_engine/encoding/test_numeric.py
+-rw-r--r--   0 root         (0) root         (0)    17635 2024-02-27 12:07:10.000000 blissdata-1.0.3/blissdata/tests/redis_engine/test_memory_tracker.py
+-rw-rw-rw-   0 root         (0) root         (0)     2759 2024-02-27 17:36:24.000000 blissdata-1.0.3/blissdata/tests/redis_engine/test_scan.py
+-rw-r--r--   0 root         (0) root         (0)     6963 2024-02-27 12:07:10.000000 blissdata-1.0.3/blissdata/tests/redis_engine/test_search.py
+-rw-rw-rw-   0 root         (0) root         (0)    21128 2024-03-06 15:50:36.000000 blissdata-1.0.3/blissdata/tests/redis_engine/test_streaming.py
+-rw-r--r--   0 root         (0) root         (0)      719 2024-02-27 12:07:10.000000 blissdata-1.0.3/blissdata/tests/redis_engine/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 15:51:38.107285 blissdata-1.0.3/blissdata.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1478 2024-03-06 15:51:38.000000 blissdata-1.0.3/blissdata.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2140 2024-03-06 15:51:38.000000 blissdata-1.0.3/blissdata.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-03-06 15:51:38.000000 blissdata-1.0.3/blissdata.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       77 2024-03-06 15:51:38.000000 blissdata-1.0.3/blissdata.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      292 2024-03-06 15:51:38.000000 blissdata-1.0.3/blissdata.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-03-06 15:51:38.000000 blissdata-1.0.3/blissdata.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       96 2024-02-27 12:07:10.000000 blissdata-1.0.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1128 2024-03-06 15:51:38.111285 blissdata-1.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       69 2024-02-27 12:07:10.000000 blissdata-1.0.3/setup.py
```

### Comparing `blissdata-1.0.2/LICENSE` & `blissdata-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `blissdata-1.0.2/PKG-INFO` & `blissdata-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blissdata
-Version: 1.0.2
+Version: 1.0.3
 Summary: Bliss data streaming client
 Home-page: https://gitlab.esrf.fr/bliss/bliss/-/tree/master/blissdata
 Author: BCU (ESRF)
 License: LGPLv3
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `blissdata-1.0.2/blissdata/beacon/_base.py` & `blissdata-1.0.3/blissdata/beacon/_base.py`

 * *Files identical despite different names*

### Comparing `blissdata-1.0.2/blissdata/beacon/config.py` & `blissdata-1.0.3/blissdata/beacon/config.py`

 * *Files identical despite different names*

### Comparing `blissdata-1.0.2/blissdata/beacon/data.py` & `blissdata-1.0.3/blissdata/beacon/data.py`

 * *Files identical despite different names*

### Comparing `blissdata-1.0.2/blissdata/beacon/files.py` & `blissdata-1.0.3/blissdata/beacon/files.py`

 * *Files identical despite different names*

### Comparing `blissdata-1.0.2/blissdata/h5api/abstract.py` & `blissdata-1.0.3/blissdata/h5api/abstract.py`

 * *Files identical despite different names*

### Comparing `blissdata-1.0.2/blissdata/h5api/dynamic_hdf5.py` & `blissdata-1.0.3/blissdata/h5api/dynamic_hdf5.py`

 * *Files identical despite different names*

### Comparing `blissdata-1.0.2/blissdata/h5api/file_arguments.py` & `blissdata-1.0.3/blissdata/h5api/file_arguments.py`

 * *Files identical despite different names*

### Comparing `blissdata-1.0.2/blissdata/h5api/static_hdf5.py` & `blissdata-1.0.3/blissdata/h5api/static_hdf5.py`

 * *Files identical despite different names*

### Comparing `blissdata-1.0.2/blissdata/h5api/utils/bliss.py` & `blissdata-1.0.3/blissdata/h5api/utils/bliss.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,15 @@
         return isinstance(h5item, (h5py.Group, h5py.File, lima.LimaGroup))
 
     def _is_initialized(self, h5item: hdf5.HDF5Item) -> bool:
         try:
             if h5item.name == hdf5.SEP:
                 return False
             scan = [s for s in h5item.name.split(hdf5.SEP) if s][0]
-            nxentry = self.file_obj.file[scan]
+            nxentry = self.file_obj[scan]
         except AttributeError:
             raise RetryError("file is closed")
         if "end_time" in nxentry:
             # Last dataset written to the file
             return True
         return self._get_writer_status(nxentry) in ("RUNNING", "SUCCEEDED", "FAILED")
 
@@ -115,18 +115,15 @@
             if h5item.name == hdf5.SEP:
                 # Assume there could be always more scans coming
                 return False
             scan = [s for s in h5item.name.split(hdf5.SEP) if s][0]
             nxentry = self.file_obj[scan]
         except AttributeError:
             raise RetryError("file is closed")
-        if "end_time" in nxentry:
-            # Last dataset written to the file
-            return True
-        return self._get_writer_status(nxentry) in ("SUCCEEDED", "FAILED")
+        return "end_time" in nxentry  # Last dataset written to the file
 
     def _get_writer_status(self, nxentry: h5py.Dataset) -> Optional[str]:
         nxnote = nxentry.get("writer", None)
         if nxnote is None:
             # writer notes not created yet
             return None
         status = nxnote.get("status", None)
```

### Comparing `blissdata-1.0.2/blissdata/h5api/utils/hdf5.py` & `blissdata-1.0.3/blissdata/h5api/utils/hdf5.py`

 * *Files 14% similar despite different names*

```diff
@@ -142,27 +142,30 @@
 
     def _get_item(self, name: str) -> HDF5Item:
         item = self._native_items.get(name)
         if item is not None:
             return item
         try:
             item = self.file_obj[name]
-        except KeyError as e:
-            parent_name = name.rpartition(SEP)[0]
+        except KeyError:
+            parent_name, _, item_name = name.rpartition(SEP)
             if not parent_name:
                 parent_name = SEP
-            if parent_name != name:
-                try:
-                    parent_item = self._get_item(parent_name)
-                except KeyError:
-                    pass
-                else:
-                    if self._is_finished(parent_item):
-                        raise RetryTimeoutError(str(e)) from e
-            raise
+            if parent_name == name:
+                raise
+            parent_item = self._get_item(parent_name)
+            if not self._is_finished(parent_item):
+                raise  # item could still be created
+            try:
+                item = parent_item[item_name]  # try one more time
+            except KeyError as e:
+                if not _key_does_not_exist(e):
+                    raise
+                # item will never be created
+                raise RetryTimeoutError(str(e)) from e
         self._native_items[name] = item
         return item
 
     def _slice_dataset(self, name: str, idx: types.DataIndexType) -> types.DataType:
         item = self._get_item(name)
         self._check_dataset_before_read(item)
         return item[idx]
@@ -170,51 +173,58 @@
     def _check_dataset_before_read(self, item: HDF5Dataset):
         pass
 
     def _get_attr(self, name: str, key: str) -> Any:
         item = self._get_item(name)
         try:
             return item.attrs[key]
-        except KeyError as e:
-            if self._is_finished(item):
+        except KeyError:
+            if not self._is_finished(item):
+                raise  # attribute could still be created
+            try:
+                return item.attrs[key]  # try one more time
+            except KeyError as e:
+                if not _key_does_not_exist(e):
+                    raise
+                # attribute will never be created
                 raise RetryTimeoutError(str(e)) from e
-            raise
 
     def _iter_attrs(self, name: str, start_index: int = 0) -> Iterator[str]:
         item = self._get_item(name)
+        is_complete = self._is_initialized(item)
         if start_index == 0:
             yield from item.attrs
         else:
             yield from list(item.attrs)[start_index:]
-        if not self._is_initialized(item):
-            raise RetryError("not fully initialized")
+        if not is_complete:
+            raise RetryError("attributes could still be added")
 
     def _len_attrs(self, name: str) -> int:
         item = self._get_item(name)
         return len(item.attrs)
 
     def _iter_item(
         self, name: str, start_index: int = 0
     ) -> Iterator[Union[str, types.DataType]]:
         item = self._get_item(name)
         self._check_dataset_before_read(item)
         if self.is_group(item):
-            is_initialized = self._is_initialized(item)
+            is_complete = self._is_initialized(item)
             for key in self._iter_group(item, start_index):
-                is_initialized = False
+                is_complete = False
                 yield key
-            if not is_initialized:
-                raise RetryError("not initialized")
+            if not is_complete:
+                raise RetryError("children could still be added to the group")
         else:
-            is_finished = self._is_finished(item)
+            is_complete = self._is_finished(item)
             for data in self._iter_dataset(item, start_index):
-                is_finished = False
+                is_complete = False
                 yield data
-            if not is_finished:
-                raise RetryError("not finished")
+            if not is_complete:
+                raise RetryError("dataset could still grow")
 
     @staticmethod
     def is_group(h5item: HDF5Item):
         return isinstance(h5item, (h5py.Group, h5py.File))
 
     def _iter_group(self, h5group: HDF5Group, start_index: int) -> Iterator[str]:
         try:
@@ -246,7 +256,25 @@
         return getattr(item, attr_name)
 
     def _is_initialized(self, h5item: HDF5Item) -> bool:
         return True
 
     def _is_finished(self, h5item: HDF5Item) -> bool:
         return True
+
+
+def _key_does_not_exist(exc: KeyError) -> bool:
+    """
+    A real KeyError (meaning that the key does not exist) gives the following error message:
+
+    .. code
+
+        KeyError: "Unable to synchronously open object (object 'end_time' doesn't exist)"
+
+    An example of a KeyError caused by another reason
+
+    .. code
+
+        KeyError: 'Unable to synchronously open object (addr overflow, addr = 64392369, size = 96, eoa = 64365353)'
+
+    """
+    return "doesn't exist" in str(exc)
```

### Comparing `blissdata-1.0.2/blissdata/h5api/utils/hdf5_retry.py` & `blissdata-1.0.3/blissdata/h5api/utils/hdf5_retry.py`

 * *Files identical despite different names*

### Comparing `blissdata-1.0.2/blissdata/h5api/utils/lima.py` & `blissdata-1.0.3/blissdata/h5api/utils/lima.py`

 * *Files identical despite different names*

### Comparing `blissdata-1.0.2/blissdata/lima/client.py` & `blissdata-1.0.3/blissdata/lima/client.py`

 * *Files identical despite different names*

### Comparing `blissdata-1.0.2/blissdata/lima/image_utils.py` & `blissdata-1.0.3/blissdata/lima/image_utils.py`

 * *Files identical despite different names*

### Comparing `blissdata-1.0.2/blissdata/redis_engine/encoding/__init__.py` & `blissdata-1.0.3/blissdata/redis_engine/encoding/__init__.py`

 * *Files identical despite different names*

### Comparing `blissdata-1.0.2/blissdata/redis_engine/encoding/json.py` & `blissdata-1.0.3/blissdata/redis_engine/encoding/json.py`

 * *Files identical despite different names*

### Comparing `blissdata-1.0.2/blissdata/redis_engine/encoding/numeric.py` & `blissdata-1.0.3/blissdata/redis_engine/encoding/numeric.py`

 * *Files identical despite different names*

### Comparing `blissdata-1.0.2/blissdata/redis_engine/exceptions.py` & `blissdata-1.0.3/blissdata/redis_engine/exceptions.py`

 * *Files identical despite different names*

### Comparing `blissdata-1.0.2/blissdata/redis_engine/identities.py` & `blissdata-1.0.3/blissdata/redis_engine/identities.py`

 * *Files identical despite different names*

### Comparing `blissdata-1.0.2/blissdata/redis_engine/memory_tracker.py` & `blissdata-1.0.3/blissdata/redis_engine/memory_tracker.py`

 * *Files identical despite different names*

### Comparing `blissdata-1.0.2/blissdata/redis_engine/scan.py` & `blissdata-1.0.3/blissdata/redis_engine/scan.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,16 @@
         prefix = scan._data_store._scan_model.make_key("")
         if not key.startswith(prefix):
             raise RuntimeError(f"Scan key should be prefixed by '{prefix}'")
 
         for prop_name in scan._data_store._scan_model.id.field.type_.schema()[
             "properties"
         ].keys():
+            if prop_name == "pk":
+                continue
 
             def get_id_field(self, field=prop_name):
                 return getattr(self._model.id, field, None)
 
             add_property(scan, prop_name, get_id_field)
 
         scan._streams = {}
@@ -105,14 +107,16 @@
             state_stream=scan._data_store._stream_model(),
             data_streams=[],
         )
 
         for prop_name in scan._data_store._scan_model.id.field.type_.schema()[
             "properties"
         ].keys():
+            if prop_name == "pk":
+                continue
 
             def get_id_field(self, field=prop_name):
                 return getattr(self._model.id, field, None)
 
             add_property(scan, prop_name, get_id_field)
 
         scan._streams = {}
@@ -274,18 +278,15 @@
         In the case of multiple processes/threads writing to the scan's streams,
         it is each writer's responsibility to seal its stream. Then the scan owner
         can wait for streams to be sealed and close the scan smoothly.
         Eventually, it may timeout and force the closure of all streams, making
         the still running writers to fail.
         """
         for stream_writer in self._writer_streams.values():
-            if not stream_writer.is_sealed():
-                stream_writer.seal()
-            else:
-                stream_writer._sink.stop()
+            stream_writer.seal()
         self._writer_streams = {}
 
     @needs_write_permission
     def prepare(self):
         if self.state is ScanState.CREATED:
             self._set_state(ScanState.PREPARED)
         else:
@@ -297,23 +298,23 @@
             self._set_state(ScanState.STARTED)
         else:
             raise UnauthorizeStateTransition(self.state, ScanState.STARTED)
 
     @needs_write_permission
     def stop(self):
         if self.state is ScanState.STARTED:
-            self._set_state(ScanState.STOPPED)
             self._close_stream_writers()
+            self._set_state(ScanState.STOPPED)
         else:
             raise UnauthorizeStateTransition(self.state, ScanState.STOPPED)
 
     @needs_write_permission
     def close(self):
-        self._set_state(ScanState.CLOSED)
         self._close_stream_writers()
+        self._set_state(ScanState.CLOSED)
 
     @needs_write_permission
     def _set_state(self, state):
         prev_state = self._state
         self._state = state
 
         self._model.info = Scan._filter_nan_values(self._model.info)
```

### Comparing `blissdata-1.0.2/blissdata/redis_engine/sink.py` & `blissdata-1.0.3/blissdata/redis_engine/sink.py`

 * *Files identical despite different names*

### Comparing `blissdata-1.0.2/blissdata/redis_engine/store.py` & `blissdata-1.0.3/blissdata/redis_engine/store.py`

 * *Files identical despite different names*

### Comparing `blissdata-1.0.2/blissdata/redis_engine/stream.py` & `blissdata-1.0.3/blissdata/redis_engine/stream.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*-
 #
 # This file is part of the bliss project
 #
 # Copyright (c) Beamline Control Unit, ESRF
 # Distributed under the GNU LGPLv3. See LICENSE for more info.
+import redis
 from functools import wraps
 from dataclasses import dataclass
 from collections.abc import Mapping
 from beartype import beartype
 
 from .encoding import EncodedBatch
 from .encoding.json import JsonStreamDecoder
@@ -266,16 +267,22 @@
 
     @needs_write_permission
     def join(self):
         self._sink.join()
 
     @needs_write_permission
     def seal(self):
-        self._sink.fcall("seal_stream", 1, self.key)
         self._sink.stop()
+        try:
+            return self._data_store._redis.fcall("seal_stream", 1, self.key)
+        except redis.exceptions.ResponseError as e:
+            if "is already sealed" in str(e):
+                return len(self)
+            else:
+                raise
 
     def __del__(self):
         # Thread based sinks can't be garbage collected, because their internal thread
         # still hold a reference. Then it is sink's owner responsibility to stop them.
         if hasattr(self, "_sink"):
             try:
                 self._sink.stop()
```

### Comparing `blissdata-1.0.2/blissdata/scan.py` & `blissdata-1.0.3/blissdata/scan.py`

 * *Files identical despite different names*

### Comparing `blissdata-1.0.2/blissdata/schemas/scan_info.py` & `blissdata-1.0.3/blissdata/schemas/scan_info.py`

 * *Files identical despite different names*

### Comparing `blissdata-1.0.2/blissdata/schemas/scan_info_display.py` & `blissdata-1.0.3/blissdata/schemas/scan_info_display.py`

 * *Files identical despite different names*

### Comparing `blissdata-1.0.2/blissdata/stream.py` & `blissdata-1.0.3/blissdata/stream.py`

 * *Files identical despite different names*

### Comparing `blissdata-1.0.2/blissdata/tests/beacon/test_config.py` & `blissdata-1.0.3/blissdata/tests/beacon/test_config.py`

 * *Files identical despite different names*

### Comparing `blissdata-1.0.2/blissdata/tests/beacon/test_data.py` & `blissdata-1.0.3/blissdata/tests/beacon/test_data.py`

 * *Files identical despite different names*

### Comparing `blissdata-1.0.2/blissdata/tests/beacon/test_files.py` & `blissdata-1.0.3/blissdata/tests/beacon/test_files.py`

 * *Files identical despite different names*

### Comparing `blissdata-1.0.2/blissdata/tests/conftest.py` & `blissdata-1.0.3/blissdata/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `blissdata-1.0.2/blissdata/tests/h5api/scanner.py` & `blissdata-1.0.3/blissdata/tests/h5api/scanner.py`

 * *Files 0% similar despite different names*

```diff
@@ -264,26 +264,26 @@
 def writer_context(filename: str, scan_number: int) -> Iterator[h5py.Group]:
     with h5py.File(filename, mode="a") as root:
         root.attrs["NX_class"] = "NXroot"
         entry = root.create_group(f"{scan_number}.1")
 
         try:
             entry.attrs["NX_class"] = "NXentry"
-            entry.attrs["start_time"] = timestamp()
+            entry["start_time"] = timestamp()
             writer = entry.create_group("writer")
             writer.attrs["NX_class"] = "NXnote"
             writer["status"] = "STARTING"
             yield entry
         except Exception:
             writer["status"][()] = "FAILED"
             raise
         else:
             writer["status"][()] = "SUCCEEDED"
         finally:
-            entry.attrs["end_time"] = timestamp()
+            entry["end_time"] = timestamp()
 
 
 @contextmanager
 def lima_servers(counters: Sequence[ChannelInfo]):
     queues = dict()
     processed = list()
     for ctr in counters:
```

### Comparing `blissdata-1.0.2/blissdata/tests/h5api/test_dynamic_files.py` & `blissdata-1.0.3/blissdata/tests/h5api/test_dynamic_files.py`

 * *Files identical despite different names*

### Comparing `blissdata-1.0.2/blissdata/tests/h5api/test_static_files.py` & `blissdata-1.0.3/blissdata/tests/h5api/test_static_files.py`

 * *Files identical despite different names*

### Comparing `blissdata-1.0.2/blissdata/tests/redis_engine/encoding/test_numeric.py` & `blissdata-1.0.3/blissdata/tests/redis_engine/encoding/test_numeric.py`

 * *Files identical despite different names*

### Comparing `blissdata-1.0.2/blissdata/tests/redis_engine/test_memory_tracker.py` & `blissdata-1.0.3/blissdata/tests/redis_engine/test_memory_tracker.py`

 * *Files identical despite different names*

### Comparing `blissdata-1.0.2/blissdata/tests/redis_engine/test_scan.py` & `blissdata-1.0.3/blissdata/tests/redis_engine/test_scan.py`

 * *Files identical despite different names*

### Comparing `blissdata-1.0.2/blissdata/tests/redis_engine/test_search.py` & `blissdata-1.0.3/blissdata/tests/redis_engine/test_search.py`

 * *Files identical despite different names*

### Comparing `blissdata-1.0.2/blissdata/tests/redis_engine/test_streaming.py` & `blissdata-1.0.3/blissdata/tests/redis_engine/test_streaming.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,30 @@
 
 def test_stream_unknown_encoding(data_store):
     model = data_store._stream_model(encoding={"type": "teapot"})
     with pytest.raises(UnknownEncodingError):
         Stream.create(data_store, "my_stream", model, None)
 
 
+def test_multiple_calls_to_seal(data_store):
+    input = np.arange(1000)
+    rw_stream, _ = stream_pair(data_store, input.dtype)
+    rw_stream.send(input)
+
+    # make a second writing stream to test re-sealing from an unaware object
+    external_writer = Stream.create(
+        data_store, rw_stream.name, rw_stream._model, rw_stream._encoder
+    )
+
+    assert rw_stream.seal() == 1000
+    assert rw_stream.seal() == 1000
+    assert external_writer.seal() == 1000
+    assert external_writer.seal() == 1000
+
+
 def test_stream_chunk_slicing(data_store):
     data = np.arange(100)
     rw_stream, ro_stream = stream_pair(data_store, data.dtype)
 
     # produce chunks of different sizes
     rw_stream.send(data[0])  # 1
     rw_stream.send(data[1:3])  # 2
```

### Comparing `blissdata-1.0.2/blissdata/tests/redis_engine/utils.py` & `blissdata-1.0.3/blissdata/tests/redis_engine/utils.py`

 * *Files identical despite different names*

### Comparing `blissdata-1.0.2/blissdata.egg-info/PKG-INFO` & `blissdata-1.0.3/blissdata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blissdata
-Version: 1.0.2
+Version: 1.0.3
 Summary: Bliss data streaming client
 Home-page: https://gitlab.esrf.fr/bliss/bliss/-/tree/master/blissdata
 Author: BCU (ESRF)
 License: LGPLv3
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `blissdata-1.0.2/blissdata.egg-info/SOURCES.txt` & `blissdata-1.0.3/blissdata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blissdata-1.0.2/setup.cfg` & `blissdata-1.0.3/setup.cfg`

 * *Files identical despite different names*

