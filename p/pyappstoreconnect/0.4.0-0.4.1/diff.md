# Comparing `tmp/pyappstoreconnect-0.4.0.tar.gz` & `tmp/pyappstoreconnect-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyappstoreconnect-0.4.0.tar", last modified: Mon Feb 19 15:17:34 2024, max compression
+gzip compressed data, was "pyappstoreconnect-0.4.1.tar", last modified: Tue Apr  2 14:26:00 2024, max compression
```

## Comparing `pyappstoreconnect-0.4.0.tar` & `pyappstoreconnect-0.4.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 15:17:34.544029 pyappstoreconnect-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-02-19 15:17:24.000000 pyappstoreconnect-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-02-19 15:17:34.544029 pyappstoreconnect-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-02-19 15:17:24.000000 pyappstoreconnect-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 15:17:34.544029 pyappstoreconnect-0.4.0/pyappstoreconnect/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-19 15:17:24.000000 pyappstoreconnect-0.4.0/pyappstoreconnect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7976 2024-02-19 15:17:24.000000 pyappstoreconnect-0.4.0/pyappstoreconnect/appAnalytics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-02-19 15:17:24.000000 pyappstoreconnect-0.4.0/pyappstoreconnect/benchmarks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10747 2024-02-19 15:17:24.000000 pyappstoreconnect-0.4.0/pyappstoreconnect/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-02-19 15:17:24.000000 pyappstoreconnect-0.4.0/pyappstoreconnect/metricsWithFilter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-02-19 15:17:24.000000 pyappstoreconnect-0.4.0/pyappstoreconnect/metricsWithGroup.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-02-19 15:17:24.000000 pyappstoreconnect-0.4.0/pyappstoreconnect/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-02-19 15:17:24.000000 pyappstoreconnect-0.4.0/pyappstoreconnect/timeSeriesAnalytics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 15:17:34.544029 pyappstoreconnect-0.4.0/pyappstoreconnect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-02-19 15:17:34.000000 pyappstoreconnect-0.4.0/pyappstoreconnect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-02-19 15:17:34.000000 pyappstoreconnect-0.4.0/pyappstoreconnect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 15:17:34.000000 pyappstoreconnect-0.4.0/pyappstoreconnect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-19 15:17:34.000000 pyappstoreconnect-0.4.0/pyappstoreconnect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-02-19 15:17:28.000000 pyappstoreconnect-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-19 15:17:34.544029 pyappstoreconnect-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:26:00.027627 pyappstoreconnect-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-02 14:25:49.000000 pyappstoreconnect-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-02 14:26:00.027627 pyappstoreconnect-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-02 14:25:49.000000 pyappstoreconnect-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:26:00.027627 pyappstoreconnect-0.4.1/pyappstoreconnect/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-02 14:25:49.000000 pyappstoreconnect-0.4.1/pyappstoreconnect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7976 2024-04-02 14:25:49.000000 pyappstoreconnect-0.4.1/pyappstoreconnect/appAnalytics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-04-02 14:25:49.000000 pyappstoreconnect-0.4.1/pyappstoreconnect/benchmarks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10747 2024-04-02 14:25:49.000000 pyappstoreconnect-0.4.1/pyappstoreconnect/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-04-02 14:25:49.000000 pyappstoreconnect-0.4.1/pyappstoreconnect/metricsWithFilter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-04-02 14:25:49.000000 pyappstoreconnect-0.4.1/pyappstoreconnect/metricsWithGroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-02 14:25:49.000000 pyappstoreconnect-0.4.1/pyappstoreconnect/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-04-02 14:25:49.000000 pyappstoreconnect-0.4.1/pyappstoreconnect/timeSeriesAnalytics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:26:00.027627 pyappstoreconnect-0.4.1/pyappstoreconnect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-02 14:26:00.000000 pyappstoreconnect-0.4.1/pyappstoreconnect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-02 14:26:00.000000 pyappstoreconnect-0.4.1/pyappstoreconnect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 14:26:00.000000 pyappstoreconnect-0.4.1/pyappstoreconnect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-02 14:26:00.000000 pyappstoreconnect-0.4.1/pyappstoreconnect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-02 14:25:55.000000 pyappstoreconnect-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 14:26:00.027627 pyappstoreconnect-0.4.1/setup.cfg
```

### Comparing `pyappstoreconnect-0.4.0/LICENSE` & `pyappstoreconnect-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyappstoreconnect-0.4.0/PKG-INFO` & `pyappstoreconnect-0.4.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyappstoreconnect
-Version: 0.4.0
+Version: 0.4.1
 Author-email: Grigory Efimov <grigory.efimov@gmail.com>
 Maintainer-email: Grigory Efimov <grigory.efimov@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Grigory Efimov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -33,7 +33,10 @@
 
 # pyappstoreconnect
 wrapper for https://appstoreconnect.apple.com/
 > :warning: **is not for official api**
 this wrapper for NOT offical internal api functions  
 based on https://github.com/fastlane/fastlane/tree/master/spaceship
 
+## 2fa
+session saved in cache file and valid one month
+
```

### Comparing `pyappstoreconnect-0.4.0/pyappstoreconnect/appAnalytics.py` & `pyappstoreconnect-0.4.1/pyappstoreconnect/appAnalytics.py`

 * *Files identical despite different names*

### Comparing `pyappstoreconnect-0.4.0/pyappstoreconnect/benchmarks.py` & `pyappstoreconnect-0.4.1/pyappstoreconnect/benchmarks.py`

 * *Files identical despite different names*

### Comparing `pyappstoreconnect-0.4.0/pyappstoreconnect/client.py` & `pyappstoreconnect-0.4.1/pyappstoreconnect/client.py`

 * *Files identical despite different names*

### Comparing `pyappstoreconnect-0.4.0/pyappstoreconnect/metricsWithFilter.py` & `pyappstoreconnect-0.4.1/pyappstoreconnect/metricsWithFilter.py`

 * *Files identical despite different names*

### Comparing `pyappstoreconnect-0.4.0/pyappstoreconnect/metricsWithGroup.py` & `pyappstoreconnect-0.4.1/pyappstoreconnect/metricsWithGroup.py`

 * *Files identical despite different names*

### Comparing `pyappstoreconnect-0.4.0/pyappstoreconnect/settings.py` & `pyappstoreconnect-0.4.1/pyappstoreconnect/settings.py`

 * *Files 19% similar despite different names*

```diff
@@ -15,11 +15,11 @@
             self.logger.error(f"{defName}: status_code = {response.status_code}, response.text={response.text}")
             return False
 
         # check json data
         try:
             data = response.json()
         except Exception as e:
-            self.logger.error(f"{defName}: failed get response.json(), error={str(e)}")
+            self.logger.error(f"{defName}: failed get response.json(), error={str(e)}, response.text={response.text}")
             return None
 
         return data
```

### Comparing `pyappstoreconnect-0.4.0/pyappstoreconnect/timeSeriesAnalytics.py` & `pyappstoreconnect-0.4.1/pyappstoreconnect/timeSeriesAnalytics.py`

 * *Files identical despite different names*

### Comparing `pyappstoreconnect-0.4.0/pyappstoreconnect.egg-info/PKG-INFO` & `pyappstoreconnect-0.4.1/pyappstoreconnect.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyappstoreconnect
-Version: 0.4.0
+Version: 0.4.1
 Author-email: Grigory Efimov <grigory.efimov@gmail.com>
 Maintainer-email: Grigory Efimov <grigory.efimov@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Grigory Efimov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -33,7 +33,10 @@
 
 # pyappstoreconnect
 wrapper for https://appstoreconnect.apple.com/
 > :warning: **is not for official api**
 this wrapper for NOT offical internal api functions  
 based on https://github.com/fastlane/fastlane/tree/master/spaceship
 
+## 2fa
+session saved in cache file and valid one month
+
```

