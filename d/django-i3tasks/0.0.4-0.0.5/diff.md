# Comparing `tmp/django_i3tasks-0.0.4.tar.gz` & `tmp/django_i3tasks-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_i3tasks-0.0.4.tar", last modified: Tue Apr  2 17:53:59 2024, max compression
+gzip compressed data, was "django_i3tasks-0.0.5.tar", last modified: Tue Apr  2 17:55:51 2024, max compression
```

## Comparing `django_i3tasks-0.0.4.tar` & `django_i3tasks-0.0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 sajlx     (1000) sajlx     (1000)        0 2024-04-02 17:53:59.180427 django_i3tasks-0.0.4/
--rw-rw-r--   0 sajlx     (1000) sajlx     (1000)    35149 2024-04-02 16:20:15.000000 django_i3tasks-0.0.4/LICENSE
--rw-rw-r--   0 sajlx     (1000) sajlx     (1000)     1465 2024-04-02 17:53:59.180427 django_i3tasks-0.0.4/PKG-INFO
--rw-rw-r--   0 sajlx     (1000) sajlx     (1000)      871 2024-04-02 17:49:46.000000 django_i3tasks-0.0.4/README.md
-drwxrwxr-x   0 sajlx     (1000) sajlx     (1000)        0 2024-04-02 17:53:59.180427 django_i3tasks-0.0.4/django_i3tasks/
--rwxrwxrwx   0 sajlx     (1000) sajlx     (1000)        0 2024-04-02 17:03:45.000000 django_i3tasks-0.0.4/django_i3tasks/__init__.py
--rwxrwxrwx   0 sajlx     (1000) sajlx     (1000)      279 2024-04-02 17:03:45.000000 django_i3tasks-0.0.4/django_i3tasks/admin.py
--rwxrwxrwx   0 sajlx     (1000) sajlx     (1000)       96 2024-04-02 17:53:23.000000 django_i3tasks-0.0.4/django_i3tasks/apps.py
--rwxrwxrwx   0 sajlx     (1000) sajlx     (1000)     1111 2024-04-02 17:03:45.000000 django_i3tasks-0.0.4/django_i3tasks/models.py
--rwxrwxrwx   0 sajlx     (1000) sajlx     (1000)      247 2024-04-02 17:03:45.000000 django_i3tasks-0.0.4/django_i3tasks/tasks.py
--rwxrwxrwx   0 sajlx     (1000) sajlx     (1000)       60 2024-04-02 17:03:45.000000 django_i3tasks-0.0.4/django_i3tasks/tests.py
--rwxrwxrwx   0 sajlx     (1000) sajlx     (1000)     1573 2024-04-02 17:03:45.000000 django_i3tasks-0.0.4/django_i3tasks/types.py
--rwxrwxrwx   0 sajlx     (1000) sajlx     (1000)     1427 2024-04-02 17:03:45.000000 django_i3tasks-0.0.4/django_i3tasks/urls.py
--rwxrwxrwx   0 sajlx     (1000) sajlx     (1000)     5518 2024-04-02 17:03:45.000000 django_i3tasks-0.0.4/django_i3tasks/utils.py
--rwxrwxrwx   0 sajlx     (1000) sajlx     (1000)     8239 2024-04-02 17:03:45.000000 django_i3tasks-0.0.4/django_i3tasks/views.py
-drwxrwxr-x   0 sajlx     (1000) sajlx     (1000)        0 2024-04-02 17:53:59.180427 django_i3tasks-0.0.4/django_i3tasks.egg-info/
--rw-rw-r--   0 sajlx     (1000) sajlx     (1000)     1465 2024-04-02 17:53:59.000000 django_i3tasks-0.0.4/django_i3tasks.egg-info/PKG-INFO
--rw-rw-r--   0 sajlx     (1000) sajlx     (1000)      494 2024-04-02 17:53:59.000000 django_i3tasks-0.0.4/django_i3tasks.egg-info/SOURCES.txt
--rw-rw-r--   0 sajlx     (1000) sajlx     (1000)        1 2024-04-02 17:53:59.000000 django_i3tasks-0.0.4/django_i3tasks.egg-info/dependency_links.txt
--rw-rw-r--   0 sajlx     (1000) sajlx     (1000)        1 2024-04-02 17:53:59.000000 django_i3tasks-0.0.4/django_i3tasks.egg-info/not-zip-safe
--rw-rw-r--   0 sajlx     (1000) sajlx     (1000)       52 2024-04-02 17:53:59.000000 django_i3tasks-0.0.4/django_i3tasks.egg-info/requires.txt
--rw-rw-r--   0 sajlx     (1000) sajlx     (1000)       15 2024-04-02 17:53:59.000000 django_i3tasks-0.0.4/django_i3tasks.egg-info/top_level.txt
--rw-rw-r--   0 sajlx     (1000) sajlx     (1000)       38 2024-04-02 17:53:59.180427 django_i3tasks-0.0.4/setup.cfg
--rw-rw-r--   0 sajlx     (1000) sajlx     (1000)     1048 2024-04-02 17:53:50.000000 django_i3tasks-0.0.4/setup.py
+drwxrwxr-x   0 sajlx     (1000) sajlx     (1000)        0 2024-04-02 17:55:51.080953 django_i3tasks-0.0.5/
+-rw-rw-r--   0 sajlx     (1000) sajlx     (1000)    35149 2024-04-02 16:20:15.000000 django_i3tasks-0.0.5/LICENSE
+-rw-rw-r--   0 sajlx     (1000) sajlx     (1000)     1465 2024-04-02 17:55:51.080953 django_i3tasks-0.0.5/PKG-INFO
+-rw-rw-r--   0 sajlx     (1000) sajlx     (1000)      871 2024-04-02 17:49:46.000000 django_i3tasks-0.0.5/README.md
+drwxrwxr-x   0 sajlx     (1000) sajlx     (1000)        0 2024-04-02 17:55:51.080953 django_i3tasks-0.0.5/django_i3tasks/
+-rwxrwxrwx   0 sajlx     (1000) sajlx     (1000)        0 2024-04-02 17:03:45.000000 django_i3tasks-0.0.5/django_i3tasks/__init__.py
+-rwxrwxrwx   0 sajlx     (1000) sajlx     (1000)      279 2024-04-02 17:03:45.000000 django_i3tasks-0.0.5/django_i3tasks/admin.py
+-rwxrwxrwx   0 sajlx     (1000) sajlx     (1000)       96 2024-04-02 17:53:23.000000 django_i3tasks-0.0.5/django_i3tasks/apps.py
+-rwxrwxrwx   0 sajlx     (1000) sajlx     (1000)     1111 2024-04-02 17:03:45.000000 django_i3tasks-0.0.5/django_i3tasks/models.py
+-rwxrwxrwx   0 sajlx     (1000) sajlx     (1000)      247 2024-04-02 17:03:45.000000 django_i3tasks-0.0.5/django_i3tasks/tasks.py
+-rwxrwxrwx   0 sajlx     (1000) sajlx     (1000)       60 2024-04-02 17:03:45.000000 django_i3tasks-0.0.5/django_i3tasks/tests.py
+-rwxrwxrwx   0 sajlx     (1000) sajlx     (1000)     1573 2024-04-02 17:03:45.000000 django_i3tasks-0.0.5/django_i3tasks/types.py
+-rwxrwxrwx   0 sajlx     (1000) sajlx     (1000)     1427 2024-04-02 17:03:45.000000 django_i3tasks-0.0.5/django_i3tasks/urls.py
+-rwxrwxrwx   0 sajlx     (1000) sajlx     (1000)     5518 2024-04-02 17:03:45.000000 django_i3tasks-0.0.5/django_i3tasks/utils.py
+-rwxrwxrwx   0 sajlx     (1000) sajlx     (1000)     8239 2024-04-02 17:03:45.000000 django_i3tasks-0.0.5/django_i3tasks/views.py
+drwxrwxr-x   0 sajlx     (1000) sajlx     (1000)        0 2024-04-02 17:55:51.080953 django_i3tasks-0.0.5/django_i3tasks.egg-info/
+-rw-rw-r--   0 sajlx     (1000) sajlx     (1000)     1465 2024-04-02 17:55:51.000000 django_i3tasks-0.0.5/django_i3tasks.egg-info/PKG-INFO
+-rw-rw-r--   0 sajlx     (1000) sajlx     (1000)      494 2024-04-02 17:55:51.000000 django_i3tasks-0.0.5/django_i3tasks.egg-info/SOURCES.txt
+-rw-rw-r--   0 sajlx     (1000) sajlx     (1000)        1 2024-04-02 17:55:51.000000 django_i3tasks-0.0.5/django_i3tasks.egg-info/dependency_links.txt
+-rw-rw-r--   0 sajlx     (1000) sajlx     (1000)        1 2024-04-02 17:55:51.000000 django_i3tasks-0.0.5/django_i3tasks.egg-info/not-zip-safe
+-rw-rw-r--   0 sajlx     (1000) sajlx     (1000)       52 2024-04-02 17:55:51.000000 django_i3tasks-0.0.5/django_i3tasks.egg-info/requires.txt
+-rw-rw-r--   0 sajlx     (1000) sajlx     (1000)       15 2024-04-02 17:55:51.000000 django_i3tasks-0.0.5/django_i3tasks.egg-info/top_level.txt
+-rw-rw-r--   0 sajlx     (1000) sajlx     (1000)       38 2024-04-02 17:55:51.080953 django_i3tasks-0.0.5/setup.cfg
+-rw-rw-r--   0 sajlx     (1000) sajlx     (1000)     1048 2024-04-02 17:55:47.000000 django_i3tasks-0.0.5/setup.py
```

### Comparing `django_i3tasks-0.0.4/LICENSE` & `django_i3tasks-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django_i3tasks-0.0.4/PKG-INFO` & `django_i3tasks-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_i3tasks
-Version: 0.0.4
+Version: 0.0.5
 Summary: Django app for manage async tasks by http requests
 Home-page: https://github.com/sajlx/django-i3tasks
 Author: Ivan Bettarini
 Author-email: ivan.bettarini@gmail.com
 License: GNU General Public License v3.0
 Classifier: Environment :: Web Environment
 Classifier: Operating System :: OS Independent
```

### Comparing `django_i3tasks-0.0.4/README.md` & `django_i3tasks-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `django_i3tasks-0.0.4/django_i3tasks/models.py` & `django_i3tasks-0.0.5/django_i3tasks/models.py`

 * *Files identical despite different names*

### Comparing `django_i3tasks-0.0.4/django_i3tasks/types.py` & `django_i3tasks-0.0.5/django_i3tasks/types.py`

 * *Files identical despite different names*

### Comparing `django_i3tasks-0.0.4/django_i3tasks/urls.py` & `django_i3tasks-0.0.5/django_i3tasks/urls.py`

 * *Files identical despite different names*

### Comparing `django_i3tasks-0.0.4/django_i3tasks/utils.py` & `django_i3tasks-0.0.5/django_i3tasks/utils.py`

 * *Files identical despite different names*

### Comparing `django_i3tasks-0.0.4/django_i3tasks/views.py` & `django_i3tasks-0.0.5/django_i3tasks/views.py`

 * *Files identical despite different names*

### Comparing `django_i3tasks-0.0.4/django_i3tasks.egg-info/PKG-INFO` & `django_i3tasks-0.0.5/django_i3tasks.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-i3tasks
-Version: 0.0.4
+Version: 0.0.5
 Summary: Django app for manage async tasks by http requests
 Home-page: https://github.com/sajlx/django-i3tasks
 Author: Ivan Bettarini
 Author-email: ivan.bettarini@gmail.com
 License: GNU General Public License v3.0
 Classifier: Environment :: Web Environment
 Classifier: Operating System :: OS Independent
```

### Comparing `django_i3tasks-0.0.4/setup.py` & `django_i3tasks-0.0.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='django_i3tasks',
-    version='0.0.4',
+    version='0.0.5',
     description='Django app for manage async tasks by http requests',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/sajlx/django-i3tasks',
     author='Ivan Bettarini',
     author_email='ivan.bettarini@gmail.com',
     license='GNU General Public License v3.0',
```

