# Comparing `tmp/bitmex-ws-0.5.0.tar.gz` & `tmp/bitmex-ws-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitmex-ws-0.5.0.tar", last modified: Mon Nov  1 14:40:31 2021, max compression
+gzip compressed data, was "bitmex-ws-1.5.0.tar", last modified: Thu Mar 28 02:06:53 2024, max compression
```

## Comparing `bitmex-ws-0.5.0.tar` & `bitmex-ws-1.5.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 tbunting   (501) staff       (20)        0 2021-11-01 14:40:31.460382 bitmex-ws-0.5.0/
--rw-r--r--   0 tbunting   (501) staff       (20)     2650 2021-11-01 14:40:31.460135 bitmex-ws-0.5.0/PKG-INFO
--rw-r--r--   0 tbunting   (501) staff       (20)     2423 2021-11-01 14:22:26.000000 bitmex-ws-0.5.0/README.md
--rw-r--r--   0 tbunting   (501) staff       (20)    11150 2021-11-01 14:22:26.000000 bitmex-ws-0.5.0/bitmex_websocket.py
-drwxr-xr-x   0 tbunting   (501) staff       (20)        0 2021-11-01 14:40:31.458171 bitmex-ws-0.5.0/bitmex_ws.egg-info/
--rw-r--r--   0 tbunting   (501) staff       (20)     2650 2021-11-01 14:40:31.000000 bitmex-ws-0.5.0/bitmex_ws.egg-info/PKG-INFO
--rw-r--r--   0 tbunting   (501) staff       (20)      265 2021-11-01 14:40:31.000000 bitmex-ws-0.5.0/bitmex_ws.egg-info/SOURCES.txt
--rw-r--r--   0 tbunting   (501) staff       (20)        1 2021-11-01 14:40:31.000000 bitmex-ws-0.5.0/bitmex_ws.egg-info/dependency_links.txt
--rw-r--r--   0 tbunting   (501) staff       (20)       25 2021-11-01 14:40:31.000000 bitmex-ws-0.5.0/bitmex_ws.egg-info/requires.txt
--rw-r--r--   0 tbunting   (501) staff       (20)        6 2021-11-01 14:40:31.000000 bitmex-ws-0.5.0/bitmex_ws.egg-info/top_level.txt
--rw-r--r--   0 tbunting   (501) staff       (20)     1234 2021-11-01 14:22:26.000000 bitmex-ws-0.5.0/main.py
--rw-r--r--   0 tbunting   (501) staff       (20)       38 2021-11-01 14:40:31.460471 bitmex-ws-0.5.0/setup.cfg
--rw-r--r--   0 tbunting   (501) staff       (20)      488 2021-11-01 14:22:26.000000 bitmex-ws-0.5.0/setup.py
-drwxr-xr-x   0 tbunting   (501) staff       (20)        0 2021-11-01 14:40:31.459534 bitmex-ws-0.5.0/util/
--rw-r--r--   0 tbunting   (501) staff       (20)        0 2021-11-01 14:22:26.000000 bitmex-ws-0.5.0/util/__init__.py
--rw-r--r--   0 tbunting   (501) staff       (20)     1240 2021-11-01 14:22:26.000000 bitmex-ws-0.5.0/util/api_key.py
--rw-r--r--   0 tbunting   (501) staff       (20)      831 2021-11-01 14:22:26.000000 bitmex-ws-0.5.0/util/subscriptions.py
+drwxr-xr-x   0 shingyuen   (501) staff       (20)        0 2024-03-28 02:06:53.467181 bitmex-ws-1.5.0/
+-rw-r--r--   0 shingyuen   (501) staff       (20)     2645 2024-03-28 02:06:53.466814 bitmex-ws-1.5.0/PKG-INFO
+-rw-r--r--   0 shingyuen   (501) staff       (20)     2423 2023-02-15 07:42:07.000000 bitmex-ws-1.5.0/README.md
+-rw-r--r--   0 shingyuen   (501) staff       (20)    11184 2024-01-29 02:44:02.000000 bitmex-ws-1.5.0/bitmex_websocket.py
+drwxr-xr-x   0 shingyuen   (501) staff       (20)        0 2024-03-28 02:06:53.465816 bitmex-ws-1.5.0/bitmex_ws.egg-info/
+-rw-r--r--   0 shingyuen   (501) staff       (20)     2645 2024-03-28 02:06:53.000000 bitmex-ws-1.5.0/bitmex_ws.egg-info/PKG-INFO
+-rw-r--r--   0 shingyuen   (501) staff       (20)      265 2024-03-28 02:06:53.000000 bitmex-ws-1.5.0/bitmex_ws.egg-info/SOURCES.txt
+-rw-r--r--   0 shingyuen   (501) staff       (20)        1 2024-03-28 02:06:53.000000 bitmex-ws-1.5.0/bitmex_ws.egg-info/dependency_links.txt
+-rw-r--r--   0 shingyuen   (501) staff       (20)       24 2024-03-28 02:06:53.000000 bitmex-ws-1.5.0/bitmex_ws.egg-info/requires.txt
+-rw-r--r--   0 shingyuen   (501) staff       (20)        6 2024-03-28 02:06:53.000000 bitmex-ws-1.5.0/bitmex_ws.egg-info/top_level.txt
+-rw-r--r--   0 shingyuen   (501) staff       (20)     1234 2024-01-26 08:40:05.000000 bitmex-ws-1.5.0/main.py
+-rw-r--r--   0 shingyuen   (501) staff       (20)       38 2024-03-28 02:06:53.467244 bitmex-ws-1.5.0/setup.cfg
+-rw-r--r--   0 shingyuen   (501) staff       (20)      487 2024-01-29 02:44:02.000000 bitmex-ws-1.5.0/setup.py
+drwxr-xr-x   0 shingyuen   (501) staff       (20)        0 2024-03-28 02:06:53.464959 bitmex-ws-1.5.0/util/
+-rw-r--r--   0 shingyuen   (501) staff       (20)        0 2023-02-15 07:42:07.000000 bitmex-ws-1.5.0/util/__init__.py
+-rw-r--r--   0 shingyuen   (501) staff       (20)     1240 2023-02-15 07:42:07.000000 bitmex-ws-1.5.0/util/api_key.py
+-rw-r--r--   0 shingyuen   (501) staff       (20)      831 2023-02-15 07:42:07.000000 bitmex-ws-1.5.0/util/subscriptions.py
```

### Comparing `bitmex-ws-0.5.0/PKG-INFO` & `bitmex-ws-1.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: bitmex-ws
-Version: 0.5.0
+Version: 1.5.0
 Summary: Sample adapter for connecting to the BitMEX Websocket API.
-Home-page: UNKNOWN
+Home-page: 
 Author: Samuel Reed
 Author-email: sam@bitmex.com
-License: UNKNOWN
-Platform: UNKNOWN
+Requires-Dist: websocket-client==1.6.4
 
 # Python Adapter for BitMEX Realtime Data
 
 This is a reference adapter for receiving realtime data from the BitMEX API. See [the BitMEX documentation](https://testnet.bitmex.com/app/wsAPI)
 for more information on the websocket API.
 
 # Installation
@@ -53,9 +52,7 @@
     2018-02-01 11:51:54,364 - root - INFO - Ticker: {'last': 8947.0, 'sell': 8948.0, 'buy': 8947.0, 'mid': 8947.0}
     2018-02-01 11:51:54,369 - root - INFO - Market Depth: [{'id': 15500000950, 'side': 'Sell', 'size': 384, 'price': 999990.5, 'symbol': 'XBTUSD' ...
     2018-02-01 11:51:54,370 - root - INFO - Recent Trades: [{'side': 'Sell', 'size': 29856, 'price': 8947, 'symbol': 'XBTUSD', 'timestamp':       ...
 
 # Compatibility
 This module supports Python 3.5+.
 
-
-
```

### Comparing `bitmex-ws-0.5.0/README.md` & `bitmex-ws-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `bitmex-ws-0.5.0/bitmex_websocket.py` & `bitmex-ws-1.5.0/bitmex_websocket.py`

 * *Files 3% similar despite different names*

```diff
@@ -179,15 +179,15 @@
 
     def __send_command(self, command, args=None):
         '''Send a raw command.'''
         if args is None:
             args = []
         self.ws.send(json.dumps({"op": command, "args": args}))
 
-    def __on_message(self, message):
+    def __on_message(self, ws, message):
         '''Handler for parsing WS messages.'''
         message = json.loads(message)
         self.logger.debug(json.dumps(message))
 
         table = message.get("table")
         action = message.get("action")
         try:
@@ -236,25 +236,25 @@
                         item = find_by_keys(self.keys[table], self.data[table], deleteData)
                         self.data[table].remove(item)
                 else:
                     raise Exception("Unknown action: %s" % action)
         except:
             self.logger.error(traceback.format_exc())
 
-    def __on_error(self, error):
+    def __on_error(self, ws, error):
         '''Called on fatal websocket errors. We exit on these.'''
         if not self.exited:
             self.logger.error("Error : %s" % error)
             raise websocket.WebSocketException(error)
 
-    def __on_open(self):
+    def __on_open(self, ws):
         '''Called when the WS opens.'''
         self.logger.debug("Websocket Opened.")
 
-    def __on_close(self):
+    def __on_close(self, ws, status_code, msg):
         '''Called on websocket close.'''
         self.logger.info('Websocket Closed')
 
 
 # Utility method for finding an item in the store.
 # When an update comes through on the websocket, we need to figure out which item in the array it is
 # in order to match that item.
```

### Comparing `bitmex-ws-0.5.0/bitmex_ws.egg-info/PKG-INFO` & `bitmex-ws-1.5.0/bitmex_ws.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: bitmex-ws
-Version: 0.5.0
+Version: 1.5.0
 Summary: Sample adapter for connecting to the BitMEX Websocket API.
-Home-page: UNKNOWN
+Home-page: 
 Author: Samuel Reed
 Author-email: sam@bitmex.com
-License: UNKNOWN
-Platform: UNKNOWN
+Requires-Dist: websocket-client==1.6.4
 
 # Python Adapter for BitMEX Realtime Data
 
 This is a reference adapter for receiving realtime data from the BitMEX API. See [the BitMEX documentation](https://testnet.bitmex.com/app/wsAPI)
 for more information on the websocket API.
 
 # Installation
@@ -53,9 +52,7 @@
     2018-02-01 11:51:54,364 - root - INFO - Ticker: {'last': 8947.0, 'sell': 8948.0, 'buy': 8947.0, 'mid': 8947.0}
     2018-02-01 11:51:54,369 - root - INFO - Market Depth: [{'id': 15500000950, 'side': 'Sell', 'size': 384, 'price': 999990.5, 'symbol': 'XBTUSD' ...
     2018-02-01 11:51:54,370 - root - INFO - Recent Trades: [{'side': 'Sell', 'size': 29856, 'price': 8947, 'symbol': 'XBTUSD', 'timestamp':       ...
 
 # Compatibility
 This module supports Python 3.5+.
 
-
-
```

### Comparing `bitmex-ws-0.5.0/main.py` & `bitmex-ws-1.5.0/main.py`

 * *Files identical despite different names*

### Comparing `bitmex-ws-0.5.0/util/api_key.py` & `bitmex-ws-1.5.0/util/api_key.py`

 * *Files identical despite different names*

### Comparing `bitmex-ws-0.5.0/util/subscriptions.py` & `bitmex-ws-1.5.0/util/subscriptions.py`

 * *Files identical despite different names*

