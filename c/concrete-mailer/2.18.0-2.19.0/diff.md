# Comparing `tmp/concrete-mailer-2.18.0.tar.gz` & `tmp/concrete-mailer-2.19.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/concrete-mailer-2.18.0.tar", last modified: Fri Feb 18 17:55:40 2022, max compression
+gzip compressed data, was "dist/concrete-mailer-2.19.0.tar", last modified: Tue Apr  2 18:35:09 2024, max compression
```

## Comparing `concrete-mailer-2.18.0.tar` & `concrete-mailer-2.19.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 lco        (503) staff       (20)        0 2022-02-18 17:55:40.000000 concrete-mailer-2.18.0/
--rw-r--r--   0 lco        (503) staff       (20)    35149 2020-01-28 21:40:26.000000 concrete-mailer-2.18.0/LICENSE
--rw-r--r--   0 lco        (503) staff       (20)     5896 2022-02-18 17:55:40.000000 concrete-mailer-2.18.0/PKG-INFO
--rw-r--r--   0 lco        (503) staff       (20)     4973 2020-02-20 23:53:01.000000 concrete-mailer-2.18.0/README.md
-drwxr-xr-x   0 lco        (503) staff       (20)        0 2022-02-18 17:55:40.000000 concrete-mailer-2.18.0/concrete_mailer/
--rw-r--r--   0 lco        (503) staff       (20)      191 2022-02-18 17:52:43.000000 concrete-mailer-2.18.0/concrete_mailer/__init__.py
--rw-r--r--   0 lco        (503) staff       (20)     2047 2020-02-04 22:13:07.000000 concrete-mailer-2.18.0/concrete_mailer/client.py
--rw-r--r--   0 lco        (503) staff       (20)     5761 2021-03-02 13:59:20.000000 concrete-mailer-2.18.0/concrete_mailer/preparers.py
--rw-r--r--   0 lco        (503) staff       (20)     1079 2020-02-13 17:49:47.000000 concrete-mailer-2.18.0/concrete_mailer/utils.py
-drwxr-xr-x   0 lco        (503) staff       (20)        0 2022-02-18 17:55:40.000000 concrete-mailer-2.18.0/concrete_mailer.egg-info/
--rw-r--r--   0 lco        (503) staff       (20)     5896 2022-02-18 17:55:40.000000 concrete-mailer-2.18.0/concrete_mailer.egg-info/PKG-INFO
--rw-r--r--   0 lco        (503) staff       (20)      376 2022-02-18 17:55:40.000000 concrete-mailer-2.18.0/concrete_mailer.egg-info/SOURCES.txt
--rw-r--r--   0 lco        (503) staff       (20)        1 2022-02-18 17:55:40.000000 concrete-mailer-2.18.0/concrete_mailer.egg-info/dependency_links.txt
--rw-r--r--   0 lco        (503) staff       (20)        1 2020-02-11 09:13:34.000000 concrete-mailer-2.18.0/concrete_mailer.egg-info/not-zip-safe
--rw-r--r--   0 lco        (503) staff       (20)      180 2022-02-18 17:55:40.000000 concrete-mailer-2.18.0/concrete_mailer.egg-info/requires.txt
--rw-r--r--   0 lco        (503) staff       (20)       16 2022-02-18 17:55:40.000000 concrete-mailer-2.18.0/concrete_mailer.egg-info/top_level.txt
--rw-r--r--   0 lco        (503) staff       (20)     1632 2022-02-18 17:55:40.000000 concrete-mailer-2.18.0/setup.cfg
--rw-r--r--   0 lco        (503) staff       (20)       54 2020-01-28 21:20:44.000000 concrete-mailer-2.18.0/setup.py
+drwxr-xr-x   0 lco        (503) staff       (20)        0 2024-04-02 18:35:09.000000 concrete-mailer-2.19.0/
+-rw-r--r--   0 lco        (503) staff       (20)    35149 2020-01-28 21:40:26.000000 concrete-mailer-2.19.0/LICENSE
+-rw-r--r--   0 lco        (503) staff       (20)     5896 2024-04-02 18:35:09.000000 concrete-mailer-2.19.0/PKG-INFO
+-rw-r--r--   0 lco        (503) staff       (20)     4973 2020-02-20 23:53:01.000000 concrete-mailer-2.19.0/README.md
+drwxr-xr-x   0 lco        (503) staff       (20)        0 2024-04-02 18:35:09.000000 concrete-mailer-2.19.0/concrete_mailer/
+-rw-r--r--   0 lco        (503) staff       (20)      191 2024-04-02 18:35:04.000000 concrete-mailer-2.19.0/concrete_mailer/__init__.py
+-rw-r--r--   0 lco        (503) staff       (20)     2047 2020-02-04 22:13:07.000000 concrete-mailer-2.19.0/concrete_mailer/client.py
+-rw-r--r--   0 lco        (503) staff       (20)     5761 2024-04-02 18:35:00.000000 concrete-mailer-2.19.0/concrete_mailer/preparers.py
+-rw-r--r--   0 lco        (503) staff       (20)     1079 2020-02-13 17:49:47.000000 concrete-mailer-2.19.0/concrete_mailer/utils.py
+drwxr-xr-x   0 lco        (503) staff       (20)        0 2024-04-02 18:35:09.000000 concrete-mailer-2.19.0/concrete_mailer.egg-info/
+-rw-r--r--   0 lco        (503) staff       (20)     5896 2024-04-02 18:35:09.000000 concrete-mailer-2.19.0/concrete_mailer.egg-info/PKG-INFO
+-rw-r--r--   0 lco        (503) staff       (20)      376 2024-04-02 18:35:09.000000 concrete-mailer-2.19.0/concrete_mailer.egg-info/SOURCES.txt
+-rw-r--r--   0 lco        (503) staff       (20)        1 2024-04-02 18:35:09.000000 concrete-mailer-2.19.0/concrete_mailer.egg-info/dependency_links.txt
+-rw-r--r--   0 lco        (503) staff       (20)        1 2020-02-11 09:13:34.000000 concrete-mailer-2.19.0/concrete_mailer.egg-info/not-zip-safe
+-rw-r--r--   0 lco        (503) staff       (20)      180 2024-04-02 18:35:09.000000 concrete-mailer-2.19.0/concrete_mailer.egg-info/requires.txt
+-rw-r--r--   0 lco        (503) staff       (20)       16 2024-04-02 18:35:09.000000 concrete-mailer-2.19.0/concrete_mailer.egg-info/top_level.txt
+-rw-r--r--   0 lco        (503) staff       (20)     1632 2024-04-02 18:35:09.000000 concrete-mailer-2.19.0/setup.cfg
+-rw-r--r--   0 lco        (503) staff       (20)       54 2020-01-28 21:20:44.000000 concrete-mailer-2.19.0/setup.py
```

### Comparing `concrete-mailer-2.18.0/LICENSE` & `concrete-mailer-2.19.0/LICENSE`

 * *Files identical despite different names*

### Comparing `concrete-mailer-2.18.0/PKG-INFO` & `concrete-mailer-2.19.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: concrete-mailer
-Version: 2.18.0
+Version: 2.19.0
 Summary: Python package for sending rich e-mails.
 Home-page: https://github.com/Netsach/concrete-mailer/
 Author: Netsach
 Author-email: contact@netsach.org
 License: GNU GENERAL PUBLIC LICENSE Version 3
 Project-URL: Bug Tracker, https://github.com/Netsach/concrete-mailer/issues
 Project-URL: Documentation, https://github.com/Netsach/concrete-mailer/blob/master/README.md
```

### Comparing `concrete-mailer-2.18.0/README.md` & `concrete-mailer-2.19.0/README.md`

 * *Files identical despite different names*

### Comparing `concrete-mailer-2.18.0/concrete_mailer/client.py` & `concrete-mailer-2.19.0/concrete_mailer/client.py`

 * *Files identical despite different names*

### Comparing `concrete-mailer-2.18.0/concrete_mailer/preparers.py` & `concrete-mailer-2.19.0/concrete_mailer/preparers.py`

 * *Files identical despite different names*

### Comparing `concrete-mailer-2.18.0/concrete_mailer/utils.py` & `concrete-mailer-2.19.0/concrete_mailer/utils.py`

 * *Files identical despite different names*

### Comparing `concrete-mailer-2.18.0/concrete_mailer.egg-info/PKG-INFO` & `concrete-mailer-2.19.0/concrete_mailer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: concrete-mailer
-Version: 2.18.0
+Version: 2.19.0
 Summary: Python package for sending rich e-mails.
 Home-page: https://github.com/Netsach/concrete-mailer/
 Author: Netsach
 Author-email: contact@netsach.org
 License: GNU GENERAL PUBLIC LICENSE Version 3
 Project-URL: Bug Tracker, https://github.com/Netsach/concrete-mailer/issues
 Project-URL: Documentation, https://github.com/Netsach/concrete-mailer/blob/master/README.md
```

### Comparing `concrete-mailer-2.18.0/setup.cfg` & `concrete-mailer-2.19.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 version = attr: concrete_mailer.__version__
 author = Netsach
 author_email = contact@netsach.org
 description = Python package for sending rich e-mails.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = GNU GENERAL PUBLIC LICENSE Version 3
-license-file = LICENSE
-home-page = https://github.com/Netsach/concrete-mailer/
+license_file = LICENSE
+home_page = https://github.com/Netsach/concrete-mailer/
 project_urls = 
 	Bug Tracker = https://github.com/Netsach/concrete-mailer/issues
 	Documentation = https://github.com/Netsach/concrete-mailer/blob/master/README.md
 	Source Code = https://github.com/Netsach/concrete-mailer/
 	Coverage = https://codecov.io/gh/Netsach/concrete-mailer
 classifiers = 
 	Programming Language :: Python :: 2.7
```

