# Comparing `tmp/pymetasnap-0.30.0.tar.gz` & `tmp/pymetasnap-0.30.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymetasnap-0.30.0.tar", max compression
+gzip compressed data, was "pymetasnap-0.30.1.tar", max compression
```

## Comparing `pymetasnap-0.30.0.tar` & `pymetasnap-0.30.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1073 2024-04-02 00:30:02.295126 pymetasnap-0.30.0/LICENSE
--rw-r--r--   0        0        0     3043 2024-04-02 00:30:02.295126 pymetasnap-0.30.0/README.md
--rw-r--r--   0        0        0        0 2024-04-02 00:30:02.295126 pymetasnap-0.30.0/extractor/__init__.py
--rw-r--r--   0        0        0     3678 2024-04-02 00:30:02.295126 pymetasnap-0.30.0/extractor/checks.py
--rw-r--r--   0        0        0     7141 2024-04-02 00:30:02.295126 pymetasnap-0.30.0/extractor/core.py
--rw-r--r--   0        0        0      227 2024-04-02 00:30:02.295126 pymetasnap-0.30.0/extractor/logger.py
--rw-r--r--   0        0        0     1345 2024-04-02 00:30:02.295126 pymetasnap-0.30.0/extractor/main.py
--rw-r--r--   0        0        0     3262 2024-04-02 00:30:02.295126 pymetasnap-0.30.0/extractor/render.py
--rw-r--r--   0        0        0      908 2024-04-02 00:30:02.295126 pymetasnap-0.30.0/pyproject.toml
--rw-r--r--   0        0        0     4050 1970-01-01 00:00:00.000000 pymetasnap-0.30.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-02 00:38:58.710910 pymetasnap-0.30.1/LICENSE
+-rw-r--r--   0        0        0     3043 2024-04-02 00:38:58.710910 pymetasnap-0.30.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-02 00:38:58.710910 pymetasnap-0.30.1/extractor/__init__.py
+-rw-r--r--   0        0        0     3678 2024-04-02 00:38:58.714910 pymetasnap-0.30.1/extractor/checks.py
+-rw-r--r--   0        0        0     7141 2024-04-02 00:38:58.714910 pymetasnap-0.30.1/extractor/core.py
+-rw-r--r--   0        0        0      227 2024-04-02 00:38:58.714910 pymetasnap-0.30.1/extractor/logger.py
+-rw-r--r--   0        0        0     1345 2024-04-02 00:38:58.714910 pymetasnap-0.30.1/extractor/main.py
+-rw-r--r--   0        0        0     3262 2024-04-02 00:38:58.714910 pymetasnap-0.30.1/extractor/render.py
+-rw-r--r--   0        0        0      921 2024-04-02 00:38:58.714910 pymetasnap-0.30.1/pyproject.toml
+-rw-r--r--   0        0        0     4050 1970-01-01 00:00:00.000000 pymetasnap-0.30.1/PKG-INFO
```

### Comparing `pymetasnap-0.30.0/LICENSE` & `pymetasnap-0.30.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymetasnap-0.30.0/README.md` & `pymetasnap-0.30.1/README.md`

 * *Files identical despite different names*

### Comparing `pymetasnap-0.30.0/extractor/checks.py` & `pymetasnap-0.30.1/extractor/checks.py`

 * *Files identical despite different names*

### Comparing `pymetasnap-0.30.0/extractor/core.py` & `pymetasnap-0.30.1/extractor/core.py`

 * *Files identical despite different names*

### Comparing `pymetasnap-0.30.0/extractor/main.py` & `pymetasnap-0.30.1/extractor/main.py`

 * *Files identical despite different names*

### Comparing `pymetasnap-0.30.0/extractor/render.py` & `pymetasnap-0.30.1/extractor/render.py`

 * *Files identical despite different names*

### Comparing `pymetasnap-0.30.0/pyproject.toml` & `pymetasnap-0.30.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pymetasnap"
-version = "0.30.0"
+version = "0.30.1"
 description = "This package allows you to scrape metadata from the Python Package Index"
 authors = ["cristian-rincon <cristian.o.rincon.b@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "extractor"}]
 
 [tool.poetry.scripts]
@@ -20,16 +20,16 @@
 loguru = "^0.7.0"
 requests = "^2.31.0"
 toml = "^0.10.2"
 ghapi = "^1.0.4"
 
 
 [tool.poetry.group.dev.dependencies]
-black = {version = "^23.3.0", allow-prereleases = true}
-pytest = "^7.3.1"
+black = {version = ">=23.3,<25.0", allow-prereleases = true}
+pytest = ">=7.3.1,<9.0.0"
 pre-commit = "^3.3.2"
 jupyterlab = "^4.0.2"
 pytest-xdist = "^3.3.1"
 pytest-sugar = ">=0.9.7,<1.1.0"
 pytest-cov = "^4.1.0"
 
 [build-system]
```

### Comparing `pymetasnap-0.30.0/PKG-INFO` & `pymetasnap-0.30.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymetasnap
-Version: 0.30.0
+Version: 0.30.1
 Summary: This package allows you to scrape metadata from the Python Package Index
 License: MIT
 Author: cristian-rincon
 Author-email: cristian.o.rincon.b@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

