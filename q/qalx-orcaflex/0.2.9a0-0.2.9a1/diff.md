# Comparing `tmp/qalx_orcaflex-0.2.9a0.tar.gz` & `tmp/qalx_orcaflex-0.2.9a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qalx_orcaflex-0.2.9a0.tar", max compression
+gzip compressed data, was "qalx_orcaflex-0.2.9a1.tar", max compression
```

## Comparing `qalx_orcaflex-0.2.9a0.tar` & `qalx_orcaflex-0.2.9a1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0      933 2023-11-27 17:18:54.310372 qalx_orcaflex-0.2.9a0/pyproject.toml
--rw-r--r--   0        0        0      407 2023-11-27 17:18:54.310372 qalx_orcaflex-0.2.9a0/qalx_orcaflex/__init__.py
--rw-r--r--   0        0        0      181 2023-11-27 17:18:54.310372 qalx_orcaflex-0.2.9a0/qalx_orcaflex/bots/__init__.py
--rw-r--r--   0        0        0     7196 2023-11-27 17:18:54.310372 qalx_orcaflex-0.2.9a0/qalx_orcaflex/bots/batch/__init__.py
--rw-r--r--   0        0        0     9768 2023-11-27 17:18:54.310372 qalx_orcaflex-0.2.9a0/qalx_orcaflex/bots/batch/summaries.py
--rw-r--r--   0        0        0     1038 2023-11-27 17:18:54.310372 qalx_orcaflex-0.2.9a0/qalx_orcaflex/bots/sim/__init__.py
--rw-r--r--   0        0        0     4047 2023-11-27 17:18:54.310372 qalx_orcaflex-0.2.9a0/qalx_orcaflex/bots/sim/functions.py
--rw-r--r--   0        0        0    32704 2023-11-27 17:18:54.314372 qalx_orcaflex-0.2.9a0/qalx_orcaflex/bots/sim/tasks.py
--rw-r--r--   0        0        0      709 2023-11-27 17:18:54.314372 qalx_orcaflex-0.2.9a0/qalx_orcaflex/bots/video.py
--rw-r--r--   0        0        0    38574 2023-11-27 17:18:54.314372 qalx_orcaflex-0.2.9a0/qalx_orcaflex/core/__init__.py
--rw-r--r--   0        0        0    35864 2023-11-27 17:18:54.314372 qalx_orcaflex-0.2.9a0/qalx_orcaflex/data_models/__init__.py
--rw-r--r--   0        0        0    10637 2023-11-27 17:18:54.314372 qalx_orcaflex-0.2.9a0/qalx_orcaflex/data_models/notifications/__init__.py
--rw-r--r--   0        0        0      325 2023-11-27 17:18:54.314372 qalx_orcaflex-0.2.9a0/qalx_orcaflex/data_models/notifications/templates/notification_completed.html
--rw-r--r--   0        0        0      385 2023-11-27 17:18:54.314372 qalx_orcaflex-0.2.9a0/qalx_orcaflex/data_models/notifications/templates/notification_submitted.html
--rw-r--r--   0        0        0      347 2023-11-27 17:18:54.314372 qalx_orcaflex-0.2.9a0/qalx_orcaflex/data_models/notifications/templates/notification_timed_out.html
--rw-r--r--   0        0        0        0 2023-11-27 17:18:54.314372 qalx_orcaflex-0.2.9a0/qalx_orcaflex/gui/__init__.py
--rw-r--r--   0        0        0        0 2023-11-27 17:18:54.314372 qalx_orcaflex-0.2.9a0/qalx_orcaflex/gui/batch/__init__.py
--rw-r--r--   0        0        0     7550 2023-11-27 17:18:54.314372 qalx_orcaflex-0.2.9a0/qalx_orcaflex/gui/batch/core.py
--rw-r--r--   0        0        0        0 2023-11-27 17:18:54.314372 qalx_orcaflex-0.2.9a0/qalx_orcaflex/gui/batch/models/__init__.py
--rw-r--r--   0        0        0     5528 2023-11-27 17:18:54.314372 qalx_orcaflex-0.2.9a0/qalx_orcaflex/gui/batch/models/table.py
--rw-r--r--   0        0        0    19365 2023-11-27 17:18:54.314372 qalx_orcaflex-0.2.9a0/qalx_orcaflex/gui/batch/overview_main.py
--rw-r--r--   0        0        0    10712 2023-11-27 17:18:54.314372 qalx_orcaflex-0.2.9a0/qalx_orcaflex/gui/batch/overview_main_ui.py
--rw-r--r--   0        0        0     1926 2023-11-27 17:18:54.314372 qalx_orcaflex-0.2.9a0/qalx_orcaflex/gui/batch/requeue_jobs_dialog.py
--rw-r--r--   0        0        0     2494 2023-11-27 17:18:54.314372 qalx_orcaflex-0.2.9a0/qalx_orcaflex/gui/batch/requeue_jobs_dialog_ui.py
--rw-r--r--   0        0        0      579 2023-11-27 17:18:54.314372 qalx_orcaflex-0.2.9a0/qalx_orcaflex/gui/icons/qalx_32x32_favicon.png
--rw-r--r--   0        0        0    18889 2023-11-27 17:18:54.314372 qalx_orcaflex-0.2.9a0/qalx_orcaflex/helpers/__init__.py
--rw-r--r--   0        0        0     2818 2023-11-27 17:18:54.314372 qalx_orcaflex-0.2.9a0/qalx_orcaflex/helpers/excel.py
--rw-r--r--   0        0        0     1346 2023-11-27 17:18:54.314372 qalx_orcaflex-0.2.9a0/qalx_orcaflex/helpers/restarts.py
--rw-r--r--   0        0        0     2539 2023-11-27 17:18:54.314372 qalx_orcaflex-0.2.9a0/qalx_orcaflex/helpers/results_dataframes.py
--rw-r--r--   0        0        0    17213 2023-11-27 17:18:54.314372 qalx_orcaflex-0.2.9a0/qalx_orcaflex/helpers/smart_statics.py
--rw-r--r--   0        0        0      135 2023-11-27 17:18:54.314372 qalx_orcaflex-0.2.9a0/qalx_orcaflex/video/__init__.py
--rw-r--r--   0        0        0     2486 2023-11-27 17:18:54.314372 qalx_orcaflex-0.2.9a0/qalx_orcaflex/video/core.py
--rw-r--r--   0        0        0     4833 2023-11-27 17:18:54.314372 qalx_orcaflex-0.2.9a0/qalx_orcaflex/video/extract.py
--rw-r--r--   0        0        0     1235 2023-11-27 17:18:54.314372 qalx_orcaflex-0.2.9a0/qalx_orcaflex/video/helpers.py
--rw-r--r--   0        0        0     1486 2023-11-27 17:18:54.314372 qalx_orcaflex-0.2.9a0/readme.md
--rw-r--r--   0        0        0     2685 1970-01-01 00:00:00.000000 qalx_orcaflex-0.2.9a0/PKG-INFO
+-rw-r--r--   0        0        0      933 2023-11-27 17:51:18.058149 qalx_orcaflex-0.2.9a1/pyproject.toml
+-rw-r--r--   0        0        0      407 2023-11-27 17:51:18.058149 qalx_orcaflex-0.2.9a1/qalx_orcaflex/__init__.py
+-rw-r--r--   0        0        0      181 2023-11-27 17:51:18.058149 qalx_orcaflex-0.2.9a1/qalx_orcaflex/bots/__init__.py
+-rw-r--r--   0        0        0     7196 2023-11-27 17:51:18.062149 qalx_orcaflex-0.2.9a1/qalx_orcaflex/bots/batch/__init__.py
+-rw-r--r--   0        0        0     9768 2023-11-27 17:51:18.062149 qalx_orcaflex-0.2.9a1/qalx_orcaflex/bots/batch/summaries.py
+-rw-r--r--   0        0        0     1038 2023-11-27 17:51:18.062149 qalx_orcaflex-0.2.9a1/qalx_orcaflex/bots/sim/__init__.py
+-rw-r--r--   0        0        0     4067 2023-11-27 17:51:18.062149 qalx_orcaflex-0.2.9a1/qalx_orcaflex/bots/sim/functions.py
+-rw-r--r--   0        0        0    32704 2023-11-27 17:51:18.062149 qalx_orcaflex-0.2.9a1/qalx_orcaflex/bots/sim/tasks.py
+-rw-r--r--   0        0        0      709 2023-11-27 17:51:18.062149 qalx_orcaflex-0.2.9a1/qalx_orcaflex/bots/video.py
+-rw-r--r--   0        0        0    38574 2023-11-27 17:51:18.062149 qalx_orcaflex-0.2.9a1/qalx_orcaflex/core/__init__.py
+-rw-r--r--   0        0        0    35864 2023-11-27 17:51:18.062149 qalx_orcaflex-0.2.9a1/qalx_orcaflex/data_models/__init__.py
+-rw-r--r--   0        0        0    10637 2023-11-27 17:51:18.062149 qalx_orcaflex-0.2.9a1/qalx_orcaflex/data_models/notifications/__init__.py
+-rw-r--r--   0        0        0      325 2023-11-27 17:51:18.062149 qalx_orcaflex-0.2.9a1/qalx_orcaflex/data_models/notifications/templates/notification_completed.html
+-rw-r--r--   0        0        0      385 2023-11-27 17:51:18.062149 qalx_orcaflex-0.2.9a1/qalx_orcaflex/data_models/notifications/templates/notification_submitted.html
+-rw-r--r--   0        0        0      347 2023-11-27 17:51:18.062149 qalx_orcaflex-0.2.9a1/qalx_orcaflex/data_models/notifications/templates/notification_timed_out.html
+-rw-r--r--   0        0        0        0 2023-11-27 17:51:18.062149 qalx_orcaflex-0.2.9a1/qalx_orcaflex/gui/__init__.py
+-rw-r--r--   0        0        0        0 2023-11-27 17:51:18.062149 qalx_orcaflex-0.2.9a1/qalx_orcaflex/gui/batch/__init__.py
+-rw-r--r--   0        0        0     7550 2023-11-27 17:51:18.062149 qalx_orcaflex-0.2.9a1/qalx_orcaflex/gui/batch/core.py
+-rw-r--r--   0        0        0        0 2023-11-27 17:51:18.062149 qalx_orcaflex-0.2.9a1/qalx_orcaflex/gui/batch/models/__init__.py
+-rw-r--r--   0        0        0     5528 2023-11-27 17:51:18.062149 qalx_orcaflex-0.2.9a1/qalx_orcaflex/gui/batch/models/table.py
+-rw-r--r--   0        0        0    19365 2023-11-27 17:51:18.062149 qalx_orcaflex-0.2.9a1/qalx_orcaflex/gui/batch/overview_main.py
+-rw-r--r--   0        0        0    10712 2023-11-27 17:51:18.062149 qalx_orcaflex-0.2.9a1/qalx_orcaflex/gui/batch/overview_main_ui.py
+-rw-r--r--   0        0        0     1926 2023-11-27 17:51:18.062149 qalx_orcaflex-0.2.9a1/qalx_orcaflex/gui/batch/requeue_jobs_dialog.py
+-rw-r--r--   0        0        0     2494 2023-11-27 17:51:18.062149 qalx_orcaflex-0.2.9a1/qalx_orcaflex/gui/batch/requeue_jobs_dialog_ui.py
+-rw-r--r--   0        0        0      579 2023-11-27 17:51:18.062149 qalx_orcaflex-0.2.9a1/qalx_orcaflex/gui/icons/qalx_32x32_favicon.png
+-rw-r--r--   0        0        0    18889 2023-11-27 17:51:18.062149 qalx_orcaflex-0.2.9a1/qalx_orcaflex/helpers/__init__.py
+-rw-r--r--   0        0        0     2818 2023-11-27 17:51:18.062149 qalx_orcaflex-0.2.9a1/qalx_orcaflex/helpers/excel.py
+-rw-r--r--   0        0        0     1346 2023-11-27 17:51:18.062149 qalx_orcaflex-0.2.9a1/qalx_orcaflex/helpers/restarts.py
+-rw-r--r--   0        0        0     2539 2023-11-27 17:51:18.062149 qalx_orcaflex-0.2.9a1/qalx_orcaflex/helpers/results_dataframes.py
+-rw-r--r--   0        0        0    17213 2023-11-27 17:51:18.062149 qalx_orcaflex-0.2.9a1/qalx_orcaflex/helpers/smart_statics.py
+-rw-r--r--   0        0        0      135 2023-11-27 17:51:18.062149 qalx_orcaflex-0.2.9a1/qalx_orcaflex/video/__init__.py
+-rw-r--r--   0        0        0     2486 2023-11-27 17:51:18.062149 qalx_orcaflex-0.2.9a1/qalx_orcaflex/video/core.py
+-rw-r--r--   0        0        0     4833 2023-11-27 17:51:18.062149 qalx_orcaflex-0.2.9a1/qalx_orcaflex/video/extract.py
+-rw-r--r--   0        0        0     1235 2023-11-27 17:51:18.062149 qalx_orcaflex-0.2.9a1/qalx_orcaflex/video/helpers.py
+-rw-r--r--   0        0        0     1486 2023-11-27 17:51:18.062149 qalx_orcaflex-0.2.9a1/readme.md
+-rw-r--r--   0        0        0     2685 1970-01-01 00:00:00.000000 qalx_orcaflex-0.2.9a1/PKG-INFO
```

### Comparing `qalx_orcaflex-0.2.9a0/pyproject.toml` & `qalx_orcaflex-0.2.9a1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qalx-orcaflex"
-version = "0.2.9a0"
+version = "0.2.9a1"
 description = "qalx bots and helpers for OrcaFlex"
 authors = ["Steven Rossiter <steve@agiletek.co.uk>"]
 license = "GPL-3.0+"
 readme = "readme.md"
 documentation = "https://orcaflex.qalx.net"
 
 [tool.poetry.dependencies]
```

### Comparing `qalx_orcaflex-0.2.9a0/qalx_orcaflex/bots/batch/__init__.py` & `qalx_orcaflex-0.2.9a1/qalx_orcaflex/bots/batch/__init__.py`

 * *Files identical despite different names*

### Comparing `qalx_orcaflex-0.2.9a0/qalx_orcaflex/bots/batch/summaries.py` & `qalx_orcaflex-0.2.9a1/qalx_orcaflex/bots/batch/summaries.py`

 * *Files identical despite different names*

### Comparing `qalx_orcaflex-0.2.9a0/qalx_orcaflex/bots/sim/__init__.py` & `qalx_orcaflex-0.2.9a1/qalx_orcaflex/bots/sim/__init__.py`

 * *Files identical despite different names*

### Comparing `qalx_orcaflex-0.2.9a0/qalx_orcaflex/bots/sim/functions.py` & `qalx_orcaflex-0.2.9a1/qalx_orcaflex/bots/sim/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,10 +107,10 @@
             del job.context["model"].progressHandlerCallback
         except AttributeError:
             pass
         del job.context["model"]
 
 
 def onload_orcaflex(job: QalxJob):
-    task = job.context["task"]
-    if task.options.delete_message_on_load:
+    _options = job.entity.get_item_data("job_options")
+    if _options.delete_message_on_load:
         job.delete_message()
```

### Comparing `qalx_orcaflex-0.2.9a0/qalx_orcaflex/bots/sim/tasks.py` & `qalx_orcaflex-0.2.9a1/qalx_orcaflex/bots/sim/tasks.py`

 * *Files identical despite different names*

### Comparing `qalx_orcaflex-0.2.9a0/qalx_orcaflex/bots/video.py` & `qalx_orcaflex-0.2.9a1/qalx_orcaflex/bots/video.py`

 * *Files identical despite different names*

### Comparing `qalx_orcaflex-0.2.9a0/qalx_orcaflex/core/__init__.py` & `qalx_orcaflex-0.2.9a1/qalx_orcaflex/core/__init__.py`

 * *Files identical despite different names*

### Comparing `qalx_orcaflex-0.2.9a0/qalx_orcaflex/data_models/__init__.py` & `qalx_orcaflex-0.2.9a1/qalx_orcaflex/data_models/__init__.py`

 * *Files identical despite different names*

### Comparing `qalx_orcaflex-0.2.9a0/qalx_orcaflex/data_models/notifications/__init__.py` & `qalx_orcaflex-0.2.9a1/qalx_orcaflex/data_models/notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `qalx_orcaflex-0.2.9a0/qalx_orcaflex/gui/batch/core.py` & `qalx_orcaflex-0.2.9a1/qalx_orcaflex/gui/batch/core.py`

 * *Files identical despite different names*

### Comparing `qalx_orcaflex-0.2.9a0/qalx_orcaflex/gui/batch/models/table.py` & `qalx_orcaflex-0.2.9a1/qalx_orcaflex/gui/batch/models/table.py`

 * *Files identical despite different names*

### Comparing `qalx_orcaflex-0.2.9a0/qalx_orcaflex/gui/batch/overview_main.py` & `qalx_orcaflex-0.2.9a1/qalx_orcaflex/gui/batch/overview_main.py`

 * *Files identical despite different names*

### Comparing `qalx_orcaflex-0.2.9a0/qalx_orcaflex/gui/batch/overview_main_ui.py` & `qalx_orcaflex-0.2.9a1/qalx_orcaflex/gui/batch/overview_main_ui.py`

 * *Files identical despite different names*

### Comparing `qalx_orcaflex-0.2.9a0/qalx_orcaflex/gui/batch/requeue_jobs_dialog.py` & `qalx_orcaflex-0.2.9a1/qalx_orcaflex/gui/batch/requeue_jobs_dialog.py`

 * *Files identical despite different names*

### Comparing `qalx_orcaflex-0.2.9a0/qalx_orcaflex/gui/batch/requeue_jobs_dialog_ui.py` & `qalx_orcaflex-0.2.9a1/qalx_orcaflex/gui/batch/requeue_jobs_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `qalx_orcaflex-0.2.9a0/qalx_orcaflex/gui/icons/qalx_32x32_favicon.png` & `qalx_orcaflex-0.2.9a1/qalx_orcaflex/gui/icons/qalx_32x32_favicon.png`

 * *Files identical despite different names*

### Comparing `qalx_orcaflex-0.2.9a0/qalx_orcaflex/helpers/__init__.py` & `qalx_orcaflex-0.2.9a1/qalx_orcaflex/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `qalx_orcaflex-0.2.9a0/qalx_orcaflex/helpers/excel.py` & `qalx_orcaflex-0.2.9a1/qalx_orcaflex/helpers/excel.py`

 * *Files identical despite different names*

### Comparing `qalx_orcaflex-0.2.9a0/qalx_orcaflex/helpers/restarts.py` & `qalx_orcaflex-0.2.9a1/qalx_orcaflex/helpers/restarts.py`

 * *Files identical despite different names*

### Comparing `qalx_orcaflex-0.2.9a0/qalx_orcaflex/helpers/results_dataframes.py` & `qalx_orcaflex-0.2.9a1/qalx_orcaflex/helpers/results_dataframes.py`

 * *Files identical despite different names*

### Comparing `qalx_orcaflex-0.2.9a0/qalx_orcaflex/helpers/smart_statics.py` & `qalx_orcaflex-0.2.9a1/qalx_orcaflex/helpers/smart_statics.py`

 * *Files identical despite different names*

### Comparing `qalx_orcaflex-0.2.9a0/qalx_orcaflex/video/core.py` & `qalx_orcaflex-0.2.9a1/qalx_orcaflex/video/core.py`

 * *Files identical despite different names*

### Comparing `qalx_orcaflex-0.2.9a0/qalx_orcaflex/video/extract.py` & `qalx_orcaflex-0.2.9a1/qalx_orcaflex/video/extract.py`

 * *Files identical despite different names*

### Comparing `qalx_orcaflex-0.2.9a0/qalx_orcaflex/video/helpers.py` & `qalx_orcaflex-0.2.9a1/qalx_orcaflex/video/helpers.py`

 * *Files identical despite different names*

### Comparing `qalx_orcaflex-0.2.9a0/readme.md` & `qalx_orcaflex-0.2.9a1/readme.md`

 * *Files identical despite different names*

### Comparing `qalx_orcaflex-0.2.9a0/PKG-INFO` & `qalx_orcaflex-0.2.9a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qalx-orcaflex
-Version: 0.2.9a0
+Version: 0.2.9a1
 Summary: qalx bots and helpers for OrcaFlex
 License: GPL-3.0+
 Author: Steven Rossiter
 Author-email: steve@agiletek.co.uk
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

