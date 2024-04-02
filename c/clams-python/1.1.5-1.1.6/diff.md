# Comparing `tmp/clams-python-1.1.5.tar.gz` & `tmp/clams-python-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clams-python-1.1.5.tar", last modified: Mon Apr  1 11:46:36 2024, max compression
+gzip compressed data, was "clams-python-1.1.6.tar", last modified: Tue Apr  2 20:03:39 2024, max compression
```

## Comparing `clams-python-1.1.5.tar` & `clams-python-1.1.6.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:46:36.630227 clams-python-1.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)    11374 2024-04-01 11:46:13.000000 clams-python-1.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-01 11:46:13.000000 clams-python-1.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-01 11:46:36.630227 clams-python-1.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-01 11:46:13.000000 clams-python-1.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-01 11:46:13.000000 clams-python-1.1.5/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:46:36.626227 clams-python-1.1.5/clams/
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-04-01 11:46:13.000000 clams-python-1.1.5/clams/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:46:36.626227 clams-python-1.1.5/clams/app/
--rw-r--r--   0 runner    (1001) docker     (127)    19308 2024-04-01 11:46:13.000000 clams-python-1.1.5/clams/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:46:36.626227 clams-python-1.1.5/clams/appmetadata/
--rw-r--r--   0 runner    (1001) docker     (127)    21677 2024-04-01 11:46:13.000000 clams-python-1.1.5/clams/appmetadata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:46:36.626227 clams-python-1.1.5/clams/develop/
--rw-r--r--   0 runner    (1001) docker     (127)     5578 2024-04-01 11:46:13.000000 clams-python-1.1.5/clams/develop/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:46:36.622227 clams-python-1.1.5/clams/develop/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:46:36.626227 clams-python-1.1.5/clams/develop/templates/app/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-01 11:46:13.000000 clams-python-1.1.5/clams/develop/templates/app/.dockerignore.template
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-04-01 11:46:13.000000 clams-python-1.1.5/clams/develop/templates/app/.gitignore.template
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-01 11:46:13.000000 clams-python-1.1.5/clams/develop/templates/app/Containerfile.template
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-01 11:46:13.000000 clams-python-1.1.5/clams/develop/templates/app/LICENSE.template
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-01 11:46:13.000000 clams-python-1.1.5/clams/develop/templates/app/README.md.template
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-04-01 11:46:13.000000 clams-python-1.1.5/clams/develop/templates/app/app.py.template
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-04-01 11:46:13.000000 clams-python-1.1.5/clams/develop/templates/app/metadata.py.template
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-01 11:46:13.000000 clams-python-1.1.5/clams/develop/templates/app/requirements.txt.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:46:36.626227 clams-python-1.1.5/clams/develop/templates/gha/
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-01 11:46:13.000000 clams-python-1.1.5/clams/develop/templates/gha/for-clams-team.md.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:46:36.626227 clams-python-1.1.5/clams/develop/templates/gha/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-01 11:46:13.000000 clams-python-1.1.5/clams/develop/templates/gha/workflows/issue-apps-project.yml.template
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-01 11:46:13.000000 clams-python-1.1.5/clams/develop/templates/gha/workflows/issue-assign.yml.template
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-01 11:46:13.000000 clams-python-1.1.5/clams/develop/templates/gha/workflows/issue-close.yml.template
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-01 11:46:13.000000 clams-python-1.1.5/clams/develop/templates/gha/workflows/publish.yml.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:46:36.626227 clams-python-1.1.5/clams/mmif_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-01 11:46:13.000000 clams-python-1.1.5/clams/mmif_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4960 2024-04-01 11:46:13.000000 clams-python-1.1.5/clams/mmif_utils/rewind.py
--rw-r--r--   0 runner    (1001) docker     (127)    11761 2024-04-01 11:46:13.000000 clams-python-1.1.5/clams/mmif_utils/source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:46:36.626227 clams-python-1.1.5/clams/restify/
--rw-r--r--   0 runner    (1001) docker     (127)     5989 2024-04-01 11:46:13.000000 clams-python-1.1.5/clams/restify/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:46:36.626227 clams-python-1.1.5/clams/serve/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-01 11:46:13.000000 clams-python-1.1.5/clams/serve/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:46:36.630227 clams-python-1.1.5/clams/ver/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-01 11:46:36.000000 clams-python-1.1.5/clams/ver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:46:36.630227 clams-python-1.1.5/clams_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-01 11:46:36.000000 clams-python-1.1.5/clams_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-01 11:46:36.000000 clams-python-1.1.5/clams_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 11:46:36.000000 clams-python-1.1.5/clams_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-01 11:46:36.000000 clams-python-1.1.5/clams_python.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-01 11:46:36.000000 clams-python-1.1.5/clams_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-01 11:46:36.000000 clams-python-1.1.5/clams_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-01 11:46:13.000000 clams-python-1.1.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 11:46:36.630227 clams-python-1.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-01 11:46:13.000000 clams-python-1.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:46:36.630227 clams-python-1.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    22424 2024-04-01 11:46:13.000000 clams-python-1.1.5/tests/test_clamsapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     7527 2024-04-01 11:46:13.000000 clams-python-1.1.5/tests/test_clamscli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:03:39.480415 clams-python-1.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    11374 2024-04-02 20:03:06.000000 clams-python-1.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-02 20:03:06.000000 clams-python-1.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-02 20:03:39.476415 clams-python-1.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-02 20:03:06.000000 clams-python-1.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-02 20:03:06.000000 clams-python-1.1.6/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:03:39.472416 clams-python-1.1.6/clams/
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-04-02 20:03:06.000000 clams-python-1.1.6/clams/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:03:39.472416 clams-python-1.1.6/clams/app/
+-rw-r--r--   0 runner    (1001) docker     (127)    19308 2024-04-02 20:03:06.000000 clams-python-1.1.6/clams/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:03:39.472416 clams-python-1.1.6/clams/appmetadata/
+-rw-r--r--   0 runner    (1001) docker     (127)    21677 2024-04-02 20:03:06.000000 clams-python-1.1.6/clams/appmetadata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:03:39.472416 clams-python-1.1.6/clams/develop/
+-rw-r--r--   0 runner    (1001) docker     (127)     5578 2024-04-02 20:03:06.000000 clams-python-1.1.6/clams/develop/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:03:39.468416 clams-python-1.1.6/clams/develop/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:03:39.472416 clams-python-1.1.6/clams/develop/templates/app/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-02 20:03:06.000000 clams-python-1.1.6/clams/develop/templates/app/.dockerignore.template
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-04-02 20:03:06.000000 clams-python-1.1.6/clams/develop/templates/app/.gitignore.template
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-02 20:03:06.000000 clams-python-1.1.6/clams/develop/templates/app/Containerfile.template
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-02 20:03:06.000000 clams-python-1.1.6/clams/develop/templates/app/LICENSE.template
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-02 20:03:06.000000 clams-python-1.1.6/clams/develop/templates/app/README.md.template
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-04-02 20:03:06.000000 clams-python-1.1.6/clams/develop/templates/app/app.py.template
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-04-02 20:03:06.000000 clams-python-1.1.6/clams/develop/templates/app/metadata.py.template
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-02 20:03:06.000000 clams-python-1.1.6/clams/develop/templates/app/requirements.txt.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:03:39.472416 clams-python-1.1.6/clams/develop/templates/gha/
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-02 20:03:06.000000 clams-python-1.1.6/clams/develop/templates/gha/for-clams-team.md.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:03:39.476415 clams-python-1.1.6/clams/develop/templates/gha/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-02 20:03:06.000000 clams-python-1.1.6/clams/develop/templates/gha/workflows/issue-apps-project.yml.template
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-02 20:03:06.000000 clams-python-1.1.6/clams/develop/templates/gha/workflows/issue-assign.yml.template
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-02 20:03:06.000000 clams-python-1.1.6/clams/develop/templates/gha/workflows/issue-close.yml.template
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-02 20:03:06.000000 clams-python-1.1.6/clams/develop/templates/gha/workflows/publish.yml.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:03:39.476415 clams-python-1.1.6/clams/mmif_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-02 20:03:06.000000 clams-python-1.1.6/clams/mmif_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4960 2024-04-02 20:03:06.000000 clams-python-1.1.6/clams/mmif_utils/rewind.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11761 2024-04-02 20:03:06.000000 clams-python-1.1.6/clams/mmif_utils/source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:03:39.476415 clams-python-1.1.6/clams/restify/
+-rw-r--r--   0 runner    (1001) docker     (127)     5989 2024-04-02 20:03:06.000000 clams-python-1.1.6/clams/restify/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:03:39.476415 clams-python-1.1.6/clams/serve/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-02 20:03:06.000000 clams-python-1.1.6/clams/serve/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:03:39.476415 clams-python-1.1.6/clams/ver/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-02 20:03:39.000000 clams-python-1.1.6/clams/ver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:03:39.476415 clams-python-1.1.6/clams_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-02 20:03:39.000000 clams-python-1.1.6/clams_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-02 20:03:39.000000 clams-python-1.1.6/clams_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 20:03:39.000000 clams-python-1.1.6/clams_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-02 20:03:39.000000 clams-python-1.1.6/clams_python.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-02 20:03:39.000000 clams-python-1.1.6/clams_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-02 20:03:39.000000 clams-python-1.1.6/clams_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-02 20:03:06.000000 clams-python-1.1.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 20:03:39.480415 clams-python-1.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-02 20:03:06.000000 clams-python-1.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:03:39.476415 clams-python-1.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    22424 2024-04-02 20:03:06.000000 clams-python-1.1.6/tests/test_clamsapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7527 2024-04-02 20:03:06.000000 clams-python-1.1.6/tests/test_clamscli.py
```

### Comparing `clams-python-1.1.5/LICENSE` & `clams-python-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `clams-python-1.1.5/PKG-INFO` & `clams-python-1.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: clams-python
-Version: 1.1.5
+Version: 1.1.6
 Summary: A collection of APIs to develop CLAMS app for python
 Home-page: https://clams.ai
 Author: Brandeis Lab for Linguistics and Computation
 Author-email: admin@clams.ai
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Flask
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers 
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mmif-python==1.0.11
+Requires-Dist: mmif-python==1.0.13
 Requires-Dist: Flask>=2
 Requires-Dist: Flask-RESTful>=0.3.9
 Requires-Dist: gunicorn>=20
 Requires-Dist: lapps>=0.0.2
 Requires-Dist: pydantic<2,>=1.8
 Requires-Dist: jsonschema>=3
```

### Comparing `clams-python-1.1.5/README.md` & `clams-python-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `clams-python-1.1.5/clams/__init__.py` & `clams-python-1.1.6/clams/__init__.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.1.5/clams/app/__init__.py` & `clams-python-1.1.6/clams/app/__init__.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.1.5/clams/appmetadata/__init__.py` & `clams-python-1.1.6/clams/appmetadata/__init__.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.1.5/clams/develop/__init__.py` & `clams-python-1.1.6/clams/develop/__init__.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.1.5/clams/develop/templates/app/.gitignore.template` & `clams-python-1.1.6/clams/develop/templates/app/.gitignore.template`

 * *Files identical despite different names*

### Comparing `clams-python-1.1.5/clams/develop/templates/app/Containerfile.template` & `clams-python-1.1.6/clams/develop/templates/app/Containerfile.template`

 * *Files identical despite different names*

### Comparing `clams-python-1.1.5/clams/develop/templates/app/README.md.template` & `clams-python-1.1.6/clams/develop/templates/app/README.md.template`

 * *Files identical despite different names*

### Comparing `clams-python-1.1.5/clams/develop/templates/app/app.py.template` & `clams-python-1.1.6/clams/develop/templates/app/app.py.template`

 * *Files identical despite different names*

### Comparing `clams-python-1.1.5/clams/develop/templates/app/metadata.py.template` & `clams-python-1.1.6/clams/develop/templates/app/metadata.py.template`

 * *Files identical despite different names*

### Comparing `clams-python-1.1.5/clams/develop/templates/gha/for-clams-team.md.template` & `clams-python-1.1.6/clams/develop/templates/gha/for-clams-team.md.template`

 * *Files identical despite different names*

### Comparing `clams-python-1.1.5/clams/develop/templates/gha/workflows/publish.yml.template` & `clams-python-1.1.6/clams/develop/templates/gha/workflows/publish.yml.template`

 * *Files identical despite different names*

### Comparing `clams-python-1.1.5/clams/mmif_utils/rewind.py` & `clams-python-1.1.6/clams/mmif_utils/rewind.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.1.5/clams/mmif_utils/source.py` & `clams-python-1.1.6/clams/mmif_utils/source.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.1.5/clams/restify/__init__.py` & `clams-python-1.1.6/clams/restify/__init__.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.1.5/clams_python.egg-info/PKG-INFO` & `clams-python-1.1.6/clams_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: clams-python
-Version: 1.1.5
+Version: 1.1.6
 Summary: A collection of APIs to develop CLAMS app for python
 Home-page: https://clams.ai
 Author: Brandeis Lab for Linguistics and Computation
 Author-email: admin@clams.ai
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Flask
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers 
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mmif-python==1.0.11
+Requires-Dist: mmif-python==1.0.13
 Requires-Dist: Flask>=2
 Requires-Dist: Flask-RESTful>=0.3.9
 Requires-Dist: gunicorn>=20
 Requires-Dist: lapps>=0.0.2
 Requires-Dist: pydantic<2,>=1.8
 Requires-Dist: jsonschema>=3
```

### Comparing `clams-python-1.1.5/clams_python.egg-info/SOURCES.txt` & `clams-python-1.1.6/clams_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clams-python-1.1.5/setup.py` & `clams-python-1.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.1.5/tests/test_clamsapp.py` & `clams-python-1.1.6/tests/test_clamsapp.py`

 * *Files identical despite different names*

### Comparing `clams-python-1.1.5/tests/test_clamscli.py` & `clams-python-1.1.6/tests/test_clamscli.py`

 * *Files identical despite different names*

