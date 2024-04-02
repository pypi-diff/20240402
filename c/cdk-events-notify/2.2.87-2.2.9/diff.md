# Comparing `tmp/cdk-events-notify-2.2.87.tar.gz` & `tmp/cdk-events-notify-2.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-events-notify-2.2.87.tar", last modified: Tue Apr  2 00:11:09 2024, max compression
+gzip compressed data, was "cdk-events-notify-2.2.9.tar", last modified: Tue Jan  9 00:11:54 2024, max compression
```

## Comparing `cdk-events-notify-2.2.87.tar` & `cdk-events-notify-2.2.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:09.372299 cdk-events-notify-2.2.87/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-02 00:10:55.000000 cdk-events-notify-2.2.87/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-02 00:10:55.000000 cdk-events-notify-2.2.87/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-04-02 00:11:09.372299 cdk-events-notify-2.2.87/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-04-02 00:10:55.000000 cdk-events-notify-2.2.87/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-02 00:10:55.000000 cdk-events-notify-2.2.87/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 00:11:09.372299 cdk-events-notify-2.2.87/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-02 00:10:55.000000 cdk-events-notify-2.2.87/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:09.368299 cdk-events-notify-2.2.87/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:09.368299 cdk-events-notify-2.2.87/src/cdk_events_notify/
--rw-r--r--   0 runner    (1001) docker     (127)     9464 2024-04-02 00:10:55.000000 cdk-events-notify-2.2.87/src/cdk_events_notify/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:09.372299 cdk-events-notify-2.2.87/src/cdk_events_notify/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-02 00:10:55.000000 cdk-events-notify-2.2.87/src/cdk_events_notify/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24932 2024-04-02 00:10:55.000000 cdk-events-notify-2.2.87/src/cdk_events_notify/_jsii/cdk-events-notify@2.2.87.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 00:10:55.000000 cdk-events-notify-2.2.87/src/cdk_events_notify/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:11:09.372299 cdk-events-notify-2.2.87/src/cdk_events_notify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-04-02 00:11:09.000000 cdk-events-notify-2.2.87/src/cdk_events_notify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-02 00:11:09.000000 cdk-events-notify-2.2.87/src/cdk_events_notify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 00:11:09.000000 cdk-events-notify-2.2.87/src/cdk_events_notify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-02 00:11:09.000000 cdk-events-notify-2.2.87/src/cdk_events_notify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-02 00:11:09.000000 cdk-events-notify-2.2.87/src/cdk_events_notify.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 00:11:54.464156 cdk-events-notify-2.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-01-09 00:11:43.000000 cdk-events-notify-2.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-01-09 00:11:43.000000 cdk-events-notify-2.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-01-09 00:11:54.464156 cdk-events-notify-2.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-01-09 00:11:43.000000 cdk-events-notify-2.2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-01-09 00:11:43.000000 cdk-events-notify-2.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-09 00:11:54.464156 cdk-events-notify-2.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-01-09 00:11:43.000000 cdk-events-notify-2.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 00:11:54.460156 cdk-events-notify-2.2.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 00:11:54.460156 cdk-events-notify-2.2.9/src/cdk_events_notify/
+-rw-r--r--   0 runner    (1001) docker     (127)     9388 2024-01-09 00:11:43.000000 cdk-events-notify-2.2.9/src/cdk_events_notify/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 00:11:54.464156 cdk-events-notify-2.2.9/src/cdk_events_notify/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-01-09 00:11:43.000000 cdk-events-notify-2.2.9/src/cdk_events_notify/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24484 2024-01-09 00:11:43.000000 cdk-events-notify-2.2.9/src/cdk_events_notify/_jsii/cdk-events-notify@2.2.9.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-09 00:11:43.000000 cdk-events-notify-2.2.9/src/cdk_events_notify/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 00:11:54.464156 cdk-events-notify-2.2.9/src/cdk_events_notify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-01-09 00:11:54.000000 cdk-events-notify-2.2.9/src/cdk_events_notify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-01-09 00:11:54.000000 cdk-events-notify-2.2.9/src/cdk_events_notify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-09 00:11:54.000000 cdk-events-notify-2.2.9/src/cdk_events_notify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-01-09 00:11:54.000000 cdk-events-notify-2.2.9/src/cdk_events_notify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-01-09 00:11:54.000000 cdk-events-notify-2.2.9/src/cdk_events_notify.egg-info/top_level.txt
```

### Comparing `cdk-events-notify-2.2.87/LICENSE` & `cdk-events-notify-2.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-events-notify-2.2.87/PKG-INFO` & `cdk-events-notify-2.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-events-notify
-Version: 2.2.87
+Version: 2.2.9
 Summary: The Events Notify AWS Construct lib for AWS CDK
 Home-page: https://github.com/neilkuan/cdk-events-notify.git
 Author: Neil Kuan<guan840912@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/neilkuan/cdk-events-notify.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-events-notify-2.2.87/README.md` & `cdk-events-notify-2.2.9/README.md`

 * *Files identical despite different names*

### Comparing `cdk-events-notify-2.2.87/setup.py` & `cdk-events-notify-2.2.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-events-notify",
-    "version": "2.2.87",
+    "version": "2.2.9",
     "description": "The Events Notify AWS Construct lib for AWS CDK",
     "license": "Apache-2.0",
     "url": "https://github.com/neilkuan/cdk-events-notify.git",
     "long_description_content_type": "text/markdown",
     "author": "Neil Kuan<guan840912@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,25 +22,25 @@
     },
     "packages": [
         "cdk_events_notify",
         "cdk_events_notify._jsii"
     ],
     "package_data": {
         "cdk_events_notify._jsii": [
-            "cdk-events-notify@2.2.87.jsii.tgz"
+            "cdk-events-notify@2.2.9.jsii.tgz"
         ],
         "cdk_events_notify": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
-        "aws-cdk-lib>=2.126.0, <3.0.0",
+        "aws-cdk-lib>=2.117.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "jsii>=1.96.0, <2.0.0",
+        "jsii>=1.93.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `cdk-events-notify-2.2.87/src/cdk_events_notify/__init__.py` & `cdk-events-notify-2.2.9/src/cdk_events_notify/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,17 +92,14 @@
 > Note: Event Bridge can not cross region , if you console sign in not the cdk-events-notify region will not get the evnet in cloudtrail see this [docs](https://docs.aws.amazon.com/IAM/latest/UserGuide/cloudtrail-integration.html#cloudtrail-integration_signin-regions)
 
 ## :clap:  Supporters
 
 [![Stargazers repo roster for @neilkuan/cdk-events-notify](https://reporoster.com/stars/neilkuan/cdk-events-notify)](https://github.com/neilkuan/cdk-events-notify/stargazers)
 [![Forkers repo roster for @neilkuan/cdk-events-notify](https://reporoster.com/forks/neilkuan/cdk-events-notify)](https://github.com/neilkuan/cdk-events-notify/network/members)
 '''
-from pkgutil import extend_path
-__path__ = extend_path(__path__, __name__)
-
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
```

### Comparing `cdk-events-notify-2.2.87/src/cdk_events_notify.egg-info/PKG-INFO` & `cdk-events-notify-2.2.9/src/cdk_events_notify.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-events-notify
-Version: 2.2.87
+Version: 2.2.9
 Summary: The Events Notify AWS Construct lib for AWS CDK
 Home-page: https://github.com/neilkuan/cdk-events-notify.git
 Author: Neil Kuan<guan840912@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/neilkuan/cdk-events-notify.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

