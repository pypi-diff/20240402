# Comparing `tmp/CustomChat-1.0.4.tar.gz` & `tmp/CustomChat-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CustomChat-1.0.4.tar", last modified: Mon Apr  1 21:57:40 2024, max compression
+gzip compressed data, was "CustomChat-1.0.5.tar", last modified: Mon Apr  1 22:38:54 2024, max compression
```

## Comparing `CustomChat-1.0.4.tar` & `CustomChat-1.0.5.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxrwxr-x   0 elliot    (1000) elliot    (1000)        0 2024-04-01 21:57:40.124383 CustomChat-1.0.4/
-drwxrwxr-x   0 elliot    (1000) elliot    (1000)        0 2024-04-01 21:57:40.124383 CustomChat-1.0.4/CustomChat/
--rw-rw-r--   0 elliot    (1000) elliot    (1000)       80 2024-03-31 21:26:32.000000 CustomChat-1.0.4/CustomChat/__init__.py
--rw-rw-r--   0 elliot    (1000) elliot    (1000)    30996 2024-03-31 21:39:42.000000 CustomChat-1.0.4/CustomChat/app.py
--rw-rw-r--   0 elliot    (1000) elliot    (1000)      189 2024-03-02 23:52:49.000000 CustomChat-1.0.4/CustomChat/configuration.py
--rw-rw-r--   0 elliot    (1000) elliot    (1000)      940 2024-03-31 21:36:42.000000 CustomChat-1.0.4/CustomChat/main.py
--rw-rw-r--   0 elliot    (1000) elliot    (1000)       15 2024-03-31 21:40:30.000000 CustomChat-1.0.4/CustomChat/new_com.py
--rw-rw-r--   0 elliot    (1000) elliot    (1000)       15 2024-03-31 21:40:13.000000 CustomChat-1.0.4/CustomChat/new_words.py
-drwxrwxr-x   0 elliot    (1000) elliot    (1000)        0 2024-04-01 21:57:40.124383 CustomChat-1.0.4/CustomChat.egg-info/
--rw-rw-r--   0 elliot    (1000) elliot    (1000)     2963 2024-04-01 21:57:40.000000 CustomChat-1.0.4/CustomChat.egg-info/PKG-INFO
--rw-rw-r--   0 elliot    (1000) elliot    (1000)      321 2024-04-01 21:57:40.000000 CustomChat-1.0.4/CustomChat.egg-info/SOURCES.txt
--rw-rw-r--   0 elliot    (1000) elliot    (1000)        1 2024-04-01 21:57:40.000000 CustomChat-1.0.4/CustomChat.egg-info/dependency_links.txt
--rw-rw-r--   0 elliot    (1000) elliot    (1000)       24 2024-04-01 21:57:40.000000 CustomChat-1.0.4/CustomChat.egg-info/requires.txt
--rw-rw-r--   0 elliot    (1000) elliot    (1000)       11 2024-04-01 21:57:40.000000 CustomChat-1.0.4/CustomChat.egg-info/top_level.txt
--rw-rw-r--   0 elliot    (1000) elliot    (1000)     2963 2024-04-01 21:57:40.124383 CustomChat-1.0.4/PKG-INFO
--rw-rw-r--   0 elliot    (1000) elliot    (1000)     2456 2024-03-31 22:00:54.000000 CustomChat-1.0.4/README.md
--rw-rw-r--   0 elliot    (1000) elliot    (1000)       38 2024-04-01 21:57:40.124383 CustomChat-1.0.4/setup.cfg
--rw-rw-r--   0 elliot    (1000) elliot    (1000)      808 2024-04-01 21:57:29.000000 CustomChat-1.0.4/setup.py
+drwxrwxr-x   0 elliot    (1000) elliot    (1000)        0 2024-04-01 22:38:54.445314 CustomChat-1.0.5/
+drwxrwxr-x   0 elliot    (1000) elliot    (1000)        0 2024-04-01 22:38:54.441314 CustomChat-1.0.5/CustomChat/
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)       11 2024-04-01 17:34:56.000000 CustomChat-1.0.5/CustomChat/Name.py
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)       80 2024-03-31 21:26:32.000000 CustomChat-1.0.5/CustomChat/__init__.py
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)    30999 2024-04-01 22:36:01.000000 CustomChat-1.0.5/CustomChat/app.py
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)      189 2024-03-02 23:52:49.000000 CustomChat-1.0.5/CustomChat/configuration.py
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)      943 2024-04-01 22:36:12.000000 CustomChat-1.0.5/CustomChat/main.py
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)       15 2024-03-31 21:40:30.000000 CustomChat-1.0.5/CustomChat/new_com.py
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)       15 2024-03-31 21:40:13.000000 CustomChat-1.0.5/CustomChat/new_words.py
+drwxrwxr-x   0 elliot    (1000) elliot    (1000)        0 2024-04-01 22:38:54.441314 CustomChat-1.0.5/CustomChat.egg-info/
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)     2985 2024-04-01 22:38:54.000000 CustomChat-1.0.5/CustomChat.egg-info/PKG-INFO
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)      348 2024-04-01 22:38:54.000000 CustomChat-1.0.5/CustomChat.egg-info/SOURCES.txt
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)        1 2024-04-01 22:38:54.000000 CustomChat-1.0.5/CustomChat.egg-info/dependency_links.txt
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)       24 2024-04-01 22:38:54.000000 CustomChat-1.0.5/CustomChat.egg-info/requires.txt
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)       11 2024-04-01 22:38:54.000000 CustomChat-1.0.5/CustomChat.egg-info/top_level.txt
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)     1186 2024-03-09 18:39:04.000000 CustomChat-1.0.5/LICENSE
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)     2985 2024-04-01 22:38:54.445314 CustomChat-1.0.5/PKG-INFO
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)     2456 2024-03-31 22:00:54.000000 CustomChat-1.0.5/README.md
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)       38 2024-04-01 22:38:54.445314 CustomChat-1.0.5/setup.cfg
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)      808 2024-04-01 22:38:51.000000 CustomChat-1.0.5/setup.py
```

### Comparing `CustomChat-1.0.4/CustomChat/app.py` & `CustomChat-1.0.5/CustomChat/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from datetime import datetime as dt
 import requests
 # Get cwd
 cwd=os.path.dirname(os.path.realpath(__file__))
 cwd=cwd+'/'
 print(cwd)
 # Get name
-namef = open(cwd+"Name", "r")
+namef = open(cwd+"Name.py", "r")
 name=namef.read()
 name=name.split('\n')[0]
 namef.close()
 print('Welcome to '+name+'\n')
 # Find username and ip
 file_location=os.path.expanduser('~')
 # Set up simple phrases
```

### Comparing `CustomChat-1.0.4/CustomChat/main.py` & `CustomChat-1.0.5/CustomChat/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 def run():
     import CustomChat.app
 def change_name(name):
     import os
-    file1 = open(os.path.join(os.path.dirname(__file__), "Name"), "w")
+    file1 = open(os.path.join(os.path.dirname(__file__), "Name.py"), "w")
     file1.write(name)
     file1.close()
 def set_config():
     import os
     import CustomChat.configuration as config
     command=input('Would you like the Command Line to be enabled? ')
     if 'yes' in command.lower() or 'true' in command.lower():
```

### Comparing `CustomChat-1.0.4/CustomChat.egg-info/PKG-INFO` & `CustomChat-1.0.5/CustomChat.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: CustomChat
-Version: 1.0.4
+Version: 1.0.5
 Summary: CustomChat: An AI-powered chatbot with easy customization. Powered by a simple but effective Python AI, it opens websites, executes commands, and delivers tailored responses. Enhance your projects with CustomChat's versatility and adaptability.
 Home-page: https://github.com/Mrpi314tech/CustomChat
 Author: Your Name
 Author-email: elliotedebruin@gmail.com
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # CustomChat
 
 CustomChat is an easily customizable AI chatbot powered by Jimbot AI. Whether you're running it on an online compiler or locally, CustomChat empowers you to tailor it to your specific needs.
 
 ## Installation
```

### Comparing `CustomChat-1.0.4/PKG-INFO` & `CustomChat-1.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: CustomChat
-Version: 1.0.4
+Version: 1.0.5
 Summary: CustomChat: An AI-powered chatbot with easy customization. Powered by a simple but effective Python AI, it opens websites, executes commands, and delivers tailored responses. Enhance your projects with CustomChat's versatility and adaptability.
 Home-page: https://github.com/Mrpi314tech/CustomChat
 Author: Your Name
 Author-email: elliotedebruin@gmail.com
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # CustomChat
 
 CustomChat is an easily customizable AI chatbot powered by Jimbot AI. Whether you're running it on an online compiler or locally, CustomChat empowers you to tailor it to your specific needs.
 
 ## Installation
```

### Comparing `CustomChat-1.0.4/README.md` & `CustomChat-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `CustomChat-1.0.4/setup.py` & `CustomChat-1.0.5/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='CustomChat',
-    version='1.0.4',
+    version='1.0.5',
     packages=find_packages(),
     install_requires=[
         'requests',
         'beautifulsoup4'
     ],
     # other metadata
     author='Your Name',
```

