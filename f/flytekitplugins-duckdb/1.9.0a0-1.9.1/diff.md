# Comparing `tmp/flytekitplugins-duckdb-1.9.0a0.tar.gz` & `tmp/flytekitplugins-duckdb-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-duckdb-1.9.0a0.tar", last modified: Thu Jul 20 18:58:17 2023, max compression
+gzip compressed data, was "flytekitplugins-duckdb-1.9.1.tar", last modified: Mon Aug 28 16:43:05 2023, max compression
```

## Comparing `flytekitplugins-duckdb-1.9.0a0.tar` & `flytekitplugins-duckdb-1.9.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:17.720659 flytekitplugins-duckdb-1.9.0a0/
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-20 18:58:17.720659 flytekitplugins-duckdb-1.9.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-20 18:57:54.000000 flytekitplugins-duckdb-1.9.0a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:17.716659 flytekitplugins-duckdb-1.9.0a0/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:17.720659 flytekitplugins-duckdb-1.9.0a0/flytekitplugins/duckdb/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-20 18:57:54.000000 flytekitplugins-duckdb-1.9.0a0/flytekitplugins/duckdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-07-20 18:57:54.000000 flytekitplugins-duckdb-1.9.0a0/flytekitplugins/duckdb/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:17.720659 flytekitplugins-duckdb-1.9.0a0/flytekitplugins_duckdb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-20 18:58:17.000000 flytekitplugins-duckdb-1.9.0a0/flytekitplugins_duckdb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-20 18:58:17.000000 flytekitplugins-duckdb-1.9.0a0/flytekitplugins_duckdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 18:58:17.000000 flytekitplugins-duckdb-1.9.0a0/flytekitplugins_duckdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 18:58:17.000000 flytekitplugins-duckdb-1.9.0a0/flytekitplugins_duckdb.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-20 18:58:17.000000 flytekitplugins-duckdb-1.9.0a0/flytekitplugins_duckdb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 18:58:17.000000 flytekitplugins-duckdb-1.9.0a0/flytekitplugins_duckdb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 18:58:17.720659 flytekitplugins-duckdb-1.9.0a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-20 18:58:12.000000 flytekitplugins-duckdb-1.9.0a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:43:05.274121 flytekitplugins-duckdb-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (999)      838 2023-08-28 16:43:05.274121 flytekitplugins-duckdb-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)      174 2023-08-28 16:42:38.000000 flytekitplugins-duckdb-1.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:43:05.270121 flytekitplugins-duckdb-1.9.1/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:43:05.274121 flytekitplugins-duckdb-1.9.1/flytekitplugins/duckdb/
+-rw-r--r--   0 runner    (1001) docker     (999)      164 2023-08-28 16:42:38.000000 flytekitplugins-duckdb-1.9.1/flytekitplugins/duckdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4633 2023-08-28 16:42:38.000000 flytekitplugins-duckdb-1.9.1/flytekitplugins/duckdb/task.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:43:05.274121 flytekitplugins-duckdb-1.9.1/flytekitplugins_duckdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (999)      838 2023-08-28 16:43:05.000000 flytekitplugins-duckdb-1.9.1/flytekitplugins_duckdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)      368 2023-08-28 16:43:05.000000 flytekitplugins-duckdb-1.9.1/flytekitplugins_duckdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-28 16:43:05.000000 flytekitplugins-duckdb-1.9.1/flytekitplugins_duckdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       16 2023-08-28 16:43:05.000000 flytekitplugins-duckdb-1.9.1/flytekitplugins_duckdb.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       32 2023-08-28 16:43:05.000000 flytekitplugins-duckdb-1.9.1/flytekitplugins_duckdb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       16 2023-08-28 16:43:05.000000 flytekitplugins-duckdb-1.9.1/flytekitplugins_duckdb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       38 2023-08-28 16:43:05.274121 flytekitplugins-duckdb-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (999)     1193 2023-08-28 16:43:00.000000 flytekitplugins-duckdb-1.9.1/setup.py
```

### Comparing `flytekitplugins-duckdb-1.9.0a0/PKG-INFO` & `flytekitplugins-duckdb-1.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-duckdb
-Version: 1.9.0a0
+Version: 1.9.1
 Summary: DuckDB Plugin for Flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-duckdb-1.9.0a0/flytekitplugins/duckdb/task.py` & `flytekitplugins-duckdb-1.9.1/flytekitplugins/duckdb/task.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-duckdb-1.9.0a0/flytekitplugins_duckdb.egg-info/PKG-INFO` & `flytekitplugins-duckdb-1.9.1/flytekitplugins_duckdb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-duckdb
-Version: 1.9.0a0
+Version: 1.9.1
 Summary: DuckDB Plugin for Flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-duckdb-1.9.0a0/setup.py` & `flytekitplugins-duckdb-1.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "duckdb"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit>=1.3.0b2,<2.0.0", "duckdb"]
 
-__version__ = "1.9.0a0"
+__version__ = "1.9.1"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="DuckDB Plugin for Flytekit",
```

