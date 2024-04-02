# Comparing `tmp/web-fragments-2.1.0.tar.gz` & `tmp/web-fragments-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web-fragments-2.1.0.tar", last modified: Thu Aug  3 11:01:03 2023, max compression
+gzip compressed data, was "web-fragments-2.2.0.tar", last modified: Tue Apr  2 19:13:58 2024, max compression
```

## Comparing `web-fragments-2.1.0.tar` & `web-fragments-2.2.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:01:03.412799 web-fragments-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (122)       31 2023-08-03 11:00:57.000000 web-fragments-2.1.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (122)      183 2023-08-03 11:00:57.000000 web-fragments-2.1.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-08-03 11:00:57.000000 web-fragments-2.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      188 2023-08-03 11:00:57.000000 web-fragments-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     3950 2023-08-03 11:01:03.412799 web-fragments-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3013 2023-08-03 11:00:57.000000 web-fragments-2.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      621 2023-08-03 11:01:03.412799 web-fragments-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1945 2023-08-03 11:00:57.000000 web-fragments-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:01:03.408799 web-fragments-2.1.0/web_fragments/
--rw-r--r--   0 runner    (1001) docker     (122)       45 2023-08-03 11:00:57.000000 web-fragments-2.1.0/web_fragments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      234 2023-08-03 11:00:57.000000 web-fragments-2.1.0/web_fragments/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:01:03.412799 web-fragments-2.1.0/web_fragments/examples/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-03 11:00:57.000000 web-fragments-2.1.0/web_fragments/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      287 2023-08-03 11:00:57.000000 web-fragments-2.1.0/web_fragments/examples/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)      611 2023-08-03 11:00:57.000000 web-fragments-2.1.0/web_fragments/examples/views.py
--rw-r--r--   0 runner    (1001) docker     (122)     9010 2023-08-03 11:00:57.000000 web-fragments-2.1.0/web_fragments/fragment.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:01:03.408799 web-fragments-2.1.0/web_fragments/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:01:03.412799 web-fragments-2.1.0/web_fragments/templates/web_fragments/
--rw-r--r--   0 runner    (1001) docker     (122)      120 2023-08-03 11:00:57.000000 web-fragments-2.1.0/web_fragments/templates/web_fragments/standalone_fragment.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:01:03.412799 web-fragments-2.1.0/web_fragments/test_utils/
--rw-r--r--   0 runner    (1001) docker     (122)      547 2023-08-03 11:00:57.000000 web-fragments-2.1.0/web_fragments/test_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:01:03.412799 web-fragments-2.1.0/web_fragments/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     7837 2023-08-03 11:00:57.000000 web-fragments-2.1.0/web_fragments/tests/test_fragment.py
--rw-r--r--   0 runner    (1001) docker     (122)     3253 2023-08-03 11:00:57.000000 web-fragments-2.1.0/web_fragments/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (122)     1982 2023-08-03 11:00:57.000000 web-fragments-2.1.0/web_fragments/views.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:01:03.408799 web-fragments-2.1.0/web_fragments.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3950 2023-08-03 11:01:03.000000 web-fragments-2.1.0/web_fragments.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      661 2023-08-03 11:01:03.000000 web-fragments-2.1.0/web_fragments.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-03 11:01:03.000000 web-fragments-2.1.0/web_fragments.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-03 11:01:03.000000 web-fragments-2.1.0/web_fragments.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       27 2023-08-03 11:01:03.000000 web-fragments-2.1.0/web_fragments.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       14 2023-08-03 11:01:03.000000 web-fragments-2.1.0/web_fragments.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:13:58.849022 web-fragments-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-02 19:13:53.000000 web-fragments-2.2.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-02 19:13:53.000000 web-fragments-2.2.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-02 19:13:53.000000 web-fragments-2.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-02 19:13:53.000000 web-fragments-2.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-04-02 19:13:58.849022 web-fragments-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-04-02 19:13:53.000000 web-fragments-2.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-02 19:13:58.849022 web-fragments-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-02 19:13:53.000000 web-fragments-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:13:58.849022 web-fragments-2.2.0/web_fragments/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-02 19:13:53.000000 web-fragments-2.2.0/web_fragments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-02 19:13:53.000000 web-fragments-2.2.0/web_fragments/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:13:58.849022 web-fragments-2.2.0/web_fragments/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:13:53.000000 web-fragments-2.2.0/web_fragments/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-02 19:13:53.000000 web-fragments-2.2.0/web_fragments/examples/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-02 19:13:53.000000 web-fragments-2.2.0/web_fragments/examples/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9010 2024-04-02 19:13:53.000000 web-fragments-2.2.0/web_fragments/fragment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:13:58.845022 web-fragments-2.2.0/web_fragments/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:13:58.849022 web-fragments-2.2.0/web_fragments/templates/web_fragments/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-02 19:13:53.000000 web-fragments-2.2.0/web_fragments/templates/web_fragments/standalone_fragment.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:13:58.849022 web-fragments-2.2.0/web_fragments/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-02 19:13:53.000000 web-fragments-2.2.0/web_fragments/test_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:13:58.849022 web-fragments-2.2.0/web_fragments/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7837 2024-04-02 19:13:53.000000 web-fragments-2.2.0/web_fragments/tests/test_fragment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-04-02 19:13:53.000000 web-fragments-2.2.0/web_fragments/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-04-02 19:13:53.000000 web-fragments-2.2.0/web_fragments/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:13:58.849022 web-fragments-2.2.0/web_fragments.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-04-02 19:13:58.000000 web-fragments-2.2.0/web_fragments.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-02 19:13:58.000000 web-fragments-2.2.0/web_fragments.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 19:13:58.000000 web-fragments-2.2.0/web_fragments.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 19:13:58.000000 web-fragments-2.2.0/web_fragments.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-02 19:13:58.000000 web-fragments-2.2.0/web_fragments.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-02 19:13:58.000000 web-fragments-2.2.0/web_fragments.egg-info/top_level.txt
```

### Comparing `web-fragments-2.1.0/LICENSE.txt` & `web-fragments-2.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `web-fragments-2.1.0/PKG-INFO` & `web-fragments-2.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: web-fragments
-Version: 2.1.0
+Version: 2.2.0
 Summary: Web fragments
 Home-page: https://github.com/openedx/web-fragments
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Django edx
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
-Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
-Provides-Extra: Django
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 License-File: LICENSE.txt
 License-File: AUTHORS
+Provides-Extra: django
+Requires-Dist: Django<4.3,>=4.2; extra == "django"
 
 web-fragments
 =============
 
 .. image:: https://img.shields.io/pypi/v/web-fragments.svg
     :target: https://pypi.python.org/pypi/web-fragments/
     :alt: PyPI
@@ -92,15 +93,15 @@
 Contributions are very welcome. Please read `the Open edX Contributing Guide`_ for details.
 
 .. _the Open edX Contributing Guide: https://github.com/openedx/.github/blob/master/CONTRIBUTING.md
 
 Reporting Security Issues
 -------------------------
 
-Please do not report security issues in public. Please email security@edx.org.
+Please do not report security issues in public. Please email security@openedx.org.
 
 Getting Help
 ------------
 
 Have a question about this repository, or about Open edX in general?  Please
 refer to the Open edX guide to `Getting Help`_.
```

### Comparing `web-fragments-2.1.0/README.rst` & `web-fragments-2.2.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 Contributions are very welcome. Please read `the Open edX Contributing Guide`_ for details.
 
 .. _the Open edX Contributing Guide: https://github.com/openedx/.github/blob/master/CONTRIBUTING.md
 
 Reporting Security Issues
 -------------------------
 
-Please do not report security issues in public. Please email security@edx.org.
+Please do not report security issues in public. Please email security@openedx.org.
 
 Getting Help
 ------------
 
 Have a question about this repository, or about Open edX in general?  Please
 refer to the Open edX guide to `Getting Help`_.
```

### Comparing `web-fragments-2.1.0/setup.cfg` & `web-fragments-2.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `web-fragments-2.1.0/setup.py` & `web-fragments-2.2.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -45,20 +45,20 @@
     include_package_data=True,
     license="AGPL 3.0",
     zip_safe=False,
     keywords='Django edx',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Framework :: Django',
-        'Framework :: Django :: 3.0',
-        'Framework :: Django :: 3.1',
-        'Framework :: Django :: 3.2',
+        'Framework :: Django :: 4.2',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
     ],
     extras_require={
-        'Django': ['Django>=3.0,<3.3'],
+        'Django': ['Django>=4.2,<4.3'],
     }
 )
```

### Comparing `web-fragments-2.1.0/web_fragments/examples/views.py` & `web-fragments-2.2.0/web_fragments/examples/views.py`

 * *Files identical despite different names*

### Comparing `web-fragments-2.1.0/web_fragments/fragment.py` & `web-fragments-2.2.0/web_fragments/fragment.py`

 * *Files identical despite different names*

### Comparing `web-fragments-2.1.0/web_fragments/test_utils/__init__.py` & `web-fragments-2.2.0/web_fragments/test_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `web-fragments-2.1.0/web_fragments/tests/test_fragment.py` & `web-fragments-2.2.0/web_fragments/tests/test_fragment.py`

 * *Files identical despite different names*

### Comparing `web-fragments-2.1.0/web_fragments/tests/test_views.py` & `web-fragments-2.2.0/web_fragments/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `web-fragments-2.1.0/web_fragments/views.py` & `web-fragments-2.2.0/web_fragments/views.py`

 * *Files identical despite different names*

### Comparing `web-fragments-2.1.0/web_fragments.egg-info/PKG-INFO` & `web-fragments-2.2.0/web_fragments.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: web-fragments
-Version: 2.1.0
+Version: 2.2.0
 Summary: Web fragments
 Home-page: https://github.com/openedx/web-fragments
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Django edx
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
-Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
-Provides-Extra: Django
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 License-File: LICENSE.txt
 License-File: AUTHORS
+Provides-Extra: django
+Requires-Dist: Django<4.3,>=4.2; extra == "django"
 
 web-fragments
 =============
 
 .. image:: https://img.shields.io/pypi/v/web-fragments.svg
     :target: https://pypi.python.org/pypi/web-fragments/
     :alt: PyPI
@@ -92,15 +93,15 @@
 Contributions are very welcome. Please read `the Open edX Contributing Guide`_ for details.
 
 .. _the Open edX Contributing Guide: https://github.com/openedx/.github/blob/master/CONTRIBUTING.md
 
 Reporting Security Issues
 -------------------------
 
-Please do not report security issues in public. Please email security@edx.org.
+Please do not report security issues in public. Please email security@openedx.org.
 
 Getting Help
 ------------
 
 Have a question about this repository, or about Open edX in general?  Please
 refer to the Open edX guide to `Getting Help`_.
```

### Comparing `web-fragments-2.1.0/web_fragments.egg-info/SOURCES.txt` & `web-fragments-2.2.0/web_fragments.egg-info/SOURCES.txt`

 * *Files identical despite different names*

