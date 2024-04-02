# Comparing `tmp/mypy-boto3-rolesanywhere-1.34.69.tar.gz` & `tmp/mypy-boto3-rolesanywhere-1.34.76.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-rolesanywhere-1.34.69.tar", last modified: Fri Mar 22 19:19:44 2024, max compression
+gzip compressed data, was "mypy-boto3-rolesanywhere-1.34.76.tar", last modified: Tue Apr  2 19:32:32 2024, max compression
```

## Comparing `mypy-boto3-rolesanywhere-1.34.69.tar` & `mypy-boto3-rolesanywhere-1.34.76.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 19:19:44.298547 mypy-boto3-rolesanywhere-1.34.69/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-22 19:19:17.000000 mypy-boto3-rolesanywhere-1.34.69/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13397 2024-03-22 19:19:44.298547 mypy-boto3-rolesanywhere-1.34.69/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11815 2024-03-22 19:19:17.000000 mypy-boto3-rolesanywhere-1.34.69/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 19:19:44.294547 mypy-boto3-rolesanywhere-1.34.69/mypy_boto3_rolesanywhere/
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-03-22 19:19:17.000000 mypy-boto3-rolesanywhere-1.34.69/mypy_boto3_rolesanywhere/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-03-22 19:19:17.000000 mypy-boto3-rolesanywhere-1.34.69/mypy_boto3_rolesanywhere/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-03-22 19:19:17.000000 mypy-boto3-rolesanywhere-1.34.69/mypy_boto3_rolesanywhere/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20471 2024-03-22 19:19:17.000000 mypy-boto3-rolesanywhere-1.34.69/mypy_boto3_rolesanywhere/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    20468 2024-03-22 19:19:17.000000 mypy-boto3-rolesanywhere-1.34.69/mypy_boto3_rolesanywhere/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9576 2024-03-22 19:19:17.000000 mypy-boto3-rolesanywhere-1.34.69/mypy_boto3_rolesanywhere/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9576 2024-03-22 19:19:17.000000 mypy-boto3-rolesanywhere-1.34.69/mypy_boto3_rolesanywhere/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5078 2024-03-22 19:19:17.000000 mypy-boto3-rolesanywhere-1.34.69/mypy_boto3_rolesanywhere/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5073 2024-03-22 19:19:17.000000 mypy-boto3-rolesanywhere-1.34.69/mypy_boto3_rolesanywhere/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 19:19:17.000000 mypy-boto3-rolesanywhere-1.34.69/mypy_boto3_rolesanywhere/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    13708 2024-03-22 19:19:18.000000 mypy-boto3-rolesanywhere-1.34.69/mypy_boto3_rolesanywhere/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    13708 2024-03-22 19:19:18.000000 mypy-boto3-rolesanywhere-1.34.69/mypy_boto3_rolesanywhere/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-22 19:19:17.000000 mypy-boto3-rolesanywhere-1.34.69/mypy_boto3_rolesanywhere/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 19:19:44.298547 mypy-boto3-rolesanywhere-1.34.69/mypy_boto3_rolesanywhere.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13397 2024-03-22 19:19:44.000000 mypy-boto3-rolesanywhere-1.34.69/mypy_boto3_rolesanywhere.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-03-22 19:19:44.000000 mypy-boto3-rolesanywhere-1.34.69/mypy_boto3_rolesanywhere.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 19:19:44.000000 mypy-boto3-rolesanywhere-1.34.69/mypy_boto3_rolesanywhere.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 19:19:44.000000 mypy-boto3-rolesanywhere-1.34.69/mypy_boto3_rolesanywhere.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-22 19:19:44.000000 mypy-boto3-rolesanywhere-1.34.69/mypy_boto3_rolesanywhere.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-22 19:19:44.000000 mypy-boto3-rolesanywhere-1.34.69/mypy_boto3_rolesanywhere.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 19:19:44.298547 mypy-boto3-rolesanywhere-1.34.69/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-03-22 19:19:16.000000 mypy-boto3-rolesanywhere-1.34.69/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:32:32.171227 mypy-boto3-rolesanywhere-1.34.76/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-02 19:32:03.000000 mypy-boto3-rolesanywhere-1.34.76/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13397 2024-04-02 19:32:32.171227 mypy-boto3-rolesanywhere-1.34.76/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11815 2024-04-02 19:32:03.000000 mypy-boto3-rolesanywhere-1.34.76/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:32:32.171227 mypy-boto3-rolesanywhere-1.34.76/mypy_boto3_rolesanywhere/
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-02 19:32:03.000000 mypy-boto3-rolesanywhere-1.34.76/mypy_boto3_rolesanywhere/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-02 19:32:03.000000 mypy-boto3-rolesanywhere-1.34.76/mypy_boto3_rolesanywhere/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-02 19:32:03.000000 mypy-boto3-rolesanywhere-1.34.76/mypy_boto3_rolesanywhere/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20471 2024-04-02 19:32:03.000000 mypy-boto3-rolesanywhere-1.34.76/mypy_boto3_rolesanywhere/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20468 2024-04-02 19:32:03.000000 mypy-boto3-rolesanywhere-1.34.76/mypy_boto3_rolesanywhere/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9615 2024-04-02 19:32:03.000000 mypy-boto3-rolesanywhere-1.34.76/mypy_boto3_rolesanywhere/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9615 2024-04-02 19:32:03.000000 mypy-boto3-rolesanywhere-1.34.76/mypy_boto3_rolesanywhere/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5078 2024-04-02 19:32:03.000000 mypy-boto3-rolesanywhere-1.34.76/mypy_boto3_rolesanywhere/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5073 2024-04-02 19:32:03.000000 mypy-boto3-rolesanywhere-1.34.76/mypy_boto3_rolesanywhere/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:32:03.000000 mypy-boto3-rolesanywhere-1.34.76/mypy_boto3_rolesanywhere/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    13708 2024-04-02 19:32:04.000000 mypy-boto3-rolesanywhere-1.34.76/mypy_boto3_rolesanywhere/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13708 2024-04-02 19:32:03.000000 mypy-boto3-rolesanywhere-1.34.76/mypy_boto3_rolesanywhere/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-02 19:32:03.000000 mypy-boto3-rolesanywhere-1.34.76/mypy_boto3_rolesanywhere/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:32:32.171227 mypy-boto3-rolesanywhere-1.34.76/mypy_boto3_rolesanywhere.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13397 2024-04-02 19:32:32.000000 mypy-boto3-rolesanywhere-1.34.76/mypy_boto3_rolesanywhere.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-02 19:32:32.000000 mypy-boto3-rolesanywhere-1.34.76/mypy_boto3_rolesanywhere.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 19:32:32.000000 mypy-boto3-rolesanywhere-1.34.76/mypy_boto3_rolesanywhere.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 19:32:32.000000 mypy-boto3-rolesanywhere-1.34.76/mypy_boto3_rolesanywhere.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-02 19:32:32.000000 mypy-boto3-rolesanywhere-1.34.76/mypy_boto3_rolesanywhere.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-02 19:32:32.000000 mypy-boto3-rolesanywhere-1.34.76/mypy_boto3_rolesanywhere.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 19:32:32.171227 mypy-boto3-rolesanywhere-1.34.76/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-02 19:32:03.000000 mypy-boto3-rolesanywhere-1.34.76/setup.py
```

### Comparing `mypy-boto3-rolesanywhere-1.34.69/LICENSE` & `mypy-boto3-rolesanywhere-1.34.76/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rolesanywhere-1.34.69/PKG-INFO` & `mypy-boto3-rolesanywhere-1.34.76/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-rolesanywhere
-Version: 1.34.69
-Summary: Type annotations for boto3.IAMRolesAnywhere 1.34.69 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.76
+Summary: Type annotations for boto3.IAMRolesAnywhere 1.34.76 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rolesanywhere.svg?color=blue)](https://pypi.org/project/mypy-boto3-rolesanywhere)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-rolesanywhere)](https://pepy.tech/project/mypy-boto3-rolesanywhere)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IAMRolesAnywhere 1.34.69](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere)
+[boto3.IAMRolesAnywhere 1.34.76](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-rolesanywhere-1.34.69/README.md` & `mypy-boto3-rolesanywhere-1.34.76/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rolesanywhere.svg?color=blue)](https://pypi.org/project/mypy-boto3-rolesanywhere)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-rolesanywhere)](https://pepy.tech/project/mypy-boto3-rolesanywhere)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IAMRolesAnywhere 1.34.69](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere)
+[boto3.IAMRolesAnywhere 1.34.76](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-rolesanywhere-1.34.69/mypy_boto3_rolesanywhere/__init__.py` & `mypy-boto3-rolesanywhere-1.34.76/mypy_boto3_rolesanywhere/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rolesanywhere-1.34.69/mypy_boto3_rolesanywhere/__init__.pyi` & `mypy-boto3-rolesanywhere-1.34.76/mypy_boto3_rolesanywhere/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rolesanywhere-1.34.69/mypy_boto3_rolesanywhere/__main__.py` & `mypy-boto3-rolesanywhere-1.34.76/mypy_boto3_rolesanywhere/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IAMRolesAnywhere 1.34.69\n"
-        "Version:         1.34.69\n"
+        "Type annotations for boto3.IAMRolesAnywhere 1.34.76\n"
+        "Version:         1.34.76\n"
         "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.69")
+    print("1.34.76")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-rolesanywhere-1.34.69/mypy_boto3_rolesanywhere/client.py` & `mypy-boto3-rolesanywhere-1.34.76/mypy_boto3_rolesanywhere/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rolesanywhere-1.34.69/mypy_boto3_rolesanywhere/client.pyi` & `mypy-boto3-rolesanywhere-1.34.76/mypy_boto3_rolesanywhere/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rolesanywhere-1.34.69/mypy_boto3_rolesanywhere/literals.py` & `mypy-boto3-rolesanywhere-1.34.76/mypy_boto3_rolesanywhere/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,14 +109,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -139,14 +140,15 @@
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
```

### Comparing `mypy-boto3-rolesanywhere-1.34.69/mypy_boto3_rolesanywhere/literals.pyi` & `mypy-boto3-rolesanywhere-1.34.76/mypy_boto3_rolesanywhere/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -109,14 +109,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -139,14 +140,15 @@
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
```

### Comparing `mypy-boto3-rolesanywhere-1.34.69/mypy_boto3_rolesanywhere/paginator.py` & `mypy-boto3-rolesanywhere-1.34.76/mypy_boto3_rolesanywhere/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rolesanywhere-1.34.69/mypy_boto3_rolesanywhere/paginator.pyi` & `mypy-boto3-rolesanywhere-1.34.76/mypy_boto3_rolesanywhere/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rolesanywhere-1.34.69/mypy_boto3_rolesanywhere/type_defs.py` & `mypy-boto3-rolesanywhere-1.34.76/mypy_boto3_rolesanywhere/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rolesanywhere-1.34.69/mypy_boto3_rolesanywhere/type_defs.pyi` & `mypy-boto3-rolesanywhere-1.34.76/mypy_boto3_rolesanywhere/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rolesanywhere-1.34.69/mypy_boto3_rolesanywhere.egg-info/PKG-INFO` & `mypy-boto3-rolesanywhere-1.34.76/mypy_boto3_rolesanywhere.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-rolesanywhere
-Version: 1.34.69
-Summary: Type annotations for boto3.IAMRolesAnywhere 1.34.69 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.76
+Summary: Type annotations for boto3.IAMRolesAnywhere 1.34.76 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rolesanywhere.svg?color=blue)](https://pypi.org/project/mypy-boto3-rolesanywhere)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rolesanywhere/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-rolesanywhere)](https://pepy.tech/project/mypy-boto3-rolesanywhere)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IAMRolesAnywhere 1.34.69](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere)
+[boto3.IAMRolesAnywhere 1.34.76](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-rolesanywhere-1.34.69/mypy_boto3_rolesanywhere.egg-info/SOURCES.txt` & `mypy-boto3-rolesanywhere-1.34.76/mypy_boto3_rolesanywhere.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rolesanywhere-1.34.69/setup.py` & `mypy-boto3-rolesanywhere-1.34.76/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-rolesanywhere",
-    version="1.34.69",
+    version="1.34.76",
     packages=["mypy_boto3_rolesanywhere"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.IAMRolesAnywhere 1.34.69 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3.IAMRolesAnywhere 1.34.76 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

