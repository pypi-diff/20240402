# Comparing `tmp/taskara-0.1.0.tar.gz` & `tmp/taskara-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskara-0.1.0.tar", max compression
+gzip compressed data, was "taskara-0.1.1.tar", max compression
```

## Comparing `taskara-0.1.0.tar` & `taskara-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0    11357 2024-03-22 17:15:53.679144 taskara-0.1.0/LICENSE
--rw-r--r--   0        0        0       41 2024-04-02 20:36:44.979933 taskara-0.1.0/README.md
--rw-r--r--   0        0        0      391 2024-04-02 20:30:42.561546 taskara-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2001 2024-04-02 20:34:43.380692 taskara-0.1.0/taskara/db/conn.py
--rw-r--r--   0        0        0     1449 2024-04-02 20:36:27.320183 taskara-0.1.0/taskara/db/models.py
--rw-r--r--   0        0        0      195 2024-04-02 20:31:31.417190 taskara-0.1.0/taskara/env.py
--rw-r--r--   0        0        0     1457 2024-04-02 20:34:08.999667 taskara-0.1.0/taskara/models.py
--rw-r--r--   0        0        0    20304 2024-04-02 20:38:39.122416 taskara-0.1.0/taskara/task.py
--rw-r--r--   0        0        0      611 1970-01-01 00:00:00.000000 taskara-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-03-22 17:15:53.679144 taskara-0.1.1/LICENSE
+-rw-r--r--   0        0        0      221 2024-04-02 20:40:49.884528 taskara-0.1.1/README.md
+-rw-r--r--   0        0        0      392 2024-04-02 20:42:07.253730 taskara-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       23 2024-04-02 20:42:34.072763 taskara-0.1.1/taskara/__init__.py
+-rw-r--r--   0        0        0     2001 2024-04-02 20:34:43.380692 taskara-0.1.1/taskara/db/conn.py
+-rw-r--r--   0        0        0     1449 2024-04-02 20:36:27.320183 taskara-0.1.1/taskara/db/models.py
+-rw-r--r--   0        0        0      195 2024-04-02 20:31:31.417190 taskara-0.1.1/taskara/env.py
+-rw-r--r--   0        0        0     1457 2024-04-02 20:34:08.999667 taskara-0.1.1/taskara/models.py
+-rw-r--r--   0        0        0    20304 2024-04-02 20:38:39.122416 taskara-0.1.1/taskara/task.py
+-rw-r--r--   0        0        0      792 1970-01-01 00:00:00.000000 taskara-0.1.1/PKG-INFO
```

### Comparing `taskara-0.1.0/LICENSE` & `taskara-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `taskara-0.1.0/taskara/db/conn.py` & `taskara-0.1.1/taskara/db/conn.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.0/taskara/db/models.py` & `taskara-0.1.1/taskara/db/models.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.0/taskara/models.py` & `taskara-0.1.1/taskara/models.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.0/taskara/task.py` & `taskara-0.1.1/taskara/task.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.0/PKG-INFO` & `taskara-0.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: taskara
-Version: 0.1.0
-Summary: A task library for AI agents
+Version: 0.1.1
+Summary: Task management for AI agents
 License: Apache 2.0
 Author: Patrick Barker
 Author-email: patrickbarkerco@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -15,7 +15,23 @@
 Requires-Dist: threadmem (>=0.2.11,<0.3.0)
 Description-Content-Type: text/markdown
 
 # Taskara
 
 Task management for AI agents
 
+## Installation
+
+```sh
+pip install taskara
+```
+
+## Usage
+
+```python
+from taskara import Task
+
+task = Task()
+
+task.post_message("assistant", "getting started working on this")
+```
+
```

