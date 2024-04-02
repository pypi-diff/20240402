# Comparing `tmp/firestore_wrapper-0.2.2.tar.gz` & `tmp/firestore_wrapper-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firestore_wrapper-0.2.2.tar", last modified: Sat Mar 30 21:12:45 2024, max compression
+gzip compressed data, was "firestore_wrapper-0.2.3.tar", last modified: Tue Apr  2 19:45:57 2024, max compression
```

## Comparing `firestore_wrapper-0.2.2.tar` & `firestore_wrapper-0.2.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 21:12:45.733950 firestore_wrapper-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-03-30 21:12:34.000000 firestore_wrapper-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3515 2024-03-30 21:12:45.733950 firestore_wrapper-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-03-30 21:12:34.000000 firestore_wrapper-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 21:12:45.733950 firestore_wrapper-0.2.2/firestore_wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-30 21:12:34.000000 firestore_wrapper-0.2.2/firestore_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-03-30 21:12:34.000000 firestore_wrapper-0.2.2/firestore_wrapper/backup_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-03-30 21:12:34.000000 firestore_wrapper-0.2.2/firestore_wrapper/collection_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-03-30 21:12:34.000000 firestore_wrapper-0.2.2/firestore_wrapper/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     7274 2024-03-30 21:12:34.000000 firestore_wrapper-0.2.2/firestore_wrapper/document_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-03-30 21:12:34.000000 firestore_wrapper-0.2.2/firestore_wrapper/firestore_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-03-30 21:12:34.000000 firestore_wrapper-0.2.2/firestore_wrapper/query_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-03-30 21:12:34.000000 firestore_wrapper-0.2.2/firestore_wrapper/schema_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-03-30 21:12:34.000000 firestore_wrapper-0.2.2/firestore_wrapper/utility_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 21:12:45.733950 firestore_wrapper-0.2.2/firestore_wrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3515 2024-03-30 21:12:45.000000 firestore_wrapper-0.2.2/firestore_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-03-30 21:12:45.000000 firestore_wrapper-0.2.2/firestore_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 21:12:45.000000 firestore_wrapper-0.2.2/firestore_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-30 21:12:45.000000 firestore_wrapper-0.2.2/firestore_wrapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-30 21:12:45.000000 firestore_wrapper-0.2.2/firestore_wrapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 21:12:45.733950 firestore_wrapper-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-03-30 21:12:34.000000 firestore_wrapper-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:45:57.126815 firestore_wrapper-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-02 19:45:47.000000 firestore_wrapper-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-04-02 19:45:57.126815 firestore_wrapper-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-04-02 19:45:47.000000 firestore_wrapper-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:45:57.126815 firestore_wrapper-0.2.3/firestore_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-02 19:45:47.000000 firestore_wrapper-0.2.3/firestore_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-04-02 19:45:47.000000 firestore_wrapper-0.2.3/firestore_wrapper/backup_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-04-02 19:45:47.000000 firestore_wrapper-0.2.3/firestore_wrapper/collection_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-02 19:45:47.000000 firestore_wrapper-0.2.3/firestore_wrapper/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7274 2024-04-02 19:45:47.000000 firestore_wrapper-0.2.3/firestore_wrapper/document_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-02 19:45:47.000000 firestore_wrapper-0.2.3/firestore_wrapper/firestore_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-04-02 19:45:47.000000 firestore_wrapper-0.2.3/firestore_wrapper/query_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-02 19:45:47.000000 firestore_wrapper-0.2.3/firestore_wrapper/schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-02 19:45:47.000000 firestore_wrapper-0.2.3/firestore_wrapper/utility_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:45:57.126815 firestore_wrapper-0.2.3/firestore_wrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-04-02 19:45:57.000000 firestore_wrapper-0.2.3/firestore_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-02 19:45:57.000000 firestore_wrapper-0.2.3/firestore_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 19:45:57.000000 firestore_wrapper-0.2.3/firestore_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-02 19:45:57.000000 firestore_wrapper-0.2.3/firestore_wrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-02 19:45:57.000000 firestore_wrapper-0.2.3/firestore_wrapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 19:45:57.126815 firestore_wrapper-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-02 19:45:47.000000 firestore_wrapper-0.2.3/setup.py
```

### Comparing `firestore_wrapper-0.2.2/LICENSE` & `firestore_wrapper-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `firestore_wrapper-0.2.2/PKG-INFO` & `firestore_wrapper-0.2.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: firestore_wrapper
-Version: 0.2.2
+Version: 0.2.3
 Summary: A custom wrapper for Google Firestore.
 Home-page: https://github.com/AntonioVentilii/firestore-wrapper
 Author: Antonio Ventilii
 Author-email: antonioventilii@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/AntonioVentilii/firestore-wrapper
 Project-URL: Issue Tracker, https://github.com/AntonioVentilii/firestore-wrapper/issues
+Keywords: firestore api wrapper database
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `firestore_wrapper-0.2.2/README.md` & `firestore_wrapper-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `firestore_wrapper-0.2.2/firestore_wrapper/backup_manager.py` & `firestore_wrapper-0.2.3/firestore_wrapper/backup_manager.py`

 * *Files identical despite different names*

### Comparing `firestore_wrapper-0.2.2/firestore_wrapper/collection_manager.py` & `firestore_wrapper-0.2.3/firestore_wrapper/collection_manager.py`

 * *Files identical despite different names*

### Comparing `firestore_wrapper-0.2.2/firestore_wrapper/core.py` & `firestore_wrapper-0.2.3/firestore_wrapper/core.py`

 * *Files identical despite different names*

### Comparing `firestore_wrapper-0.2.2/firestore_wrapper/document_manager.py` & `firestore_wrapper-0.2.3/firestore_wrapper/document_manager.py`

 * *Files identical despite different names*

### Comparing `firestore_wrapper-0.2.2/firestore_wrapper/firestore_base.py` & `firestore_wrapper-0.2.3/firestore_wrapper/firestore_base.py`

 * *Files identical despite different names*

### Comparing `firestore_wrapper-0.2.2/firestore_wrapper/query_manager.py` & `firestore_wrapper-0.2.3/firestore_wrapper/query_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from google.cloud.firestore_v1 import FieldFilter
+from google.cloud.firestore_v1.base_query import FieldFilter
 
 from .firestore_base import FirestoreBase
 
 
 class QueryManager(FirestoreBase):
 
     def __init__(self, credentials_path: str, database: str = None):
```

### Comparing `firestore_wrapper-0.2.2/firestore_wrapper/schema_utils.py` & `firestore_wrapper-0.2.3/firestore_wrapper/schema_utils.py`

 * *Files identical despite different names*

### Comparing `firestore_wrapper-0.2.2/firestore_wrapper/utility_manager.py` & `firestore_wrapper-0.2.3/firestore_wrapper/utility_manager.py`

 * *Files identical despite different names*

### Comparing `firestore_wrapper-0.2.2/firestore_wrapper.egg-info/PKG-INFO` & `firestore_wrapper-0.2.3/firestore_wrapper.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: firestore-wrapper
-Version: 0.2.2
+Version: 0.2.3
 Summary: A custom wrapper for Google Firestore.
 Home-page: https://github.com/AntonioVentilii/firestore-wrapper
 Author: Antonio Ventilii
 Author-email: antonioventilii@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/AntonioVentilii/firestore-wrapper
 Project-URL: Issue Tracker, https://github.com/AntonioVentilii/firestore-wrapper/issues
+Keywords: firestore api wrapper database
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `firestore_wrapper-0.2.2/firestore_wrapper.egg-info/SOURCES.txt` & `firestore_wrapper-0.2.3/firestore_wrapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `firestore_wrapper-0.2.2/setup.py` & `firestore_wrapper-0.2.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 from setuptools import find_packages, setup
 
 setup(
     name='firestore_wrapper',
-    version='0.2.2',
+    version='0.2.3',
     packages=find_packages(),
     description='A custom wrapper for Google Firestore.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Antonio Ventilii',
     author_email='antonioventilii@gmail.com',
     license='MIT',
     install_requires=[
-        'google-cloud-firestore>=2.1.0',
+        'google-cloud-firestore>=2.5.0',
         'schema',
     ],
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.7',
     url='https://github.com/AntonioVentilii/firestore-wrapper',
     project_urls={
         'Source Code': 'https://github.com/AntonioVentilii/firestore-wrapper',
         'Issue Tracker': 'https://github.com/AntonioVentilii/firestore-wrapper/issues',
-    }
+    },
+    keywords='firestore api wrapper database',
 )
```

