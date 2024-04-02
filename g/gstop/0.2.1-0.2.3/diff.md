# Comparing `tmp/gstop-0.2.1.tar.gz` & `tmp/gstop-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gstop-0.2.1.tar", last modified: Fri Feb 23 07:29:04 2024, max compression
+gzip compressed data, was "gstop-0.2.3.tar", last modified: Tue Apr  2 01:18:16 2024, max compression
```

## Comparing `gstop-0.2.1.tar` & `gstop-0.2.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 k_ishikawa  (1004) spcl      (1001)        0 2024-02-23 07:29:04.576249 gstop-0.2.1/
--rw-r--r--   0 k_ishikawa  (1004) spcl      (1001)     1193 2024-02-23 07:29:04.572249 gstop-0.2.1/PKG-INFO
--rw-r--r--   0 k_ishikawa  (1004) spcl      (1001)      663 2024-02-22 09:33:32.000000 gstop-0.2.1/README.md
-drwxr-xr-x   0 k_ishikawa  (1004) spcl      (1001)        0 2024-02-23 07:29:04.564249 gstop-0.2.1/gstop/
--rw-r--r--   0 k_ishikawa  (1004) spcl      (1001)      179 2024-02-23 07:26:21.000000 gstop-0.2.1/gstop/__init__.py
--rw-r--r--   0 k_ishikawa  (1004) spcl      (1001)      513 2024-02-23 07:17:12.000000 gstop-0.2.1/gstop/common.py
--rw-r--r--   0 k_ishikawa  (1004) spcl      (1001)     2652 2024-02-23 07:26:03.000000 gstop-0.2.1/gstop/stopper.py
-drwxr-xr-x   0 k_ishikawa  (1004) spcl      (1001)        0 2024-02-23 07:29:04.572249 gstop-0.2.1/gstop.egg-info/
--rw-r--r--   0 k_ishikawa  (1004) spcl      (1001)     1193 2024-02-23 07:29:04.000000 gstop-0.2.1/gstop.egg-info/PKG-INFO
--rw-r--r--   0 k_ishikawa  (1004) spcl      (1001)      241 2024-02-23 07:29:04.000000 gstop-0.2.1/gstop.egg-info/SOURCES.txt
--rw-r--r--   0 k_ishikawa  (1004) spcl      (1001)        1 2024-02-23 07:29:04.000000 gstop-0.2.1/gstop.egg-info/dependency_links.txt
--rw-r--r--   0 k_ishikawa  (1004) spcl      (1001)       57 2024-02-23 07:29:04.000000 gstop-0.2.1/gstop.egg-info/requires.txt
--rw-r--r--   0 k_ishikawa  (1004) spcl      (1001)       11 2024-02-23 07:29:04.000000 gstop-0.2.1/gstop.egg-info/top_level.txt
--rw-r--r--   0 k_ishikawa  (1004) spcl      (1001)      735 2024-02-23 07:28:57.000000 gstop-0.2.1/pyproject.toml
--rw-r--r--   0 k_ishikawa  (1004) spcl      (1001)       38 2024-02-23 07:29:04.576249 gstop-0.2.1/setup.cfg
-drwxr-xr-x   0 k_ishikawa  (1004) spcl      (1001)        0 2024-02-23 07:29:04.572249 gstop-0.2.1/tests/
--rw-r--r--   0 k_ishikawa  (1004) spcl      (1001)        0 2024-02-22 09:33:32.000000 gstop-0.2.1/tests/test_stopper.py
+drwxr-xr-x   0 k_ishikawa  (1004) spcl      (1001)        0 2024-04-02 01:18:16.063651 gstop-0.2.3/
+-rw-r--r--   0 k_ishikawa  (1004) spcl      (1001)     2832 2024-04-02 01:18:16.063651 gstop-0.2.3/PKG-INFO
+-rw-r--r--   0 k_ishikawa  (1004) spcl      (1001)     2392 2024-03-26 12:12:38.000000 gstop-0.2.3/README.md
+drwxr-xr-x   0 k_ishikawa  (1004) spcl      (1001)        0 2024-04-02 01:18:16.059651 gstop-0.2.3/gstop/
+-rw-r--r--   0 k_ishikawa  (1004) spcl      (1001)      179 2024-02-23 07:26:21.000000 gstop-0.2.3/gstop/__init__.py
+-rw-r--r--   0 k_ishikawa  (1004) spcl      (1001)      772 2024-03-21 08:50:53.000000 gstop-0.2.3/gstop/common.py
+-rw-r--r--   0 k_ishikawa  (1004) spcl      (1001)     2652 2024-02-23 07:26:03.000000 gstop-0.2.3/gstop/stopper.py
+drwxr-xr-x   0 k_ishikawa  (1004) spcl      (1001)        0 2024-04-02 01:18:16.063651 gstop-0.2.3/gstop.egg-info/
+-rw-r--r--   0 k_ishikawa  (1004) spcl      (1001)     2832 2024-04-02 01:18:16.000000 gstop-0.2.3/gstop.egg-info/PKG-INFO
+-rw-r--r--   0 k_ishikawa  (1004) spcl      (1001)      241 2024-04-02 01:18:16.000000 gstop-0.2.3/gstop.egg-info/SOURCES.txt
+-rw-r--r--   0 k_ishikawa  (1004) spcl      (1001)        1 2024-04-02 01:18:16.000000 gstop-0.2.3/gstop.egg-info/dependency_links.txt
+-rw-r--r--   0 k_ishikawa  (1004) spcl      (1001)       45 2024-04-02 01:18:16.000000 gstop-0.2.3/gstop.egg-info/requires.txt
+-rw-r--r--   0 k_ishikawa  (1004) spcl      (1001)       11 2024-04-02 01:18:16.000000 gstop-0.2.3/gstop.egg-info/top_level.txt
+-rw-r--r--   0 k_ishikawa  (1004) spcl      (1001)      657 2024-04-02 01:17:47.000000 gstop-0.2.3/pyproject.toml
+-rw-r--r--   0 k_ishikawa  (1004) spcl      (1001)       38 2024-04-02 01:18:16.063651 gstop-0.2.3/setup.cfg
+drwxr-xr-x   0 k_ishikawa  (1004) spcl      (1001)        0 2024-04-02 01:18:16.063651 gstop-0.2.3/tests/
+-rw-r--r--   0 k_ishikawa  (1004) spcl      (1001)        0 2024-02-22 09:33:32.000000 gstop-0.2.3/tests/test_stopper.py
```

### Comparing `gstop-0.2.1/gstop/stopper.py` & `gstop-0.2.3/gstop/stopper.py`

 * *Files identical despite different names*

### Comparing `gstop-0.2.1/pyproject.toml` & `gstop-0.2.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -12,33 +12,26 @@
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
     "transformers",
     "torch",
+    "loguru",
 ]
-version = "0.2.1"
+version = "0.2.3"
 
 [project.optional-dependencies]
 dev = [
     "pytest",
-    "flake8",
-    "mypy",
-    "black",
-    "isort",
+    "ruff",
 ]
 
 [tool.setuptools.packages.find]
 exclude = ["tests"]
 
-[tool.black]
+[tool.ruff]
 line-length = 88
+indent-width = 4
 
-[tool.isort]
-profile = "black"
-
-[tool.flake8]
-max-line-length = 88
-
-[tool.mypy]
-ignore_missing_imports = true
+[tool.ruff.format]
+quote-style = "double"
```

