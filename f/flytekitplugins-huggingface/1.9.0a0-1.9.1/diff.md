# Comparing `tmp/flytekitplugins-huggingface-1.9.0a0.tar.gz` & `tmp/flytekitplugins-huggingface-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-huggingface-1.9.0a0.tar", last modified: Thu Jul 20 18:58:19 2023, max compression
+gzip compressed data, was "flytekitplugins-huggingface-1.9.1.tar", last modified: Mon Aug 28 16:43:07 2023, max compression
```

## Comparing `flytekitplugins-huggingface-1.9.0a0.tar` & `flytekitplugins-huggingface-1.9.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:19.680683 flytekitplugins-huggingface-1.9.0a0/
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-20 18:58:19.680683 flytekitplugins-huggingface-1.9.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-20 18:57:54.000000 flytekitplugins-huggingface-1.9.0a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:19.680683 flytekitplugins-huggingface-1.9.0a0/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:19.680683 flytekitplugins-huggingface-1.9.0a0/flytekitplugins/huggingface/
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-20 18:57:54.000000 flytekitplugins-huggingface-1.9.0a0/flytekitplugins/huggingface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-07-20 18:57:54.000000 flytekitplugins-huggingface-1.9.0a0/flytekitplugins/huggingface/sd_transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:19.680683 flytekitplugins-huggingface-1.9.0a0/flytekitplugins_huggingface.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-20 18:58:19.000000 flytekitplugins-huggingface-1.9.0a0/flytekitplugins_huggingface.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-20 18:58:19.000000 flytekitplugins-huggingface-1.9.0a0/flytekitplugins_huggingface.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 18:58:19.000000 flytekitplugins-huggingface-1.9.0a0/flytekitplugins_huggingface.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-20 18:58:19.000000 flytekitplugins-huggingface-1.9.0a0/flytekitplugins_huggingface.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 18:58:19.000000 flytekitplugins-huggingface-1.9.0a0/flytekitplugins_huggingface.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-20 18:58:19.000000 flytekitplugins-huggingface-1.9.0a0/flytekitplugins_huggingface.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 18:58:19.000000 flytekitplugins-huggingface-1.9.0a0/flytekitplugins_huggingface.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 18:58:19.680683 flytekitplugins-huggingface-1.9.0a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-20 18:58:12.000000 flytekitplugins-huggingface-1.9.0a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:43:07.170123 flytekitplugins-huggingface-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (999)     1423 2023-08-28 16:43:07.170123 flytekitplugins-huggingface-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)      537 2023-08-28 16:42:38.000000 flytekitplugins-huggingface-1.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:43:07.166123 flytekitplugins-huggingface-1.9.1/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:43:07.170123 flytekitplugins-huggingface-1.9.1/flytekitplugins/huggingface/
+-rw-r--r--   0 runner    (1001) docker     (999)      417 2023-08-28 16:42:38.000000 flytekitplugins-huggingface-1.9.1/flytekitplugins/huggingface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2946 2023-08-28 16:42:38.000000 flytekitplugins-huggingface-1.9.1/flytekitplugins/huggingface/sd_transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:43:07.170123 flytekitplugins-huggingface-1.9.1/flytekitplugins_huggingface.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (999)     1423 2023-08-28 16:43:07.000000 flytekitplugins-huggingface-1.9.1/flytekitplugins_huggingface.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)      473 2023-08-28 16:43:07.000000 flytekitplugins-huggingface-1.9.1/flytekitplugins_huggingface.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-28 16:43:07.000000 flytekitplugins-huggingface-1.9.1/flytekitplugins_huggingface.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       61 2023-08-28 16:43:07.000000 flytekitplugins-huggingface-1.9.1/flytekitplugins_huggingface.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       16 2023-08-28 16:43:07.000000 flytekitplugins-huggingface-1.9.1/flytekitplugins_huggingface.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       41 2023-08-28 16:43:07.000000 flytekitplugins-huggingface-1.9.1/flytekitplugins_huggingface.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       16 2023-08-28 16:43:07.000000 flytekitplugins-huggingface-1.9.1/flytekitplugins_huggingface.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       38 2023-08-28 16:43:07.170123 flytekitplugins-huggingface-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (999)     1453 2023-08-28 16:43:00.000000 flytekitplugins-huggingface-1.9.1/setup.py
```

### Comparing `flytekitplugins-huggingface-1.9.0a0/PKG-INFO` & `flytekitplugins-huggingface-1.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-huggingface
-Version: 1.9.0a0
+Version: 1.9.1
 Summary: Hugging Face plugin for flytekit
 Home-page: https://github.com/flyteorg/flytekit/tree/master/plugins/flytekit-huggingface
 Author: Evan Sadler
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-huggingface-1.9.0a0/README.md` & `flytekitplugins-huggingface-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-huggingface-1.9.0a0/flytekitplugins/huggingface/sd_transformers.py` & `flytekitplugins-huggingface-1.9.1/flytekitplugins/huggingface/sd_transformers.py`

 * *Files 20% similar despite different names*

```diff
@@ -34,14 +34,18 @@
         self,
         ctx: FlyteContext,
         structured_dataset: StructuredDataset,
         structured_dataset_type: StructuredDatasetType,
     ) -> literals.StructuredDataset:
         df = typing.cast(datasets.Dataset, structured_dataset.dataframe)
 
+        if structured_dataset_type.columns:
+            columns = [c.name for c in structured_dataset_type.columns]
+            df = df.remove_columns([c for c in df.features.keys() if c not in columns])
+
         local_dir = ctx.file_access.get_random_local_directory()
         local_path = f"{local_dir}/00000"
 
         df.to_parquet(local_path)
 
         remote_dir = typing.cast(str, structured_dataset.uri) or ctx.file_access.get_random_remote_directory()
         ctx.file_access.upload_directory(local_dir, remote_dir)
```

### Comparing `flytekitplugins-huggingface-1.9.0a0/flytekitplugins_huggingface.egg-info/PKG-INFO` & `flytekitplugins-huggingface-1.9.1/flytekitplugins_huggingface.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-huggingface
-Version: 1.9.0a0
+Version: 1.9.1
 Summary: Hugging Face plugin for flytekit
 Home-page: https://github.com/flyteorg/flytekit/tree/master/plugins/flytekit-huggingface
 Author: Evan Sadler
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-huggingface-1.9.0a0/setup.py` & `flytekitplugins-huggingface-1.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = [
     "flytekit>=1.3.0b2,<2.0.0",
     "datasets>=2.4.0",
 ]
 
-__version__ = "1.9.0a0"
+__version__ = "1.9.1"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="Evan Sadler",
     description="Hugging Face plugin for flytekit",
     url="https://github.com/flyteorg/flytekit/tree/master/plugins/flytekit-huggingface",
```

