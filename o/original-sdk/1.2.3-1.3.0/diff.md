# Comparing `tmp/original_sdk-1.2.3.tar.gz` & `tmp/original_sdk-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "original_sdk-1.2.3.tar", last modified: Tue Mar 12 12:30:38 2024, max compression
+gzip compressed data, was "original_sdk-1.3.0.tar", last modified: Tue Apr  2 13:56:54 2024, max compression
```

## Comparing `original_sdk-1.2.3.tar` & `original_sdk-1.3.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 12:30:38.488460 original_sdk-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-03-12 12:30:26.000000 original_sdk-1.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-12 12:30:26.000000 original_sdk-1.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    20137 2024-03-12 12:30:38.488460 original_sdk-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19189 2024-03-12 12:30:26.000000 original_sdk-1.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 12:30:38.488460 original_sdk-1.2.3/original_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-03-12 12:30:26.000000 original_sdk-1.2.3/original_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-12 12:30:26.000000 original_sdk-1.2.3/original_sdk/__pkg__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7683 2024-03-12 12:30:26.000000 original_sdk-1.2.3/original_sdk/async_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 12:30:38.488460 original_sdk-1.2.3/original_sdk/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 12:30:26.000000 original_sdk-1.2.3/original_sdk/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7782 2024-03-12 12:30:26.000000 original_sdk-1.2.3/original_sdk/base/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6749 2024-03-12 12:30:26.000000 original_sdk-1.2.3/original_sdk/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 12:30:38.488460 original_sdk-1.2.3/original_sdk/types/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 12:30:26.000000 original_sdk-1.2.3/original_sdk/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-03-12 12:30:26.000000 original_sdk-1.2.3/original_sdk/types/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-03-12 12:30:26.000000 original_sdk-1.2.3/original_sdk/types/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-03-12 12:30:26.000000 original_sdk-1.2.3/original_sdk/types/original_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-03-12 12:30:26.000000 original_sdk-1.2.3/original_sdk/types/rate_limit.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-03-12 12:30:26.000000 original_sdk-1.2.3/original_sdk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 12:30:38.488460 original_sdk-1.2.3/original_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20137 2024-03-12 12:30:38.000000 original_sdk-1.2.3/original_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-03-12 12:30:38.000000 original_sdk-1.2.3/original_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 12:30:38.000000 original_sdk-1.2.3/original_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 12:30:38.000000 original_sdk-1.2.3/original_sdk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-03-12 12:30:38.000000 original_sdk-1.2.3/original_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-12 12:30:38.000000 original_sdk-1.2.3/original_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-03-12 12:30:26.000000 original_sdk-1.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-12 12:30:38.488460 original_sdk-1.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-03-12 12:30:26.000000 original_sdk-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:56:54.485653 original_sdk-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-02 13:56:46.000000 original_sdk-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-02 13:56:46.000000 original_sdk-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    25065 2024-04-02 13:56:54.481653 original_sdk-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    24117 2024-04-02 13:56:46.000000 original_sdk-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:56:54.481653 original_sdk-1.3.0/original_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-02 13:56:46.000000 original_sdk-1.3.0/original_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-02 13:56:46.000000 original_sdk-1.3.0/original_sdk/__pkg__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8647 2024-04-02 13:56:46.000000 original_sdk-1.3.0/original_sdk/async_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:56:54.481653 original_sdk-1.3.0/original_sdk/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 13:56:46.000000 original_sdk-1.3.0/original_sdk/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9723 2024-04-02 13:56:46.000000 original_sdk-1.3.0/original_sdk/base/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7629 2024-04-02 13:56:46.000000 original_sdk-1.3.0/original_sdk/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:56:54.481653 original_sdk-1.3.0/original_sdk/types/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 13:56:46.000000 original_sdk-1.3.0/original_sdk/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-02 13:56:46.000000 original_sdk-1.3.0/original_sdk/types/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-04-02 13:56:46.000000 original_sdk-1.3.0/original_sdk/types/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-04-02 13:56:46.000000 original_sdk-1.3.0/original_sdk/types/original_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-02 13:56:46.000000 original_sdk-1.3.0/original_sdk/types/rate_limit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-02 13:56:46.000000 original_sdk-1.3.0/original_sdk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:56:54.481653 original_sdk-1.3.0/original_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    25065 2024-04-02 13:56:54.000000 original_sdk-1.3.0/original_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-02 13:56:54.000000 original_sdk-1.3.0/original_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 13:56:54.000000 original_sdk-1.3.0/original_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 13:56:54.000000 original_sdk-1.3.0/original_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-02 13:56:54.000000 original_sdk-1.3.0/original_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-02 13:56:54.000000 original_sdk-1.3.0/original_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-02 13:56:46.000000 original_sdk-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 13:56:54.485653 original_sdk-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-02 13:56:46.000000 original_sdk-1.3.0/setup.py
```

### Comparing `original_sdk-1.2.3/LICENSE` & `original_sdk-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `original_sdk-1.2.3/PKG-INFO` & `original_sdk-1.3.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: original_sdk
-Version: 1.2.3
+Version: 1.3.0
 Summary: Python client for Original.
 Home-page: https://github.com/GetOriginal/original-python
 Author: Alexander Turowicz
 Author-email: support@getoriginal.com
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
@@ -48,14 +48,24 @@
     - [Create a new burn](#create-a-new-burn)
     - [Get a burn by burn UID](#get-a-burn-by-burn-uid)
     - [Get burns by user UID](#get-burns-by-user-uid)
   - [Deposit](#deposit)
     - [Get deposit details for a user](#get-deposit-details-by-user-uid)
   - [Collection](#collection)
     - [Get a collection by UID](#get-a-collection-by-collection-uid)
+  - [Allocation](#allocation)
+    - [Create a new allocation](#create-a-new-allocation)
+    - [Get an allocation by UID](#get-an-allocation-by-allocation-uid)
+    - [Get allocations by user UID](#get-allocations-by-user-uid)
+  - [Claim](#claim)
+    - [Create a new claim](#create-a-new-claim)
+    - [Get a claim by UID](#get-a-claim-by-claim-uid)
+    - [Get claims by user UID](#get-claims-by-user-uid)
+  - [Reward](#reward)
+    - [Get a reward by UID)](#get-a-reward-by-reward-uid)
   - [Handling Errors](#handling-errors)
 
 
 ## ✨ Getting started
 
 Ensure you have registered for an account at [Original](https://app.getoriginal.com) before getting started.
 You will need to create an app and note down your API key and secret from the [API Keys page](https://docs.getoriginal.com/docs/create-your-api-key) to use the Original SDK.
@@ -559,14 +569,181 @@
         "symbol": "SYM",
         "description": "Description of the collection",
         "explorer_url": "https://mumbai.polygonscan.com/address/0x124a6755ee787153bb6228463d5dc3a02890a7db"
     }
 }
 ```
 
+## Allocation
+
+The allocation methods exposed by the sdk are used to create and retrieve allocations from the Original API.
+
+### Create a new allocation
+```python
+
+# Prepare the allocation parameters
+allocation_params = {
+    "amount": 123.123,
+    "nonce": "nonce1",
+    "user_uid": "483581848722",
+    "reward_uid": "708469717542",
+}
+
+# Create an allocation
+allocation_response = client.create_allocation(**allocation_params)
+allocation_uid = allocation_response['data']['uid']
+# Sample allocation_response:
+{
+    "success": True,
+    "data": {
+        "uid": "365684656925",
+    }
+}
+```
+
+### Get an allocation by allocation UID
+```python
+
+# Get an allocation by UID, will throw a 404 Not Found error if the allocation does not exist
+allocation_response = client.get_allocation("365684656925")
+allocation_details = allocation_response['data']
+# Sample allocation_response:
+{
+    "success": True,
+    "data": {
+        "uid": "365684656925",
+        "status": "done",
+        "reward_uid": "reward_uid",
+        "to_user_uid": "754566475542",
+        "amount": 123.123,
+        "nonce": "nonce1",
+        "created_at": "2024-02-16T11:33:19.577827Z"
+    }
+}
+```
+
+### Get allocations by user UID
+```python
+# Get allocations by user UID
+allocations_response = client.get_allocations_by_user_uid("483581848722")
+allocations_list = allocations_response['data']
+# Sample allocations_response:
+{
+    "success": True,
+    "data": [
+        {
+            "uid": "365684656925",
+            "status": "done",
+            "reward_uid": "reward_uid",
+            "to_user_uid": "754566475542",
+            "amount": 123.123,
+            "nonce": "nonce1",
+            "created_at": "2024-02-16T11:33:19.577827Z"
+        }
+        # Additional allocations would be listed here
+    ]
+}
+```
+
+## Claim
+
+The claim methods exposed by the sdk are used to create and retrieve claims from the Original API.
+
+### Create a new claim
+```python
+
+# Prepare the claim parameters
+claim_params = {
+    "from_user_uid": "483581848722",
+    "reward_uid": "708469717542",
+    "to_address": '0x4881ab2f73c48a54b907a8b697b270f490768e6d'
+}
+
+# Create a claim
+claim_response = client.create_claim(**claim_params)
+claim_uid = claim_response['data']['uid']
+# Sample claim_response:
+{
+    "success": True,
+    "data": {
+        "uid": "365684656925",
+    }
+}
+```
+
+### Get a claim by claim UID
+```python
+
+# Get a claim by UID, will throw a 404 Not Found error if the claim does not exist
+claim_response = client.get_claim("365684656925")
+claim_details = claim_response['data']
+# Sample claim_response:
+{
+    "success": True,
+    "data": {
+        "uid": "365684656925",
+        "status": "done",
+        "reward_uid": "708469717542",
+        "from_user_uid": "754566475542",
+        "to_address": "0x4881ab2f73c48a54b907a8b697b270f490768e6d",
+        "amount": 123.123,
+        "created_at": "2024-02-16T11:33:19.577827Z"
+    }
+}
+```
+
+### Get claims by user UID
+```python
+# Get claims by user UID
+claims_response = client.get_claims_by_user_uid("483581848722")
+claims_list = claims_response['data']
+# Sample claims_response:
+{
+    "success": True,
+    "data": [
+        {
+            "uid": "365684656925",
+            "status": "done",
+            "reward_uid": "708469717542",
+            "from_user_uid": "754566475542",
+            "to_address": "0x4881ab2f73c48a54b907a8b697b270f490768e6d",
+            "amount": 123.123,
+            "created_at": "2024-02-16T11:33:19.577827Z"
+        }
+        # Additional claims would be listed here
+    ]
+}
+```
+
+## Reward
+
+The reward methods exposed by the sdk are used to retrieve reward details from the Original API.
+
+### Get a reward by reward UID
+```python
+# Get a reward by UID, will throw a 404 Not Found error if the reward does not exist
+reward_response = client.get_reward('221137489875')
+reward_details = reward_response['data']
+# Sample reward_response:
+{
+    "success": True,
+    "data": {
+        "uid": "151854912345",
+        "name": "Test SDK Reward 1",
+        "status": "deployed",
+        "token_type": "ERC20",
+        "token_name": "TestnetORI",
+        "created_at": "2024-02-13T10:45:56.952745Z",
+        "contract_address": "0x124a6755ee787153bb6228463d5dc3a02890a7db",
+        "withdraw_receiver": "0x4881ab2f73c48a54b907a8b697b270f490768e6d",
+        "description": "Description of the reward",
+        "explorer_url": "https://mumbai.polygonscan.com/address/0x124a6755ee787153bb6228463d5dc3a02890a7db"
+    }
+}
+```
 
 ## Handling Errors
 
 If something goes wrong, you will receive well typed error messages.
 
 ```python
 class ClientError(OriginalError): ...
```

### Comparing `original_sdk-1.2.3/README.md` & `original_sdk-1.3.0/original_sdk.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,32 @@
+Metadata-Version: 2.1
+Name: original-sdk
+Version: 1.3.0
+Summary: Python client for Original.
+Home-page: https://github.com/GetOriginal/original-python
+Author: Alexander Turowicz
+Author-email: support@getoriginal.com
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: System Administrators
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Software Development
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: test
+Provides-Extra: ci
+License-File: LICENSE
+
 # Official Python SDK for [Original](https://getoriginal.com) API
 
 ## Table of Contents
 
 - [Getting Started](#-getting-started)
 - [Documentation](#-documentation)
   - [Initialization](#initialization)
@@ -23,14 +48,24 @@
     - [Create a new burn](#create-a-new-burn)
     - [Get a burn by burn UID](#get-a-burn-by-burn-uid)
     - [Get burns by user UID](#get-burns-by-user-uid)
   - [Deposit](#deposit)
     - [Get deposit details for a user](#get-deposit-details-by-user-uid)
   - [Collection](#collection)
     - [Get a collection by UID](#get-a-collection-by-collection-uid)
+  - [Allocation](#allocation)
+    - [Create a new allocation](#create-a-new-allocation)
+    - [Get an allocation by UID](#get-an-allocation-by-allocation-uid)
+    - [Get allocations by user UID](#get-allocations-by-user-uid)
+  - [Claim](#claim)
+    - [Create a new claim](#create-a-new-claim)
+    - [Get a claim by UID](#get-a-claim-by-claim-uid)
+    - [Get claims by user UID](#get-claims-by-user-uid)
+  - [Reward](#reward)
+    - [Get a reward by UID)](#get-a-reward-by-reward-uid)
   - [Handling Errors](#handling-errors)
 
 
 ## ✨ Getting started
 
 Ensure you have registered for an account at [Original](https://app.getoriginal.com) before getting started.
 You will need to create an app and note down your API key and secret from the [API Keys page](https://docs.getoriginal.com/docs/create-your-api-key) to use the Original SDK.
@@ -534,14 +569,181 @@
         "symbol": "SYM",
         "description": "Description of the collection",
         "explorer_url": "https://mumbai.polygonscan.com/address/0x124a6755ee787153bb6228463d5dc3a02890a7db"
     }
 }
 ```
 
+## Allocation
+
+The allocation methods exposed by the sdk are used to create and retrieve allocations from the Original API.
+
+### Create a new allocation
+```python
+
+# Prepare the allocation parameters
+allocation_params = {
+    "amount": 123.123,
+    "nonce": "nonce1",
+    "user_uid": "483581848722",
+    "reward_uid": "708469717542",
+}
+
+# Create an allocation
+allocation_response = client.create_allocation(**allocation_params)
+allocation_uid = allocation_response['data']['uid']
+# Sample allocation_response:
+{
+    "success": True,
+    "data": {
+        "uid": "365684656925",
+    }
+}
+```
+
+### Get an allocation by allocation UID
+```python
+
+# Get an allocation by UID, will throw a 404 Not Found error if the allocation does not exist
+allocation_response = client.get_allocation("365684656925")
+allocation_details = allocation_response['data']
+# Sample allocation_response:
+{
+    "success": True,
+    "data": {
+        "uid": "365684656925",
+        "status": "done",
+        "reward_uid": "reward_uid",
+        "to_user_uid": "754566475542",
+        "amount": 123.123,
+        "nonce": "nonce1",
+        "created_at": "2024-02-16T11:33:19.577827Z"
+    }
+}
+```
+
+### Get allocations by user UID
+```python
+# Get allocations by user UID
+allocations_response = client.get_allocations_by_user_uid("483581848722")
+allocations_list = allocations_response['data']
+# Sample allocations_response:
+{
+    "success": True,
+    "data": [
+        {
+            "uid": "365684656925",
+            "status": "done",
+            "reward_uid": "reward_uid",
+            "to_user_uid": "754566475542",
+            "amount": 123.123,
+            "nonce": "nonce1",
+            "created_at": "2024-02-16T11:33:19.577827Z"
+        }
+        # Additional allocations would be listed here
+    ]
+}
+```
+
+## Claim
+
+The claim methods exposed by the sdk are used to create and retrieve claims from the Original API.
+
+### Create a new claim
+```python
+
+# Prepare the claim parameters
+claim_params = {
+    "from_user_uid": "483581848722",
+    "reward_uid": "708469717542",
+    "to_address": '0x4881ab2f73c48a54b907a8b697b270f490768e6d'
+}
+
+# Create a claim
+claim_response = client.create_claim(**claim_params)
+claim_uid = claim_response['data']['uid']
+# Sample claim_response:
+{
+    "success": True,
+    "data": {
+        "uid": "365684656925",
+    }
+}
+```
+
+### Get a claim by claim UID
+```python
+
+# Get a claim by UID, will throw a 404 Not Found error if the claim does not exist
+claim_response = client.get_claim("365684656925")
+claim_details = claim_response['data']
+# Sample claim_response:
+{
+    "success": True,
+    "data": {
+        "uid": "365684656925",
+        "status": "done",
+        "reward_uid": "708469717542",
+        "from_user_uid": "754566475542",
+        "to_address": "0x4881ab2f73c48a54b907a8b697b270f490768e6d",
+        "amount": 123.123,
+        "created_at": "2024-02-16T11:33:19.577827Z"
+    }
+}
+```
+
+### Get claims by user UID
+```python
+# Get claims by user UID
+claims_response = client.get_claims_by_user_uid("483581848722")
+claims_list = claims_response['data']
+# Sample claims_response:
+{
+    "success": True,
+    "data": [
+        {
+            "uid": "365684656925",
+            "status": "done",
+            "reward_uid": "708469717542",
+            "from_user_uid": "754566475542",
+            "to_address": "0x4881ab2f73c48a54b907a8b697b270f490768e6d",
+            "amount": 123.123,
+            "created_at": "2024-02-16T11:33:19.577827Z"
+        }
+        # Additional claims would be listed here
+    ]
+}
+```
+
+## Reward
+
+The reward methods exposed by the sdk are used to retrieve reward details from the Original API.
+
+### Get a reward by reward UID
+```python
+# Get a reward by UID, will throw a 404 Not Found error if the reward does not exist
+reward_response = client.get_reward('221137489875')
+reward_details = reward_response['data']
+# Sample reward_response:
+{
+    "success": True,
+    "data": {
+        "uid": "151854912345",
+        "name": "Test SDK Reward 1",
+        "status": "deployed",
+        "token_type": "ERC20",
+        "token_name": "TestnetORI",
+        "created_at": "2024-02-13T10:45:56.952745Z",
+        "contract_address": "0x124a6755ee787153bb6228463d5dc3a02890a7db",
+        "withdraw_receiver": "0x4881ab2f73c48a54b907a8b697b270f490768e6d",
+        "description": "Description of the reward",
+        "explorer_url": "https://mumbai.polygonscan.com/address/0x124a6755ee787153bb6228463d5dc3a02890a7db"
+    }
+}
+```
 
 ## Handling Errors
 
 If something goes wrong, you will receive well typed error messages.
 
 ```python
 class ClientError(OriginalError): ...
```

### Comparing `original_sdk-1.2.3/original_sdk/async_client.py` & `original_sdk-1.3.0/original_sdk/async_client.py`

 * *Files 13% similar despite different names*

```diff
@@ -198,14 +198,35 @@
 
     async def get_burns_by_user_uid(self, user_uid: str) -> OriginalResponse:
         return await self.get("burn", params={"user_uid": user_uid})
 
     async def get_deposit(self, user_uid: str) -> OriginalResponse:
         return await self.get("deposit", params={"user_uid": user_uid})
 
+    async def get_reward(self, uid: str) -> OriginalResponse:
+        return await self.get(f"reward/{uid}")
+
+    async def create_allocation(self, **allocation_data: Any) -> OriginalResponse:
+        return await self.post("reward/allocate", data=allocation_data)
+
+    async def get_allocation(self, uid: str) -> OriginalResponse:
+        return await self.get(f"reward/allocate/{uid}")
+
+    async def get_allocations_by_user_uid(self, user_uid: str) -> OriginalResponse:
+        return await self.get("reward/allocate", params={"user_uid": user_uid})
+
+    async def create_claim(self, **claim_data: Any) -> OriginalResponse:
+        return await self.post("reward/claim", data=claim_data)
+
+    async def get_claim(self, uid: str) -> OriginalResponse:
+        return await self.get(f"reward/claim/{uid}")
+
+    async def get_claims_by_user_uid(self, user_uid: str) -> OriginalResponse:
+        return await self.get("reward/claim", params={"user_uid": user_uid})
+
     async def close(self) -> None:
         await self.session.close()
 
     async def __aenter__(self) -> "OriginalAsyncClient":
         return self
 
     async def __aexit__(
```

### Comparing `original_sdk-1.2.3/original_sdk/base/client.py` & `original_sdk-1.3.0/original_sdk/base/client.py`

 * *Files 23% similar despite different names*

```diff
@@ -290,7 +290,91 @@
         """
         Get an Original deposit by user uid.
 
         :param user_uid: the user uid
         :return:
         """
         pass
+
+    @abc.abstractmethod
+    def get_reward(
+        self, uid: str
+    ) -> Union[OriginalResponse, Awaitable[OriginalResponse]]:
+        """
+        Get an Original reward.
+
+        :param uid: the reward uid
+        :return:
+        """
+        pass
+
+    @abc.abstractmethod
+    def create_allocation(
+        self, **allocation_data: Any
+    ) -> Union[OriginalResponse, Awaitable[OriginalResponse]]:
+        """
+        Create an Original allocation.
+
+        :param allocation_data: the allocation data
+        :return:
+        """
+        pass
+
+    @abc.abstractmethod
+    def get_allocation(
+        self, uid: str
+    ) -> Union[OriginalResponse, Awaitable[OriginalResponse]]:
+        """
+        Get an Original allocation.
+
+        :param uid: the allocation uid
+        :return:
+        """
+        pass
+
+    @abc.abstractmethod
+    def get_allocations_by_user_uid(
+        self, user_uid: str
+    ) -> Union[OriginalResponse, Awaitable[OriginalResponse]]:
+        """
+        Get a list of Original allocations by user uid.
+
+        :param user_uid: the app user uid
+        :return:
+        """
+        pass
+
+    @abc.abstractmethod
+    def create_claim(
+        self, **claim_data: Any
+    ) -> Union[OriginalResponse, Awaitable[OriginalResponse]]:
+        """
+        Create an Original claim.
+
+        :param claim_data: the claim data
+        :return:
+        """
+        pass
+
+    @abc.abstractmethod
+    def get_claim(
+        self, uid: str
+    ) -> Union[OriginalResponse, Awaitable[OriginalResponse]]:
+        """
+        Get an Original claim.
+
+        :param uid: the claim uid
+        :return:
+        """
+        pass
+
+    @abc.abstractmethod
+    def get_claims_by_user_uid(
+        self, user_uid: str
+    ) -> Union[OriginalResponse, Awaitable[OriginalResponse]]:
+        """
+        Get a list of Original claims by user uid.
+
+        :param user_uid: the app user uid
+        :return:
+        """
+        pass
```

### Comparing `original_sdk-1.2.3/original_sdk/client.py` & `original_sdk-1.3.0/original_sdk/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -181,7 +181,28 @@
         return self.get(f"burn/{uid}")
 
     def get_burns_by_user_uid(self, user_uid: str) -> OriginalResponse:
         return self.get("burn", params={"user_uid": user_uid})
 
     def get_deposit(self, user_uid: str) -> OriginalResponse:
         return self.get("deposit", params={"user_uid": user_uid})
+
+    def get_reward(self, uid: str) -> OriginalResponse:
+        return self.get(f"reward/{uid}")
+
+    def create_allocation(self, **allocation_data: Any) -> OriginalResponse:
+        return self.post("reward/allocate", data=allocation_data)
+
+    def get_allocation(self, uid: str) -> OriginalResponse:
+        return self.get(f"reward/allocate/{uid}")
+
+    def get_allocations_by_user_uid(self, user_uid: str) -> OriginalResponse:
+        return self.get("reward/allocate", params={"user_uid": user_uid})
+
+    def create_claim(self, **claim_data: Any) -> OriginalResponse:
+        return self.post("reward/claim", data=claim_data)
+
+    def get_claim(self, uid: str) -> OriginalResponse:
+        return self.get(f"reward/claim/{uid}")
+
+    def get_claims_by_user_uid(self, user_uid: str) -> OriginalResponse:
+        return self.get("reward/claim", params={"user_uid": user_uid})
```

### Comparing `original_sdk-1.2.3/original_sdk/types/exceptions.py` & `original_sdk-1.3.0/original_sdk/types/exceptions.py`

 * *Files identical despite different names*

### Comparing `original_sdk-1.2.3/original_sdk/types/original_response.py` & `original_sdk-1.3.0/original_sdk/types/original_response.py`

 * *Files identical despite different names*

### Comparing `original_sdk-1.2.3/original_sdk.egg-info/PKG-INFO` & `original_sdk-1.3.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,7 @@
-Metadata-Version: 2.1
-Name: original-sdk
-Version: 1.2.3
-Summary: Python client for Original.
-Home-page: https://github.com/GetOriginal/original-python
-Author: Alexander Turowicz
-Author-email: support@getoriginal.com
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: System Administrators
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: test
-Provides-Extra: ci
-License-File: LICENSE
-
 # Official Python SDK for [Original](https://getoriginal.com) API
 
 ## Table of Contents
 
 - [Getting Started](#-getting-started)
 - [Documentation](#-documentation)
   - [Initialization](#initialization)
@@ -48,14 +23,24 @@
     - [Create a new burn](#create-a-new-burn)
     - [Get a burn by burn UID](#get-a-burn-by-burn-uid)
     - [Get burns by user UID](#get-burns-by-user-uid)
   - [Deposit](#deposit)
     - [Get deposit details for a user](#get-deposit-details-by-user-uid)
   - [Collection](#collection)
     - [Get a collection by UID](#get-a-collection-by-collection-uid)
+  - [Allocation](#allocation)
+    - [Create a new allocation](#create-a-new-allocation)
+    - [Get an allocation by UID](#get-an-allocation-by-allocation-uid)
+    - [Get allocations by user UID](#get-allocations-by-user-uid)
+  - [Claim](#claim)
+    - [Create a new claim](#create-a-new-claim)
+    - [Get a claim by UID](#get-a-claim-by-claim-uid)
+    - [Get claims by user UID](#get-claims-by-user-uid)
+  - [Reward](#reward)
+    - [Get a reward by UID)](#get-a-reward-by-reward-uid)
   - [Handling Errors](#handling-errors)
 
 
 ## ✨ Getting started
 
 Ensure you have registered for an account at [Original](https://app.getoriginal.com) before getting started.
 You will need to create an app and note down your API key and secret from the [API Keys page](https://docs.getoriginal.com/docs/create-your-api-key) to use the Original SDK.
@@ -559,14 +544,181 @@
         "symbol": "SYM",
         "description": "Description of the collection",
         "explorer_url": "https://mumbai.polygonscan.com/address/0x124a6755ee787153bb6228463d5dc3a02890a7db"
     }
 }
 ```
 
+## Allocation
+
+The allocation methods exposed by the sdk are used to create and retrieve allocations from the Original API.
+
+### Create a new allocation
+```python
+
+# Prepare the allocation parameters
+allocation_params = {
+    "amount": 123.123,
+    "nonce": "nonce1",
+    "user_uid": "483581848722",
+    "reward_uid": "708469717542",
+}
+
+# Create an allocation
+allocation_response = client.create_allocation(**allocation_params)
+allocation_uid = allocation_response['data']['uid']
+# Sample allocation_response:
+{
+    "success": True,
+    "data": {
+        "uid": "365684656925",
+    }
+}
+```
+
+### Get an allocation by allocation UID
+```python
+
+# Get an allocation by UID, will throw a 404 Not Found error if the allocation does not exist
+allocation_response = client.get_allocation("365684656925")
+allocation_details = allocation_response['data']
+# Sample allocation_response:
+{
+    "success": True,
+    "data": {
+        "uid": "365684656925",
+        "status": "done",
+        "reward_uid": "reward_uid",
+        "to_user_uid": "754566475542",
+        "amount": 123.123,
+        "nonce": "nonce1",
+        "created_at": "2024-02-16T11:33:19.577827Z"
+    }
+}
+```
+
+### Get allocations by user UID
+```python
+# Get allocations by user UID
+allocations_response = client.get_allocations_by_user_uid("483581848722")
+allocations_list = allocations_response['data']
+# Sample allocations_response:
+{
+    "success": True,
+    "data": [
+        {
+            "uid": "365684656925",
+            "status": "done",
+            "reward_uid": "reward_uid",
+            "to_user_uid": "754566475542",
+            "amount": 123.123,
+            "nonce": "nonce1",
+            "created_at": "2024-02-16T11:33:19.577827Z"
+        }
+        # Additional allocations would be listed here
+    ]
+}
+```
+
+## Claim
+
+The claim methods exposed by the sdk are used to create and retrieve claims from the Original API.
+
+### Create a new claim
+```python
+
+# Prepare the claim parameters
+claim_params = {
+    "from_user_uid": "483581848722",
+    "reward_uid": "708469717542",
+    "to_address": '0x4881ab2f73c48a54b907a8b697b270f490768e6d'
+}
+
+# Create a claim
+claim_response = client.create_claim(**claim_params)
+claim_uid = claim_response['data']['uid']
+# Sample claim_response:
+{
+    "success": True,
+    "data": {
+        "uid": "365684656925",
+    }
+}
+```
+
+### Get a claim by claim UID
+```python
+
+# Get a claim by UID, will throw a 404 Not Found error if the claim does not exist
+claim_response = client.get_claim("365684656925")
+claim_details = claim_response['data']
+# Sample claim_response:
+{
+    "success": True,
+    "data": {
+        "uid": "365684656925",
+        "status": "done",
+        "reward_uid": "708469717542",
+        "from_user_uid": "754566475542",
+        "to_address": "0x4881ab2f73c48a54b907a8b697b270f490768e6d",
+        "amount": 123.123,
+        "created_at": "2024-02-16T11:33:19.577827Z"
+    }
+}
+```
+
+### Get claims by user UID
+```python
+# Get claims by user UID
+claims_response = client.get_claims_by_user_uid("483581848722")
+claims_list = claims_response['data']
+# Sample claims_response:
+{
+    "success": True,
+    "data": [
+        {
+            "uid": "365684656925",
+            "status": "done",
+            "reward_uid": "708469717542",
+            "from_user_uid": "754566475542",
+            "to_address": "0x4881ab2f73c48a54b907a8b697b270f490768e6d",
+            "amount": 123.123,
+            "created_at": "2024-02-16T11:33:19.577827Z"
+        }
+        # Additional claims would be listed here
+    ]
+}
+```
+
+## Reward
+
+The reward methods exposed by the sdk are used to retrieve reward details from the Original API.
+
+### Get a reward by reward UID
+```python
+# Get a reward by UID, will throw a 404 Not Found error if the reward does not exist
+reward_response = client.get_reward('221137489875')
+reward_details = reward_response['data']
+# Sample reward_response:
+{
+    "success": True,
+    "data": {
+        "uid": "151854912345",
+        "name": "Test SDK Reward 1",
+        "status": "deployed",
+        "token_type": "ERC20",
+        "token_name": "TestnetORI",
+        "created_at": "2024-02-13T10:45:56.952745Z",
+        "contract_address": "0x124a6755ee787153bb6228463d5dc3a02890a7db",
+        "withdraw_receiver": "0x4881ab2f73c48a54b907a8b697b270f490768e6d",
+        "description": "Description of the reward",
+        "explorer_url": "https://mumbai.polygonscan.com/address/0x124a6755ee787153bb6228463d5dc3a02890a7db"
+    }
+}
+```
 
 ## Handling Errors
 
 If something goes wrong, you will receive well typed error messages.
 
 ```python
 class ClientError(OriginalError): ...
```

### Comparing `original_sdk-1.2.3/original_sdk.egg-info/SOURCES.txt` & `original_sdk-1.3.0/original_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `original_sdk-1.2.3/pyproject.toml` & `original_sdk-1.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `original_sdk-1.2.3/setup.py` & `original_sdk-1.3.0/setup.py`

 * *Files identical despite different names*

