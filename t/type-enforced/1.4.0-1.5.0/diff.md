# Comparing `tmp/type_enforced-1.4.0.tar.gz` & `tmp/type_enforced-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "type_enforced-1.4.0.tar", last modified: Fri Mar  1 18:49:48 2024, max compression
+gzip compressed data, was "type_enforced-1.5.0.tar", last modified: Tue Apr  2 19:37:12 2024, max compression
```

## Comparing `type_enforced-1.4.0.tar` & `type_enforced-1.5.0.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-03-01 18:49:48.397921 type_enforced-1.4.0/
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)     1072 2024-01-17 18:48:04.000000 type_enforced-1.4.0/LICENSE
--rw-r--r--   0 conmak    (1000) conmak    (1000)     9338 2024-03-01 18:49:48.397921 type_enforced-1.4.0/PKG-INFO
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)     8678 2024-03-01 18:39:14.000000 type_enforced-1.4.0/README.md
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)      880 2024-03-01 18:46:36.000000 type_enforced-1.4.0/pyproject.toml
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)      143 2024-03-01 18:49:48.397921 type_enforced-1.4.0/setup.cfg
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-03-01 18:49:48.397921 type_enforced-1.4.0/test/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      385 2024-03-01 18:03:08.000000 type_enforced-1.4.0/test/test_class_01.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      381 2024-03-01 18:03:17.000000 type_enforced-1.4.0/test/test_class_02.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      497 2024-03-01 14:55:56.000000 type_enforced-1.4.0/test/test_class_03.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      525 2024-03-01 14:55:56.000000 type_enforced-1.4.0/test/test_class_04.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      784 2024-03-01 18:05:31.000000 type_enforced-1.4.0/test/test_class_05.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      744 2024-03-01 14:55:56.000000 type_enforced-1.4.0/test/test_class_06.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      716 2024-03-01 14:55:56.000000 type_enforced-1.4.0/test/test_class_07.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     1635 2024-03-01 14:55:56.000000 type_enforced-1.4.0/test/test_class_08.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      551 2024-03-01 14:55:56.000000 type_enforced-1.4.0/test/test_class_09.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      659 2024-03-01 18:48:46.000000 type_enforced-1.4.0/test/test_class_10.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      536 2024-03-01 18:48:46.000000 type_enforced-1.4.0/test/test_fn_01.py
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)      364 2024-01-17 18:48:04.000000 type_enforced-1.4.0/test/test_fn_02.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      465 2024-01-17 18:48:04.000000 type_enforced-1.4.0/test/test_fn_03.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      531 2024-01-17 18:48:04.000000 type_enforced-1.4.0/test/test_fn_04.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     1560 2024-01-17 18:48:04.000000 type_enforced-1.4.0/test/test_fn_05.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     1240 2024-03-01 18:07:26.000000 type_enforced-1.4.0/test/test_fn_06.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      784 2024-01-17 18:48:04.000000 type_enforced-1.4.0/test/test_fn_07.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      695 2024-01-17 18:48:04.000000 type_enforced-1.4.0/test/test_fn_08.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      726 2024-01-17 18:48:04.000000 type_enforced-1.4.0/test/test_fn_09.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      776 2024-01-17 18:48:04.000000 type_enforced-1.4.0/test/test_fn_10.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      454 2024-01-17 18:48:04.000000 type_enforced-1.4.0/test/test_fn_11.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      707 2024-01-17 18:48:04.000000 type_enforced-1.4.0/test/test_fn_12.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      430 2024-01-17 18:48:04.000000 type_enforced-1.4.0/test/test_fn_13.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     1347 2024-03-01 18:48:46.000000 type_enforced-1.4.0/test/test_fn_14.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      408 2024-03-01 18:48:46.000000 type_enforced-1.4.0/test/test_fn_15.py
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-03-01 18:49:48.397921 type_enforced-1.4.0/type_enforced/
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)       67 2024-03-01 18:00:02.000000 type_enforced-1.4.0/type_enforced/__init__.py
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)    13050 2024-03-01 18:48:46.000000 type_enforced-1.4.0/type_enforced/enforcer.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     2628 2024-03-01 18:48:46.000000 type_enforced-1.4.0/type_enforced/utils.py
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-03-01 18:49:48.397921 type_enforced-1.4.0/type_enforced.egg-info/
--rw-r--r--   0 conmak    (1000) conmak    (1000)     9338 2024-03-01 18:49:48.000000 type_enforced-1.4.0/type_enforced.egg-info/PKG-INFO
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      770 2024-03-01 18:49:48.000000 type_enforced-1.4.0/type_enforced.egg-info/SOURCES.txt
--rw-rw-r--   0 conmak    (1000) conmak    (1000)        1 2024-03-01 18:49:48.000000 type_enforced-1.4.0/type_enforced.egg-info/dependency_links.txt
--rw-rw-r--   0 conmak    (1000) conmak    (1000)       14 2024-03-01 18:49:48.000000 type_enforced-1.4.0/type_enforced.egg-info/top_level.txt
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-04-02 19:37:12.960417 type_enforced-1.5.0/
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)     1072 2024-01-17 18:48:04.000000 type_enforced-1.5.0/LICENSE
+-rw-r--r--   0 conmak    (1000) conmak    (1000)    11318 2024-04-02 19:37:12.960417 type_enforced-1.5.0/PKG-INFO
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)    10658 2024-04-02 19:29:25.000000 type_enforced-1.5.0/README.md
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)      880 2024-04-02 19:30:56.000000 type_enforced-1.5.0/pyproject.toml
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)      143 2024-04-02 19:37:12.960417 type_enforced-1.5.0/setup.cfg
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-04-02 19:37:12.956417 type_enforced-1.5.0/test/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      385 2024-04-02 13:51:25.000000 type_enforced-1.5.0/test/test_class_01.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      381 2024-04-02 13:51:25.000000 type_enforced-1.5.0/test/test_class_02.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      497 2024-04-02 13:51:25.000000 type_enforced-1.5.0/test/test_class_03.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      525 2024-04-02 13:51:25.000000 type_enforced-1.5.0/test/test_class_04.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      784 2024-04-02 13:51:25.000000 type_enforced-1.5.0/test/test_class_05.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      744 2024-04-02 13:51:25.000000 type_enforced-1.5.0/test/test_class_06.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      716 2024-04-02 13:51:25.000000 type_enforced-1.5.0/test/test_class_07.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     1635 2024-04-02 13:51:25.000000 type_enforced-1.5.0/test/test_class_08.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      551 2024-04-02 13:51:25.000000 type_enforced-1.5.0/test/test_class_09.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      659 2024-04-02 13:51:25.000000 type_enforced-1.5.0/test/test_class_10.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      536 2024-03-01 18:48:46.000000 type_enforced-1.5.0/test/test_fn_01.py
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)      364 2024-01-17 18:48:04.000000 type_enforced-1.5.0/test/test_fn_02.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      465 2024-01-17 18:48:04.000000 type_enforced-1.5.0/test/test_fn_03.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      531 2024-01-17 18:48:04.000000 type_enforced-1.5.0/test/test_fn_04.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     1560 2024-01-17 18:48:04.000000 type_enforced-1.5.0/test/test_fn_05.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     1240 2024-04-02 13:51:25.000000 type_enforced-1.5.0/test/test_fn_06.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      784 2024-01-17 18:48:04.000000 type_enforced-1.5.0/test/test_fn_07.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      695 2024-01-17 18:48:04.000000 type_enforced-1.5.0/test/test_fn_08.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      726 2024-01-17 18:48:04.000000 type_enforced-1.5.0/test/test_fn_09.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      776 2024-01-17 18:48:04.000000 type_enforced-1.5.0/test/test_fn_10.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      454 2024-01-17 18:48:04.000000 type_enforced-1.5.0/test/test_fn_11.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      707 2024-01-17 18:48:04.000000 type_enforced-1.5.0/test/test_fn_12.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      441 2024-04-02 18:23:07.000000 type_enforced-1.5.0/test/test_fn_13.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     1347 2024-04-02 13:51:25.000000 type_enforced-1.5.0/test/test_fn_14.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      408 2024-04-02 13:51:25.000000 type_enforced-1.5.0/test/test_fn_15.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     1692 2024-04-02 19:30:24.000000 type_enforced-1.5.0/test/test_fn_16.py
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-04-02 19:37:12.956417 type_enforced-1.5.0/type_enforced/
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)       67 2024-03-01 18:00:02.000000 type_enforced-1.5.0/type_enforced/__init__.py
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)    13829 2024-04-02 18:50:43.000000 type_enforced-1.5.0/type_enforced/enforcer.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     8576 2024-04-02 19:30:24.000000 type_enforced-1.5.0/type_enforced/utils.py
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-04-02 19:37:12.960417 type_enforced-1.5.0/type_enforced.egg-info/
+-rw-r--r--   0 conmak    (1000) conmak    (1000)    11318 2024-04-02 19:37:12.000000 type_enforced-1.5.0/type_enforced.egg-info/PKG-INFO
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      789 2024-04-02 19:37:12.000000 type_enforced-1.5.0/type_enforced.egg-info/SOURCES.txt
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)        1 2024-04-02 19:37:12.000000 type_enforced-1.5.0/type_enforced.egg-info/dependency_links.txt
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)       14 2024-04-02 19:37:12.000000 type_enforced-1.5.0/type_enforced.egg-info/top_level.txt
```

### Comparing `type_enforced-1.4.0/LICENSE` & `type_enforced-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `type_enforced-1.4.0/PKG-INFO` & `type_enforced-1.5.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: type_enforced
-Version: 1.4.0
-Summary: A pure python type enforcer for python type annotations
-Author-email: Connor Makowski <conmak@mit.edu>
-Project-URL: Homepage, https://github.com/connor-makowski/type_enforced
-Project-URL: Bug Tracker, https://github.com/connor-makowski/type_enforced/issues
-Project-URL: Documentation, https://connor-makowski.github.io/type_enforced/type_enforced/enforcer.html
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Type Enforced
 [![PyPI version](https://badge.fury.io/py/type_enforced.svg)](https://badge.fury.io/py/type_enforced)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 A pure python (no special compiler required) type enforcer for type annotations. Enforce types in python functions and methods.
 
 # Setup
@@ -51,14 +36,16 @@
 
 You can pass union types to validate one of multiple types. For example, you could validate an input was an int or a float with `[int, float]`, `[int | float]` or even `typing.Union[int, float]`.
 
 Nesting is allowed as long as the nested items are iterables (e.g. `typing.List`, `dict`, ...). For examle, you could validate that a list is a vector with `list[int]` or possibly `typing.List[int]`.
 
 Variables without an annotation for type are not enforced.
 
+Note: Type Enforced does not support `__future__.annotations`. If you call `from __future__ import annotations` in your file, type enforced will not work as expected.
+
 ## Supported Type Checking Features:
 
 - Function/Method Input Typing
 - Function/Method Return Typing
 - All standard python types (`str`, `list`, `int`, `dict`, ...)
 - Union types
     - typing.Union
@@ -82,19 +69,27 @@
         - Note: Can not have a nested type
             - Because this does not always meet the criteria for `Nested types` above
     - `Literal`
         - Only allow certain values to be passed. Operates slightly differently than other checks.
         - e.g. `Literal['a', 'b']` will require any passed values that are equal (`==`) to `'a'` or `'b'`.
             - This compares the value of the passed input and not the type of the passed input.
         - Note: Multiple types can be passed in the same `Literal`.
+        - Note: Literals are evaluated after type checking occurs.
     - `Callable`
         - Essentially creates a union of:
             - `staticmethod`, `classmethod`, `types.FunctionType`, `types.BuiltinFunctionType`, `types.MethodType`, `types.BuiltinMethodType`, `types.GeneratorType`
     - Note: Other functions might have support, but there are not currently tests to validate them
         - Feel free to create an issue (or better yet a PR) if you want to add tests/support
+- `Constraint` validation.
+    - This is a special type of validation that allows passed input to be validated.
+        - Standard and custom constraints are supported.
+    - This is useful for validating that a passed input is within a certain range or meets a certain criteria.
+    - Note: The constraint is checked after type checking occurs.
+    - Note: See the example below or technical [constraint](https://connor-makowski.github.io/type_enforced/type_enforced/utils.html#Constraint) and [generic constraint](https://connor-makowski.github.io/type_enforced/type_enforced/utils.html#GenericConstraint) docs for more information.
+    ```
 
 ## Interactive Example
 
 ```py
 >>> import type_enforced
 >>> @type_enforced.Enforcer
 ... def my_fn(a: int , b: [int, str] =2, c: int =3) -> None:
@@ -188,14 +183,52 @@
         pass
         
     @type_enforced.Enforcer(enabled=False)
     def my_other_fn(self, a: int) -> None:
         pass
 ```
 
+## Validate with Constraints
+Type enforcer can enforce constraints for passed variables. These constraints are vaildated after any type checks are made.
+
+To enforce basic input values are integers greater than or equal to zero, you can use the [Constraint](https://connor-makowski.github.io/type_enforced/type_enforced/utils.html#Constraint) class like so:
+```py
+import type_enforced
+from type_enforced.utils import Constraint
+
+@type_enforced.Enforcer()
+def positive_int_test(value: [int, Constraint(ge=0)]) -> bool:
+    return True
+
+positive_int_test(1) # Passes
+positive_int_test(-1) # Fails
+positive_int_test(1.0) # Fails
+```
+
+To enforce a [GenericConstraint](https://connor-makowski.github.io/type_enforced/type_enforced/utils.html#GenericConstraint):
+```py
+import type_enforced
+from type_enforced.utils import GenericConstraint
+
+CustomConstraint = GenericConstraint(
+    {
+        'in_rgb': lambda x: x in ['red', 'green', 'blue'],
+    }
+)
+
+@type_enforced.Enforcer()
+def rgb_test(value: [int, CustomConstraint]) -> bool:
+    return True
+
+rgb_test('red') # Passes
+rgb_test('yellow') # Fails
+```
+
+
+
 ## Validate class instances and classes
 
 Type enforcer can enforce class instances and classes. There are a few caveats between the two.
 
 To enforce a class instance, simply pass the class itself as a type hint:
 ```py
 import type_enforced
@@ -252,8 +285,8 @@
 def my_fn(custom_class: WithSubclasses(Foo)):
     pass
 
 print(WithSubclasses(Foo)) # Prints: [<class '__main__.Foo'>, <class '__main__.Bar'>]
 my_fn(Foo()) # Passes as expected
 my_fn(Bar()) # Passes as expected
 my_fn(Baz()) # Raises TypeError as expected
-```
+```
```

### Comparing `type_enforced-1.4.0/README.md` & `type_enforced-1.5.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: type_enforced
+Version: 1.5.0
+Summary: A pure python type enforcer for python type annotations
+Author-email: Connor Makowski <conmak@mit.edu>
+Project-URL: Homepage, https://github.com/connor-makowski/type_enforced
+Project-URL: Bug Tracker, https://github.com/connor-makowski/type_enforced/issues
+Project-URL: Documentation, https://connor-makowski.github.io/type_enforced/type_enforced/enforcer.html
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Type Enforced
 [![PyPI version](https://badge.fury.io/py/type_enforced.svg)](https://badge.fury.io/py/type_enforced)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 A pure python (no special compiler required) type enforcer for type annotations. Enforce types in python functions and methods.
 
 # Setup
@@ -36,14 +51,16 @@
 
 You can pass union types to validate one of multiple types. For example, you could validate an input was an int or a float with `[int, float]`, `[int | float]` or even `typing.Union[int, float]`.
 
 Nesting is allowed as long as the nested items are iterables (e.g. `typing.List`, `dict`, ...). For examle, you could validate that a list is a vector with `list[int]` or possibly `typing.List[int]`.
 
 Variables without an annotation for type are not enforced.
 
+Note: Type Enforced does not support `__future__.annotations`. If you call `from __future__ import annotations` in your file, type enforced will not work as expected.
+
 ## Supported Type Checking Features:
 
 - Function/Method Input Typing
 - Function/Method Return Typing
 - All standard python types (`str`, `list`, `int`, `dict`, ...)
 - Union types
     - typing.Union
@@ -67,19 +84,27 @@
         - Note: Can not have a nested type
             - Because this does not always meet the criteria for `Nested types` above
     - `Literal`
         - Only allow certain values to be passed. Operates slightly differently than other checks.
         - e.g. `Literal['a', 'b']` will require any passed values that are equal (`==`) to `'a'` or `'b'`.
             - This compares the value of the passed input and not the type of the passed input.
         - Note: Multiple types can be passed in the same `Literal`.
+        - Note: Literals are evaluated after type checking occurs.
     - `Callable`
         - Essentially creates a union of:
             - `staticmethod`, `classmethod`, `types.FunctionType`, `types.BuiltinFunctionType`, `types.MethodType`, `types.BuiltinMethodType`, `types.GeneratorType`
     - Note: Other functions might have support, but there are not currently tests to validate them
         - Feel free to create an issue (or better yet a PR) if you want to add tests/support
+- `Constraint` validation.
+    - This is a special type of validation that allows passed input to be validated.
+        - Standard and custom constraints are supported.
+    - This is useful for validating that a passed input is within a certain range or meets a certain criteria.
+    - Note: The constraint is checked after type checking occurs.
+    - Note: See the example below or technical [constraint](https://connor-makowski.github.io/type_enforced/type_enforced/utils.html#Constraint) and [generic constraint](https://connor-makowski.github.io/type_enforced/type_enforced/utils.html#GenericConstraint) docs for more information.
+    ```
 
 ## Interactive Example
 
 ```py
 >>> import type_enforced
 >>> @type_enforced.Enforcer
 ... def my_fn(a: int , b: [int, str] =2, c: int =3) -> None:
@@ -173,14 +198,52 @@
         pass
         
     @type_enforced.Enforcer(enabled=False)
     def my_other_fn(self, a: int) -> None:
         pass
 ```
 
+## Validate with Constraints
+Type enforcer can enforce constraints for passed variables. These constraints are vaildated after any type checks are made.
+
+To enforce basic input values are integers greater than or equal to zero, you can use the [Constraint](https://connor-makowski.github.io/type_enforced/type_enforced/utils.html#Constraint) class like so:
+```py
+import type_enforced
+from type_enforced.utils import Constraint
+
+@type_enforced.Enforcer()
+def positive_int_test(value: [int, Constraint(ge=0)]) -> bool:
+    return True
+
+positive_int_test(1) # Passes
+positive_int_test(-1) # Fails
+positive_int_test(1.0) # Fails
+```
+
+To enforce a [GenericConstraint](https://connor-makowski.github.io/type_enforced/type_enforced/utils.html#GenericConstraint):
+```py
+import type_enforced
+from type_enforced.utils import GenericConstraint
+
+CustomConstraint = GenericConstraint(
+    {
+        'in_rgb': lambda x: x in ['red', 'green', 'blue'],
+    }
+)
+
+@type_enforced.Enforcer()
+def rgb_test(value: [int, CustomConstraint]) -> bool:
+    return True
+
+rgb_test('red') # Passes
+rgb_test('yellow') # Fails
+```
+
+
+
 ## Validate class instances and classes
 
 Type enforcer can enforce class instances and classes. There are a few caveats between the two.
 
 To enforce a class instance, simply pass the class itself as a type hint:
 ```py
 import type_enforced
@@ -237,8 +300,8 @@
 def my_fn(custom_class: WithSubclasses(Foo)):
     pass
 
 print(WithSubclasses(Foo)) # Prints: [<class '__main__.Foo'>, <class '__main__.Bar'>]
 my_fn(Foo()) # Passes as expected
 my_fn(Bar()) # Passes as expected
 my_fn(Baz()) # Raises TypeError as expected
-```
+```
```

### Comparing `type_enforced-1.4.0/pyproject.toml` & `type_enforced-1.5.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "type_enforced"
-version = "1.4.0"
+version = "1.5.0"
 description = "A pure python type enforcer for python type annotations"
 authors = [
     {name="Connor Makowski", email="conmak@mit.edu"}
 ]
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `type_enforced-1.4.0/test/test_class_04.py` & `type_enforced-1.5.0/test/test_class_04.py`

 * *Files identical despite different names*

### Comparing `type_enforced-1.4.0/test/test_class_05.py` & `type_enforced-1.5.0/test/test_class_05.py`

 * *Files identical despite different names*

### Comparing `type_enforced-1.4.0/test/test_class_06.py` & `type_enforced-1.5.0/test/test_class_06.py`

 * *Files identical despite different names*

### Comparing `type_enforced-1.4.0/test/test_class_07.py` & `type_enforced-1.5.0/test/test_class_07.py`

 * *Files identical despite different names*

### Comparing `type_enforced-1.4.0/test/test_class_08.py` & `type_enforced-1.5.0/test/test_class_08.py`

 * *Files identical despite different names*

### Comparing `type_enforced-1.4.0/test/test_class_09.py` & `type_enforced-1.5.0/test/test_class_09.py`

 * *Files identical despite different names*

### Comparing `type_enforced-1.4.0/test/test_class_10.py` & `type_enforced-1.5.0/test/test_class_10.py`

 * *Files identical despite different names*

### Comparing `type_enforced-1.4.0/test/test_fn_01.py` & `type_enforced-1.5.0/test/test_fn_01.py`

 * *Files identical despite different names*

### Comparing `type_enforced-1.4.0/test/test_fn_04.py` & `type_enforced-1.5.0/test/test_fn_04.py`

 * *Files identical despite different names*

### Comparing `type_enforced-1.4.0/test/test_fn_05.py` & `type_enforced-1.5.0/test/test_fn_05.py`

 * *Files identical despite different names*

### Comparing `type_enforced-1.4.0/test/test_fn_06.py` & `type_enforced-1.5.0/test/test_fn_06.py`

 * *Files identical despite different names*

### Comparing `type_enforced-1.4.0/test/test_fn_07.py` & `type_enforced-1.5.0/test/test_fn_07.py`

 * *Files identical despite different names*

### Comparing `type_enforced-1.4.0/test/test_fn_08.py` & `type_enforced-1.5.0/test/test_fn_08.py`

 * *Files identical despite different names*

### Comparing `type_enforced-1.4.0/test/test_fn_09.py` & `type_enforced-1.5.0/test/test_fn_09.py`

 * *Files identical despite different names*

### Comparing `type_enforced-1.4.0/test/test_fn_10.py` & `type_enforced-1.5.0/test/test_fn_10.py`

 * *Files identical despite different names*

### Comparing `type_enforced-1.4.0/test/test_fn_12.py` & `type_enforced-1.5.0/test/test_fn_12.py`

 * *Files identical despite different names*

### Comparing `type_enforced-1.4.0/test/test_fn_14.py` & `type_enforced-1.5.0/test/test_fn_14.py`

 * *Files identical despite different names*

### Comparing `type_enforced-1.4.0/type_enforced/enforcer.py` & `type_enforced-1.5.0/type_enforced/enforcer.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     GenericAlias,
     GeneratorType,
     BuiltinFunctionType,
     BuiltinMethodType,
 )
 from typing import Type, Union, Sized, Literal, Callable
 from functools import update_wrapper, wraps
-from type_enforced.utils import Partial
+from type_enforced.utils import Partial, GenericConstraint
 
 # Python 3.10+ has a UnionType object that is used to represent Union types
 try:
     from types import UnionType
 except ImportError:
     # Python < 3.10 does not have UnionType
     # Since UnionType is validated after NoneType, we can use NoneType
@@ -69,15 +69,15 @@
         else:
             self.__fn_defaults__ = {}
 
     def __get_checkable_type__(self, item_annotation):
         """
         Gets the checkable type as a nested dict for a passed annotation.
         """
-        valid_types = {}
+        valid_types = {"__extra__": {}}
         if not isinstance(item_annotation, (list, tuple)):
             item_annotation = [item_annotation]
         for valid_type in item_annotation:
             # Special code to replace None with NoneType
             if valid_type is None:
                 valid_types[type(None)] = None
                 continue
@@ -95,18 +95,17 @@
                     valid_types.update(
                         self.__get_checkable_type__(valid_type.__args__)
                     )
                 # Handle Literals
                 # Note: These will be handled separately in the self.__check_type__
                 # as the object is validated and not its type.
                 elif valid_type.__origin__ == Literal:
-                    valid_types = {
-                        Literal: {i: None for i in valid_type.__args__}
-                    }
-
+                    valid_types["__extra__"][
+                        "__literal__"
+                    ] = valid_type.__args__
                 # Handle Sized objects
                 elif valid_type == Sized:
                     valid_types = {
                         list: None,
                         tuple: None,
                         dict: None,
                         set: None,
@@ -133,14 +132,19 @@
                 else:
                     valid_types[valid_type] = None
             # Handle special '|' syntax for Union Types
             elif isinstance(valid_type, UnionType):
                 valid_types.update(
                     self.__get_checkable_type__(valid_type.__args__)
                 )
+            # Handle Constraints
+            # Note: These will be handled separately in the self.__check_type__
+            # as the object is validated differently than a type.
+            elif isinstance(valid_type, GenericConstraint):
+                valid_types["__extra__"]["__constraint__"] = valid_type
             else:
                 valid_types[valid_type] = None
         return valid_types
 
     def __exception__(self, message):
         """
         Usage:
@@ -207,38 +211,45 @@
         """
         Raises an exception the type of a passed `obj` (parameter) is not in the list of supplied `acceptable_types` for the argument.
         """
         if isinstance(obj, type):
             passed_type = Type[obj]
         else:
             passed_type = type(obj)
-        if passed_type not in acceptable_types:
-            # Add special string to store any string to add before acceptable types
-            # in any exception message
-            pre_acceptable_types_str = ""
-            # Special check for Literals
-            if Literal in acceptable_types:
-                if obj in acceptable_types[Literal]:
-                    return
-                else:
-                    pre_acceptable_types_str = "Literal"
-                    acceptable_types = acceptable_types[Literal]
-                    passed_type = obj
-            # Raise the exception
-            self.__exception__(
-                f"Type mismatch for typed variable `{key}`. Expected one of the following `{pre_acceptable_types_str}{str(list(acceptable_types.keys()))}` but got `{passed_type}` instead."
-            )
+        acceptable_types = dict(acceptable_types)
+        extra_types = acceptable_types.pop("__extra__")
+        if acceptable_types != {}:
+            if passed_type not in acceptable_types:
+                # Raise the exception
+                self.__exception__(
+                    f"Type mismatch for typed variable `{key}`. Expected one of the following `{str(list(acceptable_types.keys()))}` but got `{passed_type}` instead."
+                )
         sub_type = acceptable_types.get(passed_type)
         if sub_type is not None:
             if passed_type == dict:
                 for sub_key, value in obj.items():
                     self.__check_type__(value, sub_type, f"{key}[{sub_key}]")
             else:
                 for sub_key, value in enumerate(obj):
                     self.__check_type__(value, sub_type, f"{key}[{sub_key}]")
+        # Special check for Literal types
+        literal_options = extra_types.get("__literal__")
+        if literal_options is not None:
+            if obj not in literal_options:
+                self.__exception__(
+                    f"Literal validation error for variable `{key}`. Expected one of the following `{str(list(literal_options))}` but got `{obj}` instead."
+                )
+        # Special check for Constraints
+        constraint = extra_types.get("__constraint__")
+        if constraint is not None:
+            constraint_validation_output = constraint.__validate__(key, obj)
+            if constraint_validation_output is not True:
+                self.__exception__(
+                    f"Constraint validation error for variable `{key}`. {constraint_validation_output}"
+                )
 
     def __repr__(self):
         return f"<type_enforced {self.__fn__.__module__}.{self.__fn__.__qualname__} object at {hex(id(self))}>"
 
 
 def Enforcer(clsFnMethod, enabled):
     """
```

### Comparing `type_enforced-1.4.0/type_enforced.egg-info/PKG-INFO` & `type_enforced-1.5.0/type_enforced.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: type_enforced
-Version: 1.4.0
+Version: 1.5.0
 Summary: A pure python type enforcer for python type annotations
 Author-email: Connor Makowski <conmak@mit.edu>
 Project-URL: Homepage, https://github.com/connor-makowski/type_enforced
 Project-URL: Bug Tracker, https://github.com/connor-makowski/type_enforced/issues
 Project-URL: Documentation, https://connor-makowski.github.io/type_enforced/type_enforced/enforcer.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -51,14 +51,16 @@
 
 You can pass union types to validate one of multiple types. For example, you could validate an input was an int or a float with `[int, float]`, `[int | float]` or even `typing.Union[int, float]`.
 
 Nesting is allowed as long as the nested items are iterables (e.g. `typing.List`, `dict`, ...). For examle, you could validate that a list is a vector with `list[int]` or possibly `typing.List[int]`.
 
 Variables without an annotation for type are not enforced.
 
+Note: Type Enforced does not support `__future__.annotations`. If you call `from __future__ import annotations` in your file, type enforced will not work as expected.
+
 ## Supported Type Checking Features:
 
 - Function/Method Input Typing
 - Function/Method Return Typing
 - All standard python types (`str`, `list`, `int`, `dict`, ...)
 - Union types
     - typing.Union
@@ -82,19 +84,27 @@
         - Note: Can not have a nested type
             - Because this does not always meet the criteria for `Nested types` above
     - `Literal`
         - Only allow certain values to be passed. Operates slightly differently than other checks.
         - e.g. `Literal['a', 'b']` will require any passed values that are equal (`==`) to `'a'` or `'b'`.
             - This compares the value of the passed input and not the type of the passed input.
         - Note: Multiple types can be passed in the same `Literal`.
+        - Note: Literals are evaluated after type checking occurs.
     - `Callable`
         - Essentially creates a union of:
             - `staticmethod`, `classmethod`, `types.FunctionType`, `types.BuiltinFunctionType`, `types.MethodType`, `types.BuiltinMethodType`, `types.GeneratorType`
     - Note: Other functions might have support, but there are not currently tests to validate them
         - Feel free to create an issue (or better yet a PR) if you want to add tests/support
+- `Constraint` validation.
+    - This is a special type of validation that allows passed input to be validated.
+        - Standard and custom constraints are supported.
+    - This is useful for validating that a passed input is within a certain range or meets a certain criteria.
+    - Note: The constraint is checked after type checking occurs.
+    - Note: See the example below or technical [constraint](https://connor-makowski.github.io/type_enforced/type_enforced/utils.html#Constraint) and [generic constraint](https://connor-makowski.github.io/type_enforced/type_enforced/utils.html#GenericConstraint) docs for more information.
+    ```
 
 ## Interactive Example
 
 ```py
 >>> import type_enforced
 >>> @type_enforced.Enforcer
 ... def my_fn(a: int , b: [int, str] =2, c: int =3) -> None:
@@ -188,14 +198,52 @@
         pass
         
     @type_enforced.Enforcer(enabled=False)
     def my_other_fn(self, a: int) -> None:
         pass
 ```
 
+## Validate with Constraints
+Type enforcer can enforce constraints for passed variables. These constraints are vaildated after any type checks are made.
+
+To enforce basic input values are integers greater than or equal to zero, you can use the [Constraint](https://connor-makowski.github.io/type_enforced/type_enforced/utils.html#Constraint) class like so:
+```py
+import type_enforced
+from type_enforced.utils import Constraint
+
+@type_enforced.Enforcer()
+def positive_int_test(value: [int, Constraint(ge=0)]) -> bool:
+    return True
+
+positive_int_test(1) # Passes
+positive_int_test(-1) # Fails
+positive_int_test(1.0) # Fails
+```
+
+To enforce a [GenericConstraint](https://connor-makowski.github.io/type_enforced/type_enforced/utils.html#GenericConstraint):
+```py
+import type_enforced
+from type_enforced.utils import GenericConstraint
+
+CustomConstraint = GenericConstraint(
+    {
+        'in_rgb': lambda x: x in ['red', 'green', 'blue'],
+    }
+)
+
+@type_enforced.Enforcer()
+def rgb_test(value: [int, CustomConstraint]) -> bool:
+    return True
+
+rgb_test('red') # Passes
+rgb_test('yellow') # Fails
+```
+
+
+
 ## Validate class instances and classes
 
 Type enforcer can enforce class instances and classes. There are a few caveats between the two.
 
 To enforce a class instance, simply pass the class itself as a type hint:
 ```py
 import type_enforced
```

### Comparing `type_enforced-1.4.0/type_enforced.egg-info/SOURCES.txt` & `type_enforced-1.5.0/type_enforced.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 test/test_fn_09.py
 test/test_fn_10.py
 test/test_fn_11.py
 test/test_fn_12.py
 test/test_fn_13.py
 test/test_fn_14.py
 test/test_fn_15.py
+test/test_fn_16.py
 type_enforced/__init__.py
 type_enforced/enforcer.py
 type_enforced/utils.py
 type_enforced.egg-info/PKG-INFO
 type_enforced.egg-info/SOURCES.txt
 type_enforced.egg-info/dependency_links.txt
 type_enforced.egg-info/top_level.txt
```

