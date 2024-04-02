# Comparing `tmp/cff2toml-1.1.3.tar.gz` & `tmp/cff2toml-1.2.0.tar.gz`

## Comparing `cff2toml-1.1.3.tar` & `cff2toml-1.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 cff2toml-1.1.3/CITATION.cff
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 cff2toml-1.1.3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 cff2toml-1.1.3/.vscode/settings.json
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 cff2toml-1.1.3/src/cff2toml/__init__.py
--rw-r--r--   0        0        0     5575 2020-02-02 00:00:00.000000 cff2toml-1.1.3/src/cff2toml/cff2toml.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 cff2toml-1.1.3/tests/__init__.py
--rw-r--r--   0        0        0    14689 2020-02-02 00:00:00.000000 cff2toml-1.1.3/tests/test_cff2toml.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 cff2toml-1.1.3/tests/dummy_files/dummy_CITATION.cff
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 cff2toml-1.1.3/tests/dummy_files/dummy_pyproject.toml
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 cff2toml-1.1.3/.gitignore
--rw-r--r--   0        0        0    10938 2020-02-02 00:00:00.000000 cff2toml-1.1.3/LICENSE
--rw-r--r--   0        0        0     6235 2020-02-02 00:00:00.000000 cff2toml-1.1.3/README.md
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 cff2toml-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     7769 2020-02-02 00:00:00.000000 cff2toml-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 cff2toml-1.2.0/CITATION.cff
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 cff2toml-1.2.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 cff2toml-1.2.0/.vscode/settings.json
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 cff2toml-1.2.0/src/cff2toml/__init__.py
+-rw-r--r--   0        0        0     6135 2020-02-02 00:00:00.000000 cff2toml-1.2.0/src/cff2toml/cff2toml.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 cff2toml-1.2.0/tests/__init__.py
+-rw-r--r--   0        0        0    15386 2020-02-02 00:00:00.000000 cff2toml-1.2.0/tests/test_cff2toml.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 cff2toml-1.2.0/tests/dummy_files/dummy_CITATION.cff
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 cff2toml-1.2.0/tests/dummy_files/dummy_pyproject.toml
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 cff2toml-1.2.0/.gitignore
+-rw-r--r--   0        0        0    10938 2020-02-02 00:00:00.000000 cff2toml-1.2.0/LICENSE
+-rw-r--r--   0        0        0     7250 2020-02-02 00:00:00.000000 cff2toml-1.2.0/README.md
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 cff2toml-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     8784 2020-02-02 00:00:00.000000 cff2toml-1.2.0/PKG-INFO
```

### Comparing `cff2toml-1.1.3/CITATION.cff` & `cff2toml-1.2.0/CITATION.cff`

 * *Files 2% similar despite different names*

```diff
@@ -17,8 +17,8 @@
   and CITATION.cff files.
 keywords:
   - Citation File Format
   - TOML
   - pyproject.toml
   - CITATION.cff
 license: Apache-2.0
-version: "1.1.3"
+version: "1.2.0"
```

### Comparing `cff2toml-1.1.3/.github/workflows/python-publish.yml` & `cff2toml-1.2.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `cff2toml-1.1.3/src/cff2toml/cff2toml.py` & `cff2toml-1.2.0/src/cff2toml/cff2toml.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Callable, Dict, Tuple, Union
+from typing import Any, Callable, Dict, Tuple
 import toml
 import yaml
 
 DEFAULT_PYPROJECT_TOML_FILENAME: str = 'pyproject.toml'
 DEFAULT_CITATION_CFF_FILENAME: str = 'CITATION.cff'
 DEFAULT_DIR: str = '.'
 
@@ -134,7 +134,26 @@
     pyproject_toml_object['project']['version'] = version
 
     save_cff_object(citation_cff_object, cff_file_path=citation_cff_file_path)
     save_toml_object(toml_object=pyproject_toml_object,
                      toml_file_path=pyproject_toml_file_path)
 
     return pyproject_toml_object, citation_cff_object
+
+
+def get_version_for_pyproject_toml(pyproject_toml_file_path: str) -> str:
+    pyproject_toml_object: TOMLObject = load_toml_object(
+        toml_file_path=pyproject_toml_file_path)
+
+    pyproject_toml_version: str = pyproject_toml_object['project']['version']
+
+    return pyproject_toml_version
+
+
+def get_version_for_citation_cff(citation_cff_file_path: str) -> str:
+
+    citation_cff_object: CFFObject = load_cff_object(
+        cff_file_path=citation_cff_file_path)
+
+    citation_cff_version: str = citation_cff_object['version']
+
+    return citation_cff_version
```

### Comparing `cff2toml-1.1.3/tests/test_cff2toml.py` & `cff2toml-1.2.0/tests/test_cff2toml.py`

 * *Files 4% similar despite different names*

```diff
@@ -203,15 +203,15 @@
             assert cff_object['version'] == '0.0.1'
             assert cff_object['title'] == 'someuncooltool'
             assert cff_object['license'] == 'Apache-1.0'
             assert cff_object['abstract'] == 'A module that does something uncool.'
             assert cff_object['repository-code'] == 'https://github.com/willnilly/somewhereuncool'
 
 
-def test_set_version_for_citation_cff_with_pyproject_toml(dummy_citation_cff_file_path, dummy_pyproject_toml_file_path):
+def test_set_version_for_pyproject_toml_and_citation_cff(dummy_citation_cff_file_path, dummy_pyproject_toml_file_path):
     expected_version: str = '10.1.1'
     with TempCopiedFile(source_file_path=dummy_citation_cff_file_path) as tmp_dummy_citation_cff_file:
         with TempCopiedFile(source_file_path=dummy_pyproject_toml_file_path) as tmp_dummy_pyproject_toml_file:
 
             toml_object: TOMLObject = load_toml_object(
                 toml_file_path=tmp_dummy_pyproject_toml_file.file_path)
             assert toml_object['project']['version'] == '0.0.1'
@@ -256,7 +256,21 @@
             cff_object = load_cff_object(
                 cff_file_path=tmp_dummy_citation_cff_file.file_path)
             assert cff_object['version'] == expected_version
             assert cff_object['title'] == 'somecooltool'
             assert cff_object['license'] == 'Apache-2.0'
             assert cff_object['abstract'] == 'A module that does something cool.'
             assert cff_object['repository-code'] == 'https://github.com/willynilly/somewherecool'
+
+
+def test_get_version_for_citation_cff(dummy_citation_cff_file_path):
+    with TempCopiedFile(source_file_path=dummy_citation_cff_file_path) as tmp_dummy_citation_cff_file:
+        cff_object: CFFObject = load_cff_object(
+            cff_file_path=tmp_dummy_citation_cff_file.file_path)
+        assert cff_object['version'] == '0.0.2'
+
+
+def test_get_version_for_pyproject_toml(dummy_pyproject_toml_file_path):
+    with TempCopiedFile(source_file_path=dummy_pyproject_toml_file_path) as tmp_dummy_pyproject_toml_file:
+        toml_object: TOMLObject = load_toml_object(
+            toml_file_path=tmp_dummy_pyproject_toml_file.file_path)
+        assert toml_object['project']['version'] == '0.0.1'
```

### Comparing `cff2toml-1.1.3/tests/dummy_files/dummy_CITATION.cff` & `cff2toml-1.2.0/tests/dummy_files/dummy_CITATION.cff`

 * *Files identical despite different names*

### Comparing `cff2toml-1.1.3/tests/dummy_files/dummy_pyproject.toml` & `cff2toml-1.2.0/tests/dummy_files/dummy_pyproject.toml`

 * *Files identical despite different names*

### Comparing `cff2toml-1.1.3/LICENSE` & `cff2toml-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cff2toml-1.1.3/README.md` & `cff2toml-1.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -67,15 +67,57 @@
 # have custom file paths
 pyproject_toml_file_path: str = os.path.join('somepath', 'pyproject.toml')
 citation_cff_file_path: str = os.path.join('someotherpath', 'CITATION.cff')
 
 update_citation_cff_with_pyproject_toml(citation_cff_file_path=citation_cff_file_path, pyproject_toml_file_path=pyproject_toml_file_path)
 ```
 
-### Set the same version property for both pyprojects.toml file and CITATION.cff file
+### Get the version for pyprojects.toml file
+
+```python
+from cff2toml import get_version_for_pyproject_toml
+
+# get the version for pyproject.toml
+# where it is located in the working directory
+pyprpject_toml_version: str = get_version_for_pyproject_toml()
+```
+
+```python
+from cff2toml import get_version_for_pyproject_toml
+import os
+
+# get version for pyproject.toml
+# where it has a custom file path
+pyproject_toml_file_path: str = os.path.join('somepath', 'pyproject.toml')
+
+pyproject_toml_version: str = get_version_for_pyproject_toml( pyproject_toml_file_path=pyproject_toml_file_path)
+```
+
+### Get the version for CITATION.cff file
+
+```python
+from cff2toml import get_version_for_citation_cff
+
+# get the version for CITATION.cff
+# where it is located in the working directory
+citation_cff_version: str = get_version_for_citation_cff()
+```
+
+```python
+from cff2toml import get_version_for_citation_cff
+import os
+
+# get version for CITATION.cff
+# where it has a custom file path
+citation_cff_file_path: str = os.path.join('somepath', 'CITATION.cff')
+
+version: str = get_version_for_citation_cff(citation_cff_file_path=citation_cff_file_path)
+```
+
+### Set the same version for both pyprojects.toml file and CITATION.cff file
 
 ```python
 from cff2toml import set_version_for_pyproject_toml_and_citation_cff
 
 # set same version for pyproject.toml
 # and CITATION.cff where both files are
 # located in the working directory
@@ -181,13 +223,12 @@
 ## Limitations
 
 For update_pyproject_toml_with_citation_cff() and update_citation_cff_with_pyproject_toml(), the only metadata that is currently updated between CITATION.cff and pyproject.toml files is: CFF (title, version, abstract, license, repository-code) <-> TOML (project.name, project.version, project.description, project.license, project.urls.Source).
 
 ## Roadmap
 
 1. Update author information for update_pyproject_toml_with_citation_cff() and update_citation_cff_with_pyproject_toml()
-2. Add get_versions_for_pyproject_toml_and_citation_cff() method that returns the current versions of both files as a tuple.
-3. Create CLI
+2. Create CLI
 
 ## License
 
 `cff2toml` is distributed under the terms of the [Apache 2.0](https://spdx.org/licenses/Apache-2.0.html) license
```

### Comparing `cff2toml-1.1.3/pyproject.toml` & `cff2toml-1.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cff2toml"
-version = "1.1.3"
+version = "1.2.0"
 description = "A module to synchronize metadata between TOML and CFF files, including between pyproject.toml and CITATION.cff files."
 readme = "README.md"
 requires-python = ">=3.8"
 license = "Apache-2.0"
 keywords = []
 authors = [
   { name = "Will Riley", email = "wanderingwill@gmail.com" },
```

### Comparing `cff2toml-1.1.3/PKG-INFO` & `cff2toml-1.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: cff2toml
-Version: 1.1.3
+Version: 1.2.0
 Summary: A module to synchronize metadata between TOML and CFF files, including between pyproject.toml and CITATION.cff files.
 Project-URL: Documentation, https://github.com/willynilly/cff2toml#readme
 Project-URL: Issues, https://github.com/willynilly/cff2toml/issues
 Project-URL: Source, https://github.com/willynilly/cff2toml
 Author-email: Will Riley <wanderingwill@gmail.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
@@ -102,15 +102,57 @@
 # have custom file paths
 pyproject_toml_file_path: str = os.path.join('somepath', 'pyproject.toml')
 citation_cff_file_path: str = os.path.join('someotherpath', 'CITATION.cff')
 
 update_citation_cff_with_pyproject_toml(citation_cff_file_path=citation_cff_file_path, pyproject_toml_file_path=pyproject_toml_file_path)
 ```
 
-### Set the same version property for both pyprojects.toml file and CITATION.cff file
+### Get the version for pyprojects.toml file
+
+```python
+from cff2toml import get_version_for_pyproject_toml
+
+# get the version for pyproject.toml
+# where it is located in the working directory
+pyprpject_toml_version: str = get_version_for_pyproject_toml()
+```
+
+```python
+from cff2toml import get_version_for_pyproject_toml
+import os
+
+# get version for pyproject.toml
+# where it has a custom file path
+pyproject_toml_file_path: str = os.path.join('somepath', 'pyproject.toml')
+
+pyproject_toml_version: str = get_version_for_pyproject_toml( pyproject_toml_file_path=pyproject_toml_file_path)
+```
+
+### Get the version for CITATION.cff file
+
+```python
+from cff2toml import get_version_for_citation_cff
+
+# get the version for CITATION.cff
+# where it is located in the working directory
+citation_cff_version: str = get_version_for_citation_cff()
+```
+
+```python
+from cff2toml import get_version_for_citation_cff
+import os
+
+# get version for CITATION.cff
+# where it has a custom file path
+citation_cff_file_path: str = os.path.join('somepath', 'CITATION.cff')
+
+version: str = get_version_for_citation_cff(citation_cff_file_path=citation_cff_file_path)
+```
+
+### Set the same version for both pyprojects.toml file and CITATION.cff file
 
 ```python
 from cff2toml import set_version_for_pyproject_toml_and_citation_cff
 
 # set same version for pyproject.toml
 # and CITATION.cff where both files are
 # located in the working directory
@@ -216,13 +258,12 @@
 ## Limitations
 
 For update_pyproject_toml_with_citation_cff() and update_citation_cff_with_pyproject_toml(), the only metadata that is currently updated between CITATION.cff and pyproject.toml files is: CFF (title, version, abstract, license, repository-code) <-> TOML (project.name, project.version, project.description, project.license, project.urls.Source).
 
 ## Roadmap
 
 1. Update author information for update_pyproject_toml_with_citation_cff() and update_citation_cff_with_pyproject_toml()
-2. Add get_versions_for_pyproject_toml_and_citation_cff() method that returns the current versions of both files as a tuple.
-3. Create CLI
+2. Create CLI
 
 ## License
 
 `cff2toml` is distributed under the terms of the [Apache 2.0](https://spdx.org/licenses/Apache-2.0.html) license
```

