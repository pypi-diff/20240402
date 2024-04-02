# Comparing `tmp/flytekitplugins-spark-1.9.0a0.tar.gz` & `tmp/flytekitplugins-spark-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-spark-1.9.0a0.tar", last modified: Thu Jul 20 18:58:26 2023, max compression
+gzip compressed data, was "flytekitplugins-spark-1.9.1.tar", last modified: Mon Aug 28 16:43:14 2023, max compression
```

## Comparing `flytekitplugins-spark-1.9.0a0.tar` & `flytekitplugins-spark-1.9.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:26.876752 flytekitplugins-spark-1.9.0a0/
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-20 18:58:26.876752 flytekitplugins-spark-1.9.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-20 18:57:54.000000 flytekitplugins-spark-1.9.0a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:26.872752 flytekitplugins-spark-1.9.0a0/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:26.876752 flytekitplugins-spark-1.9.0a0/flytekitplugins/spark/
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-07-20 18:57:54.000000 flytekitplugins-spark-1.9.0a0/flytekitplugins/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-07-20 18:57:54.000000 flytekitplugins-spark-1.9.0a0/flytekitplugins/spark/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-07-20 18:57:54.000000 flytekitplugins-spark-1.9.0a0/flytekitplugins/spark/pyspark_transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-07-20 18:57:54.000000 flytekitplugins-spark-1.9.0a0/flytekitplugins/spark/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-07-20 18:57:54.000000 flytekitplugins-spark-1.9.0a0/flytekitplugins/spark/sd_transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-07-20 18:57:54.000000 flytekitplugins-spark-1.9.0a0/flytekitplugins/spark/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:26.876752 flytekitplugins-spark-1.9.0a0/flytekitplugins_spark.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-20 18:58:26.000000 flytekitplugins-spark-1.9.0a0/flytekitplugins_spark.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-20 18:58:26.000000 flytekitplugins-spark-1.9.0a0/flytekitplugins_spark.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 18:58:26.000000 flytekitplugins-spark-1.9.0a0/flytekitplugins_spark.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-20 18:58:26.000000 flytekitplugins-spark-1.9.0a0/flytekitplugins_spark.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 18:58:26.000000 flytekitplugins-spark-1.9.0a0/flytekitplugins_spark.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-20 18:58:26.000000 flytekitplugins-spark-1.9.0a0/flytekitplugins_spark.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 18:58:26.000000 flytekitplugins-spark-1.9.0a0/flytekitplugins_spark.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:26.876752 flytekitplugins-spark-1.9.0a0/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-07-20 18:57:54.000000 flytekitplugins-spark-1.9.0a0/scripts/flytekit_install_spark3.sh
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 18:58:26.876752 flytekitplugins-spark-1.9.0a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-20 18:58:13.000000 flytekitplugins-spark-1.9.0a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:43:14.006132 flytekitplugins-spark-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (999)      782 2023-08-28 16:43:14.006132 flytekitplugins-spark-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)     1203 2023-08-28 16:42:38.000000 flytekitplugins-spark-1.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:43:13.998132 flytekitplugins-spark-1.9.1/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:43:14.002132 flytekitplugins-spark-1.9.1/flytekitplugins/spark/
+-rw-r--r--   0 runner    (1001) docker     (999)      736 2023-08-28 16:42:38.000000 flytekitplugins-spark-1.9.1/flytekitplugins/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     7019 2023-08-28 16:42:38.000000 flytekitplugins-spark-1.9.1/flytekitplugins/spark/models.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1418 2023-08-28 16:42:38.000000 flytekitplugins-spark-1.9.1/flytekitplugins/spark/pyspark_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3908 2023-08-28 16:42:38.000000 flytekitplugins-spark-1.9.1/flytekitplugins/spark/schema.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2609 2023-08-28 16:42:38.000000 flytekitplugins-spark-1.9.1/flytekitplugins/spark/sd_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (999)     8208 2023-08-28 16:42:38.000000 flytekitplugins-spark-1.9.1/flytekitplugins/spark/task.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:43:14.002132 flytekitplugins-spark-1.9.1/flytekitplugins_spark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (999)      782 2023-08-28 16:43:13.000000 flytekitplugins-spark-1.9.1/flytekitplugins_spark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)      594 2023-08-28 16:43:13.000000 flytekitplugins-spark-1.9.1/flytekitplugins_spark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-28 16:43:13.000000 flytekitplugins-spark-1.9.1/flytekitplugins_spark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       49 2023-08-28 16:43:13.000000 flytekitplugins-spark-1.9.1/flytekitplugins_spark.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       16 2023-08-28 16:43:13.000000 flytekitplugins-spark-1.9.1/flytekitplugins_spark.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       40 2023-08-28 16:43:13.000000 flytekitplugins-spark-1.9.1/flytekitplugins_spark.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       16 2023-08-28 16:43:13.000000 flytekitplugins-spark-1.9.1/flytekitplugins_spark.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:43:14.006132 flytekitplugins-spark-1.9.1/scripts/
+-rw-r--r--   0 runner    (1001) docker     (999)     1892 2023-08-28 16:42:38.000000 flytekitplugins-spark-1.9.1/scripts/flytekit_install_spark3.sh
+-rw-r--r--   0 runner    (1001) docker     (999)       38 2023-08-28 16:43:14.006132 flytekitplugins-spark-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (999)     1287 2023-08-28 16:43:00.000000 flytekitplugins-spark-1.9.1/setup.py
```

### Comparing `flytekitplugins-spark-1.9.0a0/PKG-INFO` & `flytekitplugins-spark-1.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-spark
-Version: 1.9.0a0
+Version: 1.9.1
 Summary: Spark 3 plugin for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-spark-1.9.0a0/README.md` & `flytekitplugins-spark-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-spark-1.9.0a0/flytekitplugins/spark/__init__.py` & `flytekitplugins-spark-1.9.1/flytekitplugins/spark/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-spark-1.9.0a0/flytekitplugins/spark/models.py` & `flytekitplugins-spark-1.9.1/flytekitplugins/spark/models.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-spark-1.9.0a0/flytekitplugins/spark/pyspark_transformers.py` & `flytekitplugins-spark-1.9.1/flytekitplugins/spark/pyspark_transformers.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-spark-1.9.0a0/flytekitplugins/spark/schema.py` & `flytekitplugins-spark-1.9.1/flytekitplugins/spark/schema.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-spark-1.9.0a0/flytekitplugins/spark/sd_transformers.py` & `flytekitplugins-spark-1.9.1/flytekitplugins/spark/sd_transformers.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-spark-1.9.0a0/flytekitplugins/spark/task.py` & `flytekitplugins-spark-1.9.1/flytekitplugins/spark/task.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-spark-1.9.0a0/flytekitplugins_spark.egg-info/PKG-INFO` & `flytekitplugins-spark-1.9.1/flytekitplugins_spark.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-spark
-Version: 1.9.0a0
+Version: 1.9.1
 Summary: Spark 3 plugin for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-spark-1.9.0a0/flytekitplugins_spark.egg-info/SOURCES.txt` & `flytekitplugins-spark-1.9.1/flytekitplugins_spark.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flytekitplugins-spark-1.9.0a0/scripts/flytekit_install_spark3.sh` & `flytekitplugins-spark-1.9.1/scripts/flytekit_install_spark3.sh`

 * *Files identical despite different names*

### Comparing `flytekitplugins-spark-1.9.0a0/setup.py` & `flytekitplugins-spark-1.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "spark"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit>=1.3.0b2,<2.0.0", "pyspark>=3.0.0"]
 
-__version__ = "1.9.0a0"
+__version__ = "1.9.1"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="Spark 3 plugin for flytekit",
```

