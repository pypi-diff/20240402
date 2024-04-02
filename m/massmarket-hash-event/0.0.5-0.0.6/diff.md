# Comparing `tmp/massmarket_hash_event-0.0.5.tar.gz` & `tmp/massmarket_hash_event-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "massmarket_hash_event-0.0.5.tar", last modified: Tue Mar 19 12:51:24 2024, max compression
+gzip compressed data, was "massmarket_hash_event-0.0.6.tar", last modified: Tue Apr  2 19:53:58 2024, max compression
```

## Comparing `massmarket_hash_event-0.0.5.tar` & `massmarket_hash_event-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 cryptix    (501) staff       (20)        0 2024-03-19 12:51:24.772919 massmarket_hash_event-0.0.5/
--rw-r--r--   0 cryptix    (501) staff       (20)      860 2024-03-19 12:51:24.772642 massmarket_hash_event-0.0.5/PKG-INFO
-drwxr-xr-x   0 cryptix    (501) staff       (20)        0 2024-03-19 12:51:24.770648 massmarket_hash_event-0.0.5/massmarket_hash_event/
--rw-r--r--   0 cryptix    (501) staff       (20)     3853 2024-03-19 12:49:25.000000 massmarket_hash_event-0.0.5/massmarket_hash_event/__init__.py
--rw-r--r--   0 cryptix    (501) staff       (20)    10772 2024-03-19 12:49:25.000000 massmarket_hash_event-0.0.5/massmarket_hash_event/schema_pb2.py
--rw-r--r--   0 cryptix    (501) staff       (20)    16337 2024-03-19 12:49:25.000000 massmarket_hash_event-0.0.5/massmarket_hash_event/schema_pb2.pyi
--rw-r--r--   0 cryptix    (501) staff       (20)     2914 2024-03-19 12:48:08.000000 massmarket_hash_event-0.0.5/massmarket_hash_event/typedData.json
-drwxr-xr-x   0 cryptix    (501) staff       (20)        0 2024-03-19 12:51:24.771538 massmarket_hash_event-0.0.5/massmarket_hash_event.egg-info/
--rw-r--r--   0 cryptix    (501) staff       (20)      860 2024-03-19 12:51:24.000000 massmarket_hash_event-0.0.5/massmarket_hash_event.egg-info/PKG-INFO
--rw-r--r--   0 cryptix    (501) staff       (20)      428 2024-03-19 12:51:24.000000 massmarket_hash_event-0.0.5/massmarket_hash_event.egg-info/SOURCES.txt
--rw-r--r--   0 cryptix    (501) staff       (20)        1 2024-03-19 12:51:24.000000 massmarket_hash_event-0.0.5/massmarket_hash_event.egg-info/dependency_links.txt
--rw-r--r--   0 cryptix    (501) staff       (20)       20 2024-03-19 12:51:24.000000 massmarket_hash_event-0.0.5/massmarket_hash_event.egg-info/requires.txt
--rw-r--r--   0 cryptix    (501) staff       (20)       22 2024-03-19 12:51:24.000000 massmarket_hash_event-0.0.5/massmarket_hash_event.egg-info/top_level.txt
--rw-r--r--   0 cryptix    (501) staff       (20)     1390 2024-03-19 12:51:21.000000 massmarket_hash_event-0.0.5/pyproject.toml
--rw-r--r--   0 cryptix    (501) staff       (20)       38 2024-03-19 12:51:24.772975 massmarket_hash_event-0.0.5/setup.cfg
-drwxr-xr-x   0 cryptix    (501) staff       (20)        0 2024-03-19 12:51:24.772002 massmarket_hash_event-0.0.5/tests/
--rw-r--r--   0 cryptix    (501) staff       (20)     1266 2024-03-19 12:49:25.000000 massmarket_hash_event-0.0.5/tests/test_encode.py
--rw-r--r--   0 cryptix    (501) staff       (20)     6046 2024-03-19 12:49:25.000000 massmarket_hash_event-0.0.5/tests/test_signatures.py
+drwxr-xr-x   0 cryptix   (1001) users      (100)        0 2024-04-02 19:53:58.973081 massmarket_hash_event-0.0.6/
+-rw-r--r--   0 cryptix   (1001) users      (100)      860 2024-04-02 19:53:58.973081 massmarket_hash_event-0.0.6/PKG-INFO
+drwxr-xr-x   0 cryptix   (1001) users      (100)        0 2024-04-02 19:53:58.972081 massmarket_hash_event-0.0.6/massmarket_hash_event/
+-rw-r--r--   0 cryptix   (1001) users      (100)     3853 2024-04-02 19:44:37.000000 massmarket_hash_event-0.0.6/massmarket_hash_event/__init__.py
+-rw-r--r--   0 cryptix   (1001) users      (100)    10779 2024-04-02 19:46:53.000000 massmarket_hash_event-0.0.6/massmarket_hash_event/schema_pb2.py
+-rw-r--r--   0 cryptix   (1001) users      (100)    16470 2024-04-02 19:46:53.000000 massmarket_hash_event-0.0.6/massmarket_hash_event/schema_pb2.pyi
+-rw-r--r--   0 cryptix   (1001) users      (100)     3038 2024-04-02 19:49:12.000000 massmarket_hash_event-0.0.6/massmarket_hash_event/typedData.json
+drwxr-xr-x   0 cryptix   (1001) users      (100)        0 2024-04-02 19:53:58.972081 massmarket_hash_event-0.0.6/massmarket_hash_event.egg-info/
+-rw-r--r--   0 cryptix   (1001) users      (100)      860 2024-04-02 19:53:58.000000 massmarket_hash_event-0.0.6/massmarket_hash_event.egg-info/PKG-INFO
+-rw-r--r--   0 cryptix   (1001) users      (100)      428 2024-04-02 19:53:58.000000 massmarket_hash_event-0.0.6/massmarket_hash_event.egg-info/SOURCES.txt
+-rw-r--r--   0 cryptix   (1001) users      (100)        1 2024-04-02 19:53:58.000000 massmarket_hash_event-0.0.6/massmarket_hash_event.egg-info/dependency_links.txt
+-rw-r--r--   0 cryptix   (1001) users      (100)       20 2024-04-02 19:53:58.000000 massmarket_hash_event-0.0.6/massmarket_hash_event.egg-info/requires.txt
+-rw-r--r--   0 cryptix   (1001) users      (100)       22 2024-04-02 19:53:58.000000 massmarket_hash_event-0.0.6/massmarket_hash_event.egg-info/top_level.txt
+-rw-r--r--   0 cryptix   (1001) users      (100)     1390 2024-04-02 19:53:47.000000 massmarket_hash_event-0.0.6/pyproject.toml
+-rw-r--r--   0 cryptix   (1001) users      (100)       38 2024-04-02 19:53:58.973081 massmarket_hash_event-0.0.6/setup.cfg
+drwxr-xr-x   0 cryptix   (1001) users      (100)        0 2024-04-02 19:53:58.973081 massmarket_hash_event-0.0.6/tests/
+-rw-r--r--   0 cryptix   (1001) users      (100)     1266 2024-04-02 19:44:37.000000 massmarket_hash_event-0.0.6/tests/test_encode.py
+-rw-r--r--   0 cryptix   (1001) users      (100)     6071 2024-04-02 19:53:14.000000 massmarket_hash_event-0.0.6/tests/test_signatures.py
```

### Comparing `massmarket_hash_event-0.0.5/PKG-INFO` & `massmarket_hash_event-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: massmarket_hash_event
-Version: 0.0.5
+Version: 0.0.6
 Summary: Helper functions to hash events for signature creation and verification on Mass Market.
 Author-email: Henry Bubert <henry@mass.market>
 License: MIT
 Project-URL: Homepage, https://mass.market
 Project-URL: Repository, https://github.com/masslbs/network-schema.git
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `massmarket_hash_event-0.0.5/massmarket_hash_event/__init__.py` & `massmarket_hash_event-0.0.6/massmarket_hash_event/__init__.py`

 * *Files identical despite different names*

### Comparing `massmarket_hash_event-0.0.5/massmarket_hash_event/schema_pb2.py` & `massmarket_hash_event-0.0.6/massmarket_hash_event/schema_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-# SPDX-FileCopyrightText: 2024 Mass Labs
-#
-# SPDX-License-Identifier: MIT
-
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: schema.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
@@ -13,15 +9,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0cschema.proto\x12\x0bmarket.mass\"c\n\rStoreManifest\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\x12\x16\n\x0estore_token_id\x18\x02 \x01(\x0c\x12\x0e\n\x06\x64omain\x18\x03 \x01(\t\x12\x18\n\x10published_tag_id\x18\x04 \x01(\x0c\"\xcd\x02\n\x0eUpdateManifest\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\x12\x38\n\x05\x66ield\x18\x02 \x01(\x0e\x32).market.mass.UpdateManifest.ManifestField\x12\x10\n\x06string\x18\x03 \x01(\tH\x00\x12\x10\n\x06tag_id\x18\x04 \x01(\x0cH\x00\x12\x14\n\nerc20_addr\x18\x05 \x01(\x0cH\x00\"\xab\x01\n\rManifestField\x12\x1e\n\x1aMANIFEST_FIELD_UNSPECIFIED\x10\x00\x12\x19\n\x15MANIFEST_FIELD_DOMAIN\x10\x01\x12 \n\x1cMANIFEST_FIELD_PUBLISHED_TAG\x10\x02\x12\x1c\n\x18MANIFEST_FIELD_ADD_ERC20\x10\x03\x12\x1f\n\x1bMANIFEST_FIELD_REMOVE_ERC20\x10\x04\x42\x07\n\x05value\"?\n\nCreateItem\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\x12\r\n\x05price\x18\x02 \x01(\t\x12\x10\n\x08metadata\x18\x03 \x01(\x0c\"\xe7\x01\n\nUpdateItem\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\x12\x0f\n\x07item_id\x18\x02 \x01(\x0c\x12\x30\n\x05\x66ield\x18\x03 \x01(\x0e\x32!.market.mass.UpdateItem.ItemField\x12\x0f\n\x05price\x18\x04 \x01(\tH\x00\x12\x12\n\x08metadata\x18\x05 \x01(\x0cH\x00\"V\n\tItemField\x12\x1a\n\x16ITEM_FIELD_UNSPECIFIED\x10\x00\x12\x14\n\x10ITEM_FIELD_PRICE\x10\x01\x12\x17\n\x13ITEM_FIELD_METADATA\x10\x02\x42\x07\n\x05value\"+\n\tCreateTag\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\x12\x0c\n\x04name\x18\x02 \x01(\t\"=\n\x08\x41\x64\x64ToTag\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\x12\x0e\n\x06tag_id\x18\x02 \x01(\x0c\x12\x0f\n\x07item_id\x18\x03 \x01(\x0c\"B\n\rRemoveFromTag\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\x12\x0e\n\x06tag_id\x18\x02 \x01(\x0c\x12\x0f\n\x07item_id\x18\x03 \x01(\x0c\";\n\tRenameTag\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\x12\x0e\n\x06tag_id\x18\x02 \x01(\x0c\x12\x0c\n\x04name\x18\x03 \x01(\t\"-\n\tDeleteTag\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\x12\x0e\n\x06tag_id\x18\x02 \x01(\x0c\"Q\n\x0b\x43hangeStock\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\x12\x10\n\x08item_ids\x18\x02 \x03(\x0c\x12\r\n\x05\x64iffs\x18\x03 \x03(\x11\x12\x0f\n\x07\x63\x61rt_id\x18\x04 \x01(\x0c\"Q\n\nNewKeyCard\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\x12\x18\n\x10user_wallet_addr\x18\x02 \x01(\x0c\x12\x17\n\x0f\x63\x61rd_public_key\x18\x03 \x01(\x0c\"\x1e\n\nCreateCart\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\"R\n\nChangeCart\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\x12\x0f\n\x07\x63\x61rt_id\x18\x02 \x01(\x0c\x12\x0f\n\x07item_id\x18\x03 \x01(\x0c\x12\x10\n\x08quantity\x18\x04 \x01(\x11\"\xa2\x05\n\x05\x45vent\x12\x11\n\tsignature\x18\x01 \x01(\x0c\x12\x34\n\x0estore_manifest\x18\x02 \x01(\x0b\x32\x1a.market.mass.StoreManifestH\x00\x12\x36\n\x0fupdate_manifest\x18\x03 \x01(\x0b\x32\x1b.market.mass.UpdateManifestH\x00\x12.\n\x0b\x63reate_item\x18\x04 \x01(\x0b\x32\x17.market.mass.CreateItemH\x00\x12.\n\x0bupdate_item\x18\x05 \x01(\x0b\x32\x17.market.mass.UpdateItemH\x00\x12,\n\ncreate_tag\x18\x06 \x01(\x0b\x32\x16.market.mass.CreateTagH\x00\x12+\n\nadd_to_tag\x18\x07 \x01(\x0b\x32\x15.market.mass.AddToTagH\x00\x12\x35\n\x0fremove_from_tag\x18\x08 \x01(\x0b\x32\x1a.market.mass.RemoveFromTagH\x00\x12,\n\nrename_tag\x18\t \x01(\x0b\x32\x16.market.mass.RenameTagH\x00\x12,\n\ndelete_tag\x18\n \x01(\x0b\x32\x16.market.mass.DeleteTagH\x00\x12.\n\x0b\x63reate_cart\x18\x0b \x01(\x0b\x32\x17.market.mass.CreateCartH\x00\x12.\n\x0b\x63hange_cart\x18\x0c \x01(\x0b\x32\x17.market.mass.ChangeCartH\x00\x12\x30\n\x0c\x63hange_stock\x18\r \x01(\x0b\x32\x18.market.mass.ChangeStockH\x00\x12/\n\x0cnew_key_card\x18\x0e \x01(\x0b\x32\x17.market.mass.NewKeyCardH\x00\x42\x07\n\x05union\"=\n\x13\x41uthenticateRequest\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\x12\x12\n\npublic_key\x18\x02 \x01(\x0c\"`\n\x14\x41uthenticateResponse\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\x12!\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x12.market.mass.Error\x12\x11\n\tchallenge\x18\x03 \x01(\x0c\"?\n\x16\x43hallengeSolvedRequest\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\x12\x11\n\tsignature\x18\x02 \x01(\x0c\"P\n\x17\x43hallengeSolvedResponse\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\x12!\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x12.market.mass.Error\"L\n\x11\x43ommitCartRequest\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\x12\x0f\n\x07\x63\x61rt_id\x18\x02 \x01(\x0c\x12\x12\n\nerc20_addr\x18\x03 \x01(\x0c\"\xea\x01\n\x12\x43ommitCartResponse\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\x12!\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x12.market.mass.Error\x12\x18\n\x10purchase_address\x18\x03 \x01(\x0c\x12;\n\x06totals\x18\x04 \x03(\x0b\x32+.market.mass.CommitCartResponse.TotalsEntry\x12\x17\n\x0ftotal_in_crypto\x18\x05 \x01(\t\x1a-\n\x0bTotalsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"-\n\x17GetBlobUploadURLRequest\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\"^\n\x18GetBlobUploadURLResponse\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\x12!\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x12.market.mass.Error\x12\x0b\n\x03url\x18\x03 \x01(\t\"J\n\x11\x45ventWriteRequest\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\x12!\n\x05\x65vent\x18\x02 \x01(\x0b\x32\x12.market.mass.Event\"~\n\x12\x45ventWriteResponse\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\x12!\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x12.market.mass.Error\x12\x16\n\x0enew_store_hash\x18\x03 \x01(\x0c\x12\x19\n\x11\x65vent_sequence_no\x18\x04 \x01(\x04\"@\n\x11SyncStatusRequest\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\x12\x17\n\x0funpushed_events\x18\x02 \x01(\x04\"K\n\x12SyncStatusResponse\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\x12!\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x12.market.mass.Error\"J\n\x10\x45ventPushRequest\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\x12\"\n\x06\x65vents\x18\x02 \x03(\x0b\x32\x12.market.mass.Event\"J\n\x11\x45ventPushResponse\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\x12!\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x12.market.mass.Error\"!\n\x0bPingRequest\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\"E\n\x0cPingResponse\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\x12!\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x12.market.mass.Error\"&\n\x05\x45rror\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x0f\n\x07message\x18\x02 \x01(\tb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0cschema.proto\x12\x0bmarket.mass\"c\n\rStoreManifest\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\x12\x16\n\x0estore_token_id\x18\x02 \x01(\x0c\x12\x0e\n\x06\x64omain\x18\x03 \x01(\t\x12\x18\n\x10published_tag_id\x18\x04 \x01(\x0c\"\xcd\x02\n\x0eUpdateManifest\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\x12\x38\n\x05\x66ield\x18\x02 \x01(\x0e\x32).market.mass.UpdateManifest.ManifestField\x12\x10\n\x06string\x18\x03 \x01(\tH\x00\x12\x10\n\x06tag_id\x18\x04 \x01(\x0cH\x00\x12\x14\n\nerc20_addr\x18\x05 \x01(\x0cH\x00\"\xab\x01\n\rManifestField\x12\x1e\n\x1aMANIFEST_FIELD_UNSPECIFIED\x10\x00\x12\x19\n\x15MANIFEST_FIELD_DOMAIN\x10\x01\x12 \n\x1cMANIFEST_FIELD_PUBLISHED_TAG\x10\x02\x12\x1c\n\x18MANIFEST_FIELD_ADD_ERC20\x10\x03\x12\x1f\n\x1bMANIFEST_FIELD_REMOVE_ERC20\x10\x04\x42\x07\n\x05value\"?\n\nCreateItem\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\x12\r\n\x05price\x18\x02 \x01(\t\x12\x10\n\x08metadata\x18\x03 \x01(\x0c\"\xe7\x01\n\nUpdateItem\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\x12\x0f\n\x07item_id\x18\x02 \x01(\x0c\x12\x30\n\x05\x66ield\x18\x03 \x01(\x0e\x32!.market.mass.UpdateItem.ItemField\x12\x0f\n\x05price\x18\x04 \x01(\tH\x00\x12\x12\n\x08metadata\x18\x05 \x01(\x0cH\x00\"V\n\tItemField\x12\x1a\n\x16ITEM_FIELD_UNSPECIFIED\x10\x00\x12\x14\n\x10ITEM_FIELD_PRICE\x10\x01\x12\x17\n\x13ITEM_FIELD_METADATA\x10\x02\x42\x07\n\x05value\"+\n\tCreateTag\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\x12\x0c\n\x04name\x18\x02 \x01(\t\"=\n\x08\x41\x64\x64ToTag\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\x12\x0e\n\x06tag_id\x18\x02 \x01(\x0c\x12\x0f\n\x07item_id\x18\x03 \x01(\x0c\"B\n\rRemoveFromTag\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\x12\x0e\n\x06tag_id\x18\x02 \x01(\x0c\x12\x0f\n\x07item_id\x18\x03 \x01(\x0c\";\n\tRenameTag\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\x12\x0e\n\x06tag_id\x18\x02 \x01(\x0c\x12\x0c\n\x04name\x18\x03 \x01(\t\"-\n\tDeleteTag\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\x12\x0e\n\x06tag_id\x18\x02 \x01(\x0c\"t\n\x0b\x43hangeStock\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\x12\x10\n\x08item_ids\x18\x02 \x03(\x0c\x12\r\n\x05\x64iffs\x18\x03 \x03(\x11\x12\x0f\n\x07\x63\x61rt_id\x18\x04 \x01(\x0c\x12\x0f\n\x07tx_hash\x18\x05 \x01(\x0c\x12\x10\n\x08\x62lock_no\x18\x06 \x01(\x04\"Q\n\nNewKeyCard\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\x12\x18\n\x10user_wallet_addr\x18\x02 \x01(\x0c\x12\x17\n\x0f\x63\x61rd_public_key\x18\x03 \x01(\x0c\"\x1e\n\nCreateCart\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\"R\n\nChangeCart\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\x12\x0f\n\x07\x63\x61rt_id\x18\x02 \x01(\x0c\x12\x0f\n\x07item_id\x18\x03 \x01(\x0c\x12\x10\n\x08quantity\x18\x04 \x01(\x11\"\xa2\x05\n\x05\x45vent\x12\x11\n\tsignature\x18\x01 \x01(\x0c\x12\x34\n\x0estore_manifest\x18\x02 \x01(\x0b\x32\x1a.market.mass.StoreManifestH\x00\x12\x36\n\x0fupdate_manifest\x18\x03 \x01(\x0b\x32\x1b.market.mass.UpdateManifestH\x00\x12.\n\x0b\x63reate_item\x18\x04 \x01(\x0b\x32\x17.market.mass.CreateItemH\x00\x12.\n\x0bupdate_item\x18\x05 \x01(\x0b\x32\x17.market.mass.UpdateItemH\x00\x12,\n\ncreate_tag\x18\x06 \x01(\x0b\x32\x16.market.mass.CreateTagH\x00\x12+\n\nadd_to_tag\x18\x07 \x01(\x0b\x32\x15.market.mass.AddToTagH\x00\x12\x35\n\x0fremove_from_tag\x18\x08 \x01(\x0b\x32\x1a.market.mass.RemoveFromTagH\x00\x12,\n\nrename_tag\x18\t \x01(\x0b\x32\x16.market.mass.RenameTagH\x00\x12,\n\ndelete_tag\x18\n \x01(\x0b\x32\x16.market.mass.DeleteTagH\x00\x12.\n\x0b\x63reate_cart\x18\x0b \x01(\x0b\x32\x17.market.mass.CreateCartH\x00\x12.\n\x0b\x63hange_cart\x18\x0c \x01(\x0b\x32\x17.market.mass.ChangeCartH\x00\x12\x30\n\x0c\x63hange_stock\x18\r \x01(\x0b\x32\x18.market.mass.ChangeStockH\x00\x12/\n\x0cnew_key_card\x18\x0e \x01(\x0b\x32\x17.market.mass.NewKeyCardH\x00\x42\x07\n\x05union\"=\n\x13\x41uthenticateRequest\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\x12\x12\n\npublic_key\x18\x02 \x01(\x0c\"`\n\x14\x41uthenticateResponse\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\x12!\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x12.market.mass.Error\x12\x11\n\tchallenge\x18\x03 \x01(\x0c\"?\n\x16\x43hallengeSolvedRequest\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\x12\x11\n\tsignature\x18\x02 \x01(\x0c\"P\n\x17\x43hallengeSolvedResponse\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\x12!\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x12.market.mass.Error\"L\n\x11\x43ommitCartRequest\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\x12\x0f\n\x07\x63\x61rt_id\x18\x02 \x01(\x0c\x12\x12\n\nerc20_addr\x18\x03 \x01(\x0c\"\xea\x01\n\x12\x43ommitCartResponse\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\x12!\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x12.market.mass.Error\x12\x18\n\x10purchase_address\x18\x03 \x01(\x0c\x12;\n\x06totals\x18\x04 \x03(\x0b\x32+.market.mass.CommitCartResponse.TotalsEntry\x12\x17\n\x0ftotal_in_crypto\x18\x05 \x01(\t\x1a-\n\x0bTotalsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"-\n\x17GetBlobUploadURLRequest\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\"^\n\x18GetBlobUploadURLResponse\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\x12!\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x12.market.mass.Error\x12\x0b\n\x03url\x18\x03 \x01(\t\"J\n\x11\x45ventWriteRequest\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\x12!\n\x05\x65vent\x18\x02 \x01(\x0b\x32\x12.market.mass.Event\"~\n\x12\x45ventWriteResponse\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\x12!\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x12.market.mass.Error\x12\x16\n\x0enew_store_hash\x18\x03 \x01(\x0c\x12\x19\n\x11\x65vent_sequence_no\x18\x04 \x01(\x04\"@\n\x11SyncStatusRequest\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\x12\x17\n\x0funpushed_events\x18\x02 \x01(\x04\"K\n\x12SyncStatusResponse\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\x12!\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x12.market.mass.Error\"J\n\x10\x45ventPushRequest\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\x12\"\n\x06\x65vents\x18\x02 \x03(\x0b\x32\x12.market.mass.Event\"J\n\x11\x45ventPushResponse\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\x12!\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x12.market.mass.Error\"!\n\x0bPingRequest\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\"E\n\x0cPingResponse\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\x12!\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x12.market.mass.Error\"&\n\x05\x45rror\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x0f\n\x07message\x18\x02 \x01(\tb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'schema_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   DESCRIPTOR._options = None
   _globals['_COMMITCARTRESPONSE_TOTALSENTRY']._options = None
@@ -45,53 +41,53 @@
   _globals['_REMOVEFROMTAG']._serialized_start=873
   _globals['_REMOVEFROMTAG']._serialized_end=939
   _globals['_RENAMETAG']._serialized_start=941
   _globals['_RENAMETAG']._serialized_end=1000
   _globals['_DELETETAG']._serialized_start=1002
   _globals['_DELETETAG']._serialized_end=1047
   _globals['_CHANGESTOCK']._serialized_start=1049
-  _globals['_CHANGESTOCK']._serialized_end=1130
-  _globals['_NEWKEYCARD']._serialized_start=1132
-  _globals['_NEWKEYCARD']._serialized_end=1213
-  _globals['_CREATECART']._serialized_start=1215
-  _globals['_CREATECART']._serialized_end=1245
-  _globals['_CHANGECART']._serialized_start=1247
-  _globals['_CHANGECART']._serialized_end=1329
-  _globals['_EVENT']._serialized_start=1332
-  _globals['_EVENT']._serialized_end=2006
-  _globals['_AUTHENTICATEREQUEST']._serialized_start=2008
-  _globals['_AUTHENTICATEREQUEST']._serialized_end=2069
-  _globals['_AUTHENTICATERESPONSE']._serialized_start=2071
-  _globals['_AUTHENTICATERESPONSE']._serialized_end=2167
-  _globals['_CHALLENGESOLVEDREQUEST']._serialized_start=2169
-  _globals['_CHALLENGESOLVEDREQUEST']._serialized_end=2232
-  _globals['_CHALLENGESOLVEDRESPONSE']._serialized_start=2234
-  _globals['_CHALLENGESOLVEDRESPONSE']._serialized_end=2314
-  _globals['_COMMITCARTREQUEST']._serialized_start=2316
-  _globals['_COMMITCARTREQUEST']._serialized_end=2392
-  _globals['_COMMITCARTRESPONSE']._serialized_start=2395
-  _globals['_COMMITCARTRESPONSE']._serialized_end=2629
-  _globals['_COMMITCARTRESPONSE_TOTALSENTRY']._serialized_start=2584
-  _globals['_COMMITCARTRESPONSE_TOTALSENTRY']._serialized_end=2629
-  _globals['_GETBLOBUPLOADURLREQUEST']._serialized_start=2631
-  _globals['_GETBLOBUPLOADURLREQUEST']._serialized_end=2676
-  _globals['_GETBLOBUPLOADURLRESPONSE']._serialized_start=2678
-  _globals['_GETBLOBUPLOADURLRESPONSE']._serialized_end=2772
-  _globals['_EVENTWRITEREQUEST']._serialized_start=2774
-  _globals['_EVENTWRITEREQUEST']._serialized_end=2848
-  _globals['_EVENTWRITERESPONSE']._serialized_start=2850
-  _globals['_EVENTWRITERESPONSE']._serialized_end=2976
-  _globals['_SYNCSTATUSREQUEST']._serialized_start=2978
-  _globals['_SYNCSTATUSREQUEST']._serialized_end=3042
-  _globals['_SYNCSTATUSRESPONSE']._serialized_start=3044
-  _globals['_SYNCSTATUSRESPONSE']._serialized_end=3119
-  _globals['_EVENTPUSHREQUEST']._serialized_start=3121
-  _globals['_EVENTPUSHREQUEST']._serialized_end=3195
-  _globals['_EVENTPUSHRESPONSE']._serialized_start=3197
-  _globals['_EVENTPUSHRESPONSE']._serialized_end=3271
-  _globals['_PINGREQUEST']._serialized_start=3273
-  _globals['_PINGREQUEST']._serialized_end=3306
-  _globals['_PINGRESPONSE']._serialized_start=3308
-  _globals['_PINGRESPONSE']._serialized_end=3377
-  _globals['_ERROR']._serialized_start=3379
-  _globals['_ERROR']._serialized_end=3417
+  _globals['_CHANGESTOCK']._serialized_end=1165
+  _globals['_NEWKEYCARD']._serialized_start=1167
+  _globals['_NEWKEYCARD']._serialized_end=1248
+  _globals['_CREATECART']._serialized_start=1250
+  _globals['_CREATECART']._serialized_end=1280
+  _globals['_CHANGECART']._serialized_start=1282
+  _globals['_CHANGECART']._serialized_end=1364
+  _globals['_EVENT']._serialized_start=1367
+  _globals['_EVENT']._serialized_end=2041
+  _globals['_AUTHENTICATEREQUEST']._serialized_start=2043
+  _globals['_AUTHENTICATEREQUEST']._serialized_end=2104
+  _globals['_AUTHENTICATERESPONSE']._serialized_start=2106
+  _globals['_AUTHENTICATERESPONSE']._serialized_end=2202
+  _globals['_CHALLENGESOLVEDREQUEST']._serialized_start=2204
+  _globals['_CHALLENGESOLVEDREQUEST']._serialized_end=2267
+  _globals['_CHALLENGESOLVEDRESPONSE']._serialized_start=2269
+  _globals['_CHALLENGESOLVEDRESPONSE']._serialized_end=2349
+  _globals['_COMMITCARTREQUEST']._serialized_start=2351
+  _globals['_COMMITCARTREQUEST']._serialized_end=2427
+  _globals['_COMMITCARTRESPONSE']._serialized_start=2430
+  _globals['_COMMITCARTRESPONSE']._serialized_end=2664
+  _globals['_COMMITCARTRESPONSE_TOTALSENTRY']._serialized_start=2619
+  _globals['_COMMITCARTRESPONSE_TOTALSENTRY']._serialized_end=2664
+  _globals['_GETBLOBUPLOADURLREQUEST']._serialized_start=2666
+  _globals['_GETBLOBUPLOADURLREQUEST']._serialized_end=2711
+  _globals['_GETBLOBUPLOADURLRESPONSE']._serialized_start=2713
+  _globals['_GETBLOBUPLOADURLRESPONSE']._serialized_end=2807
+  _globals['_EVENTWRITEREQUEST']._serialized_start=2809
+  _globals['_EVENTWRITEREQUEST']._serialized_end=2883
+  _globals['_EVENTWRITERESPONSE']._serialized_start=2885
+  _globals['_EVENTWRITERESPONSE']._serialized_end=3011
+  _globals['_SYNCSTATUSREQUEST']._serialized_start=3013
+  _globals['_SYNCSTATUSREQUEST']._serialized_end=3077
+  _globals['_SYNCSTATUSRESPONSE']._serialized_start=3079
+  _globals['_SYNCSTATUSRESPONSE']._serialized_end=3154
+  _globals['_EVENTPUSHREQUEST']._serialized_start=3156
+  _globals['_EVENTPUSHREQUEST']._serialized_end=3230
+  _globals['_EVENTPUSHRESPONSE']._serialized_start=3232
+  _globals['_EVENTPUSHRESPONSE']._serialized_end=3306
+  _globals['_PINGREQUEST']._serialized_start=3308
+  _globals['_PINGREQUEST']._serialized_end=3341
+  _globals['_PINGRESPONSE']._serialized_start=3343
+  _globals['_PINGRESPONSE']._serialized_end=3412
+  _globals['_ERROR']._serialized_start=3414
+  _globals['_ERROR']._serialized_end=3452
 # @@protoc_insertion_point(module_scope)
```

### Comparing `massmarket_hash_event-0.0.5/massmarket_hash_event/schema_pb2.pyi` & `massmarket_hash_event-0.0.6/massmarket_hash_event/schema_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-# SPDX-FileCopyrightText: 2024 Mass Labs
-#
-# SPDX-License-Identifier: MIT
-
 from google.protobuf.internal import containers as _containers
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
@@ -123,24 +119,28 @@
     EVENT_ID_FIELD_NUMBER: _ClassVar[int]
     TAG_ID_FIELD_NUMBER: _ClassVar[int]
     event_id: bytes
     tag_id: bytes
     def __init__(self, event_id: _Optional[bytes] = ..., tag_id: _Optional[bytes] = ...) -> None: ...
 
 class ChangeStock(_message.Message):
-    __slots__ = ["event_id", "item_ids", "diffs", "cart_id"]
+    __slots__ = ["event_id", "item_ids", "diffs", "cart_id", "tx_hash", "block_no"]
     EVENT_ID_FIELD_NUMBER: _ClassVar[int]
     ITEM_IDS_FIELD_NUMBER: _ClassVar[int]
     DIFFS_FIELD_NUMBER: _ClassVar[int]
     CART_ID_FIELD_NUMBER: _ClassVar[int]
+    TX_HASH_FIELD_NUMBER: _ClassVar[int]
+    BLOCK_NO_FIELD_NUMBER: _ClassVar[int]
     event_id: bytes
     item_ids: _containers.RepeatedScalarFieldContainer[bytes]
     diffs: _containers.RepeatedScalarFieldContainer[int]
     cart_id: bytes
-    def __init__(self, event_id: _Optional[bytes] = ..., item_ids: _Optional[_Iterable[bytes]] = ..., diffs: _Optional[_Iterable[int]] = ..., cart_id: _Optional[bytes] = ...) -> None: ...
+    tx_hash: bytes
+    block_no: int
+    def __init__(self, event_id: _Optional[bytes] = ..., item_ids: _Optional[_Iterable[bytes]] = ..., diffs: _Optional[_Iterable[int]] = ..., cart_id: _Optional[bytes] = ..., tx_hash: _Optional[bytes] = ..., block_no: _Optional[int] = ...) -> None: ...
 
 class NewKeyCard(_message.Message):
     __slots__ = ["event_id", "user_wallet_addr", "card_public_key"]
     EVENT_ID_FIELD_NUMBER: _ClassVar[int]
     USER_WALLET_ADDR_FIELD_NUMBER: _ClassVar[int]
     CARD_PUBLIC_KEY_FIELD_NUMBER: _ClassVar[int]
     event_id: bytes
```

### Comparing `massmarket_hash_event-0.0.5/massmarket_hash_event/typedData.json` & `massmarket_hash_event-0.0.6/massmarket_hash_event/typedData.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9871794871794872%*

 * *Differences: {"'ChangeStock'": "{insert: [(4, OrderedDict([('name', 'tx_hash'), ('type', 'bytes32')])), (5, "*

 * *                  "OrderedDict([('name', 'block_no'), ('type', 'uint64')]))]}"}*

```diff
@@ -43,14 +43,22 @@
         {
             "name": "diffs",
             "type": "int32[]"
         },
         {
             "name": "cart_id",
             "type": "bytes32"
+        },
+        {
+            "name": "tx_hash",
+            "type": "bytes32"
+        },
+        {
+            "name": "block_no",
+            "type": "uint64"
         }
     ],
     "CreateCart": [
         {
             "name": "event_id",
             "type": "bytes32"
         }
```

### Comparing `massmarket_hash_event-0.0.5/massmarket_hash_event.egg-info/PKG-INFO` & `massmarket_hash_event-0.0.6/massmarket_hash_event.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: massmarket-hash-event
-Version: 0.0.5
+Version: 0.0.6
 Summary: Helper functions to hash events for signature creation and verification on Mass Market.
 Author-email: Henry Bubert <henry@mass.market>
 License: MIT
 Project-URL: Homepage, https://mass.market
 Project-URL: Repository, https://github.com/masslbs/network-schema.git
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `massmarket_hash_event-0.0.5/pyproject.toml` & `massmarket_hash_event-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "massmarket_hash_event"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
     {name = "Henry Bubert", email = "henry@mass.market"},
 ]
 description = "Helper functions to hash events for signature creation and verification on Mass Market."
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
```

### Comparing `massmarket_hash_event-0.0.5/tests/test_encode.py` & `massmarket_hash_event-0.0.6/tests/test_encode.py`

 * *Files identical despite different names*

### Comparing `massmarket_hash_event-0.0.5/tests/test_signatures.py` & `massmarket_hash_event-0.0.6/tests/test_signatures.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,27 +27,27 @@
 
 def test_hash_empty_event():
   h = Hasher(2342, "0x0a0a0a0a0a0a0a0a0a0a0a0a0a0a0a0a0a0a0a0a")
   pk = Account.from_key("0x1234567890123456789012345678901234567890123456789012345678901234")
   events = [
     (schema_pb2.Event(store_manifest=schema_pb2.StoreManifest()),
      "0x3d4abe03c92aa50e2b2d59420ea24842e2455690ef1f715e245afe5da9618040"),
-    
+
     (schema_pb2.Event(update_manifest=schema_pb2.UpdateManifest(field=schema_pb2.UpdateManifest.MANIFEST_FIELD_DOMAIN)),
       "0x29bbab0c3b2a448fba1cdd96cdf0ff95ca0000b529bc6fec098667bee841f106"),
 
     (schema_pb2.Event(create_item=schema_pb2.CreateItem()),
       "0x8225d75532d725939e5025e027de840bb5c9c3d2a13a94d17ce495bdd0cdc594"),
-    
+
     (schema_pb2.Event(update_item=schema_pb2.UpdateItem(field=schema_pb2.UpdateItem.ITEM_FIELD_PRICE)),
       "0x92a19570a7e9bc04c58c984ad7203c5bfd94149cf44eda537fe6a0aefbc9da92"),
-   
+
     (schema_pb2.Event(create_tag=schema_pb2.CreateTag()),
       "0xa517d7d534cba5e6ebaf002fe765653cbd7beb9cf035641f9c9d1f0b5d3bed74"),
-    
+
     (schema_pb2.Event(add_to_tag=schema_pb2.AddToTag()),
       "0xbc870529d724c8184c5c350aa28513b0d142b09cd54f6308dc6538c7bd25a2f0"),
 
     (schema_pb2.Event(remove_from_tag=schema_pb2.RemoveFromTag()),
       "0x83e0a83733d803fd6964123fa3b5fe96efb1390c80069ad10e065d5bfd761ade"),
 
     (schema_pb2.Event(rename_tag=schema_pb2.RenameTag()),
@@ -59,15 +59,15 @@
     (schema_pb2.Event(create_cart=schema_pb2.CreateCart()),
       "0x86d113747e19f65535e20f14ca9526e683bd0255e4b8fdaaffa87e0e1a840854"),
 
     (schema_pb2.Event(change_cart=schema_pb2.ChangeCart()),
       "0xe033b1f86a7ebe1eacdbfb332c6fe7ea0294d1eebff55b5910a248d3d2baff2b"),
 
     (schema_pb2.Event(change_stock=schema_pb2.ChangeStock()),
-      "0x06dda3da556003d920246f05238d29717768408673ebc209de3fd128391cf4d8"),
+      "0x9d11ec0688dd5a50b96d04bfbcaffd834517a3c732739184697d30036f23d703"),
 
     (schema_pb2.Event(new_key_card=schema_pb2.NewKeyCard(user_wallet_addr=random.randbytes(20))),
       "0x9260d6e77645cb1245264138f9320d28a096cdffdc2a085ccb65490a24138a7d")
   ]
   for idx, (evt, expected) in enumerate(events):
     data = h.hash_event(evt)
     signed_message = pk.sign_message(data)
@@ -112,18 +112,17 @@
     (schema_pb2.Event(update_item=schema_pb2.UpdateItem(field=schema_pb2.UpdateItem.ITEM_FIELD_PRICE, item_id=test_event_id, price="123.00")),
       "0xcdf10775185454310cf3965afab693e3de0ecb11af57f4cf3013f0341d9b47b4"),
 
     (schema_pb2.Event(update_item=schema_pb2.UpdateItem(field=schema_pb2.UpdateItem.ITEM_FIELD_METADATA, item_id=test_event_id, metadata=b'{ "name": "test" }')),
       "0x88b1733cb885c6bf06bc6d3c12b5a7c08dc66b952759d84a10a1f4c1d7ae3130"),
 
     (schema_pb2.Event(change_stock=schema_pb2.ChangeStock(item_ids=[test_event_id], diffs=[1])),
-      "0xe6c9896786eaa08950cb49cca8ed1ed5fb3c128979ea7bf0d0187e478fcd88d1"),
+      "0x9cce9ffebf0475a3c29d726c485262b673ee363b090288e63231d78bb5732e78"),
 
-    (schema_pb2.Event(change_stock=schema_pb2.ChangeStock(item_ids=[test_event_id], diffs=[1], cart_id=test_event_id)),
-      "0xe6ea42817655d37accf081666bd8d67b9fba53b7ddb8f9d7fabb305e712e2c11"),
+    (schema_pb2.Event(change_stock=schema_pb2.ChangeStock(item_ids=[test_event_id], diffs=[1], cart_id=test_event_id, tx_hash=bytes(bytearray(32)), block_no=23)),
+      "0x9cebd0af7cf5a4255d352ae3afba93b0e4272efb25e685ff6279c0d9c102beb8"),
   ]
   for idx, (evt, expected) in enumerate(events):
     data = h.hash_event(evt)
     signed_message = pk.sign_message(data)
     msg_hash = signed_message.messageHash.hex()
     assert msg_hash == expected, f"Failed on event {idx}"
-
```

