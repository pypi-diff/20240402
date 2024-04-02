# Comparing `tmp/vos-data-utils-1.0.1.tar.gz` & `tmp/vos-data-utils-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/vos-data-utils/vos-data-utils/dist/.tmp-0ae5zvek/vos-data-utils-1.0.1.tar", last modified: Fri Feb  2 05:06:58 2024, max compression
+gzip compressed data, was "/home/runner/work/vos-data-utils/vos-data-utils/dist/.tmp-gvw5uu4b/vos-data-utils-1.0.2.tar", last modified: Tue Apr  2 09:57:55 2024, max compression
```

## Comparing `vos-data-utils-1.0.1.tar` & `vos-data-utils-1.0.2.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 05:06:58.000000 vos-data-utils-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    51162 2024-02-02 05:06:58.000000 vos-data-utils-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    50565 2024-02-02 05:06:23.000000 vos-data-utils-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-02 05:06:58.000000 vos-data-utils-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-02-02 05:06:23.000000 vos-data-utils-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 05:06:58.000000 vos-data-utils-1.0.1/vdutils/
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-02-02 05:06:23.000000 vos-data-utils-1.0.1/vdutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20936 2024-02-02 05:06:23.000000 vos-data-utils-1.0.1/vdutils/bjd.py
--rw-r--r--   0 runner    (1001) docker     (127)    29482 2024-02-02 05:06:23.000000 vos-data-utils-1.0.1/vdutils/bjdconnector.py
--rw-r--r--   0 runner    (1001) docker     (127)    14280 2024-02-02 05:06:23.000000 vos-data-utils-1.0.1/vdutils/convaddr.py
--rw-r--r--   0 runner    (1001) docker     (127)    13638 2024-02-02 05:06:23.000000 vos-data-utils-1.0.1/vdutils/cordate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 05:06:58.000000 vos-data-utils-1.0.1/vdutils/data/
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-02-02 05:06:23.000000 vos-data-utils-1.0.1/vdutils/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 05:06:58.000000 vos-data-utils-1.0.1/vdutils/data/bjd/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 05:06:58.000000 vos-data-utils-1.0.1/vdutils/data/bjd/20230701/
--rw-r--r--   0 runner    (1001) docker     (127)  5539602 2024-02-02 05:06:23.000000 vos-data-utils-1.0.1/vdutils/data/bjd/20230701/bjd.txt
--rw-r--r--   0 runner    (1001) docker     (127)  1730155 2024-02-02 05:06:23.000000 vos-data-utils-1.0.1/vdutils/data/bjd/20230701/bjd_changed.txt
--rw-r--r--   0 runner    (1001) docker     (127)  2293207 2024-02-02 05:06:23.000000 vos-data-utils-1.0.1/vdutils/data/bjd/20230701/bjd_current.txt
--rw-r--r--   0 runner    (1001) docker     (127)   139267 2024-02-02 05:06:23.000000 vos-data-utils-1.0.1/vdutils/data/bjd/20230701/bjd_frequency_dictionary.txt
--rw-r--r--   0 runner    (1001) docker     (127)   100009 2024-02-02 05:06:23.000000 vos-data-utils-1.0.1/vdutils/data/bjd/20230701/bjd_smallest.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-02-02 05:06:23.000000 vos-data-utils-1.0.1/vdutils/data/bjd/20230701/multiple_word_sgg_list.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 05:06:58.000000 vos-data-utils-1.0.1/vdutils/data/bjd/20240118/
--rw-r--r--   0 runner    (1001) docker     (127)  5818464 2024-02-02 05:06:23.000000 vos-data-utils-1.0.1/vdutils/data/bjd/20240118/bjd.txt
--rw-r--r--   0 runner    (1001) docker     (127)  2247502 2024-02-02 05:06:23.000000 vos-data-utils-1.0.1/vdutils/data/bjd/20240118/bjd_changed.txt
--rw-r--r--   0 runner    (1001) docker     (127)  2344590 2024-02-02 05:06:23.000000 vos-data-utils-1.0.1/vdutils/data/bjd/20240118/bjd_current.txt
--rw-r--r--   0 runner    (1001) docker     (127)   139328 2024-02-02 05:06:23.000000 vos-data-utils-1.0.1/vdutils/data/bjd/20240118/bjd_frequency_dictionary.txt
--rw-r--r--   0 runner    (1001) docker     (127)   100009 2024-02-02 05:06:23.000000 vos-data-utils-1.0.1/vdutils/data/bjd/20240118/bjd_smallest.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-02-02 05:06:23.000000 vos-data-utils-1.0.1/vdutils/data/bjd/20240118/multiple_word_sgg_list.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 05:06:58.000000 vos-data-utils-1.0.1/vdutils/data/bjd/20240201/
--rw-r--r--   0 runner    (1001) docker     (127)  5820666 2024-02-02 05:06:23.000000 vos-data-utils-1.0.1/vdutils/data/bjd/20240201/bjd.txt
--rw-r--r--   0 runner    (1001) docker     (127)  2251726 2024-02-02 05:06:23.000000 vos-data-utils-1.0.1/vdutils/data/bjd/20240201/bjd_changed.txt
--rw-r--r--   0 runner    (1001) docker     (127)  2344736 2024-02-02 05:06:23.000000 vos-data-utils-1.0.1/vdutils/data/bjd/20240201/bjd_current.txt
--rw-r--r--   0 runner    (1001) docker     (127)   139328 2024-02-02 05:06:23.000000 vos-data-utils-1.0.1/vdutils/data/bjd/20240201/bjd_frequency_dictionary.txt
--rw-r--r--   0 runner    (1001) docker     (127)   100009 2024-02-02 05:06:23.000000 vos-data-utils-1.0.1/vdutils/data/bjd/20240201/bjd_smallest.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-02-02 05:06:23.000000 vos-data-utils-1.0.1/vdutils/data/bjd/20240201/multiple_word_sgg_list.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 05:06:58.000000 vos-data-utils-1.0.1/vdutils/data/date/
--rw-r--r--   0 runner    (1001) docker     (127)  8186154 2024-02-02 05:06:23.000000 vos-data-utils-1.0.1/vdutils/data/date/date_dictionary.txt
--rw-r--r--   0 runner    (1001) docker     (127)    21800 2024-02-02 05:06:23.000000 vos-data-utils-1.0.1/vdutils/genpnu.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 05:06:58.000000 vos-data-utils-1.0.1/vdutils/library/
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-02-02 05:06:23.000000 vos-data-utils-1.0.1/vdutils/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   206956 2024-02-02 05:06:23.000000 vos-data-utils-1.0.1/vdutils/library/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 05:06:58.000000 vos-data-utils-1.0.1/vdutils/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-02 05:06:23.000000 vos-data-utils-1.0.1/vdutils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7309 2024-02-02 05:06:23.000000 vos-data-utils-1.0.1/vdutils/tests/test_convaddr.py
--rw-r--r--   0 runner    (1001) docker     (127)    11950 2024-02-02 05:06:23.000000 vos-data-utils-1.0.1/vdutils/tests/test_cordate.py
--rw-r--r--   0 runner    (1001) docker     (127)    71509 2024-02-02 05:06:23.000000 vos-data-utils-1.0.1/vdutils/tests/test_genpnu.py
--rw-r--r--   0 runner    (1001) docker     (127)     9714 2024-02-02 05:06:23.000000 vos-data-utils-1.0.1/vdutils/tests/test_vid.py
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-02-02 05:06:23.000000 vos-data-utils-1.0.1/vdutils/tests/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-02-02 05:06:23.000000 vos-data-utils-1.0.1/vdutils/vid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 05:06:58.000000 vos-data-utils-1.0.1/vos_data_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    51162 2024-02-02 05:06:58.000000 vos-data-utils-1.0.1/vos_data_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-02-02 05:06:58.000000 vos-data-utils-1.0.1/vos_data_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-02 05:06:58.000000 vos-data-utils-1.0.1/vos_data_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-02-02 05:06:58.000000 vos-data-utils-1.0.1/vos_data_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-02-02 05:06:58.000000 vos-data-utils-1.0.1/vos_data_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-02 05:06:58.000000 vos-data-utils-1.0.1/vos_data_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:57:55.000000 vos-data-utils-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    51336 2024-04-02 09:57:55.000000 vos-data-utils-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    50739 2024-04-02 09:57:42.000000 vos-data-utils-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 09:57:55.000000 vos-data-utils-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-04-02 09:57:42.000000 vos-data-utils-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:57:55.000000 vos-data-utils-1.0.2/vdutils/
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-02 09:57:42.000000 vos-data-utils-1.0.2/vdutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20936 2024-04-02 09:57:42.000000 vos-data-utils-1.0.2/vdutils/bjd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29482 2024-04-02 09:57:42.000000 vos-data-utils-1.0.2/vdutils/bjdconnector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14280 2024-04-02 09:57:42.000000 vos-data-utils-1.0.2/vdutils/convaddr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13638 2024-04-02 09:57:42.000000 vos-data-utils-1.0.2/vdutils/cordate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:57:55.000000 vos-data-utils-1.0.2/vdutils/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-02 09:57:42.000000 vos-data-utils-1.0.2/vdutils/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:57:55.000000 vos-data-utils-1.0.2/vdutils/data/bjd/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:57:55.000000 vos-data-utils-1.0.2/vdutils/data/bjd/20230701/
+-rw-r--r--   0 runner    (1001) docker     (127)  5539602 2024-04-02 09:57:42.000000 vos-data-utils-1.0.2/vdutils/data/bjd/20230701/bjd.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  1730155 2024-04-02 09:57:42.000000 vos-data-utils-1.0.2/vdutils/data/bjd/20230701/bjd_changed.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  2293207 2024-04-02 09:57:42.000000 vos-data-utils-1.0.2/vdutils/data/bjd/20230701/bjd_current.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   139267 2024-04-02 09:57:42.000000 vos-data-utils-1.0.2/vdutils/data/bjd/20230701/bjd_frequency_dictionary.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   100009 2024-04-02 09:57:42.000000 vos-data-utils-1.0.2/vdutils/data/bjd/20230701/bjd_smallest.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-04-02 09:57:42.000000 vos-data-utils-1.0.2/vdutils/data/bjd/20230701/multiple_word_sgg_list.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:57:55.000000 vos-data-utils-1.0.2/vdutils/data/bjd/20240118/
+-rw-r--r--   0 runner    (1001) docker     (127)  5818464 2024-04-02 09:57:42.000000 vos-data-utils-1.0.2/vdutils/data/bjd/20240118/bjd.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  2247502 2024-04-02 09:57:42.000000 vos-data-utils-1.0.2/vdutils/data/bjd/20240118/bjd_changed.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  2344590 2024-04-02 09:57:42.000000 vos-data-utils-1.0.2/vdutils/data/bjd/20240118/bjd_current.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   139328 2024-04-02 09:57:42.000000 vos-data-utils-1.0.2/vdutils/data/bjd/20240118/bjd_frequency_dictionary.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   100009 2024-04-02 09:57:42.000000 vos-data-utils-1.0.2/vdutils/data/bjd/20240118/bjd_smallest.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-04-02 09:57:42.000000 vos-data-utils-1.0.2/vdutils/data/bjd/20240118/multiple_word_sgg_list.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:57:55.000000 vos-data-utils-1.0.2/vdutils/data/bjd/20240201/
+-rw-r--r--   0 runner    (1001) docker     (127)  5820666 2024-04-02 09:57:42.000000 vos-data-utils-1.0.2/vdutils/data/bjd/20240201/bjd.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  2251726 2024-04-02 09:57:42.000000 vos-data-utils-1.0.2/vdutils/data/bjd/20240201/bjd_changed.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  2344736 2024-04-02 09:57:42.000000 vos-data-utils-1.0.2/vdutils/data/bjd/20240201/bjd_current.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   139328 2024-04-02 09:57:42.000000 vos-data-utils-1.0.2/vdutils/data/bjd/20240201/bjd_frequency_dictionary.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   100009 2024-04-02 09:57:42.000000 vos-data-utils-1.0.2/vdutils/data/bjd/20240201/bjd_smallest.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-04-02 09:57:42.000000 vos-data-utils-1.0.2/vdutils/data/bjd/20240201/multiple_word_sgg_list.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:57:55.000000 vos-data-utils-1.0.2/vdutils/data/date/
+-rw-r--r--   0 runner    (1001) docker     (127)  8186154 2024-04-02 09:57:42.000000 vos-data-utils-1.0.2/vdutils/data/date/date_dictionary.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    21800 2024-04-02 09:57:42.000000 vos-data-utils-1.0.2/vdutils/genpnu.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:57:55.000000 vos-data-utils-1.0.2/vdutils/library/
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-02 09:57:42.000000 vos-data-utils-1.0.2/vdutils/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   206956 2024-04-02 09:57:42.000000 vos-data-utils-1.0.2/vdutils/library/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:57:55.000000 vos-data-utils-1.0.2/vdutils/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 09:57:42.000000 vos-data-utils-1.0.2/vdutils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7309 2024-04-02 09:57:42.000000 vos-data-utils-1.0.2/vdutils/tests/test_convaddr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11950 2024-04-02 09:57:42.000000 vos-data-utils-1.0.2/vdutils/tests/test_cordate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71509 2024-04-02 09:57:42.000000 vos-data-utils-1.0.2/vdutils/tests/test_genpnu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9714 2024-04-02 09:57:42.000000 vos-data-utils-1.0.2/vdutils/tests/test_vid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-02 09:57:42.000000 vos-data-utils-1.0.2/vdutils/tests/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-04-02 09:57:42.000000 vos-data-utils-1.0.2/vdutils/vid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:57:55.000000 vos-data-utils-1.0.2/vos_data_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    51336 2024-04-02 09:57:55.000000 vos-data-utils-1.0.2/vos_data_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-02 09:57:55.000000 vos-data-utils-1.0.2/vos_data_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 09:57:55.000000 vos-data-utils-1.0.2/vos_data_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-02 09:57:55.000000 vos-data-utils-1.0.2/vos_data_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-02 09:57:55.000000 vos-data-utils-1.0.2/vos_data_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-02 09:57:55.000000 vos-data-utils-1.0.2/vos_data_utils.egg-info/top_level.txt
```

### Comparing `vos-data-utils-1.0.1/PKG-INFO` & `vos-data-utils-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vos-data-utils
-Version: 1.0.1
+Version: 1.0.2
 Summary: description
 Author: ValueOfSpace
 Author-email: dev@valueofspace.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -63,14 +63,23 @@
 
 -   업데이트
     -   법정동 데이터 업데이트(행정구역 변경사항 반영)
         -   2024년 2월 1일: '경상북도 영천군 호명읍' 관련 행정구역 변경
     -   날짜 빈도 dictionary 업데이트
 
 </details>
+<details>
+<summary><strong>Version 1.0.2 - 2024.04</strong></summary>
+
+<div style="color: gray;">
+
+-   업데이트
+    -   날짜 빈도 dictionary 업데이트
+
+</details>
 </br>
 
 # Install
 
 ```python
 pip install vos-data-utils
 ```
```

### Comparing `vos-data-utils-1.0.1/README.md` & `vos-data-utils-1.0.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -46,14 +46,23 @@
 
 -   업데이트
     -   법정동 데이터 업데이트(행정구역 변경사항 반영)
         -   2024년 2월 1일: '경상북도 영천군 호명읍' 관련 행정구역 변경
     -   날짜 빈도 dictionary 업데이트
 
 </details>
+<details>
+<summary><strong>Version 1.0.2 - 2024.04</strong></summary>
+
+<div style="color: gray;">
+
+-   업데이트
+    -   날짜 빈도 dictionary 업데이트
+
+</details>
 </br>
 
 # Install
 
 ```python
 pip install vos-data-utils
 ```
```

### Comparing `vos-data-utils-1.0.1/setup.py` & `vos-data-utils-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `vos-data-utils-1.0.1/vdutils/__init__.py` & `vos-data-utils-1.0.2/vdutils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 -------------
 Correction function for dates related to building permit, commencement, and completion in the Building Permit Information
 Support for current legal district data and change history
 Correction function to align with the current legal district by reflecting changes in legal district data
 Conversion function to transform address strings into Parcel Number (PNU)
 Generation function for unique transaction case IDs in ValueofSpace
 """
-version = "1.0.1" 
+version = "1.0.2" 
 author = "ValueOfSpace"
 description = "description"
 license = "MIT License"
 python_version = "3.7, 3.8, 3.9, 3.10, 3.11"
 
 def __version__():
     return version
```

### Comparing `vos-data-utils-1.0.1/vdutils/bjd.py` & `vos-data-utils-1.0.2/vdutils/bjd.py`

 * *Files identical despite different names*

### Comparing `vos-data-utils-1.0.1/vdutils/bjdconnector.py` & `vos-data-utils-1.0.2/vdutils/bjdconnector.py`

 * *Files identical despite different names*

### Comparing `vos-data-utils-1.0.1/vdutils/convaddr.py` & `vos-data-utils-1.0.2/vdutils/convaddr.py`

 * *Files identical despite different names*

### Comparing `vos-data-utils-1.0.1/vdutils/cordate.py` & `vos-data-utils-1.0.2/vdutils/cordate.py`

 * *Files identical despite different names*

### Comparing `vos-data-utils-1.0.1/vdutils/data/bjd/20230701/bjd.txt` & `vos-data-utils-1.0.2/vdutils/data/bjd/20230701/bjd.txt`

 * *Files identical despite different names*

### Comparing `vos-data-utils-1.0.1/vdutils/data/bjd/20230701/bjd_changed.txt` & `vos-data-utils-1.0.2/vdutils/data/bjd/20230701/bjd_changed.txt`

 * *Files identical despite different names*

### Comparing `vos-data-utils-1.0.1/vdutils/data/bjd/20230701/bjd_current.txt` & `vos-data-utils-1.0.2/vdutils/data/bjd/20230701/bjd_current.txt`

 * *Files identical despite different names*

### Comparing `vos-data-utils-1.0.1/vdutils/data/bjd/20230701/bjd_frequency_dictionary.txt` & `vos-data-utils-1.0.2/vdutils/data/bjd/20230701/bjd_frequency_dictionary.txt`

 * *Files identical despite different names*

### Comparing `vos-data-utils-1.0.1/vdutils/data/bjd/20230701/bjd_smallest.txt` & `vos-data-utils-1.0.2/vdutils/data/bjd/20230701/bjd_smallest.txt`

 * *Files identical despite different names*

### Comparing `vos-data-utils-1.0.1/vdutils/data/bjd/20230701/multiple_word_sgg_list.txt` & `vos-data-utils-1.0.2/vdutils/data/bjd/20230701/multiple_word_sgg_list.txt`

 * *Files identical despite different names*

### Comparing `vos-data-utils-1.0.1/vdutils/data/bjd/20240118/bjd.txt` & `vos-data-utils-1.0.2/vdutils/data/bjd/20240118/bjd.txt`

 * *Files identical despite different names*

### Comparing `vos-data-utils-1.0.1/vdutils/data/bjd/20240118/bjd_changed.txt` & `vos-data-utils-1.0.2/vdutils/data/bjd/20240118/bjd_changed.txt`

 * *Files identical despite different names*

### Comparing `vos-data-utils-1.0.1/vdutils/data/bjd/20240118/bjd_current.txt` & `vos-data-utils-1.0.2/vdutils/data/bjd/20240118/bjd_current.txt`

 * *Files identical despite different names*

### Comparing `vos-data-utils-1.0.1/vdutils/data/bjd/20240118/bjd_frequency_dictionary.txt` & `vos-data-utils-1.0.2/vdutils/data/bjd/20240118/bjd_frequency_dictionary.txt`

 * *Files identical despite different names*

### Comparing `vos-data-utils-1.0.1/vdutils/data/bjd/20240118/bjd_smallest.txt` & `vos-data-utils-1.0.2/vdutils/data/bjd/20240118/bjd_smallest.txt`

 * *Files identical despite different names*

### Comparing `vos-data-utils-1.0.1/vdutils/data/bjd/20240118/multiple_word_sgg_list.txt` & `vos-data-utils-1.0.2/vdutils/data/bjd/20240118/multiple_word_sgg_list.txt`

 * *Files identical despite different names*

### Comparing `vos-data-utils-1.0.1/vdutils/data/bjd/20240201/bjd.txt` & `vos-data-utils-1.0.2/vdutils/data/bjd/20240201/bjd.txt`

 * *Files identical despite different names*

### Comparing `vos-data-utils-1.0.1/vdutils/data/bjd/20240201/bjd_changed.txt` & `vos-data-utils-1.0.2/vdutils/data/bjd/20240201/bjd_changed.txt`

 * *Files identical despite different names*

### Comparing `vos-data-utils-1.0.1/vdutils/data/bjd/20240201/bjd_current.txt` & `vos-data-utils-1.0.2/vdutils/data/bjd/20240201/bjd_current.txt`

 * *Files identical despite different names*

### Comparing `vos-data-utils-1.0.1/vdutils/data/bjd/20240201/bjd_frequency_dictionary.txt` & `vos-data-utils-1.0.2/vdutils/data/bjd/20240201/bjd_frequency_dictionary.txt`

 * *Files identical despite different names*

### Comparing `vos-data-utils-1.0.1/vdutils/data/bjd/20240201/bjd_smallest.txt` & `vos-data-utils-1.0.2/vdutils/data/bjd/20240201/bjd_smallest.txt`

 * *Files identical despite different names*

### Comparing `vos-data-utils-1.0.1/vdutils/data/bjd/20240201/multiple_word_sgg_list.txt` & `vos-data-utils-1.0.2/vdutils/data/bjd/20240201/multiple_word_sgg_list.txt`

 * *Files identical despite different names*

### Comparing `vos-data-utils-1.0.1/vdutils/data/date/date_dictionary.txt` & `vos-data-utils-1.0.2/vdutils/data/date/date_dictionary.txt`

 * *Files identical despite different names*

### Comparing `vos-data-utils-1.0.1/vdutils/genpnu.py` & `vos-data-utils-1.0.2/vdutils/genpnu.py`

 * *Files identical despite different names*

### Comparing `vos-data-utils-1.0.1/vdutils/library/__init__.py` & `vos-data-utils-1.0.2/vdutils/library/__init__.py`

 * *Files identical despite different names*

### Comparing `vos-data-utils-1.0.1/vdutils/library/data.py` & `vos-data-utils-1.0.2/vdutils/library/data.py`

 * *Files identical despite different names*

### Comparing `vos-data-utils-1.0.1/vdutils/tests/test_convaddr.py` & `vos-data-utils-1.0.2/vdutils/tests/test_convaddr.py`

 * *Files identical despite different names*

### Comparing `vos-data-utils-1.0.1/vdutils/tests/test_cordate.py` & `vos-data-utils-1.0.2/vdutils/tests/test_cordate.py`

 * *Files identical despite different names*

### Comparing `vos-data-utils-1.0.1/vdutils/tests/test_genpnu.py` & `vos-data-utils-1.0.2/vdutils/tests/test_genpnu.py`

 * *Files identical despite different names*

### Comparing `vos-data-utils-1.0.1/vdutils/tests/test_vid.py` & `vos-data-utils-1.0.2/vdutils/tests/test_vid.py`

 * *Files identical despite different names*

### Comparing `vos-data-utils-1.0.1/vdutils/tests/tests.py` & `vos-data-utils-1.0.2/vdutils/tests/tests.py`

 * *Files identical despite different names*

### Comparing `vos-data-utils-1.0.1/vdutils/vid.py` & `vos-data-utils-1.0.2/vdutils/vid.py`

 * *Files identical despite different names*

### Comparing `vos-data-utils-1.0.1/vos_data_utils.egg-info/PKG-INFO` & `vos-data-utils-1.0.2/vos_data_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vos-data-utils
-Version: 1.0.1
+Version: 1.0.2
 Summary: description
 Author: ValueOfSpace
 Author-email: dev@valueofspace.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -63,14 +63,23 @@
 
 -   업데이트
     -   법정동 데이터 업데이트(행정구역 변경사항 반영)
         -   2024년 2월 1일: '경상북도 영천군 호명읍' 관련 행정구역 변경
     -   날짜 빈도 dictionary 업데이트
 
 </details>
+<details>
+<summary><strong>Version 1.0.2 - 2024.04</strong></summary>
+
+<div style="color: gray;">
+
+-   업데이트
+    -   날짜 빈도 dictionary 업데이트
+
+</details>
 </br>
 
 # Install
 
 ```python
 pip install vos-data-utils
 ```
```

### Comparing `vos-data-utils-1.0.1/vos_data_utils.egg-info/SOURCES.txt` & `vos-data-utils-1.0.2/vos_data_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

