# Comparing `tmp/alibabacloud_alikafka20190916-2.6.2.tar.gz` & `tmp/alibabacloud_alikafka20190916-2.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_alikafka20190916-2.6.2.tar", last modified: Mon Mar 25 17:12:30 2024, max compression
+gzip compressed data, was "dist/alibabacloud_alikafka20190916-2.6.3.tar", last modified: Tue Apr  2 17:18:03 2024, max compression
```

## Comparing `alibabacloud_alikafka20190916-2.6.2.tar` & `alibabacloud_alikafka20190916-2.6.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:12:30.000000 alibabacloud_alikafka20190916-2.6.2/
--rw-r--r--   0 root         (0) root         (0)     5547 2024-03-25 17:12:30.000000 alibabacloud_alikafka20190916-2.6.2/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-03-25 17:12:30.000000 alibabacloud_alikafka20190916-2.6.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-03-25 17:12:30.000000 alibabacloud_alikafka20190916-2.6.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2440 2024-03-25 17:12:30.000000 alibabacloud_alikafka20190916-2.6.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1115 2024-03-25 17:12:30.000000 alibabacloud_alikafka20190916-2.6.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1200 2024-03-25 17:12:30.000000 alibabacloud_alikafka20190916-2.6.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:12:30.000000 alibabacloud_alikafka20190916-2.6.2/alibabacloud_alikafka20190916/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-25 17:12:30.000000 alibabacloud_alikafka20190916-2.6.2/alibabacloud_alikafka20190916/__init__.py
--rw-r--r--   0 root         (0) root         (0)   178184 2024-03-25 17:12:30.000000 alibabacloud_alikafka20190916-2.6.2/alibabacloud_alikafka20190916/client.py
--rw-r--r--   0 root         (0) root         (0)   376368 2024-03-25 17:12:30.000000 alibabacloud_alikafka20190916-2.6.2/alibabacloud_alikafka20190916/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:12:30.000000 alibabacloud_alikafka20190916-2.6.2/alibabacloud_alikafka20190916.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2440 2024-03-25 17:12:30.000000 alibabacloud_alikafka20190916-2.6.2/alibabacloud_alikafka20190916.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      460 2024-03-25 17:12:30.000000 alibabacloud_alikafka20190916-2.6.2/alibabacloud_alikafka20190916.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-25 17:12:30.000000 alibabacloud_alikafka20190916-2.6.2/alibabacloud_alikafka20190916.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-03-25 17:12:30.000000 alibabacloud_alikafka20190916-2.6.2/alibabacloud_alikafka20190916.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2024-03-25 17:12:30.000000 alibabacloud_alikafka20190916-2.6.2/alibabacloud_alikafka20190916.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-25 17:12:30.000000 alibabacloud_alikafka20190916-2.6.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2640 2024-03-25 17:12:30.000000 alibabacloud_alikafka20190916-2.6.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:18:03.000000 alibabacloud_alikafka20190916-2.6.3/
+-rw-r--r--   0 root         (0) root         (0)     5628 2024-04-02 17:18:03.000000 alibabacloud_alikafka20190916-2.6.3/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-02 17:18:03.000000 alibabacloud_alikafka20190916-2.6.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-02 17:18:03.000000 alibabacloud_alikafka20190916-2.6.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2440 2024-04-02 17:18:03.000000 alibabacloud_alikafka20190916-2.6.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1115 2024-04-02 17:18:03.000000 alibabacloud_alikafka20190916-2.6.3/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1200 2024-04-02 17:18:03.000000 alibabacloud_alikafka20190916-2.6.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:18:03.000000 alibabacloud_alikafka20190916-2.6.3/alibabacloud_alikafka20190916/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-02 17:18:03.000000 alibabacloud_alikafka20190916-2.6.3/alibabacloud_alikafka20190916/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   180756 2024-04-02 17:18:03.000000 alibabacloud_alikafka20190916-2.6.3/alibabacloud_alikafka20190916/client.py
+-rw-r--r--   0 root         (0) root         (0)   384021 2024-04-02 17:18:03.000000 alibabacloud_alikafka20190916-2.6.3/alibabacloud_alikafka20190916/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:18:03.000000 alibabacloud_alikafka20190916-2.6.3/alibabacloud_alikafka20190916.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2440 2024-04-02 17:18:03.000000 alibabacloud_alikafka20190916-2.6.3/alibabacloud_alikafka20190916.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      460 2024-04-02 17:18:03.000000 alibabacloud_alikafka20190916-2.6.3/alibabacloud_alikafka20190916.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-02 17:18:03.000000 alibabacloud_alikafka20190916-2.6.3/alibabacloud_alikafka20190916.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-02 17:18:03.000000 alibabacloud_alikafka20190916-2.6.3/alibabacloud_alikafka20190916.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2024-04-02 17:18:03.000000 alibabacloud_alikafka20190916-2.6.3/alibabacloud_alikafka20190916.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-02 17:18:03.000000 alibabacloud_alikafka20190916-2.6.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2640 2024-04-02 17:18:03.000000 alibabacloud_alikafka20190916-2.6.3/setup.py
```

### Comparing `alibabacloud_alikafka20190916-2.6.2/ChangeLog.md` & `alibabacloud_alikafka20190916-2.6.3/ChangeLog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+2024-03-25 Version: 2.6.2
+- Update API GetInstanceList: update response param.
+
+
 2024-03-20 Version: 2.6.1
 - Update API CreatePrePayOrder: add param Duration.
 - Update API CreatePrePayOrder: add param PaidType.
 - Update API CreatePrePayOrder: update param DeployType.
 - Update API CreatePrePayOrder: update param DiskSize.
 - Update API CreatePrePayOrder: update param DiskType.
 - Update API GetConsumerList: add param CurrentPage.
```

### Comparing `alibabacloud_alikafka20190916-2.6.2/LICENSE` & `alibabacloud_alikafka20190916-2.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_alikafka20190916-2.6.2/PKG-INFO` & `alibabacloud_alikafka20190916-2.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_alikafka20190916
-Version: 2.6.2
+Version: 2.6.3
 Summary: Alibaba Cloud MQ for Kafka (20190916) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_alikafka20190916-2.6.2/README-CN.md` & `alibabacloud_alikafka20190916-2.6.3/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_alikafka20190916-2.6.2/README.md` & `alibabacloud_alikafka20190916-2.6.3/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_alikafka20190916-2.6.2/alibabacloud_alikafka20190916/client.py` & `alibabacloud_alikafka20190916-2.6.3/alibabacloud_alikafka20190916/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -202,20 +202,26 @@
         request: alikafka_20190916_models.CreateAclRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.CreateAclResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.acl_operation_type):
             query['AclOperationType'] = request.acl_operation_type
+        if not UtilClient.is_unset(request.acl_operation_types):
+            query['AclOperationTypes'] = request.acl_operation_types
+        if not UtilClient.is_unset(request.acl_permission_type):
+            query['AclPermissionType'] = request.acl_permission_type
         if not UtilClient.is_unset(request.acl_resource_name):
             query['AclResourceName'] = request.acl_resource_name
         if not UtilClient.is_unset(request.acl_resource_pattern_type):
             query['AclResourcePatternType'] = request.acl_resource_pattern_type
         if not UtilClient.is_unset(request.acl_resource_type):
             query['AclResourceType'] = request.acl_resource_type
+        if not UtilClient.is_unset(request.host):
+            query['Host'] = request.host
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.username):
             query['Username'] = request.username
         req = open_api_models.OpenApiRequest(
@@ -242,20 +248,26 @@
         request: alikafka_20190916_models.CreateAclRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.CreateAclResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.acl_operation_type):
             query['AclOperationType'] = request.acl_operation_type
+        if not UtilClient.is_unset(request.acl_operation_types):
+            query['AclOperationTypes'] = request.acl_operation_types
+        if not UtilClient.is_unset(request.acl_permission_type):
+            query['AclPermissionType'] = request.acl_permission_type
         if not UtilClient.is_unset(request.acl_resource_name):
             query['AclResourceName'] = request.acl_resource_name
         if not UtilClient.is_unset(request.acl_resource_pattern_type):
             query['AclResourcePatternType'] = request.acl_resource_pattern_type
         if not UtilClient.is_unset(request.acl_resource_type):
             query['AclResourceType'] = request.acl_resource_type
+        if not UtilClient.is_unset(request.host):
+            query['Host'] = request.host
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.username):
             query['Username'] = request.username
         req = open_api_models.OpenApiRequest(
@@ -686,14 +698,16 @@
         request: alikafka_20190916_models.CreateSaslUserRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.CreateSaslUserResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.mechanism):
+            query['Mechanism'] = request.mechanism
         if not UtilClient.is_unset(request.password):
             query['Password'] = request.password
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.type):
             query['Type'] = request.type
         if not UtilClient.is_unset(request.username):
@@ -722,14 +736,16 @@
         request: alikafka_20190916_models.CreateSaslUserRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.CreateSaslUserResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.mechanism):
+            query['Mechanism'] = request.mechanism
         if not UtilClient.is_unset(request.password):
             query['Password'] = request.password
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.type):
             query['Type'] = request.type
         if not UtilClient.is_unset(request.username):
@@ -912,20 +928,26 @@
         request: alikafka_20190916_models.DeleteAclRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.DeleteAclResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.acl_operation_type):
             query['AclOperationType'] = request.acl_operation_type
+        if not UtilClient.is_unset(request.acl_operation_types):
+            query['AclOperationTypes'] = request.acl_operation_types
+        if not UtilClient.is_unset(request.acl_permission_type):
+            query['AclPermissionType'] = request.acl_permission_type
         if not UtilClient.is_unset(request.acl_resource_name):
             query['AclResourceName'] = request.acl_resource_name
         if not UtilClient.is_unset(request.acl_resource_pattern_type):
             query['AclResourcePatternType'] = request.acl_resource_pattern_type
         if not UtilClient.is_unset(request.acl_resource_type):
             query['AclResourceType'] = request.acl_resource_type
+        if not UtilClient.is_unset(request.host):
+            query['Host'] = request.host
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.username):
             query['Username'] = request.username
         req = open_api_models.OpenApiRequest(
@@ -952,20 +974,26 @@
         request: alikafka_20190916_models.DeleteAclRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.DeleteAclResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.acl_operation_type):
             query['AclOperationType'] = request.acl_operation_type
+        if not UtilClient.is_unset(request.acl_operation_types):
+            query['AclOperationTypes'] = request.acl_operation_types
+        if not UtilClient.is_unset(request.acl_permission_type):
+            query['AclPermissionType'] = request.acl_permission_type
         if not UtilClient.is_unset(request.acl_resource_name):
             query['AclResourceName'] = request.acl_resource_name
         if not UtilClient.is_unset(request.acl_resource_pattern_type):
             query['AclResourcePatternType'] = request.acl_resource_pattern_type
         if not UtilClient.is_unset(request.acl_resource_type):
             query['AclResourceType'] = request.acl_resource_type
+        if not UtilClient.is_unset(request.host):
+            query['Host'] = request.host
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.username):
             query['Username'] = request.username
         req = open_api_models.OpenApiRequest(
@@ -1158,14 +1186,16 @@
         request: alikafka_20190916_models.DeleteSaslUserRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.DeleteSaslUserResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.mechanism):
+            query['Mechanism'] = request.mechanism
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.type):
             query['Type'] = request.type
         if not UtilClient.is_unset(request.username):
             query['Username'] = request.username
         req = open_api_models.OpenApiRequest(
@@ -1192,14 +1222,16 @@
         request: alikafka_20190916_models.DeleteSaslUserRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.DeleteSaslUserResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.mechanism):
+            query['Mechanism'] = request.mechanism
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.type):
             query['Type'] = request.type
         if not UtilClient.is_unset(request.username):
             query['Username'] = request.username
         req = open_api_models.OpenApiRequest(
@@ -1316,20 +1348,26 @@
     def describe_acls_with_options(
         self,
         request: alikafka_20190916_models.DescribeAclsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.DescribeAclsResponse:
         UtilClient.validate_model(request)
         query = {}
+        if not UtilClient.is_unset(request.acl_operation_type):
+            query['AclOperationType'] = request.acl_operation_type
+        if not UtilClient.is_unset(request.acl_permission_type):
+            query['AclPermissionType'] = request.acl_permission_type
         if not UtilClient.is_unset(request.acl_resource_name):
             query['AclResourceName'] = request.acl_resource_name
         if not UtilClient.is_unset(request.acl_resource_pattern_type):
             query['AclResourcePatternType'] = request.acl_resource_pattern_type
         if not UtilClient.is_unset(request.acl_resource_type):
             query['AclResourceType'] = request.acl_resource_type
+        if not UtilClient.is_unset(request.host):
+            query['Host'] = request.host
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.username):
             query['Username'] = request.username
         req = open_api_models.OpenApiRequest(
@@ -1354,20 +1392,26 @@
     async def describe_acls_with_options_async(
         self,
         request: alikafka_20190916_models.DescribeAclsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.DescribeAclsResponse:
         UtilClient.validate_model(request)
         query = {}
+        if not UtilClient.is_unset(request.acl_operation_type):
+            query['AclOperationType'] = request.acl_operation_type
+        if not UtilClient.is_unset(request.acl_permission_type):
+            query['AclPermissionType'] = request.acl_permission_type
         if not UtilClient.is_unset(request.acl_resource_name):
             query['AclResourceName'] = request.acl_resource_name
         if not UtilClient.is_unset(request.acl_resource_pattern_type):
             query['AclResourcePatternType'] = request.acl_resource_pattern_type
         if not UtilClient.is_unset(request.acl_resource_type):
             query['AclResourceType'] = request.acl_resource_type
+        if not UtilClient.is_unset(request.host):
+            query['Host'] = request.host
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.username):
             query['Username'] = request.username
         req = open_api_models.OpenApiRequest(
```

### Comparing `alibabacloud_alikafka20190916-2.6.2/alibabacloud_alikafka20190916/models.py` & `alibabacloud_alikafka20190916-2.6.3/alibabacloud_alikafka20190916/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -290,28 +290,33 @@
         return self
 
 
 class CreateAclRequest(TeaModel):
     def __init__(
         self,
         acl_operation_type: str = None,
+        acl_operation_types: str = None,
+        acl_permission_type: str = None,
         acl_resource_name: str = None,
         acl_resource_pattern_type: str = None,
         acl_resource_type: str = None,
+        host: str = None,
         instance_id: str = None,
         region_id: str = None,
         username: str = None,
     ):
         # The operation type. Valid values:
         # 
         # *   **Write**: data writes
         # *   **Read**: data reads
         # *   **Describe**: reads of transaction IDs****\
         # *   **IdempotentWrite**: idempotent data writes to clusters****\
         self.acl_operation_type = acl_operation_type
+        self.acl_operation_types = acl_operation_types
+        self.acl_permission_type = acl_permission_type
         # The name or ID of the resource.
         # 
         # *   The value can be the name of a topic, consumer group, or cluster, or the ID of a transaction.
         # *   You can use an asterisk (\*) to represent the names or IDs of all relevant resources.
         self.acl_resource_name = acl_resource_name
         # The matching mode. Valid values:
         # 
@@ -321,14 +326,15 @@
         # The resource type. Valid values:
         # 
         # *   **Topic**\
         # *   **Group**\
         # *   **Cluster**\
         # *   **TransactionalId**: transaction
         self.acl_resource_type = acl_resource_type
+        self.host = host
         # The instance ID.
         self.instance_id = instance_id
         # The region ID.
         self.region_id = region_id
         # The username.
         # 
         # You can use an asterisk (\*) to represent all usernames.
@@ -341,38 +347,50 @@
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.acl_operation_type is not None:
             result['AclOperationType'] = self.acl_operation_type
+        if self.acl_operation_types is not None:
+            result['AclOperationTypes'] = self.acl_operation_types
+        if self.acl_permission_type is not None:
+            result['AclPermissionType'] = self.acl_permission_type
         if self.acl_resource_name is not None:
             result['AclResourceName'] = self.acl_resource_name
         if self.acl_resource_pattern_type is not None:
             result['AclResourcePatternType'] = self.acl_resource_pattern_type
         if self.acl_resource_type is not None:
             result['AclResourceType'] = self.acl_resource_type
+        if self.host is not None:
+            result['Host'] = self.host
         if self.instance_id is not None:
             result['InstanceId'] = self.instance_id
         if self.region_id is not None:
             result['RegionId'] = self.region_id
         if self.username is not None:
             result['Username'] = self.username
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('AclOperationType') is not None:
             self.acl_operation_type = m.get('AclOperationType')
+        if m.get('AclOperationTypes') is not None:
+            self.acl_operation_types = m.get('AclOperationTypes')
+        if m.get('AclPermissionType') is not None:
+            self.acl_permission_type = m.get('AclPermissionType')
         if m.get('AclResourceName') is not None:
             self.acl_resource_name = m.get('AclResourceName')
         if m.get('AclResourcePatternType') is not None:
             self.acl_resource_pattern_type = m.get('AclResourcePatternType')
         if m.get('AclResourceType') is not None:
             self.acl_resource_type = m.get('AclResourceType')
+        if m.get('Host') is not None:
+            self.host = m.get('Host')
         if m.get('InstanceId') is not None:
             self.instance_id = m.get('InstanceId')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
         if m.get('Username') is not None:
             self.username = m.get('Username')
         return self
@@ -1599,21 +1617,23 @@
         return self
 
 
 class CreateSaslUserRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
+        mechanism: str = None,
         password: str = None,
         region_id: str = None,
         type: str = None,
         username: str = None,
     ):
         # The instance ID.
         self.instance_id = instance_id
+        self.mechanism = mechanism
         # The password of the SASL user.
         self.password = password
         # The region ID.
         self.region_id = region_id
         # The SASL mechanism. Valid values:
         # 
         # *   **plain**: a simple mechanism that uses usernames and passwords to verify user identities. Message Queue for Apache Kafka provides an optimized PLAIN mechanism that allows you to dynamically create SASL users for an instance without the need to restart the instance.
@@ -1631,28 +1651,32 @@
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.instance_id is not None:
             result['InstanceId'] = self.instance_id
+        if self.mechanism is not None:
+            result['Mechanism'] = self.mechanism
         if self.password is not None:
             result['Password'] = self.password
         if self.region_id is not None:
             result['RegionId'] = self.region_id
         if self.type is not None:
             result['Type'] = self.type
         if self.username is not None:
             result['Username'] = self.username
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('InstanceId') is not None:
             self.instance_id = m.get('InstanceId')
+        if m.get('Mechanism') is not None:
+            self.mechanism = m.get('Mechanism')
         if m.get('Password') is not None:
             self.password = m.get('Password')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
         if m.get('Type') is not None:
             self.type = m.get('Type')
         if m.get('Username') is not None:
@@ -2018,26 +2042,31 @@
         return self
 
 
 class DeleteAclRequest(TeaModel):
     def __init__(
         self,
         acl_operation_type: str = None,
+        acl_operation_types: str = None,
+        acl_permission_type: str = None,
         acl_resource_name: str = None,
         acl_resource_pattern_type: str = None,
         acl_resource_type: str = None,
+        host: str = None,
         instance_id: str = None,
         region_id: str = None,
         username: str = None,
     ):
         # The operation type. Valid values:
         # 
         # *   **Write**\
         # *   **Read**\
         self.acl_operation_type = acl_operation_type
+        self.acl_operation_types = acl_operation_types
+        self.acl_permission_type = acl_permission_type
         # The name of the resource.
         # 
         # *   The value can be the name of a topic or consumer group.
         # *   You can use an asterisk (\*) to indicate the names of all topics or consumer groups.
         self.acl_resource_name = acl_resource_name
         # The mode that is used to match resources. Valid values:
         # 
@@ -2045,14 +2074,15 @@
         # *   **PREFIXED**: prefix match
         self.acl_resource_pattern_type = acl_resource_pattern_type
         # The type of the resource.
         # 
         # *   **Topic**\
         # *   **Group**\
         self.acl_resource_type = acl_resource_type
+        self.host = host
         # The ID of the instance.
         self.instance_id = instance_id
         # The ID of the region.
         self.region_id = region_id
         # The name of the user.
         self.username = username
 
@@ -2063,38 +2093,50 @@
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.acl_operation_type is not None:
             result['AclOperationType'] = self.acl_operation_type
+        if self.acl_operation_types is not None:
+            result['AclOperationTypes'] = self.acl_operation_types
+        if self.acl_permission_type is not None:
+            result['AclPermissionType'] = self.acl_permission_type
         if self.acl_resource_name is not None:
             result['AclResourceName'] = self.acl_resource_name
         if self.acl_resource_pattern_type is not None:
             result['AclResourcePatternType'] = self.acl_resource_pattern_type
         if self.acl_resource_type is not None:
             result['AclResourceType'] = self.acl_resource_type
+        if self.host is not None:
+            result['Host'] = self.host
         if self.instance_id is not None:
             result['InstanceId'] = self.instance_id
         if self.region_id is not None:
             result['RegionId'] = self.region_id
         if self.username is not None:
             result['Username'] = self.username
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('AclOperationType') is not None:
             self.acl_operation_type = m.get('AclOperationType')
+        if m.get('AclOperationTypes') is not None:
+            self.acl_operation_types = m.get('AclOperationTypes')
+        if m.get('AclPermissionType') is not None:
+            self.acl_permission_type = m.get('AclPermissionType')
         if m.get('AclResourceName') is not None:
             self.acl_resource_name = m.get('AclResourceName')
         if m.get('AclResourcePatternType') is not None:
             self.acl_resource_pattern_type = m.get('AclResourcePatternType')
         if m.get('AclResourceType') is not None:
             self.acl_resource_type = m.get('AclResourceType')
+        if m.get('Host') is not None:
+            self.host = m.get('Host')
         if m.get('InstanceId') is not None:
             self.instance_id = m.get('InstanceId')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
         if m.get('Username') is not None:
             self.username = m.get('Username')
         return self
@@ -2447,20 +2489,22 @@
         return self
 
 
 class DeleteSaslUserRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
+        mechanism: str = None,
         region_id: str = None,
         type: str = None,
         username: str = None,
     ):
         # The ID of the instance.
         self.instance_id = instance_id
+        self.mechanism = mechanism
         # The ID of the region.
         self.region_id = region_id
         # The SASL mechanism. Valid values:
         # 
         # *   **plain**: a simple mechanism that uses usernames and passwords to verify user identities. Message Queue for Apache Kafka provides an optimized PLAIN mechanism that allows you to dynamically create SASL users for an instance without the need to restart the instance.
         # *   **scram**: a mechanism that uses usernames and passwords to verify user identities. This mechanism provides better security protection than the PLAIN mechanism. Message Queue for Apache Kafka uses SCRAM-SHA-256.
         # 
@@ -2476,26 +2520,30 @@
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.instance_id is not None:
             result['InstanceId'] = self.instance_id
+        if self.mechanism is not None:
+            result['Mechanism'] = self.mechanism
         if self.region_id is not None:
             result['RegionId'] = self.region_id
         if self.type is not None:
             result['Type'] = self.type
         if self.username is not None:
             result['Username'] = self.username
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('InstanceId') is not None:
             self.instance_id = m.get('InstanceId')
+        if m.get('Mechanism') is not None:
+            self.mechanism = m.get('Mechanism')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
         if m.get('Type') is not None:
             self.type = m.get('Type')
         if m.get('Username') is not None:
             self.username = m.get('Username')
         return self
@@ -2722,21 +2770,26 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeAclsRequest(TeaModel):
     def __init__(
         self,
+        acl_operation_type: str = None,
+        acl_permission_type: str = None,
         acl_resource_name: str = None,
         acl_resource_pattern_type: str = None,
         acl_resource_type: str = None,
+        host: str = None,
         instance_id: str = None,
         region_id: str = None,
         username: str = None,
     ):
+        self.acl_operation_type = acl_operation_type
+        self.acl_permission_type = acl_permission_type
         # The name or ID of the resource.
         # 
         # *   The value can be the name of a topic or a consumer group.
         # *   You can use an asterisk (\*) to represent the names of all topics or consumer groups.
         self.acl_resource_name = acl_resource_name
         # The match mode. Valid values:
         # 
@@ -2744,14 +2797,15 @@
         # *   PREFIXED: prefix match
         self.acl_resource_pattern_type = acl_resource_pattern_type
         # The resource type. Valid values:
         # 
         # *   **Topic**\
         # *   **Group**\
         self.acl_resource_type = acl_resource_type
+        self.host = host
         # The ID of the instance.
         self.instance_id = instance_id
         # The ID of the region.
         self.region_id = region_id
         # The name of the user.
         self.username = username
 
@@ -2760,60 +2814,74 @@
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.acl_operation_type is not None:
+            result['AclOperationType'] = self.acl_operation_type
+        if self.acl_permission_type is not None:
+            result['AclPermissionType'] = self.acl_permission_type
         if self.acl_resource_name is not None:
             result['AclResourceName'] = self.acl_resource_name
         if self.acl_resource_pattern_type is not None:
             result['AclResourcePatternType'] = self.acl_resource_pattern_type
         if self.acl_resource_type is not None:
             result['AclResourceType'] = self.acl_resource_type
+        if self.host is not None:
+            result['Host'] = self.host
         if self.instance_id is not None:
             result['InstanceId'] = self.instance_id
         if self.region_id is not None:
             result['RegionId'] = self.region_id
         if self.username is not None:
             result['Username'] = self.username
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('AclOperationType') is not None:
+            self.acl_operation_type = m.get('AclOperationType')
+        if m.get('AclPermissionType') is not None:
+            self.acl_permission_type = m.get('AclPermissionType')
         if m.get('AclResourceName') is not None:
             self.acl_resource_name = m.get('AclResourceName')
         if m.get('AclResourcePatternType') is not None:
             self.acl_resource_pattern_type = m.get('AclResourcePatternType')
         if m.get('AclResourceType') is not None:
             self.acl_resource_type = m.get('AclResourceType')
+        if m.get('Host') is not None:
+            self.host = m.get('Host')
         if m.get('InstanceId') is not None:
             self.instance_id = m.get('InstanceId')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
         if m.get('Username') is not None:
             self.username = m.get('Username')
         return self
 
 
 class DescribeAclsResponseBodyKafkaAclListKafkaAclVO(TeaModel):
     def __init__(
         self,
         acl_operation_type: str = None,
+        acl_permission_type: str = None,
         acl_resource_name: str = None,
         acl_resource_pattern_type: str = None,
         acl_resource_type: str = None,
         host: str = None,
         username: str = None,
     ):
         # The type of the operation. Valid values:
         # 
         # *   **Write**\
         # *   **Read**\
         self.acl_operation_type = acl_operation_type
+        self.acl_permission_type = acl_permission_type
         # The name of the resource.
         # 
         # *   The value can be the name of a topic or a consumer group.
         # *   An asterisk (\*) represents the names of all topics or consumer groups.
         self.acl_resource_name = acl_resource_name
         # The match mode. Valid values:
         # 
@@ -2837,14 +2905,16 @@
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.acl_operation_type is not None:
             result['AclOperationType'] = self.acl_operation_type
+        if self.acl_permission_type is not None:
+            result['AclPermissionType'] = self.acl_permission_type
         if self.acl_resource_name is not None:
             result['AclResourceName'] = self.acl_resource_name
         if self.acl_resource_pattern_type is not None:
             result['AclResourcePatternType'] = self.acl_resource_pattern_type
         if self.acl_resource_type is not None:
             result['AclResourceType'] = self.acl_resource_type
         if self.host is not None:
@@ -2853,14 +2923,16 @@
             result['Username'] = self.username
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('AclOperationType') is not None:
             self.acl_operation_type = m.get('AclOperationType')
+        if m.get('AclPermissionType') is not None:
+            self.acl_permission_type = m.get('AclPermissionType')
         if m.get('AclResourceName') is not None:
             self.acl_resource_name = m.get('AclResourceName')
         if m.get('AclResourcePatternType') is not None:
             self.acl_resource_pattern_type = m.get('AclResourcePatternType')
         if m.get('AclResourceType') is not None:
             self.acl_resource_type = m.get('AclResourceType')
         if m.get('Host') is not None:
@@ -3038,18 +3110,20 @@
             self.region_id = m.get('RegionId')
         return self
 
 
 class DescribeSaslUsersResponseBodySaslUserListSaslUserVO(TeaModel):
     def __init__(
         self,
+        mechanism: str = None,
         password: str = None,
         type: str = None,
         username: str = None,
     ):
+        self.mechanism = mechanism
         # The password that is used to access the Elasticsearch cluster.
         self.password = password
         # The request type. Valid values:
         # 
         # *   **plain**: a simple mechanism that uses usernames and passwords to verify user identities. Message Queue for Apache Kafka provides an optimized PLAIN mechanism that allows you to dynamically create SASL users for an instance without the need to restart the instance.
         # *   **scram**: a mechanism that uses usernames and passwords to verify user identities. This mechanism provides better security protection than the PLAIN mechanism. Message Queue for Apache Kafka uses SCRAM-SHA-256.
         # 
@@ -3063,24 +3137,28 @@
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.mechanism is not None:
+            result['Mechanism'] = self.mechanism
         if self.password is not None:
             result['Password'] = self.password
         if self.type is not None:
             result['Type'] = self.type
         if self.username is not None:
             result['Username'] = self.username
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('Mechanism') is not None:
+            self.mechanism = m.get('Mechanism')
         if m.get('Password') is not None:
             self.password = m.get('Password')
         if m.get('Type') is not None:
             self.type = m.get('Type')
         if m.get('Username') is not None:
             self.username = m.get('Username')
         return self
@@ -4294,14 +4372,106 @@
         if m.get('InstanceId') is not None:
             self.instance_id = m.get('InstanceId')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
         return self
 
 
+class GetConsumerProgressResponseBodyConsumerProgressRebalanceInfoListRebalanceInfoList(TeaModel):
+    def __init__(
+        self,
+        generation: int = None,
+        group_id: str = None,
+        last_rebalance_timestamp: int = None,
+        reason: str = None,
+        rebalance_success: bool = None,
+        rebalance_time_consuming: int = None,
+    ):
+        self.generation = generation
+        self.group_id = group_id
+        self.last_rebalance_timestamp = last_rebalance_timestamp
+        self.reason = reason
+        self.rebalance_success = rebalance_success
+        self.rebalance_time_consuming = rebalance_time_consuming
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.generation is not None:
+            result['Generation'] = self.generation
+        if self.group_id is not None:
+            result['GroupId'] = self.group_id
+        if self.last_rebalance_timestamp is not None:
+            result['LastRebalanceTimestamp'] = self.last_rebalance_timestamp
+        if self.reason is not None:
+            result['Reason'] = self.reason
+        if self.rebalance_success is not None:
+            result['RebalanceSuccess'] = self.rebalance_success
+        if self.rebalance_time_consuming is not None:
+            result['RebalanceTimeConsuming'] = self.rebalance_time_consuming
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Generation') is not None:
+            self.generation = m.get('Generation')
+        if m.get('GroupId') is not None:
+            self.group_id = m.get('GroupId')
+        if m.get('LastRebalanceTimestamp') is not None:
+            self.last_rebalance_timestamp = m.get('LastRebalanceTimestamp')
+        if m.get('Reason') is not None:
+            self.reason = m.get('Reason')
+        if m.get('RebalanceSuccess') is not None:
+            self.rebalance_success = m.get('RebalanceSuccess')
+        if m.get('RebalanceTimeConsuming') is not None:
+            self.rebalance_time_consuming = m.get('RebalanceTimeConsuming')
+        return self
+
+
+class GetConsumerProgressResponseBodyConsumerProgressRebalanceInfoList(TeaModel):
+    def __init__(
+        self,
+        rebalance_info_list: List[GetConsumerProgressResponseBodyConsumerProgressRebalanceInfoListRebalanceInfoList] = None,
+    ):
+        self.rebalance_info_list = rebalance_info_list
+
+    def validate(self):
+        if self.rebalance_info_list:
+            for k in self.rebalance_info_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['RebalanceInfoList'] = []
+        if self.rebalance_info_list is not None:
+            for k in self.rebalance_info_list:
+                result['RebalanceInfoList'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.rebalance_info_list = []
+        if m.get('RebalanceInfoList') is not None:
+            for k in m.get('RebalanceInfoList'):
+                temp_model = GetConsumerProgressResponseBodyConsumerProgressRebalanceInfoListRebalanceInfoList()
+                self.rebalance_info_list.append(temp_model.from_map(k))
+        return self
+
+
 class GetConsumerProgressResponseBodyConsumerProgressTopicListTopicListOffsetListOffsetList(TeaModel):
     def __init__(
         self,
         broker_offset: int = None,
         consumer_offset: int = None,
         last_timestamp: int = None,
         partition: int = None,
@@ -4468,46 +4638,55 @@
         return self
 
 
 class GetConsumerProgressResponseBodyConsumerProgress(TeaModel):
     def __init__(
         self,
         last_timestamp: int = None,
+        rebalance_info_list: GetConsumerProgressResponseBodyConsumerProgressRebalanceInfoList = None,
         topic_list: GetConsumerProgressResponseBodyConsumerProgressTopicList = None,
         total_diff: int = None,
     ):
         # The time when the last message consumed by the consumer group was generated.
         self.last_timestamp = last_timestamp
+        self.rebalance_info_list = rebalance_info_list
         # The consumption progress of each topic to which the consumer group is subscribed.
         self.topic_list = topic_list
         # The number of messages that were not consumed in all topics. This is also known as the number of accumulated messages in all topics.
         self.total_diff = total_diff
 
     def validate(self):
+        if self.rebalance_info_list:
+            self.rebalance_info_list.validate()
         if self.topic_list:
             self.topic_list.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.last_timestamp is not None:
             result['LastTimestamp'] = self.last_timestamp
+        if self.rebalance_info_list is not None:
+            result['RebalanceInfoList'] = self.rebalance_info_list.to_map()
         if self.topic_list is not None:
             result['TopicList'] = self.topic_list.to_map()
         if self.total_diff is not None:
             result['TotalDiff'] = self.total_diff
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('LastTimestamp') is not None:
             self.last_timestamp = m.get('LastTimestamp')
+        if m.get('RebalanceInfoList') is not None:
+            temp_model = GetConsumerProgressResponseBodyConsumerProgressRebalanceInfoList()
+            self.rebalance_info_list = temp_model.from_map(m['RebalanceInfoList'])
         if m.get('TopicList') is not None:
             temp_model = GetConsumerProgressResponseBodyConsumerProgressTopicList()
             self.topic_list = temp_model.from_map(m['TopicList'])
         if m.get('TotalDiff') is not None:
             self.total_diff = m.get('TotalDiff')
         return self
```

### Comparing `alibabacloud_alikafka20190916-2.6.2/alibabacloud_alikafka20190916.egg-info/PKG-INFO` & `alibabacloud_alikafka20190916-2.6.3/alibabacloud_alikafka20190916.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-alikafka20190916
-Version: 2.6.2
+Version: 2.6.3
 Summary: Alibaba Cloud MQ for Kafka (20190916) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_alikafka20190916-2.6.2/setup.py` & `alibabacloud_alikafka20190916-2.6.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_alikafka20190916.
 
-Created on 25/03/2024
+Created on 02/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_alikafka20190916"
 NAME = "alibabacloud_alikafka20190916" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud MQ for Kafka (20190916) SDK Library for Python"
```

