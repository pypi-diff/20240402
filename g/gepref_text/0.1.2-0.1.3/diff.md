# Comparing `tmp/gepref_text-0.1.2.tar.gz` & `tmp/gepref_text-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gepref_text-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "gepref_text-0.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gepref_text-0.1.2.tar` & `gepref_text-0.1.3.tar`

### file list

```diff
@@ -1,30 +1,35 @@
--rwxr-xr-x   0        0        0      243 2024-04-02 01:40:27.699357 gepref_text-0.1.2/.cicd/scripts.sh
--rw-r--r--   0        0        0      980 2024-04-02 01:40:27.699357 gepref_text-0.1.2/.github/workflows/cd.yml
--rw-r--r--   0        0        0      364 2024-04-02 01:40:27.699357 gepref_text-0.1.2/.github/workflows/ci.yml
--rw-r--r--   0        0        0      126 2024-04-02 01:40:27.699357 gepref_text-0.1.2/.gitignore
--rw-r--r--   0        0        0        7 2024-04-02 01:40:27.699357 gepref_text-0.1.2/.python-version
--rw-r--r--   0        0        0     1086 2024-04-02 01:40:27.703357 gepref_text-0.1.2/LICENSE
--rw-r--r--   0        0        0      427 2024-04-02 01:40:27.703357 gepref_text-0.1.2/Makefile
--rw-r--r--   0        0        0      528 2024-04-02 01:40:27.703357 gepref_text-0.1.2/README.md
--rw-r--r--   0        0        0      638 2024-04-02 01:40:27.703357 gepref_text-0.1.2/doc/Makefile
--rw-r--r--   0        0        0    12449 2024-04-02 01:40:27.703357 gepref_text-0.1.2/doc/source/_static/gepref_text.svg
--rw-r--r--   0        0        0    20860 2024-04-02 01:40:27.703357 gepref_text-0.1.2/doc/source/_static/preprocessor.svg
--rw-r--r--   0        0        0      764 2024-04-02 01:40:27.703357 gepref_text-0.1.2/doc/source/conf.py
--rw-r--r--   0        0        0      628 2024-04-02 01:40:27.703357 gepref_text-0.1.2/doc/source/gepref_text.rst
--rw-r--r--   0        0        0      521 2024-04-02 01:40:27.703357 gepref_text-0.1.2/doc/source/index.rst
--rw-r--r--   0        0        0      251 2024-04-02 01:40:27.703357 gepref_text-0.1.2/doc/source/installation.md
--rw-r--r--   0        0        0       70 2024-04-02 01:40:27.703357 gepref_text-0.1.2/doc/source/modules.rst
--rw-r--r--   0        0        0      986 2024-04-02 01:40:27.703357 gepref_text-0.1.2/doc/source/usage.rst
--rw-r--r--   0        0        0     1321 2024-04-02 01:40:27.703357 gepref_text-0.1.2/doc/source/usage/custom.md
--rw-r--r--   0        0        0      952 2024-04-02 01:40:27.703357 gepref_text-0.1.2/doc/source/usage/normalization.md
--rw-r--r--   0        0        0      744 2024-04-02 01:40:27.703357 gepref_text-0.1.2/doc/source/usage/preprocessor.md
--rw-r--r--   0        0        0     1507 2024-04-02 01:40:27.703357 gepref_text-0.1.2/doc/source/usage/regex.md
--rw-r--r--   0        0        0      615 2024-04-02 01:40:27.703357 gepref_text-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-02 01:40:27.703357 gepref_text-0.1.2/src/gepref_text/__init__.py
--rw-r--r--   0        0        0      525 2024-04-02 01:40:27.703357 gepref_text-0.1.2/src/gepref_text/base.py
--rw-r--r--   0        0        0     1898 2024-04-02 01:40:27.703357 gepref_text-0.1.2/src/gepref_text/normalization.py
--rw-r--r--   0        0        0        0 2024-04-02 01:40:27.703357 gepref_text-0.1.2/src/gepref_text/py.typed
--rw-r--r--   0        0        0     3374 2024-04-02 01:40:27.703357 gepref_text-0.1.2/src/gepref_text/regex.py
--rw-r--r--   0        0        0     1300 2024-04-02 01:40:27.703357 gepref_text-0.1.2/test/test_normalization.py
--rw-r--r--   0        0        0     2109 2024-04-02 01:40:27.703357 gepref_text-0.1.2/test/test_regex.py
--rw-r--r--   0        0        0      604 1970-01-01 00:00:00.000000 gepref_text-0.1.2/PKG-INFO
+-rwxr-xr-x   0        0        0      243 2024-04-02 02:48:43.295151 gepref_text-0.1.3/.cicd/scripts.sh
+-rw-r--r--   0        0        0      980 2024-04-02 02:48:43.295151 gepref_text-0.1.3/.github/workflows/cd.yml
+-rw-r--r--   0        0        0      364 2024-04-02 02:48:43.295151 gepref_text-0.1.3/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      126 2024-04-02 02:48:43.295151 gepref_text-0.1.3/.gitignore
+-rw-r--r--   0        0        0        7 2024-04-02 02:48:43.295151 gepref_text-0.1.3/.python-version
+-rw-r--r--   0        0        0     1086 2024-04-02 02:48:43.295151 gepref_text-0.1.3/LICENSE
+-rw-r--r--   0        0        0      457 2024-04-02 02:48:43.295151 gepref_text-0.1.3/Makefile
+-rw-r--r--   0        0        0     1548 2024-04-02 02:48:43.295151 gepref_text-0.1.3/README.md
+-rw-r--r--   0        0        0      638 2024-04-02 02:48:43.295151 gepref_text-0.1.3/doc/Makefile
+-rw-r--r--   0        0        0    12449 2024-04-02 02:48:43.295151 gepref_text-0.1.3/doc/source/_static/gepref_text.svg
+-rw-r--r--   0        0        0    20860 2024-04-02 02:48:43.295151 gepref_text-0.1.3/doc/source/_static/preprocessor.svg
+-rw-r--r--   0        0        0      764 2024-04-02 02:48:43.295151 gepref_text-0.1.3/doc/source/conf.py
+-rw-r--r--   0        0        0      791 2024-04-02 02:48:43.295151 gepref_text-0.1.3/doc/source/gepref_text.rst
+-rw-r--r--   0        0        0      521 2024-04-02 02:48:43.295151 gepref_text-0.1.3/doc/source/index.rst
+-rw-r--r--   0        0        0      251 2024-04-02 02:48:43.295151 gepref_text-0.1.3/doc/source/installation.md
+-rw-r--r--   0        0        0       70 2024-04-02 02:48:43.295151 gepref_text-0.1.3/doc/source/modules.rst
+-rw-r--r--   0        0        0     1151 2024-04-02 02:48:43.295151 gepref_text-0.1.3/doc/source/usage.rst
+-rw-r--r--   0        0        0     1321 2024-04-02 02:48:43.295151 gepref_text-0.1.3/doc/source/usage/custom.md
+-rw-r--r--   0        0        0      952 2024-04-02 02:48:43.295151 gepref_text-0.1.3/doc/source/usage/normalization.md
+-rw-r--r--   0        0        0      744 2024-04-02 02:48:43.295151 gepref_text-0.1.3/doc/source/usage/preprocessor.md
+-rw-r--r--   0        0        0     1507 2024-04-02 02:48:43.295151 gepref_text-0.1.3/doc/source/usage/regex.md
+-rw-r--r--   0        0        0     1060 2024-04-02 02:48:43.295151 gepref_text-0.1.3/doc/source/usage/tokenization.md
+-rw-r--r--   0        0        0      631 2024-04-02 02:48:43.295151 gepref_text-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-02 02:48:43.295151 gepref_text-0.1.3/src/gepref_text/__init__.py
+-rw-r--r--   0        0        0      525 2024-04-02 02:48:43.295151 gepref_text-0.1.3/src/gepref_text/base.py
+-rw-r--r--   0        0        0     1898 2024-04-02 02:48:43.295151 gepref_text-0.1.3/src/gepref_text/normalization.py
+-rw-r--r--   0        0        0        0 2024-04-02 02:48:43.295151 gepref_text-0.1.3/src/gepref_text/py.typed
+-rw-r--r--   0        0        0     3374 2024-04-02 02:48:43.295151 gepref_text-0.1.3/src/gepref_text/regex.py
+-rw-r--r--   0        0        0     1218 2024-04-02 02:48:43.295151 gepref_text-0.1.3/src/gepref_text/tokenization.py
+-rw-r--r--   0        0        0        0 2024-04-02 02:48:43.295151 gepref_text-0.1.3/stubs/nltk/__init__.pyi
+-rw-r--r--   0        0        0      149 2024-04-02 02:48:43.295151 gepref_text-0.1.3/stubs/nltk/tokenize.pyi
+-rw-r--r--   0        0        0     1300 2024-04-02 02:48:43.295151 gepref_text-0.1.3/test/test_normalization.py
+-rw-r--r--   0        0        0     2109 2024-04-02 02:48:43.295151 gepref_text-0.1.3/test/test_regex.py
+-rw-r--r--   0        0        0      879 2024-04-02 02:48:43.295151 gepref_text-0.1.3/test/test_tokenization.py
+-rw-r--r--   0        0        0      631 1970-01-01 00:00:00.000000 gepref_text-0.1.3/PKG-INFO
```

### Comparing `gepref_text-0.1.2/.github/workflows/cd.yml` & `gepref_text-0.1.3/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `gepref_text-0.1.2/LICENSE` & `gepref_text-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gepref_text-0.1.2/doc/Makefile` & `gepref_text-0.1.3/doc/Makefile`

 * *Files identical despite different names*

### Comparing `gepref_text-0.1.2/doc/source/_static/gepref_text.svg` & `gepref_text-0.1.3/doc/source/_static/gepref_text.svg`

 * *Files identical despite different names*

### Comparing `gepref_text-0.1.2/doc/source/_static/preprocessor.svg` & `gepref_text-0.1.3/doc/source/_static/preprocessor.svg`

 * *Files identical despite different names*

### Comparing `gepref_text-0.1.2/doc/source/conf.py` & `gepref_text-0.1.3/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `gepref_text-0.1.2/doc/source/gepref_text.rst` & `gepref_text-0.1.3/doc/source/gepref_text.rst`

 * *Files 18% similar despite different names*

```diff
@@ -24,14 +24,22 @@
 -------------------------
 
 .. automodule:: gepref_text.regex
    :members:
    :undoc-members:
    :show-inheritance:
 
+gepref\_text.tokenization module
+--------------------------------
+
+.. automodule:: gepref_text.tokenization
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 Module contents
 ---------------
 
 .. automodule:: gepref_text
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `gepref_text-0.1.2/doc/source/index.rst` & `gepref_text-0.1.3/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `gepref_text-0.1.2/doc/source/usage.rst` & `gepref_text-0.1.3/doc/source/usage.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Usage Guide
 ===========
 
 In this guide we'll explore how to create preprocessing pipelines for text using the different functionalities available in ``gepref_text``. This includes:
 
 * **Preprocessor**: the preprocessor is the main class that orchestates the preprocessing. It composes several preprocessing steps and allows to generate a clean text string from a raw text string.
 * **Normalization**: the ``normalization`` module contains several components for text normalization. This includes writing modification, unicode normalization, and trimming.
+* **Tokenization**: the ``tokenization`` module allows to split tokens using different tokenization techniques (word, sentence, among others).
 * **Regex substitution**: the ``regex`` module includes components for regex-based text substitution, allowing to replace special characters, numbers, duplicated spaces, URLs, among others.
 * **Custom**: you can create custom components that can be directly integrated in the preprocessing pipelines.
 
 .. toctree::
    :maxdepth: 3
    :caption: Contents:
 
    usage/preprocessor
    usage/normalization
    usage/regex
+   usage/tokenization
    usage/custom
```

### Comparing `gepref_text-0.1.2/doc/source/usage/custom.md` & `gepref_text-0.1.3/doc/source/usage/custom.md`

 * *Files identical despite different names*

### Comparing `gepref_text-0.1.2/doc/source/usage/normalization.md` & `gepref_text-0.1.3/doc/source/usage/normalization.md`

 * *Files identical despite different names*

### Comparing `gepref_text-0.1.2/doc/source/usage/preprocessor.md` & `gepref_text-0.1.3/doc/source/usage/preprocessor.md`

 * *Files identical despite different names*

### Comparing `gepref_text-0.1.2/doc/source/usage/regex.md` & `gepref_text-0.1.3/doc/source/usage/regex.md`

 * *Files identical despite different names*

### Comparing `gepref_text-0.1.2/pyproject.toml` & `gepref_text-0.1.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gepref_text"
-version = "0.1.2"
+version = "0.1.3"
 description = "GEneral PREprocessing Framework for TEXT (gepref_text)"
 authors = [{name="Juan Lara", email="julara@unal.edu.co"}]
 requires-python = ">3.10"
 dependencies = [
 	"gepref==0.1.1",
-	"unidecode==1.3.8"
+	"unidecode==1.3.8",
+	"nltk==3.8.1"
 ]
 
 [project.optional-dependencies]
 dev = [
 	"jedi-language-server", "mypy", "pytest", "ruff", "flit",
 	"sphinx", "sphinx-book-theme", "myst_parser"
 ]
```

### Comparing `gepref_text-0.1.2/src/gepref_text/base.py` & `gepref_text-0.1.3/src/gepref_text/base.py`

 * *Files identical despite different names*

### Comparing `gepref_text-0.1.2/src/gepref_text/normalization.py` & `gepref_text-0.1.3/src/gepref_text/normalization.py`

 * *Files identical despite different names*

### Comparing `gepref_text-0.1.2/src/gepref_text/regex.py` & `gepref_text-0.1.3/src/gepref_text/regex.py`

 * *Files identical despite different names*

### Comparing `gepref_text-0.1.2/test/test_normalization.py` & `gepref_text-0.1.3/test/test_normalization.py`

 * *Files identical despite different names*

### Comparing `gepref_text-0.1.2/test/test_regex.py` & `gepref_text-0.1.3/test/test_regex.py`

 * *Files identical despite different names*

### Comparing `gepref_text-0.1.2/PKG-INFO` & `gepref_text-0.1.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: gepref_text
-Version: 0.1.2
+Version: 0.1.3
 Summary: GEneral PREprocessing Framework for TEXT (gepref_text)
 Author-email: Juan Lara <julara@unal.edu.co>
 Requires-Python: >3.10
 Requires-Dist: gepref==0.1.1
 Requires-Dist: unidecode==1.3.8
+Requires-Dist: nltk==3.8.1
 Requires-Dist: jedi-language-server ; extra == "dev"
 Requires-Dist: mypy ; extra == "dev"
 Requires-Dist: pytest ; extra == "dev"
 Requires-Dist: ruff ; extra == "dev"
 Requires-Dist: flit ; extra == "dev"
 Requires-Dist: sphinx ; extra == "dev"
 Requires-Dist: sphinx-book-theme ; extra == "dev"
```

