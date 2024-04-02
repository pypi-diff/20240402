# Comparing `tmp/orderings-1.3.2.tar.gz` & `tmp/orderings-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orderings-1.3.2.tar", max compression
+gzip compressed data, was "orderings-1.4.0.tar", max compression
```

## Comparing `orderings-1.3.2.tar` & `orderings-1.4.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1092 2024-03-17 12:29:33.280384 orderings-1.3.2/LICENSE
--rw-r--r--   0        0        0     4388 2024-03-17 12:29:33.280384 orderings-1.3.2/README.md
--rw-r--r--   0        0        0      657 2024-03-17 12:29:33.280384 orderings-1.3.2/orderings/__init__.py
--rw-r--r--   0        0        0     4015 2024-03-17 12:29:33.280384 orderings-1.3.2/orderings/core.py
--rw-r--r--   0        0        0        0 2024-03-17 12:29:33.280384 orderings-1.3.2/orderings/py.typed
--rw-r--r--   0        0        0     1931 2024-03-17 12:29:33.280384 orderings-1.3.2/orderings/typing.py
--rw-r--r--   0        0        0     2557 2024-03-17 12:29:33.280384 orderings-1.3.2/pyproject.toml
--rw-r--r--   0        0        0     5582 1970-01-01 00:00:00.000000 orderings-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1092 2024-04-02 11:49:45.330667 orderings-1.4.0/LICENSE
+-rw-r--r--   0        0        0     4388 2024-04-02 11:49:45.330667 orderings-1.4.0/README.md
+-rw-r--r--   0        0        0     1006 2024-04-02 11:49:45.334667 orderings-1.4.0/orderings/__init__.py
+-rw-r--r--   0        0        0     4015 2024-04-02 11:49:45.334667 orderings-1.4.0/orderings/core.py
+-rw-r--r--   0        0        0        0 2024-04-02 11:49:45.334667 orderings-1.4.0/orderings/py.typed
+-rw-r--r--   0        0        0     4066 2024-04-02 11:49:45.334667 orderings-1.4.0/orderings/typing.py
+-rw-r--r--   0        0        0     2558 2024-04-02 11:49:45.334667 orderings-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     5583 1970-01-01 00:00:00.000000 orderings-1.4.0/PKG-INFO
```

### Comparing `orderings-1.3.2/LICENSE` & `orderings-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `orderings-1.3.2/README.md` & `orderings-1.4.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 $ poetry add orderings
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-orderings = "^1.3.2"
+orderings = "^1.4.0"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.orderings]
 git = "https://github.com/nekitdev/orderings.git"
```

### Comparing `orderings-1.3.2/orderings/core.py` & `orderings-1.4.0/orderings/core.py`

 * *Files identical despite different names*

### Comparing `orderings-1.3.2/pyproject.toml` & `orderings-1.4.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "orderings"
-version = "1.3.2"
+version = "1.4.0"
 description = "Ordering enumeration and protocols."
 authors = ["nekitdev"]
 license = "MIT"
 
 readme = "README.md"
 
 homepage = "https://github.com/nekitdev/orderings"
@@ -28,15 +28,15 @@
 
 [[tool.poetry.packages]]
 include = "orderings"
 
 [tool.poetry.dependencies]
 python = ">= 3.8"
 
-typing-aliases = ">= 1.8.0"
+typing-aliases = ">= 1.10.0"
 typing-extensions = ">= 4.10.0"
 
 [tool.poetry.group.format.dependencies]
 ruff = "0.3.3"
 
 [tool.poetry.group.check.dependencies]
 mypy = "1.9.0"
@@ -100,15 +100,15 @@
 directory = "coverage"
 
 [tool.mypy]
 strict = true
 
 [tool.changelogging]
 name = "orderings"
-version = "1.3.2"
+version = "1.4.0"
 url = "https://github.com/nekitdev/orderings"
 directory = "changes"
 output = "CHANGELOG.md"
 
 start_string = "<!-- changelogging: start -->"
 
 title_format = "{version} ({date})"
```

### Comparing `orderings-1.3.2/PKG-INFO` & `orderings-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orderings
-Version: 1.3.2
+Version: 1.4.0
 Summary: Ordering enumeration and protocols.
 Home-page: https://github.com/nekitdev/orderings
 License: MIT
 Keywords: python,ordering
 Author: nekitdev
 Requires-Python: >=3.8
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
-Requires-Dist: typing-aliases (>=1.8.0)
+Requires-Dist: typing-aliases (>=1.10.0)
 Requires-Dist: typing-extensions (>=4.10.0)
 Project-URL: Chat, https://nekit.dev/chat
 Project-URL: Documentation, https://nekitdev.github.io/orderings
 Project-URL: Funding, https://nekit.dev/funding
 Project-URL: Issues, https://github.com/nekitdev/orderings/issues
 Project-URL: Repository, https://github.com/nekitdev/orderings
 Description-Content-Type: text/markdown
@@ -70,15 +70,15 @@
 $ poetry add orderings
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-orderings = "^1.3.2"
+orderings = "^1.4.0"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.orderings]
 git = "https://github.com/nekitdev/orderings.git"
```

