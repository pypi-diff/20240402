# Comparing `tmp/django_i3tasks-0.0.6.tar.gz` & `tmp/django_i3tasks-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_i3tasks-0.0.6.tar", last modified: Tue Apr  2 18:05:14 2024, max compression
+gzip compressed data, was "django_i3tasks-0.0.7.tar", last modified: Tue Apr  2 18:09:07 2024, max compression
```

## Comparing `django_i3tasks-0.0.6.tar` & `django_i3tasks-0.0.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 sajlx     (1000) sajlx     (1000)        0 2024-04-02 18:05:14.495578 django_i3tasks-0.0.6/
--rw-rw-r--   0 sajlx     (1000) sajlx     (1000)    35149 2024-04-02 16:20:15.000000 django_i3tasks-0.0.6/LICENSE
--rw-rw-r--   0 sajlx     (1000) sajlx     (1000)     1465 2024-04-02 18:05:14.491578 django_i3tasks-0.0.6/PKG-INFO
--rw-rw-r--   0 sajlx     (1000) sajlx     (1000)      871 2024-04-02 17:49:46.000000 django_i3tasks-0.0.6/README.md
-drwxrwxr-x   0 sajlx     (1000) sajlx     (1000)        0 2024-04-02 18:05:14.491578 django_i3tasks-0.0.6/django_i3tasks/
--rwxrwxrwx   0 sajlx     (1000) sajlx     (1000)        0 2024-04-02 17:03:45.000000 django_i3tasks-0.0.6/django_i3tasks/__init__.py
--rwxrwxrwx   0 sajlx     (1000) sajlx     (1000)      279 2024-04-02 17:03:45.000000 django_i3tasks-0.0.6/django_i3tasks/admin.py
--rwxrwxrwx   0 sajlx     (1000) sajlx     (1000)      175 2024-04-02 18:03:36.000000 django_i3tasks-0.0.6/django_i3tasks/apps.py
--rwxrwxrwx   0 sajlx     (1000) sajlx     (1000)     1111 2024-04-02 17:03:45.000000 django_i3tasks-0.0.6/django_i3tasks/models.py
--rwxrwxrwx   0 sajlx     (1000) sajlx     (1000)      247 2024-04-02 17:03:45.000000 django_i3tasks-0.0.6/django_i3tasks/tasks.py
--rwxrwxrwx   0 sajlx     (1000) sajlx     (1000)       60 2024-04-02 17:03:45.000000 django_i3tasks-0.0.6/django_i3tasks/tests.py
--rwxrwxrwx   0 sajlx     (1000) sajlx     (1000)     1573 2024-04-02 17:03:45.000000 django_i3tasks-0.0.6/django_i3tasks/types.py
--rwxrwxrwx   0 sajlx     (1000) sajlx     (1000)     1427 2024-04-02 17:03:45.000000 django_i3tasks-0.0.6/django_i3tasks/urls.py
--rwxrwxrwx   0 sajlx     (1000) sajlx     (1000)     5518 2024-04-02 17:03:45.000000 django_i3tasks-0.0.6/django_i3tasks/utils.py
--rwxrwxrwx   0 sajlx     (1000) sajlx     (1000)     8239 2024-04-02 17:03:45.000000 django_i3tasks-0.0.6/django_i3tasks/views.py
-drwxrwxr-x   0 sajlx     (1000) sajlx     (1000)        0 2024-04-02 18:05:14.491578 django_i3tasks-0.0.6/django_i3tasks.egg-info/
--rw-rw-r--   0 sajlx     (1000) sajlx     (1000)     1465 2024-04-02 18:05:14.000000 django_i3tasks-0.0.6/django_i3tasks.egg-info/PKG-INFO
--rw-rw-r--   0 sajlx     (1000) sajlx     (1000)      494 2024-04-02 18:05:14.000000 django_i3tasks-0.0.6/django_i3tasks.egg-info/SOURCES.txt
--rw-rw-r--   0 sajlx     (1000) sajlx     (1000)        1 2024-04-02 18:05:14.000000 django_i3tasks-0.0.6/django_i3tasks.egg-info/dependency_links.txt
--rw-rw-r--   0 sajlx     (1000) sajlx     (1000)        1 2024-04-02 18:05:14.000000 django_i3tasks-0.0.6/django_i3tasks.egg-info/not-zip-safe
--rw-rw-r--   0 sajlx     (1000) sajlx     (1000)       52 2024-04-02 18:05:14.000000 django_i3tasks-0.0.6/django_i3tasks.egg-info/requires.txt
--rw-rw-r--   0 sajlx     (1000) sajlx     (1000)       15 2024-04-02 18:05:14.000000 django_i3tasks-0.0.6/django_i3tasks.egg-info/top_level.txt
--rw-rw-r--   0 sajlx     (1000) sajlx     (1000)       38 2024-04-02 18:05:14.495578 django_i3tasks-0.0.6/setup.cfg
--rw-rw-r--   0 sajlx     (1000) sajlx     (1000)     1048 2024-04-02 18:05:06.000000 django_i3tasks-0.0.6/setup.py
+drwxrwxr-x   0 sajlx     (1000) sajlx     (1000)        0 2024-04-02 18:09:07.779171 django_i3tasks-0.0.7/
+-rw-rw-r--   0 sajlx     (1000) sajlx     (1000)    35149 2024-04-02 16:20:15.000000 django_i3tasks-0.0.7/LICENSE
+-rw-rw-r--   0 sajlx     (1000) sajlx     (1000)     1498 2024-04-02 18:09:07.779171 django_i3tasks-0.0.7/PKG-INFO
+-rw-rw-r--   0 sajlx     (1000) sajlx     (1000)      904 2024-04-02 18:08:05.000000 django_i3tasks-0.0.7/README.md
+drwxrwxr-x   0 sajlx     (1000) sajlx     (1000)        0 2024-04-02 18:09:07.779171 django_i3tasks-0.0.7/django_i3tasks/
+-rwxrwxrwx   0 sajlx     (1000) sajlx     (1000)        0 2024-04-02 17:03:45.000000 django_i3tasks-0.0.7/django_i3tasks/__init__.py
+-rwxrwxrwx   0 sajlx     (1000) sajlx     (1000)      279 2024-04-02 17:03:45.000000 django_i3tasks-0.0.7/django_i3tasks/admin.py
+-rwxrwxrwx   0 sajlx     (1000) sajlx     (1000)      175 2024-04-02 18:03:36.000000 django_i3tasks-0.0.7/django_i3tasks/apps.py
+-rwxrwxrwx   0 sajlx     (1000) sajlx     (1000)     1111 2024-04-02 17:03:45.000000 django_i3tasks-0.0.7/django_i3tasks/models.py
+-rwxrwxrwx   0 sajlx     (1000) sajlx     (1000)      247 2024-04-02 17:03:45.000000 django_i3tasks-0.0.7/django_i3tasks/tasks.py
+-rwxrwxrwx   0 sajlx     (1000) sajlx     (1000)       60 2024-04-02 17:03:45.000000 django_i3tasks-0.0.7/django_i3tasks/tests.py
+-rwxrwxrwx   0 sajlx     (1000) sajlx     (1000)     1573 2024-04-02 17:03:45.000000 django_i3tasks-0.0.7/django_i3tasks/types.py
+-rwxrwxrwx   0 sajlx     (1000) sajlx     (1000)     1427 2024-04-02 17:03:45.000000 django_i3tasks-0.0.7/django_i3tasks/urls.py
+-rwxrwxrwx   0 sajlx     (1000) sajlx     (1000)     5525 2024-04-02 18:08:47.000000 django_i3tasks-0.0.7/django_i3tasks/utils.py
+-rwxrwxrwx   0 sajlx     (1000) sajlx     (1000)     8246 2024-04-02 18:08:46.000000 django_i3tasks-0.0.7/django_i3tasks/views.py
+drwxrwxr-x   0 sajlx     (1000) sajlx     (1000)        0 2024-04-02 18:09:07.779171 django_i3tasks-0.0.7/django_i3tasks.egg-info/
+-rw-rw-r--   0 sajlx     (1000) sajlx     (1000)     1498 2024-04-02 18:09:07.000000 django_i3tasks-0.0.7/django_i3tasks.egg-info/PKG-INFO
+-rw-rw-r--   0 sajlx     (1000) sajlx     (1000)      494 2024-04-02 18:09:07.000000 django_i3tasks-0.0.7/django_i3tasks.egg-info/SOURCES.txt
+-rw-rw-r--   0 sajlx     (1000) sajlx     (1000)        1 2024-04-02 18:09:07.000000 django_i3tasks-0.0.7/django_i3tasks.egg-info/dependency_links.txt
+-rw-rw-r--   0 sajlx     (1000) sajlx     (1000)        1 2024-04-02 18:09:07.000000 django_i3tasks-0.0.7/django_i3tasks.egg-info/not-zip-safe
+-rw-rw-r--   0 sajlx     (1000) sajlx     (1000)       52 2024-04-02 18:09:07.000000 django_i3tasks-0.0.7/django_i3tasks.egg-info/requires.txt
+-rw-rw-r--   0 sajlx     (1000) sajlx     (1000)       15 2024-04-02 18:09:07.000000 django_i3tasks-0.0.7/django_i3tasks.egg-info/top_level.txt
+-rw-rw-r--   0 sajlx     (1000) sajlx     (1000)       38 2024-04-02 18:09:07.779171 django_i3tasks-0.0.7/setup.cfg
+-rw-rw-r--   0 sajlx     (1000) sajlx     (1000)     1048 2024-04-02 18:08:59.000000 django_i3tasks-0.0.7/setup.py
```

### Comparing `django_i3tasks-0.0.6/LICENSE` & `django_i3tasks-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `django_i3tasks-0.0.6/PKG-INFO` & `django_i3tasks-0.0.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_i3tasks
-Version: 0.0.6
+Version: 0.0.7
 Summary: Django app for manage async tasks by http requests
 Home-page: https://github.com/sajlx/django-i3tasks
 Author: Ivan Bettarini
 Author-email: ivan.bettarini@gmail.com
 License: GNU General Public License v3.0
 Classifier: Environment :: Web Environment
 Classifier: Operating System :: OS Independent
@@ -33,18 +33,20 @@
         "django_i3tasks",
     ]
 
 2. Include the polls URLconf in your project urls.py like this::
 
 
     ```
+    from django.urls import path
+
     from django_i3tasks import views as i3tasks_views
 
     path("i3/tasks-beat", i3tasks_views.BeatTaskView.as_view()),
-    path("i3/tasks-beat/", i3tasks_views.BeatTaskView.as_view()),`
+    path("i3/tasks-beat/", i3tasks_views.BeatTaskView.as_view()),
     path("i3/tasks-push", i3tasks_views.PushedTaskView.as_view()),
     path("i3/tasks-push/", i3tasks_views.PushedTaskView.as_view()),
     ```
 
 3. Run ``python manage.py migrate`` to create the models.
 
 4. Start the development server and visit the admin to create a poll.
```

### Comparing `django_i3tasks-0.0.6/README.md` & `django_i3tasks-0.0.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -16,18 +16,20 @@
         "django_i3tasks",
     ]
 
 2. Include the polls URLconf in your project urls.py like this::
 
 
     ```
+    from django.urls import path
+
     from django_i3tasks import views as i3tasks_views
 
     path("i3/tasks-beat", i3tasks_views.BeatTaskView.as_view()),
-    path("i3/tasks-beat/", i3tasks_views.BeatTaskView.as_view()),`
+    path("i3/tasks-beat/", i3tasks_views.BeatTaskView.as_view()),
     path("i3/tasks-push", i3tasks_views.PushedTaskView.as_view()),
     path("i3/tasks-push/", i3tasks_views.PushedTaskView.as_view()),
     ```
 
 3. Run ``python manage.py migrate`` to create the models.
 
 4. Start the development server and visit the admin to create a poll.
```

### Comparing `django_i3tasks-0.0.6/django_i3tasks/models.py` & `django_i3tasks-0.0.7/django_i3tasks/models.py`

 * *Files identical despite different names*

### Comparing `django_i3tasks-0.0.6/django_i3tasks/types.py` & `django_i3tasks-0.0.7/django_i3tasks/types.py`

 * *Files identical despite different names*

### Comparing `django_i3tasks-0.0.6/django_i3tasks/urls.py` & `django_i3tasks-0.0.7/django_i3tasks/urls.py`

 * *Files identical despite different names*

### Comparing `django_i3tasks-0.0.6/django_i3tasks/utils.py` & `django_i3tasks-0.0.7/django_i3tasks/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # import google
 
 # from google.oauth2 import service_account
 # from google.cloud import pubsub_v1
 
 from django.conf import settings
 
-from i3tasks.queue_manager.google_pubsub import PubSubSystemUtils, get_default_queue_setting
+from django_i3tasks.queue_manager.google_pubsub import PubSubSystemUtils, get_default_queue_setting
 
 
 logger = logging.getLogger(__name__)
 
 REGITERED_TASKS = dict()
```

### Comparing `django_i3tasks-0.0.6/django_i3tasks/views.py` & `django_i3tasks-0.0.7/django_i3tasks/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from django.http import HttpResponse
 from django.http import JsonResponse
 
 from django.views import View
 
 from django.utils.decorators import method_decorator
 
-from i3tasks.utils import TaskDecorator
+from django_i3tasks.utils import TaskDecorator
 
 
 logger = logging.getLogger(__name__)
 
 
 @method_decorator(csrf_exempt, name='dispatch')
 class BeatTaskView(View):
```

### Comparing `django_i3tasks-0.0.6/django_i3tasks.egg-info/PKG-INFO` & `django_i3tasks-0.0.7/django_i3tasks.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-i3tasks
-Version: 0.0.6
+Version: 0.0.7
 Summary: Django app for manage async tasks by http requests
 Home-page: https://github.com/sajlx/django-i3tasks
 Author: Ivan Bettarini
 Author-email: ivan.bettarini@gmail.com
 License: GNU General Public License v3.0
 Classifier: Environment :: Web Environment
 Classifier: Operating System :: OS Independent
@@ -33,18 +33,20 @@
         "django_i3tasks",
     ]
 
 2. Include the polls URLconf in your project urls.py like this::
 
 
     ```
+    from django.urls import path
+
     from django_i3tasks import views as i3tasks_views
 
     path("i3/tasks-beat", i3tasks_views.BeatTaskView.as_view()),
-    path("i3/tasks-beat/", i3tasks_views.BeatTaskView.as_view()),`
+    path("i3/tasks-beat/", i3tasks_views.BeatTaskView.as_view()),
     path("i3/tasks-push", i3tasks_views.PushedTaskView.as_view()),
     path("i3/tasks-push/", i3tasks_views.PushedTaskView.as_view()),
     ```
 
 3. Run ``python manage.py migrate`` to create the models.
 
 4. Start the development server and visit the admin to create a poll.
```

### Comparing `django_i3tasks-0.0.6/setup.py` & `django_i3tasks-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='django_i3tasks',
-    version='0.0.6',
+    version='0.0.7',
     description='Django app for manage async tasks by http requests',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/sajlx/django-i3tasks',
     author='Ivan Bettarini',
     author_email='ivan.bettarini@gmail.com',
     license='GNU General Public License v3.0',
```

