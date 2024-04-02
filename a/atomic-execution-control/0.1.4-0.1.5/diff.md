# Comparing `tmp/atomic_execution_control-0.1.4.tar.gz` & `tmp/atomic_execution_control-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atomic_execution_control-0.1.4.tar", last modified: Fri Mar  8 06:42:46 2024, max compression
+gzip compressed data, was "atomic_execution_control-0.1.5.tar", last modified: Tue Apr  2 13:10:36 2024, max compression
```

## Comparing `atomic_execution_control-0.1.4.tar` & `atomic_execution_control-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 David      (501) staff       (20)        0 2024-03-08 06:42:46.159393 atomic_execution_control-0.1.4/
--rw-r--r--   0 David      (501) staff       (20)     1077 2024-03-06 14:57:50.000000 atomic_execution_control-0.1.4/LICENSE
--rw-r--r--   0 David      (501) staff       (20)     6209 2024-03-08 06:42:46.158608 atomic_execution_control-0.1.4/PKG-INFO
--rw-r--r--   0 David      (501) staff       (20)     5451 2024-03-08 06:31:11.000000 atomic_execution_control-0.1.4/README.md
-drwxr-xr-x   0 David      (501) staff       (20)        0 2024-03-08 06:42:46.151811 atomic_execution_control-0.1.4/atomic_execution_control/
--rw-r--r--   0 David      (501) staff       (20)       60 2024-03-07 17:01:25.000000 atomic_execution_control-0.1.4/atomic_execution_control/__init__.py
--rw-r--r--   0 David      (501) staff       (20)     9298 2024-03-07 17:06:04.000000 atomic_execution_control-0.1.4/atomic_execution_control/atomic_execution_control.py
-drwxr-xr-x   0 David      (501) staff       (20)        0 2024-03-08 06:42:46.157266 atomic_execution_control-0.1.4/atomic_execution_control.egg-info/
--rw-r--r--   0 David      (501) staff       (20)     6209 2024-03-08 06:42:46.000000 atomic_execution_control-0.1.4/atomic_execution_control.egg-info/PKG-INFO
--rw-r--r--   0 David      (501) staff       (20)      355 2024-03-08 06:42:46.000000 atomic_execution_control-0.1.4/atomic_execution_control.egg-info/SOURCES.txt
--rw-r--r--   0 David      (501) staff       (20)        1 2024-03-08 06:42:46.000000 atomic_execution_control-0.1.4/atomic_execution_control.egg-info/dependency_links.txt
--rw-r--r--   0 David      (501) staff       (20)       14 2024-03-08 06:42:46.000000 atomic_execution_control-0.1.4/atomic_execution_control.egg-info/requires.txt
--rw-r--r--   0 David      (501) staff       (20)       25 2024-03-08 06:42:46.000000 atomic_execution_control-0.1.4/atomic_execution_control.egg-info/top_level.txt
--rw-r--r--   0 David      (501) staff       (20)       38 2024-03-08 06:42:46.159537 atomic_execution_control-0.1.4/setup.cfg
--rw-r--r--   0 David      (501) staff       (20)     1073 2024-03-08 06:41:41.000000 atomic_execution_control-0.1.4/setup.py
+drwxr-xr-x   0 David      (501) staff       (20)        0 2024-04-02 13:10:36.695943 atomic_execution_control-0.1.5/
+-rw-r--r--   0 David      (501) staff       (20)     1077 2024-04-02 13:08:25.000000 atomic_execution_control-0.1.5/LICENSE
+-rw-r--r--   0 David      (501) staff       (20)     6634 2024-04-02 13:10:36.695223 atomic_execution_control-0.1.5/PKG-INFO
+-rw-r--r--   0 David      (501) staff       (20)     5876 2024-04-02 13:08:25.000000 atomic_execution_control-0.1.5/README.md
+drwxr-xr-x   0 David      (501) staff       (20)        0 2024-04-02 13:10:36.691202 atomic_execution_control-0.1.5/atomic_execution_control/
+-rw-r--r--   0 David      (501) staff       (20)       60 2024-04-02 13:08:25.000000 atomic_execution_control-0.1.5/atomic_execution_control/__init__.py
+-rw-r--r--   0 David      (501) staff       (20)    10401 2024-04-02 13:08:25.000000 atomic_execution_control-0.1.5/atomic_execution_control/atomic_execution_control.py
+drwxr-xr-x   0 David      (501) staff       (20)        0 2024-04-02 13:10:36.694301 atomic_execution_control-0.1.5/atomic_execution_control.egg-info/
+-rw-r--r--   0 David      (501) staff       (20)     6634 2024-04-02 13:10:36.000000 atomic_execution_control-0.1.5/atomic_execution_control.egg-info/PKG-INFO
+-rw-r--r--   0 David      (501) staff       (20)      355 2024-04-02 13:10:36.000000 atomic_execution_control-0.1.5/atomic_execution_control.egg-info/SOURCES.txt
+-rw-r--r--   0 David      (501) staff       (20)        1 2024-04-02 13:10:36.000000 atomic_execution_control-0.1.5/atomic_execution_control.egg-info/dependency_links.txt
+-rw-r--r--   0 David      (501) staff       (20)       14 2024-04-02 13:10:36.000000 atomic_execution_control-0.1.5/atomic_execution_control.egg-info/requires.txt
+-rw-r--r--   0 David      (501) staff       (20)       25 2024-04-02 13:10:36.000000 atomic_execution_control-0.1.5/atomic_execution_control.egg-info/top_level.txt
+-rw-r--r--   0 David      (501) staff       (20)       38 2024-04-02 13:10:36.696085 atomic_execution_control-0.1.5/setup.cfg
+-rw-r--r--   0 David      (501) staff       (20)     1072 2024-04-02 13:09:51.000000 atomic_execution_control-0.1.5/setup.py
```

### Comparing `atomic_execution_control-0.1.4/LICENSE` & `atomic_execution_control-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `atomic_execution_control-0.1.4/PKG-INFO` & `atomic_execution_control-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atomic_execution_control
-Version: 0.1.4
+Version: 0.1.5
 Summary: Ensures atomic executions across AWS services using DynamoDB to prevent race conditions in distributed applications.
 Home-page: https://github.com/jdaarevalo/atomic_execution_control
 Author: Jose David Arevalo
 Author-email: jdaarevalo@gmail.com
 Keywords: atomic execution,DynamoDB,AWS Lambda,AWS Fargate,EC2,distributed systems,concurrency control,race condition prevention,cloud computing,AWS services,state management
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -94,24 +94,36 @@
 import os
 
 # DynamoDB table and primary key
 TABLE_NAME = 'YourDynamoDBTableName'
 PRIMARY_KEY = 'YourPrimaryKey'
 
 # Test also in your local environment 
+# verify the endpoint_url, this url "http://localhost:8000" is also valid.
 endpoint_url = "http://docker.for.mac.localhost:8000/" if os.environ.get("AWS_SAM_LOCAL") else None
-
+ 
 # Initialize AtomicExecutionControl
 aec = AtomicExecutionControl(
     table_name=TABLE_NAME,
     primary_key=PRIMARY_KEY,
     region_name="eu-west-1",
     endpoint_url=endpoint_url
 )
 
+# In case you already log into an specific AWS account via AWS Single Sign-On (SSO)
+# you can send the profile_name parameter as follow.
+profile_name =  'AwsProfileName'
+aec = AtomicExecutionControl(
+    table_name=TABLE_NAME,
+    primary_key=PRIMARY_KEY,
+    region_name="eu-west-1",
+    endpoint_url=endpoint_url,
+    profile_name=profile_name
+)
+
 # Assume you have an event-driven architecture where multiple events 
 # could trigger the same task
 date_to_run = '2024-01-01'
 
 
 # delete items in Dynamo for old executions
 aec.delete_items_finished_or_old(keys=[date_to_run], item_execution_valid_for=20)
```

### Comparing `atomic_execution_control-0.1.4/README.md` & `atomic_execution_control-0.1.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -78,24 +78,36 @@
 import os
 
 # DynamoDB table and primary key
 TABLE_NAME = 'YourDynamoDBTableName'
 PRIMARY_KEY = 'YourPrimaryKey'
 
 # Test also in your local environment 
+# verify the endpoint_url, this url "http://localhost:8000" is also valid.
 endpoint_url = "http://docker.for.mac.localhost:8000/" if os.environ.get("AWS_SAM_LOCAL") else None
-
+ 
 # Initialize AtomicExecutionControl
 aec = AtomicExecutionControl(
     table_name=TABLE_NAME,
     primary_key=PRIMARY_KEY,
     region_name="eu-west-1",
     endpoint_url=endpoint_url
 )
 
+# In case you already log into an specific AWS account via AWS Single Sign-On (SSO)
+# you can send the profile_name parameter as follow.
+profile_name =  'AwsProfileName'
+aec = AtomicExecutionControl(
+    table_name=TABLE_NAME,
+    primary_key=PRIMARY_KEY,
+    region_name="eu-west-1",
+    endpoint_url=endpoint_url,
+    profile_name=profile_name
+)
+
 # Assume you have an event-driven architecture where multiple events 
 # could trigger the same task
 date_to_run = '2024-01-01'
 
 
 # delete items in Dynamo for old executions
 aec.delete_items_finished_or_old(keys=[date_to_run], item_execution_valid_for=20)
```

### Comparing `atomic_execution_control-0.1.4/atomic_execution_control/atomic_execution_control.py` & `atomic_execution_control-0.1.5/atomic_execution_control/atomic_execution_control.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,31 +27,55 @@
             self.logger.warning(message)
 
         def error(self, message):
             self.logger.error(message)
 
 class AtomicExecutionControl:
     def __init__(self, table_name:str, primary_key:str, region_name:str='eu-west-1',
-                 endpoint_url:str=None, logger=None):
+                 endpoint_url:str=None, logger=None, profile_name:str=None):
         self.table_name = table_name
         self.primary_key = primary_key
         self.region_name = region_name
         self.endpoint_url = endpoint_url
-        self.dynamodb_resource = boto3.resource('dynamodb', region_name=self.region_name,
-                                                endpoint_url=self.endpoint_url)
-        self.dynamodb_client = boto3.client('dynamodb', region_name=self.region_name,
+        self.profile_name = profile_name
+
+        # A custom session is created with the given profile_name parameter,
+        # otherwise AWS client will use the default session
+        # clients or resource clients will be related to the session
+        self.session = boto3.session.Session(profile_name=profile_name)
+        self.dynamodb_client = self.session.client('dynamodb', region_name=self.region_name,
                                             endpoint_url=self.endpoint_url)
+        self.dynamodb_resource = self.session.resource('dynamodb', region_name=self.region_name,
+                                                endpoint_url=self.endpoint_url)
+
         self.table = self.dynamodb_resource.Table(self.table_name)
         self.ITEM_EXECUTION_VALID_FOR = 20 # minutes
         self.TIME_TO_RETRY_CHECK_STATUS = 20 # seconds
         self.MAX_TIME_TO_CHECK_STATUS = 840 # seconds
         self.STATUS_EXECUTION_FINISHED = "FINISHED"
         self.STATUS_EXECUTION_IN_PROGRESS = "IN_PROGRESS"
         # Initialize or use the provided logger
         self.logger = logger if logger else Logger()
+        self.check_dynamodb_connection()
+
+    def check_dynamodb_connection(self) -> None:
+        try:
+            self.dynamodb_client.describe_table(TableName=self.table_name)
+            self.logger.info({
+                "message": f"Successfully connected to dynamodb table {self.table_name}",
+                "status": 'SUCCEEDED',
+                "action": "check_dynamodb_connection"
+            })
+        except ClientError as exception:
+            self.logger.error({
+                    "message": "Error checking connection to DynamoDB table",
+                    "error": exception.response['Error']['Message'],
+                    "status": 'FAILED',
+                    "action": "check_dynamodb_connection"
+                })
 
     def _log(self, level, message, **kwargs):
         if hasattr(self.logger, 'structure_logs'):  # Check if aws_lambda_powertools.Logger
             structured_message = {**message, **kwargs}
             getattr(self.logger, level)(structured_message)
         else:  # Fallback to standard logging
             log_message = json.dumps({"message": message, **kwargs})
```

### Comparing `atomic_execution_control-0.1.4/atomic_execution_control.egg-info/PKG-INFO` & `atomic_execution_control-0.1.5/atomic_execution_control.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atomic-execution-control
-Version: 0.1.4
+Version: 0.1.5
 Summary: Ensures atomic executions across AWS services using DynamoDB to prevent race conditions in distributed applications.
 Home-page: https://github.com/jdaarevalo/atomic_execution_control
 Author: Jose David Arevalo
 Author-email: jdaarevalo@gmail.com
 Keywords: atomic execution,DynamoDB,AWS Lambda,AWS Fargate,EC2,distributed systems,concurrency control,race condition prevention,cloud computing,AWS services,state management
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -94,24 +94,36 @@
 import os
 
 # DynamoDB table and primary key
 TABLE_NAME = 'YourDynamoDBTableName'
 PRIMARY_KEY = 'YourPrimaryKey'
 
 # Test also in your local environment 
+# verify the endpoint_url, this url "http://localhost:8000" is also valid.
 endpoint_url = "http://docker.for.mac.localhost:8000/" if os.environ.get("AWS_SAM_LOCAL") else None
-
+ 
 # Initialize AtomicExecutionControl
 aec = AtomicExecutionControl(
     table_name=TABLE_NAME,
     primary_key=PRIMARY_KEY,
     region_name="eu-west-1",
     endpoint_url=endpoint_url
 )
 
+# In case you already log into an specific AWS account via AWS Single Sign-On (SSO)
+# you can send the profile_name parameter as follow.
+profile_name =  'AwsProfileName'
+aec = AtomicExecutionControl(
+    table_name=TABLE_NAME,
+    primary_key=PRIMARY_KEY,
+    region_name="eu-west-1",
+    endpoint_url=endpoint_url,
+    profile_name=profile_name
+)
+
 # Assume you have an event-driven architecture where multiple events 
 # could trigger the same task
 date_to_run = '2024-01-01'
 
 
 # delete items in Dynamo for old executions
 aec.delete_items_finished_or_old(keys=[date_to_run], item_execution_valid_for=20)
```

### Comparing `atomic_execution_control-0.1.4/setup.py` & `atomic_execution_control-0.1.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Dynamic loading of the long description
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='atomic_execution_control',
-    version='0.1.4',
+    version='0.1.5',
     author='Jose David Arevalo',
     author_email='jdaarevalo@gmail.com',
     description='Ensures atomic executions across AWS services using DynamoDB to prevent race conditions in distributed applications.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/jdaarevalo/atomic_execution_control',
     packages=find_packages(),
@@ -21,8 +21,7 @@
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     keywords='atomic execution, DynamoDB, AWS Lambda, AWS Fargate, EC2, distributed systems, concurrency control, race condition prevention, cloud computing, AWS services, state management',
 )
-
```

