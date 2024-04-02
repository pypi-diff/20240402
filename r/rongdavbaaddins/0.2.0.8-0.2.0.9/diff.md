# Comparing `tmp/rongdavbaaddins-0.2.0.8.tar.gz` & `tmp/rongdavbaaddins-0.2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rongdavbaaddins-0.2.0.8.tar", last modified: Tue Aug 22 06:21:37 2023, max compression
+gzip compressed data, was "rongdavbaaddins-0.2.0.9.tar", last modified: Tue Aug 22 06:26:26 2023, max compression
```

## Comparing `rongdavbaaddins-0.2.0.8.tar` & `rongdavbaaddins-0.2.0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-08-22 06:21:37.100560 rongdavbaaddins-0.2.0.8/
--rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 rongdavbaaddins-0.2.0.8/LICENSE.txt
--rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 rongdavbaaddins-0.2.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0      417 2023-08-22 06:21:37.100560 rongdavbaaddins-0.2.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 rongdavbaaddins-0.2.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-08-22 06:21:37.067557 rongdavbaaddins-0.2.0.8/rongdaVbaAddins/
-drwxrwxrwx   0        0        0        0 2023-08-22 06:21:37.078564 rongdavbaaddins-0.2.0.8/rongdaVbaAddins/Function/
--rw-rw-rw-   0        0        0        0 2023-06-08 02:38:12.000000 rongdavbaaddins-0.2.0.8/rongdaVbaAddins/Function/__init__.py
--rw-rw-rw-   0        0        0    41472 2023-06-01 02:58:27.000000 rongdavbaaddins-0.2.0.8/rongdaVbaAddins/Function/minusFunction.pyd
--rw-rw-rw-   0        0        0      204 2023-06-01 03:01:41.000000 rongdavbaaddins-0.2.0.8/rongdaVbaAddins/Function/minusFunctionpy.py
--rw-rw-rw-   0        0        0  1893747 2023-08-18 05:34:34.000000 rongdavbaaddins-0.2.0.8/rongdaVbaAddins/RDaddins.xlam
--rw-rw-rw-   0        0        0     8192 2023-08-21 07:30:54.000000 rongdavbaaddins-0.2.0.8/rongdaVbaAddins/RecentTime.db
-drwxrwxrwx   0        0        0        0 2023-08-22 06:21:37.084562 rongdavbaaddins-0.2.0.8/rongdaVbaAddins/Ui/
--rw-rw-rw-   0        0        0        0 2023-06-08 02:38:04.000000 rongdavbaaddins-0.2.0.8/rongdaVbaAddins/Ui/__init__.py
--rw-rw-rw-   0        0        0    66560 2023-08-17 01:40:15.000000 rongdavbaaddins-0.2.0.8/rongdaVbaAddins/Ui/rongdaVbaAddinsUi.pyd
--rw-rw-rw-   0        0        0        0 2023-06-01 01:46:56.000000 rongdavbaaddins-0.2.0.8/rongdaVbaAddins/__init__.py
--rw-rw-rw-   0        0        0   236032 2023-08-17 02:15:36.000000 rongdavbaaddins-0.2.0.8/rongdaVbaAddins/registerCode.pyd
--rw-rw-rw-   0        0        0   199168 2023-08-22 06:20:51.000000 rongdavbaaddins-0.2.0.8/rongdaVbaAddins/rongdavbaaddins.pyd
--rw-rw-rw-   0        0        0      152 2023-08-22 06:02:10.000000 rongdavbaaddins-0.2.0.8/rongdaVbaAddins/runregiterCode.py
--rw-rw-rw-   0        0        0    29740 2023-08-18 05:34:34.000000 rongdavbaaddins-0.2.0.8/rongdaVbaAddins/文件处理类模板.xlsx
-drwxrwxrwx   0        0        0        0 2023-08-22 06:21:37.097561 rongdavbaaddins-0.2.0.8/rongdavbaaddins.egg-info/
--rw-rw-rw-   0        0        0      417 2023-08-22 06:21:36.000000 rongdavbaaddins-0.2.0.8/rongdavbaaddins.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      638 2023-08-22 06:21:37.000000 rongdavbaaddins-0.2.0.8/rongdavbaaddins.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-22 06:21:36.000000 rongdavbaaddins-0.2.0.8/rongdavbaaddins.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-08-22 06:21:36.000000 rongdavbaaddins-0.2.0.8/rongdavbaaddins.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      136 2023-08-22 06:21:37.102562 rongdavbaaddins-0.2.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1032 2023-08-22 06:21:26.000000 rongdavbaaddins-0.2.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-22 06:26:26.054377 rongdavbaaddins-0.2.0.9/
+-rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 rongdavbaaddins-0.2.0.9/LICENSE.txt
+-rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 rongdavbaaddins-0.2.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      417 2023-08-22 06:26:26.055377 rongdavbaaddins-0.2.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 rongdavbaaddins-0.2.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-08-22 06:26:25.987379 rongdavbaaddins-0.2.0.9/rongdaVbaAddins/
+drwxrwxrwx   0        0        0        0 2023-08-22 06:26:26.007388 rongdavbaaddins-0.2.0.9/rongdaVbaAddins/Function/
+-rw-rw-rw-   0        0        0        0 2023-06-08 02:38:12.000000 rongdavbaaddins-0.2.0.9/rongdaVbaAddins/Function/__init__.py
+-rw-rw-rw-   0        0        0    41472 2023-06-01 02:58:27.000000 rongdavbaaddins-0.2.0.9/rongdaVbaAddins/Function/minusFunction.pyd
+-rw-rw-rw-   0        0        0      204 2023-06-01 03:01:41.000000 rongdavbaaddins-0.2.0.9/rongdaVbaAddins/Function/minusFunctionpy.py
+-rw-rw-rw-   0        0        0  1893747 2023-08-18 05:34:34.000000 rongdavbaaddins-0.2.0.9/rongdaVbaAddins/RDaddins.xlam
+-rw-rw-rw-   0        0        0     8192 2023-08-21 07:30:54.000000 rongdavbaaddins-0.2.0.9/rongdaVbaAddins/RecentTime.db
+drwxrwxrwx   0        0        0        0 2023-08-22 06:26:26.020374 rongdavbaaddins-0.2.0.9/rongdaVbaAddins/Ui/
+-rw-rw-rw-   0        0        0        0 2023-06-08 02:38:04.000000 rongdavbaaddins-0.2.0.9/rongdaVbaAddins/Ui/__init__.py
+-rw-rw-rw-   0        0        0    66560 2023-08-17 01:40:15.000000 rongdavbaaddins-0.2.0.9/rongdaVbaAddins/Ui/rongdaVbaAddinsUi.pyd
+-rw-rw-rw-   0        0        0        0 2023-06-01 01:46:56.000000 rongdavbaaddins-0.2.0.9/rongdaVbaAddins/__init__.py
+-rw-rw-rw-   0        0        0   236032 2023-08-17 02:15:36.000000 rongdavbaaddins-0.2.0.9/rongdaVbaAddins/registerCode.pyd
+-rw-rw-rw-   0        0        0   199168 2023-08-22 06:24:54.000000 rongdavbaaddins-0.2.0.9/rongdaVbaAddins/rongdavbaaddins.pyd
+-rw-rw-rw-   0        0        0      152 2023-08-22 06:02:10.000000 rongdavbaaddins-0.2.0.9/rongdaVbaAddins/runregiterCode.py
+-rw-rw-rw-   0        0        0    29740 2023-08-18 05:34:34.000000 rongdavbaaddins-0.2.0.9/rongdaVbaAddins/文件处理类模板.xlsx
+drwxrwxrwx   0        0        0        0 2023-08-22 06:26:26.049378 rongdavbaaddins-0.2.0.9/rongdavbaaddins.egg-info/
+-rw-rw-rw-   0        0        0      417 2023-08-22 06:26:25.000000 rongdavbaaddins-0.2.0.9/rongdavbaaddins.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      638 2023-08-22 06:26:25.000000 rongdavbaaddins-0.2.0.9/rongdavbaaddins.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-22 06:26:25.000000 rongdavbaaddins-0.2.0.9/rongdavbaaddins.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-08-22 06:26:25.000000 rongdavbaaddins-0.2.0.9/rongdavbaaddins.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      136 2023-08-22 06:26:26.058375 rongdavbaaddins-0.2.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1032 2023-08-22 06:26:12.000000 rongdavbaaddins-0.2.0.9/setup.py
```

### Comparing `rongdavbaaddins-0.2.0.8/LICENSE.txt` & `rongdavbaaddins-0.2.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.2.0.8/rongdaVbaAddins/RDaddins.xlam` & `rongdavbaaddins-0.2.0.9/rongdaVbaAddins/RDaddins.xlam`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.2.0.8/rongdaVbaAddins/RecentTime.db` & `rongdavbaaddins-0.2.0.9/rongdaVbaAddins/RecentTime.db`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.2.0.8/rongdaVbaAddins/文件处理类模板.xlsx` & `rongdavbaaddins-0.2.0.9/rongdaVbaAddins/文件处理类模板.xlsx`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.2.0.8/rongdavbaaddins.egg-info/SOURCES.txt` & `rongdavbaaddins-0.2.0.9/rongdavbaaddins.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.2.0.8/setup.py` & `rongdavbaaddins-0.2.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #-*- coding:utf-8 -*-
 import os 
 from setuptools import setup, find_packages
 
 MAJOR = 0
 MINOR = 2
 PATCH = 0
-VERSION = f"{MAJOR}.{MINOR}.{PATCH}.8"
+VERSION = f"{MAJOR}.{MINOR}.{PATCH}.9"
 
 def get_install_requires():
     reqs = []
     return reqs
 setup(
 	name = "rongdavbaaddins",
     version=VERSION,
```

