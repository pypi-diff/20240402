# Comparing `tmp/arm_preprocessing-0.2.1.tar.gz` & `tmp/arm_preprocessing-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arm_preprocessing-0.2.1.tar", max compression
+gzip compressed data, was "arm_preprocessing-0.2.2.tar", max compression
```

## Comparing `arm_preprocessing-0.2.1.tar` & `arm_preprocessing-0.2.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       23 2024-02-19 13:23:02.710415 arm_preprocessing-0.2.1/arm_preprocessing/__init__.py
--rw-r--r--   0        0        0    18050 2024-02-19 12:58:27.744198 arm_preprocessing-0.2.1/arm_preprocessing/dataset.py
--rw-r--r--   0        0        0     2590 2024-01-05 08:27:29.995215 arm_preprocessing-0.2.1/arm_preprocessing/discretisation.py
--rw-r--r--   0        0        0      666 2024-01-05 07:52:32.720645 arm_preprocessing-0.2.1/arm_preprocessing/squashing.py
--rw-r--r--   0        0        0      225 2023-11-22 18:33:12.331022 arm_preprocessing-0.2.1/arm_preprocessing/timeseries.py
--rw-r--r--   0        0        0     1099 2024-02-12 08:58:50.488453 arm_preprocessing-0.2.1/LICENSE
--rw-r--r--   0        0        0     1054 2024-02-19 13:22:52.681485 arm_preprocessing-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     8898 2024-02-19 13:03:53.286658 arm_preprocessing-0.2.1/README.md
--rw-r--r--   0        0        0     9849 1970-01-01 00:00:00.000000 arm_preprocessing-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-04-02 08:27:01.865774 arm_preprocessing-0.2.2/LICENSE
+-rw-r--r--   0        0        0     8724 2024-04-02 08:27:01.865774 arm_preprocessing-0.2.2/README.md
+-rw-r--r--   0        0        0       22 2024-04-02 08:27:01.865774 arm_preprocessing-0.2.2/arm_preprocessing/__init__.py
+-rw-r--r--   0        0        0    17542 2024-04-02 08:27:01.865774 arm_preprocessing-0.2.2/arm_preprocessing/dataset.py
+-rw-r--r--   0        0        0     2517 2024-04-02 08:27:01.865774 arm_preprocessing-0.2.2/arm_preprocessing/discretisation.py
+-rw-r--r--   0        0        0      643 2024-04-02 08:27:01.866774 arm_preprocessing-0.2.2/arm_preprocessing/squashing.py
+-rw-r--r--   0        0        0      217 2024-04-02 08:27:01.866774 arm_preprocessing-0.2.2/arm_preprocessing/timeseries.py
+-rw-r--r--   0        0        0     1024 2024-04-02 08:27:01.885774 arm_preprocessing-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     9797 1970-01-01 00:00:00.000000 arm_preprocessing-0.2.2/PKG-INFO
```

### Comparing `arm_preprocessing-0.2.1/LICENSE` & `arm_preprocessing-0.2.2/LICENSE`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022-2024 Iztok Fister Jr.
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2022-2024 Iztok Fister Jr.
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `arm_preprocessing-0.2.1/pyproject.toml` & `arm_preprocessing-0.2.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-[tool.poetry]
-name = "arm-preprocessing"
-version = "0.2.1"
-description = "Implementation of several preprocessing techniques for Association Rule Mining (ARM)"
-authors = ["Tadej Lahovnik <lahovnik.tadej@gmail.com>", "Iztok Fister Jr. <iztok@iztok-jr-fister.eu>"]
-keywords = ['association rule mining', 'data science', 'preprocessing']
-homepage = "https://github.com/firefly-cpp/arm-preprocessing"
-repository = "https://github.com/firefly-cpp/arm-preprocessing"
-documentation = "http://arm-preprocessing.readthedocs.io"
-readme = "README.md"
-
-[tool.poetry.dependencies]
-python = ">=3.9,<3.13"
-pandas = ">=2.1.1,<3.0.0"
-Sphinx = {version = "^5.0", optional = true}
-sphinx-rtd-theme = {version = "^1.0.0", optional = true}
-scikit-learn = "^1.3.2"
-niaarm = "^0.3.5"
-sport-activities-features = "^0.3.18"
-
-[tool.poetry.dev-dependencies]
-pytest = "^7.4.4"
-
-[tool.poetry.extras]
-docs = ["Sphinx", "sphinx-rtd-theme", "sphinxcontrib-bibtex"]
-
-[build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+[tool.poetry]
+name = "arm-preprocessing"
+version = "0.2.2"
+description = "Implementation of several preprocessing techniques for Association Rule Mining (ARM)"
+authors = ["Tadej Lahovnik <lahovnik.tadej@gmail.com>", "Iztok Fister Jr. <iztok@iztok-jr-fister.eu>"]
+keywords = ['association rule mining', 'data science', 'preprocessing']
+homepage = "https://github.com/firefly-cpp/arm-preprocessing"
+repository = "https://github.com/firefly-cpp/arm-preprocessing"
+documentation = "http://arm-preprocessing.readthedocs.io"
+readme = "README.md"
+
+[tool.poetry.dependencies]
+python = ">=3.9,<3.13"
+pandas = ">=2.1.1,<3.0.0"
+Sphinx = {version = "^5.0", optional = true}
+sphinx-rtd-theme = {version = "^1.0.0", optional = true}
+scikit-learn = "^1.3.2"
+niaarm = "^0.3.5"
+sport-activities-features = "^0.4.0"
+
+[tool.poetry.dev-dependencies]
+pytest = "^7.4.4"
+
+[tool.poetry.extras]
+docs = ["Sphinx", "sphinx-rtd-theme", "sphinxcontrib-bibtex"]
+
+[build-system]
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `arm_preprocessing-0.2.1/PKG-INFO` & `arm_preprocessing-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: arm-preprocessing
-Version: 0.2.1
+Version: 0.2.2
 Summary: Implementation of several preprocessing techniques for Association Rule Mining (ARM)
 Home-page: https://github.com/firefly-cpp/arm-preprocessing
 Keywords: association rule mining,data science,preprocessing
 Author: Tadej Lahovnik
 Author-email: lahovnik.tadej@gmail.com
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: docs
 Requires-Dist: Sphinx (>=5.0,<6.0) ; extra == "docs"
 Requires-Dist: niaarm (>=0.3.5,<0.4.0)
 Requires-Dist: pandas (>=2.1.1,<3.0.0)
 Requires-Dist: scikit-learn (>=1.3.2,<2.0.0)
 Requires-Dist: sphinx-rtd-theme (>=1.0.0,<2.0.0) ; extra == "docs"
-Requires-Dist: sport-activities-features (>=0.3.18,<0.4.0)
+Requires-Dist: sport-activities-features (>=0.4.0,<0.5.0)
 Project-URL: Documentation, http://arm-preprocessing.readthedocs.io
 Project-URL: Repository, https://github.com/firefly-cpp/arm-preprocessing
 Description-Content-Type: text/markdown
 
 <p align="center">
   <img alt="logo" width="300" src=".github/images/logo_black.png">
 </p>
```

