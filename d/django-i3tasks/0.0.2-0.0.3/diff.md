# Comparing `tmp/django_i3tasks-0.0.2.tar.gz` & `tmp/django_i3tasks-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_i3tasks-0.0.2.tar", last modified: Tue Apr  2 17:16:41 2024, max compression
+gzip compressed data, was "django_i3tasks-0.0.3.tar", last modified: Tue Apr  2 17:30:00 2024, max compression
```

## Comparing `django_i3tasks-0.0.2.tar` & `django_i3tasks-0.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 sajlx     (1000) sajlx     (1000)        0 2024-04-02 17:16:41.215823 django_i3tasks-0.0.2/
--rw-rw-r--   0 sajlx     (1000) sajlx     (1000)    35149 2024-04-02 16:20:15.000000 django_i3tasks-0.0.2/LICENSE
--rw-rw-r--   0 sajlx     (1000) sajlx     (1000)      346 2024-04-02 17:16:41.215823 django_i3tasks-0.0.2/PKG-INFO
--rw-rw-r--   0 sajlx     (1000) sajlx     (1000)       16 2024-04-02 16:20:15.000000 django_i3tasks-0.0.2/README.md
-drwxrwxr-x   0 sajlx     (1000) sajlx     (1000)        0 2024-04-02 17:16:41.215823 django_i3tasks-0.0.2/django_i3tasks/
--rwxrwxrwx   0 sajlx     (1000) sajlx     (1000)        0 2024-04-02 17:03:45.000000 django_i3tasks-0.0.2/django_i3tasks/__init__.py
--rwxrwxrwx   0 sajlx     (1000) sajlx     (1000)      279 2024-04-02 17:03:45.000000 django_i3tasks-0.0.2/django_i3tasks/admin.py
--rwxrwxrwx   0 sajlx     (1000) sajlx     (1000)       89 2024-04-02 17:03:45.000000 django_i3tasks-0.0.2/django_i3tasks/apps.py
--rwxrwxrwx   0 sajlx     (1000) sajlx     (1000)     1111 2024-04-02 17:03:45.000000 django_i3tasks-0.0.2/django_i3tasks/models.py
--rwxrwxrwx   0 sajlx     (1000) sajlx     (1000)      247 2024-04-02 17:03:45.000000 django_i3tasks-0.0.2/django_i3tasks/tasks.py
--rwxrwxrwx   0 sajlx     (1000) sajlx     (1000)       60 2024-04-02 17:03:45.000000 django_i3tasks-0.0.2/django_i3tasks/tests.py
--rwxrwxrwx   0 sajlx     (1000) sajlx     (1000)     1573 2024-04-02 17:03:45.000000 django_i3tasks-0.0.2/django_i3tasks/types.py
--rwxrwxrwx   0 sajlx     (1000) sajlx     (1000)     1427 2024-04-02 17:03:45.000000 django_i3tasks-0.0.2/django_i3tasks/urls.py
--rwxrwxrwx   0 sajlx     (1000) sajlx     (1000)     5518 2024-04-02 17:03:45.000000 django_i3tasks-0.0.2/django_i3tasks/utils.py
--rwxrwxrwx   0 sajlx     (1000) sajlx     (1000)     8239 2024-04-02 17:03:45.000000 django_i3tasks-0.0.2/django_i3tasks/views.py
-drwxrwxr-x   0 sajlx     (1000) sajlx     (1000)        0 2024-04-02 17:16:41.215823 django_i3tasks-0.0.2/django_i3tasks.egg-info/
--rw-rw-r--   0 sajlx     (1000) sajlx     (1000)      346 2024-04-02 17:16:41.000000 django_i3tasks-0.0.2/django_i3tasks.egg-info/PKG-INFO
--rw-rw-r--   0 sajlx     (1000) sajlx     (1000)      494 2024-04-02 17:16:41.000000 django_i3tasks-0.0.2/django_i3tasks.egg-info/SOURCES.txt
--rw-rw-r--   0 sajlx     (1000) sajlx     (1000)        1 2024-04-02 17:16:41.000000 django_i3tasks-0.0.2/django_i3tasks.egg-info/dependency_links.txt
--rw-rw-r--   0 sajlx     (1000) sajlx     (1000)        1 2024-04-02 17:16:41.000000 django_i3tasks-0.0.2/django_i3tasks.egg-info/not-zip-safe
--rw-rw-r--   0 sajlx     (1000) sajlx     (1000)       36 2024-04-02 17:16:41.000000 django_i3tasks-0.0.2/django_i3tasks.egg-info/requires.txt
--rw-rw-r--   0 sajlx     (1000) sajlx     (1000)       15 2024-04-02 17:16:41.000000 django_i3tasks-0.0.2/django_i3tasks.egg-info/top_level.txt
--rw-rw-r--   0 sajlx     (1000) sajlx     (1000)       38 2024-04-02 17:16:41.215823 django_i3tasks-0.0.2/setup.cfg
--rw-rw-r--   0 sajlx     (1000) sajlx     (1000)      604 2024-04-02 17:15:56.000000 django_i3tasks-0.0.2/setup.py
+drwxrwxr-x   0 sajlx     (1000) sajlx     (1000)        0 2024-04-02 17:30:00.063122 django_i3tasks-0.0.3/
+-rw-rw-r--   0 sajlx     (1000) sajlx     (1000)    35149 2024-04-02 16:20:15.000000 django_i3tasks-0.0.3/LICENSE
+-rw-rw-r--   0 sajlx     (1000) sajlx     (1000)      448 2024-04-02 17:30:00.063122 django_i3tasks-0.0.3/PKG-INFO
+-rw-rw-r--   0 sajlx     (1000) sajlx     (1000)      113 2024-04-02 17:23:11.000000 django_i3tasks-0.0.3/README.md
+drwxrwxr-x   0 sajlx     (1000) sajlx     (1000)        0 2024-04-02 17:30:00.063122 django_i3tasks-0.0.3/django_i3tasks/
+-rwxrwxrwx   0 sajlx     (1000) sajlx     (1000)        0 2024-04-02 17:03:45.000000 django_i3tasks-0.0.3/django_i3tasks/__init__.py
+-rwxrwxrwx   0 sajlx     (1000) sajlx     (1000)      279 2024-04-02 17:03:45.000000 django_i3tasks-0.0.3/django_i3tasks/admin.py
+-rwxrwxrwx   0 sajlx     (1000) sajlx     (1000)       89 2024-04-02 17:03:45.000000 django_i3tasks-0.0.3/django_i3tasks/apps.py
+-rwxrwxrwx   0 sajlx     (1000) sajlx     (1000)     1111 2024-04-02 17:03:45.000000 django_i3tasks-0.0.3/django_i3tasks/models.py
+-rwxrwxrwx   0 sajlx     (1000) sajlx     (1000)      247 2024-04-02 17:03:45.000000 django_i3tasks-0.0.3/django_i3tasks/tasks.py
+-rwxrwxrwx   0 sajlx     (1000) sajlx     (1000)       60 2024-04-02 17:03:45.000000 django_i3tasks-0.0.3/django_i3tasks/tests.py
+-rwxrwxrwx   0 sajlx     (1000) sajlx     (1000)     1573 2024-04-02 17:03:45.000000 django_i3tasks-0.0.3/django_i3tasks/types.py
+-rwxrwxrwx   0 sajlx     (1000) sajlx     (1000)     1427 2024-04-02 17:03:45.000000 django_i3tasks-0.0.3/django_i3tasks/urls.py
+-rwxrwxrwx   0 sajlx     (1000) sajlx     (1000)     5518 2024-04-02 17:03:45.000000 django_i3tasks-0.0.3/django_i3tasks/utils.py
+-rwxrwxrwx   0 sajlx     (1000) sajlx     (1000)     8239 2024-04-02 17:03:45.000000 django_i3tasks-0.0.3/django_i3tasks/views.py
+drwxrwxr-x   0 sajlx     (1000) sajlx     (1000)        0 2024-04-02 17:30:00.063122 django_i3tasks-0.0.3/django_i3tasks.egg-info/
+-rw-rw-r--   0 sajlx     (1000) sajlx     (1000)      448 2024-04-02 17:30:00.000000 django_i3tasks-0.0.3/django_i3tasks.egg-info/PKG-INFO
+-rw-rw-r--   0 sajlx     (1000) sajlx     (1000)      494 2024-04-02 17:30:00.000000 django_i3tasks-0.0.3/django_i3tasks.egg-info/SOURCES.txt
+-rw-rw-r--   0 sajlx     (1000) sajlx     (1000)        1 2024-04-02 17:30:00.000000 django_i3tasks-0.0.3/django_i3tasks.egg-info/dependency_links.txt
+-rw-rw-r--   0 sajlx     (1000) sajlx     (1000)        1 2024-04-02 17:30:00.000000 django_i3tasks-0.0.3/django_i3tasks.egg-info/not-zip-safe
+-rw-rw-r--   0 sajlx     (1000) sajlx     (1000)       52 2024-04-02 17:30:00.000000 django_i3tasks-0.0.3/django_i3tasks.egg-info/requires.txt
+-rw-rw-r--   0 sajlx     (1000) sajlx     (1000)       15 2024-04-02 17:30:00.000000 django_i3tasks-0.0.3/django_i3tasks.egg-info/top_level.txt
+-rw-rw-r--   0 sajlx     (1000) sajlx     (1000)       38 2024-04-02 17:30:00.063122 django_i3tasks-0.0.3/setup.cfg
+-rw-rw-r--   0 sajlx     (1000) sajlx     (1000)      773 2024-04-02 17:28:56.000000 django_i3tasks-0.0.3/setup.py
```

### Comparing `django_i3tasks-0.0.2/LICENSE` & `django_i3tasks-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django_i3tasks-0.0.2/django_i3tasks/models.py` & `django_i3tasks-0.0.3/django_i3tasks/models.py`

 * *Files identical despite different names*

### Comparing `django_i3tasks-0.0.2/django_i3tasks/types.py` & `django_i3tasks-0.0.3/django_i3tasks/types.py`

 * *Files identical despite different names*

### Comparing `django_i3tasks-0.0.2/django_i3tasks/urls.py` & `django_i3tasks-0.0.3/django_i3tasks/urls.py`

 * *Files identical despite different names*

### Comparing `django_i3tasks-0.0.2/django_i3tasks/utils.py` & `django_i3tasks-0.0.3/django_i3tasks/utils.py`

 * *Files identical despite different names*

### Comparing `django_i3tasks-0.0.2/django_i3tasks/views.py` & `django_i3tasks-0.0.3/django_i3tasks/views.py`

 * *Files identical despite different names*

