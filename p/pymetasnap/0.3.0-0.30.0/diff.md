# Comparing `tmp/pymetasnap-0.3.0.tar.gz` & `tmp/pymetasnap-0.30.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymetasnap-0.3.0.tar", max compression
+gzip compressed data, was "pymetasnap-0.30.0.tar", max compression
```

## Comparing `pymetasnap-0.3.0.tar` & `pymetasnap-0.30.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1073 2023-10-19 21:23:56.579472 pymetasnap-0.3.0/LICENSE
--rw-r--r--   0        0        0     2927 2023-10-19 21:23:56.579472 pymetasnap-0.3.0/README.md
--rw-r--r--   0        0        0        0 2023-10-19 21:23:56.579472 pymetasnap-0.3.0/extractor/__init__.py
--rw-r--r--   0        0        0     3629 2023-10-19 21:23:56.579472 pymetasnap-0.3.0/extractor/checks.py
--rw-r--r--   0        0        0     3527 2023-10-19 21:23:56.579472 pymetasnap-0.3.0/extractor/core.py
--rw-r--r--   0        0        0      227 2023-10-19 21:23:56.579472 pymetasnap-0.3.0/extractor/logger.py
--rw-r--r--   0        0        0     1345 2023-10-19 21:23:56.579472 pymetasnap-0.3.0/extractor/main.py
--rw-r--r--   0        0        0     3262 2023-10-19 21:23:56.579472 pymetasnap-0.3.0/extractor/render.py
--rw-r--r--   0        0        0      877 2023-10-19 21:23:56.579472 pymetasnap-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3848 1970-01-01 00:00:00.000000 pymetasnap-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-02 00:30:02.295126 pymetasnap-0.30.0/LICENSE
+-rw-r--r--   0        0        0     3043 2024-04-02 00:30:02.295126 pymetasnap-0.30.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-02 00:30:02.295126 pymetasnap-0.30.0/extractor/__init__.py
+-rw-r--r--   0        0        0     3678 2024-04-02 00:30:02.295126 pymetasnap-0.30.0/extractor/checks.py
+-rw-r--r--   0        0        0     7141 2024-04-02 00:30:02.295126 pymetasnap-0.30.0/extractor/core.py
+-rw-r--r--   0        0        0      227 2024-04-02 00:30:02.295126 pymetasnap-0.30.0/extractor/logger.py
+-rw-r--r--   0        0        0     1345 2024-04-02 00:30:02.295126 pymetasnap-0.30.0/extractor/main.py
+-rw-r--r--   0        0        0     3262 2024-04-02 00:30:02.295126 pymetasnap-0.30.0/extractor/render.py
+-rw-r--r--   0        0        0      908 2024-04-02 00:30:02.295126 pymetasnap-0.30.0/pyproject.toml
+-rw-r--r--   0        0        0     4050 1970-01-01 00:00:00.000000 pymetasnap-0.30.0/PKG-INFO
```

### Comparing `pymetasnap-0.3.0/LICENSE` & `pymetasnap-0.30.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymetasnap-0.3.0/README.md` & `pymetasnap-0.30.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-# pymetasnap
+# pymetasnap [![PyPI version](https://badge.fury.io/py/pymetasnap.svg)](https://badge.fury.io/py/pymetasnap)
 
 pymetasnap is a command-line tool that enables you to extract metadata from the Python Package Index (PyPI). It allows you to retrieve essential information about Python packages hosted on PyPI, including package names, versions, licenses, project URLs, and more.
 
 By leveraging the PyPI API, pymetasnap automates the process of gathering package metadata, making it convenient for developers, researchers, and anyone interested in exploring package information in a structured manner.
 
 ## Features
 
-Retrieve metadata for Python packages from PyPI.
-Extract package names, versions, licenses, and other relevant information.
-Fetch project URLs and version-specific URLs for detailed package exploration.
-Store the extracted metadata in CSV or Excel format for further analysis.
+- Retrieve metadata for Python packages from PyPI.
+- Extract package names, versions, licenses, and other relevant information.
+- Fetch project URLs and version-specific URLs for detailed package exploration.
+- Store the extracted metadata in CSV or Excel format for further analysis.
 
 ## Installation
 
 You can install pymetasnap using pip:
 
 ```bash
 pip install pymetasnap
@@ -49,16 +49,16 @@
 
 Contributions to pymetasnap are welcome! If you encounter any issues or have suggestions for improvements, please open an issue on the project's GitHub repository.
 
 When contributing, please ensure that you follow the existing coding style, write tests for new features, and make sure the tests pass before submitting a pull request.
 
 ## License
 
-pymetasnap is licensed under the MIT License. See the LICENSE file for more details.
+pymetasnap is licensed under the MIT License. See the [LICENSE](./LICENSE) file for more details.
 
 ## Acknowledgments
 
 The pymetasnap tool builds upon the PyPI API to provide a convenient way to access package metadata. We would like to express our gratitude to the PyPI maintainers and the Python community for their continuous efforts in maintaining and improving the Python Package Index.
 
 ## Contact
 
-For any inquiries or feedback, please contact the project maintainer at cristian.o.rincon.b@gmail.com.
+For any inquiries or feedback, please contact the project maintainer at cristian.o.rincon.b@gmail.com
```

### Comparing `pymetasnap-0.3.0/extractor/checks.py` & `pymetasnap-0.30.0/extractor/checks.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 
 import requests
 
 from extractor.logger import logger
 
 
 class StandardCheck:
+    def __init__(self):
+        self.project_default_error = "No project url found, please check manually"
+        self.version_default_error = "No version url found, please check manually"
+
     def gh_pattern(self, pattern: str, url: str, custom_error: str = None):
         try:
             found = re.search(pattern, url)
         except Exception as e:
             logger.warning(custom_error) if custom_error else logger.warning(e)
         else:
             return found
@@ -80,23 +84,20 @@
         return (
             default_url
             if self._url_exists(default_url)
             else f"{filtered_data['project_url']}/tree/v{version}/"
         )
 
     def version(self, version: str, pattern: str, filtered_data: Dict) -> Dict:
-        project_default_error = "No project url found, please check manually"
-        version_default_error = "No version url found, please check manually"
         if version and self.gh_pattern(
-            pattern, filtered_data.get("project_url"), project_default_error
+            pattern, filtered_data.get("project_url"), self.project_default_error
         ):
             project_url = self._version_handler(filtered_data, version)
             if _ := self._url_exists(project_url):
                 filtered_data["version_url"] = self._version_handler(
                     filtered_data, version
                 )
             else:
-                filtered_data["version_url"] = version_default_error
+                filtered_data["version_url"] = self.version_default_error
         else:
-            filtered_data["version_url"] = version_default_error
-
+            filtered_data["version_url"] = self.version_default_error
         return filtered_data
```

### Comparing `pymetasnap-0.3.0/extractor/main.py` & `pymetasnap-0.30.0/extractor/main.py`

 * *Files identical despite different names*

### Comparing `pymetasnap-0.3.0/extractor/render.py` & `pymetasnap-0.30.0/extractor/render.py`

 * *Files identical despite different names*

### Comparing `pymetasnap-0.3.0/pyproject.toml` & `pymetasnap-0.30.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 [tool.poetry]
 name = "pymetasnap"
-version = "0.3.0"
+version = "0.30.0"
 description = "This package allows you to scrape metadata from the Python Package Index"
 authors = ["cristian-rincon <cristian.o.rincon.b@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "extractor"}]
 
 [tool.poetry.scripts]
 pymetasnap = "extractor.main:app"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-typer = {extras = ["all"], version = "^0.9.0"}
+typer = {extras = ["all"], version = ">=0.9,<0.13"}
 rich = "^13.4.1"
 shellingham = "^1.5.0.post1"
 openpyxl = "^3.1.2"
 pandas = "^2.0.2"
 loguru = "^0.7.0"
 requests = "^2.31.0"
 toml = "^0.10.2"
+ghapi = "^1.0.4"
 
 
 [tool.poetry.group.dev.dependencies]
 black = {version = "^23.3.0", allow-prereleases = true}
 pytest = "^7.3.1"
 pre-commit = "^3.3.2"
 jupyterlab = "^4.0.2"
 pytest-xdist = "^3.3.1"
-pytest-sugar = "^0.9.7"
+pytest-sugar = ">=0.9.7,<1.1.0"
 pytest-cov = "^4.1.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pymetasnap-0.3.0/PKG-INFO` & `pymetasnap-0.30.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 Metadata-Version: 2.1
 Name: pymetasnap
-Version: 0.3.0
+Version: 0.30.0
 Summary: This package allows you to scrape metadata from the Python Package Index
 License: MIT
 Author: cristian-rincon
 Author-email: cristian.o.rincon.b@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: ghapi (>=1.0.4,<2.0.0)
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: pandas (>=2.0.2,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: rich (>=13.4.1,<14.0.0)
 Requires-Dist: shellingham (>=1.5.0.post1,<2.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
-Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
+Requires-Dist: typer[all] (>=0.9,<0.13)
 Description-Content-Type: text/markdown
 
-# pymetasnap
+# pymetasnap [![PyPI version](https://badge.fury.io/py/pymetasnap.svg)](https://badge.fury.io/py/pymetasnap)
 
 pymetasnap is a command-line tool that enables you to extract metadata from the Python Package Index (PyPI). It allows you to retrieve essential information about Python packages hosted on PyPI, including package names, versions, licenses, project URLs, and more.
 
 By leveraging the PyPI API, pymetasnap automates the process of gathering package metadata, making it convenient for developers, researchers, and anyone interested in exploring package information in a structured manner.
 
 ## Features
 
-Retrieve metadata for Python packages from PyPI.
-Extract package names, versions, licenses, and other relevant information.
-Fetch project URLs and version-specific URLs for detailed package exploration.
-Store the extracted metadata in CSV or Excel format for further analysis.
+- Retrieve metadata for Python packages from PyPI.
+- Extract package names, versions, licenses, and other relevant information.
+- Fetch project URLs and version-specific URLs for detailed package exploration.
+- Store the extracted metadata in CSV or Excel format for further analysis.
 
 ## Installation
 
 You can install pymetasnap using pip:
 
 ```bash
 pip install pymetasnap
@@ -73,17 +75,17 @@
 
 Contributions to pymetasnap are welcome! If you encounter any issues or have suggestions for improvements, please open an issue on the project's GitHub repository.
 
 When contributing, please ensure that you follow the existing coding style, write tests for new features, and make sure the tests pass before submitting a pull request.
 
 ## License
 
-pymetasnap is licensed under the MIT License. See the LICENSE file for more details.
+pymetasnap is licensed under the MIT License. See the [LICENSE](./LICENSE) file for more details.
 
 ## Acknowledgments
 
 The pymetasnap tool builds upon the PyPI API to provide a convenient way to access package metadata. We would like to express our gratitude to the PyPI maintainers and the Python community for their continuous efforts in maintaining and improving the Python Package Index.
 
 ## Contact
 
-For any inquiries or feedback, please contact the project maintainer at cristian.o.rincon.b@gmail.com.
+For any inquiries or feedback, please contact the project maintainer at cristian.o.rincon.b@gmail.com
```

