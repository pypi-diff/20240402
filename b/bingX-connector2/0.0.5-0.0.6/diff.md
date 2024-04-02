# Comparing `tmp/bingX-connector2-0.0.5.tar.gz` & `tmp/bingX-connector2-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bingX-connector2-0.0.5.tar", last modified: Sat Mar  9 12:51:47 2024, max compression
+gzip compressed data, was "bingX-connector2-0.0.6.tar", last modified: Tue Apr  2 18:01:05 2024, max compression
```

## Comparing `bingX-connector2-0.0.5.tar` & `bingX-connector2-0.0.6.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 superadmin  (1000) superadmin  (1000)        0 2024-03-09 12:51:47.526061 bingX-connector2-0.0.5/
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)    35149 2024-03-04 13:27:08.000000 bingX-connector2-0.0.5/LICENSE
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)     6481 2024-03-09 12:51:47.526061 bingX-connector2-0.0.5/PKG-INFO
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)     5980 2024-03-09 12:46:00.000000 bingX-connector2-0.0.5/README.md
-drwxr-xr-x   0 superadmin  (1000) superadmin  (1000)        0 2024-03-09 12:51:47.522728 bingX-connector2-0.0.5/bingX/
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)       99 2024-03-04 13:27:08.000000 bingX-connector2-0.0.5/bingX/__init__.py
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)     2389 2024-03-04 13:27:08.000000 bingX-connector2-0.0.5/bingX/api.py
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)      786 2024-03-04 13:27:08.000000 bingX-connector2-0.0.5/bingX/error.py
-drwxr-xr-x   0 superadmin  (1000) superadmin  (1000)        0 2024-03-09 12:51:47.522728 bingX-connector2-0.0.5/bingX/perpetual/
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)        0 2024-03-04 13:27:08.000000 bingX-connector2-0.0.5/bingX/perpetual/__init__.py
-drwxr-xr-x   0 superadmin  (1000) superadmin  (1000)        0 2024-03-09 12:51:47.522728 bingX-connector2-0.0.5/bingX/perpetual/v1/
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)     1771 2024-03-04 13:27:08.000000 bingX-connector2-0.0.5/bingX/perpetual/v1/Perpetual.py
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)       88 2024-03-04 13:27:08.000000 bingX-connector2-0.0.5/bingX/perpetual/v1/__init__.py
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)      940 2024-03-04 13:27:08.000000 bingX-connector2-0.0.5/bingX/perpetual/v1/account.py
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)     4492 2024-03-04 13:27:08.000000 bingX-connector2-0.0.5/bingX/perpetual/v1/market.py
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)     1299 2024-03-04 13:27:08.000000 bingX-connector2-0.0.5/bingX/perpetual/v1/other.py
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)     9036 2024-03-04 13:27:08.000000 bingX-connector2-0.0.5/bingX/perpetual/v1/trade.py
-drwxr-xr-x   0 superadmin  (1000) superadmin  (1000)        0 2024-03-09 12:51:47.522728 bingX-connector2-0.0.5/bingX/perpetual/v2/
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)     1732 2024-03-04 13:41:22.000000 bingX-connector2-0.0.5/bingX/perpetual/v2/Perpetual.py
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)       88 2024-03-04 13:27:08.000000 bingX-connector2-0.0.5/bingX/perpetual/v2/__init__.py
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)     1761 2024-03-04 13:27:08.000000 bingX-connector2-0.0.5/bingX/perpetual/v2/account.py
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)     4357 2024-03-04 13:27:08.000000 bingX-connector2-0.0.5/bingX/perpetual/v2/market.py
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)     8862 2024-03-04 13:27:08.000000 bingX-connector2-0.0.5/bingX/perpetual/v2/trade.py
-drwxr-xr-x   0 superadmin  (1000) superadmin  (1000)        0 2024-03-09 12:51:47.526061 bingX-connector2-0.0.5/bingX/spot/
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)     1316 2024-03-04 13:41:10.000000 bingX-connector2-0.0.5/bingX/spot/Spot.py
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)       62 2024-03-04 13:27:08.000000 bingX-connector2-0.0.5/bingX/spot/__init__.py
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)     1412 2024-03-04 13:27:08.000000 bingX-connector2-0.0.5/bingX/spot/market.py
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)     1305 2024-03-04 13:27:08.000000 bingX-connector2-0.0.5/bingX/spot/other.py
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)     3703 2024-03-04 13:27:08.000000 bingX-connector2-0.0.5/bingX/spot/trade.py
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)     3261 2024-03-04 13:27:08.000000 bingX-connector2-0.0.5/bingX/spot/transfer.py
-drwxr-xr-x   0 superadmin  (1000) superadmin  (1000)        0 2024-03-09 12:51:47.526061 bingX-connector2-0.0.5/bingX/standard/
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)      778 2024-03-04 13:41:00.000000 bingX-connector2-0.0.5/bingX/standard/Standard.py
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)       78 2024-03-04 13:27:08.000000 bingX-connector2-0.0.5/bingX/standard/__init__.py
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)     1438 2024-03-04 13:27:08.000000 bingX-connector2-0.0.5/bingX/standard/trade.py
-drwxr-xr-x   0 superadmin  (1000) superadmin  (1000)        0 2024-03-09 12:51:47.526061 bingX-connector2-0.0.5/bingX_connector2.egg-info/
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)     6481 2024-03-09 12:51:47.000000 bingX-connector2-0.0.5/bingX_connector2.egg-info/PKG-INFO
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)      852 2024-03-09 12:51:47.000000 bingX-connector2-0.0.5/bingX_connector2.egg-info/SOURCES.txt
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)        1 2024-03-09 12:51:47.000000 bingX-connector2-0.0.5/bingX_connector2.egg-info/dependency_links.txt
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)       12 2024-03-09 12:51:47.000000 bingX-connector2-0.0.5/bingX_connector2.egg-info/top_level.txt
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)       38 2024-03-09 12:51:47.526061 bingX-connector2-0.0.5/setup.cfg
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)      853 2024-03-09 12:51:17.000000 bingX-connector2-0.0.5/setup.py
-drwxr-xr-x   0 superadmin  (1000) superadmin  (1000)        0 2024-03-09 12:51:47.526061 bingX-connector2-0.0.5/tests/
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)        0 2024-03-04 13:27:08.000000 bingX-connector2-0.0.5/tests/__init__.py
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)     1694 2024-03-04 13:27:08.000000 bingX-connector2-0.0.5/tests/test_spot.py
--rw-r--r--   0 superadmin  (1000) superadmin  (1000)      674 2024-03-04 13:27:08.000000 bingX-connector2-0.0.5/tests/test_standard.py
+drwxr-xr-x   0 superadmin  (1000) superadmin  (1000)        0 2024-04-02 18:01:05.952394 bingX-connector2-0.0.6/
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)    35149 2024-03-04 13:27:08.000000 bingX-connector2-0.0.6/LICENSE
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)     6481 2024-04-02 18:01:05.952394 bingX-connector2-0.0.6/PKG-INFO
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)     5980 2024-03-09 12:46:00.000000 bingX-connector2-0.0.6/README.md
+drwxr-xr-x   0 superadmin  (1000) superadmin  (1000)        0 2024-04-02 18:01:05.949060 bingX-connector2-0.0.6/bingX/
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)       99 2024-03-04 13:27:08.000000 bingX-connector2-0.0.6/bingX/__init__.py
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)     2389 2024-03-04 13:27:08.000000 bingX-connector2-0.0.6/bingX/api.py
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)      786 2024-03-04 13:27:08.000000 bingX-connector2-0.0.6/bingX/error.py
+drwxr-xr-x   0 superadmin  (1000) superadmin  (1000)        0 2024-04-02 18:01:05.949060 bingX-connector2-0.0.6/bingX/perpetual/
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)        0 2024-03-04 13:27:08.000000 bingX-connector2-0.0.6/bingX/perpetual/__init__.py
+drwxr-xr-x   0 superadmin  (1000) superadmin  (1000)        0 2024-04-02 18:01:05.952394 bingX-connector2-0.0.6/bingX/perpetual/v1/
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)     1771 2024-03-04 13:27:08.000000 bingX-connector2-0.0.6/bingX/perpetual/v1/Perpetual.py
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)       88 2024-03-04 13:27:08.000000 bingX-connector2-0.0.6/bingX/perpetual/v1/__init__.py
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)      940 2024-03-04 13:27:08.000000 bingX-connector2-0.0.6/bingX/perpetual/v1/account.py
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)     4492 2024-03-04 13:27:08.000000 bingX-connector2-0.0.6/bingX/perpetual/v1/market.py
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)     1299 2024-03-04 13:27:08.000000 bingX-connector2-0.0.6/bingX/perpetual/v1/other.py
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)     9036 2024-03-04 13:27:08.000000 bingX-connector2-0.0.6/bingX/perpetual/v1/trade.py
+drwxr-xr-x   0 superadmin  (1000) superadmin  (1000)        0 2024-04-02 18:01:05.952394 bingX-connector2-0.0.6/bingX/perpetual/v2/
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)     1732 2024-03-04 13:41:22.000000 bingX-connector2-0.0.6/bingX/perpetual/v2/Perpetual.py
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)       88 2024-03-04 13:27:08.000000 bingX-connector2-0.0.6/bingX/perpetual/v2/__init__.py
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)     1761 2024-03-04 13:27:08.000000 bingX-connector2-0.0.6/bingX/perpetual/v2/account.py
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)     4357 2024-03-04 13:27:08.000000 bingX-connector2-0.0.6/bingX/perpetual/v2/market.py
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)     9337 2024-04-02 17:59:26.000000 bingX-connector2-0.0.6/bingX/perpetual/v2/trade.py
+drwxr-xr-x   0 superadmin  (1000) superadmin  (1000)        0 2024-04-02 18:01:05.952394 bingX-connector2-0.0.6/bingX/spot/
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)     1316 2024-03-04 13:41:10.000000 bingX-connector2-0.0.6/bingX/spot/Spot.py
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)       62 2024-03-04 13:27:08.000000 bingX-connector2-0.0.6/bingX/spot/__init__.py
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)     1412 2024-03-04 13:27:08.000000 bingX-connector2-0.0.6/bingX/spot/market.py
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)     1305 2024-03-04 13:27:08.000000 bingX-connector2-0.0.6/bingX/spot/other.py
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)     3703 2024-03-04 13:27:08.000000 bingX-connector2-0.0.6/bingX/spot/trade.py
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)     3261 2024-03-04 13:27:08.000000 bingX-connector2-0.0.6/bingX/spot/transfer.py
+drwxr-xr-x   0 superadmin  (1000) superadmin  (1000)        0 2024-04-02 18:01:05.952394 bingX-connector2-0.0.6/bingX/standard/
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)      778 2024-03-04 13:41:00.000000 bingX-connector2-0.0.6/bingX/standard/Standard.py
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)       78 2024-03-04 13:27:08.000000 bingX-connector2-0.0.6/bingX/standard/__init__.py
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)     1438 2024-03-04 13:27:08.000000 bingX-connector2-0.0.6/bingX/standard/trade.py
+drwxr-xr-x   0 superadmin  (1000) superadmin  (1000)        0 2024-04-02 18:01:05.952394 bingX-connector2-0.0.6/bingX_connector2.egg-info/
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)     6481 2024-04-02 18:01:05.000000 bingX-connector2-0.0.6/bingX_connector2.egg-info/PKG-INFO
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)      852 2024-04-02 18:01:05.000000 bingX-connector2-0.0.6/bingX_connector2.egg-info/SOURCES.txt
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)        1 2024-04-02 18:01:05.000000 bingX-connector2-0.0.6/bingX_connector2.egg-info/dependency_links.txt
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)       12 2024-04-02 18:01:05.000000 bingX-connector2-0.0.6/bingX_connector2.egg-info/top_level.txt
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)       38 2024-04-02 18:01:05.955727 bingX-connector2-0.0.6/setup.cfg
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)      853 2024-04-02 18:00:41.000000 bingX-connector2-0.0.6/setup.py
+drwxr-xr-x   0 superadmin  (1000) superadmin  (1000)        0 2024-04-02 18:01:05.952394 bingX-connector2-0.0.6/tests/
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)        0 2024-03-04 13:27:08.000000 bingX-connector2-0.0.6/tests/__init__.py
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)     1694 2024-03-04 13:27:08.000000 bingX-connector2-0.0.6/tests/test_spot.py
+-rw-r--r--   0 superadmin  (1000) superadmin  (1000)      674 2024-03-04 13:27:08.000000 bingX-connector2-0.0.6/tests/test_standard.py
```

### Comparing `bingX-connector2-0.0.5/LICENSE` & `bingX-connector2-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `bingX-connector2-0.0.5/PKG-INFO` & `bingX-connector2-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bingX-connector2
-Version: 0.0.5
+Version: 0.0.6
 Summary: A simple connector to BingX Public API
 Home-page: https://github.com/demonarch/bingX-connector-python
 Author: Ming119
 License: GPLv3
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `bingX-connector2-0.0.5/README.md` & `bingX-connector2-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `bingX-connector2-0.0.5/bingX/api.py` & `bingX-connector2-0.0.6/bingX/api.py`

 * *Files identical despite different names*

### Comparing `bingX-connector2-0.0.5/bingX/error.py` & `bingX-connector2-0.0.6/bingX/error.py`

 * *Files identical despite different names*

### Comparing `bingX-connector2-0.0.5/bingX/perpetual/v1/Perpetual.py` & `bingX-connector2-0.0.6/bingX/perpetual/v1/Perpetual.py`

 * *Files identical despite different names*

### Comparing `bingX-connector2-0.0.5/bingX/perpetual/v1/account.py` & `bingX-connector2-0.0.6/bingX/perpetual/v1/account.py`

 * *Files identical despite different names*

### Comparing `bingX-connector2-0.0.5/bingX/perpetual/v1/market.py` & `bingX-connector2-0.0.6/bingX/perpetual/v1/market.py`

 * *Files identical despite different names*

### Comparing `bingX-connector2-0.0.5/bingX/perpetual/v1/other.py` & `bingX-connector2-0.0.6/bingX/perpetual/v1/other.py`

 * *Files identical despite different names*

### Comparing `bingX-connector2-0.0.5/bingX/perpetual/v1/trade.py` & `bingX-connector2-0.0.6/bingX/perpetual/v1/trade.py`

 * *Files identical despite different names*

### Comparing `bingX-connector2-0.0.5/bingX/perpetual/v2/Perpetual.py` & `bingX-connector2-0.0.6/bingX/perpetual/v2/Perpetual.py`

 * *Files identical despite different names*

### Comparing `bingX-connector2-0.0.5/bingX/perpetual/v2/account.py` & `bingX-connector2-0.0.6/bingX/perpetual/v2/account.py`

 * *Files identical despite different names*

### Comparing `bingX-connector2-0.0.5/bingX/perpetual/v2/market.py` & `bingX-connector2-0.0.6/bingX/perpetual/v2/market.py`

 * *Files identical despite different names*

### Comparing `bingX-connector2-0.0.5/bingX/perpetual/v2/trade.py` & `bingX-connector2-0.0.6/bingX/perpetual/v2/trade.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,17 @@
     type:         str,
     side:         str,
     positionSide: str   = None,
     price:        float = None,
     quantity:     float = None,
     stopPrice:    float = None,
     recvWindow:   int   = None,
+
+    takeProfit:   float = None,
+    stopLoss:     float = None,
 ) -> dict:
     ''' Place a New Order
     POST /openApi/swap/v2/trade/order
 
     https://bingx-api.github.io/docs/swapV2/trade-api.html#_1-trade-order
     '''
     res = self.post("/openApi/swap/v2/trade/order", params={
@@ -25,14 +28,17 @@
         "type":         type,
         "side":         side,
         "positionSide": positionSide,
         "price":        price,
         "quantity":     quantity,
         "stopPrice":    stopPrice,
         "recvWindow":   recvWindow,
+
+        "takeProfit":  "{\"type\": \"TAKE_PROFIT_MARKET\", \"stopPrice\": %TAKE_PROFIT%,\"price\": %TAKE_PROFIT%,\"workingType\":\"MARK_PRICE\"}".replace("%TAKE_PROFIT%", str(takeProfit)) if takeProfit else None,
+        "stopLoss":    "{\"type\": \"STOP_MARKET\", \"stopPrice\": %STOP_LOSS%,\"price\": %STOP_LOSS%,\"workingType\":\"MARK_PRICE\"}".replace("%STOP_LOSS%", str(stopLoss)) if stopLoss else None,
     })
 
     if 'code' in res and res['code']:
         raise ClientError(res['code'], res['msg'])
     return res['data']
 
 def bulk_order(self,
```

### Comparing `bingX-connector2-0.0.5/bingX/spot/Spot.py` & `bingX-connector2-0.0.6/bingX/spot/Spot.py`

 * *Files identical despite different names*

### Comparing `bingX-connector2-0.0.5/bingX/spot/market.py` & `bingX-connector2-0.0.6/bingX/spot/market.py`

 * *Files identical despite different names*

### Comparing `bingX-connector2-0.0.5/bingX/spot/other.py` & `bingX-connector2-0.0.6/bingX/spot/other.py`

 * *Files identical despite different names*

### Comparing `bingX-connector2-0.0.5/bingX/spot/trade.py` & `bingX-connector2-0.0.6/bingX/spot/trade.py`

 * *Files identical despite different names*

### Comparing `bingX-connector2-0.0.5/bingX/spot/transfer.py` & `bingX-connector2-0.0.6/bingX/spot/transfer.py`

 * *Files identical despite different names*

### Comparing `bingX-connector2-0.0.5/bingX/standard/Standard.py` & `bingX-connector2-0.0.6/bingX/standard/Standard.py`

 * *Files identical despite different names*

### Comparing `bingX-connector2-0.0.5/bingX/standard/trade.py` & `bingX-connector2-0.0.6/bingX/standard/trade.py`

 * *Files identical despite different names*

### Comparing `bingX-connector2-0.0.5/bingX_connector2.egg-info/PKG-INFO` & `bingX-connector2-0.0.6/bingX_connector2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bingX-connector2
-Version: 0.0.5
+Version: 0.0.6
 Summary: A simple connector to BingX Public API
 Home-page: https://github.com/demonarch/bingX-connector-python
 Author: Ming119
 License: GPLv3
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `bingX-connector2-0.0.5/bingX_connector2.egg-info/SOURCES.txt` & `bingX-connector2-0.0.6/bingX_connector2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bingX-connector2-0.0.5/setup.py` & `bingX-connector2-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 NAME = "bingX-connector2"
-VERSION = "0.0.5"
+VERSION = "0.0.6"
 AUTHOR = "Ming119"
 URL = "https://github.com/demonarch/bingX-connector-python"
 
 setuptools.setup(
     name=NAME,
     version=VERSION,
     author=AUTHOR,
```

### Comparing `bingX-connector2-0.0.5/tests/test_spot.py` & `bingX-connector2-0.0.6/tests/test_spot.py`

 * *Files identical despite different names*

### Comparing `bingX-connector2-0.0.5/tests/test_standard.py` & `bingX-connector2-0.0.6/tests/test_standard.py`

 * *Files identical despite different names*

