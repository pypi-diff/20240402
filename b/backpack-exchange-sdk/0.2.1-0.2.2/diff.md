# Comparing `tmp/backpack_exchange_sdk-0.2.1.tar.gz` & `tmp/backpack_exchange_sdk-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backpack_exchange_sdk-0.2.1.tar", last modified: Sun Mar 24 16:10:29 2024, max compression
+gzip compressed data, was "backpack_exchange_sdk-0.2.2.tar", last modified: Tue Apr  2 15:49:18 2024, max compression
```

## Comparing `backpack_exchange_sdk-0.2.1.tar` & `backpack_exchange_sdk-0.2.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 solomeowl   (501) staff       (20)        0 2024-03-24 16:10:29.288374 backpack_exchange_sdk-0.2.1/
--rw-r--r--   0 solomeowl   (501) staff       (20)     1066 2024-03-08 15:43:17.000000 backpack_exchange_sdk-0.2.1/LICENSE
--rw-r--r--   0 solomeowl   (501) staff       (20)     2470 2024-03-24 16:10:29.288143 backpack_exchange_sdk-0.2.1/PKG-INFO
--rw-r--r--   0 solomeowl   (501) staff       (20)     2112 2024-03-24 15:57:21.000000 backpack_exchange_sdk-0.2.1/README.md
-drwxr-xr-x   0 solomeowl   (501) staff       (20)        0 2024-03-24 16:10:29.286757 backpack_exchange_sdk-0.2.1/backpack_exchange_sdk/
--rw-r--r--   0 solomeowl   (501) staff       (20)        0 2024-03-09 08:21:03.000000 backpack_exchange_sdk-0.2.1/backpack_exchange_sdk/__init__.py
--rw-r--r--   0 solomeowl   (501) staff       (20)     9295 2024-03-24 16:07:16.000000 backpack_exchange_sdk-0.2.1/backpack_exchange_sdk/authenticated.py
--rw-r--r--   0 solomeowl   (501) staff       (20)     3754 2024-03-24 15:57:21.000000 backpack_exchange_sdk-0.2.1/backpack_exchange_sdk/public.py
-drwxr-xr-x   0 solomeowl   (501) staff       (20)        0 2024-03-24 16:10:29.287906 backpack_exchange_sdk-0.2.1/backpack_exchange_sdk.egg-info/
--rw-r--r--   0 solomeowl   (501) staff       (20)     2470 2024-03-24 16:10:29.000000 backpack_exchange_sdk-0.2.1/backpack_exchange_sdk.egg-info/PKG-INFO
--rw-r--r--   0 solomeowl   (501) staff       (20)      360 2024-03-24 16:10:29.000000 backpack_exchange_sdk-0.2.1/backpack_exchange_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 solomeowl   (501) staff       (20)        1 2024-03-24 16:10:29.000000 backpack_exchange_sdk-0.2.1/backpack_exchange_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 solomeowl   (501) staff       (20)       22 2024-03-24 16:10:29.000000 backpack_exchange_sdk-0.2.1/backpack_exchange_sdk.egg-info/top_level.txt
--rw-r--r--   0 solomeowl   (501) staff       (20)       38 2024-03-24 16:10:29.288429 backpack_exchange_sdk-0.2.1/setup.cfg
--rw-r--r--   0 solomeowl   (501) staff       (20)      533 2024-03-24 16:09:53.000000 backpack_exchange_sdk-0.2.1/setup.py
-drwxr-xr-x   0 solomeowl   (501) staff       (20)        0 2024-03-24 16:10:29.287741 backpack_exchange_sdk-0.2.1/tests/
--rw-r--r--   0 solomeowl   (501) staff       (20)        0 2024-03-09 08:00:27.000000 backpack_exchange_sdk-0.2.1/tests/test_authenticated.py
--rw-r--r--   0 solomeowl   (501) staff       (20)        0 2024-03-09 08:00:27.000000 backpack_exchange_sdk-0.2.1/tests/test_public.py
+drwxr-xr-x   0 solomeowl   (501) staff       (20)        0 2024-04-02 15:49:18.297391 backpack_exchange_sdk-0.2.2/
+-rw-r--r--   0 solomeowl   (501) staff       (20)     1066 2024-03-08 15:43:17.000000 backpack_exchange_sdk-0.2.2/LICENSE
+-rw-r--r--   0 solomeowl   (501) staff       (20)     2477 2024-04-02 15:49:18.297084 backpack_exchange_sdk-0.2.2/PKG-INFO
+-rw-r--r--   0 solomeowl   (501) staff       (20)     2119 2024-04-02 15:44:43.000000 backpack_exchange_sdk-0.2.2/README.md
+drwxr-xr-x   0 solomeowl   (501) staff       (20)        0 2024-04-02 15:49:18.295604 backpack_exchange_sdk-0.2.2/backpack_exchange_sdk/
+-rw-r--r--   0 solomeowl   (501) staff       (20)        0 2024-03-09 08:21:03.000000 backpack_exchange_sdk-0.2.2/backpack_exchange_sdk/__init__.py
+-rw-r--r--   0 solomeowl   (501) staff       (20)     9295 2024-03-24 16:07:16.000000 backpack_exchange_sdk-0.2.2/backpack_exchange_sdk/authenticated.py
+-rw-r--r--   0 solomeowl   (501) staff       (20)     3754 2024-03-24 15:57:21.000000 backpack_exchange_sdk-0.2.2/backpack_exchange_sdk/public.py
+drwxr-xr-x   0 solomeowl   (501) staff       (20)        0 2024-04-02 15:49:18.296789 backpack_exchange_sdk-0.2.2/backpack_exchange_sdk.egg-info/
+-rw-r--r--   0 solomeowl   (501) staff       (20)     2477 2024-04-02 15:49:18.000000 backpack_exchange_sdk-0.2.2/backpack_exchange_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 solomeowl   (501) staff       (20)      360 2024-04-02 15:49:18.000000 backpack_exchange_sdk-0.2.2/backpack_exchange_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 solomeowl   (501) staff       (20)        1 2024-04-02 15:49:18.000000 backpack_exchange_sdk-0.2.2/backpack_exchange_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 solomeowl   (501) staff       (20)       22 2024-04-02 15:49:18.000000 backpack_exchange_sdk-0.2.2/backpack_exchange_sdk.egg-info/top_level.txt
+-rw-r--r--   0 solomeowl   (501) staff       (20)       38 2024-04-02 15:49:18.297459 backpack_exchange_sdk-0.2.2/setup.cfg
+-rw-r--r--   0 solomeowl   (501) staff       (20)      533 2024-04-02 15:49:05.000000 backpack_exchange_sdk-0.2.2/setup.py
+drwxr-xr-x   0 solomeowl   (501) staff       (20)        0 2024-04-02 15:49:18.296589 backpack_exchange_sdk-0.2.2/tests/
+-rw-r--r--   0 solomeowl   (501) staff       (20)        0 2024-03-09 08:00:27.000000 backpack_exchange_sdk-0.2.2/tests/test_authenticated.py
+-rw-r--r--   0 solomeowl   (501) staff       (20)        0 2024-03-09 08:00:27.000000 backpack_exchange_sdk-0.2.2/tests/test_public.py
```

### Comparing `backpack_exchange_sdk-0.2.1/LICENSE` & `backpack_exchange_sdk-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `backpack_exchange_sdk-0.2.1/PKG-INFO` & `backpack_exchange_sdk-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: backpack_exchange_sdk
-Version: 0.2.1
+Version: 0.2.2
 Summary: A simple SDK for backpack exchange
 Home-page: https://github.com/solomeowl/backpack_exchange_sdk
 Author: solomeowl
 Author-email: j19940430@gmail.com
 Project-URL: Source, https://github.com/solomeowl/backpack_exchange_sdk
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Backpack Exchange SDK
-![PyPI - Version](https://img.shields.io/pypi/v/backpack-exchange-sdk)
+![PyPI - Version](https://img.shields.io/pypi/v/backpack-exchange-sdk?)
 
 
 The Backpack Exchange SDK provides a convenient interface for interacting with the Backpack Exchange API. It includes two main clients: `AuthenticationClient` for authenticated endpoints and `PublicClient` for public endpoints.
 
 ## Features
 
 - **Authentication Client**: Interact with authenticated endpoints for managing capital, historical data, and orders.
@@ -35,31 +35,30 @@
 cd backpack_exchange_sdk
 pip3 install .
 ```
 
 ## Usage
 ### Authentication Client
 ```python
-from backpack_exchange_sdk import AuthenticationClient
+from backpack_exchange_sdk.authenticated import AuthenticationClient
 
-client = AuthenticationClient()
-client.setup('<YOUR_API_KEY>', '<YOUR_SECRET>')
+client = AuthenticationClient('<YOUR_API_KEY>', '<YOUR_SECRET>')
 
 # Get account balances
 balances = client.get_balances()
 print(balances)
 
 # Request a withdrawal
 response = client.request_withdrawal('xxxxaddress', 'Solana', '0,1', 'Sol')
 print(response)
 
 ```
 ### Public Client
 ```python
-from backpack_exchange_sdk import PublicClient
+from backpack_exchange_sdk.public import PublicClient
 
 public_client = PublicClient()
 
 # Get all supported assets
 assets = public_client.get_assets()
 print(assets)
```

### Comparing `backpack_exchange_sdk-0.2.1/README.md` & `backpack_exchange_sdk-0.2.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Backpack Exchange SDK
-![PyPI - Version](https://img.shields.io/pypi/v/backpack-exchange-sdk)
+![PyPI - Version](https://img.shields.io/pypi/v/backpack-exchange-sdk?)
 
 
 The Backpack Exchange SDK provides a convenient interface for interacting with the Backpack Exchange API. It includes two main clients: `AuthenticationClient` for authenticated endpoints and `PublicClient` for public endpoints.
 
 ## Features
 
 - **Authentication Client**: Interact with authenticated endpoints for managing capital, historical data, and orders.
@@ -24,31 +24,30 @@
 cd backpack_exchange_sdk
 pip3 install .
 ```
 
 ## Usage
 ### Authentication Client
 ```python
-from backpack_exchange_sdk import AuthenticationClient
+from backpack_exchange_sdk.authenticated import AuthenticationClient
 
-client = AuthenticationClient()
-client.setup('<YOUR_API_KEY>', '<YOUR_SECRET>')
+client = AuthenticationClient('<YOUR_API_KEY>', '<YOUR_SECRET>')
 
 # Get account balances
 balances = client.get_balances()
 print(balances)
 
 # Request a withdrawal
 response = client.request_withdrawal('xxxxaddress', 'Solana', '0,1', 'Sol')
 print(response)
 
 ```
 ### Public Client
 ```python
-from backpack_exchange_sdk import PublicClient
+from backpack_exchange_sdk.public import PublicClient
 
 public_client = PublicClient()
 
 # Get all supported assets
 assets = public_client.get_assets()
 print(assets)
```

### Comparing `backpack_exchange_sdk-0.2.1/backpack_exchange_sdk/authenticated.py` & `backpack_exchange_sdk-0.2.2/backpack_exchange_sdk/authenticated.py`

 * *Files identical despite different names*

### Comparing `backpack_exchange_sdk-0.2.1/backpack_exchange_sdk/public.py` & `backpack_exchange_sdk-0.2.2/backpack_exchange_sdk/public.py`

 * *Files identical despite different names*

### Comparing `backpack_exchange_sdk-0.2.1/backpack_exchange_sdk.egg-info/PKG-INFO` & `backpack_exchange_sdk-0.2.2/backpack_exchange_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: backpack_exchange_sdk
-Version: 0.2.1
+Version: 0.2.2
 Summary: A simple SDK for backpack exchange
 Home-page: https://github.com/solomeowl/backpack_exchange_sdk
 Author: solomeowl
 Author-email: j19940430@gmail.com
 Project-URL: Source, https://github.com/solomeowl/backpack_exchange_sdk
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Backpack Exchange SDK
-![PyPI - Version](https://img.shields.io/pypi/v/backpack-exchange-sdk)
+![PyPI - Version](https://img.shields.io/pypi/v/backpack-exchange-sdk?)
 
 
 The Backpack Exchange SDK provides a convenient interface for interacting with the Backpack Exchange API. It includes two main clients: `AuthenticationClient` for authenticated endpoints and `PublicClient` for public endpoints.
 
 ## Features
 
 - **Authentication Client**: Interact with authenticated endpoints for managing capital, historical data, and orders.
@@ -35,31 +35,30 @@
 cd backpack_exchange_sdk
 pip3 install .
 ```
 
 ## Usage
 ### Authentication Client
 ```python
-from backpack_exchange_sdk import AuthenticationClient
+from backpack_exchange_sdk.authenticated import AuthenticationClient
 
-client = AuthenticationClient()
-client.setup('<YOUR_API_KEY>', '<YOUR_SECRET>')
+client = AuthenticationClient('<YOUR_API_KEY>', '<YOUR_SECRET>')
 
 # Get account balances
 balances = client.get_balances()
 print(balances)
 
 # Request a withdrawal
 response = client.request_withdrawal('xxxxaddress', 'Solana', '0,1', 'Sol')
 print(response)
 
 ```
 ### Public Client
 ```python
-from backpack_exchange_sdk import PublicClient
+from backpack_exchange_sdk.public import PublicClient
 
 public_client = PublicClient()
 
 # Get all supported assets
 assets = public_client.get_assets()
 print(assets)
```

### Comparing `backpack_exchange_sdk-0.2.1/setup.py` & `backpack_exchange_sdk-0.2.2/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="backpack_exchange_sdk",
-    version="0.2.1",
+    version="0.2.2",
     author="solomeowl",
     author_email="j19940430@gmail.com",
     description="A simple SDK for backpack exchange",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/solomeowl/backpack_exchange_sdk",
     project_urls={
```

