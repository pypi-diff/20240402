# Comparing `tmp/aiohutils-0.9.1.tar.gz` & `tmp/aiohutils-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiohutils-0.9.1.tar", last modified: Fri Aug 11 14:51:25 2023, max compression
+gzip compressed data, was "aiohutils-0.9.2.tar", last modified: Fri Aug 11 15:47:29 2023, max compression
```

## Comparing `aiohutils-0.9.1.tar` & `aiohutils-0.9.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-08-11 14:51:25.079949 aiohutils-0.9.1/
--rw-rw-rw-   0        0        0      666 2023-08-11 14:51:25.073444 aiohutils-0.9.1/PKG-INFO
--rw-rw-rw-   0        0        0      203 2023-08-11 14:48:41.000000 aiohutils-0.9.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-08-11 14:51:25.057822 aiohutils-0.9.1/aiohutils/
--rw-rw-rw-   0        0        0       22 2023-08-11 14:51:22.000000 aiohutils-0.9.1/aiohutils/__init__.py
--rw-rw-rw-   0        0        0     1130 2023-08-06 04:19:10.000000 aiohutils-0.9.1/aiohutils/session.py
--rw-rw-rw-   0        0        0     2946 2023-08-03 07:49:19.000000 aiohutils-0.9.1/aiohutils/tests.py
-drwxrwxrwx   0        0        0        0 2023-08-11 14:51:25.073444 aiohutils-0.9.1/aiohutils.egg-info/
--rw-rw-rw-   0        0        0      666 2023-08-11 14:51:24.000000 aiohutils-0.9.1/aiohutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2023-08-11 14:51:24.000000 aiohutils-0.9.1/aiohutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-11 14:51:24.000000 aiohutils-0.9.1/aiohutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-08-11 14:51:24.000000 aiohutils-0.9.1/aiohutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-08-11 14:51:24.000000 aiohutils-0.9.1/aiohutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-08-03 06:59:05.000000 aiohutils-0.9.1/aiohutils.egg-info/zip-safe
--rw-rw-rw-   0        0        0      967 2023-08-03 07:01:19.000000 aiohutils-0.9.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-11 14:51:25.079949 aiohutils-0.9.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-11 15:47:29.129942 aiohutils-0.9.2/
+-rw-rw-rw-   0        0        0      688 2023-08-11 15:47:29.129942 aiohutils-0.9.2/PKG-INFO
+-rw-rw-rw-   0        0        0      203 2023-08-11 14:48:41.000000 aiohutils-0.9.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-08-11 15:47:29.129942 aiohutils-0.9.2/aiohutils/
+-rw-rw-rw-   0        0        0       22 2023-08-11 15:47:26.000000 aiohutils-0.9.2/aiohutils/__init__.py
+-rw-rw-rw-   0        0        0     1130 2023-08-06 04:19:10.000000 aiohutils-0.9.2/aiohutils/session.py
+-rw-rw-rw-   0        0        0     2946 2023-08-03 07:49:19.000000 aiohutils-0.9.2/aiohutils/tests.py
+drwxrwxrwx   0        0        0        0 2023-08-11 15:47:29.129942 aiohutils-0.9.2/aiohutils.egg-info/
+-rw-rw-rw-   0        0        0      688 2023-08-11 15:47:28.000000 aiohutils-0.9.2/aiohutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2023-08-11 15:47:29.000000 aiohutils-0.9.2/aiohutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-11 15:47:28.000000 aiohutils-0.9.2/aiohutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-08-11 15:47:28.000000 aiohutils-0.9.2/aiohutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-08-11 15:47:28.000000 aiohutils-0.9.2/aiohutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-08-03 06:59:05.000000 aiohutils-0.9.2/aiohutils.egg-info/zip-safe
+-rw-rw-rw-   0        0        0     1041 2023-08-11 15:46:48.000000 aiohutils-0.9.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-11 15:47:29.129942 aiohutils-0.9.2/setup.cfg
```

### Comparing `aiohutils-0.9.1/aiohutils/session.py` & `aiohutils-0.9.2/aiohutils/session.py`

 * *Files identical despite different names*

### Comparing `aiohutils-0.9.1/aiohutils/tests.py` & `aiohutils-0.9.2/aiohutils/tests.py`

 * *Files identical despite different names*

### Comparing `aiohutils-0.9.1/pyproject.toml` & `aiohutils-0.9.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -9,19 +9,24 @@
 description = "A small library to for aiohttp projects."
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python :: 3.10",
 ]
 requires-python = ">=3.10"
 dependencies = [
+    "aiohttp[speedups]",
+]
+dynamic = ["version"]
+
+[project.optional-dependencies]
+test = [
     "pytest",
     "pytest-asyncio",
     "python-decouple",
 ]
-dynamic = ["version"]
 
 [project.readme]
 file = "README.rst"
 content-type = "text/x-rst"
 
 [project.urls]
 Homepage = "https://github.com/5j9/aiohutils"
```

