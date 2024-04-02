# Comparing `tmp/py_aiger_bdd-3.1.2.tar.gz` & `tmp/py_aiger_bdd-3.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_aiger_bdd-3.1.2.tar", max compression
+gzip compressed data, was "py_aiger_bdd-3.1.3.tar", max compression
```

## Comparing `py_aiger_bdd-3.1.2.tar` & `py_aiger_bdd-3.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1082 2024-03-16 20:13:53.066933 py_aiger_bdd-3.1.2/LICENSE
--rw-r--r--   0        0        0     1168 2024-03-16 20:13:53.066933 py_aiger_bdd-3.1.2/README.md
--rw-r--r--   0        0        0       76 2024-03-16 20:13:53.066933 py_aiger_bdd-3.1.2/aiger_bdd/__init__.py
--rw-r--r--   0        0        0     3148 2024-03-16 20:13:53.066933 py_aiger_bdd-3.1.2/aiger_bdd/bdd.py
--rw-r--r--   0        0        0     1627 2024-03-16 20:13:53.066933 py_aiger_bdd-3.1.2/aiger_bdd/test_bdd.py
--rw-r--r--   0        0        0      713 2024-03-16 20:16:19.050878 py_aiger_bdd-3.1.2/pyproject.toml
--rw-r--r--   0        0        0     2101 1970-01-01 00:00:00.000000 py_aiger_bdd-3.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1082 2024-03-16 20:13:53.066933 py_aiger_bdd-3.1.3/LICENSE
+-rw-r--r--   0        0        0     1168 2024-03-16 20:13:53.066933 py_aiger_bdd-3.1.3/README.md
+-rw-r--r--   0        0        0       76 2024-03-16 20:13:53.066933 py_aiger_bdd-3.1.3/aiger_bdd/__init__.py
+-rw-r--r--   0        0        0     3148 2024-03-16 20:13:53.066933 py_aiger_bdd-3.1.3/aiger_bdd/bdd.py
+-rw-r--r--   0        0        0     1627 2024-03-16 20:13:53.066933 py_aiger_bdd-3.1.3/aiger_bdd/test_bdd.py
+-rw-r--r--   0        0        0      714 2024-04-02 03:01:59.362392 py_aiger_bdd-3.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1901 1970-01-01 00:00:00.000000 py_aiger_bdd-3.1.3/PKG-INFO
```

### Comparing `py_aiger_bdd-3.1.2/LICENSE` & `py_aiger_bdd-3.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `py_aiger_bdd-3.1.2/README.md` & `py_aiger_bdd-3.1.3/README.md`

 * *Files identical despite different names*

### Comparing `py_aiger_bdd-3.1.2/aiger_bdd/bdd.py` & `py_aiger_bdd-3.1.3/aiger_bdd/bdd.py`

 * *Files identical despite different names*

### Comparing `py_aiger_bdd-3.1.2/aiger_bdd/test_bdd.py` & `py_aiger_bdd-3.1.3/aiger_bdd/test_bdd.py`

 * *Files identical despite different names*

### Comparing `py_aiger_bdd-3.1.2/pyproject.toml` & `py_aiger_bdd-3.1.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "py-aiger-bdd"
 readme="README.md"
-version = "3.1.2"
+version = "3.1.3"
 repository = "https://github.com/mvcisback/py-aiger-bdd"
 description = "Aiger to BDD bridge."
 authors = ["Marcell Vazquez-Chanlatte <mvc@linux.com>"]
 license = "MIT"
 packages = [
     { include = "aiger_bdd" },
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.11"
 attrs = ">=22"
 bidict = "^0.22.0"
 funcy = "^1.12"
 py-aiger = "^6.0.0"
-dd = "^0.5.4"
+dd = "^0.6.0"
 
 [tool.poetry.dev-dependencies]
 pytest-xdist = "^3"
 hypothesis = "^6"
 hypothesis_cfg = {git = "https://github.com/mvcisback/hypothesis-cfg.git"}
 py-aiger-bv = "^4.0.0"
 py-aiger-ptltl = "^3.0.0"
```

