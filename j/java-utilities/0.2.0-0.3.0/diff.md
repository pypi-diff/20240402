# Comparing `tmp/java-utilities-0.2.0.tar.gz` & `tmp/java-utilities-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "java-utilities-0.2.0.tar", last modified: Mon Aug 22 21:00:14 2022, max compression
+gzip compressed data, was "java-utilities-0.3.0.tar", last modified: Tue Apr  2 20:56:35 2024, max compression
```

## Comparing `java-utilities-0.2.0.tar` & `java-utilities-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 devin     (1000) devin     (1000)        0 2022-08-22 21:00:14.797520 java-utilities-0.2.0/
--rw-r--r--   0 devin     (1000) devin     (1000)    11358 2022-08-18 17:13:04.000000 java-utilities-0.2.0/LICENSE
--rw-r--r--   0 devin     (1000) devin     (1000)       22 2022-08-18 19:44:01.000000 java-utilities-0.2.0/MANIFEST.in
--rw-r--r--   0 devin     (1000) devin     (1000)     1292 2022-08-22 21:00:14.797520 java-utilities-0.2.0/PKG-INFO
--rw-r--r--   0 devin     (1000) devin     (1000)      642 2022-08-18 19:25:26.000000 java-utilities-0.2.0/README-pypi.md
--rw-r--r--   0 devin     (1000) devin     (1000)     1087 2022-08-18 18:52:50.000000 java-utilities-0.2.0/README.md
--rw-r--r--   0 devin     (1000) devin     (1000)       98 2022-08-18 01:37:05.000000 java-utilities-0.2.0/pyproject.toml
--rw-r--r--   0 devin     (1000) devin     (1000)     1180 2022-08-22 21:00:14.798520 java-utilities-0.2.0/setup.cfg
-drwxr-xr-x   0 devin     (1000) devin     (1000)        0 2022-08-22 21:00:14.791520 java-utilities-0.2.0/src/
-drwxr-xr-x   0 devin     (1000) devin     (1000)        0 2022-08-22 21:00:14.791520 java-utilities-0.2.0/src/main/
-drwxr-xr-x   0 devin     (1000) devin     (1000)        0 2022-08-22 21:00:14.791520 java-utilities-0.2.0/src/main/python/
-drwxr-xr-x   0 devin     (1000) devin     (1000)        0 2022-08-22 21:00:14.797520 java-utilities-0.2.0/src/main/python/java_utilities/
--rw-r--r--   0 devin     (1000) devin     (1000)     2953 2022-08-22 20:59:39.000000 java-utilities-0.2.0/src/main/python/java_utilities/__init__.py
--rw-r--r--   0 devin     (1000) devin     (1000)      617 2022-08-18 19:23:46.000000 java-utilities-0.2.0/src/main/python/java_utilities/_entrypoints.py
-drwxr-xr-x   0 devin     (1000) devin     (1000)        0 2022-08-22 21:00:14.797520 java-utilities-0.2.0/src/main/python/java_utilities/_jars/
--rw-r--r--   0 devin     (1000) devin     (1000)       38 2022-08-18 18:34:56.000000 java-utilities-0.2.0/src/main/python/java_utilities/_jars/__init__.py
--rw-r--r--   0 devin     (1000) devin     (1000)      561 2022-08-18 16:59:24.000000 java-utilities-0.2.0/src/main/python/java_utilities/_jars/utilities.jar
-drwxr-xr-x   0 devin     (1000) devin     (1000)        0 2022-08-22 21:00:14.797520 java-utilities-0.2.0/src/main/python/java_utilities.egg-info/
--rw-r--r--   0 devin     (1000) devin     (1000)     1292 2022-08-22 21:00:14.000000 java-utilities-0.2.0/src/main/python/java_utilities.egg-info/PKG-INFO
--rw-r--r--   0 devin     (1000) devin     (1000)      532 2022-08-22 21:00:14.000000 java-utilities-0.2.0/src/main/python/java_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 devin     (1000) devin     (1000)        1 2022-08-22 21:00:14.000000 java-utilities-0.2.0/src/main/python/java_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 devin     (1000) devin     (1000)      234 2022-08-22 21:00:14.000000 java-utilities-0.2.0/src/main/python/java_utilities.egg-info/entry_points.txt
--rw-r--r--   0 devin     (1000) devin     (1000)       15 2022-08-22 21:00:14.000000 java-utilities-0.2.0/src/main/python/java_utilities.egg-info/top_level.txt
+drwxr-xr-x   0 devin     (1000) devin     (1000)        0 2024-04-02 20:56:35.968341 java-utilities-0.3.0/
+-rw-r--r--   0 devin     (1000) devin     (1000)    11358 2022-08-18 17:13:04.000000 java-utilities-0.3.0/LICENSE
+-rw-r--r--   0 devin     (1000) devin     (1000)       22 2022-08-18 19:44:01.000000 java-utilities-0.3.0/MANIFEST.in
+-rw-r--r--   0 devin     (1000) devin     (1000)     1304 2024-04-02 20:56:35.968341 java-utilities-0.3.0/PKG-INFO
+-rw-r--r--   0 devin     (1000) devin     (1000)      642 2022-08-18 19:25:26.000000 java-utilities-0.3.0/README-pypi.md
+-rw-r--r--   0 devin     (1000) devin     (1000)     1248 2024-04-02 20:31:39.000000 java-utilities-0.3.0/README.md
+-rw-r--r--   0 devin     (1000) devin     (1000)       98 2024-04-02 20:55:09.000000 java-utilities-0.3.0/pyproject.toml
+-rw-r--r--   0 devin     (1000) devin     (1000)     1192 2024-04-02 20:56:35.969342 java-utilities-0.3.0/setup.cfg
+drwxr-xr-x   0 devin     (1000) devin     (1000)        0 2024-04-02 20:56:35.966342 java-utilities-0.3.0/src/
+drwxr-xr-x   0 devin     (1000) devin     (1000)        0 2024-04-02 20:56:35.966342 java-utilities-0.3.0/src/main/
+drwxr-xr-x   0 devin     (1000) devin     (1000)        0 2024-04-02 20:56:35.966342 java-utilities-0.3.0/src/main/python/
+drwxr-xr-x   0 devin     (1000) devin     (1000)        0 2024-04-02 20:56:35.967342 java-utilities-0.3.0/src/main/python/java_utilities/
+-rw-r--r--   0 devin     (1000) devin     (1000)     3143 2024-04-02 20:55:51.000000 java-utilities-0.3.0/src/main/python/java_utilities/__init__.py
+-rw-r--r--   0 devin     (1000) devin     (1000)      617 2022-08-18 19:23:46.000000 java-utilities-0.3.0/src/main/python/java_utilities/_entrypoints.py
+drwxr-xr-x   0 devin     (1000) devin     (1000)        0 2024-04-02 20:56:35.968341 java-utilities-0.3.0/src/main/python/java_utilities/_jars/
+-rw-r--r--   0 devin     (1000) devin     (1000)       38 2022-08-18 18:34:56.000000 java-utilities-0.3.0/src/main/python/java_utilities/_jars/__init__.py
+-rw-r--r--   0 devin     (1000) devin     (1000)      561 2022-08-18 16:59:24.000000 java-utilities-0.3.0/src/main/python/java_utilities/_jars/utilities.jar
+drwxr-xr-x   0 devin     (1000) devin     (1000)        0 2024-04-02 20:56:35.968341 java-utilities-0.3.0/src/main/python/java_utilities.egg-info/
+-rw-r--r--   0 devin     (1000) devin     (1000)     1304 2024-04-02 20:56:35.000000 java-utilities-0.3.0/src/main/python/java_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 devin     (1000) devin     (1000)      532 2024-04-02 20:56:35.000000 java-utilities-0.3.0/src/main/python/java_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 devin     (1000) devin     (1000)        1 2024-04-02 20:56:35.000000 java-utilities-0.3.0/src/main/python/java_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 devin     (1000) devin     (1000)      234 2024-04-02 20:56:35.000000 java-utilities-0.3.0/src/main/python/java_utilities.egg-info/entry_points.txt
+-rw-r--r--   0 devin     (1000) devin     (1000)       15 2024-04-02 20:56:35.000000 java-utilities-0.3.0/src/main/python/java_utilities.egg-info/top_level.txt
```

### Comparing `java-utilities-0.2.0/LICENSE` & `java-utilities-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `java-utilities-0.2.0/PKG-INFO` & `java-utilities-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: java-utilities
-Version: 0.2.0
+Version: 0.3.0
 Summary: Java utilities
 Home-page: https://github.com/devinrsmith/java-utilities
 Author: Devin Smith
 Author-email: devinsmith@deephaven.io
 Project-URL: Source Code, https://github.com/devinrsmith/java-utilities
 Project-URL: Bug Tracker, https://github.com/devinrsmith/java-utilities/issues
 Keywords: java,utility
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # java-utilities
 
 `java-utilities` is a helper package to run and introspect a `java` binary.
 It can be used as a library, or with the provided standalone scripts.
```

### Comparing `java-utilities-0.2.0/README-pypi.md` & `java-utilities-0.3.0/README-pypi.md`

 * *Files identical despite different names*

### Comparing `java-utilities-0.2.0/README.md` & `java-utilities-0.3.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # java-utilities
 
-`java-utilities` is a very small `utility.jar` (<1KiB) that provides simple Java programs.
+`java-utilities` provides a very small 
+[utilities.jar](https://github.com/devinrsmith/java-utilities/raw/main/src/main/python/java_utilities/_jars/utilities.jar) (<1KiB) for simple Java programs.
 
 It has zero dependencies.
 
 Simple stdout for easy integration with other tools / languages.
 
 Works with Java 8+.
 
@@ -30,8 +31,8 @@
 
 The [java-utilities PyPi package](https://pypi.org/project/java-utilities/) provides `java-utilities` as a Python library.
 
 See [README-pypi.md](README-pypi.md) for more information.
 
 ## JAR
 
-The [utilities.jar](src/main/python/java_utilities/_jars/utilities.jar) is checked into the repository (as opposed to uploaded to Maven Central) as it is unlikely to be depended on as a Java library.
+The [utilities.jar](https://github.com/devinrsmith/java-utilities/raw/main/src/main/python/java_utilities/_jars/utilities.jar) is checked into the repository (as opposed to uploaded to Maven Central) as it is unlikely to be depended on as a Java library.
```

### Comparing `java-utilities-0.2.0/setup.cfg` & `java-utilities-0.3.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 project_urls = 
 	Source Code = https://github.com/devinrsmith/java-utilities
 	Bug Tracker = https://github.com/devinrsmith/java-utilities/issues
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: Apache Software License
 	Operating System :: OS Independent
-	Development Status :: 3 - Alpha
+	Development Status :: 5 - Production/Stable
 keywords = java, utility
 author = Devin Smith
 author_email = devinsmith@deephaven.io
 platforms = any
 
 [options]
 package_dir =
```

### Comparing `java-utilities-0.2.0/src/main/python/java_utilities/__init__.py` & `java-utilities-0.3.0/src/main/python/java_utilities/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 from . import _jars
 from typing import Optional, Union
 import os
 import pathlib
 import subprocess
+import sys
 import importlib.resources
 
 
-__version__ = "0.2.0"
+__version__ = "0.3.0"
 
 _JAR_NAME = "utilities.jar"
 
 _LOOKUP_PROPERTIES_CLASS_NAME = "LookupProperty"
 
 
 def _jar():
-    return importlib.resources.path(_jars.__package__, _JAR_NAME)
+    if sys.version_info < (3, 9):
+        return importlib.resources.path(_jars.__package__, _JAR_NAME)
+    else:
+        return importlib.resources.as_file(
+            importlib.resources.files(_jars.__package__).joinpath(_JAR_NAME)
+        )
 
 
 def _java_executable():
     return "java.exe" if os.name == "nt" else "java"
 
 
 def _java_home():
```

### Comparing `java-utilities-0.2.0/src/main/python/java_utilities/_entrypoints.py` & `java-utilities-0.3.0/src/main/python/java_utilities/_entrypoints.py`

 * *Files identical despite different names*

### Comparing `java-utilities-0.2.0/src/main/python/java_utilities/_jars/utilities.jar` & `java-utilities-0.3.0/src/main/python/java_utilities/_jars/utilities.jar`

 * *Files identical despite different names*

### Comparing `java-utilities-0.2.0/src/main/python/java_utilities.egg-info/PKG-INFO` & `java-utilities-0.3.0/src/main/python/java_utilities.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: java-utilities
-Version: 0.2.0
+Version: 0.3.0
 Summary: Java utilities
 Home-page: https://github.com/devinrsmith/java-utilities
 Author: Devin Smith
 Author-email: devinsmith@deephaven.io
 Project-URL: Source Code, https://github.com/devinrsmith/java-utilities
 Project-URL: Bug Tracker, https://github.com/devinrsmith/java-utilities/issues
 Keywords: java,utility
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # java-utilities
 
 `java-utilities` is a helper package to run and introspect a `java` binary.
 It can be used as a library, or with the provided standalone scripts.
```

### Comparing `java-utilities-0.2.0/src/main/python/java_utilities.egg-info/SOURCES.txt` & `java-utilities-0.3.0/src/main/python/java_utilities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

