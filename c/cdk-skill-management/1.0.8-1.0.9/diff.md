# Comparing `tmp/cdk-skill-management-1.0.8.tar.gz` & `tmp/cdk-skill-management-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-skill-management-1.0.8.tar", last modified: Sun Oct 29 17:54:55 2023, max compression
+gzip compressed data, was "cdk-skill-management-1.0.9.tar", last modified: Sun Oct 29 18:36:01 2023, max compression
```

## Comparing `cdk-skill-management-1.0.8.tar` & `cdk-skill-management-1.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-29 17:54:55.358418 cdk-skill-management-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2023-10-29 17:54:37.000000 cdk-skill-management-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-10-29 17:54:37.000000 cdk-skill-management-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6439 2023-10-29 17:54:55.358418 cdk-skill-management-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5468 2023-10-29 17:54:37.000000 cdk-skill-management-1.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2023-10-29 17:54:37.000000 cdk-skill-management-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-29 17:54:55.358418 cdk-skill-management-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2023-10-29 17:54:37.000000 cdk-skill-management-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-29 17:54:55.354418 cdk-skill-management-1.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-29 17:54:55.358418 cdk-skill-management-1.0.8/src/cdk_skill_management/
--rw-r--r--   0 runner    (1001) docker     (127)    67805 2023-10-29 17:54:37.000000 cdk-skill-management-1.0.8/src/cdk_skill_management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-29 17:54:55.358418 cdk-skill-management-1.0.8/src/cdk_skill_management/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      420 2023-10-29 17:54:37.000000 cdk-skill-management-1.0.8/src/cdk_skill_management/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   236021 2023-10-29 17:54:37.000000 cdk-skill-management-1.0.8/src/cdk_skill_management/_jsii/cdk-skill-management@1.0.8.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-29 17:54:37.000000 cdk-skill-management-1.0.8/src/cdk_skill_management/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-29 17:54:55.358418 cdk-skill-management-1.0.8/src/cdk_skill_management.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6439 2023-10-29 17:54:55.000000 cdk-skill-management-1.0.8/src/cdk_skill_management.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      473 2023-10-29 17:54:55.000000 cdk-skill-management-1.0.8/src/cdk_skill_management.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-29 17:54:55.000000 cdk-skill-management-1.0.8/src/cdk_skill_management.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2023-10-29 17:54:55.000000 cdk-skill-management-1.0.8/src/cdk_skill_management.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-10-29 17:54:55.000000 cdk-skill-management-1.0.8/src/cdk_skill_management.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-29 18:36:01.879019 cdk-skill-management-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2023-10-29 18:35:49.000000 cdk-skill-management-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2023-10-29 18:35:49.000000 cdk-skill-management-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6439 2023-10-29 18:36:01.879019 cdk-skill-management-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5468 2023-10-29 18:35:49.000000 cdk-skill-management-1.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2023-10-29 18:35:49.000000 cdk-skill-management-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-29 18:36:01.879019 cdk-skill-management-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2023-10-29 18:35:49.000000 cdk-skill-management-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-29 18:36:01.879019 cdk-skill-management-1.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-29 18:36:01.879019 cdk-skill-management-1.0.9/src/cdk_skill_management/
+-rw-r--r--   0 runner    (1001) docker     (127)    67406 2023-10-29 18:35:49.000000 cdk-skill-management-1.0.9/src/cdk_skill_management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-29 18:36:01.879019 cdk-skill-management-1.0.9/src/cdk_skill_management/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2023-10-29 18:35:49.000000 cdk-skill-management-1.0.9/src/cdk_skill_management/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   235730 2023-10-29 18:35:49.000000 cdk-skill-management-1.0.9/src/cdk_skill_management/_jsii/cdk-skill-management@1.0.9.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-29 18:35:49.000000 cdk-skill-management-1.0.9/src/cdk_skill_management/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-29 18:36:01.879019 cdk-skill-management-1.0.9/src/cdk_skill_management.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6439 2023-10-29 18:36:01.000000 cdk-skill-management-1.0.9/src/cdk_skill_management.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2023-10-29 18:36:01.000000 cdk-skill-management-1.0.9/src/cdk_skill_management.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-29 18:36:01.000000 cdk-skill-management-1.0.9/src/cdk_skill_management.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2023-10-29 18:36:01.000000 cdk-skill-management-1.0.9/src/cdk_skill_management.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2023-10-29 18:36:01.000000 cdk-skill-management-1.0.9/src/cdk_skill_management.egg-info/top_level.txt
```

### Comparing `cdk-skill-management-1.0.8/LICENSE` & `cdk-skill-management-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-skill-management-1.0.8/PKG-INFO` & `cdk-skill-management-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-skill-management
-Version: 1.0.8
+Version: 1.0.9
 Summary: CDK constructs to manage Alexa Skills
 Home-page: https://github.com/t0bst4r/cdk-skill-management.git
 Author: t0bst4r<82281152+t0bst4r@users.noreply.github.com>
 License: MIT
 Project-URL: Source, https://github.com/t0bst4r/cdk-skill-management.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-skill-management-1.0.8/README.md` & `cdk-skill-management-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `cdk-skill-management-1.0.8/setup.py` & `cdk-skill-management-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-skill-management",
-    "version": "1.0.8",
+    "version": "1.0.9",
     "description": "CDK constructs to manage Alexa Skills",
     "license": "MIT",
     "url": "https://github.com/t0bst4r/cdk-skill-management.git",
     "long_description_content_type": "text/markdown",
     "author": "t0bst4r<82281152+t0bst4r@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_skill_management",
         "cdk_skill_management._jsii"
     ],
     "package_data": {
         "cdk_skill_management._jsii": [
-            "cdk-skill-management@1.0.8.jsii.tgz"
+            "cdk-skill-management@1.0.9.jsii.tgz"
         ],
         "cdk_skill_management": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk-skill-management-1.0.8/src/cdk_skill_management/__init__.py` & `cdk-skill-management-1.0.9/src/cdk_skill_management/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,15 +150,14 @@
 
 from typeguard import check_type
 
 from ._jsii import *
 
 import aws_cdk as _aws_cdk_ceddda9d
 import aws_cdk.alexa_ask as _aws_cdk_alexa_ask_ceddda9d
-import aws_cdk.aws_iam as _aws_cdk_aws_iam_ceddda9d
 import aws_cdk.aws_lambda as _aws_cdk_aws_lambda_ceddda9d
 import aws_cdk.aws_s3_assets as _aws_cdk_aws_s3_assets_ceddda9d
 import constructs as _constructs_77d1e7e8
 
 
 @jsii.data_type(
     jsii_type="cdk-skill-management.AccountLinkingPlatformAuthorizationUrl",
@@ -485,15 +484,14 @@
 
     def __repr__(self) -> str:
         return "AccountLinkingRequest(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
-@jsii.implements(_aws_cdk_aws_iam_ceddda9d.IGrantable)
 class AskCustomResource(
     _aws_cdk_ceddda9d.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="cdk-skill-management.AskCustomResource",
 ):
     '''A custom CloudFormation resource for Alexa Skill Kit SDK calls.'''
 
@@ -544,20 +542,14 @@
         :return: The value of the response field.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__b8d16c15b3ed43d105d5e1cd9c8e271ca33a03b139997f1b536fec196e34bbb0)
             check_type(argname="argument data_path", value=data_path, expected_type=type_hints["data_path"])
         return typing.cast(builtins.str, jsii.invoke(self, "getResponseField", [data_path]))
 
-    @builtins.property
-    @jsii.member(jsii_name="grantPrincipal")
-    def grant_principal(self) -> _aws_cdk_aws_iam_ceddda9d.IPrincipal:
-        '''The principal to grant permissions to.'''
-        return typing.cast(_aws_cdk_aws_iam_ceddda9d.IPrincipal, jsii.get(self, "grantPrincipal"))
-
 
 @jsii.data_type(
     jsii_type="cdk-skill-management.AskCustomResourceProps",
     jsii_struct_bases=[],
     name_mapping={
         "authentication_configuration": "authenticationConfiguration",
         "on_create": "onCreate",
```

### Comparing `cdk-skill-management-1.0.8/src/cdk_skill_management.egg-info/PKG-INFO` & `cdk-skill-management-1.0.9/src/cdk_skill_management.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-skill-management
-Version: 1.0.8
+Version: 1.0.9
 Summary: CDK constructs to manage Alexa Skills
 Home-page: https://github.com/t0bst4r/cdk-skill-management.git
 Author: t0bst4r<82281152+t0bst4r@users.noreply.github.com>
 License: MIT
 Project-URL: Source, https://github.com/t0bst4r/cdk-skill-management.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

