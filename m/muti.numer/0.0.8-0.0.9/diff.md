# Comparing `tmp/muti.numer-0.0.8.tar.gz` & `tmp/muti.numer-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muti.numer-0.0.8.tar", last modified: Tue Apr  2 11:05:06 2024, max compression
+gzip compressed data, was "muti.numer-0.0.9.tar", last modified: Tue Apr  2 11:07:18 2024, max compression
```

## Comparing `muti.numer-0.0.8.tar` & `muti.numer-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 11:05:06.286867 muti.numer-0.0.8/
--rw-rw-rw-   0        0        0     1089 2024-03-22 08:37:41.000000 muti.numer-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      767 2024-04-02 11:05:06.285866 muti.numer-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      346 2024-03-29 10:24:16.000000 muti.numer-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-04-02 11:05:06.285866 muti.numer-0.0.8/muti.numer.egg-info/
--rw-rw-rw-   0        0        0      767 2024-04-02 11:05:06.000000 muti.numer-0.0.8/muti.numer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      294 2024-04-02 11:05:06.000000 muti.numer-0.0.8/muti.numer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 11:05:06.000000 muti.numer-0.0.8/muti.numer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-04-02 11:05:06.000000 muti.numer-0.0.8/muti.numer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-02 11:05:06.284866 muti.numer-0.0.8/numer/
--rw-rw-rw-   0        0        0     1371 2024-04-02 10:48:11.000000 muti.numer-0.0.8/numer/__deps__.py
--rw-rw-rw-   0        0        0      905 2024-04-02 11:04:26.000000 muti.numer-0.0.8/numer/__init__.py
--rw-rw-rw-   0        0        0      280 2024-04-02 09:11:21.000000 muti.numer-0.0.8/numer/betLam.py
--rw-rw-rw-   0        0        0     2326 2024-04-02 06:48:19.000000 muti.numer-0.0.8/numer/depLam.py
--rw-rw-rw-   0        0        0      146 2024-04-02 10:23:28.000000 muti.numer-0.0.8/numer/getLam.py
--rw-rw-rw-   0        0        0      903 2024-04-02 08:49:06.000000 muti.numer-0.0.8/numer/iniLam.py
--rw-rw-rw-   0        0        0     1765 2024-04-02 08:48:37.000000 muti.numer-0.0.8/numer/modLas.py
--rw-rw-rw-   0        0        0     9356 2024-04-02 11:01:41.000000 muti.numer-0.0.8/numer/shfLam.py
--rw-rw-rw-   0        0        0       42 2024-04-02 11:05:06.286867 muti.numer-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      653 2024-04-02 11:04:52.000000 muti.numer-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 11:07:18.405618 muti.numer-0.0.9/
+-rw-rw-rw-   0        0        0     1089 2024-03-22 08:37:41.000000 muti.numer-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      767 2024-04-02 11:07:18.405618 muti.numer-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      346 2024-03-29 10:24:16.000000 muti.numer-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 11:07:18.404618 muti.numer-0.0.9/muti.numer.egg-info/
+-rw-rw-rw-   0        0        0      767 2024-04-02 11:07:18.000000 muti.numer-0.0.9/muti.numer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2024-04-02 11:07:18.000000 muti.numer-0.0.9/muti.numer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 11:07:18.000000 muti.numer-0.0.9/muti.numer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-02 11:07:18.000000 muti.numer-0.0.9/muti.numer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-02 11:07:18.404618 muti.numer-0.0.9/numer/
+-rw-rw-rw-   0        0        0     1371 2024-04-02 10:48:11.000000 muti.numer-0.0.9/numer/__deps__.py
+-rw-rw-rw-   0        0        0      916 2024-04-02 11:06:53.000000 muti.numer-0.0.9/numer/__init__.py
+-rw-rw-rw-   0        0        0      280 2024-04-02 09:11:21.000000 muti.numer-0.0.9/numer/betLam.py
+-rw-rw-rw-   0        0        0     2326 2024-04-02 06:48:19.000000 muti.numer-0.0.9/numer/depLam.py
+-rw-rw-rw-   0        0        0      146 2024-04-02 10:23:28.000000 muti.numer-0.0.9/numer/getLam.py
+-rw-rw-rw-   0        0        0      903 2024-04-02 08:49:06.000000 muti.numer-0.0.9/numer/iniLam.py
+-rw-rw-rw-   0        0        0     1765 2024-04-02 08:48:37.000000 muti.numer-0.0.9/numer/modLas.py
+-rw-rw-rw-   0        0        0     9356 2024-04-02 11:01:41.000000 muti.numer-0.0.9/numer/shfLam.py
+-rw-rw-rw-   0        0        0       42 2024-04-02 11:07:18.405618 muti.numer-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      653 2024-04-02 11:07:13.000000 muti.numer-0.0.9/setup.py
```

### Comparing `muti.numer-0.0.8/LICENSE` & `muti.numer-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `muti.numer-0.0.8/PKG-INFO` & `muti.numer-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muti.numer
-Version: 0.0.8
+Version: 0.0.9
 Summary: utils for math-numer
 Home-page: https://github.com/E-C-Ares/
 Author: E.C.Ares
 Author-email: E.C.Ares@outlook.com
 License: MIT DIVIƷON
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `muti.numer-0.0.8/muti.numer.egg-info/PKG-INFO` & `muti.numer-0.0.9/muti.numer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muti.numer
-Version: 0.0.8
+Version: 0.0.9
 Summary: utils for math-numer
 Home-page: https://github.com/E-C-Ares/
 Author: E.C.Ares
 Author-email: E.C.Ares@outlook.com
 License: MIT DIVIƷON
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `muti.numer-0.0.8/numer/__deps__.py` & `muti.numer-0.0.9/numer/__deps__.py`

 * *Files identical despite different names*

### Comparing `muti.numer-0.0.8/numer/__init__.py` & `muti.numer-0.0.9/numer/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 _JC_NYM = "muti.torch"
+import os
 
 _fc  =  os.getenv( 'FC_IMP')
 if _fc is NON or _fc== '': _fc='tn'
 if 'j' in _fc:
     import jax       as nmb
     import jax.numpy as nmp
     import jax.nn    as nmm
```

### Comparing `muti.numer-0.0.8/numer/depLam.py` & `muti.numer-0.0.9/numer/depLam.py`

 * *Files identical despite different names*

### Comparing `muti.numer-0.0.8/numer/iniLam.py` & `muti.numer-0.0.9/numer/iniLam.py`

 * *Files identical despite different names*

### Comparing `muti.numer-0.0.8/numer/modLas.py` & `muti.numer-0.0.9/numer/modLas.py`

 * *Files identical despite different names*

### Comparing `muti.numer-0.0.8/numer/shfLam.py` & `muti.numer-0.0.9/numer/shfLam.py`

 * *Files identical despite different names*

### Comparing `muti.numer-0.0.8/setup.py` & `muti.numer-0.0.9/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   url          = "https://github.com/E-C-Ares/",
   name         = "muti.numer",
-  version      = "0.0.8",
+  version      = "0.0.9",
   author       = "E.C.Ares",
   author_email = "E.C.Ares@outlook.com",
   license      = 'MIT DIVIƷON',
   description  = "utils for math-numer",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages     = setuptools.find_packages(),
```

