# Comparing `tmp/scrapy-influxdb-exporter-1.0.3.tar.gz` & `tmp/scrapy-influxdb-exporter-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapy-influxdb-exporter-1.0.3.tar", last modified: Tue Apr  2 21:27:06 2024, max compression
+gzip compressed data, was "scrapy-influxdb-exporter-1.0.4.tar", last modified: Tue Apr  2 21:35:22 2024, max compression
```

## Comparing `scrapy-influxdb-exporter-1.0.3.tar` & `scrapy-influxdb-exporter-1.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:27:06.751770 scrapy-influxdb-exporter-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-02 21:27:02.000000 scrapy-influxdb-exporter-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-02 21:27:06.751770 scrapy-influxdb-exporter-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-02 21:27:02.000000 scrapy-influxdb-exporter-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-02 21:27:02.000000 scrapy-influxdb-exporter-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 21:27:06.751770 scrapy-influxdb-exporter-1.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:27:06.747770 scrapy-influxdb-exporter-1.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:27:06.747770 scrapy-influxdb-exporter-1.0.3/src/scrapy_influxdb_exporter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 21:27:02.000000 scrapy-influxdb-exporter-1.0.3/src/scrapy_influxdb_exporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-02 21:27:02.000000 scrapy-influxdb-exporter-1.0.3/src/scrapy_influxdb_exporter/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-02 21:27:02.000000 scrapy-influxdb-exporter-1.0.3/src/scrapy_influxdb_exporter/statscollectors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:27:06.751770 scrapy-influxdb-exporter-1.0.3/src/scrapy_influxdb_exporter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-02 21:27:06.000000 scrapy-influxdb-exporter-1.0.3/src/scrapy_influxdb_exporter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-02 21:27:06.000000 scrapy-influxdb-exporter-1.0.3/src/scrapy_influxdb_exporter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 21:27:06.000000 scrapy-influxdb-exporter-1.0.3/src/scrapy_influxdb_exporter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-02 21:27:06.000000 scrapy-influxdb-exporter-1.0.3/src/scrapy_influxdb_exporter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-02 21:27:06.000000 scrapy-influxdb-exporter-1.0.3/src/scrapy_influxdb_exporter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:35:22.493707 scrapy-influxdb-exporter-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-02 21:35:18.000000 scrapy-influxdb-exporter-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-02 21:35:22.493707 scrapy-influxdb-exporter-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-02 21:35:18.000000 scrapy-influxdb-exporter-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-02 21:35:18.000000 scrapy-influxdb-exporter-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 21:35:22.493707 scrapy-influxdb-exporter-1.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:35:22.489707 scrapy-influxdb-exporter-1.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:35:22.489707 scrapy-influxdb-exporter-1.0.4/src/scrapy_influxdb_exporter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 21:35:18.000000 scrapy-influxdb-exporter-1.0.4/src/scrapy_influxdb_exporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-02 21:35:18.000000 scrapy-influxdb-exporter-1.0.4/src/scrapy_influxdb_exporter/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-02 21:35:18.000000 scrapy-influxdb-exporter-1.0.4/src/scrapy_influxdb_exporter/statscollectors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:35:22.493707 scrapy-influxdb-exporter-1.0.4/src/scrapy_influxdb_exporter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-02 21:35:22.000000 scrapy-influxdb-exporter-1.0.4/src/scrapy_influxdb_exporter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-02 21:35:22.000000 scrapy-influxdb-exporter-1.0.4/src/scrapy_influxdb_exporter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 21:35:22.000000 scrapy-influxdb-exporter-1.0.4/src/scrapy_influxdb_exporter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-02 21:35:22.000000 scrapy-influxdb-exporter-1.0.4/src/scrapy_influxdb_exporter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-02 21:35:22.000000 scrapy-influxdb-exporter-1.0.4/src/scrapy_influxdb_exporter.egg-info/top_level.txt
```

### Comparing `scrapy-influxdb-exporter-1.0.3/LICENSE` & `scrapy-influxdb-exporter-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapy-influxdb-exporter-1.0.3/PKG-INFO` & `scrapy-influxdb-exporter-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapy-influxdb-exporter
-Version: 1.0.3
+Version: 1.0.4
 Summary: A simple package to export Scrapy spider stats to InfluxDB
 Author-email: Stefano Fusai <stefanofusai@gmail.com>
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: influxdb3-python
 Requires-Dist: scrapy
```

### Comparing `scrapy-influxdb-exporter-1.0.3/README.md` & `scrapy-influxdb-exporter-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `scrapy-influxdb-exporter-1.0.3/pyproject.toml` & `scrapy-influxdb-exporter-1.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "scrapy-influxdb-exporter"
-version = "1.0.3"
+version = "1.0.4"
 authors = [{ "name" = "Stefano Fusai", "email" = "stefanofusai@gmail.com" }]
 description = "A simple package to export Scrapy spider stats to InfluxDB"
 readme = "README.md"
 requires-python = ">=3.11"
 dependencies = ["influxdb3-python", "scrapy"]
 
 [tool.mypy]
```

### Comparing `scrapy-influxdb-exporter-1.0.3/src/scrapy_influxdb_exporter/statscollectors.py` & `scrapy-influxdb-exporter-1.0.4/src/scrapy_influxdb_exporter/statscollectors.py`

 * *Files identical despite different names*

### Comparing `scrapy-influxdb-exporter-1.0.3/src/scrapy_influxdb_exporter.egg-info/PKG-INFO` & `scrapy-influxdb-exporter-1.0.4/src/scrapy_influxdb_exporter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapy-influxdb-exporter
-Version: 1.0.3
+Version: 1.0.4
 Summary: A simple package to export Scrapy spider stats to InfluxDB
 Author-email: Stefano Fusai <stefanofusai@gmail.com>
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: influxdb3-python
 Requires-Dist: scrapy
```

