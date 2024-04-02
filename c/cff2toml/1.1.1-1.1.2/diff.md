# Comparing `tmp/cff2toml-1.1.1.tar.gz` & `tmp/cff2toml-1.1.2.tar.gz`

## Comparing `cff2toml-1.1.1.tar` & `cff2toml-1.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 cff2toml-1.1.1/CITATION.cff
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 cff2toml-1.1.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 cff2toml-1.1.1/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-1.1.1/src/cff2toml/__init__.py
--rw-r--r--   0        0        0     5575 2020-02-02 00:00:00.000000 cff2toml-1.1.1/src/cff2toml/cff2toml.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 cff2toml-1.1.1/tests/__init__.py
--rw-r--r--   0        0        0    14689 2020-02-02 00:00:00.000000 cff2toml-1.1.1/tests/test_cff2toml.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 cff2toml-1.1.1/tests/dummy_files/dummy_CITATION.cff
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 cff2toml-1.1.1/tests/dummy_files/dummy_pyproject.toml
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 cff2toml-1.1.1/.gitignore
--rw-r--r--   0        0        0    10938 2020-02-02 00:00:00.000000 cff2toml-1.1.1/LICENSE
--rw-r--r--   0        0        0     5508 2020-02-02 00:00:00.000000 cff2toml-1.1.1/README.md
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 cff2toml-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     7042 2020-02-02 00:00:00.000000 cff2toml-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 cff2toml-1.1.2/CITATION.cff
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 cff2toml-1.1.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 cff2toml-1.1.2/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cff2toml-1.1.2/src/cff2toml/__init__.py
+-rw-r--r--   0        0        0     5575 2020-02-02 00:00:00.000000 cff2toml-1.1.2/src/cff2toml/cff2toml.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 cff2toml-1.1.2/tests/__init__.py
+-rw-r--r--   0        0        0    14689 2020-02-02 00:00:00.000000 cff2toml-1.1.2/tests/test_cff2toml.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 cff2toml-1.1.2/tests/dummy_files/dummy_CITATION.cff
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 cff2toml-1.1.2/tests/dummy_files/dummy_pyproject.toml
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 cff2toml-1.1.2/.gitignore
+-rw-r--r--   0        0        0    10938 2020-02-02 00:00:00.000000 cff2toml-1.1.2/LICENSE
+-rw-r--r--   0        0        0     6235 2020-02-02 00:00:00.000000 cff2toml-1.1.2/README.md
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 cff2toml-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     7769 2020-02-02 00:00:00.000000 cff2toml-1.1.2/PKG-INFO
```

### Comparing `cff2toml-1.1.1/CITATION.cff` & `cff2toml-1.1.2/CITATION.cff`

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
-version: "1.1.1"
+version: "1.1.2"
```

### Comparing `cff2toml-1.1.1/.github/workflows/python-publish.yml` & `cff2toml-1.1.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `cff2toml-1.1.1/src/cff2toml/cff2toml.py` & `cff2toml-1.1.2/src/cff2toml/cff2toml.py`

 * *Files identical despite different names*

### Comparing `cff2toml-1.1.1/tests/test_cff2toml.py` & `cff2toml-1.1.2/tests/test_cff2toml.py`

 * *Files identical despite different names*

### Comparing `cff2toml-1.1.1/tests/dummy_files/dummy_CITATION.cff` & `cff2toml-1.1.2/tests/dummy_files/dummy_CITATION.cff`

 * *Files identical despite different names*

### Comparing `cff2toml-1.1.1/tests/dummy_files/dummy_pyproject.toml` & `cff2toml-1.1.2/tests/dummy_files/dummy_pyproject.toml`

 * *Files identical despite different names*

### Comparing `cff2toml-1.1.1/LICENSE` & `cff2toml-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cff2toml-1.1.1/README.md` & `cff2toml-1.1.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -7,25 +7,27 @@
 
 ---
 
 **Table of Contents**
 
 - [Installation](#installation)
 - [Usage](#usage)
+- [Limitations](#limitations)
+- [Roadmap](#roadmap)
 - [License](#license)
 
 ## Installation
 
 ```console
 pip install cff2toml
 ```
 
 ## Usage
 
-### Updating pyproject.toml with metadata from CITATION.cff
+### Update pyproject.toml with metadata from CITATION.cff
 
 ```python
 from cff2toml import update_pyproject_toml_with_citation_cff
 
 # update pyproject.toml with metadata
 # from CITATION.cff
 # where both files are located in the working directory
@@ -33,23 +35,23 @@
 ```
 
 ```python
 from cff2toml import update_pyproject_toml_with_citation_cff
 import os
 
 # update pyproject.toml with metadata
-# from CITATION.cff
-# with custom file paths
+# from CITATION.cff where the files
+# have custom file paths
 pyproject_toml_file_path: str = os.path.join('somepath', 'pyproject.toml')
 citation_cff_file_path: str = os.path.join('someotherpath', 'CITATION.cff')
 
 update_pyproject_toml_with_citation_cff(pyproject_toml_file_path=pyproject_toml_file_path, citation_cff_file_path=citation_cff_file_path)
 ```
 
-### Updating CITATION.cff with metadata from pyprojects.toml
+### Update CITATION.cff with metadata from pyprojects.toml
 
 ```python
 from cff2toml import update_citation_cff_with_pyproject_toml
 
 # update CITATION.cff with metadata
 # from pyprojects.cff
 # where both files are located in the working directory
@@ -57,23 +59,23 @@
 ```
 
 ```python
 from cff2toml import update_citation_cff_with_pyproject_toml
 import os
 
 # update CITATION.cff with metadata
-# from pyprojects.cff
-# with custom file paths
+# from pyprojects.cff where the files
+# have custom file paths
 pyproject_toml_file_path: str = os.path.join('somepath', 'pyproject.toml')
 citation_cff_file_path: str = os.path.join('someotherpath', 'CITATION.cff')
 
 update_citation_cff_with_pyproject_toml(citation_cff_file_path=citation_cff_file_path, pyproject_toml_file_path=pyproject_toml_file_path)
 ```
 
-### Setting the same version for both the pyprojects.toml file and CITATION.cff file
+### Set the same version property for both pyprojects.toml file and CITATION.cff file
 
 ```python
 from cff2toml import set_version_for_pyproject_toml_and_citation_cff
 
 # set same version for pyproject.toml
 # and CITATION.cff where both files are
 # located in the working directory
@@ -81,23 +83,23 @@
 ```
 
 ```python
 from cff2toml import set_version_for_pyproject_toml_and_citation_cff
 import os
 
 # set same version for pyproject.toml
-# and CITATION.cff where both files
+# and CITATION.cff where the files
 # have custom file paths
 pyproject_toml_file_path: str = os.path.join('somepath', 'pyproject.toml')
 citation_cff_file_path: str = os.path.join('someotherpath', 'CITATION.cff')
 
 set_version_for_pyproject_toml_with_citation_cff(version="2.0.0", pyproject_toml_file_path=pyproject_toml_file_path, citation_cff_file_path=citation_cff_file_path)
 ```
 
-### Updating TOML file with metadata from CFF file
+### Update a TOML file with metadata from a CFF file
 
 ```python
 from cff2toml import update_toml_with_cff, CFFObject, TOMLObject
 import os
 
 toml_file_path: str = os.path.join('somepath', 'some_toml_file.toml')
 cff_file_path: str = os.path.join('somepath', 'some_cff_file.cff')
@@ -105,15 +107,15 @@
 def transformer(toml_object:TOMLObject, cff_object:CFFObject) -> TOMLObject:
     toml_object['somekey'] = cff_object['someotherkey']
     return toml_object
 
 updated_toml_object: TOMLObject = update_toml_with_cff(toml_file_path=toml_file_path, cff_file_path=cff_file_path,  transform_toml_object_func=transformer)
 ```
 
-### Updating CFF file with metadata from TOML file
+### Update a CFF file with metadata from a TOML file
 
 ```python
 from cff2toml import update_cff_with_toml, CFFObject, TOMLObject
 import os
 
 toml_file_path: str = os.path.join('somepath', 'some_toml_file.toml')
 cff_file_path: str = os.path.join('somepath', 'some_cff_file.cff')
@@ -121,61 +123,71 @@
 def transformer(cff_object:CFFObject, toml_object:TOMLObject) -> CFFObject:
     cff_object['somekey'] = toml_object['someotherkey']
     return cff_object
 
 updated_cff_object: CFFObject = update_cff_with_toml(cff_file_path=cff_file_path, toml_file_path=toml_file_path, transform_cff_object_func=transformer)
 ```
 
-### Load TOML file object
+### Load a TOML file object
 
 ```python
 from cff2toml import load_toml_object, TOMLObject
 import os
 
 toml_file_path: str = os.path.join('somepath', 'some_toml_file.toml')
 toml_object: TOMLObject = load_toml_object(toml_file_path=toml_file_path)
 print(toml_object['somekey'])
 ```
 
-### Save TOML file object
+### Save a TOML file object
 
 ```python
 from cff2toml import load_toml_object, save_toml_object, TOMLObject
 import os
 
 toml_file_path: str = os.path.join('somepath', 'some_toml_file.toml')
 toml_object: TOMLObject = load_toml_object(toml_file_path=toml_file_path)
 print(toml_object['somekey'])
 
 toml_object['somekey'] = 'somevalue'
 save_toml_object(toml_object=toml_object, toml_file_path=toml_file_path)
 
 ```
 
-### Load CFF file object
+### Load a CFF file object
 
 ```python
 from cff2toml import load_cff_object, CFFObject
 import os
 
 cff_file_path: str = os.path.join('somepath', 'some_cff_file.cff')
 cff_object: CFFObject = load_cff_object(cff_file_path=cff_file_path)
 print(cff_object['somekey'])
 ```
 
-### Save CFF file object
+### Save a CFF file object
 
 ```python
 from cff2toml import load_cff_object, save_cff_object, CFFObject
 import os
 
 cff_file_path: str = os.path.join('somepath', 'some_cff_file.cff')
 cff_object: CFFObject = load_cff_object(cff_file_path)
 print(cff_object['somekey'])
 
 cff_object['somekey'] = 'somevalue'
 save_cff_object(cff_object=cff_object, cff_file_path=cff_file_path)
 ```
 
+## Limitations
+
+For update_pyproject_toml_with_citation_cff() and update_citation_cff_with_pyproject_toml(), the only metadata that is currently updated between CITATION.cff and pyproject.toml files is: CFF (title, version, abstract, license, repository-code) <-> TOML (project.name, project.version, project.description, project.license, project.urls.Source).
+
+## Roadmap
+
+1. Update author information for update_pyproject_toml_with_citation_cff() and update_citation_cff_with_pyproject_toml()
+2. Add get_versions_for_pyproject_toml_and_citation_cff() method that returns the current versions of both files as a tuple.
+3. Create CLI
+
 ## License
 
 `cff2toml` is distributed under the terms of the [Apache 2.0](https://spdx.org/licenses/Apache-2.0.html) license
```

### Comparing `cff2toml-1.1.1/pyproject.toml` & `cff2toml-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cff2toml"
-version = "1.1.1"
+version = "1.1.2"
 description = "A module to synchronize metadata between TOML and CFF files, including between pyproject.toml and CITATION.cff files."
 readme = "README.md"
 requires-python = ">=3.8"
 license = "Apache-2.0"
 keywords = []
 authors = [
   { name = "Will Riley", email = "wanderingwill@gmail.com" },
```

### Comparing `cff2toml-1.1.1/PKG-INFO` & `cff2toml-1.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: cff2toml
-Version: 1.1.1
+Version: 1.1.2
 Summary: A module to synchronize metadata between TOML and CFF files, including between pyproject.toml and CITATION.cff files.
 Project-URL: Documentation, https://github.com/willynilly/cff2toml#readme
 Project-URL: Issues, https://github.com/willynilly/cff2toml/issues
 Project-URL: Source, https://github.com/willynilly/cff2toml
 Author-email: Will Riley <wanderingwill@gmail.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
@@ -42,25 +42,27 @@
 
 ---
 
 **Table of Contents**
 
 - [Installation](#installation)
 - [Usage](#usage)
+- [Limitations](#limitations)
+- [Roadmap](#roadmap)
 - [License](#license)
 
 ## Installation
 
 ```console
 pip install cff2toml
 ```
 
 ## Usage
 
-### Updating pyproject.toml with metadata from CITATION.cff
+### Update pyproject.toml with metadata from CITATION.cff
 
 ```python
 from cff2toml import update_pyproject_toml_with_citation_cff
 
 # update pyproject.toml with metadata
 # from CITATION.cff
 # where both files are located in the working directory
@@ -68,23 +70,23 @@
 ```
 
 ```python
 from cff2toml import update_pyproject_toml_with_citation_cff
 import os
 
 # update pyproject.toml with metadata
-# from CITATION.cff
-# with custom file paths
+# from CITATION.cff where the files
+# have custom file paths
 pyproject_toml_file_path: str = os.path.join('somepath', 'pyproject.toml')
 citation_cff_file_path: str = os.path.join('someotherpath', 'CITATION.cff')
 
 update_pyproject_toml_with_citation_cff(pyproject_toml_file_path=pyproject_toml_file_path, citation_cff_file_path=citation_cff_file_path)
 ```
 
-### Updating CITATION.cff with metadata from pyprojects.toml
+### Update CITATION.cff with metadata from pyprojects.toml
 
 ```python
 from cff2toml import update_citation_cff_with_pyproject_toml
 
 # update CITATION.cff with metadata
 # from pyprojects.cff
 # where both files are located in the working directory
@@ -92,23 +94,23 @@
 ```
 
 ```python
 from cff2toml import update_citation_cff_with_pyproject_toml
 import os
 
 # update CITATION.cff with metadata
-# from pyprojects.cff
-# with custom file paths
+# from pyprojects.cff where the files
+# have custom file paths
 pyproject_toml_file_path: str = os.path.join('somepath', 'pyproject.toml')
 citation_cff_file_path: str = os.path.join('someotherpath', 'CITATION.cff')
 
 update_citation_cff_with_pyproject_toml(citation_cff_file_path=citation_cff_file_path, pyproject_toml_file_path=pyproject_toml_file_path)
 ```
 
-### Setting the same version for both the pyprojects.toml file and CITATION.cff file
+### Set the same version property for both pyprojects.toml file and CITATION.cff file
 
 ```python
 from cff2toml import set_version_for_pyproject_toml_and_citation_cff
 
 # set same version for pyproject.toml
 # and CITATION.cff where both files are
 # located in the working directory
@@ -116,23 +118,23 @@
 ```
 
 ```python
 from cff2toml import set_version_for_pyproject_toml_and_citation_cff
 import os
 
 # set same version for pyproject.toml
-# and CITATION.cff where both files
+# and CITATION.cff where the files
 # have custom file paths
 pyproject_toml_file_path: str = os.path.join('somepath', 'pyproject.toml')
 citation_cff_file_path: str = os.path.join('someotherpath', 'CITATION.cff')
 
 set_version_for_pyproject_toml_with_citation_cff(version="2.0.0", pyproject_toml_file_path=pyproject_toml_file_path, citation_cff_file_path=citation_cff_file_path)
 ```
 
-### Updating TOML file with metadata from CFF file
+### Update a TOML file with metadata from a CFF file
 
 ```python
 from cff2toml import update_toml_with_cff, CFFObject, TOMLObject
 import os
 
 toml_file_path: str = os.path.join('somepath', 'some_toml_file.toml')
 cff_file_path: str = os.path.join('somepath', 'some_cff_file.cff')
@@ -140,15 +142,15 @@
 def transformer(toml_object:TOMLObject, cff_object:CFFObject) -> TOMLObject:
     toml_object['somekey'] = cff_object['someotherkey']
     return toml_object
 
 updated_toml_object: TOMLObject = update_toml_with_cff(toml_file_path=toml_file_path, cff_file_path=cff_file_path,  transform_toml_object_func=transformer)
 ```
 
-### Updating CFF file with metadata from TOML file
+### Update a CFF file with metadata from a TOML file
 
 ```python
 from cff2toml import update_cff_with_toml, CFFObject, TOMLObject
 import os
 
 toml_file_path: str = os.path.join('somepath', 'some_toml_file.toml')
 cff_file_path: str = os.path.join('somepath', 'some_cff_file.cff')
@@ -156,61 +158,71 @@
 def transformer(cff_object:CFFObject, toml_object:TOMLObject) -> CFFObject:
     cff_object['somekey'] = toml_object['someotherkey']
     return cff_object
 
 updated_cff_object: CFFObject = update_cff_with_toml(cff_file_path=cff_file_path, toml_file_path=toml_file_path, transform_cff_object_func=transformer)
 ```
 
-### Load TOML file object
+### Load a TOML file object
 
 ```python
 from cff2toml import load_toml_object, TOMLObject
 import os
 
 toml_file_path: str = os.path.join('somepath', 'some_toml_file.toml')
 toml_object: TOMLObject = load_toml_object(toml_file_path=toml_file_path)
 print(toml_object['somekey'])
 ```
 
-### Save TOML file object
+### Save a TOML file object
 
 ```python
 from cff2toml import load_toml_object, save_toml_object, TOMLObject
 import os
 
 toml_file_path: str = os.path.join('somepath', 'some_toml_file.toml')
 toml_object: TOMLObject = load_toml_object(toml_file_path=toml_file_path)
 print(toml_object['somekey'])
 
 toml_object['somekey'] = 'somevalue'
 save_toml_object(toml_object=toml_object, toml_file_path=toml_file_path)
 
 ```
 
-### Load CFF file object
+### Load a CFF file object
 
 ```python
 from cff2toml import load_cff_object, CFFObject
 import os
 
 cff_file_path: str = os.path.join('somepath', 'some_cff_file.cff')
 cff_object: CFFObject = load_cff_object(cff_file_path=cff_file_path)
 print(cff_object['somekey'])
 ```
 
-### Save CFF file object
+### Save a CFF file object
 
 ```python
 from cff2toml import load_cff_object, save_cff_object, CFFObject
 import os
 
 cff_file_path: str = os.path.join('somepath', 'some_cff_file.cff')
 cff_object: CFFObject = load_cff_object(cff_file_path)
 print(cff_object['somekey'])
 
 cff_object['somekey'] = 'somevalue'
 save_cff_object(cff_object=cff_object, cff_file_path=cff_file_path)
 ```
 
+## Limitations
+
+For update_pyproject_toml_with_citation_cff() and update_citation_cff_with_pyproject_toml(), the only metadata that is currently updated between CITATION.cff and pyproject.toml files is: CFF (title, version, abstract, license, repository-code) <-> TOML (project.name, project.version, project.description, project.license, project.urls.Source).
+
+## Roadmap
+
+1. Update author information for update_pyproject_toml_with_citation_cff() and update_citation_cff_with_pyproject_toml()
+2. Add get_versions_for_pyproject_toml_and_citation_cff() method that returns the current versions of both files as a tuple.
+3. Create CLI
+
 ## License
 
 `cff2toml` is distributed under the terms of the [Apache 2.0](https://spdx.org/licenses/Apache-2.0.html) license
```

