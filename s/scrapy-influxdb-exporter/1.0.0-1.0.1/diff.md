# Comparing `tmp/scrapy-influxdb-exporter-1.0.0.tar.gz` & `tmp/scrapy-influxdb-exporter-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapy-influxdb-exporter-1.0.0.tar", last modified: Tue Apr  2 20:52:13 2024, max compression
+gzip compressed data, was "scrapy-influxdb-exporter-1.0.1.tar", last modified: Tue Apr  2 21:03:31 2024, max compression
```

## Comparing `scrapy-influxdb-exporter-1.0.0.tar` & `scrapy-influxdb-exporter-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 stefano    (501) staff       (20)        0 2024-04-02 20:52:13.490809 scrapy-influxdb-exporter-1.0.0/
--rw-r--r--   0 stefano    (501) staff       (20)     1085 2024-04-02 20:05:10.000000 scrapy-influxdb-exporter-1.0.0/LICENSE
--rw-r--r--   0 stefano    (501) staff       (20)     1441 2024-04-02 20:52:13.490599 scrapy-influxdb-exporter-1.0.0/PKG-INFO
--rw-r--r--   0 stefano    (501) staff       (20)     1110 2024-04-02 20:38:56.000000 scrapy-influxdb-exporter-1.0.0/README.md
--rw-r--r--   0 stefano    (501) staff       (20)      888 2024-04-02 20:23:54.000000 scrapy-influxdb-exporter-1.0.0/pyproject.toml
--rw-r--r--   0 stefano    (501) staff       (20)       38 2024-04-02 20:52:13.490861 scrapy-influxdb-exporter-1.0.0/setup.cfg
-drwxr-xr-x   0 stefano    (501) staff       (20)        0 2024-04-02 20:52:13.487543 scrapy-influxdb-exporter-1.0.0/src/
-drwxr-xr-x   0 stefano    (501) staff       (20)        0 2024-04-02 20:52:13.489138 scrapy-influxdb-exporter-1.0.0/src/scrapy_influxdb_exporter/
--rw-r--r--   0 stefano    (501) staff       (20)        0 2024-04-02 19:53:43.000000 scrapy-influxdb-exporter-1.0.0/src/scrapy_influxdb_exporter/__init__.py
--rw-r--r--   0 stefano    (501) staff       (20)      196 2024-04-02 20:28:27.000000 scrapy-influxdb-exporter-1.0.0/src/scrapy_influxdb_exporter/exceptions.py
--rw-r--r--   0 stefano    (501) staff       (20)     1662 2024-04-02 20:47:39.000000 scrapy-influxdb-exporter-1.0.0/src/scrapy_influxdb_exporter/statscollectors.py
-drwxr-xr-x   0 stefano    (501) staff       (20)        0 2024-04-02 20:52:13.490349 scrapy-influxdb-exporter-1.0.0/src/scrapy_influxdb_exporter.egg-info/
--rw-r--r--   0 stefano    (501) staff       (20)     1441 2024-04-02 20:52:13.000000 scrapy-influxdb-exporter-1.0.0/src/scrapy_influxdb_exporter.egg-info/PKG-INFO
--rw-r--r--   0 stefano    (501) staff       (20)      423 2024-04-02 20:52:13.000000 scrapy-influxdb-exporter-1.0.0/src/scrapy_influxdb_exporter.egg-info/SOURCES.txt
--rw-r--r--   0 stefano    (501) staff       (20)        1 2024-04-02 20:52:13.000000 scrapy-influxdb-exporter-1.0.0/src/scrapy_influxdb_exporter.egg-info/dependency_links.txt
--rw-r--r--   0 stefano    (501) staff       (20)       24 2024-04-02 20:52:13.000000 scrapy-influxdb-exporter-1.0.0/src/scrapy_influxdb_exporter.egg-info/requires.txt
--rw-r--r--   0 stefano    (501) staff       (20)       25 2024-04-02 20:52:13.000000 scrapy-influxdb-exporter-1.0.0/src/scrapy_influxdb_exporter.egg-info/top_level.txt
+drwxr-xr-x   0 stefano    (501) staff       (20)        0 2024-04-02 21:03:31.209801 scrapy-influxdb-exporter-1.0.1/
+-rw-r--r--   0 stefano    (501) staff       (20)     1085 2024-04-02 20:05:10.000000 scrapy-influxdb-exporter-1.0.1/LICENSE
+-rw-r--r--   0 stefano    (501) staff       (20)     1440 2024-04-02 21:03:31.209618 scrapy-influxdb-exporter-1.0.1/PKG-INFO
+-rw-r--r--   0 stefano    (501) staff       (20)     1110 2024-04-02 20:52:51.000000 scrapy-influxdb-exporter-1.0.1/README.md
+-rw-r--r--   0 stefano    (501) staff       (20)      888 2024-04-02 21:03:26.000000 scrapy-influxdb-exporter-1.0.1/pyproject.toml
+-rw-r--r--   0 stefano    (501) staff       (20)       38 2024-04-02 21:03:31.209843 scrapy-influxdb-exporter-1.0.1/setup.cfg
+drwxr-xr-x   0 stefano    (501) staff       (20)        0 2024-04-02 21:03:31.207416 scrapy-influxdb-exporter-1.0.1/src/
+drwxr-xr-x   0 stefano    (501) staff       (20)        0 2024-04-02 21:03:31.208460 scrapy-influxdb-exporter-1.0.1/src/scrapy_influxdb_exporter/
+-rw-r--r--   0 stefano    (501) staff       (20)        0 2024-04-02 19:53:43.000000 scrapy-influxdb-exporter-1.0.1/src/scrapy_influxdb_exporter/__init__.py
+-rw-r--r--   0 stefano    (501) staff       (20)      196 2024-04-02 20:28:27.000000 scrapy-influxdb-exporter-1.0.1/src/scrapy_influxdb_exporter/exceptions.py
+-rw-r--r--   0 stefano    (501) staff       (20)     1662 2024-04-02 20:47:39.000000 scrapy-influxdb-exporter-1.0.1/src/scrapy_influxdb_exporter/statscollectors.py
+drwxr-xr-x   0 stefano    (501) staff       (20)        0 2024-04-02 21:03:31.209411 scrapy-influxdb-exporter-1.0.1/src/scrapy_influxdb_exporter.egg-info/
+-rw-r--r--   0 stefano    (501) staff       (20)     1440 2024-04-02 21:03:31.000000 scrapy-influxdb-exporter-1.0.1/src/scrapy_influxdb_exporter.egg-info/PKG-INFO
+-rw-r--r--   0 stefano    (501) staff       (20)      423 2024-04-02 21:03:31.000000 scrapy-influxdb-exporter-1.0.1/src/scrapy_influxdb_exporter.egg-info/SOURCES.txt
+-rw-r--r--   0 stefano    (501) staff       (20)        1 2024-04-02 21:03:31.000000 scrapy-influxdb-exporter-1.0.1/src/scrapy_influxdb_exporter.egg-info/dependency_links.txt
+-rw-r--r--   0 stefano    (501) staff       (20)       24 2024-04-02 21:03:31.000000 scrapy-influxdb-exporter-1.0.1/src/scrapy_influxdb_exporter.egg-info/requires.txt
+-rw-r--r--   0 stefano    (501) staff       (20)       25 2024-04-02 21:03:31.000000 scrapy-influxdb-exporter-1.0.1/src/scrapy_influxdb_exporter.egg-info/top_level.txt
```

### Comparing `scrapy-influxdb-exporter-1.0.0/LICENSE` & `scrapy-influxdb-exporter-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapy-influxdb-exporter-1.0.0/PKG-INFO` & `scrapy-influxdb-exporter-1.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapy-influxdb-exporter
-Version: 1.0.0
+Version: 1.0.1
 Summary: A simple package to export Scrapy spider stats to InfluxDB
 Author-email: Stefano Fusai <stefanofusai@gmail.com>
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: influxdb3-python
 Requires-Dist: scrapy
@@ -29,9 +29,9 @@
 
 ## Acknowledgments
 This project was inspired by [scrapy-prometheus-exporter](https://github.com/rangertaha/scrapy-prometheus-exporter) by [@rangertaha](https://github.com/rangertaha) and [this article](https://mikulskibartosz.name/how-to-monitor-scrapy-spiders-using-influxdb-and-grafana) by [@mikulskibartosz](https://github.com/mikulskibartosz).
 
 ## Contributing
 Contributions are welcome! To get started, please refer to our [contribution guidelines](https://github.com/stefanofusai/scrapy-influxdb-exporter/blob/main/CONTRIBUTING.md).
 
-## Issues
+## Issues
 If you encounter any problems while using this package, please open a new issue [here](https://github.com/stefanofusai/scrapy-influxdb-exporter/issues).
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `scrapy-influxdb-exporter-1.0.0/README.md` & `scrapy-influxdb-exporter-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -18,9 +18,9 @@
 
 ## Acknowledgments
 This project was inspired by [scrapy-prometheus-exporter](https://github.com/rangertaha/scrapy-prometheus-exporter) by [@rangertaha](https://github.com/rangertaha) and [this article](https://mikulskibartosz.name/how-to-monitor-scrapy-spiders-using-influxdb-and-grafana) by [@mikulskibartosz](https://github.com/mikulskibartosz).
 
 ## Contributing
 Contributions are welcome! To get started, please refer to our [contribution guidelines](https://github.com/stefanofusai/scrapy-influxdb-exporter/blob/main/CONTRIBUTING.md).
 
-## Issues
-If you encounter any problems while using this package, please open a new issue [here](https://github.com/stefanofusai/scrapy-influxdb-exporter/issues).
+## Issues
+If you encounter any problems while using this package, please open a new issue [here](https://github.com/stefanofusai/scrapy-influxdb-exporter/issues).
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `scrapy-influxdb-exporter-1.0.0/pyproject.toml` & `scrapy-influxdb-exporter-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "scrapy-influxdb-exporter"
-version = "1.0.0"
+version = "1.0.1"
 authors = [{ "name" = "Stefano Fusai", "email" = "stefanofusai@gmail.com" }]
 description = "A simple package to export Scrapy spider stats to InfluxDB"
 readme = "README.md"
 requires-python = ">=3.11"
 dependencies = ["influxdb3-python", "scrapy"]
 
 [tool.mypy]
```

### Comparing `scrapy-influxdb-exporter-1.0.0/src/scrapy_influxdb_exporter/statscollectors.py` & `scrapy-influxdb-exporter-1.0.1/src/scrapy_influxdb_exporter/statscollectors.py`

 * *Files identical despite different names*

### Comparing `scrapy-influxdb-exporter-1.0.0/src/scrapy_influxdb_exporter.egg-info/PKG-INFO` & `scrapy-influxdb-exporter-1.0.1/src/scrapy_influxdb_exporter.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapy-influxdb-exporter
-Version: 1.0.0
+Version: 1.0.1
 Summary: A simple package to export Scrapy spider stats to InfluxDB
 Author-email: Stefano Fusai <stefanofusai@gmail.com>
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: influxdb3-python
 Requires-Dist: scrapy
@@ -29,9 +29,9 @@
 
 ## Acknowledgments
 This project was inspired by [scrapy-prometheus-exporter](https://github.com/rangertaha/scrapy-prometheus-exporter) by [@rangertaha](https://github.com/rangertaha) and [this article](https://mikulskibartosz.name/how-to-monitor-scrapy-spiders-using-influxdb-and-grafana) by [@mikulskibartosz](https://github.com/mikulskibartosz).
 
 ## Contributing
 Contributions are welcome! To get started, please refer to our [contribution guidelines](https://github.com/stefanofusai/scrapy-influxdb-exporter/blob/main/CONTRIBUTING.md).
 
-## Issues
+## Issues
 If you encounter any problems while using this package, please open a new issue [here](https://github.com/stefanofusai/scrapy-influxdb-exporter/issues).
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

