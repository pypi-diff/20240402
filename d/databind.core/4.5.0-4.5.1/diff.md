# Comparing `tmp/databind_core-4.5.0.tar.gz` & `tmp/databind.core-4.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databind_core-4.5.0.tar", max compression
+gzip compressed data, was "databind.core-4.5.1.tar", max compression
```

## Comparing `databind_core-4.5.0.tar` & `databind.core-4.5.1.tar`

### file list

```diff
@@ -1,4 +1,5 @@
--rw-r--r--   0        0        0      157 2024-03-19 19:49:02.840669 databind_core-4.5.0/README.md
--rw-r--r--   0        0        0      814 2024-03-19 19:50:18.371219 databind_core-4.5.0/pyproject.toml
--rw-r--r--   0        0        0       54 2024-03-19 19:42:46.045907 databind_core-4.5.0/src/_databind_core_proxy.py
--rw-r--r--   0        0        0     1174 1970-01-01 00:00:00.000000 databind_core-4.5.0/PKG-INFO
+-rw-r--r--   0        0        0      157 2024-04-02 09:22:26.311231 databind.core-4.5.1/README.md
+-rw-r--r--   0        0        0      895 2024-04-02 10:02:28.523206 databind.core-4.5.1/pyproject.toml
+-rw-r--r--   0        0        0       54 2024-04-02 10:02:19.083972 databind.core-4.5.1/src/_databind_core_proxy/__init__.py
+-rw-r--r--   0        0        0     1000 2024-04-02 10:02:49.797020 databind.core-4.5.1/setup.py
+-rw-r--r--   0        0        0     1072 2024-04-02 10:02:49.797187 databind.core-4.5.1/PKG-INFO
```

### Comparing `databind_core-4.5.0/pyproject.toml` & `databind.core-4.5.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "databind.core"
-version = "4.5.0"
+version = "4.5.1"
 description = "Databind is a library inspired by jackson-databind to de-/serialize Python dataclasses. Compatible with Python 3.8 and newer. Deprecated, use `databind` package."
 authors = ["Niklas Rosenstein <rosensteinniklas@gmail.com>"]
 license = "MIT"
 readme = "README.md"
-packages = [{include = "_databind_core_proxy.py", from = "src"}]
+packages = [{include = "_databind_core_proxy", from = "src"}]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/NiklasRosenstein/python-databind/issues"
 Documentation = "https://niklasrosenstein.github.io/python-databind/"
 Repository = "https://github.com/NiklasRosenstein/python-databind"
 
 [tool.poetry.dependencies]
 python = "^3.8.0"
-databind = "^4.5.0"
-
-[tool.slap]
-typed = true
+databind = "^4.5.1"
 
 [build-system]
-requires = ["poetry-core==1.9.0"]
+requires = ["poetry-core==1.0.8"]  # Don't ugprade, see https://github.com/NiklasRosenstein/python-databind/issues/64
 build-backend = "poetry.core.masonry.api"
+
+[tool.slap]
+typed = true
```

### Comparing `databind_core-4.5.0/PKG-INFO` & `databind.core-4.5.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 Metadata-Version: 2.1
 Name: databind.core
-Version: 4.5.0
+Version: 4.5.1
 Summary: Databind is a library inspired by jackson-databind to de-/serialize Python dataclasses. Compatible with Python 3.8 and newer. Deprecated, use `databind` package.
 License: MIT
 Author: Niklas Rosenstein
 Author-email: rosensteinniklas@gmail.com
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: databind (>=4.5.0,<5.0.0)
+Requires-Dist: databind (>=4.5.1,<5.0.0)
 Project-URL: Bug Tracker, https://github.com/NiklasRosenstein/python-databind/issues
 Project-URL: Documentation, https://niklasrosenstein.github.io/python-databind/
 Project-URL: Repository, https://github.com/NiklasRosenstein/python-databind
 Description-Content-Type: text/markdown
 
 
 Deprecated since v4.5.0. This is a proxy for depending on [`databind`](https://pypi.org/project/databind/). Do not
```

