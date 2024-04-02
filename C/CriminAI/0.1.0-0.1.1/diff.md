# Comparing `tmp/CriminAI-0.1.0.tar.gz` & `tmp/CriminAI-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CriminAI-0.1.0.tar", last modified: Tue Apr  2 15:03:30 2024, max compression
+gzip compressed data, was "CriminAI-0.1.1.tar", last modified: Tue Apr  2 15:15:00 2024, max compression
```

## Comparing `CriminAI-0.1.0.tar` & `CriminAI-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 matis      (501) staff       (20)        0 2024-04-02 15:03:30.249607 CriminAI-0.1.0/
-drwxr-xr-x   0 matis      (501) staff       (20)        0 2024-04-02 15:03:30.249362 CriminAI-0.1.0/CriminAI.egg-info/
--rw-r--r--   0 matis      (501) staff       (20)      548 2024-04-02 15:03:30.000000 CriminAI-0.1.0/CriminAI.egg-info/PKG-INFO
--rw-r--r--   0 matis      (501) staff       (20)      146 2024-04-02 15:03:30.000000 CriminAI-0.1.0/CriminAI.egg-info/SOURCES.txt
--rw-r--r--   0 matis      (501) staff       (20)        1 2024-04-02 15:03:30.000000 CriminAI-0.1.0/CriminAI.egg-info/dependency_links.txt
--rw-r--r--   0 matis      (501) staff       (20)        1 2024-04-02 15:03:30.000000 CriminAI-0.1.0/CriminAI.egg-info/top_level.txt
--rw-r--r--   0 matis      (501) staff       (20)      548 2024-04-02 15:03:30.249504 CriminAI-0.1.0/PKG-INFO
--rw-r--r--   0 matis      (501) staff       (20)      849 2024-03-04 14:49:08.000000 CriminAI-0.1.0/README.md
--rw-r--r--   0 matis      (501) staff       (20)       38 2024-04-02 15:03:30.249653 CriminAI-0.1.0/setup.cfg
--rw-r--r--   0 matis      (501) staff       (20)      546 2024-04-02 15:03:00.000000 CriminAI-0.1.0/setup.py
+drwxr-xr-x   0 matis      (501) staff       (20)        0 2024-04-02 15:15:00.448222 CriminAI-0.1.1/
+drwxr-xr-x   0 matis      (501) staff       (20)        0 2024-04-02 15:15:00.447978 CriminAI-0.1.1/CriminAI.egg-info/
+-rw-r--r--   0 matis      (501) staff       (20)      548 2024-04-02 15:15:00.000000 CriminAI-0.1.1/CriminAI.egg-info/PKG-INFO
+-rw-r--r--   0 matis      (501) staff       (20)      146 2024-04-02 15:15:00.000000 CriminAI-0.1.1/CriminAI.egg-info/SOURCES.txt
+-rw-r--r--   0 matis      (501) staff       (20)        1 2024-04-02 15:15:00.000000 CriminAI-0.1.1/CriminAI.egg-info/dependency_links.txt
+-rw-r--r--   0 matis      (501) staff       (20)        1 2024-04-02 15:15:00.000000 CriminAI-0.1.1/CriminAI.egg-info/top_level.txt
+-rw-r--r--   0 matis      (501) staff       (20)      548 2024-04-02 15:15:00.448123 CriminAI-0.1.1/PKG-INFO
+-rw-r--r--   0 matis      (501) staff       (20)      849 2024-03-04 14:49:08.000000 CriminAI-0.1.1/README.md
+-rw-r--r--   0 matis      (501) staff       (20)       38 2024-04-02 15:15:00.448265 CriminAI-0.1.1/setup.cfg
+-rw-r--r--   0 matis      (501) staff       (20)      546 2024-04-02 15:14:41.000000 CriminAI-0.1.1/setup.py
```

### Comparing `CriminAI-0.1.0/CriminAI.egg-info/PKG-INFO` & `CriminAI-0.1.1/CriminAI.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CriminAI
-Version: 0.1.0
+Version: 0.1.1
 Summary: CriminAI est un logiciel de génération de portraits robots par IA
 Home-page: UNKNOWN
 Author: ZOUARI Matis, PEREZ Lisa, SUTTER Clemence, ZHONG Zhihan
 Author-email: matis.zouari@insa-lyon.fr, lisa.perez@insa-lyon.fr, clemence.sutter@insa-lyon.fr, zhihan.zhong@insa-lyon.fr
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `CriminAI-0.1.0/PKG-INFO` & `CriminAI-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CriminAI
-Version: 0.1.0
+Version: 0.1.1
 Summary: CriminAI est un logiciel de génération de portraits robots par IA
 Home-page: UNKNOWN
 Author: ZOUARI Matis, PEREZ Lisa, SUTTER Clemence, ZHONG Zhihan
 Author-email: matis.zouari@insa-lyon.fr, lisa.perez@insa-lyon.fr, clemence.sutter@insa-lyon.fr, zhihan.zhong@insa-lyon.fr
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `CriminAI-0.1.0/README.md` & `CriminAI-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `CriminAI-0.1.0/setup.py` & `CriminAI-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
 name='CriminAI',
-version='0.1.0',
+version='0.1.1',
 author='ZOUARI Matis, PEREZ Lisa, SUTTER Clemence, ZHONG Zhihan',
 author_email='matis.zouari@insa-lyon.fr, lisa.perez@insa-lyon.fr, clemence.sutter@insa-lyon.fr, zhihan.zhong@insa-lyon.fr',
 description="CriminAI est un logiciel de génération de portraits robots par IA",
 packages=find_packages(),
 classifiers=[
 'Programming Language :: Python :: 3',
 'License :: OSI Approved :: MIT License',
```

