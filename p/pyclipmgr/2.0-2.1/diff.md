# Comparing `tmp/pyclipmgr-2.0.tar.gz` & `tmp/pyclipmgr-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyclipmgr-2.0.tar", last modified: Tue Apr  2 01:46:10 2024, max compression
+gzip compressed data, was "pyclipmgr-2.1.tar", last modified: Tue Apr  2 01:52:14 2024, max compression
```

## Comparing `pyclipmgr-2.0.tar` & `pyclipmgr-2.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 mohamed   (1000) mohamed   (1000)        0 2024-04-02 01:46:10.603438 pyclipmgr-2.0/
--rw-r--r--   0 mohamed   (1000) mohamed   (1000)     1366 2024-04-02 01:46:10.603438 pyclipmgr-2.0/PKG-INFO
--rw-r--r--   0 mohamed   (1000) mohamed   (1000)     1030 2024-04-02 01:37:47.000000 pyclipmgr-2.0/README.md
-drwxr-xr-x   0 mohamed   (1000) mohamed   (1000)        0 2024-04-02 01:46:10.603438 pyclipmgr-2.0/pyclipmgr.egg-info/
--rw-r--r--   0 mohamed   (1000) mohamed   (1000)     1366 2024-04-02 01:46:10.000000 pyclipmgr-2.0/pyclipmgr.egg-info/PKG-INFO
--rw-r--r--   0 mohamed   (1000) mohamed   (1000)      199 2024-04-02 01:46:10.000000 pyclipmgr-2.0/pyclipmgr.egg-info/SOURCES.txt
--rw-r--r--   0 mohamed   (1000) mohamed   (1000)        1 2024-04-02 01:46:10.000000 pyclipmgr-2.0/pyclipmgr.egg-info/dependency_links.txt
--rw-r--r--   0 mohamed   (1000) mohamed   (1000)       84 2024-04-02 01:46:10.000000 pyclipmgr-2.0/pyclipmgr.egg-info/entry_points.txt
--rw-r--r--   0 mohamed   (1000) mohamed   (1000)        1 2024-04-02 01:46:10.000000 pyclipmgr-2.0/pyclipmgr.egg-info/top_level.txt
--rw-r--r--   0 mohamed   (1000) mohamed   (1000)     1130 2024-04-02 01:41:03.000000 pyclipmgr-2.0/pyclipmgr.py
--rw-r--r--   0 mohamed   (1000) mohamed   (1000)       38 2024-04-02 01:46:10.603438 pyclipmgr-2.0/setup.cfg
--rw-r--r--   0 mohamed   (1000) mohamed   (1000)      753 2024-04-02 01:46:01.000000 pyclipmgr-2.0/setup.py
+drwxr-xr-x   0 mohamed   (1000) mohamed   (1000)        0 2024-04-02 01:52:14.244779 pyclipmgr-2.1/
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)     1384 2024-04-02 01:52:14.244779 pyclipmgr-2.1/PKG-INFO
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)     1048 2024-04-02 01:51:33.000000 pyclipmgr-2.1/README.md
+drwxr-xr-x   0 mohamed   (1000) mohamed   (1000)        0 2024-04-02 01:52:14.244779 pyclipmgr-2.1/pyclipmgr.egg-info/
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)     1384 2024-04-02 01:52:14.000000 pyclipmgr-2.1/pyclipmgr.egg-info/PKG-INFO
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)      199 2024-04-02 01:52:14.000000 pyclipmgr-2.1/pyclipmgr.egg-info/SOURCES.txt
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)        1 2024-04-02 01:52:14.000000 pyclipmgr-2.1/pyclipmgr.egg-info/dependency_links.txt
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)       84 2024-04-02 01:52:14.000000 pyclipmgr-2.1/pyclipmgr.egg-info/entry_points.txt
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)        1 2024-04-02 01:52:14.000000 pyclipmgr-2.1/pyclipmgr.egg-info/top_level.txt
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)     1199 2024-04-02 01:50:11.000000 pyclipmgr-2.1/pyclipmgr.py
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)       38 2024-04-02 01:52:14.244779 pyclipmgr-2.1/setup.cfg
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)      753 2024-04-02 01:51:46.000000 pyclipmgr-2.1/setup.py
```

### Comparing `pyclipmgr-2.0/PKG-INFO` & `pyclipmgr-2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pyclipmgr
-Version: 2.0
+Version: 2.1
 Summary: this lib check for your machine's platform and use system commands to contact with clipboard (copy or paste) in python
 Home-page: https://github.com/mohammed-saleh2007/py-clip-mgr
 Author: sudo man
 Author-email: supertechman@yahoo.com
 Description-Content-Type: text/markdown
 
 # Py ClipBoard Manager
 
 ## Features:
 - this lib check for your machine's platform and use system commands to contact with clipboard (copy or paste) in python
 
 - this script works with `linux ( XORG or Wayland), Windows and Macos`
 
-- DIDN'T TESTED ON WINDOWS OR MAC!!
+-  I didn't test it on windows and macos
 
 - for linux users! you need to install `xclip` if you use xorg or `wl-clipboard` if you use wayland from your package manager
 
 ## How to install?
 
 - you can clone the repo and import the script (pyclipmgr.py) to your script
 ```
@@ -42,15 +42,15 @@
 ```
 
 - to paste from clipboard, this will print clipboard content in terminal
 ```
 pyclipmgr.paste()
 ```
 
-- you can use in your console!
+- you can use it in your (console/terminal)
 ```
 ~$ pyperclip-copy "Some Text"
 ~$ pyperclip-paste
 Some Text
 ```
 
 ### Hope this script get the work done as it did with me
```

### Comparing `pyclipmgr-2.0/README.md` & `pyclipmgr-2.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Py ClipBoard Manager
 
 ## Features:
 - this lib check for your machine's platform and use system commands to contact with clipboard (copy or paste) in python
 
 - this script works with `linux ( XORG or Wayland), Windows and Macos`
 
-- DIDN'T TESTED ON WINDOWS OR MAC!!
+-  I didn't test it on windows and macos
 
 - for linux users! you need to install `xclip` if you use xorg or `wl-clipboard` if you use wayland from your package manager
 
 ## How to install?
 
 - you can clone the repo and import the script (pyclipmgr.py) to your script
 ```
@@ -33,15 +33,15 @@
 ```
 
 - to paste from clipboard, this will print clipboard content in terminal
 ```
 pyclipmgr.paste()
 ```
 
-- you can use in your console!
+- you can use it in your (console/terminal)
 ```
 ~$ pyperclip-copy "Some Text"
 ~$ pyperclip-paste
 Some Text
 ```
 
 ### Hope this script get the work done as it did with me
```

### Comparing `pyclipmgr-2.0/pyclipmgr.egg-info/PKG-INFO` & `pyclipmgr-2.1/pyclipmgr.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pyclipmgr
-Version: 2.0
+Version: 2.1
 Summary: this lib check for your machine's platform and use system commands to contact with clipboard (copy or paste) in python
 Home-page: https://github.com/mohammed-saleh2007/py-clip-mgr
 Author: sudo man
 Author-email: supertechman@yahoo.com
 Description-Content-Type: text/markdown
 
 # Py ClipBoard Manager
 
 ## Features:
 - this lib check for your machine's platform and use system commands to contact with clipboard (copy or paste) in python
 
 - this script works with `linux ( XORG or Wayland), Windows and Macos`
 
-- DIDN'T TESTED ON WINDOWS OR MAC!!
+-  I didn't test it on windows and macos
 
 - for linux users! you need to install `xclip` if you use xorg or `wl-clipboard` if you use wayland from your package manager
 
 ## How to install?
 
 - you can clone the repo and import the script (pyclipmgr.py) to your script
 ```
@@ -42,15 +42,15 @@
 ```
 
 - to paste from clipboard, this will print clipboard content in terminal
 ```
 pyclipmgr.paste()
 ```
 
-- you can use in your console!
+- you can use it in your (console/terminal)
 ```
 ~$ pyperclip-copy "Some Text"
 ~$ pyperclip-paste
 Some Text
 ```
 
 ### Hope this script get the work done as it did with me
```

### Comparing `pyclipmgr-2.0/pyclipmgr.py` & `pyclipmgr-2.1/pyclipmgr.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import platform
 import os
 import subprocess
 
-def copy(text):
+def copy(text=None):
     if platform.system() == "Linux" :
 
         if os.getenv('WAYLAND_DISPLAY'):
             os.system(f'echo "{text}" | wl-copy')
 
         else:
             os.system(f'echo "{text}" | xclip -selection clipboard')
@@ -38,7 +38,10 @@
         text = run_command('pbpaste')
 
     elif platform.system() == "Windows":
         text = run_command('echo | clip')
     
     return text
 
+if __name__ == "__main__":
+    text = sys.argv[1]
+    copy(text)
```

### Comparing `pyclipmgr-2.0/setup.py` & `pyclipmgr-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 from pyclipmgr import copy, paste
 
 setup(
     name='pyclipmgr',
     packages=find_packages(),
     scripts=['pyclipmgr.py'],  # List of script files to be installed
-    version='2.0',
+    version='2.1',
     entry_points={
         'console_scripts': [
             'pyclipmgr-copy = pyclipmgr:copy',
             'pyclipmgr-paste = pyclipmgr:paste',
         ]
     },
     long_description=open('README.md').read(),
```

