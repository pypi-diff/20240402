# Comparing `tmp/universal_common-1.1.0.tar.gz` & `tmp/universal_common-1.2.0.tar.gz`

## Comparing `universal_common-1.1.0.tar` & `universal_common-1.2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 universal_common-1.1.0/.vscode/settings.json
--rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 universal_common-1.1.0/src/universal_common/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 universal_common-1.1.0/tests/__init__.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 universal_common-1.1.0/tests/test_global.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 universal_common-1.1.0/.gitignore
--rw-r--r--   0        0        0     7167 2020-02-02 00:00:00.000000 universal_common-1.1.0/LICENSE
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 universal_common-1.1.0/README.md
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 universal_common-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 universal_common-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 universal_common-1.2.0/.vscode/settings.json
+-rw-r--r--   0        0        0     5608 2020-02-02 00:00:00.000000 universal_common-1.2.0/src/universal_common/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 universal_common-1.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 universal_common-1.2.0/tests/test_global.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 universal_common-1.2.0/.gitignore
+-rw-r--r--   0        0        0     7167 2020-02-02 00:00:00.000000 universal_common-1.2.0/LICENSE
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 universal_common-1.2.0/README.md
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 universal_common-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 universal_common-1.2.0/PKG-INFO
```

### Comparing `universal_common-1.1.0/LICENSE` & `universal_common-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `universal_common-1.1.0/pyproject.toml` & `universal_common-1.2.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "universal_common"
-version = "1.1.0"
+version = "1.2.0"
 authors = [
   { name="Andrew Ong", email="ong.andrew@gmail.com" },
 ]
 description = "Library that extends the Python base class library with utility functions."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `universal_common-1.1.0/PKG-INFO` & `universal_common-1.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: universal_common
-Version: 1.1.0
+Version: 1.2.0
 Summary: Library that extends the Python base class library with utility functions.
 Author-email: Andrew Ong <ong.andrew@gmail.com>
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

