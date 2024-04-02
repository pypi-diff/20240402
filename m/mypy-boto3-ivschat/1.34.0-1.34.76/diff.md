# Comparing `tmp/mypy-boto3-ivschat-1.34.0.tar.gz` & `tmp/mypy-boto3-ivschat-1.34.76.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ivschat-1.34.0.tar", last modified: Wed Dec 13 21:22:58 2023, max compression
+gzip compressed data, was "mypy-boto3-ivschat-1.34.76.tar", last modified: Tue Apr  2 19:32:31 2024, max compression
```

## Comparing `mypy-boto3-ivschat-1.34.0.tar` & `mypy-boto3-ivschat-1.34.76.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:22:58.231252 mypy-boto3-ivschat-1.34.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 21:12:19.000000 mypy-boto3-ivschat-1.34.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12088 2023-12-13 21:22:58.231252 mypy-boto3-ivschat-1.34.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10555 2023-12-13 21:12:19.000000 mypy-boto3-ivschat-1.34.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:22:58.231252 mypy-boto3-ivschat-1.34.0/mypy_boto3_ivschat/
--rw-r--r--   0 runner    (1001) docker     (127)      374 2023-12-13 21:12:19.000000 mypy-boto3-ivschat-1.34.0/mypy_boto3_ivschat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2023-12-13 21:12:19.000000 mypy-boto3-ivschat-1.34.0/mypy_boto3_ivschat/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      905 2023-12-13 21:12:19.000000 mypy-boto3-ivschat-1.34.0/mypy_boto3_ivschat/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13498 2023-12-13 21:12:19.000000 mypy-boto3-ivschat-1.34.0/mypy_boto3_ivschat/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    13495 2023-12-13 21:12:19.000000 mypy-boto3-ivschat-1.34.0/mypy_boto3_ivschat/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8828 2023-12-13 21:12:19.000000 mypy-boto3-ivschat-1.34.0/mypy_boto3_ivschat/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8826 2023-12-13 21:12:19.000000 mypy-boto3-ivschat-1.34.0/mypy_boto3_ivschat/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 21:12:19.000000 mypy-boto3-ivschat-1.34.0/mypy_boto3_ivschat/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    12646 2023-12-13 21:12:19.000000 mypy-boto3-ivschat-1.34.0/mypy_boto3_ivschat/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    12645 2023-12-13 21:12:19.000000 mypy-boto3-ivschat-1.34.0/mypy_boto3_ivschat/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-13 21:12:19.000000 mypy-boto3-ivschat-1.34.0/mypy_boto3_ivschat/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:22:58.231252 mypy-boto3-ivschat-1.34.0/mypy_boto3_ivschat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12088 2023-12-13 21:22:58.000000 mypy-boto3-ivschat-1.34.0/mypy_boto3_ivschat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      615 2023-12-13 21:22:58.000000 mypy-boto3-ivschat-1.34.0/mypy_boto3_ivschat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:22:58.000000 mypy-boto3-ivschat-1.34.0/mypy_boto3_ivschat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:22:58.000000 mypy-boto3-ivschat-1.34.0/mypy_boto3_ivschat.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 21:22:58.000000 mypy-boto3-ivschat-1.34.0/mypy_boto3_ivschat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-12-13 21:22:58.000000 mypy-boto3-ivschat-1.34.0/mypy_boto3_ivschat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 21:22:58.231252 mypy-boto3-ivschat-1.34.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2023-12-13 21:12:19.000000 mypy-boto3-ivschat-1.34.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:32:31.855228 mypy-boto3-ivschat-1.34.76/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-02 19:32:02.000000 mypy-boto3-ivschat-1.34.76/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-04-02 19:32:31.851228 mypy-boto3-ivschat-1.34.76/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10556 2024-04-02 19:32:02.000000 mypy-boto3-ivschat-1.34.76/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:32:31.851228 mypy-boto3-ivschat-1.34.76/mypy_boto3_ivschat/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-02 19:32:02.000000 mypy-boto3-ivschat-1.34.76/mypy_boto3_ivschat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-02 19:32:02.000000 mypy-boto3-ivschat-1.34.76/mypy_boto3_ivschat/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-02 19:32:02.000000 mypy-boto3-ivschat-1.34.76/mypy_boto3_ivschat/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13504 2024-04-02 19:32:02.000000 mypy-boto3-ivschat-1.34.76/mypy_boto3_ivschat/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13501 2024-04-02 19:32:02.000000 mypy-boto3-ivschat-1.34.76/mypy_boto3_ivschat/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8963 2024-04-02 19:32:03.000000 mypy-boto3-ivschat-1.34.76/mypy_boto3_ivschat/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8963 2024-04-02 19:32:03.000000 mypy-boto3-ivschat-1.34.76/mypy_boto3_ivschat/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:32:02.000000 mypy-boto3-ivschat-1.34.76/mypy_boto3_ivschat/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    12658 2024-04-02 19:32:03.000000 mypy-boto3-ivschat-1.34.76/mypy_boto3_ivschat/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12658 2024-04-02 19:32:03.000000 mypy-boto3-ivschat-1.34.76/mypy_boto3_ivschat/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-02 19:32:02.000000 mypy-boto3-ivschat-1.34.76/mypy_boto3_ivschat/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:32:31.851228 mypy-boto3-ivschat-1.34.76/mypy_boto3_ivschat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-04-02 19:32:31.000000 mypy-boto3-ivschat-1.34.76/mypy_boto3_ivschat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-02 19:32:31.000000 mypy-boto3-ivschat-1.34.76/mypy_boto3_ivschat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 19:32:31.000000 mypy-boto3-ivschat-1.34.76/mypy_boto3_ivschat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 19:32:31.000000 mypy-boto3-ivschat-1.34.76/mypy_boto3_ivschat.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-02 19:32:31.000000 mypy-boto3-ivschat-1.34.76/mypy_boto3_ivschat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-02 19:32:31.000000 mypy-boto3-ivschat-1.34.76/mypy_boto3_ivschat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 19:32:31.855228 mypy-boto3-ivschat-1.34.76/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-04-02 19:32:02.000000 mypy-boto3-ivschat-1.34.76/setup.py
```

### Comparing `mypy-boto3-ivschat-1.34.0/LICENSE` & `mypy-boto3-ivschat-1.34.76/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Vlad Emelianov
+Copyright (c) 2024 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-ivschat-1.34.0/PKG-INFO` & `mypy-boto3-ivschat-1.34.76/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ivschat
-Version: 1.34.0
-Summary: Type annotations for boto3.ivschat 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.76
+Summary: Type annotations for boto3.ivschat 1.34.76 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivschat/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -13,50 +13,50 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
 
 <a id="mypy-boto3-ivschat"></a>
 
 # mypy-boto3-ivschat
 
 [![PyPI - mypy-boto3-ivschat](https://img.shields.io/pypi/v/mypy-boto3-ivschat.svg?color=blue)](https://pypi.org/project/mypy-boto3-ivschat)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ivschat.svg?color=blue)](https://pypi.org/project/mypy-boto3-ivschat)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivschat/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ivschat)](https://pepy.tech/project/mypy-boto3-ivschat)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ivschat 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#ivschat)
+[boto3.ivschat 1.34.76](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#ivschat)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-ivschat docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivschat/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-ivschat-1.34.0/README.md` & `mypy-boto3-ivschat-1.34.76/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ivschat.svg?color=blue)](https://pypi.org/project/mypy-boto3-ivschat)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivschat/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ivschat)](https://pepy.tech/project/mypy-boto3-ivschat)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ivschat 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#ivschat)
+[boto3.ivschat 1.34.76](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#ivschat)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-ivschat docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivschat/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-ivschat-1.34.0/mypy_boto3_ivschat/__main__.py` & `mypy-boto3-ivschat-1.34.76/mypy_boto3_ivschat/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,28 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ivschat 1.34.0\nVersion:         1.34.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
-        " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivschat//\nBoto3 docs:     "
-        " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#ivschat\nOther"
-        " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
-        " https://github.com/youtype/mypy_boto3_builder/releases"
+        "Type annotations for boto3.ivschat 1.34.76\n"
+        "Version:         1.34.76\n"
+        "Builder version: 7.23.2\n"
+        "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivschat//\n"
+        "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#ivschat\n"
+        "Other services:  https://pypi.org/project/boto3-stubs/\n"
+        "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.0")
+    print("1.34.76")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-ivschat-1.34.0/mypy_boto3_ivschat/client.py` & `mypy-boto3-ivschat-1.34.76/mypy_boto3_ivschat/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -35,35 +35,32 @@
     SendEventResponseTypeDef,
     UpdateLoggingConfigurationResponseTypeDef,
     UpdateRoomResponseTypeDef,
 )
 
 __all__ = ("ivschatClient",)
 
-
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     PendingVerification: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
-
 class ivschatClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#ivschat.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivschat/client/)
     """
 
     meta: ClientMeta
@@ -96,15 +93,15 @@
     def create_chat_token(
         self,
         *,
         roomIdentifier: str,
         userId: str,
         attributes: Mapping[str, str] = ...,
         capabilities: Sequence[ChatTokenCapabilityType] = ...,
-        sessionDurationInMinutes: int = ...
+        sessionDurationInMinutes: int = ...,
     ) -> CreateChatTokenResponseTypeDef:
         """
         Creates an encrypted token that is used by a chat participant to establish an
         individual WebSocket chat connection to a
         room.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#ivschat.Client.create_chat_token)
@@ -112,15 +109,15 @@
         """
 
     def create_logging_configuration(
         self,
         *,
         destinationConfiguration: DestinationConfigurationTypeDef,
         name: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateLoggingConfigurationResponseTypeDef:
         """
         Creates a logging configuration that allows clients to store and record sent
         messages.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#ivschat.Client.create_logging_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivschat/client/#create_logging_configuration)
@@ -130,15 +127,15 @@
         self,
         *,
         loggingConfigurationIdentifiers: Sequence[str] = ...,
         maximumMessageLength: int = ...,
         maximumMessageRatePerSecond: int = ...,
         messageReviewHandler: MessageReviewHandlerTypeDef = ...,
         name: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateRoomResponseTypeDef:
         """
         Creates a room that allows clients to connect and pass messages.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#ivschat.Client.create_room)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivschat/client/#create_room)
         """
@@ -228,15 +225,15 @@
     def list_rooms(
         self,
         *,
         loggingConfigurationIdentifier: str = ...,
         maxResults: int = ...,
         messageReviewHandlerUri: str = ...,
         name: str = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListRoomsResponseTypeDef:
         """
         Gets summary information about all your rooms in the AWS region where the API
         request is
         processed.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#ivschat.Client.list_rooms)
@@ -278,15 +275,15 @@
         """
 
     def update_logging_configuration(
         self,
         *,
         identifier: str,
         destinationConfiguration: DestinationConfigurationTypeDef = ...,
-        name: str = ...
+        name: str = ...,
     ) -> UpdateLoggingConfigurationResponseTypeDef:
         """
         Updates a specified logging configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#ivschat.Client.update_logging_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivschat/client/#update_logging_configuration)
         """
@@ -295,15 +292,15 @@
         self,
         *,
         identifier: str,
         loggingConfigurationIdentifiers: Sequence[str] = ...,
         maximumMessageLength: int = ...,
         maximumMessageRatePerSecond: int = ...,
         messageReviewHandler: MessageReviewHandlerTypeDef = ...,
-        name: str = ...
+        name: str = ...,
     ) -> UpdateRoomResponseTypeDef:
         """
         Updates a room’s configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#ivschat.Client.update_room)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivschat/client/#update_room)
         """
```

### Comparing `mypy-boto3-ivschat-1.34.0/mypy_boto3_ivschat/client.pyi` & `mypy-boto3-ivschat-1.34.76/mypy_boto3_ivschat/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,32 +35,35 @@
     SendEventResponseTypeDef,
     UpdateLoggingConfigurationResponseTypeDef,
     UpdateRoomResponseTypeDef,
 )
 
 __all__ = ("ivschatClient",)
 
+
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     PendingVerification: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
+
 class ivschatClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#ivschat.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivschat/client/)
     """
 
     meta: ClientMeta
@@ -93,15 +96,15 @@
     def create_chat_token(
         self,
         *,
         roomIdentifier: str,
         userId: str,
         attributes: Mapping[str, str] = ...,
         capabilities: Sequence[ChatTokenCapabilityType] = ...,
-        sessionDurationInMinutes: int = ...
+        sessionDurationInMinutes: int = ...,
     ) -> CreateChatTokenResponseTypeDef:
         """
         Creates an encrypted token that is used by a chat participant to establish an
         individual WebSocket chat connection to a
         room.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#ivschat.Client.create_chat_token)
@@ -109,15 +112,15 @@
         """
 
     def create_logging_configuration(
         self,
         *,
         destinationConfiguration: DestinationConfigurationTypeDef,
         name: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateLoggingConfigurationResponseTypeDef:
         """
         Creates a logging configuration that allows clients to store and record sent
         messages.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#ivschat.Client.create_logging_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivschat/client/#create_logging_configuration)
@@ -127,15 +130,15 @@
         self,
         *,
         loggingConfigurationIdentifiers: Sequence[str] = ...,
         maximumMessageLength: int = ...,
         maximumMessageRatePerSecond: int = ...,
         messageReviewHandler: MessageReviewHandlerTypeDef = ...,
         name: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateRoomResponseTypeDef:
         """
         Creates a room that allows clients to connect and pass messages.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#ivschat.Client.create_room)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivschat/client/#create_room)
         """
@@ -225,15 +228,15 @@
     def list_rooms(
         self,
         *,
         loggingConfigurationIdentifier: str = ...,
         maxResults: int = ...,
         messageReviewHandlerUri: str = ...,
         name: str = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListRoomsResponseTypeDef:
         """
         Gets summary information about all your rooms in the AWS region where the API
         request is
         processed.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#ivschat.Client.list_rooms)
@@ -275,15 +278,15 @@
         """
 
     def update_logging_configuration(
         self,
         *,
         identifier: str,
         destinationConfiguration: DestinationConfigurationTypeDef = ...,
-        name: str = ...
+        name: str = ...,
     ) -> UpdateLoggingConfigurationResponseTypeDef:
         """
         Updates a specified logging configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#ivschat.Client.update_logging_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivschat/client/#update_logging_configuration)
         """
@@ -292,15 +295,15 @@
         self,
         *,
         identifier: str,
         loggingConfigurationIdentifiers: Sequence[str] = ...,
         maximumMessageLength: int = ...,
         maximumMessageRatePerSecond: int = ...,
         messageReviewHandler: MessageReviewHandlerTypeDef = ...,
-        name: str = ...
+        name: str = ...,
     ) -> UpdateRoomResponseTypeDef:
         """
         Updates a room’s configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#ivschat.Client.update_room)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivschat/client/#update_room)
         """
```

### Comparing `mypy-boto3-ivschat-1.34.0/mypy_boto3_ivschat/literals.py` & `mypy-boto3-ivschat-1.34.76/mypy_boto3_ivschat/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,28 +15,26 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ChatTokenCapabilityType",
     "CreateLoggingConfigurationStateType",
     "FallbackResultType",
     "LoggingConfigurationStateType",
     "UpdateLoggingConfigurationStateType",
     "ivschatServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 ChatTokenCapabilityType = Literal["DELETE_MESSAGE", "DISCONNECT_USER", "SEND_MESSAGE"]
 CreateLoggingConfigurationStateType = Literal["ACTIVE"]
 FallbackResultType = Literal["ALLOW", "DENY"]
 LoggingConfigurationStateType = Literal[
     "ACTIVE", "CREATE_FAILED", "CREATING", "DELETE_FAILED", "DELETING", "UPDATE_FAILED", "UPDATING"
 ]
 UpdateLoggingConfigurationStateType = Literal["ACTIVE"]
@@ -63,14 +61,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -81,14 +80,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -106,14 +106,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -136,14 +137,15 @@
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -204,15 +206,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -284,17 +285,19 @@
     "migrationhuborchestrator",
     "migrationhubstrategy",
     "mobile",
     "mq",
     "mturk",
     "mwaa",
     "neptune",
+    "neptune-graph",
     "neptunedata",
     "network-firewall",
     "networkmanager",
+    "networkmonitor",
     "nimble",
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
@@ -384,19 +387,21 @@
     "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
+    "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy-boto3-ivschat-1.34.0/mypy_boto3_ivschat/literals.pyi` & `mypy-boto3-ivschat-1.34.76/mypy_boto3_ivschat/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -79,14 +80,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -104,14 +106,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -134,14 +137,15 @@
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -202,15 +206,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -282,17 +285,19 @@
     "migrationhuborchestrator",
     "migrationhubstrategy",
     "mobile",
     "mq",
     "mturk",
     "mwaa",
     "neptune",
+    "neptune-graph",
     "neptunedata",
     "network-firewall",
     "networkmanager",
+    "networkmonitor",
     "nimble",
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
@@ -382,19 +387,21 @@
     "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
+    "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy-boto3-ivschat-1.34.0/mypy_boto3_ivschat/type_defs.py` & `mypy-boto3-ivschat-1.34.76/mypy_boto3_ivschat/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "CloudWatchLogsDestinationConfigurationTypeDef",
     "CreateChatTokenRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "MessageReviewHandlerTypeDef",
     "DeleteLoggingConfigurationRequestRequestTypeDef",
     "DeleteMessageRequestRequestTypeDef",
@@ -89,18 +88,18 @@
         "sessionDurationInMinutes": NotRequired[int],
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 MessageReviewHandlerTypeDef = TypedDict(
     "MessageReviewHandlerTypeDef",
     {
         "fallbackResult": NotRequired[FallbackResultType],
         "uri": NotRequired[str],
```

### Comparing `mypy-boto3-ivschat-1.34.0/mypy_boto3_ivschat/type_defs.pyi` & `mypy-boto3-ivschat-1.34.76/mypy_boto3_ivschat/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -88,18 +88,18 @@
         "sessionDurationInMinutes": NotRequired[int],
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 MessageReviewHandlerTypeDef = TypedDict(
     "MessageReviewHandlerTypeDef",
     {
         "fallbackResult": NotRequired[FallbackResultType],
         "uri": NotRequired[str],
```

### Comparing `mypy-boto3-ivschat-1.34.0/mypy_boto3_ivschat.egg-info/PKG-INFO` & `mypy-boto3-ivschat-1.34.76/mypy_boto3_ivschat.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ivschat
-Version: 1.34.0
-Summary: Type annotations for boto3.ivschat 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.76
+Summary: Type annotations for boto3.ivschat 1.34.76 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivschat/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -13,50 +13,50 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
 
 <a id="mypy-boto3-ivschat"></a>
 
 # mypy-boto3-ivschat
 
 [![PyPI - mypy-boto3-ivschat](https://img.shields.io/pypi/v/mypy-boto3-ivschat.svg?color=blue)](https://pypi.org/project/mypy-boto3-ivschat)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ivschat.svg?color=blue)](https://pypi.org/project/mypy-boto3-ivschat)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivschat/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ivschat)](https://pepy.tech/project/mypy-boto3-ivschat)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ivschat 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#ivschat)
+[boto3.ivschat 1.34.76](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#ivschat)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-ivschat docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivschat/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-ivschat-1.34.0/mypy_boto3_ivschat.egg-info/SOURCES.txt` & `mypy-boto3-ivschat-1.34.76/mypy_boto3_ivschat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivschat-1.34.0/setup.py` & `mypy-boto3-ivschat-1.34.76/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,47 +7,44 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ivschat",
-    version="1.34.0",
+    version="1.34.76",
     packages=["mypy_boto3_ivschat"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description=(
-        "Type annotations for boto3.ivschat 1.34.0 service generated with mypy-boto3-builder 7.21.0"
-    ),
+    description="Type annotations for boto3.ivschat 1.34.76 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3.13",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
-        "Typing :: Typed",
+        "Typing :: Stubs Only",
     ],
     keywords="boto3 ivschat type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_ivschat": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivschat/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

