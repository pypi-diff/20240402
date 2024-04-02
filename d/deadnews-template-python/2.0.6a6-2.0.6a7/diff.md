# Comparing `tmp/deadnews_template_python-2.0.6a6.tar.gz` & `tmp/deadnews_template_python-2.0.6a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deadnews_template_python-2.0.6a6.tar", max compression
+gzip compressed data, was "deadnews_template_python-2.0.6a7.tar", max compression
```

## Comparing `deadnews_template_python-2.0.6a6.tar` & `deadnews_template_python-2.0.6a7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1065 2024-03-30 16:58:53.782201 deadnews_template_python-2.0.6a6/LICENSE
--rw-r--r--   0        0        0     1948 2024-03-30 16:58:53.782201 deadnews_template_python-2.0.6a6/README.md
--rw-r--r--   0        0        0     2939 2024-03-30 16:59:03.382212 deadnews_template_python-2.0.6a6/pyproject.toml
--rw-r--r--   0        0        0       94 2024-03-30 16:58:53.782201 deadnews_template_python-2.0.6a6/src/deadnews_template_python/__init__.py
--rw-r--r--   0        0        0      514 2024-03-30 16:58:53.782201 deadnews_template_python-2.0.6a6/src/deadnews_template_python/__main__.py
--rw-r--r--   0        0        0     1392 2024-03-30 16:58:53.782201 deadnews_template_python-2.0.6a6/src/deadnews_template_python/app.py
--rw-r--r--   0        0        0     2879 1970-01-01 00:00:00.000000 deadnews_template_python-2.0.6a6/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-02 17:32:50.131221 deadnews_template_python-2.0.6a7/LICENSE
+-rw-r--r--   0        0        0     1948 2024-04-02 17:32:50.131221 deadnews_template_python-2.0.6a7/README.md
+-rw-r--r--   0        0        0     2939 2024-04-02 17:33:02.187262 deadnews_template_python-2.0.6a7/pyproject.toml
+-rw-r--r--   0        0        0       94 2024-04-02 17:32:50.135221 deadnews_template_python-2.0.6a7/src/deadnews_template_python/__init__.py
+-rw-r--r--   0        0        0      514 2024-04-02 17:32:50.135221 deadnews_template_python-2.0.6a7/src/deadnews_template_python/__main__.py
+-rw-r--r--   0        0        0     1392 2024-04-02 17:32:50.135221 deadnews_template_python-2.0.6a7/src/deadnews_template_python/app.py
+-rw-r--r--   0        0        0     2879 1970-01-01 00:00:00.000000 deadnews_template_python-2.0.6a7/PKG-INFO
```

### Comparing `deadnews_template_python-2.0.6a6/LICENSE` & `deadnews_template_python-2.0.6a7/LICENSE`

 * *Files identical despite different names*

### Comparing `deadnews_template_python-2.0.6a6/README.md` & `deadnews_template_python-2.0.6a7/README.md`

 * *Files identical despite different names*

### Comparing `deadnews_template_python-2.0.6a6/pyproject.toml` & `deadnews_template_python-2.0.6a7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "deadnews-template-python"
-version = "2.0.6-alpha.6"
+version = "2.0.6-alpha.7"
 description = "Python Project Template"
 authors = ["DeadNews <aurczpbgr@mozmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/deadnews/deadnews-template-python"
 repository = "https://github.com/deadnews/deadnews-template-python"
 documentation = "https://deadnews.github.io/deadnews-template-python"
```

### Comparing `deadnews_template_python-2.0.6a6/src/deadnews_template_python/__main__.py` & `deadnews_template_python-2.0.6a7/src/deadnews_template_python/__main__.py`

 * *Files identical despite different names*

### Comparing `deadnews_template_python-2.0.6a6/src/deadnews_template_python/app.py` & `deadnews_template_python-2.0.6a7/src/deadnews_template_python/app.py`

 * *Files identical despite different names*

### Comparing `deadnews_template_python-2.0.6a6/PKG-INFO` & `deadnews_template_python-2.0.6a7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deadnews-template-python
-Version: 2.0.6a6
+Version: 2.0.6a7
 Summary: Python Project Template
 Home-page: https://github.com/deadnews/deadnews-template-python
 License: MIT
 Keywords: python,template,layout
 Author: DeadNews
 Author-email: aurczpbgr@mozmail.com
 Requires-Python: >=3.10,<4.0
```

