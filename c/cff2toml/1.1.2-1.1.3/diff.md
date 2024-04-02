# Comparing `tmp/cff2toml-1.1.2.tar.gz` & `tmp/cff2toml-1.1.3.tar.gz`

## Comparing `cff2toml-1.1.2.tar` & `cff2toml-1.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 cff2toml-1.1.2/CITATION.cff
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 cff2toml-1.1.2/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 cff2toml-1.1.2/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-1.1.2/src/cff2toml/__init__.py
--rw-r--r--   0        0        0     5575 2020-02-02 00:00:00.000000 cff2toml-1.1.2/src/cff2toml/cff2toml.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 cff2toml-1.1.2/tests/__init__.py
--rw-r--r--   0        0        0    14689 2020-02-02 00:00:00.000000 cff2toml-1.1.2/tests/test_cff2toml.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 cff2toml-1.1.2/tests/dummy_files/dummy_CITATION.cff
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 cff2toml-1.1.2/tests/dummy_files/dummy_pyproject.toml
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 cff2toml-1.1.2/.gitignore
--rw-r--r--   0        0        0    10938 2020-02-02 00:00:00.000000 cff2toml-1.1.2/LICENSE
--rw-r--r--   0        0        0     6235 2020-02-02 00:00:00.000000 cff2toml-1.1.2/README.md
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 cff2toml-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     7769 2020-02-02 00:00:00.000000 cff2toml-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 cff2toml-1.1.3/CITATION.cff
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 cff2toml-1.1.3/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 cff2toml-1.1.3/.vscode/settings.json
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 cff2toml-1.1.3/src/cff2toml/__init__.py
+-rw-r--r--   0        0        0     5575 2020-02-02 00:00:00.000000 cff2toml-1.1.3/src/cff2toml/cff2toml.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 cff2toml-1.1.3/tests/__init__.py
+-rw-r--r--   0        0        0    14689 2020-02-02 00:00:00.000000 cff2toml-1.1.3/tests/test_cff2toml.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 cff2toml-1.1.3/tests/dummy_files/dummy_CITATION.cff
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 cff2toml-1.1.3/tests/dummy_files/dummy_pyproject.toml
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 cff2toml-1.1.3/.gitignore
+-rw-r--r--   0        0        0    10938 2020-02-02 00:00:00.000000 cff2toml-1.1.3/LICENSE
+-rw-r--r--   0        0        0     6235 2020-02-02 00:00:00.000000 cff2toml-1.1.3/README.md
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 cff2toml-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     7769 2020-02-02 00:00:00.000000 cff2toml-1.1.3/PKG-INFO
```

### Comparing `cff2toml-1.1.2/CITATION.cff` & `cff2toml-1.1.3/CITATION.cff`

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
-version: "1.1.2"
+version: "1.1.3"
```

### Comparing `cff2toml-1.1.2/.github/workflows/python-publish.yml` & `cff2toml-1.1.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `cff2toml-1.1.2/src/cff2toml/cff2toml.py` & `cff2toml-1.1.3/src/cff2toml/cff2toml.py`

 * *Files identical despite different names*

### Comparing `cff2toml-1.1.2/tests/test_cff2toml.py` & `cff2toml-1.1.3/tests/test_cff2toml.py`

 * *Files identical despite different names*

### Comparing `cff2toml-1.1.2/tests/dummy_files/dummy_CITATION.cff` & `cff2toml-1.1.3/tests/dummy_files/dummy_CITATION.cff`

 * *Files identical despite different names*

### Comparing `cff2toml-1.1.2/tests/dummy_files/dummy_pyproject.toml` & `cff2toml-1.1.3/tests/dummy_files/dummy_pyproject.toml`

 * *Files identical despite different names*

### Comparing `cff2toml-1.1.2/LICENSE` & `cff2toml-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cff2toml-1.1.2/README.md` & `cff2toml-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `cff2toml-1.1.2/pyproject.toml` & `cff2toml-1.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cff2toml"
-version = "1.1.2"
+version = "1.1.3"
 description = "A module to synchronize metadata between TOML and CFF files, including between pyproject.toml and CITATION.cff files."
 readme = "README.md"
 requires-python = ">=3.8"
 license = "Apache-2.0"
 keywords = []
 authors = [
   { name = "Will Riley", email = "wanderingwill@gmail.com" },
```

### Comparing `cff2toml-1.1.2/PKG-INFO` & `cff2toml-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: cff2toml
-Version: 1.1.2
+Version: 1.1.3
 Summary: A module to synchronize metadata between TOML and CFF files, including between pyproject.toml and CITATION.cff files.
 Project-URL: Documentation, https://github.com/willynilly/cff2toml#readme
 Project-URL: Issues, https://github.com/willynilly/cff2toml/issues
 Project-URL: Source, https://github.com/willynilly/cff2toml
 Author-email: Will Riley <wanderingwill@gmail.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
```

