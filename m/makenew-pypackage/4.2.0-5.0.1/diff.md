# Comparing `tmp/makenew_pypackage-4.2.0.tar.gz` & `tmp/makenew_pypackage-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "makenew_pypackage-4.2.0.tar", max compression
+gzip compressed data, was "makenew_pypackage-5.0.1.tar", max compression
```

## Comparing `makenew_pypackage-4.2.0.tar` & `makenew_pypackage-5.0.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1079 2023-07-25 18:11:21.197274 makenew_pypackage-4.2.0/LICENSE.txt
--rw-r--r--   0        0        0     6865 2023-07-25 18:11:21.197274 makenew_pypackage-4.2.0/README.rst
--rw-r--r--   0        0        0       46 2023-07-25 18:11:21.197274 makenew_pypackage-4.2.0/makenew_pypackage/__init__.py
--rw-r--r--   0        0        0       56 2023-07-25 18:11:21.197274 makenew_pypackage-4.2.0/makenew_pypackage/todo.py
--rw-r--r--   0        0        0      156 2023-07-25 18:11:21.197274 makenew_pypackage-4.2.0/makenew_pypackage/todo_test.py
--rw-r--r--   0        0        0      615 2023-07-25 18:11:21.197274 makenew_pypackage-4.2.0/pyproject.toml
--rw-r--r--   0        0        0     7427 1970-01-01 00:00:00.000000 makenew_pypackage-4.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1079 2024-04-02 18:02:46.989584 makenew_pypackage-5.0.1/LICENSE.txt
+-rw-r--r--   0        0        0     6865 2024-04-02 18:02:46.989584 makenew_pypackage-5.0.1/README.rst
+-rw-r--r--   0        0        0       46 2024-04-02 18:02:46.989584 makenew_pypackage-5.0.1/makenew_pypackage/__init__.py
+-rw-r--r--   0        0        0       56 2024-04-02 18:02:46.989584 makenew_pypackage-5.0.1/makenew_pypackage/todo.py
+-rw-r--r--   0        0        0      156 2024-04-02 18:02:46.989584 makenew_pypackage-5.0.1/makenew_pypackage/todo_test.py
+-rw-r--r--   0        0        0      615 2024-04-02 18:02:46.989584 makenew_pypackage-5.0.1/pyproject.toml
+-rw-r--r--   0        0        0     7427 1970-01-01 00:00:00.000000 makenew_pypackage-5.0.1/PKG-INFO
```

### Comparing `makenew_pypackage-4.2.0/LICENSE.txt` & `makenew_pypackage-5.0.1/LICENSE.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2023 Evan Sosenko
+Copyright (c) 2024 Evan Sosenko
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 the Software, and to permit persons to whom the Software is furnished to do so,
 subject to the following conditions:
```

### Comparing `makenew_pypackage-4.2.0/README.rst` & `makenew_pypackage-5.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `makenew_pypackage-4.2.0/pyproject.toml` & `makenew_pypackage-5.0.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "makenew-pypackage"
-version = "4.2.0"
+version = "5.0.1"
 description = "Package skeleton for a Python module."
 authors = ["Evan Sosenko <razorx@evansosenko.com>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/makenew/pypackage"
 repository = "https://github.com/makenew/pypackage"
 
 [tool.poetry.dependencies]
-python = "^3.10.0"
+python = "^3.11.0"
 
 [tool.poetry.group.dev.dependencies]
-black = "^23.7.0"
-pylint = "^2.4.0"
-pytest = "^7.1.1"
-pytest-cov = "^4.0.0"
+black = "^24.3.0"
+pylint = "^3.1.0"
+pytest = "^8.1.1"
+pytest-cov = "^5.0.0"
 pytest-runner = "^6.0.0"
 pytest-watch = "^4.2.0"
 rstcheck = "^6.1.2"
 
 [build-system]
-requires = ["poetry>=1.2"]
+requires = ["poetry>=1.8"]
 build-backend = "poetry.masonry.api"
```

### Comparing `makenew_pypackage-4.2.0/PKG-INFO` & `makenew_pypackage-5.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: makenew-pypackage
-Version: 4.2.0
+Version: 5.0.1
 Summary: Package skeleton for a Python module.
 Home-page: https://github.com/makenew/pypackage
 License: MIT
 Author: Evan Sosenko
 Author-email: razorx@evansosenko.com
-Requires-Python: >=3.10.0,<4.0.0
+Requires-Python: >=3.11.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Project-URL: Repository, https://github.com/makenew/pypackage
 Description-Content-Type: text/x-rst
 
 Python Package Skeleton
 =======================
 
 |PyPI| |GitHub Actions|
```

