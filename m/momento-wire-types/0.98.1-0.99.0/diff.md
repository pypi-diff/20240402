# Comparing `tmp/momento_wire_types-0.98.1.tar.gz` & `tmp/momento_wire_types-0.99.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "momento_wire_types-0.98.1.tar", max compression
+gzip compressed data, was "momento_wire_types-0.99.0.tar", max compression
```

## Comparing `momento_wire_types-0.98.1.tar` & `momento_wire_types-0.99.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0      158 2023-12-15 20:46:38.115413 momento_wire_types-0.98.1/README.md
--rw-r--r--   0        0        0     3004 2023-12-15 20:47:05.215362 momento_wire_types-0.98.1/momento_wire_types/__init__.py
--rw-r--r--   0        0        0        0 2023-12-15 20:46:38.115413 momento_wire_types-0.98.1/momento_wire_types/py.typed
--rw-r--r--   0        0        0        0 2023-12-15 20:46:38.115413 momento_wire_types-0.98.1/momento_wire_types/v319/__init__.py
--rw-r--r--   0        0        0     8907 2023-12-15 20:47:01.075370 momento_wire_types-0.98.1/momento_wire_types/v319/auth_pb2.py
--rw-r--r--   0        0        0     4767 2023-12-15 20:47:04.215364 momento_wire_types-0.98.1/momento_wire_types/v319/auth_pb2.pyi
--rw-r--r--   0        0        0     5447 2023-12-15 20:47:01.019370 momento_wire_types-0.98.1/momento_wire_types/v319/auth_pb2_grpc.py
--rw-r--r--   0        0        0   103464 2023-12-15 20:47:01.075370 momento_wire_types-0.98.1/momento_wire_types/v319/cacheclient_pb2.py
--rw-r--r--   0        0        0    49703 2023-12-15 20:47:04.215364 momento_wire_types-0.98.1/momento_wire_types/v319/cacheclient_pb2.pyi
--rw-r--r--   0        0        0    64584 2023-12-15 20:47:01.023370 momento_wire_types-0.98.1/momento_wire_types/v319/cacheclient_pb2_grpc.py
--rw-r--r--   0        0        0     6236 2023-12-15 20:47:01.075370 momento_wire_types-0.98.1/momento_wire_types/v319/cachepubsub_pb2.py
--rw-r--r--   0        0        0     3068 2023-12-15 20:47:04.215364 momento_wire_types-0.98.1/momento_wire_types/v319/cachepubsub_pb2.pyi
--rw-r--r--   0        0        0     7033 2023-12-15 20:47:01.027370 momento_wire_types-0.98.1/momento_wire_types/v319/cachepubsub_pb2_grpc.py
--rw-r--r--   0        0        0    19480 2023-12-15 20:47:01.075370 momento_wire_types-0.98.1/momento_wire_types/v319/controlclient_pb2.py
--rw-r--r--   0        0        0     8342 2023-12-15 20:47:04.215364 momento_wire_types-0.98.1/momento_wire_types/v319/controlclient_pb2.pyi
--rw-r--r--   0        0        0    16964 2023-12-15 20:47:01.027370 momento_wire_types-0.98.1/momento_wire_types/v319/controlclient_pb2_grpc.py
--rw-r--r--   0        0        0     1779 2023-12-15 20:47:01.075370 momento_wire_types-0.98.1/momento_wire_types/v319/extensions_pb2.py
--rw-r--r--   0        0        0      507 2023-12-15 20:47:04.215364 momento_wire_types-0.98.1/momento_wire_types/v319/extensions_pb2.pyi
--rw-r--r--   0        0        0      159 2023-12-15 20:47:01.031370 momento_wire_types-0.98.1/momento_wire_types/v319/extensions_pb2_grpc.py
--rw-r--r--   0        0        0     9076 2023-12-15 20:47:01.075370 momento_wire_types-0.98.1/momento_wire_types/v319/permissionmessages_pb2.py
--rw-r--r--   0        0        0     5146 2023-12-15 20:47:04.215364 momento_wire_types-0.98.1/momento_wire_types/v319/permissionmessages_pb2.pyi
--rw-r--r--   0        0        0      159 2023-12-15 20:47:01.035370 momento_wire_types-0.98.1/momento_wire_types/v319/permissionmessages_pb2_grpc.py
--rw-r--r--   0        0        0     3594 2023-12-15 20:47:01.075370 momento_wire_types-0.98.1/momento_wire_types/v319/token_pb2.py
--rw-r--r--   0        0        0     1694 2023-12-15 20:47:04.215364 momento_wire_types-0.98.1/momento_wire_types/v319/token_pb2.pyi
--rw-r--r--   0        0        0     2564 2023-12-15 20:47:01.039370 momento_wire_types-0.98.1/momento_wire_types/v319/token_pb2_grpc.py
--rw-r--r--   0        0        0    26683 2023-12-15 20:47:01.075370 momento_wire_types-0.98.1/momento_wire_types/v319/vectorindex_pb2.py
--rw-r--r--   0        0        0    17576 2023-12-15 20:47:04.215364 momento_wire_types-0.98.1/momento_wire_types/v319/vectorindex_pb2.pyi
--rw-r--r--   0        0        0    10665 2023-12-15 20:47:01.039370 momento_wire_types-0.98.1/momento_wire_types/v319/vectorindex_pb2_grpc.py
--rw-r--r--   0        0        0        0 2023-12-15 20:46:38.115413 momento_wire_types-0.98.1/momento_wire_types/v4/__init__.py
--rw-r--r--   0        0        0     4318 2023-12-15 20:47:04.211364 momento_wire_types-0.98.1/momento_wire_types/v4/auth_pb2.py
--rw-r--r--   0        0        0     4767 2023-12-15 20:47:04.139364 momento_wire_types-0.98.1/momento_wire_types/v4/auth_pb2.pyi
--rw-r--r--   0        0        0     5447 2023-12-15 20:47:04.155364 momento_wire_types-0.98.1/momento_wire_types/v4/auth_pb2_grpc.py
--rw-r--r--   0        0        0    41017 2023-12-15 20:47:04.211364 momento_wire_types-0.98.1/momento_wire_types/v4/cacheclient_pb2.py
--rw-r--r--   0        0        0    49703 2023-12-15 20:47:04.139364 momento_wire_types-0.98.1/momento_wire_types/v4/cacheclient_pb2.pyi
--rw-r--r--   0        0        0    64584 2023-12-15 20:47:04.159364 momento_wire_types-0.98.1/momento_wire_types/v4/cacheclient_pb2_grpc.py
--rw-r--r--   0        0        0     3469 2023-12-15 20:47:04.211364 momento_wire_types-0.98.1/momento_wire_types/v4/cachepubsub_pb2.py
--rw-r--r--   0        0        0     3068 2023-12-15 20:47:04.139364 momento_wire_types-0.98.1/momento_wire_types/v4/cachepubsub_pb2.pyi
--rw-r--r--   0        0        0     7033 2023-12-15 20:47:04.163364 momento_wire_types-0.98.1/momento_wire_types/v4/cachepubsub_pb2_grpc.py
--rw-r--r--   0        0        0     7922 2023-12-15 20:47:04.211364 momento_wire_types-0.98.1/momento_wire_types/v4/controlclient_pb2.py
--rw-r--r--   0        0        0     8342 2023-12-15 20:47:04.139364 momento_wire_types-0.98.1/momento_wire_types/v4/controlclient_pb2.pyi
--rw-r--r--   0        0        0    16964 2023-12-15 20:47:04.167364 momento_wire_types-0.98.1/momento_wire_types/v4/controlclient_pb2_grpc.py
--rw-r--r--   0        0        0     1559 2023-12-15 20:47:04.211364 momento_wire_types-0.98.1/momento_wire_types/v4/extensions_pb2.py
--rw-r--r--   0        0        0      507 2023-12-15 20:47:04.139364 momento_wire_types-0.98.1/momento_wire_types/v4/extensions_pb2.pyi
--rw-r--r--   0        0        0      159 2023-12-15 20:47:04.167364 momento_wire_types-0.98.1/momento_wire_types/v4/extensions_pb2_grpc.py
--rw-r--r--   0        0        0     4782 2023-12-15 20:47:04.211364 momento_wire_types-0.98.1/momento_wire_types/v4/permissionmessages_pb2.py
--rw-r--r--   0        0        0     5146 2023-12-15 20:47:04.139364 momento_wire_types-0.98.1/momento_wire_types/v4/permissionmessages_pb2.pyi
--rw-r--r--   0        0        0      159 2023-12-15 20:47:04.171364 momento_wire_types-0.98.1/momento_wire_types/v4/permissionmessages_pb2_grpc.py
--rw-r--r--   0        0        0     2259 2023-12-15 20:47:04.211364 momento_wire_types-0.98.1/momento_wire_types/v4/token_pb2.py
--rw-r--r--   0        0        0     1694 2023-12-15 20:47:04.139364 momento_wire_types-0.98.1/momento_wire_types/v4/token_pb2.pyi
--rw-r--r--   0        0        0     2564 2023-12-15 20:47:04.175364 momento_wire_types-0.98.1/momento_wire_types/v4/token_pb2_grpc.py
--rw-r--r--   0        0        0    12004 2023-12-15 20:47:04.211364 momento_wire_types-0.98.1/momento_wire_types/v4/vectorindex_pb2.py
--rw-r--r--   0        0        0    17576 2023-12-15 20:47:04.139364 momento_wire_types-0.98.1/momento_wire_types/v4/vectorindex_pb2.pyi
--rw-r--r--   0        0        0    10665 2023-12-15 20:47:04.179364 momento_wire_types-0.98.1/momento_wire_types/v4/vectorindex_pb2_grpc.py
--rw-r--r--   0        0        0      986 2023-12-15 20:47:05.131362 momento_wire_types-0.98.1/pyproject.toml
--rw-r--r--   0        0        0     1348 1970-01-01 00:00:00.000000 momento_wire_types-0.98.1/PKG-INFO
+-rw-r--r--   0        0        0      158 2024-01-02 21:33:05.877073 momento_wire_types-0.99.0/README.md
+-rw-r--r--   0        0        0     3004 2024-01-02 21:33:35.904949 momento_wire_types-0.99.0/momento_wire_types/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-02 21:33:05.877073 momento_wire_types-0.99.0/momento_wire_types/py.typed
+-rw-r--r--   0        0        0        0 2024-01-02 21:33:05.877073 momento_wire_types-0.99.0/momento_wire_types/v319/__init__.py
+-rw-r--r--   0        0        0     8954 2024-01-02 21:33:31.328970 momento_wire_types-0.99.0/momento_wire_types/v319/auth_pb2.py
+-rw-r--r--   0        0        0     4883 2024-01-02 21:33:34.804954 momento_wire_types-0.99.0/momento_wire_types/v319/auth_pb2.pyi
+-rw-r--r--   0        0        0     5447 2024-01-02 21:33:31.268971 momento_wire_types-0.99.0/momento_wire_types/v319/auth_pb2_grpc.py
+-rw-r--r--   0        0        0   103464 2024-01-02 21:33:31.328970 momento_wire_types-0.99.0/momento_wire_types/v319/cacheclient_pb2.py
+-rw-r--r--   0        0        0    49703 2024-01-02 21:33:34.804954 momento_wire_types-0.99.0/momento_wire_types/v319/cacheclient_pb2.pyi
+-rw-r--r--   0        0        0    64584 2024-01-02 21:33:31.272971 momento_wire_types-0.99.0/momento_wire_types/v319/cacheclient_pb2_grpc.py
+-rw-r--r--   0        0        0     6236 2024-01-02 21:33:31.328970 momento_wire_types-0.99.0/momento_wire_types/v319/cachepubsub_pb2.py
+-rw-r--r--   0        0        0     3068 2024-01-02 21:33:34.804954 momento_wire_types-0.99.0/momento_wire_types/v319/cachepubsub_pb2.pyi
+-rw-r--r--   0        0        0     7033 2024-01-02 21:33:31.272971 momento_wire_types-0.99.0/momento_wire_types/v319/cachepubsub_pb2_grpc.py
+-rw-r--r--   0        0        0    19480 2024-01-02 21:33:31.328970 momento_wire_types-0.99.0/momento_wire_types/v319/controlclient_pb2.py
+-rw-r--r--   0        0        0     8342 2024-01-02 21:33:34.804954 momento_wire_types-0.99.0/momento_wire_types/v319/controlclient_pb2.pyi
+-rw-r--r--   0        0        0    16964 2024-01-02 21:33:31.276970 momento_wire_types-0.99.0/momento_wire_types/v319/controlclient_pb2_grpc.py
+-rw-r--r--   0        0        0     1779 2024-01-02 21:33:31.328970 momento_wire_types-0.99.0/momento_wire_types/v319/extensions_pb2.py
+-rw-r--r--   0        0        0      507 2024-01-02 21:33:34.804954 momento_wire_types-0.99.0/momento_wire_types/v319/extensions_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-01-02 21:33:31.280970 momento_wire_types-0.99.0/momento_wire_types/v319/extensions_pb2_grpc.py
+-rw-r--r--   0        0        0     9076 2024-01-02 21:33:31.328970 momento_wire_types-0.99.0/momento_wire_types/v319/permissionmessages_pb2.py
+-rw-r--r--   0        0        0     5146 2024-01-02 21:33:34.804954 momento_wire_types-0.99.0/momento_wire_types/v319/permissionmessages_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-01-02 21:33:31.284970 momento_wire_types-0.99.0/momento_wire_types/v319/permissionmessages_pb2_grpc.py
+-rw-r--r--   0        0        0     3594 2024-01-02 21:33:31.328970 momento_wire_types-0.99.0/momento_wire_types/v319/token_pb2.py
+-rw-r--r--   0        0        0     1694 2024-01-02 21:33:34.804954 momento_wire_types-0.99.0/momento_wire_types/v319/token_pb2.pyi
+-rw-r--r--   0        0        0     2564 2024-01-02 21:33:31.288970 momento_wire_types-0.99.0/momento_wire_types/v319/token_pb2_grpc.py
+-rw-r--r--   0        0        0    26683 2024-01-02 21:33:31.328970 momento_wire_types-0.99.0/momento_wire_types/v319/vectorindex_pb2.py
+-rw-r--r--   0        0        0    17576 2024-01-02 21:33:34.804954 momento_wire_types-0.99.0/momento_wire_types/v319/vectorindex_pb2.pyi
+-rw-r--r--   0        0        0    10665 2024-01-02 21:33:31.288970 momento_wire_types-0.99.0/momento_wire_types/v319/vectorindex_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2024-01-02 21:33:05.877073 momento_wire_types-0.99.0/momento_wire_types/v4/__init__.py
+-rw-r--r--   0        0        0     4365 2024-01-02 21:33:34.800954 momento_wire_types-0.99.0/momento_wire_types/v4/auth_pb2.py
+-rw-r--r--   0        0        0     4883 2024-01-02 21:33:34.724954 momento_wire_types-0.99.0/momento_wire_types/v4/auth_pb2.pyi
+-rw-r--r--   0        0        0     5447 2024-01-02 21:33:34.744954 momento_wire_types-0.99.0/momento_wire_types/v4/auth_pb2_grpc.py
+-rw-r--r--   0        0        0    41017 2024-01-02 21:33:34.800954 momento_wire_types-0.99.0/momento_wire_types/v4/cacheclient_pb2.py
+-rw-r--r--   0        0        0    49703 2024-01-02 21:33:34.724954 momento_wire_types-0.99.0/momento_wire_types/v4/cacheclient_pb2.pyi
+-rw-r--r--   0        0        0    64584 2024-01-02 21:33:34.748954 momento_wire_types-0.99.0/momento_wire_types/v4/cacheclient_pb2_grpc.py
+-rw-r--r--   0        0        0     3469 2024-01-02 21:33:34.800954 momento_wire_types-0.99.0/momento_wire_types/v4/cachepubsub_pb2.py
+-rw-r--r--   0        0        0     3068 2024-01-02 21:33:34.724954 momento_wire_types-0.99.0/momento_wire_types/v4/cachepubsub_pb2.pyi
+-rw-r--r--   0        0        0     7033 2024-01-02 21:33:34.752954 momento_wire_types-0.99.0/momento_wire_types/v4/cachepubsub_pb2_grpc.py
+-rw-r--r--   0        0        0     7922 2024-01-02 21:33:34.800954 momento_wire_types-0.99.0/momento_wire_types/v4/controlclient_pb2.py
+-rw-r--r--   0        0        0     8342 2024-01-02 21:33:34.724954 momento_wire_types-0.99.0/momento_wire_types/v4/controlclient_pb2.pyi
+-rw-r--r--   0        0        0    16964 2024-01-02 21:33:34.752954 momento_wire_types-0.99.0/momento_wire_types/v4/controlclient_pb2_grpc.py
+-rw-r--r--   0        0        0     1559 2024-01-02 21:33:34.800954 momento_wire_types-0.99.0/momento_wire_types/v4/extensions_pb2.py
+-rw-r--r--   0        0        0      507 2024-01-02 21:33:34.724954 momento_wire_types-0.99.0/momento_wire_types/v4/extensions_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-01-02 21:33:34.756954 momento_wire_types-0.99.0/momento_wire_types/v4/extensions_pb2_grpc.py
+-rw-r--r--   0        0        0     4782 2024-01-02 21:33:34.800954 momento_wire_types-0.99.0/momento_wire_types/v4/permissionmessages_pb2.py
+-rw-r--r--   0        0        0     5146 2024-01-02 21:33:34.724954 momento_wire_types-0.99.0/momento_wire_types/v4/permissionmessages_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-01-02 21:33:34.760954 momento_wire_types-0.99.0/momento_wire_types/v4/permissionmessages_pb2_grpc.py
+-rw-r--r--   0        0        0     2259 2024-01-02 21:33:34.800954 momento_wire_types-0.99.0/momento_wire_types/v4/token_pb2.py
+-rw-r--r--   0        0        0     1694 2024-01-02 21:33:34.724954 momento_wire_types-0.99.0/momento_wire_types/v4/token_pb2.pyi
+-rw-r--r--   0        0        0     2564 2024-01-02 21:33:34.764954 momento_wire_types-0.99.0/momento_wire_types/v4/token_pb2_grpc.py
+-rw-r--r--   0        0        0    12004 2024-01-02 21:33:34.800954 momento_wire_types-0.99.0/momento_wire_types/v4/vectorindex_pb2.py
+-rw-r--r--   0        0        0    17576 2024-01-02 21:33:34.724954 momento_wire_types-0.99.0/momento_wire_types/v4/vectorindex_pb2.pyi
+-rw-r--r--   0        0        0    10665 2024-01-02 21:33:34.768954 momento_wire_types-0.99.0/momento_wire_types/v4/vectorindex_pb2_grpc.py
+-rw-r--r--   0        0        0      986 2024-01-02 21:33:35.784950 momento_wire_types-0.99.0/pyproject.toml
+-rw-r--r--   0        0        0     1348 1970-01-01 00:00:00.000000 momento_wire_types-0.99.0/PKG-INFO
```

### Comparing `momento_wire_types-0.98.1/momento_wire_types/__init__.py` & `momento_wire_types-0.99.0/momento_wire_types/__init__.py`

 * *Files identical despite different names*

### Comparing `momento_wire_types-0.98.1/momento_wire_types/v319/auth_pb2.py` & `momento_wire_types-0.99.0/momento_wire_types/v319/auth_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from . import permissionmessages_pb2 as permissionmessages__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\nauth.proto\x12\x04\x61uth\x1a\x18permissionmessages.proto\"\x0f\n\r_LoginRequest\"\xfc\x02\n\x0e_LoginResponse\x12<\n\x0e\x64irect_browser\x18\x01 \x01(\x0b\x32\".auth._LoginResponse.DirectBrowserH\x00\x12\x32\n\tlogged_in\x18\x02 \x01(\x0b\x32\x1d.auth._LoginResponse.LoggedInH\x00\x12/\n\x07message\x18\x03 \x01(\x0b\x32\x1c.auth._LoginResponse.MessageH\x00\x12+\n\x05\x65rror\x18\x04 \x01(\x0b\x32\x1a.auth._LoginResponse.ErrorH\x00\x1a<\n\x08LoggedIn\x12\x15\n\rsession_token\x18\x01 \x01(\t\x12\x19\n\x11valid_for_seconds\x18\x02 \x01(\r\x1a\x1c\n\x05\x45rror\x12\x13\n\x0b\x64\x65scription\x18\x01 \x01(\t\x1a\x1c\n\rDirectBrowser\x12\x0b\n\x03url\x18\x01 \x01(\t\x1a\x17\n\x07Message\x12\x0c\n\x04text\x18\x01 \x01(\tB\x07\n\x05state\"\xa2\x02\n\x18_GenerateApiTokenRequest\x12\x35\n\x05never\x18\x01 \x01(\x0b\x32$.auth._GenerateApiTokenRequest.NeverH\x00\x12\x39\n\x07\x65xpires\x18\x02 \x01(\x0b\x32&.auth._GenerateApiTokenRequest.ExpiresH\x00\x12\x12\n\nauth_token\x18\x03 \x01(\t\x12\x35\n\x0bpermissions\x18\x04 \x01(\x0b\x32 .permission_messages.Permissions\x12\x10\n\x08token_id\x18\x05 \x01(\t\x1a\x07\n\x05Never\x1a$\n\x07\x45xpires\x12\x19\n\x11valid_for_seconds\x18\x01 \x01(\rB\x08\n\x06\x65xpiry\"j\n\x19_GenerateApiTokenResponse\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x15\n\rrefresh_token\x18\x02 \x01(\t\x12\x10\n\x08\x65ndpoint\x18\x03 \x01(\t\x12\x13\n\x0bvalid_until\x18\x04 \x01(\x04\"A\n\x17_RefreshApiTokenRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x15\n\rrefresh_token\x18\x02 \x01(\t\"i\n\x18_RefreshApiTokenResponse\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x15\n\rrefresh_token\x18\x02 \x01(\t\x12\x10\n\x08\x65ndpoint\x18\x03 \x01(\t\x12\x13\n\x0bvalid_until\x18\x04 \x01(\x04\x32\xe9\x01\n\x04\x41uth\x12\x36\n\x05Login\x12\x13.auth._LoginRequest\x1a\x14.auth._LoginResponse\"\x00\x30\x01\x12U\n\x10GenerateApiToken\x12\x1e.auth._GenerateApiTokenRequest\x1a\x1f.auth._GenerateApiTokenResponse\"\x00\x12R\n\x0fRefreshApiToken\x12\x1d.auth._RefreshApiTokenRequest\x1a\x1e.auth._RefreshApiTokenResponse\"\x00\x42\x42\n\x0cmomento.authP\x01Z0github.com/momentohq/client-sdk-go;client_sdk_gob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\nauth.proto\x12\x04\x61uth\x1a\x18permissionmessages.proto\"\x0f\n\r_LoginRequest\"\xfc\x02\n\x0e_LoginResponse\x12<\n\x0e\x64irect_browser\x18\x01 \x01(\x0b\x32\".auth._LoginResponse.DirectBrowserH\x00\x12\x32\n\tlogged_in\x18\x02 \x01(\x0b\x32\x1d.auth._LoginResponse.LoggedInH\x00\x12/\n\x07message\x18\x03 \x01(\x0b\x32\x1c.auth._LoginResponse.MessageH\x00\x12+\n\x05\x65rror\x18\x04 \x01(\x0b\x32\x1a.auth._LoginResponse.ErrorH\x00\x1a<\n\x08LoggedIn\x12\x15\n\rsession_token\x18\x01 \x01(\t\x12\x19\n\x11valid_for_seconds\x18\x02 \x01(\r\x1a\x1c\n\x05\x45rror\x12\x13\n\x0b\x64\x65scription\x18\x01 \x01(\t\x1a\x1c\n\rDirectBrowser\x12\x0b\n\x03url\x18\x01 \x01(\t\x1a\x17\n\x07Message\x12\x0c\n\x04text\x18\x01 \x01(\tB\x07\n\x05state\"\xb7\x02\n\x18_GenerateApiTokenRequest\x12\x35\n\x05never\x18\x01 \x01(\x0b\x32$.auth._GenerateApiTokenRequest.NeverH\x00\x12\x39\n\x07\x65xpires\x18\x02 \x01(\x0b\x32&.auth._GenerateApiTokenRequest.ExpiresH\x00\x12\x12\n\nauth_token\x18\x03 \x01(\t\x12\x35\n\x0bpermissions\x18\x04 \x01(\x0b\x32 .permission_messages.Permissions\x12\x10\n\x08token_id\x18\x05 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x06 \x01(\t\x1a\x07\n\x05Never\x1a$\n\x07\x45xpires\x12\x19\n\x11valid_for_seconds\x18\x01 \x01(\rB\x08\n\x06\x65xpiry\"j\n\x19_GenerateApiTokenResponse\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x15\n\rrefresh_token\x18\x02 \x01(\t\x12\x10\n\x08\x65ndpoint\x18\x03 \x01(\t\x12\x13\n\x0bvalid_until\x18\x04 \x01(\x04\"A\n\x17_RefreshApiTokenRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x15\n\rrefresh_token\x18\x02 \x01(\t\"i\n\x18_RefreshApiTokenResponse\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x15\n\rrefresh_token\x18\x02 \x01(\t\x12\x10\n\x08\x65ndpoint\x18\x03 \x01(\t\x12\x13\n\x0bvalid_until\x18\x04 \x01(\x04\x32\xe9\x01\n\x04\x41uth\x12\x36\n\x05Login\x12\x13.auth._LoginRequest\x1a\x14.auth._LoginResponse\"\x00\x30\x01\x12U\n\x10GenerateApiToken\x12\x1e.auth._GenerateApiTokenRequest\x1a\x1f.auth._GenerateApiTokenResponse\"\x00\x12R\n\x0fRefreshApiToken\x12\x1d.auth._RefreshApiTokenRequest\x1a\x1e.auth._RefreshApiTokenResponse\"\x00\x42\x42\n\x0cmomento.authP\x01Z0github.com/momentohq/client-sdk-go;client_sdk_gob\x06proto3')
 
 
 
 __LOGINREQUEST = DESCRIPTOR.message_types_by_name['_LoginRequest']
 __LOGINRESPONSE = DESCRIPTOR.message_types_by_name['_LoginResponse']
 __LOGINRESPONSE_LOGGEDIN = __LOGINRESPONSE.nested_types_by_name['LoggedIn']
 __LOGINRESPONSE_ERROR = __LOGINRESPONSE.nested_types_by_name['Error']
@@ -135,21 +135,21 @@
   __LOGINRESPONSE_ERROR._serialized_start=352
   __LOGINRESPONSE_ERROR._serialized_end=380
   __LOGINRESPONSE_DIRECTBROWSER._serialized_start=382
   __LOGINRESPONSE_DIRECTBROWSER._serialized_end=410
   __LOGINRESPONSE_MESSAGE._serialized_start=412
   __LOGINRESPONSE_MESSAGE._serialized_end=435
   __GENERATEAPITOKENREQUEST._serialized_start=447
-  __GENERATEAPITOKENREQUEST._serialized_end=737
-  __GENERATEAPITOKENREQUEST_NEVER._serialized_start=682
-  __GENERATEAPITOKENREQUEST_NEVER._serialized_end=689
-  __GENERATEAPITOKENREQUEST_EXPIRES._serialized_start=691
-  __GENERATEAPITOKENREQUEST_EXPIRES._serialized_end=727
-  __GENERATEAPITOKENRESPONSE._serialized_start=739
-  __GENERATEAPITOKENRESPONSE._serialized_end=845
-  __REFRESHAPITOKENREQUEST._serialized_start=847
-  __REFRESHAPITOKENREQUEST._serialized_end=912
-  __REFRESHAPITOKENRESPONSE._serialized_start=914
-  __REFRESHAPITOKENRESPONSE._serialized_end=1019
-  _AUTH._serialized_start=1022
-  _AUTH._serialized_end=1255
+  __GENERATEAPITOKENREQUEST._serialized_end=758
+  __GENERATEAPITOKENREQUEST_NEVER._serialized_start=703
+  __GENERATEAPITOKENREQUEST_NEVER._serialized_end=710
+  __GENERATEAPITOKENREQUEST_EXPIRES._serialized_start=712
+  __GENERATEAPITOKENREQUEST_EXPIRES._serialized_end=748
+  __GENERATEAPITOKENRESPONSE._serialized_start=760
+  __GENERATEAPITOKENRESPONSE._serialized_end=866
+  __REFRESHAPITOKENREQUEST._serialized_start=868
+  __REFRESHAPITOKENREQUEST._serialized_end=933
+  __REFRESHAPITOKENRESPONSE._serialized_start=935
+  __REFRESHAPITOKENRESPONSE._serialized_end=1040
+  _AUTH._serialized_start=1043
+  _AUTH._serialized_end=1276
 # @@protoc_insertion_point(module_scope)
```

### Comparing `momento_wire_types-0.98.1/momento_wire_types/v319/auth_pb2.pyi` & `momento_wire_types-0.99.0/momento_wire_types/v319/auth_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -2,34 +2,36 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class _GenerateApiTokenRequest(_message.Message):
-    __slots__ = ["auth_token", "expires", "never", "permissions", "token_id"]
+    __slots__ = ["auth_token", "description", "expires", "never", "permissions", "token_id"]
     class Expires(_message.Message):
         __slots__ = ["valid_for_seconds"]
         VALID_FOR_SECONDS_FIELD_NUMBER: _ClassVar[int]
         valid_for_seconds: int
         def __init__(self, valid_for_seconds: _Optional[int] = ...) -> None: ...
     class Never(_message.Message):
         __slots__ = []
         def __init__(self) -> None: ...
     AUTH_TOKEN_FIELD_NUMBER: _ClassVar[int]
+    DESCRIPTION_FIELD_NUMBER: _ClassVar[int]
     EXPIRES_FIELD_NUMBER: _ClassVar[int]
     NEVER_FIELD_NUMBER: _ClassVar[int]
     PERMISSIONS_FIELD_NUMBER: _ClassVar[int]
     TOKEN_ID_FIELD_NUMBER: _ClassVar[int]
     auth_token: str
+    description: str
     expires: _GenerateApiTokenRequest.Expires
     never: _GenerateApiTokenRequest.Never
     permissions: _permissionmessages_pb2.Permissions
     token_id: str
-    def __init__(self, never: _Optional[_Union[_GenerateApiTokenRequest.Never, _Mapping]] = ..., expires: _Optional[_Union[_GenerateApiTokenRequest.Expires, _Mapping]] = ..., auth_token: _Optional[str] = ..., permissions: _Optional[_Union[_permissionmessages_pb2.Permissions, _Mapping]] = ..., token_id: _Optional[str] = ...) -> None: ...
+    def __init__(self, never: _Optional[_Union[_GenerateApiTokenRequest.Never, _Mapping]] = ..., expires: _Optional[_Union[_GenerateApiTokenRequest.Expires, _Mapping]] = ..., auth_token: _Optional[str] = ..., permissions: _Optional[_Union[_permissionmessages_pb2.Permissions, _Mapping]] = ..., token_id: _Optional[str] = ..., description: _Optional[str] = ...) -> None: ...
 
 class _GenerateApiTokenResponse(_message.Message):
     __slots__ = ["api_key", "endpoint", "refresh_token", "valid_until"]
     API_KEY_FIELD_NUMBER: _ClassVar[int]
     ENDPOINT_FIELD_NUMBER: _ClassVar[int]
     REFRESH_TOKEN_FIELD_NUMBER: _ClassVar[int]
     VALID_UNTIL_FIELD_NUMBER: _ClassVar[int]
```

### Comparing `momento_wire_types-0.98.1/momento_wire_types/v319/auth_pb2_grpc.py` & `momento_wire_types-0.99.0/momento_wire_types/v319/auth_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `momento_wire_types-0.98.1/momento_wire_types/v319/cacheclient_pb2.py` & `momento_wire_types-0.99.0/momento_wire_types/v319/cacheclient_pb2.py`

 * *Files identical despite different names*

### Comparing `momento_wire_types-0.98.1/momento_wire_types/v319/cacheclient_pb2.pyi` & `momento_wire_types-0.99.0/momento_wire_types/v319/cacheclient_pb2.pyi`

 * *Files identical despite different names*

### Comparing `momento_wire_types-0.98.1/momento_wire_types/v319/cacheclient_pb2_grpc.py` & `momento_wire_types-0.99.0/momento_wire_types/v319/cacheclient_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `momento_wire_types-0.98.1/momento_wire_types/v319/cachepubsub_pb2.py` & `momento_wire_types-0.99.0/momento_wire_types/v319/cachepubsub_pb2.py`

 * *Files identical despite different names*

### Comparing `momento_wire_types-0.98.1/momento_wire_types/v319/cachepubsub_pb2.pyi` & `momento_wire_types-0.99.0/momento_wire_types/v319/cachepubsub_pb2.pyi`

 * *Files identical despite different names*

### Comparing `momento_wire_types-0.98.1/momento_wire_types/v319/cachepubsub_pb2_grpc.py` & `momento_wire_types-0.99.0/momento_wire_types/v319/cachepubsub_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `momento_wire_types-0.98.1/momento_wire_types/v319/controlclient_pb2.py` & `momento_wire_types-0.99.0/momento_wire_types/v319/controlclient_pb2.py`

 * *Files identical despite different names*

### Comparing `momento_wire_types-0.98.1/momento_wire_types/v319/controlclient_pb2.pyi` & `momento_wire_types-0.99.0/momento_wire_types/v319/controlclient_pb2.pyi`

 * *Files identical despite different names*

### Comparing `momento_wire_types-0.98.1/momento_wire_types/v319/controlclient_pb2_grpc.py` & `momento_wire_types-0.99.0/momento_wire_types/v319/controlclient_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `momento_wire_types-0.98.1/momento_wire_types/v319/extensions_pb2.py` & `momento_wire_types-0.99.0/momento_wire_types/v319/extensions_pb2.py`

 * *Files identical despite different names*

### Comparing `momento_wire_types-0.98.1/momento_wire_types/v319/permissionmessages_pb2.py` & `momento_wire_types-0.99.0/momento_wire_types/v319/permissionmessages_pb2.py`

 * *Files identical despite different names*

### Comparing `momento_wire_types-0.98.1/momento_wire_types/v319/permissionmessages_pb2.pyi` & `momento_wire_types-0.99.0/momento_wire_types/v319/permissionmessages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `momento_wire_types-0.98.1/momento_wire_types/v319/token_pb2.py` & `momento_wire_types-0.99.0/momento_wire_types/v319/token_pb2.py`

 * *Files identical despite different names*

### Comparing `momento_wire_types-0.98.1/momento_wire_types/v319/token_pb2.pyi` & `momento_wire_types-0.99.0/momento_wire_types/v319/token_pb2.pyi`

 * *Files identical despite different names*

### Comparing `momento_wire_types-0.98.1/momento_wire_types/v319/token_pb2_grpc.py` & `momento_wire_types-0.99.0/momento_wire_types/v319/token_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `momento_wire_types-0.98.1/momento_wire_types/v319/vectorindex_pb2.py` & `momento_wire_types-0.99.0/momento_wire_types/v319/vectorindex_pb2.py`

 * *Files identical despite different names*

### Comparing `momento_wire_types-0.98.1/momento_wire_types/v319/vectorindex_pb2.pyi` & `momento_wire_types-0.99.0/momento_wire_types/v319/vectorindex_pb2.pyi`

 * *Files identical despite different names*

### Comparing `momento_wire_types-0.98.1/momento_wire_types/v319/vectorindex_pb2_grpc.py` & `momento_wire_types-0.99.0/momento_wire_types/v319/vectorindex_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `momento_wire_types-0.98.1/momento_wire_types/v4/auth_pb2.py` & `momento_wire_types-0.99.0/momento_wire_types/v4/auth_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from . import permissionmessages_pb2 as permissionmessages__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\nauth.proto\x12\x04\x61uth\x1a\x18permissionmessages.proto\"\x0f\n\r_LoginRequest\"\xfc\x02\n\x0e_LoginResponse\x12<\n\x0e\x64irect_browser\x18\x01 \x01(\x0b\x32\".auth._LoginResponse.DirectBrowserH\x00\x12\x32\n\tlogged_in\x18\x02 \x01(\x0b\x32\x1d.auth._LoginResponse.LoggedInH\x00\x12/\n\x07message\x18\x03 \x01(\x0b\x32\x1c.auth._LoginResponse.MessageH\x00\x12+\n\x05\x65rror\x18\x04 \x01(\x0b\x32\x1a.auth._LoginResponse.ErrorH\x00\x1a<\n\x08LoggedIn\x12\x15\n\rsession_token\x18\x01 \x01(\t\x12\x19\n\x11valid_for_seconds\x18\x02 \x01(\r\x1a\x1c\n\x05\x45rror\x12\x13\n\x0b\x64\x65scription\x18\x01 \x01(\t\x1a\x1c\n\rDirectBrowser\x12\x0b\n\x03url\x18\x01 \x01(\t\x1a\x17\n\x07Message\x12\x0c\n\x04text\x18\x01 \x01(\tB\x07\n\x05state\"\xa2\x02\n\x18_GenerateApiTokenRequest\x12\x35\n\x05never\x18\x01 \x01(\x0b\x32$.auth._GenerateApiTokenRequest.NeverH\x00\x12\x39\n\x07\x65xpires\x18\x02 \x01(\x0b\x32&.auth._GenerateApiTokenRequest.ExpiresH\x00\x12\x12\n\nauth_token\x18\x03 \x01(\t\x12\x35\n\x0bpermissions\x18\x04 \x01(\x0b\x32 .permission_messages.Permissions\x12\x10\n\x08token_id\x18\x05 \x01(\t\x1a\x07\n\x05Never\x1a$\n\x07\x45xpires\x12\x19\n\x11valid_for_seconds\x18\x01 \x01(\rB\x08\n\x06\x65xpiry\"j\n\x19_GenerateApiTokenResponse\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x15\n\rrefresh_token\x18\x02 \x01(\t\x12\x10\n\x08\x65ndpoint\x18\x03 \x01(\t\x12\x13\n\x0bvalid_until\x18\x04 \x01(\x04\"A\n\x17_RefreshApiTokenRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x15\n\rrefresh_token\x18\x02 \x01(\t\"i\n\x18_RefreshApiTokenResponse\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x15\n\rrefresh_token\x18\x02 \x01(\t\x12\x10\n\x08\x65ndpoint\x18\x03 \x01(\t\x12\x13\n\x0bvalid_until\x18\x04 \x01(\x04\x32\xe9\x01\n\x04\x41uth\x12\x36\n\x05Login\x12\x13.auth._LoginRequest\x1a\x14.auth._LoginResponse\"\x00\x30\x01\x12U\n\x10GenerateApiToken\x12\x1e.auth._GenerateApiTokenRequest\x1a\x1f.auth._GenerateApiTokenResponse\"\x00\x12R\n\x0fRefreshApiToken\x12\x1d.auth._RefreshApiTokenRequest\x1a\x1e.auth._RefreshApiTokenResponse\"\x00\x42\x42\n\x0cmomento.authP\x01Z0github.com/momentohq/client-sdk-go;client_sdk_gob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\nauth.proto\x12\x04\x61uth\x1a\x18permissionmessages.proto\"\x0f\n\r_LoginRequest\"\xfc\x02\n\x0e_LoginResponse\x12<\n\x0e\x64irect_browser\x18\x01 \x01(\x0b\x32\".auth._LoginResponse.DirectBrowserH\x00\x12\x32\n\tlogged_in\x18\x02 \x01(\x0b\x32\x1d.auth._LoginResponse.LoggedInH\x00\x12/\n\x07message\x18\x03 \x01(\x0b\x32\x1c.auth._LoginResponse.MessageH\x00\x12+\n\x05\x65rror\x18\x04 \x01(\x0b\x32\x1a.auth._LoginResponse.ErrorH\x00\x1a<\n\x08LoggedIn\x12\x15\n\rsession_token\x18\x01 \x01(\t\x12\x19\n\x11valid_for_seconds\x18\x02 \x01(\r\x1a\x1c\n\x05\x45rror\x12\x13\n\x0b\x64\x65scription\x18\x01 \x01(\t\x1a\x1c\n\rDirectBrowser\x12\x0b\n\x03url\x18\x01 \x01(\t\x1a\x17\n\x07Message\x12\x0c\n\x04text\x18\x01 \x01(\tB\x07\n\x05state\"\xb7\x02\n\x18_GenerateApiTokenRequest\x12\x35\n\x05never\x18\x01 \x01(\x0b\x32$.auth._GenerateApiTokenRequest.NeverH\x00\x12\x39\n\x07\x65xpires\x18\x02 \x01(\x0b\x32&.auth._GenerateApiTokenRequest.ExpiresH\x00\x12\x12\n\nauth_token\x18\x03 \x01(\t\x12\x35\n\x0bpermissions\x18\x04 \x01(\x0b\x32 .permission_messages.Permissions\x12\x10\n\x08token_id\x18\x05 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x06 \x01(\t\x1a\x07\n\x05Never\x1a$\n\x07\x45xpires\x12\x19\n\x11valid_for_seconds\x18\x01 \x01(\rB\x08\n\x06\x65xpiry\"j\n\x19_GenerateApiTokenResponse\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x15\n\rrefresh_token\x18\x02 \x01(\t\x12\x10\n\x08\x65ndpoint\x18\x03 \x01(\t\x12\x13\n\x0bvalid_until\x18\x04 \x01(\x04\"A\n\x17_RefreshApiTokenRequest\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x15\n\rrefresh_token\x18\x02 \x01(\t\"i\n\x18_RefreshApiTokenResponse\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\x12\x15\n\rrefresh_token\x18\x02 \x01(\t\x12\x10\n\x08\x65ndpoint\x18\x03 \x01(\t\x12\x13\n\x0bvalid_until\x18\x04 \x01(\x04\x32\xe9\x01\n\x04\x41uth\x12\x36\n\x05Login\x12\x13.auth._LoginRequest\x1a\x14.auth._LoginResponse\"\x00\x30\x01\x12U\n\x10GenerateApiToken\x12\x1e.auth._GenerateApiTokenRequest\x1a\x1f.auth._GenerateApiTokenResponse\"\x00\x12R\n\x0fRefreshApiToken\x12\x1d.auth._RefreshApiTokenRequest\x1a\x1e.auth._RefreshApiTokenResponse\"\x00\x42\x42\n\x0cmomento.authP\x01Z0github.com/momentohq/client-sdk-go;client_sdk_gob\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'auth_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\014momento.authP\001Z0github.com/momentohq/client-sdk-go;client_sdk_go'
@@ -31,21 +31,21 @@
   __LOGINRESPONSE_ERROR._serialized_start=352
   __LOGINRESPONSE_ERROR._serialized_end=380
   __LOGINRESPONSE_DIRECTBROWSER._serialized_start=382
   __LOGINRESPONSE_DIRECTBROWSER._serialized_end=410
   __LOGINRESPONSE_MESSAGE._serialized_start=412
   __LOGINRESPONSE_MESSAGE._serialized_end=435
   __GENERATEAPITOKENREQUEST._serialized_start=447
-  __GENERATEAPITOKENREQUEST._serialized_end=737
-  __GENERATEAPITOKENREQUEST_NEVER._serialized_start=682
-  __GENERATEAPITOKENREQUEST_NEVER._serialized_end=689
-  __GENERATEAPITOKENREQUEST_EXPIRES._serialized_start=691
-  __GENERATEAPITOKENREQUEST_EXPIRES._serialized_end=727
-  __GENERATEAPITOKENRESPONSE._serialized_start=739
-  __GENERATEAPITOKENRESPONSE._serialized_end=845
-  __REFRESHAPITOKENREQUEST._serialized_start=847
-  __REFRESHAPITOKENREQUEST._serialized_end=912
-  __REFRESHAPITOKENRESPONSE._serialized_start=914
-  __REFRESHAPITOKENRESPONSE._serialized_end=1019
-  _AUTH._serialized_start=1022
-  _AUTH._serialized_end=1255
+  __GENERATEAPITOKENREQUEST._serialized_end=758
+  __GENERATEAPITOKENREQUEST_NEVER._serialized_start=703
+  __GENERATEAPITOKENREQUEST_NEVER._serialized_end=710
+  __GENERATEAPITOKENREQUEST_EXPIRES._serialized_start=712
+  __GENERATEAPITOKENREQUEST_EXPIRES._serialized_end=748
+  __GENERATEAPITOKENRESPONSE._serialized_start=760
+  __GENERATEAPITOKENRESPONSE._serialized_end=866
+  __REFRESHAPITOKENREQUEST._serialized_start=868
+  __REFRESHAPITOKENREQUEST._serialized_end=933
+  __REFRESHAPITOKENRESPONSE._serialized_start=935
+  __REFRESHAPITOKENRESPONSE._serialized_end=1040
+  _AUTH._serialized_start=1043
+  _AUTH._serialized_end=1276
 # @@protoc_insertion_point(module_scope)
```

### Comparing `momento_wire_types-0.98.1/momento_wire_types/v4/auth_pb2.pyi` & `momento_wire_types-0.99.0/momento_wire_types/v4/auth_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -2,34 +2,36 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class _GenerateApiTokenRequest(_message.Message):
-    __slots__ = ["auth_token", "expires", "never", "permissions", "token_id"]
+    __slots__ = ["auth_token", "description", "expires", "never", "permissions", "token_id"]
     class Expires(_message.Message):
         __slots__ = ["valid_for_seconds"]
         VALID_FOR_SECONDS_FIELD_NUMBER: _ClassVar[int]
         valid_for_seconds: int
         def __init__(self, valid_for_seconds: _Optional[int] = ...) -> None: ...
     class Never(_message.Message):
         __slots__ = []
         def __init__(self) -> None: ...
     AUTH_TOKEN_FIELD_NUMBER: _ClassVar[int]
+    DESCRIPTION_FIELD_NUMBER: _ClassVar[int]
     EXPIRES_FIELD_NUMBER: _ClassVar[int]
     NEVER_FIELD_NUMBER: _ClassVar[int]
     PERMISSIONS_FIELD_NUMBER: _ClassVar[int]
     TOKEN_ID_FIELD_NUMBER: _ClassVar[int]
     auth_token: str
+    description: str
     expires: _GenerateApiTokenRequest.Expires
     never: _GenerateApiTokenRequest.Never
     permissions: _permissionmessages_pb2.Permissions
     token_id: str
-    def __init__(self, never: _Optional[_Union[_GenerateApiTokenRequest.Never, _Mapping]] = ..., expires: _Optional[_Union[_GenerateApiTokenRequest.Expires, _Mapping]] = ..., auth_token: _Optional[str] = ..., permissions: _Optional[_Union[_permissionmessages_pb2.Permissions, _Mapping]] = ..., token_id: _Optional[str] = ...) -> None: ...
+    def __init__(self, never: _Optional[_Union[_GenerateApiTokenRequest.Never, _Mapping]] = ..., expires: _Optional[_Union[_GenerateApiTokenRequest.Expires, _Mapping]] = ..., auth_token: _Optional[str] = ..., permissions: _Optional[_Union[_permissionmessages_pb2.Permissions, _Mapping]] = ..., token_id: _Optional[str] = ..., description: _Optional[str] = ...) -> None: ...
 
 class _GenerateApiTokenResponse(_message.Message):
     __slots__ = ["api_key", "endpoint", "refresh_token", "valid_until"]
     API_KEY_FIELD_NUMBER: _ClassVar[int]
     ENDPOINT_FIELD_NUMBER: _ClassVar[int]
     REFRESH_TOKEN_FIELD_NUMBER: _ClassVar[int]
     VALID_UNTIL_FIELD_NUMBER: _ClassVar[int]
```

### Comparing `momento_wire_types-0.98.1/momento_wire_types/v4/auth_pb2_grpc.py` & `momento_wire_types-0.99.0/momento_wire_types/v4/auth_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `momento_wire_types-0.98.1/momento_wire_types/v4/cacheclient_pb2.py` & `momento_wire_types-0.99.0/momento_wire_types/v4/cacheclient_pb2.py`

 * *Files identical despite different names*

### Comparing `momento_wire_types-0.98.1/momento_wire_types/v4/cacheclient_pb2.pyi` & `momento_wire_types-0.99.0/momento_wire_types/v4/cacheclient_pb2.pyi`

 * *Files identical despite different names*

### Comparing `momento_wire_types-0.98.1/momento_wire_types/v4/cacheclient_pb2_grpc.py` & `momento_wire_types-0.99.0/momento_wire_types/v4/cacheclient_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `momento_wire_types-0.98.1/momento_wire_types/v4/cachepubsub_pb2.py` & `momento_wire_types-0.99.0/momento_wire_types/v4/cachepubsub_pb2.py`

 * *Files identical despite different names*

### Comparing `momento_wire_types-0.98.1/momento_wire_types/v4/cachepubsub_pb2.pyi` & `momento_wire_types-0.99.0/momento_wire_types/v4/cachepubsub_pb2.pyi`

 * *Files identical despite different names*

### Comparing `momento_wire_types-0.98.1/momento_wire_types/v4/cachepubsub_pb2_grpc.py` & `momento_wire_types-0.99.0/momento_wire_types/v4/cachepubsub_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `momento_wire_types-0.98.1/momento_wire_types/v4/controlclient_pb2.py` & `momento_wire_types-0.99.0/momento_wire_types/v4/controlclient_pb2.py`

 * *Files identical despite different names*

### Comparing `momento_wire_types-0.98.1/momento_wire_types/v4/controlclient_pb2.pyi` & `momento_wire_types-0.99.0/momento_wire_types/v4/controlclient_pb2.pyi`

 * *Files identical despite different names*

### Comparing `momento_wire_types-0.98.1/momento_wire_types/v4/controlclient_pb2_grpc.py` & `momento_wire_types-0.99.0/momento_wire_types/v4/controlclient_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `momento_wire_types-0.98.1/momento_wire_types/v4/extensions_pb2.py` & `momento_wire_types-0.99.0/momento_wire_types/v4/extensions_pb2.py`

 * *Files identical despite different names*

### Comparing `momento_wire_types-0.98.1/momento_wire_types/v4/permissionmessages_pb2.py` & `momento_wire_types-0.99.0/momento_wire_types/v4/permissionmessages_pb2.py`

 * *Files identical despite different names*

### Comparing `momento_wire_types-0.98.1/momento_wire_types/v4/permissionmessages_pb2.pyi` & `momento_wire_types-0.99.0/momento_wire_types/v4/permissionmessages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `momento_wire_types-0.98.1/momento_wire_types/v4/token_pb2.py` & `momento_wire_types-0.99.0/momento_wire_types/v4/token_pb2.py`

 * *Files identical despite different names*

### Comparing `momento_wire_types-0.98.1/momento_wire_types/v4/token_pb2.pyi` & `momento_wire_types-0.99.0/momento_wire_types/v4/token_pb2.pyi`

 * *Files identical despite different names*

### Comparing `momento_wire_types-0.98.1/momento_wire_types/v4/token_pb2_grpc.py` & `momento_wire_types-0.99.0/momento_wire_types/v4/token_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `momento_wire_types-0.98.1/momento_wire_types/v4/vectorindex_pb2.py` & `momento_wire_types-0.99.0/momento_wire_types/v4/vectorindex_pb2.py`

 * *Files identical despite different names*

### Comparing `momento_wire_types-0.98.1/momento_wire_types/v4/vectorindex_pb2.pyi` & `momento_wire_types-0.99.0/momento_wire_types/v4/vectorindex_pb2.pyi`

 * *Files identical despite different names*

### Comparing `momento_wire_types-0.98.1/momento_wire_types/v4/vectorindex_pb2_grpc.py` & `momento_wire_types-0.99.0/momento_wire_types/v4/vectorindex_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `momento_wire_types-0.98.1/pyproject.toml` & `momento_wire_types-0.99.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "momento-wire-types"
-version = "0.98.1"
+version = "0.99.0"
 description = "Momento Client Proto Generated Files"
 authors = ["Momento <hello@momentohq.com>"]
 
 license = "Apache-2.0"
 
 documentation = "https://docs.momentohq.com/"
 homepage = "https://gomomento.com"
```

### Comparing `momento_wire_types-0.98.1/PKG-INFO` & `momento_wire_types-0.99.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: momento-wire-types
-Version: 0.98.1
+Version: 0.99.0
 Summary: Momento Client Proto Generated Files
 Home-page: https://gomomento.com
 License: Apache-2.0
 Keywords: Momento,caching,key-value store,serverless
 Author: Momento
 Author-email: hello@momentohq.com
 Requires-Python: >=3.7,<4.0
```

