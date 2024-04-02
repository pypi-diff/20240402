# Comparing `tmp/aws-lambda-typing-2.9.8.tar.gz` & `tmp/aws-lambda-typing-2.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-lambda-typing-2.9.8.tar", max compression
+gzip compressed data, was "aws-lambda-typing-2.9.9.tar", max compression
```

## Comparing `aws-lambda-typing-2.9.8.tar` & `aws-lambda-typing-2.9.9.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     1073 2022-01-16 16:24:30.224305 aws-lambda-typing-2.9.8/LICENSE
--rw-r--r--   0        0        0     3057 2022-01-16 16:24:30.224305 aws-lambda-typing-2.9.8/README.md
--rw-r--r--   0        0        0     1390 2022-01-16 16:24:30.228305 aws-lambda-typing-2.9.8/pyproject.toml
--rw-r--r--   0        0        0        0 2022-01-16 16:24:30.228305 aws-lambda-typing-2.9.8/src/aws_lambda_typing/__init__.py
--rw-r--r--   0        0        0       50 2022-01-16 16:24:30.228305 aws-lambda-typing-2.9.8/src/aws_lambda_typing/common/__init__.py
--rw-r--r--   0        0        0     1763 2022-01-16 16:24:30.228305 aws-lambda-typing-2.9.8/src/aws_lambda_typing/common/iam.py
--rw-r--r--   0        0        0      172 2022-01-16 16:24:30.228305 aws-lambda-typing-2.9.8/src/aws_lambda_typing/context/__init__.py
--rw-r--r--   0        0        0     2922 2022-01-16 16:24:30.228305 aws-lambda-typing-2.9.8/src/aws_lambda_typing/context/context.py
--rw-r--r--   0        0        0     2028 2022-01-16 16:24:30.228305 aws-lambda-typing-2.9.8/src/aws_lambda_typing/events/__init__.py
--rw-r--r--   0        0        0     1100 2022-01-16 16:24:30.228305 aws-lambda-typing-2.9.8/src/aws_lambda_typing/events/alb.py
--rw-r--r--   0        0        0     1381 2022-01-16 16:24:30.228305 aws-lambda-typing-2.9.8/src/aws_lambda_typing/events/api_gateway_authorizer.py
--rw-r--r--   0        0        0     6911 2022-01-16 16:24:30.228305 aws-lambda-typing-2.9.8/src/aws_lambda_typing/events/api_gateway_proxy.py
--rw-r--r--   0        0        0     3136 2022-01-16 16:24:30.228305 aws-lambda-typing-2.9.8/src/aws_lambda_typing/events/app_sync_resolver.py
--rw-r--r--   0        0        0     2625 2022-01-16 16:24:30.228305 aws-lambda-typing-2.9.8/src/aws_lambda_typing/events/cloud_formation_custom_resource.py
--rw-r--r--   0        0        0      889 2022-01-16 16:24:30.228305 aws-lambda-typing-2.9.8/src/aws_lambda_typing/events/cloud_watch_events.py
--rw-r--r--   0        0        0     1461 2022-01-16 16:24:30.228305 aws-lambda-typing-2.9.8/src/aws_lambda_typing/events/cloud_watch_logs.py
--rw-r--r--   0        0        0     1517 2022-01-16 16:24:30.228305 aws-lambda-typing-2.9.8/src/aws_lambda_typing/events/code_commit.py
--rw-r--r--   0        0        0     2925 2022-01-16 16:24:30.228305 aws-lambda-typing-2.9.8/src/aws_lambda_typing/events/code_pipeline.py
--rw-r--r--   0        0        0      765 2022-01-16 16:24:30.228305 aws-lambda-typing-2.9.8/src/aws_lambda_typing/events/config.py
--rw-r--r--   0        0        0     2554 2022-01-16 16:24:30.228305 aws-lambda-typing-2.9.8/src/aws_lambda_typing/events/dynamodb_stream.py
--rw-r--r--   0        0        0      693 2022-01-16 16:24:30.228305 aws-lambda-typing-2.9.8/src/aws_lambda_typing/events/iot.py
--rw-r--r--   0        0        0     1396 2022-01-16 16:24:30.228305 aws-lambda-typing-2.9.8/src/aws_lambda_typing/events/kinesis_firehose.py
--rw-r--r--   0        0        0     1327 2022-01-16 16:24:30.228305 aws-lambda-typing-2.9.8/src/aws_lambda_typing/events/kinesis_stream.py
--rw-r--r--   0        0        0     1271 2022-01-16 16:24:30.228305 aws-lambda-typing-2.9.8/src/aws_lambda_typing/events/mq.py
--rw-r--r--   0        0        0     1046 2022-01-16 16:24:30.228305 aws-lambda-typing-2.9.8/src/aws_lambda_typing/events/msk.py
--rw-r--r--   0        0        0     3288 2022-01-16 16:24:30.228305 aws-lambda-typing-2.9.8/src/aws_lambda_typing/events/s3.py
--rw-r--r--   0        0        0     2008 2022-01-16 16:24:30.228305 aws-lambda-typing-2.9.8/src/aws_lambda_typing/events/s3_batch.py
--rw-r--r--   0        0        0      694 2022-01-16 16:24:30.228305 aws-lambda-typing-2.9.8/src/aws_lambda_typing/events/secrets_manager.py
--rw-r--r--   0        0        0     6180 2022-01-16 16:24:30.228305 aws-lambda-typing-2.9.8/src/aws_lambda_typing/events/ses.py
--rw-r--r--   0        0        0     1599 2022-01-16 16:24:30.228305 aws-lambda-typing-2.9.8/src/aws_lambda_typing/events/sns.py
--rw-r--r--   0        0        0     2191 2022-01-16 16:24:30.228305 aws-lambda-typing-2.9.8/src/aws_lambda_typing/events/sqs.py
--rw-r--r--   0        0        0        0 2022-01-16 16:24:30.228305 aws-lambda-typing-2.9.8/src/aws_lambda_typing/py.typed
--rw-r--r--   0        0        0      447 2022-01-16 16:24:30.228305 aws-lambda-typing-2.9.8/src/aws_lambda_typing/responses/__init__.py
--rw-r--r--   0        0        0      702 2022-01-16 16:24:30.228305 aws-lambda-typing-2.9.8/src/aws_lambda_typing/responses/alb.py
--rw-r--r--   0        0        0      797 2022-01-16 16:24:30.228305 aws-lambda-typing-2.9.8/src/aws_lambda_typing/responses/api_gateway_authorizer.py
--rw-r--r--   0        0        0     1889 2022-01-16 16:24:30.228305 aws-lambda-typing-2.9.8/src/aws_lambda_typing/responses/api_gateway_proxy.py
--rw-r--r--   0        0        0      536 2022-01-16 16:24:30.228305 aws-lambda-typing-2.9.8/src/aws_lambda_typing/responses/iot.py
--rw-r--r--   0        0        0     1141 2022-01-16 16:24:30.228305 aws-lambda-typing-2.9.8/src/aws_lambda_typing/responses/s3_batch.py
--rw-r--r--   0        0        0     4127 2022-01-16 16:25:06.756220 aws-lambda-typing-2.9.8/setup.py
--rw-r--r--   0        0        0     4050 2022-01-16 16:25:06.756566 aws-lambda-typing-2.9.8/PKG-INFO
+-rw-r--r--   0        0        0     1073 2022-01-16 16:32:02.863044 aws-lambda-typing-2.9.9/LICENSE
+-rw-r--r--   0        0        0     3057 2022-01-16 16:32:02.863044 aws-lambda-typing-2.9.9/README.md
+-rw-r--r--   0        0        0     1391 2022-01-16 16:32:02.867044 aws-lambda-typing-2.9.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-01-16 16:32:02.871044 aws-lambda-typing-2.9.9/src/aws_lambda_typing/__init__.py
+-rw-r--r--   0        0        0       50 2022-01-16 16:32:02.871044 aws-lambda-typing-2.9.9/src/aws_lambda_typing/common/__init__.py
+-rw-r--r--   0        0        0     1763 2022-01-16 16:32:02.871044 aws-lambda-typing-2.9.9/src/aws_lambda_typing/common/iam.py
+-rw-r--r--   0        0        0      172 2022-01-16 16:32:02.871044 aws-lambda-typing-2.9.9/src/aws_lambda_typing/context/__init__.py
+-rw-r--r--   0        0        0     2922 2022-01-16 16:32:02.871044 aws-lambda-typing-2.9.9/src/aws_lambda_typing/context/context.py
+-rw-r--r--   0        0        0     2028 2022-01-16 16:32:02.871044 aws-lambda-typing-2.9.9/src/aws_lambda_typing/events/__init__.py
+-rw-r--r--   0        0        0     1100 2022-01-16 16:32:02.871044 aws-lambda-typing-2.9.9/src/aws_lambda_typing/events/alb.py
+-rw-r--r--   0        0        0     1381 2022-01-16 16:32:02.871044 aws-lambda-typing-2.9.9/src/aws_lambda_typing/events/api_gateway_authorizer.py
+-rw-r--r--   0        0        0     6911 2022-01-16 16:32:02.871044 aws-lambda-typing-2.9.9/src/aws_lambda_typing/events/api_gateway_proxy.py
+-rw-r--r--   0        0        0     3136 2022-01-16 16:32:02.871044 aws-lambda-typing-2.9.9/src/aws_lambda_typing/events/app_sync_resolver.py
+-rw-r--r--   0        0        0     2625 2022-01-16 16:32:02.871044 aws-lambda-typing-2.9.9/src/aws_lambda_typing/events/cloud_formation_custom_resource.py
+-rw-r--r--   0        0        0      889 2022-01-16 16:32:02.871044 aws-lambda-typing-2.9.9/src/aws_lambda_typing/events/cloud_watch_events.py
+-rw-r--r--   0        0        0     1461 2022-01-16 16:32:02.871044 aws-lambda-typing-2.9.9/src/aws_lambda_typing/events/cloud_watch_logs.py
+-rw-r--r--   0        0        0     1517 2022-01-16 16:32:02.871044 aws-lambda-typing-2.9.9/src/aws_lambda_typing/events/code_commit.py
+-rw-r--r--   0        0        0     2925 2022-01-16 16:32:02.871044 aws-lambda-typing-2.9.9/src/aws_lambda_typing/events/code_pipeline.py
+-rw-r--r--   0        0        0      765 2022-01-16 16:32:02.871044 aws-lambda-typing-2.9.9/src/aws_lambda_typing/events/config.py
+-rw-r--r--   0        0        0     2554 2022-01-16 16:32:02.871044 aws-lambda-typing-2.9.9/src/aws_lambda_typing/events/dynamodb_stream.py
+-rw-r--r--   0        0        0      693 2022-01-16 16:32:02.871044 aws-lambda-typing-2.9.9/src/aws_lambda_typing/events/iot.py
+-rw-r--r--   0        0        0     1396 2022-01-16 16:32:02.871044 aws-lambda-typing-2.9.9/src/aws_lambda_typing/events/kinesis_firehose.py
+-rw-r--r--   0        0        0     1327 2022-01-16 16:32:02.871044 aws-lambda-typing-2.9.9/src/aws_lambda_typing/events/kinesis_stream.py
+-rw-r--r--   0        0        0     1271 2022-01-16 16:32:02.871044 aws-lambda-typing-2.9.9/src/aws_lambda_typing/events/mq.py
+-rw-r--r--   0        0        0     1046 2022-01-16 16:32:02.871044 aws-lambda-typing-2.9.9/src/aws_lambda_typing/events/msk.py
+-rw-r--r--   0        0        0     3288 2022-01-16 16:32:02.871044 aws-lambda-typing-2.9.9/src/aws_lambda_typing/events/s3.py
+-rw-r--r--   0        0        0     2008 2022-01-16 16:32:02.871044 aws-lambda-typing-2.9.9/src/aws_lambda_typing/events/s3_batch.py
+-rw-r--r--   0        0        0      694 2022-01-16 16:32:02.871044 aws-lambda-typing-2.9.9/src/aws_lambda_typing/events/secrets_manager.py
+-rw-r--r--   0        0        0     6180 2022-01-16 16:32:02.871044 aws-lambda-typing-2.9.9/src/aws_lambda_typing/events/ses.py
+-rw-r--r--   0        0        0     1599 2022-01-16 16:32:02.871044 aws-lambda-typing-2.9.9/src/aws_lambda_typing/events/sns.py
+-rw-r--r--   0        0        0     2191 2022-01-16 16:32:02.871044 aws-lambda-typing-2.9.9/src/aws_lambda_typing/events/sqs.py
+-rw-r--r--   0        0        0        0 2022-01-16 16:32:02.871044 aws-lambda-typing-2.9.9/src/aws_lambda_typing/py.typed
+-rw-r--r--   0        0        0      447 2022-01-16 16:32:02.871044 aws-lambda-typing-2.9.9/src/aws_lambda_typing/responses/__init__.py
+-rw-r--r--   0        0        0      702 2022-01-16 16:32:02.871044 aws-lambda-typing-2.9.9/src/aws_lambda_typing/responses/alb.py
+-rw-r--r--   0        0        0      797 2022-01-16 16:32:02.871044 aws-lambda-typing-2.9.9/src/aws_lambda_typing/responses/api_gateway_authorizer.py
+-rw-r--r--   0        0        0     1889 2022-01-16 16:32:02.871044 aws-lambda-typing-2.9.9/src/aws_lambda_typing/responses/api_gateway_proxy.py
+-rw-r--r--   0        0        0      536 2022-01-16 16:32:02.871044 aws-lambda-typing-2.9.9/src/aws_lambda_typing/responses/iot.py
+-rw-r--r--   0        0        0     1141 2022-01-16 16:32:02.871044 aws-lambda-typing-2.9.9/src/aws_lambda_typing/responses/s3_batch.py
+-rw-r--r--   0        0        0     4127 2022-01-16 16:32:47.514249 aws-lambda-typing-2.9.9/setup.py
+-rw-r--r--   0        0        0     4050 2022-01-16 16:32:47.514832 aws-lambda-typing-2.9.9/PKG-INFO
```

### Comparing `aws-lambda-typing-2.9.8/LICENSE` & `aws-lambda-typing-2.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-lambda-typing-2.9.8/README.md` & `aws-lambda-typing-2.9.9/README.md`

 * *Files identical despite different names*

### Comparing `aws-lambda-typing-2.9.8/pyproject.toml` & `aws-lambda-typing-2.9.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aws-lambda-typing"
-version = "2.9.8"
+version = "2.9.9"
 description = "A package that provides type hints for AWS Lambda event, context and response objects"
 authors = ["Mousa Zeid Baker"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/MousaZeidBaker/aws-lambda-typing"
 repository = "https://github.com/MousaZeidBaker/aws-lambda-typing"
 keywords=[
@@ -38,16 +38,16 @@
     {version = "^20.8b1", python = "<=3.6.2"},
     {version = "^21.12b0", python = ">3.6.2"},
 ]
 flake8 = "^4.0.1"
 flake8-black = "^0.2.3"
 flake8-isort = "^4.1.1"
 flake8-eradicate = "^1.2.0"
-isort = { version = "^5.9.3", python = "^3.6.1" }
-pre-commit = { version = "^2.15.0", python = "^3.6.1" }
+isort = { version = "^5.10.1", python = "^3.6.1" }
+pre-commit = { version = "^2.16.0", python = "^3.6.1" }
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 80
```

### Comparing `aws-lambda-typing-2.9.8/src/aws_lambda_typing/common/iam.py` & `aws-lambda-typing-2.9.9/src/aws_lambda_typing/common/iam.py`

 * *Files identical despite different names*

### Comparing `aws-lambda-typing-2.9.8/src/aws_lambda_typing/context/context.py` & `aws-lambda-typing-2.9.9/src/aws_lambda_typing/context/context.py`

 * *Files identical despite different names*

### Comparing `aws-lambda-typing-2.9.8/src/aws_lambda_typing/events/__init__.py` & `aws-lambda-typing-2.9.9/src/aws_lambda_typing/events/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-lambda-typing-2.9.8/src/aws_lambda_typing/events/alb.py` & `aws-lambda-typing-2.9.9/src/aws_lambda_typing/events/alb.py`

 * *Files identical despite different names*

### Comparing `aws-lambda-typing-2.9.8/src/aws_lambda_typing/events/api_gateway_authorizer.py` & `aws-lambda-typing-2.9.9/src/aws_lambda_typing/events/api_gateway_authorizer.py`

 * *Files identical despite different names*

### Comparing `aws-lambda-typing-2.9.8/src/aws_lambda_typing/events/api_gateway_proxy.py` & `aws-lambda-typing-2.9.9/src/aws_lambda_typing/events/api_gateway_proxy.py`

 * *Files identical despite different names*

### Comparing `aws-lambda-typing-2.9.8/src/aws_lambda_typing/events/app_sync_resolver.py` & `aws-lambda-typing-2.9.9/src/aws_lambda_typing/events/app_sync_resolver.py`

 * *Files identical despite different names*

### Comparing `aws-lambda-typing-2.9.8/src/aws_lambda_typing/events/cloud_formation_custom_resource.py` & `aws-lambda-typing-2.9.9/src/aws_lambda_typing/events/cloud_formation_custom_resource.py`

 * *Files identical despite different names*

### Comparing `aws-lambda-typing-2.9.8/src/aws_lambda_typing/events/cloud_watch_events.py` & `aws-lambda-typing-2.9.9/src/aws_lambda_typing/events/cloud_watch_events.py`

 * *Files identical despite different names*

### Comparing `aws-lambda-typing-2.9.8/src/aws_lambda_typing/events/cloud_watch_logs.py` & `aws-lambda-typing-2.9.9/src/aws_lambda_typing/events/cloud_watch_logs.py`

 * *Files identical despite different names*

### Comparing `aws-lambda-typing-2.9.8/src/aws_lambda_typing/events/code_commit.py` & `aws-lambda-typing-2.9.9/src/aws_lambda_typing/events/code_commit.py`

 * *Files identical despite different names*

### Comparing `aws-lambda-typing-2.9.8/src/aws_lambda_typing/events/code_pipeline.py` & `aws-lambda-typing-2.9.9/src/aws_lambda_typing/events/code_pipeline.py`

 * *Files identical despite different names*

### Comparing `aws-lambda-typing-2.9.8/src/aws_lambda_typing/events/config.py` & `aws-lambda-typing-2.9.9/src/aws_lambda_typing/events/config.py`

 * *Files identical despite different names*

### Comparing `aws-lambda-typing-2.9.8/src/aws_lambda_typing/events/dynamodb_stream.py` & `aws-lambda-typing-2.9.9/src/aws_lambda_typing/events/dynamodb_stream.py`

 * *Files identical despite different names*

### Comparing `aws-lambda-typing-2.9.8/src/aws_lambda_typing/events/iot.py` & `aws-lambda-typing-2.9.9/src/aws_lambda_typing/events/iot.py`

 * *Files identical despite different names*

### Comparing `aws-lambda-typing-2.9.8/src/aws_lambda_typing/events/kinesis_firehose.py` & `aws-lambda-typing-2.9.9/src/aws_lambda_typing/events/kinesis_firehose.py`

 * *Files identical despite different names*

### Comparing `aws-lambda-typing-2.9.8/src/aws_lambda_typing/events/kinesis_stream.py` & `aws-lambda-typing-2.9.9/src/aws_lambda_typing/events/kinesis_stream.py`

 * *Files identical despite different names*

### Comparing `aws-lambda-typing-2.9.8/src/aws_lambda_typing/events/mq.py` & `aws-lambda-typing-2.9.9/src/aws_lambda_typing/events/mq.py`

 * *Files identical despite different names*

### Comparing `aws-lambda-typing-2.9.8/src/aws_lambda_typing/events/msk.py` & `aws-lambda-typing-2.9.9/src/aws_lambda_typing/events/msk.py`

 * *Files identical despite different names*

### Comparing `aws-lambda-typing-2.9.8/src/aws_lambda_typing/events/s3.py` & `aws-lambda-typing-2.9.9/src/aws_lambda_typing/events/s3.py`

 * *Files identical despite different names*

### Comparing `aws-lambda-typing-2.9.8/src/aws_lambda_typing/events/s3_batch.py` & `aws-lambda-typing-2.9.9/src/aws_lambda_typing/events/s3_batch.py`

 * *Files identical despite different names*

### Comparing `aws-lambda-typing-2.9.8/src/aws_lambda_typing/events/secrets_manager.py` & `aws-lambda-typing-2.9.9/src/aws_lambda_typing/events/secrets_manager.py`

 * *Files identical despite different names*

### Comparing `aws-lambda-typing-2.9.8/src/aws_lambda_typing/events/ses.py` & `aws-lambda-typing-2.9.9/src/aws_lambda_typing/events/ses.py`

 * *Files identical despite different names*

### Comparing `aws-lambda-typing-2.9.8/src/aws_lambda_typing/events/sns.py` & `aws-lambda-typing-2.9.9/src/aws_lambda_typing/events/sns.py`

 * *Files identical despite different names*

### Comparing `aws-lambda-typing-2.9.8/src/aws_lambda_typing/events/sqs.py` & `aws-lambda-typing-2.9.9/src/aws_lambda_typing/events/sqs.py`

 * *Files identical despite different names*

### Comparing `aws-lambda-typing-2.9.8/src/aws_lambda_typing/responses/alb.py` & `aws-lambda-typing-2.9.9/src/aws_lambda_typing/responses/alb.py`

 * *Files identical despite different names*

### Comparing `aws-lambda-typing-2.9.8/src/aws_lambda_typing/responses/api_gateway_authorizer.py` & `aws-lambda-typing-2.9.9/src/aws_lambda_typing/responses/api_gateway_authorizer.py`

 * *Files identical despite different names*

### Comparing `aws-lambda-typing-2.9.8/src/aws_lambda_typing/responses/api_gateway_proxy.py` & `aws-lambda-typing-2.9.9/src/aws_lambda_typing/responses/api_gateway_proxy.py`

 * *Files identical despite different names*

### Comparing `aws-lambda-typing-2.9.8/src/aws_lambda_typing/responses/iot.py` & `aws-lambda-typing-2.9.9/src/aws_lambda_typing/responses/iot.py`

 * *Files identical despite different names*

### Comparing `aws-lambda-typing-2.9.8/src/aws_lambda_typing/responses/s3_batch.py` & `aws-lambda-typing-2.9.9/src/aws_lambda_typing/responses/s3_batch.py`

 * *Files identical despite different names*

### Comparing `aws-lambda-typing-2.9.8/setup.py` & `aws-lambda-typing-2.9.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 {'': ['*']}
 
 extras_require = \
 {':python_version < "3.8"': ['typing-extensions>=4.0.1,<5.0.0']}
 
 setup_kwargs = {
     'name': 'aws-lambda-typing',
-    'version': '2.9.8',
+    'version': '2.9.9',
     'description': 'A package that provides type hints for AWS Lambda event, context and response objects',
     'long_description': "# AWS Lambda Typing\n\n![build](https://github.com/MousaZeidBaker/aws-lambda-typing/workflows/Publish/badge.svg)\n![test](https://github.com/MousaZeidBaker/aws-lambda-typing/workflows/Test/badge.svg)\n[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)\n![python_version](https://img.shields.io/badge/python-%3E=3.6-blue.svg)\n[![pypi_v](https://img.shields.io/pypi/v/aws-lambda-typing.svg)](https://pypi.org/project/aws-lambda-typing)\n[![pypi_dm](https://img.shields.io/pypi/dm/aws-lambda-typing.svg)](https://pypi.org/project/aws-lambda-typing)\n\nA package that provides type hints for AWS Lambda event, context and response\nobjects. It's a convenient way to get autocomplete and type hints built into\nIDEs. Type annotations are not checked at runtime but are only enforced by third\nparty tools such as type checkers, IDEs, linters, etc.\n\n##### Table of Contents\n- [Usage](#usage)\n- [Demo](#demo)\n- [Types](#types)\n  - [Context](#context)\n  - [Events](#events)\n  - [Responses](#responses)\n- [Test](#test)\n- [Contributing](#contributing)\n- [Issues](#issues)\n\n## Usage\n### Example: AWS SQS event\n\n```python\nfrom aws_lambda_typing import context as context_, events\n\n\ndef handler(event: events.SQSEvent, context: context_.Context) -> None:\n    for record in event['Records']:\n        print(record['body'])\n\n    print(context.get_remaining_time_in_millis())\n\n    message: events.sqs.SQSMessage\n\n```\n\n## Demo\n### IDE autocomplete\n![ide_autocomplete](https://raw.githubusercontent.com/MousaZeidBaker/aws-lambda-typing/master/media/ide_autocomplete.gif)\n\n### IDE code reference information\n![code_reference_information](https://raw.githubusercontent.com/MousaZeidBaker/aws-lambda-typing/master/media/code_reference_information.gif)\n\n## Types\n### Context\n- Context\n\n### Events\n- ALBEvent\n- APIGatewayRequestAuthorizerEvent\n- APIGatewayTokenAuthorizerEvent\n- APIGatewayProxyEventV1\n- APIGatewayProxyEventV2\n- AppSyncResolverEvent\n- CloudFormationCustomResourceEvent\n- CloudWatchEventsMessageEvent\n- CloudWatchLogsEvent\n- CodeCommitMessageEvent\n- CodePipelineEvent\n- ConfigEvent\n- DynamoDBStreamEvent\n- IoTPreProvisioningHookEvent\n- KinesisFirehoseEvent\n- KinesisStreamEvent\n- MQEvent\n- MSKEvent\n- S3Event\n- S3BatchEvent\n- SecretsManagerRotationEvent\n- SESEvent\n- SNSEvent\n- SQSEvent\n\n### Responses\n- ALBResponse\n- APIGatewayAuthorizerResponse\n- APIGatewayProxyResponseV1\n- APIGatewayProxyResponseV2\n- IoTPreProvisioningHookResponse\n- S3BatchResponse\n\n### Other\n- PolicyDocument\n\n## Develop\nActivate virtual environment\n```shell\npoetry shell\n```\n\nInstall dependencies\n```shell\npoetry install --remove-untracked\n```\n\nInstall git hooks\n```shell\npre-commit install --hook-type pre-commit\n```\n\nRun tests\n```shell\nmypy tests\n```\n\nRun linter\n```shell\nflake8 .\n```\n\nFormat code\n```shell\nblack .\n```\n\nSort imports\n```shell\nisort .\n```\n\n## Contributing\nContributions are welcome via pull requests.\n\n## Issues\nIf you encounter any problems, please file an\n[issue](https://github.com/MousaZeidBaker/aws-lambda-typing/issues) along with a\ndetailed description.\n",
     'author': 'Mousa Zeid Baker',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/MousaZeidBaker/aws-lambda-typing',
```

### Comparing `aws-lambda-typing-2.9.8/PKG-INFO` & `aws-lambda-typing-2.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-lambda-typing
-Version: 2.9.8
+Version: 2.9.9
 Summary: A package that provides type hints for AWS Lambda event, context and response objects
 Home-page: https://github.com/MousaZeidBaker/aws-lambda-typing
 License: MIT
 Keywords: typing,type hints,aws,lambda,serverless,development
 Author: Mousa Zeid Baker
 Requires-Python: >=3.6,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

