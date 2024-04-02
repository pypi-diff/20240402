# Comparing `tmp/jblibaws-1.2.8.tar.gz` & `tmp/jblibaws-1.2.80.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jblibaws-1.2.8.tar", last modified: Tue Apr  2 15:27:59 2024, max compression
+gzip compressed data, was "jblibaws-1.2.80.tar", last modified: Tue Apr  2 15:32:27 2024, max compression
```

## Comparing `jblibaws-1.2.8.tar` & `jblibaws-1.2.80.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 justbard  (1000) justbard  (1000)        0 2024-04-02 15:27:59.031355 jblibaws-1.2.8/
--rw-r--r--   0 justbard  (1000) justbard  (1000)     1074 2022-10-10 13:27:49.000000 jblibaws-1.2.8/LICENSE
--rw-r--r--   0 justbard  (1000) justbard  (1000)     4510 2024-04-02 15:27:59.030355 jblibaws-1.2.8/PKG-INFO
--rw-r--r--   0 justbard  (1000) justbard  (1000)     4111 2024-03-24 19:31:31.000000 jblibaws-1.2.8/README.md
-drwxr-xr-x   0 justbard  (1000) justbard  (1000)        0 2024-04-02 15:27:59.029355 jblibaws-1.2.8/jblibaws/
--rw-r--r--   0 justbard  (1000) justbard  (1000)       63 2024-03-24 20:19:06.000000 jblibaws-1.2.8/jblibaws/__init__.py
-drwxr-xr-x   0 justbard  (1000) justbard  (1000)        0 2024-04-02 15:27:59.030355 jblibaws-1.2.8/jblibaws/aws/
--rw-r--r--   0 justbard  (1000) justbard  (1000)       76 2024-03-24 20:19:06.000000 jblibaws-1.2.8/jblibaws/aws/__init__.py
--rw-r--r--   0 justbard  (1000) justbard  (1000)     1215 2024-03-24 20:19:06.000000 jblibaws-1.2.8/jblibaws/aws/cognito.py
--rw-r--r--   0 justbard  (1000) justbard  (1000)    16132 2024-04-02 15:27:36.000000 jblibaws-1.2.8/jblibaws/aws/dynamodb.py
--rw-r--r--   0 justbard  (1000) justbard  (1000)     2182 2024-03-24 20:19:06.000000 jblibaws-1.2.8/jblibaws/aws/secretsManager.py
-drwxr-xr-x   0 justbard  (1000) justbard  (1000)        0 2024-04-02 15:27:59.030355 jblibaws-1.2.8/jblibaws/dict_tools/
--rw-r--r--   0 justbard  (1000) justbard  (1000)       25 2024-03-24 20:19:06.000000 jblibaws-1.2.8/jblibaws/dict_tools/__init__.py
--rw-r--r--   0 justbard  (1000) justbard  (1000)      235 2024-03-24 20:19:06.000000 jblibaws-1.2.8/jblibaws/dict_tools/dict_tools.py
-drwxr-xr-x   0 justbard  (1000) justbard  (1000)        0 2024-04-02 15:27:59.030355 jblibaws-1.2.8/jblibaws.egg-info/
--rw-r--r--   0 justbard  (1000) justbard  (1000)     4510 2024-04-02 15:27:59.000000 jblibaws-1.2.8/jblibaws.egg-info/PKG-INFO
--rw-r--r--   0 justbard  (1000) justbard  (1000)      346 2024-04-02 15:27:59.000000 jblibaws-1.2.8/jblibaws.egg-info/SOURCES.txt
--rw-r--r--   0 justbard  (1000) justbard  (1000)        1 2024-04-02 15:27:59.000000 jblibaws-1.2.8/jblibaws.egg-info/dependency_links.txt
--rw-r--r--   0 justbard  (1000) justbard  (1000)        9 2024-04-02 15:27:59.000000 jblibaws-1.2.8/jblibaws.egg-info/top_level.txt
--rw-r--r--   0 justbard  (1000) justbard  (1000)       38 2024-04-02 15:27:59.031355 jblibaws-1.2.8/setup.cfg
--rw-r--r--   0 justbard  (1000) justbard  (1000)      777 2024-04-02 15:27:47.000000 jblibaws-1.2.8/setup.py
+drwxr-xr-x   0 justbard  (1000) justbard  (1000)        0 2024-04-02 15:32:27.694585 jblibaws-1.2.80/
+-rw-r--r--   0 justbard  (1000) justbard  (1000)     1074 2022-10-10 13:27:49.000000 jblibaws-1.2.80/LICENSE
+-rw-r--r--   0 justbard  (1000) justbard  (1000)     4511 2024-04-02 15:32:27.694585 jblibaws-1.2.80/PKG-INFO
+-rw-r--r--   0 justbard  (1000) justbard  (1000)     4111 2024-03-24 19:31:31.000000 jblibaws-1.2.80/README.md
+drwxr-xr-x   0 justbard  (1000) justbard  (1000)        0 2024-04-02 15:32:27.693585 jblibaws-1.2.80/jblibaws/
+-rw-r--r--   0 justbard  (1000) justbard  (1000)       63 2024-03-24 20:19:06.000000 jblibaws-1.2.80/jblibaws/__init__.py
+drwxr-xr-x   0 justbard  (1000) justbard  (1000)        0 2024-04-02 15:32:27.694585 jblibaws-1.2.80/jblibaws/aws/
+-rw-r--r--   0 justbard  (1000) justbard  (1000)       76 2024-03-24 20:19:06.000000 jblibaws-1.2.80/jblibaws/aws/__init__.py
+-rw-r--r--   0 justbard  (1000) justbard  (1000)     1215 2024-03-24 20:19:06.000000 jblibaws-1.2.80/jblibaws/aws/cognito.py
+-rw-r--r--   0 justbard  (1000) justbard  (1000)    16132 2024-04-02 15:27:36.000000 jblibaws-1.2.80/jblibaws/aws/dynamodb.py
+-rw-r--r--   0 justbard  (1000) justbard  (1000)     2182 2024-03-24 20:19:06.000000 jblibaws-1.2.80/jblibaws/aws/secretsManager.py
+drwxr-xr-x   0 justbard  (1000) justbard  (1000)        0 2024-04-02 15:32:27.694585 jblibaws-1.2.80/jblibaws/dict_tools/
+-rw-r--r--   0 justbard  (1000) justbard  (1000)       25 2024-03-24 20:19:06.000000 jblibaws-1.2.80/jblibaws/dict_tools/__init__.py
+-rw-r--r--   0 justbard  (1000) justbard  (1000)      235 2024-03-24 20:19:06.000000 jblibaws-1.2.80/jblibaws/dict_tools/dict_tools.py
+drwxr-xr-x   0 justbard  (1000) justbard  (1000)        0 2024-04-02 15:32:27.694585 jblibaws-1.2.80/jblibaws.egg-info/
+-rw-r--r--   0 justbard  (1000) justbard  (1000)     4511 2024-04-02 15:32:27.000000 jblibaws-1.2.80/jblibaws.egg-info/PKG-INFO
+-rw-r--r--   0 justbard  (1000) justbard  (1000)      346 2024-04-02 15:32:27.000000 jblibaws-1.2.80/jblibaws.egg-info/SOURCES.txt
+-rw-r--r--   0 justbard  (1000) justbard  (1000)        1 2024-04-02 15:32:27.000000 jblibaws-1.2.80/jblibaws.egg-info/dependency_links.txt
+-rw-r--r--   0 justbard  (1000) justbard  (1000)        9 2024-04-02 15:32:27.000000 jblibaws-1.2.80/jblibaws.egg-info/top_level.txt
+-rw-r--r--   0 justbard  (1000) justbard  (1000)       38 2024-04-02 15:32:27.694585 jblibaws-1.2.80/setup.cfg
+-rw-r--r--   0 justbard  (1000) justbard  (1000)      778 2024-04-02 15:32:22.000000 jblibaws-1.2.80/setup.py
```

### Comparing `jblibaws-1.2.8/LICENSE` & `jblibaws-1.2.80/LICENSE`

 * *Files identical despite different names*

### Comparing `jblibaws-1.2.8/PKG-INFO` & `jblibaws-1.2.80/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jblibaws
-Version: 1.2.8
+Version: 1.2.80
 Summary: JustBard's Python based AWS Utilities
 Home-page: https://justbardtech.com
 Author: Justin Bard
 Author-email: JustinBard@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `jblibaws-1.2.8/README.md` & `jblibaws-1.2.80/README.md`

 * *Files identical despite different names*

### Comparing `jblibaws-1.2.8/jblibaws/aws/cognito.py` & `jblibaws-1.2.80/jblibaws/aws/cognito.py`

 * *Files identical despite different names*

### Comparing `jblibaws-1.2.8/jblibaws/aws/dynamodb.py` & `jblibaws-1.2.80/jblibaws/aws/dynamodb.py`

 * *Files identical despite different names*

### Comparing `jblibaws-1.2.8/jblibaws/aws/secretsManager.py` & `jblibaws-1.2.80/jblibaws/aws/secretsManager.py`

 * *Files identical despite different names*

### Comparing `jblibaws-1.2.8/jblibaws.egg-info/PKG-INFO` & `jblibaws-1.2.80/jblibaws.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jblibaws
-Version: 1.2.8
+Version: 1.2.80
 Summary: JustBard's Python based AWS Utilities
 Home-page: https://justbardtech.com
 Author: Justin Bard
 Author-email: JustinBard@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `jblibaws-1.2.8/setup.py` & `jblibaws-1.2.80/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(name='jblibaws',
-                version='1.2.8',
+                version='1.2.80',
                 description='JustBard\'s Python based AWS Utilities',
                 long_description=long_description,
                 long_description_content_type="text/markdown",
                 author='Justin Bard',
                 author_email='JustinBard@gmail.com',
                 url='https://justbardtech.com',
                 packages=setuptools.find_packages(),
```

