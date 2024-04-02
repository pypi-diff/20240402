# Comparing `tmp/monodikit-0.0.3.tar.gz` & `tmp/monodikit-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monodikit-0.0.3.tar", last modified: Wed Feb 14 14:46:07 2024, max compression
+gzip compressed data, was "monodikit-0.0.4.tar", last modified: Mon Mar  4 10:48:48 2024, max compression
```

## Comparing `monodikit-0.0.3.tar` & `monodikit-0.0.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 timeipert   (501) staff       (20)        0 2024-02-14 14:46:07.466435 monodikit-0.0.3/
--rw-r--r--   0 timeipert   (501) staff       (20)     2367 2024-02-14 14:46:07.466287 monodikit-0.0.3/PKG-INFO
-drwxr-xr-x   0 timeipert   (501) staff       (20)        0 2024-02-14 14:46:07.460820 monodikit-0.0.3/app/
-drwxr-xr-x   0 timeipert   (501) staff       (20)        0 2024-02-14 14:46:07.461047 monodikit-0.0.3/app/monodikit/
--rw-r--r--   0 timeipert   (501) staff       (20)      477 2023-10-18 10:30:41.000000 monodikit-0.0.3/app/monodikit/__init__.py
-drwxr-xr-x   0 timeipert   (501) staff       (20)        0 2024-02-14 14:46:07.462725 monodikit-0.0.3/app/monodikit/analysis/
--rw-r--r--   0 timeipert   (501) staff       (20)        0 2023-10-18 09:29:46.000000 monodikit-0.0.3/app/monodikit/analysis/__init__.py
--rw-r--r--   0 timeipert   (501) staff       (20)     6878 2023-10-18 12:18:27.000000 monodikit-0.0.3/app/monodikit/analysis/search.py
--rw-r--r--   0 timeipert   (501) staff       (20)     3582 2023-10-18 10:30:41.000000 monodikit-0.0.3/app/monodikit/analysis/synopsis.py
--rw-r--r--   0 timeipert   (501) staff       (20)     1186 2023-10-18 09:29:46.000000 monodikit-0.0.3/app/monodikit/analysis/utility.py
-drwxr-xr-x   0 timeipert   (501) staff       (20)        0 2024-02-14 14:46:07.463673 monodikit-0.0.3/app/monodikit/models/
--rw-r--r--   0 timeipert   (501) staff       (20)        0 2023-06-01 16:26:35.000000 monodikit-0.0.3/app/monodikit/models/__init__.py
--rw-r--r--   0 timeipert   (501) staff       (20)     6452 2023-10-18 10:39:07.000000 monodikit-0.0.3/app/monodikit/models/corpus.py
--rw-r--r--   0 timeipert   (501) staff       (20)    21585 2024-02-14 14:30:19.000000 monodikit-0.0.3/app/monodikit/models/document.py
--rw-r--r--   0 timeipert   (501) staff       (20)     3686 2023-10-18 09:28:37.000000 monodikit-0.0.3/app/monodikit/models/genre_specific.py
--rw-r--r--   0 timeipert   (501) staff       (20)     2475 2024-02-14 13:19:26.000000 monodikit-0.0.3/app/monodikit/models/source.py
-drwxr-xr-x   0 timeipert   (501) staff       (20)        0 2024-02-14 14:46:07.461804 monodikit-0.0.3/app/monodikit.egg-info/
--rw-r--r--   0 timeipert   (501) staff       (20)     2367 2024-02-14 14:46:07.000000 monodikit-0.0.3/app/monodikit.egg-info/PKG-INFO
--rw-r--r--   0 timeipert   (501) staff       (20)      619 2024-02-14 14:46:07.000000 monodikit-0.0.3/app/monodikit.egg-info/SOURCES.txt
--rw-r--r--   0 timeipert   (501) staff       (20)        1 2024-02-14 14:46:07.000000 monodikit-0.0.3/app/monodikit.egg-info/dependency_links.txt
--rw-r--r--   0 timeipert   (501) staff       (20)       16 2024-02-14 14:46:07.000000 monodikit-0.0.3/app/monodikit.egg-info/top_level.txt
-drwxr-xr-x   0 timeipert   (501) staff       (20)        0 2024-02-14 14:46:07.465955 monodikit-0.0.3/app/tests/
--rw-r--r--   0 timeipert   (501) staff       (20)        0 2023-10-18 10:30:41.000000 monodikit-0.0.3/app/tests/__init__.py
--rw-r--r--   0 timeipert   (501) staff       (20)   264429 2024-02-14 13:26:16.000000 monodikit-0.0.3/app/tests/mock_data.py
--rw-r--r--   0 timeipert   (501) staff       (20)      824 2024-02-14 13:30:07.000000 monodikit-0.0.3/app/tests/test_corpus.py
--rw-r--r--   0 timeipert   (501) staff       (20)     4597 2023-10-18 10:30:41.000000 monodikit-0.0.3/app/tests/test_document.py
--rw-r--r--   0 timeipert   (501) staff       (20)      671 2024-02-14 13:33:05.000000 monodikit-0.0.3/app/tests/test_metadata_creation.py
--rw-r--r--   0 timeipert   (501) staff       (20)       38 2024-02-14 14:46:07.466472 monodikit-0.0.3/setup.cfg
--rw-r--r--   0 timeipert   (501) staff       (20)     1125 2024-02-14 14:45:59.000000 monodikit-0.0.3/setup.py
+drwxr-xr-x   0 timeipert   (501) staff       (20)        0 2024-03-04 10:48:48.479548 monodikit-0.0.4/
+-rw-r--r--   0 timeipert   (501) staff       (20)     2440 2024-03-04 10:48:48.479387 monodikit-0.0.4/PKG-INFO
+drwxr-xr-x   0 timeipert   (501) staff       (20)        0 2024-03-04 10:48:48.472907 monodikit-0.0.4/app/
+drwxr-xr-x   0 timeipert   (501) staff       (20)        0 2024-03-04 10:48:48.473189 monodikit-0.0.4/app/monodikit/
+-rw-r--r--   0 timeipert   (501) staff       (20)      477 2023-10-18 10:30:41.000000 monodikit-0.0.4/app/monodikit/__init__.py
+drwxr-xr-x   0 timeipert   (501) staff       (20)        0 2024-03-04 10:48:48.474875 monodikit-0.0.4/app/monodikit/analysis/
+-rw-r--r--   0 timeipert   (501) staff       (20)        0 2023-10-18 09:29:46.000000 monodikit-0.0.4/app/monodikit/analysis/__init__.py
+-rw-r--r--   0 timeipert   (501) staff       (20)     6878 2023-10-18 12:18:27.000000 monodikit-0.0.4/app/monodikit/analysis/search.py
+-rw-r--r--   0 timeipert   (501) staff       (20)     3723 2024-03-04 10:46:15.000000 monodikit-0.0.4/app/monodikit/analysis/synopsis.py
+-rw-r--r--   0 timeipert   (501) staff       (20)     1186 2023-10-18 09:29:46.000000 monodikit-0.0.4/app/monodikit/analysis/utility.py
+drwxr-xr-x   0 timeipert   (501) staff       (20)        0 2024-03-04 10:48:48.476106 monodikit-0.0.4/app/monodikit/models/
+-rw-r--r--   0 timeipert   (501) staff       (20)        0 2023-06-01 16:26:35.000000 monodikit-0.0.4/app/monodikit/models/__init__.py
+-rw-r--r--   0 timeipert   (501) staff       (20)     6452 2023-10-18 10:39:07.000000 monodikit-0.0.4/app/monodikit/models/corpus.py
+-rw-r--r--   0 timeipert   (501) staff       (20)    21585 2024-02-14 14:30:19.000000 monodikit-0.0.4/app/monodikit/models/document.py
+-rw-r--r--   0 timeipert   (501) staff       (20)     3686 2023-10-18 09:28:37.000000 monodikit-0.0.4/app/monodikit/models/genre_specific.py
+-rw-r--r--   0 timeipert   (501) staff       (20)     2475 2024-02-14 13:19:26.000000 monodikit-0.0.4/app/monodikit/models/source.py
+drwxr-xr-x   0 timeipert   (501) staff       (20)        0 2024-03-04 10:48:48.473890 monodikit-0.0.4/app/monodikit.egg-info/
+-rw-r--r--   0 timeipert   (501) staff       (20)     2440 2024-03-04 10:48:48.000000 monodikit-0.0.4/app/monodikit.egg-info/PKG-INFO
+-rw-r--r--   0 timeipert   (501) staff       (20)      619 2024-03-04 10:48:48.000000 monodikit-0.0.4/app/monodikit.egg-info/SOURCES.txt
+-rw-r--r--   0 timeipert   (501) staff       (20)        1 2024-03-04 10:48:48.000000 monodikit-0.0.4/app/monodikit.egg-info/dependency_links.txt
+-rw-r--r--   0 timeipert   (501) staff       (20)       16 2024-03-04 10:48:48.000000 monodikit-0.0.4/app/monodikit.egg-info/top_level.txt
+drwxr-xr-x   0 timeipert   (501) staff       (20)        0 2024-03-04 10:48:48.478972 monodikit-0.0.4/app/tests/
+-rw-r--r--   0 timeipert   (501) staff       (20)        0 2023-10-18 10:30:41.000000 monodikit-0.0.4/app/tests/__init__.py
+-rw-r--r--   0 timeipert   (501) staff       (20)   264429 2024-02-14 13:26:16.000000 monodikit-0.0.4/app/tests/mock_data.py
+-rw-r--r--   0 timeipert   (501) staff       (20)      824 2024-02-14 13:30:07.000000 monodikit-0.0.4/app/tests/test_corpus.py
+-rw-r--r--   0 timeipert   (501) staff       (20)     4597 2023-10-18 10:30:41.000000 monodikit-0.0.4/app/tests/test_document.py
+-rw-r--r--   0 timeipert   (501) staff       (20)      671 2024-02-14 13:33:05.000000 monodikit-0.0.4/app/tests/test_metadata_creation.py
+-rw-r--r--   0 timeipert   (501) staff       (20)       38 2024-03-04 10:48:48.479598 monodikit-0.0.4/setup.cfg
+-rw-r--r--   0 timeipert   (501) staff       (20)     1125 2024-03-04 10:47:56.000000 monodikit-0.0.4/setup.py
```

### Comparing `monodikit-0.0.3/PKG-INFO` & `monodikit-0.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monodikit
-Version: 0.0.3
+Version: 0.0.4
 Summary: MonodiKit is a Python library designed to facilitate the analysis and processing of medieval chant documents. It was specifically tailored to handle data in the monodi+ data format as edited by the Corpus Monodicum project. The library offers a set of classes that provide a wide range of functionalities, including parsing and processing of chant documents, exploring their hierarchical structure, managing metadata, generating musical notation, and extracting relevant information.
 Home-page: https://github.com/timeipert/MonodiKit
 Author: Tim Eipert & Fabian C. Moss
 Author-email: tim.eipert@uni-wuerzburg.de
 License: MIT
 Classifier: 
 Requires-Python: >=3.8
@@ -60,7 +60,10 @@
 ## Version History
 * 0.0.1
     * Initial Release
 * 0.0.2
   * Updated Data Structure and Exception Handling
 * 0.0.3
   * Better Volpiano Support
+* 0.0.4
+  * Changed MAFFT configuration
+  * Supports matrixfile in MAFFT
```

### Comparing `monodikit-0.0.3/app/monodikit/analysis/search.py` & `monodikit-0.0.4/app/monodikit/analysis/search.py`

 * *Files identical despite different names*

### Comparing `monodikit-0.0.3/app/monodikit/analysis/synopsis.py` & `monodikit-0.0.4/app/monodikit/analysis/synopsis.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 import subprocess
 class Synopsis:
     @staticmethod
-    def run_mafft(input_data):
+    def run_mafft(input_data, textmatrix_file = None):
         """
         Runs the MAFFT multiple sequence alignment tool on the given input data.
 
         Args:
             input_data (dict): Dictionary with sequence names as keys and sequences as values.
 
         Returns:
             list: List of dictionaries containing sequence names and aligned sequences.
         """
         input_content = Synopsis.parse_mafft_input(input_data)
         with open("temp.fasta", "w") as f:
             f.write(input_content)
-        command = f"mafft --auto --anysymbol temp.fasta"
+        if textmatrix_file:
+            tmf = f"--textmatrix {textmatrix_file}"
+        else:
+            tmf = ""
+
+        command = f"mafft --auto --text {tmf} temp.fasta"
         out = subprocess.run(command, shell=True, capture_output=True)
 
         return Synopsis.parse_mafft_output(str(out.stdout))
 
     @staticmethod
     def parse_mafft_input(input_data):
         """
```

### Comparing `monodikit-0.0.3/app/monodikit/analysis/utility.py` & `monodikit-0.0.4/app/monodikit/analysis/utility.py`

 * *Files identical despite different names*

### Comparing `monodikit-0.0.3/app/monodikit/models/corpus.py` & `monodikit-0.0.4/app/monodikit/models/corpus.py`

 * *Files identical despite different names*

### Comparing `monodikit-0.0.3/app/monodikit/models/document.py` & `monodikit-0.0.4/app/monodikit/models/document.py`

 * *Files identical despite different names*

### Comparing `monodikit-0.0.3/app/monodikit/models/genre_specific.py` & `monodikit-0.0.4/app/monodikit/models/genre_specific.py`

 * *Files identical despite different names*

### Comparing `monodikit-0.0.3/app/monodikit/models/source.py` & `monodikit-0.0.4/app/monodikit/models/source.py`

 * *Files identical despite different names*

### Comparing `monodikit-0.0.3/app/monodikit.egg-info/PKG-INFO` & `monodikit-0.0.4/app/monodikit.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monodikit
-Version: 0.0.3
+Version: 0.0.4
 Summary: MonodiKit is a Python library designed to facilitate the analysis and processing of medieval chant documents. It was specifically tailored to handle data in the monodi+ data format as edited by the Corpus Monodicum project. The library offers a set of classes that provide a wide range of functionalities, including parsing and processing of chant documents, exploring their hierarchical structure, managing metadata, generating musical notation, and extracting relevant information.
 Home-page: https://github.com/timeipert/MonodiKit
 Author: Tim Eipert & Fabian C. Moss
 Author-email: tim.eipert@uni-wuerzburg.de
 License: MIT
 Classifier: 
 Requires-Python: >=3.8
@@ -60,7 +60,10 @@
 ## Version History
 * 0.0.1
     * Initial Release
 * 0.0.2
   * Updated Data Structure and Exception Handling
 * 0.0.3
   * Better Volpiano Support
+* 0.0.4
+  * Changed MAFFT configuration
+  * Supports matrixfile in MAFFT
```

### Comparing `monodikit-0.0.3/app/monodikit.egg-info/SOURCES.txt` & `monodikit-0.0.4/app/monodikit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `monodikit-0.0.3/app/tests/mock_data.py` & `monodikit-0.0.4/app/tests/mock_data.py`

 * *Files identical despite different names*

### Comparing `monodikit-0.0.3/app/tests/test_corpus.py` & `monodikit-0.0.4/app/tests/test_corpus.py`

 * *Files identical despite different names*

### Comparing `monodikit-0.0.3/app/tests/test_document.py` & `monodikit-0.0.4/app/tests/test_document.py`

 * *Files identical despite different names*

### Comparing `monodikit-0.0.3/app/tests/test_metadata_creation.py` & `monodikit-0.0.4/app/tests/test_metadata_creation.py`

 * *Files identical despite different names*

### Comparing `monodikit-0.0.3/setup.py` & `monodikit-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("app/Readme.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="monodikit",
-    version="0.0.3",
+    version="0.0.4",
     description="MonodiKit is a Python library designed to facilitate the analysis and processing of medieval chant documents. It was specifically tailored to handle data in the monodi+ data format as edited by the Corpus Monodicum project. The library offers a set of classes that provide a wide range of functionalities, including parsing and processing of chant documents, exploring their hierarchical structure, managing metadata, generating musical notation, and extracting relevant information.",
     package_dir={"": "app"},
     packages=find_packages(where="app"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/timeipert/MonodiKit",
     author="Tim Eipert & Fabian C. Moss",
```

