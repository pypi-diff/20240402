# Comparing `tmp/moyanlib-1.5.1707129404.tar.gz` & `tmp/moyanlib-1.5.1712027947.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moyanlib-1.5.1707129404.tar", last modified: Mon Feb  5 10:36:44 2024, max compression
+gzip compressed data, was "moyanlib-1.5.1712027947.tar", last modified: Tue Apr  2 03:19:07 2024, max compression
```

## Comparing `moyanlib-1.5.1707129404.tar` & `moyanlib-1.5.1712027947.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 10:36:44.831688 moyanlib-1.5.1707129404/
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-02-05 10:36:44.831688 moyanlib-1.5.1707129404/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 10:36:44.831688 moyanlib-1.5.1707129404/moyanlib/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-05 10:36:30.000000 moyanlib-1.5.1707129404/moyanlib/Error.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-02-05 10:36:30.000000 moyanlib-1.5.1707129404/moyanlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-02-05 10:36:30.000000 moyanlib-1.5.1707129404/moyanlib/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 10:36:44.831688 moyanlib-1.5.1707129404/moyanlib/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-02-05 10:36:30.000000 moyanlib-1.5.1707129404/moyanlib/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-02-05 10:36:30.000000 moyanlib-1.5.1707129404/moyanlib/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-02-05 10:36:30.000000 moyanlib-1.5.1707129404/moyanlib/jsons.py
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-02-05 10:36:30.000000 moyanlib-1.5.1707129404/moyanlib/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-02-05 10:36:30.000000 moyanlib-1.5.1707129404/moyanlib/system.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 10:36:44.831688 moyanlib-1.5.1707129404/moyanlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-02-05 10:36:44.000000 moyanlib-1.5.1707129404/moyanlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-02-05 10:36:44.000000 moyanlib-1.5.1707129404/moyanlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-05 10:36:44.000000 moyanlib-1.5.1707129404/moyanlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-02-05 10:36:44.000000 moyanlib-1.5.1707129404/moyanlib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-05 10:36:44.000000 moyanlib-1.5.1707129404/moyanlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-05 10:36:44.000000 moyanlib-1.5.1707129404/moyanlib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-05 10:36:44.831688 moyanlib-1.5.1707129404/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-02-05 10:36:30.000000 moyanlib-1.5.1707129404/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 10:36:44.831688 moyanlib-1.5.1707129404/test/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-02-05 10:36:30.000000 moyanlib-1.5.1707129404/test/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-05 10:36:30.000000 moyanlib-1.5.1707129404/test/test_dec.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-05 10:36:30.000000 moyanlib-1.5.1707129404/test/test_json.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-05 10:36:30.000000 moyanlib-1.5.1707129404/test/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-02-05 10:36:30.000000 moyanlib-1.5.1707129404/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:19:07.764869 moyanlib-1.5.1712027947/
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-02 03:19:07.764869 moyanlib-1.5.1712027947/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:19:07.760869 moyanlib-1.5.1712027947/moyanlib/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-02 03:18:49.000000 moyanlib-1.5.1712027947/moyanlib/Error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-04-02 03:18:49.000000 moyanlib-1.5.1712027947/moyanlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-02 03:18:49.000000 moyanlib-1.5.1712027947/moyanlib/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:19:07.764869 moyanlib-1.5.1712027947/moyanlib/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-02 03:18:49.000000 moyanlib-1.5.1712027947/moyanlib/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-02 03:18:49.000000 moyanlib-1.5.1712027947/moyanlib/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-04-02 03:18:49.000000 moyanlib-1.5.1712027947/moyanlib/jsons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-02 03:18:49.000000 moyanlib-1.5.1712027947/moyanlib/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-02 03:18:49.000000 moyanlib-1.5.1712027947/moyanlib/system.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:19:07.764869 moyanlib-1.5.1712027947/moyanlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-02 03:19:07.000000 moyanlib-1.5.1712027947/moyanlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-02 03:19:07.000000 moyanlib-1.5.1712027947/moyanlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 03:19:07.000000 moyanlib-1.5.1712027947/moyanlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-02 03:19:07.000000 moyanlib-1.5.1712027947/moyanlib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-02 03:19:07.000000 moyanlib-1.5.1712027947/moyanlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-02 03:19:07.000000 moyanlib-1.5.1712027947/moyanlib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 03:19:07.764869 moyanlib-1.5.1712027947/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-02 03:18:49.000000 moyanlib-1.5.1712027947/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:19:07.764869 moyanlib-1.5.1712027947/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-02 03:18:49.000000 moyanlib-1.5.1712027947/test/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 03:18:49.000000 moyanlib-1.5.1712027947/test/test_dec.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 03:18:49.000000 moyanlib-1.5.1712027947/test/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 03:18:49.000000 moyanlib-1.5.1712027947/test/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-02 03:18:49.000000 moyanlib-1.5.1712027947/test/test_utils.py
```

### Comparing `moyanlib-1.5.1707129404/moyanlib/cache.py` & `moyanlib-1.5.1712027947/moyanlib/cache.py`

 * *Files identical despite different names*

### Comparing `moyanlib-1.5.1707129404/moyanlib/cli/__init__.py` & `moyanlib-1.5.1712027947/moyanlib/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `moyanlib-1.5.1707129404/moyanlib/decorators.py` & `moyanlib-1.5.1712027947/moyanlib/decorators.py`

 * *Files identical despite different names*

### Comparing `moyanlib-1.5.1707129404/moyanlib/jsons.py` & `moyanlib-1.5.1712027947/moyanlib/jsons.py`

 * *Files identical despite different names*

### Comparing `moyanlib-1.5.1707129404/moyanlib/logger.py` & `moyanlib-1.5.1712027947/moyanlib/logger.py`

 * *Files identical despite different names*

### Comparing `moyanlib-1.5.1707129404/moyanlib/system.py` & `moyanlib-1.5.1712027947/moyanlib/system.py`

 * *Files identical despite different names*

### Comparing `moyanlib-1.5.1707129404/setup.py` & `moyanlib-1.5.1712027947/setup.py`

 * *Files identical despite different names*

### Comparing `moyanlib-1.5.1707129404/test/test_cache.py` & `moyanlib-1.5.1712027947/test/test_cache.py`

 * *Files identical despite different names*

