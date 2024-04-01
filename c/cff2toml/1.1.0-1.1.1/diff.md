# Comparing `tmp/cff2toml-1.1.0.tar.gz` & `tmp/cff2toml-1.1.1.tar.gz`

## Comparing `cff2toml-1.1.0.tar` & `cff2toml-1.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 cff2toml-1.1.0/CITATION.cff
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 cff2toml-1.1.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 cff2toml-1.1.0/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-1.1.0/src/cff2toml/__init__.py
--rw-r--r--   0        0        0     5575 2020-02-02 00:00:00.000000 cff2toml-1.1.0/src/cff2toml/cff2toml.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 cff2toml-1.1.0/tests/__init__.py
--rw-r--r--   0        0        0    14689 2020-02-02 00:00:00.000000 cff2toml-1.1.0/tests/test_cff2toml.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 cff2toml-1.1.0/tests/dummy_files/dummy_CITATION.cff
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 cff2toml-1.1.0/tests/dummy_files/dummy_pyproject.toml
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 cff2toml-1.1.0/.gitignore
--rw-r--r--   0        0        0    10938 2020-02-02 00:00:00.000000 cff2toml-1.1.0/LICENSE
--rw-r--r--   0        0        0     5465 2020-02-02 00:00:00.000000 cff2toml-1.1.0/README.md
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 cff2toml-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     6999 2020-02-02 00:00:00.000000 cff2toml-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 cff2toml-1.1.1/CITATION.cff
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 cff2toml-1.1.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 cff2toml-1.1.1/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-1.1.1/src/cff2toml/__init__.py
+-rw-r--r--   0        0        0     5575 2020-02-02 00:00:00.000000 cff2toml-1.1.1/src/cff2toml/cff2toml.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 cff2toml-1.1.1/tests/__init__.py
+-rw-r--r--   0        0        0    14689 2020-02-02 00:00:00.000000 cff2toml-1.1.1/tests/test_cff2toml.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 cff2toml-1.1.1/tests/dummy_files/dummy_CITATION.cff
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 cff2toml-1.1.1/tests/dummy_files/dummy_pyproject.toml
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 cff2toml-1.1.1/.gitignore
+-rw-r--r--   0        0        0    10938 2020-02-02 00:00:00.000000 cff2toml-1.1.1/LICENSE
+-rw-r--r--   0        0        0     5508 2020-02-02 00:00:00.000000 cff2toml-1.1.1/README.md
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 cff2toml-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     7042 2020-02-02 00:00:00.000000 cff2toml-1.1.1/PKG-INFO
```

### Comparing `cff2toml-1.1.0/CITATION.cff` & `cff2toml-1.1.1/CITATION.cff`

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
-version: "1.1.0"
+version: "1.1.1"
```

### Comparing `cff2toml-1.1.0/.github/workflows/python-publish.yml` & `cff2toml-1.1.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `cff2toml-1.1.0/src/cff2toml/cff2toml.py` & `cff2toml-1.1.1/src/cff2toml/cff2toml.py`

 * *Files identical despite different names*

### Comparing `cff2toml-1.1.0/tests/test_cff2toml.py` & `cff2toml-1.1.1/tests/test_cff2toml.py`

 * *Files identical despite different names*

### Comparing `cff2toml-1.1.0/tests/dummy_files/dummy_CITATION.cff` & `cff2toml-1.1.1/tests/dummy_files/dummy_CITATION.cff`

 * *Files identical despite different names*

### Comparing `cff2toml-1.1.0/tests/dummy_files/dummy_pyproject.toml` & `cff2toml-1.1.1/tests/dummy_files/dummy_pyproject.toml`

 * *Files identical despite different names*

### Comparing `cff2toml-1.1.0/LICENSE` & `cff2toml-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cff2toml-1.1.0/README.md` & `cff2toml-1.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 # update CITATION.cff with metadata
 # from pyprojects.cff
 # where both files are located in the working directory
 update_citation_cff_with_pyproject_toml()
 ```
 
 ```python
-from cff2toml import update_pyproject_toml_with_citation_cff
+from cff2toml import update_citation_cff_with_pyproject_toml
 import os
 
 # update CITATION.cff with metadata
 # from pyprojects.cff
 # with custom file paths
 pyproject_toml_file_path: str = os.path.join('somepath', 'pyproject.toml')
 citation_cff_file_path: str = os.path.join('someotherpath', 'CITATION.cff')
@@ -77,15 +77,15 @@
 # set same version for pyproject.toml
 # and CITATION.cff where both files are
 # located in the working directory
 set_version_for_pyproject_toml_and_citation_cff(version="2.0.0")
 ```
 
 ```python
-from cff2toml import update_pyproject_toml_with_citation_cff
+from cff2toml import set_version_for_pyproject_toml_and_citation_cff
 import os
 
 # set same version for pyproject.toml
 # and CITATION.cff where both files
 # have custom file paths
 pyproject_toml_file_path: str = os.path.join('somepath', 'pyproject.toml')
 citation_cff_file_path: str = os.path.join('someotherpath', 'CITATION.cff')
@@ -135,15 +135,15 @@
 toml_object: TOMLObject = load_toml_object(toml_file_path=toml_file_path)
 print(toml_object['somekey'])
 ```
 
 ### Save TOML file object
 
 ```python
-from cff2toml import load_toml_object, TOMLObject
+from cff2toml import load_toml_object, save_toml_object, TOMLObject
 import os
 
 toml_file_path: str = os.path.join('somepath', 'some_toml_file.toml')
 toml_object: TOMLObject = load_toml_object(toml_file_path=toml_file_path)
 print(toml_object['somekey'])
 
 toml_object['somekey'] = 'somevalue'
@@ -161,15 +161,15 @@
 cff_object: CFFObject = load_cff_object(cff_file_path=cff_file_path)
 print(cff_object['somekey'])
 ```
 
 ### Save CFF file object
 
 ```python
-from cff2toml import load_cff_object, CFFObject
+from cff2toml import load_cff_object, save_cff_object, CFFObject
 import os
 
 cff_file_path: str = os.path.join('somepath', 'some_cff_file.cff')
 cff_object: CFFObject = load_cff_object(cff_file_path)
 print(cff_object['somekey'])
 
 cff_object['somekey'] = 'somevalue'
```

### Comparing `cff2toml-1.1.0/pyproject.toml` & `cff2toml-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cff2toml"
-version = "1.1.0"
+version = "1.1.1"
 description = "A module to synchronize metadata between TOML and CFF files, including between pyproject.toml and CITATION.cff files."
 readme = "README.md"
 requires-python = ">=3.8"
 license = "Apache-2.0"
 keywords = []
 authors = [
   { name = "Will Riley", email = "wanderingwill@gmail.com" },
```

### Comparing `cff2toml-1.1.0/PKG-INFO` & `cff2toml-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: cff2toml
-Version: 1.1.0
+Version: 1.1.1
 Summary: A module to synchronize metadata between TOML and CFF files, including between pyproject.toml and CITATION.cff files.
 Project-URL: Documentation, https://github.com/willynilly/cff2toml#readme
 Project-URL: Issues, https://github.com/willynilly/cff2toml/issues
 Project-URL: Source, https://github.com/willynilly/cff2toml
 Author-email: Will Riley <wanderingwill@gmail.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
@@ -88,15 +88,15 @@
 # update CITATION.cff with metadata
 # from pyprojects.cff
 # where both files are located in the working directory
 update_citation_cff_with_pyproject_toml()
 ```
 
 ```python
-from cff2toml import update_pyproject_toml_with_citation_cff
+from cff2toml import update_citation_cff_with_pyproject_toml
 import os
 
 # update CITATION.cff with metadata
 # from pyprojects.cff
 # with custom file paths
 pyproject_toml_file_path: str = os.path.join('somepath', 'pyproject.toml')
 citation_cff_file_path: str = os.path.join('someotherpath', 'CITATION.cff')
@@ -112,15 +112,15 @@
 # set same version for pyproject.toml
 # and CITATION.cff where both files are
 # located in the working directory
 set_version_for_pyproject_toml_and_citation_cff(version="2.0.0")
 ```
 
 ```python
-from cff2toml import update_pyproject_toml_with_citation_cff
+from cff2toml import set_version_for_pyproject_toml_and_citation_cff
 import os
 
 # set same version for pyproject.toml
 # and CITATION.cff where both files
 # have custom file paths
 pyproject_toml_file_path: str = os.path.join('somepath', 'pyproject.toml')
 citation_cff_file_path: str = os.path.join('someotherpath', 'CITATION.cff')
@@ -170,15 +170,15 @@
 toml_object: TOMLObject = load_toml_object(toml_file_path=toml_file_path)
 print(toml_object['somekey'])
 ```
 
 ### Save TOML file object
 
 ```python
-from cff2toml import load_toml_object, TOMLObject
+from cff2toml import load_toml_object, save_toml_object, TOMLObject
 import os
 
 toml_file_path: str = os.path.join('somepath', 'some_toml_file.toml')
 toml_object: TOMLObject = load_toml_object(toml_file_path=toml_file_path)
 print(toml_object['somekey'])
 
 toml_object['somekey'] = 'somevalue'
@@ -196,15 +196,15 @@
 cff_object: CFFObject = load_cff_object(cff_file_path=cff_file_path)
 print(cff_object['somekey'])
 ```
 
 ### Save CFF file object
 
 ```python
-from cff2toml import load_cff_object, CFFObject
+from cff2toml import load_cff_object, save_cff_object, CFFObject
 import os
 
 cff_file_path: str = os.path.join('somepath', 'some_cff_file.cff')
 cff_object: CFFObject = load_cff_object(cff_file_path)
 print(cff_object['somekey'])
 
 cff_object['somekey'] = 'somevalue'
```

