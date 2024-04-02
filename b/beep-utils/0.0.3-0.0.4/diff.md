# Comparing `tmp/beep_utils-0.0.3.tar.gz` & `tmp/beep_utils-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beep_utils-0.0.3.tar", last modified: Mon Apr  1 20:56:30 2024, max compression
+gzip compressed data, was "beep_utils-0.0.4.tar", last modified: Mon Apr  1 21:08:42 2024, max compression
```

## Comparing `beep_utils-0.0.3.tar` & `beep_utils-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 lucaspinho  (1000) lucaspinho  (1000)        0 2024-04-01 20:56:30.845160 beep_utils-0.0.3/
--rw-r--r--   0 lucaspinho  (1000) lucaspinho  (1000)      380 2024-04-01 20:56:30.845160 beep_utils-0.0.3/PKG-INFO
--rw-r--r--   0 lucaspinho  (1000) lucaspinho  (1000)        0 2024-04-01 20:18:26.000000 beep_utils-0.0.3/README.md
-drwxr-xr-x   0 lucaspinho  (1000) lucaspinho  (1000)        0 2024-04-01 20:56:30.845160 beep_utils-0.0.3/beep_utils/
--rw-r--r--   0 lucaspinho  (1000) lucaspinho  (1000)        0 2024-04-01 20:29:20.000000 beep_utils-0.0.3/beep_utils/__init__.py
--rw-r--r--   0 lucaspinho  (1000) lucaspinho  (1000)     3424 2024-04-01 20:56:16.000000 beep_utils-0.0.3/beep_utils/beep_utils.py
-drwxr-xr-x   0 lucaspinho  (1000) lucaspinho  (1000)        0 2024-04-01 20:56:30.845160 beep_utils-0.0.3/beep_utils.egg-info/
--rw-r--r--   0 lucaspinho  (1000) lucaspinho  (1000)      380 2024-04-01 20:56:30.000000 beep_utils-0.0.3/beep_utils.egg-info/PKG-INFO
--rw-r--r--   0 lucaspinho  (1000) lucaspinho  (1000)      202 2024-04-01 20:56:30.000000 beep_utils-0.0.3/beep_utils.egg-info/SOURCES.txt
--rw-r--r--   0 lucaspinho  (1000) lucaspinho  (1000)        1 2024-04-01 20:56:30.000000 beep_utils-0.0.3/beep_utils.egg-info/dependency_links.txt
--rw-r--r--   0 lucaspinho  (1000) lucaspinho  (1000)       11 2024-04-01 20:56:30.000000 beep_utils-0.0.3/beep_utils.egg-info/top_level.txt
--rw-r--r--   0 lucaspinho  (1000) lucaspinho  (1000)       38 2024-04-01 20:56:30.845160 beep_utils-0.0.3/setup.cfg
--rw-r--r--   0 lucaspinho  (1000) lucaspinho  (1000)      622 2024-04-01 20:56:23.000000 beep_utils-0.0.3/setup.py
+drwxr-xr-x   0 lucaspinho  (1000) lucaspinho  (1000)        0 2024-04-01 21:08:42.375160 beep_utils-0.0.4/
+-rw-r--r--   0 lucaspinho  (1000) lucaspinho  (1000)      380 2024-04-01 21:08:42.375160 beep_utils-0.0.4/PKG-INFO
+-rw-r--r--   0 lucaspinho  (1000) lucaspinho  (1000)        0 2024-04-01 20:18:26.000000 beep_utils-0.0.4/README.md
+drwxr-xr-x   0 lucaspinho  (1000) lucaspinho  (1000)        0 2024-04-01 21:08:42.375160 beep_utils-0.0.4/beep_utils/
+-rw-r--r--   0 lucaspinho  (1000) lucaspinho  (1000)       70 2024-04-01 21:08:29.000000 beep_utils-0.0.4/beep_utils/__init__.py
+-rw-r--r--   0 lucaspinho  (1000) lucaspinho  (1000)     3424 2024-04-01 20:56:16.000000 beep_utils-0.0.4/beep_utils/beep_utils.py
+drwxr-xr-x   0 lucaspinho  (1000) lucaspinho  (1000)        0 2024-04-01 21:08:42.375160 beep_utils-0.0.4/beep_utils.egg-info/
+-rw-r--r--   0 lucaspinho  (1000) lucaspinho  (1000)      380 2024-04-01 21:08:42.000000 beep_utils-0.0.4/beep_utils.egg-info/PKG-INFO
+-rw-r--r--   0 lucaspinho  (1000) lucaspinho  (1000)      202 2024-04-01 21:08:42.000000 beep_utils-0.0.4/beep_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 lucaspinho  (1000) lucaspinho  (1000)        1 2024-04-01 21:08:42.000000 beep_utils-0.0.4/beep_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 lucaspinho  (1000) lucaspinho  (1000)       11 2024-04-01 21:08:42.000000 beep_utils-0.0.4/beep_utils.egg-info/top_level.txt
+-rw-r--r--   0 lucaspinho  (1000) lucaspinho  (1000)       38 2024-04-01 21:08:42.375160 beep_utils-0.0.4/setup.cfg
+-rw-r--r--   0 lucaspinho  (1000) lucaspinho  (1000)      550 2024-04-01 21:08:35.000000 beep_utils-0.0.4/setup.py
```

### Comparing `beep_utils-0.0.3/beep_utils/beep_utils.py` & `beep_utils-0.0.4/beep_utils/beep_utils.py`

 * *Files identical despite different names*

