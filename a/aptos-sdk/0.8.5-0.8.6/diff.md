# Comparing `tmp/aptos_sdk-0.8.5.tar.gz` & `tmp/aptos_sdk-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aptos_sdk-0.8.5.tar", max compression
+gzip compressed data, was "aptos_sdk-0.8.6.tar", max compression
```

## Comparing `aptos_sdk-0.8.5.tar` & `aptos_sdk-0.8.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     3351 2024-02-20 05:03:25.062080 aptos_sdk-0.8.5/README.md
--rw-r--r--   0        0        0       70 2023-11-18 22:01:26.123602 aptos_sdk-0.8.5/aptos_sdk/__init__.py
--rw-r--r--   0        0        0     6554 2024-04-01 05:08:42.252008 aptos_sdk-0.8.5/aptos_sdk/account.py
--rw-r--r--   0        0        0    22922 2023-11-18 22:01:26.123602 aptos_sdk-0.8.5/aptos_sdk/account_address.py
--rw-r--r--   0        0        0     8460 2023-11-18 22:01:26.123602 aptos_sdk-0.8.5/aptos_sdk/account_sequence_number.py
--rw-r--r--   0        0        0     6487 2023-11-18 22:01:26.123602 aptos_sdk-0.8.5/aptos_sdk/aptos_cli_wrapper.py
--rw-r--r--   0        0        0    21124 2024-04-01 05:08:42.535341 aptos_sdk-0.8.5/aptos_sdk/aptos_token_client.py
--rw-r--r--   0        0        0     9656 2024-04-01 05:08:42.332008 aptos_sdk-0.8.5/aptos_sdk/aptos_tokenv1_client.py
--rw-r--r--   0        0        0      830 2024-04-01 05:08:42.085342 aptos_sdk-0.8.5/aptos_sdk/asymmetric_crypto.py
--rw-r--r--   0        0        0     2850 2023-11-18 22:01:26.126936 aptos_sdk-0.8.5/aptos_sdk/asymmetric_crypto_wrapper.py
--rw-r--r--   0        0        0    37542 2024-04-01 05:08:42.455341 aptos_sdk-0.8.5/aptos_sdk/async_client.py
--rw-r--r--   0        0        0    13187 2023-11-18 22:01:26.126936 aptos_sdk-0.8.5/aptos_sdk/authenticator.py
--rw-r--r--   0        0        0    11077 2024-04-01 05:08:42.345341 aptos_sdk-0.8.5/aptos_sdk/bcs.py
--rw-r--r--   0        0        0     3195 2023-11-18 22:01:26.126936 aptos_sdk-0.8.5/aptos_sdk/cli.py
--rw-r--r--   0        0        0    14221 2023-11-18 22:01:26.126936 aptos_sdk-0.8.5/aptos_sdk/ed25519.py
--rw-r--r--   0        0        0      277 2023-11-18 22:01:26.126936 aptos_sdk-0.8.5/aptos_sdk/metadata.py
--rw-r--r--   0        0        0     7774 2024-04-01 05:08:42.202008 aptos_sdk-0.8.5/aptos_sdk/package_publisher.py
--rw-r--r--   0        0        0        0 2024-03-31 04:39:05.958323 aptos_sdk-0.8.5/aptos_sdk/py.typed
--rw-r--r--   0        0        0     7661 2023-11-18 22:01:26.130269 aptos_sdk-0.8.5/aptos_sdk/secp256k1_ecdsa.py
--rw-r--r--   0        0        0     8516 2024-04-01 05:08:42.222008 aptos_sdk-0.8.5/aptos_sdk/transaction_worker.py
--rw-r--r--   0        0        0    30228 2024-04-01 05:08:42.408675 aptos_sdk-0.8.5/aptos_sdk/transactions.py
--rw-r--r--   0        0        0    10193 2024-03-31 04:31:30.631173 aptos_sdk-0.8.5/aptos_sdk/type_tag.py
--rw-r--r--   0        0        0      862 2024-04-01 06:58:11.797878 aptos_sdk-0.8.5/pyproject.toml
--rw-r--r--   0        0        0     4320 1970-01-01 00:00:00.000000 aptos_sdk-0.8.5/PKG-INFO
+-rw-r--r--   0        0        0     3351 2024-04-02 02:23:07.389754 aptos_sdk-0.8.6/README.md
+-rw-r--r--   0        0        0       70 2023-11-18 22:01:26.123602 aptos_sdk-0.8.6/aptos_sdk/__init__.py
+-rw-r--r--   0        0        0     6554 2024-04-02 07:43:49.389243 aptos_sdk-0.8.6/aptos_sdk/account.py
+-rw-r--r--   0        0        0    22922 2024-04-02 02:21:12.532307 aptos_sdk-0.8.6/aptos_sdk/account_address.py
+-rw-r--r--   0        0        0     8460 2023-11-18 22:01:26.123602 aptos_sdk-0.8.6/aptos_sdk/account_sequence_number.py
+-rw-r--r--   0        0        0     6487 2023-11-18 22:01:26.123602 aptos_sdk-0.8.6/aptos_sdk/aptos_cli_wrapper.py
+-rw-r--r--   0        0        0    21124 2024-04-02 07:43:49.705911 aptos_sdk-0.8.6/aptos_sdk/aptos_token_client.py
+-rw-r--r--   0        0        0     9656 2024-04-02 07:43:49.502576 aptos_sdk-0.8.6/aptos_sdk/aptos_tokenv1_client.py
+-rw-r--r--   0        0        0      830 2024-04-02 02:28:38.275948 aptos_sdk-0.8.6/aptos_sdk/asymmetric_crypto.py
+-rw-r--r--   0        0        0     2850 2024-04-02 02:21:12.532307 aptos_sdk-0.8.6/aptos_sdk/asymmetric_crypto_wrapper.py
+-rw-r--r--   0        0        0    37542 2024-04-02 07:43:49.672577 aptos_sdk-0.8.6/aptos_sdk/async_client.py
+-rw-r--r--   0        0        0    13187 2024-04-02 02:21:12.532307 aptos_sdk-0.8.6/aptos_sdk/authenticator.py
+-rw-r--r--   0        0        0    11077 2024-04-02 02:28:38.275948 aptos_sdk-0.8.6/aptos_sdk/bcs.py
+-rw-r--r--   0        0        0     3195 2023-11-18 22:01:26.126936 aptos_sdk-0.8.6/aptos_sdk/cli.py
+-rw-r--r--   0        0        0    14221 2024-04-02 02:21:12.532307 aptos_sdk-0.8.6/aptos_sdk/ed25519.py
+-rw-r--r--   0        0        0      277 2023-11-18 22:01:26.126936 aptos_sdk-0.8.6/aptos_sdk/metadata.py
+-rw-r--r--   0        0        0     7774 2024-04-02 07:43:49.455910 aptos_sdk-0.8.6/aptos_sdk/package_publisher.py
+-rw-r--r--   0        0        0        0 2024-03-31 04:39:05.958323 aptos_sdk-0.8.6/aptos_sdk/py.typed
+-rw-r--r--   0        0        0     7661 2024-04-02 02:21:12.532307 aptos_sdk-0.8.6/aptos_sdk/secp256k1_ecdsa.py
+-rw-r--r--   0        0        0     8516 2024-04-02 07:43:49.459243 aptos_sdk-0.8.6/aptos_sdk/transaction_worker.py
+-rw-r--r--   0        0        0    30288 2024-04-02 07:48:41.987247 aptos_sdk-0.8.6/aptos_sdk/transactions.py
+-rw-r--r--   0        0        0    10841 2024-04-02 07:48:41.987247 aptos_sdk-0.8.6/aptos_sdk/type_tag.py
+-rw-r--r--   0        0        0      862 2024-04-02 07:51:27.828014 aptos_sdk-0.8.6/pyproject.toml
+-rw-r--r--   0        0        0     4320 1970-01-01 00:00:00.000000 aptos_sdk-0.8.6/PKG-INFO
```

### Comparing `aptos_sdk-0.8.5/README.md` & `aptos_sdk-0.8.6/README.md`

 * *Files identical despite different names*

### Comparing `aptos_sdk-0.8.5/aptos_sdk/account.py` & `aptos_sdk-0.8.6/aptos_sdk/account.py`

 * *Files identical despite different names*

### Comparing `aptos_sdk-0.8.5/aptos_sdk/account_address.py` & `aptos_sdk-0.8.6/aptos_sdk/account_address.py`

 * *Files identical despite different names*

### Comparing `aptos_sdk-0.8.5/aptos_sdk/account_sequence_number.py` & `aptos_sdk-0.8.6/aptos_sdk/account_sequence_number.py`

 * *Files identical despite different names*

### Comparing `aptos_sdk-0.8.5/aptos_sdk/aptos_cli_wrapper.py` & `aptos_sdk-0.8.6/aptos_sdk/aptos_cli_wrapper.py`

 * *Files identical despite different names*

### Comparing `aptos_sdk-0.8.5/aptos_sdk/aptos_token_client.py` & `aptos_sdk-0.8.6/aptos_sdk/aptos_token_client.py`

 * *Files identical despite different names*

### Comparing `aptos_sdk-0.8.5/aptos_sdk/aptos_tokenv1_client.py` & `aptos_sdk-0.8.6/aptos_sdk/aptos_tokenv1_client.py`

 * *Files identical despite different names*

### Comparing `aptos_sdk-0.8.5/aptos_sdk/asymmetric_crypto.py` & `aptos_sdk-0.8.6/aptos_sdk/asymmetric_crypto.py`

 * *Files identical despite different names*

### Comparing `aptos_sdk-0.8.5/aptos_sdk/asymmetric_crypto_wrapper.py` & `aptos_sdk-0.8.6/aptos_sdk/asymmetric_crypto_wrapper.py`

 * *Files identical despite different names*

### Comparing `aptos_sdk-0.8.5/aptos_sdk/async_client.py` & `aptos_sdk-0.8.6/aptos_sdk/async_client.py`

 * *Files identical despite different names*

### Comparing `aptos_sdk-0.8.5/aptos_sdk/authenticator.py` & `aptos_sdk-0.8.6/aptos_sdk/authenticator.py`

 * *Files identical despite different names*

### Comparing `aptos_sdk-0.8.5/aptos_sdk/bcs.py` & `aptos_sdk-0.8.6/aptos_sdk/bcs.py`

 * *Files identical despite different names*

### Comparing `aptos_sdk-0.8.5/aptos_sdk/cli.py` & `aptos_sdk-0.8.6/aptos_sdk/cli.py`

 * *Files identical despite different names*

### Comparing `aptos_sdk-0.8.5/aptos_sdk/ed25519.py` & `aptos_sdk-0.8.6/aptos_sdk/ed25519.py`

 * *Files identical despite different names*

### Comparing `aptos_sdk-0.8.5/aptos_sdk/package_publisher.py` & `aptos_sdk-0.8.6/aptos_sdk/package_publisher.py`

 * *Files identical despite different names*

### Comparing `aptos_sdk-0.8.5/aptos_sdk/secp256k1_ecdsa.py` & `aptos_sdk-0.8.6/aptos_sdk/secp256k1_ecdsa.py`

 * *Files identical despite different names*

### Comparing `aptos_sdk-0.8.5/aptos_sdk/transaction_worker.py` & `aptos_sdk-0.8.6/aptos_sdk/transaction_worker.py`

 * *Files identical despite different names*

### Comparing `aptos_sdk-0.8.5/aptos_sdk/transactions.py` & `aptos_sdk-0.8.6/aptos_sdk/transactions.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     Authenticator,
     Ed25519Authenticator,
     FeePayerAuthenticator,
     MultiAgentAuthenticator,
     SingleKeyAuthenticator,
     SingleSenderAuthenticator,
 )
-from .bcs import Deserializer, Serializer
+from .bcs import Deserializable, Deserializer, Serializable, Serializer
 from .type_tag import StructTag, TypeTag
 
 
 class RawTransactionInternal(Protocol):
     def keyed(self) -> bytes:
         ser = Serializer()
         self.serialize(ser)
@@ -74,15 +74,15 @@
 
     def prehash(self) -> bytes:
         hasher = hashlib.sha3_256()
         hasher.update(b"APTOS::RawTransactionWithData")
         return hasher.digest()
 
 
-class RawTransaction(RawTransactionInternal):
+class RawTransaction(Deserializable, RawTransactionInternal, Serializable):
     # Sender's address
     sender: AccountAddress
     # Sequence number of this transaction. This must match the sequence number in the sender's
     # account at the time of execution.
     sequence_number: int
     # The transaction payload, e.g., a script to execute.
     payload: TransactionPayload
```

### Comparing `aptos_sdk-0.8.5/aptos_sdk/type_tag.py` & `aptos_sdk-0.8.6/aptos_sdk/type_tag.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 from __future__ import annotations
 
 import typing
 import unittest
 from typing import List, Tuple
 
 from .account_address import AccountAddress
-from .bcs import Deserializer, Serializer
+from .bcs import Deserializable, Deserializer, Serializable, Serializer
 
 
-class TypeTag:
+class TypeTag(Deserializable, Serializable):
     """TypeTag represents a primitive in Move."""
 
     BOOL: int = 0
     U8: int = 1
     U64: int = 2
     U128: int = 3
     ACCOUNT_ADDRESS: int = 4
@@ -72,15 +72,15 @@
         raise NotImplementedError
 
     def serialize(self, serializer: Serializer):
         serializer.uleb128(self.value.variant())
         serializer.struct(self.value)
 
 
-class BoolTag:
+class BoolTag(Deserializable, Serializable):
     value: bool
 
     def __init__(self, value: bool):
         self.value = value
 
     def __eq__(self, other: object) -> bool:
         if not isinstance(other, BoolTag):
@@ -97,15 +97,15 @@
     def deserialize(deserializer: Deserializer) -> BoolTag:
         return BoolTag(deserializer.bool())
 
     def serialize(self, serializer: Serializer):
         serializer.bool(self.value)
 
 
-class U8Tag:
+class U8Tag(Deserializable, Serializable):
     value: int
 
     def __init__(self, value: int):
         self.value = value
 
     def __eq__(self, other: object) -> bool:
         if not isinstance(other, U8Tag):
@@ -122,15 +122,15 @@
     def deserialize(deserializer: Deserializer) -> U8Tag:
         return U8Tag(deserializer.u8())
 
     def serialize(self, serializer: Serializer):
         serializer.u8(self.value)
 
 
-class U16Tag:
+class U16Tag(Deserializable, Serializable):
     value: int
 
     def __init__(self, value: int):
         self.value = value
 
     def __eq__(self, other: object) -> bool:
         if not isinstance(other, U16Tag):
@@ -147,15 +147,15 @@
     def deserialize(deserializer: Deserializer) -> U16Tag:
         return U16Tag(deserializer.u16())
 
     def serialize(self, serializer: Serializer):
         serializer.u16(self.value)
 
 
-class U32Tag:
+class U32Tag(Deserializable, Serializable):
     value: int
 
     def __init__(self, value: int):
         self.value = value
 
     def __eq__(self, other: object) -> bool:
         if not isinstance(other, U32Tag):
@@ -172,15 +172,15 @@
     def deserialize(deserializer: Deserializer) -> U32Tag:
         return U32Tag(deserializer.u32())
 
     def serialize(self, serializer: Serializer):
         serializer.u32(self.value)
 
 
-class U64Tag:
+class U64Tag(Deserializable, Serializable):
     value: int
 
     def __init__(self, value: int):
         self.value = value
 
     def __eq__(self, other: object) -> bool:
         if not isinstance(other, U64Tag):
@@ -197,15 +197,15 @@
     def deserialize(deserializer: Deserializer) -> U64Tag:
         return U64Tag(deserializer.u64())
 
     def serialize(self, serializer: Serializer):
         serializer.u64(self.value)
 
 
-class U128Tag:
+class U128Tag(Deserializable, Serializable):
     value: int
 
     def __init__(self, value: int):
         self.value = value
 
     def __eq__(self, other: object) -> bool:
         if not isinstance(other, U128Tag):
@@ -222,15 +222,15 @@
     def deserialize(deserializer: Deserializer) -> U128Tag:
         return U128Tag(deserializer.u128())
 
     def serialize(self, serializer: Serializer):
         serializer.u128(self.value)
 
 
-class U256Tag:
+class U256Tag(Deserializable, Serializable):
     value: int
 
     def __init__(self, value: int):
         self.value = value
 
     def __eq__(self, other: object) -> bool:
         if not isinstance(other, U256Tag):
@@ -247,15 +247,15 @@
     def deserialize(deserializer: Deserializer) -> U256Tag:
         return U256Tag(deserializer.u256())
 
     def serialize(self, serializer: Serializer):
         serializer.u256(self.value)
 
 
-class AccountAddressTag:
+class AccountAddressTag(Deserializable, Serializable):
     value: AccountAddress
 
     def __init__(self, value: AccountAddress):
         self.value = value
 
     def __eq__(self, other: object) -> bool:
         if not isinstance(other, AccountAddressTag):
@@ -272,15 +272,15 @@
     def deserialize(deserializer: Deserializer) -> AccountAddressTag:
         return AccountAddressTag(deserializer.struct(AccountAddress))
 
     def serialize(self, serializer: Serializer):
         serializer.struct(self.value)
 
 
-class StructTag:
+class StructTag(Deserializable, Serializable):
     address: AccountAddress
     module: str
     name: str
     type_args: List[TypeTag]
 
     def __init__(self, address, module, name, type_args):
         self.address = address
@@ -305,50 +305,57 @@
             for type_arg in self.type_args[1:]:
                 value += f", {type_arg}"
             value += ">"
         return value
 
     @staticmethod
     def from_str(type_tag: str) -> StructTag:
-        return StructTag._from_str_internal(type_tag, 0)[0][0]
+        return StructTag._from_str_internal(type_tag, 0)[0][0].value
 
     @staticmethod
-    def _from_str_internal(type_tag: str, index: int) -> Tuple[List[StructTag], int]:
+    def _from_str_internal(type_tag: str, index: int) -> Tuple[List[TypeTag], int]:
         name = ""
         tags = []
-        inner_tags: List[StructTag] = []
+        inner_tags: List[TypeTag] = []
 
         while index < len(type_tag):
             letter = type_tag[index]
             index += 1
 
             if letter == " ":
                 continue
 
             if letter == "<":
                 (inner_tags, index) = StructTag._from_str_internal(type_tag, index)
             elif letter == ",":
                 split = name.split("::")
-                tag = StructTag(
-                    AccountAddress.from_str_relaxed(split[0]),
-                    split[1],
-                    split[2],
-                    inner_tags,
+                tag = TypeTag(
+                    StructTag(
+                        AccountAddress.from_str_relaxed(split[0]),
+                        split[1],
+                        split[2],
+                        inner_tags,
+                    )
                 )
                 tags.append(tag)
                 name = ""
                 inner_tags = []
             elif letter == ">":
                 break
             else:
                 name += letter
 
         split = name.split("::")
-        tag = StructTag(
-            AccountAddress.from_str_relaxed(split[0]), split[1], split[2], inner_tags
+        tag = TypeTag(
+            StructTag(
+                AccountAddress.from_str_relaxed(split[0]),
+                split[1],
+                split[2],
+                inner_tags,
+            )
         )
         tags.append(tag)
         return (tags, index)
 
     def variant(self):
         return TypeTag.STRUCT
 
@@ -370,13 +377,16 @@
 class Test(unittest.TestCase):
     def test_nested_structs(self):
         l0 = "0x0::l0::L0"
         l10 = "0x1::l10::L10"
         l20 = "0x2::l20::L20"
         l11 = "0x1::l11::L11"
         composite = f"{l0}<{l10}<{l20}>, {l11}>"
-
-        self.assertEqual(composite, f"{StructTag.from_str(composite)}")
+        derived = StructTag.from_str(composite)
+        self.assertEqual(composite, f"{derived}")
+        in_bytes = derived.to_bytes()
+        from_bytes = StructTag.from_bytes(in_bytes)
+        self.assertEqual(derived, from_bytes)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `aptos_sdk-0.8.5/pyproject.toml` & `aptos_sdk-0.8.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aptos-sdk"
-version = "0.8.5"
+version = "0.8.6"
 description = "Aptos SDK"
 authors = ["Aptos Labs <opensource@aptoslabs.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/aptos-labs/aptos-core"
 homepage = "https://github.com/aptos-labs/aptos-core/tree/main/ecosystem/python/sdk"
 keywords = ["web3", "sdk", "aptos", "blockchain"]
```

### Comparing `aptos_sdk-0.8.5/PKG-INFO` & `aptos_sdk-0.8.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aptos-sdk
-Version: 0.8.5
+Version: 0.8.6
 Summary: Aptos SDK
 Home-page: https://github.com/aptos-labs/aptos-core/tree/main/ecosystem/python/sdk
 License: Apache-2.0
 Keywords: web3,sdk,aptos,blockchain
 Author: Aptos Labs
 Author-email: opensource@aptoslabs.com
 Requires-Python: >=3.8.1
```

