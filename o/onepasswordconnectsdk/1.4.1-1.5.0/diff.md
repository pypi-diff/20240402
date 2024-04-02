# Comparing `tmp/onepasswordconnectsdk-1.4.1.tar.gz` & `tmp/onepasswordconnectsdk-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onepasswordconnectsdk-1.4.1.tar", max compression
+gzip compressed data, was "onepasswordconnectsdk-1.5.0.tar", max compression
```

## Comparing `onepasswordconnectsdk-1.4.1.tar` & `onepasswordconnectsdk-1.5.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1069 2024-01-08 16:20:51.687317 onepasswordconnectsdk-1.4.1/LICENSE.md
--rw-r--r--   0        0        0     3095 2024-01-08 16:20:51.687317 onepasswordconnectsdk-1.4.1/README.md
--rw-r--r--   0        0        0      681 2024-01-08 16:20:51.687317 onepasswordconnectsdk-1.4.1/pyproject.toml
--rw-r--r--   0        0        0      424 2024-01-08 16:20:51.687317 onepasswordconnectsdk-1.4.1/src/onepasswordconnectsdk/__init__.py
--rw-r--r--   0        0        0    14316 2024-01-08 16:20:51.687317 onepasswordconnectsdk-1.4.1/src/onepasswordconnectsdk/async_client.py
--rw-r--r--   0        0        0    15882 2024-01-08 16:20:51.687317 onepasswordconnectsdk-1.4.1/src/onepasswordconnectsdk/client.py
--rw-r--r--   0        0        0     7361 2024-01-08 16:20:51.687317 onepasswordconnectsdk-1.4.1/src/onepasswordconnectsdk/config.py
--rw-r--r--   0        0        0        0 2024-01-08 16:20:51.687317 onepasswordconnectsdk-1.4.1/src/onepasswordconnectsdk/connect.py
--rw-r--r--   0        0        0      473 2024-01-08 16:20:51.687317 onepasswordconnectsdk-1.4.1/src/onepasswordconnectsdk/errors.py
--rw-r--r--   0        0        0     1122 2024-01-08 16:20:51.687317 onepasswordconnectsdk-1.4.1/src/onepasswordconnectsdk/models/__init__.py
--rw-r--r--   0        0        0      145 2024-01-08 16:20:51.687317 onepasswordconnectsdk-1.4.1/src/onepasswordconnectsdk/models/constants.py
--rw-r--r--   0        0        0     3691 2024-01-08 16:20:51.691317 onepasswordconnectsdk-1.4.1/src/onepasswordconnectsdk/models/error.py
--rw-r--r--   0        0        0     9220 2024-01-08 16:20:51.691317 onepasswordconnectsdk-1.4.1/src/onepasswordconnectsdk/models/field.py
--rw-r--r--   0        0        0     2830 2024-01-08 16:20:51.691317 onepasswordconnectsdk-1.4.1/src/onepasswordconnectsdk/models/field_section.py
--rw-r--r--   0        0        0     2745 2024-01-08 16:20:51.691317 onepasswordconnectsdk-1.4.1/src/onepasswordconnectsdk/models/file.py
--rw-r--r--   0        0        0     5005 2024-01-08 16:20:51.691317 onepasswordconnectsdk-1.4.1/src/onepasswordconnectsdk/models/generator_recipe.py
--rw-r--r--   0        0        0    10861 2024-01-08 16:20:51.691317 onepasswordconnectsdk-1.4.1/src/onepasswordconnectsdk/models/item.py
--rw-r--r--   0        0        0     3610 2024-01-08 16:20:51.691317 onepasswordconnectsdk-1.4.1/src/onepasswordconnectsdk/models/item_details.py
--rw-r--r--   0        0        0     3499 2024-01-08 16:20:51.691317 onepasswordconnectsdk-1.4.1/src/onepasswordconnectsdk/models/item_urls.py
--rw-r--r--   0        0        0     2846 2024-01-08 16:20:51.691317 onepasswordconnectsdk-1.4.1/src/onepasswordconnectsdk/models/item_vault.py
--rw-r--r--   0        0        0       93 2024-01-08 16:20:51.691317 onepasswordconnectsdk-1.4.1/src/onepasswordconnectsdk/models/parsed_field.py
--rw-r--r--   0        0        0      212 2024-01-08 16:20:51.691317 onepasswordconnectsdk-1.4.1/src/onepasswordconnectsdk/models/parsed_item.py
--rw-r--r--   0        0        0     3341 2024-01-08 16:20:51.691317 onepasswordconnectsdk-1.4.1/src/onepasswordconnectsdk/models/section.py
--rw-r--r--   0        0        0     9652 2024-01-08 16:20:51.691317 onepasswordconnectsdk-1.4.1/src/onepasswordconnectsdk/models/summary_item.py
--rw-r--r--   0        0        0     8766 2024-01-08 16:20:51.691317 onepasswordconnectsdk-1.4.1/src/onepasswordconnectsdk/models/vault.py
--rw-r--r--   0        0        0     6778 2024-01-08 16:20:51.691317 onepasswordconnectsdk-1.4.1/src/onepasswordconnectsdk/serializer.py
--rw-r--r--   0        0        0     1703 2024-01-08 16:20:51.691317 onepasswordconnectsdk-1.4.1/src/onepasswordconnectsdk/utils.py
--rw-r--r--   0        0        0     4073 1970-01-01 00:00:00.000000 onepasswordconnectsdk-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-02 16:40:12.005767 onepasswordconnectsdk-1.5.0/LICENSE.md
+-rw-r--r--   0        0        0     3313 2024-04-02 16:40:12.005767 onepasswordconnectsdk-1.5.0/README.md
+-rw-r--r--   0        0        0      681 2024-04-02 16:40:12.005767 onepasswordconnectsdk-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0      424 2024-04-02 16:40:12.005767 onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/__init__.py
+-rw-r--r--   0        0        0    14399 2024-04-02 16:40:12.005767 onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/async_client.py
+-rw-r--r--   0        0        0    15938 2024-04-02 16:40:12.005767 onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/client.py
+-rw-r--r--   0        0        0     7361 2024-04-02 16:40:12.005767 onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/config.py
+-rw-r--r--   0        0        0        0 2024-04-02 16:40:12.005767 onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/connect.py
+-rw-r--r--   0        0        0      473 2024-04-02 16:40:12.005767 onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/errors.py
+-rw-r--r--   0        0        0     1122 2024-04-02 16:40:12.005767 onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/models/__init__.py
+-rw-r--r--   0        0        0      145 2024-04-02 16:40:12.005767 onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/models/constants.py
+-rw-r--r--   0        0        0     3691 2024-04-02 16:40:12.005767 onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/models/error.py
+-rw-r--r--   0        0        0     9220 2024-04-02 16:40:12.009767 onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/models/field.py
+-rw-r--r--   0        0        0     2830 2024-04-02 16:40:12.009767 onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/models/field_section.py
+-rw-r--r--   0        0        0     2745 2024-04-02 16:40:12.009767 onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/models/file.py
+-rw-r--r--   0        0        0     6599 2024-04-02 16:40:12.009767 onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/models/generator_recipe.py
+-rw-r--r--   0        0        0    10861 2024-04-02 16:40:12.009767 onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/models/item.py
+-rw-r--r--   0        0        0     3610 2024-04-02 16:40:12.009767 onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/models/item_details.py
+-rw-r--r--   0        0        0     3499 2024-04-02 16:40:12.009767 onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/models/item_urls.py
+-rw-r--r--   0        0        0     2846 2024-04-02 16:40:12.009767 onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/models/item_vault.py
+-rw-r--r--   0        0        0       93 2024-04-02 16:40:12.009767 onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/models/parsed_field.py
+-rw-r--r--   0        0        0      212 2024-04-02 16:40:12.009767 onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/models/parsed_item.py
+-rw-r--r--   0        0        0     3341 2024-04-02 16:40:12.009767 onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/models/section.py
+-rw-r--r--   0        0        0     9652 2024-04-02 16:40:12.009767 onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/models/summary_item.py
+-rw-r--r--   0        0        0     8766 2024-04-02 16:40:12.009767 onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/models/vault.py
+-rw-r--r--   0        0        0     6778 2024-04-02 16:40:12.009767 onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/serializer.py
+-rw-r--r--   0        0        0     2104 2024-04-02 16:40:12.009767 onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/utils.py
+-rw-r--r--   0        0        0     4291 1970-01-01 00:00:00.000000 onepasswordconnectsdk-1.5.0/PKG-INFO
```

### Comparing `onepasswordconnectsdk-1.4.1/LICENSE.md` & `onepasswordconnectsdk-1.5.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `onepasswordconnectsdk-1.4.1/README.md` & `onepasswordconnectsdk-1.5.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -27,14 +27,20 @@
 
 2. Export the `OP_CONNECT_HOST` and `OP_CONNECT_TOKEN` environment variables:
 
    ```sh
    export OP_CONNECT_HOST=<your-connect-host> && \
    export OP_CONNECT_TOKEN=<your-connect-token>
    ```
+   
+   2.1 If you need a higher timeout on the client requests you can export `OP_CLIENT_REQUEST_TIMEOUT` environment variable:
+   ```sh
+   # set the timeout to 90 seconds
+   export OP_CLIENT_REQUEST_TIMEOUT=90
+   ```
 
 3. Use the SDK:
 
    - Read a secret:
 
      ```python
      from onepasswordconnectsdk.client import (
```

#### html2text {}

```diff
@@ -7,28 +7,30 @@
 infrastructure. The library is intended to be used by Python applications to
 simplify accessing items in 1Password vaults. ## ðª See it in action Check
 the [Python Connect SDK Example](example/README.md) to see an example of item
 manipulation using the SDK that you can execute on your machine. ## â¨ Get
 started 1. Install the 1Password Connect Python SDK: ```sh pip install
 onepasswordconnectsdk ``` 2. Export the `OP_CONNECT_HOST` and
 `OP_CONNECT_TOKEN` environment variables: ```sh export OP_CONNECT_HOST= && \
-export OP_CONNECT_TOKEN= ``` 3. Use the SDK: - Read a secret: ```python from
-onepasswordconnectsdk.client import ( Client, new_client_from_environment, )
-connect_client: Client = new_client_from_environment() client.get_item("
-{item_id}", "{vault_id}") ``` - Write a secret: ```python from
-onepasswordconnectsdk.client import ( Client, new_client_from_environment, }
-from onepasswordconnectsdk.models import ( Item, ItemVault, Field )
-connect_client: Client = new_client_from_environment() # Example item creation.
-Create an item with your desired arguments. item = Item( vault=ItemVault
-(id=op_vault), id="custom_id", title="newtitle", category="LOGIN", tags=
-["1password-connect"], fields=[Field(value="new_user", purpose="USERNAME")], )
-new_item = connect_client.create_item(op_vault, item) ``` For more examples of
-how to use the SDK, check out [USAGE.md](USAGE.md). ## ð Community & Support
-- File an [issue](https://github.com/1Password/connect-sdk-python/issues) for
-bugs and feature requests. - Join the [Developer Slack workspace](https://
-join.slack.com/t/1password-devs/shared_invite/zt-1halo11ps-
-6o9pEv96xZ3LtX_VE0fJQA). - Subscribe to the [Developer Newsletter](https://
-1password.com/dev-subscribe/). ## ð Security 1Password requests you practice
-responsible disclosure if you discover a vulnerability. Please file requests
-via [**BugCrowd**](https://bugcrowd.com/agilebits). For information about
-security practices, please visit the [1Password Bug Bounty Program](https://
-bugcrowd.com/agilebits).
+export OP_CONNECT_TOKEN= ``` 2.1 If you need a higher timeout on the client
+requests you can export `OP_CLIENT_REQUEST_TIMEOUT` environment variable: ```sh
+# set the timeout to 90 seconds export OP_CLIENT_REQUEST_TIMEOUT=90 ``` 3. Use
+the SDK: - Read a secret: ```python from onepasswordconnectsdk.client import
+( Client, new_client_from_environment, ) connect_client: Client =
+new_client_from_environment() client.get_item("{item_id}", "{vault_id}") ``` -
+Write a secret: ```python from onepasswordconnectsdk.client import ( Client,
+new_client_from_environment, } from onepasswordconnectsdk.models import ( Item,
+ItemVault, Field ) connect_client: Client = new_client_from_environment() #
+Example item creation. Create an item with your desired arguments. item = Item
+( vault=ItemVault(id=op_vault), id="custom_id", title="newtitle",
+category="LOGIN", tags=["1password-connect"], fields=[Field(value="new_user",
+purpose="USERNAME")], ) new_item = connect_client.create_item(op_vault, item)
+``` For more examples of how to use the SDK, check out [USAGE.md](USAGE.md). ##
+ð Community & Support - File an [issue](https://github.com/1Password/
+connect-sdk-python/issues) for bugs and feature requests. - Join the [Developer
+Slack workspace](https://join.slack.com/t/1password-devs/shared_invite/zt-
+1halo11ps-6o9pEv96xZ3LtX_VE0fJQA). - Subscribe to the [Developer Newsletter]
+(https://1password.com/dev-subscribe/). ## ð Security 1Password requests you
+practice responsible disclosure if you discover a vulnerability. Please file
+requests via [**BugCrowd**](https://bugcrowd.com/agilebits). For information
+about security practices, please visit the [1Password Bug Bounty Program]
+(https://bugcrowd.com/agilebits).
```

### Comparing `onepasswordconnectsdk-1.4.1/pyproject.toml` & `onepasswordconnectsdk-1.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "onepasswordconnectsdk"
-version = "1.4.1"
+version = "1.5.0"
 description = "Python SDK for 1Password Connect"
 license = "MIT"
 authors = ["1Password"]
 readme = "README.md"
 repository = "https://github.com/1Password/connect-sdk-python"
 
 [tool.poetry.urls]
```

### Comparing `onepasswordconnectsdk-1.4.1/src/onepasswordconnectsdk/async_client.py` & `onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Python AsyncClient for connecting to 1Password Connect"""
 import httpx
 from httpx import HTTPError
 from typing import Dict, List, Union
 import os
 
 from onepasswordconnectsdk.serializer import Serializer
-from onepasswordconnectsdk.utils import build_headers, is_valid_uuid, PathBuilder
+from onepasswordconnectsdk.utils import build_headers, is_valid_uuid, PathBuilder, get_timeout
 from onepasswordconnectsdk.errors import (
     FailedToRetrieveItemException,
     FailedToRetrieveVaultException,
 )
 from onepasswordconnectsdk.models import File, Item, ItemVault, SummaryItem, Vault
 
 
@@ -20,15 +20,16 @@
         """Initialize async client"""
         self.url = url
         self.token = token
         self.session = self.create_session(url, token)
         self.serializer = Serializer()
 
     def create_session(self, url: str, token: str) -> httpx.AsyncClient:
-        return httpx.AsyncClient(base_url=url, headers=self.build_headers(token))
+        # import here to avoid circular import
+        return httpx.AsyncClient(base_url=url, headers=self.build_headers(token), timeout=get_timeout())
 
     def build_headers(self, token: str) -> Dict[str, str]:
         return build_headers(token)
 
     async def __aexit__(self):
         await self.session.aclose()
```

### Comparing `onepasswordconnectsdk-1.4.1/src/onepasswordconnectsdk/client.py` & `onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Python Client for connecting to 1Password Connect"""
 import httpx
-from httpx import HTTPError
+from httpx import HTTPError, USE_CLIENT_DEFAULT
 import json
 from typing import Dict, List, Union
 import os
 
 from onepasswordconnectsdk.async_client import AsyncClient
 from onepasswordconnectsdk.serializer import Serializer
-from onepasswordconnectsdk.utils import build_headers, is_valid_uuid, PathBuilder
+from onepasswordconnectsdk.utils import build_headers, is_valid_uuid, PathBuilder, get_timeout
 from onepasswordconnectsdk.errors import (
     FailedToRetrieveItemException,
     FailedToRetrieveVaultException,
     EnvironmentHostNotSetException,
     EnvironmentTokenNotSetException,
 )
 from onepasswordconnectsdk.models import File, Item, ItemVault, SummaryItem, Vault
@@ -28,15 +28,15 @@
         """Initialize client"""
         self.url = url
         self.token = token
         self.session = self.create_session(url, token)
         self.serializer = Serializer()
 
     def create_session(self, url: str, token: str) -> httpx.Client:
-        return httpx.Client(base_url=url, headers=self.build_headers(token))
+        return httpx.Client(base_url=url, headers=self.build_headers(token), timeout=get_timeout())
 
     def build_headers(self, token: str) -> Dict[str, str]:
         return build_headers(token)
 
     def __del__(self) -> None:
         self.session.close()
```

### Comparing `onepasswordconnectsdk-1.4.1/src/onepasswordconnectsdk/config.py` & `onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/config.py`

 * *Files identical despite different names*

### Comparing `onepasswordconnectsdk-1.4.1/src/onepasswordconnectsdk/models/__init__.py` & `onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/models/__init__.py`

 * *Files identical despite different names*

### Comparing `onepasswordconnectsdk-1.4.1/src/onepasswordconnectsdk/models/error.py` & `onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/models/error.py`

 * *Files identical despite different names*

### Comparing `onepasswordconnectsdk-1.4.1/src/onepasswordconnectsdk/models/field.py` & `onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/models/field.py`

 * *Files identical despite different names*

### Comparing `onepasswordconnectsdk-1.4.1/src/onepasswordconnectsdk/models/field_section.py` & `onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/models/field_section.py`

 * *Files identical despite different names*

### Comparing `onepasswordconnectsdk-1.4.1/src/onepasswordconnectsdk/models/file.py` & `onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/models/file.py`

 * *Files identical despite different names*

### Comparing `onepasswordconnectsdk-1.4.1/src/onepasswordconnectsdk/models/item.py` & `onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/models/item.py`

 * *Files identical despite different names*

### Comparing `onepasswordconnectsdk-1.4.1/src/onepasswordconnectsdk/models/item_details.py` & `onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/models/item_details.py`

 * *Files identical despite different names*

### Comparing `onepasswordconnectsdk-1.4.1/src/onepasswordconnectsdk/models/item_urls.py` & `onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/models/item_urls.py`

 * *Files identical despite different names*

### Comparing `onepasswordconnectsdk-1.4.1/src/onepasswordconnectsdk/models/item_vault.py` & `onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/models/item_vault.py`

 * *Files identical despite different names*

### Comparing `onepasswordconnectsdk-1.4.1/src/onepasswordconnectsdk/models/section.py` & `onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/models/section.py`

 * *Files identical despite different names*

### Comparing `onepasswordconnectsdk-1.4.1/src/onepasswordconnectsdk/models/summary_item.py` & `onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/models/summary_item.py`

 * *Files identical despite different names*

### Comparing `onepasswordconnectsdk-1.4.1/src/onepasswordconnectsdk/models/vault.py` & `onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/models/vault.py`

 * *Files identical despite different names*

### Comparing `onepasswordconnectsdk-1.4.1/src/onepasswordconnectsdk/serializer.py` & `onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/serializer.py`

 * *Files identical despite different names*

### Comparing `onepasswordconnectsdk-1.4.1/src/onepasswordconnectsdk/utils.py` & `onepasswordconnectsdk-1.5.0/src/onepasswordconnectsdk/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,107 +1,132 @@
-00000000: 5555 4944 4c65 6e67 7468 203d 2032 360a  UUIDLength = 26.
-00000010: 0a0a 6465 6620 6973 5f76 616c 6964 5f75  ..def is_valid_u
-00000020: 7569 6428 7575 6964 293a 0a20 2020 2069  uid(uuid):.    i
-00000030: 6620 6c65 6e28 7575 6964 2920 6973 206e  f len(uuid) is n
-00000040: 6f74 2055 5549 444c 656e 6774 683a 0a20  ot UUIDLength:. 
-00000050: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
-00000060: 6c73 650a 2020 2020 666f 7220 6320 696e  lse.    for c in
-00000070: 2075 7569 643a 0a20 2020 2020 2020 2076   uuid:.        v
-00000080: 616c 6964 203d 2028 6320 3e3d 2027 6127  alid = (c >= 'a'
-00000090: 2061 6e64 2063 203c 3d20 277a 2729 206f   and c <= 'z') o
-000000a0: 7220 2863 203e 3d20 2730 2720 616e 6420  r (c >= '0' and 
-000000b0: 6320 3c3d 2027 3927 290a 2020 2020 2020  c <= '9').      
-000000c0: 2020 6966 2076 616c 6964 2069 7320 4661    if valid is Fa
-000000d0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-000000e0: 2072 6574 7572 6e20 4661 6c73 650a 2020   return False.  
-000000f0: 2020 7265 7475 726e 2054 7275 650a 0a0a    return True...
-00000100: 6465 6620 6275 696c 645f 6865 6164 6572  def build_header
-00000110: 7328 746f 6b65 6e3a 2073 7472 293a 0a20  s(token: str):. 
-00000120: 2020 2022 2222 4275 696c 6473 2074 6865     """Builds the
-00000130: 2068 6561 6465 7273 206e 6565 6465 6420   headers needed 
-00000140: 746f 206d 616b 6520 6120 7265 7175 6573  to make a reques
-00000150: 7420 746f 2074 6865 2073 6572 7665 720a  t to the server.
-00000160: 0a20 2020 2052 6574 7572 6e73 3a0a 2020  .    Returns:.  
-00000170: 2020 2020 2020 6469 6374 3a20 5468 6520        dict: The 
-00000180: 3150 6173 7377 6f72 6420 436f 6e6e 6563  1Password Connec
-00000190: 7420 4150 4920 7265 7175 6573 7420 6865  t API request he
-000001a0: 6164 6572 730a 2020 2020 2222 220a 2020  aders.    """.  
-000001b0: 2020 7265 7475 726e 207b 2241 7574 686f    return {"Autho
-000001c0: 7269 7a61 7469 6f6e 223a 2066 2242 6561  rization": f"Bea
-000001d0: 7265 7220 7b74 6f6b 656e 7d22 2c20 2243  rer {token}", "C
-000001e0: 6f6e 7465 6e74 2d54 7970 6522 3a20 2261  ontent-Type": "a
-000001f0: 7070 6c69 6361 7469 6f6e 2f6a 736f 6e22  pplication/json"
-00000200: 7d0a 0a0a 636c 6173 7320 5061 7468 4275  }...class PathBu
-00000210: 696c 6465 723a 0a20 2020 2064 6566 205f  ilder:.    def _
-00000220: 5f69 6e69 745f 5f28 7365 6c66 2c20 7665  _init__(self, ve
-00000230: 7273 696f 6e3a 2073 7472 203d 2022 2f76  rsion: str = "/v
-00000240: 3122 293a 0a20 2020 2020 2020 2073 656c  1"):.        sel
-00000250: 662e 7061 7468 3a20 7374 7220 3d20 7665  f.path: str = ve
-00000260: 7273 696f 6e0a 0a20 2020 2064 6566 2062  rsion..    def b
-00000270: 7569 6c64 2873 656c 6629 202d 3e20 7374  uild(self) -> st
-00000280: 723a 0a20 2020 2020 2020 2072 6574 7572  r:.        retur
-00000290: 6e20 7365 6c66 2e70 6174 680a 0a20 2020  n self.path..   
-000002a0: 2064 6566 2076 6175 6c74 7328 7365 6c66   def vaults(self
-000002b0: 2c20 7575 6964 3a20 7374 7220 3d20 4e6f  , uuid: str = No
-000002c0: 6e65 2920 2d3e 2027 5061 7468 4275 696c  ne) -> 'PathBuil
-000002d0: 6465 7227 3a0a 2020 2020 2020 2020 7365  der':.        se
-000002e0: 6c66 2e5f 6170 7065 6e64 5f70 6174 6828  lf._append_path(
-000002f0: 2276 6175 6c74 7322 290a 2020 2020 2020  "vaults").      
-00000300: 2020 6966 2075 7569 6420 6973 206e 6f74    if uuid is not
-00000310: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00000320: 2020 2073 656c 662e 5f61 7070 656e 645f     self._append_
-00000330: 7061 7468 2875 7569 6429 0a20 2020 2020  path(uuid).     
-00000340: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
-00000350: 2020 2020 6465 6620 6974 656d 7328 7365      def items(se
+00000000: 696d 706f 7274 206f 730a 6672 6f6d 2074  import os.from t
+00000010: 7970 696e 6720 696d 706f 7274 2055 6e69  yping import Uni
+00000020: 6f6e 0a0a 6672 6f6d 2068 7474 7078 2069  on..from httpx i
+00000030: 6d70 6f72 7420 5553 455f 434c 4945 4e54  mport USE_CLIENT
+00000040: 5f44 4546 4155 4c54 0a66 726f 6d20 6874  _DEFAULT.from ht
+00000050: 7470 782e 5f63 6c69 656e 7420 696d 706f  tpx._client impo
+00000060: 7274 2055 7365 436c 6965 6e74 4465 6661  rt UseClientDefa
+00000070: 756c 740a 0a55 5549 444c 656e 6774 6820  ult..UUIDLength 
+00000080: 3d20 3236 0a45 4e56 5f43 4c49 454e 545f  = 26.ENV_CLIENT_
+00000090: 5245 5155 4553 545f 5449 4d45 4f55 5420  REQUEST_TIMEOUT 
+000000a0: 3d20 224f 505f 434f 4e4e 4543 545f 434c  = "OP_CONNECT_CL
+000000b0: 4945 4e54 5f52 4551 5f54 494d 454f 5554  IENT_REQ_TIMEOUT
+000000c0: 220a 0a0a 6465 6620 6973 5f76 616c 6964  "...def is_valid
+000000d0: 5f75 7569 6428 7575 6964 293a 0a20 2020  _uuid(uuid):.   
+000000e0: 2069 6620 6c65 6e28 7575 6964 2920 6973   if len(uuid) is
+000000f0: 206e 6f74 2055 5549 444c 656e 6774 683a   not UUIDLength:
+00000100: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00000110: 4661 6c73 650a 2020 2020 666f 7220 6320  False.    for c 
+00000120: 696e 2075 7569 643a 0a20 2020 2020 2020  in uuid:.       
+00000130: 2076 616c 6964 203d 2028 6320 3e3d 2027   valid = (c >= '
+00000140: 6127 2061 6e64 2063 203c 3d20 277a 2729  a' and c <= 'z')
+00000150: 206f 7220 2863 203e 3d20 2730 2720 616e   or (c >= '0' an
+00000160: 6420 6320 3c3d 2027 3927 290a 2020 2020  d c <= '9').    
+00000170: 2020 2020 6966 2076 616c 6964 2069 7320      if valid is 
+00000180: 4661 6c73 653a 0a20 2020 2020 2020 2020  False:.         
+00000190: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
+000001a0: 2020 2020 7265 7475 726e 2054 7275 650a      return True.
+000001b0: 0a0a 6465 6620 6275 696c 645f 6865 6164  ..def build_head
+000001c0: 6572 7328 746f 6b65 6e3a 2073 7472 293a  ers(token: str):
+000001d0: 0a20 2020 2022 2222 4275 696c 6473 2074  .    """Builds t
+000001e0: 6865 2068 6561 6465 7273 206e 6565 6465  he headers neede
+000001f0: 6420 746f 206d 616b 6520 6120 7265 7175  d to make a requ
+00000200: 6573 7420 746f 2074 6865 2073 6572 7665  est to the serve
+00000210: 720a 0a20 2020 2052 6574 7572 6e73 3a0a  r..    Returns:.
+00000220: 2020 2020 2020 2020 6469 6374 3a20 5468          dict: Th
+00000230: 6520 3150 6173 7377 6f72 6420 436f 6e6e  e 1Password Conn
+00000240: 6563 7420 4150 4920 7265 7175 6573 7420  ect API request 
+00000250: 6865 6164 6572 730a 2020 2020 2222 220a  headers.    """.
+00000260: 2020 2020 7265 7475 726e 207b 2241 7574      return {"Aut
+00000270: 686f 7269 7a61 7469 6f6e 223a 2066 2242  horization": f"B
+00000280: 6561 7265 7220 7b74 6f6b 656e 7d22 2c20  earer {token}", 
+00000290: 2243 6f6e 7465 6e74 2d54 7970 6522 3a20  "Content-Type": 
+000002a0: 2261 7070 6c69 6361 7469 6f6e 2f6a 736f  "application/jso
+000002b0: 6e22 7d0a 0a0a 636c 6173 7320 5061 7468  n"}...class Path
+000002c0: 4275 696c 6465 723a 0a20 2020 2064 6566  Builder:.    def
+000002d0: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
+000002e0: 7665 7273 696f 6e3a 2073 7472 203d 2022  version: str = "
+000002f0: 2f76 3122 293a 0a20 2020 2020 2020 2073  /v1"):.        s
+00000300: 656c 662e 7061 7468 3a20 7374 7220 3d20  elf.path: str = 
+00000310: 7665 7273 696f 6e0a 0a20 2020 2064 6566  version..    def
+00000320: 2062 7569 6c64 2873 656c 6629 202d 3e20   build(self) -> 
+00000330: 7374 723a 0a20 2020 2020 2020 2072 6574  str:.        ret
+00000340: 7572 6e20 7365 6c66 2e70 6174 680a 0a20  urn self.path.. 
+00000350: 2020 2064 6566 2076 6175 6c74 7328 7365     def vaults(se
 00000360: 6c66 2c20 7575 6964 3a20 7374 7220 3d20  lf, uuid: str = 
 00000370: 4e6f 6e65 2920 2d3e 2027 5061 7468 4275  None) -> 'PathBu
 00000380: 696c 6465 7227 3a0a 2020 2020 2020 2020  ilder':.        
 00000390: 7365 6c66 2e5f 6170 7065 6e64 5f70 6174  self._append_pat
-000003a0: 6828 2269 7465 6d73 2229 0a20 2020 2020  h("items").     
-000003b0: 2020 2069 6620 7575 6964 2069 7320 6e6f     if uuid is no
-000003c0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000003d0: 2020 2020 7365 6c66 2e5f 6170 7065 6e64      self._append
-000003e0: 5f70 6174 6828 7575 6964 290a 2020 2020  _path(uuid).    
-000003f0: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
-00000400: 0a20 2020 2064 6566 2066 696c 6573 2873  .    def files(s
-00000410: 656c 662c 2075 7569 643a 2073 7472 203d  elf, uuid: str =
-00000420: 204e 6f6e 6529 202d 3e20 2750 6174 6842   None) -> 'PathB
-00000430: 7569 6c64 6572 273a 0a20 2020 2020 2020  uilder':.       
-00000440: 2073 656c 662e 5f61 7070 656e 645f 7061   self._append_pa
-00000450: 7468 2822 6669 6c65 7322 290a 2020 2020  th("files").    
-00000460: 2020 2020 6966 2075 7569 6420 6973 206e      if uuid is n
-00000470: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00000480: 2020 2020 2073 656c 662e 5f61 7070 656e       self._appen
-00000490: 645f 7061 7468 2875 7569 6429 0a20 2020  d_path(uuid).   
-000004a0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-000004b0: 0a0a 2020 2020 6465 6620 636f 6e74 656e  ..    def conten
-000004c0: 7428 7365 6c66 2920 2d3e 2027 5061 7468  t(self) -> 'Path
-000004d0: 4275 696c 6465 7227 3a0a 2020 2020 2020  Builder':.      
-000004e0: 2020 7365 6c66 2e5f 6170 7065 6e64 5f70    self._append_p
-000004f0: 6174 6828 2263 6f6e 7465 6e74 2229 0a20  ath("content"). 
-00000500: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00000510: 6c66 0a0a 2020 2020 6465 6620 7175 6572  lf..    def quer
-00000520: 7928 7365 6c66 2c20 6b65 793a 2073 7472  y(self, key: str
-00000530: 2c20 7661 6c75 653a 2073 7472 2920 2d3e  , value: str) ->
-00000540: 2027 5061 7468 4275 696c 6465 7227 3a0a   'PathBuilder':.
-00000550: 2020 2020 2020 2020 6b65 795f 7661 6c75          key_valu
-00000560: 655f 7061 6972 203d 2066 227b 6b65 797d  e_pair = f"{key}
-00000570: 3d7b 7661 6c75 657d 220a 2020 2020 2020  ={value}".      
-00000580: 2020 7365 6c66 2e5f 6170 7065 6e64 5f70    self._append_p
-00000590: 6174 6828 7175 6572 793d 6b65 795f 7661  ath(query=key_va
-000005a0: 6c75 655f 7061 6972 290a 2020 2020 2020  lue_pair).      
-000005b0: 2020 7265 7475 726e 2073 656c 660a 0a20    return self.. 
-000005c0: 2020 2064 6566 205f 6170 7065 6e64 5f70     def _append_p
-000005d0: 6174 6828 7365 6c66 2c20 7061 7468 5f63  ath(self, path_c
-000005e0: 6875 6e6b 3a20 7374 7220 3d20 4e6f 6e65  hunk: str = None
-000005f0: 2c20 7175 6572 793a 2073 7472 203d 204e  , query: str = N
-00000600: 6f6e 6529 202d 3e20 2750 6174 6842 7569  one) -> 'PathBui
-00000610: 6c64 6572 273a 0a20 2020 2020 2020 2069  lder':.        i
-00000620: 6620 7061 7468 5f63 6875 6e6b 2069 7320  f path_chunk is 
-00000630: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00000640: 2020 2020 2020 7365 6c66 2e70 6174 6820        self.path 
-00000650: 2b3d 2066 222f 7b70 6174 685f 6368 756e  += f"/{path_chun
-00000660: 6b7d 220a 2020 2020 2020 2020 6966 2071  k}".        if q
-00000670: 7565 7279 2069 7320 6e6f 7420 4e6f 6e65  uery is not None
-00000680: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00000690: 6c66 2e70 6174 6820 2b3d 2066 223f 7b71  lf.path += f"?{q
-000006a0: 7565 7279 7d22 0a                        uery}".
+000003a0: 6828 2276 6175 6c74 7322 290a 2020 2020  h("vaults").    
+000003b0: 2020 2020 6966 2075 7569 6420 6973 206e      if uuid is n
+000003c0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000003d0: 2020 2020 2073 656c 662e 5f61 7070 656e       self._appen
+000003e0: 645f 7061 7468 2875 7569 6429 0a20 2020  d_path(uuid).   
+000003f0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00000400: 0a0a 2020 2020 6465 6620 6974 656d 7328  ..    def items(
+00000410: 7365 6c66 2c20 7575 6964 3a20 7374 7220  self, uuid: str 
+00000420: 3d20 4e6f 6e65 2920 2d3e 2027 5061 7468  = None) -> 'Path
+00000430: 4275 696c 6465 7227 3a0a 2020 2020 2020  Builder':.      
+00000440: 2020 7365 6c66 2e5f 6170 7065 6e64 5f70    self._append_p
+00000450: 6174 6828 2269 7465 6d73 2229 0a20 2020  ath("items").   
+00000460: 2020 2020 2069 6620 7575 6964 2069 7320       if uuid is 
+00000470: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00000480: 2020 2020 2020 7365 6c66 2e5f 6170 7065        self._appe
+00000490: 6e64 5f70 6174 6828 7575 6964 290a 2020  nd_path(uuid).  
+000004a0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+000004b0: 660a 0a20 2020 2064 6566 2066 696c 6573  f..    def files
+000004c0: 2873 656c 662c 2075 7569 643a 2073 7472  (self, uuid: str
+000004d0: 203d 204e 6f6e 6529 202d 3e20 2750 6174   = None) -> 'Pat
+000004e0: 6842 7569 6c64 6572 273a 0a20 2020 2020  hBuilder':.     
+000004f0: 2020 2073 656c 662e 5f61 7070 656e 645f     self._append_
+00000500: 7061 7468 2822 6669 6c65 7322 290a 2020  path("files").  
+00000510: 2020 2020 2020 6966 2075 7569 6420 6973        if uuid is
+00000520: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00000530: 2020 2020 2020 2073 656c 662e 5f61 7070         self._app
+00000540: 656e 645f 7061 7468 2875 7569 6429 0a20  end_path(uuid). 
+00000550: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00000560: 6c66 0a0a 2020 2020 6465 6620 636f 6e74  lf..    def cont
+00000570: 656e 7428 7365 6c66 2920 2d3e 2027 5061  ent(self) -> 'Pa
+00000580: 7468 4275 696c 6465 7227 3a0a 2020 2020  thBuilder':.    
+00000590: 2020 2020 7365 6c66 2e5f 6170 7065 6e64      self._append
+000005a0: 5f70 6174 6828 2263 6f6e 7465 6e74 2229  _path("content")
+000005b0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000005c0: 7365 6c66 0a0a 2020 2020 6465 6620 7175  self..    def qu
+000005d0: 6572 7928 7365 6c66 2c20 6b65 793a 2073  ery(self, key: s
+000005e0: 7472 2c20 7661 6c75 653a 2073 7472 2920  tr, value: str) 
+000005f0: 2d3e 2027 5061 7468 4275 696c 6465 7227  -> 'PathBuilder'
+00000600: 3a0a 2020 2020 2020 2020 6b65 795f 7661  :.        key_va
+00000610: 6c75 655f 7061 6972 203d 2066 227b 6b65  lue_pair = f"{ke
+00000620: 797d 3d7b 7661 6c75 657d 220a 2020 2020  y}={value}".    
+00000630: 2020 2020 7365 6c66 2e5f 6170 7065 6e64      self._append
+00000640: 5f70 6174 6828 7175 6572 793d 6b65 795f  _path(query=key_
+00000650: 7661 6c75 655f 7061 6972 290a 2020 2020  value_pair).    
+00000660: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
+00000670: 0a20 2020 2064 6566 205f 6170 7065 6e64  .    def _append
+00000680: 5f70 6174 6828 7365 6c66 2c20 7061 7468  _path(self, path
+00000690: 5f63 6875 6e6b 3a20 7374 7220 3d20 4e6f  _chunk: str = No
+000006a0: 6e65 2c20 7175 6572 793a 2073 7472 203d  ne, query: str =
+000006b0: 204e 6f6e 6529 202d 3e20 2750 6174 6842   None) -> 'PathB
+000006c0: 7569 6c64 6572 273a 0a20 2020 2020 2020  uilder':.       
+000006d0: 2069 6620 7061 7468 5f63 6875 6e6b 2069   if path_chunk i
+000006e0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000006f0: 2020 2020 2020 2020 7365 6c66 2e70 6174          self.pat
+00000700: 6820 2b3d 2066 222f 7b70 6174 685f 6368  h += f"/{path_ch
+00000710: 756e 6b7d 220a 2020 2020 2020 2020 6966  unk}".        if
+00000720: 2071 7565 7279 2069 7320 6e6f 7420 4e6f   query is not No
+00000730: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00000740: 7365 6c66 2e70 6174 6820 2b3d 2066 223f  self.path += f"?
+00000750: 7b71 7565 7279 7d22 0a0a 0a64 6566 2067  {query}"...def g
+00000760: 6574 5f74 696d 656f 7574 2829 202d 3e20  et_timeout() -> 
+00000770: 556e 696f 6e5b 696e 742c 2055 7365 436c  Union[int, UseCl
+00000780: 6965 6e74 4465 6661 756c 745d 3a0a 2020  ientDefault]:.  
+00000790: 2020 2222 2247 6574 2074 6865 2074 696d    """Get the tim
+000007a0: 656f 7574 2074 6f20 6265 2075 7365 6420  eout to be used 
+000007b0: 696e 2074 6865 2048 5454 5020 436c 6965  in the HTTP Clie
+000007c0: 6e74 2222 220a 2020 2020 7469 6d65 6f75  nt""".    timeou
+000007d0: 7420 3d20 696e 7428 6f73 2e67 6574 656e  t = int(os.geten
+000007e0: 7628 454e 565f 434c 4945 4e54 5f52 4551  v(ENV_CLIENT_REQ
+000007f0: 5545 5354 5f54 494d 454f 5554 2c20 3029  UEST_TIMEOUT, 0)
+00000800: 290a 2020 2020 7265 7475 726e 2074 696d  ).    return tim
+00000810: 656f 7574 2069 6620 7469 6d65 6f75 7420  eout if timeout 
+00000820: 656c 7365 2055 5345 5f43 4c49 454e 545f  else USE_CLIENT_
+00000830: 4445 4641 554c 540a                      DEFAULT.
```

### Comparing `onepasswordconnectsdk-1.4.1/PKG-INFO` & `onepasswordconnectsdk-1.5.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onepasswordconnectsdk
-Version: 1.4.1
+Version: 1.5.0
 Summary: Python SDK for 1Password Connect
 Home-page: https://github.com/1Password/connect-sdk-python
 License: MIT
 Author: 1Password
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -50,14 +50,20 @@
 
 2. Export the `OP_CONNECT_HOST` and `OP_CONNECT_TOKEN` environment variables:
 
    ```sh
    export OP_CONNECT_HOST=<your-connect-host> && \
    export OP_CONNECT_TOKEN=<your-connect-token>
    ```
+   
+   2.1 If you need a higher timeout on the client requests you can export `OP_CLIENT_REQUEST_TIMEOUT` environment variable:
+   ```sh
+   # set the timeout to 90 seconds
+   export OP_CLIENT_REQUEST_TIMEOUT=90
+   ```
 
 3. Use the SDK:
 
    - Read a secret:
 
      ```python
      from onepasswordconnectsdk.client import (
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: onepasswordconnectsdk Version: 1.4.1 Summary:
+Metadata-Version: 2.1 Name: onepasswordconnectsdk Version: 1.5.0 Summary:
 Python SDK for 1Password Connect Home-page: https://github.com/1Password/
 connect-sdk-python License: MIT Author: 1Password Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
@@ -20,28 +20,30 @@
 infrastructure. The library is intended to be used by Python applications to
 simplify accessing items in 1Password vaults. ## ðª See it in action Check
 the [Python Connect SDK Example](example/README.md) to see an example of item
 manipulation using the SDK that you can execute on your machine. ## â¨ Get
 started 1. Install the 1Password Connect Python SDK: ```sh pip install
 onepasswordconnectsdk ``` 2. Export the `OP_CONNECT_HOST` and
 `OP_CONNECT_TOKEN` environment variables: ```sh export OP_CONNECT_HOST= && \
-export OP_CONNECT_TOKEN= ``` 3. Use the SDK: - Read a secret: ```python from
-onepasswordconnectsdk.client import ( Client, new_client_from_environment, )
-connect_client: Client = new_client_from_environment() client.get_item("
-{item_id}", "{vault_id}") ``` - Write a secret: ```python from
-onepasswordconnectsdk.client import ( Client, new_client_from_environment, }
-from onepasswordconnectsdk.models import ( Item, ItemVault, Field )
-connect_client: Client = new_client_from_environment() # Example item creation.
-Create an item with your desired arguments. item = Item( vault=ItemVault
-(id=op_vault), id="custom_id", title="newtitle", category="LOGIN", tags=
-["1password-connect"], fields=[Field(value="new_user", purpose="USERNAME")], )
-new_item = connect_client.create_item(op_vault, item) ``` For more examples of
-how to use the SDK, check out [USAGE.md](USAGE.md). ## ð Community & Support
-- File an [issue](https://github.com/1Password/connect-sdk-python/issues) for
-bugs and feature requests. - Join the [Developer Slack workspace](https://
-join.slack.com/t/1password-devs/shared_invite/zt-1halo11ps-
-6o9pEv96xZ3LtX_VE0fJQA). - Subscribe to the [Developer Newsletter](https://
-1password.com/dev-subscribe/). ## ð Security 1Password requests you practice
-responsible disclosure if you discover a vulnerability. Please file requests
-via [**BugCrowd**](https://bugcrowd.com/agilebits). For information about
-security practices, please visit the [1Password Bug Bounty Program](https://
-bugcrowd.com/agilebits).
+export OP_CONNECT_TOKEN= ``` 2.1 If you need a higher timeout on the client
+requests you can export `OP_CLIENT_REQUEST_TIMEOUT` environment variable: ```sh
+# set the timeout to 90 seconds export OP_CLIENT_REQUEST_TIMEOUT=90 ``` 3. Use
+the SDK: - Read a secret: ```python from onepasswordconnectsdk.client import
+( Client, new_client_from_environment, ) connect_client: Client =
+new_client_from_environment() client.get_item("{item_id}", "{vault_id}") ``` -
+Write a secret: ```python from onepasswordconnectsdk.client import ( Client,
+new_client_from_environment, } from onepasswordconnectsdk.models import ( Item,
+ItemVault, Field ) connect_client: Client = new_client_from_environment() #
+Example item creation. Create an item with your desired arguments. item = Item
+( vault=ItemVault(id=op_vault), id="custom_id", title="newtitle",
+category="LOGIN", tags=["1password-connect"], fields=[Field(value="new_user",
+purpose="USERNAME")], ) new_item = connect_client.create_item(op_vault, item)
+``` For more examples of how to use the SDK, check out [USAGE.md](USAGE.md). ##
+ð Community & Support - File an [issue](https://github.com/1Password/
+connect-sdk-python/issues) for bugs and feature requests. - Join the [Developer
+Slack workspace](https://join.slack.com/t/1password-devs/shared_invite/zt-
+1halo11ps-6o9pEv96xZ3LtX_VE0fJQA). - Subscribe to the [Developer Newsletter]
+(https://1password.com/dev-subscribe/). ## ð Security 1Password requests you
+practice responsible disclosure if you discover a vulnerability. Please file
+requests via [**BugCrowd**](https://bugcrowd.com/agilebits). For information
+about security practices, please visit the [1Password Bug Bounty Program]
+(https://bugcrowd.com/agilebits).
```

