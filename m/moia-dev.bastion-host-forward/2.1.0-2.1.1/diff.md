# Comparing `tmp/moia-dev.bastion-host-forward-2.1.0.tar.gz` & `tmp/moia-dev.bastion-host-forward-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moia-dev.bastion-host-forward-2.1.0.tar", last modified: Mon Feb  5 09:37:46 2024, max compression
+gzip compressed data, was "moia-dev.bastion-host-forward-2.1.1.tar", last modified: Tue Apr  2 13:02:59 2024, max compression
```

## Comparing `moia-dev.bastion-host-forward-2.1.0.tar` & `moia-dev.bastion-host-forward-2.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 09:37:46.172164 moia-dev.bastion-host-forward-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-05 09:37:39.000000 moia-dev.bastion-host-forward-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-05 09:37:39.000000 moia-dev.bastion-host-forward-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    14920 2024-02-05 09:37:46.172164 moia-dev.bastion-host-forward-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13981 2024-02-05 09:37:39.000000 moia-dev.bastion-host-forward-2.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-02-05 09:37:39.000000 moia-dev.bastion-host-forward-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-05 09:37:46.172164 moia-dev.bastion-host-forward-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-02-05 09:37:39.000000 moia-dev.bastion-host-forward-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 09:37:46.172164 moia-dev.bastion-host-forward-2.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 09:37:46.172164 moia-dev.bastion-host-forward-2.1.0/src/moia_dev/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 09:37:46.172164 moia-dev.bastion-host-forward-2.1.0/src/moia_dev/bastion_host_forward/
--rw-r--r--   0 runner    (1001) docker     (127)    72003 2024-02-05 09:37:39.000000 moia-dev.bastion-host-forward-2.1.0/src/moia_dev/bastion_host_forward/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 09:37:46.172164 moia-dev.bastion-host-forward-2.1.0/src/moia_dev/bastion_host_forward/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-02-05 09:37:39.000000 moia-dev.bastion-host-forward-2.1.0/src/moia_dev/bastion_host_forward/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    82170 2024-02-05 09:37:39.000000 moia-dev.bastion-host-forward-2.1.0/src/moia_dev/bastion_host_forward/_jsii/bastion-host-forward@2.1.0.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-05 09:37:39.000000 moia-dev.bastion-host-forward-2.1.0/src/moia_dev/bastion_host_forward/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 09:37:46.172164 moia-dev.bastion-host-forward-2.1.0/src/moia_dev.bastion_host_forward.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14920 2024-02-05 09:37:46.000000 moia-dev.bastion-host-forward-2.1.0/src/moia_dev.bastion_host_forward.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-02-05 09:37:46.000000 moia-dev.bastion-host-forward-2.1.0/src/moia_dev.bastion_host_forward.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-05 09:37:46.000000 moia-dev.bastion-host-forward-2.1.0/src/moia_dev.bastion_host_forward.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-02-05 09:37:46.000000 moia-dev.bastion-host-forward-2.1.0/src/moia_dev.bastion_host_forward.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-05 09:37:46.000000 moia-dev.bastion-host-forward-2.1.0/src/moia_dev.bastion_host_forward.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:02:59.291098 moia-dev.bastion-host-forward-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-02 13:02:50.000000 moia-dev.bastion-host-forward-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-02 13:02:50.000000 moia-dev.bastion-host-forward-2.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    14920 2024-04-02 13:02:59.291098 moia-dev.bastion-host-forward-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13981 2024-04-02 13:02:50.000000 moia-dev.bastion-host-forward-2.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-02 13:02:50.000000 moia-dev.bastion-host-forward-2.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 13:02:59.291098 moia-dev.bastion-host-forward-2.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-02 13:02:50.000000 moia-dev.bastion-host-forward-2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:02:59.291098 moia-dev.bastion-host-forward-2.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:02:59.291098 moia-dev.bastion-host-forward-2.1.1/src/moia_dev/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:02:59.291098 moia-dev.bastion-host-forward-2.1.1/src/moia_dev/bastion_host_forward/
+-rw-r--r--   0 runner    (1001) docker     (127)    72079 2024-04-02 13:02:50.000000 moia-dev.bastion-host-forward-2.1.1/src/moia_dev/bastion_host_forward/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:02:59.291098 moia-dev.bastion-host-forward-2.1.1/src/moia_dev/bastion_host_forward/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-02 13:02:50.000000 moia-dev.bastion-host-forward-2.1.1/src/moia_dev/bastion_host_forward/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82153 2024-04-02 13:02:50.000000 moia-dev.bastion-host-forward-2.1.1/src/moia_dev/bastion_host_forward/_jsii/bastion-host-forward@2.1.1.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 13:02:50.000000 moia-dev.bastion-host-forward-2.1.1/src/moia_dev/bastion_host_forward/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:02:59.291098 moia-dev.bastion-host-forward-2.1.1/src/moia_dev.bastion_host_forward.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14920 2024-04-02 13:02:59.000000 moia-dev.bastion-host-forward-2.1.1/src/moia_dev.bastion_host_forward.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-02 13:02:59.000000 moia-dev.bastion-host-forward-2.1.1/src/moia_dev.bastion_host_forward.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 13:02:59.000000 moia-dev.bastion-host-forward-2.1.1/src/moia_dev.bastion_host_forward.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-02 13:02:59.000000 moia-dev.bastion-host-forward-2.1.1/src/moia_dev.bastion_host_forward.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-02 13:02:59.000000 moia-dev.bastion-host-forward-2.1.1/src/moia_dev.bastion_host_forward.egg-info/top_level.txt
```

### Comparing `moia-dev.bastion-host-forward-2.1.0/LICENSE` & `moia-dev.bastion-host-forward-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `moia-dev.bastion-host-forward-2.1.0/PKG-INFO` & `moia-dev.bastion-host-forward-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moia-dev.bastion-host-forward
-Version: 2.1.0
+Version: 2.1.1
 Summary: CDK Construct for creating a bastion host to forward a connection to several AWS data services inside a private subnet from your local machine
 Home-page: https://github.com/moia-oss/bastion-host-forward
 Author: MOIA GmbH
 License: Apache-2.0
 Project-URL: Source, https://github.com/moia-oss/bastion-host-forward
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `moia-dev.bastion-host-forward-2.1.0/README.md` & `moia-dev.bastion-host-forward-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `moia-dev.bastion-host-forward-2.1.0/setup.py` & `moia-dev.bastion-host-forward-2.1.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "moia-dev.bastion-host-forward",
-    "version": "2.1.0",
+    "version": "2.1.1",
     "description": "CDK Construct for creating a bastion host to forward a connection to several AWS data services inside a private subnet from your local machine",
     "license": "Apache-2.0",
     "url": "https://github.com/moia-oss/bastion-host-forward",
     "long_description_content_type": "text/markdown",
     "author": "MOIA GmbH",
     "bdist_wheel": {
         "universal": true
@@ -22,25 +22,25 @@
     },
     "packages": [
         "moia_dev.bastion_host_forward",
         "moia_dev.bastion_host_forward._jsii"
     ],
     "package_data": {
         "moia_dev.bastion_host_forward._jsii": [
-            "bastion-host-forward@2.1.0.jsii.tgz"
+            "bastion-host-forward@2.1.1.jsii.tgz"
         ],
         "moia_dev.bastion_host_forward": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
         "aws-cdk-lib>=2.121.1, <3.0.0",
         "constructs>=10.3.0, <11.0.0",
-        "jsii>=1.93.0, <2.0.0",
+        "jsii>=1.96.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `moia-dev.bastion-host-forward-2.1.0/src/moia_dev/bastion_host_forward/__init__.py` & `moia-dev.bastion-host-forward-2.1.1/src/moia_dev/bastion_host_forward/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -401,14 +401,17 @@
 ```
 psql "host=<rds endpoint> port=5432 dbname=<database name> user=<iamUser> sslrootcert=<full path to downloaded cert> sslmode=verify-ca"
 ```
 
 For a full guide on how to connect to an IAM authenticated RDS check out [this
 guide by AWS](https://aws.amazon.com/premiumsupport/knowledge-center/users-connect-rds-iam/)
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
```

### Comparing `moia-dev.bastion-host-forward-2.1.0/src/moia_dev.bastion_host_forward.egg-info/PKG-INFO` & `moia-dev.bastion-host-forward-2.1.1/src/moia_dev.bastion_host_forward.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moia-dev.bastion-host-forward
-Version: 2.1.0
+Version: 2.1.1
 Summary: CDK Construct for creating a bastion host to forward a connection to several AWS data services inside a private subnet from your local machine
 Home-page: https://github.com/moia-oss/bastion-host-forward
 Author: MOIA GmbH
 License: Apache-2.0
 Project-URL: Source, https://github.com/moia-oss/bastion-host-forward
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `moia-dev.bastion-host-forward-2.1.0/src/moia_dev.bastion_host_forward.egg-info/SOURCES.txt` & `moia-dev.bastion-host-forward-2.1.1/src/moia_dev.bastion_host_forward.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/moia_dev.bastion_host_forward.egg-info/SOURCES.txt
 src/moia_dev.bastion_host_forward.egg-info/dependency_links.txt
 src/moia_dev.bastion_host_forward.egg-info/requires.txt
 src/moia_dev.bastion_host_forward.egg-info/top_level.txt
 src/moia_dev/bastion_host_forward/__init__.py
 src/moia_dev/bastion_host_forward/py.typed
 src/moia_dev/bastion_host_forward/_jsii/__init__.py
-src/moia_dev/bastion_host_forward/_jsii/bastion-host-forward@2.1.0.jsii.tgz
+src/moia_dev/bastion_host_forward/_jsii/bastion-host-forward@2.1.1.jsii.tgz
```

