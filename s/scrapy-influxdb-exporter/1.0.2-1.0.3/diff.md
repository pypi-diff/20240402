# Comparing `tmp/scrapy-influxdb-exporter-1.0.2.tar.gz` & `tmp/scrapy-influxdb-exporter-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapy-influxdb-exporter-1.0.2.tar", last modified: Tue Apr  2 21:05:23 2024, max compression
+gzip compressed data, was "scrapy-influxdb-exporter-1.0.3.tar", last modified: Tue Apr  2 21:27:06 2024, max compression
```

## Comparing `scrapy-influxdb-exporter-1.0.2.tar` & `scrapy-influxdb-exporter-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 stefano    (501) staff       (20)        0 2024-04-02 21:05:23.831892 scrapy-influxdb-exporter-1.0.2/
--rw-r--r--   0 stefano    (501) staff       (20)     1085 2024-04-02 20:05:10.000000 scrapy-influxdb-exporter-1.0.2/LICENSE
--rw-r--r--   0 stefano    (501) staff       (20)     1440 2024-04-02 21:05:23.831677 scrapy-influxdb-exporter-1.0.2/PKG-INFO
--rw-r--r--   0 stefano    (501) staff       (20)     1110 2024-04-02 20:52:51.000000 scrapy-influxdb-exporter-1.0.2/README.md
--rw-r--r--   0 stefano    (501) staff       (20)      888 2024-04-02 21:05:01.000000 scrapy-influxdb-exporter-1.0.2/pyproject.toml
--rw-r--r--   0 stefano    (501) staff       (20)       38 2024-04-02 21:05:23.831937 scrapy-influxdb-exporter-1.0.2/setup.cfg
-drwxr-xr-x   0 stefano    (501) staff       (20)        0 2024-04-02 21:05:23.829373 scrapy-influxdb-exporter-1.0.2/src/
-drwxr-xr-x   0 stefano    (501) staff       (20)        0 2024-04-02 21:05:23.830413 scrapy-influxdb-exporter-1.0.2/src/scrapy_influxdb_exporter/
--rw-r--r--   0 stefano    (501) staff       (20)        0 2024-04-02 19:53:43.000000 scrapy-influxdb-exporter-1.0.2/src/scrapy_influxdb_exporter/__init__.py
--rw-r--r--   0 stefano    (501) staff       (20)      196 2024-04-02 20:28:27.000000 scrapy-influxdb-exporter-1.0.2/src/scrapy_influxdb_exporter/exceptions.py
--rw-r--r--   0 stefano    (501) staff       (20)     1664 2024-04-02 21:05:05.000000 scrapy-influxdb-exporter-1.0.2/src/scrapy_influxdb_exporter/statscollectors.py
-drwxr-xr-x   0 stefano    (501) staff       (20)        0 2024-04-02 21:05:23.831434 scrapy-influxdb-exporter-1.0.2/src/scrapy_influxdb_exporter.egg-info/
--rw-r--r--   0 stefano    (501) staff       (20)     1440 2024-04-02 21:05:23.000000 scrapy-influxdb-exporter-1.0.2/src/scrapy_influxdb_exporter.egg-info/PKG-INFO
--rw-r--r--   0 stefano    (501) staff       (20)      423 2024-04-02 21:05:23.000000 scrapy-influxdb-exporter-1.0.2/src/scrapy_influxdb_exporter.egg-info/SOURCES.txt
--rw-r--r--   0 stefano    (501) staff       (20)        1 2024-04-02 21:05:23.000000 scrapy-influxdb-exporter-1.0.2/src/scrapy_influxdb_exporter.egg-info/dependency_links.txt
--rw-r--r--   0 stefano    (501) staff       (20)       24 2024-04-02 21:05:23.000000 scrapy-influxdb-exporter-1.0.2/src/scrapy_influxdb_exporter.egg-info/requires.txt
--rw-r--r--   0 stefano    (501) staff       (20)       25 2024-04-02 21:05:23.000000 scrapy-influxdb-exporter-1.0.2/src/scrapy_influxdb_exporter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:27:06.751770 scrapy-influxdb-exporter-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-02 21:27:02.000000 scrapy-influxdb-exporter-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-02 21:27:06.751770 scrapy-influxdb-exporter-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-02 21:27:02.000000 scrapy-influxdb-exporter-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-02 21:27:02.000000 scrapy-influxdb-exporter-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 21:27:06.751770 scrapy-influxdb-exporter-1.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:27:06.747770 scrapy-influxdb-exporter-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:27:06.747770 scrapy-influxdb-exporter-1.0.3/src/scrapy_influxdb_exporter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 21:27:02.000000 scrapy-influxdb-exporter-1.0.3/src/scrapy_influxdb_exporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-02 21:27:02.000000 scrapy-influxdb-exporter-1.0.3/src/scrapy_influxdb_exporter/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-02 21:27:02.000000 scrapy-influxdb-exporter-1.0.3/src/scrapy_influxdb_exporter/statscollectors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:27:06.751770 scrapy-influxdb-exporter-1.0.3/src/scrapy_influxdb_exporter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-02 21:27:06.000000 scrapy-influxdb-exporter-1.0.3/src/scrapy_influxdb_exporter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-02 21:27:06.000000 scrapy-influxdb-exporter-1.0.3/src/scrapy_influxdb_exporter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 21:27:06.000000 scrapy-influxdb-exporter-1.0.3/src/scrapy_influxdb_exporter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-02 21:27:06.000000 scrapy-influxdb-exporter-1.0.3/src/scrapy_influxdb_exporter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-02 21:27:06.000000 scrapy-influxdb-exporter-1.0.3/src/scrapy_influxdb_exporter.egg-info/top_level.txt
```

### Comparing `scrapy-influxdb-exporter-1.0.2/LICENSE` & `scrapy-influxdb-exporter-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapy-influxdb-exporter-1.0.2/PKG-INFO` & `scrapy-influxdb-exporter-1.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapy-influxdb-exporter
-Version: 1.0.2
+Version: 1.0.3
 Summary: A simple package to export Scrapy spider stats to InfluxDB
 Author-email: Stefano Fusai <stefanofusai@gmail.com>
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: influxdb3-python
 Requires-Dist: scrapy
```

### Comparing `scrapy-influxdb-exporter-1.0.2/README.md` & `scrapy-influxdb-exporter-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `scrapy-influxdb-exporter-1.0.2/pyproject.toml` & `scrapy-influxdb-exporter-1.0.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "scrapy-influxdb-exporter"
-version = "1.0.2"
+version = "1.0.3"
 authors = [{ "name" = "Stefano Fusai", "email" = "stefanofusai@gmail.com" }]
 description = "A simple package to export Scrapy spider stats to InfluxDB"
 readme = "README.md"
 requires-python = ">=3.11"
 dependencies = ["influxdb3-python", "scrapy"]
 
 [tool.mypy]
```

### Comparing `scrapy-influxdb-exporter-1.0.2/src/scrapy_influxdb_exporter/statscollectors.py` & `scrapy-influxdb-exporter-1.0.3/src/scrapy_influxdb_exporter/statscollectors.py`

 * *Files identical despite different names*

### Comparing `scrapy-influxdb-exporter-1.0.2/src/scrapy_influxdb_exporter.egg-info/PKG-INFO` & `scrapy-influxdb-exporter-1.0.3/src/scrapy_influxdb_exporter.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapy-influxdb-exporter
-Version: 1.0.2
+Version: 1.0.3
 Summary: A simple package to export Scrapy spider stats to InfluxDB
 Author-email: Stefano Fusai <stefanofusai@gmail.com>
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: influxdb3-python
 Requires-Dist: scrapy
```

