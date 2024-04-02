# Comparing `tmp/datafog-2.4.0b3.tar.gz` & `tmp/datafog-2.4.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datafog-2.4.0b3.tar", last modified: Mon Apr  1 03:56:54 2024, max compression
+gzip compressed data, was "datafog-2.4.0b4.tar", last modified: Tue Apr  2 02:16:36 2024, max compression
```

## Comparing `datafog-2.4.0b3.tar` & `datafog-2.4.0b4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-04-01 03:56:54.835941 datafog-2.4.0b3/
--rw-r--r--   0 sidmohan   (501) staff       (20)     1091 2024-03-28 17:43:37.000000 datafog-2.4.0b3/LICENSE
--rw-r--r--   0 sidmohan   (501) staff       (20)     7749 2024-04-01 03:56:54.835685 datafog-2.4.0b3/PKG-INFO
--rw-r--r--   0 sidmohan   (501) staff       (20)     6355 2024-03-28 17:43:37.000000 datafog-2.4.0b3/README.md
--rw-r--r--   0 sidmohan   (501) staff       (20)       38 2024-04-01 03:56:54.836103 datafog-2.4.0b3/setup.cfg
--rw-r--r--   0 sidmohan   (501) staff       (20)     1712 2024-04-01 03:56:30.000000 datafog-2.4.0b3/setup.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-04-01 03:56:54.831581 datafog-2.4.0b3/src/
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-04-01 03:56:54.832921 datafog-2.4.0b3/src/datafog/
--rw-r--r--   0 sidmohan   (501) staff       (20)       53 2024-03-28 17:43:37.000000 datafog-2.4.0b3/src/datafog/__about__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     4362 2024-04-01 03:54:06.000000 datafog-2.4.0b3/src/datafog/__init__.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-04-01 03:56:54.831733 datafog-2.4.0b3/src/datafog/pii_tools/
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-04-01 03:56:54.834307 datafog-2.4.0b3/src/datafog/pii_tools/PresidioEngine/
--rw-r--r--   0 sidmohan   (501) staff       (20)     6651 2024-04-01 01:47:25.000000 datafog-2.4.0b3/src/datafog/pii_tools/PresidioEngine/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     6226 2024-04-01 01:47:25.000000 datafog-2.4.0b3/src/datafog/pii_tools/PresidioEngine/analyzer.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-04-01 03:56:54.835229 datafog-2.4.0b3/src/datafog.egg-info/
--rw-r--r--   0 sidmohan   (501) staff       (20)     7749 2024-04-01 03:56:54.000000 datafog-2.4.0b3/src/datafog.egg-info/PKG-INFO
--rw-r--r--   0 sidmohan   (501) staff       (20)      392 2024-04-01 03:56:54.000000 datafog-2.4.0b3/src/datafog.egg-info/SOURCES.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)        1 2024-04-01 03:56:54.000000 datafog-2.4.0b3/src/datafog.egg-info/dependency_links.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)      103 2024-04-01 03:56:54.000000 datafog-2.4.0b3/src/datafog.egg-info/requires.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)        8 2024-04-01 03:56:54.000000 datafog-2.4.0b3/src/datafog.egg-info/top_level.txt
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-04-01 03:56:54.834905 datafog-2.4.0b3/tests/
--rw-r--r--   0 sidmohan   (501) staff       (20)     2762 2024-04-01 03:56:24.000000 datafog-2.4.0b3/tests/test_datafog.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     2839 2024-04-01 01:29:31.000000 datafog-2.4.0b3/tests/test_presidio.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-04-02 02:16:36.643102 datafog-2.4.0b4/
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1091 2024-03-28 17:43:37.000000 datafog-2.4.0b4/LICENSE
+-rw-r--r--   0 sidmohan   (501) staff       (20)     7749 2024-04-02 02:16:36.642817 datafog-2.4.0b4/PKG-INFO
+-rw-r--r--   0 sidmohan   (501) staff       (20)     6355 2024-03-28 17:43:37.000000 datafog-2.4.0b4/README.md
+-rw-r--r--   0 sidmohan   (501) staff       (20)       38 2024-04-02 02:16:36.643178 datafog-2.4.0b4/setup.cfg
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1712 2024-04-02 02:00:59.000000 datafog-2.4.0b4/setup.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-04-02 02:16:36.629112 datafog-2.4.0b4/src/
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-04-02 02:16:36.633524 datafog-2.4.0b4/src/datafog/
+-rw-r--r--   0 sidmohan   (501) staff       (20)       53 2024-03-28 17:43:37.000000 datafog-2.4.0b4/src/datafog/__about__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     4866 2024-04-02 02:15:41.000000 datafog-2.4.0b4/src/datafog/__init__.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-04-02 02:16:36.629381 datafog-2.4.0b4/src/datafog/pii_tools/
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-04-02 02:16:36.640915 datafog-2.4.0b4/src/datafog/pii_tools/PresidioEngine/
+-rw-r--r--   0 sidmohan   (501) staff       (20)     6651 2024-04-02 02:15:41.000000 datafog-2.4.0b4/src/datafog/pii_tools/PresidioEngine/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     6226 2024-04-02 02:15:41.000000 datafog-2.4.0b4/src/datafog/pii_tools/PresidioEngine/analyzer.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-04-02 02:16:36.642355 datafog-2.4.0b4/src/datafog.egg-info/
+-rw-r--r--   0 sidmohan   (501) staff       (20)     7749 2024-04-02 02:16:36.000000 datafog-2.4.0b4/src/datafog.egg-info/PKG-INFO
+-rw-r--r--   0 sidmohan   (501) staff       (20)      392 2024-04-02 02:16:36.000000 datafog-2.4.0b4/src/datafog.egg-info/SOURCES.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)        1 2024-04-02 02:16:36.000000 datafog-2.4.0b4/src/datafog.egg-info/dependency_links.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)      103 2024-04-02 02:16:36.000000 datafog-2.4.0b4/src/datafog.egg-info/requires.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)        8 2024-04-02 02:16:36.000000 datafog-2.4.0b4/src/datafog.egg-info/top_level.txt
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-04-02 02:16:36.641743 datafog-2.4.0b4/tests/
+-rw-r--r--   0 sidmohan   (501) staff       (20)     3505 2024-04-02 02:15:41.000000 datafog-2.4.0b4/tests/test_datafog.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     2711 2024-04-01 15:24:39.000000 datafog-2.4.0b4/tests/test_presidio.py
```

### Comparing `datafog-2.4.0b3/LICENSE` & `datafog-2.4.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `datafog-2.4.0b3/PKG-INFO` & `datafog-2.4.0b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datafog
-Version: 2.4.0b3
+Version: 2.4.0b4
 Summary: Scan, redact, and manage PII in your documents before they get uploaded to a Retrieval Augmented Generation (RAG) system.
 Home-page: https://datafog.ai
 Author: DataFog
 Author-email: hi@datafog.ai
 Maintainer: DataFog
 Maintainer-email: hi@datafog.ai
 License: MIT
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: datafog Version: 2.4.0b3 Summary: Scan, redact, and
+Metadata-Version: 2.1 Name: datafog Version: 2.4.0b4 Summary: Scan, redact, and
 manage PII in your documents before they get uploaded to a Retrieval Augmented
 Generation (RAG) system. Home-page: https://datafog.ai Author: DataFog Author-
 email: hi@datafog.ai Maintainer: DataFog Maintainer-email: hi@datafog.ai
 License: MIT Project-URL: Homepage, https://datafog.ai Project-URL:
 Documentation, https://docs.datafog.ai Project-URL: Discord, https://
 discord.gg/bzDth394R4 Project-URL: Twitter, https://twitter.com/datafoginc
 Project-URL: GitHub, https://github.com/datafog/datafog-python Keywords:
```

### Comparing `datafog-2.4.0b3/README.md` & `datafog-2.4.0b4/README.md`

 * *Files identical despite different names*

### Comparing `datafog-2.4.0b3/setup.py` & `datafog-2.4.0b4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read README for the long description
 with open("README.md", "r") as f:
     long_description = f.read()
 
 
 def __version__():
-    return "2.4.0b3"
+    return "2.4.0b4"
 
 
 project_urls = {
     "Homepage": "https://datafog.ai",
     "Documentation": "https://docs.datafog.ai",
     "Discord": "https://discord.gg/bzDth394R4",
     "Twitter": "https://twitter.com/datafoginc",
```

### Comparing `datafog-2.4.0b3/src/datafog/__init__.py` & `datafog-2.4.0b4/src/datafog/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # datafog-python/src/datafog/__init__.py
 import json
 import logging
 import tempfile
 from pathlib import Path
+from typing import List
 
 import pandas as pd
 import requests
 import spacy
 from unstructured.partition.auto import partition
-from unstructured.partition.auto import partition_pptx
 
 from .__about__ import __version__
 from .pii_tools import PresidioEngine
 
 logger = logging.getLogger(__name__).setLevel(logging.ERROR)
 
 __all__ = [
@@ -29,14 +29,15 @@
     personally identifiable information (PII) and applies specified privacy
     operations to protect sensitive data.
 
     Attributes:
         nlp (spacy.lang): Spacy language model for PII detection.
     """
 
+    # Maintaining support
     def __init__(self):
         """
         Initialize the DataFog instance.
 
         Loads the Spacy language model for PII detection.
         """
         self.nlp = spacy.load("en_spacy_pii_fast")
@@ -69,14 +70,31 @@
             text = ""
             for element in elements:
                 text += element.text + "\n"
             texts[uploaded_file_path.name] = text
 
         return texts
 
+    @staticmethod
+    def upload_files(uploaded_files: List[str]):
+        """
+        Process uploaded files.
+
+        Args:
+            uploaded_files (List[str]): A list of file paths uploaded by the user.
+
+        Returns:
+            Dict[str, str]: A dictionary containing the processed text for each uploaded file.
+        """
+        texts = {}
+        for uploaded_file in uploaded_files:
+            result = DataFog.upload_file(uploaded_file)
+            texts.update(result)
+        return texts
+
     def __call__(self, input_source, privacy_operation):
         """
         Process the input data and apply the specified privacy operation.
 
         Args:
             input_source (Union[str, pd.DataFrame]): The input data source.
                 Can be a URL, file path, or a string containing the data.
```

### Comparing `datafog-2.4.0b3/src/datafog/pii_tools/PresidioEngine/__init__.py` & `datafog-2.4.0b4/src/datafog/pii_tools/PresidioEngine/__init__.py`

 * *Files identical despite different names*

### Comparing `datafog-2.4.0b3/src/datafog/pii_tools/PresidioEngine/analyzer.py` & `datafog-2.4.0b4/src/datafog/pii_tools/PresidioEngine/analyzer.py`

 * *Files identical despite different names*

### Comparing `datafog-2.4.0b3/src/datafog.egg-info/PKG-INFO` & `datafog-2.4.0b4/src/datafog.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datafog
-Version: 2.4.0b3
+Version: 2.4.0b4
 Summary: Scan, redact, and manage PII in your documents before they get uploaded to a Retrieval Augmented Generation (RAG) system.
 Home-page: https://datafog.ai
 Author: DataFog
 Author-email: hi@datafog.ai
 Maintainer: DataFog
 Maintainer-email: hi@datafog.ai
 License: MIT
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: datafog Version: 2.4.0b3 Summary: Scan, redact, and
+Metadata-Version: 2.1 Name: datafog Version: 2.4.0b4 Summary: Scan, redact, and
 manage PII in your documents before they get uploaded to a Retrieval Augmented
 Generation (RAG) system. Home-page: https://datafog.ai Author: DataFog Author-
 email: hi@datafog.ai Maintainer: DataFog Maintainer-email: hi@datafog.ai
 License: MIT Project-URL: Homepage, https://datafog.ai Project-URL:
 Documentation, https://docs.datafog.ai Project-URL: Discord, https://
 discord.gg/bzDth394R4 Project-URL: Twitter, https://twitter.com/datafoginc
 Project-URL: GitHub, https://github.com/datafog/datafog-python Keywords:
```

### Comparing `datafog-2.4.0b3/tests/test_presidio.py` & `datafog-2.4.0b4/tests/test_presidio.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,85 +1,85 @@
-# import os
-# import sys
+import os
+import sys
 
-# import requests
+import requests
 
-# from datafog import PresidioEngine as presidio
+from datafog import PresidioEngine as presidio
 
-# sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
+sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
 
 
-# def test_piiscan_json_detection():
-#     # Assuming sample_file already contains the data you want to test
-#     sample_file = "tests/files/input_files/sample.json"
-
-#     # Read the contents of sample_file into original_value
-#     with open(sample_file, "r") as f:
-#         original_value = f.read()
-
-#     pii_detected = presidio.scan(original_value)
-
-#     # write pii_detected to a JSON file called output.json in the same directory as sample_file
-#     with open(
-#         "tests/files/output_files/output.json",
-#         "w",
-#     ) as f:
-#         for entity in pii_detected:
-#             f.write(entity.entity_type)
-#             f.write("\n")
-
-
-# def test_piiscan_csv_detection():
-#     # Assuming sample_file already contains the data you want to test
-#     sample_file = "tests/files/input_files/sample.csv"
-
-#     # Read the contents of sample_file into original_value
-#     with open(sample_file, "r") as f:
-#         original_value = f.read()
-
-#     pii_detected = presidio.scan(original_value)
-
-#     # write pii_detected to a JSON file called output.json in the same directory as sample_file
-#     with open(
-#         "tests/files/output_files/output.csv",
-#         "w",
-#     ) as f:
-#         for entity in pii_detected:
-#             f.write(entity.entity_type)
-#             f.write("\n")
-
-
-# def test_piiscan_txt_detection():
-#     # Assuming sample_file already contains the data you want to test
-#     sample_file = "tests/files/input_files/sample.txt"
-#     # Read the contents of sample_file into original_value
-#     with open(sample_file, "r") as f:
-#         original_value = f.read()
-
-#     pii_detected = presidio.scan(original_value)
-
-#     # write pii_detected to a JSON file called output.json in the same directory as sample_file
-#     with open(
-#         "tests/files/output_files/output.txt",
-#         "w",
-#     ) as f:
-#         for entity in pii_detected:
-#             f.write(entity.entity_type)
-#             f.write("\n")
-
-
-# def test_piiscan_url_detection():
-#     # Assuming sample_file already contains the data you want to test
-#     sample_url = "https://gist.githubusercontent.com/sidmohan0/1aa3ec38b4e6594d3c34b113f2e0962d/raw/42e57146197be0f85a5901cd1dcdd9ad15b31bab/sotu_2023.txt"
-
-#     response = requests.get(sample_url)
-#     original_value = response.text
-#     pii_detected = presidio.scan(original_value)
-
-#     # write pii_detected to a output.md in the same directory as sample_url
-#     with open(
-#         "tests/files/output_files/output.md",
-#         "w",
-#     ) as f:
-#         for entity in pii_detected:
-#             f.write(entity.entity_type)
-#             f.write("\n")
+def test_piiscan_json_detection():
+    # Assuming sample_file already contains the data you want to test
+    sample_file = "tests/files/input_files/sample.json"
+
+    # Read the contents of sample_file into original_value
+    with open(sample_file, "r") as f:
+        original_value = f.read()
+
+    pii_detected = presidio.scan(original_value)
+
+    # write pii_detected to a JSON file called output.json in the same directory as sample_file
+    with open(
+        "tests/files/output_files/output.json",
+        "w",
+    ) as f:
+        for entity in pii_detected:
+            f.write(entity.entity_type)
+            f.write("\n")
+
+
+def test_piiscan_csv_detection():
+    # Assuming sample_file already contains the data you want to test
+    sample_file = "tests/files/input_files/sample.csv"
+
+    # Read the contents of sample_file into original_value
+    with open(sample_file, "r") as f:
+        original_value = f.read()
+
+    pii_detected = presidio.scan(original_value)
+
+    # write pii_detected to a JSON file called output.json in the same directory as sample_file
+    with open(
+        "tests/files/output_files/output.csv",
+        "w",
+    ) as f:
+        for entity in pii_detected:
+            f.write(entity.entity_type)
+            f.write("\n")
+
+
+def test_piiscan_txt_detection():
+    # Assuming sample_file already contains the data you want to test
+    sample_file = "tests/files/input_files/sample.txt"
+    # Read the contents of sample_file into original_value
+    with open(sample_file, "r") as f:
+        original_value = f.read()
+
+    pii_detected = presidio.scan(original_value)
+
+    # write pii_detected to a JSON file called output.json in the same directory as sample_file
+    with open(
+        "tests/files/output_files/output.txt",
+        "w",
+    ) as f:
+        for entity in pii_detected:
+            f.write(entity.entity_type)
+            f.write("\n")
+
+
+def test_piiscan_url_detection():
+    # Assuming sample_file already contains the data you want to test
+    sample_url = "https://gist.githubusercontent.com/sidmohan0/1aa3ec38b4e6594d3c34b113f2e0962d/raw/42e57146197be0f85a5901cd1dcdd9ad15b31bab/sotu_2023.txt"
+
+    response = requests.get(sample_url)
+    original_value = response.text
+    pii_detected = presidio.scan(original_value)
+
+    # write pii_detected to a output.md in the same directory as sample_url
+    with open(
+        "tests/files/output_files/output.md",
+        "w",
+    ) as f:
+        for entity in pii_detected:
+            f.write(entity.entity_type)
+            f.write("\n")
```

