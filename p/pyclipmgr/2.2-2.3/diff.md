# Comparing `tmp/pyclipmgr-2.2.tar.gz` & `tmp/pyclipmgr-2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyclipmgr-2.2.tar", last modified: Tue Apr  2 02:02:58 2024, max compression
+gzip compressed data, was "pyclipmgr-2.3.tar", last modified: Tue Apr  2 02:08:25 2024, max compression
```

## Comparing `pyclipmgr-2.2.tar` & `pyclipmgr-2.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 mohamed   (1000) mohamed   (1000)        0 2024-04-02 02:02:58.976147 pyclipmgr-2.2/
--rw-r--r--   0 mohamed   (1000) mohamed   (1000)     1384 2024-04-02 02:02:58.976147 pyclipmgr-2.2/PKG-INFO
--rw-r--r--   0 mohamed   (1000) mohamed   (1000)     1048 2024-04-02 01:51:33.000000 pyclipmgr-2.2/README.md
-drwxr-xr-x   0 mohamed   (1000) mohamed   (1000)        0 2024-04-02 02:02:58.976147 pyclipmgr-2.2/pyclipmgr.egg-info/
--rw-r--r--   0 mohamed   (1000) mohamed   (1000)     1384 2024-04-02 02:02:58.000000 pyclipmgr-2.2/pyclipmgr.egg-info/PKG-INFO
--rw-r--r--   0 mohamed   (1000) mohamed   (1000)      199 2024-04-02 02:02:58.000000 pyclipmgr-2.2/pyclipmgr.egg-info/SOURCES.txt
--rw-r--r--   0 mohamed   (1000) mohamed   (1000)        1 2024-04-02 02:02:58.000000 pyclipmgr-2.2/pyclipmgr.egg-info/dependency_links.txt
--rw-r--r--   0 mohamed   (1000) mohamed   (1000)       84 2024-04-02 02:02:58.000000 pyclipmgr-2.2/pyclipmgr.egg-info/entry_points.txt
--rw-r--r--   0 mohamed   (1000) mohamed   (1000)        1 2024-04-02 02:02:58.000000 pyclipmgr-2.2/pyclipmgr.egg-info/top_level.txt
--rw-r--r--   0 mohamed   (1000) mohamed   (1000)     1210 2024-04-02 01:53:42.000000 pyclipmgr-2.2/pyclipmgr.py
--rw-r--r--   0 mohamed   (1000) mohamed   (1000)       38 2024-04-02 02:02:58.976147 pyclipmgr-2.2/setup.cfg
--rw-r--r--   0 mohamed   (1000) mohamed   (1000)      753 2024-04-02 02:02:45.000000 pyclipmgr-2.2/setup.py
+drwxr-xr-x   0 mohamed   (1000) mohamed   (1000)        0 2024-04-02 02:08:25.778404 pyclipmgr-2.3/
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)     1384 2024-04-02 02:08:25.778404 pyclipmgr-2.3/PKG-INFO
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)     1048 2024-04-02 01:51:33.000000 pyclipmgr-2.3/README.md
+drwxr-xr-x   0 mohamed   (1000) mohamed   (1000)        0 2024-04-02 02:08:25.778404 pyclipmgr-2.3/pyclipmgr.egg-info/
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)     1384 2024-04-02 02:08:25.000000 pyclipmgr-2.3/pyclipmgr.egg-info/PKG-INFO
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)      199 2024-04-02 02:08:25.000000 pyclipmgr-2.3/pyclipmgr.egg-info/SOURCES.txt
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)        1 2024-04-02 02:08:25.000000 pyclipmgr-2.3/pyclipmgr.egg-info/dependency_links.txt
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)       84 2024-04-02 02:08:25.000000 pyclipmgr-2.3/pyclipmgr.egg-info/entry_points.txt
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)        1 2024-04-02 02:08:25.000000 pyclipmgr-2.3/pyclipmgr.egg-info/top_level.txt
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)     1270 2024-04-02 02:07:42.000000 pyclipmgr-2.3/pyclipmgr.py
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)       38 2024-04-02 02:08:25.778404 pyclipmgr-2.3/setup.cfg
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)      753 2024-04-02 02:08:09.000000 pyclipmgr-2.3/setup.py
```

### Comparing `pyclipmgr-2.2/PKG-INFO` & `pyclipmgr-2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyclipmgr
-Version: 2.2
+Version: 2.3
 Summary: this lib check for your machine's platform and use system commands to contact with clipboard (copy or paste) in python
 Home-page: https://github.com/mohammed-saleh2007/py-clip-mgr
 Author: sudo man
 Author-email: supertechman@yahoo.com
 Description-Content-Type: text/markdown
 
 # Py ClipBoard Manager
```

### Comparing `pyclipmgr-2.2/README.md` & `pyclipmgr-2.3/README.md`

 * *Files identical despite different names*

### Comparing `pyclipmgr-2.2/pyclipmgr.egg-info/PKG-INFO` & `pyclipmgr-2.3/pyclipmgr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyclipmgr
-Version: 2.2
+Version: 2.3
 Summary: this lib check for your machine's platform and use system commands to contact with clipboard (copy or paste) in python
 Home-page: https://github.com/mohammed-saleh2007/py-clip-mgr
 Author: sudo man
 Author-email: supertechman@yahoo.com
 Description-Content-Type: text/markdown
 
 # Py ClipBoard Manager
```

### Comparing `pyclipmgr-2.2/pyclipmgr.py` & `pyclipmgr-2.3/pyclipmgr.py`

 * *Files 14% similar despite different names*

```diff
@@ -40,9 +40,12 @@
 
     elif platform.system() == "Windows":
         text = run_command('echo | clip')
     
     return text
 
 if __name__ == "__main__":
-    text = sys.argv[1]
-    copy(text)
+    if len(sys.argv) > 1:
+        text = sys.argv[1]
+        copy(text)
+    else:
+        paste()
```

### Comparing `pyclipmgr-2.2/setup.py` & `pyclipmgr-2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 from pyclipmgr import copy, paste
 
 setup(
     name='pyclipmgr',
     packages=find_packages(),
     scripts=['pyclipmgr.py'],  # List of script files to be installed
-    version='2.2',
+    version='2.3',
     entry_points={
         'console_scripts': [
             'pyclipmgr-copy = pyclipmgr:copy',
             'pyclipmgr-paste = pyclipmgr:paste',
         ]
     },
     long_description=open('README.md').read(),
```

