# Comparing `tmp/pycracks-0.8.0.tar.gz` & `tmp/pycracks-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycracks-0.8.0.tar", last modified: Tue Nov  7 03:46:32 2023, max compression
+gzip compressed data, was "pycracks-0.9.0.tar", last modified: Tue Nov  7 03:50:34 2023, max compression
```

## Comparing `pycracks-0.8.0.tar` & `pycracks-0.9.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 03:46:32.361378 pycracks-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-11-07 03:46:22.000000 pycracks-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      392 2023-11-07 03:46:32.361378 pycracks-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      290 2023-11-07 03:46:22.000000 pycracks-0.8.0/Pipfile
--rw-r--r--   0 runner    (1001) docker     (127)      112 2023-11-07 03:46:22.000000 pycracks-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 03:46:32.361378 pycracks-0.8.0/pycracks/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-11-07 03:46:22.000000 pycracks-0.8.0/pycracks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2023-11-07 03:46:22.000000 pycracks-0.8.0/pycracks/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2023-11-07 03:46:22.000000 pycracks-0.8.0/pycracks/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2392 2023-11-07 03:46:22.000000 pycracks-0.8.0/pycracks/pycracks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 03:46:32.361378 pycracks-0.8.0/pycracks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      392 2023-11-07 03:46:32.000000 pycracks-0.8.0/pycracks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      320 2023-11-07 03:46:32.000000 pycracks-0.8.0/pycracks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-07 03:46:32.000000 pycracks-0.8.0/pycracks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2023-11-07 03:46:32.000000 pycracks-0.8.0/pycracks.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-11-07 03:46:32.000000 pycracks-0.8.0/pycracks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-11-07 03:46:32.000000 pycracks-0.8.0/pycracks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2023-11-07 03:46:22.000000 pycracks-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-07 03:46:32.361378 pycracks-0.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 03:50:34.146208 pycracks-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2023-11-07 03:50:21.000000 pycracks-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2023-11-07 03:50:34.146208 pycracks-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2023-11-07 03:50:21.000000 pycracks-0.9.0/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2023-11-07 03:50:21.000000 pycracks-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 03:50:34.142208 pycracks-0.9.0/pycracks/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2023-11-07 03:50:21.000000 pycracks-0.9.0/pycracks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2023-11-07 03:50:21.000000 pycracks-0.9.0/pycracks/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2023-11-07 03:50:21.000000 pycracks-0.9.0/pycracks/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2023-11-07 03:50:21.000000 pycracks-0.9.0/pycracks/pycracks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 03:50:34.146208 pycracks-0.9.0/pycracks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2023-11-07 03:50:34.000000 pycracks-0.9.0/pycracks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2023-11-07 03:50:34.000000 pycracks-0.9.0/pycracks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-07 03:50:34.000000 pycracks-0.9.0/pycracks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2023-11-07 03:50:34.000000 pycracks-0.9.0/pycracks.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2023-11-07 03:50:34.000000 pycracks-0.9.0/pycracks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-11-07 03:50:34.000000 pycracks-0.9.0/pycracks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2023-11-07 03:50:21.000000 pycracks-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-07 03:50:34.146208 pycracks-0.9.0/setup.cfg
```

### Comparing `pycracks-0.8.0/pycracks/__main__.py` & `pycracks-0.9.0/pycracks/__main__.py`

 * *Files identical despite different names*

### Comparing `pycracks-0.8.0/pycracks/pycracks.py` & `pycracks-0.9.0/pycracks/pycracks.py`

 * *Files identical despite different names*

### Comparing `pycracks-0.8.0/pyproject.toml` & `pycracks-0.9.0/pyproject.toml`

 * *Files identical despite different names*

