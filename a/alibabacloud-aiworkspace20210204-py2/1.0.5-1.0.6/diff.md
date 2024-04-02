# Comparing `tmp/alibabacloud_aiworkspace20210204_py2-1.0.5.tar.gz` & `tmp/alibabacloud_aiworkspace20210204_py2-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_aiworkspace20210204_py2-1.0.5.tar", last modified: Sat Mar 23 17:07:29 2024, max compression
+gzip compressed data, was "dist/alibabacloud_aiworkspace20210204_py2-1.0.6.tar", last modified: Tue Apr  2 17:14:18 2024, max compression
```

## Comparing `alibabacloud_aiworkspace20210204_py2-1.0.5.tar` & `alibabacloud_aiworkspace20210204_py2-1.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-23 17:07:29.000000 alibabacloud_aiworkspace20210204_py2-1.0.5/
--rw-r--r--   0 root         (0) root         (0)      375 2024-03-23 17:07:29.000000 alibabacloud_aiworkspace20210204_py2-1.0.5/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2024-03-23 17:07:29.000000 alibabacloud_aiworkspace20210204_py2-1.0.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2024-03-23 17:07:29.000000 alibabacloud_aiworkspace20210204_py2-1.0.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2520 2024-03-23 17:07:29.000000 alibabacloud_aiworkspace20210204_py2-1.0.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1057 2024-03-23 17:07:29.000000 alibabacloud_aiworkspace20210204_py2-1.0.5/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1140 2024-03-23 17:07:29.000000 alibabacloud_aiworkspace20210204_py2-1.0.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-23 17:07:29.000000 alibabacloud_aiworkspace20210204_py2-1.0.5/alibabacloud_aiworkspace20210204/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-23 17:07:29.000000 alibabacloud_aiworkspace20210204_py2-1.0.5/alibabacloud_aiworkspace20210204/__init__.py
--rw-r--r--   0 root         (0) root         (0)    86292 2024-03-23 17:07:29.000000 alibabacloud_aiworkspace20210204_py2-1.0.5/alibabacloud_aiworkspace20210204/client.py
--rw-r--r--   0 root         (0) root         (0)   326564 2024-03-23 17:07:29.000000 alibabacloud_aiworkspace20210204_py2-1.0.5/alibabacloud_aiworkspace20210204/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-23 17:07:29.000000 alibabacloud_aiworkspace20210204_py2-1.0.5/alibabacloud_aiworkspace20210204_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2520 2024-03-23 17:07:29.000000 alibabacloud_aiworkspace20210204_py2-1.0.5/alibabacloud_aiworkspace20210204_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      504 2024-03-23 17:07:29.000000 alibabacloud_aiworkspace20210204_py2-1.0.5/alibabacloud_aiworkspace20210204_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-23 17:07:29.000000 alibabacloud_aiworkspace20210204_py2-1.0.5/alibabacloud_aiworkspace20210204_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2024-03-23 17:07:29.000000 alibabacloud_aiworkspace20210204_py2-1.0.5/alibabacloud_aiworkspace20210204_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       33 2024-03-23 17:07:29.000000 alibabacloud_aiworkspace20210204_py2-1.0.5/alibabacloud_aiworkspace20210204_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-23 17:07:29.000000 alibabacloud_aiworkspace20210204_py2-1.0.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2943 2024-03-23 17:07:29.000000 alibabacloud_aiworkspace20210204_py2-1.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:14:18.000000 alibabacloud_aiworkspace20210204_py2-1.0.6/
+-rw-r--r--   0 root         (0) root         (0)      545 2024-04-02 17:14:18.000000 alibabacloud_aiworkspace20210204_py2-1.0.6/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2024-04-02 17:14:18.000000 alibabacloud_aiworkspace20210204_py2-1.0.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-02 17:14:18.000000 alibabacloud_aiworkspace20210204_py2-1.0.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2520 2024-04-02 17:14:18.000000 alibabacloud_aiworkspace20210204_py2-1.0.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1057 2024-04-02 17:14:18.000000 alibabacloud_aiworkspace20210204_py2-1.0.6/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1140 2024-04-02 17:14:18.000000 alibabacloud_aiworkspace20210204_py2-1.0.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:14:18.000000 alibabacloud_aiworkspace20210204_py2-1.0.6/alibabacloud_aiworkspace20210204/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-02 17:14:18.000000 alibabacloud_aiworkspace20210204_py2-1.0.6/alibabacloud_aiworkspace20210204/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    86389 2024-04-02 17:14:18.000000 alibabacloud_aiworkspace20210204_py2-1.0.6/alibabacloud_aiworkspace20210204/client.py
+-rw-r--r--   0 root         (0) root         (0)   326780 2024-04-02 17:14:18.000000 alibabacloud_aiworkspace20210204_py2-1.0.6/alibabacloud_aiworkspace20210204/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:14:18.000000 alibabacloud_aiworkspace20210204_py2-1.0.6/alibabacloud_aiworkspace20210204_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2520 2024-04-02 17:14:18.000000 alibabacloud_aiworkspace20210204_py2-1.0.6/alibabacloud_aiworkspace20210204_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      504 2024-04-02 17:14:18.000000 alibabacloud_aiworkspace20210204_py2-1.0.6/alibabacloud_aiworkspace20210204_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-02 17:14:18.000000 alibabacloud_aiworkspace20210204_py2-1.0.6/alibabacloud_aiworkspace20210204_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2024-04-02 17:14:18.000000 alibabacloud_aiworkspace20210204_py2-1.0.6/alibabacloud_aiworkspace20210204_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2024-04-02 17:14:18.000000 alibabacloud_aiworkspace20210204_py2-1.0.6/alibabacloud_aiworkspace20210204_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-02 17:14:18.000000 alibabacloud_aiworkspace20210204_py2-1.0.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2943 2024-04-02 17:14:18.000000 alibabacloud_aiworkspace20210204_py2-1.0.6/setup.py
```

### Comparing `alibabacloud_aiworkspace20210204_py2-1.0.5/LICENSE` & `alibabacloud_aiworkspace20210204_py2-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_aiworkspace20210204_py2-1.0.5/PKG-INFO` & `alibabacloud_aiworkspace20210204_py2-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_aiworkspace20210204_py2
-Version: 1.0.5
+Version: 1.0.6
 Summary: Alibaba Cloud AIWorkSpace (20210204) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_aiworkspace20210204_py2-1.0.5/README-CN.md` & `alibabacloud_aiworkspace20210204_py2-1.0.6/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_aiworkspace20210204_py2-1.0.5/README.md` & `alibabacloud_aiworkspace20210204_py2-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_aiworkspace20210204_py2-1.0.5/alibabacloud_aiworkspace20210204/client.py` & `alibabacloud_aiworkspace20210204_py2-1.0.6/alibabacloud_aiworkspace20210204/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1042,14 +1042,16 @@
     def get_permission_with_options(self, workspace_id, permission_code, request, headers, runtime):
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

### Comparing `alibabacloud_aiworkspace20210204_py2-1.0.5/alibabacloud_aiworkspace20210204/models.py` & `alibabacloud_aiworkspace20210204_py2-1.0.6/alibabacloud_aiworkspace20210204/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -4835,17 +4835,18 @@
         if m.get('body') is not None:
             temp_model = GetModelVersionResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class GetPermissionRequest(TeaModel):
-    def __init__(self, accessibility=None, creator=None, resource=None):
+    def __init__(self, accessibility=None, creator=None, option=None, resource=None):
         self.accessibility = accessibility  # type: str
         self.creator = creator  # type: str
+        self.option = option  # type: str
         self.resource = resource  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GetPermissionRequest, self).to_map()
@@ -4853,24 +4854,28 @@
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
 
     def from_map(self, m=None):
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
     def __init__(self, accessibility=None, entity_access_type=None):
```

### Comparing `alibabacloud_aiworkspace20210204_py2-1.0.5/alibabacloud_aiworkspace20210204_py2.egg-info/PKG-INFO` & `alibabacloud_aiworkspace20210204_py2-1.0.6/alibabacloud_aiworkspace20210204_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-aiworkspace20210204-py2
-Version: 1.0.5
+Version: 1.0.6
 Summary: Alibaba Cloud AIWorkSpace (20210204) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_aiworkspace20210204_py2-1.0.5/setup.py` & `alibabacloud_aiworkspace20210204_py2-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_aiworkspace20210204_py2.
 
-Created on 23/03/2024
+Created on 02/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_aiworkspace20210204"
 NAME = "alibabacloud_aiworkspace20210204_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud AIWorkSpace (20210204) SDK Library for Python2"
```

