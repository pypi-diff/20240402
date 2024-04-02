# Comparing `tmp/trading-backend-1.2.8.tar.gz` & `tmp/trading-backend-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trading-backend-1.2.8.tar", last modified: Sun Aug 13 17:38:25 2023, max compression
+gzip compressed data, was "trading-backend-1.2.9.tar", last modified: Thu Aug 24 19:59:14 2023, max compression
```

## Comparing `trading-backend-1.2.8.tar` & `trading-backend-1.2.9.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-13 17:38:25.769878 trading-backend-1.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-08-13 17:37:55.000000 trading-backend-1.2.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-08-13 17:37:55.000000 trading-backend-1.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-08-13 17:37:55.000000 trading-backend-1.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-08-13 17:38:25.769878 trading-backend-1.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-08-13 17:37:55.000000 trading-backend-1.2.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-13 17:37:55.000000 trading-backend-1.2.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-08-13 17:38:25.769878 trading-backend-1.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-08-13 17:37:55.000000 trading-backend-1.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-13 17:38:25.757878 trading-backend-1.2.8/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-13 17:38:25.757878 trading-backend-1.2.8/tests/exchanges/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-13 17:37:55.000000 trading-backend-1.2.8/tests/exchanges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-08-13 17:37:55.000000 trading-backend-1.2.8/tests/exchanges/test_ascendex.py
--rw-r--r--   0 runner    (1001) docker     (123)    12497 2023-08-13 17:37:55.000000 trading-backend-1.2.8/tests/exchanges/test_binance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-08-13 17:37:55.000000 trading-backend-1.2.8/tests/exchanges/test_bitget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-08-13 17:37:55.000000 trading-backend-1.2.8/tests/exchanges/test_bybit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-08-13 17:37:55.000000 trading-backend-1.2.8/tests/exchanges/test_cryptocom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-08-13 17:37:55.000000 trading-backend-1.2.8/tests/exchanges/test_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-08-13 17:37:55.000000 trading-backend-1.2.8/tests/exchanges/test_gateio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-08-13 17:37:55.000000 trading-backend-1.2.8/tests/exchanges/test_huobi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-08-13 17:37:55.000000 trading-backend-1.2.8/tests/exchanges/test_huobipro.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-08-13 17:37:55.000000 trading-backend-1.2.8/tests/exchanges/test_kucoin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-08-13 17:37:55.000000 trading-backend-1.2.8/tests/exchanges/test_kucoin_futures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-08-13 17:37:55.000000 trading-backend-1.2.8/tests/exchanges/test_mexc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-08-13 17:37:55.000000 trading-backend-1.2.8/tests/exchanges/test_okx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-08-13 17:37:55.000000 trading-backend-1.2.8/tests/exchanges/test_phemex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-13 17:38:25.757878 trading-backend-1.2.8/tests/util/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-08-13 17:37:55.000000 trading-backend-1.2.8/tests/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-08-13 17:37:55.000000 trading-backend-1.2.8/tests/util/create_order_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-13 17:38:25.761878 trading-backend-1.2.8/trading_backend/
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-08-13 17:37:55.000000 trading-backend-1.2.8/trading_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-08-13 17:37:55.000000 trading-backend-1.2.8/trading_backend/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-08-13 17:37:55.000000 trading-backend-1.2.8/trading_backend/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-08-13 17:37:55.000000 trading-backend-1.2.8/trading_backend/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-08-13 17:37:55.000000 trading-backend-1.2.8/trading_backend/exchange_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-13 17:38:25.769878 trading-backend-1.2.8/trading_backend/exchanges/
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-08-13 17:37:55.000000 trading-backend-1.2.8/trading_backend/exchanges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-08-13 17:37:55.000000 trading-backend-1.2.8/trading_backend/exchanges/ascendex.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-08-13 17:37:55.000000 trading-backend-1.2.8/trading_backend/exchanges/binance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-08-13 17:37:55.000000 trading-backend-1.2.8/trading_backend/exchanges/bitget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-08-13 17:37:55.000000 trading-backend-1.2.8/trading_backend/exchanges/bybit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-08-13 17:37:55.000000 trading-backend-1.2.8/trading_backend/exchanges/cryptocom.py
--rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-08-13 17:37:55.000000 trading-backend-1.2.8/trading_backend/exchanges/exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-08-13 17:37:55.000000 trading-backend-1.2.8/trading_backend/exchanges/gateio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-08-13 17:37:55.000000 trading-backend-1.2.8/trading_backend/exchanges/huobi.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-08-13 17:37:55.000000 trading-backend-1.2.8/trading_backend/exchanges/huobipro.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-08-13 17:37:55.000000 trading-backend-1.2.8/trading_backend/exchanges/kucoin.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-08-13 17:37:55.000000 trading-backend-1.2.8/trading_backend/exchanges/kucoinfutures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-08-13 17:37:55.000000 trading-backend-1.2.8/trading_backend/exchanges/mexc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-08-13 17:37:55.000000 trading-backend-1.2.8/trading_backend/exchanges/okx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-08-13 17:37:55.000000 trading-backend-1.2.8/trading_backend/exchanges/phemex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-13 17:38:25.765878 trading-backend-1.2.8/trading_backend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-08-13 17:38:25.000000 trading-backend-1.2.8/trading_backend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-08-13 17:38:25.000000 trading-backend-1.2.8/trading_backend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-13 17:38:25.000000 trading-backend-1.2.8/trading_backend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-13 17:38:25.000000 trading-backend-1.2.8/trading_backend.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-13 17:38:25.000000 trading-backend-1.2.8/trading_backend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-13 17:38:25.000000 trading-backend-1.2.8/trading_backend.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-24 19:59:14.873717 trading-backend-1.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-08-24 19:58:33.000000 trading-backend-1.2.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-08-24 19:58:33.000000 trading-backend-1.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-08-24 19:58:33.000000 trading-backend-1.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-08-24 19:59:14.873717 trading-backend-1.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-08-24 19:58:33.000000 trading-backend-1.2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-24 19:58:33.000000 trading-backend-1.2.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-08-24 19:59:14.873717 trading-backend-1.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-08-24 19:58:33.000000 trading-backend-1.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-24 19:59:14.865717 trading-backend-1.2.9/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-24 19:59:14.869717 trading-backend-1.2.9/tests/exchanges/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-24 19:58:33.000000 trading-backend-1.2.9/tests/exchanges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-08-24 19:58:33.000000 trading-backend-1.2.9/tests/exchanges/test_ascendex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12497 2023-08-24 19:58:33.000000 trading-backend-1.2.9/tests/exchanges/test_binance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-08-24 19:58:33.000000 trading-backend-1.2.9/tests/exchanges/test_bitget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-08-24 19:58:33.000000 trading-backend-1.2.9/tests/exchanges/test_bybit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-08-24 19:58:33.000000 trading-backend-1.2.9/tests/exchanges/test_cryptocom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-08-24 19:58:33.000000 trading-backend-1.2.9/tests/exchanges/test_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-08-24 19:58:33.000000 trading-backend-1.2.9/tests/exchanges/test_gateio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-08-24 19:58:33.000000 trading-backend-1.2.9/tests/exchanges/test_huobi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-08-24 19:58:33.000000 trading-backend-1.2.9/tests/exchanges/test_huobipro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-08-24 19:58:33.000000 trading-backend-1.2.9/tests/exchanges/test_kucoin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-08-24 19:58:33.000000 trading-backend-1.2.9/tests/exchanges/test_kucoin_futures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-08-24 19:58:33.000000 trading-backend-1.2.9/tests/exchanges/test_mexc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-08-24 19:58:33.000000 trading-backend-1.2.9/tests/exchanges/test_okx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-08-24 19:58:33.000000 trading-backend-1.2.9/tests/exchanges/test_phemex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-24 19:59:14.869717 trading-backend-1.2.9/tests/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-08-24 19:58:33.000000 trading-backend-1.2.9/tests/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-08-24 19:58:33.000000 trading-backend-1.2.9/tests/util/create_order_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-24 19:59:14.869717 trading-backend-1.2.9/trading_backend/
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-08-24 19:58:33.000000 trading-backend-1.2.9/trading_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-08-24 19:58:33.000000 trading-backend-1.2.9/trading_backend/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-08-24 19:58:33.000000 trading-backend-1.2.9/trading_backend/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-08-24 19:58:33.000000 trading-backend-1.2.9/trading_backend/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-08-24 19:58:33.000000 trading-backend-1.2.9/trading_backend/exchange_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-24 19:59:14.873717 trading-backend-1.2.9/trading_backend/exchanges/
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-08-24 19:58:33.000000 trading-backend-1.2.9/trading_backend/exchanges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-08-24 19:58:33.000000 trading-backend-1.2.9/trading_backend/exchanges/ascendex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-08-24 19:58:33.000000 trading-backend-1.2.9/trading_backend/exchanges/binance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-08-24 19:58:33.000000 trading-backend-1.2.9/trading_backend/exchanges/bitget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-08-24 19:58:33.000000 trading-backend-1.2.9/trading_backend/exchanges/bybit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-08-24 19:58:33.000000 trading-backend-1.2.9/trading_backend/exchanges/cryptocom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-08-24 19:58:33.000000 trading-backend-1.2.9/trading_backend/exchanges/exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-08-24 19:58:33.000000 trading-backend-1.2.9/trading_backend/exchanges/gateio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-08-24 19:58:33.000000 trading-backend-1.2.9/trading_backend/exchanges/huobi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-08-24 19:58:33.000000 trading-backend-1.2.9/trading_backend/exchanges/huobipro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-08-24 19:58:33.000000 trading-backend-1.2.9/trading_backend/exchanges/kucoin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-08-24 19:58:33.000000 trading-backend-1.2.9/trading_backend/exchanges/kucoinfutures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-08-24 19:58:33.000000 trading-backend-1.2.9/trading_backend/exchanges/mexc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-08-24 19:58:33.000000 trading-backend-1.2.9/trading_backend/exchanges/okx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-08-24 19:58:33.000000 trading-backend-1.2.9/trading_backend/exchanges/phemex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-24 19:59:14.869717 trading-backend-1.2.9/trading_backend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-08-24 19:59:14.000000 trading-backend-1.2.9/trading_backend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-08-24 19:59:14.000000 trading-backend-1.2.9/trading_backend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-24 19:59:14.000000 trading-backend-1.2.9/trading_backend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-24 19:59:14.000000 trading-backend-1.2.9/trading_backend.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-24 19:59:14.000000 trading-backend-1.2.9/trading_backend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-24 19:59:14.000000 trading-backend-1.2.9/trading_backend.egg-info/top_level.txt
```

### Comparing `trading-backend-1.2.8/CHANGELOG.md` & `trading-backend-1.2.9/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [1.2.9] - 2023-08-23
+### Added
+- Kucoin & OKX api key right check
+
 ## [1.2.8] - 2023-08-13
 ### Added
 - withdrawal right check in api keys
 
 ## [1.2.7] - 2023-08-11
 ### Added
 - Binance api key permission checks
```

### Comparing `trading-backend-1.2.8/LICENSE` & `trading-backend-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.8/PKG-INFO` & `trading-backend-1.2.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trading-backend
-Version: 1.2.8
+Version: 1.2.9
 Summary: Trading tools
 Home-page: https://github.com/Drakkar-Software/trading-backend
 Author: Drakkar-Software
 Author-email: contact@drakkar.software
 License: LGPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
@@ -12,15 +12,15 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.8
 License-File: LICENSE
 
-# trading-backend [1.2.8](https://github.com/Drakkar-Software/trading-backend/tree/master/CHANGELOG.md)
+# trading-backend [1.2.9](https://github.com/Drakkar-Software/trading-backend/tree/master/CHANGELOG.md)
 [![PyPI](https://img.shields.io/pypi/v/trading-backend.svg)](https://pypi.python.org/pypi/trading-backend/)
 [![Downloads](https://pepy.tech/badge/trading-backend/month)](https://pepy.tech/project/trading-backend)
 [![Github-Action-CI](https://github.com/Drakkar-Software/trading-backend/workflows/trading-backend-CI/badge.svg)](https://github.com/Drakkar-Software/trading-backend/actions)
 
 - Install trading-backend from pip : 
 
 ``` {.sourceCode .bash}
```

### Comparing `trading-backend-1.2.8/README.md` & `trading-backend-1.2.9/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# trading-backend [1.2.8](https://github.com/Drakkar-Software/trading-backend/tree/master/CHANGELOG.md)
+# trading-backend [1.2.9](https://github.com/Drakkar-Software/trading-backend/tree/master/CHANGELOG.md)
 [![PyPI](https://img.shields.io/pypi/v/trading-backend.svg)](https://pypi.python.org/pypi/trading-backend/)
 [![Downloads](https://pepy.tech/badge/trading-backend/month)](https://pepy.tech/project/trading-backend)
 [![Github-Action-CI](https://github.com/Drakkar-Software/trading-backend/workflows/trading-backend-CI/badge.svg)](https://github.com/Drakkar-Software/trading-backend/actions)
 
 - Install trading-backend from pip : 
 
 ``` {.sourceCode .bash}
```

### Comparing `trading-backend-1.2.8/setup.py` & `trading-backend-1.2.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 # from distutils.extension import Extension
 from setuptools import find_packages
 from setuptools import setup
 
-VERSION = "1.2.8"
+VERSION = "1.2.9"
 PROJECT_NAME = "trading-backend"
 
 PACKAGES = find_packages(exclude=["tests"])
 
 
 # long description from README file
 with open('README.md', encoding='utf-8') as f:
```

### Comparing `trading-backend-1.2.8/tests/exchanges/test_ascendex.py` & `trading-backend-1.2.9/tests/exchanges/test_ascendex.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.8/tests/exchanges/test_binance.py` & `trading-backend-1.2.9/tests/exchanges/test_binance.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.8/tests/exchanges/test_bitget.py` & `trading-backend-1.2.9/tests/exchanges/test_bitget.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.8/tests/exchanges/test_bybit.py` & `trading-backend-1.2.9/tests/exchanges/test_bybit.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.8/tests/exchanges/test_cryptocom.py` & `trading-backend-1.2.9/tests/exchanges/test_cryptocom.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,10 +27,10 @@
 
 @pytest.mark.asyncio
 async def test_get_orders_parameters(cryptocom_exchange):
     exchange = exchanges.CryptoCom(cryptocom_exchange)
     await create_order_tests.create_order_mocked_test_args(
         exchange,
         exchange_private_post_order_method_name="v1PrivatePostPrivateCreateOrder",
-        exchange_request_referral_key="client_oid",
-        should_contains=True
+        exchange_request_referral_key="broker_id",
+        should_contains=False
     )
```

### Comparing `trading-backend-1.2.8/tests/exchanges/test_exchange.py` & `trading-backend-1.2.9/tests/exchanges/test_exchange.py`

 * *Files 21% similar despite different names*

```diff
@@ -39,14 +39,20 @@
         fetch_balance_mock.assert_called_once()
     with mock.patch.object(exchange._exchange.connector.client, "fetch_balance",
                            mock.AsyncMock(side_effect=ccxt.AuthenticationError)) as fetch_balance_mock:
         with pytest.raises(trading_backend.errors.ExchangeAuthError):
             assert await exchange.is_valid_account() == (True, None)
         fetch_balance_mock.assert_called_once()
     with mock.patch.object(exchange._exchange.connector.client, "fetch_balance",
+                           mock.AsyncMock(side_effect=KeyError)) as fetch_balance_mock:
+        # non ccxt error: proceed to right checks and raise
+        with pytest.raises(trading_backend.errors.APIKeyPermissionsError):
+            assert await exchange.is_valid_account() == (True, None)
+        fetch_balance_mock.assert_called_once()
+    with mock.patch.object(exchange._exchange.connector.client, "fetch_balance",
                            mock.AsyncMock(side_effect=ccxt.InvalidNonce)) as fetch_balance_mock:
         with pytest.raises(trading_backend.errors.TimeSyncError):
             assert await exchange.is_valid_account() == (True, None)
         fetch_balance_mock.assert_called_once()
 
 
 @pytest.mark.asyncio
```

### Comparing `trading-backend-1.2.8/tests/exchanges/test_gateio.py` & `trading-backend-1.2.9/tests/exchanges/test_gateio.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.8/tests/exchanges/test_huobi.py` & `trading-backend-1.2.9/tests/exchanges/test_huobi.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.8/tests/exchanges/test_huobipro.py` & `trading-backend-1.2.9/tests/exchanges/test_huobipro.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.8/tests/exchanges/test_kucoin.py` & `trading-backend-1.2.9/tests/exchanges/test_kucoin.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.8/tests/exchanges/test_kucoin_futures.py` & `trading-backend-1.2.9/tests/exchanges/test_kucoin_futures.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.8/tests/exchanges/test_mexc.py` & `trading-backend-1.2.9/tests/exchanges/test_mexc.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.8/tests/exchanges/test_okx.py` & `trading-backend-1.2.9/tests/exchanges/test_okx.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.8/tests/exchanges/test_phemex.py` & `trading-backend-1.2.9/tests/exchanges/test_phemex.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.8/tests/util/__init__.py` & `trading-backend-1.2.9/tests/util/__init__.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.8/tests/util/create_order_tests.py` & `trading-backend-1.2.9/tests/util/create_order_tests.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.8/trading_backend/__init__.py` & `trading-backend-1.2.9/trading_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.8/trading_backend/constants.py` & `trading-backend-1.2.9/trading_backend/constants.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.8/trading_backend/enums.py` & `trading-backend-1.2.9/trading_backend/enums.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.8/trading_backend/errors.py` & `trading-backend-1.2.9/trading_backend/errors.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.8/trading_backend/exchange_factory.py` & `trading-backend-1.2.9/trading_backend/exchange_factory.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.8/trading_backend/exchanges/__init__.py` & `trading-backend-1.2.9/trading_backend/exchanges/__init__.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.8/trading_backend/exchanges/ascendex.py` & `trading-backend-1.2.9/trading_backend/exchanges/ascendex.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.8/trading_backend/exchanges/binance.py` & `trading-backend-1.2.9/trading_backend/exchanges/binance.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.8/trading_backend/exchanges/bitget.py` & `trading-backend-1.2.9/trading_backend/exchanges/bitget.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.8/trading_backend/exchanges/bybit.py` & `trading-backend-1.2.9/trading_backend/exchanges/bybit.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.8/trading_backend/exchanges/cryptocom.py` & `trading-backend-1.2.9/trading_backend/exchanges/cryptocom.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 import trading_backend.exchanges as exchanges
 
 
 class CryptoCom(exchanges.Exchange):
-    SPOT_ID = "OCTBT_"
-    MARGIN_ID = "OCTBT_"
-    FUTURE_ID = "OCTBT_"
+    SPOT_ID = "OCTBT"
+    MARGIN_ID = "OCTBT"
+    FUTURE_ID = "OCTBT"
     IS_SPONSORING = True
     HEADER_SPOT_KEY = "agentSource"
     HEADER_FUTURE_KEY = "Referer"
 
     @classmethod
     def get_name(cls):
         return 'cryptocom'
```

### Comparing `trading-backend-1.2.8/trading_backend/exchanges/exchange.py` & `trading-backend-1.2.9/trading_backend/exchanges/exchange.py`

 * *Files 8% similar despite different names*

```diff
@@ -70,15 +70,28 @@
             trading_backend.enums.APIKeyRights.SPOT_TRADING,
             trading_backend.enums.APIKeyRights.FUTURES_TRADING,
             trading_backend.enums.APIKeyRights.MARGIN_TRADING,
         ]
 
     async def _ensure_api_key_rights(self):
         # raise trading_backend.errors.APIKeyPermissionsError on missing permissions
-        rights = await self._get_api_key_rights()
+        rights = []
+        try:
+            rights = await self._get_api_key_rights()
+        except ccxt.BaseError:
+            raise
+        except Exception as err:
+            try:
+                import octobot_commons.logging as logging
+                logging.get_logger(self.__class__.__name__).exception(
+                    err, True, f"Error when getting {self.__class__.__name__} api key rights: {err}"
+                )
+            except ImportError:
+                pass
+            # non ccxt error: proceed to right checks and raise
         required_right = trading_backend.enums.APIKeyRights.SPOT_TRADING
         if self._exchange.exchange_manager.is_future:
             required_right = trading_backend.enums.APIKeyRights.FUTURES_TRADING
         if self._exchange.exchange_manager.is_margin:
             required_right = trading_backend.enums.APIKeyRights.MARGIN_TRADING
         if required_right not in rights:
             raise trading_backend.errors.APIKeyPermissionsError(
```

### Comparing `trading-backend-1.2.8/trading_backend/exchanges/gateio.py` & `trading-backend-1.2.9/trading_backend/exchanges/gateio.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.8/trading_backend/exchanges/huobi.py` & `trading-backend-1.2.9/trading_backend/exchanges/huobi.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.8/trading_backend/exchanges/huobipro.py` & `trading-backend-1.2.9/trading_backend/exchanges/huobipro.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.8/trading_backend/exchanges/kucoin.py` & `trading-backend-1.2.9/trading_backend/exchanges/mexc.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,36 +12,21 @@
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 import trading_backend.exchanges as exchanges
 
 
-class Kucoin(exchanges.Exchange):
-    SPOT_ID = "Octobot"
-    SPOT_PRIVATE_KEY = "0782058c-8c05-45f1-bfe1-840e2f96335a"
-    MARGIN_ID = ""
-    MARGIN_PRIVATE_KEY = ""
-    FUTURE_ID = "Octobotfutures"
-    FUTURE_PRIVATE_KEY = "018e58ef-d9ac-4c8e-9646-0afa7fa9e37c"
+class MEXC(exchanges.Exchange):
+    SPOT_ID = "OCTO"
+    MARGIN_ID = "OCTO"
+    FUTURE_ID = "OCTO"
     IS_SPONSORING = True
 
     @classmethod
     def get_name(cls):
-        return 'kucoin'
-
-    def _get_partner_details(self):
-        return {
-            'spot': {
-                'id': self.SPOT_ID,
-                'key': self.SPOT_PRIVATE_KEY,
-            },
-            'future': {
-                'id': self.FUTURE_ID,
-                'key': self.FUTURE_PRIVATE_KEY,
-            },
-        }
+        return 'mexc'
 
     def get_orders_parameters(self, params=None) -> dict:
-        if self._exchange.connector.client.options.get("partner") != self._get_partner_details():
-            self._exchange.connector.client.options["partner"] = self._get_partner_details()
+        if self._exchange.connector.client.options.get("broker", "") != self._get_id():
+            self._exchange.connector.client.options["broker"] = self._get_id()
         return super().get_orders_parameters(params)
```

### Comparing `trading-backend-1.2.8/trading_backend/exchanges/kucoinfutures.py` & `trading-backend-1.2.9/trading_backend/exchanges/kucoinfutures.py`

 * *Files identical despite different names*

### Comparing `trading-backend-1.2.8/trading_backend/exchanges/mexc.py` & `trading-backend-1.2.9/trading_backend/exchanges/phemex.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,24 +9,29 @@
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
+import aiohttp.streams
+
 import trading_backend.exchanges as exchanges
 
 
-class MEXC(exchanges.Exchange):
-    SPOT_ID = "OCTO"
-    MARGIN_ID = "OCTO"
-    FUTURE_ID = "OCTO"
+class Phemex(exchanges.Exchange):
+    SPOT_ID = "Octobot"
+    MARGIN_ID = None
+    FUTURE_ID = "Octobot"
     IS_SPONSORING = True
 
     @classmethod
     def get_name(cls):
-        return 'mexc'
+        return 'phemex'
+
+    def _get_order_custom_id(self):
+        return f"{self._get_id()}{self._exchange.connector.client.uuid16()}"
 
     def get_orders_parameters(self, params=None) -> dict:
-        if self._exchange.connector.client.options.get("broker", "") != self._get_id():
-            self._exchange.connector.client.options["broker"] = self._get_id()
+        if self._exchange.connector.client.options.get("brokerId", "") != self._get_id():
+            self._exchange.connector.client.options["brokerId"] = self._get_id()
         return super().get_orders_parameters(params)
```

### Comparing `trading-backend-1.2.8/trading_backend.egg-info/PKG-INFO` & `trading-backend-1.2.9/trading_backend.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trading-backend
-Version: 1.2.8
+Version: 1.2.9
 Summary: Trading tools
 Home-page: https://github.com/Drakkar-Software/trading-backend
 Author: Drakkar-Software
 Author-email: contact@drakkar.software
 License: LGPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
@@ -12,15 +12,15 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.8
 License-File: LICENSE
 
-# trading-backend [1.2.8](https://github.com/Drakkar-Software/trading-backend/tree/master/CHANGELOG.md)
+# trading-backend [1.2.9](https://github.com/Drakkar-Software/trading-backend/tree/master/CHANGELOG.md)
 [![PyPI](https://img.shields.io/pypi/v/trading-backend.svg)](https://pypi.python.org/pypi/trading-backend/)
 [![Downloads](https://pepy.tech/badge/trading-backend/month)](https://pepy.tech/project/trading-backend)
 [![Github-Action-CI](https://github.com/Drakkar-Software/trading-backend/workflows/trading-backend-CI/badge.svg)](https://github.com/Drakkar-Software/trading-backend/actions)
 
 - Install trading-backend from pip : 
 
 ``` {.sourceCode .bash}
```

### Comparing `trading-backend-1.2.8/trading_backend.egg-info/SOURCES.txt` & `trading-backend-1.2.9/trading_backend.egg-info/SOURCES.txt`

 * *Files identical despite different names*

