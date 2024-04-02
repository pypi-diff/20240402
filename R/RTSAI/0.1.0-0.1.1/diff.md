# Comparing `tmp/RTSAI-0.1.0.tar.gz` & `tmp/RTSAI-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RTSAI-0.1.0.tar", last modified: Tue Jan 30 12:37:04 2024, max compression
+gzip compressed data, was "RTSAI-0.1.1.tar", last modified: Tue Apr  2 08:27:47 2024, max compression
```

## Comparing `RTSAI-0.1.0.tar` & `RTSAI-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,20 @@
-drwxr-xr-x   0 abc        (501) admin       (80)        0 2024-01-30 12:37:04.466571 RTSAI-0.1.0/
--rw-r--r--   0 abc        (501) admin       (80)      404 2024-01-30 12:37:04.466264 RTSAI-0.1.0/PKG-INFO
-drwxr-xr-x   0 abc        (501) admin       (80)        0 2024-01-30 12:37:04.464386 RTSAI-0.1.0/RTSAI/
--rw-r--r--   0 abc        (501) admin       (80)       63 2024-01-30 07:08:00.000000 RTSAI-0.1.0/RTSAI/entry.py
--rw-r--r--   0 abc        (501) admin       (80)      233 2024-01-30 09:06:40.000000 RTSAI-0.1.0/RTSAI/main.py
-drwxr-xr-x   0 abc        (501) admin       (80)        0 2024-01-30 12:37:04.465975 RTSAI-0.1.0/RTSAI.egg-info/
--rw-r--r--   0 abc        (501) admin       (80)      404 2024-01-30 12:37:04.000000 RTSAI-0.1.0/RTSAI.egg-info/PKG-INFO
--rw-r--r--   0 abc        (501) admin       (80)      213 2024-01-30 12:37:04.000000 RTSAI-0.1.0/RTSAI.egg-info/SOURCES.txt
--rw-r--r--   0 abc        (501) admin       (80)        1 2024-01-30 12:37:04.000000 RTSAI-0.1.0/RTSAI.egg-info/dependency_links.txt
--rw-r--r--   0 abc        (501) admin       (80)       42 2024-01-30 12:37:04.000000 RTSAI-0.1.0/RTSAI.egg-info/entry_points.txt
--rw-r--r--   0 abc        (501) admin       (80)       15 2024-01-30 12:37:04.000000 RTSAI-0.1.0/RTSAI.egg-info/requires.txt
--rw-r--r--   0 abc        (501) admin       (80)        6 2024-01-30 12:37:04.000000 RTSAI-0.1.0/RTSAI.egg-info/top_level.txt
--rw-r--r--   0 abc        (501) admin       (80)       38 2024-01-30 12:37:04.466623 RTSAI-0.1.0/setup.cfg
--rw-r--r--   0 abc        (501) admin       (80)      877 2024-01-30 12:27:47.000000 RTSAI-0.1.0/setup.py
+drwxr-xr-x   0 abc        (501) admin       (80)        0 2024-04-02 08:27:47.897214 RTSAI-0.1.1/
+-rw-r--r--   0 abc        (501) admin       (80)      503 2024-04-02 08:27:47.896710 RTSAI-0.1.1/PKG-INFO
+drwxr-xr-x   0 abc        (501) admin       (80)        0 2024-04-02 08:27:47.891553 RTSAI-0.1.1/RTSAI/
+-rw-r--r--   0 abc        (501) admin       (80)        0 2024-01-30 12:45:47.000000 RTSAI-0.1.1/RTSAI/__init__.py
+-rw-r--r--   0 abc        (501) admin       (80)     4439 2024-04-02 08:27:20.000000 RTSAI-0.1.1/RTSAI/config.py
+-rw-r--r--   0 abc        (501) admin       (80)   100917 2024-04-01 10:54:37.000000 RTSAI-0.1.1/RTSAI/main.py
+drwxr-xr-x   0 abc        (501) admin       (80)        0 2024-04-02 08:27:47.890722 RTSAI-0.1.1/RTSAI/temp/
+drwxr-xr-x   0 abc        (501) admin       (80)        0 2024-04-02 08:27:47.895829 RTSAI-0.1.1/RTSAI/temp/kg_QALD_9/
+-rw-r--r--   0 abc        (501) admin       (80)     3089 2024-04-01 07:36:59.000000 RTSAI-0.1.1/RTSAI/temp/kg_QALD_9/QALD9_construct.py
+drwxr-xr-x   0 abc        (501) admin       (80)        0 2024-04-02 08:27:47.896049 RTSAI-0.1.1/RTSAI/temp/kg_countries/
+-rw-r--r--   0 abc        (501) admin       (80)      437 2024-04-01 07:25:50.000000 RTSAI-0.1.1/RTSAI/temp/kg_countries/countries.py
+drwxr-xr-x   0 abc        (501) admin       (80)        0 2024-04-02 08:27:47.896323 RTSAI-0.1.1/RTSAI.egg-info/
+-rw-r--r--   0 abc        (501) admin       (80)      503 2024-04-02 08:27:47.000000 RTSAI-0.1.1/RTSAI.egg-info/PKG-INFO
+-rw-r--r--   0 abc        (501) admin       (80)      309 2024-04-02 08:27:47.000000 RTSAI-0.1.1/RTSAI.egg-info/SOURCES.txt
+-rw-r--r--   0 abc        (501) admin       (80)        1 2024-04-02 08:27:47.000000 RTSAI-0.1.1/RTSAI.egg-info/dependency_links.txt
+-rw-r--r--   0 abc        (501) admin       (80)       42 2024-04-02 08:27:47.000000 RTSAI-0.1.1/RTSAI.egg-info/entry_points.txt
+-rw-r--r--   0 abc        (501) admin       (80)       54 2024-04-02 08:27:47.000000 RTSAI-0.1.1/RTSAI.egg-info/requires.txt
+-rw-r--r--   0 abc        (501) admin       (80)        6 2024-04-02 08:27:47.000000 RTSAI-0.1.1/RTSAI.egg-info/top_level.txt
+-rw-r--r--   0 abc        (501) admin       (80)       38 2024-04-02 08:27:47.897286 RTSAI-0.1.1/setup.cfg
+-rw-r--r--   0 abc        (501) admin       (80)      856 2024-04-02 08:25:14.000000 RTSAI-0.1.1/setup.py
```

### Comparing `RTSAI-0.1.0/setup.py` & `RTSAI-0.1.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 
-import sys, setuptools
-
-PACKAGE_NAME = "RTSAI"
-PACKAGE_VERSION = '0.1.0'
-ROOT_PATH = sys.executable[::-1][sys.executable[::-1].index('/')+1:][::-1]
+import os, setuptools
+from RTSAI.config import PACKAGE_NAME, PACKAGE_VERSION, DATA_PATH
 
 setuptools.setup (
     name = PACKAGE_NAME, 
     version = PACKAGE_VERSION, 
     description = 'The recreated RTSAI package with pip install. ', 
     long_description = 'The recreated RTSAI package with pip install. ', 
     long_description_content_type = 'text/x-rst', 
@@ -18,15 +15,16 @@
         'console_scripts': [
             'RTSAI = RTSAI.main:main'
         ]
     }, 
     project_urls = {
         "Source": "https://github.com/WuKunhuan/RTSAI", 
     }, 
-    python_requires=">=3.12.0", 
+    python_requires=">=3.10.0", 
     install_requires = [
         "kgtk-wukunhuan", 
-    ], 
+        "appdirs", 
+        "pyautogui", 
+        "pillow", 
+        "pytest-shutil", 
+    ]
 )
-
-#   packages = setuptools.find_packages(), 
-
```

