# Comparing `tmp/django-dbbackup-admin-1.2.0.tar.gz` & `tmp/django-dbbackup-admin-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-dbbackup-admin-1.2.0.tar", last modified: Thu Jan 11 14:57:02 2024, max compression
+gzip compressed data, was "django-dbbackup-admin-1.3.0.tar", last modified: Tue Apr  2 07:02:21 2024, max compression
```

## Comparing `django-dbbackup-admin-1.2.0.tar` & `django-dbbackup-admin-1.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0 hossein   (1000) hossein   (1000)        0 2024-01-11 14:57:02.875875 django-dbbackup-admin-1.2.0/
--rwxrwxrwx   0 hossein   (1000) hossein   (1000)     1097 2023-10-26 06:11:34.000000 django-dbbackup-admin-1.2.0/LICENSE
--rwxrwxrwx   0 hossein   (1000) hossein   (1000)     2694 2024-01-11 14:57:02.874920 django-dbbackup-admin-1.2.0/PKG-INFO
--rwxrwxrwx   0 hossein   (1000) hossein   (1000)     1354 2024-01-11 14:30:06.000000 django-dbbackup-admin-1.2.0/README.md
-drwxrwxrwx   0 hossein   (1000) hossein   (1000)        0 2024-01-11 14:57:02.866782 django-dbbackup-admin-1.2.0/dbbackup_admin/
--rwxrwxrwx   0 hossein   (1000) hossein   (1000)        0 2023-10-15 06:18:19.000000 django-dbbackup-admin-1.2.0/dbbackup_admin/__init__.py
--rwxrwxrwx   0 hossein   (1000) hossein   (1000)      238 2023-10-26 09:58:00.000000 django-dbbackup-admin-1.2.0/dbbackup_admin/admin.py
--rwxrwxrwx   0 hossein   (1000) hossein   (1000)      158 2023-10-26 13:58:08.000000 django-dbbackup-admin-1.2.0/dbbackup_admin/apps.py
--rwxrwxrwx   0 hossein   (1000) hossein   (1000)     1107 2024-01-11 14:21:21.000000 django-dbbackup-admin-1.2.0/dbbackup_admin/models.py
--rwxrwxrwx   0 hossein   (1000) hossein   (1000)       65 2023-10-26 06:20:44.000000 django-dbbackup-admin-1.2.0/dbbackup_admin/urls.py
--rwxrwxrwx   0 hossein   (1000) hossein   (1000)        0 2023-10-26 06:20:59.000000 django-dbbackup-admin-1.2.0/dbbackup_admin/views.py
-drwxrwxrwx   0 hossein   (1000) hossein   (1000)        0 2024-01-11 14:57:02.873725 django-dbbackup-admin-1.2.0/django_dbbackup_admin.egg-info/
--rwxrwxrwx   0 hossein   (1000) hossein   (1000)     2694 2024-01-11 14:57:02.000000 django-dbbackup-admin-1.2.0/django_dbbackup_admin.egg-info/PKG-INFO
--rwxrwxrwx   0 hossein   (1000) hossein   (1000)      396 2024-01-11 14:57:02.000000 django-dbbackup-admin-1.2.0/django_dbbackup_admin.egg-info/SOURCES.txt
--rwxrwxrwx   0 hossein   (1000) hossein   (1000)        1 2024-01-11 14:57:02.000000 django-dbbackup-admin-1.2.0/django_dbbackup_admin.egg-info/dependency_links.txt
--rwxrwxrwx   0 hossein   (1000) hossein   (1000)       42 2024-01-11 14:57:02.000000 django-dbbackup-admin-1.2.0/django_dbbackup_admin.egg-info/requires.txt
--rwxrwxrwx   0 hossein   (1000) hossein   (1000)       15 2024-01-11 14:57:02.000000 django-dbbackup-admin-1.2.0/django_dbbackup_admin.egg-info/top_level.txt
--rwxrwxrwx   0 hossein   (1000) hossein   (1000)       38 2024-01-11 14:57:02.876067 django-dbbackup-admin-1.2.0/setup.cfg
--rwxrwxrwx   0 hossein   (1000) hossein   (1000)     1887 2024-01-11 14:35:44.000000 django-dbbackup-admin-1.2.0/setup.py
+drwxrwxrwx   0 hossein   (1000) hossein   (1000)        0 2024-04-02 07:02:21.558426 django-dbbackup-admin-1.3.0/
+-rwxrwxrwx   0 hossein   (1000) hossein   (1000)     1097 2023-10-26 06:11:34.000000 django-dbbackup-admin-1.3.0/LICENSE
+-rwxrwxrwx   0 hossein   (1000) hossein   (1000)     2694 2024-04-02 07:02:21.557365 django-dbbackup-admin-1.3.0/PKG-INFO
+-rwxrwxrwx   0 hossein   (1000) hossein   (1000)     1354 2024-01-11 14:30:06.000000 django-dbbackup-admin-1.3.0/README.md
+drwxrwxrwx   0 hossein   (1000) hossein   (1000)        0 2024-04-02 07:02:21.549498 django-dbbackup-admin-1.3.0/dbbackup_admin/
+-rwxrwxrwx   0 hossein   (1000) hossein   (1000)        0 2023-10-15 06:18:19.000000 django-dbbackup-admin-1.3.0/dbbackup_admin/__init__.py
+-rwxrwxrwx   0 hossein   (1000) hossein   (1000)      238 2023-10-26 09:58:00.000000 django-dbbackup-admin-1.3.0/dbbackup_admin/admin.py
+-rwxrwxrwx   0 hossein   (1000) hossein   (1000)      158 2023-10-26 13:58:08.000000 django-dbbackup-admin-1.3.0/dbbackup_admin/apps.py
+-rwxrwxrwx   0 hossein   (1000) hossein   (1000)     1107 2024-01-11 14:21:21.000000 django-dbbackup-admin-1.3.0/dbbackup_admin/models.py
+-rwxrwxrwx   0 hossein   (1000) hossein   (1000)       65 2023-10-26 06:20:44.000000 django-dbbackup-admin-1.3.0/dbbackup_admin/urls.py
+-rwxrwxrwx   0 hossein   (1000) hossein   (1000)        0 2023-10-26 06:20:59.000000 django-dbbackup-admin-1.3.0/dbbackup_admin/views.py
+drwxrwxrwx   0 hossein   (1000) hossein   (1000)        0 2024-04-02 07:02:21.556143 django-dbbackup-admin-1.3.0/django_dbbackup_admin.egg-info/
+-rwxrwxrwx   0 hossein   (1000) hossein   (1000)     2694 2024-04-02 07:02:21.000000 django-dbbackup-admin-1.3.0/django_dbbackup_admin.egg-info/PKG-INFO
+-rwxrwxrwx   0 hossein   (1000) hossein   (1000)      396 2024-04-02 07:02:21.000000 django-dbbackup-admin-1.3.0/django_dbbackup_admin.egg-info/SOURCES.txt
+-rwxrwxrwx   0 hossein   (1000) hossein   (1000)        1 2024-04-02 07:02:21.000000 django-dbbackup-admin-1.3.0/django_dbbackup_admin.egg-info/dependency_links.txt
+-rwxrwxrwx   0 hossein   (1000) hossein   (1000)       42 2024-04-02 07:02:21.000000 django-dbbackup-admin-1.3.0/django_dbbackup_admin.egg-info/requires.txt
+-rwxrwxrwx   0 hossein   (1000) hossein   (1000)       15 2024-04-02 07:02:21.000000 django-dbbackup-admin-1.3.0/django_dbbackup_admin.egg-info/top_level.txt
+-rwxrwxrwx   0 hossein   (1000) hossein   (1000)       38 2024-04-02 07:02:21.558673 django-dbbackup-admin-1.3.0/setup.cfg
+-rwxrwxrwx   0 hossein   (1000) hossein   (1000)     1887 2024-04-02 07:00:33.000000 django-dbbackup-admin-1.3.0/setup.py
```

### Comparing `django-dbbackup-admin-1.2.0/LICENSE` & `django-dbbackup-admin-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-dbbackup-admin-1.2.0/PKG-INFO` & `django-dbbackup-admin-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-dbbackup-admin
-Version: 1.2.0
+Version: 1.3.0
 Summary: Get Backup From Database Through Admin Panel
 Home-page: https://github.com/HosseinSayyedMousavi
 Author: Hossein Sayyedmousavi
 Author-email: Hossein.Sayyedmousavi@gmail.com
 Keywords: django,database,media,backup,amazon,s3,dropbox
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `django-dbbackup-admin-1.2.0/README.md` & `django-dbbackup-admin-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `django-dbbackup-admin-1.2.0/dbbackup_admin/models.py` & `django-dbbackup-admin-1.3.0/dbbackup_admin/models.py`

 * *Files identical despite different names*

### Comparing `django-dbbackup-admin-1.2.0/django_dbbackup_admin.egg-info/PKG-INFO` & `django-dbbackup-admin-1.3.0/django_dbbackup_admin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-dbbackup-admin
-Version: 1.2.0
+Version: 1.3.0
 Summary: Get Backup From Database Through Admin Panel
 Home-page: https://github.com/HosseinSayyedMousavi
 Author: Hossein Sayyedmousavi
 Author-email: Hossein.Sayyedmousavi@gmail.com
 Keywords: django,database,media,backup,amazon,s3,dropbox
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `django-dbbackup-admin-1.2.0/setup.py` & `django-dbbackup-admin-1.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 try:
     import pypandoc
     long_description = pypandoc.convert_file('README.md', 'rst')
 except(IOError, ImportError):
     long_description = open('README.md').read()
 setup(
     name='django-dbbackup-admin',
-    version='1.2.0',
+    version='1.3.0',
     description='Get Backup From Database Through Admin Panel',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Hossein Sayyedmousavi',
     author_email='Hossein.Sayyedmousavi@gmail.com',
     packages=['dbbackup_admin'],
     install_requires=[
```

