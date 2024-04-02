# Comparing `tmp/hellozen-0.0.4.tar.gz` & `tmp/hellozen-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hellozen-0.0.4.tar", last modified: Tue Apr  2 09:24:59 2024, max compression
+gzip compressed data, was "hellozen-0.0.5.tar", last modified: Tue Apr  2 09:28:09 2024, max compression
```

## Comparing `hellozen-0.0.4.tar` & `hellozen-0.0.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 09:24:59.274367 hellozen-0.0.4/
--rw-rw-rw-   0        0        0      230 2024-04-02 09:24:59.273368 hellozen-0.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-02 09:24:59.273368 hellozen-0.0.4/hellozen.egg-info/
--rw-rw-rw-   0        0        0      230 2024-04-02 09:24:59.000000 hellozen-0.0.4/hellozen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      171 2024-04-02 09:24:59.000000 hellozen-0.0.4/hellozen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 09:24:59.000000 hellozen-0.0.4/hellozen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2024-04-02 09:24:59.000000 hellozen-0.0.4/hellozen.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 09:24:59.000000 hellozen-0.0.4/hellozen.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-02 09:24:59.274367 hellozen-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      553 2024-04-02 09:24:41.000000 hellozen-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 09:28:09.657016 hellozen-0.0.5/
+-rw-rw-rw-   0        0        0      230 2024-04-02 09:28:09.657016 hellozen-0.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-02 09:28:09.656014 hellozen-0.0.5/hellozen.egg-info/
+-rw-rw-rw-   0        0        0      230 2024-04-02 09:28:09.000000 hellozen-0.0.5/hellozen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      171 2024-04-02 09:28:09.000000 hellozen-0.0.5/hellozen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 09:28:09.000000 hellozen-0.0.5/hellozen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2024-04-02 09:28:09.000000 hellozen-0.0.5/hellozen.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 09:28:09.000000 hellozen-0.0.5/hellozen.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-02 09:28:09.657016 hellozen-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      581 2024-04-02 09:27:42.000000 hellozen-0.0.5/setup.py
```

### Comparing `hellozen-0.0.4/setup.py` & `hellozen-0.0.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from setuptools import setup
+from setuptools import setup, find_packages
 
 setup(
     name='hellozen',
-    version='0.0.4',
-    packages=[],
+    version='0.0.5',
+    packages=find_packages(),
     install_requires=[],
     entry_points={
         'console_scripts': [
             'hello = hellozen:main'
         ],
     },
     author='Zen',
```

