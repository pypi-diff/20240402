# Comparing `tmp/e-models-1.8.5.tar.gz` & `tmp/e-models-1.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e-models-1.8.5.tar", last modified: Tue Mar 19 21:16:22 2024, max compression
+gzip compressed data, was "e-models-1.8.6.tar", last modified: Tue Apr  2 19:05:36 2024, max compression
```

## Comparing `e-models-1.8.5.tar` & `e-models-1.8.6.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2024-03-19 21:16:22.969753 e-models-1.8.5/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1501 2023-03-30 21:13:00.000000 e-models-1.8.5/LICENSE
--rw-r--r--   0 molveyra  (1001) molveyra  (1001)    13330 2024-03-19 21:16:22.969753 e-models-1.8.5/PKG-INFO
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    12478 2024-02-27 17:55:52.000000 e-models-1.8.5/README.md
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2024-03-19 21:16:22.965753 e-models-1.8.5/e_models.egg-info/
--rw-r--r--   0 molveyra  (1001) molveyra  (1001)    13330 2024-03-19 21:16:22.000000 e-models-1.8.5/e_models.egg-info/PKG-INFO
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      710 2024-03-19 21:16:22.000000 e-models-1.8.5/e_models.egg-info/SOURCES.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        1 2024-03-19 21:16:22.000000 e-models-1.8.5/e_models.egg-info/dependency_links.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      104 2024-03-19 21:16:22.000000 e-models-1.8.5/e_models.egg-info/requires.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        8 2024-03-19 21:16:22.000000 e-models-1.8.5/e_models.egg-info/top_level.txt
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2024-03-19 21:16:22.965753 e-models-1.8.5/emodels/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       22 2024-03-19 21:15:07.000000 e-models-1.8.5/emodels/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      340 2023-11-06 19:18:12.000000 e-models-1.8.5/emodels/config.py
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2024-03-19 21:16:22.965753 e-models-1.8.5/emodels/datasets/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-06-23 18:11:59.000000 e-models-1.8.5/emodels/datasets/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    16404 2023-11-03 19:09:54.000000 e-models-1.8.5/emodels/datasets/hugging.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    20047 2024-03-19 20:50:31.000000 e-models-1.8.5/emodels/datasets/models.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      374 2023-08-31 18:27:15.000000 e-models-1.8.5/emodels/datasets/stypes.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2299 2024-03-14 19:03:35.000000 e-models-1.8.5/emodels/datasets/tokenizers.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    12361 2024-03-18 21:52:08.000000 e-models-1.8.5/emodels/datasets/utils.py
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2024-03-19 21:16:22.969753 e-models-1.8.5/emodels/html2text/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    35479 2023-07-21 16:26:32.000000 e-models-1.8.5/emodels/html2text/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3873 2023-05-04 18:51:26.000000 e-models-1.8.5/emodels/html2text/config.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      423 2023-05-04 18:51:26.000000 e-models-1.8.5/emodels/html2text/elements.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       71 2023-05-04 18:51:26.000000 e-models-1.8.5/emodels/html2text/typing.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     8034 2023-05-04 18:51:26.000000 e-models-1.8.5/emodels/html2text/utils.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-05-04 18:51:26.000000 e-models-1.8.5/emodels/py.typed
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2024-03-19 21:16:22.969753 e-models-1.8.5/emodels/scrapyutils/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-08-04 13:47:09.000000 e-models-1.8.5/emodels/scrapyutils/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     4734 2024-02-27 12:04:53.000000 e-models-1.8.5/emodels/scrapyutils/loader.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     6339 2024-02-27 17:16:48.000000 e-models-1.8.5/emodels/scrapyutils/response.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       31 2023-03-30 21:32:48.000000 e-models-1.8.5/pyproject.toml
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       38 2024-03-19 21:16:22.969753 e-models-1.8.5/setup.cfg
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1086 2024-03-19 21:15:15.000000 e-models-1.8.5/setup.py
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2024-03-19 21:16:22.969753 e-models-1.8.5/tests/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     6355 2023-08-04 13:47:35.000000 e-models-1.8.5/tests/test_html2text.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    12999 2024-02-27 17:16:48.000000 e-models-1.8.5/tests/test_scrapyutils.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2024-04-02 19:05:36.722112 e-models-1.8.6/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1501 2023-03-30 21:13:00.000000 e-models-1.8.6/LICENSE
+-rw-r--r--   0 molveyra  (1001) molveyra  (1001)    13330 2024-04-02 19:05:36.718112 e-models-1.8.6/PKG-INFO
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    12478 2024-02-27 17:55:52.000000 e-models-1.8.6/README.md
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2024-04-02 19:05:36.714112 e-models-1.8.6/e_models.egg-info/
+-rw-r--r--   0 molveyra  (1001) molveyra  (1001)    13330 2024-04-02 19:05:36.000000 e-models-1.8.6/e_models.egg-info/PKG-INFO
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      710 2024-04-02 19:05:36.000000 e-models-1.8.6/e_models.egg-info/SOURCES.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        1 2024-04-02 19:05:36.000000 e-models-1.8.6/e_models.egg-info/dependency_links.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      104 2024-04-02 19:05:36.000000 e-models-1.8.6/e_models.egg-info/requires.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        8 2024-04-02 19:05:36.000000 e-models-1.8.6/e_models.egg-info/top_level.txt
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2024-04-02 19:05:36.714112 e-models-1.8.6/emodels/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       22 2024-04-02 19:05:09.000000 e-models-1.8.6/emodels/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      340 2023-11-06 19:18:12.000000 e-models-1.8.6/emodels/config.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2024-04-02 19:05:36.714112 e-models-1.8.6/emodels/datasets/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-06-23 18:11:59.000000 e-models-1.8.6/emodels/datasets/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    16404 2023-11-03 19:09:54.000000 e-models-1.8.6/emodels/datasets/hugging.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    20458 2024-04-02 19:03:57.000000 e-models-1.8.6/emodels/datasets/models.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      374 2023-08-31 18:27:15.000000 e-models-1.8.6/emodels/datasets/stypes.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2299 2024-03-14 19:03:35.000000 e-models-1.8.6/emodels/datasets/tokenizers.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    12361 2024-03-18 21:52:08.000000 e-models-1.8.6/emodels/datasets/utils.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2024-04-02 19:05:36.718112 e-models-1.8.6/emodels/html2text/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    35479 2023-07-21 16:26:32.000000 e-models-1.8.6/emodels/html2text/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3873 2023-05-04 18:51:26.000000 e-models-1.8.6/emodels/html2text/config.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      423 2023-05-04 18:51:26.000000 e-models-1.8.6/emodels/html2text/elements.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       71 2023-05-04 18:51:26.000000 e-models-1.8.6/emodels/html2text/typing.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     8034 2023-05-04 18:51:26.000000 e-models-1.8.6/emodels/html2text/utils.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-05-04 18:51:26.000000 e-models-1.8.6/emodels/py.typed
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2024-04-02 19:05:36.718112 e-models-1.8.6/emodels/scrapyutils/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-08-04 13:47:09.000000 e-models-1.8.6/emodels/scrapyutils/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     4734 2024-02-27 12:04:53.000000 e-models-1.8.6/emodels/scrapyutils/loader.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     6339 2024-02-27 17:16:48.000000 e-models-1.8.6/emodels/scrapyutils/response.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       31 2023-03-30 21:32:48.000000 e-models-1.8.6/pyproject.toml
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       38 2024-04-02 19:05:36.722112 e-models-1.8.6/setup.cfg
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1086 2024-04-02 19:05:01.000000 e-models-1.8.6/setup.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2024-04-02 19:05:36.718112 e-models-1.8.6/tests/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     6355 2023-08-04 13:47:35.000000 e-models-1.8.6/tests/test_html2text.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    12999 2024-02-27 17:16:48.000000 e-models-1.8.6/tests/test_scrapyutils.py
```

### Comparing `e-models-1.8.5/LICENSE` & `e-models-1.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `e-models-1.8.5/PKG-INFO` & `e-models-1.8.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e-models
-Version: 1.8.5
+Version: 1.8.6
 Summary: Tools for helping build of extraction models with scrapy spiders.
 Home-page: https://github.com/kalessin/emodels
 Author: Martin Olveyra
 Author-email: molveyra@gmail.com
 License: BSD
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `e-models-1.8.5/README.md` & `e-models-1.8.6/README.md`

 * *Files identical despite different names*

### Comparing `e-models-1.8.5/e_models.egg-info/PKG-INFO` & `e-models-1.8.6/e_models.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e-models
-Version: 1.8.5
+Version: 1.8.6
 Summary: Tools for helping build of extraction models with scrapy spiders.
 Home-page: https://github.com/kalessin/emodels
 Author: Martin Olveyra
 Author-email: molveyra@gmail.com
 License: BSD
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `e-models-1.8.5/e_models.egg-info/SOURCES.txt` & `e-models-1.8.6/e_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `e-models-1.8.5/emodels/datasets/hugging.py` & `e-models-1.8.6/emodels/datasets/hugging.py`

 * *Files identical despite different names*

### Comparing `e-models-1.8.5/emodels/datasets/models.py` & `e-models-1.8.6/emodels/datasets/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,33 +172,37 @@
     def _fshelper(cls) -> FSHelper:
         if cls.FSHELPER is None:
             settings = get_project_settings()
             cls.FSHELPER = cls.build_fshelper(settings)
         return cls.FSHELPER
 
     @classmethod
+    def _check_sample(cls, dsample: E, idx: int = 0):
+        keys = set(dsample.keys())
+        assert cls.target_label in keys, f"{cls.target_label} key not in sample #{idx}."
+        missing_fields = set(cls.features).difference(keys)
+        assert not missing_fields, f"Missing fields in sample #{idx}: {missing_fields}"
+
+    @classmethod
     def load_dataset(cls) -> DatasetsPandas[E]:
         dataset_local: DatasetFilename[E] = cls.dataset_repository.local(cls.project)
 
         if cls._fshelper().exists(dataset_local):
             LOGGER.info(f"Found local copy of datasets {dataset_local}.")
         elif cls._fshelper().exists(cls.dataset_repository):
             LOGGER.info("Downloading datasets...")
             cls._fshelper().download_file(cls.dataset_repository, dataset_local)
         else:
             LOGGER.info("Generating datasets...")
             for idx, sample in enumerate(cls.generate_dataset_samples()):
+                cls._check_sample(sample, idx)
                 keys = set(sample.keys())
-                assert cls.target_label in keys, f"{cls.target_label} key not in sample #{idx}."
-                keys.remove(cls.target_label)
                 assert "dataset_bucket" in keys, f"dataset_bucket key not in sample #{idx}."
                 bucket = sample["dataset_bucket"]
                 assert bucket in ("train", "test", "validation"), f"Invalid bucket for sample #{idx}: {bucket}"
-                missing_fields = set(cls.features).difference(keys)
-                assert not missing_fields, f"Missing fields in sample #{idx}: {missing_fields}"
                 dataset_local.append(sample)
             cls._fshelper().upload_file(dataset_local, cls.dataset_repository)
         return DatasetsPandas.from_datasetfilename(dataset_local, cls.features, cls.target_label)
 
     @classmethod
     def get_dataset(cls) -> DatasetsPandas[E]:
         if cls.datasets is None:
@@ -229,17 +233,26 @@
         ...
 
     @classmethod
     def append_sample(cls, sample: SAMPLE, bucket: DatasetBucket):
         """
         Add sample to the specified dataset in cls.scraped_samples list.
         """
+        dsample = cls.get_sample_data_from_sample(sample)
+        cls._check_sample(dsample)
         cls.scraped_samples[bucket].append(sample)
 
     @classmethod
+    def rebalance_samples(cls, bucket: DatasetBucket):
+        """
+        Rebalance target sample dataset so all labels has similar count, by randomly removing
+        excess of samples with same label.
+        """
+
+    @classmethod
     def generate_dataset_samples(cls) -> Generator[E, None, None]:
         """Generate samples from cls.scraped_samples in order create the dataset repository.
         This dataset must contain sample objects, each object containing
         the features field (as specified by cls.features attribute), the target
         field (as specified by cls.target_label attribute) and the field `dataset_bucket`
         with a value being either "train" or "test".
         """
```

### Comparing `e-models-1.8.5/emodels/datasets/tokenizers.py` & `e-models-1.8.6/emodels/datasets/tokenizers.py`

 * *Files identical despite different names*

### Comparing `e-models-1.8.5/emodels/datasets/utils.py` & `e-models-1.8.6/emodels/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `e-models-1.8.5/emodels/html2text/__init__.py` & `e-models-1.8.6/emodels/html2text/__init__.py`

 * *Files identical despite different names*

### Comparing `e-models-1.8.5/emodels/html2text/config.py` & `e-models-1.8.6/emodels/html2text/config.py`

 * *Files identical despite different names*

### Comparing `e-models-1.8.5/emodels/html2text/utils.py` & `e-models-1.8.6/emodels/html2text/utils.py`

 * *Files identical despite different names*

### Comparing `e-models-1.8.5/emodels/scrapyutils/loader.py` & `e-models-1.8.6/emodels/scrapyutils/loader.py`

 * *Files identical despite different names*

### Comparing `e-models-1.8.5/emodels/scrapyutils/response.py` & `e-models-1.8.6/emodels/scrapyutils/response.py`

 * *Files identical despite different names*

### Comparing `e-models-1.8.5/setup.py` & `e-models-1.8.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Automatically created by: shub deploy
 
 from setuptools import setup, find_packages
 
 setup(
     name         = 'e-models',
-    version      = '1.8.5',
+    version      = '1.8.6',
     description  = 'Tools for helping build of extraction models with scrapy spiders.',
     long_description = open('README.md').read(),
     long_description_content_type = 'text/markdown',
     license      = 'BSD',
     author       = 'Martin Olveyra',
     author_email = 'molveyra@gmail.com',
     url          = 'https://github.com/kalessin/emodels',
```

### Comparing `e-models-1.8.5/tests/test_html2text.py` & `e-models-1.8.6/tests/test_html2text.py`

 * *Files identical despite different names*

### Comparing `e-models-1.8.5/tests/test_scrapyutils.py` & `e-models-1.8.6/tests/test_scrapyutils.py`

 * *Files identical despite different names*

