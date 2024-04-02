# Comparing `tmp/gammarer.aws-frontend-web-app-deploy-stack-1.1.2.tar.gz` & `tmp/gammarer.aws-frontend-web-app-deploy-stack-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gammarer.aws-frontend-web-app-deploy-stack-1.1.2.tar", last modified: Tue Mar 26 19:15:01 2024, max compression
+gzip compressed data, was "gammarer.aws-frontend-web-app-deploy-stack-1.1.4.tar", last modified: Tue Apr  2 19:15:51 2024, max compression
```

## Comparing `gammarer.aws-frontend-web-app-deploy-stack-1.1.2.tar` & `gammarer.aws-frontend-web-app-deploy-stack-1.1.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 19:15:01.327371 gammarer.aws-frontend-web-app-deploy-stack-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-03-26 19:14:48.000000 gammarer.aws-frontend-web-app-deploy-stack-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-26 19:14:48.000000 gammarer.aws-frontend-web-app-deploy-stack-1.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3957 2024-03-26 19:15:01.327371 gammarer.aws-frontend-web-app-deploy-stack-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-03-26 19:14:48.000000 gammarer.aws-frontend-web-app-deploy-stack-1.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-26 19:14:48.000000 gammarer.aws-frontend-web-app-deploy-stack-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 19:15:01.327371 gammarer.aws-frontend-web-app-deploy-stack-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-03-26 19:14:48.000000 gammarer.aws-frontend-web-app-deploy-stack-1.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 19:15:01.327371 gammarer.aws-frontend-web-app-deploy-stack-1.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 19:15:01.327371 gammarer.aws-frontend-web-app-deploy-stack-1.1.2/src/gammarer/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 19:15:01.327371 gammarer.aws-frontend-web-app-deploy-stack-1.1.2/src/gammarer/aws_frontend_web_app_deploy_stack/
--rw-r--r--   0 runner    (1001) docker     (127)    28187 2024-03-26 19:14:48.000000 gammarer.aws-frontend-web-app-deploy-stack-1.1.2/src/gammarer/aws_frontend_web_app_deploy_stack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 19:15:01.327371 gammarer.aws-frontend-web-app-deploy-stack-1.1.2/src/gammarer/aws_frontend_web_app_deploy_stack/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-03-26 19:14:48.000000 gammarer.aws-frontend-web-app-deploy-stack-1.1.2/src/gammarer/aws_frontend_web_app_deploy_stack/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36384 2024-03-26 19:14:48.000000 gammarer.aws-frontend-web-app-deploy-stack-1.1.2/src/gammarer/aws_frontend_web_app_deploy_stack/_jsii/aws-frontend-web-app-deploy-stack@1.1.2.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 19:14:48.000000 gammarer.aws-frontend-web-app-deploy-stack-1.1.2/src/gammarer/aws_frontend_web_app_deploy_stack/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 19:15:01.327371 gammarer.aws-frontend-web-app-deploy-stack-1.1.2/src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3957 2024-03-26 19:15:01.000000 gammarer.aws-frontend-web-app-deploy-stack-1.1.2/src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-03-26 19:15:01.000000 gammarer.aws-frontend-web-app-deploy-stack-1.1.2/src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 19:15:01.000000 gammarer.aws-frontend-web-app-deploy-stack-1.1.2/src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-03-26 19:15:01.000000 gammarer.aws-frontend-web-app-deploy-stack-1.1.2/src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-26 19:15:01.000000 gammarer.aws-frontend-web-app-deploy-stack-1.1.2/src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:15:51.046123 gammarer.aws-frontend-web-app-deploy-stack-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-02 19:15:34.000000 gammarer.aws-frontend-web-app-deploy-stack-1.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-02 19:15:34.000000 gammarer.aws-frontend-web-app-deploy-stack-1.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3957 2024-04-02 19:15:51.046123 gammarer.aws-frontend-web-app-deploy-stack-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-04-02 19:15:34.000000 gammarer.aws-frontend-web-app-deploy-stack-1.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-02 19:15:34.000000 gammarer.aws-frontend-web-app-deploy-stack-1.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 19:15:51.046123 gammarer.aws-frontend-web-app-deploy-stack-1.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-02 19:15:34.000000 gammarer.aws-frontend-web-app-deploy-stack-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:15:51.042123 gammarer.aws-frontend-web-app-deploy-stack-1.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:15:51.042123 gammarer.aws-frontend-web-app-deploy-stack-1.1.4/src/gammarer/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:15:51.046123 gammarer.aws-frontend-web-app-deploy-stack-1.1.4/src/gammarer/aws_frontend_web_app_deploy_stack/
+-rw-r--r--   0 runner    (1001) docker     (127)    28187 2024-04-02 19:15:34.000000 gammarer.aws-frontend-web-app-deploy-stack-1.1.4/src/gammarer/aws_frontend_web_app_deploy_stack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:15:51.046123 gammarer.aws-frontend-web-app-deploy-stack-1.1.4/src/gammarer/aws_frontend_web_app_deploy_stack/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-02 19:15:34.000000 gammarer.aws-frontend-web-app-deploy-stack-1.1.4/src/gammarer/aws_frontend_web_app_deploy_stack/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36387 2024-04-02 19:15:34.000000 gammarer.aws-frontend-web-app-deploy-stack-1.1.4/src/gammarer/aws_frontend_web_app_deploy_stack/_jsii/aws-frontend-web-app-deploy-stack@1.1.4.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 19:15:34.000000 gammarer.aws-frontend-web-app-deploy-stack-1.1.4/src/gammarer/aws_frontend_web_app_deploy_stack/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:15:51.046123 gammarer.aws-frontend-web-app-deploy-stack-1.1.4/src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3957 2024-04-02 19:15:51.000000 gammarer.aws-frontend-web-app-deploy-stack-1.1.4/src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-02 19:15:51.000000 gammarer.aws-frontend-web-app-deploy-stack-1.1.4/src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 19:15:51.000000 gammarer.aws-frontend-web-app-deploy-stack-1.1.4/src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-02 19:15:51.000000 gammarer.aws-frontend-web-app-deploy-stack-1.1.4/src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-02 19:15:51.000000 gammarer.aws-frontend-web-app-deploy-stack-1.1.4/src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/top_level.txt
```

### Comparing `gammarer.aws-frontend-web-app-deploy-stack-1.1.2/LICENSE` & `gammarer.aws-frontend-web-app-deploy-stack-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gammarer.aws-frontend-web-app-deploy-stack-1.1.2/PKG-INFO` & `gammarer.aws-frontend-web-app-deploy-stack-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-frontend-web-app-deploy-stack
-Version: 1.1.2
+Version: 1.1.4
 Summary: This is an AWS CDK Construct to make deploying a Frontend Web App (SPA) deploy to S3 behind CloudFront.
 Home-page: https://github.com/gammarer/aws-frontend-web-app-deploy-stack.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarer/aws-frontend-web-app-deploy-stack.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-frontend-web-app-deploy-stack-1.1.2/README.md` & `gammarer.aws-frontend-web-app-deploy-stack-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `gammarer.aws-frontend-web-app-deploy-stack-1.1.2/setup.py` & `gammarer.aws-frontend-web-app-deploy-stack-1.1.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "gammarer.aws-frontend-web-app-deploy-stack",
-    "version": "1.1.2",
+    "version": "1.1.4",
     "description": "This is an AWS CDK Construct to make deploying a Frontend Web App (SPA) deploy to S3 behind CloudFront.",
     "license": "Apache-2.0",
     "url": "https://github.com/gammarer/aws-frontend-web-app-deploy-stack.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "gammarer.aws_frontend_web_app_deploy_stack",
         "gammarer.aws_frontend_web_app_deploy_stack._jsii"
     ],
     "package_data": {
         "gammarer.aws_frontend_web_app_deploy_stack._jsii": [
-            "aws-frontend-web-app-deploy-stack@1.1.2.jsii.tgz"
+            "aws-frontend-web-app-deploy-stack@1.1.4.jsii.tgz"
         ],
         "gammarer.aws_frontend_web_app_deploy_stack": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `gammarer.aws-frontend-web-app-deploy-stack-1.1.2/src/gammarer/aws_frontend_web_app_deploy_stack/__init__.py` & `gammarer.aws-frontend-web-app-deploy-stack-1.1.4/src/gammarer/aws_frontend_web_app_deploy_stack/__init__.py`

 * *Files identical despite different names*

### Comparing `gammarer.aws-frontend-web-app-deploy-stack-1.1.2/src/gammarer/aws_frontend_web_app_deploy_stack/_jsii/__init__.py` & `gammarer.aws-frontend-web-app-deploy-stack-1.1.4/src/gammarer/aws_frontend_web_app_deploy_stack/_jsii/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 import constructs._jsii
 import gammarer.aws_secure_bucket._jsii
 import gammarer.aws_secure_cloudfront_origin_bucket._jsii
 import gammarer.aws_secure_frontend_web_app_cloudfront_distribution._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "@gammarer/aws-frontend-web-app-deploy-stack",
-    "1.1.2",
+    "1.1.4",
     __name__[0:-6],
-    "aws-frontend-web-app-deploy-stack@1.1.2.jsii.tgz",
+    "aws-frontend-web-app-deploy-stack@1.1.4.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `gammarer.aws-frontend-web-app-deploy-stack-1.1.2/src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/PKG-INFO` & `gammarer.aws-frontend-web-app-deploy-stack-1.1.4/src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-frontend-web-app-deploy-stack
-Version: 1.1.2
+Version: 1.1.4
 Summary: This is an AWS CDK Construct to make deploying a Frontend Web App (SPA) deploy to S3 behind CloudFront.
 Home-page: https://github.com/gammarer/aws-frontend-web-app-deploy-stack.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarer/aws-frontend-web-app-deploy-stack.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-frontend-web-app-deploy-stack-1.1.2/src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/SOURCES.txt` & `gammarer.aws-frontend-web-app-deploy-stack-1.1.4/src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/SOURCES.txt
 src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/dependency_links.txt
 src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/requires.txt
 src/gammarer.aws_frontend_web_app_deploy_stack.egg-info/top_level.txt
 src/gammarer/aws_frontend_web_app_deploy_stack/__init__.py
 src/gammarer/aws_frontend_web_app_deploy_stack/py.typed
 src/gammarer/aws_frontend_web_app_deploy_stack/_jsii/__init__.py
-src/gammarer/aws_frontend_web_app_deploy_stack/_jsii/aws-frontend-web-app-deploy-stack@1.1.2.jsii.tgz
+src/gammarer/aws_frontend_web_app_deploy_stack/_jsii/aws-frontend-web-app-deploy-stack@1.1.4.jsii.tgz
```

