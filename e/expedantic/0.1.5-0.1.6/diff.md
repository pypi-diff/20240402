# Comparing `tmp/expedantic-0.1.5.tar.gz` & `tmp/expedantic-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "expedantic-0.1.5.tar", last modified: Tue Mar 26 06:52:06 2024, max compression
+gzip compressed data, was "expedantic-0.1.6.tar", last modified: Tue Apr  2 02:45:06 2024, max compression
```

## Comparing `expedantic-0.1.5.tar` & `expedantic-0.1.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 js        (1000) js        (1000)        0 2024-03-26 06:52:06.913699 expedantic-0.1.5/
--rw-rw-r--   0 js        (1000) js        (1000)     1062 2024-03-12 08:20:45.000000 expedantic-0.1.5/LICENSE
--rw-r--r--   0 js        (1000) js        (1000)      314 2024-03-26 06:52:06.913699 expedantic-0.1.5/PKG-INFO
--rw-rw-r--   0 js        (1000) js        (1000)     4193 2024-03-26 06:49:17.000000 expedantic-0.1.5/README.md
-drwxrwxr-x   0 js        (1000) js        (1000)        0 2024-03-26 06:52:06.913699 expedantic-0.1.5/expedantic.egg-info/
--rw-r--r--   0 js        (1000) js        (1000)      314 2024-03-26 06:52:06.000000 expedantic-0.1.5/expedantic.egg-info/PKG-INFO
--rw-rw-r--   0 js        (1000) js        (1000)      520 2024-03-26 06:52:06.000000 expedantic-0.1.5/expedantic.egg-info/SOURCES.txt
--rw-rw-r--   0 js        (1000) js        (1000)        1 2024-03-26 06:52:06.000000 expedantic-0.1.5/expedantic.egg-info/dependency_links.txt
--rw-rw-r--   0 js        (1000) js        (1000)       59 2024-03-26 06:52:06.000000 expedantic-0.1.5/expedantic.egg-info/requires.txt
--rw-rw-r--   0 js        (1000) js        (1000)       17 2024-03-26 06:52:06.000000 expedantic-0.1.5/expedantic.egg-info/top_level.txt
--rw-rw-r--   0 js        (1000) js        (1000)       38 2024-03-26 06:52:06.913699 expedantic-0.1.5/setup.cfg
--rw-rw-r--   0 js        (1000) js        (1000)      672 2024-03-26 06:51:08.000000 expedantic-0.1.5/setup.py
-drwxrwxr-x   0 js        (1000) js        (1000)        0 2024-03-26 06:52:06.909699 expedantic-0.1.5/src/
-drwxrwxr-x   0 js        (1000) js        (1000)        0 2024-03-26 06:52:06.913699 expedantic-0.1.5/src/expedantic/
--rw-rw-r--   0 js        (1000) js        (1000)       98 2024-03-12 09:44:20.000000 expedantic-0.1.5/src/expedantic/__init__.py
--rw-rw-r--   0 js        (1000) js        (1000)    12510 2024-03-26 06:49:17.000000 expedantic-0.1.5/src/expedantic/config_base.py
--rw-rw-r--   0 js        (1000) js        (1000)      867 2024-03-12 08:26:06.000000 expedantic-0.1.5/src/expedantic/utils.py
-drwxrwxr-x   0 js        (1000) js        (1000)        0 2024-03-26 06:52:06.909699 expedantic-0.1.5/submodules/
-drwxrwxr-x   0 js        (1000) js        (1000)        0 2024-03-26 06:52:06.909699 expedantic-0.1.5/submodules/ccorp_yaml_include/
-drwxrwxr-x   0 js        (1000) js        (1000)        0 2024-03-26 06:52:06.909699 expedantic-0.1.5/submodules/ccorp_yaml_include/ccorp/
-drwxrwxr-x   0 js        (1000) js        (1000)        0 2024-03-26 06:52:06.909699 expedantic-0.1.5/submodules/ccorp_yaml_include/ccorp/ruamel/
-drwxrwxr-x   0 js        (1000) js        (1000)        0 2024-03-26 06:52:06.909699 expedantic-0.1.5/submodules/ccorp_yaml_include/ccorp/ruamel/yaml/
-drwxrwxr-x   0 js        (1000) js        (1000)        0 2024-03-26 06:52:06.913699 expedantic-0.1.5/submodules/ccorp_yaml_include/ccorp/ruamel/yaml/include/
--rw-rw-r--   0 js        (1000) js        (1000)     5284 2024-03-13 05:10:19.000000 expedantic-0.1.5/submodules/ccorp_yaml_include/ccorp/ruamel/yaml/include/__init__.py
-drwxrwxr-x   0 js        (1000) js        (1000)        0 2024-03-26 06:52:06.913699 expedantic-0.1.5/tests/
--rw-rw-r--   0 js        (1000) js        (1000)     1004 2024-03-13 08:26:54.000000 expedantic-0.1.5/tests/test.py
--rw-rw-r--   0 js        (1000) js        (1000)     1042 2024-03-26 06:49:17.000000 expedantic-0.1.5/tests/test_argparse.py
--rw-rw-r--   0 js        (1000) js        (1000)     2439 2024-03-13 04:01:24.000000 expedantic-0.1.5/tests/test_compound_types.py
--rw-rw-r--   0 js        (1000) js        (1000)     1218 2024-03-13 03:22:37.000000 expedantic-0.1.5/tests/test_constraints.py
--rw-rw-r--   0 js        (1000) js        (1000)     2050 2024-03-13 08:52:05.000000 expedantic-0.1.5/tests/test_include.py
--rw-rw-r--   0 js        (1000) js        (1000)      577 2024-03-13 03:47:40.000000 expedantic-0.1.5/tests/test_literal.py
--rw-rw-r--   0 js        (1000) js        (1000)      812 2024-03-14 01:55:31.000000 expedantic-0.1.5/tests/test_mutually_exclusive_sets.py
+drwxrwxr-x   0 js        (1000) js        (1000)        0 2024-04-02 02:45:06.989810 expedantic-0.1.6/
+-rw-rw-r--   0 js        (1000) js        (1000)     1062 2024-03-12 08:20:45.000000 expedantic-0.1.6/LICENSE
+-rw-r--r--   0 js        (1000) js        (1000)      314 2024-04-02 02:45:06.989810 expedantic-0.1.6/PKG-INFO
+-rw-rw-r--   0 js        (1000) js        (1000)     4193 2024-03-26 06:49:17.000000 expedantic-0.1.6/README.md
+drwxrwxr-x   0 js        (1000) js        (1000)        0 2024-04-02 02:45:06.989810 expedantic-0.1.6/expedantic.egg-info/
+-rw-r--r--   0 js        (1000) js        (1000)      314 2024-04-02 02:45:06.000000 expedantic-0.1.6/expedantic.egg-info/PKG-INFO
+-rw-rw-r--   0 js        (1000) js        (1000)      520 2024-04-02 02:45:06.000000 expedantic-0.1.6/expedantic.egg-info/SOURCES.txt
+-rw-rw-r--   0 js        (1000) js        (1000)        1 2024-04-02 02:45:06.000000 expedantic-0.1.6/expedantic.egg-info/dependency_links.txt
+-rw-rw-r--   0 js        (1000) js        (1000)       59 2024-04-02 02:45:06.000000 expedantic-0.1.6/expedantic.egg-info/requires.txt
+-rw-rw-r--   0 js        (1000) js        (1000)       17 2024-04-02 02:45:06.000000 expedantic-0.1.6/expedantic.egg-info/top_level.txt
+-rw-rw-r--   0 js        (1000) js        (1000)       38 2024-04-02 02:45:06.989810 expedantic-0.1.6/setup.cfg
+-rw-rw-r--   0 js        (1000) js        (1000)      672 2024-04-02 02:43:16.000000 expedantic-0.1.6/setup.py
+drwxrwxr-x   0 js        (1000) js        (1000)        0 2024-04-02 02:45:06.985810 expedantic-0.1.6/src/
+drwxrwxr-x   0 js        (1000) js        (1000)        0 2024-04-02 02:45:06.989810 expedantic-0.1.6/src/expedantic/
+-rw-rw-r--   0 js        (1000) js        (1000)       98 2024-03-12 09:44:20.000000 expedantic-0.1.6/src/expedantic/__init__.py
+-rw-rw-r--   0 js        (1000) js        (1000)    12700 2024-04-02 02:44:09.000000 expedantic-0.1.6/src/expedantic/config_base.py
+-rw-rw-r--   0 js        (1000) js        (1000)      867 2024-03-12 08:26:06.000000 expedantic-0.1.6/src/expedantic/utils.py
+drwxrwxr-x   0 js        (1000) js        (1000)        0 2024-04-02 02:45:06.985810 expedantic-0.1.6/submodules/
+drwxrwxr-x   0 js        (1000) js        (1000)        0 2024-04-02 02:45:06.985810 expedantic-0.1.6/submodules/ccorp_yaml_include/
+drwxrwxr-x   0 js        (1000) js        (1000)        0 2024-04-02 02:45:06.985810 expedantic-0.1.6/submodules/ccorp_yaml_include/ccorp/
+drwxrwxr-x   0 js        (1000) js        (1000)        0 2024-04-02 02:45:06.985810 expedantic-0.1.6/submodules/ccorp_yaml_include/ccorp/ruamel/
+drwxrwxr-x   0 js        (1000) js        (1000)        0 2024-04-02 02:45:06.985810 expedantic-0.1.6/submodules/ccorp_yaml_include/ccorp/ruamel/yaml/
+drwxrwxr-x   0 js        (1000) js        (1000)        0 2024-04-02 02:45:06.985810 expedantic-0.1.6/submodules/ccorp_yaml_include/ccorp/ruamel/yaml/include/
+-rw-rw-r--   0 js        (1000) js        (1000)     5284 2024-03-13 05:10:19.000000 expedantic-0.1.6/submodules/ccorp_yaml_include/ccorp/ruamel/yaml/include/__init__.py
+drwxrwxr-x   0 js        (1000) js        (1000)        0 2024-04-02 02:45:06.989810 expedantic-0.1.6/tests/
+-rw-rw-r--   0 js        (1000) js        (1000)     1004 2024-03-13 08:26:54.000000 expedantic-0.1.6/tests/test.py
+-rw-rw-r--   0 js        (1000) js        (1000)     1170 2024-04-02 02:44:09.000000 expedantic-0.1.6/tests/test_argparse.py
+-rw-rw-r--   0 js        (1000) js        (1000)     2439 2024-03-13 04:01:24.000000 expedantic-0.1.6/tests/test_compound_types.py
+-rw-rw-r--   0 js        (1000) js        (1000)     1218 2024-03-13 03:22:37.000000 expedantic-0.1.6/tests/test_constraints.py
+-rw-rw-r--   0 js        (1000) js        (1000)     2050 2024-03-13 08:52:05.000000 expedantic-0.1.6/tests/test_include.py
+-rw-rw-r--   0 js        (1000) js        (1000)      577 2024-03-13 03:47:40.000000 expedantic-0.1.6/tests/test_literal.py
+-rw-rw-r--   0 js        (1000) js        (1000)      812 2024-04-02 02:12:07.000000 expedantic-0.1.6/tests/test_mutually_exclusive_sets.py
```

### Comparing `expedantic-0.1.5/LICENSE` & `expedantic-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `expedantic-0.1.5/README.md` & `expedantic-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `expedantic-0.1.5/expedantic.egg-info/SOURCES.txt` & `expedantic-0.1.6/expedantic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `expedantic-0.1.5/setup.py` & `expedantic-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="expedantic",
-    version="0.1.5",
+    version="0.1.6",
     packages=["expedantic", "ccorp.ruamel.yaml.include"],
     package_dir={
         # "expedantic": "src",
         "expedantic": "src/expedantic",
         "ccorp.ruamel.yaml.include": "./submodules/ccorp_yaml_include/ccorp/ruamel/yaml/include",
     },
     python_requires=">=3.10",
     install_requires=[
         "pydantic >= 2.6.3",
-        "pydantic_yaml >= 1.2.1",
+        "pydantic_yaml >= 1.3.0",
         "typed-argument-parser",
     ],
     author="rnilva",
     author_email="rnilva849@gmail.com",
     description="",
     license="MIT",
     keywords="",
```

### Comparing `expedantic-0.1.5/src/expedantic/config_base.py` & `expedantic-0.1.6/src/expedantic/config_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import argparse
 import inspect
 import json
+import typing
 
 from abc import ABC
 from collections.abc import Mapping
 from io import IOBase
 from pathlib import Path
 from types import UnionType
 from typing import Any, Callable, Type, Literal, Union, get_origin, get_args
@@ -12,15 +13,15 @@
 
 import pydantic
 import pydantic_yaml
 
 # from ruamel.yaml import YAML
 from ccorp.ruamel.yaml.include import YAML
 
-pydantic_yaml.loader.YAML = YAML
+pydantic_yaml._internals.v2.YAML = YAML
 
 from . import utils
 
 
 class NOT_PROVIDED_CLASS:
     def __repr__(self) -> str:
         return "NOT_PROVIDED"
@@ -208,14 +209,16 @@
                 kwargs = {}
                 kwargs["type"] = tp
 
                 annot_repr = str(tp) if origin else tp.__name__
 
                 if tp is Any:
                     kwargs["type"] = str
+                elif tp is bool:
+                    kwargs["action"] = argparse.BooleanOptionalAction
                 elif origin is Literal:
                     var_type, literals = utils.get_literals(tp, name)
                     kwargs["type"] = var_type
                     kwargs["choices"] = literals
                     annot_repr = annot_repr.replace("typing.", "")
                 elif origin in {list, set, tuple}:
                     kwargs["nargs"] = "*"
@@ -286,23 +289,25 @@
             return d
 
         file_dict = update_recursively(file_dict, nested_args_dict)
         instance = cls.model_validate(file_dict)
 
         return instance
 
-    @pydantic.model_validator(mode="after")
-    def check_mutually_exclusive_sets(self) -> Self:
-        for exclusive_set in self._mutually_exclusive_sets:
-            check = sum(bool(self[key]) for key in exclusive_set) == 1
-            if not check:
-                raise ValueError(
-                    f"Mutual exclusivity has broken. (set: {exclusive_set})"
-                )
-        return self
+    if typing.TYPE_CHECKING:
+
+        @pydantic.model_validator(mode="after")
+        def check_mutually_exclusive_sets(self) -> Self:
+            for exclusive_set in self._mutually_exclusive_sets:
+                check = sum(bool(self[key]) for key in exclusive_set) == 1
+                if not check:
+                    raise ValueError(
+                        f"Mutual exclusivity has broken. (set: {exclusive_set})"
+                    )
+            return self
 
     def __getitem__(self, key: str):
         if key not in self.model_fields:
             raise KeyError(f"Key '{key}' not found.")
         return self.__getattribute__(key)
 
     def __len__(self):
```

### Comparing `expedantic-0.1.5/src/expedantic/utils.py` & `expedantic-0.1.6/src/expedantic/utils.py`

 * *Files identical despite different names*

### Comparing `expedantic-0.1.5/submodules/ccorp_yaml_include/ccorp/ruamel/yaml/include/__init__.py` & `expedantic-0.1.6/submodules/ccorp_yaml_include/ccorp/ruamel/yaml/include/__init__.py`

 * *Files identical despite different names*

### Comparing `expedantic-0.1.5/tests/test.py` & `expedantic-0.1.6/tests/test.py`

 * *Files identical despite different names*

### Comparing `expedantic-0.1.5/tests/test_argparse.py` & `expedantic-0.1.6/tests/test_argparse.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,15 @@
         name: str = "Inner"
         favourite_number: float | int = 3.14
 
     inner: Inner = Inner()
     optional: int | None = 1
     numbers: list[int] = [1, 2, 3]
     my_dict: dict[str, Any] = {}
+    switch: bool = True
 
 
 class TestArgParse(unittest.TestCase):
     def test_arg_parse(self):
         config = Config.parse_args(args=["--optional", "3"])
         self.assertEqual(config.optional, 3)
 
@@ -26,10 +27,13 @@
 
         config = Config.parse_args(
             args=["--inner.name", "Test", "--inner.favourite_number", "7"]
         )
         self.assertEqual(config.inner.name, "Test")
         self.assertEqual(config.inner.favourite_number, 7)
 
+        config = Config.parse_args(args=["--switch", "False"])
+        self.assertFalse(config.switch)
+
     def test_parse_dict(self):
         config = Config.parse_args(args=["--my_dict", "{key: value}"])
         self.assertEqual(config.my_dict.get("key"), "value")
```

### Comparing `expedantic-0.1.5/tests/test_compound_types.py` & `expedantic-0.1.6/tests/test_compound_types.py`

 * *Files identical despite different names*

### Comparing `expedantic-0.1.5/tests/test_constraints.py` & `expedantic-0.1.6/tests/test_constraints.py`

 * *Files identical despite different names*

### Comparing `expedantic-0.1.5/tests/test_include.py` & `expedantic-0.1.6/tests/test_include.py`

 * *Files identical despite different names*

### Comparing `expedantic-0.1.5/tests/test_literal.py` & `expedantic-0.1.6/tests/test_literal.py`

 * *Files identical despite different names*

### Comparing `expedantic-0.1.5/tests/test_mutually_exclusive_sets.py` & `expedantic-0.1.6/tests/test_mutually_exclusive_sets.py`

 * *Files identical despite different names*

