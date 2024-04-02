# Comparing `tmp/deribit_wrapper-0.1.4.tar.gz` & `tmp/deribit_wrapper-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deribit_wrapper-0.1.4.tar", last modified: Mon Apr  1 22:07:03 2024, max compression
+gzip compressed data, was "deribit_wrapper-0.2.0.tar", last modified: Tue Apr  2 14:10:52 2024, max compression
```

## Comparing `deribit_wrapper-0.1.4.tar` & `deribit_wrapper-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:07:03.751854 deribit_wrapper-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-01 22:06:52.000000 deribit_wrapper-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-04-01 22:07:03.751854 deribit_wrapper-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-04-01 22:06:52.000000 deribit_wrapper-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:07:03.751854 deribit_wrapper-0.1.4/deribit_wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-01 22:06:52.000000 deribit_wrapper-0.1.4/deribit_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-04-01 22:06:52.000000 deribit_wrapper-0.1.4/deribit_wrapper/account_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-04-01 22:06:52.000000 deribit_wrapper-0.1.4/deribit_wrapper/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-01 22:06:52.000000 deribit_wrapper-0.1.4/deribit_wrapper/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-01 22:06:52.000000 deribit_wrapper-0.1.4/deribit_wrapper/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    11801 2024-04-01 22:06:52.000000 deribit_wrapper-0.1.4/deribit_wrapper/market_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     6191 2024-04-01 22:06:52.000000 deribit_wrapper-0.1.4/deribit_wrapper/trading.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-01 22:06:52.000000 deribit_wrapper-0.1.4/deribit_wrapper/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:07:03.751854 deribit_wrapper-0.1.4/deribit_wrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-04-01 22:07:03.000000 deribit_wrapper-0.1.4/deribit_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-01 22:07:03.000000 deribit_wrapper-0.1.4/deribit_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 22:07:03.000000 deribit_wrapper-0.1.4/deribit_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-01 22:07:03.000000 deribit_wrapper-0.1.4/deribit_wrapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-01 22:07:03.000000 deribit_wrapper-0.1.4/deribit_wrapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 22:07:03.751854 deribit_wrapper-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-01 22:06:52.000000 deribit_wrapper-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:10:52.334598 deribit_wrapper-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-02 14:10:42.000000 deribit_wrapper-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-04-02 14:10:52.334598 deribit_wrapper-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-04-02 14:10:42.000000 deribit_wrapper-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:10:52.334598 deribit_wrapper-0.2.0/deribit_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-02 14:10:42.000000 deribit_wrapper-0.2.0/deribit_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-04-02 14:10:42.000000 deribit_wrapper-0.2.0/deribit_wrapper/account_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-04-02 14:10:42.000000 deribit_wrapper-0.2.0/deribit_wrapper/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-02 14:10:42.000000 deribit_wrapper-0.2.0/deribit_wrapper/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-02 14:10:42.000000 deribit_wrapper-0.2.0/deribit_wrapper/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-02 14:10:42.000000 deribit_wrapper-0.2.0/deribit_wrapper/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11801 2024-04-02 14:10:42.000000 deribit_wrapper-0.2.0/deribit_wrapper/market_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7854 2024-04-02 14:10:42.000000 deribit_wrapper-0.2.0/deribit_wrapper/trading.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-02 14:10:42.000000 deribit_wrapper-0.2.0/deribit_wrapper/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:10:52.334598 deribit_wrapper-0.2.0/deribit_wrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-04-02 14:10:52.000000 deribit_wrapper-0.2.0/deribit_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-02 14:10:52.000000 deribit_wrapper-0.2.0/deribit_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 14:10:52.000000 deribit_wrapper-0.2.0/deribit_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-02 14:10:52.000000 deribit_wrapper-0.2.0/deribit_wrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-02 14:10:52.000000 deribit_wrapper-0.2.0/deribit_wrapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 14:10:52.334598 deribit_wrapper-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-02 14:10:42.000000 deribit_wrapper-0.2.0/setup.py
```

### Comparing `deribit_wrapper-0.1.4/LICENSE` & `deribit_wrapper-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deribit_wrapper-0.1.4/PKG-INFO` & `deribit_wrapper-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deribit_wrapper
-Version: 0.1.4
+Version: 0.2.0
 Summary: A Python wrapper for seamless integration with Deribit's trading API, offering easy access to market data, account management, and trading operations.
 Home-page: https://github.com/AntonioVentilii/deribit-wrapper
 Author: Antonio Ventilii
 Author-email: antonioventilii@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/AntonioVentilii/deribit-wrapper
 Project-URL: Issue Tracker, https://github.com/AntonioVentilii/deribit-wrapper/issues
```

### Comparing `deribit_wrapper-0.1.4/README.md` & `deribit_wrapper-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `deribit_wrapper-0.1.4/deribit_wrapper/account_management.py` & `deribit_wrapper-0.2.0/deribit_wrapper/account_management.py`

 * *Files identical despite different names*

### Comparing `deribit_wrapper-0.1.4/deribit_wrapper/authentication.py` & `deribit_wrapper-0.2.0/deribit_wrapper/authentication.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,44 @@
 from __future__ import absolute_import, annotations
 
 import json
 import time
+import warnings
 
 import requests
 from requests.adapters import HTTPAdapter
 from urllib3.util.retry import Retry
 
 from .base import DeribitBase
+from .exceptions import DeribitClientWarning
 
 
 class Authentication(DeribitBase):
     __AUTH = '/public/auth'
 
     def __init__(self, env: str = 'prod', client_id: str = None, client_secret: str = None):
         super().__init__(env=env)
+        self._client_id = None
+        self._client_secret = None
+        self.set_credentials(client_id, client_secret)
+
+    @property
+    def client_id(self) -> str:
+        return self._client_id
+
+    @property
+    def client_secret(self) -> str:
+        return self._client_secret
+
+    def set_credentials(self, client_id: str, client_secret: str):
         if not client_id or not client_secret:
-            print('Client ID or Client Secret not provided. Only \'public\' requests will be available.')
-        self.client_id = client_id
-        self.client_secret = client_secret
+            txt = 'Client ID or Client Secret not provided. Only \'public\' requests will be available.'
+            warnings.warn(txt, DeribitClientWarning)
+        self._client_id = client_id
+        self._client_secret = client_secret
 
     @property
     def _session(self):
         session = requests.Session()
         retry = Retry(connect=3, backoff_factor=0.5)
         adapter = HTTPAdapter(max_retries=retry)
         session.mount('http://', adapter)
```

### Comparing `deribit_wrapper-0.1.4/deribit_wrapper/base.py` & `deribit_wrapper-0.2.0/deribit_wrapper/base.py`

 * *Files identical despite different names*

### Comparing `deribit_wrapper-0.1.4/deribit_wrapper/core.py` & `deribit_wrapper-0.2.0/deribit_wrapper/core.py`

 * *Files identical despite different names*

### Comparing `deribit_wrapper-0.1.4/deribit_wrapper/market_data.py` & `deribit_wrapper-0.2.0/deribit_wrapper/market_data.py`

 * *Files identical despite different names*

### Comparing `deribit_wrapper-0.1.4/deribit_wrapper/trading.py` & `deribit_wrapper-0.2.0/deribit_wrapper/trading.py`

 * *Files 16% similar despite different names*

```diff
@@ -73,14 +73,59 @@
                 results = results.merge(orders, how='left', on='order_id', suffixes=(None, '_duplicate'))
         results.sort_values('timestamp', inplace=True)
         return results
 
     def get_entire_trade_history(self, include_order_data: bool = False) -> pd.DataFrame:
         return self.get_trade_history(include_order_data=include_order_data)
 
+    def _error_handler(self, ret: dict, uri: str, params: dict, exclude_codes: list[int] = None) -> dict:
+        exclude_codes = exclude_codes or []
+        code = ret.get('code')
+
+        # 0: no error
+        if code == 0 or code is None:
+            pass
+
+        # 10009: not enough funds
+        elif code == 10009 and 10009 not in exclude_codes:
+            if params.get('reduce_only'):
+                print('Not enough funds. Already tried as reduce only.')
+            else:
+                params['reduce_only'] = True
+                max_attempts = 3
+                for i in range(max_attempts):
+                    print(f'Not enough funds. Attempt {i + 1} of {max_attempts} as reduce only...')
+                    ret = self._order_with_error_handling(uri, params, exclude_codes=[10009])
+                    code = ret.get('code')
+                    if code != 10009:
+                        break
+
+        # 10041: settlement in progress
+        elif code == 10041 and 10041 not in exclude_codes:
+            max_attempts = 60
+            for i in range(max_attempts):
+                print('Settlement in progress. Waiting 1 second...')
+                time.sleep(1)
+                ret = self._order_with_error_handling(uri, params, exclude_codes=[10041])
+                code = ret.get('code')
+                if code != 10041:
+                    break
+
+        else:
+            print(f'Error code {code} not handled yet.')
+
+        return ret
+
+    def _order_with_error_handling(self, uri: str, params: dict, handle_error: bool = True,
+                                   exclude_codes: list[int] = None) -> dict:
+        ret = self._request(uri, params)
+        if handle_error:
+            ret = self._error_handler(ret, uri, params, exclude_codes=exclude_codes)
+        return ret
+
     def _order(self, asset: str, amount: float | int, limit: float | int = None, label: str = None,
                reduce_only: bool = False) -> dict:
         label = None if label == '' else label
         if amount > 0:
             uri = self.__BUY
             side = 'buy'
         elif amount < 0:
@@ -108,20 +153,15 @@
                 'reduce_only': reduce_only,
             }
             if limit is not None:
                 params['type'] = 'limit'
                 params['price'] = limit
             if label is not None:
                 params['label'] = label
-            r = self._request(uri, params)
-            ret = r
-            while ret.get('code') == 10041:
-                time.sleep(1)
-                r = self._request(uri, params)
-                ret = r
+            ret = self._order_with_error_handling(uri, params)
         return ret
 
     def order(self, asset: str, amount: float | int, limit: float | int = None, label: str = None,
               reduce_only: bool = False) -> dict:
         self.check_min_trade_amount([(asset, amount)])
         try:
             ret = self._order(asset, amount, limit=limit, label=label, reduce_only=reduce_only)
```

### Comparing `deribit_wrapper-0.1.4/deribit_wrapper/utilities.py` & `deribit_wrapper-0.2.0/deribit_wrapper/utilities.py`

 * *Files identical despite different names*

### Comparing `deribit_wrapper-0.1.4/deribit_wrapper.egg-info/PKG-INFO` & `deribit_wrapper-0.2.0/deribit_wrapper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deribit-wrapper
-Version: 0.1.4
+Version: 0.2.0
 Summary: A Python wrapper for seamless integration with Deribit's trading API, offering easy access to market data, account management, and trading operations.
 Home-page: https://github.com/AntonioVentilii/deribit-wrapper
 Author: Antonio Ventilii
 Author-email: antonioventilii@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/AntonioVentilii/deribit-wrapper
 Project-URL: Issue Tracker, https://github.com/AntonioVentilii/deribit-wrapper/issues
```

### Comparing `deribit_wrapper-0.1.4/setup.py` & `deribit_wrapper-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='deribit_wrapper',
-    version='0.1.4',
+    version='0.2.0',
     packages=find_packages(),
     description='A Python wrapper for seamless integration with Deribit\'s trading API, offering easy access to '
                 'market data, account management, and trading operations.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Antonio Ventilii',
     author_email='antonioventilii@gmail.com',
```

