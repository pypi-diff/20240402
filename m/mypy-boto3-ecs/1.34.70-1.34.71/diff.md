# Comparing `tmp/mypy-boto3-ecs-1.34.70.tar.gz` & `tmp/mypy-boto3-ecs-1.34.71.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ecs-1.34.70.tar", last modified: Mon Mar 25 19:34:00 2024, max compression
+gzip compressed data, was "mypy-boto3-ecs-1.34.71.tar", last modified: Tue Mar 26 19:32:58 2024, max compression
```

## Comparing `mypy-boto3-ecs-1.34.70.tar` & `mypy-boto3-ecs-1.34.71.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 19:34:00.473657 mypy-boto3-ecs-1.34.70/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-25 19:33:12.000000 mypy-boto3-ecs-1.34.70/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14486 2024-03-25 19:34:00.469657 mypy-boto3-ecs-1.34.70/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12947 2024-03-25 19:33:12.000000 mypy-boto3-ecs-1.34.70/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 19:34:00.469657 mypy-boto3-ecs-1.34.70/mypy_boto3_ecs/
--rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-03-25 19:33:12.000000 mypy-boto3-ecs-1.34.70/mypy_boto3_ecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-03-25 19:33:12.000000 mypy-boto3-ecs-1.34.70/mypy_boto3_ecs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-03-25 19:33:12.000000 mypy-boto3-ecs-1.34.70/mypy_boto3_ecs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    50493 2024-03-25 19:33:13.000000 mypy-boto3-ecs-1.34.70/mypy_boto3_ecs/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    50490 2024-03-25 19:33:12.000000 mypy-boto3-ecs-1.34.70/mypy_boto3_ecs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    16737 2024-03-25 19:33:13.000000 mypy-boto3-ecs-1.34.70/mypy_boto3_ecs/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    16737 2024-03-25 19:33:13.000000 mypy-boto3-ecs-1.34.70/mypy_boto3_ecs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11526 2024-03-25 19:33:13.000000 mypy-boto3-ecs-1.34.70/mypy_boto3_ecs/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    11516 2024-03-25 19:33:13.000000 mypy-boto3-ecs-1.34.70/mypy_boto3_ecs/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 19:33:12.000000 mypy-boto3-ecs-1.34.70/mypy_boto3_ecs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    80953 2024-03-25 19:33:15.000000 mypy-boto3-ecs-1.34.70/mypy_boto3_ecs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    80953 2024-03-25 19:33:14.000000 mypy-boto3-ecs-1.34.70/mypy_boto3_ecs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-25 19:33:12.000000 mypy-boto3-ecs-1.34.70/mypy_boto3_ecs/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-03-25 19:33:13.000000 mypy-boto3-ecs-1.34.70/mypy_boto3_ecs/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-03-25 19:33:13.000000 mypy-boto3-ecs-1.34.70/mypy_boto3_ecs/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 19:34:00.469657 mypy-boto3-ecs-1.34.70/mypy_boto3_ecs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14486 2024-03-25 19:34:00.000000 mypy-boto3-ecs-1.34.70/mypy_boto3_ecs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-03-25 19:34:00.000000 mypy-boto3-ecs-1.34.70/mypy_boto3_ecs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 19:34:00.000000 mypy-boto3-ecs-1.34.70/mypy_boto3_ecs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 19:34:00.000000 mypy-boto3-ecs-1.34.70/mypy_boto3_ecs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-25 19:34:00.000000 mypy-boto3-ecs-1.34.70/mypy_boto3_ecs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-25 19:34:00.000000 mypy-boto3-ecs-1.34.70/mypy_boto3_ecs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 19:34:00.473657 mypy-boto3-ecs-1.34.70/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-03-25 19:33:12.000000 mypy-boto3-ecs-1.34.70/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 19:32:58.896927 mypy-boto3-ecs-1.34.71/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-26 19:32:42.000000 mypy-boto3-ecs-1.34.71/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14486 2024-03-26 19:32:58.896927 mypy-boto3-ecs-1.34.71/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12947 2024-03-26 19:32:42.000000 mypy-boto3-ecs-1.34.71/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 19:32:58.896927 mypy-boto3-ecs-1.34.71/mypy_boto3_ecs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-03-26 19:32:42.000000 mypy-boto3-ecs-1.34.71/mypy_boto3_ecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-03-26 19:32:42.000000 mypy-boto3-ecs-1.34.71/mypy_boto3_ecs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-03-26 19:32:42.000000 mypy-boto3-ecs-1.34.71/mypy_boto3_ecs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50493 2024-03-26 19:32:42.000000 mypy-boto3-ecs-1.34.71/mypy_boto3_ecs/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50490 2024-03-26 19:32:42.000000 mypy-boto3-ecs-1.34.71/mypy_boto3_ecs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    16737 2024-03-26 19:32:43.000000 mypy-boto3-ecs-1.34.71/mypy_boto3_ecs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16737 2024-03-26 19:32:43.000000 mypy-boto3-ecs-1.34.71/mypy_boto3_ecs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11526 2024-03-26 19:32:42.000000 mypy-boto3-ecs-1.34.71/mypy_boto3_ecs/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11516 2024-03-26 19:32:42.000000 mypy-boto3-ecs-1.34.71/mypy_boto3_ecs/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:32:42.000000 mypy-boto3-ecs-1.34.71/mypy_boto3_ecs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    80953 2024-03-26 19:32:45.000000 mypy-boto3-ecs-1.34.71/mypy_boto3_ecs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80953 2024-03-26 19:32:43.000000 mypy-boto3-ecs-1.34.71/mypy_boto3_ecs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-26 19:32:42.000000 mypy-boto3-ecs-1.34.71/mypy_boto3_ecs/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-03-26 19:32:42.000000 mypy-boto3-ecs-1.34.71/mypy_boto3_ecs/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-03-26 19:32:42.000000 mypy-boto3-ecs-1.34.71/mypy_boto3_ecs/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 19:32:58.896927 mypy-boto3-ecs-1.34.71/mypy_boto3_ecs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14486 2024-03-26 19:32:58.000000 mypy-boto3-ecs-1.34.71/mypy_boto3_ecs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-03-26 19:32:58.000000 mypy-boto3-ecs-1.34.71/mypy_boto3_ecs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 19:32:58.000000 mypy-boto3-ecs-1.34.71/mypy_boto3_ecs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 19:32:58.000000 mypy-boto3-ecs-1.34.71/mypy_boto3_ecs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-26 19:32:58.000000 mypy-boto3-ecs-1.34.71/mypy_boto3_ecs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-26 19:32:58.000000 mypy-boto3-ecs-1.34.71/mypy_boto3_ecs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 19:32:58.896927 mypy-boto3-ecs-1.34.71/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-03-26 19:32:42.000000 mypy-boto3-ecs-1.34.71/setup.py
```

### Comparing `mypy-boto3-ecs-1.34.70/LICENSE` & `mypy-boto3-ecs-1.34.71/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.34.70/PKG-INFO` & `mypy-boto3-ecs-1.34.71/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ecs
-Version: 1.34.70
-Summary: Type annotations for boto3.ECS 1.34.70 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.71
+Summary: Type annotations for boto3.ECS 1.34.71 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ecs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ecs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ecs)](https://pepy.tech/project/mypy-boto3-ecs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ECS 1.34.70](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS)
+[boto3.ECS 1.34.71](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-ecs-1.34.70/README.md` & `mypy-boto3-ecs-1.34.71/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ecs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ecs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ecs)](https://pepy.tech/project/mypy-boto3-ecs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ECS 1.34.70](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS)
+[boto3.ECS 1.34.71](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-ecs-1.34.70/mypy_boto3_ecs/__init__.py` & `mypy-boto3-ecs-1.34.71/mypy_boto3_ecs/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.34.70/mypy_boto3_ecs/__init__.pyi` & `mypy-boto3-ecs-1.34.71/mypy_boto3_ecs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.34.70/mypy_boto3_ecs/__main__.py` & `mypy-boto3-ecs-1.34.71/mypy_boto3_ecs/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ECS 1.34.70\n"
-        "Version:         1.34.70\n"
+        "Type annotations for boto3.ECS 1.34.71\n"
+        "Version:         1.34.71\n"
         "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.70")
+    print("1.34.71")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-ecs-1.34.70/mypy_boto3_ecs/client.py` & `mypy-boto3-ecs-1.34.71/mypy_boto3_ecs/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.34.70/mypy_boto3_ecs/client.pyi` & `mypy-boto3-ecs-1.34.71/mypy_boto3_ecs/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.34.70/mypy_boto3_ecs/literals.py` & `mypy-boto3-ecs-1.34.71/mypy_boto3_ecs/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.34.70/mypy_boto3_ecs/literals.pyi` & `mypy-boto3-ecs-1.34.71/mypy_boto3_ecs/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.34.70/mypy_boto3_ecs/paginator.py` & `mypy-boto3-ecs-1.34.71/mypy_boto3_ecs/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.34.70/mypy_boto3_ecs/paginator.pyi` & `mypy-boto3-ecs-1.34.71/mypy_boto3_ecs/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.34.70/mypy_boto3_ecs/type_defs.py` & `mypy-boto3-ecs-1.34.71/mypy_boto3_ecs/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.34.70/mypy_boto3_ecs/type_defs.pyi` & `mypy-boto3-ecs-1.34.71/mypy_boto3_ecs/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.34.70/mypy_boto3_ecs/waiter.py` & `mypy-boto3-ecs-1.34.71/mypy_boto3_ecs/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.34.70/mypy_boto3_ecs/waiter.pyi` & `mypy-boto3-ecs-1.34.71/mypy_boto3_ecs/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.34.70/mypy_boto3_ecs.egg-info/PKG-INFO` & `mypy-boto3-ecs-1.34.71/mypy_boto3_ecs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ecs
-Version: 1.34.70
-Summary: Type annotations for boto3.ECS 1.34.70 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.71
+Summary: Type annotations for boto3.ECS 1.34.71 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ecs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ecs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ecs)](https://pepy.tech/project/mypy-boto3-ecs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ECS 1.34.70](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS)
+[boto3.ECS 1.34.71](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-ecs-1.34.70/mypy_boto3_ecs.egg-info/SOURCES.txt` & `mypy-boto3-ecs-1.34.71/mypy_boto3_ecs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.34.70/setup.py` & `mypy-boto3-ecs-1.34.71/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ecs",
-    version="1.34.70",
+    version="1.34.71",
     packages=["mypy_boto3_ecs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.ECS 1.34.70 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3.ECS 1.34.71 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

