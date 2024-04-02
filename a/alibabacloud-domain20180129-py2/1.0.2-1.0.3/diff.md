# Comparing `tmp/alibabacloud_domain20180129_py2-1.0.2.tar.gz` & `tmp/alibabacloud_domain20180129_py2-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_domain20180129_py2-1.0.2.tar", last modified: Wed Mar 20 17:20:01 2024, max compression
+gzip compressed data, was "dist/alibabacloud_domain20180129_py2-1.0.3.tar", last modified: Tue Apr  2 17:13:46 2024, max compression
```

## Comparing `alibabacloud_domain20180129_py2-1.0.2.tar` & `alibabacloud_domain20180129_py2-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 17:20:01.000000 alibabacloud_domain20180129_py2-1.0.2/
--rw-r--r--   0 root         (0) root         (0)      140 2024-03-20 17:20:00.000000 alibabacloud_domain20180129_py2-1.0.2/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2024-03-20 17:20:00.000000 alibabacloud_domain20180129_py2-1.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2024-03-20 17:20:00.000000 alibabacloud_domain20180129_py2-1.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2491 2024-03-20 17:20:01.000000 alibabacloud_domain20180129_py2-1.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1042 2024-03-20 17:20:00.000000 alibabacloud_domain20180129_py2-1.0.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1125 2024-03-20 17:20:00.000000 alibabacloud_domain20180129_py2-1.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 17:20:01.000000 alibabacloud_domain20180129_py2-1.0.2/alibabacloud_domain20180129/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-20 17:20:00.000000 alibabacloud_domain20180129_py2-1.0.2/alibabacloud_domain20180129/__init__.py
--rw-r--r--   0 root         (0) root         (0)   201923 2024-03-20 17:20:00.000000 alibabacloud_domain20180129_py2-1.0.2/alibabacloud_domain20180129/client.py
--rw-r--r--   0 root         (0) root         (0)   826358 2024-03-20 17:20:00.000000 alibabacloud_domain20180129_py2-1.0.2/alibabacloud_domain20180129/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 17:20:01.000000 alibabacloud_domain20180129_py2-1.0.2/alibabacloud_domain20180129_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2491 2024-03-20 17:20:01.000000 alibabacloud_domain20180129_py2-1.0.2/alibabacloud_domain20180129_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      464 2024-03-20 17:20:01.000000 alibabacloud_domain20180129_py2-1.0.2/alibabacloud_domain20180129_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-20 17:20:01.000000 alibabacloud_domain20180129_py2-1.0.2/alibabacloud_domain20180129_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2024-03-20 17:20:01.000000 alibabacloud_domain20180129_py2-1.0.2/alibabacloud_domain20180129_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       28 2024-03-20 17:20:01.000000 alibabacloud_domain20180129_py2-1.0.2/alibabacloud_domain20180129_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-20 17:20:01.000000 alibabacloud_domain20180129_py2-1.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2919 2024-03-20 17:20:00.000000 alibabacloud_domain20180129_py2-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:13:46.000000 alibabacloud_domain20180129_py2-1.0.3/
+-rw-r--r--   0 root         (0) root         (0)      331 2024-04-02 17:13:46.000000 alibabacloud_domain20180129_py2-1.0.3/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2024-04-02 17:13:46.000000 alibabacloud_domain20180129_py2-1.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-02 17:13:46.000000 alibabacloud_domain20180129_py2-1.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2491 2024-04-02 17:13:46.000000 alibabacloud_domain20180129_py2-1.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1042 2024-04-02 17:13:46.000000 alibabacloud_domain20180129_py2-1.0.3/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1125 2024-04-02 17:13:46.000000 alibabacloud_domain20180129_py2-1.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:13:46.000000 alibabacloud_domain20180129_py2-1.0.3/alibabacloud_domain20180129/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-02 17:13:46.000000 alibabacloud_domain20180129_py2-1.0.3/alibabacloud_domain20180129/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   201923 2024-04-02 17:13:46.000000 alibabacloud_domain20180129_py2-1.0.3/alibabacloud_domain20180129/client.py
+-rw-r--r--   0 root         (0) root         (0)   826358 2024-04-02 17:13:46.000000 alibabacloud_domain20180129_py2-1.0.3/alibabacloud_domain20180129/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:13:46.000000 alibabacloud_domain20180129_py2-1.0.3/alibabacloud_domain20180129_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2491 2024-04-02 17:13:46.000000 alibabacloud_domain20180129_py2-1.0.3/alibabacloud_domain20180129_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      464 2024-04-02 17:13:46.000000 alibabacloud_domain20180129_py2-1.0.3/alibabacloud_domain20180129_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-02 17:13:46.000000 alibabacloud_domain20180129_py2-1.0.3/alibabacloud_domain20180129_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2024-04-02 17:13:46.000000 alibabacloud_domain20180129_py2-1.0.3/alibabacloud_domain20180129_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-02 17:13:46.000000 alibabacloud_domain20180129_py2-1.0.3/alibabacloud_domain20180129_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-02 17:13:46.000000 alibabacloud_domain20180129_py2-1.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2919 2024-04-02 17:13:46.000000 alibabacloud_domain20180129_py2-1.0.3/setup.py
```

### Comparing `alibabacloud_domain20180129_py2-1.0.2/LICENSE` & `alibabacloud_domain20180129_py2-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_domain20180129_py2-1.0.2/PKG-INFO` & `alibabacloud_domain20180129_py2-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_domain20180129_py2
-Version: 1.0.2
+Version: 1.0.3
 Summary: Alibaba Cloud Domains (20180129) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_domain20180129_py2-1.0.2/README-CN.md` & `alibabacloud_domain20180129_py2-1.0.3/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_domain20180129_py2-1.0.2/README.md` & `alibabacloud_domain20180129_py2-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_domain20180129_py2-1.0.2/alibabacloud_domain20180129/client.py` & `alibabacloud_domain20180129_py2-1.0.3/alibabacloud_domain20180129/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_domain20180129_py2-1.0.2/alibabacloud_domain20180129/models.py` & `alibabacloud_domain20180129_py2-1.0.3/alibabacloud_domain20180129/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_domain20180129_py2-1.0.2/alibabacloud_domain20180129_py2.egg-info/PKG-INFO` & `alibabacloud_domain20180129_py2-1.0.3/alibabacloud_domain20180129_py2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-domain20180129-py2
-Version: 1.0.2
+Version: 1.0.3
 Summary: Alibaba Cloud Domains (20180129) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_domain20180129_py2-1.0.2/setup.py` & `alibabacloud_domain20180129_py2-1.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_domain20180129_py2.
 
-Created on 20/03/2024
+Created on 02/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_domain20180129"
 NAME = "alibabacloud_domain20180129_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Domains (20180129) SDK Library for Python2"
```

