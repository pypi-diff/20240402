# Comparing `tmp/radosdb-0.1.2.tar.gz` & `tmp/radosdb-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radosdb-0.1.2.tar", last modified: Tue Apr  2 06:56:46 2024, max compression
+gzip compressed data, was "radosdb-0.1.3.tar", last modified: Tue Apr  2 07:14:23 2024, max compression
```

## Comparing `radosdb-0.1.2.tar` & `radosdb-0.1.3.tar`

### file list

```diff
@@ -1,47 +1,46 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 06:56:46.126452 radosdb-0.1.2/
--rw-r--r--   0 root         (0) root         (0)      250 2024-04-02 06:56:46.126452 radosdb-0.1.2/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 06:56:46.122452 radosdb-0.1.2/common/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-21 11:26:44.000000 radosdb-0.1.2/common/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 06:56:46.122452 radosdb-0.1.2/common/helper/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-21 11:26:44.000000 radosdb-0.1.2/common/helper/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2533 2024-02-21 12:49:18.000000 radosdb-0.1.2/common/helper/env.py
--rw-r--r--   0 root         (0) root         (0)      669 2024-02-21 11:26:44.000000 radosdb-0.1.2/common/helper/redis_helper.py
--rw-r--r--   0 root         (0) root         (0)     6511 2024-02-21 11:26:44.000000 radosdb-0.1.2/common/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 06:56:46.122452 radosdb-0.1.2/config/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-21 11:26:44.000000 radosdb-0.1.2/config/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1389 2024-02-21 12:49:18.000000 radosdb-0.1.2/config/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 06:56:46.122452 radosdb-0.1.2/model/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-21 07:16:18.000000 radosdb-0.1.2/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)        2 2024-02-21 07:16:18.000000 radosdb-0.1.2/model/data.py
--rw-r--r--   0 root         (0) root         (0)     4393 2024-03-13 03:49:24.000000 radosdb-0.1.2/model/time_conversion.py
--rw-r--r--   0 root         (0) root         (0)      903 2024-02-27 05:25:28.000000 radosdb-0.1.2/model/trade_day.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 06:56:46.122452 radosdb-0.1.2/mongoapi/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-21 07:16:18.000000 radosdb-0.1.2/mongoapi/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4314 2024-03-10 11:29:25.000000 radosdb-0.1.2/mongoapi/mongo_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 06:56:46.122452 radosdb-0.1.2/radosdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)      250 2024-04-02 06:56:46.000000 radosdb-0.1.2/radosdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      831 2024-04-02 06:56:46.000000 radosdb-0.1.2/radosdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-02 06:56:46.000000 radosdb-0.1.2/radosdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2024-04-02 06:56:46.000000 radosdb-0.1.2/radosdb.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       26 2024-04-02 06:56:46.000000 radosdb-0.1.2/radosdb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       48 2024-04-02 06:56:46.000000 radosdb-0.1.2/radosdb.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 06:56:46.122452 radosdb-0.1.2/repo/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-21 07:16:18.000000 radosdb-0.1.2/repo/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2331 2024-03-29 03:10:04.000000 radosdb-0.1.2/repo/mongo_data_meta_repo.py
--rw-r--r--   0 root         (0) root         (0)     3579 2024-03-13 03:49:24.000000 radosdb-0.1.2/repo/mongo_trade_day_repo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 06:56:46.126452 radosdb-0.1.2/service/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-21 07:16:18.000000 radosdb-0.1.2/service/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1264 2024-03-29 03:10:13.000000 radosdb-0.1.2/service/data_meta_service.py
--rw-r--r--   0 root         (0) root         (0)      811 2024-02-27 05:25:28.000000 radosdb-0.1.2/service/trade_day_service.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-02 06:56:46.126452 radosdb-0.1.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      479 2024-04-02 06:56:40.000000 radosdb-0.1.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 06:56:46.126452 radosdb-0.1.2/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-21 07:16:18.000000 radosdb-0.1.2/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 06:56:46.126452 radosdb-0.1.2/tests/repo/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-21 07:16:18.000000 radosdb-0.1.2/tests/repo/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1823 2024-03-24 02:07:49.000000 radosdb-0.1.2/tests/repo/test_database.py
--rw-r--r--   0 root         (0) root         (0)     1058 2024-02-21 07:16:18.000000 radosdb-0.1.2/tests/repo/test_mongo_data_meta_repo.py
--rw-r--r--   0 root         (0) root         (0)     1266 2024-02-27 05:25:28.000000 radosdb-0.1.2/tests/repo/test_mongo_trade_day_repo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 06:56:46.126452 radosdb-0.1.2/tests/service/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-27 05:25:28.000000 radosdb-0.1.2/tests/service/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1272 2024-02-27 05:25:28.000000 radosdb-0.1.2/tests/service/test_trade_day_service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 07:14:23.742892 radosdb-0.1.3/
+-rw-r--r--   0 root         (0) root         (0)      250 2024-04-02 07:14:23.742892 radosdb-0.1.3/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 07:14:23.742892 radosdb-0.1.3/common/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-02-21 11:26:44.000000 radosdb-0.1.3/common/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 07:14:23.742892 radosdb-0.1.3/common/helper/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-02-21 11:26:44.000000 radosdb-0.1.3/common/helper/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2533 2024-02-21 12:49:18.000000 radosdb-0.1.3/common/helper/env.py
+-rw-r--r--   0 root         (0) root         (0)      669 2024-02-21 11:26:44.000000 radosdb-0.1.3/common/helper/redis_helper.py
+-rw-r--r--   0 root         (0) root         (0)     6511 2024-02-21 11:26:44.000000 radosdb-0.1.3/common/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 07:14:23.742892 radosdb-0.1.3/config/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-02-21 11:26:44.000000 radosdb-0.1.3/config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1389 2024-02-21 12:49:18.000000 radosdb-0.1.3/config/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 07:14:23.742892 radosdb-0.1.3/model/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-02-21 07:16:18.000000 radosdb-0.1.3/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        2 2024-02-21 07:16:18.000000 radosdb-0.1.3/model/data.py
+-rw-r--r--   0 root         (0) root         (0)     4393 2024-03-13 03:49:24.000000 radosdb-0.1.3/model/time_conversion.py
+-rw-r--r--   0 root         (0) root         (0)      903 2024-02-27 05:25:28.000000 radosdb-0.1.3/model/trade_day.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 07:14:23.742892 radosdb-0.1.3/mongoapi/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-02-21 07:16:18.000000 radosdb-0.1.3/mongoapi/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4314 2024-03-10 11:29:25.000000 radosdb-0.1.3/mongoapi/mongo_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 07:14:23.742892 radosdb-0.1.3/radosdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      250 2024-04-02 07:14:23.000000 radosdb-0.1.3/radosdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      797 2024-04-02 07:14:23.000000 radosdb-0.1.3/radosdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-02 07:14:23.000000 radosdb-0.1.3/radosdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2024-04-02 07:14:23.000000 radosdb-0.1.3/radosdb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2024-04-02 07:14:23.000000 radosdb-0.1.3/radosdb.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 07:14:23.742892 radosdb-0.1.3/repo/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-02-21 07:16:18.000000 radosdb-0.1.3/repo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2331 2024-03-29 03:10:04.000000 radosdb-0.1.3/repo/mongo_data_meta_repo.py
+-rw-r--r--   0 root         (0) root         (0)     3579 2024-03-13 03:49:24.000000 radosdb-0.1.3/repo/mongo_trade_day_repo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 07:14:23.742892 radosdb-0.1.3/service/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-02-21 07:16:18.000000 radosdb-0.1.3/service/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1264 2024-03-29 03:10:13.000000 radosdb-0.1.3/service/data_meta_service.py
+-rw-r--r--   0 root         (0) root         (0)      811 2024-02-27 05:25:28.000000 radosdb-0.1.3/service/trade_day_service.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-02 07:14:23.742892 radosdb-0.1.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      356 2024-04-02 07:07:18.000000 radosdb-0.1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 07:14:23.742892 radosdb-0.1.3/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-02-21 07:16:18.000000 radosdb-0.1.3/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 07:14:23.742892 radosdb-0.1.3/tests/repo/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-02-21 07:16:18.000000 radosdb-0.1.3/tests/repo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1823 2024-03-24 02:07:49.000000 radosdb-0.1.3/tests/repo/test_database.py
+-rw-r--r--   0 root         (0) root         (0)     1058 2024-02-21 07:16:18.000000 radosdb-0.1.3/tests/repo/test_mongo_data_meta_repo.py
+-rw-r--r--   0 root         (0) root         (0)     1266 2024-02-27 05:25:28.000000 radosdb-0.1.3/tests/repo/test_mongo_trade_day_repo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 07:14:23.742892 radosdb-0.1.3/tests/service/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-02-27 05:25:28.000000 radosdb-0.1.3/tests/service/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1272 2024-02-27 05:25:28.000000 radosdb-0.1.3/tests/service/test_trade_day_service.py
```

### Comparing `radosdb-0.1.2/common/helper/env.py` & `radosdb-0.1.3/common/helper/env.py`

 * *Files identical despite different names*

### Comparing `radosdb-0.1.2/common/helper/redis_helper.py` & `radosdb-0.1.3/common/helper/redis_helper.py`

 * *Files identical despite different names*

### Comparing `radosdb-0.1.2/common/tools.py` & `radosdb-0.1.3/common/tools.py`

 * *Files identical despite different names*

### Comparing `radosdb-0.1.2/config/config.py` & `radosdb-0.1.3/config/config.py`

 * *Files identical despite different names*

### Comparing `radosdb-0.1.2/model/time_conversion.py` & `radosdb-0.1.3/model/time_conversion.py`

 * *Files identical despite different names*

### Comparing `radosdb-0.1.2/model/trade_day.py` & `radosdb-0.1.3/model/trade_day.py`

 * *Files identical despite different names*

### Comparing `radosdb-0.1.2/mongoapi/mongo_api.py` & `radosdb-0.1.3/mongoapi/mongo_api.py`

 * *Files identical despite different names*

### Comparing `radosdb-0.1.2/radosdb.egg-info/SOURCES.txt` & `radosdb-0.1.3/radosdb.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 model/time_conversion.py
 model/trade_day.py
 mongoapi/__init__.py
 mongoapi/mongo_api.py
 radosdb.egg-info/PKG-INFO
 radosdb.egg-info/SOURCES.txt
 radosdb.egg-info/dependency_links.txt
-radosdb.egg-info/entry_points.txt
 radosdb.egg-info/requires.txt
 radosdb.egg-info/top_level.txt
 repo/__init__.py
 repo/mongo_data_meta_repo.py
 repo/mongo_trade_day_repo.py
 service/__init__.py
 service/data_meta_service.py
```

### Comparing `radosdb-0.1.2/repo/mongo_data_meta_repo.py` & `radosdb-0.1.3/repo/mongo_data_meta_repo.py`

 * *Files identical despite different names*

### Comparing `radosdb-0.1.2/repo/mongo_trade_day_repo.py` & `radosdb-0.1.3/repo/mongo_trade_day_repo.py`

 * *Files identical despite different names*

### Comparing `radosdb-0.1.2/service/data_meta_service.py` & `radosdb-0.1.3/service/data_meta_service.py`

 * *Files identical despite different names*

### Comparing `radosdb-0.1.2/service/trade_day_service.py` & `radosdb-0.1.3/service/trade_day_service.py`

 * *Files identical despite different names*

### Comparing `radosdb-0.1.2/tests/repo/test_database.py` & `radosdb-0.1.3/tests/repo/test_database.py`

 * *Files identical despite different names*

### Comparing `radosdb-0.1.2/tests/repo/test_mongo_data_meta_repo.py` & `radosdb-0.1.3/tests/repo/test_mongo_data_meta_repo.py`

 * *Files identical despite different names*

### Comparing `radosdb-0.1.2/tests/repo/test_mongo_trade_day_repo.py` & `radosdb-0.1.3/tests/repo/test_mongo_trade_day_repo.py`

 * *Files identical despite different names*

### Comparing `radosdb-0.1.2/tests/service/test_trade_day_service.py` & `radosdb-0.1.3/tests/service/test_trade_day_service.py`

 * *Files identical despite different names*

