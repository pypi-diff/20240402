# Comparing `tmp/mypy-boto3-glue-1.34.7.tar.gz` & `tmp/mypy-boto3-glue-1.34.76.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-glue-1.34.7.tar", last modified: Fri Dec 22 20:32:30 2023, max compression
+gzip compressed data, was "mypy-boto3-glue-1.34.76.tar", last modified: Tue Apr  2 19:32:31 2024, max compression
```

## Comparing `mypy-boto3-glue-1.34.7.tar` & `mypy-boto3-glue-1.34.76.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 20:32:30.236724 mypy-boto3-glue-1.34.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-22 20:32:02.000000 mypy-boto3-glue-1.34.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14753 2023-12-22 20:32:30.236724 mypy-boto3-glue-1.34.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13277 2023-12-22 20:32:02.000000 mypy-boto3-glue-1.34.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 20:32:30.232724 mypy-boto3-glue-1.34.7/mypy_boto3_glue/
--rw-r--r--   0 runner    (1001) docker     (127)     4090 2023-12-22 20:32:02.000000 mypy-boto3-glue-1.34.7/mypy_boto3_glue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4090 2023-12-22 20:32:02.000000 mypy-boto3-glue-1.34.7/mypy_boto3_glue/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      893 2023-12-22 20:32:02.000000 mypy-boto3-glue-1.34.7/mypy_boto3_glue/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)   145115 2023-12-22 20:32:04.000000 mypy-boto3-glue-1.34.7/mypy_boto3_glue/client.py
--rw-r--r--   0 runner    (1001) docker     (127)   145112 2023-12-22 20:32:03.000000 mypy-boto3-glue-1.34.7/mypy_boto3_glue/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    22394 2023-12-22 20:32:04.000000 mypy-boto3-glue-1.34.7/mypy_boto3_glue/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    22394 2023-12-22 20:32:04.000000 mypy-boto3-glue-1.34.7/mypy_boto3_glue/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    21346 2023-12-22 20:32:04.000000 mypy-boto3-glue-1.34.7/mypy_boto3_glue/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    21326 2023-12-22 20:32:04.000000 mypy-boto3-glue-1.34.7/mypy_boto3_glue/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 20:32:02.000000 mypy-boto3-glue-1.34.7/mypy_boto3_glue/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   237224 2023-12-22 20:32:09.000000 mypy-boto3-glue-1.34.7/mypy_boto3_glue/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)   237224 2023-12-22 20:32:07.000000 mypy-boto3-glue-1.34.7/mypy_boto3_glue/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-22 20:32:02.000000 mypy-boto3-glue-1.34.7/mypy_boto3_glue/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 20:32:30.236724 mypy-boto3-glue-1.34.7/mypy_boto3_glue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14753 2023-12-22 20:32:30.000000 mypy-boto3-glue-1.34.7/mypy_boto3_glue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      623 2023-12-22 20:32:30.000000 mypy-boto3-glue-1.34.7/mypy_boto3_glue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-22 20:32:30.000000 mypy-boto3-glue-1.34.7/mypy_boto3_glue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-22 20:32:30.000000 mypy-boto3-glue-1.34.7/mypy_boto3_glue.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-22 20:32:30.000000 mypy-boto3-glue-1.34.7/mypy_boto3_glue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-12-22 20:32:30.000000 mypy-boto3-glue-1.34.7/mypy_boto3_glue.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-22 20:32:30.236724 mypy-boto3-glue-1.34.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1967 2023-12-22 20:32:02.000000 mypy-boto3-glue-1.34.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:32:31.483228 mypy-boto3-glue-1.34.76/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-02 19:31:55.000000 mypy-boto3-glue-1.34.76/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14821 2024-04-02 19:32:31.483228 mypy-boto3-glue-1.34.76/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13278 2024-04-02 19:31:55.000000 mypy-boto3-glue-1.34.76/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:32:31.479228 mypy-boto3-glue-1.34.76/mypy_boto3_glue/
+-rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-04-02 19:31:55.000000 mypy-boto3-glue-1.34.76/mypy_boto3_glue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-04-02 19:31:55.000000 mypy-boto3-glue-1.34.76/mypy_boto3_glue/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-02 19:31:55.000000 mypy-boto3-glue-1.34.76/mypy_boto3_glue/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   145115 2024-04-02 19:31:57.000000 mypy-boto3-glue-1.34.76/mypy_boto3_glue/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)   145112 2024-04-02 19:31:56.000000 mypy-boto3-glue-1.34.76/mypy_boto3_glue/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    22643 2024-04-02 19:31:57.000000 mypy-boto3-glue-1.34.76/mypy_boto3_glue/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22643 2024-04-02 19:31:57.000000 mypy-boto3-glue-1.34.76/mypy_boto3_glue/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    21346 2024-04-02 19:31:57.000000 mypy-boto3-glue-1.34.76/mypy_boto3_glue/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21326 2024-04-02 19:31:57.000000 mypy-boto3-glue-1.34.76/mypy_boto3_glue/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:31:55.000000 mypy-boto3-glue-1.34.76/mypy_boto3_glue/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   238231 2024-04-02 19:32:02.000000 mypy-boto3-glue-1.34.76/mypy_boto3_glue/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   238231 2024-04-02 19:32:00.000000 mypy-boto3-glue-1.34.76/mypy_boto3_glue/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-02 19:31:55.000000 mypy-boto3-glue-1.34.76/mypy_boto3_glue/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:32:31.483228 mypy-boto3-glue-1.34.76/mypy_boto3_glue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14821 2024-04-02 19:32:31.000000 mypy-boto3-glue-1.34.76/mypy_boto3_glue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-02 19:32:31.000000 mypy-boto3-glue-1.34.76/mypy_boto3_glue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 19:32:31.000000 mypy-boto3-glue-1.34.76/mypy_boto3_glue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 19:32:31.000000 mypy-boto3-glue-1.34.76/mypy_boto3_glue.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-02 19:32:31.000000 mypy-boto3-glue-1.34.76/mypy_boto3_glue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-02 19:32:31.000000 mypy-boto3-glue-1.34.76/mypy_boto3_glue.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 19:32:31.483228 mypy-boto3-glue-1.34.76/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-02 19:31:55.000000 mypy-boto3-glue-1.34.76/setup.py
```

### Comparing `mypy-boto3-glue-1.34.7/LICENSE` & `mypy-boto3-glue-1.34.76/LICENSE`

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

### Comparing `mypy-boto3-glue-1.34.7/PKG-INFO` & `mypy-boto3-glue-1.34.76/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-glue
-Version: 1.34.7
-Summary: Type annotations for boto3.Glue 1.34.7 service generated with mypy-boto3-builder 7.23.0
+Version: 1.34.76
+Summary: Type annotations for boto3.Glue 1.34.76 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -25,37 +25,38 @@
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Stubs Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
 
 <a id="mypy-boto3-glue"></a>
 
 # mypy-boto3-glue
 
 [![PyPI - mypy-boto3-glue](https://img.shields.io/pypi/v/mypy-boto3-glue.svg?color=blue)](https://pypi.org/project/mypy-boto3-glue)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-glue.svg?color=blue)](https://pypi.org/project/mypy-boto3-glue)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-glue)](https://pepy.tech/project/mypy-boto3-glue)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Glue 1.34.7](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue)
+[boto3.Glue 1.34.76](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-glue docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-glue-1.34.7/README.md` & `mypy-boto3-glue-1.34.76/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-glue.svg?color=blue)](https://pypi.org/project/mypy-boto3-glue)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-glue)](https://pepy.tech/project/mypy-boto3-glue)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Glue 1.34.7](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue)
+[boto3.Glue 1.34.76](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-glue docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-glue-1.34.7/mypy_boto3_glue/__init__.py` & `mypy-boto3-glue-1.34.76/mypy_boto3_glue/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glue-1.34.7/mypy_boto3_glue/__init__.pyi` & `mypy-boto3-glue-1.34.76/mypy_boto3_glue/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glue-1.34.7/mypy_boto3_glue/__main__.py` & `mypy-boto3-glue-1.34.76/mypy_boto3_glue/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,28 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Glue 1.34.7\nVersion:         1.34.7\nBuilder version:"
-        " 7.23.0\nDocs:           "
-        " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue//\nBoto3 docs:     "
-        " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue\nOther"
-        " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
-        " https://github.com/youtype/mypy_boto3_builder/releases"
+        "Type annotations for boto3.Glue 1.34.76\n"
+        "Version:         1.34.76\n"
+        "Builder version: 7.23.2\n"
+        "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue//\n"
+        "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue\n"
+        "Other services:  https://pypi.org/project/boto3-stubs/\n"
+        "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.7")
+    print("1.34.76")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-glue-1.34.7/mypy_boto3_glue/client.py` & `mypy-boto3-glue-1.34.76/mypy_boto3_glue/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glue-1.34.7/mypy_boto3_glue/client.pyi` & `mypy-boto3-glue-1.34.76/mypy_boto3_glue/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glue-1.34.7/mypy_boto3_glue/literals.py` & `mypy-boto3-glue-1.34.76/mypy_boto3_glue/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,15 +160,15 @@
     "INTERNAL_ERROR",
     "INVALID_PARTITION_TYPE_DATA_ERROR",
     "MISSING_PARTITION_VALUE_ERROR",
     "UNSUPPORTED_PARTITION_CHARACTER_ERROR",
 ]
 BlueprintRunStateType = Literal["FAILED", "ROLLING_BACK", "RUNNING", "SUCCEEDED"]
 BlueprintStatusType = Literal["ACTIVE", "CREATING", "FAILED", "UPDATING"]
-CatalogEncryptionModeType = Literal["DISABLED", "SSE-KMS"]
+CatalogEncryptionModeType = Literal["DISABLED", "SSE-KMS", "SSE-KMS-WITH-SERVICE-ROLE"]
 CloudWatchEncryptionModeType = Literal["DISABLED", "SSE-KMS"]
 ColumnStatisticsStateType = Literal["FAILED", "RUNNING", "STARTING", "STOPPED", "SUCCEEDED"]
 ColumnStatisticsTypeType = Literal[
     "BINARY", "BOOLEAN", "DATE", "DECIMAL", "DOUBLE", "LONG", "STRING"
 ]
 ComparatorType = Literal[
     "EQUALS", "GREATER_THAN", "GREATER_THAN_EQUALS", "LESS_THAN", "LESS_THAN_EQUALS"
@@ -183,14 +183,15 @@
     "CONNECTOR_CLASS_NAME",
     "CONNECTOR_TYPE",
     "CONNECTOR_URL",
     "CUSTOM_JDBC_CERT",
     "CUSTOM_JDBC_CERT_STRING",
     "ENCRYPTED_KAFKA_CLIENT_KEYSTORE_PASSWORD",
     "ENCRYPTED_KAFKA_CLIENT_KEY_PASSWORD",
+    "ENCRYPTED_KAFKA_SASL_PLAIN_PASSWORD",
     "ENCRYPTED_KAFKA_SASL_SCRAM_PASSWORD",
     "ENCRYPTED_PASSWORD",
     "HOST",
     "INSTANCE_ID",
     "JDBC_CONNECTION_URL",
     "JDBC_DRIVER_CLASS_NAME",
     "JDBC_DRIVER_JAR_URI",
@@ -203,14 +204,16 @@
     "KAFKA_CLIENT_KEY_PASSWORD",
     "KAFKA_CUSTOM_CERT",
     "KAFKA_SASL_GSSAPI_KEYTAB",
     "KAFKA_SASL_GSSAPI_KRB5_CONF",
     "KAFKA_SASL_GSSAPI_PRINCIPAL",
     "KAFKA_SASL_GSSAPI_SERVICE",
     "KAFKA_SASL_MECHANISM",
+    "KAFKA_SASL_PLAIN_PASSWORD",
+    "KAFKA_SASL_PLAIN_USERNAME",
     "KAFKA_SASL_SCRAM_PASSWORD",
     "KAFKA_SASL_SCRAM_SECRETS_ARN",
     "KAFKA_SASL_SCRAM_USERNAME",
     "KAFKA_SKIP_CUSTOM_CERT_VALIDATION",
     "KAFKA_SSL_ENABLED",
     "PASSWORD",
     "PORT",
@@ -417,14 +420,15 @@
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
@@ -435,14 +439,15 @@
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
@@ -460,14 +465,15 @@
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
@@ -490,14 +496,15 @@
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
@@ -558,15 +565,14 @@
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
@@ -740,19 +746,21 @@
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
@@ -815,14 +823,15 @@
     "ap-south-1",
     "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
     "ap-southeast-4",
     "ca-central-1",
+    "ca-west-1",
     "eu-central-1",
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
```

### Comparing `mypy-boto3-glue-1.34.7/mypy_boto3_glue/literals.pyi` & `mypy-boto3-glue-1.34.76/mypy_boto3_glue/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -160,15 +160,15 @@
     "INTERNAL_ERROR",
     "INVALID_PARTITION_TYPE_DATA_ERROR",
     "MISSING_PARTITION_VALUE_ERROR",
     "UNSUPPORTED_PARTITION_CHARACTER_ERROR",
 ]
 BlueprintRunStateType = Literal["FAILED", "ROLLING_BACK", "RUNNING", "SUCCEEDED"]
 BlueprintStatusType = Literal["ACTIVE", "CREATING", "FAILED", "UPDATING"]
-CatalogEncryptionModeType = Literal["DISABLED", "SSE-KMS"]
+CatalogEncryptionModeType = Literal["DISABLED", "SSE-KMS", "SSE-KMS-WITH-SERVICE-ROLE"]
 CloudWatchEncryptionModeType = Literal["DISABLED", "SSE-KMS"]
 ColumnStatisticsStateType = Literal["FAILED", "RUNNING", "STARTING", "STOPPED", "SUCCEEDED"]
 ColumnStatisticsTypeType = Literal[
     "BINARY", "BOOLEAN", "DATE", "DECIMAL", "DOUBLE", "LONG", "STRING"
 ]
 ComparatorType = Literal[
     "EQUALS", "GREATER_THAN", "GREATER_THAN_EQUALS", "LESS_THAN", "LESS_THAN_EQUALS"
@@ -183,14 +183,15 @@
     "CONNECTOR_CLASS_NAME",
     "CONNECTOR_TYPE",
     "CONNECTOR_URL",
     "CUSTOM_JDBC_CERT",
     "CUSTOM_JDBC_CERT_STRING",
     "ENCRYPTED_KAFKA_CLIENT_KEYSTORE_PASSWORD",
     "ENCRYPTED_KAFKA_CLIENT_KEY_PASSWORD",
+    "ENCRYPTED_KAFKA_SASL_PLAIN_PASSWORD",
     "ENCRYPTED_KAFKA_SASL_SCRAM_PASSWORD",
     "ENCRYPTED_PASSWORD",
     "HOST",
     "INSTANCE_ID",
     "JDBC_CONNECTION_URL",
     "JDBC_DRIVER_CLASS_NAME",
     "JDBC_DRIVER_JAR_URI",
@@ -203,14 +204,16 @@
     "KAFKA_CLIENT_KEY_PASSWORD",
     "KAFKA_CUSTOM_CERT",
     "KAFKA_SASL_GSSAPI_KEYTAB",
     "KAFKA_SASL_GSSAPI_KRB5_CONF",
     "KAFKA_SASL_GSSAPI_PRINCIPAL",
     "KAFKA_SASL_GSSAPI_SERVICE",
     "KAFKA_SASL_MECHANISM",
+    "KAFKA_SASL_PLAIN_PASSWORD",
+    "KAFKA_SASL_PLAIN_USERNAME",
     "KAFKA_SASL_SCRAM_PASSWORD",
     "KAFKA_SASL_SCRAM_SECRETS_ARN",
     "KAFKA_SASL_SCRAM_USERNAME",
     "KAFKA_SKIP_CUSTOM_CERT_VALIDATION",
     "KAFKA_SSL_ENABLED",
     "PASSWORD",
     "PORT",
@@ -417,14 +420,15 @@
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
@@ -435,14 +439,15 @@
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
@@ -460,14 +465,15 @@
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
@@ -490,14 +496,15 @@
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
@@ -558,15 +565,14 @@
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
@@ -740,19 +746,21 @@
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
@@ -815,14 +823,15 @@
     "ap-south-1",
     "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
     "ap-southeast-4",
     "ca-central-1",
+    "ca-west-1",
     "eu-central-1",
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
```

### Comparing `mypy-boto3-glue-1.34.7/mypy_boto3_glue/paginator.py` & `mypy-boto3-glue-1.34.76/mypy_boto3_glue/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glue-1.34.7/mypy_boto3_glue/paginator.pyi` & `mypy-boto3-glue-1.34.76/mypy_boto3_glue/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glue-1.34.7/mypy_boto3_glue/type_defs.py` & `mypy-boto3-glue-1.34.76/mypy_boto3_glue/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -433,14 +433,15 @@
     "UpdateJsonClassifierRequestTypeDef",
     "UpdateXMLClassifierRequestTypeDef",
     "UpdateCrawlerScheduleRequestRequestTypeDef",
     "UpdateDataQualityRulesetRequestRequestTypeDef",
     "UpdateJobFromSourceControlRequestRequestTypeDef",
     "UpdateSourceControlFromJobRequestRequestTypeDef",
     "UpdateWorkflowRequestRequestTypeDef",
+    "ViewRepresentationTypeDef",
     "WorkflowRunStatisticsTypeDef",
     "ActionTypeDef",
     "StartJobRunRequestRequestTypeDef",
     "AggregateTypeDef",
     "AmazonRedshiftNodeDataTypeDef",
     "SnowflakeNodeDataTypeDef",
     "BackfillErrorPaginatorTypeDef",
@@ -650,14 +651,15 @@
     "RedshiftTargetTypeDef",
     "UserDefinedFunctionInputTypeDef",
     "UserDefinedFunctionTypeDef",
     "TableOptimizerRunTypeDef",
     "SearchTablesRequestRequestTypeDef",
     "StatementOutputTypeDef",
     "UpdateClassifierRequestRequestTypeDef",
+    "ViewDefinitionTypeDef",
     "AmazonRedshiftSourceTypeDef",
     "AmazonRedshiftTargetTypeDef",
     "SnowflakeTargetTypeDef",
     "PartitionIndexDescriptorPaginatorTypeDef",
     "PartitionIndexDescriptorTypeDef",
     "BatchStopJobRunResponseTypeDef",
     "BatchUpdatePartitionResponseTypeDef",
@@ -913,18 +915,18 @@
         "Table": str,
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
 BatchDeleteConnectionRequestRequestTypeDef = TypedDict(
     "BatchDeleteConnectionRequestRequestTypeDef",
     {
         "ConnectionNameList": Sequence[str],
         "CatalogId": NotRequired[str],
@@ -2017,14 +2019,15 @@
     },
 )
 EncryptionAtRestTypeDef = TypedDict(
     "EncryptionAtRestTypeDef",
     {
         "CatalogEncryptionMode": CatalogEncryptionModeType,
         "SseAwsKmsKeyId": NotRequired[str],
+        "CatalogEncryptionServiceRole": NotRequired[str],
     },
 )
 DataLakePrincipalTypeDef = TypedDict(
     "DataLakePrincipalTypeDef",
     {
         "DataLakePrincipalIdentifier": NotRequired[str],
     },
@@ -3462,14 +3465,24 @@
     {
         "Name": str,
         "Description": NotRequired[str],
         "DefaultRunProperties": NotRequired[Mapping[str, str]],
         "MaxConcurrentRuns": NotRequired[int],
     },
 )
+ViewRepresentationTypeDef = TypedDict(
+    "ViewRepresentationTypeDef",
+    {
+        "Dialect": NotRequired[ViewDialectType],
+        "DialectVersion": NotRequired[str],
+        "ViewOriginalText": NotRequired[str],
+        "ViewExpandedText": NotRequired[str],
+        "IsStale": NotRequired[bool],
+    },
+)
 WorkflowRunStatisticsTypeDef = TypedDict(
     "WorkflowRunStatisticsTypeDef",
     {
         "TotalActions": NotRequired[int],
         "TimeoutActions": NotRequired[int],
         "FailedActions": NotRequired[int],
         "StoppedActions": NotRequired[int],
@@ -5475,14 +5488,23 @@
     {
         "GrokClassifier": NotRequired[UpdateGrokClassifierRequestTypeDef],
         "XMLClassifier": NotRequired[UpdateXMLClassifierRequestTypeDef],
         "JsonClassifier": NotRequired[UpdateJsonClassifierRequestTypeDef],
         "CsvClassifier": NotRequired[UpdateCsvClassifierRequestTypeDef],
     },
 )
+ViewDefinitionTypeDef = TypedDict(
+    "ViewDefinitionTypeDef",
+    {
+        "IsProtected": NotRequired[bool],
+        "Definer": NotRequired[str],
+        "SubObjects": NotRequired[List[str]],
+        "Representations": NotRequired[List[ViewRepresentationTypeDef]],
+    },
+)
 AmazonRedshiftSourceTypeDef = TypedDict(
     "AmazonRedshiftSourceTypeDef",
     {
         "Name": NotRequired[str],
         "Data": NotRequired[AmazonRedshiftNodeDataTypeDef],
     },
 )
@@ -6854,14 +6876,16 @@
         "Parameters": NotRequired[Dict[str, str]],
         "CreatedBy": NotRequired[str],
         "IsRegisteredWithLakeFormation": NotRequired[bool],
         "TargetTable": NotRequired[TableIdentifierTypeDef],
         "CatalogId": NotRequired[str],
         "VersionId": NotRequired[str],
         "FederatedTable": NotRequired[FederatedTableTypeDef],
+        "ViewDefinition": NotRequired[ViewDefinitionTypeDef],
+        "IsMultiDialectView": NotRequired[bool],
     },
 )
 PartitionInputTypeDef = TypedDict(
     "PartitionInputTypeDef",
     {
         "Values": NotRequired[Sequence[str]],
         "LastAccessTime": NotRequired[TimestampTypeDef],
@@ -6922,14 +6946,16 @@
         "Parameters": NotRequired[Dict[str, str]],
         "CreatedBy": NotRequired[str],
         "IsRegisteredWithLakeFormation": NotRequired[bool],
         "TargetTable": NotRequired[TableIdentifierTypeDef],
         "CatalogId": NotRequired[str],
         "VersionId": NotRequired[str],
         "FederatedTable": NotRequired[FederatedTableTypeDef],
+        "ViewDefinition": NotRequired[ViewDefinitionTypeDef],
+        "IsMultiDialectView": NotRequired[bool],
     },
 )
 GetSecurityConfigurationsResponsePaginatorTypeDef = TypedDict(
     "GetSecurityConfigurationsResponsePaginatorTypeDef",
     {
         "SecurityConfigurations": List[SecurityConfigurationPaginatorTypeDef],
         "NextToken": str,
@@ -7277,15 +7303,17 @@
     "GetUnfilteredTableMetadataResponseTypeDef",
     {
         "Table": TableTypeDef,
         "AuthorizedColumns": List[str],
         "IsRegisteredWithLakeFormation": bool,
         "CellFilters": List[ColumnRowFilterTypeDef],
         "QueryAuthorizationId": str,
+        "IsMultiDialectView": bool,
         "ResourceArn": str,
+        "IsProtected": bool,
         "Permissions": List[PermissionType],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 SearchTablesResponseTypeDef = TypedDict(
     "SearchTablesResponseTypeDef",
     {
```

### Comparing `mypy-boto3-glue-1.34.7/mypy_boto3_glue/type_defs.pyi` & `mypy-boto3-glue-1.34.76/mypy_boto3_glue/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -433,14 +433,15 @@
     "UpdateJsonClassifierRequestTypeDef",
     "UpdateXMLClassifierRequestTypeDef",
     "UpdateCrawlerScheduleRequestRequestTypeDef",
     "UpdateDataQualityRulesetRequestRequestTypeDef",
     "UpdateJobFromSourceControlRequestRequestTypeDef",
     "UpdateSourceControlFromJobRequestRequestTypeDef",
     "UpdateWorkflowRequestRequestTypeDef",
+    "ViewRepresentationTypeDef",
     "WorkflowRunStatisticsTypeDef",
     "ActionTypeDef",
     "StartJobRunRequestRequestTypeDef",
     "AggregateTypeDef",
     "AmazonRedshiftNodeDataTypeDef",
     "SnowflakeNodeDataTypeDef",
     "BackfillErrorPaginatorTypeDef",
@@ -650,14 +651,15 @@
     "RedshiftTargetTypeDef",
     "UserDefinedFunctionInputTypeDef",
     "UserDefinedFunctionTypeDef",
     "TableOptimizerRunTypeDef",
     "SearchTablesRequestRequestTypeDef",
     "StatementOutputTypeDef",
     "UpdateClassifierRequestRequestTypeDef",
+    "ViewDefinitionTypeDef",
     "AmazonRedshiftSourceTypeDef",
     "AmazonRedshiftTargetTypeDef",
     "SnowflakeTargetTypeDef",
     "PartitionIndexDescriptorPaginatorTypeDef",
     "PartitionIndexDescriptorTypeDef",
     "BatchStopJobRunResponseTypeDef",
     "BatchUpdatePartitionResponseTypeDef",
@@ -913,18 +915,18 @@
         "Table": str,
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
 BatchDeleteConnectionRequestRequestTypeDef = TypedDict(
     "BatchDeleteConnectionRequestRequestTypeDef",
     {
         "ConnectionNameList": Sequence[str],
         "CatalogId": NotRequired[str],
@@ -2017,14 +2019,15 @@
     },
 )
 EncryptionAtRestTypeDef = TypedDict(
     "EncryptionAtRestTypeDef",
     {
         "CatalogEncryptionMode": CatalogEncryptionModeType,
         "SseAwsKmsKeyId": NotRequired[str],
+        "CatalogEncryptionServiceRole": NotRequired[str],
     },
 )
 DataLakePrincipalTypeDef = TypedDict(
     "DataLakePrincipalTypeDef",
     {
         "DataLakePrincipalIdentifier": NotRequired[str],
     },
@@ -3462,14 +3465,24 @@
     {
         "Name": str,
         "Description": NotRequired[str],
         "DefaultRunProperties": NotRequired[Mapping[str, str]],
         "MaxConcurrentRuns": NotRequired[int],
     },
 )
+ViewRepresentationTypeDef = TypedDict(
+    "ViewRepresentationTypeDef",
+    {
+        "Dialect": NotRequired[ViewDialectType],
+        "DialectVersion": NotRequired[str],
+        "ViewOriginalText": NotRequired[str],
+        "ViewExpandedText": NotRequired[str],
+        "IsStale": NotRequired[bool],
+    },
+)
 WorkflowRunStatisticsTypeDef = TypedDict(
     "WorkflowRunStatisticsTypeDef",
     {
         "TotalActions": NotRequired[int],
         "TimeoutActions": NotRequired[int],
         "FailedActions": NotRequired[int],
         "StoppedActions": NotRequired[int],
@@ -5475,14 +5488,23 @@
     {
         "GrokClassifier": NotRequired[UpdateGrokClassifierRequestTypeDef],
         "XMLClassifier": NotRequired[UpdateXMLClassifierRequestTypeDef],
         "JsonClassifier": NotRequired[UpdateJsonClassifierRequestTypeDef],
         "CsvClassifier": NotRequired[UpdateCsvClassifierRequestTypeDef],
     },
 )
+ViewDefinitionTypeDef = TypedDict(
+    "ViewDefinitionTypeDef",
+    {
+        "IsProtected": NotRequired[bool],
+        "Definer": NotRequired[str],
+        "SubObjects": NotRequired[List[str]],
+        "Representations": NotRequired[List[ViewRepresentationTypeDef]],
+    },
+)
 AmazonRedshiftSourceTypeDef = TypedDict(
     "AmazonRedshiftSourceTypeDef",
     {
         "Name": NotRequired[str],
         "Data": NotRequired[AmazonRedshiftNodeDataTypeDef],
     },
 )
@@ -6854,14 +6876,16 @@
         "Parameters": NotRequired[Dict[str, str]],
         "CreatedBy": NotRequired[str],
         "IsRegisteredWithLakeFormation": NotRequired[bool],
         "TargetTable": NotRequired[TableIdentifierTypeDef],
         "CatalogId": NotRequired[str],
         "VersionId": NotRequired[str],
         "FederatedTable": NotRequired[FederatedTableTypeDef],
+        "ViewDefinition": NotRequired[ViewDefinitionTypeDef],
+        "IsMultiDialectView": NotRequired[bool],
     },
 )
 PartitionInputTypeDef = TypedDict(
     "PartitionInputTypeDef",
     {
         "Values": NotRequired[Sequence[str]],
         "LastAccessTime": NotRequired[TimestampTypeDef],
@@ -6922,14 +6946,16 @@
         "Parameters": NotRequired[Dict[str, str]],
         "CreatedBy": NotRequired[str],
         "IsRegisteredWithLakeFormation": NotRequired[bool],
         "TargetTable": NotRequired[TableIdentifierTypeDef],
         "CatalogId": NotRequired[str],
         "VersionId": NotRequired[str],
         "FederatedTable": NotRequired[FederatedTableTypeDef],
+        "ViewDefinition": NotRequired[ViewDefinitionTypeDef],
+        "IsMultiDialectView": NotRequired[bool],
     },
 )
 GetSecurityConfigurationsResponsePaginatorTypeDef = TypedDict(
     "GetSecurityConfigurationsResponsePaginatorTypeDef",
     {
         "SecurityConfigurations": List[SecurityConfigurationPaginatorTypeDef],
         "NextToken": str,
@@ -7277,15 +7303,17 @@
     "GetUnfilteredTableMetadataResponseTypeDef",
     {
         "Table": TableTypeDef,
         "AuthorizedColumns": List[str],
         "IsRegisteredWithLakeFormation": bool,
         "CellFilters": List[ColumnRowFilterTypeDef],
         "QueryAuthorizationId": str,
+        "IsMultiDialectView": bool,
         "ResourceArn": str,
+        "IsProtected": bool,
         "Permissions": List[PermissionType],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 SearchTablesResponseTypeDef = TypedDict(
     "SearchTablesResponseTypeDef",
     {
```

### Comparing `mypy-boto3-glue-1.34.7/mypy_boto3_glue.egg-info/PKG-INFO` & `mypy-boto3-glue-1.34.76/mypy_boto3_glue.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-glue
-Version: 1.34.7
-Summary: Type annotations for boto3.Glue 1.34.7 service generated with mypy-boto3-builder 7.23.0
+Version: 1.34.76
+Summary: Type annotations for boto3.Glue 1.34.76 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -25,37 +25,38 @@
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Stubs Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
 
 <a id="mypy-boto3-glue"></a>
 
 # mypy-boto3-glue
 
 [![PyPI - mypy-boto3-glue](https://img.shields.io/pypi/v/mypy-boto3-glue.svg?color=blue)](https://pypi.org/project/mypy-boto3-glue)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-glue.svg?color=blue)](https://pypi.org/project/mypy-boto3-glue)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-glue)](https://pepy.tech/project/mypy-boto3-glue)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Glue 1.34.7](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue)
+[boto3.Glue 1.34.76](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-glue docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-glue-1.34.7/mypy_boto3_glue.egg-info/SOURCES.txt` & `mypy-boto3-glue-1.34.76/mypy_boto3_glue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glue-1.34.7/setup.py` & `mypy-boto3-glue-1.34.76/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,23 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-glue",
-    version="1.34.7",
+    version="1.34.76",
     packages=["mypy_boto3_glue"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description=(
-        "Type annotations for boto3.Glue 1.34.7 service generated with mypy-boto3-builder 7.23.0"
-    ),
+    description="Type annotations for boto3.Glue 1.34.76 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

