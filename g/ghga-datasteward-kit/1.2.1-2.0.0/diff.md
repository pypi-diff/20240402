# Comparing `tmp/ghga_datasteward_kit-1.2.1.tar.gz` & `tmp/ghga_datasteward_kit-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghga_datasteward_kit-1.2.1.tar", last modified: Tue Mar 12 11:04:05 2024, max compression
+gzip compressed data, was "ghga_datasteward_kit-2.0.0.tar", last modified: Tue Apr  2 08:25:26 2024, max compression
```

## Comparing `ghga_datasteward_kit-1.2.1.tar` & `ghga_datasteward_kit-2.0.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 11:04:05.836411 ghga_datasteward_kit-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11452 2024-03-12 11:03:59.000000 ghga_datasteward_kit-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10147 2024-03-12 11:04:05.836411 ghga_datasteward_kit-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9154 2024-03-12 11:03:59.000000 ghga_datasteward_kit-1.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-03-12 11:04:01.000000 ghga_datasteward_kit-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-12 11:04:05.836411 ghga_datasteward_kit-1.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 11:04:05.828411 ghga_datasteward_kit-1.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 11:04:05.832411 ghga_datasteward_kit-1.2.1/src/ghga_datasteward_kit/
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-03-12 11:04:01.000000 ghga_datasteward_kit-1.2.1/src/ghga_datasteward_kit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-03-12 11:04:01.000000 ghga_datasteward_kit-1.2.1/src/ghga_datasteward_kit/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6949 2024-03-12 11:04:01.000000 ghga_datasteward_kit-1.2.1/src/ghga_datasteward_kit/batch_s3_upload.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3316 2024-03-12 11:04:01.000000 ghga_datasteward_kit-1.2.1/src/ghga_datasteward_kit/catalog_accession_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 11:04:05.832411 ghga_datasteward_kit-1.2.1/src/ghga_datasteward_kit/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-03-12 11:04:01.000000 ghga_datasteward_kit-1.2.1/src/ghga_datasteward_kit/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-03-12 11:04:01.000000 ghga_datasteward_kit-1.2.1/src/ghga_datasteward_kit/cli/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-03-12 11:04:01.000000 ghga_datasteward_kit-1.2.1/src/ghga_datasteward_kit/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-03-12 11:04:01.000000 ghga_datasteward_kit-1.2.1/src/ghga_datasteward_kit/cli/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-03-12 11:04:01.000000 ghga_datasteward_kit-1.2.1/src/ghga_datasteward_kit/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-03-12 11:04:01.000000 ghga_datasteward_kit-1.2.1/src/ghga_datasteward_kit/file_deletion.py
--rw-r--r--   0 runner    (1001) docker     (127)     5866 2024-03-12 11:04:01.000000 ghga_datasteward_kit-1.2.1/src/ghga_datasteward_kit/file_ingest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-03-12 11:04:01.000000 ghga_datasteward_kit-1.2.1/src/ghga_datasteward_kit/loading.py
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-03-12 11:04:01.000000 ghga_datasteward_kit-1.2.1/src/ghga_datasteward_kit/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     8124 2024-03-12 11:04:01.000000 ghga_datasteward_kit-1.2.1/src/ghga_datasteward_kit/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     9295 2024-03-12 11:04:01.000000 ghga_datasteward_kit-1.2.1/src/ghga_datasteward_kit/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 11:04:05.832411 ghga_datasteward_kit-1.2.1/src/ghga_datasteward_kit/s3_upload/
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-03-12 11:04:01.000000 ghga_datasteward_kit-1.2.1/src/ghga_datasteward_kit/s3_upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-03-12 11:04:01.000000 ghga_datasteward_kit-1.2.1/src/ghga_datasteward_kit/s3_upload/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-03-12 11:04:01.000000 ghga_datasteward_kit-1.2.1/src/ghga_datasteward_kit/s3_upload/downloader.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9077 2024-03-12 11:04:01.000000 ghga_datasteward_kit-1.2.1/src/ghga_datasteward_kit/s3_upload/entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-03-12 11:04:01.000000 ghga_datasteward_kit-1.2.1/src/ghga_datasteward_kit/s3_upload/file_decryption.py
--rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-03-12 11:04:01.000000 ghga_datasteward_kit-1.2.1/src/ghga_datasteward_kit/s3_upload/file_encryption.py
--rw-r--r--   0 runner    (1001) docker     (127)     5999 2024-03-12 11:04:01.000000 ghga_datasteward_kit-1.2.1/src/ghga_datasteward_kit/s3_upload/uploader.py
--rw-r--r--   0 runner    (1001) docker     (127)     9463 2024-03-12 11:04:01.000000 ghga_datasteward_kit-1.2.1/src/ghga_datasteward_kit/s3_upload/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-03-12 11:04:01.000000 ghga_datasteward_kit-1.2.1/src/ghga_datasteward_kit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 11:04:05.836411 ghga_datasteward_kit-1.2.1/src/ghga_datasteward_kit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10147 2024-03-12 11:04:05.000000 ghga_datasteward_kit-1.2.1/src/ghga_datasteward_kit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-03-12 11:04:05.000000 ghga_datasteward_kit-1.2.1/src/ghga_datasteward_kit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 11:04:05.000000 ghga_datasteward_kit-1.2.1/src/ghga_datasteward_kit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-12 11:04:05.000000 ghga_datasteward_kit-1.2.1/src/ghga_datasteward_kit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-12 11:04:05.000000 ghga_datasteward_kit-1.2.1/src/ghga_datasteward_kit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-12 11:04:05.000000 ghga_datasteward_kit-1.2.1/src/ghga_datasteward_kit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 11:04:05.836411 ghga_datasteward_kit-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-03-12 11:04:01.000000 ghga_datasteward_kit-1.2.1/tests/test_file_deletion.py
--rw-r--r--   0 runner    (1001) docker     (127)     6663 2024-03-12 11:04:01.000000 ghga_datasteward_kit-1.2.1/tests/test_file_ingest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-03-12 11:04:01.000000 ghga_datasteward_kit-1.2.1/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-03-12 11:04:01.000000 ghga_datasteward_kit-1.2.1/tests/test_s3_upload.py
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-03-12 11:04:01.000000 ghga_datasteward_kit-1.2.1/tests/test_size_adjustment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:25:26.150563 ghga_datasteward_kit-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11452 2024-04-02 08:25:19.000000 ghga_datasteward_kit-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10149 2024-04-02 08:25:26.150563 ghga_datasteward_kit-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9154 2024-04-02 08:25:19.000000 ghga_datasteward_kit-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-04-02 08:25:21.000000 ghga_datasteward_kit-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 08:25:26.150563 ghga_datasteward_kit-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:25:26.142563 ghga_datasteward_kit-2.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:25:26.146563 ghga_datasteward_kit-2.0.0/src/ghga_datasteward_kit/
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-02 08:25:21.000000 ghga_datasteward_kit-2.0.0/src/ghga_datasteward_kit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-02 08:25:21.000000 ghga_datasteward_kit-2.0.0/src/ghga_datasteward_kit/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6949 2024-04-02 08:25:21.000000 ghga_datasteward_kit-2.0.0/src/ghga_datasteward_kit/batch_s3_upload.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3316 2024-04-02 08:25:21.000000 ghga_datasteward_kit-2.0.0/src/ghga_datasteward_kit/catalog_accession_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:25:26.146563 ghga_datasteward_kit-2.0.0/src/ghga_datasteward_kit/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-02 08:25:21.000000 ghga_datasteward_kit-2.0.0/src/ghga_datasteward_kit/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-04-02 08:25:21.000000 ghga_datasteward_kit-2.0.0/src/ghga_datasteward_kit/cli/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-04-02 08:25:21.000000 ghga_datasteward_kit-2.0.0/src/ghga_datasteward_kit/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-04-02 08:25:21.000000 ghga_datasteward_kit-2.0.0/src/ghga_datasteward_kit/cli/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-02 08:25:21.000000 ghga_datasteward_kit-2.0.0/src/ghga_datasteward_kit/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-02 08:25:21.000000 ghga_datasteward_kit-2.0.0/src/ghga_datasteward_kit/file_deletion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5866 2024-04-02 08:25:21.000000 ghga_datasteward_kit-2.0.0/src/ghga_datasteward_kit/file_ingest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-02 08:25:21.000000 ghga_datasteward_kit-2.0.0/src/ghga_datasteward_kit/loading.py
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-02 08:25:21.000000 ghga_datasteward_kit-2.0.0/src/ghga_datasteward_kit/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8125 2024-04-02 08:25:21.000000 ghga_datasteward_kit-2.0.0/src/ghga_datasteward_kit/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9295 2024-04-02 08:25:21.000000 ghga_datasteward_kit-2.0.0/src/ghga_datasteward_kit/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:25:26.150563 ghga_datasteward_kit-2.0.0/src/ghga_datasteward_kit/s3_upload/
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-02 08:25:21.000000 ghga_datasteward_kit-2.0.0/src/ghga_datasteward_kit/s3_upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-04-02 08:25:21.000000 ghga_datasteward_kit-2.0.0/src/ghga_datasteward_kit/s3_upload/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-04-02 08:25:21.000000 ghga_datasteward_kit-2.0.0/src/ghga_datasteward_kit/s3_upload/downloader.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9077 2024-04-02 08:25:21.000000 ghga_datasteward_kit-2.0.0/src/ghga_datasteward_kit/s3_upload/entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-04-02 08:25:21.000000 ghga_datasteward_kit-2.0.0/src/ghga_datasteward_kit/s3_upload/file_decryption.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-04-02 08:25:21.000000 ghga_datasteward_kit-2.0.0/src/ghga_datasteward_kit/s3_upload/file_encryption.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5999 2024-04-02 08:25:21.000000 ghga_datasteward_kit-2.0.0/src/ghga_datasteward_kit/s3_upload/uploader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9463 2024-04-02 08:25:21.000000 ghga_datasteward_kit-2.0.0/src/ghga_datasteward_kit/s3_upload/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-04-02 08:25:21.000000 ghga_datasteward_kit-2.0.0/src/ghga_datasteward_kit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:25:26.150563 ghga_datasteward_kit-2.0.0/src/ghga_datasteward_kit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10149 2024-04-02 08:25:26.000000 ghga_datasteward_kit-2.0.0/src/ghga_datasteward_kit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-02 08:25:26.000000 ghga_datasteward_kit-2.0.0/src/ghga_datasteward_kit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 08:25:26.000000 ghga_datasteward_kit-2.0.0/src/ghga_datasteward_kit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-02 08:25:26.000000 ghga_datasteward_kit-2.0.0/src/ghga_datasteward_kit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-02 08:25:26.000000 ghga_datasteward_kit-2.0.0/src/ghga_datasteward_kit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-02 08:25:26.000000 ghga_datasteward_kit-2.0.0/src/ghga_datasteward_kit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:25:26.150563 ghga_datasteward_kit-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-02 08:25:21.000000 ghga_datasteward_kit-2.0.0/tests/test_file_deletion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6663 2024-04-02 08:25:21.000000 ghga_datasteward_kit-2.0.0/tests/test_file_ingest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-04-02 08:25:21.000000 ghga_datasteward_kit-2.0.0/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-04-02 08:25:21.000000 ghga_datasteward_kit-2.0.0/tests/test_s3_upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-02 08:25:21.000000 ghga_datasteward_kit-2.0.0/tests/test_size_adjustment.py
```

### Comparing `ghga_datasteward_kit-1.2.1/LICENSE` & `ghga_datasteward_kit-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-1.2.1/PKG-INFO` & `ghga_datasteward_kit-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghga_datasteward_kit
-Version: 1.2.1
+Version: 2.0.0
 Summary: GHGA Data Steward Kit - A utils package for GHGA data stewards.
 Author-email: "German Human Genome Phenome Archive (GHGA)" <contact@ghga.de>
 License: Apache 2.0
 Project-URL: Repository, https://github.com/ghga-de/ghga-datasteward-kit
 Classifier: Development Status :: 1 - Planning
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.9
@@ -14,17 +14,17 @@
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: crypt4gh<2,>=1.6
-Requires-Dist: hexkit[s3]~=1.0.0
-Requires-Dist: ghga-transpiler~=1.4.0
-Requires-Dist: metldata~=1.1.0
+Requires-Dist: hexkit[s3]<3,>=2.1.1
+Requires-Dist: ghga-transpiler<3,>=2
+Requires-Dist: metldata~=1.2.1
 
 [![tests](https://github.com/ghga-de/ghga-datasteward-kit/actions/workflows/tests.yaml/badge.svg)](https://github.com/ghga-de/ghga-datasteward-kit/actions/workflows/tests.yaml)
 [![Coverage Status](https://coveralls.io/repos/github/ghga-de/ghga-datasteward-kit/badge.svg?branch=main)](https://coveralls.io/github/ghga-de/ghga-datasteward-kit?branch=main)
 
 # GHGA Data Steward Kit
 
 Utilities for data stewards interacting with GHGA infrastructure.
```

### Comparing `ghga_datasteward_kit-1.2.1/README.md` & `ghga_datasteward_kit-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-1.2.1/pyproject.toml` & `ghga_datasteward_kit-2.0.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -18,21 +18,21 @@
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: Apache Software License",
     "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
     "Topic :: Software Development :: Libraries",
     "Intended Audience :: Developers",
 ]
 name = "ghga_datasteward_kit"
-version = "1.2.1"
+version = "2.0.0"
 description = "GHGA Data Steward Kit - A utils package for GHGA data stewards."
 dependencies = [
     "crypt4gh >=1.6, <2",
-    "hexkit[s3]~=1.0.0",
-    "ghga-transpiler~=1.4.0",
-    "metldata~=1.1.0",
+    "hexkit[s3] >=2.1.1, <3",
+    "ghga-transpiler >=2, <3",
+    "metldata~=1.2.1",
 ]
 
 [project.license]
 text = "Apache 2.0"
 
 [project.urls]
 Repository = "https://github.com/ghga-de/ghga-datasteward-kit"
```

### Comparing `ghga_datasteward_kit-1.2.1/src/ghga_datasteward_kit/__init__.py` & `ghga_datasteward_kit-2.0.0/src/ghga_datasteward_kit/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-1.2.1/src/ghga_datasteward_kit/__main__.py` & `ghga_datasteward_kit-2.0.0/src/ghga_datasteward_kit/__main__.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-1.2.1/src/ghga_datasteward_kit/batch_s3_upload.py` & `ghga_datasteward_kit-2.0.0/src/ghga_datasteward_kit/batch_s3_upload.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-1.2.1/src/ghga_datasteward_kit/catalog_accession_generator.py` & `ghga_datasteward_kit-2.0.0/src/ghga_datasteward_kit/catalog_accession_generator.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-1.2.1/src/ghga_datasteward_kit/cli/__init__.py` & `ghga_datasteward_kit-2.0.0/src/ghga_datasteward_kit/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-1.2.1/src/ghga_datasteward_kit/cli/file.py` & `ghga_datasteward_kit-2.0.0/src/ghga_datasteward_kit/cli/file.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-1.2.1/src/ghga_datasteward_kit/cli/main.py` & `ghga_datasteward_kit-2.0.0/src/ghga_datasteward_kit/cli/main.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-1.2.1/src/ghga_datasteward_kit/cli/metadata.py` & `ghga_datasteward_kit-2.0.0/src/ghga_datasteward_kit/cli/metadata.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-1.2.1/src/ghga_datasteward_kit/config.py` & `ghga_datasteward_kit-2.0.0/src/ghga_datasteward_kit/config.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-1.2.1/src/ghga_datasteward_kit/file_deletion.py` & `ghga_datasteward_kit-2.0.0/src/ghga_datasteward_kit/file_deletion.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-1.2.1/src/ghga_datasteward_kit/file_ingest.py` & `ghga_datasteward_kit-2.0.0/src/ghga_datasteward_kit/file_ingest.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-1.2.1/src/ghga_datasteward_kit/loading.py` & `ghga_datasteward_kit-2.0.0/src/ghga_datasteward_kit/loading.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-1.2.1/src/ghga_datasteward_kit/main.py` & `ghga_datasteward_kit-2.0.0/src/ghga_datasteward_kit/main.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-1.2.1/src/ghga_datasteward_kit/metadata.py` & `ghga_datasteward_kit-2.0.0/src/ghga_datasteward_kit/metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -210,15 +210,15 @@
 
 def transform_metadata(*, config: MetadataConfig) -> None:
     """Run transformation workflow on submitted metadata to produce artifacts."""
     asyncio.run(
         run_workflow_on_all_source_events(
             event_config=config,
             workflow_definition=GHGA_ARCHIVE_WORKFLOW,
-            worflow_config=config.workflow_config,
+            workflow_config=config.workflow_config,
             original_model=config.metadata_model,
         )
     )
 
 
 def transform_metadata_from_path(*, config_path: Path) -> None:
     """Load config from path and run transformation workflow on submitted
```

### Comparing `ghga_datasteward_kit-1.2.1/src/ghga_datasteward_kit/models.py` & `ghga_datasteward_kit-2.0.0/src/ghga_datasteward_kit/models.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-1.2.1/src/ghga_datasteward_kit/s3_upload/__init__.py` & `ghga_datasteward_kit-2.0.0/src/ghga_datasteward_kit/s3_upload/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-1.2.1/src/ghga_datasteward_kit/s3_upload/config.py` & `ghga_datasteward_kit-2.0.0/src/ghga_datasteward_kit/s3_upload/config.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-1.2.1/src/ghga_datasteward_kit/s3_upload/downloader.py` & `ghga_datasteward_kit-2.0.0/src/ghga_datasteward_kit/s3_upload/downloader.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-1.2.1/src/ghga_datasteward_kit/s3_upload/entrypoint.py` & `ghga_datasteward_kit-2.0.0/src/ghga_datasteward_kit/s3_upload/entrypoint.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-1.2.1/src/ghga_datasteward_kit/s3_upload/file_decryption.py` & `ghga_datasteward_kit-2.0.0/src/ghga_datasteward_kit/s3_upload/file_decryption.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-1.2.1/src/ghga_datasteward_kit/s3_upload/file_encryption.py` & `ghga_datasteward_kit-2.0.0/src/ghga_datasteward_kit/s3_upload/file_encryption.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-1.2.1/src/ghga_datasteward_kit/s3_upload/uploader.py` & `ghga_datasteward_kit-2.0.0/src/ghga_datasteward_kit/s3_upload/uploader.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-1.2.1/src/ghga_datasteward_kit/s3_upload/utils.py` & `ghga_datasteward_kit-2.0.0/src/ghga_datasteward_kit/s3_upload/utils.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-1.2.1/src/ghga_datasteward_kit/utils.py` & `ghga_datasteward_kit-2.0.0/src/ghga_datasteward_kit/utils.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-1.2.1/src/ghga_datasteward_kit.egg-info/PKG-INFO` & `ghga_datasteward_kit-2.0.0/src/ghga_datasteward_kit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghga_datasteward_kit
-Version: 1.2.1
+Version: 2.0.0
 Summary: GHGA Data Steward Kit - A utils package for GHGA data stewards.
 Author-email: "German Human Genome Phenome Archive (GHGA)" <contact@ghga.de>
 License: Apache 2.0
 Project-URL: Repository, https://github.com/ghga-de/ghga-datasteward-kit
 Classifier: Development Status :: 1 - Planning
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.9
@@ -14,17 +14,17 @@
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: crypt4gh<2,>=1.6
-Requires-Dist: hexkit[s3]~=1.0.0
-Requires-Dist: ghga-transpiler~=1.4.0
-Requires-Dist: metldata~=1.1.0
+Requires-Dist: hexkit[s3]<3,>=2.1.1
+Requires-Dist: ghga-transpiler<3,>=2
+Requires-Dist: metldata~=1.2.1
 
 [![tests](https://github.com/ghga-de/ghga-datasteward-kit/actions/workflows/tests.yaml/badge.svg)](https://github.com/ghga-de/ghga-datasteward-kit/actions/workflows/tests.yaml)
 [![Coverage Status](https://coveralls.io/repos/github/ghga-de/ghga-datasteward-kit/badge.svg?branch=main)](https://coveralls.io/github/ghga-de/ghga-datasteward-kit?branch=main)
 
 # GHGA Data Steward Kit
 
 Utilities for data stewards interacting with GHGA infrastructure.
```

### Comparing `ghga_datasteward_kit-1.2.1/src/ghga_datasteward_kit.egg-info/SOURCES.txt` & `ghga_datasteward_kit-2.0.0/src/ghga_datasteward_kit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-1.2.1/tests/test_file_deletion.py` & `ghga_datasteward_kit-2.0.0/tests/test_file_deletion.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-1.2.1/tests/test_file_ingest.py` & `ghga_datasteward_kit-2.0.0/tests/test_file_ingest.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-1.2.1/tests/test_metadata.py` & `ghga_datasteward_kit-2.0.0/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-1.2.1/tests/test_s3_upload.py` & `ghga_datasteward_kit-2.0.0/tests/test_s3_upload.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-1.2.1/tests/test_size_adjustment.py` & `ghga_datasteward_kit-2.0.0/tests/test_size_adjustment.py`

 * *Files identical despite different names*

