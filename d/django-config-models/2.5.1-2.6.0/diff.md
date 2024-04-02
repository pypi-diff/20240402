# Comparing `tmp/django-config-models-2.5.1.tar.gz` & `tmp/django-config-models-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-config-models-2.5.1.tar", last modified: Fri Sep 22 10:16:38 2023, max compression
+gzip compressed data, was "django-config-models-2.6.0.tar", last modified: Tue Apr  2 21:10:44 2024, max compression
```

## Comparing `django-config-models-2.5.1.tar` & `django-config-models-2.6.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 10:16:38.423637 django-config-models-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)      428 2023-09-22 10:16:31.000000 django-config-models-2.5.1/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2023-09-22 10:16:31.000000 django-config-models-2.5.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)    35119 2023-09-22 10:16:31.000000 django-config-models-2.5.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      249 2023-09-22 10:16:31.000000 django-config-models-2.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11266 2023-09-22 10:16:38.423637 django-config-models-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5860 2023-09-22 10:16:31.000000 django-config-models-2.5.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 10:16:38.419637 django-config-models-2.5.1/config_models/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2023-09-22 10:16:31.000000 django-config-models-2.5.1/config_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7978 2023-09-22 10:16:31.000000 django-config-models-2.5.1/config_models/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2023-09-22 10:16:31.000000 django-config-models-2.5.1/config_models/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2023-09-22 10:16:31.000000 django-config-models-2.5.1/config_models/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 10:16:38.419637 django-config-models-2.5.1/config_models/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 10:16:31.000000 django-config-models-2.5.1/config_models/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 10:16:38.419637 django-config-models-2.5.1/config_models/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 10:16:31.000000 django-config-models-2.5.1/config_models/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2456 2023-09-22 10:16:31.000000 django-config-models-2.5.1/config_models/management/commands/populate_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    10429 2023-09-22 10:16:31.000000 django-config-models-2.5.1/config_models/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 10:16:38.415637 django-config-models-2.5.1/config_models/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 10:16:38.419637 django-config-models-2.5.1/config_models/templates/config_models/
--rw-r--r--   0 runner    (1001) docker     (127)      662 2023-09-22 10:16:31.000000 django-config-models-2.5.1/config_models/templates/config_models/base.html
--rw-r--r--   0 runner    (1001) docker     (127)      980 2023-09-22 10:16:31.000000 django-config-models-2.5.1/config_models/templatetags.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2023-09-22 10:16:31.000000 django-config-models-2.5.1/config_models/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2023-09-22 10:16:31.000000 django-config-models-2.5.1/config_models/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2612 2023-09-22 10:16:31.000000 django-config-models-2.5.1/config_models/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 10:16:38.419637 django-config-models-2.5.1/django_config_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11266 2023-09-22 10:16:38.000000 django-config-models-2.5.1/django_config_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      900 2023-09-22 10:16:38.000000 django-config-models-2.5.1/django_config_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-22 10:16:38.000000 django-config-models-2.5.1/django_config_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-22 10:16:38.000000 django-config-models-2.5.1/django_config_models.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2023-09-22 10:16:38.000000 django-config-models-2.5.1/django_config_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-09-22 10:16:38.000000 django-config-models-2.5.1/django_config_models.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 10:16:38.419637 django-config-models-2.5.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2023-09-22 10:16:31.000000 django-config-models-2.5.1/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)      561 2023-09-22 10:16:31.000000 django-config-models-2.5.1/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-09-22 10:16:38.423637 django-config-models-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5192 2023-09-22 10:16:31.000000 django-config-models-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 10:16:38.423637 django-config-models-2.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2904 2023-09-22 10:16:31.000000 django-config-models-2.5.1/tests/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (127)    18582 2023-09-22 10:16:31.000000 django-config-models-2.5.1/tests/test_config_models.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2023-09-22 10:16:31.000000 django-config-models-2.5.1/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     7989 2023-09-22 10:16:31.000000 django-config-models-2.5.1/tests/test_model_deserialization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:10:44.992339 django-config-models-2.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-02 21:10:42.000000 django-config-models-2.6.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-04-02 21:10:42.000000 django-config-models-2.6.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35119 2024-04-02 21:10:42.000000 django-config-models-2.6.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-02 21:10:42.000000 django-config-models-2.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11463 2024-04-02 21:10:44.992339 django-config-models-2.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5864 2024-04-02 21:10:42.000000 django-config-models-2.6.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:10:44.988339 django-config-models-2.6.0/config_models/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-02 21:10:42.000000 django-config-models-2.6.0/config_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7978 2024-04-02 21:10:42.000000 django-config-models-2.6.0/config_models/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-02 21:10:42.000000 django-config-models-2.6.0/config_models/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-02 21:10:42.000000 django-config-models-2.6.0/config_models/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:10:44.988339 django-config-models-2.6.0/config_models/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 21:10:42.000000 django-config-models-2.6.0/config_models/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:10:44.988339 django-config-models-2.6.0/config_models/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 21:10:42.000000 django-config-models-2.6.0/config_models/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-04-02 21:10:42.000000 django-config-models-2.6.0/config_models/management/commands/populate_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10429 2024-04-02 21:10:42.000000 django-config-models-2.6.0/config_models/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:10:44.988339 django-config-models-2.6.0/config_models/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:10:44.988339 django-config-models-2.6.0/config_models/templates/config_models/
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-02 21:10:42.000000 django-config-models-2.6.0/config_models/templates/config_models/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-02 21:10:42.000000 django-config-models-2.6.0/config_models/templatetags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-02 21:10:42.000000 django-config-models-2.6.0/config_models/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-04-02 21:10:42.000000 django-config-models-2.6.0/config_models/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-04-02 21:10:42.000000 django-config-models-2.6.0/config_models/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:10:44.992339 django-config-models-2.6.0/django_config_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11463 2024-04-02 21:10:44.000000 django-config-models-2.6.0/django_config_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-02 21:10:44.000000 django-config-models-2.6.0/django_config_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 21:10:44.000000 django-config-models-2.6.0/django_config_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 21:10:44.000000 django-config-models-2.6.0/django_config_models.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-02 21:10:44.000000 django-config-models-2.6.0/django_config_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-02 21:10:44.000000 django-config-models-2.6.0/django_config_models.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:10:44.992339 django-config-models-2.6.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-02 21:10:42.000000 django-config-models-2.6.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-02 21:10:42.000000 django-config-models-2.6.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-02 21:10:44.992339 django-config-models-2.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5254 2024-04-02 21:10:42.000000 django-config-models-2.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:10:44.992339 django-config-models-2.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-04-02 21:10:42.000000 django-config-models-2.6.0/tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18582 2024-04-02 21:10:42.000000 django-config-models-2.6.0/tests/test_config_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-02 21:10:42.000000 django-config-models-2.6.0/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7989 2024-04-02 21:10:42.000000 django-config-models-2.6.0/tests/test_model_deserialization.py
```

### Comparing `django-config-models-2.5.1/CHANGELOG.rst` & `django-config-models-2.6.0/CHANGELOG.rst`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,20 @@
    but in reStructuredText instead of Markdown (for ease of incorporation into
    Sphinx documentation and the PyPI description).
 
    This project adheres to Semantic Versioning (http://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
+[2.6.0] - 2024-03-30
+~~~~~~~~~~~~~~~~~~~~
+
+* Adding python3.11 and 3.12 support.
+
+
 [2.5.1] - 2023-09-22
 ~~~~~~~~~~~~~~~~~~~~
 
 * Fixed issues with Django 4.2
 
 [2.5.0] - 2023-08-07
 ~~~~~~~~~~~~~~~~~~~~
```

### Comparing `django-config-models-2.5.1/LICENSE.txt` & `django-config-models-2.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-config-models-2.5.1/PKG-INFO` & `django-config-models-2.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 Metadata-Version: 2.1
 Name: django-config-models
-Version: 2.5.1
+Version: 2.6.0
 Summary: Configuration models for Django allowing config management with auditing.
 Home-page: https://github.com/openedx/django-config-models
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Django edx
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 License-File: LICENSE.txt
 License-File: AUTHORS
 Requires-Dist: Django
 Requires-Dist: djangorestframework>=3.6
 Requires-Dist: edx-django-utils
+Requires-Dist: setuptools
+Requires-Dist: wheel
 
 django-config-models
 ********************
 
 |CI|_ |Codecov|_ |pypi-badge| |doc-badge| |pyversions-badge| |license-badge| |status-badge|
 ===========================================================================================
 
@@ -176,15 +179,15 @@
 file in this repo.
 
 .. _Backstage: https://backstage.openedx.org/catalog/default/component/django-config-models
 
 Reporting Security Issues
 -------------------------
 
-Please do not report security issues in public. Please email security@edx.org.
+Please do not report security issues in public. Please email security@openedx.org.
 
 
 Change Log
 ----------
 
 ..
    All enhancements and patches to django-config-models will be documented
@@ -192,14 +195,20 @@
    but in reStructuredText instead of Markdown (for ease of incorporation into
    Sphinx documentation and the PyPI description).
 
    This project adheres to Semantic Versioning (http://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
+[2.6.0] - 2024-03-30
+~~~~~~~~~~~~~~~~~~~~
+
+* Adding python3.11 and 3.12 support.
+
+
 [2.5.1] - 2023-09-22
 ~~~~~~~~~~~~~~~~~~~~
 
 * Fixed issues with Django 4.2
 
 [2.5.0] - 2023-08-07
 ~~~~~~~~~~~~~~~~~~~~
```

### Comparing `django-config-models-2.5.1/README.rst` & `django-config-models-2.6.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -152,8 +152,8 @@
 file in this repo.
 
 .. _Backstage: https://backstage.openedx.org/catalog/default/component/django-config-models
 
 Reporting Security Issues
 -------------------------
 
-Please do not report security issues in public. Please email security@edx.org.
+Please do not report security issues in public. Please email security@openedx.org.
```

### Comparing `django-config-models-2.5.1/config_models/admin.py` & `django-config-models-2.6.0/config_models/admin.py`

 * *Files identical despite different names*

### Comparing `django-config-models-2.5.1/config_models/decorators.py` & `django-config-models-2.6.0/config_models/decorators.py`

 * *Files identical despite different names*

### Comparing `django-config-models-2.5.1/config_models/management/commands/populate_model.py` & `django-config-models-2.6.0/config_models/management/commands/populate_model.py`

 * *Files identical despite different names*

### Comparing `django-config-models-2.5.1/config_models/models.py` & `django-config-models-2.6.0/config_models/models.py`

 * *Files identical despite different names*

### Comparing `django-config-models-2.5.1/config_models/templates/config_models/base.html` & `django-config-models-2.6.0/config_models/templates/config_models/base.html`

 * *Files identical despite different names*

### Comparing `django-config-models-2.5.1/config_models/templatetags.py` & `django-config-models-2.6.0/config_models/templatetags.py`

 * *Files identical despite different names*

### Comparing `django-config-models-2.5.1/config_models/utils.py` & `django-config-models-2.6.0/config_models/utils.py`

 * *Files identical despite different names*

### Comparing `django-config-models-2.5.1/config_models/views.py` & `django-config-models-2.6.0/config_models/views.py`

 * *Files identical despite different names*

### Comparing `django-config-models-2.5.1/django_config_models.egg-info/PKG-INFO` & `django-config-models-2.6.0/django_config_models.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 Metadata-Version: 2.1
 Name: django-config-models
-Version: 2.5.1
+Version: 2.6.0
 Summary: Configuration models for Django allowing config management with auditing.
 Home-page: https://github.com/openedx/django-config-models
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Django edx
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 License-File: LICENSE.txt
 License-File: AUTHORS
 Requires-Dist: Django
 Requires-Dist: djangorestframework>=3.6
 Requires-Dist: edx-django-utils
+Requires-Dist: setuptools
+Requires-Dist: wheel
 
 django-config-models
 ********************
 
 |CI|_ |Codecov|_ |pypi-badge| |doc-badge| |pyversions-badge| |license-badge| |status-badge|
 ===========================================================================================
 
@@ -176,15 +179,15 @@
 file in this repo.
 
 .. _Backstage: https://backstage.openedx.org/catalog/default/component/django-config-models
 
 Reporting Security Issues
 -------------------------
 
-Please do not report security issues in public. Please email security@edx.org.
+Please do not report security issues in public. Please email security@openedx.org.
 
 
 Change Log
 ----------
 
 ..
    All enhancements and patches to django-config-models will be documented
@@ -192,14 +195,20 @@
    but in reStructuredText instead of Markdown (for ease of incorporation into
    Sphinx documentation and the PyPI description).
 
    This project adheres to Semantic Versioning (http://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
+[2.6.0] - 2024-03-30
+~~~~~~~~~~~~~~~~~~~~
+
+* Adding python3.11 and 3.12 support.
+
+
 [2.5.1] - 2023-09-22
 ~~~~~~~~~~~~~~~~~~~~
 
 * Fixed issues with Django 4.2
 
 [2.5.0] - 2023-08-07
 ~~~~~~~~~~~~~~~~~~~~
```

### Comparing `django-config-models-2.5.1/django_config_models.egg-info/SOURCES.txt` & `django-config-models-2.6.0/django_config_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-config-models-2.5.1/requirements/constraints.txt` & `django-config-models-2.6.0/requirements/constraints.txt`

 * *Files 23% similar despite different names*

```diff
@@ -4,9 +4,12 @@
 # that will be applied if a package is needed.
 #
 # When pinning something here, please provide an explanation of why.  Ideally,
 # link to other information that will help people in the future to remove the
 # pin when possible.  Writing an issue against the offending project and
 # linking to it here is good.
 
-# Common constraints for edx repos
--c https://raw.githubusercontent.com/edx/edx-lint/master/edx_lint/files/common_constraints.txt
+# This file contains all common constraints for edx-repos
+-c common_constraints.txt
+
+# Temporary to Support the python 3.11 Upgrade
+backports.zoneinfo;python_version<"3.9"  # Newer versions have zoneinfo available in the standard library
```

### Comparing `django-config-models-2.5.1/setup.py` & `django-config-models-2.6.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -113,16 +113,17 @@
     install_requires=load_requirements('requirements/base.in'),
     license="AGPL 3.0",
     zip_safe=False,
     keywords='Django edx',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Framework :: Django',
-        'Framework :: Django :: 3.2',
         'Framework :: Django :: 4.2',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
     ],
 )
```

### Comparing `django-config-models-2.5.1/tests/test_admin.py` & `django-config-models-2.6.0/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `django-config-models-2.5.1/tests/test_config_models.py` & `django-config-models-2.6.0/tests/test_config_models.py`

 * *Files identical despite different names*

### Comparing `django-config-models-2.5.1/tests/test_decorators.py` & `django-config-models-2.6.0/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `django-config-models-2.5.1/tests/test_model_deserialization.py` & `django-config-models-2.6.0/tests/test_model_deserialization.py`

 * *Files identical despite different names*

