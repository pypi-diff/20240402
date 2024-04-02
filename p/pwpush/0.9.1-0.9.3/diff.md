# Comparing `tmp/pwpush-0.9.1.tar.gz` & `tmp/pwpush-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwpush-0.9.1.tar", max compression
+gzip compressed data, was "pwpush-0.9.3.tar", max compression
```

## Comparing `pwpush-0.9.1.tar` & `pwpush-0.9.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1071 2021-08-20 21:05:30.110732 pwpush-0.9.1/LICENSE
--rw-r--r--   0        0        0     9702 2023-07-24 21:59:40.082265 pwpush-0.9.1/README.md
--rw-r--r--   0        0        0      432 2021-08-20 21:05:30.088281 pwpush-0.9.1/pwpush/__init__.py
--rw-r--r--   0        0        0    11811 2023-07-24 21:40:38.881003 pwpush-0.9.1/pwpush/__main__.py
--rw-r--r--   0        0        0     4821 2022-08-31 08:14:28.718237 pwpush-0.9.1/pwpush/commands/config.py
--rw-r--r--   0        0        0     3224 2022-11-14 09:47:14.551927 pwpush-0.9.1/pwpush/options.py
--rw-r--r--   0        0        0        0 2021-08-20 21:05:30.091678 pwpush-0.9.1/pwpush/py.typed
--rw-r--r--   0        0        0     3135 2023-07-24 21:59:42.296319 pwpush-0.9.1/pyproject.toml
--rw-r--r--   0        0        0    10843 1970-01-01 00:00:00.000000 pwpush-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2021-08-20 21:05:30.110732 pwpush-0.9.3/LICENSE
+-rw-r--r--   0        0        0     9702 2023-07-24 21:59:40.082265 pwpush-0.9.3/README.md
+-rw-r--r--   0        0        0      432 2021-08-20 21:05:30.088281 pwpush-0.9.3/pwpush/__init__.py
+-rw-r--r--   0        0        0    11811 2023-07-24 21:40:38.881003 pwpush-0.9.3/pwpush/__main__.py
+-rw-r--r--   0        0        0     4821 2022-08-31 08:14:28.718237 pwpush-0.9.3/pwpush/commands/config.py
+-rw-r--r--   0        0        0     3224 2022-11-14 09:47:14.551927 pwpush-0.9.3/pwpush/options.py
+-rw-r--r--   0        0        0        0 2021-08-20 21:05:30.091678 pwpush-0.9.3/pwpush/py.typed
+-rw-r--r--   0        0        0     3135 2023-07-25 07:14:08.755716 pwpush-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0    10843 1970-01-01 00:00:00.000000 pwpush-0.9.3/PKG-INFO
```

### Comparing `pwpush-0.9.1/LICENSE` & `pwpush-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pwpush-0.9.1/README.md` & `pwpush-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `pwpush-0.9.1/pwpush/__main__.py` & `pwpush-0.9.3/pwpush/__main__.py`

 * *Files identical despite different names*

### Comparing `pwpush-0.9.1/pwpush/commands/config.py` & `pwpush-0.9.3/pwpush/commands/config.py`

 * *Files identical despite different names*

### Comparing `pwpush-0.9.1/pwpush/options.py` & `pwpush-0.9.3/pwpush/options.py`

 * *Files identical despite different names*

### Comparing `pwpush-0.9.1/pyproject.toml` & `pwpush-0.9.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pwpush"
-version = "0.9.1"
+version = "0.9.3"
 description = "Command Line Interface to Password Pusher."
 readme = "README.md"
 authors = ["pwpush <pglombardo@hey.com>"]
 license = "MIT"
 repository = "https://github.com/pglombardo/pwpush"
 homepage = "https://github.com/pglombardo/pwpush"
```

### Comparing `pwpush-0.9.1/PKG-INFO` & `pwpush-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwpush
-Version: 0.9.1
+Version: 0.9.3
 Summary: Command Line Interface to Password Pusher.
 Home-page: https://github.com/pglombardo/pwpush
 License: MIT
 Author: pwpush
 Author-email: pglombardo@hey.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
```

