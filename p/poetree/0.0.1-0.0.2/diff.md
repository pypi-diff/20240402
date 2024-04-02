# Comparing `tmp/poetree-0.0.1.tar.gz` & `tmp/poetree-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/poetree-0.0.1.tar", last modified: Tue Apr  2 11:22:15 2024, max compression
+gzip compressed data, was "dist/poetree-0.0.2.tar", last modified: Tue Apr  2 14:09:45 2024, max compression
```

## Comparing `poetree-0.0.1.tar` & `poetree-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 L-plecha0000   (504) staff       (20)        0 2024-04-02 11:22:15.417661 poetree-0.0.1/
--rw-r--r--   0 L-plecha0000   (504) staff       (20)     1065 2022-05-13 18:11:31.000000 poetree-0.0.1/LICENSE.txt
--rw-r--r--   0 L-plecha0000   (504) staff       (20)     9955 2024-04-02 11:22:15.418239 poetree-0.0.1/PKG-INFO
--rw-r--r--   0 L-plecha0000   (504) staff       (20)     8821 2024-04-02 11:16:28.000000 poetree-0.0.1/README.md
-drwxr-xr-x   0 L-plecha0000   (504) staff       (20)        0 2024-04-02 11:22:15.356728 poetree-0.0.1/poetree/
--rw-r--r--   0 L-plecha0000   (504) staff       (20)      170 2024-04-02 07:25:27.000000 poetree-0.0.1/poetree/__init__.py
--rw-r--r--   0 L-plecha0000   (504) staff       (20)     5931 2024-01-05 10:27:59.000000 poetree-0.0.1/poetree/author.py
--rw-r--r--   0 L-plecha0000   (504) staff       (20)       47 2024-04-02 07:35:02.000000 poetree-0.0.1/poetree/config.py
--rw-r--r--   0 L-plecha0000   (504) staff       (20)     5510 2024-01-08 10:06:17.000000 poetree-0.0.1/poetree/corpus.py
--rw-r--r--   0 L-plecha0000   (504) staff       (20)     3334 2024-01-05 10:26:49.000000 poetree-0.0.1/poetree/glob.py
--rw-r--r--   0 L-plecha0000   (504) staff       (20)     2319 2024-01-05 10:28:07.000000 poetree-0.0.1/poetree/main.py
--rw-r--r--   0 L-plecha0000   (504) staff       (20)     4679 2024-01-08 12:53:57.000000 poetree-0.0.1/poetree/poem.py
--rw-r--r--   0 L-plecha0000   (504) staff       (20)     4814 2024-01-05 10:28:03.000000 poetree-0.0.1/poetree/source.py
-drwxr-xr-x   0 L-plecha0000   (504) staff       (20)        0 2024-04-02 11:22:15.416606 poetree-0.0.1/poetree.egg-info/
--rw-r--r--   0 L-plecha0000   (504) staff       (20)     9955 2024-04-02 11:22:14.000000 poetree-0.0.1/poetree.egg-info/PKG-INFO
--rw-r--r--   0 L-plecha0000   (504) staff       (20)      334 2024-04-02 11:22:15.000000 poetree-0.0.1/poetree.egg-info/SOURCES.txt
--rw-r--r--   0 L-plecha0000   (504) staff       (20)        1 2024-04-02 11:22:14.000000 poetree-0.0.1/poetree.egg-info/dependency_links.txt
--rw-r--r--   0 L-plecha0000   (504) staff       (20)       23 2024-04-02 11:22:14.000000 poetree-0.0.1/poetree.egg-info/requires.txt
--rw-r--r--   0 L-plecha0000   (504) staff       (20)        8 2024-04-02 11:22:14.000000 poetree-0.0.1/poetree.egg-info/top_level.txt
--rw-r--r--   0 L-plecha0000   (504) staff       (20)       79 2024-04-02 11:22:15.442939 poetree-0.0.1/setup.cfg
--rw-r--r--   0 L-plecha0000   (504) staff       (20)     1570 2024-04-02 07:37:24.000000 poetree-0.0.1/setup.py
+drwxr-xr-x   0 L-plecha0000   (504) staff       (20)        0 2024-04-02 14:09:45.168097 poetree-0.0.2/
+-rw-r--r--   0 L-plecha0000   (504) staff       (20)     1065 2022-05-13 18:11:31.000000 poetree-0.0.2/LICENSE.txt
+-rw-r--r--   0 L-plecha0000   (504) staff       (20)     9964 2024-04-02 14:09:45.168418 poetree-0.0.2/PKG-INFO
+-rw-r--r--   0 L-plecha0000   (504) staff       (20)     8821 2024-04-02 11:16:28.000000 poetree-0.0.2/README.md
+drwxr-xr-x   0 L-plecha0000   (504) staff       (20)        0 2024-04-02 14:09:45.133038 poetree-0.0.2/poetree/
+-rw-r--r--   0 L-plecha0000   (504) staff       (20)      170 2024-04-02 07:25:27.000000 poetree-0.0.2/poetree/__init__.py
+-rw-r--r--   0 L-plecha0000   (504) staff       (20)     5931 2024-01-05 10:27:59.000000 poetree-0.0.2/poetree/author.py
+-rw-r--r--   0 L-plecha0000   (504) staff       (20)       47 2024-04-02 07:35:02.000000 poetree-0.0.2/poetree/config.py
+-rw-r--r--   0 L-plecha0000   (504) staff       (20)     5510 2024-01-08 10:06:17.000000 poetree-0.0.2/poetree/corpus.py
+-rw-r--r--   0 L-plecha0000   (504) staff       (20)     3334 2024-01-05 10:26:49.000000 poetree-0.0.2/poetree/glob.py
+-rw-r--r--   0 L-plecha0000   (504) staff       (20)     2319 2024-01-05 10:28:07.000000 poetree-0.0.2/poetree/main.py
+-rw-r--r--   0 L-plecha0000   (504) staff       (20)     4679 2024-01-08 12:53:57.000000 poetree-0.0.2/poetree/poem.py
+-rw-r--r--   0 L-plecha0000   (504) staff       (20)     4814 2024-01-05 10:28:03.000000 poetree-0.0.2/poetree/source.py
+drwxr-xr-x   0 L-plecha0000   (504) staff       (20)        0 2024-04-02 14:09:45.167360 poetree-0.0.2/poetree.egg-info/
+-rw-r--r--   0 L-plecha0000   (504) staff       (20)     9964 2024-04-02 14:09:44.000000 poetree-0.0.2/poetree.egg-info/PKG-INFO
+-rw-r--r--   0 L-plecha0000   (504) staff       (20)      334 2024-04-02 14:09:44.000000 poetree-0.0.2/poetree.egg-info/SOURCES.txt
+-rw-r--r--   0 L-plecha0000   (504) staff       (20)        1 2024-04-02 14:09:44.000000 poetree-0.0.2/poetree.egg-info/dependency_links.txt
+-rw-r--r--   0 L-plecha0000   (504) staff       (20)       23 2024-04-02 14:09:44.000000 poetree-0.0.2/poetree.egg-info/requires.txt
+-rw-r--r--   0 L-plecha0000   (504) staff       (20)        8 2024-04-02 14:09:44.000000 poetree-0.0.2/poetree.egg-info/top_level.txt
+-rw-r--r--   0 L-plecha0000   (504) staff       (20)       79 2024-04-02 14:09:45.172273 poetree-0.0.2/setup.cfg
+-rw-r--r--   0 L-plecha0000   (504) staff       (20)     1579 2024-04-02 14:06:24.000000 poetree-0.0.2/setup.py
```

### Comparing `poetree-0.0.1/LICENSE.txt` & `poetree-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `poetree-0.0.1/PKG-INFO` & `poetree-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: poetree
-Version: 0.0.1
+Version: 0.0.2
 Summary: An easy way to get data from PoeTree dataset
 Home-page: https://github.com/versotym/poetree
-Download-URL: https://github.com/versotym/poetree/archive/v0.0.1.tar.gz
+Download-URL: https://github.com/versotym/poetree/archive/refs/tags/0.0.2.tar.gz
 Author: Petr Plechac
 Author-email: plechac@ucl.cas.cz
 License: MIT
 Keywords: poetry,corpus,versification
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Text Processing :: Linguistic
```

### Comparing `poetree-0.0.1/README.md` & `poetree-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `poetree-0.0.1/poetree/author.py` & `poetree-0.0.2/poetree/author.py`

 * *Files identical despite different names*

### Comparing `poetree-0.0.1/poetree/corpus.py` & `poetree-0.0.2/poetree/corpus.py`

 * *Files identical despite different names*

### Comparing `poetree-0.0.1/poetree/glob.py` & `poetree-0.0.2/poetree/glob.py`

 * *Files identical despite different names*

### Comparing `poetree-0.0.1/poetree/main.py` & `poetree-0.0.2/poetree/main.py`

 * *Files identical despite different names*

### Comparing `poetree-0.0.1/poetree/poem.py` & `poetree-0.0.2/poetree/poem.py`

 * *Files identical despite different names*

### Comparing `poetree-0.0.1/poetree/source.py` & `poetree-0.0.2/poetree/source.py`

 * *Files identical despite different names*

### Comparing `poetree-0.0.1/poetree.egg-info/PKG-INFO` & `poetree-0.0.2/poetree.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: poetree
-Version: 0.0.1
+Version: 0.0.2
 Summary: An easy way to get data from PoeTree dataset
 Home-page: https://github.com/versotym/poetree
-Download-URL: https://github.com/versotym/poetree/archive/v0.0.1.tar.gz
+Download-URL: https://github.com/versotym/poetree/archive/refs/tags/0.0.2.tar.gz
 Author: Petr Plechac
 Author-email: plechac@ucl.cas.cz
 License: MIT
 Keywords: poetry,corpus,versification
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Text Processing :: Linguistic
```

### Comparing `poetree-0.0.1/setup.py` & `poetree-0.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,21 +7,21 @@
     long_description = f.read()
 
 setup(
   name = 'poetree',
   long_description_content_type='text/markdown',
   long_description=long_description,
   packages = ['poetree'],   
-  version = '0.0.1',      
+  version = '0.0.2',      
   license='MIT',        
   description = 'An easy way to get data from PoeTree dataset',   
   author = 'Petr Plechac',                   
   author_email = 'plechac@ucl.cas.cz',      
   url = 'https://github.com/versotym/poetree',
-  download_url = 'https://github.com/versotym/poetree/archive/v0.0.1.tar.gz',
+  download_url = 'https://github.com/versotym/poetree/archive/refs/tags/0.0.2.tar.gz',
   keywords = ['poetry', 'corpus', 'versification'],
   install_requires=[           
           'typing',
           'pandas',
           'tabulate',
       ],
   classifiers=[
```

