# Comparing `tmp/temod-2.0.8.tar.gz` & `tmp/temod-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "temod-2.0.8.tar", last modified: Sun Mar 24 12:39:44 2024, max compression
+gzip compressed data, was "temod-2.0.9.tar", last modified: Tue Apr  2 10:06:42 2024, max compression
```

## Comparing `temod-2.0.8.tar` & `temod-2.0.9.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-03-24 12:39:44.223231 temod-2.0.8/
--rw-rw-r--   0 oem      (29999) oem      (29999)     1069 2023-07-16 09:53:35.000000 temod-2.0.8/LICENSE.txt
--rw-r--r--   0 oem      (29999) oem      (29999)      703 2024-03-24 12:39:44.223231 temod-2.0.8/PKG-INFO
--rw-rw-r--   0 oem      (29999) oem      (29999)       67 2023-07-16 09:51:01.000000 temod-2.0.8/README.md
--rw-rw-r--   0 oem      (29999) oem      (29999)      704 2024-03-24 12:39:35.000000 temod-2.0.8/pyproject.toml
--rw-rw-r--   0 oem      (29999) oem      (29999)       38 2024-03-24 12:39:44.223231 temod-2.0.8/setup.cfg
-drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-03-24 12:39:44.223231 temod-2.0.8/src/
-drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-03-24 12:39:44.223231 temod-2.0.8/src/temod/
--rw-rw-r--   0 oem      (29999) oem      (29999)       27 2023-07-15 13:43:54.000000 temod-2.0.8/src/temod/__init__.py
-drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-03-24 12:39:44.223231 temod-2.0.8/src/temod/base/
--rw-rw-r--   0 oem      (29999) oem      (29999)      145 2023-07-15 13:44:09.000000 temod-2.0.8/src/temod/base/__init__.py
--rw-rw-r--   0 oem      (29999) oem      (29999)     9973 2024-03-24 12:34:15.000000 temod-2.0.8/src/temod/base/attribute.py
--rw-rw-r--   0 oem      (29999) oem      (29999)     1697 2023-07-15 13:44:06.000000 temod-2.0.8/src/temod/base/cluster.py
--rw-rw-r--   0 oem      (29999) oem      (29999)     2900 2023-07-15 13:44:09.000000 temod-2.0.8/src/temod/base/condition.py
--rw-rw-r--   0 oem      (29999) oem      (29999)     1986 2023-07-15 13:44:10.000000 temod-2.0.8/src/temod/base/constraint.py
--rw-rw-r--   0 oem      (29999) oem      (29999)     6238 2023-07-15 13:44:09.000000 temod-2.0.8/src/temod/base/entity.py
--rw-rw-r--   0 oem      (29999) oem      (29999)     1481 2023-07-15 13:44:09.000000 temod-2.0.8/src/temod/base/exceptions.py
--rw-rw-r--   0 oem      (29999) oem      (29999)     2557 2023-07-15 13:44:10.000000 temod-2.0.8/src/temod/base/join.py
-drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-03-24 12:39:44.223231 temod-2.0.8/src/temod/ext/
--rw-rw-r--   0 oem      (29999) oem      (29999)    11228 2023-07-15 13:43:55.000000 temod-2.0.8/src/temod/ext/holders.py
-drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-03-24 12:39:44.223231 temod-2.0.8/src/temod/operators/
--rw-rw-r--   0 oem      (29999) oem      (29999)      451 2023-07-15 13:43:22.000000 temod-2.0.8/src/temod/operators/aggregation.py
-drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-03-24 12:39:44.223231 temod-2.0.8/src/temod/storage/
--rw-rw-r--   0 oem      (29999) oem      (29999)      201 2023-07-15 13:43:59.000000 temod-2.0.8/src/temod/storage/__init__.py
-drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-03-24 12:39:44.223231 temod-2.0.8/src/temod/storage/directory/
--rw-rw-r--   0 oem      (29999) oem      (29999)       59 2023-07-15 13:43:57.000000 temod-2.0.8/src/temod/storage/directory/__init__.py
--rw-rw-r--   0 oem      (29999) oem      (29999)     5004 2023-07-15 13:43:57.000000 temod-2.0.8/src/temod/storage/directory/directoryStorage.py
--rw-rw-r--   0 oem      (29999) oem      (29999)     2835 2023-07-15 13:43:55.000000 temod-2.0.8/src/temod/storage/directory/yamlStorage.py
-drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-03-24 12:39:44.223231 temod-2.0.8/src/temod/storage/exceptions/
--rw-rw-r--   0 oem      (29999) oem      (29999)      774 2023-07-15 13:43:58.000000 temod-2.0.8/src/temod/storage/exceptions/entities.py
--rw-rw-r--   0 oem      (29999) oem      (29999)      541 2023-07-15 13:43:58.000000 temod-2.0.8/src/temod/storage/exceptions/joins.py
--rw-rw-r--   0 oem      (29999) oem      (29999)      418 2023-07-15 13:43:58.000000 temod-2.0.8/src/temod/storage/exceptions/translators.py
-drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-03-24 12:39:44.223231 temod-2.0.8/src/temod/storage/influxdb/
--rw-rw-r--   0 oem      (29999) oem      (29999)     9803 2024-02-25 20:41:24.000000 temod-2.0.8/src/temod/storage/influxdb/influxEntityStorage.py
--rw-rw-r--   0 oem      (29999) oem      (29999)     2363 2024-02-25 20:41:37.000000 temod-2.0.8/src/temod/storage/influxdb/influxStorage.py
--rw-rw-r--   0 oem      (29999) oem      (29999)     6019 2023-07-15 13:43:59.000000 temod-2.0.8/src/temod/storage/influxdb/influxTranslators.py
-drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-03-24 12:39:44.223231 temod-2.0.8/src/temod/storage/mysql/
--rw-rw-r--   0 oem      (29999) oem      (29999)      131 2023-07-15 13:44:05.000000 temod-2.0.8/src/temod/storage/mysql/__init__.py
--rw-rw-r--   0 oem      (29999) oem      (29999)     2416 2023-07-15 13:44:01.000000 temod-2.0.8/src/temod/storage/mysql/mysqlAttributesTranslator.py
--rw-rw-r--   0 oem      (29999) oem      (29999)     6604 2024-02-25 20:41:49.000000 temod-2.0.8/src/temod/storage/mysql/mysqlClusterStorage.py
--rw-rw-r--   0 oem      (29999) oem      (29999)     4235 2023-07-15 13:44:05.000000 temod-2.0.8/src/temod/storage/mysql/mysqlConditionsTranslator.py
--rw-rw-r--   0 oem      (29999) oem      (29999)     9767 2024-03-24 11:57:03.000000 temod-2.0.8/src/temod/storage/mysql/mysqlEntityStorage.py
--rw-rw-r--   0 oem      (29999) oem      (29999)     9497 2024-03-24 11:58:47.000000 temod-2.0.8/src/temod/storage/mysql/mysqlJoinStorage.py
--rw-rw-r--   0 oem      (29999) oem      (29999)     2148 2024-03-24 12:33:38.000000 temod-2.0.8/src/temod/storage/mysql/mysqlStorage.py
-drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-03-24 12:39:44.223231 temod-2.0.8/src/temod/utils/
--rw-rw-r--   0 oem      (29999) oem      (29999)     2073 2023-07-15 13:43:23.000000 temod-2.0.8/src/temod/utils/decorators.py
--rw-rw-r--   0 oem      (29999) oem      (29999)     2373 2023-07-15 13:43:23.000000 temod-2.0.8/src/temod/utils/exoskeleton.py
--rw-rw-r--   0 oem      (29999) oem      (29999)      547 2023-07-15 13:43:24.000000 temod-2.0.8/src/temod/utils/graphs.py
-drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-03-24 12:39:44.223231 temod-2.0.8/src/temod.egg-info/
--rw-r--r--   0 oem      (29999) oem      (29999)      703 2024-03-24 12:39:44.000000 temod-2.0.8/src/temod.egg-info/PKG-INFO
--rw-rw-r--   0 oem      (29999) oem      (29999)     1329 2024-03-24 12:39:44.000000 temod-2.0.8/src/temod.egg-info/SOURCES.txt
--rw-rw-r--   0 oem      (29999) oem      (29999)        1 2024-03-24 12:39:44.000000 temod-2.0.8/src/temod.egg-info/dependency_links.txt
--rw-rw-r--   0 oem      (29999) oem      (29999)       49 2024-03-24 12:39:44.000000 temod-2.0.8/src/temod.egg-info/requires.txt
--rw-rw-r--   0 oem      (29999) oem      (29999)        6 2024-03-24 12:39:44.000000 temod-2.0.8/src/temod.egg-info/top_level.txt
+drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-04-02 10:06:42.456259 temod-2.0.9/
+-rw-rw-r--   0 oem      (29999) oem      (29999)     1069 2023-07-16 09:53:35.000000 temod-2.0.9/LICENSE.txt
+-rw-r--r--   0 oem      (29999) oem      (29999)      703 2024-04-02 10:06:42.456259 temod-2.0.9/PKG-INFO
+-rw-rw-r--   0 oem      (29999) oem      (29999)       67 2023-07-16 09:51:01.000000 temod-2.0.9/README.md
+-rw-rw-r--   0 oem      (29999) oem      (29999)      704 2024-04-02 10:06:23.000000 temod-2.0.9/pyproject.toml
+-rw-rw-r--   0 oem      (29999) oem      (29999)       38 2024-04-02 10:06:42.456259 temod-2.0.9/setup.cfg
+drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-04-02 10:06:42.452259 temod-2.0.9/src/
+drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-04-02 10:06:42.452259 temod-2.0.9/src/temod/
+-rw-rw-r--   0 oem      (29999) oem      (29999)       27 2023-07-15 13:43:54.000000 temod-2.0.9/src/temod/__init__.py
+drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-04-02 10:06:42.452259 temod-2.0.9/src/temod/base/
+-rw-rw-r--   0 oem      (29999) oem      (29999)      145 2023-07-15 13:44:09.000000 temod-2.0.9/src/temod/base/__init__.py
+-rw-rw-r--   0 oem      (29999) oem      (29999)     9973 2024-03-24 12:34:15.000000 temod-2.0.9/src/temod/base/attribute.py
+-rw-rw-r--   0 oem      (29999) oem      (29999)     1697 2023-07-15 13:44:06.000000 temod-2.0.9/src/temod/base/cluster.py
+-rw-rw-r--   0 oem      (29999) oem      (29999)     2900 2023-07-15 13:44:09.000000 temod-2.0.9/src/temod/base/condition.py
+-rw-rw-r--   0 oem      (29999) oem      (29999)     1986 2023-07-15 13:44:10.000000 temod-2.0.9/src/temod/base/constraint.py
+-rw-rw-r--   0 oem      (29999) oem      (29999)     6238 2023-07-15 13:44:09.000000 temod-2.0.9/src/temod/base/entity.py
+-rw-rw-r--   0 oem      (29999) oem      (29999)     1481 2023-07-15 13:44:09.000000 temod-2.0.9/src/temod/base/exceptions.py
+-rw-rw-r--   0 oem      (29999) oem      (29999)     2557 2023-07-15 13:44:10.000000 temod-2.0.9/src/temod/base/join.py
+drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-04-02 10:06:42.452259 temod-2.0.9/src/temod/ext/
+-rw-rw-r--   0 oem      (29999) oem      (29999)    11228 2023-07-15 13:43:55.000000 temod-2.0.9/src/temod/ext/holders.py
+drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-04-02 10:06:42.452259 temod-2.0.9/src/temod/operators/
+-rw-rw-r--   0 oem      (29999) oem      (29999)      451 2023-07-15 13:43:22.000000 temod-2.0.9/src/temod/operators/aggregation.py
+drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-04-02 10:06:42.452259 temod-2.0.9/src/temod/storage/
+-rw-rw-r--   0 oem      (29999) oem      (29999)      201 2023-07-15 13:43:59.000000 temod-2.0.9/src/temod/storage/__init__.py
+drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-04-02 10:06:42.452259 temod-2.0.9/src/temod/storage/directory/
+-rw-rw-r--   0 oem      (29999) oem      (29999)       59 2023-07-15 13:43:57.000000 temod-2.0.9/src/temod/storage/directory/__init__.py
+-rw-rw-r--   0 oem      (29999) oem      (29999)     5004 2023-07-15 13:43:57.000000 temod-2.0.9/src/temod/storage/directory/directoryStorage.py
+-rw-rw-r--   0 oem      (29999) oem      (29999)     2835 2023-07-15 13:43:55.000000 temod-2.0.9/src/temod/storage/directory/yamlStorage.py
+drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-04-02 10:06:42.456259 temod-2.0.9/src/temod/storage/exceptions/
+-rw-rw-r--   0 oem      (29999) oem      (29999)      774 2023-07-15 13:43:58.000000 temod-2.0.9/src/temod/storage/exceptions/entities.py
+-rw-rw-r--   0 oem      (29999) oem      (29999)      541 2023-07-15 13:43:58.000000 temod-2.0.9/src/temod/storage/exceptions/joins.py
+-rw-rw-r--   0 oem      (29999) oem      (29999)      418 2023-07-15 13:43:58.000000 temod-2.0.9/src/temod/storage/exceptions/translators.py
+drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-04-02 10:06:42.456259 temod-2.0.9/src/temod/storage/influxdb/
+-rw-rw-r--   0 oem      (29999) oem      (29999)     9803 2024-02-25 20:41:24.000000 temod-2.0.9/src/temod/storage/influxdb/influxEntityStorage.py
+-rw-rw-r--   0 oem      (29999) oem      (29999)     2363 2024-02-25 20:41:37.000000 temod-2.0.9/src/temod/storage/influxdb/influxStorage.py
+-rw-rw-r--   0 oem      (29999) oem      (29999)     6019 2023-07-15 13:43:59.000000 temod-2.0.9/src/temod/storage/influxdb/influxTranslators.py
+drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-04-02 10:06:42.456259 temod-2.0.9/src/temod/storage/mysql/
+-rw-rw-r--   0 oem      (29999) oem      (29999)      131 2023-07-15 13:44:05.000000 temod-2.0.9/src/temod/storage/mysql/__init__.py
+-rw-rw-r--   0 oem      (29999) oem      (29999)     2416 2023-07-15 13:44:01.000000 temod-2.0.9/src/temod/storage/mysql/mysqlAttributesTranslator.py
+-rw-rw-r--   0 oem      (29999) oem      (29999)     6604 2024-02-25 20:41:49.000000 temod-2.0.9/src/temod/storage/mysql/mysqlClusterStorage.py
+-rw-rw-r--   0 oem      (29999) oem      (29999)     4235 2023-07-15 13:44:05.000000 temod-2.0.9/src/temod/storage/mysql/mysqlConditionsTranslator.py
+-rw-rw-r--   0 oem      (29999) oem      (29999)     9775 2024-03-27 20:27:49.000000 temod-2.0.9/src/temod/storage/mysql/mysqlEntityStorage.py
+-rw-rw-r--   0 oem      (29999) oem      (29999)     9497 2024-03-24 11:58:47.000000 temod-2.0.9/src/temod/storage/mysql/mysqlJoinStorage.py
+-rw-rw-r--   0 oem      (29999) oem      (29999)     2148 2024-03-24 12:33:38.000000 temod-2.0.9/src/temod/storage/mysql/mysqlStorage.py
+drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-04-02 10:06:42.456259 temod-2.0.9/src/temod/utils/
+-rw-rw-r--   0 oem      (29999) oem      (29999)     2073 2023-07-15 13:43:23.000000 temod-2.0.9/src/temod/utils/decorators.py
+-rw-rw-r--   0 oem      (29999) oem      (29999)     2373 2023-07-15 13:43:23.000000 temod-2.0.9/src/temod/utils/exoskeleton.py
+-rw-rw-r--   0 oem      (29999) oem      (29999)      547 2023-07-15 13:43:24.000000 temod-2.0.9/src/temod/utils/graphs.py
+drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2024-04-02 10:06:42.456259 temod-2.0.9/src/temod.egg-info/
+-rw-r--r--   0 oem      (29999) oem      (29999)      703 2024-04-02 10:06:42.000000 temod-2.0.9/src/temod.egg-info/PKG-INFO
+-rw-rw-r--   0 oem      (29999) oem      (29999)     1329 2024-04-02 10:06:42.000000 temod-2.0.9/src/temod.egg-info/SOURCES.txt
+-rw-rw-r--   0 oem      (29999) oem      (29999)        1 2024-04-02 10:06:42.000000 temod-2.0.9/src/temod.egg-info/dependency_links.txt
+-rw-rw-r--   0 oem      (29999) oem      (29999)       49 2024-04-02 10:06:42.000000 temod-2.0.9/src/temod.egg-info/requires.txt
+-rw-rw-r--   0 oem      (29999) oem      (29999)        6 2024-04-02 10:06:42.000000 temod-2.0.9/src/temod.egg-info/top_level.txt
```

### Comparing `temod-2.0.8/LICENSE.txt` & `temod-2.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `temod-2.0.8/PKG-INFO` & `temod-2.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: temod
-Version: 2.0.8
+Version: 2.0.9
 Summary: Data management abstraction layer for your python programs
 Author-email: PyAxolotl <abdellatifzied.saada@gmail.com>
 Project-URL: Homepage, https://github.com/TuburboMajus/temod
 Project-URL: Bug Tracker, https://github.com/TuburboMajus/temod/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `temod-2.0.8/pyproject.toml` & `temod-2.0.9/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=42']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "temod"
-version = "2.0.8"
+version = "2.0.9"
 authors = [
   { name="PyAxolotl", email="abdellatifzied.saada@gmail.com" },
 ]
 description = "Data management abstraction layer for your python programs"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `temod-2.0.8/src/temod/base/attribute.py` & `temod-2.0.9/src/temod/base/attribute.py`

 * *Files identical despite different names*

### Comparing `temod-2.0.8/src/temod/base/cluster.py` & `temod-2.0.9/src/temod/base/cluster.py`

 * *Files identical despite different names*

### Comparing `temod-2.0.8/src/temod/base/condition.py` & `temod-2.0.9/src/temod/base/condition.py`

 * *Files identical despite different names*

### Comparing `temod-2.0.8/src/temod/base/constraint.py` & `temod-2.0.9/src/temod/base/constraint.py`

 * *Files identical despite different names*

### Comparing `temod-2.0.8/src/temod/base/entity.py` & `temod-2.0.9/src/temod/base/entity.py`

 * *Files identical despite different names*

### Comparing `temod-2.0.8/src/temod/base/exceptions.py` & `temod-2.0.9/src/temod/base/exceptions.py`

 * *Files identical despite different names*

### Comparing `temod-2.0.8/src/temod/base/join.py` & `temod-2.0.9/src/temod/base/join.py`

 * *Files identical despite different names*

### Comparing `temod-2.0.8/src/temod/ext/holders.py` & `temod-2.0.9/src/temod/ext/holders.py`

 * *Files identical despite different names*

### Comparing `temod-2.0.8/src/temod/storage/directory/directoryStorage.py` & `temod-2.0.9/src/temod/storage/directory/directoryStorage.py`

 * *Files identical despite different names*

### Comparing `temod-2.0.8/src/temod/storage/directory/yamlStorage.py` & `temod-2.0.9/src/temod/storage/directory/yamlStorage.py`

 * *Files identical despite different names*

### Comparing `temod-2.0.8/src/temod/storage/exceptions/entities.py` & `temod-2.0.9/src/temod/storage/exceptions/entities.py`

 * *Files identical despite different names*

### Comparing `temod-2.0.8/src/temod/storage/exceptions/joins.py` & `temod-2.0.9/src/temod/storage/exceptions/joins.py`

 * *Files identical despite different names*

### Comparing `temod-2.0.8/src/temod/storage/influxdb/influxEntityStorage.py` & `temod-2.0.9/src/temod/storage/influxdb/influxEntityStorage.py`

 * *Files identical despite different names*

### Comparing `temod-2.0.8/src/temod/storage/influxdb/influxStorage.py` & `temod-2.0.9/src/temod/storage/influxdb/influxStorage.py`

 * *Files identical despite different names*

### Comparing `temod-2.0.8/src/temod/storage/influxdb/influxTranslators.py` & `temod-2.0.9/src/temod/storage/influxdb/influxTranslators.py`

 * *Files identical despite different names*

### Comparing `temod-2.0.8/src/temod/storage/mysql/mysqlAttributesTranslator.py` & `temod-2.0.9/src/temod/storage/mysql/mysqlAttributesTranslator.py`

 * *Files identical despite different names*

### Comparing `temod-2.0.8/src/temod/storage/mysql/mysqlClusterStorage.py` & `temod-2.0.9/src/temod/storage/mysql/mysqlClusterStorage.py`

 * *Files identical despite different names*

### Comparing `temod-2.0.8/src/temod/storage/mysql/mysqlConditionsTranslator.py` & `temod-2.0.9/src/temod/storage/mysql/mysqlConditionsTranslator.py`

 * *Files identical despite different names*

### Comparing `temod-2.0.8/src/temod/storage/mysql/mysqlEntityStorage.py` & `temod-2.0.9/src/temod/storage/mysql/mysqlEntityStorage.py`

 * *Files 0% similar despite different names*

```diff
@@ -184,15 +184,15 @@
 			(attr,MysqlAttributesTranslator.translate(value)) 
 			for attr,value in entity.attributes.items() if not value.is_auto
 		]
 		query = f"INSERT INTO {self.entity_name} ({','.join([v[0] for v in values])}) VALUES ({','.join([v[1] for v in values])})"
 
 		return self.executeAndCommit(query).lastrowid
 
-	def update(self,*conditions,limit=None,skip=None,updateID=False,**kwargs):
+	def update(self,updates,*conditions,limit=None,skip=None,updateID=False,**kwargs):
 		condition = self._build_condition(*conditions,**kwargs)
 		try:
 			assert(updates is not None and len(updates) > 0)
 		except:
 			raise EntityStorageException("At least one attribute to update is necessary")
 		if type(updates) is dict:
 			updates = [
```

### Comparing `temod-2.0.8/src/temod/storage/mysql/mysqlJoinStorage.py` & `temod-2.0.9/src/temod/storage/mysql/mysqlJoinStorage.py`

 * *Files identical despite different names*

### Comparing `temod-2.0.8/src/temod/storage/mysql/mysqlStorage.py` & `temod-2.0.9/src/temod/storage/mysql/mysqlStorage.py`

 * *Files identical despite different names*

### Comparing `temod-2.0.8/src/temod/utils/decorators.py` & `temod-2.0.9/src/temod/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `temod-2.0.8/src/temod/utils/exoskeleton.py` & `temod-2.0.9/src/temod/utils/exoskeleton.py`

 * *Files identical despite different names*

### Comparing `temod-2.0.8/src/temod/utils/graphs.py` & `temod-2.0.9/src/temod/utils/graphs.py`

 * *Files identical despite different names*

### Comparing `temod-2.0.8/src/temod.egg-info/PKG-INFO` & `temod-2.0.9/src/temod.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: temod
-Version: 2.0.8
+Version: 2.0.9
 Summary: Data management abstraction layer for your python programs
 Author-email: PyAxolotl <abdellatifzied.saada@gmail.com>
 Project-URL: Homepage, https://github.com/TuburboMajus/temod
 Project-URL: Bug Tracker, https://github.com/TuburboMajus/temod/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `temod-2.0.8/src/temod.egg-info/SOURCES.txt` & `temod-2.0.9/src/temod.egg-info/SOURCES.txt`

 * *Files identical despite different names*

