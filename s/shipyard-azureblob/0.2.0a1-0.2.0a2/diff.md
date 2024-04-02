# Comparing `tmp/shipyard_azureblob-0.2.0a1.tar.gz` & `tmp/shipyard_azureblob-0.2.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_azureblob-0.2.0a1.tar", max compression
+gzip compressed data, was "shipyard_azureblob-0.2.0a2.tar", max compression
```

## Comparing `shipyard_azureblob-0.2.0a1.tar` & `shipyard_azureblob-0.2.0a2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2023-07-24 19:47:59.855171 shipyard_azureblob-0.2.0a1/README.md
--rw-r--r--   0        0        0      544 2024-03-14 04:03:53.051926 shipyard_azureblob-0.2.0a1/pyproject.toml
--rw-r--r--   0        0        0       39 2023-05-12 18:48:21.823238 shipyard_azureblob-0.2.0a1/shipyard_azureblob/__init__.py
--rw-r--r--   0        0        0     9498 2024-03-13 15:28:19.436358 shipyard_azureblob-0.2.0a1/shipyard_azureblob/azureblob.py
--rw-r--r--   0        0        0        0 2024-02-05 20:53:35.431002 shipyard_azureblob-0.2.0a1/shipyard_azureblob/cli/__init__.py
--rw-r--r--   0        0        0      559 2024-03-13 14:10:54.001365 shipyard_azureblob-0.2.0a1/shipyard_azureblob/cli/authtest.py
--rw-r--r--   0        0        0     3914 2024-03-13 14:10:54.001969 shipyard_azureblob-0.2.0a1/shipyard_azureblob/cli/download.py
--rw-r--r--   0        0        0     3721 2024-03-13 14:10:54.002614 shipyard_azureblob-0.2.0a1/shipyard_azureblob/cli/move.py
--rw-r--r--   0        0        0     2277 2024-03-13 14:10:54.003134 shipyard_azureblob-0.2.0a1/shipyard_azureblob/cli/remove.py
--rw-r--r--   0        0        0     3838 2024-03-13 14:10:54.003660 shipyard_azureblob-0.2.0a1/shipyard_azureblob/cli/upload.py
--rw-r--r--   0        0        0     1644 2024-03-13 14:10:54.004302 shipyard_azureblob-0.2.0a1/shipyard_azureblob/exceptions.py
--rw-r--r--   0        0        0      673 1970-01-01 00:00:00.000000 shipyard_azureblob-0.2.0a1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-24 19:47:59.855171 shipyard_azureblob-0.2.0a2/README.md
+-rw-r--r--   0        0        0      544 2024-04-02 17:38:27.677828 shipyard_azureblob-0.2.0a2/pyproject.toml
+-rw-r--r--   0        0        0       39 2023-05-12 18:48:21.823238 shipyard_azureblob-0.2.0a2/shipyard_azureblob/__init__.py
+-rw-r--r--   0        0        0     9498 2024-04-01 13:13:53.708772 shipyard_azureblob-0.2.0a2/shipyard_azureblob/azureblob.py
+-rw-r--r--   0        0        0        0 2024-02-05 20:53:35.431002 shipyard_azureblob-0.2.0a2/shipyard_azureblob/cli/__init__.py
+-rw-r--r--   0        0        0      559 2024-03-14 04:10:25.267593 shipyard_azureblob-0.2.0a2/shipyard_azureblob/cli/authtest.py
+-rw-r--r--   0        0        0     3914 2024-03-21 15:28:03.027401 shipyard_azureblob-0.2.0a2/shipyard_azureblob/cli/download.py
+-rw-r--r--   0        0        0     3721 2024-03-14 04:10:25.268493 shipyard_azureblob-0.2.0a2/shipyard_azureblob/cli/move.py
+-rw-r--r--   0        0        0     2173 2024-04-02 17:37:53.386191 shipyard_azureblob-0.2.0a2/shipyard_azureblob/cli/remove.py
+-rw-r--r--   0        0        0     3838 2024-03-14 04:10:25.269404 shipyard_azureblob-0.2.0a2/shipyard_azureblob/cli/upload.py
+-rw-r--r--   0        0        0     1644 2024-03-14 04:10:25.269708 shipyard_azureblob-0.2.0a2/shipyard_azureblob/exceptions.py
+-rw-r--r--   0        0        0      673 1970-01-01 00:00:00.000000 shipyard_azureblob-0.2.0a2/PKG-INFO
```

### Comparing `shipyard_azureblob-0.2.0a1/pyproject.toml` & `shipyard_azureblob-0.2.0a2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shipyard-azureblob"
-version = "0.2.0a1"
+version = "0.2.0a2"
 description = "A local client to connect with and work with Azure Blob"
 authors = ["wrp801 <wespoulsen@gmail.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [{include = "shipyard_azureblob"}]
 
 [tool.poetry.dependencies]
```

### Comparing `shipyard_azureblob-0.2.0a1/shipyard_azureblob/azureblob.py` & `shipyard_azureblob-0.2.0a2/shipyard_azureblob/azureblob.py`

 * *Files identical despite different names*

### Comparing `shipyard_azureblob-0.2.0a1/shipyard_azureblob/cli/authtest.py` & `shipyard_azureblob-0.2.0a2/shipyard_azureblob/cli/authtest.py`

 * *Files identical despite different names*

### Comparing `shipyard_azureblob-0.2.0a1/shipyard_azureblob/cli/download.py` & `shipyard_azureblob-0.2.0a2/shipyard_azureblob/cli/download.py`

 * *Files identical despite different names*

### Comparing `shipyard_azureblob-0.2.0a1/shipyard_azureblob/cli/move.py` & `shipyard_azureblob-0.2.0a2/shipyard_azureblob/cli/move.py`

 * *Files identical despite different names*

### Comparing `shipyard_azureblob-0.2.0a1/shipyard_azureblob/cli/remove.py` & `shipyard_azureblob-0.2.0a2/shipyard_azureblob/cli/remove.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 import argparse
-import os
 import re
 import sys
 
-import shipyard_utils as shipyard
 from shipyard_bp_utils import files as shipyard
 from shipyard_templates import ShipyardLogger
 
 from shipyard_azureblob import AzureBlobClient
-from shipyard_azureblob.cli import exit_codes as ec
 
 logger = ShipyardLogger().get_logger()
 
 
 def get_args():
     parser = argparse.ArgumentParser()
     parser.add_argument("--container-name", dest="container_name", required=True)
@@ -31,33 +28,33 @@
         "--connection-string", dest="connection_string", default=None, required=True
     )
     return parser.parse_args()
 
 
 def main():
     args = get_args()
-    source_folder_name = shipyard.files.clean_folder_name(args.source_folder_name)
+    source_folder_name = shipyard.clean_folder_name(args.source_folder_name)
 
     client = AzureBlobClient(
         connection_string=args.connection_string, container_name=args.container_name
     )
     if args.source_file_name_match_type == "exact_match":
-        source_full_path = shipyard.files.combine_folder_and_file_name(
+        source_full_path = shipyard.combine_folder_and_file_name(
             folder_name=source_folder_name, file_name=args.source_file_name
         )
         client.remove(file_name=source_full_path)
 
     elif args.source_file_name_match_type == "regex_match":
         file_names = client.find_blob_file_names(prefix=source_folder_name)
         matching_file_names = shipyard.find_all_file_matches(
             file_names, re.compile(args.source_file_name)
         )
         if number_of_matches := len(matching_file_names) == 0:
             logger.error("No file matches found")
-            sys.exit(ec.EXIT_CODE_NO_MATCHES_FOUND)
+            sys.exit(client.EXIT_CODE_NO_MATCHES_FOUND)
 
         logger.info(f"{number_of_matches} files found. Preparing to delete...")
         for index, file_name in enumerate(matching_file_names, start=1):
             logger.info(f"Deleting file {index} of {number_of_matches}")
             client.remove(file_name=file_name)
```

### Comparing `shipyard_azureblob-0.2.0a1/shipyard_azureblob/cli/upload.py` & `shipyard_azureblob-0.2.0a2/shipyard_azureblob/cli/upload.py`

 * *Files identical despite different names*

### Comparing `shipyard_azureblob-0.2.0a1/shipyard_azureblob/exceptions.py` & `shipyard_azureblob-0.2.0a2/shipyard_azureblob/exceptions.py`

 * *Files identical despite different names*

### Comparing `shipyard_azureblob-0.2.0a1/PKG-INFO` & `shipyard_azureblob-0.2.0a2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipyard-azureblob
-Version: 0.2.0a1
+Version: 0.2.0a2
 Summary: A local client to connect with and work with Azure Blob
 License: Apache 2.0
 Author: wrp801
 Author-email: wespoulsen@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

