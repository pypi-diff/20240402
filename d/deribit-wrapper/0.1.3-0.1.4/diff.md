# Comparing `tmp/deribit_wrapper-0.1.3.tar.gz` & `tmp/deribit_wrapper-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deribit_wrapper-0.1.3.tar", last modified: Fri Mar 29 22:47:01 2024, max compression
+gzip compressed data, was "deribit_wrapper-0.1.4.tar", last modified: Mon Apr  1 22:07:03 2024, max compression
```

## Comparing `deribit_wrapper-0.1.3.tar` & `deribit_wrapper-0.1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:47:01.765905 deribit_wrapper-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-03-29 22:46:54.000000 deribit_wrapper-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-03-29 22:47:01.765905 deribit_wrapper-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-03-29 22:46:54.000000 deribit_wrapper-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:47:01.765905 deribit_wrapper-0.1.3/deribit_wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-29 22:46:54.000000 deribit_wrapper-0.1.3/deribit_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5068 2024-03-29 22:46:54.000000 deribit_wrapper-0.1.3/deribit_wrapper/account_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-03-29 22:46:54.000000 deribit_wrapper-0.1.3/deribit_wrapper/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-03-29 22:46:54.000000 deribit_wrapper-0.1.3/deribit_wrapper/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-03-29 22:46:54.000000 deribit_wrapper-0.1.3/deribit_wrapper/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    11699 2024-03-29 22:46:54.000000 deribit_wrapper-0.1.3/deribit_wrapper/market_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     6191 2024-03-29 22:46:54.000000 deribit_wrapper-0.1.3/deribit_wrapper/trading.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-03-29 22:46:54.000000 deribit_wrapper-0.1.3/deribit_wrapper/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:47:01.765905 deribit_wrapper-0.1.3/deribit_wrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-03-29 22:47:01.000000 deribit_wrapper-0.1.3/deribit_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-03-29 22:47:01.000000 deribit_wrapper-0.1.3/deribit_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 22:47:01.000000 deribit_wrapper-0.1.3/deribit_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-29 22:47:01.000000 deribit_wrapper-0.1.3/deribit_wrapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-29 22:47:01.000000 deribit_wrapper-0.1.3/deribit_wrapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 22:47:01.765905 deribit_wrapper-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-03-29 22:46:54.000000 deribit_wrapper-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:07:03.751854 deribit_wrapper-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-01 22:06:52.000000 deribit_wrapper-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-04-01 22:07:03.751854 deribit_wrapper-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-04-01 22:06:52.000000 deribit_wrapper-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:07:03.751854 deribit_wrapper-0.1.4/deribit_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-01 22:06:52.000000 deribit_wrapper-0.1.4/deribit_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-04-01 22:06:52.000000 deribit_wrapper-0.1.4/deribit_wrapper/account_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-04-01 22:06:52.000000 deribit_wrapper-0.1.4/deribit_wrapper/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-01 22:06:52.000000 deribit_wrapper-0.1.4/deribit_wrapper/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-01 22:06:52.000000 deribit_wrapper-0.1.4/deribit_wrapper/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11801 2024-04-01 22:06:52.000000 deribit_wrapper-0.1.4/deribit_wrapper/market_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6191 2024-04-01 22:06:52.000000 deribit_wrapper-0.1.4/deribit_wrapper/trading.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-01 22:06:52.000000 deribit_wrapper-0.1.4/deribit_wrapper/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:07:03.751854 deribit_wrapper-0.1.4/deribit_wrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-04-01 22:07:03.000000 deribit_wrapper-0.1.4/deribit_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-01 22:07:03.000000 deribit_wrapper-0.1.4/deribit_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 22:07:03.000000 deribit_wrapper-0.1.4/deribit_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-01 22:07:03.000000 deribit_wrapper-0.1.4/deribit_wrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-01 22:07:03.000000 deribit_wrapper-0.1.4/deribit_wrapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 22:07:03.751854 deribit_wrapper-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-01 22:06:52.000000 deribit_wrapper-0.1.4/setup.py
```

### Comparing `deribit_wrapper-0.1.3/LICENSE` & `deribit_wrapper-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `deribit_wrapper-0.1.3/PKG-INFO` & `deribit_wrapper-0.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deribit_wrapper
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python wrapper for seamless integration with Deribit's trading API, offering easy access to market data, account management, and trading operations.
 Home-page: https://github.com/AntonioVentilii/deribit-wrapper
 Author: Antonio Ventilii
 Author-email: antonioventilii@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/AntonioVentilii/deribit-wrapper
 Project-URL: Issue Tracker, https://github.com/AntonioVentilii/deribit-wrapper/issues
@@ -66,26 +66,29 @@
 
 ### Market Data
 
 - **Get Contract Size:** `get_contract_size(asset)`
 - **Get Currencies:** `get_currencies()`
 - **Get Ticker Information:** `get_ticker(asset)`
 - **Get Book Summary by Currency:** `get_complete_market_book()`
+- and more...
 
 ### Account Information
 
 - **Authenticate:** Automatically handled during requests to private endpoints.
 - **Get Account Summary:** `get_account_summary(currency)`
 - **Get Positions:** `get_positions(currency, kind)`
+- and more...
 
 ### Trading
 
 - **Place an Order:** `order(asset, amount, limit=None, label=None, reduce_only=False)`
 - **Place a Market Order:** `market_order(asset, amount, label=None, reduce_only=False)`
 - **Bulk Orders:** `bulk_order(orders, label=None)`
+- and more...
 
 ## Examples
 
 1. **Retrieving Market Data:**
 
 ```python
 ticker_info = client.get_ticker('BTC-25JUN21')
```

### Comparing `deribit_wrapper-0.1.3/README.md` & `deribit_wrapper-0.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -48,26 +48,29 @@
 
 ### Market Data
 
 - **Get Contract Size:** `get_contract_size(asset)`
 - **Get Currencies:** `get_currencies()`
 - **Get Ticker Information:** `get_ticker(asset)`
 - **Get Book Summary by Currency:** `get_complete_market_book()`
+- and more...
 
 ### Account Information
 
 - **Authenticate:** Automatically handled during requests to private endpoints.
 - **Get Account Summary:** `get_account_summary(currency)`
 - **Get Positions:** `get_positions(currency, kind)`
+- and more...
 
 ### Trading
 
 - **Place an Order:** `order(asset, amount, limit=None, label=None, reduce_only=False)`
 - **Place a Market Order:** `market_order(asset, amount, label=None, reduce_only=False)`
 - **Bulk Orders:** `bulk_order(orders, label=None)`
+- and more...
 
 ## Examples
 
 1. **Retrieving Market Data:**
 
 ```python
 ticker_info = client.get_ticker('BTC-25JUN21')
```

### Comparing `deribit_wrapper-0.1.3/deribit_wrapper/account_management.py` & `deribit_wrapper-0.1.4/deribit_wrapper/account_management.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,19 @@
         for c in currency:
             params['currency'] = c
             r = self._request(uri, params)
             r = {k: [v] for k, v in r.items()}
             ret = pd.concat([ret, pd.DataFrame(r)], ignore_index=True)
         return ret
 
+    def get_margin_model(self, currency: str | list[str] = None) -> pd.DataFrame:
+        df = self.get_account_summary(currency)
+        df = df[['currency', 'margin_model', 'portfolio_margining_enabled', 'cross_collateral_enabled']]
+        return df
+
     def get_positions(self, currency: str | list[str] = None, kind: str = None) -> pd.DataFrame:
         uri = self.__GET_POSITIONS
         params = {'currency': ''}
         if kind is not None:
             params['kind'] = kind
         if currency is None:
             currency = self.currencies
```

### Comparing `deribit_wrapper-0.1.3/deribit_wrapper/authentication.py` & `deribit_wrapper-0.1.4/deribit_wrapper/authentication.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 class Authentication(DeribitBase):
     __AUTH = '/public/auth'
 
     def __init__(self, env: str = 'prod', client_id: str = None, client_secret: str = None):
         super().__init__(env=env)
         if not client_id or not client_secret:
-            print('Client ID or Client Secret not provided. Token will not be generated. Private requests will fail.')
+            print('Client ID or Client Secret not provided. Only \'public\' requests will be available.')
         self.client_id = client_id
         self.client_secret = client_secret
 
     @property
     def _session(self):
         session = requests.Session()
         retry = Retry(connect=3, backoff_factor=0.5)
```

### Comparing `deribit_wrapper-0.1.3/deribit_wrapper/base.py` & `deribit_wrapper-0.1.4/deribit_wrapper/base.py`

 * *Files identical despite different names*

### Comparing `deribit_wrapper-0.1.3/deribit_wrapper/core.py` & `deribit_wrapper-0.1.4/deribit_wrapper/core.py`

 * *Files identical despite different names*

### Comparing `deribit_wrapper-0.1.3/deribit_wrapper/market_data.py` & `deribit_wrapper-0.1.4/deribit_wrapper/market_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -225,18 +225,20 @@
         uri = self.__GET_TICKER_URI
         params = {'instrument_name': asset}
         ret = self._request(uri, params)
         return ret
 
     def last_price(self, asset: str) -> float:
         ticker = self.get_ticker(asset)
-        ret = ticker['last_price']
+        ret = ticker.get('last_price')
         if ret is None:
-            ret = ticker['mark_price']
+            ret = ticker.get('mark_price')
             logging.warning(f'Using mark price instead of last price for asset {asset}.')
+        if ret is None:
+            raise Exception(f'No price available for asset {asset}.')
         return ret
 
     def mid_price(self, asset: str) -> float:
         ticker = self.get_ticker(asset)
         bid = ticker['best_bid_price']
         ask = ticker['best_ask_price']
         if bid is None and ask is None:
```

### Comparing `deribit_wrapper-0.1.3/deribit_wrapper/trading.py` & `deribit_wrapper-0.1.4/deribit_wrapper/trading.py`

 * *Files identical despite different names*

### Comparing `deribit_wrapper-0.1.3/deribit_wrapper/utilities.py` & `deribit_wrapper-0.1.4/deribit_wrapper/utilities.py`

 * *Files identical despite different names*

### Comparing `deribit_wrapper-0.1.3/deribit_wrapper.egg-info/PKG-INFO` & `deribit_wrapper-0.1.4/deribit_wrapper.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deribit-wrapper
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python wrapper for seamless integration with Deribit's trading API, offering easy access to market data, account management, and trading operations.
 Home-page: https://github.com/AntonioVentilii/deribit-wrapper
 Author: Antonio Ventilii
 Author-email: antonioventilii@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/AntonioVentilii/deribit-wrapper
 Project-URL: Issue Tracker, https://github.com/AntonioVentilii/deribit-wrapper/issues
@@ -66,26 +66,29 @@
 
 ### Market Data
 
 - **Get Contract Size:** `get_contract_size(asset)`
 - **Get Currencies:** `get_currencies()`
 - **Get Ticker Information:** `get_ticker(asset)`
 - **Get Book Summary by Currency:** `get_complete_market_book()`
+- and more...
 
 ### Account Information
 
 - **Authenticate:** Automatically handled during requests to private endpoints.
 - **Get Account Summary:** `get_account_summary(currency)`
 - **Get Positions:** `get_positions(currency, kind)`
+- and more...
 
 ### Trading
 
 - **Place an Order:** `order(asset, amount, limit=None, label=None, reduce_only=False)`
 - **Place a Market Order:** `market_order(asset, amount, label=None, reduce_only=False)`
 - **Bulk Orders:** `bulk_order(orders, label=None)`
+- and more...
 
 ## Examples
 
 1. **Retrieving Market Data:**
 
 ```python
 ticker_info = client.get_ticker('BTC-25JUN21')
```

### Comparing `deribit_wrapper-0.1.3/setup.py` & `deribit_wrapper-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='deribit_wrapper',
-    version='0.1.3',
+    version='0.1.4',
     packages=find_packages(),
     description='A Python wrapper for seamless integration with Deribit\'s trading API, offering easy access to '
                 'market data, account management, and trading operations.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Antonio Ventilii',
     author_email='antonioventilii@gmail.com',
```

