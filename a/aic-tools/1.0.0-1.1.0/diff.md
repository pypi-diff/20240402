# Comparing `tmp/aic_tools-1.0.0.tar.gz` & `tmp/aic_tools-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aic_tools-1.0.0.tar", last modified: Mon Apr  1 22:42:36 2024, max compression
+gzip compressed data, was "aic_tools-1.1.0.tar", last modified: Mon Apr  1 23:53:44 2024, max compression
```

## Comparing `aic_tools-1.0.0.tar` & `aic_tools-1.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 vkovalevskyi   (501) staff       (20)        0 2024-04-01 22:42:36.345805 aic_tools-1.0.0/
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)      258 2024-04-01 22:42:36.345590 aic_tools-1.0.0/PKG-INFO
-drwxr-xr-x   0 vkovalevskyi   (501) staff       (20)        0 2024-04-01 22:42:36.344302 aic_tools-1.0.0/aic_tools/
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)        0 2024-04-01 20:35:34.000000 aic_tools-1.0.0/aic_tools/__init__.py
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)      428 2024-04-01 22:21:19.000000 aic_tools-1.0.0/aic_tools/datetime.py
-drwxr-xr-x   0 vkovalevskyi   (501) staff       (20)        0 2024-04-01 22:42:36.345323 aic_tools-1.0.0/aic_tools.egg-info/
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)      258 2024-04-01 22:42:36.000000 aic_tools-1.0.0/aic_tools.egg-info/PKG-INFO
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)      216 2024-04-01 22:42:36.000000 aic_tools-1.0.0/aic_tools.egg-info/SOURCES.txt
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)        1 2024-04-01 22:42:36.000000 aic_tools-1.0.0/aic_tools.egg-info/dependency_links.txt
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)       18 2024-04-01 22:42:36.000000 aic_tools-1.0.0/aic_tools.egg-info/requires.txt
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)       10 2024-04-01 22:42:36.000000 aic_tools-1.0.0/aic_tools.egg-info/top_level.txt
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)       38 2024-04-01 22:42:36.345877 aic_tools-1.0.0/setup.cfg
--rw-r--r--   0 vkovalevskyi   (501) staff       (20)      809 2024-04-01 22:42:24.000000 aic_tools-1.0.0/setup.py
+drwxr-xr-x   0 vkovalevskyi   (501) staff       (20)        0 2024-04-01 23:53:44.708566 aic_tools-1.1.0/
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)      258 2024-04-01 23:53:44.708437 aic_tools-1.1.0/PKG-INFO
+drwxr-xr-x   0 vkovalevskyi   (501) staff       (20)        0 2024-04-01 23:53:44.707425 aic_tools-1.1.0/aic_tools/
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)        0 2024-04-01 20:35:34.000000 aic_tools-1.1.0/aic_tools/__init__.py
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)      428 2024-04-01 22:21:19.000000 aic_tools-1.1.0/aic_tools/datetime.py
+drwxr-xr-x   0 vkovalevskyi   (501) staff       (20)        0 2024-04-01 23:53:44.708264 aic_tools-1.1.0/aic_tools.egg-info/
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)      258 2024-04-01 23:53:44.000000 aic_tools-1.1.0/aic_tools.egg-info/PKG-INFO
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)      216 2024-04-01 23:53:44.000000 aic_tools-1.1.0/aic_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)        1 2024-04-01 23:53:44.000000 aic_tools-1.1.0/aic_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)       18 2024-04-01 23:53:44.000000 aic_tools-1.1.0/aic_tools.egg-info/requires.txt
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)       10 2024-04-01 23:53:44.000000 aic_tools-1.1.0/aic_tools.egg-info/top_level.txt
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)       38 2024-04-01 23:53:44.708618 aic_tools-1.1.0/setup.cfg
+-rw-r--r--   0 vkovalevskyi   (501) staff       (20)      809 2024-04-01 23:51:00.000000 aic_tools-1.1.0/setup.py
```

### Comparing `aic_tools-1.0.0/setup.py` & `aic_tools-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
         return [line.strip() for line in req if line.strip() and not line.startswith('#')]
 
 # Call the function and store the requirements list
 install_requires = read_requirements()
 
 setup(
     name='aic_tools',
-    version='1.0.0',
+    version='1.1.0',
     packages=find_packages(),
     description='Tools for AI Characters',
     long_description_content_type='text/markdown',
     author='Viacheslav Kovalevskyi',
     author_email='viacheslav@kovalevskyi.com',
     license='MIT',
     install_requires=install_requires,
```

