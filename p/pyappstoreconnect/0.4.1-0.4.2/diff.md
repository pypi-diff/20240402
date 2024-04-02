# Comparing `tmp/pyappstoreconnect-0.4.1.tar.gz` & `tmp/pyappstoreconnect-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyappstoreconnect-0.4.1.tar", last modified: Tue Apr  2 14:26:00 2024, max compression
+gzip compressed data, was "pyappstoreconnect-0.4.2.tar", last modified: Tue Apr  2 19:19:11 2024, max compression
```

## Comparing `pyappstoreconnect-0.4.1.tar` & `pyappstoreconnect-0.4.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:26:00.027627 pyappstoreconnect-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-02 14:25:49.000000 pyappstoreconnect-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-02 14:26:00.027627 pyappstoreconnect-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-02 14:25:49.000000 pyappstoreconnect-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:26:00.027627 pyappstoreconnect-0.4.1/pyappstoreconnect/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-02 14:25:49.000000 pyappstoreconnect-0.4.1/pyappstoreconnect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7976 2024-04-02 14:25:49.000000 pyappstoreconnect-0.4.1/pyappstoreconnect/appAnalytics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-04-02 14:25:49.000000 pyappstoreconnect-0.4.1/pyappstoreconnect/benchmarks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10747 2024-04-02 14:25:49.000000 pyappstoreconnect-0.4.1/pyappstoreconnect/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-04-02 14:25:49.000000 pyappstoreconnect-0.4.1/pyappstoreconnect/metricsWithFilter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-04-02 14:25:49.000000 pyappstoreconnect-0.4.1/pyappstoreconnect/metricsWithGroup.py
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-02 14:25:49.000000 pyappstoreconnect-0.4.1/pyappstoreconnect/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-04-02 14:25:49.000000 pyappstoreconnect-0.4.1/pyappstoreconnect/timeSeriesAnalytics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:26:00.027627 pyappstoreconnect-0.4.1/pyappstoreconnect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-02 14:26:00.000000 pyappstoreconnect-0.4.1/pyappstoreconnect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-02 14:26:00.000000 pyappstoreconnect-0.4.1/pyappstoreconnect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 14:26:00.000000 pyappstoreconnect-0.4.1/pyappstoreconnect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-02 14:26:00.000000 pyappstoreconnect-0.4.1/pyappstoreconnect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-02 14:25:55.000000 pyappstoreconnect-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 14:26:00.027627 pyappstoreconnect-0.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:19:11.641938 pyappstoreconnect-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-02 19:19:03.000000 pyappstoreconnect-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-02 19:19:11.641938 pyappstoreconnect-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-02 19:19:03.000000 pyappstoreconnect-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:19:11.637938 pyappstoreconnect-0.4.2/pyappstoreconnect/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-02 19:19:03.000000 pyappstoreconnect-0.4.2/pyappstoreconnect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7976 2024-04-02 19:19:03.000000 pyappstoreconnect-0.4.2/pyappstoreconnect/appAnalytics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-04-02 19:19:03.000000 pyappstoreconnect-0.4.2/pyappstoreconnect/benchmarks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11079 2024-04-02 19:19:03.000000 pyappstoreconnect-0.4.2/pyappstoreconnect/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-04-02 19:19:03.000000 pyappstoreconnect-0.4.2/pyappstoreconnect/metricsWithFilter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-04-02 19:19:03.000000 pyappstoreconnect-0.4.2/pyappstoreconnect/metricsWithGroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-02 19:19:03.000000 pyappstoreconnect-0.4.2/pyappstoreconnect/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-02 19:19:03.000000 pyappstoreconnect-0.4.2/pyappstoreconnect/timeSeriesAnalytics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:19:11.637938 pyappstoreconnect-0.4.2/pyappstoreconnect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-02 19:19:11.000000 pyappstoreconnect-0.4.2/pyappstoreconnect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-02 19:19:11.000000 pyappstoreconnect-0.4.2/pyappstoreconnect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 19:19:11.000000 pyappstoreconnect-0.4.2/pyappstoreconnect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-02 19:19:11.000000 pyappstoreconnect-0.4.2/pyappstoreconnect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-02 19:19:08.000000 pyappstoreconnect-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 19:19:11.641938 pyappstoreconnect-0.4.2/setup.cfg
```

### Comparing `pyappstoreconnect-0.4.1/LICENSE` & `pyappstoreconnect-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyappstoreconnect-0.4.1/PKG-INFO` & `pyappstoreconnect-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyappstoreconnect
-Version: 0.4.1
+Version: 0.4.2
 Author-email: Grigory Efimov <grigory.efimov@gmail.com>
 Maintainer-email: Grigory Efimov <grigory.efimov@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Grigory Efimov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyappstoreconnect-0.4.1/pyappstoreconnect/appAnalytics.py` & `pyappstoreconnect-0.4.2/pyappstoreconnect/appAnalytics.py`

 * *Files identical despite different names*

### Comparing `pyappstoreconnect-0.4.1/pyappstoreconnect/benchmarks.py` & `pyappstoreconnect-0.4.2/pyappstoreconnect/benchmarks.py`

 * *Files identical despite different names*

### Comparing `pyappstoreconnect-0.4.1/pyappstoreconnect/client.py` & `pyappstoreconnect-0.4.2/pyappstoreconnect/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,15 +45,15 @@
             "backoff_factor": 30, # {backoff factor} * (2 ** ({number of previous retries}))
             "status_forcelist": [429, 500, 502, 503, 504], # HTTP status codes to retry on
             "allowed_methods": ['HEAD', 'TRACE', 'GET', 'PUT', 'OPTIONS', 'POST'],
         },
         logLevel=None,
         userAgent=None,
     ):
-        self.logger = logging.getLogger(self.__class__.__name__)
+        self.logger = logging.getLogger(__name__)
         if logLevel:
             if re.match(r"^(warn|warning)$", logLevel, re.IGNORECASE):
                 self.logger.setLevel(logging.WARNING)
             elif re.match(r"^debug$", logLevel, re.IGNORECASE):
                 self.logger.setLevel(logging.DEBUG)
             else:
                 self.logger.setLevel(logging.INFO)
@@ -261,24 +261,29 @@
         payload = {
             "accountName": username,
             "password": password,
             "rememberMe": True
         }
 
         response = self.session.post(url, json=payload, headers=headers)
+        self.logger.debug(f"{defName}: url={url}, response.status_code={response.status_code}")
         try:
             data = response.json()
         except Exception as e:
             self.logger.error(f"{defName}: failed get response.json(), error={str(e)}")
             return None
 
         if response.status_code == 409:
             # 2fa
-            self.logger.debug(f"response.status_code={response.status_code}, go to 2fa auth")
+            self.logger.debug(f"{defName}: response.status_code={response.status_code}, go to 2fa auth")
             self.handleTwoStepOrFactor(response)
+        elif response.status_code != 200:
+            message = f"url={url}, bad response.status_code={response.status_code}, should be 200 or 409"
+            self.logger.error(f"{defName}: {message}")
+            raise Exception(message)
 
         # get api settings
         self.apiSettingsAll = self.getSettingsAll()
 
         return response
 
     def timeInterval(self, days):
```

### Comparing `pyappstoreconnect-0.4.1/pyappstoreconnect/metricsWithFilter.py` & `pyappstoreconnect-0.4.2/pyappstoreconnect/metricsWithFilter.py`

 * *Files identical despite different names*

### Comparing `pyappstoreconnect-0.4.1/pyappstoreconnect/metricsWithGroup.py` & `pyappstoreconnect-0.4.2/pyappstoreconnect/metricsWithGroup.py`

 * *Files identical despite different names*

### Comparing `pyappstoreconnect-0.4.1/pyappstoreconnect/settings.py` & `pyappstoreconnect-0.4.2/pyappstoreconnect/settings.py`

 * *Files identical despite different names*

### Comparing `pyappstoreconnect-0.4.1/pyappstoreconnect/timeSeriesAnalytics.py` & `pyappstoreconnect-0.4.2/pyappstoreconnect/timeSeriesAnalytics.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,28 +23,28 @@
         }
         if group != None:
             payload['group'] = group
         headers = {
             "X-Requested-By": "appstoreconnect.apple.com",
         }
         url=f"https://appstoreconnect.apple.com/analytics/api/{apiVersion}/data/time-series"
-        self.logger.debug(f"payload={json.dumps(payload)}")
+        self.logger.debug(f"{defName}: payload={json.dumps(payload)}")
         response = self.session.post(url, json=payload, headers=headers)
 
         # check status_code
         if response.status_code != 200:
-            self.logger.error(f"{defName}: status_code = {response.status_code}, payload={payload}, response.text={response.text}")
+            self.logger.error(f"{defName}: status_code={response.status_code}, payload={payload}, response.text={response.text}")
             return False
 
         # check json data
         try:
             data = response.json()
         except Exception as e:
             self.logger.error(f"{defName}: failed get response.json(), error={str(e)}")
             return None
 
         # check results
         if 'results' not in data:
-            self.logger.error(f"{defName}: 'results' not found in response.json() = {data}")
+            self.logger.error(f"{defName}: 'results' not found in response.json()={data}")
             return False
 
         return data
```

### Comparing `pyappstoreconnect-0.4.1/pyappstoreconnect.egg-info/PKG-INFO` & `pyappstoreconnect-0.4.2/pyappstoreconnect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyappstoreconnect
-Version: 0.4.1
+Version: 0.4.2
 Author-email: Grigory Efimov <grigory.efimov@gmail.com>
 Maintainer-email: Grigory Efimov <grigory.efimov@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Grigory Efimov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

