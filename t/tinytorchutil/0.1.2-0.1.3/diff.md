# Comparing `tmp/tinytorchutil-0.1.2.tar.gz` & `tmp/tinytorchutil-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinytorchutil-0.1.2.tar", last modified: Sun Mar 31 07:47:10 2024, max compression
+gzip compressed data, was "tinytorchutil-0.1.3.tar", last modified: Tue Apr  2 18:32:34 2024, max compression
```

## Comparing `tinytorchutil-0.1.2.tar` & `tinytorchutil-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-03-31 07:47:10.741709 tinytorchutil-0.1.2/
--rw-rw-rw-   0        0        0      408 2024-03-31 07:47:10.729706 tinytorchutil-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       17 2024-03-28 21:17:31.000000 tinytorchutil-0.1.2/README.md
--rw-rw-rw-   0        0        0       42 2024-03-31 07:47:10.742709 tinytorchutil-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      530 2024-03-31 07:42:03.000000 tinytorchutil-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-31 07:47:10.663691 tinytorchutil-0.1.2/tinytorchutil/
--rw-rw-rw-   0        0        0       30 2024-03-28 23:16:03.000000 tinytorchutil-0.1.2/tinytorchutil/__init__.py
--rw-rw-rw-   0        0        0    26695 2024-03-31 07:43:46.000000 tinytorchutil-0.1.2/tinytorchutil/tinytorchutil.py
-drwxrwxrwx   0        0        0        0 2024-03-31 07:47:10.721704 tinytorchutil-0.1.2/tinytorchutil.egg-info/
--rw-rw-rw-   0        0        0      408 2024-03-31 07:47:10.000000 tinytorchutil-0.1.2/tinytorchutil.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2024-03-31 07:47:10.000000 tinytorchutil-0.1.2/tinytorchutil.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-31 07:47:10.000000 tinytorchutil-0.1.2/tinytorchutil.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-03-31 07:47:10.000000 tinytorchutil-0.1.2/tinytorchutil.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-03-31 07:47:10.000000 tinytorchutil-0.1.2/tinytorchutil.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-02 18:32:34.172328 tinytorchutil-0.1.3/
+-rw-rw-rw-   0        0        0     4242 2024-04-02 18:32:34.165015 tinytorchutil-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3831 2024-03-31 08:01:16.000000 tinytorchutil-0.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-02 18:32:34.173378 tinytorchutil-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      543 2024-04-02 18:32:29.000000 tinytorchutil-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 18:32:34.126164 tinytorchutil-0.1.3/tinytorchutil/
+-rw-rw-rw-   0        0        0       30 2024-03-28 23:16:03.000000 tinytorchutil-0.1.3/tinytorchutil/__init__.py
+-rw-rw-rw-   0        0        0    26695 2024-03-31 07:43:46.000000 tinytorchutil-0.1.3/tinytorchutil/tinytorchutil.py
+drwxrwxrwx   0        0        0        0 2024-04-02 18:32:34.160739 tinytorchutil-0.1.3/tinytorchutil.egg-info/
+-rw-rw-rw-   0        0        0     4242 2024-04-02 18:32:33.000000 tinytorchutil-0.1.3/tinytorchutil.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2024-04-02 18:32:33.000000 tinytorchutil-0.1.3/tinytorchutil.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 18:32:33.000000 tinytorchutil-0.1.3/tinytorchutil.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2024-04-02 18:32:33.000000 tinytorchutil-0.1.3/tinytorchutil.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-02 18:32:33.000000 tinytorchutil-0.1.3/tinytorchutil.egg-info/top_level.txt
```

### Comparing `tinytorchutil-0.1.2/setup.py` & `tinytorchutil-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from setuptools import setup, find_packages
 
 setup(
     name='tinytorchutil',
-    version='0.1.2',
+    version='0.1.3',
     packages=find_packages(),
     description='A personal collection of small utility functions for PyTorch and DL development.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Chainathan',
     install_requires=[
     'torch',
     'matplotlib',
     'numpy',
     'fastcore',
     'fastprogress',
     'torcheval',
+    'wandb'
     ],
     python_requires='>=3.6',
 )
```

### Comparing `tinytorchutil-0.1.2/tinytorchutil/tinytorchutil.py` & `tinytorchutil-0.1.3/tinytorchutil/tinytorchutil.py`

 * *Files identical despite different names*

