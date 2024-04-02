# Comparing `tmp/pyglass_api-0.2.1.tar.gz` & `tmp/pyglass_api-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyglass_api-0.2.1.tar", max compression
+gzip compressed data, was "pyglass_api-0.3.0.tar", max compression
```

## Comparing `pyglass_api-0.2.1.tar` & `pyglass_api-0.3.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1069 2023-12-01 15:26:42.699857 pyglass_api-0.2.1/LICENSE
--rw-r--r--   0        0        0      228 2023-12-01 15:26:42.699857 pyglass_api-0.2.1/README.md
--rw-r--r--   0        0        0       42 2023-12-01 15:26:42.703857 pyglass_api-0.2.1/pyglass/__init__.py
--rw-r--r--   0        0        0      267 2023-12-01 15:26:42.703857 pyglass_api-0.2.1/pyglass/account/__init__.py
--rw-r--r--   0        0        0     2031 2023-12-01 15:26:42.703857 pyglass_api-0.2.1/pyglass/account/account_types.py
--rw-r--r--   0        0        0     7477 2023-12-01 15:26:42.703857 pyglass_api-0.2.1/pyglass/account/main.py
--rw-r--r--   0        0        0      108 2023-12-01 15:26:42.703857 pyglass_api-0.2.1/pyglass/block/__init__.py
--rw-r--r--   0        0        0      545 2023-12-01 15:26:42.703857 pyglass_api-0.2.1/pyglass/block/block_types.py
--rw-r--r--   0        0        0     1297 2023-12-01 15:26:42.703857 pyglass_api-0.2.1/pyglass/block/main.py
--rw-r--r--   0        0        0      228 2023-12-01 15:26:42.703857 pyglass_api-0.2.1/pyglass/distribution/__init__.py
--rw-r--r--   0        0        0     1211 2023-12-01 15:26:42.703857 pyglass_api-0.2.1/pyglass/distribution/distribution_types.py
--rw-r--r--   0        0        0     4270 2023-12-01 15:26:42.703857 pyglass_api-0.2.1/pyglass/distribution/main.py
--rw-r--r--   0        0        0       48 2023-12-01 15:26:42.703857 pyglass_api-0.2.1/pyglass/exceptions.py
--rw-r--r--   0        0        0      125 2023-12-01 15:26:42.703857 pyglass_api-0.2.1/pyglass/known/__init__.py
--rw-r--r--   0        0        0      196 2023-12-01 15:26:42.703857 pyglass_api-0.2.1/pyglass/known/known_types.py
--rw-r--r--   0        0        0     1146 2023-12-01 15:26:42.703857 pyglass_api-0.2.1/pyglass/known/main.py
--rw-r--r--   0        0        0      194 2023-12-01 15:26:42.703857 pyglass_api-0.2.1/pyglass/network/__init__.py
--rw-r--r--   0        0        0     2345 2023-12-01 15:26:42.703857 pyglass_api-0.2.1/pyglass/network/main.py
--rw-r--r--   0        0        0      800 2023-12-01 15:26:42.703857 pyglass_api-0.2.1/pyglass/network/network_types.py
--rw-r--r--   0        0        0      239 2023-12-01 15:26:42.703857 pyglass_api-0.2.1/pyglass/representatives/__init__.py
--rw-r--r--   0        0        0    12239 2023-12-01 15:26:42.703857 pyglass_api-0.2.1/pyglass/representatives/main.py
--rw-r--r--   0        0        0     3301 2023-12-01 15:26:42.703857 pyglass_api-0.2.1/pyglass/representatives/representatives_types.py
--rw-r--r--   0        0        0      471 2023-12-01 15:26:42.703857 pyglass_api-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      834 1970-01-01 00:00:00.000000 pyglass_api-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-02 13:04:01.164946 pyglass_api-0.3.0/LICENSE
+-rw-r--r--   0        0        0      374 2024-04-02 13:04:01.164946 pyglass_api-0.3.0/README.md
+-rw-r--r--   0        0        0      682 2024-04-02 13:04:01.168946 pyglass_api-0.3.0/pyglass/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-02 13:04:01.168946 pyglass_api-0.3.0/pyglass/account/__init__.py
+-rw-r--r--   0        0        0     2031 2024-04-02 13:04:01.168946 pyglass_api-0.3.0/pyglass/account/account_types.py
+-rw-r--r--   0        0        0     8343 2024-04-02 13:04:01.168946 pyglass_api-0.3.0/pyglass/account/main.py
+-rw-r--r--   0        0        0        0 2024-04-02 13:04:01.168946 pyglass_api-0.3.0/pyglass/block/__init__.py
+-rw-r--r--   0        0        0      545 2024-04-02 13:04:01.168946 pyglass_api-0.3.0/pyglass/block/block_types.py
+-rw-r--r--   0        0        0     1524 2024-04-02 13:04:01.168946 pyglass_api-0.3.0/pyglass/block/main.py
+-rw-r--r--   0        0        0        0 2024-04-02 13:04:01.168946 pyglass_api-0.3.0/pyglass/distribution/__init__.py
+-rw-r--r--   0        0        0     1211 2024-04-02 13:04:01.168946 pyglass_api-0.3.0/pyglass/distribution/distribution_types.py
+-rw-r--r--   0        0        0     4954 2024-04-02 13:04:01.168946 pyglass_api-0.3.0/pyglass/distribution/main.py
+-rw-r--r--   0        0        0       48 2024-04-02 13:04:01.168946 pyglass_api-0.3.0/pyglass/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-02 13:04:01.168946 pyglass_api-0.3.0/pyglass/known/__init__.py
+-rw-r--r--   0        0        0      196 2024-04-02 13:04:01.168946 pyglass_api-0.3.0/pyglass/known/known_types.py
+-rw-r--r--   0        0        0     1383 2024-04-02 13:04:01.168946 pyglass_api-0.3.0/pyglass/known/main.py
+-rw-r--r--   0        0        0        0 2024-04-02 13:04:01.168946 pyglass_api-0.3.0/pyglass/network/__init__.py
+-rw-r--r--   0        0        0     2709 2024-04-02 13:04:01.168946 pyglass_api-0.3.0/pyglass/network/main.py
+-rw-r--r--   0        0        0      800 2024-04-02 13:04:01.168946 pyglass_api-0.3.0/pyglass/network/network_types.py
+-rw-r--r--   0        0        0        0 2024-04-02 13:04:01.168946 pyglass_api-0.3.0/pyglass/representatives/__init__.py
+-rw-r--r--   0        0        0    13767 2024-04-02 13:04:01.168946 pyglass_api-0.3.0/pyglass/representatives/main.py
+-rw-r--r--   0        0        0     3301 2024-04-02 13:04:01.168946 pyglass_api-0.3.0/pyglass/representatives/representatives_types.py
+-rw-r--r--   0        0        0      526 2024-04-02 13:04:01.168946 pyglass_api-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      980 1970-01-01 00:00:00.000000 pyglass_api-0.3.0/PKG-INFO
```

### Comparing `pyglass_api-0.2.1/LICENSE` & `pyglass_api-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyglass_api-0.2.1/pyglass/account/account_types.py` & `pyglass_api-0.3.0/pyglass/account/account_types.py`

 * *Files identical despite different names*

### Comparing `pyglass_api-0.2.1/pyglass/account/main.py` & `pyglass_api-0.3.0/pyglass/account/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,207 +1,196 @@
 from typing import Union
 
 from requests import get, post
 
-from .. import SpyglassException
-from .account_types import (
-    ConfirmedTX,
-    Delegator,
-    Delegators,
-    Insights,
-    Overview,
-    ReceivableTX,
-)
-
-ACCOUNT_URL = "https://api.spyglass.pw/banano/v1/account/"
-
-
-def get_confirmed_transactions(
-    address: str,
-    filter_addresses: list[str] = None,
-    include_change: bool = True,
-    include_receive: bool = True,
-    include_send: bool = True,
-    max_amount: Union[int, float] = None,
-    min_amount: Union[int, float] = None,
-    offset: int = 0,
-    size: int = 25,
-) -> list[ConfirmedTX]:
-    """
-    `filter_addresses`: Only show transactions that include these addresses as sender, recipient, or new representative\n
-    `max_amount`: Maximum number sent/received to be included (not raw)\n
-    `min_amount`: Minimum number sent/received to be included (not raw)\n
-    `offset`: Results will be returned starting from this block height\n
-    `size`: Max number of blocks to return; defaults to include 25 with a max of 500\n
-    https://spyglass-api.web.app/account/confirmed
-    """
-    data = {
-        "address": address,
-        "filterAddresses": filter_addresses,
-        "includeChange": include_change,
-        "includeReceive": include_receive,
-        "includeSend": include_send,
-        "maxAmount": max_amount,
-        "minAmount": min_amount,
-        "offset": offset,
-        "size": size,
-    }
-    response = post(f"{ACCOUNT_URL}confirmed-transactions", json=data)
-
-    if not response.ok:
-        raise SpyglassException(response.json())
-
-    confirmed_tx: list[dict] = response.json()
-    return [
-        ConfirmedTX(
-            address=tx.get("address", None),
-            amount=tx.get("amount", None),
-            amount_raw=tx.get("amountRaw", None),
-            date=tx["date"],
-            hash=tx["hash"],
-            height=tx["height"],
-            new_representative=tx.get("newRepresentative", None),
-            timestamp=tx["timestamp"],
-            type=tx["type"],
+from pyglass.account import account_types
+from pyglass.exceptions import SpyglassException
+
+
+class Account:
+    def __init__(self, base_url: str):
+        self._account_url = f"{base_url}/v1/account/"
+
+    def get_confirmed_transactions(
+        self,
+        address: str,
+        filter_addresses: list[str] = None,
+        include_change: bool = True,
+        include_receive: bool = True,
+        include_send: bool = True,
+        max_amount: Union[int, float] = None,
+        min_amount: Union[int, float] = None,
+        offset: int = 0,
+        size: int = 25,
+    ) -> list[account_types.ConfirmedTX]:
+        """
+        `filter_addresses`: Only show transactions that include these addresses as sender, recipient, or new representative\n
+        `max_amount`: Maximum number sent/received to be included (not raw)\n
+        `min_amount`: Minimum number sent/received to be included (not raw)\n
+        `offset`: Results will be returned starting from this block height\n
+        `size`: Max number of blocks to return; defaults to include 25 with a max of 500\n
+        https://spyglass-api.web.app/account/confirmed
+        """
+        data = {
+            "address": address,
+            "filterAddresses": filter_addresses,
+            "includeChange": include_change,
+            "includeReceive": include_receive,
+            "includeSend": include_send,
+            "maxAmount": max_amount,
+            "minAmount": min_amount,
+            "offset": offset,
+            "size": size,
+        }
+        response = post(f"{self._account_url}confirmed-transactions", json=data)
+
+        if not response.ok:
+            raise SpyglassException(response.json())
+
+        confirmed_tx: list[dict] = response.json()
+        return [
+            account_types.ConfirmedTX(
+                address=tx.get("address", None),
+                amount=tx.get("amount", None),
+                amount_raw=tx.get("amountRaw", None),
+                date=tx["date"],
+                hash=tx["hash"],
+                height=tx["height"],
+                new_representative=tx.get("newRepresentative", None),
+                timestamp=tx["timestamp"],
+                type=tx["type"],
+            )
+            for tx in confirmed_tx
+        ]
+
+    def get_delegators(
+        self,
+        address: str,
+        offset: int = 0,
+        size: int = 100,
+        threshold: Union[int, float] = 0.001,
+    ) -> account_types.Delegators:
+        """
+        `offset`: Skips the specified number of records in the result set. Used for pagination.\n
+        `size`: Number of delegators to return. Defaults to show 100 delegators.\n
+        `threshold`: Minimum required balance for a delegator to be included in the response.
+        This not in raw. Defaults to 0.0001.\n
+        https://spyglass-api.web.app/account/delegators
+        """
+        data = {"address": address, "offset": offset, "size": size, "threshold": threshold}
+        response = post(f"{self._account_url}delegators", json=data)
+
+        if not response.ok:
+            raise SpyglassException(response.json())
+
+        delegators = response.json()
+        return account_types.Delegators(
+            count=delegators["count"],
+            empty_count=delegators["emptyCount"],
+            weight_sum=delegators["weightSum"],
+            delegators=[
+                account_types.Delegator(delegator["address"], delegator["weight"])
+                for delegator in delegators["delegators"]
+            ],
         )
-        for tx in confirmed_tx
-    ]
 
+    def get_export(self, address: str):
+        """https://spyglass-api.web.app/account/export"""
+        data = {"address": address}
+        resppnse = post(f"{self._account_url}export", json=data)
+
+        if not resppnse.ok:
+            raise SpyglassException(resppnse.json())
+
+        return resppnse.json()
+
+    def get_insights(self, address: str, include_height_balances: bool = False) -> account_types.Insights:
+        """https://spyglass-api.web.app/account/insights"""
+        data = {"address": address, "includeHeightBalances": include_height_balances}
+        response = post(f"{self._account_url}insights", json=data)
+
+        if not response.ok:
+            raise SpyglassException(response.json())
+
+        insights: dict = response.json()
+        return account_types.Insights(
+            block_count=insights["blockCount"],
+            first_in_tx_hash=insights["firstInTxHash"],
+            first_in_tx_unix_timestamp=insights["firstInTxUnixTimestamp"],
+            first_out_tx_hash=insights.get("firstOutTxHash", None),
+            first_out_tx_unix_timestamp=insights.get("firstOutTxUnixTimestamp", None),
+            height_balances=list(insights["heightBalances"].values()) if insights.get("heightBalances", None) else None,
+            last_in_tx_hash=insights["lastInTxHash"],
+            last_in_tx_unix_timestamp=insights["lastInTxUnixTimestamp"],
+            last_out_tx_hash=insights.get("lastOutTxHash", None),
+            last_out_tx_unix_timestamp=insights.get("lastOutTxUnixTimestamp", None),
+            max_amount_received=insights["maxAmountReceived"],
+            max_amount_received_hash=insights["maxAmountReceivedHash"],
+            max_amount_sent=insights["maxAmountSent"],
+            max_amount_sent_hash=insights.get("maxAmountSentHash", None),
+            max_balance=insights["maxBalance"],
+            max_balance_hash=insights["maxBalanceHash"],
+            most_common_recipient_address=insights.get("mostCommonRecipientAddress", None),
+            most_common_recipient_tx_count=insights["mostCommonRecipientTxCount"],
+            most_common_sender_address=insights["mostCommonSenderAddress"],
+            most_common_sender_tx_count=insights["mostCommonSenderTxCount"],
+            total_amount_received=insights["totalAmountReceived"],
+            total_amount_sent=insights["totalAmountSent"],
+            total_tx_change=insights["totalTxChange"],
+            total_tx_received=insights["totalTxReceived"],
+            total_tx_sent=insights["totalTxSent"],
+        )
 
-def get_delegators(
-    address: str,
-    offset: int = 0,
-    size: int = 100,
-    threshold: Union[int, float] = 0.001,
-) -> Delegators:
-    """
-    `offset`: Skips the specified number of records in the result set. Used for pagination.\n
-    `size`: Number of delegators to return. Defaults to show 100 delegators.\n
-    `threshold`: Minimum required balance for a delegator to be included in the response.
-    This not in raw. Defaults to 0.0001.\n
-    https://spyglass-api.web.app/account/delegators
-    """
-    data = {"address": address, "offset": offset, "size": size, "threshold": threshold}
-    response = post(f"{ACCOUNT_URL}delegators", json=data)
-
-    if not response.ok:
-        raise SpyglassException(response.json())
-
-    delegators = response.json()
-    return Delegators(
-        count=delegators["count"],
-        empty_count=delegators["emptyCount"],
-        weight_sum=delegators["weightSum"],
-        delegators=[
-            Delegator(delegator["address"], delegator["weight"])
-            for delegator in delegators["delegators"]
-        ],
-    )
-
-
-def get_export(address: str):
-    """https://spyglass-api.web.app/account/export"""
-    data = {"address": address}
-    resppnse = post(f"{ACCOUNT_URL}export", json=data)
-
-    if not resppnse.ok:
-        raise SpyglassException(resppnse.json())
-
-    return resppnse.json()
-
-
-def get_insights(address: str, include_height_balances: bool = False) -> Insights:
-    """https://spyglass-api.web.app/account/insights"""
-    data = {"address": address, "includeHeightBalances": include_height_balances}
-    response = post(f"{ACCOUNT_URL}insights", json=data)
-
-    if not response.ok:
-        raise SpyglassException(response.json())
-
-    insights: dict = response.json()
-    return Insights(
-        block_count=insights["blockCount"],
-        first_in_tx_hash=insights["firstInTxHash"],
-        first_in_tx_unix_timestamp=insights["firstInTxUnixTimestamp"],
-        first_out_tx_hash=insights.get("firstOutTxHash", None),
-        first_out_tx_unix_timestamp=insights.get("firstOutTxUnixTimestamp", None),
-        height_balances=list(insights["heightBalances"].values())
-        if insights.get("heightBalances", None)
-        else None,
-        last_in_tx_hash=insights["lastInTxHash"],
-        last_in_tx_unix_timestamp=insights["lastInTxUnixTimestamp"],
-        last_out_tx_hash=insights.get("lastOutTxHash", None),
-        last_out_tx_unix_timestamp=insights.get("lastOutTxUnixTimestamp", None),
-        max_amount_received=insights["maxAmountReceived"],
-        max_amount_received_hash=insights["maxAmountReceivedHash"],
-        max_amount_sent=insights["maxAmountSent"],
-        max_amount_sent_hash=insights.get("maxAmountSentHash", None),
-        max_balance=insights["maxBalance"],
-        max_balance_hash=insights["maxBalanceHash"],
-        most_common_recipient_address=insights.get("mostCommonRecipientAddress", None),
-        most_common_recipient_tx_count=insights["mostCommonRecipientTxCount"],
-        most_common_sender_address=insights["mostCommonSenderAddress"],
-        most_common_sender_tx_count=insights["mostCommonSenderTxCount"],
-        total_amount_received=insights["totalAmountReceived"],
-        total_amount_sent=insights["totalAmountSent"],
-        total_tx_change=insights["totalTxChange"],
-        total_tx_received=insights["totalTxReceived"],
-        total_tx_sent=insights["totalTxSent"],
-    )
-
-
-def get_overview(address: str) -> Overview:
-    """https://spyglass-api.web.app/account/overview"""
-    response = get(f"{ACCOUNT_URL}overview/{address}")
-
-    if not response.ok:
-        raise SpyglassException(response.json())
-
-    overview: dict = response.json()
-    return Overview(
-        address=overview["address"],
-        balance=overview.get("balance", None),
-        balance_raw=overview.get("balanceRaw", None),
-        block_count=overview["blockCount"],
-        delegators_count=overview["delegatorsCount"],
-        opened=overview["opened"],
-        principal=overview["principal"],
-        receivable=overview["receivable"],
-        receivable_raw=overview["receivableRaw"],
-        representative=overview.get("representative", None),
-        weight=overview.get("weight", None),
-    )
-
-
-def get_representative(address: str) -> str:
-    """https://spyglass-api.web.app/account/representative"""
-    response = get(f"{ACCOUNT_URL}representative/{address}")
-
-    if not response.ok:
-        raise SpyglassException(response.json())
-
-    return response.json()["representative"]
-
-
-def get_receivable_transactions(
-    address: str, offset: int = 0, size: int = 50
-) -> list[ReceivableTX]:
-    """
-    `offset`: Skips the specified number of records in the result set. Used for pagination.\n
-    `size`: Number of receivable transactions to return; Defaults to include 50 with a max of 500.\n
-    https://spyglass-api.web.app/account/receivable
-    """
-    data = {"address": address, "offset": offset, "size": size}
-    response = post(f"{ACCOUNT_URL}receivable-transactions", json=data)
-    if not response.ok:
-        raise SpyglassException(response.json())
-
-    return [
-        ReceivableTX(
-            address=transaction["address"],
-            amount=transaction["amount"],
-            amount_raw=transaction["amountRaw"],
-            hash=transaction["hash"],
-            timestamp=transaction["timestamp"],
+    def get_overview(self, address: str) -> account_types.Overview:
+        """https://spyglass-api.web.app/account/overview"""
+        response = get(f"{self._account_url}overview/{address}")
+
+        if not response.ok:
+            raise SpyglassException(response.json())
+
+        overview: dict = response.json()
+        return account_types.Overview(
+            address=overview["address"],
+            balance=overview.get("balance", None),
+            balance_raw=overview.get("balanceRaw", None),
+            block_count=overview["blockCount"],
+            delegators_count=overview["delegatorsCount"],
+            opened=overview["opened"],
+            principal=overview["principal"],
+            receivable=overview["receivable"],
+            receivable_raw=overview["receivableRaw"],
+            representative=overview.get("representative", None),
+            weight=overview.get("weight", None),
         )
-        for transaction in response.json()
-    ]
+
+    def get_representative(self, address: str) -> str:
+        """https://spyglass-api.web.app/account/representative"""
+        response = get(f"{self._account_url}representative/{address}")
+
+        if not response.ok:
+            raise SpyglassException(response.json())
+
+        return response.json()["representative"]
+
+    def get_receivable_transactions(
+        self, address: str, offset: int = 0, size: int = 50
+    ) -> list[account_types.ReceivableTX]:
+        """
+        `offset`: Skips the specified number of records in the result set. Used for pagination.\n
+        `size`: Number of receivable transactions to return; Defaults to include 50 with a max of 500.\n
+        https://spyglass-api.web.app/account/receivable
+        """
+        data = {"address": address, "offset": offset, "size": size}
+        response = post(f"{self._account_url}receivable-transactions", json=data)
+        if not response.ok:
+            raise SpyglassException(response.json())
+
+        return [
+            account_types.ReceivableTX(
+                address=transaction["address"],
+                amount=transaction["amount"],
+                amount_raw=transaction["amountRaw"],
+                hash=transaction["hash"],
+                timestamp=transaction["timestamp"],
+            )
+            for transaction in response.json()
+        ]
```

### Comparing `pyglass_api-0.2.1/pyglass/block/block_types.py` & `pyglass_api-0.3.0/pyglass/block/block_types.py`

 * *Files identical despite different names*

### Comparing `pyglass_api-0.2.1/pyglass/block/main.py` & `pyglass_api-0.3.0/pyglass/block/main.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 from requests import get
 
-from .. import SpyglassException
-from .block_types import Block, BlockContents
+from pyglass.block import block_types
+from pyglass.exceptions import SpyglassException
 
-BLOCK_URL = "https://api.spyglass.pw/banano/v1/block/"
 
-
-def get_block(block_hash: str) -> Block:
-    """https://spyglass-api.web.app/account/block"""
-    response = get(f"{BLOCK_URL}{block_hash}")
-
-    if not response.ok:
-        raise SpyglassException(response.json())
-
-    block = response.json()
-    block_contents = block["contents"]
-    return Block(
-        amount=block["amount"],
-        amount_raw=block["amountRaw"],
-        balance=block["balance"],
-        block_account=block["blockAccount"],
-        confirmed=bool(block["confirmed"]),
-        contents=BlockContents(
-            account=block_contents["account"],
-            balance=block_contents["balance"],
-            link=block_contents["link"],
-            link_as_account=block_contents["linkAsAccount"],
-            previous=block_contents["previous"],
-            representative=block_contents["representative"],
-            signature=block_contents["signature"],
-            type=block_contents["type"],
-            work=block_contents["work"],
-        ),
-        height=block["height"],
-        source_account=block["sourceAccount"],
-        subtype=block["subtype"],
-        timestamp=block["timestamp"],
-    )
+class Block:
+    def __init__(self, base_url: str) -> None:
+        self._block_url = f"{base_url}/v1/block/"
+
+    def get_block(self, block_hash: str) -> block_types.Block:
+        """https://spyglass-api.web.app/account/block"""
+        response = get(f"{self._block_url}{block_hash}")
+
+        if not response.ok:
+            raise SpyglassException(response.json())
+
+        block = response.json()
+        block_contents = block["contents"]
+        return block_types.Block(
+            amount=block["amount"],
+            amount_raw=block["amountRaw"],
+            balance=block["balance"],
+            block_account=block["blockAccount"],
+            confirmed=bool(block["confirmed"]),
+            contents=block_types.BlockContents(
+                account=block_contents["account"],
+                balance=block_contents["balance"],
+                link=block_contents["link"],
+                link_as_account=block_contents["linkAsAccount"],
+                previous=block_contents["previous"],
+                representative=block_contents["representative"],
+                signature=block_contents["signature"],
+                type=block_contents["type"],
+                work=block_contents["work"],
+            ),
+            height=block["height"],
+            source_account=block["sourceAccount"],
+            subtype=block["subtype"],
+            timestamp=block["timestamp"],
+        )
```

### Comparing `pyglass_api-0.2.1/pyglass/distribution/distribution_types.py` & `pyglass_api-0.3.0/pyglass/distribution/distribution_types.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from typing import Optional, Union
 from dataclasses import dataclass
+from typing import Optional, Union
 
 
 @dataclass(frozen=True, order=True)
 class BurnAccount:
     address: str
     pending: int
```

### Comparing `pyglass_api-0.2.1/pyglass/distribution/main.py` & `pyglass_api-0.3.0/pyglass/distribution/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,136 +1,123 @@
 from requests import get, post
 
-from .. import SpyglassException
-from .distribution_types import (
-    Buckets,
-    Burn,
-    BurnAccount,
-    DeveloperFunds,
-    DeveloperWallet,
-    RichListItem,
-    Supply,
-)
-
-DISTRIBUTION_URL = "https://api.spyglass.pw/banano/v1/distribution/"
-
-
-def get_burn() -> Burn:
-    """https://spyglass-api.web.app/distribution/burn"""
-    response = get(f"{DISTRIBUTION_URL}burn")
-    if not response.ok:
-        raise SpyglassException(response.json())
-
-    burn = response.json()
-    return Burn(
-        total_amount=burn["totalAmount"],
-        burn_accounts=[
-            BurnAccount(
-                address=burn_account["address"], pending=burn_account["pending"]
-            )
-            for burn_account in burn["burnAccounts"]
-        ],
-    )
-
-
-def get_buckets() -> Buckets:
-    """https://spyglass-api.web.app/distribution/buckets"""
-    response = get(f"{DISTRIBUTION_URL}buckets")
-    if not response.ok:
-        raise SpyglassException(response.json())
-
-    buckets = response.json()
-    return Buckets(
-        number0_0001=buckets["number0_0001"],
-        number0_001=buckets["number0_001"],
-        number0_01=buckets["number0_01"],
-        number0_1=buckets["number0_1"],
-        number1=buckets["number1"],
-        number10=buckets["number10"],
-        number100=buckets["number100"],
-        number100_000=buckets["number100_000"],
-        number100_000_000=buckets["number100_000_000"],
-        number10_000=buckets["number10_000"],
-        number10_000_000=buckets["number10_000_000"],
-        number1_000=buckets["number1_000"],
-        number1_000_000=buckets["number1_000_000"],
-        total_accounts=buckets["totalAccounts"],
-    )
-
-
-def get_developer_funds() -> DeveloperFunds:
-    """https://spyglass-api.web.app/distribution/developer-funds"""
-    response = get(f"{DISTRIBUTION_URL}developer-funds")
-    if not response.ok:
-        raise SpyglassException(response.json())
-
-    dev_funds = response.json()
-    return DeveloperFunds(
-        total_balance=dev_funds["totalBalance"],
-        wallets=[
-            DeveloperWallet(address=wallet["address"], balance=wallet["balance"])
-            for wallet in dev_funds["wallets"]
-        ],
-    )
-
-
-def get_rich_list(
-    include_representative: bool = False, offset: int = 0, size: int = 50
-) -> list[RichListItem]:
-    """
-    `include_representative`: Optionally include the representative for each account.\n
-    `offset`: Number of accounts to skip before returning results; used for pagination.\n
-    `size`: Number of records to return, with a default of 50 and max of 500.\n
-    https://spyglass-api.web.app/distribution/rich-list
-    """
-    data = {
-        "includeRepresentative": include_representative,
-        "offset": offset,
-        "size": size,
-    }
-    response = post(f"{DISTRIBUTION_URL}rich-list", json=data)
-    if not response.ok:
-        raise SpyglassException(response.json())
-
-    rich_list: list[dict] = response.json()
-    return [
-        RichListItem(
-            address=item["address"],
-            amount=item["amount"],
-            representative=item.get("representative", None),
+from pyglass.distribution import distribution_types
+from pyglass.exceptions import SpyglassException
+
+
+class Distribution:
+    def __init__(self, base_url: str) -> None:
+        self._distribution_url = f"{base_url}/v1/distribution/"
+
+    def get_burn(self) -> distribution_types.Burn:
+        """https://spyglass-api.web.app/distribution/burn"""
+        response = get(f"{self._distribution_url}burn")
+        if not response.ok:
+            raise SpyglassException(response.json())
+
+        burn = response.json()
+        return distribution_types.Burn(
+            total_amount=burn["totalAmount"],
+            burn_accounts=[
+                distribution_types.BurnAccount(address=burn_account["address"], pending=burn_account["pending"])
+                for burn_account in burn["burnAccounts"]
+            ],
         )
-        for item in rich_list
-    ]
 
+    def get_buckets(self) -> distribution_types.Buckets:
+        """https://spyglass-api.web.app/distribution/buckets"""
+        response = get(f"{self._distribution_url}buckets")
+        if not response.ok:
+            raise SpyglassException(response.json())
+
+        buckets = response.json()
+        return distribution_types.Buckets(
+            number0_0001=buckets["number0_0001"],
+            number0_001=buckets["number0_001"],
+            number0_01=buckets["number0_01"],
+            number0_1=buckets["number0_1"],
+            number1=buckets["number1"],
+            number10=buckets["number10"],
+            number100=buckets["number100"],
+            number100_000=buckets["number100_000"],
+            number100_000_000=buckets["number100_000_000"],
+            number10_000=buckets["number10_000"],
+            number10_000_000=buckets["number10_000_000"],
+            number1_000=buckets["number1_000"],
+            number1_000_000=buckets["number1_000_000"],
+            total_accounts=buckets["totalAccounts"],
+        )
 
-def get_rich_list_snapshot() -> list[RichListItem]:
-    """https://spyglass-api.web.app/distribution/rich-list-snapshot"""
-    response = get(f"{DISTRIBUTION_URL}rich-list-snapshot")
-    if not response.ok:
-        raise SpyglassException(response.json())
-
-    rich_list: list[dict] = response.json()
-    return [
-        RichListItem(
-            address=item["address"],
-            amount=item["amount"],
-            representative=item.get("representative", None),
+    def get_developer_funds(self) -> distribution_types.DeveloperFunds:
+        """https://spyglass-api.web.app/distribution/developer-funds"""
+        response = get(f"{self._distribution_url}developer-funds")
+        if not response.ok:
+            raise SpyglassException(response.json())
+
+        dev_funds = response.json()
+        return distribution_types.DeveloperFunds(
+            total_balance=dev_funds["totalBalance"],
+            wallets=[
+                distribution_types.DeveloperWallet(address=wallet["address"], balance=wallet["balance"])
+                for wallet in dev_funds["wallets"]
+            ],
         )
-        for item in rich_list
-    ]
 
+    def get_rich_list(
+        self, include_representative: bool = False, offset: int = 0, size: int = 50
+    ) -> list[distribution_types.RichListItem]:
+        """
+        `include_representative`: Optionally include the representative for each account.\n
+        `offset`: Number of accounts to skip before returning results; used for pagination.\n
+        `size`: Number of records to return, with a default of 50 and max of 500.\n
+        https://spyglass-api.web.app/distribution/rich-list
+        """
+        data = {
+            "includeRepresentative": include_representative,
+            "offset": offset,
+            "size": size,
+        }
+        response = post(f"{self._distribution_url}rich-list", json=data)
+        if not response.ok:
+            raise SpyglassException(response.json())
+
+        rich_list: list[dict] = response.json()
+        return [
+            distribution_types.RichListItem(
+                address=item["address"],
+                amount=item["amount"],
+                representative=item.get("representative", None),
+            )
+            for item in rich_list
+        ]
+
+    def get_rich_list_snapshot(self) -> list[distribution_types.RichListItem]:
+        """https://spyglass-api.web.app/distribution/rich-list-snapshot"""
+        response = get(f"{self._distribution_url}rich-list-snapshot")
+        if not response.ok:
+            raise SpyglassException(response.json())
+
+        rich_list: list[dict] = response.json()
+        return [
+            distribution_types.RichListItem(
+                address=item["address"],
+                amount=item["amount"],
+                representative=item.get("representative", None),
+            )
+            for item in rich_list
+        ]
 
-def get_supply() -> Supply:
-    """https://spyglass-api.web.app/distribution/supply"""
-    response = get(f"{DISTRIBUTION_URL}supply")
-    if not response.ok:
-        raise SpyglassException(response.json())
-
-    supply: dict = response.json()
-    return Supply(
-        burned_amount=supply["burnedAmount"],
-        circulating_amount=supply["circulatingAmount"],
-        circulating_percent=supply["circulatingPercent"],
-        dev_fund_amount=supply["devFundAmount"],
-        dev_fund_percent=supply["devFundPercent"],
-        total_amount=supply["totalAmount"],
-    )
+    def get_supply(self) -> distribution_types.Supply:
+        """https://spyglass-api.web.app/distribution/supply"""
+        response = get(f"{self._distribution_url}supply")
+        if not response.ok:
+            raise SpyglassException(response.json())
+
+        supply: dict = response.json()
+        return distribution_types.Supply(
+            burned_amount=supply["burnedAmount"],
+            circulating_amount=supply["circulatingAmount"],
+            circulating_percent=supply["circulatingPercent"],
+            dev_fund_amount=supply["devFundAmount"],
+            dev_fund_percent=supply["devFundPercent"],
+            total_amount=supply["totalAmount"],
+        )
```

### Comparing `pyglass_api-0.2.1/pyglass/known/main.py` & `pyglass_api-0.3.0/pyglass/known/main.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 from requests import get, post
 
-from .. import SpyglassException
-from .known_types import Account
+from pyglass.exceptions import SpyglassException
+from pyglass.known import known_types
 
-KNOWN_URL = "https://api.spyglass.pw/banano/v1/known/"
 
+class Known:
+    def __init__(self, base_url: str) -> None:
+        self._known_url = f"{base_url}/v1/known/"
+
+    def get_accounts(
+        self, include_owner: bool = False, include_type: bool = False, type_filter: str = None
+    ) -> list[known_types.Account]:
+        """https://spyglass-api.web.app/known/accounts"""
+        data = {
+            "includeOwner": include_owner,
+            "includeType": include_type,
+            "typeFilter": type_filter,
+        }
+        response = post(f"{self._known_url}accounts", json=data)
+        if not response.ok:
+            raise SpyglassException(response.text)
+
+        accounts: list[dict] = response.json()
+
+        return [
+            known_types.Account(
+                address=account["address"],
+                alias=account["alias"],
+                owner=account.get("owner", None),
+                type=account.get("type", None),
+            )
+            for account in accounts
+        ]
+
+    def get_vanities(self) -> list[str]:
+        """https://spyglass-api.web.app/known/vanities"""
+        response = get(f"{self._known_url}vanities")
+        if not response.ok:
+            raise SpyglassException(response.json())
 
-def get_accounts(
-    include_owner: bool = False, include_type: bool = False, type_filter: str = None
-) -> list[Account]:
-    """https://spyglass-api.web.app/known/accounts"""
-    data = {
-        "includeOwner": include_owner,
-        "includeType": include_type,
-        "typeFilter": type_filter,
-    }
-    response = post(f"{KNOWN_URL}accounts", json=data)
-    if not response.ok:
-        raise SpyglassException(response.text)
-
-    accounts: list[dict] = response.json()
-
-    return [
-        Account(
-            address=account["address"],
-            alias=account["alias"],
-            owner=account.get("owner", None),
-            type=account.get("type", None),
-        )
-        for account in accounts
-    ]
-
-
-def get_vanities() -> list[str]:
-    """https://spyglass-api.web.app/known/vanities"""
-    response = get(f"{KNOWN_URL}vanities")
-    if not response.ok:
-        raise SpyglassException(response.json())
-
-    vanities: list[str] = response.json()
-    return vanities
+        vanities: list[str] = response.json()
+        return vanities
```

### Comparing `pyglass_api-0.2.1/pyglass/network/main.py` & `pyglass_api-0.3.0/pyglass/network/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,67 +1,67 @@
 from typing import Union
-from requests import get
 
-from .. import SpyglassException
-from .network_types import NakamotoCoefficient, NcRepresentative, Peer, Quorum
+from requests import get
 
-NETWORK_URL = "https://api.spyglass.pw/banano/v1/network/"
+from pyglass.exceptions import SpyglassException
+from pyglass.network import network_types
 
 
-def get_ledger_size() -> Union[int, float]:
-    """https://spyglass-api.web.app/network/ledger-size"""
-    response = get(f"{NETWORK_URL}ledger-size")
-    if not response.ok:
-        raise SpyglassException(response.json())
-
-    ledger_size = response.json()["ledgerSizeMB"]
-    return ledger_size
-
-
-def get_nakamoto_coefficient() -> NakamotoCoefficient:
-    """https://spyglass-api.web.app/network/nakamoto-coefficient"""
-    response = get(f"{NETWORK_URL}nakamoto-coefficient")
-    if not response.ok:
-        raise SpyglassException(response.json())
-
-    nakamoto_coefficient = response.json()
-    return NakamotoCoefficient(
-        delta=nakamoto_coefficient["delta"],
-        nakamoto_coefficient=nakamoto_coefficient["nakamotoCoefficient"],
-        nc_representatives=[
-            NcRepresentative(rep["address"], rep["weight"])
-            for rep in nakamoto_coefficient["ncRepresentatives"]
-        ],
-        nc_reps_weight=nakamoto_coefficient["ncRepsWeight"],
-    )
-
-
-def get_peer_versions() -> list[Peer]:
-    """https://spyglass-api.web.app/network/peer-versions"""
-    response = get(f"{NETWORK_URL}peers")
-    if not response.ok:
-        raise SpyglassException(response.json())
-
-    peers = response.json()
-    return [Peer(peer["count"], peer["version"]) for peer in peers]
-
-
-def get_quorum() -> Quorum:
-    """https://spyglass-api.web.app/network/quorum"""
-    response = get(f"{NETWORK_URL}quorum")
-    if not response.ok:
-        raise SpyglassException(response.json())
-
-    quorum = response.json()
-    return Quorum(
-        no_rep_percent=quorum["noRepPercent"],
-        no_rep_weight=quorum["noRepWeight"],
-        non_burned_weight=quorum["nonBurnedWeight"],
-        offline_percent=quorum["offlinePercent"],
-        offline_weight=quorum["offlineWeight"],
-        online_percent=quorum["onlinePercent"],
-        online_weight=quorum["onlineWeight"],
-        online_weight_minimum=quorum["onlineWeightMinimum"],
-        online_weight_quorum_percent=quorum["onlineWeightQuorumPercent"],
-        peers_stake_weight=quorum["peersStakeWeight"],
-        quorum_delta=quorum["quorumDelta"],
-    )
+class Network:
+    def __init__(self, base_url: str) -> None:
+        self._network_url = f"{base_url}/v1/network/"
+
+    def get_ledger_size(self) -> Union[int, float]:
+        """https://spyglass-api.web.app/network/ledger-size"""
+        response = get(f"{self._network_url}ledger-size")
+        if not response.ok:
+            raise SpyglassException(response.json())
+
+        ledger_size = response.json()["ledgerSizeMB"]
+        return ledger_size
+
+    def get_nakamoto_coefficient(self) -> network_types.NakamotoCoefficient:
+        """https://spyglass-api.web.app/network/nakamoto-coefficient"""
+        response = get(f"{self._network_url}nakamoto-coefficient")
+        if not response.ok:
+            raise SpyglassException(response.json())
+
+        nakamoto_coefficient = response.json()
+        return network_types.NakamotoCoefficient(
+            delta=nakamoto_coefficient["delta"],
+            nakamoto_coefficient=nakamoto_coefficient["nakamotoCoefficient"],
+            nc_representatives=[
+                network_types.NcRepresentative(rep["address"], rep["weight"])
+                for rep in nakamoto_coefficient["ncRepresentatives"]
+            ],
+            nc_reps_weight=nakamoto_coefficient["ncRepsWeight"],
+        )
+
+    def get_peer_versions(self) -> list[network_types.Peer]:
+        """https://spyglass-api.web.app/network/peer-versions"""
+        response = get(f"{self._network_url}peers")
+        if not response.ok:
+            raise SpyglassException(response.json())
+
+        peers = response.json()
+        return [network_types.Peer(peer["count"], peer["version"]) for peer in peers]
+
+    def get_quorum(self) -> network_types.Quorum:
+        """https://spyglass-api.web.app/network/quorum"""
+        response = get(f"{self._network_url}quorum")
+        if not response.ok:
+            raise SpyglassException(response.json())
+
+        quorum = response.json()
+        return network_types.Quorum(
+            no_rep_percent=quorum["noRepPercent"],
+            no_rep_weight=quorum["noRepWeight"],
+            non_burned_weight=quorum["nonBurnedWeight"],
+            offline_percent=quorum["offlinePercent"],
+            offline_weight=quorum["offlineWeight"],
+            online_percent=quorum["onlinePercent"],
+            online_weight=quorum["onlineWeight"],
+            online_weight_minimum=quorum["onlineWeightMinimum"],
+            online_weight_quorum_percent=quorum["onlineWeightQuorumPercent"],
+            peers_stake_weight=quorum["peersStakeWeight"],
+            quorum_delta=quorum["quorumDelta"],
+        )
```

### Comparing `pyglass_api-0.2.1/pyglass/network/network_types.py` & `pyglass_api-0.3.0/pyglass/network/network_types.py`

 * *Files identical despite different names*

### Comparing `pyglass_api-0.2.1/pyglass/representatives/main.py` & `pyglass_api-0.3.0/pyglass/representatives/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,296 +1,274 @@
 from typing import Union
+
 from requests import get, post
 
-from .. import SpyglassException
-from .representatives_types import (
-    Alias,
-    ConfirmationInfo,
-    MonitorStats,
-    MonitoredRepresentative,
-    NodeMonitorStats,
-    Outage,
-    Representative,
-    Score,
-    Uptime,
-    UptimePercentages,
-    UptimeStats,
-)
-
-REPRESENTATIVE_URL = "https://api.spyglass.pw/banano/v1/representatives/"
-
-
-def get_aliases() -> list[Alias]:
-    """https://spyglass-api.web.app/representatives/aliased"""
-    response = get(f"{REPRESENTATIVE_URL}aliases")
-    if not response.ok:
-        raise SpyglassException(response.json())
-
-    aliases = response.json()
-    return [Alias(address=alias["address"], alias=alias["alias"]) for alias in aliases]
-
-
-def get_monitored() -> list[MonitoredRepresentative]:
-    """https://spyglass-api.web.app/representatives/monitored"""
-    response = get(f"{REPRESENTATIVE_URL}monitored")
-    if not response.ok:
-        raise SpyglassException(response.json())
-
-    monitored = response.json()
-    return [
-        MonitoredRepresentative(
-            address=rep["address"],
-            cemented_blocks=rep.get("cementedBlocks", None),
-            confirmation_info=ConfirmationInfo(
-                count=rep["confirmationInfo"].get("count", None),
-                time_span=rep["confirmationInfo"].get("timeSpan", None),
-                average=rep["confirmationInfo"].get("average", None),
-                percentile50=rep["confirmationInfo"].get("percentile50", None),
-                percentile75=rep["confirmationInfo"].get("percentile75", None),
-                percentile90=rep["confirmationInfo"].get("percentile90", None),
-                percentile95=rep["confirmationInfo"].get("percentile95", None),
-                percentile99=rep["confirmationInfo"].get("percentile99", None),
-            )
-            if rep.get("confirmationInfo")
-            else None,
-            current_block=rep.get("currentBlock", None),
-            ip=rep.get("ip", None),
-            location=rep.get("location", None),
-            name=rep.get("name", None),
-            node_uptime_startup=rep.get("nodeUptimeStartup", None),
-            online=rep.get("online", None),
-            peers=rep.get("peers", None),
-            representative=rep.get("representative", None),
-            system_load=rep.get("systemLoad", None),
-            total_mem=rep.get("totalMem", None),
-            used_mem=rep.get("usedMem", None),
-            version=rep.get("version", None),
-            weight=rep.get("weight", None),
-        )
-        for rep in monitored
-    ]
-
-
-def get_online() -> list[str]:
-    """https://spyglass-api.web.app/representatives/online"""
-    response = get(f"{REPRESENTATIVE_URL}online")
-    if not response.ok:
-        raise SpyglassException(response.json())
-
-    return response.json()
-
-
-def get_pr_weight() -> Union[int, float]:
-    """https://spyglass-api.web.app/representatives/pr-weight"""
-    response = get(f"{REPRESENTATIVE_URL}pr-weight")
-    if not response.ok:
-        raise SpyglassException(response.json())
-
-    return response.json()["weight"]
-
-
-def get_representatives(
-    addresses: list[str] = None,
-    include_alias: bool = None,
-    include_delegator_count: bool = None,
-    include_node_monitor_stats: bool = None,
-    include_uptime_pings: bool = None,
-    include_uptime_stats: bool = None,
-    is_monitored: bool = None,
-    is_online: bool = None,
-    is_principal: bool = None,
-    minimum_weight: int = 10000,
-    maximum_weight: int = None,
-    uptime_threshold_day: float = None,
-    uptime_threshold_week: float = None,
-    uptime_threshold_month: float = None,
-    uptime_threshold_semi_annual: float = None,
-    uptime_threshold_year: float = None,
-) -> list[Representative]:
-    """
-    `addresses`: Limit search results to this list of addresses\n
-    `include_node_monitor_stats`: Only applicable to monitored representatives\n
-    `include_uptime_pings`: Append raw data used to calculate ping stats; only applicable when
-    `include_uptime_stats` is enabled\n
-    `include_uptime_stats`: Only reps with >10K BAN weight will have uptime stats available\n
-    `is_monitored`: Filter to only show monitored representatives\n
-    `is_online`: Filter to only show online representatives\n
-    `is_principal`: Filter to only show representatives with >0.1% of the total online voting weight\n
-    `minimum_weight`: Default of 10000 and minimum if 1000\n
-    `uptime_threshold_day`: Filter to only show representatives with an uptime that exceeds this percentage.
-    Only applicable when `include_uptime_stats` is enabled\n
-    https://spyglass-api.web.app/representatives/representatives
-    """
-    data = {
-        "addresses": addresses,
-        "includeAlias": include_alias,
-        "includeDelegatorCount": include_delegator_count,
-        "includeNodeMonitorStats": include_node_monitor_stats,
-        "includeUptimePings": include_uptime_pings,
-        "includeUptimeStats": include_uptime_stats,
-        "isMonitored": is_monitored,
-        "isOnline": is_online,
-        "isPrincipal": is_principal,
-        "minimumWeight": minimum_weight,
-        "maximumWeight": maximum_weight,
-        "uptimeThresholdDay": uptime_threshold_day,
-        "uptimeThresholdWeek": uptime_threshold_week,
-        "uptimeThresholdMonth": uptime_threshold_month,
-        "uptimeThresholdSemiAnnual": uptime_threshold_semi_annual,
-        "uptimeThresholdYear": uptime_threshold_year,
-    }
-    response = post(f"{REPRESENTATIVE_URL}", json=data)
-    if not response.ok:
-        raise SpyglassException(response.json())
-
-    reps = response.json()
-    return [
-        Representative(
-            address=rep["address"],
-            alias=rep.get("alias", None),
-            delegators_count=rep.get("delegatorsCount", None),
-            node_monitor_stats=NodeMonitorStats(
-                cemented_blocks=rep["nodeMonitorStats"].get("cementedBlocks", None),
-                confirmation_info=rep["nodeMonitorStats"].get("confirmationInfo", None),
-                current_block=rep["nodeMonitorStats"].get("currentBlock", None),
-                ip=rep["nodeMonitorStats"].get("ip", None),
-                location=rep["nodeMonitorStats"].get("location", None),
-                name=rep["nodeMonitorStats"].get("name", None),
-                node_uptime_startup=rep["nodeMonitorStats"].get(
-                    "nodeUptimeStartup", None
+from pyglass.exceptions import SpyglassException
+from pyglass.representatives import representatives_types
+
+
+class Representatives:
+    def __init__(self, base_url: str) -> None:
+        self._representatives_url = f"{base_url}/v1/representatives/"
+
+    def get_aliases(self) -> list[representatives_types.Alias]:
+        """https://spyglass-api.web.app/representatives/aliased"""
+        response = get(f"{self._representatives_url}aliases")
+        if not response.ok:
+            raise SpyglassException(response.json())
+
+        aliases = response.json()
+        return [representatives_types.Alias(address=alias["address"], alias=alias["alias"]) for alias in aliases]
+
+    def get_monitored(self) -> list[representatives_types.MonitoredRepresentative]:
+        """https://spyglass-api.web.app/representatives/monitored"""
+        response = get(f"{self._representatives_url}monitored")
+        if not response.ok:
+            raise SpyglassException(response.json())
+
+        monitored = response.json()
+        return [
+            representatives_types.MonitoredRepresentative(
+                address=rep["address"],
+                cemented_blocks=rep.get("cementedBlocks", None),
+                confirmation_info=(
+                    representatives_types.ConfirmationInfo(
+                        count=rep["confirmationInfo"].get("count", None),
+                        time_span=rep["confirmationInfo"].get("timeSpan", None),
+                        average=rep["confirmationInfo"].get("average", None),
+                        percentile50=rep["confirmationInfo"].get("percentile50", None),
+                        percentile75=rep["confirmationInfo"].get("percentile75", None),
+                        percentile90=rep["confirmationInfo"].get("percentile90", None),
+                        percentile95=rep["confirmationInfo"].get("percentile95", None),
+                        percentile99=rep["confirmationInfo"].get("percentile99", None),
+                    )
+                    if rep.get("confirmationInfo")
+                    else None
                 ),
-                peers=rep["nodeMonitorStats"].get("peers", None),
-                representative=rep["nodeMonitorStats"].get("representative", None),
-                system_load=rep["nodeMonitorStats"].get("systemLoad", None),
-                total_mem=rep["nodeMonitorStats"].get("totalMem", None),
-                unchecked_blocks=rep["nodeMonitorStats"].get("uncheckedBlocks", None),
-                used_mem=rep["nodeMonitorStats"].get("usedMem", None),
-                version=rep["nodeMonitorStats"].get("version", None),
-                weight=rep["nodeMonitorStats"].get("weight", None),
+                current_block=rep.get("currentBlock", None),
+                ip=rep.get("ip", None),
+                location=rep.get("location", None),
+                name=rep.get("name", None),
+                node_uptime_startup=rep.get("nodeUptimeStartup", None),
+                online=rep.get("online", None),
+                peers=rep.get("peers", None),
+                representative=rep.get("representative", None),
+                system_load=rep.get("systemLoad", None),
+                total_mem=rep.get("totalMem", None),
+                used_mem=rep.get("usedMem", None),
+                version=rep.get("version", None),
+                weight=rep.get("weight", None),
             )
-            if rep.get("nodeMonitorStats", None)
-            else None,
-            online=rep["online"],
-            uptime_stats=UptimeStats(
-                last_outage=Outage(
-                    offline_unix_timestamp=rep["uptimeStats"]["lastOutage"].get(
-                        "offlineUnixTimestamp", None
-                    ),
-                    offline_date=rep["uptimeStats"]["lastOutage"].get(
-                        "offlineDate", None
-                    ),
-                    online_unix_timestamp=rep["uptimeStats"]["lastOutage"].get(
-                        "onlineUnixTimestamp", None
-                    ),
-                    online_date=rep["uptimeStats"]["lastOutage"].get(
-                        "onlineDate", None
-                    ),
-                    duration_minutes=rep["uptimeStats"]["lastOutage"].get(
-                        "durationMinutes", None
-                    ),
-                )
-                if rep["uptimeStats"].get("lastOutage", None)
-                else None,
-                ping_stats=rep["uptimeStats"].get("pingStats", None),
-                tracking_start_date=rep["uptimeStats"]["trackingStartDate"],
-                tracking_start_unix_timestamp=rep["uptimeStats"][
-                    "trackingStartUnixTimestamp"
-                ],
-                uptime_percentages=UptimePercentages(
-                    day=rep["uptimeStats"]["uptimePercentages"]["day"],
-                    week=rep["uptimeStats"]["uptimePercentages"]["week"],
-                    month=rep["uptimeStats"]["uptimePercentages"]["month"],
-                    semi_annual=rep["uptimeStats"]["uptimePercentages"]["semiAnnual"],
-                    year=rep["uptimeStats"]["uptimePercentages"]["year"],
+            for rep in monitored
+        ]
+
+    def get_online(self) -> list[str]:
+        """https://spyglass-api.web.app/representatives/online"""
+        response = get(f"{self._representatives_url}online")
+        if not response.ok:
+            raise SpyglassException(response.json())
+
+        return response.json()
+
+    def get_pr_weight(self) -> Union[int, float]:
+        """https://spyglass-api.web.app/representatives/pr-weight"""
+        response = get(f"{self._representatives_url}pr-weight")
+        if not response.ok:
+            raise SpyglassException(response.json())
+
+        return response.json()["weight"]
+
+    def get_representatives(
+        self,
+        addresses: list[str] = None,
+        include_alias: bool = None,
+        include_delegator_count: bool = None,
+        include_node_monitor_stats: bool = None,
+        include_uptime_pings: bool = None,
+        include_uptime_stats: bool = None,
+        is_monitored: bool = None,
+        is_online: bool = None,
+        is_principal: bool = None,
+        minimum_weight: int = 10000,
+        maximum_weight: int = None,
+        uptime_threshold_day: float = None,
+        uptime_threshold_week: float = None,
+        uptime_threshold_month: float = None,
+        uptime_threshold_semi_annual: float = None,
+        uptime_threshold_year: float = None,
+    ) -> list[representatives_types.Representative]:
+        """
+        `addresses`: Limit search results to this list of addresses\n
+        `include_node_monitor_stats`: Only applicable to monitored representatives\n
+        `include_uptime_pings`: Append raw data used to calculate ping stats; only applicable when
+        `include_uptime_stats` is enabled\n
+        `include_uptime_stats`: Only reps with >10K BAN weight will have uptime stats available\n
+        `is_monitored`: Filter to only show monitored representatives\n
+        `is_online`: Filter to only show online representatives\n
+        `is_principal`: Filter to only show representatives with >0.1% of the total online voting weight\n
+        `minimum_weight`: Default of 10000 and minimum if 1000\n
+        `uptime_threshold_day`: Filter to only show representatives with an uptime that exceeds this percentage.
+        Only applicable when `include_uptime_stats` is enabled\n
+        https://spyglass-api.web.app/representatives/representatives
+        """
+        data = {
+            "addresses": addresses,
+            "includeAlias": include_alias,
+            "includeDelegatorCount": include_delegator_count,
+            "includeNodeMonitorStats": include_node_monitor_stats,
+            "includeUptimePings": include_uptime_pings,
+            "includeUptimeStats": include_uptime_stats,
+            "isMonitored": is_monitored,
+            "isOnline": is_online,
+            "isPrincipal": is_principal,
+            "minimumWeight": minimum_weight,
+            "maximumWeight": maximum_weight,
+            "uptimeThresholdDay": uptime_threshold_day,
+            "uptimeThresholdWeek": uptime_threshold_week,
+            "uptimeThresholdMonth": uptime_threshold_month,
+            "uptimeThresholdSemiAnnual": uptime_threshold_semi_annual,
+            "uptimeThresholdYear": uptime_threshold_year,
+        }
+        response = post(f"{self._representatives_url}", json=data)
+        if not response.ok:
+            raise SpyglassException(response.json())
+
+        reps = response.json()
+        return [
+            representatives_types.Representative(
+                address=rep["address"],
+                alias=rep.get("alias", None),
+                delegators_count=rep.get("delegatorsCount", None),
+                node_monitor_stats=(
+                    representatives_types.NodeMonitorStats(
+                        cemented_blocks=rep["nodeMonitorStats"].get("cementedBlocks", None),
+                        confirmation_info=rep["nodeMonitorStats"].get("confirmationInfo", None),
+                        current_block=rep["nodeMonitorStats"].get("currentBlock", None),
+                        ip=rep["nodeMonitorStats"].get("ip", None),
+                        location=rep["nodeMonitorStats"].get("location", None),
+                        name=rep["nodeMonitorStats"].get("name", None),
+                        node_uptime_startup=rep["nodeMonitorStats"].get("nodeUptimeStartup", None),
+                        peers=rep["nodeMonitorStats"].get("peers", None),
+                        representative=rep["nodeMonitorStats"].get("representative", None),
+                        system_load=rep["nodeMonitorStats"].get("systemLoad", None),
+                        total_mem=rep["nodeMonitorStats"].get("totalMem", None),
+                        unchecked_blocks=rep["nodeMonitorStats"].get("uncheckedBlocks", None),
+                        used_mem=rep["nodeMonitorStats"].get("usedMem", None),
+                        version=rep["nodeMonitorStats"].get("version", None),
+                        weight=rep["nodeMonitorStats"].get("weight", None),
+                    )
+                    if rep.get("nodeMonitorStats", None)
+                    else None
                 ),
+                online=rep["online"],
+                uptime_stats=(
+                    representatives_types.UptimeStats(
+                        last_outage=(
+                            representatives_types.Outage(
+                                offline_unix_timestamp=rep["uptimeStats"]["lastOutage"].get(
+                                    "offlineUnixTimestamp", None
+                                ),
+                                offline_date=rep["uptimeStats"]["lastOutage"].get("offlineDate", None),
+                                online_unix_timestamp=rep["uptimeStats"]["lastOutage"].get("onlineUnixTimestamp", None),
+                                online_date=rep["uptimeStats"]["lastOutage"].get("onlineDate", None),
+                                duration_minutes=rep["uptimeStats"]["lastOutage"].get("durationMinutes", None),
+                            )
+                            if rep["uptimeStats"].get("lastOutage", None)
+                            else None
+                        ),
+                        ping_stats=rep["uptimeStats"].get("pingStats", None),
+                        tracking_start_date=rep["uptimeStats"]["trackingStartDate"],
+                        tracking_start_unix_timestamp=rep["uptimeStats"]["trackingStartUnixTimestamp"],
+                        uptime_percentages=representatives_types.UptimePercentages(
+                            day=rep["uptimeStats"]["uptimePercentages"]["day"],
+                            week=rep["uptimeStats"]["uptimePercentages"]["week"],
+                            month=rep["uptimeStats"]["uptimePercentages"]["month"],
+                            semi_annual=rep["uptimeStats"]["uptimePercentages"]["semiAnnual"],
+                            year=rep["uptimeStats"]["uptimePercentages"]["year"],
+                        ),
+                    )
+                    if rep.get("uptimeStats", None)
+                    else None
+                ),
+                weight=rep["weight"],
             )
-            if rep.get("uptimeStats", None)
-            else None,
-            weight=rep["weight"],
-        )
-        for rep in reps
-    ]
-
-
-def get_scores() -> list[Score]:
-    """https://spyglass-api.web.app/representatives/scores"""
-    response = get(f"{REPRESENTATIVE_URL}scores")
-    if not response.ok:
-        raise SpyglassException(response.json())
-
-    scores = response.json()
-    return [
-        Score(
-            address=score["address"],
-            alias=score.get("alias", None),
-            monitor_stats=MonitorStats(
-                has_above_avg_cemented_blocks=score["monitorStats"][
-                    "hasAboveAvgCementedBlocks"
-                ],
-                has_below_avg_unchecked_blocks=score["monitorStats"][
-                    "hasBelowAvgUncheckedBlocks"
-                ],
-                has_min_memory_requirement=score["monitorStats"][
-                    "hasMinMemoryRequirement"
-                ],
-                name=score["monitorStats"]["name"],
-            )
-            if score.get("monitorStats", None)
-            else None,
-            online=score["online"],
-            principal=score["principal"],
-            score=score["score"],
-            uptime_percentages=UptimePercentages(
-                day=score["uptimePercentages"]["day"],
-                week=score["uptimePercentages"]["week"],
-                month=score["uptimePercentages"]["month"],
-                semi_annual=score["uptimePercentages"]["semiAnnual"],
-                year=score["uptimePercentages"]["year"],
+            for rep in reps
+        ]
+
+    def get_scores(self) -> list[representatives_types.Score]:
+        """https://spyglass-api.web.app/representatives/scores"""
+        response = get(f"{self._representatives_url}scores")
+        if not response.ok:
+            raise SpyglassException(response.json())
+
+        scores = response.json()
+        return [
+            representatives_types.Score(
+                address=score["address"],
+                alias=score.get("alias", None),
+                monitor_stats=(
+                    representatives_types.MonitorStats(
+                        has_above_avg_cemented_blocks=score["monitorStats"]["hasAboveAvgCementedBlocks"],
+                        has_below_avg_unchecked_blocks=score["monitorStats"]["hasBelowAvgUncheckedBlocks"],
+                        has_min_memory_requirement=score["monitorStats"]["hasMinMemoryRequirement"],
+                        name=score["monitorStats"]["name"],
+                    )
+                    if score.get("monitorStats", None)
+                    else None
+                ),
+                online=score["online"],
+                principal=score["principal"],
+                score=score["score"],
+                uptime_percentages=(
+                    representatives_types.UptimePercentages(
+                        day=score["uptimePercentages"]["day"],
+                        week=score["uptimePercentages"]["week"],
+                        month=score["uptimePercentages"]["month"],
+                        semi_annual=score["uptimePercentages"]["semiAnnual"],
+                        year=score["uptimePercentages"]["year"],
+                    )
+                    if score.get("uptimePercentages", None)
+                    else None
+                ),
+                weight=score["weight"],
+                weight_percentage=score["weightPercentage"],
             )
-            if score.get("uptimePercentages", None)
-            else None,
-            weight=score["weight"],
-            weight_percentage=score["weightPercentage"],
-        )
-        for score in scores
-    ]
-
-
-def get_uptime(representatives: list[str], include_pings: bool = None) -> list[Uptime]:
-    """https://spyglass-api.web.app/representatives/uptime"""
-    data = {"includePings": include_pings, "representatives": representatives}
-    response = post(f"{REPRESENTATIVE_URL}uptime", json=data)
-    if not response.ok:
-        raise SpyglassException(response.json())
-
-    reps = response.json()
-
-    return [
-        Uptime(
-            address=rep["address"],
-            last_outage=Outage(
-                offline_unix_timestamp=rep["lastOutage"].get(
-                    "offlineUnixTimestamp", None
+            for score in scores
+        ]
+
+    def get_uptime(self, representatives: list[str], include_pings: bool = None) -> list[representatives_types.Uptime]:
+        """https://spyglass-api.web.app/representatives/uptime"""
+        data = {"includePings": include_pings, "representatives": representatives}
+        response = post(f"{self._representatives_url}uptime", json=data)
+        if not response.ok:
+            raise SpyglassException(response.json())
+
+        reps = response.json()
+
+        return [
+            representatives_types.Uptime(
+                address=rep["address"],
+                last_outage=(
+                    representatives_types.Outage(
+                        offline_unix_timestamp=rep["lastOutage"].get("offlineUnixTimestamp", None),
+                        offline_date=rep["lastOutage"].get("offlineDate", None),
+                        online_unix_timestamp=rep["lastOutage"].get("onlineUnixTimestamp", None),
+                        online_date=rep["lastOutage"].get("onlineDate", None),
+                        duration_minutes=rep["lastOutage"].get("durationMinutes", None),
+                    )
+                    if rep.get("lastOutage", None)
+                    else None
                 ),
-                offline_date=rep["lastOutage"].get("offlineDate", None),
-                online_unix_timestamp=rep["lastOutage"].get(
-                    "onlineUnixTimestamp", None
+                online=rep["online"],
+                ping_stats=rep.get("pingStats", None),
+                tracking_start_date=rep["trackingStartDate"],
+                tracking_start_unix_timestamp=rep["trackingStartUnixTimestamp"],
+                uptime_percentages=representatives_types.UptimePercentages(
+                    day=rep["uptimePercentages"]["day"],
+                    week=rep["uptimePercentages"]["week"],
+                    month=rep["uptimePercentages"]["month"],
+                    semi_annual=rep["uptimePercentages"]["semiAnnual"],
+                    year=rep["uptimePercentages"]["year"],
                 ),
-                online_date=rep["lastOutage"].get("onlineDate", None),
-                duration_minutes=rep["lastOutage"].get("durationMinutes", None),
             )
-            if rep.get("lastOutage", None)
-            else None,
-            online=rep["online"],
-            ping_stats=rep.get("pingStats", None),
-            tracking_start_date=rep["trackingStartDate"],
-            tracking_start_unix_timestamp=rep["trackingStartUnixTimestamp"],
-            uptime_percentages=UptimePercentages(
-                day=rep["uptimePercentages"]["day"],
-                week=rep["uptimePercentages"]["week"],
-                month=rep["uptimePercentages"]["month"],
-                semi_annual=rep["uptimePercentages"]["semiAnnual"],
-                year=rep["uptimePercentages"]["year"],
-            ),
-        )
-        for rep in reps
-    ]
+            for rep in reps
+        ]
```

### Comparing `pyglass_api-0.2.1/pyglass/representatives/representatives_types.py` & `pyglass_api-0.3.0/pyglass/representatives/representatives_types.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from typing import Optional, Union
 from dataclasses import dataclass
+from typing import Optional, Union
 
 
 @dataclass(frozen=True, order=True)
 class Alias:
     address: str
     alias: str
```

### Comparing `pyglass_api-0.2.1/PKG-INFO` & `pyglass_api-0.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyglass-api
-Version: 0.2.1
+Version: 0.3.0
 Summary: python wrapper for /dev-ptera/spyglass-api
 Home-page: https://github.com/Eulentier161/pyglass-api
 License: MIT
 Author: Eulentier161
 Author-email: git@eule.wtf
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -16,14 +16,16 @@
 Description-Content-Type: text/markdown
 
 # python wrapper for [spyglass-api](https://github.com/dev-ptera/spyglass-api)
 
 ```console
 pip install pyglass-api
 ```
-```py
-from pyglass import account
 
-acc = account.get_overview("ban_1hootubx...hqnxd")
+```python
+from pyglass import PyglassClient
+
+client = PyglassClient() # or PyglassClient("https://api.spyglass.eule.wtf/banano")
+acc = client.account.get_overview("ban_1hootubxy68fhhrctjmaias148tz91tsse3pq1pgmfedsm3cubhobuihqnxd")
 print(acc.balance)
 ```
```

