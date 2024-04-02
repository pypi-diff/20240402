# Comparing `tmp/dynamicpy-1.2.1.tar.gz` & `tmp/dynamicpy-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamicpy-1.2.1.tar", max compression
+gzip compressed data, was "dynamicpy-1.2.2.tar", max compression
```

## Comparing `dynamicpy-1.2.1.tar` & `dynamicpy-1.2.2.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     3276 2024-01-22 21:17:53.103328 dynamicpy-1.2.1/README.md
--rw-r--r--   0        0        0      627 2024-01-22 21:17:53.103328 dynamicpy-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     1128 2024-01-22 21:18:13.671309 dynamicpy-1.2.1/src/dynamicpy/__init__.py
--rw-r--r--   0        0        0     3932 2024-01-22 21:18:13.671309 dynamicpy-1.2.1/src/dynamicpy/dependencies.py
--rw-r--r--   0        0        0     1056 2024-01-22 21:18:13.671309 dynamicpy-1.2.1/src/dynamicpy/errors.py
--rw-r--r--   0        0        0     7130 2024-01-22 21:18:13.671309 dynamicpy-1.2.1/src/dynamicpy/loader.py
--rw-r--r--   0        0        0     5604 2024-01-22 21:18:13.671309 dynamicpy-1.2.1/src/dynamicpy/utils.py
--rw-r--r--   0        0        0     2658 2024-01-22 21:18:13.671309 dynamicpy-1.2.1/src/dynamicpy/widgets.py
--rw-r--r--   0        0        0     4037 1970-01-01 00:00:00.000000 dynamicpy-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-02 13:19:20.126349 dynamicpy-1.2.2/LICENCE
+-rw-r--r--   0        0        0     3276 2024-04-02 13:19:20.126349 dynamicpy-1.2.2/README.md
+-rw-r--r--   0        0        0      610 2024-04-02 13:19:20.126349 dynamicpy-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1128 2024-04-02 13:19:37.238289 dynamicpy-1.2.2/src/dynamicpy/__init__.py
+-rw-r--r--   0        0        0     3932 2024-04-02 13:19:37.238289 dynamicpy-1.2.2/src/dynamicpy/dependencies.py
+-rw-r--r--   0        0        0     1056 2024-04-02 13:19:37.238289 dynamicpy-1.2.2/src/dynamicpy/errors.py
+-rw-r--r--   0        0        0     7195 2024-04-02 13:19:37.238289 dynamicpy-1.2.2/src/dynamicpy/loader.py
+-rw-r--r--   0        0        0     5604 2024-04-02 13:19:37.238289 dynamicpy-1.2.2/src/dynamicpy/utils.py
+-rw-r--r--   0        0        0     2658 2024-04-02 13:19:37.238289 dynamicpy-1.2.2/src/dynamicpy/widgets.py
+-rw-r--r--   0        0        0     4083 1970-01-01 00:00:00.000000 dynamicpy-1.2.2/PKG-INFO
```

### Comparing `dynamicpy-1.2.1/README.md` & `dynamicpy-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `dynamicpy-1.2.1/pyproject.toml` & `dynamicpy-1.2.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "dynamicpy"
-version = "1.2.1"
+version = "1.2.2"
 description = "A python module for dynamically interacting with objects to improve expandability."
 authors = ["NimajnebEC <nimajnebec@users.noreply.github.com>"]
 repository = "https://github.com/NimajnebEC/dynamicpy"
 packages = [{ include = "dynamicpy", from = "src" }]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 typeguard = "^4.0.0"
-python = "^3.8.1"
+python = "^3.8"
 
 [tool.poetry.group.dev.dependencies]
-flake8-length = "^0.3.1"
 pytest = "^7.3.1"
-flake8 = "^6.0.0"
-isort = "^5.12.0"
+ruff = "^0.2.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.ruff]
+line-length = 92
```

### Comparing `dynamicpy-1.2.1/src/dynamicpy/__init__.py` & `dynamicpy-1.2.2/src/dynamicpy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 A python module for dynamically interacting with objects to improve expandability.
 
 https://github.com/NimajnebEC/dynamicpy
 """
 
 
-__version__ = "1.2.1"
+__version__ = "1.2.2"
 __author__ = "NimajnebEC <nimajnebec@users.noreply.github.com>"
 
 from dynamicpy.dependencies import DependencyLibrary
 from dynamicpy.errors import (
     DependencyNotFoundError,
     DuplicateDependencyError,
     DynamicPyError,
```

### Comparing `dynamicpy-1.2.1/src/dynamicpy/dependencies.py` & `dynamicpy-1.2.2/src/dynamicpy/dependencies.py`

 * *Files identical despite different names*

### Comparing `dynamicpy-1.2.1/src/dynamicpy/errors.py` & `dynamicpy-1.2.2/src/dynamicpy/errors.py`

 * *Files identical despite different names*

### Comparing `dynamicpy-1.2.1/src/dynamicpy/loader.py` & `dynamicpy-1.2.2/src/dynamicpy/loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import contextlib
 import logging
 from types import ModuleType
 from typing import Any, Callable, Optional, Type, TypeVar, Union
 
 from typeguard import TypeCheckError, check_type
 
 from dynamicpy import utils
@@ -105,16 +104,20 @@
         widget : Type[BaseWidget]
             The widget type to run the handler on.
         handler : Callable[[BaseWidget], None]
             The handler function to run on widgets of the type of the `widget` parameter.
         """
 
         def wrapper(_, value: Any):
-            with contextlib.suppress(AttributeError):
-                for entry in BaseWidget.get_associations(value, create=False):
+            try:
+                associations = BaseWidget.get_associations(value, create=False)
+            except AttributeError:
+                return
+            else:
+                for entry in associations:
                     if isinstance(entry, widget):
                         handler(entry)
 
         self.register_handler(wrapper)
 
     def widget_handler(
         self, widget: Type[WidgetT]
```

### Comparing `dynamicpy-1.2.1/src/dynamicpy/utils.py` & `dynamicpy-1.2.2/src/dynamicpy/utils.py`

 * *Files identical despite different names*

### Comparing `dynamicpy-1.2.1/src/dynamicpy/widgets.py` & `dynamicpy-1.2.2/src/dynamicpy/widgets.py`

 * *Files identical despite different names*

### Comparing `dynamicpy-1.2.1/PKG-INFO` & `dynamicpy-1.2.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: dynamicpy
-Version: 1.2.1
+Version: 1.2.2
 Summary: A python module for dynamically interacting with objects to improve expandability.
 Home-page: https://github.com/NimajnebEC/dynamicpy
 License: MIT
 Author: NimajnebEC
 Author-email: nimajnebec@users.noreply.github.com
-Requires-Python: >=3.8.1,<4.0.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: typeguard (>=4.0.0,<5.0.0)
 Project-URL: Repository, https://github.com/NimajnebEC/dynamicpy
 Description-Content-Type: text/markdown
```

