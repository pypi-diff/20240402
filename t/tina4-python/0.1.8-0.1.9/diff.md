# Comparing `tmp/tina4_python-0.1.8.tar.gz` & `tmp/tina4_python-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tina4_python-0.1.8.tar", max compression
+gzip compressed data, was "tina4_python-0.1.9.tar", max compression
```

## Comparing `tina4_python-0.1.8.tar` & `tina4_python-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      485 2022-12-02 00:27:03.440305 tina4_python-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     2705 2022-12-02 00:26:45.717063 tina4_python-0.1.8/tina4_python/__init__.py
--rw-r--r--   0        0        0      586 2022-11-25 19:59:18.456107 tina4_python-0.1.8/tina4_python/Constant.py
--rw-r--r--   0        0        0      397 2022-11-25 14:23:51.866002 tina4_python-0.1.8/tina4_python/Debug.py
--rw-r--r--   0        0        0      481 2022-11-26 17:53:07.891744 tina4_python-0.1.8/tina4_python/Env.py
--rw-r--r--   0        0        0      459 2022-11-26 19:57:26.301000 tina4_python-0.1.8/tina4_python/public/errors/403.twig
--rw-r--r--   0        0        0      415 2022-11-26 19:57:26.309000 tina4_python-0.1.8/tina4_python/public/errors/404.twig
--rw-r--r--   0        0        0     1150 2022-11-25 14:23:51.859000 tina4_python-0.1.8/tina4_python/public/favicon.ico
--rw-r--r--   0        0        0    71422 2022-11-25 14:23:51.861000 tina4_python-0.1.8/tina4_python/public/images/403.png
--rw-r--r--   0        0        0    68538 2022-11-25 14:23:51.862000 tina4_python-0.1.8/tina4_python/public/images/404.png
--rw-r--r--   0        0        0    31844 2022-11-25 14:23:51.863000 tina4_python-0.1.8/tina4_python/public/images/logo.png
--rw-r--r--   0        0        0     6251 2022-11-26 20:31:45.751667 tina4_python-0.1.8/tina4_python/Router.py
--rw-r--r--   0        0        0      327 2022-11-25 14:23:51.866002 tina4_python-0.1.8/tina4_python/Template.py
--rw-r--r--   0        0        0     1848 2022-11-26 20:27:08.455481 tina4_python-0.1.8/tina4_python/Webserver.py
--rw-r--r--   0        0        0      847 1970-01-01 00:00:00.000000 tina4_python-0.1.8/setup.py
--rw-r--r--   0        0        0      488 1970-01-01 00:00:00.000000 tina4_python-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      485 2022-12-02 00:36:11.317173 tina4_python-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     2705 2022-12-02 00:26:45.717063 tina4_python-0.1.9/tina4_python/__init__.py
+-rw-r--r--   0        0        0      586 2022-11-25 19:59:18.456107 tina4_python-0.1.9/tina4_python/Constant.py
+-rw-r--r--   0        0        0      397 2022-11-25 14:23:51.866002 tina4_python-0.1.9/tina4_python/Debug.py
+-rw-r--r--   0        0        0      614 2022-12-02 00:35:53.838155 tina4_python-0.1.9/tina4_python/Env.py
+-rw-r--r--   0        0        0      459 2022-11-26 19:57:26.301000 tina4_python-0.1.9/tina4_python/public/errors/403.twig
+-rw-r--r--   0        0        0      415 2022-11-26 19:57:26.309000 tina4_python-0.1.9/tina4_python/public/errors/404.twig
+-rw-r--r--   0        0        0     1150 2022-11-25 14:23:51.859000 tina4_python-0.1.9/tina4_python/public/favicon.ico
+-rw-r--r--   0        0        0    71422 2022-11-25 14:23:51.861000 tina4_python-0.1.9/tina4_python/public/images/403.png
+-rw-r--r--   0        0        0    68538 2022-11-25 14:23:51.862000 tina4_python-0.1.9/tina4_python/public/images/404.png
+-rw-r--r--   0        0        0    31844 2022-11-25 14:23:51.863000 tina4_python-0.1.9/tina4_python/public/images/logo.png
+-rw-r--r--   0        0        0     6251 2022-11-26 20:31:45.751667 tina4_python-0.1.9/tina4_python/Router.py
+-rw-r--r--   0        0        0      327 2022-11-25 14:23:51.866002 tina4_python-0.1.9/tina4_python/Template.py
+-rw-r--r--   0        0        0     1848 2022-11-26 20:27:08.455481 tina4_python-0.1.9/tina4_python/Webserver.py
+-rw-r--r--   0        0        0      847 1970-01-01 00:00:00.000000 tina4_python-0.1.9/setup.py
+-rw-r--r--   0        0        0      488 1970-01-01 00:00:00.000000 tina4_python-0.1.9/PKG-INFO
```

### Comparing `tina4_python-0.1.8/tina4_python/__init__.py` & `tina4_python-0.1.9/tina4_python/__init__.py`

 * *Files identical despite different names*

### Comparing `tina4_python-0.1.8/tina4_python/Constant.py` & `tina4_python-0.1.9/tina4_python/Constant.py`

 * *Files identical despite different names*

### Comparing `tina4_python-0.1.8/tina4_python/public/favicon.ico` & `tina4_python-0.1.9/tina4_python/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `tina4_python-0.1.8/tina4_python/public/images/403.png` & `tina4_python-0.1.9/tina4_python/public/images/403.png`

 * *Files identical despite different names*

### Comparing `tina4_python-0.1.8/tina4_python/public/images/404.png` & `tina4_python-0.1.9/tina4_python/public/images/404.png`

 * *Files identical despite different names*

### Comparing `tina4_python-0.1.8/tina4_python/public/images/logo.png` & `tina4_python-0.1.9/tina4_python/public/images/logo.png`

 * *Files identical despite different names*

### Comparing `tina4_python-0.1.8/tina4_python/Router.py` & `tina4_python-0.1.9/tina4_python/Router.py`

 * *Files identical despite different names*

### Comparing `tina4_python-0.1.8/tina4_python/Webserver.py` & `tina4_python-0.1.9/tina4_python/Webserver.py`

 * *Files identical despite different names*

### Comparing `tina4_python-0.1.8/setup.py` & `tina4_python-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['Jinja2>=3.0.3,<4.0.0', 'mypy>=0.991,<0.992']
 
 entry_points = \
 {'console_scripts': ['run = main:main']}
 
 setup_kwargs = {
     'name': 'tina4-python',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'Tina4Python - This is not another framework for Python',
     'long_description': 'None',
     'author': 'Andre van Zuydam',
     'author_email': 'andrevanzuydam@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

