# Comparing `tmp/dsw-tdk-4.4.1.tar.gz` & `tmp/dsw-tdk-4.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsw-tdk-4.4.1.tar", last modified: Tue Mar 19 11:37:51 2024, max compression
+gzip compressed data, was "dsw-tdk-4.5.0.tar", last modified: Tue Apr  2 10:29:22 2024, max compression
```

## Comparing `dsw-tdk-4.4.1.tar` & `dsw-tdk-4.5.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 11:37:51.723366 dsw-tdk-4.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     8501 2024-03-19 11:37:39.000000 dsw-tdk-4.4.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-19 11:37:39.000000 dsw-tdk-4.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-19 11:37:39.000000 dsw-tdk-4.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-03-19 11:37:51.723366 dsw-tdk-4.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-03-19 11:37:39.000000 dsw-tdk-4.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 11:37:51.715366 dsw-tdk-4.4.1/dsw/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 11:37:51.719366 dsw-tdk-4.4.1/dsw/tdk/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-03-19 11:37:39.000000 dsw-tdk-4.4.1/dsw/tdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 11:37:39.000000 dsw-tdk-4.4.1/dsw/tdk/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14222 2024-03-19 11:37:39.000000 dsw-tdk-4.4.1/dsw/tdk/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-03-19 11:37:50.000000 dsw-tdk-4.4.1/dsw/tdk/build_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    21676 2024-03-19 11:37:39.000000 dsw-tdk-4.4.1/dsw/tdk/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-03-19 11:37:39.000000 dsw-tdk-4.4.1/dsw/tdk/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)    25930 2024-03-19 11:37:39.000000 dsw-tdk-4.4.1/dsw/tdk/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    17235 2024-03-19 11:37:39.000000 dsw-tdk-4.4.1/dsw/tdk/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 11:37:51.719366 dsw-tdk-4.4.1/dsw/tdk/templates/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-19 11:37:39.000000 dsw-tdk-4.4.1/dsw/tdk/templates/LICENSE.j2
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-03-19 11:37:39.000000 dsw-tdk-4.4.1/dsw/tdk/templates/README.md.j2
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-19 11:37:39.000000 dsw-tdk-4.4.1/dsw/tdk/templates/env.j2
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-03-19 11:37:39.000000 dsw-tdk-4.4.1/dsw/tdk/templates/starter.j2
--rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-03-19 11:37:39.000000 dsw-tdk-4.4.1/dsw/tdk/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7827 2024-03-19 11:37:39.000000 dsw-tdk-4.4.1/dsw/tdk/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 11:37:51.723366 dsw-tdk-4.4.1/dsw_tdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-03-19 11:37:51.000000 dsw-tdk-4.4.1/dsw_tdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-03-19 11:37:51.000000 dsw-tdk-4.4.1/dsw_tdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 11:37:51.000000 dsw-tdk-4.4.1/dsw_tdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-19 11:37:51.000000 dsw-tdk-4.4.1/dsw_tdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 11:37:51.000000 dsw-tdk-4.4.1/dsw_tdk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-03-19 11:37:51.000000 dsw-tdk-4.4.1/dsw_tdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-19 11:37:51.000000 dsw-tdk-4.4.1/dsw_tdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-03-19 11:37:39.000000 dsw-tdk-4.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 11:37:51.723366 dsw-tdk-4.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 11:37:39.000000 dsw-tdk-4.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 11:37:51.723366 dsw-tdk-4.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-03-19 11:37:39.000000 dsw-tdk-4.4.1/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-03-19 11:37:39.000000 dsw-tdk-4.4.1/tests/test_cmd_dot-env.py
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-03-19 11:37:39.000000 dsw-tdk-4.4.1/tests/test_cmd_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-03-19 11:37:39.000000 dsw-tdk-4.4.1/tests/test_cmd_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-03-19 11:37:39.000000 dsw-tdk-4.4.1/tests/test_cmd_new.py
--rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-03-19 11:37:39.000000 dsw-tdk-4.4.1/tests/test_cmd_package.py
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-03-19 11:37:39.000000 dsw-tdk-4.4.1/tests/test_cmd_put.py
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-03-19 11:37:39.000000 dsw-tdk-4.4.1/tests/test_cmd_unpackage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-03-19 11:37:39.000000 dsw-tdk-4.4.1/tests/test_cmd_verify.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:29:22.289680 dsw-tdk-4.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     8597 2024-04-02 10:29:05.000000 dsw-tdk-4.5.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-02 10:29:05.000000 dsw-tdk-4.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-02 10:29:05.000000 dsw-tdk-4.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-04-02 10:29:22.289680 dsw-tdk-4.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-04-02 10:29:05.000000 dsw-tdk-4.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:29:22.277680 dsw-tdk-4.5.0/dsw/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:29:22.281680 dsw-tdk-4.5.0/dsw/tdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-02 10:29:05.000000 dsw-tdk-4.5.0/dsw/tdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 10:29:05.000000 dsw-tdk-4.5.0/dsw/tdk/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14222 2024-04-02 10:29:05.000000 dsw-tdk-4.5.0/dsw/tdk/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-02 10:29:21.000000 dsw-tdk-4.5.0/dsw/tdk/build_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21676 2024-04-02 10:29:05.000000 dsw-tdk-4.5.0/dsw/tdk/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-02 10:29:05.000000 dsw-tdk-4.5.0/dsw/tdk/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25930 2024-04-02 10:29:05.000000 dsw-tdk-4.5.0/dsw/tdk/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17235 2024-04-02 10:29:05.000000 dsw-tdk-4.5.0/dsw/tdk/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:29:22.285680 dsw-tdk-4.5.0/dsw/tdk/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-02 10:29:05.000000 dsw-tdk-4.5.0/dsw/tdk/templates/LICENSE.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-02 10:29:05.000000 dsw-tdk-4.5.0/dsw/tdk/templates/README.md.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-02 10:29:05.000000 dsw-tdk-4.5.0/dsw/tdk/templates/env.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-02 10:29:05.000000 dsw-tdk-4.5.0/dsw/tdk/templates/starter.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-04-02 10:29:05.000000 dsw-tdk-4.5.0/dsw/tdk/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7827 2024-04-02 10:29:05.000000 dsw-tdk-4.5.0/dsw/tdk/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:29:22.285680 dsw-tdk-4.5.0/dsw_tdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-04-02 10:29:22.000000 dsw-tdk-4.5.0/dsw_tdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-02 10:29:22.000000 dsw-tdk-4.5.0/dsw_tdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 10:29:22.000000 dsw-tdk-4.5.0/dsw_tdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-02 10:29:22.000000 dsw-tdk-4.5.0/dsw_tdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 10:29:22.000000 dsw-tdk-4.5.0/dsw_tdk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-02 10:29:22.000000 dsw-tdk-4.5.0/dsw_tdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-02 10:29:22.000000 dsw-tdk-4.5.0/dsw_tdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-02 10:29:05.000000 dsw-tdk-4.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 10:29:22.289680 dsw-tdk-4.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 10:29:05.000000 dsw-tdk-4.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:29:22.285680 dsw-tdk-4.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-02 10:29:05.000000 dsw-tdk-4.5.0/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-04-02 10:29:05.000000 dsw-tdk-4.5.0/tests/test_cmd_dot-env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-02 10:29:05.000000 dsw-tdk-4.5.0/tests/test_cmd_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-02 10:29:05.000000 dsw-tdk-4.5.0/tests/test_cmd_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-04-02 10:29:05.000000 dsw-tdk-4.5.0/tests/test_cmd_new.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-02 10:29:05.000000 dsw-tdk-4.5.0/tests/test_cmd_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-02 10:29:05.000000 dsw-tdk-4.5.0/tests/test_cmd_put.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-04-02 10:29:05.000000 dsw-tdk-4.5.0/tests/test_cmd_unpackage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-04-02 10:29:05.000000 dsw-tdk-4.5.0/tests/test_cmd_verify.py
```

### Comparing `dsw-tdk-4.4.1/CHANGELOG.md` & `dsw-tdk-4.5.0/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
 
+## [4.5.0]
+
+Released for version consistency with other DSW tools.
+
 ## [4.4.1]
 
 Released for version consistency with other DSW tools.
 
 ## [4.4.0]
 
 Released for version consistency with other DSW tools.
@@ -410,7 +414,8 @@
 [4.1.1]: /../../tree/v4.1.1
 [4.2.0]: /../../tree/v4.2.0
 [4.2.1]: /../../tree/v4.2.1
 [4.3.0]: /../../tree/v4.3.0
 [4.3.1]: /../../tree/v4.3.1
 [4.4.0]: /../../tree/v4.4.0
 [4.4.1]: /../../tree/v4.4.1
+[4.5.0]: /../../tree/v4.5.0
```

### Comparing `dsw-tdk-4.4.1/LICENSE` & `dsw-tdk-4.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dsw-tdk-4.4.1/PKG-INFO` & `dsw-tdk-4.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsw-tdk
-Version: 4.4.1
+Version: 4.5.0
 Summary: Data Stewardship Wizard Template Development Toolkit
 Author-email: Marek Suchánek <marek.suchanek@ds-wizard.org>
 License: Apache License 2.0
 Project-URL: Homepage, https://ds-wizard.org
 Project-URL: Repository, https://github.com/ds-wizard/engine-tools
 Project-URL: Documentation, https://guide.ds-wizard.org
 Keywords: documents,dsw,jinja2,template,toolkit
```

### Comparing `dsw-tdk-4.4.1/README.md` & `dsw-tdk-4.5.0/README.md`

 * *Files identical despite different names*

### Comparing `dsw-tdk-4.4.1/dsw/tdk/api_client.py` & `dsw-tdk-4.5.0/dsw/tdk/api_client.py`

 * *Files identical despite different names*

### Comparing `dsw-tdk-4.4.1/dsw/tdk/cli.py` & `dsw-tdk-4.5.0/dsw/tdk/cli.py`

 * *Files identical despite different names*

### Comparing `dsw-tdk-4.4.1/dsw/tdk/consts.py` & `dsw-tdk-4.5.0/dsw/tdk/consts.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 import pathspec  # type: ignore
 import re
 
 APP = 'dsw-tdk'
-VERSION = '4.4.1'
+VERSION = '4.5.0'
 METAMODEL_VERSION = 13
 
 REGEX_SEMVER = re.compile(r'^[0-9]+\.[0-9]+\.[0-9]+$')
 REGEX_ORGANIZATION_ID = re.compile(r'^(?![.])(?!.*[.]$)[a-zA-Z0-9.]+$')
 REGEX_TEMPLATE_ID = re.compile(r'^(?![-])(?!.*[-]$)[a-zA-Z0-9-]+$')
 REGEX_KM_ID = REGEX_TEMPLATE_ID
 REGEX_MIME_TYPE = re.compile(r'^(?![-])(?!.*[-]$)[-\w.]+/[-\w.]+$')
```

### Comparing `dsw-tdk-4.4.1/dsw/tdk/core.py` & `dsw-tdk-4.5.0/dsw/tdk/core.py`

 * *Files identical despite different names*

### Comparing `dsw-tdk-4.4.1/dsw/tdk/model.py` & `dsw-tdk-4.5.0/dsw/tdk/model.py`

 * *Files identical despite different names*

### Comparing `dsw-tdk-4.4.1/dsw/tdk/utils.py` & `dsw-tdk-4.5.0/dsw/tdk/utils.py`

 * *Files identical despite different names*

### Comparing `dsw-tdk-4.4.1/dsw/tdk/validation.py` & `dsw-tdk-4.5.0/dsw/tdk/validation.py`

 * *Files identical despite different names*

### Comparing `dsw-tdk-4.4.1/dsw_tdk.egg-info/PKG-INFO` & `dsw-tdk-4.5.0/dsw_tdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsw-tdk
-Version: 4.4.1
+Version: 4.5.0
 Summary: Data Stewardship Wizard Template Development Toolkit
 Author-email: Marek Suchánek <marek.suchanek@ds-wizard.org>
 License: Apache License 2.0
 Project-URL: Homepage, https://ds-wizard.org
 Project-URL: Repository, https://github.com/ds-wizard/engine-tools
 Project-URL: Documentation, https://guide.ds-wizard.org
 Keywords: documents,dsw,jinja2,template,toolkit
```

### Comparing `dsw-tdk-4.4.1/dsw_tdk.egg-info/SOURCES.txt` & `dsw-tdk-4.5.0/dsw_tdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dsw-tdk-4.4.1/pyproject.toml` & `dsw-tdk-4.5.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'dsw-tdk'
-version = "4.4.1"
+version = "4.5.0"
 description = 'Data Stewardship Wizard Template Development Toolkit'
 readme = 'README.md'
 keywords = ['documents', 'dsw', 'jinja2', 'template', 'toolkit']
 license = { text = 'Apache License 2.0' }
 authors = [
     { name = 'Marek Suchánek', email = 'marek.suchanek@ds-wizard.org' }
 ]
```

### Comparing `dsw-tdk-4.4.1/tests/test_basic.py` & `dsw-tdk-4.5.0/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `dsw-tdk-4.4.1/tests/test_cmd_dot-env.py` & `dsw-tdk-4.5.0/tests/test_cmd_dot-env.py`

 * *Files identical despite different names*

### Comparing `dsw-tdk-4.4.1/tests/test_cmd_get.py` & `dsw-tdk-4.5.0/tests/test_cmd_get.py`

 * *Files identical despite different names*

### Comparing `dsw-tdk-4.4.1/tests/test_cmd_list.py` & `dsw-tdk-4.5.0/tests/test_cmd_list.py`

 * *Files identical despite different names*

### Comparing `dsw-tdk-4.4.1/tests/test_cmd_new.py` & `dsw-tdk-4.5.0/tests/test_cmd_new.py`

 * *Files identical despite different names*

### Comparing `dsw-tdk-4.4.1/tests/test_cmd_package.py` & `dsw-tdk-4.5.0/tests/test_cmd_package.py`

 * *Files identical despite different names*

### Comparing `dsw-tdk-4.4.1/tests/test_cmd_put.py` & `dsw-tdk-4.5.0/tests/test_cmd_put.py`

 * *Files identical despite different names*

### Comparing `dsw-tdk-4.4.1/tests/test_cmd_unpackage.py` & `dsw-tdk-4.5.0/tests/test_cmd_unpackage.py`

 * *Files identical despite different names*

### Comparing `dsw-tdk-4.4.1/tests/test_cmd_verify.py` & `dsw-tdk-4.5.0/tests/test_cmd_verify.py`

 * *Files identical despite different names*

