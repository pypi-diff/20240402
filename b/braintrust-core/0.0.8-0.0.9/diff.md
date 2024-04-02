# Comparing `tmp/braintrust_core-0.0.8.tar.gz` & `tmp/braintrust_core-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "braintrust_core-0.0.8.tar", last modified: Wed Jan 10 01:29:23 2024, max compression
+gzip compressed data, was "braintrust_core-0.0.9.tar", last modified: Fri Jan 12 06:33:27 2024, max compression
```

## Comparing `braintrust_core-0.0.8.tar` & `braintrust_core-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2024-01-10 01:29:23.147473 braintrust_core-0.0.8/
--rw-r--r--   0 ankur      (501) staff       (20)      502 2024-01-10 01:29:23.147301 braintrust_core-0.0.8/PKG-INFO
--rw-r--r--   0 ankur      (501) staff       (20)      125 2023-12-22 23:17:30.000000 braintrust_core-0.0.8/README.md
--rw-r--r--   0 ankur      (501) staff       (20)       38 2024-01-10 01:29:23.147508 braintrust_core-0.0.8/setup.cfg
--rw-r--r--   0 ankur      (501) staff       (20)     1070 2023-12-22 23:17:30.000000 braintrust_core-0.0.8/setup.py
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2024-01-10 01:29:23.145464 braintrust_core-0.0.8/src/
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2024-01-10 01:29:23.146454 braintrust_core-0.0.8/src/braintrust_core/
--rw-r--r--   0 ankur      (501) staff       (20)       41 2023-12-22 23:17:30.000000 braintrust_core-0.0.8/src/braintrust_core/__init__.py
--rw-r--r--   0 ankur      (501) staff       (20)      128 2024-01-10 00:53:38.000000 braintrust_core-0.0.8/src/braintrust_core/db_fields.py
--rw-r--r--   0 ankur      (501) staff       (20)     3108 2023-12-22 23:17:30.000000 braintrust_core-0.0.8/src/braintrust_core/merge_row_batch.py
--rw-r--r--   0 ankur      (501) staff       (20)     1713 2024-01-10 01:24:38.000000 braintrust_core-0.0.8/src/braintrust_core/score.py
--rw-r--r--   0 ankur      (501) staff       (20)     1158 2023-12-22 23:17:30.000000 braintrust_core-0.0.8/src/braintrust_core/util.py
--rw-r--r--   0 ankur      (501) staff       (20)       18 2024-01-10 01:24:47.000000 braintrust_core-0.0.8/src/braintrust_core/version.py
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2024-01-10 01:29:23.147121 braintrust_core-0.0.8/src/braintrust_core.egg-info/
--rw-r--r--   0 ankur      (501) staff       (20)      502 2024-01-10 01:29:23.000000 braintrust_core-0.0.8/src/braintrust_core.egg-info/PKG-INFO
--rw-r--r--   0 ankur      (501) staff       (20)      382 2024-01-10 01:29:23.000000 braintrust_core-0.0.8/src/braintrust_core.egg-info/SOURCES.txt
--rw-r--r--   0 ankur      (501) staff       (20)        1 2024-01-10 01:29:23.000000 braintrust_core-0.0.8/src/braintrust_core.egg-info/dependency_links.txt
--rw-r--r--   0 ankur      (501) staff       (20)       16 2024-01-10 01:29:23.000000 braintrust_core-0.0.8/src/braintrust_core.egg-info/top_level.txt
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2024-01-12 06:33:27.343187 braintrust_core-0.0.9/
+-rw-r--r--   0 ankur      (501) staff       (20)      502 2024-01-12 06:33:27.342924 braintrust_core-0.0.9/PKG-INFO
+-rw-r--r--   0 ankur      (501) staff       (20)      125 2023-12-22 23:17:30.000000 braintrust_core-0.0.9/README.md
+-rw-r--r--   0 ankur      (501) staff       (20)       38 2024-01-12 06:33:27.343228 braintrust_core-0.0.9/setup.cfg
+-rw-r--r--   0 ankur      (501) staff       (20)     1070 2023-12-22 23:17:30.000000 braintrust_core-0.0.9/setup.py
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2024-01-12 06:33:27.340065 braintrust_core-0.0.9/src/
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2024-01-12 06:33:27.341942 braintrust_core-0.0.9/src/braintrust_core/
+-rw-r--r--   0 ankur      (501) staff       (20)       41 2023-12-22 23:17:30.000000 braintrust_core-0.0.9/src/braintrust_core/__init__.py
+-rw-r--r--   0 ankur      (501) staff       (20)      250 2024-01-12 06:16:25.000000 braintrust_core-0.0.9/src/braintrust_core/db_fields.py
+-rw-r--r--   0 ankur      (501) staff       (20)     3108 2024-01-12 01:29:41.000000 braintrust_core-0.0.9/src/braintrust_core/merge_row_batch.py
+-rw-r--r--   0 ankur      (501) staff       (20)     1713 2024-01-10 01:48:31.000000 braintrust_core-0.0.9/src/braintrust_core/score.py
+-rw-r--r--   0 ankur      (501) staff       (20)     1181 2024-01-12 06:15:04.000000 braintrust_core-0.0.9/src/braintrust_core/util.py
+-rw-r--r--   0 ankur      (501) staff       (20)       18 2024-01-12 06:33:14.000000 braintrust_core-0.0.9/src/braintrust_core/version.py
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2024-01-12 06:33:27.342688 braintrust_core-0.0.9/src/braintrust_core.egg-info/
+-rw-r--r--   0 ankur      (501) staff       (20)      502 2024-01-12 06:33:27.000000 braintrust_core-0.0.9/src/braintrust_core.egg-info/PKG-INFO
+-rw-r--r--   0 ankur      (501) staff       (20)      382 2024-01-12 06:33:27.000000 braintrust_core-0.0.9/src/braintrust_core.egg-info/SOURCES.txt
+-rw-r--r--   0 ankur      (501) staff       (20)        1 2024-01-12 06:33:27.000000 braintrust_core-0.0.9/src/braintrust_core.egg-info/dependency_links.txt
+-rw-r--r--   0 ankur      (501) staff       (20)       16 2024-01-12 06:33:27.000000 braintrust_core-0.0.9/src/braintrust_core.egg-info/top_level.txt
```

### Comparing `braintrust_core-0.0.8/setup.py` & `braintrust_core-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `braintrust_core-0.0.8/src/braintrust_core/merge_row_batch.py` & `braintrust_core-0.0.9/src/braintrust_core/merge_row_batch.py`

 * *Files identical despite different names*

### Comparing `braintrust_core-0.0.8/src/braintrust_core/score.py` & `braintrust_core-0.0.9/src/braintrust_core/score.py`

 * *Files identical despite different names*

### Comparing `braintrust_core-0.0.8/src/braintrust_core/util.py` & `braintrust_core-0.0.9/src/braintrust_core/util.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,7 +34,9 @@
 
     for k, merge_from_v in merge_from.items():
         merge_into_v = merge_into.get(k)
         if isinstance(merge_into_v, dict) and isinstance(merge_from_v, dict):
             merge_dicts(merge_into_v, merge_from_v)
         else:
             merge_into[k] = merge_from_v
+
+    return merge_into
```

