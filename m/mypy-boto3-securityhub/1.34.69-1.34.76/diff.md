# Comparing `tmp/mypy-boto3-securityhub-1.34.69.tar.gz` & `tmp/mypy-boto3-securityhub-1.34.76.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-securityhub-1.34.69.tar", last modified: Fri Mar 22 19:19:44 2024, max compression
+gzip compressed data, was "mypy-boto3-securityhub-1.34.76.tar", last modified: Tue Apr  2 19:32:32 2024, max compression
```

## Comparing `mypy-boto3-securityhub-1.34.69.tar` & `mypy-boto3-securityhub-1.34.76.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 19:19:44.618550 mypy-boto3-securityhub-1.34.69/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-22 19:19:24.000000 mypy-boto3-securityhub-1.34.69/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15541 2024-03-22 19:19:44.618550 mypy-boto3-securityhub-1.34.69/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13970 2024-03-22 19:19:24.000000 mypy-boto3-securityhub-1.34.69/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 19:19:44.618550 mypy-boto3-securityhub-1.34.69/mypy_boto3_securityhub/
--rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-03-22 19:19:24.000000 mypy-boto3-securityhub-1.34.69/mypy_boto3_securityhub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-03-22 19:19:24.000000 mypy-boto3-securityhub-1.34.69/mypy_boto3_securityhub/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-03-22 19:19:24.000000 mypy-boto3-securityhub-1.34.69/mypy_boto3_securityhub/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    61446 2024-03-22 19:19:25.000000 mypy-boto3-securityhub-1.34.69/mypy_boto3_securityhub/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    61443 2024-03-22 19:19:24.000000 mypy-boto3-securityhub-1.34.69/mypy_boto3_securityhub/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    16061 2024-03-22 19:19:25.000000 mypy-boto3-securityhub-1.34.69/mypy_boto3_securityhub/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    16061 2024-03-22 19:19:25.000000 mypy-boto3-securityhub-1.34.69/mypy_boto3_securityhub/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    20877 2024-03-22 19:19:25.000000 mypy-boto3-securityhub-1.34.69/mypy_boto3_securityhub/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    20859 2024-03-22 19:19:25.000000 mypy-boto3-securityhub-1.34.69/mypy_boto3_securityhub/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 19:19:24.000000 mypy-boto3-securityhub-1.34.69/mypy_boto3_securityhub/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   475828 2024-03-22 19:19:33.000000 mypy-boto3-securityhub-1.34.69/mypy_boto3_securityhub/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)   475828 2024-03-22 19:19:31.000000 mypy-boto3-securityhub-1.34.69/mypy_boto3_securityhub/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-22 19:19:24.000000 mypy-boto3-securityhub-1.34.69/mypy_boto3_securityhub/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 19:19:44.618550 mypy-boto3-securityhub-1.34.69/mypy_boto3_securityhub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15541 2024-03-22 19:19:44.000000 mypy-boto3-securityhub-1.34.69/mypy_boto3_securityhub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-03-22 19:19:44.000000 mypy-boto3-securityhub-1.34.69/mypy_boto3_securityhub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 19:19:44.000000 mypy-boto3-securityhub-1.34.69/mypy_boto3_securityhub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 19:19:44.000000 mypy-boto3-securityhub-1.34.69/mypy_boto3_securityhub.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-22 19:19:44.000000 mypy-boto3-securityhub-1.34.69/mypy_boto3_securityhub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-22 19:19:44.000000 mypy-boto3-securityhub-1.34.69/mypy_boto3_securityhub.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 19:19:44.618550 mypy-boto3-securityhub-1.34.69/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-03-22 19:19:24.000000 mypy-boto3-securityhub-1.34.69/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:32:32.495226 mypy-boto3-securityhub-1.34.76/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-02 19:32:10.000000 mypy-boto3-securityhub-1.34.76/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15541 2024-04-02 19:32:32.491227 mypy-boto3-securityhub-1.34.76/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13970 2024-04-02 19:32:10.000000 mypy-boto3-securityhub-1.34.76/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:32:32.491227 mypy-boto3-securityhub-1.34.76/mypy_boto3_securityhub/
+-rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-04-02 19:32:10.000000 mypy-boto3-securityhub-1.34.76/mypy_boto3_securityhub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-04-02 19:32:10.000000 mypy-boto3-securityhub-1.34.76/mypy_boto3_securityhub/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-02 19:32:10.000000 mypy-boto3-securityhub-1.34.76/mypy_boto3_securityhub/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61446 2024-04-02 19:32:11.000000 mypy-boto3-securityhub-1.34.76/mypy_boto3_securityhub/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61443 2024-04-02 19:32:11.000000 mypy-boto3-securityhub-1.34.76/mypy_boto3_securityhub/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    16100 2024-04-02 19:32:11.000000 mypy-boto3-securityhub-1.34.76/mypy_boto3_securityhub/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16100 2024-04-02 19:32:11.000000 mypy-boto3-securityhub-1.34.76/mypy_boto3_securityhub/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    20877 2024-04-02 19:32:11.000000 mypy-boto3-securityhub-1.34.76/mypy_boto3_securityhub/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20859 2024-04-02 19:32:11.000000 mypy-boto3-securityhub-1.34.76/mypy_boto3_securityhub/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:32:10.000000 mypy-boto3-securityhub-1.34.76/mypy_boto3_securityhub/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   475828 2024-04-02 19:32:20.000000 mypy-boto3-securityhub-1.34.76/mypy_boto3_securityhub/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   475828 2024-04-02 19:32:17.000000 mypy-boto3-securityhub-1.34.76/mypy_boto3_securityhub/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-02 19:32:10.000000 mypy-boto3-securityhub-1.34.76/mypy_boto3_securityhub/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:32:32.491227 mypy-boto3-securityhub-1.34.76/mypy_boto3_securityhub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15541 2024-04-02 19:32:32.000000 mypy-boto3-securityhub-1.34.76/mypy_boto3_securityhub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-02 19:32:32.000000 mypy-boto3-securityhub-1.34.76/mypy_boto3_securityhub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 19:32:32.000000 mypy-boto3-securityhub-1.34.76/mypy_boto3_securityhub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 19:32:32.000000 mypy-boto3-securityhub-1.34.76/mypy_boto3_securityhub.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-02 19:32:32.000000 mypy-boto3-securityhub-1.34.76/mypy_boto3_securityhub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-02 19:32:32.000000 mypy-boto3-securityhub-1.34.76/mypy_boto3_securityhub.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 19:32:32.495226 mypy-boto3-securityhub-1.34.76/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-04-02 19:32:10.000000 mypy-boto3-securityhub-1.34.76/setup.py
```

### Comparing `mypy-boto3-securityhub-1.34.69/LICENSE` & `mypy-boto3-securityhub-1.34.76/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-securityhub-1.34.69/PKG-INFO` & `mypy-boto3-securityhub-1.34.76/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-securityhub
-Version: 1.34.69
-Summary: Type annotations for boto3.SecurityHub 1.34.69 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.76
+Summary: Type annotations for boto3.SecurityHub 1.34.76 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-securityhub.svg?color=blue)](https://pypi.org/project/mypy-boto3-securityhub)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-securityhub)](https://pepy.tech/project/mypy-boto3-securityhub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SecurityHub 1.34.69](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub)
+[boto3.SecurityHub 1.34.76](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-securityhub-1.34.69/README.md` & `mypy-boto3-securityhub-1.34.76/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-securityhub.svg?color=blue)](https://pypi.org/project/mypy-boto3-securityhub)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-securityhub)](https://pepy.tech/project/mypy-boto3-securityhub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SecurityHub 1.34.69](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub)
+[boto3.SecurityHub 1.34.76](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-securityhub-1.34.69/mypy_boto3_securityhub/__init__.py` & `mypy-boto3-securityhub-1.34.76/mypy_boto3_securityhub/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-securityhub-1.34.69/mypy_boto3_securityhub/__init__.pyi` & `mypy-boto3-securityhub-1.34.76/mypy_boto3_securityhub/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-securityhub-1.34.69/mypy_boto3_securityhub/__main__.py` & `mypy-boto3-securityhub-1.34.76/mypy_boto3_securityhub/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SecurityHub 1.34.69\n"
-        "Version:         1.34.69\n"
+        "Type annotations for boto3.SecurityHub 1.34.76\n"
+        "Version:         1.34.76\n"
         "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub\n"
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

### Comparing `mypy-boto3-securityhub-1.34.69/mypy_boto3_securityhub/client.py` & `mypy-boto3-securityhub-1.34.76/mypy_boto3_securityhub/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-securityhub-1.34.69/mypy_boto3_securityhub/client.pyi` & `mypy-boto3-securityhub-1.34.76/mypy_boto3_securityhub/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-securityhub-1.34.69/mypy_boto3_securityhub/literals.py` & `mypy-boto3-securityhub-1.34.76/mypy_boto3_securityhub/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -249,14 +249,15 @@
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
@@ -279,14 +280,15 @@
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

### Comparing `mypy-boto3-securityhub-1.34.69/mypy_boto3_securityhub/literals.pyi` & `mypy-boto3-securityhub-1.34.76/mypy_boto3_securityhub/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -249,14 +249,15 @@
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
@@ -279,14 +280,15 @@
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

### Comparing `mypy-boto3-securityhub-1.34.69/mypy_boto3_securityhub/paginator.py` & `mypy-boto3-securityhub-1.34.76/mypy_boto3_securityhub/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-securityhub-1.34.69/mypy_boto3_securityhub/paginator.pyi` & `mypy-boto3-securityhub-1.34.76/mypy_boto3_securityhub/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-securityhub-1.34.69/mypy_boto3_securityhub/type_defs.py` & `mypy-boto3-securityhub-1.34.76/mypy_boto3_securityhub/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-securityhub-1.34.69/mypy_boto3_securityhub/type_defs.pyi` & `mypy-boto3-securityhub-1.34.76/mypy_boto3_securityhub/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-securityhub-1.34.69/mypy_boto3_securityhub.egg-info/PKG-INFO` & `mypy-boto3-securityhub-1.34.76/mypy_boto3_securityhub.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-securityhub
-Version: 1.34.69
-Summary: Type annotations for boto3.SecurityHub 1.34.69 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.76
+Summary: Type annotations for boto3.SecurityHub 1.34.76 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-securityhub.svg?color=blue)](https://pypi.org/project/mypy-boto3-securityhub)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-securityhub)](https://pepy.tech/project/mypy-boto3-securityhub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SecurityHub 1.34.69](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub)
+[boto3.SecurityHub 1.34.76](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-securityhub-1.34.69/mypy_boto3_securityhub.egg-info/SOURCES.txt` & `mypy-boto3-securityhub-1.34.76/mypy_boto3_securityhub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-securityhub-1.34.69/setup.py` & `mypy-boto3-securityhub-1.34.76/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-securityhub",
-    version="1.34.69",
+    version="1.34.76",
     packages=["mypy_boto3_securityhub"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.SecurityHub 1.34.69 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3.SecurityHub 1.34.76 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

