# Comparing `tmp/alibabacloud_aiworkspace20210204-3.0.2.tar.gz` & `tmp/alibabacloud_aiworkspace20210204-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_aiworkspace20210204-3.0.2.tar", last modified: Sat Mar 23 17:07:06 2024, max compression
+gzip compressed data, was "dist/alibabacloud_aiworkspace20210204-3.0.3.tar", last modified: Tue Apr  2 17:14:52 2024, max compression
```

## Comparing `alibabacloud_aiworkspace20210204-3.0.2.tar` & `alibabacloud_aiworkspace20210204-3.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-23 17:07:06.000000 alibabacloud_aiworkspace20210204-3.0.2/
--rw-r--r--   0 root         (0) root         (0)      725 2024-03-23 17:07:06.000000 alibabacloud_aiworkspace20210204-3.0.2/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-03-23 17:07:06.000000 alibabacloud_aiworkspace20210204-3.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-03-23 17:07:06.000000 alibabacloud_aiworkspace20210204-3.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2457 2024-03-23 17:07:06.000000 alibabacloud_aiworkspace20210204-3.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1127 2024-03-23 17:07:06.000000 alibabacloud_aiworkspace20210204-3.0.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1212 2024-03-23 17:07:06.000000 alibabacloud_aiworkspace20210204-3.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-23 17:07:06.000000 alibabacloud_aiworkspace20210204-3.0.2/alibabacloud_aiworkspace20210204/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-23 17:07:06.000000 alibabacloud_aiworkspace20210204-3.0.2/alibabacloud_aiworkspace20210204/__init__.py
--rw-r--r--   0 root         (0) root         (0)   208532 2024-03-23 17:07:06.000000 alibabacloud_aiworkspace20210204-3.0.2/alibabacloud_aiworkspace20210204/client.py
--rw-r--r--   0 root         (0) root         (0)   325473 2024-03-23 17:07:06.000000 alibabacloud_aiworkspace20210204-3.0.2/alibabacloud_aiworkspace20210204/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-23 17:07:06.000000 alibabacloud_aiworkspace20210204-3.0.2/alibabacloud_aiworkspace20210204.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2457 2024-03-23 17:07:06.000000 alibabacloud_aiworkspace20210204-3.0.2/alibabacloud_aiworkspace20210204.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      484 2024-03-23 17:07:06.000000 alibabacloud_aiworkspace20210204-3.0.2/alibabacloud_aiworkspace20210204.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-23 17:07:06.000000 alibabacloud_aiworkspace20210204-3.0.2/alibabacloud_aiworkspace20210204.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-03-23 17:07:06.000000 alibabacloud_aiworkspace20210204-3.0.2/alibabacloud_aiworkspace20210204.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       33 2024-03-23 17:07:06.000000 alibabacloud_aiworkspace20210204-3.0.2/alibabacloud_aiworkspace20210204.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-23 17:07:06.000000 alibabacloud_aiworkspace20210204-3.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2651 2024-03-23 17:07:06.000000 alibabacloud_aiworkspace20210204-3.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:14:52.000000 alibabacloud_aiworkspace20210204-3.0.3/
+-rw-r--r--   0 root         (0) root         (0)      895 2024-04-02 17:14:52.000000 alibabacloud_aiworkspace20210204-3.0.3/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-02 17:14:52.000000 alibabacloud_aiworkspace20210204-3.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-02 17:14:52.000000 alibabacloud_aiworkspace20210204-3.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2457 2024-04-02 17:14:52.000000 alibabacloud_aiworkspace20210204-3.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1127 2024-04-02 17:14:52.000000 alibabacloud_aiworkspace20210204-3.0.3/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1212 2024-04-02 17:14:52.000000 alibabacloud_aiworkspace20210204-3.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:14:52.000000 alibabacloud_aiworkspace20210204-3.0.3/alibabacloud_aiworkspace20210204/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-02 17:14:52.000000 alibabacloud_aiworkspace20210204-3.0.3/alibabacloud_aiworkspace20210204/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   208726 2024-04-02 17:14:52.000000 alibabacloud_aiworkspace20210204-3.0.3/alibabacloud_aiworkspace20210204/client.py
+-rw-r--r--   0 root         (0) root         (0)   325691 2024-04-02 17:14:52.000000 alibabacloud_aiworkspace20210204-3.0.3/alibabacloud_aiworkspace20210204/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:14:52.000000 alibabacloud_aiworkspace20210204-3.0.3/alibabacloud_aiworkspace20210204.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2457 2024-04-02 17:14:52.000000 alibabacloud_aiworkspace20210204-3.0.3/alibabacloud_aiworkspace20210204.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      484 2024-04-02 17:14:52.000000 alibabacloud_aiworkspace20210204-3.0.3/alibabacloud_aiworkspace20210204.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-02 17:14:52.000000 alibabacloud_aiworkspace20210204-3.0.3/alibabacloud_aiworkspace20210204.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-02 17:14:52.000000 alibabacloud_aiworkspace20210204-3.0.3/alibabacloud_aiworkspace20210204.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2024-04-02 17:14:52.000000 alibabacloud_aiworkspace20210204-3.0.3/alibabacloud_aiworkspace20210204.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-02 17:14:52.000000 alibabacloud_aiworkspace20210204-3.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2651 2024-04-02 17:14:52.000000 alibabacloud_aiworkspace20210204-3.0.3/setup.py
```

### Comparing `alibabacloud_aiworkspace20210204-3.0.2/LICENSE` & `alibabacloud_aiworkspace20210204-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_aiworkspace20210204-3.0.2/PKG-INFO` & `alibabacloud_aiworkspace20210204-3.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_aiworkspace20210204
-Version: 3.0.2
+Version: 3.0.3
 Summary: Alibaba Cloud AIWorkSpace (20210204) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_aiworkspace20210204-3.0.2/README-CN.md` & `alibabacloud_aiworkspace20210204-3.0.3/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_aiworkspace20210204-3.0.2/README.md` & `alibabacloud_aiworkspace20210204-3.0.3/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_aiworkspace20210204-3.0.2/alibabacloud_aiworkspace20210204/client.py` & `alibabacloud_aiworkspace20210204-3.0.3/alibabacloud_aiworkspace20210204/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2643,14 +2643,16 @@
     ) -> aiwork_space_20210204_models.GetPermissionResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.accessibility):
             query['Accessibility'] = request.accessibility
         if not UtilClient.is_unset(request.creator):
             query['Creator'] = request.creator
+        if not UtilClient.is_unset(request.option):
+            query['Option'] = request.option
         if not UtilClient.is_unset(request.resource):
             query['Resource'] = request.resource
         req = open_api_models.OpenApiRequest(
             headers=headers,
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
@@ -2679,14 +2681,16 @@
     ) -> aiwork_space_20210204_models.GetPermissionResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.accessibility):
             query['Accessibility'] = request.accessibility
         if not UtilClient.is_unset(request.creator):
             query['Creator'] = request.creator
+        if not UtilClient.is_unset(request.option):
+            query['Option'] = request.option
         if not UtilClient.is_unset(request.resource):
             query['Resource'] = request.resource
         req = open_api_models.OpenApiRequest(
             headers=headers,
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
```

### Comparing `alibabacloud_aiworkspace20210204-3.0.2/alibabacloud_aiworkspace20210204/models.py` & `alibabacloud_aiworkspace20210204-3.0.3/alibabacloud_aiworkspace20210204/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -5506,18 +5506,20 @@
 
 
 class GetPermissionRequest(TeaModel):
     def __init__(
         self,
         accessibility: str = None,
         creator: str = None,
+        option: str = None,
         resource: str = None,
     ):
         self.accessibility = accessibility
         self.creator = creator
+        self.option = option
         self.resource = resource
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5525,24 +5527,28 @@
             return _map
 
         result = dict()
         if self.accessibility is not None:
             result['Accessibility'] = self.accessibility
         if self.creator is not None:
             result['Creator'] = self.creator
+        if self.option is not None:
+            result['Option'] = self.option
         if self.resource is not None:
             result['Resource'] = self.resource
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Accessibility') is not None:
             self.accessibility = m.get('Accessibility')
         if m.get('Creator') is not None:
             self.creator = m.get('Creator')
+        if m.get('Option') is not None:
+            self.option = m.get('Option')
         if m.get('Resource') is not None:
             self.resource = m.get('Resource')
         return self
 
 
 class GetPermissionResponseBodyPermissionRules(TeaModel):
     def __init__(
```

### Comparing `alibabacloud_aiworkspace20210204-3.0.2/alibabacloud_aiworkspace20210204.egg-info/PKG-INFO` & `alibabacloud_aiworkspace20210204-3.0.3/alibabacloud_aiworkspace20210204.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-aiworkspace20210204
-Version: 3.0.2
+Version: 3.0.3
 Summary: Alibaba Cloud AIWorkSpace (20210204) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_aiworkspace20210204-3.0.2/setup.py` & `alibabacloud_aiworkspace20210204-3.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_aiworkspace20210204.
 
-Created on 23/03/2024
+Created on 02/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_aiworkspace20210204"
 NAME = "alibabacloud_aiworkspace20210204" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud AIWorkSpace (20210204) SDK Library for Python"
```

