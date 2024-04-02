# Comparing `tmp/cff2toml-1.2.2.tar.gz` & `tmp/cff2toml-1.2.3.tar.gz`

## Comparing `cff2toml-1.2.2.tar` & `cff2toml-1.2.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 cff2toml-1.2.2/CITATION.cff
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 cff2toml-1.2.2/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 cff2toml-1.2.2/.vscode/settings.json
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 cff2toml-1.2.2/src/cff2toml/__init__.py
--rw-r--r--   0        0        0     6175 2020-02-02 00:00:00.000000 cff2toml-1.2.2/src/cff2toml/cff2toml.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 cff2toml-1.2.2/tests/__init__.py
--rw-r--r--   0        0        0    15382 2020-02-02 00:00:00.000000 cff2toml-1.2.2/tests/test_cff2toml.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 cff2toml-1.2.2/tests/dummy_files/dummy_CITATION.cff
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 cff2toml-1.2.2/tests/dummy_files/dummy_pyproject.toml
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 cff2toml-1.2.2/.gitignore
--rw-r--r--   0        0        0    10938 2020-02-02 00:00:00.000000 cff2toml-1.2.2/LICENSE
--rw-r--r--   0        0        0     7250 2020-02-02 00:00:00.000000 cff2toml-1.2.2/README.md
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 cff2toml-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     8784 2020-02-02 00:00:00.000000 cff2toml-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 cff2toml-1.2.3/CITATION.cff
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 cff2toml-1.2.3/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 cff2toml-1.2.3/.vscode/settings.json
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 cff2toml-1.2.3/src/cff2toml/__init__.py
+-rw-r--r--   0        0        0     6243 2020-02-02 00:00:00.000000 cff2toml-1.2.3/src/cff2toml/cff2toml.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 cff2toml-1.2.3/tests/__init__.py
+-rw-r--r--   0        0        0    16390 2020-02-02 00:00:00.000000 cff2toml-1.2.3/tests/test_cff2toml.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 cff2toml-1.2.3/tests/dummy_files/dummy_CITATION.cff
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 cff2toml-1.2.3/tests/dummy_files/dummy_pyproject.toml
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 cff2toml-1.2.3/.gitignore
+-rw-r--r--   0        0        0    10938 2020-02-02 00:00:00.000000 cff2toml-1.2.3/LICENSE
+-rw-r--r--   0        0        0     7250 2020-02-02 00:00:00.000000 cff2toml-1.2.3/README.md
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 cff2toml-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0     8784 2020-02-02 00:00:00.000000 cff2toml-1.2.3/PKG-INFO
```

### Comparing `cff2toml-1.2.2/CITATION.cff` & `cff2toml-1.2.3/CITATION.cff`

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
-version: "1.2.2"
+version: "1.2.3"
```

### Comparing `cff2toml-1.2.2/.github/workflows/python-publish.yml` & `cff2toml-1.2.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `cff2toml-1.2.2/src/cff2toml/__init__.py` & `cff2toml-1.2.3/src/cff2toml/__init__.py`

 * *Files identical despite different names*

### Comparing `cff2toml-1.2.2/src/cff2toml/cff2toml.py` & `cff2toml-1.2.3/src/cff2toml/cff2toml.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,24 +138,24 @@
     save_cff_object(citation_cff_object, cff_file_path=citation_cff_file_path)
     save_toml_object(toml_object=pyproject_toml_object,
                      toml_file_path=pyproject_toml_file_path)
 
     return pyproject_toml_object, citation_cff_object
 
 
-def get_version_for_pyproject_toml(pyproject_toml_file_path: str) -> str:
+def get_version_for_pyproject_toml(pyproject_toml_file_path: str = DEFAULT_PYPROJECT_TOML_FILE_PATH) -> str:
     pyproject_toml_object: TOMLObject = load_toml_object(
         toml_file_path=pyproject_toml_file_path)
 
     pyproject_toml_version: str = pyproject_toml_object['project']['version']
 
     return pyproject_toml_version
 
 
-def get_version_for_citation_cff(citation_cff_file_path: str) -> str:
+def get_version_for_citation_cff(citation_cff_file_path: str = DEFAULT_CITATION_CFF_FILE_PATH) -> str:
 
     citation_cff_object: CFFObject = load_cff_object(
         cff_file_path=citation_cff_file_path)
 
     citation_cff_version: str = citation_cff_object['version']
 
     return citation_cff_version
```

### Comparing `cff2toml-1.2.2/tests/test_cff2toml.py` & `cff2toml-1.2.3/tests/test_cff2toml.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+from unittest.mock import patch
 import pytest
 import os
-from cff2toml.cff2toml import load_cff_object, load_toml_object, CFFObject, TOMLObject, TransformCFFObjectWithTOMLObjectFunction, TransformTOMLObjectWithCFFObjectFunction, set_version_for_pyproject_toml_and_citation_cff, update_cff_with_toml, update_citation_cff_with_pyproject_toml, update_pyproject_toml_with_citation_cff, update_toml_with_cff
+from cff2toml.cff2toml import get_version_for_citation_cff, get_version_for_pyproject_toml, load_cff_object, load_toml_object, CFFObject, TOMLObject, TransformCFFObjectWithTOMLObjectFunction, TransformTOMLObjectWithCFFObjectFunction, set_version_for_pyproject_toml_and_citation_cff, update_cff_with_toml, update_citation_cff_with_pyproject_toml, update_pyproject_toml_with_citation_cff, update_toml_with_cff
 
 import tempfile
 import shutil
 import os
 
 
 class TempCopiedFile:
@@ -260,17 +261,33 @@
             assert cff_object['license'] == 'Apache-2.0'
             assert cff_object['abstract'] == 'A module that does something cool.'
             assert cff_object['repository-code'] == 'https://github.com/willynilly/somewherecool'
 
 
 def test_get_version_for_citation_cff(dummy_citation_cff_file_path):
     with TempCopiedFile(source_file_path=dummy_citation_cff_file_path) as tmp_dummy_citation_cff_file:
-        cff_object: CFFObject = load_cff_object(
-            cff_file_path=tmp_dummy_citation_cff_file.file_path)
-        assert cff_object['version'] == '0.0.2'
+        version: str = get_version_for_citation_cff(
+            citation_cff_file_path=tmp_dummy_citation_cff_file.file_path)
+        assert version == '0.0.2'
 
 
 def test_get_version_for_pyproject_toml(dummy_pyproject_toml_file_path):
     with TempCopiedFile(source_file_path=dummy_pyproject_toml_file_path) as tmp_dummy_pyproject_toml_file:
-        toml_object: TOMLObject = load_toml_object(
-            toml_file_path=tmp_dummy_pyproject_toml_file.file_path)
-        assert toml_object['project']['version'] == '0.0.1'
+        version: str = get_version_for_pyproject_toml(
+            pyproject_toml_file_path=tmp_dummy_pyproject_toml_file.file_path)
+        assert version == '0.0.1'
+
+
+def test_get_version_for_citation_cff_with_default_file_path(dummy_citation_cff_file_path):
+    with TempCopiedFile(source_file_path=dummy_citation_cff_file_path) as tmp_dummy_citation_cff_file:
+        # patch the default parameters
+        with patch('cff2toml.cff2toml.get_version_for_citation_cff.__defaults__', (tmp_dummy_citation_cff_file.file_path,)):
+            version: str = get_version_for_citation_cff()
+            assert version == '0.0.2'
+
+
+def test_get_version_for_pyproject_toml_with_default_file_path(dummy_pyproject_toml_file_path):
+    with TempCopiedFile(source_file_path=dummy_pyproject_toml_file_path) as tmp_dummy_pyproject_toml_file:
+        # patch the default parameters
+        with patch('cff2toml.cff2toml.get_version_for_pyproject_toml.__defaults__', (tmp_dummy_pyproject_toml_file.file_path,)):
+            version: str = get_version_for_pyproject_toml()
+            assert version == '0.0.1'
```

### Comparing `cff2toml-1.2.2/tests/dummy_files/dummy_CITATION.cff` & `cff2toml-1.2.3/tests/dummy_files/dummy_CITATION.cff`

 * *Files identical despite different names*

### Comparing `cff2toml-1.2.2/tests/dummy_files/dummy_pyproject.toml` & `cff2toml-1.2.3/tests/dummy_files/dummy_pyproject.toml`

 * *Files identical despite different names*

### Comparing `cff2toml-1.2.2/LICENSE` & `cff2toml-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cff2toml-1.2.2/README.md` & `cff2toml-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `cff2toml-1.2.2/pyproject.toml` & `cff2toml-1.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cff2toml"
-version = "1.2.2"
+version = "1.2.3"
 description = "A module to synchronize metadata between TOML and CFF files, including between pyproject.toml and CITATION.cff files."
 readme = "README.md"
 requires-python = ">=3.8"
 license = "Apache-2.0"
 keywords = []
 authors = [
   { name = "Will Riley", email = "wanderingwill@gmail.com" },
```

### Comparing `cff2toml-1.2.2/PKG-INFO` & `cff2toml-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: cff2toml
-Version: 1.2.2
+Version: 1.2.3
 Summary: A module to synchronize metadata between TOML and CFF files, including between pyproject.toml and CITATION.cff files.
 Project-URL: Documentation, https://github.com/willynilly/cff2toml#readme
 Project-URL: Issues, https://github.com/willynilly/cff2toml/issues
 Project-URL: Source, https://github.com/willynilly/cff2toml
 Author-email: Will Riley <wanderingwill@gmail.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
```

