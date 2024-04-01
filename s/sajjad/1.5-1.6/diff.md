# Comparing `tmp/sajjad-1.5.tar.gz` & `tmp/sajjad-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sajjad-1.5.tar", last modified: Mon Apr  1 22:59:21 2024, max compression
+gzip compressed data, was "sajjad-1.6.tar", last modified: Mon Apr  1 23:03:54 2024, max compression
```

## Comparing `sajjad-1.5.tar` & `sajjad-1.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 22:59:21.288834 sajjad-1.5/
--rw-rw-rw-   0        0        0      471 2024-04-01 22:59:21.287836 sajjad-1.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-01 22:59:21.260778 sajjad-1.5/sajjad/
--rw-rw-rw-   0        0        0       21 2024-04-01 20:31:53.000000 sajjad-1.5/sajjad/__init__.py
--rw-rw-rw-   0        0        0       97 2024-03-27 20:51:54.000000 sajjad-1.5/sajjad/sajjad.py
-drwxrwxrwx   0        0        0        0 2024-04-01 22:59:21.286836 sajjad-1.5/sajjad.egg-info/
--rw-rw-rw-   0        0        0      471 2024-04-01 22:59:21.000000 sajjad-1.5/sajjad.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      193 2024-04-01 22:59:21.000000 sajjad-1.5/sajjad.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 22:59:21.000000 sajjad-1.5/sajjad.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-04-01 22:59:21.000000 sajjad-1.5/sajjad.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-01 22:59:21.000000 sajjad-1.5/sajjad.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-01 22:59:21.288834 sajjad-1.5/setup.cfg
--rw-rw-rw-   0        0        0      620 2024-04-01 22:59:03.000000 sajjad-1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 23:03:54.369916 sajjad-1.6/
+-rw-rw-rw-   0        0        0      473 2024-04-01 23:03:54.368917 sajjad-1.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-01 23:03:54.352770 sajjad-1.6/sajjad/
+-rw-rw-rw-   0        0        0       21 2024-04-01 20:31:53.000000 sajjad-1.6/sajjad/__init__.py
+-rw-rw-rw-   0        0        0       97 2024-03-27 20:51:54.000000 sajjad-1.6/sajjad/sajjad.py
+drwxrwxrwx   0        0        0        0 2024-04-01 23:03:54.367916 sajjad-1.6/sajjad.egg-info/
+-rw-rw-rw-   0        0        0      473 2024-04-01 23:03:54.000000 sajjad-1.6/sajjad.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      193 2024-04-01 23:03:54.000000 sajjad-1.6/sajjad.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 23:03:54.000000 sajjad-1.6/sajjad.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-01 23:03:54.000000 sajjad-1.6/sajjad.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-01 23:03:54.000000 sajjad-1.6/sajjad.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-01 23:03:54.369916 sajjad-1.6/setup.cfg
+-rw-rw-rw-   0        0        0      622 2024-04-01 23:03:46.000000 sajjad-1.6/setup.py
```

### Comparing `sajjad-1.5/setup.py` & `sajjad-1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sajjad',
-    version='1.5',
+    version='1.6',
     packages=find_packages(),
     description='sajjad created that',
     author='sajjad seyedi',
     author_email='sajjad.seyedi.88@gmail.com',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
     ],
     install_requires=[
-        'colorama==4.6',
+        'colorama==0.4.6',
     ],
 )
```

