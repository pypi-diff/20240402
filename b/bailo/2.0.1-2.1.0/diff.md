# Comparing `tmp/bailo-2.0.1.tar.gz` & `tmp/bailo-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bailo-2.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "bailo-2.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `bailo-2.0.1.tar` & `bailo-2.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     2241 2024-03-12 16:17:06.581007 bailo-2.0.1/README.md
--rw-r--r--   0        0        0     4788 2024-03-12 16:17:06.581007 bailo-2.0.1/pyproject.toml
--rw-r--r--   0        0        0      611 2024-03-12 16:17:06.581007 bailo-2.0.1/src/bailo/__init__.py
--rw-r--r--   0        0        0      153 2024-03-12 16:17:06.585007 bailo-2.0.1/src/bailo/core/__init__.py
--rw-r--r--   0        0        0     3571 2024-03-12 16:17:06.585007 bailo-2.0.1/src/bailo/core/agent.py
--rw-r--r--   0        0        0    19039 2024-03-12 16:17:06.585007 bailo-2.0.1/src/bailo/core/client.py
--rw-r--r--   0        0        0      564 2024-03-12 16:17:06.585007 bailo-2.0.1/src/bailo/core/enums.py
--rw-r--r--   0        0        0      221 2024-03-12 16:17:06.585007 bailo-2.0.1/src/bailo/core/exceptions.py
--rw-r--r--   0        0        0      335 2024-03-12 16:17:06.585007 bailo-2.0.1/src/bailo/core/utils.py
--rw-r--r--   0        0        0      521 2024-03-12 16:17:06.585007 bailo-2.0.1/src/bailo/helper/__init__.py
--rw-r--r--   0        0        0     3923 2024-03-12 16:17:06.585007 bailo-2.0.1/src/bailo/helper/access_request.py
--rw-r--r--   0        0        0     8381 2024-03-12 16:17:06.585007 bailo-2.0.1/src/bailo/helper/model.py
--rw-r--r--   0        0        0     6103 2024-03-12 16:17:06.585007 bailo-2.0.1/src/bailo/helper/release.py
--rw-r--r--   0        0        0     2976 2024-03-12 16:17:06.585007 bailo-2.0.1/src/bailo/helper/schema.py
--rw-r--r--   0        0        0     3599 1970-01-01 00:00:00.000000 bailo-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2241 2024-04-02 10:54:52.927553 bailo-2.1.0/README.md
+-rw-r--r--   0        0        0     4869 2024-04-02 10:54:52.927553 bailo-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0      631 2024-04-02 10:54:52.927553 bailo-2.1.0/src/bailo/__init__.py
+-rw-r--r--   0        0        0      153 2024-04-02 10:54:52.927553 bailo-2.1.0/src/bailo/core/__init__.py
+-rw-r--r--   0        0        0     3571 2024-04-02 10:54:52.927553 bailo-2.1.0/src/bailo/core/agent.py
+-rw-r--r--   0        0        0    19039 2024-04-02 10:54:52.927553 bailo-2.1.0/src/bailo/core/client.py
+-rw-r--r--   0        0        0      564 2024-04-02 10:54:52.927553 bailo-2.1.0/src/bailo/core/enums.py
+-rw-r--r--   0        0        0      221 2024-04-02 10:54:52.927553 bailo-2.1.0/src/bailo/core/exceptions.py
+-rw-r--r--   0        0        0     1057 2024-04-02 10:54:52.927553 bailo-2.1.0/src/bailo/core/utils.py
+-rw-r--r--   0        0        0      521 2024-04-02 10:54:52.927553 bailo-2.1.0/src/bailo/helper/__init__.py
+-rw-r--r--   0        0        0     3923 2024-04-02 10:54:52.927553 bailo-2.1.0/src/bailo/helper/access_request.py
+-rw-r--r--   0        0        0    15195 2024-04-02 10:54:52.927553 bailo-2.1.0/src/bailo/helper/model.py
+-rw-r--r--   0        0        0     7043 2024-04-02 10:54:52.927553 bailo-2.1.0/src/bailo/helper/release.py
+-rw-r--r--   0        0        0     2976 2024-04-02 10:54:52.927553 bailo-2.1.0/src/bailo/helper/schema.py
+-rw-r--r--   0        0        0     3646 1970-01-01 00:00:00.000000 bailo-2.1.0/PKG-INFO
```

### Comparing `bailo-2.0.1/README.md` & `bailo-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `bailo-2.0.1/pyproject.toml` & `bailo-2.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     "requests>=2.22"
 ]
 
 [project.optional-dependencies]
 test = [
     "black==23.3.0",
     "check-manifest==0.49",
+    "mlflow>2.11.0",
     "pre-commit==3.3.1",
     "pylint==2.17.4",
     "pylint_junit",
     "pytest-cov==4.0.0",
     "pytest-mock<3.10.1",
     "pytest-runner",
     "pytest==7.3.1",
@@ -71,22 +72,23 @@
 pythonPlatform = "Linux"
 
 executionEnvironments = [
   { root = "src" }
 ]
 
 [tool.pytest.ini_options]
-addopts = "--cov-report xml:coverage.xml --cov src --cov-fail-under 0 --cov-append -m 'not integration'"
+addopts = "--cov-report xml:coverage.xml --cov src --cov-fail-under 0 --cov-append -m 'not (integration or mlflow)'"
 pythonpath = [
   "src"
 ]
 testpaths = "tests"
 junit_family = "xunit2"
 markers = [
     "integration: marks as integration test",
+    "mlflow: marks as mlflow integration test",
 ]
 
 [tool.pylint]
 extension-pkg-whitelist= [
     "numpy",
     "torch",
     "cv2",
```

### Comparing `bailo-2.0.1/src/bailo/__init__.py` & `bailo-2.1.0/src/bailo/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Bailo Python Client
 ===================
 
 Bailo is a ecosystem for managing the lifecycle of managing machine learning models. This package provides support for interacting with models within Bailo.
 """
 from __future__ import annotations
 
-# Package Version
-__version__ = "2.0.1"
+# Package Version (2.1.0)
+__version__ = "2.1.0"
 
 from bailo.core.agent import Agent, PkiAgent, TokenAgent
 from bailo.core.client import Client
 from bailo.core.enums import ModelVisibility, Role, SchemaKind
 from bailo.helper.access_request import AccessRequest
-from bailo.helper.model import Model
+from bailo.helper.model import Model, Experiment
 from bailo.helper.release import Release
 from bailo.helper.schema import Schema
```

### Comparing `bailo-2.0.1/src/bailo/core/agent.py` & `bailo-2.1.0/src/bailo/core/agent.py`

 * *Files identical despite different names*

### Comparing `bailo-2.0.1/src/bailo/core/client.py` & `bailo-2.1.0/src/bailo/core/client.py`

 * *Files identical despite different names*

### Comparing `bailo-2.0.1/src/bailo/core/enums.py` & `bailo-2.1.0/src/bailo/core/enums.py`

 * *Files identical despite different names*

### Comparing `bailo-2.0.1/src/bailo/helper/__init__.py` & `bailo-2.1.0/src/bailo/helper/__init__.py`

 * *Files identical despite different names*

### Comparing `bailo-2.0.1/src/bailo/helper/access_request.py` & `bailo-2.1.0/src/bailo/helper/access_request.py`

 * *Files identical despite different names*

### Comparing `bailo-2.0.1/src/bailo/helper/release.py` & `bailo-2.1.0/src/bailo/helper/release.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from __future__ import annotations
 
+import os
+import shutil
 from io import BytesIO
 from typing import Any
 
 from bailo.core.client import Client
 from semantic_version import Version
 
 
@@ -128,31 +130,58 @@
             notes,
             files,
             images,
             minor,
             draft,
         )
 
-    def download(self, filename: str) -> Any:
+    def download(self, filename: str, write: bool = True, path: str | None = None) -> Any:
         """Give returns a Reading object given the file id.
 
         :param filename: The name of the file to retrieve
+        :param write: Bool to determine if writing file to disk, defaults to True
+        :param path: Local path to write file to (if write set to True)
+
         :return: A JSON response object
         """
-        return self.client.get_download_by_filename(self.model_id, str(self.version), filename)
+        res = self.client.get_download_by_filename(self.model_id, str(self.version), filename)
+
+        if write:
+            if path is None:
+                path = filename
+            with open(path, "wb") as f:
+                f.write(res.content)
+
+        return res
 
-    def upload(self, name: str, file: BytesIO) -> str:
-        """Upload files in a given directory to the release.
+    def upload(self, path: str, data: BytesIO | None = None) -> str:
+        """Upload a file to the release.
 
-        :param name: The name of the file to upload to bailo
-        :param f: A BytesIO object
+        :param path: The path, or name of file or directory to be uploaded
+        :param data: A BytesIO object if not loading from disk
 
         :return: The unique file ID of the file uploaded
+        ..note:: If path provided is a directory, it will be uploaded as a zip
         """
-        res = self.client.simple_upload(self.model_id, name, file).json()
+        name = os.path.split(path)[1]
+
+        if data is None:
+            if is_zip := os.path.isdir(path):
+                shutil.make_archive(name, "zip", path)
+                path = f"{name}.zip"
+                name = path
+
+            with open(path, "rb") as f:
+                res = self.client.simple_upload(self.model_id, name, f).json()
+
+            if is_zip:
+                os.remove(path)
+        else:
+            res = self.client.simple_upload(self.model_id, name, data).json()
+
         self.files.append(res["file"]["id"])
         self.update()
         return res["file"]["id"]
 
     def update(self) -> Any:
         """Update the any changes to this release on Bailo.
```

### Comparing `bailo-2.0.1/src/bailo/helper/schema.py` & `bailo-2.1.0/src/bailo/helper/schema.py`

 * *Files identical despite different names*

### Comparing `bailo-2.0.1/PKG-INFO` & `bailo-2.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: bailo
-Version: 2.0.1
+Version: 2.1.0
 Summary: Simplifies interacting with Bailo
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: semantic-version==2.10.0
 Requires-Dist: requests>=2.22
 Requires-Dist: black==23.3.0 ; extra == "test"
 Requires-Dist: check-manifest==0.49 ; extra == "test"
+Requires-Dist: mlflow>2.11.0 ; extra == "test"
 Requires-Dist: pre-commit==3.3.1 ; extra == "test"
 Requires-Dist: pylint==2.17.4 ; extra == "test"
 Requires-Dist: pylint_junit ; extra == "test"
 Requires-Dist: pytest-cov==4.0.0 ; extra == "test"
 Requires-Dist: pytest-mock<3.10.1 ; extra == "test"
 Requires-Dist: pytest-runner ; extra == "test"
 Requires-Dist: pytest==7.3.1 ; extra == "test"
```

#### html2text {}

```diff
@@ -1,26 +1,27 @@
-Metadata-Version: 2.1 Name: bailo Version: 2.0.1 Summary: Simplifies
+Metadata-Version: 2.1 Name: bailo Version: 2.1.0 Summary: Simplifies
 interacting with Bailo Requires-Python: >=3.8.1 Description-Content-Type: text/
 markdown Classifier: Development Status :: 3 - Alpha Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: semantic-version==2.10.0 Requires-Dist: requests>=2.22 Requires-
 Dist: black==23.3.0 ; extra == "test" Requires-Dist: check-manifest==0.49 ;
-extra == "test" Requires-Dist: pre-commit==3.3.1 ; extra == "test" Requires-
-Dist: pylint==2.17.4 ; extra == "test" Requires-Dist: pylint_junit ; extra ==
-"test" Requires-Dist: pytest-cov==4.0.0 ; extra == "test" Requires-Dist:
-pytest-mock<3.10.1 ; extra == "test" Requires-Dist: pytest-runner ; extra ==
-"test" Requires-Dist: pytest==7.3.1 ; extra == "test" Requires-Dist: pytest-
-github-actions-annotate-failures ; extra == "test" Requires-Dist:
-requests_mock==1.11.0 ; extra == "test" Requires-Dist: shellcheck-py==0.9.0.2 ;
-extra == "test" Project-URL: Documentation, https://github.com/gchq/bailo/tree/
-main#readme Project-URL: Source, https://github.com/gchq/bailo Project-URL:
-Tracker, https://github.com/gchq/bailo/issues Provides-Extra: test # Bailo
-Python Client A simple Python API Wrapper for Bailo
+extra == "test" Requires-Dist: mlflow>2.11.0 ; extra == "test" Requires-Dist:
+pre-commit==3.3.1 ; extra == "test" Requires-Dist: pylint==2.17.4 ; extra ==
+"test" Requires-Dist: pylint_junit ; extra == "test" Requires-Dist: pytest-
+cov==4.0.0 ; extra == "test" Requires-Dist: pytest-mock<3.10.1 ; extra ==
+"test" Requires-Dist: pytest-runner ; extra == "test" Requires-Dist:
+pytest==7.3.1 ; extra == "test" Requires-Dist: pytest-github-actions-annotate-
+failures ; extra == "test" Requires-Dist: requests_mock==1.11.0 ; extra ==
+"test" Requires-Dist: shellcheck-py==0.9.0.2 ; extra == "test" Project-URL:
+Documentation, https://github.com/gchq/bailo/tree/main#readme Project-URL:
+Source, https://github.com/gchq/bailo Project-URL: Tracker, https://github.com/
+gchq/bailo/issues Provides-Extra: test # Bailo Python Client A simple Python
+API Wrapper for Bailo
 Table of Contents
    1. _K_e_y_ _F_e_a_t_u_r_e_s
    2. _I_n_s_t_a_l_l_i_n_g
    3. _G_e_t_t_i_n_g_ _S_t_a_r_t_e_d
    4. _D_e_v_e_l_o_p_m_e_n_t
           o _P_r_e_c_o_m_m_i_t_s
           o _T_e_s_t_i_n_g
```

