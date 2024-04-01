# Comparing `tmp/cff2toml-1.0.0.tar.gz` & `tmp/cff2toml-1.1.0.tar.gz`

## Comparing `cff2toml-1.0.0.tar` & `cff2toml-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 cff2toml-1.0.0/CITATION.cff
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 cff2toml-1.0.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 cff2toml-1.0.0/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-1.0.0/src/cff2toml/__init__.py
--rw-r--r--   0        0        0     4843 2020-02-02 00:00:00.000000 cff2toml-1.0.0/src/cff2toml/cff2toml.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 cff2toml-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0    11182 2020-02-02 00:00:00.000000 cff2toml-1.0.0/tests/test_cff2toml.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 cff2toml-1.0.0/tests/dummy_files/dummy_CITATION.cff
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 cff2toml-1.0.0/tests/dummy_files/dummy_pyproject.toml
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 cff2toml-1.0.0/.gitignore
--rw-r--r--   0        0        0    10938 2020-02-02 00:00:00.000000 cff2toml-1.0.0/LICENSE
--rw-r--r--   0        0        0     4673 2020-02-02 00:00:00.000000 cff2toml-1.0.0/README.md
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 cff2toml-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     6207 2020-02-02 00:00:00.000000 cff2toml-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 cff2toml-1.1.0/CITATION.cff
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 cff2toml-1.1.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 cff2toml-1.1.0/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-1.1.0/src/cff2toml/__init__.py
+-rw-r--r--   0        0        0     5575 2020-02-02 00:00:00.000000 cff2toml-1.1.0/src/cff2toml/cff2toml.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 cff2toml-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0    14689 2020-02-02 00:00:00.000000 cff2toml-1.1.0/tests/test_cff2toml.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 cff2toml-1.1.0/tests/dummy_files/dummy_CITATION.cff
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 cff2toml-1.1.0/tests/dummy_files/dummy_pyproject.toml
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 cff2toml-1.1.0/.gitignore
+-rw-r--r--   0        0        0    10938 2020-02-02 00:00:00.000000 cff2toml-1.1.0/LICENSE
+-rw-r--r--   0        0        0     5465 2020-02-02 00:00:00.000000 cff2toml-1.1.0/README.md
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 cff2toml-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6999 2020-02-02 00:00:00.000000 cff2toml-1.1.0/PKG-INFO
```

### Comparing `cff2toml-1.0.0/CITATION.cff` & `cff2toml-1.1.0/CITATION.cff`

 * *Files 0% similar despite different names*

```diff
@@ -17,8 +17,8 @@
   and CITATION.cff files.
 keywords:
   - Citation File Format
   - TOML
   - pyproject.toml
   - CITATION.cff
 license: Apache-2.0
-version: "1.0.0"
+version: "1.1.0"
```

### Comparing `cff2toml-1.0.0/.github/workflows/python-publish.yml` & `cff2toml-1.1.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `cff2toml-1.0.0/src/cff2toml/cff2toml.py` & `cff2toml-1.1.0/src/cff2toml/cff2toml.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Callable, Dict, Union
+from typing import Any, Callable, Dict, Tuple, Union
 import toml
 import yaml
 
 DEFAULT_PYPROJECT_TOML_FILENAME: str = 'pyproject.toml'
 DEFAULT_CITATION_CFF_FILENAME: str = 'CITATION.cff'
 DEFAULT_DIR: str = '.'
 
@@ -118,7 +118,23 @@
         citation_cff_object['version'] = pyproject_toml_object['project']['version']
         citation_cff_object['abstract'] = pyproject_toml_object['project']['description']
         citation_cff_object['license'] = pyproject_toml_object['project']['license']
         citation_cff_object['repository-code'] = pyproject_toml_object['project']['urls']['Source']
 
         return citation_cff_object
     return update_cff_with_toml(toml_file_path=pyproject_toml_file_path, cff_file_path=citation_cff_file_path, transform_cff_object_func=transformer)
+
+
+def set_version_for_pyproject_toml_and_citation_cff(version: str, pyproject_toml_file_path: str, citation_cff_file_path: str) -> Tuple[TOMLObject, CFFObject]:
+    pyproject_toml_object: TOMLObject = load_toml_object(
+        toml_file_path=pyproject_toml_file_path)
+    citation_cff_object: CFFObject = load_cff_object(
+        cff_file_path=citation_cff_file_path)
+
+    citation_cff_object['version'] = version
+    pyproject_toml_object['project']['version'] = version
+
+    save_cff_object(citation_cff_object, cff_file_path=citation_cff_file_path)
+    save_toml_object(toml_object=pyproject_toml_object,
+                     toml_file_path=pyproject_toml_file_path)
+
+    return pyproject_toml_object, citation_cff_object
```

### Comparing `cff2toml-1.0.0/tests/test_cff2toml.py` & `cff2toml-1.1.0/tests/test_cff2toml.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
 import os
-from src.cff2toml.cff2toml import load_cff_object, load_toml_object, CFFObject, TOMLObject, TransformCFFObjectWithTOMLObjectFunction, TransformTOMLObjectWithCFFObjectFunction, update_cff_with_toml, update_citation_cff_with_pyproject_toml, update_pyproject_toml_with_citation_cff, update_toml_with_cff
+from src.cff2toml.cff2toml import load_cff_object, load_toml_object, CFFObject, TOMLObject, TransformCFFObjectWithTOMLObjectFunction, TransformTOMLObjectWithCFFObjectFunction, set_version_for_pyproject_toml_and_citation_cff, update_cff_with_toml, update_citation_cff_with_pyproject_toml, update_pyproject_toml_with_citation_cff, update_toml_with_cff
 
 import tempfile
 import shutil
 import os
 
 
 class TempCopiedFile:
@@ -201,7 +201,62 @@
             cff_object = load_cff_object(
                 cff_file_path=tmp_dummy_citation_cff_file.file_path)
             assert cff_object['version'] == '0.0.1'
             assert cff_object['title'] == 'someuncooltool'
             assert cff_object['license'] == 'Apache-1.0'
             assert cff_object['abstract'] == 'A module that does something uncool.'
             assert cff_object['repository-code'] == 'https://github.com/willnilly/somewhereuncool'
+
+
+def test_set_version_for_citation_cff_with_pyproject_toml(dummy_citation_cff_file_path, dummy_pyproject_toml_file_path):
+    expected_version: str = '10.1.1'
+    with TempCopiedFile(source_file_path=dummy_citation_cff_file_path) as tmp_dummy_citation_cff_file:
+        with TempCopiedFile(source_file_path=dummy_pyproject_toml_file_path) as tmp_dummy_pyproject_toml_file:
+
+            toml_object: TOMLObject = load_toml_object(
+                toml_file_path=tmp_dummy_pyproject_toml_file.file_path)
+            assert toml_object['project']['version'] == '0.0.1'
+            assert toml_object['project']['name'] == 'someuncooltool'
+            assert toml_object['project']['description'] == 'A module that does something uncool.'
+            assert toml_object['project']['license'] == 'Apache-1.0'
+            assert toml_object['project']['urls']['Source'] == 'https://github.com/willnilly/somewhereuncool'
+
+            cff_object: CFFObject = load_cff_object(
+                cff_file_path=tmp_dummy_citation_cff_file.file_path)
+            assert cff_object['version'] == '0.0.2'
+            assert cff_object['title'] == 'somecooltool'
+            assert cff_object['license'] == 'Apache-2.0'
+            assert cff_object['abstract'] == 'A module that does something cool.'
+            assert cff_object['repository-code'] == 'https://github.com/willynilly/somewherecool'
+
+            toml_object, cff_object = set_version_for_pyproject_toml_and_citation_cff(
+                version=expected_version,
+                pyproject_toml_file_path=tmp_dummy_pyproject_toml_file.file_path,
+                citation_cff_file_path=tmp_dummy_citation_cff_file.file_path,)
+
+            assert toml_object['project']['version'] == expected_version
+            assert toml_object['project']['name'] == 'someuncooltool'
+            assert toml_object['project']['description'] == 'A module that does something uncool.'
+            assert toml_object['project']['license'] == 'Apache-1.0'
+            assert toml_object['project']['urls']['Source'] == 'https://github.com/willnilly/somewhereuncool'
+
+            assert cff_object['version'] == expected_version
+            assert cff_object['title'] == 'somecooltool'
+            assert cff_object['license'] == 'Apache-2.0'
+            assert cff_object['abstract'] == 'A module that does something cool.'
+            assert cff_object['repository-code'] == 'https://github.com/willynilly/somewherecool'
+
+            toml_object = load_toml_object(
+                toml_file_path=tmp_dummy_pyproject_toml_file.file_path)
+            assert toml_object['project']['version'] == expected_version
+            assert toml_object['project']['name'] == 'someuncooltool'
+            assert toml_object['project']['description'] == 'A module that does something uncool.'
+            assert toml_object['project']['license'] == 'Apache-1.0'
+            assert toml_object['project']['urls']['Source'] == 'https://github.com/willnilly/somewhereuncool'
+
+            cff_object = load_cff_object(
+                cff_file_path=tmp_dummy_citation_cff_file.file_path)
+            assert cff_object['version'] == expected_version
+            assert cff_object['title'] == 'somecooltool'
+            assert cff_object['license'] == 'Apache-2.0'
+            assert cff_object['abstract'] == 'A module that does something cool.'
+            assert cff_object['repository-code'] == 'https://github.com/willynilly/somewherecool'
```

### Comparing `cff2toml-1.0.0/tests/dummy_files/dummy_CITATION.cff` & `cff2toml-1.1.0/tests/dummy_files/dummy_CITATION.cff`

 * *Files identical despite different names*

### Comparing `cff2toml-1.0.0/tests/dummy_files/dummy_pyproject.toml` & `cff2toml-1.1.0/tests/dummy_files/dummy_pyproject.toml`

 * *Files identical despite different names*

### Comparing `cff2toml-1.0.0/LICENSE` & `cff2toml-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cff2toml-1.0.0/README.md` & `cff2toml-1.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -22,55 +22,81 @@
 ## Usage
 
 ### Updating pyproject.toml with metadata from CITATION.cff
 
 ```python
 from cff2toml import update_pyproject_toml_with_citation_cff
 
-# update the pyproject.toml file with metadata
-# from CITATION.cff file
+# update pyproject.toml with metadata
+# from CITATION.cff
 # where both files are located in the working directory
 update_pyproject_toml_with_citation_cff()
 ```
 
 ```python
 from cff2toml import update_pyproject_toml_with_citation_cff
+import os
 
-# update the pyproject.toml file with metadata
-# from CITATION.cff file
-# where both files are located in the working directory
+# update pyproject.toml with metadata
+# from CITATION.cff
+# with custom file paths
 pyproject_toml_file_path: str = os.path.join('somepath', 'pyproject.toml')
-citation_cff_file_path: str = os.path.join('somepath', 'CITATION.cff')
+citation_cff_file_path: str = os.path.join('someotherpath', 'CITATION.cff')
 
 update_pyproject_toml_with_citation_cff(pyproject_toml_file_path=pyproject_toml_file_path, citation_cff_file_path=citation_cff_file_path)
 ```
 
-### Updating CITATION.toml with metadata from pyprojects.toml
+### Updating CITATION.cff with metadata from pyprojects.toml
 
 ```python
 from cff2toml import update_citation_cff_with_pyproject_toml
 
-# update the CITATION.cff file with metadata
-# from pyprojects.cff file
+# update CITATION.cff with metadata
+# from pyprojects.cff
 # where both files are located in the working directory
 update_citation_cff_with_pyproject_toml()
 ```
 
 ```python
 from cff2toml import update_pyproject_toml_with_citation_cff
+import os
 
-# update the CITATION.cff file with metadata
-# from pyprojects.cff file
-# from specific locations
+# update CITATION.cff with metadata
+# from pyprojects.cff
+# with custom file paths
 pyproject_toml_file_path: str = os.path.join('somepath', 'pyproject.toml')
-citation_cff_file_path: str = os.path.join('somepath', 'CITATION.cff')
+citation_cff_file_path: str = os.path.join('someotherpath', 'CITATION.cff')
 
 update_citation_cff_with_pyproject_toml(citation_cff_file_path=citation_cff_file_path, pyproject_toml_file_path=pyproject_toml_file_path)
 ```
 
+### Setting the same version for both the pyprojects.toml file and CITATION.cff file
+
+```python
+from cff2toml import set_version_for_pyproject_toml_and_citation_cff
+
+# set same version for pyproject.toml
+# and CITATION.cff where both files are
+# located in the working directory
+set_version_for_pyproject_toml_and_citation_cff(version="2.0.0")
+```
+
+```python
+from cff2toml import update_pyproject_toml_with_citation_cff
+import os
+
+# set same version for pyproject.toml
+# and CITATION.cff where both files
+# have custom file paths
+pyproject_toml_file_path: str = os.path.join('somepath', 'pyproject.toml')
+citation_cff_file_path: str = os.path.join('someotherpath', 'CITATION.cff')
+
+set_version_for_pyproject_toml_with_citation_cff(version="2.0.0", pyproject_toml_file_path=pyproject_toml_file_path, citation_cff_file_path=citation_cff_file_path)
+```
+
 ### Updating TOML file with metadata from CFF file
 
 ```python
 from cff2toml import update_toml_with_cff, CFFObject, TOMLObject
 import os
 
 toml_file_path: str = os.path.join('somepath', 'some_toml_file.toml')
```

### Comparing `cff2toml-1.0.0/pyproject.toml` & `cff2toml-1.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cff2toml"
-version = "1.0.0"
+version = "1.1.0"
 description = "A module to synchronize metadata between TOML and CFF files, including between pyproject.toml and CITATION.cff files."
 readme = "README.md"
 requires-python = ">=3.8"
 license = "Apache-2.0"
 keywords = []
 authors = [
   { name = "Will Riley", email = "wanderingwill@gmail.com" },
```

### Comparing `cff2toml-1.0.0/PKG-INFO` & `cff2toml-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: cff2toml
-Version: 1.0.0
+Version: 1.1.0
 Summary: A module to synchronize metadata between TOML and CFF files, including between pyproject.toml and CITATION.cff files.
 Project-URL: Documentation, https://github.com/willynilly/cff2toml#readme
 Project-URL: Issues, https://github.com/willynilly/cff2toml/issues
 Project-URL: Source, https://github.com/willynilly/cff2toml
 Author-email: Will Riley <wanderingwill@gmail.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
@@ -57,55 +57,81 @@
 ## Usage
 
 ### Updating pyproject.toml with metadata from CITATION.cff
 
 ```python
 from cff2toml import update_pyproject_toml_with_citation_cff
 
-# update the pyproject.toml file with metadata
-# from CITATION.cff file
+# update pyproject.toml with metadata
+# from CITATION.cff
 # where both files are located in the working directory
 update_pyproject_toml_with_citation_cff()
 ```
 
 ```python
 from cff2toml import update_pyproject_toml_with_citation_cff
+import os
 
-# update the pyproject.toml file with metadata
-# from CITATION.cff file
-# where both files are located in the working directory
+# update pyproject.toml with metadata
+# from CITATION.cff
+# with custom file paths
 pyproject_toml_file_path: str = os.path.join('somepath', 'pyproject.toml')
-citation_cff_file_path: str = os.path.join('somepath', 'CITATION.cff')
+citation_cff_file_path: str = os.path.join('someotherpath', 'CITATION.cff')
 
 update_pyproject_toml_with_citation_cff(pyproject_toml_file_path=pyproject_toml_file_path, citation_cff_file_path=citation_cff_file_path)
 ```
 
-### Updating CITATION.toml with metadata from pyprojects.toml
+### Updating CITATION.cff with metadata from pyprojects.toml
 
 ```python
 from cff2toml import update_citation_cff_with_pyproject_toml
 
-# update the CITATION.cff file with metadata
-# from pyprojects.cff file
+# update CITATION.cff with metadata
+# from pyprojects.cff
 # where both files are located in the working directory
 update_citation_cff_with_pyproject_toml()
 ```
 
 ```python
 from cff2toml import update_pyproject_toml_with_citation_cff
+import os
 
-# update the CITATION.cff file with metadata
-# from pyprojects.cff file
-# from specific locations
+# update CITATION.cff with metadata
+# from pyprojects.cff
+# with custom file paths
 pyproject_toml_file_path: str = os.path.join('somepath', 'pyproject.toml')
-citation_cff_file_path: str = os.path.join('somepath', 'CITATION.cff')
+citation_cff_file_path: str = os.path.join('someotherpath', 'CITATION.cff')
 
 update_citation_cff_with_pyproject_toml(citation_cff_file_path=citation_cff_file_path, pyproject_toml_file_path=pyproject_toml_file_path)
 ```
 
+### Setting the same version for both the pyprojects.toml file and CITATION.cff file
+
+```python
+from cff2toml import set_version_for_pyproject_toml_and_citation_cff
+
+# set same version for pyproject.toml
+# and CITATION.cff where both files are
+# located in the working directory
+set_version_for_pyproject_toml_and_citation_cff(version="2.0.0")
+```
+
+```python
+from cff2toml import update_pyproject_toml_with_citation_cff
+import os
+
+# set same version for pyproject.toml
+# and CITATION.cff where both files
+# have custom file paths
+pyproject_toml_file_path: str = os.path.join('somepath', 'pyproject.toml')
+citation_cff_file_path: str = os.path.join('someotherpath', 'CITATION.cff')
+
+set_version_for_pyproject_toml_with_citation_cff(version="2.0.0", pyproject_toml_file_path=pyproject_toml_file_path, citation_cff_file_path=citation_cff_file_path)
+```
+
 ### Updating TOML file with metadata from CFF file
 
 ```python
 from cff2toml import update_toml_with_cff, CFFObject, TOMLObject
 import os
 
 toml_file_path: str = os.path.join('somepath', 'some_toml_file.toml')
```

