# Comparing `tmp/pyclipmgr-3.0.0.tar.gz` & `tmp/pyclipmgr-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyclipmgr-3.0.0.tar", last modified: Tue Apr  2 02:30:53 2024, max compression
+gzip compressed data, was "pyclipmgr-4.0.0.tar", last modified: Tue Apr  2 09:46:21 2024, max compression
```

## Comparing `pyclipmgr-3.0.0.tar` & `pyclipmgr-4.0.0.tar`

### file list

```diff
@@ -1,11 +1,13 @@
-drwxr-xr-x   0 mohamed   (1000) mohamed   (1000)        0 2024-04-02 02:30:53.927236 pyclipmgr-3.0.0/
--rw-r--r--   0 mohamed   (1000) mohamed   (1000)     1400 2024-04-02 02:30:53.927236 pyclipmgr-3.0.0/PKG-INFO
--rw-r--r--   0 mohamed   (1000) mohamed   (1000)     1062 2024-04-02 02:27:28.000000 pyclipmgr-3.0.0/README.md
-drwxr-xr-x   0 mohamed   (1000) mohamed   (1000)        0 2024-04-02 02:30:53.927236 pyclipmgr-3.0.0/pyclipmgr.egg-info/
--rw-r--r--   0 mohamed   (1000) mohamed   (1000)     1400 2024-04-02 02:30:53.000000 pyclipmgr-3.0.0/pyclipmgr.egg-info/PKG-INFO
--rw-r--r--   0 mohamed   (1000) mohamed   (1000)      163 2024-04-02 02:30:53.000000 pyclipmgr-3.0.0/pyclipmgr.egg-info/SOURCES.txt
--rw-r--r--   0 mohamed   (1000) mohamed   (1000)        1 2024-04-02 02:30:53.000000 pyclipmgr-3.0.0/pyclipmgr.egg-info/dependency_links.txt
--rw-r--r--   0 mohamed   (1000) mohamed   (1000)        1 2024-04-02 02:30:53.000000 pyclipmgr-3.0.0/pyclipmgr.egg-info/top_level.txt
--rw-r--r--   0 mohamed   (1000) mohamed   (1000)     1128 2024-04-02 02:23:34.000000 pyclipmgr-3.0.0/pyclipmgr.py
--rw-r--r--   0 mohamed   (1000) mohamed   (1000)       38 2024-04-02 02:30:53.933902 pyclipmgr-3.0.0/setup.cfg
--rw-r--r--   0 mohamed   (1000) mohamed   (1000)      554 2024-04-02 02:30:43.000000 pyclipmgr-3.0.0/setup.py
+drwxr-xr-x   0 mohamed   (1000) mohamed   (1000)        0 2024-04-02 09:46:21.224723 pyclipmgr-4.0.0/
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)    35149 2024-04-02 09:03:54.000000 pyclipmgr-4.0.0/LICENSE
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)       55 2024-04-02 09:38:27.000000 pyclipmgr-4.0.0/MANIFEST.in
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)     1651 2024-04-02 09:46:21.224723 pyclipmgr-4.0.0/PKG-INFO
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)     1291 2024-04-02 09:43:28.000000 pyclipmgr-4.0.0/README.md
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)     1346 2024-04-02 09:38:02.000000 pyclipmgr-4.0.0/__init__.py
+drwxr-xr-x   0 mohamed   (1000) mohamed   (1000)        0 2024-04-02 09:46:21.224723 pyclipmgr-4.0.0/pyclipmgr.egg-info/
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)     1651 2024-04-02 09:46:21.000000 pyclipmgr-4.0.0/pyclipmgr.egg-info/PKG-INFO
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)      182 2024-04-02 09:46:21.000000 pyclipmgr-4.0.0/pyclipmgr.egg-info/SOURCES.txt
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)        1 2024-04-02 09:46:21.000000 pyclipmgr-4.0.0/pyclipmgr.egg-info/dependency_links.txt
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)        1 2024-04-02 09:46:21.000000 pyclipmgr-4.0.0/pyclipmgr.egg-info/top_level.txt
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)       38 2024-04-02 09:46:21.224723 pyclipmgr-4.0.0/setup.cfg
+-rw-r--r--   0 mohamed   (1000) mohamed   (1000)      584 2024-04-02 09:46:16.000000 pyclipmgr-4.0.0/setup.py
```

### Comparing `pyclipmgr-3.0.0/PKG-INFO` & `pyclipmgr-4.0.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 Metadata-Version: 2.1
 Name: pyclipmgr
-Version: 3.0.0
+Version: 4.0.0
 Summary: this lib check for your machine's platform and use system commands to contact with clipboard (copy or paste) in python
 Home-page: https://github.com/mohammed-saleh2007/py-clip-mgr
 Author: sudo man
 Author-email: supertechman@yahoo.com
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # Py ClipBoard Manager
 
 ## Features:
 - this lib check for your machine's platform and use system commands to contact with clipboard (copy or paste) in python
 
-- this script works with `linux ( XORG or Wayland), Windows and Macos`
+- this script works with `linux` `(XORG or Wayland)`, `Windows` and `Macos`
 
 -  I didn't test it on windows and macos
 
-- for linux users! you need to install `xclip` if you use xorg or `wl-clipboard` if you use wayland from your package manager
+- ~~for linux users! you need to install `xclip` if you use xorg or `wl-clipboard` if you use wayland from your package manager~~ Now! you do not need to do that. I did it for you by providing the requierd binaries from this packages.
 
 ## How to install?
 
 - you can clone the repo and import the script (pyclipmgr.py) to your script
 ```
 git clone https://github.com/mohammed-saleh2007/py-clip-mgr
 ```
-- you can also use pip to install it (recommended)
+- you can also use pip [Project In PyPi here](https://pypi.org/project/pyclipmgr/) to install it (recommended)
 ```
 pip install pyclipmgr
 ```
 
 ## How to use it?
 
 - import the lib in your file 
@@ -37,19 +38,24 @@
 ```
 
 - to copy some text
 ```
 pyclipmgr.copy("Some Text")
 ```
 
-- to paste from clipboard, this will print clipboard content in terminal
+- to paste from clipboard, this will return the clipboard content
 ```
 pyclipmgr.paste()
 ```
 
+- to print them in terminal
+```
+print(pyclipmgr.paste())
+```
+
 ~~- you can use it in your (console/terminal)~~
 
 <!-- ```
 ~$ pyperclip-copy "Some Text"
 ~$ pyperclip-paste
 Some Text
 ``` -->
```

### Comparing `pyclipmgr-3.0.0/pyclipmgr.egg-info/PKG-INFO` & `pyclipmgr-4.0.0/pyclipmgr.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 Metadata-Version: 2.1
 Name: pyclipmgr
-Version: 3.0.0
+Version: 4.0.0
 Summary: this lib check for your machine's platform and use system commands to contact with clipboard (copy or paste) in python
 Home-page: https://github.com/mohammed-saleh2007/py-clip-mgr
 Author: sudo man
 Author-email: supertechman@yahoo.com
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # Py ClipBoard Manager
 
 ## Features:
 - this lib check for your machine's platform and use system commands to contact with clipboard (copy or paste) in python
 
-- this script works with `linux ( XORG or Wayland), Windows and Macos`
+- this script works with `linux` `(XORG or Wayland)`, `Windows` and `Macos`
 
 -  I didn't test it on windows and macos
 
-- for linux users! you need to install `xclip` if you use xorg or `wl-clipboard` if you use wayland from your package manager
+- ~~for linux users! you need to install `xclip` if you use xorg or `wl-clipboard` if you use wayland from your package manager~~ Now! you do not need to do that. I did it for you by providing the requierd binaries from this packages.
 
 ## How to install?
 
 - you can clone the repo and import the script (pyclipmgr.py) to your script
 ```
 git clone https://github.com/mohammed-saleh2007/py-clip-mgr
 ```
-- you can also use pip to install it (recommended)
+- you can also use pip [Project In PyPi here](https://pypi.org/project/pyclipmgr/) to install it (recommended)
 ```
 pip install pyclipmgr
 ```
 
 ## How to use it?
 
 - import the lib in your file 
@@ -37,19 +38,24 @@
 ```
 
 - to copy some text
 ```
 pyclipmgr.copy("Some Text")
 ```
 
-- to paste from clipboard, this will print clipboard content in terminal
+- to paste from clipboard, this will return the clipboard content
 ```
 pyclipmgr.paste()
 ```
 
+- to print them in terminal
+```
+print(pyclipmgr.paste())
+```
+
 ~~- you can use it in your (console/terminal)~~
 
 <!-- ```
 ~$ pyperclip-copy "Some Text"
 ~$ pyperclip-paste
 Some Text
 ``` -->
```

