# Comparing `tmp/NitroPy-1.0.0.tar.gz` & `tmp/NitroPy-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NitroPy-1.0.0.tar", last modified: Sat Mar 23 08:33:19 2024, max compression
+gzip compressed data, was "NitroPy-1.1.0.tar", last modified: Tue Apr  2 16:08:10 2024, max compression
```

## Comparing `NitroPy-1.0.0.tar` & `NitroPy-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-03-23 08:33:19.614945 NitroPy-1.0.0/
-drwxrwxrwx   0        0        0        0 2024-03-23 08:33:19.606447 NitroPy-1.0.0/NitroPy.egg-info/
--rw-rw-rw-   0        0        0      381 2024-03-23 08:33:19.000000 NitroPy-1.0.0/NitroPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      172 2024-03-23 08:33:19.000000 NitroPy-1.0.0/NitroPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-23 08:33:19.000000 NitroPy-1.0.0/NitroPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2024-03-23 08:33:19.000000 NitroPy-1.0.0/NitroPy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-03-23 08:33:19.000000 NitroPy-1.0.0/NitroPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      381 2024-03-23 08:33:19.614945 NitroPy-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-03-23 07:14:07.000000 NitroPy-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2024-03-23 08:33:19.614945 NitroPy-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      720 2024-03-23 08:28:31.000000 NitroPy-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 16:08:10.042399 NitroPy-1.1.0/
+drwxrwxrwx   0        0        0        0 2024-04-02 16:08:10.033915 NitroPy-1.1.0/NitroPy.egg-info/
+-rw-rw-rw-   0        0        0      384 2024-04-02 16:08:07.000000 NitroPy-1.1.0/NitroPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2024-04-02 16:08:07.000000 NitroPy-1.1.0/NitroPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 16:08:07.000000 NitroPy-1.1.0/NitroPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2024-04-02 16:08:07.000000 NitroPy-1.1.0/NitroPy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-02 16:08:07.000000 NitroPy-1.1.0/NitroPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      384 2024-04-02 16:08:10.040384 NitroPy-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-03-23 07:14:07.000000 NitroPy-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 16:08:10.038137 NitroPy-1.1.0/nitrotype/
+-rw-rw-rw-   0        0        0       27 2024-04-02 16:03:12.000000 NitroPy-1.1.0/nitrotype/__init__.py
+-rw-rw-rw-   0        0        0     2319 2024-04-02 16:03:12.000000 NitroPy-1.1.0/nitrotype/_nitrotype.py
+-rw-rw-rw-   0        0        0       42 2024-04-02 16:08:10.046193 NitroPy-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      757 2024-04-02 16:06:06.000000 NitroPy-1.1.0/setup.py
```

### Comparing `NitroPy-1.0.0/setup.py` & `NitroPy-1.1.0/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,27 @@
-from setuptools import setup, find_packages
+from setuptools import setup
 
 setup(
-    name='NitroPy',  
-    version='1.0.0',
+    name='NitroPy',
+    version='1.1.0',
     author='Malakai',
-    author_email='your.email@example.com',
+    author_email='Almightyslider2@gmail.com',
     description='A package for interacting with Nitrotype racers',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
-#    url='https://github.com/yourusername/nitrotype-package',
-    packages=find_packages(),
+    #    url='https://github.com/yourusername/nitrotype-package',
+    packages=[
+        "nitrotype"
+    ],
+    include_package_data=True,
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
+
     python_requires='>=3.6',
     install_requires=[
-        'cloudscraper', 
+        'cloudscraper',
         'beautifulsoup4',
     ],
 )
```

