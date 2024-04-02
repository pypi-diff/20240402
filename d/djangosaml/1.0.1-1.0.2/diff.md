# Comparing `tmp/djangosaml-1.0.1.tar.gz` & `tmp/djangosaml-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangosaml-1.0.1.tar", last modified: Thu Mar 28 17:57:24 2024, max compression
+gzip compressed data, was "djangosaml-1.0.2.tar", last modified: Tue Apr  2 03:19:27 2024, max compression
```

## Comparing `djangosaml-1.0.1.tar` & `djangosaml-1.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2024-03-28 17:57:24.589703 djangosaml-1.0.1/
--rw-rw-r--   0 suhail    (1000) suhail    (1000)      747 2024-03-28 14:37:13.000000 djangosaml-1.0.1/AUTHORS.rst
--rw-rw-r--   0 suhail    (1000) suhail    (1000)      552 2024-03-28 14:12:41.000000 djangosaml-1.0.1/LICENSE
--rw-rw-r--   0 suhail    (1000) suhail    (1000)      120 2024-03-28 14:37:43.000000 djangosaml-1.0.1/MANIFEST.in
--rw-r--r--   0 suhail    (1000) suhail    (1000)     2888 2024-03-28 17:57:24.589703 djangosaml-1.0.1/PKG-INFO
--rw-rw-r--   0 suhail    (1000) suhail    (1000)     1959 2024-03-28 17:57:10.000000 djangosaml-1.0.1/README.md
-drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2024-03-28 17:57:24.589703 djangosaml-1.0.1/djangosaml/
--rw-rw-r--   0 suhail    (1000) suhail    (1000)       24 2024-03-28 14:34:06.000000 djangosaml-1.0.1/djangosaml/__init__.py
-drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2024-03-28 17:57:24.585702 djangosaml-1.0.1/djangosaml/templates/
-drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2024-03-28 17:57:24.589703 djangosaml-1.0.1/djangosaml/templates/djangosaml/
--rw-rw-r--   0 suhail    (1000) suhail    (1000)      327 2024-03-28 14:34:06.000000 djangosaml-1.0.1/djangosaml/templates/djangosaml/denied.html
--rw-rw-r--   0 suhail    (1000) suhail    (1000)      308 2024-03-28 14:34:06.000000 djangosaml-1.0.1/djangosaml/templates/djangosaml/signout.html
--rw-rw-r--   0 suhail    (1000) suhail    (1000)      275 2024-03-28 14:34:57.000000 djangosaml-1.0.1/djangosaml/urls.py
--rw-rw-r--   0 suhail    (1000) suhail    (1000)     8965 2024-03-28 14:46:51.000000 djangosaml-1.0.1/djangosaml/views.py
-drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2024-03-28 17:57:24.589703 djangosaml-1.0.1/djangosaml.egg-info/
--rw-r--r--   0 suhail    (1000) suhail    (1000)     2888 2024-03-28 17:57:24.000000 djangosaml-1.0.1/djangosaml.egg-info/PKG-INFO
--rw-rw-r--   0 suhail    (1000) suhail    (1000)      380 2024-03-28 17:57:24.000000 djangosaml-1.0.1/djangosaml.egg-info/SOURCES.txt
--rw-rw-r--   0 suhail    (1000) suhail    (1000)        1 2024-03-28 17:57:24.000000 djangosaml-1.0.1/djangosaml.egg-info/dependency_links.txt
--rw-rw-r--   0 suhail    (1000) suhail    (1000)       15 2024-03-28 17:57:24.000000 djangosaml-1.0.1/djangosaml.egg-info/requires.txt
--rw-rw-r--   0 suhail    (1000) suhail    (1000)       11 2024-03-28 17:57:24.000000 djangosaml-1.0.1/djangosaml.egg-info/top_level.txt
--rw-rw-r--   0 suhail    (1000) suhail    (1000)       67 2024-03-28 17:57:24.589703 djangosaml-1.0.1/setup.cfg
--rw-rw-r--   0 suhail    (1000) suhail    (1000)     1343 2024-03-28 17:26:23.000000 djangosaml-1.0.1/setup.py
+drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2024-04-02 03:19:27.497859 djangosaml-1.0.2/
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)      745 2024-04-02 03:17:57.000000 djangosaml-1.0.2/AUTHORS.rst
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)      552 2024-03-29 02:19:57.000000 djangosaml-1.0.2/LICENSE
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)      120 2024-03-29 02:19:57.000000 djangosaml-1.0.2/MANIFEST.in
+-rw-r--r--   0 suhail    (1000) suhail    (1000)     2711 2024-04-02 03:19:27.497859 djangosaml-1.0.2/PKG-INFO
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)     1783 2024-04-02 03:17:57.000000 djangosaml-1.0.2/README.md
+drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2024-04-02 03:19:27.493859 djangosaml-1.0.2/djangosaml/
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)       24 2024-03-29 02:19:57.000000 djangosaml-1.0.2/djangosaml/__init__.py
+drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2024-04-02 03:19:27.493859 djangosaml-1.0.2/djangosaml/templates/
+drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2024-04-02 03:19:27.497859 djangosaml-1.0.2/djangosaml/templates/djangosaml/
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)      327 2024-03-29 02:19:57.000000 djangosaml-1.0.2/djangosaml/templates/djangosaml/denied.html
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)      308 2024-03-29 02:19:57.000000 djangosaml-1.0.2/djangosaml/templates/djangosaml/signout.html
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)      295 2024-04-02 03:17:34.000000 djangosaml-1.0.2/djangosaml/urls.py
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)     8965 2024-03-29 11:15:58.000000 djangosaml-1.0.2/djangosaml/views.py
+drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2024-04-02 03:19:27.497859 djangosaml-1.0.2/djangosaml.egg-info/
+-rw-r--r--   0 suhail    (1000) suhail    (1000)     2711 2024-04-02 03:19:27.000000 djangosaml-1.0.2/djangosaml.egg-info/PKG-INFO
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)      380 2024-04-02 03:19:27.000000 djangosaml-1.0.2/djangosaml.egg-info/SOURCES.txt
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)        1 2024-04-02 03:19:27.000000 djangosaml-1.0.2/djangosaml.egg-info/dependency_links.txt
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)       15 2024-04-02 03:19:27.000000 djangosaml-1.0.2/djangosaml.egg-info/requires.txt
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)       11 2024-04-02 03:19:27.000000 djangosaml-1.0.2/djangosaml.egg-info/top_level.txt
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)       67 2024-04-02 03:19:27.497859 djangosaml-1.0.2/setup.cfg
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)     1342 2024-04-02 03:18:15.000000 djangosaml-1.0.2/setup.py
```

### Comparing `djangosaml-1.0.1/AUTHORS.rst` & `djangosaml-1.0.2/AUTHORS.rst`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 -----------------
 
 - Fang Li
 
 Django Saml
 -----------
 
-- Suhail vs
+- Fang Li
 
 Pysaml2
 -------
 
 - Roland Hedberg and it's contributors
```

### Comparing `djangosaml-1.0.1/LICENSE` & `djangosaml-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `djangosaml-1.0.1/djangosaml/views.py` & `djangosaml-1.0.2/djangosaml/views.py`

 * *Files identical despite different names*

### Comparing `djangosaml-1.0.1/setup.py` & `djangosaml-1.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,23 +7,23 @@
 # Get the long description from the README file
 def read(f):
     with open(f, 'r', encoding='utf-8') as file:
         return file.read()
     
 setup(
     name='djangosaml',
-    version='1.0.1',
+    version='1.0.2',
     description='Django SAML2 Authentication Made Easy. Easily integrate with SAML2 SSO identity providers like Okta',
     long_description=read('README.md'),
     long_description_content_type='text/markdown',
 
     url='https://djangosaml.readthedocs.io/en/latest/',
 
-    author='Fang Li & Suhail vs',
-    author_email='suhailvs@gmail.com',
+    author='Fang Li',
+    author_email='lorenzo.gil.sanchez@gmail.com',
 
     license='Apache 2.0',
 
     classifiers=[
         'Development Status :: 5 - Production/Stable',
 
         'Intended Audience :: Developers',
```

