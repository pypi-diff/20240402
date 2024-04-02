# Comparing `tmp/pyclipmgr-2.7.tar.gz` & `tmp/pyclipmgr-2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyclipmgr-2.7.tar", last modified: Tue Apr  2 02:18:10 2024, max compression
+gzip compressed data, was "pyclipmgr-2.8.tar", last modified: Tue Apr  2 02:19:51 2024, max compression
```

## Comparing `pyclipmgr-2.7.tar` & `pyclipmgr-2.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 mohamed   (1000) mohamed   (1000)        0 2024-04-02 02:18:10.819784 pyclipmgr-2.7/
--rw-r--r--   0 mohamed   (1000) mohamed   (1000)     1384 2024-04-02 02:18:10.819784 pyclipmgr-2.7/PKG-INFO
--rw-r--r--   0 mohamed   (1000) mohamed   (1000)     1048 2024-04-02 01:51:33.000000 pyclipmgr-2.7/README.md
-drwxr-xr-x   0 mohamed   (1000) mohamed   (1000)        0 2024-04-02 02:18:10.816451 pyclipmgr-2.7/pyclipmgr.egg-info/
--rw-r--r--   0 mohamed   (1000) mohamed   (1000)     1384 2024-04-02 02:18:10.000000 pyclipmgr-2.7/pyclipmgr.egg-info/PKG-INFO
--rw-r--r--   0 mohamed   (1000) mohamed   (1000)      199 2024-04-02 02:18:10.000000 pyclipmgr-2.7/pyclipmgr.egg-info/SOURCES.txt
--rw-r--r--   0 mohamed   (1000) mohamed   (1000)        1 2024-04-02 02:18:10.000000 pyclipmgr-2.7/pyclipmgr.egg-info/dependency_links.txt
--rw-r--r--   0 mohamed   (1000) mohamed   (1000)       84 2024-04-02 02:18:10.000000 pyclipmgr-2.7/pyclipmgr.egg-info/entry_points.txt
--rw-r--r--   0 mohamed   (1000) mohamed   (1000)        1 2024-04-02 02:18:10.000000 pyclipmgr-2.7/pyclipmgr.egg-info/top_level.txt
--rw-r--r--   0 mohamed   (1000) mohamed   (1000)     1308 2024-04-02 02:17:57.000000 pyclipmgr-2.7/pyclipmgr.py
--rw-r--r--   0 mohamed   (1000) mohamed   (1000)       38 2024-04-02 02:18:10.819784 pyclipmgr-2.7/setup.cfg
--rw-r--r--   0 mohamed   (1000) mohamed   (1000)      753 2024-04-02 02:18:05.000000 pyclipmgr-2.7/setup.py
+drwxr-xr-x   0 mohamed   (1000) mohamed   (1000)        0 2024-04-02 02:19:51.331761 pyclipmgr-2.8/
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)     1384 2024-04-02 02:19:51.331761 pyclipmgr-2.8/PKG-INFO
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)     1048 2024-04-02 01:51:33.000000 pyclipmgr-2.8/README.md
+drwxr-xr-x   0 mohamed   (1000) mohamed   (1000)        0 2024-04-02 02:19:51.331761 pyclipmgr-2.8/pyclipmgr.egg-info/
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)     1384 2024-04-02 02:19:51.000000 pyclipmgr-2.8/pyclipmgr.egg-info/PKG-INFO
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)      199 2024-04-02 02:19:51.000000 pyclipmgr-2.8/pyclipmgr.egg-info/SOURCES.txt
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)        1 2024-04-02 02:19:51.000000 pyclipmgr-2.8/pyclipmgr.egg-info/dependency_links.txt
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)       79 2024-04-02 02:19:51.000000 pyclipmgr-2.8/pyclipmgr.egg-info/entry_points.txt
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)        1 2024-04-02 02:19:51.000000 pyclipmgr-2.8/pyclipmgr.egg-info/top_level.txt
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)     1308 2024-04-02 02:17:57.000000 pyclipmgr-2.8/pyclipmgr.py
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)       38 2024-04-02 02:19:51.331761 pyclipmgr-2.8/setup.cfg
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)      748 2024-04-02 02:19:46.000000 pyclipmgr-2.8/setup.py
```

### Comparing `pyclipmgr-2.7/PKG-INFO` & `pyclipmgr-2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyclipmgr
-Version: 2.7
+Version: 2.8
 Summary: this lib check for your machine's platform and use system commands to contact with clipboard (copy or paste) in python
 Home-page: https://github.com/mohammed-saleh2007/py-clip-mgr
 Author: sudo man
 Author-email: supertechman@yahoo.com
 Description-Content-Type: text/markdown
 
 # Py ClipBoard Manager
```

### Comparing `pyclipmgr-2.7/README.md` & `pyclipmgr-2.8/README.md`

 * *Files identical despite different names*

### Comparing `pyclipmgr-2.7/pyclipmgr.egg-info/PKG-INFO` & `pyclipmgr-2.8/pyclipmgr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyclipmgr
-Version: 2.7
+Version: 2.8
 Summary: this lib check for your machine's platform and use system commands to contact with clipboard (copy or paste) in python
 Home-page: https://github.com/mohammed-saleh2007/py-clip-mgr
 Author: sudo man
 Author-email: supertechman@yahoo.com
 Description-Content-Type: text/markdown
 
 # Py ClipBoard Manager
```

### Comparing `pyclipmgr-2.7/pyclipmgr.py` & `pyclipmgr-2.8/pyclipmgr.py`

 * *Files identical despite different names*

### Comparing `pyclipmgr-2.7/setup.py` & `pyclipmgr-2.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 from pyclipmgr import copy, paste
 
 setup(
     name='pyclipmgr',
     packages=find_packages(),
     scripts=['pyclipmgr.py'],  # List of script files to be installed
-    version='2.7',
+    version='2.8',
     entry_points={
         'console_scripts': [
-            'pyclipmgr-copy = pyclipmgr:copy',
+            'pyclipmgr-copy = pyclipmgr',
             'pyclipmgr-paste = pyclipmgr:paste',
         ]
     },
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='sudo man',
     author_email='supertechman@yahoo.com',
```

