# Comparing `tmp/invenio-celery-1.3.0.tar.gz` & `tmp/invenio-celery-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-celery-1.3.0.tar", last modified: Tue Mar  5 10:28:22 2024, max compression
+gzip compressed data, was "dist/invenio-celery-1.3.1.tar", last modified: Tue Apr  2 14:01:56 2024, max compression
```

## Comparing `invenio-celery-1.3.0.tar` & `invenio-celery-1.3.1.tar`

### file list

```diff
@@ -1,57 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 10:28:22.000000 invenio-celery-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-05 10:28:17.000000 invenio-celery-1.3.0/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-03-05 10:28:17.000000 invenio-celery-1.3.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-05 10:28:17.000000 invenio-celery-1.3.0/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 10:28:22.000000 invenio-celery-1.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 10:28:22.000000 invenio-celery-1.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-03-05 10:28:17.000000 invenio-celery-1.3.0/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-03-05 10:28:17.000000 invenio-celery-1.3.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-03-05 10:28:17.000000 invenio-celery-1.3.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-03-05 10:28:17.000000 invenio-celery-1.3.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-03-05 10:28:17.000000 invenio-celery-1.3.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-03-05 10:28:17.000000 invenio-celery-1.3.0/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-03-05 10:28:17.000000 invenio-celery-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-03-05 10:28:17.000000 invenio-celery-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4998 2024-03-05 10:28:22.000000 invenio-celery-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-03-05 10:28:17.000000 invenio-celery-1.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 10:28:22.000000 invenio-celery-1.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     7441 2024-03-05 10:28:17.000000 invenio-celery-1.3.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-03-05 10:28:17.000000 invenio-celery-1.3.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-03-05 10:28:17.000000 invenio-celery-1.3.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-03-05 10:28:17.000000 invenio-celery-1.3.0/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10060 2024-03-05 10:28:17.000000 invenio-celery-1.3.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-03-05 10:28:17.000000 invenio-celery-1.3.0/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-03-05 10:28:17.000000 invenio-celery-1.3.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-03-05 10:28:17.000000 invenio-celery-1.3.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-03-05 10:28:17.000000 invenio-celery-1.3.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-05 10:28:17.000000 invenio-celery-1.3.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6997 2024-03-05 10:28:17.000000 invenio-celery-1.3.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-05 10:28:17.000000 invenio-celery-1.3.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-03-05 10:28:17.000000 invenio-celery-1.3.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 10:28:22.000000 invenio-celery-1.3.0/invenio_celery/
--rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-03-05 10:28:17.000000 invenio-celery-1.3.0/invenio_celery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-03-05 10:28:17.000000 invenio-celery-1.3.0/invenio_celery/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-03-05 10:28:17.000000 invenio-celery-1.3.0/invenio_celery/ext.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 10:28:22.000000 invenio-celery-1.3.0/invenio_celery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4998 2024-03-05 10:28:22.000000 invenio-celery-1.3.0/invenio_celery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-03-05 10:28:22.000000 invenio-celery-1.3.0/invenio_celery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-05 10:28:22.000000 invenio-celery-1.3.0/invenio_celery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-05 10:28:22.000000 invenio-celery-1.3.0/invenio_celery.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-05 10:28:22.000000 invenio-celery-1.3.0/invenio_celery.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-03-05 10:28:22.000000 invenio-celery-1.3.0/invenio_celery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-05 10:28:22.000000 invenio-celery-1.3.0/invenio_celery.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-05 10:28:17.000000 invenio-celery-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-03-05 10:28:17.000000 invenio-celery-1.3.0/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      479 2024-03-05 10:28:17.000000 invenio-celery-1.3.0/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-03-05 10:28:22.000000 invenio-celery-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-03-05 10:28:17.000000 invenio-celery-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 10:28:22.000000 invenio-celery-1.3.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 10:28:22.000000 invenio-celery-1.3.0/tests/apackage/
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-03-05 10:28:17.000000 invenio-celery-1.3.0/tests/apackage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-03-05 10:28:17.000000 invenio-celery-1.3.0/tests/apackage/third_tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 10:28:22.000000 invenio-celery-1.3.0/tests/bpackage/
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-03-05 10:28:17.000000 invenio-celery-1.3.0/tests/bpackage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-03-05 10:28:17.000000 invenio-celery-1.3.0/tests/bpackage/first_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-03-05 10:28:17.000000 invenio-celery-1.3.0/tests/bpackage/second_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-03-05 10:28:17.000000 invenio-celery-1.3.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-03-05 10:28:17.000000 invenio-celery-1.3.0/tests/test_invenio_celery.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:01:56.000000 invenio-celery-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-02 14:01:48.000000 invenio-celery-1.3.1/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-02 14:01:48.000000 invenio-celery-1.3.1/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-02 14:01:48.000000 invenio-celery-1.3.1/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:01:56.000000 invenio-celery-1.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:01:56.000000 invenio-celery-1.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-02 14:01:48.000000 invenio-celery-1.3.1/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-02 14:01:48.000000 invenio-celery-1.3.1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-02 14:01:48.000000 invenio-celery-1.3.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-04-02 14:01:48.000000 invenio-celery-1.3.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-04-02 14:01:48.000000 invenio-celery-1.3.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-02 14:01:48.000000 invenio-celery-1.3.1/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-02 14:01:48.000000 invenio-celery-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-02 14:01:48.000000 invenio-celery-1.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-04-02 14:01:56.000000 invenio-celery-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-02 14:01:48.000000 invenio-celery-1.3.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:01:56.000000 invenio-celery-1.3.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     7441 2024-04-02 14:01:48.000000 invenio-celery-1.3.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-02 14:01:48.000000 invenio-celery-1.3.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-02 14:01:48.000000 invenio-celery-1.3.1/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-02 14:01:48.000000 invenio-celery-1.3.1/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10060 2024-04-02 14:01:48.000000 invenio-celery-1.3.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-02 14:01:48.000000 invenio-celery-1.3.1/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-02 14:01:48.000000 invenio-celery-1.3.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-02 14:01:48.000000 invenio-celery-1.3.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-02 14:01:48.000000 invenio-celery-1.3.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-02 14:01:48.000000 invenio-celery-1.3.1/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6997 2024-04-02 14:01:48.000000 invenio-celery-1.3.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-02 14:01:48.000000 invenio-celery-1.3.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-02 14:01:48.000000 invenio-celery-1.3.1/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:01:56.000000 invenio-celery-1.3.1/invenio_celery/
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-04-02 14:01:48.000000 invenio-celery-1.3.1/invenio_celery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-02 14:01:48.000000 invenio-celery-1.3.1/invenio_celery/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-02 14:01:48.000000 invenio-celery-1.3.1/invenio_celery/ext.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:01:56.000000 invenio-celery-1.3.1/invenio_celery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-04-02 14:01:55.000000 invenio-celery-1.3.1/invenio_celery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-02 14:01:56.000000 invenio-celery-1.3.1/invenio_celery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 14:01:55.000000 invenio-celery-1.3.1/invenio_celery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-02 14:01:55.000000 invenio-celery-1.3.1/invenio_celery.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 14:01:55.000000 invenio-celery-1.3.1/invenio_celery.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-02 14:01:55.000000 invenio-celery-1.3.1/invenio_celery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-02 14:01:55.000000 invenio-celery-1.3.1/invenio_celery.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-02 14:01:48.000000 invenio-celery-1.3.1/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      479 2024-04-02 14:01:48.000000 invenio-celery-1.3.1/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-02 14:01:56.000000 invenio-celery-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-02 14:01:48.000000 invenio-celery-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:01:56.000000 invenio-celery-1.3.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:01:56.000000 invenio-celery-1.3.1/tests/apackage/
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-02 14:01:48.000000 invenio-celery-1.3.1/tests/apackage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-02 14:01:48.000000 invenio-celery-1.3.1/tests/apackage/third_tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:01:56.000000 invenio-celery-1.3.1/tests/bpackage/
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-02 14:01:48.000000 invenio-celery-1.3.1/tests/bpackage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-02 14:01:48.000000 invenio-celery-1.3.1/tests/bpackage/first_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-02 14:01:48.000000 invenio-celery-1.3.1/tests/bpackage/second_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-02 14:01:48.000000 invenio-celery-1.3.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-04-02 14:01:48.000000 invenio-celery-1.3.1/tests/test_invenio_celery.py
```

### Comparing `invenio-celery-1.3.0/.editorconfig` & `invenio-celery-1.3.1/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-celery-1.3.0/.github/workflows/pypi-publish.yml` & `invenio-celery-1.3.1/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `invenio-celery-1.3.0/CHANGES.rst` & `invenio-celery-1.3.1/CHANGES.rst`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,19 @@
 
     Invenio is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version 1.3.1 (released 2024-04-02)
+
+- setup: unpin importlib-metadata
+- tests: update python matrix
+
 Version 1.3.0 (released 2024-03-05)
 
 - installation: bump celery to support python 3.11
 
 Version 1.2.5 (released 2022-10-03)
 
 - Pin importlib-metadata due to celery/kombu icompatibilities with v5.
```

### Comparing `invenio-celery-1.3.0/CONTRIBUTING.rst` & `invenio-celery-1.3.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-celery-1.3.0/LICENSE` & `invenio-celery-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-celery-1.3.0/MANIFEST.in` & `invenio-celery-1.3.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-celery-1.3.0/PKG-INFO` & `invenio-celery-1.3.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-celery
-Version: 1.3.0
+Version: 1.3.1
 Summary: "Celery module for Invenio."
 Home-page: https://github.com/inveniosoftware/invenio-celery
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -45,14 +45,19 @@
         
             Invenio is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
+        Version 1.3.1 (released 2024-04-02)
+        
+        - setup: unpin importlib-metadata
+        - tests: update python matrix
+        
         Version 1.3.0 (released 2024-03-05)
         
         - installation: bump celery to support python 3.11
         
         Version 1.2.5 (released 2022-10-03)
         
         - Pin importlib-metadata due to celery/kombu icompatibilities with v5.
```

### Comparing `invenio-celery-1.3.0/README.rst` & `invenio-celery-1.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-celery-1.3.0/docs/Makefile` & `invenio-celery-1.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-celery-1.3.0/docs/conf.py` & `invenio-celery-1.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-celery-1.3.0/docs/index.rst` & `invenio-celery-1.3.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-celery-1.3.0/docs/make.bat` & `invenio-celery-1.3.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-celery-1.3.0/invenio_celery/__init__.py` & `invenio-celery-1.3.1/invenio_celery/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,10 +86,10 @@
 factory please see `Flask-CeleryExt <https://flask-celeryext.readthedocs.io/>`_
 """
 
 from __future__ import absolute_import, print_function
 
 from .ext import InvenioCelery
 
-__version__ = "1.3.0"
+__version__ = "1.3.1"
 
 __all__ = ("__version__", "InvenioCelery")
```

### Comparing `invenio-celery-1.3.0/invenio_celery/config.py` & `invenio-celery-1.3.1/invenio_celery/config.py`

 * *Files identical despite different names*

### Comparing `invenio-celery-1.3.0/invenio_celery/ext.py` & `invenio-celery-1.3.1/invenio_celery/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-celery-1.3.0/invenio_celery.egg-info/PKG-INFO` & `invenio-celery-1.3.1/invenio_celery.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-celery
-Version: 1.3.0
+Version: 1.3.1
 Summary: "Celery module for Invenio."
 Home-page: https://github.com/inveniosoftware/invenio-celery
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -45,14 +45,19 @@
         
             Invenio is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
+        Version 1.3.1 (released 2024-04-02)
+        
+        - setup: unpin importlib-metadata
+        - tests: update python matrix
+        
         Version 1.3.0 (released 2024-03-05)
         
         - installation: bump celery to support python 3.11
         
         Version 1.2.5 (released 2022-10-03)
         
         - Pin importlib-metadata due to celery/kombu icompatibilities with v5.
```

### Comparing `invenio-celery-1.3.0/invenio_celery.egg-info/SOURCES.txt` & `invenio-celery-1.3.1/invenio_celery.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 CHANGES.rst
 CONTRIBUTING.rst
 INSTALL.rst
 LICENSE
 MANIFEST.in
 README.rst
 pyproject.toml
-requirements-devel.txt
 run-tests.sh
 setup.cfg
 setup.py
 .github/workflows/pypi-publish.yml
 .github/workflows/tests.yml
 docs/Makefile
 docs/api.rst
```

### Comparing `invenio-celery-1.3.0/setup.cfg` & `invenio-celery-1.3.1/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 include_package_data = True
 packages = find:
 python_requires = >=3.7
 zip_safe = False
 install_requires = 
 	celery>=5.1.0,<5.4
 	Flask-CeleryExt>=0.3.4
-	importlib-metadata>=4.0.0,<5.0.0
 	invenio-base>=1.2.5
 	msgpack>=0.6.2
 	redis>=2.10.0
 
 [options.extras_require]
 tests = 
 	pytest-black-ng>=0.4.0
```

### Comparing `invenio-celery-1.3.0/tests/conftest.py` & `invenio-celery-1.3.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-celery-1.3.0/tests/test_invenio_celery.py` & `invenio-celery-1.3.1/tests/test_invenio_celery.py`

 * *Files identical despite different names*

