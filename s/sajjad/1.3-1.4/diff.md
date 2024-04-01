# Comparing `tmp/sajjad-1.3.tar.gz` & `tmp/sajjad-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sajjad-1.3.tar", last modified: Mon Apr  1 20:22:25 2024, max compression
+gzip compressed data, was "sajjad-1.4.tar", last modified: Mon Apr  1 20:32:48 2024, max compression
```

## Comparing `sajjad-1.3.tar` & `sajjad-1.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 20:22:25.537597 sajjad-1.3/
--rw-rw-rw-   0        0        0      441 2024-04-01 20:22:25.535596 sajjad-1.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-01 20:22:25.519176 sajjad-1.3/sajjad/
--rw-rw-rw-   0        0        0        0 2024-04-01 20:21:50.000000 sajjad-1.3/sajjad/__init__.py
--rw-rw-rw-   0        0        0       97 2024-03-27 20:51:54.000000 sajjad-1.3/sajjad/sajjad.py
-drwxrwxrwx   0        0        0        0 2024-04-01 20:22:25.534625 sajjad-1.3/sajjad.egg-info/
--rw-rw-rw-   0        0        0      441 2024-04-01 20:22:25.000000 sajjad-1.3/sajjad.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      164 2024-04-01 20:22:25.000000 sajjad-1.3/sajjad.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 20:22:25.000000 sajjad-1.3/sajjad.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-01 20:22:25.000000 sajjad-1.3/sajjad.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-01 20:22:25.537597 sajjad-1.3/setup.cfg
--rw-rw-rw-   0        0        0      562 2024-04-01 20:21:06.000000 sajjad-1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 20:32:48.995613 sajjad-1.4/
+-rw-rw-rw-   0        0        0      441 2024-04-01 20:32:48.994613 sajjad-1.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-01 20:32:48.981727 sajjad-1.4/sajjad/
+-rw-rw-rw-   0        0        0       21 2024-04-01 20:31:53.000000 sajjad-1.4/sajjad/__init__.py
+-rw-rw-rw-   0        0        0       97 2024-03-27 20:51:54.000000 sajjad-1.4/sajjad/sajjad.py
+drwxrwxrwx   0        0        0        0 2024-04-01 20:32:48.993614 sajjad-1.4/sajjad.egg-info/
+-rw-rw-rw-   0        0        0      441 2024-04-01 20:32:48.000000 sajjad-1.4/sajjad.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      164 2024-04-01 20:32:48.000000 sajjad-1.4/sajjad.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 20:32:48.000000 sajjad-1.4/sajjad.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-01 20:32:48.000000 sajjad-1.4/sajjad.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-01 20:32:48.995613 sajjad-1.4/setup.cfg
+-rw-rw-rw-   0        0        0      562 2024-04-01 20:31:40.000000 sajjad-1.4/setup.py
```

### Comparing `sajjad-1.3/setup.py` & `sajjad-1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sajjad',
-    version='1.3',
+    version='1.4',
     packages=find_packages(),
     description='sajjad created that',
     author='sajjad seyedi',
     author_email='sajjad.seyedi.88@gmail.com',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
```

