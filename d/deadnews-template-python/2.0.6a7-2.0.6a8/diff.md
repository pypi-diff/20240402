# Comparing `tmp/deadnews_template_python-2.0.6a7.tar.gz` & `tmp/deadnews_template_python-2.0.6a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deadnews_template_python-2.0.6a7.tar", max compression
+gzip compressed data, was "deadnews_template_python-2.0.6a8.tar", max compression
```

## Comparing `deadnews_template_python-2.0.6a7.tar` & `deadnews_template_python-2.0.6a8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1065 2024-04-02 17:32:50.131221 deadnews_template_python-2.0.6a7/LICENSE
--rw-r--r--   0        0        0     1948 2024-04-02 17:32:50.131221 deadnews_template_python-2.0.6a7/README.md
--rw-r--r--   0        0        0     2939 2024-04-02 17:33:02.187262 deadnews_template_python-2.0.6a7/pyproject.toml
--rw-r--r--   0        0        0       94 2024-04-02 17:32:50.135221 deadnews_template_python-2.0.6a7/src/deadnews_template_python/__init__.py
--rw-r--r--   0        0        0      514 2024-04-02 17:32:50.135221 deadnews_template_python-2.0.6a7/src/deadnews_template_python/__main__.py
--rw-r--r--   0        0        0     1392 2024-04-02 17:32:50.135221 deadnews_template_python-2.0.6a7/src/deadnews_template_python/app.py
--rw-r--r--   0        0        0     2879 1970-01-01 00:00:00.000000 deadnews_template_python-2.0.6a7/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-02 17:52:52.658665 deadnews_template_python-2.0.6a8/LICENSE
+-rw-r--r--   0        0        0     1948 2024-04-02 17:52:52.658665 deadnews_template_python-2.0.6a8/README.md
+-rw-r--r--   0        0        0     2939 2024-04-02 17:53:04.166661 deadnews_template_python-2.0.6a8/pyproject.toml
+-rw-r--r--   0        0        0       94 2024-04-02 17:52:52.662665 deadnews_template_python-2.0.6a8/src/deadnews_template_python/__init__.py
+-rw-r--r--   0        0        0      514 2024-04-02 17:52:52.662665 deadnews_template_python-2.0.6a8/src/deadnews_template_python/__main__.py
+-rw-r--r--   0        0        0     1392 2024-04-02 17:52:52.662665 deadnews_template_python-2.0.6a8/src/deadnews_template_python/app.py
+-rw-r--r--   0        0        0     2879 1970-01-01 00:00:00.000000 deadnews_template_python-2.0.6a8/PKG-INFO
```

### Comparing `deadnews_template_python-2.0.6a7/LICENSE` & `deadnews_template_python-2.0.6a8/LICENSE`

 * *Files identical despite different names*

### Comparing `deadnews_template_python-2.0.6a7/README.md` & `deadnews_template_python-2.0.6a8/README.md`

 * *Files identical despite different names*

### Comparing `deadnews_template_python-2.0.6a7/pyproject.toml` & `deadnews_template_python-2.0.6a8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "deadnews-template-python"
-version = "2.0.6-alpha.7"
+version = "2.0.6-alpha.8"
 description = "Python Project Template"
-authors = ["DeadNews <aurczpbgr@mozmail.com>"]
+authors = ["DeadNews <deadnewsgit@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/deadnews/deadnews-template-python"
 repository = "https://github.com/deadnews/deadnews-template-python"
 documentation = "https://deadnews.github.io/deadnews-template-python"
 keywords = ["python", "template", "layout"]
 classifiers = ["Operating System :: OS Independent"]
```

### Comparing `deadnews_template_python-2.0.6a7/src/deadnews_template_python/__main__.py` & `deadnews_template_python-2.0.6a8/src/deadnews_template_python/__main__.py`

 * *Files identical despite different names*

### Comparing `deadnews_template_python-2.0.6a7/src/deadnews_template_python/app.py` & `deadnews_template_python-2.0.6a8/src/deadnews_template_python/app.py`

 * *Files identical despite different names*

### Comparing `deadnews_template_python-2.0.6a7/PKG-INFO` & `deadnews_template_python-2.0.6a8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: deadnews-template-python
-Version: 2.0.6a7
+Version: 2.0.6a8
 Summary: Python Project Template
 Home-page: https://github.com/deadnews/deadnews-template-python
 License: MIT
 Keywords: python,template,layout
 Author: DeadNews
-Author-email: aurczpbgr@mozmail.com
+Author-email: deadnewsgit@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

