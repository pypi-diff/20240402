# Comparing `tmp/gepref_text-0.1.1.tar.gz` & `tmp/gepref_text-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gepref_text-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "gepref_text-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gepref_text-0.1.1.tar` & `gepref_text-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,30 @@
--rwxr-xr-x   0        0        0      151 2024-03-27 19:14:54.371535 gepref_text-0.1.1/.cicd/scripts.sh
--rw-r--r--   0        0        0      445 2024-03-27 19:14:54.371535 gepref_text-0.1.1/.github/workflows/cd.yml
--rw-r--r--   0        0        0      364 2024-03-27 19:14:54.371535 gepref_text-0.1.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0      101 2024-03-27 19:14:54.371535 gepref_text-0.1.1/.gitignore
--rw-r--r--   0        0        0        7 2024-03-27 19:14:54.371535 gepref_text-0.1.1/.python-version
--rw-r--r--   0        0        0     1086 2024-03-27 19:14:54.371535 gepref_text-0.1.1/LICENSE
--rw-r--r--   0        0        0      284 2024-03-27 19:14:54.371535 gepref_text-0.1.1/Makefile
--rw-r--r--   0        0        0      256 2024-03-27 19:14:54.371535 gepref_text-0.1.1/README.md
--rw-r--r--   0        0        0      568 2024-03-27 19:14:54.375535 gepref_text-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-27 19:14:54.375535 gepref_text-0.1.1/src/gepref_text/__init__.py
--rw-r--r--   0        0        0      525 2024-03-27 19:14:54.375535 gepref_text-0.1.1/src/gepref_text/base.py
--rw-r--r--   0        0        0     1898 2024-03-27 19:14:54.375535 gepref_text-0.1.1/src/gepref_text/normalization.py
--rw-r--r--   0        0        0        0 2024-03-27 19:14:54.375535 gepref_text-0.1.1/src/gepref_text/py.typed
--rw-r--r--   0        0        0     3374 2024-03-27 19:14:54.375535 gepref_text-0.1.1/src/gepref_text/regex.py
--rw-r--r--   0        0        0     1300 2024-03-27 19:14:54.375535 gepref_text-0.1.1/test/test_normalization.py
--rw-r--r--   0        0        0     2109 2024-03-27 19:14:54.375535 gepref_text-0.1.1/test/test_regex.py
--rw-r--r--   0        0        0      471 1970-01-01 00:00:00.000000 gepref_text-0.1.1/PKG-INFO
+-rwxr-xr-x   0        0        0      243 2024-04-02 01:40:27.699357 gepref_text-0.1.2/.cicd/scripts.sh
+-rw-r--r--   0        0        0      980 2024-04-02 01:40:27.699357 gepref_text-0.1.2/.github/workflows/cd.yml
+-rw-r--r--   0        0        0      364 2024-04-02 01:40:27.699357 gepref_text-0.1.2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      126 2024-04-02 01:40:27.699357 gepref_text-0.1.2/.gitignore
+-rw-r--r--   0        0        0        7 2024-04-02 01:40:27.699357 gepref_text-0.1.2/.python-version
+-rw-r--r--   0        0        0     1086 2024-04-02 01:40:27.703357 gepref_text-0.1.2/LICENSE
+-rw-r--r--   0        0        0      427 2024-04-02 01:40:27.703357 gepref_text-0.1.2/Makefile
+-rw-r--r--   0        0        0      528 2024-04-02 01:40:27.703357 gepref_text-0.1.2/README.md
+-rw-r--r--   0        0        0      638 2024-04-02 01:40:27.703357 gepref_text-0.1.2/doc/Makefile
+-rw-r--r--   0        0        0    12449 2024-04-02 01:40:27.703357 gepref_text-0.1.2/doc/source/_static/gepref_text.svg
+-rw-r--r--   0        0        0    20860 2024-04-02 01:40:27.703357 gepref_text-0.1.2/doc/source/_static/preprocessor.svg
+-rw-r--r--   0        0        0      764 2024-04-02 01:40:27.703357 gepref_text-0.1.2/doc/source/conf.py
+-rw-r--r--   0        0        0      628 2024-04-02 01:40:27.703357 gepref_text-0.1.2/doc/source/gepref_text.rst
+-rw-r--r--   0        0        0      521 2024-04-02 01:40:27.703357 gepref_text-0.1.2/doc/source/index.rst
+-rw-r--r--   0        0        0      251 2024-04-02 01:40:27.703357 gepref_text-0.1.2/doc/source/installation.md
+-rw-r--r--   0        0        0       70 2024-04-02 01:40:27.703357 gepref_text-0.1.2/doc/source/modules.rst
+-rw-r--r--   0        0        0      986 2024-04-02 01:40:27.703357 gepref_text-0.1.2/doc/source/usage.rst
+-rw-r--r--   0        0        0     1321 2024-04-02 01:40:27.703357 gepref_text-0.1.2/doc/source/usage/custom.md
+-rw-r--r--   0        0        0      952 2024-04-02 01:40:27.703357 gepref_text-0.1.2/doc/source/usage/normalization.md
+-rw-r--r--   0        0        0      744 2024-04-02 01:40:27.703357 gepref_text-0.1.2/doc/source/usage/preprocessor.md
+-rw-r--r--   0        0        0     1507 2024-04-02 01:40:27.703357 gepref_text-0.1.2/doc/source/usage/regex.md
+-rw-r--r--   0        0        0      615 2024-04-02 01:40:27.703357 gepref_text-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-02 01:40:27.703357 gepref_text-0.1.2/src/gepref_text/__init__.py
+-rw-r--r--   0        0        0      525 2024-04-02 01:40:27.703357 gepref_text-0.1.2/src/gepref_text/base.py
+-rw-r--r--   0        0        0     1898 2024-04-02 01:40:27.703357 gepref_text-0.1.2/src/gepref_text/normalization.py
+-rw-r--r--   0        0        0        0 2024-04-02 01:40:27.703357 gepref_text-0.1.2/src/gepref_text/py.typed
+-rw-r--r--   0        0        0     3374 2024-04-02 01:40:27.703357 gepref_text-0.1.2/src/gepref_text/regex.py
+-rw-r--r--   0        0        0     1300 2024-04-02 01:40:27.703357 gepref_text-0.1.2/test/test_normalization.py
+-rw-r--r--   0        0        0     2109 2024-04-02 01:40:27.703357 gepref_text-0.1.2/test/test_regex.py
+-rw-r--r--   0        0        0      604 1970-01-01 00:00:00.000000 gepref_text-0.1.2/PKG-INFO
```

### Comparing `gepref_text-0.1.1/LICENSE` & `gepref_text-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gepref_text-0.1.1/pyproject.toml` & `gepref_text-0.1.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gepref_text"
-version = "0.1.1"
+version = "0.1.2"
 description = "GEneral PREprocessing Framework for TEXT (gepref_text)"
 authors = [{name="Juan Lara", email="julara@unal.edu.co"}]
 requires-python = ">3.10"
 dependencies = [
 	"gepref==0.1.1",
 	"unidecode==1.3.8"
 ]
 
 [project.optional-dependencies]
 dev = [
-	"jedi-language-server", "mypy", "pytest", "ruff", "flit"
+	"jedi-language-server", "mypy", "pytest", "ruff", "flit",
+	"sphinx", "sphinx-book-theme", "myst_parser"
 ]
 
 [tool.setuptools.packages.find]
 where = ["src/"]
 
 [tool.setuptools.package-data]
 pkgname = ["py.typed"]
```

### Comparing `gepref_text-0.1.1/src/gepref_text/base.py` & `gepref_text-0.1.2/src/gepref_text/base.py`

 * *Files identical despite different names*

### Comparing `gepref_text-0.1.1/src/gepref_text/normalization.py` & `gepref_text-0.1.2/src/gepref_text/normalization.py`

 * *Files identical despite different names*

### Comparing `gepref_text-0.1.1/src/gepref_text/regex.py` & `gepref_text-0.1.2/src/gepref_text/regex.py`

 * *Files identical despite different names*

### Comparing `gepref_text-0.1.1/test/test_normalization.py` & `gepref_text-0.1.2/test/test_normalization.py`

 * *Files identical despite different names*

### Comparing `gepref_text-0.1.1/test/test_regex.py` & `gepref_text-0.1.2/test/test_regex.py`

 * *Files identical despite different names*

