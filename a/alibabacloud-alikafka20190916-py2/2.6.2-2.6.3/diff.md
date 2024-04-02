# Comparing `tmp/alibabacloud_alikafka20190916_py2-2.6.2.tar.gz` & `tmp/alibabacloud_alikafka20190916_py2-2.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_alikafka20190916_py2-2.6.2.tar", last modified: Mon Mar 25 17:10:12 2024, max compression
+gzip compressed data, was "dist/alibabacloud_alikafka20190916_py2-2.6.3.tar", last modified: Tue Apr  2 17:13:35 2024, max compression
```

## Comparing `alibabacloud_alikafka20190916_py2-2.6.2.tar` & `alibabacloud_alikafka20190916_py2-2.6.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:10:12.000000 alibabacloud_alikafka20190916_py2-2.6.2/
--rw-r--r--   0 root         (0) root         (0)     5290 2024-03-25 17:10:11.000000 alibabacloud_alikafka20190916_py2-2.6.2/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2024-03-25 17:10:11.000000 alibabacloud_alikafka20190916_py2-2.6.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2024-03-25 17:10:11.000000 alibabacloud_alikafka20190916_py2-2.6.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2506 2024-03-25 17:10:12.000000 alibabacloud_alikafka20190916_py2-2.6.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1048 2024-03-25 17:10:11.000000 alibabacloud_alikafka20190916_py2-2.6.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1131 2024-03-25 17:10:11.000000 alibabacloud_alikafka20190916_py2-2.6.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:10:12.000000 alibabacloud_alikafka20190916_py2-2.6.2/alibabacloud_alikafka20190916/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-25 17:10:11.000000 alibabacloud_alikafka20190916_py2-2.6.2/alibabacloud_alikafka20190916/__init__.py
--rw-r--r--   0 root         (0) root         (0)    76051 2024-03-25 17:10:11.000000 alibabacloud_alikafka20190916_py2-2.6.2/alibabacloud_alikafka20190916/client.py
--rw-r--r--   0 root         (0) root         (0)   377937 2024-03-25 17:10:11.000000 alibabacloud_alikafka20190916_py2-2.6.2/alibabacloud_alikafka20190916/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 17:10:12.000000 alibabacloud_alikafka20190916_py2-2.6.2/alibabacloud_alikafka20190916_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2506 2024-03-25 17:10:12.000000 alibabacloud_alikafka20190916_py2-2.6.2/alibabacloud_alikafka20190916_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      480 2024-03-25 17:10:12.000000 alibabacloud_alikafka20190916_py2-2.6.2/alibabacloud_alikafka20190916_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-25 17:10:12.000000 alibabacloud_alikafka20190916_py2-2.6.2/alibabacloud_alikafka20190916_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2024-03-25 17:10:12.000000 alibabacloud_alikafka20190916_py2-2.6.2/alibabacloud_alikafka20190916_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2024-03-25 17:10:12.000000 alibabacloud_alikafka20190916_py2-2.6.2/alibabacloud_alikafka20190916_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-25 17:10:12.000000 alibabacloud_alikafka20190916_py2-2.6.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2932 2024-03-25 17:10:11.000000 alibabacloud_alikafka20190916_py2-2.6.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:13:35.000000 alibabacloud_alikafka20190916_py2-2.6.3/
+-rw-r--r--   0 root         (0) root         (0)     5371 2024-04-02 17:13:35.000000 alibabacloud_alikafka20190916_py2-2.6.3/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2024-04-02 17:13:35.000000 alibabacloud_alikafka20190916_py2-2.6.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-02 17:13:35.000000 alibabacloud_alikafka20190916_py2-2.6.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2506 2024-04-02 17:13:35.000000 alibabacloud_alikafka20190916_py2-2.6.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1048 2024-04-02 17:13:35.000000 alibabacloud_alikafka20190916_py2-2.6.3/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1131 2024-04-02 17:13:35.000000 alibabacloud_alikafka20190916_py2-2.6.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:13:35.000000 alibabacloud_alikafka20190916_py2-2.6.3/alibabacloud_alikafka20190916/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-02 17:13:35.000000 alibabacloud_alikafka20190916_py2-2.6.3/alibabacloud_alikafka20190916/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    77337 2024-04-02 17:13:35.000000 alibabacloud_alikafka20190916_py2-2.6.3/alibabacloud_alikafka20190916/client.py
+-rw-r--r--   0 root         (0) root         (0)   385713 2024-04-02 17:13:35.000000 alibabacloud_alikafka20190916_py2-2.6.3/alibabacloud_alikafka20190916/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:13:35.000000 alibabacloud_alikafka20190916_py2-2.6.3/alibabacloud_alikafka20190916_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2506 2024-04-02 17:13:35.000000 alibabacloud_alikafka20190916_py2-2.6.3/alibabacloud_alikafka20190916_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      480 2024-04-02 17:13:35.000000 alibabacloud_alikafka20190916_py2-2.6.3/alibabacloud_alikafka20190916_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-02 17:13:35.000000 alibabacloud_alikafka20190916_py2-2.6.3/alibabacloud_alikafka20190916_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2024-04-02 17:13:35.000000 alibabacloud_alikafka20190916_py2-2.6.3/alibabacloud_alikafka20190916_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2024-04-02 17:13:35.000000 alibabacloud_alikafka20190916_py2-2.6.3/alibabacloud_alikafka20190916_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-02 17:13:35.000000 alibabacloud_alikafka20190916_py2-2.6.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2932 2024-04-02 17:13:35.000000 alibabacloud_alikafka20190916_py2-2.6.3/setup.py
```

### Comparing `alibabacloud_alikafka20190916_py2-2.6.2/ChangeLog.md` & `alibabacloud_alikafka20190916_py2-2.6.3/ChangeLog.md`

 * *Files 0% similar despite different names*

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

### Comparing `alibabacloud_alikafka20190916_py2-2.6.2/LICENSE` & `alibabacloud_alikafka20190916_py2-2.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_alikafka20190916_py2-2.6.2/PKG-INFO` & `alibabacloud_alikafka20190916_py2-2.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_alikafka20190916_py2
-Version: 2.6.2
+Version: 2.6.3
 Summary: Alibaba Cloud MQ for Kafka (20190916) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_alikafka20190916_py2-2.6.2/README-CN.md` & `alibabacloud_alikafka20190916_py2-2.6.3/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_alikafka20190916_py2-2.6.2/README.md` & `alibabacloud_alikafka20190916_py2-2.6.3/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_alikafka20190916_py2-2.6.2/alibabacloud_alikafka20190916/client.py` & `alibabacloud_alikafka20190916_py2-2.6.3/alibabacloud_alikafka20190916/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,20 +95,26 @@
         return self.convert_post_pay_order_with_options(request, runtime)
 
     def create_acl_with_options(self, request, runtime):
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
@@ -319,14 +325,16 @@
         return self.create_pre_pay_order_with_options(request, runtime)
 
     def create_sasl_user_with_options(self, request, runtime):
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
@@ -423,20 +431,26 @@
         return self.create_topic_with_options(request, runtime)
 
     def delete_acl_with_options(self, request, runtime):
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
@@ -525,14 +539,16 @@
         return self.delete_instance_with_options(request, runtime)
 
     def delete_sasl_user_with_options(self, request, runtime):
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
@@ -589,20 +605,26 @@
     def delete_topic(self, request):
         runtime = util_models.RuntimeOptions()
         return self.delete_topic_with_options(request, runtime)
 
     def describe_acls_with_options(self, request, runtime):
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

### Comparing `alibabacloud_alikafka20190916_py2-2.6.2/alibabacloud_alikafka20190916/models.py` & `alibabacloud_alikafka20190916_py2-2.6.3/alibabacloud_alikafka20190916/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -252,23 +252,26 @@
         if m.get('body') is not None:
             temp_model = ConvertPostPayOrderResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateAclRequest(TeaModel):
-    def __init__(self, acl_operation_type=None, acl_resource_name=None, acl_resource_pattern_type=None,
-                 acl_resource_type=None, instance_id=None, region_id=None, username=None):
+    def __init__(self, acl_operation_type=None, acl_operation_types=None, acl_permission_type=None,
+                 acl_resource_name=None, acl_resource_pattern_type=None, acl_resource_type=None, host=None, instance_id=None,
+                 region_id=None, username=None):
         # The operation type. Valid values:
         # 
         # *   **Write**: data writes
         # *   **Read**: data reads
         # *   **Describe**: reads of transaction IDs****\
         # *   **IdempotentWrite**: idempotent data writes to clusters****\
         self.acl_operation_type = acl_operation_type  # type: str
+        self.acl_operation_types = acl_operation_types  # type: str
+        self.acl_permission_type = acl_permission_type  # type: str
         # The name or ID of the resource.
         # 
         # *   The value can be the name of a topic, consumer group, or cluster, or the ID of a transaction.
         # *   You can use an asterisk (\*) to represent the names or IDs of all relevant resources.
         self.acl_resource_name = acl_resource_name  # type: str
         # The matching mode. Valid values:
         # 
@@ -278,14 +281,15 @@
         # The resource type. Valid values:
         # 
         # *   **Topic**\
         # *   **Group**\
         # *   **Cluster**\
         # *   **TransactionalId**: transaction
         self.acl_resource_type = acl_resource_type  # type: str
+        self.host = host  # type: str
         # The instance ID.
         self.instance_id = instance_id  # type: str
         # The region ID.
         self.region_id = region_id  # type: str
         # The username.
         # 
         # You can use an asterisk (\*) to represent all usernames.
@@ -298,38 +302,50 @@
         _map = super(CreateAclRequest, self).to_map()
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
 
     def from_map(self, m=None):
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
@@ -1424,17 +1440,18 @@
         if m.get('body') is not None:
             temp_model = CreatePrePayOrderResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateSaslUserRequest(TeaModel):
-    def __init__(self, instance_id=None, password=None, region_id=None, type=None, username=None):
+    def __init__(self, instance_id=None, mechanism=None, password=None, region_id=None, type=None, username=None):
         # The instance ID.
         self.instance_id = instance_id  # type: str
+        self.mechanism = mechanism  # type: str
         # The password of the SASL user.
         self.password = password  # type: str
         # The region ID.
         self.region_id = region_id  # type: str
         # The SASL mechanism. Valid values:
         # 
         # *   **plain**: a simple mechanism that uses usernames and passwords to verify user identities. Message Queue for Apache Kafka provides an optimized PLAIN mechanism that allows you to dynamically create SASL users for an instance without the need to restart the instance.
@@ -1452,28 +1469,32 @@
         _map = super(CreateSaslUserRequest, self).to_map()
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
 
     def from_map(self, m=None):
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
@@ -1799,21 +1820,24 @@
         if m.get('body') is not None:
             temp_model = CreateTopicResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DeleteAclRequest(TeaModel):
-    def __init__(self, acl_operation_type=None, acl_resource_name=None, acl_resource_pattern_type=None,
-                 acl_resource_type=None, instance_id=None, region_id=None, username=None):
+    def __init__(self, acl_operation_type=None, acl_operation_types=None, acl_permission_type=None,
+                 acl_resource_name=None, acl_resource_pattern_type=None, acl_resource_type=None, host=None, instance_id=None,
+                 region_id=None, username=None):
         # The operation type. Valid values:
         # 
         # *   **Write**\
         # *   **Read**\
         self.acl_operation_type = acl_operation_type  # type: str
+        self.acl_operation_types = acl_operation_types  # type: str
+        self.acl_permission_type = acl_permission_type  # type: str
         # The name of the resource.
         # 
         # *   The value can be the name of a topic or consumer group.
         # *   You can use an asterisk (\*) to indicate the names of all topics or consumer groups.
         self.acl_resource_name = acl_resource_name  # type: str
         # The mode that is used to match resources. Valid values:
         # 
@@ -1821,14 +1845,15 @@
         # *   **PREFIXED**: prefix match
         self.acl_resource_pattern_type = acl_resource_pattern_type  # type: str
         # The type of the resource.
         # 
         # *   **Topic**\
         # *   **Group**\
         self.acl_resource_type = acl_resource_type  # type: str
+        self.host = host  # type: str
         # The ID of the instance.
         self.instance_id = instance_id  # type: str
         # The ID of the region.
         self.region_id = region_id  # type: str
         # The name of the user.
         self.username = username  # type: str
 
@@ -1839,38 +1864,50 @@
         _map = super(DeleteAclRequest, self).to_map()
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
 
     def from_map(self, m=None):
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
@@ -2178,17 +2215,18 @@
         if m.get('body') is not None:
             temp_model = DeleteInstanceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DeleteSaslUserRequest(TeaModel):
-    def __init__(self, instance_id=None, region_id=None, type=None, username=None):
+    def __init__(self, instance_id=None, mechanism=None, region_id=None, type=None, username=None):
         # The ID of the instance.
         self.instance_id = instance_id  # type: str
+        self.mechanism = mechanism  # type: str
         # The ID of the region.
         self.region_id = region_id  # type: str
         # The SASL mechanism. Valid values:
         # 
         # *   **plain**: a simple mechanism that uses usernames and passwords to verify user identities. Message Queue for Apache Kafka provides an optimized PLAIN mechanism that allows you to dynamically create SASL users for an instance without the need to restart the instance.
         # *   **scram**: a mechanism that uses usernames and passwords to verify user identities. This mechanism provides better security protection than the PLAIN mechanism. Message Queue for Apache Kafka uses SCRAM-SHA-256.
         # 
@@ -2204,26 +2242,30 @@
         _map = super(DeleteSaslUserRequest, self).to_map()
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
 
     def from_map(self, m=None):
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
@@ -2421,16 +2463,18 @@
         if m.get('body') is not None:
             temp_model = DeleteTopicResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeAclsRequest(TeaModel):
-    def __init__(self, acl_resource_name=None, acl_resource_pattern_type=None, acl_resource_type=None,
-                 instance_id=None, region_id=None, username=None):
+    def __init__(self, acl_operation_type=None, acl_permission_type=None, acl_resource_name=None,
+                 acl_resource_pattern_type=None, acl_resource_type=None, host=None, instance_id=None, region_id=None, username=None):
+        self.acl_operation_type = acl_operation_type  # type: str
+        self.acl_permission_type = acl_permission_type  # type: str
         # The name or ID of the resource.
         # 
         # *   The value can be the name of a topic or a consumer group.
         # *   You can use an asterisk (\*) to represent the names of all topics or consumer groups.
         self.acl_resource_name = acl_resource_name  # type: str
         # The match mode. Valid values:
         # 
@@ -2438,14 +2482,15 @@
         # *   PREFIXED: prefix match
         self.acl_resource_pattern_type = acl_resource_pattern_type  # type: str
         # The resource type. Valid values:
         # 
         # *   **Topic**\
         # *   **Group**\
         self.acl_resource_type = acl_resource_type  # type: str
+        self.host = host  # type: str
         # The ID of the instance.
         self.instance_id = instance_id  # type: str
         # The ID of the region.
         self.region_id = region_id  # type: str
         # The name of the user.
         self.username = username  # type: str
 
@@ -2454,53 +2499,66 @@
 
     def to_map(self):
         _map = super(DescribeAclsRequest, self).to_map()
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
 
     def from_map(self, m=None):
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
-    def __init__(self, acl_operation_type=None, acl_resource_name=None, acl_resource_pattern_type=None,
-                 acl_resource_type=None, host=None, username=None):
+    def __init__(self, acl_operation_type=None, acl_permission_type=None, acl_resource_name=None,
+                 acl_resource_pattern_type=None, acl_resource_type=None, host=None, username=None):
         # The type of the operation. Valid values:
         # 
         # *   **Write**\
         # *   **Read**\
         self.acl_operation_type = acl_operation_type  # type: str
+        self.acl_permission_type = acl_permission_type  # type: str
         # The name of the resource.
         # 
         # *   The value can be the name of a topic or a consumer group.
         # *   An asterisk (\*) represents the names of all topics or consumer groups.
         self.acl_resource_name = acl_resource_name  # type: str
         # The match mode. Valid values:
         # 
@@ -2524,14 +2582,16 @@
         _map = super(DescribeAclsResponseBodyKafkaAclListKafkaAclVO, self).to_map()
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
@@ -2540,14 +2600,16 @@
             result['Username'] = self.username
         return result
 
     def from_map(self, m=None):
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
@@ -2704,15 +2766,16 @@
             self.instance_id = m.get('InstanceId')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
         return self
 
 
 class DescribeSaslUsersResponseBodySaslUserListSaslUserVO(TeaModel):
-    def __init__(self, password=None, type=None, username=None):
+    def __init__(self, mechanism=None, password=None, type=None, username=None):
+        self.mechanism = mechanism  # type: str
         # The password that is used to access the Elasticsearch cluster.
         self.password = password  # type: str
         # The request type. Valid values:
         # 
         # *   **plain**: a simple mechanism that uses usernames and passwords to verify user identities. Message Queue for Apache Kafka provides an optimized PLAIN mechanism that allows you to dynamically create SASL users for an instance without the need to restart the instance.
         # *   **scram**: a mechanism that uses usernames and passwords to verify user identities. This mechanism provides better security protection than the PLAIN mechanism. Message Queue for Apache Kafka uses SCRAM-SHA-256.
         # 
@@ -2726,24 +2789,28 @@
 
     def to_map(self):
         _map = super(DescribeSaslUsersResponseBodySaslUserListSaslUserVO, self).to_map()
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
 
     def from_map(self, m=None):
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
@@ -3820,14 +3887,96 @@
         if m.get('InstanceId') is not None:
             self.instance_id = m.get('InstanceId')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
         return self
 
 
+class GetConsumerProgressResponseBodyConsumerProgressRebalanceInfoListRebalanceInfoList(TeaModel):
+    def __init__(self, generation=None, group_id=None, last_rebalance_timestamp=None, reason=None,
+                 rebalance_success=None, rebalance_time_consuming=None):
+        self.generation = generation  # type: long
+        self.group_id = group_id  # type: str
+        self.last_rebalance_timestamp = last_rebalance_timestamp  # type: long
+        self.reason = reason  # type: str
+        self.rebalance_success = rebalance_success  # type: bool
+        self.rebalance_time_consuming = rebalance_time_consuming  # type: long
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GetConsumerProgressResponseBodyConsumerProgressRebalanceInfoListRebalanceInfoList, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, rebalance_info_list=None):
+        self.rebalance_info_list = rebalance_info_list  # type: list[GetConsumerProgressResponseBodyConsumerProgressRebalanceInfoListRebalanceInfoList]
+
+    def validate(self):
+        if self.rebalance_info_list:
+            for k in self.rebalance_info_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(GetConsumerProgressResponseBodyConsumerProgressRebalanceInfoList, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, broker_offset=None, consumer_offset=None, last_timestamp=None, partition=None):
         # The latest offset in the partition of the topic.
         self.broker_offset = broker_offset  # type: long
         # The consumer offset in the partition of the topic.
         self.consumer_offset = consumer_offset  # type: long
         # The time when the last consumed message in the partition was generated.
@@ -3973,44 +4122,52 @@
             for k in m.get('TopicList'):
                 temp_model = GetConsumerProgressResponseBodyConsumerProgressTopicListTopicList()
                 self.topic_list.append(temp_model.from_map(k))
         return self
 
 
 class GetConsumerProgressResponseBodyConsumerProgress(TeaModel):
-    def __init__(self, last_timestamp=None, topic_list=None, total_diff=None):
+    def __init__(self, last_timestamp=None, rebalance_info_list=None, topic_list=None, total_diff=None):
         # The time when the last message consumed by the consumer group was generated.
         self.last_timestamp = last_timestamp  # type: long
+        self.rebalance_info_list = rebalance_info_list  # type: GetConsumerProgressResponseBodyConsumerProgressRebalanceInfoList
         # The consumption progress of each topic to which the consumer group is subscribed.
         self.topic_list = topic_list  # type: GetConsumerProgressResponseBodyConsumerProgressTopicList
         # The number of messages that were not consumed in all topics. This is also known as the number of accumulated messages in all topics.
         self.total_diff = total_diff  # type: long
 
     def validate(self):
+        if self.rebalance_info_list:
+            self.rebalance_info_list.validate()
         if self.topic_list:
             self.topic_list.validate()
 
     def to_map(self):
         _map = super(GetConsumerProgressResponseBodyConsumerProgress, self).to_map()
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
 
     def from_map(self, m=None):
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

### Comparing `alibabacloud_alikafka20190916_py2-2.6.2/alibabacloud_alikafka20190916_py2.egg-info/PKG-INFO` & `alibabacloud_alikafka20190916_py2-2.6.3/alibabacloud_alikafka20190916_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-alikafka20190916-py2
-Version: 2.6.2
+Version: 2.6.3
 Summary: Alibaba Cloud MQ for Kafka (20190916) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_alikafka20190916_py2-2.6.2/setup.py` & `alibabacloud_alikafka20190916_py2-2.6.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_alikafka20190916_py2.
 
-Created on 25/03/2024
+Created on 02/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_alikafka20190916"
 NAME = "alibabacloud_alikafka20190916_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud MQ for Kafka (20190916) SDK Library for Python2"
```

