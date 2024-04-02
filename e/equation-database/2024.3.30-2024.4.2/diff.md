# Comparing `tmp/equation_database-2024.3.30.tar.gz` & `tmp/equation_database-2024.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "equation_database-2024.3.30.tar", max compression
+gzip compressed data, was "equation_database-2024.4.2.tar", max compression
```

## Comparing `equation_database-2024.3.30.tar` & `equation_database-2024.4.2.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0       20 2024-03-30 21:01:48.299405 equation_database-2024.3.30/README.md
--rw-r--r--   0        0        0        0 2024-03-30 21:01:48.299405 equation_database-2024.3.30/equation_database/__init__.py
--rw-r--r--   0        0        0     2016 2024-03-30 22:29:25.673432 equation_database-2024.3.30/equation_database/arxiv_2202_13416/__init__.py
--rw-r--r--   0        0        0     1129 2024-03-30 22:29:25.673432 equation_database-2024.3.30/equation_database/doi_10_1103_physrev_176_1700/__init__.py
--rw-r--r--   0        0        0      718 2024-03-31 16:08:15.816482 equation_database-2024.3.30/equation_database/isbn_9780471887416/__init__.py
--rw-r--r--   0        0        0     1312 2024-03-31 16:09:24.487419 equation_database-2024.3.30/equation_database/isbn_9780511628788/__init__.py
--rw-r--r--   0        0        0        0 2024-03-30 21:01:48.299405 equation_database-2024.3.30/equation_database/util/__init__.py
--rw-r--r--   0        0        0      160 2024-03-30 22:29:25.673432 equation_database-2024.3.30/equation_database/util/parse.py
--rw-r--r--   0        0        0      215 2024-03-30 21:01:48.299405 equation_database-2024.3.30/equation_database/util/test.py
--rw-r--r--   0        0        0     1205 2024-03-30 22:39:26.174706 equation_database-2024.3.30/pyproject.toml
--rw-r--r--   0        0        0      591 1970-01-01 00:00:00.000000 equation_database-2024.3.30/PKG-INFO
+-rw-r--r--   0        0        0       20 2024-02-14 12:21:18.519559 equation_database-2024.4.2/README.md
+-rw-r--r--   0        0        0        0 2024-02-14 09:32:51.317408 equation_database-2024.4.2/equation_database/__init__.py
+-rw-r--r--   0        0        0     2016 2024-04-02 11:59:32.130176 equation_database-2024.4.2/equation_database/arxiv_2202_13416/__init__.py
+-rw-r--r--   0        0        0     1129 2024-04-02 11:59:32.130176 equation_database-2024.4.2/equation_database/doi_10_1103_physrev_176_1700/__init__.py
+-rw-r--r--   0        0        0      860 2024-04-02 13:26:17.722741 equation_database-2024.4.2/equation_database/isbn_9780201483628/__init__.py
+-rw-r--r--   0        0        0      718 2024-04-02 11:59:32.133509 equation_database-2024.4.2/equation_database/isbn_9780471887416/__init__.py
+-rw-r--r--   0        0        0     1312 2024-04-02 11:59:32.133509 equation_database-2024.4.2/equation_database/isbn_9780511628788/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-14 16:20:12.281714 equation_database-2024.4.2/equation_database/util/__init__.py
+-rw-r--r--   0        0        0      160 2024-04-02 11:59:32.133509 equation_database-2024.4.2/equation_database/util/parse.py
+-rw-r--r--   0        0        0      215 2024-02-14 16:52:11.751104 equation_database-2024.4.2/equation_database/util/test.py
+-rw-r--r--   0        0        0     1204 2024-04-02 13:27:12.132685 equation_database-2024.4.2/pyproject.toml
+-rw-r--r--   0        0        0      590 1970-01-01 00:00:00.000000 equation_database-2024.4.2/PKG-INFO
```

### Comparing `equation_database-2024.3.30/equation_database/arxiv_2202_13416/__init__.py` & `equation_database-2024.4.2/equation_database/arxiv_2202_13416/__init__.py`

 * *Files identical despite different names*

### Comparing `equation_database-2024.3.30/equation_database/doi_10_1103_physrev_176_1700/__init__.py` & `equation_database-2024.4.2/equation_database/doi_10_1103_physrev_176_1700/__init__.py`

 * *Files identical despite different names*

### Comparing `equation_database-2024.3.30/equation_database/isbn_9780471887416/__init__.py` & `equation_database-2024.4.2/equation_database/isbn_9780471887416/__init__.py`

 * *Files identical despite different names*

### Comparing `equation_database-2024.3.30/equation_database/isbn_9780511628788/__init__.py` & `equation_database-2024.4.2/equation_database/isbn_9780511628788/__init__.py`

 * *Files identical despite different names*

### Comparing `equation_database-2024.3.30/pyproject.toml` & `equation_database-2024.4.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "equation-database"
-version = "2024.3.30"
+version = "2024.4.2"
 description = "A collection of equations"
 authors = ["Alexander Puck Neuwirth <alexander@neuwirth-informatik.de>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 sympy = "*"
```

### Comparing `equation_database-2024.3.30/PKG-INFO` & `equation_database-2024.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: equation-database
-Version: 2024.3.30
+Version: 2024.4.2
 Summary: A collection of equations
 Author: Alexander Puck Neuwirth
 Author-email: alexander@neuwirth-informatik.de
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

