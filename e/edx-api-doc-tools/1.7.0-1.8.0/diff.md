# Comparing `tmp/edx-api-doc-tools-1.7.0.tar.gz` & `tmp/edx-api-doc-tools-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-api-doc-tools-1.7.0.tar", last modified: Fri Jul 21 12:22:44 2023, max compression
+gzip compressed data, was "edx-api-doc-tools-1.8.0.tar", last modified: Tue Apr  2 19:40:50 2024, max compression
```

## Comparing `edx-api-doc-tools-1.7.0.tar` & `edx-api-doc-tools-1.8.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 12:22:44.297615 edx-api-doc-tools-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (122)     2003 2023-07-21 12:22:34.000000 edx-api-doc-tools-1.7.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    10177 2023-07-21 12:22:34.000000 edx-api-doc-tools-1.7.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      127 2023-07-21 12:22:34.000000 edx-api-doc-tools-1.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     6393 2023-07-21 12:22:44.297615 edx-api-doc-tools-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3620 2023-07-21 12:22:34.000000 edx-api-doc-tools-1.7.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 12:22:44.297615 edx-api-doc-tools-1.7.0/edx_api_doc_tools/
--rw-r--r--   0 runner    (1001) docker     (122)     1253 2023-07-21 12:22:34.000000 edx-api-doc-tools-1.7.0/edx_api_doc_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1197 2023-07-21 12:22:34.000000 edx-api-doc-tools-1.7.0/edx_api_doc_tools/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)     6034 2023-07-21 12:22:34.000000 edx-api-doc-tools-1.7.0/edx_api_doc_tools/conf_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     2417 2023-07-21 12:22:34.000000 edx-api-doc-tools-1.7.0/edx_api_doc_tools/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-07-21 12:22:34.000000 edx-api-doc-tools-1.7.0/edx_api_doc_tools/internal_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      212 2023-07-21 12:22:34.000000 edx-api-doc-tools-1.7.0/edx_api_doc_tools/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)     5993 2023-07-21 12:22:34.000000 edx-api-doc-tools-1.7.0/edx_api_doc_tools/view_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 12:22:44.297615 edx-api-doc-tools-1.7.0/edx_api_doc_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     6393 2023-07-21 12:22:44.000000 edx-api-doc-tools-1.7.0/edx_api_doc_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      615 2023-07-21 12:22:44.000000 edx-api-doc-tools-1.7.0/edx_api_doc_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-21 12:22:44.000000 edx-api-doc-tools-1.7.0/edx_api_doc_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-21 12:22:44.000000 edx-api-doc-tools-1.7.0/edx_api_doc_tools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       43 2023-07-21 12:22:44.000000 edx-api-doc-tools-1.7.0/edx_api_doc_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-07-21 12:22:44.000000 edx-api-doc-tools-1.7.0/edx_api_doc_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 12:22:44.297615 edx-api-doc-tools-1.7.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      110 2023-07-21 12:22:34.000000 edx-api-doc-tools-1.7.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      573 2023-07-21 12:22:34.000000 edx-api-doc-tools-1.7.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      413 2023-07-21 12:22:44.297615 edx-api-doc-tools-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     5393 2023-07-21 12:22:34.000000 edx-api-doc-tools-1.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 12:22:44.297615 edx-api-doc-tools-1.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     6905 2023-07-21 12:22:34.000000 edx-api-doc-tools-1.7.0/tests/test_doc_tools.py
--rw-r--r--   0 runner    (1001) docker     (122)     2663 2023-07-21 12:22:34.000000 edx-api-doc-tools-1.7.0/tests/test_example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:40:50.792569 edx-api-doc-tools-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-02 19:40:47.000000 edx-api-doc-tools-1.8.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10177 2024-04-02 19:40:47.000000 edx-api-doc-tools-1.8.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-02 19:40:47.000000 edx-api-doc-tools-1.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6669 2024-04-02 19:40:50.792569 edx-api-doc-tools-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-02 19:40:47.000000 edx-api-doc-tools-1.8.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:40:50.792569 edx-api-doc-tools-1.8.0/edx_api_doc_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-02 19:40:47.000000 edx-api-doc-tools-1.8.0/edx_api_doc_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-02 19:40:47.000000 edx-api-doc-tools-1.8.0/edx_api_doc_tools/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6034 2024-04-02 19:40:47.000000 edx-api-doc-tools-1.8.0/edx_api_doc_tools/conf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-02 19:40:47.000000 edx-api-doc-tools-1.8.0/edx_api_doc_tools/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-02 19:40:47.000000 edx-api-doc-tools-1.8.0/edx_api_doc_tools/internal_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-02 19:40:47.000000 edx-api-doc-tools-1.8.0/edx_api_doc_tools/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-04-02 19:40:47.000000 edx-api-doc-tools-1.8.0/edx_api_doc_tools/view_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:40:50.792569 edx-api-doc-tools-1.8.0/edx_api_doc_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6669 2024-04-02 19:40:50.000000 edx-api-doc-tools-1.8.0/edx_api_doc_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-02 19:40:50.000000 edx-api-doc-tools-1.8.0/edx_api_doc_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 19:40:50.000000 edx-api-doc-tools-1.8.0/edx_api_doc_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 19:40:50.000000 edx-api-doc-tools-1.8.0/edx_api_doc_tools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-02 19:40:50.000000 edx-api-doc-tools-1.8.0/edx_api_doc_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-02 19:40:50.000000 edx-api-doc-tools-1.8.0/edx_api_doc_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:40:50.792569 edx-api-doc-tools-1.8.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-02 19:40:47.000000 edx-api-doc-tools-1.8.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-02 19:40:47.000000 edx-api-doc-tools-1.8.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-02 19:40:50.792569 edx-api-doc-tools-1.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5455 2024-04-02 19:40:47.000000 edx-api-doc-tools-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:40:50.792569 edx-api-doc-tools-1.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6905 2024-04-02 19:40:47.000000 edx-api-doc-tools-1.8.0/tests/test_doc_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-04-02 19:40:47.000000 edx-api-doc-tools-1.8.0/tests/test_example.py
```

### Comparing `edx-api-doc-tools-1.7.0/CHANGELOG.rst` & `edx-api-doc-tools-1.8.0/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,21 @@
    This project adheres to Semantic Versioning (http://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+1.8.0 --- 2024-02-29
+--------------------
+* Add support for python 3.11 and 3.12 support.
+* Removed django32 support.
+
+
+
 1.7.0 --- 2023-07-23
 --------------------
 
 * Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
   deprecated
 * Add support for Django 4.2
```

### Comparing `edx-api-doc-tools-1.7.0/LICENSE.txt` & `edx-api-doc-tools-1.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx-api-doc-tools-1.7.0/PKG-INFO` & `edx-api-doc-tools-1.8.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 Metadata-Version: 2.1
 Name: edx-api-doc-tools
-Version: 1.7.0
+Version: 1.8.0
 Summary: Tools for writing and generating API documentation for edX REST APIs
 Home-page: https://github.com/openedx/api-doc-tools
 Author: Open edX Project
 Author-email: oscm@openedx.org
 License: Apache Software License 2.0
 Keywords: Django edx
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
+Requires-Dist: Django
+Requires-Dist: djangorestframework>=3.2.0
+Requires-Dist: drf-yasg
 
 edX API Documentation Tools
 ===========================
 
 |pypi| |CI| |codecov| |readthedocs| |pyversions| |license|
 
 A toolkit for documenting REST APIs that are created with `DRF`_.
@@ -85,15 +89,15 @@
 
 .. _PULL_REQUEST_TEMPLATE.md: .github/PULL_REQUEST_TEMPLATE.md
 .. _ISSUE_TEMPLATE.md: .github/ISSUE_TEMPLATE.md
 
 Reporting Security Issues
 -------------------------
 
-Please do not report security issues in public. Please email security@edx.org.
+Please do not report security issues in public. Please email security@openedx.org.
 
 Getting Help
 ------------
 
 Have a question about this repository, or about the Open edX project in general?  Please refer to this `list of resources <https://open.edx.org/getting-help>`_ if you need any assistance.
 
 
@@ -130,14 +134,21 @@
    This project adheres to Semantic Versioning (http://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+1.8.0 --- 2024-02-29
+--------------------
+* Add support for python 3.11 and 3.12 support.
+* Removed django32 support.
+
+
+
 1.7.0 --- 2023-07-23
 --------------------
 
 * Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
   deprecated
 * Add support for Django 4.2
```

### Comparing `edx-api-doc-tools-1.7.0/README.rst` & `edx-api-doc-tools-1.8.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
 .. _PULL_REQUEST_TEMPLATE.md: .github/PULL_REQUEST_TEMPLATE.md
 .. _ISSUE_TEMPLATE.md: .github/ISSUE_TEMPLATE.md
 
 Reporting Security Issues
 -------------------------
 
-Please do not report security issues in public. Please email security@edx.org.
+Please do not report security issues in public. Please email security@openedx.org.
 
 Getting Help
 ------------
 
 Have a question about this repository, or about the Open edX project in general?  Please refer to this `list of resources <https://open.edx.org/getting-help>`_ if you need any assistance.
```

### Comparing `edx-api-doc-tools-1.7.0/edx_api_doc_tools/__init__.py` & `edx-api-doc-tools-1.8.0/edx_api_doc_tools/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,8 +42,8 @@
     exclude_schema_for_all,
     is_schema_request,
     schema,
     schema_for,
 )
 
 
-__version__ = '1.7.0'
+__version__ = '1.8.0'
```

### Comparing `edx-api-doc-tools-1.7.0/edx_api_doc_tools/apps.py` & `edx-api-doc-tools-1.8.0/edx_api_doc_tools/apps.py`

 * *Files identical despite different names*

### Comparing `edx-api-doc-tools-1.7.0/edx_api_doc_tools/conf_utils.py` & `edx-api-doc-tools-1.8.0/edx_api_doc_tools/conf_utils.py`

 * *Files identical despite different names*

### Comparing `edx-api-doc-tools-1.7.0/edx_api_doc_tools/data.py` & `edx-api-doc-tools-1.8.0/edx_api_doc_tools/data.py`

 * *Files identical despite different names*

### Comparing `edx-api-doc-tools-1.7.0/edx_api_doc_tools/internal_utils.py` & `edx-api-doc-tools-1.8.0/edx_api_doc_tools/internal_utils.py`

 * *Files identical despite different names*

### Comparing `edx-api-doc-tools-1.7.0/edx_api_doc_tools/view_utils.py` & `edx-api-doc-tools-1.8.0/edx_api_doc_tools/view_utils.py`

 * *Files identical despite different names*

### Comparing `edx-api-doc-tools-1.7.0/edx_api_doc_tools.egg-info/PKG-INFO` & `edx-api-doc-tools-1.8.0/edx_api_doc_tools.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 Metadata-Version: 2.1
 Name: edx-api-doc-tools
-Version: 1.7.0
+Version: 1.8.0
 Summary: Tools for writing and generating API documentation for edX REST APIs
 Home-page: https://github.com/openedx/api-doc-tools
 Author: Open edX Project
 Author-email: oscm@openedx.org
 License: Apache Software License 2.0
 Keywords: Django edx
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
+Requires-Dist: Django
+Requires-Dist: djangorestframework>=3.2.0
+Requires-Dist: drf-yasg
 
 edX API Documentation Tools
 ===========================
 
 |pypi| |CI| |codecov| |readthedocs| |pyversions| |license|
 
 A toolkit for documenting REST APIs that are created with `DRF`_.
@@ -85,15 +89,15 @@
 
 .. _PULL_REQUEST_TEMPLATE.md: .github/PULL_REQUEST_TEMPLATE.md
 .. _ISSUE_TEMPLATE.md: .github/ISSUE_TEMPLATE.md
 
 Reporting Security Issues
 -------------------------
 
-Please do not report security issues in public. Please email security@edx.org.
+Please do not report security issues in public. Please email security@openedx.org.
 
 Getting Help
 ------------
 
 Have a question about this repository, or about the Open edX project in general?  Please refer to this `list of resources <https://open.edx.org/getting-help>`_ if you need any assistance.
 
 
@@ -130,14 +134,21 @@
    This project adheres to Semantic Versioning (http://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+1.8.0 --- 2024-02-29
+--------------------
+* Add support for python 3.11 and 3.12 support.
+* Removed django32 support.
+
+
+
 1.7.0 --- 2023-07-23
 --------------------
 
 * Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
   deprecated
 * Add support for Django 4.2
```

### Comparing `edx-api-doc-tools-1.7.0/edx_api_doc_tools.egg-info/SOURCES.txt` & `edx-api-doc-tools-1.8.0/edx_api_doc_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx-api-doc-tools-1.7.0/setup.py` & `edx-api-doc-tools-1.8.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,16 +120,17 @@
     install_requires=load_requirements('requirements/base.in'),
     license="Apache Software License 2.0",
     zip_safe=False,
     keywords='Django edx',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Framework :: Django',
-        'Framework :: Django :: 3.2',
         'Framework :: Django :: 4.2',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
     ],
 )
```

### Comparing `edx-api-doc-tools-1.7.0/tests/test_doc_tools.py` & `edx-api-doc-tools-1.8.0/tests/test_doc_tools.py`

 * *Files identical despite different names*

### Comparing `edx-api-doc-tools-1.7.0/tests/test_example.py` & `edx-api-doc-tools-1.8.0/tests/test_example.py`

 * *Files identical despite different names*

