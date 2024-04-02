# Comparing `tmp/layernext-beta-3.1.1b6.tar.gz` & `tmp/layernext-beta-3.2.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "layernext-beta-3.1.1b6.tar", last modified: Wed Mar  6 10:41:37 2024, max compression
+gzip compressed data, was "layernext-beta-3.2.0b0.tar", last modified: Tue Apr  2 03:48:15 2024, max compression
```

## Comparing `layernext-beta-3.1.1b6.tar` & `layernext-beta-3.2.0b0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 chathushka   (501) staff       (20)        0 2024-03-06 10:41:37.505197 layernext-beta-3.1.1b6/
--rw-r--r--   0 chathushka   (501) staff       (20)     1073 2023-09-11 10:46:59.000000 layernext-beta-3.1.1b6/LICENSE
--rw-r--r--   0 chathushka   (501) staff       (20)     1126 2024-03-06 10:41:37.504824 layernext-beta-3.1.1b6/PKG-INFO
--rw-r--r--   0 chathushka   (501) staff       (20)      352 2023-10-18 12:39:57.000000 layernext-beta-3.1.1b6/README.md
-drwxr-xr-x   0 chathushka   (501) staff       (20)        0 2024-03-06 10:41:37.492142 layernext-beta-3.1.1b6/layernext/
--rw-r--r--   0 chathushka   (501) staff       (20)   123028 2024-03-06 10:40:45.000000 layernext-beta-3.1.1b6/layernext/__init__.py
-drwxr-xr-x   0 chathushka   (501) staff       (20)        0 2024-03-06 10:41:37.493721 layernext-beta-3.1.1b6/layernext/automatic_analysis/
--rw-r--r--   0 chathushka   (501) staff       (20)     8488 2024-02-28 06:35:15.000000 layernext-beta-3.1.1b6/layernext/automatic_analysis/__init__.py
--rw-r--r--   0 chathushka   (501) staff       (20)     3902 2024-02-28 06:35:15.000000 layernext-beta-3.1.1b6/layernext/automatic_analysis/automatic_analysis.py
--rw-r--r--   0 chathushka   (501) staff       (20)     7539 2024-02-28 06:35:15.000000 layernext-beta-3.1.1b6/layernext/automatic_analysis/automatic_analysis_interface.py
--rw-r--r--   0 chathushka   (501) staff       (20)    19710 2024-02-28 06:35:15.000000 layernext-beta-3.1.1b6/layernext/automatic_analysis/status_check_autoannotate_project.py
--rw-r--r--   0 chathushka   (501) staff       (20)     4927 2024-02-28 06:35:15.000000 layernext-beta-3.1.1b6/layernext/automatic_analysis/support.py
-drwxr-xr-x   0 chathushka   (501) staff       (20)        0 2024-03-06 10:41:37.500029 layernext-beta-3.1.1b6/layernext/datalake/
--rw-r--r--   0 chathushka   (501) staff       (20)    23426 2024-03-03 13:13:07.000000 layernext-beta-3.1.1b6/layernext/datalake/__init__.py
--rw-r--r--   0 chathushka   (501) staff       (20)    16752 2024-02-28 06:35:15.000000 layernext-beta-3.1.1b6/layernext/datalake/annotation.py
--rw-r--r--   0 chathushka   (501) staff       (20)      868 2024-02-28 06:35:15.000000 layernext-beta-3.1.1b6/layernext/datalake/aws_s3_client.py
--rw-r--r--   0 chathushka   (501) staff       (20)      964 2024-02-28 06:35:15.000000 layernext-beta-3.1.1b6/layernext/datalake/azure_client.py
--rw-r--r--   0 chathushka   (501) staff       (20)     2307 2024-02-28 06:35:15.000000 layernext-beta-3.1.1b6/layernext/datalake/constants.py
--rw-r--r--   0 chathushka   (501) staff       (20)    93042 2024-03-03 12:22:19.000000 layernext-beta-3.1.1b6/layernext/datalake/datalakeinterface.py
--rw-r--r--   0 chathushka   (501) staff       (20)        0 2023-09-11 10:46:59.000000 layernext-beta-3.1.1b6/layernext/datalake/dataset.py
--rw-r--r--   0 chathushka   (501) staff       (20)      470 2024-02-28 06:35:15.000000 layernext-beta-3.1.1b6/layernext/datalake/file_trash.py
--rw-r--r--   0 chathushka   (501) staff       (20)    12275 2024-02-28 06:35:15.000000 layernext-beta-3.1.1b6/layernext/datalake/file_upload.py
--rw-r--r--   0 chathushka   (501) staff       (20)      879 2024-02-28 06:35:15.000000 layernext-beta-3.1.1b6/layernext/datalake/gcs_client.py
--rw-r--r--   0 chathushka   (501) staff       (20)     1642 2024-02-28 06:35:15.000000 layernext-beta-3.1.1b6/layernext/datalake/ground_truth.py
--rw-r--r--   0 chathushka   (501) staff       (20)     1539 2024-02-28 06:35:15.000000 layernext-beta-3.1.1b6/layernext/datalake/keys.py
--rw-r--r--   0 chathushka   (501) staff       (20)     7555 2024-02-28 06:35:15.000000 layernext-beta-3.1.1b6/layernext/datalake/label.py
--rw-r--r--   0 chathushka   (501) staff       (20)     1283 2024-02-28 06:35:15.000000 layernext-beta-3.1.1b6/layernext/datalake/logger.py
--rw-r--r--   0 chathushka   (501) staff       (20)     6659 2024-02-28 06:35:15.000000 layernext-beta-3.1.1b6/layernext/datalake/metadata.py
--rw-r--r--   0 chathushka   (501) staff       (20)     1136 2024-02-28 06:35:15.000000 layernext-beta-3.1.1b6/layernext/datalake/model_run.py
--rw-r--r--   0 chathushka   (501) staff       (20)     1166 2024-02-28 06:35:15.000000 layernext-beta-3.1.1b6/layernext/datalake/mongo_json_encoder.py
--rw-r--r--   0 chathushka   (501) staff       (20)     1390 2024-02-28 06:35:15.000000 layernext-beta-3.1.1b6/layernext/datalake/query.py
--rw-r--r--   0 chathushka   (501) staff       (20)      261 2024-02-28 06:35:15.000000 layernext-beta-3.1.1b6/layernext/datalake/storage_client.py
--rw-r--r--   0 chathushka   (501) staff       (20)     2691 2024-02-28 06:35:15.000000 layernext-beta-3.1.1b6/layernext/datalake/storage_interface.py
--rw-r--r--   0 chathushka   (501) staff       (20)     8733 2024-02-28 06:35:15.000000 layernext-beta-3.1.1b6/layernext/datalake/storage_upload.py
-drwxr-xr-x   0 chathushka   (501) staff       (20)        0 2024-03-06 10:41:37.501658 layernext-beta-3.1.1b6/layernext/dataset/
--rw-r--r--   0 chathushka   (501) staff       (20)     3305 2024-02-28 06:35:15.000000 layernext-beta-3.1.1b6/layernext/dataset/__init__.py
--rw-r--r--   0 chathushka   (501) staff       (20)     4561 2024-02-28 06:35:15.000000 layernext-beta-3.1.1b6/layernext/dataset/dataset.py
--rw-r--r--   0 chathushka   (501) staff       (20)     9171 2024-02-28 06:35:15.000000 layernext-beta-3.1.1b6/layernext/dataset/datasetinterface.py
--rw-r--r--   0 chathushka   (501) staff       (20)      431 2024-02-28 06:35:15.000000 layernext-beta-3.1.1b6/layernext/dataset/logger.py
--rw-r--r--   0 chathushka   (501) staff       (20)    23610 2024-02-28 06:35:15.000000 layernext-beta-3.1.1b6/layernext/dataset/sync.py
-drwxr-xr-x   0 chathushka   (501) staff       (20)        0 2024-03-06 10:41:37.502524 layernext-beta-3.1.1b6/layernext/studio/
--rw-r--r--   0 chathushka   (501) staff       (20)     3661 2024-02-28 06:35:15.000000 layernext-beta-3.1.1b6/layernext/studio/__init__.py
--rw-r--r--   0 chathushka   (501) staff       (20)      431 2024-02-28 06:35:15.000000 layernext-beta-3.1.1b6/layernext/studio/logger.py
--rw-r--r--   0 chathushka   (501) staff       (20)     3860 2024-02-28 06:35:15.000000 layernext-beta-3.1.1b6/layernext/studio/project.py
--rw-r--r--   0 chathushka   (501) staff       (20)    13127 2024-02-28 06:35:15.000000 layernext-beta-3.1.1b6/layernext/studio/studiointerface.py
-drwxr-xr-x   0 chathushka   (501) staff       (20)        0 2024-03-06 10:41:37.504340 layernext-beta-3.1.1b6/layernext_beta.egg-info/
--rw-r--r--   0 chathushka   (501) staff       (20)     1126 2024-03-06 10:41:37.000000 layernext-beta-3.1.1b6/layernext_beta.egg-info/PKG-INFO
--rw-r--r--   0 chathushka   (501) staff       (20)     1487 2024-03-06 10:41:37.000000 layernext-beta-3.1.1b6/layernext_beta.egg-info/SOURCES.txt
--rw-r--r--   0 chathushka   (501) staff       (20)        1 2024-03-06 10:41:37.000000 layernext-beta-3.1.1b6/layernext_beta.egg-info/dependency_links.txt
--rw-r--r--   0 chathushka   (501) staff       (20)       78 2024-03-06 10:41:37.000000 layernext-beta-3.1.1b6/layernext_beta.egg-info/requires.txt
--rw-r--r--   0 chathushka   (501) staff       (20)       10 2024-03-06 10:41:37.000000 layernext-beta-3.1.1b6/layernext_beta.egg-info/top_level.txt
--rw-r--r--   0 chathushka   (501) staff       (20)       38 2024-03-06 10:41:37.505293 layernext-beta-3.1.1b6/setup.cfg
--rw-r--r--   0 chathushka   (501) staff       (20)     1950 2024-02-28 06:35:15.000000 layernext-beta-3.1.1b6/setup.py
-drwxr-xr-x   0 chathushka   (501) staff       (20)        0 2024-03-06 10:41:37.503938 layernext-beta-3.1.1b6/tests/
--rw-r--r--   0 chathushka   (501) staff       (20)     1043 2023-09-11 10:46:59.000000 layernext-beta-3.1.1b6/tests/test_cli.py
+drwxr-xr-x   0 chathushka   (501) staff       (20)        0 2024-04-02 03:48:15.388146 layernext-beta-3.2.0b0/
+-rw-r--r--   0 chathushka   (501) staff       (20)     1073 2023-09-11 10:46:59.000000 layernext-beta-3.2.0b0/LICENSE
+-rw-r--r--   0 chathushka   (501) staff       (20)     1126 2024-04-02 03:48:15.387676 layernext-beta-3.2.0b0/PKG-INFO
+-rw-r--r--   0 chathushka   (501) staff       (20)      352 2023-10-18 12:39:57.000000 layernext-beta-3.2.0b0/README.md
+drwxr-xr-x   0 chathushka   (501) staff       (20)        0 2024-04-02 03:48:15.365575 layernext-beta-3.2.0b0/layernext/
+-rw-r--r--   0 chathushka   (501) staff       (20)   124538 2024-04-02 03:47:32.000000 layernext-beta-3.2.0b0/layernext/__init__.py
+drwxr-xr-x   0 chathushka   (501) staff       (20)        0 2024-04-02 03:48:15.368327 layernext-beta-3.2.0b0/layernext/automatic_analysis/
+-rw-r--r--   0 chathushka   (501) staff       (20)     8488 2024-02-28 06:35:15.000000 layernext-beta-3.2.0b0/layernext/automatic_analysis/__init__.py
+-rw-r--r--   0 chathushka   (501) staff       (20)     3902 2024-02-28 06:35:15.000000 layernext-beta-3.2.0b0/layernext/automatic_analysis/automatic_analysis.py
+-rw-r--r--   0 chathushka   (501) staff       (20)     7539 2024-02-28 06:35:15.000000 layernext-beta-3.2.0b0/layernext/automatic_analysis/automatic_analysis_interface.py
+-rw-r--r--   0 chathushka   (501) staff       (20)    19710 2024-02-28 06:35:15.000000 layernext-beta-3.2.0b0/layernext/automatic_analysis/status_check_autoannotate_project.py
+-rw-r--r--   0 chathushka   (501) staff       (20)     4927 2024-02-28 06:35:15.000000 layernext-beta-3.2.0b0/layernext/automatic_analysis/support.py
+drwxr-xr-x   0 chathushka   (501) staff       (20)        0 2024-04-02 03:48:15.380866 layernext-beta-3.2.0b0/layernext/datalake/
+-rw-r--r--   0 chathushka   (501) staff       (20)    23794 2024-04-02 03:46:31.000000 layernext-beta-3.2.0b0/layernext/datalake/__init__.py
+-rw-r--r--   0 chathushka   (501) staff       (20)    16752 2024-02-28 06:35:15.000000 layernext-beta-3.2.0b0/layernext/datalake/annotation.py
+-rw-r--r--   0 chathushka   (501) staff       (20)      868 2024-02-28 06:35:15.000000 layernext-beta-3.2.0b0/layernext/datalake/aws_s3_client.py
+-rw-r--r--   0 chathushka   (501) staff       (20)      964 2024-02-28 06:35:15.000000 layernext-beta-3.2.0b0/layernext/datalake/azure_client.py
+-rw-r--r--   0 chathushka   (501) staff       (20)     2307 2024-02-28 06:35:15.000000 layernext-beta-3.2.0b0/layernext/datalake/constants.py
+-rw-r--r--   0 chathushka   (501) staff       (20)    93524 2024-04-02 03:46:31.000000 layernext-beta-3.2.0b0/layernext/datalake/datalakeinterface.py
+-rw-r--r--   0 chathushka   (501) staff       (20)        0 2023-09-11 10:46:59.000000 layernext-beta-3.2.0b0/layernext/datalake/dataset.py
+-rw-r--r--   0 chathushka   (501) staff       (20)      470 2024-02-28 06:35:15.000000 layernext-beta-3.2.0b0/layernext/datalake/file_trash.py
+-rw-r--r--   0 chathushka   (501) staff       (20)    12275 2024-02-28 06:35:15.000000 layernext-beta-3.2.0b0/layernext/datalake/file_upload.py
+-rw-r--r--   0 chathushka   (501) staff       (20)      879 2024-02-28 06:35:15.000000 layernext-beta-3.2.0b0/layernext/datalake/gcs_client.py
+-rw-r--r--   0 chathushka   (501) staff       (20)     1642 2024-02-28 06:35:15.000000 layernext-beta-3.2.0b0/layernext/datalake/ground_truth.py
+-rw-r--r--   0 chathushka   (501) staff       (20)     1539 2024-02-28 06:35:15.000000 layernext-beta-3.2.0b0/layernext/datalake/keys.py
+-rw-r--r--   0 chathushka   (501) staff       (20)     7555 2024-02-28 06:35:15.000000 layernext-beta-3.2.0b0/layernext/datalake/label.py
+-rw-r--r--   0 chathushka   (501) staff       (20)     1283 2024-02-28 06:35:15.000000 layernext-beta-3.2.0b0/layernext/datalake/logger.py
+-rw-r--r--   0 chathushka   (501) staff       (20)     6659 2024-02-28 06:35:15.000000 layernext-beta-3.2.0b0/layernext/datalake/metadata.py
+-rw-r--r--   0 chathushka   (501) staff       (20)     1136 2024-02-28 06:35:15.000000 layernext-beta-3.2.0b0/layernext/datalake/model_run.py
+-rw-r--r--   0 chathushka   (501) staff       (20)     1166 2024-02-28 06:35:15.000000 layernext-beta-3.2.0b0/layernext/datalake/mongo_json_encoder.py
+-rw-r--r--   0 chathushka   (501) staff       (20)     1390 2024-02-28 06:35:15.000000 layernext-beta-3.2.0b0/layernext/datalake/query.py
+-rw-r--r--   0 chathushka   (501) staff       (20)      261 2024-02-28 06:35:15.000000 layernext-beta-3.2.0b0/layernext/datalake/storage_client.py
+-rw-r--r--   0 chathushka   (501) staff       (20)     2691 2024-02-28 06:35:15.000000 layernext-beta-3.2.0b0/layernext/datalake/storage_interface.py
+-rw-r--r--   0 chathushka   (501) staff       (20)     8733 2024-02-28 06:35:15.000000 layernext-beta-3.2.0b0/layernext/datalake/storage_upload.py
+drwxr-xr-x   0 chathushka   (501) staff       (20)        0 2024-04-02 03:48:15.383106 layernext-beta-3.2.0b0/layernext/dataset/
+-rw-r--r--   0 chathushka   (501) staff       (20)     3305 2024-02-28 06:35:15.000000 layernext-beta-3.2.0b0/layernext/dataset/__init__.py
+-rw-r--r--   0 chathushka   (501) staff       (20)     4561 2024-02-28 06:35:15.000000 layernext-beta-3.2.0b0/layernext/dataset/dataset.py
+-rw-r--r--   0 chathushka   (501) staff       (20)     9171 2024-02-28 06:35:15.000000 layernext-beta-3.2.0b0/layernext/dataset/datasetinterface.py
+-rw-r--r--   0 chathushka   (501) staff       (20)      431 2024-02-28 06:35:15.000000 layernext-beta-3.2.0b0/layernext/dataset/logger.py
+-rw-r--r--   0 chathushka   (501) staff       (20)    23610 2024-02-28 06:35:15.000000 layernext-beta-3.2.0b0/layernext/dataset/sync.py
+drwxr-xr-x   0 chathushka   (501) staff       (20)        0 2024-04-02 03:48:15.384449 layernext-beta-3.2.0b0/layernext/studio/
+-rw-r--r--   0 chathushka   (501) staff       (20)     3661 2024-02-28 06:35:15.000000 layernext-beta-3.2.0b0/layernext/studio/__init__.py
+-rw-r--r--   0 chathushka   (501) staff       (20)      431 2024-02-28 06:35:15.000000 layernext-beta-3.2.0b0/layernext/studio/logger.py
+-rw-r--r--   0 chathushka   (501) staff       (20)     3860 2024-02-28 06:35:15.000000 layernext-beta-3.2.0b0/layernext/studio/project.py
+-rw-r--r--   0 chathushka   (501) staff       (20)    13127 2024-02-28 06:35:15.000000 layernext-beta-3.2.0b0/layernext/studio/studiointerface.py
+drwxr-xr-x   0 chathushka   (501) staff       (20)        0 2024-04-02 03:48:15.386995 layernext-beta-3.2.0b0/layernext_beta.egg-info/
+-rw-r--r--   0 chathushka   (501) staff       (20)     1126 2024-04-02 03:48:15.000000 layernext-beta-3.2.0b0/layernext_beta.egg-info/PKG-INFO
+-rw-r--r--   0 chathushka   (501) staff       (20)     1487 2024-04-02 03:48:15.000000 layernext-beta-3.2.0b0/layernext_beta.egg-info/SOURCES.txt
+-rw-r--r--   0 chathushka   (501) staff       (20)        1 2024-04-02 03:48:15.000000 layernext-beta-3.2.0b0/layernext_beta.egg-info/dependency_links.txt
+-rw-r--r--   0 chathushka   (501) staff       (20)       78 2024-04-02 03:48:15.000000 layernext-beta-3.2.0b0/layernext_beta.egg-info/requires.txt
+-rw-r--r--   0 chathushka   (501) staff       (20)       10 2024-04-02 03:48:15.000000 layernext-beta-3.2.0b0/layernext_beta.egg-info/top_level.txt
+-rw-r--r--   0 chathushka   (501) staff       (20)       38 2024-04-02 03:48:15.388650 layernext-beta-3.2.0b0/setup.cfg
+-rw-r--r--   0 chathushka   (501) staff       (20)     1950 2024-02-28 06:35:15.000000 layernext-beta-3.2.0b0/setup.py
+drwxr-xr-x   0 chathushka   (501) staff       (20)        0 2024-04-02 03:48:15.386500 layernext-beta-3.2.0b0/tests/
+-rw-r--r--   0 chathushka   (501) staff       (20)     1043 2023-09-11 10:46:59.000000 layernext-beta-3.2.0b0/tests/test_cli.py
```

### Comparing `layernext-beta-3.1.1b6/LICENSE` & `layernext-beta-3.2.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.1.1b6/PKG-INFO` & `layernext-beta-3.2.0b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: layernext-beta
-Version: 3.1.1b6
+Version: 3.2.0b0
 Summary: LayerNext Python SDK
 Author: LayerNext
 Author-email: <support@layernext.ai>
 Keywords: python,datalake,datasetsync,ai,annotation,layernext,layernext,machine learning
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `layernext-beta-3.1.1b6/layernext/__init__.py` & `layernext-beta-3.2.0b0/layernext/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from deprecated import deprecated
 import uuid
 from layernext.datalake.logger import get_debug_logger
 
 # Create a package-level logger
 logger = get_debug_logger(__name__)
 
-__version__ = "3.1.1b6"
+__version__ = "3.2.0b0"
 
 
 class LayerNextClient:
     """
     Python SDK of LayerNext
     """
 
@@ -3480,7 +3480,46 @@
 
         """
         _datalake_client = datalake.DatalakeClient(
             self.encoded_key_secret, self.layernext_url
         )
 
         return _datalake_client.get_source_list(source_list)
+
+    def retrieve_db_unstructured_records(
+        self, categories=[], filter_key_values={}, page_index=0
+    ):
+        """
+        categories (list): Category names relevant to each section of data being considered for locating records.
+
+        filter_key_values (dictionary): Key value pairs derived from the question to locate matching records.
+        Note that the values in key information should be provided as list in below format
+        { "key_1": [<value_1>, <value_2>, ...], "key_2": [<value_1>, <value_2>, ...]}
+        Example:{ "id": [1101, 1302, 1435], "type": ["retail"]}
+
+        page_index (int): Index for the batch required.
+
+        Behavior:
+
+        Returns: a list of dictionaries, where each dictionary contains key information as a dictionary and the unstructured data as list of strings.
+                [
+                    {
+                    "keyInfo": {
+                        "key_1": <value_1>,
+                        "key_2": <value_2>
+                    }
+                    "data": ["data_1", "data_2", ....]
+                    }
+                ]
+        Example usage: retrieve_documents(["reviews"], {
+                "id": [1101, 1302, 1435],
+                "type": ["retail"]
+            }, 0)
+        """
+
+        _datalake_client = datalake.DatalakeClient(
+            self.encoded_key_secret, self.layernext_url
+        )
+
+        return _datalake_client.retrieve_db_unstructured_records(
+            categories, filter_key_values, page_index
+        )
```

### Comparing `layernext-beta-3.1.1b6/layernext/automatic_analysis/__init__.py` & `layernext-beta-3.2.0b0/layernext/automatic_analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.1.1b6/layernext/automatic_analysis/automatic_analysis.py` & `layernext-beta-3.2.0b0/layernext/automatic_analysis/automatic_analysis.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.1.1b6/layernext/automatic_analysis/automatic_analysis_interface.py` & `layernext-beta-3.2.0b0/layernext/automatic_analysis/automatic_analysis_interface.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.1.1b6/layernext/automatic_analysis/status_check_autoannotate_project.py` & `layernext-beta-3.2.0b0/layernext/automatic_analysis/status_check_autoannotate_project.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.1.1b6/layernext/automatic_analysis/support.py` & `layernext-beta-3.2.0b0/layernext/automatic_analysis/support.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.1.1b6/layernext/datalake/__init__.py` & `layernext-beta-3.2.0b0/layernext/datalake/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -791,7 +791,18 @@
         """
 
         payload = {
             "sourceList": source_list,
         }
         res = self.datalake_interface.get_source_list(payload)
         return res
+
+    def retrieve_db_unstructured_records(
+        self, categories=[], filter_key_values={}, page_index=0
+    ):
+        payload = {
+            "categories": categories,
+            "filterKeyValues": filter_key_values,
+            "pageIndex": page_index,
+        }
+        res = self.datalake_interface.retrieve_db_unstructured_records(payload)
+        return res
```

### Comparing `layernext-beta-3.1.1b6/layernext/datalake/annotation.py` & `layernext-beta-3.2.0b0/layernext/datalake/annotation.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.1.1b6/layernext/datalake/aws_s3_client.py` & `layernext-beta-3.2.0b0/layernext/datalake/aws_s3_client.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.1.1b6/layernext/datalake/azure_client.py` & `layernext-beta-3.2.0b0/layernext/datalake/azure_client.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.1.1b6/layernext/datalake/constants.py` & `layernext-beta-3.2.0b0/layernext/datalake/constants.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.1.1b6/layernext/datalake/datalakeinterface.py` & `layernext-beta-3.2.0b0/layernext/datalake/datalakeinterface.py`

 * *Files 0% similar despite different names*

```diff
@@ -2176,7 +2176,19 @@
                 "success": False,
                 "message": "An unexpected request exception occurred",
             }
         except Exception as e1:
             print(f"An unexpected exception occurred: {format(e1)}")
             traceback.print_exc()
             return {"success": False, "message": "An unexpected exception occurred"}
+
+    def retrieve_db_unstructured_records(self, payload: dict):
+        hed = {"Authorization": "Basic " + self.auth_token}
+        url = f"{self.dalalake_url}/api/client/retrieve/unstructuredRecords"
+
+        response = requests.post(url=url, json=payload, headers=hed)
+        status_code = response.status_code
+        res = response.json()
+        if status_code == 200:
+            return response.json()
+        else:
+            raise Exception(f"{res['error']['message']}")
```

### Comparing `layernext-beta-3.1.1b6/layernext/datalake/file_upload.py` & `layernext-beta-3.2.0b0/layernext/datalake/file_upload.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.1.1b6/layernext/datalake/gcs_client.py` & `layernext-beta-3.2.0b0/layernext/datalake/gcs_client.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.1.1b6/layernext/datalake/ground_truth.py` & `layernext-beta-3.2.0b0/layernext/datalake/ground_truth.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.1.1b6/layernext/datalake/keys.py` & `layernext-beta-3.2.0b0/layernext/datalake/keys.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.1.1b6/layernext/datalake/label.py` & `layernext-beta-3.2.0b0/layernext/datalake/label.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.1.1b6/layernext/datalake/logger.py` & `layernext-beta-3.2.0b0/layernext/datalake/logger.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.1.1b6/layernext/datalake/metadata.py` & `layernext-beta-3.2.0b0/layernext/datalake/metadata.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.1.1b6/layernext/datalake/model_run.py` & `layernext-beta-3.2.0b0/layernext/datalake/model_run.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.1.1b6/layernext/datalake/mongo_json_encoder.py` & `layernext-beta-3.2.0b0/layernext/datalake/mongo_json_encoder.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.1.1b6/layernext/datalake/query.py` & `layernext-beta-3.2.0b0/layernext/datalake/query.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.1.1b6/layernext/datalake/storage_interface.py` & `layernext-beta-3.2.0b0/layernext/datalake/storage_interface.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.1.1b6/layernext/datalake/storage_upload.py` & `layernext-beta-3.2.0b0/layernext/datalake/storage_upload.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.1.1b6/layernext/dataset/__init__.py` & `layernext-beta-3.2.0b0/layernext/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.1.1b6/layernext/dataset/dataset.py` & `layernext-beta-3.2.0b0/layernext/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.1.1b6/layernext/dataset/datasetinterface.py` & `layernext-beta-3.2.0b0/layernext/dataset/datasetinterface.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.1.1b6/layernext/dataset/sync.py` & `layernext-beta-3.2.0b0/layernext/dataset/sync.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.1.1b6/layernext/studio/__init__.py` & `layernext-beta-3.2.0b0/layernext/studio/__init__.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.1.1b6/layernext/studio/project.py` & `layernext-beta-3.2.0b0/layernext/studio/project.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.1.1b6/layernext/studio/studiointerface.py` & `layernext-beta-3.2.0b0/layernext/studio/studiointerface.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.1.1b6/layernext_beta.egg-info/PKG-INFO` & `layernext-beta-3.2.0b0/layernext_beta.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: layernext-beta
-Version: 3.1.1b6
+Version: 3.2.0b0
 Summary: LayerNext Python SDK
 Author: LayerNext
 Author-email: <support@layernext.ai>
 Keywords: python,datalake,datasetsync,ai,annotation,layernext,layernext,machine learning
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `layernext-beta-3.1.1b6/layernext_beta.egg-info/SOURCES.txt` & `layernext-beta-3.2.0b0/layernext_beta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.1.1b6/setup.py` & `layernext-beta-3.2.0b0/setup.py`

 * *Files identical despite different names*

### Comparing `layernext-beta-3.1.1b6/tests/test_cli.py` & `layernext-beta-3.2.0b0/tests/test_cli.py`

 * *Files identical despite different names*

