# Comparing `tmp/django-spaday-0.1.2.tar.gz` & `tmp/django-spaday-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-spaday-0.1.2.tar", last modified: Thu Mar  7 21:00:34 2024, max compression
+gzip compressed data, was "django-spaday-0.1.3.tar", last modified: Tue Apr  2 17:14:15 2024, max compression
```

## Comparing `django-spaday-0.1.2.tar` & `django-spaday-0.1.3.tar`

### file list

```diff
@@ -1,60 +1,59 @@
-drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-03-07 21:00:34.427686 django-spaday-0.1.2/
--rw-r--r--   0 tsantor    (501) staff       (20)      200 2024-03-04 22:39:58.000000 django-spaday-0.1.2/AUTHORS.md
--rw-r--r--   0 tsantor    (501) staff       (20)      489 2024-03-07 21:00:25.000000 django-spaday-0.1.2/HISTORY.md
--rw-r--r--   0 tsantor    (501) staff       (20)     1079 2024-03-06 20:03:03.000000 django-spaday-0.1.2/LICENSE
--rw-r--r--   0 tsantor    (501) staff       (20)      237 2024-03-07 20:56:38.000000 django-spaday-0.1.2/MANIFEST.in
--rw-r--r--   0 tsantor    (501) staff       (20)     7119 2024-03-07 21:00:34.427367 django-spaday-0.1.2/PKG-INFO
--rw-r--r--   0 tsantor    (501) staff       (20)     5615 2024-03-07 19:46:48.000000 django-spaday-0.1.2/README.md
--rw-r--r--   0 tsantor    (501) staff       (20)     2821 2024-03-07 20:31:04.000000 django-spaday-0.1.2/pyproject.toml
--rw-r--r--   0 tsantor    (501) staff       (20)       49 2024-03-07 04:24:45.000000 django-spaday-0.1.2/requirements.txt
--rw-r--r--   0 tsantor    (501) staff       (20)       38 2024-03-07 21:00:34.427750 django-spaday-0.1.2/setup.cfg
--rwxr-xr-x   0 tsantor    (501) staff       (20)       69 2024-03-04 22:41:35.000000 django-spaday-0.1.2/setup.py
-drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-03-07 21:00:34.415320 django-spaday-0.1.2/src/
-drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-03-07 21:00:34.419796 django-spaday-0.1.2/src/django_spaday/
--rw-r--r--   0 tsantor    (501) staff       (20)       22 2024-03-07 20:58:17.000000 django-spaday-0.1.2/src/django_spaday/__init__.py
-drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-03-07 21:00:34.421954 django-spaday-0.1.2/src/django_spaday/api/
--rw-r--r--   0 tsantor    (501) staff       (20)        0 2024-03-06 20:03:03.000000 django-spaday-0.1.2/src/django_spaday/api/__init__.py
--rw-r--r--   0 tsantor    (501) staff       (20)     2162 2024-03-06 20:03:03.000000 django-spaday-0.1.2/src/django_spaday/api/pagination.py
--rw-r--r--   0 tsantor    (501) staff       (20)      319 2024-03-06 20:03:03.000000 django-spaday-0.1.2/src/django_spaday/api/permissions.py
--rw-r--r--   0 tsantor    (501) staff       (20)     1487 2024-03-06 20:03:03.000000 django-spaday-0.1.2/src/django_spaday/api/renderers.py
-drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-03-07 21:00:34.423396 django-spaday-0.1.2/src/django_spaday/api/serializers/
--rw-r--r--   0 tsantor    (501) staff       (20)      530 2024-03-06 20:03:03.000000 django-spaday-0.1.2/src/django_spaday/api/serializers/__init__.py
--rw-r--r--   0 tsantor    (501) staff       (20)     2326 2024-03-06 20:03:03.000000 django-spaday-0.1.2/src/django_spaday/api/serializers/auditlog.py
--rw-r--r--   0 tsantor    (501) staff       (20)     7586 2024-03-06 20:03:03.000000 django-spaday-0.1.2/src/django_spaday/api/serializers/auth.py
--rw-r--r--   0 tsantor    (501) staff       (20)      330 2024-03-06 20:03:03.000000 django-spaday-0.1.2/src/django_spaday/api/serializers/deleted.py
--rw-r--r--   0 tsantor    (501) staff       (20)      644 2024-03-06 20:03:03.000000 django-spaday-0.1.2/src/django_spaday/api/serializers/django_celery_results.py
--rw-r--r--   0 tsantor    (501) staff       (20)      643 2024-03-06 20:03:03.000000 django-spaday-0.1.2/src/django_spaday/api/serializers/filters.py
--rw-r--r--   0 tsantor    (501) staff       (20)      898 2024-03-06 20:03:03.000000 django-spaday-0.1.2/src/django_spaday/api/urls.py
--rw-r--r--   0 tsantor    (501) staff       (20)      695 2024-03-06 20:03:03.000000 django-spaday-0.1.2/src/django_spaday/api/utils.py
--rw-r--r--   0 tsantor    (501) staff       (20)     7507 2024-03-06 20:03:03.000000 django-spaday-0.1.2/src/django_spaday/api/views.py
--rw-r--r--   0 tsantor    (501) staff       (20)      851 2024-03-06 20:03:03.000000 django-spaday-0.1.2/src/django_spaday/api/viewsets.py
--rw-r--r--   0 tsantor    (501) staff       (20)      270 2024-03-06 20:03:03.000000 django-spaday-0.1.2/src/django_spaday/apps.py
-drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-03-07 21:00:34.423643 django-spaday-0.1.2/src/django_spaday/management/
--rw-r--r--   0 tsantor    (501) staff       (20)        0 2024-03-06 20:03:03.000000 django-spaday-0.1.2/src/django_spaday/management/__init__.py
-drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-03-07 21:00:34.423956 django-spaday-0.1.2/src/django_spaday/management/commands/
--rw-r--r--   0 tsantor    (501) staff       (20)        0 2024-03-06 20:03:03.000000 django-spaday-0.1.2/src/django_spaday/management/commands/__init__.py
--rw-r--r--   0 tsantor    (501) staff       (20)     1016 2024-03-06 20:03:03.000000 django-spaday-0.1.2/src/django_spaday/management/commands/export_perms.py
-drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-03-07 21:00:34.424585 django-spaday-0.1.2/src/django_spaday/migrations/
--rw-r--r--   0 tsantor    (501) staff       (20)      623 2024-03-06 20:03:03.000000 django-spaday-0.1.2/src/django_spaday/migrations/0001_initial.py
--rw-r--r--   0 tsantor    (501) staff       (20)        0 2024-03-06 20:03:03.000000 django-spaday-0.1.2/src/django_spaday/migrations/__init__.py
--rw-r--r--   0 tsantor    (501) staff       (20)      574 2024-03-06 20:03:03.000000 django-spaday-0.1.2/src/django_spaday/models.py
--rw-r--r--   0 tsantor    (501) staff       (20)     5159 2024-03-06 20:03:03.000000 django-spaday-0.1.2/src/django_spaday/settings.py
-drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-03-07 21:00:34.416017 django-spaday-0.1.2/src/django_spaday/templates/
-drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-03-07 21:00:34.424787 django-spaday-0.1.2/src/django_spaday/templates/includes/
--rw-r--r--   0 tsantor    (501) staff       (20)     2183 2024-03-06 20:03:03.000000 django-spaday-0.1.2/src/django_spaday/templates/includes/favicons.html
-drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-03-07 21:00:34.425092 django-spaday-0.1.2/src/django_spaday/templates/spaday/
--rw-r--r--   0 tsantor    (501) staff       (20)     1571 2024-03-06 20:03:03.000000 django-spaday-0.1.2/src/django_spaday/templates/spaday/vue.html
--rw-r--r--   0 tsantor    (501) staff       (20)      351 2024-03-06 20:03:03.000000 django-spaday-0.1.2/src/django_spaday/urls.py
--rw-r--r--   0 tsantor    (501) staff       (20)      546 2024-03-06 20:03:03.000000 django-spaday-0.1.2/src/django_spaday/utils.py
--rw-r--r--   0 tsantor    (501) staff       (20)      117 2024-03-06 20:03:03.000000 django-spaday-0.1.2/src/django_spaday/views.py
-drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-03-07 21:00:34.426735 django-spaday-0.1.2/src/django_spaday.egg-info/
--rw-r--r--   0 tsantor    (501) staff       (20)     7119 2024-03-07 21:00:34.000000 django-spaday-0.1.2/src/django_spaday.egg-info/PKG-INFO
--rw-r--r--   0 tsantor    (501) staff       (20)     1456 2024-03-07 21:00:34.000000 django-spaday-0.1.2/src/django_spaday.egg-info/SOURCES.txt
--rw-r--r--   0 tsantor    (501) staff       (20)        1 2024-03-07 21:00:34.000000 django-spaday-0.1.2/src/django_spaday.egg-info/dependency_links.txt
--rw-r--r--   0 tsantor    (501) staff       (20)      128 2024-03-07 21:00:34.000000 django-spaday-0.1.2/src/django_spaday.egg-info/requires.txt
--rw-r--r--   0 tsantor    (501) staff       (20)       14 2024-03-07 21:00:34.000000 django-spaday-0.1.2/src/django_spaday.egg-info/top_level.txt
-drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-03-07 21:00:34.426377 django-spaday-0.1.2/tests/
--rw-r--r--   0 tsantor    (501) staff       (20)     9844 2024-03-06 20:03:03.000000 django-spaday-0.1.2/tests/test_api.py
--rw-r--r--   0 tsantor    (501) staff       (20)      692 2024-03-07 04:32:15.000000 django-spaday-0.1.2/tests/test_pagination.py
--rw-r--r--   0 tsantor    (501) staff       (20)     1582 2024-03-06 20:03:03.000000 django-spaday-0.1.2/tests/test_serializers.py
--rw-r--r--   0 tsantor    (501) staff       (20)     1001 2024-03-06 20:03:03.000000 django-spaday-0.1.2/tests/test_utils.py
+drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-02 17:14:15.214071 django-spaday-0.1.3/
+-rw-r--r--   0 tsantor    (501) staff       (20)      200 2024-03-04 22:39:58.000000 django-spaday-0.1.3/AUTHORS.md
+-rw-r--r--   0 tsantor    (501) staff       (20)      544 2024-04-02 17:11:05.000000 django-spaday-0.1.3/HISTORY.md
+-rw-r--r--   0 tsantor    (501) staff       (20)     1079 2024-03-06 20:03:03.000000 django-spaday-0.1.3/LICENSE
+-rw-r--r--   0 tsantor    (501) staff       (20)      237 2024-03-07 20:56:38.000000 django-spaday-0.1.3/MANIFEST.in
+-rw-r--r--   0 tsantor    (501) staff       (20)     7173 2024-04-02 17:14:15.213818 django-spaday-0.1.3/PKG-INFO
+-rw-r--r--   0 tsantor    (501) staff       (20)     5615 2024-04-01 18:21:44.000000 django-spaday-0.1.3/README.md
+-rw-r--r--   0 tsantor    (501) staff       (20)     4812 2024-04-01 19:12:05.000000 django-spaday-0.1.3/pyproject.toml
+-rw-r--r--   0 tsantor    (501) staff       (20)       38 2024-04-02 17:14:15.214124 django-spaday-0.1.3/setup.cfg
+-rwxr-xr-x   0 tsantor    (501) staff       (20)       69 2024-03-04 22:41:35.000000 django-spaday-0.1.3/setup.py
+drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-02 17:14:15.205938 django-spaday-0.1.3/src/
+drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-02 17:14:15.208980 django-spaday-0.1.3/src/django_spaday/
+-rw-r--r--   0 tsantor    (501) staff       (20)       22 2024-04-02 17:11:00.000000 django-spaday-0.1.3/src/django_spaday/__init__.py
+drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-02 17:14:15.210824 django-spaday-0.1.3/src/django_spaday/api/
+-rw-r--r--   0 tsantor    (501) staff       (20)        0 2024-03-06 20:03:03.000000 django-spaday-0.1.3/src/django_spaday/api/__init__.py
+-rw-r--r--   0 tsantor    (501) staff       (20)     1746 2024-04-01 17:32:52.000000 django-spaday-0.1.3/src/django_spaday/api/pagination.py
+-rw-r--r--   0 tsantor    (501) staff       (20)      319 2024-03-06 20:03:03.000000 django-spaday-0.1.3/src/django_spaday/api/permissions.py
+-rw-r--r--   0 tsantor    (501) staff       (20)     1509 2024-04-01 17:51:32.000000 django-spaday-0.1.3/src/django_spaday/api/renderers.py
+drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-02 17:14:15.211685 django-spaday-0.1.3/src/django_spaday/api/serializers/
+-rw-r--r--   0 tsantor    (501) staff       (20)      530 2024-03-06 20:03:03.000000 django-spaday-0.1.3/src/django_spaday/api/serializers/__init__.py
+-rw-r--r--   0 tsantor    (501) staff       (20)     2326 2024-03-06 20:03:03.000000 django-spaday-0.1.3/src/django_spaday/api/serializers/auditlog.py
+-rw-r--r--   0 tsantor    (501) staff       (20)     7776 2024-04-01 20:20:03.000000 django-spaday-0.1.3/src/django_spaday/api/serializers/auth.py
+-rw-r--r--   0 tsantor    (501) staff       (20)      330 2024-03-06 20:03:03.000000 django-spaday-0.1.3/src/django_spaday/api/serializers/deleted.py
+-rw-r--r--   0 tsantor    (501) staff       (20)      644 2024-03-06 20:03:03.000000 django-spaday-0.1.3/src/django_spaday/api/serializers/django_celery_results.py
+-rw-r--r--   0 tsantor    (501) staff       (20)      643 2024-03-06 20:03:03.000000 django-spaday-0.1.3/src/django_spaday/api/serializers/filters.py
+-rw-r--r--   0 tsantor    (501) staff       (20)      898 2024-03-06 20:03:03.000000 django-spaday-0.1.3/src/django_spaday/api/urls.py
+-rw-r--r--   0 tsantor    (501) staff       (20)      749 2024-04-01 18:12:54.000000 django-spaday-0.1.3/src/django_spaday/api/utils.py
+-rw-r--r--   0 tsantor    (501) staff       (20)     7539 2024-04-01 18:13:40.000000 django-spaday-0.1.3/src/django_spaday/api/views.py
+-rw-r--r--   0 tsantor    (501) staff       (20)      851 2024-03-06 20:03:03.000000 django-spaday-0.1.3/src/django_spaday/api/viewsets.py
+-rw-r--r--   0 tsantor    (501) staff       (20)      270 2024-03-06 20:03:03.000000 django-spaday-0.1.3/src/django_spaday/apps.py
+drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-02 17:14:15.211832 django-spaday-0.1.3/src/django_spaday/management/
+-rw-r--r--   0 tsantor    (501) staff       (20)        0 2024-03-06 20:03:03.000000 django-spaday-0.1.3/src/django_spaday/management/__init__.py
+drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-02 17:14:15.212073 django-spaday-0.1.3/src/django_spaday/management/commands/
+-rw-r--r--   0 tsantor    (501) staff       (20)        0 2024-03-06 20:03:03.000000 django-spaday-0.1.3/src/django_spaday/management/commands/__init__.py
+-rw-r--r--   0 tsantor    (501) staff       (20)     1016 2024-03-06 20:03:03.000000 django-spaday-0.1.3/src/django_spaday/management/commands/export_perms.py
+drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-02 17:14:15.212351 django-spaday-0.1.3/src/django_spaday/migrations/
+-rw-r--r--   0 tsantor    (501) staff       (20)      623 2024-03-06 20:03:03.000000 django-spaday-0.1.3/src/django_spaday/migrations/0001_initial.py
+-rw-r--r--   0 tsantor    (501) staff       (20)        0 2024-03-06 20:03:03.000000 django-spaday-0.1.3/src/django_spaday/migrations/__init__.py
+-rw-r--r--   0 tsantor    (501) staff       (20)      574 2024-03-06 20:03:03.000000 django-spaday-0.1.3/src/django_spaday/models.py
+-rw-r--r--   0 tsantor    (501) staff       (20)     5159 2024-03-06 20:03:03.000000 django-spaday-0.1.3/src/django_spaday/settings.py
+drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-02 17:14:15.206745 django-spaday-0.1.3/src/django_spaday/templates/
+drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-02 17:14:15.212462 django-spaday-0.1.3/src/django_spaday/templates/includes/
+-rw-r--r--   0 tsantor    (501) staff       (20)     2183 2024-03-06 20:03:03.000000 django-spaday-0.1.3/src/django_spaday/templates/includes/favicons.html
+drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-02 17:14:15.212601 django-spaday-0.1.3/src/django_spaday/templates/spaday/
+-rw-r--r--   0 tsantor    (501) staff       (20)     1728 2024-03-30 03:46:49.000000 django-spaday-0.1.3/src/django_spaday/templates/spaday/vue.html
+-rw-r--r--   0 tsantor    (501) staff       (20)      351 2024-03-06 20:03:03.000000 django-spaday-0.1.3/src/django_spaday/urls.py
+-rw-r--r--   0 tsantor    (501) staff       (20)      576 2024-04-01 17:51:32.000000 django-spaday-0.1.3/src/django_spaday/utils.py
+-rw-r--r--   0 tsantor    (501) staff       (20)      117 2024-03-06 20:03:03.000000 django-spaday-0.1.3/src/django_spaday/views.py
+drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-02 17:14:15.213364 django-spaday-0.1.3/src/django_spaday.egg-info/
+-rw-r--r--   0 tsantor    (501) staff       (20)     7173 2024-04-02 17:14:15.000000 django-spaday-0.1.3/src/django_spaday.egg-info/PKG-INFO
+-rw-r--r--   0 tsantor    (501) staff       (20)     1439 2024-04-02 17:14:15.000000 django-spaday-0.1.3/src/django_spaday.egg-info/SOURCES.txt
+-rw-r--r--   0 tsantor    (501) staff       (20)        1 2024-04-02 17:14:15.000000 django-spaday-0.1.3/src/django_spaday.egg-info/dependency_links.txt
+-rw-r--r--   0 tsantor    (501) staff       (20)      128 2024-04-02 17:14:15.000000 django-spaday-0.1.3/src/django_spaday.egg-info/requires.txt
+-rw-r--r--   0 tsantor    (501) staff       (20)       14 2024-04-02 17:14:15.000000 django-spaday-0.1.3/src/django_spaday.egg-info/top_level.txt
+drwxr-xr-x   0 tsantor    (501) staff       (20)        0 2024-04-02 17:14:15.213179 django-spaday-0.1.3/tests/
+-rw-r--r--   0 tsantor    (501) staff       (20)    10001 2024-04-01 20:20:16.000000 django-spaday-0.1.3/tests/test_api.py
+-rw-r--r--   0 tsantor    (501) staff       (20)      848 2024-04-01 18:17:39.000000 django-spaday-0.1.3/tests/test_pagination.py
+-rw-r--r--   0 tsantor    (501) staff       (20)     1638 2024-04-01 20:22:21.000000 django-spaday-0.1.3/tests/test_serializers.py
+-rw-r--r--   0 tsantor    (501) staff       (20)     1001 2024-03-06 20:03:03.000000 django-spaday-0.1.3/tests/test_utils.py
```

### Comparing `django-spaday-0.1.2/LICENSE` & `django-spaday-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-spaday-0.1.2/PKG-INFO` & `django-spaday-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: django-spaday
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Django package that provides 'out-of-the-box' JWT auth, user, group, and permission APIs for use in Single Page Apps (eg - Vue, React).
 Author-email: Tim Santor <tsantor@xstudios.com>
 Project-URL: homepage, https://github.com/tsantor/django-spaday
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 Requires-Dist: django<5.0,>=4.0
 Requires-Dist: drf-spectacular
 Requires-Dist: django-auditlog
 Requires-Dist: django-celery-results
@@ -134,15 +134,15 @@
 1. `make serve`
 
 - Visit `http://127.0.0.1:8000/djadmin/` for the Django Admin
 - Visit `http://127.0.0.1:8000/api/docs/` for the API docs
 
 ### Testing
 
-Currently django_spaday has **94%** test coverage.
+Currently django_spaday has **95%** test coverage.
 
 - Pytest: `make pytest`
 - Coverage: `make coverage`
   - Open Report: `make open_coverage`
 
 ## Makefile Commands
 
@@ -215,18 +215,21 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.1.3] - 2024-04-02
+- Moved to `ruff` and added tests
+
 ## [0.1.2] - 2024-03-07
 
 - Added missing template example (assumes your Vue project has been built to `project/static/vue-frontend`)
 
 ## [0.1.1] - 2024-03-07
 
-- Added 94% test coverage
+- Added test coverage
 
 ## [0.1.0] - 2022-04-19
 
 - First release on PyPI.
```

### Comparing `django-spaday-0.1.2/README.md` & `django-spaday-0.1.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
 1. `make serve`
 
 - Visit `http://127.0.0.1:8000/djadmin/` for the Django Admin
 - Visit `http://127.0.0.1:8000/api/docs/` for the API docs
 
 ### Testing
 
-Currently django_spaday has **94%** test coverage.
+Currently django_spaday has **95%** test coverage.
 
 - Pytest: `make pytest`
 - Coverage: `make coverage`
   - Open Report: `make open_coverage`
 
 ## Makefile Commands
```

### Comparing `django-spaday-0.1.2/src/django_spaday/api/pagination.py` & `django-spaday-0.1.3/src/django_spaday/api/pagination.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,57 +1,47 @@
 from rest_framework import pagination
 from rest_framework.response import Response
-
-# class StandardPagination(pagination.PageNumberPagination):
-#     page_size = 10
-#     max_page_size = 100
-#     page_size_query_param = "size"
-#     page_query_param = "page"
-
-#     def get_page_links(self):
-#         page_links = self.get_html_context()["page_links"]
-#         return [
-#             {"number": pl.number, "url": pl.url, "is_active": pl.is_active}
-#             for pl in page_links
-#         ]
-
-#     def get_paginated_response(self, data):
-#         return Response(
-#             {
-#                 # "links": {
-#                 #     "next": self.get_next_link(),
-#                 #     "previous": self.get_previous_link(),
-#                 # },
-#                 # "has_next": self.page.has_next(),
-#                 # "has_previous": self.page.has_previous(),
-#                 # "has_other_pages": self.page.has_other_pages(),
-#                 # "next_page_number": self.page.next_page_number(),
-#                 # "previous_page_number": self.page.previous_page_number(),
-#                 "current_page": self.page.number,
-#                 "num_pages": self.page.paginator.num_pages,
-#                 # "page_range": [p for p in self.page.paginator.page_range],
-#                 # "page_links": self.get_page_links(),
-#                 "start_index": self.page.start_index(),
-#                 "end_index": self.page.end_index(),
-#                 "num_results": self.page.paginator.count,
-#                 "results": data,
-#             }
-#         )
+from rest_framework.utils.urls import replace_query_param
 
 
 class StandardPagination(pagination.PageNumberPagination):
     page_size = 10
     max_page_size = 100
     page_size_query_param = "size"
     page_query_param = "page"
 
+    def get_first_link(self):
+        """Return the first page link."""
+        url = self.request.build_absolute_uri()
+        page_number = 1
+        return replace_query_param(url, self.page_query_param, page_number)
+
+    def get_last_link(self):
+        """Return the last page link."""
+        url = self.request.build_absolute_uri()
+        page_number = self.page.paginator.num_pages
+        return replace_query_param(url, self.page_query_param, page_number)
+
     def get_paginated_response(self, data):
+        next_page = self.page.next_page_number() if self.page.has_next() else None
+        previous_page = (
+            self.page.previous_page_number() if self.page.has_previous() else None
+        )
+
         return Response(
             {
+                "links": {
+                    "next": self.get_next_link(),
+                    "previous": self.get_previous_link(),
+                    "first": self.get_first_link(),
+                    "last": self.get_last_link(),
+                },
+                "next_page": next_page,
+                "previous_page": previous_page,
                 "current_page": self.page.number,
                 "num_pages": self.page.paginator.num_pages,
-                "start_index": self.page.start_index(),
-                "end_index": self.page.end_index(),
                 "num_results": self.page.paginator.count,
+                # "start_index": self.page.start_index(),
+                # "end_index": self.page.end_index(),
                 "results": data,
             }
         )
```

### Comparing `django-spaday-0.1.2/src/django_spaday/api/renderers.py` & `django-spaday-0.1.3/src/django_spaday/api/renderers.py`

 * *Files 16% similar despite different names*

```diff
@@ -41,13 +41,15 @@
 
         # Modify the response into a cohesive response format
         modified_data = {
             "code": response.status_code,
             "status": get_status(response.status_code),
         }
 
-        if status.is_client_error(response.status_code) or status.is_server_error(response.status_code):
+        if status.is_client_error(response.status_code) or status.is_server_error(
+            response.status_code
+        ):
             modified_data["errors"] = data
         else:
             modified_data["data"] = data
 
         return super().render(modified_data, accepted_media_type, renderer_context)
```

### Comparing `django-spaday-0.1.2/src/django_spaday/api/serializers/__init__.py` & `django-spaday-0.1.3/src/django_spaday/api/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `django-spaday-0.1.2/src/django_spaday/api/serializers/auditlog.py` & `django-spaday-0.1.3/src/django_spaday/api/serializers/auditlog.py`

 * *Files identical despite different names*

### Comparing `django-spaday-0.1.2/src/django_spaday/api/serializers/auth.py` & `django-spaday-0.1.3/src/django_spaday/api/serializers/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from django.contrib.auth import get_user_model
-from django.contrib.auth.models import Group, Permission
+from django.contrib.auth.models import Group
+from django.contrib.auth.models import Permission
 from django.contrib.auth.password_validation import validate_password
 from rest_framework import serializers
 
 User = get_user_model()
 
 
 # class CsrfSerializer(serializers.Serializer):
@@ -126,15 +127,15 @@
     def get_full_name(self, instance) -> str:
         first_name = instance.first_name or ""
         last_name = instance.last_name or ""
         return f"{first_name} {last_name}".strip()
 
     def create(self, validated_data):
         validated_data["email"] = validated_data["email"].lower()
-        if "username" in User._meta.get_fields():
+        if "username" in User._meta.get_fields():  # noqa: SLF001
             validated_data["username"] = validated_data["email"]
         password = validated_data.pop("password")
         # groups = validated_data.pop("groups")
         # permissions = validated_data.pop("user_permissions")
 
         user = super().create(validated_data)
         user.set_password(password)
@@ -145,42 +146,46 @@
         return user
 
     def update(self, instance, validated_data):
         # This ensures the username is email, and email is lower case
         if "email" in validated_data:
             validated_data["email"] = validated_data["email"].lower()
 
-        if "username" in User._meta.get_fields():
+        if "username" in User._meta.get_fields():  # noqa: SLF001
             validated_data["username"] = validated_data.pop("email", None)
 
         # groups = validated_data.pop("groups")
         # permissions = validated_data.pop("user_permissions")
 
         user = super().update(instance, validated_data)
         # user.save()
 
         # user.groups.set(list(groups))
         # user.user_permissions.set(list(permissions))
-        return user
+        return user  # noqa: RET504
 
 
 class ChangePasswordSerializer(serializers.ModelSerializer):
     """This can be overriden in the SPA_DAY settings."""
 
-    password = serializers.CharField(write_only=True, required=True, validators=[validate_password])
+    password = serializers.CharField(
+        write_only=True, required=True, validators=[validate_password]
+    )
     password2 = serializers.CharField(write_only=True, required=True)
     # old_password = serializers.CharField(write_only=True, required=True)
 
     class Meta:
         model = User
         fields = ("password", "password2")
 
     def validate(self, attrs):
         if attrs["password"] != attrs["password2"]:
-            raise serializers.ValidationError({"password": "Password fields didn't match."})
+            raise serializers.ValidationError(
+                {"password": "Password fields didn't match."}
+            )
         return attrs
 
     # def validate_old_password(self, value):
     #     user = self.context["request"].user
     #     if not user.check_password(value):
     #         raise serializers.ValidationError({"old_password": "Old password is not correct"})
     #     return value
@@ -210,25 +215,27 @@
             "email",
             "permissions_codenames",
             "initials",
             "full_name",
         )
 
     def get_permissions_codenames(self, instance) -> list:
-        return sorted(list(instance.get_all_permissions()))
+        return sorted(instance.get_all_permissions())
 
     def get_initials(self, instance) -> str:
-        if instance.first_name and instance.last_name:
-            first_name = instance.first_name[0]
-            last_name = instance.last_name[0]
-            return f"{first_name}{last_name}".upper()
+        if hasattr(instance, "initials"):
+            return instance.initials
+        first_name = instance.first_name[0] if instance.first_name else "?"
+        last_name = instance.last_name[0] if instance.last_name else "?"
+        return f"{first_name}{last_name}".upper()
 
     def get_full_name(self, instance) -> str:
-        if instance.first_name and instance.last_name:
-            return f"{instance.first_name} {instance.last_name}"
+        if hasattr(instance, "full_name"):
+            return instance.full_name
+        return instance.email
 
 
 class LastLoginSerializer(serializers.ModelSerializer):
     """This can be overriden in the SPA_DAY settings."""
 
     class Meta:
         model = User
```

### Comparing `django-spaday-0.1.2/src/django_spaday/api/serializers/django_celery_results.py` & `django-spaday-0.1.3/src/django_spaday/api/serializers/django_celery_results.py`

 * *Files identical despite different names*

### Comparing `django-spaday-0.1.2/src/django_spaday/api/serializers/filters.py` & `django-spaday-0.1.3/src/django_spaday/api/serializers/filters.py`

 * *Files identical despite different names*

### Comparing `django-spaday-0.1.2/src/django_spaday/api/urls.py` & `django-spaday-0.1.3/src/django_spaday/api/urls.py`

 * *Files identical despite different names*

### Comparing `django-spaday-0.1.2/src/django_spaday/api/utils.py` & `django-spaday-0.1.3/src/django_spaday/api/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,18 @@
 
 def get_deleted_objects(objs):
     """Based on `django/contrib/admin/utils.py`"""
     collector = NestedObjects(using="default")
     collector.collect(objs)
 
     def format_callback(obj):
-        opts = obj._meta
+        opts = obj._meta  # noqa: SLF001
         return f"{capfirst(opts.verbose_name)}: {force_str(obj)}"
 
     to_delete = collector.nested(format_callback)
     protected = [format_callback(obj) for obj in collector.protected]
-    model_count = {model._meta.verbose_name_plural: len(objs) for model, objs in collector.model_objs.items()}
+    model_count = {
+        model._meta.verbose_name_plural: len(objs)  # noqa: SLF001
+        for model, objs in collector.model_objs.items()
+    }
 
     return to_delete, model_count, protected
```

### Comparing `django-spaday-0.1.2/src/django_spaday/api/views.py` & `django-spaday-0.1.3/src/django_spaday/api/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 from auditlog.models import LogEntry
 from dj_rest_auth.views import LoginView
 from django.contrib.auth import get_user_model
-from django.contrib.auth.models import Group, Permission, update_last_login
+from django.contrib.auth.models import Group
+from django.contrib.auth.models import Permission
+from django.contrib.auth.models import update_last_login
 from django_celery_results.models import TaskResult
 from django_filters.rest_framework import DjangoFilterBackend
 from django_perm_filter import filter_perms
 from drf_spectacular.utils import extend_schema
 from rest_framework import filters
 from rest_framework.decorators import action
 from rest_framework.permissions import IsAuthenticated
 from rest_framework.response import Response
 from rest_framework.viewsets import GenericViewSet
 
-from ..settings import api_settings
-from ..utils import permissions_as_combobox
+from django_spaday.settings import api_settings
+from django_spaday.utils import permissions_as_combobox
+
 from .pagination import StandardPagination
-from .serializers import (
-    GroupAddUserSerializer,
-    GroupRemoveUserSerializer,
-    LogEntrySerializer,
-    PermissionSerializer,
-    TaskResultSerializer,
-)
+from .serializers import GroupAddUserSerializer
+from .serializers import GroupRemoveUserSerializer
+from .serializers import LogEntrySerializer
+from .serializers import PermissionSerializer
+from .serializers import TaskResultSerializer
 from .serializers.filters import LogEntryFilter
 from .viewsets import MyModelViewSet
 
 # from rest_framework.generics import GenericAPIView
 # from django.middleware.csrf import get_token
 # from django.utils.decorators import method_decorator
 # from django.views.decorators.cache import cache_page
@@ -88,27 +89,23 @@
 
     @action(detail=False, methods=["get"], url_path=r"recent-logins")
     def recent_logins(self, request):
         if request.user.is_superuser:
             recent_users = User.objects.exclude(
                 last_login__isnull=True,
                 is_staff=False,
-            ).order_by(
-                "-last_login"
-            )[:10]
+            ).order_by("-last_login")[:10]
+        elif hasattr(request.user, "company"):
+            recent_users = (
+                User.objects.filter(company=request.user.company)
+                .exclude(last_login__isnull=True, is_staff=False)
+                .order_by("-last_login")[:10]
+            )
         else:
-            # TODO: Clean this up as not all users have a company
-            if hasattr(request.user, "company"):
-                recent_users = (
-                    User.objects.filter(company=request.user.company)
-                    .exclude(last_login__isnull=True, is_staff=False)
-                    .order_by("-last_login")[:10]
-                )
-            else:
-                recent_users = User.objects.filter(pk=request.user.pk, is_staff=True)
+            recent_users = User.objects.filter(pk=request.user.pk, is_staff=True)
         serializer = self.get_serializer(recent_users, many=True)
         return Response(serializer.data)
 
 
 @extend_schema(tags=["spaday"])
 class GroupViewSet(MyModelViewSet):
     http_method_names = ["get", "post", "put", "delete"]
```

### Comparing `django-spaday-0.1.2/src/django_spaday/api/viewsets.py` & `django-spaday-0.1.3/src/django_spaday/api/viewsets.py`

 * *Files identical despite different names*

### Comparing `django-spaday-0.1.2/src/django_spaday/management/commands/export_perms.py` & `django-spaday-0.1.3/src/django_spaday/management/commands/export_perms.py`

 * *Files identical despite different names*

### Comparing `django-spaday-0.1.2/src/django_spaday/migrations/0001_initial.py` & `django-spaday-0.1.3/src/django_spaday/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-spaday-0.1.2/src/django_spaday/models.py` & `django-spaday-0.1.3/src/django_spaday/models.py`

 * *Files identical despite different names*

### Comparing `django-spaday-0.1.2/src/django_spaday/settings.py` & `django-spaday-0.1.3/src/django_spaday/settings.py`

 * *Files identical despite different names*

### Comparing `django-spaday-0.1.2/src/django_spaday/templates/includes/favicons.html` & `django-spaday-0.1.3/src/django_spaday/templates/includes/favicons.html`

 * *Files identical despite different names*

### Comparing `django-spaday-0.1.2/src/django_spaday/templates/spaday/vue.html` & `django-spaday-0.1.3/src/django_spaday/templates/spaday/vue.html`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,43 @@
 {% load static i18n %}
+
 <!DOCTYPE html>
 <html lang="en">
-
-<head>
-  <meta charset="utf-8">
-  <meta http-equiv="X-UA-Compatible" content="IE=edge">
-    <meta name="viewport" content="width=device-width,initial-scale=1,shrink-to-fit=no">
-  <meta name="description" content="{{ PROJECT_TITLE }}">
-  <meta name="author" content="Tim Santor">
-  <title>{{ PROJECT_TITLE }} </title>
-  {% comment %} {% include "includes/favicons.html" %} {% endcomment %}
-  <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Roboto:100,300,400,500,700,900">
-  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@mdi/font@latest/css/materialdesignicons.min.css">
-
-  <!-- vue app specific imports -->
-  <link href="{% static 'vue-frontend/css/app.css' %}" rel="preload" as="style">
-  <link href="{% static 'vue-frontend/css/chunk-vendors.css' %}" rel="preload" as="style">
-  <link href="{% static 'vue-frontend/js/app.js' %}" rel="preload" as="script">
-  <link href="{% static 'vue-frontend/js/chunk-vendors.js' %}" rel="preload" as="script">
-
-  <link href="{% static 'vue-frontend/css/chunk-vendors.css' %}" rel="stylesheet">
-  <link href="{% static 'vue-frontend/css/app.css' %}" rel="stylesheet">
-</head>
-
-<body><noscript><strong>We're sorry but Djangp Spaday Admin doesn't work properly without JavaScript enabled. Please enable it
-      to continue.</strong></noscript>
-  <div id="app"></div>
+  <head>
+    <meta charset="utf-8" />
+    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
+    <meta name="viewport"
+          content="width=device-width,initial-scale=1,shrink-to-fit=no" />
+    <meta name="description" content="{{ PROJECT_TITLE }}" />
+    <meta name="author" content="Tim Santor" />
+    <title>{{ PROJECT_TITLE }}</title>
+    {% include "includes/favicons.html" %}
+    <link rel="stylesheet"
+          href="https://fonts.googleapis.com/css?family=Roboto:100,300,400,500,700,900" />
+    <link rel="stylesheet"
+          href="https://cdn.jsdelivr.net/npm/@mdi/font@latest/css/materialdesignicons.min.css" />
+    <!-- vue app specific imports -->
+    <link href="{% static 'vue-frontend/css/app.css' %}"
+          rel="preload"
+          as="style" />
+    <link href="{% static 'vue-frontend/css/chunk-vendors.css' %}"
+          rel="preload"
+          as="style" />
+    <link href="{% static 'vue-frontend/js/app.js' %}"
+          rel="preload"
+          as="script" />
+    <link href="{% static 'vue-frontend/js/chunk-vendors.js' %}"
+          rel="preload"
+          as="script" />
+    <link href="{% static 'vue-frontend/css/chunk-vendors.css' %}"
+          rel="stylesheet" />
+    <link href="{% static 'vue-frontend/css/app.css' %}" rel="stylesheet" />
+  </head>
+  <body>
+    <noscript><strong>We're sorry but Djangp Spaday Admin doesn't work properly without JavaScript enabled. Please enable it
+    to continue.</strong></noscript>
+    <div id="app"></div>
     {% csrf_token %}
-  <script src="{% static 'vue-frontend/js/chunk-vendors.js' %}"></script>
-  <script src="{% static 'vue-frontend/js/app.js' %}"></script>
-</body>
-
+    <script src="{% static 'vue-frontend/js/chunk-vendors.js' %}"></script>
+    <script src="{% static 'vue-frontend/js/app.js' %}"></script>
+  </body>
 </html>
```

#### html2text {}

```diff
@@ -1,5 +1,5 @@
 {% load static i18n %}
-{% comment %} {% include "includes/favicons.html" %} {% endcomment %}
+{% include "includes/favicons.html" %}
 WWee''rree ssoorrrryy bbuutt DDjjaannggpp SSppaaddaayy AAddmmiinn ddooeessnn''tt wwoorrkk pprrooppeerrllyy wwiitthhoouutt JJaavvaaSSccrriipptt
 eennaabblleedd.. PPlleeaassee eennaabbllee iitt ttoo ccoonnttiinnuuee..
 {% csrf_token %}
```

### Comparing `django-spaday-0.1.2/src/django_spaday/utils.py` & `django-spaday-0.1.3/src/django_spaday/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,10 +2,12 @@
     """Return permissions for use in a v-combobox."""
     app_label = None
     vue_combobox_list = []
     for p in qs.select_related("content_type"):
         if grouped and app_label != p.content_type.app_label:
             app_label = p.content_type.app_label
             # model_label = p.content_type.model
-            vue_combobox_list.extend(({"header": f"{app_label.title()}"}, {"divider": True}))
+            vue_combobox_list.extend(
+                ({"header": f"{app_label.title()}"}, {"divider": True})
+            )
         vue_combobox_list.append({"value": p.id, "text": p.name})
     return vue_combobox_list
```

### Comparing `django-spaday-0.1.2/src/django_spaday.egg-info/PKG-INFO` & `django-spaday-0.1.3/src/django_spaday.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: django-spaday
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Django package that provides 'out-of-the-box' JWT auth, user, group, and permission APIs for use in Single Page Apps (eg - Vue, React).
 Author-email: Tim Santor <tsantor@xstudios.com>
 Project-URL: homepage, https://github.com/tsantor/django-spaday
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 Requires-Dist: django<5.0,>=4.0
 Requires-Dist: drf-spectacular
 Requires-Dist: django-auditlog
 Requires-Dist: django-celery-results
@@ -134,15 +134,15 @@
 1. `make serve`
 
 - Visit `http://127.0.0.1:8000/djadmin/` for the Django Admin
 - Visit `http://127.0.0.1:8000/api/docs/` for the API docs
 
 ### Testing
 
-Currently django_spaday has **94%** test coverage.
+Currently django_spaday has **95%** test coverage.
 
 - Pytest: `make pytest`
 - Coverage: `make coverage`
   - Open Report: `make open_coverage`
 
 ## Makefile Commands
 
@@ -215,18 +215,21 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.1.3] - 2024-04-02
+- Moved to `ruff` and added tests
+
 ## [0.1.2] - 2024-03-07
 
 - Added missing template example (assumes your Vue project has been built to `project/static/vue-frontend`)
 
 ## [0.1.1] - 2024-03-07
 
-- Added 94% test coverage
+- Added test coverage
 
 ## [0.1.0] - 2022-04-19
 
 - First release on PyPI.
```

### Comparing `django-spaday-0.1.2/src/django_spaday.egg-info/SOURCES.txt` & `django-spaday-0.1.3/src/django_spaday.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 AUTHORS.md
 HISTORY.md
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
-requirements.txt
 setup.py
 src/django_spaday/__init__.py
 src/django_spaday/apps.py
 src/django_spaday/models.py
 src/django_spaday/settings.py
 src/django_spaday/urls.py
 src/django_spaday/utils.py
```

### Comparing `django-spaday-0.1.2/tests/test_api.py` & `django-spaday-0.1.3/tests/test_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pytest
 from django.urls import reverse
 from rest_framework import status
 
 
-@pytest.mark.django_db
+@pytest.mark.django_db()
 class TestLoginView:
     def test_login(self, api_client, user):
         url = reverse("api:rest_login")
         data = {
             "username": user.username,
             "email": user.email,
             "password": "testpass",
@@ -37,17 +37,16 @@
     def test_logout(self, authenticated_client):
         url = reverse("api:rest_logout")
         response = authenticated_client.post(url)
 
         assert response.status_code == status.HTTP_200_OK
 
 
-@pytest.mark.django_db
+@pytest.mark.django_db()
 class TestUserViewSet:
-
     def test_create(self, authenticated_client):
         url = reverse("api:users-list")
         data = {
             "first_name": "New",
             "last_name": "User",
             "username": "newuser",
             "email": "newuser@test.com",
@@ -112,22 +111,24 @@
             "email": user.email,
             "password": "testpass",
         }
         response = api_client.post(url, data)
 
         assert response.status_code == status.HTTP_200_OK
 
-        response = superuser_authenticated_client.get(reverse("api:users-recent-logins"))
+        response = superuser_authenticated_client.get(
+            reverse("api:users-recent-logins")
+        )
         assert response.status_code == status.HTTP_200_OK
         # TODO: Getting empty results as if last_login is not being updated
         # print(response.data)
         # assert len(response.data) >= 1
 
 
-@pytest.mark.django_db
+@pytest.mark.django_db()
 class TestGroupViewSet:
     def test_list(self, authenticated_client, group):
         response = authenticated_client.get(reverse("api:groups-list"))
         assert response.status_code == status.HTTP_200_OK
         assert len(response.data["results"]) == 1
 
     def test_retrieve(self, authenticated_client, group):
@@ -147,49 +148,54 @@
 
     def test_delete(self, authenticated_client, group):
         url = reverse("api:groups-detail", kwargs={"pk": group.pk})
         response = authenticated_client.delete(url)
         assert response.status_code == status.HTTP_204_NO_CONTENT
 
     def test_users(self, authenticated_client, group):
-        response = authenticated_client.get(reverse("api:groups-users", kwargs={"pk": group.pk}))
-        assert response.status_code == 200
+        response = authenticated_client.get(
+            reverse("api:groups-users", kwargs={"pk": group.pk})
+        )
+        assert response.status_code == status.HTTP_200_OK
 
     def test_add_users(self, authenticated_client, user, group):
         data = {"users": [user.pk]}
-        response = authenticated_client.post(reverse("api:groups-add-users", kwargs={"pk": group.pk}), data)
-        assert response.status_code == 200
+        response = authenticated_client.post(
+            reverse("api:groups-add-users", kwargs={"pk": group.pk}), data
+        )
+        assert response.status_code == status.HTTP_200_OK
         assert user.pk in response.data["users"]
 
     def test_remove_users(self, authenticated_client, user, group):
         group.user_set.add(user)
         data = {"users": [user.pk]}
-        response = authenticated_client.post(reverse("api:groups-remove-users", kwargs={"pk": group.pk}), data)
-        assert response.status_code == 200
+        response = authenticated_client.post(
+            reverse("api:groups-remove-users", kwargs={"pk": group.pk}), data
+        )
+        assert response.status_code == status.HTTP_200_OK
         assert user.pk not in response.data["users"]
 
     def test_combobox(self, authenticated_client, group):
         response = authenticated_client.get(reverse("api:groups-combobox"))
         assert response.status_code == status.HTTP_200_OK
         assert len(response.data) == 1
 
 
-@pytest.mark.django_db
+@pytest.mark.django_db()
 class TestPermissionViewSet:
     def test_combobox(self, authenticated_client):
         url = reverse("api:permissions-combobox")
         response = authenticated_client.get(url)
-        assert response.status_code == 200
+        assert response.status_code == status.HTTP_200_OK
         assert isinstance(response.data, list)
         assert len(response.data) >= 1
 
 
-@pytest.mark.django_db
+@pytest.mark.django_db()
 class TestLogEntryViewSet:
-
     def test_list(self, authenticated_client, log_entry):
         url = reverse("api:auditlogs-list")
         response = authenticated_client.get(url)
         assert response.status_code == status.HTTP_200_OK
         assert len(response.data["results"]) >= 1
 
     def test_retrieve(self, authenticated_client, log_entry):
@@ -209,17 +215,16 @@
 
     def test_delete(self, authenticated_client, log_entry):
         url = reverse("api:auditlogs-detail", kwargs={"pk": log_entry.pk})
         response = authenticated_client.delete(url)
         assert response.status_code == status.HTTP_204_NO_CONTENT
 
 
-@pytest.mark.django_db
+@pytest.mark.django_db()
 class TestTaskResultViewSet:
-
     def test_list(self, authenticated_client, task_result):
         url = reverse("api:taskresults-list")
         response = authenticated_client.get(url)
         assert response.status_code == status.HTTP_200_OK
         assert len(response.data["results"]) == 1
 
     def test_retrieve(self, authenticated_client, task_result):
```

### Comparing `django-spaday-0.1.2/tests/test_pagination.py` & `django-spaday-0.1.3/tests/test_pagination.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 import pytest
 from django.urls import reverse
 from rest_framework import status
 
 from tests.factories import UserFactory
 
 
-@pytest.mark.django_db
+@pytest.mark.django_db()
 def test_standard_pagination(authenticated_client):
+    num_results = 10  # Default page size
     UserFactory.create_batch(15)
     response = authenticated_client.get(reverse("api:users-list"))
     assert response.status_code == status.HTTP_200_OK
+    assert "links" in response.data
+    assert "next_page" in response.data
+    assert "previous_page" in response.data
     assert "current_page" in response.data
     assert "num_pages" in response.data
-    assert "start_index" in response.data
-    assert "end_index" in response.data
+    # assert "start_index" in response.data
+    # assert "end_index" in response.data
     assert "num_results" in response.data
     assert "results" in response.data
     # print(response.data)
-    assert len(response.data["results"]) == 10  # Default page size
+    assert len(response.data["results"]) == num_results
```

### Comparing `django-spaday-0.1.2/tests/test_serializers.py` & `django-spaday-0.1.3/tests/test_serializers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 import pytest
+from django_spaday.api.serializers import ChangePasswordSerializer
+from django_spaday.api.serializers import UserAuthSerializer
 
-from django_spaday.api.serializers import ChangePasswordSerializer, UserAuthSerializer
 
-
-@pytest.mark.django_db
+@pytest.mark.django_db()
 def test_user_auth_serializer(user):
     serializer = UserAuthSerializer(user)
     data = serializer.data
 
     assert data["pk"] == user.pk
     assert data["is_active"] == user.is_active
     assert data["is_superuser"] == user.is_superuser
     assert data["is_staff"] == user.is_staff
     assert data["first_name"] == user.first_name
     assert data["last_name"] == user.last_name
     assert data["email"] == user.email
-    assert data["permissions_codenames"] == sorted(list(user.get_all_permissions()))
+    assert data["permissions_codenames"] == sorted(user.get_all_permissions())
     assert data["initials"] == "UU"
-    assert data["full_name"] == "User User"
+    # assert data["full_name"] == "User User"
 
 
-@pytest.mark.django_db
+@pytest.mark.django_db()
 def test_change_password_serializer(user):
     data = {"password": "new_password", "password2": "new_password"}
     serializer = ChangePasswordSerializer(data=data, context={"request": user})
     assert serializer.is_valid()
     validated_data = serializer.validated_data
-    assert validated_data["password"] == "new_password"
+    assert validated_data["password"] == "new_password"  # noqa: S105
     assert validated_data["password2"] == "new_password"
 
     instance = serializer.update(user, validated_data)
     assert instance.check_password("new_password")
 
 
-@pytest.mark.django_db
+@pytest.mark.django_db()
 def test_change_password_serializer_non_matching(user):
     data = {"password": "new_password", "password2": "new_password2"}
     serializer = ChangePasswordSerializer(data=data, context={"request": user})
     assert serializer.is_valid() is False
     assert serializer.errors == {"password": ["Password fields didn't match."]}
```

### Comparing `django-spaday-0.1.2/tests/test_utils.py` & `django-spaday-0.1.3/tests/test_utils.py`

 * *Files identical despite different names*

