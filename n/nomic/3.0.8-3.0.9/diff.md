# Comparing `tmp/nomic-3.0.8.tar.gz` & `tmp/nomic-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nomic-3.0.8.tar", last modified: Thu Feb  1 02:37:04 2024, max compression
+gzip compressed data, was "nomic-3.0.9.tar", last modified: Thu Feb  1 21:33:23 2024, max compression
```

## Comparing `nomic-3.0.8.tar` & `nomic-3.0.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-02-01 02:37:04.133933 nomic-3.0.8/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      387 2024-02-01 02:37:04.133933 nomic-3.0.8/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7736 2024-02-01 02:36:57.000000 nomic-3.0.8/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-02-01 02:37:04.129933 nomic-3.0.8/nomic/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       68 2024-02-01 02:36:57.000000 nomic-3.0.8/nomic/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10304 2024-02-01 02:36:57.000000 nomic-3.0.8/nomic/atlas.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6072 2024-02-01 02:36:57.000000 nomic-3.0.8/nomic/cli.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3830 2024-02-01 02:36:57.000000 nomic-3.0.8/nomic/data_inference.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    34359 2024-02-01 02:36:57.000000 nomic-3.0.8/nomic/data_operations.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    61971 2024-02-01 02:36:57.000000 nomic-3.0.8/nomic/dataset.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6518 2024-02-01 02:36:57.000000 nomic-3.0.8/nomic/embed.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-02-01 02:37:04.133933 nomic-3.0.8/nomic/pl_callbacks/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       48 2024-02-01 02:36:57.000000 nomic-3.0.8/nomic/pl_callbacks/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6862 2024-02-01 02:36:57.000000 nomic-3.0.8/nomic/pl_callbacks/pl_callback.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      553 2024-02-01 02:36:57.000000 nomic-3.0.8/nomic/settings.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-02-01 02:37:04.133933 nomic-3.0.8/nomic/tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-02-01 02:36:57.000000 nomic-3.0.8/nomic/tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11320 2024-02-01 02:36:57.000000 nomic-3.0.8/nomic/tests/test_atlas_client.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4365 2024-02-01 02:36:57.000000 nomic-3.0.8/nomic/utils.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-02-01 02:37:04.129933 nomic-3.0.8/nomic.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      387 2024-02-01 02:37:04.000000 nomic-3.0.8/nomic.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      476 2024-02-01 02:37:04.000000 nomic-3.0.8/nomic.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2024-02-01 02:37:04.000000 nomic-3.0.8/nomic.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       41 2024-02-01 02:37:04.000000 nomic-3.0.8/nomic.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      217 2024-02-01 02:37:04.000000 nomic-3.0.8/nomic.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        6 2024-02-01 02:37:04.000000 nomic-3.0.8/nomic.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2024-02-01 02:37:04.133933 nomic-3.0.8/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1252 2024-02-01 02:36:57.000000 nomic-3.0.8/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-02-01 21:33:23.242638 nomic-3.0.9/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      387 2024-02-01 21:33:23.242638 nomic-3.0.9/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7736 2024-02-01 21:33:15.000000 nomic-3.0.9/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-02-01 21:33:23.242638 nomic-3.0.9/nomic/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       68 2024-02-01 21:33:15.000000 nomic-3.0.9/nomic/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10919 2024-02-01 21:33:15.000000 nomic-3.0.9/nomic/atlas.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6072 2024-02-01 21:33:15.000000 nomic-3.0.9/nomic/cli.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3830 2024-02-01 21:33:15.000000 nomic-3.0.9/nomic/data_inference.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    34359 2024-02-01 21:33:15.000000 nomic-3.0.9/nomic/data_operations.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    62042 2024-02-01 21:33:15.000000 nomic-3.0.9/nomic/dataset.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6518 2024-02-01 21:33:15.000000 nomic-3.0.9/nomic/embed.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-02-01 21:33:23.242638 nomic-3.0.9/nomic/pl_callbacks/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       48 2024-02-01 21:33:15.000000 nomic-3.0.9/nomic/pl_callbacks/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6862 2024-02-01 21:33:15.000000 nomic-3.0.9/nomic/pl_callbacks/pl_callback.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      553 2024-02-01 21:33:15.000000 nomic-3.0.9/nomic/settings.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-02-01 21:33:23.242638 nomic-3.0.9/nomic/tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-02-01 21:33:15.000000 nomic-3.0.9/nomic/tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11231 2024-02-01 21:33:15.000000 nomic-3.0.9/nomic/tests/test_atlas_client.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4365 2024-02-01 21:33:15.000000 nomic-3.0.9/nomic/utils.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-02-01 21:33:23.242638 nomic-3.0.9/nomic.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      387 2024-02-01 21:33:23.000000 nomic-3.0.9/nomic.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      476 2024-02-01 21:33:23.000000 nomic-3.0.9/nomic.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2024-02-01 21:33:23.000000 nomic-3.0.9/nomic.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       41 2024-02-01 21:33:23.000000 nomic-3.0.9/nomic.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      217 2024-02-01 21:33:23.000000 nomic-3.0.9/nomic.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        6 2024-02-01 21:33:23.000000 nomic-3.0.9/nomic.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2024-02-01 21:33:23.242638 nomic-3.0.9/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1252 2024-02-01 21:33:15.000000 nomic-3.0.9/setup.py
```

### Comparing `nomic-3.0.8/README.md` & `nomic-3.0.9/README.md`

 * *Files identical despite different names*

### Comparing `nomic-3.0.8/nomic/atlas.py` & `nomic-3.0.9/nomic/atlas.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,20 +71,30 @@
 
     # no metadata was specified
     added_id_field = False
     if data is None:
         data = [{ATLAS_DEFAULT_ID_FIELD: b64int(i)} for i in range(len(embeddings))]
         added_id_field = True
 
-    if id_field == ATLAS_DEFAULT_ID_FIELD and id_field not in data[0]:
-        added_id_field = True
-        for i in range(len(data)):
-            # do not modify object the user passed in - also ensures IDs are unique if two input datums are the same *object*
-            data[i] = data[i].copy()
-            data[i][id_field] = b64int(i)
+    if id_field == ATLAS_DEFAULT_ID_FIELD:
+        if isinstance(data, list) and id_field not in data[0]:
+            added_id_field = True
+            for i in range(len(data)):
+                # do not modify object the user passed in - also ensures IDs are unique if two input datums are the same *object*
+                data[i] = data[i].copy()
+                data[i][id_field] = b64int(i)
+        elif isinstance(data, DataFrame) and id_field not in data.columns:
+            data[id_field] = [b64int(i) for i in range(data.shape[0])]
+            added_id_field = True
+        elif isinstance(data, pa.Table) and not id_field in data.column_names:
+            ids = pa.array([b64int(i) for i in range(len(data))])
+            data = data.append_column(id_field, ids)
+            added_id_field = True
+        elif id_field not in data[0]:
+            raise ValueError("map_data data must be a list of dicts, a pandas dataframe, or a pyarrow table")
 
     if added_id_field:
         logger.warning("An ID field was not specified in your data so one was generated for you in insertion order.")
 
     dataset = AtlasDataset(
         identifier=dataset_name, description=description, unique_id_field=id_field, is_public=is_public
     )
```

### Comparing `nomic-3.0.8/nomic/cli.py` & `nomic-3.0.9/nomic/cli.py`

 * *Files identical despite different names*

### Comparing `nomic-3.0.8/nomic/data_inference.py` & `nomic-3.0.9/nomic/data_inference.py`

 * *Files identical despite different names*

### Comparing `nomic-3.0.8/nomic/data_operations.py` & `nomic-3.0.9/nomic/data_operations.py`

 * *Files identical despite different names*

### Comparing `nomic-3.0.8/nomic/dataset.py` & `nomic-3.0.9/nomic/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1327,15 +1327,15 @@
         """
         Adds data of varying modality to an Atlas dataset.
         Args:
             data: A pandas DataFrame, list of dictionaries, or pyarrow Table matching the dataset schema.
             embeddings: A numpy array of embeddings: each row corresponds to a row in the table. Use if you already have embeddings for your datapoints.
             pbar: (Optional). A tqdm progress bar to update.
         """
-        if embeddings is not None:
+        if embeddings is not None or (isinstance(data, pa.Table) and "_embeddings" in data.column_names):
             self._add_embeddings(data=data, embeddings=embeddings, pbar=pbar)
         else:
             self._add_text(data=data, pbar=pbar)
 
     def _add_text(self, data=Union[DataFrame, List[Dict], pa.Table], pbar=None):
         """
         Add text data to the dataset.
```

### Comparing `nomic-3.0.8/nomic/embed.py` & `nomic-3.0.9/nomic/embed.py`

 * *Files identical despite different names*

### Comparing `nomic-3.0.8/nomic/pl_callbacks/pl_callback.py` & `nomic-3.0.9/nomic/pl_callbacks/pl_callback.py`

 * *Files identical despite different names*

### Comparing `nomic-3.0.8/nomic/settings.py` & `nomic-3.0.9/nomic/settings.py`

 * *Files identical despite different names*

### Comparing `nomic-3.0.8/nomic/tests/test_atlas_client.py` & `nomic-3.0.9/nomic/tests/test_atlas_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -359,22 +359,19 @@
 
 
 def test_map_text_pandas():
     size = 50
     data = pd.DataFrame(
         {
             'field': [str(uuid.uuid4()) for i in range(size)],
-            'id': [str(uuid.uuid4()) for i in range(size)],
             'color': [random.choice(['red', 'blue', 'green']) for i in range(size)],
         }
     )
 
-    dataset = atlas.map_data(
-        identifier='UNITTEST_pandas_text', id_field='id', indexed_field="color", data=data, is_public=True
-    )
+    dataset = atlas.map_data(identifier='UNITTEST_pandas_text', indexed_field="color", data=data, is_public=True)
 
     assert dataset.total_datums == 50
 
     dataset.delete()
 
 
 def test_map_text_arrow():
```

### Comparing `nomic-3.0.8/nomic/utils.py` & `nomic-3.0.9/nomic/utils.py`

 * *Files identical despite different names*

### Comparing `nomic-3.0.8/setup.py` & `nomic-3.0.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 description = 'The official Nomic python client.'
     
 setup(
     name='nomic',
-    version='3.0.8',
+    version='3.0.9',
     url='https://github.com/nomic-ai/nomic',
     description=description,
     long_description=description,
     packages=find_packages(),
     author_email="support@nomic.ai",
     author="nomic.ai",
     classifiers=[
```

