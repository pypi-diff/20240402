# Comparing `tmp/taas-api-client-1.1.3.tar.gz` & `tmp/taas-api-client-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taas-api-client-1.1.3.tar", last modified: Fri Feb 16 20:31:53 2024, max compression
+gzip compressed data, was "taas-api-client-1.1.4.tar", last modified: Tue Apr  2 19:56:55 2024, max compression
```

## Comparing `taas-api-client-1.1.3.tar` & `taas-api-client-1.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 yiboduan   (501) staff       (20)        0 2024-02-16 20:31:53.554667 taas-api-client-1.1.3/
--rw-r--r--   0 yiboduan   (501) staff       (20)     1069 2023-08-15 20:56:36.000000 taas-api-client-1.1.3/LICENSE
--rw-r--r--   0 yiboduan   (501) staff       (20)    11327 2024-02-16 20:31:53.554344 taas-api-client-1.1.3/PKG-INFO
--rw-r--r--   0 yiboduan   (501) staff       (20)    10780 2023-08-16 07:42:51.000000 taas-api-client-1.1.3/README.md
--rw-r--r--   0 yiboduan   (501) staff       (20)      621 2024-02-16 20:30:33.000000 taas-api-client-1.1.3/pyproject.toml
--rw-r--r--   0 yiboduan   (501) staff       (20)       38 2024-02-16 20:31:53.554719 taas-api-client-1.1.3/setup.cfg
-drwxr-xr-x   0 yiboduan   (501) staff       (20)        0 2024-02-16 20:31:53.551315 taas-api-client-1.1.3/taas_api/
--rw-r--r--   0 yiboduan   (501) staff       (20)      151 2023-08-16 07:42:51.000000 taas-api-client-1.1.3/taas_api/__init__.py
--rw-r--r--   0 yiboduan   (501) staff       (20)     2686 2024-02-16 20:17:26.000000 taas-api-client-1.1.3/taas_api/client.py
--rw-r--r--   0 yiboduan   (501) staff       (20)     4951 2024-02-16 20:21:10.000000 taas-api-client-1.1.3/taas_api/data.py
--rw-r--r--   0 yiboduan   (501) staff       (20)      189 2024-02-16 20:19:22.000000 taas-api-client-1.1.3/taas_api/enums.py
-drwxr-xr-x   0 yiboduan   (501) staff       (20)        0 2024-02-16 20:31:53.553959 taas-api-client-1.1.3/taas_api_client.egg-info/
--rw-r--r--   0 yiboduan   (501) staff       (20)    11327 2024-02-16 20:31:53.000000 taas-api-client-1.1.3/taas_api_client.egg-info/PKG-INFO
--rw-r--r--   0 yiboduan   (501) staff       (20)      281 2024-02-16 20:31:53.000000 taas-api-client-1.1.3/taas_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 yiboduan   (501) staff       (20)        1 2024-02-16 20:31:53.000000 taas-api-client-1.1.3/taas_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 yiboduan   (501) staff       (20)        9 2024-02-16 20:31:53.000000 taas-api-client-1.1.3/taas_api_client.egg-info/top_level.txt
-drwxr-xr-x   0 yiboduan   (501) staff       (20)        0 2024-02-16 20:31:53.553485 taas-api-client-1.1.3/test/
--rw-r--r--   0 yiboduan   (501) staff       (20)    11789 2024-02-16 20:17:26.000000 taas-api-client-1.1.3/test/test_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:56:55.149276 taas-api-client-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-02 19:56:43.000000 taas-api-client-1.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12232 2024-04-02 19:56:55.149276 taas-api-client-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11685 2024-04-02 19:56:43.000000 taas-api-client-1.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-02 19:56:43.000000 taas-api-client-1.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 19:56:55.149276 taas-api-client-1.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:56:55.145276 taas-api-client-1.1.4/taas_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-02 19:56:43.000000 taas-api-client-1.1.4/taas_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-04-02 19:56:43.000000 taas-api-client-1.1.4/taas_api/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-04-02 19:56:43.000000 taas-api-client-1.1.4/taas_api/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-02 19:56:43.000000 taas-api-client-1.1.4/taas_api/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:56:55.145276 taas-api-client-1.1.4/taas_api_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12232 2024-04-02 19:56:55.000000 taas-api-client-1.1.4/taas_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-02 19:56:55.000000 taas-api-client-1.1.4/taas_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 19:56:55.000000 taas-api-client-1.1.4/taas_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-02 19:56:55.000000 taas-api-client-1.1.4/taas_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:56:55.145276 taas-api-client-1.1.4/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    13492 2024-04-02 19:56:43.000000 taas-api-client-1.1.4/test/test_data.py
```

### Comparing `taas-api-client-1.1.3/LICENSE` & `taas-api-client-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `taas-api-client-1.1.3/PKG-INFO` & `taas-api-client-1.1.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: taas-api-client
-Version: 1.1.3
-Summary: API client to interact with the TAAS web API
-Author-email: Tread Labs <ops@tread.fi>
-Project-URL: Homepage, https://github.com/tread-labs-public/taas-api-client
-Project-URL: Bug Tracker, https://github.com/tread-labs-public/taas-api-client/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <img width="1037" alt="TreadLabs_logo_light@2x" src="https://uploads-ssl.webflow.com/631952c105a64138b98a5339/64af023765b5d70df562e05f_TreadLabs_logo_light.svg">
 
 # TaaS Python Client
 
 ## Overview
 These APIs provide a comprehensive interface to interact with a trading platform, allowing users to manage orders, view account balances, and execute various trading strategies. The endpoints are designed to facilitate the creation, retrieval, and deletion of orders, as well as the querying of account balances.
 
@@ -34,31 +20,35 @@
 c = Client(url="http://localhost:8000", auth_token="b72ab3bcbce4423208a07f52b5aed207d5bd053e")
 ```
 
 ### Placing Orders
 
 Submits a new order with specified parameters such as accounts, trading pair, side (buy/sell), sell token amount, duration, strategy, and engine passiveness. The place order endpoint has many fields with many restrictions. To simplify the call and run validations against the parameters, we provide a data object: `PlaceOrderRequest`. Every field can be interacted with like a regular attribute in Python.
 
-| Field               | Description                                                                                       |
-|---------------------|---------------------------------------------------------------------------------------------------|
-| accounts            | A list of account names to be available for the order.                                      |
-| pair                | The trading pair for the order, following the syntax 'BASE-QUOTE' or 'BASE:VARIANT-QUOTE'.    |
-| side                | The side of the order, indicating whether it's a buy or sell ('buy' or 'sell').                |
-| duration            | The duration of the order in seconds.                                                          |
-| strategy            | The chosen trading strategy for the order (e.g. TWAP, VWAP, etc)                                |
-| sell_token_amount   | The amount of the sell token to be used in the order, if applicable.                            |
-| base_asset_qty      | The quantity of the base asset (token being bought) in the order, if applicable.                |
-| quote_asset_qty     | The quantity of the quote asset (token being sold) in the order, if applicable.                 |
-| engine_passiveness  | The engine passiveness parameter of the order, within the range [0, 0.1], 0.02 is default.         |
-| schedule_discretion | The schedule discretion parameter of the order, within the range [0, 0.1], 0.1 is default.        |
-| limit_price         | The limit price that limits all the placements in the order, if applicable.                     |
-| strategy_params     | Additional parameters specific to the chosen trading strategy, provided as a dictionary.        |
-| notes               | Any additional notes or comments related to the order.                                          |
-| custom_order_id     | A custom identifier for the order, if provided.                                                |
-| updated_leverage    | An updated leverage value for the order, if applicable. This will persist on the exchange for the pair.   |
+| Field               | Description                                                                                                        |
+|---------------------|--------------------------------------------------------------------------------------------------------------------|
+| accounts            | A list of account names to be available for the order.                                                             |
+| pair                | The trading pair for the order, following the syntax 'BASE-QUOTE' or 'BASE:VARIANT-QUOTE'.                         |
+| side                | The side of the order, indicating whether it's a buy or sell ('buy' or 'sell').                                    |
+| duration            | The duration of the order in seconds.                                                                              |
+| strategy            | The chosen trading strategy for the order (e.g. TWAP, VWAP, etc)                                                   |
+| sell_token_amount   | The amount of the sell token to be used in the order, if applicable.                                               |
+| base_asset_qty      | The quantity of the base asset (token being bought) in the order, if applicable.                                   |
+| quote_asset_qty     | The quantity of the quote asset (token being sold) in the order, if applicable.                                    |
+| engine_passiveness  | The engine passiveness parameter of the order, within the range [0, 0.1], default is 0.02.                         |
+| schedule_discretion | The schedule discretion parameter of the order, within the range [0, 0.1], default is 0.08.                        |
+| alpha_tilt          | The alpha tilt parameter of the order, within the range [-1, 1], 0 is default.                                     |
+| pov_target          | The pov target parameter of the order, within the range (0, 1], default is None. Limited to non-multi orders.      |
+| pov_limit           | The pov limit parameter of the order, within the range (0, 1], default is None. Limited to non-multi orders.       |
+| exposure_tolerance  | The exposure tolerance parameter of the order, within the range [0.1, 1], 0.5 is default. Limited to multi orders. |
+| limit_price         | The limit price that limits all the placements in the order, if applicable.                                        |
+| strategy_params     | Additional parameters specific to the chosen trading strategy, provided as a dictionary.                           |
+| notes               | Any additional notes or comments related to the order.                                                             |
+| custom_order_id     | A custom identifier for the order, if provided.                                                                    |
+| updated_leverage    | An updated leverage value for the order, if applicable. This will persist on the exchange for the pair.            |
 
 Please note that the provided validation heuristics are designed to ensure that the inputs meet certain criteria before proceeding with order placement.
 [For more details on the order APIs](https://tread-labs.gitbook.io/api-docs/interacting-with-the-api/api-reference/orders)
 
 #### Example
 
 ```
@@ -109,25 +99,26 @@
 ```
 from taas_api import ChildOrder, PlaceMultiOrderRequest
 
 request = PlaceMultiOrderRequest(
     accounts=["mock"],
     duration=200,
     strategy="TWAP",
+    exposure_tolerance=0.5,
     child_orders=[
         ChildOrder(
             pair="ETH:PERP-USDT",
             side="sell",
             base_asset_qty="10"
-        ,
+        ),
         ChildOrder(
             pair="ETH-USDT",
             side="buy",
             base_asset_qty="10"
-        ),
+        )
     ]
 )
 
 res = c.place_multi_order(request)
 ```
 
 #### Response
```

### Comparing `taas-api-client-1.1.3/README.md` & `taas-api-client-1.1.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: taas-api-client
+Version: 1.1.4
+Summary: API client to interact with the TAAS web API
+Author-email: Tread Labs <ops@tread.fi>
+Project-URL: Homepage, https://github.com/tread-labs-public/taas-api-client
+Project-URL: Bug Tracker, https://github.com/tread-labs-public/taas-api-client/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <img width="1037" alt="TreadLabs_logo_light@2x" src="https://uploads-ssl.webflow.com/631952c105a64138b98a5339/64af023765b5d70df562e05f_TreadLabs_logo_light.svg">
 
 # TaaS Python Client
 
 ## Overview
 These APIs provide a comprehensive interface to interact with a trading platform, allowing users to manage orders, view account balances, and execute various trading strategies. The endpoints are designed to facilitate the creation, retrieval, and deletion of orders, as well as the querying of account balances.
 
@@ -20,31 +34,35 @@
 c = Client(url="http://localhost:8000", auth_token="b72ab3bcbce4423208a07f52b5aed207d5bd053e")
 ```
 
 ### Placing Orders
 
 Submits a new order with specified parameters such as accounts, trading pair, side (buy/sell), sell token amount, duration, strategy, and engine passiveness. The place order endpoint has many fields with many restrictions. To simplify the call and run validations against the parameters, we provide a data object: `PlaceOrderRequest`. Every field can be interacted with like a regular attribute in Python.
 
-| Field               | Description                                                                                       |
-|---------------------|---------------------------------------------------------------------------------------------------|
-| accounts            | A list of account names to be available for the order.                                      |
-| pair                | The trading pair for the order, following the syntax 'BASE-QUOTE' or 'BASE:VARIANT-QUOTE'.    |
-| side                | The side of the order, indicating whether it's a buy or sell ('buy' or 'sell').                |
-| duration            | The duration of the order in seconds.                                                          |
-| strategy            | The chosen trading strategy for the order (e.g. TWAP, VWAP, etc)                                |
-| sell_token_amount   | The amount of the sell token to be used in the order, if applicable.                            |
-| base_asset_qty      | The quantity of the base asset (token being bought) in the order, if applicable.                |
-| quote_asset_qty     | The quantity of the quote asset (token being sold) in the order, if applicable.                 |
-| engine_passiveness  | The engine passiveness parameter of the order, within the range [0, 0.1], 0.02 is default.         |
-| schedule_discretion | The schedule discretion parameter of the order, within the range [0, 0.1], 0.1 is default.        |
-| limit_price         | The limit price that limits all the placements in the order, if applicable.                     |
-| strategy_params     | Additional parameters specific to the chosen trading strategy, provided as a dictionary.        |
-| notes               | Any additional notes or comments related to the order.                                          |
-| custom_order_id     | A custom identifier for the order, if provided.                                                |
-| updated_leverage    | An updated leverage value for the order, if applicable. This will persist on the exchange for the pair.   |
+| Field               | Description                                                                                                        |
+|---------------------|--------------------------------------------------------------------------------------------------------------------|
+| accounts            | A list of account names to be available for the order.                                                             |
+| pair                | The trading pair for the order, following the syntax 'BASE-QUOTE' or 'BASE:VARIANT-QUOTE'.                         |
+| side                | The side of the order, indicating whether it's a buy or sell ('buy' or 'sell').                                    |
+| duration            | The duration of the order in seconds.                                                                              |
+| strategy            | The chosen trading strategy for the order (e.g. TWAP, VWAP, etc)                                                   |
+| sell_token_amount   | The amount of the sell token to be used in the order, if applicable.                                               |
+| base_asset_qty      | The quantity of the base asset (token being bought) in the order, if applicable.                                   |
+| quote_asset_qty     | The quantity of the quote asset (token being sold) in the order, if applicable.                                    |
+| engine_passiveness  | The engine passiveness parameter of the order, within the range [0, 0.1], default is 0.02.                         |
+| schedule_discretion | The schedule discretion parameter of the order, within the range [0, 0.1], default is 0.08.                        |
+| alpha_tilt          | The alpha tilt parameter of the order, within the range [-1, 1], 0 is default.                                     |
+| pov_target          | The pov target parameter of the order, within the range (0, 1], default is None. Limited to non-multi orders.      |
+| pov_limit           | The pov limit parameter of the order, within the range (0, 1], default is None. Limited to non-multi orders.       |
+| exposure_tolerance  | The exposure tolerance parameter of the order, within the range [0.1, 1], 0.5 is default. Limited to multi orders. |
+| limit_price         | The limit price that limits all the placements in the order, if applicable.                                        |
+| strategy_params     | Additional parameters specific to the chosen trading strategy, provided as a dictionary.                           |
+| notes               | Any additional notes or comments related to the order.                                                             |
+| custom_order_id     | A custom identifier for the order, if provided.                                                                    |
+| updated_leverage    | An updated leverage value for the order, if applicable. This will persist on the exchange for the pair.            |
 
 Please note that the provided validation heuristics are designed to ensure that the inputs meet certain criteria before proceeding with order placement.
 [For more details on the order APIs](https://tread-labs.gitbook.io/api-docs/interacting-with-the-api/api-reference/orders)
 
 #### Example
 
 ```
@@ -95,25 +113,26 @@
 ```
 from taas_api import ChildOrder, PlaceMultiOrderRequest
 
 request = PlaceMultiOrderRequest(
     accounts=["mock"],
     duration=200,
     strategy="TWAP",
+    exposure_tolerance=0.5,
     child_orders=[
         ChildOrder(
             pair="ETH:PERP-USDT",
             side="sell",
             base_asset_qty="10"
-        ,
+        ),
         ChildOrder(
             pair="ETH-USDT",
             side="buy",
             base_asset_qty="10"
-        ),
+        )
     ]
 )
 
 res = c.place_multi_order(request)
 ```
 
 #### Response
```

### Comparing `taas-api-client-1.1.3/pyproject.toml` & `taas-api-client-1.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "taas-api-client"
-version = "1.1.3"
+version = "1.1.4"
 authors = [
   { name="Tread Labs", email="ops@tread.fi" },
 ]
 description = "API client to interact with the TAAS web API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `taas-api-client-1.1.3/taas_api/client.py` & `taas-api-client-1.1.4/taas_api/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -66,14 +66,17 @@
 
         validate_success, errors = request.validate()
 
         if not validate_success:
             raise ValueError(str(errors))
         return self.post(path=f"/api/multi_orders/", data=request.to_post_body())
 
+    def cancel_multi_order(self, order_id):
+        return self.delete(path=f"/api/multi_order/{order_id}")
+
     def place_order(self, request: data.PlaceOrderRequest):
         if not isinstance(request, data.PlaceOrderRequest):
             raise ValueError(f"Expecting request to be of type {data.PlaceOrderRequest}")
 
         validate_success, error = request.validate()
 
         if not validate_success:
```

### Comparing `taas-api-client-1.1.3/taas_api/data.py` & `taas-api-client-1.1.4/taas_api/data.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 from dataclasses import dataclass, asdict
-from typing import List, Union
+from typing import List
 from taas_api.enums import Strategy, Side
 import re
 
 INTERNAL_PAIR_RE_PATTERN = r"([a-zA-Z0-9]+)(:\w+)?-([a-zA-Z0-9]+)"
 
+
 @dataclass
 class PlaceOrderRequest:
     accounts: List[str]
     pair: str
     side: str
     duration: int
     strategy: str
-    sell_token_amount: Union[int, float, str] = None
-    base_asset_qty: Union[int, float, str] = None
-    quote_asset_qty: Union[int, float, str] = None
+    sell_token_amount: float = None
+    base_asset_qty: float = None
+    quote_asset_qty: float = None
     engine_passiveness: float = None
     schedule_discretion: float = None
+    alpha_tilt: float = None
     order_condition: str = None
     order_condition_expiry: str = None
-    limit_price: Union[int, float, str] = None
+    pov_limit: float = None
+    pov_target: float = None
+    limit_price: float = None
     strategy_params: dict = None
     notes: str = None
     custom_order_id: str = None
     updated_leverage: int = None
 
     def validate(self):
         try:
@@ -49,34 +53,47 @@
             if not (0 <= self.engine_passiveness <= 1):
                 return False, "engine_passiveness out of range, must be [0,1]"
 
         if self.schedule_discretion is not None:
             if not (0 <= self.schedule_discretion <= 1):
                 return False, "schedule_discretion out of range, must be [0,1]"
 
+        if self.alpha_tilt is not None:
+            if not (-1 <= self.alpha_tilt <= 1):
+                return False, "alpha_tilt out of range, must be [-1,1]"
+
+        if self.pov_limit is not None:
+            if not (0 < self.pov_limit <= 1):
+                return False, "pov_limit is a ratio within (0,1]"
+
+        if self.pov_target is not None:
+            if not (0 < self.pov_target <= 1):
+                return False, "pov_target is a ratio within (0,1]"
+
         valid_strategy_params = ["passive_only", "reduce_only"]
 
         if self.strategy_params is not None:
             if not isinstance(self.strategy_params, dict):
                 return False, "strategy_params must be a dict"
 
             if any([key not in valid_strategy_params for key in self.strategy_params.keys()]):
                 return False, f"must use valid strategy_params: {valid_strategy_params}"
 
         return True, None
 
     def to_post_body(self):
         return {k: v for k, v in asdict(self).items() if v is not None}
 
+
 @dataclass
 class ChildOrder:
     pair: str
     side: str
-    base_asset_qty: Union[int, float, str] = None
-    quote_asset_qty: Union[int, float, str] = None
+    base_asset_qty: float = None
+    quote_asset_qty: float = None
 
     def validate(self):
         try:
             Side(self.side)
         except ValueError:
             return False, "side must be 'buy' or 'sell'"
 
@@ -92,14 +109,15 @@
 class PlaceMultiOrderRequest:
     accounts: List[str]
     duration: int
     strategy: str
     child_orders: List[ChildOrder]
     engine_passiveness: float = None
     schedule_discretion: float = None
+    alpha_tilt: float = None
     order_condition: str = None
     order_condition_expiry: str = None
     strategy_params: dict = None
     exposure_tolerance: float = None
 
     def validate(self):
         if len(self.child_orders) == 0:
@@ -114,17 +132,21 @@
             if not (0 <= self.engine_passiveness <= 1):
                 return False, ["engine_passiveness out of range, must be [0,1]"]
 
         if self.schedule_discretion is not None:
             if not (0 <= self.schedule_discretion <= 1):
                 return False, ["schedule_discretion out of range, must be [0,1]"]
 
+        if self.alpha_tilt is not None:
+            if not (-1 <= self.alpha_tilt <= 1):
+                return False, ["alpha_tilt out of range, must be [-1,1]"]
+
         if self.exposure_tolerance is not None:
             if not (0.1 <= self.exposure_tolerance <= 1):
-                return False, ["schedule_discretion out of range, must be [0.1,1]"]
+                return False, ["exposure_tolerance out of range, must be [0.1,1]"]
 
         valid_strategy_params = ["passive_only", "reduce_only"]
 
         if self.strategy_params is not None:
             if not isinstance(self.strategy_params, dict):
                 return False, ["strategy_params must be a dict"]
```

### Comparing `taas-api-client-1.1.3/taas_api_client.egg-info/PKG-INFO` & `taas-api-client-1.1.4/taas_api_client.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taas-api-client
-Version: 1.1.3
+Version: 1.1.4
 Summary: API client to interact with the TAAS web API
 Author-email: Tread Labs <ops@tread.fi>
 Project-URL: Homepage, https://github.com/tread-labs-public/taas-api-client
 Project-URL: Bug Tracker, https://github.com/tread-labs-public/taas-api-client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -34,31 +34,35 @@
 c = Client(url="http://localhost:8000", auth_token="b72ab3bcbce4423208a07f52b5aed207d5bd053e")
 ```
 
 ### Placing Orders
 
 Submits a new order with specified parameters such as accounts, trading pair, side (buy/sell), sell token amount, duration, strategy, and engine passiveness. The place order endpoint has many fields with many restrictions. To simplify the call and run validations against the parameters, we provide a data object: `PlaceOrderRequest`. Every field can be interacted with like a regular attribute in Python.
 
-| Field               | Description                                                                                       |
-|---------------------|---------------------------------------------------------------------------------------------------|
-| accounts            | A list of account names to be available for the order.                                      |
-| pair                | The trading pair for the order, following the syntax 'BASE-QUOTE' or 'BASE:VARIANT-QUOTE'.    |
-| side                | The side of the order, indicating whether it's a buy or sell ('buy' or 'sell').                |
-| duration            | The duration of the order in seconds.                                                          |
-| strategy            | The chosen trading strategy for the order (e.g. TWAP, VWAP, etc)                                |
-| sell_token_amount   | The amount of the sell token to be used in the order, if applicable.                            |
-| base_asset_qty      | The quantity of the base asset (token being bought) in the order, if applicable.                |
-| quote_asset_qty     | The quantity of the quote asset (token being sold) in the order, if applicable.                 |
-| engine_passiveness  | The engine passiveness parameter of the order, within the range [0, 0.1], 0.02 is default.         |
-| schedule_discretion | The schedule discretion parameter of the order, within the range [0, 0.1], 0.1 is default.        |
-| limit_price         | The limit price that limits all the placements in the order, if applicable.                     |
-| strategy_params     | Additional parameters specific to the chosen trading strategy, provided as a dictionary.        |
-| notes               | Any additional notes or comments related to the order.                                          |
-| custom_order_id     | A custom identifier for the order, if provided.                                                |
-| updated_leverage    | An updated leverage value for the order, if applicable. This will persist on the exchange for the pair.   |
+| Field               | Description                                                                                                        |
+|---------------------|--------------------------------------------------------------------------------------------------------------------|
+| accounts            | A list of account names to be available for the order.                                                             |
+| pair                | The trading pair for the order, following the syntax 'BASE-QUOTE' or 'BASE:VARIANT-QUOTE'.                         |
+| side                | The side of the order, indicating whether it's a buy or sell ('buy' or 'sell').                                    |
+| duration            | The duration of the order in seconds.                                                                              |
+| strategy            | The chosen trading strategy for the order (e.g. TWAP, VWAP, etc)                                                   |
+| sell_token_amount   | The amount of the sell token to be used in the order, if applicable.                                               |
+| base_asset_qty      | The quantity of the base asset (token being bought) in the order, if applicable.                                   |
+| quote_asset_qty     | The quantity of the quote asset (token being sold) in the order, if applicable.                                    |
+| engine_passiveness  | The engine passiveness parameter of the order, within the range [0, 0.1], default is 0.02.                         |
+| schedule_discretion | The schedule discretion parameter of the order, within the range [0, 0.1], default is 0.08.                        |
+| alpha_tilt          | The alpha tilt parameter of the order, within the range [-1, 1], 0 is default.                                     |
+| pov_target          | The pov target parameter of the order, within the range (0, 1], default is None. Limited to non-multi orders.      |
+| pov_limit           | The pov limit parameter of the order, within the range (0, 1], default is None. Limited to non-multi orders.       |
+| exposure_tolerance  | The exposure tolerance parameter of the order, within the range [0.1, 1], 0.5 is default. Limited to multi orders. |
+| limit_price         | The limit price that limits all the placements in the order, if applicable.                                        |
+| strategy_params     | Additional parameters specific to the chosen trading strategy, provided as a dictionary.                           |
+| notes               | Any additional notes or comments related to the order.                                                             |
+| custom_order_id     | A custom identifier for the order, if provided.                                                                    |
+| updated_leverage    | An updated leverage value for the order, if applicable. This will persist on the exchange for the pair.            |
 
 Please note that the provided validation heuristics are designed to ensure that the inputs meet certain criteria before proceeding with order placement.
 [For more details on the order APIs](https://tread-labs.gitbook.io/api-docs/interacting-with-the-api/api-reference/orders)
 
 #### Example
 
 ```
@@ -109,25 +113,26 @@
 ```
 from taas_api import ChildOrder, PlaceMultiOrderRequest
 
 request = PlaceMultiOrderRequest(
     accounts=["mock"],
     duration=200,
     strategy="TWAP",
+    exposure_tolerance=0.5,
     child_orders=[
         ChildOrder(
             pair="ETH:PERP-USDT",
             side="sell",
             base_asset_qty="10"
-        ,
+        ),
         ChildOrder(
             pair="ETH-USDT",
             side="buy",
             base_asset_qty="10"
-        ),
+        )
     ]
 )
 
 res = c.place_multi_order(request)
 ```
 
 #### Response
```

### Comparing `taas-api-client-1.1.3/test/test_data.py` & `taas-api-client-1.1.4/test/test_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
     def test_validate_success_all_fields(self):
         order_request = self._build_order_request(
             base_asset_qty=None,
             quote_asset_qty=20000.0,
             engine_passiveness=0.2,
             schedule_discretion=0.08,
+            alpha_tilt=0.5,
             limit_price=1800.1,
             strategy_params={"reduce_only": True},
             notes="wow!!!",
             custom_order_id="abcd-efgh",
         )
         success, error = order_request.validate()
 
@@ -101,44 +102,76 @@
 
         order_request = self._build_order_request(strategy_params={"asdf": 1})
         success, error = order_request.validate()
 
         self.assertFalse(success)
         self.assertTrue("strategy_params" in error)
 
+    def test_validate_fail_bad_pov_limit(self):
+        order_request = self._build_order_request(pov_limit=0)
+        success, error = order_request.validate()
+
+        self.assertFalse(success)
+        self.assertTrue("pov_limit" in error)
+
+        order_request = self._build_order_request(pov_limit=1.1)
+        success, error = order_request.validate()
+
+        self.assertFalse(success)
+        self.assertTrue("pov_limit" in error)
+
+    def test_validate_fail_bad_pov_limit(self):
+        order_request = self._build_order_request(pov_target=0)
+        success, error = order_request.validate()
+
+        self.assertFalse(success)
+        self.assertTrue("pov_target" in error)
+
+        order_request = self._build_order_request(pov_target=1.1)
+        success, error = order_request.validate()
+
+        self.assertFalse(success)
+        self.assertTrue("pov_target" in error)
+
     def test_to_post_body(self):
         order_request = self._build_order_request(
             base_asset_qty=None,
             quote_asset_qty=20000.0,
             engine_passiveness=0.2,
             schedule_discretion=0.08,
+            alpha_tilt=0.5,
             limit_price=1800.1,
             strategy_params={"reduce_only": True},
             notes="wow!!!",
             custom_order_id="abcd-efgh",
             updated_leverage=10,
+            pov_limit=3.2,
+            pov_target=2.1,
         )
 
         post_body = order_request.to_post_body()
 
         self.assertEqual(["mock"], post_body["accounts"])
         self.assertEqual("ETH-USDT", post_body["pair"])
         self.assertEqual("buy", post_body["side"])
         self.assertEqual(300, post_body["duration"])
         self.assertEqual("TWAP", post_body["strategy"])
         self.assertFalse("base_asset_qty" in post_body)
         self.assertFalse("sell_token_amount" in post_body)
         self.assertEqual(20000, post_body["quote_asset_qty"])
         self.assertEqual(0.2, post_body["engine_passiveness"])
         self.assertEqual(0.08, post_body["schedule_discretion"])
+        self.assertEqual(0.5, post_body["alpha_tilt"])
         self.assertEqual(1800.1, post_body["limit_price"])
         self.assertEqual({"reduce_only": True}, post_body["strategy_params"])
         self.assertEqual("wow!!!", post_body["notes"])
         self.assertEqual("abcd-efgh", post_body["custom_order_id"])
         self.assertEqual(10, post_body["updated_leverage"])
+        self.assertEqual(3.2, post_body["pov_limit"])
+        self.assertEqual(2.1, post_body["pov_target"])
 
 class PlaceMultiOrderRequestTest(TestCase):
     def _build_multi_order_request(self, **kwargs):
         params = {
             "accounts": ["mock"],
             "duration": 300,
             "strategy": "TWAP",
@@ -240,14 +273,28 @@
         ]
         multi_order = self._build_multi_order_request(schedule_discretion=-1, child_orders=child_orders)
 
         success, errors = multi_order.validate()
         self.assertEqual(False, success)
         self.assertTrue("schedule_discretion" in errors[0])
 
+    def test_validate_fail_bad_alpha_tilt(self):
+        child_orders = [
+            ChildOrder(
+                pair="ETH:PERP-USDT",
+                side="sell",
+                base_asset_qty="10",
+            ),
+        ]
+        multi_order = self._build_multi_order_request(alpha_tilt=-2, child_orders=child_orders)
+
+        success, errors = multi_order.validate()
+        self.assertEqual(False, success)
+        self.assertTrue("alpha_tilt" in errors[0])
+
     def test_validate_fail_bad_strategy_params(self):
         child_orders = [
             ChildOrder(
                 pair="ETH:PERP-USDT",
                 side="sell",
                 base_asset_qty="10",
             ),
@@ -289,26 +336,28 @@
         multi_order = self._build_multi_order_request(
             strategy="VWAP",
             duration=180,
             accounts=["abc"],
             strategy_params={"passive_only": True},
             engine_passiveness=0.1,
             schedule_discretion=0.2,
-            exposure_tolerance=0.3,
+            alpha_tilt=0.3,
+            exposure_tolerance=0.4,
             child_orders=child_orders,
         )
         body = multi_order.to_post_body()
 
         self.assertEqual("VWAP", body["strategy"])
         self.assertEqual(180, body["duration"])
         self.assertEqual(["abc"], body["accounts"])
         self.assertEqual({"passive_only": True}, body["strategy_params"])
         self.assertEqual(0.1, body["engine_passiveness"])
         self.assertEqual(0.2, body["schedule_discretion"])
-        self.assertEqual(0.3, body["exposure_tolerance"])
+        self.assertEqual(0.3, body["alpha_tilt"])
+        self.assertEqual(0.4, body["exposure_tolerance"])
         self.assertEqual("ETH:PERP-USDT", body["child_orders"][0]["pair"])
         self.assertEqual("sell", body["child_orders"][0]["side"])
         self.assertEqual("10", body["child_orders"][0]["base_asset_qty"])
         self.assertEqual("ETH-USDT", body["child_orders"][1]["pair"])
         self.assertEqual("buy", body["child_orders"][1]["side"])
         self.assertEqual("10", body["child_orders"][1]["base_asset_qty"])
```

