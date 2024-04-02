# Comparing `tmp/ccxtools-0.0.98.tar.gz` & `tmp/ccxtools-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccxtools-0.0.98.tar", last modified: Mon Oct 30 16:04:11 2023, max compression
+gzip compressed data, was "ccxtools-0.0.99.tar", last modified: Mon Oct 30 17:09:35 2023, max compression
```

## Comparing `ccxtools-0.0.98.tar` & `ccxtools-0.0.99.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 woosub_private   (502) staff       (20)        0 2023-10-30 16:04:11.708058 ccxtools-0.0.98/
--rw-r--r--   0 woosub_private   (502) staff       (20)     1531 2023-10-30 16:04:11.707991 ccxtools-0.0.98/PKG-INFO
--rw-r--r--   0 woosub_private   (502) staff       (20)     1145 2022-06-23 14:28:30.000000 ccxtools-0.0.98/README.md
--rw-r--r--   0 woosub_private   (502) staff       (20)       84 2022-06-23 14:28:30.000000 ccxtools-0.0.98/pyproject.toml
--rw-r--r--   0 woosub_private   (502) staff       (20)      534 2023-10-30 16:04:11.708351 ccxtools-0.0.98/setup.cfg
-drwxr-xr-x   0 woosub_private   (502) staff       (20)        0 2023-10-30 16:04:11.702627 ccxtools-0.0.98/src/
-drwxr-xr-x   0 woosub_private   (502) staff       (20)        0 2023-10-30 16:04:11.704606 ccxtools-0.0.98/src/ccxtools/
--rw-r--r--   0 woosub_private   (502) staff       (20)        0 2022-06-23 14:28:30.000000 ccxtools-0.0.98/src/ccxtools/__init__.py
-drwxr-xr-x   0 woosub_private   (502) staff       (20)        0 2023-10-30 16:04:11.705953 ccxtools-0.0.98/src/ccxtools/base/
--rw-r--r--   0 woosub_private   (502) staff       (20)      724 2023-10-30 16:02:48.000000 ccxtools-0.0.98/src/ccxtools/base/CcxtExchange.py
--rw-r--r--   0 woosub_private   (502) staff       (20)      884 2023-10-30 16:02:44.000000 ccxtools-0.0.98/src/ccxtools/base/CcxtFutureExchange.py
--rw-r--r--   0 woosub_private   (502) staff       (20)      280 2023-10-30 16:00:10.000000 ccxtools-0.0.98/src/ccxtools/base/Exchange.py
--rw-r--r--   0 woosub_private   (502) staff       (20)      661 2023-10-30 13:17:19.000000 ccxtools-0.0.98/src/ccxtools/base/FutureExchange.py
--rw-r--r--   0 woosub_private   (502) staff       (20)        0 2023-07-02 08:02:25.000000 ccxtools-0.0.98/src/ccxtools/base/__init__.py
--rw-r--r--   0 woosub_private   (502) staff       (20)     1391 2023-10-30 16:03:55.000000 ccxtools-0.0.98/src/ccxtools/binance.py
--rw-r--r--   0 woosub_private   (502) staff       (20)     2584 2023-10-30 16:03:25.000000 ccxtools-0.0.98/src/ccxtools/binance_coin.py
--rw-r--r--   0 woosub_private   (502) staff       (20)     3773 2023-09-16 15:04:35.000000 ccxtools-0.0.98/src/ccxtools/binance_usdt.py
--rw-r--r--   0 woosub_private   (502) staff       (20)    11406 2023-10-30 13:17:19.000000 ccxtools-0.0.98/src/ccxtools/bingx.py
--rw-r--r--   0 woosub_private   (502) staff       (20)     2829 2023-10-30 13:17:19.000000 ccxtools-0.0.98/src/ccxtools/bitget.py
--rw-r--r--   0 woosub_private   (502) staff       (20)     5226 2023-10-30 13:17:19.000000 ccxtools-0.0.98/src/ccxtools/bybit.py
-drwxr-xr-x   0 woosub_private   (502) staff       (20)        0 2023-10-30 16:04:11.706161 ccxtools-0.0.98/src/ccxtools/ccserver/
--rw-r--r--   0 woosub_private   (502) staff       (20)        0 2023-01-19 18:00:04.000000 ccxtools-0.0.98/src/ccxtools/ccserver/__init__.py
--rw-r--r--   0 woosub_private   (502) staff       (20)      860 2023-09-30 16:26:56.000000 ccxtools-0.0.98/src/ccxtools/ccserver/server_fetcher.py
--rw-r--r--   0 woosub_private   (502) staff       (20)     4393 2023-10-30 13:17:19.000000 ccxtools-0.0.98/src/ccxtools/huobi.py
--rw-r--r--   0 woosub_private   (502) staff       (20)     1256 2022-07-10 16:08:54.000000 ccxtools-0.0.98/src/ccxtools/okx.py
--rw-r--r--   0 woosub_private   (502) staff       (20)     1828 2023-09-15 16:33:43.000000 ccxtools-0.0.98/src/ccxtools/tools.py
--rw-r--r--   0 woosub_private   (502) staff       (20)     2126 2023-10-30 16:03:55.000000 ccxtools-0.0.98/src/ccxtools/upbit.py
-drwxr-xr-x   0 woosub_private   (502) staff       (20)        0 2023-10-30 16:04:11.705285 ccxtools-0.0.98/src/ccxtools.egg-info/
--rw-r--r--   0 woosub_private   (502) staff       (20)     1531 2023-10-30 16:04:11.000000 ccxtools-0.0.98/src/ccxtools.egg-info/PKG-INFO
--rw-r--r--   0 woosub_private   (502) staff       (20)      912 2023-10-30 16:04:11.000000 ccxtools-0.0.98/src/ccxtools.egg-info/SOURCES.txt
--rw-r--r--   0 woosub_private   (502) staff       (20)        1 2023-10-30 16:04:11.000000 ccxtools-0.0.98/src/ccxtools.egg-info/dependency_links.txt
--rw-r--r--   0 woosub_private   (502) staff       (20)       56 2023-10-30 16:04:11.000000 ccxtools-0.0.98/src/ccxtools.egg-info/requires.txt
--rw-r--r--   0 woosub_private   (502) staff       (20)        9 2023-10-30 16:04:11.000000 ccxtools-0.0.98/src/ccxtools.egg-info/top_level.txt
-drwxr-xr-x   0 woosub_private   (502) staff       (20)        0 2023-10-30 16:04:11.707714 ccxtools-0.0.98/tests/
--rw-r--r--   0 woosub_private   (502) staff       (20)      667 2023-10-30 15:53:11.000000 ccxtools-0.0.98/tests/test_binance.py
--rw-r--r--   0 woosub_private   (502) staff       (20)     3395 2023-10-30 15:23:01.000000 ccxtools-0.0.98/tests/test_binance_coin.py
--rw-r--r--   0 woosub_private   (502) staff       (20)     2922 2023-10-30 13:15:27.000000 ccxtools-0.0.98/tests/test_binance_usdt.py
--rw-r--r--   0 woosub_private   (502) staff       (20)     4494 2023-10-03 07:23:08.000000 ccxtools-0.0.98/tests/test_bingx.py
--rw-r--r--   0 woosub_private   (502) staff       (20)     2311 2023-10-03 07:23:32.000000 ccxtools-0.0.98/tests/test_bitget.py
--rw-r--r--   0 woosub_private   (502) staff       (20)     2866 2023-10-03 07:23:55.000000 ccxtools-0.0.98/tests/test_bybit.py
--rw-r--r--   0 woosub_private   (502) staff       (20)     2142 2023-10-03 07:24:15.000000 ccxtools-0.0.98/tests/test_huobi.py
--rw-r--r--   0 woosub_private   (502) staff       (20)      652 2023-09-03 14:44:13.000000 ccxtools-0.0.98/tests/test_okx.py
--rw-r--r--   0 woosub_private   (502) staff       (20)     2223 2023-10-30 16:03:55.000000 ccxtools-0.0.98/tests/test_upbit.py
+drwxr-xr-x   0 woosub_private   (502) staff       (20)        0 2023-10-30 17:09:35.219689 ccxtools-0.0.99/
+-rw-r--r--   0 woosub_private   (502) staff       (20)     1531 2023-10-30 17:09:35.219626 ccxtools-0.0.99/PKG-INFO
+-rw-r--r--   0 woosub_private   (502) staff       (20)     1145 2022-06-23 14:28:30.000000 ccxtools-0.0.99/README.md
+-rw-r--r--   0 woosub_private   (502) staff       (20)       84 2022-06-23 14:28:30.000000 ccxtools-0.0.99/pyproject.toml
+-rw-r--r--   0 woosub_private   (502) staff       (20)      534 2023-10-30 17:09:35.219957 ccxtools-0.0.99/setup.cfg
+drwxr-xr-x   0 woosub_private   (502) staff       (20)        0 2023-10-30 17:09:35.214844 ccxtools-0.0.99/src/
+drwxr-xr-x   0 woosub_private   (502) staff       (20)        0 2023-10-30 17:09:35.216873 ccxtools-0.0.99/src/ccxtools/
+-rw-r--r--   0 woosub_private   (502) staff       (20)        0 2022-06-23 14:28:30.000000 ccxtools-0.0.99/src/ccxtools/__init__.py
+drwxr-xr-x   0 woosub_private   (502) staff       (20)        0 2023-10-30 17:09:35.218100 ccxtools-0.0.99/src/ccxtools/base/
+-rw-r--r--   0 woosub_private   (502) staff       (20)      724 2023-10-30 16:02:48.000000 ccxtools-0.0.99/src/ccxtools/base/CcxtExchange.py
+-rw-r--r--   0 woosub_private   (502) staff       (20)      884 2023-10-30 16:02:44.000000 ccxtools-0.0.99/src/ccxtools/base/CcxtFutureExchange.py
+-rw-r--r--   0 woosub_private   (502) staff       (20)      280 2023-10-30 16:00:10.000000 ccxtools-0.0.99/src/ccxtools/base/Exchange.py
+-rw-r--r--   0 woosub_private   (502) staff       (20)      661 2023-10-30 13:17:19.000000 ccxtools-0.0.99/src/ccxtools/base/FutureExchange.py
+-rw-r--r--   0 woosub_private   (502) staff       (20)        0 2023-07-02 08:02:25.000000 ccxtools-0.0.99/src/ccxtools/base/__init__.py
+-rw-r--r--   0 woosub_private   (502) staff       (20)     1391 2023-10-30 16:03:55.000000 ccxtools-0.0.99/src/ccxtools/binance.py
+-rw-r--r--   0 woosub_private   (502) staff       (20)     2584 2023-10-30 16:03:25.000000 ccxtools-0.0.99/src/ccxtools/binance_coin.py
+-rw-r--r--   0 woosub_private   (502) staff       (20)     3773 2023-09-16 15:04:35.000000 ccxtools-0.0.99/src/ccxtools/binance_usdt.py
+-rw-r--r--   0 woosub_private   (502) staff       (20)    11406 2023-10-30 13:17:19.000000 ccxtools-0.0.99/src/ccxtools/bingx.py
+-rw-r--r--   0 woosub_private   (502) staff       (20)     2829 2023-10-30 13:17:19.000000 ccxtools-0.0.99/src/ccxtools/bitget.py
+-rw-r--r--   0 woosub_private   (502) staff       (20)     5226 2023-10-30 13:17:19.000000 ccxtools-0.0.99/src/ccxtools/bybit.py
+drwxr-xr-x   0 woosub_private   (502) staff       (20)        0 2023-10-30 17:09:35.218306 ccxtools-0.0.99/src/ccxtools/ccserver/
+-rw-r--r--   0 woosub_private   (502) staff       (20)        0 2023-01-19 18:00:04.000000 ccxtools-0.0.99/src/ccxtools/ccserver/__init__.py
+-rw-r--r--   0 woosub_private   (502) staff       (20)      860 2023-09-30 16:26:56.000000 ccxtools-0.0.99/src/ccxtools/ccserver/server_fetcher.py
+-rw-r--r--   0 woosub_private   (502) staff       (20)     4393 2023-10-30 13:17:19.000000 ccxtools-0.0.99/src/ccxtools/huobi.py
+-rw-r--r--   0 woosub_private   (502) staff       (20)     1256 2022-07-10 16:08:54.000000 ccxtools-0.0.99/src/ccxtools/okx.py
+-rw-r--r--   0 woosub_private   (502) staff       (20)     1828 2023-09-15 16:33:43.000000 ccxtools-0.0.99/src/ccxtools/tools.py
+-rw-r--r--   0 woosub_private   (502) staff       (20)     2317 2023-10-30 17:09:05.000000 ccxtools-0.0.99/src/ccxtools/upbit.py
+drwxr-xr-x   0 woosub_private   (502) staff       (20)        0 2023-10-30 17:09:35.217493 ccxtools-0.0.99/src/ccxtools.egg-info/
+-rw-r--r--   0 woosub_private   (502) staff       (20)     1531 2023-10-30 17:09:35.000000 ccxtools-0.0.99/src/ccxtools.egg-info/PKG-INFO
+-rw-r--r--   0 woosub_private   (502) staff       (20)      912 2023-10-30 17:09:35.000000 ccxtools-0.0.99/src/ccxtools.egg-info/SOURCES.txt
+-rw-r--r--   0 woosub_private   (502) staff       (20)        1 2023-10-30 17:09:35.000000 ccxtools-0.0.99/src/ccxtools.egg-info/dependency_links.txt
+-rw-r--r--   0 woosub_private   (502) staff       (20)       56 2023-10-30 17:09:35.000000 ccxtools-0.0.99/src/ccxtools.egg-info/requires.txt
+-rw-r--r--   0 woosub_private   (502) staff       (20)        9 2023-10-30 17:09:35.000000 ccxtools-0.0.99/src/ccxtools.egg-info/top_level.txt
+drwxr-xr-x   0 woosub_private   (502) staff       (20)        0 2023-10-30 17:09:35.219393 ccxtools-0.0.99/tests/
+-rw-r--r--   0 woosub_private   (502) staff       (20)      667 2023-10-30 15:53:11.000000 ccxtools-0.0.99/tests/test_binance.py
+-rw-r--r--   0 woosub_private   (502) staff       (20)     3395 2023-10-30 15:23:01.000000 ccxtools-0.0.99/tests/test_binance_coin.py
+-rw-r--r--   0 woosub_private   (502) staff       (20)     2922 2023-10-30 13:15:27.000000 ccxtools-0.0.99/tests/test_binance_usdt.py
+-rw-r--r--   0 woosub_private   (502) staff       (20)     4494 2023-10-03 07:23:08.000000 ccxtools-0.0.99/tests/test_bingx.py
+-rw-r--r--   0 woosub_private   (502) staff       (20)     2311 2023-10-03 07:23:32.000000 ccxtools-0.0.99/tests/test_bitget.py
+-rw-r--r--   0 woosub_private   (502) staff       (20)     2866 2023-10-03 07:23:55.000000 ccxtools-0.0.99/tests/test_bybit.py
+-rw-r--r--   0 woosub_private   (502) staff       (20)     2142 2023-10-03 07:24:15.000000 ccxtools-0.0.99/tests/test_huobi.py
+-rw-r--r--   0 woosub_private   (502) staff       (20)      652 2023-09-03 14:44:13.000000 ccxtools-0.0.99/tests/test_okx.py
+-rw-r--r--   0 woosub_private   (502) staff       (20)     2224 2023-10-30 17:09:05.000000 ccxtools-0.0.99/tests/test_upbit.py
```

### Comparing `ccxtools-0.0.98/PKG-INFO` & `ccxtools-0.0.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccxtools
-Version: 0.0.98
+Version: 0.0.99
 Summary: ccxtools
 Home-page: https://github.com/WoosubLeee/ccxtools
 Author: Woosub Lee
 Author-email: zbxv1423@naver.com
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `ccxtools-0.0.98/README.md` & `ccxtools-0.0.99/README.md`

 * *Files identical despite different names*

### Comparing `ccxtools-0.0.98/setup.cfg` & `ccxtools-0.0.99/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ccxtools
-version = 0.0.98
+version = 0.0.99
 author = Woosub Lee
 author_email = zbxv1423@naver.com
 description = ccxtools
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/WoosubLeee/ccxtools
 classifiers =
```

### Comparing `ccxtools-0.0.98/src/ccxtools/base/CcxtExchange.py` & `ccxtools-0.0.99/src/ccxtools/base/CcxtExchange.py`

 * *Files identical despite different names*

### Comparing `ccxtools-0.0.98/src/ccxtools/base/CcxtFutureExchange.py` & `ccxtools-0.0.99/src/ccxtools/base/CcxtFutureExchange.py`

 * *Files identical despite different names*

### Comparing `ccxtools-0.0.98/src/ccxtools/base/FutureExchange.py` & `ccxtools-0.0.99/src/ccxtools/base/FutureExchange.py`

 * *Files identical despite different names*

### Comparing `ccxtools-0.0.98/src/ccxtools/binance.py` & `ccxtools-0.0.99/src/ccxtools/binance.py`

 * *Files identical despite different names*

### Comparing `ccxtools-0.0.98/src/ccxtools/binance_coin.py` & `ccxtools-0.0.99/src/ccxtools/binance_coin.py`

 * *Files identical despite different names*

### Comparing `ccxtools-0.0.98/src/ccxtools/binance_usdt.py` & `ccxtools-0.0.99/src/ccxtools/binance_usdt.py`

 * *Files identical despite different names*

### Comparing `ccxtools-0.0.98/src/ccxtools/bingx.py` & `ccxtools-0.0.99/src/ccxtools/bingx.py`

 * *Files identical despite different names*

### Comparing `ccxtools-0.0.98/src/ccxtools/bitget.py` & `ccxtools-0.0.99/src/ccxtools/bitget.py`

 * *Files identical despite different names*

### Comparing `ccxtools-0.0.98/src/ccxtools/bybit.py` & `ccxtools-0.0.99/src/ccxtools/bybit.py`

 * *Files identical despite different names*

### Comparing `ccxtools-0.0.98/src/ccxtools/ccserver/server_fetcher.py` & `ccxtools-0.0.99/src/ccxtools/ccserver/server_fetcher.py`

 * *Files identical despite different names*

### Comparing `ccxtools-0.0.98/src/ccxtools/huobi.py` & `ccxtools-0.0.99/src/ccxtools/huobi.py`

 * *Files identical despite different names*

### Comparing `ccxtools-0.0.98/src/ccxtools/okx.py` & `ccxtools-0.0.99/src/ccxtools/okx.py`

 * *Files identical despite different names*

### Comparing `ccxtools-0.0.98/src/ccxtools/tools.py` & `ccxtools-0.0.99/src/ccxtools/tools.py`

 * *Files identical despite different names*

### Comparing `ccxtools-0.0.98/src/ccxtools/upbit.py` & `ccxtools-0.0.99/src/ccxtools/upbit.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,26 @@
+import types
+from random import randrange
 import ccxt
+
 from ccxtools.base.CcxtExchange import CcxtExchange
 from ccxtools.tools import get_async_results
 
 
 class Upbit(CcxtExchange):
     DEPOSIT_COMPLETE_STATUSES = ['ACCEPTED', 'CANCELLED', 'REJECTED', 'REFUNDED']
     WITHDRAWAL_COMPLETE_STATUSES = ['DONE', 'FAILED', 'CANCELLED', 'REJECTED']
 
     def __init__(self, who, env_vars):
         super().__init__(env_vars)
         self.ccxt_inst = ccxt.upbit({
             'apiKey': env_vars(f'UPBIT_API_KEY{who}'),
             'secret': env_vars(f'UPBIT_SECRET_KEY{who}')
         })
+        self.ccxt_inst.nonce = types.MethodType(nonce, self.ccxt_inst)
 
     def get_last_price(self, ticker):
         res = self.ccxt_inst.fetch_ticker(f'{ticker}/KRW')
         return res['last']
 
     def get_last_prices(self, tickers):
         ticker_datas = self.ccxt_inst.fetch_tickers()
@@ -50,7 +54,11 @@
     def post_withdraw(self, ticker, amount, destination):
         address = self.env_vars(f'{destination}_{ticker}_ADDRESS')
         tag = self.env_vars(f'{destination}_{ticker}_TAG') if ticker in self.WITHDRAW_TAG_NECESSARY_TICKERS else None
 
         self.ccxt_inst.withdraw(ticker, amount, address, tag, {
             'net_type': ticker
         })
+
+
+def nonce(self):
+    return f'{self.milliseconds()}-{randrange(100, 999)}'
```

### Comparing `ccxtools-0.0.98/src/ccxtools.egg-info/PKG-INFO` & `ccxtools-0.0.99/src/ccxtools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccxtools
-Version: 0.0.98
+Version: 0.0.99
 Summary: ccxtools
 Home-page: https://github.com/WoosubLeee/ccxtools
 Author: Woosub Lee
 Author-email: zbxv1423@naver.com
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `ccxtools-0.0.98/src/ccxtools.egg-info/SOURCES.txt` & `ccxtools-0.0.99/src/ccxtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ccxtools-0.0.98/tests/test_binance.py` & `ccxtools-0.0.99/tests/test_binance.py`

 * *Files identical despite different names*

### Comparing `ccxtools-0.0.98/tests/test_binance_coin.py` & `ccxtools-0.0.99/tests/test_binance_coin.py`

 * *Files identical despite different names*

### Comparing `ccxtools-0.0.98/tests/test_binance_usdt.py` & `ccxtools-0.0.99/tests/test_binance_usdt.py`

 * *Files identical despite different names*

### Comparing `ccxtools-0.0.98/tests/test_bingx.py` & `ccxtools-0.0.99/tests/test_bingx.py`

 * *Files identical despite different names*

### Comparing `ccxtools-0.0.98/tests/test_bitget.py` & `ccxtools-0.0.99/tests/test_bitget.py`

 * *Files identical despite different names*

### Comparing `ccxtools-0.0.98/tests/test_bybit.py` & `ccxtools-0.0.99/tests/test_bybit.py`

 * *Files identical despite different names*

### Comparing `ccxtools-0.0.98/tests/test_huobi.py` & `ccxtools-0.0.99/tests/test_huobi.py`

 * *Files identical despite different names*

### Comparing `ccxtools-0.0.98/tests/test_okx.py` & `ccxtools-0.0.99/tests/test_okx.py`

 * *Files identical despite different names*

### Comparing `ccxtools-0.0.98/tests/test_upbit.py` & `ccxtools-0.0.99/tests/test_upbit.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 def test_get_best_book_price(upbit):
     assert isinstance(upbit.get_best_book_price('BTC', 'ask'), float)
     assert isinstance(upbit.get_best_book_price('BTC', 'bid'), float)
 
 
 def test_is_transferring(upbit, env_vars):
     # Test input Start
-    is_transferring = True
+    is_transferring = False
     withdraw_option = {
         'ticker': 'SOL',
         'amount': 0.01,
         'destination': 'BINANCE',
     }
     # Test input End
```

