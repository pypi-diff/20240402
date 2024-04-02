# Comparing `tmp/gammarer.aws-secure-bucket-1.1.9.tar.gz` & `tmp/gammarer.aws-secure-bucket-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gammarer.aws-secure-bucket-1.1.9.tar", last modified: Sun Mar  3 17:13:42 2024, max compression
+gzip compressed data, was "gammarer.aws-secure-bucket-1.2.0.tar", last modified: Tue Apr  2 06:05:46 2024, max compression
```

## Comparing `gammarer.aws-secure-bucket-1.1.9.tar` & `gammarer.aws-secure-bucket-1.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 17:13:42.173355 gammarer.aws-secure-bucket-1.1.9/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-03-03 17:13:27.000000 gammarer.aws-secure-bucket-1.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-03 17:13:27.000000 gammarer.aws-secure-bucket-1.1.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-03-03 17:13:42.173355 gammarer.aws-secure-bucket-1.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-03-03 17:13:27.000000 gammarer.aws-secure-bucket-1.1.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-03 17:13:27.000000 gammarer.aws-secure-bucket-1.1.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-03 17:13:42.173355 gammarer.aws-secure-bucket-1.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-03-03 17:13:27.000000 gammarer.aws-secure-bucket-1.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 17:13:42.169355 gammarer.aws-secure-bucket-1.1.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 17:13:42.169355 gammarer.aws-secure-bucket-1.1.9/src/gammarer/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 17:13:42.173355 gammarer.aws-secure-bucket-1.1.9/src/gammarer/aws_secure_bucket/
--rw-r--r--   0 runner    (1001) docker     (127)    11077 2024-03-03 17:13:27.000000 gammarer.aws-secure-bucket-1.1.9/src/gammarer/aws_secure_bucket/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 17:13:42.173355 gammarer.aws-secure-bucket-1.1.9/src/gammarer/aws_secure_bucket/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-03-03 17:13:27.000000 gammarer.aws-secure-bucket-1.1.9/src/gammarer/aws_secure_bucket/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33631 2024-03-03 17:13:27.000000 gammarer.aws-secure-bucket-1.1.9/src/gammarer/aws_secure_bucket/_jsii/aws-secure-bucket@1.1.9.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-03 17:13:27.000000 gammarer.aws-secure-bucket-1.1.9/src/gammarer/aws_secure_bucket/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 17:13:42.173355 gammarer.aws-secure-bucket-1.1.9/src/gammarer.aws_secure_bucket.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-03-03 17:13:42.000000 gammarer.aws-secure-bucket-1.1.9/src/gammarer.aws_secure_bucket.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-03-03 17:13:42.000000 gammarer.aws-secure-bucket-1.1.9/src/gammarer.aws_secure_bucket.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-03 17:13:42.000000 gammarer.aws-secure-bucket-1.1.9/src/gammarer.aws_secure_bucket.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-03 17:13:42.000000 gammarer.aws-secure-bucket-1.1.9/src/gammarer.aws_secure_bucket.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-03 17:13:42.000000 gammarer.aws-secure-bucket-1.1.9/src/gammarer.aws_secure_bucket.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:05:46.127530 gammarer.aws-secure-bucket-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-02 06:05:35.000000 gammarer.aws-secure-bucket-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-02 06:05:35.000000 gammarer.aws-secure-bucket-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-04-02 06:05:46.127530 gammarer.aws-secure-bucket-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-02 06:05:35.000000 gammarer.aws-secure-bucket-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-02 06:05:35.000000 gammarer.aws-secure-bucket-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 06:05:46.127530 gammarer.aws-secure-bucket-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-02 06:05:35.000000 gammarer.aws-secure-bucket-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:05:46.123530 gammarer.aws-secure-bucket-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:05:46.123530 gammarer.aws-secure-bucket-1.2.0/src/gammarer/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:05:46.127530 gammarer.aws-secure-bucket-1.2.0/src/gammarer/aws_secure_bucket/
+-rw-r--r--   0 runner    (1001) docker     (127)    11316 2024-04-02 06:05:35.000000 gammarer.aws-secure-bucket-1.2.0/src/gammarer/aws_secure_bucket/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:05:46.127530 gammarer.aws-secure-bucket-1.2.0/src/gammarer/aws_secure_bucket/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-02 06:05:35.000000 gammarer.aws-secure-bucket-1.2.0/src/gammarer/aws_secure_bucket/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33686 2024-04-02 06:05:35.000000 gammarer.aws-secure-bucket-1.2.0/src/gammarer/aws_secure_bucket/_jsii/aws-secure-bucket@1.2.0.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 06:05:35.000000 gammarer.aws-secure-bucket-1.2.0/src/gammarer/aws_secure_bucket/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:05:46.123530 gammarer.aws-secure-bucket-1.2.0/src/gammarer.aws_secure_bucket.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-04-02 06:05:46.000000 gammarer.aws-secure-bucket-1.2.0/src/gammarer.aws_secure_bucket.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-02 06:05:46.000000 gammarer.aws-secure-bucket-1.2.0/src/gammarer.aws_secure_bucket.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 06:05:46.000000 gammarer.aws-secure-bucket-1.2.0/src/gammarer.aws_secure_bucket.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-02 06:05:46.000000 gammarer.aws-secure-bucket-1.2.0/src/gammarer.aws_secure_bucket.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-02 06:05:46.000000 gammarer.aws-secure-bucket-1.2.0/src/gammarer.aws_secure_bucket.egg-info/top_level.txt
```

### Comparing `gammarer.aws-secure-bucket-1.1.9/LICENSE` & `gammarer.aws-secure-bucket-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gammarer.aws-secure-bucket-1.1.9/PKG-INFO` & `gammarer.aws-secure-bucket-1.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-secure-bucket
-Version: 1.1.9
+Version: 1.2.0
 Summary: This is a Simple S3 Secure Bucket.
 Home-page: https://github.com/gammarer/aws-secure-bucket.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarer/aws-secure-bucket.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -17,23 +17,25 @@
 Classifier: Typing :: Typed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![GitHub](https://img.shields.io/github/license/yicr/aws-secure-bucket?style=flat-square)](https://github.com/yicr/aws-secure-bucket/blob/main/LICENSE)
+# AWS Secure Bucket
+
+[![GitHub](https://img.shields.io/github/license/gammarer/aws-secure-bucket?style=flat-square)](https://github.com/gammarer/aws-secure-bucket/blob/main/LICENSE)
 [![npm (scoped)](https://img.shields.io/npm/v/@gammarer/aws-secure-bucket?style=flat-square)](https://www.npmjs.com/package/@gammarer/aws-secure-bucket)
 [![PyPI](https://img.shields.io/pypi/v/gammarer.aws-secure-bucket?style=flat-square)](https://pypi.org/project/gammarer.aws-secure-bucket/)
 [![Nuget](https://img.shields.io/nuget/v/Gammarer.CDK.AWS.SecureBucket?style=flat-square)](https://www.nuget.org/packages/Gammarer.CDK.AWS.SecureBucket/)
 [![Sonatype Nexus (Releases)](https://img.shields.io/nexus/r/com.gammarer/aws-secure-bucket?server=https%3A%2F%2Fs01.oss.sonatype.org%2F&style=flat-square)](https://s01.oss.sonatype.org/content/repositories/releases/com/gammarer/aws-secure-bucket/)
-[![GitHub Workflow Status (branch)](https://img.shields.io/github/actions/workflow/status/yicr/aws-secure-bucket/release.yml?branch=main&label=release&style=flat-square)](https://github.com/yicr/aws-secure-bucket/actions/workflows/release.yml)
-[![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/yicr/aws-secure-bucket?sort=semver&style=flat-square)](https://github.com/yicr/aws-secure-bucket/releases)
+[![GitHub Workflow Status (branch)](https://img.shields.io/github/actions/workflow/status/gammarer/aws-secure-bucket/release.yml?branch=main&label=release&style=flat-square)](https://github.com/gammarer/aws-secure-bucket/actions/workflows/release.yml)
+[![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/gammarer/aws-secure-bucket?sort=semver&style=flat-square)](https://github.com/gammarer/aws-secure-bucket/releases)
 
-# AWS Secure Bucket
+[![View on Construct Hub](https://constructs.dev/badge?package=@gammarer/aws-secure-bucket)](https://constructs.dev/packages/@gammarer/aws-secure-bucket)
 
 This is a Simple S3 Secure Bucket.
 
 * Bucket Access Control is Private
 * Public Read Access is false
 * Enforce SSL
 * All Block public access
@@ -70,16 +72,14 @@
   <groupId>com.gammarer</groupId>
   <artifactId>aws-secure-bucket</artifactId>
 </dependency>
 ```
 
 ## Example
 
-### TypeScript
-
 ```python
 import { SecureBucket } from '@gammarer/aws-secure-bucket';
 
 const bucket = new SecureBucket(stack, 'SecureBucket', {
   bucketName: 'example-secure-bucket',
 });
 ```
```

### Comparing `gammarer.aws-secure-bucket-1.1.9/README.md` & `gammarer.aws-secure-bucket-1.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-[![GitHub](https://img.shields.io/github/license/yicr/aws-secure-bucket?style=flat-square)](https://github.com/yicr/aws-secure-bucket/blob/main/LICENSE)
+# AWS Secure Bucket
+
+[![GitHub](https://img.shields.io/github/license/gammarer/aws-secure-bucket?style=flat-square)](https://github.com/gammarer/aws-secure-bucket/blob/main/LICENSE)
 [![npm (scoped)](https://img.shields.io/npm/v/@gammarer/aws-secure-bucket?style=flat-square)](https://www.npmjs.com/package/@gammarer/aws-secure-bucket)
 [![PyPI](https://img.shields.io/pypi/v/gammarer.aws-secure-bucket?style=flat-square)](https://pypi.org/project/gammarer.aws-secure-bucket/)
 [![Nuget](https://img.shields.io/nuget/v/Gammarer.CDK.AWS.SecureBucket?style=flat-square)](https://www.nuget.org/packages/Gammarer.CDK.AWS.SecureBucket/)
 [![Sonatype Nexus (Releases)](https://img.shields.io/nexus/r/com.gammarer/aws-secure-bucket?server=https%3A%2F%2Fs01.oss.sonatype.org%2F&style=flat-square)](https://s01.oss.sonatype.org/content/repositories/releases/com/gammarer/aws-secure-bucket/)
-[![GitHub Workflow Status (branch)](https://img.shields.io/github/actions/workflow/status/yicr/aws-secure-bucket/release.yml?branch=main&label=release&style=flat-square)](https://github.com/yicr/aws-secure-bucket/actions/workflows/release.yml)
-[![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/yicr/aws-secure-bucket?sort=semver&style=flat-square)](https://github.com/yicr/aws-secure-bucket/releases)
+[![GitHub Workflow Status (branch)](https://img.shields.io/github/actions/workflow/status/gammarer/aws-secure-bucket/release.yml?branch=main&label=release&style=flat-square)](https://github.com/gammarer/aws-secure-bucket/actions/workflows/release.yml)
+[![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/gammarer/aws-secure-bucket?sort=semver&style=flat-square)](https://github.com/gammarer/aws-secure-bucket/releases)
 
-# AWS Secure Bucket
+[![View on Construct Hub](https://constructs.dev/badge?package=@gammarer/aws-secure-bucket)](https://constructs.dev/packages/@gammarer/aws-secure-bucket)
 
 This is a Simple S3 Secure Bucket.
 
 * Bucket Access Control is Private
 * Public Read Access is false
 * Enforce SSL
 * All Block public access
@@ -47,16 +49,14 @@
   <groupId>com.gammarer</groupId>
   <artifactId>aws-secure-bucket</artifactId>
 </dependency>
 ```
 
 ## Example
 
-### TypeScript
-
 ```python
 import { SecureBucket } from '@gammarer/aws-secure-bucket';
 
 const bucket = new SecureBucket(stack, 'SecureBucket', {
   bucketName: 'example-secure-bucket',
 });
 ```
```

### Comparing `gammarer.aws-secure-bucket-1.1.9/setup.py` & `gammarer.aws-secure-bucket-1.2.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "gammarer.aws-secure-bucket",
-    "version": "1.1.9",
+    "version": "1.2.0",
     "description": "This is a Simple S3 Secure Bucket.",
     "license": "Apache-2.0",
     "url": "https://github.com/gammarer/aws-secure-bucket.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,25 +22,25 @@
     },
     "packages": [
         "gammarer.aws_secure_bucket",
         "gammarer.aws_secure_bucket._jsii"
     ],
     "package_data": {
         "gammarer.aws_secure_bucket._jsii": [
-            "aws-secure-bucket@1.1.9.jsii.tgz"
+            "aws-secure-bucket@1.2.0.jsii.tgz"
         ],
         "gammarer.aws_secure_bucket": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
         "aws-cdk-lib>=2.80.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "jsii>=1.94.0, <2.0.0",
+        "jsii>=1.96.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `gammarer.aws-secure-bucket-1.1.9/src/gammarer/aws_secure_bucket/__init__.py` & `gammarer.aws-secure-bucket-1.2.0/src/gammarer/aws_secure_bucket/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 '''
-[![GitHub](https://img.shields.io/github/license/yicr/aws-secure-bucket?style=flat-square)](https://github.com/yicr/aws-secure-bucket/blob/main/LICENSE)
+# AWS Secure Bucket
+
+[![GitHub](https://img.shields.io/github/license/gammarer/aws-secure-bucket?style=flat-square)](https://github.com/gammarer/aws-secure-bucket/blob/main/LICENSE)
 [![npm (scoped)](https://img.shields.io/npm/v/@gammarer/aws-secure-bucket?style=flat-square)](https://www.npmjs.com/package/@gammarer/aws-secure-bucket)
 [![PyPI](https://img.shields.io/pypi/v/gammarer.aws-secure-bucket?style=flat-square)](https://pypi.org/project/gammarer.aws-secure-bucket/)
 [![Nuget](https://img.shields.io/nuget/v/Gammarer.CDK.AWS.SecureBucket?style=flat-square)](https://www.nuget.org/packages/Gammarer.CDK.AWS.SecureBucket/)
 [![Sonatype Nexus (Releases)](https://img.shields.io/nexus/r/com.gammarer/aws-secure-bucket?server=https%3A%2F%2Fs01.oss.sonatype.org%2F&style=flat-square)](https://s01.oss.sonatype.org/content/repositories/releases/com/gammarer/aws-secure-bucket/)
-[![GitHub Workflow Status (branch)](https://img.shields.io/github/actions/workflow/status/yicr/aws-secure-bucket/release.yml?branch=main&label=release&style=flat-square)](https://github.com/yicr/aws-secure-bucket/actions/workflows/release.yml)
-[![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/yicr/aws-secure-bucket?sort=semver&style=flat-square)](https://github.com/yicr/aws-secure-bucket/releases)
+[![GitHub Workflow Status (branch)](https://img.shields.io/github/actions/workflow/status/gammarer/aws-secure-bucket/release.yml?branch=main&label=release&style=flat-square)](https://github.com/gammarer/aws-secure-bucket/actions/workflows/release.yml)
+[![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/gammarer/aws-secure-bucket?sort=semver&style=flat-square)](https://github.com/gammarer/aws-secure-bucket/releases)
 
-# AWS Secure Bucket
+[![View on Construct Hub](https://constructs.dev/badge?package=@gammarer/aws-secure-bucket)](https://constructs.dev/packages/@gammarer/aws-secure-bucket)
 
 This is a Simple S3 Secure Bucket.
 
 * Bucket Access Control is Private
 * Public Read Access is false
 * Enforce SSL
 * All Block public access
@@ -48,24 +50,25 @@
   <groupId>com.gammarer</groupId>
   <artifactId>aws-secure-bucket</artifactId>
 </dependency>
 ```
 
 ## Example
 
-### TypeScript
-
 ```python
 import { SecureBucket } from '@gammarer/aws-secure-bucket';
 
 const bucket = new SecureBucket(stack, 'SecureBucket', {
   bucketName: 'example-secure-bucket',
 });
 ```
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

### Comparing `gammarer.aws-secure-bucket-1.1.9/src/gammarer.aws_secure_bucket.egg-info/PKG-INFO` & `gammarer.aws-secure-bucket-1.2.0/src/gammarer.aws_secure_bucket.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-secure-bucket
-Version: 1.1.9
+Version: 1.2.0
 Summary: This is a Simple S3 Secure Bucket.
 Home-page: https://github.com/gammarer/aws-secure-bucket.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarer/aws-secure-bucket.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -17,23 +17,25 @@
 Classifier: Typing :: Typed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![GitHub](https://img.shields.io/github/license/yicr/aws-secure-bucket?style=flat-square)](https://github.com/yicr/aws-secure-bucket/blob/main/LICENSE)
+# AWS Secure Bucket
+
+[![GitHub](https://img.shields.io/github/license/gammarer/aws-secure-bucket?style=flat-square)](https://github.com/gammarer/aws-secure-bucket/blob/main/LICENSE)
 [![npm (scoped)](https://img.shields.io/npm/v/@gammarer/aws-secure-bucket?style=flat-square)](https://www.npmjs.com/package/@gammarer/aws-secure-bucket)
 [![PyPI](https://img.shields.io/pypi/v/gammarer.aws-secure-bucket?style=flat-square)](https://pypi.org/project/gammarer.aws-secure-bucket/)
 [![Nuget](https://img.shields.io/nuget/v/Gammarer.CDK.AWS.SecureBucket?style=flat-square)](https://www.nuget.org/packages/Gammarer.CDK.AWS.SecureBucket/)
 [![Sonatype Nexus (Releases)](https://img.shields.io/nexus/r/com.gammarer/aws-secure-bucket?server=https%3A%2F%2Fs01.oss.sonatype.org%2F&style=flat-square)](https://s01.oss.sonatype.org/content/repositories/releases/com/gammarer/aws-secure-bucket/)
-[![GitHub Workflow Status (branch)](https://img.shields.io/github/actions/workflow/status/yicr/aws-secure-bucket/release.yml?branch=main&label=release&style=flat-square)](https://github.com/yicr/aws-secure-bucket/actions/workflows/release.yml)
-[![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/yicr/aws-secure-bucket?sort=semver&style=flat-square)](https://github.com/yicr/aws-secure-bucket/releases)
+[![GitHub Workflow Status (branch)](https://img.shields.io/github/actions/workflow/status/gammarer/aws-secure-bucket/release.yml?branch=main&label=release&style=flat-square)](https://github.com/gammarer/aws-secure-bucket/actions/workflows/release.yml)
+[![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/gammarer/aws-secure-bucket?sort=semver&style=flat-square)](https://github.com/gammarer/aws-secure-bucket/releases)
 
-# AWS Secure Bucket
+[![View on Construct Hub](https://constructs.dev/badge?package=@gammarer/aws-secure-bucket)](https://constructs.dev/packages/@gammarer/aws-secure-bucket)
 
 This is a Simple S3 Secure Bucket.
 
 * Bucket Access Control is Private
 * Public Read Access is false
 * Enforce SSL
 * All Block public access
@@ -70,16 +72,14 @@
   <groupId>com.gammarer</groupId>
   <artifactId>aws-secure-bucket</artifactId>
 </dependency>
 ```
 
 ## Example
 
-### TypeScript
-
 ```python
 import { SecureBucket } from '@gammarer/aws-secure-bucket';
 
 const bucket = new SecureBucket(stack, 'SecureBucket', {
   bucketName: 'example-secure-bucket',
 });
 ```
```

### Comparing `gammarer.aws-secure-bucket-1.1.9/src/gammarer.aws_secure_bucket.egg-info/SOURCES.txt` & `gammarer.aws-secure-bucket-1.2.0/src/gammarer.aws_secure_bucket.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/gammarer.aws_secure_bucket.egg-info/SOURCES.txt
 src/gammarer.aws_secure_bucket.egg-info/dependency_links.txt
 src/gammarer.aws_secure_bucket.egg-info/requires.txt
 src/gammarer.aws_secure_bucket.egg-info/top_level.txt
 src/gammarer/aws_secure_bucket/__init__.py
 src/gammarer/aws_secure_bucket/py.typed
 src/gammarer/aws_secure_bucket/_jsii/__init__.py
-src/gammarer/aws_secure_bucket/_jsii/aws-secure-bucket@1.1.9.jsii.tgz
+src/gammarer/aws_secure_bucket/_jsii/aws-secure-bucket@1.2.0.jsii.tgz
```

