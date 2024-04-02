# Comparing `tmp/pyhashlookup-1.2.2.tar.gz` & `tmp/pyhashlookup-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhashlookup-1.2.2.tar", max compression
+gzip compressed data, was "pyhashlookup-1.2.3.tar", max compression
```

## Comparing `pyhashlookup-1.2.2.tar` & `pyhashlookup-1.2.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35149 2021-06-18 19:49:34.740477 pyhashlookup-1.2.2/LICENSE
--rw-r--r--   0        0        0      616 2021-11-29 09:20:30.563272 pyhashlookup-1.2.2/README.md
--rw-r--r--   0        0        0     1018 2024-02-06 08:15:40.972001 pyhashlookup-1.2.2/pyhashlookup/__init__.py
--rw-r--r--   0        0        0     5106 2024-02-06 08:22:36.586010 pyhashlookup-1.2.2/pyhashlookup/api.py
--rw-r--r--   0        0        0        0 2021-06-18 17:37:37.866733 pyhashlookup-1.2.2/pyhashlookup/py.typed
--rw-r--r--   0        0        0     1501 2024-02-06 08:23:39.434310 pyhashlookup-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     2059 1970-01-01 00:00:00.000000 pyhashlookup-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-02 13:42:43.669783 pyhashlookup-1.2.3/LICENSE
+-rw-r--r--   0        0        0      616 2024-04-02 13:42:43.669783 pyhashlookup-1.2.3/README.md
+-rw-r--r--   0        0        0     1018 2024-04-02 13:42:43.669783 pyhashlookup-1.2.3/pyhashlookup/__init__.py
+-rw-r--r--   0        0        0     5106 2024-04-02 13:42:43.673783 pyhashlookup-1.2.3/pyhashlookup/api.py
+-rw-r--r--   0        0        0        0 2024-04-02 13:42:43.673783 pyhashlookup-1.2.3/pyhashlookup/py.typed
+-rw-r--r--   0        0        0     1501 2024-04-02 13:42:43.673783 pyhashlookup-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0     2059 1970-01-01 00:00:00.000000 pyhashlookup-1.2.3/PKG-INFO
```

### Comparing `pyhashlookup-1.2.2/LICENSE` & `pyhashlookup-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhashlookup-1.2.2/README.md` & `pyhashlookup-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `pyhashlookup-1.2.2/pyhashlookup/__init__.py` & `pyhashlookup-1.2.3/pyhashlookup/__init__.py`

 * *Files identical despite different names*

### Comparing `pyhashlookup-1.2.2/pyhashlookup/api.py` & `pyhashlookup-1.2.3/pyhashlookup/api.py`

 * *Files identical despite different names*

### Comparing `pyhashlookup-1.2.2/pyproject.toml` & `pyhashlookup-1.2.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyhashlookup"
-version = "1.2.2"
+version = "1.2.3"
 description = "Python CLI and module for CIRCL hash lookup"
 authors = ["Raphaël Vinot <raphael.vinot@circl.lu>"]
 license = "BSD-3-Clause"
 repository = "https://github.com/hashlookup/PyHashlookup"
 documentation = "https://pyhashlookup.readthedocs.io/en/latest/"
 
 readme = "README.md"
@@ -28,25 +28,25 @@
 ]
 
 [tool.poetry.scripts]
 hashlookup = 'pyhashlookup:main'
 
 [tool.poetry.dependencies]
 python = "^3.8"
-dnspython = "^2.5.0"
+dnspython = "^2.6.1"
 requests = "^2.31.0"
 Sphinx = [
     {version = "<7.2", python = "<3.9", optional = true},
     {version = "^7.2", python = ">=3.9", optional = true}
 ]
 
 [tool.poetry.dev-dependencies]
-mypy = "^1.8.0"
-types-requests = "^2.31.0.20240125"
-pytest-cov = "^4.1.0"
+mypy = "^1.9.0"
+types-requests = "^2.31.0.20240402"
+pytest-cov = "^5.0.0"
 
 [tool.poetry.extras]
 docs = ["Sphinx"]
 
 [build-system]
 requires = ["poetry_core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pyhashlookup-1.2.2/PKG-INFO` & `pyhashlookup-1.2.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhashlookup
-Version: 1.2.2
+Version: 1.2.3
 Summary: Python CLI and module for CIRCL hash lookup
 Home-page: https://github.com/hashlookup/PyHashlookup
 License: BSD-3-Clause
 Author: Raphaël Vinot
 Author-email: raphael.vinot@circl.lu
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -21,15 +21,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet
 Classifier: Topic :: Security
 Provides-Extra: docs
 Requires-Dist: Sphinx (<7.2) ; (python_version < "3.9") and (extra == "docs")
 Requires-Dist: Sphinx (>=7.2,<8.0) ; (python_version >= "3.9") and (extra == "docs")
-Requires-Dist: dnspython (>=2.5.0,<3.0.0)
+Requires-Dist: dnspython (>=2.6.1,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Documentation, https://pyhashlookup.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/hashlookup/PyHashlookup
 Description-Content-Type: text/markdown
 
 [![Documentation Status](https://readthedocs.org/projects/pyhashlookup/badge/?version=latest)](https://pyhashlookup.readthedocs.io/en/latest/?badge=latest)
```

