# Comparing `tmp/cdklabs.cdk-verified-permissions-0.0.1a3.tar.gz` & `tmp/cdklabs.cdk-verified-permissions-0.0.1a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdklabs.cdk-verified-permissions-0.0.1a3.tar", last modified: Fri Mar 22 10:46:12 2024, max compression
+gzip compressed data, was "cdklabs.cdk-verified-permissions-0.0.1a4.tar", last modified: Tue Apr  2 06:54:24 2024, max compression
```

## Comparing `cdklabs.cdk-verified-permissions-0.0.1a3.tar` & `cdklabs.cdk-verified-permissions-0.0.1a4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 10:46:12.694956 cdklabs.cdk-verified-permissions-0.0.1a3/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-03-22 10:46:00.000000 cdklabs.cdk-verified-permissions-0.0.1a3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-22 10:46:00.000000 cdklabs.cdk-verified-permissions-0.0.1a3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-22 10:46:00.000000 cdklabs.cdk-verified-permissions-0.0.1a3/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     7803 2024-03-22 10:46:12.694956 cdklabs.cdk-verified-permissions-0.0.1a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6836 2024-03-22 10:46:00.000000 cdklabs.cdk-verified-permissions-0.0.1a3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-22 10:46:00.000000 cdklabs.cdk-verified-permissions-0.0.1a3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 10:46:12.694956 cdklabs.cdk-verified-permissions-0.0.1a3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-03-22 10:46:00.000000 cdklabs.cdk-verified-permissions-0.0.1a3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 10:46:12.690956 cdklabs.cdk-verified-permissions-0.0.1a3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 10:46:12.690956 cdklabs.cdk-verified-permissions-0.0.1a3/src/cdklabs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 10:46:12.694956 cdklabs.cdk-verified-permissions-0.0.1a3/src/cdklabs/cdk_verified_permissions/
--rw-r--r--   0 runner    (1001) docker     (127)   105864 2024-03-22 10:46:00.000000 cdklabs.cdk-verified-permissions-0.0.1a3/src/cdklabs/cdk_verified_permissions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 10:46:12.694956 cdklabs.cdk-verified-permissions-0.0.1a3/src/cdklabs/cdk_verified_permissions/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-22 10:46:00.000000 cdklabs.cdk-verified-permissions-0.0.1a3/src/cdklabs/cdk_verified_permissions/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    54410 2024-03-22 10:46:00.000000 cdklabs.cdk-verified-permissions-0.0.1a3/src/cdklabs/cdk_verified_permissions/_jsii/cdk-verified-permissions@0.0.1-alpha.3.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 10:46:00.000000 cdklabs.cdk-verified-permissions-0.0.1a3/src/cdklabs/cdk_verified_permissions/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 10:46:12.694956 cdklabs.cdk-verified-permissions-0.0.1a3/src/cdklabs.cdk_verified_permissions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7803 2024-03-22 10:46:12.000000 cdklabs.cdk-verified-permissions-0.0.1a3/src/cdklabs.cdk_verified_permissions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-03-22 10:46:12.000000 cdklabs.cdk-verified-permissions-0.0.1a3/src/cdklabs.cdk_verified_permissions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 10:46:12.000000 cdklabs.cdk-verified-permissions-0.0.1a3/src/cdklabs.cdk_verified_permissions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-22 10:46:12.000000 cdklabs.cdk-verified-permissions-0.0.1a3/src/cdklabs.cdk_verified_permissions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-22 10:46:12.000000 cdklabs.cdk-verified-permissions-0.0.1a3/src/cdklabs.cdk_verified_permissions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:54:24.020632 cdklabs.cdk-verified-permissions-0.0.1a4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-02 06:54:13.000000 cdklabs.cdk-verified-permissions-0.0.1a4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-02 06:54:13.000000 cdklabs.cdk-verified-permissions-0.0.1a4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-02 06:54:13.000000 cdklabs.cdk-verified-permissions-0.0.1a4/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-04-02 06:54:24.020632 cdklabs.cdk-verified-permissions-0.0.1a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7568 2024-04-02 06:54:13.000000 cdklabs.cdk-verified-permissions-0.0.1a4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-02 06:54:13.000000 cdklabs.cdk-verified-permissions-0.0.1a4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 06:54:24.020632 cdklabs.cdk-verified-permissions-0.0.1a4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-02 06:54:13.000000 cdklabs.cdk-verified-permissions-0.0.1a4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:54:24.020632 cdklabs.cdk-verified-permissions-0.0.1a4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:54:24.020632 cdklabs.cdk-verified-permissions-0.0.1a4/src/cdklabs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:54:24.020632 cdklabs.cdk-verified-permissions-0.0.1a4/src/cdklabs/cdk_verified_permissions/
+-rw-r--r--   0 runner    (1001) docker     (127)   107624 2024-04-02 06:54:13.000000 cdklabs.cdk-verified-permissions-0.0.1a4/src/cdklabs/cdk_verified_permissions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:54:24.020632 cdklabs.cdk-verified-permissions-0.0.1a4/src/cdklabs/cdk_verified_permissions/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-02 06:54:13.000000 cdklabs.cdk-verified-permissions-0.0.1a4/src/cdklabs/cdk_verified_permissions/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55487 2024-04-02 06:54:13.000000 cdklabs.cdk-verified-permissions-0.0.1a4/src/cdklabs/cdk_verified_permissions/_jsii/cdk-verified-permissions@0.0.1-alpha.4.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 06:54:13.000000 cdklabs.cdk-verified-permissions-0.0.1a4/src/cdklabs/cdk_verified_permissions/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:54:24.020632 cdklabs.cdk-verified-permissions-0.0.1a4/src/cdklabs.cdk_verified_permissions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-04-02 06:54:23.000000 cdklabs.cdk-verified-permissions-0.0.1a4/src/cdklabs.cdk_verified_permissions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-02 06:54:23.000000 cdklabs.cdk-verified-permissions-0.0.1a4/src/cdklabs.cdk_verified_permissions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 06:54:23.000000 cdklabs.cdk-verified-permissions-0.0.1a4/src/cdklabs.cdk_verified_permissions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-02 06:54:23.000000 cdklabs.cdk-verified-permissions-0.0.1a4/src/cdklabs.cdk_verified_permissions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-02 06:54:23.000000 cdklabs.cdk-verified-permissions-0.0.1a4/src/cdklabs.cdk_verified_permissions.egg-info/top_level.txt
```

### Comparing `cdklabs.cdk-verified-permissions-0.0.1a3/LICENSE` & `cdklabs.cdk-verified-permissions-0.0.1a4/LICENSE`

 * *Files identical despite different names*

### Comparing `cdklabs.cdk-verified-permissions-0.0.1a3/PKG-INFO` & `cdklabs.cdk-verified-permissions-0.0.1a4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdklabs.cdk-verified-permissions
-Version: 0.0.1a3
+Version: 0.0.1a4
 Summary: L2 AWS CDK Constructs for Amazon Verified Permissions
 Home-page: https://github.com/cdklabs/cdk-verified-permissions.git
 Author: Amazon Web Services<aws-cdk-dev@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-verified-permissions.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -30,15 +30,15 @@
 
 This construct is still versioned with alpha/v0 major version and we could introduce breaking changes even without a major version bump. Our goal is to keep the API stable & backwards compatible as much as possible but we currently cannot guarantee that. Once we'll publish v1.0.0 the breaking changes will be introduced via major version bumps.
 
 # Getting Started
 
 ## Policy Store
 
-Define a Policy Store with defaults (No schema & Validation Settings Mode set to OFF):
+Define a Policy Store with defaults (No description, No schema & Validation Settings Mode set to OFF):
 
 ```python
 test = PolicyStore(scope, "PolicyStore")
 ```
 
 Define a Policy Store without Schema definition (Validation Settings Mode must be set to OFF):
 
@@ -47,15 +47,15 @@
     "mode": ValidationSettingsMode.OFF
 }
 test = PolicyStore(scope, "PolicyStore",
     validation_settings=validation_settings_off
 )
 ```
 
-Define a Policy Store with Schema definition (a STRICT Validation Settings Mode is strongly suggested for Policy Stores with schemas):
+Define a Policy Store with Description and Schema definition (a STRICT Validation Settings Mode is strongly suggested for Policy Stores with schemas):
 
 ```python
 validation_settings_strict = {
     "mode": ValidationSettingsMode.STRICT
 }
 cedar_json_schema = {
     "PhotoApp": {
@@ -74,15 +74,16 @@
     }
 }
 cedar_schema = {
     "cedar_json": JSON.stringify(cedar_json_schema)
 }
 policy_store = PolicyStore(scope, "PolicyStore",
     schema=cedar_schema,
-    validation_settings=validation_settings_strict
+    validation_settings=validation_settings_strict,
+    description="PolicyStore description"
 )
 ```
 
 Define a Policy Store with Schema definition from file:
 
 ```python
 validation_settings_strict = {
@@ -99,20 +100,47 @@
 
 ## Identity Source
 
 Define Identity Source with required properties:
 
 ```python
 user_pool = UserPool(scope, "UserPool") # Creating a new Cognito UserPool
+validation_settings_strict = {
+    "mode": ValidationSettingsMode.STRICT
+}
+cedar_json_schema = {
+    "PhotoApp": {
+        "entity_types": {
+            "User": {},
+            "Photo": {}
+        },
+        "actions": {
+            "view_photo": {
+                "applies_to": {
+                    "principal_types": ["User"],
+                    "resource_types": ["Photo"]
+                }
+            }
+        }
+    }
+}
+cedar_schema = {
+    "cedar_json": JSON.stringify(cedar_json_schema)
+}
+policy_store = PolicyStore(scope, "PolicyStore",
+    schema=cedar_schema,
+    validation_settings=validation_settings_strict
+)
 IdentitySource(scope, "IdentitySource",
     configuration=IdentitySourceConfiguration(
         cognito_user_pool_configuration=CognitoUserPoolConfiguration(
             user_pool=user_pool
         )
-    )
+    ),
+    policy_store=policy_store
 )
 ```
 
 Define Identity Source with all the properties:
 
 ```python
 validation_settings_strict = {
```

### Comparing `cdklabs.cdk-verified-permissions-0.0.1a3/README.md` & `cdklabs.cdk-verified-permissions-0.0.1a4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 This construct is still versioned with alpha/v0 major version and we could introduce breaking changes even without a major version bump. Our goal is to keep the API stable & backwards compatible as much as possible but we currently cannot guarantee that. Once we'll publish v1.0.0 the breaking changes will be introduced via major version bumps.
 
 # Getting Started
 
 ## Policy Store
 
-Define a Policy Store with defaults (No schema & Validation Settings Mode set to OFF):
+Define a Policy Store with defaults (No description, No schema & Validation Settings Mode set to OFF):
 
 ```python
 test = PolicyStore(scope, "PolicyStore")
 ```
 
 Define a Policy Store without Schema definition (Validation Settings Mode must be set to OFF):
 
@@ -23,15 +23,15 @@
     "mode": ValidationSettingsMode.OFF
 }
 test = PolicyStore(scope, "PolicyStore",
     validation_settings=validation_settings_off
 )
 ```
 
-Define a Policy Store with Schema definition (a STRICT Validation Settings Mode is strongly suggested for Policy Stores with schemas):
+Define a Policy Store with Description and Schema definition (a STRICT Validation Settings Mode is strongly suggested for Policy Stores with schemas):
 
 ```python
 validation_settings_strict = {
     "mode": ValidationSettingsMode.STRICT
 }
 cedar_json_schema = {
     "PhotoApp": {
@@ -50,15 +50,16 @@
     }
 }
 cedar_schema = {
     "cedar_json": JSON.stringify(cedar_json_schema)
 }
 policy_store = PolicyStore(scope, "PolicyStore",
     schema=cedar_schema,
-    validation_settings=validation_settings_strict
+    validation_settings=validation_settings_strict,
+    description="PolicyStore description"
 )
 ```
 
 Define a Policy Store with Schema definition from file:
 
 ```python
 validation_settings_strict = {
@@ -75,20 +76,47 @@
 
 ## Identity Source
 
 Define Identity Source with required properties:
 
 ```python
 user_pool = UserPool(scope, "UserPool") # Creating a new Cognito UserPool
+validation_settings_strict = {
+    "mode": ValidationSettingsMode.STRICT
+}
+cedar_json_schema = {
+    "PhotoApp": {
+        "entity_types": {
+            "User": {},
+            "Photo": {}
+        },
+        "actions": {
+            "view_photo": {
+                "applies_to": {
+                    "principal_types": ["User"],
+                    "resource_types": ["Photo"]
+                }
+            }
+        }
+    }
+}
+cedar_schema = {
+    "cedar_json": JSON.stringify(cedar_json_schema)
+}
+policy_store = PolicyStore(scope, "PolicyStore",
+    schema=cedar_schema,
+    validation_settings=validation_settings_strict
+)
 IdentitySource(scope, "IdentitySource",
     configuration=IdentitySourceConfiguration(
         cognito_user_pool_configuration=CognitoUserPoolConfiguration(
             user_pool=user_pool
         )
-    )
+    ),
+    policy_store=policy_store
 )
 ```
 
 Define Identity Source with all the properties:
 
 ```python
 validation_settings_strict = {
```

### Comparing `cdklabs.cdk-verified-permissions-0.0.1a3/setup.py` & `cdklabs.cdk-verified-permissions-0.0.1a4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdklabs.cdk-verified-permissions",
-    "version": "0.0.1.a3",
+    "version": "0.0.1.a4",
     "description": "L2 AWS CDK Constructs for Amazon Verified Permissions",
     "license": "Apache-2.0",
     "url": "https://github.com/cdklabs/cdk-verified-permissions.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services<aws-cdk-dev@amazon.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,25 +22,25 @@
     },
     "packages": [
         "cdklabs.cdk_verified_permissions",
         "cdklabs.cdk_verified_permissions._jsii"
     ],
     "package_data": {
         "cdklabs.cdk_verified_permissions._jsii": [
-            "cdk-verified-permissions@0.0.1-alpha.3.jsii.tgz"
+            "cdk-verified-permissions@0.0.1-alpha.4.jsii.tgz"
         ],
         "cdklabs.cdk_verified_permissions": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
-        "aws-cdk-lib>=2.92.0, <3.0.0",
+        "aws-cdk-lib>=2.134.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "jsii>=1.95.0, <2.0.0",
+        "jsii>=1.96.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `cdklabs.cdk-verified-permissions-0.0.1a3/src/cdklabs/cdk_verified_permissions/__init__.py` & `cdklabs.cdk-verified-permissions-0.0.1a4/src/cdklabs/cdk_verified_permissions/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 This construct is still versioned with alpha/v0 major version and we could introduce breaking changes even without a major version bump. Our goal is to keep the API stable & backwards compatible as much as possible but we currently cannot guarantee that. Once we'll publish v1.0.0 the breaking changes will be introduced via major version bumps.
 
 # Getting Started
 
 ## Policy Store
 
-Define a Policy Store with defaults (No schema & Validation Settings Mode set to OFF):
+Define a Policy Store with defaults (No description, No schema & Validation Settings Mode set to OFF):
 
 ```python
 test = PolicyStore(scope, "PolicyStore")
 ```
 
 Define a Policy Store without Schema definition (Validation Settings Mode must be set to OFF):
 
@@ -24,15 +24,15 @@
     "mode": ValidationSettingsMode.OFF
 }
 test = PolicyStore(scope, "PolicyStore",
     validation_settings=validation_settings_off
 )
 ```
 
-Define a Policy Store with Schema definition (a STRICT Validation Settings Mode is strongly suggested for Policy Stores with schemas):
+Define a Policy Store with Description and Schema definition (a STRICT Validation Settings Mode is strongly suggested for Policy Stores with schemas):
 
 ```python
 validation_settings_strict = {
     "mode": ValidationSettingsMode.STRICT
 }
 cedar_json_schema = {
     "PhotoApp": {
@@ -51,15 +51,16 @@
     }
 }
 cedar_schema = {
     "cedar_json": JSON.stringify(cedar_json_schema)
 }
 policy_store = PolicyStore(scope, "PolicyStore",
     schema=cedar_schema,
-    validation_settings=validation_settings_strict
+    validation_settings=validation_settings_strict,
+    description="PolicyStore description"
 )
 ```
 
 Define a Policy Store with Schema definition from file:
 
 ```python
 validation_settings_strict = {
@@ -76,20 +77,47 @@
 
 ## Identity Source
 
 Define Identity Source with required properties:
 
 ```python
 user_pool = UserPool(scope, "UserPool") # Creating a new Cognito UserPool
+validation_settings_strict = {
+    "mode": ValidationSettingsMode.STRICT
+}
+cedar_json_schema = {
+    "PhotoApp": {
+        "entity_types": {
+            "User": {},
+            "Photo": {}
+        },
+        "actions": {
+            "view_photo": {
+                "applies_to": {
+                    "principal_types": ["User"],
+                    "resource_types": ["Photo"]
+                }
+            }
+        }
+    }
+}
+cedar_schema = {
+    "cedar_json": JSON.stringify(cedar_json_schema)
+}
+policy_store = PolicyStore(scope, "PolicyStore",
+    schema=cedar_schema,
+    validation_settings=validation_settings_strict
+)
 IdentitySource(scope, "IdentitySource",
     configuration=IdentitySourceConfiguration(
         cognito_user_pool_configuration=CognitoUserPoolConfiguration(
             user_pool=user_pool
         )
-    )
+    ),
+    policy_store=policy_store
 )
 ```
 
 Define Identity Source with all the properties:
 
 ```python
 validation_settings_strict = {
@@ -244,14 +272,17 @@
 ```
 
 # Notes
 
 * This project is following the AWS CDK Official Design Guidelines (see https://github.com/aws/aws-cdk/blob/main/docs/DESIGN_GUIDELINES.md) and the AWS CDK New Constructs Creation Guide (see here https://github.com/aws/aws-cdk/blob/main/docs/NEW_CONSTRUCTS_GUIDE.md).
 * Feedback is a gift: if you find something wrong or you've ideas to improve please open an issue or a pull request
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -896,22 +927,22 @@
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         configuration: typing.Union["IdentitySourceConfiguration", typing.Dict[builtins.str, typing.Any]],
-        policy_store: typing.Optional[IPolicyStore] = None,
+        policy_store: IPolicyStore,
         principal_entity_type: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
         :param configuration: (experimental) Identity Source configuration.
-        :param policy_store: (experimental) Policy Store in which you want to store this identity source. Default: - No policy store is set for the identity source.
+        :param policy_store: (experimental) Policy Store in which you want to store this identity source.
         :param principal_entity_type: (experimental) Principal entity type. Default: - No principal entity type for the identity source.
 
         :stability: experimental
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__adcf832dcd4c96c34d4f3375afa7da83f2c88d3d4b83602697fee9b9e94eac79)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
@@ -1055,28 +1086,28 @@
     def open_id_issuer(self) -> builtins.str:
         '''
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "openIdIssuer"))
 
     @builtins.property
-    @jsii.member(jsii_name="userPoolArn")
-    def user_pool_arn(self) -> builtins.str:
+    @jsii.member(jsii_name="policyStore")
+    def policy_store(self) -> IPolicyStore:
         '''
         :stability: experimental
         '''
-        return typing.cast(builtins.str, jsii.get(self, "userPoolArn"))
+        return typing.cast(IPolicyStore, jsii.get(self, "policyStore"))
 
     @builtins.property
-    @jsii.member(jsii_name="policyStore")
-    def policy_store(self) -> typing.Optional[IPolicyStore]:
+    @jsii.member(jsii_name="userPoolArn")
+    def user_pool_arn(self) -> builtins.str:
         '''
         :stability: experimental
         '''
-        return typing.cast(typing.Optional[IPolicyStore], jsii.get(self, "policyStore"))
+        return typing.cast(builtins.str, jsii.get(self, "userPoolArn"))
 
 
 @jsii.data_type(
     jsii_type="@cdklabs/cdk-verified-permissions.IdentitySourceAttributes",
     jsii_struct_bases=[],
     name_mapping={
         "identity_source_arn": "identitySourceArn",
@@ -1196,59 +1227,57 @@
     },
 )
 class IdentitySourceProps:
     def __init__(
         self,
         *,
         configuration: typing.Union[IdentitySourceConfiguration, typing.Dict[builtins.str, typing.Any]],
-        policy_store: typing.Optional[IPolicyStore] = None,
+        policy_store: IPolicyStore,
         principal_entity_type: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
         :param configuration: (experimental) Identity Source configuration.
-        :param policy_store: (experimental) Policy Store in which you want to store this identity source. Default: - No policy store is set for the identity source.
+        :param policy_store: (experimental) Policy Store in which you want to store this identity source.
         :param principal_entity_type: (experimental) Principal entity type. Default: - No principal entity type for the identity source.
 
         :stability: experimental
         '''
         if isinstance(configuration, dict):
             configuration = IdentitySourceConfiguration(**configuration)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__8d604e3e1efa31ac4503e3c0ae3ff6a127b687d8104f2f799f968ccdea32c7cd)
             check_type(argname="argument configuration", value=configuration, expected_type=type_hints["configuration"])
             check_type(argname="argument policy_store", value=policy_store, expected_type=type_hints["policy_store"])
             check_type(argname="argument principal_entity_type", value=principal_entity_type, expected_type=type_hints["principal_entity_type"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "configuration": configuration,
+            "policy_store": policy_store,
         }
-        if policy_store is not None:
-            self._values["policy_store"] = policy_store
         if principal_entity_type is not None:
             self._values["principal_entity_type"] = principal_entity_type
 
     @builtins.property
     def configuration(self) -> IdentitySourceConfiguration:
         '''(experimental) Identity Source configuration.
 
         :stability: experimental
         '''
         result = self._values.get("configuration")
         assert result is not None, "Required property 'configuration' is missing"
         return typing.cast(IdentitySourceConfiguration, result)
 
     @builtins.property
-    def policy_store(self) -> typing.Optional[IPolicyStore]:
+    def policy_store(self) -> IPolicyStore:
         '''(experimental) Policy Store in which you want to store this identity source.
 
-        :default: - No policy store is set for the identity source.
-
         :stability: experimental
         '''
         result = self._values.get("policy_store")
-        return typing.cast(typing.Optional[IPolicyStore], result)
+        assert result is not None, "Required property 'policy_store' is missing"
+        return typing.cast(IPolicyStore, result)
 
     @builtins.property
     def principal_entity_type(self) -> typing.Optional[builtins.str]:
         '''(experimental) Principal entity type.
 
         :default: - No principal entity type for the identity source.
 
@@ -1596,30 +1625,34 @@
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         validation_settings: IValidationSettings,
+        description: typing.Optional[builtins.str] = None,
         schema: typing.Optional[ISchema] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
         :param validation_settings: (experimental) The policy store's validation settings. Default: - If not provided, the Policy store will be created with ValidationSettingsMode = "OFF"
-        :param schema: (experimental) This attribute is not required from an API point of view. It represents the schema (in Cedar) to be applied to the PolicyStore. Default: - The schema (in Cedar) to be applied to the PolicyStore.
+        :param description: (experimental) The policy store's description. Default: - No description.
+        :param schema: (experimental) This attribute is not required from an API point of view. It represents the schema (in Cedar) to be applied to the PolicyStore. Default: - No schema.
 
         :stability: experimental
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__d06941f15025a4995e90a2baf1d7f752d4b3887e665257edc42d111f7d2b1e5f)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = PolicyStoreProps(
-            validation_settings=validation_settings, schema=schema
+            validation_settings=validation_settings,
+            description=description,
+            schema=schema,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
     @jsii.member(jsii_name="fromPolicyStoreArn")
     @builtins.classmethod
     def from_policy_store_arn(
@@ -1815,14 +1848,23 @@
         '''(experimental) Validation Settings of the Policy Store.
 
         :stability: experimental
         '''
         return typing.cast(IValidationSettings, jsii.get(self, "validationSettings"))
 
     @builtins.property
+    @jsii.member(jsii_name="description")
+    def description(self) -> typing.Optional[builtins.str]:
+        '''(experimental) Description of the Policy Store.
+
+        :stability: experimental
+        '''
+        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "description"))
+
+    @builtins.property
     @jsii.member(jsii_name="schema")
     def schema(self) -> typing.Optional[ISchema]:
         '''(experimental) Schema definition of the Policy Store.
 
         :stability: experimental
         '''
         return typing.cast(typing.Optional[ISchema], jsii.get(self, "schema"))
@@ -1896,36 +1938,45 @@
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 @jsii.data_type(
     jsii_type="@cdklabs/cdk-verified-permissions.PolicyStoreProps",
     jsii_struct_bases=[],
-    name_mapping={"validation_settings": "validationSettings", "schema": "schema"},
+    name_mapping={
+        "validation_settings": "validationSettings",
+        "description": "description",
+        "schema": "schema",
+    },
 )
 class PolicyStoreProps:
     def __init__(
         self,
         *,
         validation_settings: IValidationSettings,
+        description: typing.Optional[builtins.str] = None,
         schema: typing.Optional[ISchema] = None,
     ) -> None:
         '''
         :param validation_settings: (experimental) The policy store's validation settings. Default: - If not provided, the Policy store will be created with ValidationSettingsMode = "OFF"
-        :param schema: (experimental) This attribute is not required from an API point of view. It represents the schema (in Cedar) to be applied to the PolicyStore. Default: - The schema (in Cedar) to be applied to the PolicyStore.
+        :param description: (experimental) The policy store's description. Default: - No description.
+        :param schema: (experimental) This attribute is not required from an API point of view. It represents the schema (in Cedar) to be applied to the PolicyStore. Default: - No schema.
 
         :stability: experimental
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__0d5ec92989295c54a29590a4d6fa6f1ca994cd0d5327acb87553635b6cc4b262)
             check_type(argname="argument validation_settings", value=validation_settings, expected_type=type_hints["validation_settings"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
             check_type(argname="argument schema", value=schema, expected_type=type_hints["schema"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "validation_settings": validation_settings,
         }
+        if description is not None:
+            self._values["description"] = description
         if schema is not None:
             self._values["schema"] = schema
 
     @builtins.property
     def validation_settings(self) -> IValidationSettings:
         '''(experimental) The policy store's validation settings.
 
@@ -1934,20 +1985,31 @@
         :stability: experimental
         '''
         result = self._values.get("validation_settings")
         assert result is not None, "Required property 'validation_settings' is missing"
         return typing.cast(IValidationSettings, result)
 
     @builtins.property
+    def description(self) -> typing.Optional[builtins.str]:
+        '''(experimental) The policy store's description.
+
+        :default: - No description.
+
+        :stability: experimental
+        '''
+        result = self._values.get("description")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
     def schema(self) -> typing.Optional[ISchema]:
         '''(experimental) This attribute is not required from an API point of view.
 
         It represents the schema (in Cedar) to be applied to the PolicyStore.
 
-        :default: - The schema (in Cedar) to be applied to the PolicyStore.
+        :default: - No schema.
 
         :stability: experimental
         '''
         result = self._values.get("schema")
         return typing.cast(typing.Optional[ISchema], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
@@ -2532,15 +2594,15 @@
     pass
 
 def _typecheckingstub__adcf832dcd4c96c34d4f3375afa7da83f2c88d3d4b83602697fee9b9e94eac79(
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
     *,
     configuration: typing.Union[IdentitySourceConfiguration, typing.Dict[builtins.str, typing.Any]],
-    policy_store: typing.Optional[IPolicyStore] = None,
+    policy_store: IPolicyStore,
     principal_entity_type: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__13966d481243a96086cd56bc90424ea7f86bc0f7076a9caa968632a4d035c84a(
     scope: _constructs_77d1e7e8.Construct,
@@ -2588,15 +2650,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__8d604e3e1efa31ac4503e3c0ae3ff6a127b687d8104f2f799f968ccdea32c7cd(
     *,
     configuration: typing.Union[IdentitySourceConfiguration, typing.Dict[builtins.str, typing.Any]],
-    policy_store: typing.Optional[IPolicyStore] = None,
+    policy_store: IPolicyStore,
     principal_entity_type: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__5f47dde9d0958e6307c20d1613a3b35c47ba95f144f917faa89b35763026bf73(
     scope: _constructs_77d1e7e8.Construct,
@@ -2651,14 +2713,15 @@
     pass
 
 def _typecheckingstub__d06941f15025a4995e90a2baf1d7f752d4b3887e665257edc42d111f7d2b1e5f(
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
     *,
     validation_settings: IValidationSettings,
+    description: typing.Optional[builtins.str] = None,
     schema: typing.Optional[ISchema] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__0088ea5b9e024a2ae5eec623cfb05fba44406d22c819652eb17239c46f0b61ec(
     scope: _constructs_77d1e7e8.Construct,
@@ -2724,14 +2787,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__0d5ec92989295c54a29590a4d6fa6f1ca994cd0d5327acb87553635b6cc4b262(
     *,
     validation_settings: IValidationSettings,
+    description: typing.Optional[builtins.str] = None,
     schema: typing.Optional[ISchema] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__048e8afdb9ae9d874f46b943d584373e9467c5c993d26dc5f461270f297ddaf1(
     scope: _constructs_77d1e7e8.Construct,
```

### Comparing `cdklabs.cdk-verified-permissions-0.0.1a3/src/cdklabs.cdk_verified_permissions.egg-info/PKG-INFO` & `cdklabs.cdk-verified-permissions-0.0.1a4/src/cdklabs.cdk_verified_permissions.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdklabs.cdk-verified-permissions
-Version: 0.0.1a3
+Version: 0.0.1a4
 Summary: L2 AWS CDK Constructs for Amazon Verified Permissions
 Home-page: https://github.com/cdklabs/cdk-verified-permissions.git
 Author: Amazon Web Services<aws-cdk-dev@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-verified-permissions.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -30,15 +30,15 @@
 
 This construct is still versioned with alpha/v0 major version and we could introduce breaking changes even without a major version bump. Our goal is to keep the API stable & backwards compatible as much as possible but we currently cannot guarantee that. Once we'll publish v1.0.0 the breaking changes will be introduced via major version bumps.
 
 # Getting Started
 
 ## Policy Store
 
-Define a Policy Store with defaults (No schema & Validation Settings Mode set to OFF):
+Define a Policy Store with defaults (No description, No schema & Validation Settings Mode set to OFF):
 
 ```python
 test = PolicyStore(scope, "PolicyStore")
 ```
 
 Define a Policy Store without Schema definition (Validation Settings Mode must be set to OFF):
 
@@ -47,15 +47,15 @@
     "mode": ValidationSettingsMode.OFF
 }
 test = PolicyStore(scope, "PolicyStore",
     validation_settings=validation_settings_off
 )
 ```
 
-Define a Policy Store with Schema definition (a STRICT Validation Settings Mode is strongly suggested for Policy Stores with schemas):
+Define a Policy Store with Description and Schema definition (a STRICT Validation Settings Mode is strongly suggested for Policy Stores with schemas):
 
 ```python
 validation_settings_strict = {
     "mode": ValidationSettingsMode.STRICT
 }
 cedar_json_schema = {
     "PhotoApp": {
@@ -74,15 +74,16 @@
     }
 }
 cedar_schema = {
     "cedar_json": JSON.stringify(cedar_json_schema)
 }
 policy_store = PolicyStore(scope, "PolicyStore",
     schema=cedar_schema,
-    validation_settings=validation_settings_strict
+    validation_settings=validation_settings_strict,
+    description="PolicyStore description"
 )
 ```
 
 Define a Policy Store with Schema definition from file:
 
 ```python
 validation_settings_strict = {
@@ -99,20 +100,47 @@
 
 ## Identity Source
 
 Define Identity Source with required properties:
 
 ```python
 user_pool = UserPool(scope, "UserPool") # Creating a new Cognito UserPool
+validation_settings_strict = {
+    "mode": ValidationSettingsMode.STRICT
+}
+cedar_json_schema = {
+    "PhotoApp": {
+        "entity_types": {
+            "User": {},
+            "Photo": {}
+        },
+        "actions": {
+            "view_photo": {
+                "applies_to": {
+                    "principal_types": ["User"],
+                    "resource_types": ["Photo"]
+                }
+            }
+        }
+    }
+}
+cedar_schema = {
+    "cedar_json": JSON.stringify(cedar_json_schema)
+}
+policy_store = PolicyStore(scope, "PolicyStore",
+    schema=cedar_schema,
+    validation_settings=validation_settings_strict
+)
 IdentitySource(scope, "IdentitySource",
     configuration=IdentitySourceConfiguration(
         cognito_user_pool_configuration=CognitoUserPoolConfiguration(
             user_pool=user_pool
         )
-    )
+    ),
+    policy_store=policy_store
 )
 ```
 
 Define Identity Source with all the properties:
 
 ```python
 validation_settings_strict = {
```

### Comparing `cdklabs.cdk-verified-permissions-0.0.1a3/src/cdklabs.cdk_verified_permissions.egg-info/SOURCES.txt` & `cdklabs.cdk-verified-permissions-0.0.1a4/src/cdklabs.cdk_verified_permissions.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 src/cdklabs.cdk_verified_permissions.egg-info/SOURCES.txt
 src/cdklabs.cdk_verified_permissions.egg-info/dependency_links.txt
 src/cdklabs.cdk_verified_permissions.egg-info/requires.txt
 src/cdklabs.cdk_verified_permissions.egg-info/top_level.txt
 src/cdklabs/cdk_verified_permissions/__init__.py
 src/cdklabs/cdk_verified_permissions/py.typed
 src/cdklabs/cdk_verified_permissions/_jsii/__init__.py
-src/cdklabs/cdk_verified_permissions/_jsii/cdk-verified-permissions@0.0.1-alpha.3.jsii.tgz
+src/cdklabs/cdk_verified_permissions/_jsii/cdk-verified-permissions@0.0.1-alpha.4.jsii.tgz
```

