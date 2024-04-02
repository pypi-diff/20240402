# Comparing `tmp/pyclipmgr-2.8.tar.gz` & `tmp/pyclipmgr-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyclipmgr-2.8.tar", last modified: Tue Apr  2 02:19:51 2024, max compression
+gzip compressed data, was "pyclipmgr-3.0.0.tar", last modified: Tue Apr  2 02:30:53 2024, max compression
```

## Comparing `pyclipmgr-2.8.tar` & `pyclipmgr-3.0.0.tar`

### file list

```diff
@@ -1,12 +1,11 @@
-drwxr-xr-x   0 mohamed   (1000) mohamed   (1000)        0 2024-04-02 02:19:51.331761 pyclipmgr-2.8/
--rw-r--r--   0 mohamed   (1000) mohamed   (1000)     1384 2024-04-02 02:19:51.331761 pyclipmgr-2.8/PKG-INFO
--rw-r--r--   0 mohamed   (1000) mohamed   (1000)     1048 2024-04-02 01:51:33.000000 pyclipmgr-2.8/README.md
-drwxr-xr-x   0 mohamed   (1000) mohamed   (1000)        0 2024-04-02 02:19:51.331761 pyclipmgr-2.8/pyclipmgr.egg-info/
--rw-r--r--   0 mohamed   (1000) mohamed   (1000)     1384 2024-04-02 02:19:51.000000 pyclipmgr-2.8/pyclipmgr.egg-info/PKG-INFO
--rw-r--r--   0 mohamed   (1000) mohamed   (1000)      199 2024-04-02 02:19:51.000000 pyclipmgr-2.8/pyclipmgr.egg-info/SOURCES.txt
--rw-r--r--   0 mohamed   (1000) mohamed   (1000)        1 2024-04-02 02:19:51.000000 pyclipmgr-2.8/pyclipmgr.egg-info/dependency_links.txt
--rw-r--r--   0 mohamed   (1000) mohamed   (1000)       79 2024-04-02 02:19:51.000000 pyclipmgr-2.8/pyclipmgr.egg-info/entry_points.txt
--rw-r--r--   0 mohamed   (1000) mohamed   (1000)        1 2024-04-02 02:19:51.000000 pyclipmgr-2.8/pyclipmgr.egg-info/top_level.txt
--rw-r--r--   0 mohamed   (1000) mohamed   (1000)     1308 2024-04-02 02:17:57.000000 pyclipmgr-2.8/pyclipmgr.py
--rw-r--r--   0 mohamed   (1000) mohamed   (1000)       38 2024-04-02 02:19:51.331761 pyclipmgr-2.8/setup.cfg
--rw-r--r--   0 mohamed   (1000) mohamed   (1000)      748 2024-04-02 02:19:46.000000 pyclipmgr-2.8/setup.py
+drwxr-xr-x   0 mohamed   (1000) mohamed   (1000)        0 2024-04-02 02:30:53.927236 pyclipmgr-3.0.0/
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)     1400 2024-04-02 02:30:53.927236 pyclipmgr-3.0.0/PKG-INFO
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)     1062 2024-04-02 02:27:28.000000 pyclipmgr-3.0.0/README.md
+drwxr-xr-x   0 mohamed   (1000) mohamed   (1000)        0 2024-04-02 02:30:53.927236 pyclipmgr-3.0.0/pyclipmgr.egg-info/
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)     1400 2024-04-02 02:30:53.000000 pyclipmgr-3.0.0/pyclipmgr.egg-info/PKG-INFO
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)      163 2024-04-02 02:30:53.000000 pyclipmgr-3.0.0/pyclipmgr.egg-info/SOURCES.txt
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)        1 2024-04-02 02:30:53.000000 pyclipmgr-3.0.0/pyclipmgr.egg-info/dependency_links.txt
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)        1 2024-04-02 02:30:53.000000 pyclipmgr-3.0.0/pyclipmgr.egg-info/top_level.txt
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)     1128 2024-04-02 02:23:34.000000 pyclipmgr-3.0.0/pyclipmgr.py
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)       38 2024-04-02 02:30:53.933902 pyclipmgr-3.0.0/setup.cfg
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)      554 2024-04-02 02:30:43.000000 pyclipmgr-3.0.0/setup.py
```

### Comparing `pyclipmgr-2.8/PKG-INFO` & `pyclipmgr-3.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyclipmgr
-Version: 2.8
+Version: 3.0.0
 Summary: this lib check for your machine's platform and use system commands to contact with clipboard (copy or paste) in python
 Home-page: https://github.com/mohammed-saleh2007/py-clip-mgr
 Author: sudo man
 Author-email: supertechman@yahoo.com
 Description-Content-Type: text/markdown
 
 # Py ClipBoard Manager
@@ -42,15 +42,16 @@
 ```
 
 - to paste from clipboard, this will print clipboard content in terminal
 ```
 pyclipmgr.paste()
 ```
 
-- you can use it in your (console/terminal)
-```
+~~- you can use it in your (console/terminal)~~
+
+<!-- ```
 ~$ pyperclip-copy "Some Text"
 ~$ pyperclip-paste
 Some Text
-```
+``` -->
 
 ### Hope this script get the work done as it did with me
```

### Comparing `pyclipmgr-2.8/README.md` & `pyclipmgr-3.0.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -33,15 +33,16 @@
 ```
 
 - to paste from clipboard, this will print clipboard content in terminal
 ```
 pyclipmgr.paste()
 ```
 
-- you can use it in your (console/terminal)
-```
+~~- you can use it in your (console/terminal)~~
+
+<!-- ```
 ~$ pyperclip-copy "Some Text"
 ~$ pyperclip-paste
 Some Text
-```
+``` -->
 
 ### Hope this script get the work done as it did with me
```

### Comparing `pyclipmgr-2.8/pyclipmgr.egg-info/PKG-INFO` & `pyclipmgr-3.0.0/pyclipmgr.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyclipmgr
-Version: 2.8
+Version: 3.0.0
 Summary: this lib check for your machine's platform and use system commands to contact with clipboard (copy or paste) in python
 Home-page: https://github.com/mohammed-saleh2007/py-clip-mgr
 Author: sudo man
 Author-email: supertechman@yahoo.com
 Description-Content-Type: text/markdown
 
 # Py ClipBoard Manager
@@ -42,15 +42,16 @@
 ```
 
 - to paste from clipboard, this will print clipboard content in terminal
 ```
 pyclipmgr.paste()
 ```
 
-- you can use it in your (console/terminal)
-```
+~~- you can use it in your (console/terminal)~~
+
+<!-- ```
 ~$ pyperclip-copy "Some Text"
 ~$ pyperclip-paste
 Some Text
-```
+``` -->
 
 ### Hope this script get the work done as it did with me
```

### Comparing `pyclipmgr-2.8/pyclipmgr.py` & `pyclipmgr-3.0.0/pyclipmgr.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import platform
 import os
 import subprocess
-import sys
 
 def copy(text):
     if platform.system() == "Linux" :
 
         if os.getenv('WAYLAND_DISPLAY'):
             os.system(f'echo "{text}" | wl-copy')
 
@@ -37,15 +36,8 @@
 
     elif platform.system() == "Darwin":
         text = run_command('pbpaste')
 
     elif platform.system() == "Windows":
         text = run_command('echo | clip')
     
-    return text
-
-if __name__ == "__main__":
-    if len(sys.argv) < 2:
-        print('Usage: pyclipmgr-copy "text"')
-        sys.exit(1)
-    text = " ".join(sys.argv[1:])
-    copy(text)
+    return text
```

### Comparing `pyclipmgr-2.8/setup.py` & `pyclipmgr-3.0.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,15 @@
 from setuptools import setup, find_packages
 from pyclipmgr import copy, paste
 
 setup(
     name='pyclipmgr',
     packages=find_packages(),
-    scripts=['pyclipmgr.py'],  # List of script files to be installed
-    version='2.8',
-    entry_points={
-        'console_scripts': [
-            'pyclipmgr-copy = pyclipmgr',
-            'pyclipmgr-paste = pyclipmgr:paste',
-        ]
-    },
+    scripts=['pyclipmgr.py'],
+    version='3.0.0',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='sudo man',
     author_email='supertechman@yahoo.com',
     description="this lib check for your machine's platform and use system commands to contact with clipboard (copy or paste) in python",
     url='https://github.com/mohammed-saleh2007/py-clip-mgr',
 )
```

