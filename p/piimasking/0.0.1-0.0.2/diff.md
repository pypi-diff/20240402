# Comparing `tmp/piimasking-0.0.1.tar.gz` & `tmp/piimasking-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piimasking-0.0.1.tar", last modified: Tue Apr  2 15:03:46 2024, max compression
+gzip compressed data, was "piimasking-0.0.2.tar", last modified: Tue Apr  2 17:21:59 2024, max compression
```

## Comparing `piimasking-0.0.1.tar` & `piimasking-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 fahadpatel   (501) staff       (20)        0 2024-04-02 15:03:46.568894 piimasking-0.0.1/
--rw-rw-r--   0 fahadpatel   (501) staff       (20)     1067 2024-04-02 14:22:52.000000 piimasking-0.0.1/LICENSE
--rw-rw-r--   0 fahadpatel   (501) staff       (20)      209 2024-04-02 14:51:11.000000 piimasking-0.0.1/MANIFEST.in
--rw-r--r--   0 fahadpatel   (501) staff       (20)     1789 2024-04-02 15:03:46.568797 piimasking-0.0.1/PKG-INFO
--rw-rw-r--   0 fahadpatel   (501) staff       (20)     1232 2024-04-02 14:14:05.000000 piimasking-0.0.1/README.md
-drwxr-xr-x   0 fahadpatel   (501) staff       (20)        0 2024-04-02 15:03:46.568568 piimasking-0.0.1/piimasking.egg-info/
--rw-r--r--   0 fahadpatel   (501) staff       (20)     1789 2024-04-02 15:03:46.000000 piimasking-0.0.1/piimasking.egg-info/PKG-INFO
--rw-r--r--   0 fahadpatel   (501) staff       (20)      232 2024-04-02 15:03:46.000000 piimasking-0.0.1/piimasking.egg-info/SOURCES.txt
--rw-r--r--   0 fahadpatel   (501) staff       (20)        1 2024-04-02 15:03:46.000000 piimasking-0.0.1/piimasking.egg-info/dependency_links.txt
--rw-r--r--   0 fahadpatel   (501) staff       (20)       57 2024-04-02 15:03:46.000000 piimasking-0.0.1/piimasking.egg-info/requires.txt
--rw-r--r--   0 fahadpatel   (501) staff       (20)        1 2024-04-02 15:03:46.000000 piimasking-0.0.1/piimasking.egg-info/top_level.txt
--rw-rw-r--   0 fahadpatel   (501) staff       (20)      107 2024-04-02 14:11:45.000000 piimasking-0.0.1/pyproject.toml
--rw-rw-r--   0 fahadpatel   (501) staff       (20)      522 2024-04-02 15:03:46.569190 piimasking-0.0.1/setup.cfg
--rw-rw-r--   0 fahadpatel   (501) staff       (20)      855 2024-04-02 14:47:54.000000 piimasking-0.0.1/setup.py
+drwxr-xr-x   0 fahadpatel   (501) staff       (20)        0 2024-04-02 17:21:59.736521 piimasking-0.0.2/
+-rw-rw-r--   0 fahadpatel   (501) staff       (20)     1067 2024-04-02 14:22:52.000000 piimasking-0.0.2/LICENSE
+-rw-rw-r--   0 fahadpatel   (501) staff       (20)      209 2024-04-02 14:51:11.000000 piimasking-0.0.2/MANIFEST.in
+-rw-r--r--   0 fahadpatel   (501) staff       (20)     1789 2024-04-02 17:21:59.736428 piimasking-0.0.2/PKG-INFO
+-rw-rw-r--   0 fahadpatel   (501) staff       (20)     1232 2024-04-02 14:14:05.000000 piimasking-0.0.2/README.md
+drwxr-xr-x   0 fahadpatel   (501) staff       (20)        0 2024-04-02 17:21:59.736123 piimasking-0.0.2/piimasking.egg-info/
+-rw-r--r--   0 fahadpatel   (501) staff       (20)     1789 2024-04-02 17:21:59.000000 piimasking-0.0.2/piimasking.egg-info/PKG-INFO
+-rw-r--r--   0 fahadpatel   (501) staff       (20)      232 2024-04-02 17:21:59.000000 piimasking-0.0.2/piimasking.egg-info/SOURCES.txt
+-rw-r--r--   0 fahadpatel   (501) staff       (20)        1 2024-04-02 17:21:59.000000 piimasking-0.0.2/piimasking.egg-info/dependency_links.txt
+-rw-r--r--   0 fahadpatel   (501) staff       (20)       57 2024-04-02 17:21:59.000000 piimasking-0.0.2/piimasking.egg-info/requires.txt
+-rw-r--r--   0 fahadpatel   (501) staff       (20)        1 2024-04-02 17:21:59.000000 piimasking-0.0.2/piimasking.egg-info/top_level.txt
+-rw-rw-r--   0 fahadpatel   (501) staff       (20)      107 2024-04-02 14:11:45.000000 piimasking-0.0.2/pyproject.toml
+-rw-rw-r--   0 fahadpatel   (501) staff       (20)      522 2024-04-02 17:21:59.736930 piimasking-0.0.2/setup.cfg
+-rw-rw-r--   0 fahadpatel   (501) staff       (20)      853 2024-04-02 17:20:43.000000 piimasking-0.0.2/setup.py
```

### Comparing `piimasking-0.0.1/LICENSE` & `piimasking-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `piimasking-0.0.1/PKG-INFO` & `piimasking-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piimasking
-Version: 0.0.1
+Version: 0.0.2
 Summary: This repository contains a Python program designed to execute Pii Masking
 Home-page: 
 Author: Amaan Patel
 Author-email: amaanpatel7868@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `piimasking-0.0.1/README.md` & `piimasking-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `piimasking-0.0.1/piimasking.egg-info/PKG-INFO` & `piimasking-0.0.2/piimasking.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piimasking
-Version: 0.0.1
+Version: 0.0.2
 Summary: This repository contains a Python program designed to execute Pii Masking
 Home-page: 
 Author: Amaan Patel
 Author-email: amaanpatel7868@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `piimasking-0.0.1/setup.cfg` & `piimasking-0.0.2/setup.cfg`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = piimasking
-version = 0.0.1
+version = 0.0.2
 author = Amaan Patel
 author_email = amaanpatel7868@gmail.com
 description = This repository contains a Python program designed to execute Pii masking
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3
```

### Comparing `piimasking-0.0.1/setup.py` & `piimasking-0.0.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
-with open("/Users/fahadpatel/Documents/piimasking/requirements.txt") as f:
+with open("/Users/fahadpatel/Documents/Mask-PII/requirements.txt") as f:
     required = f.read().splitlines()
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="piimasking",
-    version="0.0.1",
+    version="0.0.2",
     author="Amaan Patel", 
     author_email="amaanpatel7868@gmail.com",
     description=("This repository contains a Python program designed to execute Pii Masking"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     classifiers=[
```

