# Comparing `tmp/etudatasphere-0.1.0.tar.gz` & `tmp/etudatasphere-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etudatasphere-0.1.0.tar", last modified: Wed Mar 27 20:06:09 2024, max compression
+gzip compressed data, was "etudatasphere-0.1.1.tar", last modified: Tue Apr  2 17:11:03 2024, max compression
```

## Comparing `etudatasphere-0.1.0.tar` & `etudatasphere-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-03-27 20:06:09.264876 etudatasphere-0.1.0/
--rw-rw-rw-   0        0        0     1110 2024-03-27 19:34:50.000000 etudatasphere-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      976 2024-03-27 20:06:09.263873 etudatasphere-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-03-27 19:48:47.000000 etudatasphere-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-03-27 20:06:09.239871 etudatasphere-0.1.0/etudatasphere/
--rw-rw-rw-   0        0        0        0 2024-03-27 19:31:46.000000 etudatasphere-0.1.0/etudatasphere/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-27 20:06:09.262882 etudatasphere-0.1.0/etudatasphere.egg-info/
--rw-rw-rw-   0        0        0      976 2024-03-27 20:06:09.000000 etudatasphere-0.1.0/etudatasphere.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2024-03-27 20:06:09.000000 etudatasphere-0.1.0/etudatasphere.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-27 20:06:09.000000 etudatasphere-0.1.0/etudatasphere.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-03-27 20:06:09.000000 etudatasphere-0.1.0/etudatasphere.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-03-27 20:06:09.000000 etudatasphere-0.1.0/etudatasphere.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-27 20:06:09.264876 etudatasphere-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1332 2024-03-27 19:51:23.000000 etudatasphere-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 17:11:03.739059 etudatasphere-0.1.1/
+-rw-rw-rw-   0        0        0     1110 2024-03-27 19:34:50.000000 etudatasphere-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      976 2024-04-02 17:11:03.739059 etudatasphere-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-03-27 19:48:47.000000 etudatasphere-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 17:11:03.707794 etudatasphere-0.1.1/etudatasphere/
+-rw-rw-rw-   0        0        0     8082 2024-04-02 17:05:48.000000 etudatasphere-0.1.1/etudatasphere/DataSphereManager.py
+-rw-rw-rw-   0        0        0       50 2024-04-02 17:06:36.000000 etudatasphere-0.1.1/etudatasphere/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 17:11:03.739059 etudatasphere-0.1.1/etudatasphere.egg-info/
+-rw-rw-rw-   0        0        0      976 2024-04-02 17:11:03.000000 etudatasphere-0.1.1/etudatasphere.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      271 2024-04-02 17:11:03.000000 etudatasphere-0.1.1/etudatasphere.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 17:11:03.000000 etudatasphere-0.1.1/etudatasphere.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-02 17:11:03.000000 etudatasphere-0.1.1/etudatasphere.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-02 17:11:03.000000 etudatasphere-0.1.1/etudatasphere.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-02 17:11:03.739059 etudatasphere-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1332 2024-04-02 17:10:55.000000 etudatasphere-0.1.1/setup.py
```

### Comparing `etudatasphere-0.1.0/LICENSE` & `etudatasphere-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `etudatasphere-0.1.0/PKG-INFO` & `etudatasphere-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etudatasphere
-Version: 0.1.0
+Version: 0.1.1
 Summary: etudatasphere: Simplifying Cloud Administration. Access Yandex.Cloud services with ease, automating routine tasks for resource management.
 Home-page: https://github.com/sesh00/etudatasphere
 Download-URL: https://github.com/sesh00/etudatasphere/archive/main.zip
 Author: sesh00
 Author-email: ernestrsage@gmail.com
 License: MIT License, see LICENSE file
 Classifier: Operating System :: OS Independent
```

### Comparing `etudatasphere-0.1.0/etudatasphere.egg-info/PKG-INFO` & `etudatasphere-0.1.1/etudatasphere.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etudatasphere
-Version: 0.1.0
+Version: 0.1.1
 Summary: etudatasphere: Simplifying Cloud Administration. Access Yandex.Cloud services with ease, automating routine tasks for resource management.
 Home-page: https://github.com/sesh00/etudatasphere
 Download-URL: https://github.com/sesh00/etudatasphere/archive/main.zip
 Author: sesh00
 Author-email: ernestrsage@gmail.com
 License: MIT License, see LICENSE file
 Classifier: Operating System :: OS Independent
```

### Comparing `etudatasphere-0.1.0/setup.py` & `etudatasphere-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from io import open
 from setuptools import setup
 
-version = '0.1.0'
+version = '0.1.1'
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='etudatasphere',
     version=version,
```

