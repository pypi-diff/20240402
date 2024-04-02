# Comparing `tmp/dolbaram-0.2.0.tar.gz` & `tmp/dolbaram-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dolbaram-0.2.0.tar", max compression
+gzip compressed data, was "dolbaram-0.2.1.tar", max compression
```

## Comparing `dolbaram-0.2.0.tar` & `dolbaram-0.2.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2023-12-01 01:21:09.254669 dolbaram-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-12-01 01:21:09.254618 dolbaram-0.2.0/dolbaram/__init__.py
--rw-r--r--   0        0        0    18986 2024-04-01 07:47:20.575457 dolbaram-0.2.0/dolbaram/dolbaram.py
--rw-r--r--   0        0        0      576 2024-04-01 07:47:20.571875 dolbaram-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      896 1970-01-01 00:00:00.000000 dolbaram-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-12-01 01:21:09.254669 dolbaram-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2023-12-01 01:21:09.254618 dolbaram-0.2.1/dolbaram/__init__.py
+-rw-r--r--   0        0        0    19167 2024-04-02 05:31:59.897296 dolbaram-0.2.1/dolbaram/dolbaram.py
+-rw-r--r--   0        0        0      576 2024-04-02 05:31:59.899638 dolbaram-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      896 1970-01-01 00:00:00.000000 dolbaram-0.2.1/PKG-INFO
```

### Comparing `dolbaram-0.2.0/dolbaram/dolbaram.py` & `dolbaram-0.2.1/dolbaram/dolbaram.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from great_expectations.datasource.fluent.sql_datasource import TableAsset
 from great_expectations.exceptions import DataContextError
 from great_expectations.profile.user_configurable_profiler import UserConfigurableProfiler
 from great_expectations.validator.validator import Validator
 
 
 class Dolbaram(object):
-    def __init__(self, gx_s3_bucket_name: str, data_s3_bucket_name: str):
+    def __init__(self, gx_s3_bucket_name: str, data_s3_bucket_name: str, athena_workgroup: Optional[str] = None):
         '''
 
         :param data_s3_bucket_name:
         '''
 
         self.DATASOURCE_S3_PANDAS_NAME = 's3'
         self.DATASOURCE_S3_SPARK_NAME = 'spark'
@@ -112,17 +112,20 @@
                 'enabled': True
             }
         )
         self.context = EphemeralDataContext(project_config=self.data_context_config)
         self.s3_datasource = self.context.sources.add_pandas_s3(
             name=self.DATASOURCE_S3_PANDAS_NAME, bucket=self.DATA_S3_BUCKET_NAME, boto3_options={}
         )
+        connection_string = f'awsathena+rest://@athena.ap-northeast-2.amazonaws.com/?s3_staging_dir=s3://{self.DATA_S3_BUCKET_NAME}/query_results/'
+        if athena_workgroup:
+            connection_string += f'&work_group={athena_workgroup}'
         self.athena_datasource = self.context.sources.add_sql(
             name=self.DATASOURCE_ATHENA_NAME,
-            connection_string=f'awsathena+rest://@athena.ap-northeast-2.amazonaws.com/?s3_staging_dir=s3://{self.DATA_S3_BUCKET_NAME}/query_results/'
+            connection_string=connection_string
         )
         self.spark_datasource = self.context.sources.add_or_update_spark_s3(
             name=self.DATASOURCE_S3_SPARK_NAME, bucket=self.DATA_S3_BUCKET_NAME, boto3_options={}
         )
 
     def make_suite(self, suite_name: str) -> ExpectationSuite:
         '''
@@ -463,8 +466,7 @@
         suite = self.add_expectations(suite_name, ecs)
         result = self.checkpoint(athena_database_name=db_name,
                                  athena_table_name=table_name,
                                  suite=suite,
                                  engine='athena')
         pprint(f'result={result}')
         return result
-
```

### Comparing `dolbaram-0.2.0/pyproject.toml` & `dolbaram-0.2.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dolbaram"
-version = "0.2.0"
+version = "0.2.1"
 description = ""
 authors = ["Kwangsik Lee <lks21c@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 fire = "^0.4.0"
```

### Comparing `dolbaram-0.2.0/PKG-INFO` & `dolbaram-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dolbaram
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 Author: Kwangsik Lee
 Author-email: lks21c@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

