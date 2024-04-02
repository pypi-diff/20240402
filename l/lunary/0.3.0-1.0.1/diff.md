# Comparing `tmp/lunary-0.3.0.tar.gz` & `tmp/lunary-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lunary-0.3.0.tar", max compression
+gzip compressed data, was "lunary-1.0.1.tar", max compression
```

## Comparing `lunary-0.3.0.tar` & `lunary-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      604 2024-02-28 21:10:30.380738 lunary-0.3.0/README.md
--rw-r--r--   0        0        0    57251 2024-04-02 01:49:13.753827 lunary-0.3.0/lunary/__init__.py
--rw-r--r--   0        0        0     2221 2024-04-01 02:07:49.605602 lunary-0.3.0/lunary/consumer.py
--rw-r--r--   0        0        0      607 2024-03-13 20:53:32.460623 lunary-0.3.0/lunary/event_queue.py
--rw-r--r--   0        0        0      834 2024-03-03 18:24:22.696583 lunary-0.3.0/lunary/langchain/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0      620 2024-03-03 18:23:24.270210 lunary-0.3.0/lunary/langchain/__pycache__/callback_handler.cpython-312.pyc
--rw-r--r--   0        0        0     2384 2024-03-04 00:09:26.744750 lunary-0.3.0/lunary/openai_utils.py
--rw-r--r--   0        0        0      670 2024-04-01 15:34:21.542269 lunary-0.3.0/lunary/parent.py
--rw-r--r--   0        0        0     1071 2024-04-02 01:49:22.083662 lunary-0.3.0/lunary/parsers.py
--rw-r--r--   0        0        0      425 2024-04-01 02:07:35.888287 lunary-0.3.0/lunary/project.py
--rw-r--r--   0        0        0      378 2024-03-04 00:09:26.744921 lunary-0.3.0/lunary/tags.py
--rw-r--r--   0        0        0      841 2024-03-04 00:09:26.744980 lunary-0.3.0/lunary/thread.py
--rw-r--r--   0        0        0      573 2024-03-04 00:09:26.745039 lunary-0.3.0/lunary/users.py
--rw-r--r--   0        0        0      747 2024-04-02 01:49:39.245342 lunary-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1685 1970-01-01 00:00:00.000000 lunary-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      604 2024-02-28 21:10:30.380738 lunary-1.0.1/README.md
+-rw-r--r--   0        0        0    57251 2024-04-02 01:49:13.753827 lunary-1.0.1/lunary/__init__.py
+-rw-r--r--   0        0        0     2221 2024-04-01 02:07:49.605602 lunary-1.0.1/lunary/consumer.py
+-rw-r--r--   0        0        0      607 2024-03-13 20:53:32.460623 lunary-1.0.1/lunary/event_queue.py
+-rw-r--r--   0        0        0      834 2024-03-03 18:24:22.696583 lunary-1.0.1/lunary/langchain/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0      620 2024-03-03 18:23:24.270210 lunary-1.0.1/lunary/langchain/__pycache__/callback_handler.cpython-312.pyc
+-rw-r--r--   0        0        0     2384 2024-03-04 00:09:26.744750 lunary-1.0.1/lunary/openai_utils.py
+-rw-r--r--   0        0        0      670 2024-04-01 15:34:21.542269 lunary-1.0.1/lunary/parent.py
+-rw-r--r--   0        0        0     1071 2024-04-02 01:49:22.083662 lunary-1.0.1/lunary/parsers.py
+-rw-r--r--   0        0        0      425 2024-04-01 02:07:35.888287 lunary-1.0.1/lunary/project.py
+-rw-r--r--   0        0        0      378 2024-03-04 00:09:26.744921 lunary-1.0.1/lunary/tags.py
+-rw-r--r--   0        0        0      841 2024-03-04 00:09:26.744980 lunary-1.0.1/lunary/thread.py
+-rw-r--r--   0        0        0      573 2024-03-04 00:09:26.745039 lunary-1.0.1/lunary/users.py
+-rw-r--r--   0        0        0      747 2024-04-02 01:51:54.569858 lunary-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1685 1970-01-01 00:00:00.000000 lunary-1.0.1/PKG-INFO
```

### Comparing `lunary-0.3.0/README.md` & `lunary-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `lunary-0.3.0/lunary/__init__.py` & `lunary-1.0.1/lunary/__init__.py`

 * *Files identical despite different names*

### Comparing `lunary-0.3.0/lunary/consumer.py` & `lunary-1.0.1/lunary/consumer.py`

 * *Files identical despite different names*

### Comparing `lunary-0.3.0/lunary/event_queue.py` & `lunary-1.0.1/lunary/event_queue.py`

 * *Files identical despite different names*

### Comparing `lunary-0.3.0/lunary/langchain/__pycache__/__init__.cpython-312.pyc` & `lunary-1.0.1/lunary/langchain/__pycache__/__init__.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `lunary-0.3.0/lunary/langchain/__pycache__/callback_handler.cpython-312.pyc` & `lunary-1.0.1/lunary/langchain/__pycache__/callback_handler.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `lunary-0.3.0/lunary/openai_utils.py` & `lunary-1.0.1/lunary/openai_utils.py`

 * *Files identical despite different names*

### Comparing `lunary-0.3.0/lunary/parent.py` & `lunary-1.0.1/lunary/parent.py`

 * *Files identical despite different names*

### Comparing `lunary-0.3.0/lunary/parsers.py` & `lunary-1.0.1/lunary/parsers.py`

 * *Files identical despite different names*

### Comparing `lunary-0.3.0/lunary/thread.py` & `lunary-1.0.1/lunary/thread.py`

 * *Files identical despite different names*

### Comparing `lunary-0.3.0/lunary/users.py` & `lunary-1.0.1/lunary/users.py`

 * *Files identical despite different names*

### Comparing `lunary-0.3.0/pyproject.toml` & `lunary-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lunary"
-version = "0.3.0"
+version = "1.0.1"
 description = "Observability, analytics and evaluations for AI agents and chatbots."
 authors = ["lunary <hello@lunary.ai>"]
 readme = "README.md"
 repository = "https://github.com/lunary/lunary.ai/"
 documentation = "https://lunary.ai/docs/py/usage"
 keywords = ["Lunary", "lunary.ai", "Langchain", "AI", "Analytics", "Monitoring"]
```

### Comparing `lunary-0.3.0/PKG-INFO` & `lunary-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lunary
-Version: 0.3.0
+Version: 1.0.1
 Summary: Observability, analytics and evaluations for AI agents and chatbots.
 Home-page: https://github.com/lunary/lunary.ai/
 Keywords: Lunary,lunary.ai,Langchain,AI,Analytics,Monitoring
 Author: lunary
 Author-email: hello@lunary.ai
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
```

