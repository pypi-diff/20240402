# Comparing `tmp/cff2toml-1.2.1.tar.gz` & `tmp/cff2toml-1.2.2.tar.gz`

## Comparing `cff2toml-1.2.1.tar` & `cff2toml-1.2.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 cff2toml-1.2.1/CITATION.cff
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 cff2toml-1.2.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 cff2toml-1.2.1/.vscode/settings.json
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 cff2toml-1.2.1/src/cff2toml/__init__.py
--rw-r--r--   0        0        0     6135 2020-02-02 00:00:00.000000 cff2toml-1.2.1/src/cff2toml/cff2toml.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 cff2toml-1.2.1/tests/__init__.py
--rw-r--r--   0        0        0    15382 2020-02-02 00:00:00.000000 cff2toml-1.2.1/tests/test_cff2toml.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 cff2toml-1.2.1/tests/dummy_files/dummy_CITATION.cff
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 cff2toml-1.2.1/tests/dummy_files/dummy_pyproject.toml
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 cff2toml-1.2.1/.gitignore
--rw-r--r--   0        0        0    10938 2020-02-02 00:00:00.000000 cff2toml-1.2.1/LICENSE
--rw-r--r--   0        0        0     7250 2020-02-02 00:00:00.000000 cff2toml-1.2.1/README.md
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 cff2toml-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     8784 2020-02-02 00:00:00.000000 cff2toml-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 cff2toml-1.2.2/CITATION.cff
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 cff2toml-1.2.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 cff2toml-1.2.2/.vscode/settings.json
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 cff2toml-1.2.2/src/cff2toml/__init__.py
+-rw-r--r--   0        0        0     6175 2020-02-02 00:00:00.000000 cff2toml-1.2.2/src/cff2toml/cff2toml.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 cff2toml-1.2.2/tests/__init__.py
+-rw-r--r--   0        0        0    15382 2020-02-02 00:00:00.000000 cff2toml-1.2.2/tests/test_cff2toml.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 cff2toml-1.2.2/tests/dummy_files/dummy_CITATION.cff
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 cff2toml-1.2.2/tests/dummy_files/dummy_pyproject.toml
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 cff2toml-1.2.2/.gitignore
+-rw-r--r--   0        0        0    10938 2020-02-02 00:00:00.000000 cff2toml-1.2.2/LICENSE
+-rw-r--r--   0        0        0     7250 2020-02-02 00:00:00.000000 cff2toml-1.2.2/README.md
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 cff2toml-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     8784 2020-02-02 00:00:00.000000 cff2toml-1.2.2/PKG-INFO
```

### Comparing `cff2toml-1.2.1/CITATION.cff` & `cff2toml-1.2.2/CITATION.cff`

 * *Files 1% similar despite different names*

```diff
@@ -17,8 +17,8 @@
   and CITATION.cff files.
 keywords:
   - Citation File Format
   - TOML
   - pyproject.toml
   - CITATION.cff
 license: Apache-2.0
-version: "1.2.1"
+version: "1.2.2"
```

### Comparing `cff2toml-1.2.1/.github/workflows/python-publish.yml` & `cff2toml-1.2.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `cff2toml-1.2.1/src/cff2toml/__init__.py` & `cff2toml-1.2.2/src/cff2toml/__init__.py`

 * *Files identical despite different names*

### Comparing `cff2toml-1.2.1/src/cff2toml/cff2toml.py` & `cff2toml-1.2.2/src/cff2toml/cff2toml.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from typing import Any, Callable, Dict, Tuple
 import toml
 import yaml
+import os
 
 DEFAULT_PYPROJECT_TOML_FILENAME: str = 'pyproject.toml'
 DEFAULT_CITATION_CFF_FILENAME: str = 'CITATION.cff'
 DEFAULT_DIR: str = '.'
 
-DEFAULT_PYPROJECT_TOML_FILE_PATH: str = DEFAULT_DIR + \
-    DEFAULT_PYPROJECT_TOML_FILENAME
-DEFAULT_CITATION_CFF_FILE_PATH: str = DEFAULT_DIR + DEFAULT_CITATION_CFF_FILENAME
+DEFAULT_PYPROJECT_TOML_FILE_PATH: str = os.path.join(
+    DEFAULT_DIR, DEFAULT_PYPROJECT_TOML_FILENAME)
+DEFAULT_CITATION_CFF_FILE_PATH: str = os.path.join(
+    DEFAULT_DIR, DEFAULT_CITATION_CFF_FILENAME)
 
 TOMLObject = Dict[str, Any]
 CFFObject = Any
 
 TransformCFFObjectWithTOMLObjectFunction = Callable[[
     CFFObject, TOMLObject], CFFObject]
 TransformTOMLObjectWithCFFObjectFunction = Callable[[
```

### Comparing `cff2toml-1.2.1/tests/test_cff2toml.py` & `cff2toml-1.2.2/tests/test_cff2toml.py`

 * *Files identical despite different names*

### Comparing `cff2toml-1.2.1/tests/dummy_files/dummy_CITATION.cff` & `cff2toml-1.2.2/tests/dummy_files/dummy_CITATION.cff`

 * *Files identical despite different names*

### Comparing `cff2toml-1.2.1/tests/dummy_files/dummy_pyproject.toml` & `cff2toml-1.2.2/tests/dummy_files/dummy_pyproject.toml`

 * *Files identical despite different names*

### Comparing `cff2toml-1.2.1/LICENSE` & `cff2toml-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cff2toml-1.2.1/README.md` & `cff2toml-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `cff2toml-1.2.1/pyproject.toml` & `cff2toml-1.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cff2toml"
-version = "1.2.1"
+version = "1.2.2"
 description = "A module to synchronize metadata between TOML and CFF files, including between pyproject.toml and CITATION.cff files."
 readme = "README.md"
 requires-python = ">=3.8"
 license = "Apache-2.0"
 keywords = []
 authors = [
   { name = "Will Riley", email = "wanderingwill@gmail.com" },
```

### Comparing `cff2toml-1.2.1/PKG-INFO` & `cff2toml-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: cff2toml
-Version: 1.2.1
+Version: 1.2.2
 Summary: A module to synchronize metadata between TOML and CFF files, including between pyproject.toml and CITATION.cff files.
 Project-URL: Documentation, https://github.com/willynilly/cff2toml#readme
 Project-URL: Issues, https://github.com/willynilly/cff2toml/issues
 Project-URL: Source, https://github.com/willynilly/cff2toml
 Author-email: Will Riley <wanderingwill@gmail.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
```

