# Comparing `tmp/vcx_py-1.1.3.tar.gz` & `tmp/vcx_py-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vcx_py-1.1.3.tar", last modified: Mon Apr  1 13:30:34 2024, max compression
+gzip compressed data, was "vcx_py-1.1.4.tar", last modified: Tue Apr  2 17:15:30 2024, max compression
```

## Comparing `vcx_py-1.1.3.tar` & `vcx_py-1.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 aarjaneiro  (1000) aarjaneiro  (1000)        0 2024-04-01 13:30:34.730030 vcx_py-1.1.3/
--rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)     1075 2024-03-15 22:12:30.000000 vcx_py-1.1.3/LICENSE
--rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)     4227 2024-04-01 13:30:34.730030 vcx_py-1.1.3/PKG-INFO
--rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)     3936 2024-03-22 20:52:38.000000 vcx_py-1.1.3/README.md
--rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)       38 2024-04-01 13:30:34.730030 vcx_py-1.1.3/setup.cfg
--rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)      931 2024-04-01 13:29:59.000000 vcx_py-1.1.3/setup.py
-drwxr-xr-x   0 aarjaneiro  (1000) aarjaneiro  (1000)        0 2024-04-01 13:30:34.730030 vcx_py-1.1.3/vcx_py/
--rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)      792 2024-03-18 23:09:16.000000 vcx_py-1.1.3/vcx_py/__init__.py
--rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)     9862 2024-04-01 13:29:48.000000 vcx_py-1.1.3/vcx_py/client.py
--rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)     2365 2024-03-21 19:20:57.000000 vcx_py-1.1.3/vcx_py/constants.py
--rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)     1695 2024-03-22 19:04:00.000000 vcx_py-1.1.3/vcx_py/schema.py
--rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)     3065 2024-03-28 19:39:06.000000 vcx_py-1.1.3/vcx_py/utils.py
-drwxr-xr-x   0 aarjaneiro  (1000) aarjaneiro  (1000)        0 2024-04-01 13:30:34.730030 vcx_py-1.1.3/vcx_py.egg-info/
--rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)     4227 2024-04-01 13:30:34.000000 vcx_py-1.1.3/vcx_py.egg-info/PKG-INFO
--rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)      235 2024-04-01 13:30:34.000000 vcx_py-1.1.3/vcx_py.egg-info/SOURCES.txt
--rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)        1 2024-04-01 13:30:34.000000 vcx_py-1.1.3/vcx_py.egg-info/dependency_links.txt
--rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)        7 2024-04-01 13:30:34.000000 vcx_py-1.1.3/vcx_py.egg-info/top_level.txt
+drwxr-xr-x   0 aarjaneiro  (1000) aarjaneiro  (1000)        0 2024-04-02 17:15:30.152453 vcx_py-1.1.4/
+-rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)     1075 2024-03-15 22:12:30.000000 vcx_py-1.1.4/LICENSE
+-rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)     4626 2024-04-02 17:15:30.152453 vcx_py-1.1.4/PKG-INFO
+-rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)     4336 2024-04-01 14:03:55.000000 vcx_py-1.1.4/README.md
+-rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)       38 2024-04-02 17:15:30.152453 vcx_py-1.1.4/setup.cfg
+-rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)      931 2024-04-02 17:15:27.000000 vcx_py-1.1.4/setup.py
+drwxr-xr-x   0 aarjaneiro  (1000) aarjaneiro  (1000)        0 2024-04-02 17:15:30.152453 vcx_py-1.1.4/vcx_py/
+-rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)      792 2024-03-18 23:09:16.000000 vcx_py-1.1.4/vcx_py/__init__.py
+-rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)    10366 2024-04-02 17:15:09.000000 vcx_py-1.1.4/vcx_py/client.py
+-rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)     2365 2024-03-21 19:20:57.000000 vcx_py-1.1.4/vcx_py/constants.py
+-rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)     1695 2024-03-22 19:04:00.000000 vcx_py-1.1.4/vcx_py/schema.py
+-rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)     3065 2024-03-28 19:39:06.000000 vcx_py-1.1.4/vcx_py/utils.py
+drwxr-xr-x   0 aarjaneiro  (1000) aarjaneiro  (1000)        0 2024-04-02 17:15:30.152453 vcx_py-1.1.4/vcx_py.egg-info/
+-rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)     4626 2024-04-02 17:15:30.000000 vcx_py-1.1.4/vcx_py.egg-info/PKG-INFO
+-rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)      235 2024-04-02 17:15:30.000000 vcx_py-1.1.4/vcx_py.egg-info/SOURCES.txt
+-rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)        1 2024-04-02 17:15:30.000000 vcx_py-1.1.4/vcx_py.egg-info/dependency_links.txt
+-rw-r--r--   0 aarjaneiro  (1000) aarjaneiro  (1000)        7 2024-04-02 17:15:30.000000 vcx_py-1.1.4/vcx_py.egg-info/top_level.txt
```

### Comparing `vcx_py-1.1.3/LICENSE` & `vcx_py-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vcx_py-1.1.3/PKG-INFO` & `vcx_py-1.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vcx_py
-Version: 1.1.3
+Version: 1.1.4
 Summary: A simple python client for the VirgoCX API
 Home-page: https://www.github.com/aarjaneiro/vcx_py
 Author: Aaron Janeiro Stone
 Author-email: aaron@thequant.ca
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -32,14 +32,15 @@
     - [Account Information](#account-information)
     - [Query Orders](#query-orders)
     - [Query Trades](#query-trades)
     - [Place Order](#place-order)
     - [Cancel Order](#cancel-order)
     - [Get Discount](#get-discount)
 - [Warnings](#warnings)
+- [Paused Trading](#paused-trading)
 
 ## Setup
 
 ### API Keys
 
 Generate your API key and secret from the [VirgoCX website](https://virgocx.ca/en-virgocx-api). Ensure
 that the IP address of the machine you are running this client from is whitelisted.
@@ -164,7 +165,13 @@
 ```
 
 or you can use the environment variable `PYTHONWARNINGS` to suppress the warnings:
 
 ```bash
 export PYTHONWARNINGS="ignore:Unverified HTTPS request"
 ```
+
+## Paused Trading
+
+It is possible that trading on the exchange is paused. Unfortunately, the client does not have a way to check
+if trading is paused and thus `KeyError` exceptions may be raised when attempting to access keys from the API which
+are omitted in such cases. Eventually we hope to have an endpoint which will allow us to check if trading is paused.
```

### Comparing `vcx_py-1.1.3/README.md` & `vcx_py-1.1.4/vcx_py.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: vcx_py
+Version: 1.1.4
+Summary: A simple python client for the VirgoCX API
+Home-page: https://www.github.com/aarjaneiro/vcx_py
+Author: Aaron Janeiro Stone
+Author-email: aaron@thequant.ca
+License: MIT
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # VirgoCX Python Client
 
 A simple Python client for the VirgoCX API.
 
 For more information on the REST api on which this was built, please refer to the
 [VirgoCX API Documentation](https://github.com/VirgocxDev/VirgocxApiDoc).
 
@@ -21,14 +32,15 @@
     - [Account Information](#account-information)
     - [Query Orders](#query-orders)
     - [Query Trades](#query-trades)
     - [Place Order](#place-order)
     - [Cancel Order](#cancel-order)
     - [Get Discount](#get-discount)
 - [Warnings](#warnings)
+- [Paused Trading](#paused-trading)
 
 ## Setup
 
 ### API Keys
 
 Generate your API key and secret from the [VirgoCX website](https://virgocx.ca/en-virgocx-api). Ensure
 that the IP address of the machine you are running this client from is whitelisted.
@@ -152,8 +164,14 @@
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 ```
 
 or you can use the environment variable `PYTHONWARNINGS` to suppress the warnings:
 
 ```bash
 export PYTHONWARNINGS="ignore:Unverified HTTPS request"
-```
+```
+
+## Paused Trading
+
+It is possible that trading on the exchange is paused. Unfortunately, the client does not have a way to check
+if trading is paused and thus `KeyError` exceptions may be raised when attempting to access keys from the API which
+are omitted in such cases. Eventually we hope to have an endpoint which will allow us to check if trading is paused.
```

### Comparing `vcx_py-1.1.3/setup.py` & `vcx_py-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 #  SOFTWARE.
 
 from setuptools import setup
 
 setup(
     name='vcx_py',
-    version='1.1.3',
+    version='1.1.4',
     packages=['vcx_py'],
     license='MIT',
     author='Aaron Janeiro Stone',
     author_email='aaron@thequant.ca',
     description='A simple python client for the VirgoCX API',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

### Comparing `vcx_py-1.1.3/vcx_py/__init__.py` & `vcx_py-1.1.4/vcx_py/__init__.py`

 * *Files identical despite different names*

### Comparing `vcx_py-1.1.3/vcx_py/client.py` & `vcx_py-1.1.4/vcx_py/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,23 +141,33 @@
             if qty is None:
                 if not handle_conversions:
                     raise ValueError("Quantity is required for limit orders")
                 else:
                     qty = total / price
                     total = None
         else:  # i.e., quick trade or market order
-            if total is None and direction == OrderDirection.BUY:
+            if direction == OrderDirection.BUY:
+                if total is None:
+                    if not handle_conversions:
+                        raise ValueError("Total is required for non-limit buy orders")
+                    else:
+                        market_price = kwargs.get("market_price", None)
+                        if market_price is None:
+                            market_price = self.__extract_market_price__(direction, symbol)
+                        total = qty * market_price
+                        qty = None
+            elif qty is None:
                 if not handle_conversions:
-                    raise ValueError("Total is required for non-limit buy orders")
+                    raise ValueError("Quantity is required for non-buy orders")
                 else:
                     market_price = kwargs.get("market_price", None)
                     if market_price is None:
                         market_price = self.__extract_market_price__(direction, symbol)
-                    total = qty * market_price
-                    qty = None
+                    qty = total / market_price
+                    total = None
 
         payload = {"apiKey": self._api_key(), "symbol": symbol, "category": category, "type": direction,
                    "country": 1}
 
         with VirgoCXClient.STATIC_LOCK:
             if symbol in VirgoCXClient.FMT_DATA:
                 fmt_data = VirgoCXClient.FMT_DATA[symbol]
```

### Comparing `vcx_py-1.1.3/vcx_py/constants.py` & `vcx_py-1.1.4/vcx_py/constants.py`

 * *Files identical despite different names*

### Comparing `vcx_py-1.1.3/vcx_py/schema.py` & `vcx_py-1.1.4/vcx_py/schema.py`

 * *Files identical despite different names*

### Comparing `vcx_py-1.1.3/vcx_py/utils.py` & `vcx_py-1.1.4/vcx_py/utils.py`

 * *Files identical despite different names*

### Comparing `vcx_py-1.1.3/vcx_py.egg-info/PKG-INFO` & `vcx_py-1.1.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: vcx_py
-Version: 1.1.3
-Summary: A simple python client for the VirgoCX API
-Home-page: https://www.github.com/aarjaneiro/vcx_py
-Author: Aaron Janeiro Stone
-Author-email: aaron@thequant.ca
-License: MIT
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # VirgoCX Python Client
 
 A simple Python client for the VirgoCX API.
 
 For more information on the REST api on which this was built, please refer to the
 [VirgoCX API Documentation](https://github.com/VirgocxDev/VirgocxApiDoc).
 
@@ -32,14 +21,15 @@
     - [Account Information](#account-information)
     - [Query Orders](#query-orders)
     - [Query Trades](#query-trades)
     - [Place Order](#place-order)
     - [Cancel Order](#cancel-order)
     - [Get Discount](#get-discount)
 - [Warnings](#warnings)
+- [Paused Trading](#paused-trading)
 
 ## Setup
 
 ### API Keys
 
 Generate your API key and secret from the [VirgoCX website](https://virgocx.ca/en-virgocx-api). Ensure
 that the IP address of the machine you are running this client from is whitelisted.
@@ -164,7 +154,13 @@
 ```
 
 or you can use the environment variable `PYTHONWARNINGS` to suppress the warnings:
 
 ```bash
 export PYTHONWARNINGS="ignore:Unverified HTTPS request"
 ```
+
+## Paused Trading
+
+It is possible that trading on the exchange is paused. Unfortunately, the client does not have a way to check
+if trading is paused and thus `KeyError` exceptions may be raised when attempting to access keys from the API which
+are omitted in such cases. Eventually we hope to have an endpoint which will allow us to check if trading is paused.
```

