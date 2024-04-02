# Comparing `tmp/shipyard_dropbox-0.1.1a0.tar.gz` & `tmp/shipyard_dropbox-0.1.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_dropbox-0.1.1a0.tar", max compression
+gzip compressed data, was "shipyard_dropbox-0.1.1a1.tar", max compression
```

## Comparing `shipyard_dropbox-0.1.1a0.tar` & `shipyard_dropbox-0.1.1a1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2023-07-24 19:47:59.858331 shipyard_dropbox-0.1.1a0/README.md
--rw-r--r--   0        0        0      548 2024-04-02 14:47:13.033412 shipyard_dropbox-0.1.1a0/pyproject.toml
--rw-r--r--   0        0        0       35 2023-08-09 00:44:22.123795 shipyard_dropbox-0.1.1a0/shipyard_dropbox/__init__.py
--rw-r--r--   0        0        0        0 2024-02-05 20:53:35.434779 shipyard_dropbox-0.1.1a0/shipyard_dropbox/cli/__init__.py
--rw-r--r--   0        0        0      451 2024-04-01 15:54:40.969128 shipyard_dropbox-0.1.1a0/shipyard_dropbox/cli/authtest.py
--rw-r--r--   0        0        0     5667 2024-04-01 15:54:40.969657 shipyard_dropbox-0.1.1a0/shipyard_dropbox/cli/download.py
--rw-r--r--   0        0        0     7066 2024-04-01 15:54:40.970111 shipyard_dropbox-0.1.1a0/shipyard_dropbox/cli/upload.py
--rw-r--r--   0        0        0      504 2024-04-02 14:47:07.820385 shipyard_dropbox-0.1.1a0/shipyard_dropbox/dropbox.py
--rw-r--r--   0        0        0      651 1970-01-01 00:00:00.000000 shipyard_dropbox-0.1.1a0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-24 19:47:59.858331 shipyard_dropbox-0.1.1a1/README.md
+-rw-r--r--   0        0        0      548 2024-04-02 14:57:45.438276 shipyard_dropbox-0.1.1a1/pyproject.toml
+-rw-r--r--   0        0        0       35 2023-08-09 00:44:22.123795 shipyard_dropbox-0.1.1a1/shipyard_dropbox/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-05 20:53:35.434779 shipyard_dropbox-0.1.1a1/shipyard_dropbox/cli/__init__.py
+-rw-r--r--   0        0        0      451 2024-04-01 15:54:40.969128 shipyard_dropbox-0.1.1a1/shipyard_dropbox/cli/authtest.py
+-rw-r--r--   0        0        0     5656 2024-04-02 14:57:34.965329 shipyard_dropbox-0.1.1a1/shipyard_dropbox/cli/download.py
+-rw-r--r--   0        0        0     7066 2024-04-01 15:54:40.970111 shipyard_dropbox-0.1.1a1/shipyard_dropbox/cli/upload.py
+-rw-r--r--   0        0        0      504 2024-04-02 14:47:07.820385 shipyard_dropbox-0.1.1a1/shipyard_dropbox/dropbox.py
+-rw-r--r--   0        0        0      651 1970-01-01 00:00:00.000000 shipyard_dropbox-0.1.1a1/PKG-INFO
```

### Comparing `shipyard_dropbox-0.1.1a0/pyproject.toml` & `shipyard_dropbox-0.1.1a1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shipyard-dropbox"
-version = "0.1.1a0"
+version = "0.1.1a1"
 description = "A local client to connect and work with Dropox"
 authors = ["wrp801 <wespoulsen@gmail.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [{ include = "shipyard_dropbox" }]
 
 [tool.poetry.dependencies]
```

### Comparing `shipyard_dropbox-0.1.1a0/shipyard_dropbox/cli/download.py` & `shipyard_dropbox-0.1.1a1/shipyard_dropbox/cli/download.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
 
         destination_folder_name = shipyard.clean_folder_name(
             args.destination_folder_name
         )
         if destination_folder_name:
             shipyard.create_folder_if_dne(destination_folder_name)
 
-        client = Dropbox(access_key=access_key)
+        client = Dropbox(access_key)
         if args.source_file_name_match_type == "exact_match":
             destination_name = shipyard.determine_destination_full_path(
                 destination_folder_name=destination_folder_name,
                 destination_file_name=args.destination_file_name,
                 source_full_path=source_full_path,
             )
```

### Comparing `shipyard_dropbox-0.1.1a0/shipyard_dropbox/cli/upload.py` & `shipyard_dropbox-0.1.1a1/shipyard_dropbox/cli/upload.py`

 * *Files identical despite different names*

### Comparing `shipyard_dropbox-0.1.1a0/PKG-INFO` & `shipyard_dropbox-0.1.1a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipyard-dropbox
-Version: 0.1.1a0
+Version: 0.1.1a1
 Summary: A local client to connect and work with Dropox
 License: Apache 2.0
 Author: wrp801
 Author-email: wespoulsen@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

