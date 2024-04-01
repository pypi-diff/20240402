# Comparing `tmp/safepull-2.1.0.tar.gz` & `tmp/safepull-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safepull-2.1.0.tar", max compression
+gzip compressed data, was "safepull-2.1.1.tar", max compression
```

## Comparing `safepull-2.1.0.tar` & `safepull-2.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1060 2024-02-20 19:54:16.254224 safepull-2.1.0/LICENSE
--rw-r--r--   0        0        0     5359 2024-02-20 19:54:16.254224 safepull-2.1.0/README.md
--rw-r--r--   0        0        0      685 2024-02-20 19:54:16.258224 safepull-2.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-20 19:54:16.258224 safepull-2.1.0/src/safepull/__init__.py
--rw-r--r--   0        0        0       64 2024-02-20 19:54:16.258224 safepull-2.1.0/src/safepull/__main__.py
--rw-r--r--   0        0        0     3058 2024-02-20 19:54:16.258224 safepull-2.1.0/src/safepull/models.py
--rw-r--r--   0        0        0     3501 2024-02-20 19:54:16.258224 safepull-2.1.0/src/safepull/safepull.py
--rw-r--r--   0        0        0     6017 1970-01-01 00:00:00.000000 safepull-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1060 2024-04-01 23:47:47.905048 safepull-2.1.1/LICENSE
+-rw-r--r--   0        0        0     5359 2024-04-01 23:47:47.905048 safepull-2.1.1/README.md
+-rw-r--r--   0        0        0      693 2024-04-01 23:47:47.905048 safepull-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-01 23:47:47.905048 safepull-2.1.1/src/safepull/__init__.py
+-rw-r--r--   0        0        0       64 2024-04-01 23:47:47.905048 safepull-2.1.1/src/safepull/__main__.py
+-rw-r--r--   0        0        0     3058 2024-04-01 23:47:47.905048 safepull-2.1.1/src/safepull/models.py
+-rw-r--r--   0        0        0     3571 2024-04-01 23:47:47.905048 safepull-2.1.1/src/safepull/safepull.py
+-rw-r--r--   0        0        0     6017 1970-01-01 00:00:00.000000 safepull-2.1.1/PKG-INFO
```

### Comparing `safepull-2.1.0/LICENSE` & `safepull-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `safepull-2.1.0/README.md` & `safepull-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `safepull-2.1.0/pyproject.toml` & `safepull-2.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "safepull"
-version = "2.1.0"
+version = "2.1.1"
 description = "A CLI tool for downloading and extracting packages from PyPI without interfacing with setup.py."
 authors = ["Rem <128343390+import-pandas-as-numpy@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.scripts]
 safepull = "safepull.safepull:run"
@@ -22,8 +22,8 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
 target-version = "py311"
 select = ["ALL"]
-ignore = ["ANN101", "ANN206", "ANN102"]
+ignore = ["ANN101", "ANN206", "ANN102", "S202"]
```

### Comparing `safepull-2.1.0/src/safepull/models.py` & `safepull-2.1.1/src/safepull/models.py`

 * *Files identical despite different names*

### Comparing `safepull-2.1.0/src/safepull/safepull.py` & `safepull-2.1.1/src/safepull/safepull.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """Safepull module for the safe handling of compressed Python scripts."""
+
 # ruff: noqa: T201
 
 import argparse
 import tarfile
 from io import BytesIO
+from pathlib import Path
 from zipfile import ZipFile
 
 import requests
 from rich.console import Console
 
 from .models import Package
 
@@ -39,15 +41,15 @@
                     "This may present a security risk of path traversal.",
                     sep="\n",
                 )
                 if input('To ignore this, enter "Y": ').upper() == "Y":
                     sdist_tar.extractall()
     if filename.endswith((".whl", ".zip")):
         with ZipFile(byte_object) as whl_zip:
-            whl_zip.extractall()
+            whl_zip.extractall(path=Path.cwd().joinpath(f"{filename[:-4]}"))
 
 
 def run() -> None:
     """Run the program."""
     console = Console()
     parser = argparse.ArgumentParser(
         prog="Safepull",
```

### Comparing `safepull-2.1.0/PKG-INFO` & `safepull-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safepull
-Version: 2.1.0
+Version: 2.1.1
 Summary: A CLI tool for downloading and extracting packages from PyPI without interfacing with setup.py.
 License: MIT
 Author: Rem
 Author-email: 128343390+import-pandas-as-numpy@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

